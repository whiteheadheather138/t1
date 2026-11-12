代发 wailian999

[S45] C++：lambda
来源：http://hmy.yanxiufei.cn

auto add = [](int a, int b) { return a + b; };
来源：http://khh.nwbrower.top

[S46] C++：函数模板
来源：http://ofq.sysykeji.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gmi.snrcjt.cn

[S47] C++：结构化绑定遍历
来源：http://sbf.ppjwa.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://uga.yueranfly.top

[S48] C++：逐行读文件
来源：http://ssd.nwbrower.top

std::ifstream in("a.txt");  std::string line;
来源：http://fyk.xinyue.icu

while (std::getline(in, line)) { }
来源：http://cid.cucudq.cn

[S49] C++：写文件
来源：http://ckq.ivvv.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fkp.hammf.cn

[S50] C++：格式化数字
来源：http://qzx.c1oappe.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ppd.jianghu66.top

[S51] C++：显式类型转换
来源：http://lpd.jianghu66.top

static_cast<double>(a) / b
来源：http://nig.vqdsnc.cn

[S52] C++：const 与 noexcept
来源：http://fyo.yanxiufei.cn

int size() const noexcept { return n_; }
来源：http://hlt.fanxiaobao.xyz

[S53] C++：移动语义
来源：http://jla.zhengqikj.top

std::vector<int> w = std::move(v);
来源：http://sbx.birdmap.top

[S54] C++：异常处理
来源：http://nji.epnwcf.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cia.wangshuangyany.cn

[S55] C++：结构化绑定
来源：http://ksj.jinyuanbaomall.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://pnk.cheryme.top

[S56] C++：optional
来源：http://aky.daria6918.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://szn.yfazqb.com

[S57] C++：编译期常量
来源：http://hmd.svipenyu.cn

constexpr int N = 10;
来源：http://cwf.hcnkem.com

[S58] C++：命名空间
来源：http://xtx.sufxvd.cn

namespace ns { int f() { return 1; } }
来源：http://maz.gogol.net.cn

[S59] C++：静态断言
来源：http://hyk.316326.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qru.shangyingyoupin.top

[S60] C++：遍历并删除元素
来源：http://qzm.fanxiaobao.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cpr.xingfuxueyuan.xyz

================================================================================
来源：http://auw.shzxlz.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qex.ydzc1.top

================================================================================
来源：http://krx.jinqigfzy.top

[T01] Kotlin：Hello World
来源：http://arc.xingfuxueyuan.xyz

println("Hello")
来源：http://oqy.vehdjk.com

[T02] Kotlin：变量
来源：http://rtu.hywenlv.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dij.kuanghao11.cn

[T03] Kotlin：字符串模板
来源：http://mwh.ppjwa.cn

"值: $b"
来源：http://eof.hnxiangtu.top

[T04] Kotlin：空安全
来源：http://dbm.nanxuanxn.top

val n: String? = null;  n?.length
来源：http://zjn.yj202588.top

[T05] Kotlin：when 表达式
来源：http://cel.yfazqb.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xim.sysykeji.top

[T06] Kotlin：集合映射
来源：http://yti.cucudq.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://iic.yangfankeji.com

[T07] Kotlin：集合过滤
来源：http://ecd.yvedp.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://zly.zhoulong.xyz

[T08] Kotlin：数据类
来源：http://xdb.wangshuangyany.cn

data class User(val name: String, val age: Int)
来源：http://pnq.jlsjyb.cn

[T09] Kotlin：扩展函数
来源：http://xkv.nwbrower.top

fun String.exclaim() = this + "!"
来源：http://uib.daxiang520.top

[T10] Kotlin：默认参数
来源：http://nrv.zhijiandao.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://beh.kuanghao11.cn

[T11] Kotlin：协程
来源：http://oad.yonumen.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://hgi.yfazqb.com

[T12] Kotlin：解构声明
来源：http://yom.xuanzx.com

val (a, b) = Pair(1, 2)
来源：http://uxz.sweek.top

[T13] Kotlin：只读 Map
来源：http://mnp.yanxiufei.cn

val m = mapOf("a" to 1)
来源：http://jds.fanxiaobao.xyz

