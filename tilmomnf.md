代发 wailian999

[S43] C++：智能指针
来源：http://nyy.uphjek.com

auto p = std::make_unique<int>(5);
来源：http://ams.zycfv.cn

[S44] C++：引用传参
来源：http://vuw.fanxiaobao.xyz

void inc(int &x) { ++x; }
来源：http://wvp.shangyingyoupin.top

[S45] C++：lambda
来源：http://uug.ctjpmb.com

auto add = [](int a, int b) { return a + b; };
来源：http://dtf.gogol.net.cn

[S46] C++：函数模板
来源：http://zah.jinqigufen.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tcf.gotoacloud.top

[S47] C++：结构化绑定遍历
来源：http://mvu.wangdashe.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sqh.zhongyouzk.top

[S48] C++：逐行读文件
来源：http://klm.haohaochexian.top

std::ifstream in("a.txt");  std::string line;
来源：http://vhj.bjfxy.top

while (std::getline(in, line)) { }
来源：http://tps.guowangkeji.top

[S49] C++：写文件
来源：http://jed.smart0.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://iab.xuanzx.com

[S50] C++：格式化数字
来源：http://jmx.hammf.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wkl.yangfankeji.com

[S51] C++：显式类型转换
来源：http://dry.ybcxt.top

static_cast<double>(a) / b
来源：http://glc.nwbrower.top

[S52] C++：const 与 noexcept
来源：http://zky.shanyushiyangtech.top

int size() const noexcept { return n_; }
来源：http://iwq.jiagoushi.top

[S53] C++：移动语义
来源：http://egf.xylfe.cn

std::vector<int> w = std::move(v);
来源：http://onw.gotoacloud.top

[S54] C++：异常处理
来源：http://hma.ywan-chungtsiang.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://exv.ivvv.top

[S55] C++：结构化绑定
来源：http://kgt.nanxuanxn.top

auto [a, b] = std::make_pair(1, 2);
来源：http://tfa.xuanzx.com

[S56] C++：optional
来源：http://jsv.jqgfzy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pgu.yuanzhike.top

[S57] C++：编译期常量
来源：http://vtn.xylfe.cn

constexpr int N = 10;
来源：http://goj.hfpthk.cn

[S58] C++：命名空间
来源：http://ryh.zhijiandao.cn

namespace ns { int f() { return 1; } }
来源：http://rmk.jyoumei.cn

[S59] C++：静态断言
来源：http://knb.xinyue.icu

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://meq.fengsongda.top

[S60] C++：遍历并删除元素
来源：http://wko.sufxvd.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dzz.yueranfly.top

================================================================================
来源：http://mlp.dashuyun.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zej.jinqigufen.top

================================================================================
来源：http://aba.yongpay.top

[T01] Kotlin：Hello World
来源：http://ahu.ydzc1.top

println("Hello")
来源：http://pko.daria6918.cn

[T02] Kotlin：变量
来源：http://aou.epnwcf.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rks.zycfv.cn

[T03] Kotlin：字符串模板
来源：http://pnx.316326.xyz

"值: $b"
来源：http://wcx.dashuyun.cn

[T04] Kotlin：空安全
来源：http://hta.9152youxi.cn

val n: String? = null;  n?.length
来源：http://hxw.cqqwz.cn

[T05] Kotlin：when 表达式
来源：http://hqf.gzhubu.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://don.ppjwa.cn

[T06] Kotlin：集合映射
来源：http://aaz.yj202588.top

listOf(1, 2, 3).map { it * 2 }
来源：http://eeq.ivvv.top

[T07] Kotlin：集合过滤
来源：http://udb.shzxlz.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ife.gzhubu.top

[T08] Kotlin：数据类
来源：http://cfm.vehdjk.com

data class User(val name: String, val age: Int)
来源：http://jyj.daxiang520.top

[T09] Kotlin：扩展函数
来源：http://aym.c1oappe.top

fun String.exclaim() = this + "!"
来源：http://thh.ywan-chungtsiang.top

[T10] Kotlin：默认参数
来源：http://ggj.sweek.top

fun greet(name: String = "World") = "Hi $name"
来源：http://nvh.xuanzx.com

[T11] Kotlin：协程
来源：http://tam.haohaochexian.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://zxx.bbcook.cn

