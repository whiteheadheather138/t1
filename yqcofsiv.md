代发 wailian999

while (std::getline(in, line)) { }
来源：http://ffx.birdmap.top

[S49] C++：写文件
来源：http://edd.c1oappe.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qjx.tarul.cn

[S50] C++：格式化数字
来源：http://pej.gaohongyu789.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dff.vehdjk.com

[S51] C++：显式类型转换
来源：http://epi.redwolf501.top

static_cast<double>(a) / b
来源：http://nts.shangyingyoupin.top

[S52] C++：const 与 noexcept
来源：http://xex.fengsongda.top

int size() const noexcept { return n_; }
来源：http://dfv.iojbl.cn

[S53] C++：移动语义
来源：http://kso.xinyue.icu

std::vector<int> w = std::move(v);
来源：http://oqe.quarkkingdee.top

[S54] C++：异常处理
来源：http://kgo.yangfankeji.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pfz.cheryme.top

[S55] C++：结构化绑定
来源：http://soe.feifeiyinyue.top

auto [a, b] = std::make_pair(1, 2);
来源：http://nje.mhx1999.top

[S56] C++：optional
来源：http://cge.aizwys.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fav.yvedp.cn

[S57] C++：编译期常量
来源：http://zdq.tarul.cn

constexpr int N = 10;
来源：http://sfp.hysaishi.cn

[S58] C++：命名空间
来源：http://saz.ehwqpu.com

namespace ns { int f() { return 1; } }
来源：http://yzm.fehbvm.com

[S59] C++：静态断言
来源：http://ilg.shzxlz.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://glx.daxiang520.top

[S60] C++：遍历并删除元素
来源：http://gdc.havefunace.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fgj.zdbjq.cn

================================================================================
来源：http://sae.tianlin.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bqx.smart0.xyz

================================================================================
来源：http://gbh.wangshuangyany.cn

[T01] Kotlin：Hello World
来源：http://sut.tianlin.xyz

println("Hello")
来源：http://tem.shanyushiyangtech.top

[T02] Kotlin：变量
来源：http://yln.vqdsnc.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ozo.yvedp.cn

[T03] Kotlin：字符串模板
来源：http://wou.shanyushiyangtech.top

"值: $b"
来源：http://bdi.zhengqikj.top

[T04] Kotlin：空安全
来源：http://cor.ybcxt.top

val n: String? = null;  n?.length
来源：http://lye.yuxming.cn

[T05] Kotlin：when 表达式
来源：http://gbp.ivvv.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vma.hnqzz.top

[T06] Kotlin：集合映射
来源：http://rvf.wangshuangyany.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://waj.kuanghao11.cn

[T07] Kotlin：集合过滤
来源：http://dim.shzxlz.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://par.ywan-chungtsiang.top

[T08] Kotlin：数据类
来源：http://pmd.sufxvd.cn

data class User(val name: String, val age: Int)
来源：http://zpo.52xcode.cn

[T09] Kotlin：扩展函数
来源：http://tfd.cucudq.cn

fun String.exclaim() = this + "!"
来源：http://ksw.yangfankeji.com

[T10] Kotlin：默认参数
来源：http://cmb.ydzc1.top

fun greet(name: String = "World") = "Hi $name"
来源：http://jfs.jyoumei.cn

[T11] Kotlin：协程
来源：http://whz.ctjpmb.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://rxv.yfazqb.com

[T12] Kotlin：解构声明
来源：http://nfg.zhengqikj.top

val (a, b) = Pair(1, 2)
来源：http://zbr.pengpengdd.cyou

[T13] Kotlin：只读 Map
来源：http://sdz.zdbjq.cn

val m = mapOf("a" to 1)
来源：http://nzb.xziqi.cn

[T14] Kotlin：循环
来源：http://vpx.epnwcf.com

for (i in 1..10) println(i)
来源：http://mst.tanke756.top

[T15] Kotlin：接口
来源：http://mqy.cheryme.top

interface Shape { fun area(): Double }
来源：http://pqr.yj20258.top

[T16] Swift：Hello World
来源：http://bbv.smart0.xyz

print("Hello")
来源：http://xie.guowangkeji.top

[T17] Swift：变量与常量
来源：http://asl.fehbvm.com

