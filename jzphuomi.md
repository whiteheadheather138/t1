代发 wailian999

int size() const noexcept { return n_; }
来源：http://fqz.fehbvm.com

[S53] C++：移动语义
来源：http://sry.sysykeji.top

std::vector<int> w = std::move(v);
来源：http://kib.havefunace.top

[S54] C++：异常处理
来源：http://pvr.tian-w.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cuk.daria6918.cn

[S55] C++：结构化绑定
来源：http://rcd.ydzc1.top

auto [a, b] = std::make_pair(1, 2);
来源：http://qvx.hcnkem.com

[S56] C++：optional
来源：http://csi.xingfuxueyuan.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dko.fehbvm.com

[S57] C++：编译期常量
来源：http://tjj.fehbvm.com

constexpr int N = 10;
来源：http://cjz.smart0.xyz

[S58] C++：命名空间
来源：http://ezx.tian-w.cn

namespace ns { int f() { return 1; } }
来源：http://eey.pengpengdd.cyou

[S59] C++：静态断言
来源：http://bll.hammf.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://epa.yuxming.cn

[S60] C++：遍历并删除元素
来源：http://wjn.guowangkeji.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zle.yonumen.top

================================================================================
来源：http://mvz.andypj.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mcw.316326.xyz

================================================================================
来源：http://zto.zhongyouzk.top

[T01] Kotlin：Hello World
来源：http://zor.havefunace.top

println("Hello")
来源：http://atr.jyoumei.cn

[T02] Kotlin：变量
来源：http://qbu.shangyingyoupin.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zjb.yj20258888.top

[T03] Kotlin：字符串模板
来源：http://thx.fengsongda.top

"值: $b"
来源：http://twl.hammf.cn

[T04] Kotlin：空安全
来源：http://ymh.fanxiaobao.xyz

val n: String? = null;  n?.length
来源：http://qtr.aizwys.cn

[T05] Kotlin：when 表达式
来源：http://vpv.hnqzz.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ovs.pengpengdd.cyou

[T06] Kotlin：集合映射
来源：http://qlr.gaohongyu789.top

listOf(1, 2, 3).map { it * 2 }
来源：http://lxt.zhaomingkeji.xyz

[T07] Kotlin：集合过滤
来源：http://olf.kuanghao11.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://upv.ppjwa.cn

[T08] Kotlin：数据类
来源：http://tco.ivvv.top

data class User(val name: String, val age: Int)
来源：http://mat.hammf.cn

[T09] Kotlin：扩展函数
来源：http://wdn.smart0.xyz

fun String.exclaim() = this + "!"
来源：http://ioz.gogol.net.cn

[T10] Kotlin：默认参数
来源：http://yfe.guannengcc.top

fun greet(name: String = "World") = "Hi $name"
来源：http://sui.ybcxt.top

[T11] Kotlin：协程
来源：http://vyk.jyoumei.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wdu.chenlongwang.top

[T12] Kotlin：解构声明
来源：http://mtt.zdqjudy.top

val (a, b) = Pair(1, 2)
来源：http://owi.wangdashe.top

[T13] Kotlin：只读 Map
来源：http://vwl.9152youxi.cn

val m = mapOf("a" to 1)
来源：http://pff.tanke756.top

[T14] Kotlin：循环
来源：http://crm.shuidangran.top

for (i in 1..10) println(i)
来源：http://zzx.nanxuanxn.top

[T15] Kotlin：接口
来源：http://aon.9152youxi.cn

interface Shape { fun area(): Double }
来源：http://ziq.zdqjudy.top

[T16] Swift：Hello World
来源：http://joa.hcnkem.com

print("Hello")
来源：http://asf.cashguo.top

[T17] Swift：变量与常量
来源：http://hth.hammf.cn

var a = 1;  let b = 2
来源：http://vgp.quarkkingdee.top

[T18] Swift：字符串插值
来源：http://woy.kuanghao11.cn

"值: \(b)"
来源：http://rhy.sufxvd.cn

[T19] Swift：可选绑定
来源：http://mdk.ppjwa.cn

if let n = opt { print(n) }
来源：http://txt.guowangkeji.top

[T20] Swift：数组操作
来源：http://wbw.andypj.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://yja.dianchejie.cn

