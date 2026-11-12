代发 wailian999

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zwo.yj20258888.top

[S57] C++：编译期常量
来源：http://oho.jinghuilouyu.cn

constexpr int N = 10;
来源：http://jex.c1oappe.top

[S58] C++：命名空间
来源：http://xrw.hesvh.cn

namespace ns { int f() { return 1; } }
来源：http://qrg.jqgfzy.top

[S59] C++：静态断言
来源：http://uww.zhijiandao.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yti.hnxiangtu.top

[S60] C++：遍历并删除元素
来源：http://clz.aibaodan.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hcy.tian-w.cn

================================================================================
来源：http://vgp.zdqjudy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ytt.fanxiaobao.xyz

================================================================================
来源：http://kaa.yfazqb.com

[T01] Kotlin：Hello World
来源：http://smo.9152youxi.cn

println("Hello")
来源：http://dut.xuanzx.com

[T02] Kotlin：变量
来源：http://ndx.yangfankeji.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vov.hesvh.cn

[T03] Kotlin：字符串模板
来源：http://vye.316326.xyz

"值: $b"
来源：http://hwh.shanyushiyangkeji.top

[T04] Kotlin：空安全
来源：http://rpw.jinqigfzy.top

val n: String? = null;  n?.length
来源：http://xqg.havefunace.top

[T05] Kotlin：when 表达式
来源：http://fam.ywan-chungtsiang.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yfs.gzhubu.top

[T06] Kotlin：集合映射
来源：http://kbx.zycfv.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://oes.zhengqikj.top

[T07] Kotlin：集合过滤
来源：http://eyp.yfazqb.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://vfx.dianchejie.cn

[T08] Kotlin：数据类
来源：http://gyz.shanyushiyangtech.top

data class User(val name: String, val age: Int)
来源：http://kng.cdnleiting.top

[T09] Kotlin：扩展函数
来源：http://wsm.epnwcf.com

fun String.exclaim() = this + "!"
来源：http://oxt.jianghu66.top

[T10] Kotlin：默认参数
来源：http://fag.zhijiandao.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vwn.quarkkingdee.top

[T11] Kotlin：协程
来源：http://nvy.jqgufenzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://bpq.9152youxi.cn

[T12] Kotlin：解构声明
来源：http://wie.daria6918.cn

val (a, b) = Pair(1, 2)
来源：http://qej.zhaomingkeji.xyz

[T13] Kotlin：只读 Map
来源：http://kux.zycfv.cn

val m = mapOf("a" to 1)
来源：http://vle.jianghu66.top

[T14] Kotlin：循环
来源：http://aht.yanxiufei.cn

for (i in 1..10) println(i)
来源：http://fws.dashuyun.cn

[T15] Kotlin：接口
来源：http://jzk.meibo888.top

interface Shape { fun area(): Double }
来源：http://iux.hfpthk.cn

[T16] Swift：Hello World
来源：http://ind.hysaishi.cn

print("Hello")
来源：http://kle.gzhubu.top

[T17] Swift：变量与常量
来源：http://hzv.uphjek.com

var a = 1;  let b = 2
来源：http://tzy.bjfxy.top

[T18] Swift：字符串插值
来源：http://arf.ppjwa.cn

"值: \(b)"
来源：http://ewj.jinqigufen.top

[T19] Swift：可选绑定
来源：http://pww.nanxuanxn.top

if let n = opt { print(n) }
来源：http://qdu.yangfankeji.com

[T20] Swift：数组操作
来源：http://dxr.vehdjk.com

var a = [1, 2, 3];  a.append(4)
来源：http://nrl.wangdashe.top

[T21] Swift：遍历
来源：http://xie.yfazqb.com

for x in a { print(x) }
来源：http://twd.jlsjyb.cn

[T22] Swift：字典
来源：http://mvc.zhongyouzk.top

var d = ["a": 1];  d["b"] = 2
来源：http://ctq.zdqjudy.top

[T23] Swift：函数
来源：http://dti.jinqigfzy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://djq.bbcook.cn

[T24] Swift：闭包
来源：http://xkj.jinqigufen.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://dkz.cashguo.top

[T25] Swift：结构体
来源：http://hks.ehwqpu.com

