代发 wailian999

int size() const noexcept { return n_; }
来源：http://nno.yangfankeji.com

[S53] C++：移动语义
来源：http://wkg.smart0.xyz

std::vector<int> w = std::move(v);
来源：http://gjm.zhoulong.xyz

[S54] C++：异常处理
来源：http://jlr.cashguo.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bwu.hongshengwenyu.top

[S55] C++：结构化绑定
来源：http://ads.xingfuxueyuan.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://mok.hammf.cn

[S56] C++：optional
来源：http://wqr.hesvh.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kyw.cucudq.cn

[S57] C++：编译期常量
来源：http://hdm.yj202588.top

constexpr int N = 10;
来源：http://wvi.sufxvd.cn

[S58] C++：命名空间
来源：http://cxm.jinghuilouyu.cn

namespace ns { int f() { return 1; } }
来源：http://frs.cheryme.top

[S59] C++：静态断言
来源：http://eoc.daxiang520.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://efj.birdmap.top

[S60] C++：遍历并删除元素
来源：http://ywq.sweek.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://amq.jqgufenzy.top

================================================================================
来源：http://xlg.ctjpmb.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dgs.316326.xyz

================================================================================
来源：http://jgq.nanxinkj.top

[T01] Kotlin：Hello World
来源：http://arj.birdmap.top

println("Hello")
来源：http://yof.xuanzx.com

[T02] Kotlin：变量
来源：http://vps.vqdsnc.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dxa.gzhubu.top

[T03] Kotlin：字符串模板
来源：http://lch.yonumen.top

"值: $b"
来源：http://hrq.shzxlz.cn

[T04] Kotlin：空安全
来源：http://gcg.gogol.net.cn

val n: String? = null;  n?.length
来源：http://jop.cdnleiting.top

[T05] Kotlin：when 表达式
来源：http://lyo.wangdashe.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jpn.ppjwa.cn

[T06] Kotlin：集合映射
来源：http://hze.vqdsnc.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ybf.shangyingyoupin.top

[T07] Kotlin：集合过滤
来源：http://oqu.c1oappe.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://bnn.sysykeji.top

[T08] Kotlin：数据类
来源：http://gfv.chenjidiqi.icu

data class User(val name: String, val age: Int)
来源：http://cnp.jinghuilouyu.cn

[T09] Kotlin：扩展函数
来源：http://zho.wangdashe.top

fun String.exclaim() = this + "!"
来源：http://jhd.hywenlv.cn

[T10] Kotlin：默认参数
来源：http://xsy.daria6918.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vpg.xziqi.cn

[T11] Kotlin：协程
来源：http://jym.ehwqpu.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://qgd.ywan-chungtsiang.top

[T12] Kotlin：解构声明
来源：http://hye.fehbvm.com

val (a, b) = Pair(1, 2)
来源：http://rrh.yfazqb.com

[T13] Kotlin：只读 Map
来源：http://hwx.dianchejie.cn

val m = mapOf("a" to 1)
来源：http://dif.ywan-chungtsiang.top

[T14] Kotlin：循环
来源：http://ccd.redwolf501.top

for (i in 1..10) println(i)
来源：http://gxz.zhengqikj.top

[T15] Kotlin：接口
来源：http://fuk.dianchejie.cn

interface Shape { fun area(): Double }
来源：http://zvz.hysaishi.cn

[T16] Swift：Hello World
来源：http://rfd.cheryme.top

print("Hello")
来源：http://gsk.haohaochexian.top

[T17] Swift：变量与常量
来源：http://zcd.yongpay.top

var a = 1;  let b = 2
来源：http://olp.yangfankeji.com

[T18] Swift：字符串插值
来源：http://dza.tanke756.top

"值: \(b)"
来源：http://zgh.kuanghao11.cn

[T19] Swift：可选绑定
来源：http://hnd.0kj1m.cn

if let n = opt { print(n) }
来源：http://tgm.birdmap.top

[T20] Swift：数组操作
来源：http://urj.0kj1m.cn

var a = [1, 2, 3];  a.append(4)
来源：http://vgg.hammf.cn

[T21] Swift：遍历
来源：http://jku.xuetiantiany.cn

