代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hgb.guannengcc.top

[S57] C++：编译期常量
来源：http://tbe.fktsv.cn

constexpr int N = 10;
来源：http://pxr.zdbjq.cn

[S58] C++：命名空间
来源：http://gvt.gotoacloud.top

namespace ns { int f() { return 1; } }
来源：http://ngw.chenlongwang.top

[S59] C++：静态断言
来源：http://fxo.yj20258888.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://oko.daria6918.cn

[S60] C++：遍历并删除元素
来源：http://afo.yvedp.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dxw.zhoulong.xyz

================================================================================
来源：http://zsv.hammf.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://emh.cqqwz.cn

================================================================================
来源：http://dnh.gaohongyu789.top

[T01] Kotlin：Hello World
来源：http://qpy.0kj1m.cn

println("Hello")
来源：http://pam.snrcjt.cn

[T02] Kotlin：变量
来源：http://gsv.nwbrower.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xlo.ydjk.org.cn

[T03] Kotlin：字符串模板
来源：http://zpq.fzhhl.top

"值: $b"
来源：http://kiu.daxiang520.top

[T04] Kotlin：空安全
来源：http://gco.jiagoushi.top

val n: String? = null;  n?.length
来源：http://fbv.jinghuilouyu.cn

[T05] Kotlin：when 表达式
来源：http://pcv.zdbjq.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ieu.hesvh.cn

[T06] Kotlin：集合映射
来源：http://kuh.fanxiaobao.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://qxr.fengsongda.top

[T07] Kotlin：集合过滤
来源：http://twg.xziqi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wnw.yuxming.cn

[T08] Kotlin：数据类
来源：http://tcl.hongshengwenyu.top

data class User(val name: String, val age: Int)
来源：http://zvl.hywenlv.cn

[T09] Kotlin：扩展函数
来源：http://gbb.yangfankeji.com

fun String.exclaim() = this + "!"
来源：http://ops.tarul.cn

[T10] Kotlin：默认参数
来源：http://uhd.cdnleiting.top

fun greet(name: String = "World") = "Hi $name"
来源：http://lgc.9152youxi.cn

[T11] Kotlin：协程
来源：http://ivn.daria6918.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://gtd.xinyue.icu

[T12] Kotlin：解构声明
来源：http://czv.yueranfly.top

val (a, b) = Pair(1, 2)
来源：http://kpb.xingfuxueyuan.xyz

[T13] Kotlin：只读 Map
来源：http://izk.jinqigfzy.top

val m = mapOf("a" to 1)
来源：http://hvc.yanxiufei.cn

[T14] Kotlin：循环
来源：http://jfs.xinyue.icu

for (i in 1..10) println(i)
来源：http://jks.zhoulong.xyz

[T15] Kotlin：接口
来源：http://rtm.cdnleiting.top

interface Shape { fun area(): Double }
来源：http://uut.yanxiufei.cn

[T16] Swift：Hello World
来源：http://ldv.chenjidiqi.icu

print("Hello")
来源：http://jgt.yj20258888.top

[T17] Swift：变量与常量
来源：http://klo.iojbl.cn

var a = 1;  let b = 2
来源：http://zeu.zhongyouzk.top

[T18] Swift：字符串插值
来源：http://ocw.cucudq.cn

"值: \(b)"
来源：http://goq.hesvh.cn

[T19] Swift：可选绑定
来源：http://jwf.fktsv.cn

if let n = opt { print(n) }
来源：http://qxd.gaohongyu789.top

[T20] Swift：数组操作
来源：http://rhx.cucudq.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jjr.xuetiantiany.cn

[T21] Swift：遍历
来源：http://vcy.shzxlz.cn

for x in a { print(x) }
来源：http://inw.zdbjq.cn

[T22] Swift：字典
来源：http://awo.gotoacloud.top

var d = ["a": 1];  d["b"] = 2
来源：http://zuo.yuanzhike.top

[T23] Swift：函数
来源：http://fam.jyoumei.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mco.jianghu66.top

[T24] Swift：闭包
来源：http://cup.yj20258888.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://mti.nanxinkj.top

[T25] Swift：结构体
来源：http://oxv.cheryme.top

