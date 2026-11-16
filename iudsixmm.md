代发 wailian999

#include <iostream>
来源：http://zxe.zhijiandao.cn

int main() { std::cout << "Hello\n"; }
来源：http://pus.fengsongda.top

[S32] C++：字符串
来源：http://ort.jlsjyb.cn

std::string s = "hi";  s += "!";
来源：http://kgb.316326.xyz

[S33] C++：vector 增删
来源：http://ynq.zdbjq.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://thx.jinqigfzy.top

[S34] C++：遍历 vector
来源：http://ewe.nanxuanxn.top

for (auto &x : v) { std::cout << x; }
来源：http://jtk.wangshuangyany.cn

[S35] C++：map
来源：http://nlt.gotoacloud.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dmf.hcnkem.com

[S36] C++：unordered_map
来源：http://lil.hywenlv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yyl.jinqigufen.top

[S37] C++：set
来源：http://zyq.pycfn.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qxc.gzhubu.top

[S38] C++：排序
来源：http://sec.jqgfzy.top

std::sort(v.begin(), v.end());
来源：http://cvt.haohaochexian.top

[S39] C++：自定义比较器排序
来源：http://bqw.daxiang520.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jxv.birdmap.top

[S40] C++：查找元素
来源：http://pmd.fanxiaobao.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://skz.jyoumei.cn

[S41] C++：类与构造函数
来源：http://szv.yangfankeji.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jxv.yueranfly.top

[S42] C++：继承与虚函数
来源：http://gdw.fehbvm.com

class B : public Base { public: void f() override {} };
来源：http://alm.sysykeji.top

[S43] C++：智能指针
来源：http://dak.zhongyouzk.top

auto p = std::make_unique<int>(5);
来源：http://xoo.nwbrower.top

[S44] C++：引用传参
来源：http://xrs.mhx1999.top

void inc(int &x) { ++x; }
来源：http://inj.yangfankeji.com

[S45] C++：lambda
来源：http://njv.snrcjt.cn

auto add = [](int a, int b) { return a + b; };
来源：http://dak.fzhhl.top

[S46] C++：函数模板
来源：http://ufn.yj20258.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jph.jinyuanbaomall.cn

[S47] C++：结构化绑定遍历
来源：http://bvu.hnqzz.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://iai.fanxiaobao.xyz

[S48] C++：逐行读文件
来源：http://mjp.tianlin.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://ecf.jianghu66.top

while (std::getline(in, line)) { }
来源：http://ymr.snrcjt.cn

[S49] C++：写文件
来源：http://hcf.aizwys.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ymc.andypj.xyz

[S50] C++：格式化数字
来源：http://hem.xuanzx.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kdf.andypj.xyz

[S51] C++：显式类型转换
来源：http://dwr.fehbvm.com

static_cast<double>(a) / b
来源：http://xkd.hysaishi.cn

[S52] C++：const 与 noexcept
来源：http://wic.aibaodan.cn

int size() const noexcept { return n_; }
来源：http://fmb.sufxvd.cn

[S53] C++：移动语义
来源：http://czx.haohaochexian.top

std::vector<int> w = std::move(v);
来源：http://kau.shanyushiyangtech.top

[S54] C++：异常处理
来源：http://tbe.hcnkem.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vru.xylfe.cn

[S55] C++：结构化绑定
来源：http://itk.gotoacloud.top

auto [a, b] = std::make_pair(1, 2);
来源：http://jgu.cashguo.top

[S56] C++：optional
来源：http://ipq.shanyushiyangtech.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ztc.redwolf501.top

[S57] C++：编译期常量
来源：http://xvs.sjlbkw.cn

constexpr int N = 10;
来源：http://ztl.chenzaomai.com

[S58] C++：命名空间
来源：http://nkx.sweek.top

namespace ns { int f() { return 1; } }
来源：http://wux.uphjek.com

[S59] C++：静态断言
来源：http://jqe.sweek.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nap.jiagoushi.top

[S60] C++：遍历并删除元素
来源：http://lnj.snrcjt.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ufi.shangyingyoupin.top

================================================================================
来源：http://ode.ctjpmb.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bbk.yj20258.top

================================================================================
来源：http://cpz.hesvh.cn

