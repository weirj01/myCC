# SPDX-License-Identifier: MIT
# Copyright © Andy Maloney <asmaloney@gmail.com>

target_sources( ${PROJECT_NAME}
	PRIVATE
		${CMAKE_CURRENT_LIST_DIR}/AutoSegmentationTools.h
		${CMAKE_CURRENT_LIST_DIR}/BoundingBox.h
		${CMAKE_CURRENT_LIST_DIR}/CCConst.h
		${CMAKE_CURRENT_LIST_DIR}/CCCoreLib.h
		${CMAKE_CURRENT_LIST_DIR}/CCGeom.h
		${CMAKE_CURRENT_LIST_DIR}/CCMath.h
		${CMAKE_CURRENT_LIST_DIR}/CCMiscTools.h
		${CMAKE_CURRENT_LIST_DIR}/CCPlatform.h
		${CMAKE_CURRENT_LIST_DIR}/CCShareable.h
		${CMAKE_CURRENT_LIST_DIR}/CCToolbox.h
		${CMAKE_CURRENT_LIST_DIR}/CCTypes.h
		${CMAKE_CURRENT_LIST_DIR}/ChamferDistanceTransform.h
		${CMAKE_CURRENT_LIST_DIR}/CloudSamplingTools.h
		${CMAKE_CURRENT_LIST_DIR}/ConjugateGradient.h
		${CMAKE_CURRENT_LIST_DIR}/Delaunay2dMesh.h
		${CMAKE_CURRENT_LIST_DIR}/DgmOctree.h
		${CMAKE_CURRENT_LIST_DIR}/DgmOctreeReferenceCloud.h
		${CMAKE_CURRENT_LIST_DIR}/DistanceComputationTools.h
		${CMAKE_CURRENT_LIST_DIR}/ErrorFunction.h
		${CMAKE_CURRENT_LIST_DIR}/FastMarching.h
		${CMAKE_CURRENT_LIST_DIR}/FastMarchingForPropagation.h
		${CMAKE_CURRENT_LIST_DIR}/Garbage.h
		${CMAKE_CURRENT_LIST_DIR}/GenericCloud.h
		${CMAKE_CURRENT_LIST_DIR}/GenericDistribution.h
		${CMAKE_CURRENT_LIST_DIR}/GenericIndexedCloud.h
		${CMAKE_CURRENT_LIST_DIR}/GenericIndexedCloudPersist.h
		${CMAKE_CURRENT_LIST_DIR}/GenericIndexedMesh.h
		${CMAKE_CURRENT_LIST_DIR}/GenericMesh.h
		${CMAKE_CURRENT_LIST_DIR}/GenericOctree.h
		${CMAKE_CURRENT_LIST_DIR}/GenericProgressCallback.h
		${CMAKE_CURRENT_LIST_DIR}/GenericTriangle.h
		${CMAKE_CURRENT_LIST_DIR}/GeometricalAnalysisTools.h
		${CMAKE_CURRENT_LIST_DIR}/Grid3D.h
		${CMAKE_CURRENT_LIST_DIR}/GridAndMeshIntersection.h
		${CMAKE_CURRENT_LIST_DIR}/Jacobi.h
		${CMAKE_CURRENT_LIST_DIR}/KdTree.h
		${CMAKE_CURRENT_LIST_DIR}/Kriging.h
		${CMAKE_CURRENT_LIST_DIR}/LocalModel.h
		${CMAKE_CURRENT_LIST_DIR}/ManualSegmentationTools.h
		${CMAKE_CURRENT_LIST_DIR}/MathTools.h
		${CMAKE_CURRENT_LIST_DIR}/MeshSamplingTools.h
		${CMAKE_CURRENT_LIST_DIR}/Neighbourhood.h
		${CMAKE_CURRENT_LIST_DIR}/NormalDistribution.h
		${CMAKE_CURRENT_LIST_DIR}/ParallelSort.h
		${CMAKE_CURRENT_LIST_DIR}/PointCloud.h
		${CMAKE_CURRENT_LIST_DIR}/PointCloudTpl.h
		${CMAKE_CURRENT_LIST_DIR}/PointProjectionTools.h
		${CMAKE_CURRENT_LIST_DIR}/Polyline.h
		${CMAKE_CURRENT_LIST_DIR}/RayAndBox.h
		${CMAKE_CURRENT_LIST_DIR}/ReferenceCloud.h
		${CMAKE_CURRENT_LIST_DIR}/RegistrationTools.h
		${CMAKE_CURRENT_LIST_DIR}/SaitoSquaredDistanceTransform.h
		${CMAKE_CURRENT_LIST_DIR}/ScalarField.h
		${CMAKE_CURRENT_LIST_DIR}/ScalarFieldTools.h
		${CMAKE_CURRENT_LIST_DIR}/SimpleMesh.h
		${CMAKE_CURRENT_LIST_DIR}/SimpleTriangle.h
		${CMAKE_CURRENT_LIST_DIR}/SquareMatrix.h
		${CMAKE_CURRENT_LIST_DIR}/StatisticalTestingTools.h
		${CMAKE_CURRENT_LIST_DIR}/TrueKdTree.h
		${CMAKE_CURRENT_LIST_DIR}/WeibullDistribution.h
)

install(
	FILES
		AutoSegmentationTools.h
		BoundingBox.h
		CCConst.h
		CCCoreLib.h
		CCGeom.h
		CCMath.h
		CCMiscTools.h
		CCPlatform.h
		CCShareable.h
		CCToolbox.h
		CCTypes.h
		ChamferDistanceTransform.h
		CloudSamplingTools.h
		ConjugateGradient.h
		Delaunay2dMesh.h
		DgmOctree.h
		DgmOctreeReferenceCloud.h
		DistanceComputationTools.h
		ErrorFunction.h
		FastMarching.h
		FastMarchingForPropagation.h
		Garbage.h
		GenericCloud.h
		GenericDistribution.h
		GenericIndexedCloud.h
		GenericIndexedCloudPersist.h
		GenericIndexedMesh.h
		GenericMesh.h
		GenericOctree.h
		GenericProgressCallback.h
		GenericTriangle.h
		GeometricalAnalysisTools.h
		GridAndMeshIntersection.h
		Grid3D.h
		Jacobi.h
		KdTree.h
		Kriging.h
		LocalModel.h
		ManualSegmentationTools.h
		MathTools.h
		MeshSamplingTools.h
		Neighbourhood.h
		NormalDistribution.h
		ParallelSort.h
		PointCloud.h
		PointCloudTpl.h
		PointProjectionTools.h
		Polyline.h
		RayAndBox.h
		ReferenceCloud.h
		RegistrationTools.h
		SaitoSquaredDistanceTransform.h
		ScalarField.h
		ScalarFieldTools.h
		SimpleMesh.h
		SimpleTriangle.h
		SquareMatrix.h
		StatisticalTestingTools.h
		TrueKdTree.h
		WeibullDistribution.h
	DESTINATION
		include/CCCoreLib
)

target_include_directories( ${PROJECT_NAME}
	PUBLIC
		$<INSTALL_INTERFACE:include/CCCoreLib>
		$<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}>
)

