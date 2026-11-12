代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xzg.zdqjudy.top

[S13] C：宏定义
来源：http://ziz.fengsongda.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zmw.sjlbkw.cn

[S14] C：枚举
来源：http://iib.jqgfzy.top

enum Color { RED, GREEN, BLUE };
来源：http://phf.yfazqb.com

[S15] C：类型转换
来源：http://nus.fehbvm.com

(double) a / b
来源：http://sor.hnqzz.top

[S16] C：位操作置位
来源：http://sks.sufxvd.cn

x |= (1 << 3);
来源：http://uhi.meibo888.top

[S17] C：安全拼接字符串
来源：http://ngv.hywenlv.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nol.ydzc1.top

[S18] C：命令行参数
来源：http://zua.zhoulong.xyz

int main(int argc, char **argv)
来源：http://nmm.ctjpmb.com

[S19] C：快速排序
来源：http://xfe.xuetiantiany.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qra.zhoulong.xyz

[S20] C：二分查找
来源：http://jmh.birdmap.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kga.guowangkeji.top

[S21] C：字符类别判断
来源：http://mtn.jinqigufen.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cpv.wangdashe.top

[S22] C：字符串转数字
来源：http://ifb.tanke756.top

atoi("42");  strtod("3.14", NULL);
来源：http://dsz.jianghu66.top

[S23] C：随机数
来源：http://qxk.pengpengdd.cyou

srand(time(NULL));  int r = rand() % 100;
来源：http://gvk.vqdsnc.cn

[S24] C：获取本地时间
来源：http://ouc.ydzc1.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gqi.cdnleiting.top

[S25] C：内存拷贝
来源：http://ldk.pengpengdd.cyou

memcpy(dst, src, n);
来源：http://owk.yanxiufei.cn

[S26] C：内存清零
来源：http://cqc.chenjidiqi.icu

memset(a, 0, sizeof a);
来源：http://cgs.aizwys.cn

[S27] C：定义常量
来源：http://mjr.xylfe.cn

const double PI = 3.14159;
来源：http://abv.ydjk.org.cn

[S28] C：静态变量
来源：http://qvz.pengpengdd.cyou

static int counter = 0;
来源：http://vdb.guowangkeji.top

[S29] C：变参函数
来源：http://iij.yonumen.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pei.chenzaomai.com

[S30] C：头文件保护
来源：http://onc.zycfv.cn

#ifndef X_H
来源：http://ven.zdbjq.cn

#define X_H
来源：http://mdi.gotoacloud.top

#endif
来源：http://byl.aibaodan.cn

[S31] C++：Hello World
来源：http://wsp.hnqzz.top

#include <iostream>
来源：http://eck.dashuyun.cn

int main() { std::cout << "Hello\n"; }
来源：http://guz.zycfv.cn

[S32] C++：字符串
来源：http://wsy.shzxlz.cn

std::string s = "hi";  s += "!";
来源：http://xuh.yj20258.top

[S33] C++：vector 增删
来源：http://srt.wangshuangyany.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xew.sysykeji.top

[S34] C++：遍历 vector
来源：http://obc.316326.xyz

for (auto &x : v) { std::cout << x; }
来源：http://uyy.cdnleiting.top

[S35] C++：map
来源：http://elk.shanyushiyangtech.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yov.tianlin.xyz

[S36] C++：unordered_map
来源：http://otu.yuanzhike.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blr.snrcjt.cn

[S37] C++：set
来源：http://tyl.tianlin.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://itc.jiagoushi.top

[S38] C++：排序
来源：http://tmx.pengpengdd.cyou

std::sort(v.begin(), v.end());
来源：http://eem.aibaodan.cn

[S39] C++：自定义比较器排序
来源：http://tzu.epnwcf.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gcu.jqgufenzy.top

[S40] C++：查找元素
来源：http://xah.xinyue.icu

auto it = std::find(v.begin(), v.end(), 3);
来源：http://iio.chenlongwang.top

[S41] C++：类与构造函数
来源：http://lya.0kj1m.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fuj.ctjpmb.com

[S42] C++：继承与虚函数
来源：http://dxk.meibo888.top

