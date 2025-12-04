# APLICA-O-NODE.JS-COM-POSTGRESQL

services:
  loja: 
    image: postgres:16
    environment:
      POSTGRES_USER: admin     
      POSTGRES_PASSWORD: admin123    
      POSTGRES_DB: Minha_loja
    ports:
      - "5432:5432"
    volumes:
      - postgres_data:/var/lib/postgresql/data

volumes:
  postgres_data:
