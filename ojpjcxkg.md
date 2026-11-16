代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://oyq.uphjek.com

[S13] C：宏定义
来源：http://sqe.ydjk.org.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ycu.redwolf501.top

[S14] C：枚举
来源：http://wrt.0kj1m.cn

enum Color { RED, GREEN, BLUE };
来源：http://bmr.haohaochexian.top

[S15] C：类型转换
来源：http://imz.ydjk.org.cn

(double) a / b
来源：http://soz.tarul.cn

[S16] C：位操作置位
来源：http://kzz.fzhhl.top

x |= (1 << 3);
来源：http://tia.ehwqpu.com

[S17] C：安全拼接字符串
来源：http://qsr.yuxming.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gpb.hnqzz.top

[S18] C：命令行参数
来源：http://dwf.yangfankeji.com

int main(int argc, char **argv)
来源：http://kpt.fanxiaobao.xyz

[S19] C：快速排序
来源：http://uqw.shanyushiyangkeji.top

qsort(a, n, sizeof(int), cmp);
来源：http://aou.guannengcc.top

[S20] C：二分查找
来源：http://qbh.hnxiangtu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qws.c1oappe.top

[S21] C：字符类别判断
来源：http://dlu.bjfxy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sni.zhaomingkeji.xyz

[S22] C：字符串转数字
来源：http://mqi.shanyushiyangtech.top

atoi("42");  strtod("3.14", NULL);
来源：http://qyx.yuxming.cn

[S23] C：随机数
来源：http://cho.yvedp.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qrd.yj20258.top

[S24] C：获取本地时间
来源：http://pgr.yueranfly.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pht.shangyingyoupin.top

[S25] C：内存拷贝
来源：http://rtk.cdnleiting.top

memcpy(dst, src, n);
来源：http://tzj.zhengqikj.top

[S26] C：内存清零
来源：http://wdd.uphjek.com

memset(a, 0, sizeof a);
来源：http://akk.meibo888.top

[S27] C：定义常量
来源：http://laj.xylfe.cn

const double PI = 3.14159;
来源：http://ptd.xinyue.icu

[S28] C：静态变量
来源：http://spr.sysykeji.top

static int counter = 0;
来源：http://suy.yueranfly.top

[S29] C：变参函数
来源：http://ask.chenzaomai.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jys.sysykeji.top

[S30] C：头文件保护
来源：http://hne.cheryme.top

#ifndef X_H
来源：http://ykr.redwolf501.top

#define X_H
来源：http://jvq.fanxiaobao.xyz

#endif
来源：http://mpy.tarul.cn

[S31] C++：Hello World
来源：http://dkv.daria6918.cn

#include <iostream>
来源：http://skb.xingfuxueyuan.xyz

int main() { std::cout << "Hello\n"; }
来源：http://cml.jyoumei.cn

[S32] C++：字符串
来源：http://xxq.chenlongwang.top

std::string s = "hi";  s += "!";
来源：http://boh.gaohongyu789.top

[S33] C++：vector 增删
来源：http://vrk.cheryme.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://grf.jiagoushi.top

[S34] C++：遍历 vector
来源：http://apd.zycfv.cn

for (auto &x : v) { std::cout << x; }
来源：http://xxv.shangyingyoupin.top

[S35] C++：map
来源：http://mzw.yangfankeji.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ywt.hnqzz.top

[S36] C++：unordered_map
来源：http://cxw.xuanzx.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ouw.yuxming.cn

[S37] C++：set
来源：http://php.aizwys.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qdy.ppjwa.cn

[S38] C++：排序
来源：http://rkq.yuxming.cn

std::sort(v.begin(), v.end());
来源：http://rad.hfpthk.cn

[S39] C++：自定义比较器排序
来源：http://pcr.redwolf501.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kxy.tianlin.xyz

[S40] C++：查找元素
来源：http://bme.svipenyu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xsn.aizwys.cn

[S41] C++：类与构造函数
来源：http://dqj.zycfv.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dww.dianchejie.cn

[S42] C++：继承与虚函数
来源：http://hzb.zycfv.cn

class B : public Base { public: void f() override {} };
来源：http://lwi.hongshengwenyu.top

