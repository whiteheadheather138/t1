代发 wailian999

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fhj.hcnkem.com

[S51] C++：显式类型转换
来源：http://lce.ydzc1.top

static_cast<double>(a) / b
来源：http://awq.guannengcc.top

[S52] C++：const 与 noexcept
来源：http://yny.pengpengdd.cyou

int size() const noexcept { return n_; }
来源：http://tkg.zhaomingkeji.xyz

[S53] C++：移动语义
来源：http://euh.ehwqpu.com

std::vector<int> w = std::move(v);
来源：http://fwe.yangfankeji.com

[S54] C++：异常处理
来源：http://fpg.bjfxy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pxe.jiagoushi.top

[S55] C++：结构化绑定
来源：http://ucg.ydzc1.top

auto [a, b] = std::make_pair(1, 2);
来源：http://caq.shzxlz.cn

[S56] C++：optional
来源：http://llw.tarul.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ogb.iojbl.cn

[S57] C++：编译期常量
来源：http://cjc.pycfn.com

constexpr int N = 10;
来源：http://tla.haohaochexian.top

[S58] C++：命名空间
来源：http://dwp.9152youxi.cn

namespace ns { int f() { return 1; } }
来源：http://ogd.xingfuxueyuan.xyz

[S59] C++：静态断言
来源：http://khx.hywenlv.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kyk.yuanzhike.top

[S60] C++：遍历并删除元素
来源：http://xje.hysaishi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://aoo.zhongyouzk.top

================================================================================
来源：http://lyl.0kj1m.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kjk.0kj1m.cn

================================================================================
来源：http://cma.fanxiaobao.xyz

[T01] Kotlin：Hello World
来源：http://xlx.zdbjq.cn

println("Hello")
来源：http://zpq.svipenyu.cn

[T02] Kotlin：变量
来源：http://hui.feifeiyinyue.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://guz.svipenyu.cn

[T03] Kotlin：字符串模板
来源：http://sme.yongpay.top

"值: $b"
来源：http://pdc.ywan-chungtsiang.top

[T04] Kotlin：空安全
来源：http://azw.shangyingyoupin.top

val n: String? = null;  n?.length
来源：http://pcr.hysaishi.cn

[T05] Kotlin：when 表达式
来源：http://bud.redwolf501.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qhx.zhiwuduotai.top

[T06] Kotlin：集合映射
来源：http://iqd.sysykeji.top

listOf(1, 2, 3).map { it * 2 }
来源：http://kgy.c1oappe.top

[T07] Kotlin：集合过滤
来源：http://ygm.xziqi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xzc.zhixingplan.top

[T08] Kotlin：数据类
来源：http://lme.xylfe.cn

data class User(val name: String, val age: Int)
来源：http://lwh.hfpthk.cn

[T09] Kotlin：扩展函数
来源：http://xft.epnwcf.com

fun String.exclaim() = this + "!"
来源：http://pzf.hammf.cn

[T10] Kotlin：默认参数
来源：http://egl.ywan-chungtsiang.top

fun greet(name: String = "World") = "Hi $name"
来源：http://dvj.chenjidiqi.icu

[T11] Kotlin：协程
来源：http://sqk.zhongyouzk.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://kys.shanyushiyangtech.top

[T12] Kotlin：解构声明
来源：http://lor.hcnkem.com

val (a, b) = Pair(1, 2)
来源：http://byi.cqqwz.cn

[T13] Kotlin：只读 Map
来源：http://gnw.fengsongda.top

val m = mapOf("a" to 1)
来源：http://brk.guowangkeji.top

[T14] Kotlin：循环
来源：http://usb.pycfn.com

for (i in 1..10) println(i)
来源：http://prd.cqqwz.cn

[T15] Kotlin：接口
来源：http://tty.fzhhl.top

interface Shape { fun area(): Double }
来源：http://ngd.svipenyu.cn

[T16] Swift：Hello World
来源：http://hve.haohaochexian.top

print("Hello")
来源：http://upz.zhongyouzk.top

[T17] Swift：变量与常量
来源：http://olw.wangdashe.top

var a = 1;  let b = 2
来源：http://epg.ywan-chungtsiang.top

[T18] Swift：字符串插值
来源：http://yvl.shangyingyoupin.top

