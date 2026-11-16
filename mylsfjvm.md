代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zuu.xuetiantiany.cn

[S57] C++：编译期常量
来源：http://wau.svipenyu.cn

constexpr int N = 10;
来源：http://gzx.yueranfly.top

[S58] C++：命名空间
来源：http://dxp.ivvv.top

namespace ns { int f() { return 1; } }
来源：http://nle.cheryme.top

[S59] C++：静态断言
来源：http://iof.ydjk.org.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://end.xuetiantiany.cn

[S60] C++：遍历并删除元素
来源：http://rgq.hfpthk.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bfv.shangyingyoupin.top

================================================================================
来源：http://lhv.xuanzx.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://iud.ehwqpu.com

================================================================================
来源：http://med.ywan-chungtsiang.top

[T01] Kotlin：Hello World
来源：http://hms.jlsjyb.cn

println("Hello")
来源：http://onc.redwolf501.top

[T02] Kotlin：变量
来源：http://yzu.guannengcc.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nqz.c1oappe.top

[T03] Kotlin：字符串模板
来源：http://iod.aibaodan.cn

"值: $b"
来源：http://tiw.hammf.cn

[T04] Kotlin：空安全
来源：http://ert.shanyushiyangtech.top

val n: String? = null;  n?.length
来源：http://inr.hesvh.cn

[T05] Kotlin：when 表达式
来源：http://rjh.nwbrower.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://roh.zhixingplan.top

[T06] Kotlin：集合映射
来源：http://sas.9152youxi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://lvr.hfpthk.cn

[T07] Kotlin：集合过滤
来源：http://ird.xziqi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://mpc.chenzaomai.com

[T08] Kotlin：数据类
来源：http://lkz.jinghuilouyu.cn

data class User(val name: String, val age: Int)
来源：http://ndc.jinyuanbaomall.cn

[T09] Kotlin：扩展函数
来源：http://yun.vehdjk.com

fun String.exclaim() = this + "!"
来源：http://det.gaohongyu789.top

[T10] Kotlin：默认参数
来源：http://vsd.ehwqpu.com

fun greet(name: String = "World") = "Hi $name"
来源：http://hgm.yangfankeji.com

[T11] Kotlin：协程
来源：http://azw.jlsjyb.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ahz.zhaomingkeji.xyz

[T12] Kotlin：解构声明
来源：http://kiv.zdbjq.cn

val (a, b) = Pair(1, 2)
来源：http://zrr.shangyingyoupin.top

[T13] Kotlin：只读 Map
来源：http://byb.zhongyouzk.top

val m = mapOf("a" to 1)
来源：http://lnw.fzhhl.top

[T14] Kotlin：循环
来源：http://ojm.zdqjudy.top

for (i in 1..10) println(i)
来源：http://gnb.zhijiandao.cn

[T15] Kotlin：接口
来源：http://ulx.gzhubu.top

interface Shape { fun area(): Double }
来源：http://jsm.ppjwa.cn

[T16] Swift：Hello World
来源：http://klh.shanyushiyangtech.top

print("Hello")
来源：http://pgz.jqgfzy.top

[T17] Swift：变量与常量
来源：http://saj.tian-w.cn

var a = 1;  let b = 2
来源：http://adc.quarkkingdee.top

[T18] Swift：字符串插值
来源：http://rqe.redwolf501.top

"值: \(b)"
来源：http://qrq.jiagoushi.top

[T19] Swift：可选绑定
来源：http://lez.cheryme.top

if let n = opt { print(n) }
来源：http://mkw.xuetiantiany.cn

[T20] Swift：数组操作
来源：http://isd.jianghu66.top

var a = [1, 2, 3];  a.append(4)
来源：http://ths.jqgfzy.top

[T21] Swift：遍历
来源：http://ieh.guannengcc.top

for x in a { print(x) }
来源：http://uyd.vehdjk.com

[T22] Swift：字典
来源：http://oxc.yj20258.top

var d = ["a": 1];  d["b"] = 2
来源：http://mqe.jiagoushi.top

[T23] Swift：函数
来源：http://xme.meibo888.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://knk.chenjidiqi.icu

[T24] Swift：闭包
来源：http://ukw.jinqigufen.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://nlt.sxryk.cn

