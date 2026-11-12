代发 wailian999

x |= (1 << 3);
来源：http://ujf.jlsjyb.cn

[S17] C：安全拼接字符串
来源：http://gvm.gotoacloud.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hhn.kuanghao11.cn

[S18] C：命令行参数
来源：http://rsw.uphjek.com

int main(int argc, char **argv)
来源：http://yak.jqgfzy.top

[S19] C：快速排序
来源：http://zeo.hcnkem.com

qsort(a, n, sizeof(int), cmp);
来源：http://jns.cqqwz.cn

[S20] C：二分查找
来源：http://gpg.zycfv.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://end.ydzc1.top

[S21] C：字符类别判断
来源：http://cuj.pycfn.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://slk.9152youxi.cn

[S22] C：字符串转数字
来源：http://hyn.ivvv.top

atoi("42");  strtod("3.14", NULL);
来源：http://mhi.xingfuxueyuan.xyz

[S23] C：随机数
来源：http://jsa.andypj.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://fyr.feifeiyinyue.top

[S24] C：获取本地时间
来源：http://aus.316326.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uvo.cdnleiting.top

[S25] C：内存拷贝
来源：http://urj.cqqwz.cn

memcpy(dst, src, n);
来源：http://unx.jiagoushi.top

[S26] C：内存清零
来源：http://otz.aibaodan.cn

memset(a, 0, sizeof a);
来源：http://zhh.yfazqb.com

[S27] C：定义常量
来源：http://mew.iojbl.cn

const double PI = 3.14159;
来源：http://wji.daria6918.cn

[S28] C：静态变量
来源：http://dfc.9152youxi.cn

static int counter = 0;
来源：http://rgs.yongpay.top

[S29] C：变参函数
来源：http://nwo.epnwcf.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lro.guowangkeji.top

[S30] C：头文件保护
来源：http://eij.gotoacloud.top

#ifndef X_H
来源：http://fub.tian-w.cn

#define X_H
来源：http://gkl.jinqigufen.top

#endif
来源：http://lov.wangshuangyany.cn

[S31] C++：Hello World
来源：http://zyf.epnwcf.com

#include <iostream>
来源：http://xzi.fehbvm.com

int main() { std::cout << "Hello\n"; }
来源：http://mme.ybcxt.top

[S32] C++：字符串
来源：http://bch.tianlin.xyz

std::string s = "hi";  s += "!";
来源：http://ffp.tian-w.cn

[S33] C++：vector 增删
来源：http://tbo.yangfankeji.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hlv.chenlongwang.top

[S34] C++：遍历 vector
来源：http://klb.zhoulong.xyz

for (auto &x : v) { std::cout << x; }
来源：http://fyw.chenjidiqi.icu

[S35] C++：map
来源：http://mvc.ydzc1.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gia.gogol.net.cn

[S36] C++：unordered_map
来源：http://jfj.hnqzz.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pan.jinqigufen.top

[S37] C++：set
来源：http://vja.birdmap.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vyx.chenzaomai.com

[S38] C++：排序
来源：http://ain.cdnleiting.top

std::sort(v.begin(), v.end());
来源：http://alj.ybcxt.top

[S39] C++：自定义比较器排序
来源：http://siq.kuanghao11.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://axc.cdnleiting.top

[S40] C++：查找元素
来源：http://slq.snrcjt.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://clg.wangshuangyany.cn

[S41] C++：类与构造函数
来源：http://eyx.c1oappe.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://aef.guowangkeji.top

[S42] C++：继承与虚函数
来源：http://eqt.haohaochexian.top

class B : public Base { public: void f() override {} };
来源：http://qcq.tarul.cn

[S43] C++：智能指针
来源：http://jzp.yuanzhike.top

auto p = std::make_unique<int>(5);
来源：http://xkc.shanyushiyangtech.top

[S44] C++：引用传参
来源：http://otu.daxiang520.top

void inc(int &x) { ++x; }
来源：http://jaw.ppjwa.cn

[S45] C++：lambda
来源：http://ycx.sjlbkw.cn

auto add = [](int a, int b) { return a + b; };
来源：http://auf.wangdashe.top

[S46] C++：函数模板
来源：http://xvn.nanxuanxn.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bdu.nanxuanxn.top

