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

| **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** | **Procedimientos Referenciados** |
|-------------|------------------------------|--------------------------|-------------------------------|
| Form_Activate | CMXsrv_expcbe_lee_prm | ACMXPRMGRL | sp_procxmode, CMXsrv_lee_fpro |
| Form_Activate | CMXsrv_cmx_busc_suc_usu | master..sysprocesses, tbl_User | PrmACMXSUCSAL, CMXsrv_cmx_ing_lib, sp_procxmode |
| Form_Activate | CMXsrv_expcbe_lee_cbe | ACMXPAIS, COR, ACMXPGOCBE, CBE01, CBE, ACMXMONEDA, ACMXENTDOC, ACMXSUCSAL, ACMXPRTCBE, CLN | CMXsrv_cmx_busc_suc_usu, CMXsrv_val_suc, sp_procxmode, CMXsrv_lee_fpro |
| Form_Load | CMXsrv_trae_glo_fec | ACMXSUCSAL, ACMXDL3475FEC, tbl_User | sp_procxmode |
| ingcomg_Click | CMXsrv_expcbe_avs_cyg1 | ACMXDESEMB, ASND, ACMXIMPUES, ACMXPRMGRL, EVZ, CBE, COM, TRSD, CLN, ACMXESPECI | sp_procxmode |
| ingcomg_Click | CMXsrv_expcbe_avs_cyg2 | ASND, ACMXIMPUES, ACMXPRMGRL, EVZ, CBE | por, sp_procxmode |
| ingret_Click | CMXsrv_expcbe_avs_ret | ACMXPAIS, COR, ACMXDESEMB, CBE, ACMXMONEDA, ACMXSUCSAL, CLN, ACMXESPECI, RET | sp_procxmode |
| M3_Click | CMXsrv_expcbe_swf_sel | switxt, switxt1 | CMXsrv_expcbe_swf_422, CMXsrv_expcbe_swf_420, CMXsrv_expcbe_swf_499, CMXsrv_expcbe_swf_430, sp_procxmode |
| M4_Click | CMXsrv_expcbe_swf_sel | switxt, switxt1 | CMXsrv_expcbe_swf_422, CMXsrv_expcbe_swf_420, CMXsrv_expcbe_swf_499, CMXsrv_expcbe_swf_430, sp_procxmode |
| Mcbeanl_Click | CMXsrv_expcbe_anl_cbe | CBE | CMXsrv_cnt_gen_vig, sp_procxmode, CMXsrv_expcbe_grb_evz, CMXsrv_cnt_950, CMXsrv_cnt_630 |
| Mcbectb_Click | CMXsrv_expcbe_ctb_ing | OPE_BCI, CBE | CMXsrv_cnt_600, CMXsrv_mbyte_gen, CMXsrv_nibx_upd_tran, CMXsrv_cnt_gen_vig, sp_procxmode, CMXsrv_expcbe_grb_evz, CMXsrv_cnt_950, CMXsrv_expcbe_val_cbe, CMXsrv_nibx_nilive |
| Mcbedel_Click | CMXsrv_expcbe_del_cbe | EVL, CBE01, COD, CBE, EVZ, COM, ACTZ, CTZ | sp_procxmode |
| Mcbeval_Click | CMXsrv_expcbe_val_cbe | COR, CBE01, ACMXPRMGRL, CBE, DCZ, CTZ, warnmsg, ACMXPAIS, ACMXFERIADO, CCO | sp_procxmode |
| Men1_Click | CMXsrv_expcbe_swf_sel | switxt, switxt1 | CMXsrv_expcbe_swf_422, CMXsrv_expcbe_swf_420, CMXsrv_expcbe_swf_499, CMXsrv_expcbe_swf_430, sp_procxmode |
| aceptar_Click | CMXsrv_expcbe_grb_ctp | ACMXPAIS, CBE | sp_procxmode |
| fld_cbe_cod_exp_lostfocus | CMXsrv_expcbe_lee_cln | CLN | sp_procxmode |
| fld_cbe_cod_suc_LostFocus | CMXsrv_val_suc | ACMXSUCSAL, tbl_User | sp_procxmode |
| Form_Activate | CMXsrv_expcbe_lee_ctp | ACMXSUCSAL, ACMXPAIS, CBE, CLN | sp_procxmode |
| aceptar_Click | CMXsrv_expcbe_grb_bco | ACMXPRMGRL, CBE, COR, CBE01 | sp_procxmode |
| fld_cbe_cod_cob_Lostfocus | CMXsrv_expcbe_lee_cor | ACMXPAIS, COR | sp_procxmode |
| fld_cbe_cod_rmb_LostFocus | CMXsrv_expcbe_lee_cor | ACMXPAIS, COR | sp_procxmode |
| Form_Activate | CMXsrv_expcbe_lee_bco | CBE, COR, CBE01 | CMXsrv_icrd_lee_cln, sp_procxmode |
| aceptar_Click | CMXsrv_expcbe_grb_doc | CBE, DCZ | sp_procxmode |
| aceptar_Click | CMXsrv_expcbe_grb_doc02 | CBE02 | sp_procxmode |
| Form_Activate | CMXsrv_expcbe_lee_doc | CBE | sp_procxmode |
| Form_Activate | CMXsrv_expcbe_lee_doc02 | CBE02 | sp_procxmode |
| ELIMINAR_Click | CMXsrv_expcbe_del_ctz | ACTZ, CBE, CTZ | sp_procxmode |
| Form_Activate | CMXsrv_expcbe_bus_ctz | ACTZ, CBE, CTZ | sp_procxmode |
| aceptar_Click | CMXsrv_expcbe_grb_ctz | ACTZ, CBE, CTZ | sp_procxmode |
| Form_Activate | CMXsrv_expcbe_mto_ctz | ACTZ, CBE, CTZ | sp_procxmode |
| Form_Activate | CMXsrv_expcbe_lee_ctz | ACTZ, CBE, CTZ | sp_procxmode |
| aceptar_Click | CMXsrv_expcbe_lee_cbe | ACMXPAIS, COR, ACMXPGOCBE, CBE01, CBE, ACMXMONEDA, ACMXENTDOC, ACMXSUCSAL, ACMXPRTCBE, CLN | CMXsrv_cmx_busc_suc_usu, CMXsrv_val_suc, sp_procxmode, CMXsrv_lee_fpro |
| buscar_Click | CMXsrv_expcbe_bus_cbe | CBE | sp_procxmode |
| fld_aux_cod_exp_LostFocus | CMXsrv_expcbe_lee_cln | CLN | sp_procxmode |
| Proximas_Click | CMXsrv_expcbe_bus_cbe | CBE | sp_procxmode |
| aceptar_Click | CMXsrv_expcbe_mdf_cbe | ACTZ, ACMXPRMGRL, CBE | CMXsrv_expcbe_grb_evl, CMXsrv_expcbe_act_ctz, CMXsrv_cnt_gen_vig, CMXsrv_cnt_610, sp_procxmode, CMXsrv_expcbe_grb_evz, CMXsrv_cnt_950, CMXsrv_lee_fpro |
| aceptar_Click | CMXsrv_expcbe_cre_actz | ACTZ, CBE, CTZ | sp_procxmode |
| fld_cbe_cod_suc_LostFocus | CMXsrv_val_suc | ACMXSUCSAL, tbl_User | sp_procxmode |
| Form_Activate | CMXsrv_expcbe_lee_mdf | COR, ACMXPGOCBE, CBE01, CBE, ACMXMONEDA, ACMXSUCSAL, CLN | sp_procxmode |
| aceptar_Click | CMXsrv_expcbe_pgo_cbe | ACMXDESEMB, COR, CLN, RET, vig_cmx, COD, ACMXIMPUES, ACMXPRMGRL, CBE, ACMXPRMEXP, COM, tbl_User, OPREC, ACMXPAIS, ACMXFERIADO, CCO | CMXsrv_mbyte_gen, CMXsrv_expret_grb_org, CMXsrv_expret_grb_dtn, CMXsrv_cnt_gen_vig, CMXsrv_expret_cre_ret, CMXsrv_vig_gra_vig, sp_procxmode, CMXsrv_expcbe_grb_evz, CMXsrv_cnt_950, CMXsrv_exp_ipuc_gen_pln, CMXsrv_expcbe_trp_cyg, CMXsrv_expret_grb_det, CMXsrv_cnt_620 |
| fld_cbe_cod_rmb_LostFocus | CMXsrv_expcbe_lee_cor | ACMXPAIS, COR | sp_procxmode |
| Form_Activate | CMXsrv_expcbe_lee_pgo | ACMXDESEMB, COR, CBE, ACMXPRMEXP, ACMXMONEDA, OPREC, CLN | sp_procxmode, CMXsrv_lee_fpro |
| Form_Activate | CMXsrv_expcbe_bus_evz | EVZ, CBE | sp_procxmode |
| Proximo_Click | CMXsrv_expcbe_bus_evz | EVZ, CBE | sp_procxmode |
| Reversar_Click | CMXsrv_expcbe_rev_cbe | EVL, ACMXDESEMB, COR, ORG, ACMXIMPUES, ACMXPRMGRL, EVZ, CBE, TRSD, ACMXPRMEXP, COM, EVR, CTZ, DTN, OPREC, RET, PUCBCX10 | por, CMXsrv_mbyte_gen, CMXsrv_cnt_rev_vig, CMXsrv_expcbe_rev_trp, CMXsrv_ctl_chq_aprcbl, CMXsrv_rev_950, CMXsrv_cnt_610, sp_procxmode, CMXsrv_expcbe_grb_evz, CMXsrv_cnt_631, CMXsrv_cnt_601, CMXsrv_cnt_621, CMXsrv_lee_fpro |
| Form_Activate | CMXsrv_expcbe_lee_evz | ACMXDESEMB, COR, ACMXPGOCBE, EVZ, CBE, ACMXMONEDA, ACMXTIPEVE, ACMXSUCSAL | sp_procxmode |
| Eliminar_Click | CMXsrv_expcbe_del_dcz | CBE02, CBE, DCZ | sp_procxmode |
| Form_Activate | CMXsrv_expcbe_bus_dcz | DCZ | sp_procxmode |
| aceptar_Click | CMXsrv_expcbe_grb_dcz | CBE02, CBE, DCZ | sp_procxmode |
| Form_Activate | CMXsrv_expcbe_lee_dcz | DCZ | sp_procxmode |
| aceptar_Click | CMXsrv_expcbe_lee_cbe | ACMXPAIS, COR, ACMXPGOCBE, CBE01, CBE, ACMXMONEDA, ACMXENTDOC, ACMXSUCSAL, ACMXPRTCBE, CLN | CMXsrv_cmx_busc_suc_usu, CMXsrv_val_suc, sp_procxmode, CMXsrv_lee_fpro |
| buscar_Click | CMXsrv_expcbe_bus_vto | CBE | sp_procxmode |
| fld_aux_cod_exp_LostFocus | CMXsrv_expcbe_lee_cln | CLN | sp_procxmode |
| Proximas_Click | CMXsrv_expcbe_bus_vto | CBE | sp_procxmode |
| aceptar_Click | CMXsrv_avi_dat_cou |  | sp_procxmode, CMXsrv_avigrl_crea_avitemp, bcicomex |
| aceptar_Click | CMXsrv_expcbe_avs_rem1 | COR, ACMXPGOCBE, ACMXPRTCBE, CBE01, CBE, CBE02, ACMXMONEDA, CTZ, ACMXENTDOC, ACMXPAIS, ACMXPAISES, CLN | sp_procxmode, CMXsrv_trae_glo_fec, CMXsrv_expcbe_val_cbe, CMXsrv_util_fmt_txt |
| aceptar_Click | CMXsrv_expcbe_avs_rem3 | COR, CBE01, CBE, CTZ, ACMXMONEDA, ACMXPAISES, CLN, CCO | CMXsrv_util_fmt_txt, sp_procxmode |
| imprime_esp | CMXsrv_expcbe_avs_rem2 | CBE02, CBE, DCZ | sp_procxmode, CMXsrv_expcbe_for_lin |
| imprime_esp | CMXsrv_expcbe_avs_rem4 | ACMXREMFESPMSG, ACMXREMFINGMSG | sp_procxmode |
| imprime_ing | CMXsrv_expcbe_avs_rem2 | CBE02, CBE, DCZ | sp_procxmode, CMXsrv_expcbe_for_lin |
| imprime_ing | CMXsrv_expcbe_avs_rem4 | ACMXREMFESPMSG, ACMXREMFINGMSG | sp_procxmode |
| buscar_Click | CMXsrv_busc_plz | ACMXPLAZAS, comex..ACMXPLAZAS | sp_procxmode |
| fld_cor_cod_plz_Lostfocus | CMXsrv_lee_plz | ACMXPLAZAS | CMXsrv_mbyte_cmp, sp_procxmode |
| proximos_Click | CMXsrv_busc_plz | ACMXPLAZAS, comex..ACMXPLAZAS | sp_procxmode |
| buscar_Click | CMXsrv_cor_busc_pais | ACMXPAIS | sp_procxmode |
| fld_cor_cod_pais_LostFocus | CMXsrv_cor_lee_pais | comex..ACMXPAIS | sp_procxmode |
| proximos_Click | CMXsrv_cor_busc_pais | ACMXPAIS | sp_procxmode |
| aceptar_Click | CMXsrv_expcbe_lee_cor | ACMXPAIS, COR | sp_procxmode |
| buscar_Click | CMXsrv_expcbe_bus_cor | COR | sp_procxmode |
| fld_aux_cod_pai_LostFocus | CMXsrv_cor_lee_pais | comex..ACMXPAIS | sp_procxmode |
| fld_aux_cod_plz_LostFocus | CMXsrv_lee_plz | ACMXPLAZAS | CMXsrv_mbyte_cmp, sp_procxmode |
| proximos_Click | CMXsrv_expcbe_bus_cor | COR | sp_procxmode |
| buscar_Click | CMXsrv_busc_bco_mtr | ACMXBANCOS | sp_procxmode |
| proximos_Click | CMXsrv_busc_bco_mtr | ACMXBANCOS | sp_procxmode |
| enviar_Click | CMXsrv_expcbe_swf_sel | switxt, switxt1 | CMXsrv_expcbe_swf_422, CMXsrv_expcbe_swf_420, CMXsrv_expcbe_swf_499, CMXsrv_expcbe_swf_430, sp_procxmode |
| Aceptar_Click | CMXsrv_expcbe_lee_cor | ACMXPAIS, COR | sp_procxmode |
| buscar_Click | CMXsrv_expcbe_bus_cor | COR | sp_procxmode |
| proximos_Click | CMXsrv_expcbe_bus_cor | COR | sp_procxmode |
| Form_Load | CMXsrv_grl_fec_serv |  | SRV_MessageService, sp_procxmode |

---

