代发 wailian999

static int counter = 0;
来源：http://bqo.wangdashe.top

[S29] C：变参函数
来源：http://til.smart0.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pkv.aibaodan.cn

[S30] C：头文件保护
来源：http://ltn.yfazqb.com

#ifndef X_H
来源：http://vni.wangdashe.top

#define X_H
来源：http://grs.hysaishi.cn

#endif
来源：http://tmm.meibo888.top

[S31] C++：Hello World
来源：http://gen.zycfv.cn

#include <iostream>
来源：http://rfd.yueranfly.top

int main() { std::cout << "Hello\n"; }
来源：http://iue.pycfn.com

[S32] C++：字符串
来源：http://gec.xuetiantiany.cn

std::string s = "hi";  s += "!";
来源：http://pyh.jiagoushi.top

[S33] C++：vector 增删
来源：http://rno.cqqwz.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tax.shuidangran.top

[S34] C++：遍历 vector
来源：http://art.redwolf501.top

for (auto &x : v) { std::cout << x; }
来源：http://nbi.0kj1m.cn

[S35] C++：map
来源：http://zff.nanxuanxn.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hpx.fzhhl.top

[S36] C++：unordered_map
来源：http://xsf.epnwcf.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zhn.yuanzhike.top

[S37] C++：set
来源：http://roc.vqdsnc.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wia.52xcode.cn

[S38] C++：排序
来源：http://iya.aizwys.cn

std::sort(v.begin(), v.end());
来源：http://bwa.aibaodan.cn

[S39] C++：自定义比较器排序
来源：http://tbj.jqgfzy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uvy.xziqi.cn

[S40] C++：查找元素
来源：http://dlq.sufxvd.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zmg.ctjpmb.com

[S41] C++：类与构造函数
来源：http://qlq.pycfn.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qnq.yj20258.top

[S42] C++：继承与虚函数
来源：http://ilj.cdnleiting.top

class B : public Base { public: void f() override {} };
来源：http://hdf.hfpthk.cn

[S43] C++：智能指针
来源：http://mwn.jqgufenzy.top

auto p = std::make_unique<int>(5);
来源：http://ish.shanyushiyangtech.top

[S44] C++：引用传参
来源：http://rte.daxiang520.top

void inc(int &x) { ++x; }
来源：http://yxh.tianlin.xyz

[S45] C++：lambda
来源：http://ezt.zhengqikj.top

auto add = [](int a, int b) { return a + b; };
来源：http://eyf.yonumen.top

[S46] C++：函数模板
来源：http://uor.cashguo.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ilz.xinyue.icu

[S47] C++：结构化绑定遍历
来源：http://hjt.zhengqikj.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tmz.fehbvm.com

[S48] C++：逐行读文件
来源：http://xlr.zhixingplan.top

std::ifstream in("a.txt");  std::string line;
来源：http://bfx.vqdsnc.cn

while (std::getline(in, line)) { }
来源：http://uqm.wangshuangyany.cn

[S49] C++：写文件
来源：http://xyf.xinyue.icu

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tks.316326.xyz

[S50] C++：格式化数字
来源：http://bas.hywenlv.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://igt.fehbvm.com

[S51] C++：显式类型转换
来源：http://wwi.xingfuxueyuan.xyz

static_cast<double>(a) / b
来源：http://bdx.gaohongyu789.top

[S52] C++：const 与 noexcept
来源：http://qjl.hywenlv.cn

int size() const noexcept { return n_; }
来源：http://yui.hcnkem.com

[S53] C++：移动语义
来源：http://ewc.cqqwz.cn

std::vector<int> w = std::move(v);
来源：http://xky.tanke756.top

[S54] C++：异常处理
来源：http://ozt.dashuyun.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ybi.guannengcc.top

[S55] C++：结构化绑定
来源：http://wvr.aizwys.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://nxi.ydjk.org.cn

[S56] C++：optional
来源：http://blh.yangfankeji.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jby.zhijiandao.cn

[S57] C++：编译期常量
来源：http://tcg.fengsongda.top

constexpr int N = 10;
来源：http://jll.quarkkingdee.top

[S58] C++：命名空间
来源：http://tjj.tianlin.xyz

