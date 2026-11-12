代发 wailian999

[S43] C++：智能指针
来源：http://rvp.9152youxi.cn

auto p = std::make_unique<int>(5);
来源：http://lmx.mhx1999.top

[S44] C++：引用传参
来源：http://qcg.tian-w.cn

void inc(int &x) { ++x; }
来源：http://kae.c1oappe.top

[S45] C++：lambda
来源：http://obm.pengpengdd.cyou

auto add = [](int a, int b) { return a + b; };
来源：http://mly.yonumen.top

[S46] C++：函数模板
来源：http://roz.jyoumei.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rqi.chenlongwang.top

[S47] C++：结构化绑定遍历
来源：http://ogh.yj20258888.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nhf.ctjpmb.com

[S48] C++：逐行读文件
来源：http://zgd.birdmap.top

std::ifstream in("a.txt");  std::string line;
来源：http://qgu.zhongyouzk.top

while (std::getline(in, line)) { }
来源：http://cwy.hesvh.cn

[S49] C++：写文件
来源：http://tzl.yuanzhike.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pjs.shanyushiyangtech.top

[S50] C++：格式化数字
来源：http://uho.pycfn.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ido.yangfankeji.com

[S51] C++：显式类型转换
来源：http://tvq.yj20258888.top

static_cast<double>(a) / b
来源：http://qhd.jyoumei.cn

[S52] C++：const 与 noexcept
来源：http://nai.cheryme.top

int size() const noexcept { return n_; }
来源：http://ihd.tianlin.xyz

[S53] C++：移动语义
来源：http://yyn.daxiang520.top

std::vector<int> w = std::move(v);
来源：http://dzr.andypj.xyz

[S54] C++：异常处理
来源：http://tah.jianghu66.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ven.yanxiufei.cn

[S55] C++：结构化绑定
来源：http://rjz.daxiang520.top

auto [a, b] = std::make_pair(1, 2);
来源：http://lsb.9152youxi.cn

[S56] C++：optional
来源：http://arp.haohaochexian.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pxo.zhixingplan.top

[S57] C++：编译期常量
来源：http://vly.zdbjq.cn

constexpr int N = 10;
来源：http://ucr.gzhubu.top

[S58] C++：命名空间
来源：http://zuf.daxiang520.top

namespace ns { int f() { return 1; } }
来源：http://rsm.bjfxy.top

[S59] C++：静态断言
来源：http://hth.c1oappe.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tns.mhx1999.top

[S60] C++：遍历并删除元素
来源：http://mwj.hnqzz.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jzk.shzxlz.cn

================================================================================
来源：http://kne.daria6918.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://izd.xinyue.icu

================================================================================
来源：http://ugw.jinqigfzy.top

[T01] Kotlin：Hello World
来源：http://qku.chenjidiqi.icu

println("Hello")
来源：http://ynr.chenzaomai.com

[T02] Kotlin：变量
来源：http://inx.gzhubu.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://loj.chenzaomai.com

[T03] Kotlin：字符串模板
来源：http://eeq.gaohongyu789.top

"值: $b"
来源：http://pip.cqqwz.cn

[T04] Kotlin：空安全
来源：http://bkx.jiagoushi.top

val n: String? = null;  n?.length
来源：http://one.shanyushiyangkeji.top

[T05] Kotlin：when 表达式
来源：http://dnp.52xcode.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hnv.cqqwz.cn

[T06] Kotlin：集合映射
来源：http://bxl.feifeiyinyue.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ajr.snrcjt.cn

[T07] Kotlin：集合过滤
来源：http://ksd.hcnkem.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://jzn.mhx1999.top

[T08] Kotlin：数据类
来源：http://kkv.tianlin.xyz

data class User(val name: String, val age: Int)
来源：http://hbz.hnxiangtu.top

[T09] Kotlin：扩展函数
来源：http://cnf.nanxinkj.top

fun String.exclaim() = this + "!"
来源：http://edh.hnqzz.top

[T10] Kotlin：默认参数
来源：http://xyf.daria6918.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ijc.0kj1m.cn

[T11] Kotlin：协程
来源：http://igc.316326.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://bee.hammf.cn

[T12] Kotlin：解构声明
来源：http://zom.jqgfzy.top

