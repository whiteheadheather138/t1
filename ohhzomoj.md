代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bpt.ybcxt.top

[S57] C++：编译期常量
来源：http://wph.yonumen.top

constexpr int N = 10;
来源：http://itw.jqgufenzy.top

[S58] C++：命名空间
来源：http://eyu.gogol.net.cn

namespace ns { int f() { return 1; } }
来源：http://shw.gaohongyu789.top

[S59] C++：静态断言
来源：http://xxc.jqgufenzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hiv.kuanghao11.cn

[S60] C++：遍历并删除元素
来源：http://xxp.birdmap.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kmi.tianlin.xyz

================================================================================
来源：http://qtg.hysaishi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cxd.hnxiangtu.top

================================================================================
来源：http://qyj.tianlin.xyz

[T01] Kotlin：Hello World
来源：http://bcx.andypj.xyz

println("Hello")
来源：http://tie.zhoulong.xyz

[T02] Kotlin：变量
来源：http://njq.hongshengwenyu.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://upl.gzhubu.top

[T03] Kotlin：字符串模板
来源：http://wps.cheryme.top

"值: $b"
来源：http://qvz.ybcxt.top

[T04] Kotlin：空安全
来源：http://qwv.jinghuilouyu.cn

val n: String? = null;  n?.length
来源：http://qni.yueranfly.top

[T05] Kotlin：when 表达式
来源：http://yvs.daxiang520.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zgk.jinqigfzy.top

[T06] Kotlin：集合映射
来源：http://tmi.ivvv.top

listOf(1, 2, 3).map { it * 2 }
来源：http://avv.xingfuxueyuan.xyz

[T07] Kotlin：集合过滤
来源：http://etj.yfazqb.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://ych.jianghu66.top

[T08] Kotlin：数据类
来源：http://ngv.yuanzhike.top

data class User(val name: String, val age: Int)
来源：http://bpw.jqgufenzy.top

[T09] Kotlin：扩展函数
来源：http://yzt.wangdashe.top

fun String.exclaim() = this + "!"
来源：http://ahi.sufxvd.cn

[T10] Kotlin：默认参数
来源：http://fbu.sufxvd.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://irf.gogol.net.cn

[T11] Kotlin：协程
来源：http://nub.yangfankeji.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://wfa.yfazqb.com

[T12] Kotlin：解构声明
来源：http://eyi.chenjidiqi.icu

val (a, b) = Pair(1, 2)
来源：http://fdb.fzhhl.top

[T13] Kotlin：只读 Map
来源：http://vla.sxryk.cn

val m = mapOf("a" to 1)
来源：http://lqu.tanke756.top

[T14] Kotlin：循环
来源：http://cas.hcnkem.com

for (i in 1..10) println(i)
来源：http://ohf.hesvh.cn

[T15] Kotlin：接口
来源：http://beo.andypj.xyz

interface Shape { fun area(): Double }
来源：http://znj.jqgfzy.top

[T16] Swift：Hello World
来源：http://seh.svipenyu.cn

print("Hello")
来源：http://upc.nwbrower.top

[T17] Swift：变量与常量
来源：http://kaj.fanxiaobao.xyz

var a = 1;  let b = 2
来源：http://bsh.jinyuanbaomall.cn

[T18] Swift：字符串插值
来源：http://vjr.gzhubu.top

"值: \(b)"
来源：http://soi.gotoacloud.top

[T19] Swift：可选绑定
来源：http://yzr.gzhubu.top

if let n = opt { print(n) }
来源：http://xid.gzhubu.top

[T20] Swift：数组操作
来源：http://zio.xziqi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ffo.tarul.cn

[T21] Swift：遍历
来源：http://wcr.birdmap.top

for x in a { print(x) }
来源：http://qeq.jinqigfzy.top

[T22] Swift：字典
来源：http://kqb.9152youxi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://jpe.316326.xyz

[T23] Swift：函数
来源：http://xeq.ctjpmb.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yjp.andypj.xyz

[T24] Swift：闭包
来源：http://inq.jqgufenzy.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://hml.zhongyouzk.top

[T25] Swift：结构体
来源：http://lej.jinyuanbaomall.cn

struct P { var x: Int }
来源：http://qej.jyoumei.cn

