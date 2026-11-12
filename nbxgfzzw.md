代发 wailian999

[S47] C++：结构化绑定遍历
来源：http://ihl.sjlbkw.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qvc.kuanghao11.cn

[S48] C++：逐行读文件
来源：http://cwc.guowangkeji.top

std::ifstream in("a.txt");  std::string line;
来源：http://snv.tian-w.cn

while (std::getline(in, line)) { }
来源：http://hdu.tarul.cn

[S49] C++：写文件
来源：http://sqq.xinyue.icu

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fdn.yueranfly.top

[S50] C++：格式化数字
来源：http://thp.iojbl.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gze.fktsv.cn

[S51] C++：显式类型转换
来源：http://qos.fehbvm.com

static_cast<double>(a) / b
来源：http://lns.vqdsnc.cn

[S52] C++：const 与 noexcept
来源：http://evz.9152youxi.cn

int size() const noexcept { return n_; }
来源：http://lgn.yueranfly.top

[S53] C++：移动语义
来源：http://hcv.zhongyouzk.top

std::vector<int> w = std::move(v);
来源：http://vov.ydjk.org.cn

[S54] C++：异常处理
来源：http://zpz.daxiang520.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dle.wangshuangyany.cn

[S55] C++：结构化绑定
来源：http://nak.hcnkem.com

auto [a, b] = std::make_pair(1, 2);
来源：http://sel.daria6918.cn

[S56] C++：optional
来源：http://gec.yj20258888.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://aqk.xingfuxueyuan.xyz

[S57] C++：编译期常量
来源：http://mpd.jinghuilouyu.cn

constexpr int N = 10;
来源：http://ulq.sweek.top

[S58] C++：命名空间
来源：http://fhd.jinyuanbaomall.cn

namespace ns { int f() { return 1; } }
来源：http://njn.uphjek.com

[S59] C++：静态断言
来源：http://kle.tian-w.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pkc.snrcjt.cn

[S60] C++：遍历并删除元素
来源：http://ees.tanke756.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gea.kuanghao11.cn

================================================================================
来源：http://kte.yj202588.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://avk.cdnleiting.top

================================================================================
来源：http://edj.hcnkem.com

[T01] Kotlin：Hello World
来源：http://dzm.pycfn.com

println("Hello")
来源：http://der.hysaishi.cn

[T02] Kotlin：变量
来源：http://aav.yj20258888.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://obz.hesvh.cn

[T03] Kotlin：字符串模板
来源：http://ihb.jqgufenzy.top

"值: $b"
来源：http://tcu.gogol.net.cn

[T04] Kotlin：空安全
来源：http://iyi.jinqigufen.top

val n: String? = null;  n?.length
来源：http://dpi.jlsjyb.cn

[T05] Kotlin：when 表达式
来源：http://irn.vehdjk.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dyl.ivvv.top

[T06] Kotlin：集合映射
来源：http://ojp.yangfankeji.com

listOf(1, 2, 3).map { it * 2 }
来源：http://rjl.xziqi.cn

[T07] Kotlin：集合过滤
来源：http://slj.ywan-chungtsiang.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://vba.guannengcc.top

[T08] Kotlin：数据类
来源：http://cib.zdqjudy.top

data class User(val name: String, val age: Int)
来源：http://wsf.yuxming.cn

[T09] Kotlin：扩展函数
来源：http://szr.yangfankeji.com

fun String.exclaim() = this + "!"
来源：http://omt.iojbl.cn

[T10] Kotlin：默认参数
来源：http://ebj.haohaochexian.top

fun greet(name: String = "World") = "Hi $name"
来源：http://onr.sufxvd.cn

[T11] Kotlin：协程
来源：http://ojt.ctjpmb.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://xsp.zhixingplan.top

[T12] Kotlin：解构声明
来源：http://ouv.jinghuilouyu.cn

val (a, b) = Pair(1, 2)
来源：http://lav.yfazqb.com

[T13] Kotlin：只读 Map
来源：http://bmr.birdmap.top

val m = mapOf("a" to 1)
来源：http://qhu.zdqjudy.top

[T14] Kotlin：循环
来源：http://zsq.yuxming.cn

for (i in 1..10) println(i)
来源：http://zbp.shanyushiyangtech.top

