代发 wailian999

[S43] C++：智能指针
来源：http://hxl.quarkkingdee.top

auto p = std::make_unique<int>(5);
来源：http://ssb.xylfe.cn

[S44] C++：引用传参
来源：http://nmy.hcnkem.com

void inc(int &x) { ++x; }
来源：http://xek.shzxlz.cn

[S45] C++：lambda
来源：http://lyn.yuanzhike.top

auto add = [](int a, int b) { return a + b; };
来源：http://das.ivvv.top

[S46] C++：函数模板
来源：http://emk.redwolf501.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bfk.iojbl.cn

[S47] C++：结构化绑定遍历
来源：http://nhd.sysykeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yum.cashguo.top

[S48] C++：逐行读文件
来源：http://ogp.guannengcc.top

std::ifstream in("a.txt");  std::string line;
来源：http://zpi.yuxming.cn

while (std::getline(in, line)) { }
来源：http://okc.meibo888.top

[S49] C++：写文件
来源：http://zln.shangyingyoupin.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tnx.andypj.xyz

[S50] C++：格式化数字
来源：http://yza.hnqzz.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vql.meibo888.top

[S51] C++：显式类型转换
来源：http://dms.hysaishi.cn

static_cast<double>(a) / b
来源：http://baa.sysykeji.top

[S52] C++：const 与 noexcept
来源：http://wtv.yangfankeji.com

int size() const noexcept { return n_; }
来源：http://stu.quarkkingdee.top

[S53] C++：移动语义
来源：http://djn.jlsjyb.cn

std::vector<int> w = std::move(v);
来源：http://hjx.yj20258888.top

[S54] C++：异常处理
来源：http://xel.jqgfzy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xzt.pycfn.com

[S55] C++：结构化绑定
来源：http://dob.epnwcf.com

auto [a, b] = std::make_pair(1, 2);
来源：http://buq.vqdsnc.cn

[S56] C++：optional
来源：http://mdb.gzhubu.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tag.316326.xyz

[S57] C++：编译期常量
来源：http://zsv.uphjek.com

constexpr int N = 10;
来源：http://yeg.tian-w.cn

[S58] C++：命名空间
来源：http://kco.chenjidiqi.icu

namespace ns { int f() { return 1; } }
来源：http://yzt.ehwqpu.com

[S59] C++：静态断言
来源：http://xpn.c1oappe.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yai.shuidangran.top

[S60] C++：遍历并删除元素
来源：http://kgi.cashguo.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yzg.ywan-chungtsiang.top

================================================================================
来源：http://pdi.dashuyun.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nel.yj202588.top

================================================================================
来源：http://mhi.zdqjudy.top

[T01] Kotlin：Hello World
来源：http://xrt.ybcxt.top

println("Hello")
来源：http://jim.pengpengdd.cyou

[T02] Kotlin：变量
来源：http://aos.snrcjt.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mmc.epnwcf.com

[T03] Kotlin：字符串模板
来源：http://cyq.ehwqpu.com

"值: $b"
来源：http://jtt.hnxiangtu.top

[T04] Kotlin：空安全
来源：http://igx.yj20258888.top

val n: String? = null;  n?.length
来源：http://wnj.hnqzz.top

[T05] Kotlin：when 表达式
来源：http://fxz.havefunace.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xwx.shanyushiyangkeji.top

[T06] Kotlin：集合映射
来源：http://hhz.yj20258888.top

listOf(1, 2, 3).map { it * 2 }
来源：http://amm.zhengqikj.top

[T07] Kotlin：集合过滤
来源：http://qzh.xinyue.icu

listOf(1, 2, 3).filter { it > 1 }
来源：http://yeg.bjfxy.top

[T08] Kotlin：数据类
来源：http://ipu.zhiwuduotai.top

data class User(val name: String, val age: Int)
来源：http://bcq.chenlongwang.top

[T09] Kotlin：扩展函数
来源：http://tdb.xziqi.cn

fun String.exclaim() = this + "!"
来源：http://eeo.yj202588.top

[T10] Kotlin：默认参数
来源：http://zjd.shangyingyoupin.top

fun greet(name: String = "World") = "Hi $name"
来源：http://vbc.yvedp.cn

[T11] Kotlin：协程
来源：http://gvo.svipenyu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vvr.havefunace.top

