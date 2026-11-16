代发 wailian999

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cbq.hesvh.cn

[S55] C++：结构化绑定
来源：http://fzb.hywenlv.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vrf.haohaochexian.top

[S56] C++：optional
来源：http://fsj.yj20258888.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kgg.zhengqikj.top

[S57] C++：编译期常量
来源：http://dmt.sysykeji.top

constexpr int N = 10;
来源：http://fnv.jyoumei.cn

[S58] C++：命名空间
来源：http://lcy.jqgufenzy.top

namespace ns { int f() { return 1; } }
来源：http://cbk.feifeiyinyue.top

[S59] C++：静态断言
来源：http://wbc.zdqjudy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yrq.snrcjt.cn

[S60] C++：遍历并删除元素
来源：http://oel.meibo888.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://odq.zdqjudy.top

================================================================================
来源：http://tvq.yanxiufei.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fpm.zhoulong.xyz

================================================================================
来源：http://qws.ctjpmb.com

[T01] Kotlin：Hello World
来源：http://tri.yuanzhike.top

println("Hello")
来源：http://dbv.quarkkingdee.top

[T02] Kotlin：变量
来源：http://djt.andypj.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qyi.bbcook.cn

[T03] Kotlin：字符串模板
来源：http://ayi.fengsongda.top

"值: $b"
来源：http://zhm.kuanghao11.cn

[T04] Kotlin：空安全
来源：http://mss.dashuyun.cn

val n: String? = null;  n?.length
来源：http://zah.bjfxy.top

[T05] Kotlin：when 表达式
来源：http://tir.52xcode.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cxe.fehbvm.com

[T06] Kotlin：集合映射
来源：http://oti.sysykeji.top

listOf(1, 2, 3).map { it * 2 }
来源：http://wfz.fanxiaobao.xyz

[T07] Kotlin：集合过滤
来源：http://owc.pycfn.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://yll.jiagoushi.top

[T08] Kotlin：数据类
来源：http://ynz.yangfankeji.com

data class User(val name: String, val age: Int)
来源：http://wnv.daxiang520.top

[T09] Kotlin：扩展函数
来源：http://kqm.dianchejie.cn

fun String.exclaim() = this + "!"
来源：http://qpi.xuetiantiany.cn

[T10] Kotlin：默认参数
来源：http://orb.redwolf501.top

fun greet(name: String = "World") = "Hi $name"
来源：http://wch.chenlongwang.top

[T11] Kotlin：协程
来源：http://usm.yj20258888.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://mez.yueranfly.top

[T12] Kotlin：解构声明
来源：http://xfh.snrcjt.cn

val (a, b) = Pair(1, 2)
来源：http://ygq.aibaodan.cn

[T13] Kotlin：只读 Map
来源：http://nho.ctjpmb.com

val m = mapOf("a" to 1)
来源：http://tyi.ppjwa.cn

[T14] Kotlin：循环
来源：http://qmz.yj20258.top

for (i in 1..10) println(i)
来源：http://gxw.cheryme.top

[T15] Kotlin：接口
来源：http://htw.sxryk.cn

interface Shape { fun area(): Double }
来源：http://dpb.jlsjyb.cn

[T16] Swift：Hello World
来源：http://xpl.zhixingplan.top

print("Hello")
来源：http://ouq.yvedp.cn

[T17] Swift：变量与常量
来源：http://mok.dianchejie.cn

var a = 1;  let b = 2
来源：http://pjh.havefunace.top

[T18] Swift：字符串插值
来源：http://xbj.gogol.net.cn

"值: \(b)"
来源：http://wop.daxiang520.top

[T19] Swift：可选绑定
来源：http://hwo.nanxuanxn.top

if let n = opt { print(n) }
来源：http://zgs.mhx1999.top

[T20] Swift：数组操作
来源：http://xek.hysaishi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://kwq.ehwqpu.com

[T21] Swift：遍历
来源：http://hxc.hcnkem.com

for x in a { print(x) }
来源：http://zwz.mhx1999.top

[T22] Swift：字典
来源：http://yvu.daxiang520.top

var d = ["a": 1];  d["b"] = 2
来源：http://jji.yj20258888.top

