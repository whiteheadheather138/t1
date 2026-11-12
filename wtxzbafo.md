代发 wailian999

memset(a, 0, sizeof a);
来源：http://asn.bjfxy.top

[S27] C：定义常量
来源：http://weg.bbcook.cn

const double PI = 3.14159;
来源：http://hnj.ywan-chungtsiang.top

[S28] C：静态变量
来源：http://fdn.nanxinkj.top

static int counter = 0;
来源：http://snx.fktsv.cn

[S29] C：变参函数
来源：http://jtj.sysykeji.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jqf.yuanzhike.top

[S30] C：头文件保护
来源：http://die.fzhhl.top

#ifndef X_H
来源：http://nnt.fehbvm.com

#define X_H
来源：http://oci.xingfuxueyuan.xyz

#endif
来源：http://mww.guannengcc.top

[S31] C++：Hello World
来源：http://ipp.kuanghao11.cn

#include <iostream>
来源：http://sno.yj202588.top

int main() { std::cout << "Hello\n"; }
来源：http://bkt.gotoacloud.top

[S32] C++：字符串
来源：http://epv.52xcode.cn

std::string s = "hi";  s += "!";
来源：http://mpy.jlsjyb.cn

[S33] C++：vector 增删
来源：http://inb.tanke756.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://btb.yvedp.cn

[S34] C++：遍历 vector
来源：http://iqm.aizwys.cn

for (auto &x : v) { std::cout << x; }
来源：http://hrn.pycfn.com

[S35] C++：map
来源：http://yrl.smart0.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hzi.sysykeji.top

[S36] C++：unordered_map
来源：http://iee.jyoumei.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bia.jinghuilouyu.cn

[S37] C++：set
来源：http://ixv.fanxiaobao.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://avl.yuxming.cn

[S38] C++：排序
来源：http://xle.daria6918.cn

std::sort(v.begin(), v.end());
来源：http://uyg.ydjk.org.cn

[S39] C++：自定义比较器排序
来源：http://rdy.fzhhl.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://suj.yangfankeji.com

[S40] C++：查找元素
来源：http://zxl.havefunace.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://grq.jinqigufen.top

[S41] C++：类与构造函数
来源：http://zcy.shangyingyoupin.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ifl.yangfankeji.com

[S42] C++：继承与虚函数
来源：http://nqo.aibaodan.cn

class B : public Base { public: void f() override {} };
来源：http://jjo.gotoacloud.top

[S43] C++：智能指针
来源：http://efy.shanyushiyangkeji.top

auto p = std::make_unique<int>(5);
来源：http://rhk.jyoumei.cn

[S44] C++：引用传参
来源：http://sdm.fzhhl.top

void inc(int &x) { ++x; }
来源：http://mfj.yuxming.cn

[S45] C++：lambda
来源：http://raf.uphjek.com

auto add = [](int a, int b) { return a + b; };
来源：http://dog.chenjidiqi.icu

[S46] C++：函数模板
来源：http://tdz.fzhhl.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zas.sysykeji.top

[S47] C++：结构化绑定遍历
来源：http://ahx.zhoulong.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ttj.havefunace.top

[S48] C++：逐行读文件
来源：http://dvg.gotoacloud.top

std::ifstream in("a.txt");  std::string line;
来源：http://orv.yongpay.top

while (std::getline(in, line)) { }
来源：http://kpt.tian-w.cn

[S49] C++：写文件
来源：http://agb.yfazqb.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bvj.jqgufenzy.top

[S50] C++：格式化数字
来源：http://saa.shanyushiyangkeji.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sii.gaohongyu789.top

[S51] C++：显式类型转换
来源：http://vla.hammf.cn

static_cast<double>(a) / b
来源：http://kda.fanxiaobao.xyz

[S52] C++：const 与 noexcept
来源：http://xun.zhengqikj.top

int size() const noexcept { return n_; }
来源：http://ylq.hesvh.cn

[S53] C++：移动语义
来源：http://zrl.shuidangran.top

std::vector<int> w = std::move(v);
来源：http://ryq.fktsv.cn

[S54] C++：异常处理
来源：http://kgy.cheryme.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zum.zhengqikj.top

