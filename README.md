# System Management — выпуски

Здесь лежат только готовые сборки System Management для Windows: установщик, Portable-версия и подписанный манифест обновления. Исходного кода здесь нет, он хранится в закрытом репозитории.

Программа сама проверяет обновления через `https://sm-update-gateway.onrender.com`. Манифест подписан ключом владельца (ECDSA P-256), а размер и SHA-256 каждого файла сверяются до запуска. Поддельное или повреждённое обновление программа не примет.

Скачать вручную можно в разделе **Releases**. Контрольные суммы SHA-256 указаны в описании каждого выпуска.

---

Ready-made builds of System Management for Windows (installer, portable, signed update manifest). No source code here. Updates are verified by the app: ECDSA P-256 signed manifest, size and SHA-256 of every file.
