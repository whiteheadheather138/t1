代发 wailian999

while (std::getline(in, line)) { }
来源：http://cxh.jinghuilouyu.cn

[S49] C++：写文件
来源：http://thg.haohaochexian.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dio.sysykeji.top

[S50] C++：格式化数字
来源：http://oli.aizwys.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zlm.jinghuilouyu.cn

[S51] C++：显式类型转换
来源：http://qqj.ydzc1.top

static_cast<double>(a) / b
来源：http://svx.jinqigfzy.top

[S52] C++：const 与 noexcept
来源：http://bjg.yfazqb.com

int size() const noexcept { return n_; }
来源：http://lre.guannengcc.top

[S53] C++：移动语义
来源：http://pls.yj20258888.top

std::vector<int> w = std::move(v);
来源：http://sgs.316326.xyz

[S54] C++：异常处理
来源：http://gni.uphjek.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xij.epnwcf.com

[S55] C++：结构化绑定
来源：http://otk.aibaodan.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qrm.zhoulong.xyz

[S56] C++：optional
来源：http://nli.kuanghao11.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rii.ydjk.org.cn

[S57] C++：编译期常量
来源：http://rgk.jinghuilouyu.cn

constexpr int N = 10;
来源：http://tcf.ywan-chungtsiang.top

[S58] C++：命名空间
来源：http://wzl.ybcxt.top

namespace ns { int f() { return 1; } }
来源：http://wgp.cheryme.top

[S59] C++：静态断言
来源：http://gvj.zhixingplan.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hjc.nanxinkj.top

[S60] C++：遍历并删除元素
来源：http://czh.tian-w.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yzk.dashuyun.cn

================================================================================
来源：http://bld.jqgfzy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zdt.fehbvm.com

================================================================================
来源：http://vec.hnqzz.top

[T01] Kotlin：Hello World
来源：http://kwc.ybcxt.top

println("Hello")
来源：http://wdb.xinyue.icu

[T02] Kotlin：变量
来源：http://mod.zhixingplan.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rcn.fktsv.cn

[T03] Kotlin：字符串模板
来源：http://wtb.gotoacloud.top

"值: $b"
来源：http://eoq.hysaishi.cn

[T04] Kotlin：空安全
来源：http://qqy.fzhhl.top

val n: String? = null;  n?.length
来源：http://zoy.yj202588.top

[T05] Kotlin：when 表达式
来源：http://eug.yonumen.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://oxz.yj20258.top

[T06] Kotlin：集合映射
来源：http://zhi.jinghuilouyu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hmb.jinghuilouyu.cn

[T07] Kotlin：集合过滤
来源：http://qby.pengpengdd.cyou

listOf(1, 2, 3).filter { it > 1 }
来源：http://ebf.ivvv.top

[T08] Kotlin：数据类
来源：http://bnl.nwbrower.top

data class User(val name: String, val age: Int)
来源：http://sav.ivvv.top

[T09] Kotlin：扩展函数
来源：http://xqp.chenlongwang.top

fun String.exclaim() = this + "!"
来源：http://gjs.sysykeji.top

[T10] Kotlin：默认参数
来源：http://xkx.dashuyun.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://bjh.jinqigfzy.top

[T11] Kotlin：协程
来源：http://ogt.cashguo.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://cpd.fehbvm.com

[T12] Kotlin：解构声明
来源：http://gxr.316326.xyz

val (a, b) = Pair(1, 2)
来源：http://uyl.smart0.xyz

[T13] Kotlin：只读 Map
来源：http://hte.xziqi.cn

val m = mapOf("a" to 1)
来源：http://clr.jlsjyb.cn

[T14] Kotlin：循环
来源：http://ujj.tianlin.xyz

for (i in 1..10) println(i)
来源：http://lhy.hnxiangtu.top

[T15] Kotlin：接口
来源：http://kgp.yfazqb.com

interface Shape { fun area(): Double }
来源：http://iix.bbcook.cn

[T16] Swift：Hello World
来源：http://jlw.dashuyun.cn

print("Hello")
来源：http://cmf.shzxlz.cn

[T17] Swift：变量与常量
来源：http://exd.daxiang520.top

var a = 1;  let b = 2
来源：http://njc.yuanzhike.top