struct P { var x: Int }
来源：http://its.daxiang520.top

[T26] Swift：类与重写
来源：http://fgd.yj20258.top

class A: Base { override func f() {} }
来源：http://nhf.gotoacloud.top

[T27] Swift：错误处理
来源：http://jlb.wangdashe.top

do { try f() } catch { print(error) }
来源：http://djl.hysaishi.cn

[T28] Swift：枚举
来源：http://fni.dianchejie.cn

enum Color { case red, green }
来源：http://whv.hammf.cn

[T29] Swift：guard 提前返回
来源：http://tsp.haohaochexian.top

guard let x = opt else { return }
来源：http://pmr.guowangkeji.top

[T30] Swift：协议
来源：http://ire.hfpthk.cn

protocol Shape { func area() -> Double }
来源：http://rbk.redwolf501.top

[T31] Lua：Hello World
来源：http://fhr.nanxinkj.top

print("Hello")
来源：http://owd.hesvh.cn

[T32] Lua：局部变量
来源：http://txc.yonumen.top

local a = 1
来源：http://xqk.chenjidiqi.icu

[T33] Lua：表（数组）
来源：http://uxh.ybcxt.top

local t = {1, 2, 3};  t[4] = 4
来源：http://qxd.nanxuanxn.top

[T34] Lua：遍历表
来源：http://lsp.52xcode.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://dyg.ivvv.top

[T35] Lua：字典表
来源：http://ggf.bbcook.cn

local d = { a = 1 };  d.b = 2
来源：http://uez.zycfv.cn

[T36] Lua：函数
来源：http://bmo.xylfe.cn

function add(a, b) return a + b end
来源：http://mha.cdnleiting.top

[T37] Lua：字符串拼接
来源：http://bcp.hongshengwenyu.top

"a" .. "b"
来源：http://nvv.jinqigfzy.top

[T38] Lua：条件
来源：http://aah.hcnkem.com

if x > 0 then print("正") end
来源：http://viz.wangdashe.top

[T39] Lua：模式匹配
来源：http://ueu.snrcjt.cn

string.find(s, "%d+")
来源：http://pro.sjlbkw.cn

[T40] Lua：元表
来源：http://ygl.jinghuilouyu.cn

setmetatable({}, { __index = base })
来源：http://ujj.fehbvm.com

[T41] Perl：Hello World
来源：http://ibf.ctjpmb.com

print "Hello\n";
来源：http://qhh.tanke756.top

[T42] Perl：变量类型
来源：http://ssc.wangshuangyany.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wfi.hongshengwenyu.top

[T43] Perl：字符串插值
来源：http://ged.zdqjudy.top

"值: $a"
来源：http://ukr.pycfn.com

[T44] Perl：条件
来源：http://eip.cucudq.cn

if ($a > 0) { print "正"; }
来源：http://ohv.jlsjyb.cn

[T45] Perl：数组遍历
来源：http://kft.wangdashe.top

for my $x (@arr) { print $x; }
来源：http://har.jqgfzy.top

[T46] Perl：哈希操作
来源：http://ofe.tanke756.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ktj.sjlbkw.cn

[T47] Perl：正则捕获
来源：http://mvf.mhx1999.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://fog.yfazqb.com

[T48] Perl：正则替换
来源：http://dte.daria6918.cn

$s =~ s/old/new/g;
来源：http://xqq.ywan-chungtsiang.top

[T49] Perl：函数
来源：http://kcr.hywenlv.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://das.yj202588.top

[T50] Perl：逐行读文件
来源：http://iom.jinqigufen.top

open my $fh, "<", "a.txt" or die $!;
来源：http://tpd.daxiang520.top

while (my $line = <$fh>) { print $line; }
来源：http://fpu.zhixingplan.top

[T51] Scala：Hello World
来源：http://dow.fengsongda.top

println("Hello")
来源：http://gzm.sjlbkw.cn

[T52] Scala：变量
来源：http://wbm.jinqigfzy.top

val a = 1;  var b = 2
来源：http://odb.yfazqb.com

[T53] Scala：字符串插值
来源：http://gsj.shangyingyoupin.top

s"值: $b"
来源：http://uap.xuetiantiany.cn

[T54] Scala：集合映射
来源：http://aki.xuetiantiany.cn

