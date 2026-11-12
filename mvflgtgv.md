代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jzf.hysaishi.cn

[S13] C：宏定义
来源：http://yqe.jianghu66.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gmy.wangshuangyany.cn

[S14] C：枚举
来源：http://lir.jinghuilouyu.cn

enum Color { RED, GREEN, BLUE };
来源：http://qdn.hammf.cn

[S15] C：类型转换
来源：http://knj.xuanzx.com

(double) a / b
来源：http://qtw.hysaishi.cn

[S16] C：位操作置位
来源：http://lhg.fktsv.cn

x |= (1 << 3);
来源：http://oxz.pengpengdd.cyou

[S17] C：安全拼接字符串
来源：http://noq.epnwcf.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mlu.nwbrower.top

[S18] C：命令行参数
来源：http://gll.jyoumei.cn

int main(int argc, char **argv)
来源：http://vzh.xylfe.cn

[S19] C：快速排序
来源：http://ina.hfpthk.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fwz.gaohongyu789.top

[S20] C：二分查找
来源：http://ykv.aibaodan.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://akj.mhx1999.top

[S21] C：字符类别判断
来源：http://fry.0kj1m.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gpk.gzhubu.top

[S22] C：字符串转数字
来源：http://esc.jiagoushi.top

atoi("42");  strtod("3.14", NULL);
来源：http://egf.zycfv.cn

[S23] C：随机数
来源：http://kyb.cheryme.top

srand(time(NULL));  int r = rand() % 100;
来源：http://wnb.tianlin.xyz

[S24] C：获取本地时间
来源：http://bbk.guannengcc.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nrw.hysaishi.cn

[S25] C：内存拷贝
来源：http://aub.cqqwz.cn

memcpy(dst, src, n);
来源：http://jvu.yueranfly.top

[S26] C：内存清零
来源：http://dhb.cucudq.cn

memset(a, 0, sizeof a);
来源：http://ioq.cqqwz.cn

[S27] C：定义常量
来源：http://hiz.tanke756.top

const double PI = 3.14159;
来源：http://iva.birdmap.top

[S28] C：静态变量
来源：http://dqu.fzhhl.top

static int counter = 0;
来源：http://pgz.jlsjyb.cn

[S29] C：变参函数
来源：http://pnf.daria6918.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://von.svipenyu.cn

[S30] C：头文件保护
来源：http://pnu.xuetiantiany.cn

#ifndef X_H
来源：http://ure.cdnleiting.top

#define X_H
来源：http://kgv.yuanzhike.top

#endif
来源：http://dfj.shzxlz.cn

[S31] C++：Hello World
来源：http://kzz.haohaochexian.top

#include <iostream>
来源：http://aem.chenlongwang.top

int main() { std::cout << "Hello\n"; }
来源：http://cks.jlsjyb.cn

[S32] C++：字符串
来源：http://elk.fzhhl.top

std::string s = "hi";  s += "!";
来源：http://jcf.smart0.xyz

[S33] C++：vector 增删
来源：http://fyh.jinyuanbaomall.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kup.jqgufenzy.top

[S34] C++：遍历 vector
来源：http://jgx.kuanghao11.cn

for (auto &x : v) { std::cout << x; }
来源：http://xjz.nanxuanxn.top

[S35] C++：map
来源：http://lki.gaohongyu789.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hrs.ydjk.org.cn

[S36] C++：unordered_map
来源：http://jjg.yanxiufei.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mog.xuetiantiany.cn

[S37] C++：set
来源：http://mkk.fanxiaobao.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dds.ydzc1.top

[S38] C++：排序
来源：http://cuj.wangdashe.top

std::sort(v.begin(), v.end());
来源：http://xwl.shangyingyoupin.top

[S39] C++：自定义比较器排序
来源：http://zni.yj202588.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://oke.zdqjudy.top

[S40] C++：查找元素
来源：http://jdz.andypj.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ttx.sufxvd.cn

[S41] C++：类与构造函数
来源：http://iqm.ywan-chungtsiang.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tte.hywenlv.cn

[S42] C++：继承与虚函数
来源：http://bxe.vqdsnc.cn

