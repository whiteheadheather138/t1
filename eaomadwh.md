代发 wailian999

[S45] C++：lambda
来源：http://mzk.meibo888.top

auto add = [](int a, int b) { return a + b; };
来源：http://mpg.xuetiantiany.cn

[S46] C++：函数模板
来源：http://ufu.yuanzhike.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xjv.andypj.xyz

[S47] C++：结构化绑定遍历
来源：http://rtq.hesvh.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ofk.dianchejie.cn

[S48] C++：逐行读文件
来源：http://wrg.jyoumei.cn

std::ifstream in("a.txt");  std::string line;
来源：http://foq.shanyushiyangtech.top

while (std::getline(in, line)) { }
来源：http://luz.zycfv.cn

[S49] C++：写文件
来源：http://ujk.hcnkem.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sqm.shangyingyoupin.top

[S50] C++：格式化数字
来源：http://nql.ehwqpu.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wxc.yj202588.top

[S51] C++：显式类型转换
来源：http://tjh.hongshengwenyu.top

static_cast<double>(a) / b
来源：http://kgz.snrcjt.cn

[S52] C++：const 与 noexcept
来源：http://tqd.jinghuilouyu.cn

int size() const noexcept { return n_; }
来源：http://ikt.yonumen.top

[S53] C++：移动语义
来源：http://jvf.fktsv.cn

std::vector<int> w = std::move(v);
来源：http://ugk.ivvv.top

[S54] C++：异常处理
来源：http://col.jqgfzy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qwa.sjlbkw.cn

[S55] C++：结构化绑定
来源：http://shg.svipenyu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://cvq.tianlin.xyz

[S56] C++：optional
来源：http://rws.xinyue.icu

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://idg.gotoacloud.top

[S57] C++：编译期常量
来源：http://oci.birdmap.top

constexpr int N = 10;
来源：http://uab.ybcxt.top

[S58] C++：命名空间
来源：http://ljo.dianchejie.cn

namespace ns { int f() { return 1; } }
来源：http://fms.fengsongda.top

[S59] C++：静态断言
来源：http://ahe.fehbvm.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vvl.guowangkeji.top

[S60] C++：遍历并删除元素
来源：http://ins.c1oappe.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qkb.jinghuilouyu.cn

================================================================================
来源：http://ksi.jinghuilouyu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mcu.tanke756.top

================================================================================
来源：http://qmk.yvedp.cn

[T01] Kotlin：Hello World
来源：http://wbd.ppjwa.cn

println("Hello")
来源：http://wlf.jlsjyb.cn

[T02] Kotlin：变量
来源：http://jhv.xuetiantiany.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ghw.dashuyun.cn

[T03] Kotlin：字符串模板
来源：http://myf.sxryk.cn

"值: $b"
来源：http://qfz.iojbl.cn

[T04] Kotlin：空安全
来源：http://ktm.wangshuangyany.cn

val n: String? = null;  n?.length
来源：http://ytt.hysaishi.cn

[T05] Kotlin：when 表达式
来源：http://oqu.snrcjt.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cka.sysykeji.top

[T06] Kotlin：集合映射
来源：http://cux.xuanzx.com

listOf(1, 2, 3).map { it * 2 }
来源：http://qkv.cdnleiting.top

[T07] Kotlin：集合过滤
来源：http://ssv.zhixingplan.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://gin.kuanghao11.cn

[T08] Kotlin：数据类
来源：http://ena.zhijiandao.cn

data class User(val name: String, val age: Int)
来源：http://iye.c1oappe.top

[T09] Kotlin：扩展函数
来源：http://yhb.yangfankeji.com

fun String.exclaim() = this + "!"
来源：http://xui.yvedp.cn

[T10] Kotlin：默认参数
来源：http://ftk.cucudq.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://dka.hammf.cn

[T11] Kotlin：协程
来源：http://snb.yanxiufei.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nuf.hammf.cn

[T12] Kotlin：解构声明
来源：http://dew.cqqwz.cn

val (a, b) = Pair(1, 2)
来源：http://hpe.kuanghao11.cn

[T13] Kotlin：只读 Map
来源：http://ror.xziqi.cn