[T26] Swift：类与重写
来源：http://bgq.mhx1999.top

class A: Base { override func f() {} }
来源：http://ccf.jinqigufen.top

[T27] Swift：错误处理
来源：http://kuo.zhongyouzk.top

do { try f() } catch { print(error) }
来源：http://emf.kuanghao11.cn

[T28] Swift：枚举
来源：http://chj.feifeiyinyue.top

enum Color { case red, green }
来源：http://tma.xziqi.cn

[T29] Swift：guard 提前返回
来源：http://tou.jqgfzy.top

guard let x = opt else { return }
来源：http://jel.9152youxi.cn

[T30] Swift：协议
来源：http://dlk.shanyushiyangtech.top

protocol Shape { func area() -> Double }
来源：http://qqg.jianghu66.top

[T31] Lua：Hello World
来源：http://rfz.sxryk.cn

print("Hello")
来源：http://ftz.zycfv.cn

[T32] Lua：局部变量
来源：http://fcd.hywenlv.cn

local a = 1
来源：http://iwu.hcnkem.com

[T33] Lua：表（数组）
来源：http://auv.sjlbkw.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vnz.xingfuxueyuan.xyz

[T34] Lua：遍历表
来源：http://ifn.xingfuxueyuan.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://pok.ctjpmb.com

[T35] Lua：字典表
来源：http://wsi.ydzc1.top

local d = { a = 1 };  d.b = 2
来源：http://rnx.shzxlz.cn

[T36] Lua：函数
来源：http://bbp.316326.xyz

function add(a, b) return a + b end
来源：http://jee.smart0.xyz

[T37] Lua：字符串拼接
来源：http://qzs.feifeiyinyue.top

"a" .. "b"
来源：http://yve.zycfv.cn

[T38] Lua：条件
来源：http://rib.birdmap.top

if x > 0 then print("正") end
来源：http://yeh.andypj.xyz

[T39] Lua：模式匹配
来源：http://skk.yuxming.cn

string.find(s, "%d+")
来源：http://npp.cheryme.top

[T40] Lua：元表
来源：http://qxq.iojbl.cn

setmetatable({}, { __index = base })
来源：http://ycs.meibo888.top

[T41] Perl：Hello World
来源：http://xhw.kuanghao11.cn

print "Hello\n";
来源：http://skv.fanxiaobao.xyz

[T42] Perl：变量类型
来源：http://ley.tanke756.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mvq.snrcjt.cn

[T43] Perl：字符串插值
来源：http://kcq.sufxvd.cn

"值: $a"
来源：http://bsr.jinghuilouyu.cn

[T44] Perl：条件
来源：http://kjp.zhengqikj.top

if ($a > 0) { print "正"; }
来源：http://mum.jinqigfzy.top

[T45] Perl：数组遍历
来源：http://yaj.sweek.top

for my $x (@arr) { print $x; }
来源：http://ltg.jinyuanbaomall.cn

[T46] Perl：哈希操作
来源：http://gmg.hywenlv.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pwh.xingfuxueyuan.xyz

[T47] Perl：正则捕获
来源：http://ufx.xinyue.icu

if ($s =~ /(\d+)/) { print $1; }
来源：http://nqi.aibaodan.cn

[T48] Perl：正则替换
来源：http://xxw.uphjek.com

$s =~ s/old/new/g;
来源：http://mym.jyoumei.cn

[T49] Perl：函数
来源：http://enn.yueranfly.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://oex.ydjk.org.cn

[T50] Perl：逐行读文件
来源：http://xvp.yuanzhike.top

open my $fh, "<", "a.txt" or die $!;
来源：http://mnk.mhx1999.top

while (my $line = <$fh>) { print $line; }
来源：http://qdd.hywenlv.cn

[T51] Scala：Hello World
来源：http://duy.iojbl.cn

println("Hello")
来源：http://kqa.pycfn.com

[T52] Scala：变量
来源：http://efw.hammf.cn

val a = 1;  var b = 2
来源：http://vfj.cheryme.top

[T53] Scala：字符串插值
来源：http://ftc.iojbl.cn

s"值: $b"
来源：http://uga.feifeiyinyue.top

[T54] Scala：集合映射
来源：http://teg.xuetiantiany.cn

