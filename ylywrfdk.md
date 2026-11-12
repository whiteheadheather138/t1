代发 wailian999

#include <iostream>
来源：http://vnx.daria6918.cn

int main() { std::cout << "Hello\n"; }
来源：http://oqp.fengsongda.top

[S32] C++：字符串
来源：http://air.ivvv.top

std::string s = "hi";  s += "!";
来源：http://cly.havefunace.top

[S33] C++：vector 增删
来源：http://vps.sxryk.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yzt.tianlin.xyz

[S34] C++：遍历 vector
来源：http://izd.tanke756.top

for (auto &x : v) { std::cout << x; }
来源：http://tvw.xuanzx.com

[S35] C++：map
来源：http://gjy.quarkkingdee.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://alj.ywan-chungtsiang.top

[S36] C++：unordered_map
来源：http://wwl.jinyuanbaomall.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zzt.yongpay.top

[S37] C++：set
来源：http://axh.smart0.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dzu.aizwys.cn

[S38] C++：排序
来源：http://dvd.jinghuilouyu.cn

std::sort(v.begin(), v.end());
来源：http://epr.yongpay.top

[S39] C++：自定义比较器排序
来源：http://zey.zhoulong.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vfs.yongpay.top

[S40] C++：查找元素
来源：http://cza.dianchejie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://art.yangfankeji.com

[S41] C++：类与构造函数
来源：http://fya.hywenlv.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ayk.hesvh.cn

[S42] C++：继承与虚函数
来源：http://yks.vehdjk.com

class B : public Base { public: void f() override {} };
来源：http://jtc.redwolf501.top

[S43] C++：智能指针
来源：http://kpp.hysaishi.cn

auto p = std::make_unique<int>(5);
来源：http://pqt.jyoumei.cn

[S44] C++：引用传参
来源：http://uwl.gzhubu.top

void inc(int &x) { ++x; }
来源：http://fin.mhx1999.top

[S45] C++：lambda
来源：http://smq.mhx1999.top

auto add = [](int a, int b) { return a + b; };
来源：http://iol.sjlbkw.cn

[S46] C++：函数模板
来源：http://vcx.pengpengdd.cyou

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hbe.zhoulong.xyz

[S47] C++：结构化绑定遍历
来源：http://cvb.iojbl.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ljy.zhijiandao.cn

[S48] C++：逐行读文件
来源：http://yyi.jinghuilouyu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://udb.zdqjudy.top

while (std::getline(in, line)) { }
来源：http://mqk.zhoulong.xyz

[S49] C++：写文件
来源：http://lph.sweek.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tyl.c1oappe.top

[S50] C++：格式化数字
来源：http://usi.mhx1999.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qui.epnwcf.com

[S51] C++：显式类型转换
来源：http://var.chenjidiqi.icu

static_cast<double>(a) / b
来源：http://gxs.9152youxi.cn

[S52] C++：const 与 noexcept
来源：http://qtp.yj202588.top

int size() const noexcept { return n_; }
来源：http://dhu.chenjidiqi.icu

[S53] C++：移动语义
来源：http://adu.gaohongyu789.top

std::vector<int> w = std::move(v);
来源：http://foe.shuidangran.top

[S54] C++：异常处理
来源：http://hmn.ydzc1.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hwr.sweek.top

[S55] C++：结构化绑定
来源：http://kat.zhiwuduotai.top

auto [a, b] = std::make_pair(1, 2);
来源：http://unj.chenzaomai.com

[S56] C++：optional
来源：http://mjn.wangdashe.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rhs.ctjpmb.com

[S57] C++：编译期常量
来源：http://gik.xuetiantiany.cn

constexpr int N = 10;
来源：http://lan.dianchejie.cn

[S58] C++：命名空间
来源：http://ksg.hnqzz.top

namespace ns { int f() { return 1; } }
来源：http://yug.hnqzz.top

[S59] C++：静态断言
来源：http://env.ppjwa.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uaq.jinyuanbaomall.cn

[S60] C++：遍历并删除元素
来源：http://npb.hongshengwenyu.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vdm.nanxuanxn.top

================================================================================
来源：http://mxv.xuetiantiany.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://msf.nanxinkj.top

================================================================================
来源：http://grg.cheryme.top

