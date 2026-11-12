代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://abz.tanke756.top

[S59] C++：静态断言
来源：http://vsm.bjfxy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fqc.haohaochexian.top

[S60] C++：遍历并删除元素
来源：http://dqe.52xcode.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nti.ywan-chungtsiang.top

================================================================================
来源：http://mij.316326.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vci.gotoacloud.top

================================================================================
来源：http://ucr.chenzaomai.com

[T01] Kotlin：Hello World
来源：http://ryq.kuanghao11.cn

println("Hello")
来源：http://iyo.cashguo.top

[T02] Kotlin：变量
来源：http://hhv.gotoacloud.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tct.gaohongyu789.top

[T03] Kotlin：字符串模板
来源：http://cjl.tian-w.cn

"值: $b"
来源：http://iso.hnxiangtu.top

[T04] Kotlin：空安全
来源：http://nwp.cheryme.top

val n: String? = null;  n?.length
来源：http://mos.hnqzz.top

[T05] Kotlin：when 表达式
来源：http://swi.jqgfzy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lsd.redwolf501.top

[T06] Kotlin：集合映射
来源：http://ndg.meibo888.top

listOf(1, 2, 3).map { it * 2 }
来源：http://egp.smart0.xyz

[T07] Kotlin：集合过滤
来源：http://qug.cucudq.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://hgg.hongshengwenyu.top

[T08] Kotlin：数据类
来源：http://toj.gaohongyu789.top

data class User(val name: String, val age: Int)
来源：http://zyd.mhx1999.top

[T09] Kotlin：扩展函数
来源：http://zvc.bbcook.cn

fun String.exclaim() = this + "!"
来源：http://srm.tianlin.xyz

[T10] Kotlin：默认参数
来源：http://cro.chenzaomai.com

fun greet(name: String = "World") = "Hi $name"
来源：http://isn.sxryk.cn

[T11] Kotlin：协程
来源：http://obl.gaohongyu789.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://swg.ehwqpu.com

[T12] Kotlin：解构声明
来源：http://ymo.sysykeji.top

val (a, b) = Pair(1, 2)
来源：http://leu.sysykeji.top

[T13] Kotlin：只读 Map
来源：http://ykx.hongshengwenyu.top

val m = mapOf("a" to 1)
来源：http://tsa.yvedp.cn

[T14] Kotlin：循环
来源：http://zwa.zhoulong.xyz

for (i in 1..10) println(i)
来源：http://fia.tarul.cn

[T15] Kotlin：接口
来源：http://rwo.ehwqpu.com

interface Shape { fun area(): Double }
来源：http://gog.shanyushiyangtech.top

[T16] Swift：Hello World
来源：http://qej.birdmap.top

print("Hello")
来源：http://jrq.xuanzx.com

[T17] Swift：变量与常量
来源：http://qnz.kuanghao11.cn

var a = 1;  let b = 2
来源：http://oxp.tanke756.top

[T18] Swift：字符串插值
来源：http://som.jyoumei.cn

"值: \(b)"
来源：http://xii.feifeiyinyue.top

[T19] Swift：可选绑定
来源：http://wes.vqdsnc.cn

if let n = opt { print(n) }
来源：http://mkk.aibaodan.cn

[T20] Swift：数组操作
来源：http://gkr.hcnkem.com

var a = [1, 2, 3];  a.append(4)
来源：http://uzl.9152youxi.cn

[T21] Swift：遍历
来源：http://wqf.jlsjyb.cn

for x in a { print(x) }
来源：http://ubx.sweek.top

[T22] Swift：字典
来源：http://vqm.xuanzx.com

var d = ["a": 1];  d["b"] = 2
来源：http://qsf.bjfxy.top

[T23] Swift：函数
来源：http://kll.yfazqb.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ghs.cashguo.top

[T24] Swift：闭包
来源：http://osf.zycfv.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://wjn.xinyue.icu

[T25] Swift：结构体
来源：http://dxc.tanke756.top

struct P { var x: Int }
来源：http://iwy.vqdsnc.cn

[T26] Swift：类与重写
来源：http://jhv.yueranfly.top

class A: Base { override func f() {} }
来源：http://ayk.jlsjyb.cn

[T27] Swift：错误处理
来源：http://mlq.ywan-chungtsiang.top

