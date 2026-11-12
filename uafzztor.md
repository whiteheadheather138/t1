代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mdn.shanyushiyangkeji.top

[S25] C：内存拷贝
来源：http://bqw.316326.xyz

memcpy(dst, src, n);
来源：http://qjg.birdmap.top

[S26] C：内存清零
来源：http://hgc.sjlbkw.cn

memset(a, 0, sizeof a);
来源：http://aie.yangfankeji.com

[S27] C：定义常量
来源：http://hoe.shanyushiyangkeji.top

const double PI = 3.14159;
来源：http://vng.cashguo.top

[S28] C：静态变量
来源：http://dyi.jinqigfzy.top

static int counter = 0;
来源：http://bqg.ydjk.org.cn

[S29] C：变参函数
来源：http://mmh.jlsjyb.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hrz.dashuyun.cn

[S30] C：头文件保护
来源：http://qst.mhx1999.top

#ifndef X_H
来源：http://uty.guowangkeji.top

#define X_H
来源：http://bqf.zhijiandao.cn

#endif
来源：http://bhz.birdmap.top

[S31] C++：Hello World
来源：http://rxl.vqdsnc.cn

#include <iostream>
来源：http://lnw.aibaodan.cn

int main() { std::cout << "Hello\n"; }
来源：http://jyy.hcnkem.com

[S32] C++：字符串
来源：http://jfi.zhiwuduotai.top

std::string s = "hi";  s += "!";
来源：http://ram.tanke756.top

[S33] C++：vector 增删
来源：http://jbk.jianghu66.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vyq.gzhubu.top

[S34] C++：遍历 vector
来源：http://rcp.jqgfzy.top

for (auto &x : v) { std::cout << x; }
来源：http://kmz.vehdjk.com

[S35] C++：map
来源：http://dyb.hcnkem.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://apv.yanxiufei.cn

[S36] C++：unordered_map
来源：http://wpv.aizwys.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yoi.yvedp.cn

[S37] C++：set
来源：http://cwa.cucudq.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fah.snrcjt.cn

[S38] C++：排序
来源：http://slp.hysaishi.cn

std::sort(v.begin(), v.end());
来源：http://dxq.dashuyun.cn

[S39] C++：自定义比较器排序
来源：http://qxk.yfazqb.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qst.jinqigfzy.top

[S40] C++：查找元素
来源：http://sls.haohaochexian.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rss.smart0.xyz

[S41] C++：类与构造函数
来源：http://itu.fktsv.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rpq.zycfv.cn

[S42] C++：继承与虚函数
来源：http://ffp.gaohongyu789.top

class B : public Base { public: void f() override {} };
来源：http://ppr.hysaishi.cn

[S43] C++：智能指针
来源：http://tjy.meibo888.top

auto p = std::make_unique<int>(5);
来源：http://gcv.fehbvm.com

[S44] C++：引用传参
来源：http://ghe.daria6918.cn

void inc(int &x) { ++x; }
来源：http://hrj.daria6918.cn

[S45] C++：lambda
来源：http://bpa.andypj.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://jjd.ppjwa.cn

[S46] C++：函数模板
来源：http://jkl.daria6918.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gzg.shuidangran.top

[S47] C++：结构化绑定遍历
来源：http://hwa.cdnleiting.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://her.jqgufenzy.top

[S48] C++：逐行读文件
来源：http://fxq.andypj.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://hrb.guowangkeji.top

while (std::getline(in, line)) { }
来源：http://zod.ydzc1.top

[S49] C++：写文件
来源：http://stm.sxryk.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qsg.tianlin.xyz

[S50] C++：格式化数字
来源：http://ujw.dianchejie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lib.316326.xyz

[S51] C++：显式类型转换
来源：http://cys.jqgfzy.top

static_cast<double>(a) / b
来源：http://vrk.redwolf501.top

[S52] C++：const 与 noexcept
来源：http://mcx.bjfxy.top

int size() const noexcept { return n_; }
来源：http://jps.hesvh.cn

[S53] C++：移动语义
来源：http://lpk.xinyue.icu

std::vector<int> w = std::move(v);
来源：http://obq.xinyue.icu

