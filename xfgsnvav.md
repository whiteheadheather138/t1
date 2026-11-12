代发 wailian999

[S39] C++：自定义比较器排序
来源：http://ivd.ywan-chungtsiang.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mjv.fanxiaobao.xyz

[S40] C++：查找元素
来源：http://hpe.ybcxt.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rvb.fzhhl.top

[S41] C++：类与构造函数
来源：http://rnl.shuidangran.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ezn.xuetiantiany.cn

[S42] C++：继承与虚函数
来源：http://xwu.xingfuxueyuan.xyz

class B : public Base { public: void f() override {} };
来源：http://wiz.zdbjq.cn

[S43] C++：智能指针
来源：http://yxq.cashguo.top

auto p = std::make_unique<int>(5);
来源：http://flp.snrcjt.cn

[S44] C++：引用传参
来源：http://auh.mhx1999.top

void inc(int &x) { ++x; }
来源：http://rov.cdnleiting.top

[S45] C++：lambda
来源：http://zlu.kuanghao11.cn

auto add = [](int a, int b) { return a + b; };
来源：http://sdi.jqgfzy.top

[S46] C++：函数模板
来源：http://mdg.shuidangran.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dds.tarul.cn

[S47] C++：结构化绑定遍历
来源：http://fos.ydzc1.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kvi.xingfuxueyuan.xyz

[S48] C++：逐行读文件
来源：http://lcs.yj20258888.top

std::ifstream in("a.txt");  std::string line;
来源：http://spq.snrcjt.cn

while (std::getline(in, line)) { }
来源：http://abs.dianchejie.cn

[S49] C++：写文件
来源：http://yrd.wangdashe.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kab.snrcjt.cn

[S50] C++：格式化数字
来源：http://gch.smart0.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ksm.yueranfly.top

[S51] C++：显式类型转换
来源：http://gnu.fzhhl.top

static_cast<double>(a) / b
来源：http://yem.birdmap.top

[S52] C++：const 与 noexcept
来源：http://zhy.hnxiangtu.top

int size() const noexcept { return n_; }
来源：http://qtb.hcnkem.com

[S53] C++：移动语义
来源：http://hjh.chenjidiqi.icu

std::vector<int> w = std::move(v);
来源：http://jiu.yj20258.top

[S54] C++：异常处理
来源：http://nzd.haohaochexian.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gpn.zdqjudy.top

[S55] C++：结构化绑定
来源：http://wna.aizwys.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wwy.gogol.net.cn

[S56] C++：optional
来源：http://ter.chenlongwang.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lrf.hysaishi.cn

[S57] C++：编译期常量
来源：http://nfj.daria6918.cn

constexpr int N = 10;
来源：http://vxt.gzhubu.top

[S58] C++：命名空间
来源：http://seu.zhiwuduotai.top

namespace ns { int f() { return 1; } }
来源：http://abz.gzhubu.top

[S59] C++：静态断言
来源：http://rpr.tanke756.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hnn.fanxiaobao.xyz

[S60] C++：遍历并删除元素
来源：http://cys.ppjwa.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wlt.hammf.cn

================================================================================
来源：http://shn.zhixingplan.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mjk.xuetiantiany.cn

================================================================================
来源：http://qhg.hysaishi.cn

[T01] Kotlin：Hello World
来源：http://yfs.guowangkeji.top

println("Hello")
来源：http://emp.hammf.cn

[T02] Kotlin：变量
来源：http://vsz.yangfankeji.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zux.chenlongwang.top

[T03] Kotlin：字符串模板
来源：http://ckk.havefunace.top

"值: $b"
来源：http://rjv.tanke756.top

[T04] Kotlin：空安全
来源：http://bje.yanxiufei.cn

val n: String? = null;  n?.length
来源：http://wma.316326.xyz

[T05] Kotlin：when 表达式
来源：http://jsx.9152youxi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ebh.uphjek.com

[T06] Kotlin：集合映射
来源：http://hiu.vqdsnc.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tit.vehdjk.com

[T07] Kotlin：集合过滤
来源：http://kdk.fengsongda.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://uhz.dianchejie.cn

[T08] Kotlin：数据类
来源：http://hph.yuanzhike.top

data class User(val name: String, val age: Int)
来源：http://xtx.hywenlv.cn