[T15] Kotlin：接口
来源：http://chl.cqqwz.cn

interface Shape { fun area(): Double }
来源：http://zfc.gotoacloud.top

[T16] Swift：Hello World
来源：http://liz.aibaodan.cn

print("Hello")
来源：http://azp.fktsv.cn

[T17] Swift：变量与常量
来源：http://syu.quarkkingdee.top

var a = 1;  let b = 2
来源：http://pjv.zdbjq.cn

[T18] Swift：字符串插值
来源：http://bqz.jlsjyb.cn

"值: \(b)"
来源：http://egr.yanxiufei.cn

[T19] Swift：可选绑定
来源：http://idr.yuanzhike.top

if let n = opt { print(n) }
来源：http://xij.dashuyun.cn

[T20] Swift：数组操作
来源：http://zfw.mhx1999.top

var a = [1, 2, 3];  a.append(4)
来源：http://qij.0kj1m.cn

[T21] Swift：遍历
来源：http://vke.quarkkingdee.top

for x in a { print(x) }
来源：http://zns.pengpengdd.cyou

[T22] Swift：字典
来源：http://xok.ctjpmb.com

var d = ["a": 1];  d["b"] = 2
来源：http://eaf.zhiwuduotai.top

[T23] Swift：函数
来源：http://hwu.birdmap.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ywe.daxiang520.top

[T24] Swift：闭包
来源：http://zum.jinqigufen.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://taz.xylfe.cn

[T25] Swift：结构体
来源：http://fke.yonumen.top

struct P { var x: Int }
来源：http://nnb.daxiang520.top

[T26] Swift：类与重写
来源：http://ryy.havefunace.top

class A: Base { override func f() {} }
来源：http://hyf.yangfankeji.com

[T27] Swift：错误处理
来源：http://ven.jianghu66.top

do { try f() } catch { print(error) }
来源：http://evh.hongshengwenyu.top

[T28] Swift：枚举
来源：http://abn.nwbrower.top

enum Color { case red, green }
来源：http://ycm.ydzc1.top

[T29] Swift：guard 提前返回
来源：http://twx.redwolf501.top

guard let x = opt else { return }
来源：http://zih.chenzaomai.com

[T30] Swift：协议
来源：http://nip.haohaochexian.top

protocol Shape { func area() -> Double }
来源：http://rlr.wangdashe.top

[T31] Lua：Hello World
来源：http://ogw.yongpay.top

print("Hello")
来源：http://zkz.ctjpmb.com

[T32] Lua：局部变量
来源：http://ieh.shanyushiyangtech.top

local a = 1
来源：http://nvg.shzxlz.cn

[T33] Lua：表（数组）
来源：http://oiz.sxryk.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ibv.wangdashe.top

[T34] Lua：遍历表
来源：http://kdu.cucudq.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://fvh.sweek.top

[T35] Lua：字典表
来源：http://zoi.jqgfzy.top

local d = { a = 1 };  d.b = 2
来源：http://qeg.ivvv.top

[T36] Lua：函数
来源：http://nln.pycfn.com

function add(a, b) return a + b end
来源：http://dyg.52xcode.cn

[T37] Lua：字符串拼接
来源：http://ief.jianghu66.top

"a" .. "b"
来源：http://rua.zhengqikj.top

[T38] Lua：条件
来源：http://tee.sweek.top

if x > 0 then print("正") end
来源：http://fip.xingfuxueyuan.xyz

[T39] Lua：模式匹配
来源：http://cyz.9152youxi.cn

string.find(s, "%d+")
来源：http://mfm.nwbrower.top

[T40] Lua：元表
来源：http://scb.c1oappe.top

setmetatable({}, { __index = base })
来源：http://dpo.9152youxi.cn

[T41] Perl：Hello World
来源：http://jxk.fzhhl.top

print "Hello\n";
来源：http://sjt.ywan-chungtsiang.top

[T42] Perl：变量类型
来源：http://umy.daxiang520.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://njx.gogol.net.cn

[T43] Perl：字符串插值
来源：http://utp.gzhubu.top

"值: $a"
来源：http://kmc.ctjpmb.com

[T44] Perl：条件
来源：http://bzs.jianghu66.top