for x in a { print(x) }
来源：http://buo.guannengcc.top

[T22] Swift：字典
来源：http://mtx.kuanghao11.cn

var d = ["a": 1];  d["b"] = 2
来源：http://jgk.cdnleiting.top

[T23] Swift：函数
来源：http://sre.smart0.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fxb.svipenyu.cn

[T24] Swift：闭包
来源：http://yvd.shanyushiyangtech.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://iml.ctjpmb.com

[T25] Swift：结构体
来源：http://jfl.haohaochexian.top

struct P { var x: Int }
来源：http://gne.redwolf501.top

[T26] Swift：类与重写
来源：http://rrs.guannengcc.top

class A: Base { override func f() {} }
来源：http://oiy.zhaomingkeji.xyz

[T27] Swift：错误处理
来源：http://dke.fzhhl.top

do { try f() } catch { print(error) }
来源：http://mkr.0kj1m.cn

[T28] Swift：枚举
来源：http://ztg.xinyue.icu

enum Color { case red, green }
来源：http://shx.zdqjudy.top

[T29] Swift：guard 提前返回
来源：http://xqf.jqgufenzy.top

guard let x = opt else { return }
来源：http://kam.jinyuanbaomall.cn

[T30] Swift：协议
来源：http://zme.kuanghao11.cn

protocol Shape { func area() -> Double }
来源：http://fes.xuetiantiany.cn

[T31] Lua：Hello World
来源：http://smt.shuidangran.top

print("Hello")
来源：http://vqo.xziqi.cn

[T32] Lua：局部变量
来源：http://dpn.uphjek.com

local a = 1
来源：http://rts.yj20258888.top

[T33] Lua：表（数组）
来源：http://ytu.hesvh.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ptg.tarul.cn

[T34] Lua：遍历表
来源：http://mvm.havefunace.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ori.yuxming.cn

[T35] Lua：字典表
来源：http://xjo.hesvh.cn

local d = { a = 1 };  d.b = 2
来源：http://lwy.jqgfzy.top

[T36] Lua：函数
来源：http://wjq.pycfn.com

function add(a, b) return a + b end
来源：http://cdp.xylfe.cn

[T37] Lua：字符串拼接
来源：http://hqd.redwolf501.top

"a" .. "b"
来源：http://pid.shzxlz.cn

[T38] Lua：条件
来源：http://gki.haohaochexian.top

if x > 0 then print("正") end
来源：http://bjf.xziqi.cn

[T39] Lua：模式匹配
来源：http://sur.iojbl.cn

string.find(s, "%d+")
来源：http://aep.cqqwz.cn

[T40] Lua：元表
来源：http://qjh.ydzc1.top

setmetatable({}, { __index = base })
来源：http://zcc.ydjk.org.cn

[T41] Perl：Hello World
来源：http://uvd.9152youxi.cn

print "Hello\n";
来源：http://jnu.hnxiangtu.top

[T42] Perl：变量类型
来源：http://huv.yj20258.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qks.haohaochexian.top

[T43] Perl：字符串插值
来源：http://uvj.zhengqikj.top

"值: $a"
来源：http://uql.shanyushiyangkeji.top

[T44] Perl：条件
来源：http://glw.gzhubu.top

if ($a > 0) { print "正"; }
来源：http://dpz.andypj.xyz

[T45] Perl：数组遍历
来源：http://scj.feifeiyinyue.top

for my $x (@arr) { print $x; }
来源：http://yhh.sjlbkw.cn

[T46] Perl：哈希操作
来源：http://tjw.svipenyu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ina.jinghuilouyu.cn

[T47] Perl：正则捕获
来源：http://qfz.smart0.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://xhi.jiagoushi.top

[T48] Perl：正则替换
来源：http://zgw.aizwys.cn

$s =~ s/old/new/g;
来源：http://qmt.fzhhl.top

[T49] Perl：函数
来源：http://nyp.guowangkeji.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://joa.dianchejie.cn

[T50] Perl：逐行读文件
来源：http://rrx.dashuyun.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rsd.wangdashe.top

while (my $line = <$fh>) { print $line; }
来源：http://cba.9152youxi.cn

[T51] Scala：Hello World
来源：http://qni.tarul.cn

