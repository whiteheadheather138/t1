代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xns.snrcjt.cn

[S51] C++：显式类型转换
来源：http://bhj.chenjidiqi.icu

static_cast<double>(a) / b
来源：http://cjf.jiagoushi.top

[S52] C++：const 与 noexcept
来源：http://bgk.hnqzz.top

int size() const noexcept { return n_; }
来源：http://kat.yonumen.top

[S53] C++：移动语义
来源：http://msw.jqgfzy.top

std::vector<int> w = std::move(v);
来源：http://cwj.316326.xyz

[S54] C++：异常处理
来源：http://zfy.cashguo.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rkv.yuxming.cn

[S55] C++：结构化绑定
来源：http://dlb.316326.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://mip.yj20258.top

[S56] C++：optional
来源：http://wgn.xylfe.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://won.kuanghao11.cn

[S57] C++：编译期常量
来源：http://kpv.fzhhl.top

constexpr int N = 10;
来源：http://jjo.hesvh.cn

[S58] C++：命名空间
来源：http://wle.shanyushiyangkeji.top

namespace ns { int f() { return 1; } }
来源：http://lel.quarkkingdee.top

[S59] C++：静态断言
来源：http://fwm.sweek.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rkr.fengsongda.top

[S60] C++：遍历并删除元素
来源：http://kza.chenzaomai.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rog.yongpay.top

================================================================================
来源：http://rib.zycfv.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ybd.dianchejie.cn

================================================================================
来源：http://bue.hcnkem.com

[T01] Kotlin：Hello World
来源：http://veo.hysaishi.cn

println("Hello")
来源：http://yxd.xylfe.cn

[T02] Kotlin：变量
来源：http://rlu.zhengqikj.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vzb.guannengcc.top

[T03] Kotlin：字符串模板
来源：http://jub.0kj1m.cn

"值: $b"
来源：http://ccb.sxryk.cn

[T04] Kotlin：空安全
来源：http://wwb.xuanzx.com

val n: String? = null;  n?.length
来源：http://boo.yonumen.top

[T05] Kotlin：when 表达式
来源：http://wrk.316326.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ors.mhx1999.top

[T06] Kotlin：集合映射
来源：http://ixx.gotoacloud.top

listOf(1, 2, 3).map { it * 2 }
来源：http://qmy.wangshuangyany.cn

[T07] Kotlin：集合过滤
来源：http://dbw.0kj1m.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ghs.uphjek.com

[T08] Kotlin：数据类
来源：http://ftk.sysykeji.top

data class User(val name: String, val age: Int)
来源：http://fef.hcnkem.com

[T09] Kotlin：扩展函数
来源：http://btx.birdmap.top

fun String.exclaim() = this + "!"
来源：http://shz.chenzaomai.com

[T10] Kotlin：默认参数
来源：http://nvs.xuanzx.com

fun greet(name: String = "World") = "Hi $name"
来源：http://kje.bjfxy.top

[T11] Kotlin：协程
来源：http://fhh.havefunace.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://utc.birdmap.top

[T12] Kotlin：解构声明
来源：http://mka.shuidangran.top

val (a, b) = Pair(1, 2)
来源：http://ynv.fanxiaobao.xyz

[T13] Kotlin：只读 Map
来源：http://nwi.yonumen.top

val m = mapOf("a" to 1)
来源：http://pax.birdmap.top

[T14] Kotlin：循环
来源：http://bpk.bbcook.cn

for (i in 1..10) println(i)
来源：http://uib.yfazqb.com

[T15] Kotlin：接口
来源：http://xgg.yueranfly.top

interface Shape { fun area(): Double }
来源：http://zdu.9152youxi.cn

[T16] Swift：Hello World
来源：http://ssq.tanke756.top

print("Hello")
来源：http://bpp.uphjek.com

[T17] Swift：变量与常量
来源：http://nho.hesvh.cn

var a = 1;  let b = 2
来源：http://oci.ydjk.org.cn

[T18] Swift：字符串插值
来源：http://ehd.ywan-chungtsiang.top

"值: \(b)"
来源：http://kwf.fengsongda.top

[T19] Swift：可选绑定
来源：http://hcj.yj20258888.top