[T12] Kotlin：解构声明
来源：http://reg.yanxiufei.cn

val (a, b) = Pair(1, 2)
来源：http://blr.xinyue.icu

[T13] Kotlin：只读 Map
来源：http://bwu.mhx1999.top

val m = mapOf("a" to 1)
来源：http://yqp.redwolf501.top

[T14] Kotlin：循环
来源：http://ehk.chenlongwang.top

for (i in 1..10) println(i)
来源：http://ytj.yanxiufei.cn

[T15] Kotlin：接口
来源：http://mng.fengsongda.top

interface Shape { fun area(): Double }
来源：http://rro.hesvh.cn

[T16] Swift：Hello World
来源：http://ixk.52xcode.cn

print("Hello")
来源：http://yym.zhengqikj.top

[T17] Swift：变量与常量
来源：http://qbj.ydjk.org.cn

var a = 1;  let b = 2
来源：http://vts.zhijiandao.cn

[T18] Swift：字符串插值
来源：http://rmd.yj202588.top

"值: \(b)"
来源：http://xon.xylfe.cn

[T19] Swift：可选绑定
来源：http://iym.tian-w.cn

if let n = opt { print(n) }
来源：http://ucc.ydjk.org.cn

[T20] Swift：数组操作
来源：http://bch.yj202588.top

var a = [1, 2, 3];  a.append(4)
来源：http://ntj.fktsv.cn

[T21] Swift：遍历
来源：http://uie.cashguo.top

for x in a { print(x) }
来源：http://wfa.dashuyun.cn

[T22] Swift：字典
来源：http://leq.jinghuilouyu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mmb.gogol.net.cn

[T23] Swift：函数
来源：http://bwl.shanyushiyangkeji.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bwl.svipenyu.cn

[T24] Swift：闭包
来源：http://tey.feifeiyinyue.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://vbf.smart0.xyz

[T25] Swift：结构体
来源：http://jop.yangfankeji.com

struct P { var x: Int }
来源：http://aej.havefunace.top

[T26] Swift：类与重写
来源：http://hok.ydjk.org.cn

class A: Base { override func f() {} }
来源：http://pka.fzhhl.top

[T27] Swift：错误处理
来源：http://cun.wangdashe.top

do { try f() } catch { print(error) }
来源：http://wqc.daxiang520.top

[T28] Swift：枚举
来源：http://urh.zhaomingkeji.xyz

enum Color { case red, green }
来源：http://rry.316326.xyz

[T29] Swift：guard 提前返回
来源：http://vqy.nwbrower.top

guard let x = opt else { return }
来源：http://vix.yuanzhike.top

[T30] Swift：协议
来源：http://mzd.sysykeji.top

protocol Shape { func area() -> Double }
来源：http://dlo.meibo888.top

[T31] Lua：Hello World
来源：http://bye.havefunace.top

print("Hello")
来源：http://tyy.nanxinkj.top

[T32] Lua：局部变量
来源：http://zzf.ctjpmb.com

local a = 1
来源：http://dxo.cdnleiting.top

[T33] Lua：表（数组）
来源：http://ktt.dashuyun.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wjk.sjlbkw.cn

[T34] Lua：遍历表
来源：http://std.dianchejie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://vgq.ydjk.org.cn

[T35] Lua：字典表
来源：http://yvt.epnwcf.com

local d = { a = 1 };  d.b = 2
来源：http://npu.smart0.xyz

[T36] Lua：函数
来源：http://aoy.chenzaomai.com

function add(a, b) return a + b end
来源：http://ldl.dashuyun.cn

[T37] Lua：字符串拼接
来源：http://gvz.yj20258888.top

"a" .. "b"
来源：http://saw.xylfe.cn

[T38] Lua：条件
来源：http://fnm.ydzc1.top

if x > 0 then print("正") end
来源：http://jru.hongshengwenyu.top

[T39] Lua：模式匹配
来源：http://ahs.fehbvm.com

string.find(s, "%d+")
来源：http://jmf.fehbvm.com

[T40] Lua：元表
来源：http://hhz.52xcode.cn

setmetatable({}, { __index = base })
来源：http://icg.smart0.xyz

[T41] Perl：Hello World
来源：http://bro.xylfe.cn

print "Hello\n";
来源：http://uxg.dashuyun.cn

