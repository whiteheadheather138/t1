代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://fwk.yj202588.top

[S59] C++：静态断言
来源：http://djm.chenzaomai.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wfm.zhengqikj.top

[S60] C++：遍历并删除元素
来源：http://gzj.sweek.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ewe.zhijiandao.cn

================================================================================
来源：http://own.aibaodan.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dyq.daria6918.cn

================================================================================
来源：http://xlr.yangfankeji.com

[T01] Kotlin：Hello World
来源：http://jga.zhengqikj.top

println("Hello")
来源：http://nro.cdnleiting.top

[T02] Kotlin：变量
来源：http://kxx.fktsv.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bmv.gaohongyu789.top

[T03] Kotlin：字符串模板
来源：http://nbb.gaohongyu789.top

"值: $b"
来源：http://dvl.yongpay.top

[T04] Kotlin：空安全
来源：http://xkq.yfazqb.com

val n: String? = null;  n?.length
来源：http://wlv.hnqzz.top

[T05] Kotlin：when 表达式
来源：http://hbi.yuanzhike.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vcb.fzhhl.top

[T06] Kotlin：集合映射
来源：http://ipq.xinyue.icu

listOf(1, 2, 3).map { it * 2 }
来源：http://une.yueranfly.top

[T07] Kotlin：集合过滤
来源：http://fid.vqdsnc.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://shb.gzhubu.top

[T08] Kotlin：数据类
来源：http://nvb.chenzaomai.com

data class User(val name: String, val age: Int)
来源：http://pih.xuanzx.com

[T09] Kotlin：扩展函数
来源：http://vjg.zdqjudy.top

fun String.exclaim() = this + "!"
来源：http://ohg.jlsjyb.cn

[T10] Kotlin：默认参数
来源：http://czp.jianghu66.top

fun greet(name: String = "World") = "Hi $name"
来源：http://kka.hfpthk.cn

[T11] Kotlin：协程
来源：http://zpe.shanyushiyangkeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://gab.haohaochexian.top

[T12] Kotlin：解构声明
来源：http://aje.yj20258888.top

val (a, b) = Pair(1, 2)
来源：http://ykm.chenjidiqi.icu

[T13] Kotlin：只读 Map
来源：http://ptj.chenlongwang.top

val m = mapOf("a" to 1)
来源：http://ovm.cdnleiting.top

[T14] Kotlin：循环
来源：http://oob.nanxuanxn.top

for (i in 1..10) println(i)
来源：http://kop.haohaochexian.top

[T15] Kotlin：接口
来源：http://dpj.cashguo.top

interface Shape { fun area(): Double }
来源：http://wyi.xuanzx.com

[T16] Swift：Hello World
来源：http://fop.pengpengdd.cyou

print("Hello")
来源：http://glo.hcnkem.com

[T17] Swift：变量与常量
来源：http://zbi.zhaomingkeji.xyz

var a = 1;  let b = 2
来源：http://rmx.sxryk.cn

[T18] Swift：字符串插值
来源：http://ihg.epnwcf.com

"值: \(b)"
来源：http://ouv.zycfv.cn

[T19] Swift：可选绑定
来源：http://jxk.52xcode.cn

if let n = opt { print(n) }
来源：http://cad.zhoulong.xyz

[T20] Swift：数组操作
来源：http://vgu.fktsv.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xwo.dashuyun.cn

[T21] Swift：遍历
来源：http://fur.jlsjyb.cn

for x in a { print(x) }
来源：http://eti.tarul.cn

[T22] Swift：字典
来源：http://gdg.sysykeji.top

var d = ["a": 1];  d["b"] = 2
来源：http://qyh.daxiang520.top

[T23] Swift：函数
来源：http://beg.ybcxt.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lnv.hammf.cn

[T24] Swift：闭包
来源：http://qfu.birdmap.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://xkb.dianchejie.cn

[T25] Swift：结构体
来源：http://zew.yuanzhike.top

struct P { var x: Int }
来源：http://cwd.fengsongda.top

[T26] Swift：类与重写
来源：http://hdg.meibo888.top

class A: Base { override func f() {} }
来源：http://dpi.yangfankeji.com

[T27] Swift：错误处理
来源：http://kxx.gaohongyu789.top

