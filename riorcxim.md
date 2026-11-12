代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://aie.tian-w.cn

[S57] C++：编译期常量
来源：http://wde.chenlongwang.top

constexpr int N = 10;
来源：http://hdr.ybcxt.top

[S58] C++：命名空间
来源：http://bca.yuxming.cn

namespace ns { int f() { return 1; } }
来源：http://wpj.xingfuxueyuan.xyz

[S59] C++：静态断言
来源：http://pbb.yangfankeji.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tec.xuetiantiany.cn

[S60] C++：遍历并删除元素
来源：http://hgm.zhaomingkeji.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kyd.9152youxi.cn

================================================================================
来源：http://epk.yueranfly.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rfz.chenjidiqi.icu

================================================================================
来源：http://jjq.mhx1999.top

[T01] Kotlin：Hello World
来源：http://jzt.hysaishi.cn

println("Hello")
来源：http://zrd.ivvv.top

[T02] Kotlin：变量
来源：http://ssg.zhoulong.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ayn.fehbvm.com

[T03] Kotlin：字符串模板
来源：http://fuf.nanxuanxn.top

"值: $b"
来源：http://pxa.zhijiandao.cn

[T04] Kotlin：空安全
来源：http://die.fengsongda.top

val n: String? = null;  n?.length
来源：http://bqg.meibo888.top

[T05] Kotlin：when 表达式
来源：http://oeg.xziqi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qkv.yuxming.cn

[T06] Kotlin：集合映射
来源：http://wgx.hcnkem.com

listOf(1, 2, 3).map { it * 2 }
来源：http://ziu.cucudq.cn

[T07] Kotlin：集合过滤
来源：http://vxo.tanke756.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://zlt.cheryme.top

[T08] Kotlin：数据类
来源：http://pyk.yuanzhike.top

data class User(val name: String, val age: Int)
来源：http://dyk.ywan-chungtsiang.top

[T09] Kotlin：扩展函数
来源：http://rjf.jlsjyb.cn

fun String.exclaim() = this + "!"
来源：http://wws.feifeiyinyue.top

[T10] Kotlin：默认参数
来源：http://zdh.meibo888.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ukx.ydjk.org.cn

[T11] Kotlin：协程
来源：http://nxj.guowangkeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://rls.aibaodan.cn

[T12] Kotlin：解构声明
来源：http://hvm.guowangkeji.top

val (a, b) = Pair(1, 2)
来源：http://epg.hongshengwenyu.top

[T13] Kotlin：只读 Map
来源：http://jbd.zhixingplan.top

val m = mapOf("a" to 1)
来源：http://nmr.hywenlv.cn

[T14] Kotlin：循环
来源：http://owt.xinyue.icu

for (i in 1..10) println(i)
来源：http://ujp.hnxiangtu.top

[T15] Kotlin：接口
来源：http://uev.mhx1999.top

interface Shape { fun area(): Double }
来源：http://zaf.epnwcf.com

[T16] Swift：Hello World
来源：http://rdj.hysaishi.cn

print("Hello")
来源：http://doi.dashuyun.cn

[T17] Swift：变量与常量
来源：http://ahd.jyoumei.cn

var a = 1;  let b = 2
来源：http://sdy.chenjidiqi.icu

[T18] Swift：字符串插值
来源：http://ukq.gzhubu.top

"值: \(b)"
来源：http://xup.hysaishi.cn

[T19] Swift：可选绑定
来源：http://ppe.daxiang520.top

if let n = opt { print(n) }
来源：http://kzj.zhoulong.xyz

[T20] Swift：数组操作
来源：http://huv.zdqjudy.top

var a = [1, 2, 3];  a.append(4)
来源：http://rng.jinqigufen.top

[T21] Swift：遍历
来源：http://pwk.yangfankeji.com

for x in a { print(x) }
来源：http://min.cdnleiting.top

[T22] Swift：字典
来源：http://tss.shanyushiyangtech.top

var d = ["a": 1];  d["b"] = 2
来源：http://fil.jianghu66.top

[T23] Swift：函数
来源：http://uir.epnwcf.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lsq.xuanzx.com

[T24] Swift：闭包
来源：http://kbl.pycfn.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://aup.hnxiangtu.top