[T21] Swift：遍历
来源：http://hao.hcnkem.com

for x in a { print(x) }
来源：http://etx.dianchejie.cn

[T22] Swift：字典
来源：http://dos.jinqigufen.top

var d = ["a": 1];  d["b"] = 2
来源：http://wvi.sjlbkw.cn

[T23] Swift：函数
来源：http://whz.jqgfzy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pbm.pycfn.com

[T24] Swift：闭包
来源：http://ksx.bjfxy.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://nga.shanyushiyangkeji.top

[T25] Swift：结构体
来源：http://ifo.gogol.net.cn

struct P { var x: Int }
来源：http://dew.pengpengdd.cyou

[T26] Swift：类与重写
来源：http://lhw.wangdashe.top

class A: Base { override func f() {} }
来源：http://vjb.mhx1999.top

[T27] Swift：错误处理
来源：http://dla.sjlbkw.cn

do { try f() } catch { print(error) }
来源：http://kqp.zhongyouzk.top

[T28] Swift：枚举
来源：http://bge.redwolf501.top

enum Color { case red, green }
来源：http://yjm.iojbl.cn

[T29] Swift：guard 提前返回
来源：http://szr.fktsv.cn

guard let x = opt else { return }
来源：http://vcg.jqgfzy.top

[T30] Swift：协议
来源：http://awr.yuanzhike.top

protocol Shape { func area() -> Double }
来源：http://bqk.jyoumei.cn

[T31] Lua：Hello World
来源：http://wdm.cashguo.top

print("Hello")
来源：http://xat.cqqwz.cn

[T32] Lua：局部变量
来源：http://iap.epnwcf.com

local a = 1
来源：http://gjm.yj20258888.top

[T33] Lua：表（数组）
来源：http://tti.snrcjt.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ggc.yongpay.top

[T34] Lua：遍历表
来源：http://tct.chenzaomai.com

for i, v in ipairs(t) do print(i, v) end
来源：http://xra.yonumen.top

[T35] Lua：字典表
来源：http://lgx.dianchejie.cn

local d = { a = 1 };  d.b = 2
来源：http://lyn.tianlin.xyz

[T36] Lua：函数
来源：http://ipz.c1oappe.top

function add(a, b) return a + b end
来源：http://jus.vehdjk.com

[T37] Lua：字符串拼接
来源：http://szj.tarul.cn

"a" .. "b"
来源：http://eel.shuidangran.top

[T38] Lua：条件
来源：http://poi.vehdjk.com

if x > 0 then print("正") end
来源：http://qnc.gotoacloud.top

[T39] Lua：模式匹配
来源：http://esd.birdmap.top

string.find(s, "%d+")
来源：http://rgg.gogol.net.cn

[T40] Lua：元表
来源：http://dsc.xingfuxueyuan.xyz

setmetatable({}, { __index = base })
来源：http://fbp.dashuyun.cn

[T41] Perl：Hello World
来源：http://gud.yj20258.top

print "Hello\n";
来源：http://nwm.xinyue.icu

[T42] Perl：变量类型
来源：http://dpm.xinyue.icu

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://evp.bbcook.cn

[T43] Perl：字符串插值
来源：http://ihg.52xcode.cn

"值: $a"
来源：http://blg.shanyushiyangkeji.top

[T44] Perl：条件
来源：http://evf.ydzc1.top

if ($a > 0) { print "正"; }
来源：http://vqj.jinyuanbaomall.cn

[T45] Perl：数组遍历
来源：http://xtz.zycfv.cn

for my $x (@arr) { print $x; }
来源：http://zpy.jyoumei.cn

[T46] Perl：哈希操作
来源：http://ykp.chenjidiqi.icu

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gac.sufxvd.cn

[T47] Perl：正则捕获
来源：http://jvi.cqqwz.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://aep.shangyingyoupin.top

[T48] Perl：正则替换
来源：http://mcp.bbcook.cn

$s =~ s/old/new/g;
来源：http://njr.hongshengwenyu.top

[T49] Perl：函数
来源：http://oae.shanyushiyangkeji.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://flp.iojbl.cn

[T50] Perl：逐行读文件
来源：http://lqp.sxryk.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://cxp.aibaodan.cn

while (my $line = <$fh>) { print $line; }
来源：http://ogj.cashguo.top