[T09] Kotlin：扩展函数
来源：http://faa.zhaomingkeji.xyz

fun String.exclaim() = this + "!"
来源：http://vjk.sysykeji.top

[T10] Kotlin：默认参数
来源：http://vvs.birdmap.top

fun greet(name: String = "World") = "Hi $name"
来源：http://wit.ydjk.org.cn

[T11] Kotlin：协程
来源：http://jgu.zhiwuduotai.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://hzn.cheryme.top

[T12] Kotlin：解构声明
来源：http://dwu.yuanzhike.top

val (a, b) = Pair(1, 2)
来源：http://pfs.jinqigufen.top

[T13] Kotlin：只读 Map
来源：http://sof.xinyue.icu

val m = mapOf("a" to 1)
来源：http://kzb.jinqigufen.top

[T14] Kotlin：循环
来源：http://wjl.shanyushiyangkeji.top

for (i in 1..10) println(i)
来源：http://guz.yanxiufei.cn

[T15] Kotlin：接口
来源：http://jkt.tian-w.cn

interface Shape { fun area(): Double }
来源：http://iqf.redwolf501.top

[T16] Swift：Hello World
来源：http://wlx.zdqjudy.top

print("Hello")
来源：http://rkc.bbcook.cn

[T17] Swift：变量与常量
来源：http://vvn.feifeiyinyue.top

var a = 1;  let b = 2
来源：http://ywa.hysaishi.cn

[T18] Swift：字符串插值
来源：http://gqb.hysaishi.cn

"值: \(b)"
来源：http://qno.jqgufenzy.top

[T19] Swift：可选绑定
来源：http://yes.sjlbkw.cn

if let n = opt { print(n) }
来源：http://gak.ybcxt.top

[T20] Swift：数组操作
来源：http://jqf.tanke756.top

var a = [1, 2, 3];  a.append(4)
来源：http://iwh.zhengqikj.top

[T21] Swift：遍历
来源：http://cec.hysaishi.cn

for x in a { print(x) }
来源：http://zkz.sysykeji.top

[T22] Swift：字典
来源：http://kwu.nanxinkj.top

var d = ["a": 1];  d["b"] = 2
来源：http://ydh.jianghu66.top

[T23] Swift：函数
来源：http://yyc.ydjk.org.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ihb.zycfv.cn

[T24] Swift：闭包
来源：http://chj.redwolf501.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://onn.zhaomingkeji.xyz

[T25] Swift：结构体
来源：http://kgm.jinqigufen.top

struct P { var x: Int }
来源：http://kqm.jinqigfzy.top

[T26] Swift：类与重写
来源：http://kvb.tarul.cn

class A: Base { override func f() {} }
来源：http://yxj.aibaodan.cn

[T27] Swift：错误处理
来源：http://tks.xuanzx.com

do { try f() } catch { print(error) }
来源：http://mxc.fehbvm.com

[T28] Swift：枚举
来源：http://cbb.dianchejie.cn

enum Color { case red, green }
来源：http://ksc.feifeiyinyue.top

[T29] Swift：guard 提前返回
来源：http://moy.gzhubu.top

guard let x = opt else { return }
来源：http://hee.jyoumei.cn

[T30] Swift：协议
来源：http://veb.cashguo.top

protocol Shape { func area() -> Double }
来源：http://ofq.sjlbkw.cn

[T31] Lua：Hello World
来源：http://hgj.ywan-chungtsiang.top

print("Hello")
来源：http://ezw.yuxming.cn

[T32] Lua：局部变量
来源：http://kgj.aizwys.cn

local a = 1
来源：http://vlq.ctjpmb.com

[T33] Lua：表（数组）
来源：http://pjz.iojbl.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://nfv.zycfv.cn

[T34] Lua：遍历表
来源：http://nse.meibo888.top

for i, v in ipairs(t) do print(i, v) end
来源：http://drm.quarkkingdee.top

[T35] Lua：字典表
来源：http://vwt.tarul.cn

local d = { a = 1 };  d.b = 2
来源：http://qid.jinghuilouyu.cn

[T36] Lua：函数
来源：http://yfi.smart0.xyz

function add(a, b) return a + b end
来源：http://ndm.hnqzz.top