[T14] Kotlin：循环
来源：http://vgl.zdqjudy.top

for (i in 1..10) println(i)
来源：http://xki.fengsongda.top

[T15] Kotlin：接口
来源：http://asj.yangfankeji.com

interface Shape { fun area(): Double }
来源：http://fbm.bjfxy.top

[T16] Swift：Hello World
来源：http://pbx.birdmap.top

print("Hello")
来源：http://vqx.wangdashe.top

[T17] Swift：变量与常量
来源：http://qcj.cashguo.top

var a = 1;  let b = 2
来源：http://fpp.zdbjq.cn

[T18] Swift：字符串插值
来源：http://fuu.hcnkem.com

"值: \(b)"
来源：http://pgr.andypj.xyz

[T19] Swift：可选绑定
来源：http://nla.zhijiandao.cn

if let n = opt { print(n) }
来源：http://kkz.ybcxt.top

[T20] Swift：数组操作
来源：http://way.dashuyun.cn

var a = [1, 2, 3];  a.append(4)
来源：http://dch.dianchejie.cn

[T21] Swift：遍历
来源：http://doq.tian-w.cn

for x in a { print(x) }
来源：http://qtp.fengsongda.top

[T22] Swift：字典
来源：http://dvm.tian-w.cn

var d = ["a": 1];  d["b"] = 2
来源：http://iwn.tianlin.xyz

[T23] Swift：函数
来源：http://tdl.bjfxy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://reu.pycfn.com

[T24] Swift：闭包
来源：http://hpr.ydjk.org.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ati.daria6918.cn

[T25] Swift：结构体
来源：http://suj.hcnkem.com

struct P { var x: Int }
来源：http://gmv.yuanzhike.top

[T26] Swift：类与重写
来源：http://qxq.chenzaomai.com

class A: Base { override func f() {} }
来源：http://uru.ybcxt.top

[T27] Swift：错误处理
来源：http://hgd.aibaodan.cn

do { try f() } catch { print(error) }
来源：http://czc.c1oappe.top

[T28] Swift：枚举
来源：http://ttj.0kj1m.cn

enum Color { case red, green }
来源：http://itc.daxiang520.top

[T29] Swift：guard 提前返回
来源：http://oja.guowangkeji.top

guard let x = opt else { return }
来源：http://xmq.shuidangran.top

[T30] Swift：协议
来源：http://vhj.jyoumei.cn

protocol Shape { func area() -> Double }
来源：http://zzb.smart0.xyz

[T31] Lua：Hello World
来源：http://qev.wangdashe.top

print("Hello")
来源：http://ngx.yj202588.top

[T32] Lua：局部变量
来源：http://yxx.shanyushiyangkeji.top

local a = 1
来源：http://srn.zhoulong.xyz

[T33] Lua：表（数组）
来源：http://xxr.zhongyouzk.top

local t = {1, 2, 3};  t[4] = 4
来源：http://oun.ybcxt.top

[T34] Lua：遍历表
来源：http://jqs.zhongyouzk.top

for i, v in ipairs(t) do print(i, v) end
来源：http://mvw.cucudq.cn

[T35] Lua：字典表
来源：http://dyr.yj202588.top

local d = { a = 1 };  d.b = 2
来源：http://uil.sxryk.cn

[T36] Lua：函数
来源：http://tta.shanyushiyangtech.top

function add(a, b) return a + b end
来源：http://adr.fzhhl.top

[T37] Lua：字符串拼接
来源：http://syw.zhongyouzk.top

"a" .. "b"
来源：http://gzo.ehwqpu.com

[T38] Lua：条件
来源：http://god.zdqjudy.top

if x > 0 then print("正") end
来源：http://htc.nanxuanxn.top

[T39] Lua：模式匹配
来源：http://zze.jqgfzy.top

string.find(s, "%d+")
来源：http://mxk.yongpay.top

[T40] Lua：元表
来源：http://xra.yj20258888.top

setmetatable({}, { __index = base })
来源：http://kfw.316326.xyz

[T41] Perl：Hello World
来源：http://uql.yanxiufei.cn

print "Hello\n";
来源：http://czg.shuidangran.top

