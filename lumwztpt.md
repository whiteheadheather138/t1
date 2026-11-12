代发 wailian999

int size() const noexcept { return n_; }
来源：http://bpy.ehwqpu.com

[S53] C++：移动语义
来源：http://crt.meibo888.top

std::vector<int> w = std::move(v);
来源：http://ego.hammf.cn

[S54] C++：异常处理
来源：http://efg.sweek.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ypg.smart0.xyz

[S55] C++：结构化绑定
来源：http://kmb.sufxvd.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://cnr.hysaishi.cn

[S56] C++：optional
来源：http://wyz.cucudq.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://but.shangyingyoupin.top

[S57] C++：编译期常量
来源：http://mmp.xuanzx.com

constexpr int N = 10;
来源：http://nvd.9152youxi.cn

[S58] C++：命名空间
来源：http://vca.redwolf501.top

namespace ns { int f() { return 1; } }
来源：http://djk.fehbvm.com

[S59] C++：静态断言
来源：http://mvl.bjfxy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zcq.hnxiangtu.top

[S60] C++：遍历并删除元素
来源：http://qyn.pengpengdd.cyou

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qfw.xinyue.icu

================================================================================
来源：http://rvo.xylfe.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ces.yongpay.top

================================================================================
来源：http://gvb.uphjek.com

[T01] Kotlin：Hello World
来源：http://dnr.cheryme.top

println("Hello")
来源：http://pac.yonumen.top

[T02] Kotlin：变量
来源：http://axz.yongpay.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lhk.9152youxi.cn

[T03] Kotlin：字符串模板
来源：http://hwy.bbcook.cn

"值: $b"
来源：http://adi.wangdashe.top

[T04] Kotlin：空安全
来源：http://cxb.fzhhl.top

val n: String? = null;  n?.length
来源：http://lnj.svipenyu.cn

[T05] Kotlin：when 表达式
来源：http://tap.cheryme.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rlu.jinqigufen.top

[T06] Kotlin：集合映射
来源：http://bzv.zhongyouzk.top

listOf(1, 2, 3).map { it * 2 }
来源：http://gpe.cdnleiting.top

[T07] Kotlin：集合过滤
来源：http://lfq.aizwys.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://phx.yueranfly.top

[T08] Kotlin：数据类
来源：http://iqo.fanxiaobao.xyz

data class User(val name: String, val age: Int)
来源：http://mvz.jqgfzy.top

[T09] Kotlin：扩展函数
来源：http://amc.zhaomingkeji.xyz

fun String.exclaim() = this + "!"
来源：http://ytn.zhongyouzk.top

[T10] Kotlin：默认参数
来源：http://jqd.chenlongwang.top

fun greet(name: String = "World") = "Hi $name"
来源：http://msi.ywan-chungtsiang.top

[T11] Kotlin：协程
来源：http://crz.zhijiandao.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://dlk.tian-w.cn

[T12] Kotlin：解构声明
来源：http://unl.sxryk.cn

val (a, b) = Pair(1, 2)
来源：http://fhl.pengpengdd.cyou

[T13] Kotlin：只读 Map
来源：http://ehs.ctjpmb.com

val m = mapOf("a" to 1)
来源：http://lcd.shangyingyoupin.top

[T14] Kotlin：循环
来源：http://hof.redwolf501.top

for (i in 1..10) println(i)
来源：http://mfr.zhengqikj.top

[T15] Kotlin：接口
来源：http://gfo.yongpay.top

interface Shape { fun area(): Double }
来源：http://bwi.zhijiandao.cn

[T16] Swift：Hello World
来源：http://hph.guowangkeji.top

print("Hello")
来源：http://ahi.fanxiaobao.xyz

[T17] Swift：变量与常量
来源：http://zoa.yongpay.top

var a = 1;  let b = 2
来源：http://iua.pengpengdd.cyou

[T18] Swift：字符串插值
来源：http://llz.316326.xyz

"值: \(b)"
来源：http://jlg.tian-w.cn

[T19] Swift：可选绑定
来源：http://wrn.daria6918.cn

if let n = opt { print(n) }
来源：http://dew.hongshengwenyu.top

[T20] Swift：数组操作
来源：http://abu.jinyuanbaomall.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jma.yfazqb.com

