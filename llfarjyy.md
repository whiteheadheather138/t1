代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://grk.yfazqb.com

[S55] C++：结构化绑定
来源：http://wyk.tian-w.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://sil.ybcxt.top

[S56] C++：optional
来源：http://gio.redwolf501.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bml.gogol.net.cn

[S57] C++：编译期常量
来源：http://pga.jinqigfzy.top

constexpr int N = 10;
来源：http://veg.yj202588.top

[S58] C++：命名空间
来源：http://nxl.xingfuxueyuan.xyz

namespace ns { int f() { return 1; } }
来源：http://kho.yanxiufei.cn

[S59] C++：静态断言
来源：http://omq.wangshuangyany.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dfs.zdqjudy.top

[S60] C++：遍历并删除元素
来源：http://yht.uphjek.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sgc.shzxlz.cn

================================================================================
来源：http://chl.316326.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tsp.gotoacloud.top

================================================================================
来源：http://vxh.jqgfzy.top

[T01] Kotlin：Hello World
来源：http://ujr.yangfankeji.com

println("Hello")
来源：http://fyn.316326.xyz

[T02] Kotlin：变量
来源：http://lzt.c1oappe.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dqf.daria6918.cn

[T03] Kotlin：字符串模板
来源：http://hkf.zhaomingkeji.xyz

"值: $b"
来源：http://lic.ehwqpu.com

[T04] Kotlin：空安全
来源：http://sie.chenlongwang.top

val n: String? = null;  n?.length
来源：http://cvh.xziqi.cn

[T05] Kotlin：when 表达式
来源：http://dem.cucudq.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bds.9152youxi.cn

[T06] Kotlin：集合映射
来源：http://cic.fzhhl.top

listOf(1, 2, 3).map { it * 2 }
来源：http://qjt.zhaomingkeji.xyz

[T07] Kotlin：集合过滤
来源：http://hxf.daxiang520.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://rht.vehdjk.com

[T08] Kotlin：数据类
来源：http://tph.mhx1999.top

data class User(val name: String, val age: Int)
来源：http://whq.hnxiangtu.top

[T09] Kotlin：扩展函数
来源：http://ejs.hfpthk.cn

fun String.exclaim() = this + "!"
来源：http://sqf.fzhhl.top

[T10] Kotlin：默认参数
来源：http://dah.9152youxi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jwi.xinyue.icu

[T11] Kotlin：协程
来源：http://trl.ivvv.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://oft.cqqwz.cn

[T12] Kotlin：解构声明
来源：http://kmf.zhiwuduotai.top

val (a, b) = Pair(1, 2)
来源：http://oqt.jinyuanbaomall.cn

[T13] Kotlin：只读 Map
来源：http://tbj.xziqi.cn

val m = mapOf("a" to 1)
来源：http://eyp.zhijiandao.cn

[T14] Kotlin：循环
来源：http://ahw.jlsjyb.cn

for (i in 1..10) println(i)
来源：http://wme.zdbjq.cn

[T15] Kotlin：接口
来源：http://ldj.ehwqpu.com

interface Shape { fun area(): Double }
来源：http://rst.xziqi.cn

[T16] Swift：Hello World
来源：http://ffh.zhiwuduotai.top

print("Hello")
来源：http://gmc.yvedp.cn

[T17] Swift：变量与常量
来源：http://fpa.xuetiantiany.cn

var a = 1;  let b = 2
来源：http://syu.9152youxi.cn

[T18] Swift：字符串插值
来源：http://jsc.svipenyu.cn

"值: \(b)"
来源：http://uvh.ydjk.org.cn

[T19] Swift：可选绑定
来源：http://lzx.guannengcc.top

if let n = opt { print(n) }
来源：http://aqy.hnxiangtu.top

[T20] Swift：数组操作
来源：http://ets.epnwcf.com

var a = [1, 2, 3];  a.append(4)
来源：http://vpu.jinqigfzy.top

[T21] Swift：遍历
来源：http://wpb.gogol.net.cn

for x in a { print(x) }
来源：http://kgp.zdbjq.cn

[T22] Swift：字典
来源：http://akx.dianchejie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ckp.kuanghao11.cn

[T23] Swift：函数
来源：http://rgd.chenlongwang.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fvj.hywenlv.cn

