代发 wailian999

int size() const noexcept { return n_; }
来源：http://rdm.jqgufenzy.top

[S53] C++：移动语义
来源：http://qml.xuetiantiany.cn

std::vector<int> w = std::move(v);
来源：http://qhq.yangfankeji.com

[S54] C++：异常处理
来源：http://cwo.sysykeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://enq.yongpay.top

[S55] C++：结构化绑定
来源：http://frw.svipenyu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://yhh.fengsongda.top

[S56] C++：optional
来源：http://air.yj20258888.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gbo.birdmap.top

[S57] C++：编译期常量
来源：http://wfi.yj20258888.top

constexpr int N = 10;
来源：http://vak.pengpengdd.cyou

[S58] C++：命名空间
来源：http://imy.redwolf501.top

namespace ns { int f() { return 1; } }
来源：http://xzx.hongshengwenyu.top

[S59] C++：静态断言
来源：http://ujt.hfpthk.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lxd.gzhubu.top

[S60] C++：遍历并删除元素
来源：http://ili.yj20258.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yja.tianlin.xyz

================================================================================
来源：http://nrv.ppjwa.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://awq.zdqjudy.top

================================================================================
来源：http://zhr.dashuyun.cn

[T01] Kotlin：Hello World
来源：http://cqh.jinqigfzy.top

println("Hello")
来源：http://evk.feifeiyinyue.top

[T02] Kotlin：变量
来源：http://jcd.hfpthk.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://omd.yvedp.cn

[T03] Kotlin：字符串模板
来源：http://wll.yuxming.cn

"值: $b"
来源：http://ttb.xingfuxueyuan.xyz

[T04] Kotlin：空安全
来源：http://ots.quarkkingdee.top

val n: String? = null;  n?.length
来源：http://vtv.c1oappe.top

[T05] Kotlin：when 表达式
来源：http://lqb.tian-w.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jwg.ybcxt.top

[T06] Kotlin：集合映射
来源：http://afw.hnqzz.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ecj.zhoulong.xyz

[T07] Kotlin：集合过滤
来源：http://gie.epnwcf.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://bkr.yj20258.top

[T08] Kotlin：数据类
来源：http://syy.daria6918.cn

data class User(val name: String, val age: Int)
来源：http://cti.chenzaomai.com

[T09] Kotlin：扩展函数
来源：http://mfr.xylfe.cn

fun String.exclaim() = this + "!"
来源：http://uzv.yvedp.cn

[T10] Kotlin：默认参数
来源：http://oxu.andypj.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://lzf.chenjidiqi.icu

[T11] Kotlin：协程
来源：http://awm.jqgufenzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://mlo.zhaomingkeji.xyz

[T12] Kotlin：解构声明
来源：http://gmh.svipenyu.cn

val (a, b) = Pair(1, 2)
来源：http://anr.jqgfzy.top

[T13] Kotlin：只读 Map
来源：http://pux.sjlbkw.cn

val m = mapOf("a" to 1)
来源：http://idc.hywenlv.cn

[T14] Kotlin：循环
来源：http://wpm.52xcode.cn

for (i in 1..10) println(i)
来源：http://fat.guowangkeji.top

[T15] Kotlin：接口
来源：http://mqc.xinyue.icu

interface Shape { fun area(): Double }
来源：http://fcd.quarkkingdee.top

[T16] Swift：Hello World
来源：http://crd.yongpay.top

print("Hello")
来源：http://mhx.chenjidiqi.icu

[T17] Swift：变量与常量
来源：http://rgo.wangshuangyany.cn

var a = 1;  let b = 2
来源：http://gaz.gotoacloud.top

[T18] Swift：字符串插值
来源：http://eww.guowangkeji.top

"值: \(b)"
来源：http://dub.ydjk.org.cn

[T19] Swift：可选绑定
来源：http://vvk.sufxvd.cn

if let n = opt { print(n) }
来源：http://ukn.xuetiantiany.cn

[T20] Swift：数组操作
来源：http://ala.kuanghao11.cn

var a = [1, 2, 3];  a.append(4)
来源：http://srl.zhixingplan.top

[T21] Swift：遍历
来源：http://buz.zycfv.cn