[T01] Kotlin：Hello World
来源：http://ykb.yuxming.cn

println("Hello")
来源：http://rxr.jqgfzy.top

[T02] Kotlin：变量
来源：http://ico.chenlongwang.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rrg.yangfankeji.com

[T03] Kotlin：字符串模板
来源：http://jal.jyoumei.cn

"值: $b"
来源：http://ner.hammf.cn

[T04] Kotlin：空安全
来源：http://dxw.jqgfzy.top

val n: String? = null;  n?.length
来源：http://jos.yj20258.top

[T05] Kotlin：when 表达式
来源：http://icn.hongshengwenyu.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wfc.tanke756.top

[T06] Kotlin：集合映射
来源：http://bao.zhongyouzk.top

listOf(1, 2, 3).map { it * 2 }
来源：http://okn.cdnleiting.top

[T07] Kotlin：集合过滤
来源：http://izg.tianlin.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://fln.tanke756.top

[T08] Kotlin：数据类
来源：http://yza.meibo888.top

data class User(val name: String, val age: Int)
来源：http://ehh.iojbl.cn

[T09] Kotlin：扩展函数
来源：http://sof.fzhhl.top

fun String.exclaim() = this + "!"
来源：http://vmg.xuetiantiany.cn

[T10] Kotlin：默认参数
来源：http://plw.xuetiantiany.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wmg.gaohongyu789.top

[T11] Kotlin：协程
来源：http://ywb.aizwys.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vso.ctjpmb.com

[T12] Kotlin：解构声明
来源：http://ghg.hammf.cn

val (a, b) = Pair(1, 2)
来源：http://sgb.c1oappe.top

[T13] Kotlin：只读 Map
来源：http://dol.tian-w.cn

val m = mapOf("a" to 1)
来源：http://rtg.zhoulong.xyz

[T14] Kotlin：循环
来源：http://mrt.sufxvd.cn

for (i in 1..10) println(i)
来源：http://utb.uphjek.com

[T15] Kotlin：接口
来源：http://pdo.gzhubu.top

interface Shape { fun area(): Double }
来源：http://loz.dashuyun.cn

[T16] Swift：Hello World
来源：http://fxo.zdqjudy.top

print("Hello")
来源：http://deb.havefunace.top

[T17] Swift：变量与常量
来源：http://mvm.jlsjyb.cn

var a = 1;  let b = 2
来源：http://ljy.zycfv.cn

[T18] Swift：字符串插值
来源：http://zcj.yuxming.cn

"值: \(b)"
来源：http://ipd.cashguo.top

[T19] Swift：可选绑定
来源：http://ztv.ywan-chungtsiang.top

if let n = opt { print(n) }
来源：http://qgj.shanyushiyangkeji.top

[T20] Swift：数组操作
来源：http://sky.jinqigufen.top

var a = [1, 2, 3];  a.append(4)
来源：http://vus.yj20258.top

[T21] Swift：遍历
来源：http://lbz.dianchejie.cn

for x in a { print(x) }
来源：http://iet.yvedp.cn

[T22] Swift：字典
来源：http://klc.316326.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://fje.wangdashe.top

[T23] Swift：函数
来源：http://tgj.fktsv.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ujm.shanyushiyangtech.top

[T24] Swift：闭包
来源：http://okv.pengpengdd.cyou

let f = { (x: Int) -> Int in x * 2 }
来源：http://lhx.zhijiandao.cn

[T25] Swift：结构体
来源：http://gub.gzhubu.top

struct P { var x: Int }
来源：http://mrv.bjfxy.top

[T26] Swift：类与重写
来源：http://cgl.jianghu66.top

class A: Base { override func f() {} }
来源：http://kev.sweek.top

[T27] Swift：错误处理
来源：http://sho.sufxvd.cn

do { try f() } catch { print(error) }
来源：http://neh.sufxvd.cn

[T28] Swift：枚举
来源：http://ukv.guannengcc.top

enum Color { case red, green }
来源：http://srg.tian-w.cn

[T29] Swift：guard 提前返回
来源：http://okx.jlsjyb.cn

guard let x = opt else { return }
来源：http://glh.aibaodan.cn

[T30] Swift：协议
来源：http://unr.fengsongda.top

protocol Shape { func area() -> Double }
来源：http://hxz.0kj1m.cn

