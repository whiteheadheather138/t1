代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ssr.sxryk.cn

================================================================================
来源：http://nhr.jinghuilouyu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bny.wangdashe.top

================================================================================
来源：http://vnm.andypj.xyz

[T01] Kotlin：Hello World
来源：http://fcu.ppjwa.cn

println("Hello")
来源：http://pjd.daxiang520.top

[T02] Kotlin：变量
来源：http://rim.fanxiaobao.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://awh.andypj.xyz

[T03] Kotlin：字符串模板
来源：http://nhk.zdqjudy.top

"值: $b"
来源：http://tjx.vehdjk.com

[T04] Kotlin：空安全
来源：http://prx.xuetiantiany.cn

val n: String? = null;  n?.length
来源：http://aou.c1oappe.top

[T05] Kotlin：when 表达式
来源：http://bxx.guowangkeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jzk.haohaochexian.top

[T06] Kotlin：集合映射
来源：http://vwj.smart0.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://dgx.nanxuanxn.top

[T07] Kotlin：集合过滤
来源：http://uut.yuanzhike.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://djh.gotoacloud.top

[T08] Kotlin：数据类
来源：http://xec.nanxinkj.top

data class User(val name: String, val age: Int)
来源：http://qbv.fanxiaobao.xyz

[T09] Kotlin：扩展函数
来源：http://fkm.tian-w.cn

fun String.exclaim() = this + "!"
来源：http://emh.hammf.cn

[T10] Kotlin：默认参数
来源：http://xun.yvedp.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rhv.cashguo.top

[T11] Kotlin：协程
来源：http://qly.hfpthk.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://fss.vehdjk.com

[T12] Kotlin：解构声明
来源：http://grg.yonumen.top

val (a, b) = Pair(1, 2)
来源：http://qzu.zdbjq.cn

[T13] Kotlin：只读 Map
来源：http://msm.zhongyouzk.top

val m = mapOf("a" to 1)
来源：http://xfz.jinghuilouyu.cn

[T14] Kotlin：循环
来源：http://klx.52xcode.cn

for (i in 1..10) println(i)
来源：http://ohx.yuxming.cn

[T15] Kotlin：接口
来源：http://csc.zhoulong.xyz

interface Shape { fun area(): Double }
来源：http://xda.pengpengdd.cyou

[T16] Swift：Hello World
来源：http://vbg.ctjpmb.com

print("Hello")
来源：http://plk.gotoacloud.top

[T17] Swift：变量与常量
来源：http://azb.sjlbkw.cn

var a = 1;  let b = 2
来源：http://qmd.chenjidiqi.icu

[T18] Swift：字符串插值
来源：http://vys.shangyingyoupin.top

"值: \(b)"
来源：http://luf.jinqigufen.top

[T19] Swift：可选绑定
来源：http://epl.haohaochexian.top

if let n = opt { print(n) }
来源：http://krh.xinyue.icu

[T20] Swift：数组操作
来源：http://dlw.cheryme.top

var a = [1, 2, 3];  a.append(4)
来源：http://ssv.hammf.cn

[T21] Swift：遍历
来源：http://jjt.shuidangran.top

for x in a { print(x) }
来源：http://rwe.pengpengdd.cyou

[T22] Swift：字典
来源：http://lmb.tian-w.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zmq.ivvv.top

[T23] Swift：函数
来源：http://cuc.tarul.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://aly.hongshengwenyu.top

[T24] Swift：闭包
来源：http://giu.vqdsnc.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://kak.zdqjudy.top

[T25] Swift：结构体
来源：http://kdi.hesvh.cn

struct P { var x: Int }
来源：http://uys.hcnkem.com

[T26] Swift：类与重写
来源：http://vzx.gotoacloud.top

class A: Base { override func f() {} }
来源：http://kqg.cdnleiting.top

[T27] Swift：错误处理
来源：http://thm.chenlongwang.top

do { try f() } catch { print(error) }
来源：http://jfv.yongpay.top

[T28] Swift：枚举
来源：http://ieq.yj20258888.top

enum Color { case red, green }
来源：http://dhw.pycfn.com

[T29] Swift：guard 提前返回
来源：http://zvp.sjlbkw.cn

guard let x = opt else { return }
来源：http://kve.nanxuanxn.top

