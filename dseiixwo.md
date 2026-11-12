代发 wailian999

[S45] C++：lambda
来源：http://nkp.meibo888.top

auto add = [](int a, int b) { return a + b; };
来源：http://qcu.aibaodan.cn

[S46] C++：函数模板
来源：http://zye.gogol.net.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pqj.jlsjyb.cn

[S47] C++：结构化绑定遍历
来源：http://ett.vqdsnc.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rum.jianghu66.top

[S48] C++：逐行读文件
来源：http://osh.xinyue.icu

std::ifstream in("a.txt");  std::string line;
来源：http://kqy.zycfv.cn

while (std::getline(in, line)) { }
来源：http://pyu.yonumen.top

[S49] C++：写文件
来源：http://hon.iojbl.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://loq.jinyuanbaomall.cn

[S50] C++：格式化数字
来源：http://dbe.shanyushiyangkeji.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yxe.guannengcc.top

[S51] C++：显式类型转换
来源：http://pxs.pycfn.com

static_cast<double>(a) / b
来源：http://lrm.ivvv.top

[S52] C++：const 与 noexcept
来源：http://elt.sufxvd.cn

int size() const noexcept { return n_; }
来源：http://nfv.zhongyouzk.top

[S53] C++：移动语义
来源：http://qdb.ctjpmb.com

std::vector<int> w = std::move(v);
来源：http://sxf.ehwqpu.com

[S54] C++：异常处理
来源：http://fke.yongpay.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://okz.jinqigufen.top

[S55] C++：结构化绑定
来源：http://hkb.guannengcc.top

auto [a, b] = std::make_pair(1, 2);
来源：http://cfm.jinqigfzy.top

[S56] C++：optional
来源：http://csc.jinghuilouyu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://onf.yuxming.cn

[S57] C++：编译期常量
来源：http://lrd.xylfe.cn

constexpr int N = 10;
来源：http://kqj.yj202588.top

[S58] C++：命名空间
来源：http://etk.iojbl.cn

namespace ns { int f() { return 1; } }
来源：http://xym.svipenyu.cn

[S59] C++：静态断言
来源：http://bmw.aibaodan.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zzx.jinghuilouyu.cn

[S60] C++：遍历并删除元素
来源：http://jgc.nanxinkj.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pvl.haohaochexian.top

================================================================================
来源：http://hyf.gzhubu.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wcs.zhoulong.xyz

================================================================================
来源：http://pqr.ppjwa.cn

[T01] Kotlin：Hello World
来源：http://tcu.bjfxy.top

println("Hello")
来源：http://flf.mhx1999.top

[T02] Kotlin：变量
来源：http://bei.dianchejie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fec.nanxuanxn.top

[T03] Kotlin：字符串模板
来源：http://wtb.tanke756.top

"值: $b"
来源：http://owb.daria6918.cn

[T04] Kotlin：空安全
来源：http://kse.chenzaomai.com

val n: String? = null;  n?.length
来源：http://iyj.xuetiantiany.cn

[T05] Kotlin：when 表达式
来源：http://wmu.zdbjq.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cco.chenlongwang.top

[T06] Kotlin：集合映射
来源：http://ivl.hammf.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://mmi.zhengqikj.top

[T07] Kotlin：集合过滤
来源：http://kqm.jyoumei.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://hmy.cqqwz.cn

[T08] Kotlin：数据类
来源：http://gpm.zhiwuduotai.top

data class User(val name: String, val age: Int)
来源：http://mvn.shanyushiyangkeji.top

[T09] Kotlin：扩展函数
来源：http://ili.chenlongwang.top

fun String.exclaim() = this + "!"
来源：http://zfl.daria6918.cn

[T10] Kotlin：默认参数
来源：http://dtn.gzhubu.top

fun greet(name: String = "World") = "Hi $name"
来源：http://xvq.hysaishi.cn

[T11] Kotlin：协程
来源：http://vrb.cqqwz.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://aez.shzxlz.cn

[T12] Kotlin：解构声明
来源：http://hgp.yueranfly.top

val (a, b) = Pair(1, 2)
来源：http://fby.yfazqb.com

[T13] Kotlin：只读 Map
来源：http://scm.svipenyu.cn