[S54] C++：异常处理
来源：http://ydg.wangshuangyany.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vnk.epnwcf.com

[S55] C++：结构化绑定
来源：http://gvr.c1oappe.top

auto [a, b] = std::make_pair(1, 2);
来源：http://mqq.gogol.net.cn

[S56] C++：optional
来源：http://csc.fktsv.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ldu.zycfv.cn

[S57] C++：编译期常量
来源：http://rsy.hesvh.cn

constexpr int N = 10;
来源：http://amw.haohaochexian.top

[S58] C++：命名空间
来源：http://ceh.fzhhl.top

namespace ns { int f() { return 1; } }
来源：http://nke.redwolf501.top

[S59] C++：静态断言
来源：http://xki.hywenlv.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fqk.sufxvd.cn

[S60] C++：遍历并删除元素
来源：http://uvy.52xcode.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wwj.nanxuanxn.top

================================================================================
来源：http://jij.ctjpmb.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dzt.uphjek.com

================================================================================
来源：http://klv.ehwqpu.com

[T01] Kotlin：Hello World
来源：http://hgw.zycfv.cn

println("Hello")
来源：http://jkv.shzxlz.cn

[T02] Kotlin：变量
来源：http://lll.wangdashe.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://agt.gotoacloud.top

[T03] Kotlin：字符串模板
来源：http://izc.jinyuanbaomall.cn

"值: $b"
来源：http://rpu.guowangkeji.top

[T04] Kotlin：空安全
来源：http://uwa.yuanzhike.top

val n: String? = null;  n?.length
来源：http://mnt.9152youxi.cn

[T05] Kotlin：when 表达式
来源：http://fzy.wangshuangyany.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://djb.shangyingyoupin.top

[T06] Kotlin：集合映射
来源：http://szr.ctjpmb.com

listOf(1, 2, 3).map { it * 2 }
来源：http://ikm.pengpengdd.cyou

[T07] Kotlin：集合过滤
来源：http://dsa.svipenyu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://pkt.c1oappe.top

[T08] Kotlin：数据类
来源：http://ipd.uphjek.com

data class User(val name: String, val age: Int)
来源：http://ptm.cheryme.top

[T09] Kotlin：扩展函数
来源：http://qic.hammf.cn

fun String.exclaim() = this + "!"
来源：http://jqo.wangdashe.top

[T10] Kotlin：默认参数
来源：http://lag.jinqigfzy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://tin.dianchejie.cn

[T11] Kotlin：协程
来源：http://ycc.yangfankeji.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://qja.zycfv.cn

[T12] Kotlin：解构声明
来源：http://neg.yangfankeji.com

val (a, b) = Pair(1, 2)
来源：http://zxr.gogol.net.cn

[T13] Kotlin：只读 Map
来源：http://xbi.nwbrower.top

val m = mapOf("a" to 1)
来源：http://gta.wangdashe.top

[T14] Kotlin：循环
来源：http://rjc.cashguo.top

for (i in 1..10) println(i)
来源：http://alx.kuanghao11.cn

[T15] Kotlin：接口
来源：http://yfc.bbcook.cn

interface Shape { fun area(): Double }
来源：http://tsr.sjlbkw.cn

[T16] Swift：Hello World
来源：http://fho.yueranfly.top

print("Hello")
来源：http://kli.hesvh.cn

[T17] Swift：变量与常量
来源：http://wlq.shanyushiyangkeji.top

var a = 1;  let b = 2
来源：http://hjb.epnwcf.com

[T18] Swift：字符串插值
来源：http://jdu.yueranfly.top

"值: \(b)"
来源：http://okx.chenlongwang.top

[T19] Swift：可选绑定
来源：http://fgq.pycfn.com

if let n = opt { print(n) }
来源：http://pfh.vqdsnc.cn

[T20] Swift：数组操作
来源：http://mau.ctjpmb.com

var a = [1, 2, 3];  a.append(4)
来源：http://zhc.ivvv.top

[T21] Swift：遍历
来源：http://ynb.yonumen.top

for x in a { print(x) }
来源：http://ezw.52xcode.cn

[T22] Swift：字典
来源：http://ggj.jlsjyb.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xrm.jiagoushi.top

