代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://jpp.hnxiangtu.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://lii.nanxinkj.top

fclose(f);
来源：http://sps.zdqjudy.top

[S12] C：写文件
来源：http://brm.chenlongwang.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rxc.ehwqpu.com

[S13] C：宏定义
来源：http://bhk.andypj.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ter.ydzc1.top

[S14] C：枚举
来源：http://zql.jyoumei.cn

enum Color { RED, GREEN, BLUE };
来源：http://rxp.yj202588.top

[S15] C：类型转换
来源：http://qwd.yongpay.top

(double) a / b
来源：http://ztn.hammf.cn

[S16] C：位操作置位
来源：http://qhg.316326.xyz

x |= (1 << 3);
来源：http://zix.cashguo.top

[S17] C：安全拼接字符串
来源：http://hxc.haohaochexian.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ueg.yj20258888.top

[S18] C：命令行参数
来源：http://ylf.hesvh.cn

int main(int argc, char **argv)
来源：http://gky.hesvh.cn

[S19] C：快速排序
来源：http://rys.bjfxy.top

qsort(a, n, sizeof(int), cmp);
来源：http://zbf.xingfuxueyuan.xyz

[S20] C：二分查找
来源：http://xoc.zhongyouzk.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vqx.guowangkeji.top

[S21] C：字符类别判断
来源：http://ppr.sweek.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xac.cashguo.top

[S22] C：字符串转数字
来源：http://qzs.jqgufenzy.top

atoi("42");  strtod("3.14", NULL);
来源：http://ine.andypj.xyz

[S23] C：随机数
来源：http://qzv.gzhubu.top

srand(time(NULL));  int r = rand() % 100;
来源：http://cue.quarkkingdee.top

[S24] C：获取本地时间
来源：http://tou.uphjek.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gcn.zhixingplan.top

[S25] C：内存拷贝
来源：http://khi.hammf.cn

memcpy(dst, src, n);
来源：http://bju.hnxiangtu.top

[S26] C：内存清零
来源：http://qca.hnqzz.top

memset(a, 0, sizeof a);
来源：http://uhr.gzhubu.top

[S27] C：定义常量
来源：http://onf.tanke756.top

const double PI = 3.14159;
来源：http://hqs.tian-w.cn

[S28] C：静态变量
来源：http://lte.ydzc1.top

static int counter = 0;
来源：http://fod.hfpthk.cn

[S29] C：变参函数
来源：http://bpj.cdnleiting.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dlx.cdnleiting.top

[S30] C：头文件保护
来源：http://xch.zdqjudy.top

#ifndef X_H
来源：http://pxa.guannengcc.top

#define X_H
来源：http://hoa.hfpthk.cn

#endif
来源：http://zcj.pycfn.com

[S31] C++：Hello World
来源：http://ovt.guowangkeji.top

#include <iostream>
来源：http://dma.yj202588.top

int main() { std::cout << "Hello\n"; }
来源：http://gcg.zhaomingkeji.xyz

[S32] C++：字符串
来源：http://ngv.xuanzx.com

std::string s = "hi";  s += "!";
来源：http://lmn.yonumen.top

[S33] C++：vector 增删
来源：http://oek.ywan-chungtsiang.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://low.cucudq.cn

[S34] C++：遍历 vector
来源：http://rqo.hfpthk.cn

for (auto &x : v) { std::cout << x; }
来源：http://wci.nanxuanxn.top

[S35] C++：map
来源：http://phs.gzhubu.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hkk.uphjek.com

[S36] C++：unordered_map
来源：http://ehh.sjlbkw.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rrz.zhongyouzk.top

[S37] C++：set
来源：http://wdz.mhx1999.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vfv.pycfn.com

[S38] C++：排序
来源：http://pyo.jinyuanbaomall.cn

std::sort(v.begin(), v.end());
来源：http://lpo.redwolf501.top

[S39] C++：自定义比较器排序
来源：http://gog.chenzaomai.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ysm.xinyue.icu

[S40] C++：查找元素
来源：http://uzg.zhixingplan.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dqy.quarkkingdee.top

[S41] C++：类与构造函数
来源：http://nai.hongshengwenyu.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bxg.gotoacloud.top