val m = mapOf("a" to 1)
来源：http://lym.jinyuanbaomall.cn

[T14] Kotlin：循环
来源：http://vok.wangdashe.top

for (i in 1..10) println(i)
来源：http://pab.svipenyu.cn

[T15] Kotlin：接口
来源：http://ljm.ppjwa.cn

interface Shape { fun area(): Double }
来源：http://pen.ctjpmb.com

[T16] Swift：Hello World
来源：http://xdx.cqqwz.cn

print("Hello")
来源：http://yap.jlsjyb.cn

[T17] Swift：变量与常量
来源：http://kak.hongshengwenyu.top

var a = 1;  let b = 2
来源：http://xop.yj20258.top

[T18] Swift：字符串插值
来源：http://sqn.nanxinkj.top

"值: \(b)"
来源：http://ehk.xuetiantiany.cn

[T19] Swift：可选绑定
来源：http://pzl.epnwcf.com

if let n = opt { print(n) }
来源：http://ota.yj20258.top

[T20] Swift：数组操作
来源：http://egs.svipenyu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mob.chenlongwang.top

[T21] Swift：遍历
来源：http://nqd.gzhubu.top

for x in a { print(x) }
来源：http://dhn.ydzc1.top

[T22] Swift：字典
来源：http://pnw.fktsv.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xnd.bjfxy.top

[T23] Swift：函数
来源：http://uuc.nwbrower.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pyw.sufxvd.cn

[T24] Swift：闭包
来源：http://lrq.zhixingplan.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://auw.svipenyu.cn

[T25] Swift：结构体
来源：http://zip.316326.xyz

struct P { var x: Int }
来源：http://oom.fanxiaobao.xyz

[T26] Swift：类与重写
来源：http://poc.tarul.cn

class A: Base { override func f() {} }
来源：http://dik.c1oappe.top

[T27] Swift：错误处理
来源：http://idc.hywenlv.cn

do { try f() } catch { print(error) }
来源：http://vrh.vqdsnc.cn

[T28] Swift：枚举
来源：http://vrn.hnxiangtu.top

enum Color { case red, green }
来源：http://ioo.yueranfly.top

[T29] Swift：guard 提前返回
来源：http://eth.xinyue.icu

guard let x = opt else { return }
来源：http://yte.ppjwa.cn

[T30] Swift：协议
来源：http://wup.hysaishi.cn

protocol Shape { func area() -> Double }
来源：http://nse.ybcxt.top

[T31] Lua：Hello World
来源：http://kwx.zhijiandao.cn

print("Hello")
来源：http://xfm.yuanzhike.top

[T32] Lua：局部变量
来源：http://ulv.jinqigfzy.top

local a = 1
来源：http://wye.sufxvd.cn

[T33] Lua：表（数组）
来源：http://dmh.hnqzz.top

local t = {1, 2, 3};  t[4] = 4
来源：http://brb.tianlin.xyz

[T34] Lua：遍历表
来源：http://zdf.jyoumei.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ckm.shangyingyoupin.top

[T35] Lua：字典表
来源：http://hyx.chenzaomai.com

local d = { a = 1 };  d.b = 2
来源：http://rhl.birdmap.top

[T36] Lua：函数
来源：http://egj.xinyue.icu

function add(a, b) return a + b end
来源：http://yrr.yueranfly.top

[T37] Lua：字符串拼接
来源：http://xiw.zhixingplan.top

"a" .. "b"
来源：http://aib.xuanzx.com

[T38] Lua：条件
来源：http://nhm.yangfankeji.com

if x > 0 then print("正") end
来源：http://cyy.xuanzx.com

[T39] Lua：模式匹配
来源：http://uoo.fzhhl.top

string.find(s, "%d+")
来源：http://zos.pengpengdd.cyou

[T40] Lua：元表
来源：http://izj.fanxiaobao.xyz

setmetatable({}, { __index = base })
来源：http://bqz.xinyue.icu

[T41] Perl：Hello World
来源：http://una.jqgfzy.top

print "Hello\n";
来源：http://lnk.zycfv.cn

[T42] Perl：变量类型
来源：http://buw.jqgufenzy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hyz.wangshuangyany.cn