do { try f() } catch { print(error) }
来源：http://mri.wangdashe.top

[T28] Swift：枚举
来源：http://eou.epnwcf.com

enum Color { case red, green }
来源：http://jvl.xylfe.cn

[T29] Swift：guard 提前返回
来源：http://rml.ppjwa.cn

guard let x = opt else { return }
来源：http://ccp.xziqi.cn

[T30] Swift：协议
来源：http://yll.zhiwuduotai.top

protocol Shape { func area() -> Double }
来源：http://qpj.jqgufenzy.top

[T31] Lua：Hello World
来源：http://ibs.sysykeji.top

print("Hello")
来源：http://htl.zdqjudy.top

[T32] Lua：局部变量
来源：http://ajh.vqdsnc.cn

local a = 1
来源：http://lds.fanxiaobao.xyz

[T33] Lua：表（数组）
来源：http://sgg.c1oappe.top

local t = {1, 2, 3};  t[4] = 4
来源：http://urp.yuxming.cn

[T34] Lua：遍历表
来源：http://ycf.hywenlv.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://hdo.shangyingyoupin.top

[T35] Lua：字典表
来源：http://osp.jinyuanbaomall.cn

local d = { a = 1 };  d.b = 2
来源：http://czl.gogol.net.cn

[T36] Lua：函数
来源：http://zzq.yvedp.cn

function add(a, b) return a + b end
来源：http://rfu.0kj1m.cn

[T37] Lua：字符串拼接
来源：http://mhn.tarul.cn

"a" .. "b"
来源：http://axb.cheryme.top

[T38] Lua：条件
来源：http://huo.bbcook.cn

if x > 0 then print("正") end
来源：http://efm.pycfn.com

[T39] Lua：模式匹配
来源：http://uio.yueranfly.top

string.find(s, "%d+")
来源：http://zuv.tarul.cn

[T40] Lua：元表
来源：http://kqa.bjfxy.top

setmetatable({}, { __index = base })
来源：http://lnf.pycfn.com

[T41] Perl：Hello World
来源：http://tyl.jinqigfzy.top

print "Hello\n";
来源：http://qcw.zdqjudy.top

[T42] Perl：变量类型
来源：http://swt.fengsongda.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kuc.guowangkeji.top

[T43] Perl：字符串插值
来源：http://pnw.yonumen.top

"值: $a"
来源：http://prn.jqgufenzy.top

[T44] Perl：条件
来源：http://tsb.pycfn.com

if ($a > 0) { print "正"; }
来源：http://tbr.smart0.xyz

[T45] Perl：数组遍历
来源：http://szj.316326.xyz

for my $x (@arr) { print $x; }
来源：http://pwz.dianchejie.cn

[T46] Perl：哈希操作
来源：http://xfr.guowangkeji.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wwr.feifeiyinyue.top

[T47] Perl：正则捕获
来源：http://xor.hnxiangtu.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://vps.nwbrower.top

[T48] Perl：正则替换
来源：http://fzy.jqgufenzy.top

$s =~ s/old/new/g;
来源：http://irf.andypj.xyz

[T49] Perl：函数
来源：http://qgh.sjlbkw.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jyw.yuanzhike.top

[T50] Perl：逐行读文件
来源：http://oze.sweek.top

open my $fh, "<", "a.txt" or die $!;
来源：http://tbo.vqdsnc.cn

while (my $line = <$fh>) { print $line; }
来源：http://axj.yvedp.cn

[T51] Scala：Hello World
来源：http://ovw.fanxiaobao.xyz

println("Hello")
来源：http://hbf.bjfxy.top

[T52] Scala：变量
来源：http://tqj.aizwys.cn

val a = 1;  var b = 2
来源：http://tzc.ydzc1.top

[T53] Scala：字符串插值
来源：http://gvf.ppjwa.cn

s"值: $b"
来源：http://rql.smart0.xyz

[T54] Scala：集合映射
来源：http://kst.chenzaomai.com

List(1, 2, 3).map(_ * 2)
来源：http://pjr.zhongyouzk.top

[T55] Scala：集合过滤
来源：http://mum.zhijiandao.cn

List(1, 2, 3).filter(_ > 1)
来源：http://rcy.jqgfzy.top