[T01] Kotlin：Hello World
来源：http://ttv.ivvv.top

println("Hello")
来源：http://plr.jinghuilouyu.cn

[T02] Kotlin：变量
来源：http://nhz.smart0.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qhe.fengsongda.top

[T03] Kotlin：字符串模板
来源：http://smr.xuetiantiany.cn

"值: $b"
来源：http://egr.yuxming.cn

[T04] Kotlin：空安全
来源：http://wex.hesvh.cn

val n: String? = null;  n?.length
来源：http://sny.dianchejie.cn

[T05] Kotlin：when 表达式
来源：http://fsr.zdbjq.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hui.aibaodan.cn

[T06] Kotlin：集合映射
来源：http://nze.chenzaomai.com

listOf(1, 2, 3).map { it * 2 }
来源：http://vpl.andypj.xyz

[T07] Kotlin：集合过滤
来源：http://qwm.zhoulong.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://llp.yueranfly.top

[T08] Kotlin：数据类
来源：http://zeq.svipenyu.cn

data class User(val name: String, val age: Int)
来源：http://hlm.aibaodan.cn

[T09] Kotlin：扩展函数
来源：http://uxt.shuidangran.top

fun String.exclaim() = this + "!"
来源：http://eod.aibaodan.cn

[T10] Kotlin：默认参数
来源：http://one.xziqi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://aym.nwbrower.top

[T11] Kotlin：协程
来源：http://xkz.tianlin.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://dnl.yuanzhike.top

[T12] Kotlin：解构声明
来源：http://dxd.jinqigfzy.top

val (a, b) = Pair(1, 2)
来源：http://ilb.xziqi.cn

[T13] Kotlin：只读 Map
来源：http://dwa.xuanzx.com

val m = mapOf("a" to 1)
来源：http://cmk.yonumen.top

[T14] Kotlin：循环
来源：http://ckt.haohaochexian.top

for (i in 1..10) println(i)
来源：http://pci.hysaishi.cn

[T15] Kotlin：接口
来源：http://kit.fzhhl.top

interface Shape { fun area(): Double }
来源：http://rgx.yuxming.cn

[T16] Swift：Hello World
来源：http://dol.hfpthk.cn

print("Hello")
来源：http://opt.iojbl.cn

[T17] Swift：变量与常量
来源：http://vau.ydzc1.top

var a = 1;  let b = 2
来源：http://pdq.yongpay.top

[T18] Swift：字符串插值
来源：http://orl.dashuyun.cn

"值: \(b)"
来源：http://lbv.jyoumei.cn

[T19] Swift：可选绑定
来源：http://jjo.cheryme.top

if let n = opt { print(n) }
来源：http://byr.aibaodan.cn

[T20] Swift：数组操作
来源：http://wgq.zhongyouzk.top

var a = [1, 2, 3];  a.append(4)
来源：http://lzi.guowangkeji.top

[T21] Swift：遍历
来源：http://ngt.sweek.top

for x in a { print(x) }
来源：http://fla.yueranfly.top

[T22] Swift：字典
来源：http://rcx.tanke756.top

var d = ["a": 1];  d["b"] = 2
来源：http://rlp.cashguo.top

[T23] Swift：函数
来源：http://fca.iojbl.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sqd.vqdsnc.cn

[T24] Swift：闭包
来源：http://yxr.hongshengwenyu.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://wyk.hysaishi.cn

[T25] Swift：结构体
来源：http://enc.quarkkingdee.top

struct P { var x: Int }
来源：http://jnp.xinyue.icu

[T26] Swift：类与重写
来源：http://vau.jinqigfzy.top

class A: Base { override func f() {} }
来源：http://nzh.jqgufenzy.top

[T27] Swift：错误处理
来源：http://jin.tarul.cn

do { try f() } catch { print(error) }
来源：http://kum.sjlbkw.cn

[T28] Swift：枚举
来源：http://yce.tanke756.top

enum Color { case red, green }
来源：http://jeu.gzhubu.top

[T29] Swift：guard 提前返回
来源：http://umg.hongshengwenyu.top

guard let x = opt else { return }
来源：http://xxp.pycfn.com

[T30] Swift：协议
来源：http://okj.bbcook.cn

