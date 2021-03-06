set(APP_NAME testcpp)

set(SAMPLE_SRC
  Classes/AccelerometerTest/AccelerometerTest.cpp
  Classes/ActionManagerTest/ActionManagerTest.cpp
  Classes/ActionsEaseTest/ActionsEaseTest.cpp
  Classes/ActionsProgressTest/ActionsProgressTest.cpp
  Classes/ActionsTest/ActionsTest.cpp
  Classes/Box2DTest/Box2dTest.cpp
  Classes/Box2DTestBed/Box2dView.cpp
  Classes/Box2DTestBed/GLES-Render.cpp
  Classes/Box2DTestBed/Test.cpp
  Classes/Box2DTestBed/TestEntries.cpp
  Classes/BugsTest/Bug-1159.cpp
  Classes/BugsTest/Bug-1174.cpp
  Classes/BugsTest/Bug-350.cpp
  Classes/BugsTest/Bug-422.cpp
  Classes/BugsTest/Bug-458/Bug-458.cpp
  Classes/BugsTest/Bug-458/QuestionContainerSprite.cpp
  Classes/BugsTest/Bug-624.cpp
  Classes/BugsTest/Bug-886.cpp
  Classes/BugsTest/Bug-899.cpp
  Classes/BugsTest/Bug-914.cpp
  Classes/BugsTest/BugsTest.cpp
  Classes/ChipmunkTest/ChipmunkTest.cpp
  Classes/ClickAndMoveTest/ClickAndMoveTest.cpp
  Classes/ClippingNodeTest/ClippingNodeTest.cpp
  Classes/CocosDenshionTest/CocosDenshionTest.cpp
  Classes/CurlTest/CurlTest.cpp
  Classes/CurrentLanguageTest/CurrentLanguageTest.cpp
  Classes/DrawPrimitivesTest/DrawPrimitivesTest.cpp
  Classes/EffectsAdvancedTest/EffectsAdvancedTest.cpp
  Classes/EffectsTest/EffectsTest.cpp
  Classes/ExtensionsTest/CocosBuilderTest/ButtonTest/ButtonTestLayer.cpp
  Classes/ExtensionsTest/CocosBuilderTest/CocosBuilderTest.cpp
  Classes/ExtensionsTest/CocosBuilderTest/HelloCocosBuilder/HelloCocosBuilderLayer.cpp
  Classes/ExtensionsTest/CocosBuilderTest/AnimationsTest/AnimationsTestLayer.cpp
  Classes/ExtensionsTest/CocosBuilderTest/MenuTest/MenuTestLayer.cpp
  Classes/ExtensionsTest/CocosBuilderTest/TestHeader/TestHeaderLayer.cpp
  Classes/ExtensionsTest/CocosBuilderTest/TimelineCallbackTest/TimelineCallbackTestLayer.cpp
  Classes/ExtensionsTest/ControlExtensionTest/CCControlButtonTest/CCControlButtonTest.cpp
  Classes/ExtensionsTest/ControlExtensionTest/CCControlColourPicker/CCControlColourPickerTest.cpp
  Classes/ExtensionsTest/ControlExtensionTest/CCControlScene.cpp
  Classes/ExtensionsTest/ControlExtensionTest/CCControlSceneManager.cpp
  Classes/ExtensionsTest/ControlExtensionTest/CCControlSliderTest/CCControlSliderTest.cpp
  Classes/ExtensionsTest/ControlExtensionTest/CCControlSwitchTest/CCControlSwitchTest.cpp
  Classes/ExtensionsTest/ControlExtensionTest/CCControlPotentiometerTest/CCControlPotentiometerTest.cpp
  Classes/ExtensionsTest/ControlExtensionTest/CCControlStepperTest/CCControlStepperTest.cpp
  Classes/ExtensionsTest/TableViewTest/TableViewTestScene.cpp
  Classes/ExtensionsTest/TableViewTest/CustomTableViewCell.cpp
  Classes/ExtensionsTest/ExtensionsTest.cpp
  Classes/ExtensionsTest/NotificationCenterTest/NotificationCenterTest.cpp
  Classes/ExtensionsTest/NetworkTest/HttpClientTest.cpp
  Classes/ExtensionsTest/CocoStudioArmatureTest/ArmatureScene.cpp
  Classes/ExtensionsTest/CocoStudioComponentsTest/ComponentsTestScene.cpp
  Classes/ExtensionsTest/CocoStudioComponentsTest/EnemyController.cpp
  Classes/ExtensionsTest/CocoStudioComponentsTest/GameOverScene.cpp
  Classes/ExtensionsTest/CocoStudioComponentsTest/PlayerController.cpp
  Classes/ExtensionsTest/CocoStudioComponentsTest/ProjectileController.cpp
  Classes/ExtensionsTest/CocoStudioComponentsTest/SceneController.cpp
  Classes/ExtensionsTest/CocoStudioSceneTest/SceneEditorTest.cpp
  Classes/ExtensionsTest/CocoStudioSceneTest/TriggerCode/acts.cpp
  Classes/ExtensionsTest/CocoStudioSceneTest/TriggerCode/cons.cpp
  Classes/ExtensionsTest/CocoStudioGUITest/UIScene.cpp
  Classes/ExtensionsTest/CocoStudioGUITest/UISceneManager.cpp
  Classes/ExtensionsTest/CocoStudioGUITest/UIButtonTest/UIButtonTest.cpp
  Classes/ExtensionsTest/CocoStudioGUITest/UICheckBoxTest/UICheckBoxTest.cpp
  Classes/ExtensionsTest/CocoStudioGUITest/UIImageViewTest/UIImageViewTest.cpp
  Classes/ExtensionsTest/CocoStudioGUITest/UILabelAtlasTest/UILabelAtlasTest.cpp
  Classes/ExtensionsTest/CocoStudioGUITest/UILabelBMFontTest/UILabelBMFontTest.cpp
  Classes/ExtensionsTest/CocoStudioGUITest/UILabelTest/UILabelTest.cpp
  Classes/ExtensionsTest/CocoStudioGUITest/UIListViewTest/UIListViewTest.cpp
  Classes/ExtensionsTest/CocoStudioGUITest/UILoadingBarTest/UILoadingBarTest.cpp
  Classes/ExtensionsTest/CocoStudioGUITest/UIPageViewTest/UIPageViewTest.cpp
  Classes/ExtensionsTest/CocoStudioGUITest/UILayoutTest/UILayoutTest.cpp
  Classes/ExtensionsTest/CocoStudioGUITest/UIScrollViewTest/UIScrollViewTest.cpp
  Classes/ExtensionsTest/CocoStudioGUITest/UISliderTest/UISliderTest.cpp
  Classes/ExtensionsTest/CocoStudioGUITest/UITextFieldTest/UITextFieldTest.cpp
  Classes/ExtensionsTest/CocoStudioGUITest/UIWidgetAddNodeTest/UIWidgetAddNodeTest.cpp
  Classes/ExtensionsTest/CocoStudioGUITest/CocosGUIScene.cpp
  Classes/ExtensionsTest/Scale9SpriteTest/Scale9SpriteTest.cpp
  Classes/NewRendererTest/NewRendererTest.cpp
  Classes/NewEventDispatcherTest/NewEventDispatcherTest.cpp
  Classes/FontTest/FontTest.cpp
  Classes/IntervalTest/IntervalTest.cpp
  Classes/KeyboardTest/KeyboardTest.cpp
  Classes/InputTest/MouseTest.cpp
  Classes/KeypadTest/KeypadTest.cpp
  Classes/LabelTest/LabelTest.cpp
  Classes/LabelTest/LabelTestNew.cpp
  Classes/LayerTest/LayerTest.cpp
  Classes/MenuTest/MenuTest.cpp
  Classes/MotionStreakTest/MotionStreakTest.cpp
  Classes/MutiTouchTest/MutiTouchTest.cpp
  Classes/NodeTest/NodeTest.cpp
  Classes/ParallaxTest/ParallaxTest.cpp
  Classes/ParticleTest/ParticleTest.cpp
  Classes/PerformanceTest/PerformanceAllocTest.cpp
  Classes/PerformanceTest/PerformanceNodeChildrenTest.cpp
  Classes/PerformanceTest/PerformanceParticleTest.cpp
  Classes/PerformanceTest/PerformanceSpriteTest.cpp
  Classes/PerformanceTest/PerformanceTest.cpp
  Classes/PerformanceTest/PerformanceTextureTest.cpp
  Classes/PerformanceTest/PerformanceTouchesTest.cpp
  Classes/PerformanceTest/PerformanceLabelTest.cpp
  Classes/PhysicsTest/PhysicsTest.cpp
  Classes/RenderTextureTest/RenderTextureTest.cpp
  Classes/RotateWorldTest/RotateWorldTest.cpp
  Classes/SceneTest/SceneTest.cpp
  Classes/SchedulerTest/SchedulerTest.cpp
  Classes/ShaderTest/ShaderTest.cpp
  Classes/ShaderTest/ShaderTest2.cpp
  Classes/SpriteTest/SpriteTest.cpp
  Classes/TextInputTest/TextInputTest.cpp
  Classes/Texture2dTest/Texture2dTest.cpp
  Classes/TexturePackerEncryptionTest/TextureAtlasEncryptionTest.cpp
  Classes/TextureCacheTest/TextureCacheTest.cpp
  Classes/TileMapTest/TileMapTest.cpp
  Classes/TouchesTest/Ball.cpp
  Classes/TouchesTest/Paddle.cpp
  Classes/TouchesTest/TouchesTest.cpp
  Classes/TransitionsTest/TransitionsTest.cpp
  Classes/UserDefaultTest/UserDefaultTest.cpp
  Classes/ZwoptexTest/ZwoptexTest.cpp
  Classes/FileUtilsTest/FileUtilsTest.cpp
  Classes/SpineTest/SpineTest.cpp
  Classes/DataVisitorTest/DataVisitorTest.cpp
  Classes/ConfigurationTest/ConfigurationTest.cpp
  Classes/ConsoleTest/ConsoleTest.cpp
  Classes/UnitTest/UnitTest.cpp
  Classes/controller.cpp
  Classes/testBasic.cpp
  Classes/AppDelegate.cpp
  Classes/BaseTest.cpp
  Classes/VisibleRect.cpp
  proj.linux/main.cpp
)

include_directories(
  Classes
)

# add the executable
add_executable(${APP_NAME}
  ${SAMPLE_SRC}
)

target_link_libraries(${APP_NAME}
  gui
  network
  spine
  cocostudio
  cocosbuilder
  extensions
  audio
  cocos2d
  box2d
)

set(APP_BIN_DIR "${CMAKE_BINARY_DIR}/bin/${APP_NAME}")

set_target_properties(${APP_NAME} PROPERTIES
     RUNTIME_OUTPUT_DIRECTORY  "${APP_BIN_DIR}")

pre_build(${APP_NAME}
  COMMAND ${CMAKE_COMMAND} -E remove_directory ${APP_BIN_DIR}/Resources
  COMMAND ${CMAKE_COMMAND} -E copy_directory ${CMAKE_CURRENT_SOURCE_DIR}/Resources ${APP_BIN_DIR}/Resources
  )
