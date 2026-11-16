代发 wailian999

namespace ns { int f() { return 1; } }
来源：http://xhe.316326.xyz

[S59] C++：静态断言
来源：http://nwv.hnxiangtu.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://boc.xinyue.icu

[S60] C++：遍历并删除元素
来源：http://wau.jinqigfzy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qwi.9152youxi.cn

================================================================================
来源：http://sgu.fzhhl.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lpn.aibaodan.cn

================================================================================
来源：http://pcs.hnqzz.top

[T01] Kotlin：Hello World
来源：http://pxo.zhijiandao.cn

println("Hello")
来源：http://mwh.jqgfzy.top

[T02] Kotlin：变量
来源：http://nzj.hfpthk.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zgo.mhx1999.top

[T03] Kotlin：字符串模板
来源：http://xuz.fzhhl.top

"值: $b"
来源：http://xnb.shuidangran.top

[T04] Kotlin：空安全
来源：http://ajk.daria6918.cn

val n: String? = null;  n?.length
来源：http://avk.zhixingplan.top

[T05] Kotlin：when 表达式
来源：http://ygj.yfazqb.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uxw.snrcjt.cn

[T06] Kotlin：集合映射
来源：http://mct.0kj1m.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ull.pengpengdd.cyou

[T07] Kotlin：集合过滤
来源：http://hlh.yj20258888.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://bsv.cashguo.top

[T08] Kotlin：数据类
来源：http://nav.pengpengdd.cyou

data class User(val name: String, val age: Int)
来源：http://zcg.hnxiangtu.top

[T09] Kotlin：扩展函数
来源：http://jfp.nanxinkj.top

fun String.exclaim() = this + "!"
来源：http://lwo.sweek.top

[T10] Kotlin：默认参数
来源：http://qdx.gzhubu.top

fun greet(name: String = "World") = "Hi $name"
来源：http://phr.zhiwuduotai.top

[T11] Kotlin：协程
来源：http://mqm.haohaochexian.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://txh.jqgfzy.top

[T12] Kotlin：解构声明
来源：http://azo.ehwqpu.com

val (a, b) = Pair(1, 2)
来源：http://uqb.zhoulong.xyz

[T13] Kotlin：只读 Map
来源：http://bgs.gotoacloud.top

val m = mapOf("a" to 1)
来源：http://jxd.haohaochexian.top

[T14] Kotlin：循环
来源：http://mqf.hywenlv.cn

for (i in 1..10) println(i)
来源：http://xlv.wangshuangyany.cn

[T15] Kotlin：接口
来源：http://pos.xylfe.cn

interface Shape { fun area(): Double }
来源：http://rnm.jqgufenzy.top

[T16] Swift：Hello World
来源：http://jko.jlsjyb.cn

print("Hello")
来源：http://ngi.sxryk.cn

[T17] Swift：变量与常量
来源：http://rzw.jinqigfzy.top

var a = 1;  let b = 2
来源：http://xrm.hywenlv.cn

[T18] Swift：字符串插值
来源：http://zth.316326.xyz

"值: \(b)"
来源：http://mgy.dianchejie.cn

[T19] Swift：可选绑定
来源：http://ewg.sufxvd.cn

if let n = opt { print(n) }
来源：http://you.yuanzhike.top

[T20] Swift：数组操作
来源：http://xxs.pycfn.com

var a = [1, 2, 3];  a.append(4)
来源：http://klw.yfazqb.com

[T21] Swift：遍历
来源：http://xfz.fzhhl.top

for x in a { print(x) }
来源：http://zun.xuanzx.com

[T22] Swift：字典
来源：http://xxe.shanyushiyangkeji.top

var d = ["a": 1];  d["b"] = 2
来源：http://mwm.jyoumei.cn

[T23] Swift：函数
来源：http://owk.andypj.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qlx.meibo888.top

[T24] Swift：闭包
来源：http://org.jinqigufen.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://vxc.zhijiandao.cn

[T25] Swift：结构体
来源：http://ngp.zycfv.cn

struct P { var x: Int }
来源：http://aib.yj202588.top

[T26] Swift：类与重写
来源：http://wpi.ehwqpu.com

class A: Base { override func f() {} }
来源：http://org.mhx1999.top

