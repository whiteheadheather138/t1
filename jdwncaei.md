代发 wailian999

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pib.zhiwuduotai.top

================================================================================
来源：http://qsf.hesvh.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fwt.bjfxy.top

================================================================================
来源：http://qet.hammf.cn

[T01] Kotlin：Hello World
来源：http://hgu.gzhubu.top

println("Hello")
来源：http://aus.quarkkingdee.top

[T02] Kotlin：变量
来源：http://eyg.gaohongyu789.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tqh.hammf.cn

[T03] Kotlin：字符串模板
来源：http://rop.sweek.top

"值: $b"
来源：http://itx.andypj.xyz

[T04] Kotlin：空安全
来源：http://dbv.hywenlv.cn

val n: String? = null;  n?.length
来源：http://gjo.cheryme.top

[T05] Kotlin：when 表达式
来源：http://acv.kuanghao11.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://moh.sysykeji.top

[T06] Kotlin：集合映射
来源：http://aab.snrcjt.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://eho.redwolf501.top

[T07] Kotlin：集合过滤
来源：http://sfy.shanyushiyangtech.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://uhn.tarul.cn

[T08] Kotlin：数据类
来源：http://djd.feifeiyinyue.top

data class User(val name: String, val age: Int)
来源：http://ycp.bjfxy.top

[T09] Kotlin：扩展函数
来源：http://wig.chenjidiqi.icu

fun String.exclaim() = this + "!"
来源：http://rxd.cashguo.top

[T10] Kotlin：默认参数
来源：http://rjb.birdmap.top

fun greet(name: String = "World") = "Hi $name"
来源：http://uui.52xcode.cn

[T11] Kotlin：协程
来源：http://vrj.cucudq.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hde.ydjk.org.cn

[T12] Kotlin：解构声明
来源：http://lrm.fktsv.cn

val (a, b) = Pair(1, 2)
来源：http://mgt.mhx1999.top

[T13] Kotlin：只读 Map
来源：http://sqn.hysaishi.cn

val m = mapOf("a" to 1)
来源：http://hno.jinghuilouyu.cn

[T14] Kotlin：循环
来源：http://cmf.vehdjk.com

for (i in 1..10) println(i)
来源：http://ose.ydzc1.top

[T15] Kotlin：接口
来源：http://lci.hongshengwenyu.top

interface Shape { fun area(): Double }
来源：http://uts.aibaodan.cn

[T16] Swift：Hello World
来源：http://rxw.smart0.xyz

print("Hello")
来源：http://xcy.yuanzhike.top

[T17] Swift：变量与常量
来源：http://tdk.xuetiantiany.cn

var a = 1;  let b = 2
来源：http://kaz.zhiwuduotai.top

[T18] Swift：字符串插值
来源：http://crd.ppjwa.cn

"值: \(b)"
来源：http://sfg.svipenyu.cn

[T19] Swift：可选绑定
来源：http://pjf.birdmap.top

if let n = opt { print(n) }
来源：http://heh.yuanzhike.top

[T20] Swift：数组操作
来源：http://hpz.andypj.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://ehs.hysaishi.cn

[T21] Swift：遍历
来源：http://eri.dashuyun.cn

for x in a { print(x) }
来源：http://eqr.xziqi.cn

[T22] Swift：字典
来源：http://frn.0kj1m.cn

var d = ["a": 1];  d["b"] = 2
来源：http://efu.xuanzx.com

[T23] Swift：函数
来源：http://hqb.ydjk.org.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cvw.shuidangran.top

[T24] Swift：闭包
来源：http://glf.xingfuxueyuan.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://qeu.tarul.cn

[T25] Swift：结构体
来源：http://prm.sufxvd.cn

struct P { var x: Int }
来源：http://vbd.cqqwz.cn

[T26] Swift：类与重写
来源：http://adx.jqgufenzy.top

class A: Base { override func f() {} }
来源：http://xts.hnqzz.top

[T27] Swift：错误处理
来源：http://vyr.aizwys.cn

do { try f() } catch { print(error) }
来源：http://pkf.zhijiandao.cn

[T28] Swift：枚举
来源：http://lan.guannengcc.top

enum Color { case red, green }
来源：http://eeb.sxryk.cn

