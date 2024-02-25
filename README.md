- 👋 Hi, I’m @tysarr8814
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
tysarr8814/tysarr8814 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
<?xml version="1.0" encoding="utf-8"?>
<Project ToolsVersion="4.0" DefaultTargets="Build" xmlns="http://schemas.microsoft.com/developer/msbuild/2003">
  <PropertyGroup>
    <Configuration Condition=" '$(Configuration)' == '' ">Debug</Configuration>
    <Platform Condition=" '$(Platform)' == '' ">x86</Platform>
    <ProductVersion>8.0.30703</ProductVersion>
    <SchemaVersion>2.0</SchemaVersion>
    <ProjectGuid>{181BD377-3659-411E-95D4-38CE93D0C974}</ProjectGuid>
    <OutputType>WinExe</OutputType>
    <AppDesignerFolder>Properties</AppDesignerFolder>
    <RootNamespace>BtcAddress</RootNamespace>
    <AssemblyName>BtcAddress</AssemblyName>
    <TargetFrameworkVersion>v4.0</TargetFrameworkVersion>
    <TargetFrameworkProfile>
    </TargetFrameworkProfile>
    <FileAlignment>512</FileAlignment>
    <SccProjectName>
    </SccProjectName>
    <SccLocalPath>
    </SccLocalPath>
    <SccAuxPath>
    </SccAuxPath>
    <SccProvider>
    </SccProvider>
  </PropertyGroup>
  <PropertyGroup Condition=" '$(Configuration)|$(Platform)' == 'Debug|x86' ">
    <PlatformTarget>x86</PlatformTarget>
    <DebugSymbols>true</DebugSymbols>
    <DebugType>full</DebugType>
    <Optimize>false</Optimize>
    <OutputPath>bin\Debug\</OutputPath>
    <DefineConstants>DEBUG;TRACE</DefineConstants>
    <ErrorReport>prompt</ErrorReport>
    <WarningLevel>4</WarningLevel>
  </PropertyGroup>
  <PropertyGroup Condition=" '$(Configuration)|$(Platform)' == 'Release|x86' ">
    <PlatformTarget>x86</PlatformTarget>
    <DebugType>pdbonly</DebugType>
    <Optimize>true</Optimize>
    <OutputPath>bin\Release\</OutputPath>
    <DefineConstants>TRACE</DefineConstants>
    <ErrorReport>prompt</ErrorReport>
    <WarningLevel>4</WarningLevel>
    <AllowUnsafeBlocks>true</AllowUnsafeBlocks>
  </PropertyGroup>
  <ItemGroup>
    <Reference Include="BouncyCastle.Crypto">
      <HintPath>.\BouncyCastle.Crypto.dll</HintPath>
    </Reference>
    <Reference Include="System" />
    <Reference Include="System.Core" />
    <Reference Include="System.Xml.Linq" />
    <Reference Include="System.Data.DataSetExtensions" />
    <Reference Include="System.Data" />
    <Reference Include="System.Deployment" />
    <Reference Include="System.Drawing" />
    <Reference Include="System.Windows.Forms" />
    <Reference Include="System.Xml" />
    <Reference Include="ThoughtWorks.QRCode">
      <HintPath>.\ThoughtWorks.QRCode.dll</HintPath>
    </Reference>
  </ItemGroup>
  <ItemGroup>
    <Compile Include="Barcode\Barcode128b.cs" />
    <Compile Include="Barcode\QR.cs" />
    <Compile Include="Model\Base58.cs" />
    <Compile Include="Model\Base58CheckString.cs" />
    <Compile Include="Model\Bip38Base.cs" />
    <Compile Include="Model\Bip38Confirmation.cs" />
    <Compile Include="Model\Bip38Intermediate.cs" />
    <Compile Include="Model\Bip38KeyPair.cs" />
    <Compile Include="Reports\CoinInsertDense.cs">
      <SubType>Component</SubType>
    </Compile>
    <Compile Include="CryptSharp\Helper.cs" />
    <Compile Include="CryptSharp\Pbkdf2.cs" />
    <Compile Include="Model\EncryptedKeyPair.cs" />
    <Compile Include="Model\EscrowCode.cs" />
    <Compile Include="Model\ExtraEntropy.cs" />
    <Compile Include="Forms\AddressGen.cs">
      <SubType>Form</SubType>
    </Compile>
    <Compile Include="Forms\AddressGen.Designer.cs">
      <DependentUpon>AddressGen.cs</DependentUpon>
    </Compile>
    <Compile Include="Forms\AddSingleAddress.cs">
      <SubType>Form</SubType>
    </Compile>
    <Compile Include="Forms\AddSingleAddress.Designer.cs">
      <DependentUpon>AddSingleAddress.cs</DependentUpon>
    </Compile>
    <Compile Include="Forms\Bip38ConfValidator.cs">
      <SubType>Form</SubType>
    </Compile>
    <Compile Include="Forms\Bip38ConfValidator.Designer.cs">
      <DependentUpon>Bip38ConfValidator.cs</DependentUpon>
    </Compile>
    <Compile Include="Forms\DecryptKey.cs">
      <SubType>Form</SubType>
    </Compile>
    <Compile Include="Forms\DecryptKey.Designer.cs">
      <DependentUpon>DecryptKey.cs</DependentUpon>
    </Compile>
    <Compile Include="Forms\EscrowTools.cs">
      <SubType>Form</SubType>
    </Compile>
    <Compile Include="Forms\EscrowTools.Designer.cs">
      <DependentUpon>EscrowTools.cs</DependentUpon>
    </Compile>
    <Compile Include="Forms\KeyCollectionView.cs">
      <SubType>Form</SubType>
    </Compile>
    <Compile Include="Forms\KeyCollectionView.Designer.cs">
      <DependentUpon>KeyCollectionView.cs</DependentUpon>
    </Compile>
    <Compile Include="Forms\KeyCombiner.cs">
      <SubType>Form</SubType>
    </Compile>
    <Compile Include="Forms\KeyCombiner.Designer.cs">
      <DependentUpon>KeyCombiner.cs</DependentUpon>
    </Compile>
    <Compile Include="Forms\PrintVouchers.cs">
      <SubType>Form</SubType>
    </Compile>
    <Compile Include="Forms\PrintVouchers.Designer.cs">
      <DependentUpon>PrintVouchers.cs</DependentUpon>
    </Compile>
    <Compile Include="Model\KeyCollection.cs" />
    <Compile Include="Model\KeyCollectionItem.cs" />
    <Compile Include="Model\KeyPair.cs" />
    <Compile Include="Forms\Base58Calc.cs">
      <SubType>Form</SubType>
    </Compile>
    <Compile Include="Forms\Base58Calc.Designer.cs">
      <DependentUpon>Base58Calc.cs</DependentUpon>
    </Compile>
    <Compile Include="Model\Bitcoin.cs" />
    <Compile Include="Model\Address.cs" />
    <Compile Include="Forms\Form1.cs">
      <SubType>Form</SubType>
    </Compile>
    <Compile Include="Forms\Form1.Designer.cs">
      <DependentUpon>Form1.cs</DependentUpon>
    </Compile>
    <Compile Include="Model\MiniKeyPair.cs" />
    <Compile Include="Model\MofN.cs" />
    <Compile Include="Forms\MofNcalc.cs">
      <SubType>Form</SubType>
    </Compile>
    <Compile Include="Forms\MofNcalc.Designer.cs">
      <DependentUpon>MofNcalc.cs</DependentUpon>
    </Compile>
    <Compile Include="Forms\PaperWalletPrinter.cs">
      <SubType>Form</SubType>
    </Compile>
    <Compile Include="Forms\PaperWalletPrinter.Designer.cs">
      <DependentUpon>PaperWalletPrinter.cs</DependentUpon>
    </Compile>
    <Compile Include="Model\PassphraseKeyPair.cs" />
    <Compile Include="Reports\PCPrint.cs">
      <SubType>Component</SubType>
    </Compile>
    <Compile Include="Forms\PpecKeygen.cs">
      <SubType>Form</SubType>
    </Compile>
    <Compile Include="Forms\PpecKeygen.Designer.cs">
      <DependentUpon>PpecKeygen.cs</DependentUpon>
    </Compile>
    <Compile Include="Program.cs" />
    <Compile Include="Properties\AssemblyInfo.cs" />
    <Compile Include="Model\PublicKey.cs" />
    <Compile Include="Reports\QRPrint.cs">
      <SubType>Component</SubType>
    </Compile>
    <Compile Include="CryptSharp\Salsa20Core.cs" />
    <Compile Include="CryptSharp\SCrypt.cs" />
    <Compile Include="Model\ShaPassphraseKeyPair.cs" />
    <Compile Include="Model\StringInterpreter.cs" />
    <Compile Include="Forms\Walletgen.cs">
      <SubType>Form</SubType>
    </Compile>
    <Compile Include="Forms\Walletgen.Designer.cs">
      <DependentUpon>Walletgen.cs</DependentUpon>
    </Compile>
    <Compile Include="Reports\CoinInsert.cs">
      <SubType>Component</SubType>
    </Compile>
    <EmbeddedResource Include="Forms\AddressGen.resx">
      <DependentUpon>AddressGen.cs</DependentUpon>
    </EmbeddedResource>
    <EmbeddedResource Include="Forms\AddSingleAddress.resx">
      <DependentUpon>AddSingleAddress.cs</DependentUpon>
    </EmbeddedResource>
    <EmbeddedResource Include="Forms\Base58Calc.resx">
      <DependentUpon>Base58Calc.cs</DependentUpon>
    </EmbeddedResource>
    <EmbeddedResource Include="Forms\Bip38ConfValidator.resx">
      <DependentUpon>Bip38ConfValidator.cs</DependentUpon>
    </EmbeddedResource>
    <EmbeddedResource Include="Forms\DecryptKey.resx">
      <DependentUpon>DecryptKey.cs</DependentUpon>
    </EmbeddedResource>
    <EmbeddedResource Include="Forms\EscrowTools.resx">
      <DependentUpon>EscrowTools.cs</DependentUpon>
    </EmbeddedResource>
    <EmbeddedResource Include="Forms\Form1.resx">
      <DependentUpon>Form1.cs</DependentUpon>
    </EmbeddedResource>
    <EmbeddedResource Include="Forms\KeyCollectionView.resx">
      <DependentUpon>KeyCollectionView.cs</DependentUpon>
    </EmbeddedResource>
    <EmbeddedResource Include="Forms\KeyCombiner.resx">
      <DependentUpon>KeyCombiner.cs</DependentUpon>
    </EmbeddedResource>
    <EmbeddedResource Include="Forms\MofNcalc.resx">
      <DependentUpon>MofNcalc.cs</DependentUpon>
    </EmbeddedResource>
    <EmbeddedResource Include="Forms\PaperWalletPrinter.resx">
      <DependentUpon>PaperWalletPrinter.cs</DependentUpon>
    </EmbeddedResource>
    <EmbeddedResource Include="Forms\PpecKeygen.resx">
      <DependentUpon>PpecKeygen.cs</DependentUpon>
    </EmbeddedResource>
    <EmbeddedResource Include="Forms\PrintVouchers.resx">
      <DependentUpon>PrintVouchers.cs</DependentUpon>
    </EmbeddedResource>
    <EmbeddedResource Include="Properties\Resources.resx">
      <Generator>ResXFileCodeGenerator</Generator>
      <LastGenOutput>Resources.Designer.cs</LastGenOutput>
      <SubType>Designer</SubType>
    </EmbeddedResource>
    <Compile Include="Properties\Resources.Designer.cs">
      <AutoGen>True</AutoGen>
      <DependentUpon>Resources.resx</DependentUpon>
      <DesignTime>True</DesignTime>
    </Compile>
    <EmbeddedResource Include="Forms\Walletgen.resx">
      <DependentUpon>Walletgen.cs</DependentUpon>
    </EmbeddedResource>
    <None Include="app.config" />
    <None Include="Properties\Settings.settings">
      <Generator>SettingsSingleFileGenerator</Generator>
      <LastGenOutput>Settings.Designer.cs</LastGenOutput>
    </None>
    <Compile Include="Properties\Settings.Designer.cs">
      <AutoGen>True</AutoGen>
      <DependentUpon>Settings.settings</DependentUpon>
      <DesignTimeSharedInput>True</DesignTimeSharedInput>
    </Compile>
  </ItemGroup>
  <ItemGroup>
    <Content Include="bitcoinlogo.ico" />
  </ItemGroup>
  <ItemGroup />
  <Import Project="$(MSBuildToolsPath)\Microsoft.CSharp.targets" />
  <!-- To modify your build process, add your task inside one of the targets below and uncomment it. 
       Other similar extension points exist, see Microsoft.Common.targets.
  <Target Name="BeforeBuild">
  </Target>
  <Target Name="AfterBuild">
  </Target>
  -->
</Project>
