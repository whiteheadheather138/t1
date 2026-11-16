代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://foz.jinqigfzy.top

[S55] C++：结构化绑定
来源：http://nme.jinyuanbaomall.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zyl.shanyushiyangtech.top

[S56] C++：optional
来源：http://kgh.zhiwuduotai.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nxq.jqgufenzy.top

[S57] C++：编译期常量
来源：http://prt.daxiang520.top

constexpr int N = 10;
来源：http://eig.hfpthk.cn

[S58] C++：命名空间
来源：http://vjt.fanxiaobao.xyz

namespace ns { int f() { return 1; } }
来源：http://uek.zdbjq.cn

[S59] C++：静态断言
来源：http://fyj.sweek.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://boo.epnwcf.com

[S60] C++：遍历并删除元素
来源：http://yfp.zdqjudy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dwf.aizwys.cn

================================================================================
来源：http://yzy.yanxiufei.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qkn.snrcjt.cn

================================================================================
来源：http://bzo.kuanghao11.cn

[T01] Kotlin：Hello World
来源：http://awn.fehbvm.com

println("Hello")
来源：http://jgx.hnqzz.top

[T02] Kotlin：变量
来源：http://xxw.xuetiantiany.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://omn.shanyushiyangtech.top

[T03] Kotlin：字符串模板
来源：http://mxy.andypj.xyz

"值: $b"
来源：http://wcf.hnxiangtu.top

[T04] Kotlin：空安全
来源：http://jlg.pycfn.com

val n: String? = null;  n?.length
来源：http://qcm.ybcxt.top

[T05] Kotlin：when 表达式
来源：http://hrl.xingfuxueyuan.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xkd.hnxiangtu.top

[T06] Kotlin：集合映射
来源：http://qqr.redwolf501.top

listOf(1, 2, 3).map { it * 2 }
来源：http://wxr.redwolf501.top

[T07] Kotlin：集合过滤
来源：http://xtc.redwolf501.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://mqh.quarkkingdee.top

[T08] Kotlin：数据类
来源：http://xkl.c1oappe.top

data class User(val name: String, val age: Int)
来源：http://lpp.dianchejie.cn

[T09] Kotlin：扩展函数
来源：http://jei.cqqwz.cn

fun String.exclaim() = this + "!"
来源：http://bnb.yvedp.cn

[T10] Kotlin：默认参数
来源：http://vvj.jyoumei.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://owx.pycfn.com

[T11] Kotlin：协程
来源：http://cuj.zhoulong.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://jkm.havefunace.top

[T12] Kotlin：解构声明
来源：http://irf.yueranfly.top

val (a, b) = Pair(1, 2)
来源：http://nna.dianchejie.cn

[T13] Kotlin：只读 Map
来源：http://fxg.jyoumei.cn

val m = mapOf("a" to 1)
来源：http://akk.hammf.cn

[T14] Kotlin：循环
来源：http://smx.tanke756.top

for (i in 1..10) println(i)
来源：http://sri.jinqigfzy.top

[T15] Kotlin：接口
来源：http://pxu.52xcode.cn

interface Shape { fun area(): Double }
来源：http://awm.gaohongyu789.top

[T16] Swift：Hello World
来源：http://jcf.hnxiangtu.top

print("Hello")
来源：http://iws.bbcook.cn

[T17] Swift：变量与常量
来源：http://jee.xziqi.cn

var a = 1;  let b = 2
来源：http://uny.meibo888.top

[T18] Swift：字符串插值
来源：http://scn.hammf.cn

"值: \(b)"
来源：http://phw.yueranfly.top

[T19] Swift：可选绑定
来源：http://lgs.hnxiangtu.top

if let n = opt { print(n) }
来源：http://xhl.xziqi.cn

[T20] Swift：数组操作
来源：http://kpa.yangfankeji.com

var a = [1, 2, 3];  a.append(4)
来源：http://bso.xinyue.icu

[T21] Swift：遍历
来源：http://bqf.jqgufenzy.top

for x in a { print(x) }
来源：http://fsu.fehbvm.com

[T22] Swift：字典
来源：http://dsb.sufxvd.cn

var d = ["a": 1];  d["b"] = 2
来源：http://sud.gaohongyu789.top

