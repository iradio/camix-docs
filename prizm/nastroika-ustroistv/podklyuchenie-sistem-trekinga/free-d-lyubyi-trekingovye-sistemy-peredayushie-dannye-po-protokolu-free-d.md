# Free-D (любый трекинговые системы передающие данные по протоколу free-D)

В разделе **Devices/Manage devices** необходимо выбрать  из выпадающего списка **Camera tracking device/Device** значение **FreeD Client**.

<figure><img src="../../../.gitbook/assets/2024-08-30 13-21-25 Camix Prizm SE (Demo mode) 2.24.0514.png" alt=""><figcaption><p>FreeD Tracking system</p></figcaption></figure>

Приложение поддерживает прием двух потоков данных по протоколу FreeD с использованием разных портов. Вы можете задать порты для приема данных по протоколу FreeD от источников (трекинга камеры и ZIF-энкодеров) в ниже в разделе **Devices/Manage devices**&#x20;

&#x20;

<figure><img src="../../../.gitbook/assets/2024-08-30 13-26-33 Camix Prizm SE (Demo mode) 2.24.0514.png" alt=""><figcaption><p>FreeD Ports </p></figcaption></figure>

После нажатия **Update** необходимо перезагрузить приложение, следуя инструкциям .

<figure><img src="../../../.gitbook/assets/2024-08-30 13-30-25 Camix Prizm SE (Demo mode) 2.24.0514.png" alt=""><figcaption></figcaption></figure>

После перезагрузки приложения, необходимо сначала запустить поток данных трекинга по протоколу FreeD на IP адрес Camix Prizm и один из указанных на предыдущем шаге портов. Убедитесь, что ваша система трекинга передает данные, затем в разделе **Devices/Camera tracking**  из выпадающего списка **Camera tracking device/Device.**

`Важно! Если в выпадающем списке`` `**`Camera tracking device/Device`**` ``не отображается поток данных FreeD Client (port), значит Camix Prizm не получает поток данных от источника. Проверьте запущена ли его передача на IP адрес Camix Prizm и верно ли указан порт.`&#x20;

<figure><img src="../../../.gitbook/assets/2024-08-30 13-31-38 Camix Prizm SE (Demo mode) 2.24.0514.png" alt=""><figcaption><p>FreeD. No data stream from Camera trackking system</p></figcaption></figure>
