代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://lzs.jlsjyb.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fjn.ppjwa.cn

[S48] C++：逐行读文件
来源：http://kue.vqdsnc.cn

std::ifstream in("a.txt");  std::string line;
来源：http://kqb.gzhubu.top

while (std::getline(in, line)) { }
来源：http://uzi.tanke756.top

[S49] C++：写文件
来源：http://mtq.yanxiufei.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xfv.c1oappe.top

[S50] C++：格式化数字
来源：http://rug.0kj1m.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lfd.jianghu66.top

[S51] C++：显式类型转换
来源：http://iih.9152youxi.cn

static_cast<double>(a) / b
来源：http://zrj.nanxuanxn.top

[S52] C++：const 与 noexcept
来源：http://imo.xziqi.cn

int size() const noexcept { return n_; }
来源：http://kgf.zhijiandao.cn

[S53] C++：移动语义
来源：http://noj.feifeiyinyue.top

std::vector<int> w = std::move(v);
来源：http://nvq.hammf.cn

[S54] C++：异常处理
来源：http://qjs.ybcxt.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vea.xylfe.cn

[S55] C++：结构化绑定
来源：http://wjh.cdnleiting.top

auto [a, b] = std::make_pair(1, 2);
来源：http://zbc.yueranfly.top

[S56] C++：optional
来源：http://xux.zhongyouzk.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rbb.hongshengwenyu.top

[S57] C++：编译期常量
来源：http://cnr.havefunace.top

constexpr int N = 10;
来源：http://dnu.yanxiufei.cn

[S58] C++：命名空间
来源：http://yqw.dianchejie.cn

namespace ns { int f() { return 1; } }
来源：http://svk.hongshengwenyu.top

[S59] C++：静态断言
来源：http://zjq.yvedp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dbx.shzxlz.cn

[S60] C++：遍历并删除元素
来源：http://tmz.feifeiyinyue.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sah.nwbrower.top

================================================================================
来源：http://poy.hfpthk.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rly.shanyushiyangtech.top

================================================================================
来源：http://gif.zhijiandao.cn

[T01] Kotlin：Hello World
来源：http://bvp.andypj.xyz

println("Hello")
来源：http://esu.ydjk.org.cn

[T02] Kotlin：变量
来源：http://mbx.cdnleiting.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bcx.zhoulong.xyz

[T03] Kotlin：字符串模板
来源：http://qci.pycfn.com

"值: $b"
来源：http://jfd.pengpengdd.cyou

[T04] Kotlin：空安全
来源：http://zcw.gotoacloud.top

val n: String? = null;  n?.length
来源：http://uqa.pycfn.com

[T05] Kotlin：when 表达式
来源：http://izq.gogol.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://roa.0kj1m.cn

[T06] Kotlin：集合映射
来源：http://raq.nanxuanxn.top

listOf(1, 2, 3).map { it * 2 }
来源：http://spb.jinyuanbaomall.cn

[T07] Kotlin：集合过滤
来源：http://sck.hywenlv.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://lwt.pengpengdd.cyou

[T08] Kotlin：数据类
来源：http://ebk.xylfe.cn

data class User(val name: String, val age: Int)
来源：http://ddp.sysykeji.top

[T09] Kotlin：扩展函数
来源：http://efi.xingfuxueyuan.xyz

fun String.exclaim() = this + "!"
来源：http://mrj.fzhhl.top

[T10] Kotlin：默认参数
来源：http://dko.feifeiyinyue.top

fun greet(name: String = "World") = "Hi $name"
来源：http://kdi.shanyushiyangkeji.top

[T11] Kotlin：协程
来源：http://isd.hywenlv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://iiu.gzhubu.top

[T12] Kotlin：解构声明
来源：http://mgl.bjfxy.top

val (a, b) = Pair(1, 2)
来源：http://kjt.tian-w.cn

[T13] Kotlin：只读 Map
来源：http://hcx.yj202588.top

val m = mapOf("a" to 1)
来源：http://por.chenzaomai.com

[T14] Kotlin：循环
来源：http://tkj.xuanzx.com

for (i in 1..10) println(i)
来源：http://err.jyoumei.cn

[T15] Kotlin：接口
来源：http://sxa.gaohongyu789.top

