# Índice de Productos y Módulos

## Productos y Módulos

- **Exportaciones**
  - [EXPCBE](#expcbe)
  - [EXPCCE](#expcce)
  - [EXPNEG](#expneg)
  - [expdex](#expdex)
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

---

## Detalles de Módulos

### EXPCBE
| Archivo       | Segmento             | Procedimiento Almacenado |
|--------------|----------------------|--------------------------|
| CBE00101.FRM | Form_Activate | CMXsrv_expcbe_lee_prm |
| CBE00101.FRM | Form_Activate | CMXsrv_cmx_busc_suc_usu |
| CBE00101.FRM | Form_Activate | CMXsrv_expcbe_lee_cbe |
| CBE00101.FRM | Form_Load | CMXsrv_trae_glo_fec |
| CBE00101.FRM | ingcomg_Click | CMXsrv_expcbe_avs_cyg1 |
| CBE00101.FRM | ingcomg_Click | CMXsrv_expcbe_avs_cyg2 |
| CBE00101.FRM | ingret_Click | CMXsrv_expcbe_avs_ret |
| CBE00101.FRM | M3_Click | CMXsrv_expcbe_swf_sel |
| CBE00101.FRM | M4_Click | CMXsrv_expcbe_swf_sel |
| CBE00101.FRM | Mcbeanl_Click | CMXsrv_expcbe_anl_cbe |
| CBE00101.FRM | Mcbectb_Click | CMXsrv_expcbe_ctb_ing |
| CBE00101.FRM | Mcbedel_Click | CMXsrv_expcbe_del_cbe |
| CBE00101.FRM | Mcbeval_Click | CMXsrv_expcbe_val_cbe |
| CBE00101.FRM | Men1_Click | CMXsrv_expcbe_swf_sel |
| CBE00201.FRM | aceptar_Click | CMXsrv_expcbe_grb_ctp |
| CBE00201.FRM | fld_cbe_cod_exp_lostfocus | CMXsrv_expcbe_lee_cln |
| CBE00201.FRM | fld_cbe_cod_suc_LostFocus | CMXsrv_val_suc |
| CBE00201.FRM | Form_Activate | CMXsrv_expcbe_lee_ctp |
| CBE00202.FRM | aceptar_Click | CMXsrv_expcbe_grb_bco |
| CBE00202.FRM | fld_cbe_cod_cob_Lostfocus | CMXsrv_expcbe_lee_cor |
| CBE00202.FRM | fld_cbe_cod_rmb_LostFocus | CMXsrv_expcbe_lee_cor |
| CBE00202.FRM | Form_Activate | CMXsrv_expcbe_lee_bco |
| CBE00204.FRM | aceptar_Click | CMXsrv_expcbe_grb_doc |
| CBE00204.FRM | aceptar_Click | CMXsrv_expcbe_grb_doc02 |
| CBE00204.FRM | Form_Activate | CMXsrv_expcbe_lee_doc |
| CBE00204.FRM | Form_Activate | CMXsrv_expcbe_lee_doc02 |
| CBE00206.FRM | ELIMINAR_Click | CMXsrv_expcbe_del_ctz |
| CBE00206.FRM | Form_Activate | CMXsrv_expcbe_bus_ctz |
| CBE00207.FRM | aceptar_Click | CMXsrv_expcbe_grb_ctz |
| CBE00207.FRM | Form_Activate | CMXsrv_expcbe_mto_ctz |
| CBE00207.FRM | Form_Activate | CMXsrv_expcbe_lee_ctz |
| CBE00301.FRM | aceptar_Click | CMXsrv_expcbe_lee_cbe |
| CBE00301.FRM | buscar_Click | CMXsrv_expcbe_bus_cbe |
| CBE00301.FRM | fld_aux_cod_exp_LostFocus | CMXsrv_expcbe_lee_cln |
| CBE00301.FRM | Proximas_Click | CMXsrv_expcbe_bus_cbe |
| CBE00401.FRM | aceptar_Click | CMXsrv_expcbe_mdf_cbe |
| CBE00401.FRM | aceptar_Click | CMXsrv_expcbe_cre_actz |
| CBE00401.FRM | fld_cbe_cod_suc_LostFocus | CMXsrv_val_suc |
| CBE00401.FRM | Form_Activate | CMXsrv_expcbe_lee_mdf |
| CBE00501.FRM | aceptar_Click | CMXsrv_expcbe_pgo_cbe |
| CBE00501.FRM | fld_cbe_cod_rmb_LostFocus | CMXsrv_expcbe_lee_cor |
| CBE00501.FRM | Form_Activate | CMXsrv_expcbe_lee_pgo |
| CBE00601.FRM | Form_Activate | CMXsrv_expcbe_bus_evz |
| CBE00601.FRM | Proximo_Click | CMXsrv_expcbe_bus_evz |
| CBE00601.FRM | Reversar_Click | CMXsrv_expcbe_rev_cbe |
| CBE00602.FRM | Form_Activate | CMXsrv_expcbe_lee_evz |
| CBE00603.FRM | Eliminar_Click | CMXsrv_expcbe_del_dcz |
| CBE00603.FRM | Form_Activate | CMXsrv_expcbe_bus_dcz |
| CBE00604.FRM | aceptar_Click | CMXsrv_expcbe_grb_dcz |
| CBE00604.FRM | Form_Activate | CMXsrv_expcbe_lee_dcz |
| CBE00605.FRM | aceptar_Click | CMXsrv_expcbe_lee_cbe |
| CBE00605.FRM | buscar_Click | CMXsrv_expcbe_bus_vto |
| CBE00605.FRM | fld_aux_cod_exp_LostFocus | CMXsrv_expcbe_lee_cln |
| CBE00605.FRM | Proximas_Click | CMXsrv_expcbe_bus_vto |
| CBEAVIRE.FRM | aceptar_Click | CMXsrv_avi_dat_cou |
| CBEAVIRE.FRM | aceptar_Click | CMXsrv_expcbe_avs_rem1 |
| CBEAVIRE.FRM | aceptar_Click | CMXsrv_expcbe_avs_rem3 |
| CBEAVIRE.FRM | imprime_esp | CMXsrv_expcbe_avs_rem2 |
| CBEAVIRE.FRM | imprime_esp | CMXsrv_expcbe_avs_rem4 |
| CBEAVIRE.FRM | imprime_ing | CMXsrv_expcbe_avs_rem2 |
| CBEAVIRE.FRM | imprime_ing | CMXsrv_expcbe_avs_rem4 |
| COR00906.FRM | buscar_Click | CMXsrv_busc_plz |
| COR00906.FRM | fld_cor_cod_plz_Lostfocus | CMXsrv_lee_plz |
| COR00906.FRM | proximos_Click | CMXsrv_busc_plz |
| COR00907.FRM | buscar_Click | CMXsrv_cor_busc_pais |
| COR00907.FRM | fld_cor_cod_pais_LostFocus | CMXsrv_cor_lee_pais |
| COR00907.FRM | proximos_Click | CMXsrv_cor_busc_pais |
| CRD00602.FRM | aceptar_Click | CMXsrv_expcbe_lee_cor |
| CRD00602.FRM | buscar_Click | CMXsrv_expcbe_bus_cor |
| CRD00602.FRM | fld_aux_cod_pai_LostFocus | CMXsrv_cor_lee_pais |
| CRD00602.FRM | fld_aux_cod_plz_LostFocus | CMXsrv_lee_plz |
| CRD00602.FRM | proximos_Click | CMXsrv_expcbe_bus_cor |
| GRID_BUS.FRM | buscar_Click | CMXsrv_busc_bco_mtr |
| GRID_BUS.FRM | proximos_Click | CMXsrv_busc_bco_mtr |
| GRL00101.FRM | enviar_Click | CMXsrv_expcbe_swf_sel |
| GRLPAIS0.FRM | Aceptar_Click | CMXsrv_expcbe_lee_cor |
| GRLPAIS0.FRM | buscar_Click | CMXsrv_expcbe_bus_cor |
| GRLPAIS0.FRM | proximos_Click | CMXsrv_expcbe_bus_cor |
| PREFER.FRM | Form_Load | CMXsrv_grl_fec_serv |

### EXPCCE
| Archivo       | Segmento             | Procedimiento Almacenado |
|--------------|----------------------|--------------------------|
| CCE00101.FRM | Form_Activate | CMXsrv_cmx_busc_suc_usu |
| CCE00101.FRM | Form_Activate | CMXsrv_expcce_lee_cce |
| CCE00101.FRM | Form_Activate | CMXsrv_expcce_trd_cce |
| CCE00101.FRM | MCCEANL_CLICK | CMXsrv_expcce_anl_cce |
| CCE00101.FRM | Mccectb_click | CMXsrv_expcce_ctb_ing |
| CCE00101.FRM | Mccedel_Click | CMXsrv_expcce_del_cce |
| CCE00101.FRM | MCCEVAL_CLICK | CMXsrv_expcce_val_cce |
| CCE00101.FRM | Mmt730_Click | CMXsrv_expcce_swf_sel |
| CCE00101.FRM | Mmt730Ing_Click | CMXsrv_expcce_swf_sel |
| CCE00201.FRM | Aceptar_Click | CMXsrv_expcce_grb_bco |
| CCE00201.FRM | fld_cce_bco_avs_LostFocus | CMXsrv_expcce_lee_cor |
| CCE00201.FRM | fld_cce_bco_orig_LostFocus | CMXsrv_expcce_lee_cor |
| CCE00201.FRM | fld_cce_cod_ems_LostFocus | CMXsrv_expcce_lee_cor |
| CCE00201.FRM | fld_cce_cod_rmb_LostFocus | CMXsrv_expcce_lee_cor |
| CCE00201.FRM | Form_Activate | CMXsrv_expcce_lee_bco |
| CCE00202.FRM | Aceptar_Click | CMXsrv_expcce_grb_ctp |
| CCE00202.FRM | fld_cce_cod_bn1_LostFocus | CMXsrv_expcce_lee_cln |
| CCE00202.FRM | fld_cce_cod_bn2_LostFocus | CMXsrv_expcce_lee_cln |
| CCE00202.FRM | Form_Activate | CMXsrv_expcce_lee_ctp |
| CCE00203.FRM | Aceptar_Click | CMXsrv_expcce_cre_cce |
| CCE00203.FRM | Aceptar_Click | CMXsrv_expcce_grb_bco |
| CCE00203.FRM | Aceptar_Click | CMXsrv_expcce_grb_ctp |
| CCE00203.FRM | Aceptar_Click | CMXsrv_expcce_gen_dcc |
| CCE00203.FRM | Aceptar_Click | CMXsrv_expcce_grb_cnd |
| CCE00203.FRM | fld_cce_fec_vto_LostFocus | CMXsrv_util_det_habil |
| CCE00203.FRM | Form_Activate | CMXsrv_expcce_lee_cnd |
| CCE00203.FRM | Form_Activate | CMXsrv_expcce_trd_cnd |
| CCE00204.FRM | ELIMINAR_Click | CMXsrv_expcce_del_dcc |
| CCE00204.FRM | Form_Activate | CMXsrv_expcce_bus_dcc |
| CCE00205.FRM | Aceptar_Click | CMXsrv_expcce_grb_dcc |
| CCE00205.FRM | Form_Activate | CMXsrv_expcce_lee_dcc |
| CCE00301.FRM | Aceptar_Click | CMXsrv_expcce_lee_cce |
| CCE00301.FRM | buscar_Click | CMXsrv_expcce_bus_cce |
| CCE00301.FRM | fld_aux_cod_bn1_lostfocus | CMXsrv_expcce_lee_cln |
| CCE00301.FRM | proximo_Click | CMXsrv_expcce_bus_cce |
| CCE00401.FRM | Aceptar_Click | CMXsrv_expcce_mdf_cce |
| CCE00401.FRM | Cancelar_Click | CMXsrv_expcce_can_mdf |
| CCE00401.FRM | fld_cce_cod_bn1_LostFocus | CMXsrv_expcce_lee_cln |
| CCE00401.FRM | fld_cce_cod_ems_LostFocus | CMXsrv_expcce_lee_cor |
| CCE00401.FRM | Form_Activate | CMXsrv_expcce_lee_mdf |
| CCE00501.FRM | Aceptar_Click | CMXsrv_expcce_cnf_cce |
| CCE00501.FRM | Aceptar_Click | CMXsrv_expcce_grb_afin |
| CCE00501.FRM | Form_Activate | CMXsrv_expcce_lee_cnf |
| CCE00501.FRM | Form_Activate | CMXsrv_expcce_lee_afin |
| CCE00701.FRM | Aceptar_Click | CMXsrv_expcce_trp_cce |
| CCE00701.FRM | fld_cce_bco_dst_LostFocus | CMXsrv_expcce_lee_cor |
| CCE00701.FRM | Form_Activate | CMXsrv_expcce_lee_trp |
| CCE00801.FRM | Form_Activate | CMXsrv_expcce_bus_evc |
| CCE00801.FRM | proximo_Click | CMXsrv_expcce_bus_evc |
| CCE00801.FRM | reversar_Click | CMXsrv_expcce_rev_cce |
| CCE00802.FRM | Form_Activate | CMXsrv_expcce_lee_evc |
| CCEAVIRE.FRM | aceptar_Click | CMXsrv_expcce_avs_rem1 |
| COR00906.FRM | buscar_Click | CMXsrv_busc_plz |
| COR00906.FRM | fld_cor_cod_plz_Lostfocus | CMXsrv_lee_plz |
| COR00906.FRM | proximos_Click | CMXsrv_busc_plz |
| COR00907.FRM | buscar_Click | CMXsrv_cor_busc_pais |
| COR00907.FRM | fld_cor_cod_pais_LostFocus | CMXsrv_cor_lee_pais |
| COR00907.FRM | proximos_Click | CMXsrv_cor_busc_pais |
| CRD00602.FRM | Aceptar_Click | CMXsrv_expcce_lee_cor |
| CRD00602.FRM | buscar_Click | CMXsrv_expcce_bus_cor |
| CRD00602.FRM | Command1_Click | CMXsrv_expcce_bus_cor |
| CRD00602.FRM | proximos_Click | CMXsrv_expcce_bus_cor |
| GRL00101.FRM | enviar_Click | CMXsrv_expcce_swf_sel |
| PREFER.FRM | Form_Load | CMXsrv_grl_fec_serv |

### expdex
| Archivo       | Segmento             | Procedimiento Almacenado |
|--------------|----------------------|--------------------------|
| DEX00101.FRM | form_activate | CMXsrv_expcbe_lee_prm |
| DEX00101.FRM | form_activate | CMXsrv_dex_lee_dex |
| DEX00101.FRM | Mdexeli_Click | CMXsrv_dex_eli_dex |
| DEX00102.FRM | ACEPTAR_Click | CMXsrv_dex_act_dex |
| DEX00102.FRM | fld_dex_dia_plz_max_LostFocus | CMXsrv_expdex_cal_fec |
| DEX00102.FRM | fld_dex_fec_acep_LostFocus | CMXsrv_expdex_cal_fec |
| DEX00102.FRM | fld_dex_rut_exp_LostFocus | CMXsrv_dex_lee_cli |
| DEX00102.FRM | FORM_Load | CMXsrv_dex_lee_dex |
| DEX00103.FRM | Buscar_Click | CMXsrv_dex_bus_dex |
| DEX00103.FRM | fld_dex_rut_exp_LostFocus | CMXsrv_dex_lee_cli |
| PREFER.FRM | FORM_Load | CMXsrv_grl_fec_serv |
| RESPALD2.FRM | ACEPTAR_Click | CMXsrv_dex_act_dex |
| RESPALD2.FRM | fld_dex_rut_exp_LostFocus | CMXsrv_dex_lee_cli |
| RESPALD2.FRM | FORM_Load | CMXsrv_dex_lee_dex |
| RESPALDO.FRM | COMELIMINAR_Click | CMXsrv_dex_eli_dex |
| RESPALDO.FRM | Form_Activate | CMXsrv_dex_lee_dex |

### EXPNEG
| Archivo       | Segmento             | Procedimiento Almacenado |
|--------------|----------------------|--------------------------|
| CBE00601.FRM | Form_Activate | CMXsrv_expcbe_bus_evz |
| CBE00601.FRM | Proximo_Click | CMXsrv_expcbe_bus_evz |
| CBE00601.FRM | Reversar_Click | CMXsrv_expcbe_rev_cbe |
| CBE00602.FRM | Form_Activate | CMXsrv_expcbe_lee_evz |
| CCE00601.FRM | Form_Activate | CMXsrv_expcce_lee_bas |
| CCE00601.FRM | Form_Activate | CMXsrv_expcce_lee_neg |
| CCE00601.FRM | Mccealznge_click | CMXsrv_expcce_alz_dis |
| CCE00601.FRM | Mcceanlnge_click | CMXsrv_expcce_anl_neg |
| CCE00601.FRM | Mccectbnge_Click | CMXsrv_expcce_ctb_neg |
| CCE00601.FRM | Mccedelnge_Click | CMXsrv_expcce_del_neg |
| CCE00601.FRM | Mccevalnge_click | CMXsrv_expcce_val_neg |
| CCE00601.FRM | Mtel742_Click | CMXsrv_expcce_swf_sel |
| CCE00801.FRM | Form_Activate | CMXsrv_expcce_bus_evc |
| CCE00801.FRM | Proximo_Click | CMXsrv_expcce_bus_evc |
| CCE00801.FRM | Reversar_Click | CMXsrv_expcce_rev_cce |
| CCE00802.FRM | Form_Activate | CMXsrv_expcce_lee_evc |
| CCE00901.FRM | aceptar_Click | CMXsrv_expcce_grb_neg |
| CCE00901.FRM | aceptar_Click | CMXsrv_expcce_gen_dcn |
| CCE00901.FRM | aceptar_Click | CMXsrv_expcce_grb_afin |
| CCE00901.FRM | fld_cce_cod_exp_nge_LostFocus | CMXsrv_expcce_lee_cln |
| CCE00901.FRM | fld_cce_cod_pag_nge_LostFocus | CMXsrv_expcce_lee_cor |
| CCE00901.FRM | fld_cce_cod_rmb_nge_LostFocus | CMXsrv_expcce_lee_cor |
| CCE00901.FRM | fld_cce_ins_rem1_nge_GotFocus | CMXsrv_expcce_avs_rem5 |
| CCE00901.FRM | Form_Load | CMXsrv_expcce_lee_nge |
| CCE00901.FRM | Form_Load | CMXsrv_expcce_trd_nge |
| CCE00901.FRM | Form_Load | CMXsrv_expcce_ini_neg |
| CCE00901.FRM | Form_Load | CMXsrv_expcce_lee_afin |
| CCE00901.FRM | lee_bco | CMXsrv_expcce_lee_cor |
| CCE00902.FRM | ELIMINAR_Click | CMXsrv_expcce_del_dcn |
| CCE00902.FRM | Form_Activate | CMXsrv_expcce_bus_dcn |
| CCE00903.FRM | Aceptar_Click | CMXsrv_expcce_grb_dcn |
| CCE00903.FRM | Form_Load | CMXsrv_expcce_lee_dcn |
| CCE00904.FRM | ELIMINAR_Click | CMXsrv_expcce_del_ltr |
| CCE00904.FRM | Form_Activate | CMXsrv_expcce_bus_ltr |
| CCE00905.FRM | Aceptar_Click | CMXsrv_expcce_grb_ltr |
| CCE00905.FRM | Form_Load | CMXsrv_expcce_lee_ltr |
| CCE00906.FRM | ELIMINAR_Click | CMXsrv_expcce_del_dsn |
| CCE00906.FRM | Form_Activate | CMXsrv_expcce_gen_dsn |
| CCE00906.FRM | Form_Activate | CMXsrv_expcce_bus_dsn |
| CCE00906.FRM | Salir_Click | CMXsrv_expcce_chk_dsn |
| CCE00907.FRM | Aceptar_Click | CMXsrv_expcce_grb_dsn |
| CCE00907.FRM | Form_Load | CMXsrv_expcce_lee_dsn |
| CCE01001.FRM | buscar_Click | CMXsrv_expcce_bus_neg |
| CCE01001.FRM | Proximas_Click | CMXsrv_expcce_bus_neg |
| CCE01201.FRM | aceptar_Click | CMXsrv_expcce_pgo_neg |
| CCE01201.FRM | aceptar_Click | CMXsrv_expcce_grb_afin |
| CCE01201.FRM | fld_cce_cod_exp_nge_LostFocus | CMXsrv_expcce_lee_cln |
| CCE01201.FRM | fld_cce_cod_rmb_nge_LostFocus | CMXsrv_expcce_lee_cor |
| CCE01201.FRM | Form_Load | CMXsrv_expcce_lee_pgo |
| CCE01201.FRM | Form_Load | CMXsrv_expcce_lee_afin |
| CCE01201.FRM | lee_bco | CMXsrv_expcce_lee_cor |
| CCEAVIRE.FRM | aceptar_Click | CMXsrv_avi_dat_cou |
| CCEAVIRE.FRM | aceptar_Click | CMXsrv_expcce_lee_nge |
| CCEAVIRE.FRM | aceptar_Click | CMXsrv_expcce_avs_rem1 |
| CCEAVIRE.FRM | aceptar_Click | CMXsrv_expcce_avs_rem3 |
| CCEAVIRE.FRM | imprime_esp | CMXsrv_expcce_avs_rem2 |
| CCEAVIRE.FRM | imprime_esp | CMXsrv_expcce_avs_rem4 |
| CCEAVIRE.FRM | imprime_esp | CMXsrv_expcbe_avs_rem4 |
| CCEAVIRE.FRM | imprime_ing | CMXsrv_expcce_avs_rem2 |
| CCEAVIRE.FRM | imprime_ing | CMXsrv_expcce_avs_rem4 |
| CCEAVIRE.FRM | imprime_ing | CMXsrv_expcbe_avs_rem4 |
| CRD00602.FRM | aceptar_Click | CMXsrv_expcce_lee_cor |
| CRD00602.FRM | buscar_Click | CMXsrv_expcce_bus_cor |
| CRD00602.FRM | proximos_Click | CMXsrv_expcce_bus_cor |
| GRL00101.FRM | enviar_Click | CMXsrv_expcce_swf_sel |
| PREFER.FRM | Form_Load | CMXsrv_grl_fec_serv |

### expret
| Archivo       | Segmento             | Procedimiento Almacenado |
|--------------|----------------------|--------------------------|
| COR00906.FRM | buscar_Click | CMXsrv_busc_plz |
| COR00906.FRM | fld_cor_cod_plz_Lostfocus | CMXsrv_lee_plz |
| COR00906.FRM | proximos_Click | CMXsrv_busc_plz |
| COR00907.FRM | buscar_Click | CMXsrv_cor_busc_pais |
| COR00907.FRM | fld_cor_cod_pais_LostFocus | CMXsrv_cor_lee_pais |
| COR00907.FRM | proximos_Click | CMXsrv_cor_busc_pais |
| CRD00602.FRM | Aceptar_Click | CMXsrv_expcbe_lee_cor |
| CRD00602.FRM | buscar_Click | CMXsrv_expcbe_bus_cor |
| CRD00602.FRM | proximos_Click | CMXsrv_expcbe_bus_cor |
| GRL00101.FRM | Command2_Click | CMXsrv_expret_swf_sel |
| PREFER.FRM | Form_Load | CMXsrv_grl_fec_serv |
| RET00101.FRM | Form_Activate | CMXsrv_cmx_busc_suc_usu |
| RET00101.FRM | Form_Activate | CMXsrv_expret_lee_ret |
| RET00101.FRM | Form_Load | CMXsrv_expret_lee_prm |
| RET00101.FRM | M_cgyc_Click | CMXsrv_expret_avs_cyg1 |
| RET00101.FRM | M_cgyc_Click | CMXsrv_expret_avs_cyg2 |
| RET00101.FRM | mavisliq_Click | CMXsrv_expret_avs_liq1 |
| RET00101.FRM | mavisliq_Click | CMXsrv_expret_avs_liq2 |
| RET00101.FRM | mavisliq_Click | CMXsrv_expret_avs_liq3 |
| RET00101.FRM | Mcbectb_Click | CMXsrv_expret_val_ret |
| RET00101.FRM | Mcbectb_Click | CMXsrv_expret_sum_dtn_mn |
| RET00101.FRM | Mcbectb_Click | CMXsrv_expret_ctb_ing |
| RET00101.FRM | Mcbedel_Click | CMXsrv_expret_del_ret |
| RET00101.FRM | Mliqctb_Click | CMXsrv_expret_avs_adm1 |
| RET00101.FRM | Mliqctb_Click | CMXsrv_expret_avs_adm2 |
| RET00101.FRM | Mliqctb_Click | CMXsrv_expret_avs_adm3 |
| RET00101.FRM | Mvalid_Click | CMXsrv_expret_val_ret |
| RET00101.FRM | plv2_Click | CMXsrv_ret_ipuc_gen_pln |
| RET00102.FRM | ACEPTAR_Click | CMXsrv_expret_act_tpo_cbo |
| RET00102.FRM | ACEPTAR_Click | CMXsrv_expret_val_ret |
| RET00201.FRM | ACEPTAR_Click | CMXsrv_expret_cre_ret |
| RET00201.FRM | ACEPTAR_Click | CMXsrv_expret_grb_det |
| RET00201.FRM | fld_ret_mon_ret_LostFocus | CMXsrv_expret_tpo_cbo |
| RET00201.FRM | fld_ret_rut_cli_LostFocus | CMXsrv_expret_lee_cln |
| RET00201.FRM | Form_Load | CMXsrv_expret_lee_det |
| RET00301.FRM | ELIMINAR_Click | CMXsrv_expret_del_org |
| RET00301.FRM | Form_Activate | CMXsrv_expret_bus_org |
| RET00401.FRM | ACEPTAR_Click | CMXsrv_expret_grb_org |
| RET00401.FRM | Form_Activate | CMXsrv_expret_mto_org |
| RET00401.FRM | Form_Activate | CMXsrv_expret_lee_org |
| RET00401.FRM | valida_vigente | CMXsrv_vig_lee_cta |
| RET00501.FRM | ELIMINAR_Click | CMXsrv_expret_del_dtn |
| RET00501.FRM | emitir_Click | CMXsrv_expret_swf_sel |
| RET00501.FRM | Form_Activate | CMXsrv_expret_bus_dtn |
| RET00501.FRM | Planillas_Click | CMXsrv_ret_ipuc_gen_pln |
| RET00601.FRM | ACEPTAR_Click | CMXsrv_expret_grb_dtn |
| RET00601.FRM | fld_ret_cod_ben_LostFocus | CMXsrv_expret_lee_cln |
| RET00601.FRM | fld_ret_mto_arb_LostFocus | CMXsrv_expret_cal_arb |
| RET00601.FRM | fld_ret_mto_ben_LostFocus | CMXsrv_expret_cal_arb |
| RET00601.FRM | fld_ret_par_ben_LostFocus | CMXsrv_expret_cal_arb |
| RET00601.FRM | Form_Activate | CMXsrv_expret_mto_dtn |
| RET00601.FRM | Form_Load | CMXsrv_expret_lee_dtn |
| RET00601.FRM | Form_Load | CMXsrv_expret_lee_cln |
| RET00701.FRM | buscar_Click | CMXsrv_expret_bus_ret |
| RET00701.FRM | fld_ret_rut_cli_LostFocus | CMXsrv_expret_lee_cln |
| RET00701.FRM | proxima_Click | CMXsrv_expret_bus_ret |
| RET00801.FRM | Command1_Click | CMXsrv_expret_bus_evr |
| RET00801.FRM | Form_Activate | CMXsrv_expret_bus_evr |
| RET00801.FRM | proximo_Click | CMXsrv_expret_bus_evr |
| RET00801.FRM | reversar_Click | CMXsrv_expret_rev_ret |
| RET00802.FRM | Form_Load | CMXsrv_expret_lee_evr |

### ADMIN
| Archivo       | Segmento             | Procedimiento Almacenado |
|--------------|----------------------|--------------------------|
| ADM00201.FRM | COMMAND4_Click | CMXsrv_finadm_imod_desti |
| ADM00201.FRM | Form_Load | CMXsrv_finadm_cons_dtip |
| ADM00202.FRM | Command1_Click | CMXsrv_finadm_imod_ectb |
| ADM00202.FRM | Command2_Click | CMXsrv_finadm_eli_tipop |
| ADM00202.FRM | Form_Load | CMXsrv_finadm_cons_ectb |
| ADM00203.FRM | COMMAND3_Click | CMXsrv_finadm_eli_tipop |
| ADM00203.FRM | COMMAND4_Click | CMXsrv_finadm_imod_itip |
| ADM00203.FRM | Form_Load | CMXsrv_finadm_cons_itip |
| ADM00204.FRM | Form_Activate | CMXsrv_finadm_lee_tipop |
| ADM00204.FRM | Form_Load | CMXsrv_grl_fec_serv |
| ADM00204.FRM | Mdel_Click | CMXsrv_finadm_eli_tipop |
| ADM00204.FRM | Mval_Click | CMXsrv_finadm_val_tipop |
| ADM00205.FRM | buscar_Click | CMXsrv_finadm_bus_tipope |
| ADM00205.FRM | proximas_Click | CMXsrv_finadm_bus_tipope |

### COL_NEG
| Archivo       | Segmento             | Procedimiento Almacenado |
|--------------|----------------------|--------------------------|
| COL00102.FRM | CANCELAR_Click | CMXsrv_busc_tip_tas |
| COL00102.FRM | ELIMINAR_Click | CMXsrv_fincol_ecuo |
| COL00102.FRM | Form_Activate | CMXsrv_fincol_cons_plnpa |
| COL00102.FRM | Form_Load | CMXsrv_pertas_val_display |
| COL00103.FRM | ELIMINAR_Click | CMXsrv_fincol_eava |
| COL00103.FRM | Form_Activate | CMXsrv_fincol_cons_aval |
| COL00113.FRM | ingresar_Click | CMXsrv_fincol_iava |
| COL00302.FRM | CONTABILIZAR_Click | CMXsrv_fincol_ictb_pag |
| COL00303.FRM | aviso_Click | CMXsrv_fincol_avi_2_fin |
| COL00303.FRM | Form_Activate | CMXsrv_fincol_cons_pag |
| COL00303.FRM | proximos_Click | CMXsrv_fincol_cons_pag |
| COL00304.FRM | Form_Activate | CMXsrv_fincol_trae_det_pag |
| COL00403.FRM | aviso_Click | CMXsrv_fincol_avi_3_fin |
| COL00403.FRM | Form_Activate | CMXsrv_fincol_cons_pror |
| COL00901.FRM | EFECTUAR_Click | CMXsrv_fincol_rev_eve |
| COL00901.FRM | Form_Activate | CMXsrv_fincol_cons_eve |
| CRD00602.FRM | Aceptar_Click | CMXsrv_icrd_lee_bco_swf |
| CRD00602.FRM | buscar_Click | CMXsrv_icrd_busc_bco |
| CRD00602.FRM | proximo_Click | CMXsrv_icrd_busc_bco |
| CRD01401.FRM | Aceptar_Click | CMXsrv_fincol_vtocre_prov |
| CRD01401.FRM | Form_Load | CMXsrv_fincol_prec_vtocre |
| CRD02001.FRM | buscar_Click | CMXsrv_icrd_bus_lcr_bco |
| CRD02001.FRM | proximo_Click | CMXsrv_icrd_bus_lcr_bco |
| PREFER.FRM | Form_Load | CMXsrv_grl_fec_serv |
| PREFER.FRM | Form_Load | CMXsrv_lee_fpro |

### INGRESO
| Archivo       | Segmento             | Procedimiento Almacenado |
|--------------|----------------------|--------------------------|
| COL00102.FRM | cancelar_Click | CMXsrv_fincol_ren_fin |
| COL00102.FRM | ELIMINAR_Click | CMXsrv_fincol_ecuo |
| COL00102.FRM | form_activate | CMXsrv_fincol_gpln |
| COL00102.FRM | form_activate | CMXsrv_fincol_cons_plnpa |
| COL00103.FRM | cancelar_Click | CMXsrv_fincol_ren_fin |
| COL00103.FRM | ELIMINAR_Click | CMXsrv_fincol_eava |
| COL00103.FRM | form_activate | CMXsrv_fincol_cons_aval |
| COL00104.FRM | aceptar_Click | CMXsrv_fincol_gmod_ctr |
| COL00104.FRM | busca_bco | CMXsrv_icrd_lee_bco_swf |
| COL00104.FRM | fld_obl_bco_acr_LostFocus | CMXsrv_fincol_lee_bco |
| COL00104.FRM | fld_obl_rut_acr_LostFocus | CMXsrv_fincol_lee_cln |
| COL00104.FRM | form_activate | CMXsrv_fincol_cons_ctr |
| COL00105.FRM | aceptar_Click | CMXsrv_fincol_ctb_oto |
| COL00106.FRM | avi1_Click | CMXsrv_icrd_avi_crd |
| COL00106.FRM | Avi5_Click | CMXsrv_icrd_dat_liq_ope |
| COL00106.FRM | form_activate | CMXsrv_fincol_lee_col |
| COL00106.FRM | Form_Load | CMXsrv_lee_fpro |
| COL00106.FRM | MCOLCOMI_CLICK | CMXsrv_busc_cod_ope |
| COL00106.FRM | MCOLCOMI_CLICK | CMXsrv_col_trae_num_ope |
| COL00106.FRM | MCOLCONTOTOR_CLICK | CMXsrv_busc_cod_ope |
| COL00106.FRM | MCOLCONTOTOR_CLICK | CMXsrv_col_trae_num_ope |
| COL00106.FRM | MCOLCONTOTOR_CLICK | CMXsrv_fincol_ctb_oto |
| COL00106.FRM | MCOLELI_CLICK | CMXsrv_fincol_eli_col |
| COL00106.FRM | valida | CMXsrv_fincol_val_col |
| COL00107.FRM | aceptar_Click | CMXsrv_fincol_lee_col |
| COL00107.FRM | buscar_Click | CMXsrv_fincol_bsc_col |
| COL00107.FRM | fld_col_tip_ope_lostfocus | CMXsrv_fincol_lee_tip |
| COL00107.FRM | PROXIMAS_Click | CMXsrv_fincol_bsc_col |
| COL00108.FRM | buscar_Click | CMXsrv_fincol_bsc_TIP |
| COL00113.FRM | ingresar_Click | CMXsrv_fincol_iava |
| COL00701.FRM | aceptar_Click | CMXsrv_busc_cod_ope |
| COL00701.FRM | aceptar_Click | CMXsrv_col_trae_num_ope |
| COL00701.FRM | aceptar_Click | CMXsrv_fincol_ctb_novf |
| COL00701.FRM | FLD_COL_COD_CLI_LOSTFOCUS | CMXsrv_fincol_lee_cln |
| COL00701.FRM | FLD_COL_RUT_DEU_NOV_LostFocus | CMXsrv_fincol_lee_cln |
| COL00702.FRM | form_activate | CMXsrv_fincol_cons_nov |
| COL00703.FRM | FLD_COL_COD_CLI_LOSTFOCUS | CMXsrv_fincol_lee_cln |
| COL00703.FRM | FLD_COL_RUT_DEU_NOV_LostFocus | CMXsrv_fincol_lee_cln |
| COL00703.FRM | form_activate | CMXsrv_fincol_cons_dnov |
| COL00704.FRM | cmdAceptar_Click | CMXsrv_grabar_pag_adi_dus |
| COL00704.FRM | Form_Load | CMXsrv_buscar_pag_adi_dus |
| CRD00602.FRM | Aceptar_Click | CMXsrv_icrd_lee_bco_swf |
| CRD00602.FRM | buscar_Click | CMXsrv_icrd_busc_bco |
| CRD00602.FRM | proximo_Click | CMXsrv_icrd_busc_bco |
| PREFER.FRM | Form_Load | CMXsrv_cmx_get_codes |
| PREFER.FRM | Form_Load | CMXsrv_grl_trae_cod_bco |

### MODIFIC
| Archivo       | Segmento             | Procedimiento Almacenado |
|--------------|----------------------|--------------------------|
| COL00303.FRM | Form_Activate | CMXsrv_fincol_cons_tas |
| COL00801.FRM | aceptar_click | CMXsrv_fincol_efec_tras |
| COL00802.FRM | Form_Activate | CMXsrv_fincol_cons_trasp |
| COL00803.FRM | Form_Activate | CMXsrv_fincol_cons_dtrs |
| COL00901.FRM | EFECTUAR_Click | CMXsrv_fincol_rev_eve |
| COL00901.FRM | Form_Activate | CMXsrv_fincol_cons_eve |
| COL00902.FRM | Form_Load | CMXsrv_fincol_cons_deve |
| COL01001.FRM | aceptar_click | CMXsrv_fincol_cont_gst |
| COL01002.FRM | Form_Activate | CMXsrv_fincol_cons_gst |
| COL01003.FRM | Form_Activate | CMXsrv_fincol_cons_dgst |
| PREFER.FRM | Form_Load | CMXsrv_lee_fpro |

### OBLIGA
| Archivo       | Segmento             | Procedimiento Almacenado |
|--------------|----------------------|--------------------------|
| COL00108.FRM | buscar_Click | CMXsrv_fincol_bsc_tip |
| COL00108.FRM | Proxima_Click | CMXsrv_fincol_bsc_tip |
| COL00108.FRM | proximo_Click | CMXsrv_fincol_bsc_tip |
| CRD00602.FRM | buscar_Click | CMXsrv_finobl_bus_cor |
| CRD00602.FRM | proximo_Click | CMXsrv_finobl_bus_cor |
| OBL00102.FRM | ELIMINAR_Click | CMXsrv_finobl_ecuo |
| OBL00102.FRM | form_activate | CMXsrv_finobl_gpln |
| OBL00102.FRM | form_activate | CMXsrv_finobl_cons_plnpa |
| OBL00103.FRM | anunctb_Click | CMXsrv_finobl_calc_anu |
| OBL00103.FRM | form_activate | CMXsrv_finobl_lee_obl |
| OBL00103.FRM | Form_Load | CMXsrv_lee_fpro |
| OBL00103.FRM | Mcbeanl_Click | CMXsrv_finobl_calc_anu |
| OBL00103.FRM | Mcbectb_Click | CMXsrv_finobl_ctb_oto |
| OBL00103.FRM | Mcbedel_Click | CMXsrv_fincol_eli_obl |
| OBL00103.FRM | Mobl_liq_ope_Click | CMXsrv_icrd_dat_liq_ope |
| OBL00103.FRM | valida_error | CMXsrv_finobl_val_obl |
| OBL00104.FRM | buscar_Click | CMXsrv_finobl_bsc_obl |
| OBL00104.FRM | fld_obl_tip_ope_LostFocus | CMXsrv_fincol_lee_tip |
| OBL00104.FRM | Proxima_Click | CMXsrv_finobl_bsc_obl |
| OBL00202.FRM | contabilizar_Click | CMXsrv_finobl_ictb_pag |
| OBL00202.FRM | contabilizar_Click | CMXsrv_finobl_obt_sdocuo |
| OBL00202.FRM | form_activate | CMXsrv_finobl_new_tas |
| OBL00203.FRM | form_activate | CMXsrv_finobl_cons_pag |
| OBL00204.FRM | form_activate | CMXsrv_finobl_cons_detp |
| OBL00301.FRM | calcular_Click | CMXsrv_finobl_calc_pror |
| OBL00303.FRM | form_activate | CMXsrv_finobl_cons_pror |
| OBL00304.FRM | form_activate | CMXsrv_finobl_cons_dpror |
| OBL00401.FRM | contabilizar_Click | CMXsrv_finobl_ctb_anu |
| OBL00402.FRM | calcular_Click | CMXsrv_finobl_calc_anu |
| OBL00402.FRM | form_activate | CMXsrv_finobl_cons_anu |
| OBL00502.FRM | form_activate | CMXsrv_finobl_cons_mod |
| OBL00503.FRM | form_activate | CMXsrv_finobl_cons_dmod |
| OBL00601.FRM | efectuar_Click | CMXsrv_finobl_rev_eve |
| OBL00601.FRM | form_activate | CMXsrv_finobl_cons_eve |
| OBL00602.FRM | form_activate | CMXsrv_finobl_cons_deve |
| OBL00701.FRM | ELIMINAR_Click | CMXsrv_finobl_eli_ctr |
| OBL00701.FRM | form_activate | CMXsrv_finobl_cons_ctr |
| OBL00702.FRM | nuevo_Click | CMXsrv_finobl_ing_ctr |
| OBL130.FRM | aceptar_Click | CMXsrv_finobl_cesion_obl |
| OBL130.FRM | banco_acreedor | CMXsrv_comgrl_lee_nom_cor |
| OBL130.FRM | fld_obl_cod_bco_acre_lostfocus | CMXsrv_comgrl_lee_nom_cor |
| OBL130.FRM | fld_obl_rut_acre_lostfocus | CMXsrv_lee_cln |
| OBL130.FRM | form_activate | CMXsrv_finobl_busc_acre |
| PREFER.FRM | Form_Load | CMXsrv_cmx_get_codes |

### PAGOS
| Archivo       | Segmento             | Procedimiento Almacenado |
|--------------|----------------------|--------------------------|
| COL00108.FRM | buscar_Click | CMXsrv_fincol_bsc_TIP |
| COL00301.FRM | CALCULAR_Click | CMXsrv_fincol_efec_calpa |
| COL00302.FRM | Contabilizar_Click | CMXsrv_fincol_ictb_pag |
| COL00303.FRM | Form_Activate | CMXsrv_fincol_cons_pag |
| COL00304.FRM | Form_Load | CMXsrv_fincol_cons_detp |
| COL00401.FRM | Aceptar_Click | CMXsrv_fincol_calc_pror |
| COL00402.FRM | Contabilizar_Click | CMXsrv_fincol_cont_pror |
| COL00403.FRM | Form_Activate | CMXsrv_fincol_cons_pror |
| COL00404.FRM | Form_Activate | CMXsrv_fincol_cons_dpror |
| COL00501.FRM | Aceptar_Click | CMXsrv_busc_cod_ope |
| COL00501.FRM | Aceptar_Click | CMXsrv_col_trae_num_ope |
| COL00501.FRM | Aceptar_Click | CMXsrv_fincol_cctb_anu |
| COL00501.FRM | Form_Load | CMXsrv_fincol_calc_anu |
| COL00501.FRM | Form_Load | CMXsrv_busc_cod_ope |
| COL00502.FRM | CALCULAR_Click | CMXsrv_fincol_calc_anu |
| COL00502.FRM | Form_Activate | CMXsrv_fincol_cons_anu |
| COL00602.FRM | Form_Activate | CMXsrv_fincol_cons_mod |
| COL00603.FRM | Form_Activate | CMXsrv_fincol_cons_dmod |
| PREFER.FRM | Form_Load | CMXsrv_lee_fpro |
| PREFER.FRM | Form_Load | CMXsrv_grl_trae_cod_bco |

### PGOEXT
| Archivo       | Segmento             | Procedimiento Almacenado |
|--------------|----------------------|--------------------------|
| PGOCOL01.FRM | calcular_Click | CMXsrv_fincol_cal_pext |
| PGOCOL01.FRM | Contabilizar_Click | CMXsrv_busc_cod_ope |
| PGOCOL01.FRM | Contabilizar_Click | CMXsrv_fincol_ctb_pext |
| PGOOBL01.FRM | calcular_Click | CMXsrv_finobl_cal_pext |
| PGOOBL01.FRM | Contabilizar_Click | CMXsrv_finobl_ctb_pext |
| PREFER.FRM | Form_Load | CMXsrv_grl_fec_serv |
| PREFER.FRM | Form_Load | CMXsrv_lee_fpro |

### ARCOS
| Archivo       | Segmento             | Procedimiento Almacenado |
|--------------|----------------------|--------------------------|
| ARC00100.FRM | Eliminar_Click | CMXsrv_iarc_eli_arc |
| ARC00100.FRM | Form_activate | CMXsrv_iarc_busc_arc |
| ARC00101.FRM | aceptar_click | CMXsrv_iinf_busc_inf |
| ARC00101.FRM | aceptar_click | CMXsrv_iarc_act_arc |
| ARC00101.FRM | Form_Load | CMXsrv_iarc_lee_arc |
| INFO0201.FRM | buscar_Click | CMXsrv_iinf_busc_opr |
| INFO0201.FRM | Form_activate | CMXsrv_iinf_lee_vlr |
| INFO0202.FRM | aceptar_click | CMXsrv_iarc_act_arc |
| INFO0202.FRM | Form_activate | CMXsrv_iinf_busc_inf |
| INFO0202.FRM | reversar_Click | CMXsrv_iinf_rev_evi |

### COBERIMP
| Archivo       | Segmento             | Procedimiento Almacenado |
|--------------|----------------------|--------------------------|
| COB00101.FRM | Form_Activate | CMXsrv_icob_lee_pln |
| COB00101.FRM | Mcobcur_Click | CMXsrv_icob_cur_cob |
| COB00101.FRM | Mcobcur_Click | CMXsrv_icob_pag_sop |
| COB00101.FRM | MCOBELI_CLICK | CMXsrv_icob_eli_pln |
| COB00101.FRM | Mcobrev_Click | CMXsrv_icob_rev_etd |
| COB00101.FRM | Mcobvali_Click | CMXsrv_icob_val_cob |
| COB00201.FRM | buscar_click | CMXsrv_icob_busc_pln |
| COB00201.FRM | FLD_COB_COD_CLI_LostFocus | CMXsrv_icob_lee_cln |
| COB00201.FRM | PROXIMAS_Click | CMXsrv_icob_busc_pln |
| COB00300.FRM | ACEPTAR_Click | CMXsrv_icob_crea_norm |
| COB00301.FRM | ACEPTAR_Click | CMXsrv_icob_crea_reem |
| COB00302.FRM | ACEPTAR_Click | CMXsrv_icob_act_gral |
| COB00302.FRM | FLD_COB_COD_CLI_LostFocus | CMXsrv_icob_lee_cln2 |
| COB00302.FRM | Form_Activate | CMXsrv_icob_lee_gral |
| COB00303.FRM | ACEPTAR_Click | CMXsrv_icob_act_val |
| COB00303.FRM | Form_Activate | CMXsrv_icob_lee_val |
| COB00304.FRM | ACEPTAR_Click | CMXsrv_icob_act_acu |
| COB00304.FRM | Form_Activate | CMXsrv_icob_lee_acu |
| COB00304.FRM | Form_Load | CMXsrv_icob_lee_acu |
| COB00305.FRM | ELIMINAR_Click | CMXsrv_icob_eli_int |
| COB00305.FRM | Form_Activate | CMXsrv_icob_busc_int |
| COB00306.FRM | ACEPTAR_Click | CMXsrv_icob_ingmod_int |
| COB00306.FRM | Form_Activate | CMXsrv_icob_lee_int |
| COB00307.FRM | ACEPTAR_Click | CMXsrv_icob_ing_mod_srf |
| COB00307.FRM | CmdEliminar_Click | CMXsrv_icob_eli_pln |
| COB00307.FRM | CmdReversar_Click | CMXsrv_icob_rev_etd |
| COB00307.FRM | CURSAR_Click | CMXsrv_icob_ing_mod_srf |
| COB00307.FRM | CURSAR_Click | CMXsrv_icob_pag_sop |
| COB00307.FRM | FLD_COB_COD_CLI_LostFocus | CMXsrv_icob_lee_cln2 |
| COB00307.FRM | Form_Activate | CMXsrv_icob_lee_srf |
| COB00307.FRM | Reversar_Click | CMXsrv_icob_rev_etd |
| COB00501.FRM | ACEPTAR_Click | CMXsrv_icob_anu |
| COB00501.FRM | Form_Load | CMXsrv_icob_lee_anu |
| COB0601.FRM | ACEPTAR_Click | CMXsrv_icob_act_cur_a_pag |
| COB0601.FRM | buscar_click | CMXsrv_icob_bus_cur_a_pag |
| COB0601.FRM | FLD_COB_COD_CLI_LostFocus | CMXsrv_icob_lee_cln |
| FORM2.FRM | ACEPTAR_Click | CMXsrv_icob_pag_sop |
| ORI_DEST.FRM | ACEPTAR_Click | CMXsrv_icob_cur_reem |
| PREFER.FRM | Form_Load | CMXsrv_grl_fec_serv |

### COBRANZA
| Archivo       | Segmento             | Procedimiento Almacenado |
|--------------|----------------------|--------------------------|
| CBR00101.FRM | ejecut_avi_imp_999 | CMXsrv_busc_cor_swf |
| CBR00101.FRM | ejecut_avi_imp_999 | CMXsrv_swf_bus_sms |
| CBR00101.FRM | Form_Activate | CMXsrv_icbr_lee_cbr |
| CBR00101.FRM | Form_Load | CMXsrv_grl_fec_serv |
| CBR00101.FRM | Mcbrace_Click | CMXsrv_icbr_acep_let |
| CBR00101.FRM | Mcbrcon_Click | CMXsrv_icbr_cont_cbr |
| CBR00101.FRM | Mcbreli_click | CMXsrv_icbr_eli_cbr |
| CBR00101.FRM | McbrTxt999_Click | CMXsrv_icbr_lee_ctp |
| CBR00101.FRM | Mcbrtxtrec_Click | CMXsrv_icbr_avi1 |
| CBR00102.FRM | aceptar_Click | CMXsrv_val_suc |
| CBR00102.FRM | buscar_Click | CMXsrv_icbr_busc_cbr |
| CBR00102.FRM | fld_aux_glo_ofi_LostFocus | CMXsrv_val_suc |
| CBR00102.FRM | fld_cbr_cod_gdo_LostFocus | CMXsrv_icbr_lee_cln |
| CBR00102.FRM | fld_cbr_cod_ofi_lostfocus | CMXsrv_val_suc |
| CBR00102.FRM | proximas_Click | CMXsrv_icbr_busc_cbr |
| CBR00103.FRM | crear_Click | CMXsrv_icbr_crea_cbr |
| CBR00103.FRM | fld_cbr_cod_gdo_LostFocus | CMXsrv_icbr_lee_cln |
| CBR00103.FRM | fld_cbr_cod_ofi_lostfocus | CMXsrv_val_suc |
| CBR00103.FRM | INGRESAR_Click | CMXsrv_icbr_crea_cbr |
| CBR00201.FRM | fld_cbr_cod_gdo_LostFocus | CMXsrv_icbr_lee_cln |
| CBR00201.FRM | Form_Activate | CMXsrv_icbr_lee_cob |
| CBR00201.FRM | Form_Load | CMXsrv_icbr_lee_ctp |
| CBR00201.FRM | INGRESAR_Click | CMXsrv_icbr_act_ctp |
| CBR00202.FRM | Form_Activate | CMXsrv_icbr_lee_cob |
| CBR00202.FRM | Form_Load | CMXsrv_icbr_lee_trm |
| CBR00202.FRM | INGRESAR_Click | CMXsrv_icbr_act_trm |
| CBR00203.FRM | Form_Activate | CMXsrv_icbr_lee_cob |
| CBR00203.FRM | Form_Load | CMXsrv_icbr_lee_doc |
| CBR00203.FRM | INGRESAR_Click | CMXsrv_icbr_act_doc |
| CBR00301.FRM | Form_Activate | CMXsrv_icbr_busc_let |
| CBR00302.FRM | aceptar_Click | CMXsrv_icbr_ingmod_let |
| CBR00302.FRM | eliminar_Click | CMXsrv_icbr_eli_let |
| CBR00302.FRM | Form_Activate | CMXsrv_icbr_lee_let |
| CBR00305.FRM | aceptar_Click | CMXsrv_icbr_prorr |
| CBR00401.FRM | EFECTUAR_Click | CMXsrv_icbr_rev_eve |
| CBR00401.FRM | Form_Activate | CMXsrv_icbr_busc_eve |
| CBR00402.FRM | Form_Load | CMXsrv_icbr_lee_eve |
| CBR00402.FRM | Form_Load | CMXsrv_icbr_lee_ent_doc |
| CBR00701.FRM | aceptar_Click | CMXsrv_icbr_prot |
| CBR00701.FRM | Form_Load | CMXsrv_icbr_pcg_prot |
| CBR00801.FRM | aceptar_Click | CMXsrv_icbr_liq_sdo |
| CBR00802.FRM | aceptar_Click | CMXsrv_icbr_act_vis |
| CBR00802.FRM | eliminar_Click | CMXsrv_icbr_eli_rep |
| CBR00802.FRM | Form_Activate | CMXsrv_icbr_busc_rep |
| CBR00803.FRM | aceptar_Click | CMXsrv_icbr_imod_rep |
| CBR00804.FRM | aceptar_Click | CMXsrv_icbr_ent_doc |
| CBR00804.FRM | Form_Load | CMXsrv_icbr_lee_ent_doc |
| CBR00901.FRM | aceptar_Click | CMXsrv_icbr_trf_ofi |
| CBR00901.FRM | aceptar_Click | CMXsrv_val_suc |
| CBR00902.FRM | aceptar_Click | CMXsrv_icbr_trf_bco |
| COBERTU.FRM | aceptar_Click | CMXsrv_icbr_act_inst |
| GRL00101.FRM | enviar_Click | CMXsrv_iswf_a_pru |
| GRL00101.FRM | Form_Load | CMXsrv_icbr_val_cbr |
| GRL00101.FRM | word_Click | CMXsrv_icbr_val_cbr |
| GRL00101.FRM | word_Click | CMXsrv_iswf_a_pru |

### CRDEXT
| Archivo       | Segmento             | Procedimiento Almacenado |
|--------------|----------------------|--------------------------|
| BCO_BCO.FRM | Aceptar_Click | CMXsrv_icrd_a_ibab |
| BCO_BCO.FRM | Form_Load | CMXsrv_icrd_lee_glo_ibab |
| BCO_REM.FRM | Aceptar_Click | CMXsrv_icrd_a_ibar |
| BCO_REM.FRM | Form_Load | CMXsrv_icrd_lee_glo_ibar |
| BUSC_COD.FRM | buscar_click | CMXsrv_icrd_lee_tex_swf |
| BUSC_TXT.FRM | Aceptar_Click | CMXsrv_icrd_lee_cod_txt_swf |
| BUSC_TXT.FRM | buscar_click | CMXsrv_icrd_lee_txt_swf_all |
| BUSC_TXT.FRM | Form_Load | CMXsrv_icrd_lee_ind_esp_ing |
| BUSC_TXT.FRM | llena_arreglo | CMXsrv_icrd_lee_tex_swf |
| BUSC_TXT.FRM | proximo_Click | CMXsrv_icrd_lee_txt_swf_all |
| CRD00207.FRM | aceptar_Click | CMXsrv_icrd_ing_acu |
| CRD00207.FRM | Form_Load | CMXsrv_icrd_lee_acu |
| CRD00701.FRM | aceptar_Click | CMXsrv_icrd_rech_sol |
| CRD00801.FRM | aceptar_Click | CMXsrv_icrd_end |
| CRD00801.FRM | Form_Load | CMXsrv_icrd_lee_dat_end |
| CRD02001.FRM | aceptar_Click | CMXsrv_icrd_asignar_cor |
| CRD02001.FRM | buscar_Click | CMXsrv_icrd_bus_lcr_bco |
| CRD02001.FRM | proximo_Click | CMXsrv_icrd_bus_lcr_bco |
| PREFER.FRM | Form_Load | CMXsrv_grl_fec_serv |

### CRD_CORR
| Archivo       | Segmento             | Procedimiento Almacenado |
|--------------|----------------------|--------------------------|
| COR00202.FRM | aceptar_Click | CMXsrv_icrd_asignar_cor |
| COR00202.FRM | buscar_Click | CMXsrv_icrd_bus_lcr_bco |
| COR00202.FRM | fld_cor_cod_mtr_LostFocus | CMXsrv_icrd_lee_bco_mtr |
| COR00202.FRM | fld_cor_cod_pais_Lostfocus | CMXsrv_icrd_cor_lee_pais |
| COR00202.FRM | fld_cor_cod_plz_Lostfocus | CMXsrv_icrd_lee_plz |
| COR00202.FRM | proximo_Click | CMXsrv_icrd_bus_lcr_bco |
| COR00906.FRM | buscar_Click | CMXsrv_icrd_busc_plz |
| COR00906.FRM | proximos_Click | CMXsrv_icrd_busc_plz |
| COR00907.FRM | buscar_Click | CMXsrv_icrd_cor_busc_pais |
| COR00907.FRM | proximos_Click | CMXsrv_icrd_cor_busc_pais |
| GRID_BUS.FRM | buscar_Click | CMXsrv_icrd_busc_bco_mtr |
| GRID_BUS.FRM | proximos_Click | CMXsrv_icrd_busc_bco_mtr |

### DDI
| Archivo       | Segmento             | Procedimiento Almacenado |
|--------------|----------------------|--------------------------|
| DDI00101.FRM | aceptar_Click | CMXsrv_iddi_ingmod_ddi |
| DDI00101.FRM | continuar_Click | CMXsrv_iddi_lee_dec |
| DDI00101.FRM | eliminar_Click | CMXsrv_iddi_eli_ddi |
| DDI00101.FRM | fld_ddi_fec_ii_lostfocus | CMXsrv_iddi_lee_inf |
| DDI00101.FRM | fld_ddi_rut_imp_lostfocus | CMXsrv_iddi_lee_cln |
| DDI01001.FRM | Asociar_Click | CMXsrv_iddi_lee_rut |
| DDI01001.FRM | Asociar_Click | CMXsrv_iddi_asoc_ddi |
| DDI01001.FRM | Command2_Click | CMXsrv_iddi_des_ddi |
| DDI01001.FRM | Desasociar_Click | CMXsrv_iddi_lee_rut |
| DDI01001.FRM | Desasociar_Click | CMXsrv_iddi_des_ddi |
| DDI01001.FRM | fld_aux_rut_cli_lostfocus | CMXsrv_iddi_lee_cln |
| DDI01001.FRM | inicio_asoc | CMXsrv_iddi_busc_asoc |
| DDI01001.FRM | inicio_noasoc | CMXsrv_iddi_busc_noasoc |
| DDI01001.FRM | proximo_no_aso_Click | CMXsrv_iddi_busc_noasoc |

### IMPORT
| Archivo       | Segmento             | Procedimiento Almacenado |
|--------------|----------------------|--------------------------|
| BUSCADIR.FRM | buscar_Click | CMXsrv_icrd_lee_dir_cln |
| BUSC_COD.FRM | buscar_click | CMXsrv_icrd_lee_tex_swf |
| BUSC_TXT.FRM | Aceptar_Click | CMXsrv_icrd_lee_cod_txt_swf |
| BUSC_TXT.FRM | buscar_click | CMXsrv_icrd_lee_txt_swf_all |
| BUSC_TXT.FRM | Form_Load | CMXsrv_icrd_lee_ind_esp_ing |
| BUSC_TXT.FRM | llena_arreglo | CMXsrv_icrd_lee_tex_swf |
| BUSC_TXT.FRM | proximo_Click | CMXsrv_icrd_lee_txt_swf_all |
| CONDESP.FRM | Aceptar_Click | CMXCRDsrv_icrd_a_cnd_esp |
| CONDESP.FRM | Form_Load | CMXsrv_icrd_lee_cnd_esp |
| CRD00101.FRM | clon_Click | CMXCRDsrv_icrd_clon_crd |
| CRD00101.FRM | Form_Activate | CMXCRDsrv_icrd_lee_crdcre |
| CRD00101.FRM | Form_Activate | CMXsrv_icrd_lee_ind_esp_ing |
| CRD00101.FRM | Form_Activate | CMXsrv_icrd_lee_top |
| CRD00101.FRM | Form_Load | CMXsrv_grl_fec_serv |
| CRD00101.FRM | Form_Load | CMXsrv_cmx_get_codes |
| CRD00101.FRM | Form_Load | CMXsrv_trae_glo_fec |
| CRD00101.FRM | Mcrdapr_Click | CMXCRDsrv_icrd_val_crd |
| CRD00101.FRM | Mcrdeli_click | CMXCRDsrv_icrd_eli_crd |
| CRD00101.FRM | Mcrdtxtliq_Click | CMXsrv_icrd_lee_dat_trs |
| CRD00101.FRM | Mcrdtxtope_Click | CMXsrv_icrd_dat_liq_ope |
| CRD00101.FRM | msg_swift | CMXsrv_iswf_a_pru |
| CRD00201.FRM | Aceptar_Click | CMXsrv_icrd_a_ctp |
| CRD00201.FRM | FLD_COL_COD_CLI_LostFocus | CMXsrv_icrd_lee_cln |
| CRD00201.FRM | Form_Load | CMXsrv_lee_fpro |
| CRD00202.FRM | Aceptar_Click | CMXsrv_icrd_a_cnd |
| CRD00202.FRM | Aceptar_Click | CMXCRDsrv_icrd_crea_crd |
| CRD00202.FRM | fld_col_fec_vto_LostFocus | CMXsrv_util_det_habil |
| CRD00203.FRM | Form_Activate | CMXsrv_icrd_busc_emb |
| CRD00204.FRM | ELIMINAR_Click | CMXsrv_icrd_eli_emb |
| CRD00204.FRM | Form_Load | CMXsrv_icrd_lee_emb1 |
| CRD00204.FRM | Form_Load | CMXsrv_icrd_lee_emb2 |
| CRD00204.FRM | ingresar_Click | CMXsrv_icrd_a_emb1 |
| CRD00204.FRM | ingresar_Click | CMXsrv_icrd_a_emb2 |
| CRD00204.FRM | VALIDA_EMBARQUE | CMXsrv_icrd_val_emb2 |
| CRD00204.FRM | VALIDA_EMBARQUE | CMXsrv_icrd_val_emb1 |
| CRD00205.FRM | Aceptar_Click | CMXsrv_icrd_act_ref |
| CRD00205.FRM | Form_Load | CMXsrv_icrd_act_ref |
| CRD00205.FRM | Form_Load | CMXsrv_icrd_lee_ref |
| CRD00301.FRM | buscar_click | CMXCRDsrv_icrd_busc_crd |
| CRD00301.FRM | FLD_COL_COD_CLI_LostFocus | CMXsrv_icrd_lee_cln |
| CRD00301.FRM | PROXIMA_Click | CMXCRDsrv_icrd_busc_crd |
| CRD0063.FRM | Aceptar_Click | CMXCRDsrv_icrd_apr_sol |
| CRD0063.FRM | Form_Load | CMXsrv_icrd_lee_crdapr |
| CRD00701.FRM | Aceptar_Click | CMXsrv_icrd_rech_sol |
| DESCMERC.FRM | Aceptar_Click | CMXCRDsrv_icrd_a_desc_merc |
| DESCMERC.FRM | Form_Load | CMXsrv_icrd_lee_desc_merc |
| DOCUMENT.FRM | Aceptar_Click | CMXsrv_icrd_a_otr_doc |
| DOCUMENT.FRM | Form_Load | CMXsrv_icrd_lee_otr_doc |
| GRL00101.FRM | enviar_Click | CMXsrv_iswf_a_pru |

### INFORME
| Archivo       | Segmento             | Procedimiento Almacenado |
|--------------|----------------------|--------------------------|
| ARC00100.FRM | Eliminar_Click | CMXsrv_iarc_eli_arc |
| ARC00100.FRM | Form_Activate | CMXsrv_iarc_busc_arc |
| INFO0101.FRM | Form_Activate | CMXsrv_iinf_lee0_inf |
| INFO0101.FRM | Form_Activate | CMXsrv_iinf_lee_tablas |
| INFO0101.FRM | Form_Activate | CMXsrv_iinf_lee1_inf |
| INFO0101.FRM | Form_Activate | CMXsrv_iinf_lee_cln |
| INFO0101.FRM | Form_Activate | CMXsrv_iinf_lee2_inf |
| INFO0101.FRM | Form_Activate | CMXsrv_iinf_avi_miscb |
| INFO0101.FRM | Maviapr_Click | CMXsrv_iinf_avi_misca |
| INFO0101.FRM | Maviapr_Click | CMXsrv_iinf_avi_miscb |
| INFO0101.FRM | Mavicom_Click | CMXsrv_iinf_avi_misca |
| INFO0101.FRM | Mavicom_Click | CMXsrv_iinf_avi_miscb |
| INFO0101.FRM | Mavicom_Click | CMXsrv_icrd_lee_dat_com |
| INFO0101.FRM | Mavimis1_Click | CMXsrv_iinf_avi_misca |
| INFO0101.FRM | Mavimis1_Click | CMXsrv_iinf_avi_miscb |
| INFO0101.FRM | Mavimis2_Click | CMXsrv_iinf_avi_misca |
| INFO0101.FRM | Mavimis2_Click | CMXsrv_iinf_avi_miscb |
| INFO0101.FRM | Mavirec_Click | CMXsrv_iinf_avi_misca |
| INFO0101.FRM | Mavirec_Click | CMXsrv_iinf_avi_miscb |
| INFO0101.FRM | Mavitib_Click | CMXsrv_iinf_avi_misca |
| INFO0101.FRM | Mavitib_Click | CMXsrv_iinf_avi_miscb |
| INFO0101.FRM | Mavitras_Click | CMXsrv_iinf_avi_misca |
| INFO0101.FRM | Mavitras_Click | CMXsrv_iinf_avi_miscb |
| INFO0101.FRM | Mavitras_Click | CMXsrv_icrd_lee_dat_trs |
| INFO0101.FRM | Minfoeli_click | CMXsrv_iinf_eli_inf |
| INFO0101.FRM | Minforev_Click | CMXsrv_iinf_busc_evi |
| INFO0101.FRM | Minfoval_click | CMXsrv_iinf_val_inf |
| INFO0102.FRM | Aceptar_Click | CMXsrv_iinf_ingmod_inf |
| INFO0102.FRM | Fec_pre | CMXsrv_iinf_lee_fec |
| INFO0102.FRM | fld_aux_glo_cls_com_LostFocus | CMXsrv_iinf_lee_tablas |
| INFO0102.FRM | fld_aux_glo_for_pag1_LostFocus | CMXsrv_iinf_lee_tablas |
| INFO0102.FRM | fld_aux_glo_for_pag2_LostFocus | CMXsrv_iinf_lee_tablas |
| INFO0102.FRM | fld_aux_glo_for_pag3_LostFocus | CMXsrv_iinf_lee_tablas |
| INFO0102.FRM | fld_aux_glo_mon_LostFocus | CMXsrv_iinf_lee_tablas |
| INFO0102.FRM | fld_inf_cls_com_Lostfocus | CMXsrv_iinf_lee_tablas |
| INFO0102.FRM | fld_inf_cod_imp_LostFocus | CMXsrv_iinf_lee_cln |
| INFO0102.FRM | fld_inf_for_pag1_lostfocus | CMXsrv_iinf_lee_tablas |
| INFO0102.FRM | fld_inf_for_pag2_LostFocus | CMXsrv_iinf_lee_tablas |
| INFO0102.FRM | fld_inf_for_pag3_LostFocus | CMXsrv_iinf_lee_tablas |
| INFO0102.FRM | fld_inf_mon_inf_lostfocus | CMXsrv_iinf_lee_tablas |
| INFO0102.FRM | Form_Load | CMXsrv_iinf_lee0_inf |
| INFO0102.FRM | Form_Load | CMXsrv_iinf_lee1_inf |
| INFO0102.FRM | Form_Load | CMXsrv_iinf_lee2_inf |
| INFO0102.FRM | valor_usd | CMXsrv_iinf_lee_usd |
| INFO0103.FRM | Aceptar_Click | CMXsrv_iinf_busc_inf |
| INFO0103.FRM | buscar_Click | CMXsrv_iinf_busc_inf |
| INFO0103.FRM | Fec_pre | CMXsrv_iinf_lee_fec |
| INFO0103.FRM | fld_inf_cod_imp_LostFocus | CMXsrv_iinf_lee_cln |
| INFO0103.FRM | PROXIMA_Click | CMXsrv_iinf_busc_inf |
| INFO0104.FRM | Aceptar_Click | CMXsrv_iinf_act_apr |
| INFO0105.FRM | Form_Activate | CMXsrv_iinf_busc_evi |
| INFO0105.FRM | reversar_Click | CMXsrv_iinf_rev_evi |
| INFO0106.FRM | Form_Load | CMXsrv_iinf_lee_evi |
| INFO0107.FRM | Aceptar_Click | CMXsrv_iinf_act_tib |
| INFO0108.FRM | Aceptar_Click | CMXsrv_iinf_act_rec |
| INFO0109.FRM | Aceptar_Click | CMXsrv_iinf_act_rib |
| INFO0110.FRM | Form_Activate | CMXsrv_iinf_busc_comp |
| INFO0110.FRM | proximos_Click | CMXsrv_iinf_busc_comp |
| INFO0111.FRM | Aceptar_Click | CMXsrv_iinf_ingmod_comp |
| INFO0111.FRM | Fec_pre | CMXsrv_iinf_lee_fec |
| INFO0111.FRM | Form_Activate | CMXsrv_iinf_lee_comp |
| INFO0111.FRM | Form_Activate | CMXsrv_iinf_lee_tablas |
| INFO0112.FRM | aceptar_click | CMXsrv_iinf_lee_bco |
| INFO0112.FRM | buscar_Click | CMXsrv_iinf_busc_bco |
| PREFER.FRM | Form_Load | CMXsrv_grl_fec_serv |

### MOD_ADI
| Archivo       | Segmento             | Procedimiento Almacenado |
|--------------|----------------------|--------------------------|
| CRD00202.FRM | Aceptar_Click | CMXsrv_icrd_a_cnd |
| CRD00202.FRM | busca_bco | CMXsrv_icrd_lee_bco_swf |
| CRD00202.FRM | fld_col_fec_vto_LostFocus | CMXsrv_util_det_habil |
| CRD00202.FRM | Form_Load | CMXMCRDsrv_icrd_lee_mcnd |
| PREFER.FRM | Form_Load | CMXsrv_grl_fec_serv |

### MOD_CBR
| Archivo       | Segmento             | Procedimiento Almacenado |
|--------------|----------------------|--------------------------|
| CBR00201.FRM | fld_cbr_cod_gdo_LostFocus | CMXsrv_icbr_lee_cln |
| CBR00201.FRM | Form_Load | CMXsrv_icbr_lee_ctp |
| CBR00201.FRM | INGRESAR_Click | CMXsrv_icbr_act_ctp |
| CBR00202.FRM | Form_Load | CMXsrv_icbr_lee_trm |
| CBR00202.FRM | INGRESAR_Click | CMXsrv_icbr_act_trm |
| CBR00203.FRM | Form_Load | CMXsrv_icbr_lee_doc |
| CBR00203.FRM | INGRESAR_Click | CMXsrv_icbr_act_doc |
| CBR00301.FRM | Form_Activate | CMXsrv_icbr_busc_let |
| CBR00302.FRM | aceptar_Click | CMXsrv_icbr_mod_ing_let |
| CBR00302.FRM | eliminar_Click | CMXsrv_icbr_eli_let |
| CBR00302.FRM | Form_Activate | CMXsrv_icbr_lee_let |
| PANBASE.FRM | actualizar_Click | CMXsrv_icbr_acep_mod_cbr |
| PANBASE.FRM | Cancelar_Click | CMXsrv_icbr_eli_no_cont |

### MOD_CRD
| Archivo       | Segmento             | Procedimiento Almacenado |
|--------------|----------------------|--------------------------|
| BCO_BCO.FRM | Aceptar_Click | CMXsrv_icrd_a_ibab |
| BCO_BCO.FRM | Form_Load | CMXsrv_icrd_lee_glo_ibab |
| BCO_REM.FRM | Aceptar_Click | CMXsrv_icrd_a_ibar |
| BCO_REM.FRM | Form_Load | CMXsrv_icrd_lee_glo_ibar |
| BUSCADIR.FRM | buscar_click | CMXsrv_icrd_lee_dir_cln |
| BUSCA_TE.FRM | buscar_Click | CMXsrv_icrd_lee_tex_swf |
| BUSC_COD.FRM | buscar_click | CMXsrv_icrd_lee_tex_swf |
| BUSC_TXT.FRM | Aceptar_Click | CMXsrv_icrd_lee_cod_txt_swf |
| BUSC_TXT.FRM | buscar_click | CMXsrv_icrd_lee_txt_swf_all |
| BUSC_TXT.FRM | Form_Load | CMXsrv_icrd_lee_ind_esp_ing |
| BUSC_TXT.FRM | llena_arreglo | CMXsrv_icrd_lee_tex_swf |
| BUSC_TXT.FRM | proximo_Click | CMXsrv_icrd_lee_txt_swf_all |
| CONDESP.FRM | Aceptar_Click | CMXMCRDsrv_icrd_a_mmcnd |
| CONDESP.FRM | Form_Load | CMXsrv_icrd_lee_cnd_esp |
| CRD00201.FRM | Aceptar_Click | CMXsrv_icrd_a_ctp |
| CRD00201.FRM | FLD_COL_COD_CLI_LostFocus | CMXsrv_icrd_lee_cln |
| CRD00201.FRM | Form_Load | CMXMCRDsrv_icrd_lee_mctp |
| CRD00202.FRM | Aceptar_Click | CMXsrv_icrd_a_cnd |
| CRD00202.FRM | Form_Load | CMXMCRDsrv_icrd_lee_mcnd |
| CRD00203.FRM | Form_Activate | CMXsrv_icrd_busc_emb |
| CRD00204.FRM | cancelar_Click | CMXsrv_icrd_lee_desc_merc |
| CRD00204.FRM | ELIMINAR_Click | CMXsrv_icrd_eli_emb |
| CRD00204.FRM | Form_Load | CMXMCRDsrv_icrd_lee_memb2 |
| CRD00204.FRM | Form_Load | CMXMCRDsrv_icrd_lee_memb1 |
| CRD00204.FRM | ingresar_Click | CMXsrv_icrd_a_emb1 |
| CRD00204.FRM | ingresar_Click | CMXsrv_icrd_a_emb2 |
| CRD00204.FRM | VALIDA_EMBARQUE | CMXsrv_icrd_val_emb2 |
| CRD00204.FRM | VALIDA_EMBARQUE | CMXsrv_icrd_val_emb1 |
| CRD00205.FRM | Aceptar_Click | CMXsrv_icrd_act_ref |
| CRD00205.FRM | fld_obl_cod_bco_acre_DblClick | CMXsrv_icrd_lee_bco_swf |
| CRD00205.FRM | fld_obl_cod_bco_acre_LostFocus | CMXsrv_icrd_lee_bco_swf |
| CRD00205.FRM | Form_Load | CMXMCRDsrv_icrd_lee_mref |
| CRD00206.FRM | Aceptar_Click | CMXsrv_icrd_ing_txt |
| CRD00206.FRM | Form_Load | CMXCRDsrv_icrd_get_ing_esp |
| CRD00206.FRM | Form_Load | CMXMCRDsrv_icrd_lee_mtxt |
| CRD00207.FRM | Form_Load | CMXCRDsrv_icrd_get_pre_fra |
| DESCMERC.FRM | Aceptar_Click | CMXMCRDsrv_icrd_a_mmer |
| DESCMERC.FRM | Form_Load | CMXsrv_icrd_lee_desc_merc |
| DOCUME.FRM | Aceptar_Click | CMXsrv_icrd_a_otr_doc |
| DOCUME.FRM | Form_Load | CMXsrv_icrd_lee_otr_doc |
| MOD00603.FRM | Aceptar_Click | CMXsrv_fincol_lee_cod_eve |
| MOD00603.FRM | Aceptar_Click | CMXMCRDsrv_icrd_acep_mod_crd |
| MOD00603.FRM | cancelar_Click | CMXMCRDsrv_icrd_eli_no_cont |
| MOD00603.FRM | fld_crd_cod_bco_rem_LostFocus | CMXsrv_icrd_lee_bco_swf |
| MOD00603.FRM | fld_crd_fec_mod_lostFocus | CMXsrv_fincol_efec_calpa |
| MOD00603.FRM | Form_Activate | CMXsrv_icrd_lee_ind_esp_ing |
| MOD00603.FRM | Form_Load | CMXsrv_fincol_efec_calpa |
| MOD00603.FRM | Form_Load | CMXMCRDsrv_icrd_lee_mcnd |
| PREFER.FRM | Form_Load | CMXsrv_grl_fec_serv |

### NEGO_AV
| Archivo       | Segmento             | Procedimiento Almacenado |
|--------------|----------------------|--------------------------|
| AVISOS.FRM | aviso1 | CMXsrv_icrd_a_rec_age |
| AVISOS.FRM | aviso1 | CMXsrv_busc_ofi_cta |
| AVISOS.FRM | aviso1 | CMXsrv_neg_busc_arc |
| AVISOS.FRM | aviso1 | CMXsrv_icrd_lee_avi_adi |
| AVISOS.FRM | aviso3 | CMXsrv_icrd_lee_dat_trs |
| AVISOS.FRM | Aviso4 | CMXsrv_icrd_dat_liq_ope |
| AVISOS.FRM | Aviso4 | CMXsrv_icrd_lee_dat_cln |
| AVISOS.FRM | Aviso5 | CMXsrv_icrd_lee_dat_cln |
| AVISOS.FRM | Aviso5 | CMXsrv_icrd_lee_avi_dis |
| AVISOS.FRM | Aviso5 | CMXsrv_icrd_lee_avi_adi |
| AVISOS.FRM | Aviso5 | CMXsrv_neg_ddi_asoc |
| AVISOS.FRM | Aviso5 | CMXsrv_neg_busc_arc |
| AVISOS.FRM | Aviso5 | CMXsrv_neg_trae_vcto_mcf |
| AVISOS.FRM | Aviso6 | CMXsrv_icrd_avs_cyg1 |
| AVISOS.FRM | Aviso6 | CMXsrv_icrd_avs_cyg2 |
| AVISOS.FRM | lee_aval | CMXsrv_neg_avi_lee_aval |
| AVISOS.FRM | lee_nego | CMXsrv_icrd_neg_lee_crd |
| AVISOS.FRM | lee_nego | CMXsrv_icrd_lee_neg |
| AVI_COL.FRM | avi_col1 | CMXsrv_col_avi_dat_cln |
| AVI_COL.FRM | avi_col1 | CMXsrv_col_avi_det_pag |
| AVI_COL.FRM | avi_col2 | CMXsrv_col_avi_dat_cln |
| AVI_COL.FRM | avi_col2 | CMXsrv_col_avi_det_oto |
| AVI_COL.FRM | avi_col4 | CMXsrv_col_avi_dat_cln |
| AVI_COL.FRM | avi_col4 | CMXsrv_col_lee_num_trs |
| AVI_COL.FRM | lee_obl_oto | CMXsrv_finobl_avi_oto |
| AVI_COL.FRM | lee_obl_pag | CMXsrv_finobl_avi_pag |
| AVI_COL.FRM | traspaso | CMXsrv_neg_avi_trae_asnd_mn |
| AVI_COL.FRM | traspaso | CMXsrv_neg_avi_trae_asnd_mx |
| CRD01001.FRM | Form_Activate | CMXsrv_icrd_neg_lee_crd |
| CRD01001.FRM | Form_Activate | CMXsrv_icrd_lee_neg |
| CRD01001.FRM | Mcrdtxtliq_Click | CMXsrv_icrd_lee_dat_trs |
| CRD01001.FRM | Mcrdtxtope_Click | CMXsrv_icrd_dat_liq_ope |
| CRD01001.FRM | Mnegavi3_Click | CMXsrv_icrd_avs_cyg1 |
| CRD01001.FRM | Mnegavi3_Click | CMXsrv_icrd_avs_cyg2 |
| CRD01001.FRM | Mnegavi4_Click | CMXsrv_icrd_lee_dat_liq |
| CRD01001.FRM | MNEGCONT_Click | CMXsrv_icrd_cont_neg |
| CRD01001.FRM | MNEGELI_CLICK | CMXsrv_icrd_eli_neg |
| CRD01001.FRM | precarga_datos | CMXsrv_icrd_a_rec_age |
| CRD01001.FRM | precarga_datos | CMXsrv_busc_ofi_cta |
| PREFER.FRM | Form_Load | CMXsrv_trae_glo_fec |
| PREFER.FRM | Form_Load | CMXsrv_icrd_lee_num_col |
| VER_PAGO.FRM | Form_Load | CMXsrv_icrd_bus_pago |

### NNEGO
| Archivo       | Segmento             | Procedimiento Almacenado |
|--------------|----------------------|--------------------------|
| CRD01001.FRM | Form_Activate | CMXsrv_icrd_neg_lee_crd |
| CRD01001.FRM | Form_Activate | CMXsrv_icrd_lee_neg |
| CRD01001.FRM | gen_mens_swift | CMXsrv_iswf_a_pru |
| CRD01001.FRM | llama_pagos | CMXsrv_icrd_lee_col |
| CRD01001.FRM | Mnegavi9_Click | CMXsrv_iswf_a_pru |
| CRD01001.FRM | MNEGCONT_Click | CMXsrv_icrd_cont_neg |
| CRD01001.FRM | MNEGELI_CLICK | CMXsrv_icrd_eli_neg |
| CRD01001.FRM | pertas_Click | CMXsrv_icrd_lee_col |
| CRD01001.FRM | prueba_Click | CMX2srv_neg_avi_dat_cln |
| CRD01001.FRM | prueba_Click | CMX2srv_neg_avi_det_int |
| CRD01001.FRM | prueba_Click | CMX2srv_neg_avi_trae_asnd_mn |
| CRD01001.FRM | prueba_Click | CMX2srv_neg_avi_trae_asnd_mx |
| CRD01001.FRM | prueba_pag_Click | CMX2srv_neg_avi_dat_cln |
| CRD01001.FRM | prueba_pag_Click | CMX2srv_neg_avi_det_pag |
| CRD01001.FRM | prueba_pag_Click | CMX2srv_neg_avi_trae_asnd_mn |
| CRD01001.FRM | prueba_pag_Click | CMX2srv_neg_avi_trae_asnd_mx |
| CRD01002.FRM | Form_Activate | CMXsrv_icrd_busc_neg |
| CRD01003.FRM | Form_Load | CMXsrv_icrd_busc_emb |
| CRD01005.FRM | ACEPTAR_Click | CMXsrv_icrd_a_neg_emb1 |
| CRD01005.FRM | ACEPTAR_Click | CMXsrv_icrd_a_neg_emb2 |
| CRD01005.FRM | CANCELAR_Click | CMXsrv_icrd_eli_doc_neg |
| CRD01005.FRM | Form_Activate | CMXsrv_icrd_lee_emb1 |
| CRD01005.FRM | Form_Activate | CMXsrv_icrd_lee_emb2 |
| CRD01005.FRM | Form_Activate | CMXsrv_icrd_lee_neg_emb1 |
| CRD01005.FRM | Form_Activate | CMXsrv_icrd_lee_neg_emb2 |
| CRD01005.FRM | Form_Activate | CMXsrv_icrd_lee_cnd_esp |
| CRD01005.FRM | Form_Activate | CMXsrv_icrd_lee_desc_merc |
| CRD01006.FRM | ACEPTAR_Click | CMXsrv_icrd_a_neg_disc |
| CRD01006.FRM | Form_Load | CMXsrv_icrd_neg_lee_disc |
| CRD01201.FRM | ACEPTAR_Click | CMXsrv_icrd_ent_doc |
| CRD01201.FRM | ELIMINAR_Click | CMXsrv_icrd_ent_doc |
| CRD01201.FRM | Form_Load | CMXsrv_icrd_ent_doc |
| CRD01301.FRM | ACEPTAR_Click | MIGRCMXsrv_neg_grb_ind_com_disc |
| CRD01301.FRM | ACEPTAR_Click | CMXsrv_con_convenio_banco |
| CRD01301.FRM | ACEPTAR_Click | CMXsrv_icrd_alz_disc |
| CRD02001.FRM | aceptar_click | CMXCRDsrv_icrd_asignar_cor |
| CRD02001.FRM | BUSCAR_Click | CMXCRDsrv_icrd_bus_lcr_bco |
| CRD02001.FRM | proximo_Click | CMXCRDsrv_icrd_bus_lcr_bco |
| CRD02004.FRM | ACEPTAR_Click | CMXsrv_icrd_act_doc_neg |
| CRD02004.FRM | Form_Load | CMXsrv_icrd_lee_doc_neg |
| GRL00101.FRM | enviar_Click | CMXsrv_iswf_a_pru |
| GRL00101.FRM | Form_Load | CMXsrv_icrd_val_neg |
| PREFER.FRM | Form_Load | CMXsrv_grl_fec_serv |
| VER_PAGO.FRM | Form_Load | CMXsrv_icrd_bus_pago |

### PAGCBR
| Archivo       | Segmento             | Procedimiento Almacenado |
|--------------|----------------------|--------------------------|
| CBR01005.FRM | Aceptar_Click | CMXsrv_icbr_calc_pag |
| CBR01006.FRM | ACEPTAR_Click | CMXsrv_icbr_lee_dat_var |
| CBR01006.FRM | ACEPTAR_Click | CMXsrv_icbr_val_pag |
| CBR01006.FRM | ACEPTAR_Click | CMXsrv_icbr_ctb_pag |
| CBR01006.FRM | Calcular_Click | CMXsrv_icbr_cal_pag |
| CBR01006.FRM | CANCELAR_Click | CMXsrv_icbr_eli_pag |
| CBR01006.FRM | fld_cbr_cod_des_mn_pag_lostfocus | CMXsrv_val_vig |
| CBR01006.FRM | fld_cbr_cod_des_mx_pag_lostfocus | CMXsrv_val_vig |
| CBR01006.FRM | Form_Load | CMXsrv_icbr_lee_cbr0 |
| CBR01006.FRM | Form_Load | CMXsrv_icbr_obt_mon_nac |
| CBR01006.FRM | Form_Load | CMXsrv_icbr_lee_dat_pag |
| CBR01006.FRM | Form_Load | CMXsrv_icbr_pcg_pag |
| CBR01006.FRM | lee_cta | CMXsrv_vig_lee_cta |
| CBR01007.FRM | Form_Activate | CMXsrv_icbr_busc_pago |
| CBR01008.FRM | ACEPTAR_Click | CMXsrv_icbr_val_pag |
| COB00303.FRM | Aceptar_Click | CMXsrv_icob_act_val |
| COB00303.FRM | Form_Activate | CMXsrv_icob_lee_val |
| COB00305.FRM | ELIMINAR_Click | CMXsrv_icbr_eli_int_pago |
| COB00305.FRM | Form_Activate | CMXsrv_icbr_busc_int |
| COB00306.FRM | Aceptar_Click | CMXsrv_icbr_ingmod_int |
| COB00306.FRM | Form_Activate | CMXsrv_icbr_lee_int_pago |
| CRD00602.FRM | Aceptar_Click | CMXsrv_icbr_lee_bco |
| CRD00602.FRM | buscar_Click | CMXsrv_icbr_busc_bco |
| PREFER.FRM | Form_Load | CMXsrv_grl_fec_serv |

