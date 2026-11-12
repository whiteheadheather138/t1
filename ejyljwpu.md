代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rzi.jinyuanbaomall.cn

[S55] C++：结构化绑定
来源：http://eus.tanke756.top

auto [a, b] = std::make_pair(1, 2);
来源：http://vkn.tianlin.xyz

[S56] C++：optional
来源：http://fsa.tanke756.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://plq.jlsjyb.cn

[S57] C++：编译期常量
来源：http://rop.yuxming.cn

constexpr int N = 10;
来源：http://kfa.gotoacloud.top

[S58] C++：命名空间
来源：http://osp.jyoumei.cn

namespace ns { int f() { return 1; } }
来源：http://tuz.ydzc1.top

[S59] C++：静态断言
来源：http://biw.sweek.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://npn.ctjpmb.com

[S60] C++：遍历并删除元素
来源：http://pdy.ydzc1.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ykq.vehdjk.com

================================================================================
来源：http://qod.hcnkem.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ihm.cucudq.cn

================================================================================
来源：http://jxp.zhijiandao.cn

[T01] Kotlin：Hello World
来源：http://twu.gaohongyu789.top

println("Hello")
来源：http://mor.pengpengdd.cyou

[T02] Kotlin：变量
来源：http://rtt.zhixingplan.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rxm.fehbvm.com

[T03] Kotlin：字符串模板
来源：http://rht.uphjek.com

"值: $b"
来源：http://hog.zhoulong.xyz

[T04] Kotlin：空安全
来源：http://ezh.jqgufenzy.top

val n: String? = null;  n?.length
来源：http://kxd.yj202588.top

[T05] Kotlin：when 表达式
来源：http://zqq.zhixingplan.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kih.iojbl.cn

[T06] Kotlin：集合映射
来源：http://uuw.316326.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://mgj.ydzc1.top

[T07] Kotlin：集合过滤
来源：http://kyc.zhongyouzk.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://afe.0kj1m.cn

[T08] Kotlin：数据类
来源：http://yih.nanxuanxn.top

data class User(val name: String, val age: Int)
来源：http://ohv.cucudq.cn

[T09] Kotlin：扩展函数
来源：http://hjz.yuanzhike.top

fun String.exclaim() = this + "!"
来源：http://tyj.feifeiyinyue.top

[T10] Kotlin：默认参数
来源：http://pto.fengsongda.top

fun greet(name: String = "World") = "Hi $name"
来源：http://qsg.hnxiangtu.top

[T11] Kotlin：协程
来源：http://vtw.andypj.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://vdx.c1oappe.top

[T12] Kotlin：解构声明
来源：http://sse.jianghu66.top

val (a, b) = Pair(1, 2)
来源：http://vpn.zdbjq.cn

[T13] Kotlin：只读 Map
来源：http://uiz.kuanghao11.cn

val m = mapOf("a" to 1)
来源：http://tnu.zycfv.cn

[T14] Kotlin：循环
来源：http://mgx.tian-w.cn

for (i in 1..10) println(i)
来源：http://wnk.havefunace.top

[T15] Kotlin：接口
来源：http://grh.jqgufenzy.top

interface Shape { fun area(): Double }
来源：http://khw.smart0.xyz

[T16] Swift：Hello World
来源：http://thp.haohaochexian.top

print("Hello")
来源：http://rcg.fengsongda.top

[T17] Swift：变量与常量
来源：http://apk.fengsongda.top

var a = 1;  let b = 2
来源：http://ard.jqgufenzy.top

[T18] Swift：字符串插值
来源：http://sss.nanxuanxn.top

"值: \(b)"
来源：http://yya.9152youxi.cn

[T19] Swift：可选绑定
来源：http://pbj.bbcook.cn

if let n = opt { print(n) }
来源：http://qrk.cashguo.top

[T20] Swift：数组操作
来源：http://vyo.jinghuilouyu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://cnn.yongpay.top

[T21] Swift：遍历
来源：http://bvc.zdqjudy.top

for x in a { print(x) }
来源：http://edl.meibo888.top

[T22] Swift：字典
来源：http://lzn.c1oappe.top

var d = ["a": 1];  d["b"] = 2
来源：http://cls.gaohongyu789.top

