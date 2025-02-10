| Productos | Eventos | Botón de Evento | Nombre Técnico del Botón | Función Asociada | Llamado a SP | Nombre Pantalla | Frames asociados | Llamado a Ejecutable |
|-----------|---------|-----------------|--------------------------|------------------|--------------|----------------|-----------------|--------------------|
| OBLIGA | aceptar |  | aceptar |  |  | COL00108.FRM |  |  |
| OBLIGA | buscar |  | buscar |  | CMXsrv_fincol_bsc_tip | COL00108.FRM |  |  |
| OBLIGA | cancelar |  | cancelar |  |  | COL00108.FRM |  |  |
| OBLIGA | fld_col_cod_bal |  | fld_col_cod_bal |  |  | COL00108.FRM |  |  |
| OBLIGA | FLD_GLO_TIP_CRE |  | FLD_GLO_TIP_CRE | Dim LT_index As Integer
    Dim LV_A As String
    If (fld_glo_tip_cre.ListIndex < 0) Then
        Beep
    Else
        LT_index = fld_glo_tip_cre.ItemData(fld_glo_tip_cre.ListIndex)
        GG_rsw = VBG_FLD_COD_TIP_CRE_Set(GT_FLD_glo_tip_cre(LT_index)) |  | COL00108.FRM |  |  |
| OBLIGA | GRID_TIPOPE |  | GRID_TIPOPE |  |  | COL00108.FRM |  |  |
| OBLIGA | Proxima |  | Proxima |  | CMXsrv_fincol_bsc_tip | COL00108.FRM |  |  |
| OBLIGA | proximo |  | proximo |  | CMXsrv_fincol_bsc_tip | COL00108.FRM |  |  |
| OBLIGA | Aceptar |  | Aceptar |  |  | CRD00602.FRM |  |  |
| OBLIGA | buscar |  | buscar |  | CMXsrv_finobl_bus_cor | CRD00602.FRM |  |  |
| OBLIGA | Cancelar |  | Cancelar |  |  | CRD00602.FRM |  |  |
| OBLIGA | fld_aux_glo_pai |  | fld_aux_glo_pai | Dim LT_index As Integer
    Dim LV_A As String
    If (fld_aux_glo_pai.ListIndex < 0) Then
	Beep
    Else
	LT_index = fld_aux_glo_pai.ItemData(fld_aux_glo_pai.ListIndex)
	GG_rsw = VBG_FLD_AUX_COD_PAI_Set(GT_FLD_AUX_GLO_PAI(LT_index)) |  | CRD00602.FRM |  |  |
| OBLIGA | fld_aux_glo_plz |  | fld_aux_glo_plz | Dim LT_index As Integer
    Dim LV_A As String
    If (fld_aux_glo_plz.ListIndex < 0) Then
	Beep
    Else
	LT_index = fld_aux_glo_plz.ItemData(fld_aux_glo_plz.ListIndex)
	GG_rsw = VBG_fld_aux_cod_plz_Set(GT_FLD_AUX_GLO_PLZ(LT_index)) |  | CRD00602.FRM |  |  |
| OBLIGA | FLD_INDICA_SW |  | FLD_INDICA_SW |  |  | CRD00602.FRM |  |  |
| OBLIGA | GRID_CORR |  | GRID_CORR |  |  | CRD00602.FRM |  |  |
| OBLIGA | proximo |  | proximo |  | CMXsrv_finobl_bus_cor | CRD00602.FRM |  |  |
| OBLIGA | sw_pais |  | sw_pais |  |  | CRD00602.FRM |  |  |
| OBLIGA | sw_plaza |  | sw_plaza |  |  | CRD00602.FRM |  |  |
| OBLIGA | sw_todas |  | sw_todas |  |  | CRD00602.FRM |  |  |
| OBLIGA | Command1 |  | Command1 |  |  | GRL00101.FRM |  |  |
| OBLIGA | ELIMINAR |  | ELIMINAR |  |  | GRL00101.FRM |  |  |
| OBLIGA | word |  | word |  |  | GRL00101.FRM |  |  |
| OBLIGA | aceptar |  | aceptar |  |  | INFORMES.FRM |  | supda.exe |
| OBLIGA | cancelar |  | cancelar |  |  | INFORMES.FRM |  |  |
| OBLIGA | Command3D1 |  | Command3D1 |  |  | INFORMES.FRM |  |  |
| OBLIGA | Option3D1 |  | Option3D1 |  |  | INFORMES.FRM |  |  |
| OBLIGA | Procesos |  | Procesos |  |  | INFORMES.FRM |  | supda.exe |
| OBLIGA | aceptar |  | aceptar |  |  | OBL00101.FRM |  |  |
| OBLIGA | cancelar |  | cancelar |  |  | OBL00101.FRM |  |  |
| OBLIGA | fld_aux_nom_mon |  | fld_aux_nom_mon | Dim LT_index As Integer
    Dim LV_A As String

    If (fld_aux_nom_mon.ListIndex < 0) Then
        Beep
    Else
        LT_index = fld_aux_nom_mon.ItemData(fld_aux_nom_mon.ListIndex)
        gg_rsw = VBG_fld_obl_mon_Set(GT_fld_aux_nom_mon(LT_index)) |  | OBL00101.FRM |  |  |
