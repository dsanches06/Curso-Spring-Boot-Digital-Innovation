##### Curso-Spring-Boot-Digital-Innovation
Curso framework Spring Boot Digital Innovation 2021



##### CURSO INTRODUÇÃO AO FRAMEWORK SPRING BOOT	



​      +======================+
​      |                AULA 01                 |
​      +======================+



##### PROBLEMAS DO SPRING

- configurações de beans em arquivos xml

- **dispatcher Servlet** e view resolver em **web.xml**

- setup manual de base de dados

- muito tempo gasto em configuração

- perda de foco em valor

  

##### SPRING BOOT 

- criado pela Spring Source em 2012

- facilita o setup de projetos Spring

- sem necessidade de criar arquivos de configuração

- foco em produtividade

- maior tempo no desenvolvimento de valor

  

##### PROBLEMAS RESOLVIDOS COM SPRING BOOT

- **produtividade** -> setup simplificado no projeto

- **starters** -> dependencias auto confiiguraveis pelo spring boot

- **execução simplificada** -> sem deploy em servidor externo

- **configuração** -> arquivo externo para configuração

- **valor** -> maior tempo em desenvolvimento de valor

  

##### ANNOTATIONS

- **@SpringBootApplication** -> aplicação Spring Boot

- **@RestController** -> para identificar a classe controller

- **@GetMapping("")** -> para criar API REST

- **@PostMapping("")** -> para criar API REST

- **@PutMapping("")** -> para criar API REST

- **@DeleteMapping("")** -> para criar API REST

- **@Configuration** -> para criar classe configuravel

- **@ConfigurationProperties("spring.datasource")** -> permite que a classe mapeia as propriedades do spring boot

- **@SuppressWarnings("unused")**-> para desativar avisos 

- **@Profile("dev/prod")** -> para ativar a configuração perfil do ambiente dev, stagging ou production

- **@Bean** -> para instanciar tipo de ambientes: dev, prod

- **@Value** -> para injetar propriedade appMessage

- **@Getter** -> para gerar metodos selectores dos atributos da classe fornecido pela dependencia lombok

- **@Setter** -> para gerar metodos modificadores dos atributos da classe fornecido pela dependencia lombok

      
      
      +======================+
      |                AULA 02                  |
      +======================+
      
      

##### CONFIGURAÇÃO MANUAL

- multiplos arquivos XML

- configuração manual do spring mvc -> dispatcher servlet, web.xml, spring-mvc.xml

- configuração manual de beans spring

- aplicado tambem ao spring data, spring security

  

##### AUTO CONFIGURATION

- **starters** -> dependencias simplificadas e auto configuraveis

- identificação e configuração automatica da dependencia

      
      
      +======================+
      |                AULA 03                  |
      +======================+
      
      

##### ANTES DO SPRING BOOT

- spring tradicional -> war precisava de um servidor de aplicação

- dependencia de um container web ou servidor de aplicação

- complexidade para configurações

- atualizações frequentes, junto com versão do projeto

- gerenciamento manual de configurações

  

##### FATJAR/UBERJAR

- artefato do projeto pronto para execução

- container web embutido na geraçaõ e execução (tomcat)

- deploy embarcado com outros containers são opcionais

- dependencias principais do projeto embarcado

- execução direta atraves de um unico java -jar

- podemos também gerar o war tradicional

      
      
      +======================+
      |                AULA 04                  |
      +======================+
      
      

##### MULTIPLOS AMBIENTES

- Ambientes para desenvolvimento, teste e produção

- Bancos de dados para cada ambiente

- Execução de testes unitários em ambiente local

- Suíte de testes completos em ambiente de teste

- Simulação do ambiente real em staging

- Deploy simplificado em produção

- Por isso criado so **SPRING BOOT PROFILES**

  

##### SPRING BOOT PROFILES

- Configurações próprias para cada ambiente

- Ambientes com sua configuração : **dev**, **prod**

- usa anotação profile nos metodos -> **@Profile("dev")**

- e depois ativa no **aplication.properties** -> **spring.profiles.active=dev**

      
      
      +======================+
      
      |                AULA 05                 |
      +======================+
      
      

##### CONFIGURAÇÕES COM ARQUIVOS PROPERTIES

- formato `base.propriedade.prop = valor`

  

##### LOMBOK

- disponibiliza varias anotações para adicionar em tempo  de compilação

- disponibiliza todas as propriedades do arquivo

      
      
      +======================+
      |                AULA 06                  |
      +======================+
      
      

##### CONFIGURAÇÕES COM ARQUIVOS YAML

- troca de formato de configurações: format  **.YML**

- formato `base:`
                                         `propriedade: valor`
                      
                      

+======================+
|                AULA 07                  |
+======================+



##### CONFIGURAÇÕES COM VARIÁVIES DE AMBIENTES

- variavel de ambiente pode ser injetada atraves da anotação **@Value** no projeto
- injecão com anotação `@Value("${ENV_DB_URL: NENHUMA}")`
- definição de valor default quando não há variavel

  