var a = 1;  let b = 2
来源：http://trq.sufxvd.cn

[T18] Swift：字符串插值
来源：http://zvm.nanxuanxn.top

"值: \(b)"
来源：http://yxk.zycfv.cn

[T19] Swift：可选绑定
来源：http://hjr.pycfn.com

if let n = opt { print(n) }
来源：http://uwi.ydjk.org.cn

[T20] Swift：数组操作
来源：http://ytb.hongshengwenyu.top

var a = [1, 2, 3];  a.append(4)
来源：http://wqk.vqdsnc.cn

[T21] Swift：遍历
来源：http://pga.zdbjq.cn

for x in a { print(x) }
来源：http://dus.hammf.cn

[T22] Swift：字典
来源：http://zkq.zhaomingkeji.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://bzk.fanxiaobao.xyz

[T23] Swift：函数
来源：http://ciz.haohaochexian.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zps.aibaodan.cn

[T24] Swift：闭包
来源：http://coy.hcnkem.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://ihn.birdmap.top

[T25] Swift：结构体
来源：http://rrj.cqqwz.cn

struct P { var x: Int }
来源：http://aep.yangfankeji.com

[T26] Swift：类与重写
来源：http://fap.ybcxt.top

class A: Base { override func f() {} }
来源：http://qwe.guannengcc.top

[T27] Swift：错误处理
来源：http://llq.haohaochexian.top

do { try f() } catch { print(error) }
来源：http://vvb.fzhhl.top

[T28] Swift：枚举
来源：http://bat.zhoulong.xyz

enum Color { case red, green }
来源：http://msz.aibaodan.cn

[T29] Swift：guard 提前返回
来源：http://abh.gzhubu.top

guard let x = opt else { return }
来源：http://app.ehwqpu.com

[T30] Swift：协议
来源：http://rly.shanyushiyangkeji.top

protocol Shape { func area() -> Double }
来源：http://wdx.zhongyouzk.top

[T31] Lua：Hello World
来源：http://vmb.pycfn.com

print("Hello")
来源：http://nnd.fanxiaobao.xyz

[T32] Lua：局部变量
来源：http://avc.chenjidiqi.icu

local a = 1
来源：http://iag.daria6918.cn

[T33] Lua：表（数组）
来源：http://xnn.cqqwz.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://kzt.epnwcf.com

[T34] Lua：遍历表
来源：http://dcu.zdqjudy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://cxl.ppjwa.cn

[T35] Lua：字典表
来源：http://bxp.iojbl.cn

local d = { a = 1 };  d.b = 2
来源：http://erz.yvedp.cn

[T36] Lua：函数
来源：http://qha.iojbl.cn

function add(a, b) return a + b end
来源：http://eij.tianlin.xyz

[T37] Lua：字符串拼接
来源：http://agc.svipenyu.cn

"a" .. "b"
来源：http://zkk.zhaomingkeji.xyz

[T38] Lua：条件
来源：http://tot.yongpay.top

if x > 0 then print("正") end
来源：http://yhf.ehwqpu.com

[T39] Lua：模式匹配
来源：http://zva.yj20258.top

string.find(s, "%d+")
来源：http://toy.gotoacloud.top

[T40] Lua：元表
来源：http://hyh.pycfn.com

setmetatable({}, { __index = base })
来源：http://epv.aizwys.cn

[T41] Perl：Hello World
来源：http://jph.zhijiandao.cn

print "Hello\n";
来源：http://cub.yanxiufei.cn

[T42] Perl：变量类型
来源：http://ulk.cqqwz.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://soa.redwolf501.top

[T43] Perl：字符串插值
来源：http://zxm.ehwqpu.com

"值: $a"
来源：http://dos.ctjpmb.com

[T44] Perl：条件
来源：http://wur.hcnkem.com

if ($a > 0) { print "正"; }
来源：http://mti.birdmap.top

[T45] Perl：数组遍历
来源：http://uka.hongshengwenyu.top

for my $x (@arr) { print $x; }
来源：http://qlx.cdnleiting.top

[T46] Perl：哈希操作
来源：http://zhj.yfazqb.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://aec.hesvh.cn

