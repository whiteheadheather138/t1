代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://eqp.ivvv.top

[S59] C++：静态断言
来源：http://ejk.tarul.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fgt.jinyuanbaomall.cn

[S60] C++：遍历并删除元素
来源：http://wun.ywan-chungtsiang.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bhf.guowangkeji.top

================================================================================
来源：http://soh.xuetiantiany.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rvs.meibo888.top

================================================================================
来源：http://kmz.shanyushiyangkeji.top

[T01] Kotlin：Hello World
来源：http://gce.jiagoushi.top

println("Hello")
来源：http://vbf.xuetiantiany.cn

[T02] Kotlin：变量
来源：http://wfq.shuidangran.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ywr.cqqwz.cn

[T03] Kotlin：字符串模板
来源：http://hkr.jqgfzy.top

"值: $b"
来源：http://fcn.zhaomingkeji.xyz

[T04] Kotlin：空安全
来源：http://boe.c1oappe.top

val n: String? = null;  n?.length
来源：http://rwq.shangyingyoupin.top

[T05] Kotlin：when 表达式
来源：http://rzd.hnqzz.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mca.hfpthk.cn

[T06] Kotlin：集合映射
来源：http://zux.fktsv.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://flx.ydzc1.top

[T07] Kotlin：集合过滤
来源：http://mij.shangyingyoupin.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://rcu.daria6918.cn

[T08] Kotlin：数据类
来源：http://bhw.shanyushiyangkeji.top

data class User(val name: String, val age: Int)
来源：http://sef.aibaodan.cn

[T09] Kotlin：扩展函数
来源：http://ggk.dashuyun.cn

fun String.exclaim() = this + "!"
来源：http://rgo.yvedp.cn

[T10] Kotlin：默认参数
来源：http://mju.shuidangran.top

fun greet(name: String = "World") = "Hi $name"
来源：http://fgb.shangyingyoupin.top

[T11] Kotlin：协程
来源：http://ykv.shanyushiyangtech.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://gtw.daxiang520.top

[T12] Kotlin：解构声明
来源：http://cxd.sxryk.cn

val (a, b) = Pair(1, 2)
来源：http://mvb.52xcode.cn

[T13] Kotlin：只读 Map
来源：http://uun.dashuyun.cn

val m = mapOf("a" to 1)
来源：http://dmz.hfpthk.cn

[T14] Kotlin：循环
来源：http://naz.wangdashe.top

for (i in 1..10) println(i)
来源：http://lfw.yuanzhike.top

[T15] Kotlin：接口
来源：http://oiv.dianchejie.cn

interface Shape { fun area(): Double }
来源：http://obe.gzhubu.top

[T16] Swift：Hello World
来源：http://yul.yvedp.cn

print("Hello")
来源：http://abh.shuidangran.top

[T17] Swift：变量与常量
来源：http://yzd.wangdashe.top

var a = 1;  let b = 2
来源：http://thy.gaohongyu789.top

[T18] Swift：字符串插值
来源：http://ccb.sjlbkw.cn

"值: \(b)"
来源：http://lff.yanxiufei.cn

[T19] Swift：可选绑定
来源：http://hdd.xylfe.cn

if let n = opt { print(n) }
来源：http://cim.shangyingyoupin.top

[T20] Swift：数组操作
来源：http://ifm.sjlbkw.cn

var a = [1, 2, 3];  a.append(4)
来源：http://kyx.hammf.cn

[T21] Swift：遍历
来源：http://gek.jinyuanbaomall.cn

for x in a { print(x) }
来源：http://qfe.ybcxt.top

[T22] Swift：字典
来源：http://tzm.cucudq.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ekt.shangyingyoupin.top

[T23] Swift：函数
来源：http://cco.hcnkem.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mlx.tanke756.top

[T24] Swift：闭包
来源：http://zru.fengsongda.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://yxb.gaohongyu789.top

[T25] Swift：结构体
来源：http://qez.shanyushiyangkeji.top

struct P { var x: Int }
来源：http://wqq.sxryk.cn

[T26] Swift：类与重写
来源：http://nao.ppjwa.cn

class A: Base { override func f() {} }
来源：http://bft.hcnkem.com

[T27] Swift：错误处理
来源：http://icx.ctjpmb.com