| OBLIGA | fld_aux_nom_mon_ori |  | fld_aux_nom_mon_ori | Dim LT_index As Integer
    Dim LV_A As String

    If (fld_aux_nom_mon_ori.ListIndex < 0) Then
        Beep
    Else
        LT_index = fld_aux_nom_mon_ori.ItemData(fld_aux_nom_mon_ori.ListIndex)
        gg_rsw = VBG_fld_obl_mon_reem_Set(GT_fld_aux_nom_mon_ori(LT_index)) |  | OBL00101.FRM |  |  |
| OBLIGA | fld_obl_mod_pag |  | fld_obl_mod_pag |  |  | OBL00101.FRM |  |  |
| OBLIGA | fld_obl_mto_ori |  | fld_obl_mto_ori |  |  | OBL00101.FRM |  |  |
| OBLIGA | fld_obl_rut_acre |  | fld_obl_rut_acre |  |  | OBL00101.FRM |  |  |
| OBLIGA | fld_obl_tip_ope |  | fld_obl_tip_ope |  |  | OBL00101.FRM |  |  |
| OBLIGA | fld_par_nom_suc |  | fld_par_nom_suc | Dim LT_index As Integer
    Dim LV_A As String

    If (fld_par_nom_suc.ListIndex < 0) Then
        Beep
    Else
        LT_index = fld_par_nom_suc.ItemData(fld_par_nom_suc.ListIndex)
        gg_rsw = VBG_fld_obl_suc_Set(GT_fld_par_nom_suc(LT_index)) |  | OBL00101.FRM |  |  |
| OBLIGA | FLD_PAR_NOM_TIP_TAS |  | FLD_PAR_NOM_TIP_TAS | Dim LT_index As Integer
    Dim LV_A As String
    Dim iFilas As Integer
    Dim arglist As MIGPrmModalidadPagoDiaType

    If (FLD_PAR_NOM_TIP_TAS.ListIndex < 0) Then
        Beep
    Else
        LT_index = FLD_PAR_NOM_TIP_TAS.ItemData(FLD_PAR_NOM_TIP_TAS.ListIndex)
        gg_rsw = VBG_fld_obl_tip_tas_Set(GT_FLD_PAR_NOM_TIP_TAS(LT_index))

        If GT_FLD_PAR_TAS_INT(LT_index) = "S" Then
           If GT_FLD_PAR_IND_DIA(LT_index) = "N" Then
              fld_obl_mod_bas_dia.ListIndex = 0
              'fld_obl_mod_bas_dia.Enabled = True
              
              arglist.fld_obl_tip_tas = RTrim(gv_fld_obl_tip_tas)
              
              rsw% = PrmModalidadPagoDia(gserver, arglist)
              
              If rsw% <> mig_succeed Then  ' Or GV_ERROR = 43003 Then
                 Screen.MousePointer = 0
                 Exit Sub |  | OBL00101.FRM |  |  |
