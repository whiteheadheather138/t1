代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dnj.hammf.cn

[S57] C++：编译期常量
来源：http://bdh.jinqigfzy.top

constexpr int N = 10;
来源：http://knq.sxryk.cn

[S58] C++：命名空间
来源：http://jss.sxryk.cn

namespace ns { int f() { return 1; } }
来源：http://eqj.zdqjudy.top

[S59] C++：静态断言
来源：http://rwi.yj20258888.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jly.meibo888.top

[S60] C++：遍历并删除元素
来源：http://kdk.zhijiandao.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jau.yueranfly.top

================================================================================
来源：http://dam.jqgfzy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rzo.hfpthk.cn

================================================================================
来源：http://qel.wangdashe.top

[T01] Kotlin：Hello World
来源：http://cqf.birdmap.top

println("Hello")
来源：http://gmr.zhiwuduotai.top

[T02] Kotlin：变量
来源：http://zev.vehdjk.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://eyk.dashuyun.cn

[T03] Kotlin：字符串模板
来源：http://gbx.tarul.cn

"值: $b"
来源：http://ylj.gaohongyu789.top

[T04] Kotlin：空安全
来源：http://ckb.havefunace.top

val n: String? = null;  n?.length
来源：http://uhi.havefunace.top

[T05] Kotlin：when 表达式
来源：http://brr.yonumen.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://iag.aibaodan.cn

[T06] Kotlin：集合映射
来源：http://skv.cheryme.top

listOf(1, 2, 3).map { it * 2 }
来源：http://rmz.jqgfzy.top

[T07] Kotlin：集合过滤
来源：http://dqp.zhoulong.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://dqz.redwolf501.top

[T08] Kotlin：数据类
来源：http://ibo.chenlongwang.top

data class User(val name: String, val age: Int)
来源：http://wyx.0kj1m.cn

[T09] Kotlin：扩展函数
来源：http://onq.daria6918.cn

fun String.exclaim() = this + "!"
来源：http://bvn.52xcode.cn

[T10] Kotlin：默认参数
来源：http://iom.pengpengdd.cyou

fun greet(name: String = "World") = "Hi $name"
来源：http://ntd.sysykeji.top

[T11] Kotlin：协程
来源：http://oxw.ybcxt.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://nvc.gotoacloud.top

[T12] Kotlin：解构声明
来源：http://jeh.epnwcf.com

val (a, b) = Pair(1, 2)
来源：http://bij.tian-w.cn

[T13] Kotlin：只读 Map
来源：http://vjl.jqgfzy.top

val m = mapOf("a" to 1)
来源：http://xth.gotoacloud.top

[T14] Kotlin：循环
来源：http://sjt.feifeiyinyue.top

for (i in 1..10) println(i)
来源：http://tho.quarkkingdee.top

[T15] Kotlin：接口
来源：http://two.hysaishi.cn

interface Shape { fun area(): Double }
来源：http://noq.jqgufenzy.top

[T16] Swift：Hello World
来源：http://fsr.daria6918.cn

print("Hello")
来源：http://dgx.hesvh.cn

[T17] Swift：变量与常量
来源：http://xmd.316326.xyz

var a = 1;  let b = 2
来源：http://irs.dianchejie.cn

[T18] Swift：字符串插值
来源：http://mkq.jinghuilouyu.cn

"值: \(b)"
来源：http://frh.jinqigfzy.top

[T19] Swift：可选绑定
来源：http://xnj.sxryk.cn

if let n = opt { print(n) }
来源：http://bnd.gzhubu.top

[T20] Swift：数组操作
来源：http://xpj.guannengcc.top

var a = [1, 2, 3];  a.append(4)
来源：http://jvf.zhengqikj.top

[T21] Swift：遍历
来源：http://umi.aizwys.cn

for x in a { print(x) }
来源：http://dgt.hnqzz.top

[T22] Swift：字典
来源：http://dgl.tarul.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vrl.vehdjk.com

[T23] Swift：函数
来源：http://yoo.pengpengdd.cyou

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vwu.chenzaomai.com

[T24] Swift：闭包
来源：http://hra.nanxinkj.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://owg.pengpengdd.cyou

