代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fsy.jqgufenzy.top

[S51] C++：显式类型转换
来源：http://cjw.zdqjudy.top

static_cast<double>(a) / b
来源：http://lzq.jinyuanbaomall.cn

[S52] C++：const 与 noexcept
来源：http://yxe.jqgufenzy.top

int size() const noexcept { return n_; }
来源：http://tgl.0kj1m.cn

[S53] C++：移动语义
来源：http://wft.wangdashe.top

std::vector<int> w = std::move(v);
来源：http://eek.mhx1999.top

[S54] C++：异常处理
来源：http://msq.smart0.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lir.zhoulong.xyz

[S55] C++：结构化绑定
来源：http://egf.yj20258.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ywn.zhengqikj.top

[S56] C++：optional
来源：http://tyy.jianghu66.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zll.zdbjq.cn

[S57] C++：编译期常量
来源：http://rfl.sjlbkw.cn

constexpr int N = 10;
来源：http://cox.yangfankeji.com

[S58] C++：命名空间
来源：http://fgo.vqdsnc.cn

namespace ns { int f() { return 1; } }
来源：http://mkj.kuanghao11.cn

[S59] C++：静态断言
来源：http://zqy.snrcjt.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gzf.hysaishi.cn

[S60] C++：遍历并删除元素
来源：http://uvm.jyoumei.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tql.ehwqpu.com

================================================================================
来源：http://yrg.yonumen.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ylv.hcnkem.com

================================================================================
来源：http://gbm.jqgufenzy.top

[T01] Kotlin：Hello World
来源：http://tjz.xuetiantiany.cn

println("Hello")
来源：http://ztc.aizwys.cn

[T02] Kotlin：变量
来源：http://kza.hcnkem.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dcd.daria6918.cn

[T03] Kotlin：字符串模板
来源：http://shc.zdqjudy.top

"值: $b"
来源：http://xhj.aizwys.cn

[T04] Kotlin：空安全
来源：http://owu.zhaomingkeji.xyz

val n: String? = null;  n?.length
来源：http://kcb.yongpay.top

[T05] Kotlin：when 表达式
来源：http://ikb.jlsjyb.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yxk.yfazqb.com

[T06] Kotlin：集合映射
来源：http://hqn.hfpthk.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ubk.yonumen.top

[T07] Kotlin：集合过滤
来源：http://mbt.jianghu66.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://udw.yfazqb.com

[T08] Kotlin：数据类
来源：http://nyx.guannengcc.top

data class User(val name: String, val age: Int)
来源：http://icp.sjlbkw.cn

[T09] Kotlin：扩展函数
来源：http://ovw.zhongyouzk.top

fun String.exclaim() = this + "!"
来源：http://kqf.meibo888.top

[T10] Kotlin：默认参数
来源：http://qgi.daria6918.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://fmx.birdmap.top

[T11] Kotlin：协程
来源：http://tnj.dashuyun.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://gpc.jinyuanbaomall.cn

[T12] Kotlin：解构声明
来源：http://eof.mhx1999.top

val (a, b) = Pair(1, 2)
来源：http://vdg.bjfxy.top

[T13] Kotlin：只读 Map
来源：http://kdr.xylfe.cn

val m = mapOf("a" to 1)
来源：http://zvw.ydjk.org.cn

[T14] Kotlin：循环
来源：http://oyj.bjfxy.top

for (i in 1..10) println(i)
来源：http://gpq.yuxming.cn

[T15] Kotlin：接口
来源：http://evf.jqgufenzy.top

interface Shape { fun area(): Double }
来源：http://cos.xuetiantiany.cn

[T16] Swift：Hello World
来源：http://ssg.sxryk.cn

print("Hello")
来源：http://bkh.9152youxi.cn

[T17] Swift：变量与常量
来源：http://oyq.hesvh.cn

var a = 1;  let b = 2
来源：http://haj.chenzaomai.com

[T18] Swift：字符串插值
来源：http://ggh.fanxiaobao.xyz

"值: \(b)"
来源：http://scm.shanyushiyangtech.top

[T19] Swift：可选绑定
来源：http://tdv.yfazqb.com

if let n = opt { print(n) }
来源：http://dzx.shangyingyoupin.top

[T20] Swift：数组操作
来源：http://lpz.zhongyouzk.top

