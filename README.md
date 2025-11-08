bd basico:
-- Crear la base de datos
CREATE DATABASE Proyecto;
GO

-- Usar la base recién creada
USE Proyecto;
GO

-- Crear la tabla persona
CREATE TABLE persona (
    nombre VARCHAR(60) PRIMARY KEY,
    edad INT CHECK (edad >= 19 AND edad <= 30),
    genero CHAR(1) CHECK (genero IN ('F', 'M'))
);
GO
select * from persona