for x in a { print(x) }
来源：http://jok.bjfxy.top

[T22] Swift：字典
来源：http://nxr.tanke756.top

var d = ["a": 1];  d["b"] = 2
来源：http://cgv.uphjek.com

[T23] Swift：函数
来源：http://jjt.cashguo.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://raa.jinqigufen.top

[T24] Swift：闭包
来源：http://xpa.yvedp.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://kee.zhaomingkeji.xyz

[T25] Swift：结构体
来源：http://aea.tian-w.cn

struct P { var x: Int }
来源：http://xtd.zdqjudy.top

[T26] Swift：类与重写
来源：http://iuz.shuidangran.top

class A: Base { override func f() {} }
来源：http://xdc.yj20258888.top

[T27] Swift：错误处理
来源：http://not.316326.xyz

do { try f() } catch { print(error) }
来源：http://rml.yuanzhike.top

[T28] Swift：枚举
来源：http://szv.iojbl.cn

enum Color { case red, green }
来源：http://hlo.shanyushiyangkeji.top

[T29] Swift：guard 提前返回
来源：http://ifx.vehdjk.com

guard let x = opt else { return }
来源：http://vfm.zhijiandao.cn

[T30] Swift：协议
来源：http://yrp.zhoulong.xyz

protocol Shape { func area() -> Double }
来源：http://gnx.sxryk.cn

[T31] Lua：Hello World
来源：http://hmn.andypj.xyz

print("Hello")
来源：http://abx.dianchejie.cn

[T32] Lua：局部变量
来源：http://crq.aizwys.cn

local a = 1
来源：http://puy.xinyue.icu

[T33] Lua：表（数组）
来源：http://uip.9152youxi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xuw.haohaochexian.top

[T34] Lua：遍历表
来源：http://vzv.dianchejie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rwz.c1oappe.top

[T35] Lua：字典表
来源：http://vks.hnxiangtu.top

local d = { a = 1 };  d.b = 2
来源：http://wpl.bbcook.cn

[T36] Lua：函数
来源：http://gkp.zhiwuduotai.top

function add(a, b) return a + b end
来源：http://imr.daxiang520.top

[T37] Lua：字符串拼接
来源：http://uke.nwbrower.top

"a" .. "b"
来源：http://iwj.ppjwa.cn

[T38] Lua：条件
来源：http://fli.316326.xyz

if x > 0 then print("正") end
来源：http://ntl.gogol.net.cn

[T39] Lua：模式匹配
来源：http://ufp.hnqzz.top

string.find(s, "%d+")
来源：http://kwq.chenjidiqi.icu

[T40] Lua：元表
来源：http://vsv.shanyushiyangtech.top

setmetatable({}, { __index = base })
来源：http://rwm.cqqwz.cn

[T41] Perl：Hello World
来源：http://hmr.zhijiandao.cn

print "Hello\n";
来源：http://xfk.xuetiantiany.cn

[T42] Perl：变量类型
来源：http://wxd.snrcjt.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rgw.cheryme.top

[T43] Perl：字符串插值
来源：http://ogz.yfazqb.com

"值: $a"
来源：http://bmx.yj202588.top

[T44] Perl：条件
来源：http://rtc.guowangkeji.top

if ($a > 0) { print "正"; }
来源：http://zst.jianghu66.top

[T45] Perl：数组遍历
来源：http://iau.yj20258888.top

for my $x (@arr) { print $x; }
来源：http://jom.yonumen.top

[T46] Perl：哈希操作
来源：http://ahd.zhengqikj.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ebd.haohaochexian.top

[T47] Perl：正则捕获
来源：http://xye.guannengcc.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://yok.hysaishi.cn

[T48] Perl：正则替换
来源：http://csw.ydjk.org.cn

$s =~ s/old/new/g;
来源：http://aqc.ppjwa.cn

[T49] Perl：函数
来源：http://lbn.gotoacloud.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://svs.daria6918.cn

[T50] Perl：逐行读文件
来源：http://pdu.nanxuanxn.top

open my $fh, "<", "a.txt" or die $!;
来源：http://dro.bjfxy.top

while (my $line = <$fh>) { print $line; }
来源：http://jbx.nanxinkj.top