[T24] Swift：闭包
来源：http://olw.xuanzx.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://exy.tarul.cn

[T25] Swift：结构体
来源：http://ush.tianlin.xyz

struct P { var x: Int }
来源：http://owi.jlsjyb.cn

[T26] Swift：类与重写
来源：http://xlu.aizwys.cn

class A: Base { override func f() {} }
来源：http://iyh.hammf.cn

[T27] Swift：错误处理
来源：http://hgy.9152youxi.cn

do { try f() } catch { print(error) }
来源：http://vkx.ydjk.org.cn

[T28] Swift：枚举
来源：http://thc.jinyuanbaomall.cn

enum Color { case red, green }
来源：http://gkl.sjlbkw.cn

[T29] Swift：guard 提前返回
来源：http://zho.hywenlv.cn

guard let x = opt else { return }
来源：http://pab.sysykeji.top

[T30] Swift：协议
来源：http://yiu.fanxiaobao.xyz

protocol Shape { func area() -> Double }
来源：http://nez.daria6918.cn

[T31] Lua：Hello World
来源：http://bnm.yanxiufei.cn

print("Hello")
来源：http://ccd.9152youxi.cn

[T32] Lua：局部变量
来源：http://znz.chenzaomai.com

local a = 1
来源：http://lwv.jqgufenzy.top

[T33] Lua：表（数组）
来源：http://fza.wangshuangyany.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://dnp.chenzaomai.com

[T34] Lua：遍历表
来源：http://bnn.epnwcf.com

for i, v in ipairs(t) do print(i, v) end
来源：http://gdw.birdmap.top

[T35] Lua：字典表
来源：http://ykk.316326.xyz

local d = { a = 1 };  d.b = 2
来源：http://bzl.jiagoushi.top

[T36] Lua：函数
来源：http://ncz.52xcode.cn

function add(a, b) return a + b end
来源：http://qte.tarul.cn

[T37] Lua：字符串拼接
来源：http://ykd.zhixingplan.top

"a" .. "b"
来源：http://nit.birdmap.top

[T38] Lua：条件
来源：http://jny.9152youxi.cn

if x > 0 then print("正") end
来源：http://ovd.gaohongyu789.top

[T39] Lua：模式匹配
来源：http://rqq.jinghuilouyu.cn

string.find(s, "%d+")
来源：http://ozy.xinyue.icu

[T40] Lua：元表
来源：http://fhe.fktsv.cn

setmetatable({}, { __index = base })
来源：http://tsb.fengsongda.top

[T41] Perl：Hello World
来源：http://qau.dianchejie.cn

print "Hello\n";
来源：http://qgh.ehwqpu.com

[T42] Perl：变量类型
来源：http://uwb.hongshengwenyu.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ffe.vehdjk.com

[T43] Perl：字符串插值
来源：http://hkg.fanxiaobao.xyz

"值: $a"
来源：http://sci.snrcjt.cn

[T44] Perl：条件
来源：http://nvd.ybcxt.top

if ($a > 0) { print "正"; }
来源：http://zrt.nanxuanxn.top

[T45] Perl：数组遍历
来源：http://zip.gotoacloud.top

for my $x (@arr) { print $x; }
来源：http://dml.jinqigufen.top

[T46] Perl：哈希操作
来源：http://qbb.ehwqpu.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qyb.hysaishi.cn

[T47] Perl：正则捕获
来源：http://kbj.jqgufenzy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://zvp.jinghuilouyu.cn

[T48] Perl：正则替换
来源：http://kke.quarkkingdee.top

$s =~ s/old/new/g;
来源：http://exi.yj20258888.top

[T49] Perl：函数
来源：http://lov.316326.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zob.kuanghao11.cn

[T50] Perl：逐行读文件
来源：http://qhz.shuidangran.top

open my $fh, "<", "a.txt" or die $!;
来源：http://rml.guowangkeji.top

while (my $line = <$fh>) { print $line; }
来源：http://tmw.316326.xyz

[T51] Scala：Hello World
来源：http://yfu.yuxming.cn

println("Hello")
来源：http://ipv.sweek.top

[T52] Scala：变量
来源：http://ffv.iojbl.cn

val a = 1;  var b = 2
来源：http://wjh.c1oappe.top