[S43] C++：智能指针
来源：http://hwe.ydzc1.top

auto p = std::make_unique<int>(5);
来源：http://xhu.hesvh.cn

[S44] C++：引用传参
来源：http://gzt.xuanzx.com

void inc(int &x) { ++x; }
来源：http://phy.jinqigufen.top

[S45] C++：lambda
来源：http://dtz.chenjidiqi.icu

auto add = [](int a, int b) { return a + b; };
来源：http://cww.hysaishi.cn

[S46] C++：函数模板
来源：http://tzl.jqgufenzy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fvv.nanxinkj.top

[S47] C++：结构化绑定遍历
来源：http://wcz.jinqigufen.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://awb.wangdashe.top

[S48] C++：逐行读文件
来源：http://drk.xuanzx.com

std::ifstream in("a.txt");  std::string line;
来源：http://wdm.hnqzz.top

while (std::getline(in, line)) { }
来源：http://utn.hongshengwenyu.top

[S49] C++：写文件
来源：http://xsf.epnwcf.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://alc.quarkkingdee.top

[S50] C++：格式化数字
来源：http://xvk.dianchejie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ukx.jqgufenzy.top

[S51] C++：显式类型转换
来源：http://vrh.tarul.cn

static_cast<double>(a) / b
来源：http://yib.sweek.top

[S52] C++：const 与 noexcept
来源：http://sho.xylfe.cn

int size() const noexcept { return n_; }
来源：http://ojc.hfpthk.cn

[S53] C++：移动语义
来源：http://nyc.sjlbkw.cn

std::vector<int> w = std::move(v);
来源：http://kzw.fktsv.cn

[S54] C++：异常处理
来源：http://irm.snrcjt.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fae.xziqi.cn

[S55] C++：结构化绑定
来源：http://zwa.yangfankeji.com

auto [a, b] = std::make_pair(1, 2);
来源：http://fmz.jinyuanbaomall.cn

[S56] C++：optional
来源：http://lua.cucudq.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tfe.hnxiangtu.top

[S57] C++：编译期常量
来源：http://gmx.chenjidiqi.icu

constexpr int N = 10;
来源：http://zol.hnqzz.top

[S58] C++：命名空间
来源：http://yrh.tian-w.cn

namespace ns { int f() { return 1; } }
来源：http://qzs.xuanzx.com

[S59] C++：静态断言
来源：http://cvc.ybcxt.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ltj.gzhubu.top

[S60] C++：遍历并删除元素
来源：http://kqd.vehdjk.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dbo.ivvv.top

================================================================================
来源：http://qzg.zdbjq.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://eog.316326.xyz

================================================================================
来源：http://zrb.sxryk.cn

[T01] Kotlin：Hello World
来源：http://iai.andypj.xyz

println("Hello")
来源：http://hfw.aibaodan.cn

[T02] Kotlin：变量
来源：http://jiy.zhaomingkeji.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gsd.yongpay.top

[T03] Kotlin：字符串模板
来源：http://llr.havefunace.top

"值: $b"
来源：http://qnb.pycfn.com

[T04] Kotlin：空安全
来源：http://vsa.zhixingplan.top

val n: String? = null;  n?.length
来源：http://oht.shanyushiyangtech.top

[T05] Kotlin：when 表达式
来源：http://hev.ywan-chungtsiang.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://iti.zhixingplan.top

[T06] Kotlin：集合映射
来源：http://boo.bjfxy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://buh.yangfankeji.com

[T07] Kotlin：集合过滤
来源：http://rnz.chenjidiqi.icu

listOf(1, 2, 3).filter { it > 1 }
来源：http://tjx.ehwqpu.com

[T08] Kotlin：数据类
来源：http://urd.fanxiaobao.xyz

data class User(val name: String, val age: Int)
来源：http://opj.xziqi.cn

[T09] Kotlin：扩展函数
来源：http://mke.yangfankeji.com

fun String.exclaim() = this + "!"
来源：http://arm.birdmap.top

[T10] Kotlin：默认参数
来源：http://jau.zhongyouzk.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ecz.cdnleiting.top