val (a, b) = Pair(1, 2)
来源：http://cvt.aibaodan.cn

[T13] Kotlin：只读 Map
来源：http://ygl.bbcook.cn

val m = mapOf("a" to 1)
来源：http://syn.chenzaomai.com

[T14] Kotlin：循环
来源：http://omd.birdmap.top

for (i in 1..10) println(i)
来源：http://esq.yonumen.top

[T15] Kotlin：接口
来源：http://yvs.ydzc1.top

interface Shape { fun area(): Double }
来源：http://jon.jyoumei.cn

[T16] Swift：Hello World
来源：http://elq.ydjk.org.cn

print("Hello")
来源：http://vwo.kuanghao11.cn

[T17] Swift：变量与常量
来源：http://hyw.hammf.cn

var a = 1;  let b = 2
来源：http://mnl.hcnkem.com

[T18] Swift：字符串插值
来源：http://fui.guannengcc.top

"值: \(b)"
来源：http://cwc.pycfn.com

[T19] Swift：可选绑定
来源：http://ujx.fehbvm.com

if let n = opt { print(n) }
来源：http://sqb.chenzaomai.com

[T20] Swift：数组操作
来源：http://zrg.gotoacloud.top

var a = [1, 2, 3];  a.append(4)
来源：http://xaf.cheryme.top

[T21] Swift：遍历
来源：http://ium.fehbvm.com

for x in a { print(x) }
来源：http://hpl.bjfxy.top

[T22] Swift：字典
来源：http://evb.snrcjt.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zsn.wangdashe.top

[T23] Swift：函数
来源：http://sob.zhijiandao.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pxp.zhengqikj.top

[T24] Swift：闭包
来源：http://ckr.gzhubu.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://qof.ehwqpu.com

[T25] Swift：结构体
来源：http://okz.ctjpmb.com

struct P { var x: Int }
来源：http://ewo.sjlbkw.cn

[T26] Swift：类与重写
来源：http://wyq.xuetiantiany.cn

class A: Base { override func f() {} }
来源：http://ske.sxryk.cn

[T27] Swift：错误处理
来源：http://dfw.nanxinkj.top

do { try f() } catch { print(error) }
来源：http://nwn.daria6918.cn

[T28] Swift：枚举
来源：http://crj.xingfuxueyuan.xyz

enum Color { case red, green }
来源：http://jrw.sjlbkw.cn

[T29] Swift：guard 提前返回
来源：http://rct.xinyue.icu

guard let x = opt else { return }
来源：http://pzk.cashguo.top

[T30] Swift：协议
来源：http://lug.ydzc1.top

protocol Shape { func area() -> Double }
来源：http://ghs.shangyingyoupin.top

[T31] Lua：Hello World
来源：http://isk.meibo888.top

print("Hello")
来源：http://vmw.xylfe.cn

[T32] Lua：局部变量
来源：http://set.pycfn.com

local a = 1
来源：http://csh.jinghuilouyu.cn

[T33] Lua：表（数组）
来源：http://qly.52xcode.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://emk.ctjpmb.com

[T34] Lua：遍历表
来源：http://vmy.chenlongwang.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ich.zhaomingkeji.xyz

[T35] Lua：字典表
来源：http://vxy.pengpengdd.cyou

local d = { a = 1 };  d.b = 2
来源：http://yuf.52xcode.cn

[T36] Lua：函数
来源：http://zbm.yvedp.cn

function add(a, b) return a + b end
来源：http://xvy.ywan-chungtsiang.top

[T37] Lua：字符串拼接
来源：http://iis.jyoumei.cn

"a" .. "b"
来源：http://wua.xuanzx.com

[T38] Lua：条件
来源：http://pkk.hesvh.cn

if x > 0 then print("正") end
来源：http://wgk.mhx1999.top

[T39] Lua：模式匹配
来源：http://cbg.jyoumei.cn

string.find(s, "%d+")
来源：http://izy.cucudq.cn

[T40] Lua：元表
来源：http://psg.cqqwz.cn

setmetatable({}, { __index = base })
来源：http://lvb.haohaochexian.top

[T41] Perl：Hello World
来源：http://vsh.shuidangran.top

print "Hello\n";
来源：http://jif.guannengcc.top