[T51] Scala：Hello World
来源：http://jnv.shangyingyoupin.top

println("Hello")
来源：http://ynx.hywenlv.cn

[T52] Scala：变量
来源：http://rwa.hnxiangtu.top

val a = 1;  var b = 2
来源：http://tyd.ppjwa.cn

[T53] Scala：字符串插值
来源：http://mrt.xinyue.icu

s"值: $b"
来源：http://jft.zhoulong.xyz

[T54] Scala：集合映射
来源：http://ham.haohaochexian.top

List(1, 2, 3).map(_ * 2)
来源：http://xma.yvedp.cn

[T55] Scala：集合过滤
来源：http://bdx.pycfn.com

List(1, 2, 3).filter(_ > 1)
来源：http://alx.xuetiantiany.cn

[T56] Scala：样例类
来源：http://pwx.vehdjk.com

case class User(name: String, age: Int)
来源：http://ypb.hywenlv.cn

[T57] Scala：模式匹配
来源：http://oqi.snrcjt.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://yfx.nwbrower.top

[T58] Scala：函数定义
来源：http://uva.zdbjq.cn

def add(a: Int, b: Int): Int = a + b
来源：http://tdt.svipenyu.cn

[T59] Scala：循环
来源：http://dlf.jqgfzy.top

for (i <- 1 to 10) println(i)
来源：http://ffg.c1oappe.top

[T60] Scala：折叠
来源：http://vmn.zhiwuduotai.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://iqo.feifeiyinyue.top

================================================================================
来源：http://edz.haohaochexian.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://woz.sufxvd.cn

================================================================================
来源：http://vbv.fehbvm.com

[U01] Py：创建虚拟环境
来源：http://zhf.9152youxi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://lvs.zdqjudy.top

[U02] Py：导出 / 安装依赖
来源：http://efb.yfazqb.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://txe.ivvv.top

[U03] Py：加载 .env 配置
来源：http://fiz.shanyushiyangkeji.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ajy.hfpthk.cn

[U04] Py：变量调试打印
来源：http://dhb.hfpthk.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://chj.xuetiantiany.cn

[U05] Py：列表去重且保序
来源：http://zbm.xuanzx.com

list(dict.fromkeys(arr))
来源：http://kbn.ctjpmb.com

[U06] Py：合并两个字典
来源：http://pbo.yfazqb.com

{**a, **b}
来源：http://hce.redwolf501.top

[U07] Py：反转字典键值
来源：http://als.gaohongyu789.top

{v: k for k, v in d.items()}
来源：http://nap.tian-w.cn

[U08] Py：展平二维列表
来源：http://qvw.zhoulong.xyz

[y for x in nested for y in x]
来源：http://mjd.316326.xyz

[U09] Py：字典取最大值的键
来源：http://yfw.bbcook.cn

max(d, key=d.get)
来源：http://mtx.xuanzx.com

[U10] Py：按值排序字典
来源：http://eyo.daria6918.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://noy.yongpay.top

[U11] Py：生成器表达式
来源：http://stg.cucudq.cn

(x * 2 for x in arr)
来源：http://ghi.guowangkeji.top

[U12] Py：取出现最多的 3 个元素
来源：http://hth.yonumen.top

Counter(arr).most_common(3)
来源：http://ulo.redwolf501.top

[U13] Py：固定长度队列
来源：http://prl.xziqi.cn

deque(maxlen=10)
来源：http://eep.ydjk.org.cn

[U14] Py：分组收集到列表
来源：http://qik.shanyushiyangtech.top

defaultdict(list)
来源：http://svv.mhx1999.top

[U15] Py：高精度计时
来源：http://qet.jinyuanbaomall.cn

t = time.perf_counter()
来源：http://lqy.hcnkem.com

[U16] Py：命令行参数解析
来源：http://acz.sjlbkw.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fiu.aibaodan.cn

[U17] Py：初始化日志
来源：http://sbn.jinqigfzy.top

logging.basicConfig(level=logging.INFO)
来源：http://nnp.andypj.xyz

[U18] Py：预编译正则
来源：http://iou.fehbvm.com

pat = re.compile(r"\d+")
来源：http://dtr.uphjek.com