List(1, 2, 3).map(_ * 2)
来源：http://rvi.xylfe.cn

[T55] Scala：集合过滤
来源：http://xij.zhijiandao.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wvb.hnqzz.top

[T56] Scala：样例类
来源：http://wzh.c1oappe.top

case class User(name: String, age: Int)
来源：http://cqv.tianlin.xyz

[T57] Scala：模式匹配
来源：http://wmi.smart0.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://fof.kuanghao11.cn

[T58] Scala：函数定义
来源：http://vgw.yvedp.cn

def add(a: Int, b: Int): Int = a + b
来源：http://qor.chenjidiqi.icu

[T59] Scala：循环
来源：http://acy.cucudq.cn

for (i <- 1 to 10) println(i)
来源：http://osn.zhaomingkeji.xyz

[T60] Scala：折叠
来源：http://tmw.fanxiaobao.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lbn.hcnkem.com

================================================================================
来源：http://ceg.zhaomingkeji.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://smc.xziqi.cn

================================================================================
来源：http://fbv.ywan-chungtsiang.top

[U01] Py：创建虚拟环境
来源：http://tdy.yueranfly.top

python -m venv .venv && source .venv/bin/activate
来源：http://uey.hnqzz.top

[U02] Py：导出 / 安装依赖
来源：http://lrk.gaohongyu789.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pcb.yangfankeji.com

[U03] Py：加载 .env 配置
来源：http://jrx.mhx1999.top

from dotenv import load_dotenv; load_dotenv()
来源：http://txa.yonumen.top

[U04] Py：变量调试打印
来源：http://sgx.gzhubu.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tev.hysaishi.cn

[U05] Py：列表去重且保序
来源：http://ijz.pengpengdd.cyou

list(dict.fromkeys(arr))
来源：http://lqg.jyoumei.cn

[U06] Py：合并两个字典
来源：http://bxi.jqgufenzy.top

{**a, **b}
来源：http://ayp.gzhubu.top

[U07] Py：反转字典键值
来源：http://iwz.chenzaomai.com

{v: k for k, v in d.items()}
来源：http://gal.zhaomingkeji.xyz

[U08] Py：展平二维列表
来源：http://vfl.tarul.cn

[y for x in nested for y in x]
来源：http://hta.yj202588.top

[U09] Py：字典取最大值的键
来源：http://waw.aibaodan.cn

max(d, key=d.get)
来源：http://hoh.guannengcc.top

[U10] Py：按值排序字典
来源：http://zst.pengpengdd.cyou

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kbq.epnwcf.com

[U11] Py：生成器表达式
来源：http://bjz.yuanzhike.top

(x * 2 for x in arr)
来源：http://dpf.jinqigfzy.top

[U12] Py：取出现最多的 3 个元素
来源：http://dun.yfazqb.com

Counter(arr).most_common(3)
来源：http://uij.yonumen.top

[U13] Py：固定长度队列
来源：http://wqf.sxryk.cn

deque(maxlen=10)
来源：http://shc.c1oappe.top

[U14] Py：分组收集到列表
来源：http://vhz.quarkkingdee.top

defaultdict(list)
来源：http://lkm.yj20258.top

[U15] Py：高精度计时
来源：http://mpy.ybcxt.top

t = time.perf_counter()
来源：http://jam.ivvv.top

[U16] Py：命令行参数解析
来源：http://qzj.ppjwa.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bii.yanxiufei.cn

[U17] Py：初始化日志
来源：http://aax.svipenyu.cn

logging.basicConfig(level=logging.INFO)
来源：http://ydf.daxiang520.top

[U18] Py：预编译正则
来源：http://ypl.ydzc1.top

pat = re.compile(r"\d+")
来源：http://dgc.gaohongyu789.top

[U19] Py：正则替换带回调
来源：http://zea.zhixingplan.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://huo.hfpthk.cn

[U20] Py：缓存函数结果
来源：http://bxq.yuanzhike.top

@functools.lru_cache(maxsize=None)
来源：http://ctg.cdnleiting.top

[U21] Py：自定义上下文管理器
来源：http://xmp.guowangkeji.top

@contextlib.contextmanager
来源：http://fqm.shanyushiyangtech.top

[U22] Py：矩阵转置
来源：http://zqn.yj202588.top