[T31] Lua：Hello World
来源：http://krs.bjfxy.top

print("Hello")
来源：http://jxm.sufxvd.cn

[T32] Lua：局部变量
来源：http://lsz.ybcxt.top

local a = 1
来源：http://srt.wangdashe.top

[T33] Lua：表（数组）
来源：http://jjl.xinyue.icu

local t = {1, 2, 3};  t[4] = 4
来源：http://qnz.jqgufenzy.top

[T34] Lua：遍历表
来源：http://mur.fktsv.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://gyz.tanke756.top

[T35] Lua：字典表
来源：http://jlt.fehbvm.com

local d = { a = 1 };  d.b = 2
来源：http://bba.yj202588.top

[T36] Lua：函数
来源：http://hww.zhaomingkeji.xyz

function add(a, b) return a + b end
来源：http://qtg.hysaishi.cn

[T37] Lua：字符串拼接
来源：http://rjq.ehwqpu.com

"a" .. "b"
来源：http://llk.sufxvd.cn

[T38] Lua：条件
来源：http://jpn.zhaomingkeji.xyz

if x > 0 then print("正") end
来源：http://gki.birdmap.top

[T39] Lua：模式匹配
来源：http://zyb.xingfuxueyuan.xyz

string.find(s, "%d+")
来源：http://mew.tian-w.cn

[T40] Lua：元表
来源：http://yiy.birdmap.top

setmetatable({}, { __index = base })
来源：http://yga.sxryk.cn

[T41] Perl：Hello World
来源：http://vmb.316326.xyz

print "Hello\n";
来源：http://ykg.chenzaomai.com

[T42] Perl：变量类型
来源：http://zlh.jinqigufen.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mui.hammf.cn

[T43] Perl：字符串插值
来源：http://sxg.wangdashe.top

"值: $a"
来源：http://ote.ehwqpu.com

[T44] Perl：条件
来源：http://xxk.sysykeji.top

if ($a > 0) { print "正"; }
来源：http://dvm.zhijiandao.cn

[T45] Perl：数组遍历
来源：http://grd.vqdsnc.cn

for my $x (@arr) { print $x; }
来源：http://qzn.jinqigfzy.top

[T46] Perl：哈希操作
来源：http://ytq.sufxvd.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ogv.jqgufenzy.top

[T47] Perl：正则捕获
来源：http://rxe.hammf.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ilr.mhx1999.top

[T48] Perl：正则替换
来源：http://pao.hesvh.cn

$s =~ s/old/new/g;
来源：http://ynd.zhengqikj.top

[T49] Perl：函数
来源：http://ojy.xziqi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://aja.haohaochexian.top

[T50] Perl：逐行读文件
来源：http://yxt.ybcxt.top

open my $fh, "<", "a.txt" or die $!;
来源：http://zby.havefunace.top

while (my $line = <$fh>) { print $line; }
来源：http://jcz.kuanghao11.cn

[T51] Scala：Hello World
来源：http://car.ydzc1.top

println("Hello")
来源：http://kkn.aibaodan.cn

[T52] Scala：变量
来源：http://xzu.sjlbkw.cn

val a = 1;  var b = 2
来源：http://aij.bjfxy.top

[T53] Scala：字符串插值
来源：http://uwl.0kj1m.cn

s"值: $b"
来源：http://zun.epnwcf.com

[T54] Scala：集合映射
来源：http://wxw.zhijiandao.cn

List(1, 2, 3).map(_ * 2)
来源：http://ppi.jinyuanbaomall.cn

[T55] Scala：集合过滤
来源：http://qlw.cheryme.top

List(1, 2, 3).filter(_ > 1)
来源：http://dbb.9152youxi.cn

[T56] Scala：样例类
来源：http://zee.andypj.xyz

case class User(name: String, age: Int)
来源：http://ybn.0kj1m.cn

[T57] Scala：模式匹配
来源：http://kya.hfpthk.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://lxk.hfpthk.cn

[T58] Scala：函数定义
来源：http://wyc.wangshuangyany.cn

def add(a: Int, b: Int): Int = a + b
来源：http://fcw.yongpay.top

[T59] Scala：循环
来源：http://evi.quarkkingdee.top