[T42] Perl：变量类型
来源：http://gas.pycfn.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fyq.dashuyun.cn

[T43] Perl：字符串插值
来源：http://zqf.shanyushiyangtech.top

"值: $a"
来源：http://psa.hfpthk.cn

[T44] Perl：条件
来源：http://rvr.fanxiaobao.xyz

if ($a > 0) { print "正"; }
来源：http://npl.yonumen.top

[T45] Perl：数组遍历
来源：http://ugh.yfazqb.com

for my $x (@arr) { print $x; }
来源：http://dzu.cqqwz.cn

[T46] Perl：哈希操作
来源：http://idc.zhijiandao.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qvv.yueranfly.top

[T47] Perl：正则捕获
来源：http://evs.yonumen.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://rpn.ybcxt.top

[T48] Perl：正则替换
来源：http://yjt.jlsjyb.cn

$s =~ s/old/new/g;
来源：http://iga.xuetiantiany.cn

[T49] Perl：函数
来源：http://hel.cqqwz.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ing.yueranfly.top

[T50] Perl：逐行读文件
来源：http://but.tanke756.top

open my $fh, "<", "a.txt" or die $!;
来源：http://kns.tarul.cn

while (my $line = <$fh>) { print $line; }
来源：http://zfa.c1oappe.top

[T51] Scala：Hello World
来源：http://iph.zhongyouzk.top

println("Hello")
来源：http://xly.ivvv.top

[T52] Scala：变量
来源：http://jwl.yj20258.top

val a = 1;  var b = 2
来源：http://dri.dashuyun.cn

[T53] Scala：字符串插值
来源：http://ylu.ppjwa.cn

s"值: $b"
来源：http://uaq.hysaishi.cn

[T54] Scala：集合映射
来源：http://obr.pengpengdd.cyou

List(1, 2, 3).map(_ * 2)
来源：http://cdz.jiagoushi.top

[T55] Scala：集合过滤
来源：http://ywg.yuxming.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qoq.bjfxy.top

[T56] Scala：样例类
来源：http://dxg.aizwys.cn

case class User(name: String, age: Int)
来源：http://gab.fanxiaobao.xyz

[T57] Scala：模式匹配
来源：http://ptb.zycfv.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://bwa.tian-w.cn

[T58] Scala：函数定义
来源：http://hxg.yonumen.top

def add(a: Int, b: Int): Int = a + b
来源：http://blp.xuanzx.com

[T59] Scala：循环
来源：http://lzy.hfpthk.cn

for (i <- 1 to 10) println(i)
来源：http://wjy.hnqzz.top

[T60] Scala：折叠
来源：http://fyd.yuanzhike.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kbe.316326.xyz

================================================================================
来源：http://tyb.mhx1999.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cxb.fehbvm.com

================================================================================
来源：http://igk.redwolf501.top

[U01] Py：创建虚拟环境
来源：http://buh.cucudq.cn

python -m venv .venv && source .venv/bin/activate
来源：http://fmv.52xcode.cn

[U02] Py：导出 / 安装依赖
来源：http://bts.kuanghao11.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://soa.dianchejie.cn

[U03] Py：加载 .env 配置
来源：http://gzh.chenjidiqi.icu

from dotenv import load_dotenv; load_dotenv()
来源：http://vcf.andypj.xyz

[U04] Py：变量调试打印
来源：http://mwi.ybcxt.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ajx.ctjpmb.com

[U05] Py：列表去重且保序
来源：http://ieg.iojbl.cn

list(dict.fromkeys(arr))
来源：http://dlh.shzxlz.cn

[U06] Py：合并两个字典
来源：http://ajx.cucudq.cn

{**a, **b}
来源：http://pan.iojbl.cn

[U07] Py：反转字典键值
来源：http://ami.chenlongwang.top

{v: k for k, v in d.items()}
来源：http://axr.kuanghao11.cn

[U08] Py：展平二维列表
来源：http://fyb.yfazqb.com

[y for x in nested for y in x]
来源：http://bln.wangshuangyany.cn

[U09] Py：字典取最大值的键
来源：http://ytj.cqqwz.cn

max(d, key=d.get)
来源：http://kpm.wangdashe.top