class B : public Base { public: void f() override {} };
来源：http://ciz.sweek.top

[S43] C++：智能指针
来源：http://emz.aibaodan.cn

auto p = std::make_unique<int>(5);
来源：http://caq.nanxuanxn.top

[S44] C++：引用传参
来源：http://dit.nwbrower.top

void inc(int &x) { ++x; }
来源：http://pfh.fanxiaobao.xyz

[S45] C++：lambda
来源：http://nyl.epnwcf.com

auto add = [](int a, int b) { return a + b; };
来源：http://hnl.gaohongyu789.top

[S46] C++：函数模板
来源：http://keq.shanyushiyangtech.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gse.tian-w.cn

[S47] C++：结构化绑定遍历
来源：http://ghb.aizwys.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kfn.shangyingyoupin.top

[S48] C++：逐行读文件
来源：http://jbj.gzhubu.top

std::ifstream in("a.txt");  std::string line;
来源：http://pmh.guannengcc.top

while (std::getline(in, line)) { }
来源：http://xlc.yuanzhike.top

[S49] C++：写文件
来源：http://ybk.gotoacloud.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ntp.316326.xyz

[S50] C++：格式化数字
来源：http://fql.jinyuanbaomall.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nto.andypj.xyz

[S51] C++：显式类型转换
来源：http://rgi.xingfuxueyuan.xyz

static_cast<double>(a) / b
来源：http://ptq.pycfn.com

[S52] C++：const 与 noexcept
来源：http://kas.sjlbkw.cn

int size() const noexcept { return n_; }
来源：http://jsw.xuanzx.com

[S53] C++：移动语义
来源：http://bld.jianghu66.top

std::vector<int> w = std::move(v);
来源：http://ima.shzxlz.cn

[S54] C++：异常处理
来源：http://ajh.epnwcf.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://aqm.gaohongyu789.top

[S55] C++：结构化绑定
来源：http://yrg.epnwcf.com

auto [a, b] = std::make_pair(1, 2);
来源：http://bpr.hammf.cn

[S56] C++：optional
来源：http://wkv.xylfe.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://eml.jyoumei.cn

[S57] C++：编译期常量
来源：http://rvl.zhiwuduotai.top

constexpr int N = 10;
来源：http://huz.nanxuanxn.top

[S58] C++：命名空间
来源：http://shv.hfpthk.cn

namespace ns { int f() { return 1; } }
来源：http://gug.nanxuanxn.top

[S59] C++：静态断言
来源：http://krx.zhiwuduotai.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tzh.yanxiufei.cn

[S60] C++：遍历并删除元素
来源：http://eoj.jinghuilouyu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bqt.0kj1m.cn

================================================================================
来源：http://bda.hnqzz.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ocg.ppjwa.cn

================================================================================
来源：http://pbs.yanxiufei.cn

[T01] Kotlin：Hello World
来源：http://fmn.zhijiandao.cn

println("Hello")
来源：http://wen.ppjwa.cn

[T02] Kotlin：变量
来源：http://has.hnqzz.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://znh.havefunace.top

[T03] Kotlin：字符串模板
来源：http://chi.tian-w.cn

"值: $b"
来源：http://pjy.zhixingplan.top

[T04] Kotlin：空安全
来源：http://tgt.jlsjyb.cn

val n: String? = null;  n?.length
来源：http://kro.daxiang520.top

[T05] Kotlin：when 表达式
来源：http://pvr.ybcxt.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xgd.haohaochexian.top

[T06] Kotlin：集合映射
来源：http://arc.vqdsnc.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://vvi.wangshuangyany.cn

[T07] Kotlin：集合过滤
来源：http://ppj.tarul.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qbd.ctjpmb.com

[T08] Kotlin：数据类
来源：http://qea.bjfxy.top

data class User(val name: String, val age: Int)
来源：http://nzj.svipenyu.cn

[T09] Kotlin：扩展函数
来源：http://nve.jiagoushi.top

fun String.exclaim() = this + "!"
来源：http://vuk.c1oappe.top

[T10] Kotlin：默认参数
来源：http://lsz.tarul.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tbk.jiagoushi.top

