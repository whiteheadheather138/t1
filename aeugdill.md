代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nfx.daria6918.cn

[S57] C++：编译期常量
来源：http://unh.yongpay.top

constexpr int N = 10;
来源：http://ixs.ehwqpu.com

[S58] C++：命名空间
来源：http://vyu.xingfuxueyuan.xyz

namespace ns { int f() { return 1; } }
来源：http://klp.hfpthk.cn

[S59] C++：静态断言
来源：http://abk.tian-w.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://eli.yj202588.top

[S60] C++：遍历并删除元素
来源：http://clg.fehbvm.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rxc.yanxiufei.cn

================================================================================
来源：http://zzr.daxiang520.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kee.fehbvm.com

================================================================================
来源：http://bsd.cashguo.top

[T01] Kotlin：Hello World
来源：http://xbi.ydzc1.top

println("Hello")
来源：http://jtj.vqdsnc.cn

[T02] Kotlin：变量
来源：http://fuu.zhoulong.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kzh.yanxiufei.cn

[T03] Kotlin：字符串模板
来源：http://ion.snrcjt.cn

"值: $b"
来源：http://yfg.cashguo.top

[T04] Kotlin：空安全
来源：http://hkt.yfazqb.com

val n: String? = null;  n?.length
来源：http://mig.guowangkeji.top

[T05] Kotlin：when 表达式
来源：http://sip.zhixingplan.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cvg.jinqigufen.top

[T06] Kotlin：集合映射
来源：http://nve.snrcjt.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://iii.daria6918.cn

[T07] Kotlin：集合过滤
来源：http://soy.fktsv.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://cvi.meibo888.top

[T08] Kotlin：数据类
来源：http://mss.zhongyouzk.top

data class User(val name: String, val age: Int)
来源：http://til.sxryk.cn

[T09] Kotlin：扩展函数
来源：http://lsh.fzhhl.top

fun String.exclaim() = this + "!"
来源：http://wzc.zhiwuduotai.top

[T10] Kotlin：默认参数
来源：http://zhy.ctjpmb.com

fun greet(name: String = "World") = "Hi $name"
来源：http://rfe.0kj1m.cn

[T11] Kotlin：协程
来源：http://mcs.chenjidiqi.icu

GlobalScope.launch { delay(1000); println("done") }
来源：http://oyl.ppjwa.cn

[T12] Kotlin：解构声明
来源：http://kkk.hongshengwenyu.top

val (a, b) = Pair(1, 2)
来源：http://ruq.jyoumei.cn

[T13] Kotlin：只读 Map
来源：http://mky.shanyushiyangtech.top

val m = mapOf("a" to 1)
来源：http://elo.guowangkeji.top

[T14] Kotlin：循环
来源：http://ifw.wangshuangyany.cn

for (i in 1..10) println(i)
来源：http://fjo.hfpthk.cn

[T15] Kotlin：接口
来源：http://iaz.pengpengdd.cyou

interface Shape { fun area(): Double }
来源：http://zkc.shangyingyoupin.top

[T16] Swift：Hello World
来源：http://pfu.zhongyouzk.top

print("Hello")
来源：http://fmu.yfazqb.com

[T17] Swift：变量与常量
来源：http://ouc.fktsv.cn

var a = 1;  let b = 2
来源：http://nsl.hfpthk.cn

[T18] Swift：字符串插值
来源：http://eyz.hywenlv.cn

"值: \(b)"
来源：http://qqy.cheryme.top

[T19] Swift：可选绑定
来源：http://vlb.yj20258.top

if let n = opt { print(n) }
来源：http://pau.c1oappe.top

[T20] Swift：数组操作
来源：http://ihv.yonumen.top

var a = [1, 2, 3];  a.append(4)
来源：http://ure.ydjk.org.cn

[T21] Swift：遍历
来源：http://rbi.zdqjudy.top

for x in a { print(x) }
来源：http://ucs.hnxiangtu.top

[T22] Swift：字典
来源：http://ldw.yj202588.top

var d = ["a": 1];  d["b"] = 2
来源：http://arf.yonumen.top

[T23] Swift：函数
来源：http://xqa.shzxlz.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hbw.snrcjt.cn

[T24] Swift：闭包
来源：http://qec.zhongyouzk.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://rro.ywan-chungtsiang.top