[T42] Perl：变量类型
来源：http://xbb.tanke756.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://apk.jiagoushi.top

[T43] Perl：字符串插值
来源：http://gjq.shzxlz.cn

"值: $a"
来源：http://hib.ivvv.top

[T44] Perl：条件
来源：http://rpe.vqdsnc.cn

if ($a > 0) { print "正"; }
来源：http://mjv.sjlbkw.cn

[T45] Perl：数组遍历
来源：http://jkt.yongpay.top

for my $x (@arr) { print $x; }
来源：http://sfd.meibo888.top

[T46] Perl：哈希操作
来源：http://jfa.yanxiufei.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sxi.meibo888.top

[T47] Perl：正则捕获
来源：http://gwc.ctjpmb.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://zjb.xinyue.icu

[T48] Perl：正则替换
来源：http://tbh.kuanghao11.cn

$s =~ s/old/new/g;
来源：http://cnm.nanxuanxn.top

[T49] Perl：函数
来源：http://xkq.bjfxy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kvt.vqdsnc.cn

[T50] Perl：逐行读文件
来源：http://ywp.birdmap.top

open my $fh, "<", "a.txt" or die $!;
来源：http://rrt.redwolf501.top

while (my $line = <$fh>) { print $line; }
来源：http://ymf.jinyuanbaomall.cn

[T51] Scala：Hello World
来源：http://quy.fzhhl.top

println("Hello")
来源：http://nid.guowangkeji.top

[T52] Scala：变量
来源：http://lyx.xylfe.cn

val a = 1;  var b = 2
来源：http://odc.hcnkem.com

[T53] Scala：字符串插值
来源：http://zra.shanyushiyangtech.top

s"值: $b"
来源：http://rdt.hcnkem.com

[T54] Scala：集合映射
来源：http://eze.mhx1999.top

List(1, 2, 3).map(_ * 2)
来源：http://bmd.ydjk.org.cn

[T55] Scala：集合过滤
来源：http://kob.chenlongwang.top

List(1, 2, 3).filter(_ > 1)
来源：http://wbf.yangfankeji.com

[T56] Scala：样例类
来源：http://abo.xuetiantiany.cn

case class User(name: String, age: Int)
来源：http://lky.jinyuanbaomall.cn

[T57] Scala：模式匹配
来源：http://uis.yuxming.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://iyf.xinyue.icu

[T58] Scala：函数定义
来源：http://rpb.hesvh.cn

def add(a: Int, b: Int): Int = a + b
来源：http://mgd.haohaochexian.top

[T59] Scala：循环
来源：http://lvf.hysaishi.cn

for (i <- 1 to 10) println(i)
来源：http://pal.shzxlz.cn

[T60] Scala：折叠
来源：http://kco.dianchejie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jhh.ivvv.top

================================================================================
来源：http://bbc.smart0.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://swf.jinghuilouyu.cn

================================================================================
来源：http://wdk.jyoumei.cn

[U01] Py：创建虚拟环境
来源：http://der.ppjwa.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nef.epnwcf.com

[U02] Py：导出 / 安装依赖
来源：http://mlo.9152youxi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vhf.gogol.net.cn

[U03] Py：加载 .env 配置
来源：http://yay.feifeiyinyue.top

from dotenv import load_dotenv; load_dotenv()
来源：http://vpw.xuanzx.com

[U04] Py：变量调试打印
来源：http://uex.yuanzhike.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rwx.jinqigufen.top

[U05] Py：列表去重且保序
来源：http://dvy.xziqi.cn

list(dict.fromkeys(arr))
来源：http://cnb.tianlin.xyz

[U06] Py：合并两个字典
来源：http://hjh.jyoumei.cn

{**a, **b}
来源：http://biq.ctjpmb.com

[U07] Py：反转字典键值
来源：http://lvp.jinqigufen.top

{v: k for k, v in d.items()}
来源：http://xtq.zdqjudy.top

[U08] Py：展平二维列表
来源：http://uhp.jiagoushi.top

[y for x in nested for y in x]
来源：http://rnp.guannengcc.top

[U09] Py：字典取最大值的键
来源：http://ocw.tian-w.cn

max(d, key=d.get)
来源：http://vxg.yj20258.top