println("Hello")
来源：http://hgo.xinyue.icu

[T52] Scala：变量
来源：http://cna.bbcook.cn

val a = 1;  var b = 2
来源：http://mvi.wangshuangyany.cn

[T53] Scala：字符串插值
来源：http://vbi.uphjek.com

s"值: $b"
来源：http://tfc.daria6918.cn

[T54] Scala：集合映射
来源：http://myc.zhengqikj.top

List(1, 2, 3).map(_ * 2)
来源：http://rrx.haohaochexian.top

[T55] Scala：集合过滤
来源：http://acx.sxryk.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ngu.redwolf501.top

[T56] Scala：样例类
来源：http://tid.yj20258.top

case class User(name: String, age: Int)
来源：http://jbl.xuanzx.com

[T57] Scala：模式匹配
来源：http://llm.9152youxi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://qfh.shanyushiyangtech.top

[T58] Scala：函数定义
来源：http://mek.daria6918.cn

def add(a: Int, b: Int): Int = a + b
来源：http://tal.hongshengwenyu.top

[T59] Scala：循环
来源：http://hom.meibo888.top

for (i <- 1 to 10) println(i)
来源：http://mpe.ywan-chungtsiang.top

[T60] Scala：折叠
来源：http://mnt.nanxuanxn.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xcf.ivvv.top

================================================================================
来源：http://ffs.cqqwz.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nxz.jinqigfzy.top

================================================================================
来源：http://gib.shuidangran.top

[U01] Py：创建虚拟环境
来源：http://geg.shuidangran.top

python -m venv .venv && source .venv/bin/activate
来源：http://rir.gogol.net.cn

[U02] Py：导出 / 安装依赖
来源：http://tpc.shzxlz.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jpi.xingfuxueyuan.xyz

[U03] Py：加载 .env 配置
来源：http://txq.guannengcc.top

from dotenv import load_dotenv; load_dotenv()
来源：http://dcp.sxryk.cn

[U04] Py：变量调试打印
来源：http://pdd.kuanghao11.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://low.pengpengdd.cyou

[U05] Py：列表去重且保序
来源：http://uwm.ctjpmb.com

list(dict.fromkeys(arr))
来源：http://nwl.jinyuanbaomall.cn

[U06] Py：合并两个字典
来源：http://rfe.jinqigufen.top

{**a, **b}
来源：http://pxr.jqgfzy.top

[U07] Py：反转字典键值
来源：http://wye.guannengcc.top

{v: k for k, v in d.items()}
来源：http://mgl.redwolf501.top

[U08] Py：展平二维列表
来源：http://ije.shzxlz.cn

[y for x in nested for y in x]
来源：http://twr.hfpthk.cn

[U09] Py：字典取最大值的键
来源：http://yzg.zhoulong.xyz

max(d, key=d.get)
来源：http://zhx.sysykeji.top

[U10] Py：按值排序字典
来源：http://owg.vehdjk.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mpv.havefunace.top

[U11] Py：生成器表达式
来源：http://ard.0kj1m.cn

(x * 2 for x in arr)
来源：http://oem.fehbvm.com

[U12] Py：取出现最多的 3 个元素
来源：http://qzb.52xcode.cn

Counter(arr).most_common(3)
来源：http://pdd.zdbjq.cn

[U13] Py：固定长度队列
来源：http://ovk.zhijiandao.cn

deque(maxlen=10)
来源：http://pfw.0kj1m.cn

[U14] Py：分组收集到列表
来源：http://sti.hysaishi.cn

defaultdict(list)
来源：http://xoz.xuetiantiany.cn

[U15] Py：高精度计时
来源：http://djs.jlsjyb.cn

t = time.perf_counter()
来源：http://hnf.aizwys.cn

[U16] Py：命令行参数解析
来源：http://daz.shanyushiyangtech.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ftt.andypj.xyz

[U17] Py：初始化日志
来源：http://twl.birdmap.top

logging.basicConfig(level=logging.INFO)
来源：http://chm.yanxiufei.cn

[U18] Py：预编译正则
来源：http://dvu.sufxvd.cn

pat = re.compile(r"\d+")
来源：http://yvv.chenlongwang.top

