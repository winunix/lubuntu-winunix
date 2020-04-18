# Lubuntu WinuniX 20.04 LTS

This is a fork from Lubuntu 20.04 LTS with themes and appearance of Windows System. Its for users that want migrate to a free and open source OS, but don't have technical skills.

## Generating the disc

1. Clone this repository.
2. Download the disc `lubuntu_20.04_lts.iso`.
3. Run the file `./main` without superuser.
4. Select the iso `lubuntu_20.04_lts.iso` in run time of compilation.
5. After the end of process your `iso` will available in cache folder.

## Download the disc

If you don't want to build your own disc, you can download the disc [here](#).

# Style guide for development

The project uses this style guide for better maintenance of system.

## Scaffolding

```
lubuntu-winunix/
├── main            <-- Entrypoint do projeto, use para gerar o disco
├── dependencies    <-- Dependências do Projeto
├── extract-disk    <-- Código de extração do disco
├── deploy-apps     <-- Código de implantação dos apps
├── chroot-env      <-- Código do Ambiente virtual de customização da ISO
├── pack-disk       <-- Código Empacotamento do disco
├── reset           <-- Remove pastas e arquivos nao versionado
├── modules/        <-- Bibliotecas e Apps do projeto
├── libs/           <-- Bibliotecas de terceiros (não versionado!)
├── cache/          <-- Arquivos temporários (não versionado!)
└── disk/           <-- Sistema de arquivos da ISO extraido (não versionado!) 
```