O LintSpy é uma extensão desenvolvida para o Visual Studio que visa facilitar o trabalho em equipe, sugerindo a adoção das melhores práticas de nomenclatura e documentação em tempo real, visando assim um código C# limpo, claro e objetivo.

# Notas de versão

Versão | Principais alterações
------ | -----------
0.6.0  | Primeiro beta liberado
1.0.0  | Versão inicial
1.0.1  | Otimização de busca de prefixos
1.0.2  | Prefixos internos
1.0.3  | Verificação do summary
1.0.4  | Verificação de variáveis em foreach
1.0.5  | Propriedades de classe
1.0.6  | Tipo real de declarações "var"
1.0.7  | Pequenas correções
1.0.8  | Estruturas de controle de fluxo
1.0.9  | Pequenas correções
1.1.0  | Pequenas correções
1.1.1  | Pequenas correções
1.1.2  | Verificação do documento completo

# Resumo


O LintSpy visa padronizar nomenclatura e documentação de códigos no momento da programação, sublinhando códigos em desacordo, exibindo na barra de rolagem a localização do ocorrido e sugerindo adoção das regras abaixo descritas. Também é possível visualizar todos as ocorrências através da lista de warnings do Visual Studio.

Desenvolvida pela equipe de TI da Coopavel (Cooperativa Agroindustrial de Cascavel/PR)

Veja abaixo um exemplo do LintSpy em funcionamento:

![Image not found, email me: informatica@coopavel.com.br](https://farm8.staticflickr.com/7906/33482662428_43d2fd3651_o.png)
Exibição do warning no trecho incorreto e na barra de rolagem

![Image not found, email me: informatica@coopavel.com.br](https://farm8.staticflickr.com/7849/32416775557_df5dbf56be_o.png)
Exibição da mensagem de erro ao deixar o cursor sobre o trecho marcado

![Image not found, email me: informatica@coopavel.com.br](https://farm8.staticflickr.com/7832/40393392953_6e193c0da5_o.png)
Exibição de possibilidade de correção

# Regras

1. Classes devem estar em Pascal Case;
2. O prefixo de variáveis deve seguir as tabelas na seção **Prefixos**. Classes internas não são consideradas;
3. Namespaces devem estar em Pascal Case;
4. Interfaces e classes abstratas devem ter o nome começando com a letra 'I';
5. Métodos devem possuir comentário de documentação;
6. O nome do método deve estar em Pascal Case;
7. Parâmetros de métodos devem iniciar com a letra 'p';
8. Atributos de classe devem possuir summary;
9. Underscores (_) não são permitidos para nenhum nome;
10. Constantes devem estar em Upper Case (Caso em que é permitido o uso de underscores);
11. Enums devem estar em Pascal Case;
12. Interfaces devem estar em Pascal Case após a letra 'I';
13. Parâmetros devem estar em Pascal Case após o 'p';
14. Variáveis devem estar em Pascal Case após o prefixo;
15. Underscores (_) não são permitidos para nomes de variáveis (Caso especial);
16. Parâmetros de um método devem estar no Summary do mesmo;
17. Campos do Summary não podem ficar em branco;
18. Propriedades devem estar em Pascal Case;
19. Estruturas de controle de fluxo devem possuir bloco delimitado por chaves ({});
20. Comentário não pode possuir parâmetros que não possuam correspondência;
21. Comentário deve ter o retorno do método devidamente comentado;

# Prefixos

Prefixos de variáveis possuem três letras minúsculas seguindo as tabelas abaixo descritas.

## Sobre Todos

As variáveis devem ser nomeadas utilizando o prefixo da tabela a seguir caso a classe em questão possua alguma das palavras listadas.

Palavra | Prefixo
-------------- | ------
Collection | clt
Column | cln
Row | row

## Demais

Classes que não possuam as palavras da tabela anterior devem utilizar o prefixo indicado na tabela abaixo de acordo com o nome da classe ou agrupamento.

**Classe** | **Pref.** | **Classe** | **Pref.** | **Classe** | **Pref.**
---------: | ----------- | ---------: | ----------- | ---------: | -----------
AdvRichTextBox | rtb | HScrollBar | hsb | Splitter | spt
ArrayList | arl | ImageList | ils | SqlCommand | scm
Backgroundworker | bgw | Int | int | SqlConnection | scn
Bool | bln | Jarray | jar | SqlDataAdapter | sda
Boolean | bln | Jobject | job | StatusBar | sta
Button | btn | Jtoken | jtk | StatusStrip | sst
Byte  | byt | Label | lbl | StreamWriter | stw
CampoData | txt | LinkLabel | lnk | String | str
CampoDataHora | txt | List | lst | StringBuilder | stb
CampoDecimal | txt | ListBox | lst | TabControl | tbc
CampoNumerico | txt | ListView | lvw | TabPage | tbp
CampoTelefone | txt | Long | lon | TextBox | txt
Char | chr | MaskedTextBox | txt | Textboxnumauto | txt
CheckBox | chk | MemoryStream | mms | Timer | tmr
CheckedListBox | clb | Menu | mnu | TimeSpan | tms
ColorDialog | cld | MenuStrip | mns | ToolBar | tlb
ComboBox | cbo | MonthCalendar | mcl | ToolStrip | tsp
ContextMenu | cmn | NotifyIcon | nti | ToolStripButton | tsb
Control | ctr | NumericUpDown | nud | ToolStripDrop... | 
DataGridView | dgv | OleDbCommand | ocm | DownButton | btn
DataGridViewCoopavel | dgv | OleDbConnection | ocn | ToolStripMenuItem | tmi
DataSet | dts | OleDbDataAdapter | oda | ToolStripProgressBar | prg
DataTable | dtt | OpenFileDialog | ofd | ToolStripSplitButton | btn
DataView | dtv | PageSetup Dialog | psd | ToolStripStatusLabel | lbl
DateTime  | dta | Panel | pnl | ToolTip | tip
DateTimePicker | dtp | PictureBox | pic | TrackBar | trb
DB2Command | dcm | PrintDialog | ptd | TreeView | tre
DB2Connection | dcn | PrintDocument | prn | Uint | uin
DB2DataAdapter | dda | PrintPreviewControl | ppc | Ulong | uln
Decimal | dec | PrintPreviewDialog | ppd | Ushort | ush
Dictionary | dic | Process | prc | VScrollBar | vsb
DomainUpDown | upd | Processando | pro | XmlAttribute | xat
Double | dob | ProgressBar | prg | XmlDictionary | xdi
ErrorProvider | err | RadioButton | rad | XmlDocument | xdo
Float | flt | Regex | rgx | XmlElement | xel
FontDialog | ftd | RichTextBox | rtf | XmlEntity | xen
Formulários | frm | SaveFileDialog | sfd | XmlNode | xnd
GroupBox | grp | Sbyte | sby | XmlNodeList | xnl
HelpProvider | hlp | Short | sht | XmlReader | xre
 | | | SpliterContainer | spc | XmlWriter | xwr


Classes que não se encaixam nas regras de prefixagem acima listadas devem possuir o prefixo 'obj'.