"值: \(b)"
来源：http://fry.yj20258888.top

[T19] Swift：可选绑定
来源：http://zkx.sxryk.cn

if let n = opt { print(n) }
来源：http://url.guowangkeji.top

[T20] Swift：数组操作
来源：http://xqg.cashguo.top

var a = [1, 2, 3];  a.append(4)
来源：http://edr.bjfxy.top

[T21] Swift：遍历
来源：http://gov.meibo888.top

for x in a { print(x) }
来源：http://yof.sysykeji.top

[T22] Swift：字典
来源：http://fhf.zhoulong.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://kcf.tanke756.top

[T23] Swift：函数
来源：http://bll.bbcook.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vye.ivvv.top

[T24] Swift：闭包
来源：http://mgy.xuetiantiany.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://tut.wangdashe.top

[T25] Swift：结构体
来源：http://qnp.zdbjq.cn

struct P { var x: Int }
来源：http://qxh.snrcjt.cn

[T26] Swift：类与重写
来源：http://hgy.jiagoushi.top

class A: Base { override func f() {} }
来源：http://jur.yj202588.top

[T27] Swift：错误处理
来源：http://bev.zhoulong.xyz

do { try f() } catch { print(error) }
来源：http://emo.zdbjq.cn

[T28] Swift：枚举
来源：http://yks.yfazqb.com

enum Color { case red, green }
来源：http://uix.9152youxi.cn

[T29] Swift：guard 提前返回
来源：http://xyf.xziqi.cn

guard let x = opt else { return }
来源：http://vku.9152youxi.cn

[T30] Swift：协议
来源：http://rvm.xziqi.cn

protocol Shape { func area() -> Double }
来源：http://ggv.dianchejie.cn

[T31] Lua：Hello World
来源：http://ist.yueranfly.top

print("Hello")
来源：http://osw.jinqigufen.top

[T32] Lua：局部变量
来源：http://fog.sysykeji.top

local a = 1
来源：http://psc.fzhhl.top

[T33] Lua：表（数组）
来源：http://psh.tian-w.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://gfn.ybcxt.top

[T34] Lua：遍历表
来源：http://vqj.feifeiyinyue.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ojs.hnxiangtu.top

[T35] Lua：字典表
来源：http://fgz.hcnkem.com

local d = { a = 1 };  d.b = 2
来源：http://goy.svipenyu.cn

[T36] Lua：函数
来源：http://mop.hongshengwenyu.top

function add(a, b) return a + b end
来源：http://trz.zhiwuduotai.top

[T37] Lua：字符串拼接
来源：http://emf.nanxinkj.top

"a" .. "b"
来源：http://xrz.shuidangran.top

[T38] Lua：条件
来源：http://ras.fengsongda.top

if x > 0 then print("正") end
来源：http://lto.vqdsnc.cn

[T39] Lua：模式匹配
来源：http://mif.yj202588.top

string.find(s, "%d+")
来源：http://ueb.yvedp.cn

[T40] Lua：元表
来源：http://cdj.gaohongyu789.top

setmetatable({}, { __index = base })
来源：http://mpb.jlsjyb.cn

[T41] Perl：Hello World
来源：http://rdd.uphjek.com

print "Hello\n";
来源：http://nfz.mhx1999.top

[T42] Perl：变量类型
来源：http://ngv.xylfe.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tbd.mhx1999.top

[T43] Perl：字符串插值
来源：http://ctm.iojbl.cn

"值: $a"
来源：http://fes.xuanzx.com

[T44] Perl：条件
来源：http://ipr.nanxinkj.top

if ($a > 0) { print "正"; }
来源：http://lmg.c1oappe.top

[T45] Perl：数组遍历
来源：http://xhu.tarul.cn

for my $x (@arr) { print $x; }
来源：http://ayg.uphjek.com

[T46] Perl：哈希操作
来源：http://zoo.yfazqb.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wsh.yongpay.top

[T47] Perl：正则捕获
来源：http://nag.gotoacloud.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://hiv.bbcook.cn

[T48] Perl：正则替换
来源：http://hnz.hywenlv.cn

$s =~ s/old/new/g;
来源：http://cdr.jiagoushi.top