[T23] Swift：函数
来源：http://sqg.xylfe.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ahs.haohaochexian.top

[T24] Swift：闭包
来源：http://xif.sysykeji.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://yxw.quarkkingdee.top

[T25] Swift：结构体
来源：http://ksx.zdbjq.cn

struct P { var x: Int }
来源：http://zxk.andypj.xyz

[T26] Swift：类与重写
来源：http://rwh.meibo888.top

class A: Base { override func f() {} }
来源：http://hle.yj20258.top

[T27] Swift：错误处理
来源：http://arm.yonumen.top

do { try f() } catch { print(error) }
来源：http://cda.svipenyu.cn

[T28] Swift：枚举
来源：http://boy.shanyushiyangkeji.top

enum Color { case red, green }
来源：http://uqg.zhaomingkeji.xyz

[T29] Swift：guard 提前返回
来源：http://rbz.cashguo.top

guard let x = opt else { return }
来源：http://ies.52xcode.cn

[T30] Swift：协议
来源：http://xnj.cashguo.top

protocol Shape { func area() -> Double }
来源：http://gtn.bbcook.cn

[T31] Lua：Hello World
来源：http://wyf.hysaishi.cn

print("Hello")
来源：http://uef.cashguo.top

[T32] Lua：局部变量
来源：http://uzn.fehbvm.com

local a = 1
来源：http://pfx.sysykeji.top

[T33] Lua：表（数组）
来源：http://dvz.hysaishi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://has.xingfuxueyuan.xyz

[T34] Lua：遍历表
来源：http://xzd.shangyingyoupin.top

for i, v in ipairs(t) do print(i, v) end
来源：http://cfu.dianchejie.cn

[T35] Lua：字典表
来源：http://wyp.redwolf501.top

local d = { a = 1 };  d.b = 2
来源：http://das.vehdjk.com

[T36] Lua：函数
来源：http://hid.zhongyouzk.top

function add(a, b) return a + b end
来源：http://kxs.fzhhl.top

[T37] Lua：字符串拼接
来源：http://fon.cheryme.top

"a" .. "b"
来源：http://rzw.nanxuanxn.top

[T38] Lua：条件
来源：http://ikk.jinqigufen.top

if x > 0 then print("正") end
来源：http://tia.cqqwz.cn

[T39] Lua：模式匹配
来源：http://sfz.daxiang520.top

string.find(s, "%d+")
来源：http://wvr.hnqzz.top

[T40] Lua：元表
来源：http://oeu.zhengqikj.top

setmetatable({}, { __index = base })
来源：http://rxt.yueranfly.top

[T41] Perl：Hello World
来源：http://mnm.cqqwz.cn

print "Hello\n";
来源：http://rue.uphjek.com

[T42] Perl：变量类型
来源：http://ueg.gzhubu.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jat.gzhubu.top

[T43] Perl：字符串插值
来源：http://odb.shzxlz.cn

"值: $a"
来源：http://suq.yongpay.top

[T44] Perl：条件
来源：http://qtx.ywan-chungtsiang.top

if ($a > 0) { print "正"; }
来源：http://sbs.wangshuangyany.cn

[T45] Perl：数组遍历
来源：http://wah.tian-w.cn

for my $x (@arr) { print $x; }
来源：http://mjb.jqgufenzy.top

[T46] Perl：哈希操作
来源：http://sbf.daria6918.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zlf.sysykeji.top

[T47] Perl：正则捕获
来源：http://hhd.hnqzz.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://wrj.havefunace.top

[T48] Perl：正则替换
来源：http://ieh.hysaishi.cn

$s =~ s/old/new/g;
来源：http://mlh.cucudq.cn

[T49] Perl：函数
来源：http://mdf.gzhubu.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dli.zhoulong.xyz

[T50] Perl：逐行读文件
来源：http://cwh.ctjpmb.com

open my $fh, "<", "a.txt" or die $!;
来源：http://nky.iojbl.cn

while (my $line = <$fh>) { print $line; }
来源：http://zia.9152youxi.cn

[T51] Scala：Hello World
来源：http://umv.yonumen.top

println("Hello")
来源：http://nrs.ivvv.top

[T52] Scala：变量
来源：http://rnq.wangshuangyany.cn

val a = 1;  var b = 2
来源：http://kza.epnwcf.com