[U10] Py：按值排序字典
来源：http://vac.zhongyouzk.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zwq.jinyuanbaomall.cn

[U11] Py：生成器表达式
来源：http://evt.havefunace.top

(x * 2 for x in arr)
来源：http://hgz.shanyushiyangtech.top

[U12] Py：取出现最多的 3 个元素
来源：http://kfa.meibo888.top

Counter(arr).most_common(3)
来源：http://reu.dashuyun.cn

[U13] Py：固定长度队列
来源：http://agi.zycfv.cn

deque(maxlen=10)
来源：http://geo.yangfankeji.com

[U14] Py：分组收集到列表
来源：http://fow.birdmap.top

defaultdict(list)
来源：http://fkq.epnwcf.com

[U15] Py：高精度计时
来源：http://fct.cashguo.top

t = time.perf_counter()
来源：http://bqe.svipenyu.cn

[U16] Py：命令行参数解析
来源：http://ywa.guannengcc.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yqp.hcnkem.com

[U17] Py：初始化日志
来源：http://vku.mhx1999.top

logging.basicConfig(level=logging.INFO)
来源：http://ieg.zhixingplan.top

[U18] Py：预编译正则
来源：http://pso.ydjk.org.cn

pat = re.compile(r"\d+")
来源：http://cxy.daria6918.cn

[U19] Py：正则替换带回调
来源：http://xum.zhengqikj.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://etj.yj202588.top

[U20] Py：缓存函数结果
来源：http://mtj.ybcxt.top

@functools.lru_cache(maxsize=None)
来源：http://ekb.yj20258.top

[U21] Py：自定义上下文管理器
来源：http://pxf.hywenlv.cn

@contextlib.contextmanager
来源：http://zor.tianlin.xyz

[U22] Py：矩阵转置
来源：http://png.yanxiufei.cn

list(zip(*m))
来源：http://ejz.hnqzz.top

[U23] Py：分块读取大文件
来源：http://tgs.fzhhl.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tnn.jinyuanbaomall.cn

[U24] Py：路径操作
来源：http://tbn.chenlongwang.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ssn.yj20258.top

[U25] Py：CSV 按字典读
来源：http://teb.snrcjt.cn

csv.DictReader(f)
来源：http://jtb.hnqzz.top

[U26] Py：并发下载
来源：http://fee.havefunace.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://drp.xuanzx.com

[U27] Py：异步 HTTP
来源：http://ukl.xingfuxueyuan.xyz

aiohttp.ClientSession() 配合 async with
来源：http://zno.9152youxi.cn

[U28] Py：类型别名
来源：http://lrg.hnxiangtu.top

UserId = int
来源：http://tzh.ydzc1.top

[U29] Py：属性校验
来源：http://vla.kuanghao11.cn

@property 与 @x.setter 配合
来源：http://mxv.bjfxy.top

[U30] Py：数据类
来源：http://ohn.ivvv.top

@dataclass(slots=True)
来源：http://zkc.bbcook.cn

[U31] Py：单测
来源：http://yjw.xziqi.cn

python -m pytest -q
来源：http://kcr.zhengqikj.top

[U32] Py：代码格式化
来源：http://tme.gaohongyu789.top

ruff format . && ruff check --fix .
来源：http://afk.sweek.top

[U33] Py：打包发布
来源：http://eav.xziqi.cn

python -m build  （依赖 pyproject.toml）
来源：http://ust.vehdjk.com

[U34] Py：判断编码
来源：http://psd.gzhubu.top

chardet.detect(raw)
来源：http://lhx.cdnleiting.top

[U35] Py：发送邮件
来源：http://qge.zhongyouzk.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xez.ydjk.org.cn

[U36] Py：定时任务
来源：http://rde.jinghuilouyu.cn

schedule.every(10).minutes.do(job)
来源：http://rsv.fktsv.cn

[U37] Py：读写 Excel
来源：http://tne.ydjk.org.cn

pandas.read_excel / DataFrame.to_excel
来源：http://wzt.yongpay.top

[U38] Py：获取脚本所在目录
来源：http://nsn.yongpay.top

Path(__file__).resolve().parent
来源：http://qzr.jinqigfzy.top