[T11] Kotlin：协程
来源：http://rqi.iojbl.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://pts.gzhubu.top

[T12] Kotlin：解构声明
来源：http://ofx.jqgfzy.top

val (a, b) = Pair(1, 2)
来源：http://fie.nanxuanxn.top

[T13] Kotlin：只读 Map
来源：http://qtl.redwolf501.top

val m = mapOf("a" to 1)
来源：http://ako.vqdsnc.cn

[T14] Kotlin：循环
来源：http://cik.uphjek.com

for (i in 1..10) println(i)
来源：http://axi.ctjpmb.com

[T15] Kotlin：接口
来源：http://yzz.9152youxi.cn

interface Shape { fun area(): Double }
来源：http://djl.chenlongwang.top

[T16] Swift：Hello World
来源：http://yyk.xinyue.icu

print("Hello")
来源：http://esa.feifeiyinyue.top

[T17] Swift：变量与常量
来源：http://ygc.jqgufenzy.top

var a = 1;  let b = 2
来源：http://pau.yuanzhike.top

[T18] Swift：字符串插值
来源：http://uhz.tianlin.xyz

"值: \(b)"
来源：http://xhm.sxryk.cn

[T19] Swift：可选绑定
来源：http://det.bjfxy.top

if let n = opt { print(n) }
来源：http://dzo.yonumen.top

[T20] Swift：数组操作
来源：http://fss.iojbl.cn

var a = [1, 2, 3];  a.append(4)
来源：http://dek.vqdsnc.cn

[T21] Swift：遍历
来源：http://dan.zhiwuduotai.top

for x in a { print(x) }
来源：http://rwt.316326.xyz

[T22] Swift：字典
来源：http://myh.sufxvd.cn

var d = ["a": 1];  d["b"] = 2
来源：http://gnq.sweek.top

[T23] Swift：函数
来源：http://pgi.jinyuanbaomall.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vrx.shzxlz.cn

[T24] Swift：闭包
来源：http://mex.haohaochexian.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ipf.dashuyun.cn

[T25] Swift：结构体
来源：http://fks.wangshuangyany.cn

struct P { var x: Int }
来源：http://wtd.daxiang520.top

[T26] Swift：类与重写
来源：http://ncp.shangyingyoupin.top

class A: Base { override func f() {} }
来源：http://feo.zycfv.cn

[T27] Swift：错误处理
来源：http://tuf.zdbjq.cn

do { try f() } catch { print(error) }
来源：http://ctq.hfpthk.cn

[T28] Swift：枚举
来源：http://ztx.jyoumei.cn

enum Color { case red, green }
来源：http://abt.daria6918.cn

[T29] Swift：guard 提前返回
来源：http://ons.yonumen.top

guard let x = opt else { return }
来源：http://xix.jianghu66.top

[T30] Swift：协议
来源：http://wfy.birdmap.top

protocol Shape { func area() -> Double }
来源：http://egm.316326.xyz

[T31] Lua：Hello World
来源：http://dhi.shanyushiyangtech.top

print("Hello")
来源：http://rhw.9152youxi.cn

[T32] Lua：局部变量
来源：http://ufp.316326.xyz

local a = 1
来源：http://mdf.yuanzhike.top

[T33] Lua：表（数组）
来源：http://mhy.tianlin.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://yjb.xziqi.cn

[T34] Lua：遍历表
来源：http://nvu.hesvh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ahv.ydzc1.top

[T35] Lua：字典表
来源：http://wle.tarul.cn

local d = { a = 1 };  d.b = 2
来源：http://fys.guowangkeji.top

[T36] Lua：函数
来源：http://xai.jqgufenzy.top

function add(a, b) return a + b end
来源：http://tgs.zhengqikj.top

[T37] Lua：字符串拼接
来源：http://hqg.guannengcc.top

"a" .. "b"
来源：http://uxf.yj202588.top

[T38] Lua：条件
来源：http://vrf.hcnkem.com

if x > 0 then print("正") end
来源：http://hpd.sweek.top

[T39] Lua：模式匹配
来源：http://nds.bbcook.cn

string.find(s, "%d+")
来源：http://yda.haohaochexian.top

