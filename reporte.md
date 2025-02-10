| Productos | Eventos | Botón de Evento | Nombre Técnico del Botón | Función Asociada | Llamado a SP | Nombre Pantalla | Frames asociados | Llamado a Ejecutable |
|-----------|---------|-----------------|--------------------------|------------------|--------------|----------------|-----------------|--------------------|
| COBERIMP | ABRIR |  | ABRIR |  |  | COB00101.FRM |  |  |
| COBERIMP | comgto1 |  | comgto1 |  |  | COB00101.FRM |  |  |
| COBERIMP | CONDICIONES1 |  | CONDICIONES1 |  |  | COB00101.FRM |  |  |
| COBERIMP | CONTABIL1 |  | CONTABIL1 |  |  | COB00101.FRM |  |  |
| COBERIMP | cur_a_pago1 |  | cur_a_pago1 |  |  | COB00101.FRM |  |  |
| COBERIMP | cursar1 |  | cursar1 |  |  | COB00101.FRM |  |  |
| COBERIMP | ddi1 |  | ddi1 |  |  | COB00101.FRM |  |  |
| COBERIMP | DISCREPANCIA1 |  | DISCREPANCIA1 |  |  | COB00101.FRM |  |  |
| COBERIMP | ELIMINAR1 |  | ELIMINAR1 |  |  | COB00101.FRM |  |  |
| COBERIMP | EMBARQUE1 |  | EMBARQUE1 |  |  | COB00101.FRM |  |  |
| COBERIMP | informe1 |  | informe1 |  |  | COB00101.FRM |  |  |
| COBERIMP | MCLIman |  | MCLIman |  |  | COB00101.FRM |  | client.exe |
| COBERIMP | Mcobcur |  | Mcobcur |  | CMXsrv_icob_cur_cob | COB00101.FRM |  |  |
| COBERIMP | Mcobcur_pago |  | Mcobcur_pago |  |  | COB00101.FRM |  |  |
| COBERIMP | Mcobrev |  | Mcobrev |  | CMXsrv_icob_rev_etd | COB00101.FRM |  |  |
| COBERIMP | Mcobvali |  | Mcobvali |  | CMXsrv_icob_val_cob | COB00101.FRM |  |  |
| COBERIMP | Mcomddi |  | Mcomddi |  |  | COB00101.FRM |  | decing.exe |
| COBERIMP | Mcomgto |  | Mcomgto |  |  | COB00101.FRM |  |  |
| COBERIMP | menu_carta_cre |  | menu_carta_cre |  |  | COB00101.FRM |  | import.exe |
| COBERIMP | menu_cob_imp |  | menu_cob_imp |  |  | COB00101.FRM |  | cobranza.exe |
| COBERIMP | menu_coloca |  | menu_coloca |  |  | COB00101.FRM |  | ingreso.exe |
| COBERIMP | menu_inf_imp |  | menu_inf_imp |  |  | COB00101.FRM |  | informe.exe |
| COBERIMP | menu_trapasos |  | menu_trapasos |  |  | COB00101.FRM |  | trscon.exe |
| COBERIMP | MNEGVOL |  | MNEGVOL |  |  | COB00101.FRM |  |  |
| COBERIMP | NUEVA |  | NUEVA |  |  | COB00101.FRM |  |  |
| COBERIMP | PLANPAGO1 |  | PLANPAGO1 |  |  | COB00101.FRM |  |  |
| COBERIMP | reversar1 |  | reversar1 |  |  | COB00101.FRM |  |  |
| COBERIMP | validar1 |  | validar1 |  |  | COB00101.FRM |  |  |
| COBERIMP | VOLVER1 |  | VOLVER1 |  |  | COB00101.FRM |  |  |
| COBERIMP | ACEPTAR |  | ACEPTAR |  |  | COB00201.FRM |  |  |
| COBERIMP | Cancelar |  | Cancelar |  |  | COB00201.FRM |  |  |
| COBERIMP | FLD_AUX_OPC_BUSC |  | FLD_AUX_OPC_BUSC |  |  | COB00201.FRM |  |  |
| COBERIMP | GRID_COB |  | GRID_COB |  |  | COB00201.FRM |  |  |
| COBERIMP | PROXIMAS |  | PROXIMAS |  | CMXsrv_icob_busc_pln | COB00201.FRM |  |  |
| COBERIMP | ACEPTAR |  | ACEPTAR |  | CMXsrv_icob_crea_norm | COB00300.FRM |  |  |
| COBERIMP | Cancelar |  | Cancelar |  |  | COB00300.FRM |  |  |
| COBERIMP | FLD_COB_TIP_OPR |  | FLD_COB_TIP_OPR |  |  | COB00300.FRM |  |  |
| COBERIMP | FLD_COB_TIP_PLN |  | FLD_COB_TIP_PLN |  |  | COB00300.FRM |  |  |
| COBERIMP | fld_glo_pza_inf |  | fld_glo_pza_inf | Dim LT_index As Integer
    Dim LV_A As String
    If (fld_glo_pza_inf.ListIndex < 0) Then
        Beep
    Else
        LT_index = fld_glo_pza_inf.ItemData(fld_glo_pza_inf.ListIndex)
        GG_rsw = VBG_FLD_COB_PZA_INF_Set(GT_fld_glo_pza_inf(LT_index)) |  | COB00300.FRM |  |  |