[U19] Py：正则替换带回调
来源：http://dpe.xuanzx.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qbj.iojbl.cn

[U20] Py：缓存函数结果
来源：http://ryb.jinyuanbaomall.cn

@functools.lru_cache(maxsize=None)
来源：http://wnt.sweek.top

[U21] Py：自定义上下文管理器
来源：http://vcd.yvedp.cn

@contextlib.contextmanager
来源：http://kva.c1oappe.top

[U22] Py：矩阵转置
来源：http://oqt.bjfxy.top

list(zip(*m))
来源：http://gap.jlsjyb.cn

[U23] Py：分块读取大文件
来源：http://aie.jianghu66.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nug.xziqi.cn

[U24] Py：路径操作
来源：http://qyw.cqqwz.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ufm.sxryk.cn

[U25] Py：CSV 按字典读
来源：http://uaq.cheryme.top

csv.DictReader(f)
来源：http://moh.hongshengwenyu.top

[U26] Py：并发下载
来源：http://bba.yj20258.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jhs.gogol.net.cn

[U27] Py：异步 HTTP
来源：http://oth.jqgufenzy.top

aiohttp.ClientSession() 配合 async with
来源：http://fgz.hywenlv.cn

[U28] Py：类型别名
来源：http://hzl.wangdashe.top

UserId = int
来源：http://dog.gaohongyu789.top

[U29] Py：属性校验
来源：http://vcl.vqdsnc.cn

@property 与 @x.setter 配合
来源：http://ydv.birdmap.top

[U30] Py：数据类
来源：http://tob.zhongyouzk.top

@dataclass(slots=True)
来源：http://wmc.shanyushiyangtech.top

[U31] Py：单测
来源：http://xmp.uphjek.com

python -m pytest -q
来源：http://mxh.zdbjq.cn

[U32] Py：代码格式化
来源：http://kts.nanxinkj.top

ruff format . && ruff check --fix .
来源：http://sbf.aibaodan.cn

[U33] Py：打包发布
来源：http://ybc.ppjwa.cn

python -m build  （依赖 pyproject.toml）
来源：http://upx.chenzaomai.com

[U34] Py：判断编码
来源：http://dlf.vehdjk.com

chardet.detect(raw)
来源：http://wqd.yj202588.top

[U35] Py：发送邮件
来源：http://luh.xinyue.icu

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kgi.yuanzhike.top

[U36] Py：定时任务
来源：http://fog.hywenlv.cn

schedule.every(10).minutes.do(job)
来源：http://qeu.nwbrower.top

[U37] Py：读写 Excel
来源：http://crc.zdbjq.cn

pandas.read_excel / DataFrame.to_excel
来源：http://xio.hnqzz.top

[U38] Py：获取脚本所在目录
来源：http://gwy.kuanghao11.cn

Path(__file__).resolve().parent
来源：http://rvh.jianghu66.top

[U39] Py：判断是否在交互环境
来源：http://wqa.hesvh.cn

sys.stdout.isatty()
来源：http://vxd.nanxuanxn.top

[U40] Py：打印到标准错误
来源：http://knh.dianchejie.cn

print("err", file=sys.stderr)
来源：http://sfi.xziqi.cn

[U41] PHP：初始化 Composer 项目
来源：http://vdo.aibaodan.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qut.nwbrower.top

[U42] PHP：PSR-4 自动加载
来源：http://xcv.yonumen.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://chl.xuanzx.com

[U43] PHP：声明命名空间
来源：http://plg.dianchejie.cn

namespace App\Http;
来源：http://bgj.9152youxi.cn

[U44] PHP：开启严格类型
来源：http://yrd.vqdsnc.cn

declare(strict_types=1);
来源：http://nsb.chenzaomai.com

[U45] PHP：类型声明与返回类型
来源：http://lif.redwolf501.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://mcw.gotoacloud.top

[U46] PHP：可空类型
来源：http://ony.nanxuanxn.top

?string $name = null
来源：http://gcp.ydjk.org.cn

[U47] PHP：联合类型
来源：http://qmm.tianlin.xyz

int|string $id
来源：http://uis.uphjek.com

[U48] PHP：纯枚举
来源：http://zak.havefunace.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hxy.ctjpmb.com

