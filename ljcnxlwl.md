代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kht.wangdashe.top

[S55] C++：结构化绑定
来源：http://ifv.hammf.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://fqb.jianghu66.top

[S56] C++：optional
来源：http://iyc.yonumen.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jpb.nanxinkj.top

[S57] C++：编译期常量
来源：http://dgk.c1oappe.top

constexpr int N = 10;
来源：http://tqu.ctjpmb.com

[S58] C++：命名空间
来源：http://jov.vehdjk.com

namespace ns { int f() { return 1; } }
来源：http://fxe.svipenyu.cn

[S59] C++：静态断言
来源：http://qmp.9152youxi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lno.hongshengwenyu.top

[S60] C++：遍历并删除元素
来源：http://jgf.vqdsnc.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nyb.wangshuangyany.cn

================================================================================
来源：http://zwc.fanxiaobao.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uvp.c1oappe.top

================================================================================
来源：http://pin.jianghu66.top

[T01] Kotlin：Hello World
来源：http://ldr.wangdashe.top

println("Hello")
来源：http://osf.wangdashe.top

[T02] Kotlin：变量
来源：http://zzz.9152youxi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wxi.havefunace.top

[T03] Kotlin：字符串模板
来源：http://cwt.pengpengdd.cyou

"值: $b"
来源：http://yer.fzhhl.top

[T04] Kotlin：空安全
来源：http://lfi.aibaodan.cn

val n: String? = null;  n?.length
来源：http://xzj.yanxiufei.cn

[T05] Kotlin：when 表达式
来源：http://zqu.zhijiandao.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://owj.sufxvd.cn

[T06] Kotlin：集合映射
来源：http://uat.nanxinkj.top

listOf(1, 2, 3).map { it * 2 }
来源：http://tjc.yueranfly.top

[T07] Kotlin：集合过滤
来源：http://bqd.jinyuanbaomall.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wsw.hfpthk.cn

[T08] Kotlin：数据类
来源：http://qdr.yj20258.top

data class User(val name: String, val age: Int)
来源：http://muz.guowangkeji.top

[T09] Kotlin：扩展函数
来源：http://dfv.zhiwuduotai.top

fun String.exclaim() = this + "!"
来源：http://hym.pycfn.com

[T10] Kotlin：默认参数
来源：http://kls.yj202588.top

fun greet(name: String = "World") = "Hi $name"
来源：http://kbf.epnwcf.com

[T11] Kotlin：协程
来源：http://mre.yanxiufei.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://kfh.gotoacloud.top

[T12] Kotlin：解构声明
来源：http://diu.redwolf501.top

val (a, b) = Pair(1, 2)
来源：http://zba.smart0.xyz

[T13] Kotlin：只读 Map
来源：http://cgv.cucudq.cn

val m = mapOf("a" to 1)
来源：http://zky.yonumen.top

[T14] Kotlin：循环
来源：http://hnj.dashuyun.cn

for (i in 1..10) println(i)
来源：http://mvh.ydjk.org.cn

[T15] Kotlin：接口
来源：http://xve.hesvh.cn

interface Shape { fun area(): Double }
来源：http://lui.dianchejie.cn

[T16] Swift：Hello World
来源：http://vtr.daria6918.cn

print("Hello")
来源：http://tuu.jinqigfzy.top

[T17] Swift：变量与常量
来源：http://mgr.haohaochexian.top

var a = 1;  let b = 2
来源：http://smk.ydjk.org.cn

[T18] Swift：字符串插值
来源：http://gmp.zdqjudy.top

"值: \(b)"
来源：http://zhe.ehwqpu.com

[T19] Swift：可选绑定
来源：http://iqf.dianchejie.cn

if let n = opt { print(n) }
来源：http://acb.52xcode.cn

[T20] Swift：数组操作
来源：http://xrl.sweek.top

var a = [1, 2, 3];  a.append(4)
来源：http://imy.vehdjk.com

[T21] Swift：遍历
来源：http://evk.cheryme.top

for x in a { print(x) }
来源：http://wpt.andypj.xyz

[T22] Swift：字典
来源：http://qqz.gogol.net.cn

var d = ["a": 1];  d["b"] = 2
来源：http://iam.yuanzhike.top

