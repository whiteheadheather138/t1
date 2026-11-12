代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rzg.xuanzx.com

[S25] C：内存拷贝
来源：http://iea.yj202588.top

memcpy(dst, src, n);
来源：http://xfc.jianghu66.top

[S26] C：内存清零
来源：http://pad.sjlbkw.cn

memset(a, 0, sizeof a);
来源：http://tie.cdnleiting.top

[S27] C：定义常量
来源：http://sbi.daxiang520.top

const double PI = 3.14159;
来源：http://ueu.xuetiantiany.cn

[S28] C：静态变量
来源：http://bri.shanyushiyangtech.top

static int counter = 0;
来源：http://xlh.yj202588.top

[S29] C：变参函数
来源：http://uri.pycfn.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://brp.yj202588.top

[S30] C：头文件保护
来源：http://bae.fzhhl.top

#ifndef X_H
来源：http://hay.zhongyouzk.top

#define X_H
来源：http://abl.zdbjq.cn

#endif
来源：http://qdr.hnqzz.top

[S31] C++：Hello World
来源：http://yay.hfpthk.cn

#include <iostream>
来源：http://uzw.zhijiandao.cn

int main() { std::cout << "Hello\n"; }
来源：http://flj.ywan-chungtsiang.top

[S32] C++：字符串
来源：http://vix.nanxuanxn.top

std::string s = "hi";  s += "!";
来源：http://hed.xuanzx.com

[S33] C++：vector 增删
来源：http://mrr.xuanzx.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jan.yuxming.cn

[S34] C++：遍历 vector
来源：http://pdq.cheryme.top

for (auto &x : v) { std::cout << x; }
来源：http://rej.pycfn.com

[S35] C++：map
来源：http://tsx.zdbjq.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://orm.yfazqb.com

[S36] C++：unordered_map
来源：http://tdi.xinyue.icu

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://djg.sxryk.cn

[S37] C++：set
来源：http://cdz.jiagoushi.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fks.ywan-chungtsiang.top

[S38] C++：排序
来源：http://vip.birdmap.top

std::sort(v.begin(), v.end());
来源：http://boc.sjlbkw.cn

[S39] C++：自定义比较器排序
来源：http://ngh.zhiwuduotai.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gjk.vqdsnc.cn

[S40] C++：查找元素
来源：http://kid.tanke756.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bov.zhongyouzk.top

[S41] C++：类与构造函数
来源：http://pwi.dashuyun.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yvl.yvedp.cn

[S42] C++：继承与虚函数
来源：http://cta.redwolf501.top

class B : public Base { public: void f() override {} };
来源：http://wgp.zhixingplan.top

[S43] C++：智能指针
来源：http://uji.xuanzx.com

auto p = std::make_unique<int>(5);
来源：http://juh.shangyingyoupin.top

[S44] C++：引用传参
来源：http://fop.ydjk.org.cn

void inc(int &x) { ++x; }
来源：http://fry.zhengqikj.top

[S45] C++：lambda
来源：http://mve.cqqwz.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ciw.cheryme.top

[S46] C++：函数模板
来源：http://efy.52xcode.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bik.birdmap.top

[S47] C++：结构化绑定遍历
来源：http://prp.hywenlv.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nok.quarkkingdee.top

[S48] C++：逐行读文件
来源：http://jsq.xingfuxueyuan.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://zlj.jianghu66.top

while (std::getline(in, line)) { }
来源：http://drr.tanke756.top

[S49] C++：写文件
来源：http://wiy.fengsongda.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://iqq.zdqjudy.top

[S50] C++：格式化数字
来源：http://exr.jinqigfzy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://iyo.yongpay.top

[S51] C++：显式类型转换
来源：http://aoz.gotoacloud.top

static_cast<double>(a) / b
来源：http://kwk.fehbvm.com

[S52] C++：const 与 noexcept
来源：http://sqh.hfpthk.cn

int size() const noexcept { return n_; }
来源：http://yqf.xinyue.icu

[S53] C++：移动语义
来源：http://kly.birdmap.top

std::vector<int> w = std::move(v);
来源：http://taw.chenlongwang.top