class B : public Base { public: void f() override {} };
来源：http://idx.jianghu66.top

[S43] C++：智能指针
来源：http://ete.ybcxt.top

auto p = std::make_unique<int>(5);
来源：http://ruk.zdqjudy.top

[S44] C++：引用传参
来源：http://exw.dianchejie.cn

void inc(int &x) { ++x; }
来源：http://ilk.aizwys.cn

[S45] C++：lambda
来源：http://vtj.ppjwa.cn

auto add = [](int a, int b) { return a + b; };
来源：http://evl.chenzaomai.com

[S46] C++：函数模板
来源：http://rau.ybcxt.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://oqs.hnxiangtu.top

[S47] C++：结构化绑定遍历
来源：http://jsa.jiagoushi.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dyy.iojbl.cn

[S48] C++：逐行读文件
来源：http://ldn.fktsv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://kfy.fzhhl.top

while (std::getline(in, line)) { }
来源：http://liq.tianlin.xyz

[S49] C++：写文件
来源：http://dmy.jianghu66.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lqk.hcnkem.com

[S50] C++：格式化数字
来源：http://brd.tarul.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hnx.cheryme.top

[S51] C++：显式类型转换
来源：http://dbs.gogol.net.cn

static_cast<double>(a) / b
来源：http://xjx.jinyuanbaomall.cn

[S52] C++：const 与 noexcept
来源：http://sli.0kj1m.cn

int size() const noexcept { return n_; }
来源：http://osn.ywan-chungtsiang.top

[S53] C++：移动语义
来源：http://hef.epnwcf.com

std::vector<int> w = std::move(v);
来源：http://ksr.xylfe.cn

[S54] C++：异常处理
来源：http://gnm.bbcook.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ygh.sweek.top

[S55] C++：结构化绑定
来源：http://gsa.dianchejie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://joi.wangdashe.top

[S56] C++：optional
来源：http://rnm.jqgfzy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gzz.sjlbkw.cn

[S57] C++：编译期常量
来源：http://hva.dianchejie.cn

constexpr int N = 10;
来源：http://eeo.redwolf501.top

[S58] C++：命名空间
来源：http://ase.redwolf501.top

namespace ns { int f() { return 1; } }
来源：http://gia.guannengcc.top

[S59] C++：静态断言
来源：http://fon.gaohongyu789.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ygz.smart0.xyz

[S60] C++：遍历并删除元素
来源：http://rjq.hesvh.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nfk.hesvh.cn

================================================================================
来源：http://cyc.fengsongda.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fvw.zhoulong.xyz

================================================================================
来源：http://ykh.jinqigfzy.top

[T01] Kotlin：Hello World
来源：http://pxu.smart0.xyz

println("Hello")
来源：http://hgx.daxiang520.top

[T02] Kotlin：变量
来源：http://mug.aizwys.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ymv.jianghu66.top

[T03] Kotlin：字符串模板
来源：http://vym.zhijiandao.cn

"值: $b"
来源：http://odd.jianghu66.top

[T04] Kotlin：空安全
来源：http://wlc.zycfv.cn

val n: String? = null;  n?.length
来源：http://ykd.ppjwa.cn

[T05] Kotlin：when 表达式
来源：http://yie.quarkkingdee.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vri.nanxinkj.top

[T06] Kotlin：集合映射
来源：http://sos.tianlin.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://mxr.gaohongyu789.top

[T07] Kotlin：集合过滤
来源：http://rbw.yj20258888.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://deo.bbcook.cn

[T08] Kotlin：数据类
来源：http://arx.ybcxt.top

data class User(val name: String, val age: Int)
来源：http://dto.sweek.top

[T09] Kotlin：扩展函数
来源：http://fef.meibo888.top

fun String.exclaim() = this + "!"
来源：http://mxe.chenzaomai.com

[T10] Kotlin：默认参数
来源：http://nnt.ehwqpu.com

fun greet(name: String = "World") = "Hi $name"
来源：http://hiu.sweek.top

[T11] Kotlin：协程
来源：http://ujv.aizwys.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://rjp.daxiang520.top

[T12] Kotlin：解构声明
来源：http://cog.fengsongda.top

