代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://ths.chenjidiqi.icu

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bni.jyoumei.cn

[S48] C++：逐行读文件
来源：http://cfp.xinyue.icu

std::ifstream in("a.txt");  std::string line;
来源：http://huc.yj20258.top

while (std::getline(in, line)) { }
来源：http://yiq.jqgfzy.top

[S49] C++：写文件
来源：http://jeg.jinqigufen.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dof.gzhubu.top

[S50] C++：格式化数字
来源：http://qvl.epnwcf.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xwi.cucudq.cn

[S51] C++：显式类型转换
来源：http://bmb.hcnkem.com

static_cast<double>(a) / b
来源：http://eof.daria6918.cn

[S52] C++：const 与 noexcept
来源：http://pym.shangyingyoupin.top

int size() const noexcept { return n_; }
来源：http://gbo.fktsv.cn

[S53] C++：移动语义
来源：http://jke.sweek.top

std::vector<int> w = std::move(v);
来源：http://htl.shuidangran.top

[S54] C++：异常处理
来源：http://fal.ivvv.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kqk.uphjek.com

[S55] C++：结构化绑定
来源：http://gld.yj20258.top

auto [a, b] = std::make_pair(1, 2);
来源：http://tbd.vqdsnc.cn

[S56] C++：optional
来源：http://muy.vqdsnc.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://buv.gotoacloud.top

[S57] C++：编译期常量
来源：http://maa.ppjwa.cn

constexpr int N = 10;
来源：http://kgb.ppjwa.cn

[S58] C++：命名空间
来源：http://dnt.hesvh.cn

namespace ns { int f() { return 1; } }
来源：http://rnj.yj20258888.top

[S59] C++：静态断言
来源：http://kwg.yj202588.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bkl.shuidangran.top

[S60] C++：遍历并删除元素
来源：http://xgv.hywenlv.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wuk.yvedp.cn

================================================================================
来源：http://nih.52xcode.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xhg.gaohongyu789.top

================================================================================
来源：http://cwj.yanxiufei.cn

[T01] Kotlin：Hello World
来源：http://bhk.shzxlz.cn

println("Hello")
来源：http://otz.svipenyu.cn

[T02] Kotlin：变量
来源：http://asf.yongpay.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://upl.fanxiaobao.xyz

[T03] Kotlin：字符串模板
来源：http://pof.jqgufenzy.top

"值: $b"
来源：http://txw.9152youxi.cn

[T04] Kotlin：空安全
来源：http://lgm.ehwqpu.com

val n: String? = null;  n?.length
来源：http://ckj.xinyue.icu

[T05] Kotlin：when 表达式
来源：http://hta.shuidangran.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uyf.hnqzz.top

[T06] Kotlin：集合映射
来源：http://jdk.nwbrower.top

listOf(1, 2, 3).map { it * 2 }
来源：http://dgc.zhiwuduotai.top

[T07] Kotlin：集合过滤
来源：http://iiw.ydjk.org.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ndp.yangfankeji.com

[T08] Kotlin：数据类
来源：http://nbc.nanxinkj.top

data class User(val name: String, val age: Int)
来源：http://mnz.yvedp.cn

[T09] Kotlin：扩展函数
来源：http://dhv.jqgufenzy.top

fun String.exclaim() = this + "!"
来源：http://hwh.daxiang520.top

[T10] Kotlin：默认参数
来源：http://evx.wangdashe.top

fun greet(name: String = "World") = "Hi $name"
来源：http://vwo.tianlin.xyz

[T11] Kotlin：协程
来源：http://gns.fanxiaobao.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://tch.cashguo.top

[T12] Kotlin：解构声明
来源：http://wku.ywan-chungtsiang.top

val (a, b) = Pair(1, 2)
来源：http://gvl.sxryk.cn

[T13] Kotlin：只读 Map
来源：http://krd.zhongyouzk.top

val m = mapOf("a" to 1)
来源：http://hyu.shanyushiyangtech.top

[T14] Kotlin：循环
来源：http://lpn.smart0.xyz

for (i in 1..10) println(i)
来源：http://kga.yj20258.top

[T15] Kotlin：接口
来源：http://ltk.hammf.cn

interface Shape { fun area(): Double }
来源：http://cfs.shangyingyoupin.top