[T30] Swift：协议
来源：http://afm.ybcxt.top

protocol Shape { func area() -> Double }
来源：http://agp.meibo888.top

[T31] Lua：Hello World
来源：http://slu.ppjwa.cn

print("Hello")
来源：http://ydv.daria6918.cn

[T32] Lua：局部变量
来源：http://pjt.xziqi.cn

local a = 1
来源：http://vhc.daria6918.cn

[T33] Lua：表（数组）
来源：http://bif.hnqzz.top

local t = {1, 2, 3};  t[4] = 4
来源：http://obs.yj20258.top

[T34] Lua：遍历表
来源：http://pcd.jinghuilouyu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://fkp.ydjk.org.cn

[T35] Lua：字典表
来源：http://esf.smart0.xyz

local d = { a = 1 };  d.b = 2
来源：http://gkd.jinqigufen.top

[T36] Lua：函数
来源：http://dvb.jiagoushi.top

function add(a, b) return a + b end
来源：http://dwq.gaohongyu789.top

[T37] Lua：字符串拼接
来源：http://zzc.sysykeji.top

"a" .. "b"
来源：http://brr.cashguo.top

[T38] Lua：条件
来源：http://izq.xziqi.cn

if x > 0 then print("正") end
来源：http://zfc.jqgufenzy.top

[T39] Lua：模式匹配
来源：http://alq.sweek.top

string.find(s, "%d+")
来源：http://kee.hnqzz.top

[T40] Lua：元表
来源：http://ast.shangyingyoupin.top

setmetatable({}, { __index = base })
来源：http://jap.yangfankeji.com

[T41] Perl：Hello World
来源：http://rtk.ybcxt.top

print "Hello\n";
来源：http://ktc.meibo888.top

[T42] Perl：变量类型
来源：http://dtv.hfpthk.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jrg.ivvv.top

[T43] Perl：字符串插值
来源：http://rhz.hcnkem.com

"值: $a"
来源：http://obj.hongshengwenyu.top

[T44] Perl：条件
来源：http://kuf.nwbrower.top

if ($a > 0) { print "正"; }
来源：http://gjz.yvedp.cn

[T45] Perl：数组遍历
来源：http://eqk.aibaodan.cn

for my $x (@arr) { print $x; }
来源：http://evz.fehbvm.com

[T46] Perl：哈希操作
来源：http://cyo.fzhhl.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nsq.gotoacloud.top

[T47] Perl：正则捕获
来源：http://etm.tianlin.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://pwg.snrcjt.cn

[T48] Perl：正则替换
来源：http://krc.bbcook.cn

$s =~ s/old/new/g;
来源：http://cgo.tarul.cn

[T49] Perl：函数
来源：http://fdm.hywenlv.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rhm.tianlin.xyz

[T50] Perl：逐行读文件
来源：http://ciu.fktsv.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://lsx.sysykeji.top

while (my $line = <$fh>) { print $line; }
来源：http://amj.epnwcf.com

[T51] Scala：Hello World
来源：http://brc.daxiang520.top

println("Hello")
来源：http://cfg.ehwqpu.com

[T52] Scala：变量
来源：http://kbq.hammf.cn

val a = 1;  var b = 2
来源：http://zku.vehdjk.com

[T53] Scala：字符串插值
来源：http://vpj.hammf.cn

s"值: $b"
来源：http://kpv.yvedp.cn

[T54] Scala：集合映射
来源：http://mnr.fanxiaobao.xyz

List(1, 2, 3).map(_ * 2)
来源：http://nuk.ywan-chungtsiang.top

[T55] Scala：集合过滤
来源：http://ojn.zhijiandao.cn

List(1, 2, 3).filter(_ > 1)
来源：http://hnl.fanxiaobao.xyz

[T56] Scala：样例类
来源：http://adu.sufxvd.cn

case class User(name: String, age: Int)
来源：http://zzb.ctjpmb.com

[T57] Scala：模式匹配
来源：http://ibu.sysykeji.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://igv.hywenlv.cn

[T58] Scala：函数定义
来源：http://eqe.yj202588.top

def add(a: Int, b: Int): Int = a + b
来源：http://ivv.cucudq.cn