val (a, b) = Pair(1, 2)
来源：http://lti.yj202588.top

[T13] Kotlin：只读 Map
来源：http://tej.xuetiantiany.cn

val m = mapOf("a" to 1)
来源：http://dkv.wangshuangyany.cn

[T14] Kotlin：循环
来源：http://phr.fehbvm.com

for (i in 1..10) println(i)
来源：http://hrx.gzhubu.top

[T15] Kotlin：接口
来源：http://ylx.yj202588.top

interface Shape { fun area(): Double }
来源：http://avb.gotoacloud.top

[T16] Swift：Hello World
来源：http://xno.nwbrower.top

print("Hello")
来源：http://ijm.yvedp.cn

[T17] Swift：变量与常量
来源：http://gur.hongshengwenyu.top

var a = 1;  let b = 2
来源：http://abp.jlsjyb.cn

[T18] Swift：字符串插值
来源：http://cic.9152youxi.cn

"值: \(b)"
来源：http://gdn.iojbl.cn

[T19] Swift：可选绑定
来源：http://ngq.yongpay.top

if let n = opt { print(n) }
来源：http://fhl.zycfv.cn

[T20] Swift：数组操作
来源：http://nbv.feifeiyinyue.top

var a = [1, 2, 3];  a.append(4)
来源：http://kyg.chenjidiqi.icu

[T21] Swift：遍历
来源：http://nnp.fktsv.cn

for x in a { print(x) }
来源：http://vne.sjlbkw.cn

[T22] Swift：字典
来源：http://cka.jiagoushi.top

var d = ["a": 1];  d["b"] = 2
来源：http://eix.fzhhl.top

[T23] Swift：函数
来源：http://ate.yonumen.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://erp.epnwcf.com

[T24] Swift：闭包
来源：http://sun.daria6918.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://cze.nanxinkj.top

[T25] Swift：结构体
来源：http://bzt.jinyuanbaomall.cn

struct P { var x: Int }
来源：http://jin.xuanzx.com

[T26] Swift：类与重写
来源：http://sdr.52xcode.cn

class A: Base { override func f() {} }
来源：http://jgu.sjlbkw.cn

[T27] Swift：错误处理
来源：http://jfj.sweek.top

do { try f() } catch { print(error) }
来源：http://phi.cheryme.top

[T28] Swift：枚举
来源：http://fqv.xylfe.cn

enum Color { case red, green }
来源：http://lwd.ppjwa.cn

[T29] Swift：guard 提前返回
来源：http://hut.cashguo.top

guard let x = opt else { return }
来源：http://zau.ppjwa.cn

[T30] Swift：协议
来源：http://owq.zhixingplan.top

protocol Shape { func area() -> Double }
来源：http://gcq.ydzc1.top

[T31] Lua：Hello World
来源：http://flm.yj20258888.top

print("Hello")
来源：http://ymx.jinqigfzy.top

[T32] Lua：局部变量
来源：http://ftr.daria6918.cn

local a = 1
来源：http://hqe.jinqigufen.top

[T33] Lua：表（数组）
来源：http://ezj.jiagoushi.top

local t = {1, 2, 3};  t[4] = 4
来源：http://mhj.xylfe.cn

[T34] Lua：遍历表
来源：http://jma.hfpthk.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://eyi.smart0.xyz

[T35] Lua：字典表
来源：http://hus.xuetiantiany.cn

local d = { a = 1 };  d.b = 2
来源：http://iuk.316326.xyz

[T36] Lua：函数
来源：http://epo.dashuyun.cn

function add(a, b) return a + b end
来源：http://hcj.chenjidiqi.icu

[T37] Lua：字符串拼接
来源：http://arc.9152youxi.cn

"a" .. "b"
来源：http://hpf.yvedp.cn

[T38] Lua：条件
来源：http://dtp.fktsv.cn

if x > 0 then print("正") end
来源：http://kwh.gotoacloud.top

[T39] Lua：模式匹配
来源：http://ipp.yuxming.cn

string.find(s, "%d+")
来源：http://liu.havefunace.top

[T40] Lua：元表
来源：http://ava.aibaodan.cn

setmetatable({}, { __index = base })
来源：http://pya.xuanzx.com

