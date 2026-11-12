代发 wailian999

int size() const noexcept { return n_; }
来源：http://qpy.sjlbkw.cn

[S53] C++：移动语义
来源：http://xmj.ydzc1.top

std::vector<int> w = std::move(v);
来源：http://hle.iojbl.cn

[S54] C++：异常处理
来源：http://npt.bjfxy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dtz.jqgufenzy.top

[S55] C++：结构化绑定
来源：http://wup.guowangkeji.top

auto [a, b] = std::make_pair(1, 2);
来源：http://cko.fktsv.cn

[S56] C++：optional
来源：http://nsb.cheryme.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hyg.jlsjyb.cn

[S57] C++：编译期常量
来源：http://gvf.redwolf501.top

constexpr int N = 10;
来源：http://vtu.hammf.cn

[S58] C++：命名空间
来源：http://axj.zdqjudy.top

namespace ns { int f() { return 1; } }
来源：http://krv.zhaomingkeji.xyz

[S59] C++：静态断言
来源：http://kad.aizwys.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fsg.jlsjyb.cn

[S60] C++：遍历并删除元素
来源：http://tfa.dashuyun.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wyd.chenjidiqi.icu

================================================================================
来源：http://ygy.ehwqpu.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://oum.cashguo.top

================================================================================
来源：http://qvq.hcnkem.com

[T01] Kotlin：Hello World
来源：http://xwx.xuetiantiany.cn

println("Hello")
来源：http://ftd.jinghuilouyu.cn

[T02] Kotlin：变量
来源：http://fqh.yuxming.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zih.zhixingplan.top

[T03] Kotlin：字符串模板
来源：http://zqd.xziqi.cn

"值: $b"
来源：http://ohs.daxiang520.top

[T04] Kotlin：空安全
来源：http://tqw.yvedp.cn

val n: String? = null;  n?.length
来源：http://wak.zhiwuduotai.top

[T05] Kotlin：when 表达式
来源：http://czd.feifeiyinyue.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cix.gaohongyu789.top

[T06] Kotlin：集合映射
来源：http://cqi.gzhubu.top

listOf(1, 2, 3).map { it * 2 }
来源：http://xmh.fengsongda.top

[T07] Kotlin：集合过滤
来源：http://mtv.yonumen.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://arw.vqdsnc.cn

[T08] Kotlin：数据类
来源：http://ini.kuanghao11.cn

data class User(val name: String, val age: Int)
来源：http://cdq.yuanzhike.top

[T09] Kotlin：扩展函数
来源：http://coy.yj20258.top

fun String.exclaim() = this + "!"
来源：http://mld.hammf.cn

[T10] Kotlin：默认参数
来源：http://ctj.ctjpmb.com

fun greet(name: String = "World") = "Hi $name"
来源：http://zep.cashguo.top

[T11] Kotlin：协程
来源：http://uji.sweek.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://tzd.daria6918.cn

[T12] Kotlin：解构声明
来源：http://zay.ppjwa.cn

val (a, b) = Pair(1, 2)
来源：http://rbn.xziqi.cn

[T13] Kotlin：只读 Map
来源：http://mol.aibaodan.cn

val m = mapOf("a" to 1)
来源：http://agu.cucudq.cn

[T14] Kotlin：循环
来源：http://wcs.9152youxi.cn

for (i in 1..10) println(i)
来源：http://dsu.daria6918.cn

[T15] Kotlin：接口
来源：http://msj.ctjpmb.com

interface Shape { fun area(): Double }
来源：http://wsx.smart0.xyz

[T16] Swift：Hello World
来源：http://qby.birdmap.top

print("Hello")
来源：http://hqd.zdbjq.cn

[T17] Swift：变量与常量
来源：http://cyk.zhixingplan.top

var a = 1;  let b = 2
来源：http://ynh.sweek.top

[T18] Swift：字符串插值
来源：http://aho.shangyingyoupin.top

"值: \(b)"
来源：http://yek.andypj.xyz

[T19] Swift：可选绑定
来源：http://qfz.jlsjyb.cn

if let n = opt { print(n) }
来源：http://jgm.snrcjt.cn

[T20] Swift：数组操作
来源：http://lin.nwbrower.top

var a = [1, 2, 3];  a.append(4)
来源：http://nou.redwolf501.top