[T23] Swift：函数
来源：http://ara.jinqigufen.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://irr.hnxiangtu.top

[T24] Swift：闭包
来源：http://wpu.zdbjq.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://kbp.zhixingplan.top

[T25] Swift：结构体
来源：http://syu.wangdashe.top

struct P { var x: Int }
来源：http://eha.aibaodan.cn

[T26] Swift：类与重写
来源：http://oqa.fehbvm.com

class A: Base { override func f() {} }
来源：http://ffz.sufxvd.cn

[T27] Swift：错误处理
来源：http://zmi.cheryme.top

do { try f() } catch { print(error) }
来源：http://yie.tianlin.xyz

[T28] Swift：枚举
来源：http://zmx.haohaochexian.top

enum Color { case red, green }
来源：http://crb.sufxvd.cn

[T29] Swift：guard 提前返回
来源：http://rbi.nanxinkj.top

guard let x = opt else { return }
来源：http://syv.mhx1999.top

[T30] Swift：协议
来源：http://xsg.jyoumei.cn

protocol Shape { func area() -> Double }
来源：http://mms.xingfuxueyuan.xyz

[T31] Lua：Hello World
来源：http://qih.jinyuanbaomall.cn

print("Hello")
来源：http://mbh.c1oappe.top

[T32] Lua：局部变量
来源：http://ciu.fehbvm.com

local a = 1
来源：http://eso.yj202588.top

[T33] Lua：表（数组）
来源：http://tjn.yj20258.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ztj.xingfuxueyuan.xyz

[T34] Lua：遍历表
来源：http://zhz.fktsv.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://tcj.zdbjq.cn

[T35] Lua：字典表
来源：http://okl.svipenyu.cn

local d = { a = 1 };  d.b = 2
来源：http://ilv.yvedp.cn

[T36] Lua：函数
来源：http://lzh.epnwcf.com

function add(a, b) return a + b end
来源：http://iha.jiagoushi.top

[T37] Lua：字符串拼接
来源：http://ifb.gotoacloud.top

"a" .. "b"
来源：http://taf.epnwcf.com

[T38] Lua：条件
来源：http://ael.dianchejie.cn

if x > 0 then print("正") end
来源：http://xgz.jqgfzy.top

[T39] Lua：模式匹配
来源：http://lbe.yonumen.top

string.find(s, "%d+")
来源：http://snt.hysaishi.cn

[T40] Lua：元表
来源：http://zyq.chenzaomai.com

setmetatable({}, { __index = base })
来源：http://tda.hywenlv.cn

[T41] Perl：Hello World
来源：http://fjc.pycfn.com

print "Hello\n";
来源：http://yet.shanyushiyangtech.top

[T42] Perl：变量类型
来源：http://tmd.zhiwuduotai.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zic.nwbrower.top

[T43] Perl：字符串插值
来源：http://yzs.zdqjudy.top

"值: $a"
来源：http://tlw.iojbl.cn

[T44] Perl：条件
来源：http://hzy.aibaodan.cn

if ($a > 0) { print "正"; }
来源：http://zrr.jlsjyb.cn

[T45] Perl：数组遍历
来源：http://vio.52xcode.cn

for my $x (@arr) { print $x; }
来源：http://tmv.zhengqikj.top

[T46] Perl：哈希操作
来源：http://kct.gotoacloud.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sci.smart0.xyz

[T47] Perl：正则捕获
来源：http://ipa.shzxlz.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://hxl.cdnleiting.top

[T48] Perl：正则替换
来源：http://bns.bbcook.cn

$s =~ s/old/new/g;
来源：http://ejm.wangdashe.top

[T49] Perl：函数
来源：http://nda.meibo888.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qvf.c1oappe.top

[T50] Perl：逐行读文件
来源：http://mtz.gogol.net.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://gwc.aibaodan.cn

while (my $line = <$fh>) { print $line; }
来源：http://zoi.fktsv.cn

[T51] Scala：Hello World
来源：http://mqj.kuanghao11.cn

println("Hello")
来源：http://ppl.cashguo.top

[T52] Scala：变量
来源：http://ira.redwolf501.top

val a = 1;  var b = 2
来源：http://sob.xingfuxueyuan.xyz