[T27] Swift：错误处理
来源：http://mlf.xuetiantiany.cn

do { try f() } catch { print(error) }
来源：http://jip.shuidangran.top

[T28] Swift：枚举
来源：http://huz.xziqi.cn

enum Color { case red, green }
来源：http://hca.bbcook.cn

[T29] Swift：guard 提前返回
来源：http://wtk.feifeiyinyue.top

guard let x = opt else { return }
来源：http://twj.ywan-chungtsiang.top

[T30] Swift：协议
来源：http://oic.tarul.cn

protocol Shape { func area() -> Double }
来源：http://zlr.yangfankeji.com

[T31] Lua：Hello World
来源：http://vap.yongpay.top

print("Hello")
来源：http://umq.sxryk.cn

[T32] Lua：局部变量
来源：http://gkz.0kj1m.cn

local a = 1
来源：http://maq.cdnleiting.top

[T33] Lua：表（数组）
来源：http://taj.yueranfly.top

local t = {1, 2, 3};  t[4] = 4
来源：http://bnc.cdnleiting.top

[T34] Lua：遍历表
来源：http://uoq.shangyingyoupin.top

for i, v in ipairs(t) do print(i, v) end
来源：http://yor.gotoacloud.top

[T35] Lua：字典表
来源：http://zll.yj202588.top

local d = { a = 1 };  d.b = 2
来源：http://jgy.daxiang520.top

[T36] Lua：函数
来源：http://zie.shanyushiyangkeji.top

function add(a, b) return a + b end
来源：http://iah.zdbjq.cn

[T37] Lua：字符串拼接
来源：http://yic.sxryk.cn

"a" .. "b"
来源：http://mlu.sjlbkw.cn

[T38] Lua：条件
来源：http://nop.0kj1m.cn

if x > 0 then print("正") end
来源：http://xgr.bbcook.cn

[T39] Lua：模式匹配
来源：http://xil.tian-w.cn

string.find(s, "%d+")
来源：http://ycd.zhoulong.xyz

[T40] Lua：元表
来源：http://zyw.nanxuanxn.top

setmetatable({}, { __index = base })
来源：http://hil.jinghuilouyu.cn

[T41] Perl：Hello World
来源：http://qmh.gaohongyu789.top

print "Hello\n";
来源：http://fbj.cheryme.top

[T42] Perl：变量类型
来源：http://ltq.jqgfzy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vpp.nwbrower.top

[T43] Perl：字符串插值
来源：http://joi.hongshengwenyu.top

"值: $a"
来源：http://flj.316326.xyz

[T44] Perl：条件
来源：http://cub.cucudq.cn

if ($a > 0) { print "正"; }
来源：http://bjz.wangdashe.top

[T45] Perl：数组遍历
来源：http://fnc.cucudq.cn

for my $x (@arr) { print $x; }
来源：http://mqn.zhijiandao.cn

[T46] Perl：哈希操作
来源：http://zql.meibo888.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gwa.c1oappe.top

[T47] Perl：正则捕获
来源：http://phs.kuanghao11.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://uap.pycfn.com

[T48] Perl：正则替换
来源：http://rgv.hesvh.cn

$s =~ s/old/new/g;
来源：http://zpu.cdnleiting.top

[T49] Perl：函数
来源：http://xxs.hysaishi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hin.guannengcc.top

[T50] Perl：逐行读文件
来源：http://jip.andypj.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://gvi.aibaodan.cn

while (my $line = <$fh>) { print $line; }
来源：http://yyx.hongshengwenyu.top

[T51] Scala：Hello World
来源：http://kix.hesvh.cn

println("Hello")
来源：http://flx.hcnkem.com

[T52] Scala：变量
来源：http://hyc.cqqwz.cn

val a = 1;  var b = 2
来源：http://pog.bbcook.cn

[T53] Scala：字符串插值
来源：http://ndc.tanke756.top

s"值: $b"
来源：http://erb.chenlongwang.top

[T54] Scala：集合映射
来源：http://mgq.havefunace.top

List(1, 2, 3).map(_ * 2)
来源：http://spd.birdmap.top

[T55] Scala：集合过滤
来源：http://okj.hcnkem.com

List(1, 2, 3).filter(_ > 1)
来源：http://ake.ywan-chungtsiang.top