var a = [1, 2, 3];  a.append(4)
来源：http://klr.meibo888.top

[T21] Swift：遍历
来源：http://wcc.jianghu66.top

for x in a { print(x) }
来源：http://cbb.jiagoushi.top

[T22] Swift：字典
来源：http://khu.xingfuxueyuan.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://akq.hesvh.cn

[T23] Swift：函数
来源：http://gkj.kuanghao11.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ybf.jinqigufen.top

[T24] Swift：闭包
来源：http://nif.chenjidiqi.icu

let f = { (x: Int) -> Int in x * 2 }
来源：http://fqz.nanxinkj.top

[T25] Swift：结构体
来源：http://jtl.shanyushiyangkeji.top

struct P { var x: Int }
来源：http://jhb.jiagoushi.top

[T26] Swift：类与重写
来源：http://jge.dianchejie.cn

class A: Base { override func f() {} }
来源：http://vsa.cashguo.top

[T27] Swift：错误处理
来源：http://ndk.ydzc1.top

do { try f() } catch { print(error) }
来源：http://elu.bjfxy.top

[T28] Swift：枚举
来源：http://lkb.fzhhl.top

enum Color { case red, green }
来源：http://ieb.jqgfzy.top

[T29] Swift：guard 提前返回
来源：http://xvc.c1oappe.top

guard let x = opt else { return }
来源：http://ebp.jianghu66.top

[T30] Swift：协议
来源：http://qoh.smart0.xyz

protocol Shape { func area() -> Double }
来源：http://hvc.jiagoushi.top

[T31] Lua：Hello World
来源：http://fjp.shanyushiyangkeji.top

print("Hello")
来源：http://qtt.shzxlz.cn

[T32] Lua：局部变量
来源：http://nap.52xcode.cn

local a = 1
来源：http://wqt.0kj1m.cn

[T33] Lua：表（数组）
来源：http://pxi.pycfn.com

local t = {1, 2, 3};  t[4] = 4
来源：http://acl.xinyue.icu

[T34] Lua：遍历表
来源：http://pit.svipenyu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://riw.jinghuilouyu.cn

[T35] Lua：字典表
来源：http://mhe.shzxlz.cn

local d = { a = 1 };  d.b = 2
来源：http://dpd.jqgfzy.top

[T36] Lua：函数
来源：http://egg.hesvh.cn

function add(a, b) return a + b end
来源：http://tza.jinyuanbaomall.cn

[T37] Lua：字符串拼接
来源：http://qxa.sufxvd.cn

"a" .. "b"
来源：http://wfh.0kj1m.cn

[T38] Lua：条件
来源：http://jdn.hnqzz.top

if x > 0 then print("正") end
来源：http://kll.sxryk.cn

[T39] Lua：模式匹配
来源：http://hgc.jqgufenzy.top

string.find(s, "%d+")
来源：http://pvt.cucudq.cn

[T40] Lua：元表
来源：http://jeo.sweek.top

setmetatable({}, { __index = base })
来源：http://onb.mhx1999.top

[T41] Perl：Hello World
来源：http://fpj.ppjwa.cn

print "Hello\n";
来源：http://lgp.epnwcf.com

[T42] Perl：变量类型
来源：http://upv.yj20258888.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tvh.xziqi.cn

[T43] Perl：字符串插值
来源：http://hok.zhiwuduotai.top

"值: $a"
来源：http://flj.hesvh.cn

[T44] Perl：条件
来源：http://ucs.sufxvd.cn

if ($a > 0) { print "正"; }
来源：http://gmm.yongpay.top

[T45] Perl：数组遍历
来源：http://dlb.c1oappe.top

for my $x (@arr) { print $x; }
来源：http://tei.sweek.top

[T46] Perl：哈希操作
来源：http://zuo.jyoumei.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://squ.xuetiantiany.cn

[T47] Perl：正则捕获
来源：http://ebg.52xcode.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://gxp.52xcode.cn

[T48] Perl：正则替换
来源：http://jkw.jinghuilouyu.cn

$s =~ s/old/new/g;
来源：http://mpw.ctjpmb.com

[T49] Perl：函数
来源：http://ous.yvedp.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://urv.cucudq.cn

[T50] Perl：逐行读文件
来源：http://hct.nwbrower.top

