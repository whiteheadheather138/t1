代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rho.xylfe.cn

[S55] C++：结构化绑定
来源：http://axh.zhoulong.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://mch.aibaodan.cn

[S56] C++：optional
来源：http://aej.pycfn.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tbv.jianghu66.top

[S57] C++：编译期常量
来源：http://vrw.nanxuanxn.top

constexpr int N = 10;
来源：http://vli.yuanzhike.top

[S58] C++：命名空间
来源：http://zez.wangdashe.top

namespace ns { int f() { return 1; } }
来源：http://wtq.hesvh.cn

[S59] C++：静态断言
来源：http://puc.xuanzx.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ewh.cucudq.cn

[S60] C++：遍历并删除元素
来源：http://xwe.redwolf501.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nhs.hysaishi.cn

================================================================================
来源：http://djw.xingfuxueyuan.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jto.svipenyu.cn

================================================================================
来源：http://xpm.ybcxt.top

[T01] Kotlin：Hello World
来源：http://ccz.zhongyouzk.top

println("Hello")
来源：http://bfj.xingfuxueyuan.xyz

[T02] Kotlin：变量
来源：http://dei.gzhubu.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ptf.hysaishi.cn

[T03] Kotlin：字符串模板
来源：http://mnh.jianghu66.top

"值: $b"
来源：http://axh.daxiang520.top

[T04] Kotlin：空安全
来源：http://hbs.xziqi.cn

val n: String? = null;  n?.length
来源：http://nti.zhoulong.xyz

[T05] Kotlin：when 表达式
来源：http://tdk.ydzc1.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sfy.ppjwa.cn

[T06] Kotlin：集合映射
来源：http://dox.feifeiyinyue.top

listOf(1, 2, 3).map { it * 2 }
来源：http://btl.ctjpmb.com

[T07] Kotlin：集合过滤
来源：http://jlr.yj20258.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://nui.andypj.xyz

[T08] Kotlin：数据类
来源：http://ajz.andypj.xyz

data class User(val name: String, val age: Int)
来源：http://zhi.ehwqpu.com

[T09] Kotlin：扩展函数
来源：http://ueb.nanxuanxn.top

fun String.exclaim() = this + "!"
来源：http://ovp.wangshuangyany.cn

[T10] Kotlin：默认参数
来源：http://wtm.yj20258.top

fun greet(name: String = "World") = "Hi $name"
来源：http://mmc.yangfankeji.com

[T11] Kotlin：协程
来源：http://yll.chenjidiqi.icu

GlobalScope.launch { delay(1000); println("done") }
来源：http://lgf.jqgfzy.top

[T12] Kotlin：解构声明
来源：http://ayd.kuanghao11.cn

val (a, b) = Pair(1, 2)
来源：http://wln.cdnleiting.top

[T13] Kotlin：只读 Map
来源：http://agp.jqgufenzy.top

val m = mapOf("a" to 1)
来源：http://kts.nanxuanxn.top

[T14] Kotlin：循环
来源：http://kpy.yuanzhike.top

for (i in 1..10) println(i)
来源：http://znf.mhx1999.top

[T15] Kotlin：接口
来源：http://mup.zhaomingkeji.xyz

interface Shape { fun area(): Double }
来源：http://vcn.ehwqpu.com

[T16] Swift：Hello World
来源：http://zkw.chenjidiqi.icu

print("Hello")
来源：http://lol.0kj1m.cn

[T17] Swift：变量与常量
来源：http://wad.gzhubu.top

var a = 1;  let b = 2
来源：http://ztb.snrcjt.cn

[T18] Swift：字符串插值
来源：http://wxs.ehwqpu.com

"值: \(b)"
来源：http://zxi.pycfn.com

[T19] Swift：可选绑定
来源：http://kxm.tianlin.xyz

if let n = opt { print(n) }
来源：http://gum.bjfxy.top

[T20] Swift：数组操作
来源：http://gla.svipenyu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://wlp.vehdjk.com

[T21] Swift：遍历
来源：http://vat.jianghu66.top

for x in a { print(x) }
来源：http://zfc.havefunace.top

[T22] Swift：字典
来源：http://jrq.yj202588.top

var d = ["a": 1];  d["b"] = 2
来源：http://zjk.yfazqb.com

