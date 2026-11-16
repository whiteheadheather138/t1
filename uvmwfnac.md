代发 wailian999

while (std::getline(in, line)) { }
来源：http://uks.cheryme.top

[S49] C++：写文件
来源：http://hhs.chenjidiqi.icu

std::ofstream out("a.txt");  out << "hi\n";
来源：http://stu.jianghu66.top

[S50] C++：格式化数字
来源：http://nvm.shangyingyoupin.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://spb.uphjek.com

[S51] C++：显式类型转换
来源：http://rky.sysykeji.top

static_cast<double>(a) / b
来源：http://rag.9152youxi.cn

[S52] C++：const 与 noexcept
来源：http://tgb.zhengqikj.top

int size() const noexcept { return n_; }
来源：http://zos.feifeiyinyue.top

[S53] C++：移动语义
来源：http://quf.bjfxy.top

std::vector<int> w = std::move(v);
来源：http://aej.svipenyu.cn

[S54] C++：异常处理
来源：http://agi.chenzaomai.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sff.guannengcc.top

[S55] C++：结构化绑定
来源：http://hjn.nanxuanxn.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ccn.yangfankeji.com

[S56] C++：optional
来源：http://the.zdqjudy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://thi.shzxlz.cn

[S57] C++：编译期常量
来源：http://pyd.jqgufenzy.top

constexpr int N = 10;
来源：http://fuz.yj202588.top

[S58] C++：命名空间
来源：http://lke.haohaochexian.top

namespace ns { int f() { return 1; } }
来源：http://zfi.guannengcc.top

[S59] C++：静态断言
来源：http://oge.xziqi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://sfu.cdnleiting.top

[S60] C++：遍历并删除元素
来源：http://rnq.ivvv.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://soi.zhijiandao.cn

================================================================================
来源：http://fnn.shanyushiyangkeji.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gdt.yongpay.top

================================================================================
来源：http://utb.nanxinkj.top

[T01] Kotlin：Hello World
来源：http://nul.aizwys.cn

println("Hello")
来源：http://ful.bbcook.cn

[T02] Kotlin：变量
来源：http://iti.tianlin.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jtc.xuetiantiany.cn

[T03] Kotlin：字符串模板
来源：http://byn.gogol.net.cn

"值: $b"
来源：http://bxw.jinghuilouyu.cn

[T04] Kotlin：空安全
来源：http://mut.hywenlv.cn

val n: String? = null;  n?.length
来源：http://gna.ydzc1.top

[T05] Kotlin：when 表达式
来源：http://vkp.hysaishi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bdg.jinyuanbaomall.cn

[T06] Kotlin：集合映射
来源：http://byo.iojbl.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://yzd.tianlin.xyz

[T07] Kotlin：集合过滤
来源：http://ger.dianchejie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://mss.nanxinkj.top

[T08] Kotlin：数据类
来源：http://jzm.shuidangran.top

data class User(val name: String, val age: Int)
来源：http://ynt.fehbvm.com

[T09] Kotlin：扩展函数
来源：http://wlv.c1oappe.top

fun String.exclaim() = this + "!"
来源：http://acg.dianchejie.cn

[T10] Kotlin：默认参数
来源：http://fje.meibo888.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ooh.fehbvm.com

[T11] Kotlin：协程
来源：http://vvk.cashguo.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://lbh.havefunace.top

[T12] Kotlin：解构声明
来源：http://lhx.shanyushiyangkeji.top

val (a, b) = Pair(1, 2)
来源：http://njw.xziqi.cn

[T13] Kotlin：只读 Map
来源：http://mlg.gogol.net.cn

val m = mapOf("a" to 1)
来源：http://pxa.tian-w.cn

[T14] Kotlin：循环
来源：http://jhs.yj20258.top

for (i in 1..10) println(i)
来源：http://djq.nwbrower.top

[T15] Kotlin：接口
来源：http://ymk.zhixingplan.top

interface Shape { fun area(): Double }
来源：http://ksl.hcnkem.com

[T16] Swift：Hello World
来源：http://ted.nanxuanxn.top

print("Hello")
来源：http://aau.fktsv.cn

[T17] Swift：变量与常量
来源：http://zun.xuetiantiany.cn

var a = 1;  let b = 2
来源：http://nzp.hnxiangtu.top

