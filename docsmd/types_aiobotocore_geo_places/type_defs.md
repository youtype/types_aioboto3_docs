# Type definitions

> [Index](../README.md) > [LocationServicePlacesV2](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [LocationServicePlacesV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/geo-places.html#locationserviceplacesv2)
    type annotations stubs module [types-aiobotocore-geo-places](https://pypi.org/project/types-aiobotocore-geo-places/).



## AccessPointTypeDef

```python
# AccessPointTypeDef definition

class AccessPointTypeDef(TypedDict):
    Position: NotRequired[list[float]],
```

## CategoryTypeDef

```python
# CategoryTypeDef definition

class CategoryTypeDef(TypedDict):
    Id: str,
    Name: str,
    LocalizedName: NotRequired[str],
    Primary: NotRequired[bool],
```

## AddressComponentMatchScoresTypeDef

```python
# AddressComponentMatchScoresTypeDef definition

class AddressComponentMatchScoresTypeDef(TypedDict):
    Country: NotRequired[float],
    Region: NotRequired[float],
    SubRegion: NotRequired[float],
    Locality: NotRequired[float],
    District: NotRequired[float],
    SubDistrict: NotRequired[float],
    PostalCode: NotRequired[float],
    Block: NotRequired[float],
    SubBlock: NotRequired[float],
    Intersection: NotRequired[list[float]],
    AddressNumber: NotRequired[float],
    Building: NotRequired[float],
```

## PhonemeTranscriptionTypeDef

```python
# PhonemeTranscriptionTypeDef definition

class PhonemeTranscriptionTypeDef(TypedDict):
    Value: NotRequired[str],
    Language: NotRequired[str],
    Preferred: NotRequired[bool],
```

## CountryTypeDef

```python
# CountryTypeDef definition

class CountryTypeDef(TypedDict):
    Code2: NotRequired[str],
    Code3: NotRequired[str],
    Name: NotRequired[str],
```

## RegionTypeDef

```python
# RegionTypeDef definition

class RegionTypeDef(TypedDict):
    Code: NotRequired[str],
    Name: NotRequired[str],
```

## StreetComponentsTypeDef

```python
# StreetComponentsTypeDef definition

class StreetComponentsTypeDef(TypedDict):
    BaseName: NotRequired[str],
    Type: NotRequired[str],
    TypePlacement: NotRequired[TypePlacementType],  # (1)
    TypeSeparator: NotRequired[str],
    Prefix: NotRequired[str],
    Suffix: NotRequired[str],
    Direction: NotRequired[str],
    Language: NotRequired[str],
```

1. See [:material-code-brackets: TypePlacementType](./literals.md#typeplacementtype) 
## SubRegionTypeDef

```python
# SubRegionTypeDef definition

class SubRegionTypeDef(TypedDict):
    Code: NotRequired[str],
    Name: NotRequired[str],
```

## HighlightTypeDef

```python
# HighlightTypeDef definition

class HighlightTypeDef(TypedDict):
    StartIndex: NotRequired[int],
    EndIndex: NotRequired[int],
    Value: NotRequired[str],
```

## FilterCircleTypeDef

```python
# FilterCircleTypeDef definition

class FilterCircleTypeDef(TypedDict):
    Center: Sequence[float],
    Radius: int,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## BusinessChainTypeDef

```python
# BusinessChainTypeDef definition

class BusinessChainTypeDef(TypedDict):
    Name: NotRequired[str],
    Id: NotRequired[str],
```

## FoodTypeTypeDef

```python
# FoodTypeTypeDef definition

class FoodTypeTypeDef(TypedDict):
    LocalizedName: str,
    Id: NotRequired[str],
    Primary: NotRequired[bool],
```

## GeocodeFilterTypeDef

```python
# GeocodeFilterTypeDef definition

class GeocodeFilterTypeDef(TypedDict):
    IncludeCountries: NotRequired[Sequence[str]],
    IncludePlaceTypes: NotRequired[Sequence[GeocodeFilterPlaceTypeType]],  # (1)
```

1. See [:material-code-brackets: GeocodeFilterPlaceTypeType](./literals.md#geocodefilterplacetypetype) 
## GeocodeQueryComponentsTypeDef

```python
# GeocodeQueryComponentsTypeDef definition

class GeocodeQueryComponentsTypeDef(TypedDict):
    Country: NotRequired[str],
    Region: NotRequired[str],
    SubRegion: NotRequired[str],
    Locality: NotRequired[str],
    District: NotRequired[str],
    Street: NotRequired[str],
    AddressNumber: NotRequired[str],
    PostalCode: NotRequired[str],
```

## TimeZoneTypeDef

```python
# TimeZoneTypeDef definition

class TimeZoneTypeDef(TypedDict):
    Name: str,
    Offset: NotRequired[str],
    OffsetSeconds: NotRequired[int],
```

## GetPlaceRequestRequestTypeDef

```python
# GetPlaceRequestRequestTypeDef definition

class GetPlaceRequestRequestTypeDef(TypedDict):
    PlaceId: str,
    AdditionalFeatures: NotRequired[Sequence[GetPlaceAdditionalFeatureType]],  # (1)
    Language: NotRequired[str],
    PoliticalView: NotRequired[str],
    IntendedUse: NotRequired[GetPlaceIntendedUseType],  # (2)
    Key: NotRequired[str],
```

1. See [:material-code-brackets: GetPlaceAdditionalFeatureType](./literals.md#getplaceadditionalfeaturetype) 
2. See [:material-code-brackets: GetPlaceIntendedUseType](./literals.md#getplaceintendedusetype) 
## OpeningHoursComponentsTypeDef

```python
# OpeningHoursComponentsTypeDef definition

class OpeningHoursComponentsTypeDef(TypedDict):
    OpenTime: NotRequired[str],
    OpenDuration: NotRequired[str],
    Recurrence: NotRequired[str],
```

## UspsZipPlus4TypeDef

```python
# UspsZipPlus4TypeDef definition

class UspsZipPlus4TypeDef(TypedDict):
    RecordTypeCode: NotRequired[RecordTypeCodeType],  # (1)
```

1. See [:material-code-brackets: RecordTypeCodeType](./literals.md#recordtypecodetype) 
## UspsZipTypeDef

```python
# UspsZipTypeDef definition

class UspsZipTypeDef(TypedDict):
    ZipClassificationCode: NotRequired[ZipClassificationCodeType],  # (1)
```

1. See [:material-code-brackets: ZipClassificationCodeType](./literals.md#zipclassificationcodetype) 
## QueryRefinementTypeDef

```python
# QueryRefinementTypeDef definition

class QueryRefinementTypeDef(TypedDict):
    RefinedTerm: str,
    OriginalTerm: str,
    StartIndex: int,
    EndIndex: int,
```

## ReverseGeocodeFilterTypeDef

```python
# ReverseGeocodeFilterTypeDef definition

class ReverseGeocodeFilterTypeDef(TypedDict):
    IncludePlaceTypes: NotRequired[Sequence[ReverseGeocodeFilterPlaceTypeType]],  # (1)
```

1. See [:material-code-brackets: ReverseGeocodeFilterPlaceTypeType](./literals.md#reversegeocodefilterplacetypetype) 
## SearchNearbyFilterTypeDef

```python
# SearchNearbyFilterTypeDef definition

class SearchNearbyFilterTypeDef(TypedDict):
    BoundingBox: NotRequired[Sequence[float]],
    IncludeCountries: NotRequired[Sequence[str]],
    IncludeCategories: NotRequired[Sequence[str]],
    ExcludeCategories: NotRequired[Sequence[str]],
    IncludeBusinessChains: NotRequired[Sequence[str]],
    ExcludeBusinessChains: NotRequired[Sequence[str]],
    IncludeFoodTypes: NotRequired[Sequence[str]],
    ExcludeFoodTypes: NotRequired[Sequence[str]],
```

## SuggestQueryResultTypeDef

```python
# SuggestQueryResultTypeDef definition

class SuggestQueryResultTypeDef(TypedDict):
    QueryId: NotRequired[str],
    QueryType: NotRequired[QueryTypeType],  # (1)
```

1. See [:material-code-brackets: QueryTypeType](./literals.md#querytypetype) 
## AccessRestrictionTypeDef

```python
# AccessRestrictionTypeDef definition

class AccessRestrictionTypeDef(TypedDict):
    Restricted: NotRequired[bool],
    Categories: NotRequired[list[CategoryTypeDef]],  # (1)
```

1. See [:material-code-braces: CategoryTypeDef](./type_defs.md#categorytypedef) 
## ContactDetailsTypeDef

```python
# ContactDetailsTypeDef definition

class ContactDetailsTypeDef(TypedDict):
    Label: NotRequired[str],
    Value: NotRequired[str],
    Categories: NotRequired[list[CategoryTypeDef]],  # (1)
```

1. See [:material-code-braces: CategoryTypeDef](./type_defs.md#categorytypedef) 
## ComponentMatchScoresTypeDef

```python
# ComponentMatchScoresTypeDef definition

class ComponentMatchScoresTypeDef(TypedDict):
    Title: NotRequired[float],
    Address: NotRequired[AddressComponentMatchScoresTypeDef],  # (1)
```

1. See [:material-code-braces: AddressComponentMatchScoresTypeDef](./type_defs.md#addresscomponentmatchscorestypedef) 
## AddressComponentPhonemesTypeDef

```python
# AddressComponentPhonemesTypeDef definition

class AddressComponentPhonemesTypeDef(TypedDict):
    Country: NotRequired[list[PhonemeTranscriptionTypeDef]],  # (1)
    Region: NotRequired[list[PhonemeTranscriptionTypeDef]],  # (1)
    SubRegion: NotRequired[list[PhonemeTranscriptionTypeDef]],  # (1)
    Locality: NotRequired[list[PhonemeTranscriptionTypeDef]],  # (1)
    District: NotRequired[list[PhonemeTranscriptionTypeDef]],  # (1)
    SubDistrict: NotRequired[list[PhonemeTranscriptionTypeDef]],  # (1)
    Block: NotRequired[list[PhonemeTranscriptionTypeDef]],  # (1)
    SubBlock: NotRequired[list[PhonemeTranscriptionTypeDef]],  # (1)
    Street: NotRequired[list[PhonemeTranscriptionTypeDef]],  # (1)
```

1. See [:material-code-braces: PhonemeTranscriptionTypeDef](./type_defs.md#phonemetranscriptiontypedef) 
2. See [:material-code-braces: PhonemeTranscriptionTypeDef](./type_defs.md#phonemetranscriptiontypedef) 
3. See [:material-code-braces: PhonemeTranscriptionTypeDef](./type_defs.md#phonemetranscriptiontypedef) 
4. See [:material-code-braces: PhonemeTranscriptionTypeDef](./type_defs.md#phonemetranscriptiontypedef) 
5. See [:material-code-braces: PhonemeTranscriptionTypeDef](./type_defs.md#phonemetranscriptiontypedef) 
6. See [:material-code-braces: PhonemeTranscriptionTypeDef](./type_defs.md#phonemetranscriptiontypedef) 
7. See [:material-code-braces: PhonemeTranscriptionTypeDef](./type_defs.md#phonemetranscriptiontypedef) 
8. See [:material-code-braces: PhonemeTranscriptionTypeDef](./type_defs.md#phonemetranscriptiontypedef) 
9. See [:material-code-braces: PhonemeTranscriptionTypeDef](./type_defs.md#phonemetranscriptiontypedef) 
## AddressTypeDef

```python
# AddressTypeDef definition

class AddressTypeDef(TypedDict):
    Label: NotRequired[str],
    Country: NotRequired[CountryTypeDef],  # (1)
    Region: NotRequired[RegionTypeDef],  # (2)
    SubRegion: NotRequired[SubRegionTypeDef],  # (3)
    Locality: NotRequired[str],
    District: NotRequired[str],
    SubDistrict: NotRequired[str],
    PostalCode: NotRequired[str],
    Block: NotRequired[str],
    SubBlock: NotRequired[str],
    Intersection: NotRequired[list[str]],
    Street: NotRequired[str],
    StreetComponents: NotRequired[list[StreetComponentsTypeDef]],  # (4)
    AddressNumber: NotRequired[str],
    Building: NotRequired[str],
```

1. See [:material-code-braces: CountryTypeDef](./type_defs.md#countrytypedef) 
2. See [:material-code-braces: RegionTypeDef](./type_defs.md#regiontypedef) 
3. See [:material-code-braces: SubRegionTypeDef](./type_defs.md#subregiontypedef) 
4. See [:material-code-braces: StreetComponentsTypeDef](./type_defs.md#streetcomponentstypedef) 
## CountryHighlightsTypeDef

```python
# CountryHighlightsTypeDef definition

class CountryHighlightsTypeDef(TypedDict):
    Code: NotRequired[list[HighlightTypeDef]],  # (1)
    Name: NotRequired[list[HighlightTypeDef]],  # (1)
```

1. See [:material-code-braces: HighlightTypeDef](./type_defs.md#highlighttypedef) 
2. See [:material-code-braces: HighlightTypeDef](./type_defs.md#highlighttypedef) 
## RegionHighlightsTypeDef

```python
# RegionHighlightsTypeDef definition

class RegionHighlightsTypeDef(TypedDict):
    Code: NotRequired[list[HighlightTypeDef]],  # (1)
    Name: NotRequired[list[HighlightTypeDef]],  # (1)
```

1. See [:material-code-braces: HighlightTypeDef](./type_defs.md#highlighttypedef) 
2. See [:material-code-braces: HighlightTypeDef](./type_defs.md#highlighttypedef) 
## SubRegionHighlightsTypeDef

```python
# SubRegionHighlightsTypeDef definition

class SubRegionHighlightsTypeDef(TypedDict):
    Code: NotRequired[list[HighlightTypeDef]],  # (1)
    Name: NotRequired[list[HighlightTypeDef]],  # (1)
```

1. See [:material-code-braces: HighlightTypeDef](./type_defs.md#highlighttypedef) 
2. See [:material-code-braces: HighlightTypeDef](./type_defs.md#highlighttypedef) 
## SuggestAddressHighlightsTypeDef

```python
# SuggestAddressHighlightsTypeDef definition

class SuggestAddressHighlightsTypeDef(TypedDict):
    Label: NotRequired[list[HighlightTypeDef]],  # (1)
```

1. See [:material-code-braces: HighlightTypeDef](./type_defs.md#highlighttypedef) 
## AutocompleteFilterTypeDef

```python
# AutocompleteFilterTypeDef definition

class AutocompleteFilterTypeDef(TypedDict):
    BoundingBox: NotRequired[Sequence[float]],
    Circle: NotRequired[FilterCircleTypeDef],  # (1)
    IncludeCountries: NotRequired[Sequence[str]],
    IncludePlaceTypes: NotRequired[Sequence[AutocompleteFilterPlaceTypeType]],  # (2)
```

1. See [:material-code-braces: FilterCircleTypeDef](./type_defs.md#filtercircletypedef) 
2. See [:material-code-brackets: AutocompleteFilterPlaceTypeType](./literals.md#autocompletefilterplacetypetype) 
## SearchTextFilterTypeDef

```python
# SearchTextFilterTypeDef definition

class SearchTextFilterTypeDef(TypedDict):
    BoundingBox: NotRequired[Sequence[float]],
    Circle: NotRequired[FilterCircleTypeDef],  # (1)
    IncludeCountries: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: FilterCircleTypeDef](./type_defs.md#filtercircletypedef) 
## SuggestFilterTypeDef

```python
# SuggestFilterTypeDef definition

class SuggestFilterTypeDef(TypedDict):
    BoundingBox: NotRequired[Sequence[float]],
    Circle: NotRequired[FilterCircleTypeDef],  # (1)
    IncludeCountries: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: FilterCircleTypeDef](./type_defs.md#filtercircletypedef) 
## GeocodeRequestRequestTypeDef

```python
# GeocodeRequestRequestTypeDef definition

class GeocodeRequestRequestTypeDef(TypedDict):
    QueryText: NotRequired[str],
    QueryComponents: NotRequired[GeocodeQueryComponentsTypeDef],  # (1)
    MaxResults: NotRequired[int],
    BiasPosition: NotRequired[Sequence[float]],
    Filter: NotRequired[GeocodeFilterTypeDef],  # (2)
    AdditionalFeatures: NotRequired[Sequence[GeocodeAdditionalFeatureType]],  # (3)
    Language: NotRequired[str],
    PoliticalView: NotRequired[str],
    IntendedUse: NotRequired[GeocodeIntendedUseType],  # (4)
    Key: NotRequired[str],
```

1. See [:material-code-braces: GeocodeQueryComponentsTypeDef](./type_defs.md#geocodequerycomponentstypedef) 
2. See [:material-code-braces: GeocodeFilterTypeDef](./type_defs.md#geocodefiltertypedef) 
3. See [:material-code-brackets: GeocodeAdditionalFeatureType](./literals.md#geocodeadditionalfeaturetype) 
4. See [:material-code-brackets: GeocodeIntendedUseType](./literals.md#geocodeintendedusetype) 
## OpeningHoursTypeDef

```python
# OpeningHoursTypeDef definition

class OpeningHoursTypeDef(TypedDict):
    Display: NotRequired[list[str]],
    OpenNow: NotRequired[bool],
    Components: NotRequired[list[OpeningHoursComponentsTypeDef]],  # (1)
    Categories: NotRequired[list[CategoryTypeDef]],  # (2)
```

1. See [:material-code-braces: OpeningHoursComponentsTypeDef](./type_defs.md#openinghourscomponentstypedef) 
2. See [:material-code-braces: CategoryTypeDef](./type_defs.md#categorytypedef) 
## PostalCodeDetailsTypeDef

```python
# PostalCodeDetailsTypeDef definition

class PostalCodeDetailsTypeDef(TypedDict):
    PostalCode: NotRequired[str],
    PostalAuthority: NotRequired[PostalAuthorityType],  # (1)
    PostalCodeType: NotRequired[PostalCodeTypeType],  # (2)
    UspsZip: NotRequired[UspsZipTypeDef],  # (3)
    UspsZipPlus4: NotRequired[UspsZipPlus4TypeDef],  # (4)
```

1. See [:material-code-brackets: PostalAuthorityType](./literals.md#postalauthoritytype) 
2. See [:material-code-brackets: PostalCodeTypeType](./literals.md#postalcodetypetype) 
3. See [:material-code-braces: UspsZipTypeDef](./type_defs.md#uspsziptypedef) 
4. See [:material-code-braces: UspsZipPlus4TypeDef](./type_defs.md#uspszipplus4typedef) 
## ReverseGeocodeRequestRequestTypeDef

```python
# ReverseGeocodeRequestRequestTypeDef definition

class ReverseGeocodeRequestRequestTypeDef(TypedDict):
    QueryPosition: Sequence[float],
    QueryRadius: NotRequired[int],
    MaxResults: NotRequired[int],
    Filter: NotRequired[ReverseGeocodeFilterTypeDef],  # (1)
    AdditionalFeatures: NotRequired[Sequence[ReverseGeocodeAdditionalFeatureType]],  # (2)
    Language: NotRequired[str],
    PoliticalView: NotRequired[str],
    IntendedUse: NotRequired[ReverseGeocodeIntendedUseType],  # (3)
    Key: NotRequired[str],
```

1. See [:material-code-braces: ReverseGeocodeFilterTypeDef](./type_defs.md#reversegeocodefiltertypedef) 
2. See [:material-code-brackets: ReverseGeocodeAdditionalFeatureType](./literals.md#reversegeocodeadditionalfeaturetype) 
3. See [:material-code-brackets: ReverseGeocodeIntendedUseType](./literals.md#reversegeocodeintendedusetype) 
## SearchNearbyRequestRequestTypeDef

```python
# SearchNearbyRequestRequestTypeDef definition

class SearchNearbyRequestRequestTypeDef(TypedDict):
    QueryPosition: Sequence[float],
    QueryRadius: NotRequired[int],
    MaxResults: NotRequired[int],
    Filter: NotRequired[SearchNearbyFilterTypeDef],  # (1)
    AdditionalFeatures: NotRequired[Sequence[SearchNearbyAdditionalFeatureType]],  # (2)
    Language: NotRequired[str],
    PoliticalView: NotRequired[str],
    IntendedUse: NotRequired[SearchNearbyIntendedUseType],  # (3)
    NextToken: NotRequired[str],
    Key: NotRequired[str],
```

1. See [:material-code-braces: SearchNearbyFilterTypeDef](./type_defs.md#searchnearbyfiltertypedef) 
2. See [:material-code-brackets: SearchNearbyAdditionalFeatureType](./literals.md#searchnearbyadditionalfeaturetype) 
3. See [:material-code-brackets: SearchNearbyIntendedUseType](./literals.md#searchnearbyintendedusetype) 
## ContactsTypeDef

```python
# ContactsTypeDef definition

class ContactsTypeDef(TypedDict):
    Phones: NotRequired[list[ContactDetailsTypeDef]],  # (1)
    Faxes: NotRequired[list[ContactDetailsTypeDef]],  # (1)
    Websites: NotRequired[list[ContactDetailsTypeDef]],  # (1)
    Emails: NotRequired[list[ContactDetailsTypeDef]],  # (1)
```

1. See [:material-code-braces: ContactDetailsTypeDef](./type_defs.md#contactdetailstypedef) 
2. See [:material-code-braces: ContactDetailsTypeDef](./type_defs.md#contactdetailstypedef) 
3. See [:material-code-braces: ContactDetailsTypeDef](./type_defs.md#contactdetailstypedef) 
4. See [:material-code-braces: ContactDetailsTypeDef](./type_defs.md#contactdetailstypedef) 
## MatchScoreDetailsTypeDef

```python
# MatchScoreDetailsTypeDef definition

class MatchScoreDetailsTypeDef(TypedDict):
    Overall: NotRequired[float],
    Components: NotRequired[ComponentMatchScoresTypeDef],  # (1)
```

1. See [:material-code-braces: ComponentMatchScoresTypeDef](./type_defs.md#componentmatchscorestypedef) 
## PhonemeDetailsTypeDef

```python
# PhonemeDetailsTypeDef definition

class PhonemeDetailsTypeDef(TypedDict):
    Title: NotRequired[list[PhonemeTranscriptionTypeDef]],  # (1)
    Address: NotRequired[AddressComponentPhonemesTypeDef],  # (2)
```

1. See [:material-code-braces: PhonemeTranscriptionTypeDef](./type_defs.md#phonemetranscriptiontypedef) 
2. See [:material-code-braces: AddressComponentPhonemesTypeDef](./type_defs.md#addresscomponentphonemestypedef) 
## AutocompleteAddressHighlightsTypeDef

```python
# AutocompleteAddressHighlightsTypeDef definition

class AutocompleteAddressHighlightsTypeDef(TypedDict):
    Label: NotRequired[list[HighlightTypeDef]],  # (1)
    Country: NotRequired[CountryHighlightsTypeDef],  # (2)
    Region: NotRequired[RegionHighlightsTypeDef],  # (3)
    SubRegion: NotRequired[SubRegionHighlightsTypeDef],  # (4)
    Locality: NotRequired[list[HighlightTypeDef]],  # (1)
    District: NotRequired[list[HighlightTypeDef]],  # (1)
    SubDistrict: NotRequired[list[HighlightTypeDef]],  # (1)
    Street: NotRequired[list[HighlightTypeDef]],  # (1)
    Block: NotRequired[list[HighlightTypeDef]],  # (1)
    SubBlock: NotRequired[list[HighlightTypeDef]],  # (1)
    Intersection: NotRequired[list[list[HighlightTypeDef]]],  # (11)
    PostalCode: NotRequired[list[HighlightTypeDef]],  # (1)
    AddressNumber: NotRequired[list[HighlightTypeDef]],  # (1)
    Building: NotRequired[list[HighlightTypeDef]],  # (1)
```

1. See [:material-code-braces: HighlightTypeDef](./type_defs.md#highlighttypedef) 
2. See [:material-code-braces: CountryHighlightsTypeDef](./type_defs.md#countryhighlightstypedef) 
3. See [:material-code-braces: RegionHighlightsTypeDef](./type_defs.md#regionhighlightstypedef) 
4. See [:material-code-braces: SubRegionHighlightsTypeDef](./type_defs.md#subregionhighlightstypedef) 
5. See [:material-code-braces: HighlightTypeDef](./type_defs.md#highlighttypedef) 
6. See [:material-code-braces: HighlightTypeDef](./type_defs.md#highlighttypedef) 
7. See [:material-code-braces: HighlightTypeDef](./type_defs.md#highlighttypedef) 
8. See [:material-code-braces: HighlightTypeDef](./type_defs.md#highlighttypedef) 
9. See [:material-code-braces: HighlightTypeDef](./type_defs.md#highlighttypedef) 
10. See [:material-code-braces: HighlightTypeDef](./type_defs.md#highlighttypedef) 
11. See [:material-code-braces: HighlightTypeDef](./type_defs.md#highlighttypedef) 
12. See [:material-code-braces: HighlightTypeDef](./type_defs.md#highlighttypedef) 
13. See [:material-code-braces: HighlightTypeDef](./type_defs.md#highlighttypedef) 
14. See [:material-code-braces: HighlightTypeDef](./type_defs.md#highlighttypedef) 
## SuggestHighlightsTypeDef

```python
# SuggestHighlightsTypeDef definition

class SuggestHighlightsTypeDef(TypedDict):
    Title: NotRequired[list[HighlightTypeDef]],  # (1)
    Address: NotRequired[SuggestAddressHighlightsTypeDef],  # (2)
```

1. See [:material-code-braces: HighlightTypeDef](./type_defs.md#highlighttypedef) 
2. See [:material-code-braces: SuggestAddressHighlightsTypeDef](./type_defs.md#suggestaddresshighlightstypedef) 
## AutocompleteRequestRequestTypeDef

```python
# AutocompleteRequestRequestTypeDef definition

class AutocompleteRequestRequestTypeDef(TypedDict):
    QueryText: str,
    MaxResults: NotRequired[int],
    BiasPosition: NotRequired[Sequence[float]],
    Filter: NotRequired[AutocompleteFilterTypeDef],  # (1)
    PostalCodeMode: NotRequired[PostalCodeModeType],  # (2)
    AdditionalFeatures: NotRequired[Sequence[AutocompleteAdditionalFeatureType]],  # (3)
    Language: NotRequired[str],
    PoliticalView: NotRequired[str],
    IntendedUse: NotRequired[AutocompleteIntendedUseType],  # (4)
    Key: NotRequired[str],
```

1. See [:material-code-braces: AutocompleteFilterTypeDef](./type_defs.md#autocompletefiltertypedef) 
2. See [:material-code-brackets: PostalCodeModeType](./literals.md#postalcodemodetype) 
3. See [:material-code-brackets: AutocompleteAdditionalFeatureType](./literals.md#autocompleteadditionalfeaturetype) 
4. See [:material-code-brackets: AutocompleteIntendedUseType](./literals.md#autocompleteintendedusetype) 
## SearchTextRequestRequestTypeDef

```python
# SearchTextRequestRequestTypeDef definition

class SearchTextRequestRequestTypeDef(TypedDict):
    QueryText: NotRequired[str],
    QueryId: NotRequired[str],
    MaxResults: NotRequired[int],
    BiasPosition: NotRequired[Sequence[float]],
    Filter: NotRequired[SearchTextFilterTypeDef],  # (1)
    AdditionalFeatures: NotRequired[Sequence[SearchTextAdditionalFeatureType]],  # (2)
    Language: NotRequired[str],
    PoliticalView: NotRequired[str],
    IntendedUse: NotRequired[SearchTextIntendedUseType],  # (3)
    NextToken: NotRequired[str],
    Key: NotRequired[str],
```

1. See [:material-code-braces: SearchTextFilterTypeDef](./type_defs.md#searchtextfiltertypedef) 
2. See [:material-code-brackets: SearchTextAdditionalFeatureType](./literals.md#searchtextadditionalfeaturetype) 
3. See [:material-code-brackets: SearchTextIntendedUseType](./literals.md#searchtextintendedusetype) 
## SuggestRequestRequestTypeDef

```python
# SuggestRequestRequestTypeDef definition

class SuggestRequestRequestTypeDef(TypedDict):
    QueryText: str,
    MaxResults: NotRequired[int],
    MaxQueryRefinements: NotRequired[int],
    BiasPosition: NotRequired[Sequence[float]],
    Filter: NotRequired[SuggestFilterTypeDef],  # (1)
    AdditionalFeatures: NotRequired[Sequence[SuggestAdditionalFeatureType]],  # (2)
    Language: NotRequired[str],
    PoliticalView: NotRequired[str],
    IntendedUse: NotRequired[SuggestIntendedUseType],  # (3)
    Key: NotRequired[str],
```

1. See [:material-code-braces: SuggestFilterTypeDef](./type_defs.md#suggestfiltertypedef) 
2. See [:material-code-brackets: SuggestAdditionalFeatureType](./literals.md#suggestadditionalfeaturetype) 
3. See [:material-code-brackets: SuggestIntendedUseType](./literals.md#suggestintendedusetype) 
## ReverseGeocodeResultItemTypeDef

```python
# ReverseGeocodeResultItemTypeDef definition

class ReverseGeocodeResultItemTypeDef(TypedDict):
    PlaceId: str,
    PlaceType: PlaceTypeType,  # (1)
    Title: str,
    Address: NotRequired[AddressTypeDef],  # (2)
    AddressNumberCorrected: NotRequired[bool],
    PostalCodeDetails: NotRequired[list[PostalCodeDetailsTypeDef]],  # (3)
    Position: NotRequired[list[float]],
    Distance: NotRequired[int],
    MapView: NotRequired[list[float]],
    Categories: NotRequired[list[CategoryTypeDef]],  # (4)
    FoodTypes: NotRequired[list[FoodTypeTypeDef]],  # (5)
    AccessPoints: NotRequired[list[AccessPointTypeDef]],  # (6)
    TimeZone: NotRequired[TimeZoneTypeDef],  # (7)
    PoliticalView: NotRequired[str],
```

1. See [:material-code-brackets: PlaceTypeType](./literals.md#placetypetype) 
2. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
3. See [:material-code-braces: PostalCodeDetailsTypeDef](./type_defs.md#postalcodedetailstypedef) 
4. See [:material-code-braces: CategoryTypeDef](./type_defs.md#categorytypedef) 
5. See [:material-code-braces: FoodTypeTypeDef](./type_defs.md#foodtypetypedef) 
6. See [:material-code-braces: AccessPointTypeDef](./type_defs.md#accesspointtypedef) 
7. See [:material-code-braces: TimeZoneTypeDef](./type_defs.md#timezonetypedef) 
## GeocodeResultItemTypeDef

```python
# GeocodeResultItemTypeDef definition

class GeocodeResultItemTypeDef(TypedDict):
    PlaceId: str,
    PlaceType: PlaceTypeType,  # (1)
    Title: str,
    Address: NotRequired[AddressTypeDef],  # (2)
    AddressNumberCorrected: NotRequired[bool],
    PostalCodeDetails: NotRequired[list[PostalCodeDetailsTypeDef]],  # (3)
    Position: NotRequired[list[float]],
    Distance: NotRequired[int],
    MapView: NotRequired[list[float]],
    Categories: NotRequired[list[CategoryTypeDef]],  # (4)
    FoodTypes: NotRequired[list[FoodTypeTypeDef]],  # (5)
    AccessPoints: NotRequired[list[AccessPointTypeDef]],  # (6)
    TimeZone: NotRequired[TimeZoneTypeDef],  # (7)
    PoliticalView: NotRequired[str],
    MatchScores: NotRequired[MatchScoreDetailsTypeDef],  # (8)
```

1. See [:material-code-brackets: PlaceTypeType](./literals.md#placetypetype) 
2. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
3. See [:material-code-braces: PostalCodeDetailsTypeDef](./type_defs.md#postalcodedetailstypedef) 
4. See [:material-code-braces: CategoryTypeDef](./type_defs.md#categorytypedef) 
5. See [:material-code-braces: FoodTypeTypeDef](./type_defs.md#foodtypetypedef) 
6. See [:material-code-braces: AccessPointTypeDef](./type_defs.md#accesspointtypedef) 
7. See [:material-code-braces: TimeZoneTypeDef](./type_defs.md#timezonetypedef) 
8. See [:material-code-braces: MatchScoreDetailsTypeDef](./type_defs.md#matchscoredetailstypedef) 
## GetPlaceResponseTypeDef

```python
# GetPlaceResponseTypeDef definition

class GetPlaceResponseTypeDef(TypedDict):
    PlaceId: str,
    PlaceType: PlaceTypeType,  # (1)
    Title: str,
    PricingBucket: str,
    Address: AddressTypeDef,  # (2)
    AddressNumberCorrected: bool,
    PostalCodeDetails: list[PostalCodeDetailsTypeDef],  # (3)
    Position: list[float],
    MapView: list[float],
    Categories: list[CategoryTypeDef],  # (4)
    FoodTypes: list[FoodTypeTypeDef],  # (5)
    BusinessChains: list[BusinessChainTypeDef],  # (6)
    Contacts: ContactsTypeDef,  # (7)
    OpeningHours: list[OpeningHoursTypeDef],  # (8)
    AccessPoints: list[AccessPointTypeDef],  # (9)
    AccessRestrictions: list[AccessRestrictionTypeDef],  # (10)
    TimeZone: TimeZoneTypeDef,  # (11)
    PoliticalView: str,
    Phonemes: PhonemeDetailsTypeDef,  # (12)
    ResponseMetadata: ResponseMetadataTypeDef,  # (13)
```

1. See [:material-code-brackets: PlaceTypeType](./literals.md#placetypetype) 
2. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
3. See [:material-code-braces: PostalCodeDetailsTypeDef](./type_defs.md#postalcodedetailstypedef) 
4. See [:material-code-braces: CategoryTypeDef](./type_defs.md#categorytypedef) 
5. See [:material-code-braces: FoodTypeTypeDef](./type_defs.md#foodtypetypedef) 
6. See [:material-code-braces: BusinessChainTypeDef](./type_defs.md#businesschaintypedef) 
7. See [:material-code-braces: ContactsTypeDef](./type_defs.md#contactstypedef) 
8. See [:material-code-braces: OpeningHoursTypeDef](./type_defs.md#openinghourstypedef) 
9. See [:material-code-braces: AccessPointTypeDef](./type_defs.md#accesspointtypedef) 
10. See [:material-code-braces: AccessRestrictionTypeDef](./type_defs.md#accessrestrictiontypedef) 
11. See [:material-code-braces: TimeZoneTypeDef](./type_defs.md#timezonetypedef) 
12. See [:material-code-braces: PhonemeDetailsTypeDef](./type_defs.md#phonemedetailstypedef) 
13. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchNearbyResultItemTypeDef

```python
# SearchNearbyResultItemTypeDef definition

class SearchNearbyResultItemTypeDef(TypedDict):
    PlaceId: str,
    PlaceType: PlaceTypeType,  # (1)
    Title: str,
    Address: NotRequired[AddressTypeDef],  # (2)
    AddressNumberCorrected: NotRequired[bool],
    Position: NotRequired[list[float]],
    Distance: NotRequired[int],
    MapView: NotRequired[list[float]],
    Categories: NotRequired[list[CategoryTypeDef]],  # (3)
    FoodTypes: NotRequired[list[FoodTypeTypeDef]],  # (4)
    BusinessChains: NotRequired[list[BusinessChainTypeDef]],  # (5)
    Contacts: NotRequired[ContactsTypeDef],  # (6)
    OpeningHours: NotRequired[list[OpeningHoursTypeDef]],  # (7)
    AccessPoints: NotRequired[list[AccessPointTypeDef]],  # (8)
    AccessRestrictions: NotRequired[list[AccessRestrictionTypeDef]],  # (9)
    TimeZone: NotRequired[TimeZoneTypeDef],  # (10)
    PoliticalView: NotRequired[str],
    Phonemes: NotRequired[PhonemeDetailsTypeDef],  # (11)
```

1. See [:material-code-brackets: PlaceTypeType](./literals.md#placetypetype) 
2. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
3. See [:material-code-braces: CategoryTypeDef](./type_defs.md#categorytypedef) 
4. See [:material-code-braces: FoodTypeTypeDef](./type_defs.md#foodtypetypedef) 
5. See [:material-code-braces: BusinessChainTypeDef](./type_defs.md#businesschaintypedef) 
6. See [:material-code-braces: ContactsTypeDef](./type_defs.md#contactstypedef) 
7. See [:material-code-braces: OpeningHoursTypeDef](./type_defs.md#openinghourstypedef) 
8. See [:material-code-braces: AccessPointTypeDef](./type_defs.md#accesspointtypedef) 
9. See [:material-code-braces: AccessRestrictionTypeDef](./type_defs.md#accessrestrictiontypedef) 
10. See [:material-code-braces: TimeZoneTypeDef](./type_defs.md#timezonetypedef) 
11. See [:material-code-braces: PhonemeDetailsTypeDef](./type_defs.md#phonemedetailstypedef) 
## SearchTextResultItemTypeDef

```python
# SearchTextResultItemTypeDef definition

class SearchTextResultItemTypeDef(TypedDict):
    PlaceId: str,
    PlaceType: PlaceTypeType,  # (1)
    Title: str,
    Address: NotRequired[AddressTypeDef],  # (2)
    AddressNumberCorrected: NotRequired[bool],
    Position: NotRequired[list[float]],
    Distance: NotRequired[int],
    MapView: NotRequired[list[float]],
    Categories: NotRequired[list[CategoryTypeDef]],  # (3)
    FoodTypes: NotRequired[list[FoodTypeTypeDef]],  # (4)
    BusinessChains: NotRequired[list[BusinessChainTypeDef]],  # (5)
    Contacts: NotRequired[ContactsTypeDef],  # (6)
    OpeningHours: NotRequired[list[OpeningHoursTypeDef]],  # (7)
    AccessPoints: NotRequired[list[AccessPointTypeDef]],  # (8)
    AccessRestrictions: NotRequired[list[AccessRestrictionTypeDef]],  # (9)
    TimeZone: NotRequired[TimeZoneTypeDef],  # (10)
    PoliticalView: NotRequired[str],
    Phonemes: NotRequired[PhonemeDetailsTypeDef],  # (11)
```

1. See [:material-code-brackets: PlaceTypeType](./literals.md#placetypetype) 
2. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
3. See [:material-code-braces: CategoryTypeDef](./type_defs.md#categorytypedef) 
4. See [:material-code-braces: FoodTypeTypeDef](./type_defs.md#foodtypetypedef) 
5. See [:material-code-braces: BusinessChainTypeDef](./type_defs.md#businesschaintypedef) 
6. See [:material-code-braces: ContactsTypeDef](./type_defs.md#contactstypedef) 
7. See [:material-code-braces: OpeningHoursTypeDef](./type_defs.md#openinghourstypedef) 
8. See [:material-code-braces: AccessPointTypeDef](./type_defs.md#accesspointtypedef) 
9. See [:material-code-braces: AccessRestrictionTypeDef](./type_defs.md#accessrestrictiontypedef) 
10. See [:material-code-braces: TimeZoneTypeDef](./type_defs.md#timezonetypedef) 
11. See [:material-code-braces: PhonemeDetailsTypeDef](./type_defs.md#phonemedetailstypedef) 
## SuggestPlaceResultTypeDef

```python
# SuggestPlaceResultTypeDef definition

class SuggestPlaceResultTypeDef(TypedDict):
    PlaceId: NotRequired[str],
    PlaceType: NotRequired[PlaceTypeType],  # (1)
    Address: NotRequired[AddressTypeDef],  # (2)
    Position: NotRequired[list[float]],
    Distance: NotRequired[int],
    MapView: NotRequired[list[float]],
    Categories: NotRequired[list[CategoryTypeDef]],  # (3)
    FoodTypes: NotRequired[list[FoodTypeTypeDef]],  # (4)
    BusinessChains: NotRequired[list[BusinessChainTypeDef]],  # (5)
    AccessPoints: NotRequired[list[AccessPointTypeDef]],  # (6)
    AccessRestrictions: NotRequired[list[AccessRestrictionTypeDef]],  # (7)
    TimeZone: NotRequired[TimeZoneTypeDef],  # (8)
    PoliticalView: NotRequired[str],
    Phonemes: NotRequired[PhonemeDetailsTypeDef],  # (9)
```

1. See [:material-code-brackets: PlaceTypeType](./literals.md#placetypetype) 
2. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
3. See [:material-code-braces: CategoryTypeDef](./type_defs.md#categorytypedef) 
4. See [:material-code-braces: FoodTypeTypeDef](./type_defs.md#foodtypetypedef) 
5. See [:material-code-braces: BusinessChainTypeDef](./type_defs.md#businesschaintypedef) 
6. See [:material-code-braces: AccessPointTypeDef](./type_defs.md#accesspointtypedef) 
7. See [:material-code-braces: AccessRestrictionTypeDef](./type_defs.md#accessrestrictiontypedef) 
8. See [:material-code-braces: TimeZoneTypeDef](./type_defs.md#timezonetypedef) 
9. See [:material-code-braces: PhonemeDetailsTypeDef](./type_defs.md#phonemedetailstypedef) 
## AutocompleteHighlightsTypeDef

```python
# AutocompleteHighlightsTypeDef definition

class AutocompleteHighlightsTypeDef(TypedDict):
    Title: NotRequired[list[HighlightTypeDef]],  # (1)
    Address: NotRequired[AutocompleteAddressHighlightsTypeDef],  # (2)
```

1. See [:material-code-braces: HighlightTypeDef](./type_defs.md#highlighttypedef) 
2. See [:material-code-braces: AutocompleteAddressHighlightsTypeDef](./type_defs.md#autocompleteaddresshighlightstypedef) 
## ReverseGeocodeResponseTypeDef

```python
# ReverseGeocodeResponseTypeDef definition

class ReverseGeocodeResponseTypeDef(TypedDict):
    PricingBucket: str,
    ResultItems: list[ReverseGeocodeResultItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReverseGeocodeResultItemTypeDef](./type_defs.md#reversegeocoderesultitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GeocodeResponseTypeDef

```python
# GeocodeResponseTypeDef definition

class GeocodeResponseTypeDef(TypedDict):
    PricingBucket: str,
    ResultItems: list[GeocodeResultItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GeocodeResultItemTypeDef](./type_defs.md#geocoderesultitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchNearbyResponseTypeDef

```python
# SearchNearbyResponseTypeDef definition

class SearchNearbyResponseTypeDef(TypedDict):
    PricingBucket: str,
    ResultItems: list[SearchNearbyResultItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SearchNearbyResultItemTypeDef](./type_defs.md#searchnearbyresultitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchTextResponseTypeDef

```python
# SearchTextResponseTypeDef definition

class SearchTextResponseTypeDef(TypedDict):
    PricingBucket: str,
    ResultItems: list[SearchTextResultItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SearchTextResultItemTypeDef](./type_defs.md#searchtextresultitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SuggestResultItemTypeDef

```python
# SuggestResultItemTypeDef definition

class SuggestResultItemTypeDef(TypedDict):
    Title: str,
    SuggestResultItemType: SuggestResultItemTypeType,  # (1)
    Place: NotRequired[SuggestPlaceResultTypeDef],  # (2)
    Query: NotRequired[SuggestQueryResultTypeDef],  # (3)
    Highlights: NotRequired[SuggestHighlightsTypeDef],  # (4)
```

1. See [:material-code-brackets: SuggestResultItemTypeType](./literals.md#suggestresultitemtypetype) 
2. See [:material-code-braces: SuggestPlaceResultTypeDef](./type_defs.md#suggestplaceresulttypedef) 
3. See [:material-code-braces: SuggestQueryResultTypeDef](./type_defs.md#suggestqueryresulttypedef) 
4. See [:material-code-braces: SuggestHighlightsTypeDef](./type_defs.md#suggesthighlightstypedef) 
## AutocompleteResultItemTypeDef

```python
# AutocompleteResultItemTypeDef definition

class AutocompleteResultItemTypeDef(TypedDict):
    PlaceId: str,
    PlaceType: PlaceTypeType,  # (1)
    Title: str,
    Address: NotRequired[AddressTypeDef],  # (2)
    Distance: NotRequired[int],
    Language: NotRequired[str],
    PoliticalView: NotRequired[str],
    Highlights: NotRequired[AutocompleteHighlightsTypeDef],  # (3)
```

1. See [:material-code-brackets: PlaceTypeType](./literals.md#placetypetype) 
2. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
3. See [:material-code-braces: AutocompleteHighlightsTypeDef](./type_defs.md#autocompletehighlightstypedef) 
## SuggestResponseTypeDef

```python
# SuggestResponseTypeDef definition

class SuggestResponseTypeDef(TypedDict):
    PricingBucket: str,
    ResultItems: list[SuggestResultItemTypeDef],  # (1)
    QueryRefinements: list[QueryRefinementTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: SuggestResultItemTypeDef](./type_defs.md#suggestresultitemtypedef) 
2. See [:material-code-braces: QueryRefinementTypeDef](./type_defs.md#queryrefinementtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AutocompleteResponseTypeDef

```python
# AutocompleteResponseTypeDef definition

class AutocompleteResponseTypeDef(TypedDict):
    PricingBucket: str,
    ResultItems: list[AutocompleteResultItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AutocompleteResultItemTypeDef](./type_defs.md#autocompleteresultitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 