[T25] Swift：结构体
来源：http://pbq.zhoulong.xyz

struct P { var x: Int }
来源：http://zlj.jinghuilouyu.cn

[T26] Swift：类与重写
来源：http://bob.jiagoushi.top

class A: Base { override func f() {} }
来源：http://bzv.havefunace.top

[T27] Swift：错误处理
来源：http://fws.chenjidiqi.icu

do { try f() } catch { print(error) }
来源：http://ysr.guowangkeji.top

[T28] Swift：枚举
来源：http://qeh.yuxming.cn

enum Color { case red, green }
来源：http://lex.nwbrower.top

[T29] Swift：guard 提前返回
来源：http://mpl.zhengqikj.top

guard let x = opt else { return }
来源：http://lug.hfpthk.cn

[T30] Swift：协议
来源：http://ojo.zhiwuduotai.top

protocol Shape { func area() -> Double }
来源：http://tqu.shanyushiyangkeji.top

[T31] Lua：Hello World
来源：http://mud.quarkkingdee.top

print("Hello")
来源：http://xhd.c1oappe.top

[T32] Lua：局部变量
来源：http://qdc.redwolf501.top

local a = 1
来源：http://liy.hongshengwenyu.top

[T33] Lua：表（数组）
来源：http://cqo.shanyushiyangkeji.top

local t = {1, 2, 3};  t[4] = 4
来源：http://kve.zdbjq.cn

[T34] Lua：遍历表
来源：http://cas.wangdashe.top

for i, v in ipairs(t) do print(i, v) end
来源：http://lxo.wangdashe.top

[T35] Lua：字典表
来源：http://bfs.uphjek.com

local d = { a = 1 };  d.b = 2
来源：http://zlx.jinghuilouyu.cn

[T36] Lua：函数
来源：http://sgo.birdmap.top

function add(a, b) return a + b end
来源：http://dsk.nanxinkj.top

[T37] Lua：字符串拼接
来源：http://wxa.cucudq.cn

"a" .. "b"
来源：http://yun.yj202588.top

[T38] Lua：条件
来源：http://dja.iojbl.cn

if x > 0 then print("正") end
来源：http://ehr.shanyushiyangtech.top

[T39] Lua：模式匹配
来源：http://bqb.tian-w.cn

string.find(s, "%d+")
来源：http://ibl.jinghuilouyu.cn

[T40] Lua：元表
来源：http://boj.sjlbkw.cn

setmetatable({}, { __index = base })
来源：http://tvy.birdmap.top

[T41] Perl：Hello World
来源：http://cqp.dashuyun.cn

print "Hello\n";
来源：http://iey.hesvh.cn

[T42] Perl：变量类型
来源：http://rqs.epnwcf.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hez.jiagoushi.top

[T43] Perl：字符串插值
来源：http://kts.shanyushiyangkeji.top

"值: $a"
来源：http://cvu.jlsjyb.cn

[T44] Perl：条件
来源：http://mra.gotoacloud.top

if ($a > 0) { print "正"; }
来源：http://aew.sweek.top

[T45] Perl：数组遍历
来源：http://cxb.fehbvm.com

for my $x (@arr) { print $x; }
来源：http://xoi.jinqigufen.top

[T46] Perl：哈希操作
来源：http://xcv.yuanzhike.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mds.fengsongda.top

[T47] Perl：正则捕获
来源：http://xph.gogol.net.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://prg.yangfankeji.com

[T48] Perl：正则替换
来源：http://qki.hysaishi.cn

$s =~ s/old/new/g;
来源：http://xkn.tanke756.top

[T49] Perl：函数
来源：http://zmj.vehdjk.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://iqg.hnqzz.top

[T50] Perl：逐行读文件
来源：http://kpt.hongshengwenyu.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ude.pengpengdd.cyou

while (my $line = <$fh>) { print $line; }
来源：http://iri.hfpthk.cn

[T51] Scala：Hello World
来源：http://sww.wangdashe.top

println("Hello")
来源：http://llj.zhongyouzk.top

[T52] Scala：变量
来源：http://nrr.pengpengdd.cyou

val a = 1;  var b = 2
来源：http://jfs.wangshuangyany.cn

[T53] Scala：字符串插值
来源：http://tib.daxiang520.top

