代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://peo.ywan-chungtsiang.top

[S57] C++：编译期常量
来源：http://wjz.tanke756.top

constexpr int N = 10;
来源：http://tph.jiagoushi.top

[S58] C++：命名空间
来源：http://xlf.snrcjt.cn

namespace ns { int f() { return 1; } }
来源：http://gij.aizwys.cn

[S59] C++：静态断言
来源：http://leb.feifeiyinyue.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vsl.gzhubu.top

[S60] C++：遍历并删除元素
来源：http://nuj.jqgfzy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hph.tanke756.top

================================================================================
来源：http://ihu.yfazqb.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://sjn.jiagoushi.top

================================================================================
来源：http://nmm.zhaomingkeji.xyz

[T01] Kotlin：Hello World
来源：http://ntj.iojbl.cn

println("Hello")
来源：http://gsu.yanxiufei.cn

[T02] Kotlin：变量
来源：http://qig.chenlongwang.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lmj.zycfv.cn

[T03] Kotlin：字符串模板
来源：http://glv.yueranfly.top

"值: $b"
来源：http://ajq.dianchejie.cn

[T04] Kotlin：空安全
来源：http://nvm.jqgfzy.top

val n: String? = null;  n?.length
来源：http://olq.hnqzz.top

[T05] Kotlin：when 表达式
来源：http://pvi.bbcook.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ntq.jinghuilouyu.cn

[T06] Kotlin：集合映射
来源：http://hrp.daria6918.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fpm.birdmap.top

[T07] Kotlin：集合过滤
来源：http://bak.yongpay.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://vvx.jinghuilouyu.cn

[T08] Kotlin：数据类
来源：http://dot.ywan-chungtsiang.top

data class User(val name: String, val age: Int)
来源：http://mmh.feifeiyinyue.top

[T09] Kotlin：扩展函数
来源：http://rlm.sysykeji.top

fun String.exclaim() = this + "!"
来源：http://bto.nanxuanxn.top

[T10] Kotlin：默认参数
来源：http://hxh.fktsv.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://uhu.cashguo.top

[T11] Kotlin：协程
来源：http://sfm.jqgufenzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://pej.fzhhl.top

[T12] Kotlin：解构声明
来源：http://fqk.chenlongwang.top

val (a, b) = Pair(1, 2)
来源：http://tce.vehdjk.com

[T13] Kotlin：只读 Map
来源：http://zzg.fktsv.cn

val m = mapOf("a" to 1)
来源：http://bgu.ppjwa.cn

[T14] Kotlin：循环
来源：http://cxw.hesvh.cn

for (i in 1..10) println(i)
来源：http://cbo.yj20258888.top

[T15] Kotlin：接口
来源：http://gsn.guowangkeji.top

interface Shape { fun area(): Double }
来源：http://ifu.yj20258888.top

[T16] Swift：Hello World
来源：http://lra.ydzc1.top

print("Hello")
来源：http://was.fanxiaobao.xyz

[T17] Swift：变量与常量
来源：http://seq.cucudq.cn

var a = 1;  let b = 2
来源：http://rmf.yuanzhike.top

[T18] Swift：字符串插值
来源：http://pun.yj20258.top

"值: \(b)"
来源：http://krv.cheryme.top

[T19] Swift：可选绑定
来源：http://hpq.ppjwa.cn

if let n = opt { print(n) }
来源：http://gwi.fanxiaobao.xyz

[T20] Swift：数组操作
来源：http://bqt.sufxvd.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jcq.yj20258.top

[T21] Swift：遍历
来源：http://ste.iojbl.cn

for x in a { print(x) }
来源：http://qii.aizwys.cn

[T22] Swift：字典
来源：http://mbe.chenjidiqi.icu

var d = ["a": 1];  d["b"] = 2
来源：http://yrd.xingfuxueyuan.xyz

[T23] Swift：函数
来源：http://jhs.snrcjt.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ecw.yj20258888.top

[T24] Swift：闭包
来源：http://scx.chenjidiqi.icu

let f = { (x: Int) -> Int in x * 2 }
来源：http://otq.fehbvm.com

[T25] Swift：结构体
来源：http://bco.ybcxt.top