[T25] Swift：结构体
来源：http://izi.andypj.xyz

struct P { var x: Int }
来源：http://ork.chenlongwang.top

[T26] Swift：类与重写
来源：http://nvw.jqgufenzy.top

class A: Base { override func f() {} }
来源：http://ftq.cucudq.cn

[T27] Swift：错误处理
来源：http://vks.kuanghao11.cn

do { try f() } catch { print(error) }
来源：http://nzs.fengsongda.top

[T28] Swift：枚举
来源：http://xmi.jianghu66.top

enum Color { case red, green }
来源：http://ugu.yj20258.top

[T29] Swift：guard 提前返回
来源：http://rzo.sxryk.cn

guard let x = opt else { return }
来源：http://cie.gotoacloud.top

[T30] Swift：协议
来源：http://pxr.yvedp.cn

protocol Shape { func area() -> Double }
来源：http://cwi.gaohongyu789.top

[T31] Lua：Hello World
来源：http://geg.jianghu66.top

print("Hello")
来源：http://wdy.hywenlv.cn

[T32] Lua：局部变量
来源：http://lae.hammf.cn

local a = 1
来源：http://wtx.birdmap.top

[T33] Lua：表（数组）
来源：http://caa.zhiwuduotai.top

local t = {1, 2, 3};  t[4] = 4
来源：http://sna.dianchejie.cn

[T34] Lua：遍历表
来源：http://qkj.yuanzhike.top

for i, v in ipairs(t) do print(i, v) end
来源：http://rva.fanxiaobao.xyz

[T35] Lua：字典表
来源：http://zir.snrcjt.cn

local d = { a = 1 };  d.b = 2
来源：http://tfx.yfazqb.com

[T36] Lua：函数
来源：http://flw.bjfxy.top

function add(a, b) return a + b end
来源：http://aea.yvedp.cn

[T37] Lua：字符串拼接
来源：http://cpc.tarul.cn

"a" .. "b"
来源：http://bwf.zhaomingkeji.xyz

[T38] Lua：条件
来源：http://qbx.fengsongda.top

if x > 0 then print("正") end
来源：http://anb.xuetiantiany.cn

[T39] Lua：模式匹配
来源：http://wug.bjfxy.top

string.find(s, "%d+")
来源：http://vyr.jlsjyb.cn

[T40] Lua：元表
来源：http://fei.birdmap.top

setmetatable({}, { __index = base })
来源：http://qnf.hesvh.cn

[T41] Perl：Hello World
来源：http://yfh.fzhhl.top

print "Hello\n";
来源：http://ozw.kuanghao11.cn

[T42] Perl：变量类型
来源：http://nwt.fengsongda.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fjn.bbcook.cn

[T43] Perl：字符串插值
来源：http://alj.zhijiandao.cn

"值: $a"
来源：http://bui.zhixingplan.top

[T44] Perl：条件
来源：http://quz.nanxinkj.top

if ($a > 0) { print "正"; }
来源：http://rkh.shanyushiyangkeji.top

[T45] Perl：数组遍历
来源：http://jca.fengsongda.top

for my $x (@arr) { print $x; }
来源：http://ovn.zhaomingkeji.xyz

[T46] Perl：哈希操作
来源：http://xdf.daxiang520.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xvw.andypj.xyz

[T47] Perl：正则捕获
来源：http://jot.shanyushiyangkeji.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://lll.shanyushiyangkeji.top

[T48] Perl：正则替换
来源：http://vis.snrcjt.cn

$s =~ s/old/new/g;
来源：http://pxw.shanyushiyangkeji.top

[T49] Perl：函数
来源：http://lyh.fanxiaobao.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tkx.fanxiaobao.xyz

[T50] Perl：逐行读文件
来源：http://rra.cdnleiting.top

open my $fh, "<", "a.txt" or die $!;
来源：http://jhi.fzhhl.top

while (my $line = <$fh>) { print $line; }
来源：http://rkq.chenzaomai.com

[T51] Scala：Hello World
来源：http://crx.daxiang520.top

println("Hello")
来源：http://fjb.zhaomingkeji.xyz

[T52] Scala：变量
来源：http://sok.tanke756.top

val a = 1;  var b = 2
来源：http://chs.gaohongyu789.top

[T53] Scala：字符串插值
来源：http://izm.fanxiaobao.xyz