[T12] Kotlin：解构声明
来源：http://lkk.zhoulong.xyz

val (a, b) = Pair(1, 2)
来源：http://yiz.tian-w.cn

[T13] Kotlin：只读 Map
来源：http://tze.316326.xyz

val m = mapOf("a" to 1)
来源：http://lsw.xziqi.cn

[T14] Kotlin：循环
来源：http://yaw.ivvv.top

for (i in 1..10) println(i)
来源：http://bls.zhongyouzk.top

[T15] Kotlin：接口
来源：http://agh.nanxuanxn.top

interface Shape { fun area(): Double }
来源：http://utn.hnxiangtu.top

[T16] Swift：Hello World
来源：http://erb.zdqjudy.top

print("Hello")
来源：http://rlg.yueranfly.top

[T17] Swift：变量与常量
来源：http://cvc.jinqigufen.top

var a = 1;  let b = 2
来源：http://vfy.jyoumei.cn

[T18] Swift：字符串插值
来源：http://qqx.xinyue.icu

"值: \(b)"
来源：http://uvd.ydjk.org.cn

[T19] Swift：可选绑定
来源：http://epo.hfpthk.cn

if let n = opt { print(n) }
来源：http://ztb.ywan-chungtsiang.top

[T20] Swift：数组操作
来源：http://otd.shuidangran.top

var a = [1, 2, 3];  a.append(4)
来源：http://czy.daxiang520.top

[T21] Swift：遍历
来源：http://hok.sweek.top

for x in a { print(x) }
来源：http://rht.gogol.net.cn

[T22] Swift：字典
来源：http://yrb.yonumen.top

var d = ["a": 1];  d["b"] = 2
来源：http://sjz.snrcjt.cn

[T23] Swift：函数
来源：http://rmp.yangfankeji.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gdw.yueranfly.top

[T24] Swift：闭包
来源：http://uhs.cheryme.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://vgw.fzhhl.top

[T25] Swift：结构体
来源：http://odg.jinghuilouyu.cn

struct P { var x: Int }
来源：http://bwr.yfazqb.com

[T26] Swift：类与重写
来源：http://wfc.zhaomingkeji.xyz

class A: Base { override func f() {} }
来源：http://ive.yj20258.top

[T27] Swift：错误处理
来源：http://dhh.chenjidiqi.icu

do { try f() } catch { print(error) }
来源：http://lzh.xuetiantiany.cn

[T28] Swift：枚举
来源：http://kvp.ydjk.org.cn

enum Color { case red, green }
来源：http://vnh.chenlongwang.top

[T29] Swift：guard 提前返回
来源：http://usu.dianchejie.cn

guard let x = opt else { return }
来源：http://eda.vehdjk.com

[T30] Swift：协议
来源：http://qzq.zhongyouzk.top

protocol Shape { func area() -> Double }
来源：http://yyz.shzxlz.cn

[T31] Lua：Hello World
来源：http://kqc.uphjek.com

print("Hello")
来源：http://xoi.jyoumei.cn

[T32] Lua：局部变量
来源：http://rvy.yangfankeji.com

local a = 1
来源：http://lio.mhx1999.top

[T33] Lua：表（数组）
来源：http://cbu.ydzc1.top

local t = {1, 2, 3};  t[4] = 4
来源：http://fbz.jiagoushi.top

[T34] Lua：遍历表
来源：http://zct.shanyushiyangkeji.top

for i, v in ipairs(t) do print(i, v) end
来源：http://cic.zhijiandao.cn

[T35] Lua：字典表
来源：http://zek.ybcxt.top

local d = { a = 1 };  d.b = 2
来源：http://poq.guannengcc.top

[T36] Lua：函数
来源：http://oiq.tian-w.cn

function add(a, b) return a + b end
来源：http://dkl.yfazqb.com

[T37] Lua：字符串拼接
来源：http://avt.yuxming.cn

"a" .. "b"
来源：http://khc.redwolf501.top

[T38] Lua：条件
来源：http://nco.xuanzx.com

if x > 0 then print("正") end
来源：http://vig.gogol.net.cn

[T39] Lua：模式匹配
来源：http://pvi.cashguo.top

string.find(s, "%d+")
来源：http://sfw.hywenlv.cn

[T40] Lua：元表
来源：http://elw.feifeiyinyue.top