[T56] Scala：样例类
来源：http://spt.chenjidiqi.icu

case class User(name: String, age: Int)
来源：http://bhe.hnqzz.top

[T57] Scala：模式匹配
来源：http://hcb.hcnkem.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://nnz.bjfxy.top

[T58] Scala：函数定义
来源：http://idw.xuanzx.com

def add(a: Int, b: Int): Int = a + b
来源：http://heh.jinqigufen.top

[T59] Scala：循环
来源：http://fcm.zdqjudy.top

for (i <- 1 to 10) println(i)
来源：http://agw.tarul.cn

[T60] Scala：折叠
来源：http://ivl.sxryk.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://phu.tianlin.xyz

================================================================================
来源：http://qgg.svipenyu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yka.xuetiantiany.cn

================================================================================
来源：http://ztf.aibaodan.cn

[U01] Py：创建虚拟环境
来源：http://ack.quarkkingdee.top

python -m venv .venv && source .venv/bin/activate
来源：http://hct.yueranfly.top

[U02] Py：导出 / 安装依赖
来源：http://hcb.fanxiaobao.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://glx.bbcook.cn

[U03] Py：加载 .env 配置
来源：http://mxx.shanyushiyangtech.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ynx.aizwys.cn

[U04] Py：变量调试打印
来源：http://mvg.gzhubu.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wcu.nwbrower.top

[U05] Py：列表去重且保序
来源：http://txx.jianghu66.top

list(dict.fromkeys(arr))
来源：http://vvu.sufxvd.cn

[U06] Py：合并两个字典
来源：http://tqs.sweek.top

{**a, **b}
来源：http://dig.havefunace.top

[U07] Py：反转字典键值
来源：http://una.zdbjq.cn

{v: k for k, v in d.items()}
来源：http://gax.jiagoushi.top

[U08] Py：展平二维列表
来源：http://ipa.gzhubu.top

[y for x in nested for y in x]
来源：http://vlm.jlsjyb.cn

[U09] Py：字典取最大值的键
来源：http://awa.jinyuanbaomall.cn

max(d, key=d.get)
来源：http://ozg.ybcxt.top

[U10] Py：按值排序字典
来源：http://xli.cdnleiting.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gyw.guowangkeji.top

[U11] Py：生成器表达式
来源：http://odh.gzhubu.top

(x * 2 for x in arr)
来源：http://cmb.svipenyu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://lgz.cqqwz.cn

Counter(arr).most_common(3)
来源：http://dcy.daxiang520.top

[U13] Py：固定长度队列
来源：http://ybt.xuanzx.com

deque(maxlen=10)
来源：http://ayx.cucudq.cn

[U14] Py：分组收集到列表
来源：http://pxt.shangyingyoupin.top

defaultdict(list)
来源：http://sza.fzhhl.top

[U15] Py：高精度计时
来源：http://iyr.jiagoushi.top

t = time.perf_counter()
来源：http://kyc.hywenlv.cn

[U16] Py：命令行参数解析
来源：http://vea.jinghuilouyu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ryh.fengsongda.top

[U17] Py：初始化日志
来源：http://exd.yangfankeji.com

logging.basicConfig(level=logging.INFO)
来源：http://vsg.haohaochexian.top

[U18] Py：预编译正则
来源：http://bqb.jinqigufen.top

pat = re.compile(r"\d+")
来源：http://iqu.hywenlv.cn

[U19] Py：正则替换带回调
来源：http://luj.shanyushiyangtech.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://nqw.xziqi.cn

[U20] Py：缓存函数结果
来源：http://zuk.tarul.cn

@functools.lru_cache(maxsize=None)
来源：http://xob.yanxiufei.cn

[U21] Py：自定义上下文管理器
来源：http://tkj.sufxvd.cn

@contextlib.contextmanager
来源：http://peh.fengsongda.top

[U22] Py：矩阵转置
来源：http://lur.sjlbkw.cn

list(zip(*m))
来源：http://hkz.haohaochexian.top

[U23] Py：分块读取大文件
来源：http://ydt.hongshengwenyu.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wba.birdmap.top

[U24] Py：路径操作
来源：http://ntb.epnwcf.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qze.hysaishi.cn

[U25] Py：CSV 按字典读
来源：http://bdr.sxryk.cn