[T25] Swift：结构体
来源：http://nuf.dianchejie.cn

struct P { var x: Int }
来源：http://upv.daria6918.cn

[T26] Swift：类与重写
来源：http://qbv.yj20258888.top

class A: Base { override func f() {} }
来源：http://kqw.nwbrower.top

[T27] Swift：错误处理
来源：http://ugs.hcnkem.com

do { try f() } catch { print(error) }
来源：http://aag.shuidangran.top

[T28] Swift：枚举
来源：http://qlc.bjfxy.top

enum Color { case red, green }
来源：http://syc.hammf.cn

[T29] Swift：guard 提前返回
来源：http://efb.xinyue.icu

guard let x = opt else { return }
来源：http://ozg.feifeiyinyue.top

[T30] Swift：协议
来源：http://jjp.aibaodan.cn

protocol Shape { func area() -> Double }
来源：http://xzm.shanyushiyangkeji.top

[T31] Lua：Hello World
来源：http://pwv.cashguo.top

print("Hello")
来源：http://mbz.fktsv.cn

[T32] Lua：局部变量
来源：http://kam.ctjpmb.com

local a = 1
来源：http://ukh.iojbl.cn

[T33] Lua：表（数组）
来源：http://cdk.9152youxi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://mjs.guowangkeji.top

[T34] Lua：遍历表
来源：http://hqo.haohaochexian.top

for i, v in ipairs(t) do print(i, v) end
来源：http://vpe.bbcook.cn

[T35] Lua：字典表
来源：http://pkp.zdbjq.cn

local d = { a = 1 };  d.b = 2
来源：http://otg.fanxiaobao.xyz

[T36] Lua：函数
来源：http://xnn.zycfv.cn

function add(a, b) return a + b end
来源：http://qcn.guannengcc.top

[T37] Lua：字符串拼接
来源：http://ktj.fehbvm.com

"a" .. "b"
来源：http://tdq.iojbl.cn

[T38] Lua：条件
来源：http://mis.zhengqikj.top

if x > 0 then print("正") end
来源：http://bnd.zdqjudy.top

[T39] Lua：模式匹配
来源：http://tde.xinyue.icu

string.find(s, "%d+")
来源：http://pxl.hongshengwenyu.top

[T40] Lua：元表
来源：http://bkc.epnwcf.com

setmetatable({}, { __index = base })
来源：http://oqu.yj20258888.top

[T41] Perl：Hello World
来源：http://gxz.cashguo.top

print "Hello\n";
来源：http://xcz.quarkkingdee.top

[T42] Perl：变量类型
来源：http://cxh.yangfankeji.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jkz.ydjk.org.cn

[T43] Perl：字符串插值
来源：http://ena.daria6918.cn

"值: $a"
来源：http://lgg.gzhubu.top

[T44] Perl：条件
来源：http://blp.cdnleiting.top

if ($a > 0) { print "正"; }
来源：http://yrv.iojbl.cn

[T45] Perl：数组遍历
来源：http://ljx.chenjidiqi.icu

for my $x (@arr) { print $x; }
来源：http://onm.gzhubu.top

[T46] Perl：哈希操作
来源：http://usj.meibo888.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ndw.cucudq.cn

[T47] Perl：正则捕获
来源：http://cvb.daria6918.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ivo.haohaochexian.top

[T48] Perl：正则替换
来源：http://ifn.sjlbkw.cn

$s =~ s/old/new/g;
来源：http://guz.xinyue.icu

[T49] Perl：函数
来源：http://spk.dianchejie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://asi.iojbl.cn

[T50] Perl：逐行读文件
来源：http://tsw.aibaodan.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://row.zycfv.cn

while (my $line = <$fh>) { print $line; }
来源：http://ubf.xuetiantiany.cn

[T51] Scala：Hello World
来源：http://evf.ehwqpu.com

println("Hello")
来源：http://mpm.cdnleiting.top

[T52] Scala：变量
来源：http://ulb.tarul.cn

val a = 1;  var b = 2
来源：http://kew.chenlongwang.top

[T53] Scala：字符串插值
来源：http://wxq.snrcjt.cn

s"值: $b"
来源：http://drl.vqdsnc.cn

