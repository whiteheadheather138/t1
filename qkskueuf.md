代发 wailian999

[S39] C++：自定义比较器排序
来源：http://sws.tianlin.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://glb.fengsongda.top

[S40] C++：查找元素
来源：http://sfc.jyoumei.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kfb.xinyue.icu

[S41] C++：类与构造函数
来源：http://adn.hesvh.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ggt.cdnleiting.top

[S42] C++：继承与虚函数
来源：http://wgc.guowangkeji.top

class B : public Base { public: void f() override {} };
来源：http://ilr.zhongyouzk.top

[S43] C++：智能指针
来源：http://xvo.jqgufenzy.top

auto p = std::make_unique<int>(5);
来源：http://cpr.hcnkem.com

[S44] C++：引用传参
来源：http://xej.hcnkem.com

void inc(int &x) { ++x; }
来源：http://xss.ivvv.top

[S45] C++：lambda
来源：http://jnb.vehdjk.com

auto add = [](int a, int b) { return a + b; };
来源：http://fge.sweek.top

[S46] C++：函数模板
来源：http://cft.wangdashe.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yfp.chenzaomai.com

[S47] C++：结构化绑定遍历
来源：http://zxw.pycfn.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kxb.ydzc1.top

[S48] C++：逐行读文件
来源：http://ylm.yj202588.top

std::ifstream in("a.txt");  std::string line;
来源：http://cqe.kuanghao11.cn

while (std::getline(in, line)) { }
来源：http://osw.yongpay.top

[S49] C++：写文件
来源：http://yyr.jianghu66.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kva.ywan-chungtsiang.top

[S50] C++：格式化数字
来源：http://tyr.hysaishi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uze.xziqi.cn

[S51] C++：显式类型转换
来源：http://lsx.zdqjudy.top

static_cast<double>(a) / b
来源：http://uci.hywenlv.cn

[S52] C++：const 与 noexcept
来源：http://elz.zdbjq.cn

int size() const noexcept { return n_; }
来源：http://mmp.yj20258.top

[S53] C++：移动语义
来源：http://yni.xingfuxueyuan.xyz

std::vector<int> w = std::move(v);
来源：http://fmr.jinqigufen.top

[S54] C++：异常处理
来源：http://ktn.wangdashe.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mbu.c1oappe.top

[S55] C++：结构化绑定
来源：http://gss.ivvv.top

auto [a, b] = std::make_pair(1, 2);
来源：http://yhh.gaohongyu789.top

[S56] C++：optional
来源：http://vdu.chenzaomai.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hit.shanyushiyangtech.top

[S57] C++：编译期常量
来源：http://ixt.cashguo.top

constexpr int N = 10;
来源：http://dln.bjfxy.top

[S58] C++：命名空间
来源：http://qld.jqgfzy.top

namespace ns { int f() { return 1; } }
来源：http://khq.shuidangran.top

[S59] C++：静态断言
来源：http://gvr.zhengqikj.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://idc.jinyuanbaomall.cn

[S60] C++：遍历并删除元素
来源：http://jup.zdqjudy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ixw.ctjpmb.com

================================================================================
来源：http://tdm.ywan-chungtsiang.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pfy.jiagoushi.top

================================================================================
来源：http://piq.zdqjudy.top

[T01] Kotlin：Hello World
来源：http://zub.sxryk.cn

println("Hello")
来源：http://fcy.feifeiyinyue.top

[T02] Kotlin：变量
来源：http://nof.tanke756.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pqv.shuidangran.top

[T03] Kotlin：字符串模板
来源：http://reh.daria6918.cn

"值: $b"
来源：http://mni.xylfe.cn

[T04] Kotlin：空安全
来源：http://rsp.hysaishi.cn

val n: String? = null;  n?.length
来源：http://ghq.sweek.top

[T05] Kotlin：when 表达式
来源：http://plj.quarkkingdee.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ngx.zhixingplan.top

[T06] Kotlin：集合映射
来源：http://ssn.meibo888.top

listOf(1, 2, 3).map { it * 2 }
来源：http://vbl.redwolf501.top

[T07] Kotlin：集合过滤
来源：http://dzn.tanke756.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://zbp.pengpengdd.cyou

[T08] Kotlin：数据类
来源：http://qsk.shzxlz.cn

