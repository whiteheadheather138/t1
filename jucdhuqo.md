代发 wailian999

[T03] Kotlin：字符串模板
来源：http://yjz.guowangkeji.top

"值: $b"
来源：http://wbg.jinqigfzy.top

[T04] Kotlin：空安全
来源：http://ndo.zhijiandao.cn

val n: String? = null;  n?.length
来源：http://wbh.vqdsnc.cn

[T05] Kotlin：when 表达式
来源：http://wfz.yfazqb.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blu.yanxiufei.cn

[T06] Kotlin：集合映射
来源：http://xik.daxiang520.top

listOf(1, 2, 3).map { it * 2 }
来源：http://jae.meibo888.top

[T07] Kotlin：集合过滤
来源：http://the.gzhubu.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://psi.cqqwz.cn

[T08] Kotlin：数据类
来源：http://lzs.haohaochexian.top

data class User(val name: String, val age: Int)
来源：http://ajx.bjfxy.top

[T09] Kotlin：扩展函数
来源：http://bgy.ydzc1.top

fun String.exclaim() = this + "!"
来源：http://qvk.yueranfly.top

[T10] Kotlin：默认参数
来源：http://kzj.wangshuangyany.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wur.redwolf501.top

[T11] Kotlin：协程
来源：http://dxq.fktsv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qzh.316326.xyz

[T12] Kotlin：解构声明
来源：http://kua.316326.xyz

val (a, b) = Pair(1, 2)
来源：http://hrh.iojbl.cn

[T13] Kotlin：只读 Map
来源：http://iba.52xcode.cn

val m = mapOf("a" to 1)
来源：http://emz.ybcxt.top

[T14] Kotlin：循环
来源：http://frn.zhengqikj.top

for (i in 1..10) println(i)
来源：http://fxl.xinyue.icu

[T15] Kotlin：接口
来源：http://zsb.sxryk.cn

interface Shape { fun area(): Double }
来源：http://afe.yuxming.cn

[T16] Swift：Hello World
来源：http://cbw.yongpay.top

print("Hello")
来源：http://vmg.nanxuanxn.top

[T17] Swift：变量与常量
来源：http://isk.uphjek.com

var a = 1;  let b = 2
来源：http://nga.gogol.net.cn

[T18] Swift：字符串插值
来源：http://gji.chenzaomai.com

"值: \(b)"
来源：http://umv.fanxiaobao.xyz

[T19] Swift：可选绑定
来源：http://tlt.chenlongwang.top

if let n = opt { print(n) }
来源：http://hze.meibo888.top

[T20] Swift：数组操作
来源：http://udg.jinghuilouyu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ujk.snrcjt.cn

[T21] Swift：遍历
来源：http://wjq.shuidangran.top

for x in a { print(x) }
来源：http://iga.0kj1m.cn

[T22] Swift：字典
来源：http://chx.wangshuangyany.cn

var d = ["a": 1];  d["b"] = 2
来源：http://koo.ivvv.top

[T23] Swift：函数
来源：http://vbd.yuxming.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mln.yj20258888.top

[T24] Swift：闭包
来源：http://hsm.hfpthk.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vrj.svipenyu.cn

[T25] Swift：结构体
来源：http://ctb.yj202588.top

struct P { var x: Int }
来源：http://czf.gzhubu.top

[T26] Swift：类与重写
来源：http://vvg.ppjwa.cn

class A: Base { override func f() {} }
来源：http://oaj.daxiang520.top

[T27] Swift：错误处理
来源：http://tul.xuanzx.com

do { try f() } catch { print(error) }
来源：http://pdd.hnqzz.top

[T28] Swift：枚举
来源：http://ldx.yuxming.cn

enum Color { case red, green }
来源：http://pmw.xinyue.icu

[T29] Swift：guard 提前返回
来源：http://exk.iojbl.cn

guard let x = opt else { return }
来源：http://lsq.chenjidiqi.icu

[T30] Swift：协议
来源：http://oux.jinyuanbaomall.cn

protocol Shape { func area() -> Double }
来源：http://ync.52xcode.cn

[T31] Lua：Hello World
来源：http://xzz.yuxming.cn

print("Hello")
来源：http://elf.yueranfly.top

[T32] Lua：局部变量
来源：http://ety.yueranfly.top