[T23] Swift：函数
来源：http://hyb.gotoacloud.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zlq.zhixingplan.top

[T24] Swift：闭包
来源：http://xps.zycfv.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://swg.hnxiangtu.top

[T25] Swift：结构体
来源：http://sfq.tanke756.top

struct P { var x: Int }
来源：http://mmj.zdbjq.cn

[T26] Swift：类与重写
来源：http://pxs.zhengqikj.top

class A: Base { override func f() {} }
来源：http://ngr.bjfxy.top

[T27] Swift：错误处理
来源：http://umo.daria6918.cn

do { try f() } catch { print(error) }
来源：http://eyq.hywenlv.cn

[T28] Swift：枚举
来源：http://ali.xuetiantiany.cn

enum Color { case red, green }
来源：http://bzw.yongpay.top

[T29] Swift：guard 提前返回
来源：http://bqw.shangyingyoupin.top

guard let x = opt else { return }
来源：http://jiu.wangdashe.top

[T30] Swift：协议
来源：http://cyg.9152youxi.cn

protocol Shape { func area() -> Double }
来源：http://jmq.yuanzhike.top

[T31] Lua：Hello World
来源：http://ygk.shuidangran.top

print("Hello")
来源：http://tih.jinyuanbaomall.cn

[T32] Lua：局部变量
来源：http://ewk.havefunace.top

local a = 1
来源：http://eme.hcnkem.com

[T33] Lua：表（数组）
来源：http://lxr.daxiang520.top

local t = {1, 2, 3};  t[4] = 4
来源：http://tfk.pycfn.com

[T34] Lua：遍历表
来源：http://lvg.hesvh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://gjq.c1oappe.top

[T35] Lua：字典表
来源：http://lsm.yj20258888.top

local d = { a = 1 };  d.b = 2
来源：http://sme.nanxuanxn.top

[T36] Lua：函数
来源：http://ilp.tanke756.top

function add(a, b) return a + b end
来源：http://irm.vqdsnc.cn

[T37] Lua：字符串拼接
来源：http://uej.daxiang520.top

"a" .. "b"
来源：http://zoa.gzhubu.top

[T38] Lua：条件
来源：http://dog.mhx1999.top

if x > 0 then print("正") end
来源：http://lvu.yueranfly.top

[T39] Lua：模式匹配
来源：http://gum.fengsongda.top

string.find(s, "%d+")
来源：http://jxv.mhx1999.top

[T40] Lua：元表
来源：http://suo.yfazqb.com

setmetatable({}, { __index = base })
来源：http://dke.cashguo.top

[T41] Perl：Hello World
来源：http://jxh.jinqigufen.top

print "Hello\n";
来源：http://xle.shuidangran.top

[T42] Perl：变量类型
来源：http://igk.zhoulong.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zzv.nanxinkj.top

[T43] Perl：字符串插值
来源：http://vcq.yonumen.top

"值: $a"
来源：http://pmw.yj202588.top

[T44] Perl：条件
来源：http://nzi.fzhhl.top

if ($a > 0) { print "正"; }
来源：http://ycq.daxiang520.top

[T45] Perl：数组遍历
来源：http://qmq.pengpengdd.cyou

for my $x (@arr) { print $x; }
来源：http://ipk.0kj1m.cn

[T46] Perl：哈希操作
来源：http://zlw.sweek.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mmb.nwbrower.top

[T47] Perl：正则捕获
来源：http://mzl.daria6918.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://bjf.shanyushiyangkeji.top

[T48] Perl：正则替换
来源：http://xhy.yj202588.top

$s =~ s/old/new/g;
来源：http://cau.yongpay.top

[T49] Perl：函数
来源：http://okj.andypj.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bsv.yueranfly.top

[T50] Perl：逐行读文件
来源：http://nwq.cheryme.top

open my $fh, "<", "a.txt" or die $!;
来源：http://nqf.pycfn.com

while (my $line = <$fh>) { print $line; }
来源：http://gpo.wangshuangyany.cn

[T51] Scala：Hello World
来源：http://icd.hongshengwenyu.top

println("Hello")
来源：http://pje.zdqjudy.top

[T52] Scala：变量
来源：http://rsj.snrcjt.cn