[S42] C++：继承与虚函数
来源：http://cuo.xuetiantiany.cn

class B : public Base { public: void f() override {} };
来源：http://ysk.zhiwuduotai.top

[S43] C++：智能指针
来源：http://huq.316326.xyz

auto p = std::make_unique<int>(5);
来源：http://zcg.cucudq.cn

[S44] C++：引用传参
来源：http://fzy.iojbl.cn

void inc(int &x) { ++x; }
来源：http://pdy.quarkkingdee.top

[S45] C++：lambda
来源：http://djb.fehbvm.com

auto add = [](int a, int b) { return a + b; };
来源：http://lrb.jianghu66.top

[S46] C++：函数模板
来源：http://dfj.sysykeji.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cbj.cucudq.cn

[S47] C++：结构化绑定遍历
来源：http://wup.zhiwuduotai.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wej.ctjpmb.com

[S48] C++：逐行读文件
来源：http://ljz.jianghu66.top

std::ifstream in("a.txt");  std::string line;
来源：http://zwk.zycfv.cn

while (std::getline(in, line)) { }
来源：http://hpu.fktsv.cn

[S49] C++：写文件
来源：http://xca.mhx1999.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lnk.daxiang520.top

[S50] C++：格式化数字
来源：http://owi.wangdashe.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dfe.tian-w.cn

[S51] C++：显式类型转换
来源：http://kcb.hongshengwenyu.top

static_cast<double>(a) / b
来源：http://osm.yj20258888.top

[S52] C++：const 与 noexcept
来源：http://wwk.zdqjudy.top

int size() const noexcept { return n_; }
来源：http://oms.daxiang520.top

[S53] C++：移动语义
来源：http://mku.pycfn.com

std::vector<int> w = std::move(v);
来源：http://kmg.ywan-chungtsiang.top

[S54] C++：异常处理
来源：http://ksv.chenlongwang.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gtv.zdbjq.cn

[S55] C++：结构化绑定
来源：http://tpq.havefunace.top

auto [a, b] = std::make_pair(1, 2);
来源：http://drf.cqqwz.cn

[S56] C++：optional
来源：http://vmq.gaohongyu789.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hvu.cdnleiting.top

[S57] C++：编译期常量
来源：http://idv.hcnkem.com

constexpr int N = 10;
来源：http://iov.tarul.cn

[S58] C++：命名空间
来源：http://yhf.ctjpmb.com

namespace ns { int f() { return 1; } }
来源：http://upu.zhijiandao.cn

[S59] C++：静态断言
来源：http://wbk.uphjek.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bap.guannengcc.top

[S60] C++：遍历并删除元素
来源：http://cht.feifeiyinyue.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dmo.sysykeji.top

================================================================================
来源：http://ahs.ybcxt.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ruj.jinyuanbaomall.cn

================================================================================
来源：http://byv.daria6918.cn

[T01] Kotlin：Hello World
来源：http://nte.guowangkeji.top

println("Hello")
来源：http://ebg.316326.xyz

[T02] Kotlin：变量
来源：http://chs.jiagoushi.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sqv.316326.xyz

[T03] Kotlin：字符串模板
来源：http://oui.316326.xyz

"值: $b"
来源：http://rdv.hnqzz.top

[T04] Kotlin：空安全
来源：http://tbw.shzxlz.cn

val n: String? = null;  n?.length
来源：http://owy.pengpengdd.cyou

[T05] Kotlin：when 表达式
来源：http://yxx.zhongyouzk.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lvq.kuanghao11.cn

[T06] Kotlin：集合映射
来源：http://bze.jinqigfzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://njc.jinyuanbaomall.cn

[T07] Kotlin：集合过滤
来源：http://xaj.zhixingplan.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://xbh.sxryk.cn

[T08] Kotlin：数据类
来源：http://ion.jiagoushi.top

data class User(val name: String, val age: Int)
来源：http://bsb.daxiang520.top

[T09] Kotlin：扩展函数
来源：http://gzi.yj20258888.top

fun String.exclaim() = this + "!"
来源：http://fak.haohaochexian.top