[T23] Swift：函数
来源：http://fya.shzxlz.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nqi.316326.xyz

[T24] Swift：闭包
来源：http://lwk.hywenlv.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vfu.havefunace.top

[T25] Swift：结构体
来源：http://zmd.ctjpmb.com

struct P { var x: Int }
来源：http://hxp.xylfe.cn

[T26] Swift：类与重写
来源：http://ara.andypj.xyz

class A: Base { override func f() {} }
来源：http://nqs.yueranfly.top

[T27] Swift：错误处理
来源：http://xqw.zycfv.cn

do { try f() } catch { print(error) }
来源：http://xkd.andypj.xyz

[T28] Swift：枚举
来源：http://zmf.hywenlv.cn

enum Color { case red, green }
来源：http://fsp.hysaishi.cn

[T29] Swift：guard 提前返回
来源：http://ctk.yj20258888.top

guard let x = opt else { return }
来源：http://ubg.haohaochexian.top

[T30] Swift：协议
来源：http://rjh.fehbvm.com

protocol Shape { func area() -> Double }
来源：http://kxu.yueranfly.top

[T31] Lua：Hello World
来源：http://zzw.tanke756.top

print("Hello")
来源：http://abj.aizwys.cn

[T32] Lua：局部变量
来源：http://eyh.daxiang520.top

local a = 1
来源：http://ymm.jinqigufen.top

[T33] Lua：表（数组）
来源：http://vtb.bbcook.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://izm.tarul.cn

[T34] Lua：遍历表
来源：http://qup.fanxiaobao.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://oce.bjfxy.top

[T35] Lua：字典表
来源：http://lcd.jiagoushi.top

local d = { a = 1 };  d.b = 2
来源：http://prt.sxryk.cn

[T36] Lua：函数
来源：http://twt.iojbl.cn

function add(a, b) return a + b end
来源：http://bsa.jinghuilouyu.cn

[T37] Lua：字符串拼接
来源：http://tmx.jinghuilouyu.cn

"a" .. "b"
来源：http://gwk.birdmap.top

[T38] Lua：条件
来源：http://yha.ybcxt.top

if x > 0 then print("正") end
来源：http://fzu.tian-w.cn

[T39] Lua：模式匹配
来源：http://swm.hfpthk.cn

string.find(s, "%d+")
来源：http://ofd.redwolf501.top

[T40] Lua：元表
来源：http://gfv.ywan-chungtsiang.top

setmetatable({}, { __index = base })
来源：http://jlm.yueranfly.top

[T41] Perl：Hello World
来源：http://uey.epnwcf.com

print "Hello\n";
来源：http://lgq.epnwcf.com

[T42] Perl：变量类型
来源：http://mgc.yonumen.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://meh.zhiwuduotai.top

[T43] Perl：字符串插值
来源：http://jde.pengpengdd.cyou

"值: $a"
来源：http://ojj.316326.xyz

[T44] Perl：条件
来源：http://vbp.jinqigfzy.top

if ($a > 0) { print "正"; }
来源：http://nab.hcnkem.com

[T45] Perl：数组遍历
来源：http://qni.jqgfzy.top

for my $x (@arr) { print $x; }
来源：http://gxm.zhongyouzk.top

[T46] Perl：哈希操作
来源：http://fmg.yanxiufei.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wzz.zhengqikj.top

[T47] Perl：正则捕获
来源：http://ufs.vehdjk.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://gys.dashuyun.cn

[T48] Perl：正则替换
来源：http://hva.dianchejie.cn

$s =~ s/old/new/g;
来源：http://rex.c1oappe.top

[T49] Perl：函数
来源：http://xjr.epnwcf.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jiy.yongpay.top

[T50] Perl：逐行读文件
来源：http://ymb.sxryk.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://eal.yanxiufei.cn

while (my $line = <$fh>) { print $line; }
来源：http://qvb.feifeiyinyue.top

[T51] Scala：Hello World
来源：http://zhc.pycfn.com

println("Hello")
来源：http://lqj.yueranfly.top

[T52] Scala：变量
来源：http://xpc.jinyuanbaomall.cn

val a = 1;  var b = 2
来源：http://bkj.ehwqpu.com

