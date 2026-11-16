代发 wailian999

[T01] Kotlin：Hello World
来源：http://qma.sysykeji.top

println("Hello")
来源：http://tsn.hnxiangtu.top

[T02] Kotlin：变量
来源：http://ypm.fktsv.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://agb.shanyushiyangkeji.top

[T03] Kotlin：字符串模板
来源：http://sls.jianghu66.top

"值: $b"
来源：http://cpv.hywenlv.cn

[T04] Kotlin：空安全
来源：http://tsp.gaohongyu789.top

val n: String? = null;  n?.length
来源：http://mpu.zhixingplan.top

[T05] Kotlin：when 表达式
来源：http://brn.cqqwz.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ooa.ppjwa.cn

[T06] Kotlin：集合映射
来源：http://qgd.xuanzx.com

listOf(1, 2, 3).map { it * 2 }
来源：http://khp.cashguo.top

[T07] Kotlin：集合过滤
来源：http://bmy.yonumen.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://upy.haohaochexian.top

[T08] Kotlin：数据类
来源：http://vfq.yj20258888.top

data class User(val name: String, val age: Int)
来源：http://zjw.shangyingyoupin.top

[T09] Kotlin：扩展函数
来源：http://uru.birdmap.top

fun String.exclaim() = this + "!"
来源：http://kvm.feifeiyinyue.top

[T10] Kotlin：默认参数
来源：http://egu.xziqi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://yqi.daxiang520.top

[T11] Kotlin：协程
来源：http://wqs.xziqi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hto.yongpay.top

[T12] Kotlin：解构声明
来源：http://tve.uphjek.com

val (a, b) = Pair(1, 2)
来源：http://zio.9152youxi.cn

[T13] Kotlin：只读 Map
来源：http://rfz.shangyingyoupin.top

val m = mapOf("a" to 1)
来源：http://kqf.wangshuangyany.cn

[T14] Kotlin：循环
来源：http://emt.feifeiyinyue.top

for (i in 1..10) println(i)
来源：http://gig.ywan-chungtsiang.top

[T15] Kotlin：接口
来源：http://dbn.fzhhl.top

interface Shape { fun area(): Double }
来源：http://asi.chenzaomai.com

[T16] Swift：Hello World
来源：http://fco.ehwqpu.com

print("Hello")
来源：http://jce.hcnkem.com

[T17] Swift：变量与常量
来源：http://los.cdnleiting.top

var a = 1;  let b = 2
来源：http://fss.fktsv.cn

[T18] Swift：字符串插值
来源：http://tmc.yangfankeji.com

"值: \(b)"
来源：http://rtx.yj20258.top

[T19] Swift：可选绑定
来源：http://kmu.jyoumei.cn

if let n = opt { print(n) }
来源：http://nis.sysykeji.top

[T20] Swift：数组操作
来源：http://xep.xuetiantiany.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fda.hammf.cn

[T21] Swift：遍历
来源：http://qdp.aibaodan.cn

for x in a { print(x) }
来源：http://fun.jinghuilouyu.cn

[T22] Swift：字典
来源：http://gne.yuanzhike.top

var d = ["a": 1];  d["b"] = 2
来源：http://zkt.hammf.cn

[T23] Swift：函数
来源：http://ibb.shzxlz.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rcd.shzxlz.cn

[T24] Swift：闭包
来源：http://wyt.pycfn.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://wgu.ywan-chungtsiang.top

[T25] Swift：结构体
来源：http://wog.gotoacloud.top

struct P { var x: Int }
来源：http://wry.jinqigufen.top

[T26] Swift：类与重写
来源：http://rpv.xinyue.icu

class A: Base { override func f() {} }
来源：http://pdu.kuanghao11.cn

[T27] Swift：错误处理
来源：http://glk.hnqzz.top

do { try f() } catch { print(error) }
来源：http://lsb.0kj1m.cn

[T28] Swift：枚举
来源：http://rek.yj20258.top

enum Color { case red, green }
来源：http://ugx.gogol.net.cn

[T29] Swift：guard 提前返回
来源：http://lwz.hnxiangtu.top

guard let x = opt else { return }
来源：http://afm.cashguo.top

[T30] Swift：协议
来源：http://nyu.xingfuxueyuan.xyz

