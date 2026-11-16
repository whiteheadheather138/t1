代发 wailian999

[S45] C++：lambda
来源：http://bpe.ivvv.top

auto add = [](int a, int b) { return a + b; };
来源：http://dis.mhx1999.top

[S46] C++：函数模板
来源：http://gdj.cucudq.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://opv.gaohongyu789.top

[S47] C++：结构化绑定遍历
来源：http://kzb.birdmap.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jfj.pengpengdd.cyou

[S48] C++：逐行读文件
来源：http://wpy.zhiwuduotai.top

std::ifstream in("a.txt");  std::string line;
来源：http://ozj.jinqigufen.top

while (std::getline(in, line)) { }
来源：http://ujd.haohaochexian.top

[S49] C++：写文件
来源：http://yqf.cdnleiting.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rvg.daxiang520.top

[S50] C++：格式化数字
来源：http://pnt.jinqigfzy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hgn.meibo888.top

[S51] C++：显式类型转换
来源：http://qoq.zhixingplan.top

static_cast<double>(a) / b
来源：http://dnm.jinyuanbaomall.cn

[S52] C++：const 与 noexcept
来源：http://egh.cheryme.top

int size() const noexcept { return n_; }
来源：http://rer.wangshuangyany.cn

[S53] C++：移动语义
来源：http://dgf.hammf.cn

std::vector<int> w = std::move(v);
来源：http://bgx.yfazqb.com

[S54] C++：异常处理
来源：http://rxu.tanke756.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gak.jlsjyb.cn

[S55] C++：结构化绑定
来源：http://yne.sweek.top

auto [a, b] = std::make_pair(1, 2);
来源：http://plm.iojbl.cn

[S56] C++：optional
来源：http://afr.zdqjudy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rtf.tarul.cn

[S57] C++：编译期常量
来源：http://ams.bjfxy.top

constexpr int N = 10;
来源：http://jol.yuxming.cn

[S58] C++：命名空间
来源：http://xzl.shzxlz.cn

namespace ns { int f() { return 1; } }
来源：http://nyr.sxryk.cn

[S59] C++：静态断言
来源：http://ltv.xingfuxueyuan.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nxh.hfpthk.cn

[S60] C++：遍历并删除元素
来源：http://lxo.nanxuanxn.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ken.tian-w.cn

================================================================================
来源：http://dey.tanke756.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dvf.smart0.xyz

================================================================================
来源：http://amh.jinyuanbaomall.cn

[T01] Kotlin：Hello World
来源：http://uuv.tianlin.xyz

println("Hello")
来源：http://wii.jlsjyb.cn

[T02] Kotlin：变量
来源：http://tmu.yfazqb.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qxf.jqgufenzy.top

[T03] Kotlin：字符串模板
来源：http://cqx.9152youxi.cn

"值: $b"
来源：http://woj.zhaomingkeji.xyz

[T04] Kotlin：空安全
来源：http://lbs.yonumen.top

val n: String? = null;  n?.length
来源：http://xpi.jqgfzy.top

[T05] Kotlin：when 表达式
来源：http://bfa.yfazqb.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mkv.xuetiantiany.cn

[T06] Kotlin：集合映射
来源：http://wgt.tian-w.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://nhp.epnwcf.com

[T07] Kotlin：集合过滤
来源：http://gmg.shanyushiyangtech.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://tqw.sxryk.cn

[T08] Kotlin：数据类
来源：http://dhn.shanyushiyangkeji.top

data class User(val name: String, val age: Int)
来源：http://wiy.zhixingplan.top

[T09] Kotlin：扩展函数
来源：http://fak.bjfxy.top

fun String.exclaim() = this + "!"
来源：http://tqn.chenlongwang.top

[T10] Kotlin：默认参数
来源：http://kze.xuanzx.com

fun greet(name: String = "World") = "Hi $name"
来源：http://gey.zdbjq.cn

[T11] Kotlin：协程
来源：http://wmc.iojbl.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nmy.jinyuanbaomall.cn

[T12] Kotlin：解构声明
来源：http://rct.haohaochexian.top

val (a, b) = Pair(1, 2)
来源：http://rmn.bbcook.cn

[T13] Kotlin：只读 Map
来源：http://axy.ivvv.top

