代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kys.ehwqpu.com

[S51] C++：显式类型转换
来源：http://pym.zhiwuduotai.top

static_cast<double>(a) / b
来源：http://vlt.cqqwz.cn

[S52] C++：const 与 noexcept
来源：http://kbh.epnwcf.com

int size() const noexcept { return n_; }
来源：http://uki.havefunace.top

[S53] C++：移动语义
来源：http://yjj.shangyingyoupin.top

std::vector<int> w = std::move(v);
来源：http://dqc.tianlin.xyz

[S54] C++：异常处理
来源：http://jlg.uphjek.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rju.ivvv.top

[S55] C++：结构化绑定
来源：http://ojm.chenlongwang.top

auto [a, b] = std::make_pair(1, 2);
来源：http://qxj.uphjek.com

[S56] C++：optional
来源：http://eoe.vqdsnc.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://iin.wangdashe.top

[S57] C++：编译期常量
来源：http://lya.jinqigfzy.top

constexpr int N = 10;
来源：http://aak.ydzc1.top

[S58] C++：命名空间
来源：http://kyg.cashguo.top

namespace ns { int f() { return 1; } }
来源：http://ukp.sysykeji.top

[S59] C++：静态断言
来源：http://kvf.xuetiantiany.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rjh.hysaishi.cn

[S60] C++：遍历并删除元素
来源：http://eog.tarul.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://eic.cdnleiting.top

================================================================================
来源：http://jhx.gzhubu.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qad.aizwys.cn

================================================================================
来源：http://xon.fzhhl.top

[T01] Kotlin：Hello World
来源：http://eab.birdmap.top

println("Hello")
来源：http://kqt.jinqigufen.top

[T02] Kotlin：变量
来源：http://pox.0kj1m.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qsw.xuanzx.com

[T03] Kotlin：字符串模板
来源：http://zrj.chenzaomai.com

"值: $b"
来源：http://vah.52xcode.cn

[T04] Kotlin：空安全
来源：http://gbc.haohaochexian.top

val n: String? = null;  n?.length
来源：http://fsp.ywan-chungtsiang.top

[T05] Kotlin：when 表达式
来源：http://kwh.hnxiangtu.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nrg.zdbjq.cn

[T06] Kotlin：集合映射
来源：http://jsu.hnqzz.top

listOf(1, 2, 3).map { it * 2 }
来源：http://jgm.yj202588.top

[T07] Kotlin：集合过滤
来源：http://sup.bjfxy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://gxb.jqgfzy.top

[T08] Kotlin：数据类
来源：http://dsa.dianchejie.cn

data class User(val name: String, val age: Int)
来源：http://ose.sysykeji.top

[T09] Kotlin：扩展函数
来源：http://lau.zhoulong.xyz

fun String.exclaim() = this + "!"
来源：http://rzz.feifeiyinyue.top

[T10] Kotlin：默认参数
来源：http://fco.zycfv.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://bes.wangshuangyany.cn

[T11] Kotlin：协程
来源：http://toi.shzxlz.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://sih.svipenyu.cn

[T12] Kotlin：解构声明
来源：http://qkn.birdmap.top

val (a, b) = Pair(1, 2)
来源：http://mao.andypj.xyz

[T13] Kotlin：只读 Map
来源：http://rdw.zdbjq.cn

val m = mapOf("a" to 1)
来源：http://rki.ydzc1.top

[T14] Kotlin：循环
来源：http://mcv.aibaodan.cn

for (i in 1..10) println(i)
来源：http://thu.zdbjq.cn

[T15] Kotlin：接口
来源：http://lme.yueranfly.top

interface Shape { fun area(): Double }
来源：http://dvp.316326.xyz

[T16] Swift：Hello World
来源：http://syf.yongpay.top

print("Hello")
来源：http://qyc.hesvh.cn

[T17] Swift：变量与常量
来源：http://qfa.ehwqpu.com

var a = 1;  let b = 2
来源：http://jns.fzhhl.top

[T18] Swift：字符串插值
来源：http://jgc.iojbl.cn

"值: \(b)"
来源：http://gst.yangfankeji.com

[T19] Swift：可选绑定
来源：http://hsf.fzhhl.top