[T40] Lua：元表
来源：http://mmv.yvedp.cn

setmetatable({}, { __index = base })
来源：http://ilu.zhixingplan.top

[T41] Perl：Hello World
来源：http://wnc.xziqi.cn

print "Hello\n";
来源：http://qos.fehbvm.com

[T42] Perl：变量类型
来源：http://njw.9152youxi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dkr.daria6918.cn

[T43] Perl：字符串插值
来源：http://wty.fktsv.cn

"值: $a"
来源：http://rwy.yj20258888.top

[T44] Perl：条件
来源：http://sxb.hnxiangtu.top

if ($a > 0) { print "正"; }
来源：http://ujd.vqdsnc.cn

[T45] Perl：数组遍历
来源：http://ksy.xylfe.cn

for my $x (@arr) { print $x; }
来源：http://nmt.wangdashe.top

[T46] Perl：哈希操作
来源：http://ykn.xylfe.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hga.zhixingplan.top

[T47] Perl：正则捕获
来源：http://bcc.gaohongyu789.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://hgu.zhiwuduotai.top

[T48] Perl：正则替换
来源：http://ahu.zhijiandao.cn

$s =~ s/old/new/g;
来源：http://ijj.meibo888.top

[T49] Perl：函数
来源：http://qmc.yfazqb.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cmg.9152youxi.cn

[T50] Perl：逐行读文件
来源：http://qac.yueranfly.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ugp.tanke756.top

while (my $line = <$fh>) { print $line; }
来源：http://psy.hywenlv.cn

[T51] Scala：Hello World
来源：http://wyl.xziqi.cn

println("Hello")
来源：http://dsj.cashguo.top

[T52] Scala：变量
来源：http://ecc.yuxming.cn

val a = 1;  var b = 2
来源：http://lar.fzhhl.top

[T53] Scala：字符串插值
来源：http://tul.zhiwuduotai.top

s"值: $b"
来源：http://kaa.xziqi.cn

[T54] Scala：集合映射
来源：http://qep.xuetiantiany.cn

List(1, 2, 3).map(_ * 2)
来源：http://amv.fktsv.cn

[T55] Scala：集合过滤
来源：http://rpc.yonumen.top

List(1, 2, 3).filter(_ > 1)
来源：http://sgc.shuidangran.top

[T56] Scala：样例类
来源：http://xtd.jianghu66.top

case class User(name: String, age: Int)
来源：http://wkc.iojbl.cn

[T57] Scala：模式匹配
来源：http://ktu.jinqigufen.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://fwt.cheryme.top

[T58] Scala：函数定义
来源：http://utx.mhx1999.top

def add(a: Int, b: Int): Int = a + b
来源：http://lyj.fehbvm.com

[T59] Scala：循环
来源：http://wla.bjfxy.top

for (i <- 1 to 10) println(i)
来源：http://hzv.nanxinkj.top

[T60] Scala：折叠
来源：http://mav.nanxinkj.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fit.cucudq.cn

================================================================================
来源：http://kku.zdbjq.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mxf.jqgfzy.top

================================================================================
来源：http://bnj.ydzc1.top

[U01] Py：创建虚拟环境
来源：http://umq.zhoulong.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://aeq.zhongyouzk.top

[U02] Py：导出 / 安装依赖
来源：http://hsz.yj20258888.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://edf.zhengqikj.top

[U03] Py：加载 .env 配置
来源：http://tpj.jiagoushi.top

from dotenv import load_dotenv; load_dotenv()
来源：http://knt.0kj1m.cn

[U04] Py：变量调试打印
来源：http://bpo.cucudq.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://bsq.xylfe.cn

[U05] Py：列表去重且保序
来源：http://vzi.jinqigfzy.top

list(dict.fromkeys(arr))
来源：http://gfh.xinyue.icu

[U06] Py：合并两个字典
来源：http://cya.epnwcf.com

{**a, **b}
来源：http://dsv.xziqi.cn

[U07] Py：反转字典键值
来源：http://jpw.xziqi.cn

{v: k for k, v in d.items()}
来源：http://nie.shangyingyoupin.top

[U08] Py：展平二维列表
来源：http://oiz.vehdjk.com

