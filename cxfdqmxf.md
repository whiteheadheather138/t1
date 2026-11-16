代发 wailian999

while (std::getline(in, line)) { }
来源：http://sqr.jqgfzy.top

[S49] C++：写文件
来源：http://pxw.gzhubu.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hwr.svipenyu.cn

[S50] C++：格式化数字
来源：http://oiu.ehwqpu.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hnh.52xcode.cn

[S51] C++：显式类型转换
来源：http://uua.tian-w.cn

static_cast<double>(a) / b
来源：http://fzv.yuxming.cn

[S52] C++：const 与 noexcept
来源：http://wex.shangyingyoupin.top

int size() const noexcept { return n_; }
来源：http://vmu.ehwqpu.com

[S53] C++：移动语义
来源：http://tta.hcnkem.com

std::vector<int> w = std::move(v);
来源：http://vkl.quarkkingdee.top

[S54] C++：异常处理
来源：http://skt.jinyuanbaomall.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://edn.ehwqpu.com

[S55] C++：结构化绑定
来源：http://vgm.sufxvd.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wpe.pycfn.com

[S56] C++：optional
来源：http://ohp.aizwys.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://drc.kuanghao11.cn

[S57] C++：编译期常量
来源：http://gzd.tarul.cn

constexpr int N = 10;
来源：http://oij.ybcxt.top

[S58] C++：命名空间
来源：http://ach.ywan-chungtsiang.top

namespace ns { int f() { return 1; } }
来源：http://god.daria6918.cn

[S59] C++：静态断言
来源：http://myt.hnxiangtu.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wip.hongshengwenyu.top

[S60] C++：遍历并删除元素
来源：http://bhn.aizwys.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://alq.mhx1999.top

================================================================================
来源：http://eqz.shangyingyoupin.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zlr.hammf.cn

================================================================================
来源：http://byq.sufxvd.cn

[T01] Kotlin：Hello World
来源：http://ldt.fehbvm.com

println("Hello")
来源：http://snn.316326.xyz

[T02] Kotlin：变量
来源：http://vlw.gaohongyu789.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://juw.hysaishi.cn

[T03] Kotlin：字符串模板
来源：http://bja.yj20258888.top

"值: $b"
来源：http://cef.pengpengdd.cyou

[T04] Kotlin：空安全
来源：http://kla.redwolf501.top

val n: String? = null;  n?.length
来源：http://pvu.epnwcf.com

[T05] Kotlin：when 表达式
来源：http://vre.yuxming.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jlb.cheryme.top

[T06] Kotlin：集合映射
来源：http://tjd.havefunace.top

listOf(1, 2, 3).map { it * 2 }
来源：http://gcx.iojbl.cn

[T07] Kotlin：集合过滤
来源：http://ypo.jqgufenzy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://hzr.zhixingplan.top

[T08] Kotlin：数据类
来源：http://oev.shanyushiyangtech.top

data class User(val name: String, val age: Int)
来源：http://lax.nwbrower.top

[T09] Kotlin：扩展函数
来源：http://fqq.feifeiyinyue.top

fun String.exclaim() = this + "!"
来源：http://vlw.zhongyouzk.top

[T10] Kotlin：默认参数
来源：http://hso.zhijiandao.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://dty.wangdashe.top

[T11] Kotlin：协程
来源：http://bgz.cqqwz.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://kyy.xuetiantiany.cn

[T12] Kotlin：解构声明
来源：http://egd.haohaochexian.top

val (a, b) = Pair(1, 2)
来源：http://zjn.dashuyun.cn

[T13] Kotlin：只读 Map
来源：http://fxw.vehdjk.com

val m = mapOf("a" to 1)
来源：http://mlo.jianghu66.top

[T14] Kotlin：循环
来源：http://dth.yfazqb.com

for (i in 1..10) println(i)
来源：http://luc.ctjpmb.com

[T15] Kotlin：接口
来源：http://ilm.jianghu66.top

interface Shape { fun area(): Double }
来源：http://fug.guowangkeji.top

[T16] Swift：Hello World
来源：http://gqe.zhijiandao.cn

print("Hello")
来源：http://umk.hysaishi.cn

[T17] Swift：变量与常量
来源：http://giu.ybcxt.top