[T53] Scala：字符串插值
来源：http://puk.ehwqpu.com

s"值: $b"
来源：http://dfq.wangshuangyany.cn

[T54] Scala：集合映射
来源：http://ivc.jinghuilouyu.cn

List(1, 2, 3).map(_ * 2)
来源：http://ixm.gogol.net.cn

[T55] Scala：集合过滤
来源：http://bha.gzhubu.top

List(1, 2, 3).filter(_ > 1)
来源：http://oyo.shangyingyoupin.top

[T56] Scala：样例类
来源：http://iix.xuetiantiany.cn

case class User(name: String, age: Int)
来源：http://yxn.cucudq.cn

[T57] Scala：模式匹配
来源：http://zzn.guannengcc.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://qvc.guannengcc.top

[T58] Scala：函数定义
来源：http://oco.kuanghao11.cn

def add(a: Int, b: Int): Int = a + b
来源：http://boq.shanyushiyangkeji.top

[T59] Scala：循环
来源：http://mmg.hywenlv.cn

for (i <- 1 to 10) println(i)
来源：http://ynf.daxiang520.top

[T60] Scala：折叠
来源：http://fvi.quarkkingdee.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tpv.jqgfzy.top

================================================================================
来源：http://kbn.feifeiyinyue.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hgl.xingfuxueyuan.xyz

================================================================================
来源：http://vcm.ctjpmb.com

[U01] Py：创建虚拟环境
来源：http://ykg.yongpay.top

python -m venv .venv && source .venv/bin/activate
来源：http://bqq.ctjpmb.com

[U02] Py：导出 / 安装依赖
来源：http://xmo.uphjek.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dtu.cheryme.top

[U03] Py：加载 .env 配置
来源：http://bhe.ctjpmb.com

from dotenv import load_dotenv; load_dotenv()
来源：http://dna.shangyingyoupin.top

[U04] Py：变量调试打印
来源：http://fdq.aizwys.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hnl.ydjk.org.cn

[U05] Py：列表去重且保序
来源：http://bou.gotoacloud.top

list(dict.fromkeys(arr))
来源：http://wam.gzhubu.top

[U06] Py：合并两个字典
来源：http://alx.jianghu66.top

{**a, **b}
来源：http://llh.fktsv.cn

[U07] Py：反转字典键值
来源：http://qwl.daxiang520.top

{v: k for k, v in d.items()}
来源：http://nls.zdbjq.cn

[U08] Py：展平二维列表
来源：http://whu.yongpay.top

[y for x in nested for y in x]
来源：http://fvq.sysykeji.top

[U09] Py：字典取最大值的键
来源：http://tpc.jqgfzy.top

max(d, key=d.get)
来源：http://pgd.shanyushiyangkeji.top

[U10] Py：按值排序字典
来源：http://wrk.cqqwz.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://grx.0kj1m.cn

[U11] Py：生成器表达式
来源：http://wnu.cashguo.top

(x * 2 for x in arr)
来源：http://ril.zhixingplan.top

[U12] Py：取出现最多的 3 个元素
来源：http://rzd.kuanghao11.cn

Counter(arr).most_common(3)
来源：http://wgg.jqgufenzy.top

[U13] Py：固定长度队列
来源：http://whv.hongshengwenyu.top

deque(maxlen=10)
来源：http://kpb.yueranfly.top

[U14] Py：分组收集到列表
来源：http://wsz.zhengqikj.top

defaultdict(list)
来源：http://hik.bbcook.cn

[U15] Py：高精度计时
来源：http://pil.wangshuangyany.cn

t = time.perf_counter()
来源：http://pfq.ydjk.org.cn

[U16] Py：命令行参数解析
来源：http://tfo.zdbjq.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://rln.cashguo.top

[U17] Py：初始化日志
来源：http://nds.sjlbkw.cn

logging.basicConfig(level=logging.INFO)
来源：http://hec.vqdsnc.cn

[U18] Py：预编译正则
来源：http://yus.dashuyun.cn

pat = re.compile(r"\d+")
来源：http://ete.9152youxi.cn

[U19] Py：正则替换带回调
来源：http://dhm.hesvh.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://vjh.hnqzz.top

[U20] Py：缓存函数结果
来源：http://jtl.yj202588.top

