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
<a name="expcbe" ></a>

| **Segmento** | **Tabla Referenciada** | **Procedimiento Almacenado** |
|-------------|----------------------|--------------------------|
| Form_Activate | ACMXPRMGRL | [CMXsrv_expcbe_lee_prm](#cmxsrv_expcbe_lee_prm) |
| Form_Activate | master..sysprocesses, tbl_User | [CMXsrv_cmx_busc_suc_usu](#cmxsrv_cmx_busc_suc_usu) |
| Form_Activate | ACMXPAIS, COR, ACMXPGOCBE, CBE01, CBE, ACMXMONEDA, ACMXENTDOC, ACMXSUCSAL, ACMXPRTCBE, CLN | [CMXsrv_expcbe_lee_cbe](#cmxsrv_expcbe_lee_cbe) |
| Form_Load | ACMXSUCSAL, ACMXDL3475FEC, tbl_User | [CMXsrv_trae_glo_fec](#cmxsrv_trae_glo_fec) |
| ingcomg_Click | ACMXDESEMB, ASND, ACMXIMPUES, ACMXPRMGRL, EVZ, CBE, COM, TRSD, CLN, ACMXESPECI | [CMXsrv_expcbe_avs_cyg1](#cmxsrv_expcbe_avs_cyg1) |
| ingcomg_Click | ASND, ACMXIMPUES, ACMXPRMGRL, EVZ, CBE | [CMXsrv_expcbe_avs_cyg2](#cmxsrv_expcbe_avs_cyg2) |
| ingret_Click | ACMXPAIS, COR, ACMXDESEMB, CBE, ACMXMONEDA, ACMXSUCSAL, CLN, ACMXESPECI, RET | [CMXsrv_expcbe_avs_ret](#cmxsrv_expcbe_avs_ret) |
| M3_Click | switxt, switxt1 | [CMXsrv_expcbe_swf_sel](#cmxsrv_expcbe_swf_sel) |
| M4_Click | switxt, switxt1 | [CMXsrv_expcbe_swf_sel](#cmxsrv_expcbe_swf_sel) |
| Mcbeanl_Click | CBE | [CMXsrv_expcbe_anl_cbe](#cmxsrv_expcbe_anl_cbe) |
| Mcbectb_Click | OPE_BCI, CBE | [CMXsrv_expcbe_ctb_ing](#cmxsrv_expcbe_ctb_ing) |
| Mcbedel_Click | EVL, CBE01, COD, CBE, EVZ, COM, ACTZ, CTZ | [CMXsrv_expcbe_del_cbe](#cmxsrv_expcbe_del_cbe) |
| Mcbeval_Click | COR, CBE01, ACMXPRMGRL, CBE, DCZ, CTZ, warnmsg, ACMXPAIS, ACMXFERIADO, CCO | [CMXsrv_expcbe_val_cbe](#cmxsrv_expcbe_val_cbe) |
| Men1_Click | switxt, switxt1 | [CMXsrv_expcbe_swf_sel](#cmxsrv_expcbe_swf_sel) |
| aceptar_Click | ACMXPAIS, CBE | [CMXsrv_expcbe_grb_ctp](#cmxsrv_expcbe_grb_ctp) |
| fld_cbe_cod_exp_lostfocus | CLN | [CMXsrv_expcbe_lee_cln](#cmxsrv_expcbe_lee_cln) |
| fld_cbe_cod_suc_LostFocus | ACMXSUCSAL, tbl_User | [CMXsrv_val_suc](#cmxsrv_val_suc) |
| Form_Activate | ACMXSUCSAL, ACMXPAIS, CBE, CLN | [CMXsrv_expcbe_lee_ctp](#cmxsrv_expcbe_lee_ctp) |
| aceptar_Click | ACMXPRMGRL, CBE, COR, CBE01 | [CMXsrv_expcbe_grb_bco](#cmxsrv_expcbe_grb_bco) |
| fld_cbe_cod_cob_Lostfocus | ACMXPAIS, COR | [CMXsrv_expcbe_lee_cor](#cmxsrv_expcbe_lee_cor) |
| fld_cbe_cod_rmb_LostFocus | ACMXPAIS, COR | [CMXsrv_expcbe_lee_cor](#cmxsrv_expcbe_lee_cor) |
| Form_Activate | CBE, COR, CBE01 | [CMXsrv_expcbe_lee_bco](#cmxsrv_expcbe_lee_bco) |
| aceptar_Click | CBE, DCZ | [CMXsrv_expcbe_grb_doc](#cmxsrv_expcbe_grb_doc) |
| aceptar_Click | CBE02 | [CMXsrv_expcbe_grb_doc02](#cmxsrv_expcbe_grb_doc02) |
| Form_Activate | CBE | [CMXsrv_expcbe_lee_doc](#cmxsrv_expcbe_lee_doc) |
| Form_Activate | CBE02 | [CMXsrv_expcbe_lee_doc02](#cmxsrv_expcbe_lee_doc02) |
| ELIMINAR_Click | ACTZ, CBE, CTZ | [CMXsrv_expcbe_del_ctz](#cmxsrv_expcbe_del_ctz) |
| Form_Activate | ACTZ, CBE, CTZ | [CMXsrv_expcbe_bus_ctz](#cmxsrv_expcbe_bus_ctz) |
| aceptar_Click | ACTZ, CBE, CTZ | [CMXsrv_expcbe_grb_ctz](#cmxsrv_expcbe_grb_ctz) |
| Form_Activate | ACTZ, CBE, CTZ | [CMXsrv_expcbe_mto_ctz](#cmxsrv_expcbe_mto_ctz) |
| Form_Activate | ACTZ, CBE, CTZ | [CMXsrv_expcbe_lee_ctz](#cmxsrv_expcbe_lee_ctz) |
| aceptar_Click | ACMXPAIS, COR, ACMXPGOCBE, CBE01, CBE, ACMXMONEDA, ACMXENTDOC, ACMXSUCSAL, ACMXPRTCBE, CLN | [CMXsrv_expcbe_lee_cbe](#cmxsrv_expcbe_lee_cbe) |
| buscar_Click | CBE | [CMXsrv_expcbe_bus_cbe](#cmxsrv_expcbe_bus_cbe) |
| fld_aux_cod_exp_LostFocus | CLN | [CMXsrv_expcbe_lee_cln](#cmxsrv_expcbe_lee_cln) |
| Proximas_Click | CBE | [CMXsrv_expcbe_bus_cbe](#cmxsrv_expcbe_bus_cbe) |
| aceptar_Click | ACTZ, ACMXPRMGRL, CBE | [CMXsrv_expcbe_mdf_cbe](#cmxsrv_expcbe_mdf_cbe) |
| aceptar_Click | ACTZ, CBE, CTZ | [CMXsrv_expcbe_cre_actz](#cmxsrv_expcbe_cre_actz) |
| fld_cbe_cod_suc_LostFocus | ACMXSUCSAL, tbl_User | [CMXsrv_val_suc](#cmxsrv_val_suc) |
| Form_Activate | COR, ACMXPGOCBE, CBE01, CBE, ACMXMONEDA, ACMXSUCSAL, CLN | [CMXsrv_expcbe_lee_mdf](#cmxsrv_expcbe_lee_mdf) |
| aceptar_Click | ACMXDESEMB, COR, CLN, RET, vig_cmx, COD, ACMXIMPUES, ACMXPRMGRL, CBE, ACMXPRMEXP, COM, tbl_User, OPREC, ACMXPAIS, ACMXFERIADO, CCO | [CMXsrv_expcbe_pgo_cbe](#cmxsrv_expcbe_pgo_cbe) |
| fld_cbe_cod_rmb_LostFocus | ACMXPAIS, COR | [CMXsrv_expcbe_lee_cor](#cmxsrv_expcbe_lee_cor) |
| Form_Activate | ACMXDESEMB, COR, CBE, ACMXPRMEXP, ACMXMONEDA, OPREC, CLN | [CMXsrv_expcbe_lee_pgo](#cmxsrv_expcbe_lee_pgo) |
| Form_Activate | EVZ, CBE | [CMXsrv_expcbe_bus_evz](#cmxsrv_expcbe_bus_evz) |
| Proximo_Click | EVZ, CBE | [CMXsrv_expcbe_bus_evz](#cmxsrv_expcbe_bus_evz) |
| Reversar_Click | EVL, ACMXDESEMB, COR, ORG, ACMXIMPUES, ACMXPRMGRL, EVZ, CBE, TRSD, ACMXPRMEXP, COM, EVR, CTZ, DTN, OPREC, RET, PUCBCX10 | [CMXsrv_expcbe_rev_cbe](#cmxsrv_expcbe_rev_cbe) |
| Form_Activate | ACMXDESEMB, COR, ACMXPGOCBE, EVZ, CBE, ACMXMONEDA, ACMXTIPEVE, ACMXSUCSAL | [CMXsrv_expcbe_lee_evz](#cmxsrv_expcbe_lee_evz) |
| Eliminar_Click | CBE02, CBE, DCZ | [CMXsrv_expcbe_del_dcz](#cmxsrv_expcbe_del_dcz) |
| Form_Activate | DCZ | [CMXsrv_expcbe_bus_dcz](#cmxsrv_expcbe_bus_dcz) |
| aceptar_Click | CBE02, CBE, DCZ | [CMXsrv_expcbe_grb_dcz](#cmxsrv_expcbe_grb_dcz) |
| Form_Activate | DCZ | [CMXsrv_expcbe_lee_dcz](#cmxsrv_expcbe_lee_dcz) |
| aceptar_Click | ACMXPAIS, COR, ACMXPGOCBE, CBE01, CBE, ACMXMONEDA, ACMXENTDOC, ACMXSUCSAL, ACMXPRTCBE, CLN | [CMXsrv_expcbe_lee_cbe](#cmxsrv_expcbe_lee_cbe) |
| buscar_Click | CBE | [CMXsrv_expcbe_bus_vto](#cmxsrv_expcbe_bus_vto) |
| fld_aux_cod_exp_LostFocus | CLN | [CMXsrv_expcbe_lee_cln](#cmxsrv_expcbe_lee_cln) |
| Proximas_Click | CBE | [CMXsrv_expcbe_bus_vto](#cmxsrv_expcbe_bus_vto) |
| aceptar_Click |  | [CMXsrv_avi_dat_cou](#cmxsrv_avi_dat_cou) |
| aceptar_Click | COR, ACMXPGOCBE, ACMXPRTCBE, CBE01, CBE, CBE02, ACMXMONEDA, CTZ, ACMXENTDOC, ACMXPAIS, ACMXPAISES, CLN | [CMXsrv_expcbe_avs_rem1](#cmxsrv_expcbe_avs_rem1) |
| aceptar_Click | COR, CBE01, CBE, CTZ, ACMXMONEDA, ACMXPAISES, CLN, CCO | [CMXsrv_expcbe_avs_rem3](#cmxsrv_expcbe_avs_rem3) |
| imprime_esp | CBE02, CBE, DCZ | [CMXsrv_expcbe_avs_rem2](#cmxsrv_expcbe_avs_rem2) |
| imprime_esp | ACMXREMFESPMSG, ACMXREMFINGMSG | [CMXsrv_expcbe_avs_rem4](#cmxsrv_expcbe_avs_rem4) |
| imprime_ing | CBE02, CBE, DCZ | [CMXsrv_expcbe_avs_rem2](#cmxsrv_expcbe_avs_rem2) |
| imprime_ing | ACMXREMFESPMSG, ACMXREMFINGMSG | [CMXsrv_expcbe_avs_rem4](#cmxsrv_expcbe_avs_rem4) |
| buscar_Click | ACMXPLAZAS, comex..ACMXPLAZAS | [CMXsrv_busc_plz](#cmxsrv_busc_plz) |
| fld_cor_cod_plz_Lostfocus | ACMXPLAZAS | [CMXsrv_lee_plz](#cmxsrv_lee_plz) |
| proximos_Click | ACMXPLAZAS, comex..ACMXPLAZAS | [CMXsrv_busc_plz](#cmxsrv_busc_plz) |
| buscar_Click | ACMXPAIS | [CMXsrv_cor_busc_pais](#cmxsrv_cor_busc_pais) |
| fld_cor_cod_pais_LostFocus | comex..ACMXPAIS | [CMXsrv_cor_lee_pais](#cmxsrv_cor_lee_pais) |
| proximos_Click | ACMXPAIS | [CMXsrv_cor_busc_pais](#cmxsrv_cor_busc_pais) |
| aceptar_Click | ACMXPAIS, COR | [CMXsrv_expcbe_lee_cor](#cmxsrv_expcbe_lee_cor) |
| buscar_Click | COR | [CMXsrv_expcbe_bus_cor](#cmxsrv_expcbe_bus_cor) |
| fld_aux_cod_pai_LostFocus | comex..ACMXPAIS | [CMXsrv_cor_lee_pais](#cmxsrv_cor_lee_pais) |
| fld_aux_cod_plz_LostFocus | ACMXPLAZAS | [CMXsrv_lee_plz](#cmxsrv_lee_plz) |
| proximos_Click | COR | [CMXsrv_expcbe_bus_cor](#cmxsrv_expcbe_bus_cor) |
| buscar_Click | ACMXBANCOS | [CMXsrv_busc_bco_mtr](#cmxsrv_busc_bco_mtr) |
| proximos_Click | ACMXBANCOS | [CMXsrv_busc_bco_mtr](#cmxsrv_busc_bco_mtr) |
| enviar_Click | switxt, switxt1 | [CMXsrv_expcbe_swf_sel](#cmxsrv_expcbe_swf_sel) |
| Aceptar_Click | ACMXPAIS, COR | [CMXsrv_expcbe_lee_cor](#cmxsrv_expcbe_lee_cor) |
| buscar_Click | COR | [CMXsrv_expcbe_bus_cor](#cmxsrv_expcbe_bus_cor) |
| proximos_Click | COR | [CMXsrv_expcbe_bus_cor](#cmxsrv_expcbe_bus_cor) |
| Form_Load |  | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |

---

## EXPCCE
<a name="expcce" ></a>

| **Segmento** | **Tabla Referenciada** | **Procedimiento Almacenado** |
|-------------|----------------------|--------------------------|
| Form_Activate | master..sysprocesses, tbl_User | [CMXsrv_cmx_busc_suc_usu](#cmxsrv_cmx_busc_suc_usu) |
| Form_Activate | ACMXPAIS, COR, tbl_User, CCE, ACMXSUCSAL, CLN | [CMXsrv_expcce_lee_cce](#cmxsrv_expcce_lee_cce) |
| Form_Activate | ACMXFORPAG, ACMXVIATPT, ACMXMAXCCE, ACMXCNFCCE, ACMXMONEDA, ACMXCLACOM, CCE, ACMXRCBCCE | [CMXsrv_expcce_trd_cce](#cmxsrv_expcce_trd_cce) |
| MCCEANL_CLICK | CCE | [CMXsrv_expcce_anl_cce](#cmxsrv_expcce_anl_cce) |
| Mccectb_click | CCE | [CMXsrv_expcce_ctb_ing](#cmxsrv_expcce_ctb_ing) |
| Mccedel_Click | COD, ACCECTP, ACCECND, CCB, COM, ACCEBCO, DCC, CCE, EVC, ACCEDCC, AFIN | [CMXsrv_expcce_del_cce](#cmxsrv_expcce_del_cce) |
| MCCEVAL_CLICK | ACMXPAIS, COR, ACMXPRMGRL, CCE_ADI, DCC, tbl_User, CCE, warnmsg, ACMXSUCSAL, COL | [CMXsrv_expcce_val_cce](#cmxsrv_expcce_val_cce) |
| Mmt730_Click | switxt, switxt1 | [CMXsrv_expcce_swf_sel](#cmxsrv_expcce_swf_sel) |
| Mmt730Ing_Click | switxt, switxt1 | [CMXsrv_expcce_swf_sel](#cmxsrv_expcce_swf_sel) |
| Aceptar_Click | CCB, ACCEBCO, ACCECRSE, CRSE, CCE | [CMXsrv_expcce_grb_bco](#cmxsrv_expcce_grb_bco) |
| fld_cce_bco_avs_LostFocus | ACMXPAIS, COR | [CMXsrv_expcce_lee_cor](#cmxsrv_expcce_lee_cor) |
| fld_cce_bco_orig_LostFocus | ACMXPAIS, COR | [CMXsrv_expcce_lee_cor](#cmxsrv_expcce_lee_cor) |
| fld_cce_cod_ems_LostFocus | ACMXPAIS, COR | [CMXsrv_expcce_lee_cor](#cmxsrv_expcce_lee_cor) |
| fld_cce_cod_rmb_LostFocus | ACMXPAIS, COR | [CMXsrv_expcce_lee_cor](#cmxsrv_expcce_lee_cor) |
| Form_Activate | COR, CCB, ACMXSUCSAL, ACCEBCO, CRSE, CCE, ACMXPAIS | [CMXsrv_expcce_lee_bco](#cmxsrv_expcce_lee_bco) |
| Aceptar_Click | ACCECTP, CCE | [CMXsrv_expcce_grb_ctp](#cmxsrv_expcce_grb_ctp) |
| fld_cce_cod_bn1_LostFocus | CLN | [CMXsrv_expcce_lee_cln](#cmxsrv_expcce_lee_cln) |
| fld_cce_cod_bn2_LostFocus | CLN | [CMXsrv_expcce_lee_cln](#cmxsrv_expcce_lee_cln) |
| Form_Activate | ACCECTP, ACMXPAIS, CLN, CCE | [CMXsrv_expcce_lee_ctp](#cmxsrv_expcce_lee_ctp) |
| Aceptar_Click | CCE | [CMXsrv_expcce_cre_cce](#cmxsrv_expcce_cre_cce) |
| Aceptar_Click | CCB, ACCEBCO, ACCECRSE, CRSE, CCE | [CMXsrv_expcce_grb_bco](#cmxsrv_expcce_grb_bco) |
| Aceptar_Click | ACCECTP, CCE | [CMXsrv_expcce_grb_ctp](#cmxsrv_expcce_grb_ctp) |
| Aceptar_Click | ACMXPAIS, DCC, CCE | [CMXsrv_expcce_gen_dcc](#cmxsrv_expcce_gen_dcc) |
| Aceptar_Click | CCE_ADI, ACCECRSE, CRSE, CCE, ACCE_ADI, ACCECND | [CMXsrv_expcce_grb_cnd](#cmxsrv_expcce_grb_cnd) |
| fld_cce_fec_vto_LostFocus | ACMXFERIADO | [CMXsrv_util_det_habil](#cmxsrv_util_det_habil) |
| Form_Activate | CCE_ADI, ACCECRSE, CRSE, CCE, ACCE_ADI, ACCECND | [CMXsrv_expcce_lee_cnd](#cmxsrv_expcce_lee_cnd) |
| Form_Activate | ACMXFORPAG, ACMXVIATPT, ACMXMAXCCE, ACMXCNFCCE, ACMXMONEDA, CCE, ACMXCLACOM, ACMXFDESDE, ACMXRCBCCE, ACCECND | [CMXsrv_expcce_trd_cnd](#cmxsrv_expcce_trd_cnd) |
| ELIMINAR_Click | DCC, CCE, ACCEDCC | [CMXsrv_expcce_del_dcc](#cmxsrv_expcce_del_dcc) |
| Form_Activate | DCC, CCE, ACCEDCC | [CMXsrv_expcce_bus_dcc](#cmxsrv_expcce_bus_dcc) |
| Aceptar_Click | DCC, CCE, ACCEDCC | [CMXsrv_expcce_grb_dcc](#cmxsrv_expcce_grb_dcc) |
| Form_Activate | DCC, CCE, ACCEDCC | [CMXsrv_expcce_lee_dcc](#cmxsrv_expcce_lee_dcc) |
| Aceptar_Click | ACMXPAIS, COR, tbl_User, CCE, ACMXSUCSAL, CLN | [CMXsrv_expcce_lee_cce](#cmxsrv_expcce_lee_cce) |
| buscar_Click | CCE | [CMXsrv_expcce_bus_cce](#cmxsrv_expcce_bus_cce) |
| fld_aux_cod_bn1_lostfocus | CLN | [CMXsrv_expcce_lee_cln](#cmxsrv_expcce_lee_cln) |
| proximo_Click | CCE | [CMXsrv_expcce_bus_cce](#cmxsrv_expcce_bus_cce) |
| Aceptar_Click | COR, ACCECTP, ACCEBCO, CCE_ADI, ACCECRSE, DAC, DCC, CRSE, CCE, ACCE_ADI, NGE, COL, ACCEDCC, ACCECND | [CMXsrv_expcce_mdf_cce](#cmxsrv_expcce_mdf_cce) |
| Cancelar_Click | ACCECTP, ACCEBCO, ACCEDCC, ACCECND | [CMXsrv_expcce_can_mdf](#cmxsrv_expcce_can_mdf) |
| fld_cce_cod_bn1_LostFocus | CLN | [CMXsrv_expcce_lee_cln](#cmxsrv_expcce_lee_cln) |
| fld_cce_cod_ems_LostFocus | ACMXPAIS, COR | [CMXsrv_expcce_lee_cor](#cmxsrv_expcce_lee_cor) |
| Form_Activate | ACMXSUCSAL, COR, CCE, CLN | [CMXsrv_expcce_lee_mdf](#cmxsrv_expcce_lee_mdf) |
| Aceptar_Click | COR, CCE, CLN | [CMXsrv_expcce_cnf_cce](#cmxsrv_expcce_cnf_cce) |
| Aceptar_Click | AFIN | [CMXsrv_expcce_grb_afin](#cmxsrv_expcce_grb_afin) |
| Form_Activate | ACMXFORPAG, COR, ACMXMONEDA, CCE, CLN | [CMXsrv_expcce_lee_cnf](#cmxsrv_expcce_lee_cnf) |
| Form_Activate | CCE, AFIN | [CMXsrv_expcce_lee_afin](#cmxsrv_expcce_lee_afin) |
| Aceptar_Click | COR, CCE | [CMXsrv_expcce_trp_cce](#cmxsrv_expcce_trp_cce) |
| fld_cce_bco_dst_LostFocus | ACMXPAIS, COR | [CMXsrv_expcce_lee_cor](#cmxsrv_expcce_lee_cor) |
| Form_Activate | CCE | [CMXsrv_expcce_lee_trp](#cmxsrv_expcce_lee_trp) |
| Form_Activate | EVC, CCE, NGE | [CMXsrv_expcce_bus_evc](#cmxsrv_expcce_bus_evc) |
| proximo_Click | EVC, CCE, NGE | [CMXsrv_expcce_bus_evc](#cmxsrv_expcce_bus_evc) |
| reversar_Click | COR, TAS, ACMXIMPUES, LTR, DCN, EVC, RET, CUO, EVO, TRSD, DSN, CCE, NGE, PUCBCX10, COD, CNO, COM, DAC, EVE, CAN, COL, AFIN, ORG, DTN, EVR | [CMXsrv_expcce_rev_cce](#cmxsrv_expcce_rev_cce) |
| Form_Activate | ACMXFORPAG, ACMXMONEDA, CCE, NGE, EVC, ACMXSUCSAL, ACMXTIPEVE | [CMXsrv_expcce_lee_evc](#cmxsrv_expcce_lee_evc) |
| aceptar_Click | ACMXFORPAG, COR, CCB, NGEB, ACMXMONEDA, LTR, CCE, DCN, NGE, ACMXPAISES, CLN | [CMXsrv_expcce_avs_rem1](#cmxsrv_expcce_avs_rem1) |
| buscar_Click | ACMXPLAZAS, comex..ACMXPLAZAS | [CMXsrv_busc_plz](#cmxsrv_busc_plz) |
| fld_cor_cod_plz_Lostfocus | ACMXPLAZAS | [CMXsrv_lee_plz](#cmxsrv_lee_plz) |
| proximos_Click | ACMXPLAZAS, comex..ACMXPLAZAS | [CMXsrv_busc_plz](#cmxsrv_busc_plz) |
| buscar_Click | ACMXPAIS | [CMXsrv_cor_busc_pais](#cmxsrv_cor_busc_pais) |
| fld_cor_cod_pais_LostFocus | comex..ACMXPAIS | [CMXsrv_cor_lee_pais](#cmxsrv_cor_lee_pais) |
| proximos_Click | ACMXPAIS | [CMXsrv_cor_busc_pais](#cmxsrv_cor_busc_pais) |
| Aceptar_Click | ACMXPAIS, COR | [CMXsrv_expcce_lee_cor](#cmxsrv_expcce_lee_cor) |
| buscar_Click | COR | [CMXsrv_expcce_bus_cor](#cmxsrv_expcce_bus_cor) |
| Command1_Click | COR | [CMXsrv_expcce_bus_cor](#cmxsrv_expcce_bus_cor) |
| proximos_Click | COR | [CMXsrv_expcce_bus_cor](#cmxsrv_expcce_bus_cor) |
| enviar_Click | switxt, switxt1 | [CMXsrv_expcce_swf_sel](#cmxsrv_expcce_swf_sel) |
| Form_Load |  | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |

---

## expdex
<a name="expdex" ></a>

| **Segmento** | **Tabla Referenciada** | **Procedimiento Almacenado** |
|-------------|----------------------|--------------------------|
| form_activate | ACMXPRMGRL | [CMXsrv_expcbe_lee_prm](#cmxsrv_expcbe_lee_prm) |
| form_activate | ACMXSUCSAL, DEX, CLN, ACMXADUANA | [CMXsrv_dex_lee_dex](#cmxsrv_dex_lee_dex) |
| Mdexeli_Click | DEX | [CMXsrv_dex_eli_dex](#cmxsrv_dex_eli_dex) |
| ACEPTAR_Click | DEX | [CMXsrv_dex_act_dex](#cmxsrv_dex_act_dex) |
| fld_dex_dia_plz_max_LostFocus |  | [CMXsrv_expdex_cal_fec](#cmxsrv_expdex_cal_fec) |
| fld_dex_fec_acep_LostFocus |  | [CMXsrv_expdex_cal_fec](#cmxsrv_expdex_cal_fec) |
| fld_dex_rut_exp_LostFocus | CLN | [CMXsrv_dex_lee_cli](#cmxsrv_dex_lee_cli) |
| FORM_Load | ACMXSUCSAL, DEX, CLN, ACMXADUANA | [CMXsrv_dex_lee_dex](#cmxsrv_dex_lee_dex) |
| Buscar_Click | DEX | [CMXsrv_dex_bus_dex](#cmxsrv_dex_bus_dex) |
| fld_dex_rut_exp_LostFocus | CLN | [CMXsrv_dex_lee_cli](#cmxsrv_dex_lee_cli) |
| FORM_Load |  | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |
| ACEPTAR_Click | DEX | [CMXsrv_dex_act_dex](#cmxsrv_dex_act_dex) |
| fld_dex_rut_exp_LostFocus | CLN | [CMXsrv_dex_lee_cli](#cmxsrv_dex_lee_cli) |
| FORM_Load | ACMXSUCSAL, DEX, CLN, ACMXADUANA | [CMXsrv_dex_lee_dex](#cmxsrv_dex_lee_dex) |
| COMELIMINAR_Click | DEX | [CMXsrv_dex_eli_dex](#cmxsrv_dex_eli_dex) |
| Form_Activate | ACMXSUCSAL, DEX, CLN, ACMXADUANA | [CMXsrv_dex_lee_dex](#cmxsrv_dex_lee_dex) |

---

## EXPNEG
<a name="expneg" ></a>

| **Segmento** | **Tabla Referenciada** | **Procedimiento Almacenado** |
|-------------|----------------------|--------------------------|
| Form_Activate | EVZ, CBE | [CMXsrv_expcbe_bus_evz](#cmxsrv_expcbe_bus_evz) |
| Proximo_Click | EVZ, CBE | [CMXsrv_expcbe_bus_evz](#cmxsrv_expcbe_bus_evz) |
| Reversar_Click | EVL, ACMXDESEMB, COR, ORG, ACMXIMPUES, ACMXPRMGRL, EVZ, CBE, TRSD, ACMXPRMEXP, COM, EVR, CTZ, DTN, OPREC, RET, PUCBCX10 | [CMXsrv_expcbe_rev_cbe](#cmxsrv_expcbe_rev_cbe) |
| Form_Activate | ACMXDESEMB, COR, ACMXPGOCBE, EVZ, CBE, ACMXMONEDA, ACMXTIPEVE, ACMXSUCSAL | [CMXsrv_expcbe_lee_evz](#cmxsrv_expcbe_lee_evz) |
| Form_Activate | ACMXMONEDA, CCE, ACMXFORPAG | [CMXsrv_expcce_lee_bas](#cmxsrv_expcce_lee_bas) |
| Form_Activate | COR, ACMXVIATPT, ACMXSUCSAL, ACMXDISNEG, ACMXMONEDA, ACMXCLACOM, NGE, ACMXPAIS, CLN, ACMXTPONEG | [CMXsrv_expcce_lee_neg](#cmxsrv_expcce_lee_neg) |
| Mccealznge_click | COL, CCE, NGE | [CMXsrv_expcce_alz_dis](#cmxsrv_expcce_alz_dis) |
| Mcceanlnge_click | CCE, NGE | [CMXsrv_expcce_anl_neg](#cmxsrv_expcce_anl_neg) |
| Mccectbnge_Click | COR, LTR, CCE, NGE, AFIN | [CMXsrv_expcce_ctb_neg](#cmxsrv_expcce_ctb_neg) |
| Mccedelnge_Click | CRSN, COD, COM, NGEB, LTR, DSN, CCE, DCN, NGE, EVC, AFIN | [CMXsrv_expcce_del_neg](#cmxsrv_expcce_del_neg) |
| Mccevalnge_click | NGEB, LTR, DCC, warnmsg, CCE, DCN, NGE, COL, AFIN | [CMXsrv_expcce_val_neg](#cmxsrv_expcce_val_neg) |
| Mtel742_Click | switxt, switxt1 | [CMXsrv_expcce_swf_sel](#cmxsrv_expcce_swf_sel) |
| Form_Activate | EVC, CCE, NGE | [CMXsrv_expcce_bus_evc](#cmxsrv_expcce_bus_evc) |
| Proximo_Click | EVC, CCE, NGE | [CMXsrv_expcce_bus_evc](#cmxsrv_expcce_bus_evc) |
| Reversar_Click | COR, TAS, ACMXIMPUES, LTR, DCN, EVC, RET, CUO, EVO, TRSD, DSN, CCE, NGE, PUCBCX10, COD, CNO, COM, DAC, EVE, CAN, COL, AFIN, ORG, DTN, EVR | [CMXsrv_expcce_rev_cce](#cmxsrv_expcce_rev_cce) |
| Form_Activate | ACMXFORPAG, ACMXMONEDA, CCE, NGE, EVC, ACMXSUCSAL, ACMXTIPEVE | [CMXsrv_expcce_lee_evc](#cmxsrv_expcce_lee_evc) |
| aceptar_Click | CRSN, CCE, NGEB, NGE | [CMXsrv_expcce_grb_neg](#cmxsrv_expcce_grb_neg) |
| aceptar_Click | DCC, CCE, DCN, NGE | [CMXsrv_expcce_gen_dcn](#cmxsrv_expcce_gen_dcn) |
| aceptar_Click | AFIN | [CMXsrv_expcce_grb_afin](#cmxsrv_expcce_grb_afin) |
| fld_cce_cod_exp_nge_LostFocus | CLN | [CMXsrv_expcce_lee_cln](#cmxsrv_expcce_lee_cln) |
| fld_cce_cod_pag_nge_LostFocus | ACMXPAIS, COR | [CMXsrv_expcce_lee_cor](#cmxsrv_expcce_lee_cor) |
| fld_cce_cod_rmb_nge_LostFocus | ACMXPAIS, COR | [CMXsrv_expcce_lee_cor](#cmxsrv_expcce_lee_cor) |
| fld_cce_ins_rem1_nge_GotFocus | COR, ACMXCRDREMTXT, ACMXMONEDA, CCE, NGE, ACMXPAISES, CCO | [CMXsrv_expcce_avs_rem5](#cmxsrv_expcce_avs_rem5) |
| Form_Load | COR, CRSN, NGEB, CCE, NGE, ACMXPAIS, CLN | [CMXsrv_expcce_lee_nge](#cmxsrv_expcce_lee_nge) |
| Form_Load | ACMXVIATPT, ACMXRCBCCE, ACMXMONEDA, ACMXCLACOM, NGE, ACMXTPONEG | [CMXsrv_expcce_trd_nge](#cmxsrv_expcce_trd_nge) |
| Form_Load | ACMXPAIS, COR, ACMXVIATPT, CCB, ACMXMONEDA, CRSE, CCE, ACMXCLACOM, NGE, ACMXSUCSAL, CLN, ACMXTPONEG | [CMXsrv_expcce_ini_neg](#cmxsrv_expcce_ini_neg) |
| Form_Load | CCE, AFIN | [CMXsrv_expcce_lee_afin](#cmxsrv_expcce_lee_afin) |
| lee_bco | ACMXPAIS, COR | [CMXsrv_expcce_lee_cor](#cmxsrv_expcce_lee_cor) |
| ELIMINAR_Click | CCE, DCN, NGE | [CMXsrv_expcce_del_dcn](#cmxsrv_expcce_del_dcn) |
| Form_Activate | DCN, NGE | [CMXsrv_expcce_bus_dcn](#cmxsrv_expcce_bus_dcn) |
| Aceptar_Click | CCE, DCN, NGE | [CMXsrv_expcce_grb_dcn](#cmxsrv_expcce_grb_dcn) |
| Form_Load | DCC, DCN, NGE | [CMXsrv_expcce_lee_dcn](#cmxsrv_expcce_lee_dcn) |
| ELIMINAR_Click | LTR, CCE, NGE | [CMXsrv_expcce_del_ltr](#cmxsrv_expcce_del_ltr) |
| Form_Activate | LTR, NGE | [CMXsrv_expcce_bus_ltr](#cmxsrv_expcce_bus_ltr) |
| Aceptar_Click | LTR, CCE, NGE | [CMXsrv_expcce_grb_ltr](#cmxsrv_expcce_grb_ltr) |
| Form_Load | LTR, CCE, NGE | [CMXsrv_expcce_lee_ltr](#cmxsrv_expcce_lee_ltr) |
| ELIMINAR_Click | DSN, CCE, NGE | [CMXsrv_expcce_del_dsn](#cmxsrv_expcce_del_dsn) |
| Form_Activate | DCC, DSN, CCE, DCN, NGE | [CMXsrv_expcce_gen_dsn](#cmxsrv_expcce_gen_dsn) |
| Form_Activate | DSN, NGE | [CMXsrv_expcce_bus_dsn](#cmxsrv_expcce_bus_dsn) |
| Salir_Click | DSN, CCE, NGE | [CMXsrv_expcce_chk_dsn](#cmxsrv_expcce_chk_dsn) |
| Aceptar_Click | DSN, CCE, NGE | [CMXsrv_expcce_grb_dsn](#cmxsrv_expcce_grb_dsn) |
| Form_Load | DSN, NGE | [CMXsrv_expcce_lee_dsn](#cmxsrv_expcce_lee_dsn) |
| buscar_Click | CCE, NGE | [CMXsrv_expcce_bus_neg](#cmxsrv_expcce_bus_neg) |
| Proximas_Click | CCE, NGE | [CMXsrv_expcce_bus_neg](#cmxsrv_expcce_bus_neg) |
| aceptar_Click | ACMXDESEMB, COR, vig_cmx, ACMXIMPUES, COD, ACMXPRMEXP, COM, CCE, tbl_User, NGE, CLN, RET | [CMXsrv_expcce_pgo_neg](#cmxsrv_expcce_pgo_neg) |
| aceptar_Click | AFIN | [CMXsrv_expcce_grb_afin](#cmxsrv_expcce_grb_afin) |
| fld_cce_cod_exp_nge_LostFocus | CLN | [CMXsrv_expcce_lee_cln](#cmxsrv_expcce_lee_cln) |
| fld_cce_cod_rmb_nge_LostFocus | ACMXPAIS, COR | [CMXsrv_expcce_lee_cor](#cmxsrv_expcce_lee_cor) |
| Form_Load | ACMXDESEMB, COR, ACMXPRMEXP, ACMXMONEDA, CCE, NGE, CLN | [CMXsrv_expcce_lee_pgo](#cmxsrv_expcce_lee_pgo) |
| Form_Load | CCE, AFIN | [CMXsrv_expcce_lee_afin](#cmxsrv_expcce_lee_afin) |
| lee_bco | ACMXPAIS, COR | [CMXsrv_expcce_lee_cor](#cmxsrv_expcce_lee_cor) |
| aceptar_Click |  | [CMXsrv_avi_dat_cou](#cmxsrv_avi_dat_cou) |
| aceptar_Click | COR, CRSN, NGEB, CCE, NGE, ACMXPAIS, CLN | [CMXsrv_expcce_lee_nge](#cmxsrv_expcce_lee_nge) |
| aceptar_Click | ACMXFORPAG, COR, CCB, NGEB, ACMXMONEDA, LTR, CCE, DCN, NGE, ACMXPAISES, CLN | [CMXsrv_expcce_avs_rem1](#cmxsrv_expcce_avs_rem1) |
| aceptar_Click | LTR, NGE | [CMXsrv_expcce_avs_rem3](#cmxsrv_expcce_avs_rem3) |
| imprime_esp | DCN | [CMXsrv_expcce_avs_rem2](#cmxsrv_expcce_avs_rem2) |
| imprime_esp | DSN | [CMXsrv_expcce_avs_rem4](#cmxsrv_expcce_avs_rem4) |
| imprime_esp | ACMXREMFESPMSG, ACMXREMFINGMSG | [CMXsrv_expcbe_avs_rem4](#cmxsrv_expcbe_avs_rem4) |
| imprime_ing | DCN | [CMXsrv_expcce_avs_rem2](#cmxsrv_expcce_avs_rem2) |
| imprime_ing | DSN | [CMXsrv_expcce_avs_rem4](#cmxsrv_expcce_avs_rem4) |
| imprime_ing | ACMXREMFESPMSG, ACMXREMFINGMSG | [CMXsrv_expcbe_avs_rem4](#cmxsrv_expcbe_avs_rem4) |
| aceptar_Click | ACMXPAIS, COR | [CMXsrv_expcce_lee_cor](#cmxsrv_expcce_lee_cor) |
| buscar_Click | COR | [CMXsrv_expcce_bus_cor](#cmxsrv_expcce_bus_cor) |
| proximos_Click | COR | [CMXsrv_expcce_bus_cor](#cmxsrv_expcce_bus_cor) |
| enviar_Click | switxt, switxt1 | [CMXsrv_expcce_swf_sel](#cmxsrv_expcce_swf_sel) |
| Form_Load |  | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |

---

## expret
<a name="expret" ></a>

| **Segmento** | **Tabla Referenciada** | **Procedimiento Almacenado** |
|-------------|----------------------|--------------------------|
| buscar_Click | ACMXPLAZAS, comex..ACMXPLAZAS | [CMXsrv_busc_plz](#cmxsrv_busc_plz) |
| fld_cor_cod_plz_Lostfocus | ACMXPLAZAS | [CMXsrv_lee_plz](#cmxsrv_lee_plz) |
| proximos_Click | ACMXPLAZAS, comex..ACMXPLAZAS | [CMXsrv_busc_plz](#cmxsrv_busc_plz) |
| buscar_Click | ACMXPAIS | [CMXsrv_cor_busc_pais](#cmxsrv_cor_busc_pais) |
| fld_cor_cod_pais_LostFocus | comex..ACMXPAIS | [CMXsrv_cor_lee_pais](#cmxsrv_cor_lee_pais) |
| proximos_Click | ACMXPAIS | [CMXsrv_cor_busc_pais](#cmxsrv_cor_busc_pais) |
| Aceptar_Click | ACMXPAIS, COR | [CMXsrv_expcbe_lee_cor](#cmxsrv_expcbe_lee_cor) |
| buscar_Click | COR | [CMXsrv_expcbe_bus_cor](#cmxsrv_expcbe_bus_cor) |
| proximos_Click | COR | [CMXsrv_expcbe_bus_cor](#cmxsrv_expcbe_bus_cor) |
| Command2_Click | DTN, ACMXPRMEXP, switxt, switxt1 | [CMXsrv_expret_swf_sel](#cmxsrv_expret_swf_sel) |
| Form_Load |  | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |
| Form_Activate | master..sysprocesses, tbl_User | [CMXsrv_cmx_busc_suc_usu](#cmxsrv_cmx_busc_suc_usu) |
| Form_Activate | DTN, ACMXPRMEXP, ACMXMONEDA, ACMXSUCSAL, CLN, RET | [CMXsrv_expret_lee_ret](#cmxsrv_expret_lee_ret) |
| Form_Load | ACMXPRMGRL, ACMXPRMEXP | [CMXsrv_expret_lee_prm](#cmxsrv_expret_lee_prm) |
| M_cgyc_Click | ACMXDESEMB, ASND, ACMXIMPUES, ACMXPRMGRL, COM, TRSD, EVR, CLN, ACMXESPECI, RET | [CMXsrv_expret_avs_cyg1](#cmxsrv_expret_avs_cyg1) |
| M_cgyc_Click | ASND, ACMXIMPUES, ACMXPRMGRL, EVR, RET | [CMXsrv_expret_avs_cyg2](#cmxsrv_expret_avs_cyg2) |
| mavisliq_Click | DTN, ACMXMONEDA, ACMXSUCSAL, CLN, ACMXESPECI, RET | [CMXsrv_expret_avs_liq1](#cmxsrv_expret_avs_liq1) |
| mavisliq_Click | ORG, RET | [CMXsrv_expret_avs_liq2](#cmxsrv_expret_avs_liq2) |
| mavisliq_Click | DTN, ACMXPRMEXP, RET | [CMXsrv_expret_avs_liq3](#cmxsrv_expret_avs_liq3) |
| Mcbectb_Click | ACMXDESEMB, ORG, COR, ACMXIMPUES, ACMXPRMGRL, CCL, ACMXPRMEXP, ACMXMONEDAFEC, COM, tbl_User, warnmsg, DTN, CLN, RET | [CMXsrv_expret_val_ret](#cmxsrv_expret_val_ret) |
| Mcbectb_Click | DTN, ACMXMONEDAFEC, RET, ACMXPRMENL | [CMXsrv_expret_sum_dtn_mn](#cmxsrv_expret_sum_dtn_mn) |
| Mcbectb_Click | ACMXDESEMB, ASND, PLV, ACMXPRMGRL, CCL, ACMXPRMEXP, PLI, tbl_User, DTN, CLN, RET | [CMXsrv_expret_ctb_ing](#cmxsrv_expret_ctb_ing) |
| Mcbedel_Click | ORG, COD, COM, DTN, RET | [CMXsrv_expret_del_ret](#cmxsrv_expret_del_ret) |
| Mliqctb_Click | ACMXSUCSAL, ACMXMONEDA, CLN, RET | [CMXsrv_expret_avs_adm1](#cmxsrv_expret_avs_adm1) |
| Mliqctb_Click | ORG, ACMXPRMEXP, RET | [CMXsrv_expret_avs_adm2](#cmxsrv_expret_avs_adm2) |
| Mliqctb_Click | DTN, ACMXPRMEXP, RET | [CMXsrv_expret_avs_adm3](#cmxsrv_expret_avs_adm3) |
| Mvalid_Click | ACMXDESEMB, ORG, COR, ACMXIMPUES, ACMXPRMGRL, CCL, ACMXPRMEXP, ACMXMONEDAFEC, COM, tbl_User, warnmsg, DTN, CLN, RET | [CMXsrv_expret_val_ret](#cmxsrv_expret_val_ret) |
| ACEPTAR_Click | RET | [CMXsrv_expret_act_tpo_cbo](#cmxsrv_expret_act_tpo_cbo) |
| ACEPTAR_Click | ACMXDESEMB, ORG, COR, ACMXIMPUES, ACMXPRMGRL, CCL, ACMXPRMEXP, ACMXMONEDAFEC, COM, tbl_User, warnmsg, DTN, CLN, RET | [CMXsrv_expret_val_ret](#cmxsrv_expret_val_ret) |
| ACEPTAR_Click | RET | [CMXsrv_expret_cre_ret](#cmxsrv_expret_cre_ret) |
| ACEPTAR_Click | CLN, tbl_User, RET | [CMXsrv_expret_grb_det](#cmxsrv_expret_grb_det) |
| fld_ret_mon_ret_LostFocus | ACMXMONEDAFEC | [CMXsrv_expret_tpo_cbo](#cmxsrv_expret_tpo_cbo) |
| fld_ret_rut_cli_LostFocus | CLN | [CMXsrv_expret_lee_cln](#cmxsrv_expret_lee_cln) |
| Form_Load | ACMXSUCSAL, ACMXMONEDA, CLN, RET | [CMXsrv_expret_lee_det](#cmxsrv_expret_lee_det) |
| ELIMINAR_Click | ORG, RET | [CMXsrv_expret_del_org](#cmxsrv_expret_del_org) |
| Form_Activate | ORG, RET | [CMXsrv_expret_bus_org](#cmxsrv_expret_bus_org) |
| ACEPTAR_Click | ACMXDESEMB, ORG, ACMXPLNCTAN, ACMXSRVEXT, ACMXPLNCTAX, RET | [CMXsrv_expret_grb_org](#cmxsrv_expret_grb_org) |
| Form_Activate | ORG, RET | [CMXsrv_expret_mto_org](#cmxsrv_expret_mto_org) |
| Form_Activate | ACMXDESEMB, ORG, COR, ACMXTPODOC, ACMXPAIS | [CMXsrv_expret_lee_org](#cmxsrv_expret_lee_org) |
| valida_vigente | ACMXPLNCTAN, ACMXDESEMB, ACMXPLNCTAX | [CMXsrv_vig_lee_cta](#cmxsrv_vig_lee_cta) |
| ELIMINAR_Click | DTN, RET | [CMXsrv_expret_del_dtn](#cmxsrv_expret_del_dtn) |
| emitir_Click | DTN, ACMXPRMEXP, switxt, switxt1 | [CMXsrv_expret_swf_sel](#cmxsrv_expret_swf_sel) |
| Form_Activate | DTN, RET | [CMXsrv_expret_bus_dtn](#cmxsrv_expret_bus_dtn) |
| ACEPTAR_Click | ACMXDESEMB, ACMXPRMGRL, CCL, ACMXPRMEXP, DTN, RET | [CMXsrv_expret_grb_dtn](#cmxsrv_expret_grb_dtn) |
| fld_ret_cod_ben_LostFocus | CLN | [CMXsrv_expret_lee_cln](#cmxsrv_expret_lee_cln) |
| fld_ret_mto_arb_LostFocus | ACMXPRMGRL, ACMXMONEDA | [CMXsrv_expret_cal_arb](#cmxsrv_expret_cal_arb) |
| fld_ret_mto_ben_LostFocus | ACMXPRMGRL, ACMXMONEDA | [CMXsrv_expret_cal_arb](#cmxsrv_expret_cal_arb) |
| fld_ret_par_ben_LostFocus | ACMXPRMGRL, ACMXMONEDA | [CMXsrv_expret_cal_arb](#cmxsrv_expret_cal_arb) |
| Form_Activate | DTN, COM, RET, ACMXIMPUES | [CMXsrv_expret_mto_dtn](#cmxsrv_expret_mto_dtn) |
| Form_Load | ACMXPAIS, ACMXDESEMB, COR, DTN, ACMXMONEDA, APUCCODOPECMB, ACMXSUCSAL | [CMXsrv_expret_lee_dtn](#cmxsrv_expret_lee_dtn) |
| Form_Load | CLN | [CMXsrv_expret_lee_cln](#cmxsrv_expret_lee_cln) |
| buscar_Click | RET | [CMXsrv_expret_bus_ret](#cmxsrv_expret_bus_ret) |
| fld_ret_rut_cli_LostFocus | CLN | [CMXsrv_expret_lee_cln](#cmxsrv_expret_lee_cln) |
| proxima_Click | RET | [CMXsrv_expret_bus_ret](#cmxsrv_expret_bus_ret) |
| Command1_Click | EVR, RET | [CMXsrv_expret_bus_evr](#cmxsrv_expret_bus_evr) |
| Form_Activate | EVR, RET | [CMXsrv_expret_bus_evr](#cmxsrv_expret_bus_evr) |
| proximo_Click | EVR, RET | [CMXsrv_expret_bus_evr](#cmxsrv_expret_bus_evr) |
| reversar_Click | ORG, DTN, PLV, ACMXPRMEXP, PLI, TRSD, EVR, RET | [CMXsrv_expret_rev_ret](#cmxsrv_expret_rev_ret) |
| Form_Load | ACMXTIPEVE, EVR, ACMXSUCSAL | [CMXsrv_expret_lee_evr](#cmxsrv_expret_lee_evr) |

---

## ADMIN
<a name="admin" ></a>

| **Segmento** | **Tabla Referenciada** | **Procedimiento Almacenado** |
|-------------|----------------------|--------------------------|
| COMMAND4_Click | TIP | [CMXsrv_finadm_imod_desti](#cmxsrv_finadm_imod_desti) |
| Form_Load | TIP | [CMXsrv_finadm_cons_dtip](#cmxsrv_finadm_cons_dtip) |
| Command1_Click | TIP | [CMXsrv_finadm_imod_ectb](#cmxsrv_finadm_imod_ectb) |
| Command2_Click | TIP, TIP_CTA | [CMXsrv_finadm_eli_tipop](#cmxsrv_finadm_eli_tipop) |
| Form_Load | TIP | [CMXsrv_finadm_cons_ectb](#cmxsrv_finadm_cons_ectb) |
| COMMAND3_Click | TIP, TIP_CTA | [CMXsrv_finadm_eli_tipop](#cmxsrv_finadm_eli_tipop) |
| COMMAND4_Click | TIP | [CMXsrv_finadm_imod_itip](#cmxsrv_finadm_imod_itip) |
| Form_Load | TIP | [CMXsrv_finadm_cons_itip](#cmxsrv_finadm_cons_itip) |
| Form_Activate | TIP, ACMXPLAZO, ACMXPROCMX, ACMXMB1 | [CMXsrv_finadm_lee_tipop](#cmxsrv_finadm_lee_tipop) |
| Form_Load |  | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |
| Mdel_Click | TIP, TIP_CTA | [CMXsrv_finadm_eli_tipop](#cmxsrv_finadm_eli_tipop) |
| Mval_Click | APEPROR, TIP, TAS, CUO, ACMXPLNCTAN, ACMXMONEDAFEC, PANCTL, ACLNCBCABCI, ACMXPLNCTAX, TIP_CTA, ACMXMONEDA, warnmsg, EVE, ACMXSUCSAL, PANVTO, ACMXINTEREFEC, COL, PANMOR | [CMXsrv_finadm_val_tipop](#cmxsrv_finadm_val_tipop) |
| buscar_Click | TIP | [CMXsrv_finadm_bus_tipope](#cmxsrv_finadm_bus_tipope) |
| proximas_Click | TIP | [CMXsrv_finadm_bus_tipope](#cmxsrv_finadm_bus_tipope) |

---

## COL_NEG
<a name="col_neg" ></a>

| **Segmento** | **Tabla Referenciada** | **Procedimiento Almacenado** |
|-------------|----------------------|--------------------------|
| CANCELAR_Click | CRD | [CMXsrv_busc_tip_tas](#cmxsrv_busc_tip_tas) |
| ELIMINAR_Click | CUO_REN, COL, CUO | [CMXsrv_fincol_ecuo](#cmxsrv_fincol_ecuo) |
| Form_Activate | CUO_REN, COL_REN, COL, CUO | [CMXsrv_fincol_cons_plnpa](#cmxsrv_fincol_cons_plnpa) |
| Form_Load | TAS | [CMXsrv_pertas_val_display](#cmxsrv_pertas_val_display) |
| ELIMINAR_Click | DAC, AVAL, AVAL_REN, COL | [CMXsrv_fincol_eava](#cmxsrv_fincol_eava) |
| Form_Activate | CRDCLON, AVAL, AVAL_REN, COL | [CMXsrv_fincol_cons_aval](#cmxsrv_fincol_cons_aval) |
| ingresar_Click | AVAL, AVAL_REN, CLN, COL | [CMXsrv_fincol_iava](#cmxsrv_fincol_iava) |
| Form_Activate | CAN, COL | [CMXsrv_fincol_cons_pag](#cmxsrv_fincol_cons_pag) |
| proximos_Click | CAN, COL | [CMXsrv_fincol_cons_pag](#cmxsrv_fincol_cons_pag) |
| Form_Activate | CAN, EVE | [CMXsrv_fincol_trae_det_pag](#cmxsrv_fincol_trae_det_pag) |
| Form_Activate | EVE, COL | [CMXsrv_fincol_cons_pror](#cmxsrv_fincol_cons_pror) |
| Form_Activate | EVE, COL | [CMXsrv_fincol_cons_eve](#cmxsrv_fincol_cons_eve) |
| Aceptar_Click | ACMXPAIS, COR | [CMXsrv_icrd_lee_bco_swf](#cmxsrv_icrd_lee_bco_swf) |
| buscar_Click | COR | [CMXsrv_icrd_busc_bco](#cmxsrv_icrd_busc_bco) |
| proximo_Click | COR | [CMXsrv_icrd_busc_bco](#cmxsrv_icrd_busc_bco) |
| Aceptar_Click | TIP, comex..ACMXINTEREFEC, COR, CRD, CUO, OBL, NEG, NEG_ADI, DAC, ACMXINTERE, ACMXMONEDA, ACMXINTEREFEC, AVAL, MYC, COL, CTO | [CMXsrv_fincol_vtocre_prov](#cmxsrv_fincol_vtocre_prov) |
| Form_Load | TIP, CRD, CNEG, NEG, COL | [CMXsrv_fincol_prec_vtocre](#cmxsrv_fincol_prec_vtocre) |
| buscar_Click | COR | [CMXsrv_icrd_bus_lcr_bco](#cmxsrv_icrd_bus_lcr_bco) |
| proximo_Click | COR | [CMXsrv_icrd_bus_lcr_bco](#cmxsrv_icrd_bus_lcr_bco) |
| Form_Load |  | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |
| Form_Load | ACMXFECPRO | [CMXsrv_lee_fpro](#cmxsrv_lee_fpro) |

---

## INGRESO
<a name="ingreso" ></a>

| **Segmento** | **Tabla Referenciada** | **Procedimiento Almacenado** |
|-------------|----------------------|--------------------------|
| cancelar_Click | COL_REN, TIP, TAS, TAS_REN, EVE_REN, DAC_REN, ITA, CUO_REN, AVAL_REN, EVE, CAN_REN, COL | [CMXsrv_fincol_ren_fin](#cmxsrv_fincol_ren_fin) |
| ELIMINAR_Click | CUO_REN, COL, CUO | [CMXsrv_fincol_ecuo](#cmxsrv_fincol_ecuo) |
| form_activate | CUO_REN, COL_REN, COL, CUO | [CMXsrv_fincol_cons_plnpa](#cmxsrv_fincol_cons_plnpa) |
| cancelar_Click | COL_REN, TIP, TAS, TAS_REN, EVE_REN, DAC_REN, ITA, CUO_REN, AVAL_REN, EVE, CAN_REN, COL | [CMXsrv_fincol_ren_fin](#cmxsrv_fincol_ren_fin) |
| ELIMINAR_Click | DAC, AVAL, AVAL_REN, COL | [CMXsrv_fincol_eava](#cmxsrv_fincol_eava) |
| form_activate | CRDCLON, AVAL, AVAL_REN, COL | [CMXsrv_fincol_cons_aval](#cmxsrv_fincol_cons_aval) |
| aceptar_Click | TIP, CUO, OBL, CTR, CLN, COL, CTO | [CMXsrv_fincol_gmod_ctr](#cmxsrv_fincol_gmod_ctr) |
| busca_bco | ACMXPAIS, COR | [CMXsrv_icrd_lee_bco_swf](#cmxsrv_icrd_lee_bco_swf) |
| fld_obl_bco_acr_LostFocus | COR | [CMXsrv_fincol_lee_bco](#cmxsrv_fincol_lee_bco) |
| fld_obl_rut_acr_LostFocus | CLN | [CMXsrv_fincol_lee_cln](#cmxsrv_fincol_lee_cln) |
| form_activate | OBL, CTR | [CMXsrv_fincol_cons_ctr](#cmxsrv_fincol_cons_ctr) |
| aceptar_Click | TIP, ACMXDESEMB, CUO, COD, vig_cmx, COL_ADI, ACMXPRMGRL, OBL, COM, MYC, ACMXMONEDA, LIB, OPE_BCI, CLN, COL, CCO | [CMXsrv_fincol_ctb_oto](#cmxsrv_fincol_ctb_oto) |
| Avi5_Click | ACMXDESEMB, ASND, EVO, CRD, CNO, OBL, CUO, TRSD, NEG, COM, EVE, ACMXTIPEVE, CAN, COL | [CMXsrv_icrd_dat_liq_ope](#cmxsrv_icrd_dat_liq_ope) |
| form_activate | COR, TAS, NEG_ADI, ACMXINTERE, TIP, CUO, CCL, ACMXFINVER, ACMXAPROBAC, COL_ADI, ACMXACTIVIDA, ACMXINTEREFEC, AVAL, ACMXSUCSAL, CLN, comex..ACMXINTEREFEC, COM, ACMXMONEDA, EVE, tbl_User, COL | [CMXsrv_fincol_lee_col](#cmxsrv_fincol_lee_col) |
| Form_Load | ACMXFECPRO | [CMXsrv_lee_fpro](#cmxsrv_lee_fpro) |
| MCOLCOMI_CLICK | TIP, COL | [CMXsrv_busc_cod_ope](#cmxsrv_busc_cod_ope) |
| MCOLCOMI_CLICK | COL | [CMXsrv_col_trae_num_ope](#cmxsrv_col_trae_num_ope) |
| MCOLCONTOTOR_CLICK | TIP, COL | [CMXsrv_busc_cod_ope](#cmxsrv_busc_cod_ope) |
| MCOLCONTOTOR_CLICK | COL | [CMXsrv_col_trae_num_ope](#cmxsrv_col_trae_num_ope) |
| MCOLCONTOTOR_CLICK | TIP, ACMXDESEMB, CUO, COD, vig_cmx, COL_ADI, ACMXPRMGRL, OBL, COM, MYC, ACMXMONEDA, LIB, OPE_BCI, CLN, COL, CCO | [CMXsrv_fincol_ctb_oto](#cmxsrv_fincol_ctb_oto) |
| MCOLELI_CLICK | COL_REN, COL_ADI, COM, TAS_REN, DAC_REN, EVE_REN, DAC, CUO_REN, AVAL_REN, LIB, CAN_REN, COL | [CMXsrv_fincol_eli_col](#cmxsrv_fincol_eli_col) |
| valida | TIP, COL, warnmsg | [CMXsrv_fincol_val_col](#cmxsrv_fincol_val_col) |
| aceptar_Click | COR, TAS, NEG_ADI, ACMXINTERE, TIP, CUO, CCL, ACMXFINVER, ACMXAPROBAC, COL_ADI, ACMXACTIVIDA, ACMXINTEREFEC, AVAL, ACMXSUCSAL, CLN, comex..ACMXINTEREFEC, COM, ACMXMONEDA, EVE, tbl_User, COL | [CMXsrv_fincol_lee_col](#cmxsrv_fincol_lee_col) |
| buscar_Click | TIP | [CMXsrv_fincol_bsc_col](#cmxsrv_fincol_bsc_col) |
| fld_col_tip_ope_lostfocus | TIP | [CMXsrv_fincol_lee_tip](#cmxsrv_fincol_lee_tip) |
| PROXIMAS_Click | TIP | [CMXsrv_fincol_bsc_col](#cmxsrv_fincol_bsc_col) |
| ingresar_Click | AVAL, AVAL_REN, CLN, COL | [CMXsrv_fincol_iava](#cmxsrv_fincol_iava) |
| aceptar_Click | TIP, COL | [CMXsrv_busc_cod_ope](#cmxsrv_busc_cod_ope) |
| aceptar_Click | COL | [CMXsrv_col_trae_num_ope](#cmxsrv_col_trae_num_ope) |
| aceptar_Click | CLN, COL | [CMXsrv_fincol_ctb_novf](#cmxsrv_fincol_ctb_novf) |
| FLD_COL_COD_CLI_LOSTFOCUS | CLN | [CMXsrv_fincol_lee_cln](#cmxsrv_fincol_lee_cln) |
| FLD_COL_RUT_DEU_NOV_LostFocus | CLN | [CMXsrv_fincol_lee_cln](#cmxsrv_fincol_lee_cln) |
| form_activate | EVE, COL | [CMXsrv_fincol_cons_nov](#cmxsrv_fincol_cons_nov) |
| FLD_COL_COD_CLI_LOSTFOCUS | CLN | [CMXsrv_fincol_lee_cln](#cmxsrv_fincol_lee_cln) |
| FLD_COL_RUT_DEU_NOV_LostFocus | CLN | [CMXsrv_fincol_lee_cln](#cmxsrv_fincol_lee_cln) |
| Aceptar_Click | ACMXPAIS, COR | [CMXsrv_icrd_lee_bco_swf](#cmxsrv_icrd_lee_bco_swf) |
| buscar_Click | COR | [CMXsrv_icrd_busc_bco](#cmxsrv_icrd_busc_bco) |
| proximo_Click | COR | [CMXsrv_icrd_busc_bco](#cmxsrv_icrd_busc_bco) |
| Form_Load |  | [CMXsrv_cmx_get_codes](#cmxsrv_cmx_get_codes) |
| Form_Load |  | [CMXsrv_grl_trae_cod_bco](#cmxsrv_grl_trae_cod_bco) |

---

## MODIFIC
<a name="modific" ></a>

| **Segmento** | **Tabla Referenciada** | **Procedimiento Almacenado** |
|-------------|----------------------|--------------------------|
| Form_Activate | TAS | [CMXsrv_fincol_cons_tas](#cmxsrv_fincol_cons_tas) |
| aceptar_click | TIP, comex..ACMXMONEDAFEC, COL, CUO | [CMXsrv_fincol_efec_tras](#cmxsrv_fincol_efec_tras) |
| Form_Activate | EVE, COL | [CMXsrv_fincol_cons_trasp](#cmxsrv_fincol_cons_trasp) |
| Form_Activate | EVE, COL | [CMXsrv_fincol_cons_dtrs](#cmxsrv_fincol_cons_dtrs) |
| Form_Activate | EVE, COL | [CMXsrv_fincol_cons_eve](#cmxsrv_fincol_cons_eve) |
| Form_Load | EVE, COL | [CMXsrv_fincol_cons_deve](#cmxsrv_fincol_cons_deve) |
| aceptar_click |  | [CMXsrv_fincol_cont_gst](#cmxsrv_fincol_cont_gst) |
| Form_Activate | EVE, COL | [CMXsrv_fincol_cons_gst](#cmxsrv_fincol_cons_gst) |
| Form_Activate |  | [CMXsrv_fincol_cons_dgst](#cmxsrv_fincol_cons_dgst) |
| Form_Load | ACMXFECPRO | [CMXsrv_lee_fpro](#cmxsrv_lee_fpro) |

---

## OBLIGA
<a name="obliga" ></a>

| **Segmento** | **Tabla Referenciada** | **Procedimiento Almacenado** |
|-------------|----------------------|--------------------------|
| buscar_Click | TIP | [CMXsrv_fincol_bsc_tip](#cmxsrv_fincol_bsc_tip) |
| Proxima_Click | TIP | [CMXsrv_fincol_bsc_tip](#cmxsrv_fincol_bsc_tip) |
| proximo_Click | TIP | [CMXsrv_fincol_bsc_tip](#cmxsrv_fincol_bsc_tip) |
| buscar_Click | COR | [CMXsrv_finobl_bus_cor](#cmxsrv_finobl_bus_cor) |
| proximo_Click | COR | [CMXsrv_finobl_bus_cor](#cmxsrv_finobl_bus_cor) |
| ELIMINAR_Click | OBL, CTO | [CMXsrv_finobl_ecuo](#cmxsrv_finobl_ecuo) |
| form_activate | OBL, CTO | [CMXsrv_finobl_gpln](#cmxsrv_finobl_gpln) |
| form_activate | OBL, CTO | [CMXsrv_finobl_cons_plnpa](#cmxsrv_finobl_cons_plnpa) |
| anunctb_Click | OBL | [CMXsrv_finobl_calc_anu](#cmxsrv_finobl_calc_anu) |
| form_activate | TIP, COR, OBL, ACMXINTERE, ACMXMONEDA, ACMXSUCSAL, CLN | [CMXsrv_finobl_lee_obl](#cmxsrv_finobl_lee_obl) |
| Form_Load | ACMXFECPRO | [CMXsrv_lee_fpro](#cmxsrv_lee_fpro) |
| Mcbeanl_Click | OBL | [CMXsrv_finobl_calc_anu](#cmxsrv_finobl_calc_anu) |
| Mcbectb_Click | ACMXDESEMB, TIP, COD, OBL, CTO, CCO | [CMXsrv_finobl_ctb_oto](#cmxsrv_finobl_ctb_oto) |
| Mcbedel_Click | OBL, OBL_ADI | [CMXsrv_fincol_eli_obl](#cmxsrv_fincol_eli_obl) |
| Mobl_liq_ope_Click | ACMXDESEMB, ASND, EVO, CRD, CNO, OBL, CUO, TRSD, NEG, COM, EVE, ACMXTIPEVE, CAN, COL | [CMXsrv_icrd_dat_liq_ope](#cmxsrv_icrd_dat_liq_ope) |
| valida_error | TIP, OBL, ACMXINTERE, warnmsg, OBL_ADI | [CMXsrv_finobl_val_obl](#cmxsrv_finobl_val_obl) |
| buscar_Click | OBL | [CMXsrv_finobl_bsc_obl](#cmxsrv_finobl_bsc_obl) |
| fld_obl_tip_ope_LostFocus | TIP | [CMXsrv_fincol_lee_tip](#cmxsrv_fincol_lee_tip) |
| Proxima_Click | OBL | [CMXsrv_finobl_bsc_obl](#cmxsrv_finobl_bsc_obl) |
| contabilizar_Click | OBL, CTO, EVO | [CMXsrv_finobl_ictb_pag](#cmxsrv_finobl_ictb_pag) |
| contabilizar_Click | OBL, CTO | [CMXsrv_finobl_obt_sdocuo](#cmxsrv_finobl_obt_sdocuo) |
| form_activate | CTO | [CMXsrv_finobl_new_tas](#cmxsrv_finobl_new_tas) |
| form_activate | CNO | [CMXsrv_finobl_cons_pag](#cmxsrv_finobl_cons_pag) |
| form_activate | OBL, CTO, EVO | [CMXsrv_finobl_cons_detp](#cmxsrv_finobl_cons_detp) |
| calcular_Click | OBL | [CMXsrv_finobl_calc_pror](#cmxsrv_finobl_calc_pror) |
| form_activate | OBL, EVO | [CMXsrv_finobl_cons_pror](#cmxsrv_finobl_cons_pror) |
| form_activate | OBL, EVO | [CMXsrv_finobl_cons_dpror](#cmxsrv_finobl_cons_dpror) |
| contabilizar_Click | TIP, COR, OBL, COL, CTO | [CMXsrv_finobl_ctb_anu](#cmxsrv_finobl_ctb_anu) |
| calcular_Click | OBL | [CMXsrv_finobl_calc_anu](#cmxsrv_finobl_calc_anu) |
| form_activate | CNO, EVO | [CMXsrv_finobl_cons_anu](#cmxsrv_finobl_cons_anu) |
| form_activate | OBL, EVO | [CMXsrv_finobl_cons_mod](#cmxsrv_finobl_cons_mod) |
| form_activate | CNO, EVO | [CMXsrv_finobl_cons_dmod](#cmxsrv_finobl_cons_dmod) |
| efectuar_Click | OBL, TRSD, APRCBL, EVO | [CMXsrv_finobl_rev_eve](#cmxsrv_finobl_rev_eve) |
| form_activate | EVO | [CMXsrv_finobl_cons_eve](#cmxsrv_finobl_cons_eve) |
| form_activate | EVO | [CMXsrv_finobl_cons_deve](#cmxsrv_finobl_cons_deve) |
| ELIMINAR_Click | CTR | [CMXsrv_finobl_eli_ctr](#cmxsrv_finobl_eli_ctr) |
| form_activate | CTR | [CMXsrv_finobl_cons_ctr](#cmxsrv_finobl_cons_ctr) |
| nuevo_Click | COL, OBL, TIP, CTR | [CMXsrv_finobl_ing_ctr](#cmxsrv_finobl_ing_ctr) |
| aceptar_Click | OBL, COR | [CMXsrv_finobl_cesion_obl](#cmxsrv_finobl_cesion_obl) |
| banco_acreedor | COR | [CMXsrv_comgrl_lee_nom_cor](#cmxsrv_comgrl_lee_nom_cor) |
| fld_obl_cod_bco_acre_lostfocus | COR | [CMXsrv_comgrl_lee_nom_cor](#cmxsrv_comgrl_lee_nom_cor) |
| fld_obl_rut_acre_lostfocus | CLN | [CMXsrv_lee_cln](#cmxsrv_lee_cln) |
| form_activate | OBL | [CMXsrv_finobl_busc_acre](#cmxsrv_finobl_busc_acre) |
| Form_Load |  | [CMXsrv_cmx_get_codes](#cmxsrv_cmx_get_codes) |

---

## PAGOS
<a name="pagos" ></a>

| **Segmento** | **Tabla Referenciada** | **Procedimiento Almacenado** |
|-------------|----------------------|--------------------------|
| CALCULAR_Click | TF_PPAG, TIP, TAS, CUO, comex..ACMXMONEDA, COL_ADI, OBL, CTR, NEG_ADI, ACMXINTERE, CAN, ICR, COL | [CMXsrv_fincol_efec_calpa](#cmxsrv_fincol_efec_calpa) |
| Form_Activate | CAN, COL | [CMXsrv_fincol_cons_pag](#cmxsrv_fincol_cons_pag) |
| Form_Load | ACMXDESEMB, EVE, COL, CUO | [CMXsrv_fincol_cons_detp](#cmxsrv_fincol_cons_detp) |
| Aceptar_Click | ACMXINTERE, COL | [CMXsrv_fincol_calc_pror](#cmxsrv_fincol_calc_pror) |
| Contabilizar_Click | TAS, CRD, NEG_ADI, ACMXINTERE, TIP, CUO, OBL, CAM_TAS, ACMXPLAZO, COL_ADI, LIB, ACMXINTEREFEC, CLN, ACMXOPEIMP, CTO, de, comex..ACMXINTEREFEC, COD, COM, ACMXMONEDAFEC, EVE, CAN, COL | [CMXsrv_fincol_cont_pror](#cmxsrv_fincol_cont_pror) |
| Form_Activate | EVE, COL | [CMXsrv_fincol_cons_pror](#cmxsrv_fincol_cons_pror) |
| Form_Activate | ACMXDESEMB, EVE, COL | [CMXsrv_fincol_cons_dpror](#cmxsrv_fincol_cons_dpror) |
| Aceptar_Click | TIP, COL | [CMXsrv_busc_cod_ope](#cmxsrv_busc_cod_ope) |
| Aceptar_Click | COL | [CMXsrv_col_trae_num_ope](#cmxsrv_col_trae_num_ope) |
| Aceptar_Click | TIP, CUO, COD, OBL, TF_ENL, ENL, CAN, COL, CTO | [CMXsrv_fincol_cctb_anu](#cmxsrv_fincol_cctb_anu) |
| Form_Load | TIP, COL | [CMXsrv_fincol_calc_anu](#cmxsrv_fincol_calc_anu) |
| Form_Load | TIP, COL | [CMXsrv_busc_cod_ope](#cmxsrv_busc_cod_ope) |
| CALCULAR_Click | TIP, COL | [CMXsrv_fincol_calc_anu](#cmxsrv_fincol_calc_anu) |
| Form_Activate | ACMXDESEMB, CAN, EVE, COL | [CMXsrv_fincol_cons_anu](#cmxsrv_fincol_cons_anu) |
| Form_Activate | EVE, COL | [CMXsrv_fincol_cons_mod](#cmxsrv_fincol_cons_mod) |
| Form_Activate | CAN, EVE | [CMXsrv_fincol_cons_dmod](#cmxsrv_fincol_cons_dmod) |
| Form_Load | ACMXFECPRO | [CMXsrv_lee_fpro](#cmxsrv_lee_fpro) |
| Form_Load |  | [CMXsrv_grl_trae_cod_bco](#cmxsrv_grl_trae_cod_bco) |

---

## PGOEXT
<a name="pgoext" ></a>

| **Segmento** | **Tabla Referenciada** | **Procedimiento Almacenado** |
|-------------|----------------------|--------------------------|
| calcular_Click | TIP, CUO, comex..ACMXMONEDA, OBL, CTR, COL, CTO | [CMXsrv_fincol_cal_pext](#cmxsrv_fincol_cal_pext) |
| Contabilizar_Click | TIP, COL | [CMXsrv_busc_cod_ope](#cmxsrv_busc_cod_ope) |
| Contabilizar_Click | TIP, ACMXDESEMB, comex..ACMXINTEREFEC, TAS, CUO, COD, OBL, COL_ADI, ACMXMONEDAFEC, CTR, NEG_ADI, ACMXINTERE, EVE, ACMXINTEREFEC, COL, CTO, CCO | [CMXsrv_fincol_ctb_pext](#cmxsrv_fincol_ctb_pext) |
| calcular_Click | TIP, OBL, ACMXINTERE, ACMXMONEDA, OBL_ADI, CTO | [CMXsrv_finobl_cal_pext](#cmxsrv_finobl_cal_pext) |
| Contabilizar_Click | ACMXDESEMB, TIP, COD, OBL, ACMXMONEDAFEC, CTO, CCO | [CMXsrv_finobl_ctb_pext](#cmxsrv_finobl_ctb_pext) |
| Form_Load |  | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |
| Form_Load | ACMXFECPRO | [CMXsrv_lee_fpro](#cmxsrv_lee_fpro) |

---

## ARCOS
<a name="arcos" ></a>

| **Segmento** | **Tabla Referenciada** | **Procedimiento Almacenado** |
|-------------|----------------------|--------------------------|
| Eliminar_Click | ADI, CRD, ARC, NEG, COB, INF, COL | [CMXsrv_iarc_eli_arc](#cmxsrv_iarc_eli_arc) |
| Form_activate | ARC | [CMXsrv_iarc_busc_arc](#cmxsrv_iarc_busc_arc) |
| aceptar_click | INF | [CMXsrv_iinf_busc_inf](#cmxsrv_iinf_busc_inf) |
| aceptar_click | CRD, comex..ACMXMONEDA, ARC, NEG, CBR, ACMXMONEDAFEC, INF, COL | [CMXsrv_iarc_act_arc](#cmxsrv_iarc_act_arc) |
| Form_Load | ARC | [CMXsrv_iarc_lee_arc](#cmxsrv_iarc_lee_arc) |
| buscar_Click | ARC | [CMXsrv_iinf_busc_opr](#cmxsrv_iinf_busc_opr) |
| Form_activate | INF | [CMXsrv_iinf_lee_vlr](#cmxsrv_iinf_lee_vlr) |
| aceptar_click | CRD, comex..ACMXMONEDA, ARC, NEG, CBR, ACMXMONEDAFEC, INF, COL | [CMXsrv_iarc_act_arc](#cmxsrv_iarc_act_arc) |
| Form_activate | INF | [CMXsrv_iinf_busc_inf](#cmxsrv_iinf_busc_inf) |
| reversar_Click | INF, ARC, INC, EVI | [CMXsrv_iinf_rev_evi](#cmxsrv_iinf_rev_evi) |

---

## COBERIMP
<a name="coberimp" ></a>

| **Segmento** | **Tabla Referenciada** | **Procedimiento Almacenado** |
|-------------|----------------------|--------------------------|
| Form_Activate | DIC, POSBCX10, COB, ACMXBCOCEN, ACMXMONEDA, ACMXPAIS | [CMXsrv_icob_lee_pln](#cmxsrv_icob_lee_pln) |
| Mcobcur_Click | comex.dbo, COB | [CMXsrv_icob_cur_cob](#cmxsrv_icob_cur_cob) |
| Mcobcur_Click | DDI, ACMXDESEMB, ADI, DIC, ACMXPRMGRL, ACMXMONEDAFEC, COB, INF, warnmsg | [CMXsrv_icob_pag_sop](#cmxsrv_icob_pag_sop) |
| MCOBELI_CLICK | COB | [CMXsrv_icob_eli_pln](#cmxsrv_icob_eli_pln) |
| Mcobrev_Click | POSBCX10, TRSD, PSO, comex..COB, COB | [CMXsrv_icob_rev_etd](#cmxsrv_icob_rev_etd) |
| Mcobvali_Click | DDI, LCB, ADI, CUO, ARC, NEG, CBR, COB, INF, ACMXFPAIMP, warnmsg, COL | [CMXsrv_icob_val_cob](#cmxsrv_icob_val_cob) |
| buscar_click | COB | [CMXsrv_icob_busc_pln](#cmxsrv_icob_busc_pln) |
| FLD_COB_COD_CLI_LostFocus | CLN | [CMXsrv_icob_lee_cln](#cmxsrv_icob_lee_cln) |
| PROXIMAS_Click | COB | [CMXsrv_icob_busc_pln](#cmxsrv_icob_busc_pln) |
| ACEPTAR_Click | CRD, ARC, CBR, COB, INF, tbl_User, CLN, COL | [CMXsrv_icob_crea_norm](#cmxsrv_icob_crea_norm) |
| ACEPTAR_Click | DIC, COB | [CMXsrv_icob_crea_reem](#cmxsrv_icob_crea_reem) |
| ACEPTAR_Click | CLN, COB | [CMXsrv_icob_act_gral](#cmxsrv_icob_act_gral) |
| FLD_COB_COD_CLI_LostFocus | CLN | [CMXsrv_icob_lee_cln2](#cmxsrv_icob_lee_cln2) |
| Form_Activate | ACMXBCOCEN, ACMXPAIS, COB | [CMXsrv_icob_lee_gral](#cmxsrv_icob_lee_gral) |
| ACEPTAR_Click | ACMXMONEDAFEC, COB | [CMXsrv_icob_act_val](#cmxsrv_icob_act_val) |
| Form_Activate | COB | [CMXsrv_icob_lee_val](#cmxsrv_icob_lee_val) |
| ACEPTAR_Click | COB | [CMXsrv_icob_act_acu](#cmxsrv_icob_act_acu) |
| Form_Activate | ACMXPAIS, COB | [CMXsrv_icob_lee_acu](#cmxsrv_icob_lee_acu) |
| Form_Load | ACMXPAIS, COB | [CMXsrv_icob_lee_acu](#cmxsrv_icob_lee_acu) |
| ELIMINAR_Click | DIC, COB | [CMXsrv_icob_eli_int](#cmxsrv_icob_eli_int) |
| Form_Activate | DIC | [CMXsrv_icob_busc_int](#cmxsrv_icob_busc_int) |
| ACEPTAR_Click | DIC, COB | [CMXsrv_icob_ingmod_int](#cmxsrv_icob_ingmod_int) |
| Form_Activate | DIC | [CMXsrv_icob_lee_int](#cmxsrv_icob_lee_int) |
| ACEPTAR_Click | CLN, tbl_User, COB | [CMXsrv_icob_ing_mod_srf](#cmxsrv_icob_ing_mod_srf) |
| CmdEliminar_Click | COB | [CMXsrv_icob_eli_pln](#cmxsrv_icob_eli_pln) |
| CmdReversar_Click | POSBCX10, TRSD, PSO, comex..COB, COB | [CMXsrv_icob_rev_etd](#cmxsrv_icob_rev_etd) |
| CURSAR_Click | CLN, tbl_User, COB | [CMXsrv_icob_ing_mod_srf](#cmxsrv_icob_ing_mod_srf) |
| CURSAR_Click | DDI, ACMXDESEMB, ADI, DIC, ACMXPRMGRL, ACMXMONEDAFEC, COB, INF, warnmsg | [CMXsrv_icob_pag_sop](#cmxsrv_icob_pag_sop) |
| FLD_COB_COD_CLI_LostFocus | CLN | [CMXsrv_icob_lee_cln2](#cmxsrv_icob_lee_cln2) |
| Reversar_Click | POSBCX10, TRSD, PSO, comex..COB, COB | [CMXsrv_icob_rev_etd](#cmxsrv_icob_rev_etd) |
| ACEPTAR_Click | DIC, POSBCX10, ACMXMONEDAFEC, PSO, COB, ACMXTPOAUTN | [CMXsrv_icob_anu](#cmxsrv_icob_anu) |
| Form_Load | COB | [CMXsrv_icob_lee_anu](#cmxsrv_icob_lee_anu) |
| FLD_COB_COD_CLI_LostFocus | CLN | [CMXsrv_icob_lee_cln](#cmxsrv_icob_lee_cln) |
| ACEPTAR_Click | DDI, ACMXDESEMB, ADI, DIC, ACMXPRMGRL, ACMXMONEDAFEC, COB, INF, warnmsg | [CMXsrv_icob_pag_sop](#cmxsrv_icob_pag_sop) |
| ACEPTAR_Click | comex..COB, COB | [CMXsrv_icob_cur_reem](#cmxsrv_icob_cur_reem) |
| Form_Load |  | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |

---

## COBRANZA
<a name="cobranza" ></a>

| **Segmento** | **Tabla Referenciada** | **Procedimiento Almacenado** |
|-------------|----------------------|--------------------------|
| ejecut_avi_imp_999 | SWT | [CMXsrv_busc_cor_swf](#cmxsrv_busc_cor_swf) |
| ejecut_avi_imp_999 | SMS | [CMXsrv_swf_bus_sms](#cmxsrv_swf_bus_sms) |
| Form_Activate | ACMXPAIS, COR, LCB, ACMXVIATPT, ACMXBCOBCC, CBR, ACMXMONEDA, ACMXCLACOM, tbl_User, ACMXSUCSAL, CLN | [CMXsrv_icbr_lee_cbr](#cmxsrv_icbr_lee_cbr) |
| Form_Load |  | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |
| Mcbrace_Click | comex..CBR, LCB, CBR | [CMXsrv_icbr_acep_let](#cmxsrv_icbr_acep_let) |
| Mcbrcon_Click | OPE_BCI, APRCBL, LCB, CBR | [CMXsrv_icbr_cont_cbr](#cmxsrv_icbr_cont_cbr) |
| Mcbreli_click | ARC, REMENT, CBR, comex..COL | [CMXsrv_icbr_eli_cbr](#cmxsrv_icbr_eli_cbr) |
| McbrTxt999_Click | ACMXSUCSAL, MCBRCTP, CBR, ACMXPAIS, CLN, CBRANX | [CMXsrv_icbr_lee_ctp](#cmxsrv_icbr_lee_ctp) |
| Mcbrtxtrec_Click | ACMXDESEMB, ASND, ACMXBCOBCC, ARC, CBR, ACMXINTERE, PCX, ECE, ACMXMONEDA, ACMXSUCSAL, CLN | [CMXsrv_icbr_avi1](#cmxsrv_icbr_avi1) |
| aceptar_Click | ACMXSUCSAL, tbl_User | [CMXsrv_val_suc](#cmxsrv_val_suc) |
| buscar_Click | ACMXSUCSAL, ACMXMONEDA, CLN, CBR | [CMXsrv_icbr_busc_cbr](#cmxsrv_icbr_busc_cbr) |
| fld_aux_glo_ofi_LostFocus | ACMXSUCSAL, tbl_User | [CMXsrv_val_suc](#cmxsrv_val_suc) |
| fld_cbr_cod_gdo_LostFocus | CLN | [CMXsrv_icbr_lee_cln](#cmxsrv_icbr_lee_cln) |
| fld_cbr_cod_ofi_lostfocus | ACMXSUCSAL, tbl_User | [CMXsrv_val_suc](#cmxsrv_val_suc) |
| proximas_Click | ACMXSUCSAL, ACMXMONEDA, CLN, CBR | [CMXsrv_icbr_busc_cbr](#cmxsrv_icbr_busc_cbr) |
| crear_Click | CLN, tbl_User | [CMXsrv_icbr_crea_cbr](#cmxsrv_icbr_crea_cbr) |
| fld_cbr_cod_gdo_LostFocus | CLN | [CMXsrv_icbr_lee_cln](#cmxsrv_icbr_lee_cln) |
| fld_cbr_cod_ofi_lostfocus | ACMXSUCSAL, tbl_User | [CMXsrv_val_suc](#cmxsrv_val_suc) |
| INGRESAR_Click | CLN, tbl_User | [CMXsrv_icbr_crea_cbr](#cmxsrv_icbr_crea_cbr) |
| fld_cbr_cod_gdo_LostFocus | CLN | [CMXsrv_icbr_lee_cln](#cmxsrv_icbr_lee_cln) |
| Form_Activate | COB | [CMXsrv_icbr_lee_cob](#cmxsrv_icbr_lee_cob) |
| Form_Load | ACMXSUCSAL, MCBRCTP, CBR, ACMXPAIS, CLN, CBRANX | [CMXsrv_icbr_lee_ctp](#cmxsrv_icbr_lee_ctp) |
| INGRESAR_Click | comex..CBR, MCBRCTP, CBRANX, CBR | [CMXsrv_icbr_act_ctp](#cmxsrv_icbr_act_ctp) |
| Form_Activate | COB | [CMXsrv_icbr_lee_cob](#cmxsrv_icbr_lee_cob) |
| Form_Load | ACMXVIATPT, CBR, ACMXINTERE, ACMXMONEDA, MCBRTER, ACMXCLACOM, ACMXPAIS | [CMXsrv_icbr_lee_trm](#cmxsrv_icbr_lee_trm) |
| INGRESAR_Click | LCB, COM, CBR, MCBRTER, warnmsg, CLN | [CMXsrv_icbr_act_trm](#cmxsrv_icbr_act_trm) |
| Form_Activate | COB | [CMXsrv_icbr_lee_cob](#cmxsrv_icbr_lee_cob) |
| Form_Load | LCB, MCBRDOC, MLCB, CBR, ACMXMONEDA | [CMXsrv_icbr_lee_doc](#cmxsrv_icbr_lee_doc) |
| INGRESAR_Click | LCB, MCBRDOC, MLCB, CBR, comex..CBR | [CMXsrv_icbr_act_doc](#cmxsrv_icbr_act_doc) |
| Form_Activate | MLCB, comex..MLCB, comex..LCB | [CMXsrv_icbr_busc_let](#cmxsrv_icbr_busc_let) |
| aceptar_Click | LCB, CBR, comex.dbo | [CMXsrv_icbr_ingmod_let](#cmxsrv_icbr_ingmod_let) |
| eliminar_Click | LCB, MCBRDOC, MLCB, CBR, comex..COL | [CMXsrv_icbr_eli_let](#cmxsrv_icbr_eli_let) |
| Form_Activate | ACMXNOTARIO, LCB, MLCB | [CMXsrv_icbr_lee_let](#cmxsrv_icbr_lee_let) |
| aceptar_Click | comex..CBR, LCB, CBR | [CMXsrv_icbr_prorr](#cmxsrv_icbr_prorr) |
| EFECTUAR_Click | APRCBL, TRSD, CBR, vig_trs, ECE, DIP, LIB, tbl_User | [CMXsrv_icbr_rev_eve](#cmxsrv_icbr_rev_eve) |
| Form_Activate | ECE | [CMXsrv_icbr_busc_eve](#cmxsrv_icbr_busc_eve) |
| Form_Load | ECE, ACMXDESEMB | [CMXsrv_icbr_lee_eve](#cmxsrv_icbr_lee_eve) |
| Form_Load | CBR | [CMXsrv_icbr_lee_ent_doc](#cmxsrv_icbr_lee_ent_doc) |
| aceptar_Click | LCB, CBR | [CMXsrv_icbr_prot](#cmxsrv_icbr_prot) |
| Form_Load | LCB, CBR | [CMXsrv_icbr_pcg_prot](#cmxsrv_icbr_pcg_prot) |
| aceptar_Click | comex..CBR, LCB, CBR | [CMXsrv_icbr_liq_sdo](#cmxsrv_icbr_liq_sdo) |
| aceptar_Click | comex..CBR, CBR | [CMXsrv_icbr_act_vis](#cmxsrv_icbr_act_vis) |
| eliminar_Click | REP | [CMXsrv_icbr_eli_rep](#cmxsrv_icbr_eli_rep) |
| Form_Activate | REP | [CMXsrv_icbr_busc_rep](#cmxsrv_icbr_busc_rep) |
| aceptar_Click | REP, CBR | [CMXsrv_icbr_imod_rep](#cmxsrv_icbr_imod_rep) |
| aceptar_Click | comex..CBR, LCB, CBR | [CMXsrv_icbr_ent_doc](#cmxsrv_icbr_ent_doc) |
| Form_Load | CBR | [CMXsrv_icbr_lee_ent_doc](#cmxsrv_icbr_lee_ent_doc) |
| aceptar_Click | comex..CBR, ACMXSUCSAL, CBR | [CMXsrv_icbr_trf_ofi](#cmxsrv_icbr_trf_ofi) |
| aceptar_Click | ACMXSUCSAL, tbl_User | [CMXsrv_val_suc](#cmxsrv_val_suc) |
| aceptar_Click | comex..CBR, ARC, CBR, LCB | [CMXsrv_icbr_trf_bco](#cmxsrv_icbr_trf_bco) |
| aceptar_Click | comex..CBR, CBR | [CMXsrv_icbr_act_inst](#cmxsrv_icbr_act_inst) |
| enviar_Click | switxt, switxt1 | [CMXsrv_iswf_a_pru](#cmxsrv_iswf_a_pru) |
| Form_Load | DDI, LCB, COR, ADI, ARC, ACMXMONEDAFEC, CBR, ACMXINTEREFEC, warnmsg | [CMXsrv_icbr_val_cbr](#cmxsrv_icbr_val_cbr) |
| word_Click | DDI, LCB, COR, ADI, ARC, ACMXMONEDAFEC, CBR, ACMXINTEREFEC, warnmsg | [CMXsrv_icbr_val_cbr](#cmxsrv_icbr_val_cbr) |
| word_Click | switxt, switxt1 | [CMXsrv_iswf_a_pru](#cmxsrv_iswf_a_pru) |

---

## CRDEXT
<a name="crdext" ></a>

| **Segmento** | **Tabla Referenciada** | **Procedimiento Almacenado** |
|-------------|----------------------|--------------------------|
| Aceptar_Click | MIBAB, IBAB | [CMXsrv_icrd_a_ibab](#cmxsrv_icrd_a_ibab) |
| Form_Load | IBAB, COL, MIBAB | [CMXsrv_icrd_lee_glo_ibab](#cmxsrv_icrd_lee_glo_ibab) |
| Aceptar_Click | MIBAR, IBAR | [CMXsrv_icrd_a_ibar](#cmxsrv_icrd_a_ibar) |
| Form_Load | MIBAR, COL, IBAR | [CMXsrv_icrd_lee_glo_ibar](#cmxsrv_icrd_lee_glo_ibar) |
| buscar_click | ACMXTSWFESPMSG, ACMXTSWFINGMSG | [CMXsrv_icrd_lee_tex_swf](#cmxsrv_icrd_lee_tex_swf) |
| Aceptar_Click | ACMXTSWFESPMSG, ACMXTSWFINGMSG | [CMXsrv_icrd_lee_cod_txt_swf](#cmxsrv_icrd_lee_cod_txt_swf) |
| buscar_click | ACMXTSWFESPMSG, ACMXTSWFINGMSG | [CMXsrv_icrd_lee_txt_swf_all](#cmxsrv_icrd_lee_txt_swf_all) |
| Form_Load | MCTP, CRD | [CMXsrv_icrd_lee_ind_esp_ing](#cmxsrv_icrd_lee_ind_esp_ing) |
| llena_arreglo | ACMXTSWFESPMSG, ACMXTSWFINGMSG | [CMXsrv_icrd_lee_tex_swf](#cmxsrv_icrd_lee_tex_swf) |
| proximo_Click | ACMXTSWFESPMSG, ACMXTSWFINGMSG | [CMXsrv_icrd_lee_txt_swf_all](#cmxsrv_icrd_lee_txt_swf_all) |
| aceptar_Click | CRD | [CMXsrv_icrd_ing_acu](#cmxsrv_icrd_ing_acu) |
| Form_Load | CRD | [CMXsrv_icrd_lee_acu](#cmxsrv_icrd_lee_acu) |
| aceptar_Click | CRD, comex..COL, OPE_BCI, COL, comex..CRD | [CMXsrv_icrd_rech_sol](#cmxsrv_icrd_rech_sol) |
| aceptar_Click | INF, ARC, COL, CRD | [CMXsrv_icrd_end](#cmxsrv_icrd_end) |
| Form_Load | CRD | [CMXsrv_icrd_lee_dat_end](#cmxsrv_icrd_lee_dat_end) |
| aceptar_Click | COR, ACMXMONEDAFEC, CRD, LCR | [CMXsrv_icrd_asignar_cor](#cmxsrv_icrd_asignar_cor) |
| buscar_Click | COR | [CMXsrv_icrd_bus_lcr_bco](#cmxsrv_icrd_bus_lcr_bco) |
| proximo_Click | COR | [CMXsrv_icrd_bus_lcr_bco](#cmxsrv_icrd_bus_lcr_bco) |
| Form_Load |  | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |

---

## CRD_CORR
<a name="crd_corr" ></a>

| **Segmento** | **Tabla Referenciada** | **Procedimiento Almacenado** |
|-------------|----------------------|--------------------------|
| aceptar_Click | COR, ACMXMONEDAFEC, CRD, LCR | [CMXsrv_icrd_asignar_cor](#cmxsrv_icrd_asignar_cor) |
| buscar_Click | COR | [CMXsrv_icrd_bus_lcr_bco](#cmxsrv_icrd_bus_lcr_bco) |
| fld_cor_cod_mtr_LostFocus | comex..ACMXBANCOS | [CMXsrv_icrd_lee_bco_mtr](#cmxsrv_icrd_lee_bco_mtr) |
| fld_cor_cod_pais_Lostfocus | comex..ACMXPAIS | [CMXsrv_icrd_cor_lee_pais](#cmxsrv_icrd_cor_lee_pais) |
| fld_cor_cod_plz_Lostfocus | ACMXPLAZAS | [CMXsrv_icrd_lee_plz](#cmxsrv_icrd_lee_plz) |
| proximo_Click | COR | [CMXsrv_icrd_bus_lcr_bco](#cmxsrv_icrd_bus_lcr_bco) |
| buscar_Click | comex..ACMXPLAZAS | [CMXsrv_icrd_busc_plz](#cmxsrv_icrd_busc_plz) |
| proximos_Click | comex..ACMXPLAZAS | [CMXsrv_icrd_busc_plz](#cmxsrv_icrd_busc_plz) |
| buscar_Click | comex, comex..ACMXPAIS | [CMXsrv_icrd_cor_busc_pais](#cmxsrv_icrd_cor_busc_pais) |
| proximos_Click | comex, comex..ACMXPAIS | [CMXsrv_icrd_cor_busc_pais](#cmxsrv_icrd_cor_busc_pais) |
| buscar_Click | comex | [CMXsrv_icrd_busc_bco_mtr](#cmxsrv_icrd_busc_bco_mtr) |
| proximos_Click | comex | [CMXsrv_icrd_busc_bco_mtr](#cmxsrv_icrd_busc_bco_mtr) |

---

## DDI
<a name="ddi" ></a>

| **Segmento** | **Tabla Referenciada** | **Procedimiento Almacenado** |
|-------------|----------------------|--------------------------|
| aceptar_Click | INF, DDI | [CMXsrv_iddi_ingmod_ddi](#cmxsrv_iddi_ingmod_ddi) |
| continuar_Click | DDI, ACMXVIATPT, ACMXRGMIMP, INF, ACMXBCOCEN, ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM, ACMXPAIS, CLN | [CMXsrv_iddi_lee_dec](#cmxsrv_iddi_lee_dec) |
| eliminar_Click | DDI | [CMXsrv_iddi_eli_ddi](#cmxsrv_iddi_eli_ddi) |
| fld_ddi_fec_ii_lostfocus | INF | [CMXsrv_iddi_lee_inf](#cmxsrv_iddi_lee_inf) |
| fld_ddi_rut_imp_lostfocus | CLN | [CMXsrv_iddi_lee_cln](#cmxsrv_iddi_lee_cln) |
| Asociar_Click | DDI | [CMXsrv_iddi_lee_rut](#cmxsrv_iddi_lee_rut) |
| Asociar_Click | DDI, ARC, ACMXMONEDAFEC, CBR, COB, INF, ACMXMONEDA, COL | [CMXsrv_iddi_asoc_ddi](#cmxsrv_iddi_asoc_ddi) |
| Command2_Click | DDI, ADI, COB | [CMXsrv_iddi_des_ddi](#cmxsrv_iddi_des_ddi) |
| Desasociar_Click | DDI | [CMXsrv_iddi_lee_rut](#cmxsrv_iddi_lee_rut) |
| Desasociar_Click | DDI, ADI, COB | [CMXsrv_iddi_des_ddi](#cmxsrv_iddi_des_ddi) |
| fld_aux_rut_cli_lostfocus | CLN | [CMXsrv_iddi_lee_cln](#cmxsrv_iddi_lee_cln) |
| inicio_asoc | ADI | [CMXsrv_iddi_busc_asoc](#cmxsrv_iddi_busc_asoc) |
| inicio_noasoc | DDI, ADI | [CMXsrv_iddi_busc_noasoc](#cmxsrv_iddi_busc_noasoc) |
| proximo_no_aso_Click | DDI, ADI | [CMXsrv_iddi_busc_noasoc](#cmxsrv_iddi_busc_noasoc) |

---

## IMPORT
<a name="import" ></a>

| **Segmento** | **Tabla Referenciada** | **Procedimiento Almacenado** |
|-------------|----------------------|--------------------------|
| buscar_Click | DIRCLN | [CMXsrv_icrd_lee_dir_cln](#cmxsrv_icrd_lee_dir_cln) |
| buscar_click | ACMXTSWFESPMSG, ACMXTSWFINGMSG | [CMXsrv_icrd_lee_tex_swf](#cmxsrv_icrd_lee_tex_swf) |
| Aceptar_Click | ACMXTSWFESPMSG, ACMXTSWFINGMSG | [CMXsrv_icrd_lee_cod_txt_swf](#cmxsrv_icrd_lee_cod_txt_swf) |
| buscar_click | ACMXTSWFESPMSG, ACMXTSWFINGMSG | [CMXsrv_icrd_lee_txt_swf_all](#cmxsrv_icrd_lee_txt_swf_all) |
| Form_Load | MCTP, CRD | [CMXsrv_icrd_lee_ind_esp_ing](#cmxsrv_icrd_lee_ind_esp_ing) |
| llena_arreglo | ACMXTSWFESPMSG, ACMXTSWFINGMSG | [CMXsrv_icrd_lee_tex_swf](#cmxsrv_icrd_lee_tex_swf) |
| proximo_Click | ACMXTSWFESPMSG, ACMXTSWFINGMSG | [CMXsrv_icrd_lee_txt_swf_all](#cmxsrv_icrd_lee_txt_swf_all) |
| Aceptar_Click | CND | [CMXCRDsrv_icrd_a_cnd_esp](#cmxcrdsrv_icrd_a_cnd_esp) |
| Form_Load | MMCND, COL, CND | [CMXsrv_icrd_lee_cnd_esp](#cmxsrv_icrd_lee_cnd_esp) |
| clon_Click | CRS, MER, CRD, TAS, CRDCLON, COL_ADI, CND, DAC, ODOC, AVAL, COL, EMB | [CMXCRDsrv_icrd_clon_crd](#cmxcrdsrv_icrd_clon_crd) |
| Form_Activate | CRD_ADI, ACMXFORPAG, ACMXPAIS, ACMXVIATPT, CRD, COR, COL_ADI, ACMXFINVER, PMIX, NEG, ACMXMONEDA, tbl_User, OPE_BCI, ACMXSUCSAL, CLN, COL, DIRCLN, EMB | [CMXCRDsrv_icrd_lee_crdcre](#cmxcrdsrv_icrd_lee_crdcre) |
| Form_Activate | MCTP, CRD | [CMXsrv_icrd_lee_ind_esp_ing](#cmxsrv_icrd_lee_ind_esp_ing) |
| Form_Activate | COL | [CMXsrv_icrd_lee_top](#cmxsrv_icrd_lee_top) |
| Form_Load |  | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |
| Form_Load |  | [CMXsrv_cmx_get_codes](#cmxsrv_cmx_get_codes) |
| Form_Load | ACMXSUCSAL, ACMXDL3475FEC, tbl_User | [CMXsrv_trae_glo_fec](#cmxsrv_trae_glo_fec) |
| Mcrdapr_Click | warnmsg | [CMXCRDsrv_icrd_val_crd](#cmxcrdsrv_icrd_val_crd) |
| Mcrdeli_click | comex..COL, OPE_BCI, CRD | [CMXCRDsrv_icrd_eli_crd](#cmxcrdsrv_icrd_eli_crd) |
| Mcrdtxtliq_Click | ASND, EVI, TRSD, EVE, ACMXMONEDA, COL | [CMXsrv_icrd_lee_dat_trs](#cmxsrv_icrd_lee_dat_trs) |
| Mcrdtxtope_Click | ACMXDESEMB, ASND, EVO, CRD, CNO, OBL, CUO, TRSD, NEG, COM, EVE, ACMXTIPEVE, CAN, COL | [CMXsrv_icrd_dat_liq_ope](#cmxsrv_icrd_dat_liq_ope) |
| msg_swift | switxt, switxt1 | [CMXsrv_iswf_a_pru](#cmxsrv_iswf_a_pru) |
| Aceptar_Click | CRD, CRDCLON, MCTP, comex..COL, COL | [CMXsrv_icrd_a_ctp](#cmxsrv_icrd_a_ctp) |
| FLD_COL_COD_CLI_LostFocus | CLN, DIRCLN | [CMXsrv_icrd_lee_cln](#cmxsrv_icrd_lee_cln) |
| Form_Load | ACMXFECPRO | [CMXsrv_lee_fpro](#cmxsrv_lee_fpro) |
| Aceptar_Click | TIP, CRD_ADI, CRD, CRDCLON, COL_ADI, COM, ACMXMONEDA, LIB, comex..COL, MAPR, MCND, COL, ACMXOPEIMP, comex..CRD | [CMXsrv_icrd_a_cnd](#cmxsrv_icrd_a_cnd) |
| Aceptar_Click | CRD_ADI, PMIX, ACMXMONEDA, CLN, COL | [CMXCRDsrv_icrd_crea_crd](#cmxcrdsrv_icrd_crea_crd) |
| fld_col_fec_vto_LostFocus | ACMXFERIADO | [CMXsrv_util_det_habil](#cmxsrv_util_det_habil) |
| Form_Activate | comex..EMB, comex..MEMB | [CMXsrv_icrd_busc_emb](#cmxsrv_icrd_busc_emb) |
| ELIMINAR_Click | comex..COL, EMB, COL, CRD | [CMXsrv_icrd_eli_emb](#cmxsrv_icrd_eli_emb) |
| Form_Load | CRS, COL, EMB | [CMXsrv_icrd_lee_emb1](#cmxsrv_icrd_lee_emb1) |
| Form_Load | COL, EMB | [CMXsrv_icrd_lee_emb2](#cmxsrv_icrd_lee_emb2) |
| ingresar_Click | CRS, MEMB, CRD, MCRS, CRDCLON, COL, EMB | [CMXsrv_icrd_a_emb1](#cmxsrv_icrd_a_emb1) |
| ingresar_Click | EMB, COL, MEMB, CRD | [CMXsrv_icrd_a_emb2](#cmxsrv_icrd_a_emb2) |
| VALIDA_EMBARQUE | warnmsg | [CMXsrv_icrd_val_emb2](#cmxsrv_icrd_val_emb2) |
| VALIDA_EMBARQUE | INF, ARC, warnmsg | [CMXsrv_icrd_val_emb1](#cmxsrv_icrd_val_emb1) |
| Aceptar_Click | MREF, CRD, CRDCLON, comex..MREF, comex..COL, COL | [CMXsrv_icrd_act_ref](#cmxsrv_icrd_act_ref) |
| Form_Load | MREF, CRD, CRDCLON, comex..MREF, comex..COL, COL | [CMXsrv_icrd_act_ref](#cmxsrv_icrd_act_ref) |
| Form_Load | COR, COL, CRD | [CMXsrv_icrd_lee_ref](#cmxsrv_icrd_lee_ref) |
| FLD_COL_COD_CLI_LostFocus | CLN, DIRCLN | [CMXsrv_icrd_lee_cln](#cmxsrv_icrd_lee_cln) |
| Aceptar_Click | TIP, CRD, COL_ADI, COM, LIB, OPE_BCI, sysobjects, CLN, COL | [CMXCRDsrv_icrd_apr_sol](#cmxcrdsrv_icrd_apr_sol) |
| Form_Load | CRS, CRD, COL_ADI, DAC, ACMXAPROBAC | [CMXsrv_icrd_lee_crdapr](#cmxsrv_icrd_lee_crdapr) |
| Aceptar_Click | CRD, comex..COL, OPE_BCI, COL, comex..CRD | [CMXsrv_icrd_rech_sol](#cmxsrv_icrd_rech_sol) |
| Aceptar_Click | MER | [CMXCRDsrv_icrd_a_desc_merc](#cmxcrdsrv_icrd_a_desc_merc) |
| Form_Load | MMER, MER | [CMXsrv_icrd_lee_desc_merc](#cmxsrv_icrd_lee_desc_merc) |
| Aceptar_Click | ODOC, MODOC | [CMXsrv_icrd_a_otr_doc](#cmxsrv_icrd_a_otr_doc) |
| Form_Load | ODOC, MODOC | [CMXsrv_icrd_lee_otr_doc](#cmxsrv_icrd_lee_otr_doc) |
| enviar_Click | switxt, switxt1 | [CMXsrv_iswf_a_pru](#cmxsrv_iswf_a_pru) |

---

## INFORME
<a name="informe" ></a>

| **Segmento** | **Tabla Referenciada** | **Procedimiento Almacenado** |
|-------------|----------------------|--------------------------|
| Eliminar_Click | ADI, CRD, ARC, NEG, COB, INF, COL | [CMXsrv_iarc_eli_arc](#cmxsrv_iarc_eli_arc) |
| Form_Activate | ARC | [CMXsrv_iarc_busc_arc](#cmxsrv_iarc_busc_arc) |
| Form_Activate | INF | [CMXsrv_iinf_lee0_inf](#cmxsrv_iinf_lee0_inf) |
| Form_Activate | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM | [CMXsrv_iinf_lee_tablas](#cmxsrv_iinf_lee_tablas) |
| Form_Activate | INF, CLN | [CMXsrv_iinf_lee1_inf](#cmxsrv_iinf_lee1_inf) |
| Form_Activate | CLN | [CMXsrv_iinf_lee_cln](#cmxsrv_iinf_lee_cln) |
| Form_Activate | INF | [CMXsrv_iinf_lee2_inf](#cmxsrv_iinf_lee2_inf) |
| Form_Activate | INF | [CMXsrv_iinf_avi_miscb](#cmxsrv_iinf_avi_miscb) |
| Maviapr_Click | INF, CLN | [CMXsrv_iinf_avi_misca](#cmxsrv_iinf_avi_misca) |
| Maviapr_Click | INF | [CMXsrv_iinf_avi_miscb](#cmxsrv_iinf_avi_miscb) |
| Mavicom_Click | INF, CLN | [CMXsrv_iinf_avi_misca](#cmxsrv_iinf_avi_misca) |
| Mavicom_Click | INF | [CMXsrv_iinf_avi_miscb](#cmxsrv_iinf_avi_miscb) |
| Mavicom_Click | TIP, ACMXDESEMB, ASND, CRD, EVI, COM, TRSD, EVE, ACMXMONEDA | [CMXsrv_icrd_lee_dat_com](#cmxsrv_icrd_lee_dat_com) |
| Mavimis1_Click | INF, CLN | [CMXsrv_iinf_avi_misca](#cmxsrv_iinf_avi_misca) |
| Mavimis1_Click | INF | [CMXsrv_iinf_avi_miscb](#cmxsrv_iinf_avi_miscb) |
| Mavimis2_Click | INF, CLN | [CMXsrv_iinf_avi_misca](#cmxsrv_iinf_avi_misca) |
| Mavimis2_Click | INF | [CMXsrv_iinf_avi_miscb](#cmxsrv_iinf_avi_miscb) |
| Mavirec_Click | INF, CLN | [CMXsrv_iinf_avi_misca](#cmxsrv_iinf_avi_misca) |
| Mavirec_Click | INF | [CMXsrv_iinf_avi_miscb](#cmxsrv_iinf_avi_miscb) |
| Mavitib_Click | INF, CLN | [CMXsrv_iinf_avi_misca](#cmxsrv_iinf_avi_misca) |
| Mavitib_Click | INF | [CMXsrv_iinf_avi_miscb](#cmxsrv_iinf_avi_miscb) |
| Mavitras_Click | INF, CLN | [CMXsrv_iinf_avi_misca](#cmxsrv_iinf_avi_misca) |
| Mavitras_Click | INF | [CMXsrv_iinf_avi_miscb](#cmxsrv_iinf_avi_miscb) |
| Mavitras_Click | ASND, EVI, TRSD, EVE, ACMXMONEDA, COL | [CMXsrv_icrd_lee_dat_trs](#cmxsrv_icrd_lee_dat_trs) |
| Minfoeli_click | INF, ARC | [CMXsrv_iinf_eli_inf](#cmxsrv_iinf_eli_inf) |
| Minforev_Click | EVI | [CMXsrv_iinf_busc_evi](#cmxsrv_iinf_busc_evi) |
| Minfoval_click | INF, ACMXPAIS, warnmsg | [CMXsrv_iinf_val_inf](#cmxsrv_iinf_val_inf) |
| Aceptar_Click | INF, tbl_User, warnmsg | [CMXsrv_iinf_ingmod_inf](#cmxsrv_iinf_ingmod_inf) |
| Fec_pre |  | [CMXsrv_iinf_lee_fec](#cmxsrv_iinf_lee_fec) |
| fld_aux_glo_cls_com_LostFocus | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM | [CMXsrv_iinf_lee_tablas](#cmxsrv_iinf_lee_tablas) |
| fld_aux_glo_for_pag1_LostFocus | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM | [CMXsrv_iinf_lee_tablas](#cmxsrv_iinf_lee_tablas) |
| fld_aux_glo_for_pag2_LostFocus | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM | [CMXsrv_iinf_lee_tablas](#cmxsrv_iinf_lee_tablas) |
| fld_aux_glo_for_pag3_LostFocus | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM | [CMXsrv_iinf_lee_tablas](#cmxsrv_iinf_lee_tablas) |
| fld_aux_glo_mon_LostFocus | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM | [CMXsrv_iinf_lee_tablas](#cmxsrv_iinf_lee_tablas) |
| fld_inf_cls_com_Lostfocus | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM | [CMXsrv_iinf_lee_tablas](#cmxsrv_iinf_lee_tablas) |
| fld_inf_cod_imp_LostFocus | CLN | [CMXsrv_iinf_lee_cln](#cmxsrv_iinf_lee_cln) |
| fld_inf_for_pag1_lostfocus | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM | [CMXsrv_iinf_lee_tablas](#cmxsrv_iinf_lee_tablas) |
| fld_inf_for_pag2_LostFocus | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM | [CMXsrv_iinf_lee_tablas](#cmxsrv_iinf_lee_tablas) |
| fld_inf_for_pag3_LostFocus | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM | [CMXsrv_iinf_lee_tablas](#cmxsrv_iinf_lee_tablas) |
| fld_inf_mon_inf_lostfocus | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM | [CMXsrv_iinf_lee_tablas](#cmxsrv_iinf_lee_tablas) |
| Form_Load | INF | [CMXsrv_iinf_lee0_inf](#cmxsrv_iinf_lee0_inf) |
| Form_Load | INF, CLN | [CMXsrv_iinf_lee1_inf](#cmxsrv_iinf_lee1_inf) |
| Form_Load | INF | [CMXsrv_iinf_lee2_inf](#cmxsrv_iinf_lee2_inf) |
| valor_usd |  | [CMXsrv_iinf_lee_usd](#cmxsrv_iinf_lee_usd) |
| Aceptar_Click | INF | [CMXsrv_iinf_busc_inf](#cmxsrv_iinf_busc_inf) |
| buscar_Click | INF | [CMXsrv_iinf_busc_inf](#cmxsrv_iinf_busc_inf) |
| Fec_pre |  | [CMXsrv_iinf_lee_fec](#cmxsrv_iinf_lee_fec) |
| fld_inf_cod_imp_LostFocus | CLN | [CMXsrv_iinf_lee_cln](#cmxsrv_iinf_lee_cln) |
| PROXIMA_Click | INF | [CMXsrv_iinf_busc_inf](#cmxsrv_iinf_busc_inf) |
| Aceptar_Click | INF | [CMXsrv_iinf_act_apr](#cmxsrv_iinf_act_apr) |
| Form_Activate | EVI | [CMXsrv_iinf_busc_evi](#cmxsrv_iinf_busc_evi) |
| reversar_Click | INF, ARC, INC, EVI | [CMXsrv_iinf_rev_evi](#cmxsrv_iinf_rev_evi) |
| Form_Load | EVI | [CMXsrv_iinf_lee_evi](#cmxsrv_iinf_lee_evi) |
| Aceptar_Click | INF | [CMXsrv_iinf_act_tib](#cmxsrv_iinf_act_tib) |
| Aceptar_Click | INF | [CMXsrv_iinf_act_rec](#cmxsrv_iinf_act_rec) |
| Aceptar_Click | INF | [CMXsrv_iinf_act_rib](#cmxsrv_iinf_act_rib) |
| Form_Activate | INF | [CMXsrv_iinf_busc_comp](#cmxsrv_iinf_busc_comp) |
| proximos_Click | INF | [CMXsrv_iinf_busc_comp](#cmxsrv_iinf_busc_comp) |
| Aceptar_Click | INF, warnmsg | [CMXsrv_iinf_ingmod_comp](#cmxsrv_iinf_ingmod_comp) |
| Fec_pre |  | [CMXsrv_iinf_lee_fec](#cmxsrv_iinf_lee_fec) |
| Form_Activate | INF | [CMXsrv_iinf_lee_comp](#cmxsrv_iinf_lee_comp) |
| Form_Activate | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM | [CMXsrv_iinf_lee_tablas](#cmxsrv_iinf_lee_tablas) |
| aceptar_click | COR | [CMXsrv_iinf_lee_bco](#cmxsrv_iinf_lee_bco) |
| buscar_Click | ACMXBCOBCC | [CMXsrv_iinf_busc_bco](#cmxsrv_iinf_busc_bco) |
| Form_Load |  | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |

---

## MOD_ADI
<a name="mod_adi" ></a>

| **Segmento** | **Tabla Referenciada** | **Procedimiento Almacenado** |
|-------------|----------------------|--------------------------|
| Aceptar_Click | TIP, CRD_ADI, CRD, CRDCLON, COL_ADI, COM, ACMXMONEDA, LIB, comex..COL, MAPR, MCND, COL, ACMXOPEIMP, comex..CRD | [CMXsrv_icrd_a_cnd](#cmxsrv_icrd_a_cnd) |
| busca_bco | ACMXPAIS, COR | [CMXsrv_icrd_lee_bco_swf](#cmxsrv_icrd_lee_bco_swf) |
| fld_col_fec_vto_LostFocus | ACMXFERIADO | [CMXsrv_util_det_habil](#cmxsrv_util_det_habil) |
| Form_Load | CRD_ADI, ACMXFORPAG, CRD, PMIX, ACMXMONEDA, MPMIX, MCND | [CMXMCRDsrv_icrd_lee_mcnd](#cmxmcrdsrv_icrd_lee_mcnd) |
| Form_Load |  | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |

---

## MOD_CBR
<a name="mod_cbr" ></a>

| **Segmento** | **Tabla Referenciada** | **Procedimiento Almacenado** |
|-------------|----------------------|--------------------------|
| fld_cbr_cod_gdo_LostFocus | CLN | [CMXsrv_icbr_lee_cln](#cmxsrv_icbr_lee_cln) |
| Form_Load | ACMXSUCSAL, MCBRCTP, CBR, ACMXPAIS, CLN, CBRANX | [CMXsrv_icbr_lee_ctp](#cmxsrv_icbr_lee_ctp) |
| INGRESAR_Click | comex..CBR, MCBRCTP, CBRANX, CBR | [CMXsrv_icbr_act_ctp](#cmxsrv_icbr_act_ctp) |
| Form_Load | ACMXVIATPT, CBR, ACMXINTERE, ACMXMONEDA, MCBRTER, ACMXCLACOM, ACMXPAIS | [CMXsrv_icbr_lee_trm](#cmxsrv_icbr_lee_trm) |
| INGRESAR_Click | LCB, COM, CBR, MCBRTER, warnmsg, CLN | [CMXsrv_icbr_act_trm](#cmxsrv_icbr_act_trm) |
| Form_Load | LCB, MCBRDOC, MLCB, CBR, ACMXMONEDA | [CMXsrv_icbr_lee_doc](#cmxsrv_icbr_lee_doc) |
| INGRESAR_Click | LCB, MCBRDOC, MLCB, CBR, comex..CBR | [CMXsrv_icbr_act_doc](#cmxsrv_icbr_act_doc) |
| Form_Activate | MLCB, comex..MLCB, comex..LCB | [CMXsrv_icbr_busc_let](#cmxsrv_icbr_busc_let) |
| aceptar_Click | LCB, MLCB, CBR, end | [CMXsrv_icbr_mod_ing_let](#cmxsrv_icbr_mod_ing_let) |
| eliminar_Click | LCB, MCBRDOC, MLCB, CBR, comex..COL | [CMXsrv_icbr_eli_let](#cmxsrv_icbr_eli_let) |
| Form_Activate | ACMXNOTARIO, LCB, MLCB | [CMXsrv_icbr_lee_let](#cmxsrv_icbr_lee_let) |
| actualizar_Click | LCB, MCBRDOC, MCBRCTP, MLCB, CBR, MCBRTER, warnmsg | [CMXsrv_icbr_acep_mod_cbr](#cmxsrv_icbr_acep_mod_cbr) |
| Cancelar_Click | MCBRDOC, MCBRCTP, MLCB, CBR, MCBRTER | [CMXsrv_icbr_eli_no_cont](#cmxsrv_icbr_eli_no_cont) |

---

## MOD_CRD
<a name="mod_crd" ></a>

| **Segmento** | **Tabla Referenciada** | **Procedimiento Almacenado** |
|-------------|----------------------|--------------------------|
| Aceptar_Click | MIBAB, IBAB | [CMXsrv_icrd_a_ibab](#cmxsrv_icrd_a_ibab) |
| Form_Load | IBAB, COL, MIBAB | [CMXsrv_icrd_lee_glo_ibab](#cmxsrv_icrd_lee_glo_ibab) |
| Aceptar_Click | MIBAR, IBAR | [CMXsrv_icrd_a_ibar](#cmxsrv_icrd_a_ibar) |
| Form_Load | MIBAR, COL, IBAR | [CMXsrv_icrd_lee_glo_ibar](#cmxsrv_icrd_lee_glo_ibar) |
| buscar_click | DIRCLN | [CMXsrv_icrd_lee_dir_cln](#cmxsrv_icrd_lee_dir_cln) |
| buscar_Click | ACMXTSWFESPMSG, ACMXTSWFINGMSG | [CMXsrv_icrd_lee_tex_swf](#cmxsrv_icrd_lee_tex_swf) |
| buscar_click | ACMXTSWFESPMSG, ACMXTSWFINGMSG | [CMXsrv_icrd_lee_tex_swf](#cmxsrv_icrd_lee_tex_swf) |
| Aceptar_Click | ACMXTSWFESPMSG, ACMXTSWFINGMSG | [CMXsrv_icrd_lee_cod_txt_swf](#cmxsrv_icrd_lee_cod_txt_swf) |
| buscar_click | ACMXTSWFESPMSG, ACMXTSWFINGMSG | [CMXsrv_icrd_lee_txt_swf_all](#cmxsrv_icrd_lee_txt_swf_all) |
| Form_Load | MCTP, CRD | [CMXsrv_icrd_lee_ind_esp_ing](#cmxsrv_icrd_lee_ind_esp_ing) |
| llena_arreglo | ACMXTSWFESPMSG, ACMXTSWFINGMSG | [CMXsrv_icrd_lee_tex_swf](#cmxsrv_icrd_lee_tex_swf) |
| proximo_Click | ACMXTSWFESPMSG, ACMXTSWFINGMSG | [CMXsrv_icrd_lee_txt_swf_all](#cmxsrv_icrd_lee_txt_swf_all) |
| Aceptar_Click | MMCND | [CMXMCRDsrv_icrd_a_mmcnd](#cmxmcrdsrv_icrd_a_mmcnd) |
| Form_Load | MMCND, COL, CND | [CMXsrv_icrd_lee_cnd_esp](#cmxsrv_icrd_lee_cnd_esp) |
| Aceptar_Click | CRD, CRDCLON, MCTP, comex..COL, COL | [CMXsrv_icrd_a_ctp](#cmxsrv_icrd_a_ctp) |
| FLD_COL_COD_CLI_LostFocus | CLN, DIRCLN | [CMXsrv_icrd_lee_cln](#cmxsrv_icrd_lee_cln) |
| Form_Load | ACMXPAIS, MCTP, DIRCLN, CRD | [CMXMCRDsrv_icrd_lee_mctp](#cmxmcrdsrv_icrd_lee_mctp) |
| Aceptar_Click | TIP, CRD_ADI, CRD, CRDCLON, COL_ADI, COM, ACMXMONEDA, LIB, comex..COL, MAPR, MCND, COL, ACMXOPEIMP, comex..CRD | [CMXsrv_icrd_a_cnd](#cmxsrv_icrd_a_cnd) |
| Form_Load | CRD_ADI, ACMXFORPAG, CRD, PMIX, ACMXMONEDA, MPMIX, MCND | [CMXMCRDsrv_icrd_lee_mcnd](#cmxmcrdsrv_icrd_lee_mcnd) |
| Form_Activate | comex..EMB, comex..MEMB | [CMXsrv_icrd_busc_emb](#cmxsrv_icrd_busc_emb) |
| cancelar_Click | MMER, MER | [CMXsrv_icrd_lee_desc_merc](#cmxsrv_icrd_lee_desc_merc) |
| ELIMINAR_Click | comex..COL, EMB, COL, CRD | [CMXsrv_icrd_eli_emb](#cmxsrv_icrd_eli_emb) |
| Form_Load | MEMB, EMB | [CMXMCRDsrv_icrd_lee_memb2](#cmxmcrdsrv_icrd_lee_memb2) |
| Form_Load | CRS, MEMB, EMB, MCRS | [CMXMCRDsrv_icrd_lee_memb1](#cmxmcrdsrv_icrd_lee_memb1) |
| ingresar_Click | CRS, MEMB, CRD, MCRS, CRDCLON, COL, EMB | [CMXsrv_icrd_a_emb1](#cmxsrv_icrd_a_emb1) |
| ingresar_Click | EMB, COL, MEMB, CRD | [CMXsrv_icrd_a_emb2](#cmxsrv_icrd_a_emb2) |
| VALIDA_EMBARQUE | warnmsg | [CMXsrv_icrd_val_emb2](#cmxsrv_icrd_val_emb2) |
| VALIDA_EMBARQUE | INF, ARC, warnmsg | [CMXsrv_icrd_val_emb1](#cmxsrv_icrd_val_emb1) |
| Aceptar_Click | MREF, CRD, CRDCLON, comex..MREF, comex..COL, COL | [CMXsrv_icrd_act_ref](#cmxsrv_icrd_act_ref) |
| fld_obl_cod_bco_acre_DblClick | ACMXPAIS, COR | [CMXsrv_icrd_lee_bco_swf](#cmxsrv_icrd_lee_bco_swf) |
| fld_obl_cod_bco_acre_LostFocus | ACMXPAIS, COR | [CMXsrv_icrd_lee_bco_swf](#cmxsrv_icrd_lee_bco_swf) |
| Form_Load | MREF, COR, COL, CRD | [CMXMCRDsrv_icrd_lee_mref](#cmxmcrdsrv_icrd_lee_mref) |
| Aceptar_Click | MTXT | [CMXsrv_icrd_ing_txt](#cmxsrv_icrd_ing_txt) |
| Form_Load | ACMXPAIS, MCTP, CRD | [CMXCRDsrv_icrd_get_ing_esp](#cmxcrdsrv_icrd_get_ing_esp) |
| Form_Load | MTXT | [CMXMCRDsrv_icrd_lee_mtxt](#cmxmcrdsrv_icrd_lee_mtxt) |
| Form_Load | ACMXTSWFESPMSG, ACMXTSWFINGMSG | [CMXCRDsrv_icrd_get_pre_fra](#cmxcrdsrv_icrd_get_pre_fra) |
| Aceptar_Click | MMER | [CMXMCRDsrv_icrd_a_mmer](#cmxmcrdsrv_icrd_a_mmer) |
| Form_Load | MMER, MER | [CMXsrv_icrd_lee_desc_merc](#cmxsrv_icrd_lee_desc_merc) |
| Aceptar_Click | ODOC, MODOC | [CMXsrv_icrd_a_otr_doc](#cmxsrv_icrd_a_otr_doc) |
| Form_Load | ODOC, MODOC | [CMXsrv_icrd_lee_otr_doc](#cmxsrv_icrd_lee_otr_doc) |
| Aceptar_Click | MCND, COL, CRD, COM | [CMXsrv_fincol_lee_cod_eve](#cmxsrv_fincol_lee_cod_eve) |
| Aceptar_Click | de, TIP, CRD, COD, MCRS, OBL, EVE, LIB, warnmsg, OPE_BCI, sysobjects, COL | [CMXMCRDsrv_icrd_acep_mod_crd](#cmxmcrdsrv_icrd_acep_mod_crd) |
| cancelar_Click | MREF, MEMB, MCRS, MMCND, COM, MODOC, MIBAB, CRD_AMD, MPMIX, MCTP, MMER, MCND, MIBAR, TNIH, MAPR, FE_IN_REJECTED_TRANS, MTXT | [CMXMCRDsrv_icrd_eli_no_cont](#cmxmcrdsrv_icrd_eli_no_cont) |
| fld_crd_cod_bco_rem_LostFocus | ACMXPAIS, COR | [CMXsrv_icrd_lee_bco_swf](#cmxsrv_icrd_lee_bco_swf) |
| fld_crd_fec_mod_lostFocus | TF_PPAG, TIP, TAS, CUO, comex..ACMXMONEDA, COL_ADI, OBL, CTR, NEG_ADI, ACMXINTERE, CAN, ICR, COL | [CMXsrv_fincol_efec_calpa](#cmxsrv_fincol_efec_calpa) |
| Form_Activate | MCTP, CRD | [CMXsrv_icrd_lee_ind_esp_ing](#cmxsrv_icrd_lee_ind_esp_ing) |
| Form_Load | TF_PPAG, TIP, TAS, CUO, comex..ACMXMONEDA, COL_ADI, OBL, CTR, NEG_ADI, ACMXINTERE, CAN, ICR, COL | [CMXsrv_fincol_efec_calpa](#cmxsrv_fincol_efec_calpa) |
| Form_Load | CRD_ADI, ACMXFORPAG, CRD, PMIX, ACMXMONEDA, MPMIX, MCND | [CMXMCRDsrv_icrd_lee_mcnd](#cmxmcrdsrv_icrd_lee_mcnd) |
| Form_Load |  | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |

---

## NEGO_AV
<a name="nego_av" ></a>

| **Segmento** | **Tabla Referenciada** | **Procedimiento Almacenado** |
|-------------|----------------------|--------------------------|
| aviso1 | COR, TAS, CRD, CUO, CNEG, COM, NEG, TRSD, DIS, EVE, ACMXMONEDA, ACMXINTERE, ACMXSUCSAL, COL | [CMXsrv_icrd_a_rec_age](#cmxsrv_icrd_a_rec_age) |
| aviso1 | CLN | [CMXsrv_busc_ofi_cta](#cmxsrv_busc_ofi_cta) |
| aviso1 | ARC | [CMXsrv_neg_busc_arc](#cmxsrv_neg_busc_arc) |
| aviso1 | CRD | [CMXsrv_icrd_lee_avi_adi](#cmxsrv_icrd_lee_avi_adi) |
| aviso3 | ASND, EVI, TRSD, EVE, ACMXMONEDA, COL | [CMXsrv_icrd_lee_dat_trs](#cmxsrv_icrd_lee_dat_trs) |
| Aviso4 | ACMXDESEMB, ASND, EVO, CRD, CNO, OBL, CUO, TRSD, NEG, COM, EVE, ACMXTIPEVE, CAN, COL | [CMXsrv_icrd_dat_liq_ope](#cmxsrv_icrd_dat_liq_ope) |
| Aviso4 | NEG, CLN, COL | [CMXsrv_icrd_lee_dat_cln](#cmxsrv_icrd_lee_dat_cln) |
| Aviso5 | NEG, CLN, COL | [CMXsrv_icrd_lee_dat_cln](#cmxsrv_icrd_lee_dat_cln) |
| Aviso5 | DIS, COL | [CMXsrv_icrd_lee_avi_dis](#cmxsrv_icrd_lee_avi_dis) |
| Aviso5 | CRD | [CMXsrv_icrd_lee_avi_adi](#cmxsrv_icrd_lee_avi_adi) |
| Aviso5 | ADI | [CMXsrv_neg_ddi_asoc](#cmxsrv_neg_ddi_asoc) |
| Aviso5 | ARC | [CMXsrv_neg_busc_arc](#cmxsrv_neg_busc_arc) |
| Aviso5 | COL, CUO | [CMXsrv_neg_trae_vcto_mcf](#cmxsrv_neg_trae_vcto_mcf) |
| lee_aval | TAS, CNEG, AVAL, CLN, COL | [CMXsrv_neg_avi_lee_aval](#cmxsrv_neg_avi_lee_aval) |
| lee_nego | NEG, COL | [CMXsrv_icrd_neg_lee_crd](#cmxsrv_icrd_neg_lee_crd) |
| lee_nego | TAS, CRD, ACMXFINVER, NEG, NEG_ADI, DIS, COL | [CMXsrv_icrd_lee_neg](#cmxsrv_icrd_lee_neg) |
| avi_col1 | TIP, CRD, DAC, ACMXESPECI, ACMXSUCSAL, CLN, COL, ACLNEJECTA | [CMXsrv_col_avi_dat_cln](#cmxsrv_col_avi_dat_cln) |
| avi_col1 | CCX, TIP, TAS, CRD, COB, ACMXINTERE, EVE, ACMXMONEDA, ACMXINTEREFEC, CAN, CAN_REN, COL | [CMXsrv_col_avi_det_pag](#cmxsrv_col_avi_det_pag) |
| avi_col2 | TIP, CRD, DAC, ACMXESPECI, ACMXSUCSAL, CLN, COL, ACLNEJECTA | [CMXsrv_col_avi_dat_cln](#cmxsrv_col_avi_dat_cln) |
| avi_col2 | TIP, ACMXDESEMB, ASND, TAS, CUO, COD, NEG, ACMXINTERE, EVE, ACMXMONEDA, ACMXINTEREFEC, AVAL, CLN, COL | [CMXsrv_col_avi_det_oto](#cmxsrv_col_avi_det_oto) |
| avi_col4 | TIP, CRD, DAC, ACMXESPECI, ACMXSUCSAL, CLN, COL, ACLNEJECTA | [CMXsrv_col_avi_dat_cln](#cmxsrv_col_avi_dat_cln) |
| avi_col4 | EVE, COL, TIP, COD | [CMXsrv_col_lee_num_trs](#cmxsrv_col_lee_num_trs) |
| lee_obl_pag | CNO, EVO | [CMXsrv_finobl_avi_pag](#cmxsrv_finobl_avi_pag) |
| traspaso | ACMXDESEMB, ASND, COD, TRSD, ACMXMONEDA | [CMXsrv_neg_avi_trae_asnd_mn](#cmxsrv_neg_avi_trae_asnd_mn) |
| traspaso | ACMXDESEMB, ACMXMONEDA, ASND | [CMXsrv_neg_avi_trae_asnd_mx](#cmxsrv_neg_avi_trae_asnd_mx) |
| Form_Activate | NEG, COL | [CMXsrv_icrd_neg_lee_crd](#cmxsrv_icrd_neg_lee_crd) |
| Form_Activate | TAS, CRD, ACMXFINVER, NEG, NEG_ADI, DIS, COL | [CMXsrv_icrd_lee_neg](#cmxsrv_icrd_lee_neg) |
| Mcrdtxtliq_Click | ASND, EVI, TRSD, EVE, ACMXMONEDA, COL | [CMXsrv_icrd_lee_dat_trs](#cmxsrv_icrd_lee_dat_trs) |
| Mcrdtxtope_Click | ACMXDESEMB, ASND, EVO, CRD, CNO, OBL, CUO, TRSD, NEG, COM, EVE, ACMXTIPEVE, CAN, COL | [CMXsrv_icrd_dat_liq_ope](#cmxsrv_icrd_dat_liq_ope) |
| MNEGCONT_Click | COL, NEG, CRD, COD | [CMXsrv_icrd_cont_neg](#cmxsrv_icrd_cont_neg) |
| MNEGELI_CLICK | CRD, COM, NEG, CND, NEG_ADI, ACMXTXTSWF, comex..COL | [CMXsrv_icrd_eli_neg](#cmxsrv_icrd_eli_neg) |
| precarga_datos | COR, TAS, CRD, CUO, CNEG, COM, NEG, TRSD, DIS, EVE, ACMXMONEDA, ACMXINTERE, ACMXSUCSAL, COL | [CMXsrv_icrd_a_rec_age](#cmxsrv_icrd_a_rec_age) |
| precarga_datos | CLN | [CMXsrv_busc_ofi_cta](#cmxsrv_busc_ofi_cta) |
| Form_Load | ACMXSUCSAL, ACMXDL3475FEC, tbl_User | [CMXsrv_trae_glo_fec](#cmxsrv_trae_glo_fec) |
| Form_Load | COL | [CMXsrv_icrd_lee_num_col](#cmxsrv_icrd_lee_num_col) |
| Form_Load | CAN | [CMXsrv_icrd_bus_pago](#cmxsrv_icrd_bus_pago) |

---

## NNEGO
<a name="nnego" ></a>

| **Segmento** | **Tabla Referenciada** | **Procedimiento Almacenado** |
|-------------|----------------------|--------------------------|
| Form_Activate | NEG, COL | [CMXsrv_icrd_neg_lee_crd](#cmxsrv_icrd_neg_lee_crd) |
| Form_Activate | TAS, CRD, ACMXFINVER, NEG, NEG_ADI, DIS, COL | [CMXsrv_icrd_lee_neg](#cmxsrv_icrd_lee_neg) |
| gen_mens_swift | switxt, switxt1 | [CMXsrv_iswf_a_pru](#cmxsrv_iswf_a_pru) |
| llama_pagos | CCL, COL, TAS | [CMXsrv_icrd_lee_col](#cmxsrv_icrd_lee_col) |
| Mnegavi9_Click | switxt, switxt1 | [CMXsrv_iswf_a_pru](#cmxsrv_iswf_a_pru) |
| MNEGCONT_Click | COL, NEG, CRD, COD | [CMXsrv_icrd_cont_neg](#cmxsrv_icrd_cont_neg) |
| MNEGELI_CLICK | CRD, COM, NEG, CND, NEG_ADI, ACMXTXTSWF, comex..COL | [CMXsrv_icrd_eli_neg](#cmxsrv_icrd_eli_neg) |
| pertas_Click | CCL, COL, TAS | [CMXsrv_icrd_lee_col](#cmxsrv_icrd_lee_col) |
| Form_Activate | NEG | [CMXsrv_icrd_busc_neg](#cmxsrv_icrd_busc_neg) |
| Form_Load | comex..EMB, comex..MEMB | [CMXsrv_icrd_busc_emb](#cmxsrv_icrd_busc_emb) |
| ACEPTAR_Click | TAS, CNEG, NEG, COL, DOCNEG | [CMXsrv_icrd_a_neg_emb1](#cmxsrv_icrd_a_neg_emb1) |
| ACEPTAR_Click | NEG, COL, comex..COL, DOCNEG | [CMXsrv_icrd_a_neg_emb2](#cmxsrv_icrd_a_neg_emb2) |
| CANCELAR_Click | COL, DOCNEG | [CMXsrv_icrd_eli_doc_neg](#cmxsrv_icrd_eli_doc_neg) |
| Form_Activate | CRS, COL, EMB | [CMXsrv_icrd_lee_emb1](#cmxsrv_icrd_lee_emb1) |
| Form_Activate | COL, EMB | [CMXsrv_icrd_lee_emb2](#cmxsrv_icrd_lee_emb2) |
| Form_Activate | COL, NEG | [CMXsrv_icrd_lee_neg_emb1](#cmxsrv_icrd_lee_neg_emb1) |
| Form_Activate | COL, NEG | [CMXsrv_icrd_lee_neg_emb2](#cmxsrv_icrd_lee_neg_emb2) |
| Form_Activate | MMCND, COL, CND | [CMXsrv_icrd_lee_cnd_esp](#cmxsrv_icrd_lee_cnd_esp) |
| Form_Activate | MMER, MER | [CMXsrv_icrd_lee_desc_merc](#cmxsrv_icrd_lee_desc_merc) |
| ACEPTAR_Click | COL, DIS, NEG | [CMXsrv_icrd_a_neg_disc](#cmxsrv_icrd_a_neg_disc) |
| Form_Load | DIS, NEG | [CMXsrv_icrd_neg_lee_disc](#cmxsrv_icrd_neg_lee_disc) |
| ACEPTAR_Click | COL, NEG, comex..COL | [CMXsrv_icrd_ent_doc](#cmxsrv_icrd_ent_doc) |
| ELIMINAR_Click | COL, NEG, comex..COL | [CMXsrv_icrd_ent_doc](#cmxsrv_icrd_ent_doc) |
| Form_Load | COL, NEG, comex..COL | [CMXsrv_icrd_ent_doc](#cmxsrv_icrd_ent_doc) |
| ACEPTAR_Click | comex..ACMXINTEREFEC, COR, TAS, CRD, CUO, COD, CNEG, NEG, ACMXMONEDAFEC, NEG_ADI, ACMXINTERE, ACMXBCOUSU, ACMXINTEREFEC, sysobjects, COL | [CMXsrv_icrd_alz_disc](#cmxsrv_icrd_alz_disc) |
| aceptar_click | COR, ACMXMONEDAFEC, CRD, LCR | [CMXCRDsrv_icrd_asignar_cor](#cmxcrdsrv_icrd_asignar_cor) |
| BUSCAR_Click | COR | [CMXCRDsrv_icrd_bus_lcr_bco](#cmxcrdsrv_icrd_bus_lcr_bco) |
| proximo_Click | COR | [CMXCRDsrv_icrd_bus_lcr_bco](#cmxcrdsrv_icrd_bus_lcr_bco) |
| ACEPTAR_Click | NEG, COL, DOCNEG | [CMXsrv_icrd_act_doc_neg](#cmxsrv_icrd_act_doc_neg) |
| Form_Load | NEG, EMB | [CMXsrv_icrd_lee_doc_neg](#cmxsrv_icrd_lee_doc_neg) |
| enviar_Click | switxt, switxt1 | [CMXsrv_iswf_a_pru](#cmxsrv_iswf_a_pru) |
| Form_Load | DDI, COR, ADI, TAS, CUO, NEG, ACMXMONEDAFEC, DAC, ACMXINTERE, ACMXMONEDA, ACMXSIGGAR, ACMXINTEREFEC, CAN, DIS, warnmsg, AVAL, COL, CCO | [CMXsrv_icrd_val_neg](#cmxsrv_icrd_val_neg) |
| Form_Load |  | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |
| Form_Load | CAN | [CMXsrv_icrd_bus_pago](#cmxsrv_icrd_bus_pago) |

---

## PAGCBR
<a name="pagcbr" ></a>

| **Segmento** | **Tabla Referenciada** | **Procedimiento Almacenado** |
|-------------|----------------------|--------------------------|
| ACEPTAR_Click | ACMXMONEDAFEC, CBR, ACMXPRMENL | [CMXsrv_icbr_lee_dat_var](#cmxsrv_icbr_lee_dat_var) |
| ACEPTAR_Click | LCB, CBR, CCO | [CMXsrv_icbr_val_pag](#cmxsrv_icbr_val_pag) |
| ACEPTAR_Click | LCB, ACMXDESEMB, vig_cmx, COD, ICX, COM, ACMXMONEDAFEC, CBR, PCX, DIP, LIB, CLN, CCO | [CMXsrv_icbr_ctb_pag](#cmxsrv_icbr_ctb_pag) |
| Calcular_Click | DDI, ADI, ACMXMONEDAFEC, CBR, COB, ACMXMONEDA | [CMXsrv_icbr_cal_pag](#cmxsrv_icbr_cal_pag) |
| CANCELAR_Click | ECE, PCX, COB, ICX | [CMXsrv_icbr_eli_pag](#cmxsrv_icbr_eli_pag) |
| fld_cbr_cod_des_mn_pag_lostfocus | ACMXPLNCTAN, ACMXDESEMB, ACMXPLNCTAX | [CMXsrv_val_vig](#cmxsrv_val_vig) |
| fld_cbr_cod_des_mx_pag_lostfocus | ACMXPLNCTAN, ACMXDESEMB, ACMXPLNCTAX | [CMXsrv_val_vig](#cmxsrv_val_vig) |
| Form_Load | ACMXMONEDA, CBR | [CMXsrv_icbr_lee_cbr0](#cmxsrv_icbr_lee_cbr0) |
| Form_Load |  | [CMXsrv_icbr_obt_mon_nac](#cmxsrv_icbr_obt_mon_nac) |
| Form_Load | ACMXDESEMB, ECE, PCX, CBR | [CMXsrv_icbr_lee_dat_pag](#cmxsrv_icbr_lee_dat_pag) |
| Form_Load | ACMXMONEDAFEC, CBR | [CMXsrv_icbr_pcg_pag](#cmxsrv_icbr_pcg_pag) |
| lee_cta | ACMXPLNCTAN, ACMXDESEMB, ACMXPLNCTAX | [CMXsrv_vig_lee_cta](#cmxsrv_vig_lee_cta) |
| Form_Activate | PCX | [CMXsrv_icbr_busc_pago](#cmxsrv_icbr_busc_pago) |
| ACEPTAR_Click | LCB, CBR, CCO | [CMXsrv_icbr_val_pag](#cmxsrv_icbr_val_pag) |
| Aceptar_Click | ACMXMONEDAFEC, COB | [CMXsrv_icob_act_val](#cmxsrv_icob_act_val) |
| Form_Activate | COB | [CMXsrv_icob_lee_val](#cmxsrv_icob_lee_val) |
| ELIMINAR_Click | PCX, ICX | [CMXsrv_icbr_eli_int_pago](#cmxsrv_icbr_eli_int_pago) |
| Form_Activate | ICX | [CMXsrv_icbr_busc_int](#cmxsrv_icbr_busc_int) |
| Aceptar_Click | PCX, CBR, ICX, ACMXINTEREFEC | [CMXsrv_icbr_ingmod_int](#cmxsrv_icbr_ingmod_int) |
| Form_Activate | ICX | [CMXsrv_icbr_lee_int_pago](#cmxsrv_icbr_lee_int_pago) |
| Aceptar_Click | ACMXPAIS, COR | [CMXsrv_icbr_lee_bco](#cmxsrv_icbr_lee_bco) |
| buscar_Click | COR | [CMXsrv_icbr_busc_bco](#cmxsrv_icbr_busc_bco) |
| Form_Load |  | [CMXsrv_grl_fec_serv](#cmxsrv_grl_fec_serv) |

---

# Procedimientos Referenciados

## CMXsrv_expcbe_lee_prm
<a name="cmxsrv_expcbe_lee_prm" ></a>

**Procedimientos Referenciados:**

- sp_procxmode
- CMXsrv_lee_fpro

---

## CMXsrv_cmx_busc_suc_usu
<a name="cmxsrv_cmx_busc_suc_usu" ></a>

**Procedimientos Referenciados:**

- PrmACMXSUCSAL
- CMXsrv_cmx_ing_lib
- sp_procxmode

---

## CMXsrv_expcbe_lee_cbe
<a name="cmxsrv_expcbe_lee_cbe" ></a>

**Procedimientos Referenciados:**

- CMXsrv_cmx_busc_suc_usu
- CMXsrv_val_suc
- sp_procxmode
- CMXsrv_lee_fpro

---

## CMXsrv_trae_glo_fec
<a name="cmxsrv_trae_glo_fec" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcbe_avs_cyg1
<a name="cmxsrv_expcbe_avs_cyg1" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcbe_avs_cyg2
<a name="cmxsrv_expcbe_avs_cyg2" ></a>

**Procedimientos Referenciados:**

- por
- sp_procxmode

---

## CMXsrv_expcbe_avs_ret
<a name="cmxsrv_expcbe_avs_ret" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcbe_swf_sel
<a name="cmxsrv_expcbe_swf_sel" ></a>

**Procedimientos Referenciados:**

- CMXsrv_expcbe_swf_422
- CMXsrv_expcbe_swf_420
- CMXsrv_expcbe_swf_499
- CMXsrv_expcbe_swf_430
- sp_procxmode

---

## CMXsrv_expcbe_anl_cbe
<a name="cmxsrv_expcbe_anl_cbe" ></a>

**Procedimientos Referenciados:**

- CMXsrv_cnt_gen_vig
- sp_procxmode
- CMXsrv_expcbe_grb_evz
- CMXsrv_cnt_950
- CMXsrv_cnt_630

---

## CMXsrv_expcbe_ctb_ing
<a name="cmxsrv_expcbe_ctb_ing" ></a>

**Procedimientos Referenciados:**

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

## CMXsrv_expcbe_del_cbe
<a name="cmxsrv_expcbe_del_cbe" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcbe_val_cbe
<a name="cmxsrv_expcbe_val_cbe" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcbe_grb_ctp
<a name="cmxsrv_expcbe_grb_ctp" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcbe_lee_cln
<a name="cmxsrv_expcbe_lee_cln" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_val_suc
<a name="cmxsrv_val_suc" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcbe_lee_ctp
<a name="cmxsrv_expcbe_lee_ctp" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcbe_grb_bco
<a name="cmxsrv_expcbe_grb_bco" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcbe_lee_cor
<a name="cmxsrv_expcbe_lee_cor" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcbe_lee_bco
<a name="cmxsrv_expcbe_lee_bco" ></a>

**Procedimientos Referenciados:**

- CMXsrv_icrd_lee_cln
- sp_procxmode

---

## CMXsrv_expcbe_grb_doc
<a name="cmxsrv_expcbe_grb_doc" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcbe_grb_doc02
<a name="cmxsrv_expcbe_grb_doc02" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcbe_lee_doc
<a name="cmxsrv_expcbe_lee_doc" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcbe_lee_doc02
<a name="cmxsrv_expcbe_lee_doc02" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcbe_del_ctz
<a name="cmxsrv_expcbe_del_ctz" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcbe_bus_ctz
<a name="cmxsrv_expcbe_bus_ctz" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcbe_grb_ctz
<a name="cmxsrv_expcbe_grb_ctz" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcbe_mto_ctz
<a name="cmxsrv_expcbe_mto_ctz" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcbe_lee_ctz
<a name="cmxsrv_expcbe_lee_ctz" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcbe_bus_cbe
<a name="cmxsrv_expcbe_bus_cbe" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcbe_mdf_cbe
<a name="cmxsrv_expcbe_mdf_cbe" ></a>

**Procedimientos Referenciados:**

- CMXsrv_expcbe_grb_evl
- CMXsrv_expcbe_act_ctz
- CMXsrv_cnt_gen_vig
- CMXsrv_cnt_610
- sp_procxmode
- CMXsrv_expcbe_grb_evz
- CMXsrv_cnt_950
- CMXsrv_lee_fpro

---

## CMXsrv_expcbe_cre_actz
<a name="cmxsrv_expcbe_cre_actz" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcbe_lee_mdf
<a name="cmxsrv_expcbe_lee_mdf" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcbe_pgo_cbe
<a name="cmxsrv_expcbe_pgo_cbe" ></a>

**Procedimientos Referenciados:**

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

## CMXsrv_expcbe_lee_pgo
<a name="cmxsrv_expcbe_lee_pgo" ></a>

**Procedimientos Referenciados:**

- sp_procxmode
- CMXsrv_lee_fpro

---

## CMXsrv_expcbe_bus_evz
<a name="cmxsrv_expcbe_bus_evz" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcbe_rev_cbe
<a name="cmxsrv_expcbe_rev_cbe" ></a>

**Procedimientos Referenciados:**

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

## CMXsrv_expcbe_lee_evz
<a name="cmxsrv_expcbe_lee_evz" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcbe_del_dcz
<a name="cmxsrv_expcbe_del_dcz" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcbe_bus_dcz
<a name="cmxsrv_expcbe_bus_dcz" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcbe_grb_dcz
<a name="cmxsrv_expcbe_grb_dcz" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcbe_lee_dcz
<a name="cmxsrv_expcbe_lee_dcz" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcbe_bus_vto
<a name="cmxsrv_expcbe_bus_vto" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_avi_dat_cou
<a name="cmxsrv_avi_dat_cou" ></a>

**Procedimientos Referenciados:**

- sp_procxmode
- CMXsrv_avigrl_crea_avitemp
- bcicomex

---

## CMXsrv_expcbe_avs_rem1
<a name="cmxsrv_expcbe_avs_rem1" ></a>

**Procedimientos Referenciados:**

- sp_procxmode
- CMXsrv_trae_glo_fec
- CMXsrv_expcbe_val_cbe
- CMXsrv_util_fmt_txt

---

## CMXsrv_expcbe_avs_rem3
<a name="cmxsrv_expcbe_avs_rem3" ></a>

**Procedimientos Referenciados:**

- CMXsrv_util_fmt_txt
- sp_procxmode

---

## CMXsrv_expcbe_avs_rem2
<a name="cmxsrv_expcbe_avs_rem2" ></a>

**Procedimientos Referenciados:**

- sp_procxmode
- CMXsrv_expcbe_for_lin

---

## CMXsrv_expcbe_avs_rem4
<a name="cmxsrv_expcbe_avs_rem4" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_busc_plz
<a name="cmxsrv_busc_plz" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_lee_plz
<a name="cmxsrv_lee_plz" ></a>

**Procedimientos Referenciados:**

- CMXsrv_mbyte_cmp
- sp_procxmode

---

## CMXsrv_cor_busc_pais
<a name="cmxsrv_cor_busc_pais" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_cor_lee_pais
<a name="cmxsrv_cor_lee_pais" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcbe_bus_cor
<a name="cmxsrv_expcbe_bus_cor" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_busc_bco_mtr
<a name="cmxsrv_busc_bco_mtr" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_grl_fec_serv
<a name="cmxsrv_grl_fec_serv" ></a>

**Procedimientos Referenciados:**

- SRV_MessageService
- sp_procxmode

---

## CMXsrv_expcce_lee_cce
<a name="cmxsrv_expcce_lee_cce" ></a>

**Procedimientos Referenciados:**

- por
- sp_procxmode

---

## CMXsrv_expcce_trd_cce
<a name="cmxsrv_expcce_trd_cce" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcce_anl_cce
<a name="cmxsrv_expcce_anl_cce" ></a>

**Procedimientos Referenciados:**

- CMXsrv_cmx_lee_trs
- sp_procxmode
- CMXsrv_expcce_grb_evc
- CMXsrv_expcce_ictb_anu
- CMXsrv_cnt_950
- CMXsrv_cnt_740
- CMXsrv_expcce_lee_fpro

---

## CMXsrv_expcce_ctb_ing
<a name="cmxsrv_expcce_ctb_ing" ></a>

**Procedimientos Referenciados:**

- CMXsrv_mbyte_gen
- sp_procxmode
- CMXsrv_expcce_val_cce
- CMXsrv_expcce_grb_evc
- CMXsrv_cnt_950
- CMXsrv_cnt_700

---

## CMXsrv_expcce_del_cce
<a name="cmxsrv_expcce_del_cce" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcce_val_cce
<a name="cmxsrv_expcce_val_cce" ></a>

**Procedimientos Referenciados:**

- CMXsrv_cmx_get_codes
- sp_procxmode

---

## CMXsrv_expcce_swf_sel
<a name="cmxsrv_expcce_swf_sel" ></a>

**Procedimientos Referenciados:**

- CMXsrv_expcce_swf_730
- CMXsrv_expcce_swf_742
- sp_procxmode

---

## CMXsrv_expcce_grb_bco
<a name="cmxsrv_expcce_grb_bco" ></a>

**Procedimientos Referenciados:**

- sp_procxmode
- CMXsrv_expcce_lee_fpro

---

## CMXsrv_expcce_lee_cor
<a name="cmxsrv_expcce_lee_cor" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcce_lee_bco
<a name="cmxsrv_expcce_lee_bco" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcce_grb_ctp
<a name="cmxsrv_expcce_grb_ctp" ></a>

**Procedimientos Referenciados:**

- sp_procxmode
- CMXsrv_expcce_lee_fpro

---

## CMXsrv_expcce_lee_cln
<a name="cmxsrv_expcce_lee_cln" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcce_lee_ctp
<a name="cmxsrv_expcce_lee_ctp" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcce_cre_cce
<a name="cmxsrv_expcce_cre_cce" ></a>

**Procedimientos Referenciados:**

- CMXsrv_util_num_ope
- CMXsrv_cmx_busc_suc_usu
- sp_procxmode
- CMXsrv_expcce_lee_fpro

---

## CMXsrv_expcce_gen_dcc
<a name="cmxsrv_expcce_gen_dcc" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcce_grb_cnd
<a name="cmxsrv_expcce_grb_cnd" ></a>

**Procedimientos Referenciados:**

- sp_procxmode
- CMXsrv_expcce_lee_fpro

---

## CMXsrv_util_det_habil
<a name="cmxsrv_util_det_habil" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcce_lee_cnd
<a name="cmxsrv_expcce_lee_cnd" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcce_trd_cnd
<a name="cmxsrv_expcce_trd_cnd" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcce_del_dcc
<a name="cmxsrv_expcce_del_dcc" ></a>

**Procedimientos Referenciados:**

- sp_procxmode
- CMXsrv_expcce_lee_fpro

---

## CMXsrv_expcce_bus_dcc
<a name="cmxsrv_expcce_bus_dcc" ></a>

**Procedimientos Referenciados:**

- CMXsrv_expcce_gen_adcc
- sp_procxmode

---

## CMXsrv_expcce_grb_dcc
<a name="cmxsrv_expcce_grb_dcc" ></a>

**Procedimientos Referenciados:**

- sp_procxmode
- CMXsrv_expcce_lee_fpro

---

## CMXsrv_expcce_lee_dcc
<a name="cmxsrv_expcce_lee_dcc" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcce_bus_cce
<a name="cmxsrv_expcce_bus_cce" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcce_mdf_cce
<a name="cmxsrv_expcce_mdf_cce" ></a>

**Procedimientos Referenciados:**

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

## CMXsrv_expcce_can_mdf
<a name="cmxsrv_expcce_can_mdf" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcce_lee_mdf
<a name="cmxsrv_expcce_lee_mdf" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcce_cnf_cce
<a name="cmxsrv_expcce_cnf_cce" ></a>

**Procedimientos Referenciados:**

- CMXsrv_cnt_710
- sp_procxmode
- CMXsrv_expcce_ictb_cexp
- CMXsrv_expcce_grb_evc
- CMXsrv_cnt_950
- CMXsrv_expcce_lee_fpro

---

## CMXsrv_expcce_grb_afin
<a name="cmxsrv_expcce_grb_afin" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcce_lee_cnf
<a name="cmxsrv_expcce_lee_cnf" ></a>

**Procedimientos Referenciados:**

- sp_procxmode
- CMXsrv_expcce_lee_fpro

---

## CMXsrv_expcce_lee_afin
<a name="cmxsrv_expcce_lee_afin" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcce_trp_cce
<a name="cmxsrv_expcce_trp_cce" ></a>

**Procedimientos Referenciados:**

- sp_procxmode
- CMXsrv_cnt_730
- CMXsrv_expcce_grb_evc
- CMXsrv_cnt_950

---

## CMXsrv_expcce_lee_trp
<a name="cmxsrv_expcce_lee_trp" ></a>

**Procedimientos Referenciados:**

- sp_procxmode
- CMXsrv_expcce_lee_fpro

---

## CMXsrv_expcce_bus_evc
<a name="cmxsrv_expcce_bus_evc" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcce_rev_cce
<a name="cmxsrv_expcce_rev_cce" ></a>

**Procedimientos Referenciados:**

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

## CMXsrv_expcce_lee_evc
<a name="cmxsrv_expcce_lee_evc" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcce_avs_rem1
<a name="cmxsrv_expcce_avs_rem1" ></a>

**Procedimientos Referenciados:**

- CMXsrv_trae_glo_fec
- sp_procxmode

---

## CMXsrv_expcce_bus_cor
<a name="cmxsrv_expcce_bus_cor" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_dex_lee_dex
<a name="cmxsrv_dex_lee_dex" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_dex_eli_dex
<a name="cmxsrv_dex_eli_dex" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_dex_act_dex
<a name="cmxsrv_dex_act_dex" ></a>

**Procedimientos Referenciados:**

- CMXsrv_exppln_get_dig
- sp_procxmode
- CMXsrv_lee_fpro

---

## CMXsrv_expdex_cal_fec
<a name="cmxsrv_expdex_cal_fec" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_dex_lee_cli
<a name="cmxsrv_dex_lee_cli" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_dex_bus_dex
<a name="cmxsrv_dex_bus_dex" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcce_lee_bas
<a name="cmxsrv_expcce_lee_bas" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcce_lee_neg
<a name="cmxsrv_expcce_lee_neg" ></a>

**Procedimientos Referenciados:**

- CMXsrv_cmx_busc_suc_usu
- sp_procxmode

---

## CMXsrv_expcce_alz_dis
<a name="cmxsrv_expcce_alz_dis" ></a>

**Procedimientos Referenciados:**

- CMXsrv_expcce_ctb_alz
- CMXsrv_cnt_760
- sp_procxmode
- CMXsrv_expcce_grb_evc
- CMXsrv_cnt_950
- CMXsrv_expcce_get_tip_ope
- CMXsrv_expcce_lee_fpro

---

## CMXsrv_expcce_anl_neg
<a name="cmxsrv_expcce_anl_neg" ></a>

**Procedimientos Referenciados:**

- CMXsrv_cmx_lee_trs
- sp_procxmode
- CMXsrv_cnt_780
- CMXsrv_expcce_grb_evc
- CMXsrv_expcce_ictb_anu
- CMXsrv_cnt_950
- CMXsrv_expcce_lee_fpro

---

## CMXsrv_expcce_ctb_neg
<a name="cmxsrv_expcce_ctb_neg" ></a>

**Procedimientos Referenciados:**

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

## CMXsrv_expcce_del_neg
<a name="cmxsrv_expcce_del_neg" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcce_val_neg
<a name="cmxsrv_expcce_val_neg" ></a>

**Procedimientos Referenciados:**

- CMXsrv_util_fecha
- sp_procxmode

---

## CMXsrv_expcce_grb_neg
<a name="cmxsrv_expcce_grb_neg" ></a>

**Procedimientos Referenciados:**

- CMXsrv_cmx_busc_suc_usu
- sp_procxmode
- CMXsrv_expcce_lee_fpro

---

## CMXsrv_expcce_gen_dcn
<a name="cmxsrv_expcce_gen_dcn" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcce_avs_rem5
<a name="cmxsrv_expcce_avs_rem5" ></a>

**Procedimientos Referenciados:**

- CMX_srv_pone_punto
- CMXsrv_util_fmt_txt
- sp_procxmode
- CMXsrv_expcce_get_ing_esp

---

## CMXsrv_expcce_lee_nge
<a name="cmxsrv_expcce_lee_nge" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcce_trd_nge
<a name="cmxsrv_expcce_trd_nge" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcce_ini_neg
<a name="cmxsrv_expcce_ini_neg" ></a>

**Procedimientos Referenciados:**

- sp_procxmode
- CMXsrv_expcce_lee_fpro

---

## CMXsrv_expcce_del_dcn
<a name="cmxsrv_expcce_del_dcn" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcce_bus_dcn
<a name="cmxsrv_expcce_bus_dcn" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcce_grb_dcn
<a name="cmxsrv_expcce_grb_dcn" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcce_lee_dcn
<a name="cmxsrv_expcce_lee_dcn" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcce_del_ltr
<a name="cmxsrv_expcce_del_ltr" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcce_bus_ltr
<a name="cmxsrv_expcce_bus_ltr" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcce_grb_ltr
<a name="cmxsrv_expcce_grb_ltr" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcce_lee_ltr
<a name="cmxsrv_expcce_lee_ltr" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcce_del_dsn
<a name="cmxsrv_expcce_del_dsn" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcce_gen_dsn
<a name="cmxsrv_expcce_gen_dsn" ></a>

**Procedimientos Referenciados:**

- CMXsrv_expcce_grb_dsn
- sp_procxmode

---

## CMXsrv_expcce_bus_dsn
<a name="cmxsrv_expcce_bus_dsn" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcce_chk_dsn
<a name="cmxsrv_expcce_chk_dsn" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcce_grb_dsn
<a name="cmxsrv_expcce_grb_dsn" ></a>

**Procedimientos Referenciados:**

- sp_procxmode
- CMXsrv_expcce_chk_dsn

---

## CMXsrv_expcce_lee_dsn
<a name="cmxsrv_expcce_lee_dsn" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcce_bus_neg
<a name="cmxsrv_expcce_bus_neg" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcce_pgo_neg
<a name="cmxsrv_expcce_pgo_neg" ></a>

**Procedimientos Referenciados:**

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

## CMXsrv_expcce_lee_pgo
<a name="cmxsrv_expcce_lee_pgo" ></a>

**Procedimientos Referenciados:**

- sp_procxmode
- CMXsrv_expcce_lee_fpro

---

## CMXsrv_expcce_avs_rem3
<a name="cmxsrv_expcce_avs_rem3" ></a>

**Procedimientos Referenciados:**

- CMXsrv_util_fmt_txt
- sp_procxmode

---

## CMXsrv_expcce_avs_rem2
<a name="cmxsrv_expcce_avs_rem2" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expcce_avs_rem4
<a name="cmxsrv_expcce_avs_rem4" ></a>

**Procedimientos Referenciados:**

- CMXsrv_util_fmt_txt
- sp_procxmode

---

## CMXsrv_expret_swf_sel
<a name="cmxsrv_expret_swf_sel" ></a>

**Procedimientos Referenciados:**

- CMXsrv_expret_swf_202
- CMXsrv_expret_swf_100
- sp_procxmode

---

## CMXsrv_expret_lee_ret
<a name="cmxsrv_expret_lee_ret" ></a>

**Procedimientos Referenciados:**

- CMXsrv_cmx_busc_suc_usu
- sp_procxmode
- CMXsrv_lee_fpro

---

## CMXsrv_expret_lee_prm
<a name="cmxsrv_expret_lee_prm" ></a>

**Procedimientos Referenciados:**

- sp_procxmode
- CMXsrv_lee_fpro

---

## CMXsrv_expret_avs_cyg1
<a name="cmxsrv_expret_avs_cyg1" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expret_avs_cyg2
<a name="cmxsrv_expret_avs_cyg2" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expret_avs_liq1
<a name="cmxsrv_expret_avs_liq1" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expret_avs_liq2
<a name="cmxsrv_expret_avs_liq2" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expret_avs_liq3
<a name="cmxsrv_expret_avs_liq3" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expret_val_ret
<a name="cmxsrv_expret_val_ret" ></a>

**Procedimientos Referenciados:**

- CMXsrv_val_cta_cte
- sp_procxmode
- CMXsrv_enl_val_sel
- CMXsrv_val_vig
- CMXsrv_util_len
- CMXsrv_lee_fpro

---

## CMXsrv_expret_sum_dtn_mn
<a name="cmxsrv_expret_sum_dtn_mn" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expret_ctb_ing
<a name="cmxsrv_expret_ctb_ing" ></a>

**Procedimientos Referenciados:**

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

## CMXsrv_expret_del_ret
<a name="cmxsrv_expret_del_ret" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expret_avs_adm1
<a name="cmxsrv_expret_avs_adm1" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expret_avs_adm2
<a name="cmxsrv_expret_avs_adm2" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expret_avs_adm3
<a name="cmxsrv_expret_avs_adm3" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expret_act_tpo_cbo
<a name="cmxsrv_expret_act_tpo_cbo" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expret_cre_ret
<a name="cmxsrv_expret_cre_ret" ></a>

**Procedimientos Referenciados:**

- CMXsrv_util_num_ope
- CMXsrv_cmx_busc_suc_usu
- sp_procxmode
- CMXsrv_lee_fpro

---

## CMXsrv_expret_grb_det
<a name="cmxsrv_expret_grb_det" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expret_tpo_cbo
<a name="cmxsrv_expret_tpo_cbo" ></a>

**Procedimientos Referenciados:**

- sp_procxmode
- CMXsrv_lee_fpro

---

## CMXsrv_expret_lee_cln
<a name="cmxsrv_expret_lee_cln" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expret_lee_det
<a name="cmxsrv_expret_lee_det" ></a>

**Procedimientos Referenciados:**

- sp_procxmode
- CMXsrv_lee_fpro

---

## CMXsrv_expret_del_org
<a name="cmxsrv_expret_del_org" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expret_bus_org
<a name="cmxsrv_expret_bus_org" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expret_grb_org
<a name="cmxsrv_expret_grb_org" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expret_mto_org
<a name="cmxsrv_expret_mto_org" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expret_lee_org
<a name="cmxsrv_expret_lee_org" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_vig_lee_cta
<a name="cmxsrv_vig_lee_cta" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expret_del_dtn
<a name="cmxsrv_expret_del_dtn" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expret_bus_dtn
<a name="cmxsrv_expret_bus_dtn" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expret_grb_dtn
<a name="cmxsrv_expret_grb_dtn" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expret_cal_arb
<a name="cmxsrv_expret_cal_arb" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expret_mto_dtn
<a name="cmxsrv_expret_mto_dtn" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expret_lee_dtn
<a name="cmxsrv_expret_lee_dtn" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expret_bus_ret
<a name="cmxsrv_expret_bus_ret" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expret_bus_evr
<a name="cmxsrv_expret_bus_evr" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_expret_rev_ret
<a name="cmxsrv_expret_rev_ret" ></a>

**Procedimientos Referenciados:**

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

## CMXsrv_expret_lee_evr
<a name="cmxsrv_expret_lee_evr" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_finadm_imod_desti
<a name="cmxsrv_finadm_imod_desti" ></a>

**Procedimientos Referenciados:**

- CMXsrv_finadm_val_tipop
- sp_procxmode

---

## CMXsrv_finadm_cons_dtip
<a name="cmxsrv_finadm_cons_dtip" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_finadm_imod_ectb
<a name="cmxsrv_finadm_imod_ectb" ></a>

**Procedimientos Referenciados:**

- CMXsrv_finadm_val_tipop
- sp_procxmode

---

## CMXsrv_finadm_eli_tipop
<a name="cmxsrv_finadm_eli_tipop" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_finadm_cons_ectb
<a name="cmxsrv_finadm_cons_ectb" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_finadm_imod_itip
<a name="cmxsrv_finadm_imod_itip" ></a>

**Procedimientos Referenciados:**

- CMXsrv_finadm_val_tipop
- sp_procxmode

---

## CMXsrv_finadm_cons_itip
<a name="cmxsrv_finadm_cons_itip" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_finadm_lee_tipop
<a name="cmxsrv_finadm_lee_tipop" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_finadm_val_tipop
<a name="cmxsrv_finadm_val_tipop" ></a>

**Procedimientos Referenciados:**

- CMXsrv_fincol_eval_tbat
- CMXsrv_util_fecha2
- SRV_MessageService
- sp_procxmode

---

## CMXsrv_finadm_bus_tipope
<a name="cmxsrv_finadm_bus_tipope" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_busc_tip_tas
<a name="cmxsrv_busc_tip_tas" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_fincol_ecuo
<a name="cmxsrv_fincol_ecuo" ></a>

**Procedimientos Referenciados:**

- CMXsrv_fincol_pre_cuad_tas
- sp_procxmode

---

## CMXsrv_fincol_cons_plnpa
<a name="cmxsrv_fincol_cons_plnpa" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_pertas_val_display
<a name="cmxsrv_pertas_val_display" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_fincol_eava
<a name="cmxsrv_fincol_eava" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_fincol_cons_aval
<a name="cmxsrv_fincol_cons_aval" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_fincol_iava
<a name="cmxsrv_fincol_iava" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_fincol_cons_pag
<a name="cmxsrv_fincol_cons_pag" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_fincol_trae_det_pag
<a name="cmxsrv_fincol_trae_det_pag" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_fincol_cons_pror
<a name="cmxsrv_fincol_cons_pror" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_fincol_cons_eve
<a name="cmxsrv_fincol_cons_eve" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_lee_bco_swf
<a name="cmxsrv_icrd_lee_bco_swf" ></a>

**Procedimientos Referenciados:**

- CMXsrv_icrd_lee_cln
- sp_procxmode

---

## CMXsrv_icrd_busc_bco
<a name="cmxsrv_icrd_busc_bco" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_fincol_vtocre_prov
<a name="cmxsrv_fincol_vtocre_prov" ></a>

**Procedimientos Referenciados:**

- CMXsrv_fincol_gpln
- CMXsrv_finobl_imod_obl
- CMXsrv_util_fecha
- CMXsrv_util_val_tasas
- CMXsrv_fincol_efec_calpa
- sp_procxmode
- CMXsrv_fincol_ctb_vcp
- sp_cmx_sii_1870

---

## CMXsrv_fincol_prec_vtocre
<a name="cmxsrv_fincol_prec_vtocre" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_bus_lcr_bco
<a name="cmxsrv_icrd_bus_lcr_bco" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_lee_fpro
<a name="cmxsrv_lee_fpro" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_fincol_ren_fin
<a name="cmxsrv_fincol_ren_fin" ></a>

**Procedimientos Referenciados:**

- CMXsrv_cmx_fec_hoy
- CMXsrv_fincol_pre_cuad_tas
- sp_procxmode
- CMXsrv_fincol_grb_col_ren
- CMXsrv_lee_fpro

---

## CMXsrv_fincol_gmod_ctr
<a name="cmxsrv_fincol_gmod_ctr" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_fincol_lee_bco
<a name="cmxsrv_fincol_lee_bco" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_fincol_lee_cln
<a name="cmxsrv_fincol_lee_cln" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_fincol_cons_ctr
<a name="cmxsrv_fincol_cons_ctr" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_fincol_ctb_oto
<a name="cmxsrv_fincol_ctb_oto" ></a>

**Procedimientos Referenciados:**

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

## CMXsrv_icrd_dat_liq_ope
<a name="cmxsrv_icrd_dat_liq_ope" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_fincol_lee_col
<a name="cmxsrv_fincol_lee_col" ></a>

**Procedimientos Referenciados:**

- PrmACMXESPECI
- PrmACLNEJECTA
- sp_procxmode

---

## CMXsrv_busc_cod_ope
<a name="cmxsrv_busc_cod_ope" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_col_trae_num_ope
<a name="cmxsrv_col_trae_num_ope" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_fincol_eli_col
<a name="cmxsrv_fincol_eli_col" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_fincol_val_col
<a name="cmxsrv_fincol_val_col" ></a>

**Procedimientos Referenciados:**

- CMXsrv_fincol_val_err
- CMXsrv_fincol_val_per_tas
- CMXsrv_fincol_val_adv
- sp_procxmode

---

## CMXsrv_fincol_bsc_col
<a name="cmxsrv_fincol_bsc_col" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_fincol_lee_tip
<a name="cmxsrv_fincol_lee_tip" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_fincol_ctb_novf
<a name="cmxsrv_fincol_ctb_novf" ></a>

**Procedimientos Referenciados:**

- CMXsrv_fincol_ctb_nov
- sp_procxmode
- CMXsrv_lee_fpro

---

## CMXsrv_fincol_cons_nov
<a name="cmxsrv_fincol_cons_nov" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_cmx_get_codes
<a name="cmxsrv_cmx_get_codes" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_grl_trae_cod_bco
<a name="cmxsrv_grl_trae_cod_bco" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_fincol_cons_tas
<a name="cmxsrv_fincol_cons_tas" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_fincol_efec_tras
<a name="cmxsrv_fincol_efec_tras" ></a>

**Procedimientos Referenciados:**

- CMXsrv_fincol_ctb_cnd
- CMXsrv_fincol_ctb_cob
- CMXsrv_cnt_9000
- CMXsrv_fincol_ctb_cst
- sp_procxmode
- CMXsrv_fincol_calc_cven

---

## CMXsrv_fincol_cons_trasp
<a name="cmxsrv_fincol_cons_trasp" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_fincol_cons_dtrs
<a name="cmxsrv_fincol_cons_dtrs" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_fincol_cons_deve
<a name="cmxsrv_fincol_cons_deve" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_fincol_cont_gst
<a name="cmxsrv_fincol_cont_gst" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_fincol_cons_gst
<a name="cmxsrv_fincol_cons_gst" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_fincol_cons_dgst
<a name="cmxsrv_fincol_cons_dgst" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_fincol_bsc_tip
<a name="cmxsrv_fincol_bsc_tip" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_finobl_bus_cor
<a name="cmxsrv_finobl_bus_cor" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_finobl_ecuo
<a name="cmxsrv_finobl_ecuo" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_finobl_gpln
<a name="cmxsrv_finobl_gpln" ></a>

**Procedimientos Referenciados:**

- CMXsrv_util_det_habil_tasa
- sp_procxmode

---

## CMXsrv_finobl_cons_plnpa
<a name="cmxsrv_finobl_cons_plnpa" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_finobl_calc_anu
<a name="cmxsrv_finobl_calc_anu" ></a>

**Procedimientos Referenciados:**

- sp_procxmode
- CMXsrv_finobl_efec_calpa
- CMXsrv_lee_fpro

---

## CMXsrv_finobl_lee_obl
<a name="cmxsrv_finobl_lee_obl" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_finobl_ctb_oto
<a name="cmxsrv_finobl_ctb_oto" ></a>

**Procedimientos Referenciados:**

- CMXsrv_ctbo_otorga
- CMXsrv_finobl_val_obl
- sp_procxmode
- CMXsrv_lee_fpro

---

## CMXsrv_fincol_eli_obl
<a name="cmxsrv_fincol_eli_obl" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_finobl_val_obl
<a name="cmxsrv_finobl_val_obl" ></a>

**Procedimientos Referenciados:**

- CMXsrv_util_det_habil_tasa
- CMXsrv_finobl_val_adv
- sp_procxmode

---

## CMXsrv_finobl_bsc_obl
<a name="cmxsrv_finobl_bsc_obl" ></a>

**Procedimientos Referenciados:**

- CMXsrv_finobl_bsc_obl2
- sp_procxmode
- CMXsrv_finobl_bsc_obl3

---

## CMXsrv_finobl_ictb_pag
<a name="cmxsrv_finobl_ictb_pag" ></a>

**Procedimientos Referenciados:**

- CMXsrv_finobl_ctb_pag
- sp_procxmode
- CMXsrv_lee_fpro

---

## CMXsrv_finobl_obt_sdocuo
<a name="cmxsrv_finobl_obt_sdocuo" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_finobl_new_tas
<a name="cmxsrv_finobl_new_tas" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_finobl_cons_pag
<a name="cmxsrv_finobl_cons_pag" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_finobl_cons_detp
<a name="cmxsrv_finobl_cons_detp" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_finobl_calc_pror
<a name="cmxsrv_finobl_calc_pror" ></a>

**Procedimientos Referenciados:**

- sp_procxmode
- CMXsrv_finobl_efec_calpa
- CMXsrv_lee_fpro

---

## CMXsrv_finobl_cons_pror
<a name="cmxsrv_finobl_cons_pror" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_finobl_cons_dpror
<a name="cmxsrv_finobl_cons_dpror" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_finobl_ctb_anu
<a name="cmxsrv_finobl_ctb_anu" ></a>

**Procedimientos Referenciados:**

- CMXsrv_finobl_cbo_anu
- CMXsrv_ctbo_anula
- sp_procxmode
- CMXsrv_lee_fpro

---

## CMXsrv_finobl_cons_anu
<a name="cmxsrv_finobl_cons_anu" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_finobl_cons_mod
<a name="cmxsrv_finobl_cons_mod" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_finobl_cons_dmod
<a name="cmxsrv_finobl_cons_dmod" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_finobl_rev_eve
<a name="cmxsrv_finobl_rev_eve" ></a>

**Procedimientos Referenciados:**

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

## CMXsrv_finobl_cons_eve
<a name="cmxsrv_finobl_cons_eve" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_finobl_cons_deve
<a name="cmxsrv_finobl_cons_deve" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_finobl_eli_ctr
<a name="cmxsrv_finobl_eli_ctr" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_finobl_cons_ctr
<a name="cmxsrv_finobl_cons_ctr" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_finobl_ing_ctr
<a name="cmxsrv_finobl_ing_ctr" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_finobl_cesion_obl
<a name="cmxsrv_finobl_cesion_obl" ></a>

**Procedimientos Referenciados:**

- CMXsrv_ctl_crea_apr
- sp_procxmode
- CMXsrv_lee_fpro

---

## CMXsrv_comgrl_lee_nom_cor
<a name="cmxsrv_comgrl_lee_nom_cor" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_lee_cln
<a name="cmxsrv_lee_cln" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_finobl_busc_acre
<a name="cmxsrv_finobl_busc_acre" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_fincol_efec_calpa
<a name="cmxsrv_fincol_efec_calpa" ></a>

**Procedimientos Referenciados:**

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

## CMXsrv_fincol_cons_detp
<a name="cmxsrv_fincol_cons_detp" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_fincol_calc_pror
<a name="cmxsrv_fincol_calc_pror" ></a>

**Procedimientos Referenciados:**

- CMXsrv_call_val_tas
- sp_procxmode
- CMXsrv_fincol_efec_calpa

---

## CMXsrv_fincol_cont_pror
<a name="cmxsrv_fincol_cont_pror" ></a>

**Procedimientos Referenciados:**

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

## CMXsrv_fincol_cons_dpror
<a name="cmxsrv_fincol_cons_dpror" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_fincol_cctb_anu
<a name="cmxsrv_fincol_cctb_anu" ></a>

**Procedimientos Referenciados:**

- CMXsrv_busc_cod_ope
- CMXsrv_enl_act_enl
- sp_procxmode
- CMXsrv_fincol_ctb_anu
- sp_cmx_sii_1870
- CMXsrv_lee_fpro

---

## CMXsrv_fincol_calc_anu
<a name="cmxsrv_fincol_calc_anu" ></a>

**Procedimientos Referenciados:**

- sp_procxmode
- CMXsrv_fincol_efec_calpa

---

## CMXsrv_fincol_cons_anu
<a name="cmxsrv_fincol_cons_anu" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_fincol_cons_mod
<a name="cmxsrv_fincol_cons_mod" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_fincol_cons_dmod
<a name="cmxsrv_fincol_cons_dmod" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_fincol_cal_pext
<a name="cmxsrv_fincol_cal_pext" ></a>

**Procedimientos Referenciados:**

- CMXsrv_fincol_calc_reba
- CMXsrv_fincol_eval_tasa
- sp_procxmode

---

## CMXsrv_fincol_ctb_pext
<a name="cmxsrv_fincol_ctb_pext" ></a>

**Procedimientos Referenciados:**

- CMXsrv_ctb_pago
- CMXsrv_util_gen_vig
- sp_procxmode
- CMXsrv_lee_fpro

---

## CMXsrv_finobl_cal_pext
<a name="cmxsrv_finobl_cal_pext" ></a>

**Procedimientos Referenciados:**

- CMXsrv_finobl_eval_tasa
- sp_procxmode
- CMXsrv_fincol_cal_tas_sfr

---

## CMXsrv_finobl_ctb_pext
<a name="cmxsrv_finobl_ctb_pext" ></a>

**Procedimientos Referenciados:**

- CMXsrv_ctbo_pago
- sp_procxmode
- CMXsrv_lee_fpro

---

## CMXsrv_iarc_eli_arc
<a name="cmxsrv_iarc_eli_arc" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_iarc_busc_arc
<a name="cmxsrv_iarc_busc_arc" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_iinf_busc_inf
<a name="cmxsrv_iinf_busc_inf" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_iarc_act_arc
<a name="cmxsrv_iarc_act_arc" ></a>

**Procedimientos Referenciados:**

- CMXsrv_cmx_get_codes
- PrmACMXMONEDAFEC
- CMXsrv_util_opr_fec
- sp_procxmode

---

## CMXsrv_iarc_lee_arc
<a name="cmxsrv_iarc_lee_arc" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_iinf_busc_opr
<a name="cmxsrv_iinf_busc_opr" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_iinf_lee_vlr
<a name="cmxsrv_iinf_lee_vlr" ></a>

**Procedimientos Referenciados:**

- PrmACMXCLACOM
- sp_procxmode

---

## CMXsrv_iinf_rev_evi
<a name="cmxsrv_iinf_rev_evi" ></a>

**Procedimientos Referenciados:**

- CMXsrv_com_rev
- sp_procxmode

---

## CMXsrv_icob_lee_pln
<a name="cmxsrv_icob_lee_pln" ></a>

**Procedimientos Referenciados:**

- CMXsrv_cmx_get_codes
- CMXsrv_icob_obs_pln
- sp_procxmode

---

## CMXsrv_icob_cur_cob
<a name="cmxsrv_icob_cur_cob" ></a>

**Procedimientos Referenciados:**

- CMXsrv_icob_ctb_reem
- sp_procxmode
- CMXsrv_icob_val_cob

---

## CMXsrv_icob_pag_sop
<a name="cmxsrv_icob_pag_sop" ></a>

**Procedimientos Referenciados:**

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

## CMXsrv_icob_eli_pln
<a name="cmxsrv_icob_eli_pln" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icob_rev_etd
<a name="cmxsrv_icob_rev_etd" ></a>

**Procedimientos Referenciados:**

- CMXsrv_icob_refresh_pos
- CMXsrv_ctl_chq_aprcbl
- CMXsrv_icob_ctb_anu
- CMXsrv_icob_ctb_reem
- sp_procxmode
- CMXsrv_pos_eli_010
- CMXsrv_icob_rctb_sop

---

## CMXsrv_icob_val_cob
<a name="cmxsrv_icob_val_cob" ></a>

**Procedimientos Referenciados:**

- PrmACMXPAIS
- CMXsrv_pos_bcx_lee_cob
- CMXsrv_util_fecha
- sp_procxmode

---

## CMXsrv_icob_busc_pln
<a name="cmxsrv_icob_busc_pln" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icob_lee_cln
<a name="cmxsrv_icob_lee_cln" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icob_crea_norm
<a name="cmxsrv_icob_crea_norm" ></a>

**Procedimientos Referenciados:**

- sp_procxmode
- CMXsrv_icob_get_num

---

## CMXsrv_icob_crea_reem
<a name="cmxsrv_icob_crea_reem" ></a>

**Procedimientos Referenciados:**

- sp_procxmode
- CMXsrv_icob_get_num
- CMXsrv_cmx_get_codes
- CMXsrv_pos_bcx_lee_cob
- CMXsrv_pos_bcx_ing_cob

---

## CMXsrv_icob_act_gral
<a name="cmxsrv_icob_act_gral" ></a>

**Procedimientos Referenciados:**

- sp_procxmode
- CMXsrv_icob_num_con
- CMXsrv_icob_val_cob
- CMXsrv_pos_bcx_act_cob

---

## CMXsrv_icob_lee_cln2
<a name="cmxsrv_icob_lee_cln2" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icob_lee_gral
<a name="cmxsrv_icob_lee_gral" ></a>

**Procedimientos Referenciados:**

- CMXsrv_pos_bcx_lee_cob
- sp_procxmode

---

## CMXsrv_icob_act_val
<a name="cmxsrv_icob_act_val" ></a>

**Procedimientos Referenciados:**

- CMXsrv_get_ult_dia_habil
- sp_procxmode
- CMXsrv_icob_val_cob

---

## CMXsrv_icob_lee_val
<a name="cmxsrv_icob_lee_val" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icob_act_acu
<a name="cmxsrv_icob_act_acu" ></a>

**Procedimientos Referenciados:**

- sp_procxmode
- CMXsrv_icob_val_cob

---

## CMXsrv_icob_lee_acu
<a name="cmxsrv_icob_lee_acu" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icob_eli_int
<a name="cmxsrv_icob_eli_int" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icob_busc_int
<a name="cmxsrv_icob_busc_int" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icob_ingmod_int
<a name="cmxsrv_icob_ingmod_int" ></a>

**Procedimientos Referenciados:**

- PrmACMXMONEDA
- sp_procxmode
- CMXsrv_icob_val_cob

---

## CMXsrv_icob_lee_int
<a name="cmxsrv_icob_lee_int" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icob_ing_mod_srf
<a name="cmxsrv_icob_ing_mod_srf" ></a>

**Procedimientos Referenciados:**

- CMXsrv_pos_bcx_ing_cob
- sp_procxmode
- CMXsrv_icob_get_num
- CMXsrv_pos_bcx_act_cob

---

## CMXsrv_icob_anu
<a name="cmxsrv_icob_anu" ></a>

**Procedimientos Referenciados:**

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

## CMXsrv_icob_lee_anu
<a name="cmxsrv_icob_lee_anu" ></a>

**Procedimientos Referenciados:**

- CMXsrv_pos_bcx_lee_cob
- sp_procxmode

---

## CMXsrv_icob_cur_reem
<a name="cmxsrv_icob_cur_reem" ></a>

**Procedimientos Referenciados:**

- CMXsrv_icob_ctb_reem
- sp_procxmode
- CMXsrv_icob_refresh_pos
- CMXsrv_icob_val_cob

---

## CMXsrv_busc_cor_swf
<a name="cmxsrv_busc_cor_swf" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_swf_bus_sms
<a name="cmxsrv_swf_bus_sms" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icbr_lee_cbr
<a name="cmxsrv_icbr_lee_cbr" ></a>

**Procedimientos Referenciados:**

- PrmACMXESPECI
- PrmACLNEJECTA
- sp_procxmode

---

## CMXsrv_icbr_acep_let
<a name="cmxsrv_icbr_acep_let" ></a>

**Procedimientos Referenciados:**

- CMXsrv_ctl_crea_apr
- sp_procxmode

---

## CMXsrv_icbr_cont_cbr
<a name="cmxsrv_icbr_cont_cbr" ></a>

**Procedimientos Referenciados:**

- CMXsrv_ctl_marc_firma
- CMXsrv_mbyte_gen
- CMXsrv_icbr_val_cbr
- CMXsrv_nibx_upd_tran
- CMXsrv_cnt_gen_vig
- sp_procxmode
- CMXsrv_ctb_cbr
- CMXsrv_nibx_nilive

---

## CMXsrv_icbr_eli_cbr
<a name="cmxsrv_icbr_eli_cbr" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icbr_lee_ctp
<a name="cmxsrv_icbr_lee_ctp" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icbr_avi1
<a name="cmxsrv_icbr_avi1" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icbr_busc_cbr
<a name="cmxsrv_icbr_busc_cbr" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icbr_lee_cln
<a name="cmxsrv_icbr_lee_cln" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icbr_crea_cbr
<a name="cmxsrv_icbr_crea_cbr" ></a>

**Procedimientos Referenciados:**

- srv_icbr_asig_num
- sp_procxmode
- CMXsrv_util_num_ope

---

## CMXsrv_icbr_lee_cob
<a name="cmxsrv_icbr_lee_cob" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icbr_act_ctp
<a name="cmxsrv_icbr_act_ctp" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icbr_lee_trm
<a name="cmxsrv_icbr_lee_trm" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icbr_act_trm
<a name="cmxsrv_icbr_act_trm" ></a>

**Procedimientos Referenciados:**

- CMXsrv_util_fecha
- CMXsrv_icbr_val_cbr
- sp_procxmode

---

## CMXsrv_icbr_lee_doc
<a name="cmxsrv_icbr_lee_doc" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icbr_act_doc
<a name="cmxsrv_icbr_act_doc" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icbr_busc_let
<a name="cmxsrv_icbr_busc_let" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icbr_ingmod_let
<a name="cmxsrv_icbr_ingmod_let" ></a>

**Procedimientos Referenciados:**

- CMXsrv_util_fecha
- sp_procxmode

---

## CMXsrv_icbr_eli_let
<a name="cmxsrv_icbr_eli_let" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icbr_lee_let
<a name="cmxsrv_icbr_lee_let" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icbr_prorr
<a name="cmxsrv_icbr_prorr" ></a>

**Procedimientos Referenciados:**

- CMXsrv_util_fecha
- CMXsrv_cnt_2600
- sp_procxmode
- CMXsrv_cnt_2610
- CMXsrv_cnt_2620

---

## CMXsrv_icbr_rev_eve
<a name="cmxsrv_icbr_rev_eve" ></a>

**Procedimientos Referenciados:**

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

## CMXsrv_icbr_busc_eve
<a name="cmxsrv_icbr_busc_eve" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icbr_lee_eve
<a name="cmxsrv_icbr_lee_eve" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icbr_lee_ent_doc
<a name="cmxsrv_icbr_lee_ent_doc" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icbr_prot
<a name="cmxsrv_icbr_prot" ></a>

**Procedimientos Referenciados:**

- sp_procxmode
- CMXsrv_ctl_crea_apr
- CMXsrv_cnt_950

---

## CMXsrv_icbr_pcg_prot
<a name="cmxsrv_icbr_pcg_prot" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icbr_liq_sdo
<a name="cmxsrv_icbr_liq_sdo" ></a>

**Procedimientos Referenciados:**

- CMXsrv_ctb_liq_sdo
- sp_procxmode
- CMXsrv_cnt_gen_vig

---

## CMXsrv_icbr_act_vis
<a name="cmxsrv_icbr_act_vis" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icbr_eli_rep
<a name="cmxsrv_icbr_eli_rep" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icbr_busc_rep
<a name="cmxsrv_icbr_busc_rep" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icbr_imod_rep
<a name="cmxsrv_icbr_imod_rep" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icbr_ent_doc
<a name="cmxsrv_icbr_ent_doc" ></a>

**Procedimientos Referenciados:**

- CMXsrv_ctl_crea_apr
- sp_procxmode

---

## CMXsrv_icbr_trf_ofi
<a name="cmxsrv_icbr_trf_ofi" ></a>

**Procedimientos Referenciados:**

- CMXsrv_ctb_trfo
- sp_procxmode

---

## CMXsrv_icbr_trf_bco
<a name="cmxsrv_icbr_trf_bco" ></a>

**Procedimientos Referenciados:**

- CMXsrv_ctb_trfb
- sp_procxmode

---

## CMXsrv_icbr_act_inst
<a name="cmxsrv_icbr_act_inst" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_iswf_a_pru
<a name="cmxsrv_iswf_a_pru" ></a>

**Procedimientos Referenciados:**

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

## CMXsrv_icbr_val_cbr
<a name="cmxsrv_icbr_val_cbr" ></a>

**Procedimientos Referenciados:**

- PrmACMXPAIS
- CMXsrv_icbr_val_arc
- CMXsrv_util_fecha
- sp_procxmode
- PrmACMXMONEDAFEC

---

## CMXsrv_icrd_a_ibab
<a name="cmxsrv_icrd_a_ibab" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_lee_glo_ibab
<a name="cmxsrv_icrd_lee_glo_ibab" ></a>

**Procedimientos Referenciados:**

- sp_procxmode
- CMXsrv_icrd_pre_78

---

## CMXsrv_icrd_a_ibar
<a name="cmxsrv_icrd_a_ibar" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_lee_glo_ibar
<a name="cmxsrv_icrd_lee_glo_ibar" ></a>

**Procedimientos Referenciados:**

- CMXsrv_icrd_pre_72_740
- sp_procxmode

---

## CMXsrv_icrd_lee_tex_swf
<a name="cmxsrv_icrd_lee_tex_swf" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_lee_cod_txt_swf
<a name="cmxsrv_icrd_lee_cod_txt_swf" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_lee_txt_swf_all
<a name="cmxsrv_icrd_lee_txt_swf_all" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_lee_ind_esp_ing
<a name="cmxsrv_icrd_lee_ind_esp_ing" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_ing_acu
<a name="cmxsrv_icrd_ing_acu" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_lee_acu
<a name="cmxsrv_icrd_lee_acu" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_rech_sol
<a name="cmxsrv_icrd_rech_sol" ></a>

**Procedimientos Referenciados:**

- CMXsrv_nibx_upd_tran
- CMXsrv_ctl_crea_apr
- sp_procxmode
- CMXsrv_nibx_nilive

---

## CMXsrv_icrd_end
<a name="cmxsrv_icrd_end" ></a>

**Procedimientos Referenciados:**

- CMXsrv_ctl_crea_apr
- sp_procxmode

---

## CMXsrv_icrd_lee_dat_end
<a name="cmxsrv_icrd_lee_dat_end" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_asignar_cor
<a name="cmxsrv_icrd_asignar_cor" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_lee_bco_mtr
<a name="cmxsrv_icrd_lee_bco_mtr" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_cor_lee_pais
<a name="cmxsrv_icrd_cor_lee_pais" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_lee_plz
<a name="cmxsrv_icrd_lee_plz" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_busc_plz
<a name="cmxsrv_icrd_busc_plz" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_cor_busc_pais
<a name="cmxsrv_icrd_cor_busc_pais" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_busc_bco_mtr
<a name="cmxsrv_icrd_busc_bco_mtr" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_iddi_ingmod_ddi
<a name="cmxsrv_iddi_ingmod_ddi" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_iddi_lee_dec
<a name="cmxsrv_iddi_lee_dec" ></a>

**Procedimientos Referenciados:**

- sp_procxmode
- CMXsrv_iddi_val_num_ddi

---

## CMXsrv_iddi_eli_ddi
<a name="cmxsrv_iddi_eli_ddi" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_iddi_lee_inf
<a name="cmxsrv_iddi_lee_inf" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_iddi_lee_cln
<a name="cmxsrv_iddi_lee_cln" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_iddi_lee_rut
<a name="cmxsrv_iddi_lee_rut" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_iddi_asoc_ddi
<a name="cmxsrv_iddi_asoc_ddi" ></a>

**Procedimientos Referenciados:**

- CMXsrv_cmx_get_codes
- CMXsrv_get_ult_dia_habil
- CMXsrv_util_opr_fec
- sp_procxmode

---

## CMXsrv_iddi_des_ddi
<a name="cmxsrv_iddi_des_ddi" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_iddi_busc_asoc
<a name="cmxsrv_iddi_busc_asoc" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_iddi_busc_noasoc
<a name="cmxsrv_iddi_busc_noasoc" ></a>

**Procedimientos Referenciados:**

- CMXsrv_iddi_bus_noasoc_cob
- CMXsrv_iddi_bus_noasoc_opr
- sp_procxmode

---

## CMXsrv_icrd_lee_dir_cln
<a name="cmxsrv_icrd_lee_dir_cln" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXCRDsrv_icrd_a_cnd_esp
<a name="cmxcrdsrv_icrd_a_cnd_esp" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_lee_cnd_esp
<a name="cmxsrv_icrd_lee_cnd_esp" ></a>

**Procedimientos Referenciados:**

- sp_procxmode
- CMXsrv_icrd_pre_47

---

## CMXCRDsrv_icrd_clon_crd
<a name="cmxcrdsrv_icrd_clon_crd" ></a>

**Procedimientos Referenciados:**

- CMXCRDsrv_icrd_lee_tas_cln
- sp_procxmode
- CMXsrv_fincol_ing_modcol
- CMXsrv_util_num_ope

---

## CMXCRDsrv_icrd_lee_crdcre
<a name="cmxcrdsrv_icrd_lee_crdcre" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_lee_top
<a name="cmxsrv_icrd_lee_top" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXCRDsrv_icrd_val_crd
<a name="cmxcrdsrv_icrd_val_crd" ></a>

**Procedimientos Referenciados:**

- sp_procxmode
- CMXsrv_icrd_val_adv
- CMXsrv_icrd_val_err

---

## CMXCRDsrv_icrd_eli_crd
<a name="cmxcrdsrv_icrd_eli_crd" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_lee_dat_trs
<a name="cmxsrv_icrd_lee_dat_trs" ></a>

**Procedimientos Referenciados:**

- CMXsrv_icrd_forlin
- sp_procxmode

---

## CMXsrv_icrd_a_ctp
<a name="cmxsrv_icrd_a_ctp" ></a>

**Procedimientos Referenciados:**

- CMXCRDsrv_icrd_lee_tas_cln
- CMXsrv_fincol_imod_colcc
- sp_procxmode

---

## CMXsrv_icrd_lee_cln
<a name="cmxsrv_icrd_lee_cln" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_a_cnd
<a name="cmxsrv_icrd_a_cnd" ></a>

**Procedimientos Referenciados:**

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

## CMXCRDsrv_icrd_crea_crd
<a name="cmxcrdsrv_icrd_crea_crd" ></a>

**Procedimientos Referenciados:**

- CMXsrv_imp_calc_aladi
- CMXsrv_fincol_imod_colcc
- sp_procxmode
- CMXCRDsrv_icrd_lee_tas_cln
- CMXsrv_util_num_ope
- CMXsrv_fincol_ing_modcol

---

## CMXsrv_icrd_busc_emb
<a name="cmxsrv_icrd_busc_emb" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_eli_emb
<a name="cmxsrv_icrd_eli_emb" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_lee_emb1
<a name="cmxsrv_icrd_lee_emb1" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_lee_emb2
<a name="cmxsrv_icrd_lee_emb2" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_a_emb1
<a name="cmxsrv_icrd_a_emb1" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_a_emb2
<a name="cmxsrv_icrd_a_emb2" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_val_emb2
<a name="cmxsrv_icrd_val_emb2" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_val_emb1
<a name="cmxsrv_icrd_val_emb1" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_act_ref
<a name="cmxsrv_icrd_act_ref" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_lee_ref
<a name="cmxsrv_icrd_lee_ref" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXCRDsrv_icrd_apr_sol
<a name="cmxcrdsrv_icrd_apr_sol" ></a>

**Procedimientos Referenciados:**

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

## CMXsrv_icrd_lee_crdapr
<a name="cmxsrv_icrd_lee_crdapr" ></a>

**Procedimientos Referenciados:**

- CMXsrv_icrd_pre_72
- sp_procxmode

---

## CMXCRDsrv_icrd_a_desc_merc
<a name="cmxcrdsrv_icrd_a_desc_merc" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_lee_desc_merc
<a name="cmxsrv_icrd_lee_desc_merc" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_a_otr_doc
<a name="cmxsrv_icrd_a_otr_doc" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_lee_otr_doc
<a name="cmxsrv_icrd_lee_otr_doc" ></a>

**Procedimientos Referenciados:**

- sp_procxmode
- CMXsrv_icrd_pre_46

---

## CMXsrv_iinf_lee0_inf
<a name="cmxsrv_iinf_lee0_inf" ></a>

**Procedimientos Referenciados:**

- PrmACMXFPAIMP
- PrmACMXMONEDA
- PrmACLNEJECTA
- sp_procxmode

---

## CMXsrv_iinf_lee_tablas
<a name="cmxsrv_iinf_lee_tablas" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_iinf_lee1_inf
<a name="cmxsrv_iinf_lee1_inf" ></a>

**Procedimientos Referenciados:**

- PrmACMXCLACOM
- PrmACMXESPECI
- sp_procxmode
- PrmACLNEJECTA
- PrmACMXETDINF

---

## CMXsrv_iinf_lee_cln
<a name="cmxsrv_iinf_lee_cln" ></a>

**Procedimientos Referenciados:**

- PrmACLNEJECTA
- sp_procxmode

---

## CMXsrv_iinf_lee2_inf
<a name="cmxsrv_iinf_lee2_inf" ></a>

**Procedimientos Referenciados:**

- PrmACMXPAIS
- PrmACMXORIDVS
- PrmACMXRGMIMP
- sp_procxmode
- PrmACMXBCOBCC
- PrmACMXBCOCEN
- PrmACMXSUCSAL

---

## CMXsrv_iinf_avi_miscb
<a name="cmxsrv_iinf_avi_miscb" ></a>

**Procedimientos Referenciados:**

- PrmACMXBCOBCC
- sp_procxmode

---

## CMXsrv_iinf_avi_misca
<a name="cmxsrv_iinf_avi_misca" ></a>

**Procedimientos Referenciados:**

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

## CMXsrv_icrd_lee_dat_com
<a name="cmxsrv_icrd_lee_dat_com" ></a>

**Procedimientos Referenciados:**

- PrmACMXMONEDA
- sp_procxmode

---

## CMXsrv_iinf_eli_inf
<a name="cmxsrv_iinf_eli_inf" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_iinf_busc_evi
<a name="cmxsrv_iinf_busc_evi" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_iinf_val_inf
<a name="cmxsrv_iinf_val_inf" ></a>

**Procedimientos Referenciados:**

- CMXsrv_cmx_get_codes
- PrmACMXPAIS
- PrmACMXCLACOM
- sp_procxmode

---

## CMXsrv_iinf_ingmod_inf
<a name="cmxsrv_iinf_ingmod_inf" ></a>

**Procedimientos Referenciados:**

- CMXsrv_util_fecha
- sp_procxmode
- PrmACMXMONEDAFEC
- CMXsrv_cmx_get_codes
- CMXsrv_iinf_val_inf
- CMXsrv_iinf_get_num

---

## CMXsrv_iinf_lee_fec
<a name="cmxsrv_iinf_lee_fec" ></a>

**Procedimientos Referenciados:**

- CMXsrv_util_fecha
- sp_procxmode

---

## CMXsrv_iinf_lee_usd
<a name="cmxsrv_iinf_lee_usd" ></a>

**Procedimientos Referenciados:**

- CMXsrv_cmx_get_codes
- PrmACMXMONEDAFEC
- sp_procxmode

---

## CMXsrv_iinf_act_apr
<a name="cmxsrv_iinf_act_apr" ></a>

**Procedimientos Referenciados:**

- CMXsrv_iinf_val_inf
- CMXsrv_util_fecha
- sp_procxmode

---

## CMXsrv_iinf_lee_evi
<a name="cmxsrv_iinf_lee_evi" ></a>

**Procedimientos Referenciados:**

- PrmACMXSUCSAL
- PrmACMXBCOCEN
- sp_procxmode
- PrmACMXETDINF

---

## CMXsrv_iinf_act_tib
<a name="cmxsrv_iinf_act_tib" ></a>

**Procedimientos Referenciados:**

- CMXsrv_cmx_get_codes
- sp_procxmode

---

## CMXsrv_iinf_act_rec
<a name="cmxsrv_iinf_act_rec" ></a>

**Procedimientos Referenciados:**

- CMXsrv_util_fecha
- sp_procxmode

---

## CMXsrv_iinf_act_rib
<a name="cmxsrv_iinf_act_rib" ></a>

**Procedimientos Referenciados:**

- CMXsrv_cmx_get_codes
- sp_procxmode

---

## CMXsrv_iinf_busc_comp
<a name="cmxsrv_iinf_busc_comp" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_iinf_ingmod_comp
<a name="cmxsrv_iinf_ingmod_comp" ></a>

**Procedimientos Referenciados:**

- CMXsrv_util_fecha
- sp_procxmode
- PrmACMXMONEDAFEC
- CMXsrv_cmx_get_codes
- CMXsrv_iinf_val_inf
- CMXsrv_iinf_get_num

---

## CMXsrv_iinf_lee_comp
<a name="cmxsrv_iinf_lee_comp" ></a>

**Procedimientos Referenciados:**

- PrmACMXPAIS
- PrmACMXORIDVS
- PrmACMXRGMIMP
- PrmACMXCLACOM
- sp_procxmode
- PrmACMXFPAIMP
- PrmACMXVIATPT
- PrmACMXMONEDA

---

## CMXsrv_iinf_lee_bco
<a name="cmxsrv_iinf_lee_bco" ></a>

**Procedimientos Referenciados:**

- PrmACMXPAIS
- sp_procxmode

---

## CMXsrv_iinf_busc_bco
<a name="cmxsrv_iinf_busc_bco" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXMCRDsrv_icrd_lee_mcnd
<a name="cmxmcrdsrv_icrd_lee_mcnd" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icbr_mod_ing_let
<a name="cmxsrv_icbr_mod_ing_let" ></a>

**Procedimientos Referenciados:**

- CMXsrv_util_opr_fec
- sp_procxmode

---

## CMXsrv_icbr_acep_mod_cbr
<a name="cmxsrv_icbr_acep_mod_cbr" ></a>

**Procedimientos Referenciados:**

- CMXsrv_cnt_2800
- CMXsrv_icbr_cheq_mdoc
- CMXsrv_icbr_val_cbr
- CMXsrv_icbr_cheq_mctp
- CMXsrv_icbr_cheq_mter
- sp_procxmode
- CMXsrv_icbr_cheq_mlcb

---

## CMXsrv_icbr_eli_no_cont
<a name="cmxsrv_icbr_eli_no_cont" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXMCRDsrv_icrd_a_mmcnd
<a name="cmxmcrdsrv_icrd_a_mmcnd" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXMCRDsrv_icrd_lee_mctp
<a name="cmxmcrdsrv_icrd_lee_mctp" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXMCRDsrv_icrd_lee_memb2
<a name="cmxmcrdsrv_icrd_lee_memb2" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXMCRDsrv_icrd_lee_memb1
<a name="cmxmcrdsrv_icrd_lee_memb1" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXMCRDsrv_icrd_lee_mref
<a name="cmxmcrdsrv_icrd_lee_mref" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_ing_txt
<a name="cmxsrv_icrd_ing_txt" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXCRDsrv_icrd_get_ing_esp
<a name="cmxcrdsrv_icrd_get_ing_esp" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXMCRDsrv_icrd_lee_mtxt
<a name="cmxmcrdsrv_icrd_lee_mtxt" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXCRDsrv_icrd_get_pre_fra
<a name="cmxcrdsrv_icrd_get_pre_fra" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXMCRDsrv_icrd_a_mmer
<a name="cmxmcrdsrv_icrd_a_mmer" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_fincol_lee_cod_eve
<a name="cmxsrv_fincol_lee_cod_eve" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXMCRDsrv_icrd_acep_mod_crd
<a name="cmxmcrdsrv_icrd_acep_mod_crd" ></a>

**Procedimientos Referenciados:**

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

## CMXMCRDsrv_icrd_eli_no_cont
<a name="cmxmcrdsrv_icrd_eli_no_cont" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_a_rec_age
<a name="cmxsrv_icrd_a_rec_age" ></a>

**Procedimientos Referenciados:**

- CMXsrv_util_fecha
- sp_procxmode

---

## CMXsrv_busc_ofi_cta
<a name="cmxsrv_busc_ofi_cta" ></a>

**Procedimientos Referenciados:**

- PrmACMXESPECI
- PrmACLNEJECTA
- sp_procxmode

---

## CMXsrv_neg_busc_arc
<a name="cmxsrv_neg_busc_arc" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_lee_avi_adi
<a name="cmxsrv_icrd_lee_avi_adi" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_lee_dat_cln
<a name="cmxsrv_icrd_lee_dat_cln" ></a>

**Procedimientos Referenciados:**

- CMXsrv_trae_glo_fec
- sp_procxmode

---

## CMXsrv_icrd_lee_avi_dis
<a name="cmxsrv_icrd_lee_avi_dis" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_neg_ddi_asoc
<a name="cmxsrv_neg_ddi_asoc" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_neg_trae_vcto_mcf
<a name="cmxsrv_neg_trae_vcto_mcf" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_neg_avi_lee_aval
<a name="cmxsrv_neg_avi_lee_aval" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_neg_lee_crd
<a name="cmxsrv_icrd_neg_lee_crd" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_lee_neg
<a name="cmxsrv_icrd_lee_neg" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_col_avi_dat_cln
<a name="cmxsrv_col_avi_dat_cln" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_col_avi_det_pag
<a name="cmxsrv_col_avi_det_pag" ></a>

**Procedimientos Referenciados:**

- CMX_srv_pone_punto
- CMXsrv_util_fecha
- sp_procxmode

---

## CMXsrv_col_avi_det_oto
<a name="cmxsrv_col_avi_det_oto" ></a>

**Procedimientos Referenciados:**

- CMX_srv_pone_punto
- CMXsrv_trae_glo_fec
- sp_procxmode

---

## CMXsrv_col_lee_num_trs
<a name="cmxsrv_col_lee_num_trs" ></a>

**Procedimientos Referenciados:**

- CMXsrv_avigrl_lee_avitemp
- sp_procxmode

---

## CMXsrv_finobl_avi_pag
<a name="cmxsrv_finobl_avi_pag" ></a>

**Procedimientos Referenciados:**

- CMX_srv_pone_punto
- sp_procxmode

---

## CMXsrv_neg_avi_trae_asnd_mn
<a name="cmxsrv_neg_avi_trae_asnd_mn" ></a>

**Procedimientos Referenciados:**

- CMX_srv_pone_punto
- sp_procxmode

---

## CMXsrv_neg_avi_trae_asnd_mx
<a name="cmxsrv_neg_avi_trae_asnd_mx" ></a>

**Procedimientos Referenciados:**

- CMX_srv_pone_punto
- sp_procxmode

---

## CMXsrv_icrd_cont_neg
<a name="cmxsrv_icrd_cont_neg" ></a>

**Procedimientos Referenciados:**

- CMXsrv_icrd_val_neg
- CMXsrv_mbyte_gen
- sp_procxmode
- sp_cmx_sii_1870
- CMXsrv_fincol_ictb_neg_aux

---

## CMXsrv_icrd_eli_neg
<a name="cmxsrv_icrd_eli_neg" ></a>

**Procedimientos Referenciados:**

- CMXsrv_swf_graba_det
- sp_procxmode

---

## CMXsrv_icrd_lee_num_col
<a name="cmxsrv_icrd_lee_num_col" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_bus_pago
<a name="cmxsrv_icrd_bus_pago" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_lee_col
<a name="cmxsrv_icrd_lee_col" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_busc_neg
<a name="cmxsrv_icrd_busc_neg" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_a_neg_emb1
<a name="cmxsrv_icrd_a_neg_emb1" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_a_neg_emb2
<a name="cmxsrv_icrd_a_neg_emb2" ></a>

**Procedimientos Referenciados:**

- sp_procxmode
- CMXsrv_icrd_chq_doc_neg

---

## CMXsrv_icrd_eli_doc_neg
<a name="cmxsrv_icrd_eli_doc_neg" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_lee_neg_emb1
<a name="cmxsrv_icrd_lee_neg_emb1" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_lee_neg_emb2
<a name="cmxsrv_icrd_lee_neg_emb2" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_a_neg_disc
<a name="cmxsrv_icrd_a_neg_disc" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_neg_lee_disc
<a name="cmxsrv_icrd_neg_lee_disc" ></a>

**Procedimientos Referenciados:**

- sp_procxmode
- CMXsrv_icrd_gen_disc

---

## CMXsrv_icrd_ent_doc
<a name="cmxsrv_icrd_ent_doc" ></a>

**Procedimientos Referenciados:**

- CMXsrv_mbyte_gen
- CMXsrv_swf_graba_det
- sp_procxmode

---

## CMXsrv_icrd_alz_disc
<a name="cmxsrv_icrd_alz_disc" ></a>

**Procedimientos Referenciados:**

- CMXsrv_get_ult_dia_habil
- CMXsrv_icrd_cont_alz
- CMXsrv_ipuc_gen_pln
- sp_procxmode
- CMXsrv_cnt_950
- CMXsrv_cmx_get_codes
- CMXsrv_fincol_cal_tas_sfr

---

## CMXCRDsrv_icrd_asignar_cor
<a name="cmxcrdsrv_icrd_asignar_cor" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXCRDsrv_icrd_bus_lcr_bco
<a name="cmxcrdsrv_icrd_bus_lcr_bco" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_act_doc_neg
<a name="cmxsrv_icrd_act_doc_neg" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_lee_doc_neg
<a name="cmxsrv_icrd_lee_doc_neg" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icrd_val_neg
<a name="cmxsrv_icrd_val_neg" ></a>

**Procedimientos Referenciados:**

- CMXsrv_util_det_habil_tasa
- CMXsrv_fincol_val_per_tas
- CMXsrv_util_fecha
- sp_procxmode

---

## CMXsrv_icbr_lee_dat_var
<a name="cmxsrv_icbr_lee_dat_var" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icbr_val_pag
<a name="cmxsrv_icbr_val_pag" ></a>

**Procedimientos Referenciados:**

- CMXsrv_val_cta_cte
- CMXsrv_calc_imp_4pct
- CMXsrv_util_fecha
- sp_procxmode
- CMXsrv_enl_val_sel
- CMXsrv_ctb_impto_ddi

---

## CMXsrv_icbr_ctb_pag
<a name="cmxsrv_icbr_ctb_pag" ></a>

**Procedimientos Referenciados:**

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

## CMXsrv_icbr_cal_pag
<a name="cmxsrv_icbr_cal_pag" ></a>

**Procedimientos Referenciados:**

- CMXsrv_get_ult_dia_habil
- sp_procxmode
- CMXsrv_valida_tc
- CMXsrv_icbr_cal_int
- CMXsrv_icbr_cre_pln

---

## CMXsrv_icbr_eli_pag
<a name="cmxsrv_icbr_eli_pag" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_val_vig
<a name="cmxsrv_val_vig" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icbr_lee_cbr0
<a name="cmxsrv_icbr_lee_cbr0" ></a>

**Procedimientos Referenciados:**

- CMXsrv_icrd_lee_cln
- sp_procxmode

---

## CMXsrv_icbr_obt_mon_nac
<a name="cmxsrv_icbr_obt_mon_nac" ></a>

**Procedimientos Referenciados:**

- CMXsrv_cmx_get_codes
- sp_procxmode

---

## CMXsrv_icbr_lee_dat_pag
<a name="cmxsrv_icbr_lee_dat_pag" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icbr_pcg_pag
<a name="cmxsrv_icbr_pcg_pag" ></a>

**Procedimientos Referenciados:**

- PrmACMXMONEDAFEC
- sp_procxmode

---

## CMXsrv_icbr_busc_pago
<a name="cmxsrv_icbr_busc_pago" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icbr_eli_int_pago
<a name="cmxsrv_icbr_eli_int_pago" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icbr_busc_int
<a name="cmxsrv_icbr_busc_int" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icbr_ingmod_int
<a name="cmxsrv_icbr_ingmod_int" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icbr_lee_int_pago
<a name="cmxsrv_icbr_lee_int_pago" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icbr_lee_bco
<a name="cmxsrv_icbr_lee_bco" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

## CMXsrv_icbr_busc_bco
<a name="cmxsrv_icbr_busc_bco" ></a>

**Procedimientos Referenciados:**

- sp_procxmode

---