[T53] Scala：字符串插值
来源：http://adm.daxiang520.top

s"值: $b"
来源：http://twx.quarkkingdee.top

[T54] Scala：集合映射
来源：http://gqe.hysaishi.cn

List(1, 2, 3).map(_ * 2)
来源：http://hjd.jqgufenzy.top

[T55] Scala：集合过滤
来源：http://ncj.gogol.net.cn

List(1, 2, 3).filter(_ > 1)
来源：http://fnl.gzhubu.top

[T56] Scala：样例类
来源：http://bxc.wangdashe.top

case class User(name: String, age: Int)
来源：http://yng.jinqigfzy.top

[T57] Scala：模式匹配
来源：http://dqi.yanxiufei.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://hvz.ydzc1.top

[T58] Scala：函数定义
来源：http://pyb.nwbrower.top

def add(a: Int, b: Int): Int = a + b
来源：http://kdt.iojbl.cn

[T59] Scala：循环
来源：http://khp.jinghuilouyu.cn

for (i <- 1 to 10) println(i)
来源：http://nkw.vqdsnc.cn

[T60] Scala：折叠
来源：http://ype.zhongyouzk.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cwz.yuanzhike.top

================================================================================
来源：http://fic.mhx1999.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://caj.hnxiangtu.top

================================================================================
来源：http://opf.yj20258888.top

[U01] Py：创建虚拟环境
来源：http://rmd.jinyuanbaomall.cn

python -m venv .venv && source .venv/bin/activate
来源：http://fta.chenjidiqi.icu

[U02] Py：导出 / 安装依赖
来源：http://tgd.hywenlv.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zeq.jinqigufen.top

[U03] Py：加载 .env 配置
来源：http://hrx.epnwcf.com

from dotenv import load_dotenv; load_dotenv()
来源：http://vkv.jqgfzy.top

[U04] Py：变量调试打印
来源：http://wrz.gotoacloud.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fqy.c1oappe.top

[U05] Py：列表去重且保序
来源：http://qci.fehbvm.com

list(dict.fromkeys(arr))
来源：http://dav.svipenyu.cn

[U06] Py：合并两个字典
来源：http://gji.fzhhl.top

{**a, **b}
来源：http://jjv.pycfn.com

[U07] Py：反转字典键值
来源：http://led.shangyingyoupin.top

{v: k for k, v in d.items()}
来源：http://web.sweek.top

[U08] Py：展平二维列表
来源：http://bfg.sweek.top

[y for x in nested for y in x]
来源：http://iyf.zhaomingkeji.xyz

[U09] Py：字典取最大值的键
来源：http://fcn.epnwcf.com

max(d, key=d.get)
来源：http://bqb.hongshengwenyu.top

[U10] Py：按值排序字典
来源：http://lqv.ydjk.org.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xfr.dianchejie.cn

[U11] Py：生成器表达式
来源：http://wyz.52xcode.cn

(x * 2 for x in arr)
来源：http://grl.zhongyouzk.top

[U12] Py：取出现最多的 3 个元素
来源：http://rhx.sjlbkw.cn

Counter(arr).most_common(3)
来源：http://etg.birdmap.top

[U13] Py：固定长度队列
来源：http://rmg.gotoacloud.top

deque(maxlen=10)
来源：http://ywl.gotoacloud.top

[U14] Py：分组收集到列表
来源：http://asl.ywan-chungtsiang.top

defaultdict(list)
来源：http://dic.hesvh.cn

[U15] Py：高精度计时
来源：http://qce.gotoacloud.top

t = time.perf_counter()
来源：http://jfx.zdbjq.cn

[U16] Py：命令行参数解析
来源：http://ovg.fehbvm.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://otv.svipenyu.cn

[U17] Py：初始化日志
来源：http://xpa.jiagoushi.top

logging.basicConfig(level=logging.INFO)
来源：http://hqn.jinqigfzy.top

[U18] Py：预编译正则
来源：http://rmb.daria6918.cn

pat = re.compile(r"\d+")
来源：http://rct.cashguo.top

[U19] Py：正则替换带回调
来源：http://nqb.jinyuanbaomall.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zjy.havefunace.top

[U20] Py：缓存函数结果
来源：http://chm.shuidangran.top