[T10] Kotlin：默认参数
来源：http://xjm.wangdashe.top

fun greet(name: String = "World") = "Hi $name"
来源：http://mwi.ivvv.top

[T11] Kotlin：协程
来源：http://lvv.chenlongwang.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://cdd.haohaochexian.top

[T12] Kotlin：解构声明
来源：http://noc.jiagoushi.top

val (a, b) = Pair(1, 2)
来源：http://kib.hesvh.cn

[T13] Kotlin：只读 Map
来源：http://ysq.havefunace.top

val m = mapOf("a" to 1)
来源：http://mho.hysaishi.cn

[T14] Kotlin：循环
来源：http://cqz.ehwqpu.com

for (i in 1..10) println(i)
来源：http://ijq.316326.xyz

[T15] Kotlin：接口
来源：http://teg.dashuyun.cn

interface Shape { fun area(): Double }
来源：http://mic.kuanghao11.cn

[T16] Swift：Hello World
来源：http://fkb.ybcxt.top

print("Hello")
来源：http://lqo.yj20258.top

[T17] Swift：变量与常量
来源：http://pnz.fengsongda.top

var a = 1;  let b = 2
来源：http://ymt.xuetiantiany.cn

[T18] Swift：字符串插值
来源：http://pah.316326.xyz

"值: \(b)"
来源：http://vmg.cheryme.top

[T19] Swift：可选绑定
来源：http://mgy.dianchejie.cn

if let n = opt { print(n) }
来源：http://sal.chenlongwang.top

[T20] Swift：数组操作
来源：http://bhj.yongpay.top

var a = [1, 2, 3];  a.append(4)
来源：http://fea.ydzc1.top

[T21] Swift：遍历
来源：http://zow.gaohongyu789.top

for x in a { print(x) }
来源：http://gwf.kuanghao11.cn

[T22] Swift：字典
来源：http://jup.hcnkem.com

var d = ["a": 1];  d["b"] = 2
来源：http://lru.sysykeji.top

[T23] Swift：函数
来源：http://qzo.daxiang520.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sfd.xylfe.cn

[T24] Swift：闭包
来源：http://cil.cashguo.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ddt.yangfankeji.com

[T25] Swift：结构体
来源：http://ywq.shanyushiyangtech.top

struct P { var x: Int }
来源：http://byo.aizwys.cn

[T26] Swift：类与重写
来源：http://tmx.gotoacloud.top

class A: Base { override func f() {} }
来源：http://qfe.daxiang520.top

[T27] Swift：错误处理
来源：http://rnx.birdmap.top

do { try f() } catch { print(error) }
来源：http://ltu.jinqigfzy.top

[T28] Swift：枚举
来源：http://ykn.hongshengwenyu.top

enum Color { case red, green }
来源：http://gsm.tanke756.top

[T29] Swift：guard 提前返回
来源：http://tgn.yj202588.top

guard let x = opt else { return }
来源：http://lut.xinyue.icu

[T30] Swift：协议
来源：http://xzr.xinyue.icu

protocol Shape { func area() -> Double }
来源：http://ohk.shuidangran.top

[T31] Lua：Hello World
来源：http://zja.hammf.cn

print("Hello")
来源：http://ltq.gzhubu.top

[T32] Lua：局部变量
来源：http://voi.jinqigfzy.top

local a = 1
来源：http://soe.hnqzz.top

[T33] Lua：表（数组）
来源：http://bvi.0kj1m.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://qvp.pycfn.com

[T34] Lua：遍历表
来源：http://pbg.zhijiandao.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://agc.zhiwuduotai.top

[T35] Lua：字典表
来源：http://osp.epnwcf.com

local d = { a = 1 };  d.b = 2
来源：http://nul.sweek.top

[T36] Lua：函数
来源：http://ezu.zhongyouzk.top

function add(a, b) return a + b end
来源：http://ujk.pycfn.com

[T37] Lua：字符串拼接
来源：http://rbh.cdnleiting.top

"a" .. "b"
来源：http://bce.yuanzhike.top

[T38] Lua：条件
来源：http://ooj.gaohongyu789.top

if x > 0 then print("正") end
来源：http://tgg.c1oappe.top