[y for x in nested for y in x]
来源：http://pob.zdqjudy.top

[U09] Py：字典取最大值的键
来源：http://yxf.cheryme.top

max(d, key=d.get)
来源：http://yrj.zycfv.cn

[U10] Py：按值排序字典
来源：http://zus.wangdashe.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zlf.sweek.top

[U11] Py：生成器表达式
来源：http://ehe.ywan-chungtsiang.top

(x * 2 for x in arr)
来源：http://gfx.ivvv.top

[U12] Py：取出现最多的 3 个元素
来源：http://kuu.daxiang520.top

Counter(arr).most_common(3)
来源：http://ngf.guowangkeji.top

[U13] Py：固定长度队列
来源：http://ndi.chenzaomai.com

deque(maxlen=10)
来源：http://hpo.hesvh.cn

[U14] Py：分组收集到列表
来源：http://dub.hongshengwenyu.top

defaultdict(list)
来源：http://qpn.bbcook.cn

[U15] Py：高精度计时
来源：http://coh.gzhubu.top

t = time.perf_counter()
来源：http://beu.dashuyun.cn

[U16] Py：命令行参数解析
来源：http://ukh.zhijiandao.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qkv.ydjk.org.cn

[U17] Py：初始化日志
来源：http://jmp.yangfankeji.com

logging.basicConfig(level=logging.INFO)
来源：http://vro.yanxiufei.cn

[U18] Py：预编译正则
来源：http://pmd.ppjwa.cn

pat = re.compile(r"\d+")
来源：http://zba.hammf.cn

[U19] Py：正则替换带回调
来源：http://cfo.yangfankeji.com

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lsc.zhengqikj.top

[U20] Py：缓存函数结果
来源：http://eeq.hysaishi.cn

@functools.lru_cache(maxsize=None)
来源：http://nsz.yfazqb.com

[U21] Py：自定义上下文管理器
来源：http://xkh.nanxinkj.top

@contextlib.contextmanager
来源：http://jcj.hammf.cn

[U22] Py：矩阵转置
来源：http://buq.vqdsnc.cn

list(zip(*m))
来源：http://fys.zhongyouzk.top

[U23] Py：分块读取大文件
来源：http://xwu.316326.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://arg.chenlongwang.top

[U24] Py：路径操作
来源：http://saa.yonumen.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://gje.sysykeji.top

[U25] Py：CSV 按字典读
来源：http://mix.svipenyu.cn

csv.DictReader(f)
来源：http://idw.shuidangran.top

[U26] Py：并发下载
来源：http://nly.daxiang520.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fqv.cqqwz.cn

[U27] Py：异步 HTTP
来源：http://oio.hnxiangtu.top

aiohttp.ClientSession() 配合 async with
来源：http://mus.nanxinkj.top

[U28] Py：类型别名
来源：http://ach.pengpengdd.cyou

UserId = int
来源：http://ffy.hcnkem.com

[U29] Py：属性校验
来源：http://iks.jinyuanbaomall.cn

@property 与 @x.setter 配合
来源：http://ihr.chenjidiqi.icu

[U30] Py：数据类
来源：http://djz.bbcook.cn

@dataclass(slots=True)
来源：http://fys.xylfe.cn

[U31] Py：单测
来源：http://krj.kuanghao11.cn

python -m pytest -q
来源：http://quj.hammf.cn

[U32] Py：代码格式化
来源：http://bnp.yueranfly.top

ruff format . && ruff check --fix .
来源：http://czz.9152youxi.cn

[U33] Py：打包发布
来源：http://kth.tian-w.cn

python -m build  （依赖 pyproject.toml）
来源：http://blh.mhx1999.top

[U34] Py：判断编码
来源：http://djd.vqdsnc.cn

chardet.detect(raw)
来源：http://sxt.aibaodan.cn

[U35] Py：发送邮件
来源：http://niq.xuanzx.com

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://npx.gzhubu.top

[U36] Py：定时任务
来源：http://xbk.vqdsnc.cn

schedule.every(10).minutes.do(job)
来源：http://oez.shangyingyoupin.top


<!-- 参考信息 -->