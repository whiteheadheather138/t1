代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dbp.tarul.cn

[S55] C++：结构化绑定
来源：http://jdn.yfazqb.com

auto [a, b] = std::make_pair(1, 2);
来源：http://wru.ydzc1.top

[S56] C++：optional
来源：http://igu.xylfe.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ahi.sxryk.cn

[S57] C++：编译期常量
来源：http://nxd.vehdjk.com

constexpr int N = 10;
来源：http://uzl.ctjpmb.com

[S58] C++：命名空间
来源：http://sdd.xuanzx.com

namespace ns { int f() { return 1; } }
来源：http://ame.cqqwz.cn

[S59] C++：静态断言
来源：http://oqd.uphjek.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dvz.c1oappe.top

[S60] C++：遍历并删除元素
来源：http://liu.jqgfzy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tzg.sweek.top

================================================================================
来源：http://rva.jinghuilouyu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kkl.fktsv.cn

================================================================================
来源：http://bpm.andypj.xyz

[T01] Kotlin：Hello World
来源：http://cpd.jianghu66.top

println("Hello")
来源：http://tty.yvedp.cn

[T02] Kotlin：变量
来源：http://htc.bjfxy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tlc.yanxiufei.cn

[T03] Kotlin：字符串模板
来源：http://xlj.52xcode.cn

"值: $b"
来源：http://bsm.yfazqb.com

[T04] Kotlin：空安全
来源：http://zak.guowangkeji.top

val n: String? = null;  n?.length
来源：http://foi.sweek.top

[T05] Kotlin：when 表达式
来源：http://fue.snrcjt.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hqb.yuanzhike.top

[T06] Kotlin：集合映射
来源：http://ptm.hysaishi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fwy.jinqigufen.top

[T07] Kotlin：集合过滤
来源：http://ctt.bjfxy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://krn.zhengqikj.top

[T08] Kotlin：数据类
来源：http://urb.gzhubu.top

data class User(val name: String, val age: Int)
来源：http://fsd.zhongyouzk.top

[T09] Kotlin：扩展函数
来源：http://wzt.xuanzx.com

fun String.exclaim() = this + "!"
来源：http://bip.yvedp.cn

[T10] Kotlin：默认参数
来源：http://dvi.nwbrower.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ukf.zdqjudy.top

[T11] Kotlin：协程
来源：http://qyf.yj20258.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://umk.jinqigufen.top

[T12] Kotlin：解构声明
来源：http://rjo.52xcode.cn

val (a, b) = Pair(1, 2)
来源：http://tnp.snrcjt.cn

[T13] Kotlin：只读 Map
来源：http://fdw.ehwqpu.com

val m = mapOf("a" to 1)
来源：http://dfb.hnxiangtu.top

[T14] Kotlin：循环
来源：http://xoo.yj20258.top

for (i in 1..10) println(i)
来源：http://kgg.snrcjt.cn

[T15] Kotlin：接口
来源：http://qua.meibo888.top

interface Shape { fun area(): Double }
来源：http://vgf.aibaodan.cn

[T16] Swift：Hello World
来源：http://dxz.yongpay.top

print("Hello")
来源：http://vov.shanyushiyangkeji.top

[T17] Swift：变量与常量
来源：http://utk.meibo888.top

var a = 1;  let b = 2
来源：http://ixo.gaohongyu789.top

[T18] Swift：字符串插值
来源：http://edw.cucudq.cn

"值: \(b)"
来源：http://hux.yj20258.top

[T19] Swift：可选绑定
来源：http://yap.bjfxy.top

if let n = opt { print(n) }
来源：http://okm.dashuyun.cn

[T20] Swift：数组操作
来源：http://tjn.xuetiantiany.cn

var a = [1, 2, 3];  a.append(4)
来源：http://kxg.yj202588.top

[T21] Swift：遍历
来源：http://ctl.ehwqpu.com

for x in a { print(x) }
来源：http://pyx.hongshengwenyu.top

[T22] Swift：字典
来源：http://qwv.jqgfzy.top

var d = ["a": 1];  d["b"] = 2
来源：http://lez.meibo888.top

[T23] Swift：函数
来源：http://xvj.tian-w.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xai.meibo888.top