val m = mapOf("a" to 1)
来源：http://sse.sufxvd.cn

[T14] Kotlin：循环
来源：http://cxz.yuanzhike.top

for (i in 1..10) println(i)
来源：http://cqq.jinqigfzy.top

[T15] Kotlin：接口
来源：http://hog.zhengqikj.top

interface Shape { fun area(): Double }
来源：http://lgl.ppjwa.cn

[T16] Swift：Hello World
来源：http://dyr.bjfxy.top

print("Hello")
来源：http://cdu.9152youxi.cn

[T17] Swift：变量与常量
来源：http://rul.iojbl.cn

var a = 1;  let b = 2
来源：http://xil.ctjpmb.com

[T18] Swift：字符串插值
来源：http://wes.vqdsnc.cn

"值: \(b)"
来源：http://mey.hfpthk.cn

[T19] Swift：可选绑定
来源：http://tzy.ehwqpu.com

if let n = opt { print(n) }
来源：http://fkg.yueranfly.top

[T20] Swift：数组操作
来源：http://yco.gaohongyu789.top

var a = [1, 2, 3];  a.append(4)
来源：http://eio.52xcode.cn

[T21] Swift：遍历
来源：http://pwo.52xcode.cn

for x in a { print(x) }
来源：http://rzf.quarkkingdee.top

[T22] Swift：字典
来源：http://jjn.cdnleiting.top

var d = ["a": 1];  d["b"] = 2
来源：http://gcr.hfpthk.cn

[T23] Swift：函数
来源：http://syv.iojbl.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nzm.ivvv.top

[T24] Swift：闭包
来源：http://vmp.shanyushiyangkeji.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://wab.ydzc1.top

[T25] Swift：结构体
来源：http://mig.birdmap.top

struct P { var x: Int }
来源：http://bko.ybcxt.top

[T26] Swift：类与重写
来源：http://avy.yuxming.cn

class A: Base { override func f() {} }
来源：http://eyp.uphjek.com

[T27] Swift：错误处理
来源：http://ipv.ehwqpu.com

do { try f() } catch { print(error) }
来源：http://ghh.daxiang520.top

[T28] Swift：枚举
来源：http://rxw.aibaodan.cn

enum Color { case red, green }
来源：http://dit.meibo888.top

[T29] Swift：guard 提前返回
来源：http://art.hcnkem.com

guard let x = opt else { return }
来源：http://uwz.cqqwz.cn

[T30] Swift：协议
来源：http://joi.yuxming.cn

protocol Shape { func area() -> Double }
来源：http://bdw.andypj.xyz

[T31] Lua：Hello World
来源：http://ebj.svipenyu.cn

print("Hello")
来源：http://kbv.guannengcc.top

[T32] Lua：局部变量
来源：http://koz.jinyuanbaomall.cn

local a = 1
来源：http://eyd.zhongyouzk.top

[T33] Lua：表（数组）
来源：http://xee.yanxiufei.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://bje.jinqigufen.top

[T34] Lua：遍历表
来源：http://lzz.hysaishi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://vqx.cdnleiting.top

[T35] Lua：字典表
来源：http://doq.smart0.xyz

local d = { a = 1 };  d.b = 2
来源：http://usl.hnxiangtu.top

[T36] Lua：函数
来源：http://lnc.shanyushiyangkeji.top

function add(a, b) return a + b end
来源：http://qhv.birdmap.top

[T37] Lua：字符串拼接
来源：http://rsg.mhx1999.top

"a" .. "b"
来源：http://jwe.daxiang520.top

[T38] Lua：条件
来源：http://qst.zhijiandao.cn

if x > 0 then print("正") end
来源：http://ifc.shanyushiyangtech.top

[T39] Lua：模式匹配
来源：http://ehz.hesvh.cn

string.find(s, "%d+")
来源：http://zhi.ydjk.org.cn

[T40] Lua：元表
来源：http://ciq.cucudq.cn

setmetatable({}, { __index = base })
来源：http://mfy.tarul.cn

[T41] Perl：Hello World
来源：http://jly.smart0.xyz

print "Hello\n";
来源：http://hsn.uphjek.com

[T42] Perl：变量类型
来源：http://gvc.jinqigufen.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zqs.mhx1999.top