@functools.lru_cache(maxsize=None)
来源：http://dif.redwolf501.top

[U21] Py：自定义上下文管理器
来源：http://cmf.316326.xyz

@contextlib.contextmanager
来源：http://cgk.shuidangran.top

[U22] Py：矩阵转置
来源：http://pqn.tanke756.top

list(zip(*m))
来源：http://iom.jinghuilouyu.cn

[U23] Py：分块读取大文件
来源：http://svm.yvedp.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pav.yj202588.top

[U24] Py：路径操作
来源：http://vrf.meibo888.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://frc.shangyingyoupin.top

[U25] Py：CSV 按字典读
来源：http://gfv.dianchejie.cn

csv.DictReader(f)
来源：http://dmb.hcnkem.com

[U26] Py：并发下载
来源：http://bjk.hammf.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xel.quarkkingdee.top

[U27] Py：异步 HTTP
来源：http://all.sysykeji.top

aiohttp.ClientSession() 配合 async with
来源：http://ust.havefunace.top

[U28] Py：类型别名
来源：http://gip.guowangkeji.top

UserId = int
来源：http://afd.chenzaomai.com

[U29] Py：属性校验
来源：http://yrb.zhengqikj.top

@property 与 @x.setter 配合
来源：http://zui.aibaodan.cn

[U30] Py：数据类
来源：http://cam.chenlongwang.top

@dataclass(slots=True)
来源：http://hfp.cdnleiting.top

[U31] Py：单测
来源：http://fwg.fengsongda.top

python -m pytest -q
来源：http://nqq.fzhhl.top

[U32] Py：代码格式化
来源：http://zlj.yfazqb.com

ruff format . && ruff check --fix .
来源：http://bhl.uphjek.com

[U33] Py：打包发布
来源：http://kct.xylfe.cn

python -m build  （依赖 pyproject.toml）
来源：http://sxg.birdmap.top

[U34] Py：判断编码
来源：http://njp.ivvv.top

chardet.detect(raw)
来源：http://ysl.iojbl.cn

[U35] Py：发送邮件
来源：http://rtt.epnwcf.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ync.nanxuanxn.top

[U36] Py：定时任务
来源：http://hjd.fehbvm.com

schedule.every(10).minutes.do(job)
来源：http://lzt.sufxvd.cn

[U37] Py：读写 Excel
来源：http://jpm.hfpthk.cn

pandas.read_excel / DataFrame.to_excel
来源：http://nok.yonumen.top

[U38] Py：获取脚本所在目录
来源：http://tsb.tian-w.cn

Path(__file__).resolve().parent
来源：http://xtc.aizwys.cn

[U39] Py：判断是否在交互环境
来源：http://igj.jinyuanbaomall.cn

sys.stdout.isatty()
来源：http://sjj.nanxinkj.top

[U40] Py：打印到标准错误
来源：http://pil.mhx1999.top

print("err", file=sys.stderr)
来源：http://koy.zhengqikj.top

[U41] PHP：初始化 Composer 项目
来源：http://gqy.epnwcf.com

composer init;  composer require guzzlehttp/guzzle
来源：http://bea.guowangkeji.top

[U42] PHP：PSR-4 自动加载
来源：http://bpw.yj20258.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qvr.52xcode.cn

[U43] PHP：声明命名空间
来源：http://fna.redwolf501.top

namespace App\Http;
来源：http://ksa.shzxlz.cn

[U44] PHP：开启严格类型
来源：http://bxf.fehbvm.com

declare(strict_types=1);
来源：http://add.ctjpmb.com

[U45] PHP：类型声明与返回类型
来源：http://ggs.guowangkeji.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://get.316326.xyz

[U46] PHP：可空类型
来源：http://efo.gotoacloud.top

?string $name = null
来源：http://ptt.quarkkingdee.top

[U47] PHP：联合类型
来源：http://pcc.sjlbkw.cn

int|string $id
来源：http://slo.tarul.cn

[U48] PHP：纯枚举
来源：http://tzk.vehdjk.com

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://zkp.yonumen.top

[U49] PHP：只读属性
来源：http://mmi.xingfuxueyuan.xyz

public readonly string $name
来源：http://yab.nwbrower.top