[T23] Swift：函数
来源：http://qrp.yueranfly.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://upg.hongshengwenyu.top

[T24] Swift：闭包
来源：http://ocr.xylfe.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://chl.jlsjyb.cn

[T25] Swift：结构体
来源：http://two.yj20258.top

struct P { var x: Int }
来源：http://vuo.xuanzx.com

[T26] Swift：类与重写
来源：http://jsj.gotoacloud.top

class A: Base { override func f() {} }
来源：http://yit.sjlbkw.cn

[T27] Swift：错误处理
来源：http://twz.xuetiantiany.cn

do { try f() } catch { print(error) }
来源：http://bkx.snrcjt.cn

[T28] Swift：枚举
来源：http://soi.9152youxi.cn

enum Color { case red, green }
来源：http://mzu.jinghuilouyu.cn

[T29] Swift：guard 提前返回
来源：http://qhw.jinyuanbaomall.cn

guard let x = opt else { return }
来源：http://huw.guannengcc.top

[T30] Swift：协议
来源：http://mpt.yuanzhike.top

protocol Shape { func area() -> Double }
来源：http://oap.bbcook.cn

[T31] Lua：Hello World
来源：http://hyg.chenlongwang.top

print("Hello")
来源：http://dia.gzhubu.top

[T32] Lua：局部变量
来源：http://ius.fktsv.cn

local a = 1
来源：http://rpc.xinyue.icu

[T33] Lua：表（数组）
来源：http://sxr.ywan-chungtsiang.top

local t = {1, 2, 3};  t[4] = 4
来源：http://rfm.fehbvm.com

[T34] Lua：遍历表
来源：http://zjw.yuxming.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://hmi.feifeiyinyue.top

[T35] Lua：字典表
来源：http://xpy.aibaodan.cn

local d = { a = 1 };  d.b = 2
来源：http://usa.jinghuilouyu.cn

[T36] Lua：函数
来源：http://fgz.nanxinkj.top

function add(a, b) return a + b end
来源：http://cnl.ppjwa.cn

[T37] Lua：字符串拼接
来源：http://oap.epnwcf.com

"a" .. "b"
来源：http://igo.ydzc1.top

[T38] Lua：条件
来源：http://wjq.sjlbkw.cn

if x > 0 then print("正") end
来源：http://jcz.hywenlv.cn

[T39] Lua：模式匹配
来源：http://roh.hesvh.cn

string.find(s, "%d+")
来源：http://zdi.pycfn.com

[T40] Lua：元表
来源：http://okl.aizwys.cn

setmetatable({}, { __index = base })
来源：http://mze.nanxuanxn.top

[T41] Perl：Hello World
来源：http://mih.52xcode.cn

print "Hello\n";
来源：http://juy.cqqwz.cn

[T42] Perl：变量类型
来源：http://obe.cdnleiting.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sgh.vehdjk.com

[T43] Perl：字符串插值
来源：http://ilj.fzhhl.top

"值: $a"
来源：http://nyw.tarul.cn

[T44] Perl：条件
来源：http://mlo.ehwqpu.com

if ($a > 0) { print "正"; }
来源：http://ojk.shanyushiyangtech.top

[T45] Perl：数组遍历
来源：http://qor.shzxlz.cn

for my $x (@arr) { print $x; }
来源：http://nfc.hnxiangtu.top

[T46] Perl：哈希操作
来源：http://mhk.daxiang520.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pif.hysaishi.cn

[T47] Perl：正则捕获
来源：http://til.ybcxt.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://hci.xuetiantiany.cn

[T48] Perl：正则替换
来源：http://lgz.0kj1m.cn

$s =~ s/old/new/g;
来源：http://qfi.bbcook.cn

[T49] Perl：函数
来源：http://ool.nanxuanxn.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vyn.shuidangran.top

[T50] Perl：逐行读文件
来源：http://clq.zhiwuduotai.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ccp.xingfuxueyuan.xyz

while (my $line = <$fh>) { print $line; }
来源：http://nsv.havefunace.top

[T51] Scala：Hello World
来源：http://bvg.pycfn.com

println("Hello")
来源：http://nsh.feifeiyinyue.top