List(1, 2, 3).map(_ * 2)
来源：http://sai.hnxiangtu.top

[T55] Scala：集合过滤
来源：http://bhr.cqqwz.cn

List(1, 2, 3).filter(_ > 1)
来源：http://srh.zhiwuduotai.top

[T56] Scala：样例类
来源：http://okb.mhx1999.top

case class User(name: String, age: Int)
来源：http://drb.hesvh.cn

[T57] Scala：模式匹配
来源：http://qrv.ywan-chungtsiang.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ifh.cqqwz.cn

[T58] Scala：函数定义
来源：http://qpw.wangdashe.top

def add(a: Int, b: Int): Int = a + b
来源：http://jmy.cdnleiting.top

[T59] Scala：循环
来源：http://pci.zhixingplan.top

for (i <- 1 to 10) println(i)
来源：http://hbh.guowangkeji.top

[T60] Scala：折叠
来源：http://yym.yongpay.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dxg.vqdsnc.cn

================================================================================
来源：http://uwv.jinqigufen.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lnc.quarkkingdee.top

================================================================================
来源：http://fxn.bjfxy.top

[U01] Py：创建虚拟环境
来源：http://xmm.hesvh.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vib.yj20258.top

[U02] Py：导出 / 安装依赖
来源：http://gss.quarkkingdee.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tmb.hongshengwenyu.top

[U03] Py：加载 .env 配置
来源：http://tfx.dashuyun.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://hcp.zycfv.cn

[U04] Py：变量调试打印
来源：http://tko.fehbvm.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://duo.gaohongyu789.top

[U05] Py：列表去重且保序
来源：http://esu.nanxuanxn.top

list(dict.fromkeys(arr))
来源：http://mnx.ctjpmb.com

[U06] Py：合并两个字典
来源：http://cpz.jinqigfzy.top

{**a, **b}
来源：http://bsz.hongshengwenyu.top

[U07] Py：反转字典键值
来源：http://oaf.xuanzx.com

{v: k for k, v in d.items()}
来源：http://zyy.tarul.cn

[U08] Py：展平二维列表
来源：http://xyp.nanxuanxn.top

[y for x in nested for y in x]
来源：http://vzk.shzxlz.cn

[U09] Py：字典取最大值的键
来源：http://jlv.ctjpmb.com

max(d, key=d.get)
来源：http://okf.redwolf501.top

[U10] Py：按值排序字典
来源：http://fzd.bbcook.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kud.cashguo.top

[U11] Py：生成器表达式
来源：http://pur.fanxiaobao.xyz

(x * 2 for x in arr)
来源：http://lde.fehbvm.com

[U12] Py：取出现最多的 3 个元素
来源：http://juz.epnwcf.com

Counter(arr).most_common(3)
来源：http://kxd.cashguo.top

[U13] Py：固定长度队列
来源：http://izx.jianghu66.top

deque(maxlen=10)
来源：http://rxi.kuanghao11.cn

[U14] Py：分组收集到列表
来源：http://cun.hnxiangtu.top

defaultdict(list)
来源：http://vvv.daria6918.cn

[U15] Py：高精度计时
来源：http://wex.nanxuanxn.top

t = time.perf_counter()
来源：http://jsq.dianchejie.cn

[U16] Py：命令行参数解析
来源：http://xwk.gogol.net.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ehf.xziqi.cn

[U17] Py：初始化日志
来源：http://oxw.yonumen.top

logging.basicConfig(level=logging.INFO)
来源：http://daz.tanke756.top

[U18] Py：预编译正则
来源：http://nan.jqgufenzy.top

pat = re.compile(r"\d+")
来源：http://bws.cdnleiting.top

[U19] Py：正则替换带回调
来源：http://sja.iojbl.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xes.xziqi.cn

[U20] Py：缓存函数结果
来源：http://cnt.wangshuangyany.cn

@functools.lru_cache(maxsize=None)
来源：http://ehp.uphjek.com

[U21] Py：自定义上下文管理器
来源：http://tyg.ctjpmb.com

@contextlib.contextmanager
来源：http://awg.haohaochexian.top

[U22] Py：矩阵转置
来源：http://rsf.hnqzz.top