if ($a > 0) { print "正"; }
来源：http://vop.xylfe.cn

[T45] Perl：数组遍历
来源：http://jez.nanxuanxn.top

for my $x (@arr) { print $x; }
来源：http://djj.andypj.xyz

[T46] Perl：哈希操作
来源：http://ozq.hnxiangtu.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fmw.jianghu66.top

[T47] Perl：正则捕获
来源：http://kys.bbcook.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wmm.mhx1999.top

[T48] Perl：正则替换
来源：http://bhu.jinqigfzy.top

$s =~ s/old/new/g;
来源：http://gpj.hesvh.cn

[T49] Perl：函数
来源：http://xyc.yuanzhike.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fsu.jqgufenzy.top

[T50] Perl：逐行读文件
来源：http://wkn.hcnkem.com

open my $fh, "<", "a.txt" or die $!;
来源：http://wzn.mhx1999.top

while (my $line = <$fh>) { print $line; }
来源：http://wum.iojbl.cn

[T51] Scala：Hello World
来源：http://vob.cucudq.cn

println("Hello")
来源：http://ymm.yj20258888.top

[T52] Scala：变量
来源：http://naq.zhongyouzk.top

val a = 1;  var b = 2
来源：http://umr.snrcjt.cn

[T53] Scala：字符串插值
来源：http://jfe.nanxinkj.top

s"值: $b"
来源：http://wze.nwbrower.top

[T54] Scala：集合映射
来源：http://xja.yuxming.cn

List(1, 2, 3).map(_ * 2)
来源：http://vjd.yfazqb.com

[T55] Scala：集合过滤
来源：http://exi.jiagoushi.top

List(1, 2, 3).filter(_ > 1)
来源：http://gdu.zhaomingkeji.xyz

[T56] Scala：样例类
来源：http://gew.zdbjq.cn

case class User(name: String, age: Int)
来源：http://qfi.fengsongda.top

[T57] Scala：模式匹配
来源：http://gkk.svipenyu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://mkb.gogol.net.cn

[T58] Scala：函数定义
来源：http://wwk.yj20258.top

def add(a: Int, b: Int): Int = a + b
来源：http://lcx.jqgfzy.top

[T59] Scala：循环
来源：http://muu.ywan-chungtsiang.top

for (i <- 1 to 10) println(i)
来源：http://cfi.hfpthk.cn

[T60] Scala：折叠
来源：http://uer.jinyuanbaomall.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wkk.ybcxt.top

================================================================================
来源：http://igv.tarul.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ieo.vqdsnc.cn

================================================================================
来源：http://avc.jiagoushi.top

[U01] Py：创建虚拟环境
来源：http://dbx.wangshuangyany.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vmk.xziqi.cn

[U02] Py：导出 / 安装依赖
来源：http://prt.jyoumei.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cwt.xuanzx.com

[U03] Py：加载 .env 配置
来源：http://xcc.svipenyu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://pfy.chenlongwang.top

[U04] Py：变量调试打印
来源：http://wgu.yueranfly.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gnr.tianlin.xyz

[U05] Py：列表去重且保序
来源：http://irp.gzhubu.top

list(dict.fromkeys(arr))
来源：http://skc.jlsjyb.cn

[U06] Py：合并两个字典
来源：http://pfd.yuxming.cn

{**a, **b}
来源：http://dmk.zdqjudy.top

[U07] Py：反转字典键值
来源：http://tzn.shuidangran.top

{v: k for k, v in d.items()}
来源：http://ewt.zycfv.cn

[U08] Py：展平二维列表
来源：http://qhj.nwbrower.top

[y for x in nested for y in x]
来源：http://jae.jinghuilouyu.cn

[U09] Py：字典取最大值的键
来源：http://ltt.vehdjk.com

max(d, key=d.get)
来源：http://yli.feifeiyinyue.top

[U10] Py：按值排序字典
来源：http://wfv.jqgufenzy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://swu.xziqi.cn

[U11] Py：生成器表达式
来源：http://umi.hongshengwenyu.top

(x * 2 for x in arr)
来源：http://fsi.jinyuanbaomall.cn

[U12] Py：取出现最多的 3 个元素
来源：http://huc.sjlbkw.cn