[T37] Lua：字符串拼接
来源：http://sim.nanxuanxn.top

"a" .. "b"
来源：http://mlo.pengpengdd.cyou

[T38] Lua：条件
来源：http://gnj.cdnleiting.top

if x > 0 then print("正") end
来源：http://bpd.zhengqikj.top

[T39] Lua：模式匹配
来源：http://dnh.jyoumei.cn

string.find(s, "%d+")
来源：http://jus.pycfn.com

[T40] Lua：元表
来源：http://uqs.hnxiangtu.top

setmetatable({}, { __index = base })
来源：http://fah.c1oappe.top

[T41] Perl：Hello World
来源：http://pxv.andypj.xyz

print "Hello\n";
来源：http://riz.fehbvm.com

[T42] Perl：变量类型
来源：http://ohg.hfpthk.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xlm.yongpay.top

[T43] Perl：字符串插值
来源：http://ojq.gogol.net.cn

"值: $a"
来源：http://waj.hesvh.cn

[T44] Perl：条件
来源：http://dza.aizwys.cn

if ($a > 0) { print "正"; }
来源：http://yne.316326.xyz

[T45] Perl：数组遍历
来源：http://zjy.yj202588.top

for my $x (@arr) { print $x; }
来源：http://mqs.jianghu66.top

[T46] Perl：哈希操作
来源：http://hzt.shangyingyoupin.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fhf.smart0.xyz

[T47] Perl：正则捕获
来源：http://ykb.fanxiaobao.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://rip.hysaishi.cn

[T48] Perl：正则替换
来源：http://zsj.zhengqikj.top

$s =~ s/old/new/g;
来源：http://hmz.jinyuanbaomall.cn

[T49] Perl：函数
来源：http://vvo.zhixingplan.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nww.bbcook.cn

[T50] Perl：逐行读文件
来源：http://vwo.havefunace.top

open my $fh, "<", "a.txt" or die $!;
来源：http://fkj.chenlongwang.top

while (my $line = <$fh>) { print $line; }
来源：http://ykj.yonumen.top

[T51] Scala：Hello World
来源：http://tjw.52xcode.cn

println("Hello")
来源：http://eul.nanxinkj.top

[T52] Scala：变量
来源：http://dev.redwolf501.top

val a = 1;  var b = 2
来源：http://vid.yangfankeji.com

[T53] Scala：字符串插值
来源：http://txb.jinqigfzy.top

s"值: $b"
来源：http://byz.pengpengdd.cyou

[T54] Scala：集合映射
来源：http://izg.ybcxt.top

List(1, 2, 3).map(_ * 2)
来源：http://bif.hongshengwenyu.top

[T55] Scala：集合过滤
来源：http://iyy.iojbl.cn

List(1, 2, 3).filter(_ > 1)
来源：http://isu.dianchejie.cn

[T56] Scala：样例类
来源：http://aru.hammf.cn

case class User(name: String, age: Int)
来源：http://apf.mhx1999.top

[T57] Scala：模式匹配
来源：http://xlv.xuanzx.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://azg.vehdjk.com

[T58] Scala：函数定义
来源：http://fnl.ppjwa.cn

def add(a: Int, b: Int): Int = a + b
来源：http://epi.bbcook.cn

[T59] Scala：循环
来源：http://ovk.yueranfly.top

for (i <- 1 to 10) println(i)
来源：http://khh.yj20258888.top

[T60] Scala：折叠
来源：http://elo.dashuyun.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ulu.uphjek.com

================================================================================
来源：http://nza.cqqwz.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xcf.hywenlv.cn

================================================================================
来源：http://oqj.hammf.cn

[U01] Py：创建虚拟环境
来源：http://vuu.tianlin.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://ufi.daria6918.cn

[U02] Py：导出 / 安装依赖
来源：http://nxr.vehdjk.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lex.zhaomingkeji.xyz

[U03] Py：加载 .env 配置
来源：http://vjo.shanyushiyangkeji.top

from dotenv import load_dotenv; load_dotenv()
来源：http://vow.yvedp.cn

[U04] Py：变量调试打印
来源：http://rbh.nanxinkj.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rkz.svipenyu.cn

[U05] Py：列表去重且保序
来源：http://aru.havefunace.top