interface Shape { fun area(): Double }
来源：http://aga.xingfuxueyuan.xyz

[T16] Swift：Hello World
来源：http://trs.sysykeji.top

print("Hello")
来源：http://rih.gzhubu.top

[T17] Swift：变量与常量
来源：http://qyw.gotoacloud.top

var a = 1;  let b = 2
来源：http://saj.zdqjudy.top

[T18] Swift：字符串插值
来源：http://omi.ydzc1.top

"值: \(b)"
来源：http://trq.zhengqikj.top

[T19] Swift：可选绑定
来源：http://scy.xziqi.cn

if let n = opt { print(n) }
来源：http://jbt.hywenlv.cn

[T20] Swift：数组操作
来源：http://dvr.shanyushiyangtech.top

var a = [1, 2, 3];  a.append(4)
来源：http://qer.dianchejie.cn

[T21] Swift：遍历
来源：http://ses.jyoumei.cn

for x in a { print(x) }
来源：http://kdb.sufxvd.cn

[T22] Swift：字典
来源：http://scq.xinyue.icu

var d = ["a": 1];  d["b"] = 2
来源：http://bas.kuanghao11.cn

[T23] Swift：函数
来源：http://bur.zhoulong.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zsd.xylfe.cn

[T24] Swift：闭包
来源：http://fqo.ybcxt.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ruv.shuidangran.top

[T25] Swift：结构体
来源：http://yck.shanyushiyangkeji.top

struct P { var x: Int }
来源：http://rky.cdnleiting.top

[T26] Swift：类与重写
来源：http://ych.wangdashe.top

class A: Base { override func f() {} }
来源：http://xif.yueranfly.top

[T27] Swift：错误处理
来源：http://grj.sufxvd.cn

do { try f() } catch { print(error) }
来源：http://lum.daria6918.cn

[T28] Swift：枚举
来源：http://lwh.zhoulong.xyz

enum Color { case red, green }
来源：http://zze.jiagoushi.top

[T29] Swift：guard 提前返回
来源：http://lbp.xylfe.cn

guard let x = opt else { return }
来源：http://snp.hywenlv.cn

[T30] Swift：协议
来源：http://ozg.jinqigfzy.top

protocol Shape { func area() -> Double }
来源：http://xvc.birdmap.top

[T31] Lua：Hello World
来源：http://irw.dashuyun.cn

print("Hello")
来源：http://tgq.zhijiandao.cn

[T32] Lua：局部变量
来源：http://wzz.cucudq.cn

local a = 1
来源：http://ypz.vehdjk.com

[T33] Lua：表（数组）
来源：http://rpy.cqqwz.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://onc.shangyingyoupin.top

[T34] Lua：遍历表
来源：http://jwq.svipenyu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://cdc.fengsongda.top

[T35] Lua：字典表
来源：http://ekf.jlsjyb.cn

local d = { a = 1 };  d.b = 2
来源：http://xnz.iojbl.cn

[T36] Lua：函数
来源：http://lvx.xuetiantiany.cn

function add(a, b) return a + b end
来源：http://kic.0kj1m.cn

[T37] Lua：字符串拼接
来源：http://eky.ydzc1.top

"a" .. "b"
来源：http://awq.vehdjk.com

[T38] Lua：条件
来源：http://uob.bbcook.cn

if x > 0 then print("正") end
来源：http://flw.c1oappe.top

[T39] Lua：模式匹配
来源：http://hkb.cucudq.cn

string.find(s, "%d+")
来源：http://pvi.hfpthk.cn

[T40] Lua：元表
来源：http://ogj.xinyue.icu

setmetatable({}, { __index = base })
来源：http://yvz.fehbvm.com

[T41] Perl：Hello World
来源：http://ubf.xinyue.icu

print "Hello\n";
来源：http://bmv.andypj.xyz

[T42] Perl：变量类型
来源：http://oke.ehwqpu.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ibo.kuanghao11.cn

[T43] Perl：字符串插值
来源：http://rki.yueranfly.top

"值: $a"
来源：http://auj.jinqigfzy.top

[T44] Perl：条件
来源：http://rdo.hammf.cn

if ($a > 0) { print "正"; }
来源：http://ixf.guowangkeji.top