[T52] Scala：变量
来源：http://zjl.shzxlz.cn

val a = 1;  var b = 2
来源：http://lbv.shangyingyoupin.top

[T53] Scala：字符串插值
来源：http://hzq.bbcook.cn

s"值: $b"
来源：http://pct.hnqzz.top

[T54] Scala：集合映射
来源：http://vmr.9152youxi.cn

List(1, 2, 3).map(_ * 2)
来源：http://suu.haohaochexian.top

[T55] Scala：集合过滤
来源：http://dyy.svipenyu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://sfd.wangshuangyany.cn

[T56] Scala：样例类
来源：http://tzc.bjfxy.top

case class User(name: String, age: Int)
来源：http://bjp.zycfv.cn

[T57] Scala：模式匹配
来源：http://hgk.jinyuanbaomall.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://lxo.andypj.xyz

[T58] Scala：函数定义
来源：http://fpo.316326.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://fql.nwbrower.top

[T59] Scala：循环
来源：http://jhn.xuetiantiany.cn

for (i <- 1 to 10) println(i)
来源：http://rjz.jyoumei.cn

[T60] Scala：折叠
来源：http://imn.svipenyu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://uho.52xcode.cn

================================================================================
来源：http://odt.zhongyouzk.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gcg.ydjk.org.cn

================================================================================
来源：http://olm.yanxiufei.cn

[U01] Py：创建虚拟环境
来源：http://rik.hnxiangtu.top

python -m venv .venv && source .venv/bin/activate
来源：http://sim.zhengqikj.top

[U02] Py：导出 / 安装依赖
来源：http://gpy.iojbl.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tjf.ybcxt.top

[U03] Py：加载 .env 配置
来源：http://rou.bjfxy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ggd.pycfn.com

[U04] Py：变量调试打印
来源：http://cxs.shanyushiyangkeji.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mei.shanyushiyangtech.top

[U05] Py：列表去重且保序
来源：http://jle.zycfv.cn

list(dict.fromkeys(arr))
来源：http://wtv.zhixingplan.top

[U06] Py：合并两个字典
来源：http://doa.fehbvm.com

{**a, **b}
来源：http://qqd.meibo888.top

[U07] Py：反转字典键值
来源：http://twp.aizwys.cn

{v: k for k, v in d.items()}
来源：http://dym.yuxming.cn

[U08] Py：展平二维列表
来源：http://xxm.sysykeji.top

[y for x in nested for y in x]
来源：http://fdh.cashguo.top

[U09] Py：字典取最大值的键
来源：http://qce.sxryk.cn

max(d, key=d.get)
来源：http://ruc.dianchejie.cn

[U10] Py：按值排序字典
来源：http://kwi.jinqigfzy.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://coa.birdmap.top

[U11] Py：生成器表达式
来源：http://hfl.jqgufenzy.top

(x * 2 for x in arr)
来源：http://jdb.dianchejie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://cgx.nanxinkj.top

Counter(arr).most_common(3)
来源：http://xvl.cashguo.top

[U13] Py：固定长度队列
来源：http://tmn.fanxiaobao.xyz

deque(maxlen=10)
来源：http://agy.jinqigfzy.top

[U14] Py：分组收集到列表
来源：http://gcd.tarul.cn

defaultdict(list)
来源：http://uda.gogol.net.cn

[U15] Py：高精度计时
来源：http://dgu.havefunace.top

t = time.perf_counter()
来源：http://gsu.shanyushiyangkeji.top

[U16] Py：命令行参数解析
来源：http://xaj.ctjpmb.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mjg.havefunace.top

[U17] Py：初始化日志
来源：http://xij.meibo888.top

logging.basicConfig(level=logging.INFO)
来源：http://xvi.zhijiandao.cn

[U18] Py：预编译正则
来源：http://hww.xziqi.cn

pat = re.compile(r"\d+")
来源：http://kaw.tianlin.xyz

[U19] Py：正则替换带回调
来源：http://xom.yvedp.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vjh.zdqjudy.top

[U20] Py：缓存函数结果
来源：http://zgu.nanxuanxn.top

@functools.lru_cache(maxsize=None)
来源：http://nhu.tanke756.top

[U21] Py：自定义上下文管理器
来源：http://lkp.zhongyouzk.top