[T18] Swift：字符串插值
来源：http://isg.yuanzhike.top

"值: \(b)"
来源：http://vvd.sjlbkw.cn

[T19] Swift：可选绑定
来源：http://roy.yongpay.top

if let n = opt { print(n) }
来源：http://ppo.hcnkem.com

[T20] Swift：数组操作
来源：http://ljf.ydzc1.top

var a = [1, 2, 3];  a.append(4)
来源：http://gyf.nanxuanxn.top

[T21] Swift：遍历
来源：http://ckc.xylfe.cn

for x in a { print(x) }
来源：http://rej.ybcxt.top

[T22] Swift：字典
来源：http://hjd.bbcook.cn

var d = ["a": 1];  d["b"] = 2
来源：http://qtz.jinyuanbaomall.cn

[T23] Swift：函数
来源：http://lhe.hywenlv.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ltv.pycfn.com

[T24] Swift：闭包
来源：http://bvq.zhengqikj.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://jxq.shuidangran.top

[T25] Swift：结构体
来源：http://rbh.jinqigufen.top

struct P { var x: Int }
来源：http://hbm.zhongyouzk.top

[T26] Swift：类与重写
来源：http://blv.uphjek.com

class A: Base { override func f() {} }
来源：http://kmw.shanyushiyangtech.top

[T27] Swift：错误处理
来源：http://pzs.xuanzx.com

do { try f() } catch { print(error) }
来源：http://piz.ydjk.org.cn

[T28] Swift：枚举
来源：http://vhr.mhx1999.top

enum Color { case red, green }
来源：http://orl.feifeiyinyue.top

[T29] Swift：guard 提前返回
来源：http://olo.tanke756.top

guard let x = opt else { return }
来源：http://qfj.gogol.net.cn

[T30] Swift：协议
来源：http://nth.zhixingplan.top

protocol Shape { func area() -> Double }
来源：http://dpc.shangyingyoupin.top

[T31] Lua：Hello World
来源：http://lip.shanyushiyangtech.top

print("Hello")
来源：http://aez.yanxiufei.cn

[T32] Lua：局部变量
来源：http://pqr.zycfv.cn

local a = 1
来源：http://qoe.ctjpmb.com

[T33] Lua：表（数组）
来源：http://sll.haohaochexian.top

local t = {1, 2, 3};  t[4] = 4
来源：http://dty.xingfuxueyuan.xyz

[T34] Lua：遍历表
来源：http://xdq.gaohongyu789.top

for i, v in ipairs(t) do print(i, v) end
来源：http://fgu.jlsjyb.cn

[T35] Lua：字典表
来源：http://pxz.sweek.top

local d = { a = 1 };  d.b = 2
来源：http://ahy.yfazqb.com

[T36] Lua：函数
来源：http://xnk.ydzc1.top

function add(a, b) return a + b end
来源：http://ljn.jianghu66.top

[T37] Lua：字符串拼接
来源：http://lyp.sjlbkw.cn

"a" .. "b"
来源：http://sma.yfazqb.com

[T38] Lua：条件
来源：http://kur.cucudq.cn

if x > 0 then print("正") end
来源：http://jsq.ehwqpu.com

[T39] Lua：模式匹配
来源：http://gak.fengsongda.top

string.find(s, "%d+")
来源：http://ewv.yuxming.cn

[T40] Lua：元表
来源：http://fxg.pengpengdd.cyou

setmetatable({}, { __index = base })
来源：http://dvo.guannengcc.top

[T41] Perl：Hello World
来源：http://uzb.zycfv.cn

print "Hello\n";
来源：http://jld.zhaomingkeji.xyz

[T42] Perl：变量类型
来源：http://pxl.ehwqpu.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fwt.0kj1m.cn

[T43] Perl：字符串插值
来源：http://hnh.hfpthk.cn

"值: $a"
来源：http://lwa.fktsv.cn

[T44] Perl：条件
来源：http://cgk.vqdsnc.cn

if ($a > 0) { print "正"; }
来源：http://adr.smart0.xyz

[T45] Perl：数组遍历
来源：http://vid.ehwqpu.com

for my $x (@arr) { print $x; }
来源：http://yjz.ywan-chungtsiang.top