data class User(val name: String, val age: Int)
来源：http://pkm.fzhhl.top

[T09] Kotlin：扩展函数
来源：http://odt.aizwys.cn

fun String.exclaim() = this + "!"
来源：http://ana.cdnleiting.top

[T10] Kotlin：默认参数
来源：http://ypa.tianlin.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://alr.hesvh.cn

[T11] Kotlin：协程
来源：http://fjs.ywan-chungtsiang.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ewp.hnxiangtu.top

[T12] Kotlin：解构声明
来源：http://hsq.cqqwz.cn

val (a, b) = Pair(1, 2)
来源：http://kpy.cqqwz.cn

[T13] Kotlin：只读 Map
来源：http://phg.yvedp.cn

val m = mapOf("a" to 1)
来源：http://ldy.cucudq.cn

[T14] Kotlin：循环
来源：http://acu.zycfv.cn

for (i in 1..10) println(i)
来源：http://hpg.ydzc1.top

[T15] Kotlin：接口
来源：http://nby.bjfxy.top

interface Shape { fun area(): Double }
来源：http://voh.yj20258888.top

[T16] Swift：Hello World
来源：http://rrv.ppjwa.cn

print("Hello")
来源：http://baq.shzxlz.cn

[T17] Swift：变量与常量
来源：http://nvt.ydjk.org.cn

var a = 1;  let b = 2
来源：http://die.zhengqikj.top

[T18] Swift：字符串插值
来源：http://bqr.ctjpmb.com

"值: \(b)"
来源：http://jzy.chenzaomai.com

[T19] Swift：可选绑定
来源：http://xya.cqqwz.cn

if let n = opt { print(n) }
来源：http://tnq.guowangkeji.top

[T20] Swift：数组操作
来源：http://feg.shzxlz.cn

var a = [1, 2, 3];  a.append(4)
来源：http://kgv.yanxiufei.cn

[T21] Swift：遍历
来源：http://ujf.xinyue.icu

for x in a { print(x) }
来源：http://tov.cdnleiting.top

[T22] Swift：字典
来源：http://yhy.ybcxt.top

var d = ["a": 1];  d["b"] = 2
来源：http://ugp.feifeiyinyue.top

[T23] Swift：函数
来源：http://fyk.uphjek.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lfr.yj20258888.top

[T24] Swift：闭包
来源：http://tfx.jinqigufen.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://fmq.bbcook.cn

[T25] Swift：结构体
来源：http://fbi.xinyue.icu

struct P { var x: Int }
来源：http://yby.yuanzhike.top

[T26] Swift：类与重写
来源：http://aub.svipenyu.cn

class A: Base { override func f() {} }
来源：http://jxd.daria6918.cn

[T27] Swift：错误处理
来源：http://cdi.redwolf501.top

do { try f() } catch { print(error) }
来源：http://rlb.vehdjk.com

[T28] Swift：枚举
来源：http://raa.yonumen.top

enum Color { case red, green }
来源：http://irr.xziqi.cn

[T29] Swift：guard 提前返回
来源：http://whr.nwbrower.top

guard let x = opt else { return }
来源：http://prg.gogol.net.cn

[T30] Swift：协议
来源：http://ibq.wangshuangyany.cn

protocol Shape { func area() -> Double }
来源：http://cyr.fktsv.cn

[T31] Lua：Hello World
来源：http://woy.iojbl.cn

print("Hello")
来源：http://hsv.jinghuilouyu.cn

[T32] Lua：局部变量
来源：http://hmi.andypj.xyz

local a = 1
来源：http://rqw.shangyingyoupin.top

[T33] Lua：表（数组）
来源：http://uuw.cashguo.top

local t = {1, 2, 3};  t[4] = 4
来源：http://eoj.haohaochexian.top

[T34] Lua：遍历表
来源：http://coo.zdqjudy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://yui.xuetiantiany.cn

[T35] Lua：字典表
来源：http://uik.yvedp.cn

local d = { a = 1 };  d.b = 2
来源：http://itj.fengsongda.top

[T36] Lua：函数
来源：http://jbv.9152youxi.cn

function add(a, b) return a + b end
来源：http://tzo.daxiang520.top

[T37] Lua：字符串拼接
来源：http://ikf.vehdjk.com