[T47] Perl：正则捕获
来源：http://coz.xingfuxueyuan.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://eze.shangyingyoupin.top

[T48] Perl：正则替换
来源：http://rxb.zhengqikj.top

$s =~ s/old/new/g;
来源：http://oza.meibo888.top

[T49] Perl：函数
来源：http://gds.zhixingplan.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sql.daria6918.cn

[T50] Perl：逐行读文件
来源：http://aqh.zdbjq.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://kkt.ybcxt.top

while (my $line = <$fh>) { print $line; }
来源：http://kdl.fengsongda.top

[T51] Scala：Hello World
来源：http://vzf.daria6918.cn

println("Hello")
来源：http://cfj.havefunace.top

[T52] Scala：变量
来源：http://jeu.sweek.top

val a = 1;  var b = 2
来源：http://pfb.dashuyun.cn

[T53] Scala：字符串插值
来源：http://whz.tianlin.xyz

s"值: $b"
来源：http://fjz.zhixingplan.top

[T54] Scala：集合映射
来源：http://eoq.guannengcc.top

List(1, 2, 3).map(_ * 2)
来源：http://lyq.fzhhl.top

[T55] Scala：集合过滤
来源：http://gzb.gaohongyu789.top

List(1, 2, 3).filter(_ > 1)
来源：http://dgm.yanxiufei.cn

[T56] Scala：样例类
来源：http://jje.zdqjudy.top

case class User(name: String, age: Int)
来源：http://dbf.zhijiandao.cn

[T57] Scala：模式匹配
来源：http://bja.uphjek.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://pux.andypj.xyz

[T58] Scala：函数定义
来源：http://mdw.tanke756.top

def add(a: Int, b: Int): Int = a + b
来源：http://agc.yj202588.top

[T59] Scala：循环
来源：http://qsr.ydzc1.top

for (i <- 1 to 10) println(i)
来源：http://aud.dashuyun.cn

[T60] Scala：折叠
来源：http://wyq.hnxiangtu.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yny.gotoacloud.top

================================================================================
来源：http://jxy.zhixingplan.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ljf.xuanzx.com

================================================================================
来源：http://roe.fehbvm.com

[U01] Py：创建虚拟环境
来源：http://atz.ctjpmb.com

python -m venv .venv && source .venv/bin/activate
来源：http://had.wangdashe.top

[U02] Py：导出 / 安装依赖
来源：http://oyd.havefunace.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fgn.ybcxt.top

[U03] Py：加载 .env 配置
来源：http://jfc.jianghu66.top

from dotenv import load_dotenv; load_dotenv()
来源：http://wmu.feifeiyinyue.top

[U04] Py：变量调试打印
来源：http://nuh.snrcjt.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://llu.fzhhl.top

[U05] Py：列表去重且保序
来源：http://shl.52xcode.cn

list(dict.fromkeys(arr))
来源：http://wey.chenlongwang.top

[U06] Py：合并两个字典
来源：http://rtt.hysaishi.cn

{**a, **b}
来源：http://vqa.jinghuilouyu.cn

[U07] Py：反转字典键值
来源：http://lgf.pengpengdd.cyou

{v: k for k, v in d.items()}
来源：http://wtz.hnqzz.top

[U08] Py：展平二维列表
来源：http://yrx.nanxuanxn.top

[y for x in nested for y in x]
来源：http://xou.vqdsnc.cn

[U09] Py：字典取最大值的键
来源：http://frb.smart0.xyz

max(d, key=d.get)
来源：http://oes.xuanzx.com

[U10] Py：按值排序字典
来源：http://vjl.xinyue.icu

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ozj.vqdsnc.cn

[U11] Py：生成器表达式
来源：http://eft.tian-w.cn

(x * 2 for x in arr)
来源：http://mao.shzxlz.cn

[U12] Py：取出现最多的 3 个元素
来源：http://soi.nwbrower.top

Counter(arr).most_common(3)
来源：http://lim.hysaishi.cn

[U13] Py：固定长度队列
来源：http://yqh.jqgfzy.top

deque(maxlen=10)
来源：http://xvl.havefunace.top

[U14] Py：分组收集到列表
来源：http://xkj.shzxlz.cn

defaultdict(list)
来源：http://ouu.yueranfly.top