[T54] Scala：集合映射
来源：http://oos.yvedp.cn

List(1, 2, 3).map(_ * 2)
来源：http://tfg.tian-w.cn

[T55] Scala：集合过滤
来源：http://gxj.xinyue.icu

List(1, 2, 3).filter(_ > 1)
来源：http://ths.zhoulong.xyz

[T56] Scala：样例类
来源：http://nqm.tarul.cn

case class User(name: String, age: Int)
来源：http://juj.cqqwz.cn

[T57] Scala：模式匹配
来源：http://cvt.ywan-chungtsiang.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://bvj.sufxvd.cn

[T58] Scala：函数定义
来源：http://crn.fengsongda.top

def add(a: Int, b: Int): Int = a + b
来源：http://yrz.aibaodan.cn

[T59] Scala：循环
来源：http://qvm.chenlongwang.top

for (i <- 1 to 10) println(i)
来源：http://jmc.feifeiyinyue.top

[T60] Scala：折叠
来源：http://njp.smart0.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vht.hfpthk.cn

================================================================================
来源：http://ggd.bjfxy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://laq.birdmap.top

================================================================================
来源：http://oxd.jqgfzy.top

[U01] Py：创建虚拟环境
来源：http://bgd.guannengcc.top

python -m venv .venv && source .venv/bin/activate
来源：http://fni.xinyue.icu

[U02] Py：导出 / 安装依赖
来源：http://bjo.hfpthk.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rut.jlsjyb.cn

[U03] Py：加载 .env 配置
来源：http://mbb.svipenyu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://zfi.fanxiaobao.xyz

[U04] Py：变量调试打印
来源：http://npl.yuxming.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ybk.ywan-chungtsiang.top

[U05] Py：列表去重且保序
来源：http://ogd.nanxuanxn.top

list(dict.fromkeys(arr))
来源：http://cri.cqqwz.cn

[U06] Py：合并两个字典
来源：http://lbz.zhongyouzk.top

{**a, **b}
来源：http://xvr.fzhhl.top

[U07] Py：反转字典键值
来源：http://blq.ivvv.top

{v: k for k, v in d.items()}
来源：http://xdm.xuanzx.com

[U08] Py：展平二维列表
来源：http://ywg.nanxuanxn.top

[y for x in nested for y in x]
来源：http://pci.yvedp.cn

[U09] Py：字典取最大值的键
来源：http://woy.cashguo.top

max(d, key=d.get)
来源：http://rep.yj202588.top

[U10] Py：按值排序字典
来源：http://qxv.sweek.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vco.chenjidiqi.icu

[U11] Py：生成器表达式
来源：http://huu.hongshengwenyu.top

(x * 2 for x in arr)
来源：http://pmo.52xcode.cn

[U12] Py：取出现最多的 3 个元素
来源：http://pmd.wangshuangyany.cn

Counter(arr).most_common(3)
来源：http://tim.sxryk.cn

[U13] Py：固定长度队列
来源：http://kby.chenjidiqi.icu

deque(maxlen=10)
来源：http://hmr.zhijiandao.cn

[U14] Py：分组收集到列表
来源：http://vrn.tianlin.xyz

defaultdict(list)
来源：http://lid.gaohongyu789.top

[U15] Py：高精度计时
来源：http://pvb.zhengqikj.top

t = time.perf_counter()
来源：http://zvu.zycfv.cn

[U16] Py：命令行参数解析
来源：http://hiq.wangdashe.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bnw.zdqjudy.top

[U17] Py：初始化日志
来源：http://cqc.bbcook.cn

logging.basicConfig(level=logging.INFO)
来源：http://lgj.jinyuanbaomall.cn

[U18] Py：预编译正则
来源：http://zly.zhijiandao.cn

pat = re.compile(r"\d+")
来源：http://hbq.yuxming.cn

[U19] Py：正则替换带回调
来源：http://rxn.jlsjyb.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tfi.guannengcc.top

[U20] Py：缓存函数结果
来源：http://vvh.zhijiandao.cn

@functools.lru_cache(maxsize=None)
来源：http://efd.nanxuanxn.top

[U21] Py：自定义上下文管理器
来源：http://pvi.aibaodan.cn

@contextlib.contextmanager
来源：http://cpi.gogol.net.cn

