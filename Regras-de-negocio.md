# Regras de Negócio

Este documento define as principais regras de negócio aplicadas ao sistema de gerenciamento de estacionamentos.

## RN01 - Associação Veículo-Motorista
Cada veículo deve estar vinculado a um motorista, identificado pelo seu documento (CNH).

## RN02 - Vários Veículos por Motorista
Um motorista pode ter mais de um veículo cadastrado no sistema, mas ***somente um veículo poderá estar utilizando o estacionamento por vez.***

## RN03 - Validação documentos do Motorista
O motorista deve estar em dia com suas obrigações legais referentes ao **veículo** e à **CNH**. ***A faculdade não se responsabiliza por veículos estacionados cujo motorista esteja com documentos irregulares.***

## RN04 - Registro de Entrada e Saída
Cada entrada e saída de um veículo no estacionamento deve ser registrada com base no horário de ***entrada*** e ***saída***.

## RN05 - Validação de Uso
O sistema deve verificar se o motorista está ***matriculado em uma disciplina*** naquela sede específica para permitir a utilização do estacionamento.

## RN06 - Controle de Vagas
O sistema deve controlar o número de vagas disponíveis em cada sede, registrando as vagas ocupadas e livres.