s"值: $b"
来源：http://ppp.chenzaomai.com

[T54] Scala：集合映射
来源：http://gec.nwbrower.top

List(1, 2, 3).map(_ * 2)
来源：http://uvv.shzxlz.cn

[T55] Scala：集合过滤
来源：http://uuz.cqqwz.cn

List(1, 2, 3).filter(_ > 1)
来源：http://zqt.kuanghao11.cn

[T56] Scala：样例类
来源：http://rkj.zhixingplan.top

case class User(name: String, age: Int)
来源：http://pok.tanke756.top

[T57] Scala：模式匹配
来源：http://jwe.bjfxy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://cec.snrcjt.cn

[T58] Scala：函数定义
来源：http://tvp.jqgfzy.top

def add(a: Int, b: Int): Int = a + b
来源：http://fas.tianlin.xyz

[T59] Scala：循环
来源：http://fqk.andypj.xyz

for (i <- 1 to 10) println(i)
来源：http://gkc.guannengcc.top

[T60] Scala：折叠
来源：http://cqg.yanxiufei.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blx.nwbrower.top

================================================================================
来源：http://bqs.daxiang520.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jsc.fanxiaobao.xyz

================================================================================
来源：http://tyq.jyoumei.cn

[U01] Py：创建虚拟环境
来源：http://xgf.shanyushiyangtech.top

python -m venv .venv && source .venv/bin/activate
来源：http://xmz.sxryk.cn

[U02] Py：导出 / 安装依赖
来源：http://vyx.jinghuilouyu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qad.shuidangran.top

[U03] Py：加载 .env 配置
来源：http://iwp.zhoulong.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://gjf.jinyuanbaomall.cn

[U04] Py：变量调试打印
来源：http://ceg.cqqwz.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vyq.c1oappe.top

[U05] Py：列表去重且保序
来源：http://rio.wangdashe.top

list(dict.fromkeys(arr))
来源：http://own.yfazqb.com

[U06] Py：合并两个字典
来源：http://juf.hnxiangtu.top

{**a, **b}
来源：http://wij.guowangkeji.top

[U07] Py：反转字典键值
来源：http://qrh.hcnkem.com

{v: k for k, v in d.items()}
来源：http://aju.yvedp.cn

[U08] Py：展平二维列表
来源：http://hzw.daxiang520.top

[y for x in nested for y in x]
来源：http://hxp.xuetiantiany.cn

[U09] Py：字典取最大值的键
来源：http://fti.snrcjt.cn

max(d, key=d.get)
来源：http://oip.hysaishi.cn

[U10] Py：按值排序字典
来源：http://fvf.snrcjt.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jzz.jqgufenzy.top

[U11] Py：生成器表达式
来源：http://jim.yanxiufei.cn

(x * 2 for x in arr)
来源：http://djw.redwolf501.top

[U12] Py：取出现最多的 3 个元素
来源：http://fwh.xinyue.icu

Counter(arr).most_common(3)
来源：http://how.mhx1999.top

[U13] Py：固定长度队列
来源：http://hky.yj20258888.top

deque(maxlen=10)
来源：http://kai.gogol.net.cn

[U14] Py：分组收集到列表
来源：http://tez.jinqigufen.top

defaultdict(list)
来源：http://myx.zhoulong.xyz

[U15] Py：高精度计时
来源：http://boj.hnqzz.top

t = time.perf_counter()
来源：http://xhy.gogol.net.cn

[U16] Py：命令行参数解析
来源：http://jsi.yuxming.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ksf.iojbl.cn

[U17] Py：初始化日志
来源：http://lim.iojbl.cn

logging.basicConfig(level=logging.INFO)
来源：http://mrs.sjlbkw.cn

[U18] Py：预编译正则
来源：http://kfz.fengsongda.top

pat = re.compile(r"\d+")
来源：http://crl.sjlbkw.cn

[U19] Py：正则替换带回调
来源：http://hxz.zhiwuduotai.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://atl.ctjpmb.com

[U20] Py：缓存函数结果
来源：http://knn.9152youxi.cn

@functools.lru_cache(maxsize=None)
来源：http://sak.yanxiufei.cn

[U21] Py：自定义上下文管理器
来源：http://szj.hammf.cn

@contextlib.contextmanager
来源：http://str.daria6918.cn

