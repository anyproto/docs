# Хранение и Удаление

### Хранение <a href="#storage" id="storage"></a>

Anytype в первую очередь работает в оффлайн-режиме, поэтому все данные, которые вы создаете, сначала будут сохранены локально. После этого данные синхронизируются с резервным узлом и вашими устройствами для обеспечения резервного копирования. Мы используем частную сеть [IPFS](https://docs.ipfs.tech/concepts/what-is-ipfs/) для управления хранением данных. Это пиринговая файловая система, которая способствует децентрализованному хранению данных на устройствах. Поддерживается локальная P2P-синхронизация, что означает, что вы можете синхронизировать данные между вашими устройствами напрямую, если они подключены через одну и ту же локальную сеть. Это будет работать независимо от выбранного вами режима сети, и это единственный способ синхронизировать данные между вашими устройствами, если вы используете режим только локального доступа.

#### Медиа <a href="#media" id="media"></a>

Медиафайлы не загружаются напрямую при общей синхронизации для экономии пропускной способности. Вместо этого, когда файл запрашивается, он передается на ваше устройство с резервного узла или ваших устройств в сети. Например, если у вас есть видео 4K, оно будет передано с резервного узла или P2P-устройств на ваше устройство. Таким образом, когда вы открываете объект с изображением, оно загружается. Когда вы нажимаете воспроизведение видео или аудио, оно начинает загружаться. После этого этот файл будет сохранен в кэше приложения.

Кроме того, мы используем функцию дедупликации для уменьшения объема хранилища. Например, если одно и то же изображение загружается три раза, хранится только одна копия изображения для уменьшения потребления хранилища.

Вы можете удалить весь медиаконтент с вашего мобильного устройства с помощью опции очистки кэша в iOS и Android. Это удалит все данные и заставит приложение снова полностью синхронизироваться. Поскольку загрузка медиафайлов работает локально, вы удалите весь кэшированный медиаконтент и освободите немного места.

Вы также можете управлять своими файлами на компьютере, перейдя в `Настройки пространства -> Управление пространством -> Управление файлами`.

### Удаление <a href="#deletion" id="deletion"></a>

<figure><img src="https://files.gitbook.com/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FJbcKxgThRdSa4vZyLbvH%2Fuploads%2Fgit-blob-dcb526128401892f1a4773091dbf735febb4a875%2FScreenshot%202021-11-02%20at%2016.25.23.png?alt=media" alt=""><figcaption><p>Полное удаление в Корзине</p></figcaption></figure>

Чтобы удалить объекты в Anytype, сначала их нужно переместить в корзину. После этого вы можете полностью удалить их со всех устройств, удалив их из корзины. Все ваши устройства также удалят их при подключении к интернету. Это действие необратимо, поэтому, пожалуйста, будьте осторожны.

Удаленные объекты все еще доступны в режиме только для чтения, либо из корзины, либо через ранее добавленные ссылки. Вы также можете восстановить эти объекты напрямую через режим только для чтения, не заходя в корзину.

Типы и связи, созданные Anytype, не могут быть удалены в данный момент, но могут быть удалены в будущих версиях.