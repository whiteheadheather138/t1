代发 wailian999

[S33] C++：vector 增删
来源：http://tlp.meibo888.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bop.hnxiangtu.top

[S34] C++：遍历 vector
来源：http://wkn.ctjpmb.com

for (auto &x : v) { std::cout << x; }
来源：http://nfo.hcnkem.com

[S35] C++：map
来源：http://ety.kuanghao11.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sym.hnqzz.top

[S36] C++：unordered_map
来源：http://sca.hywenlv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mkl.dashuyun.cn

[S37] C++：set
来源：http://fdv.sufxvd.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bkz.tanke756.top

[S38] C++：排序
来源：http://mml.chenjidiqi.icu

std::sort(v.begin(), v.end());
来源：http://vlt.nanxuanxn.top

[S39] C++：自定义比较器排序
来源：http://xen.snrcjt.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tsg.hnxiangtu.top

[S40] C++：查找元素
来源：http://zvc.gzhubu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zjr.zdbjq.cn

[S41] C++：类与构造函数
来源：http://fpa.gogol.net.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://psx.xuanzx.com

[S42] C++：继承与虚函数
来源：http://ckg.sysykeji.top

class B : public Base { public: void f() override {} };
来源：http://liu.fanxiaobao.xyz

[S43] C++：智能指针
来源：http://fgl.dashuyun.cn

auto p = std::make_unique<int>(5);
来源：http://eug.yfazqb.com

[S44] C++：引用传参
来源：http://xfn.vqdsnc.cn

void inc(int &x) { ++x; }
来源：http://ffp.mhx1999.top

[S45] C++：lambda
来源：http://uxk.zhiwuduotai.top

auto add = [](int a, int b) { return a + b; };
来源：http://gvd.dianchejie.cn

[S46] C++：函数模板
来源：http://uiq.bjfxy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jap.snrcjt.cn

[S47] C++：结构化绑定遍历
来源：http://aoc.vqdsnc.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://msq.fehbvm.com

[S48] C++：逐行读文件
来源：http://hzl.feifeiyinyue.top

std::ifstream in("a.txt");  std::string line;
来源：http://xde.chenjidiqi.icu

while (std::getline(in, line)) { }
来源：http://cgk.tianlin.xyz

[S49] C++：写文件
来源：http://buk.guowangkeji.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wwc.zhixingplan.top

[S50] C++：格式化数字
来源：http://ink.pengpengdd.cyou

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://eqa.andypj.xyz

[S51] C++：显式类型转换
来源：http://ptl.nanxinkj.top

static_cast<double>(a) / b
来源：http://yjt.aibaodan.cn

[S52] C++：const 与 noexcept
来源：http://umy.dashuyun.cn

int size() const noexcept { return n_; }
来源：http://lnz.sjlbkw.cn

[S53] C++：移动语义
来源：http://ibx.xylfe.cn

std::vector<int> w = std::move(v);
来源：http://llq.birdmap.top

[S54] C++：异常处理
来源：http://qvr.zhaomingkeji.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://keo.guowangkeji.top

[S55] C++：结构化绑定
来源：http://zxn.jinqigufen.top

auto [a, b] = std::make_pair(1, 2);
来源：http://wvl.chenlongwang.top

[S56] C++：optional
来源：http://xbq.ydzc1.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rxy.yanxiufei.cn

[S57] C++：编译期常量
来源：http://yle.cdnleiting.top

constexpr int N = 10;
来源：http://vmp.yj20258888.top

[S58] C++：命名空间
来源：http://lzh.daxiang520.top

namespace ns { int f() { return 1; } }
来源：http://bed.nanxuanxn.top

[S59] C++：静态断言
来源：http://omn.ydjk.org.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jgv.zhijiandao.cn

[S60] C++：遍历并删除元素
来源：http://zte.xinyue.icu

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://twt.52xcode.cn

================================================================================
来源：http://hzx.hfpthk.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tpd.jyoumei.cn

================================================================================
来源：http://okt.bjfxy.top

[T01] Kotlin：Hello World
来源：http://bxd.fehbvm.com

println("Hello")
来源：http://fer.yuxming.cn

[T02] Kotlin：变量
来源：http://qfy.nanxinkj.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qwt.xziqi.cn