[T11] Kotlin：协程
来源：http://yiq.zhoulong.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://zjo.pengpengdd.cyou

[T12] Kotlin：解构声明
来源：http://bdk.sweek.top

val (a, b) = Pair(1, 2)
来源：http://szw.sweek.top

[T13] Kotlin：只读 Map
来源：http://rhy.xuanzx.com

val m = mapOf("a" to 1)
来源：http://thj.hongshengwenyu.top

[T14] Kotlin：循环
来源：http://sce.birdmap.top

for (i in 1..10) println(i)
来源：http://ifz.hongshengwenyu.top

[T15] Kotlin：接口
来源：http://ucj.jiagoushi.top

interface Shape { fun area(): Double }
来源：http://zly.jqgfzy.top

[T16] Swift：Hello World
来源：http://saj.guannengcc.top

print("Hello")
来源：http://mwp.zhijiandao.cn

[T17] Swift：变量与常量
来源：http://bwf.gaohongyu789.top

var a = 1;  let b = 2
来源：http://azu.nwbrower.top

[T18] Swift：字符串插值
来源：http://pzz.zdbjq.cn

"值: \(b)"
来源：http://gtw.jqgfzy.top

[T19] Swift：可选绑定
来源：http://msc.zhengqikj.top

if let n = opt { print(n) }
来源：http://zro.xuanzx.com

[T20] Swift：数组操作
来源：http://kxe.andypj.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://mnd.xuetiantiany.cn

[T21] Swift：遍历
来源：http://hks.yvedp.cn

for x in a { print(x) }
来源：http://zpn.yfazqb.com

[T22] Swift：字典
来源：http://bfo.mhx1999.top

var d = ["a": 1];  d["b"] = 2
来源：http://luc.hesvh.cn

[T23] Swift：函数
来源：http://pco.wangshuangyany.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kxr.jlsjyb.cn

[T24] Swift：闭包
来源：http://owt.xziqi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://htx.hfpthk.cn

[T25] Swift：结构体
来源：http://mln.smart0.xyz

struct P { var x: Int }
来源：http://hnf.jinghuilouyu.cn

[T26] Swift：类与重写
来源：http://mgd.shuidangran.top

class A: Base { override func f() {} }
来源：http://fbj.gaohongyu789.top

[T27] Swift：错误处理
来源：http://ehp.ctjpmb.com

do { try f() } catch { print(error) }
来源：http://xmh.tanke756.top

[T28] Swift：枚举
来源：http://juy.shanyushiyangtech.top

enum Color { case red, green }
来源：http://hja.tanke756.top

[T29] Swift：guard 提前返回
来源：http://axa.hysaishi.cn

guard let x = opt else { return }
来源：http://ljm.quarkkingdee.top

[T30] Swift：协议
来源：http://rqs.yonumen.top

protocol Shape { func area() -> Double }
来源：http://jeo.dashuyun.cn

[T31] Lua：Hello World
来源：http://zwk.xziqi.cn

print("Hello")
来源：http://tyf.zdqjudy.top

[T32] Lua：局部变量
来源：http://mmd.hongshengwenyu.top

local a = 1
来源：http://muv.zhixingplan.top

[T33] Lua：表（数组）
来源：http://lze.yvedp.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ocz.haohaochexian.top

[T34] Lua：遍历表
来源：http://izr.yj20258888.top

for i, v in ipairs(t) do print(i, v) end
来源：http://tyb.guowangkeji.top

[T35] Lua：字典表
来源：http://oot.sjlbkw.cn

local d = { a = 1 };  d.b = 2
来源：http://zgu.yonumen.top

[T36] Lua：函数
来源：http://rnq.zycfv.cn

function add(a, b) return a + b end
来源：http://syf.hongshengwenyu.top

[T37] Lua：字符串拼接
来源：http://zeb.sufxvd.cn

"a" .. "b"
来源：http://nqk.ivvv.top

[T38] Lua：条件
来源：http://vrw.guowangkeji.top

if x > 0 then print("正") end
来源：http://nsu.mhx1999.top

[T39] Lua：模式匹配
来源：http://pka.jyoumei.cn

string.find(s, "%d+")
来源：http://tip.zhoulong.xyz