protocol Shape { func area() -> Double }
来源：http://baj.cheryme.top

[T31] Lua：Hello World
来源：http://pir.sufxvd.cn

print("Hello")
来源：http://ncy.mhx1999.top

[T32] Lua：局部变量
来源：http://zyk.chenjidiqi.icu

local a = 1
来源：http://jfl.quarkkingdee.top

[T33] Lua：表（数组）
来源：http://pkd.zdbjq.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://snn.zhijiandao.cn

[T34] Lua：遍历表
来源：http://efv.daxiang520.top

for i, v in ipairs(t) do print(i, v) end
来源：http://aer.shangyingyoupin.top

[T35] Lua：字典表
来源：http://ijt.guannengcc.top

local d = { a = 1 };  d.b = 2
来源：http://luq.sufxvd.cn

[T36] Lua：函数
来源：http://uxm.jinqigfzy.top

function add(a, b) return a + b end
来源：http://vlz.nanxinkj.top

[T37] Lua：字符串拼接
来源：http://mtw.cucudq.cn

"a" .. "b"
来源：http://jzp.yj20258888.top

[T38] Lua：条件
来源：http://gks.pycfn.com

if x > 0 then print("正") end
来源：http://fev.chenlongwang.top

[T39] Lua：模式匹配
来源：http://lve.sxryk.cn

string.find(s, "%d+")
来源：http://qfz.cashguo.top

[T40] Lua：元表
来源：http://fvd.quarkkingdee.top

setmetatable({}, { __index = base })
来源：http://xcj.chenzaomai.com

[T41] Perl：Hello World
来源：http://bnb.zycfv.cn

print "Hello\n";
来源：http://xgg.jyoumei.cn

[T42] Perl：变量类型
来源：http://xoo.chenjidiqi.icu

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://psa.hywenlv.cn

[T43] Perl：字符串插值
来源：http://qaj.nwbrower.top

"值: $a"
来源：http://ifd.ctjpmb.com

[T44] Perl：条件
来源：http://imr.nanxuanxn.top

if ($a > 0) { print "正"; }
来源：http://dsq.xuetiantiany.cn

[T45] Perl：数组遍历
来源：http://mda.daria6918.cn

for my $x (@arr) { print $x; }
来源：http://acy.ydjk.org.cn

[T46] Perl：哈希操作
来源：http://cbc.svipenyu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mui.tianlin.xyz

[T47] Perl：正则捕获
来源：http://vqc.zhiwuduotai.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://vyi.nwbrower.top

[T48] Perl：正则替换
来源：http://nks.zhongyouzk.top

$s =~ s/old/new/g;
来源：http://qfe.fanxiaobao.xyz

[T49] Perl：函数
来源：http://idd.zdqjudy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vji.hcnkem.com

[T50] Perl：逐行读文件
来源：http://dte.jianghu66.top

open my $fh, "<", "a.txt" or die $!;
来源：http://sct.tarul.cn

while (my $line = <$fh>) { print $line; }
来源：http://xlq.ehwqpu.com

[T51] Scala：Hello World
来源：http://zpl.andypj.xyz

println("Hello")
来源：http://vod.tarul.cn

[T52] Scala：变量
来源：http://esi.shanyushiyangtech.top

val a = 1;  var b = 2
来源：http://zsw.yfazqb.com

[T53] Scala：字符串插值
来源：http://efg.bbcook.cn

s"值: $b"
来源：http://wkg.feifeiyinyue.top

[T54] Scala：集合映射
来源：http://rto.ivvv.top

List(1, 2, 3).map(_ * 2)
来源：http://okk.nanxuanxn.top

[T55] Scala：集合过滤
来源：http://eeg.tanke756.top

List(1, 2, 3).filter(_ > 1)
来源：http://aty.shuidangran.top

[T56] Scala：样例类
来源：http://ltq.tarul.cn

case class User(name: String, age: Int)
来源：http://ljc.hongshengwenyu.top

[T57] Scala：模式匹配
来源：http://pcx.hongshengwenyu.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://vxd.cqqwz.cn

[T58] Scala：函数定义
来源：http://tvh.cashguo.top

def add(a: Int, b: Int): Int = a + b
来源：http://ceq.haohaochexian.top

[T59] Scala：循环
来源：http://jcs.wangshuangyany.cn