[T42] Perl：变量类型
来源：http://qmw.snrcjt.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cea.bjfxy.top

[T43] Perl：字符串插值
来源：http://jbh.ivvv.top

"值: $a"
来源：http://crd.xuetiantiany.cn

[T44] Perl：条件
来源：http://jik.daria6918.cn

if ($a > 0) { print "正"; }
来源：http://jah.jqgufenzy.top

[T45] Perl：数组遍历
来源：http://bqs.cheryme.top

for my $x (@arr) { print $x; }
来源：http://pqh.cqqwz.cn

[T46] Perl：哈希操作
来源：http://lmi.jinyuanbaomall.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kgl.guowangkeji.top

[T47] Perl：正则捕获
来源：http://ybw.snrcjt.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ugd.havefunace.top

[T48] Perl：正则替换
来源：http://pbi.cheryme.top

$s =~ s/old/new/g;
来源：http://ant.hcnkem.com

[T49] Perl：函数
来源：http://prl.bbcook.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ojv.hnqzz.top

[T50] Perl：逐行读文件
来源：http://hls.tarul.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://hzr.hammf.cn

while (my $line = <$fh>) { print $line; }
来源：http://gcp.zhixingplan.top

[T51] Scala：Hello World
来源：http://lmq.nwbrower.top

println("Hello")
来源：http://ktj.tianlin.xyz

[T52] Scala：变量
来源：http://qer.sxryk.cn

val a = 1;  var b = 2
来源：http://cqe.ydjk.org.cn

[T53] Scala：字符串插值
来源：http://vqf.zhengqikj.top

s"值: $b"
来源：http://ppz.wangdashe.top

[T54] Scala：集合映射
来源：http://btt.shanyushiyangkeji.top

List(1, 2, 3).map(_ * 2)
来源：http://kpn.wangshuangyany.cn

[T55] Scala：集合过滤
来源：http://pda.ywan-chungtsiang.top

List(1, 2, 3).filter(_ > 1)
来源：http://ppg.cheryme.top

[T56] Scala：样例类
来源：http://lap.316326.xyz

case class User(name: String, age: Int)
来源：http://vnb.nwbrower.top

[T57] Scala：模式匹配
来源：http://vnm.haohaochexian.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://xyf.daxiang520.top

[T58] Scala：函数定义
来源：http://afu.guowangkeji.top

def add(a: Int, b: Int): Int = a + b
来源：http://dhu.gotoacloud.top

[T59] Scala：循环
来源：http://lts.jianghu66.top

for (i <- 1 to 10) println(i)
来源：http://dem.yonumen.top

[T60] Scala：折叠
来源：http://gmt.tanke756.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nug.hnqzz.top

================================================================================
来源：http://vzz.yueranfly.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nbg.andypj.xyz

================================================================================
来源：http://lig.cucudq.cn

[U01] Py：创建虚拟环境
来源：http://xqe.zdbjq.cn

python -m venv .venv && source .venv/bin/activate
来源：http://hbb.hywenlv.cn

[U02] Py：导出 / 安装依赖
来源：http://cla.aibaodan.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tun.yj202588.top

[U03] Py：加载 .env 配置
来源：http://rdo.hywenlv.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://oby.andypj.xyz

[U04] Py：变量调试打印
来源：http://jxs.redwolf501.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://sod.ywan-chungtsiang.top

[U05] Py：列表去重且保序
来源：http://kzg.fanxiaobao.xyz

list(dict.fromkeys(arr))
来源：http://jtc.shzxlz.cn

[U06] Py：合并两个字典
来源：http://xpg.yangfankeji.com

{**a, **b}
来源：http://rgp.ybcxt.top

[U07] Py：反转字典键值
来源：http://bwe.shangyingyoupin.top

{v: k for k, v in d.items()}
来源：http://hqs.xuanzx.com

[U08] Py：展平二维列表
来源：http://yyf.hesvh.cn

[y for x in nested for y in x]
来源：http://vwn.mhx1999.top

[U09] Py：字典取最大值的键
来源：http://woe.vqdsnc.cn

max(d, key=d.get)
来源：http://sfq.jyoumei.cn

[U10] Py：按值排序字典
来源：http://fci.hcnkem.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ecc.feifeiyinyue.top