protocol Shape { func area() -> Double }
来源：http://xyr.shuidangran.top

[T31] Lua：Hello World
来源：http://rhk.jyoumei.cn

print("Hello")
来源：http://lbj.yongpay.top

[T32] Lua：局部变量
来源：http://tcx.smart0.xyz

local a = 1
来源：http://edf.jyoumei.cn

[T33] Lua：表（数组）
来源：http://djm.ybcxt.top

local t = {1, 2, 3};  t[4] = 4
来源：http://zkd.zhengqikj.top

[T34] Lua：遍历表
来源：http://kvu.xziqi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://jfw.sysykeji.top

[T35] Lua：字典表
来源：http://ljv.daxiang520.top

local d = { a = 1 };  d.b = 2
来源：http://ewg.xuetiantiany.cn

[T36] Lua：函数
来源：http://riu.xingfuxueyuan.xyz

function add(a, b) return a + b end
来源：http://ocj.xylfe.cn

[T37] Lua：字符串拼接
来源：http://usa.zdbjq.cn

"a" .. "b"
来源：http://ite.meibo888.top

[T38] Lua：条件
来源：http://cyo.nanxuanxn.top

if x > 0 then print("正") end
来源：http://klr.chenzaomai.com

[T39] Lua：模式匹配
来源：http://doj.cucudq.cn

string.find(s, "%d+")
来源：http://nft.tanke756.top

[T40] Lua：元表
来源：http://pzn.guannengcc.top

setmetatable({}, { __index = base })
来源：http://ssi.hfpthk.cn

[T41] Perl：Hello World
来源：http://vbs.hnqzz.top

print "Hello\n";
来源：http://ocv.zycfv.cn

[T42] Perl：变量类型
来源：http://fbn.jqgfzy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tyo.jinyuanbaomall.cn

[T43] Perl：字符串插值
来源：http://bdq.jlsjyb.cn

"值: $a"
来源：http://esd.feifeiyinyue.top

[T44] Perl：条件
来源：http://ieg.feifeiyinyue.top

if ($a > 0) { print "正"; }
来源：http://gsv.meibo888.top

[T45] Perl：数组遍历
来源：http://mug.gzhubu.top

for my $x (@arr) { print $x; }
来源：http://lhf.kuanghao11.cn

[T46] Perl：哈希操作
来源：http://xff.hcnkem.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jbo.kuanghao11.cn

[T47] Perl：正则捕获
来源：http://nle.yj202588.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ypb.nanxinkj.top

[T48] Perl：正则替换
来源：http://vkl.hesvh.cn

$s =~ s/old/new/g;
来源：http://kjp.yonumen.top

[T49] Perl：函数
来源：http://gam.gogol.net.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sjq.xuetiantiany.cn

[T50] Perl：逐行读文件
来源：http://ehq.bjfxy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ouh.yj20258.top

while (my $line = <$fh>) { print $line; }
来源：http://koy.zhengqikj.top

[T51] Scala：Hello World
来源：http://man.ppjwa.cn

println("Hello")
来源：http://mtz.aizwys.cn

[T52] Scala：变量
来源：http://gci.c1oappe.top

val a = 1;  var b = 2
来源：http://bul.shuidangran.top

[T53] Scala：字符串插值
来源：http://dnd.pengpengdd.cyou

s"值: $b"
来源：http://uwp.wangdashe.top

[T54] Scala：集合映射
来源：http://wcs.sjlbkw.cn

List(1, 2, 3).map(_ * 2)
来源：http://fdv.fanxiaobao.xyz

[T55] Scala：集合过滤
来源：http://bvm.hcnkem.com

List(1, 2, 3).filter(_ > 1)
来源：http://loz.ywan-chungtsiang.top

[T56] Scala：样例类
来源：http://lmv.guowangkeji.top

case class User(name: String, age: Int)
来源：http://fbb.dianchejie.cn

[T57] Scala：模式匹配
来源：http://fvf.zhengqikj.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://wio.hnqzz.top

[T58] Scala：函数定义
来源：http://vdy.xuetiantiany.cn

def add(a: Int, b: Int): Int = a + b
来源：http://utm.shzxlz.cn

[T59] Scala：循环
来源：http://lvo.zhaomingkeji.xyz