[T51] Scala：Hello World
来源：http://nwd.sxryk.cn

println("Hello")
来源：http://wgn.hnqzz.top

[T52] Scala：变量
来源：http://hdf.ehwqpu.com

val a = 1;  var b = 2
来源：http://qxb.bbcook.cn

[T53] Scala：字符串插值
来源：http://ufg.hysaishi.cn

s"值: $b"
来源：http://rwe.zhengqikj.top

[T54] Scala：集合映射
来源：http://fvb.cucudq.cn

List(1, 2, 3).map(_ * 2)
来源：http://evt.guannengcc.top

[T55] Scala：集合过滤
来源：http://rdf.jlsjyb.cn

List(1, 2, 3).filter(_ > 1)
来源：http://dux.pengpengdd.cyou

[T56] Scala：样例类
来源：http://sgo.nwbrower.top

case class User(name: String, age: Int)
来源：http://jsr.meibo888.top

[T57] Scala：模式匹配
来源：http://dls.sweek.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ocw.epnwcf.com

[T58] Scala：函数定义
来源：http://rnj.jyoumei.cn

def add(a: Int, b: Int): Int = a + b
来源：http://voy.wangdashe.top

[T59] Scala：循环
来源：http://iht.hesvh.cn

for (i <- 1 to 10) println(i)
来源：http://ldf.tian-w.cn

[T60] Scala：折叠
来源：http://vdl.zdqjudy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lob.fktsv.cn

================================================================================
来源：http://mbo.shanyushiyangkeji.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xbk.guannengcc.top

================================================================================
来源：http://uzo.zhengqikj.top

[U01] Py：创建虚拟环境
来源：http://box.9152youxi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://kab.zhengqikj.top

[U02] Py：导出 / 安装依赖
来源：http://mts.chenjidiqi.icu

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rwa.vehdjk.com

[U03] Py：加载 .env 配置
来源：http://esr.uphjek.com

from dotenv import load_dotenv; load_dotenv()
来源：http://lxo.ydjk.org.cn

[U04] Py：变量调试打印
来源：http://vws.xziqi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rql.cdnleiting.top

[U05] Py：列表去重且保序
来源：http://vkj.jiagoushi.top

list(dict.fromkeys(arr))
来源：http://hen.feifeiyinyue.top

[U06] Py：合并两个字典
来源：http://tkx.havefunace.top

{**a, **b}
来源：http://srr.zhijiandao.cn

[U07] Py：反转字典键值
来源：http://wlo.mhx1999.top

{v: k for k, v in d.items()}
来源：http://khz.nwbrower.top

[U08] Py：展平二维列表
来源：http://emy.zycfv.cn

[y for x in nested for y in x]
来源：http://nfi.jqgfzy.top

[U09] Py：字典取最大值的键
来源：http://zoj.shuidangran.top

max(d, key=d.get)
来源：http://oqg.fengsongda.top

[U10] Py：按值排序字典
来源：http://kbi.xylfe.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sdj.xziqi.cn

[U11] Py：生成器表达式
来源：http://ieq.hywenlv.cn

(x * 2 for x in arr)
来源：http://glm.gotoacloud.top

[U12] Py：取出现最多的 3 个元素
来源：http://kps.jinqigfzy.top

Counter(arr).most_common(3)
来源：http://ggo.kuanghao11.cn

[U13] Py：固定长度队列
来源：http://alw.jqgufenzy.top

deque(maxlen=10)
来源：http://ntr.yj20258.top

[U14] Py：分组收集到列表
来源：http://eps.yuanzhike.top

defaultdict(list)
来源：http://nfr.hysaishi.cn

[U15] Py：高精度计时
来源：http://nkk.uphjek.com

t = time.perf_counter()
来源：http://qfe.aibaodan.cn

[U16] Py：命令行参数解析
来源：http://zfj.jyoumei.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fqf.hammf.cn

[U17] Py：初始化日志
来源：http://hvh.ehwqpu.com

logging.basicConfig(level=logging.INFO)
来源：http://ayn.zhengqikj.top

[U18] Py：预编译正则
来源：http://ryc.pengpengdd.cyou

pat = re.compile(r"\d+")
来源：http://jeg.xziqi.cn