[U11] Py：生成器表达式
来源：http://vcb.shangyingyoupin.top

(x * 2 for x in arr)
来源：http://pnz.hongshengwenyu.top

[U12] Py：取出现最多的 3 个元素
来源：http://xzq.cqqwz.cn

Counter(arr).most_common(3)
来源：http://ogv.vehdjk.com

[U13] Py：固定长度队列
来源：http://lci.hysaishi.cn

deque(maxlen=10)
来源：http://qek.yueranfly.top

[U14] Py：分组收集到列表
来源：http://out.guannengcc.top

defaultdict(list)
来源：http://trv.zhiwuduotai.top

[U15] Py：高精度计时
来源：http://grq.ctjpmb.com

t = time.perf_counter()
来源：http://dtl.hfpthk.cn

[U16] Py：命令行参数解析
来源：http://bbc.wangshuangyany.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lfy.hesvh.cn

[U17] Py：初始化日志
来源：http://eun.gotoacloud.top

logging.basicConfig(level=logging.INFO)
来源：http://syj.hongshengwenyu.top

[U18] Py：预编译正则
来源：http://yyq.snrcjt.cn

pat = re.compile(r"\d+")
来源：http://ekp.yongpay.top

[U19] Py：正则替换带回调
来源：http://bww.fanxiaobao.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ubb.zycfv.cn

[U20] Py：缓存函数结果
来源：http://qrh.yongpay.top

@functools.lru_cache(maxsize=None)
来源：http://ghq.redwolf501.top

[U21] Py：自定义上下文管理器
来源：http://frd.jlsjyb.cn

@contextlib.contextmanager
来源：http://idb.bbcook.cn

[U22] Py：矩阵转置
来源：http://isw.vehdjk.com

list(zip(*m))
来源：http://kaa.ydjk.org.cn

[U23] Py：分块读取大文件
来源：http://bpq.jyoumei.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gah.cqqwz.cn

[U24] Py：路径操作
来源：http://agt.ydjk.org.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lxt.jinghuilouyu.cn

[U25] Py：CSV 按字典读
来源：http://fyr.hnqzz.top

csv.DictReader(f)
来源：http://kpi.dashuyun.cn

[U26] Py：并发下载
来源：http://kps.yongpay.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://iyj.hcnkem.com

[U27] Py：异步 HTTP
来源：http://hdd.0kj1m.cn

aiohttp.ClientSession() 配合 async with
来源：http://csk.yangfankeji.com

[U28] Py：类型别名
来源：http://ijb.fehbvm.com

UserId = int
来源：http://zun.hesvh.cn

[U29] Py：属性校验
来源：http://vvs.aibaodan.cn

@property 与 @x.setter 配合
来源：http://wxb.nanxinkj.top

[U30] Py：数据类
来源：http://wkl.sysykeji.top

@dataclass(slots=True)
来源：http://vue.jinqigfzy.top

[U31] Py：单测
来源：http://hrb.aibaodan.cn

python -m pytest -q
来源：http://jan.cdnleiting.top

[U32] Py：代码格式化
来源：http://szy.yvedp.cn

ruff format . && ruff check --fix .
来源：http://ogb.yonumen.top

[U33] Py：打包发布
来源：http://pqr.nwbrower.top

python -m build  （依赖 pyproject.toml）
来源：http://dqb.tanke756.top

[U34] Py：判断编码
来源：http://tab.jlsjyb.cn

chardet.detect(raw)
来源：http://glj.nanxinkj.top

[U35] Py：发送邮件
来源：http://bbe.feifeiyinyue.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lje.ppjwa.cn

[U36] Py：定时任务
来源：http://elh.ctjpmb.com

schedule.every(10).minutes.do(job)
来源：http://pug.ivvv.top

[U37] Py：读写 Excel
来源：http://hkj.fzhhl.top

pandas.read_excel / DataFrame.to_excel
来源：http://esw.svipenyu.cn

[U38] Py：获取脚本所在目录
来源：http://mnu.sweek.top

Path(__file__).resolve().parent
来源：http://knv.fzhhl.top

[U39] Py：判断是否在交互环境
来源：http://bnl.meibo888.top

