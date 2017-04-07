# 07/04

## - Atualização do Lattes

Adicionei ao meu Lattes (http://lattes.cnpq.br/1593131953023142) o projeto de Iniciação Científica que estou fazendo aqui no NNC. 
E, também o evento da Semana do Cérebro como palestra que participei.

## - Plugin Generator

Tentativa de abrir o Plugin Generator para entender melhor a ferramenta e modificar o RippleDetector, que acabou sendo frustrada. 
Então pedi ajuda ao Eliezyer (Graduado em Eng. Biomédica pela UFABC que fez o RippleDetector) por email.

## - Trabalho de Graduação (Eliezyer)

Terminei a leitura do Trabalho de Graduação do Eliezyer que discorre sobre o RippleDetector e os testes realizados para construí-lo. O que dá ideia para quais são os passos a serem seguidos para a implementação dos limiares no plugin:

 1. Saber como modificar o plugin pela ferramenta do Plugin Generator  
 2. Fazer a junção dos códigos sugeridos pelo Eliezyer (Os do GitHub, do .zip que ele enviou e o "content")  
 3. Realizar testes com o plugin modificado a partir de dados já simulados   
 4. Fazer as modificações necessárias para finalizar o plugin  
 5. Verificar questão do envio do plugin para o GitHub do Open Ephys

## - Email Eliezyer

Após entrar em contato com o Eliezyer consegui instalar o Projucer a partir do diretório "plugin-GUI" com o comando `$ git checkout plugin-generator` e posteriormente, no diretório "./plugin-GUI/Projucer/Builds/LinuxMakefile", com o comando `make`.

Sendo que houve um erro: *fatal error: curl/curl.h: No such file or directory* que foi corrigido com o comando `sudo apt-get install libcurl4-openssl-dev`

Então um segundo erro ocorreu: *fatal error: X11/extensions/Xrandr.h*, corrigido por `sudo apt-get install libxrandr-dev`

E depois do terceiro erro: *fatal error: juce_File.h*, adicionando o header "juce_File.h" ao diretório "./plugin-GUI/PluginGenerator/JuceLibraryCode" o PluginGenerator deu certo!!

****
[Voltar para Março](https://github.com/ramonbhaskara/Open-Lab-Book/edit/master/Diario/Marco)