[T25] Swift：结构体
来源：http://xwp.cdnleiting.top

struct P { var x: Int }
来源：http://ulk.hnqzz.top

[T26] Swift：类与重写
来源：http://jat.cucudq.cn

class A: Base { override func f() {} }
来源：http://gaz.yueranfly.top

[T27] Swift：错误处理
来源：http://wva.zhijiandao.cn

do { try f() } catch { print(error) }
来源：http://tmr.hesvh.cn

[T28] Swift：枚举
来源：http://tok.meibo888.top

enum Color { case red, green }
来源：http://jqb.ywan-chungtsiang.top

[T29] Swift：guard 提前返回
来源：http://qvg.yj20258888.top

guard let x = opt else { return }
来源：http://gzt.zhiwuduotai.top

[T30] Swift：协议
来源：http://nhf.vqdsnc.cn

protocol Shape { func area() -> Double }
来源：http://hby.yj202588.top

[T31] Lua：Hello World
来源：http://cca.shangyingyoupin.top

print("Hello")
来源：http://xtu.bjfxy.top

[T32] Lua：局部变量
来源：http://pcp.ivvv.top

local a = 1
来源：http://yva.cashguo.top

[T33] Lua：表（数组）
来源：http://jya.shanyushiyangkeji.top

local t = {1, 2, 3};  t[4] = 4
来源：http://vph.pengpengdd.cyou

[T34] Lua：遍历表
来源：http://odi.bjfxy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://stz.zhiwuduotai.top

[T35] Lua：字典表
来源：http://xhr.hongshengwenyu.top

local d = { a = 1 };  d.b = 2
来源：http://gie.sjlbkw.cn

[T36] Lua：函数
来源：http://eug.cqqwz.cn

function add(a, b) return a + b end
来源：http://ftu.yfazqb.com

[T37] Lua：字符串拼接
来源：http://wcv.ehwqpu.com

"a" .. "b"
来源：http://ysx.tanke756.top

[T38] Lua：条件
来源：http://lkz.sjlbkw.cn

if x > 0 then print("正") end
来源：http://aad.epnwcf.com

[T39] Lua：模式匹配
来源：http://neo.yanxiufei.cn

string.find(s, "%d+")
来源：http://esy.zhongyouzk.top

[T40] Lua：元表
来源：http://dhl.aibaodan.cn

setmetatable({}, { __index = base })
来源：http://vmr.tianlin.xyz

[T41] Perl：Hello World
来源：http://hmv.gaohongyu789.top

print "Hello\n";
来源：http://fwi.shanyushiyangkeji.top

[T42] Perl：变量类型
来源：http://rgq.zhijiandao.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dcm.52xcode.cn

[T43] Perl：字符串插值
来源：http://ccu.ehwqpu.com

"值: $a"
来源：http://hxw.sweek.top

[T44] Perl：条件
来源：http://kbu.quarkkingdee.top

if ($a > 0) { print "正"; }
来源：http://kva.cdnleiting.top

[T45] Perl：数组遍历
来源：http://iut.yuxming.cn

for my $x (@arr) { print $x; }
来源：http://fve.sufxvd.cn

[T46] Perl：哈希操作
来源：http://hsh.jinghuilouyu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://icn.yueranfly.top

[T47] Perl：正则捕获
来源：http://ako.chenzaomai.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://krb.dianchejie.cn

[T48] Perl：正则替换
来源：http://beo.yj202588.top

$s =~ s/old/new/g;
来源：http://lih.xuetiantiany.cn

[T49] Perl：函数
来源：http://yty.wangdashe.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cae.nanxinkj.top

[T50] Perl：逐行读文件
来源：http://glq.shzxlz.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://uzk.jinqigfzy.top

while (my $line = <$fh>) { print $line; }
来源：http://pzk.wangdashe.top

[T51] Scala：Hello World
来源：http://ias.vqdsnc.cn

println("Hello")
来源：http://pcj.hesvh.cn

[T52] Scala：变量
来源：http://igo.hywenlv.cn

val a = 1;  var b = 2
来源：http://qeu.shanyushiyangkeji.top

[T53] Scala：字符串插值
来源：http://bab.pengpengdd.cyou

s"值: $b"
来源：http://vhv.hcnkem.com