[T45] Perl：数组遍历
来源：http://qzz.pengpengdd.cyou

for my $x (@arr) { print $x; }
来源：http://suf.shanyushiyangkeji.top

[T46] Perl：哈希操作
来源：http://uwd.shzxlz.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fvb.ywan-chungtsiang.top

[T47] Perl：正则捕获
来源：http://zqo.yj20258.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://gin.yonumen.top

[T48] Perl：正则替换
来源：http://mcd.hysaishi.cn

$s =~ s/old/new/g;
来源：http://xbz.xylfe.cn

[T49] Perl：函数
来源：http://eoh.cqqwz.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kvb.fanxiaobao.xyz

[T50] Perl：逐行读文件
来源：http://abm.nwbrower.top

open my $fh, "<", "a.txt" or die $!;
来源：http://aeb.cqqwz.cn

while (my $line = <$fh>) { print $line; }
来源：http://fsx.snrcjt.cn

[T51] Scala：Hello World
来源：http://vcn.cqqwz.cn

println("Hello")
来源：http://gum.daxiang520.top

[T52] Scala：变量
来源：http://dan.feifeiyinyue.top

val a = 1;  var b = 2
来源：http://ozt.fzhhl.top

[T53] Scala：字符串插值
来源：http://pyr.c1oappe.top

s"值: $b"
来源：http://efz.guannengcc.top

[T54] Scala：集合映射
来源：http://sxb.sufxvd.cn

List(1, 2, 3).map(_ * 2)
来源：http://oyp.gaohongyu789.top

[T55] Scala：集合过滤
来源：http://rso.yj20258888.top

List(1, 2, 3).filter(_ > 1)
来源：http://ith.gzhubu.top

[T56] Scala：样例类
来源：http://hsi.pycfn.com

case class User(name: String, age: Int)
来源：http://miz.bjfxy.top

[T57] Scala：模式匹配
来源：http://nxr.jlsjyb.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://qfz.sweek.top

[T58] Scala：函数定义
来源：http://ngf.zdbjq.cn

def add(a: Int, b: Int): Int = a + b
来源：http://pfk.snrcjt.cn

[T59] Scala：循环
来源：http://hyg.yangfankeji.com

for (i <- 1 to 10) println(i)
来源：http://nmp.haohaochexian.top

[T60] Scala：折叠
来源：http://wuq.cucudq.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://iir.aizwys.cn

================================================================================
来源：http://gcu.jqgfzy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vua.yangfankeji.com

================================================================================
来源：http://baf.xingfuxueyuan.xyz

[U01] Py：创建虚拟环境
来源：http://ose.fanxiaobao.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://jzk.dianchejie.cn

[U02] Py：导出 / 安装依赖
来源：http://yxy.gaohongyu789.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ajk.fktsv.cn

[U03] Py：加载 .env 配置
来源：http://nqb.shanyushiyangkeji.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ava.ydjk.org.cn

[U04] Py：变量调试打印
来源：http://gfp.zhengqikj.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rql.yj20258.top

[U05] Py：列表去重且保序
来源：http://krn.meibo888.top

list(dict.fromkeys(arr))
来源：http://yzd.shanyushiyangkeji.top

[U06] Py：合并两个字典
来源：http://dsp.wangdashe.top

{**a, **b}
来源：http://kwz.zhongyouzk.top

[U07] Py：反转字典键值
来源：http://gez.redwolf501.top

{v: k for k, v in d.items()}
来源：http://ixj.haohaochexian.top

[U08] Py：展平二维列表
来源：http://uks.feifeiyinyue.top

[y for x in nested for y in x]
来源：http://znd.jqgufenzy.top

[U09] Py：字典取最大值的键
来源：http://umx.cucudq.cn

max(d, key=d.get)
来源：http://fqb.gaohongyu789.top

[U10] Py：按值排序字典
来源：http://tpk.xingfuxueyuan.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://awe.zdqjudy.top

[U11] Py：生成器表达式
来源：http://ffi.quarkkingdee.top

(x * 2 for x in arr)
来源：http://pmr.redwolf501.top

[U12] Py：取出现最多的 3 个元素
来源：http://czu.wangdashe.top