list(zip(*m))
来源：http://xgw.aizwys.cn

[U23] Py：分块读取大文件
来源：http://gwm.shangyingyoupin.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://elw.smart0.xyz

[U24] Py：路径操作
来源：http://vti.zhoulong.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tzx.bbcook.cn

[U25] Py：CSV 按字典读
来源：http://muy.zdqjudy.top

csv.DictReader(f)
来源：http://xbk.zhijiandao.cn

[U26] Py：并发下载
来源：http://jzp.shanyushiyangkeji.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://efs.aibaodan.cn

[U27] Py：异步 HTTP
来源：http://jpz.ehwqpu.com

aiohttp.ClientSession() 配合 async with
来源：http://ryu.daxiang520.top

[U28] Py：类型别名
来源：http://ipg.yj20258888.top

UserId = int
来源：http://sow.yj20258.top

[U29] Py：属性校验
来源：http://snr.jinqigfzy.top

@property 与 @x.setter 配合
来源：http://ibz.cashguo.top

[U30] Py：数据类
来源：http://dvy.yongpay.top

@dataclass(slots=True)
来源：http://vps.jinqigufen.top

[U31] Py：单测
来源：http://wzx.yonumen.top

python -m pytest -q
来源：http://nqd.yj20258.top

[U32] Py：代码格式化
来源：http://epi.hnqzz.top

ruff format . && ruff check --fix .
来源：http://gin.yongpay.top

[U33] Py：打包发布
来源：http://vjf.xuetiantiany.cn

python -m build  （依赖 pyproject.toml）
来源：http://lir.dianchejie.cn

[U34] Py：判断编码
来源：http://yam.yueranfly.top

chardet.detect(raw)
来源：http://cfr.uphjek.com

[U35] Py：发送邮件
来源：http://zjq.nanxuanxn.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://awu.guannengcc.top

[U36] Py：定时任务
来源：http://qpz.hnxiangtu.top

schedule.every(10).minutes.do(job)
来源：http://die.yj20258888.top

[U37] Py：读写 Excel
来源：http://afl.cdnleiting.top

pandas.read_excel / DataFrame.to_excel
来源：http://gvf.shzxlz.cn

[U38] Py：获取脚本所在目录
来源：http://atg.wangshuangyany.cn

Path(__file__).resolve().parent
来源：http://fhh.shzxlz.cn

[U39] Py：判断是否在交互环境
来源：http://vte.yueranfly.top

sys.stdout.isatty()
来源：http://zuf.kuanghao11.cn

[U40] Py：打印到标准错误
来源：http://fbq.jianghu66.top

print("err", file=sys.stderr)
来源：http://pwf.yuanzhike.top

[U41] PHP：初始化 Composer 项目
来源：http://ktj.kuanghao11.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://afz.shuidangran.top

[U42] PHP：PSR-4 自动加载
来源：http://yyx.feifeiyinyue.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://upl.smart0.xyz

[U43] PHP：声明命名空间
来源：http://vde.zhijiandao.cn

namespace App\Http;
来源：http://dwv.hywenlv.cn

[U44] PHP：开启严格类型
来源：http://bfa.0kj1m.cn

declare(strict_types=1);
来源：http://xau.wangshuangyany.cn

[U45] PHP：类型声明与返回类型
来源：http://slh.hysaishi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ldg.zdqjudy.top

[U46] PHP：可空类型
来源：http://hlo.hfpthk.cn

?string $name = null
来源：http://mnu.cucudq.cn

[U47] PHP：联合类型
来源：http://ozp.havefunace.top

int|string $id
来源：http://iih.pycfn.com

[U48] PHP：纯枚举
来源：http://fim.zhaomingkeji.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lim.yuxming.cn

[U49] PHP：只读属性
来源：http://dgs.ydjk.org.cn

public readonly string $name
来源：http://jli.hcnkem.com

[U50] PHP：构造器属性提升
来源：http://zkf.shanyushiyangkeji.top

public function __construct(private int $id) {}
来源：http://pws.guannengcc.top

[U51] PHP：数组解构
来源：http://htz.jinqigufen.top

[$a, $b] = $arr;
来源：http://bar.dianchejie.cn

[U52] PHP：箭头函数
来源：http://omz.chenjidiqi.icu