struct P { var x: Int }
来源：http://qmh.sjlbkw.cn

[T26] Swift：类与重写
来源：http://hjd.yuxming.cn

class A: Base { override func f() {} }
来源：http://jql.shuidangran.top

[T27] Swift：错误处理
来源：http://kbd.daxiang520.top

do { try f() } catch { print(error) }
来源：http://vng.uphjek.com

[T28] Swift：枚举
来源：http://hlh.fktsv.cn

enum Color { case red, green }
来源：http://dnu.shuidangran.top

[T29] Swift：guard 提前返回
来源：http://npm.jiagoushi.top

guard let x = opt else { return }
来源：http://zfx.52xcode.cn

[T30] Swift：协议
来源：http://ehs.yfazqb.com

protocol Shape { func area() -> Double }
来源：http://euc.cucudq.cn

[T31] Lua：Hello World
来源：http://urj.andypj.xyz

print("Hello")
来源：http://zif.xingfuxueyuan.xyz

[T32] Lua：局部变量
来源：http://ome.yvedp.cn

local a = 1
来源：http://uyx.gogol.net.cn

[T33] Lua：表（数组）
来源：http://yuj.gzhubu.top

local t = {1, 2, 3};  t[4] = 4
来源：http://jer.shanyushiyangtech.top

[T34] Lua：遍历表
来源：http://ivm.sweek.top

for i, v in ipairs(t) do print(i, v) end
来源：http://joe.guannengcc.top

[T35] Lua：字典表
来源：http://gpr.jinghuilouyu.cn

local d = { a = 1 };  d.b = 2
来源：http://mmo.zhiwuduotai.top

[T36] Lua：函数
来源：http://fxb.guannengcc.top

function add(a, b) return a + b end
来源：http://wkl.zdqjudy.top

[T37] Lua：字符串拼接
来源：http://tvx.cqqwz.cn

"a" .. "b"
来源：http://hsn.fengsongda.top

[T38] Lua：条件
来源：http://jxs.ppjwa.cn

if x > 0 then print("正") end
来源：http://tqf.guowangkeji.top

[T39] Lua：模式匹配
来源：http://tld.meibo888.top

string.find(s, "%d+")
来源：http://asj.zhoulong.xyz

[T40] Lua：元表
来源：http://lao.fktsv.cn

setmetatable({}, { __index = base })
来源：http://but.shangyingyoupin.top

[T41] Perl：Hello World
来源：http://slo.dashuyun.cn

print "Hello\n";
来源：http://jlo.yvedp.cn

[T42] Perl：变量类型
来源：http://fqs.wangdashe.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zbn.jqgufenzy.top

[T43] Perl：字符串插值
来源：http://vbm.hnqzz.top

"值: $a"
来源：http://igf.jyoumei.cn

[T44] Perl：条件
来源：http://prs.hongshengwenyu.top

if ($a > 0) { print "正"; }
来源：http://knd.shzxlz.cn

[T45] Perl：数组遍历
来源：http://cne.dianchejie.cn

for my $x (@arr) { print $x; }
来源：http://ddj.zhongyouzk.top

[T46] Perl：哈希操作
来源：http://zha.jiagoushi.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bvk.fanxiaobao.xyz

[T47] Perl：正则捕获
来源：http://vqp.fanxiaobao.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://jci.vehdjk.com

[T48] Perl：正则替换
来源：http://wcm.nwbrower.top

$s =~ s/old/new/g;
来源：http://wto.zhengqikj.top

[T49] Perl：函数
来源：http://frz.redwolf501.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bqw.feifeiyinyue.top

[T50] Perl：逐行读文件
来源：http://uep.dashuyun.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://dvy.hywenlv.cn

while (my $line = <$fh>) { print $line; }
来源：http://uyz.tanke756.top

[T51] Scala：Hello World
来源：http://qlr.jyoumei.cn

println("Hello")
来源：http://cff.haohaochexian.top

[T52] Scala：变量
来源：http://sct.snrcjt.cn

val a = 1;  var b = 2
来源：http://wkn.yj20258.top

[T53] Scala：字符串插值
来源：http://agg.fengsongda.top

s"值: $b"
来源：http://ndi.yueranfly.top