| OBLIGA | cancelar |  | cancelar |  |  | OBL00102.FRM |  |  |
| OBLIGA | ELIMINAR |  | ELIMINAR |  | CMXsrv_finobl_ecuo | OBL00102.FRM |  |  |
| OBLIGA | generar |  | generar |  |  | OBL00102.FRM |  |  |
| OBLIGA | grid_inf |  | grid_inf |  |  | OBL00102.FRM |  |  |
| OBLIGA | ingresar |  | ingresar |  |  | OBL00102.FRM |  |  |
| OBLIGA | anunctb |  | anunctb |  | CMXsrv_finobl_calc_anu | OBL00103.FRM |  |  |
| OBLIGA | avi_otor |  | avi_otor |  |  | OBL00103.FRM |  |  |
| OBLIGA | avi_pago |  | avi_pago |  |  | OBL00103.FRM |  |  |
| OBLIGA | Comabrir |  | Comabrir |  |  | OBL00103.FRM |  |  |
| OBLIGA | COMANULAR |  | COMANULAR |  |  | OBL00103.FRM |  |  |
| OBLIGA | COMAPROBADA |  | COMAPROBADA |  |  | OBL00103.FRM |  |  |
| OBLIGA | COMASIGNAR |  | COMASIGNAR |  |  | OBL00103.FRM |  |  |
| OBLIGA | COMCESI1 |  | COMCESI1 |  |  | OBL00103.FRM |  |  |
| OBLIGA | COMCONDICIONES |  | COMCONDICIONES |  |  | OBL00103.FRM |  |  |
| OBLIGA | COMCTB |  | COMCTB |  |  | OBL00103.FRM |  |  |
| OBLIGA | comEliminar |  | comEliminar |  |  | OBL00103.FRM |  |  |
| OBLIGA | COMEMBARQUE |  | COMEMBARQUE |  |  | OBL00103.FRM |  |  |
| OBLIGA | COMENDOSAR |  | COMENDOSAR |  |  | OBL00103.FRM |  |  |
| OBLIGA | COMGTO1 |  | COMGTO1 |  |  | OBL00103.FRM |  |  |
| OBLIGA | Command3D1 |  | Command3D1 |  |  | OBL00103.FRM |  |  |
| OBLIGA | Command3D5 |  | Command3D5 |  |  | OBL00103.FRM |  |  |
| OBLIGA | COMNOASIG |  | COMNOASIG |  |  | OBL00103.FRM |  |  |
| OBLIGA | Comnueva |  | Comnueva |  |  | OBL00103.FRM |  |  |
| OBLIGA | compag |  | compag |  |  | OBL00103.FRM |  |  |
| OBLIGA | COMQUIT |  | COMQUIT |  |  | OBL00103.FRM |  |  |
| OBLIGA | Comrevers |  | Comrevers |  |  | OBL00103.FRM |  |  |
| OBLIGA | COMVOLVER |  | COMVOLVER |  |  | OBL00103.FRM |  |  |
| OBLIGA | ffcorr |  | ffcorr |  |  | OBL00103.FRM |  | corres.exe |
| OBLIGA | Mcbeabr |  | Mcbeabr |  |  | OBL00103.FRM |  |  |
| OBLIGA | Mcbeanl |  | Mcbeanl |  | CMXsrv_finobl_calc_anu | OBL00103.FRM |  |  |
| OBLIGA | Mcbectb |  | Mcbectb |  | CMXsrv_finobl_ctb_oto | OBL00103.FRM |  | comgto.exe |
| OBLIGA | Mcbedel |  | Mcbedel |  | CMXsrv_fincol_eli_obl | OBL00103.FRM |  |  |
| OBLIGA | Mcbevol |  | Mcbevol |  |  | OBL00103.FRM |  |  |
| OBLIGA | mcesi |  | mcesi |  |  | OBL00103.FRM |  |  |
| OBLIGA | MCOMIGAS |  | MCOMIGAS |  |  | OBL00103.FRM |  | comgto.exe |
| OBLIGA | MCRD |  | MCRD |  |  | OBL00103.FRM |  |  |
| OBLIGA | Mexpcrd |  | Mexpcrd |  |  | OBL00103.FRM |  | import.exe |
| OBLIGA | Mfnccol |  | Mfnccol |  |  | OBL00103.FRM |  | ingreso.exe |
| OBLIGA | Minfo |  | Minfo |  |  | OBL00103.FRM |  |  |
| OBLIGA | Mobl_liq_ope |  | Mobl_liq_ope |  | CMXsrv_icrd_dat_liq_ope | OBL00103.FRM |  |  |
| OBLIGA | Mobl_proce |  | Mobl_proce |  |  | OBL00103.FRM |  |  |
| OBLIGA | MOblRel |  | MOblRel |  |  | OBL00103.FRM |  |  |
| OBLIGA | Mproce |  | Mproce |  |  | OBL00103.FRM |  |  |
| OBLIGA | Mtabtra |  | Mtabtra |  |  | OBL00103.FRM |  | trscon.exe |
| OBLIGA | pagoextra |  | pagoextra |  |  | OBL00103.FRM |  | pgoext.exe |
| OBLIGA | pertas |  | pertas |  |  | OBL00103.FRM |  | pertas.exe |
| OBLIGA | pgoext1 |  | pgoext1 |  |  | OBL00103.FRM |  |  |
| OBLIGA | valida1 |  | valida1 |  |  | OBL00103.FRM |  |  |
| OBLIGA | aceptar |  | aceptar |  |  | OBL00104.FRM |  |  |
| OBLIGA | buscar |  | buscar |  | CMXsrv_finobl_bsc_obl | OBL00104.FRM |  |  |
| OBLIGA | cancelar |  | cancelar |  |  | OBL00104.FRM |  |  |
| OBLIGA | fld_obl_nom_suc |  | fld_obl_nom_suc | Dim LT_index As Integer
    Dim LV_A As String

    If (fld_obl_nom_suc.ListIndex < 0) Then
        Beep
    Else
        LT_index = fld_obl_nom_suc.ItemData(fld_obl_nom_suc.ListIndex)
        GG_rsw = VBG_fld_obl_bus_suc_Set(GT_fld_obl_nom_suc(LT_index)) |  | OBL00104.FRM |  |  |