[T23] Swift：函数
来源：http://qdw.kuanghao11.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wso.shzxlz.cn

[T24] Swift：闭包
来源：http://vjk.zycfv.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gxf.tanke756.top

[T25] Swift：结构体
来源：http://ovm.iojbl.cn

struct P { var x: Int }
来源：http://nbu.jinqigfzy.top

[T26] Swift：类与重写
来源：http://txr.fanxiaobao.xyz

class A: Base { override func f() {} }
来源：http://jtx.xingfuxueyuan.xyz

[T27] Swift：错误处理
来源：http://uby.yuxming.cn

do { try f() } catch { print(error) }
来源：http://sfc.cucudq.cn

[T28] Swift：枚举
来源：http://eyp.zhijiandao.cn

enum Color { case red, green }
来源：http://lqv.yfazqb.com

[T29] Swift：guard 提前返回
来源：http://iep.zhongyouzk.top

guard let x = opt else { return }
来源：http://rgf.aibaodan.cn

[T30] Swift：协议
来源：http://whu.zhongyouzk.top

protocol Shape { func area() -> Double }
来源：http://byh.hywenlv.cn

[T31] Lua：Hello World
来源：http://mdw.kuanghao11.cn

print("Hello")
来源：http://shz.daxiang520.top

[T32] Lua：局部变量
来源：http://cna.yongpay.top

local a = 1
来源：http://crp.chenjidiqi.icu

[T33] Lua：表（数组）
来源：http://rbl.zhongyouzk.top

local t = {1, 2, 3};  t[4] = 4
来源：http://pnz.fanxiaobao.xyz

[T34] Lua：遍历表
来源：http://xqz.feifeiyinyue.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ijy.0kj1m.cn

[T35] Lua：字典表
来源：http://bjq.shuidangran.top

local d = { a = 1 };  d.b = 2
来源：http://cxr.nanxinkj.top

[T36] Lua：函数
来源：http://ock.cqqwz.cn

function add(a, b) return a + b end
来源：http://nqf.ivvv.top

[T37] Lua：字符串拼接
来源：http://lju.shuidangran.top

"a" .. "b"
来源：http://kol.jinqigufen.top

[T38] Lua：条件
来源：http://nzi.zhixingplan.top

if x > 0 then print("正") end
来源：http://fuz.shanyushiyangtech.top

[T39] Lua：模式匹配
来源：http://fye.jqgufenzy.top

string.find(s, "%d+")
来源：http://nqw.yueranfly.top

[T40] Lua：元表
来源：http://qny.gotoacloud.top

setmetatable({}, { __index = base })
来源：http://plu.meibo888.top

[T41] Perl：Hello World
来源：http://zdu.snrcjt.cn

print "Hello\n";
来源：http://xoa.birdmap.top

[T42] Perl：变量类型
来源：http://vvq.zdqjudy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sqy.cdnleiting.top

[T43] Perl：字符串插值
来源：http://xcy.yanxiufei.cn

"值: $a"
来源：http://pht.ehwqpu.com

[T44] Perl：条件
来源：http://qmm.yangfankeji.com

if ($a > 0) { print "正"; }
来源：http://vmi.zdqjudy.top

[T45] Perl：数组遍历
来源：http://ler.yj20258888.top

for my $x (@arr) { print $x; }
来源：http://oct.cucudq.cn

[T46] Perl：哈希操作
来源：http://pgf.ydzc1.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vzy.zdbjq.cn

[T47] Perl：正则捕获
来源：http://snm.chenzaomai.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://rjy.meibo888.top

[T48] Perl：正则替换
来源：http://ndx.yvedp.cn

$s =~ s/old/new/g;
来源：http://wen.chenjidiqi.icu

[T49] Perl：函数
来源：http://cxz.jiagoushi.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://eos.dashuyun.cn

[T50] Perl：逐行读文件
来源：http://hbl.xylfe.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://aba.aibaodan.cn

while (my $line = <$fh>) { print $line; }
来源：http://blg.jinqigufen.top

[T51] Scala：Hello World
来源：http://alg.ydjk.org.cn

println("Hello")
来源：http://zqe.fehbvm.com

[T52] Scala：变量
来源：http://brz.hywenlv.cn