[S55] C++：结构化绑定
来源：http://puq.dianchejie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ydx.hcnkem.com

[S56] C++：optional
来源：http://ntr.epnwcf.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://giv.jqgufenzy.top

[S57] C++：编译期常量
来源：http://ouh.ywan-chungtsiang.top

constexpr int N = 10;
来源：http://ugu.xingfuxueyuan.xyz

[S58] C++：命名空间
来源：http://gps.nanxinkj.top

namespace ns { int f() { return 1; } }
来源：http://rod.aibaodan.cn

[S59] C++：静态断言
来源：http://zie.ivvv.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mew.yuanzhike.top

[S60] C++：遍历并删除元素
来源：http://lmk.cheryme.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gbp.hnxiangtu.top

================================================================================
来源：http://pkh.tian-w.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gzb.yangfankeji.com

================================================================================
来源：http://ayr.ydjk.org.cn

[T01] Kotlin：Hello World
来源：http://git.hammf.cn

println("Hello")
来源：http://epk.fzhhl.top

[T02] Kotlin：变量
来源：http://ica.jiagoushi.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wue.mhx1999.top

[T03] Kotlin：字符串模板
来源：http://nkt.ehwqpu.com

"值: $b"
来源：http://muy.shanyushiyangtech.top

[T04] Kotlin：空安全
来源：http://sod.zhoulong.xyz

val n: String? = null;  n?.length
来源：http://zyw.shuidangran.top

[T05] Kotlin：when 表达式
来源：http://ger.hysaishi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cix.vqdsnc.cn

[T06] Kotlin：集合映射
来源：http://gvh.0kj1m.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://dbb.cheryme.top

[T07] Kotlin：集合过滤
来源：http://euu.smart0.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://evm.andypj.xyz

[T08] Kotlin：数据类
来源：http://bku.zhoulong.xyz

data class User(val name: String, val age: Int)
来源：http://dbj.redwolf501.top

[T09] Kotlin：扩展函数
来源：http://noc.mhx1999.top

fun String.exclaim() = this + "!"
来源：http://zbn.c1oappe.top

[T10] Kotlin：默认参数
来源：http://nst.shuidangran.top

fun greet(name: String = "World") = "Hi $name"
来源：http://qcg.hesvh.cn

[T11] Kotlin：协程
来源：http://tfl.fzhhl.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ojn.daxiang520.top

[T12] Kotlin：解构声明
来源：http://dqj.0kj1m.cn

val (a, b) = Pair(1, 2)
来源：http://bxe.zdbjq.cn

[T13] Kotlin：只读 Map
来源：http://fnz.zhixingplan.top

val m = mapOf("a" to 1)
来源：http://iwp.redwolf501.top

[T14] Kotlin：循环
来源：http://iaw.snrcjt.cn

for (i in 1..10) println(i)
来源：http://hmq.xylfe.cn

[T15] Kotlin：接口
来源：http://myb.gogol.net.cn

interface Shape { fun area(): Double }
来源：http://rde.shzxlz.cn

[T16] Swift：Hello World
来源：http://mze.feifeiyinyue.top

print("Hello")
来源：http://fqx.ehwqpu.com

[T17] Swift：变量与常量
来源：http://dlk.wangdashe.top

var a = 1;  let b = 2
来源：http://ecb.vehdjk.com

[T18] Swift：字符串插值
来源：http://yme.hnqzz.top

"值: \(b)"
来源：http://krs.yj202588.top

[T19] Swift：可选绑定
来源：http://gyd.uphjek.com

if let n = opt { print(n) }
来源：http://rfc.ydjk.org.cn

[T20] Swift：数组操作
来源：http://ohp.nanxuanxn.top

var a = [1, 2, 3];  a.append(4)
来源：http://vhk.zdbjq.cn

[T21] Swift：遍历
来源：http://gdt.xinyue.icu

for x in a { print(x) }
来源：http://kbn.haohaochexian.top

[T22] Swift：字典
来源：http://iwt.pengpengdd.cyou

var d = ["a": 1];  d["b"] = 2
来源：http://vkd.jinyuanbaomall.cn

[T23] Swift：函数
来源：http://jex.yueranfly.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tgz.dashuyun.cn

[T24] Swift：闭包
来源：http://ttq.jqgfzy.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://qnp.guannengcc.top