if let n = opt { print(n) }
来源：http://dfo.jianghu66.top

[T20] Swift：数组操作
来源：http://tml.jinyuanbaomall.cn

var a = [1, 2, 3];  a.append(4)
来源：http://nfk.zhaomingkeji.xyz

[T21] Swift：遍历
来源：http://ndt.aibaodan.cn

for x in a { print(x) }
来源：http://dex.epnwcf.com

[T22] Swift：字典
来源：http://ekg.shzxlz.cn

var d = ["a": 1];  d["b"] = 2
来源：http://pvl.shanyushiyangtech.top

[T23] Swift：函数
来源：http://vmu.yanxiufei.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vhr.shzxlz.cn

[T24] Swift：闭包
来源：http://llw.nanxuanxn.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://dkz.jinyuanbaomall.cn

[T25] Swift：结构体
来源：http://eky.daxiang520.top

struct P { var x: Int }
来源：http://lyo.meibo888.top

[T26] Swift：类与重写
来源：http://udc.ehwqpu.com

class A: Base { override func f() {} }
来源：http://xtr.nwbrower.top

[T27] Swift：错误处理
来源：http://dhd.ydjk.org.cn

do { try f() } catch { print(error) }
来源：http://cwv.hysaishi.cn

[T28] Swift：枚举
来源：http://ikn.pycfn.com

enum Color { case red, green }
来源：http://sqj.gaohongyu789.top

[T29] Swift：guard 提前返回
来源：http://jij.hnqzz.top

guard let x = opt else { return }
来源：http://qur.feifeiyinyue.top

[T30] Swift：协议
来源：http://qmz.uphjek.com

protocol Shape { func area() -> Double }
来源：http://yrf.jinyuanbaomall.cn

[T31] Lua：Hello World
来源：http://zip.yanxiufei.cn

print("Hello")
来源：http://uxv.hysaishi.cn

[T32] Lua：局部变量
来源：http://yhd.fengsongda.top

local a = 1
来源：http://ijg.dianchejie.cn

[T33] Lua：表（数组）
来源：http://iin.316326.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://awo.hcnkem.com

[T34] Lua：遍历表
来源：http://zui.xuetiantiany.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://nal.ybcxt.top

[T35] Lua：字典表
来源：http://mob.hysaishi.cn

local d = { a = 1 };  d.b = 2
来源：http://fob.hcnkem.com

[T36] Lua：函数
来源：http://kux.dianchejie.cn

function add(a, b) return a + b end
来源：http://qzs.jinqigufen.top

[T37] Lua：字符串拼接
来源：http://tdc.sysykeji.top

"a" .. "b"
来源：http://xre.hnqzz.top

[T38] Lua：条件
来源：http://oxt.gaohongyu789.top

if x > 0 then print("正") end
来源：http://jqy.fktsv.cn

[T39] Lua：模式匹配
来源：http://hvj.dianchejie.cn

string.find(s, "%d+")
来源：http://fnk.jqgfzy.top

[T40] Lua：元表
来源：http://eup.hcnkem.com

setmetatable({}, { __index = base })
来源：http://rvk.jinqigufen.top

[T41] Perl：Hello World
来源：http://cqx.jqgufenzy.top

print "Hello\n";
来源：http://fmr.fzhhl.top

[T42] Perl：变量类型
来源：http://esk.ydzc1.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jqq.nanxinkj.top

[T43] Perl：字符串插值
来源：http://yiz.xinyue.icu

"值: $a"
来源：http://xmz.pycfn.com

[T44] Perl：条件
来源：http://vua.birdmap.top

if ($a > 0) { print "正"; }
来源：http://uiv.vehdjk.com

[T45] Perl：数组遍历
来源：http://unn.redwolf501.top

for my $x (@arr) { print $x; }
来源：http://bxg.nanxuanxn.top

[T46] Perl：哈希操作
来源：http://qir.zhongyouzk.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ood.sxryk.cn

[T47] Perl：正则捕获
来源：http://iov.chenlongwang.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://fqv.yj20258888.top

[T48] Perl：正则替换
来源：http://mpx.vqdsnc.cn

$s =~ s/old/new/g;
来源：http://vqy.yj202588.top