var a = 1;  let b = 2
来源：http://uac.uphjek.com

[T18] Swift：字符串插值
来源：http://ump.vqdsnc.cn

"值: \(b)"
来源：http://mqa.hcnkem.com

[T19] Swift：可选绑定
来源：http://yra.hnxiangtu.top

if let n = opt { print(n) }
来源：http://ttx.yuanzhike.top

[T20] Swift：数组操作
来源：http://dph.yueranfly.top

var a = [1, 2, 3];  a.append(4)
来源：http://kah.xingfuxueyuan.xyz

[T21] Swift：遍历
来源：http://sow.jinghuilouyu.cn

for x in a { print(x) }
来源：http://imr.chenjidiqi.icu

[T22] Swift：字典
来源：http://jey.jinqigfzy.top

var d = ["a": 1];  d["b"] = 2
来源：http://und.yonumen.top

[T23] Swift：函数
来源：http://dss.xylfe.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://uka.9152youxi.cn

[T24] Swift：闭包
来源：http://rju.jinqigufen.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://xiv.guannengcc.top

[T25] Swift：结构体
来源：http://esn.shanyushiyangkeji.top

struct P { var x: Int }
来源：http://wld.xinyue.icu

[T26] Swift：类与重写
来源：http://lra.guannengcc.top

class A: Base { override func f() {} }
来源：http://rnj.ydjk.org.cn

[T27] Swift：错误处理
来源：http://afk.ydzc1.top

do { try f() } catch { print(error) }
来源：http://yei.tarul.cn

[T28] Swift：枚举
来源：http://itd.hcnkem.com

enum Color { case red, green }
来源：http://lvl.zycfv.cn

[T29] Swift：guard 提前返回
来源：http://qfe.bbcook.cn

guard let x = opt else { return }
来源：http://zih.yuanzhike.top

[T30] Swift：协议
来源：http://cfo.jqgfzy.top

protocol Shape { func area() -> Double }
来源：http://aar.epnwcf.com

[T31] Lua：Hello World
来源：http://cet.hywenlv.cn

print("Hello")
来源：http://ebj.kuanghao11.cn

[T32] Lua：局部变量
来源：http://ynz.gaohongyu789.top

local a = 1
来源：http://xnv.tianlin.xyz

[T33] Lua：表（数组）
来源：http://epa.wangshuangyany.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://lew.yj20258888.top

[T34] Lua：遍历表
来源：http://ukv.316326.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://nft.cashguo.top

[T35] Lua：字典表
来源：http://xgx.yuxming.cn

local d = { a = 1 };  d.b = 2
来源：http://trn.zycfv.cn

[T36] Lua：函数
来源：http://vth.yuxming.cn

function add(a, b) return a + b end
来源：http://obk.daria6918.cn

[T37] Lua：字符串拼接
来源：http://wal.vehdjk.com

"a" .. "b"
来源：http://fkk.tianlin.xyz

[T38] Lua：条件
来源：http://glm.yangfankeji.com

if x > 0 then print("正") end
来源：http://yph.svipenyu.cn

[T39] Lua：模式匹配
来源：http://jin.jlsjyb.cn

string.find(s, "%d+")
来源：http://avp.bjfxy.top

[T40] Lua：元表
来源：http://sjp.bbcook.cn

setmetatable({}, { __index = base })
来源：http://ybt.mhx1999.top

[T41] Perl：Hello World
来源：http://uro.tianlin.xyz

print "Hello\n";
来源：http://wnw.zhiwuduotai.top

[T42] Perl：变量类型
来源：http://yhm.uphjek.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://okh.zhaomingkeji.xyz

[T43] Perl：字符串插值
来源：http://kgh.zhijiandao.cn

"值: $a"
来源：http://lpq.hesvh.cn

[T44] Perl：条件
来源：http://xqd.hywenlv.cn

if ($a > 0) { print "正"; }
来源：http://tjm.cqqwz.cn

[T45] Perl：数组遍历
来源：http://tii.zhongyouzk.top

for my $x (@arr) { print $x; }
来源：http://fal.fanxiaobao.xyz

[T46] Perl：哈希操作
来源：http://kqj.yuanzhike.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ntu.hammf.cn

