# Índice de Procedimientos Almacenados

- **Exportaciones**
  - [EXPCBE](#expcbe)
  - [EXPCCE](#expcce)
  - [expdex](#expdex)
  - [EXPNEG](#expneg)
  - [expret](#expret)

- **Financiamiento**
  - [ADMIN](#admin)
  - [COL_NEG](#col_neg)
  - [INGRESO](#ingreso)
  - [MODIFIC](#modific)
  - [OBLIGA](#obliga)
  - [PAGOS](#pagos)
  - [PGOEXT](#pgoext)

- **Importaciones**
  - [ARCOS](#arcos)
  - [COBERIMP](#coberimp)
  - [COBRANZA](#cobranza)
  - [CRDEXT](#crdext)
  - [CRD_CORR](#crd_corr)
  - [DDI](#ddi)
  - [IMPORT](#import)
  - [INFORME](#informe)
  - [MOD_ADI](#mod_adi)
  - [MOD_CBR](#mod_cbr)
  - [MOD_CRD](#mod_crd)
  - [NEGO_AV](#nego_av)
  - [NNEGO](#nnego)
  - [PAGCBR](#pagcbr)

## EXPCBE
<a name="expcbe"></a>
### Archivo: CBE00101.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_expcbe_lee_prm

#### Tablas Involucradas:
- ACMXPRMGRL

#### Procedimientos Llamados:
- sp_procxmode
- CMXsrv_lee_fpro

---

### Archivo: CBE00101.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_cmx_busc_suc_usu

#### Tablas Involucradas:
- master..sysprocesses
- tbl_User

#### Procedimientos Llamados:
- PrmACMXSUCSAL
- CMXsrv_cmx_ing_lib
- sp_procxmode

---

### Archivo: CBE00101.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_expcbe_lee_cbe

#### Tablas Involucradas:
- ACMXPAIS
- COR
- ACMXPGOCBE
- CBE01
- CBE
- ACMXMONEDA
- ACMXENTDOC
- ACMXSUCSAL
- ACMXPRTCBE
- CLN

#### Procedimientos Llamados:
- CMXsrv_cmx_busc_suc_usu
- CMXsrv_val_suc
- sp_procxmode
- CMXsrv_lee_fpro

---

### Archivo: CBE00101.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_trae_glo_fec

#### Tablas Involucradas:
- ACMXSUCSAL
- ACMXDL3475FEC
- tbl_User

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBE00101.FRM
**Segmento:** ingcomg_Click
**Procedimiento Almacenado:** CMXsrv_expcbe_avs_cyg1

#### Tablas Involucradas:
- ACMXDESEMB
- ASND
- ACMXIMPUES
- ACMXPRMGRL
- EVZ
- CBE
- COM
- TRSD
- CLN
- ACMXESPECI

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBE00101.FRM
**Segmento:** ingcomg_Click
**Procedimiento Almacenado:** CMXsrv_expcbe_avs_cyg2

#### Tablas Involucradas:
- ASND
- ACMXIMPUES
- ACMXPRMGRL
- EVZ
- CBE

#### Procedimientos Llamados:
- por
- sp_procxmode

---

### Archivo: CBE00101.FRM
**Segmento:** ingret_Click
**Procedimiento Almacenado:** CMXsrv_expcbe_avs_ret

#### Tablas Involucradas:
- ACMXPAIS
- COR
- ACMXDESEMB
- CBE
- ACMXMONEDA
- ACMXSUCSAL
- CLN
- ACMXESPECI
- RET

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBE00101.FRM
**Segmento:** M3_Click
**Procedimiento Almacenado:** CMXsrv_expcbe_swf_sel

#### Tablas Involucradas:
- switxt
- switxt1

#### Procedimientos Llamados:
- CMXsrv_expcbe_swf_422
- CMXsrv_expcbe_swf_420
- CMXsrv_expcbe_swf_499
- CMXsrv_expcbe_swf_430
- sp_procxmode

---

### Archivo: CBE00101.FRM
**Segmento:** M4_Click
**Procedimiento Almacenado:** CMXsrv_expcbe_swf_sel

#### Tablas Involucradas:
- switxt
- switxt1

#### Procedimientos Llamados:
- CMXsrv_expcbe_swf_422
- CMXsrv_expcbe_swf_420
- CMXsrv_expcbe_swf_499
- CMXsrv_expcbe_swf_430
- sp_procxmode

---

### Archivo: CBE00101.FRM
**Segmento:** Mcbeanl_Click
**Procedimiento Almacenado:** CMXsrv_expcbe_anl_cbe

#### Tablas Involucradas:
- CBE

#### Procedimientos Llamados:
- CMXsrv_cnt_gen_vig
- sp_procxmode
- CMXsrv_expcbe_grb_evz
- CMXsrv_cnt_950
- CMXsrv_cnt_630

---

### Archivo: CBE00101.FRM
**Segmento:** Mcbectb_Click
**Procedimiento Almacenado:** CMXsrv_expcbe_ctb_ing

#### Tablas Involucradas:
- OPE_BCI
- CBE

#### Procedimientos Llamados:
- CMXsrv_cnt_600
- CMXsrv_mbyte_gen
- CMXsrv_nibx_upd_tran
- CMXsrv_cnt_gen_vig
- sp_procxmode
- CMXsrv_expcbe_grb_evz
- CMXsrv_cnt_950
- CMXsrv_expcbe_val_cbe
- CMXsrv_nibx_nilive

---

### Archivo: CBE00101.FRM
**Segmento:** Mcbedel_Click
**Procedimiento Almacenado:** CMXsrv_expcbe_del_cbe

#### Tablas Involucradas:
- EVL
- CBE01
- COD
- CBE
- EVZ
- COM
- ACTZ
- CTZ

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBE00101.FRM
**Segmento:** Mcbeval_Click
**Procedimiento Almacenado:** CMXsrv_expcbe_val_cbe

#### Tablas Involucradas:
- COR
- CBE01
- ACMXPRMGRL
- CBE
- DCZ
- CTZ
- warnmsg
- ACMXPAIS
- ACMXFERIADO
- CCO

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBE00101.FRM
**Segmento:** Men1_Click
**Procedimiento Almacenado:** CMXsrv_expcbe_swf_sel

#### Tablas Involucradas:
- switxt
- switxt1

#### Procedimientos Llamados:
- CMXsrv_expcbe_swf_422
- CMXsrv_expcbe_swf_420
- CMXsrv_expcbe_swf_499
- CMXsrv_expcbe_swf_430
- sp_procxmode

---

### Archivo: CBE00201.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_expcbe_grb_ctp

#### Tablas Involucradas:
- ACMXPAIS
- CBE

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBE00201.FRM
**Segmento:** fld_cbe_cod_exp_lostfocus
**Procedimiento Almacenado:** CMXsrv_expcbe_lee_cln

#### Tablas Involucradas:
- CLN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBE00201.FRM
**Segmento:** fld_cbe_cod_suc_LostFocus
**Procedimiento Almacenado:** CMXsrv_val_suc

#### Tablas Involucradas:
- ACMXSUCSAL
- tbl_User

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBE00201.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_expcbe_lee_ctp

#### Tablas Involucradas:
- ACMXSUCSAL
- ACMXPAIS
- CBE
- CLN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBE00202.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_expcbe_grb_bco

#### Tablas Involucradas:
- ACMXPRMGRL
- CBE
- COR
- CBE01

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBE00202.FRM
**Segmento:** fld_cbe_cod_cob_Lostfocus
**Procedimiento Almacenado:** CMXsrv_expcbe_lee_cor

#### Tablas Involucradas:
- ACMXPAIS
- COR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBE00202.FRM
**Segmento:** fld_cbe_cod_rmb_LostFocus
**Procedimiento Almacenado:** CMXsrv_expcbe_lee_cor

#### Tablas Involucradas:
- ACMXPAIS
- COR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBE00202.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_expcbe_lee_bco

#### Tablas Involucradas:
- CBE
- COR
- CBE01

#### Procedimientos Llamados:
- CMXsrv_icrd_lee_cln
- sp_procxmode

---

### Archivo: CBE00204.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_expcbe_grb_doc

#### Tablas Involucradas:
- CBE
- DCZ

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBE00204.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_expcbe_grb_doc02

#### Tablas Involucradas:
- CBE02

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBE00204.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_expcbe_lee_doc

#### Tablas Involucradas:
- CBE

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBE00204.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_expcbe_lee_doc02

#### Tablas Involucradas:
- CBE02

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBE00206.FRM
**Segmento:** ELIMINAR_Click
**Procedimiento Almacenado:** CMXsrv_expcbe_del_ctz

#### Tablas Involucradas:
- ACTZ
- CBE
- CTZ

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBE00206.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_expcbe_bus_ctz

#### Tablas Involucradas:
- ACTZ
- CBE
- CTZ

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBE00207.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_expcbe_grb_ctz

#### Tablas Involucradas:
- ACTZ
- CBE
- CTZ

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBE00207.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_expcbe_mto_ctz

#### Tablas Involucradas:
- ACTZ
- CBE
- CTZ

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBE00207.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_expcbe_lee_ctz

#### Tablas Involucradas:
- ACTZ
- CBE
- CTZ

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBE00301.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_expcbe_lee_cbe

#### Tablas Involucradas:
- ACMXPAIS
- COR
- ACMXPGOCBE
- CBE01
- CBE
- ACMXMONEDA
- ACMXENTDOC
- ACMXSUCSAL
- ACMXPRTCBE
- CLN

#### Procedimientos Llamados:
- CMXsrv_cmx_busc_suc_usu
- CMXsrv_val_suc
- sp_procxmode
- CMXsrv_lee_fpro

---

### Archivo: CBE00301.FRM
**Segmento:** buscar_Click
**Procedimiento Almacenado:** CMXsrv_expcbe_bus_cbe

#### Tablas Involucradas:
- CBE

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBE00301.FRM
**Segmento:** fld_aux_cod_exp_LostFocus
**Procedimiento Almacenado:** CMXsrv_expcbe_lee_cln

#### Tablas Involucradas:
- CLN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBE00301.FRM
**Segmento:** Proximas_Click
**Procedimiento Almacenado:** CMXsrv_expcbe_bus_cbe

#### Tablas Involucradas:
- CBE

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBE00401.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_expcbe_mdf_cbe

#### Tablas Involucradas:
- ACTZ
- ACMXPRMGRL
- CBE

#### Procedimientos Llamados:
- CMXsrv_expcbe_grb_evl
- CMXsrv_expcbe_act_ctz
- CMXsrv_cnt_gen_vig
- CMXsrv_cnt_610
- sp_procxmode
- CMXsrv_expcbe_grb_evz
- CMXsrv_cnt_950
- CMXsrv_lee_fpro

---

### Archivo: CBE00401.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_expcbe_cre_actz

#### Tablas Involucradas:
- ACTZ
- CBE
- CTZ

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBE00401.FRM
**Segmento:** fld_cbe_cod_suc_LostFocus
**Procedimiento Almacenado:** CMXsrv_val_suc

#### Tablas Involucradas:
- ACMXSUCSAL
- tbl_User

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBE00401.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_expcbe_lee_mdf

#### Tablas Involucradas:
- COR
- ACMXPGOCBE
- CBE01
- CBE
- ACMXMONEDA
- ACMXSUCSAL
- CLN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBE00501.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_expcbe_pgo_cbe

#### Tablas Involucradas:
- ACMXDESEMB
- COR
- CLN
- RET
- vig_cmx
- COD
- ACMXIMPUES
- ACMXPRMGRL
- CBE
- ACMXPRMEXP
- COM
- tbl_User
- OPREC
- ACMXPAIS
- ACMXFERIADO
- CCO

#### Procedimientos Llamados:
- CMXsrv_mbyte_gen
- CMXsrv_expret_grb_org
- CMXsrv_expret_grb_dtn
- CMXsrv_cnt_gen_vig
- CMXsrv_expret_cre_ret
- CMXsrv_vig_gra_vig
- sp_procxmode
- CMXsrv_expcbe_grb_evz
- CMXsrv_cnt_950
- CMXsrv_exp_ipuc_gen_pln
- CMXsrv_expcbe_trp_cyg
- CMXsrv_expret_grb_det
- CMXsrv_cnt_620

---

### Archivo: CBE00501.FRM
**Segmento:** fld_cbe_cod_rmb_LostFocus
**Procedimiento Almacenado:** CMXsrv_expcbe_lee_cor

#### Tablas Involucradas:
- ACMXPAIS
- COR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBE00501.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_expcbe_lee_pgo

#### Tablas Involucradas:
- ACMXDESEMB
- COR
- CBE
- ACMXPRMEXP
- ACMXMONEDA
- OPREC
- CLN

#### Procedimientos Llamados:
- sp_procxmode
- CMXsrv_lee_fpro

---

### Archivo: CBE00601.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_expcbe_bus_evz

#### Tablas Involucradas:
- EVZ
- CBE

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBE00601.FRM
**Segmento:** Proximo_Click
**Procedimiento Almacenado:** CMXsrv_expcbe_bus_evz

#### Tablas Involucradas:
- EVZ
- CBE

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBE00601.FRM
**Segmento:** Reversar_Click
**Procedimiento Almacenado:** CMXsrv_expcbe_rev_cbe

#### Tablas Involucradas:
- EVL
- ACMXDESEMB
- COR
- ORG
- ACMXIMPUES
- ACMXPRMGRL
- EVZ
- CBE
- TRSD
- ACMXPRMEXP
- COM
- EVR
- CTZ
- DTN
- OPREC
- RET
- PUCBCX10

#### Procedimientos Llamados:
- por
- CMXsrv_mbyte_gen
- CMXsrv_cnt_rev_vig
- CMXsrv_expcbe_rev_trp
- CMXsrv_ctl_chq_aprcbl
- CMXsrv_rev_950
- CMXsrv_cnt_610
- sp_procxmode
- CMXsrv_expcbe_grb_evz
- CMXsrv_cnt_631
- CMXsrv_cnt_601
- CMXsrv_cnt_621
- CMXsrv_lee_fpro

---

### Archivo: CBE00602.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_expcbe_lee_evz

#### Tablas Involucradas:
- ACMXDESEMB
- COR
- ACMXPGOCBE
- EVZ
- CBE
- ACMXMONEDA
- ACMXTIPEVE
- ACMXSUCSAL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBE00603.FRM
**Segmento:** Eliminar_Click
**Procedimiento Almacenado:** CMXsrv_expcbe_del_dcz

#### Tablas Involucradas:
- CBE02
- CBE
- DCZ

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBE00603.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_expcbe_bus_dcz

#### Tablas Involucradas:
- DCZ

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBE00604.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_expcbe_grb_dcz

#### Tablas Involucradas:
- CBE02
- CBE
- DCZ

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBE00604.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_expcbe_lee_dcz

#### Tablas Involucradas:
- DCZ

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBE00605.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_expcbe_lee_cbe

#### Tablas Involucradas:
- ACMXPAIS
- COR
- ACMXPGOCBE
- CBE01
- CBE
- ACMXMONEDA
- ACMXENTDOC
- ACMXSUCSAL
- ACMXPRTCBE
- CLN

#### Procedimientos Llamados:
- CMXsrv_cmx_busc_suc_usu
- CMXsrv_val_suc
- sp_procxmode
- CMXsrv_lee_fpro

---

### Archivo: CBE00605.FRM
**Segmento:** buscar_Click
**Procedimiento Almacenado:** CMXsrv_expcbe_bus_vto

#### Tablas Involucradas:
- CBE

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBE00605.FRM
**Segmento:** fld_aux_cod_exp_LostFocus
**Procedimiento Almacenado:** CMXsrv_expcbe_lee_cln

#### Tablas Involucradas:
- CLN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBE00605.FRM
**Segmento:** Proximas_Click
**Procedimiento Almacenado:** CMXsrv_expcbe_bus_vto

#### Tablas Involucradas:
- CBE

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBEAVIRE.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_avi_dat_cou

#### Tablas Involucradas:

#### Procedimientos Llamados:
- sp_procxmode
- CMXsrv_avigrl_crea_avitemp
- bcicomex

---

### Archivo: CBEAVIRE.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_expcbe_avs_rem1

#### Tablas Involucradas:
- COR
- ACMXPGOCBE
- ACMXPRTCBE
- CBE01
- CBE
- CBE02
- ACMXMONEDA
- CTZ
- ACMXENTDOC
- ACMXPAIS
- ACMXPAISES
- CLN

#### Procedimientos Llamados:
- sp_procxmode
- CMXsrv_trae_glo_fec
- CMXsrv_expcbe_val_cbe
- CMXsrv_util_fmt_txt

---

### Archivo: CBEAVIRE.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_expcbe_avs_rem3

#### Tablas Involucradas:
- COR
- CBE01
- CBE
- CTZ
- ACMXMONEDA
- ACMXPAISES
- CLN
- CCO

#### Procedimientos Llamados:
- CMXsrv_util_fmt_txt
- sp_procxmode

---

### Archivo: CBEAVIRE.FRM
**Segmento:** imprime_esp
**Procedimiento Almacenado:** CMXsrv_expcbe_avs_rem2

#### Tablas Involucradas:
- CBE02
- CBE
- DCZ

#### Procedimientos Llamados:
- sp_procxmode
- CMXsrv_expcbe_for_lin

---

### Archivo: CBEAVIRE.FRM
**Segmento:** imprime_esp
**Procedimiento Almacenado:** CMXsrv_expcbe_avs_rem4

#### Tablas Involucradas:
- ACMXREMFESPMSG
- ACMXREMFINGMSG

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBEAVIRE.FRM
**Segmento:** imprime_ing
**Procedimiento Almacenado:** CMXsrv_expcbe_avs_rem2

#### Tablas Involucradas:
- CBE02
- CBE
- DCZ

#### Procedimientos Llamados:
- sp_procxmode
- CMXsrv_expcbe_for_lin

---

### Archivo: CBEAVIRE.FRM
**Segmento:** imprime_ing
**Procedimiento Almacenado:** CMXsrv_expcbe_avs_rem4

#### Tablas Involucradas:
- ACMXREMFESPMSG
- ACMXREMFINGMSG

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COR00906.FRM
**Segmento:** buscar_Click
**Procedimiento Almacenado:** CMXsrv_busc_plz

#### Tablas Involucradas:
- ACMXPLAZAS
- comex..ACMXPLAZAS

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COR00906.FRM
**Segmento:** fld_cor_cod_plz_Lostfocus
**Procedimiento Almacenado:** CMXsrv_lee_plz

#### Tablas Involucradas:
- ACMXPLAZAS

#### Procedimientos Llamados:
- CMXsrv_mbyte_cmp
- sp_procxmode

---

### Archivo: COR00906.FRM
**Segmento:** proximos_Click
**Procedimiento Almacenado:** CMXsrv_busc_plz

#### Tablas Involucradas:
- ACMXPLAZAS
- comex..ACMXPLAZAS

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COR00907.FRM
**Segmento:** buscar_Click
**Procedimiento Almacenado:** CMXsrv_cor_busc_pais

#### Tablas Involucradas:
- ACMXPAIS

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COR00907.FRM
**Segmento:** fld_cor_cod_pais_LostFocus
**Procedimiento Almacenado:** CMXsrv_cor_lee_pais

#### Tablas Involucradas:
- comex..ACMXPAIS

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COR00907.FRM
**Segmento:** proximos_Click
**Procedimiento Almacenado:** CMXsrv_cor_busc_pais

#### Tablas Involucradas:
- ACMXPAIS

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00602.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_expcbe_lee_cor

#### Tablas Involucradas:
- ACMXPAIS
- COR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00602.FRM
**Segmento:** buscar_Click
**Procedimiento Almacenado:** CMXsrv_expcbe_bus_cor

#### Tablas Involucradas:
- COR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00602.FRM
**Segmento:** fld_aux_cod_pai_LostFocus
**Procedimiento Almacenado:** CMXsrv_cor_lee_pais

#### Tablas Involucradas:
- comex..ACMXPAIS

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00602.FRM
**Segmento:** fld_aux_cod_plz_LostFocus
**Procedimiento Almacenado:** CMXsrv_lee_plz

#### Tablas Involucradas:
- ACMXPLAZAS

#### Procedimientos Llamados:
- CMXsrv_mbyte_cmp
- sp_procxmode

---

### Archivo: CRD00602.FRM
**Segmento:** proximos_Click
**Procedimiento Almacenado:** CMXsrv_expcbe_bus_cor

#### Tablas Involucradas:
- COR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: GRID_BUS.FRM
**Segmento:** buscar_Click
**Procedimiento Almacenado:** CMXsrv_busc_bco_mtr

#### Tablas Involucradas:
- ACMXBANCOS

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: GRID_BUS.FRM
**Segmento:** proximos_Click
**Procedimiento Almacenado:** CMXsrv_busc_bco_mtr

#### Tablas Involucradas:
- ACMXBANCOS

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: GRL00101.FRM
**Segmento:** enviar_Click
**Procedimiento Almacenado:** CMXsrv_expcbe_swf_sel

#### Tablas Involucradas:
- switxt
- switxt1

#### Procedimientos Llamados:
- CMXsrv_expcbe_swf_422
- CMXsrv_expcbe_swf_420
- CMXsrv_expcbe_swf_499
- CMXsrv_expcbe_swf_430
- sp_procxmode

---

### Archivo: GRLPAIS0.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_expcbe_lee_cor

#### Tablas Involucradas:
- ACMXPAIS
- COR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: GRLPAIS0.FRM
**Segmento:** buscar_Click
**Procedimiento Almacenado:** CMXsrv_expcbe_bus_cor

#### Tablas Involucradas:
- COR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: GRLPAIS0.FRM
**Segmento:** proximos_Click
**Procedimiento Almacenado:** CMXsrv_expcbe_bus_cor

#### Tablas Involucradas:
- COR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: PREFER.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_grl_fec_serv

#### Tablas Involucradas:

#### Procedimientos Llamados:
- SRV_MessageService
- sp_procxmode

---

## EXPCCE
<a name="expcce"></a>
### Archivo: CCE00101.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_cmx_busc_suc_usu

#### Tablas Involucradas:
- master..sysprocesses
- tbl_User

#### Procedimientos Llamados:
- PrmACMXSUCSAL
- CMXsrv_cmx_ing_lib
- sp_procxmode

---

### Archivo: CCE00101.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_expcce_lee_cce

#### Tablas Involucradas:
- ACMXPAIS
- COR
- tbl_User
- CCE
- ACMXSUCSAL
- CLN

#### Procedimientos Llamados:
- por
- sp_procxmode

---

### Archivo: CCE00101.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_expcce_trd_cce

#### Tablas Involucradas:
- ACMXFORPAG
- ACMXVIATPT
- ACMXMAXCCE
- ACMXCNFCCE
- ACMXMONEDA
- ACMXCLACOM
- CCE
- ACMXRCBCCE

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00101.FRM
**Segmento:** MCCEANL_CLICK
**Procedimiento Almacenado:** CMXsrv_expcce_anl_cce

#### Tablas Involucradas:
- CCE

#### Procedimientos Llamados:
- CMXsrv_cmx_lee_trs
- sp_procxmode
- CMXsrv_expcce_grb_evc
- CMXsrv_expcce_ictb_anu
- CMXsrv_cnt_950
- CMXsrv_cnt_740
- CMXsrv_expcce_lee_fpro

---

### Archivo: CCE00101.FRM
**Segmento:** Mccectb_click
**Procedimiento Almacenado:** CMXsrv_expcce_ctb_ing

#### Tablas Involucradas:
- CCE

#### Procedimientos Llamados:
- CMXsrv_mbyte_gen
- sp_procxmode
- CMXsrv_expcce_val_cce
- CMXsrv_expcce_grb_evc
- CMXsrv_cnt_950
- CMXsrv_cnt_700

---

### Archivo: CCE00101.FRM
**Segmento:** Mccedel_Click
**Procedimiento Almacenado:** CMXsrv_expcce_del_cce

#### Tablas Involucradas:
- COD
- ACCECTP
- ACCECND
- CCB
- COM
- ACCEBCO
- DCC
- CCE
- EVC
- ACCEDCC
- AFIN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00101.FRM
**Segmento:** MCCEVAL_CLICK
**Procedimiento Almacenado:** CMXsrv_expcce_val_cce

#### Tablas Involucradas:
- ACMXPAIS
- COR
- ACMXPRMGRL
- CCE_ADI
- DCC
- tbl_User
- CCE
- warnmsg
- ACMXSUCSAL
- COL

#### Procedimientos Llamados:
- CMXsrv_cmx_get_codes
- sp_procxmode

---

### Archivo: CCE00101.FRM
**Segmento:** Mmt730_Click
**Procedimiento Almacenado:** CMXsrv_expcce_swf_sel

#### Tablas Involucradas:
- switxt
- switxt1

#### Procedimientos Llamados:
- CMXsrv_expcce_swf_730
- CMXsrv_expcce_swf_742
- sp_procxmode

---

### Archivo: CCE00101.FRM
**Segmento:** Mmt730Ing_Click
**Procedimiento Almacenado:** CMXsrv_expcce_swf_sel

#### Tablas Involucradas:
- switxt
- switxt1

#### Procedimientos Llamados:
- CMXsrv_expcce_swf_730
- CMXsrv_expcce_swf_742
- sp_procxmode

---

### Archivo: CCE00201.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_expcce_grb_bco

#### Tablas Involucradas:
- CCB
- ACCEBCO
- ACCECRSE
- CRSE
- CCE

#### Procedimientos Llamados:
- sp_procxmode
- CMXsrv_expcce_lee_fpro

---

### Archivo: CCE00201.FRM
**Segmento:** fld_cce_bco_avs_LostFocus
**Procedimiento Almacenado:** CMXsrv_expcce_lee_cor

#### Tablas Involucradas:
- ACMXPAIS
- COR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00201.FRM
**Segmento:** fld_cce_bco_orig_LostFocus
**Procedimiento Almacenado:** CMXsrv_expcce_lee_cor

#### Tablas Involucradas:
- ACMXPAIS
- COR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00201.FRM
**Segmento:** fld_cce_cod_ems_LostFocus
**Procedimiento Almacenado:** CMXsrv_expcce_lee_cor

#### Tablas Involucradas:
- ACMXPAIS
- COR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00201.FRM
**Segmento:** fld_cce_cod_rmb_LostFocus
**Procedimiento Almacenado:** CMXsrv_expcce_lee_cor

#### Tablas Involucradas:
- ACMXPAIS
- COR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00201.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_expcce_lee_bco

#### Tablas Involucradas:
- COR
- CCB
- ACMXSUCSAL
- ACCEBCO
- CRSE
- CCE
- ACMXPAIS

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00202.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_expcce_grb_ctp

#### Tablas Involucradas:
- ACCECTP
- CCE

#### Procedimientos Llamados:
- sp_procxmode
- CMXsrv_expcce_lee_fpro

---

### Archivo: CCE00202.FRM
**Segmento:** fld_cce_cod_bn1_LostFocus
**Procedimiento Almacenado:** CMXsrv_expcce_lee_cln

#### Tablas Involucradas:
- CLN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00202.FRM
**Segmento:** fld_cce_cod_bn2_LostFocus
**Procedimiento Almacenado:** CMXsrv_expcce_lee_cln

#### Tablas Involucradas:
- CLN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00202.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_expcce_lee_ctp

#### Tablas Involucradas:
- ACCECTP
- ACMXPAIS
- CLN
- CCE

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00203.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_expcce_cre_cce

#### Tablas Involucradas:
- CCE

#### Procedimientos Llamados:
- CMXsrv_util_num_ope
- CMXsrv_cmx_busc_suc_usu
- sp_procxmode
- CMXsrv_expcce_lee_fpro

---

### Archivo: CCE00203.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_expcce_grb_bco

#### Tablas Involucradas:
- CCB
- ACCEBCO
- ACCECRSE
- CRSE
- CCE

#### Procedimientos Llamados:
- sp_procxmode
- CMXsrv_expcce_lee_fpro

---

### Archivo: CCE00203.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_expcce_grb_ctp

#### Tablas Involucradas:
- ACCECTP
- CCE

#### Procedimientos Llamados:
- sp_procxmode
- CMXsrv_expcce_lee_fpro

---

### Archivo: CCE00203.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_expcce_gen_dcc

#### Tablas Involucradas:
- ACMXPAIS
- DCC
- CCE

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00203.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_expcce_grb_cnd

#### Tablas Involucradas:
- CCE_ADI
- ACCECRSE
- CRSE
- CCE
- ACCE_ADI
- ACCECND

#### Procedimientos Llamados:
- sp_procxmode
- CMXsrv_expcce_lee_fpro

---

### Archivo: CCE00203.FRM
**Segmento:** fld_cce_fec_vto_LostFocus
**Procedimiento Almacenado:** CMXsrv_util_det_habil

#### Tablas Involucradas:
- ACMXFERIADO

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00203.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_expcce_lee_cnd

#### Tablas Involucradas:
- CCE_ADI
- ACCECRSE
- CRSE
- CCE
- ACCE_ADI
- ACCECND

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00203.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_expcce_trd_cnd

#### Tablas Involucradas:
- ACMXFORPAG
- ACMXVIATPT
- ACMXMAXCCE
- ACMXCNFCCE
- ACMXMONEDA
- CCE
- ACMXCLACOM
- ACMXFDESDE
- ACMXRCBCCE
- ACCECND

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00204.FRM
**Segmento:** ELIMINAR_Click
**Procedimiento Almacenado:** CMXsrv_expcce_del_dcc

#### Tablas Involucradas:
- DCC
- CCE
- ACCEDCC

#### Procedimientos Llamados:
- sp_procxmode
- CMXsrv_expcce_lee_fpro

---

### Archivo: CCE00204.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_expcce_bus_dcc

#### Tablas Involucradas:
- DCC
- CCE
- ACCEDCC

#### Procedimientos Llamados:
- CMXsrv_expcce_gen_adcc
- sp_procxmode

---

### Archivo: CCE00205.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_expcce_grb_dcc

#### Tablas Involucradas:
- DCC
- CCE
- ACCEDCC

#### Procedimientos Llamados:
- sp_procxmode
- CMXsrv_expcce_lee_fpro

---

### Archivo: CCE00205.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_expcce_lee_dcc

#### Tablas Involucradas:
- DCC
- CCE
- ACCEDCC

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00301.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_expcce_lee_cce

#### Tablas Involucradas:
- ACMXPAIS
- COR
- tbl_User
- CCE
- ACMXSUCSAL
- CLN

#### Procedimientos Llamados:
- por
- sp_procxmode

---

### Archivo: CCE00301.FRM
**Segmento:** buscar_Click
**Procedimiento Almacenado:** CMXsrv_expcce_bus_cce

#### Tablas Involucradas:
- CCE

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00301.FRM
**Segmento:** fld_aux_cod_bn1_lostfocus
**Procedimiento Almacenado:** CMXsrv_expcce_lee_cln

#### Tablas Involucradas:
- CLN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00301.FRM
**Segmento:** proximo_Click
**Procedimiento Almacenado:** CMXsrv_expcce_bus_cce

#### Tablas Involucradas:
- CCE

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00401.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_expcce_mdf_cce

#### Tablas Involucradas:
- COR
- ACCECTP
- ACCEBCO
- CCE_ADI
- ACCECRSE
- DAC
- DCC
- CRSE
- CCE
- ACCE_ADI
- NGE
- COL
- ACCEDCC
- ACCECND

#### Procedimientos Llamados:
- CMXsrv_expcce_can_mdf
- CMXsrv_expcce_get_tip_ope
- sp_procxmode
- CMXsrv_expcce_grb_evc
- CMXsrv_cnt_950
- CMXsrv_cmx_get_codes
- CMXsrv_expcce_ctb_mdfcce
- CMXsrv_expcce_lee_fpro
- CMXsrv_cnt_720

---

### Archivo: CCE00401.FRM
**Segmento:** Cancelar_Click
**Procedimiento Almacenado:** CMXsrv_expcce_can_mdf

#### Tablas Involucradas:
- ACCECTP
- ACCEBCO
- ACCEDCC
- ACCECND

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00401.FRM
**Segmento:** fld_cce_cod_bn1_LostFocus
**Procedimiento Almacenado:** CMXsrv_expcce_lee_cln

#### Tablas Involucradas:
- CLN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00401.FRM
**Segmento:** fld_cce_cod_ems_LostFocus
**Procedimiento Almacenado:** CMXsrv_expcce_lee_cor

#### Tablas Involucradas:
- ACMXPAIS
- COR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00401.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_expcce_lee_mdf

#### Tablas Involucradas:
- ACMXSUCSAL
- COR
- CCE
- CLN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00501.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_expcce_cnf_cce

#### Tablas Involucradas:
- COR
- CCE
- CLN

#### Procedimientos Llamados:
- CMXsrv_cnt_710
- sp_procxmode
- CMXsrv_expcce_ictb_cexp
- CMXsrv_expcce_grb_evc
- CMXsrv_cnt_950
- CMXsrv_expcce_lee_fpro

---

### Archivo: CCE00501.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_expcce_grb_afin

#### Tablas Involucradas:
- AFIN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00501.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_expcce_lee_cnf

#### Tablas Involucradas:
- ACMXFORPAG
- COR
- ACMXMONEDA
- CCE
- CLN

#### Procedimientos Llamados:
- sp_procxmode
- CMXsrv_expcce_lee_fpro

---

### Archivo: CCE00501.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_expcce_lee_afin

#### Tablas Involucradas:
- CCE
- AFIN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00701.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_expcce_trp_cce

#### Tablas Involucradas:
- COR
- CCE

#### Procedimientos Llamados:
- sp_procxmode
- CMXsrv_cnt_730
- CMXsrv_expcce_grb_evc
- CMXsrv_cnt_950

---

### Archivo: CCE00701.FRM
**Segmento:** fld_cce_bco_dst_LostFocus
**Procedimiento Almacenado:** CMXsrv_expcce_lee_cor

#### Tablas Involucradas:
- ACMXPAIS
- COR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00701.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_expcce_lee_trp

#### Tablas Involucradas:
- CCE

#### Procedimientos Llamados:
- sp_procxmode
- CMXsrv_expcce_lee_fpro

---

### Archivo: CCE00801.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_expcce_bus_evc

#### Tablas Involucradas:
- EVC
- CCE
- NGE

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00801.FRM
**Segmento:** proximo_Click
**Procedimiento Almacenado:** CMXsrv_expcce_bus_evc

#### Tablas Involucradas:
- EVC
- CCE
- NGE

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00801.FRM
**Segmento:** reversar_Click
**Procedimiento Almacenado:** CMXsrv_expcce_rev_cce

#### Tablas Involucradas:
- COR
- TAS
- ACMXIMPUES
- LTR
- DCN
- EVC
- RET
- CUO
- EVO
- TRSD
- DSN
- CCE
- NGE
- PUCBCX10
- COD
- CNO
- COM
- DAC
- EVE
- CAN
- COL
- AFIN
- ORG
- DTN
- EVR

#### Procedimientos Llamados:
- CMXsrv_expcce_rev_mdf
- CMXsrv_expcce_ctb_alz
- CMXsrv_expcce_rctb_anu
- CMXsrv_cnt_751
- CMXsrv_cnt_761
- CMXsrv_expcce_rctb_oto
- CMXsrv_cnt_1771
- CMXsrv_cnt_720
- CMXsrv_expcce_ranu_neg
- CMXsrv_mbyte_gen
- CMXsrv_expcce_chk_dsn
- CMXsrv_ctl_chq_aprcbl
- CMXsrv_rev_950
- CMXsrv_cnt_771
- CMXsrv_expcce_eli_col
- CMXsrv_expcce_grb_evc
- CMXsrv_cnt_731
- CMXsrv_expcce_get_tip_ope
- CMXsrv_expcce_rctb_oto_exp
- CMXsrv_cnt_711
- CMXsrv_cnt_rev_vig
- CMXsrv_cnt_701
- CMXsrv_cmx_lee_trs
- CMXsrv_cnt_999999
- CMXsrv_expcce_lee_fpro
- CMXsrv_cnt_741
- CMXsrv_expcce_eli_obl
- CMXsrv_expneg_rev_trp
- sp_procxmode
- CMXsrv_cnt_781
- CMXsrv_expcce_ctb_mdfcce
- CMXsrv_expcce_gen_dsn
- CMXsrv_expcce_rctb_pag_exp

---

### Archivo: CCE00802.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_expcce_lee_evc

#### Tablas Involucradas:
- ACMXFORPAG
- ACMXMONEDA
- CCE
- NGE
- EVC
- ACMXSUCSAL
- ACMXTIPEVE

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCEAVIRE.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_expcce_avs_rem1

#### Tablas Involucradas:
- ACMXFORPAG
- COR
- CCB
- NGEB
- ACMXMONEDA
- LTR
- CCE
- DCN
- NGE
- ACMXPAISES
- CLN

#### Procedimientos Llamados:
- CMXsrv_trae_glo_fec
- sp_procxmode

---

### Archivo: COR00906.FRM
**Segmento:** buscar_Click
**Procedimiento Almacenado:** CMXsrv_busc_plz

#### Tablas Involucradas:
- ACMXPLAZAS
- comex..ACMXPLAZAS

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COR00906.FRM
**Segmento:** fld_cor_cod_plz_Lostfocus
**Procedimiento Almacenado:** CMXsrv_lee_plz

#### Tablas Involucradas:
- ACMXPLAZAS

#### Procedimientos Llamados:
- CMXsrv_mbyte_cmp
- sp_procxmode

---

### Archivo: COR00906.FRM
**Segmento:** proximos_Click
**Procedimiento Almacenado:** CMXsrv_busc_plz

#### Tablas Involucradas:
- ACMXPLAZAS
- comex..ACMXPLAZAS

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COR00907.FRM
**Segmento:** buscar_Click
**Procedimiento Almacenado:** CMXsrv_cor_busc_pais

#### Tablas Involucradas:
- ACMXPAIS

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COR00907.FRM
**Segmento:** fld_cor_cod_pais_LostFocus
**Procedimiento Almacenado:** CMXsrv_cor_lee_pais

#### Tablas Involucradas:
- comex..ACMXPAIS

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COR00907.FRM
**Segmento:** proximos_Click
**Procedimiento Almacenado:** CMXsrv_cor_busc_pais

#### Tablas Involucradas:
- ACMXPAIS

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00602.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_expcce_lee_cor

#### Tablas Involucradas:
- ACMXPAIS
- COR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00602.FRM
**Segmento:** buscar_Click
**Procedimiento Almacenado:** CMXsrv_expcce_bus_cor

#### Tablas Involucradas:
- COR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00602.FRM
**Segmento:** Command1_Click
**Procedimiento Almacenado:** CMXsrv_expcce_bus_cor

#### Tablas Involucradas:
- COR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00602.FRM
**Segmento:** proximos_Click
**Procedimiento Almacenado:** CMXsrv_expcce_bus_cor

#### Tablas Involucradas:
- COR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: GRL00101.FRM
**Segmento:** enviar_Click
**Procedimiento Almacenado:** CMXsrv_expcce_swf_sel

#### Tablas Involucradas:
- switxt
- switxt1

#### Procedimientos Llamados:
- CMXsrv_expcce_swf_730
- CMXsrv_expcce_swf_742
- sp_procxmode

---

### Archivo: PREFER.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_grl_fec_serv

#### Tablas Involucradas:

#### Procedimientos Llamados:
- SRV_MessageService
- sp_procxmode

---

## expdex
<a name="expdex"></a>
### Archivo: DEX00101.FRM
**Segmento:** form_activate
**Procedimiento Almacenado:** CMXsrv_expcbe_lee_prm

#### Tablas Involucradas:
- ACMXPRMGRL

#### Procedimientos Llamados:
- sp_procxmode
- CMXsrv_lee_fpro

---

### Archivo: DEX00101.FRM
**Segmento:** form_activate
**Procedimiento Almacenado:** CMXsrv_dex_lee_dex

#### Tablas Involucradas:
- ACMXSUCSAL
- DEX
- CLN
- ACMXADUANA

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: DEX00101.FRM
**Segmento:** Mdexeli_Click
**Procedimiento Almacenado:** CMXsrv_dex_eli_dex

#### Tablas Involucradas:
- DEX

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: DEX00102.FRM
**Segmento:** ACEPTAR_Click
**Procedimiento Almacenado:** CMXsrv_dex_act_dex

#### Tablas Involucradas:
- DEX

#### Procedimientos Llamados:
- CMXsrv_exppln_get_dig
- sp_procxmode
- CMXsrv_lee_fpro

---

### Archivo: DEX00102.FRM
**Segmento:** fld_dex_dia_plz_max_LostFocus
**Procedimiento Almacenado:** CMXsrv_expdex_cal_fec

#### Tablas Involucradas:

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: DEX00102.FRM
**Segmento:** fld_dex_fec_acep_LostFocus
**Procedimiento Almacenado:** CMXsrv_expdex_cal_fec

#### Tablas Involucradas:

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: DEX00102.FRM
**Segmento:** fld_dex_rut_exp_LostFocus
**Procedimiento Almacenado:** CMXsrv_dex_lee_cli

#### Tablas Involucradas:
- CLN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: DEX00102.FRM
**Segmento:** FORM_Load
**Procedimiento Almacenado:** CMXsrv_dex_lee_dex

#### Tablas Involucradas:
- ACMXSUCSAL
- DEX
- CLN
- ACMXADUANA

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: DEX00103.FRM
**Segmento:** Buscar_Click
**Procedimiento Almacenado:** CMXsrv_dex_bus_dex

#### Tablas Involucradas:
- DEX

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: DEX00103.FRM
**Segmento:** fld_dex_rut_exp_LostFocus
**Procedimiento Almacenado:** CMXsrv_dex_lee_cli

#### Tablas Involucradas:
- CLN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: PREFER.FRM
**Segmento:** FORM_Load
**Procedimiento Almacenado:** CMXsrv_grl_fec_serv

#### Tablas Involucradas:

#### Procedimientos Llamados:
- SRV_MessageService
- sp_procxmode

---

### Archivo: RESPALD2.FRM
**Segmento:** ACEPTAR_Click
**Procedimiento Almacenado:** CMXsrv_dex_act_dex

#### Tablas Involucradas:
- DEX

#### Procedimientos Llamados:
- CMXsrv_exppln_get_dig
- sp_procxmode
- CMXsrv_lee_fpro

---

### Archivo: RESPALD2.FRM
**Segmento:** fld_dex_rut_exp_LostFocus
**Procedimiento Almacenado:** CMXsrv_dex_lee_cli

#### Tablas Involucradas:
- CLN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: RESPALD2.FRM
**Segmento:** FORM_Load
**Procedimiento Almacenado:** CMXsrv_dex_lee_dex

#### Tablas Involucradas:
- ACMXSUCSAL
- DEX
- CLN
- ACMXADUANA

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: RESPALDO.FRM
**Segmento:** COMELIMINAR_Click
**Procedimiento Almacenado:** CMXsrv_dex_eli_dex

#### Tablas Involucradas:
- DEX

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: RESPALDO.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_dex_lee_dex

#### Tablas Involucradas:
- ACMXSUCSAL
- DEX
- CLN
- ACMXADUANA

#### Procedimientos Llamados:
- sp_procxmode

---

## EXPNEG
<a name="expneg"></a>
### Archivo: CBE00601.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_expcbe_bus_evz

#### Tablas Involucradas:
- EVZ
- CBE

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBE00601.FRM
**Segmento:** Proximo_Click
**Procedimiento Almacenado:** CMXsrv_expcbe_bus_evz

#### Tablas Involucradas:
- EVZ
- CBE

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBE00601.FRM
**Segmento:** Reversar_Click
**Procedimiento Almacenado:** CMXsrv_expcbe_rev_cbe

#### Tablas Involucradas:
- EVL
- ACMXDESEMB
- COR
- ORG
- ACMXIMPUES
- ACMXPRMGRL
- EVZ
- CBE
- TRSD
- ACMXPRMEXP
- COM
- EVR
- CTZ
- DTN
- OPREC
- RET
- PUCBCX10

#### Procedimientos Llamados:
- por
- CMXsrv_mbyte_gen
- CMXsrv_cnt_rev_vig
- CMXsrv_expcbe_rev_trp
- CMXsrv_ctl_chq_aprcbl
- CMXsrv_rev_950
- CMXsrv_cnt_610
- sp_procxmode
- CMXsrv_expcbe_grb_evz
- CMXsrv_cnt_631
- CMXsrv_cnt_601
- CMXsrv_cnt_621
- CMXsrv_lee_fpro

---

### Archivo: CBE00602.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_expcbe_lee_evz

#### Tablas Involucradas:
- ACMXDESEMB
- COR
- ACMXPGOCBE
- EVZ
- CBE
- ACMXMONEDA
- ACMXTIPEVE
- ACMXSUCSAL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00601.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_expcce_lee_bas

#### Tablas Involucradas:
- ACMXMONEDA
- CCE
- ACMXFORPAG

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00601.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_expcce_lee_neg

#### Tablas Involucradas:
- COR
- ACMXVIATPT
- ACMXSUCSAL
- ACMXDISNEG
- ACMXMONEDA
- ACMXCLACOM
- NGE
- ACMXPAIS
- CLN
- ACMXTPONEG

#### Procedimientos Llamados:
- CMXsrv_cmx_busc_suc_usu
- sp_procxmode

---

### Archivo: CCE00601.FRM
**Segmento:** Mccealznge_click
**Procedimiento Almacenado:** CMXsrv_expcce_alz_dis

#### Tablas Involucradas:
- COL
- CCE
- NGE

#### Procedimientos Llamados:
- CMXsrv_expcce_ctb_alz
- CMXsrv_cnt_760
- sp_procxmode
- CMXsrv_expcce_grb_evc
- CMXsrv_cnt_950
- CMXsrv_expcce_get_tip_ope
- CMXsrv_expcce_lee_fpro

---

### Archivo: CCE00601.FRM
**Segmento:** Mcceanlnge_click
**Procedimiento Almacenado:** CMXsrv_expcce_anl_neg

#### Tablas Involucradas:
- CCE
- NGE

#### Procedimientos Llamados:
- CMXsrv_cmx_lee_trs
- sp_procxmode
- CMXsrv_cnt_780
- CMXsrv_expcce_grb_evc
- CMXsrv_expcce_ictb_anu
- CMXsrv_cnt_950
- CMXsrv_expcce_lee_fpro

---

### Archivo: CCE00601.FRM
**Segmento:** Mccectbnge_Click
**Procedimiento Almacenado:** CMXsrv_expcce_ctb_neg

#### Tablas Involucradas:
- COR
- LTR
- CCE
- NGE
- AFIN

#### Procedimientos Llamados:
- CMXsrv_expcce_val_neg
- CMXsrv_mbyte_gen
- CMXsrv_expcce_ineg_cexp
- sp_procxmode
- CMXsrv_expcce_anu_cexp
- CMXsrv_expcce_grb_evc
- CMXsrv_cnt_950
- CMXsrv_expcce_lee_fpro
- CMXsrv_cnt_750

---

### Archivo: CCE00601.FRM
**Segmento:** Mccedelnge_Click
**Procedimiento Almacenado:** CMXsrv_expcce_del_neg

#### Tablas Involucradas:
- CRSN
- COD
- COM
- NGEB
- LTR
- DSN
- CCE
- DCN
- NGE
- EVC
- AFIN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00601.FRM
**Segmento:** Mccevalnge_click
**Procedimiento Almacenado:** CMXsrv_expcce_val_neg

#### Tablas Involucradas:
- NGEB
- LTR
- DCC
- warnmsg
- CCE
- DCN
- NGE
- COL
- AFIN

#### Procedimientos Llamados:
- CMXsrv_util_fecha
- sp_procxmode

---

### Archivo: CCE00601.FRM
**Segmento:** Mtel742_Click
**Procedimiento Almacenado:** CMXsrv_expcce_swf_sel

#### Tablas Involucradas:
- switxt
- switxt1

#### Procedimientos Llamados:
- CMXsrv_expcce_swf_730
- CMXsrv_expcce_swf_742
- sp_procxmode

---

### Archivo: CCE00801.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_expcce_bus_evc

#### Tablas Involucradas:
- EVC
- CCE
- NGE

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00801.FRM
**Segmento:** Proximo_Click
**Procedimiento Almacenado:** CMXsrv_expcce_bus_evc

#### Tablas Involucradas:
- EVC
- CCE
- NGE

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00801.FRM
**Segmento:** Reversar_Click
**Procedimiento Almacenado:** CMXsrv_expcce_rev_cce

#### Tablas Involucradas:
- COR
- TAS
- ACMXIMPUES
- LTR
- DCN
- EVC
- RET
- CUO
- EVO
- TRSD
- DSN
- CCE
- NGE
- PUCBCX10
- COD
- CNO
- COM
- DAC
- EVE
- CAN
- COL
- AFIN
- ORG
- DTN
- EVR

#### Procedimientos Llamados:
- CMXsrv_expcce_rev_mdf
- CMXsrv_expcce_ctb_alz
- CMXsrv_expcce_rctb_anu
- CMXsrv_cnt_751
- CMXsrv_cnt_761
- CMXsrv_expcce_rctb_oto
- CMXsrv_cnt_1771
- CMXsrv_cnt_720
- CMXsrv_expcce_ranu_neg
- CMXsrv_mbyte_gen
- CMXsrv_expcce_chk_dsn
- CMXsrv_ctl_chq_aprcbl
- CMXsrv_rev_950
- CMXsrv_cnt_771
- CMXsrv_expcce_eli_col
- CMXsrv_expcce_grb_evc
- CMXsrv_cnt_731
- CMXsrv_expcce_get_tip_ope
- CMXsrv_expcce_rctb_oto_exp
- CMXsrv_cnt_711
- CMXsrv_cnt_rev_vig
- CMXsrv_cnt_701
- CMXsrv_cmx_lee_trs
- CMXsrv_cnt_999999
- CMXsrv_expcce_lee_fpro
- CMXsrv_cnt_741
- CMXsrv_expcce_eli_obl
- CMXsrv_expneg_rev_trp
- sp_procxmode
- CMXsrv_cnt_781
- CMXsrv_expcce_ctb_mdfcce
- CMXsrv_expcce_gen_dsn
- CMXsrv_expcce_rctb_pag_exp

---

### Archivo: CCE00802.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_expcce_lee_evc

#### Tablas Involucradas:
- ACMXFORPAG
- ACMXMONEDA
- CCE
- NGE
- EVC
- ACMXSUCSAL
- ACMXTIPEVE

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00901.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_expcce_grb_neg

#### Tablas Involucradas:
- CRSN
- CCE
- NGEB
- NGE

#### Procedimientos Llamados:
- CMXsrv_cmx_busc_suc_usu
- sp_procxmode
- CMXsrv_expcce_lee_fpro

---

### Archivo: CCE00901.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_expcce_gen_dcn

#### Tablas Involucradas:
- DCC
- CCE
- DCN
- NGE

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00901.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_expcce_grb_afin

#### Tablas Involucradas:
- AFIN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00901.FRM
**Segmento:** fld_cce_cod_exp_nge_LostFocus
**Procedimiento Almacenado:** CMXsrv_expcce_lee_cln

#### Tablas Involucradas:
- CLN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00901.FRM
**Segmento:** fld_cce_cod_pag_nge_LostFocus
**Procedimiento Almacenado:** CMXsrv_expcce_lee_cor

#### Tablas Involucradas:
- ACMXPAIS
- COR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00901.FRM
**Segmento:** fld_cce_cod_rmb_nge_LostFocus
**Procedimiento Almacenado:** CMXsrv_expcce_lee_cor

#### Tablas Involucradas:
- ACMXPAIS
- COR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00901.FRM
**Segmento:** fld_cce_ins_rem1_nge_GotFocus
**Procedimiento Almacenado:** CMXsrv_expcce_avs_rem5

#### Tablas Involucradas:
- COR
- ACMXCRDREMTXT
- ACMXMONEDA
- CCE
- NGE
- ACMXPAISES
- CCO

#### Procedimientos Llamados:
- CMX_srv_pone_punto
- CMXsrv_util_fmt_txt
- sp_procxmode
- CMXsrv_expcce_get_ing_esp

---

### Archivo: CCE00901.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_expcce_lee_nge

#### Tablas Involucradas:
- COR
- CRSN
- NGEB
- CCE
- NGE
- ACMXPAIS
- CLN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00901.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_expcce_trd_nge

#### Tablas Involucradas:
- ACMXVIATPT
- ACMXRCBCCE
- ACMXMONEDA
- ACMXCLACOM
- NGE
- ACMXTPONEG

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00901.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_expcce_ini_neg

#### Tablas Involucradas:
- ACMXPAIS
- COR
- ACMXVIATPT
- CCB
- ACMXMONEDA
- CRSE
- CCE
- ACMXCLACOM
- NGE
- ACMXSUCSAL
- CLN
- ACMXTPONEG

#### Procedimientos Llamados:
- sp_procxmode
- CMXsrv_expcce_lee_fpro

---

### Archivo: CCE00901.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_expcce_lee_afin

#### Tablas Involucradas:
- CCE
- AFIN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00901.FRM
**Segmento:** lee_bco
**Procedimiento Almacenado:** CMXsrv_expcce_lee_cor

#### Tablas Involucradas:
- ACMXPAIS
- COR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00902.FRM
**Segmento:** ELIMINAR_Click
**Procedimiento Almacenado:** CMXsrv_expcce_del_dcn

#### Tablas Involucradas:
- CCE
- DCN
- NGE

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00902.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_expcce_bus_dcn

#### Tablas Involucradas:
- DCN
- NGE

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00903.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_expcce_grb_dcn

#### Tablas Involucradas:
- CCE
- DCN
- NGE

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00903.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_expcce_lee_dcn

#### Tablas Involucradas:
- DCC
- DCN
- NGE

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00904.FRM
**Segmento:** ELIMINAR_Click
**Procedimiento Almacenado:** CMXsrv_expcce_del_ltr

#### Tablas Involucradas:
- LTR
- CCE
- NGE

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00904.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_expcce_bus_ltr

#### Tablas Involucradas:
- LTR
- NGE

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00905.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_expcce_grb_ltr

#### Tablas Involucradas:
- LTR
- CCE
- NGE

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00905.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_expcce_lee_ltr

#### Tablas Involucradas:
- LTR
- CCE
- NGE

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00906.FRM
**Segmento:** ELIMINAR_Click
**Procedimiento Almacenado:** CMXsrv_expcce_del_dsn

#### Tablas Involucradas:
- DSN
- CCE
- NGE

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00906.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_expcce_gen_dsn

#### Tablas Involucradas:
- DCC
- DSN
- CCE
- DCN
- NGE

#### Procedimientos Llamados:
- CMXsrv_expcce_grb_dsn
- sp_procxmode

---

### Archivo: CCE00906.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_expcce_bus_dsn

#### Tablas Involucradas:
- DSN
- NGE

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00906.FRM
**Segmento:** Salir_Click
**Procedimiento Almacenado:** CMXsrv_expcce_chk_dsn

#### Tablas Involucradas:
- DSN
- CCE
- NGE

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE00907.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_expcce_grb_dsn

#### Tablas Involucradas:
- DSN
- CCE
- NGE

#### Procedimientos Llamados:
- sp_procxmode
- CMXsrv_expcce_chk_dsn

---

### Archivo: CCE00907.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_expcce_lee_dsn

#### Tablas Involucradas:
- DSN
- NGE

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE01001.FRM
**Segmento:** buscar_Click
**Procedimiento Almacenado:** CMXsrv_expcce_bus_neg

#### Tablas Involucradas:
- CCE
- NGE

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE01001.FRM
**Segmento:** Proximas_Click
**Procedimiento Almacenado:** CMXsrv_expcce_bus_neg

#### Tablas Involucradas:
- CCE
- NGE

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE01201.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_expcce_pgo_neg

#### Tablas Involucradas:
- ACMXDESEMB
- COR
- vig_cmx
- ACMXIMPUES
- COD
- ACMXPRMEXP
- COM
- CCE
- tbl_User
- NGE
- CLN
- RET

#### Procedimientos Llamados:
- CMXsrv_expret_grb_dtn
- CMXsrv_expcce_anu_cexp
- CMXsrv_cnt_1770
- CMXsrv_expret_grb_det
- CMXsrv_mbyte_gen
- CMXsrv_expret_grb_org
- CMXsrv_cnt_gen_vig
- CMXsrv_vig_gra_vig
- CMXsrv_expcce_grb_evc
- CMXsrv_cmx_get_codes
- CMXsrv_expret_cre_ret
- CMXsrv_cnt_770
- CMXsrv_cnt_999999
- CMXsrv_exp_ipuc_gen_pln
- CMXsrv_expcce_lee_fpro
- CMXsrv_expneg_trp_cyg
- sp_procxmode
- CMXsrv_expcce_pag_exp
- CMXsrv_cnt_950

---

### Archivo: CCE01201.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_expcce_grb_afin

#### Tablas Involucradas:
- AFIN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE01201.FRM
**Segmento:** fld_cce_cod_exp_nge_LostFocus
**Procedimiento Almacenado:** CMXsrv_expcce_lee_cln

#### Tablas Involucradas:
- CLN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE01201.FRM
**Segmento:** fld_cce_cod_rmb_nge_LostFocus
**Procedimiento Almacenado:** CMXsrv_expcce_lee_cor

#### Tablas Involucradas:
- ACMXPAIS
- COR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE01201.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_expcce_lee_pgo

#### Tablas Involucradas:
- ACMXDESEMB
- COR
- ACMXPRMEXP
- ACMXMONEDA
- CCE
- NGE
- CLN

#### Procedimientos Llamados:
- sp_procxmode
- CMXsrv_expcce_lee_fpro

---

### Archivo: CCE01201.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_expcce_lee_afin

#### Tablas Involucradas:
- CCE
- AFIN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCE01201.FRM
**Segmento:** lee_bco
**Procedimiento Almacenado:** CMXsrv_expcce_lee_cor

#### Tablas Involucradas:
- ACMXPAIS
- COR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCEAVIRE.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_avi_dat_cou

#### Tablas Involucradas:

#### Procedimientos Llamados:
- sp_procxmode
- CMXsrv_avigrl_crea_avitemp
- bcicomex

---

### Archivo: CCEAVIRE.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_expcce_lee_nge

#### Tablas Involucradas:
- COR
- CRSN
- NGEB
- CCE
- NGE
- ACMXPAIS
- CLN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCEAVIRE.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_expcce_avs_rem1

#### Tablas Involucradas:
- ACMXFORPAG
- COR
- CCB
- NGEB
- ACMXMONEDA
- LTR
- CCE
- DCN
- NGE
- ACMXPAISES
- CLN

#### Procedimientos Llamados:
- CMXsrv_trae_glo_fec
- sp_procxmode

---

### Archivo: CCEAVIRE.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_expcce_avs_rem3

#### Tablas Involucradas:
- LTR
- NGE

#### Procedimientos Llamados:
- CMXsrv_util_fmt_txt
- sp_procxmode

---

### Archivo: CCEAVIRE.FRM
**Segmento:** imprime_esp
**Procedimiento Almacenado:** CMXsrv_expcce_avs_rem2

#### Tablas Involucradas:
- DCN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCEAVIRE.FRM
**Segmento:** imprime_esp
**Procedimiento Almacenado:** CMXsrv_expcce_avs_rem4

#### Tablas Involucradas:
- DSN

#### Procedimientos Llamados:
- CMXsrv_util_fmt_txt
- sp_procxmode

---

### Archivo: CCEAVIRE.FRM
**Segmento:** imprime_esp
**Procedimiento Almacenado:** CMXsrv_expcbe_avs_rem4

#### Tablas Involucradas:
- ACMXREMFESPMSG
- ACMXREMFINGMSG

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCEAVIRE.FRM
**Segmento:** imprime_ing
**Procedimiento Almacenado:** CMXsrv_expcce_avs_rem2

#### Tablas Involucradas:
- DCN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CCEAVIRE.FRM
**Segmento:** imprime_ing
**Procedimiento Almacenado:** CMXsrv_expcce_avs_rem4

#### Tablas Involucradas:
- DSN

#### Procedimientos Llamados:
- CMXsrv_util_fmt_txt
- sp_procxmode

---

### Archivo: CCEAVIRE.FRM
**Segmento:** imprime_ing
**Procedimiento Almacenado:** CMXsrv_expcbe_avs_rem4

#### Tablas Involucradas:
- ACMXREMFESPMSG
- ACMXREMFINGMSG

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00602.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_expcce_lee_cor

#### Tablas Involucradas:
- ACMXPAIS
- COR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00602.FRM
**Segmento:** buscar_Click
**Procedimiento Almacenado:** CMXsrv_expcce_bus_cor

#### Tablas Involucradas:
- COR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00602.FRM
**Segmento:** proximos_Click
**Procedimiento Almacenado:** CMXsrv_expcce_bus_cor

#### Tablas Involucradas:
- COR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: GRL00101.FRM
**Segmento:** enviar_Click
**Procedimiento Almacenado:** CMXsrv_expcce_swf_sel

#### Tablas Involucradas:
- switxt
- switxt1

#### Procedimientos Llamados:
- CMXsrv_expcce_swf_730
- CMXsrv_expcce_swf_742
- sp_procxmode

---

### Archivo: PREFER.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_grl_fec_serv

#### Tablas Involucradas:

#### Procedimientos Llamados:
- SRV_MessageService
- sp_procxmode

---

## expret
<a name="expret"></a>
### Archivo: COR00906.FRM
**Segmento:** buscar_Click
**Procedimiento Almacenado:** CMXsrv_busc_plz

#### Tablas Involucradas:
- ACMXPLAZAS
- comex..ACMXPLAZAS

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COR00906.FRM
**Segmento:** fld_cor_cod_plz_Lostfocus
**Procedimiento Almacenado:** CMXsrv_lee_plz

#### Tablas Involucradas:
- ACMXPLAZAS

#### Procedimientos Llamados:
- CMXsrv_mbyte_cmp
- sp_procxmode

---

### Archivo: COR00906.FRM
**Segmento:** proximos_Click
**Procedimiento Almacenado:** CMXsrv_busc_plz

#### Tablas Involucradas:
- ACMXPLAZAS
- comex..ACMXPLAZAS

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COR00907.FRM
**Segmento:** buscar_Click
**Procedimiento Almacenado:** CMXsrv_cor_busc_pais

#### Tablas Involucradas:
- ACMXPAIS

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COR00907.FRM
**Segmento:** fld_cor_cod_pais_LostFocus
**Procedimiento Almacenado:** CMXsrv_cor_lee_pais

#### Tablas Involucradas:
- comex..ACMXPAIS

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COR00907.FRM
**Segmento:** proximos_Click
**Procedimiento Almacenado:** CMXsrv_cor_busc_pais

#### Tablas Involucradas:
- ACMXPAIS

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00602.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_expcbe_lee_cor

#### Tablas Involucradas:
- ACMXPAIS
- COR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00602.FRM
**Segmento:** buscar_Click
**Procedimiento Almacenado:** CMXsrv_expcbe_bus_cor

#### Tablas Involucradas:
- COR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00602.FRM
**Segmento:** proximos_Click
**Procedimiento Almacenado:** CMXsrv_expcbe_bus_cor

#### Tablas Involucradas:
- COR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: GRL00101.FRM
**Segmento:** Command2_Click
**Procedimiento Almacenado:** CMXsrv_expret_swf_sel

#### Tablas Involucradas:
- DTN
- ACMXPRMEXP
- switxt
- switxt1

#### Procedimientos Llamados:
- CMXsrv_expret_swf_202
- CMXsrv_expret_swf_100
- sp_procxmode

---

### Archivo: PREFER.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_grl_fec_serv

#### Tablas Involucradas:

#### Procedimientos Llamados:
- SRV_MessageService
- sp_procxmode

---

### Archivo: RET00101.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_cmx_busc_suc_usu

#### Tablas Involucradas:
- master..sysprocesses
- tbl_User

#### Procedimientos Llamados:
- PrmACMXSUCSAL
- CMXsrv_cmx_ing_lib
- sp_procxmode

---

### Archivo: RET00101.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_expret_lee_ret

#### Tablas Involucradas:
- DTN
- ACMXPRMEXP
- ACMXMONEDA
- ACMXSUCSAL
- CLN
- RET

#### Procedimientos Llamados:
- CMXsrv_cmx_busc_suc_usu
- sp_procxmode
- CMXsrv_lee_fpro

---

### Archivo: RET00101.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_expret_lee_prm

#### Tablas Involucradas:
- ACMXPRMGRL
- ACMXPRMEXP

#### Procedimientos Llamados:
- sp_procxmode
- CMXsrv_lee_fpro

---

### Archivo: RET00101.FRM
**Segmento:** M_cgyc_Click
**Procedimiento Almacenado:** CMXsrv_expret_avs_cyg1

#### Tablas Involucradas:
- ACMXDESEMB
- ASND
- ACMXIMPUES
- ACMXPRMGRL
- COM
- TRSD
- EVR
- CLN
- ACMXESPECI
- RET

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: RET00101.FRM
**Segmento:** M_cgyc_Click
**Procedimiento Almacenado:** CMXsrv_expret_avs_cyg2

#### Tablas Involucradas:
- ASND
- ACMXIMPUES
- ACMXPRMGRL
- EVR
- RET

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: RET00101.FRM
**Segmento:** mavisliq_Click
**Procedimiento Almacenado:** CMXsrv_expret_avs_liq1

#### Tablas Involucradas:
- DTN
- ACMXMONEDA
- ACMXSUCSAL
- CLN
- ACMXESPECI
- RET

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: RET00101.FRM
**Segmento:** mavisliq_Click
**Procedimiento Almacenado:** CMXsrv_expret_avs_liq2

#### Tablas Involucradas:
- ORG
- RET

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: RET00101.FRM
**Segmento:** mavisliq_Click
**Procedimiento Almacenado:** CMXsrv_expret_avs_liq3

#### Tablas Involucradas:
- DTN
- ACMXPRMEXP
- RET

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: RET00101.FRM
**Segmento:** Mcbectb_Click
**Procedimiento Almacenado:** CMXsrv_expret_val_ret

#### Tablas Involucradas:
- ACMXDESEMB
- ORG
- COR
- ACMXIMPUES
- ACMXPRMGRL
- CCL
- ACMXPRMEXP
- ACMXMONEDAFEC
- COM
- tbl_User
- warnmsg
- DTN
- CLN
- RET

#### Procedimientos Llamados:
- CMXsrv_val_cta_cte
- sp_procxmode
- CMXsrv_enl_val_sel
- CMXsrv_val_vig
- CMXsrv_util_len
- CMXsrv_lee_fpro

---

### Archivo: RET00101.FRM
**Segmento:** Mcbectb_Click
**Procedimiento Almacenado:** CMXsrv_expret_sum_dtn_mn

#### Tablas Involucradas:
- DTN
- ACMXMONEDAFEC
- RET
- ACMXPRMENL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: RET00101.FRM
**Segmento:** Mcbectb_Click
**Procedimiento Almacenado:** CMXsrv_expret_ctb_ing

#### Tablas Involucradas:
- ACMXDESEMB
- ASND
- PLV
- ACMXPRMGRL
- CCL
- ACMXPRMEXP
- PLI
- tbl_User
- DTN
- CLN
- RET

#### Procedimientos Llamados:
- CMXsrv_mbyte_gen
- CMXsrv_expret_grb_org
- CMXsrv_expret_grb_dtn
- CMXsrv_expret_cre_ret
- CMXsrv_vig_gra_vig
- CMXsrv_cnt_res_vig
- CMXsrv_enl_act_enl
- sp_cmx_sii_1862
- sp_procxmode
- CMXsrv_cnt_950
- sp_cmx_sii_1870
- CMXsrv_expret_val_ret
- CMXsrv_expret_grb_det
- CMXsrv_expret_cnt_cyg
- CMXsrv_cnt_800
- CMXsrv_expret_grb_evr
- CMXsrv_cnt_810

---

### Archivo: RET00101.FRM
**Segmento:** Mcbedel_Click
**Procedimiento Almacenado:** CMXsrv_expret_del_ret

#### Tablas Involucradas:
- ORG
- COD
- COM
- DTN
- RET

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: RET00101.FRM
**Segmento:** Mliqctb_Click
**Procedimiento Almacenado:** CMXsrv_expret_avs_adm1

#### Tablas Involucradas:
- ACMXSUCSAL
- ACMXMONEDA
- CLN
- RET

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: RET00101.FRM
**Segmento:** Mliqctb_Click
**Procedimiento Almacenado:** CMXsrv_expret_avs_adm2

#### Tablas Involucradas:
- ORG
- ACMXPRMEXP
- RET

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: RET00101.FRM
**Segmento:** Mliqctb_Click
**Procedimiento Almacenado:** CMXsrv_expret_avs_adm3

#### Tablas Involucradas:
- DTN
- ACMXPRMEXP
- RET

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: RET00101.FRM
**Segmento:** Mvalid_Click
**Procedimiento Almacenado:** CMXsrv_expret_val_ret

#### Tablas Involucradas:
- ACMXDESEMB
- ORG
- COR
- ACMXIMPUES
- ACMXPRMGRL
- CCL
- ACMXPRMEXP
- ACMXMONEDAFEC
- COM
- tbl_User
- warnmsg
- DTN
- CLN
- RET

#### Procedimientos Llamados:
- CMXsrv_val_cta_cte
- sp_procxmode
- CMXsrv_enl_val_sel
- CMXsrv_val_vig
- CMXsrv_util_len
- CMXsrv_lee_fpro

---

### Archivo: RET00102.FRM
**Segmento:** ACEPTAR_Click
**Procedimiento Almacenado:** CMXsrv_expret_act_tpo_cbo

#### Tablas Involucradas:
- RET

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: RET00102.FRM
**Segmento:** ACEPTAR_Click
**Procedimiento Almacenado:** CMXsrv_expret_val_ret

#### Tablas Involucradas:
- ACMXDESEMB
- ORG
- COR
- ACMXIMPUES
- ACMXPRMGRL
- CCL
- ACMXPRMEXP
- ACMXMONEDAFEC
- COM
- tbl_User
- warnmsg
- DTN
- CLN
- RET

#### Procedimientos Llamados:
- CMXsrv_val_cta_cte
- sp_procxmode
- CMXsrv_enl_val_sel
- CMXsrv_val_vig
- CMXsrv_util_len
- CMXsrv_lee_fpro

---

### Archivo: RET00201.FRM
**Segmento:** ACEPTAR_Click
**Procedimiento Almacenado:** CMXsrv_expret_cre_ret

#### Tablas Involucradas:
- RET

#### Procedimientos Llamados:
- CMXsrv_util_num_ope
- CMXsrv_cmx_busc_suc_usu
- sp_procxmode
- CMXsrv_lee_fpro

---

### Archivo: RET00201.FRM
**Segmento:** ACEPTAR_Click
**Procedimiento Almacenado:** CMXsrv_expret_grb_det

#### Tablas Involucradas:
- CLN
- tbl_User
- RET

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: RET00201.FRM
**Segmento:** fld_ret_mon_ret_LostFocus
**Procedimiento Almacenado:** CMXsrv_expret_tpo_cbo

#### Tablas Involucradas:
- ACMXMONEDAFEC

#### Procedimientos Llamados:
- sp_procxmode
- CMXsrv_lee_fpro

---

### Archivo: RET00201.FRM
**Segmento:** fld_ret_rut_cli_LostFocus
**Procedimiento Almacenado:** CMXsrv_expret_lee_cln

#### Tablas Involucradas:
- CLN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: RET00201.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_expret_lee_det

#### Tablas Involucradas:
- ACMXSUCSAL
- ACMXMONEDA
- CLN
- RET

#### Procedimientos Llamados:
- sp_procxmode
- CMXsrv_lee_fpro

---

### Archivo: RET00301.FRM
**Segmento:** ELIMINAR_Click
**Procedimiento Almacenado:** CMXsrv_expret_del_org

#### Tablas Involucradas:
- ORG
- RET

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: RET00301.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_expret_bus_org

#### Tablas Involucradas:
- ORG
- RET

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: RET00401.FRM
**Segmento:** ACEPTAR_Click
**Procedimiento Almacenado:** CMXsrv_expret_grb_org

#### Tablas Involucradas:
- ACMXDESEMB
- ORG
- ACMXPLNCTAN
- ACMXSRVEXT
- ACMXPLNCTAX
- RET

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: RET00401.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_expret_mto_org

#### Tablas Involucradas:
- ORG
- RET

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: RET00401.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_expret_lee_org

#### Tablas Involucradas:
- ACMXDESEMB
- ORG
- COR
- ACMXTPODOC
- ACMXPAIS

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: RET00401.FRM
**Segmento:** valida_vigente
**Procedimiento Almacenado:** CMXsrv_vig_lee_cta

#### Tablas Involucradas:
- ACMXPLNCTAN
- ACMXDESEMB
- ACMXPLNCTAX

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: RET00501.FRM
**Segmento:** ELIMINAR_Click
**Procedimiento Almacenado:** CMXsrv_expret_del_dtn

#### Tablas Involucradas:
- DTN
- RET

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: RET00501.FRM
**Segmento:** emitir_Click
**Procedimiento Almacenado:** CMXsrv_expret_swf_sel

#### Tablas Involucradas:
- DTN
- ACMXPRMEXP
- switxt
- switxt1

#### Procedimientos Llamados:
- CMXsrv_expret_swf_202
- CMXsrv_expret_swf_100
- sp_procxmode

---

### Archivo: RET00501.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_expret_bus_dtn

#### Tablas Involucradas:
- DTN
- RET

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: RET00601.FRM
**Segmento:** ACEPTAR_Click
**Procedimiento Almacenado:** CMXsrv_expret_grb_dtn

#### Tablas Involucradas:
- ACMXDESEMB
- ACMXPRMGRL
- CCL
- ACMXPRMEXP
- DTN
- RET

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: RET00601.FRM
**Segmento:** fld_ret_cod_ben_LostFocus
**Procedimiento Almacenado:** CMXsrv_expret_lee_cln

#### Tablas Involucradas:
- CLN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: RET00601.FRM
**Segmento:** fld_ret_mto_arb_LostFocus
**Procedimiento Almacenado:** CMXsrv_expret_cal_arb

#### Tablas Involucradas:
- ACMXPRMGRL
- ACMXMONEDA

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: RET00601.FRM
**Segmento:** fld_ret_mto_ben_LostFocus
**Procedimiento Almacenado:** CMXsrv_expret_cal_arb

#### Tablas Involucradas:
- ACMXPRMGRL
- ACMXMONEDA

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: RET00601.FRM
**Segmento:** fld_ret_par_ben_LostFocus
**Procedimiento Almacenado:** CMXsrv_expret_cal_arb

#### Tablas Involucradas:
- ACMXPRMGRL
- ACMXMONEDA

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: RET00601.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_expret_mto_dtn

#### Tablas Involucradas:
- DTN
- COM
- RET
- ACMXIMPUES

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: RET00601.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_expret_lee_dtn

#### Tablas Involucradas:
- ACMXPAIS
- ACMXDESEMB
- COR
- DTN
- ACMXMONEDA
- APUCCODOPECMB
- ACMXSUCSAL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: RET00601.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_expret_lee_cln

#### Tablas Involucradas:
- CLN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: RET00701.FRM
**Segmento:** buscar_Click
**Procedimiento Almacenado:** CMXsrv_expret_bus_ret

#### Tablas Involucradas:
- RET

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: RET00701.FRM
**Segmento:** fld_ret_rut_cli_LostFocus
**Procedimiento Almacenado:** CMXsrv_expret_lee_cln

#### Tablas Involucradas:
- CLN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: RET00701.FRM
**Segmento:** proxima_Click
**Procedimiento Almacenado:** CMXsrv_expret_bus_ret

#### Tablas Involucradas:
- RET

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: RET00801.FRM
**Segmento:** Command1_Click
**Procedimiento Almacenado:** CMXsrv_expret_bus_evr

#### Tablas Involucradas:
- EVR
- RET

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: RET00801.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_expret_bus_evr

#### Tablas Involucradas:
- EVR
- RET

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: RET00801.FRM
**Segmento:** proximo_Click
**Procedimiento Almacenado:** CMXsrv_expret_bus_evr

#### Tablas Involucradas:
- EVR
- RET

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: RET00801.FRM
**Segmento:** reversar_Click
**Procedimiento Almacenado:** CMXsrv_expret_rev_ret

#### Tablas Involucradas:
- ORG
- DTN
- PLV
- ACMXPRMEXP
- PLI
- TRSD
- EVR
- RET

#### Procedimientos Llamados:
- CMXsrv_cnt_rev_vig
- CMXsrv_cnt_811
- CMXsrv_mbyte_gen
- CMXsrv_ctl_chq_aprcbl
- CMXsrv_rev_950
- sp_cmx_sii_1862
- sp_procxmode
- CMXsrv_cnt_801
- sp_cmx_sii_1870
- CMXsrv_expret_rev_cyg
- CMXsrv_expret_grb_evr
- CMXsrv_enl_rev_enl

---

### Archivo: RET00802.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_expret_lee_evr

#### Tablas Involucradas:
- ACMXTIPEVE
- EVR
- ACMXSUCSAL

#### Procedimientos Llamados:
- sp_procxmode

---

## ADMIN
<a name="admin"></a>
### Archivo: ADM00201.FRM
**Segmento:** COMMAND4_Click
**Procedimiento Almacenado:** CMXsrv_finadm_imod_desti

#### Tablas Involucradas:
- TIP

#### Procedimientos Llamados:
- CMXsrv_finadm_val_tipop
- sp_procxmode

---

### Archivo: ADM00201.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_finadm_cons_dtip

#### Tablas Involucradas:
- TIP

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: ADM00202.FRM
**Segmento:** Command1_Click
**Procedimiento Almacenado:** CMXsrv_finadm_imod_ectb

#### Tablas Involucradas:
- TIP

#### Procedimientos Llamados:
- CMXsrv_finadm_val_tipop
- sp_procxmode

---

### Archivo: ADM00202.FRM
**Segmento:** Command2_Click
**Procedimiento Almacenado:** CMXsrv_finadm_eli_tipop

#### Tablas Involucradas:
- TIP
- TIP_CTA

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: ADM00202.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_finadm_cons_ectb

#### Tablas Involucradas:
- TIP

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: ADM00203.FRM
**Segmento:** COMMAND3_Click
**Procedimiento Almacenado:** CMXsrv_finadm_eli_tipop

#### Tablas Involucradas:
- TIP
- TIP_CTA

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: ADM00203.FRM
**Segmento:** COMMAND4_Click
**Procedimiento Almacenado:** CMXsrv_finadm_imod_itip

#### Tablas Involucradas:
- TIP

#### Procedimientos Llamados:
- CMXsrv_finadm_val_tipop
- sp_procxmode

---

### Archivo: ADM00203.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_finadm_cons_itip

#### Tablas Involucradas:
- TIP

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: ADM00204.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_finadm_lee_tipop

#### Tablas Involucradas:
- TIP
- ACMXPLAZO
- ACMXPROCMX
- ACMXMB1

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: ADM00204.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_grl_fec_serv

#### Tablas Involucradas:

#### Procedimientos Llamados:
- SRV_MessageService
- sp_procxmode

---

### Archivo: ADM00204.FRM
**Segmento:** Mdel_Click
**Procedimiento Almacenado:** CMXsrv_finadm_eli_tipop

#### Tablas Involucradas:
- TIP
- TIP_CTA

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: ADM00204.FRM
**Segmento:** Mval_Click
**Procedimiento Almacenado:** CMXsrv_finadm_val_tipop

#### Tablas Involucradas:
- APEPROR
- TIP
- TAS
- CUO
- ACMXPLNCTAN
- ACMXMONEDAFEC
- PANCTL
- ACLNCBCABCI
- ACMXPLNCTAX
- TIP_CTA
- ACMXMONEDA
- warnmsg
- EVE
- ACMXSUCSAL
- PANVTO
- ACMXINTEREFEC
- COL
- PANMOR

#### Procedimientos Llamados:
- CMXsrv_fincol_eval_tbat
- CMXsrv_util_fecha2
- SRV_MessageService
- sp_procxmode

---

### Archivo: ADM00205.FRM
**Segmento:** buscar_Click
**Procedimiento Almacenado:** CMXsrv_finadm_bus_tipope

#### Tablas Involucradas:
- TIP

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: ADM00205.FRM
**Segmento:** proximas_Click
**Procedimiento Almacenado:** CMXsrv_finadm_bus_tipope

#### Tablas Involucradas:
- TIP

#### Procedimientos Llamados:
- sp_procxmode

---

## COL_NEG
<a name="col_neg"></a>
### Archivo: COL00102.FRM
**Segmento:** CANCELAR_Click
**Procedimiento Almacenado:** CMXsrv_busc_tip_tas

#### Tablas Involucradas:
- CRD

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL00102.FRM
**Segmento:** ELIMINAR_Click
**Procedimiento Almacenado:** CMXsrv_fincol_ecuo

#### Tablas Involucradas:
- CUO_REN
- COL
- CUO

#### Procedimientos Llamados:
- CMXsrv_fincol_pre_cuad_tas
- sp_procxmode

---

### Archivo: COL00102.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_fincol_cons_plnpa

#### Tablas Involucradas:
- CUO_REN
- COL_REN
- COL
- CUO

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL00102.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_pertas_val_display

#### Tablas Involucradas:
- TAS

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL00103.FRM
**Segmento:** ELIMINAR_Click
**Procedimiento Almacenado:** CMXsrv_fincol_eava

#### Tablas Involucradas:
- DAC
- AVAL
- AVAL_REN
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL00103.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_fincol_cons_aval

#### Tablas Involucradas:
- CRDCLON
- AVAL
- AVAL_REN
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL00113.FRM
**Segmento:** ingresar_Click
**Procedimiento Almacenado:** CMXsrv_fincol_iava

#### Tablas Involucradas:
- AVAL
- AVAL_REN
- CLN
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL00303.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_fincol_cons_pag

#### Tablas Involucradas:
- CAN
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL00303.FRM
**Segmento:** proximos_Click
**Procedimiento Almacenado:** CMXsrv_fincol_cons_pag

#### Tablas Involucradas:
- CAN
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL00304.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_fincol_trae_det_pag

#### Tablas Involucradas:
- CAN
- EVE

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL00403.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_fincol_cons_pror

#### Tablas Involucradas:
- EVE
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL00901.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_fincol_cons_eve

#### Tablas Involucradas:
- EVE
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00602.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_icrd_lee_bco_swf

#### Tablas Involucradas:
- ACMXPAIS
- COR

#### Procedimientos Llamados:
- CMXsrv_icrd_lee_cln
- sp_procxmode

---

### Archivo: CRD00602.FRM
**Segmento:** buscar_Click
**Procedimiento Almacenado:** CMXsrv_icrd_busc_bco

#### Tablas Involucradas:
- COR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00602.FRM
**Segmento:** proximo_Click
**Procedimiento Almacenado:** CMXsrv_icrd_busc_bco

#### Tablas Involucradas:
- COR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD01401.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_fincol_vtocre_prov

#### Tablas Involucradas:
- TIP
- comex..ACMXINTEREFEC
- COR
- CRD
- CUO
- OBL
- NEG
- NEG_ADI
- DAC
- ACMXINTERE
- ACMXMONEDA
- ACMXINTEREFEC
- AVAL
- MYC
- COL
- CTO

#### Procedimientos Llamados:
- CMXsrv_fincol_gpln
- CMXsrv_finobl_imod_obl
- CMXsrv_util_fecha
- CMXsrv_util_val_tasas
- CMXsrv_fincol_efec_calpa
- sp_procxmode
- CMXsrv_fincol_ctb_vcp
- sp_cmx_sii_1870

---

### Archivo: CRD01401.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_fincol_prec_vtocre

#### Tablas Involucradas:
- TIP
- CRD
- CNEG
- NEG
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD02001.FRM
**Segmento:** buscar_Click
**Procedimiento Almacenado:** CMXsrv_icrd_bus_lcr_bco

#### Tablas Involucradas:
- COR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD02001.FRM
**Segmento:** proximo_Click
**Procedimiento Almacenado:** CMXsrv_icrd_bus_lcr_bco

#### Tablas Involucradas:
- COR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: PREFER.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_grl_fec_serv

#### Tablas Involucradas:

#### Procedimientos Llamados:
- SRV_MessageService
- sp_procxmode

---

### Archivo: PREFER.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_lee_fpro

#### Tablas Involucradas:
- ACMXFECPRO

#### Procedimientos Llamados:
- sp_procxmode

---

## INGRESO
<a name="ingreso"></a>
### Archivo: COL00102.FRM
**Segmento:** cancelar_Click
**Procedimiento Almacenado:** CMXsrv_fincol_ren_fin

#### Tablas Involucradas:
- COL_REN
- TIP
- TAS
- TAS_REN
- EVE_REN
- DAC_REN
- ITA
- CUO_REN
- AVAL_REN
- EVE
- CAN_REN
- COL

#### Procedimientos Llamados:
- CMXsrv_cmx_fec_hoy
- CMXsrv_fincol_pre_cuad_tas
- sp_procxmode
- CMXsrv_fincol_grb_col_ren
- CMXsrv_lee_fpro

---

### Archivo: COL00102.FRM
**Segmento:** ELIMINAR_Click
**Procedimiento Almacenado:** CMXsrv_fincol_ecuo

#### Tablas Involucradas:
- CUO_REN
- COL
- CUO

#### Procedimientos Llamados:
- CMXsrv_fincol_pre_cuad_tas
- sp_procxmode

---

### Archivo: COL00102.FRM
**Segmento:** form_activate
**Procedimiento Almacenado:** CMXsrv_fincol_cons_plnpa

#### Tablas Involucradas:
- CUO_REN
- COL_REN
- COL
- CUO

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL00103.FRM
**Segmento:** cancelar_Click
**Procedimiento Almacenado:** CMXsrv_fincol_ren_fin

#### Tablas Involucradas:
- COL_REN
- TIP
- TAS
- TAS_REN
- EVE_REN
- DAC_REN
- ITA
- CUO_REN
- AVAL_REN
- EVE
- CAN_REN
- COL

#### Procedimientos Llamados:
- CMXsrv_cmx_fec_hoy
- CMXsrv_fincol_pre_cuad_tas
- sp_procxmode
- CMXsrv_fincol_grb_col_ren
- CMXsrv_lee_fpro

---

### Archivo: COL00103.FRM
**Segmento:** ELIMINAR_Click
**Procedimiento Almacenado:** CMXsrv_fincol_eava

#### Tablas Involucradas:
- DAC
- AVAL
- AVAL_REN
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL00103.FRM
**Segmento:** form_activate
**Procedimiento Almacenado:** CMXsrv_fincol_cons_aval

#### Tablas Involucradas:
- CRDCLON
- AVAL
- AVAL_REN
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL00104.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_fincol_gmod_ctr

#### Tablas Involucradas:
- TIP
- CUO
- OBL
- CTR
- CLN
- COL
- CTO

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL00104.FRM
**Segmento:** busca_bco
**Procedimiento Almacenado:** CMXsrv_icrd_lee_bco_swf

#### Tablas Involucradas:
- ACMXPAIS
- COR

#### Procedimientos Llamados:
- CMXsrv_icrd_lee_cln
- sp_procxmode

---

### Archivo: COL00104.FRM
**Segmento:** fld_obl_bco_acr_LostFocus
**Procedimiento Almacenado:** CMXsrv_fincol_lee_bco

#### Tablas Involucradas:
- COR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL00104.FRM
**Segmento:** fld_obl_rut_acr_LostFocus
**Procedimiento Almacenado:** CMXsrv_fincol_lee_cln

#### Tablas Involucradas:
- CLN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL00104.FRM
**Segmento:** form_activate
**Procedimiento Almacenado:** CMXsrv_fincol_cons_ctr

#### Tablas Involucradas:
- OBL
- CTR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL00105.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_fincol_ctb_oto

#### Tablas Involucradas:
- TIP
- ACMXDESEMB
- CUO
- COD
- vig_cmx
- COL_ADI
- ACMXPRMGRL
- OBL
- COM
- MYC
- ACMXMONEDA
- LIB
- OPE_BCI
- CLN
- COL
- CCO

#### Procedimientos Llamados:
- CMXsrv_mbyte_gen
- CMXsrv_cmx_ing_lib
- CMXsrv_ctb_impto_tim
- CMXsrv_ctb_otorga
- CMXsrv_cnt_gen_vig
- CMXsrv_nibx_upd_tran
- CMXsrv_ctb_impto_tim2
- CMXsrv_vig_gra_vig
- CMXsrv_nibx_nilive
- CMXsrv_cyo_dsc
- sp_procxmode
- CMXsrv_fincol_val_col
- CMXsrv_cnt_999999
- sp_cmx_sii_1870
- CMXsrv_util_pesos
- CMXsrv_lee_fpro

---

### Archivo: COL00106.FRM
**Segmento:** Avi5_Click
**Procedimiento Almacenado:** CMXsrv_icrd_dat_liq_ope

#### Tablas Involucradas:
- ACMXDESEMB
- ASND
- EVO
- CRD
- CNO
- OBL
- CUO
- TRSD
- NEG
- COM
- EVE
- ACMXTIPEVE
- CAN
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL00106.FRM
**Segmento:** form_activate
**Procedimiento Almacenado:** CMXsrv_fincol_lee_col

#### Tablas Involucradas:
- COR
- TAS
- NEG_ADI
- ACMXINTERE
- TIP
- CUO
- CCL
- ACMXFINVER
- ACMXAPROBAC
- COL_ADI
- ACMXACTIVIDA
- ACMXINTEREFEC
- AVAL
- ACMXSUCSAL
- CLN
- comex..ACMXINTEREFEC
- COM
- ACMXMONEDA
- EVE
- tbl_User
- COL

#### Procedimientos Llamados:
- PrmACMXESPECI
- PrmACLNEJECTA
- sp_procxmode

---

### Archivo: COL00106.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_lee_fpro

#### Tablas Involucradas:
- ACMXFECPRO

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL00106.FRM
**Segmento:** MCOLCOMI_CLICK
**Procedimiento Almacenado:** CMXsrv_busc_cod_ope

#### Tablas Involucradas:
- TIP
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL00106.FRM
**Segmento:** MCOLCOMI_CLICK
**Procedimiento Almacenado:** CMXsrv_col_trae_num_ope

#### Tablas Involucradas:
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL00106.FRM
**Segmento:** MCOLCONTOTOR_CLICK
**Procedimiento Almacenado:** CMXsrv_busc_cod_ope

#### Tablas Involucradas:
- TIP
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL00106.FRM
**Segmento:** MCOLCONTOTOR_CLICK
**Procedimiento Almacenado:** CMXsrv_col_trae_num_ope

#### Tablas Involucradas:
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL00106.FRM
**Segmento:** MCOLCONTOTOR_CLICK
**Procedimiento Almacenado:** CMXsrv_fincol_ctb_oto

#### Tablas Involucradas:
- TIP
- ACMXDESEMB
- CUO
- COD
- vig_cmx
- COL_ADI
- ACMXPRMGRL
- OBL
- COM
- MYC
- ACMXMONEDA
- LIB
- OPE_BCI
- CLN
- COL
- CCO

#### Procedimientos Llamados:
- CMXsrv_mbyte_gen
- CMXsrv_cmx_ing_lib
- CMXsrv_ctb_impto_tim
- CMXsrv_ctb_otorga
- CMXsrv_cnt_gen_vig
- CMXsrv_nibx_upd_tran
- CMXsrv_ctb_impto_tim2
- CMXsrv_vig_gra_vig
- CMXsrv_nibx_nilive
- CMXsrv_cyo_dsc
- sp_procxmode
- CMXsrv_fincol_val_col
- CMXsrv_cnt_999999
- sp_cmx_sii_1870
- CMXsrv_util_pesos
- CMXsrv_lee_fpro

---

### Archivo: COL00106.FRM
**Segmento:** MCOLELI_CLICK
**Procedimiento Almacenado:** CMXsrv_fincol_eli_col

#### Tablas Involucradas:
- COL_REN
- COL_ADI
- COM
- TAS_REN
- DAC_REN
- EVE_REN
- DAC
- CUO_REN
- AVAL_REN
- LIB
- CAN_REN
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL00106.FRM
**Segmento:** valida
**Procedimiento Almacenado:** CMXsrv_fincol_val_col

#### Tablas Involucradas:
- TIP
- COL
- warnmsg

#### Procedimientos Llamados:
- CMXsrv_fincol_val_err
- CMXsrv_fincol_val_per_tas
- CMXsrv_fincol_val_adv
- sp_procxmode

---

### Archivo: COL00107.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_fincol_lee_col

#### Tablas Involucradas:
- COR
- TAS
- NEG_ADI
- ACMXINTERE
- TIP
- CUO
- CCL
- ACMXFINVER
- ACMXAPROBAC
- COL_ADI
- ACMXACTIVIDA
- ACMXINTEREFEC
- AVAL
- ACMXSUCSAL
- CLN
- comex..ACMXINTEREFEC
- COM
- ACMXMONEDA
- EVE
- tbl_User
- COL

#### Procedimientos Llamados:
- PrmACMXESPECI
- PrmACLNEJECTA
- sp_procxmode

---

### Archivo: COL00107.FRM
**Segmento:** buscar_Click
**Procedimiento Almacenado:** CMXsrv_fincol_bsc_col

#### Tablas Involucradas:
- TIP

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL00107.FRM
**Segmento:** fld_col_tip_ope_lostfocus
**Procedimiento Almacenado:** CMXsrv_fincol_lee_tip

#### Tablas Involucradas:
- TIP

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL00107.FRM
**Segmento:** PROXIMAS_Click
**Procedimiento Almacenado:** CMXsrv_fincol_bsc_col

#### Tablas Involucradas:
- TIP

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL00113.FRM
**Segmento:** ingresar_Click
**Procedimiento Almacenado:** CMXsrv_fincol_iava

#### Tablas Involucradas:
- AVAL
- AVAL_REN
- CLN
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL00701.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_busc_cod_ope

#### Tablas Involucradas:
- TIP
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL00701.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_col_trae_num_ope

#### Tablas Involucradas:
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL00701.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_fincol_ctb_novf

#### Tablas Involucradas:
- CLN
- COL

#### Procedimientos Llamados:
- CMXsrv_fincol_ctb_nov
- sp_procxmode
- CMXsrv_lee_fpro

---

### Archivo: COL00701.FRM
**Segmento:** FLD_COL_COD_CLI_LOSTFOCUS
**Procedimiento Almacenado:** CMXsrv_fincol_lee_cln

#### Tablas Involucradas:
- CLN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL00701.FRM
**Segmento:** FLD_COL_RUT_DEU_NOV_LostFocus
**Procedimiento Almacenado:** CMXsrv_fincol_lee_cln

#### Tablas Involucradas:
- CLN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL00702.FRM
**Segmento:** form_activate
**Procedimiento Almacenado:** CMXsrv_fincol_cons_nov

#### Tablas Involucradas:
- EVE
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL00703.FRM
**Segmento:** FLD_COL_COD_CLI_LOSTFOCUS
**Procedimiento Almacenado:** CMXsrv_fincol_lee_cln

#### Tablas Involucradas:
- CLN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL00703.FRM
**Segmento:** FLD_COL_RUT_DEU_NOV_LostFocus
**Procedimiento Almacenado:** CMXsrv_fincol_lee_cln

#### Tablas Involucradas:
- CLN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00602.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_icrd_lee_bco_swf

#### Tablas Involucradas:
- ACMXPAIS
- COR

#### Procedimientos Llamados:
- CMXsrv_icrd_lee_cln
- sp_procxmode

---

### Archivo: CRD00602.FRM
**Segmento:** buscar_Click
**Procedimiento Almacenado:** CMXsrv_icrd_busc_bco

#### Tablas Involucradas:
- COR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00602.FRM
**Segmento:** proximo_Click
**Procedimiento Almacenado:** CMXsrv_icrd_busc_bco

#### Tablas Involucradas:
- COR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: PREFER.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_cmx_get_codes

#### Tablas Involucradas:

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: PREFER.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_grl_trae_cod_bco

#### Tablas Involucradas:

#### Procedimientos Llamados:
- sp_procxmode

---

## MODIFIC
<a name="modific"></a>
### Archivo: COL00303.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_fincol_cons_tas

#### Tablas Involucradas:
- TAS

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL00801.FRM
**Segmento:** aceptar_click
**Procedimiento Almacenado:** CMXsrv_fincol_efec_tras

#### Tablas Involucradas:
- TIP
- comex..ACMXMONEDAFEC
- COL
- CUO

#### Procedimientos Llamados:
- CMXsrv_fincol_ctb_cnd
- CMXsrv_fincol_ctb_cob
- CMXsrv_cnt_9000
- CMXsrv_fincol_ctb_cst
- sp_procxmode
- CMXsrv_fincol_calc_cven

---

### Archivo: COL00802.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_fincol_cons_trasp

#### Tablas Involucradas:
- EVE
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL00803.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_fincol_cons_dtrs

#### Tablas Involucradas:
- EVE
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL00901.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_fincol_cons_eve

#### Tablas Involucradas:
- EVE
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL00902.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_fincol_cons_deve

#### Tablas Involucradas:
- EVE
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL01001.FRM
**Segmento:** aceptar_click
**Procedimiento Almacenado:** CMXsrv_fincol_cont_gst

#### Tablas Involucradas:

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL01002.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_fincol_cons_gst

#### Tablas Involucradas:
- EVE
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL01003.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_fincol_cons_dgst

#### Tablas Involucradas:

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: PREFER.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_lee_fpro

#### Tablas Involucradas:
- ACMXFECPRO

#### Procedimientos Llamados:
- sp_procxmode

---

## OBLIGA
<a name="obliga"></a>
### Archivo: COL00108.FRM
**Segmento:** buscar_Click
**Procedimiento Almacenado:** CMXsrv_fincol_bsc_tip

#### Tablas Involucradas:
- TIP

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL00108.FRM
**Segmento:** Proxima_Click
**Procedimiento Almacenado:** CMXsrv_fincol_bsc_tip

#### Tablas Involucradas:
- TIP

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL00108.FRM
**Segmento:** proximo_Click
**Procedimiento Almacenado:** CMXsrv_fincol_bsc_tip

#### Tablas Involucradas:
- TIP

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00602.FRM
**Segmento:** buscar_Click
**Procedimiento Almacenado:** CMXsrv_finobl_bus_cor

#### Tablas Involucradas:
- COR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00602.FRM
**Segmento:** proximo_Click
**Procedimiento Almacenado:** CMXsrv_finobl_bus_cor

#### Tablas Involucradas:
- COR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: OBL00102.FRM
**Segmento:** ELIMINAR_Click
**Procedimiento Almacenado:** CMXsrv_finobl_ecuo

#### Tablas Involucradas:
- OBL
- CTO

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: OBL00102.FRM
**Segmento:** form_activate
**Procedimiento Almacenado:** CMXsrv_finobl_gpln

#### Tablas Involucradas:
- OBL
- CTO

#### Procedimientos Llamados:
- CMXsrv_util_det_habil_tasa
- sp_procxmode

---

### Archivo: OBL00102.FRM
**Segmento:** form_activate
**Procedimiento Almacenado:** CMXsrv_finobl_cons_plnpa

#### Tablas Involucradas:
- OBL
- CTO

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: OBL00103.FRM
**Segmento:** anunctb_Click
**Procedimiento Almacenado:** CMXsrv_finobl_calc_anu

#### Tablas Involucradas:
- OBL

#### Procedimientos Llamados:
- sp_procxmode
- CMXsrv_finobl_efec_calpa
- CMXsrv_lee_fpro

---

### Archivo: OBL00103.FRM
**Segmento:** form_activate
**Procedimiento Almacenado:** CMXsrv_finobl_lee_obl

#### Tablas Involucradas:
- TIP
- COR
- OBL
- ACMXINTERE
- ACMXMONEDA
- ACMXSUCSAL
- CLN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: OBL00103.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_lee_fpro

#### Tablas Involucradas:
- ACMXFECPRO

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: OBL00103.FRM
**Segmento:** Mcbeanl_Click
**Procedimiento Almacenado:** CMXsrv_finobl_calc_anu

#### Tablas Involucradas:
- OBL

#### Procedimientos Llamados:
- sp_procxmode
- CMXsrv_finobl_efec_calpa
- CMXsrv_lee_fpro

---

### Archivo: OBL00103.FRM
**Segmento:** Mcbectb_Click
**Procedimiento Almacenado:** CMXsrv_finobl_ctb_oto

#### Tablas Involucradas:
- ACMXDESEMB
- TIP
- COD
- OBL
- CTO
- CCO

#### Procedimientos Llamados:
- CMXsrv_ctbo_otorga
- CMXsrv_finobl_val_obl
- sp_procxmode
- CMXsrv_lee_fpro

---

### Archivo: OBL00103.FRM
**Segmento:** Mcbedel_Click
**Procedimiento Almacenado:** CMXsrv_fincol_eli_obl

#### Tablas Involucradas:
- OBL
- OBL_ADI

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: OBL00103.FRM
**Segmento:** Mobl_liq_ope_Click
**Procedimiento Almacenado:** CMXsrv_icrd_dat_liq_ope

#### Tablas Involucradas:
- ACMXDESEMB
- ASND
- EVO
- CRD
- CNO
- OBL
- CUO
- TRSD
- NEG
- COM
- EVE
- ACMXTIPEVE
- CAN
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: OBL00103.FRM
**Segmento:** valida_error
**Procedimiento Almacenado:** CMXsrv_finobl_val_obl

#### Tablas Involucradas:
- TIP
- OBL
- ACMXINTERE
- warnmsg
- OBL_ADI

#### Procedimientos Llamados:
- CMXsrv_util_det_habil_tasa
- CMXsrv_finobl_val_adv
- sp_procxmode

---

### Archivo: OBL00104.FRM
**Segmento:** buscar_Click
**Procedimiento Almacenado:** CMXsrv_finobl_bsc_obl

#### Tablas Involucradas:
- OBL

#### Procedimientos Llamados:
- CMXsrv_finobl_bsc_obl2
- sp_procxmode
- CMXsrv_finobl_bsc_obl3

---

### Archivo: OBL00104.FRM
**Segmento:** fld_obl_tip_ope_LostFocus
**Procedimiento Almacenado:** CMXsrv_fincol_lee_tip

#### Tablas Involucradas:
- TIP

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: OBL00104.FRM
**Segmento:** Proxima_Click
**Procedimiento Almacenado:** CMXsrv_finobl_bsc_obl

#### Tablas Involucradas:
- OBL

#### Procedimientos Llamados:
- CMXsrv_finobl_bsc_obl2
- sp_procxmode
- CMXsrv_finobl_bsc_obl3

---

### Archivo: OBL00202.FRM
**Segmento:** contabilizar_Click
**Procedimiento Almacenado:** CMXsrv_finobl_ictb_pag

#### Tablas Involucradas:
- OBL
- CTO
- EVO

#### Procedimientos Llamados:
- CMXsrv_finobl_ctb_pag
- sp_procxmode
- CMXsrv_lee_fpro

---

### Archivo: OBL00202.FRM
**Segmento:** contabilizar_Click
**Procedimiento Almacenado:** CMXsrv_finobl_obt_sdocuo

#### Tablas Involucradas:
- OBL
- CTO

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: OBL00202.FRM
**Segmento:** form_activate
**Procedimiento Almacenado:** CMXsrv_finobl_new_tas

#### Tablas Involucradas:
- CTO

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: OBL00203.FRM
**Segmento:** form_activate
**Procedimiento Almacenado:** CMXsrv_finobl_cons_pag

#### Tablas Involucradas:
- CNO

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: OBL00204.FRM
**Segmento:** form_activate
**Procedimiento Almacenado:** CMXsrv_finobl_cons_detp

#### Tablas Involucradas:
- OBL
- CTO
- EVO

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: OBL00301.FRM
**Segmento:** calcular_Click
**Procedimiento Almacenado:** CMXsrv_finobl_calc_pror

#### Tablas Involucradas:
- OBL

#### Procedimientos Llamados:
- sp_procxmode
- CMXsrv_finobl_efec_calpa
- CMXsrv_lee_fpro

---

### Archivo: OBL00303.FRM
**Segmento:** form_activate
**Procedimiento Almacenado:** CMXsrv_finobl_cons_pror

#### Tablas Involucradas:
- OBL
- EVO

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: OBL00304.FRM
**Segmento:** form_activate
**Procedimiento Almacenado:** CMXsrv_finobl_cons_dpror

#### Tablas Involucradas:
- OBL
- EVO

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: OBL00401.FRM
**Segmento:** contabilizar_Click
**Procedimiento Almacenado:** CMXsrv_finobl_ctb_anu

#### Tablas Involucradas:
- TIP
- COR
- OBL
- COL
- CTO

#### Procedimientos Llamados:
- CMXsrv_finobl_cbo_anu
- CMXsrv_ctbo_anula
- sp_procxmode
- CMXsrv_lee_fpro

---

### Archivo: OBL00402.FRM
**Segmento:** calcular_Click
**Procedimiento Almacenado:** CMXsrv_finobl_calc_anu

#### Tablas Involucradas:
- OBL

#### Procedimientos Llamados:
- sp_procxmode
- CMXsrv_finobl_efec_calpa
- CMXsrv_lee_fpro

---

### Archivo: OBL00402.FRM
**Segmento:** form_activate
**Procedimiento Almacenado:** CMXsrv_finobl_cons_anu

#### Tablas Involucradas:
- CNO
- EVO

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: OBL00502.FRM
**Segmento:** form_activate
**Procedimiento Almacenado:** CMXsrv_finobl_cons_mod

#### Tablas Involucradas:
- OBL
- EVO

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: OBL00503.FRM
**Segmento:** form_activate
**Procedimiento Almacenado:** CMXsrv_finobl_cons_dmod

#### Tablas Involucradas:
- CNO
- EVO

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: OBL00601.FRM
**Segmento:** efectuar_Click
**Procedimiento Almacenado:** CMXsrv_finobl_rev_eve

#### Tablas Involucradas:
- OBL
- TRSD
- APRCBL
- EVO

#### Procedimientos Llamados:
- CMXsrv_ctl_marc_rev
- CMXsrv_ctl_chq_aprcbl
- CMXsrv_finobl_rctb_pext
- CMXsrv_rctb_cesi
- sp_procxmode
- CMXsrv_finobl_rctb_pag
- CMXsrv_finobl_rctb_pror
- CMXsrv_finobl_rctb_mod
- CMXsrv_finobl_rctb_anu
- CMXsrv_finobl_rctb_oto

---

### Archivo: OBL00601.FRM
**Segmento:** form_activate
**Procedimiento Almacenado:** CMXsrv_finobl_cons_eve

#### Tablas Involucradas:
- EVO

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: OBL00602.FRM
**Segmento:** form_activate
**Procedimiento Almacenado:** CMXsrv_finobl_cons_deve

#### Tablas Involucradas:
- EVO

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: OBL00701.FRM
**Segmento:** ELIMINAR_Click
**Procedimiento Almacenado:** CMXsrv_finobl_eli_ctr

#### Tablas Involucradas:
- CTR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: OBL00701.FRM
**Segmento:** form_activate
**Procedimiento Almacenado:** CMXsrv_finobl_cons_ctr

#### Tablas Involucradas:
- CTR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: OBL00702.FRM
**Segmento:** nuevo_Click
**Procedimiento Almacenado:** CMXsrv_finobl_ing_ctr

#### Tablas Involucradas:
- COL
- OBL
- TIP
- CTR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: OBL130.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_finobl_cesion_obl

#### Tablas Involucradas:
- OBL
- COR

#### Procedimientos Llamados:
- CMXsrv_ctl_crea_apr
- sp_procxmode
- CMXsrv_lee_fpro

---

### Archivo: OBL130.FRM
**Segmento:** banco_acreedor
**Procedimiento Almacenado:** CMXsrv_comgrl_lee_nom_cor

#### Tablas Involucradas:
- COR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: OBL130.FRM
**Segmento:** fld_obl_cod_bco_acre_lostfocus
**Procedimiento Almacenado:** CMXsrv_comgrl_lee_nom_cor

#### Tablas Involucradas:
- COR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: OBL130.FRM
**Segmento:** fld_obl_rut_acre_lostfocus
**Procedimiento Almacenado:** CMXsrv_lee_cln

#### Tablas Involucradas:
- CLN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: OBL130.FRM
**Segmento:** form_activate
**Procedimiento Almacenado:** CMXsrv_finobl_busc_acre

#### Tablas Involucradas:
- OBL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: PREFER.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_cmx_get_codes

#### Tablas Involucradas:

#### Procedimientos Llamados:
- sp_procxmode

---

## PAGOS
<a name="pagos"></a>
### Archivo: COL00301.FRM
**Segmento:** CALCULAR_Click
**Procedimiento Almacenado:** CMXsrv_fincol_efec_calpa

#### Tablas Involucradas:
- TF_PPAG
- TIP
- TAS
- CUO
- comex..ACMXMONEDA
- COL_ADI
- OBL
- CTR
- NEG_ADI
- ACMXINTERE
- CAN
- ICR
- COL

#### Procedimientos Llamados:
- CMXsrv_fincol_eval_tnem
- CMXsrv_fincol_eval_tmor
- CMXsrv_util_det_habil
- sp_procxmode
- CMXsrv_fincol_calc_reba
- CMXsrv_fincol_eval_tasa
- CMXsrv_fincol_eval_tneg
- CMXsrv_fincol_efcal_cv
- CMXsrv_fincol_cal_tas_sfr

---

### Archivo: COL00303.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_fincol_cons_pag

#### Tablas Involucradas:
- CAN
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL00304.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_fincol_cons_detp

#### Tablas Involucradas:
- ACMXDESEMB
- EVE
- COL
- CUO

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL00401.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_fincol_calc_pror

#### Tablas Involucradas:
- ACMXINTERE
- COL

#### Procedimientos Llamados:
- CMXsrv_call_val_tas
- sp_procxmode
- CMXsrv_fincol_efec_calpa

---

### Archivo: COL00402.FRM
**Segmento:** Contabilizar_Click
**Procedimiento Almacenado:** CMXsrv_fincol_cont_pror

#### Tablas Involucradas:
- TAS
- CRD
- NEG_ADI
- ACMXINTERE
- TIP
- CUO
- OBL
- CAM_TAS
- ACMXPLAZO
- COL_ADI
- LIB
- ACMXINTEREFEC
- CLN
- ACMXOPEIMP
- CTO
- de
- comex..ACMXINTEREFEC
- COD
- COM
- ACMXMONEDAFEC
- EVE
- CAN
- COL

#### Procedimientos Llamados:
- CMXsrv_mbyte_gen
- CMXsrv_fincol_ctb_pror
- CMXsrv_get_ult_dia_habil
- CMXsrv_cmx_ing_lib
- CMXsrv_ctb_impto_tim
- CMXsrv_ipuc_gen_pln
- CMXsrv_util_val_tasas
- sp_procxmode
- CMXsrv_pertas_pror_tas
- CMXsrv_cmx_get_codes
- CMXsrv_int_ccx_cns
- CMXsrv_util_pesos
- CMXsrv_fincol_cam_new_tas
- CMXsrv_lee_fpro

---

### Archivo: COL00403.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_fincol_cons_pror

#### Tablas Involucradas:
- EVE
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL00404.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_fincol_cons_dpror

#### Tablas Involucradas:
- ACMXDESEMB
- EVE
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL00501.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_busc_cod_ope

#### Tablas Involucradas:
- TIP
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL00501.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_col_trae_num_ope

#### Tablas Involucradas:
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL00501.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_fincol_cctb_anu

#### Tablas Involucradas:
- TIP
- CUO
- COD
- OBL
- TF_ENL
- ENL
- CAN
- COL
- CTO

#### Procedimientos Llamados:
- CMXsrv_busc_cod_ope
- CMXsrv_enl_act_enl
- sp_procxmode
- CMXsrv_fincol_ctb_anu
- sp_cmx_sii_1870
- CMXsrv_lee_fpro

---

### Archivo: COL00501.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_fincol_calc_anu

#### Tablas Involucradas:
- TIP
- COL

#### Procedimientos Llamados:
- sp_procxmode
- CMXsrv_fincol_efec_calpa

---

### Archivo: COL00501.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_busc_cod_ope

#### Tablas Involucradas:
- TIP
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL00502.FRM
**Segmento:** CALCULAR_Click
**Procedimiento Almacenado:** CMXsrv_fincol_calc_anu

#### Tablas Involucradas:
- TIP
- COL

#### Procedimientos Llamados:
- sp_procxmode
- CMXsrv_fincol_efec_calpa

---

### Archivo: COL00502.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_fincol_cons_anu

#### Tablas Involucradas:
- ACMXDESEMB
- CAN
- EVE
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL00602.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_fincol_cons_mod

#### Tablas Involucradas:
- EVE
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COL00603.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_fincol_cons_dmod

#### Tablas Involucradas:
- CAN
- EVE

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: PREFER.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_lee_fpro

#### Tablas Involucradas:
- ACMXFECPRO

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: PREFER.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_grl_trae_cod_bco

#### Tablas Involucradas:

#### Procedimientos Llamados:
- sp_procxmode

---

## PGOEXT
<a name="pgoext"></a>
### Archivo: PGOCOL01.FRM
**Segmento:** calcular_Click
**Procedimiento Almacenado:** CMXsrv_fincol_cal_pext

#### Tablas Involucradas:
- TIP
- CUO
- comex..ACMXMONEDA
- OBL
- CTR
- COL
- CTO

#### Procedimientos Llamados:
- CMXsrv_fincol_calc_reba
- CMXsrv_fincol_eval_tasa
- sp_procxmode

---

### Archivo: PGOCOL01.FRM
**Segmento:** Contabilizar_Click
**Procedimiento Almacenado:** CMXsrv_busc_cod_ope

#### Tablas Involucradas:
- TIP
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: PGOCOL01.FRM
**Segmento:** Contabilizar_Click
**Procedimiento Almacenado:** CMXsrv_fincol_ctb_pext

#### Tablas Involucradas:
- TIP
- ACMXDESEMB
- comex..ACMXINTEREFEC
- TAS
- CUO
- COD
- OBL
- COL_ADI
- ACMXMONEDAFEC
- CTR
- NEG_ADI
- ACMXINTERE
- EVE
- ACMXINTEREFEC
- COL
- CTO
- CCO

#### Procedimientos Llamados:
- CMXsrv_ctb_pago
- CMXsrv_util_gen_vig
- sp_procxmode
- CMXsrv_lee_fpro

---

### Archivo: PGOOBL01.FRM
**Segmento:** calcular_Click
**Procedimiento Almacenado:** CMXsrv_finobl_cal_pext

#### Tablas Involucradas:
- TIP
- OBL
- ACMXINTERE
- ACMXMONEDA
- OBL_ADI
- CTO

#### Procedimientos Llamados:
- CMXsrv_finobl_eval_tasa
- sp_procxmode
- CMXsrv_fincol_cal_tas_sfr

---

### Archivo: PGOOBL01.FRM
**Segmento:** Contabilizar_Click
**Procedimiento Almacenado:** CMXsrv_finobl_ctb_pext

#### Tablas Involucradas:
- ACMXDESEMB
- TIP
- COD
- OBL
- ACMXMONEDAFEC
- CTO
- CCO

#### Procedimientos Llamados:
- CMXsrv_ctbo_pago
- sp_procxmode
- CMXsrv_lee_fpro

---

### Archivo: PREFER.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_grl_fec_serv

#### Tablas Involucradas:

#### Procedimientos Llamados:
- SRV_MessageService
- sp_procxmode

---

### Archivo: PREFER.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_lee_fpro

#### Tablas Involucradas:
- ACMXFECPRO

#### Procedimientos Llamados:
- sp_procxmode

---

## ARCOS
<a name="arcos"></a>
### Archivo: ARC00100.FRM
**Segmento:** Eliminar_Click
**Procedimiento Almacenado:** CMXsrv_iarc_eli_arc

#### Tablas Involucradas:
- ADI
- CRD
- ARC
- NEG
- COB
- INF
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: ARC00100.FRM
**Segmento:** Form_activate
**Procedimiento Almacenado:** CMXsrv_iarc_busc_arc

#### Tablas Involucradas:
- ARC

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: ARC00101.FRM
**Segmento:** aceptar_click
**Procedimiento Almacenado:** CMXsrv_iinf_busc_inf

#### Tablas Involucradas:
- INF

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: ARC00101.FRM
**Segmento:** aceptar_click
**Procedimiento Almacenado:** CMXsrv_iarc_act_arc

#### Tablas Involucradas:
- CRD
- comex..ACMXMONEDA
- ARC
- NEG
- CBR
- ACMXMONEDAFEC
- INF
- COL

#### Procedimientos Llamados:
- CMXsrv_cmx_get_codes
- PrmACMXMONEDAFEC
- CMXsrv_util_opr_fec
- sp_procxmode

---

### Archivo: ARC00101.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_iarc_lee_arc

#### Tablas Involucradas:
- ARC

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: INFO0201.FRM
**Segmento:** buscar_Click
**Procedimiento Almacenado:** CMXsrv_iinf_busc_opr

#### Tablas Involucradas:
- ARC

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: INFO0201.FRM
**Segmento:** Form_activate
**Procedimiento Almacenado:** CMXsrv_iinf_lee_vlr

#### Tablas Involucradas:
- INF

#### Procedimientos Llamados:
- PrmACMXCLACOM
- sp_procxmode

---

### Archivo: INFO0202.FRM
**Segmento:** aceptar_click
**Procedimiento Almacenado:** CMXsrv_iarc_act_arc

#### Tablas Involucradas:
- CRD
- comex..ACMXMONEDA
- ARC
- NEG
- CBR
- ACMXMONEDAFEC
- INF
- COL

#### Procedimientos Llamados:
- CMXsrv_cmx_get_codes
- PrmACMXMONEDAFEC
- CMXsrv_util_opr_fec
- sp_procxmode

---

### Archivo: INFO0202.FRM
**Segmento:** Form_activate
**Procedimiento Almacenado:** CMXsrv_iinf_busc_inf

#### Tablas Involucradas:
- INF

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: INFO0202.FRM
**Segmento:** reversar_Click
**Procedimiento Almacenado:** CMXsrv_iinf_rev_evi

#### Tablas Involucradas:
- INF
- ARC
- INC
- EVI

#### Procedimientos Llamados:
- CMXsrv_com_rev
- sp_procxmode

---

## COBERIMP
<a name="coberimp"></a>
### Archivo: COB00101.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_icob_lee_pln

#### Tablas Involucradas:
- DIC
- POSBCX10
- COB
- ACMXBCOCEN
- ACMXMONEDA
- ACMXPAIS

#### Procedimientos Llamados:
- CMXsrv_cmx_get_codes
- CMXsrv_icob_obs_pln
- sp_procxmode

---

### Archivo: COB00101.FRM
**Segmento:** Mcobcur_Click
**Procedimiento Almacenado:** CMXsrv_icob_cur_cob

#### Tablas Involucradas:
- comex.dbo
- COB

#### Procedimientos Llamados:
- CMXsrv_icob_ctb_reem
- sp_procxmode
- CMXsrv_icob_val_cob

---

### Archivo: COB00101.FRM
**Segmento:** Mcobcur_Click
**Procedimiento Almacenado:** CMXsrv_icob_pag_sop

#### Tablas Involucradas:
- DDI
- ACMXDESEMB
- ADI
- DIC
- ACMXPRMGRL
- ACMXMONEDAFEC
- COB
- INF
- warnmsg

#### Procedimientos Llamados:
- CMXsrv_get_ult_dia_habil
- CMXsrv_icob_refresh_pos
- CMXsrv_val_cta_cte
- CMXsrv_calc_imp_4pct
- CMXsrv_icbr_act_rem
- sp_procxmode
- CMXsrv_icob_ctb_sop
- CMXsrv_ctb_imp_ddi_so
- CMXsrv_cmx_get_codes
- CMXsrv_iddi_marc_ddi2
- CMXsrv_icob_val_cob

---

### Archivo: COB00101.FRM
**Segmento:** MCOBELI_CLICK
**Procedimiento Almacenado:** CMXsrv_icob_eli_pln

#### Tablas Involucradas:
- COB

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COB00101.FRM
**Segmento:** Mcobrev_Click
**Procedimiento Almacenado:** CMXsrv_icob_rev_etd

#### Tablas Involucradas:
- POSBCX10
- TRSD
- PSO
- comex..COB
- COB

#### Procedimientos Llamados:
- CMXsrv_icob_refresh_pos
- CMXsrv_ctl_chq_aprcbl
- CMXsrv_icob_ctb_anu
- CMXsrv_icob_ctb_reem
- sp_procxmode
- CMXsrv_pos_eli_010
- CMXsrv_icob_rctb_sop

---

### Archivo: COB00101.FRM
**Segmento:** Mcobvali_Click
**Procedimiento Almacenado:** CMXsrv_icob_val_cob

#### Tablas Involucradas:
- DDI
- LCB
- ADI
- CUO
- ARC
- NEG
- CBR
- COB
- INF
- ACMXFPAIMP
- warnmsg
- COL

#### Procedimientos Llamados:
- PrmACMXPAIS
- CMXsrv_pos_bcx_lee_cob
- CMXsrv_util_fecha
- sp_procxmode

---

### Archivo: COB00201.FRM
**Segmento:** buscar_click
**Procedimiento Almacenado:** CMXsrv_icob_busc_pln

#### Tablas Involucradas:
- COB

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COB00201.FRM
**Segmento:** FLD_COB_COD_CLI_LostFocus
**Procedimiento Almacenado:** CMXsrv_icob_lee_cln

#### Tablas Involucradas:
- CLN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COB00201.FRM
**Segmento:** PROXIMAS_Click
**Procedimiento Almacenado:** CMXsrv_icob_busc_pln

#### Tablas Involucradas:
- COB

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COB00300.FRM
**Segmento:** ACEPTAR_Click
**Procedimiento Almacenado:** CMXsrv_icob_crea_norm

#### Tablas Involucradas:
- CRD
- ARC
- CBR
- COB
- INF
- tbl_User
- CLN
- COL

#### Procedimientos Llamados:
- sp_procxmode
- CMXsrv_icob_get_num

---

### Archivo: COB00301.FRM
**Segmento:** ACEPTAR_Click
**Procedimiento Almacenado:** CMXsrv_icob_crea_reem

#### Tablas Involucradas:
- DIC
- COB

#### Procedimientos Llamados:
- sp_procxmode
- CMXsrv_icob_get_num
- CMXsrv_cmx_get_codes
- CMXsrv_pos_bcx_lee_cob
- CMXsrv_pos_bcx_ing_cob

---

### Archivo: COB00302.FRM
**Segmento:** ACEPTAR_Click
**Procedimiento Almacenado:** CMXsrv_icob_act_gral

#### Tablas Involucradas:
- CLN
- COB

#### Procedimientos Llamados:
- sp_procxmode
- CMXsrv_icob_num_con
- CMXsrv_icob_val_cob
- CMXsrv_pos_bcx_act_cob

---

### Archivo: COB00302.FRM
**Segmento:** FLD_COB_COD_CLI_LostFocus
**Procedimiento Almacenado:** CMXsrv_icob_lee_cln2

#### Tablas Involucradas:
- CLN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COB00302.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_icob_lee_gral

#### Tablas Involucradas:
- ACMXBCOCEN
- ACMXPAIS
- COB

#### Procedimientos Llamados:
- CMXsrv_pos_bcx_lee_cob
- sp_procxmode

---

### Archivo: COB00303.FRM
**Segmento:** ACEPTAR_Click
**Procedimiento Almacenado:** CMXsrv_icob_act_val

#### Tablas Involucradas:
- ACMXMONEDAFEC
- COB

#### Procedimientos Llamados:
- CMXsrv_get_ult_dia_habil
- sp_procxmode
- CMXsrv_icob_val_cob

---

### Archivo: COB00303.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_icob_lee_val

#### Tablas Involucradas:
- COB

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COB00304.FRM
**Segmento:** ACEPTAR_Click
**Procedimiento Almacenado:** CMXsrv_icob_act_acu

#### Tablas Involucradas:
- COB

#### Procedimientos Llamados:
- sp_procxmode
- CMXsrv_icob_val_cob

---

### Archivo: COB00304.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_icob_lee_acu

#### Tablas Involucradas:
- ACMXPAIS
- COB

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COB00304.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_icob_lee_acu

#### Tablas Involucradas:
- ACMXPAIS
- COB

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COB00305.FRM
**Segmento:** ELIMINAR_Click
**Procedimiento Almacenado:** CMXsrv_icob_eli_int

#### Tablas Involucradas:
- DIC
- COB

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COB00305.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_icob_busc_int

#### Tablas Involucradas:
- DIC

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COB00306.FRM
**Segmento:** ACEPTAR_Click
**Procedimiento Almacenado:** CMXsrv_icob_ingmod_int

#### Tablas Involucradas:
- DIC
- COB

#### Procedimientos Llamados:
- PrmACMXMONEDA
- sp_procxmode
- CMXsrv_icob_val_cob

---

### Archivo: COB00306.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_icob_lee_int

#### Tablas Involucradas:
- DIC

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COB00307.FRM
**Segmento:** ACEPTAR_Click
**Procedimiento Almacenado:** CMXsrv_icob_ing_mod_srf

#### Tablas Involucradas:
- CLN
- tbl_User
- COB

#### Procedimientos Llamados:
- CMXsrv_pos_bcx_ing_cob
- sp_procxmode
- CMXsrv_icob_get_num
- CMXsrv_pos_bcx_act_cob

---

### Archivo: COB00307.FRM
**Segmento:** CmdEliminar_Click
**Procedimiento Almacenado:** CMXsrv_icob_eli_pln

#### Tablas Involucradas:
- COB

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COB00307.FRM
**Segmento:** CmdReversar_Click
**Procedimiento Almacenado:** CMXsrv_icob_rev_etd

#### Tablas Involucradas:
- POSBCX10
- TRSD
- PSO
- comex..COB
- COB

#### Procedimientos Llamados:
- CMXsrv_icob_refresh_pos
- CMXsrv_ctl_chq_aprcbl
- CMXsrv_icob_ctb_anu
- CMXsrv_icob_ctb_reem
- sp_procxmode
- CMXsrv_pos_eli_010
- CMXsrv_icob_rctb_sop

---

### Archivo: COB00307.FRM
**Segmento:** CURSAR_Click
**Procedimiento Almacenado:** CMXsrv_icob_ing_mod_srf

#### Tablas Involucradas:
- CLN
- tbl_User
- COB

#### Procedimientos Llamados:
- CMXsrv_pos_bcx_ing_cob
- sp_procxmode
- CMXsrv_icob_get_num
- CMXsrv_pos_bcx_act_cob

---

### Archivo: COB00307.FRM
**Segmento:** CURSAR_Click
**Procedimiento Almacenado:** CMXsrv_icob_pag_sop

#### Tablas Involucradas:
- DDI
- ACMXDESEMB
- ADI
- DIC
- ACMXPRMGRL
- ACMXMONEDAFEC
- COB
- INF
- warnmsg

#### Procedimientos Llamados:
- CMXsrv_get_ult_dia_habil
- CMXsrv_icob_refresh_pos
- CMXsrv_val_cta_cte
- CMXsrv_calc_imp_4pct
- CMXsrv_icbr_act_rem
- sp_procxmode
- CMXsrv_icob_ctb_sop
- CMXsrv_ctb_imp_ddi_so
- CMXsrv_cmx_get_codes
- CMXsrv_iddi_marc_ddi2
- CMXsrv_icob_val_cob

---

### Archivo: COB00307.FRM
**Segmento:** FLD_COB_COD_CLI_LostFocus
**Procedimiento Almacenado:** CMXsrv_icob_lee_cln2

#### Tablas Involucradas:
- CLN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COB00307.FRM
**Segmento:** Reversar_Click
**Procedimiento Almacenado:** CMXsrv_icob_rev_etd

#### Tablas Involucradas:
- POSBCX10
- TRSD
- PSO
- comex..COB
- COB

#### Procedimientos Llamados:
- CMXsrv_icob_refresh_pos
- CMXsrv_ctl_chq_aprcbl
- CMXsrv_icob_ctb_anu
- CMXsrv_icob_ctb_reem
- sp_procxmode
- CMXsrv_pos_eli_010
- CMXsrv_icob_rctb_sop

---

### Archivo: COB00501.FRM
**Segmento:** ACEPTAR_Click
**Procedimiento Almacenado:** CMXsrv_icob_anu

#### Tablas Involucradas:
- DIC
- POSBCX10
- ACMXMONEDAFEC
- PSO
- COB
- ACMXTPOAUTN

#### Procedimientos Llamados:
- CMXsrv_get_ult_dia_habil
- CMXsrv_icob_refresh_pos
- CMXsrv_icob_ctb_anu
- sp_procxmode
- CMXsrv_pos_bcx_act_cob
- CMXsrv_icob_get_num
- CMXsrv_cmx_get_codes
- CMXsrv_pos_bcx_lee_cob
- CMXsrv_pos_bcx_ing_cob

---

### Archivo: COB00501.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_icob_lee_anu

#### Tablas Involucradas:
- COB

#### Procedimientos Llamados:
- CMXsrv_pos_bcx_lee_cob
- sp_procxmode

---

### Archivo: COB0601.FRM
**Segmento:** FLD_COB_COD_CLI_LostFocus
**Procedimiento Almacenado:** CMXsrv_icob_lee_cln

#### Tablas Involucradas:
- CLN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: FORM2.FRM
**Segmento:** ACEPTAR_Click
**Procedimiento Almacenado:** CMXsrv_icob_pag_sop

#### Tablas Involucradas:
- DDI
- ACMXDESEMB
- ADI
- DIC
- ACMXPRMGRL
- ACMXMONEDAFEC
- COB
- INF
- warnmsg

#### Procedimientos Llamados:
- CMXsrv_get_ult_dia_habil
- CMXsrv_icob_refresh_pos
- CMXsrv_val_cta_cte
- CMXsrv_calc_imp_4pct
- CMXsrv_icbr_act_rem
- sp_procxmode
- CMXsrv_icob_ctb_sop
- CMXsrv_ctb_imp_ddi_so
- CMXsrv_cmx_get_codes
- CMXsrv_iddi_marc_ddi2
- CMXsrv_icob_val_cob

---

### Archivo: ORI_DEST.FRM
**Segmento:** ACEPTAR_Click
**Procedimiento Almacenado:** CMXsrv_icob_cur_reem

#### Tablas Involucradas:
- comex..COB
- COB

#### Procedimientos Llamados:
- CMXsrv_icob_ctb_reem
- sp_procxmode
- CMXsrv_icob_refresh_pos
- CMXsrv_icob_val_cob

---

### Archivo: PREFER.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_grl_fec_serv

#### Tablas Involucradas:

#### Procedimientos Llamados:
- SRV_MessageService
- sp_procxmode

---

## COBRANZA
<a name="cobranza"></a>
### Archivo: CBR00101.FRM
**Segmento:** ejecut_avi_imp_999
**Procedimiento Almacenado:** CMXsrv_busc_cor_swf

#### Tablas Involucradas:
- SWT

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR00101.FRM
**Segmento:** ejecut_avi_imp_999
**Procedimiento Almacenado:** CMXsrv_swf_bus_sms

#### Tablas Involucradas:
- SMS

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR00101.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_icbr_lee_cbr

#### Tablas Involucradas:
- ACMXPAIS
- COR
- LCB
- ACMXVIATPT
- ACMXBCOBCC
- CBR
- ACMXMONEDA
- ACMXCLACOM
- tbl_User
- ACMXSUCSAL
- CLN

#### Procedimientos Llamados:
- PrmACMXESPECI
- PrmACLNEJECTA
- sp_procxmode

---

### Archivo: CBR00101.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_grl_fec_serv

#### Tablas Involucradas:

#### Procedimientos Llamados:
- SRV_MessageService
- sp_procxmode

---

### Archivo: CBR00101.FRM
**Segmento:** Mcbrace_Click
**Procedimiento Almacenado:** CMXsrv_icbr_acep_let

#### Tablas Involucradas:
- comex..CBR
- LCB
- CBR

#### Procedimientos Llamados:
- CMXsrv_ctl_crea_apr
- sp_procxmode

---

### Archivo: CBR00101.FRM
**Segmento:** Mcbrcon_Click
**Procedimiento Almacenado:** CMXsrv_icbr_cont_cbr

#### Tablas Involucradas:
- OPE_BCI
- APRCBL
- LCB
- CBR

#### Procedimientos Llamados:
- CMXsrv_ctl_marc_firma
- CMXsrv_mbyte_gen
- CMXsrv_icbr_val_cbr
- CMXsrv_nibx_upd_tran
- CMXsrv_cnt_gen_vig
- sp_procxmode
- CMXsrv_ctb_cbr
- CMXsrv_nibx_nilive

---

### Archivo: CBR00101.FRM
**Segmento:** Mcbreli_click
**Procedimiento Almacenado:** CMXsrv_icbr_eli_cbr

#### Tablas Involucradas:
- ARC
- REMENT
- CBR
- comex..COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR00101.FRM
**Segmento:** McbrTxt999_Click
**Procedimiento Almacenado:** CMXsrv_icbr_lee_ctp

#### Tablas Involucradas:
- ACMXSUCSAL
- MCBRCTP
- CBR
- ACMXPAIS
- CLN
- CBRANX

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR00101.FRM
**Segmento:** Mcbrtxtrec_Click
**Procedimiento Almacenado:** CMXsrv_icbr_avi1

#### Tablas Involucradas:
- ACMXDESEMB
- ASND
- ACMXBCOBCC
- ARC
- CBR
- ACMXINTERE
- PCX
- ECE
- ACMXMONEDA
- ACMXSUCSAL
- CLN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR00102.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_val_suc

#### Tablas Involucradas:
- ACMXSUCSAL
- tbl_User

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR00102.FRM
**Segmento:** buscar_Click
**Procedimiento Almacenado:** CMXsrv_icbr_busc_cbr

#### Tablas Involucradas:
- ACMXSUCSAL
- ACMXMONEDA
- CLN
- CBR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR00102.FRM
**Segmento:** fld_aux_glo_ofi_LostFocus
**Procedimiento Almacenado:** CMXsrv_val_suc

#### Tablas Involucradas:
- ACMXSUCSAL
- tbl_User

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR00102.FRM
**Segmento:** fld_cbr_cod_gdo_LostFocus
**Procedimiento Almacenado:** CMXsrv_icbr_lee_cln

#### Tablas Involucradas:
- CLN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR00102.FRM
**Segmento:** fld_cbr_cod_ofi_lostfocus
**Procedimiento Almacenado:** CMXsrv_val_suc

#### Tablas Involucradas:
- ACMXSUCSAL
- tbl_User

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR00102.FRM
**Segmento:** proximas_Click
**Procedimiento Almacenado:** CMXsrv_icbr_busc_cbr

#### Tablas Involucradas:
- ACMXSUCSAL
- ACMXMONEDA
- CLN
- CBR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR00103.FRM
**Segmento:** crear_Click
**Procedimiento Almacenado:** CMXsrv_icbr_crea_cbr

#### Tablas Involucradas:
- CLN
- tbl_User

#### Procedimientos Llamados:
- srv_icbr_asig_num
- sp_procxmode
- CMXsrv_util_num_ope

---

### Archivo: CBR00103.FRM
**Segmento:** fld_cbr_cod_gdo_LostFocus
**Procedimiento Almacenado:** CMXsrv_icbr_lee_cln

#### Tablas Involucradas:
- CLN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR00103.FRM
**Segmento:** fld_cbr_cod_ofi_lostfocus
**Procedimiento Almacenado:** CMXsrv_val_suc

#### Tablas Involucradas:
- ACMXSUCSAL
- tbl_User

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR00103.FRM
**Segmento:** INGRESAR_Click
**Procedimiento Almacenado:** CMXsrv_icbr_crea_cbr

#### Tablas Involucradas:
- CLN
- tbl_User

#### Procedimientos Llamados:
- srv_icbr_asig_num
- sp_procxmode
- CMXsrv_util_num_ope

---

### Archivo: CBR00201.FRM
**Segmento:** fld_cbr_cod_gdo_LostFocus
**Procedimiento Almacenado:** CMXsrv_icbr_lee_cln

#### Tablas Involucradas:
- CLN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR00201.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_icbr_lee_cob

#### Tablas Involucradas:
- COB

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR00201.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_icbr_lee_ctp

#### Tablas Involucradas:
- ACMXSUCSAL
- MCBRCTP
- CBR
- ACMXPAIS
- CLN
- CBRANX

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR00201.FRM
**Segmento:** INGRESAR_Click
**Procedimiento Almacenado:** CMXsrv_icbr_act_ctp

#### Tablas Involucradas:
- comex..CBR
- MCBRCTP
- CBRANX
- CBR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR00202.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_icbr_lee_cob

#### Tablas Involucradas:
- COB

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR00202.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_icbr_lee_trm

#### Tablas Involucradas:
- ACMXVIATPT
- CBR
- ACMXINTERE
- ACMXMONEDA
- MCBRTER
- ACMXCLACOM
- ACMXPAIS

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR00202.FRM
**Segmento:** INGRESAR_Click
**Procedimiento Almacenado:** CMXsrv_icbr_act_trm

#### Tablas Involucradas:
- LCB
- COM
- CBR
- MCBRTER
- warnmsg
- CLN

#### Procedimientos Llamados:
- CMXsrv_util_fecha
- CMXsrv_icbr_val_cbr
- sp_procxmode

---

### Archivo: CBR00203.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_icbr_lee_cob

#### Tablas Involucradas:
- COB

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR00203.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_icbr_lee_doc

#### Tablas Involucradas:
- LCB
- MCBRDOC
- MLCB
- CBR
- ACMXMONEDA

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR00203.FRM
**Segmento:** INGRESAR_Click
**Procedimiento Almacenado:** CMXsrv_icbr_act_doc

#### Tablas Involucradas:
- LCB
- MCBRDOC
- MLCB
- CBR
- comex..CBR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR00301.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_icbr_busc_let

#### Tablas Involucradas:
- MLCB
- comex..MLCB
- comex..LCB

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR00302.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_icbr_ingmod_let

#### Tablas Involucradas:
- LCB
- CBR
- comex.dbo

#### Procedimientos Llamados:
- CMXsrv_util_fecha
- sp_procxmode

---

### Archivo: CBR00302.FRM
**Segmento:** eliminar_Click
**Procedimiento Almacenado:** CMXsrv_icbr_eli_let

#### Tablas Involucradas:
- LCB
- MCBRDOC
- MLCB
- CBR
- comex..COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR00302.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_icbr_lee_let

#### Tablas Involucradas:
- ACMXNOTARIO
- LCB
- MLCB

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR00305.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_icbr_prorr

#### Tablas Involucradas:
- comex..CBR
- LCB
- CBR

#### Procedimientos Llamados:
- CMXsrv_util_fecha
- CMXsrv_cnt_2600
- sp_procxmode
- CMXsrv_cnt_2610
- CMXsrv_cnt_2620

---

### Archivo: CBR00401.FRM
**Segmento:** EFECTUAR_Click
**Procedimiento Almacenado:** CMXsrv_icbr_rev_eve

#### Tablas Involucradas:
- APRCBL
- TRSD
- CBR
- vig_trs
- ECE
- DIP
- LIB
- tbl_User

#### Procedimientos Llamados:
- CMXsrv_icbr_rev_mod_cbr
- CMXsrv_mbyte_gen
- CMXsrv_ctl_marc_rev
- CMXsrv_ctl_chq_aprcbl
- CMXsrv_icbr_rev_prot
- CMXsrv_icbr_rev_ent
- CMXsrv_ctl_eli_firma
- CMXsrv_icbr_rev_trfo
- CMXsrv_icbr_rev_vis
- CMXsrv_cnt_rev_vig
- CMXsrv_icbr_rev_acep
- CMXsrv_icbr_rev_inst
- CMXsrv_icbr_rev_trfb
- CMXsrv_rctb_rem
- CMXsrv_icbr_rev_ing
- CMXsrv_icbr_rev_prorr
- CMXsrv_icbr_rev_liq
- sp_procxmode
- CMXsrv_com_rev
- CMXsrv_icbr_rev_pag
- sp_cmx_sii_1870

---

### Archivo: CBR00401.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_icbr_busc_eve

#### Tablas Involucradas:
- ECE

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR00402.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_icbr_lee_eve

#### Tablas Involucradas:
- ECE
- ACMXDESEMB

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR00402.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_icbr_lee_ent_doc

#### Tablas Involucradas:
- CBR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR00701.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_icbr_prot

#### Tablas Involucradas:
- LCB
- CBR

#### Procedimientos Llamados:
- sp_procxmode
- CMXsrv_ctl_crea_apr
- CMXsrv_cnt_950

---

### Archivo: CBR00701.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_icbr_pcg_prot

#### Tablas Involucradas:
- LCB
- CBR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR00801.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_icbr_liq_sdo

#### Tablas Involucradas:
- comex..CBR
- LCB
- CBR

#### Procedimientos Llamados:
- CMXsrv_ctb_liq_sdo
- sp_procxmode
- CMXsrv_cnt_gen_vig

---

### Archivo: CBR00802.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_icbr_act_vis

#### Tablas Involucradas:
- comex..CBR
- CBR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR00802.FRM
**Segmento:** eliminar_Click
**Procedimiento Almacenado:** CMXsrv_icbr_eli_rep

#### Tablas Involucradas:
- REP

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR00802.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_icbr_busc_rep

#### Tablas Involucradas:
- REP

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR00803.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_icbr_imod_rep

#### Tablas Involucradas:
- REP
- CBR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR00804.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_icbr_ent_doc

#### Tablas Involucradas:
- comex..CBR
- LCB
- CBR

#### Procedimientos Llamados:
- CMXsrv_ctl_crea_apr
- sp_procxmode

---

### Archivo: CBR00804.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_icbr_lee_ent_doc

#### Tablas Involucradas:
- CBR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR00901.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_icbr_trf_ofi

#### Tablas Involucradas:
- comex..CBR
- ACMXSUCSAL
- CBR

#### Procedimientos Llamados:
- CMXsrv_ctb_trfo
- sp_procxmode

---

### Archivo: CBR00901.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_val_suc

#### Tablas Involucradas:
- ACMXSUCSAL
- tbl_User

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR00902.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_icbr_trf_bco

#### Tablas Involucradas:
- comex..CBR
- ARC
- CBR
- LCB

#### Procedimientos Llamados:
- CMXsrv_ctb_trfb
- sp_procxmode

---

### Archivo: COBERTU.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_icbr_act_inst

#### Tablas Involucradas:
- comex..CBR
- CBR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: GRL00101.FRM
**Segmento:** enviar_Click
**Procedimiento Almacenado:** CMXsrv_iswf_a_pru

#### Tablas Involucradas:
- switxt
- switxt1

#### Procedimientos Llamados:
- CMXsrv_iswf_a_732
- CMXsrv_iswf_esp_707b
- CMXsrv_iswf_a_747
- CMXsrv_iswf_a_412
- CMXsrv_iswf_a_707b
- CMXsrv_iswf_esp_740
- CMXsrv_iswf_a_410
- CMXsrv_iswf_esp_747
- CMXsrv_iswf_neg_730
- CMXsrv_iswf_neg_752
- CMXsrv_iswf_a_700a
- CMXsrv_iswf_a_707a
- CMXsrv_iswf_esp_700b
- CMXsrv_iswf_a_740
- CMXsrv_iswf_a_700b
- CMXsrv_iswf_esp_707a
- srv_irem_imp_202
- CMXsrv_iswf_747_neg
- srv_irem_imp_100
- sp_procxmode
- CMXsrv_iswf_esp_700a

---

### Archivo: GRL00101.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_icbr_val_cbr

#### Tablas Involucradas:
- DDI
- LCB
- COR
- ADI
- ARC
- ACMXMONEDAFEC
- CBR
- ACMXINTEREFEC
- warnmsg

#### Procedimientos Llamados:
- PrmACMXPAIS
- CMXsrv_icbr_val_arc
- CMXsrv_util_fecha
- sp_procxmode
- PrmACMXMONEDAFEC

---

### Archivo: GRL00101.FRM
**Segmento:** word_Click
**Procedimiento Almacenado:** CMXsrv_icbr_val_cbr

#### Tablas Involucradas:
- DDI
- LCB
- COR
- ADI
- ARC
- ACMXMONEDAFEC
- CBR
- ACMXINTEREFEC
- warnmsg

#### Procedimientos Llamados:
- PrmACMXPAIS
- CMXsrv_icbr_val_arc
- CMXsrv_util_fecha
- sp_procxmode
- PrmACMXMONEDAFEC

---

### Archivo: GRL00101.FRM
**Segmento:** word_Click
**Procedimiento Almacenado:** CMXsrv_iswf_a_pru

#### Tablas Involucradas:
- switxt
- switxt1

#### Procedimientos Llamados:
- CMXsrv_iswf_a_732
- CMXsrv_iswf_esp_707b
- CMXsrv_iswf_a_747
- CMXsrv_iswf_a_412
- CMXsrv_iswf_a_707b
- CMXsrv_iswf_esp_740
- CMXsrv_iswf_a_410
- CMXsrv_iswf_esp_747
- CMXsrv_iswf_neg_730
- CMXsrv_iswf_neg_752
- CMXsrv_iswf_a_700a
- CMXsrv_iswf_a_707a
- CMXsrv_iswf_esp_700b
- CMXsrv_iswf_a_740
- CMXsrv_iswf_a_700b
- CMXsrv_iswf_esp_707a
- srv_irem_imp_202
- CMXsrv_iswf_747_neg
- srv_irem_imp_100
- sp_procxmode
- CMXsrv_iswf_esp_700a

---

## CRDEXT
<a name="crdext"></a>
### Archivo: BCO_BCO.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_icrd_a_ibab

#### Tablas Involucradas:
- MIBAB
- IBAB

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: BCO_BCO.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_icrd_lee_glo_ibab

#### Tablas Involucradas:
- IBAB
- COL
- MIBAB

#### Procedimientos Llamados:
- sp_procxmode
- CMXsrv_icrd_pre_78

---

### Archivo: BCO_REM.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_icrd_a_ibar

#### Tablas Involucradas:
- MIBAR
- IBAR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: BCO_REM.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_icrd_lee_glo_ibar

#### Tablas Involucradas:
- MIBAR
- COL
- IBAR

#### Procedimientos Llamados:
- CMXsrv_icrd_pre_72_740
- sp_procxmode

---

### Archivo: BUSC_COD.FRM
**Segmento:** buscar_click
**Procedimiento Almacenado:** CMXsrv_icrd_lee_tex_swf

#### Tablas Involucradas:
- ACMXTSWFESPMSG
- ACMXTSWFINGMSG

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: BUSC_TXT.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_icrd_lee_cod_txt_swf

#### Tablas Involucradas:
- ACMXTSWFESPMSG
- ACMXTSWFINGMSG

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: BUSC_TXT.FRM
**Segmento:** buscar_click
**Procedimiento Almacenado:** CMXsrv_icrd_lee_txt_swf_all

#### Tablas Involucradas:
- ACMXTSWFESPMSG
- ACMXTSWFINGMSG

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: BUSC_TXT.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_icrd_lee_ind_esp_ing

#### Tablas Involucradas:
- MCTP
- CRD

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: BUSC_TXT.FRM
**Segmento:** llena_arreglo
**Procedimiento Almacenado:** CMXsrv_icrd_lee_tex_swf

#### Tablas Involucradas:
- ACMXTSWFESPMSG
- ACMXTSWFINGMSG

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: BUSC_TXT.FRM
**Segmento:** proximo_Click
**Procedimiento Almacenado:** CMXsrv_icrd_lee_txt_swf_all

#### Tablas Involucradas:
- ACMXTSWFESPMSG
- ACMXTSWFINGMSG

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00207.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_icrd_ing_acu

#### Tablas Involucradas:
- CRD

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00207.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_icrd_lee_acu

#### Tablas Involucradas:
- CRD

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00701.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_icrd_rech_sol

#### Tablas Involucradas:
- CRD
- comex..COL
- OPE_BCI
- COL
- comex..CRD

#### Procedimientos Llamados:
- CMXsrv_nibx_upd_tran
- CMXsrv_ctl_crea_apr
- sp_procxmode
- CMXsrv_nibx_nilive

---

### Archivo: CRD00801.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_icrd_end

#### Tablas Involucradas:
- INF
- ARC
- COL
- CRD

#### Procedimientos Llamados:
- CMXsrv_ctl_crea_apr
- sp_procxmode

---

### Archivo: CRD00801.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_icrd_lee_dat_end

#### Tablas Involucradas:
- CRD

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD02001.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_icrd_asignar_cor

#### Tablas Involucradas:
- COR
- ACMXMONEDAFEC
- CRD
- LCR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD02001.FRM
**Segmento:** buscar_Click
**Procedimiento Almacenado:** CMXsrv_icrd_bus_lcr_bco

#### Tablas Involucradas:
- COR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD02001.FRM
**Segmento:** proximo_Click
**Procedimiento Almacenado:** CMXsrv_icrd_bus_lcr_bco

#### Tablas Involucradas:
- COR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: PREFER.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_grl_fec_serv

#### Tablas Involucradas:

#### Procedimientos Llamados:
- SRV_MessageService
- sp_procxmode

---

## CRD_CORR
<a name="crd_corr"></a>
### Archivo: COR00202.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_icrd_asignar_cor

#### Tablas Involucradas:
- COR
- ACMXMONEDAFEC
- CRD
- LCR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COR00202.FRM
**Segmento:** buscar_Click
**Procedimiento Almacenado:** CMXsrv_icrd_bus_lcr_bco

#### Tablas Involucradas:
- COR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COR00202.FRM
**Segmento:** fld_cor_cod_mtr_LostFocus
**Procedimiento Almacenado:** CMXsrv_icrd_lee_bco_mtr

#### Tablas Involucradas:
- comex..ACMXBANCOS

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COR00202.FRM
**Segmento:** fld_cor_cod_pais_Lostfocus
**Procedimiento Almacenado:** CMXsrv_icrd_cor_lee_pais

#### Tablas Involucradas:
- comex..ACMXPAIS

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COR00202.FRM
**Segmento:** fld_cor_cod_plz_Lostfocus
**Procedimiento Almacenado:** CMXsrv_icrd_lee_plz

#### Tablas Involucradas:
- ACMXPLAZAS

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COR00202.FRM
**Segmento:** proximo_Click
**Procedimiento Almacenado:** CMXsrv_icrd_bus_lcr_bco

#### Tablas Involucradas:
- COR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COR00906.FRM
**Segmento:** buscar_Click
**Procedimiento Almacenado:** CMXsrv_icrd_busc_plz

#### Tablas Involucradas:
- comex..ACMXPLAZAS

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COR00906.FRM
**Segmento:** proximos_Click
**Procedimiento Almacenado:** CMXsrv_icrd_busc_plz

#### Tablas Involucradas:
- comex..ACMXPLAZAS

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COR00907.FRM
**Segmento:** buscar_Click
**Procedimiento Almacenado:** CMXsrv_icrd_cor_busc_pais

#### Tablas Involucradas:
- comex
- comex..ACMXPAIS

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COR00907.FRM
**Segmento:** proximos_Click
**Procedimiento Almacenado:** CMXsrv_icrd_cor_busc_pais

#### Tablas Involucradas:
- comex
- comex..ACMXPAIS

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: GRID_BUS.FRM
**Segmento:** buscar_Click
**Procedimiento Almacenado:** CMXsrv_icrd_busc_bco_mtr

#### Tablas Involucradas:
- comex

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: GRID_BUS.FRM
**Segmento:** proximos_Click
**Procedimiento Almacenado:** CMXsrv_icrd_busc_bco_mtr

#### Tablas Involucradas:
- comex

#### Procedimientos Llamados:
- sp_procxmode

---

## DDI
<a name="ddi"></a>
### Archivo: DDI00101.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_iddi_ingmod_ddi

#### Tablas Involucradas:
- INF
- DDI

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: DDI00101.FRM
**Segmento:** continuar_Click
**Procedimiento Almacenado:** CMXsrv_iddi_lee_dec

#### Tablas Involucradas:
- DDI
- ACMXVIATPT
- ACMXRGMIMP
- INF
- ACMXBCOCEN
- ACMXFPAIMP
- ACMXMONEDA
- ACMXCLACOM
- ACMXPAIS
- CLN

#### Procedimientos Llamados:
- sp_procxmode
- CMXsrv_iddi_val_num_ddi

---

### Archivo: DDI00101.FRM
**Segmento:** eliminar_Click
**Procedimiento Almacenado:** CMXsrv_iddi_eli_ddi

#### Tablas Involucradas:
- DDI

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: DDI00101.FRM
**Segmento:** fld_ddi_fec_ii_lostfocus
**Procedimiento Almacenado:** CMXsrv_iddi_lee_inf

#### Tablas Involucradas:
- INF

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: DDI00101.FRM
**Segmento:** fld_ddi_rut_imp_lostfocus
**Procedimiento Almacenado:** CMXsrv_iddi_lee_cln

#### Tablas Involucradas:
- CLN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: DDI01001.FRM
**Segmento:** Asociar_Click
**Procedimiento Almacenado:** CMXsrv_iddi_lee_rut

#### Tablas Involucradas:
- DDI

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: DDI01001.FRM
**Segmento:** Asociar_Click
**Procedimiento Almacenado:** CMXsrv_iddi_asoc_ddi

#### Tablas Involucradas:
- DDI
- ARC
- ACMXMONEDAFEC
- CBR
- COB
- INF
- ACMXMONEDA
- COL

#### Procedimientos Llamados:
- CMXsrv_cmx_get_codes
- CMXsrv_get_ult_dia_habil
- CMXsrv_util_opr_fec
- sp_procxmode

---

### Archivo: DDI01001.FRM
**Segmento:** Command2_Click
**Procedimiento Almacenado:** CMXsrv_iddi_des_ddi

#### Tablas Involucradas:
- DDI
- ADI
- COB

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: DDI01001.FRM
**Segmento:** Desasociar_Click
**Procedimiento Almacenado:** CMXsrv_iddi_lee_rut

#### Tablas Involucradas:
- DDI

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: DDI01001.FRM
**Segmento:** Desasociar_Click
**Procedimiento Almacenado:** CMXsrv_iddi_des_ddi

#### Tablas Involucradas:
- DDI
- ADI
- COB

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: DDI01001.FRM
**Segmento:** fld_aux_rut_cli_lostfocus
**Procedimiento Almacenado:** CMXsrv_iddi_lee_cln

#### Tablas Involucradas:
- CLN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: DDI01001.FRM
**Segmento:** inicio_asoc
**Procedimiento Almacenado:** CMXsrv_iddi_busc_asoc

#### Tablas Involucradas:
- ADI

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: DDI01001.FRM
**Segmento:** inicio_noasoc
**Procedimiento Almacenado:** CMXsrv_iddi_busc_noasoc

#### Tablas Involucradas:
- DDI
- ADI

#### Procedimientos Llamados:
- CMXsrv_iddi_bus_noasoc_cob
- CMXsrv_iddi_bus_noasoc_opr
- sp_procxmode

---

### Archivo: DDI01001.FRM
**Segmento:** proximo_no_aso_Click
**Procedimiento Almacenado:** CMXsrv_iddi_busc_noasoc

#### Tablas Involucradas:
- DDI
- ADI

#### Procedimientos Llamados:
- CMXsrv_iddi_bus_noasoc_cob
- CMXsrv_iddi_bus_noasoc_opr
- sp_procxmode

---

## IMPORT
<a name="import"></a>
### Archivo: BUSCADIR.FRM
**Segmento:** buscar_Click
**Procedimiento Almacenado:** CMXsrv_icrd_lee_dir_cln

#### Tablas Involucradas:
- DIRCLN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: BUSC_COD.FRM
**Segmento:** buscar_click
**Procedimiento Almacenado:** CMXsrv_icrd_lee_tex_swf

#### Tablas Involucradas:
- ACMXTSWFESPMSG
- ACMXTSWFINGMSG

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: BUSC_TXT.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_icrd_lee_cod_txt_swf

#### Tablas Involucradas:
- ACMXTSWFESPMSG
- ACMXTSWFINGMSG

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: BUSC_TXT.FRM
**Segmento:** buscar_click
**Procedimiento Almacenado:** CMXsrv_icrd_lee_txt_swf_all

#### Tablas Involucradas:
- ACMXTSWFESPMSG
- ACMXTSWFINGMSG

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: BUSC_TXT.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_icrd_lee_ind_esp_ing

#### Tablas Involucradas:
- MCTP
- CRD

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: BUSC_TXT.FRM
**Segmento:** llena_arreglo
**Procedimiento Almacenado:** CMXsrv_icrd_lee_tex_swf

#### Tablas Involucradas:
- ACMXTSWFESPMSG
- ACMXTSWFINGMSG

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: BUSC_TXT.FRM
**Segmento:** proximo_Click
**Procedimiento Almacenado:** CMXsrv_icrd_lee_txt_swf_all

#### Tablas Involucradas:
- ACMXTSWFESPMSG
- ACMXTSWFINGMSG

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CONDESP.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXCRDsrv_icrd_a_cnd_esp

#### Tablas Involucradas:
- CND

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CONDESP.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_icrd_lee_cnd_esp

#### Tablas Involucradas:
- MMCND
- COL
- CND

#### Procedimientos Llamados:
- sp_procxmode
- CMXsrv_icrd_pre_47

---

### Archivo: CRD00101.FRM
**Segmento:** clon_Click
**Procedimiento Almacenado:** CMXCRDsrv_icrd_clon_crd

#### Tablas Involucradas:
- CRS
- MER
- CRD
- TAS
- CRDCLON
- COL_ADI
- CND
- DAC
- ODOC
- AVAL
- COL
- EMB

#### Procedimientos Llamados:
- CMXCRDsrv_icrd_lee_tas_cln
- sp_procxmode
- CMXsrv_fincol_ing_modcol
- CMXsrv_util_num_ope

---

### Archivo: CRD00101.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXCRDsrv_icrd_lee_crdcre

#### Tablas Involucradas:
- CRD_ADI
- ACMXFORPAG
- ACMXPAIS
- ACMXVIATPT
- CRD
- COR
- COL_ADI
- ACMXFINVER
- PMIX
- NEG
- ACMXMONEDA
- tbl_User
- OPE_BCI
- ACMXSUCSAL
- CLN
- COL
- DIRCLN
- EMB

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00101.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_icrd_lee_ind_esp_ing

#### Tablas Involucradas:
- MCTP
- CRD

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00101.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_icrd_lee_top

#### Tablas Involucradas:
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00101.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_grl_fec_serv

#### Tablas Involucradas:

#### Procedimientos Llamados:
- SRV_MessageService
- sp_procxmode

---

### Archivo: CRD00101.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_cmx_get_codes

#### Tablas Involucradas:

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00101.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_trae_glo_fec

#### Tablas Involucradas:
- ACMXSUCSAL
- ACMXDL3475FEC
- tbl_User

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00101.FRM
**Segmento:** Mcrdapr_Click
**Procedimiento Almacenado:** CMXCRDsrv_icrd_val_crd

#### Tablas Involucradas:
- warnmsg

#### Procedimientos Llamados:
- sp_procxmode
- CMXsrv_icrd_val_adv
- CMXsrv_icrd_val_err

---

### Archivo: CRD00101.FRM
**Segmento:** Mcrdeli_click
**Procedimiento Almacenado:** CMXCRDsrv_icrd_eli_crd

#### Tablas Involucradas:
- comex..COL
- OPE_BCI
- CRD

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00101.FRM
**Segmento:** Mcrdtxtliq_Click
**Procedimiento Almacenado:** CMXsrv_icrd_lee_dat_trs

#### Tablas Involucradas:
- ASND
- EVI
- TRSD
- EVE
- ACMXMONEDA
- COL

#### Procedimientos Llamados:
- CMXsrv_icrd_forlin
- sp_procxmode

---

### Archivo: CRD00101.FRM
**Segmento:** Mcrdtxtope_Click
**Procedimiento Almacenado:** CMXsrv_icrd_dat_liq_ope

#### Tablas Involucradas:
- ACMXDESEMB
- ASND
- EVO
- CRD
- CNO
- OBL
- CUO
- TRSD
- NEG
- COM
- EVE
- ACMXTIPEVE
- CAN
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00101.FRM
**Segmento:** msg_swift
**Procedimiento Almacenado:** CMXsrv_iswf_a_pru

#### Tablas Involucradas:
- switxt
- switxt1

#### Procedimientos Llamados:
- CMXsrv_iswf_a_732
- CMXsrv_iswf_esp_707b
- CMXsrv_iswf_a_747
- CMXsrv_iswf_a_412
- CMXsrv_iswf_a_707b
- CMXsrv_iswf_esp_740
- CMXsrv_iswf_a_410
- CMXsrv_iswf_esp_747
- CMXsrv_iswf_neg_730
- CMXsrv_iswf_neg_752
- CMXsrv_iswf_a_700a
- CMXsrv_iswf_a_707a
- CMXsrv_iswf_esp_700b
- CMXsrv_iswf_a_740
- CMXsrv_iswf_a_700b
- CMXsrv_iswf_esp_707a
- srv_irem_imp_202
- CMXsrv_iswf_747_neg
- srv_irem_imp_100
- sp_procxmode
- CMXsrv_iswf_esp_700a

---

### Archivo: CRD00201.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_icrd_a_ctp

#### Tablas Involucradas:
- CRD
- CRDCLON
- MCTP
- comex..COL
- COL

#### Procedimientos Llamados:
- CMXCRDsrv_icrd_lee_tas_cln
- CMXsrv_fincol_imod_colcc
- sp_procxmode

---

### Archivo: CRD00201.FRM
**Segmento:** FLD_COL_COD_CLI_LostFocus
**Procedimiento Almacenado:** CMXsrv_icrd_lee_cln

#### Tablas Involucradas:
- CLN
- DIRCLN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00201.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_lee_fpro

#### Tablas Involucradas:
- ACMXFECPRO

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00202.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_icrd_a_cnd

#### Tablas Involucradas:
- TIP
- CRD_ADI
- CRD
- CRDCLON
- COL_ADI
- COM
- ACMXMONEDA
- LIB
- comex..COL
- MAPR
- MCND
- COL
- ACMXOPEIMP
- comex..CRD

#### Procedimientos Llamados:
- CMXMCRDsrv_icrd_lee_mapr
- CMXsrv_ctb_impto_tim
- CMXsrv_icrd_a_dat_apr
- CMXsrv_imp_calc_aladi
- CMXsrv_ctb_impto_tim2
- CMXsrv_busc_cod_ope
- sp_procxmode
- CMXsrv_ctb_impto_tim3
- CMXsrv_icrd_act_pag_mix
- CMXsrv_util_pesos

---

### Archivo: CRD00202.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXCRDsrv_icrd_crea_crd

#### Tablas Involucradas:
- CRD_ADI
- PMIX
- ACMXMONEDA
- CLN
- COL

#### Procedimientos Llamados:
- CMXsrv_imp_calc_aladi
- CMXsrv_fincol_imod_colcc
- sp_procxmode
- CMXCRDsrv_icrd_lee_tas_cln
- CMXsrv_util_num_ope
- CMXsrv_fincol_ing_modcol

---

### Archivo: CRD00202.FRM
**Segmento:** fld_col_fec_vto_LostFocus
**Procedimiento Almacenado:** CMXsrv_util_det_habil

#### Tablas Involucradas:
- ACMXFERIADO

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00203.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_icrd_busc_emb

#### Tablas Involucradas:
- comex..EMB
- comex..MEMB

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00204.FRM
**Segmento:** ELIMINAR_Click
**Procedimiento Almacenado:** CMXsrv_icrd_eli_emb

#### Tablas Involucradas:
- comex..COL
- EMB
- COL
- CRD

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00204.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_icrd_lee_emb1

#### Tablas Involucradas:
- CRS
- COL
- EMB

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00204.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_icrd_lee_emb2

#### Tablas Involucradas:
- COL
- EMB

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00204.FRM
**Segmento:** ingresar_Click
**Procedimiento Almacenado:** CMXsrv_icrd_a_emb1

#### Tablas Involucradas:
- CRS
- MEMB
- CRD
- MCRS
- CRDCLON
- COL
- EMB

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00204.FRM
**Segmento:** ingresar_Click
**Procedimiento Almacenado:** CMXsrv_icrd_a_emb2

#### Tablas Involucradas:
- EMB
- COL
- MEMB
- CRD

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00204.FRM
**Segmento:** VALIDA_EMBARQUE
**Procedimiento Almacenado:** CMXsrv_icrd_val_emb2

#### Tablas Involucradas:
- warnmsg

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00204.FRM
**Segmento:** VALIDA_EMBARQUE
**Procedimiento Almacenado:** CMXsrv_icrd_val_emb1

#### Tablas Involucradas:
- INF
- ARC
- warnmsg

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00205.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_icrd_act_ref

#### Tablas Involucradas:
- MREF
- CRD
- CRDCLON
- comex..MREF
- comex..COL
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00205.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_icrd_act_ref

#### Tablas Involucradas:
- MREF
- CRD
- CRDCLON
- comex..MREF
- comex..COL
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00205.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_icrd_lee_ref

#### Tablas Involucradas:
- COR
- COL
- CRD

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00301.FRM
**Segmento:** FLD_COL_COD_CLI_LostFocus
**Procedimiento Almacenado:** CMXsrv_icrd_lee_cln

#### Tablas Involucradas:
- CLN
- DIRCLN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD0063.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXCRDsrv_icrd_apr_sol

#### Tablas Involucradas:
- TIP
- CRD
- COL_ADI
- COM
- LIB
- OPE_BCI
- sysobjects
- CLN
- COL

#### Procedimientos Llamados:
- CMXsrv_mbyte_gen
- CMXsrv_icrd_asignar_cor
- CMXsrv_ctb_impto_tim
- CMXsrv_cmx_ing_lib
- CMXsrv_nibx_upd_tran
- CMXsrv_ctb_impto_tim2
- CMXsrv_lee_paridad
- CMXsrv_iswf_a_700
- CMXsrv_fincol_imod_colcc
- sp_procxmode
- CMXsrv_ctb_impto_tim22
- CMXsrv_ctb_impto_tim3
- CMXsrv_icrd_val_crd
- CMXsrv_util_pesos
- CMXsrv_nibx_nilive

---

### Archivo: CRD0063.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_icrd_lee_crdapr

#### Tablas Involucradas:
- CRS
- CRD
- COL_ADI
- DAC
- ACMXAPROBAC

#### Procedimientos Llamados:
- CMXsrv_icrd_pre_72
- sp_procxmode

---

### Archivo: CRD00701.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_icrd_rech_sol

#### Tablas Involucradas:
- CRD
- comex..COL
- OPE_BCI
- COL
- comex..CRD

#### Procedimientos Llamados:
- CMXsrv_nibx_upd_tran
- CMXsrv_ctl_crea_apr
- sp_procxmode
- CMXsrv_nibx_nilive

---

### Archivo: DESCMERC.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXCRDsrv_icrd_a_desc_merc

#### Tablas Involucradas:
- MER

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: DESCMERC.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_icrd_lee_desc_merc

#### Tablas Involucradas:
- MMER
- MER

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: DOCUMENT.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_icrd_a_otr_doc

#### Tablas Involucradas:
- ODOC
- MODOC

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: DOCUMENT.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_icrd_lee_otr_doc

#### Tablas Involucradas:
- ODOC
- MODOC

#### Procedimientos Llamados:
- sp_procxmode
- CMXsrv_icrd_pre_46

---

### Archivo: GRL00101.FRM
**Segmento:** enviar_Click
**Procedimiento Almacenado:** CMXsrv_iswf_a_pru

#### Tablas Involucradas:
- switxt
- switxt1

#### Procedimientos Llamados:
- CMXsrv_iswf_a_732
- CMXsrv_iswf_esp_707b
- CMXsrv_iswf_a_747
- CMXsrv_iswf_a_412
- CMXsrv_iswf_a_707b
- CMXsrv_iswf_esp_740
- CMXsrv_iswf_a_410
- CMXsrv_iswf_esp_747
- CMXsrv_iswf_neg_730
- CMXsrv_iswf_neg_752
- CMXsrv_iswf_a_700a
- CMXsrv_iswf_a_707a
- CMXsrv_iswf_esp_700b
- CMXsrv_iswf_a_740
- CMXsrv_iswf_a_700b
- CMXsrv_iswf_esp_707a
- srv_irem_imp_202
- CMXsrv_iswf_747_neg
- srv_irem_imp_100
- sp_procxmode
- CMXsrv_iswf_esp_700a

---

## INFORME
<a name="informe"></a>
### Archivo: ARC00100.FRM
**Segmento:** Eliminar_Click
**Procedimiento Almacenado:** CMXsrv_iarc_eli_arc

#### Tablas Involucradas:
- ADI
- CRD
- ARC
- NEG
- COB
- INF
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: ARC00100.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_iarc_busc_arc

#### Tablas Involucradas:
- ARC

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: INFO0101.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_iinf_lee0_inf

#### Tablas Involucradas:
- INF

#### Procedimientos Llamados:
- PrmACMXFPAIMP
- PrmACMXMONEDA
- PrmACLNEJECTA
- sp_procxmode

---

### Archivo: INFO0101.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_iinf_lee_tablas

#### Tablas Involucradas:
- ACMXFPAIMP
- ACMXMONEDA
- ACMXCLACOM

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: INFO0101.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_iinf_lee1_inf

#### Tablas Involucradas:
- INF
- CLN

#### Procedimientos Llamados:
- PrmACMXCLACOM
- PrmACMXESPECI
- sp_procxmode
- PrmACLNEJECTA
- PrmACMXETDINF

---

### Archivo: INFO0101.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_iinf_lee_cln

#### Tablas Involucradas:
- CLN

#### Procedimientos Llamados:
- PrmACLNEJECTA
- sp_procxmode

---

### Archivo: INFO0101.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_iinf_lee2_inf

#### Tablas Involucradas:
- INF

#### Procedimientos Llamados:
- PrmACMXPAIS
- PrmACMXORIDVS
- PrmACMXRGMIMP
- sp_procxmode
- PrmACMXBCOBCC
- PrmACMXBCOCEN
- PrmACMXSUCSAL

---

### Archivo: INFO0101.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_iinf_avi_miscb

#### Tablas Involucradas:
- INF

#### Procedimientos Llamados:
- PrmACMXBCOBCC
- sp_procxmode

---

### Archivo: INFO0101.FRM
**Segmento:** Maviapr_Click
**Procedimiento Almacenado:** CMXsrv_iinf_avi_misca

#### Tablas Involucradas:
- INF
- CLN

#### Procedimientos Llamados:
- PrmACMXPAIS
- PrmACMXORIDVS
- PrmACMXRGMIMP
- PrmACMXCLACOM
- sp_procxmode
- PrmACMXFPAIMP
- PrmACLNEJECTA
- PrmACMXSUCSAL
- PrmACMXMONEDA
- PrmACMXETDINF

---

### Archivo: INFO0101.FRM
**Segmento:** Maviapr_Click
**Procedimiento Almacenado:** CMXsrv_iinf_avi_miscb

#### Tablas Involucradas:
- INF

#### Procedimientos Llamados:
- PrmACMXBCOBCC
- sp_procxmode

---

### Archivo: INFO0101.FRM
**Segmento:** Mavicom_Click
**Procedimiento Almacenado:** CMXsrv_iinf_avi_misca

#### Tablas Involucradas:
- INF
- CLN

#### Procedimientos Llamados:
- PrmACMXPAIS
- PrmACMXORIDVS
- PrmACMXRGMIMP
- PrmACMXCLACOM
- sp_procxmode
- PrmACMXFPAIMP
- PrmACLNEJECTA
- PrmACMXSUCSAL
- PrmACMXMONEDA
- PrmACMXETDINF

---

### Archivo: INFO0101.FRM
**Segmento:** Mavicom_Click
**Procedimiento Almacenado:** CMXsrv_iinf_avi_miscb

#### Tablas Involucradas:
- INF

#### Procedimientos Llamados:
- PrmACMXBCOBCC
- sp_procxmode

---

### Archivo: INFO0101.FRM
**Segmento:** Mavicom_Click
**Procedimiento Almacenado:** CMXsrv_icrd_lee_dat_com

#### Tablas Involucradas:
- TIP
- ACMXDESEMB
- ASND
- CRD
- EVI
- COM
- TRSD
- EVE
- ACMXMONEDA

#### Procedimientos Llamados:
- PrmACMXMONEDA
- sp_procxmode

---

### Archivo: INFO0101.FRM
**Segmento:** Mavimis1_Click
**Procedimiento Almacenado:** CMXsrv_iinf_avi_misca

#### Tablas Involucradas:
- INF
- CLN

#### Procedimientos Llamados:
- PrmACMXPAIS
- PrmACMXORIDVS
- PrmACMXRGMIMP
- PrmACMXCLACOM
- sp_procxmode
- PrmACMXFPAIMP
- PrmACLNEJECTA
- PrmACMXSUCSAL
- PrmACMXMONEDA
- PrmACMXETDINF

---

### Archivo: INFO0101.FRM
**Segmento:** Mavimis1_Click
**Procedimiento Almacenado:** CMXsrv_iinf_avi_miscb

#### Tablas Involucradas:
- INF

#### Procedimientos Llamados:
- PrmACMXBCOBCC
- sp_procxmode

---

### Archivo: INFO0101.FRM
**Segmento:** Mavimis2_Click
**Procedimiento Almacenado:** CMXsrv_iinf_avi_misca

#### Tablas Involucradas:
- INF
- CLN

#### Procedimientos Llamados:
- PrmACMXPAIS
- PrmACMXORIDVS
- PrmACMXRGMIMP
- PrmACMXCLACOM
- sp_procxmode
- PrmACMXFPAIMP
- PrmACLNEJECTA
- PrmACMXSUCSAL
- PrmACMXMONEDA
- PrmACMXETDINF

---

### Archivo: INFO0101.FRM
**Segmento:** Mavimis2_Click
**Procedimiento Almacenado:** CMXsrv_iinf_avi_miscb

#### Tablas Involucradas:
- INF

#### Procedimientos Llamados:
- PrmACMXBCOBCC
- sp_procxmode

---

### Archivo: INFO0101.FRM
**Segmento:** Mavirec_Click
**Procedimiento Almacenado:** CMXsrv_iinf_avi_misca

#### Tablas Involucradas:
- INF
- CLN

#### Procedimientos Llamados:
- PrmACMXPAIS
- PrmACMXORIDVS
- PrmACMXRGMIMP
- PrmACMXCLACOM
- sp_procxmode
- PrmACMXFPAIMP
- PrmACLNEJECTA
- PrmACMXSUCSAL
- PrmACMXMONEDA
- PrmACMXETDINF

---

### Archivo: INFO0101.FRM
**Segmento:** Mavirec_Click
**Procedimiento Almacenado:** CMXsrv_iinf_avi_miscb

#### Tablas Involucradas:
- INF

#### Procedimientos Llamados:
- PrmACMXBCOBCC
- sp_procxmode

---

### Archivo: INFO0101.FRM
**Segmento:** Mavitib_Click
**Procedimiento Almacenado:** CMXsrv_iinf_avi_misca

#### Tablas Involucradas:
- INF
- CLN

#### Procedimientos Llamados:
- PrmACMXPAIS
- PrmACMXORIDVS
- PrmACMXRGMIMP
- PrmACMXCLACOM
- sp_procxmode
- PrmACMXFPAIMP
- PrmACLNEJECTA
- PrmACMXSUCSAL
- PrmACMXMONEDA
- PrmACMXETDINF

---

### Archivo: INFO0101.FRM
**Segmento:** Mavitib_Click
**Procedimiento Almacenado:** CMXsrv_iinf_avi_miscb

#### Tablas Involucradas:
- INF

#### Procedimientos Llamados:
- PrmACMXBCOBCC
- sp_procxmode

---

### Archivo: INFO0101.FRM
**Segmento:** Mavitras_Click
**Procedimiento Almacenado:** CMXsrv_iinf_avi_misca

#### Tablas Involucradas:
- INF
- CLN

#### Procedimientos Llamados:
- PrmACMXPAIS
- PrmACMXORIDVS
- PrmACMXRGMIMP
- PrmACMXCLACOM
- sp_procxmode
- PrmACMXFPAIMP
- PrmACLNEJECTA
- PrmACMXSUCSAL
- PrmACMXMONEDA
- PrmACMXETDINF

---

### Archivo: INFO0101.FRM
**Segmento:** Mavitras_Click
**Procedimiento Almacenado:** CMXsrv_iinf_avi_miscb

#### Tablas Involucradas:
- INF

#### Procedimientos Llamados:
- PrmACMXBCOBCC
- sp_procxmode

---

### Archivo: INFO0101.FRM
**Segmento:** Mavitras_Click
**Procedimiento Almacenado:** CMXsrv_icrd_lee_dat_trs

#### Tablas Involucradas:
- ASND
- EVI
- TRSD
- EVE
- ACMXMONEDA
- COL

#### Procedimientos Llamados:
- CMXsrv_icrd_forlin
- sp_procxmode

---

### Archivo: INFO0101.FRM
**Segmento:** Minfoeli_click
**Procedimiento Almacenado:** CMXsrv_iinf_eli_inf

#### Tablas Involucradas:
- INF
- ARC

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: INFO0101.FRM
**Segmento:** Minforev_Click
**Procedimiento Almacenado:** CMXsrv_iinf_busc_evi

#### Tablas Involucradas:
- EVI

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: INFO0101.FRM
**Segmento:** Minfoval_click
**Procedimiento Almacenado:** CMXsrv_iinf_val_inf

#### Tablas Involucradas:
- INF
- ACMXPAIS
- warnmsg

#### Procedimientos Llamados:
- CMXsrv_cmx_get_codes
- PrmACMXPAIS
- PrmACMXCLACOM
- sp_procxmode

---

### Archivo: INFO0102.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_iinf_ingmod_inf

#### Tablas Involucradas:
- INF
- tbl_User
- warnmsg

#### Procedimientos Llamados:
- CMXsrv_util_fecha
- sp_procxmode
- PrmACMXMONEDAFEC
- CMXsrv_cmx_get_codes
- CMXsrv_iinf_val_inf
- CMXsrv_iinf_get_num

---

### Archivo: INFO0102.FRM
**Segmento:** Fec_pre
**Procedimiento Almacenado:** CMXsrv_iinf_lee_fec

#### Tablas Involucradas:

#### Procedimientos Llamados:
- CMXsrv_util_fecha
- sp_procxmode

---

### Archivo: INFO0102.FRM
**Segmento:** fld_aux_glo_cls_com_LostFocus
**Procedimiento Almacenado:** CMXsrv_iinf_lee_tablas

#### Tablas Involucradas:
- ACMXFPAIMP
- ACMXMONEDA
- ACMXCLACOM

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: INFO0102.FRM
**Segmento:** fld_aux_glo_for_pag1_LostFocus
**Procedimiento Almacenado:** CMXsrv_iinf_lee_tablas

#### Tablas Involucradas:
- ACMXFPAIMP
- ACMXMONEDA
- ACMXCLACOM

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: INFO0102.FRM
**Segmento:** fld_aux_glo_for_pag2_LostFocus
**Procedimiento Almacenado:** CMXsrv_iinf_lee_tablas

#### Tablas Involucradas:
- ACMXFPAIMP
- ACMXMONEDA
- ACMXCLACOM

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: INFO0102.FRM
**Segmento:** fld_aux_glo_for_pag3_LostFocus
**Procedimiento Almacenado:** CMXsrv_iinf_lee_tablas

#### Tablas Involucradas:
- ACMXFPAIMP
- ACMXMONEDA
- ACMXCLACOM

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: INFO0102.FRM
**Segmento:** fld_aux_glo_mon_LostFocus
**Procedimiento Almacenado:** CMXsrv_iinf_lee_tablas

#### Tablas Involucradas:
- ACMXFPAIMP
- ACMXMONEDA
- ACMXCLACOM

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: INFO0102.FRM
**Segmento:** fld_inf_cls_com_Lostfocus
**Procedimiento Almacenado:** CMXsrv_iinf_lee_tablas

#### Tablas Involucradas:
- ACMXFPAIMP
- ACMXMONEDA
- ACMXCLACOM

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: INFO0102.FRM
**Segmento:** fld_inf_cod_imp_LostFocus
**Procedimiento Almacenado:** CMXsrv_iinf_lee_cln

#### Tablas Involucradas:
- CLN

#### Procedimientos Llamados:
- PrmACLNEJECTA
- sp_procxmode

---

### Archivo: INFO0102.FRM
**Segmento:** fld_inf_for_pag1_lostfocus
**Procedimiento Almacenado:** CMXsrv_iinf_lee_tablas

#### Tablas Involucradas:
- ACMXFPAIMP
- ACMXMONEDA
- ACMXCLACOM

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: INFO0102.FRM
**Segmento:** fld_inf_for_pag2_LostFocus
**Procedimiento Almacenado:** CMXsrv_iinf_lee_tablas

#### Tablas Involucradas:
- ACMXFPAIMP
- ACMXMONEDA
- ACMXCLACOM

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: INFO0102.FRM
**Segmento:** fld_inf_for_pag3_LostFocus
**Procedimiento Almacenado:** CMXsrv_iinf_lee_tablas

#### Tablas Involucradas:
- ACMXFPAIMP
- ACMXMONEDA
- ACMXCLACOM

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: INFO0102.FRM
**Segmento:** fld_inf_mon_inf_lostfocus
**Procedimiento Almacenado:** CMXsrv_iinf_lee_tablas

#### Tablas Involucradas:
- ACMXFPAIMP
- ACMXMONEDA
- ACMXCLACOM

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: INFO0102.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_iinf_lee0_inf

#### Tablas Involucradas:
- INF

#### Procedimientos Llamados:
- PrmACMXFPAIMP
- PrmACMXMONEDA
- PrmACLNEJECTA
- sp_procxmode

---

### Archivo: INFO0102.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_iinf_lee1_inf

#### Tablas Involucradas:
- INF
- CLN

#### Procedimientos Llamados:
- PrmACMXCLACOM
- PrmACMXESPECI
- sp_procxmode
- PrmACLNEJECTA
- PrmACMXETDINF

---

### Archivo: INFO0102.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_iinf_lee2_inf

#### Tablas Involucradas:
- INF

#### Procedimientos Llamados:
- PrmACMXPAIS
- PrmACMXORIDVS
- PrmACMXRGMIMP
- sp_procxmode
- PrmACMXBCOBCC
- PrmACMXBCOCEN
- PrmACMXSUCSAL

---

### Archivo: INFO0102.FRM
**Segmento:** valor_usd
**Procedimiento Almacenado:** CMXsrv_iinf_lee_usd

#### Tablas Involucradas:

#### Procedimientos Llamados:
- CMXsrv_cmx_get_codes
- PrmACMXMONEDAFEC
- sp_procxmode

---

### Archivo: INFO0103.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_iinf_busc_inf

#### Tablas Involucradas:
- INF

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: INFO0103.FRM
**Segmento:** buscar_Click
**Procedimiento Almacenado:** CMXsrv_iinf_busc_inf

#### Tablas Involucradas:
- INF

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: INFO0103.FRM
**Segmento:** Fec_pre
**Procedimiento Almacenado:** CMXsrv_iinf_lee_fec

#### Tablas Involucradas:

#### Procedimientos Llamados:
- CMXsrv_util_fecha
- sp_procxmode

---

### Archivo: INFO0103.FRM
**Segmento:** fld_inf_cod_imp_LostFocus
**Procedimiento Almacenado:** CMXsrv_iinf_lee_cln

#### Tablas Involucradas:
- CLN

#### Procedimientos Llamados:
- PrmACLNEJECTA
- sp_procxmode

---

### Archivo: INFO0103.FRM
**Segmento:** PROXIMA_Click
**Procedimiento Almacenado:** CMXsrv_iinf_busc_inf

#### Tablas Involucradas:
- INF

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: INFO0104.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_iinf_act_apr

#### Tablas Involucradas:
- INF

#### Procedimientos Llamados:
- CMXsrv_iinf_val_inf
- CMXsrv_util_fecha
- sp_procxmode

---

### Archivo: INFO0105.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_iinf_busc_evi

#### Tablas Involucradas:
- EVI

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: INFO0105.FRM
**Segmento:** reversar_Click
**Procedimiento Almacenado:** CMXsrv_iinf_rev_evi

#### Tablas Involucradas:
- INF
- ARC
- INC
- EVI

#### Procedimientos Llamados:
- CMXsrv_com_rev
- sp_procxmode

---

### Archivo: INFO0106.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_iinf_lee_evi

#### Tablas Involucradas:
- EVI

#### Procedimientos Llamados:
- PrmACMXSUCSAL
- PrmACMXBCOCEN
- sp_procxmode
- PrmACMXETDINF

---

### Archivo: INFO0107.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_iinf_act_tib

#### Tablas Involucradas:
- INF

#### Procedimientos Llamados:
- CMXsrv_cmx_get_codes
- sp_procxmode

---

### Archivo: INFO0108.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_iinf_act_rec

#### Tablas Involucradas:
- INF

#### Procedimientos Llamados:
- CMXsrv_util_fecha
- sp_procxmode

---

### Archivo: INFO0109.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_iinf_act_rib

#### Tablas Involucradas:
- INF

#### Procedimientos Llamados:
- CMXsrv_cmx_get_codes
- sp_procxmode

---

### Archivo: INFO0110.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_iinf_busc_comp

#### Tablas Involucradas:
- INF

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: INFO0110.FRM
**Segmento:** proximos_Click
**Procedimiento Almacenado:** CMXsrv_iinf_busc_comp

#### Tablas Involucradas:
- INF

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: INFO0111.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_iinf_ingmod_comp

#### Tablas Involucradas:
- INF
- warnmsg

#### Procedimientos Llamados:
- CMXsrv_util_fecha
- sp_procxmode
- PrmACMXMONEDAFEC
- CMXsrv_cmx_get_codes
- CMXsrv_iinf_val_inf
- CMXsrv_iinf_get_num

---

### Archivo: INFO0111.FRM
**Segmento:** Fec_pre
**Procedimiento Almacenado:** CMXsrv_iinf_lee_fec

#### Tablas Involucradas:

#### Procedimientos Llamados:
- CMXsrv_util_fecha
- sp_procxmode

---

### Archivo: INFO0111.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_iinf_lee_comp

#### Tablas Involucradas:
- INF

#### Procedimientos Llamados:
- PrmACMXPAIS
- PrmACMXORIDVS
- PrmACMXRGMIMP
- PrmACMXCLACOM
- sp_procxmode
- PrmACMXFPAIMP
- PrmACMXVIATPT
- PrmACMXMONEDA

---

### Archivo: INFO0111.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_iinf_lee_tablas

#### Tablas Involucradas:
- ACMXFPAIMP
- ACMXMONEDA
- ACMXCLACOM

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: INFO0112.FRM
**Segmento:** aceptar_click
**Procedimiento Almacenado:** CMXsrv_iinf_lee_bco

#### Tablas Involucradas:
- COR

#### Procedimientos Llamados:
- PrmACMXPAIS
- sp_procxmode

---

### Archivo: INFO0112.FRM
**Segmento:** buscar_Click
**Procedimiento Almacenado:** CMXsrv_iinf_busc_bco

#### Tablas Involucradas:
- ACMXBCOBCC

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: PREFER.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_grl_fec_serv

#### Tablas Involucradas:

#### Procedimientos Llamados:
- SRV_MessageService
- sp_procxmode

---

## MOD_ADI
<a name="mod_adi"></a>
### Archivo: CRD00202.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_icrd_a_cnd

#### Tablas Involucradas:
- TIP
- CRD_ADI
- CRD
- CRDCLON
- COL_ADI
- COM
- ACMXMONEDA
- LIB
- comex..COL
- MAPR
- MCND
- COL
- ACMXOPEIMP
- comex..CRD

#### Procedimientos Llamados:
- CMXMCRDsrv_icrd_lee_mapr
- CMXsrv_ctb_impto_tim
- CMXsrv_icrd_a_dat_apr
- CMXsrv_imp_calc_aladi
- CMXsrv_ctb_impto_tim2
- CMXsrv_busc_cod_ope
- sp_procxmode
- CMXsrv_ctb_impto_tim3
- CMXsrv_icrd_act_pag_mix
- CMXsrv_util_pesos

---

### Archivo: CRD00202.FRM
**Segmento:** busca_bco
**Procedimiento Almacenado:** CMXsrv_icrd_lee_bco_swf

#### Tablas Involucradas:
- ACMXPAIS
- COR

#### Procedimientos Llamados:
- CMXsrv_icrd_lee_cln
- sp_procxmode

---

### Archivo: CRD00202.FRM
**Segmento:** fld_col_fec_vto_LostFocus
**Procedimiento Almacenado:** CMXsrv_util_det_habil

#### Tablas Involucradas:
- ACMXFERIADO

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00202.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXMCRDsrv_icrd_lee_mcnd

#### Tablas Involucradas:
- CRD_ADI
- ACMXFORPAG
- CRD
- PMIX
- ACMXMONEDA
- MPMIX
- MCND

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: PREFER.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_grl_fec_serv

#### Tablas Involucradas:

#### Procedimientos Llamados:
- SRV_MessageService
- sp_procxmode

---

## MOD_CBR
<a name="mod_cbr"></a>
### Archivo: CBR00201.FRM
**Segmento:** fld_cbr_cod_gdo_LostFocus
**Procedimiento Almacenado:** CMXsrv_icbr_lee_cln

#### Tablas Involucradas:
- CLN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR00201.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_icbr_lee_ctp

#### Tablas Involucradas:
- ACMXSUCSAL
- MCBRCTP
- CBR
- ACMXPAIS
- CLN
- CBRANX

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR00201.FRM
**Segmento:** INGRESAR_Click
**Procedimiento Almacenado:** CMXsrv_icbr_act_ctp

#### Tablas Involucradas:
- comex..CBR
- MCBRCTP
- CBRANX
- CBR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR00202.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_icbr_lee_trm

#### Tablas Involucradas:
- ACMXVIATPT
- CBR
- ACMXINTERE
- ACMXMONEDA
- MCBRTER
- ACMXCLACOM
- ACMXPAIS

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR00202.FRM
**Segmento:** INGRESAR_Click
**Procedimiento Almacenado:** CMXsrv_icbr_act_trm

#### Tablas Involucradas:
- LCB
- COM
- CBR
- MCBRTER
- warnmsg
- CLN

#### Procedimientos Llamados:
- CMXsrv_util_fecha
- CMXsrv_icbr_val_cbr
- sp_procxmode

---

### Archivo: CBR00203.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_icbr_lee_doc

#### Tablas Involucradas:
- LCB
- MCBRDOC
- MLCB
- CBR
- ACMXMONEDA

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR00203.FRM
**Segmento:** INGRESAR_Click
**Procedimiento Almacenado:** CMXsrv_icbr_act_doc

#### Tablas Involucradas:
- LCB
- MCBRDOC
- MLCB
- CBR
- comex..CBR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR00301.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_icbr_busc_let

#### Tablas Involucradas:
- MLCB
- comex..MLCB
- comex..LCB

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR00302.FRM
**Segmento:** aceptar_Click
**Procedimiento Almacenado:** CMXsrv_icbr_mod_ing_let

#### Tablas Involucradas:
- LCB
- MLCB
- CBR
- end

#### Procedimientos Llamados:
- CMXsrv_util_opr_fec
- sp_procxmode

---

### Archivo: CBR00302.FRM
**Segmento:** eliminar_Click
**Procedimiento Almacenado:** CMXsrv_icbr_eli_let

#### Tablas Involucradas:
- LCB
- MCBRDOC
- MLCB
- CBR
- comex..COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR00302.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_icbr_lee_let

#### Tablas Involucradas:
- ACMXNOTARIO
- LCB
- MLCB

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: PANBASE.FRM
**Segmento:** actualizar_Click
**Procedimiento Almacenado:** CMXsrv_icbr_acep_mod_cbr

#### Tablas Involucradas:
- LCB
- MCBRDOC
- MCBRCTP
- MLCB
- CBR
- MCBRTER
- warnmsg

#### Procedimientos Llamados:
- CMXsrv_cnt_2800
- CMXsrv_icbr_cheq_mdoc
- CMXsrv_icbr_val_cbr
- CMXsrv_icbr_cheq_mctp
- CMXsrv_icbr_cheq_mter
- sp_procxmode
- CMXsrv_icbr_cheq_mlcb

---

### Archivo: PANBASE.FRM
**Segmento:** Cancelar_Click
**Procedimiento Almacenado:** CMXsrv_icbr_eli_no_cont

#### Tablas Involucradas:
- MCBRDOC
- MCBRCTP
- MLCB
- CBR
- MCBRTER

#### Procedimientos Llamados:
- sp_procxmode

---

## MOD_CRD
<a name="mod_crd"></a>
### Archivo: BCO_BCO.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_icrd_a_ibab

#### Tablas Involucradas:
- MIBAB
- IBAB

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: BCO_BCO.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_icrd_lee_glo_ibab

#### Tablas Involucradas:
- IBAB
- COL
- MIBAB

#### Procedimientos Llamados:
- sp_procxmode
- CMXsrv_icrd_pre_78

---

### Archivo: BCO_REM.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_icrd_a_ibar

#### Tablas Involucradas:
- MIBAR
- IBAR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: BCO_REM.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_icrd_lee_glo_ibar

#### Tablas Involucradas:
- MIBAR
- COL
- IBAR

#### Procedimientos Llamados:
- CMXsrv_icrd_pre_72_740
- sp_procxmode

---

### Archivo: BUSCADIR.FRM
**Segmento:** buscar_click
**Procedimiento Almacenado:** CMXsrv_icrd_lee_dir_cln

#### Tablas Involucradas:
- DIRCLN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: BUSCA_TE.FRM
**Segmento:** buscar_Click
**Procedimiento Almacenado:** CMXsrv_icrd_lee_tex_swf

#### Tablas Involucradas:
- ACMXTSWFESPMSG
- ACMXTSWFINGMSG

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: BUSC_COD.FRM
**Segmento:** buscar_click
**Procedimiento Almacenado:** CMXsrv_icrd_lee_tex_swf

#### Tablas Involucradas:
- ACMXTSWFESPMSG
- ACMXTSWFINGMSG

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: BUSC_TXT.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_icrd_lee_cod_txt_swf

#### Tablas Involucradas:
- ACMXTSWFESPMSG
- ACMXTSWFINGMSG

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: BUSC_TXT.FRM
**Segmento:** buscar_click
**Procedimiento Almacenado:** CMXsrv_icrd_lee_txt_swf_all

#### Tablas Involucradas:
- ACMXTSWFESPMSG
- ACMXTSWFINGMSG

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: BUSC_TXT.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_icrd_lee_ind_esp_ing

#### Tablas Involucradas:
- MCTP
- CRD

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: BUSC_TXT.FRM
**Segmento:** llena_arreglo
**Procedimiento Almacenado:** CMXsrv_icrd_lee_tex_swf

#### Tablas Involucradas:
- ACMXTSWFESPMSG
- ACMXTSWFINGMSG

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: BUSC_TXT.FRM
**Segmento:** proximo_Click
**Procedimiento Almacenado:** CMXsrv_icrd_lee_txt_swf_all

#### Tablas Involucradas:
- ACMXTSWFESPMSG
- ACMXTSWFINGMSG

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CONDESP.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXMCRDsrv_icrd_a_mmcnd

#### Tablas Involucradas:
- MMCND

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CONDESP.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_icrd_lee_cnd_esp

#### Tablas Involucradas:
- MMCND
- COL
- CND

#### Procedimientos Llamados:
- sp_procxmode
- CMXsrv_icrd_pre_47

---

### Archivo: CRD00201.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_icrd_a_ctp

#### Tablas Involucradas:
- CRD
- CRDCLON
- MCTP
- comex..COL
- COL

#### Procedimientos Llamados:
- CMXCRDsrv_icrd_lee_tas_cln
- CMXsrv_fincol_imod_colcc
- sp_procxmode

---

### Archivo: CRD00201.FRM
**Segmento:** FLD_COL_COD_CLI_LostFocus
**Procedimiento Almacenado:** CMXsrv_icrd_lee_cln

#### Tablas Involucradas:
- CLN
- DIRCLN

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00201.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXMCRDsrv_icrd_lee_mctp

#### Tablas Involucradas:
- ACMXPAIS
- MCTP
- DIRCLN
- CRD

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00202.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_icrd_a_cnd

#### Tablas Involucradas:
- TIP
- CRD_ADI
- CRD
- CRDCLON
- COL_ADI
- COM
- ACMXMONEDA
- LIB
- comex..COL
- MAPR
- MCND
- COL
- ACMXOPEIMP
- comex..CRD

#### Procedimientos Llamados:
- CMXMCRDsrv_icrd_lee_mapr
- CMXsrv_ctb_impto_tim
- CMXsrv_icrd_a_dat_apr
- CMXsrv_imp_calc_aladi
- CMXsrv_ctb_impto_tim2
- CMXsrv_busc_cod_ope
- sp_procxmode
- CMXsrv_ctb_impto_tim3
- CMXsrv_icrd_act_pag_mix
- CMXsrv_util_pesos

---

### Archivo: CRD00202.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXMCRDsrv_icrd_lee_mcnd

#### Tablas Involucradas:
- CRD_ADI
- ACMXFORPAG
- CRD
- PMIX
- ACMXMONEDA
- MPMIX
- MCND

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00203.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_icrd_busc_emb

#### Tablas Involucradas:
- comex..EMB
- comex..MEMB

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00204.FRM
**Segmento:** cancelar_Click
**Procedimiento Almacenado:** CMXsrv_icrd_lee_desc_merc

#### Tablas Involucradas:
- MMER
- MER

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00204.FRM
**Segmento:** ELIMINAR_Click
**Procedimiento Almacenado:** CMXsrv_icrd_eli_emb

#### Tablas Involucradas:
- comex..COL
- EMB
- COL
- CRD

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00204.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXMCRDsrv_icrd_lee_memb2

#### Tablas Involucradas:
- MEMB
- EMB

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00204.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXMCRDsrv_icrd_lee_memb1

#### Tablas Involucradas:
- CRS
- MEMB
- EMB
- MCRS

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00204.FRM
**Segmento:** ingresar_Click
**Procedimiento Almacenado:** CMXsrv_icrd_a_emb1

#### Tablas Involucradas:
- CRS
- MEMB
- CRD
- MCRS
- CRDCLON
- COL
- EMB

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00204.FRM
**Segmento:** ingresar_Click
**Procedimiento Almacenado:** CMXsrv_icrd_a_emb2

#### Tablas Involucradas:
- EMB
- COL
- MEMB
- CRD

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00204.FRM
**Segmento:** VALIDA_EMBARQUE
**Procedimiento Almacenado:** CMXsrv_icrd_val_emb2

#### Tablas Involucradas:
- warnmsg

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00204.FRM
**Segmento:** VALIDA_EMBARQUE
**Procedimiento Almacenado:** CMXsrv_icrd_val_emb1

#### Tablas Involucradas:
- INF
- ARC
- warnmsg

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00205.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_icrd_act_ref

#### Tablas Involucradas:
- MREF
- CRD
- CRDCLON
- comex..MREF
- comex..COL
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00205.FRM
**Segmento:** fld_obl_cod_bco_acre_DblClick
**Procedimiento Almacenado:** CMXsrv_icrd_lee_bco_swf

#### Tablas Involucradas:
- ACMXPAIS
- COR

#### Procedimientos Llamados:
- CMXsrv_icrd_lee_cln
- sp_procxmode

---

### Archivo: CRD00205.FRM
**Segmento:** fld_obl_cod_bco_acre_LostFocus
**Procedimiento Almacenado:** CMXsrv_icrd_lee_bco_swf

#### Tablas Involucradas:
- ACMXPAIS
- COR

#### Procedimientos Llamados:
- CMXsrv_icrd_lee_cln
- sp_procxmode

---

### Archivo: CRD00205.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXMCRDsrv_icrd_lee_mref

#### Tablas Involucradas:
- MREF
- COR
- COL
- CRD

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00206.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_icrd_ing_txt

#### Tablas Involucradas:
- MTXT

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00206.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXCRDsrv_icrd_get_ing_esp

#### Tablas Involucradas:
- ACMXPAIS
- MCTP
- CRD

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00206.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXMCRDsrv_icrd_lee_mtxt

#### Tablas Involucradas:
- MTXT

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00207.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXCRDsrv_icrd_get_pre_fra

#### Tablas Involucradas:
- ACMXTSWFESPMSG
- ACMXTSWFINGMSG

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: DESCMERC.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXMCRDsrv_icrd_a_mmer

#### Tablas Involucradas:
- MMER

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: DESCMERC.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_icrd_lee_desc_merc

#### Tablas Involucradas:
- MMER
- MER

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: DOCUME.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_icrd_a_otr_doc

#### Tablas Involucradas:
- ODOC
- MODOC

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: DOCUME.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_icrd_lee_otr_doc

#### Tablas Involucradas:
- ODOC
- MODOC

#### Procedimientos Llamados:
- sp_procxmode
- CMXsrv_icrd_pre_46

---

### Archivo: MOD00603.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_fincol_lee_cod_eve

#### Tablas Involucradas:
- MCND
- COL
- CRD
- COM

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: MOD00603.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXMCRDsrv_icrd_acep_mod_crd

#### Tablas Involucradas:
- de
- TIP
- CRD
- COD
- MCRS
- OBL
- EVE
- LIB
- warnmsg
- OPE_BCI
- sysobjects
- COL

#### Procedimientos Llamados:
- CMXsrv_icrd_cheq_modoc
- CMXCRDsrv_icrd_val_crd
- CMXsrv_icrd_cheq_memb
- CMXsrv_nibx_upd_tran
- CMXsrv_expcce_anl_cce
- CMXsrv_fincol_ctb_mod
- CMXsrv_icrd_cheq_mtxt
- CMXsrv_icrd_cheq_mcnd
- CMXsrv_icrd_cheq_mmer
- CMXsrv_icrd_cheq_mref
- CMXsrv_nibx_nilive
- CMXsrv_icrd_cheq_mpmix
- CMXsrv_ctl_crea_apr
- CMXsrv_icrd_cheq_mibar
- CMXMCRDsrv_icrd_eli_no_cont
- CMXsrv_icrd_lee_tip_ope
- CMXsrv_icrd_cheq_mmcnd
- CMXsrv_icrd_cheq_mibab
- sp_procxmode
- CMXsrv_icrd_cheq_mctp
- CMXsrv_icrd_cheq_mapr
- CMXsrv_cnt_950

---

### Archivo: MOD00603.FRM
**Segmento:** cancelar_Click
**Procedimiento Almacenado:** CMXMCRDsrv_icrd_eli_no_cont

#### Tablas Involucradas:
- MREF
- MEMB
- MCRS
- MMCND
- COM
- MODOC
- MIBAB
- CRD_AMD
- MPMIX
- MCTP
- MMER
- MCND
- MIBAR
- TNIH
- MAPR
- FE_IN_REJECTED_TRANS
- MTXT

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: MOD00603.FRM
**Segmento:** fld_crd_cod_bco_rem_LostFocus
**Procedimiento Almacenado:** CMXsrv_icrd_lee_bco_swf

#### Tablas Involucradas:
- ACMXPAIS
- COR

#### Procedimientos Llamados:
- CMXsrv_icrd_lee_cln
- sp_procxmode

---

### Archivo: MOD00603.FRM
**Segmento:** fld_crd_fec_mod_lostFocus
**Procedimiento Almacenado:** CMXsrv_fincol_efec_calpa

#### Tablas Involucradas:
- TF_PPAG
- TIP
- TAS
- CUO
- comex..ACMXMONEDA
- COL_ADI
- OBL
- CTR
- NEG_ADI
- ACMXINTERE
- CAN
- ICR
- COL

#### Procedimientos Llamados:
- CMXsrv_fincol_eval_tnem
- CMXsrv_fincol_eval_tmor
- CMXsrv_util_det_habil
- sp_procxmode
- CMXsrv_fincol_calc_reba
- CMXsrv_fincol_eval_tasa
- CMXsrv_fincol_eval_tneg
- CMXsrv_fincol_efcal_cv
- CMXsrv_fincol_cal_tas_sfr

---

### Archivo: MOD00603.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_icrd_lee_ind_esp_ing

#### Tablas Involucradas:
- MCTP
- CRD

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: MOD00603.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_fincol_efec_calpa

#### Tablas Involucradas:
- TF_PPAG
- TIP
- TAS
- CUO
- comex..ACMXMONEDA
- COL_ADI
- OBL
- CTR
- NEG_ADI
- ACMXINTERE
- CAN
- ICR
- COL

#### Procedimientos Llamados:
- CMXsrv_fincol_eval_tnem
- CMXsrv_fincol_eval_tmor
- CMXsrv_util_det_habil
- sp_procxmode
- CMXsrv_fincol_calc_reba
- CMXsrv_fincol_eval_tasa
- CMXsrv_fincol_eval_tneg
- CMXsrv_fincol_efcal_cv
- CMXsrv_fincol_cal_tas_sfr

---

### Archivo: MOD00603.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXMCRDsrv_icrd_lee_mcnd

#### Tablas Involucradas:
- CRD_ADI
- ACMXFORPAG
- CRD
- PMIX
- ACMXMONEDA
- MPMIX
- MCND

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: PREFER.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_grl_fec_serv

#### Tablas Involucradas:

#### Procedimientos Llamados:
- SRV_MessageService
- sp_procxmode

---

## NEGO_AV
<a name="nego_av"></a>
### Archivo: AVISOS.FRM
**Segmento:** aviso1
**Procedimiento Almacenado:** CMXsrv_icrd_a_rec_age

#### Tablas Involucradas:
- COR
- TAS
- CRD
- CUO
- CNEG
- COM
- NEG
- TRSD
- DIS
- EVE
- ACMXMONEDA
- ACMXINTERE
- ACMXSUCSAL
- COL

#### Procedimientos Llamados:
- CMXsrv_util_fecha
- sp_procxmode

---

### Archivo: AVISOS.FRM
**Segmento:** aviso1
**Procedimiento Almacenado:** CMXsrv_busc_ofi_cta

#### Tablas Involucradas:
- CLN

#### Procedimientos Llamados:
- PrmACMXESPECI
- PrmACLNEJECTA
- sp_procxmode

---

### Archivo: AVISOS.FRM
**Segmento:** aviso1
**Procedimiento Almacenado:** CMXsrv_neg_busc_arc

#### Tablas Involucradas:
- ARC

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: AVISOS.FRM
**Segmento:** aviso1
**Procedimiento Almacenado:** CMXsrv_icrd_lee_avi_adi

#### Tablas Involucradas:
- CRD

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: AVISOS.FRM
**Segmento:** aviso3
**Procedimiento Almacenado:** CMXsrv_icrd_lee_dat_trs

#### Tablas Involucradas:
- ASND
- EVI
- TRSD
- EVE
- ACMXMONEDA
- COL

#### Procedimientos Llamados:
- CMXsrv_icrd_forlin
- sp_procxmode

---

### Archivo: AVISOS.FRM
**Segmento:** Aviso4
**Procedimiento Almacenado:** CMXsrv_icrd_dat_liq_ope

#### Tablas Involucradas:
- ACMXDESEMB
- ASND
- EVO
- CRD
- CNO
- OBL
- CUO
- TRSD
- NEG
- COM
- EVE
- ACMXTIPEVE
- CAN
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: AVISOS.FRM
**Segmento:** Aviso4
**Procedimiento Almacenado:** CMXsrv_icrd_lee_dat_cln

#### Tablas Involucradas:
- NEG
- CLN
- COL

#### Procedimientos Llamados:
- CMXsrv_trae_glo_fec
- sp_procxmode

---

### Archivo: AVISOS.FRM
**Segmento:** Aviso5
**Procedimiento Almacenado:** CMXsrv_icrd_lee_dat_cln

#### Tablas Involucradas:
- NEG
- CLN
- COL

#### Procedimientos Llamados:
- CMXsrv_trae_glo_fec
- sp_procxmode

---

### Archivo: AVISOS.FRM
**Segmento:** Aviso5
**Procedimiento Almacenado:** CMXsrv_icrd_lee_avi_dis

#### Tablas Involucradas:
- DIS
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: AVISOS.FRM
**Segmento:** Aviso5
**Procedimiento Almacenado:** CMXsrv_icrd_lee_avi_adi

#### Tablas Involucradas:
- CRD

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: AVISOS.FRM
**Segmento:** Aviso5
**Procedimiento Almacenado:** CMXsrv_neg_ddi_asoc

#### Tablas Involucradas:
- ADI

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: AVISOS.FRM
**Segmento:** Aviso5
**Procedimiento Almacenado:** CMXsrv_neg_busc_arc

#### Tablas Involucradas:
- ARC

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: AVISOS.FRM
**Segmento:** Aviso5
**Procedimiento Almacenado:** CMXsrv_neg_trae_vcto_mcf

#### Tablas Involucradas:
- COL
- CUO

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: AVISOS.FRM
**Segmento:** lee_aval
**Procedimiento Almacenado:** CMXsrv_neg_avi_lee_aval

#### Tablas Involucradas:
- TAS
- CNEG
- AVAL
- CLN
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: AVISOS.FRM
**Segmento:** lee_nego
**Procedimiento Almacenado:** CMXsrv_icrd_neg_lee_crd

#### Tablas Involucradas:
- NEG
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: AVISOS.FRM
**Segmento:** lee_nego
**Procedimiento Almacenado:** CMXsrv_icrd_lee_neg

#### Tablas Involucradas:
- TAS
- CRD
- ACMXFINVER
- NEG
- NEG_ADI
- DIS
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: AVI_COL.FRM
**Segmento:** avi_col1
**Procedimiento Almacenado:** CMXsrv_col_avi_dat_cln

#### Tablas Involucradas:
- TIP
- CRD
- DAC
- ACMXESPECI
- ACMXSUCSAL
- CLN
- COL
- ACLNEJECTA

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: AVI_COL.FRM
**Segmento:** avi_col1
**Procedimiento Almacenado:** CMXsrv_col_avi_det_pag

#### Tablas Involucradas:
- CCX
- TIP
- TAS
- CRD
- COB
- ACMXINTERE
- EVE
- ACMXMONEDA
- ACMXINTEREFEC
- CAN
- CAN_REN
- COL

#### Procedimientos Llamados:
- CMX_srv_pone_punto
- CMXsrv_util_fecha
- sp_procxmode

---

### Archivo: AVI_COL.FRM
**Segmento:** avi_col2
**Procedimiento Almacenado:** CMXsrv_col_avi_dat_cln

#### Tablas Involucradas:
- TIP
- CRD
- DAC
- ACMXESPECI
- ACMXSUCSAL
- CLN
- COL
- ACLNEJECTA

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: AVI_COL.FRM
**Segmento:** avi_col2
**Procedimiento Almacenado:** CMXsrv_col_avi_det_oto

#### Tablas Involucradas:
- TIP
- ACMXDESEMB
- ASND
- TAS
- CUO
- COD
- NEG
- ACMXINTERE
- EVE
- ACMXMONEDA
- ACMXINTEREFEC
- AVAL
- CLN
- COL

#### Procedimientos Llamados:
- CMX_srv_pone_punto
- CMXsrv_trae_glo_fec
- sp_procxmode

---

### Archivo: AVI_COL.FRM
**Segmento:** avi_col4
**Procedimiento Almacenado:** CMXsrv_col_avi_dat_cln

#### Tablas Involucradas:
- TIP
- CRD
- DAC
- ACMXESPECI
- ACMXSUCSAL
- CLN
- COL
- ACLNEJECTA

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: AVI_COL.FRM
**Segmento:** avi_col4
**Procedimiento Almacenado:** CMXsrv_col_lee_num_trs

#### Tablas Involucradas:
- EVE
- COL
- TIP
- COD

#### Procedimientos Llamados:
- CMXsrv_avigrl_lee_avitemp
- sp_procxmode

---

### Archivo: AVI_COL.FRM
**Segmento:** lee_obl_pag
**Procedimiento Almacenado:** CMXsrv_finobl_avi_pag

#### Tablas Involucradas:
- CNO
- EVO

#### Procedimientos Llamados:
- CMX_srv_pone_punto
- sp_procxmode

---

### Archivo: AVI_COL.FRM
**Segmento:** traspaso
**Procedimiento Almacenado:** CMXsrv_neg_avi_trae_asnd_mn

#### Tablas Involucradas:
- ACMXDESEMB
- ASND
- COD
- TRSD
- ACMXMONEDA

#### Procedimientos Llamados:
- CMX_srv_pone_punto
- sp_procxmode

---

### Archivo: AVI_COL.FRM
**Segmento:** traspaso
**Procedimiento Almacenado:** CMXsrv_neg_avi_trae_asnd_mx

#### Tablas Involucradas:
- ACMXDESEMB
- ACMXMONEDA
- ASND

#### Procedimientos Llamados:
- CMX_srv_pone_punto
- sp_procxmode

---

### Archivo: CRD01001.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_icrd_neg_lee_crd

#### Tablas Involucradas:
- NEG
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD01001.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_icrd_lee_neg

#### Tablas Involucradas:
- TAS
- CRD
- ACMXFINVER
- NEG
- NEG_ADI
- DIS
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD01001.FRM
**Segmento:** Mcrdtxtliq_Click
**Procedimiento Almacenado:** CMXsrv_icrd_lee_dat_trs

#### Tablas Involucradas:
- ASND
- EVI
- TRSD
- EVE
- ACMXMONEDA
- COL

#### Procedimientos Llamados:
- CMXsrv_icrd_forlin
- sp_procxmode

---

### Archivo: CRD01001.FRM
**Segmento:** Mcrdtxtope_Click
**Procedimiento Almacenado:** CMXsrv_icrd_dat_liq_ope

#### Tablas Involucradas:
- ACMXDESEMB
- ASND
- EVO
- CRD
- CNO
- OBL
- CUO
- TRSD
- NEG
- COM
- EVE
- ACMXTIPEVE
- CAN
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD01001.FRM
**Segmento:** MNEGCONT_Click
**Procedimiento Almacenado:** CMXsrv_icrd_cont_neg

#### Tablas Involucradas:
- COL
- NEG
- CRD
- COD

#### Procedimientos Llamados:
- CMXsrv_icrd_val_neg
- CMXsrv_mbyte_gen
- sp_procxmode
- sp_cmx_sii_1870
- CMXsrv_fincol_ictb_neg_aux

---

### Archivo: CRD01001.FRM
**Segmento:** MNEGELI_CLICK
**Procedimiento Almacenado:** CMXsrv_icrd_eli_neg

#### Tablas Involucradas:
- CRD
- COM
- NEG
- CND
- NEG_ADI
- ACMXTXTSWF
- comex..COL

#### Procedimientos Llamados:
- CMXsrv_swf_graba_det
- sp_procxmode

---

### Archivo: CRD01001.FRM
**Segmento:** precarga_datos
**Procedimiento Almacenado:** CMXsrv_icrd_a_rec_age

#### Tablas Involucradas:
- COR
- TAS
- CRD
- CUO
- CNEG
- COM
- NEG
- TRSD
- DIS
- EVE
- ACMXMONEDA
- ACMXINTERE
- ACMXSUCSAL
- COL

#### Procedimientos Llamados:
- CMXsrv_util_fecha
- sp_procxmode

---

### Archivo: CRD01001.FRM
**Segmento:** precarga_datos
**Procedimiento Almacenado:** CMXsrv_busc_ofi_cta

#### Tablas Involucradas:
- CLN

#### Procedimientos Llamados:
- PrmACMXESPECI
- PrmACLNEJECTA
- sp_procxmode

---

### Archivo: PREFER.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_trae_glo_fec

#### Tablas Involucradas:
- ACMXSUCSAL
- ACMXDL3475FEC
- tbl_User

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: PREFER.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_icrd_lee_num_col

#### Tablas Involucradas:
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: VER_PAGO.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_icrd_bus_pago

#### Tablas Involucradas:
- CAN

#### Procedimientos Llamados:
- sp_procxmode

---

## NNEGO
<a name="nnego"></a>
### Archivo: CRD01001.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_icrd_neg_lee_crd

#### Tablas Involucradas:
- NEG
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD01001.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_icrd_lee_neg

#### Tablas Involucradas:
- TAS
- CRD
- ACMXFINVER
- NEG
- NEG_ADI
- DIS
- COL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD01001.FRM
**Segmento:** gen_mens_swift
**Procedimiento Almacenado:** CMXsrv_iswf_a_pru

#### Tablas Involucradas:
- switxt
- switxt1

#### Procedimientos Llamados:
- CMXsrv_iswf_a_732
- CMXsrv_iswf_esp_707b
- CMXsrv_iswf_a_747
- CMXsrv_iswf_a_412
- CMXsrv_iswf_a_707b
- CMXsrv_iswf_esp_740
- CMXsrv_iswf_a_410
- CMXsrv_iswf_esp_747
- CMXsrv_iswf_neg_730
- CMXsrv_iswf_neg_752
- CMXsrv_iswf_a_700a
- CMXsrv_iswf_a_707a
- CMXsrv_iswf_esp_700b
- CMXsrv_iswf_a_740
- CMXsrv_iswf_a_700b
- CMXsrv_iswf_esp_707a
- srv_irem_imp_202
- CMXsrv_iswf_747_neg
- srv_irem_imp_100
- sp_procxmode
- CMXsrv_iswf_esp_700a

---

### Archivo: CRD01001.FRM
**Segmento:** llama_pagos
**Procedimiento Almacenado:** CMXsrv_icrd_lee_col

#### Tablas Involucradas:
- CCL
- COL
- TAS

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD01001.FRM
**Segmento:** Mnegavi9_Click
**Procedimiento Almacenado:** CMXsrv_iswf_a_pru

#### Tablas Involucradas:
- switxt
- switxt1

#### Procedimientos Llamados:
- CMXsrv_iswf_a_732
- CMXsrv_iswf_esp_707b
- CMXsrv_iswf_a_747
- CMXsrv_iswf_a_412
- CMXsrv_iswf_a_707b
- CMXsrv_iswf_esp_740
- CMXsrv_iswf_a_410
- CMXsrv_iswf_esp_747
- CMXsrv_iswf_neg_730
- CMXsrv_iswf_neg_752
- CMXsrv_iswf_a_700a
- CMXsrv_iswf_a_707a
- CMXsrv_iswf_esp_700b
- CMXsrv_iswf_a_740
- CMXsrv_iswf_a_700b
- CMXsrv_iswf_esp_707a
- srv_irem_imp_202
- CMXsrv_iswf_747_neg
- srv_irem_imp_100
- sp_procxmode
- CMXsrv_iswf_esp_700a

---

### Archivo: CRD01001.FRM
**Segmento:** MNEGCONT_Click
**Procedimiento Almacenado:** CMXsrv_icrd_cont_neg

#### Tablas Involucradas:
- COL
- NEG
- CRD
- COD

#### Procedimientos Llamados:
- CMXsrv_icrd_val_neg
- CMXsrv_mbyte_gen
- sp_procxmode
- sp_cmx_sii_1870
- CMXsrv_fincol_ictb_neg_aux

---

### Archivo: CRD01001.FRM
**Segmento:** MNEGELI_CLICK
**Procedimiento Almacenado:** CMXsrv_icrd_eli_neg

#### Tablas Involucradas:
- CRD
- COM
- NEG
- CND
- NEG_ADI
- ACMXTXTSWF
- comex..COL

#### Procedimientos Llamados:
- CMXsrv_swf_graba_det
- sp_procxmode

---

### Archivo: CRD01001.FRM
**Segmento:** pertas_Click
**Procedimiento Almacenado:** CMXsrv_icrd_lee_col

#### Tablas Involucradas:
- CCL
- COL
- TAS

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD01002.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_icrd_busc_neg

#### Tablas Involucradas:
- NEG

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD01003.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_icrd_busc_emb

#### Tablas Involucradas:
- comex..EMB
- comex..MEMB

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD01005.FRM
**Segmento:** ACEPTAR_Click
**Procedimiento Almacenado:** CMXsrv_icrd_a_neg_emb1

#### Tablas Involucradas:
- TAS
- CNEG
- NEG
- COL
- DOCNEG

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD01005.FRM
**Segmento:** ACEPTAR_Click
**Procedimiento Almacenado:** CMXsrv_icrd_a_neg_emb2

#### Tablas Involucradas:
- NEG
- COL
- comex..COL
- DOCNEG

#### Procedimientos Llamados:
- sp_procxmode
- CMXsrv_icrd_chq_doc_neg

---

### Archivo: CRD01005.FRM
**Segmento:** CANCELAR_Click
**Procedimiento Almacenado:** CMXsrv_icrd_eli_doc_neg

#### Tablas Involucradas:
- COL
- DOCNEG

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD01005.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_icrd_lee_emb1

#### Tablas Involucradas:
- CRS
- COL
- EMB

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD01005.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_icrd_lee_emb2

#### Tablas Involucradas:
- COL
- EMB

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD01005.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_icrd_lee_neg_emb1

#### Tablas Involucradas:
- COL
- NEG

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD01005.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_icrd_lee_neg_emb2

#### Tablas Involucradas:
- COL
- NEG

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD01005.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_icrd_lee_cnd_esp

#### Tablas Involucradas:
- MMCND
- COL
- CND

#### Procedimientos Llamados:
- sp_procxmode
- CMXsrv_icrd_pre_47

---

### Archivo: CRD01005.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_icrd_lee_desc_merc

#### Tablas Involucradas:
- MMER
- MER

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD01006.FRM
**Segmento:** ACEPTAR_Click
**Procedimiento Almacenado:** CMXsrv_icrd_a_neg_disc

#### Tablas Involucradas:
- COL
- DIS
- NEG

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD01006.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_icrd_neg_lee_disc

#### Tablas Involucradas:
- DIS
- NEG

#### Procedimientos Llamados:
- sp_procxmode
- CMXsrv_icrd_gen_disc

---

### Archivo: CRD01201.FRM
**Segmento:** ACEPTAR_Click
**Procedimiento Almacenado:** CMXsrv_icrd_ent_doc

#### Tablas Involucradas:
- COL
- NEG
- comex..COL

#### Procedimientos Llamados:
- CMXsrv_mbyte_gen
- CMXsrv_swf_graba_det
- sp_procxmode

---

### Archivo: CRD01201.FRM
**Segmento:** ELIMINAR_Click
**Procedimiento Almacenado:** CMXsrv_icrd_ent_doc

#### Tablas Involucradas:
- COL
- NEG
- comex..COL

#### Procedimientos Llamados:
- CMXsrv_mbyte_gen
- CMXsrv_swf_graba_det
- sp_procxmode

---

### Archivo: CRD01201.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_icrd_ent_doc

#### Tablas Involucradas:
- COL
- NEG
- comex..COL

#### Procedimientos Llamados:
- CMXsrv_mbyte_gen
- CMXsrv_swf_graba_det
- sp_procxmode

---

### Archivo: CRD01301.FRM
**Segmento:** ACEPTAR_Click
**Procedimiento Almacenado:** CMXsrv_icrd_alz_disc

#### Tablas Involucradas:
- comex..ACMXINTEREFEC
- COR
- TAS
- CRD
- CUO
- COD
- CNEG
- NEG
- ACMXMONEDAFEC
- NEG_ADI
- ACMXINTERE
- ACMXBCOUSU
- ACMXINTEREFEC
- sysobjects
- COL

#### Procedimientos Llamados:
- CMXsrv_get_ult_dia_habil
- CMXsrv_icrd_cont_alz
- CMXsrv_ipuc_gen_pln
- sp_procxmode
- CMXsrv_cnt_950
- CMXsrv_cmx_get_codes
- CMXsrv_fincol_cal_tas_sfr

---

### Archivo: CRD02001.FRM
**Segmento:** aceptar_click
**Procedimiento Almacenado:** CMXCRDsrv_icrd_asignar_cor

#### Tablas Involucradas:
- COR
- ACMXMONEDAFEC
- CRD
- LCR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD02001.FRM
**Segmento:** BUSCAR_Click
**Procedimiento Almacenado:** CMXCRDsrv_icrd_bus_lcr_bco

#### Tablas Involucradas:
- COR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD02001.FRM
**Segmento:** proximo_Click
**Procedimiento Almacenado:** CMXCRDsrv_icrd_bus_lcr_bco

#### Tablas Involucradas:
- COR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD02004.FRM
**Segmento:** ACEPTAR_Click
**Procedimiento Almacenado:** CMXsrv_icrd_act_doc_neg

#### Tablas Involucradas:
- NEG
- COL
- DOCNEG

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD02004.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_icrd_lee_doc_neg

#### Tablas Involucradas:
- NEG
- EMB

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: GRL00101.FRM
**Segmento:** enviar_Click
**Procedimiento Almacenado:** CMXsrv_iswf_a_pru

#### Tablas Involucradas:
- switxt
- switxt1

#### Procedimientos Llamados:
- CMXsrv_iswf_a_732
- CMXsrv_iswf_esp_707b
- CMXsrv_iswf_a_747
- CMXsrv_iswf_a_412
- CMXsrv_iswf_a_707b
- CMXsrv_iswf_esp_740
- CMXsrv_iswf_a_410
- CMXsrv_iswf_esp_747
- CMXsrv_iswf_neg_730
- CMXsrv_iswf_neg_752
- CMXsrv_iswf_a_700a
- CMXsrv_iswf_a_707a
- CMXsrv_iswf_esp_700b
- CMXsrv_iswf_a_740
- CMXsrv_iswf_a_700b
- CMXsrv_iswf_esp_707a
- srv_irem_imp_202
- CMXsrv_iswf_747_neg
- srv_irem_imp_100
- sp_procxmode
- CMXsrv_iswf_esp_700a

---

### Archivo: GRL00101.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_icrd_val_neg

#### Tablas Involucradas:
- DDI
- COR
- ADI
- TAS
- CUO
- NEG
- ACMXMONEDAFEC
- DAC
- ACMXINTERE
- ACMXMONEDA
- ACMXSIGGAR
- ACMXINTEREFEC
- CAN
- DIS
- warnmsg
- AVAL
- COL
- CCO

#### Procedimientos Llamados:
- CMXsrv_util_det_habil_tasa
- CMXsrv_fincol_val_per_tas
- CMXsrv_util_fecha
- sp_procxmode

---

### Archivo: PREFER.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_grl_fec_serv

#### Tablas Involucradas:

#### Procedimientos Llamados:
- SRV_MessageService
- sp_procxmode

---

### Archivo: VER_PAGO.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_icrd_bus_pago

#### Tablas Involucradas:
- CAN

#### Procedimientos Llamados:
- sp_procxmode

---

## PAGCBR
<a name="pagcbr"></a>
### Archivo: CBR01006.FRM
**Segmento:** ACEPTAR_Click
**Procedimiento Almacenado:** CMXsrv_icbr_lee_dat_var

#### Tablas Involucradas:
- ACMXMONEDAFEC
- CBR
- ACMXPRMENL

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR01006.FRM
**Segmento:** ACEPTAR_Click
**Procedimiento Almacenado:** CMXsrv_icbr_val_pag

#### Tablas Involucradas:
- LCB
- CBR
- CCO

#### Procedimientos Llamados:
- CMXsrv_val_cta_cte
- CMXsrv_calc_imp_4pct
- CMXsrv_util_fecha
- sp_procxmode
- CMXsrv_enl_val_sel
- CMXsrv_ctb_impto_ddi

---

### Archivo: CBR01006.FRM
**Segmento:** ACEPTAR_Click
**Procedimiento Almacenado:** CMXsrv_icbr_ctb_pag

#### Tablas Involucradas:
- LCB
- ACMXDESEMB
- vig_cmx
- COD
- ICX
- COM
- ACMXMONEDAFEC
- CBR
- PCX
- DIP
- LIB
- CLN
- CCO

#### Procedimientos Llamados:
- CMXsrv_mbyte_gen
- CMXsrv_get_ult_dia_habil
- CMXsrv_val_cta_cte
- CMXsrv_cnt_gen_vig
- CMXsrv_calc_imp_4pct
- CMXsrv_util_fecha
- CMXsrv_vig_gra_vig
- CMXsrv_ipuc_gen_pln
- CMXsrv_icbr_act_rem
- CMXsrv_enl_act_enl
- sp_procxmode
- CMXsrv_icbr_ctb_pag1
- sp_cmx_sii_1870
- CMXsrv_iddi2_gen_det_pag
- CMXsrv_cmx_get_codes
- CMXsrv_ctb_impto_ddi
- CMXsrv_util_pesos

---

### Archivo: CBR01006.FRM
**Segmento:** Calcular_Click
**Procedimiento Almacenado:** CMXsrv_icbr_cal_pag

#### Tablas Involucradas:
- DDI
- ADI
- ACMXMONEDAFEC
- CBR
- COB
- ACMXMONEDA

#### Procedimientos Llamados:
- CMXsrv_get_ult_dia_habil
- sp_procxmode
- CMXsrv_valida_tc
- CMXsrv_icbr_cal_int
- CMXsrv_icbr_cre_pln

---

### Archivo: CBR01006.FRM
**Segmento:** CANCELAR_Click
**Procedimiento Almacenado:** CMXsrv_icbr_eli_pag

#### Tablas Involucradas:
- ECE
- PCX
- COB
- ICX

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR01006.FRM
**Segmento:** fld_cbr_cod_des_mn_pag_lostfocus
**Procedimiento Almacenado:** CMXsrv_val_vig

#### Tablas Involucradas:
- ACMXPLNCTAN
- ACMXDESEMB
- ACMXPLNCTAX

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR01006.FRM
**Segmento:** fld_cbr_cod_des_mx_pag_lostfocus
**Procedimiento Almacenado:** CMXsrv_val_vig

#### Tablas Involucradas:
- ACMXPLNCTAN
- ACMXDESEMB
- ACMXPLNCTAX

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR01006.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_icbr_lee_cbr0

#### Tablas Involucradas:
- ACMXMONEDA
- CBR

#### Procedimientos Llamados:
- CMXsrv_icrd_lee_cln
- sp_procxmode

---

### Archivo: CBR01006.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_icbr_obt_mon_nac

#### Tablas Involucradas:

#### Procedimientos Llamados:
- CMXsrv_cmx_get_codes
- sp_procxmode

---

### Archivo: CBR01006.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_icbr_lee_dat_pag

#### Tablas Involucradas:
- ACMXDESEMB
- ECE
- PCX
- CBR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR01006.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_icbr_pcg_pag

#### Tablas Involucradas:
- ACMXMONEDAFEC
- CBR

#### Procedimientos Llamados:
- PrmACMXMONEDAFEC
- sp_procxmode

---

### Archivo: CBR01006.FRM
**Segmento:** lee_cta
**Procedimiento Almacenado:** CMXsrv_vig_lee_cta

#### Tablas Involucradas:
- ACMXPLNCTAN
- ACMXDESEMB
- ACMXPLNCTAX

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR01007.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_icbr_busc_pago

#### Tablas Involucradas:
- PCX

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CBR01008.FRM
**Segmento:** ACEPTAR_Click
**Procedimiento Almacenado:** CMXsrv_icbr_val_pag

#### Tablas Involucradas:
- LCB
- CBR
- CCO

#### Procedimientos Llamados:
- CMXsrv_val_cta_cte
- CMXsrv_calc_imp_4pct
- CMXsrv_util_fecha
- sp_procxmode
- CMXsrv_enl_val_sel
- CMXsrv_ctb_impto_ddi

---

### Archivo: COB00303.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_icob_act_val

#### Tablas Involucradas:
- ACMXMONEDAFEC
- COB

#### Procedimientos Llamados:
- CMXsrv_get_ult_dia_habil
- sp_procxmode
- CMXsrv_icob_val_cob

---

### Archivo: COB00303.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_icob_lee_val

#### Tablas Involucradas:
- COB

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COB00305.FRM
**Segmento:** ELIMINAR_Click
**Procedimiento Almacenado:** CMXsrv_icbr_eli_int_pago

#### Tablas Involucradas:
- PCX
- ICX

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COB00305.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_icbr_busc_int

#### Tablas Involucradas:
- ICX

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COB00306.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_icbr_ingmod_int

#### Tablas Involucradas:
- PCX
- CBR
- ICX
- ACMXINTEREFEC

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: COB00306.FRM
**Segmento:** Form_Activate
**Procedimiento Almacenado:** CMXsrv_icbr_lee_int_pago

#### Tablas Involucradas:
- ICX

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00602.FRM
**Segmento:** Aceptar_Click
**Procedimiento Almacenado:** CMXsrv_icbr_lee_bco

#### Tablas Involucradas:
- ACMXPAIS
- COR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: CRD00602.FRM
**Segmento:** buscar_Click
**Procedimiento Almacenado:** CMXsrv_icbr_busc_bco

#### Tablas Involucradas:
- COR

#### Procedimientos Llamados:
- sp_procxmode

---

### Archivo: PREFER.FRM
**Segmento:** Form_Load
**Procedimiento Almacenado:** CMXsrv_grl_fec_serv

#### Tablas Involucradas:

#### Procedimientos Llamados:
- SRV_MessageService
- sp_procxmode

---