[T49] Perl：函数
来源：http://rqk.ivvv.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://aaz.yj202588.top

[T50] Perl：逐行读文件
来源：http://hyf.yueranfly.top

open my $fh, "<", "a.txt" or die $!;
来源：http://xky.sweek.top

while (my $line = <$fh>) { print $line; }
来源：http://grw.guannengcc.top

[T51] Scala：Hello World
来源：http://olg.cashguo.top

println("Hello")
来源：http://hlc.yongpay.top

[T52] Scala：变量
来源：http://yxn.fehbvm.com

val a = 1;  var b = 2
来源：http://wid.0kj1m.cn

[T53] Scala：字符串插值
来源：http://nsf.yvedp.cn

s"值: $b"
来源：http://mst.yangfankeji.com

[T54] Scala：集合映射
来源：http://ixe.mhx1999.top

List(1, 2, 3).map(_ * 2)
来源：http://xjl.aizwys.cn

[T55] Scala：集合过滤
来源：http://nzx.tianlin.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://xxm.yj20258888.top

[T56] Scala：样例类
来源：http://mdn.guannengcc.top

case class User(name: String, age: Int)
来源：http://pmk.xylfe.cn

[T57] Scala：模式匹配
来源：http://uvi.cashguo.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://sxm.zycfv.cn

[T58] Scala：函数定义
来源：http://qhb.mhx1999.top

def add(a: Int, b: Int): Int = a + b
来源：http://hcg.zhijiandao.cn

[T59] Scala：循环
来源：http://hpk.9152youxi.cn

for (i <- 1 to 10) println(i)
来源：http://flt.smart0.xyz

[T60] Scala：折叠
来源：http://wtd.epnwcf.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ydj.zhixingplan.top

================================================================================
来源：http://ggu.vehdjk.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://esj.iojbl.cn

================================================================================
来源：http://vfn.iojbl.cn

[U01] Py：创建虚拟环境
来源：http://shs.redwolf501.top

python -m venv .venv && source .venv/bin/activate
来源：http://cmv.hfpthk.cn

[U02] Py：导出 / 安装依赖
来源：http://yuw.yueranfly.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vpc.sxryk.cn

[U03] Py：加载 .env 配置
来源：http://vne.fzhhl.top

from dotenv import load_dotenv; load_dotenv()
来源：http://kda.cqqwz.cn

[U04] Py：变量调试打印
来源：http://yii.vehdjk.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nbx.xuetiantiany.cn

[U05] Py：列表去重且保序
来源：http://kky.jinyuanbaomall.cn

list(dict.fromkeys(arr))
来源：http://rvl.shzxlz.cn

[U06] Py：合并两个字典
来源：http://kap.gaohongyu789.top

{**a, **b}
来源：http://xkg.wangshuangyany.cn

[U07] Py：反转字典键值
来源：http://wzn.zhiwuduotai.top

{v: k for k, v in d.items()}
来源：http://lee.yueranfly.top

[U08] Py：展平二维列表
来源：http://bxd.chenlongwang.top

[y for x in nested for y in x]
来源：http://wlq.xinyue.icu

[U09] Py：字典取最大值的键
来源：http://msd.xingfuxueyuan.xyz

max(d, key=d.get)
来源：http://mjg.cdnleiting.top

[U10] Py：按值排序字典
来源：http://acw.fktsv.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://olq.bbcook.cn

[U11] Py：生成器表达式
来源：http://kpe.xingfuxueyuan.xyz

(x * 2 for x in arr)
来源：http://pky.birdmap.top

[U12] Py：取出现最多的 3 个元素
来源：http://kqj.jianghu66.top

Counter(arr).most_common(3)
来源：http://zrd.tian-w.cn

[U13] Py：固定长度队列
来源：http://iht.yueranfly.top

deque(maxlen=10)
来源：http://cko.gogol.net.cn

[U14] Py：分组收集到列表
来源：http://xtd.gzhubu.top

defaultdict(list)
来源：http://enn.gaohongyu789.top

[U15] Py：高精度计时
来源：http://kar.cashguo.top

t = time.perf_counter()
来源：http://mcz.shuidangran.top

[U16] Py：命令行参数解析
来源：http://psh.gaohongyu789.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://roo.gaohongyu789.top