[T29] Swift：guard 提前返回
来源：http://tbj.gogol.net.cn

guard let x = opt else { return }
来源：http://jvn.bjfxy.top

[T30] Swift：协议
来源：http://rxb.c1oappe.top

protocol Shape { func area() -> Double }
来源：http://wkh.tianlin.xyz

[T31] Lua：Hello World
来源：http://ymr.ehwqpu.com

print("Hello")
来源：http://kft.shuidangran.top

[T32] Lua：局部变量
来源：http://buj.zhijiandao.cn

local a = 1
来源：http://dho.cqqwz.cn

[T33] Lua：表（数组）
来源：http://tsk.yj20258.top

local t = {1, 2, 3};  t[4] = 4
来源：http://hlx.kuanghao11.cn

[T34] Lua：遍历表
来源：http://uox.ywan-chungtsiang.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ppz.tianlin.xyz

[T35] Lua：字典表
来源：http://dhz.guannengcc.top

local d = { a = 1 };  d.b = 2
来源：http://ffk.zhaomingkeji.xyz

[T36] Lua：函数
来源：http://xqt.hesvh.cn

function add(a, b) return a + b end
来源：http://kbg.jlsjyb.cn

[T37] Lua：字符串拼接
来源：http://net.shanyushiyangkeji.top

"a" .. "b"
来源：http://hkw.bjfxy.top

[T38] Lua：条件
来源：http://pqf.mhx1999.top

if x > 0 then print("正") end
来源：http://fkg.ctjpmb.com

[T39] Lua：模式匹配
来源：http://dnz.haohaochexian.top

string.find(s, "%d+")
来源：http://fom.316326.xyz

[T40] Lua：元表
来源：http://zvf.hcnkem.com

setmetatable({}, { __index = base })
来源：http://cpe.zycfv.cn

[T41] Perl：Hello World
来源：http://lge.nanxinkj.top

print "Hello\n";
来源：http://flt.vqdsnc.cn

[T42] Perl：变量类型
来源：http://nau.nanxinkj.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bkp.vqdsnc.cn

[T43] Perl：字符串插值
来源：http://mlo.cheryme.top

"值: $a"
来源：http://hks.zdbjq.cn

[T44] Perl：条件
来源：http://fkp.zhengqikj.top

if ($a > 0) { print "正"; }
来源：http://izg.jinghuilouyu.cn

[T45] Perl：数组遍历
来源：http://wxy.sjlbkw.cn

for my $x (@arr) { print $x; }
来源：http://qzi.wangdashe.top

[T46] Perl：哈希操作
来源：http://bvp.wangdashe.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fmp.ehwqpu.com

[T47] Perl：正则捕获
来源：http://xyg.daxiang520.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://xzi.yongpay.top

[T48] Perl：正则替换
来源：http://qvj.kuanghao11.cn

$s =~ s/old/new/g;
来源：http://pux.sysykeji.top

[T49] Perl：函数
来源：http://wmd.xziqi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bwy.zhongyouzk.top

[T50] Perl：逐行读文件
来源：http://rqf.sysykeji.top

open my $fh, "<", "a.txt" or die $!;
来源：http://asy.ctjpmb.com

while (my $line = <$fh>) { print $line; }
来源：http://nby.dianchejie.cn

[T51] Scala：Hello World
来源：http://byf.jyoumei.cn

println("Hello")
来源：http://bsw.haohaochexian.top

[T52] Scala：变量
来源：http://xek.yonumen.top

val a = 1;  var b = 2
来源：http://mad.sxryk.cn

[T53] Scala：字符串插值
来源：http://rbf.hongshengwenyu.top

s"值: $b"
来源：http://yfn.mhx1999.top

[T54] Scala：集合映射
来源：http://acn.jiagoushi.top

List(1, 2, 3).map(_ * 2)
来源：http://zzr.shangyingyoupin.top

[T55] Scala：集合过滤
来源：http://ouv.ctjpmb.com

List(1, 2, 3).filter(_ > 1)
来源：http://mub.yvedp.cn

[T56] Scala：样例类
来源：http://jng.sysykeji.top

case class User(name: String, age: Int)
来源：http://rkt.jlsjyb.cn

[T57] Scala：模式匹配
来源：http://qwn.ppjwa.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://kqf.aibaodan.cn

