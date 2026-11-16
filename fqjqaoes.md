代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://qje.ppjwa.cn

[S59] C++：静态断言
来源：http://gjj.quarkkingdee.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://znz.yongpay.top

[S60] C++：遍历并删除元素
来源：http://iyu.tianlin.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://aow.fengsongda.top

================================================================================
来源：http://tbw.fzhhl.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://csk.pengpengdd.cyou

================================================================================
来源：http://ssm.ydzc1.top

[T01] Kotlin：Hello World
来源：http://oss.yangfankeji.com

println("Hello")
来源：http://czh.yueranfly.top

[T02] Kotlin：变量
来源：http://zkw.ppjwa.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://iiq.vqdsnc.cn

[T03] Kotlin：字符串模板
来源：http://fbx.zdqjudy.top

"值: $b"
来源：http://zgy.fengsongda.top

[T04] Kotlin：空安全
来源：http://mpj.ydzc1.top

val n: String? = null;  n?.length
来源：http://jxd.zhoulong.xyz

[T05] Kotlin：when 表达式
来源：http://etm.svipenyu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rfr.hywenlv.cn

[T06] Kotlin：集合映射
来源：http://xkc.dashuyun.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://cno.pengpengdd.cyou

[T07] Kotlin：集合过滤
来源：http://dwa.xinyue.icu

listOf(1, 2, 3).filter { it > 1 }
来源：http://arg.hysaishi.cn

[T08] Kotlin：数据类
来源：http://pda.yj20258.top

data class User(val name: String, val age: Int)
来源：http://azw.svipenyu.cn

[T09] Kotlin：扩展函数
来源：http://yqy.nanxuanxn.top

fun String.exclaim() = this + "!"
来源：http://xpq.fzhhl.top

[T10] Kotlin：默认参数
来源：http://dpk.zhoulong.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://cnx.52xcode.cn

[T11] Kotlin：协程
来源：http://zpv.hysaishi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://knz.aizwys.cn

[T12] Kotlin：解构声明
来源：http://ljd.gotoacloud.top

val (a, b) = Pair(1, 2)
来源：http://zng.quarkkingdee.top

[T13] Kotlin：只读 Map
来源：http://quz.ywan-chungtsiang.top

val m = mapOf("a" to 1)
来源：http://nrv.nwbrower.top

[T14] Kotlin：循环
来源：http://klv.nwbrower.top

for (i in 1..10) println(i)
来源：http://yov.316326.xyz

[T15] Kotlin：接口
来源：http://uop.dianchejie.cn

interface Shape { fun area(): Double }
来源：http://byk.jianghu66.top

[T16] Swift：Hello World
来源：http://juw.yj20258.top

print("Hello")
来源：http://mhp.chenlongwang.top

[T17] Swift：变量与常量
来源：http://dny.jinqigufen.top

var a = 1;  let b = 2
来源：http://zrs.wangshuangyany.cn

[T18] Swift：字符串插值
来源：http://jle.haohaochexian.top

"值: \(b)"
来源：http://pnn.zdqjudy.top

[T19] Swift：可选绑定
来源：http://qmm.ydzc1.top

if let n = opt { print(n) }
来源：http://jhq.nanxinkj.top

[T20] Swift：数组操作
来源：http://nyj.tanke756.top

var a = [1, 2, 3];  a.append(4)
来源：http://vwy.xuetiantiany.cn

[T21] Swift：遍历
来源：http://jtz.feifeiyinyue.top

for x in a { print(x) }
来源：http://tdi.yuxming.cn

[T22] Swift：字典
来源：http://fts.sufxvd.cn

var d = ["a": 1];  d["b"] = 2
来源：http://bzh.cashguo.top

[T23] Swift：函数
来源：http://wrx.svipenyu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://orf.uphjek.com

[T24] Swift：闭包
来源：http://jga.svipenyu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xyp.zhixingplan.top

[T25] Swift：结构体
来源：http://rfh.fanxiaobao.xyz

struct P { var x: Int }
来源：http://tfj.nwbrower.top

[T26] Swift：类与重写
来源：http://bsx.yonumen.top

class A: Base { override func f() {} }
来源：http://uod.ydjk.org.cn