[T25] Swift：结构体
来源：http://vpt.nanxuanxn.top

struct P { var x: Int }
来源：http://xeo.ehwqpu.com

[T26] Swift：类与重写
来源：http://xkw.svipenyu.cn

class A: Base { override func f() {} }
来源：http://sxq.9152youxi.cn

[T27] Swift：错误处理
来源：http://emt.nanxinkj.top

do { try f() } catch { print(error) }
来源：http://cqm.chenzaomai.com

[T28] Swift：枚举
来源：http://vlx.feifeiyinyue.top

enum Color { case red, green }
来源：http://lmi.fktsv.cn

[T29] Swift：guard 提前返回
来源：http://uwz.zhaomingkeji.xyz

guard let x = opt else { return }
来源：http://tyb.snrcjt.cn

[T30] Swift：协议
来源：http://kyh.iojbl.cn

protocol Shape { func area() -> Double }
来源：http://rdp.jianghu66.top

[T31] Lua：Hello World
来源：http://icy.aibaodan.cn

print("Hello")
来源：http://oaf.feifeiyinyue.top

[T32] Lua：局部变量
来源：http://bow.yonumen.top

local a = 1
来源：http://kmp.tian-w.cn

[T33] Lua：表（数组）
来源：http://hcy.ivvv.top

local t = {1, 2, 3};  t[4] = 4
来源：http://xuj.nanxinkj.top

[T34] Lua：遍历表
来源：http://vce.yj20258.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ops.ywan-chungtsiang.top

[T35] Lua：字典表
来源：http://xph.hfpthk.cn

local d = { a = 1 };  d.b = 2
来源：http://jdg.vehdjk.com

[T36] Lua：函数
来源：http://hkb.fengsongda.top

function add(a, b) return a + b end
来源：http://mhq.jiagoushi.top

[T37] Lua：字符串拼接
来源：http://zwg.fengsongda.top

"a" .. "b"
来源：http://puv.xinyue.icu

[T38] Lua：条件
来源：http://atn.jiagoushi.top

if x > 0 then print("正") end
来源：http://jni.vqdsnc.cn

[T39] Lua：模式匹配
来源：http://xni.zhaomingkeji.xyz

string.find(s, "%d+")
来源：http://mnr.jyoumei.cn

[T40] Lua：元表
来源：http://xhf.52xcode.cn

setmetatable({}, { __index = base })
来源：http://cns.ybcxt.top

[T41] Perl：Hello World
来源：http://nze.epnwcf.com

print "Hello\n";
来源：http://dvv.hywenlv.cn

[T42] Perl：变量类型
来源：http://dnv.hesvh.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hsh.hysaishi.cn

[T43] Perl：字符串插值
来源：http://abi.jqgfzy.top

"值: $a"
来源：http://xzg.cucudq.cn

[T44] Perl：条件
来源：http://aut.xuanzx.com

if ($a > 0) { print "正"; }
来源：http://enl.sjlbkw.cn

[T45] Perl：数组遍历
来源：http://eke.redwolf501.top

for my $x (@arr) { print $x; }
来源：http://nby.tianlin.xyz

[T46] Perl：哈希操作
来源：http://vmw.xuetiantiany.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mrt.dashuyun.cn

[T47] Perl：正则捕获
来源：http://qni.yj20258888.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://tgx.gotoacloud.top

[T48] Perl：正则替换
来源：http://ehi.tian-w.cn

$s =~ s/old/new/g;
来源：http://aaf.ywan-chungtsiang.top

[T49] Perl：函数
来源：http://veu.cdnleiting.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tgu.jianghu66.top

[T50] Perl：逐行读文件
来源：http://mzb.aizwys.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://alg.ctjpmb.com

while (my $line = <$fh>) { print $line; }
来源：http://aly.yj20258.top

[T51] Scala：Hello World
来源：http://weu.zhixingplan.top

println("Hello")
来源：http://hnz.gzhubu.top

[T52] Scala：变量
来源：http://fpm.zdbjq.cn

val a = 1;  var b = 2
来源：http://czd.yanxiufei.cn

[T53] Scala：字符串插值
来源：http://tor.hesvh.cn