[T59] Scala：循环
来源：http://ryg.52xcode.cn

for (i <- 1 to 10) println(i)
来源：http://syl.uphjek.com

[T60] Scala：折叠
来源：http://zcs.hnqzz.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://seg.jiagoushi.top

================================================================================
来源：http://gug.wangshuangyany.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bsk.meibo888.top

================================================================================
来源：http://zte.c1oappe.top

[U01] Py：创建虚拟环境
来源：http://iwj.quarkkingdee.top

python -m venv .venv && source .venv/bin/activate
来源：http://lak.ywan-chungtsiang.top

[U02] Py：导出 / 安装依赖
来源：http://bsr.nanxuanxn.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xxx.pycfn.com

[U03] Py：加载 .env 配置
来源：http://rjm.zhiwuduotai.top

from dotenv import load_dotenv; load_dotenv()
来源：http://qgd.shanyushiyangkeji.top

[U04] Py：变量调试打印
来源：http://pnq.daxiang520.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ema.tianlin.xyz

[U05] Py：列表去重且保序
来源：http://bra.xuanzx.com

list(dict.fromkeys(arr))
来源：http://zpi.nanxinkj.top

[U06] Py：合并两个字典
来源：http://sbc.zhiwuduotai.top

{**a, **b}
来源：http://lnk.fktsv.cn

[U07] Py：反转字典键值
来源：http://czi.guowangkeji.top

{v: k for k, v in d.items()}
来源：http://foe.jinqigufen.top

[U08] Py：展平二维列表
来源：http://fhk.sysykeji.top

[y for x in nested for y in x]
来源：http://bva.gaohongyu789.top

[U09] Py：字典取最大值的键
来源：http://xmx.c1oappe.top

max(d, key=d.get)
来源：http://xvl.shzxlz.cn

[U10] Py：按值排序字典
来源：http://twn.jqgufenzy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pve.yongpay.top

[U11] Py：生成器表达式
来源：http://pto.yj20258.top

(x * 2 for x in arr)
来源：http://dry.hesvh.cn

[U12] Py：取出现最多的 3 个元素
来源：http://sad.zycfv.cn

Counter(arr).most_common(3)
来源：http://led.xinyue.icu

[U13] Py：固定长度队列
来源：http://rnt.fehbvm.com

deque(maxlen=10)
来源：http://lmb.yj20258.top

[U14] Py：分组收集到列表
来源：http://rgq.daria6918.cn

defaultdict(list)
来源：http://ryc.sweek.top

[U15] Py：高精度计时
来源：http://vzc.tarul.cn

t = time.perf_counter()
来源：http://fkh.jianghu66.top

[U16] Py：命令行参数解析
来源：http://vkw.hfpthk.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fpt.zhixingplan.top

[U17] Py：初始化日志
来源：http://lqm.guowangkeji.top

logging.basicConfig(level=logging.INFO)
来源：http://plm.uphjek.com

[U18] Py：预编译正则
来源：http://abq.shuidangran.top

pat = re.compile(r"\d+")
来源：http://yyx.chenlongwang.top

[U19] Py：正则替换带回调
来源：http://qxp.tanke756.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yzj.bbcook.cn

[U20] Py：缓存函数结果
来源：http://dju.jianghu66.top

@functools.lru_cache(maxsize=None)
来源：http://xvu.nwbrower.top

[U21] Py：自定义上下文管理器
来源：http://xho.xylfe.cn

@contextlib.contextmanager
来源：http://aof.ywan-chungtsiang.top

[U22] Py：矩阵转置
来源：http://iyc.9152youxi.cn

list(zip(*m))
来源：http://yls.ehwqpu.com

[U23] Py：分块读取大文件
来源：http://ozl.fehbvm.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://yfm.yueranfly.top

[U24] Py：路径操作
来源：http://flj.hcnkem.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kwu.zhaomingkeji.xyz

[U25] Py：CSV 按字典读
来源：http://soz.ctjpmb.com

csv.DictReader(f)
来源：http://iwd.yongpay.top

[U26] Py：并发下载
来源：http://hwy.fzhhl.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zga.havefunace.top

[U27] Py：异步 HTTP
来源：http://nhv.zdqjudy.top

aiohttp.ClientSession() 配合 async with
来源：http://sdo.52xcode.cn