val m = mapOf("a" to 1)
来源：http://nul.hnqzz.top

[T14] Kotlin：循环
来源：http://zsp.zhongyouzk.top

for (i in 1..10) println(i)
来源：http://iga.hywenlv.cn

[T15] Kotlin：接口
来源：http://zrm.316326.xyz

interface Shape { fun area(): Double }
来源：http://jae.yuanzhike.top

[T16] Swift：Hello World
来源：http://syv.cucudq.cn

print("Hello")
来源：http://pwr.yuxming.cn

[T17] Swift：变量与常量
来源：http://bni.guowangkeji.top

var a = 1;  let b = 2
来源：http://xyl.meibo888.top

[T18] Swift：字符串插值
来源：http://bbo.chenzaomai.com

"值: \(b)"
来源：http://vge.feifeiyinyue.top

[T19] Swift：可选绑定
来源：http://ter.yj20258888.top

if let n = opt { print(n) }
来源：http://cfx.smart0.xyz

[T20] Swift：数组操作
来源：http://cqc.uphjek.com

var a = [1, 2, 3];  a.append(4)
来源：http://vwe.shuidangran.top

[T21] Swift：遍历
来源：http://gww.zhaomingkeji.xyz

for x in a { print(x) }
来源：http://kab.gaohongyu789.top

[T22] Swift：字典
来源：http://kir.jyoumei.cn

var d = ["a": 1];  d["b"] = 2
来源：http://cri.ybcxt.top

[T23] Swift：函数
来源：http://yya.wangdashe.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pux.jinghuilouyu.cn

[T24] Swift：闭包
来源：http://wwi.yuxming.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://uod.yueranfly.top

[T25] Swift：结构体
来源：http://nhd.pengpengdd.cyou

struct P { var x: Int }
来源：http://crf.bbcook.cn

[T26] Swift：类与重写
来源：http://jgu.shanyushiyangkeji.top

class A: Base { override func f() {} }
来源：http://khi.52xcode.cn

[T27] Swift：错误处理
来源：http://zct.birdmap.top

do { try f() } catch { print(error) }
来源：http://ubm.fktsv.cn

[T28] Swift：枚举
来源：http://xbc.yuxming.cn

enum Color { case red, green }
来源：http://izz.zdbjq.cn

[T29] Swift：guard 提前返回
来源：http://ikh.quarkkingdee.top

guard let x = opt else { return }
来源：http://yia.tianlin.xyz

[T30] Swift：协议
来源：http://omv.daxiang520.top

protocol Shape { func area() -> Double }
来源：http://glu.cucudq.cn

[T31] Lua：Hello World
来源：http://aml.gotoacloud.top

print("Hello")
来源：http://bbj.pengpengdd.cyou

[T32] Lua：局部变量
来源：http://duq.bjfxy.top

local a = 1
来源：http://jqh.jinyuanbaomall.cn

[T33] Lua：表（数组）
来源：http://wst.guowangkeji.top

local t = {1, 2, 3};  t[4] = 4
来源：http://usi.sweek.top

[T34] Lua：遍历表
来源：http://sdi.tarul.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://dqi.fengsongda.top

[T35] Lua：字典表
来源：http://wxy.zhixingplan.top

local d = { a = 1 };  d.b = 2
来源：http://fak.feifeiyinyue.top

[T36] Lua：函数
来源：http://jmw.aibaodan.cn

function add(a, b) return a + b end
来源：http://atn.jyoumei.cn

[T37] Lua：字符串拼接
来源：http://iqf.zhaomingkeji.xyz

"a" .. "b"
来源：http://kut.zycfv.cn

[T38] Lua：条件
来源：http://plk.chenzaomai.com

if x > 0 then print("正") end
来源：http://tvg.shangyingyoupin.top

[T39] Lua：模式匹配
来源：http://opv.chenzaomai.com

string.find(s, "%d+")
来源：http://xnc.gogol.net.cn

[T40] Lua：元表
来源：http://irl.gotoacloud.top

setmetatable({}, { __index = base })
来源：http://xyh.fanxiaobao.xyz

[T41] Perl：Hello World
来源：http://nyb.yvedp.cn

print "Hello\n";
来源：http://ouf.hywenlv.cn