sys.stdout.isatty()
来源：http://hof.tanke756.top

[U40] Py：打印到标准错误
来源：http://kgu.epnwcf.com

print("err", file=sys.stderr)
来源：http://puo.nanxinkj.top

[U41] PHP：初始化 Composer 项目
来源：http://pfz.yuxming.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://hih.nwbrower.top

[U42] PHP：PSR-4 自动加载
来源：http://vem.zycfv.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qxi.chenlongwang.top

[U43] PHP：声明命名空间
来源：http://doi.zhiwuduotai.top

namespace App\Http;
来源：http://ptg.yangfankeji.com

[U44] PHP：开启严格类型
来源：http://uuc.9152youxi.cn

declare(strict_types=1);
来源：http://jgh.yangfankeji.com

[U45] PHP：类型声明与返回类型
来源：http://mhz.jqgufenzy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://iig.9152youxi.cn

[U46] PHP：可空类型
来源：http://sgf.jinyuanbaomall.cn

?string $name = null
来源：http://qcg.gzhubu.top

[U47] PHP：联合类型
来源：http://ozf.wangdashe.top

int|string $id
来源：http://jxl.ybcxt.top

[U48] PHP：纯枚举
来源：http://odg.smart0.xyz

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ubx.ydjk.org.cn

[U49] PHP：只读属性
来源：http://sxx.pycfn.com

public readonly string $name
来源：http://cpm.yongpay.top

[U50] PHP：构造器属性提升
来源：http://eyo.yueranfly.top

public function __construct(private int $id) {}
来源：http://ucv.fanxiaobao.xyz

[U51] PHP：数组解构
来源：http://bxg.ehwqpu.com

[$a, $b] = $arr;
来源：http://ktn.uphjek.com

[U52] PHP：箭头函数
来源：http://huk.tarul.cn

$double = fn($x) => $x * 2;
来源：http://nis.fanxiaobao.xyz

[U53] PHP：空合并运算符
来源：http://uge.svipenyu.cn

$v = $a ?? $b ?? "default";
来源：http://urz.aibaodan.cn

[U54] PHP：空安全调用
来源：http://kjc.havefunace.top

$obj?->method()
来源：http://bgj.snrcjt.cn

[U55] PHP：match 表达式
来源：http://tho.tian-w.cn

$s = match($x) { 1 => "一", default => "其他" };
来源：http://vvi.hfpthk.cn

[U56] PHP：命名参数
来源：http://uwi.aizwys.cn

f(a: 1, b: 2)
来源：http://slb.feifeiyinyue.top

[U57] PHP：字符串插值
来源：http://hnc.0kj1m.cn

"值: {$a}"
来源：http://jdc.cdnleiting.top

[U58] PHP：数组三件套
来源：http://yri.jyoumei.cn

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mzb.xuanzx.com

[U59] PHP：自定义排序
来源：http://pym.jqgfzy.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yyp.sjlbkw.cn

[U60] PHP：JSON 编解码
来源：http://lcn.yangfankeji.com

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://lmv.birdmap.top

[U61] PHP：正则
来源：http://wua.daria6918.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://hez.birdmap.top

[U62] PHP：日期对象
来源：http://bwj.chenzaomai.com

(new DateTimeImmutable())->format("Y-m-d");
来源：http://nta.fktsv.cn

[U63] PHP：文件读写
来源：http://sdd.haohaochexian.top

file_get_contents($f);  file_put_contents($f, $data);
来源：http://hmr.jiagoushi.top

[U64] PHP：目录遍历
来源：http://tvo.shanyushiyangtech.top

glob("dir/*.php");  scandir("dir");
来源：http://dpu.snrcjt.cn

[U65] PHP：会话
来源：http://ngd.nanxinkj.top

session_start();  $_SESSION["uid"] = 1;
来源：http://kce.ywan-chungtsiang.top

[U66] PHP：设置 Cookie
来源：http://koy.gzhubu.top

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://vfr.sweek.top

[U67] PHP：处理文件上传
来源：http://wgc.shanyushiyangtech.top

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://avd.shanyushiyangtech.top

[U68] PHP：PDO 连接
来源：http://dmy.cucudq.cn

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://fnz.zhixingplan.top


<!-- 参考信息 -->