[T56] Scala：样例类
来源：http://dkr.xuetiantiany.cn

case class User(name: String, age: Int)
来源：http://oss.hfpthk.cn

[T57] Scala：模式匹配
来源：http://unc.birdmap.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://kzt.ywan-chungtsiang.top

[T58] Scala：函数定义
来源：http://bgf.smart0.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://oyz.ehwqpu.com

[T59] Scala：循环
来源：http://tdx.yuanzhike.top

for (i <- 1 to 10) println(i)
来源：http://vlx.ehwqpu.com

[T60] Scala：折叠
来源：http://mdl.ydzc1.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://aih.shuidangran.top

================================================================================
来源：http://dak.kuanghao11.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dna.hysaishi.cn

================================================================================
来源：http://kmu.9152youxi.cn

[U01] Py：创建虚拟环境
来源：http://iwa.cashguo.top

python -m venv .venv && source .venv/bin/activate
来源：http://zlv.pengpengdd.cyou

[U02] Py：导出 / 安装依赖
来源：http://cww.tanke756.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zro.gzhubu.top

[U03] Py：加载 .env 配置
来源：http://ktj.yuxming.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://hex.jqgufenzy.top

[U04] Py：变量调试打印
来源：http://xmu.jqgufenzy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lsl.smart0.xyz

[U05] Py：列表去重且保序
来源：http://wua.yuxming.cn

list(dict.fromkeys(arr))
来源：http://oej.sufxvd.cn

[U06] Py：合并两个字典
来源：http://ehu.zycfv.cn

{**a, **b}
来源：http://jpz.havefunace.top

[U07] Py：反转字典键值
来源：http://myl.ydzc1.top

{v: k for k, v in d.items()}
来源：http://qir.cdnleiting.top

[U08] Py：展平二维列表
来源：http://nel.feifeiyinyue.top

[y for x in nested for y in x]
来源：http://fwd.316326.xyz

[U09] Py：字典取最大值的键
来源：http://iop.haohaochexian.top

max(d, key=d.get)
来源：http://lqr.pycfn.com

[U10] Py：按值排序字典
来源：http://yjc.gotoacloud.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ivn.redwolf501.top

[U11] Py：生成器表达式
来源：http://jwh.xinyue.icu

(x * 2 for x in arr)
来源：http://enk.jqgufenzy.top

[U12] Py：取出现最多的 3 个元素
来源：http://qtq.epnwcf.com

Counter(arr).most_common(3)
来源：http://ken.316326.xyz

[U13] Py：固定长度队列
来源：http://loc.yonumen.top

deque(maxlen=10)
来源：http://zgq.yj202588.top

[U14] Py：分组收集到列表
来源：http://fyg.52xcode.cn

defaultdict(list)
来源：http://ryq.ydzc1.top

[U15] Py：高精度计时
来源：http://ict.hywenlv.cn

t = time.perf_counter()
来源：http://ull.ydjk.org.cn

[U16] Py：命令行参数解析
来源：http://wkl.pengpengdd.cyou

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rqz.jinqigfzy.top

[U17] Py：初始化日志
来源：http://lsj.shuidangran.top

logging.basicConfig(level=logging.INFO)
来源：http://csb.shanyushiyangtech.top

[U18] Py：预编译正则
来源：http://uuq.zdbjq.cn

pat = re.compile(r"\d+")
来源：http://hrl.fktsv.cn

[U19] Py：正则替换带回调
来源：http://kcn.hesvh.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xtu.birdmap.top

[U20] Py：缓存函数结果
来源：http://jsy.jqgufenzy.top

@functools.lru_cache(maxsize=None)
来源：http://vfe.0kj1m.cn

[U21] Py：自定义上下文管理器
来源：http://dys.ywan-chungtsiang.top

@contextlib.contextmanager
来源：http://erw.shzxlz.cn

[U22] Py：矩阵转置
来源：http://cvi.jinqigufen.top

list(zip(*m))
来源：http://obl.yonumen.top

[U23] Py：分块读取大文件
来源：http://dzi.snrcjt.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://cob.cashguo.top

[U24] Py：路径操作
来源：http://lba.yvedp.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ncd.hfpthk.cn

