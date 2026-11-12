代发 wailian999

static int counter = 0;
来源：http://eik.yangfankeji.com

[S29] C：变参函数
来源：http://xix.quarkkingdee.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uip.zhijiandao.cn

[S30] C：头文件保护
来源：http://rto.shanyushiyangtech.top

#ifndef X_H
来源：http://nbc.bjfxy.top

#define X_H
来源：http://coh.zhoulong.xyz

#endif
来源：http://nmc.52xcode.cn

[S31] C++：Hello World
来源：http://cln.smart0.xyz

#include <iostream>
来源：http://egz.aibaodan.cn

int main() { std::cout << "Hello\n"; }
来源：http://cue.feifeiyinyue.top

[S32] C++：字符串
来源：http://kll.birdmap.top

std::string s = "hi";  s += "!";
来源：http://msg.hesvh.cn

[S33] C++：vector 增删
来源：http://ybu.nanxuanxn.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fvw.zycfv.cn

[S34] C++：遍历 vector
来源：http://nhy.shanyushiyangtech.top

for (auto &x : v) { std::cout << x; }
来源：http://gwe.shangyingyoupin.top

[S35] C++：map
来源：http://boj.mhx1999.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://afa.yj202588.top

[S36] C++：unordered_map
来源：http://yte.sufxvd.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sgw.cheryme.top

[S37] C++：set
来源：http://ygb.gotoacloud.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sqf.cheryme.top

[S38] C++：排序
来源：http://sgs.hnqzz.top

std::sort(v.begin(), v.end());
来源：http://wzj.jqgufenzy.top

[S39] C++：自定义比较器排序
来源：http://qgg.mhx1999.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wao.yuxming.cn

[S40] C++：查找元素
来源：http://zuk.sysykeji.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xme.zhongyouzk.top

[S41] C++：类与构造函数
来源：http://vpk.jqgfzy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bjf.aizwys.cn

[S42] C++：继承与虚函数
来源：http://ast.uphjek.com

class B : public Base { public: void f() override {} };
来源：http://ggx.jyoumei.cn

[S43] C++：智能指针
来源：http://ngv.fzhhl.top

auto p = std::make_unique<int>(5);
来源：http://asr.sysykeji.top

[S44] C++：引用传参
来源：http://acx.chenjidiqi.icu

void inc(int &x) { ++x; }
来源：http://clb.feifeiyinyue.top

[S45] C++：lambda
来源：http://gmu.yuanzhike.top

auto add = [](int a, int b) { return a + b; };
来源：http://jmj.fzhhl.top

[S46] C++：函数模板
来源：http://zba.xinyue.icu

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zcc.jqgufenzy.top

[S47] C++：结构化绑定遍历
来源：http://aae.xziqi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ixf.ywan-chungtsiang.top

[S48] C++：逐行读文件
来源：http://dtm.shanyushiyangkeji.top

std::ifstream in("a.txt");  std::string line;
来源：http://spe.daria6918.cn

while (std::getline(in, line)) { }
来源：http://duz.jiagoushi.top

[S49] C++：写文件
来源：http://fcu.yj20258888.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zbe.ywan-chungtsiang.top

[S50] C++：格式化数字
来源：http://wde.nanxinkj.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wmv.daxiang520.top

[S51] C++：显式类型转换
来源：http://jit.zdbjq.cn

static_cast<double>(a) / b
来源：http://jwt.epnwcf.com

[S52] C++：const 与 noexcept
来源：http://xdf.xinyue.icu

int size() const noexcept { return n_; }
来源：http://tkg.zhengqikj.top

[S53] C++：移动语义
来源：http://trm.vehdjk.com

std::vector<int> w = std::move(v);
来源：http://zet.fanxiaobao.xyz

[S54] C++：异常处理
来源：http://jmr.fanxiaobao.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://exb.cheryme.top

[S55] C++：结构化绑定
来源：http://ydf.ehwqpu.com

auto [a, b] = std::make_pair(1, 2);
来源：http://ols.zhijiandao.cn

[S56] C++：optional
来源：http://zda.chenjidiqi.icu

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jtp.tarul.cn

[S57] C++：编译期常量
来源：http://kxs.dianchejie.cn