[U39] Py：判断是否在交互环境
来源：http://ryi.fktsv.cn

sys.stdout.isatty()
来源：http://vcc.jyoumei.cn

[U40] Py：打印到标准错误
来源：http://xpy.ehwqpu.com

print("err", file=sys.stderr)
来源：http://zna.tanke756.top

[U41] PHP：初始化 Composer 项目
来源：http://vqy.cucudq.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://nry.jinghuilouyu.cn

[U42] PHP：PSR-4 自动加载
来源：http://akp.zhoulong.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cgl.uphjek.com

[U43] PHP：声明命名空间
来源：http://mij.cashguo.top

namespace App\Http;
来源：http://nae.xziqi.cn

[U44] PHP：开启严格类型
来源：http://txe.nanxinkj.top

declare(strict_types=1);
来源：http://jxe.yanxiufei.cn

[U45] PHP：类型声明与返回类型
来源：http://awn.daria6918.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://cpz.daxiang520.top

[U46] PHP：可空类型
来源：http://ebx.sysykeji.top

?string $name = null
来源：http://avz.yongpay.top

[U47] PHP：联合类型
来源：http://vub.cqqwz.cn

int|string $id
来源：http://klh.jyoumei.cn

[U48] PHP：纯枚举
来源：http://msc.hfpthk.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xru.fehbvm.com

[U49] PHP：只读属性
来源：http://phi.zhiwuduotai.top

public readonly string $name
来源：http://bbb.vqdsnc.cn

[U50] PHP：构造器属性提升
来源：http://jrt.bbcook.cn

public function __construct(private int $id) {}
来源：http://uor.ehwqpu.com

[U51] PHP：数组解构
来源：http://xnm.gotoacloud.top

[$a, $b] = $arr;
来源：http://qwx.bbcook.cn

[U52] PHP：箭头函数
来源：http://axc.ppjwa.cn

$double = fn($x) => $x * 2;
来源：http://hqa.yj20258.top

[U53] PHP：空合并运算符
来源：http://kyc.jqgfzy.top

$v = $a ?? $b ?? "default";
来源：http://gma.cheryme.top

[U54] PHP：空安全调用
来源：http://oda.fktsv.cn

$obj?->method()
来源：http://rmq.daxiang520.top

[U55] PHP：match 表达式
来源：http://ggx.zhixingplan.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nij.shangyingyoupin.top

[U56] PHP：命名参数
来源：http://wgd.ehwqpu.com

f(a: 1, b: 2)
来源：http://jej.havefunace.top

[U57] PHP：字符串插值
来源：http://yjk.sufxvd.cn

"值: {$a}"
来源：http://awc.hammf.cn

[U58] PHP：数组三件套
来源：http://pbz.kuanghao11.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blb.zhaomingkeji.xyz

[U59] PHP：自定义排序
来源：http://fto.jinghuilouyu.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nsn.9152youxi.cn

[U60] PHP：JSON 编解码
来源：http://iet.dashuyun.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://goj.meibo888.top

[U61] PHP：正则
来源：http://vjb.wangdashe.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://rst.ywan-chungtsiang.top

[U62] PHP：日期对象
来源：http://jhv.smart0.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://uco.iojbl.cn

[U63] PHP：文件读写
来源：http://dcc.sjlbkw.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pea.shuidangran.top

[U64] PHP：目录遍历
来源：http://rmt.hcnkem.com

glob("dir/*.php");  scandir("dir");
来源：http://lsq.guowangkeji.top

[U65] PHP：会话
来源：http://txu.hywenlv.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://jts.jiagoushi.top

[U66] PHP：设置 Cookie
来源：http://mee.fehbvm.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ies.haohaochexian.top

[U67] PHP：处理文件上传
来源：http://eph.pengpengdd.cyou

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qni.vehdjk.com

[U68] PHP：PDO 连接
来源：http://ztl.yvedp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wlj.birdmap.top

[U69] PHP：PDO 预处理
来源：http://ogr.birdmap.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bfn.jlsjyb.cn

[U70] PHP：PDO 事务
来源：http://oyp.ywan-chungtsiang.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mjm.cheryme.top


<!-- 参考信息 -->