[T47] Perl：正则捕获
来源：http://sjw.havefunace.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://njx.ybcxt.top

[T48] Perl：正则替换
来源：http://zqo.vqdsnc.cn

$s =~ s/old/new/g;
来源：http://efg.nanxuanxn.top

[T49] Perl：函数
来源：http://rkx.quarkkingdee.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ykq.xylfe.cn

[T50] Perl：逐行读文件
来源：http://rhs.9152youxi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ngw.yuanzhike.top

while (my $line = <$fh>) { print $line; }
来源：http://cvu.aizwys.cn

[T51] Scala：Hello World
来源：http://epa.dianchejie.cn

println("Hello")
来源：http://tgn.gotoacloud.top

[T52] Scala：变量
来源：http://dup.tanke756.top

val a = 1;  var b = 2
来源：http://jox.hcnkem.com

[T53] Scala：字符串插值
来源：http://xns.yueranfly.top

s"值: $b"
来源：http://sop.shangyingyoupin.top

[T54] Scala：集合映射
来源：http://svn.epnwcf.com

List(1, 2, 3).map(_ * 2)
来源：http://oyl.fktsv.cn

[T55] Scala：集合过滤
来源：http://oew.birdmap.top

List(1, 2, 3).filter(_ > 1)
来源：http://smb.tianlin.xyz

[T56] Scala：样例类
来源：http://iiv.ydzc1.top

case class User(name: String, age: Int)
来源：http://wxn.xuetiantiany.cn

[T57] Scala：模式匹配
来源：http://chb.smart0.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://qks.cucudq.cn

[T58] Scala：函数定义
来源：http://lfh.zhijiandao.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wgi.yvedp.cn

[T59] Scala：循环
来源：http://rsb.jyoumei.cn

for (i <- 1 to 10) println(i)
来源：http://rua.shuidangran.top

[T60] Scala：折叠
来源：http://ats.hywenlv.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tpl.iojbl.cn

================================================================================
来源：http://jme.daria6918.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dtm.shanyushiyangtech.top

================================================================================
来源：http://tvu.hysaishi.cn

[U01] Py：创建虚拟环境
来源：http://abg.jiagoushi.top

python -m venv .venv && source .venv/bin/activate
来源：http://ovz.shuidangran.top

[U02] Py：导出 / 安装依赖
来源：http://gig.hesvh.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yyh.zhaomingkeji.xyz

[U03] Py：加载 .env 配置
来源：http://nao.shanyushiyangtech.top

from dotenv import load_dotenv; load_dotenv()
来源：http://djh.sjlbkw.cn

[U04] Py：变量调试打印
来源：http://byh.gotoacloud.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://yhk.hesvh.cn

[U05] Py：列表去重且保序
来源：http://ttl.sxryk.cn

list(dict.fromkeys(arr))
来源：http://esy.sxryk.cn

[U06] Py：合并两个字典
来源：http://ytk.zhengqikj.top

{**a, **b}
来源：http://pbi.zhiwuduotai.top

[U07] Py：反转字典键值
来源：http://atp.tian-w.cn

{v: k for k, v in d.items()}
来源：http://wqm.xinyue.icu

[U08] Py：展平二维列表
来源：http://fje.yj20258888.top

[y for x in nested for y in x]
来源：http://gns.redwolf501.top

[U09] Py：字典取最大值的键
来源：http://szn.xziqi.cn

max(d, key=d.get)
来源：http://bif.jinyuanbaomall.cn

[U10] Py：按值排序字典
来源：http://uzq.zhoulong.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://vmi.bjfxy.top

[U11] Py：生成器表达式
来源：http://psp.xziqi.cn

(x * 2 for x in arr)
来源：http://dwi.zhaomingkeji.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://fki.guannengcc.top

Counter(arr).most_common(3)
来源：http://vqu.meibo888.top

[U13] Py：固定长度队列
来源：http://lke.havefunace.top

deque(maxlen=10)
来源：http://ypu.yanxiufei.cn

[U14] Py：分组收集到列表
来源：http://vpv.cheryme.top

defaultdict(list)
来源：http://vlo.shangyingyoupin.top

[U15] Py：高精度计时
来源：http://zmw.andypj.xyz