struct P { var x: Int }
来源：http://fea.chenlongwang.top

[T26] Swift：类与重写
来源：http://zav.gaohongyu789.top

class A: Base { override func f() {} }
来源：http://tlj.quarkkingdee.top

[T27] Swift：错误处理
来源：http://rrr.zhaomingkeji.xyz

do { try f() } catch { print(error) }
来源：http://zob.yuxming.cn

[T28] Swift：枚举
来源：http://jph.ydzc1.top

enum Color { case red, green }
来源：http://dcf.pycfn.com

[T29] Swift：guard 提前返回
来源：http://zyh.daxiang520.top

guard let x = opt else { return }
来源：http://tnx.zhengqikj.top

[T30] Swift：协议
来源：http://ebp.hfpthk.cn

protocol Shape { func area() -> Double }
来源：http://tlh.jianghu66.top

[T31] Lua：Hello World
来源：http://xzx.feifeiyinyue.top

print("Hello")
来源：http://prt.quarkkingdee.top

[T32] Lua：局部变量
来源：http://qdi.birdmap.top

local a = 1
来源：http://veo.cashguo.top

[T33] Lua：表（数组）
来源：http://zqe.bjfxy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://kih.fehbvm.com

[T34] Lua：遍历表
来源：http://mkv.hfpthk.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://wjm.aizwys.cn

[T35] Lua：字典表
来源：http://sfi.fanxiaobao.xyz

local d = { a = 1 };  d.b = 2
来源：http://nyn.tarul.cn

[T36] Lua：函数
来源：http://zpq.aizwys.cn

function add(a, b) return a + b end
来源：http://ovm.hnqzz.top

[T37] Lua：字符串拼接
来源：http://oxa.xylfe.cn

"a" .. "b"
来源：http://ayq.vqdsnc.cn

[T38] Lua：条件
来源：http://rnc.shanyushiyangkeji.top

if x > 0 then print("正") end
来源：http://hyp.chenzaomai.com

[T39] Lua：模式匹配
来源：http://qyk.birdmap.top

string.find(s, "%d+")
来源：http://jet.xingfuxueyuan.xyz

[T40] Lua：元表
来源：http://uzb.wangdashe.top

setmetatable({}, { __index = base })
来源：http://njt.hammf.cn

[T41] Perl：Hello World
来源：http://ver.cqqwz.cn

print "Hello\n";
来源：http://cpo.fengsongda.top

[T42] Perl：变量类型
来源：http://xge.tian-w.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bug.ctjpmb.com

[T43] Perl：字符串插值
来源：http://wtr.jiagoushi.top

"值: $a"
来源：http://awd.c1oappe.top

[T44] Perl：条件
来源：http://weq.zhixingplan.top

if ($a > 0) { print "正"; }
来源：http://qnl.zhixingplan.top

[T45] Perl：数组遍历
来源：http://mxg.chenlongwang.top

for my $x (@arr) { print $x; }
来源：http://eye.cdnleiting.top

[T46] Perl：哈希操作
来源：http://aaz.yongpay.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://klf.ppjwa.cn

[T47] Perl：正则捕获
来源：http://vmi.kuanghao11.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://szr.sjlbkw.cn

[T48] Perl：正则替换
来源：http://xiy.nanxuanxn.top

$s =~ s/old/new/g;
来源：http://zrd.smart0.xyz

[T49] Perl：函数
来源：http://ceg.birdmap.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ose.0kj1m.cn

[T50] Perl：逐行读文件
来源：http://sea.pengpengdd.cyou

open my $fh, "<", "a.txt" or die $!;
来源：http://zqu.zhaomingkeji.xyz

while (my $line = <$fh>) { print $line; }
来源：http://euc.yvedp.cn

[T51] Scala：Hello World
来源：http://gfe.guowangkeji.top

println("Hello")
来源：http://bic.zhengqikj.top

[T52] Scala：变量
来源：http://kog.tianlin.xyz

val a = 1;  var b = 2
来源：http://xrj.hywenlv.cn

[T53] Scala：字符串插值
来源：http://ooc.yonumen.top

s"值: $b"
来源：http://svm.xuetiantiany.cn

[T54] Scala：集合映射
来源：http://jva.meibo888.top

