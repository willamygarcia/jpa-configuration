# CONFIGURAÇÕES NECESSÁRIAS PARA O JPA

<p>
  Para fazer funcionar o framework com a especificação JPA além de possuir as bibliotecas necesssárias, devemos configurar o arquivo de persistence.xml que geralmente em projetos java ele fica localizado no diretorio META-INF do projeto java.
</p>

<p>No código abaixo temos a configuração necessária para que possamos rodar nosso projeto usando a especificação JPA</p>

  <persistence-unit name="nome-do-banco ou o nome de sua preferencia">
      <provider>org.hibernate.ejb.HibernatePersistence</provider>
      <class>o paconte com o nome da classe entidade para persistencia</class>
      <properties>
         <property name="javax.persistence.jdbc.driver" value="DRIVER do db que será ultilizado"/>
         <property name="javax.persistence.jdbc.url" value="URL do db que será ultilizado"/>
         <property name="javax.persistence.jdbc.user" value="USUÁRIO do db que será ultilizado"/>
         <property name="javax.persistence.jdbc.password" value="SENHA do db que será ultilizado"/>

         <property name="hibernate.dialect" value="DIALETO do db que será ultilizado"/>
         <property name="hibernate.hbm2ddl.auto" value="MANEIRA DE MANIPULAÇÃO DO DB"/>
         <property name="hibernate.show_sql" value="true"/>
         <property name="hibernate.format_sql" value="true"/>
      </properties>
    </persistence-unit>