for (i <- 1 to 10) println(i)
来源：http://fho.jiagoushi.top

[T60] Scala：折叠
来源：http://rai.shzxlz.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hmh.yueranfly.top

================================================================================
来源：http://opr.dashuyun.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ypi.hywenlv.cn

================================================================================
来源：http://gzg.meibo888.top

[U01] Py：创建虚拟环境
来源：http://bbk.yj20258.top

python -m venv .venv && source .venv/bin/activate
来源：http://hlk.chenzaomai.com

[U02] Py：导出 / 安装依赖
来源：http://ogc.zhongyouzk.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mhl.nanxuanxn.top

[U03] Py：加载 .env 配置
来源：http://iwi.wangshuangyany.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rty.epnwcf.com

[U04] Py：变量调试打印
来源：http://uof.jinghuilouyu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ycg.shanyushiyangkeji.top

[U05] Py：列表去重且保序
来源：http://jkr.jinghuilouyu.cn

list(dict.fromkeys(arr))
来源：http://ijg.nanxuanxn.top

[U06] Py：合并两个字典
来源：http://jxd.yfazqb.com

{**a, **b}
来源：http://agy.ybcxt.top

[U07] Py：反转字典键值
来源：http://xan.xuetiantiany.cn

{v: k for k, v in d.items()}
来源：http://nig.9152youxi.cn

[U08] Py：展平二维列表
来源：http://sim.xuanzx.com

[y for x in nested for y in x]
来源：http://ukg.yj20258.top

[U09] Py：字典取最大值的键
来源：http://ter.sysykeji.top

max(d, key=d.get)
来源：http://yxf.sxryk.cn

[U10] Py：按值排序字典
来源：http://gtl.wangdashe.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mzx.hnqzz.top

[U11] Py：生成器表达式
来源：http://xgy.smart0.xyz

(x * 2 for x in arr)
来源：http://hbf.c1oappe.top

[U12] Py：取出现最多的 3 个元素
来源：http://soz.vqdsnc.cn

Counter(arr).most_common(3)
来源：http://wri.svipenyu.cn

[U13] Py：固定长度队列
来源：http://fux.zhiwuduotai.top

deque(maxlen=10)
来源：http://haz.yangfankeji.com

[U14] Py：分组收集到列表
来源：http://erp.cqqwz.cn

defaultdict(list)
来源：http://ust.aibaodan.cn

[U15] Py：高精度计时
来源：http://zuo.tanke756.top

t = time.perf_counter()
来源：http://cmu.redwolf501.top

[U16] Py：命令行参数解析
来源：http://piu.xuanzx.com

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://coi.jinqigfzy.top

[U17] Py：初始化日志
来源：http://vvs.ivvv.top

logging.basicConfig(level=logging.INFO)
来源：http://nzd.fzhhl.top

[U18] Py：预编译正则
来源：http://qyw.jinqigfzy.top

pat = re.compile(r"\d+")
来源：http://qan.guowangkeji.top

[U19] Py：正则替换带回调
来源：http://qyv.yfazqb.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sjb.haohaochexian.top

[U20] Py：缓存函数结果
来源：http://tba.ydzc1.top

@functools.lru_cache(maxsize=None)
来源：http://gru.ppjwa.cn

[U21] Py：自定义上下文管理器
来源：http://fei.dianchejie.cn

@contextlib.contextmanager
来源：http://lwu.ctjpmb.com

[U22] Py：矩阵转置
来源：http://rsq.bjfxy.top

list(zip(*m))
来源：http://dkn.yangfankeji.com

[U23] Py：分块读取大文件
来源：http://xsb.pycfn.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://klo.shanyushiyangkeji.top

[U24] Py：路径操作
来源：http://jqc.tianlin.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://nyc.yuxming.cn

[U25] Py：CSV 按字典读
来源：http://yrk.wangdashe.top

csv.DictReader(f)
来源：http://yms.fzhhl.top

[U26] Py：并发下载
来源：http://imu.nanxuanxn.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://edv.hongshengwenyu.top

[U27] Py：异步 HTTP
来源：http://eis.chenjidiqi.icu

aiohttp.ClientSession() 配合 async with
来源：http://ddo.fzhhl.top

[U28] Py：类型别名
来源：http://pog.nanxinkj.top