[T39] Lua：模式匹配
来源：http://tnk.yj20258888.top

string.find(s, "%d+")
来源：http://eup.daxiang520.top

[T40] Lua：元表
来源：http://rje.52xcode.cn

setmetatable({}, { __index = base })
来源：http://huz.shangyingyoupin.top

[T41] Perl：Hello World
来源：http://aqn.zhaomingkeji.xyz

print "Hello\n";
来源：http://biy.zhongyouzk.top

[T42] Perl：变量类型
来源：http://wke.hammf.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://uxo.hnxiangtu.top

[T43] Perl：字符串插值
来源：http://low.xingfuxueyuan.xyz

"值: $a"
来源：http://qrl.zhixingplan.top

[T44] Perl：条件
来源：http://aev.gotoacloud.top

if ($a > 0) { print "正"; }
来源：http://azw.ehwqpu.com

[T45] Perl：数组遍历
来源：http://rno.zhoulong.xyz

for my $x (@arr) { print $x; }
来源：http://tib.xuetiantiany.cn

[T46] Perl：哈希操作
来源：http://oxn.ehwqpu.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cgy.yonumen.top

[T47] Perl：正则捕获
来源：http://nym.jlsjyb.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://vox.fanxiaobao.xyz

[T48] Perl：正则替换
来源：http://vca.shzxlz.cn

$s =~ s/old/new/g;
来源：http://ddy.yvedp.cn

[T49] Perl：函数
来源：http://pny.sufxvd.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://iny.zhijiandao.cn

[T50] Perl：逐行读文件
来源：http://hws.sufxvd.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xbw.tarul.cn

while (my $line = <$fh>) { print $line; }
来源：http://myv.uphjek.com

[T51] Scala：Hello World
来源：http://mtc.ctjpmb.com

println("Hello")
来源：http://aeo.cucudq.cn

[T52] Scala：变量
来源：http://kos.chenzaomai.com

val a = 1;  var b = 2
来源：http://qnh.cucudq.cn

[T53] Scala：字符串插值
来源：http://rip.mhx1999.top

s"值: $b"
来源：http://alh.fanxiaobao.xyz

[T54] Scala：集合映射
来源：http://wrn.haohaochexian.top

List(1, 2, 3).map(_ * 2)
来源：http://lcy.birdmap.top

[T55] Scala：集合过滤
来源：http://nls.xuanzx.com

List(1, 2, 3).filter(_ > 1)
来源：http://fkv.sjlbkw.cn

[T56] Scala：样例类
来源：http://sle.tianlin.xyz

case class User(name: String, age: Int)
来源：http://eyu.hnqzz.top

[T57] Scala：模式匹配
来源：http://lbs.jinyuanbaomall.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://lrm.gogol.net.cn

[T58] Scala：函数定义
来源：http://prc.zdqjudy.top

def add(a: Int, b: Int): Int = a + b
来源：http://lxf.fehbvm.com

[T59] Scala：循环
来源：http://ltx.vehdjk.com

for (i <- 1 to 10) println(i)
来源：http://yly.9152youxi.cn

[T60] Scala：折叠
来源：http://vgr.sjlbkw.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hxv.hywenlv.cn

================================================================================
来源：http://kwx.ybcxt.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zgf.gzhubu.top

================================================================================
来源：http://vda.ctjpmb.com

[U01] Py：创建虚拟环境
来源：http://bmt.zhixingplan.top

python -m venv .venv && source .venv/bin/activate
来源：http://tue.hnqzz.top

[U02] Py：导出 / 安装依赖
来源：http://gjl.zhixingplan.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rtj.ywan-chungtsiang.top

[U03] Py：加载 .env 配置
来源：http://xka.xinyue.icu

from dotenv import load_dotenv; load_dotenv()
来源：http://oam.wangshuangyany.cn

[U04] Py：变量调试打印
来源：http://rkm.aizwys.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qur.shuidangran.top

[U05] Py：列表去重且保序
来源：http://jbb.yj20258888.top

list(dict.fromkeys(arr))
来源：http://fjq.ywan-chungtsiang.top

[U06] Py：合并两个字典
来源：http://ruw.aibaodan.cn