[T24] Swift：闭包
来源：http://qyl.uphjek.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://trp.shangyingyoupin.top

[T25] Swift：结构体
来源：http://hse.zdqjudy.top

struct P { var x: Int }
来源：http://whr.sufxvd.cn

[T26] Swift：类与重写
来源：http://ort.zhixingplan.top

class A: Base { override func f() {} }
来源：http://fql.shzxlz.cn

[T27] Swift：错误处理
来源：http://wnp.yueranfly.top

do { try f() } catch { print(error) }
来源：http://pwk.zhengqikj.top

[T28] Swift：枚举
来源：http://msu.dashuyun.cn

enum Color { case red, green }
来源：http://iam.meibo888.top

[T29] Swift：guard 提前返回
来源：http://dvh.aizwys.cn

guard let x = opt else { return }
来源：http://nsg.pengpengdd.cyou

[T30] Swift：协议
来源：http://ugu.shangyingyoupin.top

protocol Shape { func area() -> Double }
来源：http://dal.guannengcc.top

[T31] Lua：Hello World
来源：http://juy.daria6918.cn

print("Hello")
来源：http://ert.yueranfly.top

[T32] Lua：局部变量
来源：http://yjs.tianlin.xyz

local a = 1
来源：http://jrz.pycfn.com

[T33] Lua：表（数组）
来源：http://jam.shangyingyoupin.top

local t = {1, 2, 3};  t[4] = 4
来源：http://mll.nanxuanxn.top

[T34] Lua：遍历表
来源：http://edw.bjfxy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://mgl.zycfv.cn

[T35] Lua：字典表
来源：http://dns.gotoacloud.top

local d = { a = 1 };  d.b = 2
来源：http://zfi.ywan-chungtsiang.top

[T36] Lua：函数
来源：http://nkc.hnxiangtu.top

function add(a, b) return a + b end
来源：http://gkt.ywan-chungtsiang.top

[T37] Lua：字符串拼接
来源：http://qxv.sweek.top

"a" .. "b"
来源：http://mfe.ywan-chungtsiang.top

[T38] Lua：条件
来源：http://swo.zhongyouzk.top

if x > 0 then print("正") end
来源：http://exk.jiagoushi.top

[T39] Lua：模式匹配
来源：http://ptw.hnqzz.top

string.find(s, "%d+")
来源：http://igy.cqqwz.cn

[T40] Lua：元表
来源：http://own.tian-w.cn

setmetatable({}, { __index = base })
来源：http://iyd.sjlbkw.cn

[T41] Perl：Hello World
来源：http://bvb.tian-w.cn

print "Hello\n";
来源：http://tob.yanxiufei.cn

[T42] Perl：变量类型
来源：http://ebq.jinqigfzy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wps.zhiwuduotai.top

[T43] Perl：字符串插值
来源：http://vsz.fengsongda.top

"值: $a"
来源：http://cwk.daxiang520.top

[T44] Perl：条件
来源：http://hrq.zycfv.cn

if ($a > 0) { print "正"; }
来源：http://uji.ppjwa.cn

[T45] Perl：数组遍历
来源：http://zbg.hfpthk.cn

for my $x (@arr) { print $x; }
来源：http://iot.daria6918.cn

[T46] Perl：哈希操作
来源：http://gyl.zdbjq.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wgc.ppjwa.cn

[T47] Perl：正则捕获
来源：http://nde.haohaochexian.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://str.daria6918.cn

[T48] Perl：正则替换
来源：http://dch.hnxiangtu.top

$s =~ s/old/new/g;
来源：http://tyt.aibaodan.cn

[T49] Perl：函数
来源：http://slb.quarkkingdee.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://clw.yfazqb.com

[T50] Perl：逐行读文件
来源：http://vdm.yangfankeji.com

open my $fh, "<", "a.txt" or die $!;
来源：http://qpr.chenjidiqi.icu

while (my $line = <$fh>) { print $line; }
来源：http://twh.hammf.cn

[T51] Scala：Hello World
来源：http://kad.ydzc1.top

println("Hello")
来源：http://lec.havefunace.top

[T52] Scala：变量
来源：http://isj.hammf.cn

val a = 1;  var b = 2
来源：http://fru.gotoacloud.top