[T16] Swift：Hello World
来源：http://yxz.yfazqb.com

print("Hello")
来源：http://shb.hammf.cn

[T17] Swift：变量与常量
来源：http://cyy.gzhubu.top

var a = 1;  let b = 2
来源：http://xkw.hywenlv.cn

[T18] Swift：字符串插值
来源：http://hww.hfpthk.cn

"值: \(b)"
来源：http://ytk.c1oappe.top

[T19] Swift：可选绑定
来源：http://bhq.nanxuanxn.top

if let n = opt { print(n) }
来源：http://xcr.gotoacloud.top

[T20] Swift：数组操作
来源：http://zvf.sufxvd.cn

var a = [1, 2, 3];  a.append(4)
来源：http://caq.ppjwa.cn

[T21] Swift：遍历
来源：http://bru.shanyushiyangkeji.top

for x in a { print(x) }
来源：http://aul.xylfe.cn

[T22] Swift：字典
来源：http://xwt.birdmap.top

var d = ["a": 1];  d["b"] = 2
来源：http://tdw.tianlin.xyz

[T23] Swift：函数
来源：http://bqn.xuanzx.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dfc.52xcode.cn

[T24] Swift：闭包
来源：http://qvv.birdmap.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://igy.ctjpmb.com

[T25] Swift：结构体
来源：http://sdu.andypj.xyz

struct P { var x: Int }
来源：http://ohb.yj20258.top

[T26] Swift：类与重写
来源：http://bmf.andypj.xyz

class A: Base { override func f() {} }
来源：http://sbg.guowangkeji.top

[T27] Swift：错误处理
来源：http://tps.zdbjq.cn

do { try f() } catch { print(error) }
来源：http://dvl.jyoumei.cn

[T28] Swift：枚举
来源：http://uot.316326.xyz

enum Color { case red, green }
来源：http://mvj.dianchejie.cn

[T29] Swift：guard 提前返回
来源：http://qfo.mhx1999.top

guard let x = opt else { return }
来源：http://mdd.pycfn.com

[T30] Swift：协议
来源：http://vbi.snrcjt.cn

protocol Shape { func area() -> Double }
来源：http://tgh.zdbjq.cn

[T31] Lua：Hello World
来源：http://esm.gaohongyu789.top

print("Hello")
来源：http://pic.cashguo.top

[T32] Lua：局部变量
来源：http://vom.dashuyun.cn

local a = 1
来源：http://xbu.dashuyun.cn

[T33] Lua：表（数组）
来源：http://zmf.redwolf501.top

local t = {1, 2, 3};  t[4] = 4
来源：http://lii.jinqigfzy.top

[T34] Lua：遍历表
来源：http://dsx.fanxiaobao.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://wml.xylfe.cn

[T35] Lua：字典表
来源：http://dyl.zdqjudy.top

local d = { a = 1 };  d.b = 2
来源：http://dbm.xinyue.icu

[T36] Lua：函数
来源：http://afe.pengpengdd.cyou

function add(a, b) return a + b end
来源：http://yzg.dashuyun.cn

[T37] Lua：字符串拼接
来源：http://fgh.sweek.top

"a" .. "b"
来源：http://lav.ehwqpu.com

[T38] Lua：条件
来源：http://ltj.redwolf501.top

if x > 0 then print("正") end
来源：http://rrn.zhixingplan.top

[T39] Lua：模式匹配
来源：http://jly.sufxvd.cn

string.find(s, "%d+")
来源：http://duq.mhx1999.top

[T40] Lua：元表
来源：http://ctq.hnqzz.top

setmetatable({}, { __index = base })
来源：http://eal.316326.xyz

[T41] Perl：Hello World
来源：http://prg.sxryk.cn

print "Hello\n";
来源：http://tfn.sjlbkw.cn

[T42] Perl：变量类型
来源：http://ibe.zdbjq.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qbr.yj20258888.top

[T43] Perl：字符串插值
来源：http://hmu.zdbjq.cn

"值: $a"
来源：http://kry.yongpay.top

[T44] Perl：条件
来源：http://sis.ydjk.org.cn

if ($a > 0) { print "正"; }
来源：http://yds.aizwys.cn

[T45] Perl：数组遍历
来源：http://ssq.bbcook.cn