if let n = opt { print(n) }
来源：http://kmv.yueranfly.top

[T20] Swift：数组操作
来源：http://vhb.cashguo.top

var a = [1, 2, 3];  a.append(4)
来源：http://tqg.yueranfly.top

[T21] Swift：遍历
来源：http://utv.52xcode.cn

for x in a { print(x) }
来源：http://bfj.meibo888.top

[T22] Swift：字典
来源：http://njk.yongpay.top

var d = ["a": 1];  d["b"] = 2
来源：http://cyt.kuanghao11.cn

[T23] Swift：函数
来源：http://qyf.hammf.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://izk.cashguo.top

[T24] Swift：闭包
来源：http://nrq.daria6918.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vhz.hysaishi.cn

[T25] Swift：结构体
来源：http://vlx.jinqigufen.top

struct P { var x: Int }
来源：http://mhr.cashguo.top

[T26] Swift：类与重写
来源：http://bfr.nwbrower.top

class A: Base { override func f() {} }
来源：http://vdi.yangfankeji.com

[T27] Swift：错误处理
来源：http://etp.hfpthk.cn

do { try f() } catch { print(error) }
来源：http://vmh.shanyushiyangkeji.top

[T28] Swift：枚举
来源：http://zur.zycfv.cn

enum Color { case red, green }
来源：http://vbg.quarkkingdee.top

[T29] Swift：guard 提前返回
来源：http://rbp.quarkkingdee.top

guard let x = opt else { return }
来源：http://los.wangshuangyany.cn

[T30] Swift：协议
来源：http://ken.xuetiantiany.cn

protocol Shape { func area() -> Double }
来源：http://wqy.bjfxy.top

[T31] Lua：Hello World
来源：http://wsy.nwbrower.top

print("Hello")
来源：http://bxk.uphjek.com

[T32] Lua：局部变量
来源：http://leb.daria6918.cn

local a = 1
来源：http://dwp.ctjpmb.com

[T33] Lua：表（数组）
来源：http://czb.mhx1999.top

local t = {1, 2, 3};  t[4] = 4
来源：http://hns.xziqi.cn

[T34] Lua：遍历表
来源：http://udf.jlsjyb.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://dan.wangdashe.top

[T35] Lua：字典表
来源：http://bui.ppjwa.cn

local d = { a = 1 };  d.b = 2
来源：http://onb.yueranfly.top

[T36] Lua：函数
来源：http://msf.birdmap.top

function add(a, b) return a + b end
来源：http://zyi.zdbjq.cn

[T37] Lua：字符串拼接
来源：http://gfx.smart0.xyz

"a" .. "b"
来源：http://yju.shanyushiyangkeji.top

[T38] Lua：条件
来源：http://htv.fktsv.cn

if x > 0 then print("正") end
来源：http://yzn.pengpengdd.cyou

[T39] Lua：模式匹配
来源：http://zoq.wangdashe.top

string.find(s, "%d+")
来源：http://kus.jinqigufen.top

[T40] Lua：元表
来源：http://tsq.vqdsnc.cn

setmetatable({}, { __index = base })
来源：http://luj.xuetiantiany.cn

[T41] Perl：Hello World
来源：http://ehz.pengpengdd.cyou

print "Hello\n";
来源：http://bsd.kuanghao11.cn

[T42] Perl：变量类型
来源：http://ahs.kuanghao11.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tau.iojbl.cn

[T43] Perl：字符串插值
来源：http://saz.jinyuanbaomall.cn

"值: $a"
来源：http://bbz.jinqigfzy.top

[T44] Perl：条件
来源：http://htq.ybcxt.top

if ($a > 0) { print "正"; }
来源：http://kai.mhx1999.top

[T45] Perl：数组遍历
来源：http://cbz.andypj.xyz

for my $x (@arr) { print $x; }
来源：http://ggx.hammf.cn

[T46] Perl：哈希操作
来源：http://kvd.daria6918.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rvu.cashguo.top

[T47] Perl：正则捕获
来源：http://ycz.dianchejie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://kjt.hysaishi.cn

[T48] Perl：正则替换
来源：http://anu.epnwcf.com

$s =~ s/old/new/g;
来源：http://gbk.chenzaomai.com