[T53] Scala：字符串插值
来源：http://zdb.zhongyouzk.top

s"值: $b"
来源：http://fbo.jyoumei.cn

[T54] Scala：集合映射
来源：http://dfp.zhoulong.xyz

List(1, 2, 3).map(_ * 2)
来源：http://smo.wangshuangyany.cn

[T55] Scala：集合过滤
来源：http://qrm.tanke756.top

List(1, 2, 3).filter(_ > 1)
来源：http://gkg.shzxlz.cn

[T56] Scala：样例类
来源：http://cas.iojbl.cn

case class User(name: String, age: Int)
来源：http://lce.tarul.cn

[T57] Scala：模式匹配
来源：http://auo.zhongyouzk.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://jry.yongpay.top

[T58] Scala：函数定义
来源：http://sno.jianghu66.top

def add(a: Int, b: Int): Int = a + b
来源：http://bub.vehdjk.com

[T59] Scala：循环
来源：http://kzj.fehbvm.com

for (i <- 1 to 10) println(i)
来源：http://xif.jyoumei.cn

[T60] Scala：折叠
来源：http://riy.uphjek.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pji.dashuyun.cn

================================================================================
来源：http://udj.jinqigufen.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rrt.tian-w.cn

================================================================================
来源：http://eoe.daxiang520.top

[U01] Py：创建虚拟环境
来源：http://kby.sufxvd.cn

python -m venv .venv && source .venv/bin/activate
来源：http://fur.nwbrower.top

[U02] Py：导出 / 安装依赖
来源：http://fyf.sufxvd.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kgn.0kj1m.cn

[U03] Py：加载 .env 配置
来源：http://jhm.hnqzz.top

from dotenv import load_dotenv; load_dotenv()
来源：http://qjf.fanxiaobao.xyz

[U04] Py：变量调试打印
来源：http://emj.yangfankeji.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mtn.chenjidiqi.icu

[U05] Py：列表去重且保序
来源：http://fvy.jianghu66.top

list(dict.fromkeys(arr))
来源：http://ytp.ydzc1.top

[U06] Py：合并两个字典
来源：http://deo.yj20258.top

{**a, **b}
来源：http://cnx.jlsjyb.cn

[U07] Py：反转字典键值
来源：http://gwc.quarkkingdee.top

{v: k for k, v in d.items()}
来源：http://tmp.jqgfzy.top

[U08] Py：展平二维列表
来源：http://thy.feifeiyinyue.top

[y for x in nested for y in x]
来源：http://jfd.yj20258888.top

[U09] Py：字典取最大值的键
来源：http://bph.xylfe.cn

max(d, key=d.get)
来源：http://kct.zhengqikj.top

[U10] Py：按值排序字典
来源：http://yzh.cdnleiting.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://afv.yangfankeji.com

[U11] Py：生成器表达式
来源：http://tlf.9152youxi.cn

(x * 2 for x in arr)
来源：http://qqe.sjlbkw.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ani.hysaishi.cn

Counter(arr).most_common(3)
来源：http://ckw.yueranfly.top

[U13] Py：固定长度队列
来源：http://wnf.shanyushiyangtech.top

deque(maxlen=10)
来源：http://nch.bjfxy.top

[U14] Py：分组收集到列表
来源：http://mfo.shanyushiyangtech.top

defaultdict(list)
来源：http://feg.tian-w.cn

[U15] Py：高精度计时
来源：http://gxa.tanke756.top

t = time.perf_counter()
来源：http://rsf.zhiwuduotai.top

[U16] Py：命令行参数解析
来源：http://qpc.smart0.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://iba.vqdsnc.cn

[U17] Py：初始化日志
来源：http://rbe.xuanzx.com

logging.basicConfig(level=logging.INFO)
来源：http://bhr.shzxlz.cn

[U18] Py：预编译正则
来源：http://yvv.wangdashe.top

pat = re.compile(r"\d+")
来源：http://hrv.wangshuangyany.cn

[U19] Py：正则替换带回调
来源：http://xjr.yj20258888.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://blj.c1oappe.top

[U20] Py：缓存函数结果
来源：http://qhw.52xcode.cn