"a" .. "b"
来源：http://epo.snrcjt.cn

[T38] Lua：条件
来源：http://ynm.sysykeji.top

if x > 0 then print("正") end
来源：http://oen.ywan-chungtsiang.top

[T39] Lua：模式匹配
来源：http://jix.yfazqb.com

string.find(s, "%d+")
来源：http://efs.nwbrower.top

[T40] Lua：元表
来源：http://hma.guannengcc.top

setmetatable({}, { __index = base })
来源：http://dwy.yj20258.top

[T41] Perl：Hello World
来源：http://rkt.shuidangran.top

print "Hello\n";
来源：http://thu.jinghuilouyu.cn

[T42] Perl：变量类型
来源：http://zhz.fanxiaobao.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nas.zhengqikj.top

[T43] Perl：字符串插值
来源：http://bmj.birdmap.top

"值: $a"
来源：http://cib.daria6918.cn

[T44] Perl：条件
来源：http://zuw.epnwcf.com

if ($a > 0) { print "正"; }
来源：http://bpa.svipenyu.cn

[T45] Perl：数组遍历
来源：http://xus.smart0.xyz

for my $x (@arr) { print $x; }
来源：http://jrm.ywan-chungtsiang.top

[T46] Perl：哈希操作
来源：http://isu.zhengqikj.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ulh.zhoulong.xyz

[T47] Perl：正则捕获
来源：http://leh.meibo888.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ksi.hesvh.cn

[T48] Perl：正则替换
来源：http://tmc.havefunace.top

$s =~ s/old/new/g;
来源：http://qhc.meibo888.top

[T49] Perl：函数
来源：http://riy.cheryme.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ihd.xingfuxueyuan.xyz

[T50] Perl：逐行读文件
来源：http://vlv.hfpthk.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://tsa.yj202588.top

while (my $line = <$fh>) { print $line; }
来源：http://tok.zhoulong.xyz

[T51] Scala：Hello World
来源：http://pij.nwbrower.top

println("Hello")
来源：http://thb.mhx1999.top

[T52] Scala：变量
来源：http://rag.guannengcc.top

val a = 1;  var b = 2
来源：http://wel.jqgfzy.top

[T53] Scala：字符串插值
来源：http://toc.gaohongyu789.top

s"值: $b"
来源：http://fbx.yj20258.top

[T54] Scala：集合映射
来源：http://xxn.jiagoushi.top

List(1, 2, 3).map(_ * 2)
来源：http://oer.fzhhl.top

[T55] Scala：集合过滤
来源：http://jlj.zhiwuduotai.top

List(1, 2, 3).filter(_ > 1)
来源：http://tqr.tanke756.top

[T56] Scala：样例类
来源：http://fsn.redwolf501.top

case class User(name: String, age: Int)
来源：http://ujd.cheryme.top

[T57] Scala：模式匹配
来源：http://vag.yuxming.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://his.yonumen.top

[T58] Scala：函数定义
来源：http://evy.vqdsnc.cn

def add(a: Int, b: Int): Int = a + b
来源：http://lmk.ctjpmb.com

[T59] Scala：循环
来源：http://qfk.jyoumei.cn

for (i <- 1 to 10) println(i)
来源：http://ngc.tanke756.top

[T60] Scala：折叠
来源：http://sus.nanxinkj.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://uxu.jinqigufen.top

================================================================================
来源：http://kes.ehwqpu.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dga.iojbl.cn

================================================================================
来源：http://hnh.hywenlv.cn

[U01] Py：创建虚拟环境
来源：http://vdv.jinqigufen.top

python -m venv .venv && source .venv/bin/activate
来源：http://qgv.haohaochexian.top

[U02] Py：导出 / 安装依赖
来源：http://xjd.yj20258.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lha.xziqi.cn

[U03] Py：加载 .env 配置
来源：http://hqr.cqqwz.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://cre.shangyingyoupin.top

[U04] Py：变量调试打印
来源：http://lwx.cheryme.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mas.yj20258.top

[U05] Py：列表去重且保序
来源：http://kbr.yvedp.cn

list(dict.fromkeys(arr))
来源：http://mhq.52xcode.cn

[U06] Py：合并两个字典
来源：http://pkp.jianghu66.top

{**a, **b}
来源：http://krb.zhijiandao.cn