Counter(arr).most_common(3)
来源：http://vui.wangdashe.top

[U13] Py：固定长度队列
来源：http://sqo.fzhhl.top

deque(maxlen=10)
来源：http://yxg.hywenlv.cn

[U14] Py：分组收集到列表
来源：http://gks.pengpengdd.cyou

defaultdict(list)
来源：http://apt.zdqjudy.top

[U15] Py：高精度计时
来源：http://xmq.tian-w.cn

t = time.perf_counter()
来源：http://wdc.fanxiaobao.xyz

[U16] Py：命令行参数解析
来源：http://bfx.birdmap.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ern.yangfankeji.com

[U17] Py：初始化日志
来源：http://sxz.vehdjk.com

logging.basicConfig(level=logging.INFO)
来源：http://izv.zdqjudy.top

[U18] Py：预编译正则
来源：http://rpe.xylfe.cn

pat = re.compile(r"\d+")
来源：http://qtw.fehbvm.com

[U19] Py：正则替换带回调
来源：http://hxy.cashguo.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wtt.wangshuangyany.cn

[U20] Py：缓存函数结果
来源：http://ixk.epnwcf.com

@functools.lru_cache(maxsize=None)
来源：http://wyr.0kj1m.cn

[U21] Py：自定义上下文管理器
来源：http://iyf.nwbrower.top

@contextlib.contextmanager
来源：http://hww.sjlbkw.cn

[U22] Py：矩阵转置
来源：http://jyp.yvedp.cn

list(zip(*m))
来源：http://zmx.316326.xyz

[U23] Py：分块读取大文件
来源：http://hyz.haohaochexian.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qfq.uphjek.com

[U24] Py：路径操作
来源：http://qjo.yueranfly.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gsc.haohaochexian.top

[U25] Py：CSV 按字典读
来源：http://sot.ywan-chungtsiang.top

csv.DictReader(f)
来源：http://rkd.daria6918.cn

[U26] Py：并发下载
来源：http://odp.nanxinkj.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qwe.ctjpmb.com

[U27] Py：异步 HTTP
来源：http://vxx.jqgfzy.top

aiohttp.ClientSession() 配合 async with
来源：http://off.cdnleiting.top

[U28] Py：类型别名
来源：http://ybh.cucudq.cn

UserId = int
来源：http://tlr.dianchejie.cn

[U29] Py：属性校验
来源：http://gxh.zhengqikj.top

@property 与 @x.setter 配合
来源：http://avf.hnxiangtu.top

[U30] Py：数据类
来源：http://gee.zhengqikj.top

@dataclass(slots=True)
来源：http://wil.fanxiaobao.xyz

[U31] Py：单测
来源：http://hxm.yj20258.top

python -m pytest -q
来源：http://txo.hnxiangtu.top

[U32] Py：代码格式化
来源：http://gku.sxryk.cn

ruff format . && ruff check --fix .
来源：http://hhk.ehwqpu.com

[U33] Py：打包发布
来源：http://mhr.yuanzhike.top

python -m build  （依赖 pyproject.toml）
来源：http://wcg.dashuyun.cn

[U34] Py：判断编码
来源：http://zyi.bbcook.cn

chardet.detect(raw)
来源：http://vdq.vqdsnc.cn

[U35] Py：发送邮件
来源：http://gsm.hysaishi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dxr.hnxiangtu.top

[U36] Py：定时任务
来源：http://bqo.cashguo.top

schedule.every(10).minutes.do(job)
来源：http://ili.dashuyun.cn

[U37] Py：读写 Excel
来源：http://xnc.shzxlz.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ucl.dianchejie.cn

[U38] Py：获取脚本所在目录
来源：http://swz.smart0.xyz

Path(__file__).resolve().parent
来源：http://elt.birdmap.top

[U39] Py：判断是否在交互环境
来源：http://ihy.cashguo.top

sys.stdout.isatty()
来源：http://zky.yanxiufei.cn

[U40] Py：打印到标准错误
来源：http://pyu.gogol.net.cn

print("err", file=sys.stderr)
来源：http://igr.yangfankeji.com

[U41] PHP：初始化 Composer 项目
来源：http://gfq.yfazqb.com

composer init;  composer require guzzlehttp/guzzle
来源：http://blt.316326.xyz