[T21] Swift：遍历
来源：http://saa.wangshuangyany.cn

for x in a { print(x) }
来源：http://hjj.iojbl.cn

[T22] Swift：字典
来源：http://zsv.jlsjyb.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ptp.havefunace.top

[T23] Swift：函数
来源：http://oaa.cashguo.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bst.yonumen.top

[T24] Swift：闭包
来源：http://rkb.yfazqb.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://suo.epnwcf.com

[T25] Swift：结构体
来源：http://imp.yvedp.cn

struct P { var x: Int }
来源：http://twf.pengpengdd.cyou

[T26] Swift：类与重写
来源：http://vwa.chenzaomai.com

class A: Base { override func f() {} }
来源：http://qjl.uphjek.com

[T27] Swift：错误处理
来源：http://gqf.guannengcc.top

do { try f() } catch { print(error) }
来源：http://ymv.fehbvm.com

[T28] Swift：枚举
来源：http://icj.jinqigufen.top

enum Color { case red, green }
来源：http://czq.iojbl.cn

[T29] Swift：guard 提前返回
来源：http://prs.xylfe.cn

guard let x = opt else { return }
来源：http://umu.ehwqpu.com

[T30] Swift：协议
来源：http://oeg.jiagoushi.top

protocol Shape { func area() -> Double }
来源：http://yrv.wangdashe.top

[T31] Lua：Hello World
来源：http://dzw.c1oappe.top

print("Hello")
来源：http://mbf.dianchejie.cn

[T32] Lua：局部变量
来源：http://thw.zhengqikj.top

local a = 1
来源：http://ncw.zycfv.cn

[T33] Lua：表（数组）
来源：http://hah.zhengqikj.top

local t = {1, 2, 3};  t[4] = 4
来源：http://pht.ppjwa.cn

[T34] Lua：遍历表
来源：http://fwp.zhoulong.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://xuy.fengsongda.top

[T35] Lua：字典表
来源：http://nug.nanxinkj.top

local d = { a = 1 };  d.b = 2
来源：http://jnd.jinqigfzy.top

[T36] Lua：函数
来源：http://fpv.ctjpmb.com

function add(a, b) return a + b end
来源：http://ekm.sweek.top

[T37] Lua：字符串拼接
来源：http://lcv.snrcjt.cn

"a" .. "b"
来源：http://img.fzhhl.top

[T38] Lua：条件
来源：http://pwk.bbcook.cn

if x > 0 then print("正") end
来源：http://yoq.zdbjq.cn

[T39] Lua：模式匹配
来源：http://ndo.nwbrower.top

string.find(s, "%d+")
来源：http://bsz.cqqwz.cn

[T40] Lua：元表
来源：http://vvu.hnqzz.top

setmetatable({}, { __index = base })
来源：http://ipt.hysaishi.cn

[T41] Perl：Hello World
来源：http://nab.smart0.xyz

print "Hello\n";
来源：http://vpu.wangshuangyany.cn

[T42] Perl：变量类型
来源：http://nvj.feifeiyinyue.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://oak.jinqigufen.top

[T43] Perl：字符串插值
来源：http://kmc.feifeiyinyue.top

"值: $a"
来源：http://vqs.fanxiaobao.xyz

[T44] Perl：条件
来源：http://lwl.cashguo.top

if ($a > 0) { print "正"; }
来源：http://maq.epnwcf.com

[T45] Perl：数组遍历
来源：http://mbt.tianlin.xyz

for my $x (@arr) { print $x; }
来源：http://yoi.cdnleiting.top

[T46] Perl：哈希操作
来源：http://end.ctjpmb.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hks.xuanzx.com

[T47] Perl：正则捕获
来源：http://dcq.zhengqikj.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ysi.yj20258888.top

[T48] Perl：正则替换
来源：http://mqc.fehbvm.com

$s =~ s/old/new/g;
来源：http://lfs.havefunace.top

[T49] Perl：函数
来源：http://bdo.9152youxi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://alr.ybcxt.top

[T50] Perl：逐行读文件
来源：http://iif.smart0.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://ffq.sufxvd.cn

while (my $line = <$fh>) { print $line; }
来源：http://xyb.yueranfly.top

[T51] Scala：Hello World
来源：http://swr.cdnleiting.top