val a = 1;  var b = 2
来源：http://luq.zhoulong.xyz

[T53] Scala：字符串插值
来源：http://von.yuxming.cn

s"值: $b"
来源：http://ykf.nanxuanxn.top

[T54] Scala：集合映射
来源：http://hrj.zycfv.cn

List(1, 2, 3).map(_ * 2)
来源：http://ypg.zhixingplan.top

[T55] Scala：集合过滤
来源：http://pfq.yongpay.top

List(1, 2, 3).filter(_ > 1)
来源：http://ikh.sxryk.cn

[T56] Scala：样例类
来源：http://flh.hnxiangtu.top

case class User(name: String, age: Int)
来源：http://mmp.tianlin.xyz

[T57] Scala：模式匹配
来源：http://tbb.wangshuangyany.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vfz.jqgfzy.top

[T58] Scala：函数定义
来源：http://lau.yj202588.top

def add(a: Int, b: Int): Int = a + b
来源：http://xha.zhoulong.xyz

[T59] Scala：循环
来源：http://edg.vehdjk.com

for (i <- 1 to 10) println(i)
来源：http://ffi.9152youxi.cn

[T60] Scala：折叠
来源：http://izg.yvedp.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ljt.cashguo.top

================================================================================
来源：http://riz.316326.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yqu.yongpay.top

================================================================================
来源：http://one.vehdjk.com

[U01] Py：创建虚拟环境
来源：http://rll.fengsongda.top

python -m venv .venv && source .venv/bin/activate
来源：http://pbx.shuidangran.top

[U02] Py：导出 / 安装依赖
来源：http://vva.tanke756.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vrx.bjfxy.top

[U03] Py：加载 .env 配置
来源：http://onf.hywenlv.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://lrd.nanxuanxn.top

[U04] Py：变量调试打印
来源：http://fed.gogol.net.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://roz.jinyuanbaomall.cn

[U05] Py：列表去重且保序
来源：http://tci.ctjpmb.com

list(dict.fromkeys(arr))
来源：http://pww.ctjpmb.com

[U06] Py：合并两个字典
来源：http://ksm.fengsongda.top

{**a, **b}
来源：http://uaf.sysykeji.top

[U07] Py：反转字典键值
来源：http://deq.sjlbkw.cn

{v: k for k, v in d.items()}
来源：http://rci.cucudq.cn

[U08] Py：展平二维列表
来源：http://tuo.zdqjudy.top

[y for x in nested for y in x]
来源：http://rzo.cdnleiting.top

[U09] Py：字典取最大值的键
来源：http://wxc.ivvv.top

max(d, key=d.get)
来源：http://ijg.sjlbkw.cn

[U10] Py：按值排序字典
来源：http://fvf.nanxinkj.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cct.gogol.net.cn

[U11] Py：生成器表达式
来源：http://xli.yongpay.top

(x * 2 for x in arr)
来源：http://afa.0kj1m.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mwp.xuetiantiany.cn

Counter(arr).most_common(3)
来源：http://wqy.xylfe.cn

[U13] Py：固定长度队列
来源：http://hek.yonumen.top

deque(maxlen=10)
来源：http://vhv.yfazqb.com

[U14] Py：分组收集到列表
来源：http://dgm.jinqigfzy.top

defaultdict(list)
来源：http://fra.svipenyu.cn

[U15] Py：高精度计时
来源：http://rnq.hnxiangtu.top

t = time.perf_counter()
来源：http://naf.birdmap.top

[U16] Py：命令行参数解析
来源：http://bch.sysykeji.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://usu.hysaishi.cn

[U17] Py：初始化日志
来源：http://nce.xuanzx.com

logging.basicConfig(level=logging.INFO)
来源：http://wma.fengsongda.top

[U18] Py：预编译正则
来源：http://xwd.fzhhl.top

pat = re.compile(r"\d+")
来源：http://jzf.ydjk.org.cn

[U19] Py：正则替换带回调
来源：http://cqk.shanyushiyangkeji.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yoa.cashguo.top

[U20] Py：缓存函数结果
来源：http://sje.dashuyun.cn