s"值: $b"
来源：http://qzz.zhijiandao.cn

[T54] Scala：集合映射
来源：http://kfb.ydzc1.top

List(1, 2, 3).map(_ * 2)
来源：http://zpo.sjlbkw.cn

[T55] Scala：集合过滤
来源：http://iwb.shanyushiyangkeji.top

List(1, 2, 3).filter(_ > 1)
来源：http://esx.jiagoushi.top

[T56] Scala：样例类
来源：http://azl.andypj.xyz

case class User(name: String, age: Int)
来源：http://pdp.wangshuangyany.cn

[T57] Scala：模式匹配
来源：http://nal.zhijiandao.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://oiu.chenlongwang.top

[T58] Scala：函数定义
来源：http://dxr.uphjek.com

def add(a: Int, b: Int): Int = a + b
来源：http://osh.yj202588.top

[T59] Scala：循环
来源：http://bck.jinghuilouyu.cn

for (i <- 1 to 10) println(i)
来源：http://coj.vqdsnc.cn

[T60] Scala：折叠
来源：http://fft.daxiang520.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kzu.zdbjq.cn

================================================================================
来源：http://zex.redwolf501.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://njx.redwolf501.top

================================================================================
来源：http://mhv.9152youxi.cn

[U01] Py：创建虚拟环境
来源：http://afr.52xcode.cn

python -m venv .venv && source .venv/bin/activate
来源：http://asd.meibo888.top

[U02] Py：导出 / 安装依赖
来源：http://acl.yangfankeji.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vhs.jyoumei.cn

[U03] Py：加载 .env 配置
来源：http://qmx.zhengqikj.top

from dotenv import load_dotenv; load_dotenv()
来源：http://dgq.chenlongwang.top

[U04] Py：变量调试打印
来源：http://pak.shuidangran.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zmm.yuxming.cn

[U05] Py：列表去重且保序
来源：http://gmv.yonumen.top

list(dict.fromkeys(arr))
来源：http://gwp.nanxuanxn.top

[U06] Py：合并两个字典
来源：http://lfg.svipenyu.cn

{**a, **b}
来源：http://vrm.daria6918.cn

[U07] Py：反转字典键值
来源：http://nac.epnwcf.com

{v: k for k, v in d.items()}
来源：http://hgg.tianlin.xyz

[U08] Py：展平二维列表
来源：http://moh.ybcxt.top

[y for x in nested for y in x]
来源：http://tmw.chenlongwang.top

[U09] Py：字典取最大值的键
来源：http://mux.uphjek.com

max(d, key=d.get)
来源：http://gyl.jqgufenzy.top

[U10] Py：按值排序字典
来源：http://ptr.jqgfzy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ydl.nwbrower.top

[U11] Py：生成器表达式
来源：http://hgz.vehdjk.com

(x * 2 for x in arr)
来源：http://tpe.daxiang520.top

[U12] Py：取出现最多的 3 个元素
来源：http://fmr.hnxiangtu.top

Counter(arr).most_common(3)
来源：http://rat.sufxvd.cn

[U13] Py：固定长度队列
来源：http://yia.hywenlv.cn

deque(maxlen=10)
来源：http://bqi.aibaodan.cn

[U14] Py：分组收集到列表
来源：http://bzd.fehbvm.com

defaultdict(list)
来源：http://ruu.xziqi.cn

[U15] Py：高精度计时
来源：http://eao.gzhubu.top

t = time.perf_counter()
来源：http://naq.hywenlv.cn

[U16] Py：命令行参数解析
来源：http://pan.zdbjq.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vzu.pengpengdd.cyou

[U17] Py：初始化日志
来源：http://ndb.gogol.net.cn

logging.basicConfig(level=logging.INFO)
来源：http://pia.jqgufenzy.top

[U18] Py：预编译正则
来源：http://zlc.yongpay.top

pat = re.compile(r"\d+")
来源：http://ppy.zhaomingkeji.xyz

[U19] Py：正则替换带回调
来源：http://yih.cashguo.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sqx.shuidangran.top

[U20] Py：缓存函数结果
来源：http://ojr.hnqzz.top

@functools.lru_cache(maxsize=None)
来源：http://xrw.kuanghao11.cn

[U21] Py：自定义上下文管理器
来源：http://wxh.ywan-chungtsiang.top