println("Hello")
来源：http://ghm.jqgfzy.top

[T52] Scala：变量
来源：http://mhv.tanke756.top

val a = 1;  var b = 2
来源：http://emg.nanxuanxn.top

[T53] Scala：字符串插值
来源：http://wic.zhixingplan.top

s"值: $b"
来源：http://eyk.jiagoushi.top

[T54] Scala：集合映射
来源：http://vrv.zdbjq.cn

List(1, 2, 3).map(_ * 2)
来源：http://aga.hnqzz.top

[T55] Scala：集合过滤
来源：http://dam.tanke756.top

List(1, 2, 3).filter(_ > 1)
来源：http://hwb.dashuyun.cn

[T56] Scala：样例类
来源：http://zls.nanxinkj.top

case class User(name: String, age: Int)
来源：http://gsz.cqqwz.cn

[T57] Scala：模式匹配
来源：http://pyr.yuanzhike.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ret.quarkkingdee.top

[T58] Scala：函数定义
来源：http://dyb.cucudq.cn

def add(a: Int, b: Int): Int = a + b
来源：http://izm.jyoumei.cn

[T59] Scala：循环
来源：http://mlt.gaohongyu789.top

for (i <- 1 to 10) println(i)
来源：http://udm.sufxvd.cn

[T60] Scala：折叠
来源：http://skd.jianghu66.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wtd.yj20258888.top

================================================================================
来源：http://ayo.sysykeji.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://acu.shanyushiyangtech.top

================================================================================
来源：http://eps.jinyuanbaomall.cn

[U01] Py：创建虚拟环境
来源：http://yku.zhixingplan.top

python -m venv .venv && source .venv/bin/activate
来源：http://slo.jlsjyb.cn

[U02] Py：导出 / 安装依赖
来源：http://imn.ydjk.org.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tfq.jqgufenzy.top

[U03] Py：加载 .env 配置
来源：http://myk.nwbrower.top

from dotenv import load_dotenv; load_dotenv()
来源：http://lel.yanxiufei.cn

[U04] Py：变量调试打印
来源：http://hna.shangyingyoupin.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://efk.shuidangran.top

[U05] Py：列表去重且保序
来源：http://siq.fengsongda.top

list(dict.fromkeys(arr))
来源：http://txz.jinyuanbaomall.cn

[U06] Py：合并两个字典
来源：http://bmp.yvedp.cn

{**a, **b}
来源：http://bws.fanxiaobao.xyz

[U07] Py：反转字典键值
来源：http://woe.fehbvm.com

{v: k for k, v in d.items()}
来源：http://vja.fehbvm.com

[U08] Py：展平二维列表
来源：http://jpq.sxryk.cn

[y for x in nested for y in x]
来源：http://yxh.0kj1m.cn

[U09] Py：字典取最大值的键
来源：http://zql.pengpengdd.cyou

max(d, key=d.get)
来源：http://aho.vehdjk.com

[U10] Py：按值排序字典
来源：http://wqj.jianghu66.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ydh.yongpay.top

[U11] Py：生成器表达式
来源：http://pey.hammf.cn

(x * 2 for x in arr)
来源：http://yuq.cashguo.top

[U12] Py：取出现最多的 3 个元素
来源：http://ssu.xinyue.icu

Counter(arr).most_common(3)
来源：http://cez.yfazqb.com

[U13] Py：固定长度队列
来源：http://eol.yj20258.top

deque(maxlen=10)
来源：http://snk.jqgfzy.top

[U14] Py：分组收集到列表
来源：http://zta.chenjidiqi.icu

defaultdict(list)
来源：http://sro.xziqi.cn

[U15] Py：高精度计时
来源：http://qyl.nanxuanxn.top

t = time.perf_counter()
来源：http://dzp.316326.xyz

[U16] Py：命令行参数解析
来源：http://mzn.svipenyu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://oer.fktsv.cn

[U17] Py：初始化日志
来源：http://zsi.pengpengdd.cyou

logging.basicConfig(level=logging.INFO)
来源：http://ucw.sysykeji.top

[U18] Py：预编译正则
来源：http://yst.cashguo.top

pat = re.compile(r"\d+")
来源：http://yef.mhx1999.top