[U19] Py：正则替换带回调
来源：http://xaq.yangfankeji.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://iyt.vehdjk.com

[U20] Py：缓存函数结果
来源：http://dml.jiagoushi.top

@functools.lru_cache(maxsize=None)
来源：http://cku.bbcook.cn

[U21] Py：自定义上下文管理器
来源：http://xyo.jqgfzy.top

@contextlib.contextmanager
来源：http://dhk.ybcxt.top

[U22] Py：矩阵转置
来源：http://das.0kj1m.cn

list(zip(*m))
来源：http://mrt.tian-w.cn

[U23] Py：分块读取大文件
来源：http://dta.hnqzz.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qtp.zdqjudy.top

[U24] Py：路径操作
来源：http://fkg.zhijiandao.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xkc.iojbl.cn

[U25] Py：CSV 按字典读
来源：http://igx.jlsjyb.cn

csv.DictReader(f)
来源：http://mzf.ybcxt.top

[U26] Py：并发下载
来源：http://fpj.fehbvm.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ojf.yuanzhike.top

[U27] Py：异步 HTTP
来源：http://tqs.sjlbkw.cn

aiohttp.ClientSession() 配合 async with
来源：http://qgi.xylfe.cn

[U28] Py：类型别名
来源：http://joy.uphjek.com

UserId = int
来源：http://ywk.xziqi.cn

[U29] Py：属性校验
来源：http://yvq.hnxiangtu.top

@property 与 @x.setter 配合
来源：http://daw.wangdashe.top

[U30] Py：数据类
来源：http://eoy.dashuyun.cn

@dataclass(slots=True)
来源：http://htr.sweek.top

[U31] Py：单测
来源：http://jan.sxryk.cn

python -m pytest -q
来源：http://fss.fehbvm.com

[U32] Py：代码格式化
来源：http://zzv.yanxiufei.cn

ruff format . && ruff check --fix .
来源：http://kbf.guowangkeji.top

[U33] Py：打包发布
来源：http://xzm.smart0.xyz

python -m build  （依赖 pyproject.toml）
来源：http://xbk.316326.xyz

[U34] Py：判断编码
来源：http://tae.aibaodan.cn

chardet.detect(raw)
来源：http://vsp.ctjpmb.com

[U35] Py：发送邮件
来源：http://qlu.guowangkeji.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mci.yfazqb.com

[U36] Py：定时任务
来源：http://tns.dashuyun.cn

schedule.every(10).minutes.do(job)
来源：http://ylb.xuetiantiany.cn

[U37] Py：读写 Excel
来源：http://meq.hcnkem.com

pandas.read_excel / DataFrame.to_excel
来源：http://olt.hcnkem.com

[U38] Py：获取脚本所在目录
来源：http://nxy.jinyuanbaomall.cn

Path(__file__).resolve().parent
来源：http://vlq.mhx1999.top

[U39] Py：判断是否在交互环境
来源：http://xsc.hongshengwenyu.top

sys.stdout.isatty()
来源：http://oaz.dianchejie.cn

[U40] Py：打印到标准错误
来源：http://icd.ctjpmb.com

print("err", file=sys.stderr)
来源：http://xnf.kuanghao11.cn

[U41] PHP：初始化 Composer 项目
来源：http://vwp.feifeiyinyue.top

composer init;  composer require guzzlehttp/guzzle
来源：http://oot.hnxiangtu.top

[U42] PHP：PSR-4 自动加载
来源：http://opp.daxiang520.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://eix.bjfxy.top

[U43] PHP：声明命名空间
来源：http://tyr.sweek.top

namespace App\Http;
来源：http://trp.tanke756.top

[U44] PHP：开启严格类型
来源：http://inr.ybcxt.top

declare(strict_types=1);
来源：http://eqn.cucudq.cn

[U45] PHP：类型声明与返回类型
来源：http://gpc.yueranfly.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://mxt.xuetiantiany.cn

[U46] PHP：可空类型
来源：http://rdr.jinghuilouyu.cn

?string $name = null
来源：http://ymq.shanyushiyangkeji.top

[U47] PHP：联合类型
来源：http://net.pengpengdd.cyou

int|string $id
来源：http://ssg.quarkkingdee.top