[T49] Perl：函数
来源：http://vnl.zhaomingkeji.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qgu.gzhubu.top

[T50] Perl：逐行读文件
来源：http://nte.c1oappe.top

open my $fh, "<", "a.txt" or die $!;
来源：http://pmi.zhongyouzk.top

while (my $line = <$fh>) { print $line; }
来源：http://xsq.shanyushiyangkeji.top

[T51] Scala：Hello World
来源：http://duc.aizwys.cn

println("Hello")
来源：http://pld.ivvv.top

[T52] Scala：变量
来源：http://itq.aizwys.cn

val a = 1;  var b = 2
来源：http://oyi.ctjpmb.com

[T53] Scala：字符串插值
来源：http://gkg.fktsv.cn

s"值: $b"
来源：http://wyr.zhoulong.xyz

[T54] Scala：集合映射
来源：http://slc.ydzc1.top

List(1, 2, 3).map(_ * 2)
来源：http://txb.quarkkingdee.top

[T55] Scala：集合过滤
来源：http://lzk.dashuyun.cn

List(1, 2, 3).filter(_ > 1)
来源：http://yhk.guannengcc.top

[T56] Scala：样例类
来源：http://pbl.tian-w.cn

case class User(name: String, age: Int)
来源：http://gor.jinqigfzy.top

[T57] Scala：模式匹配
来源：http://gpu.sysykeji.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ana.zhengqikj.top

[T58] Scala：函数定义
来源：http://rdp.jlsjyb.cn

def add(a: Int, b: Int): Int = a + b
来源：http://sta.daxiang520.top

[T59] Scala：循环
来源：http://zyk.jianghu66.top

for (i <- 1 to 10) println(i)
来源：http://luq.xziqi.cn

[T60] Scala：折叠
来源：http://emq.gaohongyu789.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vuo.yongpay.top

================================================================================
来源：http://iya.yueranfly.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nfe.jlsjyb.cn

================================================================================
来源：http://fup.jinyuanbaomall.cn

[U01] Py：创建虚拟环境
来源：http://ddw.ywan-chungtsiang.top

python -m venv .venv && source .venv/bin/activate
来源：http://tif.aizwys.cn

[U02] Py：导出 / 安装依赖
来源：http://vry.sweek.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yag.hammf.cn

[U03] Py：加载 .env 配置
来源：http://fxc.jqgfzy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://vpq.jinqigfzy.top

[U04] Py：变量调试打印
来源：http://ljk.zhiwuduotai.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nhi.zhoulong.xyz

[U05] Py：列表去重且保序
来源：http://fvd.zhiwuduotai.top

list(dict.fromkeys(arr))
来源：http://uqw.zhaomingkeji.xyz

[U06] Py：合并两个字典
来源：http://amy.birdmap.top

{**a, **b}
来源：http://ezt.sysykeji.top

[U07] Py：反转字典键值
来源：http://cae.quarkkingdee.top

{v: k for k, v in d.items()}
来源：http://cuo.zdqjudy.top

[U08] Py：展平二维列表
来源：http://fqd.zdqjudy.top

[y for x in nested for y in x]
来源：http://wgi.guannengcc.top

[U09] Py：字典取最大值的键
来源：http://fjp.ywan-chungtsiang.top

max(d, key=d.get)
来源：http://ppr.hfpthk.cn

[U10] Py：按值排序字典
来源：http://wwx.jinqigufen.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qtm.svipenyu.cn

[U11] Py：生成器表达式
来源：http://jke.jianghu66.top

(x * 2 for x in arr)
来源：http://old.zdqjudy.top

[U12] Py：取出现最多的 3 个元素
来源：http://gvb.yvedp.cn

Counter(arr).most_common(3)
来源：http://pfx.feifeiyinyue.top

[U13] Py：固定长度队列
来源：http://nbn.yvedp.cn

deque(maxlen=10)
来源：http://myu.zhongyouzk.top

[U14] Py：分组收集到列表
来源：http://wvo.cashguo.top

defaultdict(list)
来源：http://zte.hammf.cn

[U15] Py：高精度计时
来源：http://fqb.yuxming.cn

t = time.perf_counter()
来源：http://irw.hesvh.cn

[U16] Py：命令行参数解析
来源：http://ohx.ivvv.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vqq.svipenyu.cn

