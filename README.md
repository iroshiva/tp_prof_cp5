# Esther Henna Architecte

Ce projet a été réalisé à la demande d'un architecte pour l'élaboration d'un site vitrine de présentation de projets réalisés par l'architecte.
Un MCD et un MLD ont été effectués

## Modèle Conceptuel des Données (MCD)

Réalisation du MCD avec MOCODO (cf eha_mcd.svg)<br/><br/>

> USER: userId, name, password<br/><br/>CREE, 01 PROJECT, 0N USER<br/><br/>PROJECT: projectId, title, content, project reference, moa, moe, date, mission, performance, size, cost, role<br/><br/>1_PEUT CONTENIR, 0N PROFIL PICTURE, 01 PROJECT<br/>2_PEUT CONTENIR, 0N HEAD PICTURE, 01 PROJECT<br/>3_PEUT CONTENIR, 0N UP PICTURE, 01 PROJECT<br/>4_PEUT CONTENIR, 0N MIDDLE PICTURE, 01 PROJECT<br/>5_PEUT CONTENIR, 0N DOWN PICTURE, 01 PROJECT<br/>6_PEUT CONTENIR, 0N BOTTOM PICTURE, 01 PROJECT<br/><br/>PROFIL PICTURE: profilePictureId, key, filename, content_type, metadata, byte_size<br/>HEAD PICTURE: headPictureId, key, filename, content_type, metadata, byte_size<br/>UP PICTURE: upPictureId, key, filename, content_type, metadata, byte_size<br/>MIDDLE PICTURE: middlePictureId, key, filename, content_type, metadata, byte_size<br/>DOWN PICTURE: downPictureId, key, filename, content_type, metadata, byte_size<br/>BOTTOM PICTURE: bottomPictureId, key, filename, content_type, metadata, byte_size<br/><br/>

## Modèle Logique de Données (MLD)

> - User (UserId, Name, Password)<br/>
> - Project (ProjectId, title, content, ref, moa, moe, date, mission, perf, size, cost, role, #UserId)<br/>
> - Profil (ProfilePictureId, key, filename, content_type, metadata, byte_size)<br/>
> - Head (HeadPictureId, key, filename, content_type, metadata, byte_size)<br/>
> - Up (UpPictureId, key, filename, content_type, metadata, byte_size)<br/>
> - Middle (MiddlePictureId, key, filename, content_type, metadata, byte_size)<br/>
> - Down (DownPictureId, key, filename, content_type, metadata, byte_size)<br/>
> - Bottom (BottomPictureId, key, filename, content_type, metadata, byte_size)<br/>
> - 1_PEUT CONTENIR (ProjectId, ProfilePictureId)<br/>
> - 2_PEUT CONTENIR (ProjectId, HeadPictureId)<br/>
> - 3_PEUT CONTENIR (ProjectId, UpPictureId)<br/>
> - 4_PEUT CONTENIR (ProjectId, MiddlePictureId)<br/>
> - 5_PEUT CONTENIR (ProjectId, DownPictureId)<br/>
> - 6_PEUT CONTENIR (ProjectId, BottomPictureId)<br/>