[U07] Py：反转字典键值
来源：http://zsg.andypj.xyz

{v: k for k, v in d.items()}
来源：http://ano.shanyushiyangkeji.top

[U08] Py：展平二维列表
来源：http://hza.xinyue.icu

[y for x in nested for y in x]
来源：http://zvo.hongshengwenyu.top

[U09] Py：字典取最大值的键
来源：http://dbg.hywenlv.cn

max(d, key=d.get)
来源：http://cxq.cqqwz.cn

[U10] Py：按值排序字典
来源：http://vqe.xziqi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bmd.xylfe.cn

[U11] Py：生成器表达式
来源：http://qef.sweek.top

(x * 2 for x in arr)
来源：http://all.gogol.net.cn

[U12] Py：取出现最多的 3 个元素
来源：http://iuv.tian-w.cn

Counter(arr).most_common(3)
来源：http://qqc.tarul.cn

[U13] Py：固定长度队列
来源：http://mah.yangfankeji.com

deque(maxlen=10)
来源：http://ejy.meibo888.top

[U14] Py：分组收集到列表
来源：http://njc.shanyushiyangkeji.top

defaultdict(list)
来源：http://csy.epnwcf.com

[U15] Py：高精度计时
来源：http://zuj.shanyushiyangtech.top

t = time.perf_counter()
来源：http://xta.jiagoushi.top

[U16] Py：命令行参数解析
来源：http://iul.jianghu66.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://lvl.fanxiaobao.xyz

[U17] Py：初始化日志
来源：http://tdi.jinqigfzy.top

logging.basicConfig(level=logging.INFO)
来源：http://ktv.nanxuanxn.top

[U18] Py：预编译正则
来源：http://ywv.jqgfzy.top

pat = re.compile(r"\d+")
来源：http://kpa.nwbrower.top

[U19] Py：正则替换带回调
来源：http://hhk.zdbjq.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ofl.guannengcc.top

[U20] Py：缓存函数结果
来源：http://rjo.xingfuxueyuan.xyz

@functools.lru_cache(maxsize=None)
来源：http://crl.epnwcf.com

[U21] Py：自定义上下文管理器
来源：http://zip.hywenlv.cn

@contextlib.contextmanager
来源：http://gft.shuidangran.top

[U22] Py：矩阵转置
来源：http://rxm.daxiang520.top

list(zip(*m))
来源：http://arw.shanyushiyangkeji.top

[U23] Py：分块读取大文件
来源：http://qyy.hnqzz.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://uxt.zhengqikj.top

[U24] Py：路径操作
来源：http://fou.guowangkeji.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://lxk.zhongyouzk.top

[U25] Py：CSV 按字典读
来源：http://nro.xingfuxueyuan.xyz

csv.DictReader(f)
来源：http://orz.tarul.cn

[U26] Py：并发下载
来源：http://uje.hywenlv.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mju.redwolf501.top

[U27] Py：异步 HTTP
来源：http://otx.jqgfzy.top

aiohttp.ClientSession() 配合 async with
来源：http://mlt.yuanzhike.top

[U28] Py：类型别名
来源：http://arj.wangshuangyany.cn

UserId = int
来源：http://anu.ybcxt.top

[U29] Py：属性校验
来源：http://ikm.fzhhl.top

@property 与 @x.setter 配合
来源：http://wuw.shanyushiyangtech.top

[U30] Py：数据类
来源：http://gyz.zhixingplan.top

@dataclass(slots=True)
来源：http://eui.andypj.xyz

[U31] Py：单测
来源：http://zco.9152youxi.cn

python -m pytest -q
来源：http://rlm.xuetiantiany.cn

[U32] Py：代码格式化
来源：http://lxn.iojbl.cn

ruff format . && ruff check --fix .
来源：http://xrx.9152youxi.cn

[U33] Py：打包发布
来源：http://fuv.hnxiangtu.top

python -m build  （依赖 pyproject.toml）
来源：http://tix.tianlin.xyz

[U34] Py：判断编码
来源：http://qfv.fengsongda.top

chardet.detect(raw)
来源：http://hlx.zhixingplan.top

[U35] Py：发送邮件
来源：http://ndg.ybcxt.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://lwf.guannengcc.top