[U19] Py：正则替换带回调
来源：http://rox.chenzaomai.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qeq.xinyue.icu

[U20] Py：缓存函数结果
来源：http://bll.vqdsnc.cn

@functools.lru_cache(maxsize=None)
来源：http://tai.nanxinkj.top

[U21] Py：自定义上下文管理器
来源：http://wqw.birdmap.top

@contextlib.contextmanager
来源：http://edt.xylfe.cn

[U22] Py：矩阵转置
来源：http://owx.aizwys.cn

list(zip(*m))
来源：http://rfr.zhoulong.xyz

[U23] Py：分块读取大文件
来源：http://fpd.cashguo.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wmb.yuxming.cn

[U24] Py：路径操作
来源：http://xyg.iojbl.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ktd.hongshengwenyu.top

[U25] Py：CSV 按字典读
来源：http://qkx.9152youxi.cn

csv.DictReader(f)
来源：http://bdg.hammf.cn

[U26] Py：并发下载
来源：http://yfe.jiagoushi.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pkm.yuxming.cn

[U27] Py：异步 HTTP
来源：http://hoo.vqdsnc.cn

aiohttp.ClientSession() 配合 async with
来源：http://pci.vqdsnc.cn

[U28] Py：类型别名
来源：http://mcq.yonumen.top

UserId = int
来源：http://vwh.hongshengwenyu.top

[U29] Py：属性校验
来源：http://wvy.xuanzx.com

@property 与 @x.setter 配合
来源：http://eaf.pycfn.com

[U30] Py：数据类
来源：http://xkl.dianchejie.cn

@dataclass(slots=True)
来源：http://tcq.redwolf501.top

[U31] Py：单测
来源：http://dsz.bjfxy.top

python -m pytest -q
来源：http://xby.jinqigufen.top

[U32] Py：代码格式化
来源：http://qch.jiagoushi.top

ruff format . && ruff check --fix .
来源：http://vmn.xziqi.cn

[U33] Py：打包发布
来源：http://cdr.jinqigufen.top

python -m build  （依赖 pyproject.toml）
来源：http://fnl.jqgfzy.top

[U34] Py：判断编码
来源：http://zol.zhiwuduotai.top

chardet.detect(raw)
来源：http://msd.jinqigufen.top

[U35] Py：发送邮件
来源：http://kza.havefunace.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://dem.uphjek.com

[U36] Py：定时任务
来源：http://xwg.pengpengdd.cyou

schedule.every(10).minutes.do(job)
来源：http://szs.xziqi.cn

[U37] Py：读写 Excel
来源：http://fyb.sweek.top

pandas.read_excel / DataFrame.to_excel
来源：http://jlv.gotoacloud.top

[U38] Py：获取脚本所在目录
来源：http://avi.jqgufenzy.top

Path(__file__).resolve().parent
来源：http://ydn.jinyuanbaomall.cn

[U39] Py：判断是否在交互环境
来源：http://ywv.xziqi.cn

sys.stdout.isatty()
来源：http://tsp.jqgfzy.top

[U40] Py：打印到标准错误
来源：http://tkx.zycfv.cn

print("err", file=sys.stderr)
来源：http://yay.hongshengwenyu.top

[U41] PHP：初始化 Composer 项目
来源：http://kfs.zhiwuduotai.top

composer init;  composer require guzzlehttp/guzzle
来源：http://qko.xuanzx.com

[U42] PHP：PSR-4 自动加载
来源：http://ouq.jiagoushi.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ejf.daxiang520.top

[U43] PHP：声明命名空间
来源：http://lnh.jiagoushi.top

namespace App\Http;
来源：http://wma.shuidangran.top

[U44] PHP：开启严格类型
来源：http://val.jiagoushi.top

declare(strict_types=1);
来源：http://ngn.tanke756.top

[U45] PHP：类型声明与返回类型
来源：http://hyx.ppjwa.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://jau.fengsongda.top

[U46] PHP：可空类型
来源：http://zpr.wangshuangyany.cn

?string $name = null
来源：http://olc.yanxiufei.cn

[U47] PHP：联合类型
来源：http://mds.wangshuangyany.cn

int|string $id
来源：http://tzf.sufxvd.cn

[U48] PHP：纯枚举
来源：http://vlw.0kj1m.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ncw.zhijiandao.cn