| OBLIGA | fld_obl_tip_ope |  | fld_obl_tip_ope |  |  | OBL00104.FRM |  |  |
| OBLIGA | grid_inf |  | grid_inf |  |  | OBL00104.FRM |  |  |
| OBLIGA | opcion |  | opcion |  | CMXsrv_lee_opcion | OBL00104.FRM |  |  |
| OBLIGA | Proxima |  | Proxima |  | CMXsrv_finobl_bsc_obl | OBL00104.FRM |  |  |
| OBLIGA | cancelar |  | cancelar |  |  | OBL00112.FRM |  |  |
| OBLIGA | generar |  | generar |  |  | OBL00112.FRM |  |  |
| OBLIGA | aceptar |  | aceptar |  |  | OBL00122.FRM |  |  |
| OBLIGA | cancelar |  | cancelar |  |  | OBL00122.FRM |  |  |
| OBLIGA | calcular |  | calcular |  |  | OBL00201.FRM |  |  |
| OBLIGA | cancelar |  | cancelar |  |  | OBL00201.FRM |  |  |
| OBLIGA | fld_aux_nom_mon_ori |  | fld_aux_nom_mon_ori | Dim LT_index As Integer
    Dim LV_A As String
    If (fld_aux_nom_mon_ori.ListIndex < 0) Then
        Beep
    Else
        LT_index = fld_aux_nom_mon_ori.ItemData(fld_aux_nom_mon_ori.ListIndex)
        gg_rsw = VBG_fld_obl_mon_pag_Set(GT_fld_aux_nom_mon_ori(LT_index)) |  | OBL00201.FRM |  |  |