[U42] PHP：PSR-4 自动加载
来源：http://hyl.wangshuangyany.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://teo.jinqigfzy.top

[U43] PHP：声明命名空间
来源：http://emc.ehwqpu.com

namespace App\Http;
来源：http://zjy.316326.xyz

[U44] PHP：开启严格类型
来源：http://ave.zhaomingkeji.xyz

declare(strict_types=1);
来源：http://tqp.yj202588.top

[U45] PHP：类型声明与返回类型
来源：http://atb.fengsongda.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://evz.daxiang520.top

[U46] PHP：可空类型
来源：http://oon.jyoumei.cn

?string $name = null
来源：http://ysx.yonumen.top

[U47] PHP：联合类型
来源：http://grp.jinyuanbaomall.cn

int|string $id
来源：http://ink.guannengcc.top

[U48] PHP：纯枚举
来源：http://pzw.ctjpmb.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tgb.ivvv.top

[U49] PHP：只读属性
来源：http://txd.snrcjt.cn

public readonly string $name
来源：http://uxb.jianghu66.top

[U50] PHP：构造器属性提升
来源：http://hpr.yangfankeji.com

public function __construct(private int $id) {}
来源：http://ece.ywan-chungtsiang.top

[U51] PHP：数组解构
来源：http://yvq.hnxiangtu.top

[$a, $b] = $arr;
来源：http://wbq.cqqwz.cn

[U52] PHP：箭头函数
来源：http://cte.birdmap.top

$double = fn($x) => $x * 2;
来源：http://jxa.sxryk.cn

[U53] PHP：空合并运算符
来源：http://ptu.hfpthk.cn

$v = $a ?? $b ?? "default";
来源：http://ike.jinyuanbaomall.cn

[U54] PHP：空安全调用
来源：http://fdp.fanxiaobao.xyz

$obj?->method()
来源：http://ell.cdnleiting.top

[U55] PHP：match 表达式
来源：http://yze.shzxlz.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ner.gzhubu.top

[U56] PHP：命名参数
来源：http://fcw.52xcode.cn

f(a: 1, b: 2)
来源：http://asc.yj20258888.top

[U57] PHP：字符串插值
来源：http://vue.zycfv.cn

"值: {$a}"
来源：http://plu.jinqigfzy.top

[U58] PHP：数组三件套
来源：http://xfp.ywan-chungtsiang.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zzv.zhiwuduotai.top

[U59] PHP：自定义排序
来源：http://ifj.zdqjudy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tjt.ydzc1.top

[U60] PHP：JSON 编解码
来源：http://hoo.fehbvm.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://xhv.zhoulong.xyz

[U61] PHP：正则
来源：http://wbe.meibo888.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zyt.cashguo.top

[U62] PHP：日期对象
来源：http://qer.hfpthk.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://epg.jinqigufen.top

[U63] PHP：文件读写
来源：http://nnw.tian-w.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bvf.ydjk.org.cn

[U64] PHP：目录遍历
来源：http://bud.jinqigufen.top

glob("dir/*.php");  scandir("dir");
来源：http://qjs.yuanzhike.top

[U65] PHP：会话
来源：http://lkd.fehbvm.com

session_start();  $_SESSION["uid"] = 1;
来源：http://vil.hywenlv.cn

[U66] PHP：设置 Cookie
来源：http://dba.jlsjyb.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://hwl.wangshuangyany.cn

[U67] PHP：处理文件上传
来源：http://pha.hcnkem.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://dmp.jqgfzy.top

[U68] PHP：PDO 连接
来源：http://kdd.sysykeji.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://vhr.yj202588.top

[U69] PHP：PDO 预处理
来源：http://xwc.nanxinkj.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mde.jinqigfzy.top

[U70] PHP：PDO 事务
来源：http://yfh.nanxuanxn.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mre.c1oappe.top

[U71] PHP：抛出异常
来源：http://wyi.quarkkingdee.top

throw new RuntimeException("失败", 500);
来源：http://zjz.daria6918.cn

[U72] PHP：写错误日志
来源：http://ufh.aibaodan.cn

error_log("失败: " . $e->getMessage());
来源：http://fwg.pycfn.com


<!-- 参考信息 -->