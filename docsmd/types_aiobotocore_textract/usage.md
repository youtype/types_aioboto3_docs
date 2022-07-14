# Examples

> [Index](../README.md) > [Textract](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Textract](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract)
    type annotations stubs module [types-aiobotocore-textract](https://pypi.org/project/types-aiobotocore-textract/).

## Client

### Implicit type annotations

Can be used with `types-aioboto3[textract]` package installed.

Write your `Textract` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session


    session = Session()

    async with session.client("textract") as client:  # (1)
        result = await client.analyze_document()  # (2)
    ```

    1. client: [TextractClient](./client.md)
    2. result: [:material-code-braces: AnalyzeDocumentResponseTypeDef](./type_defs.md#analyzedocumentresponsetypedef) 






### Explicit type annotations

With `types-aioboto3-lite[textract]`
or a standalone `types_aiobotocore_textract` package, you have to explicitly specify
`client: TextractClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aioboto3.session import Session

    from types_aiobotocore_textract.client import TextractClient
    from types_aiobotocore_textract.type_defs import AnalyzeDocumentResponseTypeDef
    from types_aiobotocore_textract.type_defs import AnalyzeDocumentRequestRequestTypeDef


    session = Session()

    client: TextractClient
    async with session.client("textract") as client:  # (1)
        kwargs: AnalyzeDocumentRequestRequestTypeDef = {...}  # (2)
        result: AnalyzeDocumentResponseTypeDef = await client.analyze_document(**kwargs)  # (3)
    ```

    1. client: [TextractClient](./client.md)
    2. kwargs: [:material-code-braces: AnalyzeDocumentRequestRequestTypeDef](./type_defs.md#analyzedocumentrequestrequesttypedef) 
    3. result: [:material-code-braces: AnalyzeDocumentResponseTypeDef](./type_defs.md#analyzedocumentresponsetypedef) 