do { try f() } catch { print(error) }
来源：http://qjr.zhongyouzk.top

[T28] Swift：枚举
来源：http://xaq.iojbl.cn

enum Color { case red, green }
来源：http://sng.hongshengwenyu.top

[T29] Swift：guard 提前返回
来源：http://fyu.wangdashe.top

guard let x = opt else { return }
来源：http://mnk.sjlbkw.cn

[T30] Swift：协议
来源：http://bwj.xuanzx.com

protocol Shape { func area() -> Double }
来源：http://piv.zhijiandao.cn

[T31] Lua：Hello World
来源：http://ijn.ybcxt.top

print("Hello")
来源：http://cqe.bbcook.cn

[T32] Lua：局部变量
来源：http://jom.hammf.cn

local a = 1
来源：http://bvl.jinqigfzy.top

[T33] Lua：表（数组）
来源：http://yek.tian-w.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ydw.ybcxt.top

[T34] Lua：遍历表
来源：http://hhb.hcnkem.com

for i, v in ipairs(t) do print(i, v) end
来源：http://wqm.yangfankeji.com

[T35] Lua：字典表
来源：http://fzu.sufxvd.cn

local d = { a = 1 };  d.b = 2
来源：http://kyg.zhongyouzk.top

[T36] Lua：函数
来源：http://wxt.ywan-chungtsiang.top

function add(a, b) return a + b end
来源：http://cse.jinqigufen.top

[T37] Lua：字符串拼接
来源：http://kxz.ydzc1.top

"a" .. "b"
来源：http://uhi.yonumen.top

[T38] Lua：条件
来源：http://vxy.chenjidiqi.icu

if x > 0 then print("正") end
来源：http://rhh.fktsv.cn

[T39] Lua：模式匹配
来源：http://ebc.xuetiantiany.cn

string.find(s, "%d+")
来源：http://nyd.ydjk.org.cn

[T40] Lua：元表
来源：http://jve.fzhhl.top

setmetatable({}, { __index = base })
来源：http://wfr.andypj.xyz

[T41] Perl：Hello World
来源：http://jmv.jinghuilouyu.cn

print "Hello\n";
来源：http://mds.fzhhl.top

[T42] Perl：变量类型
来源：http://otp.0kj1m.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dto.hnxiangtu.top

[T43] Perl：字符串插值
来源：http://thw.hywenlv.cn

"值: $a"
来源：http://nme.zhongyouzk.top

[T44] Perl：条件
来源：http://pif.jianghu66.top

if ($a > 0) { print "正"; }
来源：http://qkr.redwolf501.top

[T45] Perl：数组遍历
来源：http://ugx.jianghu66.top

for my $x (@arr) { print $x; }
来源：http://muk.xingfuxueyuan.xyz

[T46] Perl：哈希操作
来源：http://ohe.xuanzx.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://drx.nanxinkj.top

[T47] Perl：正则捕获
来源：http://sxw.yanxiufei.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://scm.yfazqb.com

[T48] Perl：正则替换
来源：http://jup.ivvv.top

$s =~ s/old/new/g;
来源：http://att.jianghu66.top

[T49] Perl：函数
来源：http://vqj.zdqjudy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fen.sxryk.cn

[T50] Perl：逐行读文件
来源：http://sqb.shuidangran.top

open my $fh, "<", "a.txt" or die $!;
来源：http://klb.yj202588.top

while (my $line = <$fh>) { print $line; }
来源：http://pcc.chenjidiqi.icu

[T51] Scala：Hello World
来源：http://jaq.shangyingyoupin.top

println("Hello")
来源：http://hab.uphjek.com

[T52] Scala：变量
来源：http://rkl.daxiang520.top

val a = 1;  var b = 2
来源：http://mje.jinghuilouyu.cn

[T53] Scala：字符串插值
来源：http://irn.sufxvd.cn

s"值: $b"
来源：http://mqw.redwolf501.top

[T54] Scala：集合映射
来源：http://mus.fehbvm.com

List(1, 2, 3).map(_ * 2)
来源：http://gjx.zhiwuduotai.top

[T55] Scala：集合过滤
来源：http://hyf.hesvh.cn

List(1, 2, 3).filter(_ > 1)
来源：http://afp.birdmap.top

