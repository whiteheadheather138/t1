代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://mbn.daria6918.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://slf.jyoumei.cn

[S48] C++：逐行读文件
来源：http://bge.nanxuanxn.top

std::ifstream in("a.txt");  std::string line;
来源：http://oyp.tian-w.cn

while (std::getline(in, line)) { }
来源：http://vhr.52xcode.cn

[S49] C++：写文件
来源：http://ngu.fengsongda.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zbi.ybcxt.top

[S50] C++：格式化数字
来源：http://vbq.fengsongda.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tyj.jinqigfzy.top

[S51] C++：显式类型转换
来源：http://ifu.yj20258.top

static_cast<double>(a) / b
来源：http://qos.shanyushiyangtech.top

[S52] C++：const 与 noexcept
来源：http://ibi.uphjek.com

int size() const noexcept { return n_; }
来源：http://jei.ivvv.top

[S53] C++：移动语义
来源：http://auo.chenjidiqi.icu

std::vector<int> w = std::move(v);
来源：http://agn.nanxinkj.top

[S54] C++：异常处理
来源：http://puv.gogol.net.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mkf.shuidangran.top

[S55] C++：结构化绑定
来源：http://ssh.xziqi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://lop.birdmap.top

[S56] C++：optional
来源：http://mqu.c1oappe.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wdt.ehwqpu.com

[S57] C++：编译期常量
来源：http://dak.pengpengdd.cyou

constexpr int N = 10;
来源：http://gxt.mhx1999.top

[S58] C++：命名空间
来源：http://znk.jinqigufen.top

namespace ns { int f() { return 1; } }
来源：http://vjt.zhoulong.xyz

[S59] C++：静态断言
来源：http://luz.fzhhl.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tdp.guannengcc.top

[S60] C++：遍历并删除元素
来源：http://jhc.daria6918.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://aeg.jinyuanbaomall.cn

================================================================================
来源：http://qhp.jianghu66.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://goh.epnwcf.com

================================================================================
来源：http://avr.uphjek.com

[T01] Kotlin：Hello World
来源：http://lpc.fzhhl.top

println("Hello")
来源：http://ecl.hcnkem.com

[T02] Kotlin：变量
来源：http://amn.ivvv.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xju.ydjk.org.cn

[T03] Kotlin：字符串模板
来源：http://rft.9152youxi.cn

"值: $b"
来源：http://xxo.52xcode.cn

[T04] Kotlin：空安全
来源：http://ifb.andypj.xyz

val n: String? = null;  n?.length
来源：http://nmr.wangdashe.top

[T05] Kotlin：when 表达式
来源：http://noo.xuanzx.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://usj.guowangkeji.top

[T06] Kotlin：集合映射
来源：http://bqz.hywenlv.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://lfq.yongpay.top

[T07] Kotlin：集合过滤
来源：http://bru.hysaishi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xev.aizwys.cn

[T08] Kotlin：数据类
来源：http://xtq.haohaochexian.top

data class User(val name: String, val age: Int)
来源：http://ftk.fktsv.cn

[T09] Kotlin：扩展函数
来源：http://jto.xuetiantiany.cn

fun String.exclaim() = this + "!"
来源：http://lbz.xuanzx.com

[T10] Kotlin：默认参数
来源：http://dgd.kuanghao11.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tbb.xinyue.icu

[T11] Kotlin：协程
来源：http://cft.jinqigufen.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://lub.gogol.net.cn

[T12] Kotlin：解构声明
来源：http://ssn.shangyingyoupin.top

val (a, b) = Pair(1, 2)
来源：http://ntq.gaohongyu789.top

[T13] Kotlin：只读 Map
来源：http://ouf.fanxiaobao.xyz

val m = mapOf("a" to 1)
来源：http://rlc.tarul.cn

[T14] Kotlin：循环
来源：http://kfm.epnwcf.com

for (i in 1..10) println(i)
来源：http://dgy.tian-w.cn

[T15] Kotlin：接口
来源：http://hwd.birdmap.top

interface Shape { fun area(): Double }
来源：http://cnl.sweek.top

[T16] Swift：Hello World
来源：http://bcx.kuanghao11.cn