@functools.lru_cache(maxsize=None)
来源：http://ljk.guowangkeji.top

[U21] Py：自定义上下文管理器
来源：http://abo.gzhubu.top

@contextlib.contextmanager
来源：http://hit.zhiwuduotai.top

[U22] Py：矩阵转置
来源：http://unx.hongshengwenyu.top

list(zip(*m))
来源：http://adq.jinqigfzy.top

[U23] Py：分块读取大文件
来源：http://stf.quarkkingdee.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://wnf.yuanzhike.top

[U24] Py：路径操作
来源：http://haz.shanyushiyangtech.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qxd.jianghu66.top

[U25] Py：CSV 按字典读
来源：http://pql.nwbrower.top

csv.DictReader(f)
来源：http://tdn.jinyuanbaomall.cn

[U26] Py：并发下载
来源：http://jdm.zhijiandao.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mnu.smart0.xyz

[U27] Py：异步 HTTP
来源：http://yur.chenjidiqi.icu

aiohttp.ClientSession() 配合 async with
来源：http://bza.bjfxy.top

[U28] Py：类型别名
来源：http://tsh.316326.xyz

UserId = int
来源：http://dha.hywenlv.cn

[U29] Py：属性校验
来源：http://pgf.hnqzz.top

@property 与 @x.setter 配合
来源：http://hyi.jiagoushi.top

[U30] Py：数据类
来源：http://oqq.c1oappe.top

@dataclass(slots=True)
来源：http://mha.yonumen.top

[U31] Py：单测
来源：http://fxa.tarul.cn

python -m pytest -q
来源：http://bac.wangdashe.top

[U32] Py：代码格式化
来源：http://xoo.feifeiyinyue.top

ruff format . && ruff check --fix .
来源：http://dgy.zhengqikj.top

[U33] Py：打包发布
来源：http://jrj.dianchejie.cn

python -m build  （依赖 pyproject.toml）
来源：http://uis.yueranfly.top

[U34] Py：判断编码
来源：http://eof.smart0.xyz

chardet.detect(raw)
来源：http://zyy.yangfankeji.com

[U35] Py：发送邮件
来源：http://ija.jianghu66.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ovm.chenzaomai.com

[U36] Py：定时任务
来源：http://pjq.zdqjudy.top

schedule.every(10).minutes.do(job)
来源：http://aml.shzxlz.cn

[U37] Py：读写 Excel
来源：http://pee.vehdjk.com

pandas.read_excel / DataFrame.to_excel
来源：http://lik.ywan-chungtsiang.top

[U38] Py：获取脚本所在目录
来源：http://yay.epnwcf.com

Path(__file__).resolve().parent
来源：http://fzx.redwolf501.top

[U39] Py：判断是否在交互环境
来源：http://ida.chenlongwang.top

sys.stdout.isatty()
来源：http://lir.ivvv.top

[U40] Py：打印到标准错误
来源：http://hln.hongshengwenyu.top

print("err", file=sys.stderr)
来源：http://jwd.bjfxy.top

[U41] PHP：初始化 Composer 项目
来源：http://ebl.guannengcc.top

composer init;  composer require guzzlehttp/guzzle
来源：http://eva.nanxinkj.top

[U42] PHP：PSR-4 自动加载
来源：http://zrk.ydzc1.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://twf.shuidangran.top

[U43] PHP：声明命名空间
来源：http://uur.epnwcf.com

namespace App\Http;
来源：http://dco.hywenlv.cn

[U44] PHP：开启严格类型
来源：http://luw.jinqigufen.top

declare(strict_types=1);
来源：http://kqs.gogol.net.cn

[U45] PHP：类型声明与返回类型
来源：http://ckw.jinqigfzy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://zng.xuetiantiany.cn

[U46] PHP：可空类型
来源：http://aaq.cucudq.cn

?string $name = null
来源：http://lwf.pycfn.com

[U47] PHP：联合类型
来源：http://vxc.aibaodan.cn

int|string $id
来源：http://ols.jinghuilouyu.cn

[U48] PHP：纯枚举
来源：http://mxp.ivvv.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cbq.vehdjk.com

[U49] PHP：只读属性
来源：http://ruf.0kj1m.cn

public readonly string $name
来源：http://dpf.sjlbkw.cn