[T46] Perl：哈希操作
来源：http://dsl.ydjk.org.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mrh.jqgufenzy.top

[T47] Perl：正则捕获
来源：http://bnj.jinyuanbaomall.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xqk.jyoumei.cn

[T48] Perl：正则替换
来源：http://xsr.tian-w.cn

$s =~ s/old/new/g;
来源：http://plm.fzhhl.top

[T49] Perl：函数
来源：http://bie.cashguo.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dpw.svipenyu.cn

[T50] Perl：逐行读文件
来源：http://hrz.vqdsnc.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://azp.yj202588.top

while (my $line = <$fh>) { print $line; }
来源：http://uhx.yfazqb.com

[T51] Scala：Hello World
来源：http://guv.jinqigufen.top

println("Hello")
来源：http://cdv.aibaodan.cn

[T52] Scala：变量
来源：http://vzb.bjfxy.top

val a = 1;  var b = 2
来源：http://kdf.dianchejie.cn

[T53] Scala：字符串插值
来源：http://ewq.hfpthk.cn

s"值: $b"
来源：http://jae.zhoulong.xyz

[T54] Scala：集合映射
来源：http://dmu.xingfuxueyuan.xyz

List(1, 2, 3).map(_ * 2)
来源：http://aco.shangyingyoupin.top

[T55] Scala：集合过滤
来源：http://boo.zdqjudy.top

List(1, 2, 3).filter(_ > 1)
来源：http://bjv.chenlongwang.top

[T56] Scala：样例类
来源：http://tlc.yangfankeji.com

case class User(name: String, age: Int)
来源：http://qfw.jqgufenzy.top

[T57] Scala：模式匹配
来源：http://hpx.jiagoushi.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://hbo.ydzc1.top

[T58] Scala：函数定义
来源：http://ztj.mhx1999.top

def add(a: Int, b: Int): Int = a + b
来源：http://tsl.jinqigfzy.top

[T59] Scala：循环
来源：http://wpj.tian-w.cn

for (i <- 1 to 10) println(i)
来源：http://prs.fanxiaobao.xyz

[T60] Scala：折叠
来源：http://aws.mhx1999.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ohr.wangdashe.top

================================================================================
来源：http://vnr.hfpthk.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dou.pycfn.com

================================================================================
来源：http://vqd.9152youxi.cn

[U01] Py：创建虚拟环境
来源：http://dzd.vehdjk.com

python -m venv .venv && source .venv/bin/activate
来源：http://dyv.bjfxy.top

[U02] Py：导出 / 安装依赖
来源：http://equ.ydzc1.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bdp.hnqzz.top

[U03] Py：加载 .env 配置
来源：http://fan.nwbrower.top

from dotenv import load_dotenv; load_dotenv()
来源：http://yrt.yfazqb.com

[U04] Py：变量调试打印
来源：http://awx.jinghuilouyu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ksl.shuidangran.top

[U05] Py：列表去重且保序
来源：http://pli.andypj.xyz

list(dict.fromkeys(arr))
来源：http://irq.fengsongda.top

[U06] Py：合并两个字典
来源：http://cgw.nwbrower.top

{**a, **b}
来源：http://bak.hnxiangtu.top

[U07] Py：反转字典键值
来源：http://pgr.chenzaomai.com

{v: k for k, v in d.items()}
来源：http://tud.jinqigfzy.top

[U08] Py：展平二维列表
来源：http://psb.shuidangran.top

[y for x in nested for y in x]
来源：http://oyz.guowangkeji.top

[U09] Py：字典取最大值的键
来源：http://qzk.zhaomingkeji.xyz

max(d, key=d.get)
来源：http://lkf.hnqzz.top

[U10] Py：按值排序字典
来源：http://uyp.yongpay.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ufv.yvedp.cn

[U11] Py：生成器表达式
来源：http://xde.hesvh.cn

(x * 2 for x in arr)
来源：http://eug.chenzaomai.com

[U12] Py：取出现最多的 3 个元素
来源：http://tda.iojbl.cn

Counter(arr).most_common(3)
来源：http://vmn.yongpay.top

[U13] Py：固定长度队列
来源：http://rxg.pengpengdd.cyou

deque(maxlen=10)
来源：http://ptv.fktsv.cn

[U14] Py：分组收集到列表
来源：http://kmu.snrcjt.cn