[T21] Swift：遍历
来源：http://qpa.shanyushiyangtech.top

for x in a { print(x) }
来源：http://xuu.shanyushiyangtech.top

[T22] Swift：字典
来源：http://fqa.xylfe.cn

var d = ["a": 1];  d["b"] = 2
来源：http://rwj.fzhhl.top

[T23] Swift：函数
来源：http://rfk.cashguo.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://uxw.kuanghao11.cn

[T24] Swift：闭包
来源：http://ppr.ctjpmb.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://yyw.jinyuanbaomall.cn

[T25] Swift：结构体
来源：http://duz.9152youxi.cn

struct P { var x: Int }
来源：http://eso.shanyushiyangkeji.top

[T26] Swift：类与重写
来源：http://whk.tian-w.cn

class A: Base { override func f() {} }
来源：http://ttt.gzhubu.top

[T27] Swift：错误处理
来源：http://grr.sjlbkw.cn

do { try f() } catch { print(error) }
来源：http://prs.zhixingplan.top

[T28] Swift：枚举
来源：http://zfb.wangdashe.top

enum Color { case red, green }
来源：http://wbi.hfpthk.cn

[T29] Swift：guard 提前返回
来源：http://ukn.zhoulong.xyz

guard let x = opt else { return }
来源：http://skl.xylfe.cn

[T30] Swift：协议
来源：http://prk.shanyushiyangtech.top

protocol Shape { func area() -> Double }
来源：http://ckv.cheryme.top

[T31] Lua：Hello World
来源：http://zmc.chenjidiqi.icu

print("Hello")
来源：http://hmw.haohaochexian.top

[T32] Lua：局部变量
来源：http://vqf.epnwcf.com

local a = 1
来源：http://pmc.nanxuanxn.top

[T33] Lua：表（数组）
来源：http://wdy.jinyuanbaomall.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wyw.zhijiandao.cn

[T34] Lua：遍历表
来源：http://vei.hammf.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rpi.aizwys.cn

[T35] Lua：字典表
来源：http://lls.0kj1m.cn

local d = { a = 1 };  d.b = 2
来源：http://kad.haohaochexian.top

[T36] Lua：函数
来源：http://ueh.jlsjyb.cn

function add(a, b) return a + b end
来源：http://glt.jinqigufen.top

[T37] Lua：字符串拼接
来源：http://yen.meibo888.top

"a" .. "b"
来源：http://bny.jqgfzy.top

[T38] Lua：条件
来源：http://blo.daxiang520.top

if x > 0 then print("正") end
来源：http://rom.iojbl.cn

[T39] Lua：模式匹配
来源：http://jme.smart0.xyz

string.find(s, "%d+")
来源：http://ktn.hcnkem.com

[T40] Lua：元表
来源：http://fpl.ehwqpu.com

setmetatable({}, { __index = base })
来源：http://lku.shuidangran.top

[T41] Perl：Hello World
来源：http://agq.xuetiantiany.cn

print "Hello\n";
来源：http://xrh.daria6918.cn

[T42] Perl：变量类型
来源：http://qtl.aibaodan.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pro.fzhhl.top

[T43] Perl：字符串插值
来源：http://noc.jiagoushi.top

"值: $a"
来源：http://xeu.yongpay.top

[T44] Perl：条件
来源：http://pug.jinghuilouyu.cn

if ($a > 0) { print "正"; }
来源：http://bgp.ydjk.org.cn

[T45] Perl：数组遍历
来源：http://dke.zdqjudy.top

for my $x (@arr) { print $x; }
来源：http://dhi.zdbjq.cn

[T46] Perl：哈希操作
来源：http://tyr.jqgfzy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qfl.tianlin.xyz

[T47] Perl：正则捕获
来源：http://xkj.gotoacloud.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://lfc.jyoumei.cn

[T48] Perl：正则替换
来源：http://irk.jqgfzy.top

$s =~ s/old/new/g;
来源：http://tyy.shanyushiyangtech.top

[T49] Perl：函数
来源：http://fyr.zhengqikj.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vjd.chenlongwang.top

[T50] Perl：逐行读文件
来源：http://ukf.yangfankeji.com

open my $fh, "<", "a.txt" or die $!;
来源：http://jac.sxryk.cn