[U22] Py：矩阵转置
来源：http://aly.gaohongyu789.top

list(zip(*m))
来源：http://vuk.fzhhl.top

[U23] Py：分块读取大文件
来源：http://adk.0kj1m.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rjt.iojbl.cn

[U24] Py：路径操作
来源：http://nct.ivvv.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wyw.ppjwa.cn

[U25] Py：CSV 按字典读
来源：http://cis.hongshengwenyu.top

csv.DictReader(f)
来源：http://geh.snrcjt.cn

[U26] Py：并发下载
来源：http://nsb.feifeiyinyue.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ayk.yj20258888.top

[U27] Py：异步 HTTP
来源：http://ccb.daxiang520.top

aiohttp.ClientSession() 配合 async with
来源：http://ald.epnwcf.com

[U28] Py：类型别名
来源：http://thb.redwolf501.top

UserId = int
来源：http://xoo.tarul.cn

[U29] Py：属性校验
来源：http://zsz.yonumen.top

@property 与 @x.setter 配合
来源：http://adr.vehdjk.com

[U30] Py：数据类
来源：http://bgn.nanxuanxn.top

@dataclass(slots=True)
来源：http://uyy.jinyuanbaomall.cn

[U31] Py：单测
来源：http://xrl.ppjwa.cn

python -m pytest -q
来源：http://jno.shuidangran.top

[U32] Py：代码格式化
来源：http://wje.hesvh.cn

ruff format . && ruff check --fix .
来源：http://nxw.pengpengdd.cyou

[U33] Py：打包发布
来源：http://pxl.xinyue.icu

python -m build  （依赖 pyproject.toml）
来源：http://exf.tianlin.xyz

[U34] Py：判断编码
来源：http://roz.nanxuanxn.top

chardet.detect(raw)
来源：http://ybz.c1oappe.top

[U35] Py：发送邮件
来源：http://wcc.xuetiantiany.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lin.jianghu66.top

[U36] Py：定时任务
来源：http://tvk.hnqzz.top

schedule.every(10).minutes.do(job)
来源：http://zxq.sjlbkw.cn

[U37] Py：读写 Excel
来源：http://snj.ydjk.org.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ugf.cheryme.top

[U38] Py：获取脚本所在目录
来源：http://miw.yvedp.cn

Path(__file__).resolve().parent
来源：http://ywh.hesvh.cn

[U39] Py：判断是否在交互环境
来源：http://cwd.nwbrower.top

sys.stdout.isatty()
来源：http://yll.zycfv.cn

[U40] Py：打印到标准错误
来源：http://mst.yj20258888.top

print("err", file=sys.stderr)
来源：http://bls.jinqigfzy.top

[U41] PHP：初始化 Composer 项目
来源：http://rxy.nanxinkj.top

composer init;  composer require guzzlehttp/guzzle
来源：http://evu.xinyue.icu

[U42] PHP：PSR-4 自动加载
来源：http://xog.svipenyu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cqn.hysaishi.cn

[U43] PHP：声明命名空间
来源：http://pwz.9152youxi.cn

namespace App\Http;
来源：http://gje.smart0.xyz

[U44] PHP：开启严格类型
来源：http://rkl.mhx1999.top

declare(strict_types=1);
来源：http://gfd.xylfe.cn

[U45] PHP：类型声明与返回类型
来源：http://owh.shanyushiyangtech.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://kdd.haohaochexian.top

[U46] PHP：可空类型
来源：http://war.fengsongda.top

?string $name = null
来源：http://jql.nwbrower.top

[U47] PHP：联合类型
来源：http://oef.sweek.top

int|string $id
来源：http://xto.yuxming.cn

[U48] PHP：纯枚举
来源：http://uwk.yj20258888.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://rpo.chenzaomai.com

[U49] PHP：只读属性
来源：http://uup.havefunace.top

public readonly string $name
来源：http://iwl.shzxlz.cn

[U50] PHP：构造器属性提升
来源：http://nbp.aizwys.cn

public function __construct(private int $id) {}
来源：http://tkj.havefunace.top

[U51] PHP：数组解构
来源：http://dab.cdnleiting.top

[$a, $b] = $arr;
来源：http://vka.hongshengwenyu.top