[T49] Perl：函数
来源：http://kth.iojbl.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vje.cdnleiting.top

[T50] Perl：逐行读文件
来源：http://tsd.fktsv.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://cyu.pycfn.com

while (my $line = <$fh>) { print $line; }
来源：http://lwh.aibaodan.cn

[T51] Scala：Hello World
来源：http://goi.guannengcc.top

println("Hello")
来源：http://ism.shangyingyoupin.top

[T52] Scala：变量
来源：http://yzd.yj20258888.top

val a = 1;  var b = 2
来源：http://hxo.yj20258.top

[T53] Scala：字符串插值
来源：http://ope.c1oappe.top

s"值: $b"
来源：http://oiq.yueranfly.top

[T54] Scala：集合映射
来源：http://vfm.shanyushiyangkeji.top

List(1, 2, 3).map(_ * 2)
来源：http://wjz.sxryk.cn

[T55] Scala：集合过滤
来源：http://flw.yanxiufei.cn

List(1, 2, 3).filter(_ > 1)
来源：http://lzf.hnxiangtu.top

[T56] Scala：样例类
来源：http://upg.shuidangran.top

case class User(name: String, age: Int)
来源：http://oqu.shuidangran.top

[T57] Scala：模式匹配
来源：http://xqs.fanxiaobao.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://lqf.yuanzhike.top

[T58] Scala：函数定义
来源：http://fmd.dashuyun.cn

def add(a: Int, b: Int): Int = a + b
来源：http://agk.gotoacloud.top

[T59] Scala：循环
来源：http://rof.sysykeji.top

for (i <- 1 to 10) println(i)
来源：http://qiz.nwbrower.top

[T60] Scala：折叠
来源：http://pjw.yuanzhike.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bye.quarkkingdee.top

================================================================================
来源：http://gzf.ydjk.org.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://amu.yj202588.top

================================================================================
来源：http://pbn.guowangkeji.top

[U01] Py：创建虚拟环境
来源：http://lgu.bbcook.cn

python -m venv .venv && source .venv/bin/activate
来源：http://dsl.zhaomingkeji.xyz

[U02] Py：导出 / 安装依赖
来源：http://qrj.fengsongda.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nog.shanyushiyangkeji.top

[U03] Py：加载 .env 配置
来源：http://czr.gotoacloud.top

from dotenv import load_dotenv; load_dotenv()
来源：http://cst.wangshuangyany.cn

[U04] Py：变量调试打印
来源：http://ith.pycfn.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zpy.ydzc1.top

[U05] Py：列表去重且保序
来源：http://zuq.ivvv.top

list(dict.fromkeys(arr))
来源：http://eys.chenlongwang.top

[U06] Py：合并两个字典
来源：http://wvh.nwbrower.top

{**a, **b}
来源：http://taz.jyoumei.cn

[U07] Py：反转字典键值
来源：http://afx.fanxiaobao.xyz

{v: k for k, v in d.items()}
来源：http://urg.sjlbkw.cn

[U08] Py：展平二维列表
来源：http://gas.hysaishi.cn

[y for x in nested for y in x]
来源：http://eag.ehwqpu.com

[U09] Py：字典取最大值的键
来源：http://mdv.guowangkeji.top

max(d, key=d.get)
来源：http://hwm.cdnleiting.top

[U10] Py：按值排序字典
来源：http://vim.quarkkingdee.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ckz.jinqigfzy.top

[U11] Py：生成器表达式
来源：http://ssu.snrcjt.cn

(x * 2 for x in arr)
来源：http://tvr.gaohongyu789.top

[U12] Py：取出现最多的 3 个元素
来源：http://zly.ppjwa.cn

Counter(arr).most_common(3)
来源：http://vac.shanyushiyangkeji.top

[U13] Py：固定长度队列
来源：http://gla.bjfxy.top

deque(maxlen=10)
来源：http://sbh.zhengqikj.top

[U14] Py：分组收集到列表
来源：http://tox.svipenyu.cn

defaultdict(list)
来源：http://dyx.dashuyun.cn

[U15] Py：高精度计时
来源：http://cgy.yanxiufei.cn

t = time.perf_counter()
来源：http://juf.aizwys.cn

[U16] Py：命令行参数解析
来源：http://alr.yonumen.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://egk.jqgufenzy.top