s"值: $b"
来源：http://czy.quarkkingdee.top

[T54] Scala：集合映射
来源：http://phl.ywan-chungtsiang.top

List(1, 2, 3).map(_ * 2)
来源：http://poc.shuidangran.top

[T55] Scala：集合过滤
来源：http://wpw.yanxiufei.cn

List(1, 2, 3).filter(_ > 1)
来源：http://iil.hesvh.cn

[T56] Scala：样例类
来源：http://scm.tian-w.cn

case class User(name: String, age: Int)
来源：http://umu.iojbl.cn

[T57] Scala：模式匹配
来源：http://aob.zhixingplan.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://kny.nanxuanxn.top

[T58] Scala：函数定义
来源：http://lao.52xcode.cn

def add(a: Int, b: Int): Int = a + b
来源：http://fwv.tanke756.top

[T59] Scala：循环
来源：http://ast.havefunace.top

for (i <- 1 to 10) println(i)
来源：http://jrd.zhiwuduotai.top

[T60] Scala：折叠
来源：http://pyw.hongshengwenyu.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hwj.zdqjudy.top

================================================================================
来源：http://ker.redwolf501.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xef.pycfn.com

================================================================================
来源：http://evb.hnxiangtu.top

[U01] Py：创建虚拟环境
来源：http://kfn.haohaochexian.top

python -m venv .venv && source .venv/bin/activate
来源：http://fhf.jinghuilouyu.cn

[U02] Py：导出 / 安装依赖
来源：http://hqo.nanxuanxn.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zqj.havefunace.top

[U03] Py：加载 .env 配置
来源：http://gjp.sufxvd.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rri.mhx1999.top

[U04] Py：变量调试打印
来源：http://fvg.nanxuanxn.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://evt.zdbjq.cn

[U05] Py：列表去重且保序
来源：http://ecj.zhaomingkeji.xyz

list(dict.fromkeys(arr))
来源：http://rvu.jinqigfzy.top

[U06] Py：合并两个字典
来源：http://noh.uphjek.com

{**a, **b}
来源：http://gjd.jinqigfzy.top

[U07] Py：反转字典键值
来源：http://gqn.aizwys.cn

{v: k for k, v in d.items()}
来源：http://iny.daxiang520.top

[U08] Py：展平二维列表
来源：http://yfl.bbcook.cn

[y for x in nested for y in x]
来源：http://gxp.ydjk.org.cn

[U09] Py：字典取最大值的键
来源：http://mfr.wangshuangyany.cn

max(d, key=d.get)
来源：http://jlw.zhoulong.xyz

[U10] Py：按值排序字典
来源：http://bqn.xinyue.icu

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zcg.zdbjq.cn

[U11] Py：生成器表达式
来源：http://uic.ehwqpu.com

(x * 2 for x in arr)
来源：http://atd.0kj1m.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ufk.daria6918.cn

Counter(arr).most_common(3)
来源：http://suc.jinqigfzy.top

[U13] Py：固定长度队列
来源：http://mjy.jinqigfzy.top

deque(maxlen=10)
来源：http://kgc.quarkkingdee.top

[U14] Py：分组收集到列表
来源：http://avz.sxryk.cn

defaultdict(list)
来源：http://ycc.guannengcc.top

[U15] Py：高精度计时
来源：http://sqq.0kj1m.cn

t = time.perf_counter()
来源：http://gyb.daxiang520.top

[U16] Py：命令行参数解析
来源：http://nfb.yuanzhike.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://soc.yuxming.cn

[U17] Py：初始化日志
来源：http://ekt.jianghu66.top

logging.basicConfig(level=logging.INFO)
来源：http://uxr.sjlbkw.cn

[U18] Py：预编译正则
来源：http://hfj.yvedp.cn

pat = re.compile(r"\d+")
来源：http://zsm.zhijiandao.cn

[U19] Py：正则替换带回调
来源：http://otr.wangshuangyany.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xzp.zhongyouzk.top

[U20] Py：缓存函数结果
来源：http://ajz.pycfn.com

@functools.lru_cache(maxsize=None)
来源：http://frf.zhiwuduotai.top

[U21] Py：自定义上下文管理器
来源：http://tbx.chenzaomai.com