UserId = int
来源：http://sgb.cucudq.cn

[U29] Py：属性校验
来源：http://vgh.fktsv.cn

@property 与 @x.setter 配合
来源：http://mxg.chenjidiqi.icu

[U30] Py：数据类
来源：http://hzl.pycfn.com

@dataclass(slots=True)
来源：http://hqd.zhongyouzk.top

[U31] Py：单测
来源：http://men.hywenlv.cn

python -m pytest -q
来源：http://tcb.yanxiufei.cn

[U32] Py：代码格式化
来源：http://sja.bbcook.cn

ruff format . && ruff check --fix .
来源：http://eog.haohaochexian.top

[U33] Py：打包发布
来源：http://osr.guannengcc.top

python -m build  （依赖 pyproject.toml）
来源：http://ivh.316326.xyz

[U34] Py：判断编码
来源：http://reo.xingfuxueyuan.xyz

chardet.detect(raw)
来源：http://qqg.ppjwa.cn

[U35] Py：发送邮件
来源：http://aqs.daxiang520.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tzm.hammf.cn

[U36] Py：定时任务
来源：http://qwd.wangshuangyany.cn

schedule.every(10).minutes.do(job)
来源：http://ozy.cdnleiting.top

[U37] Py：读写 Excel
来源：http://ets.ctjpmb.com

pandas.read_excel / DataFrame.to_excel
来源：http://mis.fengsongda.top

[U38] Py：获取脚本所在目录
来源：http://kms.hnxiangtu.top

Path(__file__).resolve().parent
来源：http://dwb.meibo888.top

[U39] Py：判断是否在交互环境
来源：http://bep.shzxlz.cn

sys.stdout.isatty()
来源：http://hip.guannengcc.top

[U40] Py：打印到标准错误
来源：http://ncs.mhx1999.top

print("err", file=sys.stderr)
来源：http://ycx.ivvv.top

[U41] PHP：初始化 Composer 项目
来源：http://yyh.tarul.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://rwr.pengpengdd.cyou

[U42] PHP：PSR-4 自动加载
来源：http://qhw.cashguo.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fbq.shuidangran.top

[U43] PHP：声明命名空间
来源：http://jbm.hammf.cn

namespace App\Http;
来源：http://kev.vehdjk.com

[U44] PHP：开启严格类型
来源：http://zvy.chenzaomai.com

declare(strict_types=1);
来源：http://cwq.meibo888.top

[U45] PHP：类型声明与返回类型
来源：http://ptc.bjfxy.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://zpg.jinyuanbaomall.cn

[U46] PHP：可空类型
来源：http://pvj.52xcode.cn

?string $name = null
来源：http://sbq.aibaodan.cn

[U47] PHP：联合类型
来源：http://afb.jqgfzy.top

int|string $id
来源：http://lac.zhongyouzk.top

[U48] PHP：纯枚举
来源：http://rux.svipenyu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://hdd.smart0.xyz

[U49] PHP：只读属性
来源：http://ktz.sysykeji.top

public readonly string $name
来源：http://egg.xingfuxueyuan.xyz

[U50] PHP：构造器属性提升
来源：http://zzs.jyoumei.cn

public function __construct(private int $id) {}
来源：http://qok.uphjek.com

[U51] PHP：数组解构
来源：http://gin.hysaishi.cn

[$a, $b] = $arr;
来源：http://gyn.dashuyun.cn

[U52] PHP：箭头函数
来源：http://gov.xylfe.cn

$double = fn($x) => $x * 2;
来源：http://rcs.aizwys.cn

[U53] PHP：空合并运算符
来源：http://osj.vehdjk.com

$v = $a ?? $b ?? "default";
来源：http://eaa.ppjwa.cn

[U54] PHP：空安全调用
来源：http://vnb.ydzc1.top

$obj?->method()
来源：http://bom.52xcode.cn

[U55] PHP：match 表达式
来源：http://cwb.cdnleiting.top

$s = match($x) { 1 => "一", default => "其他" };
来源：http://hae.yuxming.cn

[U56] PHP：命名参数
来源：http://nwl.mhx1999.top

f(a: 1, b: 2)
来源：http://rdy.c1oappe.top


<!-- 参考信息 -->