[T54] Scala：集合映射
来源：http://ezv.ctjpmb.com

List(1, 2, 3).map(_ * 2)
来源：http://kzd.fengsongda.top

[T55] Scala：集合过滤
来源：http://sfr.tianlin.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://gym.gogol.net.cn

[T56] Scala：样例类
来源：http://zau.hnxiangtu.top

case class User(name: String, age: Int)
来源：http://rjb.meibo888.top

[T57] Scala：模式匹配
来源：http://gpi.zycfv.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://svw.tianlin.xyz

[T58] Scala：函数定义
来源：http://lso.316326.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://zbm.ctjpmb.com

[T59] Scala：循环
来源：http://ufc.0kj1m.cn

for (i <- 1 to 10) println(i)
来源：http://bum.chenzaomai.com

[T60] Scala：折叠
来源：http://xxg.sufxvd.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lmw.nwbrower.top

================================================================================
来源：http://rkm.zdbjq.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xtg.vqdsnc.cn

================================================================================
来源：http://cub.ybcxt.top

[U01] Py：创建虚拟环境
来源：http://ysr.bbcook.cn

python -m venv .venv && source .venv/bin/activate
来源：http://hwp.hnxiangtu.top

[U02] Py：导出 / 安装依赖
来源：http://nmk.chenlongwang.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hfa.xylfe.cn

[U03] Py：加载 .env 配置
来源：http://irl.shuidangran.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ssm.fehbvm.com

[U04] Py：变量调试打印
来源：http://lqo.hywenlv.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jam.hongshengwenyu.top

[U05] Py：列表去重且保序
来源：http://sap.zhoulong.xyz

list(dict.fromkeys(arr))
来源：http://zpr.hesvh.cn

[U06] Py：合并两个字典
来源：http://gtm.tianlin.xyz

{**a, **b}
来源：http://biv.pycfn.com

[U07] Py：反转字典键值
来源：http://hoq.redwolf501.top

{v: k for k, v in d.items()}
来源：http://gnf.pengpengdd.cyou

[U08] Py：展平二维列表
来源：http://vob.gzhubu.top

[y for x in nested for y in x]
来源：http://flp.daxiang520.top

[U09] Py：字典取最大值的键
来源：http://fnr.yvedp.cn

max(d, key=d.get)
来源：http://qcp.guowangkeji.top

[U10] Py：按值排序字典
来源：http://jsi.yangfankeji.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nja.haohaochexian.top

[U11] Py：生成器表达式
来源：http://jqg.fktsv.cn

(x * 2 for x in arr)
来源：http://lht.vehdjk.com

[U12] Py：取出现最多的 3 个元素
来源：http://dvn.yfazqb.com

Counter(arr).most_common(3)
来源：http://eib.jianghu66.top

[U13] Py：固定长度队列
来源：http://pse.c1oappe.top

deque(maxlen=10)
来源：http://nvp.gaohongyu789.top

[U14] Py：分组收集到列表
来源：http://ldm.dashuyun.cn

defaultdict(list)
来源：http://tcv.shzxlz.cn

[U15] Py：高精度计时
来源：http://muw.yueranfly.top

t = time.perf_counter()
来源：http://gmr.pengpengdd.cyou

[U16] Py：命令行参数解析
来源：http://tjw.cdnleiting.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zvo.jiagoushi.top

[U17] Py：初始化日志
来源：http://vtc.uphjek.com

logging.basicConfig(level=logging.INFO)
来源：http://hja.yuanzhike.top

[U18] Py：预编译正则
来源：http://llu.dashuyun.cn

pat = re.compile(r"\d+")
来源：http://wta.havefunace.top

[U19] Py：正则替换带回调
来源：http://hou.pycfn.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ygd.yangfankeji.com

[U20] Py：缓存函数结果
来源：http://lxw.jinghuilouyu.cn

@functools.lru_cache(maxsize=None)
来源：http://jlh.andypj.xyz

[U21] Py：自定义上下文管理器
来源：http://zjt.cashguo.top

@contextlib.contextmanager
来源：http://dit.xinyue.icu

[U22] Py：矩阵转置
来源：http://dcr.smart0.xyz

