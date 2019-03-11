O LintSpy é uma extensão desenvolvida para o Visual Studio que visa facilitar o trabalho em equipe, sugerindo a adoção das melhores práticas de nomenclatura e documentação em tempo real, visando assim um código C# limpo, claro e objetivo. 

# Notas de versão

Versão | Descrição
------ | -----------
0.6.0  | Primeiro beta liberado
1.0.0  | Versão inicial
1.0.1  | Otimização de busca de prefixos

# Resumo


O LintSpy visa padronizar nomenclatura e documentação de códigos no momento da programação, sublinhando códigos em desacordo, exibindo na barra de rolagem a localização do ocorrido e sugerindo adoção das regras abaixo descritas. Também é possível visualizar todos as ocorrências através da lista de warnings do Visual Studio.

Desenvolvida pela equipe de TI da Coopavel (Cooperativa Agroindustrial de Cascavel/PR)

Veja abaixo um exemplo do LintSpy em funcionamento:

![Image not found, email me: informatica@coopavel.com.br](https://1.bp.blogspot.com/-vKw-bO3EXxg/XH1ZPYBIEuI/AAAAAAAAAYU/Sn7X_741RGwL3gB3o0Eo1kc5eXgQbCahQCK4BGAYYCw/s1600/02-1.png)
Exibição do warning no trecho incorreto e na barra de rolagem

![Image not found, email me: informatica@coopavel.com.br](https://2.bp.blogspot.com/-GuGIpk2sYNI/XH1ZPU5lY4I/AAAAAAAAAYY/qUljsc6O_u4YhoculRlJ2SRr78MXrG0_wCK4BGAYYCw/s1600/07.png)
Exibição da mensagem de erro ao deixar o cursor sobre o trecho marcado

![Image not found, email me: informatica@coopavel.com.br](https://3.bp.blogspot.com/-NKtyqrEWqGc/XH1ZPcUS-VI/AAAAAAAAAYc/nf9l0RyEyLsAzL_LZq87u5noaA-i0SGtgCK4BGAYYCw/s1600/08.png)
Exibição de possibilidade de correção

# Regras

1. Classe deve estar em Pascal Case;
2. O prefixo de variáveis deve seguir as tabelas abaixo. Classes internas não são consideradas

**Sobre Todos**

Classe | Prefixo
-------------- | ------
Collection | clt
Column | cln
Row | row

**Demais**

**Classe** | **Prefixo** | **Classe** | **Prefixo** | **Classe** | **Prefixo**
---------: | ----------- | ---------: | ----------- | ---------: | -----------
AdvRichTextBox | rtb | ImageList | ils | Short | sht
ArrayList | arl | Int | int | Splitter | spt
Bool | bln | Label | lbl | SqlCommand | scm
Boolean | bln | LinkLabel | lnk | SqlConnection | scn
Button | btn | List | lst | SqlDataAdapter | sda
Byte  | byt | ListBox | lst | StatusBar | sta
Char | chr | ListView | lvw | StreamWriter | stw
CheckBox | chk | Long | lon | String | str
CheckedListBox | clb | MaskedTextBox | txt | StringBuilder | stb
ColorDialog | cld | MemoryStream | mms | TabControl | tbc
ComboBox | cbo | Menu | mnu | TabPage | tbp
ContextMenu | cmn | MenuStrip | mns | TextBox | txt
Control | ctr | MonthCalendar | mcl | Timer | tmr
DataGridView | dgv | NotifyIcon | nti | ToolBar | tlb
DataGridViewCoopavel | dgv | NumericUpDown | nud | ToolStrip | tsp
DataSet | dts | OleDbCommand | ocm | ToolStripButton | tsb
DataTable | dtt | OleDbConnection | ocn | ToolStripMenuItem | tmi
DataView | dtv | OleDbDataAdapter | oda | ToolTip | tip
DateTime  | dta | OpenFileDialog | ofd | TrackBar | trb
DateTimePicker | dtp | PageSetup Dialog | psd | TreeView | tre
DB2Command | dcm | Panel | pnl | Uint | uin
DB2Connection | dcn | PictureBox | pic | Ulong | uln
DB2DataAdapter | dda | PrintDialog | ptd | Ushort | ush
Decimal | dec | PrintDocument | prn | VScrollBar | vsb
Dictionary | dic | PrintPreviewControl | ppc | XmlAttribute | xat
DomainUpDown | upd | PrintPreviewDialog | ppd | XmlDictionary | xdi
Double | dob | Process | prc | XmlDocument | xdo
ErrorProvider | err | Processando | pro | XmlElement | xel
Float | flt | ProgressBar | prg | XmlEntity | xen
FontDialog | ftd | RadioButton | rad | XmlNode | xnd
Formulários | frm | Regex | rgx | XmlNodeList | xnl
GroupBox | grp | RichTextBox | rtf | XmlReader | xre
HelpProvider | hlp | SaveFileDialog | sfd | XmlWriter | xwr
HScrollBar | hsb | Sbyte | sby |  | 

Classes que não estão listadas na tabela acima devem possuir o prefixo 'obj'

3. Namespace deve estar em Pascal Case;
4. Interfaces e classes abstratas devem ter o nome começando com a letra 'I';
5. Método deve possuir comentário de documentação;
6. O nome do método deve estar em Pascal Case;
7. Parâmetros de métodos devem iniciar com a letra 'p';
8. Atributos de classe devem possuir summary;
9. Underscores (_) não são permitidos para nenhum nome;
10. Constante deve estar em Upper Case (Caso em que é permitido o uso de underscores);
11. Enum deve estar em Pascal Case;
12. Interface deve estar em Pascal Case após a letra 'I';
13. Parâmetros devem estar em Pascal Case após o 'p';
14. Variáveis devem estar em Pascal Case após o prefixo;
15. Underscores (_) não são permitidos para nomes de variáveis (Caso especial);
16. Parâmetros de um método devem estar no Summary do mesmo;