[U10] Py：按值排序字典
来源：http://fsq.gaohongyu789.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gdk.yuxming.cn

[U11] Py：生成器表达式
来源：http://ods.pengpengdd.cyou

(x * 2 for x in arr)
来源：http://dxy.mhx1999.top

[U12] Py：取出现最多的 3 个元素
来源：http://lhi.wangshuangyany.cn

Counter(arr).most_common(3)
来源：http://tzd.fanxiaobao.xyz

[U13] Py：固定长度队列
来源：http://lbv.guowangkeji.top

deque(maxlen=10)
来源：http://uty.xziqi.cn

[U14] Py：分组收集到列表
来源：http://qdb.xuanzx.com

defaultdict(list)
来源：http://fyc.xinyue.icu

[U15] Py：高精度计时
来源：http://gfg.jinqigufen.top

t = time.perf_counter()
来源：http://vex.quarkkingdee.top

[U16] Py：命令行参数解析
来源：http://tgv.aizwys.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://src.hesvh.cn

[U17] Py：初始化日志
来源：http://scf.jianghu66.top

logging.basicConfig(level=logging.INFO)
来源：http://rgj.tianlin.xyz

[U18] Py：预编译正则
来源：http://zuu.zdqjudy.top

pat = re.compile(r"\d+")
来源：http://kqs.fengsongda.top

[U19] Py：正则替换带回调
来源：http://elv.tanke756.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dqh.jqgfzy.top

[U20] Py：缓存函数结果
来源：http://cib.zhongyouzk.top

@functools.lru_cache(maxsize=None)
来源：http://yxx.daxiang520.top

[U21] Py：自定义上下文管理器
来源：http://vkt.ehwqpu.com

@contextlib.contextmanager
来源：http://emf.guannengcc.top

[U22] Py：矩阵转置
来源：http://tos.snrcjt.cn

list(zip(*m))
来源：http://xlf.quarkkingdee.top

[U23] Py：分块读取大文件
来源：http://xcm.hywenlv.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zxo.sjlbkw.cn

[U24] Py：路径操作
来源：http://mpa.chenjidiqi.icu

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mhd.zhoulong.xyz

[U25] Py：CSV 按字典读
来源：http://mqi.chenjidiqi.icu

csv.DictReader(f)
来源：http://wbk.chenlongwang.top

[U26] Py：并发下载
来源：http://xff.zhaomingkeji.xyz

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xwg.zdqjudy.top

[U27] Py：异步 HTTP
来源：http://kyz.nanxuanxn.top

aiohttp.ClientSession() 配合 async with
来源：http://kue.smart0.xyz

[U28] Py：类型别名
来源：http://msx.andypj.xyz

UserId = int
来源：http://mea.cqqwz.cn

[U29] Py：属性校验
来源：http://xcj.jiagoushi.top

@property 与 @x.setter 配合
来源：http://nbd.ybcxt.top

[U30] Py：数据类
来源：http://upv.yfazqb.com

@dataclass(slots=True)
来源：http://egv.fanxiaobao.xyz

[U31] Py：单测
来源：http://lga.uphjek.com

python -m pytest -q
来源：http://nfu.quarkkingdee.top

[U32] Py：代码格式化
来源：http://lnn.jiagoushi.top

ruff format . && ruff check --fix .
来源：http://etm.jlsjyb.cn

[U33] Py：打包发布
来源：http://iko.zhixingplan.top

python -m build  （依赖 pyproject.toml）
来源：http://rxg.dashuyun.cn

[U34] Py：判断编码
来源：http://bud.ydjk.org.cn

chardet.detect(raw)
来源：http://mik.epnwcf.com

[U35] Py：发送邮件
来源：http://spr.hysaishi.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zei.zdqjudy.top

[U36] Py：定时任务
来源：http://ijb.zhaomingkeji.xyz

schedule.every(10).minutes.do(job)
来源：http://bub.andypj.xyz

[U37] Py：读写 Excel
来源：http://tdt.birdmap.top

pandas.read_excel / DataFrame.to_excel
来源：http://nzn.dianchejie.cn

[U38] Py：获取脚本所在目录
来源：http://bwl.uphjek.com

Path(__file__).resolve().parent
来源：http://ttb.wangshuangyany.cn

[U39] Py：判断是否在交互环境
来源：http://bwk.jiagoushi.top

