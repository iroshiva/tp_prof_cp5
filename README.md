# Esther Henna Architecte

Ce projet a été réalisé à la demande d'un architecte pour l'élaboration d'un site vitrine de présentation de projets réalisés par l'architecte.
Un MCD et un MLD ont été effectués

## Modèle Conceptuel des Données (MCD)

Réalisation du MCD avec MOCODO (cf eha_mcd.svg)<br/><br/>

> USER: userId, name, password<br/><br/>CREE, 01 PROJECT, 0N USER<br/><br/>PROJECT: projectId, title, content, project reference, moa, moe, date, mission, performance, size, cost, role<br/><br/>1_PEUT CONTENIR, 0N PROFIL PICTURE, 01 PROJECT<br/>2_PEUT CONTENIR, 0N CONTENT PICTURE, 0N PROJECT<br/><br/>PROFIL PICTURE: profilePictureId, key, filename, content_type, metadata, byte_size<br/>CONTENT PICTURE: contentPictureId, key, filename, content_type, metadata, byte_size<br/><br/>


## Modèle Logique de Données (MLD)

cf mld.md