| COBERIMP | ACEPTAR |  | ACEPTAR |  | CMXsrv_icob_crea_reem | COB00301.FRM |  |  |
| COBERIMP | Cancelar |  | Cancelar |  |  | COB00301.FRM |  |  |
| COBERIMP | ACEPTAR |  | ACEPTAR |  | CMXsrv_icob_act_gral | COB00302.FRM |  |  |
| COBERIMP | Cancelar |  | Cancelar |  |  | COB00302.FRM |  |  |
| COBERIMP | FLD_GLO_FOR_PAG |  | FLD_GLO_FOR_PAG | Dim LT_index As Integer
    Dim LV_A As String
    If (fld_glo_for_pag.ListIndex < 0) Then
        Beep
    Else
        LT_index = fld_glo_for_pag.ItemData(fld_glo_for_pag.ListIndex)
        GG_rsw = VBG_FLD_COB_FOR_PAG_Set(GT_FLD_GLO_FOR_PAG(LT_index)) |  | COB00302.FRM |  |  |
| COBERIMP | FLD_GLO_PAI_PGO |  | FLD_GLO_PAI_PGO | Dim LT_index As Integer
    Dim LV_A As String
    If (FLD_GLO_PAI_PGO.ListIndex < 0) Then
        Beep
    Else
        LT_index = FLD_GLO_PAI_PGO.ItemData(FLD_GLO_PAI_PGO.ListIndex)
        GG_rsw = VBG_FLD_COB_PAI_PGO_Set(GT_FLD_GLO_PAI_PGO(LT_index)) |  | COB00302.FRM |  |  |
| COBERIMP | fld_glo_pza_bcch |  | fld_glo_pza_bcch | Dim LT_index As Integer
    Dim LV_A As String
    If (fld_glo_pza_bcch.ListIndex < 0) Then
        Beep
    Else
        LT_index = fld_glo_pza_bcch.ItemData(fld_glo_pza_bcch.ListIndex)
        GG_rsw = VBG_FLD_COB_PZA_BCCH_Set(GT_fld_glo_pza_bcch(LT_index)) |  | COB00302.FRM |  |  |
| COBERIMP | fld_glo_pza_inf |  | fld_glo_pza_inf | Dim LT_index As Integer
    Dim LV_A As String
    If (fld_glo_pza_inf.ListIndex < 0) Then
        Beep
    Else
        LT_index = fld_glo_pza_inf.ItemData(fld_glo_pza_inf.ListIndex)
        GG_rsw = VBG_FLD_COB_PZA_INF_Set(GT_fld_glo_pza_inf(LT_index)) |  | COB00302.FRM |  |  |