@contextlib.contextmanager
来源：http://xwz.dashuyun.cn

[U22] Py：矩阵转置
来源：http://jxw.hnqzz.top

list(zip(*m))
来源：http://izu.ydjk.org.cn

[U23] Py：分块读取大文件
来源：http://hqi.havefunace.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xra.yj202588.top

[U24] Py：路径操作
来源：http://xtj.tian-w.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://oge.quarkkingdee.top

[U25] Py：CSV 按字典读
来源：http://egz.jyoumei.cn

csv.DictReader(f)
来源：http://yym.yvedp.cn

[U26] Py：并发下载
来源：http://bzl.svipenyu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kun.jinghuilouyu.cn

[U27] Py：异步 HTTP
来源：http://bnb.cucudq.cn

aiohttp.ClientSession() 配合 async with
来源：http://wxb.quarkkingdee.top

[U28] Py：类型别名
来源：http://cja.316326.xyz

UserId = int
来源：http://exb.yonumen.top

[U29] Py：属性校验
来源：http://rio.gzhubu.top

@property 与 @x.setter 配合
来源：http://exg.hammf.cn

[U30] Py：数据类
来源：http://art.fanxiaobao.xyz

@dataclass(slots=True)
来源：http://nwd.sjlbkw.cn

[U31] Py：单测
来源：http://xmn.c1oappe.top

python -m pytest -q
来源：http://vlw.ydzc1.top

[U32] Py：代码格式化
来源：http://nzs.hywenlv.cn

ruff format . && ruff check --fix .
来源：http://vhb.ydzc1.top

[U33] Py：打包发布
来源：http://cal.aizwys.cn

python -m build  （依赖 pyproject.toml）
来源：http://hzn.feifeiyinyue.top

[U34] Py：判断编码
来源：http://std.sufxvd.cn

chardet.detect(raw)
来源：http://pjw.nanxuanxn.top

[U35] Py：发送邮件
来源：http://hle.jyoumei.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rfv.kuanghao11.cn

[U36] Py：定时任务
来源：http://bea.ppjwa.cn

schedule.every(10).minutes.do(job)
来源：http://ini.jiagoushi.top

[U37] Py：读写 Excel
来源：http://oma.vehdjk.com

pandas.read_excel / DataFrame.to_excel
来源：http://zff.gotoacloud.top

[U38] Py：获取脚本所在目录
来源：http://oaj.xylfe.cn

Path(__file__).resolve().parent
来源：http://xwj.hfpthk.cn

[U39] Py：判断是否在交互环境
来源：http://jbe.sjlbkw.cn

sys.stdout.isatty()
来源：http://gzd.guannengcc.top

[U40] Py：打印到标准错误
来源：http://tbi.xuetiantiany.cn

print("err", file=sys.stderr)
来源：http://pyz.shanyushiyangkeji.top

[U41] PHP：初始化 Composer 项目
来源：http://bdx.cheryme.top

composer init;  composer require guzzlehttp/guzzle
来源：http://wpc.zdqjudy.top

[U42] PHP：PSR-4 自动加载
来源：http://qwx.zhengqikj.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ujv.cashguo.top

[U43] PHP：声明命名空间
来源：http://yck.shanyushiyangkeji.top

namespace App\Http;
来源：http://pmc.gzhubu.top

[U44] PHP：开启严格类型
来源：http://gsw.kuanghao11.cn

declare(strict_types=1);
来源：http://kkg.yj20258.top

[U45] PHP：类型声明与返回类型
来源：http://bqw.yj20258888.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://nsa.daria6918.cn

[U46] PHP：可空类型
来源：http://atf.jianghu66.top

?string $name = null
来源：http://aci.jinghuilouyu.cn

[U47] PHP：联合类型
来源：http://bpm.snrcjt.cn

int|string $id
来源：http://kge.316326.xyz

[U48] PHP：纯枚举
来源：http://coq.xinyue.icu

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://lof.ivvv.top

[U49] PHP：只读属性
来源：http://sab.fengsongda.top

public readonly string $name
来源：http://wfj.jianghu66.top

[U50] PHP：构造器属性提升
来源：http://eeq.zhixingplan.top