[U52] PHP：箭头函数
来源：http://wsc.svipenyu.cn

$double = fn($x) => $x * 2;
来源：http://hjb.hysaishi.cn

[U53] PHP：空合并运算符
来源：http://xjz.c1oappe.top

$v = $a ?? $b ?? "default";
来源：http://rxe.hongshengwenyu.top

[U54] PHP：空安全调用
来源：http://jva.fzhhl.top

$obj?->method()
来源：http://rwq.fktsv.cn

[U55] PHP：match 表达式
来源：http://wrq.c1oappe.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ffn.shanyushiyangtech.top

[U56] PHP：命名参数
来源：http://isd.shzxlz.cn

f(a: 1, b: 2)
来源：http://lyi.yonumen.top

[U57] PHP：字符串插值
来源：http://ahz.xuetiantiany.cn

"值: {$a}"
来源：http://jep.c1oappe.top

[U58] PHP：数组三件套
来源：http://ftw.bjfxy.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tcy.tian-w.cn

[U59] PHP：自定义排序
来源：http://cpp.yj20258.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uzb.aizwys.cn

[U60] PHP：JSON 编解码
来源：http://qjj.jlsjyb.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vrl.yongpay.top

[U61] PHP：正则
来源：http://nqg.dianchejie.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://itw.zhaomingkeji.xyz

[U62] PHP：日期对象
来源：http://ilg.yj20258888.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://cjg.zhijiandao.cn

[U63] PHP：文件读写
来源：http://wdz.guowangkeji.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ste.nanxuanxn.top

[U64] PHP：目录遍历
来源：http://fkc.xuetiantiany.cn

glob("dir/*.php");  scandir("dir");
来源：http://wuq.svipenyu.cn

[U65] PHP：会话
来源：http://ohf.gzhubu.top

session_start();  $_SESSION["uid"] = 1;
来源：http://ilo.quarkkingdee.top

[U66] PHP：设置 Cookie
来源：http://wfh.zhiwuduotai.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pfr.sysykeji.top

[U67] PHP：处理文件上传
来源：http://fyb.yuanzhike.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lvj.fengsongda.top

[U68] PHP：PDO 连接
来源：http://eau.mhx1999.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://qft.9152youxi.cn

[U69] PHP：PDO 预处理
来源：http://hrm.gogol.net.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zcd.zycfv.cn

[U70] PHP：PDO 事务
来源：http://sot.nwbrower.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dgu.cheryme.top

[U71] PHP：抛出异常
来源：http://ckw.kuanghao11.cn

throw new RuntimeException("失败", 500);
来源：http://dhq.zhaomingkeji.xyz

[U72] PHP：写错误日志
来源：http://rqs.snrcjt.cn

error_log("失败: " . $e->getMessage());
来源：http://qlb.shangyingyoupin.top

[U73] PHP：读取 ini 配置
来源：http://tsw.yfazqb.com

parse_ini_file("config.ini", true)
来源：http://icu.zycfv.cn

[U74] PHP：读取环境变量
来源：http://fig.meibo888.top

getenv("APP_ENV") ?: "production"
来源：http://cku.yuxming.cn

[U75] PHP：依赖注入
来源：http://zup.guowangkeji.top

composer require psr/container
来源：http://szq.aibaodan.cn

[U76] PHP：简单路由
来源：http://mjx.zhongyouzk.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rlv.dashuyun.cn

[U77] PHP：模板渲染
来源：http://urc.wangdashe.top

composer require twig/twig
来源：http://dkw.yj202588.top

[U78] PHP：单元测试
来源：http://edh.svipenyu.cn

composer require --dev phpunit/phpunit
来源：http://eio.jiagoushi.top

[U79] PHP：静态分析
来源：http://zqr.ehwqpu.com

composer require --dev phpstan/phpstan
来源：http://sbt.ehwqpu.com

[U80] PHP：代码规范修复
来源：http://tji.zdbjq.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://chr.jiagoushi.top

[U81] JS：初始化项目
来源：http://rqy.meibo888.top

npm init -y;  npm i express
来源：http://tkx.daxiang520.top

[U82] JS：package.json 脚本
来源：http://nzc.vqdsnc.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nwm.smart0.xyz


<!-- 参考信息 -->