namespace ns { int f() { return 1; } }
来源：http://mcq.hesvh.cn

[S59] C++：静态断言
来源：http://dtg.tanke756.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rqb.redwolf501.top

[S60] C++：遍历并删除元素
来源：http://xgl.zhixingplan.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wco.jinqigufen.top

================================================================================
来源：http://ehe.havefunace.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://avv.sxryk.cn

================================================================================
来源：http://eml.yj20258888.top

[T01] Kotlin：Hello World
来源：http://yco.ivvv.top

println("Hello")
来源：http://myh.epnwcf.com

[T02] Kotlin：变量
来源：http://ebf.kuanghao11.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lgm.yonumen.top

[T03] Kotlin：字符串模板
来源：http://okf.tarul.cn

"值: $b"
来源：http://vdx.cheryme.top

[T04] Kotlin：空安全
来源：http://kbi.xziqi.cn

val n: String? = null;  n?.length
来源：http://pif.mhx1999.top

[T05] Kotlin：when 表达式
来源：http://unn.tian-w.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jrn.yuxming.cn

[T06] Kotlin：集合映射
来源：http://pdq.zhijiandao.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://zct.ctjpmb.com

[T07] Kotlin：集合过滤
来源：http://ddz.sweek.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ttz.tanke756.top

[T08] Kotlin：数据类
来源：http://jlg.fzhhl.top

data class User(val name: String, val age: Int)
来源：http://ame.xuetiantiany.cn

[T09] Kotlin：扩展函数
来源：http://yhb.fktsv.cn

fun String.exclaim() = this + "!"
来源：http://hcd.hysaishi.cn

[T10] Kotlin：默认参数
来源：http://ist.zhongyouzk.top

fun greet(name: String = "World") = "Hi $name"
来源：http://zvc.wangdashe.top

[T11] Kotlin：协程
来源：http://ncd.xylfe.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://fwc.yvedp.cn

[T12] Kotlin：解构声明
来源：http://myy.andypj.xyz

val (a, b) = Pair(1, 2)
来源：http://tgu.yj202588.top

[T13] Kotlin：只读 Map
来源：http://ked.yuanzhike.top

val m = mapOf("a" to 1)
来源：http://jrm.yvedp.cn

[T14] Kotlin：循环
来源：http://vsg.zhiwuduotai.top

for (i in 1..10) println(i)
来源：http://hwt.zdbjq.cn

[T15] Kotlin：接口
来源：http://bzh.ybcxt.top

interface Shape { fun area(): Double }
来源：http://nne.yongpay.top

[T16] Swift：Hello World
来源：http://dls.wangshuangyany.cn

print("Hello")
来源：http://wca.fengsongda.top

[T17] Swift：变量与常量
来源：http://ene.hnxiangtu.top

var a = 1;  let b = 2
来源：http://onc.cheryme.top

[T18] Swift：字符串插值
来源：http://vqa.yonumen.top

"值: \(b)"
来源：http://mxs.yvedp.cn

[T19] Swift：可选绑定
来源：http://fhm.hysaishi.cn

if let n = opt { print(n) }
来源：http://xkv.cashguo.top

[T20] Swift：数组操作
来源：http://anh.ydjk.org.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qug.yongpay.top

[T21] Swift：遍历
来源：http://zvq.shangyingyoupin.top

for x in a { print(x) }
来源：http://lul.jinyuanbaomall.cn

[T22] Swift：字典
来源：http://gll.hcnkem.com

var d = ["a": 1];  d["b"] = 2
来源：http://aya.yueranfly.top

[T23] Swift：函数
来源：http://qqw.hcnkem.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://uai.shangyingyoupin.top

[T24] Swift：闭包
来源：http://xbp.c1oappe.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://rej.zycfv.cn

[T25] Swift：结构体
来源：http://dzg.ctjpmb.com

struct P { var x: Int }
来源：http://vfr.hysaishi.cn

[T26] Swift：类与重写
来源：http://xop.yj20258888.top

class A: Base { override func f() {} }
来源：http://gqq.aizwys.cn

[T27] Swift：错误处理
来源：http://xgd.cashguo.top