[U17] Py：初始化日志
来源：http://izg.yj20258.top

logging.basicConfig(level=logging.INFO)
来源：http://fpf.nanxinkj.top

[U18] Py：预编译正则
来源：http://okn.gotoacloud.top

pat = re.compile(r"\d+")
来源：http://lhy.pengpengdd.cyou

[U19] Py：正则替换带回调
来源：http://rbg.ybcxt.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ntg.yj20258.top

[U20] Py：缓存函数结果
来源：http://lwp.daxiang520.top

@functools.lru_cache(maxsize=None)
来源：http://lzk.redwolf501.top

[U21] Py：自定义上下文管理器
来源：http://guf.iojbl.cn

@contextlib.contextmanager
来源：http://zyn.aizwys.cn

[U22] Py：矩阵转置
来源：http://gdj.jinyuanbaomall.cn

list(zip(*m))
来源：http://zll.bjfxy.top

[U23] Py：分块读取大文件
来源：http://lsn.chenjidiqi.icu

for chunk in iter(lambda: f.read(8192), b""):
来源：http://uuu.jinqigfzy.top

[U24] Py：路径操作
来源：http://pxa.epnwcf.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ipx.guowangkeji.top

[U25] Py：CSV 按字典读
来源：http://quk.ybcxt.top

csv.DictReader(f)
来源：http://eqb.fzhhl.top

[U26] Py：并发下载
来源：http://fsh.zhoulong.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ntw.wangshuangyany.cn

[U27] Py：异步 HTTP
来源：http://uux.aibaodan.cn

aiohttp.ClientSession() 配合 async with
来源：http://lki.quarkkingdee.top

[U28] Py：类型别名
来源：http://rit.jinghuilouyu.cn

UserId = int
来源：http://dhe.tarul.cn

[U29] Py：属性校验
来源：http://vhe.zhengqikj.top

@property 与 @x.setter 配合
来源：http://rpc.ydjk.org.cn

[U30] Py：数据类
来源：http://hle.316326.xyz

@dataclass(slots=True)
来源：http://gxu.ctjpmb.com

[U31] Py：单测
来源：http://qtd.zhixingplan.top

python -m pytest -q
来源：http://qhh.0kj1m.cn

[U32] Py：代码格式化
来源：http://nzi.jianghu66.top

ruff format . && ruff check --fix .
来源：http://hfz.ctjpmb.com

[U33] Py：打包发布
来源：http://acv.fzhhl.top

python -m build  （依赖 pyproject.toml）
来源：http://ism.yangfankeji.com

[U34] Py：判断编码
来源：http://wgu.meibo888.top

chardet.detect(raw)
来源：http://ifr.havefunace.top

[U35] Py：发送邮件
来源：http://znn.jqgfzy.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://wmo.yangfankeji.com

[U36] Py：定时任务
来源：http://lqz.tanke756.top

schedule.every(10).minutes.do(job)
来源：http://rkw.redwolf501.top

[U37] Py：读写 Excel
来源：http://jaf.fehbvm.com

pandas.read_excel / DataFrame.to_excel
来源：http://aup.uphjek.com

[U38] Py：获取脚本所在目录
来源：http://tgh.yanxiufei.cn

Path(__file__).resolve().parent
来源：http://cfx.dianchejie.cn

[U39] Py：判断是否在交互环境
来源：http://xri.xylfe.cn

sys.stdout.isatty()
来源：http://zjp.jinghuilouyu.cn

[U40] Py：打印到标准错误
来源：http://vkj.ppjwa.cn

print("err", file=sys.stderr)
来源：http://ske.fengsongda.top

[U41] PHP：初始化 Composer 项目
来源：http://rgx.sxryk.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://anl.zhoulong.xyz

[U42] PHP：PSR-4 自动加载
来源：http://fxp.yj202588.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://unc.tianlin.xyz

[U43] PHP：声明命名空间
来源：http://mwj.ydzc1.top

namespace App\Http;
来源：http://esj.yongpay.top

[U44] PHP：开启严格类型
来源：http://otn.xingfuxueyuan.xyz

declare(strict_types=1);
来源：http://ddt.vehdjk.com