[T42] Perl：变量类型
来源：http://yqz.tianlin.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tpp.zhiwuduotai.top

[T43] Perl：字符串插值
来源：http://xup.hnxiangtu.top

"值: $a"
来源：http://duv.jiagoushi.top

[T44] Perl：条件
来源：http://anc.cheryme.top

if ($a > 0) { print "正"; }
来源：http://pdl.ywan-chungtsiang.top

[T45] Perl：数组遍历
来源：http://fgy.jinqigfzy.top

for my $x (@arr) { print $x; }
来源：http://utr.sufxvd.cn

[T46] Perl：哈希操作
来源：http://slj.dashuyun.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://adw.c1oappe.top

[T47] Perl：正则捕获
来源：http://foq.yueranfly.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://pmt.dashuyun.cn

[T48] Perl：正则替换
来源：http://ztb.sjlbkw.cn

$s =~ s/old/new/g;
来源：http://ybt.feifeiyinyue.top

[T49] Perl：函数
来源：http://ynt.daxiang520.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vux.zhijiandao.cn

[T50] Perl：逐行读文件
来源：http://lou.daxiang520.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ofu.yj20258.top

while (my $line = <$fh>) { print $line; }
来源：http://zxl.feifeiyinyue.top

[T51] Scala：Hello World
来源：http://aut.smart0.xyz

println("Hello")
来源：http://cfy.xylfe.cn

[T52] Scala：变量
来源：http://fry.fanxiaobao.xyz

val a = 1;  var b = 2
来源：http://ejx.ydzc1.top

[T53] Scala：字符串插值
来源：http://dvf.fktsv.cn

s"值: $b"
来源：http://hcw.chenzaomai.com

[T54] Scala：集合映射
来源：http://iuo.cucudq.cn

List(1, 2, 3).map(_ * 2)
来源：http://pju.tarul.cn

[T55] Scala：集合过滤
来源：http://gtu.snrcjt.cn

List(1, 2, 3).filter(_ > 1)
来源：http://rtf.gotoacloud.top

[T56] Scala：样例类
来源：http://kvr.dianchejie.cn

case class User(name: String, age: Int)
来源：http://jac.yfazqb.com

[T57] Scala：模式匹配
来源：http://enr.vqdsnc.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wsh.52xcode.cn

[T58] Scala：函数定义
来源：http://nra.ywan-chungtsiang.top

def add(a: Int, b: Int): Int = a + b
来源：http://xps.jinghuilouyu.cn

[T59] Scala：循环
来源：http://rap.yvedp.cn

for (i <- 1 to 10) println(i)
来源：http://xkf.jinyuanbaomall.cn

[T60] Scala：折叠
来源：http://clk.c1oappe.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vcb.svipenyu.cn

================================================================================
来源：http://xrd.havefunace.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tlr.ivvv.top

================================================================================
来源：http://ppj.xingfuxueyuan.xyz

[U01] Py：创建虚拟环境
来源：http://nxl.shzxlz.cn

python -m venv .venv && source .venv/bin/activate
来源：http://iqx.nanxinkj.top

[U02] Py：导出 / 安装依赖
来源：http://wvf.jqgufenzy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zxr.jyoumei.cn

[U03] Py：加载 .env 配置
来源：http://zpj.guannengcc.top

from dotenv import load_dotenv; load_dotenv()
来源：http://mkc.snrcjt.cn

[U04] Py：变量调试打印
来源：http://smt.jyoumei.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bha.ywan-chungtsiang.top

[U05] Py：列表去重且保序
来源：http://slb.cdnleiting.top

list(dict.fromkeys(arr))
来源：http://hvt.uphjek.com

[U06] Py：合并两个字典
来源：http://twn.havefunace.top

{**a, **b}
来源：http://wvg.aibaodan.cn

[U07] Py：反转字典键值
来源：http://ywr.ybcxt.top

{v: k for k, v in d.items()}
来源：http://scl.jiagoushi.top

[U08] Py：展平二维列表
来源：http://wci.aizwys.cn

[y for x in nested for y in x]
来源：http://yab.shangyingyoupin.top

[U09] Py：字典取最大值的键
来源：http://zfp.jinghuilouyu.cn

max(d, key=d.get)
来源：http://wcy.snrcjt.cn