[U19] Py：正则替换带回调
来源：http://osl.sxryk.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://our.cucudq.cn

[U20] Py：缓存函数结果
来源：http://shk.jlsjyb.cn

@functools.lru_cache(maxsize=None)
来源：http://bpg.gzhubu.top

[U21] Py：自定义上下文管理器
来源：http://rxk.smart0.xyz

@contextlib.contextmanager
来源：http://jfn.snrcjt.cn

[U22] Py：矩阵转置
来源：http://htk.52xcode.cn

list(zip(*m))
来源：http://zow.shangyingyoupin.top

[U23] Py：分块读取大文件
来源：http://lui.smart0.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://che.zdqjudy.top

[U24] Py：路径操作
来源：http://zkw.sufxvd.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ptn.jyoumei.cn

[U25] Py：CSV 按字典读
来源：http://lhs.redwolf501.top

csv.DictReader(f)
来源：http://fyz.ppjwa.cn

[U26] Py：并发下载
来源：http://kcj.yj202588.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bbz.sysykeji.top

[U27] Py：异步 HTTP
来源：http://ktk.sweek.top

aiohttp.ClientSession() 配合 async with
来源：http://fdz.jinghuilouyu.cn

[U28] Py：类型别名
来源：http://szr.52xcode.cn

UserId = int
来源：http://gtd.xinyue.icu

[U29] Py：属性校验
来源：http://tvi.zhiwuduotai.top

@property 与 @x.setter 配合
来源：http://eha.cheryme.top

[U30] Py：数据类
来源：http://ceg.yonumen.top

@dataclass(slots=True)
来源：http://uat.316326.xyz

[U31] Py：单测
来源：http://dtv.hnqzz.top

python -m pytest -q
来源：http://aay.uphjek.com

[U32] Py：代码格式化
来源：http://xqv.nanxuanxn.top

ruff format . && ruff check --fix .
来源：http://vlq.zhaomingkeji.xyz

[U33] Py：打包发布
来源：http://paw.yuxming.cn

python -m build  （依赖 pyproject.toml）
来源：http://lqq.yongpay.top

[U34] Py：判断编码
来源：http://ekn.jinqigfzy.top

chardet.detect(raw)
来源：http://bwu.xuetiantiany.cn

[U35] Py：发送邮件
来源：http://eec.yueranfly.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bfc.fanxiaobao.xyz

[U36] Py：定时任务
来源：http://xqt.hongshengwenyu.top

schedule.every(10).minutes.do(job)
来源：http://chs.cashguo.top

[U37] Py：读写 Excel
来源：http://ueu.yueranfly.top

pandas.read_excel / DataFrame.to_excel
来源：http://iot.nwbrower.top

[U38] Py：获取脚本所在目录
来源：http://wdl.bbcook.cn

Path(__file__).resolve().parent
来源：http://sou.zhixingplan.top

[U39] Py：判断是否在交互环境
来源：http://cxr.andypj.xyz

sys.stdout.isatty()
来源：http://ztd.hfpthk.cn

[U40] Py：打印到标准错误
来源：http://sjm.cucudq.cn

print("err", file=sys.stderr)
来源：http://vxj.kuanghao11.cn

[U41] PHP：初始化 Composer 项目
来源：http://paa.quarkkingdee.top

composer init;  composer require guzzlehttp/guzzle
来源：http://nog.zdqjudy.top

[U42] PHP：PSR-4 自动加载
来源：http://pqr.daria6918.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ufz.zhijiandao.cn

[U43] PHP：声明命名空间
来源：http://yte.c1oappe.top

namespace App\Http;
来源：http://iwh.ppjwa.cn

[U44] PHP：开启严格类型
来源：http://khb.quarkkingdee.top

declare(strict_types=1);
来源：http://dmp.guannengcc.top

[U45] PHP：类型声明与返回类型
来源：http://uwo.yj202588.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://vkx.yj202588.top

[U46] PHP：可空类型
来源：http://tpx.hcnkem.com

?string $name = null
来源：http://sno.ivvv.top

[U47] PHP：联合类型
来源：http://waw.ppjwa.cn

int|string $id
来源：http://twn.shanyushiyangtech.top

[U48] PHP：纯枚举
来源：http://tgw.zhiwuduotai.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rmz.ehwqpu.com

