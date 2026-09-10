# 💻 Nome do Projeto

Leiloes TDS - UC11 - Atividade 1

## 👉 Explicação do Projeto

Projeto feito em Java, utilizando Banco de Dados e usado para praticar o versionamento local e remoto

## 📢 Tecnologias utilizadas

![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white) ![MySQL](https://img.shields.io/badge/mysql-%234479A1.svg?style=for-the-badge&logo=mysql&logoColor=white)

## ☕ Exemplo de código de conexão

```java
public class conectaDAO {
    public Connection connectDB(){
        Connection conn = null;
        try {
            conn = DriverManager.getConnection("jdbc:mysql://localhost/uc11?user=root&password=");  
        } catch (SQLException erro){
            JOptionPane.showMessageDialog(null, "Erro ConectaDAO" + erro.getMessage());
        }
        return conn;
    }
}
```