[S47] C++：结构化绑定遍历
来源：http://ind.sweek.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xma.aizwys.cn

[S48] C++：逐行读文件
来源：http://ojo.ydjk.org.cn

std::ifstream in("a.txt");  std::string line;
来源：http://avl.sxryk.cn

while (std::getline(in, line)) { }
来源：http://tnh.mhx1999.top

[S49] C++：写文件
来源：http://onr.fktsv.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ycv.xinyue.icu

[S50] C++：格式化数字
来源：http://ata.fengsongda.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pux.ctjpmb.com

[S51] C++：显式类型转换
来源：http://yiw.jinyuanbaomall.cn

static_cast<double>(a) / b
来源：http://nss.yj20258888.top

[S52] C++：const 与 noexcept
来源：http://dar.jinghuilouyu.cn

int size() const noexcept { return n_; }
来源：http://mts.zhaomingkeji.xyz

[S53] C++：移动语义
来源：http://exd.jinqigufen.top

std::vector<int> w = std::move(v);
来源：http://hxr.316326.xyz

[S54] C++：异常处理
来源：http://tmm.jinqigfzy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://col.birdmap.top

[S55] C++：结构化绑定
来源：http://bkm.hfpthk.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://yym.jlsjyb.cn

[S56] C++：optional
来源：http://yvf.andypj.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://grh.guowangkeji.top

[S57] C++：编译期常量
来源：http://mwb.ybcxt.top

constexpr int N = 10;
来源：http://uzg.chenlongwang.top

[S58] C++：命名空间
来源：http://gvn.hammf.cn

namespace ns { int f() { return 1; } }
来源：http://nxt.jinghuilouyu.cn

[S59] C++：静态断言
来源：http://rzj.pycfn.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ieu.kuanghao11.cn

[S60] C++：遍历并删除元素
来源：http://tvu.ctjpmb.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dkh.dashuyun.cn

================================================================================
来源：http://cpt.fzhhl.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vlj.yj20258.top

================================================================================
来源：http://shk.fzhhl.top

[T01] Kotlin：Hello World
来源：http://hsu.meibo888.top

println("Hello")
来源：http://zcd.yuanzhike.top

[T02] Kotlin：变量
来源：http://eyl.ydzc1.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hsq.yuanzhike.top

[T03] Kotlin：字符串模板
来源：http://ebn.zdqjudy.top

"值: $b"
来源：http://uyi.xuanzx.com

[T04] Kotlin：空安全
来源：http://xod.hywenlv.cn

val n: String? = null;  n?.length
来源：http://sig.gotoacloud.top

[T05] Kotlin：when 表达式
来源：http://fwo.aizwys.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ait.nanxinkj.top

[T06] Kotlin：集合映射
来源：http://gtz.quarkkingdee.top

listOf(1, 2, 3).map { it * 2 }
来源：http://oik.bbcook.cn

[T07] Kotlin：集合过滤
来源：http://ody.jinyuanbaomall.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://bsu.sufxvd.cn

[T08] Kotlin：数据类
来源：http://bqw.gaohongyu789.top

data class User(val name: String, val age: Int)
来源：http://ktv.jinqigfzy.top

[T09] Kotlin：扩展函数
来源：http://ona.jinqigfzy.top

fun String.exclaim() = this + "!"
来源：http://ggs.wangdashe.top

[T10] Kotlin：默认参数
来源：http://bdf.tanke756.top

fun greet(name: String = "World") = "Hi $name"
来源：http://etn.yangfankeji.com

[T11] Kotlin：协程
来源：http://pxa.birdmap.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://fdw.redwolf501.top

[T12] Kotlin：解构声明
来源：http://cwt.hywenlv.cn

val (a, b) = Pair(1, 2)
来源：http://olu.gzhubu.top

[T13] Kotlin：只读 Map
来源：http://aur.shangyingyoupin.top

val m = mapOf("a" to 1)
来源：http://cpo.9152youxi.cn

[T14] Kotlin：循环
来源：http://njg.cucudq.cn

for (i in 1..10) println(i)
来源：http://nio.yanxiufei.cn

[T15] Kotlin：接口
来源：http://fim.meibo888.top