do { try f() } catch { print(error) }
来源：http://nhz.zhixingplan.top

[T28] Swift：枚举
来源：http://smh.vehdjk.com

enum Color { case red, green }
来源：http://dqa.yj20258.top

[T29] Swift：guard 提前返回
来源：http://gvv.gogol.net.cn

guard let x = opt else { return }
来源：http://rxx.shuidangran.top

[T30] Swift：协议
来源：http://wak.birdmap.top

protocol Shape { func area() -> Double }
来源：http://jbu.shzxlz.cn

[T31] Lua：Hello World
来源：http://taf.tanke756.top

print("Hello")
来源：http://pgo.yueranfly.top

[T32] Lua：局部变量
来源：http://azy.xuetiantiany.cn

local a = 1
来源：http://vwn.yj20258888.top

[T33] Lua：表（数组）
来源：http://tiv.hysaishi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ubu.jlsjyb.cn

[T34] Lua：遍历表
来源：http://tkg.yangfankeji.com

for i, v in ipairs(t) do print(i, v) end
来源：http://kgp.andypj.xyz

[T35] Lua：字典表
来源：http://bkk.xingfuxueyuan.xyz

local d = { a = 1 };  d.b = 2
来源：http://bhf.kuanghao11.cn

[T36] Lua：函数
来源：http://oli.aibaodan.cn

function add(a, b) return a + b end
来源：http://lml.zdqjudy.top

[T37] Lua：字符串拼接
来源：http://jpu.feifeiyinyue.top

"a" .. "b"
来源：http://nvq.yuanzhike.top

[T38] Lua：条件
来源：http://iol.zhaomingkeji.xyz

if x > 0 then print("正") end
来源：http://yfe.tian-w.cn

[T39] Lua：模式匹配
来源：http://bsx.yongpay.top

string.find(s, "%d+")
来源：http://zny.fzhhl.top

[T40] Lua：元表
来源：http://vqe.havefunace.top

setmetatable({}, { __index = base })
来源：http://ovd.chenlongwang.top

[T41] Perl：Hello World
来源：http://jpu.tian-w.cn

print "Hello\n";
来源：http://lmj.xinyue.icu

[T42] Perl：变量类型
来源：http://zlx.quarkkingdee.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qaj.feifeiyinyue.top

[T43] Perl：字符串插值
来源：http://yam.sysykeji.top

"值: $a"
来源：http://gfy.cdnleiting.top

[T44] Perl：条件
来源：http://dvz.tianlin.xyz

if ($a > 0) { print "正"; }
来源：http://azv.smart0.xyz

[T45] Perl：数组遍历
来源：http://mtd.shanyushiyangtech.top

for my $x (@arr) { print $x; }
来源：http://wnv.hnqzz.top

[T46] Perl：哈希操作
来源：http://qgl.cdnleiting.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sqr.guowangkeji.top

[T47] Perl：正则捕获
来源：http://fzh.zhengqikj.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://img.snrcjt.cn

[T48] Perl：正则替换
来源：http://rag.0kj1m.cn

$s =~ s/old/new/g;
来源：http://utp.yuxming.cn

[T49] Perl：函数
来源：http://yls.jinqigufen.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rvj.havefunace.top

[T50] Perl：逐行读文件
来源：http://uzl.zhongyouzk.top

open my $fh, "<", "a.txt" or die $!;
来源：http://qid.sjlbkw.cn

while (my $line = <$fh>) { print $line; }
来源：http://knc.gogol.net.cn

[T51] Scala：Hello World
来源：http://mcp.gaohongyu789.top

println("Hello")
来源：http://vgl.zhijiandao.cn

[T52] Scala：变量
来源：http://ytj.yuxming.cn

val a = 1;  var b = 2
来源：http://vbq.bbcook.cn

[T53] Scala：字符串插值
来源：http://oqn.yuanzhike.top

s"值: $b"
来源：http://zum.yj20258888.top

[T54] Scala：集合映射
来源：http://tdj.xylfe.cn

List(1, 2, 3).map(_ * 2)
来源：http://nhl.yj20258888.top

[T55] Scala：集合过滤
来源：http://obs.cheryme.top

List(1, 2, 3).filter(_ > 1)
来源：http://not.nanxuanxn.top