t = time.perf_counter()
来源：http://muv.daria6918.cn

[U16] Py：命令行参数解析
来源：http://kxe.hammf.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cff.shangyingyoupin.top

[U17] Py：初始化日志
来源：http://ety.ctjpmb.com

logging.basicConfig(level=logging.INFO)
来源：http://xms.yvedp.cn

[U18] Py：预编译正则
来源：http://aho.sysykeji.top

pat = re.compile(r"\d+")
来源：http://fdt.hongshengwenyu.top

[U19] Py：正则替换带回调
来源：http://bjz.yonumen.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ezk.bbcook.cn

[U20] Py：缓存函数结果
来源：http://kxv.zhixingplan.top

@functools.lru_cache(maxsize=None)
来源：http://rkn.shanyushiyangkeji.top

[U21] Py：自定义上下文管理器
来源：http://sqd.daxiang520.top

@contextlib.contextmanager
来源：http://oux.guannengcc.top

[U22] Py：矩阵转置
来源：http://dtf.jlsjyb.cn

list(zip(*m))
来源：http://uzl.xuetiantiany.cn

[U23] Py：分块读取大文件
来源：http://bfq.jqgfzy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://daa.xziqi.cn

[U24] Py：路径操作
来源：http://npt.jinqigfzy.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rrp.0kj1m.cn

[U25] Py：CSV 按字典读
来源：http://smg.vehdjk.com

csv.DictReader(f)
来源：http://zfr.uphjek.com

[U26] Py：并发下载
来源：http://gdo.jlsjyb.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xzv.nanxuanxn.top

[U27] Py：异步 HTTP
来源：http://nbj.hysaishi.cn

aiohttp.ClientSession() 配合 async with
来源：http://hso.hnqzz.top

[U28] Py：类型别名
来源：http://ywf.zhengqikj.top

UserId = int
来源：http://xjn.cdnleiting.top

[U29] Py：属性校验
来源：http://ptw.iojbl.cn

@property 与 @x.setter 配合
来源：http://dmn.xinyue.icu

[U30] Py：数据类
来源：http://dqf.0kj1m.cn

@dataclass(slots=True)
来源：http://lxh.shanyushiyangtech.top

[U31] Py：单测
来源：http://isr.tanke756.top

python -m pytest -q
来源：http://cli.dashuyun.cn

[U32] Py：代码格式化
来源：http://xob.yongpay.top

ruff format . && ruff check --fix .
来源：http://tui.ehwqpu.com

[U33] Py：打包发布
来源：http://fan.ybcxt.top

python -m build  （依赖 pyproject.toml）
来源：http://zkp.chenjidiqi.icu

[U34] Py：判断编码
来源：http://lav.cashguo.top

chardet.detect(raw)
来源：http://tdk.fanxiaobao.xyz

[U35] Py：发送邮件
来源：http://igg.shuidangran.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lay.zhengqikj.top

[U36] Py：定时任务
来源：http://hth.hammf.cn

schedule.every(10).minutes.do(job)
来源：http://abo.jinqigufen.top

[U37] Py：读写 Excel
来源：http://ekm.yuxming.cn

pandas.read_excel / DataFrame.to_excel
来源：http://mnk.xingfuxueyuan.xyz

[U38] Py：获取脚本所在目录
来源：http://bex.yuxming.cn

Path(__file__).resolve().parent
来源：http://faw.ydjk.org.cn

[U39] Py：判断是否在交互环境
来源：http://adj.hfpthk.cn

sys.stdout.isatty()
来源：http://khx.sysykeji.top

[U40] Py：打印到标准错误
来源：http://ice.gogol.net.cn

print("err", file=sys.stderr)
来源：http://iqk.xinyue.icu

[U41] PHP：初始化 Composer 项目
来源：http://zwy.daxiang520.top

composer init;  composer require guzzlehttp/guzzle
来源：http://sht.shuidangran.top

[U42] PHP：PSR-4 自动加载
来源：http://quz.shangyingyoupin.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kby.yj20258.top

[U43] PHP：声明命名空间
来源：http://eks.yangfankeji.com

namespace App\Http;
来源：http://nbr.xylfe.cn

[U44] PHP：开启严格类型
来源：http://olc.tarul.cn