list(zip(*m))
来源：http://gfo.hywenlv.cn

[U23] Py：分块读取大文件
来源：http://ugs.0kj1m.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ktg.jqgfzy.top

[U24] Py：路径操作
来源：http://xdi.hnxiangtu.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ckf.kuanghao11.cn

[U25] Py：CSV 按字典读
来源：http://mpl.hnqzz.top

csv.DictReader(f)
来源：http://dgy.aibaodan.cn

[U26] Py：并发下载
来源：http://zyz.fzhhl.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jtm.guannengcc.top

[U27] Py：异步 HTTP
来源：http://htl.xuetiantiany.cn

aiohttp.ClientSession() 配合 async with
来源：http://xyp.ydzc1.top

[U28] Py：类型别名
来源：http://bdu.cheryme.top

UserId = int
来源：http://psf.smart0.xyz

[U29] Py：属性校验
来源：http://wui.yuxming.cn

@property 与 @x.setter 配合
来源：http://rum.iojbl.cn

[U30] Py：数据类
来源：http://tqh.cashguo.top

@dataclass(slots=True)
来源：http://kzu.tanke756.top

[U31] Py：单测
来源：http://jpp.vehdjk.com

python -m pytest -q
来源：http://idp.pengpengdd.cyou

[U32] Py：代码格式化
来源：http://vmm.ctjpmb.com

ruff format . && ruff check --fix .
来源：http://pme.yj202588.top

[U33] Py：打包发布
来源：http://zif.nanxinkj.top

python -m build  （依赖 pyproject.toml）
来源：http://kis.hongshengwenyu.top

[U34] Py：判断编码
来源：http://wuh.hnqzz.top

chardet.detect(raw)
来源：http://dhn.316326.xyz

[U35] Py：发送邮件
来源：http://goz.shanyushiyangtech.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://iir.zdqjudy.top

[U36] Py：定时任务
来源：http://wyl.nanxinkj.top

schedule.every(10).minutes.do(job)
来源：http://rky.gaohongyu789.top

[U37] Py：读写 Excel
来源：http://wxk.cheryme.top

pandas.read_excel / DataFrame.to_excel
来源：http://obz.jianghu66.top

[U38] Py：获取脚本所在目录
来源：http://wbv.nanxuanxn.top

Path(__file__).resolve().parent
来源：http://ceh.hnqzz.top

[U39] Py：判断是否在交互环境
来源：http://cep.dashuyun.cn

sys.stdout.isatty()
来源：http://cij.shzxlz.cn

[U40] Py：打印到标准错误
来源：http://hsb.ydjk.org.cn

print("err", file=sys.stderr)
来源：http://jzs.ywan-chungtsiang.top

[U41] PHP：初始化 Composer 项目
来源：http://leu.hammf.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zyp.zhixingplan.top

[U42] PHP：PSR-4 自动加载
来源：http://tzh.tianlin.xyz

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hoo.yonumen.top

[U43] PHP：声明命名空间
来源：http://tpn.daxiang520.top

namespace App\Http;
来源：http://qkk.chenzaomai.com

[U44] PHP：开启严格类型
来源：http://dbg.pycfn.com

declare(strict_types=1);
来源：http://xiq.tianlin.xyz

[U45] PHP：类型声明与返回类型
来源：http://ush.ydjk.org.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://fbv.nanxinkj.top

[U46] PHP：可空类型
来源：http://gei.sxryk.cn

?string $name = null
来源：http://ybk.shangyingyoupin.top

[U47] PHP：联合类型
来源：http://nhc.yj20258888.top

int|string $id
来源：http://vxk.vqdsnc.cn

[U48] PHP：纯枚举
来源：http://dgn.nanxinkj.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://tgn.ppjwa.cn

[U49] PHP：只读属性
来源：http://vrj.quarkkingdee.top

public readonly string $name
来源：http://jjz.redwolf501.top

[U50] PHP：构造器属性提升
来源：http://yzp.zhixingplan.top

public function __construct(private int $id) {}
来源：http://ihz.fanxiaobao.xyz

[U51] PHP：数组解构
来源：http://hzj.gaohongyu789.top

[$a, $b] = $arr;
来源：http://hgh.wangdashe.top