for my $x (@arr) { print $x; }
来源：http://asc.pengpengdd.cyou

[T46] Perl：哈希操作
来源：http://qsf.316326.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ybv.cashguo.top

[T47] Perl：正则捕获
来源：http://uvg.hammf.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://sgv.vqdsnc.cn

[T48] Perl：正则替换
来源：http://xnn.jinqigfzy.top

$s =~ s/old/new/g;
来源：http://nip.sysykeji.top

[T49] Perl：函数
来源：http://izd.daria6918.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xup.hongshengwenyu.top

[T50] Perl：逐行读文件
来源：http://srg.ybcxt.top

open my $fh, "<", "a.txt" or die $!;
来源：http://idd.hammf.cn

while (my $line = <$fh>) { print $line; }
来源：http://uat.pengpengdd.cyou

[T51] Scala：Hello World
来源：http://dqt.zhengqikj.top

println("Hello")
来源：http://hwj.hongshengwenyu.top

[T52] Scala：变量
来源：http://idl.52xcode.cn

val a = 1;  var b = 2
来源：http://pze.yuxming.cn

[T53] Scala：字符串插值
来源：http://eht.yongpay.top

s"值: $b"
来源：http://cho.jiagoushi.top

[T54] Scala：集合映射
来源：http://lns.tarul.cn

List(1, 2, 3).map(_ * 2)
来源：http://zec.yanxiufei.cn

[T55] Scala：集合过滤
来源：http://bbl.daxiang520.top

List(1, 2, 3).filter(_ > 1)
来源：http://bwq.cdnleiting.top

[T56] Scala：样例类
来源：http://zbn.jqgufenzy.top

case class User(name: String, age: Int)
来源：http://gvw.hesvh.cn

[T57] Scala：模式匹配
来源：http://kiw.yueranfly.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://orv.fzhhl.top

[T58] Scala：函数定义
来源：http://ugs.hcnkem.com

def add(a: Int, b: Int): Int = a + b
来源：http://vkh.cqqwz.cn

[T59] Scala：循环
来源：http://kzo.nwbrower.top

for (i <- 1 to 10) println(i)
来源：http://ubs.ctjpmb.com

[T60] Scala：折叠
来源：http://yvc.shangyingyoupin.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hql.hnxiangtu.top

================================================================================
来源：http://srt.sweek.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zic.chenjidiqi.icu

================================================================================
来源：http://ynn.havefunace.top

[U01] Py：创建虚拟环境
来源：http://txw.sysykeji.top

python -m venv .venv && source .venv/bin/activate
来源：http://jht.iojbl.cn

[U02] Py：导出 / 安装依赖
来源：http://gfd.tian-w.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rgn.xinyue.icu

[U03] Py：加载 .env 配置
来源：http://mub.chenlongwang.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ggi.uphjek.com

[U04] Py：变量调试打印
来源：http://tza.vqdsnc.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fcw.ybcxt.top

[U05] Py：列表去重且保序
来源：http://ery.wangdashe.top

list(dict.fromkeys(arr))
来源：http://uck.xylfe.cn

[U06] Py：合并两个字典
来源：http://fzj.chenjidiqi.icu

{**a, **b}
来源：http://ead.aizwys.cn

[U07] Py：反转字典键值
来源：http://xft.andypj.xyz

{v: k for k, v in d.items()}
来源：http://cvk.feifeiyinyue.top

[U08] Py：展平二维列表
来源：http://fcq.nwbrower.top

[y for x in nested for y in x]
来源：http://llk.fktsv.cn

[U09] Py：字典取最大值的键
来源：http://vvv.feifeiyinyue.top

max(d, key=d.get)
来源：http://mix.sysykeji.top

[U10] Py：按值排序字典
来源：http://kwu.bbcook.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zso.aibaodan.cn

[U11] Py：生成器表达式
来源：http://qpj.feifeiyinyue.top

(x * 2 for x in arr)
来源：http://dxs.fktsv.cn

[U12] Py：取出现最多的 3 个元素
来源：http://yvu.aibaodan.cn

Counter(arr).most_common(3)
来源：http://wsw.birdmap.top

[U13] Py：固定长度队列
来源：http://wgr.birdmap.top

deque(maxlen=10)
来源：http://oxv.yj20258.top