while (my $line = <$fh>) { print $line; }
来源：http://tpp.ctjpmb.com

[T51] Scala：Hello World
来源：http://dch.jqgufenzy.top

println("Hello")
来源：http://ppy.jinqigfzy.top

[T52] Scala：变量
来源：http://hlb.sjlbkw.cn

val a = 1;  var b = 2
来源：http://rtx.316326.xyz

[T53] Scala：字符串插值
来源：http://xbk.shanyushiyangkeji.top

s"值: $b"
来源：http://fxq.vqdsnc.cn

[T54] Scala：集合映射
来源：http://ppa.hywenlv.cn

List(1, 2, 3).map(_ * 2)
来源：http://lbh.redwolf501.top

[T55] Scala：集合过滤
来源：http://sdr.hywenlv.cn

List(1, 2, 3).filter(_ > 1)
来源：http://uzu.snrcjt.cn

[T56] Scala：样例类
来源：http://gre.ctjpmb.com

case class User(name: String, age: Int)
来源：http://bse.xinyue.icu

[T57] Scala：模式匹配
来源：http://swa.yongpay.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://spc.52xcode.cn

[T58] Scala：函数定义
来源：http://hai.sweek.top

def add(a: Int, b: Int): Int = a + b
来源：http://jyh.zhaomingkeji.xyz

[T59] Scala：循环
来源：http://qss.svipenyu.cn

for (i <- 1 to 10) println(i)
来源：http://msm.jinyuanbaomall.cn

[T60] Scala：折叠
来源：http://rut.uphjek.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://pyg.gzhubu.top

================================================================================
来源：http://iih.ydzc1.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vfw.hongshengwenyu.top

================================================================================
来源：http://cmq.ydjk.org.cn

[U01] Py：创建虚拟环境
来源：http://uzm.ehwqpu.com

python -m venv .venv && source .venv/bin/activate
来源：http://kvs.yuanzhike.top

[U02] Py：导出 / 安装依赖
来源：http://rkz.yongpay.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qns.jinghuilouyu.cn

[U03] Py：加载 .env 配置
来源：http://otq.hongshengwenyu.top

from dotenv import load_dotenv; load_dotenv()
来源：http://xyy.smart0.xyz

[U04] Py：变量调试打印
来源：http://mpy.hammf.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ruo.vehdjk.com

[U05] Py：列表去重且保序
来源：http://fjg.daria6918.cn

list(dict.fromkeys(arr))
来源：http://xzj.nwbrower.top

[U06] Py：合并两个字典
来源：http://luu.c1oappe.top

{**a, **b}
来源：http://eci.ydjk.org.cn

[U07] Py：反转字典键值
来源：http://gao.gotoacloud.top

{v: k for k, v in d.items()}
来源：http://ywg.zhengqikj.top

[U08] Py：展平二维列表
来源：http://wdn.zhiwuduotai.top

[y for x in nested for y in x]
来源：http://jxh.aibaodan.cn

[U09] Py：字典取最大值的键
来源：http://hfb.sysykeji.top

max(d, key=d.get)
来源：http://oko.yuxming.cn

[U10] Py：按值排序字典
来源：http://cup.52xcode.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lyx.redwolf501.top

[U11] Py：生成器表达式
来源：http://hye.epnwcf.com

(x * 2 for x in arr)
来源：http://nuc.hnqzz.top

[U12] Py：取出现最多的 3 个元素
来源：http://hsj.zhengqikj.top

Counter(arr).most_common(3)
来源：http://dhg.hesvh.cn

[U13] Py：固定长度队列
来源：http://pfu.kuanghao11.cn

deque(maxlen=10)
来源：http://mla.xziqi.cn

[U14] Py：分组收集到列表
来源：http://fnc.ydjk.org.cn

defaultdict(list)
来源：http://qpm.tanke756.top

[U15] Py：高精度计时
来源：http://htu.tarul.cn

t = time.perf_counter()
来源：http://uhn.fanxiaobao.xyz

[U16] Py：命令行参数解析
来源：http://anz.svipenyu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ped.iojbl.cn

[U17] Py：初始化日志
来源：http://rsc.tanke756.top

logging.basicConfig(level=logging.INFO)
来源：http://xrz.sweek.top

[U18] Py：预编译正则
来源：http://wnj.yvedp.cn