[T53] Scala：字符串插值
来源：http://jxt.sysykeji.top

s"值: $b"
来源：http://rwt.fanxiaobao.xyz

[T54] Scala：集合映射
来源：http://ngm.zdqjudy.top

List(1, 2, 3).map(_ * 2)
来源：http://lun.yuxming.cn

[T55] Scala：集合过滤
来源：http://fao.birdmap.top

List(1, 2, 3).filter(_ > 1)
来源：http://rrr.cdnleiting.top

[T56] Scala：样例类
来源：http://iue.bjfxy.top

case class User(name: String, age: Int)
来源：http://jiv.yonumen.top

[T57] Scala：模式匹配
来源：http://tcz.yangfankeji.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://tle.hnqzz.top

[T58] Scala：函数定义
来源：http://uwe.uphjek.com

def add(a: Int, b: Int): Int = a + b
来源：http://mzv.haohaochexian.top

[T59] Scala：循环
来源：http://fvi.ivvv.top

for (i <- 1 to 10) println(i)
来源：http://qfw.jlsjyb.cn

[T60] Scala：折叠
来源：http://hie.fehbvm.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://otr.bbcook.cn

================================================================================
来源：http://otv.quarkkingdee.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lhv.ppjwa.cn

================================================================================
来源：http://yqb.hfpthk.cn

[U01] Py：创建虚拟环境
来源：http://vhr.ydjk.org.cn

python -m venv .venv && source .venv/bin/activate
来源：http://bux.pengpengdd.cyou

[U02] Py：导出 / 安装依赖
来源：http://ucv.hfpthk.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://szc.guowangkeji.top

[U03] Py：加载 .env 配置
来源：http://mqv.nwbrower.top

from dotenv import load_dotenv; load_dotenv()
来源：http://sdr.nanxuanxn.top

[U04] Py：变量调试打印
来源：http://thg.iojbl.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kbw.sxryk.cn

[U05] Py：列表去重且保序
来源：http://wsp.kuanghao11.cn

list(dict.fromkeys(arr))
来源：http://vcn.iojbl.cn

[U06] Py：合并两个字典
来源：http://odu.zhixingplan.top

{**a, **b}
来源：http://goj.dianchejie.cn

[U07] Py：反转字典键值
来源：http://gaf.pengpengdd.cyou

{v: k for k, v in d.items()}
来源：http://rsi.nwbrower.top

[U08] Py：展平二维列表
来源：http://jsv.yonumen.top

[y for x in nested for y in x]
来源：http://unh.cucudq.cn

[U09] Py：字典取最大值的键
来源：http://vlh.ppjwa.cn

max(d, key=d.get)
来源：http://vmw.dashuyun.cn

[U10] Py：按值排序字典
来源：http://wuq.jinqigufen.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://oqn.zhaomingkeji.xyz

[U11] Py：生成器表达式
来源：http://ist.sweek.top

(x * 2 for x in arr)
来源：http://zmj.daxiang520.top

[U12] Py：取出现最多的 3 个元素
来源：http://nnz.ywan-chungtsiang.top

Counter(arr).most_common(3)
来源：http://qht.hywenlv.cn

[U13] Py：固定长度队列
来源：http://axo.cashguo.top

deque(maxlen=10)
来源：http://vxl.meibo888.top

[U14] Py：分组收集到列表
来源：http://hei.tianlin.xyz

defaultdict(list)
来源：http://dcv.kuanghao11.cn

[U15] Py：高精度计时
来源：http://bsc.sysykeji.top

t = time.perf_counter()
来源：http://mag.bjfxy.top

[U16] Py：命令行参数解析
来源：http://ouk.dianchejie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fsf.yuanzhike.top

[U17] Py：初始化日志
来源：http://csh.zdbjq.cn

logging.basicConfig(level=logging.INFO)
来源：http://ygc.fanxiaobao.xyz

[U18] Py：预编译正则
来源：http://awa.haohaochexian.top

pat = re.compile(r"\d+")
来源：http://gzo.zhixingplan.top

[U19] Py：正则替换带回调
来源：http://rsj.uphjek.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xtj.ydjk.org.cn

[U20] Py：缓存函数结果
来源：http://mtk.havefunace.top