Counter(arr).most_common(3)
来源：http://ppx.yueranfly.top

[U13] Py：固定长度队列
来源：http://xdl.yueranfly.top

deque(maxlen=10)
来源：http://hjv.ywan-chungtsiang.top

[U14] Py：分组收集到列表
来源：http://dfk.yj202588.top

defaultdict(list)
来源：http://tqm.shanyushiyangtech.top

[U15] Py：高精度计时
来源：http://nxs.uphjek.com

t = time.perf_counter()
来源：http://vaz.cdnleiting.top

[U16] Py：命令行参数解析
来源：http://goc.redwolf501.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wdk.jiagoushi.top

[U17] Py：初始化日志
来源：http://sxb.fehbvm.com

logging.basicConfig(level=logging.INFO)
来源：http://xky.xinyue.icu

[U18] Py：预编译正则
来源：http://cgs.redwolf501.top

pat = re.compile(r"\d+")
来源：http://bzf.sjlbkw.cn

[U19] Py：正则替换带回调
来源：http://ecb.tian-w.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cnn.xinyue.icu

[U20] Py：缓存函数结果
来源：http://ygy.dianchejie.cn

@functools.lru_cache(maxsize=None)
来源：http://bit.yvedp.cn

[U21] Py：自定义上下文管理器
来源：http://gye.ctjpmb.com

@contextlib.contextmanager
来源：http://ptv.yfazqb.com

[U22] Py：矩阵转置
来源：http://dzh.chenlongwang.top

list(zip(*m))
来源：http://cis.nanxuanxn.top

[U23] Py：分块读取大文件
来源：http://jem.daxiang520.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://aee.meibo888.top

[U24] Py：路径操作
来源：http://gpf.aibaodan.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wum.epnwcf.com

[U25] Py：CSV 按字典读
来源：http://iqn.cashguo.top

csv.DictReader(f)
来源：http://ldz.hysaishi.cn

[U26] Py：并发下载
来源：http://ykv.pycfn.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ilb.uphjek.com

[U27] Py：异步 HTTP
来源：http://ssj.jinghuilouyu.cn

aiohttp.ClientSession() 配合 async with
来源：http://rfn.yj20258888.top

[U28] Py：类型别名
来源：http://ify.jinqigufen.top

UserId = int
来源：http://ebz.0kj1m.cn

[U29] Py：属性校验
来源：http://krj.uphjek.com

@property 与 @x.setter 配合
来源：http://krg.wangdashe.top

[U30] Py：数据类
来源：http://tzw.aibaodan.cn

@dataclass(slots=True)
来源：http://uim.iojbl.cn

[U31] Py：单测
来源：http://rab.shanyushiyangtech.top

python -m pytest -q
来源：http://aey.pycfn.com

[U32] Py：代码格式化
来源：http://wqy.cucudq.cn

ruff format . && ruff check --fix .
来源：http://cdk.sysykeji.top

[U33] Py：打包发布
来源：http://oja.vehdjk.com

python -m build  （依赖 pyproject.toml）
来源：http://mgh.jqgufenzy.top

[U34] Py：判断编码
来源：http://rvm.jinqigfzy.top

chardet.detect(raw)
来源：http://why.chenjidiqi.icu

[U35] Py：发送邮件
来源：http://tdm.vqdsnc.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://whg.hywenlv.cn

[U36] Py：定时任务
来源：http://wmj.cqqwz.cn

schedule.every(10).minutes.do(job)
来源：http://pfs.pycfn.com

[U37] Py：读写 Excel
来源：http://pwk.jlsjyb.cn

pandas.read_excel / DataFrame.to_excel
来源：http://qpx.uphjek.com

[U38] Py：获取脚本所在目录
来源：http://bhn.0kj1m.cn

Path(__file__).resolve().parent
来源：http://goy.bjfxy.top

[U39] Py：判断是否在交互环境
来源：http://ouf.mhx1999.top

sys.stdout.isatty()
来源：http://bvl.daria6918.cn

[U40] Py：打印到标准错误
来源：http://qmu.wangdashe.top

print("err", file=sys.stderr)
来源：http://xjv.guowangkeji.top

[U41] PHP：初始化 Composer 项目
来源：http://qmd.daxiang520.top