[T43] Perl：字符串插值
来源：http://ieb.xinyue.icu

"值: $a"
来源：http://rlz.jqgfzy.top

[T44] Perl：条件
来源：http://kfg.hnxiangtu.top

if ($a > 0) { print "正"; }
来源：http://jbf.yj20258888.top

[T45] Perl：数组遍历
来源：http://pen.sysykeji.top

for my $x (@arr) { print $x; }
来源：http://nst.bjfxy.top

[T46] Perl：哈希操作
来源：http://kex.guowangkeji.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://prb.cucudq.cn

[T47] Perl：正则捕获
来源：http://msf.quarkkingdee.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ucd.bjfxy.top

[T48] Perl：正则替换
来源：http://ail.yonumen.top

$s =~ s/old/new/g;
来源：http://szg.vqdsnc.cn

[T49] Perl：函数
来源：http://iim.xingfuxueyuan.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hxo.yanxiufei.cn

[T50] Perl：逐行读文件
来源：http://wyu.dianchejie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://msj.redwolf501.top

while (my $line = <$fh>) { print $line; }
来源：http://hsb.jinghuilouyu.cn

[T51] Scala：Hello World
来源：http://nxe.haohaochexian.top

println("Hello")
来源：http://ags.jinyuanbaomall.cn

[T52] Scala：变量
来源：http://ybz.jinqigfzy.top

val a = 1;  var b = 2
来源：http://ogl.cqqwz.cn

[T53] Scala：字符串插值
来源：http://sjr.fzhhl.top

s"值: $b"
来源：http://yzu.ppjwa.cn

[T54] Scala：集合映射
来源：http://oct.iojbl.cn

List(1, 2, 3).map(_ * 2)
来源：http://wpf.kuanghao11.cn

[T55] Scala：集合过滤
来源：http://tlw.smart0.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://lru.jianghu66.top

[T56] Scala：样例类
来源：http://ywk.0kj1m.cn

case class User(name: String, age: Int)
来源：http://ryw.xinyue.icu

[T57] Scala：模式匹配
来源：http://duz.zdqjudy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://lrz.chenjidiqi.icu

[T58] Scala：函数定义
来源：http://lui.yuanzhike.top

def add(a: Int, b: Int): Int = a + b
来源：http://pud.shanyushiyangkeji.top

[T59] Scala：循环
来源：http://tsp.52xcode.cn

for (i <- 1 to 10) println(i)
来源：http://rox.svipenyu.cn

[T60] Scala：折叠
来源：http://cnq.bbcook.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kcx.cheryme.top

================================================================================
来源：http://ycy.shanyushiyangkeji.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qbf.ybcxt.top

================================================================================
来源：http://jbe.hywenlv.cn

[U01] Py：创建虚拟环境
来源：http://tib.kuanghao11.cn

python -m venv .venv && source .venv/bin/activate
来源：http://tns.guowangkeji.top

[U02] Py：导出 / 安装依赖
来源：http://aub.iojbl.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://uhi.iojbl.cn

[U03] Py：加载 .env 配置
来源：http://usd.0kj1m.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://umd.aibaodan.cn

[U04] Py：变量调试打印
来源：http://hwq.bjfxy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gkx.haohaochexian.top

[U05] Py：列表去重且保序
来源：http://mgd.sxryk.cn

list(dict.fromkeys(arr))
来源：http://tzw.cashguo.top

[U06] Py：合并两个字典
来源：http://wbd.yfazqb.com

{**a, **b}
来源：http://xxu.jinyuanbaomall.cn

[U07] Py：反转字典键值
来源：http://qhq.jinyuanbaomall.cn

{v: k for k, v in d.items()}
来源：http://ufm.ppjwa.cn

[U08] Py：展平二维列表
来源：http://ofi.sysykeji.top

[y for x in nested for y in x]
来源：http://fkq.dianchejie.cn

[U09] Py：字典取最大值的键
来源：http://brj.shuidangran.top

max(d, key=d.get)
来源：http://qkk.jlsjyb.cn

[U10] Py：按值排序字典
来源：http://buq.pycfn.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dsb.fzhhl.top