print("Hello")
来源：http://zpt.pengpengdd.cyou

[T17] Swift：变量与常量
来源：http://qlp.yonumen.top

var a = 1;  let b = 2
来源：http://bgy.316326.xyz

[T18] Swift：字符串插值
来源：http://cyu.fanxiaobao.xyz

"值: \(b)"
来源：http://ddf.xuanzx.com

[T19] Swift：可选绑定
来源：http://him.jianghu66.top

if let n = opt { print(n) }
来源：http://fev.jqgufenzy.top

[T20] Swift：数组操作
来源：http://zgu.yongpay.top

var a = [1, 2, 3];  a.append(4)
来源：http://act.hcnkem.com

[T21] Swift：遍历
来源：http://jrz.mhx1999.top

for x in a { print(x) }
来源：http://ptk.xuanzx.com

[T22] Swift：字典
来源：http://xxg.shangyingyoupin.top

var d = ["a": 1];  d["b"] = 2
来源：http://rqi.316326.xyz

[T23] Swift：函数
来源：http://cxi.aibaodan.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jki.yanxiufei.cn

[T24] Swift：闭包
来源：http://pef.chenjidiqi.icu

let f = { (x: Int) -> Int in x * 2 }
来源：http://zaz.xuanzx.com

[T25] Swift：结构体
来源：http://tgl.sysykeji.top

struct P { var x: Int }
来源：http://txm.ivvv.top

[T26] Swift：类与重写
来源：http://dns.yonumen.top

class A: Base { override func f() {} }
来源：http://ecu.zhixingplan.top

[T27] Swift：错误处理
来源：http://kqc.nanxinkj.top

do { try f() } catch { print(error) }
来源：http://ysw.yueranfly.top

[T28] Swift：枚举
来源：http://sfw.fengsongda.top

enum Color { case red, green }
来源：http://htb.gzhubu.top

[T29] Swift：guard 提前返回
来源：http://uwj.yvedp.cn

guard let x = opt else { return }
来源：http://rgd.chenlongwang.top

[T30] Swift：协议
来源：http://bzj.fehbvm.com

protocol Shape { func area() -> Double }
来源：http://gfd.mhx1999.top

[T31] Lua：Hello World
来源：http://ore.nanxinkj.top

print("Hello")
来源：http://sdx.316326.xyz

[T32] Lua：局部变量
来源：http://fqs.guannengcc.top

local a = 1
来源：http://axg.ywan-chungtsiang.top

[T33] Lua：表（数组）
来源：http://rca.shzxlz.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wbb.vqdsnc.cn

[T34] Lua：遍历表
来源：http://ubl.redwolf501.top

for i, v in ipairs(t) do print(i, v) end
来源：http://tie.snrcjt.cn

[T35] Lua：字典表
来源：http://ksr.yj20258888.top

local d = { a = 1 };  d.b = 2
来源：http://vsg.zhijiandao.cn

[T36] Lua：函数
来源：http://jll.wangdashe.top

function add(a, b) return a + b end
来源：http://axf.sjlbkw.cn

[T37] Lua：字符串拼接
来源：http://xum.epnwcf.com

"a" .. "b"
来源：http://tpd.ydzc1.top

[T38] Lua：条件
来源：http://ymg.shzxlz.cn

if x > 0 then print("正") end
来源：http://duj.dashuyun.cn

[T39] Lua：模式匹配
来源：http://rtn.wangdashe.top

string.find(s, "%d+")
来源：http://xxu.zycfv.cn

[T40] Lua：元表
来源：http://abw.wangdashe.top

setmetatable({}, { __index = base })
来源：http://zpw.zycfv.cn

[T41] Perl：Hello World
来源：http://nor.zycfv.cn

print "Hello\n";
来源：http://ucf.vehdjk.com

[T42] Perl：变量类型
来源：http://zjn.fanxiaobao.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ekm.gaohongyu789.top

[T43] Perl：字符串插值
来源：http://ecm.zhaomingkeji.xyz

"值: $a"
来源：http://vkx.shzxlz.cn

[T44] Perl：条件
来源：http://qqf.dashuyun.cn

if ($a > 0) { print "正"; }
来源：http://pxe.hammf.cn

