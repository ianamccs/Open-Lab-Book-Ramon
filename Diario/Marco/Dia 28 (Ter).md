# 28/03

## - Plugin Generator

Pelo Tutorial do Plugin Generator (https://open-ephys.atlassian.net/wiki/display/OEW/Plugin+Generator), é possível perceber que, provavelmente, terei de alterar o arquivo *ContentComponent*, como informado pelo Eliezyer. E também usar a parte de adicionar Parâmetros (do tipo numérico) ao plugin.

Fiz então a modificação de um parâmetro (largura) do módulo do RippleDetector pra fins de teste e limpei a área de plugins e os construí novamente.

## - Ripple Detector

Ao tentar rodar o plugin modificado no Open Ephys GUI (OEG) ocorreram alguns erros. Decidi então reinstalar o OEG e os Plugins padrões. Depois reinstalei o plugin do Ripple Detector, no qual tive que mudar uma configuração para que desse certo. (Mudei "ProcessorPlugin" para "PLUGIN_TYPE_PROCESSOR", na linha 53 do OpenEphysLib.cpp situado na pasta "SPWRsDetector" do Eliezyer)

E agora mudei de ideia sobre o Plugin Generator. Acredito que seja melhor modificar o código dos arquivos do RippleDetector que está funcionando que modificar os gerado pelo PluginGenerator que o Eliezyer me enviou.

 1. Fazer testes com o código contidos no diretório ./plugin-GUI/Source/SPWRsDetector tendo como base o plugins que têm as características que quero implementar (*Bandpass Filter*, pelo parâmetro numérico e *Spike Detector*, pela largura do módulo).
 
## - Testes
 
O teste de largura do módulo baseado no *Spike Detector* foi eficaz. Portanto em questão gráfica, acredito que será simples implementar as mudanças

 1. Agora será necessário saber como juntar a parte gráfica na funcionalidade de modificação dos limiares de amplitude e tempo para o RippleDetector.
 
****
[Voltar para Março](https://github.com/ramonbhaskara/Open-Lab-Book/edit/master/Diario/Marco)
