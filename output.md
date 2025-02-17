# Índice Bancomex

# Exportaciones
  - **[EXPCBE](#expcbe)**
  - **[EXPCCE](#expcce)**
  - **[expdex](#expdex)**
  - **[EXPNEG](#expneg)**
  - **[expret](#expret)**

# Financiamiento
  - **[ADMIN](#admin)**
  - **[COL_NEG](#col_neg)**
  - **[INGRESO](#ingreso)**
  - **[MODIFIC](#modific)**
  - **[OBLIGA](#obliga)**
  - **[PAGOS](#pagos)**
  - **[PGOEXT](#pgoext)**

# Importaciones
  - **[ARCOS](#arcos)**
  - **[COBERIMP](#coberimp)**
  - **[COBRANZA](#cobranza)**
  - **[CRDEXT](#crdext)**
  - **[CRD_CORR](#crd_corr)**
  - **[DDI](#ddi)**
  - **[IMPORT](#import)**
  - **[INFORME](#informe)**
  - **[MOD_ADI](#mod_adi)**
  - **[MOD_CBR](#mod_cbr)**
  - **[MOD_CRD](#mod_crd)**
  - **[NEGO_AV](#nego_av)**
  - **[NNEGO](#nnego)**
  - **[PAGCBR](#pagcbr)**

## EXPCBE
<a name="expcbe"></a>

| **Archivo (Frame)** | **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** |
|--------------------|-------------|-----------------------------|----------------------|
| CBE00101.FRM | Form_Activate | [CMXsrv_expcbe_lee_prm](#cmxsrv_expcbe_lee_prm) | ACMXPRMGRL |
| CBE00101.FRM | Form_Activate | [CMXsrv_cmx_busc_suc_usu](#cmxsrv_cmx_busc_suc_usu) | master..sysprocesses, tbl_User |
| CBE00101.FRM | Form_Activate | [CMXsrv_expcbe_lee_cbe](#cmxsrv_expcbe_lee_cbe) | ACMXPAIS, COR, ACMXPGOCBE, CBE01, CBE, ACMXMONEDA, ACMXENTDOC, ACMXSUCSAL, ACMXPRTCBE, CLN |
| CBE00101.FRM | Form_Load | [CMXsrv_trae_glo_fec](#cmxsrv_trae_glo_fec) | ACMXSUCSAL, ACMXDL3475FEC, tbl_User |
| CBE00101.FRM | ingcomg_Click | [CMXsrv_expcbe_avs_cyg1](#cmxsrv_expcbe_avs_cyg1) | ACMXDESEMB, ASND, ACMXIMPUES, ACMXPRMGRL, EVZ, CBE, COM, TRSD, CLN, ACMXESPECI |
| CBE00101.FRM | ingcomg_Click | [CMXsrv_expcbe_avs_cyg2](#cmxsrv_expcbe_avs_cyg2) | ASND, ACMXIMPUES, ACMXPRMGRL, EVZ, CBE |
| CBE00101.FRM | ingret_Click | [CMXsrv_expcbe_avs_ret](#cmxsrv_expcbe_avs_ret) | ACMXPAIS, COR, ACMXDESEMB, CBE, ACMXMONEDA, ACMXSUCSAL, CLN, ACMXESPECI, RET |
| CBE00101.FRM | M3_Click | [CMXsrv_expcbe_swf_sel](#cmxsrv_expcbe_swf_sel) | switxt, switxt1 |
| CBE00101.FRM | M4_Click | [CMXsrv_expcbe_swf_sel](#cmxsrv_expcbe_swf_sel) | switxt, switxt1 |
| CBE00101.FRM | Mcbeanl_Click | [CMXsrv_expcbe_anl_cbe](#cmxsrv_expcbe_anl_cbe) | CBE |
| CBE00101.FRM | Mcbectb_Click | [CMXsrv_expcbe_ctb_ing](#cmxsrv_expcbe_ctb_ing) | OPE_BCI, CBE |
| CBE00101.FRM | Mcbedel_Click | [CMXsrv_expcbe_del_cbe](#cmxsrv_expcbe_del_cbe) | EVL, CBE01, COD, CBE, EVZ, COM, ACTZ, CTZ |
| CBE00101.FRM | Mcbeval_Click | [CMXsrv_expcbe_val_cbe](#cmxsrv_expcbe_val_cbe) | COR, CBE01, ACMXPRMGRL, CBE, DCZ, CTZ, warnmsg, ACMXPAIS, ACMXFERIADO, CCO |
| CBE00101.FRM | Men1_Click | [CMXsrv_expcbe_swf_sel](#cmxsrv_expcbe_swf_sel) | switxt, switxt1 |
| CBE00201.FRM | aceptar_Click | [CMXsrv_expcbe_grb_ctp](#cmxsrv_expcbe_grb_ctp) | ACMXPAIS, CBE |
| CBE00201.FRM | fld_cbe_cod_exp_lostfocus | [CMXsrv_expcbe_lee_cln](#cmxsrv_expcbe_lee_cln) | CLN |
| CBE00201.FRM | fld_cbe_cod_suc_LostFocus | [CMXsrv_val_suc](#cmxsrv_val_suc) | ACMXSUCSAL, tbl_User |
| CBE00201.FRM | Form_Activate | [CMXsrv_expcbe_lee_ctp](#cmxsrv_expcbe_lee_ctp) | ACMXSUCSAL, ACMXPAIS, CBE, CLN |
| CBE00202.FRM | aceptar_Click | [CMXsrv_expcbe_grb_bco](#cmxsrv_expcbe_grb_bco) | ACMXPRMGRL, CBE, COR, CBE01 |
| CBE00202.FRM | fld_cbe_cod_cob_Lostfocus | [CMXsrv_expcbe_lee_cor](#cmxsrv_expcbe_lee_cor) | ACMXPAIS, COR |
| CBE00202.FRM | fld_cbe_cod_rmb_LostFocus | [CMXsrv_expcbe_lee_cor](#cmxsrv_expcbe_lee_cor) | ACMXPAIS, COR |
| CBE00202.FRM | Form_Activate | [CMXsrv_expcbe_lee_bco](#cmxsrv_expcbe_lee_bco) | CBE, COR, CBE01 |
| CBE00204.FRM | aceptar_Click | [CMXsrv_expcbe_grb_doc](#cmxsrv_expcbe_grb_doc) | CBE, DCZ |
| CBE00204.FRM | aceptar_Click | [CMXsrv_expcbe_grb_doc02](#cmxsrv_expcbe_grb_doc02) | CBE02 |
| CBE00204.FRM | Form_Activate | [CMXsrv_expcbe_lee_doc](#cmxsrv_expcbe_lee_doc) | CBE |
| CBE00204.FRM | Form_Activate | [CMXsrv_expcbe_lee_doc02](#cmxsrv_expcbe_lee_doc02) | CBE02 |
| CBE00206.FRM | ELIMINAR_Click | [CMXsrv_expcbe_del_ctz](#cmxsrv_expcbe_del_ctz) | ACTZ, CBE, CTZ |
| CBE00206.FRM | Form_Activate | [CMXsrv_expcbe_bus_ctz](#cmxsrv_expcbe_bus_ctz) | ACTZ, CBE, CTZ |
| CBE00207.FRM | aceptar_Click | [CMXsrv_expcbe_grb_ctz](#cmxsrv_expcbe_grb_ctz) | ACTZ, CBE, CTZ |
| CBE00207.FRM | Form_Activate | [CMXsrv_expcbe_mto_ctz](#cmxsrv_expcbe_mto_ctz) | ACTZ, CBE, CTZ |
| CBE00207.FRM | Form_Activate | [CMXsrv_expcbe_lee_ctz](#cmxsrv_expcbe_lee_ctz) | ACTZ, CBE, CTZ |
| CBE00301.FRM | aceptar_Click | [CMXsrv_expcbe_lee_cbe](#cmxsrv_expcbe_lee_cbe) | ACMXPAIS, COR, ACMXPGOCBE, CBE01, CBE, ACMXMONEDA, ACMXENTDOC, ACMXSUCSAL, ACMXPRTCBE, CLN |
| CBE00301.FRM | buscar_Click | [CMXsrv_expcbe_bus_cbe](#cmxsrv_expcbe_bus_cbe) | CBE |
| CBE00301.FRM | fld_aux_cod_exp_LostFocus | [CMXsrv_expcbe_lee_cln](#cmxsrv_expcbe_lee_cln) | CLN |
| CBE00301.FRM | Proximas_Click | [CMXsrv_expcbe_bus_cbe](#cmxsrv_expcbe_bus_cbe) | CBE |
| CBE00401.FRM | aceptar_Click | [CMXsrv_expcbe_mdf_cbe](#cmxsrv_expcbe_mdf_cbe) | ACTZ, ACMXPRMGRL, CBE |
| CBE00401.FRM | aceptar_Click | [CMXsrv_expcbe_cre_actz](#cmxsrv_expcbe_cre_actz) | ACTZ, CBE, CTZ |
| CBE00401.FRM | fld_cbe_cod_suc_LostFocus | [CMXsrv_val_suc](#cmxsrv_val_suc) | ACMXSUCSAL, tbl_User |
| CBE00401.FRM | Form_Activate | [CMXsrv_expcbe_lee_mdf](#cmxsrv_expcbe_lee_mdf) | COR, ACMXPGOCBE, CBE01, CBE, ACMXMONEDA, ACMXSUCSAL, CLN |
| CBE00501.FRM | aceptar_Click | [CMXsrv_expcbe_pgo_cbe](#cmxsrv_expcbe_pgo_cbe) | ACMXDESEMB, COR, CLN, RET, vig_cmx, COD, ACMXIMPUES, ACMXPRMGRL, CBE, ACMXPRMEXP, COM, tbl_User, OPREC, ACMXPAIS, ACMXFERIADO, CCO |
| CBE00501.FRM | fld_cbe_cod_rmb_LostFocus | [CMXsrv_expcbe_lee_cor](#cmxsrv_expcbe_lee_cor) | ACMXPAIS, COR |
| CBE00501.FRM | Form_Activate | [CMXsrv_expcbe_lee_pgo](#cmxsrv_expcbe_lee_pgo) | ACMXDESEMB, COR, CBE, ACMXPRMEXP, ACMXMONEDA, OPREC, CLN |
| CBE00601.FRM | Form_Activate | [CMXsrv_expcbe_bus_evz](#cmxsrv_expcbe_bus_evz) | EVZ, CBE |
| CBE00601.FRM | Proximo_Click | [CMXsrv_expcbe_bus_evz](#cmxsrv_expcbe_bus_evz) | EVZ, CBE |
| CBE00601.FRM | Reversar_Click | [CMXsrv_expcbe_rev_cbe](#cmxsrv_expcbe_rev_cbe) | EVL, ACMXDESEMB, COR, ORG, ACMXIMPUES, ACMXPRMGRL, EVZ, CBE, TRSD, ACMXPRMEXP, COM, EVR, CTZ, DTN, OPREC, RET, PUCBCX10 |
| CBE00602.FRM | Form_Activate | [CMXsrv_expcbe_lee_evz](#cmxsrv_expcbe_lee_evz) | ACMXDESEMB, COR, ACMXPGOCBE, EVZ, CBE, ACMXMONEDA, ACMXTIPEVE, ACMXSUCSAL |
| CBE00603.FRM | Eliminar_Click | [CMXsrv_expcbe_del_dcz](#cmxsrv_expcbe_del_dcz) | CBE02, CBE, DCZ |
| CBE00603.FRM | Form_Activate | [CMXsrv_expcbe_bus_dcz](#cmxsrv_expcbe_bus_dcz) | DCZ |
| CBE00604.FRM | aceptar_Click | [CMXsrv_expcbe_grb_dcz](#cmxsrv_expcbe_grb_dcz) | CBE02, CBE, DCZ |
| CBE00604.FRM | Form_Activate | [CMXsrv_expcbe_lee_dcz](#cmxsrv_expcbe_lee_dcz) | DCZ |
| CBE00605.FRM | aceptar_Click | [CMXsrv_expcbe_lee_cbe](#cmxsrv_expcbe_lee_cbe) | ACMXPAIS, COR, ACMXPGOCBE, CBE01, CBE, ACMXMONEDA, ACMXENTDOC, ACMXSUCSAL, ACMXPRTCBE, CLN |
| CBE00605.FRM | buscar_Click | [CMXsrv_expcbe_bus_vto](#cmxsrv_expcbe_bus_vto) | CBE |
| CBE00605.FRM | fld_aux_cod_exp_LostFocus | [CMXsrv_expcbe_lee_cln](#cmxsrv_expcbe_lee_cln) | CLN |
| CBE00605.FRM | Proximas_Click | [CMXsrv_expcbe_bus_vto](#cmxsrv_expcbe_bus_vto) | CBE |
| CBEAVIRE.FRM | aceptar_Click | [CMXsrv_avi_dat_cou](#cmxsrv_avi_dat_cou) |  |
| CBEAVIRE.FRM | aceptar_Click | [CMXsrv_expcbe_avs_rem1](#cmxsrv_expcbe_avs_rem1) | COR, ACMXPGOCBE, ACMXPRTCBE, CBE01, CBE, CBE02, ACMXMONEDA, CTZ, ACMXENTDOC, ACMXPAIS, ACMXPAISES, CLN |
| CBEAVIRE.FRM | aceptar_Click | [CMXsrv_expcbe_avs_rem3](#cmxsrv_expcbe_avs_rem3) | COR, CBE01, CBE, CTZ, ACMXMONEDA, ACMXPAISES, CLN, CCO |
| CBEAVIRE.FRM | imprime_esp | [CMXsrv_expcbe_avs_rem2](#cmxsrv_expcbe_avs_rem2) | CBE02, CBE, DCZ |
| CBEAVIRE.FRM | imprime_esp | [CMXsrv_expcbe_avs_rem4](#cmxsrv_expcbe_avs_rem4) | ACMXREMFESPMSG, ACMXREMFINGMSG |
| CBEAVIRE.FRM | imprime_ing | [CMXsrv_expcbe_avs_rem2](#cmxsrv_expcbe_avs_rem2) | CBE02, CBE, DCZ |
| CBEAVIRE.FRM | imprime_ing | [CMXsrv_expcbe_avs_rem4](#cmxsrv_expcbe_avs_rem4) | ACMXREMFESPMSG, ACMXREMFINGMSG |
| COR00906.FRM | buscar_Click | [CMXsrv_busc_plz](#cmxsrv_busc_plz) | ACMXPLAZAS, comex..ACMXPLAZAS |
| COR00906.FRM | fld_cor_cod_plz_Lostfocus | [CMXsrv_lee_plz](#cmxsrv_lee_plz) | ACMXPLAZAS |
| COR00906.FRM | proximos_Click | [CMXsrv_busc_plz](#cmxsrv_busc_plz) | ACMXPLAZAS, comex..ACMXPLAZAS |
| COR00907.FRM | buscar_Click | [CMXsrv_cor_busc_pais](#cmxsrv_cor_busc_pais) | ACMXPAIS |
| COR00907.FRM | fld_cor_cod_pais_LostFocus | [CMXsrv_cor_lee_pais](#cmxsrv_cor_lee_pais) | comex..ACMXPAIS |
| COR00907.FRM | proximos_Click | [CMXsrv_cor_busc_pais](#cmxsrv_cor_busc_pais) | ACMXPAIS |
| CRD00602.FRM | aceptar_Click | [CMXsrv_expcbe_lee_cor](#cmxsrv_expcbe_lee_cor) | ACMXPAIS, COR |
| CRD00602.FRM | buscar_Click | [CMXsrv_expcbe_bus_cor](#cmxsrv_expcbe_bus_cor) | COR |
| CRD00602.FRM | fld_aux_cod_pai_LostFocus | [CMXsrv_cor_lee_pais](#cmxsrv_cor_lee_pais) | comex..ACMXPAIS |
| CRD00602.FRM | fld_aux_cod_plz_LostFocus | [CMXsrv_lee_plz](#cmxsrv_lee_plz) | ACMXPLAZAS |
| CRD00602.FRM | proximos_Click | [CMXsrv_expcbe_bus_cor](#cmxsrv_expcbe_bus_cor) | COR |
| GRID_BUS.FRM | buscar_Click | [CMXsrv_busc_bco_mtr](#cmxsrv_busc_bco_mtr) | ACMXBANCOS |
| GRID_BUS.FRM | proximos_Click | [CMXsrv_busc_bco_mtr](#cmxsrv_busc_bco_mtr) | ACMXBANCOS |
| GRL00101.FRM | enviar_Click | [CMXsrv_expcbe_swf_sel](#cmxsrv_expcbe_swf_sel) | switxt, switxt1 |
| GRLPAIS0.FRM | Aceptar_Click | [CMXsrv_expcbe_lee_cor](#cmxsrv_expcbe_lee_cor) | ACMXPAIS, COR |
| GRLPAIS0.FRM | buscar_Click | [CMXsrv_expcbe_bus_cor](#cmxsrv_expcbe_bus_cor) | COR |
| GRLPAIS0.FRM | proximos_Click | [CMXsrv_expcbe_bus_cor](#cmxsrv_expcbe_bus_cor) | COR |
| PREFER.FRM | Form_Load | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |  |

---

## EXPCCE
<a name="expcce"></a>

| **Archivo (Frame)** | **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** |
|--------------------|-------------|-----------------------------|----------------------|
| CCE00101.FRM | Form_Activate | [CMXsrv_cmx_busc_suc_usu](#cmxsrv_cmx_busc_suc_usu) | master..sysprocesses, tbl_User |
| CCE00101.FRM | Form_Activate | [CMXsrv_expcce_lee_cce](#cmxsrv_expcce_lee_cce) | ACMXPAIS, COR, tbl_User, CCE, ACMXSUCSAL, CLN |
| CCE00101.FRM | Form_Activate | [CMXsrv_expcce_trd_cce](#cmxsrv_expcce_trd_cce) | ACMXFORPAG, ACMXVIATPT, ACMXMAXCCE, ACMXCNFCCE, ACMXMONEDA, ACMXCLACOM, CCE, ACMXRCBCCE |
| CCE00101.FRM | MCCEANL_CLICK | [CMXsrv_expcce_anl_cce](#cmxsrv_expcce_anl_cce) | CCE |
| CCE00101.FRM | Mccectb_click | [CMXsrv_expcce_ctb_ing](#cmxsrv_expcce_ctb_ing) | CCE |
| CCE00101.FRM | Mccedel_Click | [CMXsrv_expcce_del_cce](#cmxsrv_expcce_del_cce) | COD, ACCECTP, ACCECND, CCB, COM, ACCEBCO, DCC, CCE, EVC, ACCEDCC, AFIN |
| CCE00101.FRM | MCCEVAL_CLICK | [CMXsrv_expcce_val_cce](#cmxsrv_expcce_val_cce) | ACMXPAIS, COR, ACMXPRMGRL, CCE_ADI, DCC, tbl_User, CCE, warnmsg, ACMXSUCSAL, COL |
| CCE00101.FRM | Mmt730_Click | [CMXsrv_expcce_swf_sel](#cmxsrv_expcce_swf_sel) | switxt, switxt1 |
| CCE00101.FRM | Mmt730Ing_Click | [CMXsrv_expcce_swf_sel](#cmxsrv_expcce_swf_sel) | switxt, switxt1 |
| CCE00201.FRM | Aceptar_Click | [CMXsrv_expcce_grb_bco](#cmxsrv_expcce_grb_bco) | CCB, ACCEBCO, ACCECRSE, CRSE, CCE |
| CCE00201.FRM | fld_cce_bco_avs_LostFocus | [CMXsrv_expcce_lee_cor](#cmxsrv_expcce_lee_cor) | ACMXPAIS, COR |
| CCE00201.FRM | fld_cce_bco_orig_LostFocus | [CMXsrv_expcce_lee_cor](#cmxsrv_expcce_lee_cor) | ACMXPAIS, COR |
| CCE00201.FRM | fld_cce_cod_ems_LostFocus | [CMXsrv_expcce_lee_cor](#cmxsrv_expcce_lee_cor) | ACMXPAIS, COR |
| CCE00201.FRM | fld_cce_cod_rmb_LostFocus | [CMXsrv_expcce_lee_cor](#cmxsrv_expcce_lee_cor) | ACMXPAIS, COR |
| CCE00201.FRM | Form_Activate | [CMXsrv_expcce_lee_bco](#cmxsrv_expcce_lee_bco) | COR, CCB, ACMXSUCSAL, ACCEBCO, CRSE, CCE, ACMXPAIS |
| CCE00202.FRM | Aceptar_Click | [CMXsrv_expcce_grb_ctp](#cmxsrv_expcce_grb_ctp) | ACCECTP, CCE |
| CCE00202.FRM | fld_cce_cod_bn1_LostFocus | [CMXsrv_expcce_lee_cln](#cmxsrv_expcce_lee_cln) | CLN |
| CCE00202.FRM | fld_cce_cod_bn2_LostFocus | [CMXsrv_expcce_lee_cln](#cmxsrv_expcce_lee_cln) | CLN |
| CCE00202.FRM | Form_Activate | [CMXsrv_expcce_lee_ctp](#cmxsrv_expcce_lee_ctp) | ACCECTP, ACMXPAIS, CLN, CCE |
| CCE00203.FRM | Aceptar_Click | [CMXsrv_expcce_cre_cce](#cmxsrv_expcce_cre_cce) | CCE |
| CCE00203.FRM | Aceptar_Click | [CMXsrv_expcce_grb_bco](#cmxsrv_expcce_grb_bco) | CCB, ACCEBCO, ACCECRSE, CRSE, CCE |
| CCE00203.FRM | Aceptar_Click | [CMXsrv_expcce_grb_ctp](#cmxsrv_expcce_grb_ctp) | ACCECTP, CCE |
| CCE00203.FRM | Aceptar_Click | [CMXsrv_expcce_gen_dcc](#cmxsrv_expcce_gen_dcc) | ACMXPAIS, DCC, CCE |
| CCE00203.FRM | Aceptar_Click | [CMXsrv_expcce_grb_cnd](#cmxsrv_expcce_grb_cnd) | CCE_ADI, ACCECRSE, CRSE, CCE, ACCE_ADI, ACCECND |
| CCE00203.FRM | fld_cce_fec_vto_LostFocus | [CMXsrv_util_det_habil](#cmxsrv_util_det_habil) | ACMXFERIADO |
| CCE00203.FRM | Form_Activate | [CMXsrv_expcce_lee_cnd](#cmxsrv_expcce_lee_cnd) | CCE_ADI, ACCECRSE, CRSE, CCE, ACCE_ADI, ACCECND |
| CCE00203.FRM | Form_Activate | [CMXsrv_expcce_trd_cnd](#cmxsrv_expcce_trd_cnd) | ACMXFORPAG, ACMXVIATPT, ACMXMAXCCE, ACMXCNFCCE, ACMXMONEDA, CCE, ACMXCLACOM, ACMXFDESDE, ACMXRCBCCE, ACCECND |
| CCE00204.FRM | ELIMINAR_Click | [CMXsrv_expcce_del_dcc](#cmxsrv_expcce_del_dcc) | DCC, CCE, ACCEDCC |
| CCE00204.FRM | Form_Activate | [CMXsrv_expcce_bus_dcc](#cmxsrv_expcce_bus_dcc) | DCC, CCE, ACCEDCC |
| CCE00205.FRM | Aceptar_Click | [CMXsrv_expcce_grb_dcc](#cmxsrv_expcce_grb_dcc) | DCC, CCE, ACCEDCC |
| CCE00205.FRM | Form_Activate | [CMXsrv_expcce_lee_dcc](#cmxsrv_expcce_lee_dcc) | DCC, CCE, ACCEDCC |
| CCE00301.FRM | Aceptar_Click | [CMXsrv_expcce_lee_cce](#cmxsrv_expcce_lee_cce) | ACMXPAIS, COR, tbl_User, CCE, ACMXSUCSAL, CLN |
| CCE00301.FRM | buscar_Click | [CMXsrv_expcce_bus_cce](#cmxsrv_expcce_bus_cce) | CCE |
| CCE00301.FRM | fld_aux_cod_bn1_lostfocus | [CMXsrv_expcce_lee_cln](#cmxsrv_expcce_lee_cln) | CLN |
| CCE00301.FRM | proximo_Click | [CMXsrv_expcce_bus_cce](#cmxsrv_expcce_bus_cce) | CCE |
| CCE00401.FRM | Aceptar_Click | [CMXsrv_expcce_mdf_cce](#cmxsrv_expcce_mdf_cce) | COR, ACCECTP, ACCEBCO, CCE_ADI, ACCECRSE, DAC, DCC, CRSE, CCE, ACCE_ADI, NGE, COL, ACCEDCC, ACCECND |
| CCE00401.FRM | Cancelar_Click | [CMXsrv_expcce_can_mdf](#cmxsrv_expcce_can_mdf) | ACCECTP, ACCEBCO, ACCEDCC, ACCECND |
| CCE00401.FRM | fld_cce_cod_bn1_LostFocus | [CMXsrv_expcce_lee_cln](#cmxsrv_expcce_lee_cln) | CLN |
| CCE00401.FRM | fld_cce_cod_ems_LostFocus | [CMXsrv_expcce_lee_cor](#cmxsrv_expcce_lee_cor) | ACMXPAIS, COR |
| CCE00401.FRM | Form_Activate | [CMXsrv_expcce_lee_mdf](#cmxsrv_expcce_lee_mdf) | ACMXSUCSAL, COR, CCE, CLN |
| CCE00501.FRM | Aceptar_Click | [CMXsrv_expcce_cnf_cce](#cmxsrv_expcce_cnf_cce) | COR, CCE, CLN |
| CCE00501.FRM | Aceptar_Click | [CMXsrv_expcce_grb_afin](#cmxsrv_expcce_grb_afin) | AFIN |
| CCE00501.FRM | Form_Activate | [CMXsrv_expcce_lee_cnf](#cmxsrv_expcce_lee_cnf) | ACMXFORPAG, COR, ACMXMONEDA, CCE, CLN |
| CCE00501.FRM | Form_Activate | [CMXsrv_expcce_lee_afin](#cmxsrv_expcce_lee_afin) | CCE, AFIN |
| CCE00701.FRM | Aceptar_Click | [CMXsrv_expcce_trp_cce](#cmxsrv_expcce_trp_cce) | COR, CCE |
| CCE00701.FRM | fld_cce_bco_dst_LostFocus | [CMXsrv_expcce_lee_cor](#cmxsrv_expcce_lee_cor) | ACMXPAIS, COR |
| CCE00701.FRM | Form_Activate | [CMXsrv_expcce_lee_trp](#cmxsrv_expcce_lee_trp) | CCE |
| CCE00801.FRM | Form_Activate | [CMXsrv_expcce_bus_evc](#cmxsrv_expcce_bus_evc) | EVC, CCE, NGE |
| CCE00801.FRM | proximo_Click | [CMXsrv_expcce_bus_evc](#cmxsrv_expcce_bus_evc) | EVC, CCE, NGE |
| CCE00801.FRM | reversar_Click | [CMXsrv_expcce_rev_cce](#cmxsrv_expcce_rev_cce) | COR, TAS, ACMXIMPUES, LTR, DCN, EVC, RET, CUO, EVO, TRSD, DSN, CCE, NGE, PUCBCX10, COD, CNO, COM, DAC, EVE, CAN, COL, AFIN, ORG, DTN, EVR |
| CCE00802.FRM | Form_Activate | [CMXsrv_expcce_lee_evc](#cmxsrv_expcce_lee_evc) | ACMXFORPAG, ACMXMONEDA, CCE, NGE, EVC, ACMXSUCSAL, ACMXTIPEVE |
| CCEAVIRE.FRM | aceptar_Click | [CMXsrv_expcce_avs_rem1](#cmxsrv_expcce_avs_rem1) | ACMXFORPAG, COR, CCB, NGEB, ACMXMONEDA, LTR, CCE, DCN, NGE, ACMXPAISES, CLN |
| COR00906.FRM | buscar_Click | [CMXsrv_busc_plz](#cmxsrv_busc_plz) | ACMXPLAZAS, comex..ACMXPLAZAS |
| COR00906.FRM | fld_cor_cod_plz_Lostfocus | [CMXsrv_lee_plz](#cmxsrv_lee_plz) | ACMXPLAZAS |
| COR00906.FRM | proximos_Click | [CMXsrv_busc_plz](#cmxsrv_busc_plz) | ACMXPLAZAS, comex..ACMXPLAZAS |
| COR00907.FRM | buscar_Click | [CMXsrv_cor_busc_pais](#cmxsrv_cor_busc_pais) | ACMXPAIS |
| COR00907.FRM | fld_cor_cod_pais_LostFocus | [CMXsrv_cor_lee_pais](#cmxsrv_cor_lee_pais) | comex..ACMXPAIS |
| COR00907.FRM | proximos_Click | [CMXsrv_cor_busc_pais](#cmxsrv_cor_busc_pais) | ACMXPAIS |
| CRD00602.FRM | Aceptar_Click | [CMXsrv_expcce_lee_cor](#cmxsrv_expcce_lee_cor) | ACMXPAIS, COR |
| CRD00602.FRM | buscar_Click | [CMXsrv_expcce_bus_cor](#cmxsrv_expcce_bus_cor) | COR |
| CRD00602.FRM | Command1_Click | [CMXsrv_expcce_bus_cor](#cmxsrv_expcce_bus_cor) | COR |
| CRD00602.FRM | proximos_Click | [CMXsrv_expcce_bus_cor](#cmxsrv_expcce_bus_cor) | COR |
| GRL00101.FRM | enviar_Click | [CMXsrv_expcce_swf_sel](#cmxsrv_expcce_swf_sel) | switxt, switxt1 |
| PREFER.FRM | Form_Load | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |  |

---

## expdex
<a name="expdex"></a>

| **Archivo (Frame)** | **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** |
|--------------------|-------------|-----------------------------|----------------------|
| DEX00101.FRM | form_activate | [CMXsrv_expcbe_lee_prm](#cmxsrv_expcbe_lee_prm) | ACMXPRMGRL |
| DEX00101.FRM | form_activate | [CMXsrv_dex_lee_dex](#cmxsrv_dex_lee_dex) | ACMXSUCSAL, DEX, CLN, ACMXADUANA |
| DEX00101.FRM | Mdexeli_Click | [CMXsrv_dex_eli_dex](#cmxsrv_dex_eli_dex) | DEX |
| DEX00102.FRM | ACEPTAR_Click | [CMXsrv_dex_act_dex](#cmxsrv_dex_act_dex) | DEX |
| DEX00102.FRM | fld_dex_dia_plz_max_LostFocus | [CMXsrv_expdex_cal_fec](#cmxsrv_expdex_cal_fec) |  |
| DEX00102.FRM | fld_dex_fec_acep_LostFocus | [CMXsrv_expdex_cal_fec](#cmxsrv_expdex_cal_fec) |  |
| DEX00102.FRM | fld_dex_rut_exp_LostFocus | [CMXsrv_dex_lee_cli](#cmxsrv_dex_lee_cli) | CLN |
| DEX00102.FRM | FORM_Load | [CMXsrv_dex_lee_dex](#cmxsrv_dex_lee_dex) | ACMXSUCSAL, DEX, CLN, ACMXADUANA |
| DEX00103.FRM | Buscar_Click | [CMXsrv_dex_bus_dex](#cmxsrv_dex_bus_dex) | DEX |
| DEX00103.FRM | fld_dex_rut_exp_LostFocus | [CMXsrv_dex_lee_cli](#cmxsrv_dex_lee_cli) | CLN |
| PREFER.FRM | FORM_Load | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |  |
| RESPALD2.FRM | ACEPTAR_Click | [CMXsrv_dex_act_dex](#cmxsrv_dex_act_dex) | DEX |
| RESPALD2.FRM | fld_dex_rut_exp_LostFocus | [CMXsrv_dex_lee_cli](#cmxsrv_dex_lee_cli) | CLN |
| RESPALD2.FRM | FORM_Load | [CMXsrv_dex_lee_dex](#cmxsrv_dex_lee_dex) | ACMXSUCSAL, DEX, CLN, ACMXADUANA |
| RESPALDO.FRM | COMELIMINAR_Click | [CMXsrv_dex_eli_dex](#cmxsrv_dex_eli_dex) | DEX |
| RESPALDO.FRM | Form_Activate | [CMXsrv_dex_lee_dex](#cmxsrv_dex_lee_dex) | ACMXSUCSAL, DEX, CLN, ACMXADUANA |

---

## EXPNEG
<a name="expneg"></a>

| **Archivo (Frame)** | **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** |
|--------------------|-------------|-----------------------------|----------------------|
| CBE00601.FRM | Form_Activate | [CMXsrv_expcbe_bus_evz](#cmxsrv_expcbe_bus_evz) | EVZ, CBE |
| CBE00601.FRM | Proximo_Click | [CMXsrv_expcbe_bus_evz](#cmxsrv_expcbe_bus_evz) | EVZ, CBE |
| CBE00601.FRM | Reversar_Click | [CMXsrv_expcbe_rev_cbe](#cmxsrv_expcbe_rev_cbe) | EVL, ACMXDESEMB, COR, ORG, ACMXIMPUES, ACMXPRMGRL, EVZ, CBE, TRSD, ACMXPRMEXP, COM, EVR, CTZ, DTN, OPREC, RET, PUCBCX10 |
| CBE00602.FRM | Form_Activate | [CMXsrv_expcbe_lee_evz](#cmxsrv_expcbe_lee_evz) | ACMXDESEMB, COR, ACMXPGOCBE, EVZ, CBE, ACMXMONEDA, ACMXTIPEVE, ACMXSUCSAL |
| CCE00601.FRM | Form_Activate | [CMXsrv_expcce_lee_bas](#cmxsrv_expcce_lee_bas) | ACMXMONEDA, CCE, ACMXFORPAG |
| CCE00601.FRM | Form_Activate | [CMXsrv_expcce_lee_neg](#cmxsrv_expcce_lee_neg) | COR, ACMXVIATPT, ACMXSUCSAL, ACMXDISNEG, ACMXMONEDA, ACMXCLACOM, NGE, ACMXPAIS, CLN, ACMXTPONEG |
| CCE00601.FRM | Mccealznge_click | [CMXsrv_expcce_alz_dis](#cmxsrv_expcce_alz_dis) | COL, CCE, NGE |
| CCE00601.FRM | Mcceanlnge_click | [CMXsrv_expcce_anl_neg](#cmxsrv_expcce_anl_neg) | CCE, NGE |
| CCE00601.FRM | Mccectbnge_Click | [CMXsrv_expcce_ctb_neg](#cmxsrv_expcce_ctb_neg) | COR, LTR, CCE, NGE, AFIN |
| CCE00601.FRM | Mccedelnge_Click | [CMXsrv_expcce_del_neg](#cmxsrv_expcce_del_neg) | CRSN, COD, COM, NGEB, LTR, DSN, CCE, DCN, NGE, EVC, AFIN |
| CCE00601.FRM | Mccevalnge_click | [CMXsrv_expcce_val_neg](#cmxsrv_expcce_val_neg) | NGEB, LTR, DCC, warnmsg, CCE, DCN, NGE, COL, AFIN |
| CCE00601.FRM | Mtel742_Click | [CMXsrv_expcce_swf_sel](#cmxsrv_expcce_swf_sel) | switxt, switxt1 |
| CCE00801.FRM | Form_Activate | [CMXsrv_expcce_bus_evc](#cmxsrv_expcce_bus_evc) | EVC, CCE, NGE |
| CCE00801.FRM | Proximo_Click | [CMXsrv_expcce_bus_evc](#cmxsrv_expcce_bus_evc) | EVC, CCE, NGE |
| CCE00801.FRM | Reversar_Click | [CMXsrv_expcce_rev_cce](#cmxsrv_expcce_rev_cce) | COR, TAS, ACMXIMPUES, LTR, DCN, EVC, RET, CUO, EVO, TRSD, DSN, CCE, NGE, PUCBCX10, COD, CNO, COM, DAC, EVE, CAN, COL, AFIN, ORG, DTN, EVR |
| CCE00802.FRM | Form_Activate | [CMXsrv_expcce_lee_evc](#cmxsrv_expcce_lee_evc) | ACMXFORPAG, ACMXMONEDA, CCE, NGE, EVC, ACMXSUCSAL, ACMXTIPEVE |
| CCE00901.FRM | aceptar_Click | [CMXsrv_expcce_grb_neg](#cmxsrv_expcce_grb_neg) | CRSN, CCE, NGEB, NGE |
| CCE00901.FRM | aceptar_Click | [CMXsrv_expcce_gen_dcn](#cmxsrv_expcce_gen_dcn) | DCC, CCE, DCN, NGE |
| CCE00901.FRM | aceptar_Click | [CMXsrv_expcce_grb_afin](#cmxsrv_expcce_grb_afin) | AFIN |
| CCE00901.FRM | fld_cce_cod_exp_nge_LostFocus | [CMXsrv_expcce_lee_cln](#cmxsrv_expcce_lee_cln) | CLN |
| CCE00901.FRM | fld_cce_cod_pag_nge_LostFocus | [CMXsrv_expcce_lee_cor](#cmxsrv_expcce_lee_cor) | ACMXPAIS, COR |
| CCE00901.FRM | fld_cce_cod_rmb_nge_LostFocus | [CMXsrv_expcce_lee_cor](#cmxsrv_expcce_lee_cor) | ACMXPAIS, COR |
| CCE00901.FRM | fld_cce_ins_rem1_nge_GotFocus | [CMXsrv_expcce_avs_rem5](#cmxsrv_expcce_avs_rem5) | COR, ACMXCRDREMTXT, ACMXMONEDA, CCE, NGE, ACMXPAISES, CCO |
| CCE00901.FRM | Form_Load | [CMXsrv_expcce_lee_nge](#cmxsrv_expcce_lee_nge) | COR, CRSN, NGEB, CCE, NGE, ACMXPAIS, CLN |
| CCE00901.FRM | Form_Load | [CMXsrv_expcce_trd_nge](#cmxsrv_expcce_trd_nge) | ACMXVIATPT, ACMXRCBCCE, ACMXMONEDA, ACMXCLACOM, NGE, ACMXTPONEG |
| CCE00901.FRM | Form_Load | [CMXsrv_expcce_ini_neg](#cmxsrv_expcce_ini_neg) | ACMXPAIS, COR, ACMXVIATPT, CCB, ACMXMONEDA, CRSE, CCE, ACMXCLACOM, NGE, ACMXSUCSAL, CLN, ACMXTPONEG |
| CCE00901.FRM | Form_Load | [CMXsrv_expcce_lee_afin](#cmxsrv_expcce_lee_afin) | CCE, AFIN |
| CCE00901.FRM | lee_bco | [CMXsrv_expcce_lee_cor](#cmxsrv_expcce_lee_cor) | ACMXPAIS, COR |
| CCE00902.FRM | ELIMINAR_Click | [CMXsrv_expcce_del_dcn](#cmxsrv_expcce_del_dcn) | CCE, DCN, NGE |
| CCE00902.FRM | Form_Activate | [CMXsrv_expcce_bus_dcn](#cmxsrv_expcce_bus_dcn) | DCN, NGE |
| CCE00903.FRM | Aceptar_Click | [CMXsrv_expcce_grb_dcn](#cmxsrv_expcce_grb_dcn) | CCE, DCN, NGE |
| CCE00903.FRM | Form_Load | [CMXsrv_expcce_lee_dcn](#cmxsrv_expcce_lee_dcn) | DCC, DCN, NGE |
| CCE00904.FRM | ELIMINAR_Click | [CMXsrv_expcce_del_ltr](#cmxsrv_expcce_del_ltr) | LTR, CCE, NGE |
| CCE00904.FRM | Form_Activate | [CMXsrv_expcce_bus_ltr](#cmxsrv_expcce_bus_ltr) | LTR, NGE |
| CCE00905.FRM | Aceptar_Click | [CMXsrv_expcce_grb_ltr](#cmxsrv_expcce_grb_ltr) | LTR, CCE, NGE |
| CCE00905.FRM | Form_Load | [CMXsrv_expcce_lee_ltr](#cmxsrv_expcce_lee_ltr) | LTR, CCE, NGE |
| CCE00906.FRM | ELIMINAR_Click | [CMXsrv_expcce_del_dsn](#cmxsrv_expcce_del_dsn) | DSN, CCE, NGE |
| CCE00906.FRM | Form_Activate | [CMXsrv_expcce_gen_dsn](#cmxsrv_expcce_gen_dsn) | DCC, DSN, CCE, DCN, NGE |
| CCE00906.FRM | Form_Activate | [CMXsrv_expcce_bus_dsn](#cmxsrv_expcce_bus_dsn) | DSN, NGE |
| CCE00906.FRM | Salir_Click | [CMXsrv_expcce_chk_dsn](#cmxsrv_expcce_chk_dsn) | DSN, CCE, NGE |
| CCE00907.FRM | Aceptar_Click | [CMXsrv_expcce_grb_dsn](#cmxsrv_expcce_grb_dsn) | DSN, CCE, NGE |
| CCE00907.FRM | Form_Load | [CMXsrv_expcce_lee_dsn](#cmxsrv_expcce_lee_dsn) | DSN, NGE |
| CCE01001.FRM | buscar_Click | [CMXsrv_expcce_bus_neg](#cmxsrv_expcce_bus_neg) | CCE, NGE |
| CCE01001.FRM | Proximas_Click | [CMXsrv_expcce_bus_neg](#cmxsrv_expcce_bus_neg) | CCE, NGE |
| CCE01201.FRM | aceptar_Click | [CMXsrv_expcce_pgo_neg](#cmxsrv_expcce_pgo_neg) | ACMXDESEMB, COR, vig_cmx, ACMXIMPUES, COD, ACMXPRMEXP, COM, CCE, tbl_User, NGE, CLN, RET |
| CCE01201.FRM | aceptar_Click | [CMXsrv_expcce_grb_afin](#cmxsrv_expcce_grb_afin) | AFIN |
| CCE01201.FRM | fld_cce_cod_exp_nge_LostFocus | [CMXsrv_expcce_lee_cln](#cmxsrv_expcce_lee_cln) | CLN |
| CCE01201.FRM | fld_cce_cod_rmb_nge_LostFocus | [CMXsrv_expcce_lee_cor](#cmxsrv_expcce_lee_cor) | ACMXPAIS, COR |
| CCE01201.FRM | Form_Load | [CMXsrv_expcce_lee_pgo](#cmxsrv_expcce_lee_pgo) | ACMXDESEMB, COR, ACMXPRMEXP, ACMXMONEDA, CCE, NGE, CLN |
| CCE01201.FRM | Form_Load | [CMXsrv_expcce_lee_afin](#cmxsrv_expcce_lee_afin) | CCE, AFIN |
| CCE01201.FRM | lee_bco | [CMXsrv_expcce_lee_cor](#cmxsrv_expcce_lee_cor) | ACMXPAIS, COR |
| CCEAVIRE.FRM | aceptar_Click | [CMXsrv_avi_dat_cou](#cmxsrv_avi_dat_cou) |  |
| CCEAVIRE.FRM | aceptar_Click | [CMXsrv_expcce_lee_nge](#cmxsrv_expcce_lee_nge) | COR, CRSN, NGEB, CCE, NGE, ACMXPAIS, CLN |
| CCEAVIRE.FRM | aceptar_Click | [CMXsrv_expcce_avs_rem1](#cmxsrv_expcce_avs_rem1) | ACMXFORPAG, COR, CCB, NGEB, ACMXMONEDA, LTR, CCE, DCN, NGE, ACMXPAISES, CLN |
| CCEAVIRE.FRM | aceptar_Click | [CMXsrv_expcce_avs_rem3](#cmxsrv_expcce_avs_rem3) | LTR, NGE |
| CCEAVIRE.FRM | imprime_esp | [CMXsrv_expcce_avs_rem2](#cmxsrv_expcce_avs_rem2) | DCN |
| CCEAVIRE.FRM | imprime_esp | [CMXsrv_expcce_avs_rem4](#cmxsrv_expcce_avs_rem4) | DSN |
| CCEAVIRE.FRM | imprime_esp | [CMXsrv_expcbe_avs_rem4](#cmxsrv_expcbe_avs_rem4) | ACMXREMFESPMSG, ACMXREMFINGMSG |
| CCEAVIRE.FRM | imprime_ing | [CMXsrv_expcce_avs_rem2](#cmxsrv_expcce_avs_rem2) | DCN |
| CCEAVIRE.FRM | imprime_ing | [CMXsrv_expcce_avs_rem4](#cmxsrv_expcce_avs_rem4) | DSN |
| CCEAVIRE.FRM | imprime_ing | [CMXsrv_expcbe_avs_rem4](#cmxsrv_expcbe_avs_rem4) | ACMXREMFESPMSG, ACMXREMFINGMSG |
| CRD00602.FRM | aceptar_Click | [CMXsrv_expcce_lee_cor](#cmxsrv_expcce_lee_cor) | ACMXPAIS, COR |
| CRD00602.FRM | buscar_Click | [CMXsrv_expcce_bus_cor](#cmxsrv_expcce_bus_cor) | COR |
| CRD00602.FRM | proximos_Click | [CMXsrv_expcce_bus_cor](#cmxsrv_expcce_bus_cor) | COR |
| GRL00101.FRM | enviar_Click | [CMXsrv_expcce_swf_sel](#cmxsrv_expcce_swf_sel) | switxt, switxt1 |
| PREFER.FRM | Form_Load | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |  |

---

## expret
<a name="expret"></a>

| **Archivo (Frame)** | **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** |
|--------------------|-------------|-----------------------------|----------------------|
| COR00906.FRM | buscar_Click | [CMXsrv_busc_plz](#cmxsrv_busc_plz) | ACMXPLAZAS, comex..ACMXPLAZAS |
| COR00906.FRM | fld_cor_cod_plz_Lostfocus | [CMXsrv_lee_plz](#cmxsrv_lee_plz) | ACMXPLAZAS |
| COR00906.FRM | proximos_Click | [CMXsrv_busc_plz](#cmxsrv_busc_plz) | ACMXPLAZAS, comex..ACMXPLAZAS |
| COR00907.FRM | buscar_Click | [CMXsrv_cor_busc_pais](#cmxsrv_cor_busc_pais) | ACMXPAIS |
| COR00907.FRM | fld_cor_cod_pais_LostFocus | [CMXsrv_cor_lee_pais](#cmxsrv_cor_lee_pais) | comex..ACMXPAIS |
| COR00907.FRM | proximos_Click | [CMXsrv_cor_busc_pais](#cmxsrv_cor_busc_pais) | ACMXPAIS |
| CRD00602.FRM | Aceptar_Click | [CMXsrv_expcbe_lee_cor](#cmxsrv_expcbe_lee_cor) | ACMXPAIS, COR |
| CRD00602.FRM | buscar_Click | [CMXsrv_expcbe_bus_cor](#cmxsrv_expcbe_bus_cor) | COR |
| CRD00602.FRM | proximos_Click | [CMXsrv_expcbe_bus_cor](#cmxsrv_expcbe_bus_cor) | COR |
| GRL00101.FRM | Command2_Click | [CMXsrv_expret_swf_sel](#cmxsrv_expret_swf_sel) | DTN, ACMXPRMEXP, switxt, switxt1 |
| PREFER.FRM | Form_Load | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |  |
| RET00101.FRM | Form_Activate | [CMXsrv_cmx_busc_suc_usu](#cmxsrv_cmx_busc_suc_usu) | master..sysprocesses, tbl_User |
| RET00101.FRM | Form_Activate | [CMXsrv_expret_lee_ret](#cmxsrv_expret_lee_ret) | DTN, ACMXPRMEXP, ACMXMONEDA, ACMXSUCSAL, CLN, RET |
| RET00101.FRM | Form_Load | [CMXsrv_expret_lee_prm](#cmxsrv_expret_lee_prm) | ACMXPRMGRL, ACMXPRMEXP |
| RET00101.FRM | M_cgyc_Click | [CMXsrv_expret_avs_cyg1](#cmxsrv_expret_avs_cyg1) | ACMXDESEMB, ASND, ACMXIMPUES, ACMXPRMGRL, COM, TRSD, EVR, CLN, ACMXESPECI, RET |
| RET00101.FRM | M_cgyc_Click | [CMXsrv_expret_avs_cyg2](#cmxsrv_expret_avs_cyg2) | ASND, ACMXIMPUES, ACMXPRMGRL, EVR, RET |
| RET00101.FRM | mavisliq_Click | [CMXsrv_expret_avs_liq1](#cmxsrv_expret_avs_liq1) | DTN, ACMXMONEDA, ACMXSUCSAL, CLN, ACMXESPECI, RET |
| RET00101.FRM | mavisliq_Click | [CMXsrv_expret_avs_liq2](#cmxsrv_expret_avs_liq2) | ORG, RET |
| RET00101.FRM | mavisliq_Click | [CMXsrv_expret_avs_liq3](#cmxsrv_expret_avs_liq3) | DTN, ACMXPRMEXP, RET |
| RET00101.FRM | Mcbectb_Click | [CMXsrv_expret_val_ret](#cmxsrv_expret_val_ret) | ACMXDESEMB, ORG, COR, ACMXIMPUES, ACMXPRMGRL, CCL, ACMXPRMEXP, ACMXMONEDAFEC, COM, tbl_User, warnmsg, DTN, CLN, RET |
| RET00101.FRM | Mcbectb_Click | [CMXsrv_expret_sum_dtn_mn](#cmxsrv_expret_sum_dtn_mn) | DTN, ACMXMONEDAFEC, RET, ACMXPRMENL |
| RET00101.FRM | Mcbectb_Click | [CMXsrv_expret_ctb_ing](#cmxsrv_expret_ctb_ing) | ACMXDESEMB, ASND, PLV, ACMXPRMGRL, CCL, ACMXPRMEXP, PLI, tbl_User, DTN, CLN, RET |
| RET00101.FRM | Mcbedel_Click | [CMXsrv_expret_del_ret](#cmxsrv_expret_del_ret) | ORG, COD, COM, DTN, RET |
| RET00101.FRM | Mliqctb_Click | [CMXsrv_expret_avs_adm1](#cmxsrv_expret_avs_adm1) | ACMXSUCSAL, ACMXMONEDA, CLN, RET |
| RET00101.FRM | Mliqctb_Click | [CMXsrv_expret_avs_adm2](#cmxsrv_expret_avs_adm2) | ORG, ACMXPRMEXP, RET |
| RET00101.FRM | Mliqctb_Click | [CMXsrv_expret_avs_adm3](#cmxsrv_expret_avs_adm3) | DTN, ACMXPRMEXP, RET |
| RET00101.FRM | Mvalid_Click | [CMXsrv_expret_val_ret](#cmxsrv_expret_val_ret) | ACMXDESEMB, ORG, COR, ACMXIMPUES, ACMXPRMGRL, CCL, ACMXPRMEXP, ACMXMONEDAFEC, COM, tbl_User, warnmsg, DTN, CLN, RET |
| RET00102.FRM | ACEPTAR_Click | [CMXsrv_expret_act_tpo_cbo](#cmxsrv_expret_act_tpo_cbo) | RET |
| RET00102.FRM | ACEPTAR_Click | [CMXsrv_expret_val_ret](#cmxsrv_expret_val_ret) | ACMXDESEMB, ORG, COR, ACMXIMPUES, ACMXPRMGRL, CCL, ACMXPRMEXP, ACMXMONEDAFEC, COM, tbl_User, warnmsg, DTN, CLN, RET |
| RET00201.FRM | ACEPTAR_Click | [CMXsrv_expret_cre_ret](#cmxsrv_expret_cre_ret) | RET |
| RET00201.FRM | ACEPTAR_Click | [CMXsrv_expret_grb_det](#cmxsrv_expret_grb_det) | CLN, tbl_User, RET |
| RET00201.FRM | fld_ret_mon_ret_LostFocus | [CMXsrv_expret_tpo_cbo](#cmxsrv_expret_tpo_cbo) | ACMXMONEDAFEC |
| RET00201.FRM | fld_ret_rut_cli_LostFocus | [CMXsrv_expret_lee_cln](#cmxsrv_expret_lee_cln) | CLN |
| RET00201.FRM | Form_Load | [CMXsrv_expret_lee_det](#cmxsrv_expret_lee_det) | ACMXSUCSAL, ACMXMONEDA, CLN, RET |
| RET00301.FRM | ELIMINAR_Click | [CMXsrv_expret_del_org](#cmxsrv_expret_del_org) | ORG, RET |
| RET00301.FRM | Form_Activate | [CMXsrv_expret_bus_org](#cmxsrv_expret_bus_org) | ORG, RET |
| RET00401.FRM | ACEPTAR_Click | [CMXsrv_expret_grb_org](#cmxsrv_expret_grb_org) | ACMXDESEMB, ORG, ACMXPLNCTAN, ACMXSRVEXT, ACMXPLNCTAX, RET |
| RET00401.FRM | Form_Activate | [CMXsrv_expret_mto_org](#cmxsrv_expret_mto_org) | ORG, RET |
| RET00401.FRM | Form_Activate | [CMXsrv_expret_lee_org](#cmxsrv_expret_lee_org) | ACMXDESEMB, ORG, COR, ACMXTPODOC, ACMXPAIS |
| RET00401.FRM | valida_vigente | [CMXsrv_vig_lee_cta](#cmxsrv_vig_lee_cta) | ACMXPLNCTAN, ACMXDESEMB, ACMXPLNCTAX |
| RET00501.FRM | ELIMINAR_Click | [CMXsrv_expret_del_dtn](#cmxsrv_expret_del_dtn) | DTN, RET |
| RET00501.FRM | emitir_Click | [CMXsrv_expret_swf_sel](#cmxsrv_expret_swf_sel) | DTN, ACMXPRMEXP, switxt, switxt1 |
| RET00501.FRM | Form_Activate | [CMXsrv_expret_bus_dtn](#cmxsrv_expret_bus_dtn) | DTN, RET |
| RET00601.FRM | ACEPTAR_Click | [CMXsrv_expret_grb_dtn](#cmxsrv_expret_grb_dtn) | ACMXDESEMB, ACMXPRMGRL, CCL, ACMXPRMEXP, DTN, RET |
| RET00601.FRM | fld_ret_cod_ben_LostFocus | [CMXsrv_expret_lee_cln](#cmxsrv_expret_lee_cln) | CLN |
| RET00601.FRM | fld_ret_mto_arb_LostFocus | [CMXsrv_expret_cal_arb](#cmxsrv_expret_cal_arb) | ACMXPRMGRL, ACMXMONEDA |
| RET00601.FRM | fld_ret_mto_ben_LostFocus | [CMXsrv_expret_cal_arb](#cmxsrv_expret_cal_arb) | ACMXPRMGRL, ACMXMONEDA |
| RET00601.FRM | fld_ret_par_ben_LostFocus | [CMXsrv_expret_cal_arb](#cmxsrv_expret_cal_arb) | ACMXPRMGRL, ACMXMONEDA |
| RET00601.FRM | Form_Activate | [CMXsrv_expret_mto_dtn](#cmxsrv_expret_mto_dtn) | DTN, COM, RET, ACMXIMPUES |
| RET00601.FRM | Form_Load | [CMXsrv_expret_lee_dtn](#cmxsrv_expret_lee_dtn) | ACMXPAIS, ACMXDESEMB, COR, DTN, ACMXMONEDA, APUCCODOPECMB, ACMXSUCSAL |
| RET00601.FRM | Form_Load | [CMXsrv_expret_lee_cln](#cmxsrv_expret_lee_cln) | CLN |
| RET00701.FRM | buscar_Click | [CMXsrv_expret_bus_ret](#cmxsrv_expret_bus_ret) | RET |
| RET00701.FRM | fld_ret_rut_cli_LostFocus | [CMXsrv_expret_lee_cln](#cmxsrv_expret_lee_cln) | CLN |
| RET00701.FRM | proxima_Click | [CMXsrv_expret_bus_ret](#cmxsrv_expret_bus_ret) | RET |
| RET00801.FRM | Command1_Click | [CMXsrv_expret_bus_evr](#cmxsrv_expret_bus_evr) | EVR, RET |
| RET00801.FRM | Form_Activate | [CMXsrv_expret_bus_evr](#cmxsrv_expret_bus_evr) | EVR, RET |
| RET00801.FRM | proximo_Click | [CMXsrv_expret_bus_evr](#cmxsrv_expret_bus_evr) | EVR, RET |
| RET00801.FRM | reversar_Click | [CMXsrv_expret_rev_ret](#cmxsrv_expret_rev_ret) | ORG, DTN, PLV, ACMXPRMEXP, PLI, TRSD, EVR, RET |
| RET00802.FRM | Form_Load | [CMXsrv_expret_lee_evr](#cmxsrv_expret_lee_evr) | ACMXTIPEVE, EVR, ACMXSUCSAL |

---

## ADMIN
<a name="admin"></a>

| **Archivo (Frame)** | **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** |
|--------------------|-------------|-----------------------------|----------------------|
| ADM00201.FRM | COMMAND4_Click | [CMXsrv_finadm_imod_desti](#cmxsrv_finadm_imod_desti) | TIP |
| ADM00201.FRM | Form_Load | [CMXsrv_finadm_cons_dtip](#cmxsrv_finadm_cons_dtip) | TIP |
| ADM00202.FRM | Command1_Click | [CMXsrv_finadm_imod_ectb](#cmxsrv_finadm_imod_ectb) | TIP |
| ADM00202.FRM | Command2_Click | [CMXsrv_finadm_eli_tipop](#cmxsrv_finadm_eli_tipop) | TIP, TIP_CTA |
| ADM00202.FRM | Form_Load | [CMXsrv_finadm_cons_ectb](#cmxsrv_finadm_cons_ectb) | TIP |
| ADM00203.FRM | COMMAND3_Click | [CMXsrv_finadm_eli_tipop](#cmxsrv_finadm_eli_tipop) | TIP, TIP_CTA |
| ADM00203.FRM | COMMAND4_Click | [CMXsrv_finadm_imod_itip](#cmxsrv_finadm_imod_itip) | TIP |
| ADM00203.FRM | Form_Load | [CMXsrv_finadm_cons_itip](#cmxsrv_finadm_cons_itip) | TIP |
| ADM00204.FRM | Form_Activate | [CMXsrv_finadm_lee_tipop](#cmxsrv_finadm_lee_tipop) | TIP, ACMXPLAZO, ACMXPROCMX, ACMXMB1 |
| ADM00204.FRM | Form_Load | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |  |
| ADM00204.FRM | Mdel_Click | [CMXsrv_finadm_eli_tipop](#cmxsrv_finadm_eli_tipop) | TIP, TIP_CTA |
| ADM00204.FRM | Mval_Click | [CMXsrv_finadm_val_tipop](#cmxsrv_finadm_val_tipop) | APEPROR, TIP, TAS, CUO, ACMXPLNCTAN, ACMXMONEDAFEC, PANCTL, ACLNCBCABCI, ACMXPLNCTAX, TIP_CTA, ACMXMONEDA, warnmsg, EVE, ACMXSUCSAL, PANVTO, ACMXINTEREFEC, COL, PANMOR |
| ADM00205.FRM | buscar_Click | [CMXsrv_finadm_bus_tipope](#cmxsrv_finadm_bus_tipope) | TIP |
| ADM00205.FRM | proximas_Click | [CMXsrv_finadm_bus_tipope](#cmxsrv_finadm_bus_tipope) | TIP |

---

## COL_NEG
<a name="col_neg"></a>

| **Archivo (Frame)** | **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** |
|--------------------|-------------|-----------------------------|----------------------|
| COL00102.FRM | CANCELAR_Click | [CMXsrv_busc_tip_tas](#cmxsrv_busc_tip_tas) | CRD |
| COL00102.FRM | ELIMINAR_Click | [CMXsrv_fincol_ecuo](#cmxsrv_fincol_ecuo) | CUO_REN, COL, CUO |
| COL00102.FRM | Form_Activate | [CMXsrv_fincol_cons_plnpa](#cmxsrv_fincol_cons_plnpa) | CUO_REN, COL_REN, COL, CUO |
| COL00102.FRM | Form_Load | [CMXsrv_pertas_val_display](#cmxsrv_pertas_val_display) | TAS |
| COL00103.FRM | ELIMINAR_Click | [CMXsrv_fincol_eava](#cmxsrv_fincol_eava) | DAC, AVAL, AVAL_REN, COL |
| COL00103.FRM | Form_Activate | [CMXsrv_fincol_cons_aval](#cmxsrv_fincol_cons_aval) | CRDCLON, AVAL, AVAL_REN, COL |
| COL00113.FRM | ingresar_Click | [CMXsrv_fincol_iava](#cmxsrv_fincol_iava) | AVAL, AVAL_REN, CLN, COL |
| COL00303.FRM | Form_Activate | [CMXsrv_fincol_cons_pag](#cmxsrv_fincol_cons_pag) | CAN, COL |
| COL00303.FRM | proximos_Click | [CMXsrv_fincol_cons_pag](#cmxsrv_fincol_cons_pag) | CAN, COL |
| COL00304.FRM | Form_Activate | [CMXsrv_fincol_trae_det_pag](#cmxsrv_fincol_trae_det_pag) | CAN, EVE |
| COL00403.FRM | Form_Activate | [CMXsrv_fincol_cons_pror](#cmxsrv_fincol_cons_pror) | EVE, COL |
| COL00901.FRM | Form_Activate | [CMXsrv_fincol_cons_eve](#cmxsrv_fincol_cons_eve) | EVE, COL |
| CRD00602.FRM | Aceptar_Click | [CMXsrv_icrd_lee_bco_swf](#cmxsrv_icrd_lee_bco_swf) | ACMXPAIS, COR |
| CRD00602.FRM | buscar_Click | [CMXsrv_icrd_busc_bco](#cmxsrv_icrd_busc_bco) | COR |
| CRD00602.FRM | proximo_Click | [CMXsrv_icrd_busc_bco](#cmxsrv_icrd_busc_bco) | COR |
| CRD01401.FRM | Aceptar_Click | [CMXsrv_fincol_vtocre_prov](#cmxsrv_fincol_vtocre_prov) | TIP, comex..ACMXINTEREFEC, COR, CRD, CUO, OBL, NEG, NEG_ADI, DAC, ACMXINTERE, ACMXMONEDA, ACMXINTEREFEC, AVAL, MYC, COL, CTO |
| CRD01401.FRM | Form_Load | [CMXsrv_fincol_prec_vtocre](#cmxsrv_fincol_prec_vtocre) | TIP, CRD, CNEG, NEG, COL |
| CRD02001.FRM | buscar_Click | [CMXsrv_icrd_bus_lcr_bco](#cmxsrv_icrd_bus_lcr_bco) | COR |
| CRD02001.FRM | proximo_Click | [CMXsrv_icrd_bus_lcr_bco](#cmxsrv_icrd_bus_lcr_bco) | COR |
| PREFER.FRM | Form_Load | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |  |
| PREFER.FRM | Form_Load | [CMXsrv_lee_fpro](#cmxsrv_lee_fpro) | ACMXFECPRO |

---

## INGRESO
<a name="ingreso"></a>

| **Archivo (Frame)** | **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** |
|--------------------|-------------|-----------------------------|----------------------|
| COL00102.FRM | cancelar_Click | [CMXsrv_fincol_ren_fin](#cmxsrv_fincol_ren_fin) | COL_REN, TIP, TAS, TAS_REN, EVE_REN, DAC_REN, ITA, CUO_REN, AVAL_REN, EVE, CAN_REN, COL |
| COL00102.FRM | ELIMINAR_Click | [CMXsrv_fincol_ecuo](#cmxsrv_fincol_ecuo) | CUO_REN, COL, CUO |
| COL00102.FRM | form_activate | [CMXsrv_fincol_cons_plnpa](#cmxsrv_fincol_cons_plnpa) | CUO_REN, COL_REN, COL, CUO |
| COL00103.FRM | cancelar_Click | [CMXsrv_fincol_ren_fin](#cmxsrv_fincol_ren_fin) | COL_REN, TIP, TAS, TAS_REN, EVE_REN, DAC_REN, ITA, CUO_REN, AVAL_REN, EVE, CAN_REN, COL |
| COL00103.FRM | ELIMINAR_Click | [CMXsrv_fincol_eava](#cmxsrv_fincol_eava) | DAC, AVAL, AVAL_REN, COL |
| COL00103.FRM | form_activate | [CMXsrv_fincol_cons_aval](#cmxsrv_fincol_cons_aval) | CRDCLON, AVAL, AVAL_REN, COL |
| COL00104.FRM | aceptar_Click | [CMXsrv_fincol_gmod_ctr](#cmxsrv_fincol_gmod_ctr) | TIP, CUO, OBL, CTR, CLN, COL, CTO |
| COL00104.FRM | busca_bco | [CMXsrv_icrd_lee_bco_swf](#cmxsrv_icrd_lee_bco_swf) | ACMXPAIS, COR |
| COL00104.FRM | fld_obl_bco_acr_LostFocus | [CMXsrv_fincol_lee_bco](#cmxsrv_fincol_lee_bco) | COR |
| COL00104.FRM | fld_obl_rut_acr_LostFocus | [CMXsrv_fincol_lee_cln](#cmxsrv_fincol_lee_cln) | CLN |
| COL00104.FRM | form_activate | [CMXsrv_fincol_cons_ctr](#cmxsrv_fincol_cons_ctr) | OBL, CTR |
| COL00105.FRM | aceptar_Click | [CMXsrv_fincol_ctb_oto](#cmxsrv_fincol_ctb_oto) | TIP, ACMXDESEMB, CUO, COD, vig_cmx, COL_ADI, ACMXPRMGRL, OBL, COM, MYC, ACMXMONEDA, LIB, OPE_BCI, CLN, COL, CCO |
| COL00106.FRM | Avi5_Click | [CMXsrv_icrd_dat_liq_ope](#cmxsrv_icrd_dat_liq_ope) | ACMXDESEMB, ASND, EVO, CRD, CNO, OBL, CUO, TRSD, NEG, COM, EVE, ACMXTIPEVE, CAN, COL |
| COL00106.FRM | form_activate | [CMXsrv_fincol_lee_col](#cmxsrv_fincol_lee_col) | COR, TAS, NEG_ADI, ACMXINTERE, TIP, CUO, CCL, ACMXFINVER, ACMXAPROBAC, COL_ADI, ACMXACTIVIDA, ACMXINTEREFEC, AVAL, ACMXSUCSAL, CLN, comex..ACMXINTEREFEC, COM, ACMXMONEDA, EVE, tbl_User, COL |
| COL00106.FRM | Form_Load | [CMXsrv_lee_fpro](#cmxsrv_lee_fpro) | ACMXFECPRO |
| COL00106.FRM | MCOLCOMI_CLICK | [CMXsrv_busc_cod_ope](#cmxsrv_busc_cod_ope) | TIP, COL |
| COL00106.FRM | MCOLCOMI_CLICK | [CMXsrv_col_trae_num_ope](#cmxsrv_col_trae_num_ope) | COL |
| COL00106.FRM | MCOLCONTOTOR_CLICK | [CMXsrv_busc_cod_ope](#cmxsrv_busc_cod_ope) | TIP, COL |
| COL00106.FRM | MCOLCONTOTOR_CLICK | [CMXsrv_col_trae_num_ope](#cmxsrv_col_trae_num_ope) | COL |
| COL00106.FRM | MCOLCONTOTOR_CLICK | [CMXsrv_fincol_ctb_oto](#cmxsrv_fincol_ctb_oto) | TIP, ACMXDESEMB, CUO, COD, vig_cmx, COL_ADI, ACMXPRMGRL, OBL, COM, MYC, ACMXMONEDA, LIB, OPE_BCI, CLN, COL, CCO |
| COL00106.FRM | MCOLELI_CLICK | [CMXsrv_fincol_eli_col](#cmxsrv_fincol_eli_col) | COL_REN, COL_ADI, COM, TAS_REN, DAC_REN, EVE_REN, DAC, CUO_REN, AVAL_REN, LIB, CAN_REN, COL |
| COL00106.FRM | valida | [CMXsrv_fincol_val_col](#cmxsrv_fincol_val_col) | TIP, COL, warnmsg |
| COL00107.FRM | aceptar_Click | [CMXsrv_fincol_lee_col](#cmxsrv_fincol_lee_col) | COR, TAS, NEG_ADI, ACMXINTERE, TIP, CUO, CCL, ACMXFINVER, ACMXAPROBAC, COL_ADI, ACMXACTIVIDA, ACMXINTEREFEC, AVAL, ACMXSUCSAL, CLN, comex..ACMXINTEREFEC, COM, ACMXMONEDA, EVE, tbl_User, COL |
| COL00107.FRM | buscar_Click | [CMXsrv_fincol_bsc_col](#cmxsrv_fincol_bsc_col) | TIP |
| COL00107.FRM | fld_col_tip_ope_lostfocus | [CMXsrv_fincol_lee_tip](#cmxsrv_fincol_lee_tip) | TIP |
| COL00107.FRM | PROXIMAS_Click | [CMXsrv_fincol_bsc_col](#cmxsrv_fincol_bsc_col) | TIP |
| COL00113.FRM | ingresar_Click | [CMXsrv_fincol_iava](#cmxsrv_fincol_iava) | AVAL, AVAL_REN, CLN, COL |
| COL00701.FRM | aceptar_Click | [CMXsrv_busc_cod_ope](#cmxsrv_busc_cod_ope) | TIP, COL |
| COL00701.FRM | aceptar_Click | [CMXsrv_col_trae_num_ope](#cmxsrv_col_trae_num_ope) | COL |
| COL00701.FRM | aceptar_Click | [CMXsrv_fincol_ctb_novf](#cmxsrv_fincol_ctb_novf) | CLN, COL |
| COL00701.FRM | FLD_COL_COD_CLI_LOSTFOCUS | [CMXsrv_fincol_lee_cln](#cmxsrv_fincol_lee_cln) | CLN |
| COL00701.FRM | FLD_COL_RUT_DEU_NOV_LostFocus | [CMXsrv_fincol_lee_cln](#cmxsrv_fincol_lee_cln) | CLN |
| COL00702.FRM | form_activate | [CMXsrv_fincol_cons_nov](#cmxsrv_fincol_cons_nov) | EVE, COL |
| COL00703.FRM | FLD_COL_COD_CLI_LOSTFOCUS | [CMXsrv_fincol_lee_cln](#cmxsrv_fincol_lee_cln) | CLN |
| COL00703.FRM | FLD_COL_RUT_DEU_NOV_LostFocus | [CMXsrv_fincol_lee_cln](#cmxsrv_fincol_lee_cln) | CLN |
| CRD00602.FRM | Aceptar_Click | [CMXsrv_icrd_lee_bco_swf](#cmxsrv_icrd_lee_bco_swf) | ACMXPAIS, COR |
| CRD00602.FRM | buscar_Click | [CMXsrv_icrd_busc_bco](#cmxsrv_icrd_busc_bco) | COR |
| CRD00602.FRM | proximo_Click | [CMXsrv_icrd_busc_bco](#cmxsrv_icrd_busc_bco) | COR |
| PREFER.FRM | Form_Load | [CMXsrv_cmx_get_codes](#cmxsrv_cmx_get_codes) |  |
| PREFER.FRM | Form_Load | [CMXsrv_grl_trae_cod_bco](#cmxsrv_grl_trae_cod_bco) |  |

---

## MODIFIC
<a name="modific"></a>

| **Archivo (Frame)** | **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** |
|--------------------|-------------|-----------------------------|----------------------|
| COL00303.FRM | Form_Activate | [CMXsrv_fincol_cons_tas](#cmxsrv_fincol_cons_tas) | TAS |
| COL00801.FRM | aceptar_click | [CMXsrv_fincol_efec_tras](#cmxsrv_fincol_efec_tras) | TIP, comex..ACMXMONEDAFEC, COL, CUO |
| COL00802.FRM | Form_Activate | [CMXsrv_fincol_cons_trasp](#cmxsrv_fincol_cons_trasp) | EVE, COL |
| COL00803.FRM | Form_Activate | [CMXsrv_fincol_cons_dtrs](#cmxsrv_fincol_cons_dtrs) | EVE, COL |
| COL00901.FRM | Form_Activate | [CMXsrv_fincol_cons_eve](#cmxsrv_fincol_cons_eve) | EVE, COL |
| COL00902.FRM | Form_Load | [CMXsrv_fincol_cons_deve](#cmxsrv_fincol_cons_deve) | EVE, COL |
| COL01001.FRM | aceptar_click | [CMXsrv_fincol_cont_gst](#cmxsrv_fincol_cont_gst) |  |
| COL01002.FRM | Form_Activate | [CMXsrv_fincol_cons_gst](#cmxsrv_fincol_cons_gst) | EVE, COL |
| COL01003.FRM | Form_Activate | [CMXsrv_fincol_cons_dgst](#cmxsrv_fincol_cons_dgst) |  |
| PREFER.FRM | Form_Load | [CMXsrv_lee_fpro](#cmxsrv_lee_fpro) | ACMXFECPRO |

---

## OBLIGA
<a name="obliga"></a>

| **Archivo (Frame)** | **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** |
|--------------------|-------------|-----------------------------|----------------------|
| COL00108.FRM | buscar_Click | [CMXsrv_fincol_bsc_tip](#cmxsrv_fincol_bsc_tip) | TIP |
| COL00108.FRM | Proxima_Click | [CMXsrv_fincol_bsc_tip](#cmxsrv_fincol_bsc_tip) | TIP |
| COL00108.FRM | proximo_Click | [CMXsrv_fincol_bsc_tip](#cmxsrv_fincol_bsc_tip) | TIP |
| CRD00602.FRM | buscar_Click | [CMXsrv_finobl_bus_cor](#cmxsrv_finobl_bus_cor) | COR |
| CRD00602.FRM | proximo_Click | [CMXsrv_finobl_bus_cor](#cmxsrv_finobl_bus_cor) | COR |
| OBL00102.FRM | ELIMINAR_Click | [CMXsrv_finobl_ecuo](#cmxsrv_finobl_ecuo) | OBL, CTO |
| OBL00102.FRM | form_activate | [CMXsrv_finobl_gpln](#cmxsrv_finobl_gpln) | OBL, CTO |
| OBL00102.FRM | form_activate | [CMXsrv_finobl_cons_plnpa](#cmxsrv_finobl_cons_plnpa) | OBL, CTO |
| OBL00103.FRM | anunctb_Click | [CMXsrv_finobl_calc_anu](#cmxsrv_finobl_calc_anu) | OBL |
| OBL00103.FRM | form_activate | [CMXsrv_finobl_lee_obl](#cmxsrv_finobl_lee_obl) | TIP, COR, OBL, ACMXINTERE, ACMXMONEDA, ACMXSUCSAL, CLN |
| OBL00103.FRM | Form_Load | [CMXsrv_lee_fpro](#cmxsrv_lee_fpro) | ACMXFECPRO |
| OBL00103.FRM | Mcbeanl_Click | [CMXsrv_finobl_calc_anu](#cmxsrv_finobl_calc_anu) | OBL |
| OBL00103.FRM | Mcbectb_Click | [CMXsrv_finobl_ctb_oto](#cmxsrv_finobl_ctb_oto) | ACMXDESEMB, TIP, COD, OBL, CTO, CCO |
| OBL00103.FRM | Mcbedel_Click | [CMXsrv_fincol_eli_obl](#cmxsrv_fincol_eli_obl) | OBL, OBL_ADI |
| OBL00103.FRM | Mobl_liq_ope_Click | [CMXsrv_icrd_dat_liq_ope](#cmxsrv_icrd_dat_liq_ope) | ACMXDESEMB, ASND, EVO, CRD, CNO, OBL, CUO, TRSD, NEG, COM, EVE, ACMXTIPEVE, CAN, COL |
| OBL00103.FRM | valida_error | [CMXsrv_finobl_val_obl](#cmxsrv_finobl_val_obl) | TIP, OBL, ACMXINTERE, warnmsg, OBL_ADI |
| OBL00104.FRM | buscar_Click | [CMXsrv_finobl_bsc_obl](#cmxsrv_finobl_bsc_obl) | OBL |
| OBL00104.FRM | fld_obl_tip_ope_LostFocus | [CMXsrv_fincol_lee_tip](#cmxsrv_fincol_lee_tip) | TIP |
| OBL00104.FRM | Proxima_Click | [CMXsrv_finobl_bsc_obl](#cmxsrv_finobl_bsc_obl) | OBL |
| OBL00202.FRM | contabilizar_Click | [CMXsrv_finobl_ictb_pag](#cmxsrv_finobl_ictb_pag) | OBL, CTO, EVO |
| OBL00202.FRM | contabilizar_Click | [CMXsrv_finobl_obt_sdocuo](#cmxsrv_finobl_obt_sdocuo) | OBL, CTO |
| OBL00202.FRM | form_activate | [CMXsrv_finobl_new_tas](#cmxsrv_finobl_new_tas) | CTO |
| OBL00203.FRM | form_activate | [CMXsrv_finobl_cons_pag](#cmxsrv_finobl_cons_pag) | CNO |
| OBL00204.FRM | form_activate | [CMXsrv_finobl_cons_detp](#cmxsrv_finobl_cons_detp) | OBL, CTO, EVO |
| OBL00301.FRM | calcular_Click | [CMXsrv_finobl_calc_pror](#cmxsrv_finobl_calc_pror) | OBL |
| OBL00303.FRM | form_activate | [CMXsrv_finobl_cons_pror](#cmxsrv_finobl_cons_pror) | OBL, EVO |
| OBL00304.FRM | form_activate | [CMXsrv_finobl_cons_dpror](#cmxsrv_finobl_cons_dpror) | OBL, EVO |
| OBL00401.FRM | contabilizar_Click | [CMXsrv_finobl_ctb_anu](#cmxsrv_finobl_ctb_anu) | TIP, COR, OBL, COL, CTO |
| OBL00402.FRM | calcular_Click | [CMXsrv_finobl_calc_anu](#cmxsrv_finobl_calc_anu) | OBL |
| OBL00402.FRM | form_activate | [CMXsrv_finobl_cons_anu](#cmxsrv_finobl_cons_anu) | CNO, EVO |
| OBL00502.FRM | form_activate | [CMXsrv_finobl_cons_mod](#cmxsrv_finobl_cons_mod) | OBL, EVO |
| OBL00503.FRM | form_activate | [CMXsrv_finobl_cons_dmod](#cmxsrv_finobl_cons_dmod) | CNO, EVO |
| OBL00601.FRM | efectuar_Click | [CMXsrv_finobl_rev_eve](#cmxsrv_finobl_rev_eve) | OBL, TRSD, APRCBL, EVO |
| OBL00601.FRM | form_activate | [CMXsrv_finobl_cons_eve](#cmxsrv_finobl_cons_eve) | EVO |
| OBL00602.FRM | form_activate | [CMXsrv_finobl_cons_deve](#cmxsrv_finobl_cons_deve) | EVO |
| OBL00701.FRM | ELIMINAR_Click | [CMXsrv_finobl_eli_ctr](#cmxsrv_finobl_eli_ctr) | CTR |
| OBL00701.FRM | form_activate | [CMXsrv_finobl_cons_ctr](#cmxsrv_finobl_cons_ctr) | CTR |
| OBL00702.FRM | nuevo_Click | [CMXsrv_finobl_ing_ctr](#cmxsrv_finobl_ing_ctr) | COL, OBL, TIP, CTR |
| OBL130.FRM | aceptar_Click | [CMXsrv_finobl_cesion_obl](#cmxsrv_finobl_cesion_obl) | OBL, COR |
| OBL130.FRM | banco_acreedor | [CMXsrv_comgrl_lee_nom_cor](#cmxsrv_comgrl_lee_nom_cor) | COR |
| OBL130.FRM | fld_obl_cod_bco_acre_lostfocus | [CMXsrv_comgrl_lee_nom_cor](#cmxsrv_comgrl_lee_nom_cor) | COR |
| OBL130.FRM | fld_obl_rut_acre_lostfocus | [CMXsrv_lee_cln](#cmxsrv_lee_cln) | CLN |
| OBL130.FRM | form_activate | [CMXsrv_finobl_busc_acre](#cmxsrv_finobl_busc_acre) | OBL |
| PREFER.FRM | Form_Load | [CMXsrv_cmx_get_codes](#cmxsrv_cmx_get_codes) |  |

---

## PAGOS
<a name="pagos"></a>

| **Archivo (Frame)** | **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** |
|--------------------|-------------|-----------------------------|----------------------|
| COL00301.FRM | CALCULAR_Click | [CMXsrv_fincol_efec_calpa](#cmxsrv_fincol_efec_calpa) | TF_PPAG, TIP, TAS, CUO, comex..ACMXMONEDA, COL_ADI, OBL, CTR, NEG_ADI, ACMXINTERE, CAN, ICR, COL |
| COL00303.FRM | Form_Activate | [CMXsrv_fincol_cons_pag](#cmxsrv_fincol_cons_pag) | CAN, COL |
| COL00304.FRM | Form_Load | [CMXsrv_fincol_cons_detp](#cmxsrv_fincol_cons_detp) | ACMXDESEMB, EVE, COL, CUO |
| COL00401.FRM | Aceptar_Click | [CMXsrv_fincol_calc_pror](#cmxsrv_fincol_calc_pror) | ACMXINTERE, COL |
| COL00402.FRM | Contabilizar_Click | [CMXsrv_fincol_cont_pror](#cmxsrv_fincol_cont_pror) | TAS, CRD, NEG_ADI, ACMXINTERE, TIP, CUO, OBL, CAM_TAS, ACMXPLAZO, COL_ADI, LIB, ACMXINTEREFEC, CLN, ACMXOPEIMP, CTO, de, comex..ACMXINTEREFEC, COD, COM, ACMXMONEDAFEC, EVE, CAN, COL |
| COL00403.FRM | Form_Activate | [CMXsrv_fincol_cons_pror](#cmxsrv_fincol_cons_pror) | EVE, COL |
| COL00404.FRM | Form_Activate | [CMXsrv_fincol_cons_dpror](#cmxsrv_fincol_cons_dpror) | ACMXDESEMB, EVE, COL |
| COL00501.FRM | Aceptar_Click | [CMXsrv_busc_cod_ope](#cmxsrv_busc_cod_ope) | TIP, COL |
| COL00501.FRM | Aceptar_Click | [CMXsrv_col_trae_num_ope](#cmxsrv_col_trae_num_ope) | COL |
| COL00501.FRM | Aceptar_Click | [CMXsrv_fincol_cctb_anu](#cmxsrv_fincol_cctb_anu) | TIP, CUO, COD, OBL, TF_ENL, ENL, CAN, COL, CTO |
| COL00501.FRM | Form_Load | [CMXsrv_fincol_calc_anu](#cmxsrv_fincol_calc_anu) | TIP, COL |
| COL00501.FRM | Form_Load | [CMXsrv_busc_cod_ope](#cmxsrv_busc_cod_ope) | TIP, COL |
| COL00502.FRM | CALCULAR_Click | [CMXsrv_fincol_calc_anu](#cmxsrv_fincol_calc_anu) | TIP, COL |
| COL00502.FRM | Form_Activate | [CMXsrv_fincol_cons_anu](#cmxsrv_fincol_cons_anu) | ACMXDESEMB, CAN, EVE, COL |
| COL00602.FRM | Form_Activate | [CMXsrv_fincol_cons_mod](#cmxsrv_fincol_cons_mod) | EVE, COL |
| COL00603.FRM | Form_Activate | [CMXsrv_fincol_cons_dmod](#cmxsrv_fincol_cons_dmod) | CAN, EVE |
| PREFER.FRM | Form_Load | [CMXsrv_lee_fpro](#cmxsrv_lee_fpro) | ACMXFECPRO |
| PREFER.FRM | Form_Load | [CMXsrv_grl_trae_cod_bco](#cmxsrv_grl_trae_cod_bco) |  |

---

## PGOEXT
<a name="pgoext"></a>

| **Archivo (Frame)** | **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** |
|--------------------|-------------|-----------------------------|----------------------|
| PGOCOL01.FRM | calcular_Click | [CMXsrv_fincol_cal_pext](#cmxsrv_fincol_cal_pext) | TIP, CUO, comex..ACMXMONEDA, OBL, CTR, COL, CTO |
| PGOCOL01.FRM | Contabilizar_Click | [CMXsrv_busc_cod_ope](#cmxsrv_busc_cod_ope) | TIP, COL |
| PGOCOL01.FRM | Contabilizar_Click | [CMXsrv_fincol_ctb_pext](#cmxsrv_fincol_ctb_pext) | TIP, ACMXDESEMB, comex..ACMXINTEREFEC, TAS, CUO, COD, OBL, COL_ADI, ACMXMONEDAFEC, CTR, NEG_ADI, ACMXINTERE, EVE, ACMXINTEREFEC, COL, CTO, CCO |
| PGOOBL01.FRM | calcular_Click | [CMXsrv_finobl_cal_pext](#cmxsrv_finobl_cal_pext) | TIP, OBL, ACMXINTERE, ACMXMONEDA, OBL_ADI, CTO |
| PGOOBL01.FRM | Contabilizar_Click | [CMXsrv_finobl_ctb_pext](#cmxsrv_finobl_ctb_pext) | ACMXDESEMB, TIP, COD, OBL, ACMXMONEDAFEC, CTO, CCO |
| PREFER.FRM | Form_Load | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |  |
| PREFER.FRM | Form_Load | [CMXsrv_lee_fpro](#cmxsrv_lee_fpro) | ACMXFECPRO |

---

## ARCOS
<a name="arcos"></a>

| **Archivo (Frame)** | **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** |
|--------------------|-------------|-----------------------------|----------------------|
| ARC00100.FRM | Eliminar_Click | [CMXsrv_iarc_eli_arc](#cmxsrv_iarc_eli_arc) | ADI, CRD, ARC, NEG, COB, INF, COL |
| ARC00100.FRM | Form_activate | [CMXsrv_iarc_busc_arc](#cmxsrv_iarc_busc_arc) | ARC |
| ARC00101.FRM | aceptar_click | [CMXsrv_iinf_busc_inf](#cmxsrv_iinf_busc_inf) | INF |
| ARC00101.FRM | aceptar_click | [CMXsrv_iarc_act_arc](#cmxsrv_iarc_act_arc) | CRD, comex..ACMXMONEDA, ARC, NEG, CBR, ACMXMONEDAFEC, INF, COL |
| ARC00101.FRM | Form_Load | [CMXsrv_iarc_lee_arc](#cmxsrv_iarc_lee_arc) | ARC |
| INFO0201.FRM | buscar_Click | [CMXsrv_iinf_busc_opr](#cmxsrv_iinf_busc_opr) | ARC |
| INFO0201.FRM | Form_activate | [CMXsrv_iinf_lee_vlr](#cmxsrv_iinf_lee_vlr) | INF |
| INFO0202.FRM | aceptar_click | [CMXsrv_iarc_act_arc](#cmxsrv_iarc_act_arc) | CRD, comex..ACMXMONEDA, ARC, NEG, CBR, ACMXMONEDAFEC, INF, COL |
| INFO0202.FRM | Form_activate | [CMXsrv_iinf_busc_inf](#cmxsrv_iinf_busc_inf) | INF |
| INFO0202.FRM | reversar_Click | [CMXsrv_iinf_rev_evi](#cmxsrv_iinf_rev_evi) | INF, ARC, INC, EVI |

---

## COBERIMP
<a name="coberimp"></a>

| **Archivo (Frame)** | **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** |
|--------------------|-------------|-----------------------------|----------------------|
| COB00101.FRM | Form_Activate | [CMXsrv_icob_lee_pln](#cmxsrv_icob_lee_pln) | DIC, POSBCX10, COB, ACMXBCOCEN, ACMXMONEDA, ACMXPAIS |
| COB00101.FRM | Mcobcur_Click | [CMXsrv_icob_cur_cob](#cmxsrv_icob_cur_cob) | comex.dbo, COB |
| COB00101.FRM | Mcobcur_Click | [CMXsrv_icob_pag_sop](#cmxsrv_icob_pag_sop) | DDI, ACMXDESEMB, ADI, DIC, ACMXPRMGRL, ACMXMONEDAFEC, COB, INF, warnmsg |
| COB00101.FRM | MCOBELI_CLICK | [CMXsrv_icob_eli_pln](#cmxsrv_icob_eli_pln) | COB |
| COB00101.FRM | Mcobrev_Click | [CMXsrv_icob_rev_etd](#cmxsrv_icob_rev_etd) | POSBCX10, TRSD, PSO, comex..COB, COB |
| COB00101.FRM | Mcobvali_Click | [CMXsrv_icob_val_cob](#cmxsrv_icob_val_cob) | DDI, LCB, ADI, CUO, ARC, NEG, CBR, COB, INF, ACMXFPAIMP, warnmsg, COL |
| COB00201.FRM | buscar_click | [CMXsrv_icob_busc_pln](#cmxsrv_icob_busc_pln) | COB |
| COB00201.FRM | FLD_COB_COD_CLI_LostFocus | [CMXsrv_icob_lee_cln](#cmxsrv_icob_lee_cln) | CLN |
| COB00201.FRM | PROXIMAS_Click | [CMXsrv_icob_busc_pln](#cmxsrv_icob_busc_pln) | COB |
| COB00300.FRM | ACEPTAR_Click | [CMXsrv_icob_crea_norm](#cmxsrv_icob_crea_norm) | CRD, ARC, CBR, COB, INF, tbl_User, CLN, COL |
| COB00301.FRM | ACEPTAR_Click | [CMXsrv_icob_crea_reem](#cmxsrv_icob_crea_reem) | DIC, COB |
| COB00302.FRM | ACEPTAR_Click | [CMXsrv_icob_act_gral](#cmxsrv_icob_act_gral) | CLN, COB |
| COB00302.FRM | FLD_COB_COD_CLI_LostFocus | [CMXsrv_icob_lee_cln2](#cmxsrv_icob_lee_cln2) | CLN |
| COB00302.FRM | Form_Activate | [CMXsrv_icob_lee_gral](#cmxsrv_icob_lee_gral) | ACMXBCOCEN, ACMXPAIS, COB |
| COB00303.FRM | ACEPTAR_Click | [CMXsrv_icob_act_val](#cmxsrv_icob_act_val) | ACMXMONEDAFEC, COB |
| COB00303.FRM | Form_Activate | [CMXsrv_icob_lee_val](#cmxsrv_icob_lee_val) | COB |
| COB00304.FRM | ACEPTAR_Click | [CMXsrv_icob_act_acu](#cmxsrv_icob_act_acu) | COB |
| COB00304.FRM | Form_Activate | [CMXsrv_icob_lee_acu](#cmxsrv_icob_lee_acu) | ACMXPAIS, COB |
| COB00304.FRM | Form_Load | [CMXsrv_icob_lee_acu](#cmxsrv_icob_lee_acu) | ACMXPAIS, COB |
| COB00305.FRM | ELIMINAR_Click | [CMXsrv_icob_eli_int](#cmxsrv_icob_eli_int) | DIC, COB |
| COB00305.FRM | Form_Activate | [CMXsrv_icob_busc_int](#cmxsrv_icob_busc_int) | DIC |
| COB00306.FRM | ACEPTAR_Click | [CMXsrv_icob_ingmod_int](#cmxsrv_icob_ingmod_int) | DIC, COB |
| COB00306.FRM | Form_Activate | [CMXsrv_icob_lee_int](#cmxsrv_icob_lee_int) | DIC |
| COB00307.FRM | ACEPTAR_Click | [CMXsrv_icob_ing_mod_srf](#cmxsrv_icob_ing_mod_srf) | CLN, tbl_User, COB |
| COB00307.FRM | CmdEliminar_Click | [CMXsrv_icob_eli_pln](#cmxsrv_icob_eli_pln) | COB |
| COB00307.FRM | CmdReversar_Click | [CMXsrv_icob_rev_etd](#cmxsrv_icob_rev_etd) | POSBCX10, TRSD, PSO, comex..COB, COB |
| COB00307.FRM | CURSAR_Click | [CMXsrv_icob_ing_mod_srf](#cmxsrv_icob_ing_mod_srf) | CLN, tbl_User, COB |
| COB00307.FRM | CURSAR_Click | [CMXsrv_icob_pag_sop](#cmxsrv_icob_pag_sop) | DDI, ACMXDESEMB, ADI, DIC, ACMXPRMGRL, ACMXMONEDAFEC, COB, INF, warnmsg |
| COB00307.FRM | FLD_COB_COD_CLI_LostFocus | [CMXsrv_icob_lee_cln2](#cmxsrv_icob_lee_cln2) | CLN |
| COB00307.FRM | Reversar_Click | [CMXsrv_icob_rev_etd](#cmxsrv_icob_rev_etd) | POSBCX10, TRSD, PSO, comex..COB, COB |
| COB00501.FRM | ACEPTAR_Click | [CMXsrv_icob_anu](#cmxsrv_icob_anu) | DIC, POSBCX10, ACMXMONEDAFEC, PSO, COB, ACMXTPOAUTN |
| COB00501.FRM | Form_Load | [CMXsrv_icob_lee_anu](#cmxsrv_icob_lee_anu) | COB |
| COB0601.FRM | FLD_COB_COD_CLI_LostFocus | [CMXsrv_icob_lee_cln](#cmxsrv_icob_lee_cln) | CLN |
| FORM2.FRM | ACEPTAR_Click | [CMXsrv_icob_pag_sop](#cmxsrv_icob_pag_sop) | DDI, ACMXDESEMB, ADI, DIC, ACMXPRMGRL, ACMXMONEDAFEC, COB, INF, warnmsg |
| ORI_DEST.FRM | ACEPTAR_Click | [CMXsrv_icob_cur_reem](#cmxsrv_icob_cur_reem) | comex..COB, COB |
| PREFER.FRM | Form_Load | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |  |

---

## COBRANZA
<a name="cobranza"></a>

| **Archivo (Frame)** | **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** |
|--------------------|-------------|-----------------------------|----------------------|
| CBR00101.FRM | ejecut_avi_imp_999 | [CMXsrv_busc_cor_swf](#cmxsrv_busc_cor_swf) | SWT |
| CBR00101.FRM | ejecut_avi_imp_999 | [CMXsrv_swf_bus_sms](#cmxsrv_swf_bus_sms) | SMS |
| CBR00101.FRM | Form_Activate | [CMXsrv_icbr_lee_cbr](#cmxsrv_icbr_lee_cbr) | ACMXPAIS, COR, LCB, ACMXVIATPT, ACMXBCOBCC, CBR, ACMXMONEDA, ACMXCLACOM, tbl_User, ACMXSUCSAL, CLN |
| CBR00101.FRM | Form_Load | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |  |
| CBR00101.FRM | Mcbrace_Click | [CMXsrv_icbr_acep_let](#cmxsrv_icbr_acep_let) | comex..CBR, LCB, CBR |
| CBR00101.FRM | Mcbrcon_Click | [CMXsrv_icbr_cont_cbr](#cmxsrv_icbr_cont_cbr) | OPE_BCI, APRCBL, LCB, CBR |
| CBR00101.FRM | Mcbreli_click | [CMXsrv_icbr_eli_cbr](#cmxsrv_icbr_eli_cbr) | ARC, REMENT, CBR, comex..COL |
| CBR00101.FRM | McbrTxt999_Click | [CMXsrv_icbr_lee_ctp](#cmxsrv_icbr_lee_ctp) | ACMXSUCSAL, MCBRCTP, CBR, ACMXPAIS, CLN, CBRANX |
| CBR00101.FRM | Mcbrtxtrec_Click | [CMXsrv_icbr_avi1](#cmxsrv_icbr_avi1) | ACMXDESEMB, ASND, ACMXBCOBCC, ARC, CBR, ACMXINTERE, PCX, ECE, ACMXMONEDA, ACMXSUCSAL, CLN |
| CBR00102.FRM | aceptar_Click | [CMXsrv_val_suc](#cmxsrv_val_suc) | ACMXSUCSAL, tbl_User |
| CBR00102.FRM | buscar_Click | [CMXsrv_icbr_busc_cbr](#cmxsrv_icbr_busc_cbr) | ACMXSUCSAL, ACMXMONEDA, CLN, CBR |
| CBR00102.FRM | fld_aux_glo_ofi_LostFocus | [CMXsrv_val_suc](#cmxsrv_val_suc) | ACMXSUCSAL, tbl_User |
| CBR00102.FRM | fld_cbr_cod_gdo_LostFocus | [CMXsrv_icbr_lee_cln](#cmxsrv_icbr_lee_cln) | CLN |
| CBR00102.FRM | fld_cbr_cod_ofi_lostfocus | [CMXsrv_val_suc](#cmxsrv_val_suc) | ACMXSUCSAL, tbl_User |
| CBR00102.FRM | proximas_Click | [CMXsrv_icbr_busc_cbr](#cmxsrv_icbr_busc_cbr) | ACMXSUCSAL, ACMXMONEDA, CLN, CBR |
| CBR00103.FRM | crear_Click | [CMXsrv_icbr_crea_cbr](#cmxsrv_icbr_crea_cbr) | CLN, tbl_User |
| CBR00103.FRM | fld_cbr_cod_gdo_LostFocus | [CMXsrv_icbr_lee_cln](#cmxsrv_icbr_lee_cln) | CLN |
| CBR00103.FRM | fld_cbr_cod_ofi_lostfocus | [CMXsrv_val_suc](#cmxsrv_val_suc) | ACMXSUCSAL, tbl_User |
| CBR00103.FRM | INGRESAR_Click | [CMXsrv_icbr_crea_cbr](#cmxsrv_icbr_crea_cbr) | CLN, tbl_User |
| CBR00201.FRM | fld_cbr_cod_gdo_LostFocus | [CMXsrv_icbr_lee_cln](#cmxsrv_icbr_lee_cln) | CLN |
| CBR00201.FRM | Form_Activate | [CMXsrv_icbr_lee_cob](#cmxsrv_icbr_lee_cob) | COB |
| CBR00201.FRM | Form_Load | [CMXsrv_icbr_lee_ctp](#cmxsrv_icbr_lee_ctp) | ACMXSUCSAL, MCBRCTP, CBR, ACMXPAIS, CLN, CBRANX |
| CBR00201.FRM | INGRESAR_Click | [CMXsrv_icbr_act_ctp](#cmxsrv_icbr_act_ctp) | comex..CBR, MCBRCTP, CBRANX, CBR |
| CBR00202.FRM | Form_Activate | [CMXsrv_icbr_lee_cob](#cmxsrv_icbr_lee_cob) | COB |
| CBR00202.FRM | Form_Load | [CMXsrv_icbr_lee_trm](#cmxsrv_icbr_lee_trm) | ACMXVIATPT, CBR, ACMXINTERE, ACMXMONEDA, MCBRTER, ACMXCLACOM, ACMXPAIS |
| CBR00202.FRM | INGRESAR_Click | [CMXsrv_icbr_act_trm](#cmxsrv_icbr_act_trm) | LCB, COM, CBR, MCBRTER, warnmsg, CLN |
| CBR00203.FRM | Form_Activate | [CMXsrv_icbr_lee_cob](#cmxsrv_icbr_lee_cob) | COB |
| CBR00203.FRM | Form_Load | [CMXsrv_icbr_lee_doc](#cmxsrv_icbr_lee_doc) | LCB, MCBRDOC, MLCB, CBR, ACMXMONEDA |
| CBR00203.FRM | INGRESAR_Click | [CMXsrv_icbr_act_doc](#cmxsrv_icbr_act_doc) | LCB, MCBRDOC, MLCB, CBR, comex..CBR |
| CBR00301.FRM | Form_Activate | [CMXsrv_icbr_busc_let](#cmxsrv_icbr_busc_let) | MLCB, comex..MLCB, comex..LCB |
| CBR00302.FRM | aceptar_Click | [CMXsrv_icbr_ingmod_let](#cmxsrv_icbr_ingmod_let) | LCB, CBR, comex.dbo |
| CBR00302.FRM | eliminar_Click | [CMXsrv_icbr_eli_let](#cmxsrv_icbr_eli_let) | LCB, MCBRDOC, MLCB, CBR, comex..COL |
| CBR00302.FRM | Form_Activate | [CMXsrv_icbr_lee_let](#cmxsrv_icbr_lee_let) | ACMXNOTARIO, LCB, MLCB |
| CBR00305.FRM | aceptar_Click | [CMXsrv_icbr_prorr](#cmxsrv_icbr_prorr) | comex..CBR, LCB, CBR |
| CBR00401.FRM | EFECTUAR_Click | [CMXsrv_icbr_rev_eve](#cmxsrv_icbr_rev_eve) | APRCBL, TRSD, CBR, vig_trs, ECE, DIP, LIB, tbl_User |
| CBR00401.FRM | Form_Activate | [CMXsrv_icbr_busc_eve](#cmxsrv_icbr_busc_eve) | ECE |
| CBR00402.FRM | Form_Load | [CMXsrv_icbr_lee_eve](#cmxsrv_icbr_lee_eve) | ECE, ACMXDESEMB |
| CBR00402.FRM | Form_Load | [CMXsrv_icbr_lee_ent_doc](#cmxsrv_icbr_lee_ent_doc) | CBR |
| CBR00701.FRM | aceptar_Click | [CMXsrv_icbr_prot](#cmxsrv_icbr_prot) | LCB, CBR |
| CBR00701.FRM | Form_Load | [CMXsrv_icbr_pcg_prot](#cmxsrv_icbr_pcg_prot) | LCB, CBR |
| CBR00801.FRM | aceptar_Click | [CMXsrv_icbr_liq_sdo](#cmxsrv_icbr_liq_sdo) | comex..CBR, LCB, CBR |
| CBR00802.FRM | aceptar_Click | [CMXsrv_icbr_act_vis](#cmxsrv_icbr_act_vis) | comex..CBR, CBR |
| CBR00802.FRM | eliminar_Click | [CMXsrv_icbr_eli_rep](#cmxsrv_icbr_eli_rep) | REP |
| CBR00802.FRM | Form_Activate | [CMXsrv_icbr_busc_rep](#cmxsrv_icbr_busc_rep) | REP |
| CBR00803.FRM | aceptar_Click | [CMXsrv_icbr_imod_rep](#cmxsrv_icbr_imod_rep) | REP, CBR |
| CBR00804.FRM | aceptar_Click | [CMXsrv_icbr_ent_doc](#cmxsrv_icbr_ent_doc) | comex..CBR, LCB, CBR |
| CBR00804.FRM | Form_Load | [CMXsrv_icbr_lee_ent_doc](#cmxsrv_icbr_lee_ent_doc) | CBR |
| CBR00901.FRM | aceptar_Click | [CMXsrv_icbr_trf_ofi](#cmxsrv_icbr_trf_ofi) | comex..CBR, ACMXSUCSAL, CBR |
| CBR00901.FRM | aceptar_Click | [CMXsrv_val_suc](#cmxsrv_val_suc) | ACMXSUCSAL, tbl_User |
| CBR00902.FRM | aceptar_Click | [CMXsrv_icbr_trf_bco](#cmxsrv_icbr_trf_bco) | comex..CBR, ARC, CBR, LCB |
| COBERTU.FRM | aceptar_Click | [CMXsrv_icbr_act_inst](#cmxsrv_icbr_act_inst) | comex..CBR, CBR |
| GRL00101.FRM | enviar_Click | [CMXsrv_iswf_a_pru](#cmxsrv_iswf_a_pru) | switxt, switxt1 |
| GRL00101.FRM | Form_Load | [CMXsrv_icbr_val_cbr](#cmxsrv_icbr_val_cbr) | DDI, LCB, COR, ADI, ARC, ACMXMONEDAFEC, CBR, ACMXINTEREFEC, warnmsg |
| GRL00101.FRM | word_Click | [CMXsrv_icbr_val_cbr](#cmxsrv_icbr_val_cbr) | DDI, LCB, COR, ADI, ARC, ACMXMONEDAFEC, CBR, ACMXINTEREFEC, warnmsg |
| GRL00101.FRM | word_Click | [CMXsrv_iswf_a_pru](#cmxsrv_iswf_a_pru) | switxt, switxt1 |

---

## CRDEXT
<a name="crdext"></a>

| **Archivo (Frame)** | **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** |
|--------------------|-------------|-----------------------------|----------------------|
| BCO_BCO.FRM | Aceptar_Click | [CMXsrv_icrd_a_ibab](#cmxsrv_icrd_a_ibab) | MIBAB, IBAB |
| BCO_BCO.FRM | Form_Load | [CMXsrv_icrd_lee_glo_ibab](#cmxsrv_icrd_lee_glo_ibab) | IBAB, COL, MIBAB |
| BCO_REM.FRM | Aceptar_Click | [CMXsrv_icrd_a_ibar](#cmxsrv_icrd_a_ibar) | MIBAR, IBAR |
| BCO_REM.FRM | Form_Load | [CMXsrv_icrd_lee_glo_ibar](#cmxsrv_icrd_lee_glo_ibar) | MIBAR, COL, IBAR |
| BUSC_COD.FRM | buscar_click | [CMXsrv_icrd_lee_tex_swf](#cmxsrv_icrd_lee_tex_swf) | ACMXTSWFESPMSG, ACMXTSWFINGMSG |
| BUSC_TXT.FRM | Aceptar_Click | [CMXsrv_icrd_lee_cod_txt_swf](#cmxsrv_icrd_lee_cod_txt_swf) | ACMXTSWFESPMSG, ACMXTSWFINGMSG |
| BUSC_TXT.FRM | buscar_click | [CMXsrv_icrd_lee_txt_swf_all](#cmxsrv_icrd_lee_txt_swf_all) | ACMXTSWFESPMSG, ACMXTSWFINGMSG |
| BUSC_TXT.FRM | Form_Load | [CMXsrv_icrd_lee_ind_esp_ing](#cmxsrv_icrd_lee_ind_esp_ing) | MCTP, CRD |
| BUSC_TXT.FRM | llena_arreglo | [CMXsrv_icrd_lee_tex_swf](#cmxsrv_icrd_lee_tex_swf) | ACMXTSWFESPMSG, ACMXTSWFINGMSG |
| BUSC_TXT.FRM | proximo_Click | [CMXsrv_icrd_lee_txt_swf_all](#cmxsrv_icrd_lee_txt_swf_all) | ACMXTSWFESPMSG, ACMXTSWFINGMSG |
| CRD00207.FRM | aceptar_Click | [CMXsrv_icrd_ing_acu](#cmxsrv_icrd_ing_acu) | CRD |
| CRD00207.FRM | Form_Load | [CMXsrv_icrd_lee_acu](#cmxsrv_icrd_lee_acu) | CRD |
| CRD00701.FRM | aceptar_Click | [CMXsrv_icrd_rech_sol](#cmxsrv_icrd_rech_sol) | CRD, comex..COL, OPE_BCI, COL, comex..CRD |
| CRD00801.FRM | aceptar_Click | [CMXsrv_icrd_end](#cmxsrv_icrd_end) | INF, ARC, COL, CRD |
| CRD00801.FRM | Form_Load | [CMXsrv_icrd_lee_dat_end](#cmxsrv_icrd_lee_dat_end) | CRD |
| CRD02001.FRM | aceptar_Click | [CMXsrv_icrd_asignar_cor](#cmxsrv_icrd_asignar_cor) | COR, ACMXMONEDAFEC, CRD, LCR |
| CRD02001.FRM | buscar_Click | [CMXsrv_icrd_bus_lcr_bco](#cmxsrv_icrd_bus_lcr_bco) | COR |
| CRD02001.FRM | proximo_Click | [CMXsrv_icrd_bus_lcr_bco](#cmxsrv_icrd_bus_lcr_bco) | COR |
| PREFER.FRM | Form_Load | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |  |

---

## CRD_CORR
<a name="crd_corr"></a>

| **Archivo (Frame)** | **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** |
|--------------------|-------------|-----------------------------|----------------------|
| COR00202.FRM | aceptar_Click | [CMXsrv_icrd_asignar_cor](#cmxsrv_icrd_asignar_cor) | COR, ACMXMONEDAFEC, CRD, LCR |
| COR00202.FRM | buscar_Click | [CMXsrv_icrd_bus_lcr_bco](#cmxsrv_icrd_bus_lcr_bco) | COR |
| COR00202.FRM | fld_cor_cod_mtr_LostFocus | [CMXsrv_icrd_lee_bco_mtr](#cmxsrv_icrd_lee_bco_mtr) | comex..ACMXBANCOS |
| COR00202.FRM | fld_cor_cod_pais_Lostfocus | [CMXsrv_icrd_cor_lee_pais](#cmxsrv_icrd_cor_lee_pais) | comex..ACMXPAIS |
| COR00202.FRM | fld_cor_cod_plz_Lostfocus | [CMXsrv_icrd_lee_plz](#cmxsrv_icrd_lee_plz) | ACMXPLAZAS |
| COR00202.FRM | proximo_Click | [CMXsrv_icrd_bus_lcr_bco](#cmxsrv_icrd_bus_lcr_bco) | COR |
| COR00906.FRM | buscar_Click | [CMXsrv_icrd_busc_plz](#cmxsrv_icrd_busc_plz) | comex..ACMXPLAZAS |
| COR00906.FRM | proximos_Click | [CMXsrv_icrd_busc_plz](#cmxsrv_icrd_busc_plz) | comex..ACMXPLAZAS |
| COR00907.FRM | buscar_Click | [CMXsrv_icrd_cor_busc_pais](#cmxsrv_icrd_cor_busc_pais) | comex, comex..ACMXPAIS |
| COR00907.FRM | proximos_Click | [CMXsrv_icrd_cor_busc_pais](#cmxsrv_icrd_cor_busc_pais) | comex, comex..ACMXPAIS |
| GRID_BUS.FRM | buscar_Click | [CMXsrv_icrd_busc_bco_mtr](#cmxsrv_icrd_busc_bco_mtr) | comex |
| GRID_BUS.FRM | proximos_Click | [CMXsrv_icrd_busc_bco_mtr](#cmxsrv_icrd_busc_bco_mtr) | comex |

---

## DDI
<a name="ddi"></a>

| **Archivo (Frame)** | **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** |
|--------------------|-------------|-----------------------------|----------------------|
| DDI00101.FRM | aceptar_Click | [CMXsrv_iddi_ingmod_ddi](#cmxsrv_iddi_ingmod_ddi) | INF, DDI |
| DDI00101.FRM | continuar_Click | [CMXsrv_iddi_lee_dec](#cmxsrv_iddi_lee_dec) | DDI, ACMXVIATPT, ACMXRGMIMP, INF, ACMXBCOCEN, ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM, ACMXPAIS, CLN |
| DDI00101.FRM | eliminar_Click | [CMXsrv_iddi_eli_ddi](#cmxsrv_iddi_eli_ddi) | DDI |
| DDI00101.FRM | fld_ddi_fec_ii_lostfocus | [CMXsrv_iddi_lee_inf](#cmxsrv_iddi_lee_inf) | INF |
| DDI00101.FRM | fld_ddi_rut_imp_lostfocus | [CMXsrv_iddi_lee_cln](#cmxsrv_iddi_lee_cln) | CLN |
| DDI01001.FRM | Asociar_Click | [CMXsrv_iddi_lee_rut](#cmxsrv_iddi_lee_rut) | DDI |
| DDI01001.FRM | Asociar_Click | [CMXsrv_iddi_asoc_ddi](#cmxsrv_iddi_asoc_ddi) | DDI, ARC, ACMXMONEDAFEC, CBR, COB, INF, ACMXMONEDA, COL |
| DDI01001.FRM | Command2_Click | [CMXsrv_iddi_des_ddi](#cmxsrv_iddi_des_ddi) | DDI, ADI, COB |
| DDI01001.FRM | Desasociar_Click | [CMXsrv_iddi_lee_rut](#cmxsrv_iddi_lee_rut) | DDI |
| DDI01001.FRM | Desasociar_Click | [CMXsrv_iddi_des_ddi](#cmxsrv_iddi_des_ddi) | DDI, ADI, COB |
| DDI01001.FRM | fld_aux_rut_cli_lostfocus | [CMXsrv_iddi_lee_cln](#cmxsrv_iddi_lee_cln) | CLN |
| DDI01001.FRM | inicio_asoc | [CMXsrv_iddi_busc_asoc](#cmxsrv_iddi_busc_asoc) | ADI |
| DDI01001.FRM | inicio_noasoc | [CMXsrv_iddi_busc_noasoc](#cmxsrv_iddi_busc_noasoc) | DDI, ADI |
| DDI01001.FRM | proximo_no_aso_Click | [CMXsrv_iddi_busc_noasoc](#cmxsrv_iddi_busc_noasoc) | DDI, ADI |

---

## IMPORT
<a name="import"></a>

| **Archivo (Frame)** | **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** |
|--------------------|-------------|-----------------------------|----------------------|
| BUSCADIR.FRM | buscar_Click | [CMXsrv_icrd_lee_dir_cln](#cmxsrv_icrd_lee_dir_cln) | DIRCLN |
| BUSC_COD.FRM | buscar_click | [CMXsrv_icrd_lee_tex_swf](#cmxsrv_icrd_lee_tex_swf) | ACMXTSWFESPMSG, ACMXTSWFINGMSG |
| BUSC_TXT.FRM | Aceptar_Click | [CMXsrv_icrd_lee_cod_txt_swf](#cmxsrv_icrd_lee_cod_txt_swf) | ACMXTSWFESPMSG, ACMXTSWFINGMSG |
| BUSC_TXT.FRM | buscar_click | [CMXsrv_icrd_lee_txt_swf_all](#cmxsrv_icrd_lee_txt_swf_all) | ACMXTSWFESPMSG, ACMXTSWFINGMSG |
| BUSC_TXT.FRM | Form_Load | [CMXsrv_icrd_lee_ind_esp_ing](#cmxsrv_icrd_lee_ind_esp_ing) | MCTP, CRD |
| BUSC_TXT.FRM | llena_arreglo | [CMXsrv_icrd_lee_tex_swf](#cmxsrv_icrd_lee_tex_swf) | ACMXTSWFESPMSG, ACMXTSWFINGMSG |
| BUSC_TXT.FRM | proximo_Click | [CMXsrv_icrd_lee_txt_swf_all](#cmxsrv_icrd_lee_txt_swf_all) | ACMXTSWFESPMSG, ACMXTSWFINGMSG |
| CONDESP.FRM | Aceptar_Click | [CMXCRDsrv_icrd_a_cnd_esp](#cmxcrdsrv_icrd_a_cnd_esp) | CND |
| CONDESP.FRM | Form_Load | [CMXsrv_icrd_lee_cnd_esp](#cmxsrv_icrd_lee_cnd_esp) | MMCND, COL, CND |
| CRD00101.FRM | clon_Click | [CMXCRDsrv_icrd_clon_crd](#cmxcrdsrv_icrd_clon_crd) | CRS, MER, CRD, TAS, CRDCLON, COL_ADI, CND, DAC, ODOC, AVAL, COL, EMB |
| CRD00101.FRM | Form_Activate | [CMXCRDsrv_icrd_lee_crdcre](#cmxcrdsrv_icrd_lee_crdcre) | CRD_ADI, ACMXFORPAG, ACMXPAIS, ACMXVIATPT, CRD, COR, COL_ADI, ACMXFINVER, PMIX, NEG, ACMXMONEDA, tbl_User, OPE_BCI, ACMXSUCSAL, CLN, COL, DIRCLN, EMB |
| CRD00101.FRM | Form_Activate | [CMXsrv_icrd_lee_ind_esp_ing](#cmxsrv_icrd_lee_ind_esp_ing) | MCTP, CRD |
| CRD00101.FRM | Form_Activate | [CMXsrv_icrd_lee_top](#cmxsrv_icrd_lee_top) | COL |
| CRD00101.FRM | Form_Load | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |  |
| CRD00101.FRM | Form_Load | [CMXsrv_cmx_get_codes](#cmxsrv_cmx_get_codes) |  |
| CRD00101.FRM | Form_Load | [CMXsrv_trae_glo_fec](#cmxsrv_trae_glo_fec) | ACMXSUCSAL, ACMXDL3475FEC, tbl_User |
| CRD00101.FRM | Mcrdapr_Click | [CMXCRDsrv_icrd_val_crd](#cmxcrdsrv_icrd_val_crd) | warnmsg |
| CRD00101.FRM | Mcrdeli_click | [CMXCRDsrv_icrd_eli_crd](#cmxcrdsrv_icrd_eli_crd) | comex..COL, OPE_BCI, CRD |
| CRD00101.FRM | Mcrdtxtliq_Click | [CMXsrv_icrd_lee_dat_trs](#cmxsrv_icrd_lee_dat_trs) | ASND, EVI, TRSD, EVE, ACMXMONEDA, COL |
| CRD00101.FRM | Mcrdtxtope_Click | [CMXsrv_icrd_dat_liq_ope](#cmxsrv_icrd_dat_liq_ope) | ACMXDESEMB, ASND, EVO, CRD, CNO, OBL, CUO, TRSD, NEG, COM, EVE, ACMXTIPEVE, CAN, COL |
| CRD00101.FRM | msg_swift | [CMXsrv_iswf_a_pru](#cmxsrv_iswf_a_pru) | switxt, switxt1 |
| CRD00201.FRM | Aceptar_Click | [CMXsrv_icrd_a_ctp](#cmxsrv_icrd_a_ctp) | CRD, CRDCLON, MCTP, comex..COL, COL |
| CRD00201.FRM | FLD_COL_COD_CLI_LostFocus | [CMXsrv_icrd_lee_cln](#cmxsrv_icrd_lee_cln) | CLN, DIRCLN |
| CRD00201.FRM | Form_Load | [CMXsrv_lee_fpro](#cmxsrv_lee_fpro) | ACMXFECPRO |
| CRD00202.FRM | Aceptar_Click | [CMXsrv_icrd_a_cnd](#cmxsrv_icrd_a_cnd) | TIP, CRD_ADI, CRD, CRDCLON, COL_ADI, COM, ACMXMONEDA, LIB, comex..COL, MAPR, MCND, COL, ACMXOPEIMP, comex..CRD |
| CRD00202.FRM | Aceptar_Click | [CMXCRDsrv_icrd_crea_crd](#cmxcrdsrv_icrd_crea_crd) | CRD_ADI, PMIX, ACMXMONEDA, CLN, COL |
| CRD00202.FRM | fld_col_fec_vto_LostFocus | [CMXsrv_util_det_habil](#cmxsrv_util_det_habil) | ACMXFERIADO |
| CRD00203.FRM | Form_Activate | [CMXsrv_icrd_busc_emb](#cmxsrv_icrd_busc_emb) | comex..EMB, comex..MEMB |
| CRD00204.FRM | ELIMINAR_Click | [CMXsrv_icrd_eli_emb](#cmxsrv_icrd_eli_emb) | comex..COL, EMB, COL, CRD |
| CRD00204.FRM | Form_Load | [CMXsrv_icrd_lee_emb1](#cmxsrv_icrd_lee_emb1) | CRS, COL, EMB |
| CRD00204.FRM | Form_Load | [CMXsrv_icrd_lee_emb2](#cmxsrv_icrd_lee_emb2) | COL, EMB |
| CRD00204.FRM | ingresar_Click | [CMXsrv_icrd_a_emb1](#cmxsrv_icrd_a_emb1) | CRS, MEMB, CRD, MCRS, CRDCLON, COL, EMB |
| CRD00204.FRM | ingresar_Click | [CMXsrv_icrd_a_emb2](#cmxsrv_icrd_a_emb2) | EMB, COL, MEMB, CRD |
| CRD00204.FRM | VALIDA_EMBARQUE | [CMXsrv_icrd_val_emb2](#cmxsrv_icrd_val_emb2) | warnmsg |
| CRD00204.FRM | VALIDA_EMBARQUE | [CMXsrv_icrd_val_emb1](#cmxsrv_icrd_val_emb1) | INF, ARC, warnmsg |
| CRD00205.FRM | Aceptar_Click | [CMXsrv_icrd_act_ref](#cmxsrv_icrd_act_ref) | MREF, CRD, CRDCLON, comex..MREF, comex..COL, COL |
| CRD00205.FRM | Form_Load | [CMXsrv_icrd_act_ref](#cmxsrv_icrd_act_ref) | MREF, CRD, CRDCLON, comex..MREF, comex..COL, COL |
| CRD00205.FRM | Form_Load | [CMXsrv_icrd_lee_ref](#cmxsrv_icrd_lee_ref) | COR, COL, CRD |
| CRD00301.FRM | FLD_COL_COD_CLI_LostFocus | [CMXsrv_icrd_lee_cln](#cmxsrv_icrd_lee_cln) | CLN, DIRCLN |
| CRD0063.FRM | Aceptar_Click | [CMXCRDsrv_icrd_apr_sol](#cmxcrdsrv_icrd_apr_sol) | TIP, CRD, COL_ADI, COM, LIB, OPE_BCI, sysobjects, CLN, COL |
| CRD0063.FRM | Form_Load | [CMXsrv_icrd_lee_crdapr](#cmxsrv_icrd_lee_crdapr) | CRS, CRD, COL_ADI, DAC, ACMXAPROBAC |
| CRD00701.FRM | Aceptar_Click | [CMXsrv_icrd_rech_sol](#cmxsrv_icrd_rech_sol) | CRD, comex..COL, OPE_BCI, COL, comex..CRD |
| DESCMERC.FRM | Aceptar_Click | [CMXCRDsrv_icrd_a_desc_merc](#cmxcrdsrv_icrd_a_desc_merc) | MER |
| DESCMERC.FRM | Form_Load | [CMXsrv_icrd_lee_desc_merc](#cmxsrv_icrd_lee_desc_merc) | MMER, MER |
| DOCUMENT.FRM | Aceptar_Click | [CMXsrv_icrd_a_otr_doc](#cmxsrv_icrd_a_otr_doc) | ODOC, MODOC |
| DOCUMENT.FRM | Form_Load | [CMXsrv_icrd_lee_otr_doc](#cmxsrv_icrd_lee_otr_doc) | ODOC, MODOC |
| GRL00101.FRM | enviar_Click | [CMXsrv_iswf_a_pru](#cmxsrv_iswf_a_pru) | switxt, switxt1 |

---

## INFORME
<a name="informe"></a>

| **Archivo (Frame)** | **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** |
|--------------------|-------------|-----------------------------|----------------------|
| ARC00100.FRM | Eliminar_Click | [CMXsrv_iarc_eli_arc](#cmxsrv_iarc_eli_arc) | ADI, CRD, ARC, NEG, COB, INF, COL |
| ARC00100.FRM | Form_Activate | [CMXsrv_iarc_busc_arc](#cmxsrv_iarc_busc_arc) | ARC |
| INFO0101.FRM | Form_Activate | [CMXsrv_iinf_lee0_inf](#cmxsrv_iinf_lee0_inf) | INF |
| INFO0101.FRM | Form_Activate | [CMXsrv_iinf_lee_tablas](#cmxsrv_iinf_lee_tablas) | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM |
| INFO0101.FRM | Form_Activate | [CMXsrv_iinf_lee1_inf](#cmxsrv_iinf_lee1_inf) | INF, CLN |
| INFO0101.FRM | Form_Activate | [CMXsrv_iinf_lee_cln](#cmxsrv_iinf_lee_cln) | CLN |
| INFO0101.FRM | Form_Activate | [CMXsrv_iinf_lee2_inf](#cmxsrv_iinf_lee2_inf) | INF |
| INFO0101.FRM | Form_Activate | [CMXsrv_iinf_avi_miscb](#cmxsrv_iinf_avi_miscb) | INF |
| INFO0101.FRM | Maviapr_Click | [CMXsrv_iinf_avi_misca](#cmxsrv_iinf_avi_misca) | INF, CLN |
| INFO0101.FRM | Maviapr_Click | [CMXsrv_iinf_avi_miscb](#cmxsrv_iinf_avi_miscb) | INF |
| INFO0101.FRM | Mavicom_Click | [CMXsrv_iinf_avi_misca](#cmxsrv_iinf_avi_misca) | INF, CLN |
| INFO0101.FRM | Mavicom_Click | [CMXsrv_iinf_avi_miscb](#cmxsrv_iinf_avi_miscb) | INF |
| INFO0101.FRM | Mavicom_Click | [CMXsrv_icrd_lee_dat_com](#cmxsrv_icrd_lee_dat_com) | TIP, ACMXDESEMB, ASND, CRD, EVI, COM, TRSD, EVE, ACMXMONEDA |
| INFO0101.FRM | Mavimis1_Click | [CMXsrv_iinf_avi_misca](#cmxsrv_iinf_avi_misca) | INF, CLN |
| INFO0101.FRM | Mavimis1_Click | [CMXsrv_iinf_avi_miscb](#cmxsrv_iinf_avi_miscb) | INF |
| INFO0101.FRM | Mavimis2_Click | [CMXsrv_iinf_avi_misca](#cmxsrv_iinf_avi_misca) | INF, CLN |
| INFO0101.FRM | Mavimis2_Click | [CMXsrv_iinf_avi_miscb](#cmxsrv_iinf_avi_miscb) | INF |
| INFO0101.FRM | Mavirec_Click | [CMXsrv_iinf_avi_misca](#cmxsrv_iinf_avi_misca) | INF, CLN |
| INFO0101.FRM | Mavirec_Click | [CMXsrv_iinf_avi_miscb](#cmxsrv_iinf_avi_miscb) | INF |
| INFO0101.FRM | Mavitib_Click | [CMXsrv_iinf_avi_misca](#cmxsrv_iinf_avi_misca) | INF, CLN |
| INFO0101.FRM | Mavitib_Click | [CMXsrv_iinf_avi_miscb](#cmxsrv_iinf_avi_miscb) | INF |
| INFO0101.FRM | Mavitras_Click | [CMXsrv_iinf_avi_misca](#cmxsrv_iinf_avi_misca) | INF, CLN |
| INFO0101.FRM | Mavitras_Click | [CMXsrv_iinf_avi_miscb](#cmxsrv_iinf_avi_miscb) | INF |
| INFO0101.FRM | Mavitras_Click | [CMXsrv_icrd_lee_dat_trs](#cmxsrv_icrd_lee_dat_trs) | ASND, EVI, TRSD, EVE, ACMXMONEDA, COL |
| INFO0101.FRM | Minfoeli_click | [CMXsrv_iinf_eli_inf](#cmxsrv_iinf_eli_inf) | INF, ARC |
| INFO0101.FRM | Minforev_Click | [CMXsrv_iinf_busc_evi](#cmxsrv_iinf_busc_evi) | EVI |
| INFO0101.FRM | Minfoval_click | [CMXsrv_iinf_val_inf](#cmxsrv_iinf_val_inf) | INF, ACMXPAIS, warnmsg |
| INFO0102.FRM | Aceptar_Click | [CMXsrv_iinf_ingmod_inf](#cmxsrv_iinf_ingmod_inf) | INF, tbl_User, warnmsg |
| INFO0102.FRM | Fec_pre | [CMXsrv_iinf_lee_fec](#cmxsrv_iinf_lee_fec) |  |
| INFO0102.FRM | fld_aux_glo_cls_com_LostFocus | [CMXsrv_iinf_lee_tablas](#cmxsrv_iinf_lee_tablas) | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM |
| INFO0102.FRM | fld_aux_glo_for_pag1_LostFocus | [CMXsrv_iinf_lee_tablas](#cmxsrv_iinf_lee_tablas) | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM |
| INFO0102.FRM | fld_aux_glo_for_pag2_LostFocus | [CMXsrv_iinf_lee_tablas](#cmxsrv_iinf_lee_tablas) | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM |
| INFO0102.FRM | fld_aux_glo_for_pag3_LostFocus | [CMXsrv_iinf_lee_tablas](#cmxsrv_iinf_lee_tablas) | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM |
| INFO0102.FRM | fld_aux_glo_mon_LostFocus | [CMXsrv_iinf_lee_tablas](#cmxsrv_iinf_lee_tablas) | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM |
| INFO0102.FRM | fld_inf_cls_com_Lostfocus | [CMXsrv_iinf_lee_tablas](#cmxsrv_iinf_lee_tablas) | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM |
| INFO0102.FRM | fld_inf_cod_imp_LostFocus | [CMXsrv_iinf_lee_cln](#cmxsrv_iinf_lee_cln) | CLN |
| INFO0102.FRM | fld_inf_for_pag1_lostfocus | [CMXsrv_iinf_lee_tablas](#cmxsrv_iinf_lee_tablas) | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM |
| INFO0102.FRM | fld_inf_for_pag2_LostFocus | [CMXsrv_iinf_lee_tablas](#cmxsrv_iinf_lee_tablas) | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM |
| INFO0102.FRM | fld_inf_for_pag3_LostFocus | [CMXsrv_iinf_lee_tablas](#cmxsrv_iinf_lee_tablas) | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM |
| INFO0102.FRM | fld_inf_mon_inf_lostfocus | [CMXsrv_iinf_lee_tablas](#cmxsrv_iinf_lee_tablas) | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM |
| INFO0102.FRM | Form_Load | [CMXsrv_iinf_lee0_inf](#cmxsrv_iinf_lee0_inf) | INF |
| INFO0102.FRM | Form_Load | [CMXsrv_iinf_lee1_inf](#cmxsrv_iinf_lee1_inf) | INF, CLN |
| INFO0102.FRM | Form_Load | [CMXsrv_iinf_lee2_inf](#cmxsrv_iinf_lee2_inf) | INF |
| INFO0102.FRM | valor_usd | [CMXsrv_iinf_lee_usd](#cmxsrv_iinf_lee_usd) |  |
| INFO0103.FRM | Aceptar_Click | [CMXsrv_iinf_busc_inf](#cmxsrv_iinf_busc_inf) | INF |
| INFO0103.FRM | buscar_Click | [CMXsrv_iinf_busc_inf](#cmxsrv_iinf_busc_inf) | INF |
| INFO0103.FRM | Fec_pre | [CMXsrv_iinf_lee_fec](#cmxsrv_iinf_lee_fec) |  |
| INFO0103.FRM | fld_inf_cod_imp_LostFocus | [CMXsrv_iinf_lee_cln](#cmxsrv_iinf_lee_cln) | CLN |
| INFO0103.FRM | PROXIMA_Click | [CMXsrv_iinf_busc_inf](#cmxsrv_iinf_busc_inf) | INF |
| INFO0104.FRM | Aceptar_Click | [CMXsrv_iinf_act_apr](#cmxsrv_iinf_act_apr) | INF |
| INFO0105.FRM | Form_Activate | [CMXsrv_iinf_busc_evi](#cmxsrv_iinf_busc_evi) | EVI |
| INFO0105.FRM | reversar_Click | [CMXsrv_iinf_rev_evi](#cmxsrv_iinf_rev_evi) | INF, ARC, INC, EVI |
| INFO0106.FRM | Form_Load | [CMXsrv_iinf_lee_evi](#cmxsrv_iinf_lee_evi) | EVI |
| INFO0107.FRM | Aceptar_Click | [CMXsrv_iinf_act_tib](#cmxsrv_iinf_act_tib) | INF |
| INFO0108.FRM | Aceptar_Click | [CMXsrv_iinf_act_rec](#cmxsrv_iinf_act_rec) | INF |
| INFO0109.FRM | Aceptar_Click | [CMXsrv_iinf_act_rib](#cmxsrv_iinf_act_rib) | INF |
| INFO0110.FRM | Form_Activate | [CMXsrv_iinf_busc_comp](#cmxsrv_iinf_busc_comp) | INF |
| INFO0110.FRM | proximos_Click | [CMXsrv_iinf_busc_comp](#cmxsrv_iinf_busc_comp) | INF |
| INFO0111.FRM | Aceptar_Click | [CMXsrv_iinf_ingmod_comp](#cmxsrv_iinf_ingmod_comp) | INF, warnmsg |
| INFO0111.FRM | Fec_pre | [CMXsrv_iinf_lee_fec](#cmxsrv_iinf_lee_fec) |  |
| INFO0111.FRM | Form_Activate | [CMXsrv_iinf_lee_comp](#cmxsrv_iinf_lee_comp) | INF |
| INFO0111.FRM | Form_Activate | [CMXsrv_iinf_lee_tablas](#cmxsrv_iinf_lee_tablas) | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM |
| INFO0112.FRM | aceptar_click | [CMXsrv_iinf_lee_bco](#cmxsrv_iinf_lee_bco) | COR |
| INFO0112.FRM | buscar_Click | [CMXsrv_iinf_busc_bco](#cmxsrv_iinf_busc_bco) | ACMXBCOBCC |
| PREFER.FRM | Form_Load | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |  |

---

## MOD_ADI
<a name="mod_adi"></a>

| **Archivo (Frame)** | **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** |
|--------------------|-------------|-----------------------------|----------------------|
| CRD00202.FRM | Aceptar_Click | [CMXsrv_icrd_a_cnd](#cmxsrv_icrd_a_cnd) | TIP, CRD_ADI, CRD, CRDCLON, COL_ADI, COM, ACMXMONEDA, LIB, comex..COL, MAPR, MCND, COL, ACMXOPEIMP, comex..CRD |
| CRD00202.FRM | busca_bco | [CMXsrv_icrd_lee_bco_swf](#cmxsrv_icrd_lee_bco_swf) | ACMXPAIS, COR |
| CRD00202.FRM | fld_col_fec_vto_LostFocus | [CMXsrv_util_det_habil](#cmxsrv_util_det_habil) | ACMXFERIADO |
| CRD00202.FRM | Form_Load | [CMXMCRDsrv_icrd_lee_mcnd](#cmxmcrdsrv_icrd_lee_mcnd) | CRD_ADI, ACMXFORPAG, CRD, PMIX, ACMXMONEDA, MPMIX, MCND |
| PREFER.FRM | Form_Load | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |  |

---

## MOD_CBR
<a name="mod_cbr"></a>

| **Archivo (Frame)** | **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** |
|--------------------|-------------|-----------------------------|----------------------|
| CBR00201.FRM | fld_cbr_cod_gdo_LostFocus | [CMXsrv_icbr_lee_cln](#cmxsrv_icbr_lee_cln) | CLN |
| CBR00201.FRM | Form_Load | [CMXsrv_icbr_lee_ctp](#cmxsrv_icbr_lee_ctp) | ACMXSUCSAL, MCBRCTP, CBR, ACMXPAIS, CLN, CBRANX |
| CBR00201.FRM | INGRESAR_Click | [CMXsrv_icbr_act_ctp](#cmxsrv_icbr_act_ctp) | comex..CBR, MCBRCTP, CBRANX, CBR |
| CBR00202.FRM | Form_Load | [CMXsrv_icbr_lee_trm](#cmxsrv_icbr_lee_trm) | ACMXVIATPT, CBR, ACMXINTERE, ACMXMONEDA, MCBRTER, ACMXCLACOM, ACMXPAIS |
| CBR00202.FRM | INGRESAR_Click | [CMXsrv_icbr_act_trm](#cmxsrv_icbr_act_trm) | LCB, COM, CBR, MCBRTER, warnmsg, CLN |
| CBR00203.FRM | Form_Load | [CMXsrv_icbr_lee_doc](#cmxsrv_icbr_lee_doc) | LCB, MCBRDOC, MLCB, CBR, ACMXMONEDA |
| CBR00203.FRM | INGRESAR_Click | [CMXsrv_icbr_act_doc](#cmxsrv_icbr_act_doc) | LCB, MCBRDOC, MLCB, CBR, comex..CBR |
| CBR00301.FRM | Form_Activate | [CMXsrv_icbr_busc_let](#cmxsrv_icbr_busc_let) | MLCB, comex..MLCB, comex..LCB |
| CBR00302.FRM | aceptar_Click | [CMXsrv_icbr_mod_ing_let](#cmxsrv_icbr_mod_ing_let) | LCB, MLCB, CBR, end |
| CBR00302.FRM | eliminar_Click | [CMXsrv_icbr_eli_let](#cmxsrv_icbr_eli_let) | LCB, MCBRDOC, MLCB, CBR, comex..COL |
| CBR00302.FRM | Form_Activate | [CMXsrv_icbr_lee_let](#cmxsrv_icbr_lee_let) | ACMXNOTARIO, LCB, MLCB |
| PANBASE.FRM | actualizar_Click | [CMXsrv_icbr_acep_mod_cbr](#cmxsrv_icbr_acep_mod_cbr) | LCB, MCBRDOC, MCBRCTP, MLCB, CBR, MCBRTER, warnmsg |
| PANBASE.FRM | Cancelar_Click | [CMXsrv_icbr_eli_no_cont](#cmxsrv_icbr_eli_no_cont) | MCBRDOC, MCBRCTP, MLCB, CBR, MCBRTER |

---

## MOD_CRD
<a name="mod_crd"></a>

| **Archivo (Frame)** | **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** |
|--------------------|-------------|-----------------------------|----------------------|
| BCO_BCO.FRM | Aceptar_Click | [CMXsrv_icrd_a_ibab](#cmxsrv_icrd_a_ibab) | MIBAB, IBAB |
| BCO_BCO.FRM | Form_Load | [CMXsrv_icrd_lee_glo_ibab](#cmxsrv_icrd_lee_glo_ibab) | IBAB, COL, MIBAB |
| BCO_REM.FRM | Aceptar_Click | [CMXsrv_icrd_a_ibar](#cmxsrv_icrd_a_ibar) | MIBAR, IBAR |
| BCO_REM.FRM | Form_Load | [CMXsrv_icrd_lee_glo_ibar](#cmxsrv_icrd_lee_glo_ibar) | MIBAR, COL, IBAR |
| BUSCADIR.FRM | buscar_click | [CMXsrv_icrd_lee_dir_cln](#cmxsrv_icrd_lee_dir_cln) | DIRCLN |
| BUSCA_TE.FRM | buscar_Click | [CMXsrv_icrd_lee_tex_swf](#cmxsrv_icrd_lee_tex_swf) | ACMXTSWFESPMSG, ACMXTSWFINGMSG |
| BUSC_COD.FRM | buscar_click | [CMXsrv_icrd_lee_tex_swf](#cmxsrv_icrd_lee_tex_swf) | ACMXTSWFESPMSG, ACMXTSWFINGMSG |
| BUSC_TXT.FRM | Aceptar_Click | [CMXsrv_icrd_lee_cod_txt_swf](#cmxsrv_icrd_lee_cod_txt_swf) | ACMXTSWFESPMSG, ACMXTSWFINGMSG |
| BUSC_TXT.FRM | buscar_click | [CMXsrv_icrd_lee_txt_swf_all](#cmxsrv_icrd_lee_txt_swf_all) | ACMXTSWFESPMSG, ACMXTSWFINGMSG |
| BUSC_TXT.FRM | Form_Load | [CMXsrv_icrd_lee_ind_esp_ing](#cmxsrv_icrd_lee_ind_esp_ing) | MCTP, CRD |
| BUSC_TXT.FRM | llena_arreglo | [CMXsrv_icrd_lee_tex_swf](#cmxsrv_icrd_lee_tex_swf) | ACMXTSWFESPMSG, ACMXTSWFINGMSG |
| BUSC_TXT.FRM | proximo_Click | [CMXsrv_icrd_lee_txt_swf_all](#cmxsrv_icrd_lee_txt_swf_all) | ACMXTSWFESPMSG, ACMXTSWFINGMSG |
| CONDESP.FRM | Aceptar_Click | [CMXMCRDsrv_icrd_a_mmcnd](#cmxmcrdsrv_icrd_a_mmcnd) | MMCND |
| CONDESP.FRM | Form_Load | [CMXsrv_icrd_lee_cnd_esp](#cmxsrv_icrd_lee_cnd_esp) | MMCND, COL, CND |
| CRD00201.FRM | Aceptar_Click | [CMXsrv_icrd_a_ctp](#cmxsrv_icrd_a_ctp) | CRD, CRDCLON, MCTP, comex..COL, COL |
| CRD00201.FRM | FLD_COL_COD_CLI_LostFocus | [CMXsrv_icrd_lee_cln](#cmxsrv_icrd_lee_cln) | CLN, DIRCLN |
| CRD00201.FRM | Form_Load | [CMXMCRDsrv_icrd_lee_mctp](#cmxmcrdsrv_icrd_lee_mctp) | ACMXPAIS, MCTP, DIRCLN, CRD |
| CRD00202.FRM | Aceptar_Click | [CMXsrv_icrd_a_cnd](#cmxsrv_icrd_a_cnd) | TIP, CRD_ADI, CRD, CRDCLON, COL_ADI, COM, ACMXMONEDA, LIB, comex..COL, MAPR, MCND, COL, ACMXOPEIMP, comex..CRD |
| CRD00202.FRM | Form_Load | [CMXMCRDsrv_icrd_lee_mcnd](#cmxmcrdsrv_icrd_lee_mcnd) | CRD_ADI, ACMXFORPAG, CRD, PMIX, ACMXMONEDA, MPMIX, MCND |
| CRD00203.FRM | Form_Activate | [CMXsrv_icrd_busc_emb](#cmxsrv_icrd_busc_emb) | comex..EMB, comex..MEMB |
| CRD00204.FRM | cancelar_Click | [CMXsrv_icrd_lee_desc_merc](#cmxsrv_icrd_lee_desc_merc) | MMER, MER |
| CRD00204.FRM | ELIMINAR_Click | [CMXsrv_icrd_eli_emb](#cmxsrv_icrd_eli_emb) | comex..COL, EMB, COL, CRD |
| CRD00204.FRM | Form_Load | [CMXMCRDsrv_icrd_lee_memb2](#cmxmcrdsrv_icrd_lee_memb2) | MEMB, EMB |
| CRD00204.FRM | Form_Load | [CMXMCRDsrv_icrd_lee_memb1](#cmxmcrdsrv_icrd_lee_memb1) | CRS, MEMB, EMB, MCRS |
| CRD00204.FRM | ingresar_Click | [CMXsrv_icrd_a_emb1](#cmxsrv_icrd_a_emb1) | CRS, MEMB, CRD, MCRS, CRDCLON, COL, EMB |
| CRD00204.FRM | ingresar_Click | [CMXsrv_icrd_a_emb2](#cmxsrv_icrd_a_emb2) | EMB, COL, MEMB, CRD |
| CRD00204.FRM | VALIDA_EMBARQUE | [CMXsrv_icrd_val_emb2](#cmxsrv_icrd_val_emb2) | warnmsg |
| CRD00204.FRM | VALIDA_EMBARQUE | [CMXsrv_icrd_val_emb1](#cmxsrv_icrd_val_emb1) | INF, ARC, warnmsg |
| CRD00205.FRM | Aceptar_Click | [CMXsrv_icrd_act_ref](#cmxsrv_icrd_act_ref) | MREF, CRD, CRDCLON, comex..MREF, comex..COL, COL |
| CRD00205.FRM | fld_obl_cod_bco_acre_DblClick | [CMXsrv_icrd_lee_bco_swf](#cmxsrv_icrd_lee_bco_swf) | ACMXPAIS, COR |
| CRD00205.FRM | fld_obl_cod_bco_acre_LostFocus | [CMXsrv_icrd_lee_bco_swf](#cmxsrv_icrd_lee_bco_swf) | ACMXPAIS, COR |
| CRD00205.FRM | Form_Load | [CMXMCRDsrv_icrd_lee_mref](#cmxmcrdsrv_icrd_lee_mref) | MREF, COR, COL, CRD |
| CRD00206.FRM | Aceptar_Click | [CMXsrv_icrd_ing_txt](#cmxsrv_icrd_ing_txt) | MTXT |
| CRD00206.FRM | Form_Load | [CMXCRDsrv_icrd_get_ing_esp](#cmxcrdsrv_icrd_get_ing_esp) | ACMXPAIS, MCTP, CRD |
| CRD00206.FRM | Form_Load | [CMXMCRDsrv_icrd_lee_mtxt](#cmxmcrdsrv_icrd_lee_mtxt) | MTXT |
| CRD00207.FRM | Form_Load | [CMXCRDsrv_icrd_get_pre_fra](#cmxcrdsrv_icrd_get_pre_fra) | ACMXTSWFESPMSG, ACMXTSWFINGMSG |
| DESCMERC.FRM | Aceptar_Click | [CMXMCRDsrv_icrd_a_mmer](#cmxmcrdsrv_icrd_a_mmer) | MMER |
| DESCMERC.FRM | Form_Load | [CMXsrv_icrd_lee_desc_merc](#cmxsrv_icrd_lee_desc_merc) | MMER, MER |
| DOCUME.FRM | Aceptar_Click | [CMXsrv_icrd_a_otr_doc](#cmxsrv_icrd_a_otr_doc) | ODOC, MODOC |
| DOCUME.FRM | Form_Load | [CMXsrv_icrd_lee_otr_doc](#cmxsrv_icrd_lee_otr_doc) | ODOC, MODOC |
| MOD00603.FRM | Aceptar_Click | [CMXsrv_fincol_lee_cod_eve](#cmxsrv_fincol_lee_cod_eve) | MCND, COL, CRD, COM |
| MOD00603.FRM | Aceptar_Click | [CMXMCRDsrv_icrd_acep_mod_crd](#cmxmcrdsrv_icrd_acep_mod_crd) | de, TIP, CRD, COD, MCRS, OBL, EVE, LIB, warnmsg, OPE_BCI, sysobjects, COL |
| MOD00603.FRM | cancelar_Click | [CMXMCRDsrv_icrd_eli_no_cont](#cmxmcrdsrv_icrd_eli_no_cont) | MREF, MEMB, MCRS, MMCND, COM, MODOC, MIBAB, CRD_AMD, MPMIX, MCTP, MMER, MCND, MIBAR, TNIH, MAPR, FE_IN_REJECTED_TRANS, MTXT |
| MOD00603.FRM | fld_crd_cod_bco_rem_LostFocus | [CMXsrv_icrd_lee_bco_swf](#cmxsrv_icrd_lee_bco_swf) | ACMXPAIS, COR |
| MOD00603.FRM | fld_crd_fec_mod_lostFocus | [CMXsrv_fincol_efec_calpa](#cmxsrv_fincol_efec_calpa) | TF_PPAG, TIP, TAS, CUO, comex..ACMXMONEDA, COL_ADI, OBL, CTR, NEG_ADI, ACMXINTERE, CAN, ICR, COL |
| MOD00603.FRM | Form_Activate | [CMXsrv_icrd_lee_ind_esp_ing](#cmxsrv_icrd_lee_ind_esp_ing) | MCTP, CRD |
| MOD00603.FRM | Form_Load | [CMXsrv_fincol_efec_calpa](#cmxsrv_fincol_efec_calpa) | TF_PPAG, TIP, TAS, CUO, comex..ACMXMONEDA, COL_ADI, OBL, CTR, NEG_ADI, ACMXINTERE, CAN, ICR, COL |
| MOD00603.FRM | Form_Load | [CMXMCRDsrv_icrd_lee_mcnd](#cmxmcrdsrv_icrd_lee_mcnd) | CRD_ADI, ACMXFORPAG, CRD, PMIX, ACMXMONEDA, MPMIX, MCND |
| PREFER.FRM | Form_Load | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |  |

---

## NEGO_AV
<a name="nego_av"></a>

| **Archivo (Frame)** | **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** |
|--------------------|-------------|-----------------------------|----------------------|
| AVISOS.FRM | aviso1 | [CMXsrv_icrd_a_rec_age](#cmxsrv_icrd_a_rec_age) | COR, TAS, CRD, CUO, CNEG, COM, NEG, TRSD, DIS, EVE, ACMXMONEDA, ACMXINTERE, ACMXSUCSAL, COL |
| AVISOS.FRM | aviso1 | [CMXsrv_busc_ofi_cta](#cmxsrv_busc_ofi_cta) | CLN |
| AVISOS.FRM | aviso1 | [CMXsrv_neg_busc_arc](#cmxsrv_neg_busc_arc) | ARC |
| AVISOS.FRM | aviso1 | [CMXsrv_icrd_lee_avi_adi](#cmxsrv_icrd_lee_avi_adi) | CRD |
| AVISOS.FRM | aviso3 | [CMXsrv_icrd_lee_dat_trs](#cmxsrv_icrd_lee_dat_trs) | ASND, EVI, TRSD, EVE, ACMXMONEDA, COL |
| AVISOS.FRM | Aviso4 | [CMXsrv_icrd_dat_liq_ope](#cmxsrv_icrd_dat_liq_ope) | ACMXDESEMB, ASND, EVO, CRD, CNO, OBL, CUO, TRSD, NEG, COM, EVE, ACMXTIPEVE, CAN, COL |
| AVISOS.FRM | Aviso4 | [CMXsrv_icrd_lee_dat_cln](#cmxsrv_icrd_lee_dat_cln) | NEG, CLN, COL |
| AVISOS.FRM | Aviso5 | [CMXsrv_icrd_lee_dat_cln](#cmxsrv_icrd_lee_dat_cln) | NEG, CLN, COL |
| AVISOS.FRM | Aviso5 | [CMXsrv_icrd_lee_avi_dis](#cmxsrv_icrd_lee_avi_dis) | DIS, COL |
| AVISOS.FRM | Aviso5 | [CMXsrv_icrd_lee_avi_adi](#cmxsrv_icrd_lee_avi_adi) | CRD |
| AVISOS.FRM | Aviso5 | [CMXsrv_neg_ddi_asoc](#cmxsrv_neg_ddi_asoc) | ADI |
| AVISOS.FRM | Aviso5 | [CMXsrv_neg_busc_arc](#cmxsrv_neg_busc_arc) | ARC |
| AVISOS.FRM | Aviso5 | [CMXsrv_neg_trae_vcto_mcf](#cmxsrv_neg_trae_vcto_mcf) | COL, CUO |
| AVISOS.FRM | lee_aval | [CMXsrv_neg_avi_lee_aval](#cmxsrv_neg_avi_lee_aval) | TAS, CNEG, AVAL, CLN, COL |
| AVISOS.FRM | lee_nego | [CMXsrv_icrd_neg_lee_crd](#cmxsrv_icrd_neg_lee_crd) | NEG, COL |
| AVISOS.FRM | lee_nego | [CMXsrv_icrd_lee_neg](#cmxsrv_icrd_lee_neg) | TAS, CRD, ACMXFINVER, NEG, NEG_ADI, DIS, COL |
| AVI_COL.FRM | avi_col1 | [CMXsrv_col_avi_dat_cln](#cmxsrv_col_avi_dat_cln) | TIP, CRD, DAC, ACMXESPECI, ACMXSUCSAL, CLN, COL, ACLNEJECTA |
| AVI_COL.FRM | avi_col1 | [CMXsrv_col_avi_det_pag](#cmxsrv_col_avi_det_pag) | CCX, TIP, TAS, CRD, COB, ACMXINTERE, EVE, ACMXMONEDA, ACMXINTEREFEC, CAN, CAN_REN, COL |
| AVI_COL.FRM | avi_col2 | [CMXsrv_col_avi_dat_cln](#cmxsrv_col_avi_dat_cln) | TIP, CRD, DAC, ACMXESPECI, ACMXSUCSAL, CLN, COL, ACLNEJECTA |
| AVI_COL.FRM | avi_col2 | [CMXsrv_col_avi_det_oto](#cmxsrv_col_avi_det_oto) | TIP, ACMXDESEMB, ASND, TAS, CUO, COD, NEG, ACMXINTERE, EVE, ACMXMONEDA, ACMXINTEREFEC, AVAL, CLN, COL |
| AVI_COL.FRM | avi_col4 | [CMXsrv_col_avi_dat_cln](#cmxsrv_col_avi_dat_cln) | TIP, CRD, DAC, ACMXESPECI, ACMXSUCSAL, CLN, COL, ACLNEJECTA |
| AVI_COL.FRM | avi_col4 | [CMXsrv_col_lee_num_trs](#cmxsrv_col_lee_num_trs) | EVE, COL, TIP, COD |
| AVI_COL.FRM | lee_obl_pag | [CMXsrv_finobl_avi_pag](#cmxsrv_finobl_avi_pag) | CNO, EVO |
| AVI_COL.FRM | traspaso | [CMXsrv_neg_avi_trae_asnd_mn](#cmxsrv_neg_avi_trae_asnd_mn) | ACMXDESEMB, ASND, COD, TRSD, ACMXMONEDA |
| AVI_COL.FRM | traspaso | [CMXsrv_neg_avi_trae_asnd_mx](#cmxsrv_neg_avi_trae_asnd_mx) | ACMXDESEMB, ACMXMONEDA, ASND |
| CRD01001.FRM | Form_Activate | [CMXsrv_icrd_neg_lee_crd](#cmxsrv_icrd_neg_lee_crd) | NEG, COL |
| CRD01001.FRM | Form_Activate | [CMXsrv_icrd_lee_neg](#cmxsrv_icrd_lee_neg) | TAS, CRD, ACMXFINVER, NEG, NEG_ADI, DIS, COL |
| CRD01001.FRM | Mcrdtxtliq_Click | [CMXsrv_icrd_lee_dat_trs](#cmxsrv_icrd_lee_dat_trs) | ASND, EVI, TRSD, EVE, ACMXMONEDA, COL |
| CRD01001.FRM | Mcrdtxtope_Click | [CMXsrv_icrd_dat_liq_ope](#cmxsrv_icrd_dat_liq_ope) | ACMXDESEMB, ASND, EVO, CRD, CNO, OBL, CUO, TRSD, NEG, COM, EVE, ACMXTIPEVE, CAN, COL |
| CRD01001.FRM | MNEGCONT_Click | [CMXsrv_icrd_cont_neg](#cmxsrv_icrd_cont_neg) | COL, NEG, CRD, COD |
| CRD01001.FRM | MNEGELI_CLICK | [CMXsrv_icrd_eli_neg](#cmxsrv_icrd_eli_neg) | CRD, COM, NEG, CND, NEG_ADI, ACMXTXTSWF, comex..COL |
| CRD01001.FRM | precarga_datos | [CMXsrv_icrd_a_rec_age](#cmxsrv_icrd_a_rec_age) | COR, TAS, CRD, CUO, CNEG, COM, NEG, TRSD, DIS, EVE, ACMXMONEDA, ACMXINTERE, ACMXSUCSAL, COL |
| CRD01001.FRM | precarga_datos | [CMXsrv_busc_ofi_cta](#cmxsrv_busc_ofi_cta) | CLN |
| PREFER.FRM | Form_Load | [CMXsrv_trae_glo_fec](#cmxsrv_trae_glo_fec) | ACMXSUCSAL, ACMXDL3475FEC, tbl_User |
| PREFER.FRM | Form_Load | [CMXsrv_icrd_lee_num_col](#cmxsrv_icrd_lee_num_col) | COL |
| VER_PAGO.FRM | Form_Load | [CMXsrv_icrd_bus_pago](#cmxsrv_icrd_bus_pago) | CAN |

---

## NNEGO
<a name="nnego"></a>

| **Archivo (Frame)** | **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** |
|--------------------|-------------|-----------------------------|----------------------|
| CRD01001.FRM | Form_Activate | [CMXsrv_icrd_neg_lee_crd](#cmxsrv_icrd_neg_lee_crd) | NEG, COL |
| CRD01001.FRM | Form_Activate | [CMXsrv_icrd_lee_neg](#cmxsrv_icrd_lee_neg) | TAS, CRD, ACMXFINVER, NEG, NEG_ADI, DIS, COL |
| CRD01001.FRM | gen_mens_swift | [CMXsrv_iswf_a_pru](#cmxsrv_iswf_a_pru) | switxt, switxt1 |
| CRD01001.FRM | llama_pagos | [CMXsrv_icrd_lee_col](#cmxsrv_icrd_lee_col) | CCL, COL, TAS |
| CRD01001.FRM | Mnegavi9_Click | [CMXsrv_iswf_a_pru](#cmxsrv_iswf_a_pru) | switxt, switxt1 |
| CRD01001.FRM | MNEGCONT_Click | [CMXsrv_icrd_cont_neg](#cmxsrv_icrd_cont_neg) | COL, NEG, CRD, COD |
| CRD01001.FRM | MNEGELI_CLICK | [CMXsrv_icrd_eli_neg](#cmxsrv_icrd_eli_neg) | CRD, COM, NEG, CND, NEG_ADI, ACMXTXTSWF, comex..COL |
| CRD01001.FRM | pertas_Click | [CMXsrv_icrd_lee_col](#cmxsrv_icrd_lee_col) | CCL, COL, TAS |
| CRD01002.FRM | Form_Activate | [CMXsrv_icrd_busc_neg](#cmxsrv_icrd_busc_neg) | NEG |
| CRD01003.FRM | Form_Load | [CMXsrv_icrd_busc_emb](#cmxsrv_icrd_busc_emb) | comex..EMB, comex..MEMB |
| CRD01005.FRM | ACEPTAR_Click | [CMXsrv_icrd_a_neg_emb1](#cmxsrv_icrd_a_neg_emb1) | TAS, CNEG, NEG, COL, DOCNEG |
| CRD01005.FRM | ACEPTAR_Click | [CMXsrv_icrd_a_neg_emb2](#cmxsrv_icrd_a_neg_emb2) | NEG, COL, comex..COL, DOCNEG |
| CRD01005.FRM | CANCELAR_Click | [CMXsrv_icrd_eli_doc_neg](#cmxsrv_icrd_eli_doc_neg) | COL, DOCNEG |
| CRD01005.FRM | Form_Activate | [CMXsrv_icrd_lee_emb1](#cmxsrv_icrd_lee_emb1) | CRS, COL, EMB |
| CRD01005.FRM | Form_Activate | [CMXsrv_icrd_lee_emb2](#cmxsrv_icrd_lee_emb2) | COL, EMB |
| CRD01005.FRM | Form_Activate | [CMXsrv_icrd_lee_neg_emb1](#cmxsrv_icrd_lee_neg_emb1) | COL, NEG |
| CRD01005.FRM | Form_Activate | [CMXsrv_icrd_lee_neg_emb2](#cmxsrv_icrd_lee_neg_emb2) | COL, NEG |
| CRD01005.FRM | Form_Activate | [CMXsrv_icrd_lee_cnd_esp](#cmxsrv_icrd_lee_cnd_esp) | MMCND, COL, CND |
| CRD01005.FRM | Form_Activate | [CMXsrv_icrd_lee_desc_merc](#cmxsrv_icrd_lee_desc_merc) | MMER, MER |
| CRD01006.FRM | ACEPTAR_Click | [CMXsrv_icrd_a_neg_disc](#cmxsrv_icrd_a_neg_disc) | COL, DIS, NEG |
| CRD01006.FRM | Form_Load | [CMXsrv_icrd_neg_lee_disc](#cmxsrv_icrd_neg_lee_disc) | DIS, NEG |
| CRD01201.FRM | ACEPTAR_Click | [CMXsrv_icrd_ent_doc](#cmxsrv_icrd_ent_doc) | COL, NEG, comex..COL |
| CRD01201.FRM | ELIMINAR_Click | [CMXsrv_icrd_ent_doc](#cmxsrv_icrd_ent_doc) | COL, NEG, comex..COL |
| CRD01201.FRM | Form_Load | [CMXsrv_icrd_ent_doc](#cmxsrv_icrd_ent_doc) | COL, NEG, comex..COL |
| CRD01301.FRM | ACEPTAR_Click | [CMXsrv_icrd_alz_disc](#cmxsrv_icrd_alz_disc) | comex..ACMXINTEREFEC, COR, TAS, CRD, CUO, COD, CNEG, NEG, ACMXMONEDAFEC, NEG_ADI, ACMXINTERE, ACMXBCOUSU, ACMXINTEREFEC, sysobjects, COL |
| CRD02001.FRM | aceptar_click | [CMXCRDsrv_icrd_asignar_cor](#cmxcrdsrv_icrd_asignar_cor) | COR, ACMXMONEDAFEC, CRD, LCR |
| CRD02001.FRM | BUSCAR_Click | [CMXCRDsrv_icrd_bus_lcr_bco](#cmxcrdsrv_icrd_bus_lcr_bco) | COR |
| CRD02001.FRM | proximo_Click | [CMXCRDsrv_icrd_bus_lcr_bco](#cmxcrdsrv_icrd_bus_lcr_bco) | COR |
| CRD02004.FRM | ACEPTAR_Click | [CMXsrv_icrd_act_doc_neg](#cmxsrv_icrd_act_doc_neg) | NEG, COL, DOCNEG |
| CRD02004.FRM | Form_Load | [CMXsrv_icrd_lee_doc_neg](#cmxsrv_icrd_lee_doc_neg) | NEG, EMB |
| GRL00101.FRM | enviar_Click | [CMXsrv_iswf_a_pru](#cmxsrv_iswf_a_pru) | switxt, switxt1 |
| GRL00101.FRM | Form_Load | [CMXsrv_icrd_val_neg](#cmxsrv_icrd_val_neg) | DDI, COR, ADI, TAS, CUO, NEG, ACMXMONEDAFEC, DAC, ACMXINTERE, ACMXMONEDA, ACMXSIGGAR, ACMXINTEREFEC, CAN, DIS, warnmsg, AVAL, COL, CCO |
| PREFER.FRM | Form_Load | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |  |
| VER_PAGO.FRM | Form_Load | [CMXsrv_icrd_bus_pago](#cmxsrv_icrd_bus_pago) | CAN |

---

## PAGCBR
<a name="pagcbr"></a>

| **Archivo (Frame)** | **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** |
|--------------------|-------------|-----------------------------|----------------------|
| CBR01006.FRM | ACEPTAR_Click | [CMXsrv_icbr_lee_dat_var](#cmxsrv_icbr_lee_dat_var) | ACMXMONEDAFEC, CBR, ACMXPRMENL |
| CBR01006.FRM | ACEPTAR_Click | [CMXsrv_icbr_val_pag](#cmxsrv_icbr_val_pag) | LCB, CBR, CCO |
| CBR01006.FRM | ACEPTAR_Click | [CMXsrv_icbr_ctb_pag](#cmxsrv_icbr_ctb_pag) | LCB, ACMXDESEMB, vig_cmx, COD, ICX, COM, ACMXMONEDAFEC, CBR, PCX, DIP, LIB, CLN, CCO |
| CBR01006.FRM | Calcular_Click | [CMXsrv_icbr_cal_pag](#cmxsrv_icbr_cal_pag) | DDI, ADI, ACMXMONEDAFEC, CBR, COB, ACMXMONEDA |
| CBR01006.FRM | CANCELAR_Click | [CMXsrv_icbr_eli_pag](#cmxsrv_icbr_eli_pag) | ECE, PCX, COB, ICX |
| CBR01006.FRM | fld_cbr_cod_des_mn_pag_lostfocus | [CMXsrv_val_vig](#cmxsrv_val_vig) | ACMXPLNCTAN, ACMXDESEMB, ACMXPLNCTAX |
| CBR01006.FRM | fld_cbr_cod_des_mx_pag_lostfocus | [CMXsrv_val_vig](#cmxsrv_val_vig) | ACMXPLNCTAN, ACMXDESEMB, ACMXPLNCTAX |
| CBR01006.FRM | Form_Load | [CMXsrv_icbr_lee_cbr0](#cmxsrv_icbr_lee_cbr0) | ACMXMONEDA, CBR |
| CBR01006.FRM | Form_Load | [CMXsrv_icbr_obt_mon_nac](#cmxsrv_icbr_obt_mon_nac) |  |
| CBR01006.FRM | Form_Load | [CMXsrv_icbr_lee_dat_pag](#cmxsrv_icbr_lee_dat_pag) | ACMXDESEMB, ECE, PCX, CBR |
| CBR01006.FRM | Form_Load | [CMXsrv_icbr_pcg_pag](#cmxsrv_icbr_pcg_pag) | ACMXMONEDAFEC, CBR |
| CBR01006.FRM | lee_cta | [CMXsrv_vig_lee_cta](#cmxsrv_vig_lee_cta) | ACMXPLNCTAN, ACMXDESEMB, ACMXPLNCTAX |
| CBR01007.FRM | Form_Activate | [CMXsrv_icbr_busc_pago](#cmxsrv_icbr_busc_pago) | PCX |
| CBR01008.FRM | ACEPTAR_Click | [CMXsrv_icbr_val_pag](#cmxsrv_icbr_val_pag) | LCB, CBR, CCO |
| COB00303.FRM | Aceptar_Click | [CMXsrv_icob_act_val](#cmxsrv_icob_act_val) | ACMXMONEDAFEC, COB |
| COB00303.FRM | Form_Activate | [CMXsrv_icob_lee_val](#cmxsrv_icob_lee_val) | COB |
| COB00305.FRM | ELIMINAR_Click | [CMXsrv_icbr_eli_int_pago](#cmxsrv_icbr_eli_int_pago) | PCX, ICX |
| COB00305.FRM | Form_Activate | [CMXsrv_icbr_busc_int](#cmxsrv_icbr_busc_int) | ICX |
| COB00306.FRM | Aceptar_Click | [CMXsrv_icbr_ingmod_int](#cmxsrv_icbr_ingmod_int) | PCX, CBR, ICX, ACMXINTEREFEC |
| COB00306.FRM | Form_Activate | [CMXsrv_icbr_lee_int_pago](#cmxsrv_icbr_lee_int_pago) | ICX |
| CRD00602.FRM | Aceptar_Click | [CMXsrv_icbr_lee_bco](#cmxsrv_icbr_lee_bco) | ACMXPAIS, COR |
| CRD00602.FRM | buscar_Click | [CMXsrv_icbr_busc_bco](#cmxsrv_icbr_busc_bco) | COR |
| PREFER.FRM | Form_Load | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |  |

---

# Procedimientos Referenciados

## CMXsrv_expcbe_lee_prm
<a name="cmxsrv_expcbe_lee_prm"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBE00101.FRM**: [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)
- **Exportaciones → expdex → DEX00101.FRM**: [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)
- **Exportaciones → EXPCBE → CBE00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → expdex → DEX00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_cmx_busc_suc_usu
<a name="cmxsrv_cmx_busc_suc_usu"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCCE → CCE00101.FRM**: [CMXsrv_cmx_ing_lib](#referencia-cmxsrv_cmx_ing_lib)
- **Exportaciones → expret → RET00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → expret → RET00101.FRM**: [CMXsrv_cmx_ing_lib](#referencia-cmxsrv_cmx_ing_lib)
- **Exportaciones → EXPCBE → CBE00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCBE → CBE00101.FRM**: [CMXsrv_cmx_ing_lib](#referencia-cmxsrv_cmx_ing_lib)
- **Exportaciones → EXPCCE → CCE00101.FRM**: [PrmACMXSUCSAL](#referencia-prmacmxsucsal)
- **Exportaciones → expret → RET00101.FRM**: [PrmACMXSUCSAL](#referencia-prmacmxsucsal)
- **Exportaciones → EXPCBE → CBE00101.FRM**: [PrmACMXSUCSAL](#referencia-prmacmxsucsal)
- **Exportaciones → EXPCCE → CCE00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_lee_cbe
<a name="cmxsrv_expcbe_lee_cbe"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBE00605.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCBE → CBE00301.FRM**: [CMXsrv_cmx_busc_suc_usu](#referencia-cmxsrv_cmx_busc_suc_usu)
- **Exportaciones → EXPCBE → CBE00101.FRM**: [CMXsrv_val_suc](#referencia-cmxsrv_val_suc)
- **Exportaciones → EXPCBE → CBE00101.FRM**: [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)
- **Exportaciones → EXPCBE → CBE00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCBE → CBE00301.FRM**: [CMXsrv_val_suc](#referencia-cmxsrv_val_suc)
- **Exportaciones → EXPCBE → CBE00605.FRM**: [CMXsrv_cmx_busc_suc_usu](#referencia-cmxsrv_cmx_busc_suc_usu)
- **Exportaciones → EXPCBE → CBE00101.FRM**: [CMXsrv_cmx_busc_suc_usu](#referencia-cmxsrv_cmx_busc_suc_usu)
- **Exportaciones → EXPCBE → CBE00301.FRM**: [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)
- **Exportaciones → EXPCBE → CBE00301.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCBE → CBE00605.FRM**: [CMXsrv_val_suc](#referencia-cmxsrv_val_suc)
- **Exportaciones → EXPCBE → CBE00605.FRM**: [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)

---

## CMXsrv_trae_glo_fec
<a name="cmxsrv_trae_glo_fec"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → NEGO_AV → PREFER.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCBE → CBE00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → IMPORT → CRD00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_avs_cyg1
<a name="cmxsrv_expcbe_avs_cyg1"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBE00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_avs_cyg2
<a name="cmxsrv_expcbe_avs_cyg2"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBE00101.FRM**: [por](#referencia-por)
- **Exportaciones → EXPCBE → CBE00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_avs_ret
<a name="cmxsrv_expcbe_avs_ret"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBE00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_swf_sel
<a name="cmxsrv_expcbe_swf_sel"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBE00101.FRM**: [CMXsrv_expcbe_swf_420](#referencia-cmxsrv_expcbe_swf_420)
- **Exportaciones → EXPCBE → GRL00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCBE → GRL00101.FRM**: [CMXsrv_expcbe_swf_430](#referencia-cmxsrv_expcbe_swf_430)
- **Exportaciones → EXPCBE → GRL00101.FRM**: [CMXsrv_expcbe_swf_422](#referencia-cmxsrv_expcbe_swf_422)
- **Exportaciones → EXPCBE → CBE00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCBE → GRL00101.FRM**: [CMXsrv_expcbe_swf_499](#referencia-cmxsrv_expcbe_swf_499)
- **Exportaciones → EXPCBE → CBE00101.FRM**: [CMXsrv_expcbe_swf_430](#referencia-cmxsrv_expcbe_swf_430)
- **Exportaciones → EXPCBE → CBE00101.FRM**: [CMXsrv_expcbe_swf_422](#referencia-cmxsrv_expcbe_swf_422)
- **Exportaciones → EXPCBE → CBE00101.FRM**: [CMXsrv_expcbe_swf_499](#referencia-cmxsrv_expcbe_swf_499)
- **Exportaciones → EXPCBE → GRL00101.FRM**: [CMXsrv_expcbe_swf_420](#referencia-cmxsrv_expcbe_swf_420)

---

## CMXsrv_expcbe_anl_cbe
<a name="cmxsrv_expcbe_anl_cbe"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBE00101.FRM**: [CMXsrv_cnt_630](#referencia-cmxsrv_cnt_630)
- **Exportaciones → EXPCBE → CBE00101.FRM**: [CMXsrv_expcbe_grb_evz](#referencia-cmxsrv_expcbe_grb_evz)
- **Exportaciones → EXPCBE → CBE00101.FRM**: [CMXsrv_cnt_950](#referencia-cmxsrv_cnt_950)
- **Exportaciones → EXPCBE → CBE00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCBE → CBE00101.FRM**: [CMXsrv_cnt_gen_vig](#referencia-cmxsrv_cnt_gen_vig)

---

## CMXsrv_expcbe_ctb_ing
<a name="cmxsrv_expcbe_ctb_ing"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBE00101.FRM**: [CMXsrv_mbyte_gen](#referencia-cmxsrv_mbyte_gen)
- **Exportaciones → EXPCBE → CBE00101.FRM**: [CMXsrv_cnt_600](#referencia-cmxsrv_cnt_600)
- **Exportaciones → EXPCBE → CBE00101.FRM**: [CMXsrv_expcbe_grb_evz](#referencia-cmxsrv_expcbe_grb_evz)
- **Exportaciones → EXPCBE → CBE00101.FRM**: [CMXsrv_nibx_upd_tran](#referencia-cmxsrv_nibx_upd_tran)
- **Exportaciones → EXPCBE → CBE00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCBE → CBE00101.FRM**: [CMXsrv_cnt_950](#referencia-cmxsrv_cnt_950)
- **Exportaciones → EXPCBE → CBE00101.FRM**: [CMXsrv_nibx_nilive](#referencia-cmxsrv_nibx_nilive)
- **Exportaciones → EXPCBE → CBE00101.FRM**: [CMXsrv_expcbe_val_cbe](#referencia-cmxsrv_expcbe_val_cbe)
- **Exportaciones → EXPCBE → CBE00101.FRM**: [CMXsrv_cnt_gen_vig](#referencia-cmxsrv_cnt_gen_vig)

---

## CMXsrv_expcbe_del_cbe
<a name="cmxsrv_expcbe_del_cbe"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBE00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_val_cbe
<a name="cmxsrv_expcbe_val_cbe"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBE00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_grb_ctp
<a name="cmxsrv_expcbe_grb_ctp"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBE00201.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_lee_cln
<a name="cmxsrv_expcbe_lee_cln"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBE00201.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCBE → CBE00605.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCBE → CBE00301.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_val_suc
<a name="cmxsrv_val_suc"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBE00201.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → COBRANZA → CBR00102.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → COBRANZA → CBR00901.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → COBRANZA → CBR00103.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCBE → CBE00401.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_lee_ctp
<a name="cmxsrv_expcbe_lee_ctp"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBE00201.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_grb_bco
<a name="cmxsrv_expcbe_grb_bco"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBE00202.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_lee_cor
<a name="cmxsrv_expcbe_lee_cor"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBE00501.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCBE → CRD00602.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCBE → GRLPAIS0.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → expret → CRD00602.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCBE → CBE00202.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_lee_bco
<a name="cmxsrv_expcbe_lee_bco"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBE00202.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCBE → CBE00202.FRM**: [CMXsrv_icrd_lee_cln](#referencia-cmxsrv_icrd_lee_cln)

---

## CMXsrv_expcbe_grb_doc
<a name="cmxsrv_expcbe_grb_doc"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBE00204.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_grb_doc02
<a name="cmxsrv_expcbe_grb_doc02"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBE00204.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_lee_doc
<a name="cmxsrv_expcbe_lee_doc"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBE00204.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_lee_doc02
<a name="cmxsrv_expcbe_lee_doc02"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBE00204.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_del_ctz
<a name="cmxsrv_expcbe_del_ctz"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBE00206.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_bus_ctz
<a name="cmxsrv_expcbe_bus_ctz"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBE00206.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_grb_ctz
<a name="cmxsrv_expcbe_grb_ctz"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBE00207.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_mto_ctz
<a name="cmxsrv_expcbe_mto_ctz"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBE00207.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_lee_ctz
<a name="cmxsrv_expcbe_lee_ctz"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBE00207.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_bus_cbe
<a name="cmxsrv_expcbe_bus_cbe"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBE00301.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_mdf_cbe
<a name="cmxsrv_expcbe_mdf_cbe"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBE00401.FRM**: [CMXsrv_cnt_610](#referencia-cmxsrv_cnt_610)
- **Exportaciones → EXPCBE → CBE00401.FRM**: [CMXsrv_cnt_gen_vig](#referencia-cmxsrv_cnt_gen_vig)
- **Exportaciones → EXPCBE → CBE00401.FRM**: [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)
- **Exportaciones → EXPCBE → CBE00401.FRM**: [CMXsrv_expcbe_grb_evl](#referencia-cmxsrv_expcbe_grb_evl)
- **Exportaciones → EXPCBE → CBE00401.FRM**: [CMXsrv_expcbe_grb_evz](#referencia-cmxsrv_expcbe_grb_evz)
- **Exportaciones → EXPCBE → CBE00401.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCBE → CBE00401.FRM**: [CMXsrv_expcbe_act_ctz](#referencia-cmxsrv_expcbe_act_ctz)
- **Exportaciones → EXPCBE → CBE00401.FRM**: [CMXsrv_cnt_950](#referencia-cmxsrv_cnt_950)

---

## CMXsrv_expcbe_cre_actz
<a name="cmxsrv_expcbe_cre_actz"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBE00401.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_lee_mdf
<a name="cmxsrv_expcbe_lee_mdf"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBE00401.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_pgo_cbe
<a name="cmxsrv_expcbe_pgo_cbe"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBE00501.FRM**: [CMXsrv_expret_grb_org](#referencia-cmxsrv_expret_grb_org)
- **Exportaciones → EXPCBE → CBE00501.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCBE → CBE00501.FRM**: [CMXsrv_exp_ipuc_gen_pln](#referencia-cmxsrv_exp_ipuc_gen_pln)
- **Exportaciones → EXPCBE → CBE00501.FRM**: [CMXsrv_expcbe_trp_cyg](#referencia-cmxsrv_expcbe_trp_cyg)
- **Exportaciones → EXPCBE → CBE00501.FRM**: [CMXsrv_expret_grb_det](#referencia-cmxsrv_expret_grb_det)
- **Exportaciones → EXPCBE → CBE00501.FRM**: [CMXsrv_expret_cre_ret](#referencia-cmxsrv_expret_cre_ret)
- **Exportaciones → EXPCBE → CBE00501.FRM**: [CMXsrv_cnt_620](#referencia-cmxsrv_cnt_620)
- **Exportaciones → EXPCBE → CBE00501.FRM**: [CMXsrv_cnt_950](#referencia-cmxsrv_cnt_950)
- **Exportaciones → EXPCBE → CBE00501.FRM**: [CMXsrv_vig_gra_vig](#referencia-cmxsrv_vig_gra_vig)
- **Exportaciones → EXPCBE → CBE00501.FRM**: [CMXsrv_cnt_gen_vig](#referencia-cmxsrv_cnt_gen_vig)
- **Exportaciones → EXPCBE → CBE00501.FRM**: [CMXsrv_mbyte_gen](#referencia-cmxsrv_mbyte_gen)
- **Exportaciones → EXPCBE → CBE00501.FRM**: [CMXsrv_expcbe_grb_evz](#referencia-cmxsrv_expcbe_grb_evz)
- **Exportaciones → EXPCBE → CBE00501.FRM**: [CMXsrv_expret_grb_dtn](#referencia-cmxsrv_expret_grb_dtn)

---

## CMXsrv_expcbe_lee_pgo
<a name="cmxsrv_expcbe_lee_pgo"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBE00501.FRM**: [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)
- **Exportaciones → EXPCBE → CBE00501.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_bus_evz
<a name="cmxsrv_expcbe_bus_evz"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPNEG → CBE00601.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCBE → CBE00601.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_rev_cbe
<a name="cmxsrv_expcbe_rev_cbe"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPNEG → CBE00601.FRM**: [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)
- **Exportaciones → EXPCBE → CBE00601.FRM**: [CMXsrv_rev_950](#referencia-cmxsrv_rev_950)
- **Exportaciones → EXPCBE → CBE00601.FRM**: [CMXsrv_cnt_601](#referencia-cmxsrv_cnt_601)
- **Exportaciones → EXPCBE → CBE00601.FRM**: [CMXsrv_expcbe_rev_trp](#referencia-cmxsrv_expcbe_rev_trp)
- **Exportaciones → EXPNEG → CBE00601.FRM**: [CMXsrv_cnt_621](#referencia-cmxsrv_cnt_621)
- **Exportaciones → EXPCBE → CBE00601.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCBE → CBE00601.FRM**: [CMXsrv_ctl_chq_aprcbl](#referencia-cmxsrv_ctl_chq_aprcbl)
- **Exportaciones → EXPNEG → CBE00601.FRM**: [CMXsrv_cnt_631](#referencia-cmxsrv_cnt_631)
- **Exportaciones → EXPNEG → CBE00601.FRM**: [CMXsrv_expcbe_grb_evz](#referencia-cmxsrv_expcbe_grb_evz)
- **Exportaciones → EXPNEG → CBE00601.FRM**: [CMXsrv_cnt_rev_vig](#referencia-cmxsrv_cnt_rev_vig)
- **Exportaciones → EXPCBE → CBE00601.FRM**: [CMXsrv_cnt_610](#referencia-cmxsrv_cnt_610)
- **Exportaciones → EXPCBE → CBE00601.FRM**: [por](#referencia-por)
- **Exportaciones → EXPNEG → CBE00601.FRM**: [CMXsrv_mbyte_gen](#referencia-cmxsrv_mbyte_gen)
- **Exportaciones → EXPCBE → CBE00601.FRM**: [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)
- **Exportaciones → EXPNEG → CBE00601.FRM**: [CMXsrv_rev_950](#referencia-cmxsrv_rev_950)
- **Exportaciones → EXPCBE → CBE00601.FRM**: [CMXsrv_cnt_621](#referencia-cmxsrv_cnt_621)
- **Exportaciones → EXPCBE → CBE00601.FRM**: [CMXsrv_expcbe_grb_evz](#referencia-cmxsrv_expcbe_grb_evz)
- **Exportaciones → EXPCBE → CBE00601.FRM**: [CMXsrv_cnt_rev_vig](#referencia-cmxsrv_cnt_rev_vig)
- **Exportaciones → EXPCBE → CBE00601.FRM**: [CMXsrv_cnt_631](#referencia-cmxsrv_cnt_631)
- **Exportaciones → EXPNEG → CBE00601.FRM**: [CMXsrv_cnt_601](#referencia-cmxsrv_cnt_601)
- **Exportaciones → EXPNEG → CBE00601.FRM**: [CMXsrv_expcbe_rev_trp](#referencia-cmxsrv_expcbe_rev_trp)
- **Exportaciones → EXPNEG → CBE00601.FRM**: [CMXsrv_ctl_chq_aprcbl](#referencia-cmxsrv_ctl_chq_aprcbl)
- **Exportaciones → EXPNEG → CBE00601.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPNEG → CBE00601.FRM**: [CMXsrv_cnt_610](#referencia-cmxsrv_cnt_610)
- **Exportaciones → EXPCBE → CBE00601.FRM**: [CMXsrv_mbyte_gen](#referencia-cmxsrv_mbyte_gen)
- **Exportaciones → EXPNEG → CBE00601.FRM**: [por](#referencia-por)

---

## CMXsrv_expcbe_lee_evz
<a name="cmxsrv_expcbe_lee_evz"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBE00602.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPNEG → CBE00602.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_del_dcz
<a name="cmxsrv_expcbe_del_dcz"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBE00603.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_bus_dcz
<a name="cmxsrv_expcbe_bus_dcz"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBE00603.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_grb_dcz
<a name="cmxsrv_expcbe_grb_dcz"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBE00604.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_lee_dcz
<a name="cmxsrv_expcbe_lee_dcz"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBE00604.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_bus_vto
<a name="cmxsrv_expcbe_bus_vto"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBE00605.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_avi_dat_cou
<a name="cmxsrv_avi_dat_cou"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBEAVIRE.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPNEG → CCEAVIRE.FRM**: [bcicomex](#referencia-bcicomex)
- **Exportaciones → EXPNEG → CCEAVIRE.FRM**: [CMXsrv_avigrl_crea_avitemp](#referencia-cmxsrv_avigrl_crea_avitemp)
- **Exportaciones → EXPCBE → CBEAVIRE.FRM**: [bcicomex](#referencia-bcicomex)
- **Exportaciones → EXPNEG → CCEAVIRE.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCBE → CBEAVIRE.FRM**: [CMXsrv_avigrl_crea_avitemp](#referencia-cmxsrv_avigrl_crea_avitemp)

---

## CMXsrv_expcbe_avs_rem1
<a name="cmxsrv_expcbe_avs_rem1"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBEAVIRE.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCBE → CBEAVIRE.FRM**: [CMXsrv_trae_glo_fec](#referencia-cmxsrv_trae_glo_fec)
- **Exportaciones → EXPCBE → CBEAVIRE.FRM**: [CMXsrv_util_fmt_txt](#referencia-cmxsrv_util_fmt_txt)
- **Exportaciones → EXPCBE → CBEAVIRE.FRM**: [CMXsrv_expcbe_val_cbe](#referencia-cmxsrv_expcbe_val_cbe)

---

## CMXsrv_expcbe_avs_rem3
<a name="cmxsrv_expcbe_avs_rem3"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBEAVIRE.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCBE → CBEAVIRE.FRM**: [CMXsrv_util_fmt_txt](#referencia-cmxsrv_util_fmt_txt)

---

## CMXsrv_expcbe_avs_rem2
<a name="cmxsrv_expcbe_avs_rem2"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBEAVIRE.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCBE → CBEAVIRE.FRM**: [CMXsrv_expcbe_for_lin](#referencia-cmxsrv_expcbe_for_lin)

---

## CMXsrv_expcbe_avs_rem4
<a name="cmxsrv_expcbe_avs_rem4"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBEAVIRE.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPNEG → CCEAVIRE.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_busc_plz
<a name="cmxsrv_busc_plz"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCCE → COR00906.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → expret → COR00906.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCBE → COR00906.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_lee_plz
<a name="cmxsrv_lee_plz"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → expret → COR00906.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → expret → COR00906.FRM**: [CMXsrv_mbyte_cmp](#referencia-cmxsrv_mbyte_cmp)
- **Exportaciones → EXPCBE → CRD00602.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCBE → CRD00602.FRM**: [CMXsrv_mbyte_cmp](#referencia-cmxsrv_mbyte_cmp)
- **Exportaciones → EXPCBE → COR00906.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCBE → COR00906.FRM**: [CMXsrv_mbyte_cmp](#referencia-cmxsrv_mbyte_cmp)
- **Exportaciones → EXPCCE → COR00906.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCCE → COR00906.FRM**: [CMXsrv_mbyte_cmp](#referencia-cmxsrv_mbyte_cmp)

---

## CMXsrv_cor_busc_pais
<a name="cmxsrv_cor_busc_pais"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCBE → COR00907.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCCE → COR00907.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → expret → COR00907.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_cor_lee_pais
<a name="cmxsrv_cor_lee_pais"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCBE → COR00907.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCCE → COR00907.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → expret → COR00907.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCBE → CRD00602.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_bus_cor
<a name="cmxsrv_expcbe_bus_cor"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCBE → GRLPAIS0.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → expret → CRD00602.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCBE → CRD00602.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_busc_bco_mtr
<a name="cmxsrv_busc_bco_mtr"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCBE → GRID_BUS.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_grl_fec_serv
<a name="cmxsrv_grl_fec_serv"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → PGOEXT → PREFER.FRM**: [SRV_MessageService](#referencia-srv_messageservice)
- **Exportaciones → EXPNEG → PREFER.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCCE → PREFER.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCCE → PREFER.FRM**: [SRV_MessageService](#referencia-srv_messageservice)
- **Exportaciones → expdex → PREFER.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → expdex → PREFER.FRM**: [SRV_MessageService](#referencia-srv_messageservice)
- **Exportaciones → EXPNEG → PREFER.FRM**: [SRV_MessageService](#referencia-srv_messageservice)
- **Importaciones → PAGCBR → PREFER.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → PAGCBR → PREFER.FRM**: [SRV_MessageService](#referencia-srv_messageservice)
- **Financiamiento → ADMIN → ADM00204.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → ADMIN → ADM00204.FRM**: [SRV_MessageService](#referencia-srv_messageservice)
- **Importaciones → COBERIMP → PREFER.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → MOD_ADI → PREFER.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → COBERIMP → PREFER.FRM**: [SRV_MessageService](#referencia-srv_messageservice)
- **Importaciones → MOD_ADI → PREFER.FRM**: [SRV_MessageService](#referencia-srv_messageservice)
- **Importaciones → COBRANZA → CBR00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → CRDEXT → PREFER.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → CRDEXT → PREFER.FRM**: [SRV_MessageService](#referencia-srv_messageservice)
- **Importaciones → COBRANZA → CBR00101.FRM**: [SRV_MessageService](#referencia-srv_messageservice)
- **Importaciones → IMPORT → CRD00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → MOD_CRD → PREFER.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → MOD_CRD → PREFER.FRM**: [SRV_MessageService](#referencia-srv_messageservice)
- **Exportaciones → expret → PREFER.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → expret → PREFER.FRM**: [SRV_MessageService](#referencia-srv_messageservice)
- **Importaciones → IMPORT → CRD00101.FRM**: [SRV_MessageService](#referencia-srv_messageservice)
- **Importaciones → INFORME → PREFER.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → INFORME → PREFER.FRM**: [SRV_MessageService](#referencia-srv_messageservice)
- **Exportaciones → EXPCBE → PREFER.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCBE → PREFER.FRM**: [SRV_MessageService](#referencia-srv_messageservice)
- **Financiamiento → COL_NEG → PREFER.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → NNEGO → PREFER.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → NNEGO → PREFER.FRM**: [SRV_MessageService](#referencia-srv_messageservice)
- **Financiamiento → COL_NEG → PREFER.FRM**: [SRV_MessageService](#referencia-srv_messageservice)
- **Financiamiento → PGOEXT → PREFER.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_lee_cce
<a name="cmxsrv_expcce_lee_cce"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCCE → CCE00301.FRM**: [por](#referencia-por)
- **Exportaciones → EXPCCE → CCE00101.FRM**: [por](#referencia-por)
- **Exportaciones → EXPCCE → CCE00301.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCCE → CCE00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_trd_cce
<a name="cmxsrv_expcce_trd_cce"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCCE → CCE00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_anl_cce
<a name="cmxsrv_expcce_anl_cce"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCCE → CCE00101.FRM**: [CMXsrv_cmx_lee_trs](#referencia-cmxsrv_cmx_lee_trs)
- **Exportaciones → EXPCCE → CCE00101.FRM**: [CMXsrv_expcce_ictb_anu](#referencia-cmxsrv_expcce_ictb_anu)
- **Exportaciones → EXPCCE → CCE00101.FRM**: [CMXsrv_expcce_lee_fpro](#referencia-cmxsrv_expcce_lee_fpro)
- **Exportaciones → EXPCCE → CCE00101.FRM**: [CMXsrv_cnt_740](#referencia-cmxsrv_cnt_740)
- **Exportaciones → EXPCCE → CCE00101.FRM**: [CMXsrv_expcce_grb_evc](#referencia-cmxsrv_expcce_grb_evc)
- **Exportaciones → EXPCCE → CCE00101.FRM**: [CMXsrv_cnt_950](#referencia-cmxsrv_cnt_950)
- **Exportaciones → EXPCCE → CCE00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_ctb_ing
<a name="cmxsrv_expcce_ctb_ing"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCCE → CCE00101.FRM**: [CMXsrv_expcce_val_cce](#referencia-cmxsrv_expcce_val_cce)
- **Exportaciones → EXPCCE → CCE00101.FRM**: [CMXsrv_cnt_700](#referencia-cmxsrv_cnt_700)
- **Exportaciones → EXPCCE → CCE00101.FRM**: [CMXsrv_mbyte_gen](#referencia-cmxsrv_mbyte_gen)
- **Exportaciones → EXPCCE → CCE00101.FRM**: [CMXsrv_expcce_grb_evc](#referencia-cmxsrv_expcce_grb_evc)
- **Exportaciones → EXPCCE → CCE00101.FRM**: [CMXsrv_cnt_950](#referencia-cmxsrv_cnt_950)
- **Exportaciones → EXPCCE → CCE00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_del_cce
<a name="cmxsrv_expcce_del_cce"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCCE → CCE00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_val_cce
<a name="cmxsrv_expcce_val_cce"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCCE → CCE00101.FRM**: [CMXsrv_cmx_get_codes](#referencia-cmxsrv_cmx_get_codes)
- **Exportaciones → EXPCCE → CCE00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_swf_sel
<a name="cmxsrv_expcce_swf_sel"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCCE → GRL00101.FRM**: [CMXsrv_expcce_swf_730](#referencia-cmxsrv_expcce_swf_730)
- **Exportaciones → EXPNEG → CCE00601.FRM**: [CMXsrv_expcce_swf_730](#referencia-cmxsrv_expcce_swf_730)
- **Exportaciones → EXPNEG → GRL00101.FRM**: [CMXsrv_expcce_swf_742](#referencia-cmxsrv_expcce_swf_742)
- **Exportaciones → EXPNEG → GRL00101.FRM**: [CMXsrv_expcce_swf_730](#referencia-cmxsrv_expcce_swf_730)
- **Exportaciones → EXPCCE → CCE00101.FRM**: [CMXsrv_expcce_swf_730](#referencia-cmxsrv_expcce_swf_730)
- **Exportaciones → EXPCCE → CCE00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCCE → GRL00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPNEG → CCE00601.FRM**: [CMXsrv_expcce_swf_742](#referencia-cmxsrv_expcce_swf_742)
- **Exportaciones → EXPCCE → CCE00101.FRM**: [CMXsrv_expcce_swf_742](#referencia-cmxsrv_expcce_swf_742)
- **Exportaciones → EXPNEG → GRL00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPNEG → CCE00601.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCCE → GRL00101.FRM**: [CMXsrv_expcce_swf_742](#referencia-cmxsrv_expcce_swf_742)

---

## CMXsrv_expcce_grb_bco
<a name="cmxsrv_expcce_grb_bco"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCCE → CCE00201.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCCE → CCE00203.FRM**: [CMXsrv_expcce_lee_fpro](#referencia-cmxsrv_expcce_lee_fpro)
- **Exportaciones → EXPCCE → CCE00203.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCCE → CCE00201.FRM**: [CMXsrv_expcce_lee_fpro](#referencia-cmxsrv_expcce_lee_fpro)

---

## CMXsrv_expcce_lee_cor
<a name="cmxsrv_expcce_lee_cor"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCCE → CCE00401.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCCE → CRD00602.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPNEG → CCE01201.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCCE → CCE00201.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPNEG → CCE00901.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPNEG → CRD00602.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCCE → CCE00701.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_lee_bco
<a name="cmxsrv_expcce_lee_bco"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCCE → CCE00201.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_grb_ctp
<a name="cmxsrv_expcce_grb_ctp"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCCE → CCE00203.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCCE → CCE00202.FRM**: [CMXsrv_expcce_lee_fpro](#referencia-cmxsrv_expcce_lee_fpro)
- **Exportaciones → EXPCCE → CCE00202.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCCE → CCE00203.FRM**: [CMXsrv_expcce_lee_fpro](#referencia-cmxsrv_expcce_lee_fpro)

---

## CMXsrv_expcce_lee_cln
<a name="cmxsrv_expcce_lee_cln"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCCE → CCE00401.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPNEG → CCE01201.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCCE → CCE00202.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCCE → CCE00301.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPNEG → CCE00901.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_lee_ctp
<a name="cmxsrv_expcce_lee_ctp"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCCE → CCE00202.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_cre_cce
<a name="cmxsrv_expcce_cre_cce"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCCE → CCE00203.FRM**: [CMXsrv_cmx_busc_suc_usu](#referencia-cmxsrv_cmx_busc_suc_usu)
- **Exportaciones → EXPCCE → CCE00203.FRM**: [CMXsrv_expcce_lee_fpro](#referencia-cmxsrv_expcce_lee_fpro)
- **Exportaciones → EXPCCE → CCE00203.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCCE → CCE00203.FRM**: [CMXsrv_util_num_ope](#referencia-cmxsrv_util_num_ope)

---

## CMXsrv_expcce_gen_dcc
<a name="cmxsrv_expcce_gen_dcc"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCCE → CCE00203.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_grb_cnd
<a name="cmxsrv_expcce_grb_cnd"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCCE → CCE00203.FRM**: [CMXsrv_expcce_lee_fpro](#referencia-cmxsrv_expcce_lee_fpro)
- **Exportaciones → EXPCCE → CCE00203.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_util_det_habil
<a name="cmxsrv_util_det_habil"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → IMPORT → CRD00202.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCCE → CCE00203.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → MOD_ADI → CRD00202.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_lee_cnd
<a name="cmxsrv_expcce_lee_cnd"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCCE → CCE00203.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_trd_cnd
<a name="cmxsrv_expcce_trd_cnd"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCCE → CCE00203.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_del_dcc
<a name="cmxsrv_expcce_del_dcc"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCCE → CCE00204.FRM**: [CMXsrv_expcce_lee_fpro](#referencia-cmxsrv_expcce_lee_fpro)
- **Exportaciones → EXPCCE → CCE00204.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_bus_dcc
<a name="cmxsrv_expcce_bus_dcc"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCCE → CCE00204.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCCE → CCE00204.FRM**: [CMXsrv_expcce_gen_adcc](#referencia-cmxsrv_expcce_gen_adcc)

---

## CMXsrv_expcce_grb_dcc
<a name="cmxsrv_expcce_grb_dcc"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCCE → CCE00205.FRM**: [CMXsrv_expcce_lee_fpro](#referencia-cmxsrv_expcce_lee_fpro)
- **Exportaciones → EXPCCE → CCE00205.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_lee_dcc
<a name="cmxsrv_expcce_lee_dcc"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCCE → CCE00205.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_bus_cce
<a name="cmxsrv_expcce_bus_cce"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCCE → CCE00301.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_mdf_cce
<a name="cmxsrv_expcce_mdf_cce"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCCE → CCE00401.FRM**: [CMXsrv_expcce_grb_evc](#referencia-cmxsrv_expcce_grb_evc)
- **Exportaciones → EXPCCE → CCE00401.FRM**: [CMXsrv_cnt_950](#referencia-cmxsrv_cnt_950)
- **Exportaciones → EXPCCE → CCE00401.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCCE → CCE00401.FRM**: [CMXsrv_expcce_lee_fpro](#referencia-cmxsrv_expcce_lee_fpro)
- **Exportaciones → EXPCCE → CCE00401.FRM**: [CMXsrv_cnt_720](#referencia-cmxsrv_cnt_720)
- **Exportaciones → EXPCCE → CCE00401.FRM**: [CMXsrv_expcce_ctb_mdfcce](#referencia-cmxsrv_expcce_ctb_mdfcce)
- **Exportaciones → EXPCCE → CCE00401.FRM**: [CMXsrv_expcce_get_tip_ope](#referencia-cmxsrv_expcce_get_tip_ope)
- **Exportaciones → EXPCCE → CCE00401.FRM**: [CMXsrv_expcce_can_mdf](#referencia-cmxsrv_expcce_can_mdf)
- **Exportaciones → EXPCCE → CCE00401.FRM**: [CMXsrv_cmx_get_codes](#referencia-cmxsrv_cmx_get_codes)

---

## CMXsrv_expcce_can_mdf
<a name="cmxsrv_expcce_can_mdf"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCCE → CCE00401.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_lee_mdf
<a name="cmxsrv_expcce_lee_mdf"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCCE → CCE00401.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_cnf_cce
<a name="cmxsrv_expcce_cnf_cce"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCCE → CCE00501.FRM**: [CMXsrv_expcce_grb_evc](#referencia-cmxsrv_expcce_grb_evc)
- **Exportaciones → EXPCCE → CCE00501.FRM**: [CMXsrv_cnt_950](#referencia-cmxsrv_cnt_950)
- **Exportaciones → EXPCCE → CCE00501.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCCE → CCE00501.FRM**: [CMXsrv_cnt_710](#referencia-cmxsrv_cnt_710)
- **Exportaciones → EXPCCE → CCE00501.FRM**: [CMXsrv_expcce_lee_fpro](#referencia-cmxsrv_expcce_lee_fpro)
- **Exportaciones → EXPCCE → CCE00501.FRM**: [CMXsrv_expcce_ictb_cexp](#referencia-cmxsrv_expcce_ictb_cexp)

---

## CMXsrv_expcce_grb_afin
<a name="cmxsrv_expcce_grb_afin"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPNEG → CCE00901.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPNEG → CCE01201.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCCE → CCE00501.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_lee_cnf
<a name="cmxsrv_expcce_lee_cnf"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCCE → CCE00501.FRM**: [CMXsrv_expcce_lee_fpro](#referencia-cmxsrv_expcce_lee_fpro)
- **Exportaciones → EXPCCE → CCE00501.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_lee_afin
<a name="cmxsrv_expcce_lee_afin"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPNEG → CCE00901.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPNEG → CCE01201.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCCE → CCE00501.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_trp_cce
<a name="cmxsrv_expcce_trp_cce"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCCE → CCE00701.FRM**: [CMXsrv_cnt_730](#referencia-cmxsrv_cnt_730)
- **Exportaciones → EXPCCE → CCE00701.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCCE → CCE00701.FRM**: [CMXsrv_cnt_950](#referencia-cmxsrv_cnt_950)
- **Exportaciones → EXPCCE → CCE00701.FRM**: [CMXsrv_expcce_grb_evc](#referencia-cmxsrv_expcce_grb_evc)

---

## CMXsrv_expcce_lee_trp
<a name="cmxsrv_expcce_lee_trp"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCCE → CCE00701.FRM**: [CMXsrv_expcce_lee_fpro](#referencia-cmxsrv_expcce_lee_fpro)
- **Exportaciones → EXPCCE → CCE00701.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_bus_evc
<a name="cmxsrv_expcce_bus_evc"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPNEG → CCE00801.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCCE → CCE00801.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_rev_cce
<a name="cmxsrv_expcce_rev_cce"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCCE → CCE00801.FRM**: [CMXsrv_expcce_rctb_oto_exp](#referencia-cmxsrv_expcce_rctb_oto_exp)
- **Exportaciones → EXPCCE → CCE00801.FRM**: [CMXsrv_expcce_get_tip_ope](#referencia-cmxsrv_expcce_get_tip_ope)
- **Exportaciones → EXPCCE → CCE00801.FRM**: [CMXsrv_expcce_eli_obl](#referencia-cmxsrv_expcce_eli_obl)
- **Exportaciones → EXPNEG → CCE00801.FRM**: [CMXsrv_expcce_rctb_anu](#referencia-cmxsrv_expcce_rctb_anu)
- **Exportaciones → EXPNEG → CCE00801.FRM**: [CMXsrv_expcce_rev_mdf](#referencia-cmxsrv_expcce_rev_mdf)
- **Exportaciones → EXPNEG → CCE00801.FRM**: [CMXsrv_expcce_ctb_mdfcce](#referencia-cmxsrv_expcce_ctb_mdfcce)
- **Exportaciones → EXPNEG → CCE00801.FRM**: [CMXsrv_expneg_rev_trp](#referencia-cmxsrv_expneg_rev_trp)
- **Exportaciones → EXPCCE → CCE00801.FRM**: [CMXsrv_cnt_781](#referencia-cmxsrv_cnt_781)
- **Exportaciones → EXPCCE → CCE00801.FRM**: [CMXsrv_cnt_rev_vig](#referencia-cmxsrv_cnt_rev_vig)
- **Exportaciones → EXPCCE → CCE00801.FRM**: [CMXsrv_expcce_chk_dsn](#referencia-cmxsrv_expcce_chk_dsn)
- **Exportaciones → EXPCCE → CCE00801.FRM**: [CMXsrv_expcce_grb_evc](#referencia-cmxsrv_expcce_grb_evc)
- **Exportaciones → EXPNEG → CCE00801.FRM**: [CMXsrv_cnt_999999](#referencia-cmxsrv_cnt_999999)
- **Exportaciones → EXPCCE → CCE00801.FRM**: [CMXsrv_cnt_720](#referencia-cmxsrv_cnt_720)
- **Exportaciones → EXPCCE → CCE00801.FRM**: [CMXsrv_cnt_771](#referencia-cmxsrv_cnt_771)
- **Exportaciones → EXPCCE → CCE00801.FRM**: [CMXsrv_mbyte_gen](#referencia-cmxsrv_mbyte_gen)
- **Exportaciones → EXPCCE → CCE00801.FRM**: [CMXsrv_cnt_711](#referencia-cmxsrv_cnt_711)
- **Exportaciones → EXPCCE → CCE00801.FRM**: [CMXsrv_cnt_701](#referencia-cmxsrv_cnt_701)
- **Exportaciones → EXPNEG → CCE00801.FRM**: [CMXsrv_expcce_get_tip_ope](#referencia-cmxsrv_expcce_get_tip_ope)
- **Exportaciones → EXPCCE → CCE00801.FRM**: [CMXsrv_expcce_rctb_pag_exp](#referencia-cmxsrv_expcce_rctb_pag_exp)
- **Exportaciones → EXPNEG → CCE00801.FRM**: [CMXsrv_expcce_rctb_oto_exp](#referencia-cmxsrv_expcce_rctb_oto_exp)
- **Exportaciones → EXPNEG → CCE00801.FRM**: [CMXsrv_expcce_eli_obl](#referencia-cmxsrv_expcce_eli_obl)
- **Exportaciones → EXPCCE → CCE00801.FRM**: [CMXsrv_cnt_1771](#referencia-cmxsrv_cnt_1771)
- **Exportaciones → EXPNEG → CCE00801.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPNEG → CCE00801.FRM**: [CMXsrv_cnt_781](#referencia-cmxsrv_cnt_781)
- **Exportaciones → EXPCCE → CCE00801.FRM**: [CMXsrv_expcce_ranu_neg](#referencia-cmxsrv_expcce_ranu_neg)
- **Exportaciones → EXPCCE → CCE00801.FRM**: [CMXsrv_cnt_731](#referencia-cmxsrv_cnt_731)
- **Exportaciones → EXPNEG → CCE00801.FRM**: [CMXsrv_expcce_grb_evc](#referencia-cmxsrv_expcce_grb_evc)
- **Exportaciones → EXPNEG → CCE00801.FRM**: [CMXsrv_cnt_rev_vig](#referencia-cmxsrv_cnt_rev_vig)
- **Exportaciones → EXPCCE → CCE00801.FRM**: [CMXsrv_rev_950](#referencia-cmxsrv_rev_950)
- **Exportaciones → EXPCCE → CCE00801.FRM**: [CMXsrv_cmx_lee_trs](#referencia-cmxsrv_cmx_lee_trs)
- **Exportaciones → EXPNEG → CCE00801.FRM**: [CMXsrv_expcce_chk_dsn](#referencia-cmxsrv_expcce_chk_dsn)
- **Exportaciones → EXPCCE → CCE00801.FRM**: [CMXsrv_expcce_lee_fpro](#referencia-cmxsrv_expcce_lee_fpro)
- **Exportaciones → EXPCCE → CCE00801.FRM**: [CMXsrv_expcce_rctb_oto](#referencia-cmxsrv_expcce_rctb_oto)
- **Exportaciones → EXPNEG → CCE00801.FRM**: [CMXsrv_cnt_720](#referencia-cmxsrv_cnt_720)
- **Exportaciones → EXPNEG → CCE00801.FRM**: [CMXsrv_cnt_771](#referencia-cmxsrv_cnt_771)
- **Exportaciones → EXPCCE → CCE00801.FRM**: [CMXsrv_cnt_741](#referencia-cmxsrv_cnt_741)
- **Exportaciones → EXPCCE → CCE00801.FRM**: [CMXsrv_cnt_761](#referencia-cmxsrv_cnt_761)
- **Exportaciones → EXPCCE → CCE00801.FRM**: [CMXsrv_cnt_751](#referencia-cmxsrv_cnt_751)
- **Exportaciones → EXPNEG → CCE00801.FRM**: [CMXsrv_mbyte_gen](#referencia-cmxsrv_mbyte_gen)
- **Exportaciones → EXPCCE → CCE00801.FRM**: [CMXsrv_expcce_ctb_alz](#referencia-cmxsrv_expcce_ctb_alz)
- **Exportaciones → EXPNEG → CCE00801.FRM**: [CMXsrv_cnt_711](#referencia-cmxsrv_cnt_711)
- **Exportaciones → EXPNEG → CCE00801.FRM**: [CMXsrv_cnt_1771](#referencia-cmxsrv_cnt_1771)
- **Exportaciones → EXPCCE → CCE00801.FRM**: [CMXsrv_ctl_chq_aprcbl](#referencia-cmxsrv_ctl_chq_aprcbl)
- **Exportaciones → EXPCCE → CCE00801.FRM**: [CMXsrv_expcce_eli_col](#referencia-cmxsrv_expcce_eli_col)
- **Exportaciones → EXPNEG → CCE00801.FRM**: [CMXsrv_cnt_701](#referencia-cmxsrv_cnt_701)
- **Exportaciones → EXPCCE → CCE00801.FRM**: [CMXsrv_expcce_gen_dsn](#referencia-cmxsrv_expcce_gen_dsn)
- **Exportaciones → EXPCCE → CCE00801.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPNEG → CCE00801.FRM**: [CMXsrv_expcce_rctb_pag_exp](#referencia-cmxsrv_expcce_rctb_pag_exp)
- **Exportaciones → EXPCCE → CCE00801.FRM**: [CMXsrv_expcce_rctb_anu](#referencia-cmxsrv_expcce_rctb_anu)
- **Exportaciones → EXPCCE → CCE00801.FRM**: [CMXsrv_expcce_ctb_mdfcce](#referencia-cmxsrv_expcce_ctb_mdfcce)
- **Exportaciones → EXPCCE → CCE00801.FRM**: [CMXsrv_expcce_rev_mdf](#referencia-cmxsrv_expcce_rev_mdf)
- **Exportaciones → EXPNEG → CCE00801.FRM**: [CMXsrv_expcce_ranu_neg](#referencia-cmxsrv_expcce_ranu_neg)
- **Exportaciones → EXPNEG → CCE00801.FRM**: [CMXsrv_cnt_731](#referencia-cmxsrv_cnt_731)
- **Exportaciones → EXPCCE → CCE00801.FRM**: [CMXsrv_expneg_rev_trp](#referencia-cmxsrv_expneg_rev_trp)
- **Exportaciones → EXPNEG → CCE00801.FRM**: [CMXsrv_rev_950](#referencia-cmxsrv_rev_950)
- **Exportaciones → EXPNEG → CCE00801.FRM**: [CMXsrv_cmx_lee_trs](#referencia-cmxsrv_cmx_lee_trs)
- **Exportaciones → EXPNEG → CCE00801.FRM**: [CMXsrv_expcce_lee_fpro](#referencia-cmxsrv_expcce_lee_fpro)
- **Exportaciones → EXPNEG → CCE00801.FRM**: [CMXsrv_expcce_rctb_oto](#referencia-cmxsrv_expcce_rctb_oto)
- **Exportaciones → EXPNEG → CCE00801.FRM**: [CMXsrv_cnt_741](#referencia-cmxsrv_cnt_741)
- **Exportaciones → EXPCCE → CCE00801.FRM**: [CMXsrv_cnt_999999](#referencia-cmxsrv_cnt_999999)
- **Exportaciones → EXPNEG → CCE00801.FRM**: [CMXsrv_cnt_761](#referencia-cmxsrv_cnt_761)
- **Exportaciones → EXPNEG → CCE00801.FRM**: [CMXsrv_cnt_751](#referencia-cmxsrv_cnt_751)
- **Exportaciones → EXPNEG → CCE00801.FRM**: [CMXsrv_expcce_ctb_alz](#referencia-cmxsrv_expcce_ctb_alz)
- **Exportaciones → EXPNEG → CCE00801.FRM**: [CMXsrv_ctl_chq_aprcbl](#referencia-cmxsrv_ctl_chq_aprcbl)
- **Exportaciones → EXPNEG → CCE00801.FRM**: [CMXsrv_expcce_eli_col](#referencia-cmxsrv_expcce_eli_col)
- **Exportaciones → EXPNEG → CCE00801.FRM**: [CMXsrv_expcce_gen_dsn](#referencia-cmxsrv_expcce_gen_dsn)

---

## CMXsrv_expcce_lee_evc
<a name="cmxsrv_expcce_lee_evc"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCCE → CCE00802.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPNEG → CCE00802.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_avs_rem1
<a name="cmxsrv_expcce_avs_rem1"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPNEG → CCEAVIRE.FRM**: [CMXsrv_trae_glo_fec](#referencia-cmxsrv_trae_glo_fec)
- **Exportaciones → EXPCCE → CCEAVIRE.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPNEG → CCEAVIRE.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPCCE → CCEAVIRE.FRM**: [CMXsrv_trae_glo_fec](#referencia-cmxsrv_trae_glo_fec)

---

## CMXsrv_expcce_bus_cor
<a name="cmxsrv_expcce_bus_cor"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPCCE → CRD00602.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPNEG → CRD00602.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_dex_lee_dex
<a name="cmxsrv_dex_lee_dex"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → expdex → RESPALD2.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → expdex → DEX00102.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → expdex → DEX00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → expdex → RESPALDO.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_dex_eli_dex
<a name="cmxsrv_dex_eli_dex"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → expdex → DEX00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → expdex → RESPALDO.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_dex_act_dex
<a name="cmxsrv_dex_act_dex"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → expdex → RESPALD2.FRM**: [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)
- **Exportaciones → expdex → RESPALD2.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → expdex → DEX00102.FRM**: [CMXsrv_exppln_get_dig](#referencia-cmxsrv_exppln_get_dig)
- **Exportaciones → expdex → RESPALD2.FRM**: [CMXsrv_exppln_get_dig](#referencia-cmxsrv_exppln_get_dig)
- **Exportaciones → expdex → DEX00102.FRM**: [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)
- **Exportaciones → expdex → DEX00102.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expdex_cal_fec
<a name="cmxsrv_expdex_cal_fec"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → expdex → DEX00102.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_dex_lee_cli
<a name="cmxsrv_dex_lee_cli"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → expdex → RESPALD2.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → expdex → DEX00102.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → expdex → DEX00103.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_dex_bus_dex
<a name="cmxsrv_dex_bus_dex"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → expdex → DEX00103.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_lee_bas
<a name="cmxsrv_expcce_lee_bas"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPNEG → CCE00601.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_lee_neg
<a name="cmxsrv_expcce_lee_neg"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPNEG → CCE00601.FRM**: [CMXsrv_cmx_busc_suc_usu](#referencia-cmxsrv_cmx_busc_suc_usu)
- **Exportaciones → EXPNEG → CCE00601.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_alz_dis
<a name="cmxsrv_expcce_alz_dis"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPNEG → CCE00601.FRM**: [CMXsrv_expcce_lee_fpro](#referencia-cmxsrv_expcce_lee_fpro)
- **Exportaciones → EXPNEG → CCE00601.FRM**: [CMXsrv_expcce_get_tip_ope](#referencia-cmxsrv_expcce_get_tip_ope)
- **Exportaciones → EXPNEG → CCE00601.FRM**: [CMXsrv_cnt_760](#referencia-cmxsrv_cnt_760)
- **Exportaciones → EXPNEG → CCE00601.FRM**: [CMXsrv_expcce_ctb_alz](#referencia-cmxsrv_expcce_ctb_alz)
- **Exportaciones → EXPNEG → CCE00601.FRM**: [CMXsrv_expcce_grb_evc](#referencia-cmxsrv_expcce_grb_evc)
- **Exportaciones → EXPNEG → CCE00601.FRM**: [CMXsrv_cnt_950](#referencia-cmxsrv_cnt_950)
- **Exportaciones → EXPNEG → CCE00601.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_anl_neg
<a name="cmxsrv_expcce_anl_neg"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPNEG → CCE00601.FRM**: [CMXsrv_expcce_lee_fpro](#referencia-cmxsrv_expcce_lee_fpro)
- **Exportaciones → EXPNEG → CCE00601.FRM**: [CMXsrv_cnt_780](#referencia-cmxsrv_cnt_780)
- **Exportaciones → EXPNEG → CCE00601.FRM**: [CMXsrv_expcce_grb_evc](#referencia-cmxsrv_expcce_grb_evc)
- **Exportaciones → EXPNEG → CCE00601.FRM**: [CMXsrv_expcce_ictb_anu](#referencia-cmxsrv_expcce_ictb_anu)
- **Exportaciones → EXPNEG → CCE00601.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPNEG → CCE00601.FRM**: [CMXsrv_cnt_950](#referencia-cmxsrv_cnt_950)
- **Exportaciones → EXPNEG → CCE00601.FRM**: [CMXsrv_cmx_lee_trs](#referencia-cmxsrv_cmx_lee_trs)

---

## CMXsrv_expcce_ctb_neg
<a name="cmxsrv_expcce_ctb_neg"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPNEG → CCE00601.FRM**: [CMXsrv_expcce_lee_fpro](#referencia-cmxsrv_expcce_lee_fpro)
- **Exportaciones → EXPNEG → CCE00601.FRM**: [CMXsrv_expcce_anu_cexp](#referencia-cmxsrv_expcce_anu_cexp)
- **Exportaciones → EXPNEG → CCE00601.FRM**: [CMXsrv_cnt_750](#referencia-cmxsrv_cnt_750)
- **Exportaciones → EXPNEG → CCE00601.FRM**: [CMXsrv_mbyte_gen](#referencia-cmxsrv_mbyte_gen)
- **Exportaciones → EXPNEG → CCE00601.FRM**: [CMXsrv_expcce_ineg_cexp](#referencia-cmxsrv_expcce_ineg_cexp)
- **Exportaciones → EXPNEG → CCE00601.FRM**: [CMXsrv_expcce_grb_evc](#referencia-cmxsrv_expcce_grb_evc)
- **Exportaciones → EXPNEG → CCE00601.FRM**: [CMXsrv_cnt_950](#referencia-cmxsrv_cnt_950)
- **Exportaciones → EXPNEG → CCE00601.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPNEG → CCE00601.FRM**: [CMXsrv_expcce_val_neg](#referencia-cmxsrv_expcce_val_neg)

---

## CMXsrv_expcce_del_neg
<a name="cmxsrv_expcce_del_neg"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPNEG → CCE00601.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_val_neg
<a name="cmxsrv_expcce_val_neg"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPNEG → CCE00601.FRM**: [CMXsrv_util_fecha](#referencia-cmxsrv_util_fecha)
- **Exportaciones → EXPNEG → CCE00601.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_grb_neg
<a name="cmxsrv_expcce_grb_neg"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPNEG → CCE00901.FRM**: [CMXsrv_cmx_busc_suc_usu](#referencia-cmxsrv_cmx_busc_suc_usu)
- **Exportaciones → EXPNEG → CCE00901.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPNEG → CCE00901.FRM**: [CMXsrv_expcce_lee_fpro](#referencia-cmxsrv_expcce_lee_fpro)

---

## CMXsrv_expcce_gen_dcn
<a name="cmxsrv_expcce_gen_dcn"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPNEG → CCE00901.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_avs_rem5
<a name="cmxsrv_expcce_avs_rem5"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPNEG → CCE00901.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPNEG → CCE00901.FRM**: [CMX_srv_pone_punto](#referencia-cmx_srv_pone_punto)
- **Exportaciones → EXPNEG → CCE00901.FRM**: [CMXsrv_expcce_get_ing_esp](#referencia-cmxsrv_expcce_get_ing_esp)
- **Exportaciones → EXPNEG → CCE00901.FRM**: [CMXsrv_util_fmt_txt](#referencia-cmxsrv_util_fmt_txt)

---

## CMXsrv_expcce_lee_nge
<a name="cmxsrv_expcce_lee_nge"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPNEG → CCEAVIRE.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPNEG → CCE00901.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_trd_nge
<a name="cmxsrv_expcce_trd_nge"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPNEG → CCE00901.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_ini_neg
<a name="cmxsrv_expcce_ini_neg"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPNEG → CCE00901.FRM**: [CMXsrv_expcce_lee_fpro](#referencia-cmxsrv_expcce_lee_fpro)
- **Exportaciones → EXPNEG → CCE00901.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_del_dcn
<a name="cmxsrv_expcce_del_dcn"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPNEG → CCE00902.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_bus_dcn
<a name="cmxsrv_expcce_bus_dcn"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPNEG → CCE00902.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_grb_dcn
<a name="cmxsrv_expcce_grb_dcn"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPNEG → CCE00903.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_lee_dcn
<a name="cmxsrv_expcce_lee_dcn"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPNEG → CCE00903.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_del_ltr
<a name="cmxsrv_expcce_del_ltr"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPNEG → CCE00904.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_bus_ltr
<a name="cmxsrv_expcce_bus_ltr"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPNEG → CCE00904.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_grb_ltr
<a name="cmxsrv_expcce_grb_ltr"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPNEG → CCE00905.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_lee_ltr
<a name="cmxsrv_expcce_lee_ltr"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPNEG → CCE00905.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_del_dsn
<a name="cmxsrv_expcce_del_dsn"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPNEG → CCE00906.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_gen_dsn
<a name="cmxsrv_expcce_gen_dsn"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPNEG → CCE00906.FRM**: [CMXsrv_expcce_grb_dsn](#referencia-cmxsrv_expcce_grb_dsn)
- **Exportaciones → EXPNEG → CCE00906.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_bus_dsn
<a name="cmxsrv_expcce_bus_dsn"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPNEG → CCE00906.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_chk_dsn
<a name="cmxsrv_expcce_chk_dsn"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPNEG → CCE00906.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_grb_dsn
<a name="cmxsrv_expcce_grb_dsn"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPNEG → CCE00907.FRM**: [CMXsrv_expcce_chk_dsn](#referencia-cmxsrv_expcce_chk_dsn)
- **Exportaciones → EXPNEG → CCE00907.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_lee_dsn
<a name="cmxsrv_expcce_lee_dsn"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPNEG → CCE00907.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_bus_neg
<a name="cmxsrv_expcce_bus_neg"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPNEG → CCE01001.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_pgo_neg
<a name="cmxsrv_expcce_pgo_neg"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPNEG → CCE01201.FRM**: [CMXsrv_expret_grb_dtn](#referencia-cmxsrv_expret_grb_dtn)
- **Exportaciones → EXPNEG → CCE01201.FRM**: [CMXsrv_cnt_999999](#referencia-cmxsrv_cnt_999999)
- **Exportaciones → EXPNEG → CCE01201.FRM**: [CMXsrv_expret_cre_ret](#referencia-cmxsrv_expret_cre_ret)
- **Exportaciones → EXPNEG → CCE01201.FRM**: [CMXsrv_expcce_pag_exp](#referencia-cmxsrv_expcce_pag_exp)
- **Exportaciones → EXPNEG → CCE01201.FRM**: [CMXsrv_exp_ipuc_gen_pln](#referencia-cmxsrv_exp_ipuc_gen_pln)
- **Exportaciones → EXPNEG → CCE01201.FRM**: [CMXsrv_expcce_grb_evc](#referencia-cmxsrv_expcce_grb_evc)
- **Exportaciones → EXPNEG → CCE01201.FRM**: [CMXsrv_cnt_950](#referencia-cmxsrv_cnt_950)
- **Exportaciones → EXPNEG → CCE01201.FRM**: [CMXsrv_cnt_770](#referencia-cmxsrv_cnt_770)
- **Exportaciones → EXPNEG → CCE01201.FRM**: [CMXsrv_mbyte_gen](#referencia-cmxsrv_mbyte_gen)
- **Exportaciones → EXPNEG → CCE01201.FRM**: [CMXsrv_expcce_anu_cexp](#referencia-cmxsrv_expcce_anu_cexp)
- **Exportaciones → EXPNEG → CCE01201.FRM**: [CMXsrv_expret_grb_org](#referencia-cmxsrv_expret_grb_org)
- **Exportaciones → EXPNEG → CCE01201.FRM**: [CMXsrv_expcce_lee_fpro](#referencia-cmxsrv_expcce_lee_fpro)
- **Exportaciones → EXPNEG → CCE01201.FRM**: [CMXsrv_expneg_trp_cyg](#referencia-cmxsrv_expneg_trp_cyg)
- **Exportaciones → EXPNEG → CCE01201.FRM**: [CMXsrv_vig_gra_vig](#referencia-cmxsrv_vig_gra_vig)
- **Exportaciones → EXPNEG → CCE01201.FRM**: [CMXsrv_cnt_1770](#referencia-cmxsrv_cnt_1770)
- **Exportaciones → EXPNEG → CCE01201.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPNEG → CCE01201.FRM**: [CMXsrv_expret_grb_det](#referencia-cmxsrv_expret_grb_det)
- **Exportaciones → EXPNEG → CCE01201.FRM**: [CMXsrv_cnt_gen_vig](#referencia-cmxsrv_cnt_gen_vig)
- **Exportaciones → EXPNEG → CCE01201.FRM**: [CMXsrv_cmx_get_codes](#referencia-cmxsrv_cmx_get_codes)

---

## CMXsrv_expcce_lee_pgo
<a name="cmxsrv_expcce_lee_pgo"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPNEG → CCE01201.FRM**: [CMXsrv_expcce_lee_fpro](#referencia-cmxsrv_expcce_lee_fpro)
- **Exportaciones → EXPNEG → CCE01201.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_avs_rem3
<a name="cmxsrv_expcce_avs_rem3"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPNEG → CCEAVIRE.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPNEG → CCEAVIRE.FRM**: [CMXsrv_util_fmt_txt](#referencia-cmxsrv_util_fmt_txt)

---

## CMXsrv_expcce_avs_rem2
<a name="cmxsrv_expcce_avs_rem2"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPNEG → CCEAVIRE.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_avs_rem4
<a name="cmxsrv_expcce_avs_rem4"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → EXPNEG → CCEAVIRE.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → EXPNEG → CCEAVIRE.FRM**: [CMXsrv_util_fmt_txt](#referencia-cmxsrv_util_fmt_txt)

---

## CMXsrv_expret_swf_sel
<a name="cmxsrv_expret_swf_sel"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → expret → RET00501.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → expret → GRL00101.FRM**: [CMXsrv_expret_swf_100](#referencia-cmxsrv_expret_swf_100)
- **Exportaciones → expret → GRL00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → expret → GRL00101.FRM**: [CMXsrv_expret_swf_202](#referencia-cmxsrv_expret_swf_202)
- **Exportaciones → expret → RET00501.FRM**: [CMXsrv_expret_swf_100](#referencia-cmxsrv_expret_swf_100)
- **Exportaciones → expret → RET00501.FRM**: [CMXsrv_expret_swf_202](#referencia-cmxsrv_expret_swf_202)

---

## CMXsrv_expret_lee_ret
<a name="cmxsrv_expret_lee_ret"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → expret → RET00101.FRM**: [CMXsrv_cmx_busc_suc_usu](#referencia-cmxsrv_cmx_busc_suc_usu)
- **Exportaciones → expret → RET00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → expret → RET00101.FRM**: [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)

---

## CMXsrv_expret_lee_prm
<a name="cmxsrv_expret_lee_prm"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → expret → RET00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → expret → RET00101.FRM**: [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)

---

## CMXsrv_expret_avs_cyg1
<a name="cmxsrv_expret_avs_cyg1"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → expret → RET00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_avs_cyg2
<a name="cmxsrv_expret_avs_cyg2"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → expret → RET00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_avs_liq1
<a name="cmxsrv_expret_avs_liq1"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → expret → RET00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_avs_liq2
<a name="cmxsrv_expret_avs_liq2"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → expret → RET00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_avs_liq3
<a name="cmxsrv_expret_avs_liq3"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → expret → RET00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_val_ret
<a name="cmxsrv_expret_val_ret"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → expret → RET00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → expret → RET00102.FRM**: [CMXsrv_util_len](#referencia-cmxsrv_util_len)
- **Exportaciones → expret → RET00102.FRM**: [CMXsrv_val_vig](#referencia-cmxsrv_val_vig)
- **Exportaciones → expret → RET00102.FRM**: [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)
- **Exportaciones → expret → RET00102.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → expret → RET00101.FRM**: [CMXsrv_enl_val_sel](#referencia-cmxsrv_enl_val_sel)
- **Exportaciones → expret → RET00101.FRM**: [CMXsrv_val_vig](#referencia-cmxsrv_val_vig)
- **Exportaciones → expret → RET00101.FRM**: [CMXsrv_val_cta_cte](#referencia-cmxsrv_val_cta_cte)
- **Exportaciones → expret → RET00102.FRM**: [CMXsrv_val_cta_cte](#referencia-cmxsrv_val_cta_cte)
- **Exportaciones → expret → RET00102.FRM**: [CMXsrv_enl_val_sel](#referencia-cmxsrv_enl_val_sel)
- **Exportaciones → expret → RET00101.FRM**: [CMXsrv_util_len](#referencia-cmxsrv_util_len)
- **Exportaciones → expret → RET00101.FRM**: [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)

---

## CMXsrv_expret_sum_dtn_mn
<a name="cmxsrv_expret_sum_dtn_mn"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → expret → RET00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_ctb_ing
<a name="cmxsrv_expret_ctb_ing"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → expret → RET00101.FRM**: [CMXsrv_expret_grb_org](#referencia-cmxsrv_expret_grb_org)
- **Exportaciones → expret → RET00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → expret → RET00101.FRM**: [CMXsrv_cnt_950](#referencia-cmxsrv_cnt_950)
- **Exportaciones → expret → RET00101.FRM**: [CMXsrv_expret_grb_det](#referencia-cmxsrv_expret_grb_det)
- **Exportaciones → expret → RET00101.FRM**: [CMXsrv_cnt_810](#referencia-cmxsrv_cnt_810)
- **Exportaciones → expret → RET00101.FRM**: [CMXsrv_cnt_res_vig](#referencia-cmxsrv_cnt_res_vig)
- **Exportaciones → expret → RET00101.FRM**: [sp_cmx_sii_1870](#referencia-sp_cmx_sii_1870)
- **Exportaciones → expret → RET00101.FRM**: [CMXsrv_expret_val_ret](#referencia-cmxsrv_expret_val_ret)
- **Exportaciones → expret → RET00101.FRM**: [CMXsrv_expret_cnt_cyg](#referencia-cmxsrv_expret_cnt_cyg)
- **Exportaciones → expret → RET00101.FRM**: [CMXsrv_enl_act_enl](#referencia-cmxsrv_enl_act_enl)
- **Exportaciones → expret → RET00101.FRM**: [CMXsrv_cnt_800](#referencia-cmxsrv_cnt_800)
- **Exportaciones → expret → RET00101.FRM**: [CMXsrv_vig_gra_vig](#referencia-cmxsrv_vig_gra_vig)
- **Exportaciones → expret → RET00101.FRM**: [sp_cmx_sii_1862](#referencia-sp_cmx_sii_1862)
- **Exportaciones → expret → RET00101.FRM**: [CMXsrv_mbyte_gen](#referencia-cmxsrv_mbyte_gen)
- **Exportaciones → expret → RET00101.FRM**: [CMXsrv_expret_grb_evr](#referencia-cmxsrv_expret_grb_evr)
- **Exportaciones → expret → RET00101.FRM**: [CMXsrv_expret_grb_dtn](#referencia-cmxsrv_expret_grb_dtn)
- **Exportaciones → expret → RET00101.FRM**: [CMXsrv_expret_cre_ret](#referencia-cmxsrv_expret_cre_ret)

---

## CMXsrv_expret_del_ret
<a name="cmxsrv_expret_del_ret"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → expret → RET00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_avs_adm1
<a name="cmxsrv_expret_avs_adm1"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → expret → RET00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_avs_adm2
<a name="cmxsrv_expret_avs_adm2"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → expret → RET00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_avs_adm3
<a name="cmxsrv_expret_avs_adm3"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → expret → RET00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_act_tpo_cbo
<a name="cmxsrv_expret_act_tpo_cbo"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → expret → RET00102.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_cre_ret
<a name="cmxsrv_expret_cre_ret"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → expret → RET00201.FRM**: [CMXsrv_util_num_ope](#referencia-cmxsrv_util_num_ope)
- **Exportaciones → expret → RET00201.FRM**: [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)
- **Exportaciones → expret → RET00201.FRM**: [CMXsrv_cmx_busc_suc_usu](#referencia-cmxsrv_cmx_busc_suc_usu)
- **Exportaciones → expret → RET00201.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_grb_det
<a name="cmxsrv_expret_grb_det"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → expret → RET00201.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_tpo_cbo
<a name="cmxsrv_expret_tpo_cbo"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → expret → RET00201.FRM**: [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)
- **Exportaciones → expret → RET00201.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_lee_cln
<a name="cmxsrv_expret_lee_cln"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → expret → RET00601.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → expret → RET00201.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → expret → RET00701.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_lee_det
<a name="cmxsrv_expret_lee_det"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → expret → RET00201.FRM**: [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)
- **Exportaciones → expret → RET00201.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_del_org
<a name="cmxsrv_expret_del_org"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → expret → RET00301.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_bus_org
<a name="cmxsrv_expret_bus_org"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → expret → RET00301.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_grb_org
<a name="cmxsrv_expret_grb_org"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → expret → RET00401.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_mto_org
<a name="cmxsrv_expret_mto_org"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → expret → RET00401.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_lee_org
<a name="cmxsrv_expret_lee_org"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → expret → RET00401.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_vig_lee_cta
<a name="cmxsrv_vig_lee_cta"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → expret → RET00401.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → PAGCBR → CBR01006.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_del_dtn
<a name="cmxsrv_expret_del_dtn"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → expret → RET00501.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_bus_dtn
<a name="cmxsrv_expret_bus_dtn"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → expret → RET00501.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_grb_dtn
<a name="cmxsrv_expret_grb_dtn"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → expret → RET00601.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_cal_arb
<a name="cmxsrv_expret_cal_arb"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → expret → RET00601.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_mto_dtn
<a name="cmxsrv_expret_mto_dtn"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → expret → RET00601.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_lee_dtn
<a name="cmxsrv_expret_lee_dtn"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → expret → RET00601.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_bus_ret
<a name="cmxsrv_expret_bus_ret"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → expret → RET00701.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_bus_evr
<a name="cmxsrv_expret_bus_evr"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → expret → RET00801.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_rev_ret
<a name="cmxsrv_expret_rev_ret"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → expret → RET00801.FRM**: [CMXsrv_cnt_rev_vig](#referencia-cmxsrv_cnt_rev_vig)
- **Exportaciones → expret → RET00801.FRM**: [CMXsrv_ctl_chq_aprcbl](#referencia-cmxsrv_ctl_chq_aprcbl)
- **Exportaciones → expret → RET00801.FRM**: [sp_cmx_sii_1870](#referencia-sp_cmx_sii_1870)
- **Exportaciones → expret → RET00801.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Exportaciones → expret → RET00801.FRM**: [CMXsrv_cnt_801](#referencia-cmxsrv_cnt_801)
- **Exportaciones → expret → RET00801.FRM**: [CMXsrv_rev_950](#referencia-cmxsrv_rev_950)
- **Exportaciones → expret → RET00801.FRM**: [CMXsrv_enl_rev_enl](#referencia-cmxsrv_enl_rev_enl)
- **Exportaciones → expret → RET00801.FRM**: [CMXsrv_expret_rev_cyg](#referencia-cmxsrv_expret_rev_cyg)
- **Exportaciones → expret → RET00801.FRM**: [sp_cmx_sii_1862](#referencia-sp_cmx_sii_1862)
- **Exportaciones → expret → RET00801.FRM**: [CMXsrv_mbyte_gen](#referencia-cmxsrv_mbyte_gen)
- **Exportaciones → expret → RET00801.FRM**: [CMXsrv_expret_grb_evr](#referencia-cmxsrv_expret_grb_evr)
- **Exportaciones → expret → RET00801.FRM**: [CMXsrv_cnt_811](#referencia-cmxsrv_cnt_811)

---

## CMXsrv_expret_lee_evr
<a name="cmxsrv_expret_lee_evr"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Exportaciones → expret → RET00802.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finadm_imod_desti
<a name="cmxsrv_finadm_imod_desti"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → ADMIN → ADM00201.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → ADMIN → ADM00201.FRM**: [CMXsrv_finadm_val_tipop](#referencia-cmxsrv_finadm_val_tipop)

---

## CMXsrv_finadm_cons_dtip
<a name="cmxsrv_finadm_cons_dtip"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → ADMIN → ADM00201.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finadm_imod_ectb
<a name="cmxsrv_finadm_imod_ectb"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → ADMIN → ADM00202.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → ADMIN → ADM00202.FRM**: [CMXsrv_finadm_val_tipop](#referencia-cmxsrv_finadm_val_tipop)

---

## CMXsrv_finadm_eli_tipop
<a name="cmxsrv_finadm_eli_tipop"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → ADMIN → ADM00203.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → ADMIN → ADM00202.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → ADMIN → ADM00204.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finadm_cons_ectb
<a name="cmxsrv_finadm_cons_ectb"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → ADMIN → ADM00202.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finadm_imod_itip
<a name="cmxsrv_finadm_imod_itip"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → ADMIN → ADM00203.FRM**: [CMXsrv_finadm_val_tipop](#referencia-cmxsrv_finadm_val_tipop)
- **Financiamiento → ADMIN → ADM00203.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finadm_cons_itip
<a name="cmxsrv_finadm_cons_itip"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → ADMIN → ADM00203.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finadm_lee_tipop
<a name="cmxsrv_finadm_lee_tipop"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → ADMIN → ADM00204.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finadm_val_tipop
<a name="cmxsrv_finadm_val_tipop"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → ADMIN → ADM00204.FRM**: [CMXsrv_fincol_eval_tbat](#referencia-cmxsrv_fincol_eval_tbat)
- **Financiamiento → ADMIN → ADM00204.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → ADMIN → ADM00204.FRM**: [SRV_MessageService](#referencia-srv_messageservice)
- **Financiamiento → ADMIN → ADM00204.FRM**: [CMXsrv_util_fecha2](#referencia-cmxsrv_util_fecha2)

---

## CMXsrv_finadm_bus_tipope
<a name="cmxsrv_finadm_bus_tipope"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → ADMIN → ADM00205.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_busc_tip_tas
<a name="cmxsrv_busc_tip_tas"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → COL_NEG → COL00102.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_ecuo
<a name="cmxsrv_fincol_ecuo"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → INGRESO → COL00102.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → INGRESO → COL00102.FRM**: [CMXsrv_fincol_pre_cuad_tas](#referencia-cmxsrv_fincol_pre_cuad_tas)
- **Financiamiento → COL_NEG → COL00102.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → COL_NEG → COL00102.FRM**: [CMXsrv_fincol_pre_cuad_tas](#referencia-cmxsrv_fincol_pre_cuad_tas)

---

## CMXsrv_fincol_cons_plnpa
<a name="cmxsrv_fincol_cons_plnpa"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → INGRESO → COL00102.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → COL_NEG → COL00102.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_pertas_val_display
<a name="cmxsrv_pertas_val_display"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → COL_NEG → COL00102.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_eava
<a name="cmxsrv_fincol_eava"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → COL_NEG → COL00103.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → INGRESO → COL00103.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_cons_aval
<a name="cmxsrv_fincol_cons_aval"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → COL_NEG → COL00103.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → INGRESO → COL00103.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_iava
<a name="cmxsrv_fincol_iava"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → INGRESO → COL00113.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → COL_NEG → COL00113.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_cons_pag
<a name="cmxsrv_fincol_cons_pag"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → PAGOS → COL00303.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → COL_NEG → COL00303.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_trae_det_pag
<a name="cmxsrv_fincol_trae_det_pag"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → COL_NEG → COL00304.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_cons_pror
<a name="cmxsrv_fincol_cons_pror"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → COL_NEG → COL00403.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → PAGOS → COL00403.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_cons_eve
<a name="cmxsrv_fincol_cons_eve"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → COL_NEG → COL00901.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → MODIFIC → COL00901.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_bco_swf
<a name="cmxsrv_icrd_lee_bco_swf"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → MOD_CRD → CRD00205.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → MOD_ADI → CRD00202.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → INGRESO → CRD00602.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → MOD_CRD → MOD00603.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → INGRESO → COL00104.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → COL_NEG → CRD00602.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → MOD_ADI → CRD00202.FRM**: [CMXsrv_icrd_lee_cln](#referencia-cmxsrv_icrd_lee_cln)
- **Importaciones → MOD_CRD → CRD00205.FRM**: [CMXsrv_icrd_lee_cln](#referencia-cmxsrv_icrd_lee_cln)
- **Financiamiento → INGRESO → CRD00602.FRM**: [CMXsrv_icrd_lee_cln](#referencia-cmxsrv_icrd_lee_cln)
- **Importaciones → MOD_CRD → MOD00603.FRM**: [CMXsrv_icrd_lee_cln](#referencia-cmxsrv_icrd_lee_cln)
- **Financiamiento → INGRESO → COL00104.FRM**: [CMXsrv_icrd_lee_cln](#referencia-cmxsrv_icrd_lee_cln)
- **Financiamiento → COL_NEG → CRD00602.FRM**: [CMXsrv_icrd_lee_cln](#referencia-cmxsrv_icrd_lee_cln)

---

## CMXsrv_icrd_busc_bco
<a name="cmxsrv_icrd_busc_bco"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → INGRESO → CRD00602.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → COL_NEG → CRD00602.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_vtocre_prov
<a name="cmxsrv_fincol_vtocre_prov"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → COL_NEG → CRD01401.FRM**: [CMXsrv_finobl_imod_obl](#referencia-cmxsrv_finobl_imod_obl)
- **Financiamiento → COL_NEG → CRD01401.FRM**: [CMXsrv_fincol_ctb_vcp](#referencia-cmxsrv_fincol_ctb_vcp)
- **Financiamiento → COL_NEG → CRD01401.FRM**: [CMXsrv_fincol_gpln](#referencia-cmxsrv_fincol_gpln)
- **Financiamiento → COL_NEG → CRD01401.FRM**: [CMXsrv_util_fecha](#referencia-cmxsrv_util_fecha)
- **Financiamiento → COL_NEG → CRD01401.FRM**: [CMXsrv_util_val_tasas](#referencia-cmxsrv_util_val_tasas)
- **Financiamiento → COL_NEG → CRD01401.FRM**: [sp_cmx_sii_1870](#referencia-sp_cmx_sii_1870)
- **Financiamiento → COL_NEG → CRD01401.FRM**: [CMXsrv_fincol_efec_calpa](#referencia-cmxsrv_fincol_efec_calpa)
- **Financiamiento → COL_NEG → CRD01401.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_prec_vtocre
<a name="cmxsrv_fincol_prec_vtocre"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → COL_NEG → CRD01401.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_bus_lcr_bco
<a name="cmxsrv_icrd_bus_lcr_bco"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → CRDEXT → CRD02001.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → CRD_CORR → COR00202.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → COL_NEG → CRD02001.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_lee_fpro
<a name="cmxsrv_lee_fpro"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → OBLIGA → OBL00103.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → MODIFIC → PREFER.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → INGRESO → COL00106.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → PAGOS → PREFER.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → COL_NEG → PREFER.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → IMPORT → CRD00201.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → PGOEXT → PREFER.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_ren_fin
<a name="cmxsrv_fincol_ren_fin"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → INGRESO → COL00102.FRM**: [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)
- **Financiamiento → INGRESO → COL00103.FRM**: [CMXsrv_fincol_pre_cuad_tas](#referencia-cmxsrv_fincol_pre_cuad_tas)
- **Financiamiento → INGRESO → COL00103.FRM**: [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)
- **Financiamiento → INGRESO → COL00102.FRM**: [CMXsrv_fincol_pre_cuad_tas](#referencia-cmxsrv_fincol_pre_cuad_tas)
- **Financiamiento → INGRESO → COL00103.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → INGRESO → COL00102.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → INGRESO → COL00103.FRM**: [CMXsrv_cmx_fec_hoy](#referencia-cmxsrv_cmx_fec_hoy)
- **Financiamiento → INGRESO → COL00103.FRM**: [CMXsrv_fincol_grb_col_ren](#referencia-cmxsrv_fincol_grb_col_ren)
- **Financiamiento → INGRESO → COL00102.FRM**: [CMXsrv_fincol_grb_col_ren](#referencia-cmxsrv_fincol_grb_col_ren)
- **Financiamiento → INGRESO → COL00102.FRM**: [CMXsrv_cmx_fec_hoy](#referencia-cmxsrv_cmx_fec_hoy)

---

## CMXsrv_fincol_gmod_ctr
<a name="cmxsrv_fincol_gmod_ctr"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → INGRESO → COL00104.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_lee_bco
<a name="cmxsrv_fincol_lee_bco"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → INGRESO → COL00104.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_lee_cln
<a name="cmxsrv_fincol_lee_cln"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → INGRESO → COL00701.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → INGRESO → COL00703.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → INGRESO → COL00104.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_cons_ctr
<a name="cmxsrv_fincol_cons_ctr"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → INGRESO → COL00104.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_ctb_oto
<a name="cmxsrv_fincol_ctb_oto"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → INGRESO → COL00106.FRM**: [sp_cmx_sii_1870](#referencia-sp_cmx_sii_1870)
- **Financiamiento → INGRESO → COL00105.FRM**: [CMXsrv_nibx_nilive](#referencia-cmxsrv_nibx_nilive)
- **Financiamiento → INGRESO → COL00105.FRM**: [CMXsrv_mbyte_gen](#referencia-cmxsrv_mbyte_gen)
- **Financiamiento → INGRESO → COL00106.FRM**: [CMXsrv_ctb_otorga](#referencia-cmxsrv_ctb_otorga)
- **Financiamiento → INGRESO → COL00105.FRM**: [sp_cmx_sii_1870](#referencia-sp_cmx_sii_1870)
- **Financiamiento → INGRESO → COL00106.FRM**: [CMXsrv_vig_gra_vig](#referencia-cmxsrv_vig_gra_vig)
- **Financiamiento → INGRESO → COL00105.FRM**: [CMXsrv_ctb_otorga](#referencia-cmxsrv_ctb_otorga)
- **Financiamiento → INGRESO → COL00105.FRM**: [CMXsrv_vig_gra_vig](#referencia-cmxsrv_vig_gra_vig)
- **Financiamiento → INGRESO → COL00106.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → INGRESO → COL00106.FRM**: [CMXsrv_cmx_ing_lib](#referencia-cmxsrv_cmx_ing_lib)
- **Financiamiento → INGRESO → COL00106.FRM**: [CMXsrv_ctb_impto_tim](#referencia-cmxsrv_ctb_impto_tim)
- **Financiamiento → INGRESO → COL00106.FRM**: [CMXsrv_cnt_gen_vig](#referencia-cmxsrv_cnt_gen_vig)
- **Financiamiento → INGRESO → COL00106.FRM**: [CMXsrv_ctb_impto_tim2](#referencia-cmxsrv_ctb_impto_tim2)
- **Financiamiento → INGRESO → COL00106.FRM**: [CMXsrv_util_pesos](#referencia-cmxsrv_util_pesos)
- **Financiamiento → INGRESO → COL00105.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → INGRESO → COL00105.FRM**: [CMXsrv_cmx_ing_lib](#referencia-cmxsrv_cmx_ing_lib)
- **Financiamiento → INGRESO → COL00106.FRM**: [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)
- **Financiamiento → INGRESO → COL00106.FRM**: [CMXsrv_nibx_upd_tran](#referencia-cmxsrv_nibx_upd_tran)
- **Financiamiento → INGRESO → COL00105.FRM**: [CMXsrv_ctb_impto_tim](#referencia-cmxsrv_ctb_impto_tim)
- **Financiamiento → INGRESO → COL00106.FRM**: [CMXsrv_cnt_999999](#referencia-cmxsrv_cnt_999999)
- **Financiamiento → INGRESO → COL00105.FRM**: [CMXsrv_util_pesos](#referencia-cmxsrv_util_pesos)
- **Financiamiento → INGRESO → COL00106.FRM**: [CMXsrv_fincol_val_col](#referencia-cmxsrv_fincol_val_col)
- **Financiamiento → INGRESO → COL00105.FRM**: [CMXsrv_cnt_gen_vig](#referencia-cmxsrv_cnt_gen_vig)
- **Financiamiento → INGRESO → COL00105.FRM**: [CMXsrv_ctb_impto_tim2](#referencia-cmxsrv_ctb_impto_tim2)
- **Financiamiento → INGRESO → COL00105.FRM**: [CMXsrv_cnt_999999](#referencia-cmxsrv_cnt_999999)
- **Financiamiento → INGRESO → COL00105.FRM**: [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)
- **Financiamiento → INGRESO → COL00105.FRM**: [CMXsrv_fincol_val_col](#referencia-cmxsrv_fincol_val_col)
- **Financiamiento → INGRESO → COL00105.FRM**: [CMXsrv_nibx_upd_tran](#referencia-cmxsrv_nibx_upd_tran)
- **Financiamiento → INGRESO → COL00106.FRM**: [CMXsrv_cyo_dsc](#referencia-cmxsrv_cyo_dsc)
- **Financiamiento → INGRESO → COL00105.FRM**: [CMXsrv_cyo_dsc](#referencia-cmxsrv_cyo_dsc)
- **Financiamiento → INGRESO → COL00106.FRM**: [CMXsrv_nibx_nilive](#referencia-cmxsrv_nibx_nilive)
- **Financiamiento → INGRESO → COL00106.FRM**: [CMXsrv_mbyte_gen](#referencia-cmxsrv_mbyte_gen)

---

## CMXsrv_icrd_dat_liq_ope
<a name="cmxsrv_icrd_dat_liq_ope"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → OBLIGA → OBL00103.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → INGRESO → COL00106.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → NEGO_AV → AVISOS.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → IMPORT → CRD00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → NEGO_AV → CRD01001.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_lee_col
<a name="cmxsrv_fincol_lee_col"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → INGRESO → COL00107.FRM**: [PrmACLNEJECTA](#referencia-prmaclnejecta)
- **Financiamiento → INGRESO → COL00106.FRM**: [PrmACMXESPECI](#referencia-prmacmxespeci)
- **Financiamiento → INGRESO → COL00106.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → INGRESO → COL00106.FRM**: [PrmACLNEJECTA](#referencia-prmaclnejecta)
- **Financiamiento → INGRESO → COL00107.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → INGRESO → COL00107.FRM**: [PrmACMXESPECI](#referencia-prmacmxespeci)

---

## CMXsrv_busc_cod_ope
<a name="cmxsrv_busc_cod_ope"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → INGRESO → COL00701.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → PGOEXT → PGOCOL01.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → PAGOS → COL00501.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → INGRESO → COL00106.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_col_trae_num_ope
<a name="cmxsrv_col_trae_num_ope"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → INGRESO → COL00701.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → PAGOS → COL00501.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → INGRESO → COL00106.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_eli_col
<a name="cmxsrv_fincol_eli_col"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → INGRESO → COL00106.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_val_col
<a name="cmxsrv_fincol_val_col"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → INGRESO → COL00106.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → INGRESO → COL00106.FRM**: [CMXsrv_fincol_val_adv](#referencia-cmxsrv_fincol_val_adv)
- **Financiamiento → INGRESO → COL00106.FRM**: [CMXsrv_fincol_val_per_tas](#referencia-cmxsrv_fincol_val_per_tas)
- **Financiamiento → INGRESO → COL00106.FRM**: [CMXsrv_fincol_val_err](#referencia-cmxsrv_fincol_val_err)

---

## CMXsrv_fincol_bsc_col
<a name="cmxsrv_fincol_bsc_col"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → INGRESO → COL00107.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_lee_tip
<a name="cmxsrv_fincol_lee_tip"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → INGRESO → COL00107.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → OBLIGA → OBL00104.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_ctb_novf
<a name="cmxsrv_fincol_ctb_novf"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → INGRESO → COL00701.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → INGRESO → COL00701.FRM**: [CMXsrv_fincol_ctb_nov](#referencia-cmxsrv_fincol_ctb_nov)
- **Financiamiento → INGRESO → COL00701.FRM**: [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)

---

## CMXsrv_fincol_cons_nov
<a name="cmxsrv_fincol_cons_nov"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → INGRESO → COL00702.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_cmx_get_codes
<a name="cmxsrv_cmx_get_codes"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → INGRESO → PREFER.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → OBLIGA → PREFER.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → IMPORT → CRD00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_grl_trae_cod_bco
<a name="cmxsrv_grl_trae_cod_bco"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → INGRESO → PREFER.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → PAGOS → PREFER.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_cons_tas
<a name="cmxsrv_fincol_cons_tas"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → MODIFIC → COL00303.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_efec_tras
<a name="cmxsrv_fincol_efec_tras"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → MODIFIC → COL00801.FRM**: [CMXsrv_cnt_9000](#referencia-cmxsrv_cnt_9000)
- **Financiamiento → MODIFIC → COL00801.FRM**: [CMXsrv_fincol_ctb_cst](#referencia-cmxsrv_fincol_ctb_cst)
- **Financiamiento → MODIFIC → COL00801.FRM**: [CMXsrv_fincol_ctb_cnd](#referencia-cmxsrv_fincol_ctb_cnd)
- **Financiamiento → MODIFIC → COL00801.FRM**: [CMXsrv_fincol_calc_cven](#referencia-cmxsrv_fincol_calc_cven)
- **Financiamiento → MODIFIC → COL00801.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → MODIFIC → COL00801.FRM**: [CMXsrv_fincol_ctb_cob](#referencia-cmxsrv_fincol_ctb_cob)

---

## CMXsrv_fincol_cons_trasp
<a name="cmxsrv_fincol_cons_trasp"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → MODIFIC → COL00802.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_cons_dtrs
<a name="cmxsrv_fincol_cons_dtrs"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → MODIFIC → COL00803.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_cons_deve
<a name="cmxsrv_fincol_cons_deve"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → MODIFIC → COL00902.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_cont_gst
<a name="cmxsrv_fincol_cont_gst"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → MODIFIC → COL01001.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_cons_gst
<a name="cmxsrv_fincol_cons_gst"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → MODIFIC → COL01002.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_cons_dgst
<a name="cmxsrv_fincol_cons_dgst"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → MODIFIC → COL01003.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_bsc_tip
<a name="cmxsrv_fincol_bsc_tip"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → OBLIGA → COL00108.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_bus_cor
<a name="cmxsrv_finobl_bus_cor"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → OBLIGA → CRD00602.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_ecuo
<a name="cmxsrv_finobl_ecuo"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → OBLIGA → OBL00102.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_gpln
<a name="cmxsrv_finobl_gpln"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → OBLIGA → OBL00102.FRM**: [CMXsrv_util_det_habil_tasa](#referencia-cmxsrv_util_det_habil_tasa)
- **Financiamiento → OBLIGA → OBL00102.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_cons_plnpa
<a name="cmxsrv_finobl_cons_plnpa"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → OBLIGA → OBL00102.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_calc_anu
<a name="cmxsrv_finobl_calc_anu"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → OBLIGA → OBL00103.FRM**: [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)
- **Financiamiento → OBLIGA → OBL00402.FRM**: [CMXsrv_finobl_efec_calpa](#referencia-cmxsrv_finobl_efec_calpa)
- **Financiamiento → OBLIGA → OBL00103.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → OBLIGA → OBL00103.FRM**: [CMXsrv_finobl_efec_calpa](#referencia-cmxsrv_finobl_efec_calpa)
- **Financiamiento → OBLIGA → OBL00402.FRM**: [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)
- **Financiamiento → OBLIGA → OBL00402.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_lee_obl
<a name="cmxsrv_finobl_lee_obl"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → OBLIGA → OBL00103.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_ctb_oto
<a name="cmxsrv_finobl_ctb_oto"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → OBLIGA → OBL00103.FRM**: [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)
- **Financiamiento → OBLIGA → OBL00103.FRM**: [CMXsrv_finobl_val_obl](#referencia-cmxsrv_finobl_val_obl)
- **Financiamiento → OBLIGA → OBL00103.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → OBLIGA → OBL00103.FRM**: [CMXsrv_ctbo_otorga](#referencia-cmxsrv_ctbo_otorga)

---

## CMXsrv_fincol_eli_obl
<a name="cmxsrv_fincol_eli_obl"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → OBLIGA → OBL00103.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_val_obl
<a name="cmxsrv_finobl_val_obl"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → OBLIGA → OBL00103.FRM**: [CMXsrv_finobl_val_adv](#referencia-cmxsrv_finobl_val_adv)
- **Financiamiento → OBLIGA → OBL00103.FRM**: [CMXsrv_util_det_habil_tasa](#referencia-cmxsrv_util_det_habil_tasa)
- **Financiamiento → OBLIGA → OBL00103.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_bsc_obl
<a name="cmxsrv_finobl_bsc_obl"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → OBLIGA → OBL00104.FRM**: [CMXsrv_finobl_bsc_obl2](#referencia-cmxsrv_finobl_bsc_obl2)
- **Financiamiento → OBLIGA → OBL00104.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → OBLIGA → OBL00104.FRM**: [CMXsrv_finobl_bsc_obl3](#referencia-cmxsrv_finobl_bsc_obl3)

---

## CMXsrv_finobl_ictb_pag
<a name="cmxsrv_finobl_ictb_pag"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → OBLIGA → OBL00202.FRM**: [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)
- **Financiamiento → OBLIGA → OBL00202.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → OBLIGA → OBL00202.FRM**: [CMXsrv_finobl_ctb_pag](#referencia-cmxsrv_finobl_ctb_pag)

---

## CMXsrv_finobl_obt_sdocuo
<a name="cmxsrv_finobl_obt_sdocuo"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → OBLIGA → OBL00202.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_new_tas
<a name="cmxsrv_finobl_new_tas"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → OBLIGA → OBL00202.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_cons_pag
<a name="cmxsrv_finobl_cons_pag"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → OBLIGA → OBL00203.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_cons_detp
<a name="cmxsrv_finobl_cons_detp"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → OBLIGA → OBL00204.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_calc_pror
<a name="cmxsrv_finobl_calc_pror"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → OBLIGA → OBL00301.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → OBLIGA → OBL00301.FRM**: [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)
- **Financiamiento → OBLIGA → OBL00301.FRM**: [CMXsrv_finobl_efec_calpa](#referencia-cmxsrv_finobl_efec_calpa)

---

## CMXsrv_finobl_cons_pror
<a name="cmxsrv_finobl_cons_pror"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → OBLIGA → OBL00303.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_cons_dpror
<a name="cmxsrv_finobl_cons_dpror"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → OBLIGA → OBL00304.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_ctb_anu
<a name="cmxsrv_finobl_ctb_anu"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → OBLIGA → OBL00401.FRM**: [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)
- **Financiamiento → OBLIGA → OBL00401.FRM**: [CMXsrv_finobl_cbo_anu](#referencia-cmxsrv_finobl_cbo_anu)
- **Financiamiento → OBLIGA → OBL00401.FRM**: [CMXsrv_ctbo_anula](#referencia-cmxsrv_ctbo_anula)
- **Financiamiento → OBLIGA → OBL00401.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_cons_anu
<a name="cmxsrv_finobl_cons_anu"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → OBLIGA → OBL00402.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_cons_mod
<a name="cmxsrv_finobl_cons_mod"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → OBLIGA → OBL00502.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_cons_dmod
<a name="cmxsrv_finobl_cons_dmod"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → OBLIGA → OBL00503.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_rev_eve
<a name="cmxsrv_finobl_rev_eve"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → OBLIGA → OBL00601.FRM**: [CMXsrv_rctb_cesi](#referencia-cmxsrv_rctb_cesi)
- **Financiamiento → OBLIGA → OBL00601.FRM**: [CMXsrv_finobl_rctb_pror](#referencia-cmxsrv_finobl_rctb_pror)
- **Financiamiento → OBLIGA → OBL00601.FRM**: [CMXsrv_finobl_rctb_pag](#referencia-cmxsrv_finobl_rctb_pag)
- **Financiamiento → OBLIGA → OBL00601.FRM**: [CMXsrv_finobl_rctb_oto](#referencia-cmxsrv_finobl_rctb_oto)
- **Financiamiento → OBLIGA → OBL00601.FRM**: [CMXsrv_finobl_rctb_pext](#referencia-cmxsrv_finobl_rctb_pext)
- **Financiamiento → OBLIGA → OBL00601.FRM**: [CMXsrv_finobl_rctb_mod](#referencia-cmxsrv_finobl_rctb_mod)
- **Financiamiento → OBLIGA → OBL00601.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → OBLIGA → OBL00601.FRM**: [CMXsrv_finobl_rctb_anu](#referencia-cmxsrv_finobl_rctb_anu)
- **Financiamiento → OBLIGA → OBL00601.FRM**: [CMXsrv_ctl_chq_aprcbl](#referencia-cmxsrv_ctl_chq_aprcbl)
- **Financiamiento → OBLIGA → OBL00601.FRM**: [CMXsrv_ctl_marc_rev](#referencia-cmxsrv_ctl_marc_rev)

---

## CMXsrv_finobl_cons_eve
<a name="cmxsrv_finobl_cons_eve"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → OBLIGA → OBL00601.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_cons_deve
<a name="cmxsrv_finobl_cons_deve"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → OBLIGA → OBL00602.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_eli_ctr
<a name="cmxsrv_finobl_eli_ctr"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → OBLIGA → OBL00701.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_cons_ctr
<a name="cmxsrv_finobl_cons_ctr"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → OBLIGA → OBL00701.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_ing_ctr
<a name="cmxsrv_finobl_ing_ctr"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → OBLIGA → OBL00702.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_cesion_obl
<a name="cmxsrv_finobl_cesion_obl"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → OBLIGA → OBL130.FRM**: [CMXsrv_ctl_crea_apr](#referencia-cmxsrv_ctl_crea_apr)
- **Financiamiento → OBLIGA → OBL130.FRM**: [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)
- **Financiamiento → OBLIGA → OBL130.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_comgrl_lee_nom_cor
<a name="cmxsrv_comgrl_lee_nom_cor"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → OBLIGA → OBL130.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_lee_cln
<a name="cmxsrv_lee_cln"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → OBLIGA → OBL130.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_busc_acre
<a name="cmxsrv_finobl_busc_acre"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → OBLIGA → OBL130.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_efec_calpa
<a name="cmxsrv_fincol_efec_calpa"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → PAGOS → COL00301.FRM**: [CMXsrv_fincol_calc_reba](#referencia-cmxsrv_fincol_calc_reba)
- **Importaciones → MOD_CRD → MOD00603.FRM**: [CMXsrv_fincol_calc_reba](#referencia-cmxsrv_fincol_calc_reba)
- **Financiamiento → PAGOS → COL00301.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → PAGOS → COL00301.FRM**: [CMXsrv_fincol_eval_tasa](#referencia-cmxsrv_fincol_eval_tasa)
- **Importaciones → MOD_CRD → MOD00603.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → MOD_CRD → MOD00603.FRM**: [CMXsrv_fincol_eval_tasa](#referencia-cmxsrv_fincol_eval_tasa)
- **Financiamiento → PAGOS → COL00301.FRM**: [CMXsrv_fincol_cal_tas_sfr](#referencia-cmxsrv_fincol_cal_tas_sfr)
- **Financiamiento → PAGOS → COL00301.FRM**: [CMXsrv_fincol_eval_tnem](#referencia-cmxsrv_fincol_eval_tnem)
- **Importaciones → MOD_CRD → MOD00603.FRM**: [CMXsrv_fincol_cal_tas_sfr](#referencia-cmxsrv_fincol_cal_tas_sfr)
- **Financiamiento → PAGOS → COL00301.FRM**: [CMXsrv_util_det_habil](#referencia-cmxsrv_util_det_habil)
- **Importaciones → MOD_CRD → MOD00603.FRM**: [CMXsrv_fincol_eval_tnem](#referencia-cmxsrv_fincol_eval_tnem)
- **Financiamiento → PAGOS → COL00301.FRM**: [CMXsrv_fincol_eval_tneg](#referencia-cmxsrv_fincol_eval_tneg)
- **Importaciones → MOD_CRD → MOD00603.FRM**: [CMXsrv_util_det_habil](#referencia-cmxsrv_util_det_habil)
- **Financiamiento → PAGOS → COL00301.FRM**: [CMXsrv_fincol_efcal_cv](#referencia-cmxsrv_fincol_efcal_cv)
- **Importaciones → MOD_CRD → MOD00603.FRM**: [CMXsrv_fincol_eval_tneg](#referencia-cmxsrv_fincol_eval_tneg)
- **Financiamiento → PAGOS → COL00301.FRM**: [CMXsrv_fincol_eval_tmor](#referencia-cmxsrv_fincol_eval_tmor)
- **Importaciones → MOD_CRD → MOD00603.FRM**: [CMXsrv_fincol_efcal_cv](#referencia-cmxsrv_fincol_efcal_cv)
- **Importaciones → MOD_CRD → MOD00603.FRM**: [CMXsrv_fincol_eval_tmor](#referencia-cmxsrv_fincol_eval_tmor)

---

## CMXsrv_fincol_cons_detp
<a name="cmxsrv_fincol_cons_detp"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → PAGOS → COL00304.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_calc_pror
<a name="cmxsrv_fincol_calc_pror"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → PAGOS → COL00401.FRM**: [CMXsrv_fincol_efec_calpa](#referencia-cmxsrv_fincol_efec_calpa)
- **Financiamiento → PAGOS → COL00401.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → PAGOS → COL00401.FRM**: [CMXsrv_call_val_tas](#referencia-cmxsrv_call_val_tas)

---

## CMXsrv_fincol_cont_pror
<a name="cmxsrv_fincol_cont_pror"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → PAGOS → COL00402.FRM**: [CMXsrv_fincol_cam_new_tas](#referencia-cmxsrv_fincol_cam_new_tas)
- **Financiamiento → PAGOS → COL00402.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → PAGOS → COL00402.FRM**: [CMXsrv_cmx_ing_lib](#referencia-cmxsrv_cmx_ing_lib)
- **Financiamiento → PAGOS → COL00402.FRM**: [CMXsrv_ipuc_gen_pln](#referencia-cmxsrv_ipuc_gen_pln)
- **Financiamiento → PAGOS → COL00402.FRM**: [CMXsrv_util_val_tasas](#referencia-cmxsrv_util_val_tasas)
- **Financiamiento → PAGOS → COL00402.FRM**: [CMXsrv_ctb_impto_tim](#referencia-cmxsrv_ctb_impto_tim)
- **Financiamiento → PAGOS → COL00402.FRM**: [CMXsrv_cmx_get_codes](#referencia-cmxsrv_cmx_get_codes)
- **Financiamiento → PAGOS → COL00402.FRM**: [CMXsrv_fincol_ctb_pror](#referencia-cmxsrv_fincol_ctb_pror)
- **Financiamiento → PAGOS → COL00402.FRM**: [CMXsrv_util_pesos](#referencia-cmxsrv_util_pesos)
- **Financiamiento → PAGOS → COL00402.FRM**: [CMXsrv_mbyte_gen](#referencia-cmxsrv_mbyte_gen)
- **Financiamiento → PAGOS → COL00402.FRM**: [CMXsrv_get_ult_dia_habil](#referencia-cmxsrv_get_ult_dia_habil)
- **Financiamiento → PAGOS → COL00402.FRM**: [CMXsrv_int_ccx_cns](#referencia-cmxsrv_int_ccx_cns)
- **Financiamiento → PAGOS → COL00402.FRM**: [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)
- **Financiamiento → PAGOS → COL00402.FRM**: [CMXsrv_pertas_pror_tas](#referencia-cmxsrv_pertas_pror_tas)

---

## CMXsrv_fincol_cons_dpror
<a name="cmxsrv_fincol_cons_dpror"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → PAGOS → COL00404.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_cctb_anu
<a name="cmxsrv_fincol_cctb_anu"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → PAGOS → COL00501.FRM**: [sp_cmx_sii_1870](#referencia-sp_cmx_sii_1870)
- **Financiamiento → PAGOS → COL00501.FRM**: [CMXsrv_enl_act_enl](#referencia-cmxsrv_enl_act_enl)
- **Financiamiento → PAGOS → COL00501.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → PAGOS → COL00501.FRM**: [CMXsrv_busc_cod_ope](#referencia-cmxsrv_busc_cod_ope)
- **Financiamiento → PAGOS → COL00501.FRM**: [CMXsrv_fincol_ctb_anu](#referencia-cmxsrv_fincol_ctb_anu)
- **Financiamiento → PAGOS → COL00501.FRM**: [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)

---

## CMXsrv_fincol_calc_anu
<a name="cmxsrv_fincol_calc_anu"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → PAGOS → COL00501.FRM**: [CMXsrv_fincol_efec_calpa](#referencia-cmxsrv_fincol_efec_calpa)
- **Financiamiento → PAGOS → COL00501.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → PAGOS → COL00502.FRM**: [CMXsrv_fincol_efec_calpa](#referencia-cmxsrv_fincol_efec_calpa)
- **Financiamiento → PAGOS → COL00502.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_cons_anu
<a name="cmxsrv_fincol_cons_anu"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → PAGOS → COL00502.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_cons_mod
<a name="cmxsrv_fincol_cons_mod"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → PAGOS → COL00602.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_cons_dmod
<a name="cmxsrv_fincol_cons_dmod"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → PAGOS → COL00603.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_cal_pext
<a name="cmxsrv_fincol_cal_pext"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → PGOEXT → PGOCOL01.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → PGOEXT → PGOCOL01.FRM**: [CMXsrv_fincol_eval_tasa](#referencia-cmxsrv_fincol_eval_tasa)
- **Financiamiento → PGOEXT → PGOCOL01.FRM**: [CMXsrv_fincol_calc_reba](#referencia-cmxsrv_fincol_calc_reba)

---

## CMXsrv_fincol_ctb_pext
<a name="cmxsrv_fincol_ctb_pext"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → PGOEXT → PGOCOL01.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Financiamiento → PGOEXT → PGOCOL01.FRM**: [CMXsrv_ctb_pago](#referencia-cmxsrv_ctb_pago)
- **Financiamiento → PGOEXT → PGOCOL01.FRM**: [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)
- **Financiamiento → PGOEXT → PGOCOL01.FRM**: [CMXsrv_util_gen_vig](#referencia-cmxsrv_util_gen_vig)

---

## CMXsrv_finobl_cal_pext
<a name="cmxsrv_finobl_cal_pext"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → PGOEXT → PGOOBL01.FRM**: [CMXsrv_fincol_cal_tas_sfr](#referencia-cmxsrv_fincol_cal_tas_sfr)
- **Financiamiento → PGOEXT → PGOOBL01.FRM**: [CMXsrv_finobl_eval_tasa](#referencia-cmxsrv_finobl_eval_tasa)
- **Financiamiento → PGOEXT → PGOOBL01.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_ctb_pext
<a name="cmxsrv_finobl_ctb_pext"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Financiamiento → PGOEXT → PGOOBL01.FRM**: [CMXsrv_ctbo_pago](#referencia-cmxsrv_ctbo_pago)
- **Financiamiento → PGOEXT → PGOOBL01.FRM**: [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)
- **Financiamiento → PGOEXT → PGOOBL01.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iarc_eli_arc
<a name="cmxsrv_iarc_eli_arc"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → INFORME → ARC00100.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → ARCOS → ARC00100.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iarc_busc_arc
<a name="cmxsrv_iarc_busc_arc"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → INFORME → ARC00100.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → ARCOS → ARC00100.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iinf_busc_inf
<a name="cmxsrv_iinf_busc_inf"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → ARCOS → INFO0202.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → ARCOS → ARC00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → INFORME → INFO0103.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iarc_act_arc
<a name="cmxsrv_iarc_act_arc"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → ARCOS → ARC00101.FRM**: [CMXsrv_util_opr_fec](#referencia-cmxsrv_util_opr_fec)
- **Importaciones → ARCOS → INFO0202.FRM**: [PrmACMXMONEDAFEC](#referencia-prmacmxmonedafec)
- **Importaciones → ARCOS → INFO0202.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → ARCOS → INFO0202.FRM**: [CMXsrv_util_opr_fec](#referencia-cmxsrv_util_opr_fec)
- **Importaciones → ARCOS → INFO0202.FRM**: [CMXsrv_cmx_get_codes](#referencia-cmxsrv_cmx_get_codes)
- **Importaciones → ARCOS → ARC00101.FRM**: [PrmACMXMONEDAFEC](#referencia-prmacmxmonedafec)
- **Importaciones → ARCOS → ARC00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → ARCOS → ARC00101.FRM**: [CMXsrv_cmx_get_codes](#referencia-cmxsrv_cmx_get_codes)

---

## CMXsrv_iarc_lee_arc
<a name="cmxsrv_iarc_lee_arc"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → ARCOS → ARC00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iinf_busc_opr
<a name="cmxsrv_iinf_busc_opr"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → ARCOS → INFO0201.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iinf_lee_vlr
<a name="cmxsrv_iinf_lee_vlr"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → ARCOS → INFO0201.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → ARCOS → INFO0201.FRM**: [PrmACMXCLACOM](#referencia-prmacmxclacom)

---

## CMXsrv_iinf_rev_evi
<a name="cmxsrv_iinf_rev_evi"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → INFORME → INFO0105.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → ARCOS → INFO0202.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → ARCOS → INFO0202.FRM**: [CMXsrv_com_rev](#referencia-cmxsrv_com_rev)
- **Importaciones → INFORME → INFO0105.FRM**: [CMXsrv_com_rev](#referencia-cmxsrv_com_rev)

---

## CMXsrv_icob_lee_pln
<a name="cmxsrv_icob_lee_pln"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBERIMP → COB00101.FRM**: [CMXsrv_icob_obs_pln](#referencia-cmxsrv_icob_obs_pln)
- **Importaciones → COBERIMP → COB00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → COBERIMP → COB00101.FRM**: [CMXsrv_cmx_get_codes](#referencia-cmxsrv_cmx_get_codes)

---

## CMXsrv_icob_cur_cob
<a name="cmxsrv_icob_cur_cob"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBERIMP → COB00101.FRM**: [CMXsrv_icob_ctb_reem](#referencia-cmxsrv_icob_ctb_reem)
- **Importaciones → COBERIMP → COB00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → COBERIMP → COB00101.FRM**: [CMXsrv_icob_val_cob](#referencia-cmxsrv_icob_val_cob)

---

## CMXsrv_icob_pag_sop
<a name="cmxsrv_icob_pag_sop"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBERIMP → FORM2.FRM**: [CMXsrv_cmx_get_codes](#referencia-cmxsrv_cmx_get_codes)
- **Importaciones → COBERIMP → COB00101.FRM**: [CMXsrv_icob_ctb_sop](#referencia-cmxsrv_icob_ctb_sop)
- **Importaciones → COBERIMP → COB00307.FRM**: [CMXsrv_val_cta_cte](#referencia-cmxsrv_val_cta_cte)
- **Importaciones → COBERIMP → COB00101.FRM**: [CMXsrv_val_cta_cte](#referencia-cmxsrv_val_cta_cte)
- **Importaciones → COBERIMP → FORM2.FRM**: [CMXsrv_ctb_imp_ddi_so](#referencia-cmxsrv_ctb_imp_ddi_so)
- **Importaciones → COBERIMP → FORM2.FRM**: [CMXsrv_icob_refresh_pos](#referencia-cmxsrv_icob_refresh_pos)
- **Importaciones → COBERIMP → COB00307.FRM**: [CMXsrv_calc_imp_4pct](#referencia-cmxsrv_calc_imp_4pct)
- **Importaciones → COBERIMP → COB00307.FRM**: [CMXsrv_icbr_act_rem](#referencia-cmxsrv_icbr_act_rem)
- **Importaciones → COBERIMP → COB00101.FRM**: [CMXsrv_icbr_act_rem](#referencia-cmxsrv_icbr_act_rem)
- **Importaciones → COBERIMP → COB00307.FRM**: [CMXsrv_get_ult_dia_habil](#referencia-cmxsrv_get_ult_dia_habil)
- **Importaciones → COBERIMP → COB00307.FRM**: [CMXsrv_iddi_marc_ddi2](#referencia-cmxsrv_iddi_marc_ddi2)
- **Importaciones → COBERIMP → COB00101.FRM**: [CMXsrv_calc_imp_4pct](#referencia-cmxsrv_calc_imp_4pct)
- **Importaciones → COBERIMP → COB00307.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → COBERIMP → COB00101.FRM**: [CMXsrv_iddi_marc_ddi2](#referencia-cmxsrv_iddi_marc_ddi2)
- **Importaciones → COBERIMP → COB00101.FRM**: [CMXsrv_get_ult_dia_habil](#referencia-cmxsrv_get_ult_dia_habil)
- **Importaciones → COBERIMP → COB00307.FRM**: [CMXsrv_icob_val_cob](#referencia-cmxsrv_icob_val_cob)
- **Importaciones → COBERIMP → FORM2.FRM**: [CMXsrv_icob_ctb_sop](#referencia-cmxsrv_icob_ctb_sop)
- **Importaciones → COBERIMP → COB00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → COBERIMP → COB00101.FRM**: [CMXsrv_icob_val_cob](#referencia-cmxsrv_icob_val_cob)
- **Importaciones → COBERIMP → COB00307.FRM**: [CMXsrv_cmx_get_codes](#referencia-cmxsrv_cmx_get_codes)
- **Importaciones → COBERIMP → FORM2.FRM**: [CMXsrv_val_cta_cte](#referencia-cmxsrv_val_cta_cte)
- **Importaciones → COBERIMP → COB00101.FRM**: [CMXsrv_cmx_get_codes](#referencia-cmxsrv_cmx_get_codes)
- **Importaciones → COBERIMP → COB00307.FRM**: [CMXsrv_icob_refresh_pos](#referencia-cmxsrv_icob_refresh_pos)
- **Importaciones → COBERIMP → FORM2.FRM**: [CMXsrv_icbr_act_rem](#referencia-cmxsrv_icbr_act_rem)
- **Importaciones → COBERIMP → COB00307.FRM**: [CMXsrv_ctb_imp_ddi_so](#referencia-cmxsrv_ctb_imp_ddi_so)
- **Importaciones → COBERIMP → FORM2.FRM**: [CMXsrv_calc_imp_4pct](#referencia-cmxsrv_calc_imp_4pct)
- **Importaciones → COBERIMP → COB00101.FRM**: [CMXsrv_ctb_imp_ddi_so](#referencia-cmxsrv_ctb_imp_ddi_so)
- **Importaciones → COBERIMP → COB00101.FRM**: [CMXsrv_icob_refresh_pos](#referencia-cmxsrv_icob_refresh_pos)
- **Importaciones → COBERIMP → FORM2.FRM**: [CMXsrv_get_ult_dia_habil](#referencia-cmxsrv_get_ult_dia_habil)
- **Importaciones → COBERIMP → FORM2.FRM**: [CMXsrv_iddi_marc_ddi2](#referencia-cmxsrv_iddi_marc_ddi2)
- **Importaciones → COBERIMP → FORM2.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → COBERIMP → COB00307.FRM**: [CMXsrv_icob_ctb_sop](#referencia-cmxsrv_icob_ctb_sop)
- **Importaciones → COBERIMP → FORM2.FRM**: [CMXsrv_icob_val_cob](#referencia-cmxsrv_icob_val_cob)

---

## CMXsrv_icob_eli_pln
<a name="cmxsrv_icob_eli_pln"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBERIMP → COB00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → COBERIMP → COB00307.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icob_rev_etd
<a name="cmxsrv_icob_rev_etd"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBERIMP → COB00307.FRM**: [CMXsrv_icob_refresh_pos](#referencia-cmxsrv_icob_refresh_pos)
- **Importaciones → COBERIMP → COB00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → COBERIMP → COB00307.FRM**: [CMXsrv_icob_rctb_sop](#referencia-cmxsrv_icob_rctb_sop)
- **Importaciones → COBERIMP → COB00307.FRM**: [CMXsrv_icob_ctb_reem](#referencia-cmxsrv_icob_ctb_reem)
- **Importaciones → COBERIMP → COB00101.FRM**: [CMXsrv_icob_refresh_pos](#referencia-cmxsrv_icob_refresh_pos)
- **Importaciones → COBERIMP → COB00101.FRM**: [CMXsrv_icob_rctb_sop](#referencia-cmxsrv_icob_rctb_sop)
- **Importaciones → COBERIMP → COB00307.FRM**: [CMXsrv_icob_ctb_anu](#referencia-cmxsrv_icob_ctb_anu)
- **Importaciones → COBERIMP → COB00101.FRM**: [CMXsrv_icob_ctb_reem](#referencia-cmxsrv_icob_ctb_reem)
- **Importaciones → COBERIMP → COB00307.FRM**: [CMXsrv_ctl_chq_aprcbl](#referencia-cmxsrv_ctl_chq_aprcbl)
- **Importaciones → COBERIMP → COB00101.FRM**: [CMXsrv_icob_ctb_anu](#referencia-cmxsrv_icob_ctb_anu)
- **Importaciones → COBERIMP → COB00307.FRM**: [CMXsrv_pos_eli_010](#referencia-cmxsrv_pos_eli_010)
- **Importaciones → COBERIMP → COB00307.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → COBERIMP → COB00101.FRM**: [CMXsrv_pos_eli_010](#referencia-cmxsrv_pos_eli_010)
- **Importaciones → COBERIMP → COB00101.FRM**: [CMXsrv_ctl_chq_aprcbl](#referencia-cmxsrv_ctl_chq_aprcbl)

---

## CMXsrv_icob_val_cob
<a name="cmxsrv_icob_val_cob"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBERIMP → COB00101.FRM**: [CMXsrv_util_fecha](#referencia-cmxsrv_util_fecha)
- **Importaciones → COBERIMP → COB00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → COBERIMP → COB00101.FRM**: [CMXsrv_pos_bcx_lee_cob](#referencia-cmxsrv_pos_bcx_lee_cob)
- **Importaciones → COBERIMP → COB00101.FRM**: [PrmACMXPAIS](#referencia-prmacmxpais)

---

## CMXsrv_icob_busc_pln
<a name="cmxsrv_icob_busc_pln"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBERIMP → COB00201.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icob_lee_cln
<a name="cmxsrv_icob_lee_cln"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBERIMP → COB0601.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → COBERIMP → COB00201.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icob_crea_norm
<a name="cmxsrv_icob_crea_norm"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBERIMP → COB00300.FRM**: [CMXsrv_icob_get_num](#referencia-cmxsrv_icob_get_num)
- **Importaciones → COBERIMP → COB00300.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icob_crea_reem
<a name="cmxsrv_icob_crea_reem"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBERIMP → COB00301.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → COBERIMP → COB00301.FRM**: [CMXsrv_pos_bcx_lee_cob](#referencia-cmxsrv_pos_bcx_lee_cob)
- **Importaciones → COBERIMP → COB00301.FRM**: [CMXsrv_icob_get_num](#referencia-cmxsrv_icob_get_num)
- **Importaciones → COBERIMP → COB00301.FRM**: [CMXsrv_pos_bcx_ing_cob](#referencia-cmxsrv_pos_bcx_ing_cob)
- **Importaciones → COBERIMP → COB00301.FRM**: [CMXsrv_cmx_get_codes](#referencia-cmxsrv_cmx_get_codes)

---

## CMXsrv_icob_act_gral
<a name="cmxsrv_icob_act_gral"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBERIMP → COB00302.FRM**: [CMXsrv_icob_val_cob](#referencia-cmxsrv_icob_val_cob)
- **Importaciones → COBERIMP → COB00302.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → COBERIMP → COB00302.FRM**: [CMXsrv_pos_bcx_act_cob](#referencia-cmxsrv_pos_bcx_act_cob)
- **Importaciones → COBERIMP → COB00302.FRM**: [CMXsrv_icob_num_con](#referencia-cmxsrv_icob_num_con)

---

## CMXsrv_icob_lee_cln2
<a name="cmxsrv_icob_lee_cln2"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBERIMP → COB00302.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → COBERIMP → COB00307.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icob_lee_gral
<a name="cmxsrv_icob_lee_gral"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBERIMP → COB00302.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → COBERIMP → COB00302.FRM**: [CMXsrv_pos_bcx_lee_cob](#referencia-cmxsrv_pos_bcx_lee_cob)

---

## CMXsrv_icob_act_val
<a name="cmxsrv_icob_act_val"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → PAGCBR → COB00303.FRM**: [CMXsrv_get_ult_dia_habil](#referencia-cmxsrv_get_ult_dia_habil)
- **Importaciones → COBERIMP → COB00303.FRM**: [CMXsrv_icob_val_cob](#referencia-cmxsrv_icob_val_cob)
- **Importaciones → PAGCBR → COB00303.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → PAGCBR → COB00303.FRM**: [CMXsrv_icob_val_cob](#referencia-cmxsrv_icob_val_cob)
- **Importaciones → COBERIMP → COB00303.FRM**: [CMXsrv_get_ult_dia_habil](#referencia-cmxsrv_get_ult_dia_habil)
- **Importaciones → COBERIMP → COB00303.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icob_lee_val
<a name="cmxsrv_icob_lee_val"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → PAGCBR → COB00303.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → COBERIMP → COB00303.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icob_act_acu
<a name="cmxsrv_icob_act_acu"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBERIMP → COB00304.FRM**: [CMXsrv_icob_val_cob](#referencia-cmxsrv_icob_val_cob)
- **Importaciones → COBERIMP → COB00304.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icob_lee_acu
<a name="cmxsrv_icob_lee_acu"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBERIMP → COB00304.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icob_eli_int
<a name="cmxsrv_icob_eli_int"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBERIMP → COB00305.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icob_busc_int
<a name="cmxsrv_icob_busc_int"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBERIMP → COB00305.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icob_ingmod_int
<a name="cmxsrv_icob_ingmod_int"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBERIMP → COB00306.FRM**: [PrmACMXMONEDA](#referencia-prmacmxmoneda)
- **Importaciones → COBERIMP → COB00306.FRM**: [CMXsrv_icob_val_cob](#referencia-cmxsrv_icob_val_cob)
- **Importaciones → COBERIMP → COB00306.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icob_lee_int
<a name="cmxsrv_icob_lee_int"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBERIMP → COB00306.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icob_ing_mod_srf
<a name="cmxsrv_icob_ing_mod_srf"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBERIMP → COB00307.FRM**: [CMXsrv_pos_bcx_ing_cob](#referencia-cmxsrv_pos_bcx_ing_cob)
- **Importaciones → COBERIMP → COB00307.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → COBERIMP → COB00307.FRM**: [CMXsrv_icob_get_num](#referencia-cmxsrv_icob_get_num)
- **Importaciones → COBERIMP → COB00307.FRM**: [CMXsrv_pos_bcx_act_cob](#referencia-cmxsrv_pos_bcx_act_cob)

---

## CMXsrv_icob_anu
<a name="cmxsrv_icob_anu"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBERIMP → COB00501.FRM**: [CMXsrv_icob_get_num](#referencia-cmxsrv_icob_get_num)
- **Importaciones → COBERIMP → COB00501.FRM**: [CMXsrv_icob_refresh_pos](#referencia-cmxsrv_icob_refresh_pos)
- **Importaciones → COBERIMP → COB00501.FRM**: [CMXsrv_pos_bcx_ing_cob](#referencia-cmxsrv_pos_bcx_ing_cob)
- **Importaciones → COBERIMP → COB00501.FRM**: [CMXsrv_cmx_get_codes](#referencia-cmxsrv_cmx_get_codes)
- **Importaciones → COBERIMP → COB00501.FRM**: [CMXsrv_icob_ctb_anu](#referencia-cmxsrv_icob_ctb_anu)
- **Importaciones → COBERIMP → COB00501.FRM**: [CMXsrv_pos_bcx_act_cob](#referencia-cmxsrv_pos_bcx_act_cob)
- **Importaciones → COBERIMP → COB00501.FRM**: [CMXsrv_get_ult_dia_habil](#referencia-cmxsrv_get_ult_dia_habil)
- **Importaciones → COBERIMP → COB00501.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → COBERIMP → COB00501.FRM**: [CMXsrv_pos_bcx_lee_cob](#referencia-cmxsrv_pos_bcx_lee_cob)

---

## CMXsrv_icob_lee_anu
<a name="cmxsrv_icob_lee_anu"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBERIMP → COB00501.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → COBERIMP → COB00501.FRM**: [CMXsrv_pos_bcx_lee_cob](#referencia-cmxsrv_pos_bcx_lee_cob)

---

## CMXsrv_icob_cur_reem
<a name="cmxsrv_icob_cur_reem"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBERIMP → ORI_DEST.FRM**: [CMXsrv_icob_refresh_pos](#referencia-cmxsrv_icob_refresh_pos)
- **Importaciones → COBERIMP → ORI_DEST.FRM**: [CMXsrv_icob_val_cob](#referencia-cmxsrv_icob_val_cob)
- **Importaciones → COBERIMP → ORI_DEST.FRM**: [CMXsrv_icob_ctb_reem](#referencia-cmxsrv_icob_ctb_reem)
- **Importaciones → COBERIMP → ORI_DEST.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_busc_cor_swf
<a name="cmxsrv_busc_cor_swf"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBRANZA → CBR00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_swf_bus_sms
<a name="cmxsrv_swf_bus_sms"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBRANZA → CBR00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_lee_cbr
<a name="cmxsrv_icbr_lee_cbr"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBRANZA → CBR00101.FRM**: [PrmACMXESPECI](#referencia-prmacmxespeci)
- **Importaciones → COBRANZA → CBR00101.FRM**: [PrmACLNEJECTA](#referencia-prmaclnejecta)
- **Importaciones → COBRANZA → CBR00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_acep_let
<a name="cmxsrv_icbr_acep_let"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBRANZA → CBR00101.FRM**: [CMXsrv_ctl_crea_apr](#referencia-cmxsrv_ctl_crea_apr)
- **Importaciones → COBRANZA → CBR00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_cont_cbr
<a name="cmxsrv_icbr_cont_cbr"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBRANZA → CBR00101.FRM**: [CMXsrv_nibx_upd_tran](#referencia-cmxsrv_nibx_upd_tran)
- **Importaciones → COBRANZA → CBR00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → COBRANZA → CBR00101.FRM**: [CMXsrv_ctb_cbr](#referencia-cmxsrv_ctb_cbr)
- **Importaciones → COBRANZA → CBR00101.FRM**: [CMXsrv_icbr_val_cbr](#referencia-cmxsrv_icbr_val_cbr)
- **Importaciones → COBRANZA → CBR00101.FRM**: [CMXsrv_nibx_nilive](#referencia-cmxsrv_nibx_nilive)
- **Importaciones → COBRANZA → CBR00101.FRM**: [CMXsrv_cnt_gen_vig](#referencia-cmxsrv_cnt_gen_vig)
- **Importaciones → COBRANZA → CBR00101.FRM**: [CMXsrv_mbyte_gen](#referencia-cmxsrv_mbyte_gen)
- **Importaciones → COBRANZA → CBR00101.FRM**: [CMXsrv_ctl_marc_firma](#referencia-cmxsrv_ctl_marc_firma)

---

## CMXsrv_icbr_eli_cbr
<a name="cmxsrv_icbr_eli_cbr"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBRANZA → CBR00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_lee_ctp
<a name="cmxsrv_icbr_lee_ctp"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBRANZA → CBR00201.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → MOD_CBR → CBR00201.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → COBRANZA → CBR00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_avi1
<a name="cmxsrv_icbr_avi1"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBRANZA → CBR00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_busc_cbr
<a name="cmxsrv_icbr_busc_cbr"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBRANZA → CBR00102.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_lee_cln
<a name="cmxsrv_icbr_lee_cln"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → MOD_CBR → CBR00201.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → COBRANZA → CBR00201.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → COBRANZA → CBR00102.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → COBRANZA → CBR00103.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_crea_cbr
<a name="cmxsrv_icbr_crea_cbr"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBRANZA → CBR00103.FRM**: [CMXsrv_util_num_ope](#referencia-cmxsrv_util_num_ope)
- **Importaciones → COBRANZA → CBR00103.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → COBRANZA → CBR00103.FRM**: [srv_icbr_asig_num](#referencia-srv_icbr_asig_num)

---

## CMXsrv_icbr_lee_cob
<a name="cmxsrv_icbr_lee_cob"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBRANZA → CBR00203.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → COBRANZA → CBR00202.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → COBRANZA → CBR00201.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_act_ctp
<a name="cmxsrv_icbr_act_ctp"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → MOD_CBR → CBR00201.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → COBRANZA → CBR00201.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_lee_trm
<a name="cmxsrv_icbr_lee_trm"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → MOD_CBR → CBR00202.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → COBRANZA → CBR00202.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_act_trm
<a name="cmxsrv_icbr_act_trm"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → MOD_CBR → CBR00202.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → COBRANZA → CBR00202.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → MOD_CBR → CBR00202.FRM**: [CMXsrv_util_fecha](#referencia-cmxsrv_util_fecha)
- **Importaciones → MOD_CBR → CBR00202.FRM**: [CMXsrv_icbr_val_cbr](#referencia-cmxsrv_icbr_val_cbr)
- **Importaciones → COBRANZA → CBR00202.FRM**: [CMXsrv_icbr_val_cbr](#referencia-cmxsrv_icbr_val_cbr)
- **Importaciones → COBRANZA → CBR00202.FRM**: [CMXsrv_util_fecha](#referencia-cmxsrv_util_fecha)

---

## CMXsrv_icbr_lee_doc
<a name="cmxsrv_icbr_lee_doc"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → MOD_CBR → CBR00203.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → COBRANZA → CBR00203.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_act_doc
<a name="cmxsrv_icbr_act_doc"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → MOD_CBR → CBR00203.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → COBRANZA → CBR00203.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_busc_let
<a name="cmxsrv_icbr_busc_let"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBRANZA → CBR00301.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → MOD_CBR → CBR00301.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_ingmod_let
<a name="cmxsrv_icbr_ingmod_let"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBRANZA → CBR00302.FRM**: [CMXsrv_util_fecha](#referencia-cmxsrv_util_fecha)
- **Importaciones → COBRANZA → CBR00302.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_eli_let
<a name="cmxsrv_icbr_eli_let"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → MOD_CBR → CBR00302.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → COBRANZA → CBR00302.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_lee_let
<a name="cmxsrv_icbr_lee_let"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → MOD_CBR → CBR00302.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → COBRANZA → CBR00302.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_prorr
<a name="cmxsrv_icbr_prorr"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBRANZA → CBR00305.FRM**: [CMXsrv_cnt_2600](#referencia-cmxsrv_cnt_2600)
- **Importaciones → COBRANZA → CBR00305.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → COBRANZA → CBR00305.FRM**: [CMXsrv_cnt_2620](#referencia-cmxsrv_cnt_2620)
- **Importaciones → COBRANZA → CBR00305.FRM**: [CMXsrv_cnt_2610](#referencia-cmxsrv_cnt_2610)
- **Importaciones → COBRANZA → CBR00305.FRM**: [CMXsrv_util_fecha](#referencia-cmxsrv_util_fecha)

---

## CMXsrv_icbr_rev_eve
<a name="cmxsrv_icbr_rev_eve"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBRANZA → CBR00401.FRM**: [CMXsrv_rctb_rem](#referencia-cmxsrv_rctb_rem)
- **Importaciones → COBRANZA → CBR00401.FRM**: [CMXsrv_icbr_rev_trfo](#referencia-cmxsrv_icbr_rev_trfo)
- **Importaciones → COBRANZA → CBR00401.FRM**: [CMXsrv_icbr_rev_vis](#referencia-cmxsrv_icbr_rev_vis)
- **Importaciones → COBRANZA → CBR00401.FRM**: [CMXsrv_cnt_rev_vig](#referencia-cmxsrv_cnt_rev_vig)
- **Importaciones → COBRANZA → CBR00401.FRM**: [CMXsrv_icbr_rev_acep](#referencia-cmxsrv_icbr_rev_acep)
- **Importaciones → COBRANZA → CBR00401.FRM**: [CMXsrv_com_rev](#referencia-cmxsrv_com_rev)
- **Importaciones → COBRANZA → CBR00401.FRM**: [CMXsrv_icbr_rev_liq](#referencia-cmxsrv_icbr_rev_liq)
- **Importaciones → COBRANZA → CBR00401.FRM**: [CMXsrv_icbr_rev_ent](#referencia-cmxsrv_icbr_rev_ent)
- **Importaciones → COBRANZA → CBR00401.FRM**: [CMXsrv_icbr_rev_prorr](#referencia-cmxsrv_icbr_rev_prorr)
- **Importaciones → COBRANZA → CBR00401.FRM**: [CMXsrv_icbr_rev_trfb](#referencia-cmxsrv_icbr_rev_trfb)
- **Importaciones → COBRANZA → CBR00401.FRM**: [CMXsrv_mbyte_gen](#referencia-cmxsrv_mbyte_gen)
- **Importaciones → COBRANZA → CBR00401.FRM**: [sp_cmx_sii_1870](#referencia-sp_cmx_sii_1870)
- **Importaciones → COBRANZA → CBR00401.FRM**: [CMXsrv_ctl_marc_rev](#referencia-cmxsrv_ctl_marc_rev)
- **Importaciones → COBRANZA → CBR00401.FRM**: [CMXsrv_icbr_rev_pag](#referencia-cmxsrv_icbr_rev_pag)
- **Importaciones → COBRANZA → CBR00401.FRM**: [CMXsrv_ctl_chq_aprcbl](#referencia-cmxsrv_ctl_chq_aprcbl)
- **Importaciones → COBRANZA → CBR00401.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → COBRANZA → CBR00401.FRM**: [CMXsrv_icbr_rev_prot](#referencia-cmxsrv_icbr_rev_prot)
- **Importaciones → COBRANZA → CBR00401.FRM**: [CMXsrv_ctl_eli_firma](#referencia-cmxsrv_ctl_eli_firma)
- **Importaciones → COBRANZA → CBR00401.FRM**: [CMXsrv_icbr_rev_inst](#referencia-cmxsrv_icbr_rev_inst)
- **Importaciones → COBRANZA → CBR00401.FRM**: [CMXsrv_icbr_rev_mod_cbr](#referencia-cmxsrv_icbr_rev_mod_cbr)
- **Importaciones → COBRANZA → CBR00401.FRM**: [CMXsrv_icbr_rev_ing](#referencia-cmxsrv_icbr_rev_ing)

---

## CMXsrv_icbr_busc_eve
<a name="cmxsrv_icbr_busc_eve"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBRANZA → CBR00401.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_lee_eve
<a name="cmxsrv_icbr_lee_eve"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBRANZA → CBR00402.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_lee_ent_doc
<a name="cmxsrv_icbr_lee_ent_doc"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBRANZA → CBR00402.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → COBRANZA → CBR00804.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_prot
<a name="cmxsrv_icbr_prot"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBRANZA → CBR00701.FRM**: [CMXsrv_ctl_crea_apr](#referencia-cmxsrv_ctl_crea_apr)
- **Importaciones → COBRANZA → CBR00701.FRM**: [CMXsrv_cnt_950](#referencia-cmxsrv_cnt_950)
- **Importaciones → COBRANZA → CBR00701.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_pcg_prot
<a name="cmxsrv_icbr_pcg_prot"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBRANZA → CBR00701.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_liq_sdo
<a name="cmxsrv_icbr_liq_sdo"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBRANZA → CBR00801.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → COBRANZA → CBR00801.FRM**: [CMXsrv_ctb_liq_sdo](#referencia-cmxsrv_ctb_liq_sdo)
- **Importaciones → COBRANZA → CBR00801.FRM**: [CMXsrv_cnt_gen_vig](#referencia-cmxsrv_cnt_gen_vig)

---

## CMXsrv_icbr_act_vis
<a name="cmxsrv_icbr_act_vis"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBRANZA → CBR00802.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_eli_rep
<a name="cmxsrv_icbr_eli_rep"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBRANZA → CBR00802.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_busc_rep
<a name="cmxsrv_icbr_busc_rep"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBRANZA → CBR00802.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_imod_rep
<a name="cmxsrv_icbr_imod_rep"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBRANZA → CBR00803.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_ent_doc
<a name="cmxsrv_icbr_ent_doc"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBRANZA → CBR00804.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → COBRANZA → CBR00804.FRM**: [CMXsrv_ctl_crea_apr](#referencia-cmxsrv_ctl_crea_apr)

---

## CMXsrv_icbr_trf_ofi
<a name="cmxsrv_icbr_trf_ofi"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBRANZA → CBR00901.FRM**: [CMXsrv_ctb_trfo](#referencia-cmxsrv_ctb_trfo)
- **Importaciones → COBRANZA → CBR00901.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_trf_bco
<a name="cmxsrv_icbr_trf_bco"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBRANZA → CBR00902.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → COBRANZA → CBR00902.FRM**: [CMXsrv_ctb_trfb](#referencia-cmxsrv_ctb_trfb)

---

## CMXsrv_icbr_act_inst
<a name="cmxsrv_icbr_act_inst"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBRANZA → COBERTU.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iswf_a_pru
<a name="cmxsrv_iswf_a_pru"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBRANZA → GRL00101.FRM**: [CMXsrv_iswf_esp_707b](#referencia-cmxsrv_iswf_esp_707b)
- **Importaciones → NNEGO → GRL00101.FRM**: [CMXsrv_iswf_a_707a](#referencia-cmxsrv_iswf_a_707a)
- **Importaciones → NNEGO → GRL00101.FRM**: [CMXsrv_iswf_a_700b](#referencia-cmxsrv_iswf_a_700b)
- **Importaciones → IMPORT → GRL00101.FRM**: [CMXsrv_iswf_a_410](#referencia-cmxsrv_iswf_a_410)
- **Importaciones → NNEGO → GRL00101.FRM**: [CMXsrv_iswf_a_412](#referencia-cmxsrv_iswf_a_412)
- **Importaciones → NNEGO → GRL00101.FRM**: [CMXsrv_iswf_a_732](#referencia-cmxsrv_iswf_a_732)
- **Importaciones → IMPORT → GRL00101.FRM**: [CMXsrv_iswf_a_740](#referencia-cmxsrv_iswf_a_740)
- **Importaciones → COBRANZA → GRL00101.FRM**: [CMXsrv_iswf_a_700a](#referencia-cmxsrv_iswf_a_700a)
- **Importaciones → NNEGO → CRD01001.FRM**: [CMXsrv_iswf_a_707a](#referencia-cmxsrv_iswf_a_707a)
- **Importaciones → NNEGO → CRD01001.FRM**: [CMXsrv_iswf_a_700b](#referencia-cmxsrv_iswf_a_700b)
- **Importaciones → NNEGO → GRL00101.FRM**: [CMXsrv_iswf_esp_707a](#referencia-cmxsrv_iswf_esp_707a)
- **Importaciones → COBRANZA → GRL00101.FRM**: [CMXsrv_iswf_a_747](#referencia-cmxsrv_iswf_a_747)
- **Importaciones → COBRANZA → GRL00101.FRM**: [CMXsrv_iswf_a_410](#referencia-cmxsrv_iswf_a_410)
- **Importaciones → COBRANZA → GRL00101.FRM**: [CMXsrv_iswf_a_740](#referencia-cmxsrv_iswf_a_740)
- **Importaciones → IMPORT → GRL00101.FRM**: [CMXsrv_iswf_esp_700a](#referencia-cmxsrv_iswf_esp_700a)
- **Importaciones → NNEGO → CRD01001.FRM**: [CMXsrv_iswf_a_412](#referencia-cmxsrv_iswf_a_412)
- **Importaciones → IMPORT → GRL00101.FRM**: [CMXsrv_iswf_esp_700b](#referencia-cmxsrv_iswf_esp_700b)
- **Importaciones → COBRANZA → GRL00101.FRM**: [CMXsrv_iswf_esp_747](#referencia-cmxsrv_iswf_esp_747)
- **Importaciones → IMPORT → GRL00101.FRM**: [CMXsrv_iswf_747_neg](#referencia-cmxsrv_iswf_747_neg)
- **Importaciones → NNEGO → CRD01001.FRM**: [srv_irem_imp_100](#referencia-srv_irem_imp_100)
- **Importaciones → NNEGO → CRD01001.FRM**: [CMXsrv_iswf_esp_707b](#referencia-cmxsrv_iswf_esp_707b)
- **Importaciones → NNEGO → GRL00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → NNEGO → CRD01001.FRM**: [CMXsrv_iswf_esp_707a](#referencia-cmxsrv_iswf_esp_707a)
- **Importaciones → NNEGO → GRL00101.FRM**: [CMXsrv_iswf_neg_752](#referencia-cmxsrv_iswf_neg_752)
- **Importaciones → NNEGO → GRL00101.FRM**: [CMXsrv_iswf_a_747](#referencia-cmxsrv_iswf_a_747)
- **Importaciones → COBRANZA → GRL00101.FRM**: [CMXsrv_iswf_esp_700a](#referencia-cmxsrv_iswf_esp_700a)
- **Importaciones → IMPORT → CRD00101.FRM**: [CMXsrv_iswf_esp_700a](#referencia-cmxsrv_iswf_esp_700a)
- **Importaciones → IMPORT → GRL00101.FRM**: [CMXsrv_iswf_esp_740](#referencia-cmxsrv_iswf_esp_740)
- **Importaciones → IMPORT → CRD00101.FRM**: [CMXsrv_iswf_esp_700b](#referencia-cmxsrv_iswf_esp_700b)
- **Importaciones → IMPORT → CRD00101.FRM**: [CMXsrv_iswf_747_neg](#referencia-cmxsrv_iswf_747_neg)
- **Importaciones → NNEGO → GRL00101.FRM**: [CMXsrv_iswf_esp_747](#referencia-cmxsrv_iswf_esp_747)
- **Importaciones → NNEGO → CRD01001.FRM**: [CMXsrv_iswf_a_700a](#referencia-cmxsrv_iswf_a_700a)
- **Importaciones → NNEGO → CRD01001.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → NNEGO → CRD01001.FRM**: [CMXsrv_iswf_neg_752](#referencia-cmxsrv_iswf_neg_752)
- **Importaciones → NNEGO → CRD01001.FRM**: [CMXsrv_iswf_a_747](#referencia-cmxsrv_iswf_a_747)
- **Importaciones → NNEGO → GRL00101.FRM**: [CMXsrv_iswf_neg_730](#referencia-cmxsrv_iswf_neg_730)
- **Importaciones → IMPORT → CRD00101.FRM**: [CMXsrv_iswf_esp_740](#referencia-cmxsrv_iswf_esp_740)
- **Importaciones → NNEGO → CRD01001.FRM**: [CMXsrv_iswf_esp_747](#referencia-cmxsrv_iswf_esp_747)
- **Importaciones → NNEGO → GRL00101.FRM**: [srv_irem_imp_100](#referencia-srv_irem_imp_100)
- **Importaciones → NNEGO → GRL00101.FRM**: [CMXsrv_iswf_esp_707b](#referencia-cmxsrv_iswf_esp_707b)
- **Importaciones → IMPORT → GRL00101.FRM**: [CMXsrv_iswf_a_732](#referencia-cmxsrv_iswf_a_732)
- **Importaciones → IMPORT → GRL00101.FRM**: [srv_irem_imp_202](#referencia-srv_irem_imp_202)
- **Importaciones → NNEGO → CRD01001.FRM**: [CMXsrv_iswf_neg_730](#referencia-cmxsrv_iswf_neg_730)
- **Importaciones → IMPORT → GRL00101.FRM**: [CMXsrv_iswf_a_707b](#referencia-cmxsrv_iswf_a_707b)
- **Importaciones → NNEGO → GRL00101.FRM**: [CMXsrv_iswf_a_700a](#referencia-cmxsrv_iswf_a_700a)
- **Importaciones → IMPORT → CRD00101.FRM**: [CMXsrv_iswf_a_732](#referencia-cmxsrv_iswf_a_732)
- **Importaciones → IMPORT → CRD00101.FRM**: [srv_irem_imp_202](#referencia-srv_irem_imp_202)
- **Importaciones → NNEGO → GRL00101.FRM**: [CMXsrv_iswf_a_410](#referencia-cmxsrv_iswf_a_410)
- **Importaciones → COBRANZA → GRL00101.FRM**: [CMXsrv_iswf_esp_700b](#referencia-cmxsrv_iswf_esp_700b)
- **Importaciones → COBRANZA → GRL00101.FRM**: [CMXsrv_iswf_747_neg](#referencia-cmxsrv_iswf_747_neg)
- **Importaciones → IMPORT → CRD00101.FRM**: [CMXsrv_iswf_esp_707a](#referencia-cmxsrv_iswf_esp_707a)
- **Importaciones → NNEGO → GRL00101.FRM**: [CMXsrv_iswf_a_740](#referencia-cmxsrv_iswf_a_740)
- **Importaciones → IMPORT → CRD00101.FRM**: [CMXsrv_iswf_a_707b](#referencia-cmxsrv_iswf_a_707b)
- **Importaciones → COBRANZA → GRL00101.FRM**: [CMXsrv_iswf_esp_740](#referencia-cmxsrv_iswf_esp_740)
- **Importaciones → NNEGO → CRD01001.FRM**: [CMXsrv_iswf_a_410](#referencia-cmxsrv_iswf_a_410)
- **Importaciones → NNEGO → GRL00101.FRM**: [CMXsrv_iswf_esp_700a](#referencia-cmxsrv_iswf_esp_700a)
- **Importaciones → NNEGO → GRL00101.FRM**: [CMXsrv_iswf_esp_700b](#referencia-cmxsrv_iswf_esp_700b)
- **Importaciones → IMPORT → CRD00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → NNEGO → GRL00101.FRM**: [CMXsrv_iswf_747_neg](#referencia-cmxsrv_iswf_747_neg)
- **Importaciones → IMPORT → GRL00101.FRM**: [CMXsrv_iswf_a_707a](#referencia-cmxsrv_iswf_a_707a)
- **Importaciones → IMPORT → GRL00101.FRM**: [CMXsrv_iswf_a_700b](#referencia-cmxsrv_iswf_a_700b)
- **Importaciones → NNEGO → CRD01001.FRM**: [CMXsrv_iswf_a_740](#referencia-cmxsrv_iswf_a_740)
- **Importaciones → IMPORT → CRD00101.FRM**: [CMXsrv_iswf_neg_752](#referencia-cmxsrv_iswf_neg_752)
- **Importaciones → IMPORT → GRL00101.FRM**: [CMXsrv_iswf_a_412](#referencia-cmxsrv_iswf_a_412)
- **Importaciones → IMPORT → GRL00101.FRM**: [srv_irem_imp_100](#referencia-srv_irem_imp_100)
- **Importaciones → NNEGO → CRD01001.FRM**: [CMXsrv_iswf_esp_700a](#referencia-cmxsrv_iswf_esp_700a)
- **Importaciones → NNEGO → CRD01001.FRM**: [CMXsrv_iswf_esp_700b](#referencia-cmxsrv_iswf_esp_700b)
- **Importaciones → IMPORT → GRL00101.FRM**: [CMXsrv_iswf_esp_707b](#referencia-cmxsrv_iswf_esp_707b)
- **Importaciones → IMPORT → CRD00101.FRM**: [CMXsrv_iswf_a_707a](#referencia-cmxsrv_iswf_a_707a)
- **Importaciones → IMPORT → CRD00101.FRM**: [CMXsrv_iswf_a_700b](#referencia-cmxsrv_iswf_a_700b)
- **Importaciones → NNEGO → CRD01001.FRM**: [CMXsrv_iswf_747_neg](#referencia-cmxsrv_iswf_747_neg)
- **Importaciones → IMPORT → GRL00101.FRM**: [CMXsrv_iswf_esp_707a](#referencia-cmxsrv_iswf_esp_707a)
- **Importaciones → COBRANZA → GRL00101.FRM**: [CMXsrv_iswf_a_732](#referencia-cmxsrv_iswf_a_732)
- **Importaciones → COBRANZA → GRL00101.FRM**: [srv_irem_imp_202](#referencia-srv_irem_imp_202)
- **Importaciones → IMPORT → CRD00101.FRM**: [CMXsrv_iswf_a_412](#referencia-cmxsrv_iswf_a_412)
- **Importaciones → IMPORT → CRD00101.FRM**: [srv_irem_imp_100](#referencia-srv_irem_imp_100)
- **Importaciones → NNEGO → CRD01001.FRM**: [CMXsrv_iswf_esp_740](#referencia-cmxsrv_iswf_esp_740)
- **Importaciones → COBRANZA → GRL00101.FRM**: [CMXsrv_iswf_esp_707a](#referencia-cmxsrv_iswf_esp_707a)
- **Importaciones → IMPORT → CRD00101.FRM**: [CMXsrv_iswf_esp_707b](#referencia-cmxsrv_iswf_esp_707b)
- **Importaciones → COBRANZA → GRL00101.FRM**: [CMXsrv_iswf_a_707b](#referencia-cmxsrv_iswf_a_707b)
- **Importaciones → IMPORT → GRL00101.FRM**: [CMXsrv_iswf_a_700a](#referencia-cmxsrv_iswf_a_700a)
- **Importaciones → IMPORT → GRL00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → IMPORT → GRL00101.FRM**: [CMXsrv_iswf_neg_752](#referencia-cmxsrv_iswf_neg_752)
- **Importaciones → IMPORT → GRL00101.FRM**: [CMXsrv_iswf_a_747](#referencia-cmxsrv_iswf_a_747)
- **Importaciones → NNEGO → GRL00101.FRM**: [srv_irem_imp_202](#referencia-srv_irem_imp_202)
- **Importaciones → COBRANZA → GRL00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → IMPORT → GRL00101.FRM**: [CMXsrv_iswf_esp_747](#referencia-cmxsrv_iswf_esp_747)
- **Importaciones → COBRANZA → GRL00101.FRM**: [CMXsrv_iswf_neg_752](#referencia-cmxsrv_iswf_neg_752)
- **Importaciones → IMPORT → CRD00101.FRM**: [CMXsrv_iswf_a_700a](#referencia-cmxsrv_iswf_a_700a)
- **Importaciones → NNEGO → GRL00101.FRM**: [CMXsrv_iswf_a_707b](#referencia-cmxsrv_iswf_a_707b)
- **Importaciones → IMPORT → CRD00101.FRM**: [CMXsrv_iswf_a_747](#referencia-cmxsrv_iswf_a_747)
- **Importaciones → IMPORT → CRD00101.FRM**: [CMXsrv_iswf_a_410](#referencia-cmxsrv_iswf_a_410)
- **Importaciones → IMPORT → GRL00101.FRM**: [CMXsrv_iswf_neg_730](#referencia-cmxsrv_iswf_neg_730)
- **Importaciones → NNEGO → CRD01001.FRM**: [CMXsrv_iswf_a_732](#referencia-cmxsrv_iswf_a_732)
- **Importaciones → IMPORT → CRD00101.FRM**: [CMXsrv_iswf_a_740](#referencia-cmxsrv_iswf_a_740)
- **Importaciones → NNEGO → CRD01001.FRM**: [srv_irem_imp_202](#referencia-srv_irem_imp_202)
- **Importaciones → IMPORT → CRD00101.FRM**: [CMXsrv_iswf_esp_747](#referencia-cmxsrv_iswf_esp_747)
- **Importaciones → COBRANZA → GRL00101.FRM**: [CMXsrv_iswf_a_707a](#referencia-cmxsrv_iswf_a_707a)
- **Importaciones → COBRANZA → GRL00101.FRM**: [CMXsrv_iswf_a_700b](#referencia-cmxsrv_iswf_a_700b)
- **Importaciones → NNEGO → GRL00101.FRM**: [CMXsrv_iswf_esp_740](#referencia-cmxsrv_iswf_esp_740)
- **Importaciones → NNEGO → CRD01001.FRM**: [CMXsrv_iswf_a_707b](#referencia-cmxsrv_iswf_a_707b)
- **Importaciones → COBRANZA → GRL00101.FRM**: [CMXsrv_iswf_neg_730](#referencia-cmxsrv_iswf_neg_730)
- **Importaciones → IMPORT → CRD00101.FRM**: [CMXsrv_iswf_neg_730](#referencia-cmxsrv_iswf_neg_730)
- **Importaciones → COBRANZA → GRL00101.FRM**: [CMXsrv_iswf_a_412](#referencia-cmxsrv_iswf_a_412)
- **Importaciones → COBRANZA → GRL00101.FRM**: [srv_irem_imp_100](#referencia-srv_irem_imp_100)

---

## CMXsrv_icbr_val_cbr
<a name="cmxsrv_icbr_val_cbr"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → COBRANZA → GRL00101.FRM**: [PrmACMXPAIS](#referencia-prmacmxpais)
- **Importaciones → COBRANZA → GRL00101.FRM**: [CMXsrv_icbr_val_arc](#referencia-cmxsrv_icbr_val_arc)
- **Importaciones → COBRANZA → GRL00101.FRM**: [PrmACMXMONEDAFEC](#referencia-prmacmxmonedafec)
- **Importaciones → COBRANZA → GRL00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → COBRANZA → GRL00101.FRM**: [CMXsrv_util_fecha](#referencia-cmxsrv_util_fecha)

---

## CMXsrv_icrd_a_ibab
<a name="cmxsrv_icrd_a_ibab"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → MOD_CRD → BCO_BCO.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → CRDEXT → BCO_BCO.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_glo_ibab
<a name="cmxsrv_icrd_lee_glo_ibab"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → CRDEXT → BCO_BCO.FRM**: [CMXsrv_icrd_pre_78](#referencia-cmxsrv_icrd_pre_78)
- **Importaciones → MOD_CRD → BCO_BCO.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → CRDEXT → BCO_BCO.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → MOD_CRD → BCO_BCO.FRM**: [CMXsrv_icrd_pre_78](#referencia-cmxsrv_icrd_pre_78)

---

## CMXsrv_icrd_a_ibar
<a name="cmxsrv_icrd_a_ibar"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → MOD_CRD → BCO_REM.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → CRDEXT → BCO_REM.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_glo_ibar
<a name="cmxsrv_icrd_lee_glo_ibar"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → MOD_CRD → BCO_REM.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → CRDEXT → BCO_REM.FRM**: [CMXsrv_icrd_pre_72_740](#referencia-cmxsrv_icrd_pre_72_740)
- **Importaciones → MOD_CRD → BCO_REM.FRM**: [CMXsrv_icrd_pre_72_740](#referencia-cmxsrv_icrd_pre_72_740)
- **Importaciones → CRDEXT → BCO_REM.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_tex_swf
<a name="cmxsrv_icrd_lee_tex_swf"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → CRDEXT → BUSC_TXT.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → IMPORT → BUSC_COD.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → MOD_CRD → BUSC_TXT.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → MOD_CRD → BUSCA_TE.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → IMPORT → BUSC_TXT.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → CRDEXT → BUSC_COD.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → MOD_CRD → BUSC_COD.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_cod_txt_swf
<a name="cmxsrv_icrd_lee_cod_txt_swf"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → CRDEXT → BUSC_TXT.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → MOD_CRD → BUSC_TXT.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → IMPORT → BUSC_TXT.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_txt_swf_all
<a name="cmxsrv_icrd_lee_txt_swf_all"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → CRDEXT → BUSC_TXT.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → MOD_CRD → BUSC_TXT.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → IMPORT → BUSC_TXT.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_ind_esp_ing
<a name="cmxsrv_icrd_lee_ind_esp_ing"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → CRDEXT → BUSC_TXT.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → MOD_CRD → BUSC_TXT.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → MOD_CRD → MOD00603.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → IMPORT → BUSC_TXT.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → IMPORT → CRD00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_ing_acu
<a name="cmxsrv_icrd_ing_acu"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → CRDEXT → CRD00207.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_acu
<a name="cmxsrv_icrd_lee_acu"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → CRDEXT → CRD00207.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_rech_sol
<a name="cmxsrv_icrd_rech_sol"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → CRDEXT → CRD00701.FRM**: [CMXsrv_nibx_nilive](#referencia-cmxsrv_nibx_nilive)
- **Importaciones → IMPORT → CRD00701.FRM**: [CMXsrv_ctl_crea_apr](#referencia-cmxsrv_ctl_crea_apr)
- **Importaciones → CRDEXT → CRD00701.FRM**: [CMXsrv_ctl_crea_apr](#referencia-cmxsrv_ctl_crea_apr)
- **Importaciones → IMPORT → CRD00701.FRM**: [CMXsrv_nibx_upd_tran](#referencia-cmxsrv_nibx_upd_tran)
- **Importaciones → CRDEXT → CRD00701.FRM**: [CMXsrv_nibx_upd_tran](#referencia-cmxsrv_nibx_upd_tran)
- **Importaciones → CRDEXT → CRD00701.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → IMPORT → CRD00701.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → IMPORT → CRD00701.FRM**: [CMXsrv_nibx_nilive](#referencia-cmxsrv_nibx_nilive)

---

## CMXsrv_icrd_end
<a name="cmxsrv_icrd_end"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → CRDEXT → CRD00801.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → CRDEXT → CRD00801.FRM**: [CMXsrv_ctl_crea_apr](#referencia-cmxsrv_ctl_crea_apr)

---

## CMXsrv_icrd_lee_dat_end
<a name="cmxsrv_icrd_lee_dat_end"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → CRDEXT → CRD00801.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_asignar_cor
<a name="cmxsrv_icrd_asignar_cor"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → CRDEXT → CRD02001.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → CRD_CORR → COR00202.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_bco_mtr
<a name="cmxsrv_icrd_lee_bco_mtr"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → CRD_CORR → COR00202.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_cor_lee_pais
<a name="cmxsrv_icrd_cor_lee_pais"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → CRD_CORR → COR00202.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_plz
<a name="cmxsrv_icrd_lee_plz"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → CRD_CORR → COR00202.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_busc_plz
<a name="cmxsrv_icrd_busc_plz"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → CRD_CORR → COR00906.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_cor_busc_pais
<a name="cmxsrv_icrd_cor_busc_pais"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → CRD_CORR → COR00907.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_busc_bco_mtr
<a name="cmxsrv_icrd_busc_bco_mtr"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → CRD_CORR → GRID_BUS.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iddi_ingmod_ddi
<a name="cmxsrv_iddi_ingmod_ddi"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → DDI → DDI00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iddi_lee_dec
<a name="cmxsrv_iddi_lee_dec"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → DDI → DDI00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → DDI → DDI00101.FRM**: [CMXsrv_iddi_val_num_ddi](#referencia-cmxsrv_iddi_val_num_ddi)

---

## CMXsrv_iddi_eli_ddi
<a name="cmxsrv_iddi_eli_ddi"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → DDI → DDI00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iddi_lee_inf
<a name="cmxsrv_iddi_lee_inf"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → DDI → DDI00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iddi_lee_cln
<a name="cmxsrv_iddi_lee_cln"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → DDI → DDI01001.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → DDI → DDI00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iddi_lee_rut
<a name="cmxsrv_iddi_lee_rut"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → DDI → DDI01001.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iddi_asoc_ddi
<a name="cmxsrv_iddi_asoc_ddi"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → DDI → DDI01001.FRM**: [CMXsrv_get_ult_dia_habil](#referencia-cmxsrv_get_ult_dia_habil)
- **Importaciones → DDI → DDI01001.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → DDI → DDI01001.FRM**: [CMXsrv_cmx_get_codes](#referencia-cmxsrv_cmx_get_codes)
- **Importaciones → DDI → DDI01001.FRM**: [CMXsrv_util_opr_fec](#referencia-cmxsrv_util_opr_fec)

---

## CMXsrv_iddi_des_ddi
<a name="cmxsrv_iddi_des_ddi"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → DDI → DDI01001.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iddi_busc_asoc
<a name="cmxsrv_iddi_busc_asoc"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → DDI → DDI01001.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iddi_busc_noasoc
<a name="cmxsrv_iddi_busc_noasoc"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → DDI → DDI01001.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → DDI → DDI01001.FRM**: [CMXsrv_iddi_bus_noasoc_cob](#referencia-cmxsrv_iddi_bus_noasoc_cob)
- **Importaciones → DDI → DDI01001.FRM**: [CMXsrv_iddi_bus_noasoc_opr](#referencia-cmxsrv_iddi_bus_noasoc_opr)

---

## CMXsrv_icrd_lee_dir_cln
<a name="cmxsrv_icrd_lee_dir_cln"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → IMPORT → BUSCADIR.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → MOD_CRD → BUSCADIR.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXCRDsrv_icrd_a_cnd_esp
<a name="cmxcrdsrv_icrd_a_cnd_esp"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → IMPORT → CONDESP.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_cnd_esp
<a name="cmxsrv_icrd_lee_cnd_esp"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → NNEGO → CRD01005.FRM**: [CMXsrv_icrd_pre_47](#referencia-cmxsrv_icrd_pre_47)
- **Importaciones → IMPORT → CONDESP.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → MOD_CRD → CONDESP.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → MOD_CRD → CONDESP.FRM**: [CMXsrv_icrd_pre_47](#referencia-cmxsrv_icrd_pre_47)
- **Importaciones → NNEGO → CRD01005.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → IMPORT → CONDESP.FRM**: [CMXsrv_icrd_pre_47](#referencia-cmxsrv_icrd_pre_47)

---

## CMXCRDsrv_icrd_clon_crd
<a name="cmxcrdsrv_icrd_clon_crd"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → IMPORT → CRD00101.FRM**: [CMXsrv_util_num_ope](#referencia-cmxsrv_util_num_ope)
- **Importaciones → IMPORT → CRD00101.FRM**: [CMXCRDsrv_icrd_lee_tas_cln](#referencia-cmxcrdsrv_icrd_lee_tas_cln)
- **Importaciones → IMPORT → CRD00101.FRM**: [CMXsrv_fincol_ing_modcol](#referencia-cmxsrv_fincol_ing_modcol)
- **Importaciones → IMPORT → CRD00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXCRDsrv_icrd_lee_crdcre
<a name="cmxcrdsrv_icrd_lee_crdcre"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → IMPORT → CRD00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_top
<a name="cmxsrv_icrd_lee_top"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → IMPORT → CRD00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXCRDsrv_icrd_val_crd
<a name="cmxcrdsrv_icrd_val_crd"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → IMPORT → CRD00101.FRM**: [CMXsrv_icrd_val_adv](#referencia-cmxsrv_icrd_val_adv)
- **Importaciones → IMPORT → CRD00101.FRM**: [CMXsrv_icrd_val_err](#referencia-cmxsrv_icrd_val_err)
- **Importaciones → IMPORT → CRD00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXCRDsrv_icrd_eli_crd
<a name="cmxcrdsrv_icrd_eli_crd"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → IMPORT → CRD00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_dat_trs
<a name="cmxsrv_icrd_lee_dat_trs"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → NEGO_AV → AVISOS.FRM**: [CMXsrv_icrd_forlin](#referencia-cmxsrv_icrd_forlin)
- **Importaciones → NEGO_AV → CRD01001.FRM**: [CMXsrv_icrd_forlin](#referencia-cmxsrv_icrd_forlin)
- **Importaciones → INFORME → INFO0101.FRM**: [CMXsrv_icrd_forlin](#referencia-cmxsrv_icrd_forlin)
- **Importaciones → IMPORT → CRD00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → NEGO_AV → AVISOS.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → IMPORT → CRD00101.FRM**: [CMXsrv_icrd_forlin](#referencia-cmxsrv_icrd_forlin)
- **Importaciones → NEGO_AV → CRD01001.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → INFORME → INFO0101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_a_ctp
<a name="cmxsrv_icrd_a_ctp"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → MOD_CRD → CRD00201.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → IMPORT → CRD00201.FRM**: [CMXsrv_fincol_imod_colcc](#referencia-cmxsrv_fincol_imod_colcc)
- **Importaciones → MOD_CRD → CRD00201.FRM**: [CMXCRDsrv_icrd_lee_tas_cln](#referencia-cmxcrdsrv_icrd_lee_tas_cln)
- **Importaciones → IMPORT → CRD00201.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → MOD_CRD → CRD00201.FRM**: [CMXsrv_fincol_imod_colcc](#referencia-cmxsrv_fincol_imod_colcc)
- **Importaciones → IMPORT → CRD00201.FRM**: [CMXCRDsrv_icrd_lee_tas_cln](#referencia-cmxcrdsrv_icrd_lee_tas_cln)

---

## CMXsrv_icrd_lee_cln
<a name="cmxsrv_icrd_lee_cln"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → IMPORT → CRD00201.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → IMPORT → CRD00301.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → MOD_CRD → CRD00201.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_a_cnd
<a name="cmxsrv_icrd_a_cnd"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → IMPORT → CRD00202.FRM**: [CMXsrv_icrd_a_dat_apr](#referencia-cmxsrv_icrd_a_dat_apr)
- **Importaciones → MOD_CRD → CRD00202.FRM**: [CMXMCRDsrv_icrd_lee_mapr](#referencia-cmxmcrdsrv_icrd_lee_mapr)
- **Importaciones → IMPORT → CRD00202.FRM**: [CMXsrv_imp_calc_aladi](#referencia-cmxsrv_imp_calc_aladi)
- **Importaciones → MOD_CRD → CRD00202.FRM**: [CMXsrv_ctb_impto_tim3](#referencia-cmxsrv_ctb_impto_tim3)
- **Importaciones → MOD_ADI → CRD00202.FRM**: [CMXsrv_icrd_act_pag_mix](#referencia-cmxsrv_icrd_act_pag_mix)
- **Importaciones → IMPORT → CRD00202.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → IMPORT → CRD00202.FRM**: [CMXsrv_ctb_impto_tim](#referencia-cmxsrv_ctb_impto_tim)
- **Importaciones → IMPORT → CRD00202.FRM**: [CMXsrv_ctb_impto_tim2](#referencia-cmxsrv_ctb_impto_tim2)
- **Importaciones → IMPORT → CRD00202.FRM**: [CMXsrv_busc_cod_ope](#referencia-cmxsrv_busc_cod_ope)
- **Importaciones → IMPORT → CRD00202.FRM**: [CMXsrv_util_pesos](#referencia-cmxsrv_util_pesos)
- **Importaciones → MOD_ADI → CRD00202.FRM**: [CMXsrv_icrd_a_dat_apr](#referencia-cmxsrv_icrd_a_dat_apr)
- **Importaciones → MOD_ADI → CRD00202.FRM**: [CMXsrv_imp_calc_aladi](#referencia-cmxsrv_imp_calc_aladi)
- **Importaciones → IMPORT → CRD00202.FRM**: [CMXMCRDsrv_icrd_lee_mapr](#referencia-cmxmcrdsrv_icrd_lee_mapr)
- **Importaciones → MOD_CRD → CRD00202.FRM**: [CMXsrv_icrd_act_pag_mix](#referencia-cmxsrv_icrd_act_pag_mix)
- **Importaciones → IMPORT → CRD00202.FRM**: [CMXsrv_ctb_impto_tim3](#referencia-cmxsrv_ctb_impto_tim3)
- **Importaciones → MOD_ADI → CRD00202.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → MOD_ADI → CRD00202.FRM**: [CMXsrv_ctb_impto_tim](#referencia-cmxsrv_ctb_impto_tim)
- **Importaciones → MOD_ADI → CRD00202.FRM**: [CMXsrv_ctb_impto_tim2](#referencia-cmxsrv_ctb_impto_tim2)
- **Importaciones → MOD_ADI → CRD00202.FRM**: [CMXsrv_busc_cod_ope](#referencia-cmxsrv_busc_cod_ope)
- **Importaciones → MOD_ADI → CRD00202.FRM**: [CMXsrv_util_pesos](#referencia-cmxsrv_util_pesos)
- **Importaciones → MOD_CRD → CRD00202.FRM**: [CMXsrv_icrd_a_dat_apr](#referencia-cmxsrv_icrd_a_dat_apr)
- **Importaciones → MOD_CRD → CRD00202.FRM**: [CMXsrv_imp_calc_aladi](#referencia-cmxsrv_imp_calc_aladi)
- **Importaciones → MOD_ADI → CRD00202.FRM**: [CMXMCRDsrv_icrd_lee_mapr](#referencia-cmxmcrdsrv_icrd_lee_mapr)
- **Importaciones → MOD_CRD → CRD00202.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → MOD_ADI → CRD00202.FRM**: [CMXsrv_ctb_impto_tim3](#referencia-cmxsrv_ctb_impto_tim3)
- **Importaciones → IMPORT → CRD00202.FRM**: [CMXsrv_icrd_act_pag_mix](#referencia-cmxsrv_icrd_act_pag_mix)
- **Importaciones → MOD_CRD → CRD00202.FRM**: [CMXsrv_ctb_impto_tim](#referencia-cmxsrv_ctb_impto_tim)
- **Importaciones → MOD_CRD → CRD00202.FRM**: [CMXsrv_busc_cod_ope](#referencia-cmxsrv_busc_cod_ope)
- **Importaciones → MOD_CRD → CRD00202.FRM**: [CMXsrv_ctb_impto_tim2](#referencia-cmxsrv_ctb_impto_tim2)
- **Importaciones → MOD_CRD → CRD00202.FRM**: [CMXsrv_util_pesos](#referencia-cmxsrv_util_pesos)

---

## CMXCRDsrv_icrd_crea_crd
<a name="cmxcrdsrv_icrd_crea_crd"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → IMPORT → CRD00202.FRM**: [CMXsrv_fincol_ing_modcol](#referencia-cmxsrv_fincol_ing_modcol)
- **Importaciones → IMPORT → CRD00202.FRM**: [CMXsrv_imp_calc_aladi](#referencia-cmxsrv_imp_calc_aladi)
- **Importaciones → IMPORT → CRD00202.FRM**: [CMXCRDsrv_icrd_lee_tas_cln](#referencia-cmxcrdsrv_icrd_lee_tas_cln)
- **Importaciones → IMPORT → CRD00202.FRM**: [CMXsrv_fincol_imod_colcc](#referencia-cmxsrv_fincol_imod_colcc)
- **Importaciones → IMPORT → CRD00202.FRM**: [CMXsrv_util_num_ope](#referencia-cmxsrv_util_num_ope)
- **Importaciones → IMPORT → CRD00202.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_busc_emb
<a name="cmxsrv_icrd_busc_emb"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → IMPORT → CRD00203.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → MOD_CRD → CRD00203.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → NNEGO → CRD01003.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_eli_emb
<a name="cmxsrv_icrd_eli_emb"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → IMPORT → CRD00204.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → MOD_CRD → CRD00204.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_emb1
<a name="cmxsrv_icrd_lee_emb1"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → IMPORT → CRD00204.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → NNEGO → CRD01005.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_emb2
<a name="cmxsrv_icrd_lee_emb2"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → IMPORT → CRD00204.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → NNEGO → CRD01005.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_a_emb1
<a name="cmxsrv_icrd_a_emb1"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → IMPORT → CRD00204.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → MOD_CRD → CRD00204.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_a_emb2
<a name="cmxsrv_icrd_a_emb2"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → IMPORT → CRD00204.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → MOD_CRD → CRD00204.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_val_emb2
<a name="cmxsrv_icrd_val_emb2"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → IMPORT → CRD00204.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → MOD_CRD → CRD00204.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_val_emb1
<a name="cmxsrv_icrd_val_emb1"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → IMPORT → CRD00204.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → MOD_CRD → CRD00204.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_act_ref
<a name="cmxsrv_icrd_act_ref"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → IMPORT → CRD00205.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → MOD_CRD → CRD00205.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_ref
<a name="cmxsrv_icrd_lee_ref"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → IMPORT → CRD00205.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXCRDsrv_icrd_apr_sol
<a name="cmxcrdsrv_icrd_apr_sol"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → IMPORT → CRD0063.FRM**: [CMXsrv_icrd_asignar_cor](#referencia-cmxsrv_icrd_asignar_cor)
- **Importaciones → IMPORT → CRD0063.FRM**: [CMXsrv_ctb_impto_tim](#referencia-cmxsrv_ctb_impto_tim)
- **Importaciones → IMPORT → CRD0063.FRM**: [CMXsrv_ctb_impto_tim3](#referencia-cmxsrv_ctb_impto_tim3)
- **Importaciones → IMPORT → CRD0063.FRM**: [CMXsrv_nibx_nilive](#referencia-cmxsrv_nibx_nilive)
- **Importaciones → IMPORT → CRD0063.FRM**: [CMXsrv_util_pesos](#referencia-cmxsrv_util_pesos)
- **Importaciones → IMPORT → CRD0063.FRM**: [CMXsrv_ctb_impto_tim22](#referencia-cmxsrv_ctb_impto_tim22)
- **Importaciones → IMPORT → CRD0063.FRM**: [CMXsrv_ctb_impto_tim2](#referencia-cmxsrv_ctb_impto_tim2)
- **Importaciones → IMPORT → CRD0063.FRM**: [CMXsrv_mbyte_gen](#referencia-cmxsrv_mbyte_gen)
- **Importaciones → IMPORT → CRD0063.FRM**: [CMXsrv_icrd_val_crd](#referencia-cmxsrv_icrd_val_crd)
- **Importaciones → IMPORT → CRD0063.FRM**: [CMXsrv_iswf_a_700](#referencia-cmxsrv_iswf_a_700)
- **Importaciones → IMPORT → CRD0063.FRM**: [CMXsrv_lee_paridad](#referencia-cmxsrv_lee_paridad)
- **Importaciones → IMPORT → CRD0063.FRM**: [CMXsrv_fincol_imod_colcc](#referencia-cmxsrv_fincol_imod_colcc)
- **Importaciones → IMPORT → CRD0063.FRM**: [CMXsrv_nibx_upd_tran](#referencia-cmxsrv_nibx_upd_tran)
- **Importaciones → IMPORT → CRD0063.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → IMPORT → CRD0063.FRM**: [CMXsrv_cmx_ing_lib](#referencia-cmxsrv_cmx_ing_lib)

---

## CMXsrv_icrd_lee_crdapr
<a name="cmxsrv_icrd_lee_crdapr"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → IMPORT → CRD0063.FRM**: [CMXsrv_icrd_pre_72](#referencia-cmxsrv_icrd_pre_72)
- **Importaciones → IMPORT → CRD0063.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXCRDsrv_icrd_a_desc_merc
<a name="cmxcrdsrv_icrd_a_desc_merc"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → IMPORT → DESCMERC.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_desc_merc
<a name="cmxsrv_icrd_lee_desc_merc"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → IMPORT → DESCMERC.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → MOD_CRD → DESCMERC.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → MOD_CRD → CRD00204.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → NNEGO → CRD01005.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_a_otr_doc
<a name="cmxsrv_icrd_a_otr_doc"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → MOD_CRD → DOCUME.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → IMPORT → DOCUMENT.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_otr_doc
<a name="cmxsrv_icrd_lee_otr_doc"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → MOD_CRD → DOCUME.FRM**: [CMXsrv_icrd_pre_46](#referencia-cmxsrv_icrd_pre_46)
- **Importaciones → MOD_CRD → DOCUME.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → IMPORT → DOCUMENT.FRM**: [CMXsrv_icrd_pre_46](#referencia-cmxsrv_icrd_pre_46)
- **Importaciones → IMPORT → DOCUMENT.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iinf_lee0_inf
<a name="cmxsrv_iinf_lee0_inf"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → INFORME → INFO0102.FRM**: [PrmACLNEJECTA](#referencia-prmaclnejecta)
- **Importaciones → INFORME → INFO0101.FRM**: [PrmACLNEJECTA](#referencia-prmaclnejecta)
- **Importaciones → INFORME → INFO0102.FRM**: [PrmACMXMONEDA](#referencia-prmacmxmoneda)
- **Importaciones → INFORME → INFO0101.FRM**: [PrmACMXFPAIMP](#referencia-prmacmxfpaimp)
- **Importaciones → INFORME → INFO0101.FRM**: [PrmACMXMONEDA](#referencia-prmacmxmoneda)
- **Importaciones → INFORME → INFO0102.FRM**: [PrmACMXFPAIMP](#referencia-prmacmxfpaimp)
- **Importaciones → INFORME → INFO0102.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → INFORME → INFO0101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iinf_lee_tablas
<a name="cmxsrv_iinf_lee_tablas"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → INFORME → INFO0111.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → INFORME → INFO0102.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → INFORME → INFO0101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iinf_lee1_inf
<a name="cmxsrv_iinf_lee1_inf"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → INFORME → INFO0101.FRM**: [PrmACMXESPECI](#referencia-prmacmxespeci)
- **Importaciones → INFORME → INFO0101.FRM**: [PrmACMXCLACOM](#referencia-prmacmxclacom)
- **Importaciones → INFORME → INFO0102.FRM**: [PrmACLNEJECTA](#referencia-prmaclnejecta)
- **Importaciones → INFORME → INFO0102.FRM**: [PrmACMXETDINF](#referencia-prmacmxetdinf)
- **Importaciones → INFORME → INFO0101.FRM**: [PrmACLNEJECTA](#referencia-prmaclnejecta)
- **Importaciones → INFORME → INFO0101.FRM**: [PrmACMXETDINF](#referencia-prmacmxetdinf)
- **Importaciones → INFORME → INFO0102.FRM**: [PrmACMXCLACOM](#referencia-prmacmxclacom)
- **Importaciones → INFORME → INFO0102.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → INFORME → INFO0102.FRM**: [PrmACMXESPECI](#referencia-prmacmxespeci)
- **Importaciones → INFORME → INFO0101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iinf_lee_cln
<a name="cmxsrv_iinf_lee_cln"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → INFORME → INFO0103.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → INFORME → INFO0102.FRM**: [PrmACLNEJECTA](#referencia-prmaclnejecta)
- **Importaciones → INFORME → INFO0103.FRM**: [PrmACLNEJECTA](#referencia-prmaclnejecta)
- **Importaciones → INFORME → INFO0101.FRM**: [PrmACLNEJECTA](#referencia-prmaclnejecta)
- **Importaciones → INFORME → INFO0102.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → INFORME → INFO0101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iinf_lee2_inf
<a name="cmxsrv_iinf_lee2_inf"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → INFORME → INFO0101.FRM**: [PrmACMXBCOCEN](#referencia-prmacmxbcocen)
- **Importaciones → INFORME → INFO0102.FRM**: [PrmACMXRGMIMP](#referencia-prmacmxrgmimp)
- **Importaciones → INFORME → INFO0102.FRM**: [PrmACMXBCOCEN](#referencia-prmacmxbcocen)
- **Importaciones → INFORME → INFO0102.FRM**: [PrmACMXPAIS](#referencia-prmacmxpais)
- **Importaciones → INFORME → INFO0101.FRM**: [PrmACMXRGMIMP](#referencia-prmacmxrgmimp)
- **Importaciones → INFORME → INFO0102.FRM**: [PrmACMXSUCSAL](#referencia-prmacmxsucsal)
- **Importaciones → INFORME → INFO0101.FRM**: [PrmACMXPAIS](#referencia-prmacmxpais)
- **Importaciones → INFORME → INFO0101.FRM**: [PrmACMXORIDVS](#referencia-prmacmxoridvs)
- **Importaciones → INFORME → INFO0101.FRM**: [PrmACMXSUCSAL](#referencia-prmacmxsucsal)
- **Importaciones → INFORME → INFO0102.FRM**: [PrmACMXORIDVS](#referencia-prmacmxoridvs)
- **Importaciones → INFORME → INFO0101.FRM**: [PrmACMXBCOBCC](#referencia-prmacmxbcobcc)
- **Importaciones → INFORME → INFO0102.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → INFORME → INFO0102.FRM**: [PrmACMXBCOBCC](#referencia-prmacmxbcobcc)
- **Importaciones → INFORME → INFO0101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iinf_avi_miscb
<a name="cmxsrv_iinf_avi_miscb"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → INFORME → INFO0101.FRM**: [PrmACMXBCOBCC](#referencia-prmacmxbcobcc)
- **Importaciones → INFORME → INFO0101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iinf_avi_misca
<a name="cmxsrv_iinf_avi_misca"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → INFORME → INFO0101.FRM**: [PrmACMXCLACOM](#referencia-prmacmxclacom)
- **Importaciones → INFORME → INFO0101.FRM**: [PrmACMXRGMIMP](#referencia-prmacmxrgmimp)
- **Importaciones → INFORME → INFO0101.FRM**: [PrmACLNEJECTA](#referencia-prmaclnejecta)
- **Importaciones → INFORME → INFO0101.FRM**: [PrmACMXPAIS](#referencia-prmacmxpais)
- **Importaciones → INFORME → INFO0101.FRM**: [PrmACMXORIDVS](#referencia-prmacmxoridvs)
- **Importaciones → INFORME → INFO0101.FRM**: [PrmACMXFPAIMP](#referencia-prmacmxfpaimp)
- **Importaciones → INFORME → INFO0101.FRM**: [PrmACMXSUCSAL](#referencia-prmacmxsucsal)
- **Importaciones → INFORME → INFO0101.FRM**: [PrmACMXMONEDA](#referencia-prmacmxmoneda)
- **Importaciones → INFORME → INFO0101.FRM**: [PrmACMXETDINF](#referencia-prmacmxetdinf)
- **Importaciones → INFORME → INFO0101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_dat_com
<a name="cmxsrv_icrd_lee_dat_com"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → INFORME → INFO0101.FRM**: [PrmACMXMONEDA](#referencia-prmacmxmoneda)
- **Importaciones → INFORME → INFO0101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iinf_eli_inf
<a name="cmxsrv_iinf_eli_inf"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → INFORME → INFO0101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iinf_busc_evi
<a name="cmxsrv_iinf_busc_evi"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → INFORME → INFO0105.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → INFORME → INFO0101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iinf_val_inf
<a name="cmxsrv_iinf_val_inf"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → INFORME → INFO0101.FRM**: [CMXsrv_cmx_get_codes](#referencia-cmxsrv_cmx_get_codes)
- **Importaciones → INFORME → INFO0101.FRM**: [PrmACMXCLACOM](#referencia-prmacmxclacom)
- **Importaciones → INFORME → INFO0101.FRM**: [PrmACMXPAIS](#referencia-prmacmxpais)
- **Importaciones → INFORME → INFO0101.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iinf_ingmod_inf
<a name="cmxsrv_iinf_ingmod_inf"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → INFORME → INFO0102.FRM**: [CMXsrv_util_fecha](#referencia-cmxsrv_util_fecha)
- **Importaciones → INFORME → INFO0102.FRM**: [CMXsrv_cmx_get_codes](#referencia-cmxsrv_cmx_get_codes)
- **Importaciones → INFORME → INFO0102.FRM**: [CMXsrv_iinf_get_num](#referencia-cmxsrv_iinf_get_num)
- **Importaciones → INFORME → INFO0102.FRM**: [CMXsrv_iinf_val_inf](#referencia-cmxsrv_iinf_val_inf)
- **Importaciones → INFORME → INFO0102.FRM**: [PrmACMXMONEDAFEC](#referencia-prmacmxmonedafec)
- **Importaciones → INFORME → INFO0102.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iinf_lee_fec
<a name="cmxsrv_iinf_lee_fec"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → INFORME → INFO0111.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → INFORME → INFO0111.FRM**: [CMXsrv_util_fecha](#referencia-cmxsrv_util_fecha)
- **Importaciones → INFORME → INFO0102.FRM**: [CMXsrv_util_fecha](#referencia-cmxsrv_util_fecha)
- **Importaciones → INFORME → INFO0103.FRM**: [CMXsrv_util_fecha](#referencia-cmxsrv_util_fecha)
- **Importaciones → INFORME → INFO0102.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → INFORME → INFO0103.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iinf_lee_usd
<a name="cmxsrv_iinf_lee_usd"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → INFORME → INFO0102.FRM**: [PrmACMXMONEDAFEC](#referencia-prmacmxmonedafec)
- **Importaciones → INFORME → INFO0102.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → INFORME → INFO0102.FRM**: [CMXsrv_cmx_get_codes](#referencia-cmxsrv_cmx_get_codes)

---

## CMXsrv_iinf_act_apr
<a name="cmxsrv_iinf_act_apr"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → INFORME → INFO0104.FRM**: [CMXsrv_iinf_val_inf](#referencia-cmxsrv_iinf_val_inf)
- **Importaciones → INFORME → INFO0104.FRM**: [CMXsrv_util_fecha](#referencia-cmxsrv_util_fecha)
- **Importaciones → INFORME → INFO0104.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iinf_lee_evi
<a name="cmxsrv_iinf_lee_evi"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → INFORME → INFO0106.FRM**: [PrmACMXBCOCEN](#referencia-prmacmxbcocen)
- **Importaciones → INFORME → INFO0106.FRM**: [PrmACMXETDINF](#referencia-prmacmxetdinf)
- **Importaciones → INFORME → INFO0106.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → INFORME → INFO0106.FRM**: [PrmACMXSUCSAL](#referencia-prmacmxsucsal)

---

## CMXsrv_iinf_act_tib
<a name="cmxsrv_iinf_act_tib"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → INFORME → INFO0107.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → INFORME → INFO0107.FRM**: [CMXsrv_cmx_get_codes](#referencia-cmxsrv_cmx_get_codes)

---

## CMXsrv_iinf_act_rec
<a name="cmxsrv_iinf_act_rec"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → INFORME → INFO0108.FRM**: [CMXsrv_util_fecha](#referencia-cmxsrv_util_fecha)
- **Importaciones → INFORME → INFO0108.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iinf_act_rib
<a name="cmxsrv_iinf_act_rib"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → INFORME → INFO0109.FRM**: [CMXsrv_cmx_get_codes](#referencia-cmxsrv_cmx_get_codes)
- **Importaciones → INFORME → INFO0109.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iinf_busc_comp
<a name="cmxsrv_iinf_busc_comp"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → INFORME → INFO0110.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iinf_ingmod_comp
<a name="cmxsrv_iinf_ingmod_comp"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → INFORME → INFO0111.FRM**: [PrmACMXMONEDAFEC](#referencia-prmacmxmonedafec)
- **Importaciones → INFORME → INFO0111.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → INFORME → INFO0111.FRM**: [CMXsrv_util_fecha](#referencia-cmxsrv_util_fecha)
- **Importaciones → INFORME → INFO0111.FRM**: [CMXsrv_cmx_get_codes](#referencia-cmxsrv_cmx_get_codes)
- **Importaciones → INFORME → INFO0111.FRM**: [CMXsrv_iinf_val_inf](#referencia-cmxsrv_iinf_val_inf)
- **Importaciones → INFORME → INFO0111.FRM**: [CMXsrv_iinf_get_num](#referencia-cmxsrv_iinf_get_num)

---

## CMXsrv_iinf_lee_comp
<a name="cmxsrv_iinf_lee_comp"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → INFORME → INFO0111.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → INFORME → INFO0111.FRM**: [PrmACMXCLACOM](#referencia-prmacmxclacom)
- **Importaciones → INFORME → INFO0111.FRM**: [PrmACMXRGMIMP](#referencia-prmacmxrgmimp)
- **Importaciones → INFORME → INFO0111.FRM**: [PrmACMXPAIS](#referencia-prmacmxpais)
- **Importaciones → INFORME → INFO0111.FRM**: [PrmACMXORIDVS](#referencia-prmacmxoridvs)
- **Importaciones → INFORME → INFO0111.FRM**: [PrmACMXFPAIMP](#referencia-prmacmxfpaimp)
- **Importaciones → INFORME → INFO0111.FRM**: [PrmACMXMONEDA](#referencia-prmacmxmoneda)
- **Importaciones → INFORME → INFO0111.FRM**: [PrmACMXVIATPT](#referencia-prmacmxviatpt)

---

## CMXsrv_iinf_lee_bco
<a name="cmxsrv_iinf_lee_bco"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → INFORME → INFO0112.FRM**: [PrmACMXPAIS](#referencia-prmacmxpais)
- **Importaciones → INFORME → INFO0112.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iinf_busc_bco
<a name="cmxsrv_iinf_busc_bco"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → INFORME → INFO0112.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXMCRDsrv_icrd_lee_mcnd
<a name="cmxmcrdsrv_icrd_lee_mcnd"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → MOD_CRD → CRD00202.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → MOD_CRD → MOD00603.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → MOD_ADI → CRD00202.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_mod_ing_let
<a name="cmxsrv_icbr_mod_ing_let"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → MOD_CBR → CBR00302.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → MOD_CBR → CBR00302.FRM**: [CMXsrv_util_opr_fec](#referencia-cmxsrv_util_opr_fec)

---

## CMXsrv_icbr_acep_mod_cbr
<a name="cmxsrv_icbr_acep_mod_cbr"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → MOD_CBR → PANBASE.FRM**: [CMXsrv_icbr_cheq_mlcb](#referencia-cmxsrv_icbr_cheq_mlcb)
- **Importaciones → MOD_CBR → PANBASE.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → MOD_CBR → PANBASE.FRM**: [CMXsrv_icbr_cheq_mctp](#referencia-cmxsrv_icbr_cheq_mctp)
- **Importaciones → MOD_CBR → PANBASE.FRM**: [CMXsrv_cnt_2800](#referencia-cmxsrv_cnt_2800)
- **Importaciones → MOD_CBR → PANBASE.FRM**: [CMXsrv_icbr_cheq_mdoc](#referencia-cmxsrv_icbr_cheq_mdoc)
- **Importaciones → MOD_CBR → PANBASE.FRM**: [CMXsrv_icbr_val_cbr](#referencia-cmxsrv_icbr_val_cbr)
- **Importaciones → MOD_CBR → PANBASE.FRM**: [CMXsrv_icbr_cheq_mter](#referencia-cmxsrv_icbr_cheq_mter)

---

## CMXsrv_icbr_eli_no_cont
<a name="cmxsrv_icbr_eli_no_cont"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → MOD_CBR → PANBASE.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXMCRDsrv_icrd_a_mmcnd
<a name="cmxmcrdsrv_icrd_a_mmcnd"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → MOD_CRD → CONDESP.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXMCRDsrv_icrd_lee_mctp
<a name="cmxmcrdsrv_icrd_lee_mctp"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → MOD_CRD → CRD00201.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXMCRDsrv_icrd_lee_memb2
<a name="cmxmcrdsrv_icrd_lee_memb2"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → MOD_CRD → CRD00204.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXMCRDsrv_icrd_lee_memb1
<a name="cmxmcrdsrv_icrd_lee_memb1"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → MOD_CRD → CRD00204.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXMCRDsrv_icrd_lee_mref
<a name="cmxmcrdsrv_icrd_lee_mref"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → MOD_CRD → CRD00205.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_ing_txt
<a name="cmxsrv_icrd_ing_txt"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → MOD_CRD → CRD00206.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXCRDsrv_icrd_get_ing_esp
<a name="cmxcrdsrv_icrd_get_ing_esp"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → MOD_CRD → CRD00206.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXMCRDsrv_icrd_lee_mtxt
<a name="cmxmcrdsrv_icrd_lee_mtxt"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → MOD_CRD → CRD00206.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXCRDsrv_icrd_get_pre_fra
<a name="cmxcrdsrv_icrd_get_pre_fra"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → MOD_CRD → CRD00207.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXMCRDsrv_icrd_a_mmer
<a name="cmxmcrdsrv_icrd_a_mmer"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → MOD_CRD → DESCMERC.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_lee_cod_eve
<a name="cmxsrv_fincol_lee_cod_eve"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → MOD_CRD → MOD00603.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXMCRDsrv_icrd_acep_mod_crd
<a name="cmxmcrdsrv_icrd_acep_mod_crd"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → MOD_CRD → MOD00603.FRM**: [CMXsrv_icrd_cheq_mmcnd](#referencia-cmxsrv_icrd_cheq_mmcnd)
- **Importaciones → MOD_CRD → MOD00603.FRM**: [CMXsrv_nibx_upd_tran](#referencia-cmxsrv_nibx_upd_tran)
- **Importaciones → MOD_CRD → MOD00603.FRM**: [CMXCRDsrv_icrd_val_crd](#referencia-cmxcrdsrv_icrd_val_crd)
- **Importaciones → MOD_CRD → MOD00603.FRM**: [CMXsrv_expcce_anl_cce](#referencia-cmxsrv_expcce_anl_cce)
- **Importaciones → MOD_CRD → MOD00603.FRM**: [CMXsrv_icrd_cheq_mtxt](#referencia-cmxsrv_icrd_cheq_mtxt)
- **Importaciones → MOD_CRD → MOD00603.FRM**: [CMXsrv_icrd_cheq_mref](#referencia-cmxsrv_icrd_cheq_mref)
- **Importaciones → MOD_CRD → MOD00603.FRM**: [CMXMCRDsrv_icrd_eli_no_cont](#referencia-cmxmcrdsrv_icrd_eli_no_cont)
- **Importaciones → MOD_CRD → MOD00603.FRM**: [CMXsrv_icrd_cheq_mibar](#referencia-cmxsrv_icrd_cheq_mibar)
- **Importaciones → MOD_CRD → MOD00603.FRM**: [CMXsrv_ctl_crea_apr](#referencia-cmxsrv_ctl_crea_apr)
- **Importaciones → MOD_CRD → MOD00603.FRM**: [CMXsrv_cnt_950](#referencia-cmxsrv_cnt_950)
- **Importaciones → MOD_CRD → MOD00603.FRM**: [CMXsrv_icrd_lee_tip_ope](#referencia-cmxsrv_icrd_lee_tip_ope)
- **Importaciones → MOD_CRD → MOD00603.FRM**: [CMXsrv_nibx_nilive](#referencia-cmxsrv_nibx_nilive)
- **Importaciones → MOD_CRD → MOD00603.FRM**: [CMXsrv_icrd_cheq_mctp](#referencia-cmxsrv_icrd_cheq_mctp)
- **Importaciones → MOD_CRD → MOD00603.FRM**: [CMXsrv_icrd_cheq_mapr](#referencia-cmxsrv_icrd_cheq_mapr)
- **Importaciones → MOD_CRD → MOD00603.FRM**: [CMXsrv_fincol_ctb_mod](#referencia-cmxsrv_fincol_ctb_mod)
- **Importaciones → MOD_CRD → MOD00603.FRM**: [CMXsrv_icrd_cheq_mcnd](#referencia-cmxsrv_icrd_cheq_mcnd)
- **Importaciones → MOD_CRD → MOD00603.FRM**: [CMXsrv_icrd_cheq_mpmix](#referencia-cmxsrv_icrd_cheq_mpmix)
- **Importaciones → MOD_CRD → MOD00603.FRM**: [CMXsrv_icrd_cheq_mmer](#referencia-cmxsrv_icrd_cheq_mmer)
- **Importaciones → MOD_CRD → MOD00603.FRM**: [CMXsrv_icrd_cheq_mibab](#referencia-cmxsrv_icrd_cheq_mibab)
- **Importaciones → MOD_CRD → MOD00603.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → MOD_CRD → MOD00603.FRM**: [CMXsrv_icrd_cheq_modoc](#referencia-cmxsrv_icrd_cheq_modoc)
- **Importaciones → MOD_CRD → MOD00603.FRM**: [CMXsrv_icrd_cheq_memb](#referencia-cmxsrv_icrd_cheq_memb)

---

## CMXMCRDsrv_icrd_eli_no_cont
<a name="cmxmcrdsrv_icrd_eli_no_cont"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → MOD_CRD → MOD00603.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_a_rec_age
<a name="cmxsrv_icrd_a_rec_age"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → NEGO_AV → CRD01001.FRM**: [CMXsrv_util_fecha](#referencia-cmxsrv_util_fecha)
- **Importaciones → NEGO_AV → AVISOS.FRM**: [CMXsrv_util_fecha](#referencia-cmxsrv_util_fecha)
- **Importaciones → NEGO_AV → CRD01001.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → NEGO_AV → AVISOS.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_busc_ofi_cta
<a name="cmxsrv_busc_ofi_cta"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → NEGO_AV → CRD01001.FRM**: [PrmACLNEJECTA](#referencia-prmaclnejecta)
- **Importaciones → NEGO_AV → AVISOS.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → NEGO_AV → AVISOS.FRM**: [PrmACMXESPECI](#referencia-prmacmxespeci)
- **Importaciones → NEGO_AV → AVISOS.FRM**: [PrmACLNEJECTA](#referencia-prmaclnejecta)
- **Importaciones → NEGO_AV → CRD01001.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → NEGO_AV → CRD01001.FRM**: [PrmACMXESPECI](#referencia-prmacmxespeci)

---

## CMXsrv_neg_busc_arc
<a name="cmxsrv_neg_busc_arc"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → NEGO_AV → AVISOS.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_avi_adi
<a name="cmxsrv_icrd_lee_avi_adi"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → NEGO_AV → AVISOS.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_dat_cln
<a name="cmxsrv_icrd_lee_dat_cln"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → NEGO_AV → AVISOS.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → NEGO_AV → AVISOS.FRM**: [CMXsrv_trae_glo_fec](#referencia-cmxsrv_trae_glo_fec)

---

## CMXsrv_icrd_lee_avi_dis
<a name="cmxsrv_icrd_lee_avi_dis"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → NEGO_AV → AVISOS.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_neg_ddi_asoc
<a name="cmxsrv_neg_ddi_asoc"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → NEGO_AV → AVISOS.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_neg_trae_vcto_mcf
<a name="cmxsrv_neg_trae_vcto_mcf"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → NEGO_AV → AVISOS.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_neg_avi_lee_aval
<a name="cmxsrv_neg_avi_lee_aval"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → NEGO_AV → AVISOS.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_neg_lee_crd
<a name="cmxsrv_icrd_neg_lee_crd"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → NNEGO → CRD01001.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → NEGO_AV → CRD01001.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → NEGO_AV → AVISOS.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_neg
<a name="cmxsrv_icrd_lee_neg"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → NNEGO → CRD01001.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → NEGO_AV → CRD01001.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → NEGO_AV → AVISOS.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_col_avi_dat_cln
<a name="cmxsrv_col_avi_dat_cln"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → NEGO_AV → AVI_COL.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_col_avi_det_pag
<a name="cmxsrv_col_avi_det_pag"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → NEGO_AV → AVI_COL.FRM**: [CMXsrv_util_fecha](#referencia-cmxsrv_util_fecha)
- **Importaciones → NEGO_AV → AVI_COL.FRM**: [CMX_srv_pone_punto](#referencia-cmx_srv_pone_punto)
- **Importaciones → NEGO_AV → AVI_COL.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_col_avi_det_oto
<a name="cmxsrv_col_avi_det_oto"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → NEGO_AV → AVI_COL.FRM**: [CMX_srv_pone_punto](#referencia-cmx_srv_pone_punto)
- **Importaciones → NEGO_AV → AVI_COL.FRM**: [CMXsrv_trae_glo_fec](#referencia-cmxsrv_trae_glo_fec)
- **Importaciones → NEGO_AV → AVI_COL.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_col_lee_num_trs
<a name="cmxsrv_col_lee_num_trs"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → NEGO_AV → AVI_COL.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → NEGO_AV → AVI_COL.FRM**: [CMXsrv_avigrl_lee_avitemp](#referencia-cmxsrv_avigrl_lee_avitemp)

---

## CMXsrv_finobl_avi_pag
<a name="cmxsrv_finobl_avi_pag"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → NEGO_AV → AVI_COL.FRM**: [CMX_srv_pone_punto](#referencia-cmx_srv_pone_punto)
- **Importaciones → NEGO_AV → AVI_COL.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_neg_avi_trae_asnd_mn
<a name="cmxsrv_neg_avi_trae_asnd_mn"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → NEGO_AV → AVI_COL.FRM**: [CMX_srv_pone_punto](#referencia-cmx_srv_pone_punto)
- **Importaciones → NEGO_AV → AVI_COL.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_neg_avi_trae_asnd_mx
<a name="cmxsrv_neg_avi_trae_asnd_mx"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → NEGO_AV → AVI_COL.FRM**: [CMX_srv_pone_punto](#referencia-cmx_srv_pone_punto)
- **Importaciones → NEGO_AV → AVI_COL.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_cont_neg
<a name="cmxsrv_icrd_cont_neg"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → NEGO_AV → CRD01001.FRM**: [CMXsrv_icrd_val_neg](#referencia-cmxsrv_icrd_val_neg)
- **Importaciones → NNEGO → CRD01001.FRM**: [CMXsrv_mbyte_gen](#referencia-cmxsrv_mbyte_gen)
- **Importaciones → NNEGO → CRD01001.FRM**: [sp_cmx_sii_1870](#referencia-sp_cmx_sii_1870)
- **Importaciones → NNEGO → CRD01001.FRM**: [CMXsrv_fincol_ictb_neg_aux](#referencia-cmxsrv_fincol_ictb_neg_aux)
- **Importaciones → NNEGO → CRD01001.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → NEGO_AV → CRD01001.FRM**: [CMXsrv_mbyte_gen](#referencia-cmxsrv_mbyte_gen)
- **Importaciones → NEGO_AV → CRD01001.FRM**: [CMXsrv_fincol_ictb_neg_aux](#referencia-cmxsrv_fincol_ictb_neg_aux)
- **Importaciones → NNEGO → CRD01001.FRM**: [CMXsrv_icrd_val_neg](#referencia-cmxsrv_icrd_val_neg)
- **Importaciones → NEGO_AV → CRD01001.FRM**: [sp_cmx_sii_1870](#referencia-sp_cmx_sii_1870)
- **Importaciones → NEGO_AV → CRD01001.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_eli_neg
<a name="cmxsrv_icrd_eli_neg"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → NEGO_AV → CRD01001.FRM**: [CMXsrv_swf_graba_det](#referencia-cmxsrv_swf_graba_det)
- **Importaciones → NNEGO → CRD01001.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → NNEGO → CRD01001.FRM**: [CMXsrv_swf_graba_det](#referencia-cmxsrv_swf_graba_det)
- **Importaciones → NEGO_AV → CRD01001.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_num_col
<a name="cmxsrv_icrd_lee_num_col"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → NEGO_AV → PREFER.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_bus_pago
<a name="cmxsrv_icrd_bus_pago"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → NEGO_AV → VER_PAGO.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → NNEGO → VER_PAGO.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_col
<a name="cmxsrv_icrd_lee_col"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → NNEGO → CRD01001.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_busc_neg
<a name="cmxsrv_icrd_busc_neg"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → NNEGO → CRD01002.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_a_neg_emb1
<a name="cmxsrv_icrd_a_neg_emb1"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → NNEGO → CRD01005.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_a_neg_emb2
<a name="cmxsrv_icrd_a_neg_emb2"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → NNEGO → CRD01005.FRM**: [CMXsrv_icrd_chq_doc_neg](#referencia-cmxsrv_icrd_chq_doc_neg)
- **Importaciones → NNEGO → CRD01005.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_eli_doc_neg
<a name="cmxsrv_icrd_eli_doc_neg"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → NNEGO → CRD01005.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_neg_emb1
<a name="cmxsrv_icrd_lee_neg_emb1"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → NNEGO → CRD01005.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_neg_emb2
<a name="cmxsrv_icrd_lee_neg_emb2"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → NNEGO → CRD01005.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_a_neg_disc
<a name="cmxsrv_icrd_a_neg_disc"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → NNEGO → CRD01006.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_neg_lee_disc
<a name="cmxsrv_icrd_neg_lee_disc"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → NNEGO → CRD01006.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → NNEGO → CRD01006.FRM**: [CMXsrv_icrd_gen_disc](#referencia-cmxsrv_icrd_gen_disc)

---

## CMXsrv_icrd_ent_doc
<a name="cmxsrv_icrd_ent_doc"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → NNEGO → CRD01201.FRM**: [CMXsrv_swf_graba_det](#referencia-cmxsrv_swf_graba_det)
- **Importaciones → NNEGO → CRD01201.FRM**: [CMXsrv_mbyte_gen](#referencia-cmxsrv_mbyte_gen)
- **Importaciones → NNEGO → CRD01201.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_alz_disc
<a name="cmxsrv_icrd_alz_disc"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → NNEGO → CRD01301.FRM**: [CMXsrv_cnt_950](#referencia-cmxsrv_cnt_950)
- **Importaciones → NNEGO → CRD01301.FRM**: [CMXsrv_ipuc_gen_pln](#referencia-cmxsrv_ipuc_gen_pln)
- **Importaciones → NNEGO → CRD01301.FRM**: [CMXsrv_fincol_cal_tas_sfr](#referencia-cmxsrv_fincol_cal_tas_sfr)
- **Importaciones → NNEGO → CRD01301.FRM**: [CMXsrv_cmx_get_codes](#referencia-cmxsrv_cmx_get_codes)
- **Importaciones → NNEGO → CRD01301.FRM**: [CMXsrv_get_ult_dia_habil](#referencia-cmxsrv_get_ult_dia_habil)
- **Importaciones → NNEGO → CRD01301.FRM**: [CMXsrv_icrd_cont_alz](#referencia-cmxsrv_icrd_cont_alz)
- **Importaciones → NNEGO → CRD01301.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXCRDsrv_icrd_asignar_cor
<a name="cmxcrdsrv_icrd_asignar_cor"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → NNEGO → CRD02001.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXCRDsrv_icrd_bus_lcr_bco
<a name="cmxcrdsrv_icrd_bus_lcr_bco"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → NNEGO → CRD02001.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_act_doc_neg
<a name="cmxsrv_icrd_act_doc_neg"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → NNEGO → CRD02004.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_doc_neg
<a name="cmxsrv_icrd_lee_doc_neg"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → NNEGO → CRD02004.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_val_neg
<a name="cmxsrv_icrd_val_neg"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → NNEGO → GRL00101.FRM**: [CMXsrv_util_det_habil_tasa](#referencia-cmxsrv_util_det_habil_tasa)
- **Importaciones → NNEGO → GRL00101.FRM**: [CMXsrv_fincol_val_per_tas](#referencia-cmxsrv_fincol_val_per_tas)
- **Importaciones → NNEGO → GRL00101.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → NNEGO → GRL00101.FRM**: [CMXsrv_util_fecha](#referencia-cmxsrv_util_fecha)

---

## CMXsrv_icbr_lee_dat_var
<a name="cmxsrv_icbr_lee_dat_var"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → PAGCBR → CBR01006.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_val_pag
<a name="cmxsrv_icbr_val_pag"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → PAGCBR → CBR01006.FRM**: [CMXsrv_val_cta_cte](#referencia-cmxsrv_val_cta_cte)
- **Importaciones → PAGCBR → CBR01008.FRM**: [CMXsrv_enl_val_sel](#referencia-cmxsrv_enl_val_sel)
- **Importaciones → PAGCBR → CBR01006.FRM**: [CMXsrv_calc_imp_4pct](#referencia-cmxsrv_calc_imp_4pct)
- **Importaciones → PAGCBR → CBR01008.FRM**: [CMXsrv_val_cta_cte](#referencia-cmxsrv_val_cta_cte)
- **Importaciones → PAGCBR → CBR01008.FRM**: [CMXsrv_calc_imp_4pct](#referencia-cmxsrv_calc_imp_4pct)
- **Importaciones → PAGCBR → CBR01006.FRM**: [CMXsrv_util_fecha](#referencia-cmxsrv_util_fecha)
- **Importaciones → PAGCBR → CBR01006.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → PAGCBR → CBR01006.FRM**: [CMXsrv_ctb_impto_ddi](#referencia-cmxsrv_ctb_impto_ddi)
- **Importaciones → PAGCBR → CBR01008.FRM**: [CMXsrv_ctb_impto_ddi](#referencia-cmxsrv_ctb_impto_ddi)
- **Importaciones → PAGCBR → CBR01008.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → PAGCBR → CBR01006.FRM**: [CMXsrv_enl_val_sel](#referencia-cmxsrv_enl_val_sel)
- **Importaciones → PAGCBR → CBR01008.FRM**: [CMXsrv_util_fecha](#referencia-cmxsrv_util_fecha)

---

## CMXsrv_icbr_ctb_pag
<a name="cmxsrv_icbr_ctb_pag"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → PAGCBR → CBR01006.FRM**: [CMXsrv_val_cta_cte](#referencia-cmxsrv_val_cta_cte)
- **Importaciones → PAGCBR → CBR01006.FRM**: [CMXsrv_cnt_gen_vig](#referencia-cmxsrv_cnt_gen_vig)
- **Importaciones → PAGCBR → CBR01006.FRM**: [CMXsrv_icbr_act_rem](#referencia-cmxsrv_icbr_act_rem)
- **Importaciones → PAGCBR → CBR01006.FRM**: [CMXsrv_mbyte_gen](#referencia-cmxsrv_mbyte_gen)
- **Importaciones → PAGCBR → CBR01006.FRM**: [CMXsrv_cmx_get_codes](#referencia-cmxsrv_cmx_get_codes)
- **Importaciones → PAGCBR → CBR01006.FRM**: [CMXsrv_get_ult_dia_habil](#referencia-cmxsrv_get_ult_dia_habil)
- **Importaciones → PAGCBR → CBR01006.FRM**: [CMXsrv_calc_imp_4pct](#referencia-cmxsrv_calc_imp_4pct)
- **Importaciones → PAGCBR → CBR01006.FRM**: [CMXsrv_enl_act_enl](#referencia-cmxsrv_enl_act_enl)
- **Importaciones → PAGCBR → CBR01006.FRM**: [CMXsrv_iddi2_gen_det_pag](#referencia-cmxsrv_iddi2_gen_det_pag)
- **Importaciones → PAGCBR → CBR01006.FRM**: [sp_cmx_sii_1870](#referencia-sp_cmx_sii_1870)
- **Importaciones → PAGCBR → CBR01006.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → PAGCBR → CBR01006.FRM**: [CMXsrv_icbr_ctb_pag1](#referencia-cmxsrv_icbr_ctb_pag1)
- **Importaciones → PAGCBR → CBR01006.FRM**: [CMXsrv_ctb_impto_ddi](#referencia-cmxsrv_ctb_impto_ddi)
- **Importaciones → PAGCBR → CBR01006.FRM**: [CMXsrv_ipuc_gen_pln](#referencia-cmxsrv_ipuc_gen_pln)
- **Importaciones → PAGCBR → CBR01006.FRM**: [CMXsrv_util_fecha](#referencia-cmxsrv_util_fecha)
- **Importaciones → PAGCBR → CBR01006.FRM**: [CMXsrv_vig_gra_vig](#referencia-cmxsrv_vig_gra_vig)
- **Importaciones → PAGCBR → CBR01006.FRM**: [CMXsrv_util_pesos](#referencia-cmxsrv_util_pesos)

---

## CMXsrv_icbr_cal_pag
<a name="cmxsrv_icbr_cal_pag"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → PAGCBR → CBR01006.FRM**: [CMXsrv_get_ult_dia_habil](#referencia-cmxsrv_get_ult_dia_habil)
- **Importaciones → PAGCBR → CBR01006.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → PAGCBR → CBR01006.FRM**: [CMXsrv_icbr_cre_pln](#referencia-cmxsrv_icbr_cre_pln)
- **Importaciones → PAGCBR → CBR01006.FRM**: [CMXsrv_icbr_cal_int](#referencia-cmxsrv_icbr_cal_int)
- **Importaciones → PAGCBR → CBR01006.FRM**: [CMXsrv_valida_tc](#referencia-cmxsrv_valida_tc)

---

## CMXsrv_icbr_eli_pag
<a name="cmxsrv_icbr_eli_pag"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → PAGCBR → CBR01006.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_val_vig
<a name="cmxsrv_val_vig"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → PAGCBR → CBR01006.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_lee_cbr0
<a name="cmxsrv_icbr_lee_cbr0"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → PAGCBR → CBR01006.FRM**: [sp_procxmode](#referencia-sp_procxmode)
- **Importaciones → PAGCBR → CBR01006.FRM**: [CMXsrv_icrd_lee_cln](#referencia-cmxsrv_icrd_lee_cln)

---

## CMXsrv_icbr_obt_mon_nac
<a name="cmxsrv_icbr_obt_mon_nac"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → PAGCBR → CBR01006.FRM**: [CMXsrv_cmx_get_codes](#referencia-cmxsrv_cmx_get_codes)
- **Importaciones → PAGCBR → CBR01006.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_lee_dat_pag
<a name="cmxsrv_icbr_lee_dat_pag"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → PAGCBR → CBR01006.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_pcg_pag
<a name="cmxsrv_icbr_pcg_pag"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → PAGCBR → CBR01006.FRM**: [PrmACMXMONEDAFEC](#referencia-prmacmxmonedafec)
- **Importaciones → PAGCBR → CBR01006.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_busc_pago
<a name="cmxsrv_icbr_busc_pago"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → PAGCBR → CBR01007.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_eli_int_pago
<a name="cmxsrv_icbr_eli_int_pago"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → PAGCBR → COB00305.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_busc_int
<a name="cmxsrv_icbr_busc_int"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → PAGCBR → COB00305.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_ingmod_int
<a name="cmxsrv_icbr_ingmod_int"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → PAGCBR → COB00306.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_lee_int_pago
<a name="cmxsrv_icbr_lee_int_pago"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → PAGCBR → COB00306.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_lee_bco
<a name="cmxsrv_icbr_lee_bco"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → PAGCBR → CRD00602.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_busc_bco
<a name="cmxsrv_icbr_busc_bco"></a>

**Procedimientos Referenciados en los siguientes archivos:**

- **Importaciones → PAGCBR → CRD00602.FRM**: [sp_procxmode](#referencia-sp_procxmode)

---

## Uso de CMXsrv_expcbe_lee_prm
<a name="referencia-cmxsrv_expcbe_lee_prm"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_cmx_busc_suc_usu
<a name="referencia-cmxsrv_cmx_busc_suc_usu"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBE00101.FRM**: CMXsrv_expcbe_lee_cbe
- **Exportaciones → EXPCBE → CBE00301.FRM**: CMXsrv_expcbe_lee_cbe
- **Exportaciones → EXPCBE → CBE00605.FRM**: CMXsrv_expcbe_lee_cbe
- **Exportaciones → EXPCCE → CCE00203.FRM**: CMXsrv_expcce_cre_cce
- **Exportaciones → EXPNEG → CCE00601.FRM**: CMXsrv_expcce_lee_neg
- **Exportaciones → EXPNEG → CCE00901.FRM**: CMXsrv_expcce_grb_neg
- **Exportaciones → expret → RET00101.FRM**: CMXsrv_expret_lee_ret
- **Exportaciones → expret → RET00201.FRM**: CMXsrv_expret_cre_ret

---

## Uso de CMXsrv_expcbe_lee_cbe
<a name="referencia-cmxsrv_expcbe_lee_cbe"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_trae_glo_fec
<a name="referencia-cmxsrv_trae_glo_fec"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBEAVIRE.FRM**: CMXsrv_expcbe_avs_rem1
- **Exportaciones → EXPCCE → CCEAVIRE.FRM**: CMXsrv_expcce_avs_rem1
- **Exportaciones → EXPNEG → CCEAVIRE.FRM**: CMXsrv_expcce_avs_rem1
- **Importaciones → NEGO_AV → AVISOS.FRM**: CMXsrv_icrd_lee_dat_cln
- **Importaciones → NEGO_AV → AVI_COL.FRM**: CMXsrv_col_avi_det_oto

---

## Uso de CMXsrv_expcbe_avs_cyg1
<a name="referencia-cmxsrv_expcbe_avs_cyg1"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_avs_cyg2
<a name="referencia-cmxsrv_expcbe_avs_cyg2"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_avs_ret
<a name="referencia-cmxsrv_expcbe_avs_ret"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_swf_sel
<a name="referencia-cmxsrv_expcbe_swf_sel"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_anl_cbe
<a name="referencia-cmxsrv_expcbe_anl_cbe"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_ctb_ing
<a name="referencia-cmxsrv_expcbe_ctb_ing"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_del_cbe
<a name="referencia-cmxsrv_expcbe_del_cbe"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_val_cbe
<a name="referencia-cmxsrv_expcbe_val_cbe"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBE00101.FRM**: CMXsrv_expcbe_ctb_ing
- **Exportaciones → EXPCBE → CBEAVIRE.FRM**: CMXsrv_expcbe_avs_rem1

---

## Uso de CMXsrv_expcbe_grb_ctp
<a name="referencia-cmxsrv_expcbe_grb_ctp"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_lee_cln
<a name="referencia-cmxsrv_expcbe_lee_cln"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_val_suc
<a name="referencia-cmxsrv_val_suc"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBE00101.FRM**: CMXsrv_expcbe_lee_cbe
- **Exportaciones → EXPCBE → CBE00301.FRM**: CMXsrv_expcbe_lee_cbe
- **Exportaciones → EXPCBE → CBE00605.FRM**: CMXsrv_expcbe_lee_cbe

---

## Uso de CMXsrv_expcbe_lee_ctp
<a name="referencia-cmxsrv_expcbe_lee_ctp"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_grb_bco
<a name="referencia-cmxsrv_expcbe_grb_bco"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_lee_cor
<a name="referencia-cmxsrv_expcbe_lee_cor"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_lee_bco
<a name="referencia-cmxsrv_expcbe_lee_bco"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_grb_doc
<a name="referencia-cmxsrv_expcbe_grb_doc"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_grb_doc02
<a name="referencia-cmxsrv_expcbe_grb_doc02"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_lee_doc
<a name="referencia-cmxsrv_expcbe_lee_doc"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_lee_doc02
<a name="referencia-cmxsrv_expcbe_lee_doc02"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_del_ctz
<a name="referencia-cmxsrv_expcbe_del_ctz"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_bus_ctz
<a name="referencia-cmxsrv_expcbe_bus_ctz"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_grb_ctz
<a name="referencia-cmxsrv_expcbe_grb_ctz"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_mto_ctz
<a name="referencia-cmxsrv_expcbe_mto_ctz"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_lee_ctz
<a name="referencia-cmxsrv_expcbe_lee_ctz"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_bus_cbe
<a name="referencia-cmxsrv_expcbe_bus_cbe"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_mdf_cbe
<a name="referencia-cmxsrv_expcbe_mdf_cbe"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_cre_actz
<a name="referencia-cmxsrv_expcbe_cre_actz"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_lee_mdf
<a name="referencia-cmxsrv_expcbe_lee_mdf"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_pgo_cbe
<a name="referencia-cmxsrv_expcbe_pgo_cbe"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_lee_pgo
<a name="referencia-cmxsrv_expcbe_lee_pgo"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_bus_evz
<a name="referencia-cmxsrv_expcbe_bus_evz"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_rev_cbe
<a name="referencia-cmxsrv_expcbe_rev_cbe"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_lee_evz
<a name="referencia-cmxsrv_expcbe_lee_evz"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_del_dcz
<a name="referencia-cmxsrv_expcbe_del_dcz"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_bus_dcz
<a name="referencia-cmxsrv_expcbe_bus_dcz"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_grb_dcz
<a name="referencia-cmxsrv_expcbe_grb_dcz"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_lee_dcz
<a name="referencia-cmxsrv_expcbe_lee_dcz"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_bus_vto
<a name="referencia-cmxsrv_expcbe_bus_vto"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_avi_dat_cou
<a name="referencia-cmxsrv_avi_dat_cou"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_avs_rem1
<a name="referencia-cmxsrv_expcbe_avs_rem1"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_avs_rem3
<a name="referencia-cmxsrv_expcbe_avs_rem3"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_avs_rem2
<a name="referencia-cmxsrv_expcbe_avs_rem2"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_avs_rem4
<a name="referencia-cmxsrv_expcbe_avs_rem4"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_busc_plz
<a name="referencia-cmxsrv_busc_plz"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_lee_plz
<a name="referencia-cmxsrv_lee_plz"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_cor_busc_pais
<a name="referencia-cmxsrv_cor_busc_pais"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_cor_lee_pais
<a name="referencia-cmxsrv_cor_lee_pais"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_bus_cor
<a name="referencia-cmxsrv_expcbe_bus_cor"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_busc_bco_mtr
<a name="referencia-cmxsrv_busc_bco_mtr"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_grl_fec_serv
<a name="referencia-cmxsrv_grl_fec_serv"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_lee_cce
<a name="referencia-cmxsrv_expcce_lee_cce"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_trd_cce
<a name="referencia-cmxsrv_expcce_trd_cce"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_anl_cce
<a name="referencia-cmxsrv_expcce_anl_cce"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- **Importaciones → MOD_CRD → MOD00603.FRM**: CMXMCRDsrv_icrd_acep_mod_crd

---

## Uso de CMXsrv_expcce_ctb_ing
<a name="referencia-cmxsrv_expcce_ctb_ing"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_del_cce
<a name="referencia-cmxsrv_expcce_del_cce"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_val_cce
<a name="referencia-cmxsrv_expcce_val_cce"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- **Exportaciones → EXPCCE → CCE00101.FRM**: CMXsrv_expcce_ctb_ing

---

## Uso de CMXsrv_expcce_swf_sel
<a name="referencia-cmxsrv_expcce_swf_sel"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_grb_bco
<a name="referencia-cmxsrv_expcce_grb_bco"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_lee_cor
<a name="referencia-cmxsrv_expcce_lee_cor"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_lee_bco
<a name="referencia-cmxsrv_expcce_lee_bco"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_grb_ctp
<a name="referencia-cmxsrv_expcce_grb_ctp"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_lee_cln
<a name="referencia-cmxsrv_expcce_lee_cln"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_lee_ctp
<a name="referencia-cmxsrv_expcce_lee_ctp"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_cre_cce
<a name="referencia-cmxsrv_expcce_cre_cce"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_gen_dcc
<a name="referencia-cmxsrv_expcce_gen_dcc"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_grb_cnd
<a name="referencia-cmxsrv_expcce_grb_cnd"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_util_det_habil
<a name="referencia-cmxsrv_util_det_habil"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- **Financiamiento → PAGOS → COL00301.FRM**: CMXsrv_fincol_efec_calpa
- **Importaciones → MOD_CRD → MOD00603.FRM**: CMXsrv_fincol_efec_calpa

---

## Uso de CMXsrv_expcce_lee_cnd
<a name="referencia-cmxsrv_expcce_lee_cnd"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_trd_cnd
<a name="referencia-cmxsrv_expcce_trd_cnd"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_del_dcc
<a name="referencia-cmxsrv_expcce_del_dcc"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_bus_dcc
<a name="referencia-cmxsrv_expcce_bus_dcc"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_grb_dcc
<a name="referencia-cmxsrv_expcce_grb_dcc"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_lee_dcc
<a name="referencia-cmxsrv_expcce_lee_dcc"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_bus_cce
<a name="referencia-cmxsrv_expcce_bus_cce"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_mdf_cce
<a name="referencia-cmxsrv_expcce_mdf_cce"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_can_mdf
<a name="referencia-cmxsrv_expcce_can_mdf"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- **Exportaciones → EXPCCE → CCE00401.FRM**: CMXsrv_expcce_mdf_cce

---

## Uso de CMXsrv_expcce_lee_mdf
<a name="referencia-cmxsrv_expcce_lee_mdf"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_cnf_cce
<a name="referencia-cmxsrv_expcce_cnf_cce"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_grb_afin
<a name="referencia-cmxsrv_expcce_grb_afin"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_lee_cnf
<a name="referencia-cmxsrv_expcce_lee_cnf"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_lee_afin
<a name="referencia-cmxsrv_expcce_lee_afin"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_trp_cce
<a name="referencia-cmxsrv_expcce_trp_cce"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_lee_trp
<a name="referencia-cmxsrv_expcce_lee_trp"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_bus_evc
<a name="referencia-cmxsrv_expcce_bus_evc"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_rev_cce
<a name="referencia-cmxsrv_expcce_rev_cce"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_lee_evc
<a name="referencia-cmxsrv_expcce_lee_evc"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_avs_rem1
<a name="referencia-cmxsrv_expcce_avs_rem1"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_bus_cor
<a name="referencia-cmxsrv_expcce_bus_cor"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_dex_lee_dex
<a name="referencia-cmxsrv_dex_lee_dex"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_dex_eli_dex
<a name="referencia-cmxsrv_dex_eli_dex"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_dex_act_dex
<a name="referencia-cmxsrv_dex_act_dex"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expdex_cal_fec
<a name="referencia-cmxsrv_expdex_cal_fec"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_dex_lee_cli
<a name="referencia-cmxsrv_dex_lee_cli"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_dex_bus_dex
<a name="referencia-cmxsrv_dex_bus_dex"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_lee_bas
<a name="referencia-cmxsrv_expcce_lee_bas"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_lee_neg
<a name="referencia-cmxsrv_expcce_lee_neg"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_alz_dis
<a name="referencia-cmxsrv_expcce_alz_dis"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_anl_neg
<a name="referencia-cmxsrv_expcce_anl_neg"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_ctb_neg
<a name="referencia-cmxsrv_expcce_ctb_neg"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_del_neg
<a name="referencia-cmxsrv_expcce_del_neg"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_val_neg
<a name="referencia-cmxsrv_expcce_val_neg"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- **Exportaciones → EXPNEG → CCE00601.FRM**: CMXsrv_expcce_ctb_neg

---

## Uso de CMXsrv_expcce_grb_neg
<a name="referencia-cmxsrv_expcce_grb_neg"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_gen_dcn
<a name="referencia-cmxsrv_expcce_gen_dcn"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_avs_rem5
<a name="referencia-cmxsrv_expcce_avs_rem5"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_lee_nge
<a name="referencia-cmxsrv_expcce_lee_nge"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_trd_nge
<a name="referencia-cmxsrv_expcce_trd_nge"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_ini_neg
<a name="referencia-cmxsrv_expcce_ini_neg"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_del_dcn
<a name="referencia-cmxsrv_expcce_del_dcn"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_bus_dcn
<a name="referencia-cmxsrv_expcce_bus_dcn"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_grb_dcn
<a name="referencia-cmxsrv_expcce_grb_dcn"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_lee_dcn
<a name="referencia-cmxsrv_expcce_lee_dcn"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_del_ltr
<a name="referencia-cmxsrv_expcce_del_ltr"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_bus_ltr
<a name="referencia-cmxsrv_expcce_bus_ltr"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_grb_ltr
<a name="referencia-cmxsrv_expcce_grb_ltr"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_lee_ltr
<a name="referencia-cmxsrv_expcce_lee_ltr"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_del_dsn
<a name="referencia-cmxsrv_expcce_del_dsn"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_gen_dsn
<a name="referencia-cmxsrv_expcce_gen_dsn"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- **Exportaciones → EXPCCE → CCE00801.FRM**: CMXsrv_expcce_rev_cce
- **Exportaciones → EXPNEG → CCE00801.FRM**: CMXsrv_expcce_rev_cce

---

## Uso de CMXsrv_expcce_bus_dsn
<a name="referencia-cmxsrv_expcce_bus_dsn"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_chk_dsn
<a name="referencia-cmxsrv_expcce_chk_dsn"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- **Exportaciones → EXPCCE → CCE00801.FRM**: CMXsrv_expcce_rev_cce
- **Exportaciones → EXPNEG → CCE00801.FRM**: CMXsrv_expcce_rev_cce
- **Exportaciones → EXPNEG → CCE00907.FRM**: CMXsrv_expcce_grb_dsn

---

## Uso de CMXsrv_expcce_grb_dsn
<a name="referencia-cmxsrv_expcce_grb_dsn"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- **Exportaciones → EXPNEG → CCE00906.FRM**: CMXsrv_expcce_gen_dsn

---

## Uso de CMXsrv_expcce_lee_dsn
<a name="referencia-cmxsrv_expcce_lee_dsn"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_bus_neg
<a name="referencia-cmxsrv_expcce_bus_neg"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_pgo_neg
<a name="referencia-cmxsrv_expcce_pgo_neg"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_lee_pgo
<a name="referencia-cmxsrv_expcce_lee_pgo"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_avs_rem3
<a name="referencia-cmxsrv_expcce_avs_rem3"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_avs_rem2
<a name="referencia-cmxsrv_expcce_avs_rem2"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_avs_rem4
<a name="referencia-cmxsrv_expcce_avs_rem4"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_swf_sel
<a name="referencia-cmxsrv_expret_swf_sel"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_lee_ret
<a name="referencia-cmxsrv_expret_lee_ret"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_lee_prm
<a name="referencia-cmxsrv_expret_lee_prm"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_avs_cyg1
<a name="referencia-cmxsrv_expret_avs_cyg1"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_avs_cyg2
<a name="referencia-cmxsrv_expret_avs_cyg2"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_avs_liq1
<a name="referencia-cmxsrv_expret_avs_liq1"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_avs_liq2
<a name="referencia-cmxsrv_expret_avs_liq2"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_avs_liq3
<a name="referencia-cmxsrv_expret_avs_liq3"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_val_ret
<a name="referencia-cmxsrv_expret_val_ret"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- **Exportaciones → expret → RET00101.FRM**: CMXsrv_expret_ctb_ing

---

## Uso de CMXsrv_expret_sum_dtn_mn
<a name="referencia-cmxsrv_expret_sum_dtn_mn"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_ctb_ing
<a name="referencia-cmxsrv_expret_ctb_ing"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_del_ret
<a name="referencia-cmxsrv_expret_del_ret"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_avs_adm1
<a name="referencia-cmxsrv_expret_avs_adm1"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_avs_adm2
<a name="referencia-cmxsrv_expret_avs_adm2"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_avs_adm3
<a name="referencia-cmxsrv_expret_avs_adm3"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_act_tpo_cbo
<a name="referencia-cmxsrv_expret_act_tpo_cbo"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_cre_ret
<a name="referencia-cmxsrv_expret_cre_ret"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBE00501.FRM**: CMXsrv_expcbe_pgo_cbe
- **Exportaciones → EXPNEG → CCE01201.FRM**: CMXsrv_expcce_pgo_neg
- **Exportaciones → expret → RET00101.FRM**: CMXsrv_expret_ctb_ing

---

## Uso de CMXsrv_expret_grb_det
<a name="referencia-cmxsrv_expret_grb_det"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBE00501.FRM**: CMXsrv_expcbe_pgo_cbe
- **Exportaciones → EXPNEG → CCE01201.FRM**: CMXsrv_expcce_pgo_neg
- **Exportaciones → expret → RET00101.FRM**: CMXsrv_expret_ctb_ing

---

## Uso de CMXsrv_expret_tpo_cbo
<a name="referencia-cmxsrv_expret_tpo_cbo"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_lee_cln
<a name="referencia-cmxsrv_expret_lee_cln"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_lee_det
<a name="referencia-cmxsrv_expret_lee_det"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_del_org
<a name="referencia-cmxsrv_expret_del_org"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_bus_org
<a name="referencia-cmxsrv_expret_bus_org"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_grb_org
<a name="referencia-cmxsrv_expret_grb_org"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBE00501.FRM**: CMXsrv_expcbe_pgo_cbe
- **Exportaciones → EXPNEG → CCE01201.FRM**: CMXsrv_expcce_pgo_neg
- **Exportaciones → expret → RET00101.FRM**: CMXsrv_expret_ctb_ing

---

## Uso de CMXsrv_expret_mto_org
<a name="referencia-cmxsrv_expret_mto_org"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_lee_org
<a name="referencia-cmxsrv_expret_lee_org"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_vig_lee_cta
<a name="referencia-cmxsrv_vig_lee_cta"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_del_dtn
<a name="referencia-cmxsrv_expret_del_dtn"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_bus_dtn
<a name="referencia-cmxsrv_expret_bus_dtn"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_grb_dtn
<a name="referencia-cmxsrv_expret_grb_dtn"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBE00501.FRM**: CMXsrv_expcbe_pgo_cbe
- **Exportaciones → EXPNEG → CCE01201.FRM**: CMXsrv_expcce_pgo_neg
- **Exportaciones → expret → RET00101.FRM**: CMXsrv_expret_ctb_ing

---

## Uso de CMXsrv_expret_cal_arb
<a name="referencia-cmxsrv_expret_cal_arb"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_mto_dtn
<a name="referencia-cmxsrv_expret_mto_dtn"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_lee_dtn
<a name="referencia-cmxsrv_expret_lee_dtn"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_bus_ret
<a name="referencia-cmxsrv_expret_bus_ret"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_bus_evr
<a name="referencia-cmxsrv_expret_bus_evr"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_rev_ret
<a name="referencia-cmxsrv_expret_rev_ret"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_lee_evr
<a name="referencia-cmxsrv_expret_lee_evr"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finadm_imod_desti
<a name="referencia-cmxsrv_finadm_imod_desti"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finadm_cons_dtip
<a name="referencia-cmxsrv_finadm_cons_dtip"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finadm_imod_ectb
<a name="referencia-cmxsrv_finadm_imod_ectb"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finadm_eli_tipop
<a name="referencia-cmxsrv_finadm_eli_tipop"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finadm_cons_ectb
<a name="referencia-cmxsrv_finadm_cons_ectb"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finadm_imod_itip
<a name="referencia-cmxsrv_finadm_imod_itip"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finadm_cons_itip
<a name="referencia-cmxsrv_finadm_cons_itip"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finadm_lee_tipop
<a name="referencia-cmxsrv_finadm_lee_tipop"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finadm_val_tipop
<a name="referencia-cmxsrv_finadm_val_tipop"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- **Financiamiento → ADMIN → ADM00201.FRM**: CMXsrv_finadm_imod_desti
- **Financiamiento → ADMIN → ADM00202.FRM**: CMXsrv_finadm_imod_ectb
- **Financiamiento → ADMIN → ADM00203.FRM**: CMXsrv_finadm_imod_itip

---

## Uso de CMXsrv_finadm_bus_tipope
<a name="referencia-cmxsrv_finadm_bus_tipope"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_busc_tip_tas
<a name="referencia-cmxsrv_busc_tip_tas"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_ecuo
<a name="referencia-cmxsrv_fincol_ecuo"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_cons_plnpa
<a name="referencia-cmxsrv_fincol_cons_plnpa"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_pertas_val_display
<a name="referencia-cmxsrv_pertas_val_display"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_eava
<a name="referencia-cmxsrv_fincol_eava"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_cons_aval
<a name="referencia-cmxsrv_fincol_cons_aval"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_iava
<a name="referencia-cmxsrv_fincol_iava"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_cons_pag
<a name="referencia-cmxsrv_fincol_cons_pag"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_trae_det_pag
<a name="referencia-cmxsrv_fincol_trae_det_pag"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_cons_pror
<a name="referencia-cmxsrv_fincol_cons_pror"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_cons_eve
<a name="referencia-cmxsrv_fincol_cons_eve"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_bco_swf
<a name="referencia-cmxsrv_icrd_lee_bco_swf"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_busc_bco
<a name="referencia-cmxsrv_icrd_busc_bco"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_vtocre_prov
<a name="referencia-cmxsrv_fincol_vtocre_prov"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_prec_vtocre
<a name="referencia-cmxsrv_fincol_prec_vtocre"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_bus_lcr_bco
<a name="referencia-cmxsrv_icrd_bus_lcr_bco"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_lee_fpro
<a name="referencia-cmxsrv_lee_fpro"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBE00101.FRM**: CMXsrv_expcbe_lee_prm
- **Exportaciones → EXPCBE → CBE00101.FRM**: CMXsrv_expcbe_lee_cbe
- **Exportaciones → EXPCBE → CBE00301.FRM**: CMXsrv_expcbe_lee_cbe
- **Exportaciones → EXPCBE → CBE00401.FRM**: CMXsrv_expcbe_mdf_cbe
- **Exportaciones → EXPCBE → CBE00501.FRM**: CMXsrv_expcbe_lee_pgo
- **Exportaciones → EXPCBE → CBE00601.FRM**: CMXsrv_expcbe_rev_cbe
- **Exportaciones → EXPCBE → CBE00605.FRM**: CMXsrv_expcbe_lee_cbe
- **Exportaciones → expdex → DEX00101.FRM**: CMXsrv_expcbe_lee_prm
- **Exportaciones → expdex → DEX00102.FRM**: CMXsrv_dex_act_dex
- **Exportaciones → expdex → RESPALD2.FRM**: CMXsrv_dex_act_dex
- **Exportaciones → EXPNEG → CBE00601.FRM**: CMXsrv_expcbe_rev_cbe
- **Exportaciones → expret → RET00101.FRM**: CMXsrv_expret_lee_ret
- **Exportaciones → expret → RET00101.FRM**: CMXsrv_expret_lee_prm
- **Exportaciones → expret → RET00101.FRM**: CMXsrv_expret_val_ret
- **Exportaciones → expret → RET00102.FRM**: CMXsrv_expret_val_ret
- **Exportaciones → expret → RET00201.FRM**: CMXsrv_expret_cre_ret
- **Exportaciones → expret → RET00201.FRM**: CMXsrv_expret_tpo_cbo
- **Exportaciones → expret → RET00201.FRM**: CMXsrv_expret_lee_det
- **Financiamiento → INGRESO → COL00102.FRM**: CMXsrv_fincol_ren_fin
- **Financiamiento → INGRESO → COL00103.FRM**: CMXsrv_fincol_ren_fin
- **Financiamiento → INGRESO → COL00105.FRM**: CMXsrv_fincol_ctb_oto
- **Financiamiento → INGRESO → COL00106.FRM**: CMXsrv_fincol_ctb_oto
- **Financiamiento → INGRESO → COL00701.FRM**: CMXsrv_fincol_ctb_novf
- **Financiamiento → OBLIGA → OBL00103.FRM**: CMXsrv_finobl_calc_anu
- **Financiamiento → OBLIGA → OBL00103.FRM**: CMXsrv_finobl_ctb_oto
- **Financiamiento → OBLIGA → OBL00202.FRM**: CMXsrv_finobl_ictb_pag
- **Financiamiento → OBLIGA → OBL00301.FRM**: CMXsrv_finobl_calc_pror
- **Financiamiento → OBLIGA → OBL00401.FRM**: CMXsrv_finobl_ctb_anu
- **Financiamiento → OBLIGA → OBL00402.FRM**: CMXsrv_finobl_calc_anu
- **Financiamiento → OBLIGA → OBL130.FRM**: CMXsrv_finobl_cesion_obl
- **Financiamiento → PAGOS → COL00402.FRM**: CMXsrv_fincol_cont_pror
- **Financiamiento → PAGOS → COL00501.FRM**: CMXsrv_fincol_cctb_anu
- **Financiamiento → PGOEXT → PGOCOL01.FRM**: CMXsrv_fincol_ctb_pext
- **Financiamiento → PGOEXT → PGOOBL01.FRM**: CMXsrv_finobl_ctb_pext

---

## Uso de CMXsrv_fincol_ren_fin
<a name="referencia-cmxsrv_fincol_ren_fin"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_gmod_ctr
<a name="referencia-cmxsrv_fincol_gmod_ctr"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_lee_bco
<a name="referencia-cmxsrv_fincol_lee_bco"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_lee_cln
<a name="referencia-cmxsrv_fincol_lee_cln"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_cons_ctr
<a name="referencia-cmxsrv_fincol_cons_ctr"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_ctb_oto
<a name="referencia-cmxsrv_fincol_ctb_oto"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_dat_liq_ope
<a name="referencia-cmxsrv_icrd_dat_liq_ope"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_lee_col
<a name="referencia-cmxsrv_fincol_lee_col"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_busc_cod_ope
<a name="referencia-cmxsrv_busc_cod_ope"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- **Financiamiento → PAGOS → COL00501.FRM**: CMXsrv_fincol_cctb_anu
- **Importaciones → IMPORT → CRD00202.FRM**: CMXsrv_icrd_a_cnd
- **Importaciones → MOD_ADI → CRD00202.FRM**: CMXsrv_icrd_a_cnd
- **Importaciones → MOD_CRD → CRD00202.FRM**: CMXsrv_icrd_a_cnd

---

## Uso de CMXsrv_col_trae_num_ope
<a name="referencia-cmxsrv_col_trae_num_ope"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_eli_col
<a name="referencia-cmxsrv_fincol_eli_col"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_val_col
<a name="referencia-cmxsrv_fincol_val_col"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- **Financiamiento → INGRESO → COL00105.FRM**: CMXsrv_fincol_ctb_oto
- **Financiamiento → INGRESO → COL00106.FRM**: CMXsrv_fincol_ctb_oto

---

## Uso de CMXsrv_fincol_bsc_col
<a name="referencia-cmxsrv_fincol_bsc_col"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_lee_tip
<a name="referencia-cmxsrv_fincol_lee_tip"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_ctb_novf
<a name="referencia-cmxsrv_fincol_ctb_novf"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_cons_nov
<a name="referencia-cmxsrv_fincol_cons_nov"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_cmx_get_codes
<a name="referencia-cmxsrv_cmx_get_codes"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- **Exportaciones → EXPCCE → CCE00101.FRM**: CMXsrv_expcce_val_cce
- **Exportaciones → EXPCCE → CCE00401.FRM**: CMXsrv_expcce_mdf_cce
- **Exportaciones → EXPNEG → CCE01201.FRM**: CMXsrv_expcce_pgo_neg
- **Financiamiento → PAGOS → COL00402.FRM**: CMXsrv_fincol_cont_pror
- **Importaciones → ARCOS → ARC00101.FRM**: CMXsrv_iarc_act_arc
- **Importaciones → ARCOS → INFO0202.FRM**: CMXsrv_iarc_act_arc
- **Importaciones → COBERIMP → COB00101.FRM**: CMXsrv_icob_lee_pln
- **Importaciones → COBERIMP → COB00101.FRM**: CMXsrv_icob_pag_sop
- **Importaciones → COBERIMP → COB00301.FRM**: CMXsrv_icob_crea_reem
- **Importaciones → COBERIMP → COB00307.FRM**: CMXsrv_icob_pag_sop
- **Importaciones → COBERIMP → COB00501.FRM**: CMXsrv_icob_anu
- **Importaciones → COBERIMP → FORM2.FRM**: CMXsrv_icob_pag_sop
- **Importaciones → DDI → DDI01001.FRM**: CMXsrv_iddi_asoc_ddi
- **Importaciones → INFORME → INFO0101.FRM**: CMXsrv_iinf_val_inf
- **Importaciones → INFORME → INFO0102.FRM**: CMXsrv_iinf_ingmod_inf
- **Importaciones → INFORME → INFO0102.FRM**: CMXsrv_iinf_lee_usd
- **Importaciones → INFORME → INFO0107.FRM**: CMXsrv_iinf_act_tib
- **Importaciones → INFORME → INFO0109.FRM**: CMXsrv_iinf_act_rib
- **Importaciones → INFORME → INFO0111.FRM**: CMXsrv_iinf_ingmod_comp
- **Importaciones → NNEGO → CRD01301.FRM**: CMXsrv_icrd_alz_disc
- **Importaciones → PAGCBR → CBR01006.FRM**: CMXsrv_icbr_ctb_pag
- **Importaciones → PAGCBR → CBR01006.FRM**: CMXsrv_icbr_obt_mon_nac

---

## Uso de CMXsrv_grl_trae_cod_bco
<a name="referencia-cmxsrv_grl_trae_cod_bco"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_cons_tas
<a name="referencia-cmxsrv_fincol_cons_tas"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_efec_tras
<a name="referencia-cmxsrv_fincol_efec_tras"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_cons_trasp
<a name="referencia-cmxsrv_fincol_cons_trasp"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_cons_dtrs
<a name="referencia-cmxsrv_fincol_cons_dtrs"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_cons_deve
<a name="referencia-cmxsrv_fincol_cons_deve"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_cont_gst
<a name="referencia-cmxsrv_fincol_cont_gst"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_cons_gst
<a name="referencia-cmxsrv_fincol_cons_gst"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_cons_dgst
<a name="referencia-cmxsrv_fincol_cons_dgst"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_bsc_tip
<a name="referencia-cmxsrv_fincol_bsc_tip"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_bus_cor
<a name="referencia-cmxsrv_finobl_bus_cor"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_ecuo
<a name="referencia-cmxsrv_finobl_ecuo"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_gpln
<a name="referencia-cmxsrv_finobl_gpln"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_cons_plnpa
<a name="referencia-cmxsrv_finobl_cons_plnpa"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_calc_anu
<a name="referencia-cmxsrv_finobl_calc_anu"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_lee_obl
<a name="referencia-cmxsrv_finobl_lee_obl"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_ctb_oto
<a name="referencia-cmxsrv_finobl_ctb_oto"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_eli_obl
<a name="referencia-cmxsrv_fincol_eli_obl"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_val_obl
<a name="referencia-cmxsrv_finobl_val_obl"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- **Financiamiento → OBLIGA → OBL00103.FRM**: CMXsrv_finobl_ctb_oto

---

## Uso de CMXsrv_finobl_bsc_obl
<a name="referencia-cmxsrv_finobl_bsc_obl"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_ictb_pag
<a name="referencia-cmxsrv_finobl_ictb_pag"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_obt_sdocuo
<a name="referencia-cmxsrv_finobl_obt_sdocuo"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_new_tas
<a name="referencia-cmxsrv_finobl_new_tas"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_cons_pag
<a name="referencia-cmxsrv_finobl_cons_pag"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_cons_detp
<a name="referencia-cmxsrv_finobl_cons_detp"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_calc_pror
<a name="referencia-cmxsrv_finobl_calc_pror"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_cons_pror
<a name="referencia-cmxsrv_finobl_cons_pror"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_cons_dpror
<a name="referencia-cmxsrv_finobl_cons_dpror"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_ctb_anu
<a name="referencia-cmxsrv_finobl_ctb_anu"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_cons_anu
<a name="referencia-cmxsrv_finobl_cons_anu"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_cons_mod
<a name="referencia-cmxsrv_finobl_cons_mod"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_cons_dmod
<a name="referencia-cmxsrv_finobl_cons_dmod"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_rev_eve
<a name="referencia-cmxsrv_finobl_rev_eve"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_cons_eve
<a name="referencia-cmxsrv_finobl_cons_eve"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_cons_deve
<a name="referencia-cmxsrv_finobl_cons_deve"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_eli_ctr
<a name="referencia-cmxsrv_finobl_eli_ctr"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_cons_ctr
<a name="referencia-cmxsrv_finobl_cons_ctr"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_ing_ctr
<a name="referencia-cmxsrv_finobl_ing_ctr"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_cesion_obl
<a name="referencia-cmxsrv_finobl_cesion_obl"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_comgrl_lee_nom_cor
<a name="referencia-cmxsrv_comgrl_lee_nom_cor"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_lee_cln
<a name="referencia-cmxsrv_lee_cln"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_busc_acre
<a name="referencia-cmxsrv_finobl_busc_acre"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_efec_calpa
<a name="referencia-cmxsrv_fincol_efec_calpa"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- **Financiamiento → COL_NEG → CRD01401.FRM**: CMXsrv_fincol_vtocre_prov
- **Financiamiento → PAGOS → COL00401.FRM**: CMXsrv_fincol_calc_pror
- **Financiamiento → PAGOS → COL00501.FRM**: CMXsrv_fincol_calc_anu
- **Financiamiento → PAGOS → COL00502.FRM**: CMXsrv_fincol_calc_anu

---

## Uso de CMXsrv_fincol_cons_detp
<a name="referencia-cmxsrv_fincol_cons_detp"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_calc_pror
<a name="referencia-cmxsrv_fincol_calc_pror"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_cont_pror
<a name="referencia-cmxsrv_fincol_cont_pror"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_cons_dpror
<a name="referencia-cmxsrv_fincol_cons_dpror"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_cctb_anu
<a name="referencia-cmxsrv_fincol_cctb_anu"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_calc_anu
<a name="referencia-cmxsrv_fincol_calc_anu"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_cons_anu
<a name="referencia-cmxsrv_fincol_cons_anu"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_cons_mod
<a name="referencia-cmxsrv_fincol_cons_mod"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_cons_dmod
<a name="referencia-cmxsrv_fincol_cons_dmod"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_cal_pext
<a name="referencia-cmxsrv_fincol_cal_pext"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_ctb_pext
<a name="referencia-cmxsrv_fincol_ctb_pext"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_cal_pext
<a name="referencia-cmxsrv_finobl_cal_pext"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_ctb_pext
<a name="referencia-cmxsrv_finobl_ctb_pext"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iarc_eli_arc
<a name="referencia-cmxsrv_iarc_eli_arc"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iarc_busc_arc
<a name="referencia-cmxsrv_iarc_busc_arc"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_busc_inf
<a name="referencia-cmxsrv_iinf_busc_inf"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iarc_act_arc
<a name="referencia-cmxsrv_iarc_act_arc"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iarc_lee_arc
<a name="referencia-cmxsrv_iarc_lee_arc"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_busc_opr
<a name="referencia-cmxsrv_iinf_busc_opr"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_lee_vlr
<a name="referencia-cmxsrv_iinf_lee_vlr"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_rev_evi
<a name="referencia-cmxsrv_iinf_rev_evi"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icob_lee_pln
<a name="referencia-cmxsrv_icob_lee_pln"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icob_cur_cob
<a name="referencia-cmxsrv_icob_cur_cob"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icob_pag_sop
<a name="referencia-cmxsrv_icob_pag_sop"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icob_eli_pln
<a name="referencia-cmxsrv_icob_eli_pln"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icob_rev_etd
<a name="referencia-cmxsrv_icob_rev_etd"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icob_val_cob
<a name="referencia-cmxsrv_icob_val_cob"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- **Importaciones → COBERIMP → COB00101.FRM**: CMXsrv_icob_cur_cob
- **Importaciones → COBERIMP → COB00101.FRM**: CMXsrv_icob_pag_sop
- **Importaciones → COBERIMP → COB00302.FRM**: CMXsrv_icob_act_gral
- **Importaciones → COBERIMP → COB00303.FRM**: CMXsrv_icob_act_val
- **Importaciones → COBERIMP → COB00304.FRM**: CMXsrv_icob_act_acu
- **Importaciones → COBERIMP → COB00306.FRM**: CMXsrv_icob_ingmod_int
- **Importaciones → COBERIMP → COB00307.FRM**: CMXsrv_icob_pag_sop
- **Importaciones → COBERIMP → FORM2.FRM**: CMXsrv_icob_pag_sop
- **Importaciones → COBERIMP → ORI_DEST.FRM**: CMXsrv_icob_cur_reem
- **Importaciones → PAGCBR → COB00303.FRM**: CMXsrv_icob_act_val

---

## Uso de CMXsrv_icob_busc_pln
<a name="referencia-cmxsrv_icob_busc_pln"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icob_lee_cln
<a name="referencia-cmxsrv_icob_lee_cln"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icob_crea_norm
<a name="referencia-cmxsrv_icob_crea_norm"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icob_crea_reem
<a name="referencia-cmxsrv_icob_crea_reem"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icob_act_gral
<a name="referencia-cmxsrv_icob_act_gral"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icob_lee_cln2
<a name="referencia-cmxsrv_icob_lee_cln2"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icob_lee_gral
<a name="referencia-cmxsrv_icob_lee_gral"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icob_act_val
<a name="referencia-cmxsrv_icob_act_val"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icob_lee_val
<a name="referencia-cmxsrv_icob_lee_val"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icob_act_acu
<a name="referencia-cmxsrv_icob_act_acu"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icob_lee_acu
<a name="referencia-cmxsrv_icob_lee_acu"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icob_eli_int
<a name="referencia-cmxsrv_icob_eli_int"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icob_busc_int
<a name="referencia-cmxsrv_icob_busc_int"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icob_ingmod_int
<a name="referencia-cmxsrv_icob_ingmod_int"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icob_lee_int
<a name="referencia-cmxsrv_icob_lee_int"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icob_ing_mod_srf
<a name="referencia-cmxsrv_icob_ing_mod_srf"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icob_anu
<a name="referencia-cmxsrv_icob_anu"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icob_lee_anu
<a name="referencia-cmxsrv_icob_lee_anu"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icob_cur_reem
<a name="referencia-cmxsrv_icob_cur_reem"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_busc_cor_swf
<a name="referencia-cmxsrv_busc_cor_swf"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_swf_bus_sms
<a name="referencia-cmxsrv_swf_bus_sms"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_lee_cbr
<a name="referencia-cmxsrv_icbr_lee_cbr"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_acep_let
<a name="referencia-cmxsrv_icbr_acep_let"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_cont_cbr
<a name="referencia-cmxsrv_icbr_cont_cbr"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_eli_cbr
<a name="referencia-cmxsrv_icbr_eli_cbr"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_lee_ctp
<a name="referencia-cmxsrv_icbr_lee_ctp"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_avi1
<a name="referencia-cmxsrv_icbr_avi1"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_busc_cbr
<a name="referencia-cmxsrv_icbr_busc_cbr"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_lee_cln
<a name="referencia-cmxsrv_icbr_lee_cln"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_crea_cbr
<a name="referencia-cmxsrv_icbr_crea_cbr"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_lee_cob
<a name="referencia-cmxsrv_icbr_lee_cob"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_act_ctp
<a name="referencia-cmxsrv_icbr_act_ctp"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_lee_trm
<a name="referencia-cmxsrv_icbr_lee_trm"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_act_trm
<a name="referencia-cmxsrv_icbr_act_trm"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_lee_doc
<a name="referencia-cmxsrv_icbr_lee_doc"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_act_doc
<a name="referencia-cmxsrv_icbr_act_doc"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_busc_let
<a name="referencia-cmxsrv_icbr_busc_let"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_ingmod_let
<a name="referencia-cmxsrv_icbr_ingmod_let"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_eli_let
<a name="referencia-cmxsrv_icbr_eli_let"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_lee_let
<a name="referencia-cmxsrv_icbr_lee_let"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_prorr
<a name="referencia-cmxsrv_icbr_prorr"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_rev_eve
<a name="referencia-cmxsrv_icbr_rev_eve"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_busc_eve
<a name="referencia-cmxsrv_icbr_busc_eve"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_lee_eve
<a name="referencia-cmxsrv_icbr_lee_eve"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_lee_ent_doc
<a name="referencia-cmxsrv_icbr_lee_ent_doc"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_prot
<a name="referencia-cmxsrv_icbr_prot"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_pcg_prot
<a name="referencia-cmxsrv_icbr_pcg_prot"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_liq_sdo
<a name="referencia-cmxsrv_icbr_liq_sdo"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_act_vis
<a name="referencia-cmxsrv_icbr_act_vis"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_eli_rep
<a name="referencia-cmxsrv_icbr_eli_rep"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_busc_rep
<a name="referencia-cmxsrv_icbr_busc_rep"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_imod_rep
<a name="referencia-cmxsrv_icbr_imod_rep"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_ent_doc
<a name="referencia-cmxsrv_icbr_ent_doc"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_trf_ofi
<a name="referencia-cmxsrv_icbr_trf_ofi"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_trf_bco
<a name="referencia-cmxsrv_icbr_trf_bco"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_act_inst
<a name="referencia-cmxsrv_icbr_act_inst"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iswf_a_pru
<a name="referencia-cmxsrv_iswf_a_pru"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_val_cbr
<a name="referencia-cmxsrv_icbr_val_cbr"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- **Importaciones → COBRANZA → CBR00101.FRM**: CMXsrv_icbr_cont_cbr
- **Importaciones → COBRANZA → CBR00202.FRM**: CMXsrv_icbr_act_trm
- **Importaciones → MOD_CBR → CBR00202.FRM**: CMXsrv_icbr_act_trm
- **Importaciones → MOD_CBR → PANBASE.FRM**: CMXsrv_icbr_acep_mod_cbr

---

## Uso de CMXsrv_icrd_a_ibab
<a name="referencia-cmxsrv_icrd_a_ibab"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_glo_ibab
<a name="referencia-cmxsrv_icrd_lee_glo_ibab"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_a_ibar
<a name="referencia-cmxsrv_icrd_a_ibar"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_glo_ibar
<a name="referencia-cmxsrv_icrd_lee_glo_ibar"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_tex_swf
<a name="referencia-cmxsrv_icrd_lee_tex_swf"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_cod_txt_swf
<a name="referencia-cmxsrv_icrd_lee_cod_txt_swf"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_txt_swf_all
<a name="referencia-cmxsrv_icrd_lee_txt_swf_all"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_ind_esp_ing
<a name="referencia-cmxsrv_icrd_lee_ind_esp_ing"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_ing_acu
<a name="referencia-cmxsrv_icrd_ing_acu"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_acu
<a name="referencia-cmxsrv_icrd_lee_acu"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_rech_sol
<a name="referencia-cmxsrv_icrd_rech_sol"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_end
<a name="referencia-cmxsrv_icrd_end"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_dat_end
<a name="referencia-cmxsrv_icrd_lee_dat_end"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_asignar_cor
<a name="referencia-cmxsrv_icrd_asignar_cor"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- **Importaciones → IMPORT → CRD0063.FRM**: CMXCRDsrv_icrd_apr_sol

---

## Uso de CMXsrv_icrd_lee_bco_mtr
<a name="referencia-cmxsrv_icrd_lee_bco_mtr"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_cor_lee_pais
<a name="referencia-cmxsrv_icrd_cor_lee_pais"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_plz
<a name="referencia-cmxsrv_icrd_lee_plz"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_busc_plz
<a name="referencia-cmxsrv_icrd_busc_plz"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_cor_busc_pais
<a name="referencia-cmxsrv_icrd_cor_busc_pais"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_busc_bco_mtr
<a name="referencia-cmxsrv_icrd_busc_bco_mtr"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iddi_ingmod_ddi
<a name="referencia-cmxsrv_iddi_ingmod_ddi"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iddi_lee_dec
<a name="referencia-cmxsrv_iddi_lee_dec"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iddi_eli_ddi
<a name="referencia-cmxsrv_iddi_eli_ddi"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iddi_lee_inf
<a name="referencia-cmxsrv_iddi_lee_inf"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iddi_lee_cln
<a name="referencia-cmxsrv_iddi_lee_cln"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iddi_lee_rut
<a name="referencia-cmxsrv_iddi_lee_rut"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iddi_asoc_ddi
<a name="referencia-cmxsrv_iddi_asoc_ddi"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iddi_des_ddi
<a name="referencia-cmxsrv_iddi_des_ddi"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iddi_busc_asoc
<a name="referencia-cmxsrv_iddi_busc_asoc"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iddi_busc_noasoc
<a name="referencia-cmxsrv_iddi_busc_noasoc"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_dir_cln
<a name="referencia-cmxsrv_icrd_lee_dir_cln"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXCRDsrv_icrd_a_cnd_esp
<a name="referencia-cmxcrdsrv_icrd_a_cnd_esp"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_cnd_esp
<a name="referencia-cmxsrv_icrd_lee_cnd_esp"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXCRDsrv_icrd_clon_crd
<a name="referencia-cmxcrdsrv_icrd_clon_crd"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXCRDsrv_icrd_lee_crdcre
<a name="referencia-cmxcrdsrv_icrd_lee_crdcre"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_top
<a name="referencia-cmxsrv_icrd_lee_top"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXCRDsrv_icrd_val_crd
<a name="referencia-cmxcrdsrv_icrd_val_crd"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- **Importaciones → MOD_CRD → MOD00603.FRM**: CMXMCRDsrv_icrd_acep_mod_crd

---

## Uso de CMXCRDsrv_icrd_eli_crd
<a name="referencia-cmxcrdsrv_icrd_eli_crd"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_dat_trs
<a name="referencia-cmxsrv_icrd_lee_dat_trs"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_a_ctp
<a name="referencia-cmxsrv_icrd_a_ctp"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_cln
<a name="referencia-cmxsrv_icrd_lee_cln"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- **Exportaciones → EXPCBE → CBE00202.FRM**: CMXsrv_expcbe_lee_bco
- **Financiamiento → COL_NEG → CRD00602.FRM**: CMXsrv_icrd_lee_bco_swf
- **Financiamiento → INGRESO → COL00104.FRM**: CMXsrv_icrd_lee_bco_swf
- **Financiamiento → INGRESO → CRD00602.FRM**: CMXsrv_icrd_lee_bco_swf
- **Importaciones → MOD_ADI → CRD00202.FRM**: CMXsrv_icrd_lee_bco_swf
- **Importaciones → MOD_CRD → CRD00205.FRM**: CMXsrv_icrd_lee_bco_swf
- **Importaciones → MOD_CRD → MOD00603.FRM**: CMXsrv_icrd_lee_bco_swf
- **Importaciones → PAGCBR → CBR01006.FRM**: CMXsrv_icbr_lee_cbr0

---

## Uso de CMXsrv_icrd_a_cnd
<a name="referencia-cmxsrv_icrd_a_cnd"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXCRDsrv_icrd_crea_crd
<a name="referencia-cmxcrdsrv_icrd_crea_crd"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_busc_emb
<a name="referencia-cmxsrv_icrd_busc_emb"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_eli_emb
<a name="referencia-cmxsrv_icrd_eli_emb"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_emb1
<a name="referencia-cmxsrv_icrd_lee_emb1"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_emb2
<a name="referencia-cmxsrv_icrd_lee_emb2"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_a_emb1
<a name="referencia-cmxsrv_icrd_a_emb1"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_a_emb2
<a name="referencia-cmxsrv_icrd_a_emb2"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_val_emb2
<a name="referencia-cmxsrv_icrd_val_emb2"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_val_emb1
<a name="referencia-cmxsrv_icrd_val_emb1"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_act_ref
<a name="referencia-cmxsrv_icrd_act_ref"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_ref
<a name="referencia-cmxsrv_icrd_lee_ref"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXCRDsrv_icrd_apr_sol
<a name="referencia-cmxcrdsrv_icrd_apr_sol"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_crdapr
<a name="referencia-cmxsrv_icrd_lee_crdapr"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXCRDsrv_icrd_a_desc_merc
<a name="referencia-cmxcrdsrv_icrd_a_desc_merc"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_desc_merc
<a name="referencia-cmxsrv_icrd_lee_desc_merc"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_a_otr_doc
<a name="referencia-cmxsrv_icrd_a_otr_doc"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_otr_doc
<a name="referencia-cmxsrv_icrd_lee_otr_doc"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_lee0_inf
<a name="referencia-cmxsrv_iinf_lee0_inf"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_lee_tablas
<a name="referencia-cmxsrv_iinf_lee_tablas"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_lee1_inf
<a name="referencia-cmxsrv_iinf_lee1_inf"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_lee_cln
<a name="referencia-cmxsrv_iinf_lee_cln"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_lee2_inf
<a name="referencia-cmxsrv_iinf_lee2_inf"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_avi_miscb
<a name="referencia-cmxsrv_iinf_avi_miscb"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_avi_misca
<a name="referencia-cmxsrv_iinf_avi_misca"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_dat_com
<a name="referencia-cmxsrv_icrd_lee_dat_com"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_eli_inf
<a name="referencia-cmxsrv_iinf_eli_inf"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_busc_evi
<a name="referencia-cmxsrv_iinf_busc_evi"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_val_inf
<a name="referencia-cmxsrv_iinf_val_inf"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- **Importaciones → INFORME → INFO0102.FRM**: CMXsrv_iinf_ingmod_inf
- **Importaciones → INFORME → INFO0104.FRM**: CMXsrv_iinf_act_apr
- **Importaciones → INFORME → INFO0111.FRM**: CMXsrv_iinf_ingmod_comp

---

## Uso de CMXsrv_iinf_ingmod_inf
<a name="referencia-cmxsrv_iinf_ingmod_inf"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_lee_fec
<a name="referencia-cmxsrv_iinf_lee_fec"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_lee_usd
<a name="referencia-cmxsrv_iinf_lee_usd"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_act_apr
<a name="referencia-cmxsrv_iinf_act_apr"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_lee_evi
<a name="referencia-cmxsrv_iinf_lee_evi"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_act_tib
<a name="referencia-cmxsrv_iinf_act_tib"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_act_rec
<a name="referencia-cmxsrv_iinf_act_rec"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_act_rib
<a name="referencia-cmxsrv_iinf_act_rib"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_busc_comp
<a name="referencia-cmxsrv_iinf_busc_comp"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_ingmod_comp
<a name="referencia-cmxsrv_iinf_ingmod_comp"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_lee_comp
<a name="referencia-cmxsrv_iinf_lee_comp"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_lee_bco
<a name="referencia-cmxsrv_iinf_lee_bco"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_busc_bco
<a name="referencia-cmxsrv_iinf_busc_bco"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXMCRDsrv_icrd_lee_mcnd
<a name="referencia-cmxmcrdsrv_icrd_lee_mcnd"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_mod_ing_let
<a name="referencia-cmxsrv_icbr_mod_ing_let"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_acep_mod_cbr
<a name="referencia-cmxsrv_icbr_acep_mod_cbr"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_eli_no_cont
<a name="referencia-cmxsrv_icbr_eli_no_cont"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXMCRDsrv_icrd_a_mmcnd
<a name="referencia-cmxmcrdsrv_icrd_a_mmcnd"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXMCRDsrv_icrd_lee_mctp
<a name="referencia-cmxmcrdsrv_icrd_lee_mctp"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXMCRDsrv_icrd_lee_memb2
<a name="referencia-cmxmcrdsrv_icrd_lee_memb2"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXMCRDsrv_icrd_lee_memb1
<a name="referencia-cmxmcrdsrv_icrd_lee_memb1"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXMCRDsrv_icrd_lee_mref
<a name="referencia-cmxmcrdsrv_icrd_lee_mref"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_ing_txt
<a name="referencia-cmxsrv_icrd_ing_txt"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXCRDsrv_icrd_get_ing_esp
<a name="referencia-cmxcrdsrv_icrd_get_ing_esp"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXMCRDsrv_icrd_lee_mtxt
<a name="referencia-cmxmcrdsrv_icrd_lee_mtxt"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXCRDsrv_icrd_get_pre_fra
<a name="referencia-cmxcrdsrv_icrd_get_pre_fra"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXMCRDsrv_icrd_a_mmer
<a name="referencia-cmxmcrdsrv_icrd_a_mmer"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_lee_cod_eve
<a name="referencia-cmxsrv_fincol_lee_cod_eve"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXMCRDsrv_icrd_acep_mod_crd
<a name="referencia-cmxmcrdsrv_icrd_acep_mod_crd"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXMCRDsrv_icrd_eli_no_cont
<a name="referencia-cmxmcrdsrv_icrd_eli_no_cont"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- **Importaciones → MOD_CRD → MOD00603.FRM**: CMXMCRDsrv_icrd_acep_mod_crd

---

## Uso de CMXsrv_icrd_a_rec_age
<a name="referencia-cmxsrv_icrd_a_rec_age"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_busc_ofi_cta
<a name="referencia-cmxsrv_busc_ofi_cta"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_neg_busc_arc
<a name="referencia-cmxsrv_neg_busc_arc"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_avi_adi
<a name="referencia-cmxsrv_icrd_lee_avi_adi"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_dat_cln
<a name="referencia-cmxsrv_icrd_lee_dat_cln"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_avi_dis
<a name="referencia-cmxsrv_icrd_lee_avi_dis"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_neg_ddi_asoc
<a name="referencia-cmxsrv_neg_ddi_asoc"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_neg_trae_vcto_mcf
<a name="referencia-cmxsrv_neg_trae_vcto_mcf"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_neg_avi_lee_aval
<a name="referencia-cmxsrv_neg_avi_lee_aval"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_neg_lee_crd
<a name="referencia-cmxsrv_icrd_neg_lee_crd"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_neg
<a name="referencia-cmxsrv_icrd_lee_neg"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_col_avi_dat_cln
<a name="referencia-cmxsrv_col_avi_dat_cln"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_col_avi_det_pag
<a name="referencia-cmxsrv_col_avi_det_pag"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_col_avi_det_oto
<a name="referencia-cmxsrv_col_avi_det_oto"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_col_lee_num_trs
<a name="referencia-cmxsrv_col_lee_num_trs"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_avi_pag
<a name="referencia-cmxsrv_finobl_avi_pag"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_neg_avi_trae_asnd_mn
<a name="referencia-cmxsrv_neg_avi_trae_asnd_mn"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_neg_avi_trae_asnd_mx
<a name="referencia-cmxsrv_neg_avi_trae_asnd_mx"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_cont_neg
<a name="referencia-cmxsrv_icrd_cont_neg"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_eli_neg
<a name="referencia-cmxsrv_icrd_eli_neg"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_num_col
<a name="referencia-cmxsrv_icrd_lee_num_col"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_bus_pago
<a name="referencia-cmxsrv_icrd_bus_pago"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_col
<a name="referencia-cmxsrv_icrd_lee_col"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_busc_neg
<a name="referencia-cmxsrv_icrd_busc_neg"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_a_neg_emb1
<a name="referencia-cmxsrv_icrd_a_neg_emb1"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_a_neg_emb2
<a name="referencia-cmxsrv_icrd_a_neg_emb2"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_eli_doc_neg
<a name="referencia-cmxsrv_icrd_eli_doc_neg"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_neg_emb1
<a name="referencia-cmxsrv_icrd_lee_neg_emb1"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_neg_emb2
<a name="referencia-cmxsrv_icrd_lee_neg_emb2"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_a_neg_disc
<a name="referencia-cmxsrv_icrd_a_neg_disc"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_neg_lee_disc
<a name="referencia-cmxsrv_icrd_neg_lee_disc"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_ent_doc
<a name="referencia-cmxsrv_icrd_ent_doc"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_alz_disc
<a name="referencia-cmxsrv_icrd_alz_disc"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXCRDsrv_icrd_asignar_cor
<a name="referencia-cmxcrdsrv_icrd_asignar_cor"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXCRDsrv_icrd_bus_lcr_bco
<a name="referencia-cmxcrdsrv_icrd_bus_lcr_bco"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_act_doc_neg
<a name="referencia-cmxsrv_icrd_act_doc_neg"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_doc_neg
<a name="referencia-cmxsrv_icrd_lee_doc_neg"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_val_neg
<a name="referencia-cmxsrv_icrd_val_neg"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- **Importaciones → NEGO_AV → CRD01001.FRM**: CMXsrv_icrd_cont_neg
- **Importaciones → NNEGO → CRD01001.FRM**: CMXsrv_icrd_cont_neg

---

## Uso de CMXsrv_icbr_lee_dat_var
<a name="referencia-cmxsrv_icbr_lee_dat_var"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_val_pag
<a name="referencia-cmxsrv_icbr_val_pag"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_ctb_pag
<a name="referencia-cmxsrv_icbr_ctb_pag"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_cal_pag
<a name="referencia-cmxsrv_icbr_cal_pag"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_eli_pag
<a name="referencia-cmxsrv_icbr_eli_pag"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_val_vig
<a name="referencia-cmxsrv_val_vig"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- **Exportaciones → expret → RET00101.FRM**: CMXsrv_expret_val_ret
- **Exportaciones → expret → RET00102.FRM**: CMXsrv_expret_val_ret

---

## Uso de CMXsrv_icbr_lee_cbr0
<a name="referencia-cmxsrv_icbr_lee_cbr0"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_obt_mon_nac
<a name="referencia-cmxsrv_icbr_obt_mon_nac"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_lee_dat_pag
<a name="referencia-cmxsrv_icbr_lee_dat_pag"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_pcg_pag
<a name="referencia-cmxsrv_icbr_pcg_pag"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_busc_pago
<a name="referencia-cmxsrv_icbr_busc_pago"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_eli_int_pago
<a name="referencia-cmxsrv_icbr_eli_int_pago"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_busc_int
<a name="referencia-cmxsrv_icbr_busc_int"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_ingmod_int
<a name="referencia-cmxsrv_icbr_ingmod_int"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_lee_int_pago
<a name="referencia-cmxsrv_icbr_lee_int_pago"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_lee_bco
<a name="referencia-cmxsrv_icbr_lee_bco"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_busc_bco
<a name="referencia-cmxsrv_icbr_busc_bco"></a>

**Este procedimiento es invocado en los siguientes archivos:**

- No se encontraron referencias.

---