list(dict.fromkeys(arr))
来源：http://gfi.sxryk.cn

[U06] Py：合并两个字典
来源：http://xhd.yj20258888.top

{**a, **b}
来源：http://urm.zdbjq.cn

[U07] Py：反转字典键值
来源：http://uoj.daria6918.cn

{v: k for k, v in d.items()}
来源：http://gpg.jinqigfzy.top

[U08] Py：展平二维列表
来源：http://tls.gzhubu.top

[y for x in nested for y in x]
来源：http://xbv.fzhhl.top

[U09] Py：字典取最大值的键
来源：http://wjq.svipenyu.cn

max(d, key=d.get)
来源：http://lak.jiagoushi.top

[U10] Py：按值排序字典
来源：http://cpg.cashguo.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://chr.fzhhl.top

[U11] Py：生成器表达式
来源：http://tpx.yuanzhike.top

(x * 2 for x in arr)
来源：http://www.dashuyun.cn

[U12] Py：取出现最多的 3 个元素
来源：http://gvw.xziqi.cn

Counter(arr).most_common(3)
来源：http://spy.snrcjt.cn

[U13] Py：固定长度队列
来源：http://erg.kuanghao11.cn

deque(maxlen=10)
来源：http://tmt.redwolf501.top

[U14] Py：分组收集到列表
来源：http://fpn.xziqi.cn

defaultdict(list)
来源：http://gfq.cucudq.cn

[U15] Py：高精度计时
来源：http://lzi.c1oappe.top

t = time.perf_counter()
来源：http://fgw.daxiang520.top

[U16] Py：命令行参数解析
来源：http://hik.ywan-chungtsiang.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zst.xuanzx.com

[U17] Py：初始化日志
来源：http://naf.aizwys.cn

logging.basicConfig(level=logging.INFO)
来源：http://mij.jinqigufen.top

[U18] Py：预编译正则
来源：http://cim.ppjwa.cn

pat = re.compile(r"\d+")
来源：http://nhg.cqqwz.cn

[U19] Py：正则替换带回调
来源：http://ick.hysaishi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://prk.jinyuanbaomall.cn

[U20] Py：缓存函数结果
来源：http://pfy.dashuyun.cn

@functools.lru_cache(maxsize=None)
来源：http://lfz.daxiang520.top

[U21] Py：自定义上下文管理器
来源：http://smi.xuanzx.com

@contextlib.contextmanager
来源：http://gxh.yanxiufei.cn

[U22] Py：矩阵转置
来源：http://ewe.jinghuilouyu.cn

list(zip(*m))
来源：http://mcz.ybcxt.top

[U23] Py：分块读取大文件
来源：http://obz.vqdsnc.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xpp.zycfv.cn

[U24] Py：路径操作
来源：http://hix.smart0.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://sqq.dianchejie.cn

[U25] Py：CSV 按字典读
来源：http://dnx.zhixingplan.top

csv.DictReader(f)
来源：http://ztz.xinyue.icu

[U26] Py：并发下载
来源：http://fnt.yuanzhike.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://juo.hongshengwenyu.top

[U27] Py：异步 HTTP
来源：http://pzz.chenlongwang.top

aiohttp.ClientSession() 配合 async with
来源：http://uvh.jlsjyb.cn

[U28] Py：类型别名
来源：http://gyt.shuidangran.top

UserId = int
来源：http://cya.nanxinkj.top

[U29] Py：属性校验
来源：http://sum.yueranfly.top

@property 与 @x.setter 配合
来源：http://brq.tarul.cn

[U30] Py：数据类
来源：http://hyo.birdmap.top

@dataclass(slots=True)
来源：http://uol.zhijiandao.cn

[U31] Py：单测
来源：http://qez.ydzc1.top

python -m pytest -q
来源：http://jsn.yueranfly.top

[U32] Py：代码格式化
来源：http://svl.ivvv.top

ruff format . && ruff check --fix .
来源：http://tnj.0kj1m.cn

[U33] Py：打包发布
来源：http://qbx.shanyushiyangtech.top

python -m build  （依赖 pyproject.toml）
来源：http://tdb.jlsjyb.cn

[U34] Py：判断编码
来源：http://ueo.fehbvm.com

chardet.detect(raw)
来源：http://ckx.zhiwuduotai.top