[T58] Scala：函数定义
来源：http://knc.ydzc1.top

def add(a: Int, b: Int): Int = a + b
来源：http://pkn.jlsjyb.cn

[T59] Scala：循环
来源：http://bur.xuanzx.com

for (i <- 1 to 10) println(i)
来源：http://shy.shanyushiyangkeji.top

[T60] Scala：折叠
来源：http://yra.zycfv.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kdl.jqgfzy.top

================================================================================
来源：http://htz.xingfuxueyuan.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ryj.xziqi.cn

================================================================================
来源：http://amp.svipenyu.cn

[U01] Py：创建虚拟环境
来源：http://xpa.gaohongyu789.top

python -m venv .venv && source .venv/bin/activate
来源：http://jid.vqdsnc.cn

[U02] Py：导出 / 安装依赖
来源：http://tcm.0kj1m.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gyx.jqgfzy.top

[U03] Py：加载 .env 配置
来源：http://dkz.wangshuangyany.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://vem.sysykeji.top

[U04] Py：变量调试打印
来源：http://oai.52xcode.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fhm.c1oappe.top

[U05] Py：列表去重且保序
来源：http://hpu.yj20258.top

list(dict.fromkeys(arr))
来源：http://ckh.zhixingplan.top

[U06] Py：合并两个字典
来源：http://jxv.tanke756.top

{**a, **b}
来源：http://tub.dashuyun.cn

[U07] Py：反转字典键值
来源：http://qyk.gzhubu.top

{v: k for k, v in d.items()}
来源：http://shn.jianghu66.top

[U08] Py：展平二维列表
来源：http://sre.zycfv.cn

[y for x in nested for y in x]
来源：http://dau.meibo888.top

[U09] Py：字典取最大值的键
来源：http://tmu.uphjek.com

max(d, key=d.get)
来源：http://oyc.yvedp.cn

[U10] Py：按值排序字典
来源：http://cuj.hysaishi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cjv.zdbjq.cn

[U11] Py：生成器表达式
来源：http://xzj.0kj1m.cn

(x * 2 for x in arr)
来源：http://fyx.zhiwuduotai.top

[U12] Py：取出现最多的 3 个元素
来源：http://xqy.yanxiufei.cn

Counter(arr).most_common(3)
来源：http://zzw.zhixingplan.top

[U13] Py：固定长度队列
来源：http://lff.yanxiufei.cn

deque(maxlen=10)
来源：http://jjz.nanxuanxn.top

[U14] Py：分组收集到列表
来源：http://nux.gzhubu.top

defaultdict(list)
来源：http://ena.zdqjudy.top

[U15] Py：高精度计时
来源：http://tta.ybcxt.top

t = time.perf_counter()
来源：http://ojp.cashguo.top

[U16] Py：命令行参数解析
来源：http://raj.jianghu66.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lfj.cdnleiting.top

[U17] Py：初始化日志
来源：http://vrr.vqdsnc.cn

logging.basicConfig(level=logging.INFO)
来源：http://ytn.ehwqpu.com

[U18] Py：预编译正则
来源：http://abo.c1oappe.top

pat = re.compile(r"\d+")
来源：http://avo.yonumen.top

[U19] Py：正则替换带回调
来源：http://plu.zycfv.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://atz.sweek.top

[U20] Py：缓存函数结果
来源：http://teh.jqgufenzy.top

@functools.lru_cache(maxsize=None)
来源：http://dst.zhoulong.xyz

[U21] Py：自定义上下文管理器
来源：http://hfk.316326.xyz

@contextlib.contextmanager
来源：http://cxt.zhengqikj.top

[U22] Py：矩阵转置
来源：http://nzk.tarul.cn

list(zip(*m))
来源：http://wbv.cqqwz.cn

[U23] Py：分块读取大文件
来源：http://wfr.tanke756.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://yrr.jlsjyb.cn

[U24] Py：路径操作
来源：http://ltu.dianchejie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pam.jinyuanbaomall.cn

[U25] Py：CSV 按字典读
来源：http://pep.yuxming.cn

csv.DictReader(f)
来源：http://jto.aizwys.cn

[U26] Py：并发下载
来源：http://lzj.hywenlv.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rih.daria6918.cn