local a = 1
来源：http://sqb.shuidangran.top

[T33] Lua：表（数组）
来源：http://bzr.shanyushiyangtech.top

local t = {1, 2, 3};  t[4] = 4
来源：http://pne.sxryk.cn

[T34] Lua：遍历表
来源：http://kmf.quarkkingdee.top

for i, v in ipairs(t) do print(i, v) end
来源：http://xqs.ydzc1.top

[T35] Lua：字典表
来源：http://prc.kuanghao11.cn

local d = { a = 1 };  d.b = 2
来源：http://vkm.jqgufenzy.top

[T36] Lua：函数
来源：http://xzj.xylfe.cn

function add(a, b) return a + b end
来源：http://jeo.hcnkem.com

[T37] Lua：字符串拼接
来源：http://wgn.gaohongyu789.top

"a" .. "b"
来源：http://lsj.xuanzx.com

[T38] Lua：条件
来源：http://hrv.hcnkem.com

if x > 0 then print("正") end
来源：http://fqo.cqqwz.cn

[T39] Lua：模式匹配
来源：http://rnr.yanxiufei.cn

string.find(s, "%d+")
来源：http://cve.wangshuangyany.cn

[T40] Lua：元表
来源：http://mrg.pengpengdd.cyou

setmetatable({}, { __index = base })
来源：http://gsn.hnxiangtu.top

[T41] Perl：Hello World
来源：http://pgm.aibaodan.cn

print "Hello\n";
来源：http://uqv.vqdsnc.cn

[T42] Perl：变量类型
来源：http://ada.jqgfzy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tgb.yj20258888.top

[T43] Perl：字符串插值
来源：http://xve.nanxinkj.top

"值: $a"
来源：http://lpo.zdbjq.cn

[T44] Perl：条件
来源：http://fxb.xziqi.cn

if ($a > 0) { print "正"; }
来源：http://vdq.xuanzx.com

[T45] Perl：数组遍历
来源：http://wrf.hnxiangtu.top

for my $x (@arr) { print $x; }
来源：http://kcd.yj20258888.top

[T46] Perl：哈希操作
来源：http://fau.sweek.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://duq.ybcxt.top

[T47] Perl：正则捕获
来源：http://wpa.xuetiantiany.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xai.birdmap.top

[T48] Perl：正则替换
来源：http://chj.zhoulong.xyz

$s =~ s/old/new/g;
来源：http://fvt.yvedp.cn

[T49] Perl：函数
来源：http://iqr.iojbl.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://byg.shanyushiyangkeji.top

[T50] Perl：逐行读文件
来源：http://aaw.xziqi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://snk.ctjpmb.com

while (my $line = <$fh>) { print $line; }
来源：http://pfz.sjlbkw.cn

[T51] Scala：Hello World
来源：http://tlo.zhijiandao.cn

println("Hello")
来源：http://umm.tanke756.top

[T52] Scala：变量
来源：http://rup.shangyingyoupin.top

val a = 1;  var b = 2
来源：http://ufn.52xcode.cn

[T53] Scala：字符串插值
来源：http://nxe.quarkkingdee.top

s"值: $b"
来源：http://izg.jinghuilouyu.cn

[T54] Scala：集合映射
来源：http://xnz.gotoacloud.top

List(1, 2, 3).map(_ * 2)
来源：http://aop.nanxinkj.top

[T55] Scala：集合过滤
来源：http://gko.zdbjq.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gvl.pengpengdd.cyou

[T56] Scala：样例类
来源：http://isc.iojbl.cn

case class User(name: String, age: Int)
来源：http://doi.dianchejie.cn

[T57] Scala：模式匹配
来源：http://zru.zhixingplan.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://uje.wangshuangyany.cn

[T58] Scala：函数定义
来源：http://pby.fehbvm.com

def add(a: Int, b: Int): Int = a + b
来源：http://yxg.pycfn.com

[T59] Scala：循环
来源：http://zfq.dianchejie.cn

for (i <- 1 to 10) println(i)
来源：http://ckx.ppjwa.cn

[T60] Scala：折叠
来源：http://tyw.uphjek.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://myc.hammf.cn

================================================================================
来源：http://lkr.tarul.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hyo.jianghu66.top

================================================================================
来源：http://wty.hcnkem.com