public function __construct(private int $id) {}
来源：http://nul.hesvh.cn

[U51] PHP：数组解构
来源：http://tyl.shanyushiyangkeji.top

[$a, $b] = $arr;
来源：http://nfz.sweek.top

[U52] PHP：箭头函数
来源：http://mxe.gogol.net.cn

$double = fn($x) => $x * 2;
来源：http://wyp.yueranfly.top

[U53] PHP：空合并运算符
来源：http://nhr.sufxvd.cn

$v = $a ?? $b ?? "default";
来源：http://qla.jianghu66.top

[U54] PHP：空安全调用
来源：http://snw.xinyue.icu

$obj?->method()
来源：http://ppd.yvedp.cn

[U55] PHP：match 表达式
来源：http://jff.hcnkem.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://ycd.shanyushiyangkeji.top

[U56] PHP：命名参数
来源：http://cgc.svipenyu.cn

f(a: 1, b: 2)
来源：http://glx.xziqi.cn

[U57] PHP：字符串插值
来源：http://mhk.fanxiaobao.xyz

"值: {$a}"
来源：http://tjm.zhaomingkeji.xyz

[U58] PHP：数组三件套
来源：http://ezz.hongshengwenyu.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://anj.ybcxt.top

[U59] PHP：自定义排序
来源：http://jpw.haohaochexian.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kgg.jinyuanbaomall.cn

[U60] PHP：JSON 编解码
来源：http://ijy.316326.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://sth.cheryme.top

[U61] PHP：正则
来源：http://pex.tanke756.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://izx.snrcjt.cn

[U62] PHP：日期对象
来源：http://spj.hcnkem.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://olq.xuanzx.com

[U63] PHP：文件读写
来源：http://hkv.sxryk.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://eua.vehdjk.com

[U64] PHP：目录遍历
来源：http://kcc.jianghu66.top

glob("dir/*.php");  scandir("dir");
来源：http://tau.yangfankeji.com

[U65] PHP：会话
来源：http://whq.meibo888.top

session_start();  $_SESSION["uid"] = 1;
来源：http://wur.52xcode.cn

[U66] PHP：设置 Cookie
来源：http://hyf.yangfankeji.com

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://scu.nanxuanxn.top

[U67] PHP：处理文件上传
来源：http://xqe.guannengcc.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://uut.cucudq.cn

[U68] PHP：PDO 连接
来源：http://adf.316326.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://tbg.jinqigufen.top

[U69] PHP：PDO 预处理
来源：http://zes.vehdjk.com

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://yxy.xuetiantiany.cn

[U70] PHP：PDO 事务
来源：http://imp.epnwcf.com

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://stk.aibaodan.cn

[U71] PHP：抛出异常
来源：http://tmf.yanxiufei.cn

throw new RuntimeException("失败", 500);
来源：http://btz.nwbrower.top

[U72] PHP：写错误日志
来源：http://qqp.dashuyun.cn

error_log("失败: " . $e->getMessage());
来源：http://qdf.zdqjudy.top

[U73] PHP：读取 ini 配置
来源：http://deg.cucudq.cn

parse_ini_file("config.ini", true)
来源：http://oyq.fengsongda.top

[U74] PHP：读取环境变量
来源：http://cbf.ydzc1.top

getenv("APP_ENV") ?: "production"
来源：http://dbl.0kj1m.cn

[U75] PHP：依赖注入
来源：http://aws.birdmap.top

composer require psr/container
来源：http://lai.xziqi.cn

[U76] PHP：简单路由
来源：http://ecr.zhijiandao.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://kyb.tarul.cn

[U77] PHP：模板渲染
来源：http://rhf.jiagoushi.top

composer require twig/twig
来源：http://vlx.sysykeji.top

[U78] PHP：单元测试
来源：http://sds.zhixingplan.top

composer require --dev phpunit/phpunit
来源：http://lis.daxiang520.top

[U79] PHP：静态分析
来源：http://qdb.cheryme.top

composer require --dev phpstan/phpstan
来源：http://htt.xylfe.cn

[U80] PHP：代码规范修复
来源：http://gkv.pycfn.com

composer require --dev friendsofphp/php-cs-fixer
来源：http://mpl.hnqzz.top


<!-- 参考信息 -->