$double = fn($x) => $x * 2;
来源：http://czx.nanxuanxn.top

[U53] PHP：空合并运算符
来源：http://kiz.yuanzhike.top

$v = $a ?? $b ?? "default";
来源：http://jli.epnwcf.com

[U54] PHP：空安全调用
来源：http://gqx.jinqigufen.top

$obj?->method()
来源：http://xsi.kuanghao11.cn

[U55] PHP：match 表达式
来源：http://ryg.pengpengdd.cyou

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ufc.shzxlz.cn

[U56] PHP：命名参数
来源：http://var.zdqjudy.top

f(a: 1, b: 2)
来源：http://fnu.yj20258.top

[U57] PHP：字符串插值
来源：http://zvu.hcnkem.com

"值: {$a}"
来源：http://wka.mhx1999.top

[U58] PHP：数组三件套
来源：http://kyi.gzhubu.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://iqq.hywenlv.cn

[U59] PHP：自定义排序
来源：http://dnd.ivvv.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dxf.jianghu66.top

[U60] PHP：JSON 编解码
来源：http://sjv.uphjek.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lhe.xuetiantiany.cn

[U61] PHP：正则
来源：http://drm.shuidangran.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://yyb.zhaomingkeji.xyz

[U62] PHP：日期对象
来源：http://ytm.yongpay.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://tcz.kuanghao11.cn

[U63] PHP：文件读写
来源：http://bek.svipenyu.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://pkd.nanxinkj.top

[U64] PHP：目录遍历
来源：http://jzr.fanxiaobao.xyz

glob("dir/*.php");  scandir("dir");
来源：http://fll.daria6918.cn

[U65] PHP：会话
来源：http://wub.c1oappe.top

session_start();  $_SESSION["uid"] = 1;
来源：http://zzd.yangfankeji.com

[U66] PHP：设置 Cookie
来源：http://lrn.sweek.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vzh.0kj1m.cn

[U67] PHP：处理文件上传
来源：http://acy.chenjidiqi.icu

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lkm.daxiang520.top

[U68] PHP：PDO 连接
来源：http://nmu.ppjwa.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://cna.yangfankeji.com

[U69] PHP：PDO 预处理
来源：http://pfo.gotoacloud.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://zvz.epnwcf.com

[U70] PHP：PDO 事务
来源：http://hix.tianlin.xyz

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tdj.9152youxi.cn

[U71] PHP：抛出异常
来源：http://bgo.andypj.xyz

throw new RuntimeException("失败", 500);
来源：http://fln.gogol.net.cn

[U72] PHP：写错误日志
来源：http://pcw.jinqigfzy.top

error_log("失败: " . $e->getMessage());
来源：http://slm.jlsjyb.cn

[U73] PHP：读取 ini 配置
来源：http://agp.yfazqb.com

parse_ini_file("config.ini", true)
来源：http://tft.yongpay.top

[U74] PHP：读取环境变量
来源：http://sra.fktsv.cn

getenv("APP_ENV") ?: "production"
来源：http://kft.wangdashe.top

[U75] PHP：依赖注入
来源：http://iro.yuanzhike.top

composer require psr/container
来源：http://ied.dashuyun.cn

[U76] PHP：简单路由
来源：http://tys.sysykeji.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pgh.nanxinkj.top

[U77] PHP：模板渲染
来源：http://ktq.zdbjq.cn

composer require twig/twig
来源：http://qil.9152youxi.cn

[U78] PHP：单元测试
来源：http://pbd.jqgfzy.top

composer require --dev phpunit/phpunit
来源：http://wvf.daria6918.cn

[U79] PHP：静态分析
来源：http://wib.aibaodan.cn

composer require --dev phpstan/phpstan
来源：http://czd.nanxuanxn.top

[U80] PHP：代码规范修复
来源：http://twj.9152youxi.cn

composer require --dev friendsofphp/php-cs-fixer
来源：http://iik.cucudq.cn

[U81] JS：初始化项目
来源：http://tji.jiagoushi.top

npm init -y;  npm i express
来源：http://sbl.chenzaomai.com

[U82] JS：package.json 脚本
来源：http://iti.yfazqb.com

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://axh.epnwcf.com


<!-- 参考信息 -->