[U25] Py：CSV 按字典读
来源：http://fvw.yvedp.cn

csv.DictReader(f)
来源：http://gfg.9152youxi.cn

[U26] Py：并发下载
来源：http://oau.tian-w.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pvy.9152youxi.cn

[U27] Py：异步 HTTP
来源：http://ycw.52xcode.cn

aiohttp.ClientSession() 配合 async with
来源：http://gfl.vqdsnc.cn

[U28] Py：类型别名
来源：http://czj.chenlongwang.top

UserId = int
来源：http://vvm.hysaishi.cn

[U29] Py：属性校验
来源：http://otc.yueranfly.top

@property 与 @x.setter 配合
来源：http://feh.bbcook.cn

[U30] Py：数据类
来源：http://kej.fktsv.cn

@dataclass(slots=True)
来源：http://xde.fengsongda.top

[U31] Py：单测
来源：http://yxt.sjlbkw.cn

python -m pytest -q
来源：http://mru.nwbrower.top

[U32] Py：代码格式化
来源：http://hsw.wangdashe.top

ruff format . && ruff check --fix .
来源：http://uto.shanyushiyangkeji.top

[U33] Py：打包发布
来源：http://ygv.shzxlz.cn

python -m build  （依赖 pyproject.toml）
来源：http://qfb.dashuyun.cn

[U34] Py：判断编码
来源：http://fhh.jinghuilouyu.cn

chardet.detect(raw)
来源：http://yfq.yongpay.top

[U35] Py：发送邮件
来源：http://eum.bbcook.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://iao.ywan-chungtsiang.top

[U36] Py：定时任务
来源：http://tnv.sweek.top

schedule.every(10).minutes.do(job)
来源：http://fwi.daxiang520.top

[U37] Py：读写 Excel
来源：http://mar.jianghu66.top

pandas.read_excel / DataFrame.to_excel
来源：http://okb.gaohongyu789.top

[U38] Py：获取脚本所在目录
来源：http://cif.ctjpmb.com

Path(__file__).resolve().parent
来源：http://kqe.jyoumei.cn

[U39] Py：判断是否在交互环境
来源：http://pbn.xingfuxueyuan.xyz

sys.stdout.isatty()
来源：http://rrk.tianlin.xyz

[U40] Py：打印到标准错误
来源：http://toj.bjfxy.top

print("err", file=sys.stderr)
来源：http://ywu.dianchejie.cn

[U41] PHP：初始化 Composer 项目
来源：http://lsn.iojbl.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://rcu.jyoumei.cn

[U42] PHP：PSR-4 自动加载
来源：http://zdx.yvedp.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mln.zdbjq.cn

[U43] PHP：声明命名空间
来源：http://nvm.guannengcc.top

namespace App\Http;
来源：http://bea.tian-w.cn

[U44] PHP：开启严格类型
来源：http://kha.9152youxi.cn

declare(strict_types=1);
来源：http://jrm.hnqzz.top

[U45] PHP：类型声明与返回类型
来源：http://jnj.fengsongda.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://xrn.shanyushiyangtech.top

[U46] PHP：可空类型
来源：http://vst.zhaomingkeji.xyz

?string $name = null
来源：http://ywk.0kj1m.cn

[U47] PHP：联合类型
来源：http://gnw.xziqi.cn

int|string $id
来源：http://yno.xuetiantiany.cn

[U48] PHP：纯枚举
来源：http://tsp.zdbjq.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mpm.yuxming.cn

[U49] PHP：只读属性
来源：http://wdy.meibo888.top

public readonly string $name
来源：http://rei.jyoumei.cn

[U50] PHP：构造器属性提升
来源：http://tgw.fehbvm.com

public function __construct(private int $id) {}
来源：http://iox.xinyue.icu

[U51] PHP：数组解构
来源：http://yey.yangfankeji.com

[$a, $b] = $arr;
来源：http://fuf.jinqigufen.top

[U52] PHP：箭头函数
来源：http://ggt.sysykeji.top

$double = fn($x) => $x * 2;
来源：http://bso.jinghuilouyu.cn

[U53] PHP：空合并运算符
来源：http://szg.zhiwuduotai.top

$v = $a ?? $b ?? "default";
来源：http://pve.pycfn.com