## EXPCCE
<a name="expcce"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** | **Procedimientos Referenciados** |
|-------------|------------------------------|--------------------------|-------------------------------|
| Form_Activate | CMXsrv_cmx_busc_suc_usu | master..sysprocesses, tbl_User | PrmACMXSUCSAL, CMXsrv_cmx_ing_lib, sp_procxmode |
| Form_Activate | CMXsrv_expcce_lee_cce | ACMXPAIS, COR, tbl_User, CCE, ACMXSUCSAL, CLN | por, sp_procxmode |
| Form_Activate | CMXsrv_expcce_trd_cce | ACMXFORPAG, ACMXVIATPT, ACMXMAXCCE, ACMXCNFCCE, ACMXMONEDA, ACMXCLACOM, CCE, ACMXRCBCCE | sp_procxmode |
| MCCEANL_CLICK | CMXsrv_expcce_anl_cce | CCE | CMXsrv_cmx_lee_trs, sp_procxmode, CMXsrv_expcce_grb_evc, CMXsrv_expcce_ictb_anu, CMXsrv_cnt_950, CMXsrv_cnt_740, CMXsrv_expcce_lee_fpro |
| Mccectb_click | CMXsrv_expcce_ctb_ing | CCE | CMXsrv_mbyte_gen, sp_procxmode, CMXsrv_expcce_val_cce, CMXsrv_expcce_grb_evc, CMXsrv_cnt_950, CMXsrv_cnt_700 |
| Mccedel_Click | CMXsrv_expcce_del_cce | COD, ACCECTP, ACCECND, CCB, COM, ACCEBCO, DCC, CCE, EVC, ACCEDCC, AFIN | sp_procxmode |
| MCCEVAL_CLICK | CMXsrv_expcce_val_cce | ACMXPAIS, COR, ACMXPRMGRL, CCE_ADI, DCC, tbl_User, CCE, warnmsg, ACMXSUCSAL, COL | CMXsrv_cmx_get_codes, sp_procxmode |
| Mmt730_Click | CMXsrv_expcce_swf_sel | switxt, switxt1 | CMXsrv_expcce_swf_730, CMXsrv_expcce_swf_742, sp_procxmode |
| Mmt730Ing_Click | CMXsrv_expcce_swf_sel | switxt, switxt1 | CMXsrv_expcce_swf_730, CMXsrv_expcce_swf_742, sp_procxmode |
| Aceptar_Click | CMXsrv_expcce_grb_bco | CCB, ACCEBCO, ACCECRSE, CRSE, CCE | sp_procxmode, CMXsrv_expcce_lee_fpro |
| fld_cce_bco_avs_LostFocus | CMXsrv_expcce_lee_cor | ACMXPAIS, COR | sp_procxmode |
| fld_cce_bco_orig_LostFocus | CMXsrv_expcce_lee_cor | ACMXPAIS, COR | sp_procxmode |
| fld_cce_cod_ems_LostFocus | CMXsrv_expcce_lee_cor | ACMXPAIS, COR | sp_procxmode |
| fld_cce_cod_rmb_LostFocus | CMXsrv_expcce_lee_cor | ACMXPAIS, COR | sp_procxmode |
| Form_Activate | CMXsrv_expcce_lee_bco | COR, CCB, ACMXSUCSAL, ACCEBCO, CRSE, CCE, ACMXPAIS | sp_procxmode |
| Aceptar_Click | CMXsrv_expcce_grb_ctp | ACCECTP, CCE | sp_procxmode, CMXsrv_expcce_lee_fpro |
| fld_cce_cod_bn1_LostFocus | CMXsrv_expcce_lee_cln | CLN | sp_procxmode |
| fld_cce_cod_bn2_LostFocus | CMXsrv_expcce_lee_cln | CLN | sp_procxmode |
| Form_Activate | CMXsrv_expcce_lee_ctp | ACCECTP, ACMXPAIS, CLN, CCE | sp_procxmode |
| Aceptar_Click | CMXsrv_expcce_cre_cce | CCE | CMXsrv_util_num_ope, CMXsrv_cmx_busc_suc_usu, sp_procxmode, CMXsrv_expcce_lee_fpro |
| Aceptar_Click | CMXsrv_expcce_grb_bco | CCB, ACCEBCO, ACCECRSE, CRSE, CCE | sp_procxmode, CMXsrv_expcce_lee_fpro |
| Aceptar_Click | CMXsrv_expcce_grb_ctp | ACCECTP, CCE | sp_procxmode, CMXsrv_expcce_lee_fpro |
| Aceptar_Click | CMXsrv_expcce_gen_dcc | ACMXPAIS, DCC, CCE | sp_procxmode |
| Aceptar_Click | CMXsrv_expcce_grb_cnd | CCE_ADI, ACCECRSE, CRSE, CCE, ACCE_ADI, ACCECND | sp_procxmode, CMXsrv_expcce_lee_fpro |
| fld_cce_fec_vto_LostFocus | CMXsrv_util_det_habil | ACMXFERIADO | sp_procxmode |
| Form_Activate | CMXsrv_expcce_lee_cnd | CCE_ADI, ACCECRSE, CRSE, CCE, ACCE_ADI, ACCECND | sp_procxmode |
| Form_Activate | CMXsrv_expcce_trd_cnd | ACMXFORPAG, ACMXVIATPT, ACMXMAXCCE, ACMXCNFCCE, ACMXMONEDA, CCE, ACMXCLACOM, ACMXFDESDE, ACMXRCBCCE, ACCECND | sp_procxmode |
| ELIMINAR_Click | CMXsrv_expcce_del_dcc | DCC, CCE, ACCEDCC | sp_procxmode, CMXsrv_expcce_lee_fpro |
| Form_Activate | CMXsrv_expcce_bus_dcc | DCC, CCE, ACCEDCC | CMXsrv_expcce_gen_adcc, sp_procxmode |
| Aceptar_Click | CMXsrv_expcce_grb_dcc | DCC, CCE, ACCEDCC | sp_procxmode, CMXsrv_expcce_lee_fpro |
| Form_Activate | CMXsrv_expcce_lee_dcc | DCC, CCE, ACCEDCC | sp_procxmode |
| Aceptar_Click | CMXsrv_expcce_lee_cce | ACMXPAIS, COR, tbl_User, CCE, ACMXSUCSAL, CLN | por, sp_procxmode |
| buscar_Click | CMXsrv_expcce_bus_cce | CCE | sp_procxmode |
| fld_aux_cod_bn1_lostfocus | CMXsrv_expcce_lee_cln | CLN | sp_procxmode |
| proximo_Click | CMXsrv_expcce_bus_cce | CCE | sp_procxmode |
| Aceptar_Click | CMXsrv_expcce_mdf_cce | COR, ACCECTP, ACCEBCO, CCE_ADI, ACCECRSE, DAC, DCC, CRSE, CCE, ACCE_ADI, NGE, COL, ACCEDCC, ACCECND | CMXsrv_expcce_can_mdf, CMXsrv_expcce_get_tip_ope, sp_procxmode, CMXsrv_expcce_grb_evc, CMXsrv_cnt_950, CMXsrv_cmx_get_codes, CMXsrv_expcce_ctb_mdfcce, CMXsrv_expcce_lee_fpro, CMXsrv_cnt_720 |
| Cancelar_Click | CMXsrv_expcce_can_mdf | ACCECTP, ACCEBCO, ACCEDCC, ACCECND | sp_procxmode |
| fld_cce_cod_bn1_LostFocus | CMXsrv_expcce_lee_cln | CLN | sp_procxmode |
| fld_cce_cod_ems_LostFocus | CMXsrv_expcce_lee_cor | ACMXPAIS, COR | sp_procxmode |
| Form_Activate | CMXsrv_expcce_lee_mdf | ACMXSUCSAL, COR, CCE, CLN | sp_procxmode |
| Aceptar_Click | CMXsrv_expcce_cnf_cce | COR, CCE, CLN | CMXsrv_cnt_710, sp_procxmode, CMXsrv_expcce_ictb_cexp, CMXsrv_expcce_grb_evc, CMXsrv_cnt_950, CMXsrv_expcce_lee_fpro |
| Aceptar_Click | CMXsrv_expcce_grb_afin | AFIN | sp_procxmode |
| Form_Activate | CMXsrv_expcce_lee_cnf | ACMXFORPAG, COR, ACMXMONEDA, CCE, CLN | sp_procxmode, CMXsrv_expcce_lee_fpro |
| Form_Activate | CMXsrv_expcce_lee_afin | CCE, AFIN | sp_procxmode |
| Aceptar_Click | CMXsrv_expcce_trp_cce | COR, CCE | sp_procxmode, CMXsrv_cnt_730, CMXsrv_expcce_grb_evc, CMXsrv_cnt_950 |
| fld_cce_bco_dst_LostFocus | CMXsrv_expcce_lee_cor | ACMXPAIS, COR | sp_procxmode |
| Form_Activate | CMXsrv_expcce_lee_trp | CCE | sp_procxmode, CMXsrv_expcce_lee_fpro |
| Form_Activate | CMXsrv_expcce_bus_evc | EVC, CCE, NGE | sp_procxmode |
| proximo_Click | CMXsrv_expcce_bus_evc | EVC, CCE, NGE | sp_procxmode |
| reversar_Click | CMXsrv_expcce_rev_cce | COR, TAS, ACMXIMPUES, LTR, DCN, EVC, RET, CUO, EVO, TRSD, DSN, CCE, NGE, PUCBCX10, COD, CNO, COM, DAC, EVE, CAN, COL, AFIN, ORG, DTN, EVR | CMXsrv_expcce_rev_mdf, CMXsrv_expcce_ctb_alz, CMXsrv_expcce_rctb_anu, CMXsrv_cnt_751, CMXsrv_cnt_761, CMXsrv_expcce_rctb_oto, CMXsrv_cnt_1771, CMXsrv_cnt_720, CMXsrv_expcce_ranu_neg, CMXsrv_mbyte_gen, CMXsrv_expcce_chk_dsn, CMXsrv_ctl_chq_aprcbl, CMXsrv_rev_950, CMXsrv_cnt_771, CMXsrv_expcce_eli_col, CMXsrv_expcce_grb_evc, CMXsrv_cnt_731, CMXsrv_expcce_get_tip_ope, CMXsrv_expcce_rctb_oto_exp, CMXsrv_cnt_711, CMXsrv_cnt_rev_vig, CMXsrv_cnt_701, CMXsrv_cmx_lee_trs, CMXsrv_cnt_999999, CMXsrv_expcce_lee_fpro, CMXsrv_cnt_741, CMXsrv_expcce_eli_obl, CMXsrv_expneg_rev_trp, sp_procxmode, CMXsrv_cnt_781, CMXsrv_expcce_ctb_mdfcce, CMXsrv_expcce_gen_dsn, CMXsrv_expcce_rctb_pag_exp |
| Form_Activate | CMXsrv_expcce_lee_evc | ACMXFORPAG, ACMXMONEDA, CCE, NGE, EVC, ACMXSUCSAL, ACMXTIPEVE | sp_procxmode |
| aceptar_Click | CMXsrv_expcce_avs_rem1 | ACMXFORPAG, COR, CCB, NGEB, ACMXMONEDA, LTR, CCE, DCN, NGE, ACMXPAISES, CLN | CMXsrv_trae_glo_fec, sp_procxmode |
| buscar_Click | CMXsrv_busc_plz | ACMXPLAZAS, comex..ACMXPLAZAS | sp_procxmode |
| fld_cor_cod_plz_Lostfocus | CMXsrv_lee_plz | ACMXPLAZAS | CMXsrv_mbyte_cmp, sp_procxmode |
| proximos_Click | CMXsrv_busc_plz | ACMXPLAZAS, comex..ACMXPLAZAS | sp_procxmode |
| buscar_Click | CMXsrv_cor_busc_pais | ACMXPAIS | sp_procxmode |
| fld_cor_cod_pais_LostFocus | CMXsrv_cor_lee_pais | comex..ACMXPAIS | sp_procxmode |
| proximos_Click | CMXsrv_cor_busc_pais | ACMXPAIS | sp_procxmode |
| Aceptar_Click | CMXsrv_expcce_lee_cor | ACMXPAIS, COR | sp_procxmode |
| buscar_Click | CMXsrv_expcce_bus_cor | COR | sp_procxmode |
| Command1_Click | CMXsrv_expcce_bus_cor | COR | sp_procxmode |
| proximos_Click | CMXsrv_expcce_bus_cor | COR | sp_procxmode |
| enviar_Click | CMXsrv_expcce_swf_sel | switxt, switxt1 | CMXsrv_expcce_swf_730, CMXsrv_expcce_swf_742, sp_procxmode |
| Form_Load | CMXsrv_grl_fec_serv |  | SRV_MessageService, sp_procxmode |

---

## expdex
<a name="expdex"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** | **Procedimientos Referenciados** |
|-------------|------------------------------|--------------------------|-------------------------------|
| form_activate | CMXsrv_expcbe_lee_prm | ACMXPRMGRL | sp_procxmode, CMXsrv_lee_fpro |
| form_activate | CMXsrv_dex_lee_dex | ACMXSUCSAL, DEX, CLN, ACMXADUANA | sp_procxmode |
| Mdexeli_Click | CMXsrv_dex_eli_dex | DEX | sp_procxmode |
| ACEPTAR_Click | CMXsrv_dex_act_dex | DEX | CMXsrv_exppln_get_dig, sp_procxmode, CMXsrv_lee_fpro |
| fld_dex_dia_plz_max_LostFocus | CMXsrv_expdex_cal_fec |  | sp_procxmode |
| fld_dex_fec_acep_LostFocus | CMXsrv_expdex_cal_fec |  | sp_procxmode |
| fld_dex_rut_exp_LostFocus | CMXsrv_dex_lee_cli | CLN | sp_procxmode |
| FORM_Load | CMXsrv_dex_lee_dex | ACMXSUCSAL, DEX, CLN, ACMXADUANA | sp_procxmode |
| Buscar_Click | CMXsrv_dex_bus_dex | DEX | sp_procxmode |
| fld_dex_rut_exp_LostFocus | CMXsrv_dex_lee_cli | CLN | sp_procxmode |
| FORM_Load | CMXsrv_grl_fec_serv |  | SRV_MessageService, sp_procxmode |
| ACEPTAR_Click | CMXsrv_dex_act_dex | DEX | CMXsrv_exppln_get_dig, sp_procxmode, CMXsrv_lee_fpro |
| fld_dex_rut_exp_LostFocus | CMXsrv_dex_lee_cli | CLN | sp_procxmode |
| FORM_Load | CMXsrv_dex_lee_dex | ACMXSUCSAL, DEX, CLN, ACMXADUANA | sp_procxmode |
| COMELIMINAR_Click | CMXsrv_dex_eli_dex | DEX | sp_procxmode |
| Form_Activate | CMXsrv_dex_lee_dex | ACMXSUCSAL, DEX, CLN, ACMXADUANA | sp_procxmode |

---

## EXPNEG
<a name="expneg"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** | **Procedimientos Referenciados** |
|-------------|------------------------------|--------------------------|-------------------------------|
| Form_Activate | CMXsrv_expcbe_bus_evz | EVZ, CBE | sp_procxmode |
| Proximo_Click | CMXsrv_expcbe_bus_evz | EVZ, CBE | sp_procxmode |
| Reversar_Click | CMXsrv_expcbe_rev_cbe | EVL, ACMXDESEMB, COR, ORG, ACMXIMPUES, ACMXPRMGRL, EVZ, CBE, TRSD, ACMXPRMEXP, COM, EVR, CTZ, DTN, OPREC, RET, PUCBCX10 | por, CMXsrv_mbyte_gen, CMXsrv_cnt_rev_vig, CMXsrv_expcbe_rev_trp, CMXsrv_ctl_chq_aprcbl, CMXsrv_rev_950, CMXsrv_cnt_610, sp_procxmode, CMXsrv_expcbe_grb_evz, CMXsrv_cnt_631, CMXsrv_cnt_601, CMXsrv_cnt_621, CMXsrv_lee_fpro |
| Form_Activate | CMXsrv_expcbe_lee_evz | ACMXDESEMB, COR, ACMXPGOCBE, EVZ, CBE, ACMXMONEDA, ACMXTIPEVE, ACMXSUCSAL | sp_procxmode |
| Form_Activate | CMXsrv_expcce_lee_bas | ACMXMONEDA, CCE, ACMXFORPAG | sp_procxmode |
| Form_Activate | CMXsrv_expcce_lee_neg | COR, ACMXVIATPT, ACMXSUCSAL, ACMXDISNEG, ACMXMONEDA, ACMXCLACOM, NGE, ACMXPAIS, CLN, ACMXTPONEG | CMXsrv_cmx_busc_suc_usu, sp_procxmode |
| Mccealznge_click | CMXsrv_expcce_alz_dis | COL, CCE, NGE | CMXsrv_expcce_ctb_alz, CMXsrv_cnt_760, sp_procxmode, CMXsrv_expcce_grb_evc, CMXsrv_cnt_950, CMXsrv_expcce_get_tip_ope, CMXsrv_expcce_lee_fpro |
| Mcceanlnge_click | CMXsrv_expcce_anl_neg | CCE, NGE | CMXsrv_cmx_lee_trs, sp_procxmode, CMXsrv_cnt_780, CMXsrv_expcce_grb_evc, CMXsrv_expcce_ictb_anu, CMXsrv_cnt_950, CMXsrv_expcce_lee_fpro |
| Mccectbnge_Click | CMXsrv_expcce_ctb_neg | COR, LTR, CCE, NGE, AFIN | CMXsrv_expcce_val_neg, CMXsrv_mbyte_gen, CMXsrv_expcce_ineg_cexp, sp_procxmode, CMXsrv_expcce_anu_cexp, CMXsrv_expcce_grb_evc, CMXsrv_cnt_950, CMXsrv_expcce_lee_fpro, CMXsrv_cnt_750 |
| Mccedelnge_Click | CMXsrv_expcce_del_neg | CRSN, COD, COM, NGEB, LTR, DSN, CCE, DCN, NGE, EVC, AFIN | sp_procxmode |
| Mccevalnge_click | CMXsrv_expcce_val_neg | NGEB, LTR, DCC, warnmsg, CCE, DCN, NGE, COL, AFIN | CMXsrv_util_fecha, sp_procxmode |
| Mtel742_Click | CMXsrv_expcce_swf_sel | switxt, switxt1 | CMXsrv_expcce_swf_730, CMXsrv_expcce_swf_742, sp_procxmode |
| Form_Activate | CMXsrv_expcce_bus_evc | EVC, CCE, NGE | sp_procxmode |
| Proximo_Click | CMXsrv_expcce_bus_evc | EVC, CCE, NGE | sp_procxmode |
| Reversar_Click | CMXsrv_expcce_rev_cce | COR, TAS, ACMXIMPUES, LTR, DCN, EVC, RET, CUO, EVO, TRSD, DSN, CCE, NGE, PUCBCX10, COD, CNO, COM, DAC, EVE, CAN, COL, AFIN, ORG, DTN, EVR | CMXsrv_expcce_rev_mdf, CMXsrv_expcce_ctb_alz, CMXsrv_expcce_rctb_anu, CMXsrv_cnt_751, CMXsrv_cnt_761, CMXsrv_expcce_rctb_oto, CMXsrv_cnt_1771, CMXsrv_cnt_720, CMXsrv_expcce_ranu_neg, CMXsrv_mbyte_gen, CMXsrv_expcce_chk_dsn, CMXsrv_ctl_chq_aprcbl, CMXsrv_rev_950, CMXsrv_cnt_771, CMXsrv_expcce_eli_col, CMXsrv_expcce_grb_evc, CMXsrv_cnt_731, CMXsrv_expcce_get_tip_ope, CMXsrv_expcce_rctb_oto_exp, CMXsrv_cnt_711, CMXsrv_cnt_rev_vig, CMXsrv_cnt_701, CMXsrv_cmx_lee_trs, CMXsrv_cnt_999999, CMXsrv_expcce_lee_fpro, CMXsrv_cnt_741, CMXsrv_expcce_eli_obl, CMXsrv_expneg_rev_trp, sp_procxmode, CMXsrv_cnt_781, CMXsrv_expcce_ctb_mdfcce, CMXsrv_expcce_gen_dsn, CMXsrv_expcce_rctb_pag_exp |
| Form_Activate | CMXsrv_expcce_lee_evc | ACMXFORPAG, ACMXMONEDA, CCE, NGE, EVC, ACMXSUCSAL, ACMXTIPEVE | sp_procxmode |
| aceptar_Click | CMXsrv_expcce_grb_neg | CRSN, CCE, NGEB, NGE | CMXsrv_cmx_busc_suc_usu, sp_procxmode, CMXsrv_expcce_lee_fpro |
| aceptar_Click | CMXsrv_expcce_gen_dcn | DCC, CCE, DCN, NGE | sp_procxmode |
| aceptar_Click | CMXsrv_expcce_grb_afin | AFIN | sp_procxmode |
| fld_cce_cod_exp_nge_LostFocus | CMXsrv_expcce_lee_cln | CLN | sp_procxmode |
| fld_cce_cod_pag_nge_LostFocus | CMXsrv_expcce_lee_cor | ACMXPAIS, COR | sp_procxmode |
| fld_cce_cod_rmb_nge_LostFocus | CMXsrv_expcce_lee_cor | ACMXPAIS, COR | sp_procxmode |
| fld_cce_ins_rem1_nge_GotFocus | CMXsrv_expcce_avs_rem5 | COR, ACMXCRDREMTXT, ACMXMONEDA, CCE, NGE, ACMXPAISES, CCO | CMX_srv_pone_punto, CMXsrv_util_fmt_txt, sp_procxmode, CMXsrv_expcce_get_ing_esp |
| Form_Load | CMXsrv_expcce_lee_nge | COR, CRSN, NGEB, CCE, NGE, ACMXPAIS, CLN | sp_procxmode |
| Form_Load | CMXsrv_expcce_trd_nge | ACMXVIATPT, ACMXRCBCCE, ACMXMONEDA, ACMXCLACOM, NGE, ACMXTPONEG | sp_procxmode |
| Form_Load | CMXsrv_expcce_ini_neg | ACMXPAIS, COR, ACMXVIATPT, CCB, ACMXMONEDA, CRSE, CCE, ACMXCLACOM, NGE, ACMXSUCSAL, CLN, ACMXTPONEG | sp_procxmode, CMXsrv_expcce_lee_fpro |
| Form_Load | CMXsrv_expcce_lee_afin | CCE, AFIN | sp_procxmode |
| lee_bco | CMXsrv_expcce_lee_cor | ACMXPAIS, COR | sp_procxmode |
| ELIMINAR_Click | CMXsrv_expcce_del_dcn | CCE, DCN, NGE | sp_procxmode |
| Form_Activate | CMXsrv_expcce_bus_dcn | DCN, NGE | sp_procxmode |
| Aceptar_Click | CMXsrv_expcce_grb_dcn | CCE, DCN, NGE | sp_procxmode |
| Form_Load | CMXsrv_expcce_lee_dcn | DCC, DCN, NGE | sp_procxmode |
| ELIMINAR_Click | CMXsrv_expcce_del_ltr | LTR, CCE, NGE | sp_procxmode |
| Form_Activate | CMXsrv_expcce_bus_ltr | LTR, NGE | sp_procxmode |
| Aceptar_Click | CMXsrv_expcce_grb_ltr | LTR, CCE, NGE | sp_procxmode |
| Form_Load | CMXsrv_expcce_lee_ltr | LTR, CCE, NGE | sp_procxmode |
| ELIMINAR_Click | CMXsrv_expcce_del_dsn | DSN, CCE, NGE | sp_procxmode |
| Form_Activate | CMXsrv_expcce_gen_dsn | DCC, DSN, CCE, DCN, NGE | CMXsrv_expcce_grb_dsn, sp_procxmode |
| Form_Activate | CMXsrv_expcce_bus_dsn | DSN, NGE | sp_procxmode |
| Salir_Click | CMXsrv_expcce_chk_dsn | DSN, CCE, NGE | sp_procxmode |
| Aceptar_Click | CMXsrv_expcce_grb_dsn | DSN, CCE, NGE | sp_procxmode, CMXsrv_expcce_chk_dsn |
| Form_Load | CMXsrv_expcce_lee_dsn | DSN, NGE | sp_procxmode |
| buscar_Click | CMXsrv_expcce_bus_neg | CCE, NGE | sp_procxmode |
| Proximas_Click | CMXsrv_expcce_bus_neg | CCE, NGE | sp_procxmode |
| aceptar_Click | CMXsrv_expcce_pgo_neg | ACMXDESEMB, COR, vig_cmx, ACMXIMPUES, COD, ACMXPRMEXP, COM, CCE, tbl_User, NGE, CLN, RET | CMXsrv_expret_grb_dtn, CMXsrv_expcce_anu_cexp, CMXsrv_cnt_1770, CMXsrv_expret_grb_det, CMXsrv_mbyte_gen, CMXsrv_expret_grb_org, CMXsrv_cnt_gen_vig, CMXsrv_vig_gra_vig, CMXsrv_expcce_grb_evc, CMXsrv_cmx_get_codes, CMXsrv_expret_cre_ret, CMXsrv_cnt_770, CMXsrv_cnt_999999, CMXsrv_exp_ipuc_gen_pln, CMXsrv_expcce_lee_fpro, CMXsrv_expneg_trp_cyg, sp_procxmode, CMXsrv_expcce_pag_exp, CMXsrv_cnt_950 |
| aceptar_Click | CMXsrv_expcce_grb_afin | AFIN | sp_procxmode |
| fld_cce_cod_exp_nge_LostFocus | CMXsrv_expcce_lee_cln | CLN | sp_procxmode |
| fld_cce_cod_rmb_nge_LostFocus | CMXsrv_expcce_lee_cor | ACMXPAIS, COR | sp_procxmode |
| Form_Load | CMXsrv_expcce_lee_pgo | ACMXDESEMB, COR, ACMXPRMEXP, ACMXMONEDA, CCE, NGE, CLN | sp_procxmode, CMXsrv_expcce_lee_fpro |
| Form_Load | CMXsrv_expcce_lee_afin | CCE, AFIN | sp_procxmode |
| lee_bco | CMXsrv_expcce_lee_cor | ACMXPAIS, COR | sp_procxmode |
| aceptar_Click | CMXsrv_avi_dat_cou |  | sp_procxmode, CMXsrv_avigrl_crea_avitemp, bcicomex |
| aceptar_Click | CMXsrv_expcce_lee_nge | COR, CRSN, NGEB, CCE, NGE, ACMXPAIS, CLN | sp_procxmode |
| aceptar_Click | CMXsrv_expcce_avs_rem1 | ACMXFORPAG, COR, CCB, NGEB, ACMXMONEDA, LTR, CCE, DCN, NGE, ACMXPAISES, CLN | CMXsrv_trae_glo_fec, sp_procxmode |
| aceptar_Click | CMXsrv_expcce_avs_rem3 | LTR, NGE | CMXsrv_util_fmt_txt, sp_procxmode |
| imprime_esp | CMXsrv_expcce_avs_rem2 | DCN | sp_procxmode |
| imprime_esp | CMXsrv_expcce_avs_rem4 | DSN | CMXsrv_util_fmt_txt, sp_procxmode |
| imprime_esp | CMXsrv_expcbe_avs_rem4 | ACMXREMFESPMSG, ACMXREMFINGMSG | sp_procxmode |
| imprime_ing | CMXsrv_expcce_avs_rem2 | DCN | sp_procxmode |
| imprime_ing | CMXsrv_expcce_avs_rem4 | DSN | CMXsrv_util_fmt_txt, sp_procxmode |
| imprime_ing | CMXsrv_expcbe_avs_rem4 | ACMXREMFESPMSG, ACMXREMFINGMSG | sp_procxmode |
| aceptar_Click | CMXsrv_expcce_lee_cor | ACMXPAIS, COR | sp_procxmode |
| buscar_Click | CMXsrv_expcce_bus_cor | COR | sp_procxmode |
| proximos_Click | CMXsrv_expcce_bus_cor | COR | sp_procxmode |
| enviar_Click | CMXsrv_expcce_swf_sel | switxt, switxt1 | CMXsrv_expcce_swf_730, CMXsrv_expcce_swf_742, sp_procxmode |
| Form_Load | CMXsrv_grl_fec_serv |  | SRV_MessageService, sp_procxmode |