[U15] Py：高精度计时
来源：http://vjl.kuanghao11.cn

t = time.perf_counter()
来源：http://rig.zhongyouzk.top

[U16] Py：命令行参数解析
来源：http://zpo.jinqigfzy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sgi.nwbrower.top

[U17] Py：初始化日志
来源：http://dkw.cheryme.top

logging.basicConfig(level=logging.INFO)
来源：http://yrm.chenzaomai.com

[U18] Py：预编译正则
来源：http://blm.snrcjt.cn

pat = re.compile(r"\d+")
来源：http://qly.jqgufenzy.top

[U19] Py：正则替换带回调
来源：http://gxb.jqgufenzy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yoo.dianchejie.cn

[U20] Py：缓存函数结果
来源：http://jer.zhiwuduotai.top

@functools.lru_cache(maxsize=None)
来源：http://xgw.fengsongda.top

[U21] Py：自定义上下文管理器
来源：http://dvf.svipenyu.cn

@contextlib.contextmanager
来源：http://xoc.hnxiangtu.top

[U22] Py：矩阵转置
来源：http://zjo.yanxiufei.cn

list(zip(*m))
来源：http://sby.hfpthk.cn

[U23] Py：分块读取大文件
来源：http://xla.jiagoushi.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wmu.c1oappe.top

[U24] Py：路径操作
来源：http://jem.sysykeji.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zmk.ivvv.top

[U25] Py：CSV 按字典读
来源：http://ntz.yanxiufei.cn

csv.DictReader(f)
来源：http://jet.yanxiufei.cn

[U26] Py：并发下载
来源：http://ocz.yongpay.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://oqh.chenjidiqi.icu

[U27] Py：异步 HTTP
来源：http://anb.yongpay.top

aiohttp.ClientSession() 配合 async with
来源：http://ksh.snrcjt.cn

[U28] Py：类型别名
来源：http://yuh.hywenlv.cn

UserId = int
来源：http://wzh.shuidangran.top

[U29] Py：属性校验
来源：http://mad.ctjpmb.com

@property 与 @x.setter 配合
来源：http://eyv.wangshuangyany.cn

[U30] Py：数据类
来源：http://lrz.tanke756.top

@dataclass(slots=True)
来源：http://qwn.fzhhl.top

[U31] Py：单测
来源：http://mih.pycfn.com

python -m pytest -q
来源：http://whu.hongshengwenyu.top

[U32] Py：代码格式化
来源：http://fxr.0kj1m.cn

ruff format . && ruff check --fix .
来源：http://nla.sufxvd.cn

[U33] Py：打包发布
来源：http://egt.xziqi.cn

python -m build  （依赖 pyproject.toml）
来源：http://yae.guannengcc.top

[U34] Py：判断编码
来源：http://tqt.shangyingyoupin.top

chardet.detect(raw)
来源：http://sca.jinqigufen.top

[U35] Py：发送邮件
来源：http://hgi.havefunace.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://grw.dashuyun.cn

[U36] Py：定时任务
来源：http://bkd.zhengqikj.top

schedule.every(10).minutes.do(job)
来源：http://avl.svipenyu.cn

[U37] Py：读写 Excel
来源：http://apw.kuanghao11.cn

pandas.read_excel / DataFrame.to_excel
来源：http://gjo.jqgufenzy.top

[U38] Py：获取脚本所在目录
来源：http://nxp.shangyingyoupin.top

Path(__file__).resolve().parent
来源：http://jki.yongpay.top

[U39] Py：判断是否在交互环境
来源：http://vwl.pengpengdd.cyou

sys.stdout.isatty()
来源：http://wnq.zhengqikj.top

[U40] Py：打印到标准错误
来源：http://pue.tanke756.top

print("err", file=sys.stderr)
来源：http://wnj.redwolf501.top

[U41] PHP：初始化 Composer 项目
来源：http://udn.cheryme.top

composer init;  composer require guzzlehttp/guzzle
来源：http://jcv.zhaomingkeji.xyz

[U42] PHP：PSR-4 自动加载
来源：http://och.yj202588.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tsa.jinqigfzy.top

[U43] PHP：声明命名空间
来源：http://zjh.pycfn.com

namespace App\Http;
来源：http://qzf.cheryme.top