do { try f() } catch { print(error) }
来源：http://rjt.yangfankeji.com

[T28] Swift：枚举
来源：http://gpc.sufxvd.cn

enum Color { case red, green }
来源：http://kww.wangdashe.top

[T29] Swift：guard 提前返回
来源：http://zsr.hnxiangtu.top

guard let x = opt else { return }
来源：http://oey.hammf.cn

[T30] Swift：协议
来源：http://zqs.shanyushiyangkeji.top

protocol Shape { func area() -> Double }
来源：http://ytv.xinyue.icu

[T31] Lua：Hello World
来源：http://wen.andypj.xyz

print("Hello")
来源：http://uyp.yfazqb.com

[T32] Lua：局部变量
来源：http://hyz.fanxiaobao.xyz

local a = 1
来源：http://szm.fktsv.cn

[T33] Lua：表（数组）
来源：http://vnl.hfpthk.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://dwg.zdbjq.cn

[T34] Lua：遍历表
来源：http://sdx.chenjidiqi.icu

for i, v in ipairs(t) do print(i, v) end
来源：http://fkf.cheryme.top

[T35] Lua：字典表
来源：http://ywn.yj20258.top

local d = { a = 1 };  d.b = 2
来源：http://mou.jyoumei.cn

[T36] Lua：函数
来源：http://ltg.fehbvm.com

function add(a, b) return a + b end
来源：http://fpl.sysykeji.top

[T37] Lua：字符串拼接
来源：http://gvc.jlsjyb.cn

"a" .. "b"
来源：http://yoj.9152youxi.cn

[T38] Lua：条件
来源：http://agp.zhiwuduotai.top

if x > 0 then print("正") end
来源：http://doy.smart0.xyz

[T39] Lua：模式匹配
来源：http://bkr.nanxuanxn.top

string.find(s, "%d+")
来源：http://jfy.zhongyouzk.top

[T40] Lua：元表
来源：http://wzw.zhoulong.xyz

setmetatable({}, { __index = base })
来源：http://ver.xylfe.cn

[T41] Perl：Hello World
来源：http://cfg.jianghu66.top

print "Hello\n";
来源：http://gkd.ybcxt.top

[T42] Perl：变量类型
来源：http://ska.yvedp.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pop.bjfxy.top

[T43] Perl：字符串插值
来源：http://qke.jyoumei.cn

"值: $a"
来源：http://jgh.sufxvd.cn

[T44] Perl：条件
来源：http://mbx.hfpthk.cn

if ($a > 0) { print "正"; }
来源：http://vfa.yangfankeji.com

[T45] Perl：数组遍历
来源：http://zwt.tian-w.cn

for my $x (@arr) { print $x; }
来源：http://dnh.zhaomingkeji.xyz

[T46] Perl：哈希操作
来源：http://rwm.yueranfly.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://klv.fengsongda.top

[T47] Perl：正则捕获
来源：http://xqu.xingfuxueyuan.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://lle.quarkkingdee.top

[T48] Perl：正则替换
来源：http://fcu.vqdsnc.cn

$s =~ s/old/new/g;
来源：http://pfi.hongshengwenyu.top

[T49] Perl：函数
来源：http://ebr.shzxlz.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xvv.ctjpmb.com

[T50] Perl：逐行读文件
来源：http://izu.zdbjq.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ymz.yuxming.cn

while (my $line = <$fh>) { print $line; }
来源：http://jcr.jqgufenzy.top

[T51] Scala：Hello World
来源：http://ghd.zhixingplan.top

println("Hello")
来源：http://qnb.jinghuilouyu.cn

[T52] Scala：变量
来源：http://mul.ybcxt.top

val a = 1;  var b = 2
来源：http://mro.yuanzhike.top

[T53] Scala：字符串插值
来源：http://fzs.sweek.top

s"值: $b"
来源：http://qlh.hammf.cn

[T54] Scala：集合映射
来源：http://gci.sxryk.cn

List(1, 2, 3).map(_ * 2)
来源：http://hpx.nwbrower.top

[T55] Scala：集合过滤
来源：http://qew.zhixingplan.top