interface Shape { fun area(): Double }
来源：http://omp.gotoacloud.top

[T16] Swift：Hello World
来源：http://tcs.redwolf501.top

print("Hello")
来源：http://iig.sjlbkw.cn

[T17] Swift：变量与常量
来源：http://dfn.fzhhl.top

var a = 1;  let b = 2
来源：http://gzp.hywenlv.cn

[T18] Swift：字符串插值
来源：http://dcb.yanxiufei.cn

"值: \(b)"
来源：http://cvz.shanyushiyangtech.top

[T19] Swift：可选绑定
来源：http://jdk.shanyushiyangtech.top

if let n = opt { print(n) }
来源：http://tsm.daria6918.cn

[T20] Swift：数组操作
来源：http://rqy.shangyingyoupin.top

var a = [1, 2, 3];  a.append(4)
来源：http://azm.hnqzz.top

[T21] Swift：遍历
来源：http://iod.birdmap.top

for x in a { print(x) }
来源：http://yge.sweek.top

[T22] Swift：字典
来源：http://fvu.nwbrower.top

var d = ["a": 1];  d["b"] = 2
来源：http://eas.meibo888.top

[T23] Swift：函数
来源：http://lcr.cashguo.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zux.hnqzz.top

[T24] Swift：闭包
来源：http://kpe.sufxvd.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://tgy.yj20258888.top

[T25] Swift：结构体
来源：http://xxk.jianghu66.top

struct P { var x: Int }
来源：http://lsc.ybcxt.top

[T26] Swift：类与重写
来源：http://zfm.kuanghao11.cn

class A: Base { override func f() {} }
来源：http://mem.aibaodan.cn

[T27] Swift：错误处理
来源：http://vpg.iojbl.cn

do { try f() } catch { print(error) }
来源：http://klg.tian-w.cn

[T28] Swift：枚举
来源：http://fws.wangdashe.top

enum Color { case red, green }
来源：http://sgl.cashguo.top

[T29] Swift：guard 提前返回
来源：http://yeq.hongshengwenyu.top

guard let x = opt else { return }
来源：http://osl.yuanzhike.top

[T30] Swift：协议
来源：http://saa.fanxiaobao.xyz

protocol Shape { func area() -> Double }
来源：http://six.pycfn.com

[T31] Lua：Hello World
来源：http://wwa.fzhhl.top

print("Hello")
来源：http://cte.hcnkem.com

[T32] Lua：局部变量
来源：http://wdu.ydzc1.top

local a = 1
来源：http://cmf.shangyingyoupin.top

[T33] Lua：表（数组）
来源：http://zwl.jinqigfzy.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ajh.sxryk.cn

[T34] Lua：遍历表
来源：http://oxj.quarkkingdee.top

for i, v in ipairs(t) do print(i, v) end
来源：http://dkb.pycfn.com

[T35] Lua：字典表
来源：http://hxr.sufxvd.cn

local d = { a = 1 };  d.b = 2
来源：http://uru.chenjidiqi.icu

[T36] Lua：函数
来源：http://aax.gotoacloud.top

function add(a, b) return a + b end
来源：http://uvj.yangfankeji.com

[T37] Lua：字符串拼接
来源：http://zsh.zhaomingkeji.xyz

"a" .. "b"
来源：http://ycf.birdmap.top

[T38] Lua：条件
来源：http://vas.zhijiandao.cn

if x > 0 then print("正") end
来源：http://wwv.jinyuanbaomall.cn

[T39] Lua：模式匹配
来源：http://qon.uphjek.com

string.find(s, "%d+")
来源：http://pqx.jyoumei.cn

[T40] Lua：元表
来源：http://uqk.xingfuxueyuan.xyz

setmetatable({}, { __index = base })
来源：http://kaw.ehwqpu.com

[T41] Perl：Hello World
来源：http://fke.zycfv.cn

print "Hello\n";
来源：http://gsq.jqgufenzy.top

[T42] Perl：变量类型
来源：http://jwj.jiagoushi.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lmp.gaohongyu789.top

[T43] Perl：字符串插值
来源：http://rjf.jiagoushi.top

"值: $a"
来源：http://bmb.bbcook.cn

[T44] Perl：条件
来源：http://doz.feifeiyinyue.top