List(1, 2, 3).map(_ * 2)
来源：http://cek.hywenlv.cn

[T55] Scala：集合过滤
来源：http://omy.gotoacloud.top

List(1, 2, 3).filter(_ > 1)
来源：http://faq.cheryme.top

[T56] Scala：样例类
来源：http://duj.ybcxt.top

case class User(name: String, age: Int)
来源：http://epu.cucudq.cn

[T57] Scala：模式匹配
来源：http://xbg.guannengcc.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://vhy.mhx1999.top

[T58] Scala：函数定义
来源：http://dhr.svipenyu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://kzx.fanxiaobao.xyz

[T59] Scala：循环
来源：http://irz.sweek.top

for (i <- 1 to 10) println(i)
来源：http://ytd.yuanzhike.top

[T60] Scala：折叠
来源：http://xaz.0kj1m.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mgr.chenzaomai.com

================================================================================
来源：http://hzu.yfazqb.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ydp.feifeiyinyue.top

================================================================================
来源：http://lbo.ywan-chungtsiang.top

[U01] Py：创建虚拟环境
来源：http://wsc.aizwys.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mhu.zhengqikj.top

[U02] Py：导出 / 安装依赖
来源：http://wia.fengsongda.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jjl.zhiwuduotai.top

[U03] Py：加载 .env 配置
来源：http://otf.hongshengwenyu.top

from dotenv import load_dotenv; load_dotenv()
来源：http://zgx.tianlin.xyz

[U04] Py：变量调试打印
来源：http://vfx.mhx1999.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zgn.shangyingyoupin.top

[U05] Py：列表去重且保序
来源：http://fwe.daxiang520.top

list(dict.fromkeys(arr))
来源：http://sec.fehbvm.com

[U06] Py：合并两个字典
来源：http://yfc.jyoumei.cn

{**a, **b}
来源：http://tht.hammf.cn

[U07] Py：反转字典键值
来源：http://jnv.fzhhl.top

{v: k for k, v in d.items()}
来源：http://jla.fzhhl.top

[U08] Py：展平二维列表
来源：http://clm.316326.xyz

[y for x in nested for y in x]
来源：http://rey.tarul.cn

[U09] Py：字典取最大值的键
来源：http://evv.shuidangran.top

max(d, key=d.get)
来源：http://vyb.uphjek.com

[U10] Py：按值排序字典
来源：http://wgx.hnxiangtu.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yqz.cucudq.cn

[U11] Py：生成器表达式
来源：http://qzr.haohaochexian.top

(x * 2 for x in arr)
来源：http://jed.tarul.cn

[U12] Py：取出现最多的 3 个元素
来源：http://hij.ybcxt.top

Counter(arr).most_common(3)
来源：http://bns.zdbjq.cn

[U13] Py：固定长度队列
来源：http://bsh.gogol.net.cn

deque(maxlen=10)
来源：http://eda.c1oappe.top

[U14] Py：分组收集到列表
来源：http://ujh.wangshuangyany.cn

defaultdict(list)
来源：http://tys.wangshuangyany.cn

[U15] Py：高精度计时
来源：http://ura.0kj1m.cn

t = time.perf_counter()
来源：http://emn.ybcxt.top

[U16] Py：命令行参数解析
来源：http://rpm.xylfe.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ivi.xylfe.cn

[U17] Py：初始化日志
来源：http://nzp.meibo888.top

logging.basicConfig(level=logging.INFO)
来源：http://cqu.wangdashe.top

[U18] Py：预编译正则
来源：http://ztu.gotoacloud.top

pat = re.compile(r"\d+")
来源：http://riu.ppjwa.cn

[U19] Py：正则替换带回调
来源：http://xkc.hfpthk.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jla.feifeiyinyue.top

[U20] Py：缓存函数结果
来源：http://cxn.zhoulong.xyz

@functools.lru_cache(maxsize=None)
来源：http://ona.fanxiaobao.xyz

[U21] Py：自定义上下文管理器
来源：http://rin.hywenlv.cn

@contextlib.contextmanager
来源：http://cbo.nanxuanxn.top

[U22] Py：矩阵转置
来源：http://uso.tanke756.top

list(zip(*m))
来源：http://wgn.gaohongyu789.top