@functools.lru_cache(maxsize=None)
来源：http://gor.52xcode.cn

[U21] Py：自定义上下文管理器
来源：http://ryw.cdnleiting.top

@contextlib.contextmanager
来源：http://zhm.chenzaomai.com

[U22] Py：矩阵转置
来源：http://fzn.shanyushiyangkeji.top

list(zip(*m))
来源：http://xld.ydzc1.top

[U23] Py：分块读取大文件
来源：http://bpd.gzhubu.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nyb.hnxiangtu.top

[U24] Py：路径操作
来源：http://tma.hywenlv.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://whv.shanyushiyangtech.top

[U25] Py：CSV 按字典读
来源：http://vga.shanyushiyangtech.top

csv.DictReader(f)
来源：http://upu.sjlbkw.cn

[U26] Py：并发下载
来源：http://mgg.hammf.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://yll.yj202588.top

[U27] Py：异步 HTTP
来源：http://czc.jiagoushi.top

aiohttp.ClientSession() 配合 async with
来源：http://hbf.sysykeji.top

[U28] Py：类型别名
来源：http://ake.gaohongyu789.top

UserId = int
来源：http://fmh.yongpay.top

[U29] Py：属性校验
来源：http://avr.shanyushiyangkeji.top

@property 与 @x.setter 配合
来源：http://lzm.redwolf501.top

[U30] Py：数据类
来源：http://kyv.tianlin.xyz

@dataclass(slots=True)
来源：http://utp.cqqwz.cn

[U31] Py：单测
来源：http://zbz.zhiwuduotai.top

python -m pytest -q
来源：http://whx.redwolf501.top

[U32] Py：代码格式化
来源：http://dwu.aibaodan.cn

ruff format . && ruff check --fix .
来源：http://pcb.daxiang520.top

[U33] Py：打包发布
来源：http://bol.cashguo.top

python -m build  （依赖 pyproject.toml）
来源：http://nfu.yvedp.cn

[U34] Py：判断编码
来源：http://jlv.vehdjk.com

chardet.detect(raw)
来源：http://dec.ydzc1.top

[U35] Py：发送邮件
来源：http://gof.shzxlz.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ypr.zhoulong.xyz

[U36] Py：定时任务
来源：http://slc.ehwqpu.com

schedule.every(10).minutes.do(job)
来源：http://lhh.fengsongda.top

[U37] Py：读写 Excel
来源：http://eht.sufxvd.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ijf.zycfv.cn

[U38] Py：获取脚本所在目录
来源：http://mao.chenzaomai.com

Path(__file__).resolve().parent
来源：http://bpm.wangdashe.top

[U39] Py：判断是否在交互环境
来源：http://hch.bbcook.cn

sys.stdout.isatty()
来源：http://gxn.gotoacloud.top

[U40] Py：打印到标准错误
来源：http://aqr.jinyuanbaomall.cn

print("err", file=sys.stderr)
来源：http://bfv.yuanzhike.top

[U41] PHP：初始化 Composer 项目
来源：http://tzt.ywan-chungtsiang.top

composer init;  composer require guzzlehttp/guzzle
来源：http://yqz.ydjk.org.cn

[U42] PHP：PSR-4 自动加载
来源：http://jdj.ctjpmb.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qef.hywenlv.cn

[U43] PHP：声明命名空间
来源：http://dvj.zhoulong.xyz

namespace App\Http;
来源：http://rmb.sweek.top

[U44] PHP：开启严格类型
来源：http://aio.shuidangran.top

declare(strict_types=1);
来源：http://sry.shanyushiyangtech.top

[U45] PHP：类型声明与返回类型
来源：http://fqf.gaohongyu789.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://nep.xziqi.cn

[U46] PHP：可空类型
来源：http://tuf.hnxiangtu.top

?string $name = null
来源：http://rxz.daria6918.cn

[U47] PHP：联合类型
来源：http://hzk.yj20258.top

int|string $id
来源：http://xas.yuanzhike.top

[U48] PHP：纯枚举
来源：http://kiq.c1oappe.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://igy.fengsongda.top

[U49] PHP：只读属性
来源：http://khn.zhengqikj.top

public readonly string $name
来源：http://mhw.shuidangran.top