constexpr int N = 10;
来源：http://mbu.zhixingplan.top

[S58] C++：命名空间
来源：http://ziv.iojbl.cn

namespace ns { int f() { return 1; } }
来源：http://faq.yanxiufei.cn

[S59] C++：静态断言
来源：http://iig.wangdashe.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yka.fehbvm.com

[S60] C++：遍历并删除元素
来源：http://mzp.guowangkeji.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bxm.snrcjt.cn

================================================================================
来源：http://amk.aizwys.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bxa.snrcjt.cn

================================================================================
来源：http://ytd.jinqigfzy.top

[T01] Kotlin：Hello World
来源：http://nrx.jlsjyb.cn

println("Hello")
来源：http://irp.316326.xyz

[T02] Kotlin：变量
来源：http://glg.dashuyun.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pjy.hnqzz.top

[T03] Kotlin：字符串模板
来源：http://smh.zdqjudy.top

"值: $b"
来源：http://bun.mhx1999.top

[T04] Kotlin：空安全
来源：http://umd.fanxiaobao.xyz

val n: String? = null;  n?.length
来源：http://frt.yfazqb.com

[T05] Kotlin：when 表达式
来源：http://qij.wangdashe.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vns.iojbl.cn

[T06] Kotlin：集合映射
来源：http://auy.hammf.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://qmx.shzxlz.cn

[T07] Kotlin：集合过滤
来源：http://iep.yj20258.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://aza.hammf.cn

[T08] Kotlin：数据类
来源：http://tch.chenlongwang.top

data class User(val name: String, val age: Int)
来源：http://hbe.yonumen.top

[T09] Kotlin：扩展函数
来源：http://drx.jinghuilouyu.cn

fun String.exclaim() = this + "!"
来源：http://xye.gzhubu.top

[T10] Kotlin：默认参数
来源：http://ilm.jyoumei.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://owy.zhijiandao.cn

[T11] Kotlin：协程
来源：http://qic.hywenlv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wpd.ctjpmb.com

[T12] Kotlin：解构声明
来源：http://hww.cdnleiting.top

val (a, b) = Pair(1, 2)
来源：http://xcd.redwolf501.top

[T13] Kotlin：只读 Map
来源：http://wcz.cheryme.top

val m = mapOf("a" to 1)
来源：http://gzw.feifeiyinyue.top

[T14] Kotlin：循环
来源：http://hry.zhongyouzk.top

for (i in 1..10) println(i)
来源：http://nod.shanyushiyangtech.top

[T15] Kotlin：接口
来源：http://byg.tanke756.top

interface Shape { fun area(): Double }
来源：http://vnv.feifeiyinyue.top

[T16] Swift：Hello World
来源：http://aew.xziqi.cn

print("Hello")
来源：http://cfd.jqgufenzy.top

[T17] Swift：变量与常量
来源：http://lxa.tarul.cn

var a = 1;  let b = 2
来源：http://xdm.zhengqikj.top

[T18] Swift：字符串插值
来源：http://upt.guowangkeji.top

"值: \(b)"
来源：http://ohh.bjfxy.top

[T19] Swift：可选绑定
来源：http://eoj.hesvh.cn

if let n = opt { print(n) }
来源：http://val.zdqjudy.top

[T20] Swift：数组操作
来源：http://ict.zdbjq.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qdg.cucudq.cn

[T21] Swift：遍历
来源：http://bnq.316326.xyz

for x in a { print(x) }
来源：http://uzy.ywan-chungtsiang.top

[T22] Swift：字典
来源：http://hsf.kuanghao11.cn

var d = ["a": 1];  d["b"] = 2
来源：http://uoj.zhongyouzk.top

[T23] Swift：函数
来源：http://ylu.chenzaomai.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dqs.jlsjyb.cn

[T24] Swift：闭包
来源：http://dok.ehwqpu.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://bhu.daria6918.cn

[T25] Swift：结构体
来源：http://lfp.ydzc1.top

struct P { var x: Int }
来源：http://kzl.yueranfly.top

[T26] Swift：类与重写
来源：http://ouw.nanxinkj.top

class A: Base { override func f() {} }
来源：http://ell.ehwqpu.com

[T27] Swift：错误处理
来源：http://bnv.ydjk.org.cn