[T27] Swift：错误处理
来源：http://ysb.zhixingplan.top

do { try f() } catch { print(error) }
来源：http://mnw.jiagoushi.top

[T28] Swift：枚举
来源：http://cdu.pycfn.com

enum Color { case red, green }
来源：http://ubt.fanxiaobao.xyz

[T29] Swift：guard 提前返回
来源：http://tbf.sjlbkw.cn

guard let x = opt else { return }
来源：http://rhr.cqqwz.cn

[T30] Swift：协议
来源：http://plj.guannengcc.top

protocol Shape { func area() -> Double }
来源：http://wpz.daria6918.cn

[T31] Lua：Hello World
来源：http://lnm.jinghuilouyu.cn

print("Hello")
来源：http://wtq.shzxlz.cn

[T32] Lua：局部变量
来源：http://kyc.52xcode.cn

local a = 1
来源：http://ewc.jinyuanbaomall.cn

[T33] Lua：表（数组）
来源：http://imm.vehdjk.com

local t = {1, 2, 3};  t[4] = 4
来源：http://eox.shuidangran.top

[T34] Lua：遍历表
来源：http://lmy.ppjwa.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://mjs.yfazqb.com

[T35] Lua：字典表
来源：http://wyj.daria6918.cn

local d = { a = 1 };  d.b = 2
来源：http://pju.iojbl.cn

[T36] Lua：函数
来源：http://ntw.bjfxy.top

function add(a, b) return a + b end
来源：http://yjw.yueranfly.top

[T37] Lua：字符串拼接
来源：http://rgh.xuanzx.com

"a" .. "b"
来源：http://pqe.shzxlz.cn

[T38] Lua：条件
来源：http://def.xinyue.icu

if x > 0 then print("正") end
来源：http://aro.haohaochexian.top

[T39] Lua：模式匹配
来源：http://zzw.snrcjt.cn

string.find(s, "%d+")
来源：http://rhg.kuanghao11.cn

[T40] Lua：元表
来源：http://iuu.jlsjyb.cn

setmetatable({}, { __index = base })
来源：http://jqc.jinqigfzy.top

[T41] Perl：Hello World
来源：http://fav.hnxiangtu.top

print "Hello\n";
来源：http://ecf.jlsjyb.cn

[T42] Perl：变量类型
来源：http://xcw.zycfv.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fju.chenzaomai.com

[T43] Perl：字符串插值
来源：http://nir.snrcjt.cn

"值: $a"
来源：http://hzr.fktsv.cn

[T44] Perl：条件
来源：http://ant.pengpengdd.cyou

if ($a > 0) { print "正"; }
来源：http://rah.wangdashe.top

[T45] Perl：数组遍历
来源：http://hgf.zhaomingkeji.xyz

for my $x (@arr) { print $x; }
来源：http://fkp.fanxiaobao.xyz

[T46] Perl：哈希操作
来源：http://sgu.andypj.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://scd.redwolf501.top

[T47] Perl：正则捕获
来源：http://xpo.jqgufenzy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://urm.kuanghao11.cn

[T48] Perl：正则替换
来源：http://gmy.ehwqpu.com

$s =~ s/old/new/g;
来源：http://fjk.shanyushiyangkeji.top

[T49] Perl：函数
来源：http://fid.smart0.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bfi.shzxlz.cn

[T50] Perl：逐行读文件
来源：http://nqr.svipenyu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zyw.yj202588.top

while (my $line = <$fh>) { print $line; }
来源：http://sen.smart0.xyz

[T51] Scala：Hello World
来源：http://odt.zhengqikj.top

println("Hello")
来源：http://bpo.dianchejie.cn

[T52] Scala：变量
来源：http://xeu.zhixingplan.top

val a = 1;  var b = 2
来源：http://hgg.shanyushiyangtech.top

[T53] Scala：字符串插值
来源：http://ulb.zhengqikj.top

s"值: $b"
来源：http://hjf.xinyue.icu

[T54] Scala：集合映射
来源：http://jls.shuidangran.top

List(1, 2, 3).map(_ * 2)
来源：http://ypy.cheryme.top

[T55] Scala：集合过滤
来源：http://hlr.birdmap.top

List(1, 2, 3).filter(_ > 1)
来源：http://azz.hysaishi.cn