---

## expret
<a name="expret"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** | **Procedimientos Referenciados** |
|-------------|------------------------------|--------------------------|-------------------------------|
| buscar_Click | CMXsrv_busc_plz | ACMXPLAZAS, comex..ACMXPLAZAS | sp_procxmode |
| fld_cor_cod_plz_Lostfocus | CMXsrv_lee_plz | ACMXPLAZAS | CMXsrv_mbyte_cmp, sp_procxmode |
| proximos_Click | CMXsrv_busc_plz | ACMXPLAZAS, comex..ACMXPLAZAS | sp_procxmode |
| buscar_Click | CMXsrv_cor_busc_pais | ACMXPAIS | sp_procxmode |
| fld_cor_cod_pais_LostFocus | CMXsrv_cor_lee_pais | comex..ACMXPAIS | sp_procxmode |
| proximos_Click | CMXsrv_cor_busc_pais | ACMXPAIS | sp_procxmode |
| Aceptar_Click | CMXsrv_expcbe_lee_cor | ACMXPAIS, COR | sp_procxmode |
| buscar_Click | CMXsrv_expcbe_bus_cor | COR | sp_procxmode |
| proximos_Click | CMXsrv_expcbe_bus_cor | COR | sp_procxmode |
| Command2_Click | CMXsrv_expret_swf_sel | DTN, ACMXPRMEXP, switxt, switxt1 | CMXsrv_expret_swf_202, CMXsrv_expret_swf_100, sp_procxmode |
| Form_Load | CMXsrv_grl_fec_serv |  | SRV_MessageService, sp_procxmode |
| Form_Activate | CMXsrv_cmx_busc_suc_usu | master..sysprocesses, tbl_User | PrmACMXSUCSAL, CMXsrv_cmx_ing_lib, sp_procxmode |
| Form_Activate | CMXsrv_expret_lee_ret | DTN, ACMXPRMEXP, ACMXMONEDA, ACMXSUCSAL, CLN, RET | CMXsrv_cmx_busc_suc_usu, sp_procxmode, CMXsrv_lee_fpro |
| Form_Load | CMXsrv_expret_lee_prm | ACMXPRMGRL, ACMXPRMEXP | sp_procxmode, CMXsrv_lee_fpro |
| M_cgyc_Click | CMXsrv_expret_avs_cyg1 | ACMXDESEMB, ASND, ACMXIMPUES, ACMXPRMGRL, COM, TRSD, EVR, CLN, ACMXESPECI, RET | sp_procxmode |
| M_cgyc_Click | CMXsrv_expret_avs_cyg2 | ASND, ACMXIMPUES, ACMXPRMGRL, EVR, RET | sp_procxmode |
| mavisliq_Click | CMXsrv_expret_avs_liq1 | DTN, ACMXMONEDA, ACMXSUCSAL, CLN, ACMXESPECI, RET | sp_procxmode |
| mavisliq_Click | CMXsrv_expret_avs_liq2 | ORG, RET | sp_procxmode |
| mavisliq_Click | CMXsrv_expret_avs_liq3 | DTN, ACMXPRMEXP, RET | sp_procxmode |
| Mcbectb_Click | CMXsrv_expret_val_ret | ACMXDESEMB, ORG, COR, ACMXIMPUES, ACMXPRMGRL, CCL, ACMXPRMEXP, ACMXMONEDAFEC, COM, tbl_User, warnmsg, DTN, CLN, RET | CMXsrv_val_cta_cte, sp_procxmode, CMXsrv_enl_val_sel, CMXsrv_val_vig, CMXsrv_util_len, CMXsrv_lee_fpro |
| Mcbectb_Click | CMXsrv_expret_sum_dtn_mn | DTN, ACMXMONEDAFEC, RET, ACMXPRMENL | sp_procxmode |
| Mcbectb_Click | CMXsrv_expret_ctb_ing | ACMXDESEMB, ASND, PLV, ACMXPRMGRL, CCL, ACMXPRMEXP, PLI, tbl_User, DTN, CLN, RET | CMXsrv_mbyte_gen, CMXsrv_expret_grb_org, CMXsrv_expret_grb_dtn, CMXsrv_expret_cre_ret, CMXsrv_vig_gra_vig, CMXsrv_cnt_res_vig, CMXsrv_enl_act_enl, sp_cmx_sii_1862, sp_procxmode, CMXsrv_cnt_950, sp_cmx_sii_1870, CMXsrv_expret_val_ret, CMXsrv_expret_grb_det, CMXsrv_expret_cnt_cyg, CMXsrv_cnt_800, CMXsrv_expret_grb_evr, CMXsrv_cnt_810 |
| Mcbedel_Click | CMXsrv_expret_del_ret | ORG, COD, COM, DTN, RET | sp_procxmode |
| Mliqctb_Click | CMXsrv_expret_avs_adm1 | ACMXSUCSAL, ACMXMONEDA, CLN, RET | sp_procxmode |
| Mliqctb_Click | CMXsrv_expret_avs_adm2 | ORG, ACMXPRMEXP, RET | sp_procxmode |
| Mliqctb_Click | CMXsrv_expret_avs_adm3 | DTN, ACMXPRMEXP, RET | sp_procxmode |
| Mvalid_Click | CMXsrv_expret_val_ret | ACMXDESEMB, ORG, COR, ACMXIMPUES, ACMXPRMGRL, CCL, ACMXPRMEXP, ACMXMONEDAFEC, COM, tbl_User, warnmsg, DTN, CLN, RET | CMXsrv_val_cta_cte, sp_procxmode, CMXsrv_enl_val_sel, CMXsrv_val_vig, CMXsrv_util_len, CMXsrv_lee_fpro |
| ACEPTAR_Click | CMXsrv_expret_act_tpo_cbo | RET | sp_procxmode |
| ACEPTAR_Click | CMXsrv_expret_val_ret | ACMXDESEMB, ORG, COR, ACMXIMPUES, ACMXPRMGRL, CCL, ACMXPRMEXP, ACMXMONEDAFEC, COM, tbl_User, warnmsg, DTN, CLN, RET | CMXsrv_val_cta_cte, sp_procxmode, CMXsrv_enl_val_sel, CMXsrv_val_vig, CMXsrv_util_len, CMXsrv_lee_fpro |
| ACEPTAR_Click | CMXsrv_expret_cre_ret | RET | CMXsrv_util_num_ope, CMXsrv_cmx_busc_suc_usu, sp_procxmode, CMXsrv_lee_fpro |
| ACEPTAR_Click | CMXsrv_expret_grb_det | CLN, tbl_User, RET | sp_procxmode |
| fld_ret_mon_ret_LostFocus | CMXsrv_expret_tpo_cbo | ACMXMONEDAFEC | sp_procxmode, CMXsrv_lee_fpro |
| fld_ret_rut_cli_LostFocus | CMXsrv_expret_lee_cln | CLN | sp_procxmode |
| Form_Load | CMXsrv_expret_lee_det | ACMXSUCSAL, ACMXMONEDA, CLN, RET | sp_procxmode, CMXsrv_lee_fpro |
| ELIMINAR_Click | CMXsrv_expret_del_org | ORG, RET | sp_procxmode |
| Form_Activate | CMXsrv_expret_bus_org | ORG, RET | sp_procxmode |
| ACEPTAR_Click | CMXsrv_expret_grb_org | ACMXDESEMB, ORG, ACMXPLNCTAN, ACMXSRVEXT, ACMXPLNCTAX, RET | sp_procxmode |
| Form_Activate | CMXsrv_expret_mto_org | ORG, RET | sp_procxmode |
| Form_Activate | CMXsrv_expret_lee_org | ACMXDESEMB, ORG, COR, ACMXTPODOC, ACMXPAIS | sp_procxmode |
| valida_vigente | CMXsrv_vig_lee_cta | ACMXPLNCTAN, ACMXDESEMB, ACMXPLNCTAX | sp_procxmode |
| ELIMINAR_Click | CMXsrv_expret_del_dtn | DTN, RET | sp_procxmode |
| emitir_Click | CMXsrv_expret_swf_sel | DTN, ACMXPRMEXP, switxt, switxt1 | CMXsrv_expret_swf_202, CMXsrv_expret_swf_100, sp_procxmode |
| Form_Activate | CMXsrv_expret_bus_dtn | DTN, RET | sp_procxmode |
| ACEPTAR_Click | CMXsrv_expret_grb_dtn | ACMXDESEMB, ACMXPRMGRL, CCL, ACMXPRMEXP, DTN, RET | sp_procxmode |
| fld_ret_cod_ben_LostFocus | CMXsrv_expret_lee_cln | CLN | sp_procxmode |
| fld_ret_mto_arb_LostFocus | CMXsrv_expret_cal_arb | ACMXPRMGRL, ACMXMONEDA | sp_procxmode |
| fld_ret_mto_ben_LostFocus | CMXsrv_expret_cal_arb | ACMXPRMGRL, ACMXMONEDA | sp_procxmode |
| fld_ret_par_ben_LostFocus | CMXsrv_expret_cal_arb | ACMXPRMGRL, ACMXMONEDA | sp_procxmode |
| Form_Activate | CMXsrv_expret_mto_dtn | DTN, COM, RET, ACMXIMPUES | sp_procxmode |
| Form_Load | CMXsrv_expret_lee_dtn | ACMXPAIS, ACMXDESEMB, COR, DTN, ACMXMONEDA, APUCCODOPECMB, ACMXSUCSAL | sp_procxmode |
| Form_Load | CMXsrv_expret_lee_cln | CLN | sp_procxmode |
| buscar_Click | CMXsrv_expret_bus_ret | RET | sp_procxmode |
| fld_ret_rut_cli_LostFocus | CMXsrv_expret_lee_cln | CLN | sp_procxmode |
| proxima_Click | CMXsrv_expret_bus_ret | RET | sp_procxmode |
| Command1_Click | CMXsrv_expret_bus_evr | EVR, RET | sp_procxmode |
| Form_Activate | CMXsrv_expret_bus_evr | EVR, RET | sp_procxmode |
| proximo_Click | CMXsrv_expret_bus_evr | EVR, RET | sp_procxmode |
| reversar_Click | CMXsrv_expret_rev_ret | ORG, DTN, PLV, ACMXPRMEXP, PLI, TRSD, EVR, RET | CMXsrv_cnt_rev_vig, CMXsrv_cnt_811, CMXsrv_mbyte_gen, CMXsrv_ctl_chq_aprcbl, CMXsrv_rev_950, sp_cmx_sii_1862, sp_procxmode, CMXsrv_cnt_801, sp_cmx_sii_1870, CMXsrv_expret_rev_cyg, CMXsrv_expret_grb_evr, CMXsrv_enl_rev_enl |
| Form_Load | CMXsrv_expret_lee_evr | ACMXTIPEVE, EVR, ACMXSUCSAL | sp_procxmode |

---

## ADMIN
<a name="admin"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** | **Procedimientos Referenciados** |
|-------------|------------------------------|--------------------------|-------------------------------|
| COMMAND4_Click | CMXsrv_finadm_imod_desti | TIP | CMXsrv_finadm_val_tipop, sp_procxmode |
| Form_Load | CMXsrv_finadm_cons_dtip | TIP | sp_procxmode |
| Command1_Click | CMXsrv_finadm_imod_ectb | TIP | CMXsrv_finadm_val_tipop, sp_procxmode |
| Command2_Click | CMXsrv_finadm_eli_tipop | TIP, TIP_CTA | sp_procxmode |
| Form_Load | CMXsrv_finadm_cons_ectb | TIP | sp_procxmode |
| COMMAND3_Click | CMXsrv_finadm_eli_tipop | TIP, TIP_CTA | sp_procxmode |
| COMMAND4_Click | CMXsrv_finadm_imod_itip | TIP | CMXsrv_finadm_val_tipop, sp_procxmode |
| Form_Load | CMXsrv_finadm_cons_itip | TIP | sp_procxmode |
| Form_Activate | CMXsrv_finadm_lee_tipop | TIP, ACMXPLAZO, ACMXPROCMX, ACMXMB1 | sp_procxmode |
| Form_Load | CMXsrv_grl_fec_serv |  | SRV_MessageService, sp_procxmode |
| Mdel_Click | CMXsrv_finadm_eli_tipop | TIP, TIP_CTA | sp_procxmode |
| Mval_Click | CMXsrv_finadm_val_tipop | APEPROR, TIP, TAS, CUO, ACMXPLNCTAN, ACMXMONEDAFEC, PANCTL, ACLNCBCABCI, ACMXPLNCTAX, TIP_CTA, ACMXMONEDA, warnmsg, EVE, ACMXSUCSAL, PANVTO, ACMXINTEREFEC, COL, PANMOR | CMXsrv_fincol_eval_tbat, CMXsrv_util_fecha2, SRV_MessageService, sp_procxmode |
| buscar_Click | CMXsrv_finadm_bus_tipope | TIP | sp_procxmode |
| proximas_Click | CMXsrv_finadm_bus_tipope | TIP | sp_procxmode |

---

## COL_NEG
<a name="col_neg"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** | **Procedimientos Referenciados** |
|-------------|------------------------------|--------------------------|-------------------------------|
| CANCELAR_Click | CMXsrv_busc_tip_tas | CRD | sp_procxmode |
| ELIMINAR_Click | CMXsrv_fincol_ecuo | CUO_REN, COL, CUO | CMXsrv_fincol_pre_cuad_tas, sp_procxmode |
| Form_Activate | CMXsrv_fincol_cons_plnpa | CUO_REN, COL_REN, COL, CUO | sp_procxmode |
| Form_Load | CMXsrv_pertas_val_display | TAS | sp_procxmode |
| ELIMINAR_Click | CMXsrv_fincol_eava | DAC, AVAL, AVAL_REN, COL | sp_procxmode |
| Form_Activate | CMXsrv_fincol_cons_aval | CRDCLON, AVAL, AVAL_REN, COL | sp_procxmode |
| ingresar_Click | CMXsrv_fincol_iava | AVAL, AVAL_REN, CLN, COL | sp_procxmode |
| Form_Activate | CMXsrv_fincol_cons_pag | CAN, COL | sp_procxmode |
| proximos_Click | CMXsrv_fincol_cons_pag | CAN, COL | sp_procxmode |
| Form_Activate | CMXsrv_fincol_trae_det_pag | CAN, EVE | sp_procxmode |
| Form_Activate | CMXsrv_fincol_cons_pror | EVE, COL | sp_procxmode |
| Form_Activate | CMXsrv_fincol_cons_eve | EVE, COL | sp_procxmode |
| Aceptar_Click | CMXsrv_icrd_lee_bco_swf | ACMXPAIS, COR | CMXsrv_icrd_lee_cln, sp_procxmode |
| buscar_Click | CMXsrv_icrd_busc_bco | COR | sp_procxmode |
| proximo_Click | CMXsrv_icrd_busc_bco | COR | sp_procxmode |
| Aceptar_Click | CMXsrv_fincol_vtocre_prov | TIP, comex..ACMXINTEREFEC, COR, CRD, CUO, OBL, NEG, NEG_ADI, DAC, ACMXINTERE, ACMXMONEDA, ACMXINTEREFEC, AVAL, MYC, COL, CTO | CMXsrv_fincol_gpln, CMXsrv_finobl_imod_obl, CMXsrv_util_fecha, CMXsrv_util_val_tasas, CMXsrv_fincol_efec_calpa, sp_procxmode, CMXsrv_fincol_ctb_vcp, sp_cmx_sii_1870 |
| Form_Load | CMXsrv_fincol_prec_vtocre | TIP, CRD, CNEG, NEG, COL | sp_procxmode |
| buscar_Click | CMXsrv_icrd_bus_lcr_bco | COR | sp_procxmode |
| proximo_Click | CMXsrv_icrd_bus_lcr_bco | COR | sp_procxmode |
| Form_Load | CMXsrv_grl_fec_serv |  | SRV_MessageService, sp_procxmode |
| Form_Load | CMXsrv_lee_fpro | ACMXFECPRO | sp_procxmode |

---