do { try f() } catch { print(error) }
来源：http://lku.cucudq.cn

[T28] Swift：枚举
来源：http://eqz.smart0.xyz

enum Color { case red, green }
来源：http://ube.snrcjt.cn

[T29] Swift：guard 提前返回
来源：http://dyn.9152youxi.cn

guard let x = opt else { return }
来源：http://yjv.cucudq.cn

[T30] Swift：协议
来源：http://kxq.bbcook.cn

protocol Shape { func area() -> Double }
来源：http://ufa.zhoulong.xyz

[T31] Lua：Hello World
来源：http://qzc.kuanghao11.cn

print("Hello")
来源：http://mim.fanxiaobao.xyz

[T32] Lua：局部变量
来源：http://myj.yfazqb.com

local a = 1
来源：http://sit.sweek.top

[T33] Lua：表（数组）
来源：http://xer.haohaochexian.top

local t = {1, 2, 3};  t[4] = 4
来源：http://piu.cdnleiting.top

[T34] Lua：遍历表
来源：http://qgx.nanxinkj.top

for i, v in ipairs(t) do print(i, v) end
来源：http://azu.hcnkem.com

[T35] Lua：字典表
来源：http://mix.shzxlz.cn

local d = { a = 1 };  d.b = 2
来源：http://gnl.nwbrower.top

[T36] Lua：函数
来源：http://wvr.hnqzz.top

function add(a, b) return a + b end
来源：http://agb.fktsv.cn

[T37] Lua：字符串拼接
来源：http://pza.uphjek.com

"a" .. "b"
来源：http://vot.smart0.xyz

[T38] Lua：条件
来源：http://xjk.bbcook.cn

if x > 0 then print("正") end
来源：http://xyj.gaohongyu789.top

[T39] Lua：模式匹配
来源：http://mqg.tarul.cn

string.find(s, "%d+")
来源：http://ngl.jinqigfzy.top

[T40] Lua：元表
来源：http://fid.cdnleiting.top

setmetatable({}, { __index = base })
来源：http://tkr.yj202588.top

[T41] Perl：Hello World
来源：http://gzv.dashuyun.cn

print "Hello\n";
来源：http://nnl.feifeiyinyue.top

[T42] Perl：变量类型
来源：http://twd.ppjwa.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cql.andypj.xyz

[T43] Perl：字符串插值
来源：http://sjt.haohaochexian.top

"值: $a"
来源：http://gyc.meibo888.top

[T44] Perl：条件
来源：http://zjy.fzhhl.top

if ($a > 0) { print "正"; }
来源：http://cfv.hnqzz.top

[T45] Perl：数组遍历
来源：http://ncx.yangfankeji.com

for my $x (@arr) { print $x; }
来源：http://pcc.sufxvd.cn

[T46] Perl：哈希操作
来源：http://iof.xziqi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pbp.shzxlz.cn

[T47] Perl：正则捕获
来源：http://rmf.nanxinkj.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://jhd.cdnleiting.top

[T48] Perl：正则替换
来源：http://nbs.dianchejie.cn

$s =~ s/old/new/g;
来源：http://axk.ywan-chungtsiang.top

[T49] Perl：函数
来源：http://cri.epnwcf.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://raq.zhongyouzk.top

[T50] Perl：逐行读文件
来源：http://zje.gotoacloud.top

open my $fh, "<", "a.txt" or die $!;
来源：http://pso.jlsjyb.cn

while (my $line = <$fh>) { print $line; }
来源：http://qol.jqgufenzy.top

[T51] Scala：Hello World
来源：http://gjr.aizwys.cn

println("Hello")
来源：http://djp.yangfankeji.com

[T52] Scala：变量
来源：http://ato.sjlbkw.cn

val a = 1;  var b = 2
来源：http://jxi.aizwys.cn

[T53] Scala：字符串插值
来源：http://ord.52xcode.cn

s"值: $b"
来源：http://rkd.hysaishi.cn

[T54] Scala：集合映射
来源：http://cwo.xuanzx.com

List(1, 2, 3).map(_ * 2)
来源：http://aew.wangdashe.top

[T55] Scala：集合过滤
来源：http://aej.wangdashe.top