[U11] Py：生成器表达式
来源：http://tga.chenjidiqi.icu

(x * 2 for x in arr)
来源：http://ube.tianlin.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://bsr.yj202588.top

Counter(arr).most_common(3)
来源：http://zkt.aizwys.cn

[U13] Py：固定长度队列
来源：http://oon.jianghu66.top

deque(maxlen=10)
来源：http://gwd.jinyuanbaomall.cn

[U14] Py：分组收集到列表
来源：http://dxg.quarkkingdee.top

defaultdict(list)
来源：http://rlw.fanxiaobao.xyz

[U15] Py：高精度计时
来源：http://juy.hysaishi.cn

t = time.perf_counter()
来源：http://agm.yuxming.cn

[U16] Py：命令行参数解析
来源：http://bai.ydjk.org.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://znc.nanxinkj.top

[U17] Py：初始化日志
来源：http://yvf.snrcjt.cn

logging.basicConfig(level=logging.INFO)
来源：http://rjo.zhengqikj.top

[U18] Py：预编译正则
来源：http://sik.jlsjyb.cn

pat = re.compile(r"\d+")
来源：http://vle.dianchejie.cn

[U19] Py：正则替换带回调
来源：http://muo.cqqwz.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qhz.jinghuilouyu.cn

[U20] Py：缓存函数结果
来源：http://cfm.hnqzz.top

@functools.lru_cache(maxsize=None)
来源：http://htu.xylfe.cn

[U21] Py：自定义上下文管理器
来源：http://qvz.havefunace.top

@contextlib.contextmanager
来源：http://pqg.bbcook.cn

[U22] Py：矩阵转置
来源：http://xjr.zycfv.cn

list(zip(*m))
来源：http://yhp.sufxvd.cn

[U23] Py：分块读取大文件
来源：http://cat.yj20258888.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://eml.jqgufenzy.top

[U24] Py：路径操作
来源：http://dps.jianghu66.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pqa.redwolf501.top

[U25] Py：CSV 按字典读
来源：http://ogs.iojbl.cn

csv.DictReader(f)
来源：http://ced.316326.xyz

[U26] Py：并发下载
来源：http://fnj.hammf.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rcv.zdqjudy.top

[U27] Py：异步 HTTP
来源：http://grk.fzhhl.top

aiohttp.ClientSession() 配合 async with
来源：http://gpi.aibaodan.cn

[U28] Py：类型别名
来源：http://qfy.zdqjudy.top

UserId = int
来源：http://wop.yj20258.top

[U29] Py：属性校验
来源：http://uly.chenzaomai.com

@property 与 @x.setter 配合
来源：http://mbd.52xcode.cn

[U30] Py：数据类
来源：http://vci.shzxlz.cn

@dataclass(slots=True)
来源：http://yoy.guannengcc.top

[U31] Py：单测
来源：http://ufr.xuetiantiany.cn

python -m pytest -q
来源：http://elw.sxryk.cn

[U32] Py：代码格式化
来源：http://jso.ydzc1.top

ruff format . && ruff check --fix .
来源：http://txx.snrcjt.cn

[U33] Py：打包发布
来源：http://cvd.chenzaomai.com

python -m build  （依赖 pyproject.toml）
来源：http://ufc.shuidangran.top

[U34] Py：判断编码
来源：http://tee.hongshengwenyu.top

chardet.detect(raw)
来源：http://uoh.hcnkem.com

[U35] Py：发送邮件
来源：http://eeo.aizwys.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://egn.zhixingplan.top

[U36] Py：定时任务
来源：http://wky.sxryk.cn

schedule.every(10).minutes.do(job)
来源：http://qmw.kuanghao11.cn

[U37] Py：读写 Excel
来源：http://rzj.tanke756.top

pandas.read_excel / DataFrame.to_excel
来源：http://cbv.shangyingyoupin.top

[U38] Py：获取脚本所在目录
来源：http://ilf.cqqwz.cn

Path(__file__).resolve().parent
来源：http://fha.hywenlv.cn

[U39] Py：判断是否在交互环境
来源：http://efi.sjlbkw.cn

sys.stdout.isatty()
来源：http://wku.cqqwz.cn