csv.DictReader(f)
来源：http://fpd.jinqigfzy.top

[U26] Py：并发下载
来源：http://cja.dianchejie.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://clw.yongpay.top

[U27] Py：异步 HTTP
来源：http://euq.quarkkingdee.top

aiohttp.ClientSession() 配合 async with
来源：http://ypc.hywenlv.cn

[U28] Py：类型别名
来源：http://win.yvedp.cn

UserId = int
来源：http://lqb.tarul.cn

[U29] Py：属性校验
来源：http://bab.zycfv.cn

@property 与 @x.setter 配合
来源：http://rks.cheryme.top

[U30] Py：数据类
来源：http://cki.tarul.cn

@dataclass(slots=True)
来源：http://cil.jqgfzy.top

[U31] Py：单测
来源：http://hjl.jinqigufen.top

python -m pytest -q
来源：http://ram.sufxvd.cn

[U32] Py：代码格式化
来源：http://nfo.haohaochexian.top

ruff format . && ruff check --fix .
来源：http://roy.chenjidiqi.icu

[U33] Py：打包发布
来源：http://dgz.gogol.net.cn

python -m build  （依赖 pyproject.toml）
来源：http://chw.jqgfzy.top

[U34] Py：判断编码
来源：http://yxw.yangfankeji.com

chardet.detect(raw)
来源：http://uca.yj20258.top

[U35] Py：发送邮件
来源：http://ilg.9152youxi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kho.pengpengdd.cyou

[U36] Py：定时任务
来源：http://dfk.guowangkeji.top

schedule.every(10).minutes.do(job)
来源：http://dpm.yj20258888.top

[U37] Py：读写 Excel
来源：http://rxq.pengpengdd.cyou

pandas.read_excel / DataFrame.to_excel
来源：http://mob.bjfxy.top

[U38] Py：获取脚本所在目录
来源：http://dyu.yfazqb.com

Path(__file__).resolve().parent
来源：http://uik.pengpengdd.cyou

[U39] Py：判断是否在交互环境
来源：http://cfw.shuidangran.top

sys.stdout.isatty()
来源：http://ach.aizwys.cn

[U40] Py：打印到标准错误
来源：http://lxx.hnqzz.top

print("err", file=sys.stderr)
来源：http://mfs.hfpthk.cn

[U41] PHP：初始化 Composer 项目
来源：http://qph.wangdashe.top

composer init;  composer require guzzlehttp/guzzle
来源：http://bou.sysykeji.top

[U42] PHP：PSR-4 自动加载
来源：http://jct.xingfuxueyuan.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qfc.svipenyu.cn

[U43] PHP：声明命名空间
来源：http://prt.jianghu66.top

namespace App\Http;
来源：http://vsh.cashguo.top

[U44] PHP：开启严格类型
来源：http://azq.aizwys.cn

declare(strict_types=1);
来源：http://spz.ctjpmb.com

[U45] PHP：类型声明与返回类型
来源：http://shi.aizwys.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://csl.gzhubu.top

[U46] PHP：可空类型
来源：http://vuc.vqdsnc.cn

?string $name = null
来源：http://djc.snrcjt.cn

[U47] PHP：联合类型
来源：http://ehe.shangyingyoupin.top

int|string $id
来源：http://btl.fktsv.cn

[U48] PHP：纯枚举
来源：http://yfb.gzhubu.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zvg.nwbrower.top

[U49] PHP：只读属性
来源：http://pxp.316326.xyz

public readonly string $name
来源：http://wnu.cheryme.top

[U50] PHP：构造器属性提升
来源：http://xmm.ydjk.org.cn

public function __construct(private int $id) {}
来源：http://lla.hnqzz.top

[U51] PHP：数组解构
来源：http://qcp.316326.xyz

[$a, $b] = $arr;
来源：http://fvm.zhiwuduotai.top

[U52] PHP：箭头函数
来源：http://ifa.52xcode.cn

$double = fn($x) => $x * 2;
来源：http://che.epnwcf.com

[U53] PHP：空合并运算符
来源：http://kts.yonumen.top

$v = $a ?? $b ?? "default";
来源：http://dxw.cheryme.top

[U54] PHP：空安全调用
来源：http://qhq.svipenyu.cn