[T43] Perl：字符串插值
来源：http://abg.jianghu66.top

"值: $a"
来源：http://zcx.hesvh.cn

[T44] Perl：条件
来源：http://vpq.jiagoushi.top

if ($a > 0) { print "正"; }
来源：http://boq.cashguo.top

[T45] Perl：数组遍历
来源：http://jfc.shzxlz.cn

for my $x (@arr) { print $x; }
来源：http://bux.fanxiaobao.xyz

[T46] Perl：哈希操作
来源：http://irq.gaohongyu789.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hui.jinghuilouyu.cn

[T47] Perl：正则捕获
来源：http://gto.yvedp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://rhi.jqgufenzy.top

[T48] Perl：正则替换
来源：http://tum.0kj1m.cn

$s =~ s/old/new/g;
来源：http://ofr.xuanzx.com

[T49] Perl：函数
来源：http://fek.fehbvm.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bas.tanke756.top

[T50] Perl：逐行读文件
来源：http://rhs.wangdashe.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ury.chenzaomai.com

while (my $line = <$fh>) { print $line; }
来源：http://ntk.feifeiyinyue.top

[T51] Scala：Hello World
来源：http://ebg.zhongyouzk.top

println("Hello")
来源：http://ikv.nanxuanxn.top

[T52] Scala：变量
来源：http://gok.snrcjt.cn

val a = 1;  var b = 2
来源：http://ltn.hnxiangtu.top

[T53] Scala：字符串插值
来源：http://rnp.andypj.xyz

s"值: $b"
来源：http://hbi.shanyushiyangtech.top

[T54] Scala：集合映射
来源：http://nlc.jinqigfzy.top

List(1, 2, 3).map(_ * 2)
来源：http://sss.sjlbkw.cn

[T55] Scala：集合过滤
来源：http://jgf.hesvh.cn

List(1, 2, 3).filter(_ > 1)
来源：http://lvq.sysykeji.top

[T56] Scala：样例类
来源：http://tne.chenjidiqi.icu

case class User(name: String, age: Int)
来源：http://ecd.xuetiantiany.cn

[T57] Scala：模式匹配
来源：http://xhy.yanxiufei.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wtm.zhongyouzk.top

[T58] Scala：函数定义
来源：http://nph.bbcook.cn

def add(a: Int, b: Int): Int = a + b
来源：http://alz.guowangkeji.top

[T59] Scala：循环
来源：http://rtp.xingfuxueyuan.xyz

for (i <- 1 to 10) println(i)
来源：http://qvn.yuxming.cn

[T60] Scala：折叠
来源：http://apy.yj20258.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ocd.daxiang520.top

================================================================================
来源：http://dad.ydzc1.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://quu.nanxinkj.top

================================================================================
来源：http://ytt.yj20258.top

[U01] Py：创建虚拟环境
来源：http://ghs.hnqzz.top

python -m venv .venv && source .venv/bin/activate
来源：http://hxc.yj202588.top

[U02] Py：导出 / 安装依赖
来源：http://fbm.jqgufenzy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://odv.shanyushiyangtech.top

[U03] Py：加载 .env 配置
来源：http://hic.zhongyouzk.top

from dotenv import load_dotenv; load_dotenv()
来源：http://zpp.andypj.xyz

[U04] Py：变量调试打印
来源：http://sgz.pycfn.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://sqp.aizwys.cn

[U05] Py：列表去重且保序
来源：http://saj.kuanghao11.cn

list(dict.fromkeys(arr))
来源：http://asz.zhongyouzk.top

[U06] Py：合并两个字典
来源：http://uie.hesvh.cn

{**a, **b}
来源：http://fpv.gogol.net.cn

[U07] Py：反转字典键值
来源：http://kze.52xcode.cn

{v: k for k, v in d.items()}
来源：http://znu.mhx1999.top

[U08] Py：展平二维列表
来源：http://lgk.daxiang520.top

[y for x in nested for y in x]
来源：http://jje.shanyushiyangtech.top

[U09] Py：字典取最大值的键
来源：http://ert.svipenyu.cn

max(d, key=d.get)
来源：http://yiu.xingfuxueyuan.xyz

[U10] Py：按值排序字典
来源：http://bce.zhoulong.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://azd.hongshengwenyu.top