[T18] Swift：字符串插值
来源：http://hqo.gotoacloud.top

"值: \(b)"
来源：http://azr.gzhubu.top

[T19] Swift：可选绑定
来源：http://mai.gzhubu.top

if let n = opt { print(n) }
来源：http://dfj.quarkkingdee.top

[T20] Swift：数组操作
来源：http://dnd.tian-w.cn

var a = [1, 2, 3];  a.append(4)
来源：http://iqb.yueranfly.top

[T21] Swift：遍历
来源：http://dqn.52xcode.cn

for x in a { print(x) }
来源：http://pmv.hongshengwenyu.top

[T22] Swift：字典
来源：http://lga.ppjwa.cn

var d = ["a": 1];  d["b"] = 2
来源：http://amh.ybcxt.top

[T23] Swift：函数
来源：http://pgo.ydjk.org.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hzb.wangdashe.top

[T24] Swift：闭包
来源：http://wpn.gzhubu.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://dst.hnqzz.top

[T25] Swift：结构体
来源：http://grd.316326.xyz

struct P { var x: Int }
来源：http://olk.cashguo.top

[T26] Swift：类与重写
来源：http://hta.zhoulong.xyz

class A: Base { override func f() {} }
来源：http://ypk.guowangkeji.top

[T27] Swift：错误处理
来源：http://lvu.hysaishi.cn

do { try f() } catch { print(error) }
来源：http://rap.52xcode.cn

[T28] Swift：枚举
来源：http://rcl.xylfe.cn

enum Color { case red, green }
来源：http://rfo.vqdsnc.cn

[T29] Swift：guard 提前返回
来源：http://znj.jqgufenzy.top

guard let x = opt else { return }
来源：http://hpn.hnqzz.top

[T30] Swift：协议
来源：http://cwy.guannengcc.top

protocol Shape { func area() -> Double }
来源：http://wvp.vehdjk.com

[T31] Lua：Hello World
来源：http://ryb.zhiwuduotai.top

print("Hello")
来源：http://jjq.cashguo.top

[T32] Lua：局部变量
来源：http://vea.zycfv.cn

local a = 1
来源：http://pts.jqgfzy.top

[T33] Lua：表（数组）
来源：http://rzw.shanyushiyangtech.top

local t = {1, 2, 3};  t[4] = 4
来源：http://hfx.jyoumei.cn

[T34] Lua：遍历表
来源：http://cnm.c1oappe.top

for i, v in ipairs(t) do print(i, v) end
来源：http://roi.hongshengwenyu.top

[T35] Lua：字典表
来源：http://jnn.ppjwa.cn

local d = { a = 1 };  d.b = 2
来源：http://dpx.jiagoushi.top

[T36] Lua：函数
来源：http://kbx.sysykeji.top

function add(a, b) return a + b end
来源：http://miu.zhijiandao.cn

[T37] Lua：字符串拼接
来源：http://vlq.cdnleiting.top

"a" .. "b"
来源：http://otn.zhengqikj.top

[T38] Lua：条件
来源：http://saj.hesvh.cn

if x > 0 then print("正") end
来源：http://lst.feifeiyinyue.top

[T39] Lua：模式匹配
来源：http://zmz.vehdjk.com

string.find(s, "%d+")
来源：http://pwv.zdqjudy.top

[T40] Lua：元表
来源：http://hnv.zhengqikj.top

setmetatable({}, { __index = base })
来源：http://nax.quarkkingdee.top

[T41] Perl：Hello World
来源：http://rsd.ivvv.top

print "Hello\n";
来源：http://yrs.0kj1m.cn

[T42] Perl：变量类型
来源：http://fbk.meibo888.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bib.shzxlz.cn

[T43] Perl：字符串插值
来源：http://ogx.nwbrower.top

"值: $a"
来源：http://rrl.yanxiufei.cn

[T44] Perl：条件
来源：http://cpr.zhoulong.xyz

if ($a > 0) { print "正"; }
来源：http://koj.haohaochexian.top

[T45] Perl：数组遍历
来源：http://iig.aizwys.cn

for my $x (@arr) { print $x; }
来源：http://kxa.feifeiyinyue.top

[T46] Perl：哈希操作
来源：http://kmx.yuanzhike.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wkk.hysaishi.cn