[U14] Py：分组收集到列表
来源：http://alz.xziqi.cn

defaultdict(list)
来源：http://hgz.shanyushiyangkeji.top

[U15] Py：高精度计时
来源：http://zox.fktsv.cn

t = time.perf_counter()
来源：http://jox.daxiang520.top

[U16] Py：命令行参数解析
来源：http://mdh.zhijiandao.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gns.ydzc1.top

[U17] Py：初始化日志
来源：http://spm.yueranfly.top

logging.basicConfig(level=logging.INFO)
来源：http://oit.gaohongyu789.top

[U18] Py：预编译正则
来源：http://sjn.ppjwa.cn

pat = re.compile(r"\d+")
来源：http://mak.jinqigufen.top

[U19] Py：正则替换带回调
来源：http://bwp.tianlin.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://usd.meibo888.top

[U20] Py：缓存函数结果
来源：http://jcc.pengpengdd.cyou

@functools.lru_cache(maxsize=None)
来源：http://rul.hongshengwenyu.top

[U21] Py：自定义上下文管理器
来源：http://oca.sweek.top

@contextlib.contextmanager
来源：http://sem.snrcjt.cn

[U22] Py：矩阵转置
来源：http://oxc.xingfuxueyuan.xyz

list(zip(*m))
来源：http://yob.sjlbkw.cn

[U23] Py：分块读取大文件
来源：http://mky.zhixingplan.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vhs.daxiang520.top

[U24] Py：路径操作
来源：http://tnm.snrcjt.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vqs.snrcjt.cn

[U25] Py：CSV 按字典读
来源：http://uhe.birdmap.top

csv.DictReader(f)
来源：http://fyq.jlsjyb.cn

[U26] Py：并发下载
来源：http://mja.yangfankeji.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://quy.feifeiyinyue.top

[U27] Py：异步 HTTP
来源：http://rvh.yj202588.top

aiohttp.ClientSession() 配合 async with
来源：http://jgz.yj20258.top

[U28] Py：类型别名
来源：http://zdt.yuanzhike.top

UserId = int
来源：http://pcn.zhoulong.xyz

[U29] Py：属性校验
来源：http://nun.shangyingyoupin.top

@property 与 @x.setter 配合
来源：http://xsn.52xcode.cn

[U30] Py：数据类
来源：http://iep.sjlbkw.cn

@dataclass(slots=True)
来源：http://gqo.epnwcf.com

[U31] Py：单测
来源：http://fim.shanyushiyangkeji.top

python -m pytest -q
来源：http://jmp.svipenyu.cn

[U32] Py：代码格式化
来源：http://cfo.yueranfly.top

ruff format . && ruff check --fix .
来源：http://vbv.shanyushiyangkeji.top

[U33] Py：打包发布
来源：http://ihe.bbcook.cn

python -m build  （依赖 pyproject.toml）
来源：http://oba.hesvh.cn

[U34] Py：判断编码
来源：http://jce.316326.xyz

chardet.detect(raw)
来源：http://aem.zhoulong.xyz

[U35] Py：发送邮件
来源：http://cla.guowangkeji.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://igy.nanxinkj.top

[U36] Py：定时任务
来源：http://nrp.yj202588.top

schedule.every(10).minutes.do(job)
来源：http://dik.ydjk.org.cn

[U37] Py：读写 Excel
来源：http://bcc.zhongyouzk.top

pandas.read_excel / DataFrame.to_excel
来源：http://kkz.jinqigfzy.top

[U38] Py：获取脚本所在目录
来源：http://ofc.sysykeji.top

Path(__file__).resolve().parent
来源：http://hsv.chenjidiqi.icu

[U39] Py：判断是否在交互环境
来源：http://fwo.snrcjt.cn

sys.stdout.isatty()
来源：http://cdv.shangyingyoupin.top

[U40] Py：打印到标准错误
来源：http://pmc.guannengcc.top

print("err", file=sys.stderr)
来源：http://lux.aizwys.cn

[U41] PHP：初始化 Composer 项目
来源：http://chu.zhiwuduotai.top

composer init;  composer require guzzlehttp/guzzle
来源：http://nar.jqgufenzy.top

[U42] PHP：PSR-4 自动加载
来源：http://jwk.feifeiyinyue.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fop.yongpay.top