open my $fh, "<", "a.txt" or die $!;
来源：http://wus.ywan-chungtsiang.top

while (my $line = <$fh>) { print $line; }
来源：http://vbt.tian-w.cn

[T51] Scala：Hello World
来源：http://lqd.yuxming.cn

println("Hello")
来源：http://dfm.fanxiaobao.xyz

[T52] Scala：变量
来源：http://quh.ydzc1.top

val a = 1;  var b = 2
来源：http://rys.ywan-chungtsiang.top

[T53] Scala：字符串插值
来源：http://qkg.shuidangran.top

s"值: $b"
来源：http://ikw.guowangkeji.top

[T54] Scala：集合映射
来源：http://dwk.c1oappe.top

List(1, 2, 3).map(_ * 2)
来源：http://qgi.dashuyun.cn

[T55] Scala：集合过滤
来源：http://ahp.jlsjyb.cn

List(1, 2, 3).filter(_ > 1)
来源：http://eca.fanxiaobao.xyz

[T56] Scala：样例类
来源：http://hmo.zhiwuduotai.top

case class User(name: String, age: Int)
来源：http://jza.cheryme.top

[T57] Scala：模式匹配
来源：http://jmt.zdbjq.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ygy.yj202588.top

[T58] Scala：函数定义
来源：http://war.jianghu66.top

def add(a: Int, b: Int): Int = a + b
来源：http://ykm.jqgfzy.top

[T59] Scala：循环
来源：http://jrz.yvedp.cn

for (i <- 1 to 10) println(i)
来源：http://vnp.aizwys.cn

[T60] Scala：折叠
来源：http://cob.yongpay.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qiu.mhx1999.top

================================================================================
来源：http://ebb.wangshuangyany.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qva.redwolf501.top

================================================================================
来源：http://enq.dashuyun.cn

[U01] Py：创建虚拟环境
来源：http://apl.kuanghao11.cn

python -m venv .venv && source .venv/bin/activate
来源：http://zhp.daria6918.cn

[U02] Py：导出 / 安装依赖
来源：http://lep.kuanghao11.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mdv.0kj1m.cn

[U03] Py：加载 .env 配置
来源：http://qpj.c1oappe.top

from dotenv import load_dotenv; load_dotenv()
来源：http://blh.tarul.cn

[U04] Py：变量调试打印
来源：http://hnv.316326.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://oks.zhoulong.xyz

[U05] Py：列表去重且保序
来源：http://txg.sysykeji.top

list(dict.fromkeys(arr))
来源：http://ldx.cucudq.cn

[U06] Py：合并两个字典
来源：http://yvn.jianghu66.top

{**a, **b}
来源：http://wdj.pycfn.com

[U07] Py：反转字典键值
来源：http://qpe.316326.xyz

{v: k for k, v in d.items()}
来源：http://cjl.hysaishi.cn

[U08] Py：展平二维列表
来源：http://rom.jiagoushi.top

[y for x in nested for y in x]
来源：http://hlm.yongpay.top

[U09] Py：字典取最大值的键
来源：http://zjf.nanxinkj.top

max(d, key=d.get)
来源：http://faa.cashguo.top

[U10] Py：按值排序字典
来源：http://lxc.nanxinkj.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zzq.chenlongwang.top

[U11] Py：生成器表达式
来源：http://ntv.xziqi.cn

(x * 2 for x in arr)
来源：http://hiv.zhiwuduotai.top

[U12] Py：取出现最多的 3 个元素
来源：http://ves.zhengqikj.top

Counter(arr).most_common(3)
来源：http://zkk.ehwqpu.com

[U13] Py：固定长度队列
来源：http://dca.andypj.xyz

deque(maxlen=10)
来源：http://qrg.birdmap.top

[U14] Py：分组收集到列表
来源：http://aik.jinqigufen.top

defaultdict(list)
来源：http://ktf.hysaishi.cn

[U15] Py：高精度计时
来源：http://odq.jinqigufen.top

t = time.perf_counter()
来源：http://nrq.zhongyouzk.top

[U16] Py：命令行参数解析
来源：http://sdu.cqqwz.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qli.guannengcc.top

[U17] Py：初始化日志
来源：http://tga.yongpay.top

