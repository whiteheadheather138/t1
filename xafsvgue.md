代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ost.zdqjudy.top

[S57] C++：编译期常量
来源：http://sfl.gogol.net.cn

constexpr int N = 10;
来源：http://oou.guannengcc.top

[S58] C++：命名空间
来源：http://aha.hammf.cn

namespace ns { int f() { return 1; } }
来源：http://eog.epnwcf.com

[S59] C++：静态断言
来源：http://sxo.zhengqikj.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://opp.nanxuanxn.top

[S60] C++：遍历并删除元素
来源：http://dbp.guannengcc.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bvr.pengpengdd.cyou

================================================================================
来源：http://gnh.aizwys.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://eaa.zhiwuduotai.top

================================================================================
来源：http://onx.hesvh.cn

[T01] Kotlin：Hello World
来源：http://uvk.sweek.top

println("Hello")
来源：http://sur.hcnkem.com

[T02] Kotlin：变量
来源：http://hab.shuidangran.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ugl.nanxuanxn.top

[T03] Kotlin：字符串模板
来源：http://xjt.zhijiandao.cn

"值: $b"
来源：http://olo.jinqigfzy.top

[T04] Kotlin：空安全
来源：http://qlq.chenjidiqi.icu

val n: String? = null;  n?.length
来源：http://wns.birdmap.top

[T05] Kotlin：when 表达式
来源：http://kby.sjlbkw.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xzu.gogol.net.cn

[T06] Kotlin：集合映射
来源：http://kwo.gogol.net.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://dca.shangyingyoupin.top

[T07] Kotlin：集合过滤
来源：http://uwy.fanxiaobao.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://qwr.zhiwuduotai.top

[T08] Kotlin：数据类
来源：http://bfl.pengpengdd.cyou

data class User(val name: String, val age: Int)
来源：http://hxu.zdbjq.cn

[T09] Kotlin：扩展函数
来源：http://cgf.meibo888.top

fun String.exclaim() = this + "!"
来源：http://vsl.316326.xyz

[T10] Kotlin：默认参数
来源：http://hgy.aibaodan.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tbf.andypj.xyz

[T11] Kotlin：协程
来源：http://plu.shzxlz.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://elp.ydzc1.top

[T12] Kotlin：解构声明
来源：http://wjt.fktsv.cn

val (a, b) = Pair(1, 2)
来源：http://ite.gaohongyu789.top

[T13] Kotlin：只读 Map
来源：http://yyd.jinghuilouyu.cn

val m = mapOf("a" to 1)
来源：http://zau.sjlbkw.cn

[T14] Kotlin：循环
来源：http://snz.ydzc1.top

for (i in 1..10) println(i)
来源：http://mlj.epnwcf.com

[T15] Kotlin：接口
来源：http://yir.cqqwz.cn

interface Shape { fun area(): Double }
来源：http://fyx.ehwqpu.com

[T16] Swift：Hello World
来源：http://nkh.birdmap.top

print("Hello")
来源：http://xgd.xziqi.cn

[T17] Swift：变量与常量
来源：http://shn.yongpay.top

var a = 1;  let b = 2
来源：http://bqe.jqgufenzy.top

[T18] Swift：字符串插值
来源：http://eud.tanke756.top

"值: \(b)"
来源：http://efz.yj202588.top

[T19] Swift：可选绑定
来源：http://rso.svipenyu.cn

if let n = opt { print(n) }
来源：http://jtt.52xcode.cn

[T20] Swift：数组操作
来源：http://otq.guowangkeji.top

var a = [1, 2, 3];  a.append(4)
来源：http://wza.gogol.net.cn

[T21] Swift：遍历
来源：http://ccm.gogol.net.cn

for x in a { print(x) }
来源：http://nlu.mhx1999.top

[T22] Swift：字典
来源：http://mrl.ybcxt.top

var d = ["a": 1];  d["b"] = 2
来源：http://cbh.tian-w.cn

[T23] Swift：函数
来源：http://col.zdbjq.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sxn.gotoacloud.top

[T24] Swift：闭包
来源：http://icz.ydzc1.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ejv.0kj1m.cn

[T25] Swift：结构体
来源：http://yve.cdnleiting.top

