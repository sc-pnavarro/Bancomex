
# Índice de Módulos

- [ADMIN](#admin)
- [ARCOS](#arcos)
- [COBERIMP](#coberimp)
- [COBRANZA](#cobranza)
- [COL_NEG](#col_neg)
- [CRDEXT](#crdext)
- [CRD_CORR](#crd_corr)
- [DDI](#ddi)
- [EXPCBE](#expcbe)
- [EXPCCE](#expcce)
- [EXPNEG](#expneg)
- [IMPORT](#import)
- [INFORME](#informe)
- [INGRESO](#ingreso)
- [MODIFIC](#modific)
- [MOD_ADI](#mod_adi)
- [MOD_CBR](#mod_cbr)
- [MOD_CRD](#mod_crd)
- [NEGO_AV](#nego_av)
- [NNEGO](#nnego)
- [OBLIGA](#obliga)
- [PAGCBR](#pagcbr)
- [PAGOS](#pagos)
- [PGOEXT](#pgoext)
- [expdex](#expdex)
- [expret](#expret)

# Detalle de Módulos

## ADMIN
| Segmento | Procedimiento Almacenado | Tablas Referenciadas | Procedimientos Referenciados |
|----------|--------------------------|----------------------|--------------------------|
| COMMAND4_Click | CMXsrv_finadm_imod_desti | N/A | N/A |
| Form_Load | CMXsrv_finadm_cons_dtip | N/A | N/A |
| Command1_Click | CMXsrv_finadm_imod_ectb | N/A | N/A |
| Command2_Click | CMXsrv_finadm_eli_tipop | N/A | N/A |
| Form_Load | CMXsrv_finadm_cons_ectb | N/A | N/A |
| COMMAND3_Click | CMXsrv_finadm_eli_tipop | N/A | N/A |
| COMMAND4_Click | CMXsrv_finadm_imod_itip | N/A | N/A |
| Form_Load | CMXsrv_finadm_cons_itip | N/A | N/A |
| Form_Activate | CMXsrv_finadm_lee_tipop | N/A | N/A |
| Form_Load | CMXsrv_grl_fec_serv | N/A | N/A |
| Mdel_Click | CMXsrv_finadm_eli_tipop | N/A | N/A |
| Mval_Click | CMXsrv_finadm_val_tipop | N/A | N/A |
| buscar_Click | CMXsrv_finadm_bus_tipope | N/A | N/A |
| proximas_Click | CMXsrv_finadm_bus_tipope | N/A | N/A |

## ARCOS
| Segmento | Procedimiento Almacenado | Tablas Referenciadas | Procedimientos Referenciados |
|----------|--------------------------|----------------------|--------------------------|
| Eliminar_Click | CMXsrv_iarc_eli_arc | N/A | N/A |
| Form_activate | CMXsrv_iarc_busc_arc | N/A | N/A |
| aceptar_click | CMXsrv_iinf_busc_inf | N/A | N/A |
| aceptar_click | CMXsrv_iarc_act_arc | N/A | N/A |
| Form_Load | CMXsrv_iarc_lee_arc | N/A | N/A |
| buscar_Click | CMXsrv_iinf_busc_opr | N/A | N/A |
| Form_activate | CMXsrv_iinf_lee_vlr | N/A | N/A |
| aceptar_click | CMXsrv_iarc_act_arc | N/A | N/A |
| Form_activate | CMXsrv_iinf_busc_inf | N/A | N/A |
| reversar_Click | CMXsrv_iinf_rev_evi | N/A | N/A |

## COBERIMP
| Segmento | Procedimiento Almacenado | Tablas Referenciadas | Procedimientos Referenciados |
|----------|--------------------------|----------------------|--------------------------|
| Form_Activate | CMXsrv_icob_lee_pln | N/A | N/A |
| Mcobcur_Click | CMXsrv_icob_cur_cob | N/A | N/A |
| Mcobcur_Click | CMXsrv_icob_pag_sop | N/A | N/A |
| MCOBELI_CLICK | CMXsrv_icob_eli_pln | N/A | N/A |
| Mcobrev_Click | CMXsrv_icob_rev_etd | N/A | N/A |
| Mcobvali_Click | CMXsrv_icob_val_cob | N/A | N/A |
| buscar_click | CMXsrv_icob_busc_pln | N/A | N/A |
| FLD_COB_COD_CLI_LostFocus | CMXsrv_icob_lee_cln | N/A | N/A |
| PROXIMAS_Click | CMXsrv_icob_busc_pln | N/A | N/A |
| ACEPTAR_Click | CMXsrv_icob_crea_norm | N/A | N/A |
| ACEPTAR_Click | CMXsrv_icob_crea_reem | N/A | N/A |
| ACEPTAR_Click | CMXsrv_icob_act_gral | N/A | N/A |
| FLD_COB_COD_CLI_LostFocus | CMXsrv_icob_lee_cln2 | N/A | N/A |
| Form_Activate | CMXsrv_icob_lee_gral | N/A | N/A |
| ACEPTAR_Click | CMXsrv_icob_act_val | N/A | N/A |
| Form_Activate | CMXsrv_icob_lee_val | N/A | N/A |
| ACEPTAR_Click | CMXsrv_icob_act_acu | N/A | N/A |
| Form_Activate | CMXsrv_icob_lee_acu | N/A | N/A |
| Form_Load | CMXsrv_icob_lee_acu | N/A | N/A |
| ELIMINAR_Click | CMXsrv_icob_eli_int | N/A | N/A |
| Form_Activate | CMXsrv_icob_busc_int | N/A | N/A |
| ACEPTAR_Click | CMXsrv_icob_ingmod_int | N/A | N/A |
| Form_Activate | CMXsrv_icob_lee_int | N/A | N/A |
| ACEPTAR_Click | CMXsrv_icob_ing_mod_srf | N/A | N/A |
| CmdEliminar_Click | CMXsrv_icob_eli_pln | N/A | N/A |
| CmdReversar_Click | CMXsrv_icob_rev_etd | N/A | N/A |
| CURSAR_Click | CMXsrv_icob_ing_mod_srf | N/A | N/A |
| CURSAR_Click | CMXsrv_icob_pag_sop | N/A | N/A |
| FLD_COB_COD_CLI_LostFocus | CMXsrv_icob_lee_cln2 | N/A | N/A |
| Form_Activate | CMXsrv_icob_lee_srf | N/A | N/A |
| Reversar_Click | CMXsrv_icob_rev_etd | N/A | N/A |
| ACEPTAR_Click | CMXsrv_icob_anu | N/A | N/A |
| Form_Load | CMXsrv_icob_lee_anu | N/A | N/A |
| ACEPTAR_Click | CMXsrv_icob_act_cur_a_pag | N/A | N/A |
| buscar_click | CMXsrv_icob_bus_cur_a_pag | N/A | N/A |
| FLD_COB_COD_CLI_LostFocus | CMXsrv_icob_lee_cln | N/A | N/A |
| ACEPTAR_Click | CMXsrv_icob_pag_sop | N/A | N/A |
| ACEPTAR_Click | CMXsrv_icob_cur_reem | N/A | N/A |
| Form_Load | CMXsrv_grl_fec_serv | N/A | N/A |

## COBRANZA
| Segmento | Procedimiento Almacenado | Tablas Referenciadas | Procedimientos Referenciados |
|----------|--------------------------|----------------------|--------------------------|
| ejecut_avi_imp_999 | CMXsrv_busc_cor_swf | N/A | N/A |
| ejecut_avi_imp_999 | CMXsrv_swf_bus_sms | N/A | N/A |
| Form_Activate | CMXsrv_icbr_lee_cbr | N/A | N/A |
| Form_Load | CMXsrv_grl_fec_serv | N/A | N/A |
| Mcbrace_Click | CMXsrv_icbr_acep_let | N/A | N/A |
| Mcbrcon_Click | CMXsrv_icbr_cont_cbr | N/A | N/A |
| Mcbreli_click | CMXsrv_icbr_eli_cbr | N/A | N/A |
| McbrTxt999_Click | CMXsrv_icbr_lee_ctp | N/A | N/A |
| Mcbrtxtrec_Click | CMXsrv_icbr_avi1 | N/A | N/A |
| aceptar_Click | CMXsrv_val_suc | N/A | N/A |
| buscar_Click | CMXsrv_icbr_busc_cbr | N/A | N/A |
| fld_aux_glo_ofi_LostFocus | CMXsrv_val_suc | N/A | N/A |
| fld_cbr_cod_gdo_LostFocus | CMXsrv_icbr_lee_cln | N/A | N/A |
| fld_cbr_cod_ofi_lostfocus | CMXsrv_val_suc | N/A | N/A |
| proximas_Click | CMXsrv_icbr_busc_cbr | N/A | N/A |
| crear_Click | CMXsrv_icbr_crea_cbr | N/A | N/A |
| fld_cbr_cod_gdo_LostFocus | CMXsrv_icbr_lee_cln | N/A | N/A |
| fld_cbr_cod_ofi_lostfocus | CMXsrv_val_suc | N/A | N/A |
| INGRESAR_Click | CMXsrv_icbr_crea_cbr | N/A | N/A |
| fld_cbr_cod_gdo_LostFocus | CMXsrv_icbr_lee_cln | N/A | N/A |
| Form_Activate | CMXsrv_icbr_lee_cob | N/A | N/A |
| Form_Load | CMXsrv_icbr_lee_ctp | N/A | N/A |
| INGRESAR_Click | CMXsrv_icbr_act_ctp | N/A | N/A |
| Form_Activate | CMXsrv_icbr_lee_cob | N/A | N/A |
| Form_Load | CMXsrv_icbr_lee_trm | N/A | N/A |
| INGRESAR_Click | CMXsrv_icbr_act_trm | N/A | N/A |
| Form_Activate | CMXsrv_icbr_lee_cob | N/A | N/A |
| Form_Load | CMXsrv_icbr_lee_doc | N/A | N/A |
| INGRESAR_Click | CMXsrv_icbr_act_doc | N/A | N/A |
| Form_Activate | CMXsrv_icbr_busc_let | N/A | N/A |
| aceptar_Click | CMXsrv_icbr_ingmod_let | N/A | N/A |
| eliminar_Click | CMXsrv_icbr_eli_let | N/A | N/A |
| Form_Activate | CMXsrv_icbr_lee_let | N/A | N/A |
| aceptar_Click | CMXsrv_icbr_prorr | N/A | N/A |
| EFECTUAR_Click | CMXsrv_icbr_rev_eve | N/A | N/A |
| Form_Activate | CMXsrv_icbr_busc_eve | N/A | N/A |
| Form_Load | CMXsrv_icbr_lee_eve | N/A | N/A |
| Form_Load | CMXsrv_icbr_lee_ent_doc | N/A | N/A |
| aceptar_Click | CMXsrv_icbr_prot | N/A | N/A |
| Form_Load | CMXsrv_icbr_pcg_prot | N/A | N/A |
| aceptar_Click | CMXsrv_icbr_liq_sdo | N/A | N/A |
| aceptar_Click | CMXsrv_icbr_act_vis | N/A | N/A |
| eliminar_Click | CMXsrv_icbr_eli_rep | N/A | N/A |
| Form_Activate | CMXsrv_icbr_busc_rep | N/A | N/A |
| aceptar_Click | CMXsrv_icbr_imod_rep | N/A | N/A |
| aceptar_Click | CMXsrv_icbr_ent_doc | N/A | N/A |
| Form_Load | CMXsrv_icbr_lee_ent_doc | N/A | N/A |
| aceptar_Click | CMXsrv_icbr_trf_ofi | N/A | N/A |
| aceptar_Click | CMXsrv_val_suc | N/A | N/A |
| aceptar_Click | CMXsrv_icbr_trf_bco | N/A | N/A |
| aceptar_Click | CMXsrv_icbr_act_inst | N/A | N/A |
| enviar_Click | CMXsrv_iswf_a_pru | N/A | N/A |
| Form_Load | CMXsrv_icbr_val_cbr | N/A | N/A |
| word_Click | CMXsrv_icbr_val_cbr | N/A | N/A |
| word_Click | CMXsrv_iswf_a_pru | N/A | N/A |

## COL_NEG
| Segmento | Procedimiento Almacenado | Tablas Referenciadas | Procedimientos Referenciados |
|----------|--------------------------|----------------------|--------------------------|
| CANCELAR_Click | CMXsrv_busc_tip_tas | N/A | N/A |
| ELIMINAR_Click | CMXsrv_fincol_ecuo | N/A | N/A |
| Form_Activate | CMXsrv_fincol_cons_plnpa | N/A | N/A |
| Form_Load | CMXsrv_pertas_val_display | N/A | N/A |
| ELIMINAR_Click | CMXsrv_fincol_eava | N/A | N/A |
| Form_Activate | CMXsrv_fincol_cons_aval | N/A | N/A |
| ingresar_Click | CMXsrv_fincol_iava | N/A | N/A |
| CONTABILIZAR_Click | CMXsrv_fincol_ictb_pag | N/A | N/A |
| aviso_Click | CMXsrv_fincol_avi_2_fin | N/A | N/A |
| Form_Activate | CMXsrv_fincol_cons_pag | N/A | N/A |
| proximos_Click | CMXsrv_fincol_cons_pag | N/A | N/A |
| Form_Activate | CMXsrv_fincol_trae_det_pag | N/A | N/A |
| aviso_Click | CMXsrv_fincol_avi_3_fin | N/A | N/A |
| Form_Activate | CMXsrv_fincol_cons_pror | N/A | N/A |
| EFECTUAR_Click | CMXsrv_fincol_rev_eve | N/A | N/A |
| Form_Activate | CMXsrv_fincol_cons_eve | N/A | N/A |
| Aceptar_Click | CMXsrv_icrd_lee_bco_swf | N/A | N/A |
| buscar_Click | CMXsrv_icrd_busc_bco | N/A | N/A |
| proximo_Click | CMXsrv_icrd_busc_bco | N/A | N/A |
| Aceptar_Click | CMXsrv_fincol_vtocre_prov | N/A | N/A |
| Form_Load | CMXsrv_fincol_prec_vtocre | N/A | N/A |
| buscar_Click | CMXsrv_icrd_bus_lcr_bco | N/A | N/A |
| proximo_Click | CMXsrv_icrd_bus_lcr_bco | N/A | N/A |
| Form_Load | CMXsrv_grl_fec_serv | N/A | N/A |
| Form_Load | CMXsrv_lee_fpro | N/A | N/A |

## CRDEXT
| Segmento | Procedimiento Almacenado | Tablas Referenciadas | Procedimientos Referenciados |
|----------|--------------------------|----------------------|--------------------------|
| Aceptar_Click | CMXsrv_icrd_a_ibab | N/A | N/A |
| Form_Load | CMXsrv_icrd_lee_glo_ibab | N/A | N/A |
| Aceptar_Click | CMXsrv_icrd_a_ibar | N/A | N/A |
| Form_Load | CMXsrv_icrd_lee_glo_ibar | N/A | N/A |
| buscar_click | CMXsrv_icrd_lee_tex_swf | N/A | N/A |
| Aceptar_Click | CMXsrv_icrd_lee_cod_txt_swf | N/A | N/A |
| buscar_click | CMXsrv_icrd_lee_txt_swf_all | N/A | N/A |
| Form_Load | CMXsrv_icrd_lee_ind_esp_ing | N/A | N/A |
| llena_arreglo | CMXsrv_icrd_lee_tex_swf | N/A | N/A |
| proximo_Click | CMXsrv_icrd_lee_txt_swf_all | N/A | N/A |
| aceptar_Click | CMXsrv_icrd_ing_acu | N/A | N/A |
| Form_Load | CMXsrv_icrd_lee_acu | N/A | N/A |
| aceptar_Click | CMXsrv_icrd_rech_sol | N/A | N/A |
| aceptar_Click | CMXsrv_icrd_end | N/A | N/A |
| Form_Load | CMXsrv_icrd_lee_dat_end | N/A | N/A |
| aceptar_Click | CMXsrv_icrd_asignar_cor | N/A | N/A |
| buscar_Click | CMXsrv_icrd_bus_lcr_bco | N/A | N/A |
| proximo_Click | CMXsrv_icrd_bus_lcr_bco | N/A | N/A |
| Form_Load | CMXsrv_grl_fec_serv | N/A | N/A |

## CRD_CORR
| Segmento | Procedimiento Almacenado | Tablas Referenciadas | Procedimientos Referenciados |
|----------|--------------------------|----------------------|--------------------------|
| aceptar_Click | CMXsrv_icrd_asignar_cor | N/A | N/A |
| buscar_Click | CMXsrv_icrd_bus_lcr_bco | N/A | N/A |
| fld_cor_cod_mtr_LostFocus | CMXsrv_icrd_lee_bco_mtr | N/A | N/A |
| fld_cor_cod_pais_Lostfocus | CMXsrv_icrd_cor_lee_pais | N/A | N/A |
| fld_cor_cod_plz_Lostfocus | CMXsrv_icrd_lee_plz | N/A | N/A |
| proximo_Click | CMXsrv_icrd_bus_lcr_bco | N/A | N/A |
| buscar_Click | CMXsrv_icrd_busc_plz | N/A | N/A |
| proximos_Click | CMXsrv_icrd_busc_plz | N/A | N/A |
| buscar_Click | CMXsrv_icrd_cor_busc_pais | N/A | N/A |
| proximos_Click | CMXsrv_icrd_cor_busc_pais | N/A | N/A |
| buscar_Click | CMXsrv_icrd_busc_bco_mtr | N/A | N/A |
| proximos_Click | CMXsrv_icrd_busc_bco_mtr | N/A | N/A |

## DDI
| Segmento | Procedimiento Almacenado | Tablas Referenciadas | Procedimientos Referenciados |
|----------|--------------------------|----------------------|--------------------------|
| aceptar_Click | CMXsrv_iddi_ingmod_ddi | N/A | N/A |
| continuar_Click | CMXsrv_iddi_lee_dec | N/A | N/A |
| eliminar_Click | CMXsrv_iddi_eli_ddi | N/A | N/A |
| fld_ddi_fec_ii_lostfocus | CMXsrv_iddi_lee_inf | N/A | N/A |
| fld_ddi_rut_imp_lostfocus | CMXsrv_iddi_lee_cln | N/A | N/A |
| Asociar_Click | CMXsrv_iddi_lee_rut | N/A | N/A |
| Asociar_Click | CMXsrv_iddi_asoc_ddi | N/A | N/A |
| Command2_Click | CMXsrv_iddi_des_ddi | N/A | N/A |
| Desasociar_Click | CMXsrv_iddi_lee_rut | N/A | N/A |
| Desasociar_Click | CMXsrv_iddi_des_ddi | N/A | N/A |
| fld_aux_rut_cli_lostfocus | CMXsrv_iddi_lee_cln | N/A | N/A |
| inicio_asoc | CMXsrv_iddi_busc_asoc | N/A | N/A |
| inicio_noasoc | CMXsrv_iddi_busc_noasoc | N/A | N/A |
| proximo_no_aso_Click | CMXsrv_iddi_busc_noasoc | N/A | N/A |

## EXPCBE
| Segmento | Procedimiento Almacenado | Tablas Referenciadas | Procedimientos Referenciados |
|----------|--------------------------|----------------------|--------------------------|
| Form_Activate | CMXsrv_expcbe_lee_prm | N/A | N/A |
| Form_Activate | CMXsrv_cmx_busc_suc_usu | N/A | N/A |
| Form_Activate | CMXsrv_expcbe_lee_cbe | N/A | N/A |
| Form_Load | CMXsrv_trae_glo_fec | N/A | N/A |
| ingcomg_Click | CMXsrv_expcbe_avs_cyg1 | N/A | N/A |
| ingcomg_Click | CMXsrv_expcbe_avs_cyg2 | N/A | N/A |
| ingret_Click | CMXsrv_expcbe_avs_ret | N/A | N/A |
| M3_Click | CMXsrv_expcbe_swf_sel | N/A | N/A |
| M4_Click | CMXsrv_expcbe_swf_sel | N/A | N/A |
| Mcbeanl_Click | CMXsrv_expcbe_anl_cbe | N/A | N/A |
| Mcbectb_Click | CMXsrv_expcbe_ctb_ing | N/A | N/A |
| Mcbedel_Click | CMXsrv_expcbe_del_cbe | N/A | N/A |
| Mcbeval_Click | CMXsrv_expcbe_val_cbe | N/A | N/A |
| Men1_Click | CMXsrv_expcbe_swf_sel | N/A | N/A |
| aceptar_Click | CMXsrv_expcbe_grb_ctp | N/A | N/A |
| fld_cbe_cod_exp_lostfocus | CMXsrv_expcbe_lee_cln | N/A | N/A |
| fld_cbe_cod_suc_LostFocus | CMXsrv_val_suc | N/A | N/A |
| Form_Activate | CMXsrv_expcbe_lee_ctp | N/A | N/A |
| aceptar_Click | CMXsrv_expcbe_grb_bco | N/A | N/A |
| fld_cbe_cod_cob_Lostfocus | CMXsrv_expcbe_lee_cor | N/A | N/A |
| fld_cbe_cod_rmb_LostFocus | CMXsrv_expcbe_lee_cor | N/A | N/A |
| Form_Activate | CMXsrv_expcbe_lee_bco | N/A | N/A |
| aceptar_Click | CMXsrv_expcbe_grb_doc | N/A | N/A |
| aceptar_Click | CMXsrv_expcbe_grb_doc02 | N/A | N/A |
| Form_Activate | CMXsrv_expcbe_lee_doc | N/A | N/A |
| Form_Activate | CMXsrv_expcbe_lee_doc02 | N/A | N/A |
| ELIMINAR_Click | CMXsrv_expcbe_del_ctz | N/A | N/A |
| Form_Activate | CMXsrv_expcbe_bus_ctz | N/A | N/A |
| aceptar_Click | CMXsrv_expcbe_grb_ctz | N/A | N/A |
| Form_Activate | CMXsrv_expcbe_mto_ctz | N/A | N/A |
| Form_Activate | CMXsrv_expcbe_lee_ctz | N/A | N/A |
| aceptar_Click | CMXsrv_expcbe_lee_cbe | N/A | N/A |
| buscar_Click | CMXsrv_expcbe_bus_cbe | N/A | N/A |
| fld_aux_cod_exp_LostFocus | CMXsrv_expcbe_lee_cln | N/A | N/A |
| Proximas_Click | CMXsrv_expcbe_bus_cbe | N/A | N/A |
| aceptar_Click | CMXsrv_expcbe_mdf_cbe | N/A | N/A |
| aceptar_Click | CMXsrv_expcbe_cre_actz | N/A | N/A |
| fld_cbe_cod_suc_LostFocus | CMXsrv_val_suc | N/A | N/A |
| Form_Activate | CMXsrv_expcbe_lee_mdf | N/A | N/A |
| aceptar_Click | CMXsrv_expcbe_pgo_cbe | N/A | N/A |
| fld_cbe_cod_rmb_LostFocus | CMXsrv_expcbe_lee_cor | N/A | N/A |
| Form_Activate | CMXsrv_expcbe_lee_pgo | N/A | N/A |
| Form_Activate | CMXsrv_expcbe_bus_evz | N/A | N/A |
| Proximo_Click | CMXsrv_expcbe_bus_evz | N/A | N/A |
| Reversar_Click | CMXsrv_expcbe_rev_cbe | N/A | N/A |
| Form_Activate | CMXsrv_expcbe_lee_evz | N/A | N/A |
| Eliminar_Click | CMXsrv_expcbe_del_dcz | N/A | N/A |
| Form_Activate | CMXsrv_expcbe_bus_dcz | N/A | N/A |
| aceptar_Click | CMXsrv_expcbe_grb_dcz | N/A | N/A |
| Form_Activate | CMXsrv_expcbe_lee_dcz | N/A | N/A |
| aceptar_Click | CMXsrv_expcbe_lee_cbe | N/A | N/A |
| buscar_Click | CMXsrv_expcbe_bus_vto | N/A | N/A |
| fld_aux_cod_exp_LostFocus | CMXsrv_expcbe_lee_cln | N/A | N/A |
| Proximas_Click | CMXsrv_expcbe_bus_vto | N/A | N/A |
| aceptar_Click | CMXsrv_avi_dat_cou | N/A | N/A |
| aceptar_Click | CMXsrv_expcbe_avs_rem1 | N/A | N/A |
| aceptar_Click | CMXsrv_expcbe_avs_rem3 | N/A | N/A |
| imprime_esp | CMXsrv_expcbe_avs_rem2 | N/A | N/A |
| imprime_esp | CMXsrv_expcbe_avs_rem4 | N/A | N/A |
| imprime_ing | CMXsrv_expcbe_avs_rem2 | N/A | N/A |
| imprime_ing | CMXsrv_expcbe_avs_rem4 | N/A | N/A |
| buscar_Click | CMXsrv_busc_plz | N/A | N/A |
| fld_cor_cod_plz_Lostfocus | CMXsrv_lee_plz | N/A | N/A |
| proximos_Click | CMXsrv_busc_plz | N/A | N/A |
| buscar_Click | CMXsrv_cor_busc_pais | N/A | N/A |
| fld_cor_cod_pais_LostFocus | CMXsrv_cor_lee_pais | N/A | N/A |
| proximos_Click | CMXsrv_cor_busc_pais | N/A | N/A |
| aceptar_Click | CMXsrv_expcbe_lee_cor | N/A | N/A |
| buscar_Click | CMXsrv_expcbe_bus_cor | N/A | N/A |
| fld_aux_cod_pai_LostFocus | CMXsrv_cor_lee_pais | N/A | N/A |
| fld_aux_cod_plz_LostFocus | CMXsrv_lee_plz | N/A | N/A |
| proximos_Click | CMXsrv_expcbe_bus_cor | N/A | N/A |
| buscar_Click | CMXsrv_busc_bco_mtr | N/A | N/A |
| proximos_Click | CMXsrv_busc_bco_mtr | N/A | N/A |
| enviar_Click | CMXsrv_expcbe_swf_sel | N/A | N/A |
| Aceptar_Click | CMXsrv_expcbe_lee_cor | N/A | N/A |
| buscar_Click | CMXsrv_expcbe_bus_cor | N/A | N/A |
| proximos_Click | CMXsrv_expcbe_bus_cor | N/A | N/A |
| Form_Load | CMXsrv_grl_fec_serv | N/A | N/A |

## EXPCCE
| Segmento | Procedimiento Almacenado | Tablas Referenciadas | Procedimientos Referenciados |
|----------|--------------------------|----------------------|--------------------------|
| Form_Activate | CMXsrv_cmx_busc_suc_usu | N/A | N/A |
| Form_Activate | CMXsrv_expcce_lee_cce | N/A | N/A |
| Form_Activate | CMXsrv_expcce_trd_cce | N/A | N/A |
| MCCEANL_CLICK | CMXsrv_expcce_anl_cce | N/A | N/A |
| Mccectb_click | CMXsrv_expcce_ctb_ing | N/A | N/A |
| Mccedel_Click | CMXsrv_expcce_del_cce | N/A | N/A |
| MCCEVAL_CLICK | CMXsrv_expcce_val_cce | N/A | N/A |
| Mmt730_Click | CMXsrv_expcce_swf_sel | N/A | N/A |
| Mmt730Ing_Click | CMXsrv_expcce_swf_sel | N/A | N/A |
| Aceptar_Click | CMXsrv_expcce_grb_bco | N/A | N/A |
| fld_cce_bco_avs_LostFocus | CMXsrv_expcce_lee_cor | N/A | N/A |
| fld_cce_bco_orig_LostFocus | CMXsrv_expcce_lee_cor | N/A | N/A |
| fld_cce_cod_ems_LostFocus | CMXsrv_expcce_lee_cor | N/A | N/A |
| fld_cce_cod_rmb_LostFocus | CMXsrv_expcce_lee_cor | N/A | N/A |
| Form_Activate | CMXsrv_expcce_lee_bco | N/A | N/A |
| Aceptar_Click | CMXsrv_expcce_grb_ctp | N/A | N/A |
| fld_cce_cod_bn1_LostFocus | CMXsrv_expcce_lee_cln | N/A | N/A |
| fld_cce_cod_bn2_LostFocus | CMXsrv_expcce_lee_cln | N/A | N/A |
| Form_Activate | CMXsrv_expcce_lee_ctp | N/A | N/A |
| Aceptar_Click | CMXsrv_expcce_cre_cce | N/A | N/A |
| Aceptar_Click | CMXsrv_expcce_grb_bco | N/A | N/A |
| Aceptar_Click | CMXsrv_expcce_grb_ctp | N/A | N/A |
| Aceptar_Click | CMXsrv_expcce_gen_dcc | N/A | N/A |
| Aceptar_Click | CMXsrv_expcce_grb_cnd | N/A | N/A |
| fld_cce_fec_vto_LostFocus | CMXsrv_util_det_habil | N/A | N/A |
| Form_Activate | CMXsrv_expcce_lee_cnd | N/A | N/A |
| Form_Activate | CMXsrv_expcce_trd_cnd | N/A | N/A |
| ELIMINAR_Click | CMXsrv_expcce_del_dcc | N/A | N/A |
| Form_Activate | CMXsrv_expcce_bus_dcc | N/A | N/A |
| Aceptar_Click | CMXsrv_expcce_grb_dcc | N/A | N/A |
| Form_Activate | CMXsrv_expcce_lee_dcc | N/A | N/A |
| Aceptar_Click | CMXsrv_expcce_lee_cce | N/A | N/A |
| buscar_Click | CMXsrv_expcce_bus_cce | N/A | N/A |
| fld_aux_cod_bn1_lostfocus | CMXsrv_expcce_lee_cln | N/A | N/A |
| proximo_Click | CMXsrv_expcce_bus_cce | N/A | N/A |
| Aceptar_Click | CMXsrv_expcce_mdf_cce | N/A | N/A |
| Cancelar_Click | CMXsrv_expcce_can_mdf | N/A | N/A |
| fld_cce_cod_bn1_LostFocus | CMXsrv_expcce_lee_cln | N/A | N/A |
| fld_cce_cod_ems_LostFocus | CMXsrv_expcce_lee_cor | N/A | N/A |
| Form_Activate | CMXsrv_expcce_lee_mdf | N/A | N/A |
| Aceptar_Click | CMXsrv_expcce_cnf_cce | N/A | N/A |
| Aceptar_Click | CMXsrv_expcce_grb_afin | N/A | N/A |
| Form_Activate | CMXsrv_expcce_lee_cnf | N/A | N/A |
| Form_Activate | CMXsrv_expcce_lee_afin | N/A | N/A |
| Aceptar_Click | CMXsrv_expcce_trp_cce | N/A | N/A |
| fld_cce_bco_dst_LostFocus | CMXsrv_expcce_lee_cor | N/A | N/A |
| Form_Activate | CMXsrv_expcce_lee_trp | N/A | N/A |
| Form_Activate | CMXsrv_expcce_bus_evc | N/A | N/A |
| proximo_Click | CMXsrv_expcce_bus_evc | N/A | N/A |
| reversar_Click | CMXsrv_expcce_rev_cce | N/A | N/A |
| Form_Activate | CMXsrv_expcce_lee_evc | N/A | N/A |
| aceptar_Click | CMXsrv_expcce_avs_rem1 | N/A | N/A |
| buscar_Click | CMXsrv_busc_plz | N/A | N/A |
| fld_cor_cod_plz_Lostfocus | CMXsrv_lee_plz | N/A | N/A |
| proximos_Click | CMXsrv_busc_plz | N/A | N/A |
| buscar_Click | CMXsrv_cor_busc_pais | N/A | N/A |
| fld_cor_cod_pais_LostFocus | CMXsrv_cor_lee_pais | N/A | N/A |
| proximos_Click | CMXsrv_cor_busc_pais | N/A | N/A |
| Aceptar_Click | CMXsrv_expcce_lee_cor | N/A | N/A |
| buscar_Click | CMXsrv_expcce_bus_cor | N/A | N/A |
| Command1_Click | CMXsrv_expcce_bus_cor | N/A | N/A |
| proximos_Click | CMXsrv_expcce_bus_cor | N/A | N/A |
| enviar_Click | CMXsrv_expcce_swf_sel | N/A | N/A |
| Form_Load | CMXsrv_grl_fec_serv | N/A | N/A |

## EXPNEG
| Segmento | Procedimiento Almacenado | Tablas Referenciadas | Procedimientos Referenciados |
|----------|--------------------------|----------------------|--------------------------|
| Form_Activate | CMXsrv_expcbe_bus_evz | N/A | N/A |
| Proximo_Click | CMXsrv_expcbe_bus_evz | N/A | N/A |
| Reversar_Click | CMXsrv_expcbe_rev_cbe | N/A | N/A |
| Form_Activate | CMXsrv_expcbe_lee_evz | N/A | N/A |
| Form_Activate | CMXsrv_expcce_lee_bas | N/A | N/A |
| Form_Activate | CMXsrv_expcce_lee_neg | N/A | N/A |
| Mccealznge_click | CMXsrv_expcce_alz_dis | N/A | N/A |
| Mcceanlnge_click | CMXsrv_expcce_anl_neg | N/A | N/A |
| Mccectbnge_Click | CMXsrv_expcce_ctb_neg | N/A | N/A |
| Mccedelnge_Click | CMXsrv_expcce_del_neg | N/A | N/A |
| Mccevalnge_click | CMXsrv_expcce_val_neg | N/A | N/A |
| Mtel742_Click | CMXsrv_expcce_swf_sel | N/A | N/A |
| Form_Activate | CMXsrv_expcce_bus_evc | N/A | N/A |
| Proximo_Click | CMXsrv_expcce_bus_evc | N/A | N/A |
| Reversar_Click | CMXsrv_expcce_rev_cce | N/A | N/A |
| Form_Activate | CMXsrv_expcce_lee_evc | N/A | N/A |
| aceptar_Click | CMXsrv_expcce_grb_neg | N/A | N/A |
| aceptar_Click | CMXsrv_expcce_gen_dcn | N/A | N/A |
| aceptar_Click | CMXsrv_expcce_grb_afin | N/A | N/A |
| fld_cce_cod_exp_nge_LostFocus | CMXsrv_expcce_lee_cln | N/A | N/A |
| fld_cce_cod_pag_nge_LostFocus | CMXsrv_expcce_lee_cor | N/A | N/A |
| fld_cce_cod_rmb_nge_LostFocus | CMXsrv_expcce_lee_cor | N/A | N/A |
| fld_cce_ins_rem1_nge_GotFocus | CMXsrv_expcce_avs_rem5 | N/A | N/A |
| Form_Load | CMXsrv_expcce_lee_nge | N/A | N/A |
| Form_Load | CMXsrv_expcce_trd_nge | N/A | N/A |
| Form_Load | CMXsrv_expcce_ini_neg | N/A | N/A |
| Form_Load | CMXsrv_expcce_lee_afin | N/A | N/A |
| lee_bco | CMXsrv_expcce_lee_cor | N/A | N/A |
| ELIMINAR_Click | CMXsrv_expcce_del_dcn | N/A | N/A |
| Form_Activate | CMXsrv_expcce_bus_dcn | N/A | N/A |
| Aceptar_Click | CMXsrv_expcce_grb_dcn | N/A | N/A |
| Form_Load | CMXsrv_expcce_lee_dcn | N/A | N/A |
| ELIMINAR_Click | CMXsrv_expcce_del_ltr | N/A | N/A |
| Form_Activate | CMXsrv_expcce_bus_ltr | N/A | N/A |
| Aceptar_Click | CMXsrv_expcce_grb_ltr | N/A | N/A |
| Form_Load | CMXsrv_expcce_lee_ltr | N/A | N/A |
| ELIMINAR_Click | CMXsrv_expcce_del_dsn | N/A | N/A |
| Form_Activate | CMXsrv_expcce_gen_dsn | N/A | N/A |
| Form_Activate | CMXsrv_expcce_bus_dsn | N/A | N/A |
| Salir_Click | CMXsrv_expcce_chk_dsn | N/A | N/A |
| Aceptar_Click | CMXsrv_expcce_grb_dsn | N/A | N/A |
| Form_Load | CMXsrv_expcce_lee_dsn | N/A | N/A |
| buscar_Click | CMXsrv_expcce_bus_neg | N/A | N/A |
| Proximas_Click | CMXsrv_expcce_bus_neg | N/A | N/A |
| aceptar_Click | CMXsrv_expcce_pgo_neg | N/A | N/A |
| aceptar_Click | CMXsrv_expcce_grb_afin | N/A | N/A |
| fld_cce_cod_exp_nge_LostFocus | CMXsrv_expcce_lee_cln | N/A | N/A |
| fld_cce_cod_rmb_nge_LostFocus | CMXsrv_expcce_lee_cor | N/A | N/A |
| Form_Load | CMXsrv_expcce_lee_pgo | N/A | N/A |
| Form_Load | CMXsrv_expcce_lee_afin | N/A | N/A |
| lee_bco | CMXsrv_expcce_lee_cor | N/A | N/A |
| aceptar_Click | CMXsrv_avi_dat_cou | N/A | N/A |
| aceptar_Click | CMXsrv_expcce_lee_nge | N/A | N/A |
| aceptar_Click | CMXsrv_expcce_avs_rem1 | N/A | N/A |
| aceptar_Click | CMXsrv_expcce_avs_rem3 | N/A | N/A |
| imprime_esp | CMXsrv_expcce_avs_rem2 | N/A | N/A |
| imprime_esp | CMXsrv_expcce_avs_rem4 | N/A | N/A |
| imprime_esp | CMXsrv_expcbe_avs_rem4 | N/A | N/A |
| imprime_ing | CMXsrv_expcce_avs_rem2 | N/A | N/A |
| imprime_ing | CMXsrv_expcce_avs_rem4 | N/A | N/A |
| imprime_ing | CMXsrv_expcbe_avs_rem4 | N/A | N/A |
| aceptar_Click | CMXsrv_expcce_lee_cor | N/A | N/A |
| buscar_Click | CMXsrv_expcce_bus_cor | N/A | N/A |
| proximos_Click | CMXsrv_expcce_bus_cor | N/A | N/A |
| enviar_Click | CMXsrv_expcce_swf_sel | N/A | N/A |
| Form_Load | CMXsrv_grl_fec_serv | N/A | N/A |

## IMPORT
| Segmento | Procedimiento Almacenado | Tablas Referenciadas | Procedimientos Referenciados |
|----------|--------------------------|----------------------|--------------------------|
| buscar_Click | CMXsrv_icrd_lee_dir_cln | N/A | N/A |
| buscar_click | CMXsrv_icrd_lee_tex_swf | N/A | N/A |
| Aceptar_Click | CMXsrv_icrd_lee_cod_txt_swf | N/A | N/A |
| buscar_click | CMXsrv_icrd_lee_txt_swf_all | N/A | N/A |
| Form_Load | CMXsrv_icrd_lee_ind_esp_ing | N/A | N/A |
| llena_arreglo | CMXsrv_icrd_lee_tex_swf | N/A | N/A |
| proximo_Click | CMXsrv_icrd_lee_txt_swf_all | N/A | N/A |
| Aceptar_Click | CMXCRDsrv_icrd_a_cnd_esp | N/A | N/A |
| Form_Load | CMXsrv_icrd_lee_cnd_esp | N/A | N/A |
| clon_Click | CMXCRDsrv_icrd_clon_crd | N/A | N/A |
| Form_Activate | CMXCRDsrv_icrd_lee_crdcre | N/A | N/A |
| Form_Activate | CMXsrv_icrd_lee_ind_esp_ing | N/A | N/A |
| Form_Activate | CMXsrv_icrd_lee_top | N/A | N/A |
| Form_Load | CMXsrv_grl_fec_serv | N/A | N/A |
| Form_Load | CMXsrv_cmx_get_codes | N/A | N/A |
| Form_Load | CMXsrv_trae_glo_fec | N/A | N/A |
| Mcrdapr_Click | CMXCRDsrv_icrd_val_crd | N/A | N/A |
| Mcrdeli_click | CMXCRDsrv_icrd_eli_crd | N/A | N/A |
| Mcrdtxtliq_Click | CMXsrv_icrd_lee_dat_trs | N/A | N/A |
| Mcrdtxtope_Click | CMXsrv_icrd_dat_liq_ope | N/A | N/A |
| msg_swift | CMXsrv_iswf_a_pru | N/A | N/A |
| Aceptar_Click | CMXsrv_icrd_a_ctp | N/A | N/A |
| FLD_COL_COD_CLI_LostFocus | CMXsrv_icrd_lee_cln | N/A | N/A |
| Form_Load | CMXsrv_lee_fpro | N/A | N/A |
| Aceptar_Click | CMXsrv_icrd_a_cnd | N/A | N/A |
| Aceptar_Click | CMXCRDsrv_icrd_crea_crd | N/A | N/A |
| fld_col_fec_vto_LostFocus | CMXsrv_util_det_habil | N/A | N/A |
| Form_Activate | CMXsrv_icrd_busc_emb | N/A | N/A |
| ELIMINAR_Click | CMXsrv_icrd_eli_emb | N/A | N/A |
| Form_Load | CMXsrv_icrd_lee_emb1 | N/A | N/A |
| Form_Load | CMXsrv_icrd_lee_emb2 | N/A | N/A |
| ingresar_Click | CMXsrv_icrd_a_emb1 | N/A | N/A |
| ingresar_Click | CMXsrv_icrd_a_emb2 | N/A | N/A |
| VALIDA_EMBARQUE | CMXsrv_icrd_val_emb2 | N/A | N/A |
| VALIDA_EMBARQUE | CMXsrv_icrd_val_emb1 | N/A | N/A |
| Aceptar_Click | CMXsrv_icrd_act_ref | N/A | N/A |
| Form_Load | CMXsrv_icrd_act_ref | N/A | N/A |
| Form_Load | CMXsrv_icrd_lee_ref | N/A | N/A |
| buscar_click | CMXCRDsrv_icrd_busc_crd | N/A | N/A |
| FLD_COL_COD_CLI_LostFocus | CMXsrv_icrd_lee_cln | N/A | N/A |
| PROXIMA_Click | CMXCRDsrv_icrd_busc_crd | N/A | N/A |
| Aceptar_Click | CMXCRDsrv_icrd_apr_sol | N/A | N/A |
| Form_Load | CMXsrv_icrd_lee_crdapr | N/A | N/A |
| Aceptar_Click | CMXsrv_icrd_rech_sol | N/A | N/A |
| Aceptar_Click | CMXCRDsrv_icrd_a_desc_merc | N/A | N/A |
| Form_Load | CMXsrv_icrd_lee_desc_merc | N/A | N/A |
| Aceptar_Click | CMXsrv_icrd_a_otr_doc | N/A | N/A |
| Form_Load | CMXsrv_icrd_lee_otr_doc | N/A | N/A |
| enviar_Click | CMXsrv_iswf_a_pru | N/A | N/A |

## INFORME
| Segmento | Procedimiento Almacenado | Tablas Referenciadas | Procedimientos Referenciados |
|----------|--------------------------|----------------------|--------------------------|
| Eliminar_Click | CMXsrv_iarc_eli_arc | N/A | N/A |
| Form_Activate | CMXsrv_iarc_busc_arc | N/A | N/A |
| Form_Activate | CMXsrv_iinf_lee0_inf | N/A | N/A |
| Form_Activate | CMXsrv_iinf_lee_tablas | N/A | N/A |
| Form_Activate | CMXsrv_iinf_lee1_inf | N/A | N/A |
| Form_Activate | CMXsrv_iinf_lee_cln | N/A | N/A |
| Form_Activate | CMXsrv_iinf_lee2_inf | N/A | N/A |
| Form_Activate | CMXsrv_iinf_avi_miscb | N/A | N/A |
| Maviapr_Click | CMXsrv_iinf_avi_misca | N/A | N/A |
| Maviapr_Click | CMXsrv_iinf_avi_miscb | N/A | N/A |
| Mavicom_Click | CMXsrv_iinf_avi_misca | N/A | N/A |
| Mavicom_Click | CMXsrv_iinf_avi_miscb | N/A | N/A |
| Mavicom_Click | CMXsrv_icrd_lee_dat_com | N/A | N/A |
| Mavimis1_Click | CMXsrv_iinf_avi_misca | N/A | N/A |
| Mavimis1_Click | CMXsrv_iinf_avi_miscb | N/A | N/A |
| Mavimis2_Click | CMXsrv_iinf_avi_misca | N/A | N/A |
| Mavimis2_Click | CMXsrv_iinf_avi_miscb | N/A | N/A |
| Mavirec_Click | CMXsrv_iinf_avi_misca | N/A | N/A |
| Mavirec_Click | CMXsrv_iinf_avi_miscb | N/A | N/A |
| Mavitib_Click | CMXsrv_iinf_avi_misca | N/A | N/A |
| Mavitib_Click | CMXsrv_iinf_avi_miscb | N/A | N/A |
| Mavitras_Click | CMXsrv_iinf_avi_misca | N/A | N/A |
| Mavitras_Click | CMXsrv_iinf_avi_miscb | N/A | N/A |
| Mavitras_Click | CMXsrv_icrd_lee_dat_trs | N/A | N/A |
| Minfoeli_click | CMXsrv_iinf_eli_inf | N/A | N/A |
| Minforev_Click | CMXsrv_iinf_busc_evi | N/A | N/A |
| Minfoval_click | CMXsrv_iinf_val_inf | N/A | N/A |
| Aceptar_Click | CMXsrv_iinf_ingmod_inf | N/A | N/A |
| Fec_pre | CMXsrv_iinf_lee_fec | N/A | N/A |
| fld_aux_glo_cls_com_LostFocus | CMXsrv_iinf_lee_tablas | N/A | N/A |
| fld_aux_glo_for_pag1_LostFocus | CMXsrv_iinf_lee_tablas | N/A | N/A |
| fld_aux_glo_for_pag2_LostFocus | CMXsrv_iinf_lee_tablas | N/A | N/A |
| fld_aux_glo_for_pag3_LostFocus | CMXsrv_iinf_lee_tablas | N/A | N/A |
| fld_aux_glo_mon_LostFocus | CMXsrv_iinf_lee_tablas | N/A | N/A |
| fld_inf_cls_com_Lostfocus | CMXsrv_iinf_lee_tablas | N/A | N/A |
| fld_inf_cod_imp_LostFocus | CMXsrv_iinf_lee_cln | N/A | N/A |
| fld_inf_for_pag1_lostfocus | CMXsrv_iinf_lee_tablas | N/A | N/A |
| fld_inf_for_pag2_LostFocus | CMXsrv_iinf_lee_tablas | N/A | N/A |
| fld_inf_for_pag3_LostFocus | CMXsrv_iinf_lee_tablas | N/A | N/A |
| fld_inf_mon_inf_lostfocus | CMXsrv_iinf_lee_tablas | N/A | N/A |
| Form_Load | CMXsrv_iinf_lee0_inf | N/A | N/A |
| Form_Load | CMXsrv_iinf_lee1_inf | N/A | N/A |
| Form_Load | CMXsrv_iinf_lee2_inf | N/A | N/A |
| valor_usd | CMXsrv_iinf_lee_usd | N/A | N/A |
| Aceptar_Click | CMXsrv_iinf_busc_inf | N/A | N/A |
| buscar_Click | CMXsrv_iinf_busc_inf | N/A | N/A |
| Fec_pre | CMXsrv_iinf_lee_fec | N/A | N/A |
| fld_inf_cod_imp_LostFocus | CMXsrv_iinf_lee_cln | N/A | N/A |
| PROXIMA_Click | CMXsrv_iinf_busc_inf | N/A | N/A |
| Aceptar_Click | CMXsrv_iinf_act_apr | N/A | N/A |
| Form_Activate | CMXsrv_iinf_busc_evi | N/A | N/A |
| reversar_Click | CMXsrv_iinf_rev_evi | N/A | N/A |
| Form_Load | CMXsrv_iinf_lee_evi | N/A | N/A |
| Aceptar_Click | CMXsrv_iinf_act_tib | N/A | N/A |
| Aceptar_Click | CMXsrv_iinf_act_rec | N/A | N/A |
| Aceptar_Click | CMXsrv_iinf_act_rib | N/A | N/A |
| Form_Activate | CMXsrv_iinf_busc_comp | N/A | N/A |
| proximos_Click | CMXsrv_iinf_busc_comp | N/A | N/A |
| Aceptar_Click | CMXsrv_iinf_ingmod_comp | N/A | N/A |
| Fec_pre | CMXsrv_iinf_lee_fec | N/A | N/A |
| Form_Activate | CMXsrv_iinf_lee_comp | N/A | N/A |
| Form_Activate | CMXsrv_iinf_lee_tablas | N/A | N/A |
| aceptar_click | CMXsrv_iinf_lee_bco | N/A | N/A |
| buscar_Click | CMXsrv_iinf_busc_bco | N/A | N/A |
| Form_Load | CMXsrv_grl_fec_serv | N/A | N/A |

## INGRESO
| Segmento | Procedimiento Almacenado | Tablas Referenciadas | Procedimientos Referenciados |
|----------|--------------------------|----------------------|--------------------------|
| cancelar_Click | CMXsrv_fincol_ren_fin | N/A | N/A |
| ELIMINAR_Click | CMXsrv_fincol_ecuo | N/A | N/A |
| form_activate | CMXsrv_fincol_gpln | N/A | N/A |
| form_activate | CMXsrv_fincol_cons_plnpa | N/A | N/A |
| cancelar_Click | CMXsrv_fincol_ren_fin | N/A | N/A |
| ELIMINAR_Click | CMXsrv_fincol_eava | N/A | N/A |
| form_activate | CMXsrv_fincol_cons_aval | N/A | N/A |
| aceptar_Click | CMXsrv_fincol_gmod_ctr | N/A | N/A |
| busca_bco | CMXsrv_icrd_lee_bco_swf | N/A | N/A |
| fld_obl_bco_acr_LostFocus | CMXsrv_fincol_lee_bco | N/A | N/A |
| fld_obl_rut_acr_LostFocus | CMXsrv_fincol_lee_cln | N/A | N/A |
| form_activate | CMXsrv_fincol_cons_ctr | N/A | N/A |
| aceptar_Click | CMXsrv_fincol_ctb_oto | N/A | N/A |
| avi1_Click | CMXsrv_icrd_avi_crd | N/A | N/A |
| Avi5_Click | CMXsrv_icrd_dat_liq_ope | N/A | N/A |
| form_activate | CMXsrv_fincol_lee_col | N/A | N/A |
| Form_Load | CMXsrv_lee_fpro | N/A | N/A |
| MCOLCOMI_CLICK | CMXsrv_busc_cod_ope | N/A | N/A |
| MCOLCOMI_CLICK | CMXsrv_col_trae_num_ope | N/A | N/A |
| MCOLCONTOTOR_CLICK | CMXsrv_busc_cod_ope | N/A | N/A |
| MCOLCONTOTOR_CLICK | CMXsrv_col_trae_num_ope | N/A | N/A |
| MCOLCONTOTOR_CLICK | CMXsrv_fincol_ctb_oto | N/A | N/A |
| MCOLELI_CLICK | CMXsrv_fincol_eli_col | N/A | N/A |
| valida | CMXsrv_fincol_val_col | N/A | N/A |
| aceptar_Click | CMXsrv_fincol_lee_col | N/A | N/A |
| buscar_Click | CMXsrv_fincol_bsc_col | N/A | N/A |
| fld_col_tip_ope_lostfocus | CMXsrv_fincol_lee_tip | N/A | N/A |
| PROXIMAS_Click | CMXsrv_fincol_bsc_col | N/A | N/A |
| buscar_Click | CMXsrv_fincol_bsc_TIP | N/A | N/A |
| ingresar_Click | CMXsrv_fincol_iava | N/A | N/A |
| aceptar_Click | CMXsrv_busc_cod_ope | N/A | N/A |
| aceptar_Click | CMXsrv_col_trae_num_ope | N/A | N/A |
| aceptar_Click | CMXsrv_fincol_ctb_novf | N/A | N/A |
| FLD_COL_COD_CLI_LOSTFOCUS | CMXsrv_fincol_lee_cln | N/A | N/A |
| FLD_COL_RUT_DEU_NOV_LostFocus | CMXsrv_fincol_lee_cln | N/A | N/A |
| form_activate | CMXsrv_fincol_cons_nov | N/A | N/A |
| FLD_COL_COD_CLI_LOSTFOCUS | CMXsrv_fincol_lee_cln | N/A | N/A |
| FLD_COL_RUT_DEU_NOV_LostFocus | CMXsrv_fincol_lee_cln | N/A | N/A |
| form_activate | CMXsrv_fincol_cons_dnov | N/A | N/A |
| cmdAceptar_Click | CMXsrv_grabar_pag_adi_dus | N/A | N/A |
| Form_Load | CMXsrv_buscar_pag_adi_dus | N/A | N/A |
| Aceptar_Click | CMXsrv_icrd_lee_bco_swf | N/A | N/A |
| buscar_Click | CMXsrv_icrd_busc_bco | N/A | N/A |
| proximo_Click | CMXsrv_icrd_busc_bco | N/A | N/A |
| Form_Load | CMXsrv_cmx_get_codes | N/A | N/A |
| Form_Load | CMXsrv_grl_trae_cod_bco | N/A | N/A |

## MODIFIC
| Segmento | Procedimiento Almacenado | Tablas Referenciadas | Procedimientos Referenciados |
|----------|--------------------------|----------------------|--------------------------|
| Form_Activate | CMXsrv_fincol_cons_tas | N/A | N/A |
| aceptar_click | CMXsrv_fincol_efec_tras | N/A | N/A |
| Form_Activate | CMXsrv_fincol_cons_trasp | N/A | N/A |
| Form_Activate | CMXsrv_fincol_cons_dtrs | N/A | N/A |
| EFECTUAR_Click | CMXsrv_fincol_rev_eve | N/A | N/A |
| Form_Activate | CMXsrv_fincol_cons_eve | N/A | N/A |
| Form_Load | CMXsrv_fincol_cons_deve | N/A | N/A |
| aceptar_click | CMXsrv_fincol_cont_gst | N/A | N/A |
| Form_Activate | CMXsrv_fincol_cons_gst | N/A | N/A |
| Form_Activate | CMXsrv_fincol_cons_dgst | N/A | N/A |
| Form_Load | CMXsrv_lee_fpro | N/A | N/A |

## MOD_ADI
| Segmento | Procedimiento Almacenado | Tablas Referenciadas | Procedimientos Referenciados |
|----------|--------------------------|----------------------|--------------------------|
| Aceptar_Click | CMXsrv_icrd_a_cnd | N/A | N/A |
| busca_bco | CMXsrv_icrd_lee_bco_swf | N/A | N/A |
| fld_col_fec_vto_LostFocus | CMXsrv_util_det_habil | N/A | N/A |
| Form_Load | CMXMCRDsrv_icrd_lee_mcnd | N/A | N/A |
| Form_Load | CMXsrv_grl_fec_serv | N/A | N/A |

## MOD_CBR
| Segmento | Procedimiento Almacenado | Tablas Referenciadas | Procedimientos Referenciados |
|----------|--------------------------|----------------------|--------------------------|
| fld_cbr_cod_gdo_LostFocus | CMXsrv_icbr_lee_cln | N/A | N/A |
| Form_Load | CMXsrv_icbr_lee_ctp | N/A | N/A |
| INGRESAR_Click | CMXsrv_icbr_act_ctp | N/A | N/A |
| Form_Load | CMXsrv_icbr_lee_trm | N/A | N/A |
| INGRESAR_Click | CMXsrv_icbr_act_trm | N/A | N/A |
| Form_Load | CMXsrv_icbr_lee_doc | N/A | N/A |
| INGRESAR_Click | CMXsrv_icbr_act_doc | N/A | N/A |
| Form_Activate | CMXsrv_icbr_busc_let | N/A | N/A |
| aceptar_Click | CMXsrv_icbr_mod_ing_let | N/A | N/A |
| eliminar_Click | CMXsrv_icbr_eli_let | N/A | N/A |
| Form_Activate | CMXsrv_icbr_lee_let | N/A | N/A |
| actualizar_Click | CMXsrv_icbr_acep_mod_cbr | N/A | N/A |
| Cancelar_Click | CMXsrv_icbr_eli_no_cont | N/A | N/A |

## MOD_CRD
| Segmento | Procedimiento Almacenado | Tablas Referenciadas | Procedimientos Referenciados |
|----------|--------------------------|----------------------|--------------------------|
| Aceptar_Click | CMXsrv_icrd_a_ibab | N/A | N/A |
| Form_Load | CMXsrv_icrd_lee_glo_ibab | N/A | N/A |
| Aceptar_Click | CMXsrv_icrd_a_ibar | N/A | N/A |
| Form_Load | CMXsrv_icrd_lee_glo_ibar | N/A | N/A |
| buscar_click | CMXsrv_icrd_lee_dir_cln | N/A | N/A |
| buscar_Click | CMXsrv_icrd_lee_tex_swf | N/A | N/A |
| buscar_click | CMXsrv_icrd_lee_tex_swf | N/A | N/A |
| Aceptar_Click | CMXsrv_icrd_lee_cod_txt_swf | N/A | N/A |
| buscar_click | CMXsrv_icrd_lee_txt_swf_all | N/A | N/A |
| Form_Load | CMXsrv_icrd_lee_ind_esp_ing | N/A | N/A |
| llena_arreglo | CMXsrv_icrd_lee_tex_swf | N/A | N/A |
| proximo_Click | CMXsrv_icrd_lee_txt_swf_all | N/A | N/A |
| Aceptar_Click | CMXMCRDsrv_icrd_a_mmcnd | N/A | N/A |
| Form_Load | CMXsrv_icrd_lee_cnd_esp | N/A | N/A |
| Aceptar_Click | CMXsrv_icrd_a_ctp | N/A | N/A |
| FLD_COL_COD_CLI_LostFocus | CMXsrv_icrd_lee_cln | N/A | N/A |
| Form_Load | CMXMCRDsrv_icrd_lee_mctp | N/A | N/A |
| Aceptar_Click | CMXsrv_icrd_a_cnd | N/A | N/A |
| Form_Load | CMXMCRDsrv_icrd_lee_mcnd | N/A | N/A |
| Form_Activate | CMXsrv_icrd_busc_emb | N/A | N/A |
| cancelar_Click | CMXsrv_icrd_lee_desc_merc | N/A | N/A |
| ELIMINAR_Click | CMXsrv_icrd_eli_emb | N/A | N/A |
| Form_Load | CMXMCRDsrv_icrd_lee_memb2 | N/A | N/A |
| Form_Load | CMXMCRDsrv_icrd_lee_memb1 | N/A | N/A |
| ingresar_Click | CMXsrv_icrd_a_emb1 | N/A | N/A |
| ingresar_Click | CMXsrv_icrd_a_emb2 | N/A | N/A |
| VALIDA_EMBARQUE | CMXsrv_icrd_val_emb2 | N/A | N/A |
| VALIDA_EMBARQUE | CMXsrv_icrd_val_emb1 | N/A | N/A |
| Aceptar_Click | CMXsrv_icrd_act_ref | N/A | N/A |
| fld_obl_cod_bco_acre_DblClick | CMXsrv_icrd_lee_bco_swf | N/A | N/A |
| fld_obl_cod_bco_acre_LostFocus | CMXsrv_icrd_lee_bco_swf | N/A | N/A |
| Form_Load | CMXMCRDsrv_icrd_lee_mref | N/A | N/A |
| Aceptar_Click | CMXsrv_icrd_ing_txt | N/A | N/A |
| Form_Load | CMXCRDsrv_icrd_get_ing_esp | N/A | N/A |
| Form_Load | CMXMCRDsrv_icrd_lee_mtxt | N/A | N/A |
| Form_Load | CMXCRDsrv_icrd_get_pre_fra | N/A | N/A |
| Aceptar_Click | CMXMCRDsrv_icrd_a_mmer | N/A | N/A |
| Form_Load | CMXsrv_icrd_lee_desc_merc | N/A | N/A |
| Aceptar_Click | CMXsrv_icrd_a_otr_doc | N/A | N/A |
| Form_Load | CMXsrv_icrd_lee_otr_doc | N/A | N/A |
| Aceptar_Click | CMXsrv_fincol_lee_cod_eve | N/A | N/A |
| Aceptar_Click | CMXMCRDsrv_icrd_acep_mod_crd | N/A | N/A |
| cancelar_Click | CMXMCRDsrv_icrd_eli_no_cont | N/A | N/A |
| fld_crd_cod_bco_rem_LostFocus | CMXsrv_icrd_lee_bco_swf | N/A | N/A |
| fld_crd_fec_mod_lostFocus | CMXsrv_fincol_efec_calpa | N/A | N/A |
| Form_Activate | CMXsrv_icrd_lee_ind_esp_ing | N/A | N/A |
| Form_Load | CMXsrv_fincol_efec_calpa | N/A | N/A |
| Form_Load | CMXMCRDsrv_icrd_lee_mcnd | N/A | N/A |
| Form_Load | CMXsrv_grl_fec_serv | N/A | N/A |

## NEGO_AV
| Segmento | Procedimiento Almacenado | Tablas Referenciadas | Procedimientos Referenciados |
|----------|--------------------------|----------------------|--------------------------|
| aviso1 | CMXsrv_icrd_a_rec_age | N/A | N/A |
| aviso1 | CMXsrv_busc_ofi_cta | N/A | N/A |
| aviso1 | CMXsrv_neg_busc_arc | N/A | N/A |
| aviso1 | CMXsrv_icrd_lee_avi_adi | N/A | N/A |
| aviso3 | CMXsrv_icrd_lee_dat_trs | N/A | N/A |
| Aviso4 | CMXsrv_icrd_dat_liq_ope | N/A | N/A |
| Aviso4 | CMXsrv_icrd_lee_dat_cln | N/A | N/A |
| Aviso5 | CMXsrv_icrd_lee_dat_cln | N/A | N/A |
| Aviso5 | CMXsrv_icrd_lee_avi_dis | N/A | N/A |
| Aviso5 | CMXsrv_icrd_lee_avi_adi | N/A | N/A |
| Aviso5 | CMXsrv_neg_ddi_asoc | N/A | N/A |
| Aviso5 | CMXsrv_neg_busc_arc | N/A | N/A |
| Aviso5 | CMXsrv_neg_trae_vcto_mcf | N/A | N/A |
| Aviso6 | CMXsrv_icrd_avs_cyg1 | N/A | N/A |
| Aviso6 | CMXsrv_icrd_avs_cyg2 | N/A | N/A |
| lee_aval | CMXsrv_neg_avi_lee_aval | N/A | N/A |
| lee_nego | CMXsrv_icrd_neg_lee_crd | N/A | N/A |
| lee_nego | CMXsrv_icrd_lee_neg | N/A | N/A |
| avi_col1 | CMXsrv_col_avi_dat_cln | N/A | N/A |
| avi_col1 | CMXsrv_col_avi_det_pag | N/A | N/A |
| avi_col2 | CMXsrv_col_avi_dat_cln | N/A | N/A |
| avi_col2 | CMXsrv_col_avi_det_oto | N/A | N/A |
| avi_col4 | CMXsrv_col_avi_dat_cln | N/A | N/A |
| avi_col4 | CMXsrv_col_lee_num_trs | N/A | N/A |
| lee_obl_oto | CMXsrv_finobl_avi_oto | N/A | N/A |
| lee_obl_pag | CMXsrv_finobl_avi_pag | N/A | N/A |
| traspaso | CMXsrv_neg_avi_trae_asnd_mn | N/A | N/A |
| traspaso | CMXsrv_neg_avi_trae_asnd_mx | N/A | N/A |
| Form_Activate | CMXsrv_icrd_neg_lee_crd | N/A | N/A |
| Form_Activate | CMXsrv_icrd_lee_neg | N/A | N/A |
| Mcrdtxtliq_Click | CMXsrv_icrd_lee_dat_trs | N/A | N/A |
| Mcrdtxtope_Click | CMXsrv_icrd_dat_liq_ope | N/A | N/A |
| Mnegavi3_Click | CMXsrv_icrd_avs_cyg1 | N/A | N/A |
| Mnegavi3_Click | CMXsrv_icrd_avs_cyg2 | N/A | N/A |
| Mnegavi4_Click | CMXsrv_icrd_lee_dat_liq | N/A | N/A |
| MNEGCONT_Click | CMXsrv_icrd_cont_neg | N/A | N/A |
| MNEGELI_CLICK | CMXsrv_icrd_eli_neg | N/A | N/A |
| precarga_datos | CMXsrv_icrd_a_rec_age | N/A | N/A |
| precarga_datos | CMXsrv_busc_ofi_cta | N/A | N/A |
| Form_Load | CMXsrv_trae_glo_fec | N/A | N/A |
| Form_Load | CMXsrv_icrd_lee_num_col | N/A | N/A |
| Form_Load | CMXsrv_icrd_bus_pago | N/A | N/A |

## NNEGO
| Segmento | Procedimiento Almacenado | Tablas Referenciadas | Procedimientos Referenciados |
|----------|--------------------------|----------------------|--------------------------|
| Form_Activate | CMXsrv_icrd_neg_lee_crd | N/A | N/A |
| Form_Activate | CMXsrv_icrd_lee_neg | N/A | N/A |
| gen_mens_swift | CMXsrv_iswf_a_pru | N/A | N/A |
| llama_pagos | CMXsrv_icrd_lee_col | N/A | N/A |
| Mnegavi9_Click | CMXsrv_iswf_a_pru | N/A | N/A |
| MNEGCONT_Click | CMXsrv_icrd_cont_neg | N/A | N/A |
| MNEGELI_CLICK | CMXsrv_icrd_eli_neg | N/A | N/A |
| pertas_Click | CMXsrv_icrd_lee_col | N/A | N/A |
| prueba_Click | CMX2srv_neg_avi_dat_cln | N/A | N/A |
| prueba_Click | CMX2srv_neg_avi_det_int | N/A | N/A |
| prueba_Click | CMX2srv_neg_avi_trae_asnd_mn | N/A | N/A |
| prueba_Click | CMX2srv_neg_avi_trae_asnd_mx | N/A | N/A |
| prueba_pag_Click | CMX2srv_neg_avi_dat_cln | N/A | N/A |
| prueba_pag_Click | CMX2srv_neg_avi_det_pag | N/A | N/A |
| prueba_pag_Click | CMX2srv_neg_avi_trae_asnd_mn | N/A | N/A |
| prueba_pag_Click | CMX2srv_neg_avi_trae_asnd_mx | N/A | N/A |
| Form_Activate | CMXsrv_icrd_busc_neg | N/A | N/A |
| Form_Load | CMXsrv_icrd_busc_emb | N/A | N/A |
| ACEPTAR_Click | CMXsrv_icrd_a_neg_emb1 | N/A | N/A |
| ACEPTAR_Click | CMXsrv_icrd_a_neg_emb2 | N/A | N/A |
| CANCELAR_Click | CMXsrv_icrd_eli_doc_neg | N/A | N/A |
| Form_Activate | CMXsrv_icrd_lee_emb1 | N/A | N/A |
| Form_Activate | CMXsrv_icrd_lee_emb2 | N/A | N/A |
| Form_Activate | CMXsrv_icrd_lee_neg_emb1 | N/A | N/A |
| Form_Activate | CMXsrv_icrd_lee_neg_emb2 | N/A | N/A |
| Form_Activate | CMXsrv_icrd_lee_cnd_esp | N/A | N/A |
| Form_Activate | CMXsrv_icrd_lee_desc_merc | N/A | N/A |
| ACEPTAR_Click | CMXsrv_icrd_a_neg_disc | N/A | N/A |
| Form_Load | CMXsrv_icrd_neg_lee_disc | N/A | N/A |
| ACEPTAR_Click | CMXsrv_icrd_ent_doc | N/A | N/A |
| ELIMINAR_Click | CMXsrv_icrd_ent_doc | N/A | N/A |
| Form_Load | CMXsrv_icrd_ent_doc | N/A | N/A |
| ACEPTAR_Click | MIGRCMXsrv_neg_grb_ind_com_disc | N/A | N/A |
| ACEPTAR_Click | CMXsrv_con_convenio_banco | N/A | N/A |
| ACEPTAR_Click | CMXsrv_icrd_alz_disc | N/A | N/A |
| aceptar_click | CMXCRDsrv_icrd_asignar_cor | N/A | N/A |
| BUSCAR_Click | CMXCRDsrv_icrd_bus_lcr_bco | N/A | N/A |
| proximo_Click | CMXCRDsrv_icrd_bus_lcr_bco | N/A | N/A |
| ACEPTAR_Click | CMXsrv_icrd_act_doc_neg | N/A | N/A |
| Form_Load | CMXsrv_icrd_lee_doc_neg | N/A | N/A |
| enviar_Click | CMXsrv_iswf_a_pru | N/A | N/A |
| Form_Load | CMXsrv_icrd_val_neg | N/A | N/A |
| Form_Load | CMXsrv_grl_fec_serv | N/A | N/A |
| Form_Load | CMXsrv_icrd_bus_pago | N/A | N/A |

## OBLIGA
| Segmento | Procedimiento Almacenado | Tablas Referenciadas | Procedimientos Referenciados |
|----------|--------------------------|----------------------|--------------------------|
| buscar_Click | CMXsrv_fincol_bsc_tip | N/A | N/A |
| Proxima_Click | CMXsrv_fincol_bsc_tip | N/A | N/A |
| proximo_Click | CMXsrv_fincol_bsc_tip | N/A | N/A |
| buscar_Click | CMXsrv_finobl_bus_cor | N/A | N/A |
| proximo_Click | CMXsrv_finobl_bus_cor | N/A | N/A |
| ELIMINAR_Click | CMXsrv_finobl_ecuo | N/A | N/A |
| form_activate | CMXsrv_finobl_gpln | N/A | N/A |
| form_activate | CMXsrv_finobl_cons_plnpa | N/A | N/A |
| anunctb_Click | CMXsrv_finobl_calc_anu | N/A | N/A |
| form_activate | CMXsrv_finobl_lee_obl | N/A | N/A |
| Form_Load | CMXsrv_lee_fpro | N/A | N/A |
| Mcbeanl_Click | CMXsrv_finobl_calc_anu | N/A | N/A |
| Mcbectb_Click | CMXsrv_finobl_ctb_oto | N/A | N/A |
| Mcbedel_Click | CMXsrv_fincol_eli_obl | N/A | N/A |
| Mobl_liq_ope_Click | CMXsrv_icrd_dat_liq_ope | N/A | N/A |
| valida_error | CMXsrv_finobl_val_obl | N/A | N/A |
| buscar_Click | CMXsrv_finobl_bsc_obl | N/A | N/A |
| fld_obl_tip_ope_LostFocus | CMXsrv_fincol_lee_tip | N/A | N/A |
| Proxima_Click | CMXsrv_finobl_bsc_obl | N/A | N/A |
| contabilizar_Click | CMXsrv_finobl_ictb_pag | N/A | N/A |
| contabilizar_Click | CMXsrv_finobl_obt_sdocuo | N/A | N/A |
| form_activate | CMXsrv_finobl_new_tas | N/A | N/A |
| form_activate | CMXsrv_finobl_cons_pag | N/A | N/A |
| form_activate | CMXsrv_finobl_cons_detp | N/A | N/A |
| calcular_Click | CMXsrv_finobl_calc_pror | N/A | N/A |
| form_activate | CMXsrv_finobl_cons_pror | N/A | N/A |
| form_activate | CMXsrv_finobl_cons_dpror | N/A | N/A |
| contabilizar_Click | CMXsrv_finobl_ctb_anu | N/A | N/A |
| calcular_Click | CMXsrv_finobl_calc_anu | N/A | N/A |
| form_activate | CMXsrv_finobl_cons_anu | N/A | N/A |
| form_activate | CMXsrv_finobl_cons_mod | N/A | N/A |
| form_activate | CMXsrv_finobl_cons_dmod | N/A | N/A |
| efectuar_Click | CMXsrv_finobl_rev_eve | N/A | N/A |
| form_activate | CMXsrv_finobl_cons_eve | N/A | N/A |
| form_activate | CMXsrv_finobl_cons_deve | N/A | N/A |
| ELIMINAR_Click | CMXsrv_finobl_eli_ctr | N/A | N/A |
| form_activate | CMXsrv_finobl_cons_ctr | N/A | N/A |
| nuevo_Click | CMXsrv_finobl_ing_ctr | N/A | N/A |
| aceptar_Click | CMXsrv_finobl_cesion_obl | N/A | N/A |
| banco_acreedor | CMXsrv_comgrl_lee_nom_cor | N/A | N/A |
| fld_obl_cod_bco_acre_lostfocus | CMXsrv_comgrl_lee_nom_cor | N/A | N/A |
| fld_obl_rut_acre_lostfocus | CMXsrv_lee_cln | N/A | N/A |
| form_activate | CMXsrv_finobl_busc_acre | N/A | N/A |
| Form_Load | CMXsrv_cmx_get_codes | N/A | N/A |

## PAGCBR
| Segmento | Procedimiento Almacenado | Tablas Referenciadas | Procedimientos Referenciados |
|----------|--------------------------|----------------------|--------------------------|
| Aceptar_Click | CMXsrv_icbr_calc_pag | N/A | N/A |
| ACEPTAR_Click | CMXsrv_icbr_lee_dat_var | N/A | N/A |
| ACEPTAR_Click | CMXsrv_icbr_val_pag | N/A | N/A |
| ACEPTAR_Click | CMXsrv_icbr_ctb_pag | N/A | N/A |
| Calcular_Click | CMXsrv_icbr_cal_pag | N/A | N/A |
| CANCELAR_Click | CMXsrv_icbr_eli_pag | N/A | N/A |
| fld_cbr_cod_des_mn_pag_lostfocus | CMXsrv_val_vig | N/A | N/A |
| fld_cbr_cod_des_mx_pag_lostfocus | CMXsrv_val_vig | N/A | N/A |
| Form_Load | CMXsrv_icbr_lee_cbr0 | N/A | N/A |
| Form_Load | CMXsrv_icbr_obt_mon_nac | N/A | N/A |
| Form_Load | CMXsrv_icbr_lee_dat_pag | N/A | N/A |
| Form_Load | CMXsrv_icbr_pcg_pag | N/A | N/A |
| lee_cta | CMXsrv_vig_lee_cta | N/A | N/A |
| Form_Activate | CMXsrv_icbr_busc_pago | N/A | N/A |
| ACEPTAR_Click | CMXsrv_icbr_val_pag | N/A | N/A |
| Aceptar_Click | CMXsrv_icob_act_val | N/A | N/A |
| Form_Activate | CMXsrv_icob_lee_val | N/A | N/A |
| ELIMINAR_Click | CMXsrv_icbr_eli_int_pago | N/A | N/A |
| Form_Activate | CMXsrv_icbr_busc_int | N/A | N/A |
| Aceptar_Click | CMXsrv_icbr_ingmod_int | N/A | N/A |
| Form_Activate | CMXsrv_icbr_lee_int_pago | N/A | N/A |
| Aceptar_Click | CMXsrv_icbr_lee_bco | N/A | N/A |
| buscar_Click | CMXsrv_icbr_busc_bco | N/A | N/A |
| Form_Load | CMXsrv_grl_fec_serv | N/A | N/A |

## PAGOS
| Segmento | Procedimiento Almacenado | Tablas Referenciadas | Procedimientos Referenciados |
|----------|--------------------------|----------------------|--------------------------|
| buscar_Click | CMXsrv_fincol_bsc_TIP | N/A | N/A |
| CALCULAR_Click | CMXsrv_fincol_efec_calpa | N/A | N/A |
| Contabilizar_Click | CMXsrv_fincol_ictb_pag | N/A | N/A |
| Form_Activate | CMXsrv_fincol_cons_pag | N/A | N/A |
| Form_Load | CMXsrv_fincol_cons_detp | N/A | N/A |
| Aceptar_Click | CMXsrv_fincol_calc_pror | N/A | N/A |
| Contabilizar_Click | CMXsrv_fincol_cont_pror | N/A | N/A |
| Form_Activate | CMXsrv_fincol_cons_pror | N/A | N/A |
| Form_Activate | CMXsrv_fincol_cons_dpror | N/A | N/A |
| Aceptar_Click | CMXsrv_busc_cod_ope | N/A | N/A |
| Aceptar_Click | CMXsrv_col_trae_num_ope | N/A | N/A |
| Aceptar_Click | CMXsrv_fincol_cctb_anu | N/A | N/A |
| Form_Load | CMXsrv_fincol_calc_anu | N/A | N/A |
| Form_Load | CMXsrv_busc_cod_ope | N/A | N/A |
| CALCULAR_Click | CMXsrv_fincol_calc_anu | N/A | N/A |
| Form_Activate | CMXsrv_fincol_cons_anu | N/A | N/A |
| Form_Activate | CMXsrv_fincol_cons_mod | N/A | N/A |
| Form_Activate | CMXsrv_fincol_cons_dmod | N/A | N/A |
| Form_Load | CMXsrv_lee_fpro | N/A | N/A |
| Form_Load | CMXsrv_grl_trae_cod_bco | N/A | N/A |

## PGOEXT
| Segmento | Procedimiento Almacenado | Tablas Referenciadas | Procedimientos Referenciados |
|----------|--------------------------|----------------------|--------------------------|
| calcular_Click | CMXsrv_fincol_cal_pext | N/A | N/A |
| Contabilizar_Click | CMXsrv_busc_cod_ope | N/A | N/A |
| Contabilizar_Click | CMXsrv_fincol_ctb_pext | N/A | N/A |
| calcular_Click | CMXsrv_finobl_cal_pext | N/A | N/A |
| Contabilizar_Click | CMXsrv_finobl_ctb_pext | N/A | N/A |
| Form_Load | CMXsrv_grl_fec_serv | N/A | N/A |
| Form_Load | CMXsrv_lee_fpro | N/A | N/A |

## expdex
| Segmento | Procedimiento Almacenado | Tablas Referenciadas | Procedimientos Referenciados |
|----------|--------------------------|----------------------|--------------------------|
| form_activate | CMXsrv_expcbe_lee_prm | N/A | N/A |
| form_activate | CMXsrv_dex_lee_dex | N/A | N/A |
| Mdexeli_Click | CMXsrv_dex_eli_dex | N/A | N/A |
| ACEPTAR_Click | CMXsrv_dex_act_dex | N/A | N/A |
| fld_dex_dia_plz_max_LostFocus | CMXsrv_expdex_cal_fec | N/A | N/A |
| fld_dex_fec_acep_LostFocus | CMXsrv_expdex_cal_fec | N/A | N/A |
| fld_dex_rut_exp_LostFocus | CMXsrv_dex_lee_cli | N/A | N/A |
| FORM_Load | CMXsrv_dex_lee_dex | N/A | N/A |
| Buscar_Click | CMXsrv_dex_bus_dex | N/A | N/A |
| fld_dex_rut_exp_LostFocus | CMXsrv_dex_lee_cli | N/A | N/A |
| FORM_Load | CMXsrv_grl_fec_serv | N/A | N/A |
| ACEPTAR_Click | CMXsrv_dex_act_dex | N/A | N/A |
| fld_dex_rut_exp_LostFocus | CMXsrv_dex_lee_cli | N/A | N/A |
| FORM_Load | CMXsrv_dex_lee_dex | N/A | N/A |
| COMELIMINAR_Click | CMXsrv_dex_eli_dex | N/A | N/A |
| Form_Activate | CMXsrv_dex_lee_dex | N/A | N/A |

## expret
| Segmento | Procedimiento Almacenado | Tablas Referenciadas | Procedimientos Referenciados |
|----------|--------------------------|----------------------|--------------------------|
| buscar_Click | CMXsrv_busc_plz | N/A | N/A |
| fld_cor_cod_plz_Lostfocus | CMXsrv_lee_plz | N/A | N/A |
| proximos_Click | CMXsrv_busc_plz | N/A | N/A |
| buscar_Click | CMXsrv_cor_busc_pais | N/A | N/A |
| fld_cor_cod_pais_LostFocus | CMXsrv_cor_lee_pais | N/A | N/A |
| proximos_Click | CMXsrv_cor_busc_pais | N/A | N/A |
| Aceptar_Click | CMXsrv_expcbe_lee_cor | N/A | N/A |
| buscar_Click | CMXsrv_expcbe_bus_cor | N/A | N/A |
| proximos_Click | CMXsrv_expcbe_bus_cor | N/A | N/A |
| Command2_Click | CMXsrv_expret_swf_sel | N/A | N/A |
| Form_Load | CMXsrv_grl_fec_serv | N/A | N/A |
| Form_Activate | CMXsrv_cmx_busc_suc_usu | N/A | N/A |
| Form_Activate | CMXsrv_expret_lee_ret | N/A | N/A |
| Form_Load | CMXsrv_expret_lee_prm | N/A | N/A |
| M_cgyc_Click | CMXsrv_expret_avs_cyg1 | N/A | N/A |
| M_cgyc_Click | CMXsrv_expret_avs_cyg2 | N/A | N/A |
| mavisliq_Click | CMXsrv_expret_avs_liq1 | N/A | N/A |
| mavisliq_Click | CMXsrv_expret_avs_liq2 | N/A | N/A |
| mavisliq_Click | CMXsrv_expret_avs_liq3 | N/A | N/A |
| Mcbectb_Click | CMXsrv_expret_val_ret | N/A | N/A |
| Mcbectb_Click | CMXsrv_expret_sum_dtn_mn | N/A | N/A |
| Mcbectb_Click | CMXsrv_expret_ctb_ing | N/A | N/A |
| Mcbedel_Click | CMXsrv_expret_del_ret | N/A | N/A |
| Mliqctb_Click | CMXsrv_expret_avs_adm1 | N/A | N/A |
| Mliqctb_Click | CMXsrv_expret_avs_adm2 | N/A | N/A |
| Mliqctb_Click | CMXsrv_expret_avs_adm3 | N/A | N/A |
| Mvalid_Click | CMXsrv_expret_val_ret | N/A | N/A |
| plv2_Click | CMXsrv_ret_ipuc_gen_pln | N/A | N/A |
| ACEPTAR_Click | CMXsrv_expret_act_tpo_cbo | N/A | N/A |
| ACEPTAR_Click | CMXsrv_expret_val_ret | N/A | N/A |
| ACEPTAR_Click | CMXsrv_expret_cre_ret | N/A | N/A |
| ACEPTAR_Click | CMXsrv_expret_grb_det | N/A | N/A |
| fld_ret_mon_ret_LostFocus | CMXsrv_expret_tpo_cbo | N/A | N/A |
| fld_ret_rut_cli_LostFocus | CMXsrv_expret_lee_cln | N/A | N/A |
| Form_Load | CMXsrv_expret_lee_det | N/A | N/A |
| ELIMINAR_Click | CMXsrv_expret_del_org | N/A | N/A |
| Form_Activate | CMXsrv_expret_bus_org | N/A | N/A |
| ACEPTAR_Click | CMXsrv_expret_grb_org | N/A | N/A |
| Form_Activate | CMXsrv_expret_mto_org | N/A | N/A |
| Form_Activate | CMXsrv_expret_lee_org | N/A | N/A |
| valida_vigente | CMXsrv_vig_lee_cta | N/A | N/A |
| ELIMINAR_Click | CMXsrv_expret_del_dtn | N/A | N/A |
| emitir_Click | CMXsrv_expret_swf_sel | N/A | N/A |
| Form_Activate | CMXsrv_expret_bus_dtn | N/A | N/A |
| Planillas_Click | CMXsrv_ret_ipuc_gen_pln | N/A | N/A |
| ACEPTAR_Click | CMXsrv_expret_grb_dtn | N/A | N/A |
| fld_ret_cod_ben_LostFocus | CMXsrv_expret_lee_cln | N/A | N/A |
| fld_ret_mto_arb_LostFocus | CMXsrv_expret_cal_arb | N/A | N/A |
| fld_ret_mto_ben_LostFocus | CMXsrv_expret_cal_arb | N/A | N/A |
| fld_ret_par_ben_LostFocus | CMXsrv_expret_cal_arb | N/A | N/A |
| Form_Activate | CMXsrv_expret_mto_dtn | N/A | N/A |
| Form_Load | CMXsrv_expret_lee_dtn | N/A | N/A |
| Form_Load | CMXsrv_expret_lee_cln | N/A | N/A |
| buscar_Click | CMXsrv_expret_bus_ret | N/A | N/A |
| fld_ret_rut_cli_LostFocus | CMXsrv_expret_lee_cln | N/A | N/A |
| proxima_Click | CMXsrv_expret_bus_ret | N/A | N/A |
| Command1_Click | CMXsrv_expret_bus_evr | N/A | N/A |
| Form_Activate | CMXsrv_expret_bus_evr | N/A | N/A |
| proximo_Click | CMXsrv_expret_bus_evr | N/A | N/A |
| reversar_Click | CMXsrv_expret_rev_ret | N/A | N/A |
| Form_Load | CMXsrv_expret_lee_evr | N/A | N/A |