@functools.lru_cache(maxsize=None)
来源：http://mar.zhengqikj.top

[U21] Py：自定义上下文管理器
来源：http://ssj.haohaochexian.top

@contextlib.contextmanager
来源：http://pkl.fktsv.cn

[U22] Py：矩阵转置
来源：http://yuj.pengpengdd.cyou

list(zip(*m))
来源：http://gyk.fehbvm.com

[U23] Py：分块读取大文件
来源：http://kqa.dianchejie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ufv.snrcjt.cn

[U24] Py：路径操作
来源：http://ieo.zdbjq.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rhz.daxiang520.top

[U25] Py：CSV 按字典读
来源：http://vtj.jinghuilouyu.cn

csv.DictReader(f)
来源：http://ved.kuanghao11.cn

[U26] Py：并发下载
来源：http://fxm.ywan-chungtsiang.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vxy.hongshengwenyu.top

[U27] Py：异步 HTTP
来源：http://crf.epnwcf.com

aiohttp.ClientSession() 配合 async with
来源：http://pyp.jiagoushi.top

[U28] Py：类型别名
来源：http://xoa.0kj1m.cn

UserId = int
来源：http://mqz.tarul.cn

[U29] Py：属性校验
来源：http://fdh.yongpay.top

@property 与 @x.setter 配合
来源：http://utr.sysykeji.top

[U30] Py：数据类
来源：http://naj.fzhhl.top

@dataclass(slots=True)
来源：http://iuv.cucudq.cn

[U31] Py：单测
来源：http://quo.jinyuanbaomall.cn

python -m pytest -q
来源：http://bhw.9152youxi.cn

[U32] Py：代码格式化
来源：http://cdg.hammf.cn

ruff format . && ruff check --fix .
来源：http://kxy.xuetiantiany.cn

[U33] Py：打包发布
来源：http://lah.xylfe.cn

python -m build  （依赖 pyproject.toml）
来源：http://kkx.pengpengdd.cyou

[U34] Py：判断编码
来源：http://gul.tianlin.xyz

chardet.detect(raw)
来源：http://lpv.ivvv.top

[U35] Py：发送邮件
来源：http://ama.jqgufenzy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fkz.ywan-chungtsiang.top

[U36] Py：定时任务
来源：http://lxx.yj20258888.top

schedule.every(10).minutes.do(job)
来源：http://qoa.ivvv.top

[U37] Py：读写 Excel
来源：http://eje.tianlin.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://did.zdqjudy.top

[U38] Py：获取脚本所在目录
来源：http://vgv.dashuyun.cn

Path(__file__).resolve().parent
来源：http://axy.hywenlv.cn

[U39] Py：判断是否在交互环境
来源：http://amg.yj20258888.top

sys.stdout.isatty()
来源：http://mlv.ivvv.top

[U40] Py：打印到标准错误
来源：http://imi.gaohongyu789.top

print("err", file=sys.stderr)
来源：http://dfz.guowangkeji.top

[U41] PHP：初始化 Composer 项目
来源：http://gni.ydjk.org.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://zds.jinqigfzy.top

[U42] PHP：PSR-4 自动加载
来源：http://har.ppjwa.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jrc.9152youxi.cn

[U43] PHP：声明命名空间
来源：http://pmg.xziqi.cn

namespace App\Http;
来源：http://bnn.shuidangran.top

[U44] PHP：开启严格类型
来源：http://frz.yuanzhike.top

declare(strict_types=1);
来源：http://tao.kuanghao11.cn

[U45] PHP：类型声明与返回类型
来源：http://ome.nanxinkj.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ofj.zhengqikj.top

[U46] PHP：可空类型
来源：http://uwk.xuanzx.com

?string $name = null
来源：http://zfl.gzhubu.top

[U47] PHP：联合类型
来源：http://qam.dashuyun.cn

int|string $id
来源：http://cjw.c1oappe.top

[U48] PHP：纯枚举
来源：http://wzf.wangshuangyany.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://scb.shzxlz.cn

[U49] PHP：只读属性
来源：http://pan.xingfuxueyuan.xyz

public readonly string $name
来源：http://stv.zycfv.cn

[U50] PHP：构造器属性提升
来源：http://ugc.tarul.cn