| OBLIGA | fld_aux_sw_for_pag |  | fld_aux_sw_for_pag |  |  | OBL00201.FRM |  |  |
| OBLIGA | fld_aux_sw_ind_pag |  | fld_aux_sw_ind_pag |  |  | OBL00201.FRM |  |  |
| OBLIGA | fld_obl_mto_pag |  | fld_obl_mto_pag |  |  | OBL00201.FRM |  |  |
| OBLIGA | cancelar |  | cancelar |  |  | OBL00202.FRM |  |  |
| OBLIGA | contabilizar |  | contabilizar |  | CMXsrv_finobl_ictb_pag | OBL00202.FRM |  | comgto.exe |
| OBLIGA | fld_obl_mto_int_pac |  | fld_obl_mto_int_pac |  |  | OBL00202.FRM |  |  |
| OBLIGA | fld_obl_mto_pag |  | fld_obl_mto_pag |  |  | OBL00202.FRM |  |  |
| OBLIGA | cancelar |  | cancelar |  |  | OBL00203.FRM |  |  |
| OBLIGA | grid_inf |  | grid_inf |  |  | OBL00203.FRM |  |  |
| OBLIGA | nuevo |  | nuevo |  |  | OBL00203.FRM |  |  |
| OBLIGA | cancelar |  | cancelar |  |  | OBL00204.FRM |  |  |
| OBLIGA | fld_obl_cap_pag |  | fld_obl_cap_pag |  |  | OBL00204.FRM |  |  |
| OBLIGA | fld_obl_mto_int_pac |  | fld_obl_mto_int_pac |  |  | OBL00204.FRM |  |  |
| OBLIGA | fld_obl_mto_tot_pag_mori |  | fld_obl_mto_tot_pag_mori |  |  | OBL00204.FRM |  |  |
| OBLIGA | fld_obl_sdo_cuo |  | fld_obl_sdo_cuo |  |  | OBL00204.FRM |  |  |
| OBLIGA | calcular |  | calcular |  | CMXsrv_finobl_calc_pror | OBL00301.FRM |  |  |
| OBLIGA | cancelar |  | cancelar |  |  | OBL00301.FRM |  |  |
| OBLIGA | cancelar |  | cancelar |  |  | OBL00302.FRM |  |  |
| OBLIGA | contabilizar |  | contabilizar |  |  | OBL00302.FRM |  |  |
| OBLIGA | fld_obl_int_pag |  | fld_obl_int_pag |  |  | OBL00302.FRM |  |  |
| OBLIGA | fld_obl_mod_pag |  | fld_obl_mod_pag |  |  | OBL00302.FRM |  |  |
| OBLIGA | FLD_PAR_NOM_TIP_TAS |  | FLD_PAR_NOM_TIP_TAS | Dim LT_index As Integer
    Dim LV_A As String
    Dim iFilas As Integer
    Dim arglist As MIGPrmModalidadPagoDiaType

    If (FLD_PAR_NOM_TIP_TAS.ListIndex < 0) Then
	Beep
    Else
	LT_index = FLD_PAR_NOM_TIP_TAS.ItemData(FLD_PAR_NOM_TIP_TAS.ListIndex)
	gg_rsw = VBG_fld_aux_tip_tas_pror_Set(GT_FLD_PAR_NOM_TIP_TAS(LT_index))

	If GT_FLD_PAR_TAS_INT(LT_index) = "S" Then
	   If GT_FLD_PAR_IND_DIA(LT_index) = "N" Then
	      fld_obl_mod_bas_dia.ListIndex = 0
	      'fld_obl_mod_bas_dia.Enabled = True

	      arglist.fld_obl_tip_tas = RTrim(fld_aux_tip_tas_pror)   'RTrim(gv_fld_obl_tip_tas)
	      
	      rsw% = PrmModalidadPagoDia(gserver, arglist)
	      
	      If rsw% <> mig_succeed Then  ' Or GV_ERROR = 43003 Then
		 Screen.MousePointer = 0
		 Exit Sub |  | OBL00302.FRM |  |  |
| OBLIGA | cancelar |  | cancelar |  |  | OBL00303.FRM |  |  |
| OBLIGA | grid_inf |  | grid_inf |  |  | OBL00303.FRM |  |  |
| OBLIGA | nuevo |  | nuevo |  |  | OBL00303.FRM |  |  |
| OBLIGA | cancelar |  | cancelar |  |  | OBL00304.FRM |  |  |
| OBLIGA | fld_par_nom_tip_tas |  | fld_par_nom_tip_tas | Dim LT_index As Integer
    Dim LV_A As String
    If (fld_par_nom_tip_tas.ListIndex < 0) Then
        Beep
    Else
        LT_index = fld_par_nom_tip_tas.ItemData(fld_par_nom_tip_tas.ListIndex)
        GG_rsw = VBG_fld_aux_tip_tas_pror_Set(GT_fld_par_nom_tip_tas(LT_index)) |  | OBL00304.FRM |  |  |
| OBLIGA | cancelar |  | cancelar |  |  | OBL00401.FRM |  |  |
| OBLIGA | contabilizar |  | contabilizar |  | CMXsrv_finobl_ctb_anu | OBL00401.FRM |  |  |
| OBLIGA | fld_obl_cap_pag |  | fld_obl_cap_pag |  |  | OBL00401.FRM |  |  |
| OBLIGA | fld_obl_int_pag |  | fld_obl_int_pag |  |  | OBL00401.FRM |  |  |
| OBLIGA | calcular |  | calcular |  | CMXsrv_finobl_calc_anu | OBL00402.FRM |  |  |
| OBLIGA | cancelar |  | cancelar |  |  | OBL00402.FRM |  |  |
| OBLIGA | fld_obl_int_pag |  | fld_obl_int_pag |  |  | OBL00402.FRM |  |  |
| OBLIGA | fld_obl_mto_pag |  | fld_obl_mto_pag |  |  | OBL00402.FRM |  |  |
| OBLIGA | aceptar |  | aceptar |  |  | OBL00501.FRM |  |  |
| OBLIGA | cancelar |  | cancelar |  |  | OBL00501.FRM |  |  |
| OBLIGA | fld_aux_nom_mon_ori |  | fld_aux_nom_mon_ori | Dim LT_index As Integer
    Dim LV_A As String

    If (fld_aux_nom_mon_ori.ListIndex < 0) Then
        Beep
    Else
        LT_index = fld_aux_nom_mon_ori.ItemData(fld_aux_nom_mon_ori.ListIndex)
        gg_rsw = VBG_fld_obl_mon_reem_Set(GT_fld_aux_nom_mon_ori(LT_index)) |  | OBL00501.FRM |  |  |