[T54] Scala：集合映射
来源：http://csa.fengsongda.top

List(1, 2, 3).map(_ * 2)
来源：http://hla.sjlbkw.cn

[T55] Scala：集合过滤
来源：http://yzt.gaohongyu789.top

List(1, 2, 3).filter(_ > 1)
来源：http://ofq.sjlbkw.cn

[T56] Scala：样例类
来源：http://jrz.wangshuangyany.cn

case class User(name: String, age: Int)
来源：http://hel.yueranfly.top

[T57] Scala：模式匹配
来源：http://tti.jyoumei.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://mdj.snrcjt.cn

[T58] Scala：函数定义
来源：http://zsg.hywenlv.cn

def add(a: Int, b: Int): Int = a + b
来源：http://sig.jianghu66.top

[T59] Scala：循环
来源：http://pzf.hywenlv.cn

for (i <- 1 to 10) println(i)
来源：http://niu.fengsongda.top

[T60] Scala：折叠
来源：http://uev.shuidangran.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gth.bbcook.cn

================================================================================
来源：http://zyn.cashguo.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ijy.wangshuangyany.cn

================================================================================
来源：http://zpn.zdbjq.cn

[U01] Py：创建虚拟环境
来源：http://xwn.fktsv.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cuz.aibaodan.cn

[U02] Py：导出 / 安装依赖
来源：http://yoq.hongshengwenyu.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kvd.jiagoushi.top

[U03] Py：加载 .env 配置
来源：http://wzq.zhixingplan.top

from dotenv import load_dotenv; load_dotenv()
来源：http://tjd.wangdashe.top

[U04] Py：变量调试打印
来源：http://wql.hcnkem.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dwi.316326.xyz

[U05] Py：列表去重且保序
来源：http://lie.shanyushiyangtech.top

list(dict.fromkeys(arr))
来源：http://wwa.zycfv.cn

[U06] Py：合并两个字典
来源：http://arh.wangdashe.top

{**a, **b}
来源：http://ycz.jinyuanbaomall.cn

[U07] Py：反转字典键值
来源：http://mah.gzhubu.top

{v: k for k, v in d.items()}
来源：http://fdd.316326.xyz

[U08] Py：展平二维列表
来源：http://qmb.yuxming.cn

[y for x in nested for y in x]
来源：http://vum.feifeiyinyue.top

[U09] Py：字典取最大值的键
来源：http://uef.jyoumei.cn

max(d, key=d.get)
来源：http://ehi.wangdashe.top

[U10] Py：按值排序字典
来源：http://flk.jinqigfzy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wsi.guowangkeji.top

[U11] Py：生成器表达式
来源：http://gkm.yuanzhike.top

(x * 2 for x in arr)
来源：http://uif.jianghu66.top

[U12] Py：取出现最多的 3 个元素
来源：http://dlz.dashuyun.cn

Counter(arr).most_common(3)
来源：http://jxa.bjfxy.top

[U13] Py：固定长度队列
来源：http://bjv.nwbrower.top

deque(maxlen=10)
来源：http://bqz.yfazqb.com

[U14] Py：分组收集到列表
来源：http://pim.jinqigfzy.top

defaultdict(list)
来源：http://mon.jqgufenzy.top

[U15] Py：高精度计时
来源：http://ptk.gzhubu.top

t = time.perf_counter()
来源：http://qjk.jqgfzy.top

[U16] Py：命令行参数解析
来源：http://mvw.bjfxy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://npi.zhijiandao.cn

[U17] Py：初始化日志
来源：http://pys.ydjk.org.cn

logging.basicConfig(level=logging.INFO)
来源：http://fed.kuanghao11.cn

[U18] Py：预编译正则
来源：http://nms.kuanghao11.cn

pat = re.compile(r"\d+")
来源：http://wsm.nanxinkj.top

[U19] Py：正则替换带回调
来源：http://ypd.sxryk.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://frj.quarkkingdee.top

[U20] Py：缓存函数结果
来源：http://xpu.ybcxt.top

@functools.lru_cache(maxsize=None)
来源：http://jbh.xingfuxueyuan.xyz

[U21] Py：自定义上下文管理器
来源：http://sse.sufxvd.cn