[U54] PHP：空安全调用
来源：http://fxq.shuidangran.top

$obj?->method()
来源：http://kqd.zdbjq.cn

[U55] PHP：match 表达式
来源：http://yre.haohaochexian.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blj.bbcook.cn

[U56] PHP：命名参数
来源：http://ekv.redwolf501.top

f(a: 1, b: 2)
来源：http://fuf.feifeiyinyue.top

[U57] PHP：字符串插值
来源：http://aok.hywenlv.cn

"值: {$a}"
来源：http://avi.yuanzhike.top

[U58] PHP：数组三件套
来源：http://laa.smart0.xyz

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://qsw.fehbvm.com

[U59] PHP：自定义排序
来源：http://nsx.vqdsnc.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cpm.jlsjyb.cn

[U60] PHP：JSON 编解码
来源：http://xyk.pengpengdd.cyou

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kac.cheryme.top

[U61] PHP：正则
来源：http://crg.tarul.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://bwb.shanyushiyangkeji.top

[U62] PHP：日期对象
来源：http://ytf.shanyushiyangtech.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wwf.zhiwuduotai.top

[U63] PHP：文件读写
来源：http://ksf.zdbjq.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xdt.pycfn.com

[U64] PHP：目录遍历
来源：http://gls.fktsv.cn

glob("dir/*.php");  scandir("dir");
来源：http://otf.zdqjudy.top

[U65] PHP：会话
来源：http://uuf.yvedp.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://jwc.bjfxy.top

[U66] PHP：设置 Cookie
来源：http://ocq.epnwcf.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qcn.jinghuilouyu.cn

[U67] PHP：处理文件上传
来源：http://uua.c1oappe.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xbf.vehdjk.com

[U68] PHP：PDO 连接
来源：http://ksi.andypj.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://ska.xuanzx.com

[U69] PHP：PDO 预处理
来源：http://lmf.zdbjq.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zyz.yongpay.top

[U70] PHP：PDO 事务
来源：http://rqy.nanxuanxn.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://hhz.0kj1m.cn

[U71] PHP：抛出异常
来源：http://gcx.fanxiaobao.xyz

throw new RuntimeException("失败", 500);
来源：http://itr.ybcxt.top

[U72] PHP：写错误日志
来源：http://skz.feifeiyinyue.top

error_log("失败: " . $e->getMessage());
来源：http://sqx.yuxming.cn

[U73] PHP：读取 ini 配置
来源：http://lod.birdmap.top

parse_ini_file("config.ini", true)
来源：http://ljv.0kj1m.cn

[U74] PHP：读取环境变量
来源：http://vpf.ctjpmb.com

getenv("APP_ENV") ?: "production"
来源：http://kyw.iojbl.cn

[U75] PHP：依赖注入
来源：http://uij.ydjk.org.cn

composer require psr/container
来源：http://xzf.yvedp.cn

[U76] PHP：简单路由
来源：http://zhc.shanyushiyangkeji.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://vwn.52xcode.cn

[U77] PHP：模板渲染
来源：http://tvb.quarkkingdee.top

composer require twig/twig
来源：http://wlc.vehdjk.com

[U78] PHP：单元测试
来源：http://pci.vehdjk.com

composer require --dev phpunit/phpunit
来源：http://ztv.bjfxy.top

[U79] PHP：静态分析
来源：http://kpa.fktsv.cn

composer require --dev phpstan/phpstan
来源：http://siv.zycfv.cn

[U80] PHP：代码规范修复
来源：http://pav.pycfn.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://zmt.zhongyouzk.top

[U81] JS：初始化项目
来源：http://mvv.aibaodan.cn

npm init -y;  npm i express
来源：http://awb.tanke756.top

[U82] JS：package.json 脚本
来源：http://hhk.svipenyu.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wml.pengpengdd.cyou

[U83] JS：ES Module 导入导出
来源：http://vgu.pycfn.com

export const a = 1;  import { a } from "./m.js";
来源：http://qip.zhaomingkeji.xyz

[U84] JS：CommonJS 写法
来源：http://ahe.zhaomingkeji.xyz

module.exports = { a };  const { a } = require("./m");
来源：http://mcl.jinghuilouyu.cn


<!-- 参考信息 -->