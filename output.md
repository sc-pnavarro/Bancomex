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

| **Segmento** | **Procedimiento Almacenado** | **Tabla Referenciada** |
|-------------|-----------------------------|----------------------|
| Form_Activate | [CMXsrv_expcbe_lee_prm](#cmxsrv_expcbe_lee_prm) | ACMXPRMGRL |
| Form_Activate | [CMXsrv_cmx_busc_suc_usu](#cmxsrv_cmx_busc_suc_usu) | master..sysprocesses, tbl_User |
| Form_Activate | [CMXsrv_expcbe_lee_cbe](#cmxsrv_expcbe_lee_cbe) | ACMXPAIS, COR, ACMXPGOCBE, CBE01, CBE, ACMXMONEDA, ACMXENTDOC, ACMXSUCSAL, ACMXPRTCBE, CLN |
| Form_Load | [CMXsrv_trae_glo_fec](#cmxsrv_trae_glo_fec) | ACMXSUCSAL, ACMXDL3475FEC, tbl_User |
| ingcomg_Click | [CMXsrv_expcbe_avs_cyg1](#cmxsrv_expcbe_avs_cyg1) | ACMXDESEMB, ASND, ACMXIMPUES, ACMXPRMGRL, EVZ, CBE, COM, TRSD, CLN, ACMXESPECI |
| ingcomg_Click | [CMXsrv_expcbe_avs_cyg2](#cmxsrv_expcbe_avs_cyg2) | ASND, ACMXIMPUES, ACMXPRMGRL, EVZ, CBE |
| ingret_Click | [CMXsrv_expcbe_avs_ret](#cmxsrv_expcbe_avs_ret) | ACMXPAIS, COR, ACMXDESEMB, CBE, ACMXMONEDA, ACMXSUCSAL, CLN, ACMXESPECI, RET |
| M3_Click | [CMXsrv_expcbe_swf_sel](#cmxsrv_expcbe_swf_sel) | switxt, switxt1 |
| M4_Click | [CMXsrv_expcbe_swf_sel](#cmxsrv_expcbe_swf_sel) | switxt, switxt1 |
| Mcbeanl_Click | [CMXsrv_expcbe_anl_cbe](#cmxsrv_expcbe_anl_cbe) | CBE |
| Mcbectb_Click | [CMXsrv_expcbe_ctb_ing](#cmxsrv_expcbe_ctb_ing) | OPE_BCI, CBE |
| Mcbedel_Click | [CMXsrv_expcbe_del_cbe](#cmxsrv_expcbe_del_cbe) | EVL, CBE01, COD, CBE, EVZ, COM, ACTZ, CTZ |
| Mcbeval_Click | [CMXsrv_expcbe_val_cbe](#cmxsrv_expcbe_val_cbe) | COR, CBE01, ACMXPRMGRL, CBE, DCZ, CTZ, warnmsg, ACMXPAIS, ACMXFERIADO, CCO |
| Men1_Click | [CMXsrv_expcbe_swf_sel](#cmxsrv_expcbe_swf_sel) | switxt, switxt1 |
| aceptar_Click | [CMXsrv_expcbe_grb_ctp](#cmxsrv_expcbe_grb_ctp) | ACMXPAIS, CBE |
| fld_cbe_cod_exp_lostfocus | [CMXsrv_expcbe_lee_cln](#cmxsrv_expcbe_lee_cln) | CLN |
| fld_cbe_cod_suc_LostFocus | [CMXsrv_val_suc](#cmxsrv_val_suc) | ACMXSUCSAL, tbl_User |
| Form_Activate | [CMXsrv_expcbe_lee_ctp](#cmxsrv_expcbe_lee_ctp) | ACMXSUCSAL, ACMXPAIS, CBE, CLN |
| aceptar_Click | [CMXsrv_expcbe_grb_bco](#cmxsrv_expcbe_grb_bco) | ACMXPRMGRL, CBE, COR, CBE01 |
| fld_cbe_cod_cob_Lostfocus | [CMXsrv_expcbe_lee_cor](#cmxsrv_expcbe_lee_cor) | ACMXPAIS, COR |
| fld_cbe_cod_rmb_LostFocus | [CMXsrv_expcbe_lee_cor](#cmxsrv_expcbe_lee_cor) | ACMXPAIS, COR |
| Form_Activate | [CMXsrv_expcbe_lee_bco](#cmxsrv_expcbe_lee_bco) | CBE, COR, CBE01 |
| aceptar_Click | [CMXsrv_expcbe_grb_doc](#cmxsrv_expcbe_grb_doc) | CBE, DCZ |
| aceptar_Click | [CMXsrv_expcbe_grb_doc02](#cmxsrv_expcbe_grb_doc02) | CBE02 |
| Form_Activate | [CMXsrv_expcbe_lee_doc](#cmxsrv_expcbe_lee_doc) | CBE |
| Form_Activate | [CMXsrv_expcbe_lee_doc02](#cmxsrv_expcbe_lee_doc02) | CBE02 |
| ELIMINAR_Click | [CMXsrv_expcbe_del_ctz](#cmxsrv_expcbe_del_ctz) | ACTZ, CBE, CTZ |
| Form_Activate | [CMXsrv_expcbe_bus_ctz](#cmxsrv_expcbe_bus_ctz) | ACTZ, CBE, CTZ |
| aceptar_Click | [CMXsrv_expcbe_grb_ctz](#cmxsrv_expcbe_grb_ctz) | ACTZ, CBE, CTZ |
| Form_Activate | [CMXsrv_expcbe_mto_ctz](#cmxsrv_expcbe_mto_ctz) | ACTZ, CBE, CTZ |
| Form_Activate | [CMXsrv_expcbe_lee_ctz](#cmxsrv_expcbe_lee_ctz) | ACTZ, CBE, CTZ |
| aceptar_Click | [CMXsrv_expcbe_lee_cbe](#cmxsrv_expcbe_lee_cbe) | ACMXPAIS, COR, ACMXPGOCBE, CBE01, CBE, ACMXMONEDA, ACMXENTDOC, ACMXSUCSAL, ACMXPRTCBE, CLN |
| buscar_Click | [CMXsrv_expcbe_bus_cbe](#cmxsrv_expcbe_bus_cbe) | CBE |
| fld_aux_cod_exp_LostFocus | [CMXsrv_expcbe_lee_cln](#cmxsrv_expcbe_lee_cln) | CLN |
| Proximas_Click | [CMXsrv_expcbe_bus_cbe](#cmxsrv_expcbe_bus_cbe) | CBE |
| aceptar_Click | [CMXsrv_expcbe_mdf_cbe](#cmxsrv_expcbe_mdf_cbe) | ACTZ, ACMXPRMGRL, CBE |
| aceptar_Click | [CMXsrv_expcbe_cre_actz](#cmxsrv_expcbe_cre_actz) | ACTZ, CBE, CTZ |
| fld_cbe_cod_suc_LostFocus | [CMXsrv_val_suc](#cmxsrv_val_suc) | ACMXSUCSAL, tbl_User |
| Form_Activate | [CMXsrv_expcbe_lee_mdf](#cmxsrv_expcbe_lee_mdf) | COR, ACMXPGOCBE, CBE01, CBE, ACMXMONEDA, ACMXSUCSAL, CLN |
| aceptar_Click | [CMXsrv_expcbe_pgo_cbe](#cmxsrv_expcbe_pgo_cbe) | ACMXDESEMB, COR, CLN, RET, vig_cmx, COD, ACMXIMPUES, ACMXPRMGRL, CBE, ACMXPRMEXP, COM, tbl_User, OPREC, ACMXPAIS, ACMXFERIADO, CCO |
| fld_cbe_cod_rmb_LostFocus | [CMXsrv_expcbe_lee_cor](#cmxsrv_expcbe_lee_cor) | ACMXPAIS, COR |
| Form_Activate | [CMXsrv_expcbe_lee_pgo](#cmxsrv_expcbe_lee_pgo) | ACMXDESEMB, COR, CBE, ACMXPRMEXP, ACMXMONEDA, OPREC, CLN |
| Form_Activate | [CMXsrv_expcbe_bus_evz](#cmxsrv_expcbe_bus_evz) | EVZ, CBE |
| Proximo_Click | [CMXsrv_expcbe_bus_evz](#cmxsrv_expcbe_bus_evz) | EVZ, CBE |
| Reversar_Click | [CMXsrv_expcbe_rev_cbe](#cmxsrv_expcbe_rev_cbe) | EVL, ACMXDESEMB, COR, ORG, ACMXIMPUES, ACMXPRMGRL, EVZ, CBE, TRSD, ACMXPRMEXP, COM, EVR, CTZ, DTN, OPREC, RET, PUCBCX10 |
| Form_Activate | [CMXsrv_expcbe_lee_evz](#cmxsrv_expcbe_lee_evz) | ACMXDESEMB, COR, ACMXPGOCBE, EVZ, CBE, ACMXMONEDA, ACMXTIPEVE, ACMXSUCSAL |
| Eliminar_Click | [CMXsrv_expcbe_del_dcz](#cmxsrv_expcbe_del_dcz) | CBE02, CBE, DCZ |
| Form_Activate | [CMXsrv_expcbe_bus_dcz](#cmxsrv_expcbe_bus_dcz) | DCZ |
| aceptar_Click | [CMXsrv_expcbe_grb_dcz](#cmxsrv_expcbe_grb_dcz) | CBE02, CBE, DCZ |
| Form_Activate | [CMXsrv_expcbe_lee_dcz](#cmxsrv_expcbe_lee_dcz) | DCZ |
| aceptar_Click | [CMXsrv_expcbe_lee_cbe](#cmxsrv_expcbe_lee_cbe) | ACMXPAIS, COR, ACMXPGOCBE, CBE01, CBE, ACMXMONEDA, ACMXENTDOC, ACMXSUCSAL, ACMXPRTCBE, CLN |
| buscar_Click | [CMXsrv_expcbe_bus_vto](#cmxsrv_expcbe_bus_vto) | CBE |
| fld_aux_cod_exp_LostFocus | [CMXsrv_expcbe_lee_cln](#cmxsrv_expcbe_lee_cln) | CLN |
| Proximas_Click | [CMXsrv_expcbe_bus_vto](#cmxsrv_expcbe_bus_vto) | CBE |
| aceptar_Click | [CMXsrv_avi_dat_cou](#cmxsrv_avi_dat_cou) |  |
| aceptar_Click | [CMXsrv_expcbe_avs_rem1](#cmxsrv_expcbe_avs_rem1) | COR, ACMXPGOCBE, ACMXPRTCBE, CBE01, CBE, CBE02, ACMXMONEDA, CTZ, ACMXENTDOC, ACMXPAIS, ACMXPAISES, CLN |
| aceptar_Click | [CMXsrv_expcbe_avs_rem3](#cmxsrv_expcbe_avs_rem3) | COR, CBE01, CBE, CTZ, ACMXMONEDA, ACMXPAISES, CLN, CCO |
| imprime_esp | [CMXsrv_expcbe_avs_rem2](#cmxsrv_expcbe_avs_rem2) | CBE02, CBE, DCZ |
| imprime_esp | [CMXsrv_expcbe_avs_rem4](#cmxsrv_expcbe_avs_rem4) | ACMXREMFESPMSG, ACMXREMFINGMSG |
| imprime_ing | [CMXsrv_expcbe_avs_rem2](#cmxsrv_expcbe_avs_rem2) | CBE02, CBE, DCZ |
| imprime_ing | [CMXsrv_expcbe_avs_rem4](#cmxsrv_expcbe_avs_rem4) | ACMXREMFESPMSG, ACMXREMFINGMSG |
| buscar_Click | [CMXsrv_busc_plz](#cmxsrv_busc_plz) | ACMXPLAZAS, comex..ACMXPLAZAS |
| fld_cor_cod_plz_Lostfocus | [CMXsrv_lee_plz](#cmxsrv_lee_plz) | ACMXPLAZAS |
| proximos_Click | [CMXsrv_busc_plz](#cmxsrv_busc_plz) | ACMXPLAZAS, comex..ACMXPLAZAS |
| buscar_Click | [CMXsrv_cor_busc_pais](#cmxsrv_cor_busc_pais) | ACMXPAIS |
| fld_cor_cod_pais_LostFocus | [CMXsrv_cor_lee_pais](#cmxsrv_cor_lee_pais) | comex..ACMXPAIS |
| proximos_Click | [CMXsrv_cor_busc_pais](#cmxsrv_cor_busc_pais) | ACMXPAIS |
| aceptar_Click | [CMXsrv_expcbe_lee_cor](#cmxsrv_expcbe_lee_cor) | ACMXPAIS, COR |
| buscar_Click | [CMXsrv_expcbe_bus_cor](#cmxsrv_expcbe_bus_cor) | COR |
| fld_aux_cod_pai_LostFocus | [CMXsrv_cor_lee_pais](#cmxsrv_cor_lee_pais) | comex..ACMXPAIS |
| fld_aux_cod_plz_LostFocus | [CMXsrv_lee_plz](#cmxsrv_lee_plz) | ACMXPLAZAS |
| proximos_Click | [CMXsrv_expcbe_bus_cor](#cmxsrv_expcbe_bus_cor) | COR |
| buscar_Click | [CMXsrv_busc_bco_mtr](#cmxsrv_busc_bco_mtr) | ACMXBANCOS |
| proximos_Click | [CMXsrv_busc_bco_mtr](#cmxsrv_busc_bco_mtr) | ACMXBANCOS |
| enviar_Click | [CMXsrv_expcbe_swf_sel](#cmxsrv_expcbe_swf_sel) | switxt, switxt1 |
| Aceptar_Click | [CMXsrv_expcbe_lee_cor](#cmxsrv_expcbe_lee_cor) | ACMXPAIS, COR |
| buscar_Click | [CMXsrv_expcbe_bus_cor](#cmxsrv_expcbe_bus_cor) | COR |
| proximos_Click | [CMXsrv_expcbe_bus_cor](#cmxsrv_expcbe_bus_cor) | COR |
| Form_Load | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |  |

---

## EXPCCE
<a name="expcce"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tabla Referenciada** |
|-------------|-----------------------------|----------------------|
| Form_Activate | [CMXsrv_cmx_busc_suc_usu](#cmxsrv_cmx_busc_suc_usu) | master..sysprocesses, tbl_User |
| Form_Activate | [CMXsrv_expcce_lee_cce](#cmxsrv_expcce_lee_cce) | ACMXPAIS, COR, tbl_User, CCE, ACMXSUCSAL, CLN |
| Form_Activate | [CMXsrv_expcce_trd_cce](#cmxsrv_expcce_trd_cce) | ACMXFORPAG, ACMXVIATPT, ACMXMAXCCE, ACMXCNFCCE, ACMXMONEDA, ACMXCLACOM, CCE, ACMXRCBCCE |
| MCCEANL_CLICK | [CMXsrv_expcce_anl_cce](#cmxsrv_expcce_anl_cce) | CCE |
| Mccectb_click | [CMXsrv_expcce_ctb_ing](#cmxsrv_expcce_ctb_ing) | CCE |
| Mccedel_Click | [CMXsrv_expcce_del_cce](#cmxsrv_expcce_del_cce) | COD, ACCECTP, ACCECND, CCB, COM, ACCEBCO, DCC, CCE, EVC, ACCEDCC, AFIN |
| MCCEVAL_CLICK | [CMXsrv_expcce_val_cce](#cmxsrv_expcce_val_cce) | ACMXPAIS, COR, ACMXPRMGRL, CCE_ADI, DCC, tbl_User, CCE, warnmsg, ACMXSUCSAL, COL |
| Mmt730_Click | [CMXsrv_expcce_swf_sel](#cmxsrv_expcce_swf_sel) | switxt, switxt1 |
| Mmt730Ing_Click | [CMXsrv_expcce_swf_sel](#cmxsrv_expcce_swf_sel) | switxt, switxt1 |
| Aceptar_Click | [CMXsrv_expcce_grb_bco](#cmxsrv_expcce_grb_bco) | CCB, ACCEBCO, ACCECRSE, CRSE, CCE |
| fld_cce_bco_avs_LostFocus | [CMXsrv_expcce_lee_cor](#cmxsrv_expcce_lee_cor) | ACMXPAIS, COR |
| fld_cce_bco_orig_LostFocus | [CMXsrv_expcce_lee_cor](#cmxsrv_expcce_lee_cor) | ACMXPAIS, COR |
| fld_cce_cod_ems_LostFocus | [CMXsrv_expcce_lee_cor](#cmxsrv_expcce_lee_cor) | ACMXPAIS, COR |
| fld_cce_cod_rmb_LostFocus | [CMXsrv_expcce_lee_cor](#cmxsrv_expcce_lee_cor) | ACMXPAIS, COR |
| Form_Activate | [CMXsrv_expcce_lee_bco](#cmxsrv_expcce_lee_bco) | COR, CCB, ACMXSUCSAL, ACCEBCO, CRSE, CCE, ACMXPAIS |
| Aceptar_Click | [CMXsrv_expcce_grb_ctp](#cmxsrv_expcce_grb_ctp) | ACCECTP, CCE |
| fld_cce_cod_bn1_LostFocus | [CMXsrv_expcce_lee_cln](#cmxsrv_expcce_lee_cln) | CLN |
| fld_cce_cod_bn2_LostFocus | [CMXsrv_expcce_lee_cln](#cmxsrv_expcce_lee_cln) | CLN |
| Form_Activate | [CMXsrv_expcce_lee_ctp](#cmxsrv_expcce_lee_ctp) | ACCECTP, ACMXPAIS, CLN, CCE |
| Aceptar_Click | [CMXsrv_expcce_cre_cce](#cmxsrv_expcce_cre_cce) | CCE |
| Aceptar_Click | [CMXsrv_expcce_grb_bco](#cmxsrv_expcce_grb_bco) | CCB, ACCEBCO, ACCECRSE, CRSE, CCE |
| Aceptar_Click | [CMXsrv_expcce_grb_ctp](#cmxsrv_expcce_grb_ctp) | ACCECTP, CCE |
| Aceptar_Click | [CMXsrv_expcce_gen_dcc](#cmxsrv_expcce_gen_dcc) | ACMXPAIS, DCC, CCE |
| Aceptar_Click | [CMXsrv_expcce_grb_cnd](#cmxsrv_expcce_grb_cnd) | CCE_ADI, ACCECRSE, CRSE, CCE, ACCE_ADI, ACCECND |
| fld_cce_fec_vto_LostFocus | [CMXsrv_util_det_habil](#cmxsrv_util_det_habil) | ACMXFERIADO |
| Form_Activate | [CMXsrv_expcce_lee_cnd](#cmxsrv_expcce_lee_cnd) | CCE_ADI, ACCECRSE, CRSE, CCE, ACCE_ADI, ACCECND |
| Form_Activate | [CMXsrv_expcce_trd_cnd](#cmxsrv_expcce_trd_cnd) | ACMXFORPAG, ACMXVIATPT, ACMXMAXCCE, ACMXCNFCCE, ACMXMONEDA, CCE, ACMXCLACOM, ACMXFDESDE, ACMXRCBCCE, ACCECND |
| ELIMINAR_Click | [CMXsrv_expcce_del_dcc](#cmxsrv_expcce_del_dcc) | DCC, CCE, ACCEDCC |
| Form_Activate | [CMXsrv_expcce_bus_dcc](#cmxsrv_expcce_bus_dcc) | DCC, CCE, ACCEDCC |
| Aceptar_Click | [CMXsrv_expcce_grb_dcc](#cmxsrv_expcce_grb_dcc) | DCC, CCE, ACCEDCC |
| Form_Activate | [CMXsrv_expcce_lee_dcc](#cmxsrv_expcce_lee_dcc) | DCC, CCE, ACCEDCC |
| Aceptar_Click | [CMXsrv_expcce_lee_cce](#cmxsrv_expcce_lee_cce) | ACMXPAIS, COR, tbl_User, CCE, ACMXSUCSAL, CLN |
| buscar_Click | [CMXsrv_expcce_bus_cce](#cmxsrv_expcce_bus_cce) | CCE |
| fld_aux_cod_bn1_lostfocus | [CMXsrv_expcce_lee_cln](#cmxsrv_expcce_lee_cln) | CLN |
| proximo_Click | [CMXsrv_expcce_bus_cce](#cmxsrv_expcce_bus_cce) | CCE |
| Aceptar_Click | [CMXsrv_expcce_mdf_cce](#cmxsrv_expcce_mdf_cce) | COR, ACCECTP, ACCEBCO, CCE_ADI, ACCECRSE, DAC, DCC, CRSE, CCE, ACCE_ADI, NGE, COL, ACCEDCC, ACCECND |
| Cancelar_Click | [CMXsrv_expcce_can_mdf](#cmxsrv_expcce_can_mdf) | ACCECTP, ACCEBCO, ACCEDCC, ACCECND |
| fld_cce_cod_bn1_LostFocus | [CMXsrv_expcce_lee_cln](#cmxsrv_expcce_lee_cln) | CLN |
| fld_cce_cod_ems_LostFocus | [CMXsrv_expcce_lee_cor](#cmxsrv_expcce_lee_cor) | ACMXPAIS, COR |
| Form_Activate | [CMXsrv_expcce_lee_mdf](#cmxsrv_expcce_lee_mdf) | ACMXSUCSAL, COR, CCE, CLN |
| Aceptar_Click | [CMXsrv_expcce_cnf_cce](#cmxsrv_expcce_cnf_cce) | COR, CCE, CLN |
| Aceptar_Click | [CMXsrv_expcce_grb_afin](#cmxsrv_expcce_grb_afin) | AFIN |
| Form_Activate | [CMXsrv_expcce_lee_cnf](#cmxsrv_expcce_lee_cnf) | ACMXFORPAG, COR, ACMXMONEDA, CCE, CLN |
| Form_Activate | [CMXsrv_expcce_lee_afin](#cmxsrv_expcce_lee_afin) | CCE, AFIN |
| Aceptar_Click | [CMXsrv_expcce_trp_cce](#cmxsrv_expcce_trp_cce) | COR, CCE |
| fld_cce_bco_dst_LostFocus | [CMXsrv_expcce_lee_cor](#cmxsrv_expcce_lee_cor) | ACMXPAIS, COR |
| Form_Activate | [CMXsrv_expcce_lee_trp](#cmxsrv_expcce_lee_trp) | CCE |
| Form_Activate | [CMXsrv_expcce_bus_evc](#cmxsrv_expcce_bus_evc) | EVC, CCE, NGE |
| proximo_Click | [CMXsrv_expcce_bus_evc](#cmxsrv_expcce_bus_evc) | EVC, CCE, NGE |
| reversar_Click | [CMXsrv_expcce_rev_cce](#cmxsrv_expcce_rev_cce) | COR, TAS, ACMXIMPUES, LTR, DCN, EVC, RET, CUO, EVO, TRSD, DSN, CCE, NGE, PUCBCX10, COD, CNO, COM, DAC, EVE, CAN, COL, AFIN, ORG, DTN, EVR |
| Form_Activate | [CMXsrv_expcce_lee_evc](#cmxsrv_expcce_lee_evc) | ACMXFORPAG, ACMXMONEDA, CCE, NGE, EVC, ACMXSUCSAL, ACMXTIPEVE |
| aceptar_Click | [CMXsrv_expcce_avs_rem1](#cmxsrv_expcce_avs_rem1) | ACMXFORPAG, COR, CCB, NGEB, ACMXMONEDA, LTR, CCE, DCN, NGE, ACMXPAISES, CLN |
| buscar_Click | [CMXsrv_busc_plz](#cmxsrv_busc_plz) | ACMXPLAZAS, comex..ACMXPLAZAS |
| fld_cor_cod_plz_Lostfocus | [CMXsrv_lee_plz](#cmxsrv_lee_plz) | ACMXPLAZAS |
| proximos_Click | [CMXsrv_busc_plz](#cmxsrv_busc_plz) | ACMXPLAZAS, comex..ACMXPLAZAS |
| buscar_Click | [CMXsrv_cor_busc_pais](#cmxsrv_cor_busc_pais) | ACMXPAIS |
| fld_cor_cod_pais_LostFocus | [CMXsrv_cor_lee_pais](#cmxsrv_cor_lee_pais) | comex..ACMXPAIS |
| proximos_Click | [CMXsrv_cor_busc_pais](#cmxsrv_cor_busc_pais) | ACMXPAIS |
| Aceptar_Click | [CMXsrv_expcce_lee_cor](#cmxsrv_expcce_lee_cor) | ACMXPAIS, COR |
| buscar_Click | [CMXsrv_expcce_bus_cor](#cmxsrv_expcce_bus_cor) | COR |
| Command1_Click | [CMXsrv_expcce_bus_cor](#cmxsrv_expcce_bus_cor) | COR |
| proximos_Click | [CMXsrv_expcce_bus_cor](#cmxsrv_expcce_bus_cor) | COR |
| enviar_Click | [CMXsrv_expcce_swf_sel](#cmxsrv_expcce_swf_sel) | switxt, switxt1 |
| Form_Load | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |  |

---

## expdex
<a name="expdex"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tabla Referenciada** |
|-------------|-----------------------------|----------------------|
| form_activate | [CMXsrv_expcbe_lee_prm](#cmxsrv_expcbe_lee_prm) | ACMXPRMGRL |
| form_activate | [CMXsrv_dex_lee_dex](#cmxsrv_dex_lee_dex) | ACMXSUCSAL, DEX, CLN, ACMXADUANA |
| Mdexeli_Click | [CMXsrv_dex_eli_dex](#cmxsrv_dex_eli_dex) | DEX |
| ACEPTAR_Click | [CMXsrv_dex_act_dex](#cmxsrv_dex_act_dex) | DEX |
| fld_dex_dia_plz_max_LostFocus | [CMXsrv_expdex_cal_fec](#cmxsrv_expdex_cal_fec) |  |
| fld_dex_fec_acep_LostFocus | [CMXsrv_expdex_cal_fec](#cmxsrv_expdex_cal_fec) |  |
| fld_dex_rut_exp_LostFocus | [CMXsrv_dex_lee_cli](#cmxsrv_dex_lee_cli) | CLN |
| FORM_Load | [CMXsrv_dex_lee_dex](#cmxsrv_dex_lee_dex) | ACMXSUCSAL, DEX, CLN, ACMXADUANA |
| Buscar_Click | [CMXsrv_dex_bus_dex](#cmxsrv_dex_bus_dex) | DEX |
| fld_dex_rut_exp_LostFocus | [CMXsrv_dex_lee_cli](#cmxsrv_dex_lee_cli) | CLN |
| FORM_Load | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |  |
| ACEPTAR_Click | [CMXsrv_dex_act_dex](#cmxsrv_dex_act_dex) | DEX |
| fld_dex_rut_exp_LostFocus | [CMXsrv_dex_lee_cli](#cmxsrv_dex_lee_cli) | CLN |
| FORM_Load | [CMXsrv_dex_lee_dex](#cmxsrv_dex_lee_dex) | ACMXSUCSAL, DEX, CLN, ACMXADUANA |
| COMELIMINAR_Click | [CMXsrv_dex_eli_dex](#cmxsrv_dex_eli_dex) | DEX |
| Form_Activate | [CMXsrv_dex_lee_dex](#cmxsrv_dex_lee_dex) | ACMXSUCSAL, DEX, CLN, ACMXADUANA |

---

## EXPNEG
<a name="expneg"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tabla Referenciada** |
|-------------|-----------------------------|----------------------|
| Form_Activate | [CMXsrv_expcbe_bus_evz](#cmxsrv_expcbe_bus_evz) | EVZ, CBE |
| Proximo_Click | [CMXsrv_expcbe_bus_evz](#cmxsrv_expcbe_bus_evz) | EVZ, CBE |
| Reversar_Click | [CMXsrv_expcbe_rev_cbe](#cmxsrv_expcbe_rev_cbe) | EVL, ACMXDESEMB, COR, ORG, ACMXIMPUES, ACMXPRMGRL, EVZ, CBE, TRSD, ACMXPRMEXP, COM, EVR, CTZ, DTN, OPREC, RET, PUCBCX10 |
| Form_Activate | [CMXsrv_expcbe_lee_evz](#cmxsrv_expcbe_lee_evz) | ACMXDESEMB, COR, ACMXPGOCBE, EVZ, CBE, ACMXMONEDA, ACMXTIPEVE, ACMXSUCSAL |
| Form_Activate | [CMXsrv_expcce_lee_bas](#cmxsrv_expcce_lee_bas) | ACMXMONEDA, CCE, ACMXFORPAG |
| Form_Activate | [CMXsrv_expcce_lee_neg](#cmxsrv_expcce_lee_neg) | COR, ACMXVIATPT, ACMXSUCSAL, ACMXDISNEG, ACMXMONEDA, ACMXCLACOM, NGE, ACMXPAIS, CLN, ACMXTPONEG |
| Mccealznge_click | [CMXsrv_expcce_alz_dis](#cmxsrv_expcce_alz_dis) | COL, CCE, NGE |
| Mcceanlnge_click | [CMXsrv_expcce_anl_neg](#cmxsrv_expcce_anl_neg) | CCE, NGE |
| Mccectbnge_Click | [CMXsrv_expcce_ctb_neg](#cmxsrv_expcce_ctb_neg) | COR, LTR, CCE, NGE, AFIN |
| Mccedelnge_Click | [CMXsrv_expcce_del_neg](#cmxsrv_expcce_del_neg) | CRSN, COD, COM, NGEB, LTR, DSN, CCE, DCN, NGE, EVC, AFIN |
| Mccevalnge_click | [CMXsrv_expcce_val_neg](#cmxsrv_expcce_val_neg) | NGEB, LTR, DCC, warnmsg, CCE, DCN, NGE, COL, AFIN |
| Mtel742_Click | [CMXsrv_expcce_swf_sel](#cmxsrv_expcce_swf_sel) | switxt, switxt1 |
| Form_Activate | [CMXsrv_expcce_bus_evc](#cmxsrv_expcce_bus_evc) | EVC, CCE, NGE |
| Proximo_Click | [CMXsrv_expcce_bus_evc](#cmxsrv_expcce_bus_evc) | EVC, CCE, NGE |
| Reversar_Click | [CMXsrv_expcce_rev_cce](#cmxsrv_expcce_rev_cce) | COR, TAS, ACMXIMPUES, LTR, DCN, EVC, RET, CUO, EVO, TRSD, DSN, CCE, NGE, PUCBCX10, COD, CNO, COM, DAC, EVE, CAN, COL, AFIN, ORG, DTN, EVR |
| Form_Activate | [CMXsrv_expcce_lee_evc](#cmxsrv_expcce_lee_evc) | ACMXFORPAG, ACMXMONEDA, CCE, NGE, EVC, ACMXSUCSAL, ACMXTIPEVE |
| aceptar_Click | [CMXsrv_expcce_grb_neg](#cmxsrv_expcce_grb_neg) | CRSN, CCE, NGEB, NGE |
| aceptar_Click | [CMXsrv_expcce_gen_dcn](#cmxsrv_expcce_gen_dcn) | DCC, CCE, DCN, NGE |
| aceptar_Click | [CMXsrv_expcce_grb_afin](#cmxsrv_expcce_grb_afin) | AFIN |
| fld_cce_cod_exp_nge_LostFocus | [CMXsrv_expcce_lee_cln](#cmxsrv_expcce_lee_cln) | CLN |
| fld_cce_cod_pag_nge_LostFocus | [CMXsrv_expcce_lee_cor](#cmxsrv_expcce_lee_cor) | ACMXPAIS, COR |
| fld_cce_cod_rmb_nge_LostFocus | [CMXsrv_expcce_lee_cor](#cmxsrv_expcce_lee_cor) | ACMXPAIS, COR |
| fld_cce_ins_rem1_nge_GotFocus | [CMXsrv_expcce_avs_rem5](#cmxsrv_expcce_avs_rem5) | COR, ACMXCRDREMTXT, ACMXMONEDA, CCE, NGE, ACMXPAISES, CCO |
| Form_Load | [CMXsrv_expcce_lee_nge](#cmxsrv_expcce_lee_nge) | COR, CRSN, NGEB, CCE, NGE, ACMXPAIS, CLN |
| Form_Load | [CMXsrv_expcce_trd_nge](#cmxsrv_expcce_trd_nge) | ACMXVIATPT, ACMXRCBCCE, ACMXMONEDA, ACMXCLACOM, NGE, ACMXTPONEG |
| Form_Load | [CMXsrv_expcce_ini_neg](#cmxsrv_expcce_ini_neg) | ACMXPAIS, COR, ACMXVIATPT, CCB, ACMXMONEDA, CRSE, CCE, ACMXCLACOM, NGE, ACMXSUCSAL, CLN, ACMXTPONEG |
| Form_Load | [CMXsrv_expcce_lee_afin](#cmxsrv_expcce_lee_afin) | CCE, AFIN |
| lee_bco | [CMXsrv_expcce_lee_cor](#cmxsrv_expcce_lee_cor) | ACMXPAIS, COR |
| ELIMINAR_Click | [CMXsrv_expcce_del_dcn](#cmxsrv_expcce_del_dcn) | CCE, DCN, NGE |
| Form_Activate | [CMXsrv_expcce_bus_dcn](#cmxsrv_expcce_bus_dcn) | DCN, NGE |
| Aceptar_Click | [CMXsrv_expcce_grb_dcn](#cmxsrv_expcce_grb_dcn) | CCE, DCN, NGE |
| Form_Load | [CMXsrv_expcce_lee_dcn](#cmxsrv_expcce_lee_dcn) | DCC, DCN, NGE |
| ELIMINAR_Click | [CMXsrv_expcce_del_ltr](#cmxsrv_expcce_del_ltr) | LTR, CCE, NGE |
| Form_Activate | [CMXsrv_expcce_bus_ltr](#cmxsrv_expcce_bus_ltr) | LTR, NGE |
| Aceptar_Click | [CMXsrv_expcce_grb_ltr](#cmxsrv_expcce_grb_ltr) | LTR, CCE, NGE |
| Form_Load | [CMXsrv_expcce_lee_ltr](#cmxsrv_expcce_lee_ltr) | LTR, CCE, NGE |
| ELIMINAR_Click | [CMXsrv_expcce_del_dsn](#cmxsrv_expcce_del_dsn) | DSN, CCE, NGE |
| Form_Activate | [CMXsrv_expcce_gen_dsn](#cmxsrv_expcce_gen_dsn) | DCC, DSN, CCE, DCN, NGE |
| Form_Activate | [CMXsrv_expcce_bus_dsn](#cmxsrv_expcce_bus_dsn) | DSN, NGE |
| Salir_Click | [CMXsrv_expcce_chk_dsn](#cmxsrv_expcce_chk_dsn) | DSN, CCE, NGE |
| Aceptar_Click | [CMXsrv_expcce_grb_dsn](#cmxsrv_expcce_grb_dsn) | DSN, CCE, NGE |
| Form_Load | [CMXsrv_expcce_lee_dsn](#cmxsrv_expcce_lee_dsn) | DSN, NGE |
| buscar_Click | [CMXsrv_expcce_bus_neg](#cmxsrv_expcce_bus_neg) | CCE, NGE |
| Proximas_Click | [CMXsrv_expcce_bus_neg](#cmxsrv_expcce_bus_neg) | CCE, NGE |
| aceptar_Click | [CMXsrv_expcce_pgo_neg](#cmxsrv_expcce_pgo_neg) | ACMXDESEMB, COR, vig_cmx, ACMXIMPUES, COD, ACMXPRMEXP, COM, CCE, tbl_User, NGE, CLN, RET |
| aceptar_Click | [CMXsrv_expcce_grb_afin](#cmxsrv_expcce_grb_afin) | AFIN |
| fld_cce_cod_exp_nge_LostFocus | [CMXsrv_expcce_lee_cln](#cmxsrv_expcce_lee_cln) | CLN |
| fld_cce_cod_rmb_nge_LostFocus | [CMXsrv_expcce_lee_cor](#cmxsrv_expcce_lee_cor) | ACMXPAIS, COR |
| Form_Load | [CMXsrv_expcce_lee_pgo](#cmxsrv_expcce_lee_pgo) | ACMXDESEMB, COR, ACMXPRMEXP, ACMXMONEDA, CCE, NGE, CLN |
| Form_Load | [CMXsrv_expcce_lee_afin](#cmxsrv_expcce_lee_afin) | CCE, AFIN |
| lee_bco | [CMXsrv_expcce_lee_cor](#cmxsrv_expcce_lee_cor) | ACMXPAIS, COR |
| aceptar_Click | [CMXsrv_avi_dat_cou](#cmxsrv_avi_dat_cou) |  |
| aceptar_Click | [CMXsrv_expcce_lee_nge](#cmxsrv_expcce_lee_nge) | COR, CRSN, NGEB, CCE, NGE, ACMXPAIS, CLN |
| aceptar_Click | [CMXsrv_expcce_avs_rem1](#cmxsrv_expcce_avs_rem1) | ACMXFORPAG, COR, CCB, NGEB, ACMXMONEDA, LTR, CCE, DCN, NGE, ACMXPAISES, CLN |
| aceptar_Click | [CMXsrv_expcce_avs_rem3](#cmxsrv_expcce_avs_rem3) | LTR, NGE |
| imprime_esp | [CMXsrv_expcce_avs_rem2](#cmxsrv_expcce_avs_rem2) | DCN |
| imprime_esp | [CMXsrv_expcce_avs_rem4](#cmxsrv_expcce_avs_rem4) | DSN |
| imprime_esp | [CMXsrv_expcbe_avs_rem4](#cmxsrv_expcbe_avs_rem4) | ACMXREMFESPMSG, ACMXREMFINGMSG |
| imprime_ing | [CMXsrv_expcce_avs_rem2](#cmxsrv_expcce_avs_rem2) | DCN |
| imprime_ing | [CMXsrv_expcce_avs_rem4](#cmxsrv_expcce_avs_rem4) | DSN |
| imprime_ing | [CMXsrv_expcbe_avs_rem4](#cmxsrv_expcbe_avs_rem4) | ACMXREMFESPMSG, ACMXREMFINGMSG |
| aceptar_Click | [CMXsrv_expcce_lee_cor](#cmxsrv_expcce_lee_cor) | ACMXPAIS, COR |
| buscar_Click | [CMXsrv_expcce_bus_cor](#cmxsrv_expcce_bus_cor) | COR |
| proximos_Click | [CMXsrv_expcce_bus_cor](#cmxsrv_expcce_bus_cor) | COR |
| enviar_Click | [CMXsrv_expcce_swf_sel](#cmxsrv_expcce_swf_sel) | switxt, switxt1 |
| Form_Load | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |  |

---

## expret
<a name="expret"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tabla Referenciada** |
|-------------|-----------------------------|----------------------|
| buscar_Click | [CMXsrv_busc_plz](#cmxsrv_busc_plz) | ACMXPLAZAS, comex..ACMXPLAZAS |
| fld_cor_cod_plz_Lostfocus | [CMXsrv_lee_plz](#cmxsrv_lee_plz) | ACMXPLAZAS |
| proximos_Click | [CMXsrv_busc_plz](#cmxsrv_busc_plz) | ACMXPLAZAS, comex..ACMXPLAZAS |
| buscar_Click | [CMXsrv_cor_busc_pais](#cmxsrv_cor_busc_pais) | ACMXPAIS |
| fld_cor_cod_pais_LostFocus | [CMXsrv_cor_lee_pais](#cmxsrv_cor_lee_pais) | comex..ACMXPAIS |
| proximos_Click | [CMXsrv_cor_busc_pais](#cmxsrv_cor_busc_pais) | ACMXPAIS |
| Aceptar_Click | [CMXsrv_expcbe_lee_cor](#cmxsrv_expcbe_lee_cor) | ACMXPAIS, COR |
| buscar_Click | [CMXsrv_expcbe_bus_cor](#cmxsrv_expcbe_bus_cor) | COR |
| proximos_Click | [CMXsrv_expcbe_bus_cor](#cmxsrv_expcbe_bus_cor) | COR |
| Command2_Click | [CMXsrv_expret_swf_sel](#cmxsrv_expret_swf_sel) | DTN, ACMXPRMEXP, switxt, switxt1 |
| Form_Load | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |  |
| Form_Activate | [CMXsrv_cmx_busc_suc_usu](#cmxsrv_cmx_busc_suc_usu) | master..sysprocesses, tbl_User |
| Form_Activate | [CMXsrv_expret_lee_ret](#cmxsrv_expret_lee_ret) | DTN, ACMXPRMEXP, ACMXMONEDA, ACMXSUCSAL, CLN, RET |
| Form_Load | [CMXsrv_expret_lee_prm](#cmxsrv_expret_lee_prm) | ACMXPRMGRL, ACMXPRMEXP |
| M_cgyc_Click | [CMXsrv_expret_avs_cyg1](#cmxsrv_expret_avs_cyg1) | ACMXDESEMB, ASND, ACMXIMPUES, ACMXPRMGRL, COM, TRSD, EVR, CLN, ACMXESPECI, RET |
| M_cgyc_Click | [CMXsrv_expret_avs_cyg2](#cmxsrv_expret_avs_cyg2) | ASND, ACMXIMPUES, ACMXPRMGRL, EVR, RET |
| mavisliq_Click | [CMXsrv_expret_avs_liq1](#cmxsrv_expret_avs_liq1) | DTN, ACMXMONEDA, ACMXSUCSAL, CLN, ACMXESPECI, RET |
| mavisliq_Click | [CMXsrv_expret_avs_liq2](#cmxsrv_expret_avs_liq2) | ORG, RET |
| mavisliq_Click | [CMXsrv_expret_avs_liq3](#cmxsrv_expret_avs_liq3) | DTN, ACMXPRMEXP, RET |
| Mcbectb_Click | [CMXsrv_expret_val_ret](#cmxsrv_expret_val_ret) | ACMXDESEMB, ORG, COR, ACMXIMPUES, ACMXPRMGRL, CCL, ACMXPRMEXP, ACMXMONEDAFEC, COM, tbl_User, warnmsg, DTN, CLN, RET |
| Mcbectb_Click | [CMXsrv_expret_sum_dtn_mn](#cmxsrv_expret_sum_dtn_mn) | DTN, ACMXMONEDAFEC, RET, ACMXPRMENL |
| Mcbectb_Click | [CMXsrv_expret_ctb_ing](#cmxsrv_expret_ctb_ing) | ACMXDESEMB, ASND, PLV, ACMXPRMGRL, CCL, ACMXPRMEXP, PLI, tbl_User, DTN, CLN, RET |
| Mcbedel_Click | [CMXsrv_expret_del_ret](#cmxsrv_expret_del_ret) | ORG, COD, COM, DTN, RET |
| Mliqctb_Click | [CMXsrv_expret_avs_adm1](#cmxsrv_expret_avs_adm1) | ACMXSUCSAL, ACMXMONEDA, CLN, RET |
| Mliqctb_Click | [CMXsrv_expret_avs_adm2](#cmxsrv_expret_avs_adm2) | ORG, ACMXPRMEXP, RET |
| Mliqctb_Click | [CMXsrv_expret_avs_adm3](#cmxsrv_expret_avs_adm3) | DTN, ACMXPRMEXP, RET |
| Mvalid_Click | [CMXsrv_expret_val_ret](#cmxsrv_expret_val_ret) | ACMXDESEMB, ORG, COR, ACMXIMPUES, ACMXPRMGRL, CCL, ACMXPRMEXP, ACMXMONEDAFEC, COM, tbl_User, warnmsg, DTN, CLN, RET |
| ACEPTAR_Click | [CMXsrv_expret_act_tpo_cbo](#cmxsrv_expret_act_tpo_cbo) | RET |
| ACEPTAR_Click | [CMXsrv_expret_val_ret](#cmxsrv_expret_val_ret) | ACMXDESEMB, ORG, COR, ACMXIMPUES, ACMXPRMGRL, CCL, ACMXPRMEXP, ACMXMONEDAFEC, COM, tbl_User, warnmsg, DTN, CLN, RET |
| ACEPTAR_Click | [CMXsrv_expret_cre_ret](#cmxsrv_expret_cre_ret) | RET |
| ACEPTAR_Click | [CMXsrv_expret_grb_det](#cmxsrv_expret_grb_det) | CLN, tbl_User, RET |
| fld_ret_mon_ret_LostFocus | [CMXsrv_expret_tpo_cbo](#cmxsrv_expret_tpo_cbo) | ACMXMONEDAFEC |
| fld_ret_rut_cli_LostFocus | [CMXsrv_expret_lee_cln](#cmxsrv_expret_lee_cln) | CLN |
| Form_Load | [CMXsrv_expret_lee_det](#cmxsrv_expret_lee_det) | ACMXSUCSAL, ACMXMONEDA, CLN, RET |
| ELIMINAR_Click | [CMXsrv_expret_del_org](#cmxsrv_expret_del_org) | ORG, RET |
| Form_Activate | [CMXsrv_expret_bus_org](#cmxsrv_expret_bus_org) | ORG, RET |
| ACEPTAR_Click | [CMXsrv_expret_grb_org](#cmxsrv_expret_grb_org) | ACMXDESEMB, ORG, ACMXPLNCTAN, ACMXSRVEXT, ACMXPLNCTAX, RET |
| Form_Activate | [CMXsrv_expret_mto_org](#cmxsrv_expret_mto_org) | ORG, RET |
| Form_Activate | [CMXsrv_expret_lee_org](#cmxsrv_expret_lee_org) | ACMXDESEMB, ORG, COR, ACMXTPODOC, ACMXPAIS |
| valida_vigente | [CMXsrv_vig_lee_cta](#cmxsrv_vig_lee_cta) | ACMXPLNCTAN, ACMXDESEMB, ACMXPLNCTAX |
| ELIMINAR_Click | [CMXsrv_expret_del_dtn](#cmxsrv_expret_del_dtn) | DTN, RET |
| emitir_Click | [CMXsrv_expret_swf_sel](#cmxsrv_expret_swf_sel) | DTN, ACMXPRMEXP, switxt, switxt1 |
| Form_Activate | [CMXsrv_expret_bus_dtn](#cmxsrv_expret_bus_dtn) | DTN, RET |
| ACEPTAR_Click | [CMXsrv_expret_grb_dtn](#cmxsrv_expret_grb_dtn) | ACMXDESEMB, ACMXPRMGRL, CCL, ACMXPRMEXP, DTN, RET |
| fld_ret_cod_ben_LostFocus | [CMXsrv_expret_lee_cln](#cmxsrv_expret_lee_cln) | CLN |
| fld_ret_mto_arb_LostFocus | [CMXsrv_expret_cal_arb](#cmxsrv_expret_cal_arb) | ACMXPRMGRL, ACMXMONEDA |
| fld_ret_mto_ben_LostFocus | [CMXsrv_expret_cal_arb](#cmxsrv_expret_cal_arb) | ACMXPRMGRL, ACMXMONEDA |
| fld_ret_par_ben_LostFocus | [CMXsrv_expret_cal_arb](#cmxsrv_expret_cal_arb) | ACMXPRMGRL, ACMXMONEDA |
| Form_Activate | [CMXsrv_expret_mto_dtn](#cmxsrv_expret_mto_dtn) | DTN, COM, RET, ACMXIMPUES |
| Form_Load | [CMXsrv_expret_lee_dtn](#cmxsrv_expret_lee_dtn) | ACMXPAIS, ACMXDESEMB, COR, DTN, ACMXMONEDA, APUCCODOPECMB, ACMXSUCSAL |
| Form_Load | [CMXsrv_expret_lee_cln](#cmxsrv_expret_lee_cln) | CLN |
| buscar_Click | [CMXsrv_expret_bus_ret](#cmxsrv_expret_bus_ret) | RET |
| fld_ret_rut_cli_LostFocus | [CMXsrv_expret_lee_cln](#cmxsrv_expret_lee_cln) | CLN |
| proxima_Click | [CMXsrv_expret_bus_ret](#cmxsrv_expret_bus_ret) | RET |
| Command1_Click | [CMXsrv_expret_bus_evr](#cmxsrv_expret_bus_evr) | EVR, RET |
| Form_Activate | [CMXsrv_expret_bus_evr](#cmxsrv_expret_bus_evr) | EVR, RET |
| proximo_Click | [CMXsrv_expret_bus_evr](#cmxsrv_expret_bus_evr) | EVR, RET |
| reversar_Click | [CMXsrv_expret_rev_ret](#cmxsrv_expret_rev_ret) | ORG, DTN, PLV, ACMXPRMEXP, PLI, TRSD, EVR, RET |
| Form_Load | [CMXsrv_expret_lee_evr](#cmxsrv_expret_lee_evr) | ACMXTIPEVE, EVR, ACMXSUCSAL |

---

## ADMIN
<a name="admin"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tabla Referenciada** |
|-------------|-----------------------------|----------------------|
| COMMAND4_Click | [CMXsrv_finadm_imod_desti](#cmxsrv_finadm_imod_desti) | TIP |
| Form_Load | [CMXsrv_finadm_cons_dtip](#cmxsrv_finadm_cons_dtip) | TIP |
| Command1_Click | [CMXsrv_finadm_imod_ectb](#cmxsrv_finadm_imod_ectb) | TIP |
| Command2_Click | [CMXsrv_finadm_eli_tipop](#cmxsrv_finadm_eli_tipop) | TIP, TIP_CTA |
| Form_Load | [CMXsrv_finadm_cons_ectb](#cmxsrv_finadm_cons_ectb) | TIP |
| COMMAND3_Click | [CMXsrv_finadm_eli_tipop](#cmxsrv_finadm_eli_tipop) | TIP, TIP_CTA |
| COMMAND4_Click | [CMXsrv_finadm_imod_itip](#cmxsrv_finadm_imod_itip) | TIP |
| Form_Load | [CMXsrv_finadm_cons_itip](#cmxsrv_finadm_cons_itip) | TIP |
| Form_Activate | [CMXsrv_finadm_lee_tipop](#cmxsrv_finadm_lee_tipop) | TIP, ACMXPLAZO, ACMXPROCMX, ACMXMB1 |
| Form_Load | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |  |
| Mdel_Click | [CMXsrv_finadm_eli_tipop](#cmxsrv_finadm_eli_tipop) | TIP, TIP_CTA |
| Mval_Click | [CMXsrv_finadm_val_tipop](#cmxsrv_finadm_val_tipop) | APEPROR, TIP, TAS, CUO, ACMXPLNCTAN, ACMXMONEDAFEC, PANCTL, ACLNCBCABCI, ACMXPLNCTAX, TIP_CTA, ACMXMONEDA, warnmsg, EVE, ACMXSUCSAL, PANVTO, ACMXINTEREFEC, COL, PANMOR |
| buscar_Click | [CMXsrv_finadm_bus_tipope](#cmxsrv_finadm_bus_tipope) | TIP |
| proximas_Click | [CMXsrv_finadm_bus_tipope](#cmxsrv_finadm_bus_tipope) | TIP |

---

## COL_NEG
<a name="col_neg"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tabla Referenciada** |
|-------------|-----------------------------|----------------------|
| CANCELAR_Click | [CMXsrv_busc_tip_tas](#cmxsrv_busc_tip_tas) | CRD |
| ELIMINAR_Click | [CMXsrv_fincol_ecuo](#cmxsrv_fincol_ecuo) | CUO_REN, COL, CUO |
| Form_Activate | [CMXsrv_fincol_cons_plnpa](#cmxsrv_fincol_cons_plnpa) | CUO_REN, COL_REN, COL, CUO |
| Form_Load | [CMXsrv_pertas_val_display](#cmxsrv_pertas_val_display) | TAS |
| ELIMINAR_Click | [CMXsrv_fincol_eava](#cmxsrv_fincol_eava) | DAC, AVAL, AVAL_REN, COL |
| Form_Activate | [CMXsrv_fincol_cons_aval](#cmxsrv_fincol_cons_aval) | CRDCLON, AVAL, AVAL_REN, COL |
| ingresar_Click | [CMXsrv_fincol_iava](#cmxsrv_fincol_iava) | AVAL, AVAL_REN, CLN, COL |
| Form_Activate | [CMXsrv_fincol_cons_pag](#cmxsrv_fincol_cons_pag) | CAN, COL |
| proximos_Click | [CMXsrv_fincol_cons_pag](#cmxsrv_fincol_cons_pag) | CAN, COL |
| Form_Activate | [CMXsrv_fincol_trae_det_pag](#cmxsrv_fincol_trae_det_pag) | CAN, EVE |
| Form_Activate | [CMXsrv_fincol_cons_pror](#cmxsrv_fincol_cons_pror) | EVE, COL |
| Form_Activate | [CMXsrv_fincol_cons_eve](#cmxsrv_fincol_cons_eve) | EVE, COL |
| Aceptar_Click | [CMXsrv_icrd_lee_bco_swf](#cmxsrv_icrd_lee_bco_swf) | ACMXPAIS, COR |
| buscar_Click | [CMXsrv_icrd_busc_bco](#cmxsrv_icrd_busc_bco) | COR |
| proximo_Click | [CMXsrv_icrd_busc_bco](#cmxsrv_icrd_busc_bco) | COR |
| Aceptar_Click | [CMXsrv_fincol_vtocre_prov](#cmxsrv_fincol_vtocre_prov) | TIP, comex..ACMXINTEREFEC, COR, CRD, CUO, OBL, NEG, NEG_ADI, DAC, ACMXINTERE, ACMXMONEDA, ACMXINTEREFEC, AVAL, MYC, COL, CTO |
| Form_Load | [CMXsrv_fincol_prec_vtocre](#cmxsrv_fincol_prec_vtocre) | TIP, CRD, CNEG, NEG, COL |
| buscar_Click | [CMXsrv_icrd_bus_lcr_bco](#cmxsrv_icrd_bus_lcr_bco) | COR |
| proximo_Click | [CMXsrv_icrd_bus_lcr_bco](#cmxsrv_icrd_bus_lcr_bco) | COR |
| Form_Load | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |  |
| Form_Load | [CMXsrv_lee_fpro](#cmxsrv_lee_fpro) | ACMXFECPRO |

---

## INGRESO
<a name="ingreso"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tabla Referenciada** |
|-------------|-----------------------------|----------------------|
| cancelar_Click | [CMXsrv_fincol_ren_fin](#cmxsrv_fincol_ren_fin) | COL_REN, TIP, TAS, TAS_REN, EVE_REN, DAC_REN, ITA, CUO_REN, AVAL_REN, EVE, CAN_REN, COL |
| ELIMINAR_Click | [CMXsrv_fincol_ecuo](#cmxsrv_fincol_ecuo) | CUO_REN, COL, CUO |
| form_activate | [CMXsrv_fincol_cons_plnpa](#cmxsrv_fincol_cons_plnpa) | CUO_REN, COL_REN, COL, CUO |
| cancelar_Click | [CMXsrv_fincol_ren_fin](#cmxsrv_fincol_ren_fin) | COL_REN, TIP, TAS, TAS_REN, EVE_REN, DAC_REN, ITA, CUO_REN, AVAL_REN, EVE, CAN_REN, COL |
| ELIMINAR_Click | [CMXsrv_fincol_eava](#cmxsrv_fincol_eava) | DAC, AVAL, AVAL_REN, COL |
| form_activate | [CMXsrv_fincol_cons_aval](#cmxsrv_fincol_cons_aval) | CRDCLON, AVAL, AVAL_REN, COL |
| aceptar_Click | [CMXsrv_fincol_gmod_ctr](#cmxsrv_fincol_gmod_ctr) | TIP, CUO, OBL, CTR, CLN, COL, CTO |
| busca_bco | [CMXsrv_icrd_lee_bco_swf](#cmxsrv_icrd_lee_bco_swf) | ACMXPAIS, COR |
| fld_obl_bco_acr_LostFocus | [CMXsrv_fincol_lee_bco](#cmxsrv_fincol_lee_bco) | COR |
| fld_obl_rut_acr_LostFocus | [CMXsrv_fincol_lee_cln](#cmxsrv_fincol_lee_cln) | CLN |
| form_activate | [CMXsrv_fincol_cons_ctr](#cmxsrv_fincol_cons_ctr) | OBL, CTR |
| aceptar_Click | [CMXsrv_fincol_ctb_oto](#cmxsrv_fincol_ctb_oto) | TIP, ACMXDESEMB, CUO, COD, vig_cmx, COL_ADI, ACMXPRMGRL, OBL, COM, MYC, ACMXMONEDA, LIB, OPE_BCI, CLN, COL, CCO |
| Avi5_Click | [CMXsrv_icrd_dat_liq_ope](#cmxsrv_icrd_dat_liq_ope) | ACMXDESEMB, ASND, EVO, CRD, CNO, OBL, CUO, TRSD, NEG, COM, EVE, ACMXTIPEVE, CAN, COL |
| form_activate | [CMXsrv_fincol_lee_col](#cmxsrv_fincol_lee_col) | COR, TAS, NEG_ADI, ACMXINTERE, TIP, CUO, CCL, ACMXFINVER, ACMXAPROBAC, COL_ADI, ACMXACTIVIDA, ACMXINTEREFEC, AVAL, ACMXSUCSAL, CLN, comex..ACMXINTEREFEC, COM, ACMXMONEDA, EVE, tbl_User, COL |
| Form_Load | [CMXsrv_lee_fpro](#cmxsrv_lee_fpro) | ACMXFECPRO |
| MCOLCOMI_CLICK | [CMXsrv_busc_cod_ope](#cmxsrv_busc_cod_ope) | TIP, COL |
| MCOLCOMI_CLICK | [CMXsrv_col_trae_num_ope](#cmxsrv_col_trae_num_ope) | COL |
| MCOLCONTOTOR_CLICK | [CMXsrv_busc_cod_ope](#cmxsrv_busc_cod_ope) | TIP, COL |
| MCOLCONTOTOR_CLICK | [CMXsrv_col_trae_num_ope](#cmxsrv_col_trae_num_ope) | COL |
| MCOLCONTOTOR_CLICK | [CMXsrv_fincol_ctb_oto](#cmxsrv_fincol_ctb_oto) | TIP, ACMXDESEMB, CUO, COD, vig_cmx, COL_ADI, ACMXPRMGRL, OBL, COM, MYC, ACMXMONEDA, LIB, OPE_BCI, CLN, COL, CCO |
| MCOLELI_CLICK | [CMXsrv_fincol_eli_col](#cmxsrv_fincol_eli_col) | COL_REN, COL_ADI, COM, TAS_REN, DAC_REN, EVE_REN, DAC, CUO_REN, AVAL_REN, LIB, CAN_REN, COL |
| valida | [CMXsrv_fincol_val_col](#cmxsrv_fincol_val_col) | TIP, COL, warnmsg |
| aceptar_Click | [CMXsrv_fincol_lee_col](#cmxsrv_fincol_lee_col) | COR, TAS, NEG_ADI, ACMXINTERE, TIP, CUO, CCL, ACMXFINVER, ACMXAPROBAC, COL_ADI, ACMXACTIVIDA, ACMXINTEREFEC, AVAL, ACMXSUCSAL, CLN, comex..ACMXINTEREFEC, COM, ACMXMONEDA, EVE, tbl_User, COL |
| buscar_Click | [CMXsrv_fincol_bsc_col](#cmxsrv_fincol_bsc_col) | TIP |
| fld_col_tip_ope_lostfocus | [CMXsrv_fincol_lee_tip](#cmxsrv_fincol_lee_tip) | TIP |
| PROXIMAS_Click | [CMXsrv_fincol_bsc_col](#cmxsrv_fincol_bsc_col) | TIP |
| ingresar_Click | [CMXsrv_fincol_iava](#cmxsrv_fincol_iava) | AVAL, AVAL_REN, CLN, COL |
| aceptar_Click | [CMXsrv_busc_cod_ope](#cmxsrv_busc_cod_ope) | TIP, COL |
| aceptar_Click | [CMXsrv_col_trae_num_ope](#cmxsrv_col_trae_num_ope) | COL |
| aceptar_Click | [CMXsrv_fincol_ctb_novf](#cmxsrv_fincol_ctb_novf) | CLN, COL |
| FLD_COL_COD_CLI_LOSTFOCUS | [CMXsrv_fincol_lee_cln](#cmxsrv_fincol_lee_cln) | CLN |
| FLD_COL_RUT_DEU_NOV_LostFocus | [CMXsrv_fincol_lee_cln](#cmxsrv_fincol_lee_cln) | CLN |
| form_activate | [CMXsrv_fincol_cons_nov](#cmxsrv_fincol_cons_nov) | EVE, COL |
| FLD_COL_COD_CLI_LOSTFOCUS | [CMXsrv_fincol_lee_cln](#cmxsrv_fincol_lee_cln) | CLN |
| FLD_COL_RUT_DEU_NOV_LostFocus | [CMXsrv_fincol_lee_cln](#cmxsrv_fincol_lee_cln) | CLN |
| Aceptar_Click | [CMXsrv_icrd_lee_bco_swf](#cmxsrv_icrd_lee_bco_swf) | ACMXPAIS, COR |
| buscar_Click | [CMXsrv_icrd_busc_bco](#cmxsrv_icrd_busc_bco) | COR |
| proximo_Click | [CMXsrv_icrd_busc_bco](#cmxsrv_icrd_busc_bco) | COR |
| Form_Load | [CMXsrv_cmx_get_codes](#cmxsrv_cmx_get_codes) |  |
| Form_Load | [CMXsrv_grl_trae_cod_bco](#cmxsrv_grl_trae_cod_bco) |  |

---

## MODIFIC
<a name="modific"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tabla Referenciada** |
|-------------|-----------------------------|----------------------|
| Form_Activate | [CMXsrv_fincol_cons_tas](#cmxsrv_fincol_cons_tas) | TAS |
| aceptar_click | [CMXsrv_fincol_efec_tras](#cmxsrv_fincol_efec_tras) | TIP, comex..ACMXMONEDAFEC, COL, CUO |
| Form_Activate | [CMXsrv_fincol_cons_trasp](#cmxsrv_fincol_cons_trasp) | EVE, COL |
| Form_Activate | [CMXsrv_fincol_cons_dtrs](#cmxsrv_fincol_cons_dtrs) | EVE, COL |
| Form_Activate | [CMXsrv_fincol_cons_eve](#cmxsrv_fincol_cons_eve) | EVE, COL |
| Form_Load | [CMXsrv_fincol_cons_deve](#cmxsrv_fincol_cons_deve) | EVE, COL |
| aceptar_click | [CMXsrv_fincol_cont_gst](#cmxsrv_fincol_cont_gst) |  |
| Form_Activate | [CMXsrv_fincol_cons_gst](#cmxsrv_fincol_cons_gst) | EVE, COL |
| Form_Activate | [CMXsrv_fincol_cons_dgst](#cmxsrv_fincol_cons_dgst) |  |
| Form_Load | [CMXsrv_lee_fpro](#cmxsrv_lee_fpro) | ACMXFECPRO |

---

## OBLIGA
<a name="obliga"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tabla Referenciada** |
|-------------|-----------------------------|----------------------|
| buscar_Click | [CMXsrv_fincol_bsc_tip](#cmxsrv_fincol_bsc_tip) | TIP |
| Proxima_Click | [CMXsrv_fincol_bsc_tip](#cmxsrv_fincol_bsc_tip) | TIP |
| proximo_Click | [CMXsrv_fincol_bsc_tip](#cmxsrv_fincol_bsc_tip) | TIP |
| buscar_Click | [CMXsrv_finobl_bus_cor](#cmxsrv_finobl_bus_cor) | COR |
| proximo_Click | [CMXsrv_finobl_bus_cor](#cmxsrv_finobl_bus_cor) | COR |
| ELIMINAR_Click | [CMXsrv_finobl_ecuo](#cmxsrv_finobl_ecuo) | OBL, CTO |
| form_activate | [CMXsrv_finobl_gpln](#cmxsrv_finobl_gpln) | OBL, CTO |
| form_activate | [CMXsrv_finobl_cons_plnpa](#cmxsrv_finobl_cons_plnpa) | OBL, CTO |
| anunctb_Click | [CMXsrv_finobl_calc_anu](#cmxsrv_finobl_calc_anu) | OBL |
| form_activate | [CMXsrv_finobl_lee_obl](#cmxsrv_finobl_lee_obl) | TIP, COR, OBL, ACMXINTERE, ACMXMONEDA, ACMXSUCSAL, CLN |
| Form_Load | [CMXsrv_lee_fpro](#cmxsrv_lee_fpro) | ACMXFECPRO |
| Mcbeanl_Click | [CMXsrv_finobl_calc_anu](#cmxsrv_finobl_calc_anu) | OBL |
| Mcbectb_Click | [CMXsrv_finobl_ctb_oto](#cmxsrv_finobl_ctb_oto) | ACMXDESEMB, TIP, COD, OBL, CTO, CCO |
| Mcbedel_Click | [CMXsrv_fincol_eli_obl](#cmxsrv_fincol_eli_obl) | OBL, OBL_ADI |
| Mobl_liq_ope_Click | [CMXsrv_icrd_dat_liq_ope](#cmxsrv_icrd_dat_liq_ope) | ACMXDESEMB, ASND, EVO, CRD, CNO, OBL, CUO, TRSD, NEG, COM, EVE, ACMXTIPEVE, CAN, COL |
| valida_error | [CMXsrv_finobl_val_obl](#cmxsrv_finobl_val_obl) | TIP, OBL, ACMXINTERE, warnmsg, OBL_ADI |
| buscar_Click | [CMXsrv_finobl_bsc_obl](#cmxsrv_finobl_bsc_obl) | OBL |
| fld_obl_tip_ope_LostFocus | [CMXsrv_fincol_lee_tip](#cmxsrv_fincol_lee_tip) | TIP |
| Proxima_Click | [CMXsrv_finobl_bsc_obl](#cmxsrv_finobl_bsc_obl) | OBL |
| contabilizar_Click | [CMXsrv_finobl_ictb_pag](#cmxsrv_finobl_ictb_pag) | OBL, CTO, EVO |
| contabilizar_Click | [CMXsrv_finobl_obt_sdocuo](#cmxsrv_finobl_obt_sdocuo) | OBL, CTO |
| form_activate | [CMXsrv_finobl_new_tas](#cmxsrv_finobl_new_tas) | CTO |
| form_activate | [CMXsrv_finobl_cons_pag](#cmxsrv_finobl_cons_pag) | CNO |
| form_activate | [CMXsrv_finobl_cons_detp](#cmxsrv_finobl_cons_detp) | OBL, CTO, EVO |
| calcular_Click | [CMXsrv_finobl_calc_pror](#cmxsrv_finobl_calc_pror) | OBL |
| form_activate | [CMXsrv_finobl_cons_pror](#cmxsrv_finobl_cons_pror) | OBL, EVO |
| form_activate | [CMXsrv_finobl_cons_dpror](#cmxsrv_finobl_cons_dpror) | OBL, EVO |
| contabilizar_Click | [CMXsrv_finobl_ctb_anu](#cmxsrv_finobl_ctb_anu) | TIP, COR, OBL, COL, CTO |
| calcular_Click | [CMXsrv_finobl_calc_anu](#cmxsrv_finobl_calc_anu) | OBL |
| form_activate | [CMXsrv_finobl_cons_anu](#cmxsrv_finobl_cons_anu) | CNO, EVO |
| form_activate | [CMXsrv_finobl_cons_mod](#cmxsrv_finobl_cons_mod) | OBL, EVO |
| form_activate | [CMXsrv_finobl_cons_dmod](#cmxsrv_finobl_cons_dmod) | CNO, EVO |
| efectuar_Click | [CMXsrv_finobl_rev_eve](#cmxsrv_finobl_rev_eve) | OBL, TRSD, APRCBL, EVO |
| form_activate | [CMXsrv_finobl_cons_eve](#cmxsrv_finobl_cons_eve) | EVO |
| form_activate | [CMXsrv_finobl_cons_deve](#cmxsrv_finobl_cons_deve) | EVO |
| ELIMINAR_Click | [CMXsrv_finobl_eli_ctr](#cmxsrv_finobl_eli_ctr) | CTR |
| form_activate | [CMXsrv_finobl_cons_ctr](#cmxsrv_finobl_cons_ctr) | CTR |
| nuevo_Click | [CMXsrv_finobl_ing_ctr](#cmxsrv_finobl_ing_ctr) | COL, OBL, TIP, CTR |
| aceptar_Click | [CMXsrv_finobl_cesion_obl](#cmxsrv_finobl_cesion_obl) | OBL, COR |
| banco_acreedor | [CMXsrv_comgrl_lee_nom_cor](#cmxsrv_comgrl_lee_nom_cor) | COR |
| fld_obl_cod_bco_acre_lostfocus | [CMXsrv_comgrl_lee_nom_cor](#cmxsrv_comgrl_lee_nom_cor) | COR |
| fld_obl_rut_acre_lostfocus | [CMXsrv_lee_cln](#cmxsrv_lee_cln) | CLN |
| form_activate | [CMXsrv_finobl_busc_acre](#cmxsrv_finobl_busc_acre) | OBL |
| Form_Load | [CMXsrv_cmx_get_codes](#cmxsrv_cmx_get_codes) |  |

---

## PAGOS
<a name="pagos"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tabla Referenciada** |
|-------------|-----------------------------|----------------------|
| CALCULAR_Click | [CMXsrv_fincol_efec_calpa](#cmxsrv_fincol_efec_calpa) | TF_PPAG, TIP, TAS, CUO, comex..ACMXMONEDA, COL_ADI, OBL, CTR, NEG_ADI, ACMXINTERE, CAN, ICR, COL |
| Form_Activate | [CMXsrv_fincol_cons_pag](#cmxsrv_fincol_cons_pag) | CAN, COL |
| Form_Load | [CMXsrv_fincol_cons_detp](#cmxsrv_fincol_cons_detp) | ACMXDESEMB, EVE, COL, CUO |
| Aceptar_Click | [CMXsrv_fincol_calc_pror](#cmxsrv_fincol_calc_pror) | ACMXINTERE, COL |
| Contabilizar_Click | [CMXsrv_fincol_cont_pror](#cmxsrv_fincol_cont_pror) | TAS, CRD, NEG_ADI, ACMXINTERE, TIP, CUO, OBL, CAM_TAS, ACMXPLAZO, COL_ADI, LIB, ACMXINTEREFEC, CLN, ACMXOPEIMP, CTO, de, comex..ACMXINTEREFEC, COD, COM, ACMXMONEDAFEC, EVE, CAN, COL |
| Form_Activate | [CMXsrv_fincol_cons_pror](#cmxsrv_fincol_cons_pror) | EVE, COL |
| Form_Activate | [CMXsrv_fincol_cons_dpror](#cmxsrv_fincol_cons_dpror) | ACMXDESEMB, EVE, COL |
| Aceptar_Click | [CMXsrv_busc_cod_ope](#cmxsrv_busc_cod_ope) | TIP, COL |
| Aceptar_Click | [CMXsrv_col_trae_num_ope](#cmxsrv_col_trae_num_ope) | COL |
| Aceptar_Click | [CMXsrv_fincol_cctb_anu](#cmxsrv_fincol_cctb_anu) | TIP, CUO, COD, OBL, TF_ENL, ENL, CAN, COL, CTO |
| Form_Load | [CMXsrv_fincol_calc_anu](#cmxsrv_fincol_calc_anu) | TIP, COL |
| Form_Load | [CMXsrv_busc_cod_ope](#cmxsrv_busc_cod_ope) | TIP, COL |
| CALCULAR_Click | [CMXsrv_fincol_calc_anu](#cmxsrv_fincol_calc_anu) | TIP, COL |
| Form_Activate | [CMXsrv_fincol_cons_anu](#cmxsrv_fincol_cons_anu) | ACMXDESEMB, CAN, EVE, COL |
| Form_Activate | [CMXsrv_fincol_cons_mod](#cmxsrv_fincol_cons_mod) | EVE, COL |
| Form_Activate | [CMXsrv_fincol_cons_dmod](#cmxsrv_fincol_cons_dmod) | CAN, EVE |
| Form_Load | [CMXsrv_lee_fpro](#cmxsrv_lee_fpro) | ACMXFECPRO |
| Form_Load | [CMXsrv_grl_trae_cod_bco](#cmxsrv_grl_trae_cod_bco) |  |

---

## PGOEXT
<a name="pgoext"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tabla Referenciada** |
|-------------|-----------------------------|----------------------|
| calcular_Click | [CMXsrv_fincol_cal_pext](#cmxsrv_fincol_cal_pext) | TIP, CUO, comex..ACMXMONEDA, OBL, CTR, COL, CTO |
| Contabilizar_Click | [CMXsrv_busc_cod_ope](#cmxsrv_busc_cod_ope) | TIP, COL |
| Contabilizar_Click | [CMXsrv_fincol_ctb_pext](#cmxsrv_fincol_ctb_pext) | TIP, ACMXDESEMB, comex..ACMXINTEREFEC, TAS, CUO, COD, OBL, COL_ADI, ACMXMONEDAFEC, CTR, NEG_ADI, ACMXINTERE, EVE, ACMXINTEREFEC, COL, CTO, CCO |
| calcular_Click | [CMXsrv_finobl_cal_pext](#cmxsrv_finobl_cal_pext) | TIP, OBL, ACMXINTERE, ACMXMONEDA, OBL_ADI, CTO |
| Contabilizar_Click | [CMXsrv_finobl_ctb_pext](#cmxsrv_finobl_ctb_pext) | ACMXDESEMB, TIP, COD, OBL, ACMXMONEDAFEC, CTO, CCO |
| Form_Load | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |  |
| Form_Load | [CMXsrv_lee_fpro](#cmxsrv_lee_fpro) | ACMXFECPRO |

---

## ARCOS
<a name="arcos"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tabla Referenciada** |
|-------------|-----------------------------|----------------------|
| Eliminar_Click | [CMXsrv_iarc_eli_arc](#cmxsrv_iarc_eli_arc) | ADI, CRD, ARC, NEG, COB, INF, COL |
| Form_activate | [CMXsrv_iarc_busc_arc](#cmxsrv_iarc_busc_arc) | ARC |
| aceptar_click | [CMXsrv_iinf_busc_inf](#cmxsrv_iinf_busc_inf) | INF |
| aceptar_click | [CMXsrv_iarc_act_arc](#cmxsrv_iarc_act_arc) | CRD, comex..ACMXMONEDA, ARC, NEG, CBR, ACMXMONEDAFEC, INF, COL |
| Form_Load | [CMXsrv_iarc_lee_arc](#cmxsrv_iarc_lee_arc) | ARC |
| buscar_Click | [CMXsrv_iinf_busc_opr](#cmxsrv_iinf_busc_opr) | ARC |
| Form_activate | [CMXsrv_iinf_lee_vlr](#cmxsrv_iinf_lee_vlr) | INF |
| aceptar_click | [CMXsrv_iarc_act_arc](#cmxsrv_iarc_act_arc) | CRD, comex..ACMXMONEDA, ARC, NEG, CBR, ACMXMONEDAFEC, INF, COL |
| Form_activate | [CMXsrv_iinf_busc_inf](#cmxsrv_iinf_busc_inf) | INF |
| reversar_Click | [CMXsrv_iinf_rev_evi](#cmxsrv_iinf_rev_evi) | INF, ARC, INC, EVI |

---

## COBERIMP
<a name="coberimp"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tabla Referenciada** |
|-------------|-----------------------------|----------------------|
| Form_Activate | [CMXsrv_icob_lee_pln](#cmxsrv_icob_lee_pln) | DIC, POSBCX10, COB, ACMXBCOCEN, ACMXMONEDA, ACMXPAIS |
| Mcobcur_Click | [CMXsrv_icob_cur_cob](#cmxsrv_icob_cur_cob) | comex.dbo, COB |
| Mcobcur_Click | [CMXsrv_icob_pag_sop](#cmxsrv_icob_pag_sop) | DDI, ACMXDESEMB, ADI, DIC, ACMXPRMGRL, ACMXMONEDAFEC, COB, INF, warnmsg |
| MCOBELI_CLICK | [CMXsrv_icob_eli_pln](#cmxsrv_icob_eli_pln) | COB |
| Mcobrev_Click | [CMXsrv_icob_rev_etd](#cmxsrv_icob_rev_etd) | POSBCX10, TRSD, PSO, comex..COB, COB |
| Mcobvali_Click | [CMXsrv_icob_val_cob](#cmxsrv_icob_val_cob) | DDI, LCB, ADI, CUO, ARC, NEG, CBR, COB, INF, ACMXFPAIMP, warnmsg, COL |
| buscar_click | [CMXsrv_icob_busc_pln](#cmxsrv_icob_busc_pln) | COB |
| FLD_COB_COD_CLI_LostFocus | [CMXsrv_icob_lee_cln](#cmxsrv_icob_lee_cln) | CLN |
| PROXIMAS_Click | [CMXsrv_icob_busc_pln](#cmxsrv_icob_busc_pln) | COB |
| ACEPTAR_Click | [CMXsrv_icob_crea_norm](#cmxsrv_icob_crea_norm) | CRD, ARC, CBR, COB, INF, tbl_User, CLN, COL |
| ACEPTAR_Click | [CMXsrv_icob_crea_reem](#cmxsrv_icob_crea_reem) | DIC, COB |
| ACEPTAR_Click | [CMXsrv_icob_act_gral](#cmxsrv_icob_act_gral) | CLN, COB |
| FLD_COB_COD_CLI_LostFocus | [CMXsrv_icob_lee_cln2](#cmxsrv_icob_lee_cln2) | CLN |
| Form_Activate | [CMXsrv_icob_lee_gral](#cmxsrv_icob_lee_gral) | ACMXBCOCEN, ACMXPAIS, COB |
| ACEPTAR_Click | [CMXsrv_icob_act_val](#cmxsrv_icob_act_val) | ACMXMONEDAFEC, COB |
| Form_Activate | [CMXsrv_icob_lee_val](#cmxsrv_icob_lee_val) | COB |
| ACEPTAR_Click | [CMXsrv_icob_act_acu](#cmxsrv_icob_act_acu) | COB |
| Form_Activate | [CMXsrv_icob_lee_acu](#cmxsrv_icob_lee_acu) | ACMXPAIS, COB |
| Form_Load | [CMXsrv_icob_lee_acu](#cmxsrv_icob_lee_acu) | ACMXPAIS, COB |
| ELIMINAR_Click | [CMXsrv_icob_eli_int](#cmxsrv_icob_eli_int) | DIC, COB |
| Form_Activate | [CMXsrv_icob_busc_int](#cmxsrv_icob_busc_int) | DIC |
| ACEPTAR_Click | [CMXsrv_icob_ingmod_int](#cmxsrv_icob_ingmod_int) | DIC, COB |
| Form_Activate | [CMXsrv_icob_lee_int](#cmxsrv_icob_lee_int) | DIC |
| ACEPTAR_Click | [CMXsrv_icob_ing_mod_srf](#cmxsrv_icob_ing_mod_srf) | CLN, tbl_User, COB |
| CmdEliminar_Click | [CMXsrv_icob_eli_pln](#cmxsrv_icob_eli_pln) | COB |
| CmdReversar_Click | [CMXsrv_icob_rev_etd](#cmxsrv_icob_rev_etd) | POSBCX10, TRSD, PSO, comex..COB, COB |
| CURSAR_Click | [CMXsrv_icob_ing_mod_srf](#cmxsrv_icob_ing_mod_srf) | CLN, tbl_User, COB |
| CURSAR_Click | [CMXsrv_icob_pag_sop](#cmxsrv_icob_pag_sop) | DDI, ACMXDESEMB, ADI, DIC, ACMXPRMGRL, ACMXMONEDAFEC, COB, INF, warnmsg |
| FLD_COB_COD_CLI_LostFocus | [CMXsrv_icob_lee_cln2](#cmxsrv_icob_lee_cln2) | CLN |
| Reversar_Click | [CMXsrv_icob_rev_etd](#cmxsrv_icob_rev_etd) | POSBCX10, TRSD, PSO, comex..COB, COB |
| ACEPTAR_Click | [CMXsrv_icob_anu](#cmxsrv_icob_anu) | DIC, POSBCX10, ACMXMONEDAFEC, PSO, COB, ACMXTPOAUTN |
| Form_Load | [CMXsrv_icob_lee_anu](#cmxsrv_icob_lee_anu) | COB |
| FLD_COB_COD_CLI_LostFocus | [CMXsrv_icob_lee_cln](#cmxsrv_icob_lee_cln) | CLN |
| ACEPTAR_Click | [CMXsrv_icob_pag_sop](#cmxsrv_icob_pag_sop) | DDI, ACMXDESEMB, ADI, DIC, ACMXPRMGRL, ACMXMONEDAFEC, COB, INF, warnmsg |
| ACEPTAR_Click | [CMXsrv_icob_cur_reem](#cmxsrv_icob_cur_reem) | comex..COB, COB |
| Form_Load | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |  |

---

## COBRANZA
<a name="cobranza"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tabla Referenciada** |
|-------------|-----------------------------|----------------------|
| ejecut_avi_imp_999 | [CMXsrv_busc_cor_swf](#cmxsrv_busc_cor_swf) | SWT |
| ejecut_avi_imp_999 | [CMXsrv_swf_bus_sms](#cmxsrv_swf_bus_sms) | SMS |
| Form_Activate | [CMXsrv_icbr_lee_cbr](#cmxsrv_icbr_lee_cbr) | ACMXPAIS, COR, LCB, ACMXVIATPT, ACMXBCOBCC, CBR, ACMXMONEDA, ACMXCLACOM, tbl_User, ACMXSUCSAL, CLN |
| Form_Load | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |  |
| Mcbrace_Click | [CMXsrv_icbr_acep_let](#cmxsrv_icbr_acep_let) | comex..CBR, LCB, CBR |
| Mcbrcon_Click | [CMXsrv_icbr_cont_cbr](#cmxsrv_icbr_cont_cbr) | OPE_BCI, APRCBL, LCB, CBR |
| Mcbreli_click | [CMXsrv_icbr_eli_cbr](#cmxsrv_icbr_eli_cbr) | ARC, REMENT, CBR, comex..COL |
| McbrTxt999_Click | [CMXsrv_icbr_lee_ctp](#cmxsrv_icbr_lee_ctp) | ACMXSUCSAL, MCBRCTP, CBR, ACMXPAIS, CLN, CBRANX |
| Mcbrtxtrec_Click | [CMXsrv_icbr_avi1](#cmxsrv_icbr_avi1) | ACMXDESEMB, ASND, ACMXBCOBCC, ARC, CBR, ACMXINTERE, PCX, ECE, ACMXMONEDA, ACMXSUCSAL, CLN |
| aceptar_Click | [CMXsrv_val_suc](#cmxsrv_val_suc) | ACMXSUCSAL, tbl_User |
| buscar_Click | [CMXsrv_icbr_busc_cbr](#cmxsrv_icbr_busc_cbr) | ACMXSUCSAL, ACMXMONEDA, CLN, CBR |
| fld_aux_glo_ofi_LostFocus | [CMXsrv_val_suc](#cmxsrv_val_suc) | ACMXSUCSAL, tbl_User |
| fld_cbr_cod_gdo_LostFocus | [CMXsrv_icbr_lee_cln](#cmxsrv_icbr_lee_cln) | CLN |
| fld_cbr_cod_ofi_lostfocus | [CMXsrv_val_suc](#cmxsrv_val_suc) | ACMXSUCSAL, tbl_User |
| proximas_Click | [CMXsrv_icbr_busc_cbr](#cmxsrv_icbr_busc_cbr) | ACMXSUCSAL, ACMXMONEDA, CLN, CBR |
| crear_Click | [CMXsrv_icbr_crea_cbr](#cmxsrv_icbr_crea_cbr) | CLN, tbl_User |
| fld_cbr_cod_gdo_LostFocus | [CMXsrv_icbr_lee_cln](#cmxsrv_icbr_lee_cln) | CLN |
| fld_cbr_cod_ofi_lostfocus | [CMXsrv_val_suc](#cmxsrv_val_suc) | ACMXSUCSAL, tbl_User |
| INGRESAR_Click | [CMXsrv_icbr_crea_cbr](#cmxsrv_icbr_crea_cbr) | CLN, tbl_User |
| fld_cbr_cod_gdo_LostFocus | [CMXsrv_icbr_lee_cln](#cmxsrv_icbr_lee_cln) | CLN |
| Form_Activate | [CMXsrv_icbr_lee_cob](#cmxsrv_icbr_lee_cob) | COB |
| Form_Load | [CMXsrv_icbr_lee_ctp](#cmxsrv_icbr_lee_ctp) | ACMXSUCSAL, MCBRCTP, CBR, ACMXPAIS, CLN, CBRANX |
| INGRESAR_Click | [CMXsrv_icbr_act_ctp](#cmxsrv_icbr_act_ctp) | comex..CBR, MCBRCTP, CBRANX, CBR |
| Form_Activate | [CMXsrv_icbr_lee_cob](#cmxsrv_icbr_lee_cob) | COB |
| Form_Load | [CMXsrv_icbr_lee_trm](#cmxsrv_icbr_lee_trm) | ACMXVIATPT, CBR, ACMXINTERE, ACMXMONEDA, MCBRTER, ACMXCLACOM, ACMXPAIS |
| INGRESAR_Click | [CMXsrv_icbr_act_trm](#cmxsrv_icbr_act_trm) | LCB, COM, CBR, MCBRTER, warnmsg, CLN |
| Form_Activate | [CMXsrv_icbr_lee_cob](#cmxsrv_icbr_lee_cob) | COB |
| Form_Load | [CMXsrv_icbr_lee_doc](#cmxsrv_icbr_lee_doc) | LCB, MCBRDOC, MLCB, CBR, ACMXMONEDA |
| INGRESAR_Click | [CMXsrv_icbr_act_doc](#cmxsrv_icbr_act_doc) | LCB, MCBRDOC, MLCB, CBR, comex..CBR |
| Form_Activate | [CMXsrv_icbr_busc_let](#cmxsrv_icbr_busc_let) | MLCB, comex..MLCB, comex..LCB |
| aceptar_Click | [CMXsrv_icbr_ingmod_let](#cmxsrv_icbr_ingmod_let) | LCB, CBR, comex.dbo |
| eliminar_Click | [CMXsrv_icbr_eli_let](#cmxsrv_icbr_eli_let) | LCB, MCBRDOC, MLCB, CBR, comex..COL |
| Form_Activate | [CMXsrv_icbr_lee_let](#cmxsrv_icbr_lee_let) | ACMXNOTARIO, LCB, MLCB |
| aceptar_Click | [CMXsrv_icbr_prorr](#cmxsrv_icbr_prorr) | comex..CBR, LCB, CBR |
| EFECTUAR_Click | [CMXsrv_icbr_rev_eve](#cmxsrv_icbr_rev_eve) | APRCBL, TRSD, CBR, vig_trs, ECE, DIP, LIB, tbl_User |
| Form_Activate | [CMXsrv_icbr_busc_eve](#cmxsrv_icbr_busc_eve) | ECE |
| Form_Load | [CMXsrv_icbr_lee_eve](#cmxsrv_icbr_lee_eve) | ECE, ACMXDESEMB |
| Form_Load | [CMXsrv_icbr_lee_ent_doc](#cmxsrv_icbr_lee_ent_doc) | CBR |
| aceptar_Click | [CMXsrv_icbr_prot](#cmxsrv_icbr_prot) | LCB, CBR |
| Form_Load | [CMXsrv_icbr_pcg_prot](#cmxsrv_icbr_pcg_prot) | LCB, CBR |
| aceptar_Click | [CMXsrv_icbr_liq_sdo](#cmxsrv_icbr_liq_sdo) | comex..CBR, LCB, CBR |
| aceptar_Click | [CMXsrv_icbr_act_vis](#cmxsrv_icbr_act_vis) | comex..CBR, CBR |
| eliminar_Click | [CMXsrv_icbr_eli_rep](#cmxsrv_icbr_eli_rep) | REP |
| Form_Activate | [CMXsrv_icbr_busc_rep](#cmxsrv_icbr_busc_rep) | REP |
| aceptar_Click | [CMXsrv_icbr_imod_rep](#cmxsrv_icbr_imod_rep) | REP, CBR |
| aceptar_Click | [CMXsrv_icbr_ent_doc](#cmxsrv_icbr_ent_doc) | comex..CBR, LCB, CBR |
| Form_Load | [CMXsrv_icbr_lee_ent_doc](#cmxsrv_icbr_lee_ent_doc) | CBR |
| aceptar_Click | [CMXsrv_icbr_trf_ofi](#cmxsrv_icbr_trf_ofi) | comex..CBR, ACMXSUCSAL, CBR |
| aceptar_Click | [CMXsrv_val_suc](#cmxsrv_val_suc) | ACMXSUCSAL, tbl_User |
| aceptar_Click | [CMXsrv_icbr_trf_bco](#cmxsrv_icbr_trf_bco) | comex..CBR, ARC, CBR, LCB |
| aceptar_Click | [CMXsrv_icbr_act_inst](#cmxsrv_icbr_act_inst) | comex..CBR, CBR |
| enviar_Click | [CMXsrv_iswf_a_pru](#cmxsrv_iswf_a_pru) | switxt, switxt1 |
| Form_Load | [CMXsrv_icbr_val_cbr](#cmxsrv_icbr_val_cbr) | DDI, LCB, COR, ADI, ARC, ACMXMONEDAFEC, CBR, ACMXINTEREFEC, warnmsg |
| word_Click | [CMXsrv_icbr_val_cbr](#cmxsrv_icbr_val_cbr) | DDI, LCB, COR, ADI, ARC, ACMXMONEDAFEC, CBR, ACMXINTEREFEC, warnmsg |
| word_Click | [CMXsrv_iswf_a_pru](#cmxsrv_iswf_a_pru) | switxt, switxt1 |

---

## CRDEXT
<a name="crdext"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tabla Referenciada** |
|-------------|-----------------------------|----------------------|
| Aceptar_Click | [CMXsrv_icrd_a_ibab](#cmxsrv_icrd_a_ibab) | MIBAB, IBAB |
| Form_Load | [CMXsrv_icrd_lee_glo_ibab](#cmxsrv_icrd_lee_glo_ibab) | IBAB, COL, MIBAB |
| Aceptar_Click | [CMXsrv_icrd_a_ibar](#cmxsrv_icrd_a_ibar) | MIBAR, IBAR |
| Form_Load | [CMXsrv_icrd_lee_glo_ibar](#cmxsrv_icrd_lee_glo_ibar) | MIBAR, COL, IBAR |
| buscar_click | [CMXsrv_icrd_lee_tex_swf](#cmxsrv_icrd_lee_tex_swf) | ACMXTSWFESPMSG, ACMXTSWFINGMSG |
| Aceptar_Click | [CMXsrv_icrd_lee_cod_txt_swf](#cmxsrv_icrd_lee_cod_txt_swf) | ACMXTSWFESPMSG, ACMXTSWFINGMSG |
| buscar_click | [CMXsrv_icrd_lee_txt_swf_all](#cmxsrv_icrd_lee_txt_swf_all) | ACMXTSWFESPMSG, ACMXTSWFINGMSG |
| Form_Load | [CMXsrv_icrd_lee_ind_esp_ing](#cmxsrv_icrd_lee_ind_esp_ing) | MCTP, CRD |
| llena_arreglo | [CMXsrv_icrd_lee_tex_swf](#cmxsrv_icrd_lee_tex_swf) | ACMXTSWFESPMSG, ACMXTSWFINGMSG |
| proximo_Click | [CMXsrv_icrd_lee_txt_swf_all](#cmxsrv_icrd_lee_txt_swf_all) | ACMXTSWFESPMSG, ACMXTSWFINGMSG |
| aceptar_Click | [CMXsrv_icrd_ing_acu](#cmxsrv_icrd_ing_acu) | CRD |
| Form_Load | [CMXsrv_icrd_lee_acu](#cmxsrv_icrd_lee_acu) | CRD |
| aceptar_Click | [CMXsrv_icrd_rech_sol](#cmxsrv_icrd_rech_sol) | CRD, comex..COL, OPE_BCI, COL, comex..CRD |
| aceptar_Click | [CMXsrv_icrd_end](#cmxsrv_icrd_end) | INF, ARC, COL, CRD |
| Form_Load | [CMXsrv_icrd_lee_dat_end](#cmxsrv_icrd_lee_dat_end) | CRD |
| aceptar_Click | [CMXsrv_icrd_asignar_cor](#cmxsrv_icrd_asignar_cor) | COR, ACMXMONEDAFEC, CRD, LCR |
| buscar_Click | [CMXsrv_icrd_bus_lcr_bco](#cmxsrv_icrd_bus_lcr_bco) | COR |
| proximo_Click | [CMXsrv_icrd_bus_lcr_bco](#cmxsrv_icrd_bus_lcr_bco) | COR |
| Form_Load | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |  |

---

## CRD_CORR
<a name="crd_corr"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tabla Referenciada** |
|-------------|-----------------------------|----------------------|
| aceptar_Click | [CMXsrv_icrd_asignar_cor](#cmxsrv_icrd_asignar_cor) | COR, ACMXMONEDAFEC, CRD, LCR |
| buscar_Click | [CMXsrv_icrd_bus_lcr_bco](#cmxsrv_icrd_bus_lcr_bco) | COR |
| fld_cor_cod_mtr_LostFocus | [CMXsrv_icrd_lee_bco_mtr](#cmxsrv_icrd_lee_bco_mtr) | comex..ACMXBANCOS |
| fld_cor_cod_pais_Lostfocus | [CMXsrv_icrd_cor_lee_pais](#cmxsrv_icrd_cor_lee_pais) | comex..ACMXPAIS |
| fld_cor_cod_plz_Lostfocus | [CMXsrv_icrd_lee_plz](#cmxsrv_icrd_lee_plz) | ACMXPLAZAS |
| proximo_Click | [CMXsrv_icrd_bus_lcr_bco](#cmxsrv_icrd_bus_lcr_bco) | COR |
| buscar_Click | [CMXsrv_icrd_busc_plz](#cmxsrv_icrd_busc_plz) | comex..ACMXPLAZAS |
| proximos_Click | [CMXsrv_icrd_busc_plz](#cmxsrv_icrd_busc_plz) | comex..ACMXPLAZAS |
| buscar_Click | [CMXsrv_icrd_cor_busc_pais](#cmxsrv_icrd_cor_busc_pais) | comex, comex..ACMXPAIS |
| proximos_Click | [CMXsrv_icrd_cor_busc_pais](#cmxsrv_icrd_cor_busc_pais) | comex, comex..ACMXPAIS |
| buscar_Click | [CMXsrv_icrd_busc_bco_mtr](#cmxsrv_icrd_busc_bco_mtr) | comex |
| proximos_Click | [CMXsrv_icrd_busc_bco_mtr](#cmxsrv_icrd_busc_bco_mtr) | comex |

---

## DDI
<a name="ddi"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tabla Referenciada** |
|-------------|-----------------------------|----------------------|
| aceptar_Click | [CMXsrv_iddi_ingmod_ddi](#cmxsrv_iddi_ingmod_ddi) | INF, DDI |
| continuar_Click | [CMXsrv_iddi_lee_dec](#cmxsrv_iddi_lee_dec) | DDI, ACMXVIATPT, ACMXRGMIMP, INF, ACMXBCOCEN, ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM, ACMXPAIS, CLN |
| eliminar_Click | [CMXsrv_iddi_eli_ddi](#cmxsrv_iddi_eli_ddi) | DDI |
| fld_ddi_fec_ii_lostfocus | [CMXsrv_iddi_lee_inf](#cmxsrv_iddi_lee_inf) | INF |
| fld_ddi_rut_imp_lostfocus | [CMXsrv_iddi_lee_cln](#cmxsrv_iddi_lee_cln) | CLN |
| Asociar_Click | [CMXsrv_iddi_lee_rut](#cmxsrv_iddi_lee_rut) | DDI |
| Asociar_Click | [CMXsrv_iddi_asoc_ddi](#cmxsrv_iddi_asoc_ddi) | DDI, ARC, ACMXMONEDAFEC, CBR, COB, INF, ACMXMONEDA, COL |
| Command2_Click | [CMXsrv_iddi_des_ddi](#cmxsrv_iddi_des_ddi) | DDI, ADI, COB |
| Desasociar_Click | [CMXsrv_iddi_lee_rut](#cmxsrv_iddi_lee_rut) | DDI |
| Desasociar_Click | [CMXsrv_iddi_des_ddi](#cmxsrv_iddi_des_ddi) | DDI, ADI, COB |
| fld_aux_rut_cli_lostfocus | [CMXsrv_iddi_lee_cln](#cmxsrv_iddi_lee_cln) | CLN |
| inicio_asoc | [CMXsrv_iddi_busc_asoc](#cmxsrv_iddi_busc_asoc) | ADI |
| inicio_noasoc | [CMXsrv_iddi_busc_noasoc](#cmxsrv_iddi_busc_noasoc) | DDI, ADI |
| proximo_no_aso_Click | [CMXsrv_iddi_busc_noasoc](#cmxsrv_iddi_busc_noasoc) | DDI, ADI |

---

## IMPORT
<a name="import"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tabla Referenciada** |
|-------------|-----------------------------|----------------------|
| buscar_Click | [CMXsrv_icrd_lee_dir_cln](#cmxsrv_icrd_lee_dir_cln) | DIRCLN |
| buscar_click | [CMXsrv_icrd_lee_tex_swf](#cmxsrv_icrd_lee_tex_swf) | ACMXTSWFESPMSG, ACMXTSWFINGMSG |
| Aceptar_Click | [CMXsrv_icrd_lee_cod_txt_swf](#cmxsrv_icrd_lee_cod_txt_swf) | ACMXTSWFESPMSG, ACMXTSWFINGMSG |
| buscar_click | [CMXsrv_icrd_lee_txt_swf_all](#cmxsrv_icrd_lee_txt_swf_all) | ACMXTSWFESPMSG, ACMXTSWFINGMSG |
| Form_Load | [CMXsrv_icrd_lee_ind_esp_ing](#cmxsrv_icrd_lee_ind_esp_ing) | MCTP, CRD |
| llena_arreglo | [CMXsrv_icrd_lee_tex_swf](#cmxsrv_icrd_lee_tex_swf) | ACMXTSWFESPMSG, ACMXTSWFINGMSG |
| proximo_Click | [CMXsrv_icrd_lee_txt_swf_all](#cmxsrv_icrd_lee_txt_swf_all) | ACMXTSWFESPMSG, ACMXTSWFINGMSG |
| Aceptar_Click | [CMXCRDsrv_icrd_a_cnd_esp](#cmxcrdsrv_icrd_a_cnd_esp) | CND |
| Form_Load | [CMXsrv_icrd_lee_cnd_esp](#cmxsrv_icrd_lee_cnd_esp) | MMCND, COL, CND |
| clon_Click | [CMXCRDsrv_icrd_clon_crd](#cmxcrdsrv_icrd_clon_crd) | CRS, MER, CRD, TAS, CRDCLON, COL_ADI, CND, DAC, ODOC, AVAL, COL, EMB |
| Form_Activate | [CMXCRDsrv_icrd_lee_crdcre](#cmxcrdsrv_icrd_lee_crdcre) | CRD_ADI, ACMXFORPAG, ACMXPAIS, ACMXVIATPT, CRD, COR, COL_ADI, ACMXFINVER, PMIX, NEG, ACMXMONEDA, tbl_User, OPE_BCI, ACMXSUCSAL, CLN, COL, DIRCLN, EMB |
| Form_Activate | [CMXsrv_icrd_lee_ind_esp_ing](#cmxsrv_icrd_lee_ind_esp_ing) | MCTP, CRD |
| Form_Activate | [CMXsrv_icrd_lee_top](#cmxsrv_icrd_lee_top) | COL |
| Form_Load | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |  |
| Form_Load | [CMXsrv_cmx_get_codes](#cmxsrv_cmx_get_codes) |  |
| Form_Load | [CMXsrv_trae_glo_fec](#cmxsrv_trae_glo_fec) | ACMXSUCSAL, ACMXDL3475FEC, tbl_User |
| Mcrdapr_Click | [CMXCRDsrv_icrd_val_crd](#cmxcrdsrv_icrd_val_crd) | warnmsg |
| Mcrdeli_click | [CMXCRDsrv_icrd_eli_crd](#cmxcrdsrv_icrd_eli_crd) | comex..COL, OPE_BCI, CRD |
| Mcrdtxtliq_Click | [CMXsrv_icrd_lee_dat_trs](#cmxsrv_icrd_lee_dat_trs) | ASND, EVI, TRSD, EVE, ACMXMONEDA, COL |
| Mcrdtxtope_Click | [CMXsrv_icrd_dat_liq_ope](#cmxsrv_icrd_dat_liq_ope) | ACMXDESEMB, ASND, EVO, CRD, CNO, OBL, CUO, TRSD, NEG, COM, EVE, ACMXTIPEVE, CAN, COL |
| msg_swift | [CMXsrv_iswf_a_pru](#cmxsrv_iswf_a_pru) | switxt, switxt1 |
| Aceptar_Click | [CMXsrv_icrd_a_ctp](#cmxsrv_icrd_a_ctp) | CRD, CRDCLON, MCTP, comex..COL, COL |
| FLD_COL_COD_CLI_LostFocus | [CMXsrv_icrd_lee_cln](#cmxsrv_icrd_lee_cln) | CLN, DIRCLN |
| Form_Load | [CMXsrv_lee_fpro](#cmxsrv_lee_fpro) | ACMXFECPRO |
| Aceptar_Click | [CMXsrv_icrd_a_cnd](#cmxsrv_icrd_a_cnd) | TIP, CRD_ADI, CRD, CRDCLON, COL_ADI, COM, ACMXMONEDA, LIB, comex..COL, MAPR, MCND, COL, ACMXOPEIMP, comex..CRD |
| Aceptar_Click | [CMXCRDsrv_icrd_crea_crd](#cmxcrdsrv_icrd_crea_crd) | CRD_ADI, PMIX, ACMXMONEDA, CLN, COL |
| fld_col_fec_vto_LostFocus | [CMXsrv_util_det_habil](#cmxsrv_util_det_habil) | ACMXFERIADO |
| Form_Activate | [CMXsrv_icrd_busc_emb](#cmxsrv_icrd_busc_emb) | comex..EMB, comex..MEMB |
| ELIMINAR_Click | [CMXsrv_icrd_eli_emb](#cmxsrv_icrd_eli_emb) | comex..COL, EMB, COL, CRD |
| Form_Load | [CMXsrv_icrd_lee_emb1](#cmxsrv_icrd_lee_emb1) | CRS, COL, EMB |
| Form_Load | [CMXsrv_icrd_lee_emb2](#cmxsrv_icrd_lee_emb2) | COL, EMB |
| ingresar_Click | [CMXsrv_icrd_a_emb1](#cmxsrv_icrd_a_emb1) | CRS, MEMB, CRD, MCRS, CRDCLON, COL, EMB |
| ingresar_Click | [CMXsrv_icrd_a_emb2](#cmxsrv_icrd_a_emb2) | EMB, COL, MEMB, CRD |
| VALIDA_EMBARQUE | [CMXsrv_icrd_val_emb2](#cmxsrv_icrd_val_emb2) | warnmsg |
| VALIDA_EMBARQUE | [CMXsrv_icrd_val_emb1](#cmxsrv_icrd_val_emb1) | INF, ARC, warnmsg |
| Aceptar_Click | [CMXsrv_icrd_act_ref](#cmxsrv_icrd_act_ref) | MREF, CRD, CRDCLON, comex..MREF, comex..COL, COL |
| Form_Load | [CMXsrv_icrd_act_ref](#cmxsrv_icrd_act_ref) | MREF, CRD, CRDCLON, comex..MREF, comex..COL, COL |
| Form_Load | [CMXsrv_icrd_lee_ref](#cmxsrv_icrd_lee_ref) | COR, COL, CRD |
| FLD_COL_COD_CLI_LostFocus | [CMXsrv_icrd_lee_cln](#cmxsrv_icrd_lee_cln) | CLN, DIRCLN |
| Aceptar_Click | [CMXCRDsrv_icrd_apr_sol](#cmxcrdsrv_icrd_apr_sol) | TIP, CRD, COL_ADI, COM, LIB, OPE_BCI, sysobjects, CLN, COL |
| Form_Load | [CMXsrv_icrd_lee_crdapr](#cmxsrv_icrd_lee_crdapr) | CRS, CRD, COL_ADI, DAC, ACMXAPROBAC |
| Aceptar_Click | [CMXsrv_icrd_rech_sol](#cmxsrv_icrd_rech_sol) | CRD, comex..COL, OPE_BCI, COL, comex..CRD |
| Aceptar_Click | [CMXCRDsrv_icrd_a_desc_merc](#cmxcrdsrv_icrd_a_desc_merc) | MER |
| Form_Load | [CMXsrv_icrd_lee_desc_merc](#cmxsrv_icrd_lee_desc_merc) | MMER, MER |
| Aceptar_Click | [CMXsrv_icrd_a_otr_doc](#cmxsrv_icrd_a_otr_doc) | ODOC, MODOC |
| Form_Load | [CMXsrv_icrd_lee_otr_doc](#cmxsrv_icrd_lee_otr_doc) | ODOC, MODOC |
| enviar_Click | [CMXsrv_iswf_a_pru](#cmxsrv_iswf_a_pru) | switxt, switxt1 |

---

## INFORME
<a name="informe"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tabla Referenciada** |
|-------------|-----------------------------|----------------------|
| Eliminar_Click | [CMXsrv_iarc_eli_arc](#cmxsrv_iarc_eli_arc) | ADI, CRD, ARC, NEG, COB, INF, COL |
| Form_Activate | [CMXsrv_iarc_busc_arc](#cmxsrv_iarc_busc_arc) | ARC |
| Form_Activate | [CMXsrv_iinf_lee0_inf](#cmxsrv_iinf_lee0_inf) | INF |
| Form_Activate | [CMXsrv_iinf_lee_tablas](#cmxsrv_iinf_lee_tablas) | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM |
| Form_Activate | [CMXsrv_iinf_lee1_inf](#cmxsrv_iinf_lee1_inf) | INF, CLN |
| Form_Activate | [CMXsrv_iinf_lee_cln](#cmxsrv_iinf_lee_cln) | CLN |
| Form_Activate | [CMXsrv_iinf_lee2_inf](#cmxsrv_iinf_lee2_inf) | INF |
| Form_Activate | [CMXsrv_iinf_avi_miscb](#cmxsrv_iinf_avi_miscb) | INF |
| Maviapr_Click | [CMXsrv_iinf_avi_misca](#cmxsrv_iinf_avi_misca) | INF, CLN |
| Maviapr_Click | [CMXsrv_iinf_avi_miscb](#cmxsrv_iinf_avi_miscb) | INF |
| Mavicom_Click | [CMXsrv_iinf_avi_misca](#cmxsrv_iinf_avi_misca) | INF, CLN |
| Mavicom_Click | [CMXsrv_iinf_avi_miscb](#cmxsrv_iinf_avi_miscb) | INF |
| Mavicom_Click | [CMXsrv_icrd_lee_dat_com](#cmxsrv_icrd_lee_dat_com) | TIP, ACMXDESEMB, ASND, CRD, EVI, COM, TRSD, EVE, ACMXMONEDA |
| Mavimis1_Click | [CMXsrv_iinf_avi_misca](#cmxsrv_iinf_avi_misca) | INF, CLN |
| Mavimis1_Click | [CMXsrv_iinf_avi_miscb](#cmxsrv_iinf_avi_miscb) | INF |
| Mavimis2_Click | [CMXsrv_iinf_avi_misca](#cmxsrv_iinf_avi_misca) | INF, CLN |
| Mavimis2_Click | [CMXsrv_iinf_avi_miscb](#cmxsrv_iinf_avi_miscb) | INF |
| Mavirec_Click | [CMXsrv_iinf_avi_misca](#cmxsrv_iinf_avi_misca) | INF, CLN |
| Mavirec_Click | [CMXsrv_iinf_avi_miscb](#cmxsrv_iinf_avi_miscb) | INF |
| Mavitib_Click | [CMXsrv_iinf_avi_misca](#cmxsrv_iinf_avi_misca) | INF, CLN |
| Mavitib_Click | [CMXsrv_iinf_avi_miscb](#cmxsrv_iinf_avi_miscb) | INF |
| Mavitras_Click | [CMXsrv_iinf_avi_misca](#cmxsrv_iinf_avi_misca) | INF, CLN |
| Mavitras_Click | [CMXsrv_iinf_avi_miscb](#cmxsrv_iinf_avi_miscb) | INF |
| Mavitras_Click | [CMXsrv_icrd_lee_dat_trs](#cmxsrv_icrd_lee_dat_trs) | ASND, EVI, TRSD, EVE, ACMXMONEDA, COL |
| Minfoeli_click | [CMXsrv_iinf_eli_inf](#cmxsrv_iinf_eli_inf) | INF, ARC |
| Minforev_Click | [CMXsrv_iinf_busc_evi](#cmxsrv_iinf_busc_evi) | EVI |
| Minfoval_click | [CMXsrv_iinf_val_inf](#cmxsrv_iinf_val_inf) | INF, ACMXPAIS, warnmsg |
| Aceptar_Click | [CMXsrv_iinf_ingmod_inf](#cmxsrv_iinf_ingmod_inf) | INF, tbl_User, warnmsg |
| Fec_pre | [CMXsrv_iinf_lee_fec](#cmxsrv_iinf_lee_fec) |  |
| fld_aux_glo_cls_com_LostFocus | [CMXsrv_iinf_lee_tablas](#cmxsrv_iinf_lee_tablas) | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM |
| fld_aux_glo_for_pag1_LostFocus | [CMXsrv_iinf_lee_tablas](#cmxsrv_iinf_lee_tablas) | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM |
| fld_aux_glo_for_pag2_LostFocus | [CMXsrv_iinf_lee_tablas](#cmxsrv_iinf_lee_tablas) | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM |
| fld_aux_glo_for_pag3_LostFocus | [CMXsrv_iinf_lee_tablas](#cmxsrv_iinf_lee_tablas) | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM |
| fld_aux_glo_mon_LostFocus | [CMXsrv_iinf_lee_tablas](#cmxsrv_iinf_lee_tablas) | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM |
| fld_inf_cls_com_Lostfocus | [CMXsrv_iinf_lee_tablas](#cmxsrv_iinf_lee_tablas) | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM |
| fld_inf_cod_imp_LostFocus | [CMXsrv_iinf_lee_cln](#cmxsrv_iinf_lee_cln) | CLN |
| fld_inf_for_pag1_lostfocus | [CMXsrv_iinf_lee_tablas](#cmxsrv_iinf_lee_tablas) | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM |
| fld_inf_for_pag2_LostFocus | [CMXsrv_iinf_lee_tablas](#cmxsrv_iinf_lee_tablas) | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM |
| fld_inf_for_pag3_LostFocus | [CMXsrv_iinf_lee_tablas](#cmxsrv_iinf_lee_tablas) | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM |
| fld_inf_mon_inf_lostfocus | [CMXsrv_iinf_lee_tablas](#cmxsrv_iinf_lee_tablas) | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM |
| Form_Load | [CMXsrv_iinf_lee0_inf](#cmxsrv_iinf_lee0_inf) | INF |
| Form_Load | [CMXsrv_iinf_lee1_inf](#cmxsrv_iinf_lee1_inf) | INF, CLN |
| Form_Load | [CMXsrv_iinf_lee2_inf](#cmxsrv_iinf_lee2_inf) | INF |
| valor_usd | [CMXsrv_iinf_lee_usd](#cmxsrv_iinf_lee_usd) |  |
| Aceptar_Click | [CMXsrv_iinf_busc_inf](#cmxsrv_iinf_busc_inf) | INF |
| buscar_Click | [CMXsrv_iinf_busc_inf](#cmxsrv_iinf_busc_inf) | INF |
| Fec_pre | [CMXsrv_iinf_lee_fec](#cmxsrv_iinf_lee_fec) |  |
| fld_inf_cod_imp_LostFocus | [CMXsrv_iinf_lee_cln](#cmxsrv_iinf_lee_cln) | CLN |
| PROXIMA_Click | [CMXsrv_iinf_busc_inf](#cmxsrv_iinf_busc_inf) | INF |
| Aceptar_Click | [CMXsrv_iinf_act_apr](#cmxsrv_iinf_act_apr) | INF |
| Form_Activate | [CMXsrv_iinf_busc_evi](#cmxsrv_iinf_busc_evi) | EVI |
| reversar_Click | [CMXsrv_iinf_rev_evi](#cmxsrv_iinf_rev_evi) | INF, ARC, INC, EVI |
| Form_Load | [CMXsrv_iinf_lee_evi](#cmxsrv_iinf_lee_evi) | EVI |
| Aceptar_Click | [CMXsrv_iinf_act_tib](#cmxsrv_iinf_act_tib) | INF |
| Aceptar_Click | [CMXsrv_iinf_act_rec](#cmxsrv_iinf_act_rec) | INF |
| Aceptar_Click | [CMXsrv_iinf_act_rib](#cmxsrv_iinf_act_rib) | INF |
| Form_Activate | [CMXsrv_iinf_busc_comp](#cmxsrv_iinf_busc_comp) | INF |
| proximos_Click | [CMXsrv_iinf_busc_comp](#cmxsrv_iinf_busc_comp) | INF |
| Aceptar_Click | [CMXsrv_iinf_ingmod_comp](#cmxsrv_iinf_ingmod_comp) | INF, warnmsg |
| Fec_pre | [CMXsrv_iinf_lee_fec](#cmxsrv_iinf_lee_fec) |  |
| Form_Activate | [CMXsrv_iinf_lee_comp](#cmxsrv_iinf_lee_comp) | INF |
| Form_Activate | [CMXsrv_iinf_lee_tablas](#cmxsrv_iinf_lee_tablas) | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM |
| aceptar_click | [CMXsrv_iinf_lee_bco](#cmxsrv_iinf_lee_bco) | COR |
| buscar_Click | [CMXsrv_iinf_busc_bco](#cmxsrv_iinf_busc_bco) | ACMXBCOBCC |
| Form_Load | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |  |

---

## MOD_ADI
<a name="mod_adi"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tabla Referenciada** |
|-------------|-----------------------------|----------------------|
| Aceptar_Click | [CMXsrv_icrd_a_cnd](#cmxsrv_icrd_a_cnd) | TIP, CRD_ADI, CRD, CRDCLON, COL_ADI, COM, ACMXMONEDA, LIB, comex..COL, MAPR, MCND, COL, ACMXOPEIMP, comex..CRD |
| busca_bco | [CMXsrv_icrd_lee_bco_swf](#cmxsrv_icrd_lee_bco_swf) | ACMXPAIS, COR |
| fld_col_fec_vto_LostFocus | [CMXsrv_util_det_habil](#cmxsrv_util_det_habil) | ACMXFERIADO |
| Form_Load | [CMXMCRDsrv_icrd_lee_mcnd](#cmxmcrdsrv_icrd_lee_mcnd) | CRD_ADI, ACMXFORPAG, CRD, PMIX, ACMXMONEDA, MPMIX, MCND |
| Form_Load | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |  |

---

## MOD_CBR
<a name="mod_cbr"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tabla Referenciada** |
|-------------|-----------------------------|----------------------|
| fld_cbr_cod_gdo_LostFocus | [CMXsrv_icbr_lee_cln](#cmxsrv_icbr_lee_cln) | CLN |
| Form_Load | [CMXsrv_icbr_lee_ctp](#cmxsrv_icbr_lee_ctp) | ACMXSUCSAL, MCBRCTP, CBR, ACMXPAIS, CLN, CBRANX |
| INGRESAR_Click | [CMXsrv_icbr_act_ctp](#cmxsrv_icbr_act_ctp) | comex..CBR, MCBRCTP, CBRANX, CBR |
| Form_Load | [CMXsrv_icbr_lee_trm](#cmxsrv_icbr_lee_trm) | ACMXVIATPT, CBR, ACMXINTERE, ACMXMONEDA, MCBRTER, ACMXCLACOM, ACMXPAIS |
| INGRESAR_Click | [CMXsrv_icbr_act_trm](#cmxsrv_icbr_act_trm) | LCB, COM, CBR, MCBRTER, warnmsg, CLN |
| Form_Load | [CMXsrv_icbr_lee_doc](#cmxsrv_icbr_lee_doc) | LCB, MCBRDOC, MLCB, CBR, ACMXMONEDA |
| INGRESAR_Click | [CMXsrv_icbr_act_doc](#cmxsrv_icbr_act_doc) | LCB, MCBRDOC, MLCB, CBR, comex..CBR |
| Form_Activate | [CMXsrv_icbr_busc_let](#cmxsrv_icbr_busc_let) | MLCB, comex..MLCB, comex..LCB |
| aceptar_Click | [CMXsrv_icbr_mod_ing_let](#cmxsrv_icbr_mod_ing_let) | LCB, MLCB, CBR, end |
| eliminar_Click | [CMXsrv_icbr_eli_let](#cmxsrv_icbr_eli_let) | LCB, MCBRDOC, MLCB, CBR, comex..COL |
| Form_Activate | [CMXsrv_icbr_lee_let](#cmxsrv_icbr_lee_let) | ACMXNOTARIO, LCB, MLCB |
| actualizar_Click | [CMXsrv_icbr_acep_mod_cbr](#cmxsrv_icbr_acep_mod_cbr) | LCB, MCBRDOC, MCBRCTP, MLCB, CBR, MCBRTER, warnmsg |
| Cancelar_Click | [CMXsrv_icbr_eli_no_cont](#cmxsrv_icbr_eli_no_cont) | MCBRDOC, MCBRCTP, MLCB, CBR, MCBRTER |

---

## MOD_CRD
<a name="mod_crd"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tabla Referenciada** |
|-------------|-----------------------------|----------------------|
| Aceptar_Click | [CMXsrv_icrd_a_ibab](#cmxsrv_icrd_a_ibab) | MIBAB, IBAB |
| Form_Load | [CMXsrv_icrd_lee_glo_ibab](#cmxsrv_icrd_lee_glo_ibab) | IBAB, COL, MIBAB |
| Aceptar_Click | [CMXsrv_icrd_a_ibar](#cmxsrv_icrd_a_ibar) | MIBAR, IBAR |
| Form_Load | [CMXsrv_icrd_lee_glo_ibar](#cmxsrv_icrd_lee_glo_ibar) | MIBAR, COL, IBAR |
| buscar_click | [CMXsrv_icrd_lee_dir_cln](#cmxsrv_icrd_lee_dir_cln) | DIRCLN |
| buscar_Click | [CMXsrv_icrd_lee_tex_swf](#cmxsrv_icrd_lee_tex_swf) | ACMXTSWFESPMSG, ACMXTSWFINGMSG |
| buscar_click | [CMXsrv_icrd_lee_tex_swf](#cmxsrv_icrd_lee_tex_swf) | ACMXTSWFESPMSG, ACMXTSWFINGMSG |
| Aceptar_Click | [CMXsrv_icrd_lee_cod_txt_swf](#cmxsrv_icrd_lee_cod_txt_swf) | ACMXTSWFESPMSG, ACMXTSWFINGMSG |
| buscar_click | [CMXsrv_icrd_lee_txt_swf_all](#cmxsrv_icrd_lee_txt_swf_all) | ACMXTSWFESPMSG, ACMXTSWFINGMSG |
| Form_Load | [CMXsrv_icrd_lee_ind_esp_ing](#cmxsrv_icrd_lee_ind_esp_ing) | MCTP, CRD |
| llena_arreglo | [CMXsrv_icrd_lee_tex_swf](#cmxsrv_icrd_lee_tex_swf) | ACMXTSWFESPMSG, ACMXTSWFINGMSG |
| proximo_Click | [CMXsrv_icrd_lee_txt_swf_all](#cmxsrv_icrd_lee_txt_swf_all) | ACMXTSWFESPMSG, ACMXTSWFINGMSG |
| Aceptar_Click | [CMXMCRDsrv_icrd_a_mmcnd](#cmxmcrdsrv_icrd_a_mmcnd) | MMCND |
| Form_Load | [CMXsrv_icrd_lee_cnd_esp](#cmxsrv_icrd_lee_cnd_esp) | MMCND, COL, CND |
| Aceptar_Click | [CMXsrv_icrd_a_ctp](#cmxsrv_icrd_a_ctp) | CRD, CRDCLON, MCTP, comex..COL, COL |
| FLD_COL_COD_CLI_LostFocus | [CMXsrv_icrd_lee_cln](#cmxsrv_icrd_lee_cln) | CLN, DIRCLN |
| Form_Load | [CMXMCRDsrv_icrd_lee_mctp](#cmxmcrdsrv_icrd_lee_mctp) | ACMXPAIS, MCTP, DIRCLN, CRD |
| Aceptar_Click | [CMXsrv_icrd_a_cnd](#cmxsrv_icrd_a_cnd) | TIP, CRD_ADI, CRD, CRDCLON, COL_ADI, COM, ACMXMONEDA, LIB, comex..COL, MAPR, MCND, COL, ACMXOPEIMP, comex..CRD |
| Form_Load | [CMXMCRDsrv_icrd_lee_mcnd](#cmxmcrdsrv_icrd_lee_mcnd) | CRD_ADI, ACMXFORPAG, CRD, PMIX, ACMXMONEDA, MPMIX, MCND |
| Form_Activate | [CMXsrv_icrd_busc_emb](#cmxsrv_icrd_busc_emb) | comex..EMB, comex..MEMB |
| cancelar_Click | [CMXsrv_icrd_lee_desc_merc](#cmxsrv_icrd_lee_desc_merc) | MMER, MER |
| ELIMINAR_Click | [CMXsrv_icrd_eli_emb](#cmxsrv_icrd_eli_emb) | comex..COL, EMB, COL, CRD |
| Form_Load | [CMXMCRDsrv_icrd_lee_memb2](#cmxmcrdsrv_icrd_lee_memb2) | MEMB, EMB |
| Form_Load | [CMXMCRDsrv_icrd_lee_memb1](#cmxmcrdsrv_icrd_lee_memb1) | CRS, MEMB, EMB, MCRS |
| ingresar_Click | [CMXsrv_icrd_a_emb1](#cmxsrv_icrd_a_emb1) | CRS, MEMB, CRD, MCRS, CRDCLON, COL, EMB |
| ingresar_Click | [CMXsrv_icrd_a_emb2](#cmxsrv_icrd_a_emb2) | EMB, COL, MEMB, CRD |
| VALIDA_EMBARQUE | [CMXsrv_icrd_val_emb2](#cmxsrv_icrd_val_emb2) | warnmsg |
| VALIDA_EMBARQUE | [CMXsrv_icrd_val_emb1](#cmxsrv_icrd_val_emb1) | INF, ARC, warnmsg |
| Aceptar_Click | [CMXsrv_icrd_act_ref](#cmxsrv_icrd_act_ref) | MREF, CRD, CRDCLON, comex..MREF, comex..COL, COL |
| fld_obl_cod_bco_acre_DblClick | [CMXsrv_icrd_lee_bco_swf](#cmxsrv_icrd_lee_bco_swf) | ACMXPAIS, COR |
| fld_obl_cod_bco_acre_LostFocus | [CMXsrv_icrd_lee_bco_swf](#cmxsrv_icrd_lee_bco_swf) | ACMXPAIS, COR |
| Form_Load | [CMXMCRDsrv_icrd_lee_mref](#cmxmcrdsrv_icrd_lee_mref) | MREF, COR, COL, CRD |
| Aceptar_Click | [CMXsrv_icrd_ing_txt](#cmxsrv_icrd_ing_txt) | MTXT |
| Form_Load | [CMXCRDsrv_icrd_get_ing_esp](#cmxcrdsrv_icrd_get_ing_esp) | ACMXPAIS, MCTP, CRD |
| Form_Load | [CMXMCRDsrv_icrd_lee_mtxt](#cmxmcrdsrv_icrd_lee_mtxt) | MTXT |
| Form_Load | [CMXCRDsrv_icrd_get_pre_fra](#cmxcrdsrv_icrd_get_pre_fra) | ACMXTSWFESPMSG, ACMXTSWFINGMSG |
| Aceptar_Click | [CMXMCRDsrv_icrd_a_mmer](#cmxmcrdsrv_icrd_a_mmer) | MMER |
| Form_Load | [CMXsrv_icrd_lee_desc_merc](#cmxsrv_icrd_lee_desc_merc) | MMER, MER |
| Aceptar_Click | [CMXsrv_icrd_a_otr_doc](#cmxsrv_icrd_a_otr_doc) | ODOC, MODOC |
| Form_Load | [CMXsrv_icrd_lee_otr_doc](#cmxsrv_icrd_lee_otr_doc) | ODOC, MODOC |
| Aceptar_Click | [CMXsrv_fincol_lee_cod_eve](#cmxsrv_fincol_lee_cod_eve) | MCND, COL, CRD, COM |
| Aceptar_Click | [CMXMCRDsrv_icrd_acep_mod_crd](#cmxmcrdsrv_icrd_acep_mod_crd) | de, TIP, CRD, COD, MCRS, OBL, EVE, LIB, warnmsg, OPE_BCI, sysobjects, COL |
| cancelar_Click | [CMXMCRDsrv_icrd_eli_no_cont](#cmxmcrdsrv_icrd_eli_no_cont) | MREF, MEMB, MCRS, MMCND, COM, MODOC, MIBAB, CRD_AMD, MPMIX, MCTP, MMER, MCND, MIBAR, TNIH, MAPR, FE_IN_REJECTED_TRANS, MTXT |
| fld_crd_cod_bco_rem_LostFocus | [CMXsrv_icrd_lee_bco_swf](#cmxsrv_icrd_lee_bco_swf) | ACMXPAIS, COR |
| fld_crd_fec_mod_lostFocus | [CMXsrv_fincol_efec_calpa](#cmxsrv_fincol_efec_calpa) | TF_PPAG, TIP, TAS, CUO, comex..ACMXMONEDA, COL_ADI, OBL, CTR, NEG_ADI, ACMXINTERE, CAN, ICR, COL |
| Form_Activate | [CMXsrv_icrd_lee_ind_esp_ing](#cmxsrv_icrd_lee_ind_esp_ing) | MCTP, CRD |
| Form_Load | [CMXsrv_fincol_efec_calpa](#cmxsrv_fincol_efec_calpa) | TF_PPAG, TIP, TAS, CUO, comex..ACMXMONEDA, COL_ADI, OBL, CTR, NEG_ADI, ACMXINTERE, CAN, ICR, COL |
| Form_Load | [CMXMCRDsrv_icrd_lee_mcnd](#cmxmcrdsrv_icrd_lee_mcnd) | CRD_ADI, ACMXFORPAG, CRD, PMIX, ACMXMONEDA, MPMIX, MCND |
| Form_Load | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |  |

---

## NEGO_AV
<a name="nego_av"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tabla Referenciada** |
|-------------|-----------------------------|----------------------|
| aviso1 | [CMXsrv_icrd_a_rec_age](#cmxsrv_icrd_a_rec_age) | COR, TAS, CRD, CUO, CNEG, COM, NEG, TRSD, DIS, EVE, ACMXMONEDA, ACMXINTERE, ACMXSUCSAL, COL |
| aviso1 | [CMXsrv_busc_ofi_cta](#cmxsrv_busc_ofi_cta) | CLN |
| aviso1 | [CMXsrv_neg_busc_arc](#cmxsrv_neg_busc_arc) | ARC |
| aviso1 | [CMXsrv_icrd_lee_avi_adi](#cmxsrv_icrd_lee_avi_adi) | CRD |
| aviso3 | [CMXsrv_icrd_lee_dat_trs](#cmxsrv_icrd_lee_dat_trs) | ASND, EVI, TRSD, EVE, ACMXMONEDA, COL |
| Aviso4 | [CMXsrv_icrd_dat_liq_ope](#cmxsrv_icrd_dat_liq_ope) | ACMXDESEMB, ASND, EVO, CRD, CNO, OBL, CUO, TRSD, NEG, COM, EVE, ACMXTIPEVE, CAN, COL |
| Aviso4 | [CMXsrv_icrd_lee_dat_cln](#cmxsrv_icrd_lee_dat_cln) | NEG, CLN, COL |
| Aviso5 | [CMXsrv_icrd_lee_dat_cln](#cmxsrv_icrd_lee_dat_cln) | NEG, CLN, COL |
| Aviso5 | [CMXsrv_icrd_lee_avi_dis](#cmxsrv_icrd_lee_avi_dis) | DIS, COL |
| Aviso5 | [CMXsrv_icrd_lee_avi_adi](#cmxsrv_icrd_lee_avi_adi) | CRD |
| Aviso5 | [CMXsrv_neg_ddi_asoc](#cmxsrv_neg_ddi_asoc) | ADI |
| Aviso5 | [CMXsrv_neg_busc_arc](#cmxsrv_neg_busc_arc) | ARC |
| Aviso5 | [CMXsrv_neg_trae_vcto_mcf](#cmxsrv_neg_trae_vcto_mcf) | COL, CUO |
| lee_aval | [CMXsrv_neg_avi_lee_aval](#cmxsrv_neg_avi_lee_aval) | TAS, CNEG, AVAL, CLN, COL |
| lee_nego | [CMXsrv_icrd_neg_lee_crd](#cmxsrv_icrd_neg_lee_crd) | NEG, COL |
| lee_nego | [CMXsrv_icrd_lee_neg](#cmxsrv_icrd_lee_neg) | TAS, CRD, ACMXFINVER, NEG, NEG_ADI, DIS, COL |
| avi_col1 | [CMXsrv_col_avi_dat_cln](#cmxsrv_col_avi_dat_cln) | TIP, CRD, DAC, ACMXESPECI, ACMXSUCSAL, CLN, COL, ACLNEJECTA |
| avi_col1 | [CMXsrv_col_avi_det_pag](#cmxsrv_col_avi_det_pag) | CCX, TIP, TAS, CRD, COB, ACMXINTERE, EVE, ACMXMONEDA, ACMXINTEREFEC, CAN, CAN_REN, COL |
| avi_col2 | [CMXsrv_col_avi_dat_cln](#cmxsrv_col_avi_dat_cln) | TIP, CRD, DAC, ACMXESPECI, ACMXSUCSAL, CLN, COL, ACLNEJECTA |
| avi_col2 | [CMXsrv_col_avi_det_oto](#cmxsrv_col_avi_det_oto) | TIP, ACMXDESEMB, ASND, TAS, CUO, COD, NEG, ACMXINTERE, EVE, ACMXMONEDA, ACMXINTEREFEC, AVAL, CLN, COL |
| avi_col4 | [CMXsrv_col_avi_dat_cln](#cmxsrv_col_avi_dat_cln) | TIP, CRD, DAC, ACMXESPECI, ACMXSUCSAL, CLN, COL, ACLNEJECTA |
| avi_col4 | [CMXsrv_col_lee_num_trs](#cmxsrv_col_lee_num_trs) | EVE, COL, TIP, COD |
| lee_obl_pag | [CMXsrv_finobl_avi_pag](#cmxsrv_finobl_avi_pag) | CNO, EVO |
| traspaso | [CMXsrv_neg_avi_trae_asnd_mn](#cmxsrv_neg_avi_trae_asnd_mn) | ACMXDESEMB, ASND, COD, TRSD, ACMXMONEDA |
| traspaso | [CMXsrv_neg_avi_trae_asnd_mx](#cmxsrv_neg_avi_trae_asnd_mx) | ACMXDESEMB, ACMXMONEDA, ASND |
| Form_Activate | [CMXsrv_icrd_neg_lee_crd](#cmxsrv_icrd_neg_lee_crd) | NEG, COL |
| Form_Activate | [CMXsrv_icrd_lee_neg](#cmxsrv_icrd_lee_neg) | TAS, CRD, ACMXFINVER, NEG, NEG_ADI, DIS, COL |
| Mcrdtxtliq_Click | [CMXsrv_icrd_lee_dat_trs](#cmxsrv_icrd_lee_dat_trs) | ASND, EVI, TRSD, EVE, ACMXMONEDA, COL |
| Mcrdtxtope_Click | [CMXsrv_icrd_dat_liq_ope](#cmxsrv_icrd_dat_liq_ope) | ACMXDESEMB, ASND, EVO, CRD, CNO, OBL, CUO, TRSD, NEG, COM, EVE, ACMXTIPEVE, CAN, COL |
| MNEGCONT_Click | [CMXsrv_icrd_cont_neg](#cmxsrv_icrd_cont_neg) | COL, NEG, CRD, COD |
| MNEGELI_CLICK | [CMXsrv_icrd_eli_neg](#cmxsrv_icrd_eli_neg) | CRD, COM, NEG, CND, NEG_ADI, ACMXTXTSWF, comex..COL |
| precarga_datos | [CMXsrv_icrd_a_rec_age](#cmxsrv_icrd_a_rec_age) | COR, TAS, CRD, CUO, CNEG, COM, NEG, TRSD, DIS, EVE, ACMXMONEDA, ACMXINTERE, ACMXSUCSAL, COL |
| precarga_datos | [CMXsrv_busc_ofi_cta](#cmxsrv_busc_ofi_cta) | CLN |
| Form_Load | [CMXsrv_trae_glo_fec](#cmxsrv_trae_glo_fec) | ACMXSUCSAL, ACMXDL3475FEC, tbl_User |
| Form_Load | [CMXsrv_icrd_lee_num_col](#cmxsrv_icrd_lee_num_col) | COL |
| Form_Load | [CMXsrv_icrd_bus_pago](#cmxsrv_icrd_bus_pago) | CAN |

---

## NNEGO
<a name="nnego"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tabla Referenciada** |
|-------------|-----------------------------|----------------------|
| Form_Activate | [CMXsrv_icrd_neg_lee_crd](#cmxsrv_icrd_neg_lee_crd) | NEG, COL |
| Form_Activate | [CMXsrv_icrd_lee_neg](#cmxsrv_icrd_lee_neg) | TAS, CRD, ACMXFINVER, NEG, NEG_ADI, DIS, COL |
| gen_mens_swift | [CMXsrv_iswf_a_pru](#cmxsrv_iswf_a_pru) | switxt, switxt1 |
| llama_pagos | [CMXsrv_icrd_lee_col](#cmxsrv_icrd_lee_col) | CCL, COL, TAS |
| Mnegavi9_Click | [CMXsrv_iswf_a_pru](#cmxsrv_iswf_a_pru) | switxt, switxt1 |
| MNEGCONT_Click | [CMXsrv_icrd_cont_neg](#cmxsrv_icrd_cont_neg) | COL, NEG, CRD, COD |
| MNEGELI_CLICK | [CMXsrv_icrd_eli_neg](#cmxsrv_icrd_eli_neg) | CRD, COM, NEG, CND, NEG_ADI, ACMXTXTSWF, comex..COL |
| pertas_Click | [CMXsrv_icrd_lee_col](#cmxsrv_icrd_lee_col) | CCL, COL, TAS |
| Form_Activate | [CMXsrv_icrd_busc_neg](#cmxsrv_icrd_busc_neg) | NEG |
| Form_Load | [CMXsrv_icrd_busc_emb](#cmxsrv_icrd_busc_emb) | comex..EMB, comex..MEMB |
| ACEPTAR_Click | [CMXsrv_icrd_a_neg_emb1](#cmxsrv_icrd_a_neg_emb1) | TAS, CNEG, NEG, COL, DOCNEG |
| ACEPTAR_Click | [CMXsrv_icrd_a_neg_emb2](#cmxsrv_icrd_a_neg_emb2) | NEG, COL, comex..COL, DOCNEG |
| CANCELAR_Click | [CMXsrv_icrd_eli_doc_neg](#cmxsrv_icrd_eli_doc_neg) | COL, DOCNEG |
| Form_Activate | [CMXsrv_icrd_lee_emb1](#cmxsrv_icrd_lee_emb1) | CRS, COL, EMB |
| Form_Activate | [CMXsrv_icrd_lee_emb2](#cmxsrv_icrd_lee_emb2) | COL, EMB |
| Form_Activate | [CMXsrv_icrd_lee_neg_emb1](#cmxsrv_icrd_lee_neg_emb1) | COL, NEG |
| Form_Activate | [CMXsrv_icrd_lee_neg_emb2](#cmxsrv_icrd_lee_neg_emb2) | COL, NEG |
| Form_Activate | [CMXsrv_icrd_lee_cnd_esp](#cmxsrv_icrd_lee_cnd_esp) | MMCND, COL, CND |
| Form_Activate | [CMXsrv_icrd_lee_desc_merc](#cmxsrv_icrd_lee_desc_merc) | MMER, MER |
| ACEPTAR_Click | [CMXsrv_icrd_a_neg_disc](#cmxsrv_icrd_a_neg_disc) | COL, DIS, NEG |
| Form_Load | [CMXsrv_icrd_neg_lee_disc](#cmxsrv_icrd_neg_lee_disc) | DIS, NEG |
| ACEPTAR_Click | [CMXsrv_icrd_ent_doc](#cmxsrv_icrd_ent_doc) | COL, NEG, comex..COL |
| ELIMINAR_Click | [CMXsrv_icrd_ent_doc](#cmxsrv_icrd_ent_doc) | COL, NEG, comex..COL |
| Form_Load | [CMXsrv_icrd_ent_doc](#cmxsrv_icrd_ent_doc) | COL, NEG, comex..COL |
| ACEPTAR_Click | [CMXsrv_icrd_alz_disc](#cmxsrv_icrd_alz_disc) | comex..ACMXINTEREFEC, COR, TAS, CRD, CUO, COD, CNEG, NEG, ACMXMONEDAFEC, NEG_ADI, ACMXINTERE, ACMXBCOUSU, ACMXINTEREFEC, sysobjects, COL |
| aceptar_click | [CMXCRDsrv_icrd_asignar_cor](#cmxcrdsrv_icrd_asignar_cor) | COR, ACMXMONEDAFEC, CRD, LCR |
| BUSCAR_Click | [CMXCRDsrv_icrd_bus_lcr_bco](#cmxcrdsrv_icrd_bus_lcr_bco) | COR |
| proximo_Click | [CMXCRDsrv_icrd_bus_lcr_bco](#cmxcrdsrv_icrd_bus_lcr_bco) | COR |
| ACEPTAR_Click | [CMXsrv_icrd_act_doc_neg](#cmxsrv_icrd_act_doc_neg) | NEG, COL, DOCNEG |
| Form_Load | [CMXsrv_icrd_lee_doc_neg](#cmxsrv_icrd_lee_doc_neg) | NEG, EMB |
| enviar_Click | [CMXsrv_iswf_a_pru](#cmxsrv_iswf_a_pru) | switxt, switxt1 |
| Form_Load | [CMXsrv_icrd_val_neg](#cmxsrv_icrd_val_neg) | DDI, COR, ADI, TAS, CUO, NEG, ACMXMONEDAFEC, DAC, ACMXINTERE, ACMXMONEDA, ACMXSIGGAR, ACMXINTEREFEC, CAN, DIS, warnmsg, AVAL, COL, CCO |
| Form_Load | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |  |
| Form_Load | [CMXsrv_icrd_bus_pago](#cmxsrv_icrd_bus_pago) | CAN |

---

## PAGCBR
<a name="pagcbr"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tabla Referenciada** |
|-------------|-----------------------------|----------------------|
| ACEPTAR_Click | [CMXsrv_icbr_lee_dat_var](#cmxsrv_icbr_lee_dat_var) | ACMXMONEDAFEC, CBR, ACMXPRMENL |
| ACEPTAR_Click | [CMXsrv_icbr_val_pag](#cmxsrv_icbr_val_pag) | LCB, CBR, CCO |
| ACEPTAR_Click | [CMXsrv_icbr_ctb_pag](#cmxsrv_icbr_ctb_pag) | LCB, ACMXDESEMB, vig_cmx, COD, ICX, COM, ACMXMONEDAFEC, CBR, PCX, DIP, LIB, CLN, CCO |
| Calcular_Click | [CMXsrv_icbr_cal_pag](#cmxsrv_icbr_cal_pag) | DDI, ADI, ACMXMONEDAFEC, CBR, COB, ACMXMONEDA |
| CANCELAR_Click | [CMXsrv_icbr_eli_pag](#cmxsrv_icbr_eli_pag) | ECE, PCX, COB, ICX |
| fld_cbr_cod_des_mn_pag_lostfocus | [CMXsrv_val_vig](#cmxsrv_val_vig) | ACMXPLNCTAN, ACMXDESEMB, ACMXPLNCTAX |
| fld_cbr_cod_des_mx_pag_lostfocus | [CMXsrv_val_vig](#cmxsrv_val_vig) | ACMXPLNCTAN, ACMXDESEMB, ACMXPLNCTAX |
| Form_Load | [CMXsrv_icbr_lee_cbr0](#cmxsrv_icbr_lee_cbr0) | ACMXMONEDA, CBR |
| Form_Load | [CMXsrv_icbr_obt_mon_nac](#cmxsrv_icbr_obt_mon_nac) |  |
| Form_Load | [CMXsrv_icbr_lee_dat_pag](#cmxsrv_icbr_lee_dat_pag) | ACMXDESEMB, ECE, PCX, CBR |
| Form_Load | [CMXsrv_icbr_pcg_pag](#cmxsrv_icbr_pcg_pag) | ACMXMONEDAFEC, CBR |
| lee_cta | [CMXsrv_vig_lee_cta](#cmxsrv_vig_lee_cta) | ACMXPLNCTAN, ACMXDESEMB, ACMXPLNCTAX |
| Form_Activate | [CMXsrv_icbr_busc_pago](#cmxsrv_icbr_busc_pago) | PCX |
| ACEPTAR_Click | [CMXsrv_icbr_val_pag](#cmxsrv_icbr_val_pag) | LCB, CBR, CCO |
| Aceptar_Click | [CMXsrv_icob_act_val](#cmxsrv_icob_act_val) | ACMXMONEDAFEC, COB |
| Form_Activate | [CMXsrv_icob_lee_val](#cmxsrv_icob_lee_val) | COB |
| ELIMINAR_Click | [CMXsrv_icbr_eli_int_pago](#cmxsrv_icbr_eli_int_pago) | PCX, ICX |
| Form_Activate | [CMXsrv_icbr_busc_int](#cmxsrv_icbr_busc_int) | ICX |
| Aceptar_Click | [CMXsrv_icbr_ingmod_int](#cmxsrv_icbr_ingmod_int) | PCX, CBR, ICX, ACMXINTEREFEC |
| Form_Activate | [CMXsrv_icbr_lee_int_pago](#cmxsrv_icbr_lee_int_pago) | ICX |
| Aceptar_Click | [CMXsrv_icbr_lee_bco](#cmxsrv_icbr_lee_bco) | ACMXPAIS, COR |
| buscar_Click | [CMXsrv_icbr_busc_bco](#cmxsrv_icbr_busc_bco) | COR |
| Form_Load | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |  |

---

# Procedimientos Referenciados

## CMXsrv_expcbe_lee_prm
<a name="cmxsrv_expcbe_lee_prm"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)

---

## CMXsrv_cmx_busc_suc_usu
<a name="cmxsrv_cmx_busc_suc_usu"></a>

**Procedimientos Referenciados:**

- [PrmACMXSUCSAL](#referencia-prmacmxsucsal)
- [CMXsrv_cmx_ing_lib](#referencia-cmxsrv_cmx_ing_lib)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_lee_cbe
<a name="cmxsrv_expcbe_lee_cbe"></a>

**Procedimientos Referenciados:**

- [CMXsrv_cmx_busc_suc_usu](#referencia-cmxsrv_cmx_busc_suc_usu)
- [CMXsrv_val_suc](#referencia-cmxsrv_val_suc)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)

---

## CMXsrv_trae_glo_fec
<a name="cmxsrv_trae_glo_fec"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_avs_cyg1
<a name="cmxsrv_expcbe_avs_cyg1"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_avs_cyg2
<a name="cmxsrv_expcbe_avs_cyg2"></a>

**Procedimientos Referenciados:**

- [por](#referencia-por)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_avs_ret
<a name="cmxsrv_expcbe_avs_ret"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_swf_sel
<a name="cmxsrv_expcbe_swf_sel"></a>

**Procedimientos Referenciados:**

- [CMXsrv_expcbe_swf_422](#referencia-cmxsrv_expcbe_swf_422)
- [CMXsrv_expcbe_swf_420](#referencia-cmxsrv_expcbe_swf_420)
- [CMXsrv_expcbe_swf_499](#referencia-cmxsrv_expcbe_swf_499)
- [CMXsrv_expcbe_swf_430](#referencia-cmxsrv_expcbe_swf_430)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_anl_cbe
<a name="cmxsrv_expcbe_anl_cbe"></a>

**Procedimientos Referenciados:**

- [CMXsrv_cnt_gen_vig](#referencia-cmxsrv_cnt_gen_vig)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_expcbe_grb_evz](#referencia-cmxsrv_expcbe_grb_evz)
- [CMXsrv_cnt_950](#referencia-cmxsrv_cnt_950)
- [CMXsrv_cnt_630](#referencia-cmxsrv_cnt_630)

---

## CMXsrv_expcbe_ctb_ing
<a name="cmxsrv_expcbe_ctb_ing"></a>

**Procedimientos Referenciados:**

- [CMXsrv_cnt_600](#referencia-cmxsrv_cnt_600)
- [CMXsrv_mbyte_gen](#referencia-cmxsrv_mbyte_gen)
- [CMXsrv_nibx_upd_tran](#referencia-cmxsrv_nibx_upd_tran)
- [CMXsrv_cnt_gen_vig](#referencia-cmxsrv_cnt_gen_vig)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_expcbe_grb_evz](#referencia-cmxsrv_expcbe_grb_evz)
- [CMXsrv_cnt_950](#referencia-cmxsrv_cnt_950)
- [CMXsrv_expcbe_val_cbe](#referencia-cmxsrv_expcbe_val_cbe)
- [CMXsrv_nibx_nilive](#referencia-cmxsrv_nibx_nilive)

---

## CMXsrv_expcbe_del_cbe
<a name="cmxsrv_expcbe_del_cbe"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_val_cbe
<a name="cmxsrv_expcbe_val_cbe"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_grb_ctp
<a name="cmxsrv_expcbe_grb_ctp"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_lee_cln
<a name="cmxsrv_expcbe_lee_cln"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_val_suc
<a name="cmxsrv_val_suc"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_lee_ctp
<a name="cmxsrv_expcbe_lee_ctp"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_grb_bco
<a name="cmxsrv_expcbe_grb_bco"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_lee_cor
<a name="cmxsrv_expcbe_lee_cor"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_lee_bco
<a name="cmxsrv_expcbe_lee_bco"></a>

**Procedimientos Referenciados:**

- [CMXsrv_icrd_lee_cln](#referencia-cmxsrv_icrd_lee_cln)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_grb_doc
<a name="cmxsrv_expcbe_grb_doc"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_grb_doc02
<a name="cmxsrv_expcbe_grb_doc02"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_lee_doc
<a name="cmxsrv_expcbe_lee_doc"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_lee_doc02
<a name="cmxsrv_expcbe_lee_doc02"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_del_ctz
<a name="cmxsrv_expcbe_del_ctz"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_bus_ctz
<a name="cmxsrv_expcbe_bus_ctz"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_grb_ctz
<a name="cmxsrv_expcbe_grb_ctz"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_mto_ctz
<a name="cmxsrv_expcbe_mto_ctz"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_lee_ctz
<a name="cmxsrv_expcbe_lee_ctz"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_bus_cbe
<a name="cmxsrv_expcbe_bus_cbe"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_mdf_cbe
<a name="cmxsrv_expcbe_mdf_cbe"></a>

**Procedimientos Referenciados:**

- [CMXsrv_expcbe_grb_evl](#referencia-cmxsrv_expcbe_grb_evl)
- [CMXsrv_expcbe_act_ctz](#referencia-cmxsrv_expcbe_act_ctz)
- [CMXsrv_cnt_gen_vig](#referencia-cmxsrv_cnt_gen_vig)
- [CMXsrv_cnt_610](#referencia-cmxsrv_cnt_610)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_expcbe_grb_evz](#referencia-cmxsrv_expcbe_grb_evz)
- [CMXsrv_cnt_950](#referencia-cmxsrv_cnt_950)
- [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)

---

## CMXsrv_expcbe_cre_actz
<a name="cmxsrv_expcbe_cre_actz"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_lee_mdf
<a name="cmxsrv_expcbe_lee_mdf"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_pgo_cbe
<a name="cmxsrv_expcbe_pgo_cbe"></a>

**Procedimientos Referenciados:**

- [CMXsrv_mbyte_gen](#referencia-cmxsrv_mbyte_gen)
- [CMXsrv_expret_grb_org](#referencia-cmxsrv_expret_grb_org)
- [CMXsrv_expret_grb_dtn](#referencia-cmxsrv_expret_grb_dtn)
- [CMXsrv_cnt_gen_vig](#referencia-cmxsrv_cnt_gen_vig)
- [CMXsrv_expret_cre_ret](#referencia-cmxsrv_expret_cre_ret)
- [CMXsrv_vig_gra_vig](#referencia-cmxsrv_vig_gra_vig)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_expcbe_grb_evz](#referencia-cmxsrv_expcbe_grb_evz)
- [CMXsrv_cnt_950](#referencia-cmxsrv_cnt_950)
- [CMXsrv_exp_ipuc_gen_pln](#referencia-cmxsrv_exp_ipuc_gen_pln)
- [CMXsrv_expcbe_trp_cyg](#referencia-cmxsrv_expcbe_trp_cyg)
- [CMXsrv_expret_grb_det](#referencia-cmxsrv_expret_grb_det)
- [CMXsrv_cnt_620](#referencia-cmxsrv_cnt_620)

---

## CMXsrv_expcbe_lee_pgo
<a name="cmxsrv_expcbe_lee_pgo"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)

---

## CMXsrv_expcbe_bus_evz
<a name="cmxsrv_expcbe_bus_evz"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_rev_cbe
<a name="cmxsrv_expcbe_rev_cbe"></a>

**Procedimientos Referenciados:**

- [por](#referencia-por)
- [CMXsrv_mbyte_gen](#referencia-cmxsrv_mbyte_gen)
- [CMXsrv_cnt_rev_vig](#referencia-cmxsrv_cnt_rev_vig)
- [CMXsrv_expcbe_rev_trp](#referencia-cmxsrv_expcbe_rev_trp)
- [CMXsrv_ctl_chq_aprcbl](#referencia-cmxsrv_ctl_chq_aprcbl)
- [CMXsrv_rev_950](#referencia-cmxsrv_rev_950)
- [CMXsrv_cnt_610](#referencia-cmxsrv_cnt_610)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_expcbe_grb_evz](#referencia-cmxsrv_expcbe_grb_evz)
- [CMXsrv_cnt_631](#referencia-cmxsrv_cnt_631)
- [CMXsrv_cnt_601](#referencia-cmxsrv_cnt_601)
- [CMXsrv_cnt_621](#referencia-cmxsrv_cnt_621)
- [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)

---

## CMXsrv_expcbe_lee_evz
<a name="cmxsrv_expcbe_lee_evz"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_del_dcz
<a name="cmxsrv_expcbe_del_dcz"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_bus_dcz
<a name="cmxsrv_expcbe_bus_dcz"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_grb_dcz
<a name="cmxsrv_expcbe_grb_dcz"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_lee_dcz
<a name="cmxsrv_expcbe_lee_dcz"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_bus_vto
<a name="cmxsrv_expcbe_bus_vto"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_avi_dat_cou
<a name="cmxsrv_avi_dat_cou"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_avigrl_crea_avitemp](#referencia-cmxsrv_avigrl_crea_avitemp)
- [bcicomex](#referencia-bcicomex)

---

## CMXsrv_expcbe_avs_rem1
<a name="cmxsrv_expcbe_avs_rem1"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_trae_glo_fec](#referencia-cmxsrv_trae_glo_fec)
- [CMXsrv_expcbe_val_cbe](#referencia-cmxsrv_expcbe_val_cbe)
- [CMXsrv_util_fmt_txt](#referencia-cmxsrv_util_fmt_txt)

---

## CMXsrv_expcbe_avs_rem3
<a name="cmxsrv_expcbe_avs_rem3"></a>

**Procedimientos Referenciados:**

- [CMXsrv_util_fmt_txt](#referencia-cmxsrv_util_fmt_txt)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_avs_rem2
<a name="cmxsrv_expcbe_avs_rem2"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_expcbe_for_lin](#referencia-cmxsrv_expcbe_for_lin)

---

## CMXsrv_expcbe_avs_rem4
<a name="cmxsrv_expcbe_avs_rem4"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_busc_plz
<a name="cmxsrv_busc_plz"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_lee_plz
<a name="cmxsrv_lee_plz"></a>

**Procedimientos Referenciados:**

- [CMXsrv_mbyte_cmp](#referencia-cmxsrv_mbyte_cmp)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_cor_busc_pais
<a name="cmxsrv_cor_busc_pais"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_cor_lee_pais
<a name="cmxsrv_cor_lee_pais"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcbe_bus_cor
<a name="cmxsrv_expcbe_bus_cor"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_busc_bco_mtr
<a name="cmxsrv_busc_bco_mtr"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_grl_fec_serv
<a name="cmxsrv_grl_fec_serv"></a>

**Procedimientos Referenciados:**

- [SRV_MessageService](#referencia-srv_messageservice)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_lee_cce
<a name="cmxsrv_expcce_lee_cce"></a>

**Procedimientos Referenciados:**

- [por](#referencia-por)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_trd_cce
<a name="cmxsrv_expcce_trd_cce"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_anl_cce
<a name="cmxsrv_expcce_anl_cce"></a>

**Procedimientos Referenciados:**

- [CMXsrv_cmx_lee_trs](#referencia-cmxsrv_cmx_lee_trs)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_expcce_grb_evc](#referencia-cmxsrv_expcce_grb_evc)
- [CMXsrv_expcce_ictb_anu](#referencia-cmxsrv_expcce_ictb_anu)
- [CMXsrv_cnt_950](#referencia-cmxsrv_cnt_950)
- [CMXsrv_cnt_740](#referencia-cmxsrv_cnt_740)
- [CMXsrv_expcce_lee_fpro](#referencia-cmxsrv_expcce_lee_fpro)

---

## CMXsrv_expcce_ctb_ing
<a name="cmxsrv_expcce_ctb_ing"></a>

**Procedimientos Referenciados:**

- [CMXsrv_mbyte_gen](#referencia-cmxsrv_mbyte_gen)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_expcce_val_cce](#referencia-cmxsrv_expcce_val_cce)
- [CMXsrv_expcce_grb_evc](#referencia-cmxsrv_expcce_grb_evc)
- [CMXsrv_cnt_950](#referencia-cmxsrv_cnt_950)
- [CMXsrv_cnt_700](#referencia-cmxsrv_cnt_700)

---

## CMXsrv_expcce_del_cce
<a name="cmxsrv_expcce_del_cce"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_val_cce
<a name="cmxsrv_expcce_val_cce"></a>

**Procedimientos Referenciados:**

- [CMXsrv_cmx_get_codes](#referencia-cmxsrv_cmx_get_codes)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_swf_sel
<a name="cmxsrv_expcce_swf_sel"></a>

**Procedimientos Referenciados:**

- [CMXsrv_expcce_swf_730](#referencia-cmxsrv_expcce_swf_730)
- [CMXsrv_expcce_swf_742](#referencia-cmxsrv_expcce_swf_742)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_grb_bco
<a name="cmxsrv_expcce_grb_bco"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_expcce_lee_fpro](#referencia-cmxsrv_expcce_lee_fpro)

---

## CMXsrv_expcce_lee_cor
<a name="cmxsrv_expcce_lee_cor"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_lee_bco
<a name="cmxsrv_expcce_lee_bco"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_grb_ctp
<a name="cmxsrv_expcce_grb_ctp"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_expcce_lee_fpro](#referencia-cmxsrv_expcce_lee_fpro)

---

## CMXsrv_expcce_lee_cln
<a name="cmxsrv_expcce_lee_cln"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_lee_ctp
<a name="cmxsrv_expcce_lee_ctp"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_cre_cce
<a name="cmxsrv_expcce_cre_cce"></a>

**Procedimientos Referenciados:**

- [CMXsrv_util_num_ope](#referencia-cmxsrv_util_num_ope)
- [CMXsrv_cmx_busc_suc_usu](#referencia-cmxsrv_cmx_busc_suc_usu)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_expcce_lee_fpro](#referencia-cmxsrv_expcce_lee_fpro)

---

## CMXsrv_expcce_gen_dcc
<a name="cmxsrv_expcce_gen_dcc"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_grb_cnd
<a name="cmxsrv_expcce_grb_cnd"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_expcce_lee_fpro](#referencia-cmxsrv_expcce_lee_fpro)

---

## CMXsrv_util_det_habil
<a name="cmxsrv_util_det_habil"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_lee_cnd
<a name="cmxsrv_expcce_lee_cnd"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_trd_cnd
<a name="cmxsrv_expcce_trd_cnd"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_del_dcc
<a name="cmxsrv_expcce_del_dcc"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_expcce_lee_fpro](#referencia-cmxsrv_expcce_lee_fpro)

---

## CMXsrv_expcce_bus_dcc
<a name="cmxsrv_expcce_bus_dcc"></a>

**Procedimientos Referenciados:**

- [CMXsrv_expcce_gen_adcc](#referencia-cmxsrv_expcce_gen_adcc)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_grb_dcc
<a name="cmxsrv_expcce_grb_dcc"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_expcce_lee_fpro](#referencia-cmxsrv_expcce_lee_fpro)

---

## CMXsrv_expcce_lee_dcc
<a name="cmxsrv_expcce_lee_dcc"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_bus_cce
<a name="cmxsrv_expcce_bus_cce"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_mdf_cce
<a name="cmxsrv_expcce_mdf_cce"></a>

**Procedimientos Referenciados:**

- [CMXsrv_expcce_can_mdf](#referencia-cmxsrv_expcce_can_mdf)
- [CMXsrv_expcce_get_tip_ope](#referencia-cmxsrv_expcce_get_tip_ope)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_expcce_grb_evc](#referencia-cmxsrv_expcce_grb_evc)
- [CMXsrv_cnt_950](#referencia-cmxsrv_cnt_950)
- [CMXsrv_cmx_get_codes](#referencia-cmxsrv_cmx_get_codes)
- [CMXsrv_expcce_ctb_mdfcce](#referencia-cmxsrv_expcce_ctb_mdfcce)
- [CMXsrv_expcce_lee_fpro](#referencia-cmxsrv_expcce_lee_fpro)
- [CMXsrv_cnt_720](#referencia-cmxsrv_cnt_720)

---

## CMXsrv_expcce_can_mdf
<a name="cmxsrv_expcce_can_mdf"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_lee_mdf
<a name="cmxsrv_expcce_lee_mdf"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_cnf_cce
<a name="cmxsrv_expcce_cnf_cce"></a>

**Procedimientos Referenciados:**

- [CMXsrv_cnt_710](#referencia-cmxsrv_cnt_710)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_expcce_ictb_cexp](#referencia-cmxsrv_expcce_ictb_cexp)
- [CMXsrv_expcce_grb_evc](#referencia-cmxsrv_expcce_grb_evc)
- [CMXsrv_cnt_950](#referencia-cmxsrv_cnt_950)
- [CMXsrv_expcce_lee_fpro](#referencia-cmxsrv_expcce_lee_fpro)

---

## CMXsrv_expcce_grb_afin
<a name="cmxsrv_expcce_grb_afin"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_lee_cnf
<a name="cmxsrv_expcce_lee_cnf"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_expcce_lee_fpro](#referencia-cmxsrv_expcce_lee_fpro)

---

## CMXsrv_expcce_lee_afin
<a name="cmxsrv_expcce_lee_afin"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_trp_cce
<a name="cmxsrv_expcce_trp_cce"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_cnt_730](#referencia-cmxsrv_cnt_730)
- [CMXsrv_expcce_grb_evc](#referencia-cmxsrv_expcce_grb_evc)
- [CMXsrv_cnt_950](#referencia-cmxsrv_cnt_950)

---

## CMXsrv_expcce_lee_trp
<a name="cmxsrv_expcce_lee_trp"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_expcce_lee_fpro](#referencia-cmxsrv_expcce_lee_fpro)

---

## CMXsrv_expcce_bus_evc
<a name="cmxsrv_expcce_bus_evc"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_rev_cce
<a name="cmxsrv_expcce_rev_cce"></a>

**Procedimientos Referenciados:**

- [CMXsrv_expcce_rev_mdf](#referencia-cmxsrv_expcce_rev_mdf)
- [CMXsrv_expcce_ctb_alz](#referencia-cmxsrv_expcce_ctb_alz)
- [CMXsrv_expcce_rctb_anu](#referencia-cmxsrv_expcce_rctb_anu)
- [CMXsrv_cnt_751](#referencia-cmxsrv_cnt_751)
- [CMXsrv_cnt_761](#referencia-cmxsrv_cnt_761)
- [CMXsrv_expcce_rctb_oto](#referencia-cmxsrv_expcce_rctb_oto)
- [CMXsrv_cnt_1771](#referencia-cmxsrv_cnt_1771)
- [CMXsrv_cnt_720](#referencia-cmxsrv_cnt_720)
- [CMXsrv_expcce_ranu_neg](#referencia-cmxsrv_expcce_ranu_neg)
- [CMXsrv_mbyte_gen](#referencia-cmxsrv_mbyte_gen)
- [CMXsrv_expcce_chk_dsn](#referencia-cmxsrv_expcce_chk_dsn)
- [CMXsrv_ctl_chq_aprcbl](#referencia-cmxsrv_ctl_chq_aprcbl)
- [CMXsrv_rev_950](#referencia-cmxsrv_rev_950)
- [CMXsrv_cnt_771](#referencia-cmxsrv_cnt_771)
- [CMXsrv_expcce_eli_col](#referencia-cmxsrv_expcce_eli_col)
- [CMXsrv_expcce_grb_evc](#referencia-cmxsrv_expcce_grb_evc)
- [CMXsrv_cnt_731](#referencia-cmxsrv_cnt_731)
- [CMXsrv_expcce_get_tip_ope](#referencia-cmxsrv_expcce_get_tip_ope)
- [CMXsrv_expcce_rctb_oto_exp](#referencia-cmxsrv_expcce_rctb_oto_exp)
- [CMXsrv_cnt_711](#referencia-cmxsrv_cnt_711)
- [CMXsrv_cnt_rev_vig](#referencia-cmxsrv_cnt_rev_vig)
- [CMXsrv_cnt_701](#referencia-cmxsrv_cnt_701)
- [CMXsrv_cmx_lee_trs](#referencia-cmxsrv_cmx_lee_trs)
- [CMXsrv_cnt_999999](#referencia-cmxsrv_cnt_999999)
- [CMXsrv_expcce_lee_fpro](#referencia-cmxsrv_expcce_lee_fpro)
- [CMXsrv_cnt_741](#referencia-cmxsrv_cnt_741)
- [CMXsrv_expcce_eli_obl](#referencia-cmxsrv_expcce_eli_obl)
- [CMXsrv_expneg_rev_trp](#referencia-cmxsrv_expneg_rev_trp)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_cnt_781](#referencia-cmxsrv_cnt_781)
- [CMXsrv_expcce_ctb_mdfcce](#referencia-cmxsrv_expcce_ctb_mdfcce)
- [CMXsrv_expcce_gen_dsn](#referencia-cmxsrv_expcce_gen_dsn)
- [CMXsrv_expcce_rctb_pag_exp](#referencia-cmxsrv_expcce_rctb_pag_exp)

---

## CMXsrv_expcce_lee_evc
<a name="cmxsrv_expcce_lee_evc"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_avs_rem1
<a name="cmxsrv_expcce_avs_rem1"></a>

**Procedimientos Referenciados:**

- [CMXsrv_trae_glo_fec](#referencia-cmxsrv_trae_glo_fec)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_bus_cor
<a name="cmxsrv_expcce_bus_cor"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_dex_lee_dex
<a name="cmxsrv_dex_lee_dex"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_dex_eli_dex
<a name="cmxsrv_dex_eli_dex"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_dex_act_dex
<a name="cmxsrv_dex_act_dex"></a>

**Procedimientos Referenciados:**

- [CMXsrv_exppln_get_dig](#referencia-cmxsrv_exppln_get_dig)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)

---

## CMXsrv_expdex_cal_fec
<a name="cmxsrv_expdex_cal_fec"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_dex_lee_cli
<a name="cmxsrv_dex_lee_cli"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_dex_bus_dex
<a name="cmxsrv_dex_bus_dex"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_lee_bas
<a name="cmxsrv_expcce_lee_bas"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_lee_neg
<a name="cmxsrv_expcce_lee_neg"></a>

**Procedimientos Referenciados:**

- [CMXsrv_cmx_busc_suc_usu](#referencia-cmxsrv_cmx_busc_suc_usu)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_alz_dis
<a name="cmxsrv_expcce_alz_dis"></a>

**Procedimientos Referenciados:**

- [CMXsrv_expcce_ctb_alz](#referencia-cmxsrv_expcce_ctb_alz)
- [CMXsrv_cnt_760](#referencia-cmxsrv_cnt_760)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_expcce_grb_evc](#referencia-cmxsrv_expcce_grb_evc)
- [CMXsrv_cnt_950](#referencia-cmxsrv_cnt_950)
- [CMXsrv_expcce_get_tip_ope](#referencia-cmxsrv_expcce_get_tip_ope)
- [CMXsrv_expcce_lee_fpro](#referencia-cmxsrv_expcce_lee_fpro)

---

## CMXsrv_expcce_anl_neg
<a name="cmxsrv_expcce_anl_neg"></a>

**Procedimientos Referenciados:**

- [CMXsrv_cmx_lee_trs](#referencia-cmxsrv_cmx_lee_trs)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_cnt_780](#referencia-cmxsrv_cnt_780)
- [CMXsrv_expcce_grb_evc](#referencia-cmxsrv_expcce_grb_evc)
- [CMXsrv_expcce_ictb_anu](#referencia-cmxsrv_expcce_ictb_anu)
- [CMXsrv_cnt_950](#referencia-cmxsrv_cnt_950)
- [CMXsrv_expcce_lee_fpro](#referencia-cmxsrv_expcce_lee_fpro)

---

## CMXsrv_expcce_ctb_neg
<a name="cmxsrv_expcce_ctb_neg"></a>

**Procedimientos Referenciados:**

- [CMXsrv_expcce_val_neg](#referencia-cmxsrv_expcce_val_neg)
- [CMXsrv_mbyte_gen](#referencia-cmxsrv_mbyte_gen)
- [CMXsrv_expcce_ineg_cexp](#referencia-cmxsrv_expcce_ineg_cexp)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_expcce_anu_cexp](#referencia-cmxsrv_expcce_anu_cexp)
- [CMXsrv_expcce_grb_evc](#referencia-cmxsrv_expcce_grb_evc)
- [CMXsrv_cnt_950](#referencia-cmxsrv_cnt_950)
- [CMXsrv_expcce_lee_fpro](#referencia-cmxsrv_expcce_lee_fpro)
- [CMXsrv_cnt_750](#referencia-cmxsrv_cnt_750)

---

## CMXsrv_expcce_del_neg
<a name="cmxsrv_expcce_del_neg"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_val_neg
<a name="cmxsrv_expcce_val_neg"></a>

**Procedimientos Referenciados:**

- [CMXsrv_util_fecha](#referencia-cmxsrv_util_fecha)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_grb_neg
<a name="cmxsrv_expcce_grb_neg"></a>

**Procedimientos Referenciados:**

- [CMXsrv_cmx_busc_suc_usu](#referencia-cmxsrv_cmx_busc_suc_usu)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_expcce_lee_fpro](#referencia-cmxsrv_expcce_lee_fpro)

---

## CMXsrv_expcce_gen_dcn
<a name="cmxsrv_expcce_gen_dcn"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_avs_rem5
<a name="cmxsrv_expcce_avs_rem5"></a>

**Procedimientos Referenciados:**

- [CMX_srv_pone_punto](#referencia-cmx_srv_pone_punto)
- [CMXsrv_util_fmt_txt](#referencia-cmxsrv_util_fmt_txt)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_expcce_get_ing_esp](#referencia-cmxsrv_expcce_get_ing_esp)

---

## CMXsrv_expcce_lee_nge
<a name="cmxsrv_expcce_lee_nge"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_trd_nge
<a name="cmxsrv_expcce_trd_nge"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_ini_neg
<a name="cmxsrv_expcce_ini_neg"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_expcce_lee_fpro](#referencia-cmxsrv_expcce_lee_fpro)

---

## CMXsrv_expcce_del_dcn
<a name="cmxsrv_expcce_del_dcn"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_bus_dcn
<a name="cmxsrv_expcce_bus_dcn"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_grb_dcn
<a name="cmxsrv_expcce_grb_dcn"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_lee_dcn
<a name="cmxsrv_expcce_lee_dcn"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_del_ltr
<a name="cmxsrv_expcce_del_ltr"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_bus_ltr
<a name="cmxsrv_expcce_bus_ltr"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_grb_ltr
<a name="cmxsrv_expcce_grb_ltr"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_lee_ltr
<a name="cmxsrv_expcce_lee_ltr"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_del_dsn
<a name="cmxsrv_expcce_del_dsn"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_gen_dsn
<a name="cmxsrv_expcce_gen_dsn"></a>

**Procedimientos Referenciados:**

- [CMXsrv_expcce_grb_dsn](#referencia-cmxsrv_expcce_grb_dsn)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_bus_dsn
<a name="cmxsrv_expcce_bus_dsn"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_chk_dsn
<a name="cmxsrv_expcce_chk_dsn"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_grb_dsn
<a name="cmxsrv_expcce_grb_dsn"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_expcce_chk_dsn](#referencia-cmxsrv_expcce_chk_dsn)

---

## CMXsrv_expcce_lee_dsn
<a name="cmxsrv_expcce_lee_dsn"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_bus_neg
<a name="cmxsrv_expcce_bus_neg"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_pgo_neg
<a name="cmxsrv_expcce_pgo_neg"></a>

**Procedimientos Referenciados:**

- [CMXsrv_expret_grb_dtn](#referencia-cmxsrv_expret_grb_dtn)
- [CMXsrv_expcce_anu_cexp](#referencia-cmxsrv_expcce_anu_cexp)
- [CMXsrv_cnt_1770](#referencia-cmxsrv_cnt_1770)
- [CMXsrv_expret_grb_det](#referencia-cmxsrv_expret_grb_det)
- [CMXsrv_mbyte_gen](#referencia-cmxsrv_mbyte_gen)
- [CMXsrv_expret_grb_org](#referencia-cmxsrv_expret_grb_org)
- [CMXsrv_cnt_gen_vig](#referencia-cmxsrv_cnt_gen_vig)
- [CMXsrv_vig_gra_vig](#referencia-cmxsrv_vig_gra_vig)
- [CMXsrv_expcce_grb_evc](#referencia-cmxsrv_expcce_grb_evc)
- [CMXsrv_cmx_get_codes](#referencia-cmxsrv_cmx_get_codes)
- [CMXsrv_expret_cre_ret](#referencia-cmxsrv_expret_cre_ret)
- [CMXsrv_cnt_770](#referencia-cmxsrv_cnt_770)
- [CMXsrv_cnt_999999](#referencia-cmxsrv_cnt_999999)
- [CMXsrv_exp_ipuc_gen_pln](#referencia-cmxsrv_exp_ipuc_gen_pln)
- [CMXsrv_expcce_lee_fpro](#referencia-cmxsrv_expcce_lee_fpro)
- [CMXsrv_expneg_trp_cyg](#referencia-cmxsrv_expneg_trp_cyg)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_expcce_pag_exp](#referencia-cmxsrv_expcce_pag_exp)
- [CMXsrv_cnt_950](#referencia-cmxsrv_cnt_950)

---

## CMXsrv_expcce_lee_pgo
<a name="cmxsrv_expcce_lee_pgo"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_expcce_lee_fpro](#referencia-cmxsrv_expcce_lee_fpro)

---

## CMXsrv_expcce_avs_rem3
<a name="cmxsrv_expcce_avs_rem3"></a>

**Procedimientos Referenciados:**

- [CMXsrv_util_fmt_txt](#referencia-cmxsrv_util_fmt_txt)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_avs_rem2
<a name="cmxsrv_expcce_avs_rem2"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expcce_avs_rem4
<a name="cmxsrv_expcce_avs_rem4"></a>

**Procedimientos Referenciados:**

- [CMXsrv_util_fmt_txt](#referencia-cmxsrv_util_fmt_txt)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_swf_sel
<a name="cmxsrv_expret_swf_sel"></a>

**Procedimientos Referenciados:**

- [CMXsrv_expret_swf_202](#referencia-cmxsrv_expret_swf_202)
- [CMXsrv_expret_swf_100](#referencia-cmxsrv_expret_swf_100)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_lee_ret
<a name="cmxsrv_expret_lee_ret"></a>

**Procedimientos Referenciados:**

- [CMXsrv_cmx_busc_suc_usu](#referencia-cmxsrv_cmx_busc_suc_usu)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)

---

## CMXsrv_expret_lee_prm
<a name="cmxsrv_expret_lee_prm"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)

---

## CMXsrv_expret_avs_cyg1
<a name="cmxsrv_expret_avs_cyg1"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_avs_cyg2
<a name="cmxsrv_expret_avs_cyg2"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_avs_liq1
<a name="cmxsrv_expret_avs_liq1"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_avs_liq2
<a name="cmxsrv_expret_avs_liq2"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_avs_liq3
<a name="cmxsrv_expret_avs_liq3"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_val_ret
<a name="cmxsrv_expret_val_ret"></a>

**Procedimientos Referenciados:**

- [CMXsrv_val_cta_cte](#referencia-cmxsrv_val_cta_cte)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_enl_val_sel](#referencia-cmxsrv_enl_val_sel)
- [CMXsrv_val_vig](#referencia-cmxsrv_val_vig)
- [CMXsrv_util_len](#referencia-cmxsrv_util_len)
- [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)

---

## CMXsrv_expret_sum_dtn_mn
<a name="cmxsrv_expret_sum_dtn_mn"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_ctb_ing
<a name="cmxsrv_expret_ctb_ing"></a>

**Procedimientos Referenciados:**

- [CMXsrv_mbyte_gen](#referencia-cmxsrv_mbyte_gen)
- [CMXsrv_expret_grb_org](#referencia-cmxsrv_expret_grb_org)
- [CMXsrv_expret_grb_dtn](#referencia-cmxsrv_expret_grb_dtn)
- [CMXsrv_expret_cre_ret](#referencia-cmxsrv_expret_cre_ret)
- [CMXsrv_vig_gra_vig](#referencia-cmxsrv_vig_gra_vig)
- [CMXsrv_cnt_res_vig](#referencia-cmxsrv_cnt_res_vig)
- [CMXsrv_enl_act_enl](#referencia-cmxsrv_enl_act_enl)
- [sp_cmx_sii_1862](#referencia-sp_cmx_sii_1862)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_cnt_950](#referencia-cmxsrv_cnt_950)
- [sp_cmx_sii_1870](#referencia-sp_cmx_sii_1870)
- [CMXsrv_expret_val_ret](#referencia-cmxsrv_expret_val_ret)
- [CMXsrv_expret_grb_det](#referencia-cmxsrv_expret_grb_det)
- [CMXsrv_expret_cnt_cyg](#referencia-cmxsrv_expret_cnt_cyg)
- [CMXsrv_cnt_800](#referencia-cmxsrv_cnt_800)
- [CMXsrv_expret_grb_evr](#referencia-cmxsrv_expret_grb_evr)
- [CMXsrv_cnt_810](#referencia-cmxsrv_cnt_810)

---

## CMXsrv_expret_del_ret
<a name="cmxsrv_expret_del_ret"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_avs_adm1
<a name="cmxsrv_expret_avs_adm1"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_avs_adm2
<a name="cmxsrv_expret_avs_adm2"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_avs_adm3
<a name="cmxsrv_expret_avs_adm3"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_act_tpo_cbo
<a name="cmxsrv_expret_act_tpo_cbo"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_cre_ret
<a name="cmxsrv_expret_cre_ret"></a>

**Procedimientos Referenciados:**

- [CMXsrv_util_num_ope](#referencia-cmxsrv_util_num_ope)
- [CMXsrv_cmx_busc_suc_usu](#referencia-cmxsrv_cmx_busc_suc_usu)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)

---

## CMXsrv_expret_grb_det
<a name="cmxsrv_expret_grb_det"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_tpo_cbo
<a name="cmxsrv_expret_tpo_cbo"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)

---

## CMXsrv_expret_lee_cln
<a name="cmxsrv_expret_lee_cln"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_lee_det
<a name="cmxsrv_expret_lee_det"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)

---

## CMXsrv_expret_del_org
<a name="cmxsrv_expret_del_org"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_bus_org
<a name="cmxsrv_expret_bus_org"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_grb_org
<a name="cmxsrv_expret_grb_org"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_mto_org
<a name="cmxsrv_expret_mto_org"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_lee_org
<a name="cmxsrv_expret_lee_org"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_vig_lee_cta
<a name="cmxsrv_vig_lee_cta"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_del_dtn
<a name="cmxsrv_expret_del_dtn"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_bus_dtn
<a name="cmxsrv_expret_bus_dtn"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_grb_dtn
<a name="cmxsrv_expret_grb_dtn"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_cal_arb
<a name="cmxsrv_expret_cal_arb"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_mto_dtn
<a name="cmxsrv_expret_mto_dtn"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_lee_dtn
<a name="cmxsrv_expret_lee_dtn"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_bus_ret
<a name="cmxsrv_expret_bus_ret"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_bus_evr
<a name="cmxsrv_expret_bus_evr"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_expret_rev_ret
<a name="cmxsrv_expret_rev_ret"></a>

**Procedimientos Referenciados:**

- [CMXsrv_cnt_rev_vig](#referencia-cmxsrv_cnt_rev_vig)
- [CMXsrv_cnt_811](#referencia-cmxsrv_cnt_811)
- [CMXsrv_mbyte_gen](#referencia-cmxsrv_mbyte_gen)
- [CMXsrv_ctl_chq_aprcbl](#referencia-cmxsrv_ctl_chq_aprcbl)
- [CMXsrv_rev_950](#referencia-cmxsrv_rev_950)
- [sp_cmx_sii_1862](#referencia-sp_cmx_sii_1862)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_cnt_801](#referencia-cmxsrv_cnt_801)
- [sp_cmx_sii_1870](#referencia-sp_cmx_sii_1870)
- [CMXsrv_expret_rev_cyg](#referencia-cmxsrv_expret_rev_cyg)
- [CMXsrv_expret_grb_evr](#referencia-cmxsrv_expret_grb_evr)
- [CMXsrv_enl_rev_enl](#referencia-cmxsrv_enl_rev_enl)

---

## CMXsrv_expret_lee_evr
<a name="cmxsrv_expret_lee_evr"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finadm_imod_desti
<a name="cmxsrv_finadm_imod_desti"></a>

**Procedimientos Referenciados:**

- [CMXsrv_finadm_val_tipop](#referencia-cmxsrv_finadm_val_tipop)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finadm_cons_dtip
<a name="cmxsrv_finadm_cons_dtip"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finadm_imod_ectb
<a name="cmxsrv_finadm_imod_ectb"></a>

**Procedimientos Referenciados:**

- [CMXsrv_finadm_val_tipop](#referencia-cmxsrv_finadm_val_tipop)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finadm_eli_tipop
<a name="cmxsrv_finadm_eli_tipop"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finadm_cons_ectb
<a name="cmxsrv_finadm_cons_ectb"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finadm_imod_itip
<a name="cmxsrv_finadm_imod_itip"></a>

**Procedimientos Referenciados:**

- [CMXsrv_finadm_val_tipop](#referencia-cmxsrv_finadm_val_tipop)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finadm_cons_itip
<a name="cmxsrv_finadm_cons_itip"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finadm_lee_tipop
<a name="cmxsrv_finadm_lee_tipop"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finadm_val_tipop
<a name="cmxsrv_finadm_val_tipop"></a>

**Procedimientos Referenciados:**

- [CMXsrv_fincol_eval_tbat](#referencia-cmxsrv_fincol_eval_tbat)
- [CMXsrv_util_fecha2](#referencia-cmxsrv_util_fecha2)
- [SRV_MessageService](#referencia-srv_messageservice)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finadm_bus_tipope
<a name="cmxsrv_finadm_bus_tipope"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_busc_tip_tas
<a name="cmxsrv_busc_tip_tas"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_ecuo
<a name="cmxsrv_fincol_ecuo"></a>

**Procedimientos Referenciados:**

- [CMXsrv_fincol_pre_cuad_tas](#referencia-cmxsrv_fincol_pre_cuad_tas)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_cons_plnpa
<a name="cmxsrv_fincol_cons_plnpa"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_pertas_val_display
<a name="cmxsrv_pertas_val_display"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_eava
<a name="cmxsrv_fincol_eava"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_cons_aval
<a name="cmxsrv_fincol_cons_aval"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_iava
<a name="cmxsrv_fincol_iava"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_cons_pag
<a name="cmxsrv_fincol_cons_pag"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_trae_det_pag
<a name="cmxsrv_fincol_trae_det_pag"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_cons_pror
<a name="cmxsrv_fincol_cons_pror"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_cons_eve
<a name="cmxsrv_fincol_cons_eve"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_bco_swf
<a name="cmxsrv_icrd_lee_bco_swf"></a>

**Procedimientos Referenciados:**

- [CMXsrv_icrd_lee_cln](#referencia-cmxsrv_icrd_lee_cln)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_busc_bco
<a name="cmxsrv_icrd_busc_bco"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_vtocre_prov
<a name="cmxsrv_fincol_vtocre_prov"></a>

**Procedimientos Referenciados:**

- [CMXsrv_fincol_gpln](#referencia-cmxsrv_fincol_gpln)
- [CMXsrv_finobl_imod_obl](#referencia-cmxsrv_finobl_imod_obl)
- [CMXsrv_util_fecha](#referencia-cmxsrv_util_fecha)
- [CMXsrv_util_val_tasas](#referencia-cmxsrv_util_val_tasas)
- [CMXsrv_fincol_efec_calpa](#referencia-cmxsrv_fincol_efec_calpa)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_fincol_ctb_vcp](#referencia-cmxsrv_fincol_ctb_vcp)
- [sp_cmx_sii_1870](#referencia-sp_cmx_sii_1870)

---

## CMXsrv_fincol_prec_vtocre
<a name="cmxsrv_fincol_prec_vtocre"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_bus_lcr_bco
<a name="cmxsrv_icrd_bus_lcr_bco"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_lee_fpro
<a name="cmxsrv_lee_fpro"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_ren_fin
<a name="cmxsrv_fincol_ren_fin"></a>

**Procedimientos Referenciados:**

- [CMXsrv_cmx_fec_hoy](#referencia-cmxsrv_cmx_fec_hoy)
- [CMXsrv_fincol_pre_cuad_tas](#referencia-cmxsrv_fincol_pre_cuad_tas)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_fincol_grb_col_ren](#referencia-cmxsrv_fincol_grb_col_ren)
- [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)

---

## CMXsrv_fincol_gmod_ctr
<a name="cmxsrv_fincol_gmod_ctr"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_lee_bco
<a name="cmxsrv_fincol_lee_bco"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_lee_cln
<a name="cmxsrv_fincol_lee_cln"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_cons_ctr
<a name="cmxsrv_fincol_cons_ctr"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_ctb_oto
<a name="cmxsrv_fincol_ctb_oto"></a>

**Procedimientos Referenciados:**

- [CMXsrv_mbyte_gen](#referencia-cmxsrv_mbyte_gen)
- [CMXsrv_cmx_ing_lib](#referencia-cmxsrv_cmx_ing_lib)
- [CMXsrv_ctb_impto_tim](#referencia-cmxsrv_ctb_impto_tim)
- [CMXsrv_ctb_otorga](#referencia-cmxsrv_ctb_otorga)
- [CMXsrv_cnt_gen_vig](#referencia-cmxsrv_cnt_gen_vig)
- [CMXsrv_nibx_upd_tran](#referencia-cmxsrv_nibx_upd_tran)
- [CMXsrv_ctb_impto_tim2](#referencia-cmxsrv_ctb_impto_tim2)
- [CMXsrv_vig_gra_vig](#referencia-cmxsrv_vig_gra_vig)
- [CMXsrv_nibx_nilive](#referencia-cmxsrv_nibx_nilive)
- [CMXsrv_cyo_dsc](#referencia-cmxsrv_cyo_dsc)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_fincol_val_col](#referencia-cmxsrv_fincol_val_col)
- [CMXsrv_cnt_999999](#referencia-cmxsrv_cnt_999999)
- [sp_cmx_sii_1870](#referencia-sp_cmx_sii_1870)
- [CMXsrv_util_pesos](#referencia-cmxsrv_util_pesos)
- [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)

---

## CMXsrv_icrd_dat_liq_ope
<a name="cmxsrv_icrd_dat_liq_ope"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_lee_col
<a name="cmxsrv_fincol_lee_col"></a>

**Procedimientos Referenciados:**

- [PrmACMXESPECI](#referencia-prmacmxespeci)
- [PrmACLNEJECTA](#referencia-prmaclnejecta)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_busc_cod_ope
<a name="cmxsrv_busc_cod_ope"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_col_trae_num_ope
<a name="cmxsrv_col_trae_num_ope"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_eli_col
<a name="cmxsrv_fincol_eli_col"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_val_col
<a name="cmxsrv_fincol_val_col"></a>

**Procedimientos Referenciados:**

- [CMXsrv_fincol_val_err](#referencia-cmxsrv_fincol_val_err)
- [CMXsrv_fincol_val_per_tas](#referencia-cmxsrv_fincol_val_per_tas)
- [CMXsrv_fincol_val_adv](#referencia-cmxsrv_fincol_val_adv)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_bsc_col
<a name="cmxsrv_fincol_bsc_col"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_lee_tip
<a name="cmxsrv_fincol_lee_tip"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_ctb_novf
<a name="cmxsrv_fincol_ctb_novf"></a>

**Procedimientos Referenciados:**

- [CMXsrv_fincol_ctb_nov](#referencia-cmxsrv_fincol_ctb_nov)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)

---

## CMXsrv_fincol_cons_nov
<a name="cmxsrv_fincol_cons_nov"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_cmx_get_codes
<a name="cmxsrv_cmx_get_codes"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_grl_trae_cod_bco
<a name="cmxsrv_grl_trae_cod_bco"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_cons_tas
<a name="cmxsrv_fincol_cons_tas"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_efec_tras
<a name="cmxsrv_fincol_efec_tras"></a>

**Procedimientos Referenciados:**

- [CMXsrv_fincol_ctb_cnd](#referencia-cmxsrv_fincol_ctb_cnd)
- [CMXsrv_fincol_ctb_cob](#referencia-cmxsrv_fincol_ctb_cob)
- [CMXsrv_cnt_9000](#referencia-cmxsrv_cnt_9000)
- [CMXsrv_fincol_ctb_cst](#referencia-cmxsrv_fincol_ctb_cst)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_fincol_calc_cven](#referencia-cmxsrv_fincol_calc_cven)

---

## CMXsrv_fincol_cons_trasp
<a name="cmxsrv_fincol_cons_trasp"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_cons_dtrs
<a name="cmxsrv_fincol_cons_dtrs"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_cons_deve
<a name="cmxsrv_fincol_cons_deve"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_cont_gst
<a name="cmxsrv_fincol_cont_gst"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_cons_gst
<a name="cmxsrv_fincol_cons_gst"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_cons_dgst
<a name="cmxsrv_fincol_cons_dgst"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_bsc_tip
<a name="cmxsrv_fincol_bsc_tip"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_bus_cor
<a name="cmxsrv_finobl_bus_cor"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_ecuo
<a name="cmxsrv_finobl_ecuo"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_gpln
<a name="cmxsrv_finobl_gpln"></a>

**Procedimientos Referenciados:**

- [CMXsrv_util_det_habil_tasa](#referencia-cmxsrv_util_det_habil_tasa)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_cons_plnpa
<a name="cmxsrv_finobl_cons_plnpa"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_calc_anu
<a name="cmxsrv_finobl_calc_anu"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_finobl_efec_calpa](#referencia-cmxsrv_finobl_efec_calpa)
- [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)

---

## CMXsrv_finobl_lee_obl
<a name="cmxsrv_finobl_lee_obl"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_ctb_oto
<a name="cmxsrv_finobl_ctb_oto"></a>

**Procedimientos Referenciados:**

- [CMXsrv_ctbo_otorga](#referencia-cmxsrv_ctbo_otorga)
- [CMXsrv_finobl_val_obl](#referencia-cmxsrv_finobl_val_obl)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)

---

## CMXsrv_fincol_eli_obl
<a name="cmxsrv_fincol_eli_obl"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_val_obl
<a name="cmxsrv_finobl_val_obl"></a>

**Procedimientos Referenciados:**

- [CMXsrv_util_det_habil_tasa](#referencia-cmxsrv_util_det_habil_tasa)
- [CMXsrv_finobl_val_adv](#referencia-cmxsrv_finobl_val_adv)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_bsc_obl
<a name="cmxsrv_finobl_bsc_obl"></a>

**Procedimientos Referenciados:**

- [CMXsrv_finobl_bsc_obl2](#referencia-cmxsrv_finobl_bsc_obl2)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_finobl_bsc_obl3](#referencia-cmxsrv_finobl_bsc_obl3)

---

## CMXsrv_finobl_ictb_pag
<a name="cmxsrv_finobl_ictb_pag"></a>

**Procedimientos Referenciados:**

- [CMXsrv_finobl_ctb_pag](#referencia-cmxsrv_finobl_ctb_pag)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)

---

## CMXsrv_finobl_obt_sdocuo
<a name="cmxsrv_finobl_obt_sdocuo"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_new_tas
<a name="cmxsrv_finobl_new_tas"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_cons_pag
<a name="cmxsrv_finobl_cons_pag"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_cons_detp
<a name="cmxsrv_finobl_cons_detp"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_calc_pror
<a name="cmxsrv_finobl_calc_pror"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_finobl_efec_calpa](#referencia-cmxsrv_finobl_efec_calpa)
- [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)

---

## CMXsrv_finobl_cons_pror
<a name="cmxsrv_finobl_cons_pror"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_cons_dpror
<a name="cmxsrv_finobl_cons_dpror"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_ctb_anu
<a name="cmxsrv_finobl_ctb_anu"></a>

**Procedimientos Referenciados:**

- [CMXsrv_finobl_cbo_anu](#referencia-cmxsrv_finobl_cbo_anu)
- [CMXsrv_ctbo_anula](#referencia-cmxsrv_ctbo_anula)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)

---

## CMXsrv_finobl_cons_anu
<a name="cmxsrv_finobl_cons_anu"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_cons_mod
<a name="cmxsrv_finobl_cons_mod"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_cons_dmod
<a name="cmxsrv_finobl_cons_dmod"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_rev_eve
<a name="cmxsrv_finobl_rev_eve"></a>

**Procedimientos Referenciados:**

- [CMXsrv_ctl_marc_rev](#referencia-cmxsrv_ctl_marc_rev)
- [CMXsrv_ctl_chq_aprcbl](#referencia-cmxsrv_ctl_chq_aprcbl)
- [CMXsrv_finobl_rctb_pext](#referencia-cmxsrv_finobl_rctb_pext)
- [CMXsrv_rctb_cesi](#referencia-cmxsrv_rctb_cesi)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_finobl_rctb_pag](#referencia-cmxsrv_finobl_rctb_pag)
- [CMXsrv_finobl_rctb_pror](#referencia-cmxsrv_finobl_rctb_pror)
- [CMXsrv_finobl_rctb_mod](#referencia-cmxsrv_finobl_rctb_mod)
- [CMXsrv_finobl_rctb_anu](#referencia-cmxsrv_finobl_rctb_anu)
- [CMXsrv_finobl_rctb_oto](#referencia-cmxsrv_finobl_rctb_oto)

---

## CMXsrv_finobl_cons_eve
<a name="cmxsrv_finobl_cons_eve"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_cons_deve
<a name="cmxsrv_finobl_cons_deve"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_eli_ctr
<a name="cmxsrv_finobl_eli_ctr"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_cons_ctr
<a name="cmxsrv_finobl_cons_ctr"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_ing_ctr
<a name="cmxsrv_finobl_ing_ctr"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_cesion_obl
<a name="cmxsrv_finobl_cesion_obl"></a>

**Procedimientos Referenciados:**

- [CMXsrv_ctl_crea_apr](#referencia-cmxsrv_ctl_crea_apr)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)

---

## CMXsrv_comgrl_lee_nom_cor
<a name="cmxsrv_comgrl_lee_nom_cor"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_lee_cln
<a name="cmxsrv_lee_cln"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_busc_acre
<a name="cmxsrv_finobl_busc_acre"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_efec_calpa
<a name="cmxsrv_fincol_efec_calpa"></a>

**Procedimientos Referenciados:**

- [CMXsrv_fincol_eval_tnem](#referencia-cmxsrv_fincol_eval_tnem)
- [CMXsrv_fincol_eval_tmor](#referencia-cmxsrv_fincol_eval_tmor)
- [CMXsrv_util_det_habil](#referencia-cmxsrv_util_det_habil)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_fincol_calc_reba](#referencia-cmxsrv_fincol_calc_reba)
- [CMXsrv_fincol_eval_tasa](#referencia-cmxsrv_fincol_eval_tasa)
- [CMXsrv_fincol_eval_tneg](#referencia-cmxsrv_fincol_eval_tneg)
- [CMXsrv_fincol_efcal_cv](#referencia-cmxsrv_fincol_efcal_cv)
- [CMXsrv_fincol_cal_tas_sfr](#referencia-cmxsrv_fincol_cal_tas_sfr)

---

## CMXsrv_fincol_cons_detp
<a name="cmxsrv_fincol_cons_detp"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_calc_pror
<a name="cmxsrv_fincol_calc_pror"></a>

**Procedimientos Referenciados:**

- [CMXsrv_call_val_tas](#referencia-cmxsrv_call_val_tas)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_fincol_efec_calpa](#referencia-cmxsrv_fincol_efec_calpa)

---

## CMXsrv_fincol_cont_pror
<a name="cmxsrv_fincol_cont_pror"></a>

**Procedimientos Referenciados:**

- [CMXsrv_mbyte_gen](#referencia-cmxsrv_mbyte_gen)
- [CMXsrv_fincol_ctb_pror](#referencia-cmxsrv_fincol_ctb_pror)
- [CMXsrv_get_ult_dia_habil](#referencia-cmxsrv_get_ult_dia_habil)
- [CMXsrv_cmx_ing_lib](#referencia-cmxsrv_cmx_ing_lib)
- [CMXsrv_ctb_impto_tim](#referencia-cmxsrv_ctb_impto_tim)
- [CMXsrv_ipuc_gen_pln](#referencia-cmxsrv_ipuc_gen_pln)
- [CMXsrv_util_val_tasas](#referencia-cmxsrv_util_val_tasas)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_pertas_pror_tas](#referencia-cmxsrv_pertas_pror_tas)
- [CMXsrv_cmx_get_codes](#referencia-cmxsrv_cmx_get_codes)
- [CMXsrv_int_ccx_cns](#referencia-cmxsrv_int_ccx_cns)
- [CMXsrv_util_pesos](#referencia-cmxsrv_util_pesos)
- [CMXsrv_fincol_cam_new_tas](#referencia-cmxsrv_fincol_cam_new_tas)
- [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)

---

## CMXsrv_fincol_cons_dpror
<a name="cmxsrv_fincol_cons_dpror"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_cctb_anu
<a name="cmxsrv_fincol_cctb_anu"></a>

**Procedimientos Referenciados:**

- [CMXsrv_busc_cod_ope](#referencia-cmxsrv_busc_cod_ope)
- [CMXsrv_enl_act_enl](#referencia-cmxsrv_enl_act_enl)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_fincol_ctb_anu](#referencia-cmxsrv_fincol_ctb_anu)
- [sp_cmx_sii_1870](#referencia-sp_cmx_sii_1870)
- [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)

---

## CMXsrv_fincol_calc_anu
<a name="cmxsrv_fincol_calc_anu"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_fincol_efec_calpa](#referencia-cmxsrv_fincol_efec_calpa)

---

## CMXsrv_fincol_cons_anu
<a name="cmxsrv_fincol_cons_anu"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_cons_mod
<a name="cmxsrv_fincol_cons_mod"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_cons_dmod
<a name="cmxsrv_fincol_cons_dmod"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_cal_pext
<a name="cmxsrv_fincol_cal_pext"></a>

**Procedimientos Referenciados:**

- [CMXsrv_fincol_calc_reba](#referencia-cmxsrv_fincol_calc_reba)
- [CMXsrv_fincol_eval_tasa](#referencia-cmxsrv_fincol_eval_tasa)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_ctb_pext
<a name="cmxsrv_fincol_ctb_pext"></a>

**Procedimientos Referenciados:**

- [CMXsrv_ctb_pago](#referencia-cmxsrv_ctb_pago)
- [CMXsrv_util_gen_vig](#referencia-cmxsrv_util_gen_vig)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)

---

## CMXsrv_finobl_cal_pext
<a name="cmxsrv_finobl_cal_pext"></a>

**Procedimientos Referenciados:**

- [CMXsrv_finobl_eval_tasa](#referencia-cmxsrv_finobl_eval_tasa)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_fincol_cal_tas_sfr](#referencia-cmxsrv_fincol_cal_tas_sfr)

---

## CMXsrv_finobl_ctb_pext
<a name="cmxsrv_finobl_ctb_pext"></a>

**Procedimientos Referenciados:**

- [CMXsrv_ctbo_pago](#referencia-cmxsrv_ctbo_pago)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_lee_fpro](#referencia-cmxsrv_lee_fpro)

---

## CMXsrv_iarc_eli_arc
<a name="cmxsrv_iarc_eli_arc"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iarc_busc_arc
<a name="cmxsrv_iarc_busc_arc"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iinf_busc_inf
<a name="cmxsrv_iinf_busc_inf"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iarc_act_arc
<a name="cmxsrv_iarc_act_arc"></a>

**Procedimientos Referenciados:**

- [CMXsrv_cmx_get_codes](#referencia-cmxsrv_cmx_get_codes)
- [PrmACMXMONEDAFEC](#referencia-prmacmxmonedafec)
- [CMXsrv_util_opr_fec](#referencia-cmxsrv_util_opr_fec)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iarc_lee_arc
<a name="cmxsrv_iarc_lee_arc"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iinf_busc_opr
<a name="cmxsrv_iinf_busc_opr"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iinf_lee_vlr
<a name="cmxsrv_iinf_lee_vlr"></a>

**Procedimientos Referenciados:**

- [PrmACMXCLACOM](#referencia-prmacmxclacom)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iinf_rev_evi
<a name="cmxsrv_iinf_rev_evi"></a>

**Procedimientos Referenciados:**

- [CMXsrv_com_rev](#referencia-cmxsrv_com_rev)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icob_lee_pln
<a name="cmxsrv_icob_lee_pln"></a>

**Procedimientos Referenciados:**

- [CMXsrv_cmx_get_codes](#referencia-cmxsrv_cmx_get_codes)
- [CMXsrv_icob_obs_pln](#referencia-cmxsrv_icob_obs_pln)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icob_cur_cob
<a name="cmxsrv_icob_cur_cob"></a>

**Procedimientos Referenciados:**

- [CMXsrv_icob_ctb_reem](#referencia-cmxsrv_icob_ctb_reem)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_icob_val_cob](#referencia-cmxsrv_icob_val_cob)

---

## CMXsrv_icob_pag_sop
<a name="cmxsrv_icob_pag_sop"></a>

**Procedimientos Referenciados:**

- [CMXsrv_get_ult_dia_habil](#referencia-cmxsrv_get_ult_dia_habil)
- [CMXsrv_icob_refresh_pos](#referencia-cmxsrv_icob_refresh_pos)
- [CMXsrv_val_cta_cte](#referencia-cmxsrv_val_cta_cte)
- [CMXsrv_calc_imp_4pct](#referencia-cmxsrv_calc_imp_4pct)
- [CMXsrv_icbr_act_rem](#referencia-cmxsrv_icbr_act_rem)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_icob_ctb_sop](#referencia-cmxsrv_icob_ctb_sop)
- [CMXsrv_ctb_imp_ddi_so](#referencia-cmxsrv_ctb_imp_ddi_so)
- [CMXsrv_cmx_get_codes](#referencia-cmxsrv_cmx_get_codes)
- [CMXsrv_iddi_marc_ddi2](#referencia-cmxsrv_iddi_marc_ddi2)
- [CMXsrv_icob_val_cob](#referencia-cmxsrv_icob_val_cob)

---

## CMXsrv_icob_eli_pln
<a name="cmxsrv_icob_eli_pln"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icob_rev_etd
<a name="cmxsrv_icob_rev_etd"></a>

**Procedimientos Referenciados:**

- [CMXsrv_icob_refresh_pos](#referencia-cmxsrv_icob_refresh_pos)
- [CMXsrv_ctl_chq_aprcbl](#referencia-cmxsrv_ctl_chq_aprcbl)
- [CMXsrv_icob_ctb_anu](#referencia-cmxsrv_icob_ctb_anu)
- [CMXsrv_icob_ctb_reem](#referencia-cmxsrv_icob_ctb_reem)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_pos_eli_010](#referencia-cmxsrv_pos_eli_010)
- [CMXsrv_icob_rctb_sop](#referencia-cmxsrv_icob_rctb_sop)

---

## CMXsrv_icob_val_cob
<a name="cmxsrv_icob_val_cob"></a>

**Procedimientos Referenciados:**

- [PrmACMXPAIS](#referencia-prmacmxpais)
- [CMXsrv_pos_bcx_lee_cob](#referencia-cmxsrv_pos_bcx_lee_cob)
- [CMXsrv_util_fecha](#referencia-cmxsrv_util_fecha)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icob_busc_pln
<a name="cmxsrv_icob_busc_pln"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icob_lee_cln
<a name="cmxsrv_icob_lee_cln"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icob_crea_norm
<a name="cmxsrv_icob_crea_norm"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_icob_get_num](#referencia-cmxsrv_icob_get_num)

---

## CMXsrv_icob_crea_reem
<a name="cmxsrv_icob_crea_reem"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_icob_get_num](#referencia-cmxsrv_icob_get_num)
- [CMXsrv_cmx_get_codes](#referencia-cmxsrv_cmx_get_codes)
- [CMXsrv_pos_bcx_lee_cob](#referencia-cmxsrv_pos_bcx_lee_cob)
- [CMXsrv_pos_bcx_ing_cob](#referencia-cmxsrv_pos_bcx_ing_cob)

---

## CMXsrv_icob_act_gral
<a name="cmxsrv_icob_act_gral"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_icob_num_con](#referencia-cmxsrv_icob_num_con)
- [CMXsrv_icob_val_cob](#referencia-cmxsrv_icob_val_cob)
- [CMXsrv_pos_bcx_act_cob](#referencia-cmxsrv_pos_bcx_act_cob)

---

## CMXsrv_icob_lee_cln2
<a name="cmxsrv_icob_lee_cln2"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icob_lee_gral
<a name="cmxsrv_icob_lee_gral"></a>

**Procedimientos Referenciados:**

- [CMXsrv_pos_bcx_lee_cob](#referencia-cmxsrv_pos_bcx_lee_cob)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icob_act_val
<a name="cmxsrv_icob_act_val"></a>

**Procedimientos Referenciados:**

- [CMXsrv_get_ult_dia_habil](#referencia-cmxsrv_get_ult_dia_habil)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_icob_val_cob](#referencia-cmxsrv_icob_val_cob)

---

## CMXsrv_icob_lee_val
<a name="cmxsrv_icob_lee_val"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icob_act_acu
<a name="cmxsrv_icob_act_acu"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_icob_val_cob](#referencia-cmxsrv_icob_val_cob)

---

## CMXsrv_icob_lee_acu
<a name="cmxsrv_icob_lee_acu"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icob_eli_int
<a name="cmxsrv_icob_eli_int"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icob_busc_int
<a name="cmxsrv_icob_busc_int"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icob_ingmod_int
<a name="cmxsrv_icob_ingmod_int"></a>

**Procedimientos Referenciados:**

- [PrmACMXMONEDA](#referencia-prmacmxmoneda)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_icob_val_cob](#referencia-cmxsrv_icob_val_cob)

---

## CMXsrv_icob_lee_int
<a name="cmxsrv_icob_lee_int"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icob_ing_mod_srf
<a name="cmxsrv_icob_ing_mod_srf"></a>

**Procedimientos Referenciados:**

- [CMXsrv_pos_bcx_ing_cob](#referencia-cmxsrv_pos_bcx_ing_cob)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_icob_get_num](#referencia-cmxsrv_icob_get_num)
- [CMXsrv_pos_bcx_act_cob](#referencia-cmxsrv_pos_bcx_act_cob)

---

## CMXsrv_icob_anu
<a name="cmxsrv_icob_anu"></a>

**Procedimientos Referenciados:**

- [CMXsrv_get_ult_dia_habil](#referencia-cmxsrv_get_ult_dia_habil)
- [CMXsrv_icob_refresh_pos](#referencia-cmxsrv_icob_refresh_pos)
- [CMXsrv_icob_ctb_anu](#referencia-cmxsrv_icob_ctb_anu)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_pos_bcx_act_cob](#referencia-cmxsrv_pos_bcx_act_cob)
- [CMXsrv_icob_get_num](#referencia-cmxsrv_icob_get_num)
- [CMXsrv_cmx_get_codes](#referencia-cmxsrv_cmx_get_codes)
- [CMXsrv_pos_bcx_lee_cob](#referencia-cmxsrv_pos_bcx_lee_cob)
- [CMXsrv_pos_bcx_ing_cob](#referencia-cmxsrv_pos_bcx_ing_cob)

---

## CMXsrv_icob_lee_anu
<a name="cmxsrv_icob_lee_anu"></a>

**Procedimientos Referenciados:**

- [CMXsrv_pos_bcx_lee_cob](#referencia-cmxsrv_pos_bcx_lee_cob)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icob_cur_reem
<a name="cmxsrv_icob_cur_reem"></a>

**Procedimientos Referenciados:**

- [CMXsrv_icob_ctb_reem](#referencia-cmxsrv_icob_ctb_reem)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_icob_refresh_pos](#referencia-cmxsrv_icob_refresh_pos)
- [CMXsrv_icob_val_cob](#referencia-cmxsrv_icob_val_cob)

---

## CMXsrv_busc_cor_swf
<a name="cmxsrv_busc_cor_swf"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_swf_bus_sms
<a name="cmxsrv_swf_bus_sms"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_lee_cbr
<a name="cmxsrv_icbr_lee_cbr"></a>

**Procedimientos Referenciados:**

- [PrmACMXESPECI](#referencia-prmacmxespeci)
- [PrmACLNEJECTA](#referencia-prmaclnejecta)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_acep_let
<a name="cmxsrv_icbr_acep_let"></a>

**Procedimientos Referenciados:**

- [CMXsrv_ctl_crea_apr](#referencia-cmxsrv_ctl_crea_apr)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_cont_cbr
<a name="cmxsrv_icbr_cont_cbr"></a>

**Procedimientos Referenciados:**

- [CMXsrv_ctl_marc_firma](#referencia-cmxsrv_ctl_marc_firma)
- [CMXsrv_mbyte_gen](#referencia-cmxsrv_mbyte_gen)
- [CMXsrv_icbr_val_cbr](#referencia-cmxsrv_icbr_val_cbr)
- [CMXsrv_nibx_upd_tran](#referencia-cmxsrv_nibx_upd_tran)
- [CMXsrv_cnt_gen_vig](#referencia-cmxsrv_cnt_gen_vig)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_ctb_cbr](#referencia-cmxsrv_ctb_cbr)
- [CMXsrv_nibx_nilive](#referencia-cmxsrv_nibx_nilive)

---

## CMXsrv_icbr_eli_cbr
<a name="cmxsrv_icbr_eli_cbr"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_lee_ctp
<a name="cmxsrv_icbr_lee_ctp"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_avi1
<a name="cmxsrv_icbr_avi1"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_busc_cbr
<a name="cmxsrv_icbr_busc_cbr"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_lee_cln
<a name="cmxsrv_icbr_lee_cln"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_crea_cbr
<a name="cmxsrv_icbr_crea_cbr"></a>

**Procedimientos Referenciados:**

- [srv_icbr_asig_num](#referencia-srv_icbr_asig_num)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_util_num_ope](#referencia-cmxsrv_util_num_ope)

---

## CMXsrv_icbr_lee_cob
<a name="cmxsrv_icbr_lee_cob"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_act_ctp
<a name="cmxsrv_icbr_act_ctp"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_lee_trm
<a name="cmxsrv_icbr_lee_trm"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_act_trm
<a name="cmxsrv_icbr_act_trm"></a>

**Procedimientos Referenciados:**

- [CMXsrv_util_fecha](#referencia-cmxsrv_util_fecha)
- [CMXsrv_icbr_val_cbr](#referencia-cmxsrv_icbr_val_cbr)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_lee_doc
<a name="cmxsrv_icbr_lee_doc"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_act_doc
<a name="cmxsrv_icbr_act_doc"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_busc_let
<a name="cmxsrv_icbr_busc_let"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_ingmod_let
<a name="cmxsrv_icbr_ingmod_let"></a>

**Procedimientos Referenciados:**

- [CMXsrv_util_fecha](#referencia-cmxsrv_util_fecha)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_eli_let
<a name="cmxsrv_icbr_eli_let"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_lee_let
<a name="cmxsrv_icbr_lee_let"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_prorr
<a name="cmxsrv_icbr_prorr"></a>

**Procedimientos Referenciados:**

- [CMXsrv_util_fecha](#referencia-cmxsrv_util_fecha)
- [CMXsrv_cnt_2600](#referencia-cmxsrv_cnt_2600)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_cnt_2610](#referencia-cmxsrv_cnt_2610)
- [CMXsrv_cnt_2620](#referencia-cmxsrv_cnt_2620)

---

## CMXsrv_icbr_rev_eve
<a name="cmxsrv_icbr_rev_eve"></a>

**Procedimientos Referenciados:**

- [CMXsrv_icbr_rev_mod_cbr](#referencia-cmxsrv_icbr_rev_mod_cbr)
- [CMXsrv_mbyte_gen](#referencia-cmxsrv_mbyte_gen)
- [CMXsrv_ctl_marc_rev](#referencia-cmxsrv_ctl_marc_rev)
- [CMXsrv_ctl_chq_aprcbl](#referencia-cmxsrv_ctl_chq_aprcbl)
- [CMXsrv_icbr_rev_prot](#referencia-cmxsrv_icbr_rev_prot)
- [CMXsrv_icbr_rev_ent](#referencia-cmxsrv_icbr_rev_ent)
- [CMXsrv_ctl_eli_firma](#referencia-cmxsrv_ctl_eli_firma)
- [CMXsrv_icbr_rev_trfo](#referencia-cmxsrv_icbr_rev_trfo)
- [CMXsrv_icbr_rev_vis](#referencia-cmxsrv_icbr_rev_vis)
- [CMXsrv_cnt_rev_vig](#referencia-cmxsrv_cnt_rev_vig)
- [CMXsrv_icbr_rev_acep](#referencia-cmxsrv_icbr_rev_acep)
- [CMXsrv_icbr_rev_inst](#referencia-cmxsrv_icbr_rev_inst)
- [CMXsrv_icbr_rev_trfb](#referencia-cmxsrv_icbr_rev_trfb)
- [CMXsrv_rctb_rem](#referencia-cmxsrv_rctb_rem)
- [CMXsrv_icbr_rev_ing](#referencia-cmxsrv_icbr_rev_ing)
- [CMXsrv_icbr_rev_prorr](#referencia-cmxsrv_icbr_rev_prorr)
- [CMXsrv_icbr_rev_liq](#referencia-cmxsrv_icbr_rev_liq)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_com_rev](#referencia-cmxsrv_com_rev)
- [CMXsrv_icbr_rev_pag](#referencia-cmxsrv_icbr_rev_pag)
- [sp_cmx_sii_1870](#referencia-sp_cmx_sii_1870)

---

## CMXsrv_icbr_busc_eve
<a name="cmxsrv_icbr_busc_eve"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_lee_eve
<a name="cmxsrv_icbr_lee_eve"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_lee_ent_doc
<a name="cmxsrv_icbr_lee_ent_doc"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_prot
<a name="cmxsrv_icbr_prot"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_ctl_crea_apr](#referencia-cmxsrv_ctl_crea_apr)
- [CMXsrv_cnt_950](#referencia-cmxsrv_cnt_950)

---

## CMXsrv_icbr_pcg_prot
<a name="cmxsrv_icbr_pcg_prot"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_liq_sdo
<a name="cmxsrv_icbr_liq_sdo"></a>

**Procedimientos Referenciados:**

- [CMXsrv_ctb_liq_sdo](#referencia-cmxsrv_ctb_liq_sdo)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_cnt_gen_vig](#referencia-cmxsrv_cnt_gen_vig)

---

## CMXsrv_icbr_act_vis
<a name="cmxsrv_icbr_act_vis"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_eli_rep
<a name="cmxsrv_icbr_eli_rep"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_busc_rep
<a name="cmxsrv_icbr_busc_rep"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_imod_rep
<a name="cmxsrv_icbr_imod_rep"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_ent_doc
<a name="cmxsrv_icbr_ent_doc"></a>

**Procedimientos Referenciados:**

- [CMXsrv_ctl_crea_apr](#referencia-cmxsrv_ctl_crea_apr)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_trf_ofi
<a name="cmxsrv_icbr_trf_ofi"></a>

**Procedimientos Referenciados:**

- [CMXsrv_ctb_trfo](#referencia-cmxsrv_ctb_trfo)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_trf_bco
<a name="cmxsrv_icbr_trf_bco"></a>

**Procedimientos Referenciados:**

- [CMXsrv_ctb_trfb](#referencia-cmxsrv_ctb_trfb)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_act_inst
<a name="cmxsrv_icbr_act_inst"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iswf_a_pru
<a name="cmxsrv_iswf_a_pru"></a>

**Procedimientos Referenciados:**

- [CMXsrv_iswf_a_732](#referencia-cmxsrv_iswf_a_732)
- [CMXsrv_iswf_esp_707b](#referencia-cmxsrv_iswf_esp_707b)
- [CMXsrv_iswf_a_747](#referencia-cmxsrv_iswf_a_747)
- [CMXsrv_iswf_a_412](#referencia-cmxsrv_iswf_a_412)
- [CMXsrv_iswf_a_707b](#referencia-cmxsrv_iswf_a_707b)
- [CMXsrv_iswf_esp_740](#referencia-cmxsrv_iswf_esp_740)
- [CMXsrv_iswf_a_410](#referencia-cmxsrv_iswf_a_410)
- [CMXsrv_iswf_esp_747](#referencia-cmxsrv_iswf_esp_747)
- [CMXsrv_iswf_neg_730](#referencia-cmxsrv_iswf_neg_730)
- [CMXsrv_iswf_neg_752](#referencia-cmxsrv_iswf_neg_752)
- [CMXsrv_iswf_a_700a](#referencia-cmxsrv_iswf_a_700a)
- [CMXsrv_iswf_a_707a](#referencia-cmxsrv_iswf_a_707a)
- [CMXsrv_iswf_esp_700b](#referencia-cmxsrv_iswf_esp_700b)
- [CMXsrv_iswf_a_740](#referencia-cmxsrv_iswf_a_740)
- [CMXsrv_iswf_a_700b](#referencia-cmxsrv_iswf_a_700b)
- [CMXsrv_iswf_esp_707a](#referencia-cmxsrv_iswf_esp_707a)
- [srv_irem_imp_202](#referencia-srv_irem_imp_202)
- [CMXsrv_iswf_747_neg](#referencia-cmxsrv_iswf_747_neg)
- [srv_irem_imp_100](#referencia-srv_irem_imp_100)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_iswf_esp_700a](#referencia-cmxsrv_iswf_esp_700a)

---

## CMXsrv_icbr_val_cbr
<a name="cmxsrv_icbr_val_cbr"></a>

**Procedimientos Referenciados:**

- [PrmACMXPAIS](#referencia-prmacmxpais)
- [CMXsrv_icbr_val_arc](#referencia-cmxsrv_icbr_val_arc)
- [CMXsrv_util_fecha](#referencia-cmxsrv_util_fecha)
- [sp_procxmode](#referencia-sp_procxmode)
- [PrmACMXMONEDAFEC](#referencia-prmacmxmonedafec)

---

## CMXsrv_icrd_a_ibab
<a name="cmxsrv_icrd_a_ibab"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_glo_ibab
<a name="cmxsrv_icrd_lee_glo_ibab"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_icrd_pre_78](#referencia-cmxsrv_icrd_pre_78)

---

## CMXsrv_icrd_a_ibar
<a name="cmxsrv_icrd_a_ibar"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_glo_ibar
<a name="cmxsrv_icrd_lee_glo_ibar"></a>

**Procedimientos Referenciados:**

- [CMXsrv_icrd_pre_72_740](#referencia-cmxsrv_icrd_pre_72_740)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_tex_swf
<a name="cmxsrv_icrd_lee_tex_swf"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_cod_txt_swf
<a name="cmxsrv_icrd_lee_cod_txt_swf"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_txt_swf_all
<a name="cmxsrv_icrd_lee_txt_swf_all"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_ind_esp_ing
<a name="cmxsrv_icrd_lee_ind_esp_ing"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_ing_acu
<a name="cmxsrv_icrd_ing_acu"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_acu
<a name="cmxsrv_icrd_lee_acu"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_rech_sol
<a name="cmxsrv_icrd_rech_sol"></a>

**Procedimientos Referenciados:**

- [CMXsrv_nibx_upd_tran](#referencia-cmxsrv_nibx_upd_tran)
- [CMXsrv_ctl_crea_apr](#referencia-cmxsrv_ctl_crea_apr)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_nibx_nilive](#referencia-cmxsrv_nibx_nilive)

---

## CMXsrv_icrd_end
<a name="cmxsrv_icrd_end"></a>

**Procedimientos Referenciados:**

- [CMXsrv_ctl_crea_apr](#referencia-cmxsrv_ctl_crea_apr)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_dat_end
<a name="cmxsrv_icrd_lee_dat_end"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_asignar_cor
<a name="cmxsrv_icrd_asignar_cor"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_bco_mtr
<a name="cmxsrv_icrd_lee_bco_mtr"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_cor_lee_pais
<a name="cmxsrv_icrd_cor_lee_pais"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_plz
<a name="cmxsrv_icrd_lee_plz"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_busc_plz
<a name="cmxsrv_icrd_busc_plz"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_cor_busc_pais
<a name="cmxsrv_icrd_cor_busc_pais"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_busc_bco_mtr
<a name="cmxsrv_icrd_busc_bco_mtr"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iddi_ingmod_ddi
<a name="cmxsrv_iddi_ingmod_ddi"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iddi_lee_dec
<a name="cmxsrv_iddi_lee_dec"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_iddi_val_num_ddi](#referencia-cmxsrv_iddi_val_num_ddi)

---

## CMXsrv_iddi_eli_ddi
<a name="cmxsrv_iddi_eli_ddi"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iddi_lee_inf
<a name="cmxsrv_iddi_lee_inf"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iddi_lee_cln
<a name="cmxsrv_iddi_lee_cln"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iddi_lee_rut
<a name="cmxsrv_iddi_lee_rut"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iddi_asoc_ddi
<a name="cmxsrv_iddi_asoc_ddi"></a>

**Procedimientos Referenciados:**

- [CMXsrv_cmx_get_codes](#referencia-cmxsrv_cmx_get_codes)
- [CMXsrv_get_ult_dia_habil](#referencia-cmxsrv_get_ult_dia_habil)
- [CMXsrv_util_opr_fec](#referencia-cmxsrv_util_opr_fec)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iddi_des_ddi
<a name="cmxsrv_iddi_des_ddi"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iddi_busc_asoc
<a name="cmxsrv_iddi_busc_asoc"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iddi_busc_noasoc
<a name="cmxsrv_iddi_busc_noasoc"></a>

**Procedimientos Referenciados:**

- [CMXsrv_iddi_bus_noasoc_cob](#referencia-cmxsrv_iddi_bus_noasoc_cob)
- [CMXsrv_iddi_bus_noasoc_opr](#referencia-cmxsrv_iddi_bus_noasoc_opr)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_dir_cln
<a name="cmxsrv_icrd_lee_dir_cln"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXCRDsrv_icrd_a_cnd_esp
<a name="cmxcrdsrv_icrd_a_cnd_esp"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_cnd_esp
<a name="cmxsrv_icrd_lee_cnd_esp"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_icrd_pre_47](#referencia-cmxsrv_icrd_pre_47)

---

## CMXCRDsrv_icrd_clon_crd
<a name="cmxcrdsrv_icrd_clon_crd"></a>

**Procedimientos Referenciados:**

- [CMXCRDsrv_icrd_lee_tas_cln](#referencia-cmxcrdsrv_icrd_lee_tas_cln)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_fincol_ing_modcol](#referencia-cmxsrv_fincol_ing_modcol)
- [CMXsrv_util_num_ope](#referencia-cmxsrv_util_num_ope)

---

## CMXCRDsrv_icrd_lee_crdcre
<a name="cmxcrdsrv_icrd_lee_crdcre"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_top
<a name="cmxsrv_icrd_lee_top"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXCRDsrv_icrd_val_crd
<a name="cmxcrdsrv_icrd_val_crd"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_icrd_val_adv](#referencia-cmxsrv_icrd_val_adv)
- [CMXsrv_icrd_val_err](#referencia-cmxsrv_icrd_val_err)

---

## CMXCRDsrv_icrd_eli_crd
<a name="cmxcrdsrv_icrd_eli_crd"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_dat_trs
<a name="cmxsrv_icrd_lee_dat_trs"></a>

**Procedimientos Referenciados:**

- [CMXsrv_icrd_forlin](#referencia-cmxsrv_icrd_forlin)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_a_ctp
<a name="cmxsrv_icrd_a_ctp"></a>

**Procedimientos Referenciados:**

- [CMXCRDsrv_icrd_lee_tas_cln](#referencia-cmxcrdsrv_icrd_lee_tas_cln)
- [CMXsrv_fincol_imod_colcc](#referencia-cmxsrv_fincol_imod_colcc)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_cln
<a name="cmxsrv_icrd_lee_cln"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_a_cnd
<a name="cmxsrv_icrd_a_cnd"></a>

**Procedimientos Referenciados:**

- [CMXMCRDsrv_icrd_lee_mapr](#referencia-cmxmcrdsrv_icrd_lee_mapr)
- [CMXsrv_ctb_impto_tim](#referencia-cmxsrv_ctb_impto_tim)
- [CMXsrv_icrd_a_dat_apr](#referencia-cmxsrv_icrd_a_dat_apr)
- [CMXsrv_imp_calc_aladi](#referencia-cmxsrv_imp_calc_aladi)
- [CMXsrv_ctb_impto_tim2](#referencia-cmxsrv_ctb_impto_tim2)
- [CMXsrv_busc_cod_ope](#referencia-cmxsrv_busc_cod_ope)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_ctb_impto_tim3](#referencia-cmxsrv_ctb_impto_tim3)
- [CMXsrv_icrd_act_pag_mix](#referencia-cmxsrv_icrd_act_pag_mix)
- [CMXsrv_util_pesos](#referencia-cmxsrv_util_pesos)

---

## CMXCRDsrv_icrd_crea_crd
<a name="cmxcrdsrv_icrd_crea_crd"></a>

**Procedimientos Referenciados:**

- [CMXsrv_imp_calc_aladi](#referencia-cmxsrv_imp_calc_aladi)
- [CMXsrv_fincol_imod_colcc](#referencia-cmxsrv_fincol_imod_colcc)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXCRDsrv_icrd_lee_tas_cln](#referencia-cmxcrdsrv_icrd_lee_tas_cln)
- [CMXsrv_util_num_ope](#referencia-cmxsrv_util_num_ope)
- [CMXsrv_fincol_ing_modcol](#referencia-cmxsrv_fincol_ing_modcol)

---

## CMXsrv_icrd_busc_emb
<a name="cmxsrv_icrd_busc_emb"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_eli_emb
<a name="cmxsrv_icrd_eli_emb"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_emb1
<a name="cmxsrv_icrd_lee_emb1"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_emb2
<a name="cmxsrv_icrd_lee_emb2"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_a_emb1
<a name="cmxsrv_icrd_a_emb1"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_a_emb2
<a name="cmxsrv_icrd_a_emb2"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_val_emb2
<a name="cmxsrv_icrd_val_emb2"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_val_emb1
<a name="cmxsrv_icrd_val_emb1"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_act_ref
<a name="cmxsrv_icrd_act_ref"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_ref
<a name="cmxsrv_icrd_lee_ref"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXCRDsrv_icrd_apr_sol
<a name="cmxcrdsrv_icrd_apr_sol"></a>

**Procedimientos Referenciados:**

- [CMXsrv_mbyte_gen](#referencia-cmxsrv_mbyte_gen)
- [CMXsrv_icrd_asignar_cor](#referencia-cmxsrv_icrd_asignar_cor)
- [CMXsrv_ctb_impto_tim](#referencia-cmxsrv_ctb_impto_tim)
- [CMXsrv_cmx_ing_lib](#referencia-cmxsrv_cmx_ing_lib)
- [CMXsrv_nibx_upd_tran](#referencia-cmxsrv_nibx_upd_tran)
- [CMXsrv_ctb_impto_tim2](#referencia-cmxsrv_ctb_impto_tim2)
- [CMXsrv_lee_paridad](#referencia-cmxsrv_lee_paridad)
- [CMXsrv_iswf_a_700](#referencia-cmxsrv_iswf_a_700)
- [CMXsrv_fincol_imod_colcc](#referencia-cmxsrv_fincol_imod_colcc)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_ctb_impto_tim22](#referencia-cmxsrv_ctb_impto_tim22)
- [CMXsrv_ctb_impto_tim3](#referencia-cmxsrv_ctb_impto_tim3)
- [CMXsrv_icrd_val_crd](#referencia-cmxsrv_icrd_val_crd)
- [CMXsrv_util_pesos](#referencia-cmxsrv_util_pesos)
- [CMXsrv_nibx_nilive](#referencia-cmxsrv_nibx_nilive)

---

## CMXsrv_icrd_lee_crdapr
<a name="cmxsrv_icrd_lee_crdapr"></a>

**Procedimientos Referenciados:**

- [CMXsrv_icrd_pre_72](#referencia-cmxsrv_icrd_pre_72)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXCRDsrv_icrd_a_desc_merc
<a name="cmxcrdsrv_icrd_a_desc_merc"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_desc_merc
<a name="cmxsrv_icrd_lee_desc_merc"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_a_otr_doc
<a name="cmxsrv_icrd_a_otr_doc"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_otr_doc
<a name="cmxsrv_icrd_lee_otr_doc"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_icrd_pre_46](#referencia-cmxsrv_icrd_pre_46)

---

## CMXsrv_iinf_lee0_inf
<a name="cmxsrv_iinf_lee0_inf"></a>

**Procedimientos Referenciados:**

- [PrmACMXFPAIMP](#referencia-prmacmxfpaimp)
- [PrmACMXMONEDA](#referencia-prmacmxmoneda)
- [PrmACLNEJECTA](#referencia-prmaclnejecta)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iinf_lee_tablas
<a name="cmxsrv_iinf_lee_tablas"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iinf_lee1_inf
<a name="cmxsrv_iinf_lee1_inf"></a>

**Procedimientos Referenciados:**

- [PrmACMXCLACOM](#referencia-prmacmxclacom)
- [PrmACMXESPECI](#referencia-prmacmxespeci)
- [sp_procxmode](#referencia-sp_procxmode)
- [PrmACLNEJECTA](#referencia-prmaclnejecta)
- [PrmACMXETDINF](#referencia-prmacmxetdinf)

---

## CMXsrv_iinf_lee_cln
<a name="cmxsrv_iinf_lee_cln"></a>

**Procedimientos Referenciados:**

- [PrmACLNEJECTA](#referencia-prmaclnejecta)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iinf_lee2_inf
<a name="cmxsrv_iinf_lee2_inf"></a>

**Procedimientos Referenciados:**

- [PrmACMXPAIS](#referencia-prmacmxpais)
- [PrmACMXORIDVS](#referencia-prmacmxoridvs)
- [PrmACMXRGMIMP](#referencia-prmacmxrgmimp)
- [sp_procxmode](#referencia-sp_procxmode)
- [PrmACMXBCOBCC](#referencia-prmacmxbcobcc)
- [PrmACMXBCOCEN](#referencia-prmacmxbcocen)
- [PrmACMXSUCSAL](#referencia-prmacmxsucsal)

---

## CMXsrv_iinf_avi_miscb
<a name="cmxsrv_iinf_avi_miscb"></a>

**Procedimientos Referenciados:**

- [PrmACMXBCOBCC](#referencia-prmacmxbcobcc)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iinf_avi_misca
<a name="cmxsrv_iinf_avi_misca"></a>

**Procedimientos Referenciados:**

- [PrmACMXPAIS](#referencia-prmacmxpais)
- [PrmACMXORIDVS](#referencia-prmacmxoridvs)
- [PrmACMXRGMIMP](#referencia-prmacmxrgmimp)
- [PrmACMXCLACOM](#referencia-prmacmxclacom)
- [sp_procxmode](#referencia-sp_procxmode)
- [PrmACMXFPAIMP](#referencia-prmacmxfpaimp)
- [PrmACLNEJECTA](#referencia-prmaclnejecta)
- [PrmACMXSUCSAL](#referencia-prmacmxsucsal)
- [PrmACMXMONEDA](#referencia-prmacmxmoneda)
- [PrmACMXETDINF](#referencia-prmacmxetdinf)

---

## CMXsrv_icrd_lee_dat_com
<a name="cmxsrv_icrd_lee_dat_com"></a>

**Procedimientos Referenciados:**

- [PrmACMXMONEDA](#referencia-prmacmxmoneda)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iinf_eli_inf
<a name="cmxsrv_iinf_eli_inf"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iinf_busc_evi
<a name="cmxsrv_iinf_busc_evi"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iinf_val_inf
<a name="cmxsrv_iinf_val_inf"></a>

**Procedimientos Referenciados:**

- [CMXsrv_cmx_get_codes](#referencia-cmxsrv_cmx_get_codes)
- [PrmACMXPAIS](#referencia-prmacmxpais)
- [PrmACMXCLACOM](#referencia-prmacmxclacom)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iinf_ingmod_inf
<a name="cmxsrv_iinf_ingmod_inf"></a>

**Procedimientos Referenciados:**

- [CMXsrv_util_fecha](#referencia-cmxsrv_util_fecha)
- [sp_procxmode](#referencia-sp_procxmode)
- [PrmACMXMONEDAFEC](#referencia-prmacmxmonedafec)
- [CMXsrv_cmx_get_codes](#referencia-cmxsrv_cmx_get_codes)
- [CMXsrv_iinf_val_inf](#referencia-cmxsrv_iinf_val_inf)
- [CMXsrv_iinf_get_num](#referencia-cmxsrv_iinf_get_num)

---

## CMXsrv_iinf_lee_fec
<a name="cmxsrv_iinf_lee_fec"></a>

**Procedimientos Referenciados:**

- [CMXsrv_util_fecha](#referencia-cmxsrv_util_fecha)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iinf_lee_usd
<a name="cmxsrv_iinf_lee_usd"></a>

**Procedimientos Referenciados:**

- [CMXsrv_cmx_get_codes](#referencia-cmxsrv_cmx_get_codes)
- [PrmACMXMONEDAFEC](#referencia-prmacmxmonedafec)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iinf_act_apr
<a name="cmxsrv_iinf_act_apr"></a>

**Procedimientos Referenciados:**

- [CMXsrv_iinf_val_inf](#referencia-cmxsrv_iinf_val_inf)
- [CMXsrv_util_fecha](#referencia-cmxsrv_util_fecha)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iinf_lee_evi
<a name="cmxsrv_iinf_lee_evi"></a>

**Procedimientos Referenciados:**

- [PrmACMXSUCSAL](#referencia-prmacmxsucsal)
- [PrmACMXBCOCEN](#referencia-prmacmxbcocen)
- [sp_procxmode](#referencia-sp_procxmode)
- [PrmACMXETDINF](#referencia-prmacmxetdinf)

---

## CMXsrv_iinf_act_tib
<a name="cmxsrv_iinf_act_tib"></a>

**Procedimientos Referenciados:**

- [CMXsrv_cmx_get_codes](#referencia-cmxsrv_cmx_get_codes)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iinf_act_rec
<a name="cmxsrv_iinf_act_rec"></a>

**Procedimientos Referenciados:**

- [CMXsrv_util_fecha](#referencia-cmxsrv_util_fecha)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iinf_act_rib
<a name="cmxsrv_iinf_act_rib"></a>

**Procedimientos Referenciados:**

- [CMXsrv_cmx_get_codes](#referencia-cmxsrv_cmx_get_codes)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iinf_busc_comp
<a name="cmxsrv_iinf_busc_comp"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iinf_ingmod_comp
<a name="cmxsrv_iinf_ingmod_comp"></a>

**Procedimientos Referenciados:**

- [CMXsrv_util_fecha](#referencia-cmxsrv_util_fecha)
- [sp_procxmode](#referencia-sp_procxmode)
- [PrmACMXMONEDAFEC](#referencia-prmacmxmonedafec)
- [CMXsrv_cmx_get_codes](#referencia-cmxsrv_cmx_get_codes)
- [CMXsrv_iinf_val_inf](#referencia-cmxsrv_iinf_val_inf)
- [CMXsrv_iinf_get_num](#referencia-cmxsrv_iinf_get_num)

---

## CMXsrv_iinf_lee_comp
<a name="cmxsrv_iinf_lee_comp"></a>

**Procedimientos Referenciados:**

- [PrmACMXPAIS](#referencia-prmacmxpais)
- [PrmACMXORIDVS](#referencia-prmacmxoridvs)
- [PrmACMXRGMIMP](#referencia-prmacmxrgmimp)
- [PrmACMXCLACOM](#referencia-prmacmxclacom)
- [sp_procxmode](#referencia-sp_procxmode)
- [PrmACMXFPAIMP](#referencia-prmacmxfpaimp)
- [PrmACMXVIATPT](#referencia-prmacmxviatpt)
- [PrmACMXMONEDA](#referencia-prmacmxmoneda)

---

## CMXsrv_iinf_lee_bco
<a name="cmxsrv_iinf_lee_bco"></a>

**Procedimientos Referenciados:**

- [PrmACMXPAIS](#referencia-prmacmxpais)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_iinf_busc_bco
<a name="cmxsrv_iinf_busc_bco"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXMCRDsrv_icrd_lee_mcnd
<a name="cmxmcrdsrv_icrd_lee_mcnd"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_mod_ing_let
<a name="cmxsrv_icbr_mod_ing_let"></a>

**Procedimientos Referenciados:**

- [CMXsrv_util_opr_fec](#referencia-cmxsrv_util_opr_fec)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_acep_mod_cbr
<a name="cmxsrv_icbr_acep_mod_cbr"></a>

**Procedimientos Referenciados:**

- [CMXsrv_cnt_2800](#referencia-cmxsrv_cnt_2800)
- [CMXsrv_icbr_cheq_mdoc](#referencia-cmxsrv_icbr_cheq_mdoc)
- [CMXsrv_icbr_val_cbr](#referencia-cmxsrv_icbr_val_cbr)
- [CMXsrv_icbr_cheq_mctp](#referencia-cmxsrv_icbr_cheq_mctp)
- [CMXsrv_icbr_cheq_mter](#referencia-cmxsrv_icbr_cheq_mter)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_icbr_cheq_mlcb](#referencia-cmxsrv_icbr_cheq_mlcb)

---

## CMXsrv_icbr_eli_no_cont
<a name="cmxsrv_icbr_eli_no_cont"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXMCRDsrv_icrd_a_mmcnd
<a name="cmxmcrdsrv_icrd_a_mmcnd"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXMCRDsrv_icrd_lee_mctp
<a name="cmxmcrdsrv_icrd_lee_mctp"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXMCRDsrv_icrd_lee_memb2
<a name="cmxmcrdsrv_icrd_lee_memb2"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXMCRDsrv_icrd_lee_memb1
<a name="cmxmcrdsrv_icrd_lee_memb1"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXMCRDsrv_icrd_lee_mref
<a name="cmxmcrdsrv_icrd_lee_mref"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_ing_txt
<a name="cmxsrv_icrd_ing_txt"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXCRDsrv_icrd_get_ing_esp
<a name="cmxcrdsrv_icrd_get_ing_esp"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXMCRDsrv_icrd_lee_mtxt
<a name="cmxmcrdsrv_icrd_lee_mtxt"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXCRDsrv_icrd_get_pre_fra
<a name="cmxcrdsrv_icrd_get_pre_fra"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXMCRDsrv_icrd_a_mmer
<a name="cmxmcrdsrv_icrd_a_mmer"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_fincol_lee_cod_eve
<a name="cmxsrv_fincol_lee_cod_eve"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXMCRDsrv_icrd_acep_mod_crd
<a name="cmxmcrdsrv_icrd_acep_mod_crd"></a>

**Procedimientos Referenciados:**

- [CMXsrv_icrd_cheq_modoc](#referencia-cmxsrv_icrd_cheq_modoc)
- [CMXCRDsrv_icrd_val_crd](#referencia-cmxcrdsrv_icrd_val_crd)
- [CMXsrv_icrd_cheq_memb](#referencia-cmxsrv_icrd_cheq_memb)
- [CMXsrv_nibx_upd_tran](#referencia-cmxsrv_nibx_upd_tran)
- [CMXsrv_expcce_anl_cce](#referencia-cmxsrv_expcce_anl_cce)
- [CMXsrv_fincol_ctb_mod](#referencia-cmxsrv_fincol_ctb_mod)
- [CMXsrv_icrd_cheq_mtxt](#referencia-cmxsrv_icrd_cheq_mtxt)
- [CMXsrv_icrd_cheq_mcnd](#referencia-cmxsrv_icrd_cheq_mcnd)
- [CMXsrv_icrd_cheq_mmer](#referencia-cmxsrv_icrd_cheq_mmer)
- [CMXsrv_icrd_cheq_mref](#referencia-cmxsrv_icrd_cheq_mref)
- [CMXsrv_nibx_nilive](#referencia-cmxsrv_nibx_nilive)
- [CMXsrv_icrd_cheq_mpmix](#referencia-cmxsrv_icrd_cheq_mpmix)
- [CMXsrv_ctl_crea_apr](#referencia-cmxsrv_ctl_crea_apr)
- [CMXsrv_icrd_cheq_mibar](#referencia-cmxsrv_icrd_cheq_mibar)
- [CMXMCRDsrv_icrd_eli_no_cont](#referencia-cmxmcrdsrv_icrd_eli_no_cont)
- [CMXsrv_icrd_lee_tip_ope](#referencia-cmxsrv_icrd_lee_tip_ope)
- [CMXsrv_icrd_cheq_mmcnd](#referencia-cmxsrv_icrd_cheq_mmcnd)
- [CMXsrv_icrd_cheq_mibab](#referencia-cmxsrv_icrd_cheq_mibab)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_icrd_cheq_mctp](#referencia-cmxsrv_icrd_cheq_mctp)
- [CMXsrv_icrd_cheq_mapr](#referencia-cmxsrv_icrd_cheq_mapr)
- [CMXsrv_cnt_950](#referencia-cmxsrv_cnt_950)

---

## CMXMCRDsrv_icrd_eli_no_cont
<a name="cmxmcrdsrv_icrd_eli_no_cont"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_a_rec_age
<a name="cmxsrv_icrd_a_rec_age"></a>

**Procedimientos Referenciados:**

- [CMXsrv_util_fecha](#referencia-cmxsrv_util_fecha)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_busc_ofi_cta
<a name="cmxsrv_busc_ofi_cta"></a>

**Procedimientos Referenciados:**

- [PrmACMXESPECI](#referencia-prmacmxespeci)
- [PrmACLNEJECTA](#referencia-prmaclnejecta)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_neg_busc_arc
<a name="cmxsrv_neg_busc_arc"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_avi_adi
<a name="cmxsrv_icrd_lee_avi_adi"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_dat_cln
<a name="cmxsrv_icrd_lee_dat_cln"></a>

**Procedimientos Referenciados:**

- [CMXsrv_trae_glo_fec](#referencia-cmxsrv_trae_glo_fec)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_avi_dis
<a name="cmxsrv_icrd_lee_avi_dis"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_neg_ddi_asoc
<a name="cmxsrv_neg_ddi_asoc"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_neg_trae_vcto_mcf
<a name="cmxsrv_neg_trae_vcto_mcf"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_neg_avi_lee_aval
<a name="cmxsrv_neg_avi_lee_aval"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_neg_lee_crd
<a name="cmxsrv_icrd_neg_lee_crd"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_neg
<a name="cmxsrv_icrd_lee_neg"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_col_avi_dat_cln
<a name="cmxsrv_col_avi_dat_cln"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_col_avi_det_pag
<a name="cmxsrv_col_avi_det_pag"></a>

**Procedimientos Referenciados:**

- [CMX_srv_pone_punto](#referencia-cmx_srv_pone_punto)
- [CMXsrv_util_fecha](#referencia-cmxsrv_util_fecha)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_col_avi_det_oto
<a name="cmxsrv_col_avi_det_oto"></a>

**Procedimientos Referenciados:**

- [CMX_srv_pone_punto](#referencia-cmx_srv_pone_punto)
- [CMXsrv_trae_glo_fec](#referencia-cmxsrv_trae_glo_fec)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_col_lee_num_trs
<a name="cmxsrv_col_lee_num_trs"></a>

**Procedimientos Referenciados:**

- [CMXsrv_avigrl_lee_avitemp](#referencia-cmxsrv_avigrl_lee_avitemp)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_finobl_avi_pag
<a name="cmxsrv_finobl_avi_pag"></a>

**Procedimientos Referenciados:**

- [CMX_srv_pone_punto](#referencia-cmx_srv_pone_punto)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_neg_avi_trae_asnd_mn
<a name="cmxsrv_neg_avi_trae_asnd_mn"></a>

**Procedimientos Referenciados:**

- [CMX_srv_pone_punto](#referencia-cmx_srv_pone_punto)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_neg_avi_trae_asnd_mx
<a name="cmxsrv_neg_avi_trae_asnd_mx"></a>

**Procedimientos Referenciados:**

- [CMX_srv_pone_punto](#referencia-cmx_srv_pone_punto)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_cont_neg
<a name="cmxsrv_icrd_cont_neg"></a>

**Procedimientos Referenciados:**

- [CMXsrv_icrd_val_neg](#referencia-cmxsrv_icrd_val_neg)
- [CMXsrv_mbyte_gen](#referencia-cmxsrv_mbyte_gen)
- [sp_procxmode](#referencia-sp_procxmode)
- [sp_cmx_sii_1870](#referencia-sp_cmx_sii_1870)
- [CMXsrv_fincol_ictb_neg_aux](#referencia-cmxsrv_fincol_ictb_neg_aux)

---

## CMXsrv_icrd_eli_neg
<a name="cmxsrv_icrd_eli_neg"></a>

**Procedimientos Referenciados:**

- [CMXsrv_swf_graba_det](#referencia-cmxsrv_swf_graba_det)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_num_col
<a name="cmxsrv_icrd_lee_num_col"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_bus_pago
<a name="cmxsrv_icrd_bus_pago"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_col
<a name="cmxsrv_icrd_lee_col"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_busc_neg
<a name="cmxsrv_icrd_busc_neg"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_a_neg_emb1
<a name="cmxsrv_icrd_a_neg_emb1"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_a_neg_emb2
<a name="cmxsrv_icrd_a_neg_emb2"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_icrd_chq_doc_neg](#referencia-cmxsrv_icrd_chq_doc_neg)

---

## CMXsrv_icrd_eli_doc_neg
<a name="cmxsrv_icrd_eli_doc_neg"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_neg_emb1
<a name="cmxsrv_icrd_lee_neg_emb1"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_neg_emb2
<a name="cmxsrv_icrd_lee_neg_emb2"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_a_neg_disc
<a name="cmxsrv_icrd_a_neg_disc"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_neg_lee_disc
<a name="cmxsrv_icrd_neg_lee_disc"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_icrd_gen_disc](#referencia-cmxsrv_icrd_gen_disc)

---

## CMXsrv_icrd_ent_doc
<a name="cmxsrv_icrd_ent_doc"></a>

**Procedimientos Referenciados:**

- [CMXsrv_mbyte_gen](#referencia-cmxsrv_mbyte_gen)
- [CMXsrv_swf_graba_det](#referencia-cmxsrv_swf_graba_det)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_alz_disc
<a name="cmxsrv_icrd_alz_disc"></a>

**Procedimientos Referenciados:**

- [CMXsrv_get_ult_dia_habil](#referencia-cmxsrv_get_ult_dia_habil)
- [CMXsrv_icrd_cont_alz](#referencia-cmxsrv_icrd_cont_alz)
- [CMXsrv_ipuc_gen_pln](#referencia-cmxsrv_ipuc_gen_pln)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_cnt_950](#referencia-cmxsrv_cnt_950)
- [CMXsrv_cmx_get_codes](#referencia-cmxsrv_cmx_get_codes)
- [CMXsrv_fincol_cal_tas_sfr](#referencia-cmxsrv_fincol_cal_tas_sfr)

---

## CMXCRDsrv_icrd_asignar_cor
<a name="cmxcrdsrv_icrd_asignar_cor"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXCRDsrv_icrd_bus_lcr_bco
<a name="cmxcrdsrv_icrd_bus_lcr_bco"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_act_doc_neg
<a name="cmxsrv_icrd_act_doc_neg"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_lee_doc_neg
<a name="cmxsrv_icrd_lee_doc_neg"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icrd_val_neg
<a name="cmxsrv_icrd_val_neg"></a>

**Procedimientos Referenciados:**

- [CMXsrv_util_det_habil_tasa](#referencia-cmxsrv_util_det_habil_tasa)
- [CMXsrv_fincol_val_per_tas](#referencia-cmxsrv_fincol_val_per_tas)
- [CMXsrv_util_fecha](#referencia-cmxsrv_util_fecha)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_lee_dat_var
<a name="cmxsrv_icbr_lee_dat_var"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_val_pag
<a name="cmxsrv_icbr_val_pag"></a>

**Procedimientos Referenciados:**

- [CMXsrv_val_cta_cte](#referencia-cmxsrv_val_cta_cte)
- [CMXsrv_calc_imp_4pct](#referencia-cmxsrv_calc_imp_4pct)
- [CMXsrv_util_fecha](#referencia-cmxsrv_util_fecha)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_enl_val_sel](#referencia-cmxsrv_enl_val_sel)
- [CMXsrv_ctb_impto_ddi](#referencia-cmxsrv_ctb_impto_ddi)

---

## CMXsrv_icbr_ctb_pag
<a name="cmxsrv_icbr_ctb_pag"></a>

**Procedimientos Referenciados:**

- [CMXsrv_mbyte_gen](#referencia-cmxsrv_mbyte_gen)
- [CMXsrv_get_ult_dia_habil](#referencia-cmxsrv_get_ult_dia_habil)
- [CMXsrv_val_cta_cte](#referencia-cmxsrv_val_cta_cte)
- [CMXsrv_cnt_gen_vig](#referencia-cmxsrv_cnt_gen_vig)
- [CMXsrv_calc_imp_4pct](#referencia-cmxsrv_calc_imp_4pct)
- [CMXsrv_util_fecha](#referencia-cmxsrv_util_fecha)
- [CMXsrv_vig_gra_vig](#referencia-cmxsrv_vig_gra_vig)
- [CMXsrv_ipuc_gen_pln](#referencia-cmxsrv_ipuc_gen_pln)
- [CMXsrv_icbr_act_rem](#referencia-cmxsrv_icbr_act_rem)
- [CMXsrv_enl_act_enl](#referencia-cmxsrv_enl_act_enl)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_icbr_ctb_pag1](#referencia-cmxsrv_icbr_ctb_pag1)
- [sp_cmx_sii_1870](#referencia-sp_cmx_sii_1870)
- [CMXsrv_iddi2_gen_det_pag](#referencia-cmxsrv_iddi2_gen_det_pag)
- [CMXsrv_cmx_get_codes](#referencia-cmxsrv_cmx_get_codes)
- [CMXsrv_ctb_impto_ddi](#referencia-cmxsrv_ctb_impto_ddi)
- [CMXsrv_util_pesos](#referencia-cmxsrv_util_pesos)

---

## CMXsrv_icbr_cal_pag
<a name="cmxsrv_icbr_cal_pag"></a>

**Procedimientos Referenciados:**

- [CMXsrv_get_ult_dia_habil](#referencia-cmxsrv_get_ult_dia_habil)
- [sp_procxmode](#referencia-sp_procxmode)
- [CMXsrv_valida_tc](#referencia-cmxsrv_valida_tc)
- [CMXsrv_icbr_cal_int](#referencia-cmxsrv_icbr_cal_int)
- [CMXsrv_icbr_cre_pln](#referencia-cmxsrv_icbr_cre_pln)

---

## CMXsrv_icbr_eli_pag
<a name="cmxsrv_icbr_eli_pag"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_val_vig
<a name="cmxsrv_val_vig"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_lee_cbr0
<a name="cmxsrv_icbr_lee_cbr0"></a>

**Procedimientos Referenciados:**

- [CMXsrv_icrd_lee_cln](#referencia-cmxsrv_icrd_lee_cln)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_obt_mon_nac
<a name="cmxsrv_icbr_obt_mon_nac"></a>

**Procedimientos Referenciados:**

- [CMXsrv_cmx_get_codes](#referencia-cmxsrv_cmx_get_codes)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_lee_dat_pag
<a name="cmxsrv_icbr_lee_dat_pag"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_pcg_pag
<a name="cmxsrv_icbr_pcg_pag"></a>

**Procedimientos Referenciados:**

- [PrmACMXMONEDAFEC](#referencia-prmacmxmonedafec)
- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_busc_pago
<a name="cmxsrv_icbr_busc_pago"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_eli_int_pago
<a name="cmxsrv_icbr_eli_int_pago"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_busc_int
<a name="cmxsrv_icbr_busc_int"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_ingmod_int
<a name="cmxsrv_icbr_ingmod_int"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_lee_int_pago
<a name="cmxsrv_icbr_lee_int_pago"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_lee_bco
<a name="cmxsrv_icbr_lee_bco"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## CMXsrv_icbr_busc_bco
<a name="cmxsrv_icbr_busc_bco"></a>

**Procedimientos Referenciados:**

- [sp_procxmode](#referencia-sp_procxmode)

---

## Uso de CMXsrv_expcbe_lee_prm
<a name="referencia-cmxsrv_expcbe_lee_prm"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_cmx_busc_suc_usu
<a name="referencia-cmxsrv_cmx_busc_suc_usu"></a>

**Este procedimiento es invocado en:**

- **Exportaciones → EXPCBE**: CMXsrv_expcbe_lee_cbe
- **Exportaciones → EXPCBE**: CMXsrv_expcbe_lee_cbe
- **Exportaciones → EXPCBE**: CMXsrv_expcbe_lee_cbe
- **Exportaciones → EXPCCE**: CMXsrv_expcce_cre_cce
- **Exportaciones → EXPNEG**: CMXsrv_expcce_lee_neg
- **Exportaciones → EXPNEG**: CMXsrv_expcce_grb_neg
- **Exportaciones → expret**: CMXsrv_expret_lee_ret
- **Exportaciones → expret**: CMXsrv_expret_cre_ret

---

## Uso de CMXsrv_expcbe_lee_cbe
<a name="referencia-cmxsrv_expcbe_lee_cbe"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_trae_glo_fec
<a name="referencia-cmxsrv_trae_glo_fec"></a>

**Este procedimiento es invocado en:**

- **Exportaciones → EXPCBE**: CMXsrv_expcbe_avs_rem1
- **Exportaciones → EXPCCE**: CMXsrv_expcce_avs_rem1
- **Exportaciones → EXPNEG**: CMXsrv_expcce_avs_rem1
- **Importaciones → NEGO_AV**: CMXsrv_icrd_lee_dat_cln
- **Importaciones → NEGO_AV**: CMXsrv_icrd_lee_dat_cln
- **Importaciones → NEGO_AV**: CMXsrv_col_avi_det_oto

---

## Uso de CMXsrv_expcbe_avs_cyg1
<a name="referencia-cmxsrv_expcbe_avs_cyg1"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_avs_cyg2
<a name="referencia-cmxsrv_expcbe_avs_cyg2"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_avs_ret
<a name="referencia-cmxsrv_expcbe_avs_ret"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_swf_sel
<a name="referencia-cmxsrv_expcbe_swf_sel"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_anl_cbe
<a name="referencia-cmxsrv_expcbe_anl_cbe"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_ctb_ing
<a name="referencia-cmxsrv_expcbe_ctb_ing"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_del_cbe
<a name="referencia-cmxsrv_expcbe_del_cbe"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_val_cbe
<a name="referencia-cmxsrv_expcbe_val_cbe"></a>

**Este procedimiento es invocado en:**

- **Exportaciones → EXPCBE**: CMXsrv_expcbe_ctb_ing
- **Exportaciones → EXPCBE**: CMXsrv_expcbe_avs_rem1

---

## Uso de CMXsrv_expcbe_grb_ctp
<a name="referencia-cmxsrv_expcbe_grb_ctp"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_lee_cln
<a name="referencia-cmxsrv_expcbe_lee_cln"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_val_suc
<a name="referencia-cmxsrv_val_suc"></a>

**Este procedimiento es invocado en:**

- **Exportaciones → EXPCBE**: CMXsrv_expcbe_lee_cbe
- **Exportaciones → EXPCBE**: CMXsrv_expcbe_lee_cbe
- **Exportaciones → EXPCBE**: CMXsrv_expcbe_lee_cbe

---

## Uso de CMXsrv_expcbe_lee_ctp
<a name="referencia-cmxsrv_expcbe_lee_ctp"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_grb_bco
<a name="referencia-cmxsrv_expcbe_grb_bco"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_lee_cor
<a name="referencia-cmxsrv_expcbe_lee_cor"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_lee_bco
<a name="referencia-cmxsrv_expcbe_lee_bco"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_grb_doc
<a name="referencia-cmxsrv_expcbe_grb_doc"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_grb_doc02
<a name="referencia-cmxsrv_expcbe_grb_doc02"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_lee_doc
<a name="referencia-cmxsrv_expcbe_lee_doc"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_lee_doc02
<a name="referencia-cmxsrv_expcbe_lee_doc02"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_del_ctz
<a name="referencia-cmxsrv_expcbe_del_ctz"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_bus_ctz
<a name="referencia-cmxsrv_expcbe_bus_ctz"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_grb_ctz
<a name="referencia-cmxsrv_expcbe_grb_ctz"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_mto_ctz
<a name="referencia-cmxsrv_expcbe_mto_ctz"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_lee_ctz
<a name="referencia-cmxsrv_expcbe_lee_ctz"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_bus_cbe
<a name="referencia-cmxsrv_expcbe_bus_cbe"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_mdf_cbe
<a name="referencia-cmxsrv_expcbe_mdf_cbe"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_cre_actz
<a name="referencia-cmxsrv_expcbe_cre_actz"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_lee_mdf
<a name="referencia-cmxsrv_expcbe_lee_mdf"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_pgo_cbe
<a name="referencia-cmxsrv_expcbe_pgo_cbe"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_lee_pgo
<a name="referencia-cmxsrv_expcbe_lee_pgo"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_bus_evz
<a name="referencia-cmxsrv_expcbe_bus_evz"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_rev_cbe
<a name="referencia-cmxsrv_expcbe_rev_cbe"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_lee_evz
<a name="referencia-cmxsrv_expcbe_lee_evz"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_del_dcz
<a name="referencia-cmxsrv_expcbe_del_dcz"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_bus_dcz
<a name="referencia-cmxsrv_expcbe_bus_dcz"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_grb_dcz
<a name="referencia-cmxsrv_expcbe_grb_dcz"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_lee_dcz
<a name="referencia-cmxsrv_expcbe_lee_dcz"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_bus_vto
<a name="referencia-cmxsrv_expcbe_bus_vto"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_avi_dat_cou
<a name="referencia-cmxsrv_avi_dat_cou"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_avs_rem1
<a name="referencia-cmxsrv_expcbe_avs_rem1"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_avs_rem3
<a name="referencia-cmxsrv_expcbe_avs_rem3"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_avs_rem2
<a name="referencia-cmxsrv_expcbe_avs_rem2"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_avs_rem4
<a name="referencia-cmxsrv_expcbe_avs_rem4"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_busc_plz
<a name="referencia-cmxsrv_busc_plz"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_lee_plz
<a name="referencia-cmxsrv_lee_plz"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_cor_busc_pais
<a name="referencia-cmxsrv_cor_busc_pais"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_cor_lee_pais
<a name="referencia-cmxsrv_cor_lee_pais"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcbe_bus_cor
<a name="referencia-cmxsrv_expcbe_bus_cor"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_busc_bco_mtr
<a name="referencia-cmxsrv_busc_bco_mtr"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_grl_fec_serv
<a name="referencia-cmxsrv_grl_fec_serv"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_lee_cce
<a name="referencia-cmxsrv_expcce_lee_cce"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_trd_cce
<a name="referencia-cmxsrv_expcce_trd_cce"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_anl_cce
<a name="referencia-cmxsrv_expcce_anl_cce"></a>

**Este procedimiento es invocado en:**

- **Importaciones → MOD_CRD**: CMXMCRDsrv_icrd_acep_mod_crd

---

## Uso de CMXsrv_expcce_ctb_ing
<a name="referencia-cmxsrv_expcce_ctb_ing"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_del_cce
<a name="referencia-cmxsrv_expcce_del_cce"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_val_cce
<a name="referencia-cmxsrv_expcce_val_cce"></a>

**Este procedimiento es invocado en:**

- **Exportaciones → EXPCCE**: CMXsrv_expcce_ctb_ing

---

## Uso de CMXsrv_expcce_swf_sel
<a name="referencia-cmxsrv_expcce_swf_sel"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_grb_bco
<a name="referencia-cmxsrv_expcce_grb_bco"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_lee_cor
<a name="referencia-cmxsrv_expcce_lee_cor"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_lee_bco
<a name="referencia-cmxsrv_expcce_lee_bco"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_grb_ctp
<a name="referencia-cmxsrv_expcce_grb_ctp"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_lee_cln
<a name="referencia-cmxsrv_expcce_lee_cln"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_lee_ctp
<a name="referencia-cmxsrv_expcce_lee_ctp"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_cre_cce
<a name="referencia-cmxsrv_expcce_cre_cce"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_gen_dcc
<a name="referencia-cmxsrv_expcce_gen_dcc"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_grb_cnd
<a name="referencia-cmxsrv_expcce_grb_cnd"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_util_det_habil
<a name="referencia-cmxsrv_util_det_habil"></a>

**Este procedimiento es invocado en:**

- **Financiamiento → PAGOS**: CMXsrv_fincol_efec_calpa
- **Importaciones → MOD_CRD**: CMXsrv_fincol_efec_calpa
- **Importaciones → MOD_CRD**: CMXsrv_fincol_efec_calpa

---

## Uso de CMXsrv_expcce_lee_cnd
<a name="referencia-cmxsrv_expcce_lee_cnd"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_trd_cnd
<a name="referencia-cmxsrv_expcce_trd_cnd"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_del_dcc
<a name="referencia-cmxsrv_expcce_del_dcc"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_bus_dcc
<a name="referencia-cmxsrv_expcce_bus_dcc"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_grb_dcc
<a name="referencia-cmxsrv_expcce_grb_dcc"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_lee_dcc
<a name="referencia-cmxsrv_expcce_lee_dcc"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_bus_cce
<a name="referencia-cmxsrv_expcce_bus_cce"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_mdf_cce
<a name="referencia-cmxsrv_expcce_mdf_cce"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_can_mdf
<a name="referencia-cmxsrv_expcce_can_mdf"></a>

**Este procedimiento es invocado en:**

- **Exportaciones → EXPCCE**: CMXsrv_expcce_mdf_cce

---

## Uso de CMXsrv_expcce_lee_mdf
<a name="referencia-cmxsrv_expcce_lee_mdf"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_cnf_cce
<a name="referencia-cmxsrv_expcce_cnf_cce"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_grb_afin
<a name="referencia-cmxsrv_expcce_grb_afin"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_lee_cnf
<a name="referencia-cmxsrv_expcce_lee_cnf"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_lee_afin
<a name="referencia-cmxsrv_expcce_lee_afin"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_trp_cce
<a name="referencia-cmxsrv_expcce_trp_cce"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_lee_trp
<a name="referencia-cmxsrv_expcce_lee_trp"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_bus_evc
<a name="referencia-cmxsrv_expcce_bus_evc"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_rev_cce
<a name="referencia-cmxsrv_expcce_rev_cce"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_lee_evc
<a name="referencia-cmxsrv_expcce_lee_evc"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_avs_rem1
<a name="referencia-cmxsrv_expcce_avs_rem1"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_bus_cor
<a name="referencia-cmxsrv_expcce_bus_cor"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_dex_lee_dex
<a name="referencia-cmxsrv_dex_lee_dex"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_dex_eli_dex
<a name="referencia-cmxsrv_dex_eli_dex"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_dex_act_dex
<a name="referencia-cmxsrv_dex_act_dex"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expdex_cal_fec
<a name="referencia-cmxsrv_expdex_cal_fec"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_dex_lee_cli
<a name="referencia-cmxsrv_dex_lee_cli"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_dex_bus_dex
<a name="referencia-cmxsrv_dex_bus_dex"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_lee_bas
<a name="referencia-cmxsrv_expcce_lee_bas"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_lee_neg
<a name="referencia-cmxsrv_expcce_lee_neg"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_alz_dis
<a name="referencia-cmxsrv_expcce_alz_dis"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_anl_neg
<a name="referencia-cmxsrv_expcce_anl_neg"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_ctb_neg
<a name="referencia-cmxsrv_expcce_ctb_neg"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_del_neg
<a name="referencia-cmxsrv_expcce_del_neg"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_val_neg
<a name="referencia-cmxsrv_expcce_val_neg"></a>

**Este procedimiento es invocado en:**

- **Exportaciones → EXPNEG**: CMXsrv_expcce_ctb_neg

---

## Uso de CMXsrv_expcce_grb_neg
<a name="referencia-cmxsrv_expcce_grb_neg"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_gen_dcn
<a name="referencia-cmxsrv_expcce_gen_dcn"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_avs_rem5
<a name="referencia-cmxsrv_expcce_avs_rem5"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_lee_nge
<a name="referencia-cmxsrv_expcce_lee_nge"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_trd_nge
<a name="referencia-cmxsrv_expcce_trd_nge"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_ini_neg
<a name="referencia-cmxsrv_expcce_ini_neg"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_del_dcn
<a name="referencia-cmxsrv_expcce_del_dcn"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_bus_dcn
<a name="referencia-cmxsrv_expcce_bus_dcn"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_grb_dcn
<a name="referencia-cmxsrv_expcce_grb_dcn"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_lee_dcn
<a name="referencia-cmxsrv_expcce_lee_dcn"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_del_ltr
<a name="referencia-cmxsrv_expcce_del_ltr"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_bus_ltr
<a name="referencia-cmxsrv_expcce_bus_ltr"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_grb_ltr
<a name="referencia-cmxsrv_expcce_grb_ltr"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_lee_ltr
<a name="referencia-cmxsrv_expcce_lee_ltr"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_del_dsn
<a name="referencia-cmxsrv_expcce_del_dsn"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_gen_dsn
<a name="referencia-cmxsrv_expcce_gen_dsn"></a>

**Este procedimiento es invocado en:**

- **Exportaciones → EXPCCE**: CMXsrv_expcce_rev_cce
- **Exportaciones → EXPNEG**: CMXsrv_expcce_rev_cce

---

## Uso de CMXsrv_expcce_bus_dsn
<a name="referencia-cmxsrv_expcce_bus_dsn"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_chk_dsn
<a name="referencia-cmxsrv_expcce_chk_dsn"></a>

**Este procedimiento es invocado en:**

- **Exportaciones → EXPCCE**: CMXsrv_expcce_rev_cce
- **Exportaciones → EXPNEG**: CMXsrv_expcce_rev_cce
- **Exportaciones → EXPNEG**: CMXsrv_expcce_grb_dsn

---

## Uso de CMXsrv_expcce_grb_dsn
<a name="referencia-cmxsrv_expcce_grb_dsn"></a>

**Este procedimiento es invocado en:**

- **Exportaciones → EXPNEG**: CMXsrv_expcce_gen_dsn

---

## Uso de CMXsrv_expcce_lee_dsn
<a name="referencia-cmxsrv_expcce_lee_dsn"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_bus_neg
<a name="referencia-cmxsrv_expcce_bus_neg"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_pgo_neg
<a name="referencia-cmxsrv_expcce_pgo_neg"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_lee_pgo
<a name="referencia-cmxsrv_expcce_lee_pgo"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_avs_rem3
<a name="referencia-cmxsrv_expcce_avs_rem3"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_avs_rem2
<a name="referencia-cmxsrv_expcce_avs_rem2"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expcce_avs_rem4
<a name="referencia-cmxsrv_expcce_avs_rem4"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_swf_sel
<a name="referencia-cmxsrv_expret_swf_sel"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_lee_ret
<a name="referencia-cmxsrv_expret_lee_ret"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_lee_prm
<a name="referencia-cmxsrv_expret_lee_prm"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_avs_cyg1
<a name="referencia-cmxsrv_expret_avs_cyg1"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_avs_cyg2
<a name="referencia-cmxsrv_expret_avs_cyg2"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_avs_liq1
<a name="referencia-cmxsrv_expret_avs_liq1"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_avs_liq2
<a name="referencia-cmxsrv_expret_avs_liq2"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_avs_liq3
<a name="referencia-cmxsrv_expret_avs_liq3"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_val_ret
<a name="referencia-cmxsrv_expret_val_ret"></a>

**Este procedimiento es invocado en:**

- **Exportaciones → expret**: CMXsrv_expret_ctb_ing

---

## Uso de CMXsrv_expret_sum_dtn_mn
<a name="referencia-cmxsrv_expret_sum_dtn_mn"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_ctb_ing
<a name="referencia-cmxsrv_expret_ctb_ing"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_del_ret
<a name="referencia-cmxsrv_expret_del_ret"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_avs_adm1
<a name="referencia-cmxsrv_expret_avs_adm1"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_avs_adm2
<a name="referencia-cmxsrv_expret_avs_adm2"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_avs_adm3
<a name="referencia-cmxsrv_expret_avs_adm3"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_act_tpo_cbo
<a name="referencia-cmxsrv_expret_act_tpo_cbo"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_cre_ret
<a name="referencia-cmxsrv_expret_cre_ret"></a>

**Este procedimiento es invocado en:**

- **Exportaciones → EXPCBE**: CMXsrv_expcbe_pgo_cbe
- **Exportaciones → EXPNEG**: CMXsrv_expcce_pgo_neg
- **Exportaciones → expret**: CMXsrv_expret_ctb_ing

---

## Uso de CMXsrv_expret_grb_det
<a name="referencia-cmxsrv_expret_grb_det"></a>

**Este procedimiento es invocado en:**

- **Exportaciones → EXPCBE**: CMXsrv_expcbe_pgo_cbe
- **Exportaciones → EXPNEG**: CMXsrv_expcce_pgo_neg
- **Exportaciones → expret**: CMXsrv_expret_ctb_ing

---

## Uso de CMXsrv_expret_tpo_cbo
<a name="referencia-cmxsrv_expret_tpo_cbo"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_lee_cln
<a name="referencia-cmxsrv_expret_lee_cln"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_lee_det
<a name="referencia-cmxsrv_expret_lee_det"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_del_org
<a name="referencia-cmxsrv_expret_del_org"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_bus_org
<a name="referencia-cmxsrv_expret_bus_org"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_grb_org
<a name="referencia-cmxsrv_expret_grb_org"></a>

**Este procedimiento es invocado en:**

- **Exportaciones → EXPCBE**: CMXsrv_expcbe_pgo_cbe
- **Exportaciones → EXPNEG**: CMXsrv_expcce_pgo_neg
- **Exportaciones → expret**: CMXsrv_expret_ctb_ing

---

## Uso de CMXsrv_expret_mto_org
<a name="referencia-cmxsrv_expret_mto_org"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_lee_org
<a name="referencia-cmxsrv_expret_lee_org"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_vig_lee_cta
<a name="referencia-cmxsrv_vig_lee_cta"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_del_dtn
<a name="referencia-cmxsrv_expret_del_dtn"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_bus_dtn
<a name="referencia-cmxsrv_expret_bus_dtn"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_grb_dtn
<a name="referencia-cmxsrv_expret_grb_dtn"></a>

**Este procedimiento es invocado en:**

- **Exportaciones → EXPCBE**: CMXsrv_expcbe_pgo_cbe
- **Exportaciones → EXPNEG**: CMXsrv_expcce_pgo_neg
- **Exportaciones → expret**: CMXsrv_expret_ctb_ing

---

## Uso de CMXsrv_expret_cal_arb
<a name="referencia-cmxsrv_expret_cal_arb"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_mto_dtn
<a name="referencia-cmxsrv_expret_mto_dtn"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_lee_dtn
<a name="referencia-cmxsrv_expret_lee_dtn"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_bus_ret
<a name="referencia-cmxsrv_expret_bus_ret"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_bus_evr
<a name="referencia-cmxsrv_expret_bus_evr"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_rev_ret
<a name="referencia-cmxsrv_expret_rev_ret"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_expret_lee_evr
<a name="referencia-cmxsrv_expret_lee_evr"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finadm_imod_desti
<a name="referencia-cmxsrv_finadm_imod_desti"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finadm_cons_dtip
<a name="referencia-cmxsrv_finadm_cons_dtip"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finadm_imod_ectb
<a name="referencia-cmxsrv_finadm_imod_ectb"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finadm_eli_tipop
<a name="referencia-cmxsrv_finadm_eli_tipop"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finadm_cons_ectb
<a name="referencia-cmxsrv_finadm_cons_ectb"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finadm_imod_itip
<a name="referencia-cmxsrv_finadm_imod_itip"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finadm_cons_itip
<a name="referencia-cmxsrv_finadm_cons_itip"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finadm_lee_tipop
<a name="referencia-cmxsrv_finadm_lee_tipop"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finadm_val_tipop
<a name="referencia-cmxsrv_finadm_val_tipop"></a>

**Este procedimiento es invocado en:**

- **Financiamiento → ADMIN**: CMXsrv_finadm_imod_desti
- **Financiamiento → ADMIN**: CMXsrv_finadm_imod_ectb
- **Financiamiento → ADMIN**: CMXsrv_finadm_imod_itip

---

## Uso de CMXsrv_finadm_bus_tipope
<a name="referencia-cmxsrv_finadm_bus_tipope"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_busc_tip_tas
<a name="referencia-cmxsrv_busc_tip_tas"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_ecuo
<a name="referencia-cmxsrv_fincol_ecuo"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_cons_plnpa
<a name="referencia-cmxsrv_fincol_cons_plnpa"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_pertas_val_display
<a name="referencia-cmxsrv_pertas_val_display"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_eava
<a name="referencia-cmxsrv_fincol_eava"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_cons_aval
<a name="referencia-cmxsrv_fincol_cons_aval"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_iava
<a name="referencia-cmxsrv_fincol_iava"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_cons_pag
<a name="referencia-cmxsrv_fincol_cons_pag"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_trae_det_pag
<a name="referencia-cmxsrv_fincol_trae_det_pag"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_cons_pror
<a name="referencia-cmxsrv_fincol_cons_pror"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_cons_eve
<a name="referencia-cmxsrv_fincol_cons_eve"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_bco_swf
<a name="referencia-cmxsrv_icrd_lee_bco_swf"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_busc_bco
<a name="referencia-cmxsrv_icrd_busc_bco"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_vtocre_prov
<a name="referencia-cmxsrv_fincol_vtocre_prov"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_prec_vtocre
<a name="referencia-cmxsrv_fincol_prec_vtocre"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_bus_lcr_bco
<a name="referencia-cmxsrv_icrd_bus_lcr_bco"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_lee_fpro
<a name="referencia-cmxsrv_lee_fpro"></a>

**Este procedimiento es invocado en:**

- **Exportaciones → EXPCBE**: CMXsrv_expcbe_lee_prm
- **Exportaciones → EXPCBE**: CMXsrv_expcbe_lee_cbe
- **Exportaciones → EXPCBE**: CMXsrv_expcbe_lee_cbe
- **Exportaciones → EXPCBE**: CMXsrv_expcbe_mdf_cbe
- **Exportaciones → EXPCBE**: CMXsrv_expcbe_lee_pgo
- **Exportaciones → EXPCBE**: CMXsrv_expcbe_rev_cbe
- **Exportaciones → EXPCBE**: CMXsrv_expcbe_lee_cbe
- **Exportaciones → expdex**: CMXsrv_expcbe_lee_prm
- **Exportaciones → expdex**: CMXsrv_dex_act_dex
- **Exportaciones → expdex**: CMXsrv_dex_act_dex
- **Exportaciones → EXPNEG**: CMXsrv_expcbe_rev_cbe
- **Exportaciones → expret**: CMXsrv_expret_lee_ret
- **Exportaciones → expret**: CMXsrv_expret_lee_prm
- **Exportaciones → expret**: CMXsrv_expret_val_ret
- **Exportaciones → expret**: CMXsrv_expret_val_ret
- **Exportaciones → expret**: CMXsrv_expret_val_ret
- **Exportaciones → expret**: CMXsrv_expret_cre_ret
- **Exportaciones → expret**: CMXsrv_expret_tpo_cbo
- **Exportaciones → expret**: CMXsrv_expret_lee_det
- **Financiamiento → INGRESO**: CMXsrv_fincol_ren_fin
- **Financiamiento → INGRESO**: CMXsrv_fincol_ren_fin
- **Financiamiento → INGRESO**: CMXsrv_fincol_ctb_oto
- **Financiamiento → INGRESO**: CMXsrv_fincol_ctb_oto
- **Financiamiento → INGRESO**: CMXsrv_fincol_ctb_novf
- **Financiamiento → OBLIGA**: CMXsrv_finobl_calc_anu
- **Financiamiento → OBLIGA**: CMXsrv_finobl_calc_anu
- **Financiamiento → OBLIGA**: CMXsrv_finobl_ctb_oto
- **Financiamiento → OBLIGA**: CMXsrv_finobl_ictb_pag
- **Financiamiento → OBLIGA**: CMXsrv_finobl_calc_pror
- **Financiamiento → OBLIGA**: CMXsrv_finobl_ctb_anu
- **Financiamiento → OBLIGA**: CMXsrv_finobl_calc_anu
- **Financiamiento → OBLIGA**: CMXsrv_finobl_cesion_obl
- **Financiamiento → PAGOS**: CMXsrv_fincol_cont_pror
- **Financiamiento → PAGOS**: CMXsrv_fincol_cctb_anu
- **Financiamiento → PGOEXT**: CMXsrv_fincol_ctb_pext
- **Financiamiento → PGOEXT**: CMXsrv_finobl_ctb_pext

---

## Uso de CMXsrv_fincol_ren_fin
<a name="referencia-cmxsrv_fincol_ren_fin"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_gmod_ctr
<a name="referencia-cmxsrv_fincol_gmod_ctr"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_lee_bco
<a name="referencia-cmxsrv_fincol_lee_bco"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_lee_cln
<a name="referencia-cmxsrv_fincol_lee_cln"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_cons_ctr
<a name="referencia-cmxsrv_fincol_cons_ctr"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_ctb_oto
<a name="referencia-cmxsrv_fincol_ctb_oto"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_dat_liq_ope
<a name="referencia-cmxsrv_icrd_dat_liq_ope"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_lee_col
<a name="referencia-cmxsrv_fincol_lee_col"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_busc_cod_ope
<a name="referencia-cmxsrv_busc_cod_ope"></a>

**Este procedimiento es invocado en:**

- **Financiamiento → PAGOS**: CMXsrv_fincol_cctb_anu
- **Importaciones → IMPORT**: CMXsrv_icrd_a_cnd
- **Importaciones → MOD_ADI**: CMXsrv_icrd_a_cnd
- **Importaciones → MOD_CRD**: CMXsrv_icrd_a_cnd

---

## Uso de CMXsrv_col_trae_num_ope
<a name="referencia-cmxsrv_col_trae_num_ope"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_eli_col
<a name="referencia-cmxsrv_fincol_eli_col"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_val_col
<a name="referencia-cmxsrv_fincol_val_col"></a>

**Este procedimiento es invocado en:**

- **Financiamiento → INGRESO**: CMXsrv_fincol_ctb_oto
- **Financiamiento → INGRESO**: CMXsrv_fincol_ctb_oto

---

## Uso de CMXsrv_fincol_bsc_col
<a name="referencia-cmxsrv_fincol_bsc_col"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_lee_tip
<a name="referencia-cmxsrv_fincol_lee_tip"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_ctb_novf
<a name="referencia-cmxsrv_fincol_ctb_novf"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_cons_nov
<a name="referencia-cmxsrv_fincol_cons_nov"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_cmx_get_codes
<a name="referencia-cmxsrv_cmx_get_codes"></a>

**Este procedimiento es invocado en:**

- **Exportaciones → EXPCCE**: CMXsrv_expcce_val_cce
- **Exportaciones → EXPCCE**: CMXsrv_expcce_mdf_cce
- **Exportaciones → EXPNEG**: CMXsrv_expcce_pgo_neg
- **Financiamiento → PAGOS**: CMXsrv_fincol_cont_pror
- **Importaciones → ARCOS**: CMXsrv_iarc_act_arc
- **Importaciones → ARCOS**: CMXsrv_iarc_act_arc
- **Importaciones → COBERIMP**: CMXsrv_icob_lee_pln
- **Importaciones → COBERIMP**: CMXsrv_icob_pag_sop
- **Importaciones → COBERIMP**: CMXsrv_icob_crea_reem
- **Importaciones → COBERIMP**: CMXsrv_icob_pag_sop
- **Importaciones → COBERIMP**: CMXsrv_icob_anu
- **Importaciones → COBERIMP**: CMXsrv_icob_pag_sop
- **Importaciones → DDI**: CMXsrv_iddi_asoc_ddi
- **Importaciones → INFORME**: CMXsrv_iinf_val_inf
- **Importaciones → INFORME**: CMXsrv_iinf_ingmod_inf
- **Importaciones → INFORME**: CMXsrv_iinf_lee_usd
- **Importaciones → INFORME**: CMXsrv_iinf_act_tib
- **Importaciones → INFORME**: CMXsrv_iinf_act_rib
- **Importaciones → INFORME**: CMXsrv_iinf_ingmod_comp
- **Importaciones → NNEGO**: CMXsrv_icrd_alz_disc
- **Importaciones → PAGCBR**: CMXsrv_icbr_ctb_pag
- **Importaciones → PAGCBR**: CMXsrv_icbr_obt_mon_nac

---

## Uso de CMXsrv_grl_trae_cod_bco
<a name="referencia-cmxsrv_grl_trae_cod_bco"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_cons_tas
<a name="referencia-cmxsrv_fincol_cons_tas"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_efec_tras
<a name="referencia-cmxsrv_fincol_efec_tras"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_cons_trasp
<a name="referencia-cmxsrv_fincol_cons_trasp"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_cons_dtrs
<a name="referencia-cmxsrv_fincol_cons_dtrs"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_cons_deve
<a name="referencia-cmxsrv_fincol_cons_deve"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_cont_gst
<a name="referencia-cmxsrv_fincol_cont_gst"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_cons_gst
<a name="referencia-cmxsrv_fincol_cons_gst"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_cons_dgst
<a name="referencia-cmxsrv_fincol_cons_dgst"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_bsc_tip
<a name="referencia-cmxsrv_fincol_bsc_tip"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_bus_cor
<a name="referencia-cmxsrv_finobl_bus_cor"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_ecuo
<a name="referencia-cmxsrv_finobl_ecuo"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_gpln
<a name="referencia-cmxsrv_finobl_gpln"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_cons_plnpa
<a name="referencia-cmxsrv_finobl_cons_plnpa"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_calc_anu
<a name="referencia-cmxsrv_finobl_calc_anu"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_lee_obl
<a name="referencia-cmxsrv_finobl_lee_obl"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_ctb_oto
<a name="referencia-cmxsrv_finobl_ctb_oto"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_eli_obl
<a name="referencia-cmxsrv_fincol_eli_obl"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_val_obl
<a name="referencia-cmxsrv_finobl_val_obl"></a>

**Este procedimiento es invocado en:**

- **Financiamiento → OBLIGA**: CMXsrv_finobl_ctb_oto

---

## Uso de CMXsrv_finobl_bsc_obl
<a name="referencia-cmxsrv_finobl_bsc_obl"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_ictb_pag
<a name="referencia-cmxsrv_finobl_ictb_pag"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_obt_sdocuo
<a name="referencia-cmxsrv_finobl_obt_sdocuo"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_new_tas
<a name="referencia-cmxsrv_finobl_new_tas"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_cons_pag
<a name="referencia-cmxsrv_finobl_cons_pag"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_cons_detp
<a name="referencia-cmxsrv_finobl_cons_detp"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_calc_pror
<a name="referencia-cmxsrv_finobl_calc_pror"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_cons_pror
<a name="referencia-cmxsrv_finobl_cons_pror"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_cons_dpror
<a name="referencia-cmxsrv_finobl_cons_dpror"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_ctb_anu
<a name="referencia-cmxsrv_finobl_ctb_anu"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_cons_anu
<a name="referencia-cmxsrv_finobl_cons_anu"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_cons_mod
<a name="referencia-cmxsrv_finobl_cons_mod"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_cons_dmod
<a name="referencia-cmxsrv_finobl_cons_dmod"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_rev_eve
<a name="referencia-cmxsrv_finobl_rev_eve"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_cons_eve
<a name="referencia-cmxsrv_finobl_cons_eve"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_cons_deve
<a name="referencia-cmxsrv_finobl_cons_deve"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_eli_ctr
<a name="referencia-cmxsrv_finobl_eli_ctr"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_cons_ctr
<a name="referencia-cmxsrv_finobl_cons_ctr"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_ing_ctr
<a name="referencia-cmxsrv_finobl_ing_ctr"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_cesion_obl
<a name="referencia-cmxsrv_finobl_cesion_obl"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_comgrl_lee_nom_cor
<a name="referencia-cmxsrv_comgrl_lee_nom_cor"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_lee_cln
<a name="referencia-cmxsrv_lee_cln"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_busc_acre
<a name="referencia-cmxsrv_finobl_busc_acre"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_efec_calpa
<a name="referencia-cmxsrv_fincol_efec_calpa"></a>

**Este procedimiento es invocado en:**

- **Financiamiento → COL_NEG**: CMXsrv_fincol_vtocre_prov
- **Financiamiento → PAGOS**: CMXsrv_fincol_calc_pror
- **Financiamiento → PAGOS**: CMXsrv_fincol_calc_anu
- **Financiamiento → PAGOS**: CMXsrv_fincol_calc_anu

---

## Uso de CMXsrv_fincol_cons_detp
<a name="referencia-cmxsrv_fincol_cons_detp"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_calc_pror
<a name="referencia-cmxsrv_fincol_calc_pror"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_cont_pror
<a name="referencia-cmxsrv_fincol_cont_pror"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_cons_dpror
<a name="referencia-cmxsrv_fincol_cons_dpror"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_cctb_anu
<a name="referencia-cmxsrv_fincol_cctb_anu"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_calc_anu
<a name="referencia-cmxsrv_fincol_calc_anu"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_cons_anu
<a name="referencia-cmxsrv_fincol_cons_anu"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_cons_mod
<a name="referencia-cmxsrv_fincol_cons_mod"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_cons_dmod
<a name="referencia-cmxsrv_fincol_cons_dmod"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_cal_pext
<a name="referencia-cmxsrv_fincol_cal_pext"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_ctb_pext
<a name="referencia-cmxsrv_fincol_ctb_pext"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_cal_pext
<a name="referencia-cmxsrv_finobl_cal_pext"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_ctb_pext
<a name="referencia-cmxsrv_finobl_ctb_pext"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iarc_eli_arc
<a name="referencia-cmxsrv_iarc_eli_arc"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iarc_busc_arc
<a name="referencia-cmxsrv_iarc_busc_arc"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_busc_inf
<a name="referencia-cmxsrv_iinf_busc_inf"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iarc_act_arc
<a name="referencia-cmxsrv_iarc_act_arc"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iarc_lee_arc
<a name="referencia-cmxsrv_iarc_lee_arc"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_busc_opr
<a name="referencia-cmxsrv_iinf_busc_opr"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_lee_vlr
<a name="referencia-cmxsrv_iinf_lee_vlr"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_rev_evi
<a name="referencia-cmxsrv_iinf_rev_evi"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icob_lee_pln
<a name="referencia-cmxsrv_icob_lee_pln"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icob_cur_cob
<a name="referencia-cmxsrv_icob_cur_cob"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icob_pag_sop
<a name="referencia-cmxsrv_icob_pag_sop"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icob_eli_pln
<a name="referencia-cmxsrv_icob_eli_pln"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icob_rev_etd
<a name="referencia-cmxsrv_icob_rev_etd"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icob_val_cob
<a name="referencia-cmxsrv_icob_val_cob"></a>

**Este procedimiento es invocado en:**

- **Importaciones → COBERIMP**: CMXsrv_icob_cur_cob
- **Importaciones → COBERIMP**: CMXsrv_icob_pag_sop
- **Importaciones → COBERIMP**: CMXsrv_icob_act_gral
- **Importaciones → COBERIMP**: CMXsrv_icob_act_val
- **Importaciones → COBERIMP**: CMXsrv_icob_act_acu
- **Importaciones → COBERIMP**: CMXsrv_icob_ingmod_int
- **Importaciones → COBERIMP**: CMXsrv_icob_pag_sop
- **Importaciones → COBERIMP**: CMXsrv_icob_pag_sop
- **Importaciones → COBERIMP**: CMXsrv_icob_cur_reem
- **Importaciones → PAGCBR**: CMXsrv_icob_act_val

---

## Uso de CMXsrv_icob_busc_pln
<a name="referencia-cmxsrv_icob_busc_pln"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icob_lee_cln
<a name="referencia-cmxsrv_icob_lee_cln"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icob_crea_norm
<a name="referencia-cmxsrv_icob_crea_norm"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icob_crea_reem
<a name="referencia-cmxsrv_icob_crea_reem"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icob_act_gral
<a name="referencia-cmxsrv_icob_act_gral"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icob_lee_cln2
<a name="referencia-cmxsrv_icob_lee_cln2"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icob_lee_gral
<a name="referencia-cmxsrv_icob_lee_gral"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icob_act_val
<a name="referencia-cmxsrv_icob_act_val"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icob_lee_val
<a name="referencia-cmxsrv_icob_lee_val"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icob_act_acu
<a name="referencia-cmxsrv_icob_act_acu"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icob_lee_acu
<a name="referencia-cmxsrv_icob_lee_acu"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icob_eli_int
<a name="referencia-cmxsrv_icob_eli_int"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icob_busc_int
<a name="referencia-cmxsrv_icob_busc_int"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icob_ingmod_int
<a name="referencia-cmxsrv_icob_ingmod_int"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icob_lee_int
<a name="referencia-cmxsrv_icob_lee_int"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icob_ing_mod_srf
<a name="referencia-cmxsrv_icob_ing_mod_srf"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icob_anu
<a name="referencia-cmxsrv_icob_anu"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icob_lee_anu
<a name="referencia-cmxsrv_icob_lee_anu"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icob_cur_reem
<a name="referencia-cmxsrv_icob_cur_reem"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_busc_cor_swf
<a name="referencia-cmxsrv_busc_cor_swf"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_swf_bus_sms
<a name="referencia-cmxsrv_swf_bus_sms"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_lee_cbr
<a name="referencia-cmxsrv_icbr_lee_cbr"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_acep_let
<a name="referencia-cmxsrv_icbr_acep_let"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_cont_cbr
<a name="referencia-cmxsrv_icbr_cont_cbr"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_eli_cbr
<a name="referencia-cmxsrv_icbr_eli_cbr"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_lee_ctp
<a name="referencia-cmxsrv_icbr_lee_ctp"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_avi1
<a name="referencia-cmxsrv_icbr_avi1"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_busc_cbr
<a name="referencia-cmxsrv_icbr_busc_cbr"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_lee_cln
<a name="referencia-cmxsrv_icbr_lee_cln"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_crea_cbr
<a name="referencia-cmxsrv_icbr_crea_cbr"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_lee_cob
<a name="referencia-cmxsrv_icbr_lee_cob"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_act_ctp
<a name="referencia-cmxsrv_icbr_act_ctp"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_lee_trm
<a name="referencia-cmxsrv_icbr_lee_trm"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_act_trm
<a name="referencia-cmxsrv_icbr_act_trm"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_lee_doc
<a name="referencia-cmxsrv_icbr_lee_doc"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_act_doc
<a name="referencia-cmxsrv_icbr_act_doc"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_busc_let
<a name="referencia-cmxsrv_icbr_busc_let"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_ingmod_let
<a name="referencia-cmxsrv_icbr_ingmod_let"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_eli_let
<a name="referencia-cmxsrv_icbr_eli_let"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_lee_let
<a name="referencia-cmxsrv_icbr_lee_let"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_prorr
<a name="referencia-cmxsrv_icbr_prorr"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_rev_eve
<a name="referencia-cmxsrv_icbr_rev_eve"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_busc_eve
<a name="referencia-cmxsrv_icbr_busc_eve"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_lee_eve
<a name="referencia-cmxsrv_icbr_lee_eve"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_lee_ent_doc
<a name="referencia-cmxsrv_icbr_lee_ent_doc"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_prot
<a name="referencia-cmxsrv_icbr_prot"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_pcg_prot
<a name="referencia-cmxsrv_icbr_pcg_prot"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_liq_sdo
<a name="referencia-cmxsrv_icbr_liq_sdo"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_act_vis
<a name="referencia-cmxsrv_icbr_act_vis"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_eli_rep
<a name="referencia-cmxsrv_icbr_eli_rep"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_busc_rep
<a name="referencia-cmxsrv_icbr_busc_rep"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_imod_rep
<a name="referencia-cmxsrv_icbr_imod_rep"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_ent_doc
<a name="referencia-cmxsrv_icbr_ent_doc"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_trf_ofi
<a name="referencia-cmxsrv_icbr_trf_ofi"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_trf_bco
<a name="referencia-cmxsrv_icbr_trf_bco"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_act_inst
<a name="referencia-cmxsrv_icbr_act_inst"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iswf_a_pru
<a name="referencia-cmxsrv_iswf_a_pru"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_val_cbr
<a name="referencia-cmxsrv_icbr_val_cbr"></a>

**Este procedimiento es invocado en:**

- **Importaciones → COBRANZA**: CMXsrv_icbr_cont_cbr
- **Importaciones → COBRANZA**: CMXsrv_icbr_act_trm
- **Importaciones → MOD_CBR**: CMXsrv_icbr_act_trm
- **Importaciones → MOD_CBR**: CMXsrv_icbr_acep_mod_cbr

---

## Uso de CMXsrv_icrd_a_ibab
<a name="referencia-cmxsrv_icrd_a_ibab"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_glo_ibab
<a name="referencia-cmxsrv_icrd_lee_glo_ibab"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_a_ibar
<a name="referencia-cmxsrv_icrd_a_ibar"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_glo_ibar
<a name="referencia-cmxsrv_icrd_lee_glo_ibar"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_tex_swf
<a name="referencia-cmxsrv_icrd_lee_tex_swf"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_cod_txt_swf
<a name="referencia-cmxsrv_icrd_lee_cod_txt_swf"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_txt_swf_all
<a name="referencia-cmxsrv_icrd_lee_txt_swf_all"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_ind_esp_ing
<a name="referencia-cmxsrv_icrd_lee_ind_esp_ing"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_ing_acu
<a name="referencia-cmxsrv_icrd_ing_acu"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_acu
<a name="referencia-cmxsrv_icrd_lee_acu"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_rech_sol
<a name="referencia-cmxsrv_icrd_rech_sol"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_end
<a name="referencia-cmxsrv_icrd_end"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_dat_end
<a name="referencia-cmxsrv_icrd_lee_dat_end"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_asignar_cor
<a name="referencia-cmxsrv_icrd_asignar_cor"></a>

**Este procedimiento es invocado en:**

- **Importaciones → IMPORT**: CMXCRDsrv_icrd_apr_sol

---

## Uso de CMXsrv_icrd_lee_bco_mtr
<a name="referencia-cmxsrv_icrd_lee_bco_mtr"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_cor_lee_pais
<a name="referencia-cmxsrv_icrd_cor_lee_pais"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_plz
<a name="referencia-cmxsrv_icrd_lee_plz"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_busc_plz
<a name="referencia-cmxsrv_icrd_busc_plz"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_cor_busc_pais
<a name="referencia-cmxsrv_icrd_cor_busc_pais"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_busc_bco_mtr
<a name="referencia-cmxsrv_icrd_busc_bco_mtr"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iddi_ingmod_ddi
<a name="referencia-cmxsrv_iddi_ingmod_ddi"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iddi_lee_dec
<a name="referencia-cmxsrv_iddi_lee_dec"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iddi_eli_ddi
<a name="referencia-cmxsrv_iddi_eli_ddi"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iddi_lee_inf
<a name="referencia-cmxsrv_iddi_lee_inf"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iddi_lee_cln
<a name="referencia-cmxsrv_iddi_lee_cln"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iddi_lee_rut
<a name="referencia-cmxsrv_iddi_lee_rut"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iddi_asoc_ddi
<a name="referencia-cmxsrv_iddi_asoc_ddi"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iddi_des_ddi
<a name="referencia-cmxsrv_iddi_des_ddi"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iddi_busc_asoc
<a name="referencia-cmxsrv_iddi_busc_asoc"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iddi_busc_noasoc
<a name="referencia-cmxsrv_iddi_busc_noasoc"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_dir_cln
<a name="referencia-cmxsrv_icrd_lee_dir_cln"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXCRDsrv_icrd_a_cnd_esp
<a name="referencia-cmxcrdsrv_icrd_a_cnd_esp"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_cnd_esp
<a name="referencia-cmxsrv_icrd_lee_cnd_esp"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXCRDsrv_icrd_clon_crd
<a name="referencia-cmxcrdsrv_icrd_clon_crd"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXCRDsrv_icrd_lee_crdcre
<a name="referencia-cmxcrdsrv_icrd_lee_crdcre"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_top
<a name="referencia-cmxsrv_icrd_lee_top"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXCRDsrv_icrd_val_crd
<a name="referencia-cmxcrdsrv_icrd_val_crd"></a>

**Este procedimiento es invocado en:**

- **Importaciones → MOD_CRD**: CMXMCRDsrv_icrd_acep_mod_crd

---

## Uso de CMXCRDsrv_icrd_eli_crd
<a name="referencia-cmxcrdsrv_icrd_eli_crd"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_dat_trs
<a name="referencia-cmxsrv_icrd_lee_dat_trs"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_a_ctp
<a name="referencia-cmxsrv_icrd_a_ctp"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_cln
<a name="referencia-cmxsrv_icrd_lee_cln"></a>

**Este procedimiento es invocado en:**

- **Exportaciones → EXPCBE**: CMXsrv_expcbe_lee_bco
- **Financiamiento → COL_NEG**: CMXsrv_icrd_lee_bco_swf
- **Financiamiento → INGRESO**: CMXsrv_icrd_lee_bco_swf
- **Financiamiento → INGRESO**: CMXsrv_icrd_lee_bco_swf
- **Importaciones → MOD_ADI**: CMXsrv_icrd_lee_bco_swf
- **Importaciones → MOD_CRD**: CMXsrv_icrd_lee_bco_swf
- **Importaciones → MOD_CRD**: CMXsrv_icrd_lee_bco_swf
- **Importaciones → MOD_CRD**: CMXsrv_icrd_lee_bco_swf
- **Importaciones → PAGCBR**: CMXsrv_icbr_lee_cbr0

---

## Uso de CMXsrv_icrd_a_cnd
<a name="referencia-cmxsrv_icrd_a_cnd"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXCRDsrv_icrd_crea_crd
<a name="referencia-cmxcrdsrv_icrd_crea_crd"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_busc_emb
<a name="referencia-cmxsrv_icrd_busc_emb"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_eli_emb
<a name="referencia-cmxsrv_icrd_eli_emb"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_emb1
<a name="referencia-cmxsrv_icrd_lee_emb1"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_emb2
<a name="referencia-cmxsrv_icrd_lee_emb2"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_a_emb1
<a name="referencia-cmxsrv_icrd_a_emb1"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_a_emb2
<a name="referencia-cmxsrv_icrd_a_emb2"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_val_emb2
<a name="referencia-cmxsrv_icrd_val_emb2"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_val_emb1
<a name="referencia-cmxsrv_icrd_val_emb1"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_act_ref
<a name="referencia-cmxsrv_icrd_act_ref"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_ref
<a name="referencia-cmxsrv_icrd_lee_ref"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXCRDsrv_icrd_apr_sol
<a name="referencia-cmxcrdsrv_icrd_apr_sol"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_crdapr
<a name="referencia-cmxsrv_icrd_lee_crdapr"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXCRDsrv_icrd_a_desc_merc
<a name="referencia-cmxcrdsrv_icrd_a_desc_merc"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_desc_merc
<a name="referencia-cmxsrv_icrd_lee_desc_merc"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_a_otr_doc
<a name="referencia-cmxsrv_icrd_a_otr_doc"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_otr_doc
<a name="referencia-cmxsrv_icrd_lee_otr_doc"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_lee0_inf
<a name="referencia-cmxsrv_iinf_lee0_inf"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_lee_tablas
<a name="referencia-cmxsrv_iinf_lee_tablas"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_lee1_inf
<a name="referencia-cmxsrv_iinf_lee1_inf"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_lee_cln
<a name="referencia-cmxsrv_iinf_lee_cln"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_lee2_inf
<a name="referencia-cmxsrv_iinf_lee2_inf"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_avi_miscb
<a name="referencia-cmxsrv_iinf_avi_miscb"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_avi_misca
<a name="referencia-cmxsrv_iinf_avi_misca"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_dat_com
<a name="referencia-cmxsrv_icrd_lee_dat_com"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_eli_inf
<a name="referencia-cmxsrv_iinf_eli_inf"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_busc_evi
<a name="referencia-cmxsrv_iinf_busc_evi"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_val_inf
<a name="referencia-cmxsrv_iinf_val_inf"></a>

**Este procedimiento es invocado en:**

- **Importaciones → INFORME**: CMXsrv_iinf_ingmod_inf
- **Importaciones → INFORME**: CMXsrv_iinf_act_apr
- **Importaciones → INFORME**: CMXsrv_iinf_ingmod_comp

---

## Uso de CMXsrv_iinf_ingmod_inf
<a name="referencia-cmxsrv_iinf_ingmod_inf"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_lee_fec
<a name="referencia-cmxsrv_iinf_lee_fec"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_lee_usd
<a name="referencia-cmxsrv_iinf_lee_usd"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_act_apr
<a name="referencia-cmxsrv_iinf_act_apr"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_lee_evi
<a name="referencia-cmxsrv_iinf_lee_evi"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_act_tib
<a name="referencia-cmxsrv_iinf_act_tib"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_act_rec
<a name="referencia-cmxsrv_iinf_act_rec"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_act_rib
<a name="referencia-cmxsrv_iinf_act_rib"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_busc_comp
<a name="referencia-cmxsrv_iinf_busc_comp"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_ingmod_comp
<a name="referencia-cmxsrv_iinf_ingmod_comp"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_lee_comp
<a name="referencia-cmxsrv_iinf_lee_comp"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_lee_bco
<a name="referencia-cmxsrv_iinf_lee_bco"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_iinf_busc_bco
<a name="referencia-cmxsrv_iinf_busc_bco"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXMCRDsrv_icrd_lee_mcnd
<a name="referencia-cmxmcrdsrv_icrd_lee_mcnd"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_mod_ing_let
<a name="referencia-cmxsrv_icbr_mod_ing_let"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_acep_mod_cbr
<a name="referencia-cmxsrv_icbr_acep_mod_cbr"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_eli_no_cont
<a name="referencia-cmxsrv_icbr_eli_no_cont"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXMCRDsrv_icrd_a_mmcnd
<a name="referencia-cmxmcrdsrv_icrd_a_mmcnd"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXMCRDsrv_icrd_lee_mctp
<a name="referencia-cmxmcrdsrv_icrd_lee_mctp"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXMCRDsrv_icrd_lee_memb2
<a name="referencia-cmxmcrdsrv_icrd_lee_memb2"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXMCRDsrv_icrd_lee_memb1
<a name="referencia-cmxmcrdsrv_icrd_lee_memb1"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXMCRDsrv_icrd_lee_mref
<a name="referencia-cmxmcrdsrv_icrd_lee_mref"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_ing_txt
<a name="referencia-cmxsrv_icrd_ing_txt"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXCRDsrv_icrd_get_ing_esp
<a name="referencia-cmxcrdsrv_icrd_get_ing_esp"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXMCRDsrv_icrd_lee_mtxt
<a name="referencia-cmxmcrdsrv_icrd_lee_mtxt"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXCRDsrv_icrd_get_pre_fra
<a name="referencia-cmxcrdsrv_icrd_get_pre_fra"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXMCRDsrv_icrd_a_mmer
<a name="referencia-cmxmcrdsrv_icrd_a_mmer"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_fincol_lee_cod_eve
<a name="referencia-cmxsrv_fincol_lee_cod_eve"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXMCRDsrv_icrd_acep_mod_crd
<a name="referencia-cmxmcrdsrv_icrd_acep_mod_crd"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXMCRDsrv_icrd_eli_no_cont
<a name="referencia-cmxmcrdsrv_icrd_eli_no_cont"></a>

**Este procedimiento es invocado en:**

- **Importaciones → MOD_CRD**: CMXMCRDsrv_icrd_acep_mod_crd

---

## Uso de CMXsrv_icrd_a_rec_age
<a name="referencia-cmxsrv_icrd_a_rec_age"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_busc_ofi_cta
<a name="referencia-cmxsrv_busc_ofi_cta"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_neg_busc_arc
<a name="referencia-cmxsrv_neg_busc_arc"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_avi_adi
<a name="referencia-cmxsrv_icrd_lee_avi_adi"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_dat_cln
<a name="referencia-cmxsrv_icrd_lee_dat_cln"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_avi_dis
<a name="referencia-cmxsrv_icrd_lee_avi_dis"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_neg_ddi_asoc
<a name="referencia-cmxsrv_neg_ddi_asoc"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_neg_trae_vcto_mcf
<a name="referencia-cmxsrv_neg_trae_vcto_mcf"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_neg_avi_lee_aval
<a name="referencia-cmxsrv_neg_avi_lee_aval"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_neg_lee_crd
<a name="referencia-cmxsrv_icrd_neg_lee_crd"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_neg
<a name="referencia-cmxsrv_icrd_lee_neg"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_col_avi_dat_cln
<a name="referencia-cmxsrv_col_avi_dat_cln"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_col_avi_det_pag
<a name="referencia-cmxsrv_col_avi_det_pag"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_col_avi_det_oto
<a name="referencia-cmxsrv_col_avi_det_oto"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_col_lee_num_trs
<a name="referencia-cmxsrv_col_lee_num_trs"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_finobl_avi_pag
<a name="referencia-cmxsrv_finobl_avi_pag"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_neg_avi_trae_asnd_mn
<a name="referencia-cmxsrv_neg_avi_trae_asnd_mn"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_neg_avi_trae_asnd_mx
<a name="referencia-cmxsrv_neg_avi_trae_asnd_mx"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_cont_neg
<a name="referencia-cmxsrv_icrd_cont_neg"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_eli_neg
<a name="referencia-cmxsrv_icrd_eli_neg"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_num_col
<a name="referencia-cmxsrv_icrd_lee_num_col"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_bus_pago
<a name="referencia-cmxsrv_icrd_bus_pago"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_col
<a name="referencia-cmxsrv_icrd_lee_col"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_busc_neg
<a name="referencia-cmxsrv_icrd_busc_neg"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_a_neg_emb1
<a name="referencia-cmxsrv_icrd_a_neg_emb1"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_a_neg_emb2
<a name="referencia-cmxsrv_icrd_a_neg_emb2"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_eli_doc_neg
<a name="referencia-cmxsrv_icrd_eli_doc_neg"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_neg_emb1
<a name="referencia-cmxsrv_icrd_lee_neg_emb1"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_neg_emb2
<a name="referencia-cmxsrv_icrd_lee_neg_emb2"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_a_neg_disc
<a name="referencia-cmxsrv_icrd_a_neg_disc"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_neg_lee_disc
<a name="referencia-cmxsrv_icrd_neg_lee_disc"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_ent_doc
<a name="referencia-cmxsrv_icrd_ent_doc"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_alz_disc
<a name="referencia-cmxsrv_icrd_alz_disc"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXCRDsrv_icrd_asignar_cor
<a name="referencia-cmxcrdsrv_icrd_asignar_cor"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXCRDsrv_icrd_bus_lcr_bco
<a name="referencia-cmxcrdsrv_icrd_bus_lcr_bco"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_act_doc_neg
<a name="referencia-cmxsrv_icrd_act_doc_neg"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_lee_doc_neg
<a name="referencia-cmxsrv_icrd_lee_doc_neg"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icrd_val_neg
<a name="referencia-cmxsrv_icrd_val_neg"></a>

**Este procedimiento es invocado en:**

- **Importaciones → NEGO_AV**: CMXsrv_icrd_cont_neg
- **Importaciones → NNEGO**: CMXsrv_icrd_cont_neg

---

## Uso de CMXsrv_icbr_lee_dat_var
<a name="referencia-cmxsrv_icbr_lee_dat_var"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_val_pag
<a name="referencia-cmxsrv_icbr_val_pag"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_ctb_pag
<a name="referencia-cmxsrv_icbr_ctb_pag"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_cal_pag
<a name="referencia-cmxsrv_icbr_cal_pag"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_eli_pag
<a name="referencia-cmxsrv_icbr_eli_pag"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_val_vig
<a name="referencia-cmxsrv_val_vig"></a>

**Este procedimiento es invocado en:**

- **Exportaciones → expret**: CMXsrv_expret_val_ret
- **Exportaciones → expret**: CMXsrv_expret_val_ret
- **Exportaciones → expret**: CMXsrv_expret_val_ret

---

## Uso de CMXsrv_icbr_lee_cbr0
<a name="referencia-cmxsrv_icbr_lee_cbr0"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_obt_mon_nac
<a name="referencia-cmxsrv_icbr_obt_mon_nac"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_lee_dat_pag
<a name="referencia-cmxsrv_icbr_lee_dat_pag"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_pcg_pag
<a name="referencia-cmxsrv_icbr_pcg_pag"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_busc_pago
<a name="referencia-cmxsrv_icbr_busc_pago"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_eli_int_pago
<a name="referencia-cmxsrv_icbr_eli_int_pago"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_busc_int
<a name="referencia-cmxsrv_icbr_busc_int"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_ingmod_int
<a name="referencia-cmxsrv_icbr_ingmod_int"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_lee_int_pago
<a name="referencia-cmxsrv_icbr_lee_int_pago"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_lee_bco
<a name="referencia-cmxsrv_icbr_lee_bco"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

## Uso de CMXsrv_icbr_busc_bco
<a name="referencia-cmxsrv_icbr_busc_bco"></a>

**Este procedimiento es invocado en:**

- No se encontraron referencias.

---