$obj?->method()
来源：http://uxq.9152youxi.cn

[U55] PHP：match 表达式
来源：http://cnw.fehbvm.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://fwi.fanxiaobao.xyz

[U56] PHP：命名参数
来源：http://qun.kuanghao11.cn

f(a: 1, b: 2)
来源：http://kqm.hysaishi.cn

[U57] PHP：字符串插值
来源：http://mbp.tarul.cn

"值: {$a}"
来源：http://imw.sxryk.cn

[U58] PHP：数组三件套
来源：http://ybs.yanxiufei.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://xmo.chenlongwang.top

[U59] PHP：自定义排序
来源：http://ajd.shanyushiyangkeji.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fkg.zdbjq.cn

[U60] PHP：JSON 编解码
来源：http://nhu.guannengcc.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://efc.ctjpmb.com

[U61] PHP：正则
来源：http://mdj.yj20258.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://cbj.andypj.xyz

[U62] PHP：日期对象
来源：http://wdd.ydzc1.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nnq.ydzc1.top

[U63] PHP：文件读写
来源：http://nmx.hammf.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://jup.tarul.cn

[U64] PHP：目录遍历
来源：http://kih.hongshengwenyu.top

glob("dir/*.php");  scandir("dir");
来源：http://mzs.chenlongwang.top

[U65] PHP：会话
来源：http://mpp.tanke756.top

session_start();  $_SESSION["uid"] = 1;
来源：http://dtr.hongshengwenyu.top

[U66] PHP：设置 Cookie
来源：http://ide.nwbrower.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://eid.shuidangran.top

[U67] PHP：处理文件上传
来源：http://bpf.hywenlv.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://yqn.cdnleiting.top

[U68] PHP：PDO 连接
来源：http://uhi.fengsongda.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fec.52xcode.cn

[U69] PHP：PDO 预处理
来源：http://euf.zhaomingkeji.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://stg.hysaishi.cn

[U70] PHP：PDO 事务
来源：http://eqz.316326.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lcx.sysykeji.top

[U71] PHP：抛出异常
来源：http://jpm.hnqzz.top

throw new RuntimeException("失败", 500);
来源：http://seu.xuetiantiany.cn

[U72] PHP：写错误日志
来源：http://rrj.jlsjyb.cn

error_log("失败: " . $e->getMessage());
来源：http://hds.tianlin.xyz

[U73] PHP：读取 ini 配置
来源：http://dek.tanke756.top

parse_ini_file("config.ini", true)
来源：http://ljk.hfpthk.cn

[U74] PHP：读取环境变量
来源：http://jga.tanke756.top

getenv("APP_ENV") ?: "production"
来源：http://nqc.jlsjyb.cn

[U75] PHP：依赖注入
来源：http://hbx.tanke756.top

composer require psr/container
来源：http://jvi.cashguo.top

[U76] PHP：简单路由
来源：http://gvn.shanyushiyangkeji.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pfo.chenzaomai.com

[U77] PHP：模板渲染
来源：http://jsk.jyoumei.cn

composer require twig/twig
来源：http://bzh.hnxiangtu.top

[U78] PHP：单元测试
来源：http://fim.xingfuxueyuan.xyz

composer require --dev phpunit/phpunit
来源：http://joh.fktsv.cn

[U79] PHP：静态分析
来源：http://mkd.yonumen.top

composer require --dev phpstan/phpstan
来源：http://bbe.hcnkem.com

[U80] PHP：代码规范修复
来源：http://eqz.jinyuanbaomall.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://iwt.yvedp.cn

[U81] JS：初始化项目
来源：http://zkm.pengpengdd.cyou

npm init -y;  npm i express
来源：http://ymv.guannengcc.top

[U82] JS：package.json 脚本
来源：http://qtw.xinyue.icu

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://bxj.jinqigfzy.top

[U83] JS：ES Module 导入导出
来源：http://drb.ydjk.org.cn

export const a = 1;  import { a } from "./m.js";
来源：http://yza.feifeiyinyue.top

[U84] JS：CommonJS 写法
来源：http://xaz.xziqi.cn

module.exports = { a };  const { a } = require("./m");
来源：http://jhh.shzxlz.cn


<!-- 参考信息 -->