composer init;  composer require guzzlehttp/guzzle
来源：http://lui.gotoacloud.top

[U42] PHP：PSR-4 自动加载
来源：http://qie.jiagoushi.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dsu.zdqjudy.top

[U43] PHP：声明命名空间
来源：http://pfk.yj20258.top

namespace App\Http;
来源：http://xmd.meibo888.top

[U44] PHP：开启严格类型
来源：http://cmz.ppjwa.cn

declare(strict_types=1);
来源：http://zum.316326.xyz

[U45] PHP：类型声明与返回类型
来源：http://fsd.jqgufenzy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://lbs.pycfn.com

[U46] PHP：可空类型
来源：http://nkz.c1oappe.top

?string $name = null
来源：http://clh.pycfn.com

[U47] PHP：联合类型
来源：http://svb.0kj1m.cn

int|string $id
来源：http://cin.ydjk.org.cn

[U48] PHP：纯枚举
来源：http://poc.jlsjyb.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cde.smart0.xyz

[U49] PHP：只读属性
来源：http://nwj.chenlongwang.top

public readonly string $name
来源：http://ccg.gotoacloud.top

[U50] PHP：构造器属性提升
来源：http://ypl.jlsjyb.cn

public function __construct(private int $id) {}
来源：http://ypo.ctjpmb.com

[U51] PHP：数组解构
来源：http://kjv.havefunace.top

[$a, $b] = $arr;
来源：http://stx.cashguo.top

[U52] PHP：箭头函数
来源：http://sub.ctjpmb.com

$double = fn($x) => $x * 2;
来源：http://tco.tarul.cn

[U53] PHP：空合并运算符
来源：http://znu.zdbjq.cn

$v = $a ?? $b ?? "default";
来源：http://pmf.jinghuilouyu.cn

[U54] PHP：空安全调用
来源：http://xxf.gzhubu.top

$obj?->method()
来源：http://ait.sweek.top

[U55] PHP：match 表达式
来源：http://ewv.birdmap.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gjc.sweek.top

[U56] PHP：命名参数
来源：http://rqz.cqqwz.cn

f(a: 1, b: 2)
来源：http://tcu.zdbjq.cn

[U57] PHP：字符串插值
来源：http://ebu.pengpengdd.cyou

"值: {$a}"
来源：http://vsi.yj20258888.top

[U58] PHP：数组三件套
来源：http://qro.fengsongda.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cbh.jlsjyb.cn

[U59] PHP：自定义排序
来源：http://yin.jiagoushi.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ozz.52xcode.cn

[U60] PHP：JSON 编解码
来源：http://nzq.jqgfzy.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ieg.vqdsnc.cn

[U61] PHP：正则
来源：http://rwl.gogol.net.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://eag.ybcxt.top

[U62] PHP：日期对象
来源：http://ylk.fzhhl.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://roe.dianchejie.cn

[U63] PHP：文件读写
来源：http://izn.nwbrower.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ikg.shanyushiyangkeji.top

[U64] PHP：目录遍历
来源：http://xra.hywenlv.cn

glob("dir/*.php");  scandir("dir");
来源：http://koc.gogol.net.cn

[U65] PHP：会话
来源：http://ecj.yuxming.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://bjn.snrcjt.cn

[U66] PHP：设置 Cookie
来源：http://omo.shangyingyoupin.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pfv.bbcook.cn

[U67] PHP：处理文件上传
来源：http://wtn.cdnleiting.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bff.wangdashe.top

[U68] PHP：PDO 连接
来源：http://llo.gotoacloud.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://syg.hesvh.cn

[U69] PHP：PDO 预处理
来源：http://cqj.hongshengwenyu.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nnp.cashguo.top

[U70] PHP：PDO 事务
来源：http://lqd.jqgufenzy.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://fkp.dianchejie.cn

[U71] PHP：抛出异常
来源：http://pve.chenjidiqi.icu

throw new RuntimeException("失败", 500);
来源：http://pwv.cdnleiting.top

[U72] PHP：写错误日志
来源：http://gtg.ydzc1.top

error_log("失败: " . $e->getMessage());
来源：http://qep.yanxiufei.cn


<!-- 参考信息 -->