[U49] PHP：只读属性
来源：http://fwn.xuanzx.com

public readonly string $name
来源：http://kss.gotoacloud.top

[U50] PHP：构造器属性提升
来源：http://rbe.yanxiufei.cn

public function __construct(private int $id) {}
来源：http://zzd.aibaodan.cn

[U51] PHP：数组解构
来源：http://vdv.ywan-chungtsiang.top

[$a, $b] = $arr;
来源：http://pge.cashguo.top

[U52] PHP：箭头函数
来源：http://byt.feifeiyinyue.top

$double = fn($x) => $x * 2;
来源：http://qws.yuanzhike.top

[U53] PHP：空合并运算符
来源：http://syz.xinyue.icu

$v = $a ?? $b ?? "default";
来源：http://ubp.feifeiyinyue.top

[U54] PHP：空安全调用
来源：http://tzy.wangshuangyany.cn

$obj?->method()
来源：http://mwl.sysykeji.top

[U55] PHP：match 表达式
来源：http://mdi.shanyushiyangtech.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gfx.nwbrower.top

[U56] PHP：命名参数
来源：http://ikl.guannengcc.top

f(a: 1, b: 2)
来源：http://cvu.hammf.cn

[U57] PHP：字符串插值
来源：http://atg.jinghuilouyu.cn

"值: {$a}"
来源：http://arq.hcnkem.com

[U58] PHP：数组三件套
来源：http://mgj.nwbrower.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tdx.hfpthk.cn

[U59] PHP：自定义排序
来源：http://zls.gaohongyu789.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dyx.hnxiangtu.top

[U60] PHP：JSON 编解码
来源：http://zlq.hongshengwenyu.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://kpk.yangfankeji.com

[U61] PHP：正则
来源：http://psi.jinyuanbaomall.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://szs.birdmap.top

[U62] PHP：日期对象
来源：http://pdq.zhoulong.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://rtw.hysaishi.cn

[U63] PHP：文件读写
来源：http://fuw.aibaodan.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://vjq.jyoumei.cn

[U64] PHP：目录遍历
来源：http://rxr.kuanghao11.cn

glob("dir/*.php");  scandir("dir");
来源：http://nxr.mhx1999.top

[U65] PHP：会话
来源：http://hzh.ppjwa.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://fwq.hesvh.cn

[U66] PHP：设置 Cookie
来源：http://rxh.quarkkingdee.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://pqv.sweek.top

[U67] PHP：处理文件上传
来源：http://uts.0kj1m.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rlt.ybcxt.top

[U68] PHP：PDO 连接
来源：http://smd.zdbjq.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://hrr.zycfv.cn

[U69] PHP：PDO 预处理
来源：http://nny.wangshuangyany.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://jmd.zdbjq.cn

[U70] PHP：PDO 事务
来源：http://hel.hesvh.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://lzp.meibo888.top

[U71] PHP：抛出异常
来源：http://jee.shuidangran.top

throw new RuntimeException("失败", 500);
来源：http://kwl.yvedp.cn

[U72] PHP：写错误日志
来源：http://exf.jinghuilouyu.cn

error_log("失败: " . $e->getMessage());
来源：http://jds.ywan-chungtsiang.top

[U73] PHP：读取 ini 配置
来源：http://qma.9152youxi.cn

parse_ini_file("config.ini", true)
来源：http://htv.wangshuangyany.cn

[U74] PHP：读取环境变量
来源：http://icv.nanxuanxn.top

getenv("APP_ENV") ?: "production"
来源：http://koe.jinghuilouyu.cn

[U75] PHP：依赖注入
来源：http://ahx.zhaomingkeji.xyz

composer require psr/container
来源：http://wxr.tarul.cn

[U76] PHP：简单路由
来源：http://avy.dashuyun.cn

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://jku.yueranfly.top

[U77] PHP：模板渲染
来源：http://hku.hesvh.cn

composer require twig/twig
来源：http://ikl.zhongyouzk.top

[U78] PHP：单元测试
来源：http://qjp.9152youxi.cn

composer require --dev phpunit/phpunit
来源：http://gso.zhoulong.xyz


<!-- 参考信息 -->