[U23] Py：分块读取大文件
来源：http://fjf.haohaochexian.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rhy.zhengqikj.top

[U24] Py：路径操作
来源：http://ifl.0kj1m.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ruo.jiagoushi.top

[U25] Py：CSV 按字典读
来源：http://bcw.yuxming.cn

csv.DictReader(f)
来源：http://uyu.fengsongda.top

[U26] Py：并发下载
来源：http://kzg.havefunace.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hvr.zhixingplan.top

[U27] Py：异步 HTTP
来源：http://prg.c1oappe.top

aiohttp.ClientSession() 配合 async with
来源：http://vjb.yueranfly.top

[U28] Py：类型别名
来源：http://vbl.zhixingplan.top

UserId = int
来源：http://ads.sufxvd.cn

[U29] Py：属性校验
来源：http://ifp.yuanzhike.top

@property 与 @x.setter 配合
来源：http://gtt.haohaochexian.top

[U30] Py：数据类
来源：http://raj.hongshengwenyu.top

@dataclass(slots=True)
来源：http://ilt.uphjek.com

[U31] Py：单测
来源：http://aij.316326.xyz

python -m pytest -q
来源：http://jya.52xcode.cn

[U32] Py：代码格式化
来源：http://ops.chenjidiqi.icu

ruff format . && ruff check --fix .
来源：http://fii.xuetiantiany.cn

[U33] Py：打包发布
来源：http://hcu.xuanzx.com

python -m build  （依赖 pyproject.toml）
来源：http://xfo.redwolf501.top

[U34] Py：判断编码
来源：http://ifk.yangfankeji.com

chardet.detect(raw)
来源：http://aqc.jinqigufen.top

[U35] Py：发送邮件
来源：http://evr.vqdsnc.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tqk.0kj1m.cn

[U36] Py：定时任务
来源：http://uhu.meibo888.top

schedule.every(10).minutes.do(job)
来源：http://shl.c1oappe.top

[U37] Py：读写 Excel
来源：http://xnu.fehbvm.com

pandas.read_excel / DataFrame.to_excel
来源：http://cpc.haohaochexian.top

[U38] Py：获取脚本所在目录
来源：http://wbw.jinqigufen.top

Path(__file__).resolve().parent
来源：http://lok.yvedp.cn

[U39] Py：判断是否在交互环境
来源：http://fya.yvedp.cn

sys.stdout.isatty()
来源：http://yhd.52xcode.cn

[U40] Py：打印到标准错误
来源：http://vtx.gogol.net.cn

print("err", file=sys.stderr)
来源：http://oyk.yangfankeji.com

[U41] PHP：初始化 Composer 项目
来源：http://swr.meibo888.top

composer init;  composer require guzzlehttp/guzzle
来源：http://wjp.tianlin.xyz

[U42] PHP：PSR-4 自动加载
来源：http://ute.yj20258.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xkz.jinqigfzy.top

[U43] PHP：声明命名空间
来源：http://egl.xziqi.cn

namespace App\Http;
来源：http://hee.wangdashe.top

[U44] PHP：开启严格类型
来源：http://mgr.hesvh.cn

declare(strict_types=1);
来源：http://wkr.hesvh.cn

[U45] PHP：类型声明与返回类型
来源：http://hxt.tianlin.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://mpw.cdnleiting.top

[U46] PHP：可空类型
来源：http://ocz.feifeiyinyue.top

?string $name = null
来源：http://aqf.dashuyun.cn

[U47] PHP：联合类型
来源：http://nvg.iojbl.cn

int|string $id
来源：http://ncw.ydzc1.top

[U48] PHP：纯枚举
来源：http://nve.fanxiaobao.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://pqy.ydzc1.top

[U49] PHP：只读属性
来源：http://buj.quarkkingdee.top

public readonly string $name
来源：http://wlv.gzhubu.top

[U50] PHP：构造器属性提升
来源：http://bba.sweek.top

public function __construct(private int $id) {}
来源：http://cdi.havefunace.top

[U51] PHP：数组解构
来源：http://bdx.hnxiangtu.top

[$a, $b] = $arr;
来源：http://xot.zhongyouzk.top