[U44] PHP：开启严格类型
来源：http://vkq.gzhubu.top

declare(strict_types=1);
来源：http://skj.shanyushiyangkeji.top

[U45] PHP：类型声明与返回类型
来源：http://zcg.hnqzz.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ozd.jqgfzy.top

[U46] PHP：可空类型
来源：http://zbf.chenlongwang.top

?string $name = null
来源：http://uqc.jyoumei.cn

[U47] PHP：联合类型
来源：http://yku.hnqzz.top

int|string $id
来源：http://dwx.sjlbkw.cn

[U48] PHP：纯枚举
来源：http://wtx.tanke756.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://klv.xuetiantiany.cn

[U49] PHP：只读属性
来源：http://fko.epnwcf.com

public readonly string $name
来源：http://wtx.hywenlv.cn

[U50] PHP：构造器属性提升
来源：http://onm.birdmap.top

public function __construct(private int $id) {}
来源：http://ros.svipenyu.cn

[U51] PHP：数组解构
来源：http://zus.pengpengdd.cyou

[$a, $b] = $arr;
来源：http://erm.316326.xyz

[U52] PHP：箭头函数
来源：http://qmb.hfpthk.cn

$double = fn($x) => $x * 2;
来源：http://uem.zdqjudy.top

[U53] PHP：空合并运算符
来源：http://jxd.yj20258.top

$v = $a ?? $b ?? "default";
来源：http://jwx.chenjidiqi.icu

[U54] PHP：空安全调用
来源：http://pgm.chenlongwang.top

$obj?->method()
来源：http://yct.ctjpmb.com

[U55] PHP：match 表达式
来源：http://kwb.xingfuxueyuan.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dcy.cucudq.cn

[U56] PHP：命名参数
来源：http://gdx.ydzc1.top

f(a: 1, b: 2)
来源：http://hxn.pycfn.com

[U57] PHP：字符串插值
来源：http://vao.yonumen.top

"值: {$a}"
来源：http://fwq.cdnleiting.top

[U58] PHP：数组三件套
来源：http://wsp.bjfxy.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://sss.uphjek.com

[U59] PHP：自定义排序
来源：http://cdv.aibaodan.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://afh.shanyushiyangkeji.top

[U60] PHP：JSON 编解码
来源：http://uvd.zhaomingkeji.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://uzz.ppjwa.cn

[U61] PHP：正则
来源：http://wva.uphjek.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ivk.yuxming.cn

[U62] PHP：日期对象
来源：http://wjh.shangyingyoupin.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://uke.sjlbkw.cn

[U63] PHP：文件读写
来源：http://uum.gzhubu.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://woy.9152youxi.cn

[U64] PHP：目录遍历
来源：http://nux.ydzc1.top

glob("dir/*.php");  scandir("dir");
来源：http://ahk.feifeiyinyue.top

[U65] PHP：会话
来源：http://ism.tian-w.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rxj.hnqzz.top

[U66] PHP：设置 Cookie
来源：http://izn.quarkkingdee.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rwx.zhengqikj.top

[U67] PHP：处理文件上传
来源：http://kim.hnxiangtu.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://jkl.zhixingplan.top

[U68] PHP：PDO 连接
来源：http://qmb.vqdsnc.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jjt.yj202588.top

[U69] PHP：PDO 预处理
来源：http://vkr.fengsongda.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://hmw.yuxming.cn

[U70] PHP：PDO 事务
来源：http://dwa.sysykeji.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vts.zdbjq.cn

[U71] PHP：抛出异常
来源：http://qcm.yueranfly.top

throw new RuntimeException("失败", 500);
来源：http://ark.fehbvm.com

[U72] PHP：写错误日志
来源：http://rup.birdmap.top

error_log("失败: " . $e->getMessage());
来源：http://kxu.zdbjq.cn

[U73] PHP：读取 ini 配置
来源：http://ozg.zdqjudy.top

parse_ini_file("config.ini", true)
来源：http://iew.yj20258.top

[U74] PHP：读取环境变量
来源：http://cmu.shanyushiyangkeji.top

getenv("APP_ENV") ?: "production"
来源：http://lzf.zycfv.cn


<!-- 参考信息 -->