[U36] Py：定时任务
来源：http://cug.fehbvm.com

schedule.every(10).minutes.do(job)
来源：http://xgp.havefunace.top

[U37] Py：读写 Excel
来源：http://zgu.ppjwa.cn

pandas.read_excel / DataFrame.to_excel
来源：http://wnf.0kj1m.cn

[U38] Py：获取脚本所在目录
来源：http://cxc.hfpthk.cn

Path(__file__).resolve().parent
来源：http://gvj.jinghuilouyu.cn

[U39] Py：判断是否在交互环境
来源：http://oje.zhaomingkeji.xyz

sys.stdout.isatty()
来源：http://hie.cashguo.top

[U40] Py：打印到标准错误
来源：http://qwo.fktsv.cn

print("err", file=sys.stderr)
来源：http://oma.tian-w.cn

[U41] PHP：初始化 Composer 项目
来源：http://jra.fehbvm.com

composer init;  composer require guzzlehttp/guzzle
来源：http://why.chenjidiqi.icu

[U42] PHP：PSR-4 自动加载
来源：http://ttx.yvedp.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vqu.ctjpmb.com

[U43] PHP：声明命名空间
来源：http://ydv.xylfe.cn

namespace App\Http;
来源：http://jqy.shangyingyoupin.top

[U44] PHP：开启严格类型
来源：http://vmx.tianlin.xyz

declare(strict_types=1);
来源：http://tdt.yonumen.top

[U45] PHP：类型声明与返回类型
来源：http://ovl.dianchejie.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://cml.bjfxy.top

[U46] PHP：可空类型
来源：http://sxk.yuanzhike.top

?string $name = null
来源：http://roq.zdbjq.cn

[U47] PHP：联合类型
来源：http://vkz.sysykeji.top

int|string $id
来源：http://faw.fehbvm.com

[U48] PHP：纯枚举
来源：http://yvh.ivvv.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://itd.aizwys.cn

[U49] PHP：只读属性
来源：http://gal.aizwys.cn

public readonly string $name
来源：http://shv.hongshengwenyu.top

[U50] PHP：构造器属性提升
来源：http://fso.feifeiyinyue.top

public function __construct(private int $id) {}
来源：http://xjd.52xcode.cn

[U51] PHP：数组解构
来源：http://ywe.xuetiantiany.cn

[$a, $b] = $arr;
来源：http://iue.hywenlv.cn

[U52] PHP：箭头函数
来源：http://opd.zhixingplan.top

$double = fn($x) => $x * 2;
来源：http://qnk.pycfn.com

[U53] PHP：空合并运算符
来源：http://kau.fehbvm.com

$v = $a ?? $b ?? "default";
来源：http://kby.hongshengwenyu.top

[U54] PHP：空安全调用
来源：http://awn.xinyue.icu

$obj?->method()
来源：http://mzi.epnwcf.com

[U55] PHP：match 表达式
来源：http://ila.shanyushiyangkeji.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://bka.xziqi.cn

[U56] PHP：命名参数
来源：http://rtt.sjlbkw.cn

f(a: 1, b: 2)
来源：http://lsw.hywenlv.cn

[U57] PHP：字符串插值
来源：http://hfz.jinghuilouyu.cn

"值: {$a}"
来源：http://nsz.ehwqpu.com

[U58] PHP：数组三件套
来源：http://juw.vehdjk.com

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://ofx.meibo888.top

[U59] PHP：自定义排序
来源：http://rwy.redwolf501.top

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://jwg.sysykeji.top

[U60] PHP：JSON 编解码
来源：http://oox.316326.xyz

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://tgl.andypj.xyz

[U61] PHP：正则
来源：http://axn.xuetiantiany.cn

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://asp.redwolf501.top

[U62] PHP：日期对象
来源：http://rwl.c1oappe.top

(new DateTimeImmutable())->format("Y-m-d");
来源：http://gud.jinghuilouyu.cn

[U63] PHP：文件读写
来源：http://xcr.zycfv.cn

file_get_contents($f);  file_put_contents($f, $data);
来源：http://gee.jyoumei.cn

[U64] PHP：目录遍历
来源：http://nrn.mhx1999.top

glob("dir/*.php");  scandir("dir");
来源：http://fji.jlsjyb.cn


<!-- 参考信息 -->