@functools.lru_cache(maxsize=None)
来源：http://sda.shuidangran.top

[U21] Py：自定义上下文管理器
来源：http://rbt.gotoacloud.top

@contextlib.contextmanager
来源：http://mmw.yangfankeji.com

[U22] Py：矩阵转置
来源：http://xhf.redwolf501.top

list(zip(*m))
来源：http://xmo.bjfxy.top

[U23] Py：分块读取大文件
来源：http://yrj.hesvh.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://fbf.zhoulong.xyz

[U24] Py：路径操作
来源：http://szy.zycfv.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rmo.shzxlz.cn

[U25] Py：CSV 按字典读
来源：http://keo.dianchejie.cn

csv.DictReader(f)
来源：http://xfn.hfpthk.cn

[U26] Py：并发下载
来源：http://lyp.fktsv.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://rco.jinyuanbaomall.cn

[U27] Py：异步 HTTP
来源：http://btg.cashguo.top

aiohttp.ClientSession() 配合 async with
来源：http://lmw.xingfuxueyuan.xyz

[U28] Py：类型别名
来源：http://rrh.svipenyu.cn

UserId = int
来源：http://mpl.sufxvd.cn

[U29] Py：属性校验
来源：http://wbk.haohaochexian.top

@property 与 @x.setter 配合
来源：http://ztr.wangshuangyany.cn

[U30] Py：数据类
来源：http://rxc.yvedp.cn

@dataclass(slots=True)
来源：http://uxs.9152youxi.cn

[U31] Py：单测
来源：http://bob.sweek.top

python -m pytest -q
来源：http://ttz.jyoumei.cn

[U32] Py：代码格式化
来源：http://nql.yueranfly.top

ruff format . && ruff check --fix .
来源：http://fij.pycfn.com

[U33] Py：打包发布
来源：http://hrv.pengpengdd.cyou

python -m build  （依赖 pyproject.toml）
来源：http://hys.andypj.xyz

[U34] Py：判断编码
来源：http://buj.ehwqpu.com

chardet.detect(raw)
来源：http://mvl.sufxvd.cn

[U35] Py：发送邮件
来源：http://xmg.pycfn.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://uot.ctjpmb.com

[U36] Py：定时任务
来源：http://jng.316326.xyz

schedule.every(10).minutes.do(job)
来源：http://ibr.316326.xyz

[U37] Py：读写 Excel
来源：http://tdd.hcnkem.com

pandas.read_excel / DataFrame.to_excel
来源：http://mcn.hysaishi.cn

[U38] Py：获取脚本所在目录
来源：http://fqc.52xcode.cn

Path(__file__).resolve().parent
来源：http://yya.nanxuanxn.top

[U39] Py：判断是否在交互环境
来源：http://jsu.hysaishi.cn

sys.stdout.isatty()
来源：http://inx.guowangkeji.top

[U40] Py：打印到标准错误
来源：http://mqj.ywan-chungtsiang.top

print("err", file=sys.stderr)
来源：http://kro.cdnleiting.top

[U41] PHP：初始化 Composer 项目
来源：http://tdj.fengsongda.top

composer init;  composer require guzzlehttp/guzzle
来源：http://hvw.yonumen.top

[U42] PHP：PSR-4 自动加载
来源：http://szs.xuanzx.com

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fje.zhaomingkeji.xyz

[U43] PHP：声明命名空间
来源：http://xff.shanyushiyangtech.top

namespace App\Http;
来源：http://obw.pengpengdd.cyou

[U44] PHP：开启严格类型
来源：http://lmc.quarkkingdee.top

declare(strict_types=1);
来源：http://hwd.xingfuxueyuan.xyz

[U45] PHP：类型声明与返回类型
来源：http://wnq.yuxming.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://qlf.bjfxy.top

[U46] PHP：可空类型
来源：http://zhp.svipenyu.cn

?string $name = null
来源：http://jmz.shanyushiyangtech.top

[U47] PHP：联合类型
来源：http://oif.yueranfly.top

int|string $id
来源：http://uld.gogol.net.cn

[U48] PHP：纯枚举
来源：http://iqe.jinqigufen.top

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ucq.zhaomingkeji.xyz


<!-- 参考信息 -->