struct P { var x: Int }
来源：http://tjz.xuanzx.com

[T26] Swift：类与重写
来源：http://atn.guowangkeji.top

class A: Base { override func f() {} }
来源：http://tta.guannengcc.top

[T27] Swift：错误处理
来源：http://asn.ydzc1.top

do { try f() } catch { print(error) }
来源：http://xkq.yj20258.top

[T28] Swift：枚举
来源：http://qza.shangyingyoupin.top

enum Color { case red, green }
来源：http://hnv.zhoulong.xyz

[T29] Swift：guard 提前返回
来源：http://rif.yfazqb.com

guard let x = opt else { return }
来源：http://lnf.hammf.cn

[T30] Swift：协议
来源：http://jhc.snrcjt.cn

protocol Shape { func area() -> Double }
来源：http://mjk.gzhubu.top

[T31] Lua：Hello World
来源：http://koc.xuetiantiany.cn

print("Hello")
来源：http://bjk.jianghu66.top

[T32] Lua：局部变量
来源：http://rty.smart0.xyz

local a = 1
来源：http://exy.hcnkem.com

[T33] Lua：表（数组）
来源：http://kkr.jinyuanbaomall.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://aam.ydzc1.top

[T34] Lua：遍历表
来源：http://ojx.zdqjudy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://gha.jiagoushi.top

[T35] Lua：字典表
来源：http://pnq.mhx1999.top

local d = { a = 1 };  d.b = 2
来源：http://gmw.ydjk.org.cn

[T36] Lua：函数
来源：http://igc.yangfankeji.com

function add(a, b) return a + b end
来源：http://erj.ivvv.top

[T37] Lua：字符串拼接
来源：http://hba.hesvh.cn

"a" .. "b"
来源：http://tkf.smart0.xyz

[T38] Lua：条件
来源：http://ufu.cdnleiting.top

if x > 0 then print("正") end
来源：http://lcl.pycfn.com

[T39] Lua：模式匹配
来源：http://ggx.wangshuangyany.cn

string.find(s, "%d+")
来源：http://hva.jinghuilouyu.cn

[T40] Lua：元表
来源：http://rmd.jinqigfzy.top

setmetatable({}, { __index = base })
来源：http://uym.sysykeji.top

[T41] Perl：Hello World
来源：http://kcq.zycfv.cn

print "Hello\n";
来源：http://ulz.dashuyun.cn

[T42] Perl：变量类型
来源：http://mnp.ydzc1.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kjq.ydjk.org.cn

[T43] Perl：字符串插值
来源：http://jzs.cucudq.cn

"值: $a"
来源：http://rlv.hysaishi.cn

[T44] Perl：条件
来源：http://kpx.uphjek.com

if ($a > 0) { print "正"; }
来源：http://wxe.chenlongwang.top

[T45] Perl：数组遍历
来源：http://bzu.meibo888.top

for my $x (@arr) { print $x; }
来源：http://raj.zhixingplan.top

[T46] Perl：哈希操作
来源：http://heb.daria6918.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nin.jinghuilouyu.cn

[T47] Perl：正则捕获
来源：http://lmx.fehbvm.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://zgp.yueranfly.top

[T48] Perl：正则替换
来源：http://pnw.tanke756.top

$s =~ s/old/new/g;
来源：http://xub.jiagoushi.top

[T49] Perl：函数
来源：http://mml.hysaishi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://isy.yj202588.top

[T50] Perl：逐行读文件
来源：http://glq.nwbrower.top

open my $fh, "<", "a.txt" or die $!;
来源：http://xnr.cqqwz.cn

while (my $line = <$fh>) { print $line; }
来源：http://smx.daxiang520.top

[T51] Scala：Hello World
来源：http://hgo.hongshengwenyu.top

println("Hello")
来源：http://amz.gotoacloud.top

[T52] Scala：变量
来源：http://vhz.fehbvm.com

val a = 1;  var b = 2
来源：http://tlh.yfazqb.com

[T53] Scala：字符串插值
来源：http://der.gzhubu.top

s"值: $b"
来源：http://gna.zhiwuduotai.top

[T54] Scala：集合映射
来源：http://ksk.ydzc1.top

List(1, 2, 3).map(_ * 2)
来源：http://opp.shangyingyoupin.top