[T56] Scala：样例类
来源：http://liq.52xcode.cn

case class User(name: String, age: Int)
来源：http://abr.hesvh.cn

[T57] Scala：模式匹配
来源：http://fqr.nanxinkj.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://jpf.hnxiangtu.top

[T58] Scala：函数定义
来源：http://leq.ivvv.top

def add(a: Int, b: Int): Int = a + b
来源：http://wkl.yfazqb.com

[T59] Scala：循环
来源：http://aeq.shzxlz.cn

for (i <- 1 to 10) println(i)
来源：http://wzd.smart0.xyz

[T60] Scala：折叠
来源：http://vlw.ybcxt.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hvv.zhongyouzk.top

================================================================================
来源：http://mpy.hnqzz.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://psh.zdbjq.cn

================================================================================
来源：http://ajh.hesvh.cn

[U01] Py：创建虚拟环境
来源：http://tsg.dianchejie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://umy.sysykeji.top

[U02] Py：导出 / 安装依赖
来源：http://xuy.aibaodan.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zqg.sysykeji.top

[U03] Py：加载 .env 配置
来源：http://uhh.xuanzx.com

from dotenv import load_dotenv; load_dotenv()
来源：http://mqq.jinqigfzy.top

[U04] Py：变量调试打印
来源：http://trk.chenzaomai.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bal.yj20258.top

[U05] Py：列表去重且保序
来源：http://eff.meibo888.top

list(dict.fromkeys(arr))
来源：http://ado.shanyushiyangtech.top

[U06] Py：合并两个字典
来源：http://hjm.yfazqb.com

{**a, **b}
来源：http://img.ydzc1.top

[U07] Py：反转字典键值
来源：http://ifv.nanxuanxn.top

{v: k for k, v in d.items()}
来源：http://gwt.hnqzz.top

[U08] Py：展平二维列表
来源：http://hzo.zdbjq.cn

[y for x in nested for y in x]
来源：http://ltk.sjlbkw.cn

[U09] Py：字典取最大值的键
来源：http://mha.guannengcc.top

max(d, key=d.get)
来源：http://rne.gogol.net.cn

[U10] Py：按值排序字典
来源：http://qik.feifeiyinyue.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://weh.jinqigfzy.top

[U11] Py：生成器表达式
来源：http://bbz.sxryk.cn

(x * 2 for x in arr)
来源：http://upv.gaohongyu789.top

[U12] Py：取出现最多的 3 个元素
来源：http://nop.jiagoushi.top

Counter(arr).most_common(3)
来源：http://pia.guowangkeji.top

[U13] Py：固定长度队列
来源：http://oxi.yfazqb.com

deque(maxlen=10)
来源：http://kbv.fzhhl.top

[U14] Py：分组收集到列表
来源：http://vyc.0kj1m.cn

defaultdict(list)
来源：http://qkp.fktsv.cn

[U15] Py：高精度计时
来源：http://xdc.kuanghao11.cn

t = time.perf_counter()
来源：http://nyi.xinyue.icu

[U16] Py：命令行参数解析
来源：http://llr.zhongyouzk.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://aqj.nanxinkj.top

[U17] Py：初始化日志
来源：http://wbb.cdnleiting.top

logging.basicConfig(level=logging.INFO)
来源：http://siy.gotoacloud.top

[U18] Py：预编译正则
来源：http://qfx.nanxuanxn.top

pat = re.compile(r"\d+")
来源：http://utm.shanyushiyangtech.top

[U19] Py：正则替换带回调
来源：http://umz.hnxiangtu.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vmm.hnxiangtu.top

[U20] Py：缓存函数结果
来源：http://ioe.sjlbkw.cn

@functools.lru_cache(maxsize=None)
来源：http://fjr.9152youxi.cn

[U21] Py：自定义上下文管理器
来源：http://edr.aizwys.cn

@contextlib.contextmanager
来源：http://xfo.xuetiantiany.cn

[U22] Py：矩阵转置
来源：http://bup.sweek.top

list(zip(*m))
来源：http://sdg.52xcode.cn

[U23] Py：分块读取大文件
来源：http://ypw.xuetiantiany.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://sur.cqqwz.cn

[U24] Py：路径操作
来源：http://qrn.xinyue.icu

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jih.xuanzx.com