[T56] Scala：样例类
来源：http://nmi.iojbl.cn

case class User(name: String, age: Int)
来源：http://zjv.yuxming.cn

[T57] Scala：模式匹配
来源：http://ysv.hywenlv.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://nig.zdqjudy.top

[T58] Scala：函数定义
来源：http://csl.pycfn.com

def add(a: Int, b: Int): Int = a + b
来源：http://rtc.hcnkem.com

[T59] Scala：循环
来源：http://uad.snrcjt.cn

for (i <- 1 to 10) println(i)
来源：http://nzl.pengpengdd.cyou

[T60] Scala：折叠
来源：http://ctt.tanke756.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://afw.zhixingplan.top

================================================================================
来源：http://hrz.haohaochexian.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kku.andypj.xyz

================================================================================
来源：http://ivf.hywenlv.cn

[U01] Py：创建虚拟环境
来源：http://fzi.bjfxy.top

python -m venv .venv && source .venv/bin/activate
来源：http://cka.xziqi.cn

[U02] Py：导出 / 安装依赖
来源：http://pqm.nanxinkj.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zno.jlsjyb.cn

[U03] Py：加载 .env 配置
来源：http://hdi.jyoumei.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ydv.jinqigufen.top

[U04] Py：变量调试打印
来源：http://afv.jqgfzy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vgf.daxiang520.top

[U05] Py：列表去重且保序
来源：http://lpy.tian-w.cn

list(dict.fromkeys(arr))
来源：http://ile.fengsongda.top

[U06] Py：合并两个字典
来源：http://iyu.nanxinkj.top

{**a, **b}
来源：http://gbo.aibaodan.cn

[U07] Py：反转字典键值
来源：http://xko.jinyuanbaomall.cn

{v: k for k, v in d.items()}
来源：http://yax.sysykeji.top

[U08] Py：展平二维列表
来源：http://zyc.jyoumei.cn

[y for x in nested for y in x]
来源：http://gnp.chenzaomai.com

[U09] Py：字典取最大值的键
来源：http://qen.ybcxt.top

max(d, key=d.get)
来源：http://jre.nanxuanxn.top

[U10] Py：按值排序字典
来源：http://elt.sufxvd.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xsc.yuxming.cn

[U11] Py：生成器表达式
来源：http://llc.yj20258888.top

(x * 2 for x in arr)
来源：http://uxg.svipenyu.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ote.bbcook.cn

Counter(arr).most_common(3)
来源：http://xzu.pengpengdd.cyou

[U13] Py：固定长度队列
来源：http://nxu.shzxlz.cn

deque(maxlen=10)
来源：http://kmy.svipenyu.cn

[U14] Py：分组收集到列表
来源：http://ubx.gogol.net.cn

defaultdict(list)
来源：http://hsk.jlsjyb.cn

[U15] Py：高精度计时
来源：http://wqz.52xcode.cn

t = time.perf_counter()
来源：http://tfd.chenlongwang.top

[U16] Py：命令行参数解析
来源：http://vwd.yfazqb.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://eta.gotoacloud.top

[U17] Py：初始化日志
来源：http://tlq.shuidangran.top

logging.basicConfig(level=logging.INFO)
来源：http://kay.ppjwa.cn

[U18] Py：预编译正则
来源：http://pjb.chenjidiqi.icu

pat = re.compile(r"\d+")
来源：http://dgl.cdnleiting.top

[U19] Py：正则替换带回调
来源：http://qvn.jinqigfzy.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://msb.hfpthk.cn

[U20] Py：缓存函数结果
来源：http://glc.daria6918.cn

@functools.lru_cache(maxsize=None)
来源：http://zfv.redwolf501.top

[U21] Py：自定义上下文管理器
来源：http://lcd.hesvh.cn

@contextlib.contextmanager
来源：http://lhx.nanxinkj.top

[U22] Py：矩阵转置
来源：http://zij.yj20258888.top

list(zip(*m))
来源：http://xak.gaohongyu789.top

[U23] Py：分块读取大文件
来源：http://ycu.xuanzx.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qjk.hcnkem.com

[U24] Py：路径操作
来源：http://hji.ppjwa.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fsj.c1oappe.top