| COBERIMP | fld_glo_tip_doc |  | fld_glo_tip_doc | Dim LT_index As Integer
    Dim LV_A As String
    If (fld_glo_tip_doc.ListIndex < 0) Then
        Beep
    Else
        LT_index = fld_glo_tip_doc.ItemData(fld_glo_tip_doc.ListIndex)
        GG_rsw = VBG_FLD_POS_TIP_DOC_Set(GT_fld_glo_tip_doc(LT_index)) |  | COB00302.FRM |  |  |
| COBERIMP | fld_pos_glo_are_ctb |  | fld_pos_glo_are_ctb | Dim LT_index As Integer
    Dim LV_A As String
    If (fld_pos_glo_are_ctb.ListIndex < 0) Then
        Beep
    Else
        LT_index = fld_pos_glo_are_ctb.ItemData(fld_pos_glo_are_ctb.ListIndex)
        GG_rsw = VBG_FLD_POS_COD_ARE_CTB_Set(GT_fld_pos_glo_are_ctb(LT_index)) |  | COB00302.FRM |  |  |
| COBERIMP | fld_pos_glo_ins_uti |  | fld_pos_glo_ins_uti | Dim LT_index As Integer
    Dim LV_A As String
    If (fld_pos_glo_ins_uti.ListIndex < 0) Then
        Beep
    Else
        LT_index = fld_pos_glo_ins_uti.ItemData(fld_pos_glo_ins_uti.ListIndex)
        GG_rsw = VBG_FLD_POS_COD_INS_UTI_Set(GT_fld_pos_glo_ins_uti(LT_index)) |  | COB00302.FRM |  |  |
| COBERIMP | fld_pos_ind_afe |  | fld_pos_ind_afe |  |  | COB00302.FRM |  |  |
| COBERIMP | ACEPTAR |  | ACEPTAR |  | CMXsrv_icob_act_val | COB00303.FRM |  |  |
| COBERIMP | Cancelar |  | Cancelar |  |  | COB00303.FRM |  |  |
| COBERIMP | FLD_COB_GTO_BAN |  | FLD_COB_GTO_BAN |  |  | COB00303.FRM |  |  |
| COBERIMP | FLD_COB_GTO_HAS_FOB |  | FLD_COB_GTO_HAS_FOB |  |  | COB00303.FRM |  |  |
| COBERIMP | FLD_COB_VAL_FLT |  | FLD_COB_VAL_FLT |  |  | COB00303.FRM |  |  |
| COBERIMP | FLD_COB_VAL_FOB |  | FLD_COB_VAL_FOB |  |  | COB00303.FRM |  |  |
| COBERIMP | FLD_COB_VAL_MER |  | FLD_COB_VAL_MER |  |  | COB00303.FRM |  |  |
| COBERIMP | FLD_COB_VAL_SEG |  | FLD_COB_VAL_SEG |  |  | COB00303.FRM |  |  |
| COBERIMP | FLD_GLO_MON |  | FLD_GLO_MON | Dim LT_index As Integer
    Dim LV_A As String
    If (FLD_GLO_MON.ListIndex < 0) Then
        Beep
    Else
        LT_index = FLD_GLO_MON.ItemData(FLD_GLO_MON.ListIndex)
        GG_rsw = VBG_FLD_COB_MON_Set(GT_FLD_GLO_MON(LT_index)) |  | COB00303.FRM |  |  |
| COBERIMP | ACEPTAR |  | ACEPTAR |  | CMXsrv_icob_act_acu | COB00304.FRM |  |  |
| COBERIMP | Cancelar |  | Cancelar |  |  | COB00304.FRM |  |  |
| COBERIMP | FLD_GLO_ACU1 |  | FLD_GLO_ACU1 | Dim LT_index As Integer
    Dim LV_A As String
    If (FLD_GLO_ACU1.ListIndex < 0) Then
      ' Beep
      Else
       LT_index = FLD_GLO_ACU1.ItemData(FLD_GLO_ACU1.ListIndex)
       GG_rsw = VBG_FLD_COB_COD_ACU1_Set(GT_FLD_GLO_ACU1(LT_index)) |  | COB00304.FRM |  |  |