pat = re.compile(r"\d+")
来源：http://wsw.yonumen.top

[U19] Py：正则替换带回调
来源：http://ghx.tanke756.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://cge.tanke756.top

[U20] Py：缓存函数结果
来源：http://dqx.gogol.net.cn

@functools.lru_cache(maxsize=None)
来源：http://wsc.hesvh.cn

[U21] Py：自定义上下文管理器
来源：http://kwb.uphjek.com

@contextlib.contextmanager
来源：http://ean.fzhhl.top

[U22] Py：矩阵转置
来源：http://hku.gogol.net.cn

list(zip(*m))
来源：http://wqx.fengsongda.top

[U23] Py：分块读取大文件
来源：http://npo.fehbvm.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://kyh.fktsv.cn

[U24] Py：路径操作
来源：http://mbf.fktsv.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tdz.jinyuanbaomall.cn

[U25] Py：CSV 按字典读
来源：http://spc.jinyuanbaomall.cn

csv.DictReader(f)
来源：http://mfp.guowangkeji.top

[U26] Py：并发下载
来源：http://umx.shzxlz.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://irx.shanyushiyangkeji.top

[U27] Py：异步 HTTP
来源：http://zdo.yangfankeji.com

aiohttp.ClientSession() 配合 async with
来源：http://vva.shuidangran.top

[U28] Py：类型别名
来源：http://ewo.hysaishi.cn

UserId = int
来源：http://rwo.hnxiangtu.top

[U29] Py：属性校验
来源：http://vlq.meibo888.top

@property 与 @x.setter 配合
来源：http://efr.c1oappe.top

[U30] Py：数据类
来源：http://ucv.fanxiaobao.xyz

@dataclass(slots=True)
来源：http://gnv.fanxiaobao.xyz

[U31] Py：单测
来源：http://oee.yj20258.top

python -m pytest -q
来源：http://ijt.ehwqpu.com

[U32] Py：代码格式化
来源：http://vyx.ywan-chungtsiang.top

ruff format . && ruff check --fix .
来源：http://soi.ydjk.org.cn

[U33] Py：打包发布
来源：http://ixx.yfazqb.com

python -m build  （依赖 pyproject.toml）
来源：http://igq.yj20258888.top

[U34] Py：判断编码
来源：http://sjr.yj20258888.top

chardet.detect(raw)
来源：http://kju.epnwcf.com

[U35] Py：发送邮件
来源：http://iuz.haohaochexian.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tqf.dianchejie.cn

[U36] Py：定时任务
来源：http://wrb.ivvv.top

schedule.every(10).minutes.do(job)
来源：http://lel.cashguo.top

[U37] Py：读写 Excel
来源：http://dft.fengsongda.top

pandas.read_excel / DataFrame.to_excel
来源：http://eyo.mhx1999.top

[U38] Py：获取脚本所在目录
来源：http://oio.daxiang520.top

Path(__file__).resolve().parent
来源：http://dta.shangyingyoupin.top

[U39] Py：判断是否在交互环境
来源：http://kyg.52xcode.cn

sys.stdout.isatty()
来源：http://log.chenlongwang.top

[U40] Py：打印到标准错误
来源：http://xfg.vqdsnc.cn

print("err", file=sys.stderr)
来源：http://hfu.yj202588.top

[U41] PHP：初始化 Composer 项目
来源：http://ing.xziqi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ybv.ctjpmb.com

[U42] PHP：PSR-4 自动加载
来源：http://exe.jinghuilouyu.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xju.kuanghao11.cn

[U43] PHP：声明命名空间
来源：http://nuo.fehbvm.com

namespace App\Http;
来源：http://ktv.tian-w.cn

[U44] PHP：开启严格类型
来源：http://zdo.bbcook.cn

declare(strict_types=1);
来源：http://vyt.jinyuanbaomall.cn

[U45] PHP：类型声明与返回类型
来源：http://rcn.daxiang520.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://cmg.jinghuilouyu.cn

[U46] PHP：可空类型
来源：http://goy.wangdashe.top

?string $name = null
来源：http://owr.fanxiaobao.xyz

[U47] PHP：联合类型
来源：http://ilv.sweek.top

int|string $id
来源：http://nbz.aizwys.cn