## INGRESO
<a name="ingreso"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** | **Procedimientos Referenciados** |
|-------------|------------------------------|--------------------------|-------------------------------|
| cancelar_Click | CMXsrv_fincol_ren_fin | COL_REN, TIP, TAS, TAS_REN, EVE_REN, DAC_REN, ITA, CUO_REN, AVAL_REN, EVE, CAN_REN, COL | CMXsrv_cmx_fec_hoy, CMXsrv_fincol_pre_cuad_tas, sp_procxmode, CMXsrv_fincol_grb_col_ren, CMXsrv_lee_fpro |
| ELIMINAR_Click | CMXsrv_fincol_ecuo | CUO_REN, COL, CUO | CMXsrv_fincol_pre_cuad_tas, sp_procxmode |
| form_activate | CMXsrv_fincol_cons_plnpa | CUO_REN, COL_REN, COL, CUO | sp_procxmode |
| cancelar_Click | CMXsrv_fincol_ren_fin | COL_REN, TIP, TAS, TAS_REN, EVE_REN, DAC_REN, ITA, CUO_REN, AVAL_REN, EVE, CAN_REN, COL | CMXsrv_cmx_fec_hoy, CMXsrv_fincol_pre_cuad_tas, sp_procxmode, CMXsrv_fincol_grb_col_ren, CMXsrv_lee_fpro |
| ELIMINAR_Click | CMXsrv_fincol_eava | DAC, AVAL, AVAL_REN, COL | sp_procxmode |
| form_activate | CMXsrv_fincol_cons_aval | CRDCLON, AVAL, AVAL_REN, COL | sp_procxmode |
| aceptar_Click | CMXsrv_fincol_gmod_ctr | TIP, CUO, OBL, CTR, CLN, COL, CTO | sp_procxmode |
| busca_bco | CMXsrv_icrd_lee_bco_swf | ACMXPAIS, COR | CMXsrv_icrd_lee_cln, sp_procxmode |
| fld_obl_bco_acr_LostFocus | CMXsrv_fincol_lee_bco | COR | sp_procxmode |
| fld_obl_rut_acr_LostFocus | CMXsrv_fincol_lee_cln | CLN | sp_procxmode |
| form_activate | CMXsrv_fincol_cons_ctr | OBL, CTR | sp_procxmode |
| aceptar_Click | CMXsrv_fincol_ctb_oto | TIP, ACMXDESEMB, CUO, COD, vig_cmx, COL_ADI, ACMXPRMGRL, OBL, COM, MYC, ACMXMONEDA, LIB, OPE_BCI, CLN, COL, CCO | CMXsrv_mbyte_gen, CMXsrv_cmx_ing_lib, CMXsrv_ctb_impto_tim, CMXsrv_ctb_otorga, CMXsrv_cnt_gen_vig, CMXsrv_nibx_upd_tran, CMXsrv_ctb_impto_tim2, CMXsrv_vig_gra_vig, CMXsrv_nibx_nilive, CMXsrv_cyo_dsc, sp_procxmode, CMXsrv_fincol_val_col, CMXsrv_cnt_999999, sp_cmx_sii_1870, CMXsrv_util_pesos, CMXsrv_lee_fpro |
| Avi5_Click | CMXsrv_icrd_dat_liq_ope | ACMXDESEMB, ASND, EVO, CRD, CNO, OBL, CUO, TRSD, NEG, COM, EVE, ACMXTIPEVE, CAN, COL | sp_procxmode |
| form_activate | CMXsrv_fincol_lee_col | COR, TAS, NEG_ADI, ACMXINTERE, TIP, CUO, CCL, ACMXFINVER, ACMXAPROBAC, COL_ADI, ACMXACTIVIDA, ACMXINTEREFEC, AVAL, ACMXSUCSAL, CLN, comex..ACMXINTEREFEC, COM, ACMXMONEDA, EVE, tbl_User, COL | PrmACMXESPECI, PrmACLNEJECTA, sp_procxmode |
| Form_Load | CMXsrv_lee_fpro | ACMXFECPRO | sp_procxmode |
| MCOLCOMI_CLICK | CMXsrv_busc_cod_ope | TIP, COL | sp_procxmode |
| MCOLCOMI_CLICK | CMXsrv_col_trae_num_ope | COL | sp_procxmode |
| MCOLCONTOTOR_CLICK | CMXsrv_busc_cod_ope | TIP, COL | sp_procxmode |
| MCOLCONTOTOR_CLICK | CMXsrv_col_trae_num_ope | COL | sp_procxmode |
| MCOLCONTOTOR_CLICK | CMXsrv_fincol_ctb_oto | TIP, ACMXDESEMB, CUO, COD, vig_cmx, COL_ADI, ACMXPRMGRL, OBL, COM, MYC, ACMXMONEDA, LIB, OPE_BCI, CLN, COL, CCO | CMXsrv_mbyte_gen, CMXsrv_cmx_ing_lib, CMXsrv_ctb_impto_tim, CMXsrv_ctb_otorga, CMXsrv_cnt_gen_vig, CMXsrv_nibx_upd_tran, CMXsrv_ctb_impto_tim2, CMXsrv_vig_gra_vig, CMXsrv_nibx_nilive, CMXsrv_cyo_dsc, sp_procxmode, CMXsrv_fincol_val_col, CMXsrv_cnt_999999, sp_cmx_sii_1870, CMXsrv_util_pesos, CMXsrv_lee_fpro |
| MCOLELI_CLICK | CMXsrv_fincol_eli_col | COL_REN, COL_ADI, COM, TAS_REN, DAC_REN, EVE_REN, DAC, CUO_REN, AVAL_REN, LIB, CAN_REN, COL | sp_procxmode |
| valida | CMXsrv_fincol_val_col | TIP, COL, warnmsg | CMXsrv_fincol_val_err, CMXsrv_fincol_val_per_tas, CMXsrv_fincol_val_adv, sp_procxmode |
| aceptar_Click | CMXsrv_fincol_lee_col | COR, TAS, NEG_ADI, ACMXINTERE, TIP, CUO, CCL, ACMXFINVER, ACMXAPROBAC, COL_ADI, ACMXACTIVIDA, ACMXINTEREFEC, AVAL, ACMXSUCSAL, CLN, comex..ACMXINTEREFEC, COM, ACMXMONEDA, EVE, tbl_User, COL | PrmACMXESPECI, PrmACLNEJECTA, sp_procxmode |
| buscar_Click | CMXsrv_fincol_bsc_col | TIP | sp_procxmode |
| fld_col_tip_ope_lostfocus | CMXsrv_fincol_lee_tip | TIP | sp_procxmode |
| PROXIMAS_Click | CMXsrv_fincol_bsc_col | TIP | sp_procxmode |
| ingresar_Click | CMXsrv_fincol_iava | AVAL, AVAL_REN, CLN, COL | sp_procxmode |
| aceptar_Click | CMXsrv_busc_cod_ope | TIP, COL | sp_procxmode |
| aceptar_Click | CMXsrv_col_trae_num_ope | COL | sp_procxmode |
| aceptar_Click | CMXsrv_fincol_ctb_novf | CLN, COL | CMXsrv_fincol_ctb_nov, sp_procxmode, CMXsrv_lee_fpro |
| FLD_COL_COD_CLI_LOSTFOCUS | CMXsrv_fincol_lee_cln | CLN | sp_procxmode |
| FLD_COL_RUT_DEU_NOV_LostFocus | CMXsrv_fincol_lee_cln | CLN | sp_procxmode |
| form_activate | CMXsrv_fincol_cons_nov | EVE, COL | sp_procxmode |
| FLD_COL_COD_CLI_LOSTFOCUS | CMXsrv_fincol_lee_cln | CLN | sp_procxmode |
| FLD_COL_RUT_DEU_NOV_LostFocus | CMXsrv_fincol_lee_cln | CLN | sp_procxmode |
| Aceptar_Click | CMXsrv_icrd_lee_bco_swf | ACMXPAIS, COR | CMXsrv_icrd_lee_cln, sp_procxmode |
| buscar_Click | CMXsrv_icrd_busc_bco | COR | sp_procxmode |
| proximo_Click | CMXsrv_icrd_busc_bco | COR | sp_procxmode |
| Form_Load | CMXsrv_cmx_get_codes |  | sp_procxmode |
| Form_Load | CMXsrv_grl_trae_cod_bco |  | sp_procxmode |

---

## MODIFIC
<a name="modific"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** | **Procedimientos Referenciados** |
|-------------|------------------------------|--------------------------|-------------------------------|
| Form_Activate | CMXsrv_fincol_cons_tas | TAS | sp_procxmode |
| aceptar_click | CMXsrv_fincol_efec_tras | TIP, comex..ACMXMONEDAFEC, COL, CUO | CMXsrv_fincol_ctb_cnd, CMXsrv_fincol_ctb_cob, CMXsrv_cnt_9000, CMXsrv_fincol_ctb_cst, sp_procxmode, CMXsrv_fincol_calc_cven |
| Form_Activate | CMXsrv_fincol_cons_trasp | EVE, COL | sp_procxmode |
| Form_Activate | CMXsrv_fincol_cons_dtrs | EVE, COL | sp_procxmode |
| Form_Activate | CMXsrv_fincol_cons_eve | EVE, COL | sp_procxmode |
| Form_Load | CMXsrv_fincol_cons_deve | EVE, COL | sp_procxmode |
| aceptar_click | CMXsrv_fincol_cont_gst |  | sp_procxmode |
| Form_Activate | CMXsrv_fincol_cons_gst | EVE, COL | sp_procxmode |
| Form_Activate | CMXsrv_fincol_cons_dgst |  | sp_procxmode |
| Form_Load | CMXsrv_lee_fpro | ACMXFECPRO | sp_procxmode |

---

## OBLIGA
<a name="obliga"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** | **Procedimientos Referenciados** |
|-------------|------------------------------|--------------------------|-------------------------------|
| buscar_Click | CMXsrv_fincol_bsc_tip | TIP | sp_procxmode |
| Proxima_Click | CMXsrv_fincol_bsc_tip | TIP | sp_procxmode |
| proximo_Click | CMXsrv_fincol_bsc_tip | TIP | sp_procxmode |
| buscar_Click | CMXsrv_finobl_bus_cor | COR | sp_procxmode |
| proximo_Click | CMXsrv_finobl_bus_cor | COR | sp_procxmode |
| ELIMINAR_Click | CMXsrv_finobl_ecuo | OBL, CTO | sp_procxmode |
| form_activate | CMXsrv_finobl_gpln | OBL, CTO | CMXsrv_util_det_habil_tasa, sp_procxmode |
| form_activate | CMXsrv_finobl_cons_plnpa | OBL, CTO | sp_procxmode |
| anunctb_Click | CMXsrv_finobl_calc_anu | OBL | sp_procxmode, CMXsrv_finobl_efec_calpa, CMXsrv_lee_fpro |
| form_activate | CMXsrv_finobl_lee_obl | TIP, COR, OBL, ACMXINTERE, ACMXMONEDA, ACMXSUCSAL, CLN | sp_procxmode |
| Form_Load | CMXsrv_lee_fpro | ACMXFECPRO | sp_procxmode |
| Mcbeanl_Click | CMXsrv_finobl_calc_anu | OBL | sp_procxmode, CMXsrv_finobl_efec_calpa, CMXsrv_lee_fpro |
| Mcbectb_Click | CMXsrv_finobl_ctb_oto | ACMXDESEMB, TIP, COD, OBL, CTO, CCO | CMXsrv_ctbo_otorga, CMXsrv_finobl_val_obl, sp_procxmode, CMXsrv_lee_fpro |
| Mcbedel_Click | CMXsrv_fincol_eli_obl | OBL, OBL_ADI | sp_procxmode |
| Mobl_liq_ope_Click | CMXsrv_icrd_dat_liq_ope | ACMXDESEMB, ASND, EVO, CRD, CNO, OBL, CUO, TRSD, NEG, COM, EVE, ACMXTIPEVE, CAN, COL | sp_procxmode |
| valida_error | CMXsrv_finobl_val_obl | TIP, OBL, ACMXINTERE, warnmsg, OBL_ADI | CMXsrv_util_det_habil_tasa, CMXsrv_finobl_val_adv, sp_procxmode |
| buscar_Click | CMXsrv_finobl_bsc_obl | OBL | CMXsrv_finobl_bsc_obl2, sp_procxmode, CMXsrv_finobl_bsc_obl3 |
| fld_obl_tip_ope_LostFocus | CMXsrv_fincol_lee_tip | TIP | sp_procxmode |
| Proxima_Click | CMXsrv_finobl_bsc_obl | OBL | CMXsrv_finobl_bsc_obl2, sp_procxmode, CMXsrv_finobl_bsc_obl3 |
| contabilizar_Click | CMXsrv_finobl_ictb_pag | OBL, CTO, EVO | CMXsrv_finobl_ctb_pag, sp_procxmode, CMXsrv_lee_fpro |
| contabilizar_Click | CMXsrv_finobl_obt_sdocuo | OBL, CTO | sp_procxmode |
| form_activate | CMXsrv_finobl_new_tas | CTO | sp_procxmode |
| form_activate | CMXsrv_finobl_cons_pag | CNO | sp_procxmode |
| form_activate | CMXsrv_finobl_cons_detp | OBL, CTO, EVO | sp_procxmode |
| calcular_Click | CMXsrv_finobl_calc_pror | OBL | sp_procxmode, CMXsrv_finobl_efec_calpa, CMXsrv_lee_fpro |
| form_activate | CMXsrv_finobl_cons_pror | OBL, EVO | sp_procxmode |
| form_activate | CMXsrv_finobl_cons_dpror | OBL, EVO | sp_procxmode |
| contabilizar_Click | CMXsrv_finobl_ctb_anu | TIP, COR, OBL, COL, CTO | CMXsrv_finobl_cbo_anu, CMXsrv_ctbo_anula, sp_procxmode, CMXsrv_lee_fpro |
| calcular_Click | CMXsrv_finobl_calc_anu | OBL | sp_procxmode, CMXsrv_finobl_efec_calpa, CMXsrv_lee_fpro |
| form_activate | CMXsrv_finobl_cons_anu | CNO, EVO | sp_procxmode |
| form_activate | CMXsrv_finobl_cons_mod | OBL, EVO | sp_procxmode |
| form_activate | CMXsrv_finobl_cons_dmod | CNO, EVO | sp_procxmode |
| efectuar_Click | CMXsrv_finobl_rev_eve | OBL, TRSD, APRCBL, EVO | CMXsrv_ctl_marc_rev, CMXsrv_ctl_chq_aprcbl, CMXsrv_finobl_rctb_pext, CMXsrv_rctb_cesi, sp_procxmode, CMXsrv_finobl_rctb_pag, CMXsrv_finobl_rctb_pror, CMXsrv_finobl_rctb_mod, CMXsrv_finobl_rctb_anu, CMXsrv_finobl_rctb_oto |
| form_activate | CMXsrv_finobl_cons_eve | EVO | sp_procxmode |
| form_activate | CMXsrv_finobl_cons_deve | EVO | sp_procxmode |
| ELIMINAR_Click | CMXsrv_finobl_eli_ctr | CTR | sp_procxmode |
| form_activate | CMXsrv_finobl_cons_ctr | CTR | sp_procxmode |
| nuevo_Click | CMXsrv_finobl_ing_ctr | COL, OBL, TIP, CTR | sp_procxmode |
| aceptar_Click | CMXsrv_finobl_cesion_obl | OBL, COR | CMXsrv_ctl_crea_apr, sp_procxmode, CMXsrv_lee_fpro |
| banco_acreedor | CMXsrv_comgrl_lee_nom_cor | COR | sp_procxmode |
| fld_obl_cod_bco_acre_lostfocus | CMXsrv_comgrl_lee_nom_cor | COR | sp_procxmode |
| fld_obl_rut_acre_lostfocus | CMXsrv_lee_cln | CLN | sp_procxmode |
| form_activate | CMXsrv_finobl_busc_acre | OBL | sp_procxmode |
| Form_Load | CMXsrv_cmx_get_codes |  | sp_procxmode |

---

## PAGOS
<a name="pagos"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** | **Procedimientos Referenciados** |
|-------------|------------------------------|--------------------------|-------------------------------|
| CALCULAR_Click | CMXsrv_fincol_efec_calpa | TF_PPAG, TIP, TAS, CUO, comex..ACMXMONEDA, COL_ADI, OBL, CTR, NEG_ADI, ACMXINTERE, CAN, ICR, COL | CMXsrv_fincol_eval_tnem, CMXsrv_fincol_eval_tmor, CMXsrv_util_det_habil, sp_procxmode, CMXsrv_fincol_calc_reba, CMXsrv_fincol_eval_tasa, CMXsrv_fincol_eval_tneg, CMXsrv_fincol_efcal_cv, CMXsrv_fincol_cal_tas_sfr |
| Form_Activate | CMXsrv_fincol_cons_pag | CAN, COL | sp_procxmode |
| Form_Load | CMXsrv_fincol_cons_detp | ACMXDESEMB, EVE, COL, CUO | sp_procxmode |
| Aceptar_Click | CMXsrv_fincol_calc_pror | ACMXINTERE, COL | CMXsrv_call_val_tas, sp_procxmode, CMXsrv_fincol_efec_calpa |
| Contabilizar_Click | CMXsrv_fincol_cont_pror | TAS, CRD, NEG_ADI, ACMXINTERE, TIP, CUO, OBL, CAM_TAS, ACMXPLAZO, COL_ADI, LIB, ACMXINTEREFEC, CLN, ACMXOPEIMP, CTO, de, comex..ACMXINTEREFEC, COD, COM, ACMXMONEDAFEC, EVE, CAN, COL | CMXsrv_mbyte_gen, CMXsrv_fincol_ctb_pror, CMXsrv_get_ult_dia_habil, CMXsrv_cmx_ing_lib, CMXsrv_ctb_impto_tim, CMXsrv_ipuc_gen_pln, CMXsrv_util_val_tasas, sp_procxmode, CMXsrv_pertas_pror_tas, CMXsrv_cmx_get_codes, CMXsrv_int_ccx_cns, CMXsrv_util_pesos, CMXsrv_fincol_cam_new_tas, CMXsrv_lee_fpro |
| Form_Activate | CMXsrv_fincol_cons_pror | EVE, COL | sp_procxmode |
| Form_Activate | CMXsrv_fincol_cons_dpror | ACMXDESEMB, EVE, COL | sp_procxmode |
| Aceptar_Click | CMXsrv_busc_cod_ope | TIP, COL | sp_procxmode |
| Aceptar_Click | CMXsrv_col_trae_num_ope | COL | sp_procxmode |
| Aceptar_Click | CMXsrv_fincol_cctb_anu | TIP, CUO, COD, OBL, TF_ENL, ENL, CAN, COL, CTO | CMXsrv_busc_cod_ope, CMXsrv_enl_act_enl, sp_procxmode, CMXsrv_fincol_ctb_anu, sp_cmx_sii_1870, CMXsrv_lee_fpro |
| Form_Load | CMXsrv_fincol_calc_anu | TIP, COL | sp_procxmode, CMXsrv_fincol_efec_calpa |
| Form_Load | CMXsrv_busc_cod_ope | TIP, COL | sp_procxmode |
| CALCULAR_Click | CMXsrv_fincol_calc_anu | TIP, COL | sp_procxmode, CMXsrv_fincol_efec_calpa |
| Form_Activate | CMXsrv_fincol_cons_anu | ACMXDESEMB, CAN, EVE, COL | sp_procxmode |
| Form_Activate | CMXsrv_fincol_cons_mod | EVE, COL | sp_procxmode |
| Form_Activate | CMXsrv_fincol_cons_dmod | CAN, EVE | sp_procxmode |
| Form_Load | CMXsrv_lee_fpro | ACMXFECPRO | sp_procxmode |
| Form_Load | CMXsrv_grl_trae_cod_bco |  | sp_procxmode |

---

## PGOEXT
<a name="pgoext"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** | **Procedimientos Referenciados** |
|-------------|------------------------------|--------------------------|-------------------------------|
| calcular_Click | CMXsrv_fincol_cal_pext | TIP, CUO, comex..ACMXMONEDA, OBL, CTR, COL, CTO | CMXsrv_fincol_calc_reba, CMXsrv_fincol_eval_tasa, sp_procxmode |
| Contabilizar_Click | CMXsrv_busc_cod_ope | TIP, COL | sp_procxmode |
| Contabilizar_Click | CMXsrv_fincol_ctb_pext | TIP, ACMXDESEMB, comex..ACMXINTEREFEC, TAS, CUO, COD, OBL, COL_ADI, ACMXMONEDAFEC, CTR, NEG_ADI, ACMXINTERE, EVE, ACMXINTEREFEC, COL, CTO, CCO | CMXsrv_ctb_pago, CMXsrv_util_gen_vig, sp_procxmode, CMXsrv_lee_fpro |
| calcular_Click | CMXsrv_finobl_cal_pext | TIP, OBL, ACMXINTERE, ACMXMONEDA, OBL_ADI, CTO | CMXsrv_finobl_eval_tasa, sp_procxmode, CMXsrv_fincol_cal_tas_sfr |
| Contabilizar_Click | CMXsrv_finobl_ctb_pext | ACMXDESEMB, TIP, COD, OBL, ACMXMONEDAFEC, CTO, CCO | CMXsrv_ctbo_pago, sp_procxmode, CMXsrv_lee_fpro |
| Form_Load | CMXsrv_grl_fec_serv |  | SRV_MessageService, sp_procxmode |
| Form_Load | CMXsrv_lee_fpro | ACMXFECPRO | sp_procxmode |

---

## ARCOS
<a name="arcos"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** | **Procedimientos Referenciados** |
|-------------|------------------------------|--------------------------|-------------------------------|
| Eliminar_Click | CMXsrv_iarc_eli_arc | ADI, CRD, ARC, NEG, COB, INF, COL | sp_procxmode |
| Form_activate | CMXsrv_iarc_busc_arc | ARC | sp_procxmode |
| aceptar_click | CMXsrv_iinf_busc_inf | INF | sp_procxmode |
| aceptar_click | CMXsrv_iarc_act_arc | CRD, comex..ACMXMONEDA, ARC, NEG, CBR, ACMXMONEDAFEC, INF, COL | CMXsrv_cmx_get_codes, PrmACMXMONEDAFEC, CMXsrv_util_opr_fec, sp_procxmode |
| Form_Load | CMXsrv_iarc_lee_arc | ARC | sp_procxmode |
| buscar_Click | CMXsrv_iinf_busc_opr | ARC | sp_procxmode |
| Form_activate | CMXsrv_iinf_lee_vlr | INF | PrmACMXCLACOM, sp_procxmode |
| aceptar_click | CMXsrv_iarc_act_arc | CRD, comex..ACMXMONEDA, ARC, NEG, CBR, ACMXMONEDAFEC, INF, COL | CMXsrv_cmx_get_codes, PrmACMXMONEDAFEC, CMXsrv_util_opr_fec, sp_procxmode |
| Form_activate | CMXsrv_iinf_busc_inf | INF | sp_procxmode |
| reversar_Click | CMXsrv_iinf_rev_evi | INF, ARC, INC, EVI | CMXsrv_com_rev, sp_procxmode |