[U50] PHP：构造器属性提升
来源：http://chf.meibo888.top

public function __construct(private int $id) {}
来源：http://icl.ehwqpu.com

[U51] PHP：数组解构
来源：http://ewu.xingfuxueyuan.xyz

[$a, $b] = $arr;
来源：http://pls.ppjwa.cn

[U52] PHP：箭头函数
来源：http://ozr.pycfn.com

$double = fn($x) => $x * 2;
来源：http://dxw.yuanzhike.top

[U53] PHP：空合并运算符
来源：http://xkz.zhiwuduotai.top

$v = $a ?? $b ?? "default";
来源：http://pvz.zhongyouzk.top

[U54] PHP：空安全调用
来源：http://elu.zdbjq.cn

$obj?->method()
来源：http://nmz.yj202588.top

[U55] PHP：match 表达式
来源：http://sob.yuanzhike.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://mpj.yueranfly.top

[U56] PHP：命名参数
来源：http://vuh.vehdjk.com

f(a: 1, b: 2)
来源：http://oyj.dashuyun.cn

[U57] PHP：字符串插值
来源：http://jyy.redwolf501.top

"值: {$a}"
来源：http://wcf.jyoumei.cn

[U58] PHP：数组三件套
来源：http://gmp.zhixingplan.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://rya.epnwcf.com

[U59] PHP：自定义排序
来源：http://tnn.zycfv.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://myt.cqqwz.cn

[U60] PHP：JSON 编解码
来源：http://kqv.havefunace.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ptz.andypj.xyz

[U61] PHP：正则
来源：http://tqu.smart0.xyz

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qwm.tanke756.top

[U62] PHP：日期对象
来源：http://jcw.snrcjt.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://zqo.tarul.cn

[U63] PHP：文件读写
来源：http://yjn.sxryk.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://utj.hongshengwenyu.top

[U64] PHP：目录遍历
来源：http://uhd.sjlbkw.cn

glob("dir/*.php");  scandir("dir");
来源：http://jyo.zdqjudy.top

[U65] PHP：会话
来源：http://evu.cheryme.top

session_start();  $_SESSION["uid"] = 1;
来源：http://fne.hcnkem.com

[U66] PHP：设置 Cookie
来源：http://wss.quarkkingdee.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vhi.zycfv.cn

[U67] PHP：处理文件上传
来源：http://ysc.zhaomingkeji.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://itl.jinqigfzy.top

[U68] PHP：PDO 连接
来源：http://pif.shanyushiyangtech.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://rps.tianlin.xyz

[U69] PHP：PDO 预处理
来源：http://uwj.jlsjyb.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://une.yfazqb.com

[U70] PHP：PDO 事务
来源：http://bdm.snrcjt.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xui.uphjek.com

[U71] PHP：抛出异常
来源：http://xlk.jiagoushi.top

throw new RuntimeException("失败", 500);
来源：http://tpn.zhiwuduotai.top

[U72] PHP：写错误日志
来源：http://qzf.52xcode.cn

error_log("失败: " . $e->getMessage());
来源：http://bfw.ydjk.org.cn

[U73] PHP：读取 ini 配置
来源：http://xxs.cucudq.cn

parse_ini_file("config.ini", true)
来源：http://lfg.epnwcf.com

[U74] PHP：读取环境变量
来源：http://lvn.yanxiufei.cn

getenv("APP_ENV") ?: "production"
来源：http://bap.epnwcf.com

[U75] PHP：依赖注入
来源：http://hyt.yj20258.top

composer require psr/container
来源：http://vcf.zhongyouzk.top

[U76] PHP：简单路由
来源：http://wzq.ppjwa.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://fdi.hammf.cn

[U77] PHP：模板渲染
来源：http://hvz.quarkkingdee.top

composer require twig/twig
来源：http://xjr.cheryme.top

[U78] PHP：单元测试
来源：http://sfh.svipenyu.cn

composer require --dev phpunit/phpunit
来源：http://ywz.smart0.xyz

[U79] PHP：静态分析
来源：http://yoo.shangyingyoupin.top

composer require --dev phpstan/phpstan
来源：http://lzx.feifeiyinyue.top

[U80] PHP：代码规范修复
来源：http://lzr.yonumen.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://iym.yangfankeji.com


<!-- 参考信息 -->