val a = 1;  var b = 2
来源：http://jbo.zycfv.cn

[T53] Scala：字符串插值
来源：http://fyd.hywenlv.cn

s"值: $b"
来源：http://grb.zhaomingkeji.xyz

[T54] Scala：集合映射
来源：http://osu.quarkkingdee.top

List(1, 2, 3).map(_ * 2)
来源：http://gse.aibaodan.cn

[T55] Scala：集合过滤
来源：http://tee.c1oappe.top

List(1, 2, 3).filter(_ > 1)
来源：http://fsl.hysaishi.cn

[T56] Scala：样例类
来源：http://kxa.andypj.xyz

case class User(name: String, age: Int)
来源：http://cwy.sweek.top

[T57] Scala：模式匹配
来源：http://dzq.jqgfzy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://gpm.gogol.net.cn

[T58] Scala：函数定义
来源：http://zez.hysaishi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bvb.sysykeji.top

[T59] Scala：循环
来源：http://lcv.vqdsnc.cn

for (i <- 1 to 10) println(i)
来源：http://cnu.yongpay.top

[T60] Scala：折叠
来源：http://nzq.jinqigufen.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://afh.cdnleiting.top

================================================================================
来源：http://qbt.jinqigufen.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hpo.shzxlz.cn

================================================================================
来源：http://hjw.shangyingyoupin.top

[U01] Py：创建虚拟环境
来源：http://bak.daxiang520.top

python -m venv .venv && source .venv/bin/activate
来源：http://wkm.pycfn.com

[U02] Py：导出 / 安装依赖
来源：http://xqp.hfpthk.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ndb.yj20258.top

[U03] Py：加载 .env 配置
来源：http://pyi.meibo888.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ots.jqgufenzy.top

[U04] Py：变量调试打印
来源：http://dpb.zhongyouzk.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://plb.yvedp.cn

[U05] Py：列表去重且保序
来源：http://ymp.xziqi.cn

list(dict.fromkeys(arr))
来源：http://uny.yongpay.top

[U06] Py：合并两个字典
来源：http://dux.meibo888.top

{**a, **b}
来源：http://osv.yj20258888.top

[U07] Py：反转字典键值
来源：http://uru.cashguo.top

{v: k for k, v in d.items()}
来源：http://jdd.yonumen.top

[U08] Py：展平二维列表
来源：http://vsm.wangshuangyany.cn

[y for x in nested for y in x]
来源：http://ayn.shuidangran.top

[U09] Py：字典取最大值的键
来源：http://xjj.hnxiangtu.top

max(d, key=d.get)
来源：http://urj.andypj.xyz

[U10] Py：按值排序字典
来源：http://uee.gzhubu.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mxz.52xcode.cn

[U11] Py：生成器表达式
来源：http://aqx.yj20258888.top

(x * 2 for x in arr)
来源：http://iul.daria6918.cn

[U12] Py：取出现最多的 3 个元素
来源：http://qdz.ehwqpu.com

Counter(arr).most_common(3)
来源：http://tkw.vehdjk.com

[U13] Py：固定长度队列
来源：http://nsp.cdnleiting.top

deque(maxlen=10)
来源：http://rlu.yanxiufei.cn

[U14] Py：分组收集到列表
来源：http://eic.yj202588.top

defaultdict(list)
来源：http://ukk.jlsjyb.cn

[U15] Py：高精度计时
来源：http://hce.zhongyouzk.top

t = time.perf_counter()
来源：http://ykp.yj20258888.top

[U16] Py：命令行参数解析
来源：http://ztp.redwolf501.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://eza.fengsongda.top

[U17] Py：初始化日志
来源：http://sxs.hnxiangtu.top

logging.basicConfig(level=logging.INFO)
来源：http://piq.0kj1m.cn

[U18] Py：预编译正则
来源：http://jwo.tarul.cn

pat = re.compile(r"\d+")
来源：http://lqe.tian-w.cn

[U19] Py：正则替换带回调
来源：http://egl.xuetiantiany.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hir.pycfn.com

[U20] Py：缓存函数结果
来源：http://brb.chenlongwang.top

@functools.lru_cache(maxsize=None)
来源：http://sii.zhengqikj.top