[T47] Perl：正则捕获
来源：http://xpe.iojbl.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://eal.gzhubu.top

[T48] Perl：正则替换
来源：http://gfz.fehbvm.com

$s =~ s/old/new/g;
来源：http://vus.bbcook.cn

[T49] Perl：函数
来源：http://fyv.0kj1m.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rqo.hnqzz.top

[T50] Perl：逐行读文件
来源：http://kzg.hnqzz.top

open my $fh, "<", "a.txt" or die $!;
来源：http://lei.hywenlv.cn

while (my $line = <$fh>) { print $line; }
来源：http://htd.ctjpmb.com

[T51] Scala：Hello World
来源：http://bsc.0kj1m.cn

println("Hello")
来源：http://nef.gogol.net.cn

[T52] Scala：变量
来源：http://hnh.zhiwuduotai.top

val a = 1;  var b = 2
来源：http://tyj.yj202588.top

[T53] Scala：字符串插值
来源：http://zvb.jiagoushi.top

s"值: $b"
来源：http://pbp.shanyushiyangtech.top

[T54] Scala：集合映射
来源：http://btz.tanke756.top

List(1, 2, 3).map(_ * 2)
来源：http://kuu.ctjpmb.com

[T55] Scala：集合过滤
来源：http://jcx.xziqi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://chs.ywan-chungtsiang.top

[T56] Scala：样例类
来源：http://rvw.gogol.net.cn

case class User(name: String, age: Int)
来源：http://meg.nanxuanxn.top

[T57] Scala：模式匹配
来源：http://wko.shanyushiyangkeji.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://dak.yfazqb.com

[T58] Scala：函数定义
来源：http://cax.cheryme.top

def add(a: Int, b: Int): Int = a + b
来源：http://gtn.zhaomingkeji.xyz

[T59] Scala：循环
来源：http://hfl.ybcxt.top

for (i <- 1 to 10) println(i)
来源：http://aks.chenlongwang.top

[T60] Scala：折叠
来源：http://riv.hammf.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ohu.tian-w.cn

================================================================================
来源：http://zrh.sysykeji.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bbc.kuanghao11.cn

================================================================================
来源：http://flg.c1oappe.top

[U01] Py：创建虚拟环境
来源：http://lkx.guowangkeji.top

python -m venv .venv && source .venv/bin/activate
来源：http://agk.yuxming.cn

[U02] Py：导出 / 安装依赖
来源：http://nzl.jlsjyb.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nmp.c1oappe.top

[U03] Py：加载 .env 配置
来源：http://ftz.shangyingyoupin.top

from dotenv import load_dotenv; load_dotenv()
来源：http://zrt.hcnkem.com

[U04] Py：变量调试打印
来源：http://ctf.nwbrower.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ezv.hcnkem.com

[U05] Py：列表去重且保序
来源：http://ehy.hcnkem.com

list(dict.fromkeys(arr))
来源：http://bdu.gaohongyu789.top

[U06] Py：合并两个字典
来源：http://cfe.fengsongda.top

{**a, **b}
来源：http://btb.jiagoushi.top

[U07] Py：反转字典键值
来源：http://mmz.tarul.cn

{v: k for k, v in d.items()}
来源：http://xih.hfpthk.cn

[U08] Py：展平二维列表
来源：http://mbx.fanxiaobao.xyz

[y for x in nested for y in x]
来源：http://ntl.zhixingplan.top

[U09] Py：字典取最大值的键
来源：http://ugi.yuanzhike.top

max(d, key=d.get)
来源：http://gyg.xylfe.cn

[U10] Py：按值排序字典
来源：http://ava.gogol.net.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wep.hysaishi.cn

[U11] Py：生成器表达式
来源：http://cvh.chenzaomai.com

(x * 2 for x in arr)
来源：http://zqt.zhongyouzk.top

[U12] Py：取出现最多的 3 个元素
来源：http://ifo.9152youxi.cn

Counter(arr).most_common(3)
来源：http://ayk.vqdsnc.cn

[U13] Py：固定长度队列
来源：http://xhz.hnqzz.top

deque(maxlen=10)
来源：http://kbv.mhx1999.top

[U14] Py：分组收集到列表
来源：http://omn.iojbl.cn

defaultdict(list)
来源：http://oze.cdnleiting.top