---

## COBERIMP
<a name="coberimp"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** | **Procedimientos Referenciados** |
|-------------|------------------------------|--------------------------|-------------------------------|
| Form_Activate | CMXsrv_icob_lee_pln | DIC, POSBCX10, COB, ACMXBCOCEN, ACMXMONEDA, ACMXPAIS | CMXsrv_cmx_get_codes, CMXsrv_icob_obs_pln, sp_procxmode |
| Mcobcur_Click | CMXsrv_icob_cur_cob | comex.dbo, COB | CMXsrv_icob_ctb_reem, sp_procxmode, CMXsrv_icob_val_cob |
| Mcobcur_Click | CMXsrv_icob_pag_sop | DDI, ACMXDESEMB, ADI, DIC, ACMXPRMGRL, ACMXMONEDAFEC, COB, INF, warnmsg | CMXsrv_get_ult_dia_habil, CMXsrv_icob_refresh_pos, CMXsrv_val_cta_cte, CMXsrv_calc_imp_4pct, CMXsrv_icbr_act_rem, sp_procxmode, CMXsrv_icob_ctb_sop, CMXsrv_ctb_imp_ddi_so, CMXsrv_cmx_get_codes, CMXsrv_iddi_marc_ddi2, CMXsrv_icob_val_cob |
| MCOBELI_CLICK | CMXsrv_icob_eli_pln | COB | sp_procxmode |
| Mcobrev_Click | CMXsrv_icob_rev_etd | POSBCX10, TRSD, PSO, comex..COB, COB | CMXsrv_icob_refresh_pos, CMXsrv_ctl_chq_aprcbl, CMXsrv_icob_ctb_anu, CMXsrv_icob_ctb_reem, sp_procxmode, CMXsrv_pos_eli_010, CMXsrv_icob_rctb_sop |
| Mcobvali_Click | CMXsrv_icob_val_cob | DDI, LCB, ADI, CUO, ARC, NEG, CBR, COB, INF, ACMXFPAIMP, warnmsg, COL | PrmACMXPAIS, CMXsrv_pos_bcx_lee_cob, CMXsrv_util_fecha, sp_procxmode |
| buscar_click | CMXsrv_icob_busc_pln | COB | sp_procxmode |
| FLD_COB_COD_CLI_LostFocus | CMXsrv_icob_lee_cln | CLN | sp_procxmode |
| PROXIMAS_Click | CMXsrv_icob_busc_pln | COB | sp_procxmode |
| ACEPTAR_Click | CMXsrv_icob_crea_norm | CRD, ARC, CBR, COB, INF, tbl_User, CLN, COL | sp_procxmode, CMXsrv_icob_get_num |
| ACEPTAR_Click | CMXsrv_icob_crea_reem | DIC, COB | sp_procxmode, CMXsrv_icob_get_num, CMXsrv_cmx_get_codes, CMXsrv_pos_bcx_lee_cob, CMXsrv_pos_bcx_ing_cob |
| ACEPTAR_Click | CMXsrv_icob_act_gral | CLN, COB | sp_procxmode, CMXsrv_icob_num_con, CMXsrv_icob_val_cob, CMXsrv_pos_bcx_act_cob |
| FLD_COB_COD_CLI_LostFocus | CMXsrv_icob_lee_cln2 | CLN | sp_procxmode |
| Form_Activate | CMXsrv_icob_lee_gral | ACMXBCOCEN, ACMXPAIS, COB | CMXsrv_pos_bcx_lee_cob, sp_procxmode |
| ACEPTAR_Click | CMXsrv_icob_act_val | ACMXMONEDAFEC, COB | CMXsrv_get_ult_dia_habil, sp_procxmode, CMXsrv_icob_val_cob |
| Form_Activate | CMXsrv_icob_lee_val | COB | sp_procxmode |
| ACEPTAR_Click | CMXsrv_icob_act_acu | COB | sp_procxmode, CMXsrv_icob_val_cob |
| Form_Activate | CMXsrv_icob_lee_acu | ACMXPAIS, COB | sp_procxmode |
| Form_Load | CMXsrv_icob_lee_acu | ACMXPAIS, COB | sp_procxmode |
| ELIMINAR_Click | CMXsrv_icob_eli_int | DIC, COB | sp_procxmode |
| Form_Activate | CMXsrv_icob_busc_int | DIC | sp_procxmode |
| ACEPTAR_Click | CMXsrv_icob_ingmod_int | DIC, COB | PrmACMXMONEDA, sp_procxmode, CMXsrv_icob_val_cob |
| Form_Activate | CMXsrv_icob_lee_int | DIC | sp_procxmode |
| ACEPTAR_Click | CMXsrv_icob_ing_mod_srf | CLN, tbl_User, COB | CMXsrv_pos_bcx_ing_cob, sp_procxmode, CMXsrv_icob_get_num, CMXsrv_pos_bcx_act_cob |
| CmdEliminar_Click | CMXsrv_icob_eli_pln | COB | sp_procxmode |
| CmdReversar_Click | CMXsrv_icob_rev_etd | POSBCX10, TRSD, PSO, comex..COB, COB | CMXsrv_icob_refresh_pos, CMXsrv_ctl_chq_aprcbl, CMXsrv_icob_ctb_anu, CMXsrv_icob_ctb_reem, sp_procxmode, CMXsrv_pos_eli_010, CMXsrv_icob_rctb_sop |
| CURSAR_Click | CMXsrv_icob_ing_mod_srf | CLN, tbl_User, COB | CMXsrv_pos_bcx_ing_cob, sp_procxmode, CMXsrv_icob_get_num, CMXsrv_pos_bcx_act_cob |
| CURSAR_Click | CMXsrv_icob_pag_sop | DDI, ACMXDESEMB, ADI, DIC, ACMXPRMGRL, ACMXMONEDAFEC, COB, INF, warnmsg | CMXsrv_get_ult_dia_habil, CMXsrv_icob_refresh_pos, CMXsrv_val_cta_cte, CMXsrv_calc_imp_4pct, CMXsrv_icbr_act_rem, sp_procxmode, CMXsrv_icob_ctb_sop, CMXsrv_ctb_imp_ddi_so, CMXsrv_cmx_get_codes, CMXsrv_iddi_marc_ddi2, CMXsrv_icob_val_cob |
| FLD_COB_COD_CLI_LostFocus | CMXsrv_icob_lee_cln2 | CLN | sp_procxmode |
| Reversar_Click | CMXsrv_icob_rev_etd | POSBCX10, TRSD, PSO, comex..COB, COB | CMXsrv_icob_refresh_pos, CMXsrv_ctl_chq_aprcbl, CMXsrv_icob_ctb_anu, CMXsrv_icob_ctb_reem, sp_procxmode, CMXsrv_pos_eli_010, CMXsrv_icob_rctb_sop |
| ACEPTAR_Click | CMXsrv_icob_anu | DIC, POSBCX10, ACMXMONEDAFEC, PSO, COB, ACMXTPOAUTN | CMXsrv_get_ult_dia_habil, CMXsrv_icob_refresh_pos, CMXsrv_icob_ctb_anu, sp_procxmode, CMXsrv_pos_bcx_act_cob, CMXsrv_icob_get_num, CMXsrv_cmx_get_codes, CMXsrv_pos_bcx_lee_cob, CMXsrv_pos_bcx_ing_cob |
| Form_Load | CMXsrv_icob_lee_anu | COB | CMXsrv_pos_bcx_lee_cob, sp_procxmode |
| FLD_COB_COD_CLI_LostFocus | CMXsrv_icob_lee_cln | CLN | sp_procxmode |
| ACEPTAR_Click | CMXsrv_icob_pag_sop | DDI, ACMXDESEMB, ADI, DIC, ACMXPRMGRL, ACMXMONEDAFEC, COB, INF, warnmsg | CMXsrv_get_ult_dia_habil, CMXsrv_icob_refresh_pos, CMXsrv_val_cta_cte, CMXsrv_calc_imp_4pct, CMXsrv_icbr_act_rem, sp_procxmode, CMXsrv_icob_ctb_sop, CMXsrv_ctb_imp_ddi_so, CMXsrv_cmx_get_codes, CMXsrv_iddi_marc_ddi2, CMXsrv_icob_val_cob |
| ACEPTAR_Click | CMXsrv_icob_cur_reem | comex..COB, COB | CMXsrv_icob_ctb_reem, sp_procxmode, CMXsrv_icob_refresh_pos, CMXsrv_icob_val_cob |
| Form_Load | CMXsrv_grl_fec_serv |  | SRV_MessageService, sp_procxmode |

---

## COBRANZA
<a name="cobranza"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** | **Procedimientos Referenciados** |
|-------------|------------------------------|--------------------------|-------------------------------|
| ejecut_avi_imp_999 | CMXsrv_busc_cor_swf | SWT | sp_procxmode |
| ejecut_avi_imp_999 | CMXsrv_swf_bus_sms | SMS | sp_procxmode |
| Form_Activate | CMXsrv_icbr_lee_cbr | ACMXPAIS, COR, LCB, ACMXVIATPT, ACMXBCOBCC, CBR, ACMXMONEDA, ACMXCLACOM, tbl_User, ACMXSUCSAL, CLN | PrmACMXESPECI, PrmACLNEJECTA, sp_procxmode |
| Form_Load | CMXsrv_grl_fec_serv |  | SRV_MessageService, sp_procxmode |
| Mcbrace_Click | CMXsrv_icbr_acep_let | comex..CBR, LCB, CBR | CMXsrv_ctl_crea_apr, sp_procxmode |
| Mcbrcon_Click | CMXsrv_icbr_cont_cbr | OPE_BCI, APRCBL, LCB, CBR | CMXsrv_ctl_marc_firma, CMXsrv_mbyte_gen, CMXsrv_icbr_val_cbr, CMXsrv_nibx_upd_tran, CMXsrv_cnt_gen_vig, sp_procxmode, CMXsrv_ctb_cbr, CMXsrv_nibx_nilive |
| Mcbreli_click | CMXsrv_icbr_eli_cbr | ARC, REMENT, CBR, comex..COL | sp_procxmode |
| McbrTxt999_Click | CMXsrv_icbr_lee_ctp | ACMXSUCSAL, MCBRCTP, CBR, ACMXPAIS, CLN, CBRANX | sp_procxmode |
| Mcbrtxtrec_Click | CMXsrv_icbr_avi1 | ACMXDESEMB, ASND, ACMXBCOBCC, ARC, CBR, ACMXINTERE, PCX, ECE, ACMXMONEDA, ACMXSUCSAL, CLN | sp_procxmode |
| aceptar_Click | CMXsrv_val_suc | ACMXSUCSAL, tbl_User | sp_procxmode |
| buscar_Click | CMXsrv_icbr_busc_cbr | ACMXSUCSAL, ACMXMONEDA, CLN, CBR | sp_procxmode |
| fld_aux_glo_ofi_LostFocus | CMXsrv_val_suc | ACMXSUCSAL, tbl_User | sp_procxmode |
| fld_cbr_cod_gdo_LostFocus | CMXsrv_icbr_lee_cln | CLN | sp_procxmode |
| fld_cbr_cod_ofi_lostfocus | CMXsrv_val_suc | ACMXSUCSAL, tbl_User | sp_procxmode |
| proximas_Click | CMXsrv_icbr_busc_cbr | ACMXSUCSAL, ACMXMONEDA, CLN, CBR | sp_procxmode |
| crear_Click | CMXsrv_icbr_crea_cbr | CLN, tbl_User | srv_icbr_asig_num, sp_procxmode, CMXsrv_util_num_ope |
| fld_cbr_cod_gdo_LostFocus | CMXsrv_icbr_lee_cln | CLN | sp_procxmode |
| fld_cbr_cod_ofi_lostfocus | CMXsrv_val_suc | ACMXSUCSAL, tbl_User | sp_procxmode |
| INGRESAR_Click | CMXsrv_icbr_crea_cbr | CLN, tbl_User | srv_icbr_asig_num, sp_procxmode, CMXsrv_util_num_ope |
| fld_cbr_cod_gdo_LostFocus | CMXsrv_icbr_lee_cln | CLN | sp_procxmode |
| Form_Activate | CMXsrv_icbr_lee_cob | COB | sp_procxmode |
| Form_Load | CMXsrv_icbr_lee_ctp | ACMXSUCSAL, MCBRCTP, CBR, ACMXPAIS, CLN, CBRANX | sp_procxmode |
| INGRESAR_Click | CMXsrv_icbr_act_ctp | comex..CBR, MCBRCTP, CBRANX, CBR | sp_procxmode |
| Form_Activate | CMXsrv_icbr_lee_cob | COB | sp_procxmode |
| Form_Load | CMXsrv_icbr_lee_trm | ACMXVIATPT, CBR, ACMXINTERE, ACMXMONEDA, MCBRTER, ACMXCLACOM, ACMXPAIS | sp_procxmode |
| INGRESAR_Click | CMXsrv_icbr_act_trm | LCB, COM, CBR, MCBRTER, warnmsg, CLN | CMXsrv_util_fecha, CMXsrv_icbr_val_cbr, sp_procxmode |
| Form_Activate | CMXsrv_icbr_lee_cob | COB | sp_procxmode |
| Form_Load | CMXsrv_icbr_lee_doc | LCB, MCBRDOC, MLCB, CBR, ACMXMONEDA | sp_procxmode |
| INGRESAR_Click | CMXsrv_icbr_act_doc | LCB, MCBRDOC, MLCB, CBR, comex..CBR | sp_procxmode |
| Form_Activate | CMXsrv_icbr_busc_let | MLCB, comex..MLCB, comex..LCB | sp_procxmode |
| aceptar_Click | CMXsrv_icbr_ingmod_let | LCB, CBR, comex.dbo | CMXsrv_util_fecha, sp_procxmode |
| eliminar_Click | CMXsrv_icbr_eli_let | LCB, MCBRDOC, MLCB, CBR, comex..COL | sp_procxmode |
| Form_Activate | CMXsrv_icbr_lee_let | ACMXNOTARIO, LCB, MLCB | sp_procxmode |
| aceptar_Click | CMXsrv_icbr_prorr | comex..CBR, LCB, CBR | CMXsrv_util_fecha, CMXsrv_cnt_2600, sp_procxmode, CMXsrv_cnt_2610, CMXsrv_cnt_2620 |
| EFECTUAR_Click | CMXsrv_icbr_rev_eve | APRCBL, TRSD, CBR, vig_trs, ECE, DIP, LIB, tbl_User | CMXsrv_icbr_rev_mod_cbr, CMXsrv_mbyte_gen, CMXsrv_ctl_marc_rev, CMXsrv_ctl_chq_aprcbl, CMXsrv_icbr_rev_prot, CMXsrv_icbr_rev_ent, CMXsrv_ctl_eli_firma, CMXsrv_icbr_rev_trfo, CMXsrv_icbr_rev_vis, CMXsrv_cnt_rev_vig, CMXsrv_icbr_rev_acep, CMXsrv_icbr_rev_inst, CMXsrv_icbr_rev_trfb, CMXsrv_rctb_rem, CMXsrv_icbr_rev_ing, CMXsrv_icbr_rev_prorr, CMXsrv_icbr_rev_liq, sp_procxmode, CMXsrv_com_rev, CMXsrv_icbr_rev_pag, sp_cmx_sii_1870 |
| Form_Activate | CMXsrv_icbr_busc_eve | ECE | sp_procxmode |
| Form_Load | CMXsrv_icbr_lee_eve | ECE, ACMXDESEMB | sp_procxmode |
| Form_Load | CMXsrv_icbr_lee_ent_doc | CBR | sp_procxmode |
| aceptar_Click | CMXsrv_icbr_prot | LCB, CBR | sp_procxmode, CMXsrv_ctl_crea_apr, CMXsrv_cnt_950 |
| Form_Load | CMXsrv_icbr_pcg_prot | LCB, CBR | sp_procxmode |
| aceptar_Click | CMXsrv_icbr_liq_sdo | comex..CBR, LCB, CBR | CMXsrv_ctb_liq_sdo, sp_procxmode, CMXsrv_cnt_gen_vig |
| aceptar_Click | CMXsrv_icbr_act_vis | comex..CBR, CBR | sp_procxmode |
| eliminar_Click | CMXsrv_icbr_eli_rep | REP | sp_procxmode |
| Form_Activate | CMXsrv_icbr_busc_rep | REP | sp_procxmode |
| aceptar_Click | CMXsrv_icbr_imod_rep | REP, CBR | sp_procxmode |
| aceptar_Click | CMXsrv_icbr_ent_doc | comex..CBR, LCB, CBR | CMXsrv_ctl_crea_apr, sp_procxmode |
| Form_Load | CMXsrv_icbr_lee_ent_doc | CBR | sp_procxmode |
| aceptar_Click | CMXsrv_icbr_trf_ofi | comex..CBR, ACMXSUCSAL, CBR | CMXsrv_ctb_trfo, sp_procxmode |
| aceptar_Click | CMXsrv_val_suc | ACMXSUCSAL, tbl_User | sp_procxmode |
| aceptar_Click | CMXsrv_icbr_trf_bco | comex..CBR, ARC, CBR, LCB | CMXsrv_ctb_trfb, sp_procxmode |
| aceptar_Click | CMXsrv_icbr_act_inst | comex..CBR, CBR | sp_procxmode |
| enviar_Click | CMXsrv_iswf_a_pru | switxt, switxt1 | CMXsrv_iswf_a_732, CMXsrv_iswf_esp_707b, CMXsrv_iswf_a_747, CMXsrv_iswf_a_412, CMXsrv_iswf_a_707b, CMXsrv_iswf_esp_740, CMXsrv_iswf_a_410, CMXsrv_iswf_esp_747, CMXsrv_iswf_neg_730, CMXsrv_iswf_neg_752, CMXsrv_iswf_a_700a, CMXsrv_iswf_a_707a, CMXsrv_iswf_esp_700b, CMXsrv_iswf_a_740, CMXsrv_iswf_a_700b, CMXsrv_iswf_esp_707a, srv_irem_imp_202, CMXsrv_iswf_747_neg, srv_irem_imp_100, sp_procxmode, CMXsrv_iswf_esp_700a |
| Form_Load | CMXsrv_icbr_val_cbr | DDI, LCB, COR, ADI, ARC, ACMXMONEDAFEC, CBR, ACMXINTEREFEC, warnmsg | PrmACMXPAIS, CMXsrv_icbr_val_arc, CMXsrv_util_fecha, sp_procxmode, PrmACMXMONEDAFEC |
| word_Click | CMXsrv_icbr_val_cbr | DDI, LCB, COR, ADI, ARC, ACMXMONEDAFEC, CBR, ACMXINTEREFEC, warnmsg | PrmACMXPAIS, CMXsrv_icbr_val_arc, CMXsrv_util_fecha, sp_procxmode, PrmACMXMONEDAFEC |
| word_Click | CMXsrv_iswf_a_pru | switxt, switxt1 | CMXsrv_iswf_a_732, CMXsrv_iswf_esp_707b, CMXsrv_iswf_a_747, CMXsrv_iswf_a_412, CMXsrv_iswf_a_707b, CMXsrv_iswf_esp_740, CMXsrv_iswf_a_410, CMXsrv_iswf_esp_747, CMXsrv_iswf_neg_730, CMXsrv_iswf_neg_752, CMXsrv_iswf_a_700a, CMXsrv_iswf_a_707a, CMXsrv_iswf_esp_700b, CMXsrv_iswf_a_740, CMXsrv_iswf_a_700b, CMXsrv_iswf_esp_707a, srv_irem_imp_202, CMXsrv_iswf_747_neg, srv_irem_imp_100, sp_procxmode, CMXsrv_iswf_esp_700a |

---