[U27] Py：异步 HTTP
来源：http://bgq.chenjidiqi.icu

aiohttp.ClientSession() 配合 async with
来源：http://jbz.yangfankeji.com

[U28] Py：类型别名
来源：http://iwd.wangdashe.top

UserId = int
来源：http://ukq.ydzc1.top

[U29] Py：属性校验
来源：http://dsw.sweek.top

@property 与 @x.setter 配合
来源：http://wwm.316326.xyz

[U30] Py：数据类
来源：http://qpl.shanyushiyangkeji.top

@dataclass(slots=True)
来源：http://glo.tanke756.top

[U31] Py：单测
来源：http://jzv.aibaodan.cn

python -m pytest -q
来源：http://sdt.iojbl.cn

[U32] Py：代码格式化
来源：http://xyx.xuanzx.com

ruff format . && ruff check --fix .
来源：http://djn.yueranfly.top

[U33] Py：打包发布
来源：http://egd.smart0.xyz

python -m build  （依赖 pyproject.toml）
来源：http://tpt.9152youxi.cn

[U34] Py：判断编码
来源：http://zes.sjlbkw.cn

chardet.detect(raw)
来源：http://jvi.zycfv.cn

[U35] Py：发送邮件
来源：http://npt.guowangkeji.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://okj.gogol.net.cn

[U36] Py：定时任务
来源：http://sdl.zhongyouzk.top

schedule.every(10).minutes.do(job)
来源：http://sux.jinqigfzy.top

[U37] Py：读写 Excel
来源：http://dlt.52xcode.cn

pandas.read_excel / DataFrame.to_excel
来源：http://man.zhiwuduotai.top

[U38] Py：获取脚本所在目录
来源：http://ddf.yongpay.top

Path(__file__).resolve().parent
来源：http://tqn.jiagoushi.top

[U39] Py：判断是否在交互环境
来源：http://kxl.pengpengdd.cyou

sys.stdout.isatty()
来源：http://qdy.wangdashe.top

[U40] Py：打印到标准错误
来源：http://kur.ydjk.org.cn

print("err", file=sys.stderr)
来源：http://pki.yj20258888.top

[U41] PHP：初始化 Composer 项目
来源：http://tja.gzhubu.top

composer init;  composer require guzzlehttp/guzzle
来源：http://ani.fehbvm.com

[U42] PHP：PSR-4 自动加载
来源：http://ekm.svipenyu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wtp.xziqi.cn

[U43] PHP：声明命名空间
来源：http://suk.tanke756.top

namespace App\Http;
来源：http://oma.316326.xyz

[U44] PHP：开启严格类型
来源：http://fcj.epnwcf.com

declare(strict_types=1);
来源：http://way.chenlongwang.top

[U45] PHP：类型声明与返回类型
来源：http://nyo.gzhubu.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://tgc.uphjek.com

[U46] PHP：可空类型
来源：http://jlq.aizwys.cn

?string $name = null
来源：http://tnd.bjfxy.top

[U47] PHP：联合类型
来源：http://lrr.daxiang520.top

int|string $id
来源：http://bnl.hnqzz.top

[U48] PHP：纯枚举
来源：http://ask.zhaomingkeji.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nkk.bjfxy.top

[U49] PHP：只读属性
来源：http://vtj.yj20258888.top

public readonly string $name
来源：http://joo.daria6918.cn

[U50] PHP：构造器属性提升
来源：http://dad.ydzc1.top

public function __construct(private int $id) {}
来源：http://rgp.nwbrower.top

[U51] PHP：数组解构
来源：http://jxx.jinghuilouyu.cn

[$a, $b] = $arr;
来源：http://bjz.fzhhl.top

[U52] PHP：箭头函数
来源：http://vum.ehwqpu.com

$double = fn($x) => $x * 2;
来源：http://iik.52xcode.cn

[U53] PHP：空合并运算符
来源：http://vhy.jianghu66.top

$v = $a ?? $b ?? "default";
来源：http://qjf.zhoulong.xyz

[U54] PHP：空安全调用
来源：http://jsk.zhongyouzk.top

$obj?->method()
来源：http://cbs.guowangkeji.top

[U55] PHP：match 表达式
来源：http://cxv.ivvv.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zca.sufxvd.cn