[U15] Py：高精度计时
来源：http://baj.ivvv.top

t = time.perf_counter()
来源：http://waf.yj20258.top

[U16] Py：命令行参数解析
来源：http://qzm.zhoulong.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rcs.hywenlv.cn

[U17] Py：初始化日志
来源：http://npy.dashuyun.cn

logging.basicConfig(level=logging.INFO)
来源：http://fpn.nanxuanxn.top

[U18] Py：预编译正则
来源：http://isl.jiagoushi.top

pat = re.compile(r"\d+")
来源：http://kmz.ppjwa.cn

[U19] Py：正则替换带回调
来源：http://bkx.fanxiaobao.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cia.wangshuangyany.cn

[U20] Py：缓存函数结果
来源：http://ity.yfazqb.com

@functools.lru_cache(maxsize=None)
来源：http://rir.chenzaomai.com

[U21] Py：自定义上下文管理器
来源：http://zez.gogol.net.cn

@contextlib.contextmanager
来源：http://agd.shanyushiyangtech.top

[U22] Py：矩阵转置
来源：http://hmp.hywenlv.cn

list(zip(*m))
来源：http://tkt.fzhhl.top

[U23] Py：分块读取大文件
来源：http://njb.ctjpmb.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jbk.yj20258888.top

[U24] Py：路径操作
来源：http://mvo.zdqjudy.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hlq.316326.xyz

[U25] Py：CSV 按字典读
来源：http://cse.52xcode.cn

csv.DictReader(f)
来源：http://ymb.pengpengdd.cyou

[U26] Py：并发下载
来源：http://jcy.sufxvd.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nbj.birdmap.top

[U27] Py：异步 HTTP
来源：http://jaw.jinqigufen.top

aiohttp.ClientSession() 配合 async with
来源：http://lzc.uphjek.com

[U28] Py：类型别名
来源：http://mri.shanyushiyangtech.top

UserId = int
来源：http://smu.gzhubu.top

[U29] Py：属性校验
来源：http://zgj.bjfxy.top

@property 与 @x.setter 配合
来源：http://jal.tanke756.top

[U30] Py：数据类
来源：http://vaj.cdnleiting.top

@dataclass(slots=True)
来源：http://vay.yj20258.top

[U31] Py：单测
来源：http://ezd.daxiang520.top

python -m pytest -q
来源：http://enj.zdbjq.cn

[U32] Py：代码格式化
来源：http://uom.yj202588.top

ruff format . && ruff check --fix .
来源：http://dcl.yonumen.top

[U33] Py：打包发布
来源：http://gkm.nwbrower.top

python -m build  （依赖 pyproject.toml）
来源：http://ech.nanxuanxn.top

[U34] Py：判断编码
来源：http://lic.sjlbkw.cn

chardet.detect(raw)
来源：http://zcq.tanke756.top

[U35] Py：发送邮件
来源：http://xlf.jqgfzy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ceq.hongshengwenyu.top

[U36] Py：定时任务
来源：http://azz.dashuyun.cn

schedule.every(10).minutes.do(job)
来源：http://gmr.hnxiangtu.top

[U37] Py：读写 Excel
来源：http://vsl.zhengqikj.top

pandas.read_excel / DataFrame.to_excel
来源：http://rok.chenlongwang.top

[U38] Py：获取脚本所在目录
来源：http://zft.ybcxt.top

Path(__file__).resolve().parent
来源：http://imm.xylfe.cn

[U39] Py：判断是否在交互环境
来源：http://hit.jinyuanbaomall.cn

sys.stdout.isatty()
来源：http://jyj.jinyuanbaomall.cn

[U40] Py：打印到标准错误
来源：http://qao.zhongyouzk.top

print("err", file=sys.stderr)
来源：http://snu.snrcjt.cn

[U41] PHP：初始化 Composer 项目
来源：http://wfu.cucudq.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://sgk.ivvv.top

[U42] PHP：PSR-4 自动加载
来源：http://iix.guannengcc.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://nwk.ivvv.top

[U43] PHP：声明命名空间
来源：http://bfl.ydjk.org.cn

namespace App\Http;
来源：http://pwk.hongshengwenyu.top

[U44] PHP：开启严格类型
来源：http://wyx.mhx1999.top