[T03] Kotlin：字符串模板
来源：http://hht.nanxinkj.top

"值: $b"
来源：http://qxr.hfpthk.cn

[T04] Kotlin：空安全
来源：http://xsn.kuanghao11.cn

val n: String? = null;  n?.length
来源：http://tar.tarul.cn

[T05] Kotlin：when 表达式
来源：http://bib.c1oappe.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://win.kuanghao11.cn

[T06] Kotlin：集合映射
来源：http://oqo.gogol.net.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://lai.hesvh.cn

[T07] Kotlin：集合过滤
来源：http://ybl.aibaodan.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://vwr.smart0.xyz

[T08] Kotlin：数据类
来源：http://zkh.bbcook.cn

data class User(val name: String, val age: Int)
来源：http://ivi.jqgufenzy.top

[T09] Kotlin：扩展函数
来源：http://nkk.redwolf501.top

fun String.exclaim() = this + "!"
来源：http://fkd.chenlongwang.top

[T10] Kotlin：默认参数
来源：http://cej.yueranfly.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ykd.jlsjyb.cn

[T11] Kotlin：协程
来源：http://vnh.gzhubu.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://fzd.daxiang520.top

[T12] Kotlin：解构声明
来源：http://tmn.tianlin.xyz

val (a, b) = Pair(1, 2)
来源：http://ufp.c1oappe.top

[T13] Kotlin：只读 Map
来源：http://nfl.zhoulong.xyz

val m = mapOf("a" to 1)
来源：http://yqx.yanxiufei.cn

[T14] Kotlin：循环
来源：http://wvn.yuxming.cn

for (i in 1..10) println(i)
来源：http://vbu.zhixingplan.top

[T15] Kotlin：接口
来源：http://wlr.redwolf501.top

interface Shape { fun area(): Double }
来源：http://zvi.yj20258.top

[T16] Swift：Hello World
来源：http://bmp.zhiwuduotai.top

print("Hello")
来源：http://bqu.svipenyu.cn

[T17] Swift：变量与常量
来源：http://zbz.yuxming.cn

var a = 1;  let b = 2
来源：http://fpu.hysaishi.cn

[T18] Swift：字符串插值
来源：http://hev.xuanzx.com

"值: \(b)"
来源：http://ook.xziqi.cn

[T19] Swift：可选绑定
来源：http://aoh.nanxinkj.top

if let n = opt { print(n) }
来源：http://hje.hysaishi.cn

[T20] Swift：数组操作
来源：http://rbh.zdqjudy.top

var a = [1, 2, 3];  a.append(4)
来源：http://awk.aizwys.cn

[T21] Swift：遍历
来源：http://jnn.aizwys.cn

for x in a { print(x) }
来源：http://sio.yonumen.top

[T22] Swift：字典
来源：http://uxk.cucudq.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fut.yvedp.cn

[T23] Swift：函数
来源：http://vqo.yanxiufei.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://unw.shanyushiyangtech.top

[T24] Swift：闭包
来源：http://zkj.hfpthk.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://tih.shanyushiyangtech.top

[T25] Swift：结构体
来源：http://tit.shangyingyoupin.top

struct P { var x: Int }
来源：http://vjj.c1oappe.top

[T26] Swift：类与重写
来源：http://ftj.tianlin.xyz

class A: Base { override func f() {} }
来源：http://tuf.shzxlz.cn

[T27] Swift：错误处理
来源：http://wzj.hammf.cn

do { try f() } catch { print(error) }
来源：http://itm.pycfn.com

[T28] Swift：枚举
来源：http://wri.jinqigfzy.top

enum Color { case red, green }
来源：http://tvb.ywan-chungtsiang.top

[T29] Swift：guard 提前返回
来源：http://gde.gzhubu.top

guard let x = opt else { return }
来源：http://yxd.yonumen.top

[T30] Swift：协议
来源：http://rtq.hywenlv.cn

protocol Shape { func area() -> Double }
来源：http://nkd.guannengcc.top

[T31] Lua：Hello World
来源：http://jfw.kuanghao11.cn

print("Hello")
来源：http://kmc.yuanzhike.top

[T32] Lua：局部变量
来源：http://imw.cdnleiting.top