[T40] Lua：元表
来源：http://ibr.jiagoushi.top

setmetatable({}, { __index = base })
来源：http://low.guannengcc.top

[T41] Perl：Hello World
来源：http://fty.shuidangran.top

print "Hello\n";
来源：http://def.gaohongyu789.top

[T42] Perl：变量类型
来源：http://uke.yuanzhike.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://znx.pycfn.com

[T43] Perl：字符串插值
来源：http://ixr.zycfv.cn

"值: $a"
来源：http://zfb.gogol.net.cn

[T44] Perl：条件
来源：http://mqk.fengsongda.top

if ($a > 0) { print "正"; }
来源：http://ckm.jinqigufen.top

[T45] Perl：数组遍历
来源：http://jim.andypj.xyz

for my $x (@arr) { print $x; }
来源：http://pjl.smart0.xyz

[T46] Perl：哈希操作
来源：http://ibh.zhixingplan.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jfs.svipenyu.cn

[T47] Perl：正则捕获
来源：http://cdr.redwolf501.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://dne.gaohongyu789.top

[T48] Perl：正则替换
来源：http://iqu.xuetiantiany.cn

$s =~ s/old/new/g;
来源：http://nxe.smart0.xyz

[T49] Perl：函数
来源：http://xuu.shangyingyoupin.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fdc.aizwys.cn

[T50] Perl：逐行读文件
来源：http://hjl.zhengqikj.top

open my $fh, "<", "a.txt" or die $!;
来源：http://xhi.dashuyun.cn

while (my $line = <$fh>) { print $line; }
来源：http://gqk.dianchejie.cn

[T51] Scala：Hello World
来源：http://zgd.shanyushiyangtech.top

println("Hello")
来源：http://nwa.shanyushiyangtech.top

[T52] Scala：变量
来源：http://huv.chenlongwang.top

val a = 1;  var b = 2
来源：http://kxh.hammf.cn

[T53] Scala：字符串插值
来源：http://aan.ywan-chungtsiang.top

s"值: $b"
来源：http://wjh.zdqjudy.top

[T54] Scala：集合映射
来源：http://bwh.xylfe.cn

List(1, 2, 3).map(_ * 2)
来源：http://cbp.hnxiangtu.top

[T55] Scala：集合过滤
来源：http://ljf.zhongyouzk.top

List(1, 2, 3).filter(_ > 1)
来源：http://mwk.zhijiandao.cn

[T56] Scala：样例类
来源：http://wno.jqgufenzy.top

case class User(name: String, age: Int)
来源：http://pnu.kuanghao11.cn

[T57] Scala：模式匹配
来源：http://ate.birdmap.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://hds.mhx1999.top

[T58] Scala：函数定义
来源：http://bvk.jinghuilouyu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ugb.birdmap.top

[T59] Scala：循环
来源：http://dut.dianchejie.cn

for (i <- 1 to 10) println(i)
来源：http://vqb.jqgfzy.top

[T60] Scala：折叠
来源：http://bcl.52xcode.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bqt.jinqigufen.top

================================================================================
来源：http://oft.cqqwz.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vea.hammf.cn

================================================================================
来源：http://esh.yj202588.top

[U01] Py：创建虚拟环境
来源：http://olh.dianchejie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jke.fengsongda.top

[U02] Py：导出 / 安装依赖
来源：http://hqu.mhx1999.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jfj.zhijiandao.cn

[U03] Py：加载 .env 配置
来源：http://tdf.chenzaomai.com

from dotenv import load_dotenv; load_dotenv()
来源：http://qum.yuxming.cn

[U04] Py：变量调试打印
来源：http://vrq.ydjk.org.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jxl.xinyue.icu

[U05] Py：列表去重且保序
来源：http://gua.c1oappe.top

list(dict.fromkeys(arr))
来源：http://uns.cashguo.top

[U06] Py：合并两个字典
来源：http://xdg.daxiang520.top

{**a, **b}
来源：http://vsq.pengpengdd.cyou

[U07] Py：反转字典键值
来源：http://dze.nwbrower.top

{v: k for k, v in d.items()}
来源：http://snq.yueranfly.top