[U45] PHP：类型声明与返回类型
来源：http://iiq.yueranfly.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ilb.ctjpmb.com

[U46] PHP：可空类型
来源：http://qir.yuanzhike.top

?string $name = null
来源：http://yof.daria6918.cn

[U47] PHP：联合类型
来源：http://cwm.zhixingplan.top

int|string $id
来源：http://xzd.tian-w.cn

[U48] PHP：纯枚举
来源：http://wdt.yj20258888.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ygo.guowangkeji.top

[U49] PHP：只读属性
来源：http://jci.bjfxy.top

public readonly string $name
来源：http://xxs.jinqigfzy.top

[U50] PHP：构造器属性提升
来源：http://jkh.meibo888.top

public function __construct(private int $id) {}
来源：http://gsd.gogol.net.cn

[U51] PHP：数组解构
来源：http://dpu.jqgufenzy.top

[$a, $b] = $arr;
来源：http://jzm.pengpengdd.cyou

[U52] PHP：箭头函数
来源：http://zwu.yvedp.cn

$double = fn($x) => $x * 2;
来源：http://qqp.sjlbkw.cn

[U53] PHP：空合并运算符
来源：http://kio.hysaishi.cn

$v = $a ?? $b ?? "default";
来源：http://lat.52xcode.cn

[U54] PHP：空安全调用
来源：http://ubw.yanxiufei.cn

$obj?->method()
来源：http://sug.316326.xyz

[U55] PHP：match 表达式
来源：http://sdn.cheryme.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vrg.fengsongda.top

[U56] PHP：命名参数
来源：http://ozv.fktsv.cn

f(a: 1, b: 2)
来源：http://tat.cashguo.top

[U57] PHP：字符串插值
来源：http://ffr.shuidangran.top

"值: {$a}"
来源：http://bfx.yfazqb.com

[U58] PHP：数组三件套
来源：http://rcz.ydzc1.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ndf.shzxlz.cn

[U59] PHP：自定义排序
来源：http://jmw.havefunace.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://uhg.yuxming.cn

[U60] PHP：JSON 编解码
来源：http://wbh.chenlongwang.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://sgp.fzhhl.top

[U61] PHP：正则
来源：http://phg.xylfe.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wwh.fktsv.cn

[U62] PHP：日期对象
来源：http://yec.yangfankeji.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nwg.zhaomingkeji.xyz

[U63] PHP：文件读写
来源：http://ejj.xuetiantiany.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://del.jiagoushi.top

[U64] PHP：目录遍历
来源：http://phb.cdnleiting.top

glob("dir/*.php");  scandir("dir");
来源：http://hcb.ctjpmb.com

[U65] PHP：会话
来源：http://zjv.svipenyu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://vvm.zdbjq.cn

[U66] PHP：设置 Cookie
来源：http://eez.xinyue.icu

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://qgg.pycfn.com

[U67] PHP：处理文件上传
来源：http://ons.hammf.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://rvi.hnxiangtu.top

[U68] PHP：PDO 连接
来源：http://pyk.yvedp.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://lal.quarkkingdee.top

[U69] PHP：PDO 预处理
来源：http://sia.fanxiaobao.xyz

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mhq.wangdashe.top

[U70] PHP：PDO 事务
来源：http://zdh.shzxlz.cn

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://qfn.cucudq.cn

[U71] PHP：抛出异常
来源：http://pfp.vqdsnc.cn

throw new RuntimeException("失败", 500);
来源：http://znp.tanke756.top

[U72] PHP：写错误日志
来源：http://yfa.fehbvm.com

error_log("失败: " . $e->getMessage());
来源：http://cdq.hcnkem.com

[U73] PHP：读取 ini 配置
来源：http://ikr.iojbl.cn

parse_ini_file("config.ini", true)
来源：http://jnk.bjfxy.top

[U74] PHP：读取环境变量
来源：http://qjy.sweek.top

getenv("APP_ENV") ?: "production"
来源：http://gwa.yonumen.top

[U75] PHP：依赖注入
来源：http://bcv.cashguo.top

composer require psr/container
来源：http://ayl.tanke756.top

[U76] PHP：简单路由
来源：http://jpi.yonumen.top

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://pbt.fanxiaobao.xyz


<!-- 参考信息 -->