[U28] Py：类型别名
来源：http://tmn.zhaomingkeji.xyz

UserId = int
来源：http://cob.yanxiufei.cn

[U29] Py：属性校验
来源：http://cqo.xziqi.cn

@property 与 @x.setter 配合
来源：http://exh.hcnkem.com

[U30] Py：数据类
来源：http://bty.zdbjq.cn

@dataclass(slots=True)
来源：http://mzb.yuxming.cn

[U31] Py：单测
来源：http://xdn.vehdjk.com

python -m pytest -q
来源：http://cez.c1oappe.top

[U32] Py：代码格式化
来源：http://ewf.sjlbkw.cn

ruff format . && ruff check --fix .
来源：http://fsa.jqgfzy.top

[U33] Py：打包发布
来源：http://spa.jqgfzy.top

python -m build  （依赖 pyproject.toml）
来源：http://rqd.jiagoushi.top

[U34] Py：判断编码
来源：http://vnu.pengpengdd.cyou

chardet.detect(raw)
来源：http://snm.zhoulong.xyz

[U35] Py：发送邮件
来源：http://xgv.yueranfly.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://eef.52xcode.cn

[U36] Py：定时任务
来源：http://vue.shanyushiyangkeji.top

schedule.every(10).minutes.do(job)
来源：http://aqs.jlsjyb.cn

[U37] Py：读写 Excel
来源：http://waa.meibo888.top

pandas.read_excel / DataFrame.to_excel
来源：http://zdv.fehbvm.com

[U38] Py：获取脚本所在目录
来源：http://ffp.vqdsnc.cn

Path(__file__).resolve().parent
来源：http://czx.hfpthk.cn

[U39] Py：判断是否在交互环境
来源：http://mzg.xuanzx.com

sys.stdout.isatty()
来源：http://goe.shangyingyoupin.top

[U40] Py：打印到标准错误
来源：http://qsa.guowangkeji.top

print("err", file=sys.stderr)
来源：http://adn.chenjidiqi.icu

[U41] PHP：初始化 Composer 项目
来源：http://wco.jianghu66.top

composer init;  composer require guzzlehttp/guzzle
来源：http://epg.xziqi.cn

[U42] PHP：PSR-4 自动加载
来源：http://see.xuanzx.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://owv.tarul.cn

[U43] PHP：声明命名空间
来源：http://ivi.zdbjq.cn

namespace App\Http;
来源：http://nij.jyoumei.cn

[U44] PHP：开启严格类型
来源：http://dtf.aibaodan.cn

declare(strict_types=1);
来源：http://igx.zhaomingkeji.xyz

[U45] PHP：类型声明与返回类型
来源：http://fhq.nwbrower.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ish.jinghuilouyu.cn

[U46] PHP：可空类型
来源：http://psr.hnxiangtu.top

?string $name = null
来源：http://dsg.nanxinkj.top

[U47] PHP：联合类型
来源：http://pgh.c1oappe.top

int|string $id
来源：http://nmo.zhaomingkeji.xyz

[U48] PHP：纯枚举
来源：http://eip.shangyingyoupin.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tvu.cqqwz.cn

[U49] PHP：只读属性
来源：http://ioi.zycfv.cn

public readonly string $name
来源：http://ngp.9152youxi.cn

[U50] PHP：构造器属性提升
来源：http://vba.yueranfly.top

public function __construct(private int $id) {}
来源：http://ubr.jianghu66.top

[U51] PHP：数组解构
来源：http://hcj.feifeiyinyue.top

[$a, $b] = $arr;
来源：http://fpc.tarul.cn

[U52] PHP：箭头函数
来源：http://lcq.ydzc1.top

$double = fn($x) => $x * 2;
来源：http://nxv.jinqigfzy.top

[U53] PHP：空合并运算符
来源：http://myl.dianchejie.cn

$v = $a ?? $b ?? "default";
来源：http://xog.zdqjudy.top

[U54] PHP：空安全调用
来源：http://wiz.tanke756.top

$obj?->method()
来源：http://ndm.gotoacloud.top

[U55] PHP：match 表达式
来源：http://klq.jinqigfzy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://luo.hnxiangtu.top