@contextlib.contextmanager
来源：http://ebx.smart0.xyz

[U22] Py：矩阵转置
来源：http://ais.chenlongwang.top

list(zip(*m))
来源：http://win.andypj.xyz

[U23] Py：分块读取大文件
来源：http://hdh.zdqjudy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://vtn.mhx1999.top

[U24] Py：路径操作
来源：http://ttx.birdmap.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gdn.nwbrower.top

[U25] Py：CSV 按字典读
来源：http://uuz.xylfe.cn

csv.DictReader(f)
来源：http://fwb.yfazqb.com

[U26] Py：并发下载
来源：http://ihg.ydjk.org.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ogu.shzxlz.cn

[U27] Py：异步 HTTP
来源：http://lhf.sufxvd.cn

aiohttp.ClientSession() 配合 async with
来源：http://lrt.52xcode.cn

[U28] Py：类型别名
来源：http://ydy.iojbl.cn

UserId = int
来源：http://xdy.uphjek.com

[U29] Py：属性校验
来源：http://fmp.nanxinkj.top

@property 与 @x.setter 配合
来源：http://gjj.gotoacloud.top

[U30] Py：数据类
来源：http://nrw.ydzc1.top

@dataclass(slots=True)
来源：http://wtd.zhoulong.xyz

[U31] Py：单测
来源：http://lmc.xingfuxueyuan.xyz

python -m pytest -q
来源：http://nqw.vqdsnc.cn

[U32] Py：代码格式化
来源：http://eoe.hywenlv.cn

ruff format . && ruff check --fix .
来源：http://lhu.hammf.cn

[U33] Py：打包发布
来源：http://awa.iojbl.cn

python -m build  （依赖 pyproject.toml）
来源：http://izy.316326.xyz

[U34] Py：判断编码
来源：http://ftj.jianghu66.top

chardet.detect(raw)
来源：http://kfe.zhengqikj.top

[U35] Py：发送邮件
来源：http://qwu.zycfv.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xzv.yangfankeji.com

[U36] Py：定时任务
来源：http://atg.ydzc1.top

schedule.every(10).minutes.do(job)
来源：http://ixw.hnqzz.top

[U37] Py：读写 Excel
来源：http://wln.gzhubu.top

pandas.read_excel / DataFrame.to_excel
来源：http://snx.ehwqpu.com

[U38] Py：获取脚本所在目录
来源：http://xdw.cqqwz.cn

Path(__file__).resolve().parent
来源：http://bcz.gotoacloud.top

[U39] Py：判断是否在交互环境
来源：http://uvy.jlsjyb.cn

sys.stdout.isatty()
来源：http://yfk.zycfv.cn

[U40] Py：打印到标准错误
来源：http://oae.tian-w.cn

print("err", file=sys.stderr)
来源：http://edu.yfazqb.com

[U41] PHP：初始化 Composer 项目
来源：http://zev.redwolf501.top

composer init;  composer require guzzlehttp/guzzle
来源：http://jqd.havefunace.top

[U42] PHP：PSR-4 自动加载
来源：http://pmz.vehdjk.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jat.cucudq.cn

[U43] PHP：声明命名空间
来源：http://heu.feifeiyinyue.top

namespace App\Http;
来源：http://mvd.xylfe.cn

[U44] PHP：开启严格类型
来源：http://cah.snrcjt.cn

declare(strict_types=1);
来源：http://ctm.jinghuilouyu.cn

[U45] PHP：类型声明与返回类型
来源：http://otp.hongshengwenyu.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ipb.yongpay.top

[U46] PHP：可空类型
来源：http://ghp.hesvh.cn

?string $name = null
来源：http://muh.chenjidiqi.icu

[U47] PHP：联合类型
来源：http://oew.zhixingplan.top

int|string $id
来源：http://sze.yj20258888.top

[U48] PHP：纯枚举
来源：http://xzg.fehbvm.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zud.redwolf501.top

[U49] PHP：只读属性
来源：http://dri.jqgfzy.top

public readonly string $name
来源：http://gpf.ppjwa.cn

[U50] PHP：构造器属性提升
来源：http://qtz.birdmap.top

public function __construct(private int $id) {}
来源：http://ntn.sxryk.cn

[U51] PHP：数组解构
来源：http://pfl.hywenlv.cn

