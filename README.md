# lada2
Создал Виртуальную машину с дисками ssd1, ssd2
![1](https://user-images.githubusercontent.com/50837842/58712134-a8c9b500-83c8-11e9-94a2-aa0867ebba5c.jpg)
Посмотрел диски в системе
![2](https://user-images.githubusercontent.com/50837842/58713210-d3b50880-83ca-11e9-9663-f0df0da035fb.jpg)
Установил grub на диск, на котрый он еще не был установлен
![3](https://user-images.githubusercontent.com/50837842/58713211-d3b50880-83ca-11e9-8188-9198e3a81a7e.jpg)
Просмотрел информацию о текущем raid
![5](https://user-images.githubusercontent.com/50837842/58713213-d3b50880-83ca-11e9-8bcc-595982ff60c4.jpg)
Удалил диск ssd1, за пустил машину, проверил статус RAID-массива
![7](https://user-images.githubusercontent.com/50837842/58713215-d44d9f00-83ca-11e9-87f5-e9f0869c24cd.jpg)
![6](https://user-images.githubusercontent.com/50837842/58713214-d3b50880-83ca-11e9-8b6d-437fd13d1776.jpg)
Вывод fdisk -l
![8](https://user-images.githubusercontent.com/50837842/58713216-d44d9f00-83ca-11e9-9eca-23b5f2d8f9ae.jpg)

![9](https://user-images.githubusercontent.com/50837842/58713218-d44d9f00-83ca-11e9-97eb-26e5b7d9669d.jpg)

![10](https://user-images.githubusercontent.com/50837842/58713219-d44d9f00-83ca-11e9-81b2-91421c482b75.jpg)

![11](https://user-images.githubusercontent.com/50837842/58713221-d4e63580-83ca-11e9-949e-a25290754ea7.jpg)

![12](https://user-images.githubusercontent.com/50837842/58713223-d4e63580-83ca-11e9-8e7d-f0e14f4608cc.jpg)

![13](https://user-images.githubusercontent.com/50837842/58713225-d4e63580-83ca-11e9-964e-3e0090527b97.jpg)

![14](https://user-images.githubusercontent.com/50837842/58713227-d57ecc00-83ca-11e9-9e85-4952cdca1a22.jpg)

![15](https://user-images.githubusercontent.com/50837842/58713229-d57ecc00-83ca-11e9-8a36-74bcb0a83e62.jpg)

![16](https://user-images.githubusercontent.com/50837842/58713231-d57ecc00-83ca-11e9-95e5-43f13cbdb9c4.jpg)

![17](https://user-images.githubusercontent.com/50837842/58713234-d6176280-83ca-11e9-97d1-f03df408ed83.jpg)

![18](https://user-images.githubusercontent.com/50837842/58713237-d6176280-83ca-11e9-8ed7-62a64dfdeb16.jpg)

![19](https://user-images.githubusercontent.com/50837842/58713238-d6176280-83ca-11e9-975b-3fd6f06f6a88.jpg)
PV=2
![20](https://user-images.githubusercontent.com/50837842/58713239-d6176280-83ca-11e9-9b72-53fc8252253f.jpg)
Перенос PV
![21](https://user-images.githubusercontent.com/50837842/58713240-d6aff900-83ca-11e9-9a89-dcf36a03763e.jpg)

![22](https://user-images.githubusercontent.com/50837842/58713241-d6aff900-83ca-11e9-9620-b865768d1c3e.jpg)

![23](https://user-images.githubusercontent.com/50837842/58713242-d6aff900-83ca-11e9-98f7-738b863f0ae8.jpg)
PV=1
![24](https://user-images.githubusercontent.com/50837842/58713244-d6aff900-83ca-11e9-9455-3652496a1aec.jpg)

![25](https://user-images.githubusercontent.com/50837842/58713245-d6aff900-83ca-11e9-90b4-6a31a04ae6be.jpg)

![26](https://user-images.githubusercontent.com/50837842/58713246-d7488f80-83ca-11e9-8661-c2ee51154576.jpg)

![27](https://user-images.githubusercontent.com/50837842/58713247-d7488f80-83ca-11e9-975e-4bff8b5c0397.jpg)

![28](https://user-images.githubusercontent.com/50837842/58713248-d7488f80-83ca-11e9-8755-fd2eeda2daec.jpg)

![29](https://user-images.githubusercontent.com/50837842/58713190-d152ae80-83ca-11e9-8e70-70e1f90491cb.jpg)

![30](https://user-images.githubusercontent.com/50837842/58713191-d152ae80-83ca-11e9-90f5-eb71ad36cfe9.jpg)
Сделал pvresize
![31](https://user-images.githubusercontent.com/50837842/58713193-d152ae80-83ca-11e9-9c8b-2ad3fd5dab43.jpg)
Добавил место VG var,root
![32](https://user-images.githubusercontent.com/50837842/58713194-d1eb4500-83ca-11e9-9f27-5d17d8faab60.jpg)

![33](https://user-images.githubusercontent.com/50837842/58713196-d1eb4500-83ca-11e9-8b16-eb99c8749492.jpg)
Создал логический том val_log
![34](https://user-images.githubusercontent.com/50837842/58713197-d283db80-83ca-11e9-89f8-8882844d78d8.jpg)
lsblk
![35](https://user-images.githubusercontent.com/50837842/58713198-d283db80-83ca-11e9-8102-14da7f0587a0.jpg)
Выяснил какие процессы работают сейчас с /var/log
![36](https://user-images.githubusercontent.com/50837842/58713201-d283db80-83ca-11e9-88db-c64581c8ad93.jpg)
Поменял местами разделы
![37](https://user-images.githubusercontent.com/50837842/58713202-d283db80-83ca-11e9-901e-58234ffecb44.jpg)
Правлю /etc/fstab fstab - файл, в котором записываются правила, по которым при загрузке будут смонтированы разделы.
![38](https://user-images.githubusercontent.com/50837842/58713204-d283db80-83ca-11e9-9c1b-c10dd40e2415.jpg)
Сравниваю последствия
![39](https://user-images.githubusercontent.com/50837842/58713205-d31c7200-83ca-11e9-8460-62ecd6b4590a.jpg)
Финальный аккорд: последние проверки
![40](https://user-images.githubusercontent.com/50837842/58713207-d31c7200-83ca-11e9-8fa8-06df805f275e.jpg)
![41](https://user-images.githubusercontent.com/50837842/58713208-d31c7200-83ca-11e9-834d-e5340898d033.jpg)