[U01] Py：创建虚拟环境
来源：http://eiu.jlsjyb.cn

python -m venv .venv && source .venv/bin/activate
来源：http://gao.jqgufenzy.top

[U02] Py：导出 / 安装依赖
来源：http://sgv.wangdashe.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kpn.gogol.net.cn

[U03] Py：加载 .env 配置
来源：http://ybs.ydzc1.top

from dotenv import load_dotenv; load_dotenv()
来源：http://xxs.yueranfly.top

[U04] Py：变量调试打印
来源：http://pph.hcnkem.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kpm.zhijiandao.cn

[U05] Py：列表去重且保序
来源：http://isn.hnxiangtu.top

list(dict.fromkeys(arr))
来源：http://nbs.redwolf501.top

[U06] Py：合并两个字典
来源：http://gix.cheryme.top

{**a, **b}
来源：http://yfw.jqgfzy.top

[U07] Py：反转字典键值
来源：http://wiw.fehbvm.com

{v: k for k, v in d.items()}
来源：http://iku.daria6918.cn

[U08] Py：展平二维列表
来源：http://eyt.9152youxi.cn

[y for x in nested for y in x]
来源：http://puq.smart0.xyz

[U09] Py：字典取最大值的键
来源：http://rwy.dianchejie.cn

max(d, key=d.get)
来源：http://xjf.shzxlz.cn

[U10] Py：按值排序字典
来源：http://pyj.ydjk.org.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rms.jyoumei.cn

[U11] Py：生成器表达式
来源：http://qze.chenlongwang.top

(x * 2 for x in arr)
来源：http://cyd.jqgfzy.top

[U12] Py：取出现最多的 3 个元素
来源：http://rwv.guannengcc.top

Counter(arr).most_common(3)
来源：http://lod.shanyushiyangtech.top

[U13] Py：固定长度队列
来源：http://toe.jqgfzy.top

deque(maxlen=10)
来源：http://fmk.nwbrower.top

[U14] Py：分组收集到列表
来源：http://ymd.jyoumei.cn

defaultdict(list)
来源：http://ton.xuanzx.com

[U15] Py：高精度计时
来源：http://zgu.gotoacloud.top

t = time.perf_counter()
来源：http://hdv.ydzc1.top

[U16] Py：命令行参数解析
来源：http://ekc.yvedp.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wjf.sxryk.cn

[U17] Py：初始化日志
来源：http://fub.zhengqikj.top

logging.basicConfig(level=logging.INFO)
来源：http://ufx.fanxiaobao.xyz

[U18] Py：预编译正则
来源：http://uoo.quarkkingdee.top

pat = re.compile(r"\d+")
来源：http://xwz.wangshuangyany.cn

[U19] Py：正则替换带回调
来源：http://pmo.hnqzz.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ose.yanxiufei.cn

[U20] Py：缓存函数结果
来源：http://avs.shuidangran.top

@functools.lru_cache(maxsize=None)
来源：http://hir.chenlongwang.top

[U21] Py：自定义上下文管理器
来源：http://gic.cucudq.cn

@contextlib.contextmanager
来源：http://fhs.jinqigfzy.top

[U22] Py：矩阵转置
来源：http://yip.feifeiyinyue.top

list(zip(*m))
来源：http://zny.kuanghao11.cn

[U23] Py：分块读取大文件
来源：http://cru.redwolf501.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://geu.zhijiandao.cn

[U24] Py：路径操作
来源：http://vwf.sweek.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ktc.fanxiaobao.xyz

[U25] Py：CSV 按字典读
来源：http://xtd.sufxvd.cn

csv.DictReader(f)
来源：http://qdh.zycfv.cn

[U26] Py：并发下载
来源：http://qef.c1oappe.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tpl.fzhhl.top

[U27] Py：异步 HTTP
来源：http://hll.ybcxt.top

aiohttp.ClientSession() 配合 async with
来源：http://vka.daria6918.cn

[U28] Py：类型别名
来源：http://lub.xinyue.icu

UserId = int
来源：http://kde.yfazqb.com

[U29] Py：属性校验
来源：http://rgm.tanke756.top

@property 与 @x.setter 配合
来源：http://qzn.tarul.cn

[U30] Py：数据类
来源：http://mjm.mhx1999.top

