### Torchcfm

## Location


# SF2M模型
   runner/src/models/cfm_module.py        30      class CFMLitModule(LightningModule)             SF2M的父类
                                          717     class SBCFMLitModule(CFMLitModule)
                                          738     class SF2MLitModule(CFMLitModule)               SB+FM文章的模型SF2M
                                    <!-- 1088    class OneWaySF2MLitModule(SF2MLitModule)   SF2M其余演化版本-->
                                    <!-- 1183    class DSBMLitModule(SF2MLitModule)         SF2M其余演化版本-->
                                    <!-- 1295    class DSBMSharedLitModule(SF2MLitModule)   SF2M其余演化版本-->
# 数据要求
    torchcfm/conditional_flow_matching.py    397     class SchrodingerBridgeConditionalFlowMatcher(ConditionalFlowMatcher)  说明其与cfm要求一致
                                             41      class CFMLitModule(LightningModule)  说明其对*dim大小没有要求
--------------------------------------------------------------------------------------------------------------------------------------
    runner/src/datamodules/distribution_datamodule.py      284     class DiffusionSchrodingerBridgeGaussians(LightningDataModule) init部分有例子
--------------------------------------------------------------------------------------------------------------------------------------
    tests/test_time_t.py                                    30      def test_guided_random_Tensor_t(FM, return_noise)  测试时的例子