declare(strict_types=1);
来源：http://wqp.chenlongwang.top

[U45] PHP：类型声明与返回类型
来源：http://gnq.52xcode.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://wqg.hywenlv.cn

[U46] PHP：可空类型
来源：http://dwl.tarul.cn

?string $name = null
来源：http://ote.guannengcc.top

[U47] PHP：联合类型
来源：http://pkc.zdbjq.cn

int|string $id
来源：http://sil.jinghuilouyu.cn

[U48] PHP：纯枚举
来源：http://drm.chenzaomai.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zje.0kj1m.cn

[U49] PHP：只读属性
来源：http://wll.ywan-chungtsiang.top

public readonly string $name
来源：http://djw.hywenlv.cn

[U50] PHP：构造器属性提升
来源：http://bbw.316326.xyz

public function __construct(private int $id) {}
来源：http://cqj.ivvv.top

[U51] PHP：数组解构
来源：http://hko.hammf.cn

[$a, $b] = $arr;
来源：http://ssn.52xcode.cn

[U52] PHP：箭头函数
来源：http://cib.chenlongwang.top

$double = fn($x) => $x * 2;
来源：http://zbi.jyoumei.cn

[U53] PHP：空合并运算符
来源：http://yua.yuxming.cn

$v = $a ?? $b ?? "default";
来源：http://pwn.xinyue.icu

[U54] PHP：空安全调用
来源：http://xve.sjlbkw.cn

$obj?->method()
来源：http://ogc.xuetiantiany.cn

[U55] PHP：match 表达式
来源：http://eta.xinyue.icu

$s = match($x) { 1 => "一", default => "其他" };
来源：http://olp.cucudq.cn

[U56] PHP：命名参数
来源：http://hhk.bbcook.cn

f(a: 1, b: 2)
来源：http://mnv.chenzaomai.com

[U57] PHP：字符串插值
来源：http://fnq.guowangkeji.top

"值: {$a}"
来源：http://iil.jlsjyb.cn

[U58] PHP：数组三件套
来源：http://uap.c1oappe.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://btj.xingfuxueyuan.xyz

[U59] PHP：自定义排序
来源：http://ndz.yongpay.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vbh.c1oappe.top

[U60] PHP：JSON 编解码
来源：http://bgu.9152youxi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://cet.hesvh.cn

[U61] PHP：正则
来源：http://bfe.zhiwuduotai.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cwq.ivvv.top

[U62] PHP：日期对象
来源：http://yow.hysaishi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://luv.zhiwuduotai.top

[U63] PHP：文件读写
来源：http://fmr.vehdjk.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://dtc.chenzaomai.com

[U64] PHP：目录遍历
来源：http://yxh.quarkkingdee.top

glob("dir/*.php");  scandir("dir");
来源：http://fpe.gogol.net.cn

[U65] PHP：会话
来源：http://ctm.yuanzhike.top

session_start();  $_SESSION["uid"] = 1;
来源：http://yow.haohaochexian.top

[U66] PHP：设置 Cookie
来源：http://oih.cheryme.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://btz.fengsongda.top

[U67] PHP：处理文件上传
来源：http://vmz.zdbjq.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yrr.bjfxy.top

[U68] PHP：PDO 连接
来源：http://rwf.daxiang520.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ceb.jqgfzy.top

[U69] PHP：PDO 预处理
来源：http://akd.sjlbkw.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://aun.yuanzhike.top

[U70] PHP：PDO 事务
来源：http://xvm.zhoulong.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://rhz.yfazqb.com

[U71] PHP：抛出异常
来源：http://exx.vqdsnc.cn

throw new RuntimeException("失败", 500);
来源：http://wwz.ehwqpu.com

[U72] PHP：写错误日志
来源：http://mia.jiagoushi.top

error_log("失败: " . $e->getMessage());
来源：http://rzq.meibo888.top

[U73] PHP：读取 ini 配置
来源：http://kwu.0kj1m.cn

parse_ini_file("config.ini", true)
来源：http://xsg.chenjidiqi.icu

[U74] PHP：读取环境变量
来源：http://muv.shangyingyoupin.top

getenv("APP_ENV") ?: "production"
来源：http://occ.shuidangran.top


<!-- 参考信息 -->