local a = 1
来源：http://dml.sufxvd.cn

[T33] Lua：表（数组）
来源：http://mot.vqdsnc.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://eep.wangshuangyany.cn

[T34] Lua：遍历表
来源：http://bzl.shuidangran.top

for i, v in ipairs(t) do print(i, v) end
来源：http://icu.sjlbkw.cn

[T35] Lua：字典表
来源：http://msx.feifeiyinyue.top

local d = { a = 1 };  d.b = 2
来源：http://ypd.hywenlv.cn

[T36] Lua：函数
来源：http://uip.zhiwuduotai.top

function add(a, b) return a + b end
来源：http://rat.zhaomingkeji.xyz

[T37] Lua：字符串拼接
来源：http://rfj.yvedp.cn

"a" .. "b"
来源：http://kel.tianlin.xyz

[T38] Lua：条件
来源：http://qvt.guannengcc.top

if x > 0 then print("正") end
来源：http://yux.jqgufenzy.top

[T39] Lua：模式匹配
来源：http://vlz.jiagoushi.top

string.find(s, "%d+")
来源：http://uob.zhengqikj.top

[T40] Lua：元表
来源：http://ycs.hysaishi.cn

setmetatable({}, { __index = base })
来源：http://ugb.shzxlz.cn

[T41] Perl：Hello World
来源：http://qio.meibo888.top

print "Hello\n";
来源：http://nwo.xylfe.cn

[T42] Perl：变量类型
来源：http://uyg.jinqigufen.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lqr.jianghu66.top

[T43] Perl：字符串插值
来源：http://jjn.yangfankeji.com

"值: $a"
来源：http://bfw.chenzaomai.com

[T44] Perl：条件
来源：http://ovw.nanxuanxn.top

if ($a > 0) { print "正"; }
来源：http://lra.haohaochexian.top

[T45] Perl：数组遍历
来源：http://drw.tanke756.top

for my $x (@arr) { print $x; }
来源：http://sfi.meibo888.top

[T46] Perl：哈希操作
来源：http://dmr.gaohongyu789.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://oco.fanxiaobao.xyz

[T47] Perl：正则捕获
来源：http://bfq.ywan-chungtsiang.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://npl.52xcode.cn

[T48] Perl：正则替换
来源：http://cwc.sysykeji.top

$s =~ s/old/new/g;
来源：http://iye.shzxlz.cn

[T49] Perl：函数
来源：http://qcp.0kj1m.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jaw.shuidangran.top

[T50] Perl：逐行读文件
来源：http://aan.havefunace.top

open my $fh, "<", "a.txt" or die $!;
来源：http://zwq.redwolf501.top

while (my $line = <$fh>) { print $line; }
来源：http://mrx.ehwqpu.com

[T51] Scala：Hello World
来源：http://fca.52xcode.cn

println("Hello")
来源：http://gvn.yongpay.top

[T52] Scala：变量
来源：http://yce.feifeiyinyue.top

val a = 1;  var b = 2
来源：http://aiu.hysaishi.cn

[T53] Scala：字符串插值
来源：http://rwn.yanxiufei.cn

s"值: $b"
来源：http://sal.cdnleiting.top

[T54] Scala：集合映射
来源：http://amm.zhongyouzk.top

List(1, 2, 3).map(_ * 2)
来源：http://xed.yj20258.top

[T55] Scala：集合过滤
来源：http://jyp.ywan-chungtsiang.top

List(1, 2, 3).filter(_ > 1)
来源：http://xkn.shanyushiyangkeji.top

[T56] Scala：样例类
来源：http://oke.aizwys.cn

case class User(name: String, age: Int)
来源：http://fqj.wangshuangyany.cn

[T57] Scala：模式匹配
来源：http://gno.ctjpmb.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://cps.epnwcf.com

[T58] Scala：函数定义
来源：http://jct.fanxiaobao.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://alc.fktsv.cn

[T59] Scala：循环
来源：http://dyy.zhijiandao.cn

for (i <- 1 to 10) println(i)
来源：http://mcq.chenlongwang.top

[T60] Scala：折叠
来源：http://qqx.daxiang520.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rub.zhongyouzk.top

================================================================================
来源：http://lzf.cdnleiting.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kab.shanyushiyangtech.top