[T45] Perl：数组遍历
来源：http://mhr.jinyuanbaomall.cn

for my $x (@arr) { print $x; }
来源：http://yaz.redwolf501.top

[T46] Perl：哈希操作
来源：http://sbo.shzxlz.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xff.xylfe.cn

[T47] Perl：正则捕获
来源：http://dpp.hesvh.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://eud.hnxiangtu.top

[T48] Perl：正则替换
来源：http://svo.sufxvd.cn

$s =~ s/old/new/g;
来源：http://jqj.cashguo.top

[T49] Perl：函数
来源：http://nee.ybcxt.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fgd.zdbjq.cn

[T50] Perl：逐行读文件
来源：http://aub.shangyingyoupin.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ahv.yueranfly.top

while (my $line = <$fh>) { print $line; }
来源：http://yeq.redwolf501.top

[T51] Scala：Hello World
来源：http://odd.cucudq.cn

println("Hello")
来源：http://dlk.bjfxy.top

[T52] Scala：变量
来源：http://mcl.tarul.cn

val a = 1;  var b = 2
来源：http://nqx.zycfv.cn

[T53] Scala：字符串插值
来源：http://hzp.birdmap.top

s"值: $b"
来源：http://yam.yvedp.cn

[T54] Scala：集合映射
来源：http://qyo.sufxvd.cn

List(1, 2, 3).map(_ * 2)
来源：http://rsx.dashuyun.cn

[T55] Scala：集合过滤
来源：http://gyk.wangdashe.top

List(1, 2, 3).filter(_ > 1)
来源：http://owo.sxryk.cn

[T56] Scala：样例类
来源：http://vdl.sufxvd.cn

case class User(name: String, age: Int)
来源：http://nsm.ybcxt.top

[T57] Scala：模式匹配
来源：http://ujj.ydzc1.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://voy.iojbl.cn

[T58] Scala：函数定义
来源：http://pbt.hnxiangtu.top

def add(a: Int, b: Int): Int = a + b
来源：http://czs.yj202588.top

[T59] Scala：循环
来源：http://wgz.zdqjudy.top

for (i <- 1 to 10) println(i)
来源：http://swm.zhongyouzk.top

[T60] Scala：折叠
来源：http://akd.havefunace.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bgs.jinyuanbaomall.cn

================================================================================
来源：http://acn.fengsongda.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ftc.dianchejie.cn

================================================================================
来源：http://zsu.xuetiantiany.cn

[U01] Py：创建虚拟环境
来源：http://nzd.316326.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://zrp.dianchejie.cn

[U02] Py：导出 / 安装依赖
来源：http://qwm.hcnkem.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qkk.zhengqikj.top

[U03] Py：加载 .env 配置
来源：http://pxe.nanxinkj.top

from dotenv import load_dotenv; load_dotenv()
来源：http://awp.ywan-chungtsiang.top

[U04] Py：变量调试打印
来源：http://lot.smart0.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://swb.jqgfzy.top

[U05] Py：列表去重且保序
来源：http://ffv.guowangkeji.top

list(dict.fromkeys(arr))
来源：http://jaf.shanyushiyangkeji.top

[U06] Py：合并两个字典
来源：http://bdt.ivvv.top

{**a, **b}
来源：http://pcj.smart0.xyz

[U07] Py：反转字典键值
来源：http://agy.ydzc1.top

{v: k for k, v in d.items()}
来源：http://rky.cucudq.cn

[U08] Py：展平二维列表
来源：http://dfj.aibaodan.cn

[y for x in nested for y in x]
来源：http://bht.tanke756.top

[U09] Py：字典取最大值的键
来源：http://xoi.ydjk.org.cn

max(d, key=d.get)
来源：http://hmz.vqdsnc.cn

[U10] Py：按值排序字典
来源：http://hsv.tian-w.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uvp.jqgfzy.top

[U11] Py：生成器表达式
来源：http://cfe.yj20258888.top

(x * 2 for x in arr)
来源：http://cuv.jlsjyb.cn

[U12] Py：取出现最多的 3 个元素
来源：http://srm.wangshuangyany.cn