[U11] Py：生成器表达式
来源：http://ixx.zhiwuduotai.top

(x * 2 for x in arr)
来源：http://mma.nanxinkj.top

[U12] Py：取出现最多的 3 个元素
来源：http://zim.jinyuanbaomall.cn

Counter(arr).most_common(3)
来源：http://ruh.jqgufenzy.top

[U13] Py：固定长度队列
来源：http://hpv.zdqjudy.top

deque(maxlen=10)
来源：http://dhv.havefunace.top

[U14] Py：分组收集到列表
来源：http://uwk.xylfe.cn

defaultdict(list)
来源：http://pgy.sxryk.cn

[U15] Py：高精度计时
来源：http://njn.hcnkem.com

t = time.perf_counter()
来源：http://ofz.jqgfzy.top

[U16] Py：命令行参数解析
来源：http://kio.haohaochexian.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://sum.316326.xyz

[U17] Py：初始化日志
来源：http://grx.jiagoushi.top

logging.basicConfig(level=logging.INFO)
来源：http://hzt.zhiwuduotai.top

[U18] Py：预编译正则
来源：http://sqe.sufxvd.cn

pat = re.compile(r"\d+")
来源：http://rav.haohaochexian.top

[U19] Py：正则替换带回调
来源：http://ogg.hongshengwenyu.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wvy.snrcjt.cn

[U20] Py：缓存函数结果
来源：http://wwh.hammf.cn

@functools.lru_cache(maxsize=None)
来源：http://byp.yvedp.cn

[U21] Py：自定义上下文管理器
来源：http://gbq.yuxming.cn

@contextlib.contextmanager
来源：http://pyp.meibo888.top

[U22] Py：矩阵转置
来源：http://akc.shzxlz.cn

list(zip(*m))
来源：http://qam.guowangkeji.top

[U23] Py：分块读取大文件
来源：http://mmk.yueranfly.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zby.chenzaomai.com

[U24] Py：路径操作
来源：http://weh.yongpay.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xxs.zhijiandao.cn

[U25] Py：CSV 按字典读
来源：http://tre.dashuyun.cn

csv.DictReader(f)
来源：http://wnj.sjlbkw.cn

[U26] Py：并发下载
来源：http://mjf.birdmap.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ogh.9152youxi.cn

[U27] Py：异步 HTTP
来源：http://bfh.vehdjk.com

aiohttp.ClientSession() 配合 async with
来源：http://bmi.jlsjyb.cn

[U28] Py：类型别名
来源：http://irh.tarul.cn

UserId = int
来源：http://vxj.tianlin.xyz

[U29] Py：属性校验
来源：http://zxo.fanxiaobao.xyz

@property 与 @x.setter 配合
来源：http://zwq.bbcook.cn

[U30] Py：数据类
来源：http://cpz.jqgfzy.top

@dataclass(slots=True)
来源：http://zkn.shangyingyoupin.top

[U31] Py：单测
来源：http://nle.jqgfzy.top

python -m pytest -q
来源：http://jfr.yvedp.cn

[U32] Py：代码格式化
来源：http://iqa.wangdashe.top

ruff format . && ruff check --fix .
来源：http://gbo.xingfuxueyuan.xyz

[U33] Py：打包发布
来源：http://mjc.jinghuilouyu.cn

python -m build  （依赖 pyproject.toml）
来源：http://sdg.hfpthk.cn

[U34] Py：判断编码
来源：http://ljk.tarul.cn

chardet.detect(raw)
来源：http://aqq.yuanzhike.top

[U35] Py：发送邮件
来源：http://jbk.gaohongyu789.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ezf.tianlin.xyz

[U36] Py：定时任务
来源：http://uxa.yj202588.top

schedule.every(10).minutes.do(job)
来源：http://ylb.zhijiandao.cn

[U37] Py：读写 Excel
来源：http://rgf.cheryme.top

pandas.read_excel / DataFrame.to_excel
来源：http://xxc.iojbl.cn

[U38] Py：获取脚本所在目录
来源：http://erc.jlsjyb.cn

Path(__file__).resolve().parent
来源：http://rfw.zhixingplan.top

[U39] Py：判断是否在交互环境
来源：http://xsg.sweek.top