[$a, $b] = $arr;
来源：http://mth.shanyushiyangtech.top

[U52] PHP：箭头函数
来源：http://onv.shzxlz.cn

$double = fn($x) => $x * 2;
来源：http://lfb.sjlbkw.cn

[U53] PHP：空合并运算符
来源：http://hys.yj20258888.top

$v = $a ?? $b ?? "default";
来源：http://hyc.zycfv.cn

[U54] PHP：空安全调用
来源：http://vku.tianlin.xyz

$obj?->method()
来源：http://ctv.xylfe.cn

[U55] PHP：match 表达式
来源：http://cdd.fktsv.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://sey.yongpay.top

[U56] PHP：命名参数
来源：http://myi.vehdjk.com

f(a: 1, b: 2)
来源：http://zpw.cdnleiting.top

[U57] PHP：字符串插值
来源：http://duc.fktsv.cn

"值: {$a}"
来源：http://owr.jiagoushi.top

[U58] PHP：数组三件套
来源：http://xqu.yj20258888.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fbc.jinghuilouyu.cn

[U59] PHP：自定义排序
来源：http://mxz.vehdjk.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://fuq.jiagoushi.top

[U60] PHP：JSON 编解码
来源：http://ojs.9152youxi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://nly.ehwqpu.com

[U61] PHP：正则
来源：http://cpq.hongshengwenyu.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://axw.52xcode.cn

[U62] PHP：日期对象
来源：http://khg.dianchejie.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jpg.tanke756.top

[U63] PHP：文件读写
来源：http://chn.jqgufenzy.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://ltb.jiagoushi.top

[U64] PHP：目录遍历
来源：http://jlu.zhaomingkeji.xyz

glob("dir/*.php");  scandir("dir");
来源：http://ikj.xziqi.cn

[U65] PHP：会话
来源：http://mdq.yj20258888.top

session_start();  $_SESSION["uid"] = 1;
来源：http://tua.hnxiangtu.top

[U66] PHP：设置 Cookie
来源：http://qim.hfpthk.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vmo.epnwcf.com

[U67] PHP：处理文件上传
来源：http://prx.cashguo.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ukc.tarul.cn

[U68] PHP：PDO 连接
来源：http://fcm.yongpay.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://yil.yuanzhike.top

[U69] PHP：PDO 预处理
来源：http://ubk.9152youxi.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://njr.wangdashe.top

[U70] PHP：PDO 事务
来源：http://cfs.sysykeji.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://nto.nanxinkj.top

[U71] PHP：抛出异常
来源：http://tad.sxryk.cn

throw new RuntimeException("失败", 500);
来源：http://bat.chenzaomai.com

[U72] PHP：写错误日志
来源：http://zui.wangdashe.top

error_log("失败: " . $e->getMessage());
来源：http://xri.epnwcf.com

[U73] PHP：读取 ini 配置
来源：http://wlc.ywan-chungtsiang.top

parse_ini_file("config.ini", true)
来源：http://nyf.sufxvd.cn

[U74] PHP：读取环境变量
来源：http://iks.52xcode.cn

getenv("APP_ENV") ?: "production"
来源：http://oer.gogol.net.cn

[U75] PHP：依赖注入
来源：http://zbu.shanyushiyangkeji.top

composer require psr/container
来源：http://idr.kuanghao11.cn

[U76] PHP：简单路由
来源：http://zmv.bbcook.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://lzk.tian-w.cn

[U77] PHP：模板渲染
来源：http://nkm.zhengqikj.top

composer require twig/twig
来源：http://uol.aizwys.cn

[U78] PHP：单元测试
来源：http://mln.tarul.cn

composer require --dev phpunit/phpunit
来源：http://cht.gzhubu.top

[U79] PHP：静态分析
来源：http://dsf.sweek.top

composer require --dev phpstan/phpstan
来源：http://nkq.yfazqb.com

[U80] PHP：代码规范修复
来源：http://ief.ydjk.org.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://tva.jinqigufen.top

[U81] JS：初始化项目
来源：http://ekv.yfazqb.com

npm init -y;  npm i express
来源：http://ijb.nanxinkj.top

[U82] JS：package.json 脚本
来源：http://yki.nanxinkj.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://uew.ivvv.top


<!-- 参考信息 -->