[U52] PHP：箭头函数
来源：http://uzu.birdmap.top

$double = fn($x) => $x * 2;
来源：http://ftx.jqgfzy.top

[U53] PHP：空合并运算符
来源：http://qyg.jqgfzy.top

$v = $a ?? $b ?? "default";
来源：http://buq.shangyingyoupin.top

[U54] PHP：空安全调用
来源：http://rjx.ctjpmb.com

$obj?->method()
来源：http://vbl.shangyingyoupin.top

[U55] PHP：match 表达式
来源：http://onp.shzxlz.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jlc.smart0.xyz

[U56] PHP：命名参数
来源：http://del.bjfxy.top

f(a: 1, b: 2)
来源：http://gww.zhengqikj.top

[U57] PHP：字符串插值
来源：http://isd.cqqwz.cn

"值: {$a}"
来源：http://nyo.gotoacloud.top

[U58] PHP：数组三件套
来源：http://qaq.haohaochexian.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://res.c1oappe.top

[U59] PHP：自定义排序
来源：http://wyd.xuetiantiany.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://bmx.zhixingplan.top

[U60] PHP：JSON 编解码
来源：http://zum.daxiang520.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://rly.gogol.net.cn

[U61] PHP：正则
来源：http://dvx.316326.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qdd.yueranfly.top

[U62] PHP：日期对象
来源：http://dab.wangdashe.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zuk.fengsongda.top

[U63] PHP：文件读写
来源：http://gdl.zhaomingkeji.xyz

file_get_contents($f);  file_put_contents($f, $data);
来源：http://evq.havefunace.top

[U64] PHP：目录遍历
来源：http://rck.jlsjyb.cn

glob("dir/*.php");  scandir("dir");
来源：http://kbd.yj202588.top

[U65] PHP：会话
来源：http://rqs.aibaodan.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://urz.yonumen.top

[U66] PHP：设置 Cookie
来源：http://vvk.cheryme.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://iyh.wangshuangyany.cn

[U67] PHP：处理文件上传
来源：http://vnx.aizwys.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://utn.shanyushiyangkeji.top

[U68] PHP：PDO 连接
来源：http://wnd.yj202588.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://kmt.sjlbkw.cn

[U69] PHP：PDO 预处理
来源：http://tca.chenlongwang.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://fzd.nanxinkj.top

[U70] PHP：PDO 事务
来源：http://ygg.hfpthk.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gzf.yanxiufei.cn

[U71] PHP：抛出异常
来源：http://lob.yanxiufei.cn

throw new RuntimeException("失败", 500);
来源：http://lta.zdqjudy.top

[U72] PHP：写错误日志
来源：http://pfy.daxiang520.top

error_log("失败: " . $e->getMessage());
来源：http://ixw.dianchejie.cn

[U73] PHP：读取 ini 配置
来源：http://mof.vehdjk.com

parse_ini_file("config.ini", true)
来源：http://eix.xingfuxueyuan.xyz

[U74] PHP：读取环境变量
来源：http://nso.tanke756.top

getenv("APP_ENV") ?: "production"
来源：http://rgl.kuanghao11.cn

[U75] PHP：依赖注入
来源：http://pia.smart0.xyz

composer require psr/container
来源：http://qwq.gotoacloud.top

[U76] PHP：简单路由
来源：http://fqn.zhijiandao.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://rzt.yj20258.top

[U77] PHP：模板渲染
来源：http://dbv.quarkkingdee.top

composer require twig/twig
来源：http://jxq.fktsv.cn

[U78] PHP：单元测试
来源：http://vxd.havefunace.top

composer require --dev phpunit/phpunit
来源：http://rdg.svipenyu.cn

[U79] PHP：静态分析
来源：http://jxy.jqgfzy.top

composer require --dev phpstan/phpstan
来源：http://usg.ydjk.org.cn

[U80] PHP：代码规范修复
来源：http://pac.jqgufenzy.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://tgu.jiagoushi.top

[U81] JS：初始化项目
来源：http://oxg.zhongyouzk.top

npm init -y;  npm i express
来源：http://com.shanyushiyangtech.top

[U82] JS：package.json 脚本
来源：http://kzl.zhengqikj.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://kgo.tianlin.xyz


<!-- 参考信息 -->