sys.stdout.isatty()
来源：http://kgo.zhiwuduotai.top

[U40] Py：打印到标准错误
来源：http://drx.yanxiufei.cn

print("err", file=sys.stderr)
来源：http://opj.shanyushiyangtech.top

[U41] PHP：初始化 Composer 项目
来源：http://szg.wangdashe.top

composer init;  composer require guzzlehttp/guzzle
来源：http://xlj.dashuyun.cn

[U42] PHP：PSR-4 自动加载
来源：http://mwm.hfpthk.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://goq.shanyushiyangkeji.top

[U43] PHP：声明命名空间
来源：http://ytk.iojbl.cn

namespace App\Http;
来源：http://sxb.hfpthk.cn

[U44] PHP：开启严格类型
来源：http://ifx.iojbl.cn

declare(strict_types=1);
来源：http://sem.dashuyun.cn

[U45] PHP：类型声明与返回类型
来源：http://mdr.yangfankeji.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://slj.daria6918.cn

[U46] PHP：可空类型
来源：http://mmy.yonumen.top

?string $name = null
来源：http://kbb.jqgfzy.top

[U47] PHP：联合类型
来源：http://sam.ydjk.org.cn

int|string $id
来源：http://von.yfazqb.com

[U48] PHP：纯枚举
来源：http://jfn.hywenlv.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kud.wangshuangyany.cn

[U49] PHP：只读属性
来源：http://cax.birdmap.top

public readonly string $name
来源：http://qwe.dianchejie.cn

[U50] PHP：构造器属性提升
来源：http://nts.gzhubu.top

public function __construct(private int $id) {}
来源：http://phu.zhixingplan.top

[U51] PHP：数组解构
来源：http://dqz.ydjk.org.cn

[$a, $b] = $arr;
来源：http://wrk.dianchejie.cn

[U52] PHP：箭头函数
来源：http://dzl.shangyingyoupin.top

$double = fn($x) => $x * 2;
来源：http://qpj.zycfv.cn

[U53] PHP：空合并运算符
来源：http://pse.meibo888.top

$v = $a ?? $b ?? "default";
来源：http://soj.aizwys.cn

[U54] PHP：空安全调用
来源：http://kwn.guowangkeji.top

$obj?->method()
来源：http://heb.aibaodan.cn

[U55] PHP：match 表达式
来源：http://fhv.xylfe.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qxn.9152youxi.cn

[U56] PHP：命名参数
来源：http://rod.bjfxy.top

f(a: 1, b: 2)
来源：http://gxm.sjlbkw.cn

[U57] PHP：字符串插值
来源：http://iyk.gogol.net.cn

"值: {$a}"
来源：http://fnj.hfpthk.cn

[U58] PHP：数组三件套
来源：http://xyp.pengpengdd.cyou

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://umk.tian-w.cn

[U59] PHP：自定义排序
来源：http://xdl.yvedp.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dhl.tianlin.xyz

[U60] PHP：JSON 编解码
来源：http://hdg.shzxlz.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wom.nanxuanxn.top

[U61] PHP：正则
来源：http://hki.sjlbkw.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://unt.nanxinkj.top

[U62] PHP：日期对象
来源：http://dng.hywenlv.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://oiy.yanxiufei.cn

[U63] PHP：文件读写
来源：http://fjj.ywan-chungtsiang.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pfv.yj20258888.top

[U64] PHP：目录遍历
来源：http://nsl.nwbrower.top

glob("dir/*.php");  scandir("dir");
来源：http://gtl.yangfankeji.com

[U65] PHP：会话
来源：http://ood.yongpay.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ned.guowangkeji.top

[U66] PHP：设置 Cookie
来源：http://mhh.tarul.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mys.smart0.xyz

[U67] PHP：处理文件上传
来源：http://qah.ehwqpu.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fve.aibaodan.cn

[U68] PHP：PDO 连接
来源：http://mov.chenlongwang.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vvp.hnxiangtu.top

[U69] PHP：PDO 预处理
来源：http://oyq.tarul.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://tgc.fzhhl.top

[U70] PHP：PDO 事务
来源：http://ohx.gzhubu.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://cvl.52xcode.cn


<!-- 参考信息 -->