| OBLIGA | fld_obl_mod_pag |  | fld_obl_mod_pag |  |  | OBL00501.FRM |  |  |
| OBLIGA | fld_obl_mto_ori |  | fld_obl_mto_ori |  |  | OBL00501.FRM |  |  |
| OBLIGA | FLD_PAR_NOM_TIP_TAS |  | FLD_PAR_NOM_TIP_TAS | Dim LT_index As Integer
    Dim LV_A As String
    Dim iFilas As Integer
    Dim arglist As MIGPrmModalidadPagoDiaType

    If (FLD_PAR_NOM_TIP_TAS.ListIndex < 0) Then
        Beep
    Else
        LT_index = FLD_PAR_NOM_TIP_TAS.ItemData(FLD_PAR_NOM_TIP_TAS.ListIndex)
        gg_rsw = VBG_fld_obl_tip_tas_Set(GT_FLD_PAR_NOM_TIP_TAS(LT_index))

        If GT_FLD_PAR_TAS_INT(LT_index) = "S" Then
           If GT_FLD_PAR_IND_DIA(LT_index) = "N" Then
              arglist.fld_obl_tip_tas = RTrim(gv_fld_obl_tip_tas)

              rsw% = PrmModalidadPagoDia(gserver, arglist)
              
              If rsw% <> mig_succeed Then  ' Or GV_ERROR = 43003 Then
                 Screen.MousePointer = 0
                 Exit Sub |  | OBL00501.FRM |  |  |
| OBLIGA | cancelar |  | cancelar |  |  | OBL00502.FRM |  |  |
| OBLIGA | grid_inf |  | grid_inf |  |  | OBL00502.FRM |  |  |
| OBLIGA | nueva |  | nueva |  |  | OBL00502.FRM |  |  |
| OBLIGA | cancelar |  | cancelar |  |  | OBL00503.FRM |  |  |
| OBLIGA | fld_obl_mto_cap_ori |  | fld_obl_mto_cap_ori |  |  | OBL00503.FRM |  |  |
| OBLIGA | cancelar |  | cancelar |  |  | OBL00601.FRM |  |  |
| OBLIGA | efectuar |  | efectuar |  | CMXsrv_finobl_rev_eve | OBL00601.FRM |  |  |
| OBLIGA | grid_inf |  | grid_inf |  |  | OBL00601.FRM |  |  |
| OBLIGA | cancelar |  | cancelar |  |  | OBL00602.FRM |  |  |
| OBLIGA | fld_obl_mto_cap_ori |  | fld_obl_mto_cap_ori |  |  | OBL00602.FRM |  |  |
| OBLIGA | cancelar |  | cancelar |  |  | OBL00701.FRM |  |  |
| OBLIGA | ELIMINAR |  | ELIMINAR |  | CMXsrv_finobl_eli_ctr | OBL00701.FRM |  |  |
| OBLIGA | grid_oblcol |  | grid_oblcol |  |  | OBL00701.FRM |  |  |
| OBLIGA | nuevo |  | nuevo |  |  | OBL00701.FRM |  |  |
| OBLIGA | cancelar |  | cancelar |  |  | OBL00702.FRM |  |  |
| OBLIGA | nuevo |  | nuevo |  | CMXsrv_finobl_ing_ctr | OBL00702.FRM |  |  |
| OBLIGA | aceptar |  | aceptar |  | CMXsrv_finobl_cesion_obl | OBL130.FRM |  |  |
| OBLIGA | cancelar |  | cancelar |  |  | OBL130.FRM |  |  |
| OBLIGA | aceptar |  | aceptar |  |  | PREFER.FRM |  |  |
| OBLIGA | cancelar |  | cancelar |  |  | PREFER.FRM |  |  |
| OBLIGA | Cargar |  | Cargar |  |  | PREFER.FRM |  |  |