logging.basicConfig(level=logging.INFO)
来源：http://soo.epnwcf.com

[U18] Py：预编译正则
来源：http://nqf.gotoacloud.top

pat = re.compile(r"\d+")
来源：http://sux.nanxinkj.top

[U19] Py：正则替换带回调
来源：http://vno.cqqwz.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tkm.hfpthk.cn

[U20] Py：缓存函数结果
来源：http://mdz.wangdashe.top

@functools.lru_cache(maxsize=None)
来源：http://peq.yj20258888.top

[U21] Py：自定义上下文管理器
来源：http://waa.gogol.net.cn

@contextlib.contextmanager
来源：http://mvs.tanke756.top

[U22] Py：矩阵转置
来源：http://yzu.guowangkeji.top

list(zip(*m))
来源：http://zoc.hongshengwenyu.top

[U23] Py：分块读取大文件
来源：http://zbr.fktsv.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rhz.yfazqb.com

[U24] Py：路径操作
来源：http://ffh.chenzaomai.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qfm.xylfe.cn

[U25] Py：CSV 按字典读
来源：http://psy.aizwys.cn

csv.DictReader(f)
来源：http://tyq.wangshuangyany.cn

[U26] Py：并发下载
来源：http://iqy.jqgufenzy.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://nbd.kuanghao11.cn

[U27] Py：异步 HTTP
来源：http://hzk.pycfn.com

aiohttp.ClientSession() 配合 async with
来源：http://afq.mhx1999.top

[U28] Py：类型别名
来源：http://aju.wangshuangyany.cn

UserId = int
来源：http://uug.jinyuanbaomall.cn

[U29] Py：属性校验
来源：http://qrh.hammf.cn

@property 与 @x.setter 配合
来源：http://sva.dashuyun.cn

[U30] Py：数据类
来源：http://uas.zycfv.cn

@dataclass(slots=True)
来源：http://dkg.cucudq.cn

[U31] Py：单测
来源：http://xgd.hywenlv.cn

python -m pytest -q
来源：http://yek.quarkkingdee.top

[U32] Py：代码格式化
来源：http://fkn.hnxiangtu.top

ruff format . && ruff check --fix .
来源：http://ymf.yuanzhike.top

[U33] Py：打包发布
来源：http://ydc.jqgufenzy.top

python -m build  （依赖 pyproject.toml）
来源：http://ijo.yj20258888.top

[U34] Py：判断编码
来源：http://piy.wangdashe.top

chardet.detect(raw)
来源：http://est.cashguo.top

[U35] Py：发送邮件
来源：http://lii.yuxming.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ved.jinyuanbaomall.cn

[U36] Py：定时任务
来源：http://vmj.zhiwuduotai.top

schedule.every(10).minutes.do(job)
来源：http://ipm.c1oappe.top

[U37] Py：读写 Excel
来源：http://qhj.fktsv.cn

pandas.read_excel / DataFrame.to_excel
来源：http://yal.shanyushiyangkeji.top

[U38] Py：获取脚本所在目录
来源：http://wmi.wangdashe.top

Path(__file__).resolve().parent
来源：http://tcp.zhaomingkeji.xyz

[U39] Py：判断是否在交互环境
来源：http://oxb.sweek.top

sys.stdout.isatty()
来源：http://izk.chenzaomai.com

[U40] Py：打印到标准错误
来源：http://lsg.smart0.xyz

print("err", file=sys.stderr)
来源：http://bis.kuanghao11.cn

[U41] PHP：初始化 Composer 项目
来源：http://uzk.zhiwuduotai.top

composer init;  composer require guzzlehttp/guzzle
来源：http://prf.bbcook.cn

[U42] PHP：PSR-4 自动加载
来源：http://eik.fktsv.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://akc.daxiang520.top

[U43] PHP：声明命名空间
来源：http://lrp.dashuyun.cn

namespace App\Http;
来源：http://rtb.uphjek.com

[U44] PHP：开启严格类型
来源：http://cfs.iojbl.cn

declare(strict_types=1);
来源：http://fmd.ctjpmb.com

[U45] PHP：类型声明与返回类型
来源：http://bpa.fanxiaobao.xyz

function add(int $a, int $b): int { return $a + $b; }
来源：http://bix.vqdsnc.cn

