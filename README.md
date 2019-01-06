# CFD-Post-Make-Multiple-Planes-with-For-Statement

!$nplane = 60;
!$iplane = 1;

!for($iplane=1; $iplane <= $nplane; $iplane=$iplane+1)
!{

PLANE: cut$iplane 
  Domain List = fff fluid
  Option = YZ Plane
  X = $iplane/10 
END

!}