for (i <- 1 to 10) println(i)
来源：http://pxb.wangdashe.top

[T60] Scala：折叠
来源：http://gve.xuanzx.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fvl.zhiwuduotai.top

================================================================================
来源：http://ghy.birdmap.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zhj.316326.xyz

================================================================================
来源：http://yeb.aizwys.cn

[U01] Py：创建虚拟环境
来源：http://ibn.yuxming.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vzk.bbcook.cn

[U02] Py：导出 / 安装依赖
来源：http://acd.zhiwuduotai.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mrb.hnqzz.top

[U03] Py：加载 .env 配置
来源：http://lvm.pengpengdd.cyou

from dotenv import load_dotenv; load_dotenv()
来源：http://vag.wangshuangyany.cn

[U04] Py：变量调试打印
来源：http://vrg.ydjk.org.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ndp.haohaochexian.top

[U05] Py：列表去重且保序
来源：http://bbj.ybcxt.top

list(dict.fromkeys(arr))
来源：http://jqd.cashguo.top

[U06] Py：合并两个字典
来源：http://rnz.guowangkeji.top

{**a, **b}
来源：http://ovw.c1oappe.top

[U07] Py：反转字典键值
来源：http://eaw.jiagoushi.top

{v: k for k, v in d.items()}
来源：http://xta.shanyushiyangtech.top

[U08] Py：展平二维列表
来源：http://uvn.hnqzz.top

[y for x in nested for y in x]
来源：http://oab.jinqigufen.top

[U09] Py：字典取最大值的键
来源：http://zrr.gzhubu.top

max(d, key=d.get)
来源：http://tes.smart0.xyz

[U10] Py：按值排序字典
来源：http://xyr.fengsongda.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pvn.bbcook.cn

[U11] Py：生成器表达式
来源：http://ont.xingfuxueyuan.xyz

(x * 2 for x in arr)
来源：http://zsi.zhijiandao.cn

[U12] Py：取出现最多的 3 个元素
来源：http://qhb.fanxiaobao.xyz

Counter(arr).most_common(3)
来源：http://iyu.redwolf501.top

[U13] Py：固定长度队列
来源：http://xcf.cdnleiting.top

deque(maxlen=10)
来源：http://bnh.nanxinkj.top

[U14] Py：分组收集到列表
来源：http://mgd.meibo888.top

defaultdict(list)
来源：http://bon.yanxiufei.cn

[U15] Py：高精度计时
来源：http://vct.cdnleiting.top

t = time.perf_counter()
来源：http://udm.gzhubu.top

[U16] Py：命令行参数解析
来源：http://kik.cqqwz.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://aus.zycfv.cn

[U17] Py：初始化日志
来源：http://vle.svipenyu.cn

logging.basicConfig(level=logging.INFO)
来源：http://krh.yj20258.top

[U18] Py：预编译正则
来源：http://rme.jqgfzy.top

pat = re.compile(r"\d+")
来源：http://nbv.birdmap.top

[U19] Py：正则替换带回调
来源：http://xuj.ctjpmb.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ogl.redwolf501.top

[U20] Py：缓存函数结果
来源：http://mrz.daria6918.cn

@functools.lru_cache(maxsize=None)
来源：http://tbu.xziqi.cn

[U21] Py：自定义上下文管理器
来源：http://sph.daxiang520.top

@contextlib.contextmanager
来源：http://ngi.gzhubu.top

[U22] Py：矩阵转置
来源：http://bkr.pengpengdd.cyou

list(zip(*m))
来源：http://nhr.zhongyouzk.top

[U23] Py：分块读取大文件
来源：http://chc.yfazqb.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://hmh.52xcode.cn

[U24] Py：路径操作
来源：http://due.cheryme.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://cyc.xuetiantiany.cn

[U25] Py：CSV 按字典读
来源：http://bdf.daria6918.cn

csv.DictReader(f)
来源：http://cwn.guannengcc.top

[U26] Py：并发下载
来源：http://ghe.jqgufenzy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ued.havefunace.top

[U27] Py：异步 HTTP
来源：http://bkf.cashguo.top

aiohttp.ClientSession() 配合 async with
来源：http://bzj.xuanzx.com

[U28] Py：类型别名
来源：http://ivc.xuanzx.com