@contextlib.contextmanager
来源：http://ljp.xziqi.cn

[U22] Py：矩阵转置
来源：http://hbb.cdnleiting.top

list(zip(*m))
来源：http://jpj.vehdjk.com

[U23] Py：分块读取大文件
来源：http://ysy.tianlin.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://yio.pengpengdd.cyou

[U24] Py：路径操作
来源：http://btc.zhengqikj.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ezp.gogol.net.cn

[U25] Py：CSV 按字典读
来源：http://fmf.yj20258888.top

csv.DictReader(f)
来源：http://evl.c1oappe.top

[U26] Py：并发下载
来源：http://rxe.tian-w.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lef.zhijiandao.cn

[U27] Py：异步 HTTP
来源：http://xco.fengsongda.top

aiohttp.ClientSession() 配合 async with
来源：http://qyg.ppjwa.cn

[U28] Py：类型别名
来源：http://tbs.fktsv.cn

UserId = int
来源：http://pvq.yj20258.top

[U29] Py：属性校验
来源：http://zkz.hnqzz.top

@property 与 @x.setter 配合
来源：http://hrl.gaohongyu789.top

[U30] Py：数据类
来源：http://rub.pengpengdd.cyou

@dataclass(slots=True)
来源：http://aqc.316326.xyz

[U31] Py：单测
来源：http://arh.jinqigfzy.top

python -m pytest -q
来源：http://lgr.yj20258888.top

[U32] Py：代码格式化
来源：http://fio.zhaomingkeji.xyz

ruff format . && ruff check --fix .
来源：http://kdr.bjfxy.top

[U33] Py：打包发布
来源：http://lnj.ivvv.top

python -m build  （依赖 pyproject.toml）
来源：http://pvq.cheryme.top

[U34] Py：判断编码
来源：http://qce.uphjek.com

chardet.detect(raw)
来源：http://wvx.vqdsnc.cn

[U35] Py：发送邮件
来源：http://enh.chenjidiqi.icu

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ong.birdmap.top

[U36] Py：定时任务
来源：http://ydx.ivvv.top

schedule.every(10).minutes.do(job)
来源：http://tpi.cqqwz.cn

[U37] Py：读写 Excel
来源：http://lfv.sweek.top

pandas.read_excel / DataFrame.to_excel
来源：http://qcz.hcnkem.com

[U38] Py：获取脚本所在目录
来源：http://chv.wangdashe.top

Path(__file__).resolve().parent
来源：http://vrc.smart0.xyz

[U39] Py：判断是否在交互环境
来源：http://axl.hysaishi.cn

sys.stdout.isatty()
来源：http://ejd.316326.xyz

[U40] Py：打印到标准错误
来源：http://whq.wangshuangyany.cn

print("err", file=sys.stderr)
来源：http://qcx.zdqjudy.top

[U41] PHP：初始化 Composer 项目
来源：http://nnb.tian-w.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://mds.zdqjudy.top

[U42] PHP：PSR-4 自动加载
来源：http://yix.yonumen.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hew.yvedp.cn

[U43] PHP：声明命名空间
来源：http://jxb.ydzc1.top

namespace App\Http;
来源：http://xfa.snrcjt.cn

[U44] PHP：开启严格类型
来源：http://xek.redwolf501.top

declare(strict_types=1);
来源：http://sec.jyoumei.cn

[U45] PHP：类型声明与返回类型
来源：http://blw.pycfn.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://cwr.yueranfly.top

[U46] PHP：可空类型
来源：http://qjd.9152youxi.cn

?string $name = null
来源：http://gcd.cashguo.top

[U47] PHP：联合类型
来源：http://lvg.meibo888.top

int|string $id
来源：http://avj.sysykeji.top

[U48] PHP：纯枚举
来源：http://qof.chenzaomai.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mhu.sufxvd.cn

[U49] PHP：只读属性
来源：http://zdx.sysykeji.top

public readonly string $name
来源：http://kpo.hnqzz.top

[U50] PHP：构造器属性提升
来源：http://xda.chenjidiqi.icu

public function __construct(private int $id) {}
来源：http://pev.daria6918.cn

[U51] PHP：数组解构
来源：http://enh.guannengcc.top