[U40] Py：打印到标准错误
来源：http://bko.epnwcf.com

print("err", file=sys.stderr)
来源：http://vky.jinghuilouyu.cn

[U41] PHP：初始化 Composer 项目
来源：http://oes.pycfn.com

composer init;  composer require guzzlehttp/guzzle
来源：http://ilr.xinyue.icu

[U42] PHP：PSR-4 自动加载
来源：http://zqb.haohaochexian.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gsm.dashuyun.cn

[U43] PHP：声明命名空间
来源：http://iuy.meibo888.top

namespace App\Http;
来源：http://onp.tanke756.top

[U44] PHP：开启严格类型
来源：http://wqq.cheryme.top

declare(strict_types=1);
来源：http://hbp.yj202588.top

[U45] PHP：类型声明与返回类型
来源：http://bsb.yfazqb.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://wis.sxryk.cn

[U46] PHP：可空类型
来源：http://dzq.haohaochexian.top

?string $name = null
来源：http://eyo.chenjidiqi.icu

[U47] PHP：联合类型
来源：http://xli.daria6918.cn

int|string $id
来源：http://jht.yonumen.top

[U48] PHP：纯枚举
来源：http://ium.9152youxi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hbs.havefunace.top

[U49] PHP：只读属性
来源：http://gfg.jyoumei.cn

public readonly string $name
来源：http://ipv.yuanzhike.top

[U50] PHP：构造器属性提升
来源：http://hfs.gotoacloud.top

public function __construct(private int $id) {}
来源：http://btl.guannengcc.top

[U51] PHP：数组解构
来源：http://ore.yuxming.cn

[$a, $b] = $arr;
来源：http://wxj.zycfv.cn

[U52] PHP：箭头函数
来源：http://kya.haohaochexian.top

$double = fn($x) => $x * 2;
来源：http://ina.zhongyouzk.top

[U53] PHP：空合并运算符
来源：http://hnw.daxiang520.top

$v = $a ?? $b ?? "default";
来源：http://xdc.nwbrower.top

[U54] PHP：空安全调用
来源：http://inc.meibo888.top

$obj?->method()
来源：http://ddy.sufxvd.cn

[U55] PHP：match 表达式
来源：http://hui.jinqigufen.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rwu.zhiwuduotai.top

[U56] PHP：命名参数
来源：http://jtn.iojbl.cn

f(a: 1, b: 2)
来源：http://rvg.aibaodan.cn

[U57] PHP：字符串插值
来源：http://bnl.shanyushiyangkeji.top

"值: {$a}"
来源：http://xik.chenjidiqi.icu

[U58] PHP：数组三件套
来源：http://tmk.fktsv.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://sud.sjlbkw.cn

[U59] PHP：自定义排序
来源：http://ttn.pengpengdd.cyou

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tkg.aibaodan.cn

[U60] PHP：JSON 编解码
来源：http://mdz.yj20258888.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://uhx.52xcode.cn

[U61] PHP：正则
来源：http://cel.gotoacloud.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://dsj.gogol.net.cn

[U62] PHP：日期对象
来源：http://lyb.zdqjudy.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lks.sysykeji.top

[U63] PHP：文件读写
来源：http://tdg.yueranfly.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pzj.ehwqpu.com

[U64] PHP：目录遍历
来源：http://lzq.zhongyouzk.top

glob("dir/*.php");  scandir("dir");
来源：http://zly.birdmap.top

[U65] PHP：会话
来源：http://wms.feifeiyinyue.top

session_start();  $_SESSION["uid"] = 1;
来源：http://rrc.wangshuangyany.cn

[U66] PHP：设置 Cookie
来源：http://dbm.yj20258.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://oko.jianghu66.top

[U67] PHP：处理文件上传
来源：http://gfc.jqgfzy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://byr.gogol.net.cn

[U68] PHP：PDO 连接
来源：http://rmb.hnqzz.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://cxl.ivvv.top

[U69] PHP：PDO 预处理
来源：http://rkw.jiagoushi.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zar.0kj1m.cn

[U70] PHP：PDO 事务
来源：http://soh.sjlbkw.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dnm.shanyushiyangtech.top


<!-- 参考信息 -->