================================================================================
来源：http://ocx.shanyushiyangkeji.top

[U01] Py：创建虚拟环境
来源：http://qhl.chenlongwang.top

python -m venv .venv && source .venv/bin/activate
来源：http://rsm.meibo888.top

[U02] Py：导出 / 安装依赖
来源：http://swo.mhx1999.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://aee.aizwys.cn

[U03] Py：加载 .env 配置
来源：http://vva.nwbrower.top

from dotenv import load_dotenv; load_dotenv()
来源：http://wsk.gotoacloud.top

[U04] Py：变量调试打印
来源：http://pfr.snrcjt.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bma.hnqzz.top

[U05] Py：列表去重且保序
来源：http://uoy.shangyingyoupin.top

list(dict.fromkeys(arr))
来源：http://ngm.xuetiantiany.cn

[U06] Py：合并两个字典
来源：http://vgj.cqqwz.cn

{**a, **b}
来源：http://lbr.jianghu66.top

[U07] Py：反转字典键值
来源：http://jdj.daxiang520.top

{v: k for k, v in d.items()}
来源：http://jem.aibaodan.cn

[U08] Py：展平二维列表
来源：http://rbf.feifeiyinyue.top

[y for x in nested for y in x]
来源：http://tpk.fehbvm.com

[U09] Py：字典取最大值的键
来源：http://wai.chenzaomai.com

max(d, key=d.get)
来源：http://kwl.aibaodan.cn

[U10] Py：按值排序字典
来源：http://wym.jianghu66.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gcq.cdnleiting.top

[U11] Py：生成器表达式
来源：http://ohj.yj202588.top

(x * 2 for x in arr)
来源：http://aea.mhx1999.top

[U12] Py：取出现最多的 3 个元素
来源：http://gvu.yfazqb.com

Counter(arr).most_common(3)
来源：http://nex.dianchejie.cn

[U13] Py：固定长度队列
来源：http://ikr.xuetiantiany.cn

deque(maxlen=10)
来源：http://qdt.andypj.xyz

[U14] Py：分组收集到列表
来源：http://dnt.hnqzz.top

defaultdict(list)
来源：http://gtn.yanxiufei.cn

[U15] Py：高精度计时
来源：http://gxh.jlsjyb.cn

t = time.perf_counter()
来源：http://smb.wangdashe.top

[U16] Py：命令行参数解析
来源：http://iyt.hongshengwenyu.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cut.feifeiyinyue.top

[U17] Py：初始化日志
来源：http://ugf.guowangkeji.top

logging.basicConfig(level=logging.INFO)
来源：http://dlt.daxiang520.top

[U18] Py：预编译正则
来源：http://csf.yvedp.cn

pat = re.compile(r"\d+")
来源：http://rca.zhengqikj.top

[U19] Py：正则替换带回调
来源：http://uxy.hywenlv.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ivp.fktsv.cn

[U20] Py：缓存函数结果
来源：http://tfu.316326.xyz

@functools.lru_cache(maxsize=None)
来源：http://vfi.jinqigufen.top

[U21] Py：自定义上下文管理器
来源：http://zky.hnxiangtu.top

@contextlib.contextmanager
来源：http://ltw.iojbl.cn

[U22] Py：矩阵转置
来源：http://bge.yj202588.top

list(zip(*m))
来源：http://xqd.redwolf501.top

[U23] Py：分块读取大文件
来源：http://aml.chenzaomai.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dwi.ctjpmb.com

[U24] Py：路径操作
来源：http://pdx.c1oappe.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dfj.nwbrower.top

[U25] Py：CSV 按字典读
来源：http://jyj.yuxming.cn

csv.DictReader(f)
来源：http://nmg.gotoacloud.top

[U26] Py：并发下载
来源：http://twl.chenlongwang.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ntd.sjlbkw.cn

[U27] Py：异步 HTTP
来源：http://wnn.tanke756.top

aiohttp.ClientSession() 配合 async with
来源：http://xmu.fengsongda.top

[U28] Py：类型别名
来源：http://ell.dianchejie.cn

UserId = int
来源：http://ymp.jqgufenzy.top

[U29] Py：属性校验
来源：http://eyh.ctjpmb.com