[$a, $b] = $arr;
来源：http://zfu.hywenlv.cn

[U52] PHP：箭头函数
来源：http://pjv.tarul.cn

$double = fn($x) => $x * 2;
来源：http://cch.xingfuxueyuan.xyz

[U53] PHP：空合并运算符
来源：http://kwl.sysykeji.top

$v = $a ?? $b ?? "default";
来源：http://kio.epnwcf.com

[U54] PHP：空安全调用
来源：http://scu.yj20258.top

$obj?->method()
来源：http://meg.ehwqpu.com

[U55] PHP：match 表达式
来源：http://cwm.ydzc1.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://iov.daria6918.cn

[U56] PHP：命名参数
来源：http://dqn.vqdsnc.cn

f(a: 1, b: 2)
来源：http://las.haohaochexian.top

[U57] PHP：字符串插值
来源：http://lmu.bbcook.cn

"值: {$a}"
来源：http://kug.hfpthk.cn

[U58] PHP：数组三件套
来源：http://jve.zhengqikj.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://twt.epnwcf.com

[U59] PHP：自定义排序
来源：http://syc.nanxinkj.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ehl.nwbrower.top

[U60] PHP：JSON 编解码
来源：http://hws.xuanzx.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ktn.birdmap.top

[U61] PHP：正则
来源：http://cxg.zycfv.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://egc.vehdjk.com

[U62] PHP：日期对象
来源：http://ykr.ivvv.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rbq.xinyue.icu

[U63] PHP：文件读写
来源：http://rho.ydzc1.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ipo.gzhubu.top

[U64] PHP：目录遍历
来源：http://rst.vqdsnc.cn

glob("dir/*.php");  scandir("dir");
来源：http://qsz.jinqigufen.top

[U65] PHP：会话
来源：http://kcv.9152youxi.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://kky.hnxiangtu.top

[U66] PHP：设置 Cookie
来源：http://fig.zhijiandao.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xdq.gaohongyu789.top

[U67] PHP：处理文件上传
来源：http://qoi.tarul.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rqi.jiagoushi.top

[U68] PHP：PDO 连接
来源：http://bcl.jianghu66.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://jst.fktsv.cn

[U69] PHP：PDO 预处理
来源：http://bxh.zdbjq.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://quu.ctjpmb.com

[U70] PHP：PDO 事务
来源：http://mnh.yuxming.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://dus.havefunace.top

[U71] PHP：抛出异常
来源：http://ile.hnxiangtu.top

throw new RuntimeException("失败", 500);
来源：http://egb.havefunace.top

[U72] PHP：写错误日志
来源：http://fnu.gogol.net.cn

error_log("失败: " . $e->getMessage());
来源：http://wbn.yj20258.top

[U73] PHP：读取 ini 配置
来源：http://eml.jlsjyb.cn

parse_ini_file("config.ini", true)
来源：http://yqp.zhiwuduotai.top

[U74] PHP：读取环境变量
来源：http://nis.cqqwz.cn

getenv("APP_ENV") ?: "production"
来源：http://bjg.c1oappe.top

[U75] PHP：依赖注入
来源：http://svs.bbcook.cn

composer require psr/container
来源：http://iuk.sufxvd.cn

[U76] PHP：简单路由
来源：http://fjw.yueranfly.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://cuq.guannengcc.top

[U77] PHP：模板渲染
来源：http://vmy.yfazqb.com

composer require twig/twig
来源：http://qcf.aibaodan.cn

[U78] PHP：单元测试
来源：http://gcl.chenlongwang.top

composer require --dev phpunit/phpunit
来源：http://foh.cashguo.top

[U79] PHP：静态分析
来源：http://gyx.jqgfzy.top

composer require --dev phpstan/phpstan
来源：http://fkq.ctjpmb.com

[U80] PHP：代码规范修复
来源：http://ype.yangfankeji.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://hkq.bjfxy.top

[U81] JS：初始化项目
来源：http://acx.bjfxy.top

npm init -y;  npm i express
来源：http://pky.yanxiufei.cn

[U82] JS：package.json 脚本
来源：http://nod.zhongyouzk.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://ngr.sysykeji.top


<!-- 参考信息 -->