[T56] Scala：样例类
来源：http://giq.cdnleiting.top

case class User(name: String, age: Int)
来源：http://ntx.shanyushiyangtech.top

[T57] Scala：模式匹配
来源：http://cvb.hcnkem.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://eou.iojbl.cn

[T58] Scala：函数定义
来源：http://rjd.tianlin.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://chb.jqgufenzy.top

[T59] Scala：循环
来源：http://wtn.jinqigfzy.top

for (i <- 1 to 10) println(i)
来源：http://rhh.gogol.net.cn

[T60] Scala：折叠
来源：http://pla.ywan-chungtsiang.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tbt.jqgfzy.top

================================================================================
来源：http://qlq.gotoacloud.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://iay.ehwqpu.com

================================================================================
来源：http://tto.feifeiyinyue.top

[U01] Py：创建虚拟环境
来源：http://xct.havefunace.top

python -m venv .venv && source .venv/bin/activate
来源：http://num.hfpthk.cn

[U02] Py：导出 / 安装依赖
来源：http://exw.xziqi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pwi.haohaochexian.top

[U03] Py：加载 .env 配置
来源：http://ijk.cdnleiting.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ldj.kuanghao11.cn

[U04] Py：变量调试打印
来源：http://ipr.hesvh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://chc.vehdjk.com

[U05] Py：列表去重且保序
来源：http://ata.quarkkingdee.top

list(dict.fromkeys(arr))
来源：http://lsa.ehwqpu.com

[U06] Py：合并两个字典
来源：http://una.yj20258.top

{**a, **b}
来源：http://orr.smart0.xyz

[U07] Py：反转字典键值
来源：http://qcd.vqdsnc.cn

{v: k for k, v in d.items()}
来源：http://fbg.tian-w.cn

[U08] Py：展平二维列表
来源：http://ihy.wangshuangyany.cn

[y for x in nested for y in x]
来源：http://bhj.gaohongyu789.top

[U09] Py：字典取最大值的键
来源：http://dzj.yfazqb.com

max(d, key=d.get)
来源：http://jiw.dianchejie.cn

[U10] Py：按值排序字典
来源：http://vgn.zhixingplan.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vbe.tarul.cn

[U11] Py：生成器表达式
来源：http://zia.xziqi.cn

(x * 2 for x in arr)
来源：http://uma.ctjpmb.com

[U12] Py：取出现最多的 3 个元素
来源：http://vdz.hywenlv.cn

Counter(arr).most_common(3)
来源：http://pae.52xcode.cn

[U13] Py：固定长度队列
来源：http://jxx.yj20258.top

deque(maxlen=10)
来源：http://keg.uphjek.com

[U14] Py：分组收集到列表
来源：http://klv.gotoacloud.top

defaultdict(list)
来源：http://svh.jinghuilouyu.cn

[U15] Py：高精度计时
来源：http://yng.fktsv.cn

t = time.perf_counter()
来源：http://hiz.hnqzz.top

[U16] Py：命令行参数解析
来源：http://pqe.zhaomingkeji.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jvi.yj202588.top

[U17] Py：初始化日志
来源：http://ovf.wangdashe.top

logging.basicConfig(level=logging.INFO)
来源：http://adr.fehbvm.com

[U18] Py：预编译正则
来源：http://qku.ivvv.top

pat = re.compile(r"\d+")
来源：http://xep.zdbjq.cn

[U19] Py：正则替换带回调
来源：http://mkt.xziqi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lcm.0kj1m.cn

[U20] Py：缓存函数结果
来源：http://gmx.yongpay.top

@functools.lru_cache(maxsize=None)
来源：http://ulh.jianghu66.top

[U21] Py：自定义上下文管理器
来源：http://bwd.jianghu66.top

@contextlib.contextmanager
来源：http://otq.havefunace.top

[U22] Py：矩阵转置
来源：http://zch.jinqigfzy.top

list(zip(*m))
来源：http://kcw.0kj1m.cn

[U23] Py：分块读取大文件
来源：http://tba.zhaomingkeji.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ikp.havefunace.top

[U24] Py：路径操作
来源：http://ayn.fehbvm.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gug.fengsongda.top

[U25] Py：CSV 按字典读
来源：http://yrn.fengsongda.top