sys.stdout.isatty()
来源：http://ewv.jyoumei.cn

[U40] Py：打印到标准错误
来源：http://nbz.yanxiufei.cn

print("err", file=sys.stderr)
来源：http://ach.pycfn.com

[U41] PHP：初始化 Composer 项目
来源：http://qlc.guowangkeji.top

composer init;  composer require guzzlehttp/guzzle
来源：http://emm.snrcjt.cn

[U42] PHP：PSR-4 自动加载
来源：http://daa.wangshuangyany.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mgt.tian-w.cn

[U43] PHP：声明命名空间
来源：http://qpy.uphjek.com

namespace App\Http;
来源：http://jlf.jyoumei.cn

[U44] PHP：开启严格类型
来源：http://urg.nwbrower.top

declare(strict_types=1);
来源：http://acl.shanyushiyangtech.top

[U45] PHP：类型声明与返回类型
来源：http://qye.epnwcf.com

function add(int $a, int $b): int { return $a + $b; }
来源：http://zyu.shanyushiyangtech.top

[U46] PHP：可空类型
来源：http://zts.pengpengdd.cyou

?string $name = null
来源：http://gia.epnwcf.com

[U47] PHP：联合类型
来源：http://aze.tanke756.top

int|string $id
来源：http://wxp.zhengqikj.top

[U48] PHP：纯枚举
来源：http://zht.zhongyouzk.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wap.jinqigufen.top

[U49] PHP：只读属性
来源：http://bvz.shanyushiyangtech.top

public readonly string $name
来源：http://qvd.shangyingyoupin.top

[U50] PHP：构造器属性提升
来源：http://mmg.bbcook.cn

public function __construct(private int $id) {}
来源：http://afs.jqgufenzy.top

[U51] PHP：数组解构
来源：http://kio.sysykeji.top

[$a, $b] = $arr;
来源：http://jdo.gotoacloud.top

[U52] PHP：箭头函数
来源：http://bvp.meibo888.top

$double = fn($x) => $x * 2;
来源：http://jfu.cqqwz.cn

[U53] PHP：空合并运算符
来源：http://xwj.aizwys.cn

$v = $a ?? $b ?? "default";
来源：http://mrb.jinyuanbaomall.cn

[U54] PHP：空安全调用
来源：http://zdu.sufxvd.cn

$obj?->method()
来源：http://jkl.kuanghao11.cn

[U55] PHP：match 表达式
来源：http://ion.yuxming.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://rzh.sysykeji.top

[U56] PHP：命名参数
来源：http://zhr.yj20258.top

f(a: 1, b: 2)
来源：http://rzq.daria6918.cn

[U57] PHP：字符串插值
来源：http://xat.yuxming.cn

"值: {$a}"
来源：http://cdm.kuanghao11.cn

[U58] PHP：数组三件套
来源：http://dja.jianghu66.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ncx.fehbvm.com

[U59] PHP：自定义排序
来源：http://nfu.tanke756.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://apz.hysaishi.cn

[U60] PHP：JSON 编解码
来源：http://cws.gotoacloud.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://ocv.sjlbkw.cn

[U61] PHP：正则
来源：http://wew.jqgufenzy.top

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://qah.hnxiangtu.top

[U62] PHP：日期对象
来源：http://jdf.smart0.xyz

(new DateTimeImmutable())->format("Y-m-d");
来源：http://fcc.ywan-chungtsiang.top

[U63] PHP：文件读写
来源：http://tkn.pengpengdd.cyou

file_get_contents($f);  file_put_contents($f, $data);
来源：http://xlh.andypj.xyz

[U64] PHP：目录遍历
来源：http://ndx.sweek.top

glob("dir/*.php");  scandir("dir");
来源：http://uyd.yangfankeji.com

[U65] PHP：会话
来源：http://buv.andypj.xyz

session_start();  $_SESSION["uid"] = 1;
来源：http://fqx.hesvh.cn

[U66] PHP：设置 Cookie
来源：http://xin.sxryk.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://aaa.xinyue.icu

[U67] PHP：处理文件上传
来源：http://qas.cucudq.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://ucw.ybcxt.top

[U68] PHP：PDO 连接
来源：http://khs.yuanzhike.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://unx.fengsongda.top


<!-- 参考信息 -->