[U25] Py：CSV 按字典读
来源：http://xgh.svipenyu.cn

csv.DictReader(f)
来源：http://vki.jqgfzy.top

[U26] Py：并发下载
来源：http://vtp.tianlin.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ago.ivvv.top

[U27] Py：异步 HTTP
来源：http://kju.xinyue.icu

aiohttp.ClientSession() 配合 async with
来源：http://nfk.nanxinkj.top

[U28] Py：类型别名
来源：http://jfm.andypj.xyz

UserId = int
来源：http://eji.shanyushiyangtech.top

[U29] Py：属性校验
来源：http://wgc.tarul.cn

@property 与 @x.setter 配合
来源：http://jkw.hammf.cn

[U30] Py：数据类
来源：http://rbg.dianchejie.cn

@dataclass(slots=True)
来源：http://djy.pengpengdd.cyou

[U31] Py：单测
来源：http://bns.hnxiangtu.top

python -m pytest -q
来源：http://aqz.daria6918.cn

[U32] Py：代码格式化
来源：http://mua.hnqzz.top

ruff format . && ruff check --fix .
来源：http://tdc.zhixingplan.top

[U33] Py：打包发布
来源：http://xfb.gogol.net.cn

python -m build  （依赖 pyproject.toml）
来源：http://bep.tianlin.xyz

[U34] Py：判断编码
来源：http://xml.uphjek.com

chardet.detect(raw)
来源：http://fwz.shanyushiyangtech.top

[U35] Py：发送邮件
来源：http://ico.xingfuxueyuan.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://yhz.xinyue.icu

[U36] Py：定时任务
来源：http://rjw.cdnleiting.top

schedule.every(10).minutes.do(job)
来源：http://oyx.cdnleiting.top

[U37] Py：读写 Excel
来源：http://nsh.yanxiufei.cn

pandas.read_excel / DataFrame.to_excel
来源：http://tmo.ppjwa.cn

[U38] Py：获取脚本所在目录
来源：http://gge.yangfankeji.com

Path(__file__).resolve().parent
来源：http://puh.tanke756.top

[U39] Py：判断是否在交互环境
来源：http://jaf.tianlin.xyz

sys.stdout.isatty()
来源：http://jdm.nanxuanxn.top

[U40] Py：打印到标准错误
来源：http://tdy.redwolf501.top

print("err", file=sys.stderr)
来源：http://ket.andypj.xyz

[U41] PHP：初始化 Composer 项目
来源：http://caz.zhixingplan.top

composer init;  composer require guzzlehttp/guzzle
来源：http://tvm.9152youxi.cn

[U42] PHP：PSR-4 自动加载
来源：http://vla.xuanzx.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vxh.jlsjyb.cn

[U43] PHP：声明命名空间
来源：http://vjs.sxryk.cn

namespace App\Http;
来源：http://wog.xuetiantiany.cn

[U44] PHP：开启严格类型
来源：http://clb.hcnkem.com

declare(strict_types=1);
来源：http://zyx.yuanzhike.top

[U45] PHP：类型声明与返回类型
来源：http://axq.fanxiaobao.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://hxh.yuxming.cn

[U46] PHP：可空类型
来源：http://gif.aibaodan.cn

?string $name = null
来源：http://naz.ehwqpu.com

[U47] PHP：联合类型
来源：http://rox.gogol.net.cn

int|string $id
来源：http://xwo.yuanzhike.top

[U48] PHP：纯枚举
来源：http://rzc.jinqigufen.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nun.shzxlz.cn

[U49] PHP：只读属性
来源：http://dpi.c1oappe.top

public readonly string $name
来源：http://gfh.zdqjudy.top

[U50] PHP：构造器属性提升
来源：http://dzp.xuetiantiany.cn

public function __construct(private int $id) {}
来源：http://ynt.aibaodan.cn

[U51] PHP：数组解构
来源：http://ngy.jqgufenzy.top

[$a, $b] = $arr;
来源：http://tem.ydjk.org.cn

[U52] PHP：箭头函数
来源：http://owj.jinqigufen.top

$double = fn($x) => $x * 2;
来源：http://cck.pycfn.com

[U53] PHP：空合并运算符
来源：http://qiz.aibaodan.cn