| COBERIMP | FLD_GLO_ACU2 |  | FLD_GLO_ACU2 | Dim LT_index As Integer
    Dim LV_A As String
    If (FLD_GLO_ACU2.ListIndex < 0) Then
       Beep
      Else
       LT_index = FLD_GLO_ACU2.ItemData(FLD_GLO_ACU2.ListIndex)
       GG_rsw = VBG_FLD_COB_COD_ACU2_Set(GT_FLD_GLO_ACU2(LT_index)) |  | COB00304.FRM |  |  |
| COBERIMP | FLD_GLO_ACU3 |  | FLD_GLO_ACU3 | Dim LT_index As Integer
    Dim LV_A As String
    If (FLD_GLO_ACU3.ListIndex < 0) Then
'      Beep
      Else
       LT_index = FLD_GLO_ACU3.ItemData(FLD_GLO_ACU3.ListIndex)
       GG_rsw = VBG_FLD_COB_COD_ACU3_Set(GT_FLD_GLO_ACU3(LT_index)) |  | COB00304.FRM |  |  |
| COBERIMP | FLD_GLO_ACU4 |  | FLD_GLO_ACU4 | Dim LT_index As Integer
    Dim LV_A As String
    If (FLD_GLO_ACU4.ListIndex < 0) Then
       Beep
      Else
       LT_index = FLD_GLO_ACU4.ItemData(FLD_GLO_ACU4.ListIndex)
       GG_rsw = VBG_FLD_COB_COD_ACU4_Set(GT_FLD_GLO_ACU4(LT_index)) |  | COB00304.FRM |  |  |
| COBERIMP | FLD_GLO_ACU5 |  | FLD_GLO_ACU5 | Dim LT_index As Integer
    Dim LV_A As String
    If (FLD_GLO_ACU5.ListIndex < 0) Then
        Beep
    Else
        LT_index = FLD_GLO_ACU5.ItemData(FLD_GLO_ACU5.ListIndex)
        GG_rsw = VBG_FLD_COB_COD_ACU5_Set(GT_FLD_GLO_ACU5(LT_index)) |  | COB00304.FRM |  |  |
| COBERIMP | ACEPTAR |  | ACEPTAR |  |  | COB00305.FRM |  |  |
| COBERIMP | Cancelar |  | Cancelar |  |  | COB00305.FRM |  |  |
| COBERIMP | ELIMINAR |  | ELIMINAR |  | CMXsrv_icob_eli_int | COB00305.FRM |  |  |
| COBERIMP | GRID_COB |  | GRID_COB |  |  | COB00305.FRM |  |  |
| COBERIMP | NUEVO |  | NUEVO |  |  | COB00305.FRM |  |  |
| COBERIMP | ACEPTAR |  | ACEPTAR |  | CMXsrv_icob_ingmod_int | COB00306.FRM |  |  |
| COBERIMP | Cancelar |  | Cancelar |  |  | COB00306.FRM |  |  |
| COBERIMP | FLD_COB_CAP_INT |  | FLD_COB_CAP_INT |  |  | COB00306.FRM |  |  |
| COBERIMP | FLD_COB_MTO_INT |  | FLD_COB_MTO_INT |  |  | COB00306.FRM |  |  |
| COBERIMP | FLD_COB_TAS_INT_ANL |  | FLD_COB_TAS_INT_ANL |  |  | COB00306.FRM |  |  |
| COBERIMP | FLD_GLO_BASE_TAS |  | FLD_GLO_BASE_TAS |  |  | COB00306.FRM |  |  |
| COBERIMP | FLD_GLO_CPT_INT |  | FLD_GLO_CPT_INT | Dim LT_index As Integer
    Dim LV_A As String
    If (FLD_GLO_CPT_INT.ListIndex < 0) Then
'      Beep
      Else
       LT_index = FLD_GLO_CPT_INT.ItemData(FLD_GLO_CPT_INT.ListIndex)
       gg_rsw = VBG_FLD_COB_CPT_INT_Set(GT_FLD_GLO_CPT_INT(LT_index)) |  | COB00306.FRM |  |  |