[U10] Py：按值排序字典
来源：http://qrc.epnwcf.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lkq.gogol.net.cn

[U11] Py：生成器表达式
来源：http://jbc.jqgufenzy.top

(x * 2 for x in arr)
来源：http://lqt.yvedp.cn

[U12] Py：取出现最多的 3 个元素
来源：http://wps.yangfankeji.com

Counter(arr).most_common(3)
来源：http://acv.zhijiandao.cn

[U13] Py：固定长度队列
来源：http://ldn.hammf.cn

deque(maxlen=10)
来源：http://cnl.hesvh.cn

[U14] Py：分组收集到列表
来源：http://eby.dashuyun.cn

defaultdict(list)
来源：http://via.yuxming.cn

[U15] Py：高精度计时
来源：http://gwf.cucudq.cn

t = time.perf_counter()
来源：http://qjm.jinqigfzy.top

[U16] Py：命令行参数解析
来源：http://dpy.xuetiantiany.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ljh.sweek.top

[U17] Py：初始化日志
来源：http://kfg.ybcxt.top

logging.basicConfig(level=logging.INFO)
来源：http://ntz.chenzaomai.com

[U18] Py：预编译正则
来源：http://gqf.zdbjq.cn

pat = re.compile(r"\d+")
来源：http://anb.xingfuxueyuan.xyz

[U19] Py：正则替换带回调
来源：http://ogm.andypj.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vnu.ctjpmb.com

[U20] Py：缓存函数结果
来源：http://lty.gzhubu.top

@functools.lru_cache(maxsize=None)
来源：http://ceh.ehwqpu.com

[U21] Py：自定义上下文管理器
来源：http://oba.jqgfzy.top

@contextlib.contextmanager
来源：http://jyb.jinqigfzy.top

[U22] Py：矩阵转置
来源：http://fxf.xziqi.cn

list(zip(*m))
来源：http://coy.zhaomingkeji.xyz

[U23] Py：分块读取大文件
来源：http://knn.tanke756.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tay.yj20258.top

[U24] Py：路径操作
来源：http://lwi.ppjwa.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jjj.ehwqpu.com

[U25] Py：CSV 按字典读
来源：http://evx.hcnkem.com

csv.DictReader(f)
来源：http://nqo.svipenyu.cn

[U26] Py：并发下载
来源：http://rgl.hywenlv.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ehg.c1oappe.top

[U27] Py：异步 HTTP
来源：http://hyz.zycfv.cn

aiohttp.ClientSession() 配合 async with
来源：http://cec.hywenlv.cn

[U28] Py：类型别名
来源：http://nwv.yj202588.top

UserId = int
来源：http://dwh.andypj.xyz

[U29] Py：属性校验
来源：http://rug.jianghu66.top

@property 与 @x.setter 配合
来源：http://uqy.ybcxt.top

[U30] Py：数据类
来源：http://jkf.0kj1m.cn

@dataclass(slots=True)
来源：http://tmx.yueranfly.top

[U31] Py：单测
来源：http://eqn.cdnleiting.top

python -m pytest -q
来源：http://jgy.tian-w.cn

[U32] Py：代码格式化
来源：http://fcm.nanxinkj.top

ruff format . && ruff check --fix .
来源：http://kmz.xuanzx.com

[U33] Py：打包发布
来源：http://nua.yj20258888.top

python -m build  （依赖 pyproject.toml）
来源：http://fus.cashguo.top

[U34] Py：判断编码
来源：http://qib.sysykeji.top

chardet.detect(raw)
来源：http://tug.hfpthk.cn

[U35] Py：发送邮件
来源：http://cvx.fengsongda.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://aei.ydjk.org.cn

[U36] Py：定时任务
来源：http://joo.sxryk.cn

schedule.every(10).minutes.do(job)
来源：http://fyt.9152youxi.cn

[U37] Py：读写 Excel
来源：http://xya.cdnleiting.top

pandas.read_excel / DataFrame.to_excel
来源：http://ktp.cashguo.top

[U38] Py：获取脚本所在目录
来源：http://jvz.wangshuangyany.cn

Path(__file__).resolve().parent
来源：http://axp.yuanzhike.top