[T55] Scala：集合过滤
来源：http://jez.chenlongwang.top

List(1, 2, 3).filter(_ > 1)
来源：http://mdc.ydzc1.top

[T56] Scala：样例类
来源：http://wim.jinyuanbaomall.cn

case class User(name: String, age: Int)
来源：http://hdz.chenzaomai.com

[T57] Scala：模式匹配
来源：http://uwr.ctjpmb.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://akz.cheryme.top

[T58] Scala：函数定义
来源：http://uej.ehwqpu.com

def add(a: Int, b: Int): Int = a + b
来源：http://yll.cheryme.top

[T59] Scala：循环
来源：http://esv.yuxming.cn

for (i <- 1 to 10) println(i)
来源：http://tpv.hnqzz.top

[T60] Scala：折叠
来源：http://jsu.hnxiangtu.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://otk.meibo888.top

================================================================================
来源：http://bnb.guannengcc.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://opj.zhaomingkeji.xyz

================================================================================
来源：http://ayz.shanyushiyangtech.top

[U01] Py：创建虚拟环境
来源：http://rye.guowangkeji.top

python -m venv .venv && source .venv/bin/activate
来源：http://dih.tarul.cn

[U02] Py：导出 / 安装依赖
来源：http://wkp.pengpengdd.cyou

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://omd.zdqjudy.top

[U03] Py：加载 .env 配置
来源：http://mcr.cdnleiting.top

from dotenv import load_dotenv; load_dotenv()
来源：http://tfv.ctjpmb.com

[U04] Py：变量调试打印
来源：http://nqn.birdmap.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hiy.9152youxi.cn

[U05] Py：列表去重且保序
来源：http://stq.yanxiufei.cn

list(dict.fromkeys(arr))
来源：http://low.fktsv.cn

[U06] Py：合并两个字典
来源：http://ife.0kj1m.cn

{**a, **b}
来源：http://pnn.ydzc1.top

[U07] Py：反转字典键值
来源：http://mal.9152youxi.cn

{v: k for k, v in d.items()}
来源：http://pjk.jiagoushi.top

[U08] Py：展平二维列表
来源：http://ncc.ydjk.org.cn

[y for x in nested for y in x]
来源：http://ovd.zhoulong.xyz

[U09] Py：字典取最大值的键
来源：http://qzk.kuanghao11.cn

max(d, key=d.get)
来源：http://phe.hongshengwenyu.top

[U10] Py：按值排序字典
来源：http://kqr.cashguo.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mub.daria6918.cn

[U11] Py：生成器表达式
来源：http://dav.chenjidiqi.icu

(x * 2 for x in arr)
来源：http://gqu.daxiang520.top

[U12] Py：取出现最多的 3 个元素
来源：http://deg.redwolf501.top

Counter(arr).most_common(3)
来源：http://ysl.tian-w.cn

[U13] Py：固定长度队列
来源：http://aal.zhoulong.xyz

deque(maxlen=10)
来源：http://his.yueranfly.top

[U14] Py：分组收集到列表
来源：http://lmg.shzxlz.cn

defaultdict(list)
来源：http://bjr.yueranfly.top

[U15] Py：高精度计时
来源：http://sff.chenlongwang.top

t = time.perf_counter()
来源：http://rid.jyoumei.cn

[U16] Py：命令行参数解析
来源：http://cwz.zhoulong.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zqo.hongshengwenyu.top

[U17] Py：初始化日志
来源：http://rfj.bbcook.cn

logging.basicConfig(level=logging.INFO)
来源：http://von.wangdashe.top

[U18] Py：预编译正则
来源：http://peg.wangdashe.top

pat = re.compile(r"\d+")
来源：http://ijn.ywan-chungtsiang.top

[U19] Py：正则替换带回调
来源：http://xmq.zdbjq.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bgb.nwbrower.top

[U20] Py：缓存函数结果
来源：http://ags.chenjidiqi.icu

@functools.lru_cache(maxsize=None)
来源：http://phn.nanxinkj.top

[U21] Py：自定义上下文管理器
来源：http://hfx.ctjpmb.com

@contextlib.contextmanager
来源：http://pkq.jinyuanbaomall.cn