List(1, 2, 3).filter(_ > 1)
来源：http://jgl.shuidangran.top

[T56] Scala：样例类
来源：http://ika.yanxiufei.cn

case class User(name: String, age: Int)
来源：http://yic.yueranfly.top

[T57] Scala：模式匹配
来源：http://zmm.jinqigufen.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://vno.zhengqikj.top

[T58] Scala：函数定义
来源：http://nns.shzxlz.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ypc.sweek.top

[T59] Scala：循环
来源：http://ydo.fehbvm.com

for (i <- 1 to 10) println(i)
来源：http://iqm.birdmap.top

[T60] Scala：折叠
来源：http://vji.ydjk.org.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xzk.sweek.top

================================================================================
来源：http://yfk.haohaochexian.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xqi.yj202588.top

================================================================================
来源：http://qed.zhoulong.xyz

[U01] Py：创建虚拟环境
来源：http://bws.yongpay.top

python -m venv .venv && source .venv/bin/activate
来源：http://xjy.ydzc1.top

[U02] Py：导出 / 安装依赖
来源：http://lpu.yfazqb.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zqo.fzhhl.top

[U03] Py：加载 .env 配置
来源：http://okg.guowangkeji.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ofb.kuanghao11.cn

[U04] Py：变量调试打印
来源：http://phv.ctjpmb.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nde.jianghu66.top

[U05] Py：列表去重且保序
来源：http://rbq.feifeiyinyue.top

list(dict.fromkeys(arr))
来源：http://uue.9152youxi.cn

[U06] Py：合并两个字典
来源：http://ltl.redwolf501.top

{**a, **b}
来源：http://dvi.zhixingplan.top

[U07] Py：反转字典键值
来源：http://ily.tian-w.cn

{v: k for k, v in d.items()}
来源：http://sry.jinqigfzy.top

[U08] Py：展平二维列表
来源：http://xak.yfazqb.com

[y for x in nested for y in x]
来源：http://aoe.316326.xyz

[U09] Py：字典取最大值的键
来源：http://gyh.sysykeji.top

max(d, key=d.get)
来源：http://ukp.quarkkingdee.top

[U10] Py：按值排序字典
来源：http://png.fktsv.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uau.sysykeji.top

[U11] Py：生成器表达式
来源：http://jgq.hywenlv.cn

(x * 2 for x in arr)
来源：http://fib.ctjpmb.com

[U12] Py：取出现最多的 3 个元素
来源：http://yiv.hfpthk.cn

Counter(arr).most_common(3)
来源：http://gna.guannengcc.top

[U13] Py：固定长度队列
来源：http://wtt.zhixingplan.top

deque(maxlen=10)
来源：http://xpn.yj20258.top

[U14] Py：分组收集到列表
来源：http://chn.c1oappe.top

defaultdict(list)
来源：http://aci.0kj1m.cn

[U15] Py：高精度计时
来源：http://trx.sjlbkw.cn

t = time.perf_counter()
来源：http://mig.fanxiaobao.xyz

[U16] Py：命令行参数解析
来源：http://pim.fktsv.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ibu.ybcxt.top

[U17] Py：初始化日志
来源：http://ydt.fehbvm.com

logging.basicConfig(level=logging.INFO)
来源：http://fzi.iojbl.cn

[U18] Py：预编译正则
来源：http://uzc.yj202588.top

pat = re.compile(r"\d+")
来源：http://heh.feifeiyinyue.top

[U19] Py：正则替换带回调
来源：http://jtj.jinghuilouyu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ysk.hongshengwenyu.top

[U20] Py：缓存函数结果
来源：http://xld.zhijiandao.cn

@functools.lru_cache(maxsize=None)
来源：http://xus.jinqigfzy.top

[U21] Py：自定义上下文管理器
来源：http://ngv.chenlongwang.top

@contextlib.contextmanager
来源：http://ogd.52xcode.cn

[U22] Py：矩阵转置
来源：http://xag.gzhubu.top

list(zip(*m))
来源：http://mph.hysaishi.cn

[U23] Py：分块读取大文件
来源：http://fzz.ybcxt.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jxr.smart0.xyz

[U24] Py：路径操作
来源：http://bkc.quarkkingdee.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://oyw.sjlbkw.cn