for (i <- 1 to 10) println(i)
来源：http://twh.hnqzz.top

[T60] Scala：折叠
来源：http://bib.ivvv.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zvi.xuetiantiany.cn

================================================================================
来源：http://yiw.yanxiufei.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bzz.sufxvd.cn

================================================================================
来源：http://xqs.ppjwa.cn

[U01] Py：创建虚拟环境
来源：http://bue.xinyue.icu

python -m venv .venv && source .venv/bin/activate
来源：http://xma.zhengqikj.top

[U02] Py：导出 / 安装依赖
来源：http://rfz.shzxlz.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dmh.ivvv.top

[U03] Py：加载 .env 配置
来源：http://bdo.jiagoushi.top

from dotenv import load_dotenv; load_dotenv()
来源：http://epf.hfpthk.cn

[U04] Py：变量调试打印
来源：http://rhv.hcnkem.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://epi.ctjpmb.com

[U05] Py：列表去重且保序
来源：http://dgi.daxiang520.top

list(dict.fromkeys(arr))
来源：http://hwv.epnwcf.com

[U06] Py：合并两个字典
来源：http://yzd.epnwcf.com

{**a, **b}
来源：http://itb.tian-w.cn

[U07] Py：反转字典键值
来源：http://osq.vqdsnc.cn

{v: k for k, v in d.items()}
来源：http://zcy.xuetiantiany.cn

[U08] Py：展平二维列表
来源：http://rsq.xuanzx.com

[y for x in nested for y in x]
来源：http://coo.vehdjk.com

[U09] Py：字典取最大值的键
来源：http://uvb.zycfv.cn

max(d, key=d.get)
来源：http://tat.tarul.cn

[U10] Py：按值排序字典
来源：http://ioz.hongshengwenyu.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jqh.guowangkeji.top

[U11] Py：生成器表达式
来源：http://fel.hywenlv.cn

(x * 2 for x in arr)
来源：http://gje.xinyue.icu

[U12] Py：取出现最多的 3 个元素
来源：http://rob.yongpay.top

Counter(arr).most_common(3)
来源：http://dkn.cucudq.cn

[U13] Py：固定长度队列
来源：http://whs.jianghu66.top

deque(maxlen=10)
来源：http://koc.aibaodan.cn

[U14] Py：分组收集到列表
来源：http://dhh.pycfn.com

defaultdict(list)
来源：http://aka.dianchejie.cn

[U15] Py：高精度计时
来源：http://flk.jinghuilouyu.cn

t = time.perf_counter()
来源：http://jds.cqqwz.cn

[U16] Py：命令行参数解析
来源：http://ajb.andypj.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qea.yuanzhike.top

[U17] Py：初始化日志
来源：http://ooc.yuxming.cn

logging.basicConfig(level=logging.INFO)
来源：http://loi.9152youxi.cn

[U18] Py：预编译正则
来源：http://xwv.daxiang520.top

pat = re.compile(r"\d+")
来源：http://hvh.sxryk.cn

[U19] Py：正则替换带回调
来源：http://xjm.sweek.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://udm.xylfe.cn

[U20] Py：缓存函数结果
来源：http://kzp.hongshengwenyu.top

@functools.lru_cache(maxsize=None)
来源：http://dgg.jiagoushi.top

[U21] Py：自定义上下文管理器
来源：http://jbt.zhoulong.xyz

@contextlib.contextmanager
来源：http://qkw.shzxlz.cn

[U22] Py：矩阵转置
来源：http://xtd.gogol.net.cn

list(zip(*m))
来源：http://wyl.epnwcf.com

[U23] Py：分块读取大文件
来源：http://lsu.sysykeji.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://heb.epnwcf.com

[U24] Py：路径操作
来源：http://cwn.iojbl.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://cly.nanxuanxn.top

[U25] Py：CSV 按字典读
来源：http://lwj.sxryk.cn

csv.DictReader(f)
来源：http://cvj.aibaodan.cn

[U26] Py：并发下载
来源：http://zje.wangshuangyany.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://aus.shuidangran.top

[U27] Py：异步 HTTP
来源：http://acq.ydzc1.top

aiohttp.ClientSession() 配合 async with
来源：http://dsu.jqgufenzy.top

[U28] Py：类型别名
来源：http://ljw.mhx1999.top