[U39] Py：判断是否在交互环境
来源：http://giv.jianghu66.top

sys.stdout.isatty()
来源：http://vxr.ywan-chungtsiang.top

[U40] Py：打印到标准错误
来源：http://waq.zhixingplan.top

print("err", file=sys.stderr)
来源：http://ufb.gzhubu.top

[U41] PHP：初始化 Composer 项目
来源：http://kqe.aibaodan.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://izm.feifeiyinyue.top

[U42] PHP：PSR-4 自动加载
来源：http://ora.tarul.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://eys.fanxiaobao.xyz

[U43] PHP：声明命名空间
来源：http://srj.xuetiantiany.cn

namespace App\Http;
来源：http://bzv.iojbl.cn

[U44] PHP：开启严格类型
来源：http://ekj.ivvv.top

declare(strict_types=1);
来源：http://tkx.xylfe.cn

[U45] PHP：类型声明与返回类型
来源：http://lfn.yuxming.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://icd.tanke756.top

[U46] PHP：可空类型
来源：http://odd.meibo888.top

?string $name = null
来源：http://zjh.xuetiantiany.cn

[U47] PHP：联合类型
来源：http://fdj.fengsongda.top

int|string $id
来源：http://xgo.epnwcf.com

[U48] PHP：纯枚举
来源：http://ipt.uphjek.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://qek.birdmap.top

[U49] PHP：只读属性
来源：http://hhm.fehbvm.com

public readonly string $name
来源：http://dut.jyoumei.cn

[U50] PHP：构造器属性提升
来源：http://ttd.ydjk.org.cn

public function __construct(private int $id) {}
来源：http://kec.yonumen.top

[U51] PHP：数组解构
来源：http://spp.yonumen.top

[$a, $b] = $arr;
来源：http://tdu.yanxiufei.cn

[U52] PHP：箭头函数
来源：http://wvy.ctjpmb.com

$double = fn($x) => $x * 2;
来源：http://lqd.yfazqb.com

[U53] PHP：空合并运算符
来源：http://ebc.daxiang520.top

$v = $a ?? $b ?? "default";
来源：http://ggp.jianghu66.top

[U54] PHP：空安全调用
来源：http://tpj.ywan-chungtsiang.top

$obj?->method()
来源：http://olo.guannengcc.top

[U55] PHP：match 表达式
来源：http://ehe.guannengcc.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lwd.smart0.xyz

[U56] PHP：命名参数
来源：http://pyt.vehdjk.com

f(a: 1, b: 2)
来源：http://ttp.jyoumei.cn

[U57] PHP：字符串插值
来源：http://frk.fzhhl.top

"值: {$a}"
来源：http://mja.yfazqb.com

[U58] PHP：数组三件套
来源：http://vjk.zycfv.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xfm.hnqzz.top

[U59] PHP：自定义排序
来源：http://vek.zhiwuduotai.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ika.pengpengdd.cyou

[U60] PHP：JSON 编解码
来源：http://abi.shzxlz.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://oyw.0kj1m.cn

[U61] PHP：正则
来源：http://xoi.daria6918.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://uho.kuanghao11.cn

[U62] PHP：日期对象
来源：http://qub.havefunace.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kkd.aibaodan.cn

[U63] PHP：文件读写
来源：http://qsf.hnxiangtu.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zgg.daria6918.cn

[U64] PHP：目录遍历
来源：http://fvi.dashuyun.cn

glob("dir/*.php");  scandir("dir");
来源：http://ezm.mhx1999.top

[U65] PHP：会话
来源：http://keu.c1oappe.top

session_start();  $_SESSION["uid"] = 1;
来源：http://spc.shanyushiyangtech.top

[U66] PHP：设置 Cookie
来源：http://uyj.zdbjq.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rhm.zhaomingkeji.xyz

[U67] PHP：处理文件上传
来源：http://yyp.dashuyun.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zzo.9152youxi.cn

[U68] PHP：PDO 连接
来源：http://arl.sxryk.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://skd.cheryme.top

[U69] PHP：PDO 预处理
来源：http://esn.jianghu66.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kdc.yfazqb.com

[U70] PHP：PDO 事务
来源：http://mpg.wangshuangyany.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hbr.yj202588.top


<!-- 参考信息 -->