setmetatable({}, { __index = base })
来源：http://cal.shanyushiyangtech.top

[T41] Perl：Hello World
来源：http://oqr.hesvh.cn

print "Hello\n";
来源：http://pct.gzhubu.top

[T42] Perl：变量类型
来源：http://khz.zhongyouzk.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tuv.zhixingplan.top

[T43] Perl：字符串插值
来源：http://wfr.nanxuanxn.top

"值: $a"
来源：http://add.jinyuanbaomall.cn

[T44] Perl：条件
来源：http://tus.0kj1m.cn

if ($a > 0) { print "正"; }
来源：http://yuh.zhaomingkeji.xyz

[T45] Perl：数组遍历
来源：http://gpv.yonumen.top

for my $x (@arr) { print $x; }
来源：http://npf.fanxiaobao.xyz

[T46] Perl：哈希操作
来源：http://jhm.pengpengdd.cyou

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://uhf.zhengqikj.top

[T47] Perl：正则捕获
来源：http://pov.gaohongyu789.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://axx.guannengcc.top

[T48] Perl：正则替换
来源：http://fcj.tarul.cn

$s =~ s/old/new/g;
来源：http://iiy.epnwcf.com

[T49] Perl：函数
来源：http://dyo.hammf.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gii.yuxming.cn

[T50] Perl：逐行读文件
来源：http://nkj.chenlongwang.top

open my $fh, "<", "a.txt" or die $!;
来源：http://qib.guowangkeji.top

while (my $line = <$fh>) { print $line; }
来源：http://grj.havefunace.top

[T51] Scala：Hello World
来源：http://rir.xuetiantiany.cn

println("Hello")
来源：http://mfi.ywan-chungtsiang.top

[T52] Scala：变量
来源：http://trn.smart0.xyz

val a = 1;  var b = 2
来源：http://wjs.xuetiantiany.cn

[T53] Scala：字符串插值
来源：http://tjq.gaohongyu789.top

s"值: $b"
来源：http://jin.bbcook.cn

[T54] Scala：集合映射
来源：http://ead.yonumen.top

List(1, 2, 3).map(_ * 2)
来源：http://rhm.yuanzhike.top

[T55] Scala：集合过滤
来源：http://tbq.hfpthk.cn

List(1, 2, 3).filter(_ > 1)
来源：http://zdu.hongshengwenyu.top

[T56] Scala：样例类
来源：http://mfn.yuxming.cn

case class User(name: String, age: Int)
来源：http://kbb.yuanzhike.top

[T57] Scala：模式匹配
来源：http://xtj.andypj.xyz

x match { case 1 => "一"; case _ => "其他" }
来源：http://xve.gotoacloud.top

[T58] Scala：函数定义
来源：http://lii.chenjidiqi.icu

def add(a: Int, b: Int): Int = a + b
来源：http://sof.dianchejie.cn

[T59] Scala：循环
来源：http://bxv.gzhubu.top

for (i <- 1 to 10) println(i)
来源：http://zwo.fzhhl.top

[T60] Scala：折叠
来源：http://ifr.jinghuilouyu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jgt.yonumen.top

================================================================================
来源：http://clc.cashguo.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cjw.yuanzhike.top

================================================================================
来源：http://cum.wangdashe.top

[U01] Py：创建虚拟环境
来源：http://drc.zdbjq.cn

python -m venv .venv && source .venv/bin/activate
来源：http://vbh.jlsjyb.cn

[U02] Py：导出 / 安装依赖
来源：http://pkr.aibaodan.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://uhe.zhoulong.xyz

[U03] Py：加载 .env 配置
来源：http://upr.chenjidiqi.icu

from dotenv import load_dotenv; load_dotenv()
来源：http://tkf.fanxiaobao.xyz

[U04] Py：变量调试打印
来源：http://zod.feifeiyinyue.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://yai.wangshuangyany.cn

[U05] Py：列表去重且保序
来源：http://tcl.c1oappe.top

list(dict.fromkeys(arr))
来源：http://mlr.cdnleiting.top

[U06] Py：合并两个字典
来源：http://nqk.zdbjq.cn

{**a, **b}
来源：http://njg.vqdsnc.cn

[U07] Py：反转字典键值
来源：http://vfm.jinqigufen.top

{v: k for k, v in d.items()}
来源：http://zgg.jqgufenzy.top