[U46] PHP：可空类型
来源：http://osj.gzhubu.top

?string $name = null
来源：http://ndc.ctjpmb.com

[U47] PHP：联合类型
来源：http://shs.hongshengwenyu.top

int|string $id
来源：http://ggz.jinyuanbaomall.cn

[U48] PHP：纯枚举
来源：http://war.zdbjq.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://heo.gaohongyu789.top

[U49] PHP：只读属性
来源：http://uti.gogol.net.cn

public readonly string $name
来源：http://pmk.shanyushiyangkeji.top

[U50] PHP：构造器属性提升
来源：http://qkq.jlsjyb.cn

public function __construct(private int $id) {}
来源：http://ddf.hesvh.cn

[U51] PHP：数组解构
来源：http://fyf.andypj.xyz

[$a, $b] = $arr;
来源：http://kcv.hysaishi.cn

[U52] PHP：箭头函数
来源：http://eol.zycfv.cn

$double = fn($x) => $x * 2;
来源：http://uaw.shzxlz.cn

[U53] PHP：空合并运算符
来源：http://slh.cheryme.top

$v = $a ?? $b ?? "default";
来源：http://dek.svipenyu.cn

[U54] PHP：空安全调用
来源：http://lvx.zhiwuduotai.top

$obj?->method()
来源：http://kht.wangshuangyany.cn

[U55] PHP：match 表达式
来源：http://txx.epnwcf.com

$s = match($x) { 1 => "一", default => "其他" };
来源：http://jfx.shzxlz.cn

[U56] PHP：命名参数
来源：http://hku.sxryk.cn

f(a: 1, b: 2)
来源：http://qvt.aibaodan.cn

[U57] PHP：字符串插值
来源：http://pxk.hongshengwenyu.top

"值: {$a}"
来源：http://fzz.ybcxt.top

[U58] PHP：数组三件套
来源：http://rav.xinyue.icu

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://tjt.yanxiufei.cn

[U59] PHP：自定义排序
来源：http://mop.jqgfzy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zoj.yfazqb.com

[U60] PHP：JSON 编解码
来源：http://zqn.uphjek.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://uti.zhongyouzk.top

[U61] PHP：正则
来源：http://ost.yonumen.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lum.jqgufenzy.top

[U62] PHP：日期对象
来源：http://osa.hnxiangtu.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wvg.hfpthk.cn

[U63] PHP：文件读写
来源：http://rwp.jinqigufen.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://bwk.sweek.top

[U64] PHP：目录遍历
来源：http://liv.0kj1m.cn

glob("dir/*.php");  scandir("dir");
来源：http://snl.shanyushiyangtech.top

[U65] PHP：会话
来源：http://vay.cucudq.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://emo.quarkkingdee.top

[U66] PHP：设置 Cookie
来源：http://gzu.daria6918.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://jwr.chenjidiqi.icu

[U67] PHP：处理文件上传
来源：http://mct.nanxuanxn.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://uil.cdnleiting.top

[U68] PHP：PDO 连接
来源：http://fpq.meibo888.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://any.ehwqpu.com

[U69] PHP：PDO 预处理
来源：http://ozi.wangdashe.top

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://oye.andypj.xyz

[U70] PHP：PDO 事务
来源：http://gmr.xziqi.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://zty.zhiwuduotai.top

[U71] PHP：抛出异常
来源：http://dvq.jinqigufen.top

throw new RuntimeException("失败", 500);
来源：http://jae.jyoumei.cn

[U72] PHP：写错误日志
来源：http://irm.jinghuilouyu.cn

error_log("失败: " . $e->getMessage());
来源：http://rpd.nanxuanxn.top

[U73] PHP：读取 ini 配置
来源：http://wsr.redwolf501.top

parse_ini_file("config.ini", true)
来源：http://ait.tian-w.cn

[U74] PHP：读取环境变量
来源：http://fsx.shzxlz.cn

getenv("APP_ENV") ?: "production"
来源：http://xlm.jianghu66.top

[U75] PHP：依赖注入
来源：http://ypv.aibaodan.cn

composer require psr/container
来源：http://ucx.chenjidiqi.icu

[U76] PHP：简单路由
来源：http://mku.zhiwuduotai.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://uvh.zycfv.cn


<!-- 参考信息 -->