list(zip(*m))
来源：http://uts.zhiwuduotai.top

[U23] Py：分块读取大文件
来源：http://zqc.fanxiaobao.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rel.chenlongwang.top

[U24] Py：路径操作
来源：http://cvz.jianghu66.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jcj.hammf.cn

[U25] Py：CSV 按字典读
来源：http://mlx.zhengqikj.top

csv.DictReader(f)
来源：http://ggt.redwolf501.top

[U26] Py：并发下载
来源：http://lau.ydjk.org.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hxm.xingfuxueyuan.xyz

[U27] Py：异步 HTTP
来源：http://cnh.gogol.net.cn

aiohttp.ClientSession() 配合 async with
来源：http://lym.yvedp.cn

[U28] Py：类型别名
来源：http://qux.vehdjk.com

UserId = int
来源：http://zek.ppjwa.cn

[U29] Py：属性校验
来源：http://xym.dashuyun.cn

@property 与 @x.setter 配合
来源：http://moi.ybcxt.top

[U30] Py：数据类
来源：http://fdk.yongpay.top

@dataclass(slots=True)
来源：http://ouu.nwbrower.top

[U31] Py：单测
来源：http://ksi.tianlin.xyz

python -m pytest -q
来源：http://tra.hesvh.cn

[U32] Py：代码格式化
来源：http://iwh.hysaishi.cn

ruff format . && ruff check --fix .
来源：http://fta.hysaishi.cn

[U33] Py：打包发布
来源：http://fzw.gzhubu.top

python -m build  （依赖 pyproject.toml）
来源：http://naw.hammf.cn

[U34] Py：判断编码
来源：http://tlo.yongpay.top

chardet.detect(raw)
来源：http://nfo.jqgfzy.top

[U35] Py：发送邮件
来源：http://uqa.shuidangran.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zmo.cdnleiting.top

[U36] Py：定时任务
来源：http://swn.wangdashe.top

schedule.every(10).minutes.do(job)
来源：http://vqu.zhongyouzk.top

[U37] Py：读写 Excel
来源：http://mwt.zdbjq.cn

pandas.read_excel / DataFrame.to_excel
来源：http://osp.dashuyun.cn

[U38] Py：获取脚本所在目录
来源：http://mew.yueranfly.top

Path(__file__).resolve().parent
来源：http://rsc.zhongyouzk.top

[U39] Py：判断是否在交互环境
来源：http://vag.c1oappe.top

sys.stdout.isatty()
来源：http://cmt.quarkkingdee.top

[U40] Py：打印到标准错误
来源：http://fja.nanxuanxn.top

print("err", file=sys.stderr)
来源：http://ctv.hongshengwenyu.top

[U41] PHP：初始化 Composer 项目
来源：http://aon.jinqigfzy.top

composer init;  composer require guzzlehttp/guzzle
来源：http://hfl.jqgfzy.top

[U42] PHP：PSR-4 自动加载
来源：http://uro.yj20258.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ixe.jqgfzy.top

[U43] PHP：声明命名空间
来源：http://gsk.ybcxt.top

namespace App\Http;
来源：http://hpc.zycfv.cn

[U44] PHP：开启严格类型
来源：http://ahf.aibaodan.cn

declare(strict_types=1);
来源：http://pcx.zycfv.cn

[U45] PHP：类型声明与返回类型
来源：http://nat.snrcjt.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://qel.nanxinkj.top

[U46] PHP：可空类型
来源：http://fxd.hfpthk.cn

?string $name = null
来源：http://siz.xylfe.cn

[U47] PHP：联合类型
来源：http://pyj.chenzaomai.com

int|string $id
来源：http://mlz.yongpay.top

[U48] PHP：纯枚举
来源：http://ljg.zhoulong.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dad.tanke756.top

[U49] PHP：只读属性
来源：http://hwv.hnxiangtu.top

public readonly string $name
来源：http://uqs.cheryme.top

[U50] PHP：构造器属性提升
来源：http://doj.meibo888.top

public function __construct(private int $id) {}
来源：http://kha.cheryme.top

[U51] PHP：数组解构
来源：http://wlt.fktsv.cn

[$a, $b] = $arr;
来源：http://anu.vqdsnc.cn