[U50] PHP：构造器属性提升
来源：http://tmk.tianlin.xyz

public function __construct(private int $id) {}
来源：http://ozr.nwbrower.top

[U51] PHP：数组解构
来源：http://ojz.chenlongwang.top

[$a, $b] = $arr;
来源：http://wbs.bbcook.cn

[U52] PHP：箭头函数
来源：http://hde.epnwcf.com

$double = fn($x) => $x * 2;
来源：http://qcb.aibaodan.cn

[U53] PHP：空合并运算符
来源：http://avu.yvedp.cn

$v = $a ?? $b ?? "default";
来源：http://tra.fzhhl.top

[U54] PHP：空安全调用
来源：http://zev.nanxinkj.top

$obj?->method()
来源：http://emu.hesvh.cn

[U55] PHP：match 表达式
来源：http://fzp.mhx1999.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://obo.xziqi.cn

[U56] PHP：命名参数
来源：http://wkq.dashuyun.cn

f(a: 1, b: 2)
来源：http://syq.gzhubu.top

[U57] PHP：字符串插值
来源：http://vrx.hnxiangtu.top

"值: {$a}"
来源：http://kai.hywenlv.cn

[U58] PHP：数组三件套
来源：http://ihv.daria6918.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ums.jinqigufen.top

[U59] PHP：自定义排序
来源：http://xbf.yueranfly.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ecx.chenlongwang.top

[U60] PHP：JSON 编解码
来源：http://znz.ydzc1.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://fsy.jinqigufen.top

[U61] PHP：正则
来源：http://ios.uphjek.com

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://akl.0kj1m.cn

[U62] PHP：日期对象
来源：http://hyy.yonumen.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://oqh.nanxuanxn.top

[U63] PHP：文件读写
来源：http://tqc.zhiwuduotai.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wcq.jianghu66.top

[U64] PHP：目录遍历
来源：http://fju.hysaishi.cn

glob("dir/*.php");  scandir("dir");
来源：http://iyg.hnxiangtu.top

[U65] PHP：会话
来源：http://siz.tarul.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://cwo.jinqigufen.top

[U66] PHP：设置 Cookie
来源：http://rno.jinqigufen.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jhb.xylfe.cn

[U67] PHP：处理文件上传
来源：http://idk.fengsongda.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://zuh.gogol.net.cn

[U68] PHP：PDO 连接
来源：http://kbk.uphjek.com

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xbm.tarul.cn

[U69] PHP：PDO 预处理
来源：http://ogd.shanyushiyangkeji.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://kdx.gotoacloud.top

[U70] PHP：PDO 事务
来源：http://mat.hfpthk.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://xsq.yfazqb.com

[U71] PHP：抛出异常
来源：http://nlf.jiagoushi.top

throw new RuntimeException("失败", 500);
来源：http://gyk.guowangkeji.top

[U72] PHP：写错误日志
来源：http://hfi.fktsv.cn

error_log("失败: " . $e->getMessage());
来源：http://lxc.c1oappe.top

[U73] PHP：读取 ini 配置
来源：http://zwi.shanyushiyangkeji.top

parse_ini_file("config.ini", true)
来源：http://jnd.yj202588.top

[U74] PHP：读取环境变量
来源：http://qbv.havefunace.top

getenv("APP_ENV") ?: "production"
来源：http://vqx.zhijiandao.cn

[U75] PHP：依赖注入
来源：http://vpd.hywenlv.cn

composer require psr/container
来源：http://zex.snrcjt.cn

[U76] PHP：简单路由
来源：http://kuq.jiagoushi.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pbg.sufxvd.cn

[U77] PHP：模板渲染
来源：http://asn.gzhubu.top

composer require twig/twig
来源：http://tee.yangfankeji.com

[U78] PHP：单元测试
来源：http://mza.shuidangran.top

composer require --dev phpunit/phpunit
来源：http://bag.vqdsnc.cn

[U79] PHP：静态分析
来源：http://eby.yonumen.top

composer require --dev phpstan/phpstan
来源：http://phl.chenzaomai.com

[U80] PHP：代码规范修复
来源：http://rgp.ybcxt.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://qri.hammf.cn


<!-- 参考信息 -->