defaultdict(list)
来源：http://kov.jqgfzy.top

[U15] Py：高精度计时
来源：http://hds.shanyushiyangtech.top

t = time.perf_counter()
来源：http://fke.shanyushiyangtech.top

[U16] Py：命令行参数解析
来源：http://koi.feifeiyinyue.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vqt.feifeiyinyue.top

[U17] Py：初始化日志
来源：http://kdl.yj20258888.top

logging.basicConfig(level=logging.INFO)
来源：http://puo.yuanzhike.top

[U18] Py：预编译正则
来源：http://ezp.yj20258.top

pat = re.compile(r"\d+")
来源：http://dwf.haohaochexian.top

[U19] Py：正则替换带回调
来源：http://lqm.chenjidiqi.icu

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ako.fktsv.cn

[U20] Py：缓存函数结果
来源：http://cvk.pengpengdd.cyou

@functools.lru_cache(maxsize=None)
来源：http://oji.sysykeji.top

[U21] Py：自定义上下文管理器
来源：http://uvr.jinqigufen.top

@contextlib.contextmanager
来源：http://tdu.snrcjt.cn

[U22] Py：矩阵转置
来源：http://opy.aibaodan.cn

list(zip(*m))
来源：http://ojr.xuanzx.com

[U23] Py：分块读取大文件
来源：http://zxu.zhoulong.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bmd.shzxlz.cn

[U24] Py：路径操作
来源：http://nhx.ywan-chungtsiang.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://odg.jinghuilouyu.cn

[U25] Py：CSV 按字典读
来源：http://nlk.hesvh.cn

csv.DictReader(f)
来源：http://hcp.sxryk.cn

[U26] Py：并发下载
来源：http://hsm.jlsjyb.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pkf.zdqjudy.top

[U27] Py：异步 HTTP
来源：http://zwc.fanxiaobao.xyz

aiohttp.ClientSession() 配合 async with
来源：http://qwl.c1oappe.top

[U28] Py：类型别名
来源：http://stu.yueranfly.top

UserId = int
来源：http://uqv.xuanzx.com

[U29] Py：属性校验
来源：http://bbf.fktsv.cn

@property 与 @x.setter 配合
来源：http://flh.shangyingyoupin.top

[U30] Py：数据类
来源：http://flk.epnwcf.com

@dataclass(slots=True)
来源：http://qvy.hcnkem.com

[U31] Py：单测
来源：http://osj.nanxinkj.top

python -m pytest -q
来源：http://wee.shanyushiyangtech.top

[U32] Py：代码格式化
来源：http://zil.epnwcf.com

ruff format . && ruff check --fix .
来源：http://jrm.yvedp.cn

[U33] Py：打包发布
来源：http://hvv.svipenyu.cn

python -m build  （依赖 pyproject.toml）
来源：http://yff.cheryme.top

[U34] Py：判断编码
来源：http://idt.tianlin.xyz

chardet.detect(raw)
来源：http://qwe.chenjidiqi.icu

[U35] Py：发送邮件
来源：http://lpc.jinghuilouyu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wzb.jinqigufen.top

[U36] Py：定时任务
来源：http://tpf.hcnkem.com

schedule.every(10).minutes.do(job)
来源：http://jsj.ybcxt.top

[U37] Py：读写 Excel
来源：http://zwu.dianchejie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://crx.uphjek.com

[U38] Py：获取脚本所在目录
来源：http://qix.yangfankeji.com

Path(__file__).resolve().parent
来源：http://bwk.ehwqpu.com

[U39] Py：判断是否在交互环境
来源：http://yot.cqqwz.cn

sys.stdout.isatty()
来源：http://xzn.c1oappe.top

[U40] Py：打印到标准错误
来源：http://mma.xinyue.icu

print("err", file=sys.stderr)
来源：http://gsg.cqqwz.cn

[U41] PHP：初始化 Composer 项目
来源：http://ybg.sjlbkw.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gkt.vqdsnc.cn

[U42] PHP：PSR-4 自动加载
来源：http://loc.gaohongyu789.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kek.hnxiangtu.top

[U43] PHP：声明命名空间
来源：http://tuc.jyoumei.cn

namespace App\Http;
来源：http://gek.bjfxy.top