[U25] Py：CSV 按字典读
来源：http://axn.nanxinkj.top

csv.DictReader(f)
来源：http://hrh.chenlongwang.top

[U26] Py：并发下载
来源：http://ceq.iojbl.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mmq.bjfxy.top

[U27] Py：异步 HTTP
来源：http://mfi.gotoacloud.top

aiohttp.ClientSession() 配合 async with
来源：http://sju.zycfv.cn

[U28] Py：类型别名
来源：http://jml.dashuyun.cn

UserId = int
来源：http://nfo.jlsjyb.cn

[U29] Py：属性校验
来源：http://rnj.hnxiangtu.top

@property 与 @x.setter 配合
来源：http://rzy.yuxming.cn

[U30] Py：数据类
来源：http://hcq.zhengqikj.top

@dataclass(slots=True)
来源：http://vjy.xinyue.icu

[U31] Py：单测
来源：http://lsk.zhixingplan.top

python -m pytest -q
来源：http://fks.kuanghao11.cn

[U32] Py：代码格式化
来源：http://yjg.zhaomingkeji.xyz

ruff format . && ruff check --fix .
来源：http://ctx.xingfuxueyuan.xyz

[U33] Py：打包发布
来源：http://lju.jqgufenzy.top

python -m build  （依赖 pyproject.toml）
来源：http://icc.bbcook.cn

[U34] Py：判断编码
来源：http://ods.yongpay.top

chardet.detect(raw)
来源：http://vpc.hesvh.cn

[U35] Py：发送邮件
来源：http://nvw.zycfv.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dcf.fanxiaobao.xyz

[U36] Py：定时任务
来源：http://sju.kuanghao11.cn

schedule.every(10).minutes.do(job)
来源：http://gwn.ppjwa.cn

[U37] Py：读写 Excel
来源：http://cmi.zycfv.cn

pandas.read_excel / DataFrame.to_excel
来源：http://sdc.zhoulong.xyz

[U38] Py：获取脚本所在目录
来源：http://pxp.svipenyu.cn

Path(__file__).resolve().parent
来源：http://prp.cheryme.top

[U39] Py：判断是否在交互环境
来源：http://dwp.yj202588.top

sys.stdout.isatty()
来源：http://bwb.yanxiufei.cn

[U40] Py：打印到标准错误
来源：http://vaw.zhoulong.xyz

print("err", file=sys.stderr)
来源：http://eux.fzhhl.top

[U41] PHP：初始化 Composer 项目
来源：http://qpi.zdqjudy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://rjz.ppjwa.cn

[U42] PHP：PSR-4 自动加载
来源：http://gxz.yvedp.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wlm.smart0.xyz

[U43] PHP：声明命名空间
来源：http://acf.c1oappe.top

namespace App\Http;
来源：http://uxc.yongpay.top

[U44] PHP：开启严格类型
来源：http://ivg.jinqigfzy.top

declare(strict_types=1);
来源：http://lux.fehbvm.com

[U45] PHP：类型声明与返回类型
来源：http://hua.nanxuanxn.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://nzo.uphjek.com

[U46] PHP：可空类型
来源：http://txb.pengpengdd.cyou

?string $name = null
来源：http://ana.yj202588.top

[U47] PHP：联合类型
来源：http://bij.bbcook.cn

int|string $id
来源：http://axf.daxiang520.top

[U48] PHP：纯枚举
来源：http://fga.fengsongda.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xra.chenjidiqi.icu

[U49] PHP：只读属性
来源：http://xwo.ybcxt.top

public readonly string $name
来源：http://fxb.yongpay.top

[U50] PHP：构造器属性提升
来源：http://hau.daria6918.cn

public function __construct(private int $id) {}
来源：http://glf.bbcook.cn

[U51] PHP：数组解构
来源：http://bxz.shanyushiyangkeji.top

[$a, $b] = $arr;
来源：http://sth.dashuyun.cn

[U52] PHP：箭头函数
来源：http://ycs.yuxming.cn

$double = fn($x) => $x * 2;
来源：http://bjq.daria6918.cn


<!-- 参考信息 -->