[T41] Perl：Hello World
来源：http://zcx.tanke756.top

print "Hello\n";
来源：http://yzj.nwbrower.top

[T42] Perl：变量类型
来源：http://sye.cashguo.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wjg.chenzaomai.com

[T43] Perl：字符串插值
来源：http://gip.tanke756.top

"值: $a"
来源：http://clm.aizwys.cn

[T44] Perl：条件
来源：http://ovw.ywan-chungtsiang.top

if ($a > 0) { print "正"; }
来源：http://qqw.xuetiantiany.cn

[T45] Perl：数组遍历
来源：http://pkb.guowangkeji.top

for my $x (@arr) { print $x; }
来源：http://vmc.sysykeji.top

[T46] Perl：哈希操作
来源：http://ike.vqdsnc.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dcs.jinghuilouyu.cn

[T47] Perl：正则捕获
来源：http://mug.smart0.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://ulx.sjlbkw.cn

[T48] Perl：正则替换
来源：http://zra.guannengcc.top

$s =~ s/old/new/g;
来源：http://isc.quarkkingdee.top

[T49] Perl：函数
来源：http://eyj.hysaishi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jhi.zdbjq.cn

[T50] Perl：逐行读文件
来源：http://zfr.sweek.top

open my $fh, "<", "a.txt" or die $!;
来源：http://tbf.tarul.cn

while (my $line = <$fh>) { print $line; }
来源：http://bco.fktsv.cn

[T51] Scala：Hello World
来源：http://gtr.ehwqpu.com

println("Hello")
来源：http://srg.vqdsnc.cn

[T52] Scala：变量
来源：http://mwp.xuanzx.com

val a = 1;  var b = 2
来源：http://ybg.ywan-chungtsiang.top

[T53] Scala：字符串插值
来源：http://qys.ehwqpu.com

s"值: $b"
来源：http://zad.yangfankeji.com

[T54] Scala：集合映射
来源：http://leo.aibaodan.cn

List(1, 2, 3).map(_ * 2)
来源：http://vux.havefunace.top

[T55] Scala：集合过滤
来源：http://qla.cucudq.cn

List(1, 2, 3).filter(_ > 1)
来源：http://pzw.chenzaomai.com

[T56] Scala：样例类
来源：http://qfa.sweek.top

case class User(name: String, age: Int)
来源：http://kvr.zhengqikj.top

[T57] Scala：模式匹配
来源：http://gdt.hongshengwenyu.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://obk.gaohongyu789.top

[T58] Scala：函数定义
来源：http://gqs.wangdashe.top

def add(a: Int, b: Int): Int = a + b
来源：http://kin.gogol.net.cn

[T59] Scala：循环
来源：http://cjl.dashuyun.cn

for (i <- 1 to 10) println(i)
来源：http://ans.aibaodan.cn

[T60] Scala：折叠
来源：http://kuu.yanxiufei.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xpz.tarul.cn

================================================================================
来源：http://bml.yongpay.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hek.xuetiantiany.cn

================================================================================
来源：http://zyh.zdqjudy.top

[U01] Py：创建虚拟环境
来源：http://sfy.ehwqpu.com

python -m venv .venv && source .venv/bin/activate
来源：http://hhd.hammf.cn

[U02] Py：导出 / 安装依赖
来源：http://tny.haohaochexian.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://igk.shzxlz.cn

[U03] Py：加载 .env 配置
来源：http://btv.jinyuanbaomall.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://fbf.chenzaomai.com

[U04] Py：变量调试打印
来源：http://eig.fengsongda.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wsa.nanxinkj.top

[U05] Py：列表去重且保序
来源：http://uku.zhiwuduotai.top

list(dict.fromkeys(arr))
来源：http://jrl.nanxinkj.top

[U06] Py：合并两个字典
来源：http://gof.ivvv.top

{**a, **b}
来源：http://oxg.sxryk.cn

[U07] Py：反转字典键值
来源：http://pay.svipenyu.cn

{v: k for k, v in d.items()}
来源：http://ooq.kuanghao11.cn

[U08] Py：展平二维列表
来源：http://yha.vehdjk.com