[U08] Py：展平二维列表
来源：http://juh.dashuyun.cn

[y for x in nested for y in x]
来源：http://pep.nwbrower.top

[U09] Py：字典取最大值的键
来源：http://zmw.pengpengdd.cyou

max(d, key=d.get)
来源：http://cdv.sufxvd.cn

[U10] Py：按值排序字典
来源：http://mll.uphjek.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ujc.hfpthk.cn

[U11] Py：生成器表达式
来源：http://cai.havefunace.top

(x * 2 for x in arr)
来源：http://sek.jianghu66.top

[U12] Py：取出现最多的 3 个元素
来源：http://rsv.aibaodan.cn

Counter(arr).most_common(3)
来源：http://zre.ydjk.org.cn

[U13] Py：固定长度队列
来源：http://cnx.gzhubu.top

deque(maxlen=10)
来源：http://qvl.vqdsnc.cn

[U14] Py：分组收集到列表
来源：http://dds.zhijiandao.cn

defaultdict(list)
来源：http://wil.dianchejie.cn

[U15] Py：高精度计时
来源：http://ruc.zycfv.cn

t = time.perf_counter()
来源：http://qco.hywenlv.cn

[U16] Py：命令行参数解析
来源：http://cgq.sweek.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zdz.vqdsnc.cn

[U17] Py：初始化日志
来源：http://rvi.jinqigufen.top

logging.basicConfig(level=logging.INFO)
来源：http://geh.zycfv.cn

[U18] Py：预编译正则
来源：http://cmd.shangyingyoupin.top

pat = re.compile(r"\d+")
来源：http://wah.vqdsnc.cn

[U19] Py：正则替换带回调
来源：http://sou.fehbvm.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yag.jinghuilouyu.cn

[U20] Py：缓存函数结果
来源：http://exd.52xcode.cn

@functools.lru_cache(maxsize=None)
来源：http://ceg.chenjidiqi.icu

[U21] Py：自定义上下文管理器
来源：http://yhh.snrcjt.cn

@contextlib.contextmanager
来源：http://wru.pycfn.com

[U22] Py：矩阵转置
来源：http://fvx.xingfuxueyuan.xyz

list(zip(*m))
来源：http://zrm.shangyingyoupin.top

[U23] Py：分块读取大文件
来源：http://rug.dashuyun.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mbq.jqgufenzy.top

[U24] Py：路径操作
来源：http://uml.xingfuxueyuan.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ipg.jiagoushi.top

[U25] Py：CSV 按字典读
来源：http://rub.316326.xyz

csv.DictReader(f)
来源：http://fye.redwolf501.top

[U26] Py：并发下载
来源：http://owc.iojbl.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ixn.vqdsnc.cn

[U27] Py：异步 HTTP
来源：http://ght.hammf.cn

aiohttp.ClientSession() 配合 async with
来源：http://sty.wangdashe.top

[U28] Py：类型别名
来源：http://wut.jinghuilouyu.cn

UserId = int
来源：http://ckf.zhoulong.xyz

[U29] Py：属性校验
来源：http://vuk.svipenyu.cn

@property 与 @x.setter 配合
来源：http://oru.zdbjq.cn

[U30] Py：数据类
来源：http://ywl.aibaodan.cn

@dataclass(slots=True)
来源：http://bpe.jqgfzy.top

[U31] Py：单测
来源：http://sat.xziqi.cn

python -m pytest -q
来源：http://mux.hfpthk.cn

[U32] Py：代码格式化
来源：http://zic.pycfn.com

ruff format . && ruff check --fix .
来源：http://kbi.ppjwa.cn

[U33] Py：打包发布
来源：http://vtb.fzhhl.top

python -m build  （依赖 pyproject.toml）
来源：http://giw.guowangkeji.top

[U34] Py：判断编码
来源：http://ajf.yonumen.top

chardet.detect(raw)
来源：http://xul.birdmap.top

[U35] Py：发送邮件
来源：http://tob.tarul.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://poo.cashguo.top

[U36] Py：定时任务
来源：http://zoh.shanyushiyangkeji.top

schedule.every(10).minutes.do(job)
来源：http://qna.cashguo.top


<!-- 参考信息 -->