## CRDEXT
<a name="crdext"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** | **Procedimientos Referenciados** |
|-------------|------------------------------|--------------------------|-------------------------------|
| Aceptar_Click | CMXsrv_icrd_a_ibab | MIBAB, IBAB | sp_procxmode |
| Form_Load | CMXsrv_icrd_lee_glo_ibab | IBAB, COL, MIBAB | sp_procxmode, CMXsrv_icrd_pre_78 |
| Aceptar_Click | CMXsrv_icrd_a_ibar | MIBAR, IBAR | sp_procxmode |
| Form_Load | CMXsrv_icrd_lee_glo_ibar | MIBAR, COL, IBAR | CMXsrv_icrd_pre_72_740, sp_procxmode |
| buscar_click | CMXsrv_icrd_lee_tex_swf | ACMXTSWFESPMSG, ACMXTSWFINGMSG | sp_procxmode |
| Aceptar_Click | CMXsrv_icrd_lee_cod_txt_swf | ACMXTSWFESPMSG, ACMXTSWFINGMSG | sp_procxmode |
| buscar_click | CMXsrv_icrd_lee_txt_swf_all | ACMXTSWFESPMSG, ACMXTSWFINGMSG | sp_procxmode |
| Form_Load | CMXsrv_icrd_lee_ind_esp_ing | MCTP, CRD | sp_procxmode |
| llena_arreglo | CMXsrv_icrd_lee_tex_swf | ACMXTSWFESPMSG, ACMXTSWFINGMSG | sp_procxmode |
| proximo_Click | CMXsrv_icrd_lee_txt_swf_all | ACMXTSWFESPMSG, ACMXTSWFINGMSG | sp_procxmode |
| aceptar_Click | CMXsrv_icrd_ing_acu | CRD | sp_procxmode |
| Form_Load | CMXsrv_icrd_lee_acu | CRD | sp_procxmode |
| aceptar_Click | CMXsrv_icrd_rech_sol | CRD, comex..COL, OPE_BCI, COL, comex..CRD | CMXsrv_nibx_upd_tran, CMXsrv_ctl_crea_apr, sp_procxmode, CMXsrv_nibx_nilive |
| aceptar_Click | CMXsrv_icrd_end | INF, ARC, COL, CRD | CMXsrv_ctl_crea_apr, sp_procxmode |
| Form_Load | CMXsrv_icrd_lee_dat_end | CRD | sp_procxmode |
| aceptar_Click | CMXsrv_icrd_asignar_cor | COR, ACMXMONEDAFEC, CRD, LCR | sp_procxmode |
| buscar_Click | CMXsrv_icrd_bus_lcr_bco | COR | sp_procxmode |
| proximo_Click | CMXsrv_icrd_bus_lcr_bco | COR | sp_procxmode |
| Form_Load | CMXsrv_grl_fec_serv |  | SRV_MessageService, sp_procxmode |

---

## CRD_CORR
<a name="crd_corr"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** | **Procedimientos Referenciados** |
|-------------|------------------------------|--------------------------|-------------------------------|
| aceptar_Click | CMXsrv_icrd_asignar_cor | COR, ACMXMONEDAFEC, CRD, LCR | sp_procxmode |
| buscar_Click | CMXsrv_icrd_bus_lcr_bco | COR | sp_procxmode |
| fld_cor_cod_mtr_LostFocus | CMXsrv_icrd_lee_bco_mtr | comex..ACMXBANCOS | sp_procxmode |
| fld_cor_cod_pais_Lostfocus | CMXsrv_icrd_cor_lee_pais | comex..ACMXPAIS | sp_procxmode |
| fld_cor_cod_plz_Lostfocus | CMXsrv_icrd_lee_plz | ACMXPLAZAS | sp_procxmode |
| proximo_Click | CMXsrv_icrd_bus_lcr_bco | COR | sp_procxmode |
| buscar_Click | CMXsrv_icrd_busc_plz | comex..ACMXPLAZAS | sp_procxmode |
| proximos_Click | CMXsrv_icrd_busc_plz | comex..ACMXPLAZAS | sp_procxmode |
| buscar_Click | CMXsrv_icrd_cor_busc_pais | comex, comex..ACMXPAIS | sp_procxmode |
| proximos_Click | CMXsrv_icrd_cor_busc_pais | comex, comex..ACMXPAIS | sp_procxmode |
| buscar_Click | CMXsrv_icrd_busc_bco_mtr | comex | sp_procxmode |
| proximos_Click | CMXsrv_icrd_busc_bco_mtr | comex | sp_procxmode |

---

## DDI
<a name="ddi"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** | **Procedimientos Referenciados** |
|-------------|------------------------------|--------------------------|-------------------------------|
| aceptar_Click | CMXsrv_iddi_ingmod_ddi | INF, DDI | sp_procxmode |
| continuar_Click | CMXsrv_iddi_lee_dec | DDI, ACMXVIATPT, ACMXRGMIMP, INF, ACMXBCOCEN, ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM, ACMXPAIS, CLN | sp_procxmode, CMXsrv_iddi_val_num_ddi |
| eliminar_Click | CMXsrv_iddi_eli_ddi | DDI | sp_procxmode |
| fld_ddi_fec_ii_lostfocus | CMXsrv_iddi_lee_inf | INF | sp_procxmode |
| fld_ddi_rut_imp_lostfocus | CMXsrv_iddi_lee_cln | CLN | sp_procxmode |
| Asociar_Click | CMXsrv_iddi_lee_rut | DDI | sp_procxmode |
| Asociar_Click | CMXsrv_iddi_asoc_ddi | DDI, ARC, ACMXMONEDAFEC, CBR, COB, INF, ACMXMONEDA, COL | CMXsrv_cmx_get_codes, CMXsrv_get_ult_dia_habil, CMXsrv_util_opr_fec, sp_procxmode |
| Command2_Click | CMXsrv_iddi_des_ddi | DDI, ADI, COB | sp_procxmode |
| Desasociar_Click | CMXsrv_iddi_lee_rut | DDI | sp_procxmode |
| Desasociar_Click | CMXsrv_iddi_des_ddi | DDI, ADI, COB | sp_procxmode |
| fld_aux_rut_cli_lostfocus | CMXsrv_iddi_lee_cln | CLN | sp_procxmode |
| inicio_asoc | CMXsrv_iddi_busc_asoc | ADI | sp_procxmode |
| inicio_noasoc | CMXsrv_iddi_busc_noasoc | DDI, ADI | CMXsrv_iddi_bus_noasoc_cob, CMXsrv_iddi_bus_noasoc_opr, sp_procxmode |
| proximo_no_aso_Click | CMXsrv_iddi_busc_noasoc | DDI, ADI | CMXsrv_iddi_bus_noasoc_cob, CMXsrv_iddi_bus_noasoc_opr, sp_procxmode |

---

## IMPORT
<a name="import"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** | **Procedimientos Referenciados** |
|-------------|------------------------------|--------------------------|-------------------------------|
| buscar_Click | CMXsrv_icrd_lee_dir_cln | DIRCLN | sp_procxmode |
| buscar_click | CMXsrv_icrd_lee_tex_swf | ACMXTSWFESPMSG, ACMXTSWFINGMSG | sp_procxmode |
| Aceptar_Click | CMXsrv_icrd_lee_cod_txt_swf | ACMXTSWFESPMSG, ACMXTSWFINGMSG | sp_procxmode |
| buscar_click | CMXsrv_icrd_lee_txt_swf_all | ACMXTSWFESPMSG, ACMXTSWFINGMSG | sp_procxmode |
| Form_Load | CMXsrv_icrd_lee_ind_esp_ing | MCTP, CRD | sp_procxmode |
| llena_arreglo | CMXsrv_icrd_lee_tex_swf | ACMXTSWFESPMSG, ACMXTSWFINGMSG | sp_procxmode |
| proximo_Click | CMXsrv_icrd_lee_txt_swf_all | ACMXTSWFESPMSG, ACMXTSWFINGMSG | sp_procxmode |
| Aceptar_Click | CMXCRDsrv_icrd_a_cnd_esp | CND | sp_procxmode |
| Form_Load | CMXsrv_icrd_lee_cnd_esp | MMCND, COL, CND | sp_procxmode, CMXsrv_icrd_pre_47 |
| clon_Click | CMXCRDsrv_icrd_clon_crd | CRS, MER, CRD, TAS, CRDCLON, COL_ADI, CND, DAC, ODOC, AVAL, COL, EMB | CMXCRDsrv_icrd_lee_tas_cln, sp_procxmode, CMXsrv_fincol_ing_modcol, CMXsrv_util_num_ope |
| Form_Activate | CMXCRDsrv_icrd_lee_crdcre | CRD_ADI, ACMXFORPAG, ACMXPAIS, ACMXVIATPT, CRD, COR, COL_ADI, ACMXFINVER, PMIX, NEG, ACMXMONEDA, tbl_User, OPE_BCI, ACMXSUCSAL, CLN, COL, DIRCLN, EMB | sp_procxmode |
| Form_Activate | CMXsrv_icrd_lee_ind_esp_ing | MCTP, CRD | sp_procxmode |
| Form_Activate | CMXsrv_icrd_lee_top | COL | sp_procxmode |
| Form_Load | CMXsrv_grl_fec_serv |  | SRV_MessageService, sp_procxmode |
| Form_Load | CMXsrv_cmx_get_codes |  | sp_procxmode |
| Form_Load | CMXsrv_trae_glo_fec | ACMXSUCSAL, ACMXDL3475FEC, tbl_User | sp_procxmode |
| Mcrdapr_Click | CMXCRDsrv_icrd_val_crd | warnmsg | sp_procxmode, CMXsrv_icrd_val_adv, CMXsrv_icrd_val_err |
| Mcrdeli_click | CMXCRDsrv_icrd_eli_crd | comex..COL, OPE_BCI, CRD | sp_procxmode |
| Mcrdtxtliq_Click | CMXsrv_icrd_lee_dat_trs | ASND, EVI, TRSD, EVE, ACMXMONEDA, COL | CMXsrv_icrd_forlin, sp_procxmode |
| Mcrdtxtope_Click | CMXsrv_icrd_dat_liq_ope | ACMXDESEMB, ASND, EVO, CRD, CNO, OBL, CUO, TRSD, NEG, COM, EVE, ACMXTIPEVE, CAN, COL | sp_procxmode |
| msg_swift | CMXsrv_iswf_a_pru | switxt, switxt1 | CMXsrv_iswf_a_732, CMXsrv_iswf_esp_707b, CMXsrv_iswf_a_747, CMXsrv_iswf_a_412, CMXsrv_iswf_a_707b, CMXsrv_iswf_esp_740, CMXsrv_iswf_a_410, CMXsrv_iswf_esp_747, CMXsrv_iswf_neg_730, CMXsrv_iswf_neg_752, CMXsrv_iswf_a_700a, CMXsrv_iswf_a_707a, CMXsrv_iswf_esp_700b, CMXsrv_iswf_a_740, CMXsrv_iswf_a_700b, CMXsrv_iswf_esp_707a, srv_irem_imp_202, CMXsrv_iswf_747_neg, srv_irem_imp_100, sp_procxmode, CMXsrv_iswf_esp_700a |
| Aceptar_Click | CMXsrv_icrd_a_ctp | CRD, CRDCLON, MCTP, comex..COL, COL | CMXCRDsrv_icrd_lee_tas_cln, CMXsrv_fincol_imod_colcc, sp_procxmode |
| FLD_COL_COD_CLI_LostFocus | CMXsrv_icrd_lee_cln | CLN, DIRCLN | sp_procxmode |
| Form_Load | CMXsrv_lee_fpro | ACMXFECPRO | sp_procxmode |
| Aceptar_Click | CMXsrv_icrd_a_cnd | TIP, CRD_ADI, CRD, CRDCLON, COL_ADI, COM, ACMXMONEDA, LIB, comex..COL, MAPR, MCND, COL, ACMXOPEIMP, comex..CRD | CMXMCRDsrv_icrd_lee_mapr, CMXsrv_ctb_impto_tim, CMXsrv_icrd_a_dat_apr, CMXsrv_imp_calc_aladi, CMXsrv_ctb_impto_tim2, CMXsrv_busc_cod_ope, sp_procxmode, CMXsrv_ctb_impto_tim3, CMXsrv_icrd_act_pag_mix, CMXsrv_util_pesos |
| Aceptar_Click | CMXCRDsrv_icrd_crea_crd | CRD_ADI, PMIX, ACMXMONEDA, CLN, COL | CMXsrv_imp_calc_aladi, CMXsrv_fincol_imod_colcc, sp_procxmode, CMXCRDsrv_icrd_lee_tas_cln, CMXsrv_util_num_ope, CMXsrv_fincol_ing_modcol |
| fld_col_fec_vto_LostFocus | CMXsrv_util_det_habil | ACMXFERIADO | sp_procxmode |
| Form_Activate | CMXsrv_icrd_busc_emb | comex..EMB, comex..MEMB | sp_procxmode |
| ELIMINAR_Click | CMXsrv_icrd_eli_emb | comex..COL, EMB, COL, CRD | sp_procxmode |
| Form_Load | CMXsrv_icrd_lee_emb1 | CRS, COL, EMB | sp_procxmode |
| Form_Load | CMXsrv_icrd_lee_emb2 | COL, EMB | sp_procxmode |
| ingresar_Click | CMXsrv_icrd_a_emb1 | CRS, MEMB, CRD, MCRS, CRDCLON, COL, EMB | sp_procxmode |
| ingresar_Click | CMXsrv_icrd_a_emb2 | EMB, COL, MEMB, CRD | sp_procxmode |
| VALIDA_EMBARQUE | CMXsrv_icrd_val_emb2 | warnmsg | sp_procxmode |
| VALIDA_EMBARQUE | CMXsrv_icrd_val_emb1 | INF, ARC, warnmsg | sp_procxmode |
| Aceptar_Click | CMXsrv_icrd_act_ref | MREF, CRD, CRDCLON, comex..MREF, comex..COL, COL | sp_procxmode |
| Form_Load | CMXsrv_icrd_act_ref | MREF, CRD, CRDCLON, comex..MREF, comex..COL, COL | sp_procxmode |
| Form_Load | CMXsrv_icrd_lee_ref | COR, COL, CRD | sp_procxmode |
| FLD_COL_COD_CLI_LostFocus | CMXsrv_icrd_lee_cln | CLN, DIRCLN | sp_procxmode |
| Aceptar_Click | CMXCRDsrv_icrd_apr_sol | TIP, CRD, COL_ADI, COM, LIB, OPE_BCI, sysobjects, CLN, COL | CMXsrv_mbyte_gen, CMXsrv_icrd_asignar_cor, CMXsrv_ctb_impto_tim, CMXsrv_cmx_ing_lib, CMXsrv_nibx_upd_tran, CMXsrv_ctb_impto_tim2, CMXsrv_lee_paridad, CMXsrv_iswf_a_700, CMXsrv_fincol_imod_colcc, sp_procxmode, CMXsrv_ctb_impto_tim22, CMXsrv_ctb_impto_tim3, CMXsrv_icrd_val_crd, CMXsrv_util_pesos, CMXsrv_nibx_nilive |
| Form_Load | CMXsrv_icrd_lee_crdapr | CRS, CRD, COL_ADI, DAC, ACMXAPROBAC | CMXsrv_icrd_pre_72, sp_procxmode |
| Aceptar_Click | CMXsrv_icrd_rech_sol | CRD, comex..COL, OPE_BCI, COL, comex..CRD | CMXsrv_nibx_upd_tran, CMXsrv_ctl_crea_apr, sp_procxmode, CMXsrv_nibx_nilive |
| Aceptar_Click | CMXCRDsrv_icrd_a_desc_merc | MER | sp_procxmode |
| Form_Load | CMXsrv_icrd_lee_desc_merc | MMER, MER | sp_procxmode |
| Aceptar_Click | CMXsrv_icrd_a_otr_doc | ODOC, MODOC | sp_procxmode |
| Form_Load | CMXsrv_icrd_lee_otr_doc | ODOC, MODOC | sp_procxmode, CMXsrv_icrd_pre_46 |
| enviar_Click | CMXsrv_iswf_a_pru | switxt, switxt1 | CMXsrv_iswf_a_732, CMXsrv_iswf_esp_707b, CMXsrv_iswf_a_747, CMXsrv_iswf_a_412, CMXsrv_iswf_a_707b, CMXsrv_iswf_esp_740, CMXsrv_iswf_a_410, CMXsrv_iswf_esp_747, CMXsrv_iswf_neg_730, CMXsrv_iswf_neg_752, CMXsrv_iswf_a_700a, CMXsrv_iswf_a_707a, CMXsrv_iswf_esp_700b, CMXsrv_iswf_a_740, CMXsrv_iswf_a_700b, CMXsrv_iswf_esp_707a, srv_irem_imp_202, CMXsrv_iswf_747_neg, srv_irem_imp_100, sp_procxmode, CMXsrv_iswf_esp_700a |

---