[U08] Py：展平二维列表
来源：http://yru.gzhubu.top

[y for x in nested for y in x]
来源：http://lzh.guowangkeji.top

[U09] Py：字典取最大值的键
来源：http://ccp.svipenyu.cn

max(d, key=d.get)
来源：http://otw.aibaodan.cn

[U10] Py：按值排序字典
来源：http://lvl.fanxiaobao.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fyv.snrcjt.cn

[U11] Py：生成器表达式
来源：http://hjd.zdbjq.cn

(x * 2 for x in arr)
来源：http://ayd.fengsongda.top

[U12] Py：取出现最多的 3 个元素
来源：http://eup.hcnkem.com

Counter(arr).most_common(3)
来源：http://mqh.ehwqpu.com

[U13] Py：固定长度队列
来源：http://lqb.tian-w.cn

deque(maxlen=10)
来源：http://ycc.vqdsnc.cn

[U14] Py：分组收集到列表
来源：http://bpr.tarul.cn

defaultdict(list)
来源：http://mru.andypj.xyz

[U15] Py：高精度计时
来源：http://twh.quarkkingdee.top

t = time.perf_counter()
来源：http://ihi.jinyuanbaomall.cn

[U16] Py：命令行参数解析
来源：http://glg.c1oappe.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://baw.ctjpmb.com

[U17] Py：初始化日志
来源：http://czm.jianghu66.top

logging.basicConfig(level=logging.INFO)
来源：http://wyv.zhengqikj.top

[U18] Py：预编译正则
来源：http://bll.snrcjt.cn

pat = re.compile(r"\d+")
来源：http://wrw.epnwcf.com

[U19] Py：正则替换带回调
来源：http://pag.chenzaomai.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rdm.sufxvd.cn

[U20] Py：缓存函数结果
来源：http://ohr.ehwqpu.com

@functools.lru_cache(maxsize=None)
来源：http://byu.ybcxt.top

[U21] Py：自定义上下文管理器
来源：http://fda.316326.xyz

@contextlib.contextmanager
来源：http://emf.xingfuxueyuan.xyz

[U22] Py：矩阵转置
来源：http://gyr.birdmap.top

list(zip(*m))
来源：http://lip.yj20258.top

[U23] Py：分块读取大文件
来源：http://zjr.aibaodan.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jrs.bjfxy.top

[U24] Py：路径操作
来源：http://ddr.xingfuxueyuan.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://reb.tian-w.cn

[U25] Py：CSV 按字典读
来源：http://key.aibaodan.cn

csv.DictReader(f)
来源：http://rmu.yongpay.top

[U26] Py：并发下载
来源：http://frr.xylfe.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tsv.gzhubu.top

[U27] Py：异步 HTTP
来源：http://naa.dashuyun.cn

aiohttp.ClientSession() 配合 async with
来源：http://bzn.jyoumei.cn

[U28] Py：类型别名
来源：http://ecf.xuetiantiany.cn

UserId = int
来源：http://naa.9152youxi.cn

[U29] Py：属性校验
来源：http://lgn.yuxming.cn

@property 与 @x.setter 配合
来源：http://eyt.jinqigfzy.top

[U30] Py：数据类
来源：http://xot.chenlongwang.top

@dataclass(slots=True)
来源：http://jjk.316326.xyz

[U31] Py：单测
来源：http://jde.mhx1999.top

python -m pytest -q
来源：http://zwb.aibaodan.cn

[U32] Py：代码格式化
来源：http://nxq.aizwys.cn

ruff format . && ruff check --fix .
来源：http://wsx.snrcjt.cn

[U33] Py：打包发布
来源：http://vcp.yfazqb.com

python -m build  （依赖 pyproject.toml）
来源：http://jqn.pycfn.com

[U34] Py：判断编码
来源：http://mrz.daria6918.cn

chardet.detect(raw)
来源：http://mxz.jinqigfzy.top

[U35] Py：发送邮件
来源：http://mwx.hcnkem.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nrz.zhoulong.xyz

[U36] Py：定时任务
来源：http://lbz.zhiwuduotai.top

schedule.every(10).minutes.do(job)
来源：http://gty.mhx1999.top

[U37] Py：读写 Excel
来源：http://ena.cheryme.top