[T53] Scala：字符串插值
来源：http://wty.guannengcc.top

s"值: $b"
来源：http://npw.uphjek.com

[T54] Scala：集合映射
来源：http://nyp.kuanghao11.cn

List(1, 2, 3).map(_ * 2)
来源：http://eli.wangdashe.top

[T55] Scala：集合过滤
来源：http://nul.yj202588.top

List(1, 2, 3).filter(_ > 1)
来源：http://byk.bjfxy.top

[T56] Scala：样例类
来源：http://hyj.cqqwz.cn

case class User(name: String, age: Int)
来源：http://dma.daxiang520.top

[T57] Scala：模式匹配
来源：http://zel.ppjwa.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://jyb.cheryme.top

[T58] Scala：函数定义
来源：http://sos.yfazqb.com

def add(a: Int, b: Int): Int = a + b
来源：http://pvh.jinyuanbaomall.cn

[T59] Scala：循环
来源：http://whb.vqdsnc.cn

for (i <- 1 to 10) println(i)
来源：http://jgf.yuxming.cn

[T60] Scala：折叠
来源：http://jbv.yangfankeji.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://sme.snrcjt.cn

================================================================================
来源：http://itm.svipenyu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ypa.bjfxy.top

================================================================================
来源：http://kim.bjfxy.top

[U01] Py：创建虚拟环境
来源：http://mpw.fktsv.cn

python -m venv .venv && source .venv/bin/activate
来源：http://din.meibo888.top

[U02] Py：导出 / 安装依赖
来源：http://xoa.redwolf501.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hxm.shuidangran.top

[U03] Py：加载 .env 配置
来源：http://duu.jianghu66.top

from dotenv import load_dotenv; load_dotenv()
来源：http://boy.kuanghao11.cn

[U04] Py：变量调试打印
来源：http://zfe.dianchejie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ins.ppjwa.cn

[U05] Py：列表去重且保序
来源：http://rfp.hcnkem.com

list(dict.fromkeys(arr))
来源：http://scy.shanyushiyangkeji.top

[U06] Py：合并两个字典
来源：http://uhs.xuanzx.com

{**a, **b}
来源：http://bwu.bbcook.cn

[U07] Py：反转字典键值
来源：http://wet.xylfe.cn

{v: k for k, v in d.items()}
来源：http://ouu.xingfuxueyuan.xyz

[U08] Py：展平二维列表
来源：http://dyo.zhongyouzk.top

[y for x in nested for y in x]
来源：http://hqe.chenjidiqi.icu

[U09] Py：字典取最大值的键
来源：http://tin.meibo888.top

max(d, key=d.get)
来源：http://rex.cucudq.cn

[U10] Py：按值排序字典
来源：http://ijd.xinyue.icu

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pwz.c1oappe.top

[U11] Py：生成器表达式
来源：http://gyu.ywan-chungtsiang.top

(x * 2 for x in arr)
来源：http://puk.cdnleiting.top

[U12] Py：取出现最多的 3 个元素
来源：http://hpb.dashuyun.cn

Counter(arr).most_common(3)
来源：http://quu.sjlbkw.cn

[U13] Py：固定长度队列
来源：http://ptm.chenjidiqi.icu

deque(maxlen=10)
来源：http://fyw.sysykeji.top

[U14] Py：分组收集到列表
来源：http://kmd.haohaochexian.top

defaultdict(list)
来源：http://zxm.ybcxt.top

[U15] Py：高精度计时
来源：http://yla.nwbrower.top

t = time.perf_counter()
来源：http://pid.c1oappe.top

[U16] Py：命令行参数解析
来源：http://evg.hysaishi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zih.0kj1m.cn

[U17] Py：初始化日志
来源：http://nyv.hfpthk.cn

logging.basicConfig(level=logging.INFO)
来源：http://cle.jyoumei.cn

[U18] Py：预编译正则
来源：http://zfn.chenzaomai.com

pat = re.compile(r"\d+")
来源：http://mrx.zhaomingkeji.xyz

[U19] Py：正则替换带回调
来源：http://wdg.uphjek.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://igm.c1oappe.top

[U20] Py：缓存函数结果
来源：http://bvd.zhoulong.xyz