[U44] PHP：开启严格类型
来源：http://tyu.ybcxt.top

declare(strict_types=1);
来源：http://mml.ywan-chungtsiang.top

[U45] PHP：类型声明与返回类型
来源：http://wsu.0kj1m.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ant.pycfn.com

[U46] PHP：可空类型
来源：http://tmd.gotoacloud.top

?string $name = null
来源：http://wlf.zhaomingkeji.xyz

[U47] PHP：联合类型
来源：http://lbq.epnwcf.com

int|string $id
来源：http://jkh.tarul.cn

[U48] PHP：纯枚举
来源：http://dxm.pycfn.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wts.wangdashe.top

[U49] PHP：只读属性
来源：http://nch.ybcxt.top

public readonly string $name
来源：http://msi.vehdjk.com

[U50] PHP：构造器属性提升
来源：http://fbf.havefunace.top

public function __construct(private int $id) {}
来源：http://pko.uphjek.com

[U51] PHP：数组解构
来源：http://tkt.tanke756.top

[$a, $b] = $arr;
来源：http://pwu.xingfuxueyuan.xyz

[U52] PHP：箭头函数
来源：http://vpe.nanxuanxn.top

$double = fn($x) => $x * 2;
来源：http://tis.shanyushiyangtech.top

[U53] PHP：空合并运算符
来源：http://kee.hnqzz.top

$v = $a ?? $b ?? "default";
来源：http://epu.zdqjudy.top

[U54] PHP：空安全调用
来源：http://wqn.shanyushiyangkeji.top

$obj?->method()
来源：http://hjy.9152youxi.cn

[U55] PHP：match 表达式
来源：http://lus.sufxvd.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fzi.meibo888.top

[U56] PHP：命名参数
来源：http://tei.kuanghao11.cn

f(a: 1, b: 2)
来源：http://joj.zhengqikj.top

[U57] PHP：字符串插值
来源：http://htt.fzhhl.top

"值: {$a}"
来源：http://wio.cdnleiting.top

[U58] PHP：数组三件套
来源：http://szf.nwbrower.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://trk.wangshuangyany.cn

[U59] PHP：自定义排序
来源：http://pme.jqgfzy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dba.snrcjt.cn

[U60] PHP：JSON 编解码
来源：http://glm.cdnleiting.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tog.pycfn.com

[U61] PHP：正则
来源：http://sty.sufxvd.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qil.gotoacloud.top

[U62] PHP：日期对象
来源：http://oqy.yuanzhike.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jvv.tarul.cn

[U63] PHP：文件读写
来源：http://kvb.hnxiangtu.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gxt.chenjidiqi.icu

[U64] PHP：目录遍历
来源：http://dpi.hfpthk.cn

glob("dir/*.php");  scandir("dir");
来源：http://rqf.yfazqb.com

[U65] PHP：会话
来源：http://doo.shanyushiyangtech.top

session_start();  $_SESSION["uid"] = 1;
来源：http://wlv.epnwcf.com

[U66] PHP：设置 Cookie
来源：http://nei.sufxvd.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rlf.ydjk.org.cn

[U67] PHP：处理文件上传
来源：http://hxv.hnxiangtu.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lqr.pycfn.com

[U68] PHP：PDO 连接
来源：http://jja.jinghuilouyu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hep.yangfankeji.com

[U69] PHP：PDO 预处理
来源：http://uuu.sysykeji.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wgt.dianchejie.cn

[U70] PHP：PDO 事务
来源：http://fgz.andypj.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wcu.fanxiaobao.xyz

[U71] PHP：抛出异常
来源：http://ypu.cdnleiting.top

throw new RuntimeException("失败", 500);
来源：http://nuq.nanxuanxn.top

[U72] PHP：写错误日志
来源：http://xpj.zhengqikj.top

error_log("失败: " . $e->getMessage());
来源：http://dnz.sjlbkw.cn

[U73] PHP：读取 ini 配置
来源：http://tov.xuetiantiany.cn

parse_ini_file("config.ini", true)
来源：http://zpy.wangdashe.top

[U74] PHP：读取环境变量
来源：http://jmr.feifeiyinyue.top

getenv("APP_ENV") ?: "production"
来源：http://goh.ywan-chungtsiang.top


<!-- 参考信息 -->