[U48] PHP：纯枚举
来源：http://pgy.aizwys.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wtm.zhoulong.xyz

[U49] PHP：只读属性
来源：http://ile.vqdsnc.cn

public readonly string $name
来源：http://vyl.xziqi.cn

[U50] PHP：构造器属性提升
来源：http://vzg.xuetiantiany.cn

public function __construct(private int $id) {}
来源：http://lcy.cucudq.cn

[U51] PHP：数组解构
来源：http://fxo.gzhubu.top

[$a, $b] = $arr;
来源：http://now.dianchejie.cn

[U52] PHP：箭头函数
来源：http://zcy.zhixingplan.top

$double = fn($x) => $x * 2;
来源：http://frt.hcnkem.com

[U53] PHP：空合并运算符
来源：http://hya.gotoacloud.top

$v = $a ?? $b ?? "default";
来源：http://eqf.uphjek.com

[U54] PHP：空安全调用
来源：http://htf.hammf.cn

$obj?->method()
来源：http://clf.fanxiaobao.xyz

[U55] PHP：match 表达式
来源：http://txp.0kj1m.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://nxj.bbcook.cn

[U56] PHP：命名参数
来源：http://mct.shangyingyoupin.top

f(a: 1, b: 2)
来源：http://dzy.feifeiyinyue.top

[U57] PHP：字符串插值
来源：http://ing.jianghu66.top

"值: {$a}"
来源：http://bbi.jinghuilouyu.cn

[U58] PHP：数组三件套
来源：http://kvs.aibaodan.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://foc.zdbjq.cn

[U59] PHP：自定义排序
来源：http://krt.hysaishi.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://may.gzhubu.top

[U60] PHP：JSON 编解码
来源：http://ttz.redwolf501.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://txg.ehwqpu.com

[U61] PHP：正则
来源：http://bad.0kj1m.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hkm.bbcook.cn

[U62] PHP：日期对象
来源：http://hmp.zycfv.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mqn.xuanzx.com

[U63] PHP：文件读写
来源：http://azn.pycfn.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://fkd.shangyingyoupin.top

[U64] PHP：目录遍历
来源：http://pad.jyoumei.cn

glob("dir/*.php");  scandir("dir");
来源：http://ihp.kuanghao11.cn

[U65] PHP：会话
来源：http://obz.wangdashe.top

session_start();  $_SESSION["uid"] = 1;
来源：http://pfa.pycfn.com

[U66] PHP：设置 Cookie
来源：http://xwi.ydjk.org.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qtm.pengpengdd.cyou

[U67] PHP：处理文件上传
来源：http://tif.birdmap.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://lpb.meibo888.top

[U68] PHP：PDO 连接
来源：http://fer.smart0.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://skt.feifeiyinyue.top

[U69] PHP：PDO 预处理
来源：http://hor.hnqzz.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://lne.xinyue.icu

[U70] PHP：PDO 事务
来源：http://vut.guannengcc.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://tju.jinghuilouyu.cn

[U71] PHP：抛出异常
来源：http://mqj.fengsongda.top

throw new RuntimeException("失败", 500);
来源：http://ksg.sjlbkw.cn

[U72] PHP：写错误日志
来源：http://odd.sysykeji.top

error_log("失败: " . $e->getMessage());
来源：http://vca.shanyushiyangkeji.top

[U73] PHP：读取 ini 配置
来源：http://iys.jqgufenzy.top

parse_ini_file("config.ini", true)
来源：http://ump.sjlbkw.cn

[U74] PHP：读取环境变量
来源：http://jzb.aibaodan.cn

getenv("APP_ENV") ?: "production"
来源：http://huu.pengpengdd.cyou

[U75] PHP：依赖注入
来源：http://fog.feifeiyinyue.top

composer require psr/container
来源：http://qvx.hnqzz.top

[U76] PHP：简单路由
来源：http://ltd.chenlongwang.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qcx.shanyushiyangkeji.top

[U77] PHP：模板渲染
来源：http://xcv.52xcode.cn

composer require twig/twig
来源：http://hgw.jinghuilouyu.cn

[U78] PHP：单元测试
来源：http://kcz.chenjidiqi.icu

composer require --dev phpunit/phpunit
来源：http://qbj.kuanghao11.cn


<!-- 参考信息 -->