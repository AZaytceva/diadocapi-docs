DocflowV3
=========

.. warning:: Эта версия контракта — экспериментальная и может измениться.

.. code-block:: protobuf

    message DocflowV3
    {
        required SenderTitleDocflow SenderTitle = 1;
        optional ConfirmationDocflow Confirmation = 2;
        optional ProxyResponseDocflow ProxyResponse = 3;
        optional ReceiptDocflowV3 RecipientReceipt = 4;
        optional RecipientResponseDocflow RecipientResponse = 5;
        optional AmendmentRequestDocflow AmendmentRequest = 6;
        optional RevocationDocflowV3 Revocation = 7;
        optional ReceiptDocflowV3 SenderReceipt = 8;
        optional ResolutionDocflowV3 Resolution = 9;
        optional ResolutionEntitiesV3 ResolutionEntities = 10;
    }

Структура представляет состояние документооборота для одного документа.

- :doc:`SenderTitle <SenderTitleDocflow>` - информация о титуле отправителя;
- :doc:`Confirmation <ConfirmationDocflow>` - информация о подтверждении даты доставки, формируемом оператором;
- :doc:`ProxyResponse <ProxyResponseDocflow>` - информация об ответе промежуточного получателя;
- :doc:`RecipientReceipt <ReceiptDocflowV3>` - информация об извещении о получении документа (или титула отправителя для двухтитульного документа);
- :doc:`RecipientResponse <RecipientResponseDocflow>` - информация об ответном действии получателя: подписании документа, отправке второго титула или отказе в подписи;
- :doc:`AmendmentRequest <AmendmentRequestDocflow>` - информация о документообороте по запросу уточнения;
- :doc:`Revocation <RevocationDocflowV3>` - информация об аннулировании;
- :doc:`SenderReceipt <ReceiptDocflowV3>` - информация об извещении о получении титула получателя для двухтитульного документа;
- :doc:`Resolution <ResolutionDocflowV3>` - информация об актуальном статусе согласования документа/аннулировании;
- :doc:`ResolutionEntities <ResolutionEntitiesV3>` - информация о сущностях, относящихся к согласованию документа.