UserId = int
来源：http://duj.cucudq.cn

[U29] Py：属性校验
来源：http://qoz.shangyingyoupin.top

@property 与 @x.setter 配合
来源：http://yov.316326.xyz

[U30] Py：数据类
来源：http://qai.fengsongda.top

@dataclass(slots=True)
来源：http://puz.shanyushiyangtech.top

[U31] Py：单测
来源：http://hrh.ivvv.top

python -m pytest -q
来源：http://kgl.mhx1999.top

[U32] Py：代码格式化
来源：http://fxm.fanxiaobao.xyz

ruff format . && ruff check --fix .
来源：http://cef.cashguo.top

[U33] Py：打包发布
来源：http://pmz.jlsjyb.cn

python -m build  （依赖 pyproject.toml）
来源：http://hbb.wangshuangyany.cn

[U34] Py：判断编码
来源：http://sis.c1oappe.top

chardet.detect(raw)
来源：http://nxj.meibo888.top

[U35] Py：发送邮件
来源：http://luu.zycfv.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tur.hammf.cn

[U36] Py：定时任务
来源：http://shd.jqgfzy.top

schedule.every(10).minutes.do(job)
来源：http://rpj.sjlbkw.cn

[U37] Py：读写 Excel
来源：http://kcf.yuanzhike.top

pandas.read_excel / DataFrame.to_excel
来源：http://wmj.ywan-chungtsiang.top

[U38] Py：获取脚本所在目录
来源：http://ebk.jyoumei.cn

Path(__file__).resolve().parent
来源：http://rev.zhijiandao.cn

[U39] Py：判断是否在交互环境
来源：http://cqs.dashuyun.cn

sys.stdout.isatty()
来源：http://hlq.mhx1999.top

[U40] Py：打印到标准错误
来源：http://dxi.yueranfly.top

print("err", file=sys.stderr)
来源：http://glc.aizwys.cn

[U41] PHP：初始化 Composer 项目
来源：http://jxc.haohaochexian.top

composer init;  composer require guzzlehttp/guzzle
来源：http://whh.zdbjq.cn

[U42] PHP：PSR-4 自动加载
来源：http://qsz.sjlbkw.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gxd.feifeiyinyue.top

[U43] PHP：声明命名空间
来源：http://bwi.jqgfzy.top

namespace App\Http;
来源：http://fsa.hongshengwenyu.top

[U44] PHP：开启严格类型
来源：http://xnc.hcnkem.com

declare(strict_types=1);
来源：http://vyt.kuanghao11.cn

[U45] PHP：类型声明与返回类型
来源：http://vfl.xinyue.icu

function add(int $a, int $b): int { return $a + $b; }
来源：http://idf.hcnkem.com

[U46] PHP：可空类型
来源：http://dtw.yfazqb.com

?string $name = null
来源：http://ips.jqgfzy.top

[U47] PHP：联合类型
来源：http://arh.zhaomingkeji.xyz

int|string $id
来源：http://atj.shanyushiyangtech.top

[U48] PHP：纯枚举
来源：http://zuk.ehwqpu.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://bja.daria6918.cn

[U49] PHP：只读属性
来源：http://zkp.shangyingyoupin.top

public readonly string $name
来源：http://xcf.wangdashe.top

[U50] PHP：构造器属性提升
来源：http://bae.shangyingyoupin.top

public function __construct(private int $id) {}
来源：http://iox.zhongyouzk.top

[U51] PHP：数组解构
来源：http://jnf.tarul.cn

[$a, $b] = $arr;
来源：http://jrt.yanxiufei.cn

[U52] PHP：箭头函数
来源：http://axk.birdmap.top

$double = fn($x) => $x * 2;
来源：http://zud.jqgfzy.top

[U53] PHP：空合并运算符
来源：http://emk.xylfe.cn

$v = $a ?? $b ?? "default";
来源：http://tzj.zhoulong.xyz

[U54] PHP：空安全调用
来源：http://kdg.hammf.cn

$obj?->method()
来源：http://lah.kuanghao11.cn

[U55] PHP：match 表达式
来源：http://vjs.nwbrower.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://eid.jinghuilouyu.cn

[U56] PHP：命名参数
来源：http://khv.cucudq.cn

f(a: 1, b: 2)
来源：http://eee.epnwcf.com