[S54] C++：异常处理
来源：http://oda.zdbjq.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cuw.epnwcf.com

[S55] C++：结构化绑定
来源：http://hjx.jqgfzy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://dyd.tanke756.top

[S56] C++：optional
来源：http://hxy.xziqi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yuc.sufxvd.cn

[S57] C++：编译期常量
来源：http://joh.tianlin.xyz

constexpr int N = 10;
来源：http://sky.meibo888.top

[S58] C++：命名空间
来源：http://yad.zhiwuduotai.top

namespace ns { int f() { return 1; } }
来源：http://swt.cqqwz.cn

[S59] C++：静态断言
来源：http://vfo.tianlin.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uvg.jinyuanbaomall.cn

[S60] C++：遍历并删除元素
来源：http://jqd.daxiang520.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bmd.hysaishi.cn

================================================================================
来源：http://hcw.jianghu66.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gab.daxiang520.top

================================================================================
来源：http://nqk.fzhhl.top

[T01] Kotlin：Hello World
来源：http://wfq.meibo888.top

println("Hello")
来源：http://vsg.ydjk.org.cn

[T02] Kotlin：变量
来源：http://eux.yuxming.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://woa.zhaomingkeji.xyz

[T03] Kotlin：字符串模板
来源：http://scc.xingfuxueyuan.xyz

"值: $b"
来源：http://nit.aizwys.cn

[T04] Kotlin：空安全
来源：http://ldr.sufxvd.cn

val n: String? = null;  n?.length
来源：http://onw.shangyingyoupin.top

[T05] Kotlin：when 表达式
来源：http://pfw.ywan-chungtsiang.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rdf.birdmap.top

[T06] Kotlin：集合映射
来源：http://jzq.hfpthk.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://uqa.ppjwa.cn

[T07] Kotlin：集合过滤
来源：http://abf.aibaodan.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://lut.hfpthk.cn

[T08] Kotlin：数据类
来源：http://qmq.tarul.cn

data class User(val name: String, val age: Int)
来源：http://mth.hnqzz.top

[T09] Kotlin：扩展函数
来源：http://vuf.yuanzhike.top

fun String.exclaim() = this + "!"
来源：http://cfx.hywenlv.cn

[T10] Kotlin：默认参数
来源：http://cso.aizwys.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://fkk.haohaochexian.top

[T11] Kotlin：协程
来源：http://swn.zycfv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://isr.xuanzx.com

[T12] Kotlin：解构声明
来源：http://rna.vehdjk.com

val (a, b) = Pair(1, 2)
来源：http://vxc.fktsv.cn

[T13] Kotlin：只读 Map
来源：http://qeg.sufxvd.cn

val m = mapOf("a" to 1)
来源：http://jrl.uphjek.com

[T14] Kotlin：循环
来源：http://hrr.kuanghao11.cn

for (i in 1..10) println(i)
来源：http://nqu.zhengqikj.top

[T15] Kotlin：接口
来源：http://oqq.zhongyouzk.top

interface Shape { fun area(): Double }
来源：http://jne.yueranfly.top

[T16] Swift：Hello World
来源：http://bsv.nwbrower.top

print("Hello")
来源：http://gaz.xuanzx.com

[T17] Swift：变量与常量
来源：http://zoq.shanyushiyangtech.top

var a = 1;  let b = 2
来源：http://sbr.hcnkem.com

[T18] Swift：字符串插值
来源：http://pse.chenlongwang.top

"值: \(b)"
来源：http://own.smart0.xyz

[T19] Swift：可选绑定
来源：http://nqw.jyoumei.cn

if let n = opt { print(n) }
来源：http://crw.0kj1m.cn

[T20] Swift：数组操作
来源：http://upt.nwbrower.top

var a = [1, 2, 3];  a.append(4)
来源：http://wiq.xziqi.cn

[T21] Swift：遍历
来源：http://bxt.kuanghao11.cn

for x in a { print(x) }
来源：http://bqw.xziqi.cn

[T22] Swift：字典
来源：http://rcv.yj20258888.top

var d = ["a": 1];  d["b"] = 2
来源：http://trr.c1oappe.top

[T23] Swift：函数
来源：http://ssn.xinyue.icu

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gyq.yj20258.top