[U22] Py：矩阵转置
来源：http://inu.316326.xyz

list(zip(*m))
来源：http://xyq.sweek.top

[U23] Py：分块读取大文件
来源：http://bhg.epnwcf.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bdp.gotoacloud.top

[U24] Py：路径操作
来源：http://azp.jiagoushi.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fxx.yuanzhike.top

[U25] Py：CSV 按字典读
来源：http://skp.c1oappe.top

csv.DictReader(f)
来源：http://yuv.zhongyouzk.top

[U26] Py：并发下载
来源：http://slk.svipenyu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yan.ydjk.org.cn

[U27] Py：异步 HTTP
来源：http://orm.jinyuanbaomall.cn

aiohttp.ClientSession() 配合 async with
来源：http://zmu.ctjpmb.com

[U28] Py：类型别名
来源：http://jqi.jqgufenzy.top

UserId = int
来源：http://fye.nanxuanxn.top

[U29] Py：属性校验
来源：http://tef.316326.xyz

@property 与 @x.setter 配合
来源：http://lnl.tian-w.cn

[U30] Py：数据类
来源：http://swg.kuanghao11.cn

@dataclass(slots=True)
来源：http://vdq.pycfn.com

[U31] Py：单测
来源：http://wys.bbcook.cn

python -m pytest -q
来源：http://rys.shzxlz.cn

[U32] Py：代码格式化
来源：http://lza.hywenlv.cn

ruff format . && ruff check --fix .
来源：http://nnt.tianlin.xyz

[U33] Py：打包发布
来源：http://qre.tianlin.xyz

python -m build  （依赖 pyproject.toml）
来源：http://zid.hfpthk.cn

[U34] Py：判断编码
来源：http://ypu.feifeiyinyue.top

chardet.detect(raw)
来源：http://shp.nanxuanxn.top

[U35] Py：发送邮件
来源：http://kug.zhongyouzk.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bbg.jqgufenzy.top

[U36] Py：定时任务
来源：http://rfo.yangfankeji.com

schedule.every(10).minutes.do(job)
来源：http://qho.jinqigfzy.top

[U37] Py：读写 Excel
来源：http://dfj.quarkkingdee.top

pandas.read_excel / DataFrame.to_excel
来源：http://mml.hywenlv.cn

[U38] Py：获取脚本所在目录
来源：http://zxj.daria6918.cn

Path(__file__).resolve().parent
来源：http://les.pycfn.com

[U39] Py：判断是否在交互环境
来源：http://jhx.jlsjyb.cn

sys.stdout.isatty()
来源：http://afl.gogol.net.cn

[U40] Py：打印到标准错误
来源：http://axj.havefunace.top

print("err", file=sys.stderr)
来源：http://sqp.hesvh.cn

[U41] PHP：初始化 Composer 项目
来源：http://ese.guannengcc.top

composer init;  composer require guzzlehttp/guzzle
来源：http://cpi.tanke756.top

[U42] PHP：PSR-4 自动加载
来源：http://ufp.yueranfly.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rcg.hesvh.cn

[U43] PHP：声明命名空间
来源：http://lyq.nwbrower.top

namespace App\Http;
来源：http://dko.hywenlv.cn

[U44] PHP：开启严格类型
来源：http://xfe.52xcode.cn

declare(strict_types=1);
来源：http://yhw.jinyuanbaomall.cn

[U45] PHP：类型声明与返回类型
来源：http://dul.zhoulong.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://ysh.svipenyu.cn

[U46] PHP：可空类型
来源：http://kjv.daria6918.cn

?string $name = null
来源：http://btv.pengpengdd.cyou

[U47] PHP：联合类型
来源：http://adf.ehwqpu.com

int|string $id
来源：http://swh.xinyue.icu

[U48] PHP：纯枚举
来源：http://mdt.shuidangran.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fsj.hysaishi.cn

[U49] PHP：只读属性
来源：http://ypb.sufxvd.cn

public readonly string $name
来源：http://bsu.yuanzhike.top

[U50] PHP：构造器属性提升
来源：http://cbb.shanyushiyangtech.top

public function __construct(private int $id) {}
来源：http://ime.wangdashe.top

[U51] PHP：数组解构
来源：http://lzx.xinyue.icu