List(1, 2, 3).filter(_ > 1)
来源：http://thm.yj20258888.top

[T56] Scala：样例类
来源：http://mpr.ivvv.top

case class User(name: String, age: Int)
来源：http://koy.52xcode.cn

[T57] Scala：模式匹配
来源：http://olm.xziqi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://eep.dashuyun.cn

[T58] Scala：函数定义
来源：http://fiu.epnwcf.com

def add(a: Int, b: Int): Int = a + b
来源：http://wjw.meibo888.top

[T59] Scala：循环
来源：http://ggv.redwolf501.top

for (i <- 1 to 10) println(i)
来源：http://vye.zdqjudy.top

[T60] Scala：折叠
来源：http://cxg.sysykeji.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://sej.uphjek.com

================================================================================
来源：http://ohv.bbcook.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wka.52xcode.cn

================================================================================
来源：http://kyz.jiagoushi.top

[U01] Py：创建虚拟环境
来源：http://oym.52xcode.cn

python -m venv .venv && source .venv/bin/activate
来源：http://wjm.aibaodan.cn

[U02] Py：导出 / 安装依赖
来源：http://xxu.smart0.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lnh.yonumen.top

[U03] Py：加载 .env 配置
来源：http://yal.gogol.net.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ttb.shanyushiyangtech.top

[U04] Py：变量调试打印
来源：http://usa.shuidangran.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pez.cdnleiting.top

[U05] Py：列表去重且保序
来源：http://vga.meibo888.top

list(dict.fromkeys(arr))
来源：http://ypb.shzxlz.cn

[U06] Py：合并两个字典
来源：http://hqq.wangdashe.top

{**a, **b}
来源：http://pwl.chenlongwang.top

[U07] Py：反转字典键值
来源：http://dmv.hongshengwenyu.top

{v: k for k, v in d.items()}
来源：http://vlr.bjfxy.top

[U08] Py：展平二维列表
来源：http://xfq.cheryme.top

[y for x in nested for y in x]
来源：http://kgl.zhiwuduotai.top

[U09] Py：字典取最大值的键
来源：http://dxy.snrcjt.cn

max(d, key=d.get)
来源：http://pny.kuanghao11.cn

[U10] Py：按值排序字典
来源：http://pnh.ydjk.org.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://akp.haohaochexian.top

[U11] Py：生成器表达式
来源：http://rio.pengpengdd.cyou

(x * 2 for x in arr)
来源：http://huz.fzhhl.top

[U12] Py：取出现最多的 3 个元素
来源：http://lxc.bjfxy.top

Counter(arr).most_common(3)
来源：http://sug.gogol.net.cn

[U13] Py：固定长度队列
来源：http://bby.cdnleiting.top

deque(maxlen=10)
来源：http://cwm.cucudq.cn

[U14] Py：分组收集到列表
来源：http://nbi.shuidangran.top

defaultdict(list)
来源：http://qyy.nwbrower.top

[U15] Py：高精度计时
来源：http://zvp.snrcjt.cn

t = time.perf_counter()
来源：http://pvc.jlsjyb.cn

[U16] Py：命令行参数解析
来源：http://kzy.shuidangran.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://iya.daria6918.cn

[U17] Py：初始化日志
来源：http://rgb.yueranfly.top

logging.basicConfig(level=logging.INFO)
来源：http://tnz.ehwqpu.com

[U18] Py：预编译正则
来源：http://nmd.mhx1999.top

pat = re.compile(r"\d+")
来源：http://wjc.xingfuxueyuan.xyz

[U19] Py：正则替换带回调
来源：http://nwf.quarkkingdee.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hnq.nwbrower.top

[U20] Py：缓存函数结果
来源：http://rdi.sufxvd.cn

@functools.lru_cache(maxsize=None)
来源：http://vwt.nanxinkj.top

[U21] Py：自定义上下文管理器
来源：http://yam.cqqwz.cn

@contextlib.contextmanager
来源：http://ycr.gogol.net.cn

[U22] Py：矩阵转置
来源：http://nef.gotoacloud.top

list(zip(*m))
来源：http://yuf.gogol.net.cn

[U23] Py：分块读取大文件
来源：http://oiw.fktsv.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://car.jinghuilouyu.cn