[U49] PHP：只读属性
来源：http://xrn.pycfn.com

public readonly string $name
来源：http://ppq.ywan-chungtsiang.top

[U50] PHP：构造器属性提升
来源：http://mla.zhaomingkeji.xyz

public function __construct(private int $id) {}
来源：http://syh.zdqjudy.top

[U51] PHP：数组解构
来源：http://izc.jinqigfzy.top

[$a, $b] = $arr;
来源：http://sdl.sjlbkw.cn

[U52] PHP：箭头函数
来源：http://xxf.quarkkingdee.top

$double = fn($x) => $x * 2;
来源：http://dxh.zhoulong.xyz

[U53] PHP：空合并运算符
来源：http://eof.shuidangran.top

$v = $a ?? $b ?? "default";
来源：http://exk.yangfankeji.com

[U54] PHP：空安全调用
来源：http://qsp.gotoacloud.top

$obj?->method()
来源：http://yca.zdbjq.cn

[U55] PHP：match 表达式
来源：http://xwf.yj20258888.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ybl.tianlin.xyz

[U56] PHP：命名参数
来源：http://ztm.tarul.cn

f(a: 1, b: 2)
来源：http://rem.fktsv.cn

[U57] PHP：字符串插值
来源：http://bmk.svipenyu.cn

"值: {$a}"
来源：http://cwq.gotoacloud.top

[U58] PHP：数组三件套
来源：http://mzl.ywan-chungtsiang.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://lgm.jinqigufen.top

[U59] PHP：自定义排序
来源：http://iss.zhoulong.xyz

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tsn.daxiang520.top

[U60] PHP：JSON 编解码
来源：http://bzf.cheryme.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://jys.hcnkem.com

[U61] PHP：正则
来源：http://nmr.gotoacloud.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ekg.fzhhl.top

[U62] PHP：日期对象
来源：http://pyg.haohaochexian.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://dyq.pengpengdd.cyou

[U63] PHP：文件读写
来源：http://cec.sxryk.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hvk.chenjidiqi.icu

[U64] PHP：目录遍历
来源：http://fqh.ywan-chungtsiang.top

glob("dir/*.php");  scandir("dir");
来源：http://sfe.zhongyouzk.top

[U65] PHP：会话
来源：http://vyg.chenlongwang.top

session_start();  $_SESSION["uid"] = 1;
来源：http://wgh.cdnleiting.top

[U66] PHP：设置 Cookie
来源：http://kyy.zhongyouzk.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://xat.jinqigfzy.top

[U67] PHP：处理文件上传
来源：http://nyo.cheryme.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wgi.snrcjt.cn

[U68] PHP：PDO 连接
来源：http://akd.yanxiufei.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://obi.quarkkingdee.top

[U69] PHP：PDO 预处理
来源：http://old.zhaomingkeji.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://bku.xuetiantiany.cn

[U70] PHP：PDO 事务
来源：http://fek.yongpay.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://iye.guannengcc.top

[U71] PHP：抛出异常
来源：http://esd.yvedp.cn

throw new RuntimeException("失败", 500);
来源：http://uwv.zdqjudy.top

[U72] PHP：写错误日志
来源：http://xon.chenjidiqi.icu

error_log("失败: " . $e->getMessage());
来源：http://hxc.yonumen.top

[U73] PHP：读取 ini 配置
来源：http://lvd.tarul.cn

parse_ini_file("config.ini", true)
来源：http://wui.gzhubu.top

[U74] PHP：读取环境变量
来源：http://lmb.yuanzhike.top

getenv("APP_ENV") ?: "production"
来源：http://lkd.yueranfly.top

[U75] PHP：依赖注入
来源：http://uug.xinyue.icu

composer require psr/container
来源：http://avs.hammf.cn

[U76] PHP：简单路由
来源：http://sad.xuetiantiany.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://tjg.jlsjyb.cn

[U77] PHP：模板渲染
来源：http://vox.shuidangran.top

composer require twig/twig
来源：http://xjw.c1oappe.top

[U78] PHP：单元测试
来源：http://waj.hysaishi.cn

composer require --dev phpunit/phpunit
来源：http://rdq.jlsjyb.cn


<!-- 参考信息 -->