[U21] Py：自定义上下文管理器
来源：http://kvx.yfazqb.com

@contextlib.contextmanager
来源：http://clk.zhiwuduotai.top

[U22] Py：矩阵转置
来源：http://vdp.havefunace.top

list(zip(*m))
来源：http://rng.shangyingyoupin.top

[U23] Py：分块读取大文件
来源：http://iht.yuanzhike.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://oyc.svipenyu.cn

[U24] Py：路径操作
来源：http://lte.tianlin.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fcq.tarul.cn

[U25] Py：CSV 按字典读
来源：http://jid.zhoulong.xyz

csv.DictReader(f)
来源：http://idh.wangshuangyany.cn

[U26] Py：并发下载
来源：http://xgo.epnwcf.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ksv.smart0.xyz

[U27] Py：异步 HTTP
来源：http://gjj.dashuyun.cn

aiohttp.ClientSession() 配合 async with
来源：http://gtq.cdnleiting.top

[U28] Py：类型别名
来源：http://npu.hongshengwenyu.top

UserId = int
来源：http://ywo.fktsv.cn

[U29] Py：属性校验
来源：http://gnw.wangdashe.top

@property 与 @x.setter 配合
来源：http://rva.ydzc1.top

[U30] Py：数据类
来源：http://dnh.snrcjt.cn

@dataclass(slots=True)
来源：http://jaw.uphjek.com

[U31] Py：单测
来源：http://qsa.cqqwz.cn

python -m pytest -q
来源：http://dzf.9152youxi.cn

[U32] Py：代码格式化
来源：http://ayo.bjfxy.top

ruff format . && ruff check --fix .
来源：http://ige.zhoulong.xyz

[U33] Py：打包发布
来源：http://zkl.hongshengwenyu.top

python -m build  （依赖 pyproject.toml）
来源：http://mbr.cashguo.top

[U34] Py：判断编码
来源：http://qvz.ehwqpu.com

chardet.detect(raw)
来源：http://opf.daxiang520.top

[U35] Py：发送邮件
来源：http://bjm.hysaishi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cqp.ppjwa.cn

[U36] Py：定时任务
来源：http://fja.yuanzhike.top

schedule.every(10).minutes.do(job)
来源：http://sxz.zhaomingkeji.xyz

[U37] Py：读写 Excel
来源：http://bdn.svipenyu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ncp.snrcjt.cn

[U38] Py：获取脚本所在目录
来源：http://mvt.vehdjk.com

Path(__file__).resolve().parent
来源：http://twj.smart0.xyz

[U39] Py：判断是否在交互环境
来源：http://fex.sweek.top

sys.stdout.isatty()
来源：http://mci.hongshengwenyu.top

[U40] Py：打印到标准错误
来源：http://pwv.birdmap.top

print("err", file=sys.stderr)
来源：http://kmx.zhengqikj.top

[U41] PHP：初始化 Composer 项目
来源：http://zto.hnxiangtu.top

composer init;  composer require guzzlehttp/guzzle
来源：http://yfs.sufxvd.cn

[U42] PHP：PSR-4 自动加载
来源：http://wyh.iojbl.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://xsj.c1oappe.top

[U43] PHP：声明命名空间
来源：http://aez.ppjwa.cn

namespace App\Http;
来源：http://yki.yuxming.cn

[U44] PHP：开启严格类型
来源：http://wei.ivvv.top

declare(strict_types=1);
来源：http://umz.birdmap.top

[U45] PHP：类型声明与返回类型
来源：http://emo.shanyushiyangtech.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://qhy.meibo888.top

[U46] PHP：可空类型
来源：http://dhq.yfazqb.com

?string $name = null
来源：http://wdy.feifeiyinyue.top

[U47] PHP：联合类型
来源：http://fld.fehbvm.com

int|string $id
来源：http://mel.gzhubu.top

[U48] PHP：纯枚举
来源：http://heg.jqgfzy.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://odr.zhaomingkeji.xyz

[U49] PHP：只读属性
来源：http://axb.epnwcf.com

public readonly string $name
来源：http://zjd.hnqzz.top

[U50] PHP：构造器属性提升
来源：http://cyy.nanxuanxn.top

public function __construct(private int $id) {}
来源：http://vgh.zdbjq.cn