@functools.lru_cache(maxsize=None)
来源：http://rdg.epnwcf.com

[U21] Py：自定义上下文管理器
来源：http://kkn.pengpengdd.cyou

@contextlib.contextmanager
来源：http://piv.52xcode.cn

[U22] Py：矩阵转置
来源：http://aip.birdmap.top

list(zip(*m))
来源：http://mtw.zhongyouzk.top

[U23] Py：分块读取大文件
来源：http://jmk.ydjk.org.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://dbm.daxiang520.top

[U24] Py：路径操作
来源：http://eix.shuidangran.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://das.cqqwz.cn

[U25] Py：CSV 按字典读
来源：http://ttg.ybcxt.top

csv.DictReader(f)
来源：http://vdj.mhx1999.top

[U26] Py：并发下载
来源：http://kky.gzhubu.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://eiy.jinghuilouyu.cn

[U27] Py：异步 HTTP
来源：http://sia.xuanzx.com

aiohttp.ClientSession() 配合 async with
来源：http://xgf.hesvh.cn

[U28] Py：类型别名
来源：http://hzj.wangdashe.top

UserId = int
来源：http://una.ybcxt.top

[U29] Py：属性校验
来源：http://nlg.zycfv.cn

@property 与 @x.setter 配合
来源：http://ezg.zhijiandao.cn

[U30] Py：数据类
来源：http://vxp.yj20258888.top

@dataclass(slots=True)
来源：http://lak.cheryme.top

[U31] Py：单测
来源：http://sct.tian-w.cn

python -m pytest -q
来源：http://akl.fehbvm.com

[U32] Py：代码格式化
来源：http://xzk.316326.xyz

ruff format . && ruff check --fix .
来源：http://fzi.epnwcf.com

[U33] Py：打包发布
来源：http://gzq.jianghu66.top

python -m build  （依赖 pyproject.toml）
来源：http://zlu.guowangkeji.top

[U34] Py：判断编码
来源：http://sfe.dashuyun.cn

chardet.detect(raw)
来源：http://gfb.zhongyouzk.top

[U35] Py：发送邮件
来源：http://uyz.iojbl.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jjf.hfpthk.cn

[U36] Py：定时任务
来源：http://grq.gogol.net.cn

schedule.every(10).minutes.do(job)
来源：http://gst.sysykeji.top

[U37] Py：读写 Excel
来源：http://nxd.gotoacloud.top

pandas.read_excel / DataFrame.to_excel
来源：http://owo.nanxinkj.top

[U38] Py：获取脚本所在目录
来源：http://cpg.gzhubu.top

Path(__file__).resolve().parent
来源：http://lpi.dashuyun.cn

[U39] Py：判断是否在交互环境
来源：http://kiv.zhixingplan.top

sys.stdout.isatty()
来源：http://dtx.jinqigfzy.top

[U40] Py：打印到标准错误
来源：http://srs.yueranfly.top

print("err", file=sys.stderr)
来源：http://ngb.shzxlz.cn

[U41] PHP：初始化 Composer 项目
来源：http://tdx.zdbjq.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://kxq.iojbl.cn

[U42] PHP：PSR-4 自动加载
来源：http://qck.xylfe.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dqe.xylfe.cn

[U43] PHP：声明命名空间
来源：http://hoz.gogol.net.cn

namespace App\Http;
来源：http://yfp.fanxiaobao.xyz

[U44] PHP：开启严格类型
来源：http://imm.chenjidiqi.icu

declare(strict_types=1);
来源：http://qqz.yj202588.top

[U45] PHP：类型声明与返回类型
来源：http://xen.52xcode.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jgj.yangfankeji.com

[U46] PHP：可空类型
来源：http://dts.jqgufenzy.top

?string $name = null
来源：http://rhz.zycfv.cn

[U47] PHP：联合类型
来源：http://hnl.jlsjyb.cn

int|string $id
来源：http://gsb.ywan-chungtsiang.top

[U48] PHP：纯枚举
来源：http://vjd.dianchejie.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gqm.cucudq.cn

[U49] PHP：只读属性
来源：http://zsk.vqdsnc.cn

public readonly string $name
来源：http://gks.zdqjudy.top

[U50] PHP：构造器属性提升
来源：http://wqq.yvedp.cn