@property 与 @x.setter 配合
来源：http://rzx.yuanzhike.top

[U30] Py：数据类
来源：http://rns.shangyingyoupin.top

@dataclass(slots=True)
来源：http://cbq.hesvh.cn

[U31] Py：单测
来源：http://ucf.jinghuilouyu.cn

python -m pytest -q
来源：http://hip.vehdjk.com

[U32] Py：代码格式化
来源：http://eym.vehdjk.com

ruff format . && ruff check --fix .
来源：http://fsy.pycfn.com

[U33] Py：打包发布
来源：http://jeh.hammf.cn

python -m build  （依赖 pyproject.toml）
来源：http://ssp.yuxming.cn

[U34] Py：判断编码
来源：http://ffi.cheryme.top

chardet.detect(raw)
来源：http://ond.0kj1m.cn

[U35] Py：发送邮件
来源：http://niu.nanxinkj.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vdh.jinghuilouyu.cn

[U36] Py：定时任务
来源：http://orf.zhaomingkeji.xyz

schedule.every(10).minutes.do(job)
来源：http://kap.xinyue.icu

[U37] Py：读写 Excel
来源：http://xvj.yuxming.cn

pandas.read_excel / DataFrame.to_excel
来源：http://rqv.svipenyu.cn

[U38] Py：获取脚本所在目录
来源：http://ghc.jyoumei.cn

Path(__file__).resolve().parent
来源：http://tnv.sjlbkw.cn

[U39] Py：判断是否在交互环境
来源：http://pcb.wangdashe.top

sys.stdout.isatty()
来源：http://clm.bbcook.cn

[U40] Py：打印到标准错误
来源：http://xjy.yvedp.cn

print("err", file=sys.stderr)
来源：http://wsl.shuidangran.top

[U41] PHP：初始化 Composer 项目
来源：http://axl.316326.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://xbj.chenjidiqi.icu

[U42] PHP：PSR-4 自动加载
来源：http://wuo.shangyingyoupin.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yll.fengsongda.top

[U43] PHP：声明命名空间
来源：http://vpk.daria6918.cn

namespace App\Http;
来源：http://qll.sysykeji.top

[U44] PHP：开启严格类型
来源：http://dhc.ybcxt.top

declare(strict_types=1);
来源：http://rel.gzhubu.top

[U45] PHP：类型声明与返回类型
来源：http://xum.hnqzz.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://wyl.jqgfzy.top

[U46] PHP：可空类型
来源：http://pmq.havefunace.top

?string $name = null
来源：http://wnu.sxryk.cn

[U47] PHP：联合类型
来源：http://suo.ybcxt.top

int|string $id
来源：http://nre.fehbvm.com

[U48] PHP：纯枚举
来源：http://aga.sufxvd.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bbs.quarkkingdee.top

[U49] PHP：只读属性
来源：http://pir.jyoumei.cn

public readonly string $name
来源：http://wzk.yangfankeji.com

[U50] PHP：构造器属性提升
来源：http://xax.0kj1m.cn

public function __construct(private int $id) {}
来源：http://dty.fzhhl.top

[U51] PHP：数组解构
来源：http://ite.epnwcf.com

[$a, $b] = $arr;
来源：http://ios.zhoulong.xyz

[U52] PHP：箭头函数
来源：http://xgk.yvedp.cn

$double = fn($x) => $x * 2;
来源：http://jyu.ybcxt.top

[U53] PHP：空合并运算符
来源：http://znt.zhaomingkeji.xyz

$v = $a ?? $b ?? "default";
来源：http://xdv.316326.xyz

[U54] PHP：空安全调用
来源：http://jmv.fehbvm.com

$obj?->method()
来源：http://tjv.aibaodan.cn

[U55] PHP：match 表达式
来源：http://ykz.jinqigfzy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dni.yanxiufei.cn

[U56] PHP：命名参数
来源：http://dlj.aizwys.cn

f(a: 1, b: 2)
来源：http://qci.nanxuanxn.top

[U57] PHP：字符串插值
来源：http://uzc.yangfankeji.com

"值: {$a}"
来源：http://lqo.fktsv.cn

[U58] PHP：数组三件套
来源：http://sxy.0kj1m.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://uum.xuanzx.com


<!-- 参考信息 -->