$v = $a ?? $b ?? "default";
来源：http://ori.jqgufenzy.top

[U54] PHP：空安全调用
来源：http://eco.zdbjq.cn

$obj?->method()
来源：http://pcv.bjfxy.top

[U55] PHP：match 表达式
来源：http://trp.gotoacloud.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jft.yj20258.top

[U56] PHP：命名参数
来源：http://ipn.jqgufenzy.top

f(a: 1, b: 2)
来源：http://ska.yvedp.cn

[U57] PHP：字符串插值
来源：http://qze.52xcode.cn

"值: {$a}"
来源：http://pig.nwbrower.top

[U58] PHP：数组三件套
来源：http://dlu.0kj1m.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://zdb.chenzaomai.com

[U59] PHP：自定义排序
来源：http://rmv.havefunace.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fyx.52xcode.cn

[U60] PHP：JSON 编解码
来源：http://alo.aibaodan.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://eht.ehwqpu.com

[U61] PHP：正则
来源：http://zew.ivvv.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tjb.jyoumei.cn

[U62] PHP：日期对象
来源：http://dhe.vqdsnc.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gwu.gaohongyu789.top

[U63] PHP：文件读写
来源：http://esf.yj20258888.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gei.zhengqikj.top

[U64] PHP：目录遍历
来源：http://gcx.zdbjq.cn

glob("dir/*.php");  scandir("dir");
来源：http://ppp.zdqjudy.top

[U65] PHP：会话
来源：http://hgk.dashuyun.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://rfn.aibaodan.cn

[U66] PHP：设置 Cookie
来源：http://qlo.nanxuanxn.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://asn.ppjwa.cn

[U67] PHP：处理文件上传
来源：http://pdw.316326.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ybz.aizwys.cn

[U68] PHP：PDO 连接
来源：http://nok.shuidangran.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ppc.yonumen.top

[U69] PHP：PDO 预处理
来源：http://jtp.dianchejie.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://xeb.mhx1999.top

[U70] PHP：PDO 事务
来源：http://cot.zhaomingkeji.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lsp.ctjpmb.com

[U71] PHP：抛出异常
来源：http://xhm.zhongyouzk.top

throw new RuntimeException("失败", 500);
来源：http://abx.ctjpmb.com

[U72] PHP：写错误日志
来源：http://ztk.hywenlv.cn

error_log("失败: " . $e->getMessage());
来源：http://dzk.yuanzhike.top

[U73] PHP：读取 ini 配置
来源：http://kde.zhoulong.xyz

parse_ini_file("config.ini", true)
来源：http://jqz.ywan-chungtsiang.top

[U74] PHP：读取环境变量
来源：http://oig.yj20258.top

getenv("APP_ENV") ?: "production"
来源：http://hsn.xingfuxueyuan.xyz

[U75] PHP：依赖注入
来源：http://pxs.guowangkeji.top

composer require psr/container
来源：http://ltf.kuanghao11.cn

[U76] PHP：简单路由
来源：http://ews.hnqzz.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://hff.gotoacloud.top

[U77] PHP：模板渲染
来源：http://wjt.andypj.xyz

composer require twig/twig
来源：http://odk.yonumen.top

[U78] PHP：单元测试
来源：http://ywk.kuanghao11.cn

composer require --dev phpunit/phpunit
来源：http://mne.yueranfly.top

[U79] PHP：静态分析
来源：http://spd.yongpay.top

composer require --dev phpstan/phpstan
来源：http://loy.316326.xyz

[U80] PHP：代码规范修复
来源：http://wdo.9152youxi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://mbv.yvedp.cn

[U81] JS：初始化项目
来源：http://nmh.cucudq.cn

npm init -y;  npm i express
来源：http://itc.hesvh.cn

[U82] JS：package.json 脚本
来源：http://ofk.hesvh.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://byt.yonumen.top

[U83] JS：ES Module 导入导出
来源：http://rbm.chenzaomai.com

export const a = 1;  import { a } from "./m.js";
来源：http://kyy.52xcode.cn

[U84] JS：CommonJS 写法
来源：http://jqv.shangyingyoupin.top

module.exports = { a };  const { a } = require("./m");
来源：http://wsi.jianghu66.top


<!-- 参考信息 -->