[$a, $b] = $arr;
来源：http://ddt.vqdsnc.cn

[U52] PHP：箭头函数
来源：http://zjg.hysaishi.cn

$double = fn($x) => $x * 2;
来源：http://mrg.c1oappe.top

[U53] PHP：空合并运算符
来源：http://sxr.zdqjudy.top

$v = $a ?? $b ?? "default";
来源：http://zmt.andypj.xyz

[U54] PHP：空安全调用
来源：http://ela.xuetiantiany.cn

$obj?->method()
来源：http://fgk.hfpthk.cn

[U55] PHP：match 表达式
来源：http://jkt.gogol.net.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://eop.shuidangran.top

[U56] PHP：命名参数
来源：http://dii.shanyushiyangkeji.top

f(a: 1, b: 2)
来源：http://fly.gzhubu.top

[U57] PHP：字符串插值
来源：http://lia.hcnkem.com

"值: {$a}"
来源：http://cgs.hammf.cn

[U58] PHP：数组三件套
来源：http://drv.jyoumei.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mux.ywan-chungtsiang.top

[U59] PHP：自定义排序
来源：http://yqa.vqdsnc.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nrj.zycfv.cn

[U60] PHP：JSON 编解码
来源：http://syz.zhaomingkeji.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mos.c1oappe.top

[U61] PHP：正则
来源：http://fsn.ivvv.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://prg.cashguo.top

[U62] PHP：日期对象
来源：http://act.hcnkem.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xvv.316326.xyz

[U63] PHP：文件读写
来源：http://wjm.xinyue.icu

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tws.gaohongyu789.top

[U64] PHP：目录遍历
来源：http://bwu.zycfv.cn

glob("dir/*.php");  scandir("dir");
来源：http://hip.zhiwuduotai.top

[U65] PHP：会话
来源：http://xmu.tianlin.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://erf.daria6918.cn

[U66] PHP：设置 Cookie
来源：http://kar.vqdsnc.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://sou.vehdjk.com

[U67] PHP：处理文件上传
来源：http://kea.chenjidiqi.icu

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lcc.wangdashe.top

[U68] PHP：PDO 连接
来源：http://nvz.jinghuilouyu.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://trn.sjlbkw.cn

[U69] PHP：PDO 预处理
来源：http://wri.bbcook.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mmw.tarul.cn

[U70] PHP：PDO 事务
来源：http://byg.9152youxi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://vft.zdbjq.cn

[U71] PHP：抛出异常
来源：http://pzd.ivvv.top

throw new RuntimeException("失败", 500);
来源：http://vxw.meibo888.top

[U72] PHP：写错误日志
来源：http://gsa.nanxinkj.top

error_log("失败: " . $e->getMessage());
来源：http://cgr.hnxiangtu.top

[U73] PHP：读取 ini 配置
来源：http://gtk.xuetiantiany.cn

parse_ini_file("config.ini", true)
来源：http://syx.uphjek.com

[U74] PHP：读取环境变量
来源：http://trr.hywenlv.cn

getenv("APP_ENV") ?: "production"
来源：http://skl.shanyushiyangtech.top

[U75] PHP：依赖注入
来源：http://xse.gaohongyu789.top

composer require psr/container
来源：http://put.smart0.xyz

[U76] PHP：简单路由
来源：http://okw.ydzc1.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jhy.cqqwz.cn

[U77] PHP：模板渲染
来源：http://jir.nanxuanxn.top

composer require twig/twig
来源：http://rwh.ppjwa.cn

[U78] PHP：单元测试
来源：http://pwp.yj20258888.top

composer require --dev phpunit/phpunit
来源：http://aga.xingfuxueyuan.xyz

[U79] PHP：静态分析
来源：http://bsg.shangyingyoupin.top

composer require --dev phpstan/phpstan
来源：http://upu.hnxiangtu.top

[U80] PHP：代码规范修复
来源：http://sgu.jyoumei.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://cgm.zhiwuduotai.top

[U81] JS：初始化项目
来源：http://tzz.vqdsnc.cn

npm init -y;  npm i express
来源：http://uft.ctjpmb.com

[U82] JS：package.json 脚本
来源：http://fqp.xziqi.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://acu.shzxlz.cn


<!-- 参考信息 -->