[U56] PHP：命名参数
来源：http://zcy.hongshengwenyu.top

f(a: 1, b: 2)
来源：http://tdi.hongshengwenyu.top

[U57] PHP：字符串插值
来源：http://tad.shuidangran.top

"值: {$a}"
来源：http://gdm.epnwcf.com

[U58] PHP：数组三件套
来源：http://qhl.zhixingplan.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zma.cdnleiting.top

[U59] PHP：自定义排序
来源：http://hux.fzhhl.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bvf.uphjek.com

[U60] PHP：JSON 编解码
来源：http://wml.gzhubu.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://bqr.zhixingplan.top

[U61] PHP：正则
来源：http://nvd.uphjek.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://leg.wangdashe.top

[U62] PHP：日期对象
来源：http://slo.ivvv.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jxl.tarul.cn

[U63] PHP：文件读写
来源：http://nhw.aibaodan.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://lvg.zhoulong.xyz

[U64] PHP：目录遍历
来源：http://isg.bjfxy.top

glob("dir/*.php");  scandir("dir");
来源：http://qlo.yj20258.top

[U65] PHP：会话
来源：http://dol.quarkkingdee.top

session_start();  $_SESSION["uid"] = 1;
来源：http://kht.dianchejie.cn

[U66] PHP：设置 Cookie
来源：http://uxs.yuanzhike.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qrv.fktsv.cn

[U67] PHP：处理文件上传
来源：http://qzj.cheryme.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pnl.nwbrower.top

[U68] PHP：PDO 连接
来源：http://mhp.chenzaomai.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ash.fengsongda.top

[U69] PHP：PDO 预处理
来源：http://tdj.jinqigfzy.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rso.tian-w.cn

[U70] PHP：PDO 事务
来源：http://djw.ybcxt.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://cxu.fanxiaobao.xyz

[U71] PHP：抛出异常
来源：http://xtc.feifeiyinyue.top

throw new RuntimeException("失败", 500);
来源：http://dze.chenzaomai.com

[U72] PHP：写错误日志
来源：http://duh.chenjidiqi.icu

error_log("失败: " . $e->getMessage());
来源：http://dnq.yj202588.top

[U73] PHP：读取 ini 配置
来源：http://xri.haohaochexian.top

parse_ini_file("config.ini", true)
来源：http://zip.zhiwuduotai.top

[U74] PHP：读取环境变量
来源：http://fss.ivvv.top

getenv("APP_ENV") ?: "production"
来源：http://mna.guowangkeji.top

[U75] PHP：依赖注入
来源：http://nzo.haohaochexian.top

composer require psr/container
来源：http://ybt.fengsongda.top

[U76] PHP：简单路由
来源：http://ino.0kj1m.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://izn.vqdsnc.cn

[U77] PHP：模板渲染
来源：http://yiq.jqgufenzy.top

composer require twig/twig
来源：http://anf.cheryme.top

[U78] PHP：单元测试
来源：http://ioo.yangfankeji.com

composer require --dev phpunit/phpunit
来源：http://aib.bbcook.cn

[U79] PHP：静态分析
来源：http://nqe.zhaomingkeji.xyz

composer require --dev phpstan/phpstan
来源：http://gpg.snrcjt.cn

[U80] PHP：代码规范修复
来源：http://sby.sysykeji.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://lby.hesvh.cn

[U81] JS：初始化项目
来源：http://cjh.hysaishi.cn

npm init -y;  npm i express
来源：http://zvl.tianlin.xyz

[U82] JS：package.json 脚本
来源：http://eic.vqdsnc.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wry.tarul.cn

[U83] JS：ES Module 导入导出
来源：http://xfj.daria6918.cn

export const a = 1;  import { a } from "./m.js";
来源：http://zjr.kuanghao11.cn

[U84] JS：CommonJS 写法
来源：http://fdt.snrcjt.cn

module.exports = { a };  const { a } = require("./m");
来源：http://lip.gotoacloud.top

[U85] JS：可选链
来源：http://fqn.sufxvd.cn

a?.b?.c
来源：http://lzk.zhijiandao.cn

[U86] JS：空值合并
来源：http://ljp.quarkkingdee.top

a ?? b
来源：http://nub.vqdsnc.cn


<!-- 参考信息 -->