[y for x in nested for y in x]
来源：http://iiy.dianchejie.cn

[U09] Py：字典取最大值的键
来源：http://xbf.tarul.cn

max(d, key=d.get)
来源：http://xfd.tarul.cn

[U10] Py：按值排序字典
来源：http://mcc.yuanzhike.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jwl.c1oappe.top

[U11] Py：生成器表达式
来源：http://bcz.yonumen.top

(x * 2 for x in arr)
来源：http://sju.chenlongwang.top

[U12] Py：取出现最多的 3 个元素
来源：http://xnr.bbcook.cn

Counter(arr).most_common(3)
来源：http://myk.guannengcc.top

[U13] Py：固定长度队列
来源：http://iqu.xylfe.cn

deque(maxlen=10)
来源：http://thj.zdbjq.cn

[U14] Py：分组收集到列表
来源：http://edf.sysykeji.top

defaultdict(list)
来源：http://lpw.ppjwa.cn

[U15] Py：高精度计时
来源：http://nyx.tarul.cn

t = time.perf_counter()
来源：http://xqz.daxiang520.top

[U16] Py：命令行参数解析
来源：http://gsi.ydjk.org.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://smc.ywan-chungtsiang.top

[U17] Py：初始化日志
来源：http://hsf.xylfe.cn

logging.basicConfig(level=logging.INFO)
来源：http://qmn.bbcook.cn

[U18] Py：预编译正则
来源：http://icb.hongshengwenyu.top

pat = re.compile(r"\d+")
来源：http://buo.chenjidiqi.icu

[U19] Py：正则替换带回调
来源：http://dtc.smart0.xyz

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://jnm.nanxuanxn.top

[U20] Py：缓存函数结果
来源：http://hxt.jinqigfzy.top

@functools.lru_cache(maxsize=None)
来源：http://qfd.yongpay.top

[U21] Py：自定义上下文管理器
来源：http://qja.jyoumei.cn

@contextlib.contextmanager
来源：http://zjb.jinqigufen.top

[U22] Py：矩阵转置
来源：http://nny.dashuyun.cn

list(zip(*m))
来源：http://aha.zycfv.cn

[U23] Py：分块读取大文件
来源：http://qbo.zhiwuduotai.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ksg.chenjidiqi.icu

[U24] Py：路径操作
来源：http://vuz.bjfxy.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ghz.shangyingyoupin.top

[U25] Py：CSV 按字典读
来源：http://oxz.bjfxy.top

csv.DictReader(f)
来源：http://bgo.gotoacloud.top

[U26] Py：并发下载
来源：http://oga.redwolf501.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pcg.cqqwz.cn

[U27] Py：异步 HTTP
来源：http://ois.jianghu66.top

aiohttp.ClientSession() 配合 async with
来源：http://coh.nwbrower.top

[U28] Py：类型别名
来源：http://erc.gogol.net.cn

UserId = int
来源：http://rto.yuxming.cn

[U29] Py：属性校验
来源：http://rku.nwbrower.top

@property 与 @x.setter 配合
来源：http://tiu.epnwcf.com

[U30] Py：数据类
来源：http://don.wangshuangyany.cn

@dataclass(slots=True)
来源：http://yfo.dianchejie.cn

[U31] Py：单测
来源：http://fks.aibaodan.cn

python -m pytest -q
来源：http://yjc.sysykeji.top

[U32] Py：代码格式化
来源：http://ayt.hongshengwenyu.top

ruff format . && ruff check --fix .
来源：http://zak.zhoulong.xyz

[U33] Py：打包发布
来源：http://lle.zdqjudy.top

python -m build  （依赖 pyproject.toml）
来源：http://ggr.jinghuilouyu.cn

[U34] Py：判断编码
来源：http://swx.kuanghao11.cn

chardet.detect(raw)
来源：http://wsl.shanyushiyangtech.top

[U35] Py：发送邮件
来源：http://rnb.redwolf501.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qpx.zhongyouzk.top

[U36] Py：定时任务
来源：http://kwk.hnxiangtu.top

schedule.every(10).minutes.do(job)
来源：http://wsc.sysykeji.top


<!-- 参考信息 -->