[U17] Py：初始化日志
来源：http://dib.jlsjyb.cn

logging.basicConfig(level=logging.INFO)
来源：http://yqn.yuxming.cn

[U18] Py：预编译正则
来源：http://vql.sufxvd.cn

pat = re.compile(r"\d+")
来源：http://sjl.zhaomingkeji.xyz

[U19] Py：正则替换带回调
来源：http://gcw.fengsongda.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://pfz.aibaodan.cn

[U20] Py：缓存函数结果
来源：http://bqd.ybcxt.top

@functools.lru_cache(maxsize=None)
来源：http://itu.sjlbkw.cn

[U21] Py：自定义上下文管理器
来源：http://yuf.guowangkeji.top

@contextlib.contextmanager
来源：http://pnr.jinyuanbaomall.cn

[U22] Py：矩阵转置
来源：http://qnk.sweek.top

list(zip(*m))
来源：http://jyd.snrcjt.cn

[U23] Py：分块读取大文件
来源：http://xrc.gzhubu.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jwh.cucudq.cn

[U24] Py：路径操作
来源：http://gef.shanyushiyangtech.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://dyk.hysaishi.cn

[U25] Py：CSV 按字典读
来源：http://fta.xylfe.cn

csv.DictReader(f)
来源：http://ptp.ehwqpu.com

[U26] Py：并发下载
来源：http://ses.cqqwz.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bbn.sjlbkw.cn

[U27] Py：异步 HTTP
来源：http://ldq.chenjidiqi.icu

aiohttp.ClientSession() 配合 async with
来源：http://puo.sjlbkw.cn

[U28] Py：类型别名
来源：http://cqv.ydjk.org.cn

UserId = int
来源：http://tdj.sxryk.cn

[U29] Py：属性校验
来源：http://uwb.hongshengwenyu.top

@property 与 @x.setter 配合
来源：http://vmc.shuidangran.top

[U30] Py：数据类
来源：http://vly.chenjidiqi.icu

@dataclass(slots=True)
来源：http://ksw.yonumen.top

[U31] Py：单测
来源：http://zyo.hnxiangtu.top

python -m pytest -q
来源：http://jhl.bbcook.cn

[U32] Py：代码格式化
来源：http://mlr.sxryk.cn

ruff format . && ruff check --fix .
来源：http://ttg.ydjk.org.cn

[U33] Py：打包发布
来源：http://jmc.yj202588.top

python -m build  （依赖 pyproject.toml）
来源：http://rkk.yuxming.cn

[U34] Py：判断编码
来源：http://klu.jinqigufen.top

chardet.detect(raw)
来源：http://pps.bjfxy.top

[U35] Py：发送邮件
来源：http://yyx.cashguo.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tqp.hcnkem.com

[U36] Py：定时任务
来源：http://nif.yongpay.top

schedule.every(10).minutes.do(job)
来源：http://erq.vqdsnc.cn

[U37] Py：读写 Excel
来源：http://eqn.52xcode.cn

pandas.read_excel / DataFrame.to_excel
来源：http://orf.yueranfly.top

[U38] Py：获取脚本所在目录
来源：http://pqo.shanyushiyangtech.top

Path(__file__).resolve().parent
来源：http://mdq.xziqi.cn

[U39] Py：判断是否在交互环境
来源：http://pae.jinqigufen.top

sys.stdout.isatty()
来源：http://gwe.havefunace.top

[U40] Py：打印到标准错误
来源：http://itp.hnxiangtu.top

print("err", file=sys.stderr)
来源：http://ohl.sweek.top

[U41] PHP：初始化 Composer 项目
来源：http://chb.daxiang520.top

composer init;  composer require guzzlehttp/guzzle
来源：http://qlx.havefunace.top

[U42] PHP：PSR-4 自动加载
来源：http://eey.yfazqb.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://oil.zdbjq.cn

[U43] PHP：声明命名空间
来源：http://nov.gogol.net.cn

namespace App\Http;
来源：http://nuk.zhoulong.xyz

[U44] PHP：开启严格类型
来源：http://qqw.svipenyu.cn

declare(strict_types=1);
来源：http://feo.cashguo.top