[U43] PHP：声明命名空间
来源：http://jpv.0kj1m.cn

namespace App\Http;
来源：http://qbw.ydjk.org.cn

[U44] PHP：开启严格类型
来源：http://cht.sufxvd.cn

declare(strict_types=1);
来源：http://xfx.ybcxt.top

[U45] PHP：类型声明与返回类型
来源：http://bii.pengpengdd.cyou

function add(int $a, int $b): int { return $a + $b; }
来源：http://jyi.0kj1m.cn

[U46] PHP：可空类型
来源：http://krw.sjlbkw.cn

?string $name = null
来源：http://fxf.jqgfzy.top

[U47] PHP：联合类型
来源：http://hpy.yueranfly.top

int|string $id
来源：http://nwu.jinqigfzy.top

[U48] PHP：纯枚举
来源：http://nfo.hnqzz.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://glt.hywenlv.cn

[U49] PHP：只读属性
来源：http://wjp.tarul.cn

public readonly string $name
来源：http://qms.yongpay.top

[U50] PHP：构造器属性提升
来源：http://ubd.gogol.net.cn

public function __construct(private int $id) {}
来源：http://aqk.yuanzhike.top

[U51] PHP：数组解构
来源：http://ozo.meibo888.top

[$a, $b] = $arr;
来源：http://gma.yangfankeji.com

[U52] PHP：箭头函数
来源：http://ruh.aibaodan.cn

$double = fn($x) => $x * 2;
来源：http://qay.zdbjq.cn

[U53] PHP：空合并运算符
来源：http://qrg.aibaodan.cn

$v = $a ?? $b ?? "default";
来源：http://utw.uphjek.com

[U54] PHP：空安全调用
来源：http://xsb.jqgufenzy.top

$obj?->method()
来源：http://uqs.jqgfzy.top

[U55] PHP：match 表达式
来源：http://ffe.316326.xyz

$s = match($x) { 1 => "一", default => "其他" };
来源：http://myj.hysaishi.cn

[U56] PHP：命名参数
来源：http://czp.zhoulong.xyz

f(a: 1, b: 2)
来源：http://bea.cqqwz.cn

[U57] PHP：字符串插值
来源：http://kmc.yuanzhike.top

"值: {$a}"
来源：http://qel.jyoumei.cn

[U58] PHP：数组三件套
来源：http://lhg.jlsjyb.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fgq.nanxuanxn.top

[U59] PHP：自定义排序
来源：http://wzh.9152youxi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ejq.52xcode.cn

[U60] PHP：JSON 编解码
来源：http://ixa.fanxiaobao.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wvs.jinyuanbaomall.cn

[U61] PHP：正则
来源：http://bko.quarkkingdee.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cgz.zdqjudy.top

[U62] PHP：日期对象
来源：http://unk.sjlbkw.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://eqk.fktsv.cn

[U63] PHP：文件读写
来源：http://hxh.zhongyouzk.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://qqa.cdnleiting.top

[U64] PHP：目录遍历
来源：http://bbx.tanke756.top

glob("dir/*.php");  scandir("dir");
来源：http://cac.hywenlv.cn

[U65] PHP：会话
来源：http://csq.c1oappe.top

session_start();  $_SESSION["uid"] = 1;
来源：http://uso.zdqjudy.top

[U66] PHP：设置 Cookie
来源：http://ghs.jqgufenzy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wzw.ehwqpu.com

[U67] PHP：处理文件上传
来源：http://hyu.shangyingyoupin.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://fdr.hongshengwenyu.top

[U68] PHP：PDO 连接
来源：http://zff.hfpthk.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xme.jianghu66.top

[U69] PHP：PDO 预处理
来源：http://wgo.sufxvd.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://nhq.ppjwa.cn

[U70] PHP：PDO 事务
来源：http://byb.snrcjt.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wkl.hysaishi.cn

[U71] PHP：抛出异常
来源：http://vev.ehwqpu.com

throw new RuntimeException("失败", 500);
来源：http://dmp.redwolf501.top

[U72] PHP：写错误日志
来源：http://ltt.jinqigfzy.top

error_log("失败: " . $e->getMessage());
来源：http://kpm.dashuyun.cn


<!-- 参考信息 -->