# Desafio-Phishing-Dio

phishing cloner web:

# Phishing para captura de credenciais de paginas web.
site de exemplo `Instagram`.
### **ATENÇÃO**

uso dessa ferramenta é apenas para propositos legais!!!

### **Ferramentas**

- [Kali Linux](https://www.kali.org)
- [SEToolkit](https://github.com/trustedsec/social-engineer-toolkit) (pré-instalada no kali)

### **Desafios e Recomendaões**:
- Se estiver usando uma Máquina Virtual(VM), verifique se as configurações de rede estejam em modo **Bridged Adapter** ou **Placa de modo Bridge**.
- Ao clonar uma página, clone a página de login e senha.
- Verificar possiveis erros de CORS(Cross-origin Resource Sharing).
  

### **Configurando o Phishing no Kali Linux**
###### **Resumo**:
- Acesso root: ``` sudo su ```
 
  <div style="position: relative;">
  <pre><code>sudo su</code></pre>
</div>

- Iniciando o setoolkit: ``` setoolkit ```
  
  <div style="position: relative;">
  <pre><code>setoolkit</code></pre>
  
- Tipo de ataque: ``` Social-Engineering Attacks ```
- Vetor de ataque: ``` Web Site Attack Vectors ```
- Método de ataque: ```Credential Harvester Attack Method ```
- Método de ataque: ``` Site Cloner ```
- Obtendo o endereço da máquina: ``` ifconfig ```

  <div style="position: relative;">
  <pre><code>ifconfig</code></pre>
  
- URL para clone: http://www.instagram.com

### **Resutados**

![Resultado1](https://github.com/user-attachments/assets/66dedb53-e159-4f1d-af84-2c2d8f350048)

###### **passo a passo**:
1- Obetenha acesso root no kali linux, execute o seguinte comando: ``` sudo su ```.

![sudo su](https://github.com/user-attachments/assets/231b9f1d-0b97-4fad-93df-6c6f4e650ad0)

2- Após isso digite a senha e click enter.

3- Em seguida, inicie o SEToolkit, execute o comando :``` setoolkit ```

![setoolkit](https://github.com/user-attachments/assets/55c47490-e54f-45ba-8a9e-dd3f96cc050d)

4- Acessando pela primeira vez, vai solicitar apenas uma vez para aceitar os termos da ferramenta, confirme com ```y```.

![primeiro uso setoolkit](https://github.com/user-attachments/assets/b56bfe67-6984-4e84-854f-b6b67222b69e)

5- Aparecera o menu com as opções, selecione a opoção ``` 01) Social-Engineering Attacks ```.

![1](https://github.com/user-attachments/assets/e87628c4-d4e9-4c91-889c-2e0ebc284d27)

6- Em seguida selecione a opção ``` 2) Web Site Attack Vectors ```.

![2](https://github.com/user-attachments/assets/dc32b31d-d6a8-478b-848e-f18f67c2fc5f)

7- logo após a opção ```3) Credential Harvester Attack Method ```.

![3](https://github.com/user-attachments/assets/86b5fe6e-911d-4f9c-8e7f-84e8041555ea)


8- A próxima é a opção ``` 2) Site Cloner ```.

![2 site cloner](https://github.com/user-attachments/assets/fe88005f-a794-4019-8d13-6eee1fcffcd5)

9- Nessa etapa a ferramenta identifica o IP que esta rodando, o ``` setoolkit ``` vai usar a máquina como um servidor para receber as credenciais, então apenas click em ``` enter ```.

![ip](https://github.com/user-attachments/assets/ac40f173-2d12-4ee6-89ad-b3a2e5cd77fe)

10- Agora insira a url que deseja clonar e click enter, neste exemplo será ``` http://www.instagram.com ```

![url](https://github.com/user-attachments/assets/c794b4ad-7bf4-4aba-ad14-9215b6289d45)

11- Após clicar em enter, a configuração está pronta esperando alguém tentar fazer o login, a tela fica assim:

![rodando](https://github.com/user-attachments/assets/2329a244-30b6-4067-bace-e77287b761cc)

12- Envie para alguém o IP no qual você criou o clone, que é o IP da máquina(a ferramenta identificou automaticamente no passo 9)

13- Resultado: Quando alguém tentar realizar o login(com usuario e senha), aparecerá varios textos role o scroll do mouse e procure o texto em destaque conforme a imagem abaixo:

![Resultado2](https://github.com/user-attachments/assets/f33af2b3-578a-424c-af24-9053fc5cee55)