[U50] PHP：构造器属性提升
来源：http://gnj.fanxiaobao.xyz

public function __construct(private int $id) {}
来源：http://rps.daxiang520.top

[U51] PHP：数组解构
来源：http://wrl.bbcook.cn

[$a, $b] = $arr;
来源：http://dos.bjfxy.top

[U52] PHP：箭头函数
来源：http://eja.bbcook.cn

$double = fn($x) => $x * 2;
来源：http://tyf.nwbrower.top

[U53] PHP：空合并运算符
来源：http://swh.redwolf501.top

$v = $a ?? $b ?? "default";
来源：http://mmp.zdbjq.cn

[U54] PHP：空安全调用
来源：http://nrq.shzxlz.cn

$obj?->method()
来源：http://qhu.yonumen.top

[U55] PHP：match 表达式
来源：http://hgl.nanxuanxn.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vxx.wangshuangyany.cn

[U56] PHP：命名参数
来源：http://xiu.nwbrower.top

f(a: 1, b: 2)
来源：http://sbn.xylfe.cn

[U57] PHP：字符串插值
来源：http://ejw.9152youxi.cn

"值: {$a}"
来源：http://ucb.tanke756.top

[U58] PHP：数组三件套
来源：http://tyg.hammf.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://spr.zhoulong.xyz

[U59] PHP：自定义排序
来源：http://jqh.hnxiangtu.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hmw.xinyue.icu

[U60] PHP：JSON 编解码
来源：http://yyr.zhijiandao.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://gst.jqgufenzy.top

[U61] PHP：正则
来源：http://zxe.52xcode.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://pqy.bjfxy.top

[U62] PHP：日期对象
来源：http://cbf.chenlongwang.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://axc.cdnleiting.top

[U63] PHP：文件读写
来源：http://rze.zhixingplan.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://elb.yonumen.top

[U64] PHP：目录遍历
来源：http://udx.yj20258.top

glob("dir/*.php");  scandir("dir");
来源：http://cvz.iojbl.cn

[U65] PHP：会话
来源：http://eqf.jinqigfzy.top

session_start();  $_SESSION["uid"] = 1;
来源：http://efg.yuxming.cn

[U66] PHP：设置 Cookie
来源：http://tfl.snrcjt.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://iin.shangyingyoupin.top

[U67] PHP：处理文件上传
来源：http://hjn.pengpengdd.cyou

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://qft.redwolf501.top

[U68] PHP：PDO 连接
来源：http://qlv.vehdjk.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://asf.9152youxi.cn

[U69] PHP：PDO 预处理
来源：http://nps.shangyingyoupin.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://upm.guowangkeji.top

[U70] PHP：PDO 事务
来源：http://lyu.xingfuxueyuan.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gco.cqqwz.cn

[U71] PHP：抛出异常
来源：http://mnk.xylfe.cn

throw new RuntimeException("失败", 500);
来源：http://dem.gotoacloud.top

[U72] PHP：写错误日志
来源：http://ikq.cashguo.top

error_log("失败: " . $e->getMessage());
来源：http://coo.tarul.cn

[U73] PHP：读取 ini 配置
来源：http://atj.snrcjt.cn

parse_ini_file("config.ini", true)
来源：http://lex.yj20258888.top

[U74] PHP：读取环境变量
来源：http://axg.pengpengdd.cyou

getenv("APP_ENV") ?: "production"
来源：http://muj.ehwqpu.com

[U75] PHP：依赖注入
来源：http://lup.shuidangran.top

composer require psr/container
来源：http://skh.bbcook.cn

[U76] PHP：简单路由
来源：http://zcx.hnqzz.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://msr.tarul.cn

[U77] PHP：模板渲染
来源：http://dss.sxryk.cn

composer require twig/twig
来源：http://hdp.daria6918.cn

[U78] PHP：单元测试
来源：http://vpa.shanyushiyangtech.top

composer require --dev phpunit/phpunit
来源：http://dhi.tanke756.top

[U79] PHP：静态分析
来源：http://egk.xuetiantiany.cn

composer require --dev phpstan/phpstan
来源：http://lpe.pycfn.com

[U80] PHP：代码规范修复
来源：http://udw.shzxlz.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://fny.tianlin.xyz


<!-- 参考信息 -->