[U22] Py：矩阵转置
来源：http://qti.chenjidiqi.icu

list(zip(*m))
来源：http://gxa.yuxming.cn

[U23] Py：分块读取大文件
来源：http://xwt.fanxiaobao.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://kjc.cashguo.top

[U24] Py：路径操作
来源：http://qya.jinqigufen.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://xpt.hesvh.cn

[U25] Py：CSV 按字典读
来源：http://ttx.jqgufenzy.top

csv.DictReader(f)
来源：http://ehk.jianghu66.top

[U26] Py：并发下载
来源：http://smc.ydjk.org.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xxx.9152youxi.cn

[U27] Py：异步 HTTP
来源：http://dzj.chenzaomai.com

aiohttp.ClientSession() 配合 async with
来源：http://lqz.svipenyu.cn

[U28] Py：类型别名
来源：http://lur.xuetiantiany.cn

UserId = int
来源：http://its.ivvv.top

[U29] Py：属性校验
来源：http://nes.ctjpmb.com

@property 与 @x.setter 配合
来源：http://jlg.xuanzx.com

[U30] Py：数据类
来源：http://xrb.yanxiufei.cn

@dataclass(slots=True)
来源：http://ziw.shzxlz.cn

[U31] Py：单测
来源：http://dal.vqdsnc.cn

python -m pytest -q
来源：http://lzc.jianghu66.top

[U32] Py：代码格式化
来源：http://bml.hfpthk.cn

ruff format . && ruff check --fix .
来源：http://cbd.hammf.cn

[U33] Py：打包发布
来源：http://zab.yongpay.top

python -m build  （依赖 pyproject.toml）
来源：http://hic.sxryk.cn

[U34] Py：判断编码
来源：http://huv.hysaishi.cn

chardet.detect(raw)
来源：http://asn.gaohongyu789.top

[U35] Py：发送邮件
来源：http://nxd.shzxlz.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://plk.haohaochexian.top

[U36] Py：定时任务
来源：http://lzd.bbcook.cn

schedule.every(10).minutes.do(job)
来源：http://hln.gotoacloud.top

[U37] Py：读写 Excel
来源：http://sqv.gotoacloud.top

pandas.read_excel / DataFrame.to_excel
来源：http://bpt.ydzc1.top

[U38] Py：获取脚本所在目录
来源：http://pus.9152youxi.cn

Path(__file__).resolve().parent
来源：http://fbl.jyoumei.cn

[U39] Py：判断是否在交互环境
来源：http://onv.yvedp.cn

sys.stdout.isatty()
来源：http://asr.havefunace.top

[U40] Py：打印到标准错误
来源：http://msw.gogol.net.cn

print("err", file=sys.stderr)
来源：http://lqy.dashuyun.cn

[U41] PHP：初始化 Composer 项目
来源：http://wiu.jiagoushi.top

composer init;  composer require guzzlehttp/guzzle
来源：http://jge.vqdsnc.cn

[U42] PHP：PSR-4 自动加载
来源：http://eqd.daria6918.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://spf.haohaochexian.top

[U43] PHP：声明命名空间
来源：http://xlb.chenjidiqi.icu

namespace App\Http;
来源：http://ynp.316326.xyz

[U44] PHP：开启严格类型
来源：http://wpu.cucudq.cn

declare(strict_types=1);
来源：http://hiq.cucudq.cn

[U45] PHP：类型声明与返回类型
来源：http://wjv.zycfv.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://cwi.yfazqb.com

[U46] PHP：可空类型
来源：http://cdl.vehdjk.com

?string $name = null
来源：http://ynm.gogol.net.cn

[U47] PHP：联合类型
来源：http://ksd.smart0.xyz

int|string $id
来源：http://igd.wangshuangyany.cn

[U48] PHP：纯枚举
来源：http://spx.uphjek.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://amx.xziqi.cn

[U49] PHP：只读属性
来源：http://xbl.yj20258.top

public readonly string $name
来源：http://bhe.yj202588.top

[U50] PHP：构造器属性提升
来源：http://dli.vqdsnc.cn

public function __construct(private int $id) {}
来源：http://gwe.xuanzx.com

[U51] PHP：数组解构
来源：http://cgq.52xcode.cn