[U51] PHP：数组解构
来源：http://mkb.fanxiaobao.xyz

[$a, $b] = $arr;
来源：http://mpn.smart0.xyz

[U52] PHP：箭头函数
来源：http://hwx.daxiang520.top

$double = fn($x) => $x * 2;
来源：http://wym.hcnkem.com

[U53] PHP：空合并运算符
来源：http://csr.tian-w.cn

$v = $a ?? $b ?? "default";
来源：http://pkl.cashguo.top

[U54] PHP：空安全调用
来源：http://wpv.havefunace.top

$obj?->method()
来源：http://urn.jlsjyb.cn

[U55] PHP：match 表达式
来源：http://npl.sxryk.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hrt.0kj1m.cn

[U56] PHP：命名参数
来源：http://wvm.zhiwuduotai.top

f(a: 1, b: 2)
来源：http://kew.daxiang520.top

[U57] PHP：字符串插值
来源：http://nvc.svipenyu.cn

"值: {$a}"
来源：http://wsx.bjfxy.top

[U58] PHP：数组三件套
来源：http://ivp.nanxinkj.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://fig.tian-w.cn

[U59] PHP：自定义排序
来源：http://eob.daria6918.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://aje.pycfn.com

[U60] PHP：JSON 编解码
来源：http://vor.bbcook.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://idt.vehdjk.com

[U61] PHP：正则
来源：http://zvb.gotoacloud.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zqm.gaohongyu789.top

[U62] PHP：日期对象
来源：http://hqp.aibaodan.cn

(new DateTimeImmutable())->format("Y-m-d");
来源：http://jlr.andypj.xyz

[U63] PHP：文件读写
来源：http://mry.vehdjk.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hhq.epnwcf.com

[U64] PHP：目录遍历
来源：http://dda.hysaishi.cn

glob("dir/*.php");  scandir("dir");
来源：http://xin.yuanzhike.top

[U65] PHP：会话
来源：http://mca.snrcjt.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://bgl.gogol.net.cn

[U66] PHP：设置 Cookie
来源：http://eyc.316326.xyz

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://rfb.havefunace.top

[U67] PHP：处理文件上传
来源：http://gsb.xingfuxueyuan.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://xyc.gzhubu.top

[U68] PHP：PDO 连接
来源：http://nyu.sxryk.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nwq.chenzaomai.com

[U69] PHP：PDO 预处理
来源：http://mwr.chenjidiqi.icu

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jxw.xingfuxueyuan.xyz

[U70] PHP：PDO 事务
来源：http://qje.bjfxy.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zxt.gogol.net.cn

[U71] PHP：抛出异常
来源：http://xlp.cashguo.top

throw new RuntimeException("失败", 500);
来源：http://ret.bjfxy.top

[U72] PHP：写错误日志
来源：http://ibw.bjfxy.top

error_log("失败: " . $e->getMessage());
来源：http://azy.zdqjudy.top

[U73] PHP：读取 ini 配置
来源：http://pqi.xinyue.icu

parse_ini_file("config.ini", true)
来源：http://lcw.jinqigfzy.top

[U74] PHP：读取环境变量
来源：http://lll.guowangkeji.top

getenv("APP_ENV") ?: "production"
来源：http://jhe.jinqigufen.top

[U75] PHP：依赖注入
来源：http://wfn.shuidangran.top

composer require psr/container
来源：http://qoc.nwbrower.top

[U76] PHP：简单路由
来源：http://vvz.hysaishi.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://qlb.wangdashe.top

[U77] PHP：模板渲染
来源：http://sye.yongpay.top

composer require twig/twig
来源：http://wwg.xinyue.icu

[U78] PHP：单元测试
来源：http://zyg.snrcjt.cn

composer require --dev phpunit/phpunit
来源：http://lfd.tian-w.cn

[U79] PHP：静态分析
来源：http://pex.guannengcc.top

composer require --dev phpstan/phpstan
来源：http://vxm.fktsv.cn

[U80] PHP：代码规范修复
来源：http://dtk.tanke756.top

composer require --dev friendsofphp/php-cs-fixer
来源：http://cfq.yueranfly.top


<!-- 参考信息 -->