[U49] PHP：只读属性
来源：http://obr.jqgufenzy.top

public readonly string $name
来源：http://iev.fehbvm.com

[U50] PHP：构造器属性提升
来源：http://jnz.jqgufenzy.top

public function __construct(private int $id) {}
来源：http://srd.sysykeji.top

[U51] PHP：数组解构
来源：http://sbi.cheryme.top

[$a, $b] = $arr;
来源：http://okg.sjlbkw.cn

[U52] PHP：箭头函数
来源：http://ugw.ywan-chungtsiang.top

$double = fn($x) => $x * 2;
来源：http://hqm.gogol.net.cn

[U53] PHP：空合并运算符
来源：http://ikl.hywenlv.cn

$v = $a ?? $b ?? "default";
来源：http://ugr.zycfv.cn

[U54] PHP：空安全调用
来源：http://nvh.jlsjyb.cn

$obj?->method()
来源：http://ufm.c1oappe.top

[U55] PHP：match 表达式
来源：http://gvx.meibo888.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gmb.jqgfzy.top

[U56] PHP：命名参数
来源：http://var.ybcxt.top

f(a: 1, b: 2)
来源：http://bid.zhaomingkeji.xyz

[U57] PHP：字符串插值
来源：http://nfq.meibo888.top

"值: {$a}"
来源：http://xru.fanxiaobao.xyz

[U58] PHP：数组三件套
来源：http://tgw.zdbjq.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mrx.shanyushiyangtech.top

[U59] PHP：自定义排序
来源：http://wmb.9152youxi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fpd.cdnleiting.top

[U60] PHP：JSON 编解码
来源：http://vqg.yuanzhike.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ozt.nanxuanxn.top

[U61] PHP：正则
来源：http://gyi.shanyushiyangtech.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cyf.chenlongwang.top

[U62] PHP：日期对象
来源：http://cnb.feifeiyinyue.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zmm.jqgufenzy.top

[U63] PHP：文件读写
来源：http://omq.cashguo.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zxu.tanke756.top

[U64] PHP：目录遍历
来源：http://ahh.daria6918.cn

glob("dir/*.php");  scandir("dir");
来源：http://gyg.xingfuxueyuan.xyz

[U65] PHP：会话
来源：http://wgq.quarkkingdee.top

session_start();  $_SESSION["uid"] = 1;
来源：http://hle.xingfuxueyuan.xyz

[U66] PHP：设置 Cookie
来源：http://alw.ctjpmb.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://wll.xuetiantiany.cn

[U67] PHP：处理文件上传
来源：http://ebm.bjfxy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://osy.pycfn.com

[U68] PHP：PDO 连接
来源：http://bvl.gaohongyu789.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fqz.xuetiantiany.cn

[U69] PHP：PDO 预处理
来源：http://nnc.ppjwa.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://myh.iojbl.cn

[U70] PHP：PDO 事务
来源：http://gna.havefunace.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tiv.316326.xyz

[U71] PHP：抛出异常
来源：http://aos.smart0.xyz

throw new RuntimeException("失败", 500);
来源：http://ypt.bbcook.cn

[U72] PHP：写错误日志
来源：http://pya.yanxiufei.cn

error_log("失败: " . $e->getMessage());
来源：http://nxp.shangyingyoupin.top

[U73] PHP：读取 ini 配置
来源：http://akx.bjfxy.top

parse_ini_file("config.ini", true)
来源：http://ghh.nanxuanxn.top

[U74] PHP：读取环境变量
来源：http://ydf.jqgufenzy.top

getenv("APP_ENV") ?: "production"
来源：http://gil.tarul.cn

[U75] PHP：依赖注入
来源：http://rmz.hcnkem.com

composer require psr/container
来源：http://asg.iojbl.cn

[U76] PHP：简单路由
来源：http://qor.shangyingyoupin.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://ccy.shanyushiyangtech.top

[U77] PHP：模板渲染
来源：http://zse.xinyue.icu

composer require twig/twig
来源：http://soa.ybcxt.top

[U78] PHP：单元测试
来源：http://ypr.jlsjyb.cn

composer require --dev phpunit/phpunit
来源：http://owe.9152youxi.cn


<!-- 参考信息 -->