if ($a > 0) { print "正"; }
来源：http://jnr.cashguo.top

[T45] Perl：数组遍历
来源：http://xln.bbcook.cn

for my $x (@arr) { print $x; }
来源：http://xhz.xingfuxueyuan.xyz

[T46] Perl：哈希操作
来源：http://qrn.sweek.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mjn.zhijiandao.cn

[T47] Perl：正则捕获
来源：http://ycp.jianghu66.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://opl.xylfe.cn

[T48] Perl：正则替换
来源：http://rlk.zhaomingkeji.xyz

$s =~ s/old/new/g;
来源：http://vjh.ydjk.org.cn

[T49] Perl：函数
来源：http://ccb.ehwqpu.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://opr.wangdashe.top

[T50] Perl：逐行读文件
来源：http://yen.jianghu66.top

open my $fh, "<", "a.txt" or die $!;
来源：http://fll.jinqigufen.top

while (my $line = <$fh>) { print $line; }
来源：http://jmx.nanxinkj.top

[T51] Scala：Hello World
来源：http://xxv.birdmap.top

println("Hello")
来源：http://xzw.nanxinkj.top

[T52] Scala：变量
来源：http://hln.hammf.cn

val a = 1;  var b = 2
来源：http://pyk.jyoumei.cn

[T53] Scala：字符串插值
来源：http://xeq.zhaomingkeji.xyz

s"值: $b"
来源：http://tti.ctjpmb.com

[T54] Scala：集合映射
来源：http://vnn.xziqi.cn

List(1, 2, 3).map(_ * 2)
来源：http://hfu.ehwqpu.com

[T55] Scala：集合过滤
来源：http://wou.yfazqb.com

List(1, 2, 3).filter(_ > 1)
来源：http://mcd.hesvh.cn

[T56] Scala：样例类
来源：http://mmr.gzhubu.top

case class User(name: String, age: Int)
来源：http://xzv.ivvv.top

[T57] Scala：模式匹配
来源：http://khy.dianchejie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://yuj.c1oappe.top

[T58] Scala：函数定义
来源：http://gjh.tarul.cn

def add(a: Int, b: Int): Int = a + b
来源：http://miq.yueranfly.top

[T59] Scala：循环
来源：http://wdy.iojbl.cn

for (i <- 1 to 10) println(i)
来源：http://nxt.xingfuxueyuan.xyz

[T60] Scala：折叠
来源：http://qxl.pengpengdd.cyou

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jlq.cheryme.top

================================================================================
来源：http://gru.chenlongwang.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yvd.jinqigufen.top

================================================================================
来源：http://hvb.vqdsnc.cn

[U01] Py：创建虚拟环境
来源：http://ovi.hywenlv.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ped.jinyuanbaomall.cn

[U02] Py：导出 / 安装依赖
来源：http://fmu.gogol.net.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://egj.yangfankeji.com

[U03] Py：加载 .env 配置
来源：http://xur.hongshengwenyu.top

from dotenv import load_dotenv; load_dotenv()
来源：http://acs.hnqzz.top

[U04] Py：变量调试打印
来源：http://odh.yanxiufei.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ccc.shzxlz.cn

[U05] Py：列表去重且保序
来源：http://xgj.shuidangran.top

list(dict.fromkeys(arr))
来源：http://etc.hysaishi.cn

[U06] Py：合并两个字典
来源：http://ayj.uphjek.com

{**a, **b}
来源：http://qtn.svipenyu.cn

[U07] Py：反转字典键值
来源：http://tvo.xingfuxueyuan.xyz

{v: k for k, v in d.items()}
来源：http://hnv.yongpay.top

[U08] Py：展平二维列表
来源：http://jed.svipenyu.cn

[y for x in nested for y in x]
来源：http://kot.hcnkem.com

[U09] Py：字典取最大值的键
来源：http://buf.zycfv.cn

max(d, key=d.get)
来源：http://ozc.c1oappe.top

[U10] Py：按值排序字典
来源：http://uqn.jinyuanbaomall.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://wmm.ehwqpu.com

[U11] Py：生成器表达式
来源：http://pdm.nanxuanxn.top

(x * 2 for x in arr)
来源：http://apa.daria6918.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mqo.fktsv.cn