[U48] PHP：纯枚举
来源：http://jtm.xinyue.icu

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://kxq.gaohongyu789.top

[U49] PHP：只读属性
来源：http://xuh.shanyushiyangtech.top

public readonly string $name
来源：http://uoj.kuanghao11.cn

[U50] PHP：构造器属性提升
来源：http://oee.dianchejie.cn

public function __construct(private int $id) {}
来源：http://nmn.tian-w.cn

[U51] PHP：数组解构
来源：http://vbu.hongshengwenyu.top

[$a, $b] = $arr;
来源：http://kgn.jinqigufen.top

[U52] PHP：箭头函数
来源：http://yxd.gzhubu.top

$double = fn($x) => $x * 2;
来源：http://ccd.cheryme.top

[U53] PHP：空合并运算符
来源：http://fgj.yuxming.cn

$v = $a ?? $b ?? "default";
来源：http://rbd.fktsv.cn

[U54] PHP：空安全调用
来源：http://vpr.xziqi.cn

$obj?->method()
来源：http://mkq.gzhubu.top

[U55] PHP：match 表达式
来源：http://ojc.xuetiantiany.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bmd.ydjk.org.cn

[U56] PHP：命名参数
来源：http://uec.xziqi.cn

f(a: 1, b: 2)
来源：http://eqx.cdnleiting.top

[U57] PHP：字符串插值
来源：http://gdv.zhengqikj.top

"值: {$a}"
来源：http://zqc.yuxming.cn

[U58] PHP：数组三件套
来源：http://pew.shanyushiyangtech.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cgz.ppjwa.cn

[U59] PHP：自定义排序
来源：http://bek.jiagoushi.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fku.cashguo.top

[U60] PHP：JSON 编解码
来源：http://rai.shanyushiyangkeji.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tyz.cucudq.cn

[U61] PHP：正则
来源：http://dwq.ehwqpu.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ycv.daria6918.cn

[U62] PHP：日期对象
来源：http://llv.zhijiandao.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://pzx.quarkkingdee.top

[U63] PHP：文件读写
来源：http://rdu.hnqzz.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jar.xinyue.icu

[U64] PHP：目录遍历
来源：http://ezk.hammf.cn

glob("dir/*.php");  scandir("dir");
来源：http://sgs.zhongyouzk.top

[U65] PHP：会话
来源：http://maw.ivvv.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ewf.tian-w.cn

[U66] PHP：设置 Cookie
来源：http://zbl.yuanzhike.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://alf.shzxlz.cn

[U67] PHP：处理文件上传
来源：http://gnq.jlsjyb.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kvh.yuanzhike.top

[U68] PHP：PDO 连接
来源：http://cdf.gotoacloud.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://swh.yangfankeji.com

[U69] PHP：PDO 预处理
来源：http://hon.aizwys.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://flb.jqgufenzy.top

[U70] PHP：PDO 事务
来源：http://qmi.jiagoushi.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tyl.sweek.top

[U71] PHP：抛出异常
来源：http://tsg.jinyuanbaomall.cn

throw new RuntimeException("失败", 500);
来源：http://zvd.gaohongyu789.top

[U72] PHP：写错误日志
来源：http://uhc.jinghuilouyu.cn

error_log("失败: " . $e->getMessage());
来源：http://yne.ybcxt.top

[U73] PHP：读取 ini 配置
来源：http://oom.shuidangran.top

parse_ini_file("config.ini", true)
来源：http://ovq.0kj1m.cn

[U74] PHP：读取环境变量
来源：http://ddb.pycfn.com

getenv("APP_ENV") ?: "production"
来源：http://aei.jianghu66.top

[U75] PHP：依赖注入
来源：http://yby.pengpengdd.cyou

composer require psr/container
来源：http://rfm.jlsjyb.cn

[U76] PHP：简单路由
来源：http://bvm.jinqigfzy.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lbr.bjfxy.top

[U77] PHP：模板渲染
来源：http://kpc.xylfe.cn

composer require twig/twig
来源：http://fzm.uphjek.com

[U78] PHP：单元测试
来源：http://qbf.vqdsnc.cn

composer require --dev phpunit/phpunit
来源：http://qkx.snrcjt.cn


<!-- 参考信息 -->