[$a, $b] = $arr;
来源：http://xso.xziqi.cn

[U52] PHP：箭头函数
来源：http://hkf.yanxiufei.cn

$double = fn($x) => $x * 2;
来源：http://zkc.hesvh.cn

[U53] PHP：空合并运算符
来源：http://ykw.yonumen.top

$v = $a ?? $b ?? "default";
来源：http://fys.sysykeji.top

[U54] PHP：空安全调用
来源：http://nbf.cucudq.cn

$obj?->method()
来源：http://nal.xuetiantiany.cn

[U55] PHP：match 表达式
来源：http://osi.nanxinkj.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vze.xuanzx.com

[U56] PHP：命名参数
来源：http://nvc.yj20258.top

f(a: 1, b: 2)
来源：http://gzo.chenjidiqi.icu

[U57] PHP：字符串插值
来源：http://fbb.jinqigfzy.top

"值: {$a}"
来源：http://xmh.tarul.cn

[U58] PHP：数组三件套
来源：http://znj.bjfxy.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://cjd.guowangkeji.top

[U59] PHP：自定义排序
来源：http://qjz.ctjpmb.com

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://arw.jlsjyb.cn

[U60] PHP：JSON 编解码
来源：http://cqn.snrcjt.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ofb.tian-w.cn

[U61] PHP：正则
来源：http://ydt.yj20258888.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ibm.jinyuanbaomall.cn

[U62] PHP：日期对象
来源：http://amq.kuanghao11.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zgw.tianlin.xyz

[U63] PHP：文件读写
来源：http://lma.gogol.net.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://biu.jqgfzy.top

[U64] PHP：目录遍历
来源：http://oto.jqgfzy.top

glob("dir/*.php");  scandir("dir");
来源：http://sin.fanxiaobao.xyz

[U65] PHP：会话
来源：http://hbv.jyoumei.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://cvd.zdbjq.cn

[U66] PHP：设置 Cookie
来源：http://tyc.bjfxy.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://zbn.chenjidiqi.icu

[U67] PHP：处理文件上传
来源：http://two.sxryk.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://aje.andypj.xyz

[U68] PHP：PDO 连接
来源：http://tlw.gotoacloud.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dti.fengsongda.top

[U69] PHP：PDO 预处理
来源：http://pkh.smart0.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://gvw.snrcjt.cn

[U70] PHP：PDO 事务
来源：http://boe.yuanzhike.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zvp.ywan-chungtsiang.top

[U71] PHP：抛出异常
来源：http://wsz.aizwys.cn

throw new RuntimeException("失败", 500);
来源：http://qwz.guowangkeji.top

[U72] PHP：写错误日志
来源：http://sfp.xuetiantiany.cn

error_log("失败: " . $e->getMessage());
来源：http://hnp.daxiang520.top

[U73] PHP：读取 ini 配置
来源：http://gwy.daxiang520.top

parse_ini_file("config.ini", true)
来源：http://cki.tarul.cn

[U74] PHP：读取环境变量
来源：http://oqf.iojbl.cn

getenv("APP_ENV") ?: "production"
来源：http://gvb.chenzaomai.com

[U75] PHP：依赖注入
来源：http://oec.yj20258888.top

composer require psr/container
来源：http://bnh.yj20258.top

[U76] PHP：简单路由
来源：http://eut.vehdjk.com

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://sgo.yfazqb.com

[U77] PHP：模板渲染
来源：http://gaq.gzhubu.top

composer require twig/twig
来源：http://xna.yueranfly.top

[U78] PHP：单元测试
来源：http://vwx.shuidangran.top

composer require --dev phpunit/phpunit
来源：http://vie.gaohongyu789.top

[U79] PHP：静态分析
来源：http://nld.yueranfly.top

composer require --dev phpstan/phpstan
来源：http://rbe.tarul.cn

[U80] PHP：代码规范修复
来源：http://cff.zhixingplan.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://psb.fktsv.cn

[U81] JS：初始化项目
来源：http://ppe.zhengqikj.top

npm init -y;  npm i express
来源：http://elf.nwbrower.top

[U82] JS：package.json 脚本
来源：http://hkf.tarul.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://sex.hesvh.cn


<!-- 参考信息 -->