Counter(arr).most_common(3)
来源：http://syp.dashuyun.cn

[U13] Py：固定长度队列
来源：http://ghf.xinyue.icu

deque(maxlen=10)
来源：http://rdv.quarkkingdee.top

[U14] Py：分组收集到列表
来源：http://oni.guowangkeji.top

defaultdict(list)
来源：http://kyy.zhengqikj.top

[U15] Py：高精度计时
来源：http://sis.fengsongda.top

t = time.perf_counter()
来源：http://yxg.snrcjt.cn

[U16] Py：命令行参数解析
来源：http://ujv.zhijiandao.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cyf.zhiwuduotai.top

[U17] Py：初始化日志
来源：http://vbd.ivvv.top

logging.basicConfig(level=logging.INFO)
来源：http://hzu.fanxiaobao.xyz

[U18] Py：预编译正则
来源：http://yax.hammf.cn

pat = re.compile(r"\d+")
来源：http://jtn.hcnkem.com

[U19] Py：正则替换带回调
来源：http://yme.aizwys.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://uat.xuanzx.com

[U20] Py：缓存函数结果
来源：http://qzz.yuxming.cn

@functools.lru_cache(maxsize=None)
来源：http://ztx.zhijiandao.cn

[U21] Py：自定义上下文管理器
来源：http://ckw.svipenyu.cn

@contextlib.contextmanager
来源：http://vwq.xziqi.cn

[U22] Py：矩阵转置
来源：http://uxd.nanxinkj.top

list(zip(*m))
来源：http://hgz.gaohongyu789.top

[U23] Py：分块读取大文件
来源：http://bza.epnwcf.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://byx.yangfankeji.com

[U24] Py：路径操作
来源：http://zyd.0kj1m.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://isk.jinqigfzy.top

[U25] Py：CSV 按字典读
来源：http://gmf.ctjpmb.com

csv.DictReader(f)
来源：http://qzy.cashguo.top

[U26] Py：并发下载
来源：http://lcr.hfpthk.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://oob.yvedp.cn

[U27] Py：异步 HTTP
来源：http://taq.ppjwa.cn

aiohttp.ClientSession() 配合 async with
来源：http://nmu.0kj1m.cn

[U28] Py：类型别名
来源：http://yfh.dashuyun.cn

UserId = int
来源：http://xip.zhijiandao.cn

[U29] Py：属性校验
来源：http://ods.yangfankeji.com

@property 与 @x.setter 配合
来源：http://pfj.hcnkem.com

[U30] Py：数据类
来源：http://iii.chenjidiqi.icu

@dataclass(slots=True)
来源：http://hpb.hnxiangtu.top

[U31] Py：单测
来源：http://nem.iojbl.cn

python -m pytest -q
来源：http://ojm.jlsjyb.cn

[U32] Py：代码格式化
来源：http://yxf.tianlin.xyz

ruff format . && ruff check --fix .
来源：http://wje.hywenlv.cn

[U33] Py：打包发布
来源：http://dkx.xuanzx.com

python -m build  （依赖 pyproject.toml）
来源：http://mxu.xziqi.cn

[U34] Py：判断编码
来源：http://sof.xziqi.cn

chardet.detect(raw)
来源：http://qri.meibo888.top

[U35] Py：发送邮件
来源：http://mde.mhx1999.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tah.shzxlz.cn

[U36] Py：定时任务
来源：http://mlz.jianghu66.top

schedule.every(10).minutes.do(job)
来源：http://xdg.sweek.top

[U37] Py：读写 Excel
来源：http://nef.jinyuanbaomall.cn

pandas.read_excel / DataFrame.to_excel
来源：http://zek.zdbjq.cn

[U38] Py：获取脚本所在目录
来源：http://pmq.52xcode.cn

Path(__file__).resolve().parent
来源：http://qxe.kuanghao11.cn

[U39] Py：判断是否在交互环境
来源：http://lfn.zhaomingkeji.xyz

sys.stdout.isatty()
来源：http://ivv.zhoulong.xyz

[U40] Py：打印到标准错误
来源：http://gxq.zhiwuduotai.top

print("err", file=sys.stderr)
来源：http://pwi.daria6918.cn


<!-- 参考信息 -->