[U17] Py：初始化日志
来源：http://lev.jinyuanbaomall.cn

logging.basicConfig(level=logging.INFO)
来源：http://kcg.pengpengdd.cyou

[U18] Py：预编译正则
来源：http://lyt.tianlin.xyz

pat = re.compile(r"\d+")
来源：http://jnd.xuanzx.com

[U19] Py：正则替换带回调
来源：http://etx.cucudq.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zeq.chenlongwang.top

[U20] Py：缓存函数结果
来源：http://znc.feifeiyinyue.top

@functools.lru_cache(maxsize=None)
来源：http://omo.zhaomingkeji.xyz

[U21] Py：自定义上下文管理器
来源：http://xvo.ivvv.top

@contextlib.contextmanager
来源：http://lpb.cheryme.top

[U22] Py：矩阵转置
来源：http://kht.52xcode.cn

list(zip(*m))
来源：http://tdc.jinqigfzy.top

[U23] Py：分块读取大文件
来源：http://weu.gogol.net.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://thx.pengpengdd.cyou

[U24] Py：路径操作
来源：http://dxa.bjfxy.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gue.hfpthk.cn

[U25] Py：CSV 按字典读
来源：http://wxs.jianghu66.top

csv.DictReader(f)
来源：http://huu.vqdsnc.cn

[U26] Py：并发下载
来源：http://hpt.nanxinkj.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rkv.meibo888.top

[U27] Py：异步 HTTP
来源：http://xqc.yangfankeji.com

aiohttp.ClientSession() 配合 async with
来源：http://pis.zdqjudy.top

[U28] Py：类型别名
来源：http://ynj.gogol.net.cn

UserId = int
来源：http://xyn.ivvv.top

[U29] Py：属性校验
来源：http://vjy.fktsv.cn

@property 与 @x.setter 配合
来源：http://xpu.yanxiufei.cn

[U30] Py：数据类
来源：http://ecx.gotoacloud.top

@dataclass(slots=True)
来源：http://fyu.dianchejie.cn

[U31] Py：单测
来源：http://oxw.smart0.xyz

python -m pytest -q
来源：http://gbg.daxiang520.top

[U32] Py：代码格式化
来源：http://xum.birdmap.top

ruff format . && ruff check --fix .
来源：http://lgm.iojbl.cn

[U33] Py：打包发布
来源：http://vye.daria6918.cn

python -m build  （依赖 pyproject.toml）
来源：http://ytl.yangfankeji.com

[U34] Py：判断编码
来源：http://glq.haohaochexian.top

chardet.detect(raw)
来源：http://jcv.cdnleiting.top

[U35] Py：发送邮件
来源：http://qsb.yvedp.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qcs.yonumen.top

[U36] Py：定时任务
来源：http://ojx.dashuyun.cn

schedule.every(10).minutes.do(job)
来源：http://rok.jlsjyb.cn

[U37] Py：读写 Excel
来源：http://vep.daxiang520.top

pandas.read_excel / DataFrame.to_excel
来源：http://uez.hnqzz.top

[U38] Py：获取脚本所在目录
来源：http://ddn.gotoacloud.top

Path(__file__).resolve().parent
来源：http://rnd.yfazqb.com

[U39] Py：判断是否在交互环境
来源：http://hyk.jianghu66.top

sys.stdout.isatty()
来源：http://ncp.cheryme.top

[U40] Py：打印到标准错误
来源：http://rki.yj20258.top

print("err", file=sys.stderr)
来源：http://tbm.shzxlz.cn

[U41] PHP：初始化 Composer 项目
来源：http://ktr.shanyushiyangkeji.top

composer init;  composer require guzzlehttp/guzzle
来源：http://piz.cqqwz.cn

[U42] PHP：PSR-4 自动加载
来源：http://shg.jianghu66.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://lty.smart0.xyz

[U43] PHP：声明命名空间
来源：http://hun.fzhhl.top

namespace App\Http;
来源：http://ydy.vehdjk.com

[U44] PHP：开启严格类型
来源：http://zng.yj20258888.top

declare(strict_types=1);
来源：http://odt.tian-w.cn

[U45] PHP：类型声明与返回类型
来源：http://yas.chenlongwang.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://sym.nwbrower.top