## INFORME
<a name="informe"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** | **Procedimientos Referenciados** |
|-------------|------------------------------|--------------------------|-------------------------------|
| Eliminar_Click | CMXsrv_iarc_eli_arc | ADI, CRD, ARC, NEG, COB, INF, COL | sp_procxmode |
| Form_Activate | CMXsrv_iarc_busc_arc | ARC | sp_procxmode |
| Form_Activate | CMXsrv_iinf_lee0_inf | INF | PrmACMXFPAIMP, PrmACMXMONEDA, PrmACLNEJECTA, sp_procxmode |
| Form_Activate | CMXsrv_iinf_lee_tablas | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM | sp_procxmode |
| Form_Activate | CMXsrv_iinf_lee1_inf | INF, CLN | PrmACMXCLACOM, PrmACMXESPECI, sp_procxmode, PrmACLNEJECTA, PrmACMXETDINF |
| Form_Activate | CMXsrv_iinf_lee_cln | CLN | PrmACLNEJECTA, sp_procxmode |
| Form_Activate | CMXsrv_iinf_lee2_inf | INF | PrmACMXPAIS, PrmACMXORIDVS, PrmACMXRGMIMP, sp_procxmode, PrmACMXBCOBCC, PrmACMXBCOCEN, PrmACMXSUCSAL |
| Form_Activate | CMXsrv_iinf_avi_miscb | INF | PrmACMXBCOBCC, sp_procxmode |
| Maviapr_Click | CMXsrv_iinf_avi_misca | INF, CLN | PrmACMXPAIS, PrmACMXORIDVS, PrmACMXRGMIMP, PrmACMXCLACOM, sp_procxmode, PrmACMXFPAIMP, PrmACLNEJECTA, PrmACMXSUCSAL, PrmACMXMONEDA, PrmACMXETDINF |
| Maviapr_Click | CMXsrv_iinf_avi_miscb | INF | PrmACMXBCOBCC, sp_procxmode |
| Mavicom_Click | CMXsrv_iinf_avi_misca | INF, CLN | PrmACMXPAIS, PrmACMXORIDVS, PrmACMXRGMIMP, PrmACMXCLACOM, sp_procxmode, PrmACMXFPAIMP, PrmACLNEJECTA, PrmACMXSUCSAL, PrmACMXMONEDA, PrmACMXETDINF |
| Mavicom_Click | CMXsrv_iinf_avi_miscb | INF | PrmACMXBCOBCC, sp_procxmode |
| Mavicom_Click | CMXsrv_icrd_lee_dat_com | TIP, ACMXDESEMB, ASND, CRD, EVI, COM, TRSD, EVE, ACMXMONEDA | PrmACMXMONEDA, sp_procxmode |
| Mavimis1_Click | CMXsrv_iinf_avi_misca | INF, CLN | PrmACMXPAIS, PrmACMXORIDVS, PrmACMXRGMIMP, PrmACMXCLACOM, sp_procxmode, PrmACMXFPAIMP, PrmACLNEJECTA, PrmACMXSUCSAL, PrmACMXMONEDA, PrmACMXETDINF |
| Mavimis1_Click | CMXsrv_iinf_avi_miscb | INF | PrmACMXBCOBCC, sp_procxmode |
| Mavimis2_Click | CMXsrv_iinf_avi_misca | INF, CLN | PrmACMXPAIS, PrmACMXORIDVS, PrmACMXRGMIMP, PrmACMXCLACOM, sp_procxmode, PrmACMXFPAIMP, PrmACLNEJECTA, PrmACMXSUCSAL, PrmACMXMONEDA, PrmACMXETDINF |
| Mavimis2_Click | CMXsrv_iinf_avi_miscb | INF | PrmACMXBCOBCC, sp_procxmode |
| Mavirec_Click | CMXsrv_iinf_avi_misca | INF, CLN | PrmACMXPAIS, PrmACMXORIDVS, PrmACMXRGMIMP, PrmACMXCLACOM, sp_procxmode, PrmACMXFPAIMP, PrmACLNEJECTA, PrmACMXSUCSAL, PrmACMXMONEDA, PrmACMXETDINF |
| Mavirec_Click | CMXsrv_iinf_avi_miscb | INF | PrmACMXBCOBCC, sp_procxmode |
| Mavitib_Click | CMXsrv_iinf_avi_misca | INF, CLN | PrmACMXPAIS, PrmACMXORIDVS, PrmACMXRGMIMP, PrmACMXCLACOM, sp_procxmode, PrmACMXFPAIMP, PrmACLNEJECTA, PrmACMXSUCSAL, PrmACMXMONEDA, PrmACMXETDINF |
| Mavitib_Click | CMXsrv_iinf_avi_miscb | INF | PrmACMXBCOBCC, sp_procxmode |
| Mavitras_Click | CMXsrv_iinf_avi_misca | INF, CLN | PrmACMXPAIS, PrmACMXORIDVS, PrmACMXRGMIMP, PrmACMXCLACOM, sp_procxmode, PrmACMXFPAIMP, PrmACLNEJECTA, PrmACMXSUCSAL, PrmACMXMONEDA, PrmACMXETDINF |
| Mavitras_Click | CMXsrv_iinf_avi_miscb | INF | PrmACMXBCOBCC, sp_procxmode |
| Mavitras_Click | CMXsrv_icrd_lee_dat_trs | ASND, EVI, TRSD, EVE, ACMXMONEDA, COL | CMXsrv_icrd_forlin, sp_procxmode |
| Minfoeli_click | CMXsrv_iinf_eli_inf | INF, ARC | sp_procxmode |
| Minforev_Click | CMXsrv_iinf_busc_evi | EVI | sp_procxmode |
| Minfoval_click | CMXsrv_iinf_val_inf | INF, ACMXPAIS, warnmsg | CMXsrv_cmx_get_codes, PrmACMXPAIS, PrmACMXCLACOM, sp_procxmode |
| Aceptar_Click | CMXsrv_iinf_ingmod_inf | INF, tbl_User, warnmsg | CMXsrv_util_fecha, sp_procxmode, PrmACMXMONEDAFEC, CMXsrv_cmx_get_codes, CMXsrv_iinf_val_inf, CMXsrv_iinf_get_num |
| Fec_pre | CMXsrv_iinf_lee_fec |  | CMXsrv_util_fecha, sp_procxmode |
| fld_aux_glo_cls_com_LostFocus | CMXsrv_iinf_lee_tablas | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM | sp_procxmode |
| fld_aux_glo_for_pag1_LostFocus | CMXsrv_iinf_lee_tablas | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM | sp_procxmode |
| fld_aux_glo_for_pag2_LostFocus | CMXsrv_iinf_lee_tablas | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM | sp_procxmode |
| fld_aux_glo_for_pag3_LostFocus | CMXsrv_iinf_lee_tablas | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM | sp_procxmode |
| fld_aux_glo_mon_LostFocus | CMXsrv_iinf_lee_tablas | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM | sp_procxmode |
| fld_inf_cls_com_Lostfocus | CMXsrv_iinf_lee_tablas | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM | sp_procxmode |
| fld_inf_cod_imp_LostFocus | CMXsrv_iinf_lee_cln | CLN | PrmACLNEJECTA, sp_procxmode |
| fld_inf_for_pag1_lostfocus | CMXsrv_iinf_lee_tablas | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM | sp_procxmode |
| fld_inf_for_pag2_LostFocus | CMXsrv_iinf_lee_tablas | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM | sp_procxmode |
| fld_inf_for_pag3_LostFocus | CMXsrv_iinf_lee_tablas | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM | sp_procxmode |
| fld_inf_mon_inf_lostfocus | CMXsrv_iinf_lee_tablas | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM | sp_procxmode |
| Form_Load | CMXsrv_iinf_lee0_inf | INF | PrmACMXFPAIMP, PrmACMXMONEDA, PrmACLNEJECTA, sp_procxmode |
| Form_Load | CMXsrv_iinf_lee1_inf | INF, CLN | PrmACMXCLACOM, PrmACMXESPECI, sp_procxmode, PrmACLNEJECTA, PrmACMXETDINF |
| Form_Load | CMXsrv_iinf_lee2_inf | INF | PrmACMXPAIS, PrmACMXORIDVS, PrmACMXRGMIMP, sp_procxmode, PrmACMXBCOBCC, PrmACMXBCOCEN, PrmACMXSUCSAL |
| valor_usd | CMXsrv_iinf_lee_usd |  | CMXsrv_cmx_get_codes, PrmACMXMONEDAFEC, sp_procxmode |
| Aceptar_Click | CMXsrv_iinf_busc_inf | INF | sp_procxmode |
| buscar_Click | CMXsrv_iinf_busc_inf | INF | sp_procxmode |
| Fec_pre | CMXsrv_iinf_lee_fec |  | CMXsrv_util_fecha, sp_procxmode |
| fld_inf_cod_imp_LostFocus | CMXsrv_iinf_lee_cln | CLN | PrmACLNEJECTA, sp_procxmode |
| PROXIMA_Click | CMXsrv_iinf_busc_inf | INF | sp_procxmode |
| Aceptar_Click | CMXsrv_iinf_act_apr | INF | CMXsrv_iinf_val_inf, CMXsrv_util_fecha, sp_procxmode |
| Form_Activate | CMXsrv_iinf_busc_evi | EVI | sp_procxmode |
| reversar_Click | CMXsrv_iinf_rev_evi | INF, ARC, INC, EVI | CMXsrv_com_rev, sp_procxmode |
| Form_Load | CMXsrv_iinf_lee_evi | EVI | PrmACMXSUCSAL, PrmACMXBCOCEN, sp_procxmode, PrmACMXETDINF |
| Aceptar_Click | CMXsrv_iinf_act_tib | INF | CMXsrv_cmx_get_codes, sp_procxmode |
| Aceptar_Click | CMXsrv_iinf_act_rec | INF | CMXsrv_util_fecha, sp_procxmode |
| Aceptar_Click | CMXsrv_iinf_act_rib | INF | CMXsrv_cmx_get_codes, sp_procxmode |
| Form_Activate | CMXsrv_iinf_busc_comp | INF | sp_procxmode |
| proximos_Click | CMXsrv_iinf_busc_comp | INF | sp_procxmode |
| Aceptar_Click | CMXsrv_iinf_ingmod_comp | INF, warnmsg | CMXsrv_util_fecha, sp_procxmode, PrmACMXMONEDAFEC, CMXsrv_cmx_get_codes, CMXsrv_iinf_val_inf, CMXsrv_iinf_get_num |
| Fec_pre | CMXsrv_iinf_lee_fec |  | CMXsrv_util_fecha, sp_procxmode |
| Form_Activate | CMXsrv_iinf_lee_comp | INF | PrmACMXPAIS, PrmACMXORIDVS, PrmACMXRGMIMP, PrmACMXCLACOM, sp_procxmode, PrmACMXFPAIMP, PrmACMXVIATPT, PrmACMXMONEDA |
| Form_Activate | CMXsrv_iinf_lee_tablas | ACMXFPAIMP, ACMXMONEDA, ACMXCLACOM | sp_procxmode |
| aceptar_click | CMXsrv_iinf_lee_bco | COR | PrmACMXPAIS, sp_procxmode |
| buscar_Click | CMXsrv_iinf_busc_bco | ACMXBCOBCC | sp_procxmode |
| Form_Load | CMXsrv_grl_fec_serv |  | SRV_MessageService, sp_procxmode |

---

## MOD_ADI
<a name="mod_adi"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** | **Procedimientos Referenciados** |
|-------------|------------------------------|--------------------------|-------------------------------|
| Aceptar_Click | CMXsrv_icrd_a_cnd | TIP, CRD_ADI, CRD, CRDCLON, COL_ADI, COM, ACMXMONEDA, LIB, comex..COL, MAPR, MCND, COL, ACMXOPEIMP, comex..CRD | CMXMCRDsrv_icrd_lee_mapr, CMXsrv_ctb_impto_tim, CMXsrv_icrd_a_dat_apr, CMXsrv_imp_calc_aladi, CMXsrv_ctb_impto_tim2, CMXsrv_busc_cod_ope, sp_procxmode, CMXsrv_ctb_impto_tim3, CMXsrv_icrd_act_pag_mix, CMXsrv_util_pesos |
| busca_bco | CMXsrv_icrd_lee_bco_swf | ACMXPAIS, COR | CMXsrv_icrd_lee_cln, sp_procxmode |
| fld_col_fec_vto_LostFocus | CMXsrv_util_det_habil | ACMXFERIADO | sp_procxmode |
| Form_Load | CMXMCRDsrv_icrd_lee_mcnd | CRD_ADI, ACMXFORPAG, CRD, PMIX, ACMXMONEDA, MPMIX, MCND | sp_procxmode |
| Form_Load | CMXsrv_grl_fec_serv |  | SRV_MessageService, sp_procxmode |

---

## MOD_CBR
<a name="mod_cbr"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** | **Procedimientos Referenciados** |
|-------------|------------------------------|--------------------------|-------------------------------|
| fld_cbr_cod_gdo_LostFocus | CMXsrv_icbr_lee_cln | CLN | sp_procxmode |
| Form_Load | CMXsrv_icbr_lee_ctp | ACMXSUCSAL, MCBRCTP, CBR, ACMXPAIS, CLN, CBRANX | sp_procxmode |
| INGRESAR_Click | CMXsrv_icbr_act_ctp | comex..CBR, MCBRCTP, CBRANX, CBR | sp_procxmode |
| Form_Load | CMXsrv_icbr_lee_trm | ACMXVIATPT, CBR, ACMXINTERE, ACMXMONEDA, MCBRTER, ACMXCLACOM, ACMXPAIS | sp_procxmode |
| INGRESAR_Click | CMXsrv_icbr_act_trm | LCB, COM, CBR, MCBRTER, warnmsg, CLN | CMXsrv_util_fecha, CMXsrv_icbr_val_cbr, sp_procxmode |
| Form_Load | CMXsrv_icbr_lee_doc | LCB, MCBRDOC, MLCB, CBR, ACMXMONEDA | sp_procxmode |
| INGRESAR_Click | CMXsrv_icbr_act_doc | LCB, MCBRDOC, MLCB, CBR, comex..CBR | sp_procxmode |
| Form_Activate | CMXsrv_icbr_busc_let | MLCB, comex..MLCB, comex..LCB | sp_procxmode |
| aceptar_Click | CMXsrv_icbr_mod_ing_let | LCB, MLCB, CBR, end | CMXsrv_util_opr_fec, sp_procxmode |
| eliminar_Click | CMXsrv_icbr_eli_let | LCB, MCBRDOC, MLCB, CBR, comex..COL | sp_procxmode |
| Form_Activate | CMXsrv_icbr_lee_let | ACMXNOTARIO, LCB, MLCB | sp_procxmode |
| actualizar_Click | CMXsrv_icbr_acep_mod_cbr | LCB, MCBRDOC, MCBRCTP, MLCB, CBR, MCBRTER, warnmsg | CMXsrv_cnt_2800, CMXsrv_icbr_cheq_mdoc, CMXsrv_icbr_val_cbr, CMXsrv_icbr_cheq_mctp, CMXsrv_icbr_cheq_mter, sp_procxmode, CMXsrv_icbr_cheq_mlcb |
| Cancelar_Click | CMXsrv_icbr_eli_no_cont | MCBRDOC, MCBRCTP, MLCB, CBR, MCBRTER | sp_procxmode |

---

## MOD_CRD
<a name="mod_crd"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** | **Procedimientos Referenciados** |
|-------------|------------------------------|--------------------------|-------------------------------|
| Aceptar_Click | CMXsrv_icrd_a_ibab | MIBAB, IBAB | sp_procxmode |
| Form_Load | CMXsrv_icrd_lee_glo_ibab | IBAB, COL, MIBAB | sp_procxmode, CMXsrv_icrd_pre_78 |
| Aceptar_Click | CMXsrv_icrd_a_ibar | MIBAR, IBAR | sp_procxmode |
| Form_Load | CMXsrv_icrd_lee_glo_ibar | MIBAR, COL, IBAR | CMXsrv_icrd_pre_72_740, sp_procxmode |
| buscar_click | CMXsrv_icrd_lee_dir_cln | DIRCLN | sp_procxmode |
| buscar_Click | CMXsrv_icrd_lee_tex_swf | ACMXTSWFESPMSG, ACMXTSWFINGMSG | sp_procxmode |
| buscar_click | CMXsrv_icrd_lee_tex_swf | ACMXTSWFESPMSG, ACMXTSWFINGMSG | sp_procxmode |
| Aceptar_Click | CMXsrv_icrd_lee_cod_txt_swf | ACMXTSWFESPMSG, ACMXTSWFINGMSG | sp_procxmode |
| buscar_click | CMXsrv_icrd_lee_txt_swf_all | ACMXTSWFESPMSG, ACMXTSWFINGMSG | sp_procxmode |
| Form_Load | CMXsrv_icrd_lee_ind_esp_ing | MCTP, CRD | sp_procxmode |
| llena_arreglo | CMXsrv_icrd_lee_tex_swf | ACMXTSWFESPMSG, ACMXTSWFINGMSG | sp_procxmode |
| proximo_Click | CMXsrv_icrd_lee_txt_swf_all | ACMXTSWFESPMSG, ACMXTSWFINGMSG | sp_procxmode |
| Aceptar_Click | CMXMCRDsrv_icrd_a_mmcnd | MMCND | sp_procxmode |
| Form_Load | CMXsrv_icrd_lee_cnd_esp | MMCND, COL, CND | sp_procxmode, CMXsrv_icrd_pre_47 |
| Aceptar_Click | CMXsrv_icrd_a_ctp | CRD, CRDCLON, MCTP, comex..COL, COL | CMXCRDsrv_icrd_lee_tas_cln, CMXsrv_fincol_imod_colcc, sp_procxmode |
| FLD_COL_COD_CLI_LostFocus | CMXsrv_icrd_lee_cln | CLN, DIRCLN | sp_procxmode |
| Form_Load | CMXMCRDsrv_icrd_lee_mctp | ACMXPAIS, MCTP, DIRCLN, CRD | sp_procxmode |
| Aceptar_Click | CMXsrv_icrd_a_cnd | TIP, CRD_ADI, CRD, CRDCLON, COL_ADI, COM, ACMXMONEDA, LIB, comex..COL, MAPR, MCND, COL, ACMXOPEIMP, comex..CRD | CMXMCRDsrv_icrd_lee_mapr, CMXsrv_ctb_impto_tim, CMXsrv_icrd_a_dat_apr, CMXsrv_imp_calc_aladi, CMXsrv_ctb_impto_tim2, CMXsrv_busc_cod_ope, sp_procxmode, CMXsrv_ctb_impto_tim3, CMXsrv_icrd_act_pag_mix, CMXsrv_util_pesos |
| Form_Load | CMXMCRDsrv_icrd_lee_mcnd | CRD_ADI, ACMXFORPAG, CRD, PMIX, ACMXMONEDA, MPMIX, MCND | sp_procxmode |
| Form_Activate | CMXsrv_icrd_busc_emb | comex..EMB, comex..MEMB | sp_procxmode |
| cancelar_Click | CMXsrv_icrd_lee_desc_merc | MMER, MER | sp_procxmode |
| ELIMINAR_Click | CMXsrv_icrd_eli_emb | comex..COL, EMB, COL, CRD | sp_procxmode |
| Form_Load | CMXMCRDsrv_icrd_lee_memb2 | MEMB, EMB | sp_procxmode |
| Form_Load | CMXMCRDsrv_icrd_lee_memb1 | CRS, MEMB, EMB, MCRS | sp_procxmode |
| ingresar_Click | CMXsrv_icrd_a_emb1 | CRS, MEMB, CRD, MCRS, CRDCLON, COL, EMB | sp_procxmode |
| ingresar_Click | CMXsrv_icrd_a_emb2 | EMB, COL, MEMB, CRD | sp_procxmode |
| VALIDA_EMBARQUE | CMXsrv_icrd_val_emb2 | warnmsg | sp_procxmode |
| VALIDA_EMBARQUE | CMXsrv_icrd_val_emb1 | INF, ARC, warnmsg | sp_procxmode |
| Aceptar_Click | CMXsrv_icrd_act_ref | MREF, CRD, CRDCLON, comex..MREF, comex..COL, COL | sp_procxmode |
| fld_obl_cod_bco_acre_DblClick | CMXsrv_icrd_lee_bco_swf | ACMXPAIS, COR | CMXsrv_icrd_lee_cln, sp_procxmode |
| fld_obl_cod_bco_acre_LostFocus | CMXsrv_icrd_lee_bco_swf | ACMXPAIS, COR | CMXsrv_icrd_lee_cln, sp_procxmode |
| Form_Load | CMXMCRDsrv_icrd_lee_mref | MREF, COR, COL, CRD | sp_procxmode |
| Aceptar_Click | CMXsrv_icrd_ing_txt | MTXT | sp_procxmode |
| Form_Load | CMXCRDsrv_icrd_get_ing_esp | ACMXPAIS, MCTP, CRD | sp_procxmode |
| Form_Load | CMXMCRDsrv_icrd_lee_mtxt | MTXT | sp_procxmode |
| Form_Load | CMXCRDsrv_icrd_get_pre_fra | ACMXTSWFESPMSG, ACMXTSWFINGMSG | sp_procxmode |
| Aceptar_Click | CMXMCRDsrv_icrd_a_mmer | MMER | sp_procxmode |
| Form_Load | CMXsrv_icrd_lee_desc_merc | MMER, MER | sp_procxmode |
| Aceptar_Click | CMXsrv_icrd_a_otr_doc | ODOC, MODOC | sp_procxmode |
| Form_Load | CMXsrv_icrd_lee_otr_doc | ODOC, MODOC | sp_procxmode, CMXsrv_icrd_pre_46 |
| Aceptar_Click | CMXsrv_fincol_lee_cod_eve | MCND, COL, CRD, COM | sp_procxmode |
| Aceptar_Click | CMXMCRDsrv_icrd_acep_mod_crd | de, TIP, CRD, COD, MCRS, OBL, EVE, LIB, warnmsg, OPE_BCI, sysobjects, COL | CMXsrv_icrd_cheq_modoc, CMXCRDsrv_icrd_val_crd, CMXsrv_icrd_cheq_memb, CMXsrv_nibx_upd_tran, CMXsrv_expcce_anl_cce, CMXsrv_fincol_ctb_mod, CMXsrv_icrd_cheq_mtxt, CMXsrv_icrd_cheq_mcnd, CMXsrv_icrd_cheq_mmer, CMXsrv_icrd_cheq_mref, CMXsrv_nibx_nilive, CMXsrv_icrd_cheq_mpmix, CMXsrv_ctl_crea_apr, CMXsrv_icrd_cheq_mibar, CMXMCRDsrv_icrd_eli_no_cont, CMXsrv_icrd_lee_tip_ope, CMXsrv_icrd_cheq_mmcnd, CMXsrv_icrd_cheq_mibab, sp_procxmode, CMXsrv_icrd_cheq_mctp, CMXsrv_icrd_cheq_mapr, CMXsrv_cnt_950 |
| cancelar_Click | CMXMCRDsrv_icrd_eli_no_cont | MREF, MEMB, MCRS, MMCND, COM, MODOC, MIBAB, CRD_AMD, MPMIX, MCTP, MMER, MCND, MIBAR, TNIH, MAPR, FE_IN_REJECTED_TRANS, MTXT | sp_procxmode |
| fld_crd_cod_bco_rem_LostFocus | CMXsrv_icrd_lee_bco_swf | ACMXPAIS, COR | CMXsrv_icrd_lee_cln, sp_procxmode |
| fld_crd_fec_mod_lostFocus | CMXsrv_fincol_efec_calpa | TF_PPAG, TIP, TAS, CUO, comex..ACMXMONEDA, COL_ADI, OBL, CTR, NEG_ADI, ACMXINTERE, CAN, ICR, COL | CMXsrv_fincol_eval_tnem, CMXsrv_fincol_eval_tmor, CMXsrv_util_det_habil, sp_procxmode, CMXsrv_fincol_calc_reba, CMXsrv_fincol_eval_tasa, CMXsrv_fincol_eval_tneg, CMXsrv_fincol_efcal_cv, CMXsrv_fincol_cal_tas_sfr |
| Form_Activate | CMXsrv_icrd_lee_ind_esp_ing | MCTP, CRD | sp_procxmode |
| Form_Load | CMXsrv_fincol_efec_calpa | TF_PPAG, TIP, TAS, CUO, comex..ACMXMONEDA, COL_ADI, OBL, CTR, NEG_ADI, ACMXINTERE, CAN, ICR, COL | CMXsrv_fincol_eval_tnem, CMXsrv_fincol_eval_tmor, CMXsrv_util_det_habil, sp_procxmode, CMXsrv_fincol_calc_reba, CMXsrv_fincol_eval_tasa, CMXsrv_fincol_eval_tneg, CMXsrv_fincol_efcal_cv, CMXsrv_fincol_cal_tas_sfr |
| Form_Load | CMXMCRDsrv_icrd_lee_mcnd | CRD_ADI, ACMXFORPAG, CRD, PMIX, ACMXMONEDA, MPMIX, MCND | sp_procxmode |
| Form_Load | CMXsrv_grl_fec_serv |  | SRV_MessageService, sp_procxmode |