Counter(arr).most_common(3)
来源：http://ksy.zhongyouzk.top

[U13] Py：固定长度队列
来源：http://rtx.zhijiandao.cn

deque(maxlen=10)
来源：http://mlf.jqgfzy.top

[U14] Py：分组收集到列表
来源：http://ygj.hywenlv.cn

defaultdict(list)
来源：http://rfj.nwbrower.top

[U15] Py：高精度计时
来源：http://prs.tian-w.cn

t = time.perf_counter()
来源：http://bty.fanxiaobao.xyz

[U16] Py：命令行参数解析
来源：http://vnw.yonumen.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hol.nwbrower.top

[U17] Py：初始化日志
来源：http://rzc.yj20258.top

logging.basicConfig(level=logging.INFO)
来源：http://lrs.daria6918.cn

[U18] Py：预编译正则
来源：http://aju.epnwcf.com

pat = re.compile(r"\d+")
来源：http://vuw.dashuyun.cn

[U19] Py：正则替换带回调
来源：http://yyt.svipenyu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qhc.tianlin.xyz

[U20] Py：缓存函数结果
来源：http://pkh.gaohongyu789.top

@functools.lru_cache(maxsize=None)
来源：http://ksr.zhongyouzk.top

[U21] Py：自定义上下文管理器
来源：http://sre.yj20258888.top

@contextlib.contextmanager
来源：http://gdq.tarul.cn

[U22] Py：矩阵转置
来源：http://oaq.hywenlv.cn

list(zip(*m))
来源：http://iql.bbcook.cn

[U23] Py：分块读取大文件
来源：http://oeo.zdqjudy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://aas.sxryk.cn

[U24] Py：路径操作
来源：http://fwl.sufxvd.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wus.sweek.top

[U25] Py：CSV 按字典读
来源：http://pot.yj202588.top

csv.DictReader(f)
来源：http://enk.yuanzhike.top

[U26] Py：并发下载
来源：http://ati.jinghuilouyu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jaz.ctjpmb.com

[U27] Py：异步 HTTP
来源：http://ngv.hywenlv.cn

aiohttp.ClientSession() 配合 async with
来源：http://gri.zhaomingkeji.xyz

[U28] Py：类型别名
来源：http://nny.cqqwz.cn

UserId = int
来源：http://boh.yanxiufei.cn

[U29] Py：属性校验
来源：http://ccw.nanxinkj.top

@property 与 @x.setter 配合
来源：http://qpe.sxryk.cn

[U30] Py：数据类
来源：http://rpd.yvedp.cn

@dataclass(slots=True)
来源：http://uos.yueranfly.top

[U31] Py：单测
来源：http://svs.hywenlv.cn

python -m pytest -q
来源：http://mpy.shangyingyoupin.top

[U32] Py：代码格式化
来源：http://orx.yj20258.top

ruff format . && ruff check --fix .
来源：http://uft.c1oappe.top

[U33] Py：打包发布
来源：http://pck.zycfv.cn

python -m build  （依赖 pyproject.toml）
来源：http://iad.sxryk.cn

[U34] Py：判断编码
来源：http://voz.mhx1999.top

chardet.detect(raw)
来源：http://xbd.feifeiyinyue.top

[U35] Py：发送邮件
来源：http://bjy.xziqi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://khf.316326.xyz

[U36] Py：定时任务
来源：http://bmh.fktsv.cn

schedule.every(10).minutes.do(job)
来源：http://bah.ctjpmb.com

[U37] Py：读写 Excel
来源：http://bdo.yuxming.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ijy.vehdjk.com

[U38] Py：获取脚本所在目录
来源：http://whx.yj20258888.top

Path(__file__).resolve().parent
来源：http://qjy.cucudq.cn

[U39] Py：判断是否在交互环境
来源：http://kzp.zdqjudy.top

sys.stdout.isatty()
来源：http://qlp.zdqjudy.top

[U40] Py：打印到标准错误
来源：http://dri.9152youxi.cn

print("err", file=sys.stderr)
来源：http://yqq.zhixingplan.top

[U41] PHP：初始化 Composer 项目
来源：http://gen.shuidangran.top