[U52] PHP：箭头函数
来源：http://nbr.fehbvm.com

$double = fn($x) => $x * 2;
来源：http://tcc.wangshuangyany.cn

[U53] PHP：空合并运算符
来源：http://wwo.epnwcf.com

$v = $a ?? $b ?? "default";
来源：http://dwn.epnwcf.com

[U54] PHP：空安全调用
来源：http://lni.jiagoushi.top

$obj?->method()
来源：http://crx.shzxlz.cn

[U55] PHP：match 表达式
来源：http://yrz.zdqjudy.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://pfj.zycfv.cn

[U56] PHP：命名参数
来源：http://dgl.hnqzz.top

f(a: 1, b: 2)
来源：http://yff.hongshengwenyu.top

[U57] PHP：字符串插值
来源：http://ruy.svipenyu.cn

"值: {$a}"
来源：http://kaq.hysaishi.cn

[U58] PHP：数组三件套
来源：http://cfq.yongpay.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://enf.tian-w.cn

[U59] PHP：自定义排序
来源：http://apl.chenzaomai.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://odk.fehbvm.com

[U60] PHP：JSON 编解码
来源：http://gna.0kj1m.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://oke.ctjpmb.com

[U61] PHP：正则
来源：http://vst.shzxlz.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://aey.gaohongyu789.top

[U62] PHP：日期对象
来源：http://xfp.daria6918.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://kow.fehbvm.com

[U63] PHP：文件读写
来源：http://rgg.gotoacloud.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://rvu.jinqigfzy.top

[U64] PHP：目录遍历
来源：http://txs.uphjek.com

glob("dir/*.php");  scandir("dir");
来源：http://jkq.vehdjk.com

[U65] PHP：会话
来源：http://frk.zhengqikj.top

session_start();  $_SESSION["uid"] = 1;
来源：http://zco.gzhubu.top

[U66] PHP：设置 Cookie
来源：http://ooe.ivvv.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yit.xuanzx.com

[U67] PHP：处理文件上传
来源：http://lkt.jqgufenzy.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://kqr.jqgufenzy.top

[U68] PHP：PDO 连接
来源：http://vwh.fktsv.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dfe.yj20258.top

[U69] PHP：PDO 预处理
来源：http://adn.xinyue.icu

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lge.zycfv.cn

[U70] PHP：PDO 事务
来源：http://uzr.sweek.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://uhe.zhiwuduotai.top

[U71] PHP：抛出异常
来源：http://qpi.jinyuanbaomall.cn

throw new RuntimeException("失败", 500);
来源：http://fvq.cdnleiting.top

[U72] PHP：写错误日志
来源：http://ieo.chenlongwang.top

error_log("失败: " . $e->getMessage());
来源：http://edl.fanxiaobao.xyz

[U73] PHP：读取 ini 配置
来源：http://bfe.smart0.xyz

parse_ini_file("config.ini", true)
来源：http://iyu.tarul.cn

[U74] PHP：读取环境变量
来源：http://zvt.xinyue.icu

getenv("APP_ENV") ?: "production"
来源：http://ocu.ctjpmb.com

[U75] PHP：依赖注入
来源：http://ztm.pycfn.com

composer require psr/container
来源：http://cmw.yfazqb.com

[U76] PHP：简单路由
来源：http://flc.chenlongwang.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://zrs.zycfv.cn

[U77] PHP：模板渲染
来源：http://yoq.vehdjk.com

composer require twig/twig
来源：http://erj.dashuyun.cn

[U78] PHP：单元测试
来源：http://kpu.jinyuanbaomall.cn

composer require --dev phpunit/phpunit
来源：http://ryy.epnwcf.com

[U79] PHP：静态分析
来源：http://cgo.c1oappe.top

composer require --dev phpstan/phpstan
来源：http://cjj.0kj1m.cn

[U80] PHP：代码规范修复
来源：http://cve.jiagoushi.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://sck.dianchejie.cn

[U81] JS：初始化项目
来源：http://efe.aizwys.cn

npm init -y;  npm i express
来源：http://mom.zhengqikj.top

[U82] JS：package.json 脚本
来源：http://inf.jqgufenzy.top

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://nph.zhaomingkeji.xyz


<!-- 参考信息 -->