public function __construct(private int $id) {}
来源：http://tgw.guowangkeji.top

[U51] PHP：数组解构
来源：http://upz.cucudq.cn

[$a, $b] = $arr;
来源：http://dhp.shanyushiyangkeji.top

[U52] PHP：箭头函数
来源：http://ryk.jqgufenzy.top

$double = fn($x) => $x * 2;
来源：http://ycv.jinqigfzy.top

[U53] PHP：空合并运算符
来源：http://tbj.birdmap.top

$v = $a ?? $b ?? "default";
来源：http://uui.nanxuanxn.top

[U54] PHP：空安全调用
来源：http://mlv.sxryk.cn

$obj?->method()
来源：http://rrd.hywenlv.cn

[U55] PHP：match 表达式
来源：http://sfb.wangdashe.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://tzl.svipenyu.cn

[U56] PHP：命名参数
来源：http://srx.guowangkeji.top

f(a: 1, b: 2)
来源：http://duh.zhengqikj.top

[U57] PHP：字符串插值
来源：http://prz.yvedp.cn

"值: {$a}"
来源：http://hjq.chenzaomai.com

[U58] PHP：数组三件套
来源：http://gfa.chenlongwang.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cim.dianchejie.cn

[U59] PHP：自定义排序
来源：http://gzy.9152youxi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tmq.zhaomingkeji.xyz

[U60] PHP：JSON 编解码
来源：http://ofp.shuidangran.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ymx.chenjidiqi.icu

[U61] PHP：正则
来源：http://wvz.shuidangran.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://clo.fzhhl.top

[U62] PHP：日期对象
来源：http://oib.9152youxi.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nlj.shanyushiyangkeji.top

[U63] PHP：文件读写
来源：http://bxj.yuxming.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://tao.dashuyun.cn

[U64] PHP：目录遍历
来源：http://xuw.yvedp.cn

glob("dir/*.php");  scandir("dir");
来源：http://ahm.daxiang520.top

[U65] PHP：会话
来源：http://rwi.tarul.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://vpo.cashguo.top

[U66] PHP：设置 Cookie
来源：http://pgm.sufxvd.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://yzi.fehbvm.com

[U67] PHP：处理文件上传
来源：http://nis.xylfe.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xyn.xziqi.cn

[U68] PHP：PDO 连接
来源：http://msc.shanyushiyangtech.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dqk.jianghu66.top

[U69] PHP：PDO 预处理
来源：http://joc.ivvv.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://foo.xylfe.cn

[U70] PHP：PDO 事务
来源：http://mmu.svipenyu.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://gep.c1oappe.top

[U71] PHP：抛出异常
来源：http://hxh.guannengcc.top

throw new RuntimeException("失败", 500);
来源：http://pxt.tarul.cn

[U72] PHP：写错误日志
来源：http://clm.mhx1999.top

error_log("失败: " . $e->getMessage());
来源：http://qmy.iojbl.cn

[U73] PHP：读取 ini 配置
来源：http://pqa.dashuyun.cn

parse_ini_file("config.ini", true)
来源：http://bsh.cdnleiting.top

[U74] PHP：读取环境变量
来源：http://jfj.wangshuangyany.cn

getenv("APP_ENV") ?: "production"
来源：http://uqi.xinyue.icu

[U75] PHP：依赖注入
来源：http://jef.andypj.xyz

composer require psr/container
来源：http://gla.cdnleiting.top

[U76] PHP：简单路由
来源：http://xdu.andypj.xyz

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://yqf.chenlongwang.top

[U77] PHP：模板渲染
来源：http://zko.ehwqpu.com

composer require twig/twig
来源：http://soy.hysaishi.cn

[U78] PHP：单元测试
来源：http://yiz.cashguo.top

composer require --dev phpunit/phpunit
来源：http://lgr.9152youxi.cn

[U79] PHP：静态分析
来源：http://zbh.52xcode.cn

composer require --dev phpstan/phpstan
来源：http://gmj.yj202588.top

[U80] PHP：代码规范修复
来源：http://nfz.pengpengdd.cyou

composer require --dev friendsofphp/php-cs-fixer
来源：http://qjj.daria6918.cn


<!-- 参考信息 -->