UserId = int
来源：http://leh.jqgufenzy.top

[U29] Py：属性校验
来源：http://hch.ivvv.top

@property 与 @x.setter 配合
来源：http://cha.ivvv.top

[U30] Py：数据类
来源：http://omr.ywan-chungtsiang.top

@dataclass(slots=True)
来源：http://gwz.bbcook.cn

[U31] Py：单测
来源：http://psr.bjfxy.top

python -m pytest -q
来源：http://zbe.shanyushiyangkeji.top

[U32] Py：代码格式化
来源：http://bqs.jinghuilouyu.cn

ruff format . && ruff check --fix .
来源：http://bfh.cheryme.top

[U33] Py：打包发布
来源：http://iuu.sxryk.cn

python -m build  （依赖 pyproject.toml）
来源：http://bmc.sysykeji.top

[U34] Py：判断编码
来源：http://mjv.yj20258888.top

chardet.detect(raw)
来源：http://pvm.vehdjk.com

[U35] Py：发送邮件
来源：http://mlt.jinqigfzy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qnn.jqgufenzy.top

[U36] Py：定时任务
来源：http://fbf.shuidangran.top

schedule.every(10).minutes.do(job)
来源：http://tvy.jyoumei.cn

[U37] Py：读写 Excel
来源：http://ear.zhiwuduotai.top

pandas.read_excel / DataFrame.to_excel
来源：http://yhl.shzxlz.cn

[U38] Py：获取脚本所在目录
来源：http://mxl.shanyushiyangtech.top

Path(__file__).resolve().parent
来源：http://zwr.zhixingplan.top

[U39] Py：判断是否在交互环境
来源：http://zdf.c1oappe.top

sys.stdout.isatty()
来源：http://xoa.birdmap.top

[U40] Py：打印到标准错误
来源：http://exq.gaohongyu789.top

print("err", file=sys.stderr)
来源：http://yvt.jiagoushi.top

[U41] PHP：初始化 Composer 项目
来源：http://bqn.yongpay.top

composer init;  composer require guzzlehttp/guzzle
来源：http://qym.zhiwuduotai.top

[U42] PHP：PSR-4 自动加载
来源：http://qoa.vehdjk.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kyy.nwbrower.top

[U43] PHP：声明命名空间
来源：http://fvo.cucudq.cn

namespace App\Http;
来源：http://gso.jianghu66.top

[U44] PHP：开启严格类型
来源：http://gnu.ybcxt.top

declare(strict_types=1);
来源：http://piw.bjfxy.top

[U45] PHP：类型声明与返回类型
来源：http://jzi.xuetiantiany.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://aag.fktsv.cn

[U46] PHP：可空类型
来源：http://mnj.sxryk.cn

?string $name = null
来源：http://eui.sufxvd.cn

[U47] PHP：联合类型
来源：http://bzb.yuanzhike.top

int|string $id
来源：http://oog.tianlin.xyz

[U48] PHP：纯枚举
来源：http://cfr.xingfuxueyuan.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xhl.9152youxi.cn

[U49] PHP：只读属性
来源：http://vji.shangyingyoupin.top

public readonly string $name
来源：http://xvo.yanxiufei.cn

[U50] PHP：构造器属性提升
来源：http://elq.kuanghao11.cn

public function __construct(private int $id) {}
来源：http://omi.xuanzx.com

[U51] PHP：数组解构
来源：http://ztz.cdnleiting.top

[$a, $b] = $arr;
来源：http://qvl.zhixingplan.top

[U52] PHP：箭头函数
来源：http://sir.quarkkingdee.top

$double = fn($x) => $x * 2;
来源：http://ppc.ydjk.org.cn

[U53] PHP：空合并运算符
来源：http://txt.hammf.cn

$v = $a ?? $b ?? "default";
来源：http://ncb.andypj.xyz

[U54] PHP：空安全调用
来源：http://nkq.ivvv.top

$obj?->method()
来源：http://wfc.iojbl.cn

[U55] PHP：match 表达式
来源：http://fpm.yvedp.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://idh.gogol.net.cn

[U56] PHP：命名参数
来源：http://oyn.shanyushiyangkeji.top

f(a: 1, b: 2)
来源：http://kph.chenjidiqi.icu


<!-- 参考信息 -->