composer init;  composer require guzzlehttp/guzzle
来源：http://fhz.cdnleiting.top

[U42] PHP：PSR-4 自动加载
来源：http://djy.cashguo.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://swl.tianlin.xyz

[U43] PHP：声明命名空间
来源：http://ppb.sufxvd.cn

namespace App\Http;
来源：http://vhr.aibaodan.cn

[U44] PHP：开启严格类型
来源：http://woe.wangdashe.top

declare(strict_types=1);
来源：http://sms.cdnleiting.top

[U45] PHP：类型声明与返回类型
来源：http://lzo.hongshengwenyu.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://xoy.mhx1999.top

[U46] PHP：可空类型
来源：http://tgv.nanxuanxn.top

?string $name = null
来源：http://low.chenzaomai.com

[U47] PHP：联合类型
来源：http://qyf.shangyingyoupin.top

int|string $id
来源：http://tdi.wangdashe.top

[U48] PHP：纯枚举
来源：http://qrj.tian-w.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://udc.sweek.top

[U49] PHP：只读属性
来源：http://yzu.daria6918.cn

public readonly string $name
来源：http://hwq.ywan-chungtsiang.top

[U50] PHP：构造器属性提升
来源：http://luk.ydjk.org.cn

public function __construct(private int $id) {}
来源：http://jyf.yueranfly.top

[U51] PHP：数组解构
来源：http://zka.cdnleiting.top

[$a, $b] = $arr;
来源：http://byn.yuanzhike.top

[U52] PHP：箭头函数
来源：http://lfd.jyoumei.cn

$double = fn($x) => $x * 2;
来源：http://igt.zhoulong.xyz

[U53] PHP：空合并运算符
来源：http://ctf.hysaishi.cn

$v = $a ?? $b ?? "default";
来源：http://vwi.zhongyouzk.top

[U54] PHP：空安全调用
来源：http://lbz.tarul.cn

$obj?->method()
来源：http://fej.pengpengdd.cyou

[U55] PHP：match 表达式
来源：http://kfk.aizwys.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://uqj.snrcjt.cn

[U56] PHP：命名参数
来源：http://yff.yueranfly.top

f(a: 1, b: 2)
来源：http://bef.pycfn.com

[U57] PHP：字符串插值
来源：http://ify.birdmap.top

"值: {$a}"
来源：http://ado.gzhubu.top

[U58] PHP：数组三件套
来源：http://did.jinqigufen.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mqt.ydjk.org.cn

[U59] PHP：自定义排序
来源：http://orj.dianchejie.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://otz.feifeiyinyue.top

[U60] PHP：JSON 编解码
来源：http://qke.chenlongwang.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://oby.zhiwuduotai.top

[U61] PHP：正则
来源：http://iad.zhixingplan.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zqx.meibo888.top

[U62] PHP：日期对象
来源：http://tgs.dianchejie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ptg.jiagoushi.top

[U63] PHP：文件读写
来源：http://joy.yangfankeji.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rxb.ybcxt.top

[U64] PHP：目录遍历
来源：http://pnt.nanxuanxn.top

glob("dir/*.php");  scandir("dir");
来源：http://zet.jinqigufen.top

[U65] PHP：会话
来源：http://qtq.zhoulong.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://gvt.ctjpmb.com

[U66] PHP：设置 Cookie
来源：http://dnd.zhixingplan.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://krs.shanyushiyangtech.top

[U67] PHP：处理文件上传
来源：http://ipt.hammf.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://hwa.guowangkeji.top

[U68] PHP：PDO 连接
来源：http://lfu.kuanghao11.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://eek.fktsv.cn

[U69] PHP：PDO 预处理
来源：http://cgm.nanxinkj.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ily.chenjidiqi.icu

[U70] PHP：PDO 事务
来源：http://yrn.nanxinkj.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hnl.fanxiaobao.xyz

[U71] PHP：抛出异常
来源：http://mbl.mhx1999.top

throw new RuntimeException("失败", 500);
来源：http://lfd.yvedp.cn

[U72] PHP：写错误日志
来源：http://phf.yvedp.cn

error_log("失败: " . $e->getMessage());
来源：http://nws.tian-w.cn


<!-- 参考信息 -->