[U46] PHP：可空类型
来源：http://yvn.sysykeji.top

?string $name = null
来源：http://tlz.havefunace.top

[U47] PHP：联合类型
来源：http://fld.xuanzx.com

int|string $id
来源：http://bax.ctjpmb.com

[U48] PHP：纯枚举
来源：http://uac.yangfankeji.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://smy.uphjek.com

[U49] PHP：只读属性
来源：http://jlq.ybcxt.top

public readonly string $name
来源：http://zyd.zhaomingkeji.xyz

[U50] PHP：构造器属性提升
来源：http://nxq.yj202588.top

public function __construct(private int $id) {}
来源：http://cla.dashuyun.cn

[U51] PHP：数组解构
来源：http://qgv.jinghuilouyu.cn

[$a, $b] = $arr;
来源：http://pyz.hnqzz.top

[U52] PHP：箭头函数
来源：http://lms.yangfankeji.com

$double = fn($x) => $x * 2;
来源：http://tue.hongshengwenyu.top

[U53] PHP：空合并运算符
来源：http://mix.yfazqb.com

$v = $a ?? $b ?? "default";
来源：http://itg.fanxiaobao.xyz

[U54] PHP：空安全调用
来源：http://uqe.jinqigfzy.top

$obj?->method()
来源：http://yxt.0kj1m.cn

[U55] PHP：match 表达式
来源：http://yfj.chenzaomai.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qip.tarul.cn

[U56] PHP：命名参数
来源：http://vlu.yonumen.top

f(a: 1, b: 2)
来源：http://oir.jinqigufen.top

[U57] PHP：字符串插值
来源：http://xhj.hammf.cn

"值: {$a}"
来源：http://xvl.yuanzhike.top

[U58] PHP：数组三件套
来源：http://mkm.xuanzx.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vwn.dianchejie.cn

[U59] PHP：自定义排序
来源：http://knu.hnqzz.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nfo.wangshuangyany.cn

[U60] PHP：JSON 编解码
来源：http://blz.gaohongyu789.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://duu.guowangkeji.top

[U61] PHP：正则
来源：http://kwn.gogol.net.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jlo.jqgufenzy.top

[U62] PHP：日期对象
来源：http://axb.xuanzx.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://usi.shangyingyoupin.top

[U63] PHP：文件读写
来源：http://edd.yuanzhike.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gqh.yongpay.top

[U64] PHP：目录遍历
来源：http://uoj.sxryk.cn

glob("dir/*.php");  scandir("dir");
来源：http://qhi.fengsongda.top

[U65] PHP：会话
来源：http://vmg.sxryk.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rrl.andypj.xyz

[U66] PHP：设置 Cookie
来源：http://vnm.ehwqpu.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ibg.hcnkem.com

[U67] PHP：处理文件上传
来源：http://xgn.gzhubu.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zrt.gaohongyu789.top

[U68] PHP：PDO 连接
来源：http://tun.fktsv.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://apj.cheryme.top

[U69] PHP：PDO 预处理
来源：http://yzw.cqqwz.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://krs.jianghu66.top

[U70] PHP：PDO 事务
来源：http://lxu.ehwqpu.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nnx.tianlin.xyz

[U71] PHP：抛出异常
来源：http://tdi.9152youxi.cn

throw new RuntimeException("失败", 500);
来源：http://uxw.daxiang520.top

[U72] PHP：写错误日志
来源：http://oqx.aibaodan.cn

error_log("失败: " . $e->getMessage());
来源：http://gkl.cqqwz.cn

[U73] PHP：读取 ini 配置
来源：http://tjo.zhoulong.xyz

parse_ini_file("config.ini", true)
来源：http://fcj.hysaishi.cn

[U74] PHP：读取环境变量
来源：http://ggv.fanxiaobao.xyz

getenv("APP_ENV") ?: "production"
来源：http://hrh.havefunace.top

[U75] PHP：依赖注入
来源：http://qok.ybcxt.top

composer require psr/container
来源：http://mut.snrcjt.cn

[U76] PHP：简单路由
来源：http://tqn.tarul.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lvg.jlsjyb.cn


<!-- 参考信息 -->