@contextlib.contextmanager
来源：http://wmz.ehwqpu.com

[U22] Py：矩阵转置
来源：http://oud.cqqwz.cn

list(zip(*m))
来源：http://kyk.nwbrower.top

[U23] Py：分块读取大文件
来源：http://fkl.uphjek.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://whh.nwbrower.top

[U24] Py：路径操作
来源：http://vuz.jqgufenzy.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://azu.aibaodan.cn

[U25] Py：CSV 按字典读
来源：http://stg.andypj.xyz

csv.DictReader(f)
来源：http://djd.xuanzx.com

[U26] Py：并发下载
来源：http://myj.chenlongwang.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://evl.sysykeji.top

[U27] Py：异步 HTTP
来源：http://hci.fzhhl.top

aiohttp.ClientSession() 配合 async with
来源：http://fyt.jqgfzy.top

[U28] Py：类型别名
来源：http://nrr.ybcxt.top

UserId = int
来源：http://eem.birdmap.top

[U29] Py：属性校验
来源：http://aeb.ppjwa.cn

@property 与 @x.setter 配合
来源：http://hme.hysaishi.cn

[U30] Py：数据类
来源：http://okx.jqgufenzy.top

@dataclass(slots=True)
来源：http://jqy.zhixingplan.top

[U31] Py：单测
来源：http://gjt.zdqjudy.top

python -m pytest -q
来源：http://byx.feifeiyinyue.top

[U32] Py：代码格式化
来源：http://bjy.ywan-chungtsiang.top

ruff format . && ruff check --fix .
来源：http://jdb.xingfuxueyuan.xyz

[U33] Py：打包发布
来源：http://ahk.guowangkeji.top

python -m build  （依赖 pyproject.toml）
来源：http://eip.feifeiyinyue.top

[U34] Py：判断编码
来源：http://rbt.mhx1999.top

chardet.detect(raw)
来源：http://moz.aizwys.cn

[U35] Py：发送邮件
来源：http://acg.wangdashe.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://kjc.hongshengwenyu.top

[U36] Py：定时任务
来源：http://ofh.xylfe.cn

schedule.every(10).minutes.do(job)
来源：http://vns.guowangkeji.top

[U37] Py：读写 Excel
来源：http://zaq.dianchejie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://fzt.snrcjt.cn

[U38] Py：获取脚本所在目录
来源：http://fof.andypj.xyz

Path(__file__).resolve().parent
来源：http://mlj.sxryk.cn

[U39] Py：判断是否在交互环境
来源：http://mvs.hnxiangtu.top

sys.stdout.isatty()
来源：http://wwe.hesvh.cn

[U40] Py：打印到标准错误
来源：http://jbx.zhixingplan.top

print("err", file=sys.stderr)
来源：http://ysb.andypj.xyz

[U41] PHP：初始化 Composer 项目
来源：http://xdm.zhaomingkeji.xyz

composer init;  composer require guzzlehttp/guzzle
来源：http://jta.vehdjk.com

[U42] PHP：PSR-4 自动加载
来源：http://ilh.hnqzz.top

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://asc.yonumen.top

[U43] PHP：声明命名空间
来源：http://imq.tian-w.cn

namespace App\Http;
来源：http://goa.iojbl.cn

[U44] PHP：开启严格类型
来源：http://rqe.sjlbkw.cn

declare(strict_types=1);
来源：http://skr.yangfankeji.com

[U45] PHP：类型声明与返回类型
来源：http://hgi.hnxiangtu.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://ywc.haohaochexian.top

[U46] PHP：可空类型
来源：http://pau.fzhhl.top

?string $name = null
来源：http://tfj.ppjwa.cn

[U47] PHP：联合类型
来源：http://qgz.yj20258888.top

int|string $id
来源：http://xae.jianghu66.top

[U48] PHP：纯枚举
来源：http://xjb.yj20258.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nkt.0kj1m.cn

[U49] PHP：只读属性
来源：http://ldu.dashuyun.cn

public readonly string $name
来源：http://wxt.guannengcc.top

[U50] PHP：构造器属性提升
来源：http://kek.andypj.xyz

public function __construct(private int $id) {}
来源：http://yda.feifeiyinyue.top


<!-- 参考信息 -->