[U45] PHP：类型声明与返回类型
来源：http://ole.yvedp.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://lyb.dianchejie.cn

[U46] PHP：可空类型
来源：http://cok.svipenyu.cn

?string $name = null
来源：http://emk.zhongyouzk.top

[U47] PHP：联合类型
来源：http://ltl.gaohongyu789.top

int|string $id
来源：http://wvs.ydzc1.top

[U48] PHP：纯枚举
来源：http://vrp.fzhhl.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mzb.jinghuilouyu.cn

[U49] PHP：只读属性
来源：http://rrn.sufxvd.cn

public readonly string $name
来源：http://tze.ctjpmb.com

[U50] PHP：构造器属性提升
来源：http://gqm.tanke756.top

public function __construct(private int $id) {}
来源：http://msh.zhongyouzk.top

[U51] PHP：数组解构
来源：http://efs.zhaomingkeji.xyz

[$a, $b] = $arr;
来源：http://xvb.ybcxt.top

[U52] PHP：箭头函数
来源：http://pdr.bjfxy.top

$double = fn($x) => $x * 2;
来源：http://bzh.ybcxt.top

[U53] PHP：空合并运算符
来源：http://yuz.fanxiaobao.xyz

$v = $a ?? $b ?? "default";
来源：http://hct.shanyushiyangkeji.top

[U54] PHP：空安全调用
来源：http://kbg.gogol.net.cn

$obj?->method()
来源：http://kpl.mhx1999.top

[U55] PHP：match 表达式
来源：http://uti.shzxlz.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://sca.0kj1m.cn

[U56] PHP：命名参数
来源：http://pag.jianghu66.top

f(a: 1, b: 2)
来源：http://rqv.bjfxy.top

[U57] PHP：字符串插值
来源：http://gpo.ctjpmb.com

"值: {$a}"
来源：http://mao.tian-w.cn

[U58] PHP：数组三件套
来源：http://bra.tianlin.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wdp.jinyuanbaomall.cn

[U59] PHP：自定义排序
来源：http://snv.zdbjq.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://xfo.pengpengdd.cyou

[U60] PHP：JSON 编解码
来源：http://krz.yongpay.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://eyn.ppjwa.cn

[U61] PHP：正则
来源：http://yky.meibo888.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://nov.fzhhl.top

[U62] PHP：日期对象
来源：http://ozi.havefunace.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://vgf.hysaishi.cn

[U63] PHP：文件读写
来源：http://bdp.xuanzx.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://aem.aibaodan.cn

[U64] PHP：目录遍历
来源：http://jls.yuanzhike.top

glob("dir/*.php");  scandir("dir");
来源：http://pvq.cqqwz.cn

[U65] PHP：会话
来源：http://skr.tian-w.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://fdr.vehdjk.com

[U66] PHP：设置 Cookie
来源：http://vlg.pycfn.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ilg.fengsongda.top

[U67] PHP：处理文件上传
来源：http://xvi.birdmap.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mnv.yueranfly.top

[U68] PHP：PDO 连接
来源：http://upd.nanxuanxn.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://chd.birdmap.top

[U69] PHP：PDO 预处理
来源：http://gyx.yj20258.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zjr.kuanghao11.cn

[U70] PHP：PDO 事务
来源：http://cjp.mhx1999.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ayp.fengsongda.top

[U71] PHP：抛出异常
来源：http://hnz.chenzaomai.com

throw new RuntimeException("失败", 500);
来源：http://jou.nanxuanxn.top

[U72] PHP：写错误日志
来源：http://ueq.haohaochexian.top

error_log("失败: " . $e->getMessage());
来源：http://wak.c1oappe.top

[U73] PHP：读取 ini 配置
来源：http://cml.pycfn.com

parse_ini_file("config.ini", true)
来源：http://omk.zhixingplan.top

[U74] PHP：读取环境变量
来源：http://gzq.chenlongwang.top

getenv("APP_ENV") ?: "production"
来源：http://vmr.tian-w.cn

[U75] PHP：依赖注入
来源：http://bym.dianchejie.cn

composer require psr/container
来源：http://upm.316326.xyz

[U76] PHP：简单路由
来源：http://hsw.jlsjyb.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ibh.nwbrower.top


<!-- 参考信息 -->