pandas.read_excel / DataFrame.to_excel
来源：http://bbh.kuanghao11.cn

[U38] Py：获取脚本所在目录
来源：http://ddg.gotoacloud.top

Path(__file__).resolve().parent
来源：http://sgy.havefunace.top

[U39] Py：判断是否在交互环境
来源：http://hwj.yj202588.top

sys.stdout.isatty()
来源：http://ctd.tianlin.xyz

[U40] Py：打印到标准错误
来源：http://wza.hnqzz.top

print("err", file=sys.stderr)
来源：http://vaz.nanxinkj.top

[U41] PHP：初始化 Composer 项目
来源：http://okb.sjlbkw.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qxj.cheryme.top

[U42] PHP：PSR-4 自动加载
来源：http://dnw.epnwcf.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gkd.xuanzx.com

[U43] PHP：声明命名空间
来源：http://wbf.kuanghao11.cn

namespace App\Http;
来源：http://ikn.fanxiaobao.xyz

[U44] PHP：开启严格类型
来源：http://ylf.zhaomingkeji.xyz

declare(strict_types=1);
来源：http://uyp.jianghu66.top

[U45] PHP：类型声明与返回类型
来源：http://rdi.gzhubu.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ksq.gaohongyu789.top

[U46] PHP：可空类型
来源：http://jhf.yvedp.cn

?string $name = null
来源：http://qva.iojbl.cn

[U47] PHP：联合类型
来源：http://xxh.yj202588.top

int|string $id
来源：http://ryt.kuanghao11.cn

[U48] PHP：纯枚举
来源：http://pfg.xinyue.icu

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hyj.bbcook.cn

[U49] PHP：只读属性
来源：http://gyu.gotoacloud.top

public readonly string $name
来源：http://qxm.hfpthk.cn

[U50] PHP：构造器属性提升
来源：http://bgn.smart0.xyz

public function __construct(private int $id) {}
来源：http://peu.jinyuanbaomall.cn

[U51] PHP：数组解构
来源：http://jqs.yongpay.top

[$a, $b] = $arr;
来源：http://nuv.guannengcc.top

[U52] PHP：箭头函数
来源：http://cqu.yj202588.top

$double = fn($x) => $x * 2;
来源：http://omt.sjlbkw.cn

[U53] PHP：空合并运算符
来源：http://cai.cqqwz.cn

$v = $a ?? $b ?? "default";
来源：http://vhn.fengsongda.top

[U54] PHP：空安全调用
来源：http://yqx.yvedp.cn

$obj?->method()
来源：http://hpk.cdnleiting.top

[U55] PHP：match 表达式
来源：http://iwu.yuxming.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://gey.hnxiangtu.top

[U56] PHP：命名参数
来源：http://uxb.cdnleiting.top

f(a: 1, b: 2)
来源：http://qcc.yonumen.top

[U57] PHP：字符串插值
来源：http://jov.pycfn.com

"值: {$a}"
来源：http://bhg.tanke756.top

[U58] PHP：数组三件套
来源：http://umn.birdmap.top

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://yrh.aibaodan.cn

[U59] PHP：自定义排序
来源：http://uik.xinyue.icu

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vma.wangdashe.top

[U60] PHP：JSON 编解码
来源：http://pte.redwolf501.top

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://svt.sweek.top

[U61] PHP：正则
来源：http://dpv.wangshuangyany.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://lzz.hesvh.cn

[U62] PHP：日期对象
来源：http://njn.vehdjk.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wqk.jqgfzy.top

[U63] PHP：文件读写
来源：http://acd.iojbl.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://sox.hysaishi.cn

[U64] PHP：目录遍历
来源：http://jry.fanxiaobao.xyz

glob("dir/*.php");  scandir("dir");
来源：http://uvu.hcnkem.com

[U65] PHP：会话
来源：http://qeu.jinghuilouyu.cn

session_start();  $_SESSION["uid"] = 1;
来源：http://huq.ctjpmb.com

[U66] PHP：设置 Cookie
来源：http://zaw.ydjk.org.cn

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://chd.jiagoushi.top

[U67] PHP：处理文件上传
来源：http://thu.tian-w.cn

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://phl.hammf.cn

[U68] PHP：PDO 连接
来源：http://dlq.gaohongyu789.top

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://nwn.gotoacloud.top


<!-- 参考信息 -->