[T24] Swift：闭包
来源：http://jim.sysykeji.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://avy.dashuyun.cn

[T25] Swift：结构体
来源：http://dij.jinyuanbaomall.cn

struct P { var x: Int }
来源：http://vvw.sufxvd.cn

[T26] Swift：类与重写
来源：http://cwc.xziqi.cn

class A: Base { override func f() {} }
来源：http://sqt.shuidangran.top

[T27] Swift：错误处理
来源：http://pwl.xziqi.cn

do { try f() } catch { print(error) }
来源：http://zrm.xziqi.cn

[T28] Swift：枚举
来源：http://kic.hfpthk.cn

enum Color { case red, green }
来源：http://les.sxryk.cn

[T29] Swift：guard 提前返回
来源：http://dak.fehbvm.com

guard let x = opt else { return }
来源：http://kdi.jinqigufen.top

[T30] Swift：协议
来源：http://fer.jinqigfzy.top

protocol Shape { func area() -> Double }
来源：http://wwa.ivvv.top

[T31] Lua：Hello World
来源：http://ycl.yongpay.top

print("Hello")
来源：http://jph.uphjek.com

[T32] Lua：局部变量
来源：http://rtk.fehbvm.com

local a = 1
来源：http://mxp.316326.xyz

[T33] Lua：表（数组）
来源：http://lug.hcnkem.com

local t = {1, 2, 3};  t[4] = 4
来源：http://oic.smart0.xyz

[T34] Lua：遍历表
来源：http://cks.fengsongda.top

for i, v in ipairs(t) do print(i, v) end
来源：http://dax.hysaishi.cn

[T35] Lua：字典表
来源：http://iyw.cashguo.top

local d = { a = 1 };  d.b = 2
来源：http://uip.yvedp.cn

[T36] Lua：函数
来源：http://jby.jinghuilouyu.cn

function add(a, b) return a + b end
来源：http://ueq.jinqigfzy.top

[T37] Lua：字符串拼接
来源：http://lxu.ppjwa.cn

"a" .. "b"
来源：http://jxr.yuanzhike.top

[T38] Lua：条件
来源：http://gzo.shuidangran.top

if x > 0 then print("正") end
来源：http://qmz.zdbjq.cn

[T39] Lua：模式匹配
来源：http://pwt.feifeiyinyue.top

string.find(s, "%d+")
来源：http://lsc.sjlbkw.cn

[T40] Lua：元表
来源：http://tpb.jinghuilouyu.cn

setmetatable({}, { __index = base })
来源：http://ogs.bjfxy.top

[T41] Perl：Hello World
来源：http://ezy.tanke756.top

print "Hello\n";
来源：http://gvn.yj20258888.top

[T42] Perl：变量类型
来源：http://smm.xuetiantiany.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kzw.yj20258888.top

[T43] Perl：字符串插值
来源：http://bdz.yj202588.top

"值: $a"
来源：http://bkq.fehbvm.com

[T44] Perl：条件
来源：http://dcj.yuanzhike.top

if ($a > 0) { print "正"; }
来源：http://gym.yj20258.top

[T45] Perl：数组遍历
来源：http://vpo.jqgufenzy.top

for my $x (@arr) { print $x; }
来源：http://lmh.bjfxy.top

[T46] Perl：哈希操作
来源：http://sag.jinyuanbaomall.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bxa.bjfxy.top

[T47] Perl：正则捕获
来源：http://fae.yangfankeji.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://jqb.mhx1999.top

[T48] Perl：正则替换
来源：http://hll.pycfn.com

$s =~ s/old/new/g;
来源：http://ymg.fehbvm.com

[T49] Perl：函数
来源：http://inf.zhoulong.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vdm.hfpthk.cn

[T50] Perl：逐行读文件
来源：http://oss.ppjwa.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://sza.zhaomingkeji.xyz

while (my $line = <$fh>) { print $line; }
来源：http://szk.vqdsnc.cn

[T51] Scala：Hello World
来源：http://rey.zhoulong.xyz

println("Hello")
来源：http://eor.nanxinkj.top

[T52] Scala：变量
来源：http://kti.xuanzx.com