---

## NEGO_AV
<a name="nego_av"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** | **Procedimientos Referenciados** |
|-------------|------------------------------|--------------------------|-------------------------------|
| aviso1 | CMXsrv_icrd_a_rec_age | COR, TAS, CRD, CUO, CNEG, COM, NEG, TRSD, DIS, EVE, ACMXMONEDA, ACMXINTERE, ACMXSUCSAL, COL | CMXsrv_util_fecha, sp_procxmode |
| aviso1 | CMXsrv_busc_ofi_cta | CLN | PrmACMXESPECI, PrmACLNEJECTA, sp_procxmode |
| aviso1 | CMXsrv_neg_busc_arc | ARC | sp_procxmode |
| aviso1 | CMXsrv_icrd_lee_avi_adi | CRD | sp_procxmode |
| aviso3 | CMXsrv_icrd_lee_dat_trs | ASND, EVI, TRSD, EVE, ACMXMONEDA, COL | CMXsrv_icrd_forlin, sp_procxmode |
| Aviso4 | CMXsrv_icrd_dat_liq_ope | ACMXDESEMB, ASND, EVO, CRD, CNO, OBL, CUO, TRSD, NEG, COM, EVE, ACMXTIPEVE, CAN, COL | sp_procxmode |
| Aviso4 | CMXsrv_icrd_lee_dat_cln | NEG, CLN, COL | CMXsrv_trae_glo_fec, sp_procxmode |
| Aviso5 | CMXsrv_icrd_lee_dat_cln | NEG, CLN, COL | CMXsrv_trae_glo_fec, sp_procxmode |
| Aviso5 | CMXsrv_icrd_lee_avi_dis | DIS, COL | sp_procxmode |
| Aviso5 | CMXsrv_icrd_lee_avi_adi | CRD | sp_procxmode |
| Aviso5 | CMXsrv_neg_ddi_asoc | ADI | sp_procxmode |
| Aviso5 | CMXsrv_neg_busc_arc | ARC | sp_procxmode |
| Aviso5 | CMXsrv_neg_trae_vcto_mcf | COL, CUO | sp_procxmode |
| lee_aval | CMXsrv_neg_avi_lee_aval | TAS, CNEG, AVAL, CLN, COL | sp_procxmode |
| lee_nego | CMXsrv_icrd_neg_lee_crd | NEG, COL | sp_procxmode |
| lee_nego | CMXsrv_icrd_lee_neg | TAS, CRD, ACMXFINVER, NEG, NEG_ADI, DIS, COL | sp_procxmode |
| avi_col1 | CMXsrv_col_avi_dat_cln | TIP, CRD, DAC, ACMXESPECI, ACMXSUCSAL, CLN, COL, ACLNEJECTA | sp_procxmode |
| avi_col1 | CMXsrv_col_avi_det_pag | CCX, TIP, TAS, CRD, COB, ACMXINTERE, EVE, ACMXMONEDA, ACMXINTEREFEC, CAN, CAN_REN, COL | CMX_srv_pone_punto, CMXsrv_util_fecha, sp_procxmode |
| avi_col2 | CMXsrv_col_avi_dat_cln | TIP, CRD, DAC, ACMXESPECI, ACMXSUCSAL, CLN, COL, ACLNEJECTA | sp_procxmode |
| avi_col2 | CMXsrv_col_avi_det_oto | TIP, ACMXDESEMB, ASND, TAS, CUO, COD, NEG, ACMXINTERE, EVE, ACMXMONEDA, ACMXINTEREFEC, AVAL, CLN, COL | CMX_srv_pone_punto, CMXsrv_trae_glo_fec, sp_procxmode |
| avi_col4 | CMXsrv_col_avi_dat_cln | TIP, CRD, DAC, ACMXESPECI, ACMXSUCSAL, CLN, COL, ACLNEJECTA | sp_procxmode |
| avi_col4 | CMXsrv_col_lee_num_trs | EVE, COL, TIP, COD | CMXsrv_avigrl_lee_avitemp, sp_procxmode |
| lee_obl_pag | CMXsrv_finobl_avi_pag | CNO, EVO | CMX_srv_pone_punto, sp_procxmode |
| traspaso | CMXsrv_neg_avi_trae_asnd_mn | ACMXDESEMB, ASND, COD, TRSD, ACMXMONEDA | CMX_srv_pone_punto, sp_procxmode |
| traspaso | CMXsrv_neg_avi_trae_asnd_mx | ACMXDESEMB, ACMXMONEDA, ASND | CMX_srv_pone_punto, sp_procxmode |
| Form_Activate | CMXsrv_icrd_neg_lee_crd | NEG, COL | sp_procxmode |
| Form_Activate | CMXsrv_icrd_lee_neg | TAS, CRD, ACMXFINVER, NEG, NEG_ADI, DIS, COL | sp_procxmode |
| Mcrdtxtliq_Click | CMXsrv_icrd_lee_dat_trs | ASND, EVI, TRSD, EVE, ACMXMONEDA, COL | CMXsrv_icrd_forlin, sp_procxmode |
| Mcrdtxtope_Click | CMXsrv_icrd_dat_liq_ope | ACMXDESEMB, ASND, EVO, CRD, CNO, OBL, CUO, TRSD, NEG, COM, EVE, ACMXTIPEVE, CAN, COL | sp_procxmode |
| MNEGCONT_Click | CMXsrv_icrd_cont_neg | COL, NEG, CRD, COD | CMXsrv_icrd_val_neg, CMXsrv_mbyte_gen, sp_procxmode, sp_cmx_sii_1870, CMXsrv_fincol_ictb_neg_aux |
| MNEGELI_CLICK | CMXsrv_icrd_eli_neg | CRD, COM, NEG, CND, NEG_ADI, ACMXTXTSWF, comex..COL | CMXsrv_swf_graba_det, sp_procxmode |
| precarga_datos | CMXsrv_icrd_a_rec_age | COR, TAS, CRD, CUO, CNEG, COM, NEG, TRSD, DIS, EVE, ACMXMONEDA, ACMXINTERE, ACMXSUCSAL, COL | CMXsrv_util_fecha, sp_procxmode |
| precarga_datos | CMXsrv_busc_ofi_cta | CLN | PrmACMXESPECI, PrmACLNEJECTA, sp_procxmode |
| Form_Load | CMXsrv_trae_glo_fec | ACMXSUCSAL, ACMXDL3475FEC, tbl_User | sp_procxmode |
| Form_Load | CMXsrv_icrd_lee_num_col | COL | sp_procxmode |
| Form_Load | CMXsrv_icrd_bus_pago | CAN | sp_procxmode |

---

## NNEGO
<a name="nnego"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** | **Procedimientos Referenciados** |
|-------------|------------------------------|--------------------------|-------------------------------|
| Form_Activate | CMXsrv_icrd_neg_lee_crd | NEG, COL | sp_procxmode |
| Form_Activate | CMXsrv_icrd_lee_neg | TAS, CRD, ACMXFINVER, NEG, NEG_ADI, DIS, COL | sp_procxmode |
| gen_mens_swift | CMXsrv_iswf_a_pru | switxt, switxt1 | CMXsrv_iswf_a_732, CMXsrv_iswf_esp_707b, CMXsrv_iswf_a_747, CMXsrv_iswf_a_412, CMXsrv_iswf_a_707b, CMXsrv_iswf_esp_740, CMXsrv_iswf_a_410, CMXsrv_iswf_esp_747, CMXsrv_iswf_neg_730, CMXsrv_iswf_neg_752, CMXsrv_iswf_a_700a, CMXsrv_iswf_a_707a, CMXsrv_iswf_esp_700b, CMXsrv_iswf_a_740, CMXsrv_iswf_a_700b, CMXsrv_iswf_esp_707a, srv_irem_imp_202, CMXsrv_iswf_747_neg, srv_irem_imp_100, sp_procxmode, CMXsrv_iswf_esp_700a |
| llama_pagos | CMXsrv_icrd_lee_col | CCL, COL, TAS | sp_procxmode |
| Mnegavi9_Click | CMXsrv_iswf_a_pru | switxt, switxt1 | CMXsrv_iswf_a_732, CMXsrv_iswf_esp_707b, CMXsrv_iswf_a_747, CMXsrv_iswf_a_412, CMXsrv_iswf_a_707b, CMXsrv_iswf_esp_740, CMXsrv_iswf_a_410, CMXsrv_iswf_esp_747, CMXsrv_iswf_neg_730, CMXsrv_iswf_neg_752, CMXsrv_iswf_a_700a, CMXsrv_iswf_a_707a, CMXsrv_iswf_esp_700b, CMXsrv_iswf_a_740, CMXsrv_iswf_a_700b, CMXsrv_iswf_esp_707a, srv_irem_imp_202, CMXsrv_iswf_747_neg, srv_irem_imp_100, sp_procxmode, CMXsrv_iswf_esp_700a |
| MNEGCONT_Click | CMXsrv_icrd_cont_neg | COL, NEG, CRD, COD | CMXsrv_icrd_val_neg, CMXsrv_mbyte_gen, sp_procxmode, sp_cmx_sii_1870, CMXsrv_fincol_ictb_neg_aux |
| MNEGELI_CLICK | CMXsrv_icrd_eli_neg | CRD, COM, NEG, CND, NEG_ADI, ACMXTXTSWF, comex..COL | CMXsrv_swf_graba_det, sp_procxmode |
| pertas_Click | CMXsrv_icrd_lee_col | CCL, COL, TAS | sp_procxmode |
| Form_Activate | CMXsrv_icrd_busc_neg | NEG | sp_procxmode |
| Form_Load | CMXsrv_icrd_busc_emb | comex..EMB, comex..MEMB | sp_procxmode |
| ACEPTAR_Click | CMXsrv_icrd_a_neg_emb1 | TAS, CNEG, NEG, COL, DOCNEG | sp_procxmode |
| ACEPTAR_Click | CMXsrv_icrd_a_neg_emb2 | NEG, COL, comex..COL, DOCNEG | sp_procxmode, CMXsrv_icrd_chq_doc_neg |
| CANCELAR_Click | CMXsrv_icrd_eli_doc_neg | COL, DOCNEG | sp_procxmode |
| Form_Activate | CMXsrv_icrd_lee_emb1 | CRS, COL, EMB | sp_procxmode |
| Form_Activate | CMXsrv_icrd_lee_emb2 | COL, EMB | sp_procxmode |
| Form_Activate | CMXsrv_icrd_lee_neg_emb1 | COL, NEG | sp_procxmode |
| Form_Activate | CMXsrv_icrd_lee_neg_emb2 | COL, NEG | sp_procxmode |
| Form_Activate | CMXsrv_icrd_lee_cnd_esp | MMCND, COL, CND | sp_procxmode, CMXsrv_icrd_pre_47 |
| Form_Activate | CMXsrv_icrd_lee_desc_merc | MMER, MER | sp_procxmode |
| ACEPTAR_Click | CMXsrv_icrd_a_neg_disc | COL, DIS, NEG | sp_procxmode |
| Form_Load | CMXsrv_icrd_neg_lee_disc | DIS, NEG | sp_procxmode, CMXsrv_icrd_gen_disc |
| ACEPTAR_Click | CMXsrv_icrd_ent_doc | COL, NEG, comex..COL | CMXsrv_mbyte_gen, CMXsrv_swf_graba_det, sp_procxmode |
| ELIMINAR_Click | CMXsrv_icrd_ent_doc | COL, NEG, comex..COL | CMXsrv_mbyte_gen, CMXsrv_swf_graba_det, sp_procxmode |
| Form_Load | CMXsrv_icrd_ent_doc | COL, NEG, comex..COL | CMXsrv_mbyte_gen, CMXsrv_swf_graba_det, sp_procxmode |
| ACEPTAR_Click | CMXsrv_icrd_alz_disc | comex..ACMXINTEREFEC, COR, TAS, CRD, CUO, COD, CNEG, NEG, ACMXMONEDAFEC, NEG_ADI, ACMXINTERE, ACMXBCOUSU, ACMXINTEREFEC, sysobjects, COL | CMXsrv_get_ult_dia_habil, CMXsrv_icrd_cont_alz, CMXsrv_ipuc_gen_pln, sp_procxmode, CMXsrv_cnt_950, CMXsrv_cmx_get_codes, CMXsrv_fincol_cal_tas_sfr |
| aceptar_click | CMXCRDsrv_icrd_asignar_cor | COR, ACMXMONEDAFEC, CRD, LCR | sp_procxmode |
| BUSCAR_Click | CMXCRDsrv_icrd_bus_lcr_bco | COR | sp_procxmode |
| proximo_Click | CMXCRDsrv_icrd_bus_lcr_bco | COR | sp_procxmode |
| ACEPTAR_Click | CMXsrv_icrd_act_doc_neg | NEG, COL, DOCNEG | sp_procxmode |
| Form_Load | CMXsrv_icrd_lee_doc_neg | NEG, EMB | sp_procxmode |
| enviar_Click | CMXsrv_iswf_a_pru | switxt, switxt1 | CMXsrv_iswf_a_732, CMXsrv_iswf_esp_707b, CMXsrv_iswf_a_747, CMXsrv_iswf_a_412, CMXsrv_iswf_a_707b, CMXsrv_iswf_esp_740, CMXsrv_iswf_a_410, CMXsrv_iswf_esp_747, CMXsrv_iswf_neg_730, CMXsrv_iswf_neg_752, CMXsrv_iswf_a_700a, CMXsrv_iswf_a_707a, CMXsrv_iswf_esp_700b, CMXsrv_iswf_a_740, CMXsrv_iswf_a_700b, CMXsrv_iswf_esp_707a, srv_irem_imp_202, CMXsrv_iswf_747_neg, srv_irem_imp_100, sp_procxmode, CMXsrv_iswf_esp_700a |
| Form_Load | CMXsrv_icrd_val_neg | DDI, COR, ADI, TAS, CUO, NEG, ACMXMONEDAFEC, DAC, ACMXINTERE, ACMXMONEDA, ACMXSIGGAR, ACMXINTEREFEC, CAN, DIS, warnmsg, AVAL, COL, CCO | CMXsrv_util_det_habil_tasa, CMXsrv_fincol_val_per_tas, CMXsrv_util_fecha, sp_procxmode |
| Form_Load | CMXsrv_grl_fec_serv |  | SRV_MessageService, sp_procxmode |
| Form_Load | CMXsrv_icrd_bus_pago | CAN | sp_procxmode |

---

## PAGCBR
<a name="pagcbr"></a>

| **Segmento** | **Procedimiento Almacenado** | **Tablas Referenciadas** | **Procedimientos Referenciados** |
|-------------|------------------------------|--------------------------|-------------------------------|
| ACEPTAR_Click | CMXsrv_icbr_lee_dat_var | ACMXMONEDAFEC, CBR, ACMXPRMENL | sp_procxmode |
| ACEPTAR_Click | CMXsrv_icbr_val_pag | LCB, CBR, CCO | CMXsrv_val_cta_cte, CMXsrv_calc_imp_4pct, CMXsrv_util_fecha, sp_procxmode, CMXsrv_enl_val_sel, CMXsrv_ctb_impto_ddi |
| ACEPTAR_Click | CMXsrv_icbr_ctb_pag | LCB, ACMXDESEMB, vig_cmx, COD, ICX, COM, ACMXMONEDAFEC, CBR, PCX, DIP, LIB, CLN, CCO | CMXsrv_mbyte_gen, CMXsrv_get_ult_dia_habil, CMXsrv_val_cta_cte, CMXsrv_cnt_gen_vig, CMXsrv_calc_imp_4pct, CMXsrv_util_fecha, CMXsrv_vig_gra_vig, CMXsrv_ipuc_gen_pln, CMXsrv_icbr_act_rem, CMXsrv_enl_act_enl, sp_procxmode, CMXsrv_icbr_ctb_pag1, sp_cmx_sii_1870, CMXsrv_iddi2_gen_det_pag, CMXsrv_cmx_get_codes, CMXsrv_ctb_impto_ddi, CMXsrv_util_pesos |
| Calcular_Click | CMXsrv_icbr_cal_pag | DDI, ADI, ACMXMONEDAFEC, CBR, COB, ACMXMONEDA | CMXsrv_get_ult_dia_habil, sp_procxmode, CMXsrv_valida_tc, CMXsrv_icbr_cal_int, CMXsrv_icbr_cre_pln |
| CANCELAR_Click | CMXsrv_icbr_eli_pag | ECE, PCX, COB, ICX | sp_procxmode |
| fld_cbr_cod_des_mn_pag_lostfocus | CMXsrv_val_vig | ACMXPLNCTAN, ACMXDESEMB, ACMXPLNCTAX | sp_procxmode |
| fld_cbr_cod_des_mx_pag_lostfocus | CMXsrv_val_vig | ACMXPLNCTAN, ACMXDESEMB, ACMXPLNCTAX | sp_procxmode |
| Form_Load | CMXsrv_icbr_lee_cbr0 | ACMXMONEDA, CBR | CMXsrv_icrd_lee_cln, sp_procxmode |
| Form_Load | CMXsrv_icbr_obt_mon_nac |  | CMXsrv_cmx_get_codes, sp_procxmode |
| Form_Load | CMXsrv_icbr_lee_dat_pag | ACMXDESEMB, ECE, PCX, CBR | sp_procxmode |
| Form_Load | CMXsrv_icbr_pcg_pag | ACMXMONEDAFEC, CBR | PrmACMXMONEDAFEC, sp_procxmode |
| lee_cta | CMXsrv_vig_lee_cta | ACMXPLNCTAN, ACMXDESEMB, ACMXPLNCTAX | sp_procxmode |
| Form_Activate | CMXsrv_icbr_busc_pago | PCX | sp_procxmode |
| ACEPTAR_Click | CMXsrv_icbr_val_pag | LCB, CBR, CCO | CMXsrv_val_cta_cte, CMXsrv_calc_imp_4pct, CMXsrv_util_fecha, sp_procxmode, CMXsrv_enl_val_sel, CMXsrv_ctb_impto_ddi |
| Aceptar_Click | CMXsrv_icob_act_val | ACMXMONEDAFEC, COB | CMXsrv_get_ult_dia_habil, sp_procxmode, CMXsrv_icob_val_cob |
| Form_Activate | CMXsrv_icob_lee_val | COB | sp_procxmode |
| ELIMINAR_Click | CMXsrv_icbr_eli_int_pago | PCX, ICX | sp_procxmode |
| Form_Activate | CMXsrv_icbr_busc_int | ICX | sp_procxmode |
| Aceptar_Click | CMXsrv_icbr_ingmod_int | PCX, CBR, ICX, ACMXINTEREFEC | sp_procxmode |
| Form_Activate | CMXsrv_icbr_lee_int_pago | ICX | sp_procxmode |
| Aceptar_Click | CMXsrv_icbr_lee_bco | ACMXPAIS, COR | sp_procxmode |
| buscar_Click | CMXsrv_icbr_busc_bco | COR | sp_procxmode |
| Form_Load | CMXsrv_grl_fec_serv |  | SRV_MessageService, sp_procxmode |

---