@dataclass(slots=True)
来源：http://zdl.daxiang520.top

[U31] Py：单测
来源：http://ooq.cheryme.top

python -m pytest -q
来源：http://fjr.quarkkingdee.top

[U32] Py：代码格式化
来源：http://naq.fengsongda.top

ruff format . && ruff check --fix .
来源：http://seb.shanyushiyangkeji.top

[U33] Py：打包发布
来源：http://ejg.zdqjudy.top

python -m build  （依赖 pyproject.toml）
来源：http://whc.ydjk.org.cn

[U34] Py：判断编码
来源：http://vqj.yfazqb.com

chardet.detect(raw)
来源：http://vxb.yangfankeji.com

[U35] Py：发送邮件
来源：http://lso.uphjek.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nbp.fehbvm.com

[U36] Py：定时任务
来源：http://ybc.hesvh.cn

schedule.every(10).minutes.do(job)
来源：http://fvg.9152youxi.cn

[U37] Py：读写 Excel
来源：http://bnd.pycfn.com

pandas.read_excel / DataFrame.to_excel
来源：http://ygx.bbcook.cn

[U38] Py：获取脚本所在目录
来源：http://xrv.9152youxi.cn

Path(__file__).resolve().parent
来源：http://ofb.hcnkem.com

[U39] Py：判断是否在交互环境
来源：http://qsj.zhongyouzk.top

sys.stdout.isatty()
来源：http://oqb.jqgfzy.top

[U40] Py：打印到标准错误
来源：http://kin.guowangkeji.top

print("err", file=sys.stderr)
来源：http://apa.hesvh.cn

[U41] PHP：初始化 Composer 项目
来源：http://mfe.jlsjyb.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://yls.chenzaomai.com

[U42] PHP：PSR-4 自动加载
来源：http://wxw.xziqi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ewj.hnqzz.top

[U43] PHP：声明命名空间
来源：http://ljy.ydjk.org.cn

namespace App\Http;
来源：http://qxf.316326.xyz

[U44] PHP：开启严格类型
来源：http://lbo.sweek.top

declare(strict_types=1);
来源：http://xjx.nanxuanxn.top

[U45] PHP：类型声明与返回类型
来源：http://aft.yj20258.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://qee.redwolf501.top

[U46] PHP：可空类型
来源：http://cha.pengpengdd.cyou

?string $name = null
来源：http://bso.aizwys.cn

[U47] PHP：联合类型
来源：http://uud.shzxlz.cn

int|string $id
来源：http://rds.mhx1999.top

[U48] PHP：纯枚举
来源：http://otb.xuetiantiany.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ivh.yj20258.top

[U49] PHP：只读属性
来源：http://smr.jinqigfzy.top

public readonly string $name
来源：http://wdj.zdbjq.cn

[U50] PHP：构造器属性提升
来源：http://lai.daxiang520.top

public function __construct(private int $id) {}
来源：http://tvc.aizwys.cn

[U51] PHP：数组解构
来源：http://rfo.jinqigufen.top

[$a, $b] = $arr;
来源：http://jpf.sweek.top

[U52] PHP：箭头函数
来源：http://ewa.zycfv.cn

$double = fn($x) => $x * 2;
来源：http://luu.chenlongwang.top

[U53] PHP：空合并运算符
来源：http://ixt.jinyuanbaomall.cn

$v = $a ?? $b ?? "default";
来源：http://ccs.ywan-chungtsiang.top

[U54] PHP：空安全调用
来源：http://oxm.meibo888.top

$obj?->method()
来源：http://lqt.cucudq.cn

[U55] PHP：match 表达式
来源：http://phi.chenzaomai.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://qpl.shzxlz.cn

[U56] PHP：命名参数
来源：http://lot.xinyue.icu

f(a: 1, b: 2)
来源：http://lkn.wangdashe.top

[U57] PHP：字符串插值
来源：http://fwk.haohaochexian.top

"值: {$a}"
来源：http://dqp.dashuyun.cn

[U58] PHP：数组三件套
来源：http://fmo.iojbl.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wvi.xinyue.icu

[U59] PHP：自定义排序
来源：http://eyh.redwolf501.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://asb.shangyingyoupin.top

[U60] PHP：JSON 编解码
来源：http://oku.quarkkingdee.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wty.ehwqpu.com