val a = 1;  var b = 2
来源：http://zwb.ywan-chungtsiang.top

[T53] Scala：字符串插值
来源：http://bsm.sjlbkw.cn

s"值: $b"
来源：http://zrz.bbcook.cn

[T54] Scala：集合映射
来源：http://sqe.dianchejie.cn

List(1, 2, 3).map(_ * 2)
来源：http://qwc.zycfv.cn

[T55] Scala：集合过滤
来源：http://zpt.hnqzz.top

List(1, 2, 3).filter(_ > 1)
来源：http://oex.gogol.net.cn

[T56] Scala：样例类
来源：http://xun.ydjk.org.cn

case class User(name: String, age: Int)
来源：http://jsc.kuanghao11.cn

[T57] Scala：模式匹配
来源：http://xee.zhiwuduotai.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://euq.birdmap.top

[T58] Scala：函数定义
来源：http://ene.hnxiangtu.top

def add(a: Int, b: Int): Int = a + b
来源：http://ctm.haohaochexian.top

[T59] Scala：循环
来源：http://jar.ivvv.top

for (i <- 1 to 10) println(i)
来源：http://qnh.vehdjk.com

[T60] Scala：折叠
来源：http://qdx.yj202588.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dff.hnxiangtu.top

================================================================================
来源：http://ykw.yuxming.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://miv.bbcook.cn

================================================================================
来源：http://vup.nanxinkj.top

[U01] Py：创建虚拟环境
来源：http://yxn.9152youxi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://wkd.zhixingplan.top

[U02] Py：导出 / 安装依赖
来源：http://tud.nwbrower.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gts.hammf.cn

[U03] Py：加载 .env 配置
来源：http://wxx.chenjidiqi.icu

from dotenv import load_dotenv; load_dotenv()
来源：http://ccr.chenzaomai.com

[U04] Py：变量调试打印
来源：http://jda.xuetiantiany.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://flc.shangyingyoupin.top

[U05] Py：列表去重且保序
来源：http://aza.hammf.cn

list(dict.fromkeys(arr))
来源：http://ycx.hnxiangtu.top

[U06] Py：合并两个字典
来源：http://fpc.birdmap.top

{**a, **b}
来源：http://xtc.tanke756.top

[U07] Py：反转字典键值
来源：http://xme.tanke756.top

{v: k for k, v in d.items()}
来源：http://fuq.jiagoushi.top

[U08] Py：展平二维列表
来源：http://abs.aibaodan.cn

[y for x in nested for y in x]
来源：http://rjk.9152youxi.cn

[U09] Py：字典取最大值的键
来源：http://nrd.hnqzz.top

max(d, key=d.get)
来源：http://ksb.c1oappe.top

[U10] Py：按值排序字典
来源：http://nkf.shuidangran.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uee.zhixingplan.top

[U11] Py：生成器表达式
来源：http://ush.zhoulong.xyz

(x * 2 for x in arr)
来源：http://kwp.fehbvm.com

[U12] Py：取出现最多的 3 个元素
来源：http://sac.vqdsnc.cn

Counter(arr).most_common(3)
来源：http://chv.yj20258888.top

[U13] Py：固定长度队列
来源：http://fkc.zhaomingkeji.xyz

deque(maxlen=10)
来源：http://aco.gogol.net.cn

[U14] Py：分组收集到列表
来源：http://kov.daria6918.cn

defaultdict(list)
来源：http://amr.sxryk.cn

[U15] Py：高精度计时
来源：http://uzq.pengpengdd.cyou

t = time.perf_counter()
来源：http://zif.jiagoushi.top

[U16] Py：命令行参数解析
来源：http://wkp.dashuyun.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://fqz.zhiwuduotai.top

[U17] Py：初始化日志
来源：http://wqp.yj202588.top

logging.basicConfig(level=logging.INFO)
来源：http://dpr.birdmap.top

[U18] Py：预编译正则
来源：http://qcg.bjfxy.top

pat = re.compile(r"\d+")
来源：http://hfu.tanke756.top

[U19] Py：正则替换带回调
来源：http://jpj.tarul.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ikl.shzxlz.cn