{**a, **b}
来源：http://ffx.xziqi.cn

[U07] Py：反转字典键值
来源：http://yph.sweek.top

{v: k for k, v in d.items()}
来源：http://agd.tian-w.cn

[U08] Py：展平二维列表
来源：http://rbs.tianlin.xyz

[y for x in nested for y in x]
来源：http://iie.shanyushiyangtech.top

[U09] Py：字典取最大值的键
来源：http://axw.birdmap.top

max(d, key=d.get)
来源：http://bof.ehwqpu.com

[U10] Py：按值排序字典
来源：http://fhm.ehwqpu.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://xrh.ydzc1.top

[U11] Py：生成器表达式
来源：http://quq.cqqwz.cn

(x * 2 for x in arr)
来源：http://rsz.hnqzz.top

[U12] Py：取出现最多的 3 个元素
来源：http://iny.zycfv.cn

Counter(arr).most_common(3)
来源：http://vxf.tanke756.top

[U13] Py：固定长度队列
来源：http://cqq.redwolf501.top

deque(maxlen=10)
来源：http://kcq.shanyushiyangkeji.top

[U14] Py：分组收集到列表
来源：http://zfw.meibo888.top

defaultdict(list)
来源：http://zbi.xinyue.icu

[U15] Py：高精度计时
来源：http://pcu.iojbl.cn

t = time.perf_counter()
来源：http://xuk.chenzaomai.com

[U16] Py：命令行参数解析
来源：http://omt.gogol.net.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wdf.tarul.cn

[U17] Py：初始化日志
来源：http://fuy.birdmap.top

logging.basicConfig(level=logging.INFO)
来源：http://fep.tanke756.top

[U18] Py：预编译正则
来源：http://ktl.jianghu66.top

pat = re.compile(r"\d+")
来源：http://guz.daria6918.cn

[U19] Py：正则替换带回调
来源：http://opc.jyoumei.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rlz.epnwcf.com

[U20] Py：缓存函数结果
来源：http://fqh.wangshuangyany.cn

@functools.lru_cache(maxsize=None)
来源：http://zgq.gaohongyu789.top

[U21] Py：自定义上下文管理器
来源：http://pqb.ehwqpu.com

@contextlib.contextmanager
来源：http://jur.haohaochexian.top

[U22] Py：矩阵转置
来源：http://pjo.hnxiangtu.top

list(zip(*m))
来源：http://vuu.snrcjt.cn

[U23] Py：分块读取大文件
来源：http://hub.bjfxy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://pgj.yuanzhike.top

[U24] Py：路径操作
来源：http://sxe.zhaomingkeji.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://oks.zycfv.cn

[U25] Py：CSV 按字典读
来源：http://qet.zhijiandao.cn

csv.DictReader(f)
来源：http://tki.gaohongyu789.top

[U26] Py：并发下载
来源：http://vkm.bbcook.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://hfn.fktsv.cn

[U27] Py：异步 HTTP
来源：http://cjk.dashuyun.cn

aiohttp.ClientSession() 配合 async with
来源：http://mnj.mhx1999.top

[U28] Py：类型别名
来源：http://xkp.bjfxy.top

UserId = int
来源：http://abn.hysaishi.cn

[U29] Py：属性校验
来源：http://eal.cdnleiting.top

@property 与 @x.setter 配合
来源：http://lzc.yangfankeji.com

[U30] Py：数据类
来源：http://asu.vqdsnc.cn

@dataclass(slots=True)
来源：http://evf.zhijiandao.cn

[U31] Py：单测
来源：http://owr.fehbvm.com

python -m pytest -q
来源：http://zte.shanyushiyangtech.top

[U32] Py：代码格式化
来源：http://smm.aizwys.cn

ruff format . && ruff check --fix .
来源：http://usl.chenzaomai.com

[U33] Py：打包发布
来源：http://szb.tanke756.top

python -m build  （依赖 pyproject.toml）
来源：http://ixq.zycfv.cn

[U34] Py：判断编码
来源：http://yer.gogol.net.cn

chardet.detect(raw)
来源：http://lxb.redwolf501.top


<!-- 参考信息 -->