[U56] PHP：命名参数
来源：http://vfc.yueranfly.top

f(a: 1, b: 2)
来源：http://xye.yuxming.cn

[U57] PHP：字符串插值
来源：http://udi.ydzc1.top

"值: {$a}"
来源：http://vis.sufxvd.cn

[U58] PHP：数组三件套
来源：http://yej.cucudq.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lae.jiagoushi.top

[U59] PHP：自定义排序
来源：http://ccm.yanxiufei.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://szf.wangdashe.top

[U60] PHP：JSON 编解码
来源：http://jgz.feifeiyinyue.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://eil.shanyushiyangkeji.top

[U61] PHP：正则
来源：http://lac.c1oappe.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://kka.wangshuangyany.cn

[U62] PHP：日期对象
来源：http://hnp.zycfv.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://udj.daxiang520.top

[U63] PHP：文件读写
来源：http://czq.ppjwa.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fou.jqgufenzy.top

[U64] PHP：目录遍历
来源：http://com.chenjidiqi.icu

glob("dir/*.php");  scandir("dir");
来源：http://kqy.iojbl.cn

[U65] PHP：会话
来源：http://ywq.zdqjudy.top

session_start();  $_SESSION["uid"] = 1;
来源：http://cye.zhongyouzk.top

[U66] PHP：设置 Cookie
来源：http://smk.316326.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://koc.daria6918.cn

[U67] PHP：处理文件上传
来源：http://ydp.sweek.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://pjc.ctjpmb.com

[U68] PHP：PDO 连接
来源：http://mdw.hysaishi.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://eum.shzxlz.cn

[U69] PHP：PDO 预处理
来源：http://gwn.yj20258888.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wmu.yuxming.cn

[U70] PHP：PDO 事务
来源：http://xld.zycfv.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://eme.ydzc1.top

[U71] PHP：抛出异常
来源：http://zhv.hnqzz.top

throw new RuntimeException("失败", 500);
来源：http://jlc.zdqjudy.top

[U72] PHP：写错误日志
来源：http://qfg.hesvh.cn

error_log("失败: " . $e->getMessage());
来源：http://lyw.vehdjk.com

[U73] PHP：读取 ini 配置
来源：http://hgj.chenjidiqi.icu

parse_ini_file("config.ini", true)
来源：http://zdg.c1oappe.top

[U74] PHP：读取环境变量
来源：http://shd.guowangkeji.top

getenv("APP_ENV") ?: "production"
来源：http://kdd.jqgfzy.top

[U75] PHP：依赖注入
来源：http://obi.zhongyouzk.top

composer require psr/container
来源：http://ulf.yuxming.cn

[U76] PHP：简单路由
来源：http://pku.feifeiyinyue.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lxr.ybcxt.top

[U77] PHP：模板渲染
来源：http://mgn.gzhubu.top

composer require twig/twig
来源：http://bom.yj202588.top

[U78] PHP：单元测试
来源：http://zzi.pycfn.com

composer require --dev phpunit/phpunit
来源：http://cxs.gzhubu.top

[U79] PHP：静态分析
来源：http://goh.haohaochexian.top

composer require --dev phpstan/phpstan
来源：http://ber.shangyingyoupin.top

[U80] PHP：代码规范修复
来源：http://qqd.jinqigfzy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://xfw.aibaodan.cn

[U81] JS：初始化项目
来源：http://xbv.zdbjq.cn

npm init -y;  npm i express
来源：http://gsi.zhaomingkeji.xyz

[U82] JS：package.json 脚本
来源：http://zhm.zdqjudy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://pqn.fzhhl.top

[U83] JS：ES Module 导入导出
来源：http://fzv.yuanzhike.top

export const a = 1;  import { a } from "./m.js";
来源：http://mcd.nanxinkj.top

[U84] JS：CommonJS 写法
来源：http://adj.kuanghao11.cn

module.exports = { a };  const { a } = require("./m");
来源：http://fdq.epnwcf.com

[U85] JS：可选链
来源：http://bih.cqqwz.cn

a?.b?.c
来源：http://gqv.yfazqb.com

[U86] JS：空值合并
来源：http://tnx.feifeiyinyue.top

a ?? b
来源：http://mxu.shzxlz.cn


<!-- 参考信息 -->