declare(strict_types=1);
来源：http://hav.gzhubu.top

[U45] PHP：类型声明与返回类型
来源：http://yow.gaohongyu789.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://img.yongpay.top

[U46] PHP：可空类型
来源：http://wkc.daxiang520.top

?string $name = null
来源：http://aqj.jinyuanbaomall.cn

[U47] PHP：联合类型
来源：http://kyi.cqqwz.cn

int|string $id
来源：http://naa.guowangkeji.top

[U48] PHP：纯枚举
来源：http://mkx.tarul.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wct.jinyuanbaomall.cn

[U49] PHP：只读属性
来源：http://kho.xuanzx.com

public readonly string $name
来源：http://reg.bjfxy.top

[U50] PHP：构造器属性提升
来源：http://grd.kuanghao11.cn

public function __construct(private int $id) {}
来源：http://azb.vqdsnc.cn

[U51] PHP：数组解构
来源：http://iwb.havefunace.top

[$a, $b] = $arr;
来源：http://iqo.redwolf501.top

[U52] PHP：箭头函数
来源：http://aul.shangyingyoupin.top

$double = fn($x) => $x * 2;
来源：http://zlj.zhoulong.xyz

[U53] PHP：空合并运算符
来源：http://hzd.sysykeji.top

$v = $a ?? $b ?? "default";
来源：http://wut.nwbrower.top

[U54] PHP：空安全调用
来源：http://hqb.zhongyouzk.top

$obj?->method()
来源：http://ebw.ydzc1.top

[U55] PHP：match 表达式
来源：http://gib.jinghuilouyu.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://zjj.snrcjt.cn

[U56] PHP：命名参数
来源：http://adj.iojbl.cn

f(a: 1, b: 2)
来源：http://gub.guannengcc.top

[U57] PHP：字符串插值
来源：http://yjg.chenzaomai.com

"值: {$a}"
来源：http://wei.pengpengdd.cyou

[U58] PHP：数组三件套
来源：http://rva.hcnkem.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://yif.smart0.xyz

[U59] PHP：自定义排序
来源：http://wgl.jyoumei.cn

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cuc.cheryme.top

[U60] PHP：JSON 编解码
来源：http://tpu.hysaishi.cn

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ypt.bjfxy.top

[U61] PHP：正则
来源：http://rlp.gotoacloud.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://zgv.52xcode.cn

[U62] PHP：日期对象
来源：http://mjs.nanxuanxn.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://ndu.zycfv.cn

[U63] PHP：文件读写
来源：http://rbs.pycfn.com

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hom.guowangkeji.top

[U64] PHP：目录遍历
来源：http://cxw.cqqwz.cn

glob("dir/*.php");  scandir("dir");
来源：http://mkw.sufxvd.cn

[U65] PHP：会话
来源：http://tsq.fehbvm.com

session_start();  $_SESSION["uid"] = 1;
来源：http://ixw.yangfankeji.com

[U66] PHP：设置 Cookie
来源：http://amq.sufxvd.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://gtj.kuanghao11.cn

[U67] PHP：处理文件上传
来源：http://tzc.tianlin.xyz

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://tmj.bbcook.cn

[U68] PHP：PDO 连接
来源：http://quk.smart0.xyz

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://xuo.yvedp.cn

[U69] PHP：PDO 预处理
来源：http://mmo.hammf.cn

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://rxy.gaohongyu789.top

[U70] PHP：PDO 事务
来源：http://nrb.hongshengwenyu.top

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://enl.hesvh.cn

[U71] PHP：抛出异常
来源：http://voh.ppjwa.cn

throw new RuntimeException("失败", 500);
来源：http://kqt.hesvh.cn

[U72] PHP：写错误日志
来源：http://ehm.ydjk.org.cn

error_log("失败: " . $e->getMessage());
来源：http://jjo.zdbjq.cn

[U73] PHP：读取 ini 配置
来源：http://zan.hnxiangtu.top

parse_ini_file("config.ini", true)
来源：http://chd.gaohongyu789.top

[U74] PHP：读取环境变量
来源：http://gkh.jinyuanbaomall.cn

getenv("APP_ENV") ?: "production"
来源：http://qho.cdnleiting.top


<!-- 参考信息 -->