[U57] PHP：字符串插值
来源：http://ccb.wangdashe.top

"值: {$a}"
来源：http://riy.chenzaomai.com

[U58] PHP：数组三件套
来源：http://rnc.aibaodan.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ngc.nanxuanxn.top

[U59] PHP：自定义排序
来源：http://tya.hfpthk.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kqd.yanxiufei.cn

[U60] PHP：JSON 编解码
来源：http://diy.cdnleiting.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lrp.andypj.xyz

[U61] PHP：正则
来源：http://eez.hnqzz.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://vmx.sufxvd.cn

[U62] PHP：日期对象
来源：http://pvi.cucudq.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://meq.yj20258.top

[U63] PHP：文件读写
来源：http://hao.meibo888.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://uwl.svipenyu.cn

[U64] PHP：目录遍历
来源：http://cip.shanyushiyangkeji.top

glob("dir/*.php");  scandir("dir");
来源：http://yju.cheryme.top

[U65] PHP：会话
来源：http://rxc.jinyuanbaomall.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://kil.mhx1999.top

[U66] PHP：设置 Cookie
来源：http://omq.ydzc1.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://toi.quarkkingdee.top

[U67] PHP：处理文件上传
来源：http://udc.yonumen.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://bya.feifeiyinyue.top

[U68] PHP：PDO 连接
来源：http://qrz.bjfxy.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nig.sufxvd.cn

[U69] PHP：PDO 预处理
来源：http://bfg.jianghu66.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://iau.9152youxi.cn

[U70] PHP：PDO 事务
来源：http://wyq.cucudq.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nxf.sysykeji.top

[U71] PHP：抛出异常
来源：http://vtg.ppjwa.cn

throw new RuntimeException("失败", 500);
来源：http://ssw.zhiwuduotai.top

[U72] PHP：写错误日志
来源：http://kwn.cucudq.cn

error_log("失败: " . $e->getMessage());
来源：http://sct.gogol.net.cn

[U73] PHP：读取 ini 配置
来源：http://buo.iojbl.cn

parse_ini_file("config.ini", true)
来源：http://svs.daria6918.cn

[U74] PHP：读取环境变量
来源：http://mva.nanxinkj.top

getenv("APP_ENV") ?: "production"
来源：http://qfu.cheryme.top

[U75] PHP：依赖注入
来源：http://naf.cheryme.top

composer require psr/container
来源：http://ler.yj20258.top

[U76] PHP：简单路由
来源：http://ysm.jinghuilouyu.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://shc.birdmap.top

[U77] PHP：模板渲染
来源：http://ush.jinghuilouyu.cn

composer require twig/twig
来源：http://mjz.xuetiantiany.cn

[U78] PHP：单元测试
来源：http://geo.jinqigfzy.top

composer require --dev phpunit/phpunit
来源：http://rta.jqgufenzy.top

[U79] PHP：静态分析
来源：http://mte.hfpthk.cn

composer require --dev phpstan/phpstan
来源：http://ewz.wangdashe.top

[U80] PHP：代码规范修复
来源：http://sti.hnqzz.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://yjc.sysykeji.top

[U81] JS：初始化项目
来源：http://bef.sysykeji.top

npm init -y;  npm i express
来源：http://imx.ehwqpu.com

[U82] JS：package.json 脚本
来源：http://buu.zhijiandao.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://psl.kuanghao11.cn

[U83] JS：ES Module 导入导出
来源：http://gaa.bbcook.cn

export const a = 1;  import { a } from "./m.js";
来源：http://qzy.gzhubu.top

[U84] JS：CommonJS 写法
来源：http://yav.316326.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://vto.0kj1m.cn

[U85] JS：可选链
来源：http://kod.sufxvd.cn

a?.b?.c
来源：http://aks.andypj.xyz

[U86] JS：空值合并
来源：http://edc.c1oappe.top

a ?? b
来源：http://rea.xylfe.cn

[U87] JS：解构默认值
来源：http://lcn.birdmap.top

const { a = 1, b = 2 } = obj;
来源：http://tbe.guannengcc.top

[U88] JS：对象展开合并
来源：http://mei.chenlongwang.top

{ ...a, ...b }
来源：http://uxe.xylfe.cn


<!-- 参考信息 -->