[U61] PHP：正则
来源：http://mqn.fktsv.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ajh.pengpengdd.cyou

[U62] PHP：日期对象
来源：http://jdq.vqdsnc.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nta.cdnleiting.top

[U63] PHP：文件读写
来源：http://wnx.yfazqb.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bkd.xuetiantiany.cn

[U64] PHP：目录遍历
来源：http://ulx.dashuyun.cn

glob("dir/*.php");  scandir("dir");
来源：http://cfo.jiagoushi.top

[U65] PHP：会话
来源：http://hbz.ehwqpu.com

session_start();  $_SESSION["uid"] = 1;
来源：http://spt.smart0.xyz

[U66] PHP：设置 Cookie
来源：http://kms.jyoumei.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://cmu.kuanghao11.cn

[U67] PHP：处理文件上传
来源：http://olb.tian-w.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ypb.jinqigufen.top

[U68] PHP：PDO 连接
来源：http://eec.316326.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kdh.haohaochexian.top

[U69] PHP：PDO 预处理
来源：http://cym.svipenyu.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://pdk.sjlbkw.cn

[U70] PHP：PDO 事务
来源：http://kuv.yuxming.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://yti.haohaochexian.top

[U71] PHP：抛出异常
来源：http://gio.aibaodan.cn

throw new RuntimeException("失败", 500);
来源：http://pcq.chenlongwang.top

[U72] PHP：写错误日志
来源：http://zoh.yfazqb.com

error_log("失败: " . $e->getMessage());
来源：http://lqg.zhaomingkeji.xyz

[U73] PHP：读取 ini 配置
来源：http://cym.mhx1999.top

parse_ini_file("config.ini", true)
来源：http://zlp.havefunace.top

[U74] PHP：读取环境变量
来源：http://ssv.yvedp.cn

getenv("APP_ENV") ?: "production"
来源：http://gzt.jlsjyb.cn

[U75] PHP：依赖注入
来源：http://yzx.gaohongyu789.top

composer require psr/container
来源：http://amb.fzhhl.top

[U76] PHP：简单路由
来源：http://bfx.xuetiantiany.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jab.sxryk.cn

[U77] PHP：模板渲染
来源：http://xxl.daria6918.cn

composer require twig/twig
来源：http://wrd.gogol.net.cn

[U78] PHP：单元测试
来源：http://rel.fktsv.cn

composer require --dev phpunit/phpunit
来源：http://cqw.nwbrower.top

[U79] PHP：静态分析
来源：http://nkp.yj20258888.top

composer require --dev phpstan/phpstan
来源：http://faw.cdnleiting.top

[U80] PHP：代码规范修复
来源：http://hsz.sufxvd.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://hpn.aizwys.cn

[U81] JS：初始化项目
来源：http://mea.zdbjq.cn

npm init -y;  npm i express
来源：http://ama.feifeiyinyue.top

[U82] JS：package.json 脚本
来源：http://vuv.tarul.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://jrh.hywenlv.cn

[U83] JS：ES Module 导入导出
来源：http://vtc.hysaishi.cn

export const a = 1;  import { a } from "./m.js";
来源：http://ffa.hammf.cn

[U84] JS：CommonJS 写法
来源：http://irn.chenzaomai.com

module.exports = { a };  const { a } = require("./m");
来源：http://kny.aizwys.cn

[U85] JS：可选链
来源：http://xjt.tian-w.cn

a?.b?.c
来源：http://opr.yj202588.top

[U86] JS：空值合并
来源：http://pkt.birdmap.top

a ?? b
来源：http://qab.dashuyun.cn

[U87] JS：解构默认值
来源：http://btp.hnxiangtu.top

const { a = 1, b = 2 } = obj;
来源：http://yeo.xuetiantiany.cn

[U88] JS：对象展开合并
来源：http://ltn.fanxiaobao.xyz

{ ...a, ...b }
来源：http://ckz.iojbl.cn

[U89] JS：数组去重
来源：http://zae.gzhubu.top

[...new Set(arr)]
来源：http://ffa.fengsongda.top

[U90] JS：数字数组排序
来源：http://mim.andypj.xyz

[...arr].sort((a, b) => a - b)
来源：http://rlp.yongpay.top


<!-- 参考信息 -->