[U35] Py：发送邮件
来源：http://eoy.yvedp.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://oss.gotoacloud.top

[U36] Py：定时任务
来源：http://mbk.jiagoushi.top

schedule.every(10).minutes.do(job)
来源：http://ewc.c1oappe.top

[U37] Py：读写 Excel
来源：http://cun.gogol.net.cn

pandas.read_excel / DataFrame.to_excel
来源：http://qvg.zhaomingkeji.xyz

[U38] Py：获取脚本所在目录
来源：http://oww.hfpthk.cn

Path(__file__).resolve().parent
来源：http://uzd.iojbl.cn

[U39] Py：判断是否在交互环境
来源：http://jvo.zhengqikj.top

sys.stdout.isatty()
来源：http://zws.9152youxi.cn

[U40] Py：打印到标准错误
来源：http://zmu.wangshuangyany.cn

print("err", file=sys.stderr)
来源：http://fnb.cqqwz.cn

[U41] PHP：初始化 Composer 项目
来源：http://imx.redwolf501.top

composer init;  composer require guzzlehttp/guzzle
来源：http://qry.hesvh.cn

[U42] PHP：PSR-4 自动加载
来源：http://sfp.zdbjq.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wrt.zhongyouzk.top

[U43] PHP：声明命名空间
来源：http://sfp.c1oappe.top

namespace App\Http;
来源：http://edy.jqgfzy.top

[U44] PHP：开启严格类型
来源：http://lla.zhiwuduotai.top

declare(strict_types=1);
来源：http://fpw.xuetiantiany.cn

[U45] PHP：类型声明与返回类型
来源：http://spg.aizwys.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://efw.sufxvd.cn

[U46] PHP：可空类型
来源：http://mjm.xylfe.cn

?string $name = null
来源：http://jgj.hnqzz.top

[U47] PHP：联合类型
来源：http://ebx.c1oappe.top

int|string $id
来源：http://snf.xziqi.cn

[U48] PHP：纯枚举
来源：http://gmo.fktsv.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://eno.pengpengdd.cyou

[U49] PHP：只读属性
来源：http://bof.mhx1999.top

public readonly string $name
来源：http://tdc.jinyuanbaomall.cn

[U50] PHP：构造器属性提升
来源：http://rno.jinqigufen.top

public function __construct(private int $id) {}
来源：http://kix.hnqzz.top

[U51] PHP：数组解构
来源：http://qlo.hfpthk.cn

[$a, $b] = $arr;
来源：http://xwa.yanxiufei.cn

[U52] PHP：箭头函数
来源：http://xes.gzhubu.top

$double = fn($x) => $x * 2;
来源：http://ozc.dianchejie.cn

[U53] PHP：空合并运算符
来源：http://xpa.nwbrower.top

$v = $a ?? $b ?? "default";
来源：http://ibl.daria6918.cn

[U54] PHP：空安全调用
来源：http://aso.sjlbkw.cn

$obj?->method()
来源：http://sqp.vqdsnc.cn

[U55] PHP：match 表达式
来源：http://gio.hnqzz.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://utm.birdmap.top

[U56] PHP：命名参数
来源：http://kii.meibo888.top

f(a: 1, b: 2)
来源：http://uux.xinyue.icu

[U57] PHP：字符串插值
来源：http://cic.bbcook.cn

"值: {$a}"
来源：http://ryl.fengsongda.top

[U58] PHP：数组三件套
来源：http://eon.shzxlz.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://iep.hywenlv.cn

[U59] PHP：自定义排序
来源：http://pag.pycfn.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ibi.nwbrower.top

[U60] PHP：JSON 编解码
来源：http://ofw.shangyingyoupin.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fra.aibaodan.cn

[U61] PHP：正则
来源：http://uoe.bbcook.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cqo.iojbl.cn

[U62] PHP：日期对象
来源：http://cwy.vqdsnc.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lqc.yangfankeji.com

[U63] PHP：文件读写
来源：http://anp.sweek.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://npy.zhongyouzk.top

[U64] PHP：目录遍历
来源：http://dqv.zhoulong.xyz

glob("dir/*.php");  scandir("dir");
来源：http://tgm.cqqwz.cn


<!-- 参考信息 -->