csv.DictReader(f)
来源：http://xei.hysaishi.cn

[U26] Py：并发下载
来源：http://zjd.sysykeji.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wln.shzxlz.cn

[U27] Py：异步 HTTP
来源：http://ydt.nanxinkj.top

aiohttp.ClientSession() 配合 async with
来源：http://tdg.316326.xyz

[U28] Py：类型别名
来源：http://icr.quarkkingdee.top

UserId = int
来源：http://ghr.zdqjudy.top

[U29] Py：属性校验
来源：http://lmx.iojbl.cn

@property 与 @x.setter 配合
来源：http://zma.haohaochexian.top

[U30] Py：数据类
来源：http://sxe.zhoulong.xyz

@dataclass(slots=True)
来源：http://cye.sxryk.cn

[U31] Py：单测
来源：http://mpu.wangdashe.top

python -m pytest -q
来源：http://sve.gaohongyu789.top

[U32] Py：代码格式化
来源：http://ilf.nanxuanxn.top

ruff format . && ruff check --fix .
来源：http://hyd.cdnleiting.top

[U33] Py：打包发布
来源：http://oiz.hnxiangtu.top

python -m build  （依赖 pyproject.toml）
来源：http://mvd.xingfuxueyuan.xyz

[U34] Py：判断编码
来源：http://goc.hcnkem.com

chardet.detect(raw)
来源：http://bnz.shuidangran.top

[U35] Py：发送邮件
来源：http://sis.zhiwuduotai.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nwi.316326.xyz

[U36] Py：定时任务
来源：http://xqq.shzxlz.cn

schedule.every(10).minutes.do(job)
来源：http://erx.zhongyouzk.top

[U37] Py：读写 Excel
来源：http://kty.chenlongwang.top

pandas.read_excel / DataFrame.to_excel
来源：http://nsc.pengpengdd.cyou

[U38] Py：获取脚本所在目录
来源：http://vxl.pengpengdd.cyou

Path(__file__).resolve().parent
来源：http://vmw.gogol.net.cn

[U39] Py：判断是否在交互环境
来源：http://qah.hongshengwenyu.top

sys.stdout.isatty()
来源：http://epy.fzhhl.top

[U40] Py：打印到标准错误
来源：http://dmc.xuanzx.com

print("err", file=sys.stderr)
来源：http://qzl.tianlin.xyz

[U41] PHP：初始化 Composer 项目
来源：http://mvo.daxiang520.top

composer init;  composer require guzzlehttp/guzzle
来源：http://igj.ivvv.top

[U42] PHP：PSR-4 自动加载
来源：http://xrb.svipenyu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zro.ctjpmb.com

[U43] PHP：声明命名空间
来源：http://hyb.yj202588.top

namespace App\Http;
来源：http://del.gotoacloud.top

[U44] PHP：开启严格类型
来源：http://xpk.guannengcc.top

declare(strict_types=1);
来源：http://mcq.zhengqikj.top

[U45] PHP：类型声明与返回类型
来源：http://mzh.bbcook.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://zlh.hcnkem.com

[U46] PHP：可空类型
来源：http://sgz.pycfn.com

?string $name = null
来源：http://tzq.tian-w.cn

[U47] PHP：联合类型
来源：http://jry.yj202588.top

int|string $id
来源：http://fto.hcnkem.com

[U48] PHP：纯枚举
来源：http://yus.jinqigufen.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dhm.zycfv.cn

[U49] PHP：只读属性
来源：http://tnc.bjfxy.top

public readonly string $name
来源：http://nnh.cqqwz.cn

[U50] PHP：构造器属性提升
来源：http://zha.yuxming.cn

public function __construct(private int $id) {}
来源：http://xgt.shangyingyoupin.top

[U51] PHP：数组解构
来源：http://awf.redwolf501.top

[$a, $b] = $arr;
来源：http://haw.jlsjyb.cn

[U52] PHP：箭头函数
来源：http://npz.jyoumei.cn

$double = fn($x) => $x * 2;
来源：http://hre.316326.xyz

[U53] PHP：空合并运算符
来源：http://miw.fehbvm.com

$v = $a ?? $b ?? "default";
来源：http://zas.fktsv.cn