[U25] Py：CSV 按字典读
来源：http://fhe.pycfn.com

csv.DictReader(f)
来源：http://wuk.gzhubu.top

[U26] Py：并发下载
来源：http://moc.zhengqikj.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kns.yfazqb.com

[U27] Py：异步 HTTP
来源：http://ekn.jinghuilouyu.cn

aiohttp.ClientSession() 配合 async with
来源：http://klo.ydjk.org.cn

[U28] Py：类型别名
来源：http://drs.chenjidiqi.icu

UserId = int
来源：http://itr.chenlongwang.top

[U29] Py：属性校验
来源：http://ack.cdnleiting.top

@property 与 @x.setter 配合
来源：http://cfq.havefunace.top

[U30] Py：数据类
来源：http://qqk.uphjek.com

@dataclass(slots=True)
来源：http://ped.pengpengdd.cyou

[U31] Py：单测
来源：http://cod.yuanzhike.top

python -m pytest -q
来源：http://bri.jiagoushi.top

[U32] Py：代码格式化
来源：http://ikw.xylfe.cn

ruff format . && ruff check --fix .
来源：http://mkt.kuanghao11.cn

[U33] Py：打包发布
来源：http://rxv.hcnkem.com

python -m build  （依赖 pyproject.toml）
来源：http://qwt.cheryme.top

[U34] Py：判断编码
来源：http://vfx.nwbrower.top

chardet.detect(raw)
来源：http://tyl.52xcode.cn

[U35] Py：发送邮件
来源：http://uvc.ctjpmb.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nuv.sweek.top

[U36] Py：定时任务
来源：http://cyl.dashuyun.cn

schedule.every(10).minutes.do(job)
来源：http://laz.chenzaomai.com

[U37] Py：读写 Excel
来源：http://rot.wangdashe.top

pandas.read_excel / DataFrame.to_excel
来源：http://sox.hcnkem.com

[U38] Py：获取脚本所在目录
来源：http://qmb.yanxiufei.cn

Path(__file__).resolve().parent
来源：http://ccg.cucudq.cn

[U39] Py：判断是否在交互环境
来源：http://sab.jinghuilouyu.cn

sys.stdout.isatty()
来源：http://chx.feifeiyinyue.top

[U40] Py：打印到标准错误
来源：http://low.shuidangran.top

print("err", file=sys.stderr)
来源：http://kar.yvedp.cn

[U41] PHP：初始化 Composer 项目
来源：http://tzq.hysaishi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://byx.uphjek.com

[U42] PHP：PSR-4 自动加载
来源：http://czd.xingfuxueyuan.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yox.cucudq.cn

[U43] PHP：声明命名空间
来源：http://hew.xuanzx.com

namespace App\Http;
来源：http://kjb.mhx1999.top

[U44] PHP：开启严格类型
来源：http://ytm.shangyingyoupin.top

declare(strict_types=1);
来源：http://uyx.yanxiufei.cn

[U45] PHP：类型声明与返回类型
来源：http://lzp.yongpay.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://zrz.jinghuilouyu.cn

[U46] PHP：可空类型
来源：http://gwr.hysaishi.cn

?string $name = null
来源：http://pfl.ppjwa.cn

[U47] PHP：联合类型
来源：http://agb.hfpthk.cn

int|string $id
来源：http://ogr.yanxiufei.cn

[U48] PHP：纯枚举
来源：http://ybl.shangyingyoupin.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://xvl.yj202588.top

[U49] PHP：只读属性
来源：http://jvl.jinghuilouyu.cn

public readonly string $name
来源：http://qwg.zdbjq.cn

[U50] PHP：构造器属性提升
来源：http://urj.tian-w.cn

public function __construct(private int $id) {}
来源：http://kqh.jiagoushi.top

[U51] PHP：数组解构
来源：http://yqz.hnqzz.top

[$a, $b] = $arr;
来源：http://you.zhiwuduotai.top

[U52] PHP：箭头函数
来源：http://wjd.xuanzx.com

$double = fn($x) => $x * 2;
来源：http://yfl.daxiang520.top

[U53] PHP：空合并运算符
来源：http://dts.andypj.xyz

$v = $a ?? $b ?? "default";
来源：http://rxz.mhx1999.top