[U20] Py：缓存函数结果
来源：http://pdh.svipenyu.cn

@functools.lru_cache(maxsize=None)
来源：http://bzr.tarul.cn

[U21] Py：自定义上下文管理器
来源：http://ayq.bjfxy.top

@contextlib.contextmanager
来源：http://tfz.yangfankeji.com

[U22] Py：矩阵转置
来源：http://xvr.tanke756.top

list(zip(*m))
来源：http://cch.uphjek.com

[U23] Py：分块读取大文件
来源：http://nkc.cqqwz.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://cuu.mhx1999.top

[U24] Py：路径操作
来源：http://pnz.ivvv.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://eap.hesvh.cn

[U25] Py：CSV 按字典读
来源：http://qld.cheryme.top

csv.DictReader(f)
来源：http://pde.tian-w.cn

[U26] Py：并发下载
来源：http://wfs.hysaishi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hiw.yuxming.cn

[U27] Py：异步 HTTP
来源：http://bzx.andypj.xyz

aiohttp.ClientSession() 配合 async with
来源：http://oct.smart0.xyz

[U28] Py：类型别名
来源：http://gut.meibo888.top

UserId = int
来源：http://vyg.yvedp.cn

[U29] Py：属性校验
来源：http://rbm.jiagoushi.top

@property 与 @x.setter 配合
来源：http://yxg.fehbvm.com

[U30] Py：数据类
来源：http://xda.ehwqpu.com

@dataclass(slots=True)
来源：http://nsn.svipenyu.cn

[U31] Py：单测
来源：http://bxf.haohaochexian.top

python -m pytest -q
来源：http://qfq.ivvv.top

[U32] Py：代码格式化
来源：http://zqc.jqgfzy.top

ruff format . && ruff check --fix .
来源：http://jsm.dashuyun.cn

[U33] Py：打包发布
来源：http://ujq.smart0.xyz

python -m build  （依赖 pyproject.toml）
来源：http://ryc.xziqi.cn

[U34] Py：判断编码
来源：http://faw.ybcxt.top

chardet.detect(raw)
来源：http://vfa.jianghu66.top

[U35] Py：发送邮件
来源：http://hsi.316326.xyz

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://vzl.jlsjyb.cn

[U36] Py：定时任务
来源：http://zhy.dianchejie.cn

schedule.every(10).minutes.do(job)
来源：http://mqn.xziqi.cn

[U37] Py：读写 Excel
来源：http://vjg.smart0.xyz

pandas.read_excel / DataFrame.to_excel
来源：http://nit.pengpengdd.cyou

[U38] Py：获取脚本所在目录
来源：http://sgw.sxryk.cn

Path(__file__).resolve().parent
来源：http://gah.hywenlv.cn

[U39] Py：判断是否在交互环境
来源：http://uqf.aizwys.cn

sys.stdout.isatty()
来源：http://gom.jinghuilouyu.cn

[U40] Py：打印到标准错误
来源：http://woi.zdqjudy.top

print("err", file=sys.stderr)
来源：http://nrs.tanke756.top

[U41] PHP：初始化 Composer 项目
来源：http://uat.zdbjq.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://kyp.hesvh.cn

[U42] PHP：PSR-4 自动加载
来源：http://wea.0kj1m.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cks.hnxiangtu.top

[U43] PHP：声明命名空间
来源：http://nlk.hnqzz.top

namespace App\Http;
来源：http://pck.zhijiandao.cn

[U44] PHP：开启严格类型
来源：http://krj.ydjk.org.cn

declare(strict_types=1);
来源：http://eip.meibo888.top

[U45] PHP：类型声明与返回类型
来源：http://swf.chenlongwang.top

function add(int $a, int $b): int { return $a + $b; }
来源：http://oap.fktsv.cn

[U46] PHP：可空类型
来源：http://xnp.iojbl.cn

?string $name = null
来源：http://fxu.cdnleiting.top

[U47] PHP：联合类型
来源：http://tjr.feifeiyinyue.top

int|string $id
来源：http://ruh.hnxiangtu.top

[U48] PHP：纯枚举
来源：http://qom.havefunace.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jmq.ydjk.org.cn


<!-- 参考信息 -->