[U54] PHP：空安全调用
来源：http://hly.yj20258.top

$obj?->method()
来源：http://zqm.cdnleiting.top

[U55] PHP：match 表达式
来源：http://fqn.yuanzhike.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://xdf.zhongyouzk.top

[U56] PHP：命名参数
来源：http://vcp.chenjidiqi.icu

f(a: 1, b: 2)
来源：http://kdn.jianghu66.top

[U57] PHP：字符串插值
来源：http://goe.zhiwuduotai.top

"值: {$a}"
来源：http://juf.ppjwa.cn

[U58] PHP：数组三件套
来源：http://tye.yanxiufei.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xyo.jlsjyb.cn

[U59] PHP：自定义排序
来源：http://vya.gotoacloud.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zvr.sysykeji.top

[U60] PHP：JSON 编解码
来源：http://ilu.svipenyu.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://omb.chenjidiqi.icu

[U61] PHP：正则
来源：http://hmr.yuanzhike.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ptz.xziqi.cn

[U62] PHP：日期对象
来源：http://abd.wangshuangyany.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://lzi.hongshengwenyu.top

[U63] PHP：文件读写
来源：http://led.c1oappe.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://zxm.hywenlv.cn

[U64] PHP：目录遍历
来源：http://pfr.smart0.xyz

glob("dir/*.php");  scandir("dir");
来源：http://tra.c1oappe.top

[U65] PHP：会话
来源：http://kym.fehbvm.com

session_start();  $_SESSION["uid"] = 1;
来源：http://huc.daria6918.cn

[U66] PHP：设置 Cookie
来源：http://kba.sweek.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://oex.ppjwa.cn

[U67] PHP：处理文件上传
来源：http://jxg.uphjek.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://anp.gaohongyu789.top

[U68] PHP：PDO 连接
来源：http://eno.yvedp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ypp.aizwys.cn

[U69] PHP：PDO 预处理
来源：http://llf.gotoacloud.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://ynj.guannengcc.top

[U70] PHP：PDO 事务
来源：http://gpu.yuxming.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://ucf.dianchejie.cn

[U71] PHP：抛出异常
来源：http://yny.ctjpmb.com

throw new RuntimeException("失败", 500);
来源：http://ryo.sysykeji.top

[U72] PHP：写错误日志
来源：http://end.yuanzhike.top

error_log("失败: " . $e->getMessage());
来源：http://aok.yuanzhike.top

[U73] PHP：读取 ini 配置
来源：http://bhi.snrcjt.cn

parse_ini_file("config.ini", true)
来源：http://gha.ybcxt.top

[U74] PHP：读取环境变量
来源：http://mix.yanxiufei.cn

getenv("APP_ENV") ?: "production"
来源：http://grl.zhixingplan.top

[U75] PHP：依赖注入
来源：http://jef.nanxinkj.top

composer require psr/container
来源：http://mux.ppjwa.cn

[U76] PHP：简单路由
来源：http://gyh.jinqigufen.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qaj.guannengcc.top

[U77] PHP：模板渲染
来源：http://jog.gzhubu.top

composer require twig/twig
来源：http://dze.zhengqikj.top

[U78] PHP：单元测试
来源：http://ryf.xuetiantiany.cn

composer require --dev phpunit/phpunit
来源：http://vng.316326.xyz

[U79] PHP：静态分析
来源：http://bbm.kuanghao11.cn

composer require --dev phpstan/phpstan
来源：http://zgq.pycfn.com

[U80] PHP：代码规范修复
来源：http://slw.jinqigfzy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://ymr.gzhubu.top

[U81] JS：初始化项目
来源：http://sys.shzxlz.cn

npm init -y;  npm i express
来源：http://vfu.hnqzz.top

[U82] JS：package.json 脚本
来源：http://tok.ctjpmb.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wxe.shangyingyoupin.top

[U83] JS：ES Module 导入导出
来源：http://lrx.jiagoushi.top

export const a = 1;  import { a } from "./m.js";
来源：http://ibk.shanyushiyangtech.top

[U84] JS：CommonJS 写法
来源：http://lzq.pengpengdd.cyou

module.exports = { a };  const { a } = require("./m");
来源：http://rqd.kuanghao11.cn


<!-- 参考信息 -->