| COBERIMP | FLD_GLO_TIP_INT |  | FLD_GLO_TIP_INT | Dim LT_index As Integer
    Dim LV_A As String
    If (FLD_GLO_TIP_INT.ListIndex < 0) Then
       Beep
      Else
       LT_index = FLD_GLO_TIP_INT.ItemData(FLD_GLO_TIP_INT.ListIndex)
       gg_rsw = VBG_FLD_COB_TIP_INT_Set(GT_FLD_GLO_TIP_INT(LT_index)) |  | COB00306.FRM |  |  |
| COBERIMP | ACEPTAR |  | ACEPTAR |  | CMXsrv_icob_ing_mod_srf | COB00307.FRM |  |  |
| COBERIMP | Cancelar |  | Cancelar |  |  | COB00307.FRM |  |  |
| COBERIMP | CmdEliminar |  | CmdEliminar |  | CMXsrv_icob_eli_pln | COB00307.FRM |  |  |
| COBERIMP | CmdReversar |  | CmdReversar |  | CMXsrv_icob_rev_etd | COB00307.FRM |  |  |
| COBERIMP | CURSAR |  | CURSAR |  | CMXsrv_icob_ing_mod_srf | COB00307.FRM |  |  |
| COBERIMP | CyG |  | CyG |  |  | COB00307.FRM |  |  |
| COBERIMP | FLD_COB_VAL_TOT |  | FLD_COB_VAL_TOT |  |  | COB00307.FRM |  |  |
| COBERIMP | FLD_GLO_MON |  | FLD_GLO_MON | Dim LT_index As Integer
    Dim LV_A As String
    If (FLD_GLO_MON.ListIndex < 0) Then
	Beep
    Else
	LT_index = FLD_GLO_MON.ItemData(FLD_GLO_MON.ListIndex)
	GG_rsw = VBG_FLD_COB_MON_Set(GT_FLD_GLO_MON(LT_index)) |  | COB00307.FRM |  |  |
| COBERIMP | FLD_GLO_PAI_PGO |  | FLD_GLO_PAI_PGO | Dim LT_index As Integer
    Dim LV_A As String
    If (fld_glo_pai_pgo.ListIndex < 0) Then
	Beep
    Else
	LT_index = fld_glo_pai_pgo.ItemData(fld_glo_pai_pgo.ListIndex)
	GG_rsw = VBG_FLD_COB_PAI_PGO_Set(GT_FLD_GLO_PAI_PGO(LT_index)) |  | COB00307.FRM |  |  |
| COBERIMP | Reversar |  | Reversar |  | CMXsrv_icob_rev_etd | COB00307.FRM |  |  |
| COBERIMP | ACEPTAR |  | ACEPTAR |  | CMXsrv_icob_anu | COB00501.FRM |  |  |
| COBERIMP | Cancelar |  | Cancelar |  |  | COB00501.FRM |  |  |
| COBERIMP | ACEPTAR |  | ACEPTAR |  | CMXsrv_icob_act_cur_a_pag | COB0601.FRM |  |  |
| COBERIMP | Cancelar |  | Cancelar |  |  | COB0601.FRM |  |  |
| COBERIMP | FLD_AUX_OPC_BUSC |  | FLD_AUX_OPC_BUSC |  |  | COB0601.FRM |  |  |
| COBERIMP | fld_cob_tip_pla |  | fld_cob_tip_pla |  |  | COB0601.FRM |  |  |
| COBERIMP | ACEPTAR |  | ACEPTAR |  | CMXsrv_icob_pag_sop | FORM2.FRM |  |  |
| COBERIMP | Cancelar |  | Cancelar |  |  | FORM2.FRM |  |  |
| COBERIMP | fld_cob_mto2_mn |  | fld_cob_mto2_mn |  |  | FORM2.FRM |  |  |
| COBERIMP | fld_glo_cob_mon_pag |  | fld_glo_cob_mon_pag | Dim LT_index As Integer
    Dim LV_A As String
    If (fld_glo_cob_mon_pag.ListIndex < 0) Then
        Beep
      Else
        LT_index = fld_glo_cob_mon_pag.ItemData(fld_glo_cob_mon_pag.ListIndex)
        GG_rsw = VBG_fld_cob_mon_pag_Set(GT_fld_glo_cob_mon_pag(LT_index)) |  | FORM2.FRM |  |  |