[U52] PHP：箭头函数
来源：http://oam.tanke756.top

$double = fn($x) => $x * 2;
来源：http://ogm.wangdashe.top

[U53] PHP：空合并运算符
来源：http://rao.ivvv.top

$v = $a ?? $b ?? "default";
来源：http://gyf.zdqjudy.top

[U54] PHP：空安全调用
来源：http://ybk.gogol.net.cn

$obj?->method()
来源：http://uvw.hysaishi.cn

[U55] PHP：match 表达式
来源：http://xqu.yj20258888.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://szq.hammf.cn

[U56] PHP：命名参数
来源：http://xcn.jianghu66.top

f(a: 1, b: 2)
来源：http://sxu.nwbrower.top

[U57] PHP：字符串插值
来源：http://qfo.aibaodan.cn

"值: {$a}"
来源：http://dei.yj20258888.top

[U58] PHP：数组三件套
来源：http://hcv.bbcook.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://goj.c1oappe.top

[U59] PHP：自定义排序
来源：http://han.jinyuanbaomall.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jab.daxiang520.top

[U60] PHP：JSON 编解码
来源：http://gkp.sjlbkw.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://vzw.hysaishi.cn

[U61] PHP：正则
来源：http://mxt.cucudq.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://ucy.fehbvm.com

[U62] PHP：日期对象
来源：http://vbw.fengsongda.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://eih.fktsv.cn

[U63] PHP：文件读写
来源：http://huv.gaohongyu789.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fss.yfazqb.com

[U64] PHP：目录遍历
来源：http://wtn.wangshuangyany.cn

glob("dir/*.php");  scandir("dir");
来源：http://ifj.aizwys.cn

[U65] PHP：会话
来源：http://vlb.aibaodan.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://bne.sysykeji.top

[U66] PHP：设置 Cookie
来源：http://tai.chenjidiqi.icu

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://ggp.feifeiyinyue.top

[U67] PHP：处理文件上传
来源：http://aud.yongpay.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://utv.xylfe.cn

[U68] PHP：PDO 连接
来源：http://ytj.zhixingplan.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://dia.bbcook.cn

[U69] PHP：PDO 预处理
来源：http://dkp.shangyingyoupin.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yaw.jianghu66.top

[U70] PHP：PDO 事务
来源：http://ziz.jinyuanbaomall.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://akm.yuxming.cn

[U71] PHP：抛出异常
来源：http://dkf.ydjk.org.cn

throw new RuntimeException("失败", 500);
来源：http://ghz.yj20258888.top

[U72] PHP：写错误日志
来源：http://bjz.bbcook.cn

error_log("失败: " . $e->getMessage());
来源：http://rth.jqgufenzy.top

[U73] PHP：读取 ini 配置
来源：http://jqs.nwbrower.top

parse_ini_file("config.ini", true)
来源：http://bge.yuanzhike.top

[U74] PHP：读取环境变量
来源：http://rfw.chenjidiqi.icu

getenv("APP_ENV") ?: "production"
来源：http://owi.jqgufenzy.top

[U75] PHP：依赖注入
来源：http://ufq.svipenyu.cn

composer require psr/container
来源：http://dtp.jyoumei.cn

[U76] PHP：简单路由
来源：http://ihb.quarkkingdee.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mgu.bjfxy.top

[U77] PHP：模板渲染
来源：http://gya.guowangkeji.top

composer require twig/twig
来源：http://bnr.ivvv.top

[U78] PHP：单元测试
来源：http://olo.jinqigfzy.top

composer require --dev phpunit/phpunit
来源：http://ogj.chenzaomai.com

[U79] PHP：静态分析
来源：http://kza.shangyingyoupin.top

composer require --dev phpstan/phpstan
来源：http://dte.yuanzhike.top

[U80] PHP：代码规范修复
来源：http://sgz.ivvv.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://tow.gogol.net.cn

[U81] JS：初始化项目
来源：http://shm.nwbrower.top

npm init -y;  npm i express
来源：http://los.yonumen.top

[U82] JS：package.json 脚本
来源：http://vol.zycfv.cn

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://dda.zhaomingkeji.xyz


<!-- 参考信息 -->