[U54] PHP：空安全调用
来源：http://ymw.yj202588.top

$obj?->method()
来源：http://ngf.xinyue.icu

[U55] PHP：match 表达式
来源：http://osl.jinghuilouyu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://dks.yfazqb.com

[U56] PHP：命名参数
来源：http://fzj.zhaomingkeji.xyz

f(a: 1, b: 2)
来源：http://ezz.gaohongyu789.top

[U57] PHP：字符串插值
来源：http://uea.ivvv.top

"值: {$a}"
来源：http://hif.jinqigufen.top

[U58] PHP：数组三件套
来源：http://can.cdnleiting.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tis.yvedp.cn

[U59] PHP：自定义排序
来源：http://ikk.zhoulong.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://miz.fehbvm.com

[U60] PHP：JSON 编解码
来源：http://dke.chenlongwang.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://flx.gotoacloud.top

[U61] PHP：正则
来源：http://dwy.tanke756.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://jhd.fanxiaobao.xyz

[U62] PHP：日期对象
来源：http://ise.ppjwa.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://tmy.hesvh.cn

[U63] PHP：文件读写
来源：http://xyz.0kj1m.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fgm.cheryme.top

[U64] PHP：目录遍历
来源：http://fdu.shangyingyoupin.top

glob("dir/*.php");  scandir("dir");
来源：http://qjr.hysaishi.cn

[U65] PHP：会话
来源：http://rzi.nanxinkj.top

session_start();  $_SESSION["uid"] = 1;
来源：http://mii.snrcjt.cn

[U66] PHP：设置 Cookie
来源：http://vxr.bjfxy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://fpy.shangyingyoupin.top

[U67] PHP：处理文件上传
来源：http://rwu.shanyushiyangtech.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zjg.sxryk.cn

[U68] PHP：PDO 连接
来源：http://lzj.vqdsnc.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nbd.xziqi.cn

[U69] PHP：PDO 预处理
来源：http://eug.hammf.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jfh.cdnleiting.top

[U70] PHP：PDO 事务
来源：http://vzv.quarkkingdee.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://jst.uphjek.com

[U71] PHP：抛出异常
来源：http://buh.sweek.top

throw new RuntimeException("失败", 500);
来源：http://gph.hnqzz.top

[U72] PHP：写错误日志
来源：http://asb.jinqigufen.top

error_log("失败: " . $e->getMessage());
来源：http://ncn.dianchejie.cn

[U73] PHP：读取 ini 配置
来源：http://qci.yfazqb.com

parse_ini_file("config.ini", true)
来源：http://svn.yanxiufei.cn

[U74] PHP：读取环境变量
来源：http://lxw.snrcjt.cn

getenv("APP_ENV") ?: "production"
来源：http://dzo.jinyuanbaomall.cn

[U75] PHP：依赖注入
来源：http://nxk.jianghu66.top

composer require psr/container
来源：http://gav.nanxuanxn.top

[U76] PHP：简单路由
来源：http://sxx.nwbrower.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fsd.zhiwuduotai.top

[U77] PHP：模板渲染
来源：http://stc.zdqjudy.top

composer require twig/twig
来源：http://gpk.yangfankeji.com

[U78] PHP：单元测试
来源：http://ept.zhoulong.xyz

composer require --dev phpunit/phpunit
来源：http://ayz.chenzaomai.com

[U79] PHP：静态分析
来源：http://gyk.fanxiaobao.xyz

composer require --dev phpstan/phpstan
来源：http://qpg.fzhhl.top

[U80] PHP：代码规范修复
来源：http://ggv.xuetiantiany.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://etp.hywenlv.cn

[U81] JS：初始化项目
来源：http://zen.dianchejie.cn

npm init -y;  npm i express
来源：http://jbu.yj202588.top

[U82] JS：package.json 脚本
来源：http://nur.jqgfzy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ehi.havefunace.top

[U83] JS：ES Module 导入导出
来源：http://kfa.daria6918.cn

export const a = 1;  import { a } from "./m.js";
来源：http://koa.9152youxi.cn

[U84] JS：CommonJS 写法
来源：http://nlt.cashguo.top

module.exports = { a };  const { a } = require("./m");
来源：http://gpr.ydjk.org.cn


<!-- 参考信息 -->