| COBERIMP | fld_glo_cob_odf_mx |  | fld_glo_cob_odf_mx | Dim LT_index As Integer
    Dim LV_A As String

    If (fld_glo_cob_odf_mx.ListIndex < 0) Then
        Beep
    Else
        LT_index = fld_glo_cob_odf_mx.ItemData(fld_glo_cob_odf_mx.ListIndex)
        GG_rsw = VBG_fld_cob_odf_mx_Set(GT_fld_glo_cob_odf_mx(LT_index)) |  | FORM2.FRM |  |  |
| COBERIMP | fld_glo_cob_odf1_mn |  | fld_glo_cob_odf1_mn | Dim LT_index As Integer
    Dim LV_A As String

    If (fld_glo_cob_odf1_mn.ListIndex < 0) Then
        Beep
    Else
        LT_index = fld_glo_cob_odf1_mn.ItemData(fld_glo_cob_odf1_mn.ListIndex)
        GG_rsw = VBG_fld_cob_odf1_mn_Set(GT_fld_glo_cob_odf1_mn(LT_index)) |  | FORM2.FRM |  |  |
| COBERIMP | fld_glo_cob_odf2_mn |  | fld_glo_cob_odf2_mn | Dim LT_index As Integer
    Dim LV_A As String

    If (fld_glo_cob_odf2_mn.ListIndex < 0) Then
        Beep
    Else
        LT_index = fld_glo_cob_odf2_mn.ItemData(fld_glo_cob_odf2_mn.ListIndex)
        GG_rsw = VBG_fld_cob_odf2_mn_Set(GT_fld_glo_cob_odf2_mn(LT_index)) |  | FORM2.FRM |  |  |
| COBERIMP | Command1 |  | Command1 |  |  | GRL00101.FRM |  |  |
| COBERIMP | ELIMINAR |  | ELIMINAR |  |  | GRL00101.FRM |  |  |
| COBERIMP | word |  | word |  |  | GRL00101.FRM |  |  |
| COBERIMP | ACEPTAR |  | ACEPTAR |  |  | INFORMES.FRM |  | supda.exe |
| COBERIMP | Cancelar |  | Cancelar |  |  | INFORMES.FRM |  |  |
| COBERIMP | Command3D1 |  | Command3D1 |  |  | INFORMES.FRM |  |  |
| COBERIMP | Option3D1 |  | Option3D1 |  |  | INFORMES.FRM |  |  |
| COBERIMP | Procesos |  | Procesos |  |  | INFORMES.FRM |  | supda.exe |
| COBERIMP | ACEPTAR |  | ACEPTAR |  | CMXsrv_icob_cur_reem | ORI_DEST.FRM |  |  |
| COBERIMP | Cancelar |  | Cancelar |  |  | ORI_DEST.FRM |  |  |
| COBERIMP | fld_glo_cob_odf1_mn |  | fld_glo_cob_odf1_mn | Dim LT_index As Integer
    Dim LV_A As String

    If (fld_glo_cob_odf1_mn.ListIndex < 0) Then
        Beep
    Else
        LT_index = fld_glo_cob_odf1_mn.ItemData(fld_glo_cob_odf1_mn.ListIndex)
        GG_rsw = VBG_fld_cob_odf1_mn_Set(GT_fld_glo_cob_odf1_mn(LT_index)) |  | ORI_DEST.FRM |  |  |
| COBERIMP | ACEPTAR |  | ACEPTAR |  |  | PREFER.FRM |  |  |
| COBERIMP | Cancelar |  | Cancelar |  |  | PREFER.FRM |  |  |
| COBERIMP | Cargar |  | Cargar |  |  | PREFER.FRM |  |  |
| COBERIMP | Cancelar |  | Cancelar |  |  | PREGUNTA.FRM |  |  |
| COBERIMP | contabilizar |  | contabilizar |  |  | PREGUNTA.FRM |  |  |
| COBERIMP | pregunta |  | pregunta |  |  | PREGUNTA.FRM |  |  |
| COBERIMP | sin_contabilizar |  | sin_contabilizar |  |  | PREGUNTA.FRM |  |  |