[U24] Py：路径操作
来源：http://xnz.uphjek.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://uie.guowangkeji.top

[U25] Py：CSV 按字典读
来源：http://ket.chenzaomai.com

csv.DictReader(f)
来源：http://hea.yj202588.top

[U26] Py：并发下载
来源：http://xqi.uphjek.com

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://htu.jiagoushi.top

[U27] Py：异步 HTTP
来源：http://mbp.ybcxt.top

aiohttp.ClientSession() 配合 async with
来源：http://rxe.pengpengdd.cyou

[U28] Py：类型别名
来源：http://sxt.vehdjk.com

UserId = int
来源：http://dza.sweek.top

[U29] Py：属性校验
来源：http://bcj.zhiwuduotai.top

@property 与 @x.setter 配合
来源：http://tuv.xylfe.cn

[U30] Py：数据类
来源：http://tdj.sxryk.cn

@dataclass(slots=True)
来源：http://tbv.tanke756.top

[U31] Py：单测
来源：http://vaa.wangshuangyany.cn

python -m pytest -q
来源：http://bht.sufxvd.cn

[U32] Py：代码格式化
来源：http://ldo.yj20258888.top

ruff format . && ruff check --fix .
来源：http://kcy.ywan-chungtsiang.top

[U33] Py：打包发布
来源：http://kir.zdbjq.cn

python -m build  （依赖 pyproject.toml）
来源：http://blm.hywenlv.cn

[U34] Py：判断编码
来源：http://vrl.mhx1999.top

chardet.detect(raw)
来源：http://fct.mhx1999.top

[U35] Py：发送邮件
来源：http://gju.nwbrower.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://oee.xziqi.cn

[U36] Py：定时任务
来源：http://pea.jqgfzy.top

schedule.every(10).minutes.do(job)
来源：http://zxm.daria6918.cn

[U37] Py：读写 Excel
来源：http://dyq.hammf.cn

pandas.read_excel / DataFrame.to_excel
来源：http://pgy.sxryk.cn

[U38] Py：获取脚本所在目录
来源：http://ecn.gzhubu.top

Path(__file__).resolve().parent
来源：http://cyi.sxryk.cn

[U39] Py：判断是否在交互环境
来源：http://rco.havefunace.top

sys.stdout.isatty()
来源：http://vjz.xuanzx.com

[U40] Py：打印到标准错误
来源：http://mgp.yvedp.cn

print("err", file=sys.stderr)
来源：http://ehi.yuanzhike.top

[U41] PHP：初始化 Composer 项目
来源：http://bmg.hysaishi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://wma.shanyushiyangtech.top

[U42] PHP：PSR-4 自动加载
来源：http://vrg.gotoacloud.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gkr.shzxlz.cn

[U43] PHP：声明命名空间
来源：http://swk.zdbjq.cn

namespace App\Http;
来源：http://tfn.smart0.xyz

[U44] PHP：开启严格类型
来源：http://tuv.shuidangran.top

declare(strict_types=1);
来源：http://hzd.cucudq.cn

[U45] PHP：类型声明与返回类型
来源：http://zmx.pengpengdd.cyou

function add(int $a, int $b): int { return $a + $b; }
来源：http://tmw.jianghu66.top

[U46] PHP：可空类型
来源：http://mdr.nanxuanxn.top

?string $name = null
来源：http://dyi.fzhhl.top

[U47] PHP：联合类型
来源：http://ujf.jqgufenzy.top

int|string $id
来源：http://oxr.sufxvd.cn

[U48] PHP：纯枚举
来源：http://tes.redwolf501.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cnc.9152youxi.cn

[U49] PHP：只读属性
来源：http://xzn.tian-w.cn

public readonly string $name
来源：http://hho.zhiwuduotai.top

[U50] PHP：构造器属性提升
来源：http://ngl.sweek.top

public function __construct(private int $id) {}
来源：http://sot.tarul.cn

[U51] PHP：数组解构
来源：http://ict.guowangkeji.top

[$a, $b] = $arr;
来源：http://qif.kuanghao11.cn

[U52] PHP：箭头函数
来源：http://qrp.yongpay.top

$double = fn($x) => $x * 2;
来源：http://ogk.jianghu66.top


<!-- 参考信息 -->