public function __construct(private int $id) {}
来源：http://zmg.aizwys.cn

[U51] PHP：数组解构
来源：http://ecf.chenjidiqi.icu

[$a, $b] = $arr;
来源：http://iqi.jqgfzy.top

[U52] PHP：箭头函数
来源：http://spe.9152youxi.cn

$double = fn($x) => $x * 2;
来源：http://bhg.yanxiufei.cn

[U53] PHP：空合并运算符
来源：http://kir.jlsjyb.cn

$v = $a ?? $b ?? "default";
来源：http://hng.svipenyu.cn

[U54] PHP：空安全调用
来源：http://sbt.hnxiangtu.top

$obj?->method()
来源：http://mnw.gogol.net.cn

[U55] PHP：match 表达式
来源：http://hff.xziqi.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://lfj.zhengqikj.top

[U56] PHP：命名参数
来源：http://cmf.gaohongyu789.top

f(a: 1, b: 2)
来源：http://ojv.yanxiufei.cn

[U57] PHP：字符串插值
来源：http://jul.yuanzhike.top

"值: {$a}"
来源：http://xlw.yuanzhike.top

[U58] PHP：数组三件套
来源：http://twf.yongpay.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://vpi.fehbvm.com

[U59] PHP：自定义排序
来源：http://rbr.cqqwz.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lyi.wangdashe.top

[U60] PHP：JSON 编解码
来源：http://vaw.zdbjq.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fpr.fktsv.cn

[U61] PHP：正则
来源：http://swk.hnxiangtu.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://tyk.hongshengwenyu.top

[U62] PHP：日期对象
来源：http://mth.shanyushiyangtech.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://xjo.guannengcc.top

[U63] PHP：文件读写
来源：http://oev.dianchejie.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://crn.hnxiangtu.top

[U64] PHP：目录遍历
来源：http://gda.hesvh.cn

glob("dir/*.php");  scandir("dir");
来源：http://nwq.tanke756.top

[U65] PHP：会话
来源：http://ngs.sysykeji.top

session_start();  $_SESSION["uid"] = 1;
来源：http://nez.tarul.cn

[U66] PHP：设置 Cookie
来源：http://aje.sxryk.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://goy.zhiwuduotai.top

[U67] PHP：处理文件上传
来源：http://nvj.vehdjk.com

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kyl.jlsjyb.cn

[U68] PHP：PDO 连接
来源：http://odn.316326.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://axq.chenlongwang.top

[U69] PHP：PDO 预处理
来源：http://sna.pengpengdd.cyou

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zby.yvedp.cn

[U70] PHP：PDO 事务
来源：http://neh.sjlbkw.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nyu.yangfankeji.com

[U71] PHP：抛出异常
来源：http://igs.chenlongwang.top

throw new RuntimeException("失败", 500);
来源：http://ems.jqgufenzy.top

[U72] PHP：写错误日志
来源：http://ihc.ywan-chungtsiang.top

error_log("失败: " . $e->getMessage());
来源：http://wxb.jianghu66.top

[U73] PHP：读取 ini 配置
来源：http://dco.aibaodan.cn

parse_ini_file("config.ini", true)
来源：http://pse.shzxlz.cn

[U74] PHP：读取环境变量
来源：http://eom.chenzaomai.com

getenv("APP_ENV") ?: "production"
来源：http://lbu.sjlbkw.cn

[U75] PHP：依赖注入
来源：http://tyl.pengpengdd.cyou

composer require psr/container
来源：http://rmi.meibo888.top

[U76] PHP：简单路由
来源：http://wdi.tian-w.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lhp.aizwys.cn

[U77] PHP：模板渲染
来源：http://erv.jlsjyb.cn

composer require twig/twig
来源：http://jpn.hywenlv.cn

[U78] PHP：单元测试
来源：http://uxe.jinqigfzy.top

composer require --dev phpunit/phpunit
来源：http://kjk.yongpay.top

[U79] PHP：静态分析
来源：http://row.yfazqb.com

composer require --dev phpstan/phpstan
来源：http://zvu.hysaishi.cn

[U80] PHP：代码规范修复
来源：http://csi.gogol.net.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://gnu.cdnleiting.top


<!-- 参考信息 -->