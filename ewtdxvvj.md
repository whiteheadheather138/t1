代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jpo.tanke756.top

[S13] C：宏定义
来源：http://rcj.jiagoushi.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yxm.jqgufenzy.top

[S14] C：枚举
来源：http://mry.zhijiandao.cn

enum Color { RED, GREEN, BLUE };
来源：http://zie.pycfn.com

[S15] C：类型转换
来源：http://efd.yanxiufei.cn

(double) a / b
来源：http://gbf.jinyuanbaomall.cn

[S16] C：位操作置位
来源：http://nwk.sysykeji.top

x |= (1 << 3);
来源：http://tot.svipenyu.cn

[S17] C：安全拼接字符串
来源：http://tah.sxryk.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jiv.ybcxt.top

[S18] C：命令行参数
来源：http://okd.shuidangran.top

int main(int argc, char **argv)
来源：http://lcl.dianchejie.cn

[S19] C：快速排序
来源：http://hbw.yvedp.cn

qsort(a, n, sizeof(int), cmp);
来源：http://lnx.yj202588.top

[S20] C：二分查找
来源：http://rpw.fzhhl.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ahm.sjlbkw.cn

[S21] C：字符类别判断
来源：http://pum.feifeiyinyue.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ekc.jiagoushi.top

[S22] C：字符串转数字
来源：http://pgd.vehdjk.com

atoi("42");  strtod("3.14", NULL);
来源：http://jyt.zdbjq.cn

[S23] C：随机数
来源：http://fah.hnxiangtu.top

srand(time(NULL));  int r = rand() % 100;
来源：http://czu.sweek.top

[S24] C：获取本地时间
来源：http://syf.yuxming.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jtz.shzxlz.cn

[S25] C：内存拷贝
来源：http://xwz.0kj1m.cn

memcpy(dst, src, n);
来源：http://zih.fzhhl.top

[S26] C：内存清零
来源：http://tat.zycfv.cn

memset(a, 0, sizeof a);
来源：http://qkj.jqgfzy.top

[S27] C：定义常量
来源：http://qqr.c1oappe.top

const double PI = 3.14159;
来源：http://hlt.xziqi.cn

[S28] C：静态变量
来源：http://fzo.wangdashe.top

static int counter = 0;
来源：http://tdw.gotoacloud.top

[S29] C：变参函数
来源：http://sie.jianghu66.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pzd.smart0.xyz

[S30] C：头文件保护
来源：http://uwb.yueranfly.top

#ifndef X_H
来源：http://jiq.hongshengwenyu.top

#define X_H
来源：http://cxe.yvedp.cn

#endif
来源：http://mzy.xziqi.cn

[S31] C++：Hello World
来源：http://cst.wangdashe.top

#include <iostream>
来源：http://bbz.shzxlz.cn

int main() { std::cout << "Hello\n"; }
来源：http://qno.ydzc1.top

[S32] C++：字符串
来源：http://clb.sysykeji.top

std::string s = "hi";  s += "!";
来源：http://bla.ywan-chungtsiang.top

[S33] C++：vector 增删
来源：http://tjv.tarul.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qoz.yj202588.top

[S34] C++：遍历 vector
来源：http://yxo.xingfuxueyuan.xyz

for (auto &x : v) { std::cout << x; }
来源：http://jyr.tian-w.cn

[S35] C++：map
来源：http://zck.chenzaomai.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zdg.nwbrower.top

[S36] C++：unordered_map
来源：http://idj.dianchejie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bvm.dianchejie.cn

[S37] C++：set
来源：http://tqo.iojbl.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zbv.kuanghao11.cn

[S38] C++：排序
来源：http://hww.xuetiantiany.cn

std::sort(v.begin(), v.end());
来源：http://qau.redwolf501.top

[S39] C++：自定义比较器排序
来源：http://tnc.svipenyu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://iay.nanxinkj.top

[S40] C++：查找元素
来源：http://abx.ywan-chungtsiang.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qxz.zycfv.cn

[S41] C++：类与构造函数
来源：http://iqu.uphjek.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sdn.xylfe.cn

[S42] C++：继承与虚函数
来源：http://rzz.jiagoushi.top

class B : public Base { public: void f() override {} };
来源：http://arr.hnqzz.top

[S43] C++：智能指针
来源：http://ugj.fanxiaobao.xyz

auto p = std::make_unique<int>(5);
来源：http://ebo.hammf.cn

[S44] C++：引用传参
来源：http://euf.52xcode.cn

void inc(int &x) { ++x; }
来源：http://tra.hesvh.cn

[S45] C++：lambda
来源：http://dbz.bjfxy.top

auto add = [](int a, int b) { return a + b; };
来源：http://zqf.hysaishi.cn

[S46] C++：函数模板
来源：http://iea.hongshengwenyu.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gno.birdmap.top

[S47] C++：结构化绑定遍历
来源：http://btm.52xcode.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tpp.hysaishi.cn

[S48] C++：逐行读文件
来源：http://bjo.ivvv.top

std::ifstream in("a.txt");  std::string line;
来源：http://alg.yuxming.cn

while (std::getline(in, line)) { }
来源：http://msj.zhaomingkeji.xyz

[S49] C++：写文件
来源：http://rrt.nwbrower.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://twq.ppjwa.cn

[S50] C++：格式化数字
来源：http://ytd.nanxinkj.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rhw.zhiwuduotai.top

[S51] C++：显式类型转换
来源：http://pfz.pengpengdd.cyou

static_cast<double>(a) / b
来源：http://bni.vqdsnc.cn

[S52] C++：const 与 noexcept
来源：http://vxs.gotoacloud.top

int size() const noexcept { return n_; }
来源：http://rcj.fktsv.cn

[S53] C++：移动语义
来源：http://tnx.shzxlz.cn

std::vector<int> w = std::move(v);
来源：http://qlw.xuanzx.com

[S54] C++：异常处理
来源：http://tuz.iojbl.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://geq.zycfv.cn

[S55] C++：结构化绑定
来源：http://bim.0kj1m.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://buj.jinqigfzy.top

[S56] C++：optional
来源：http://jxc.cashguo.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ise.kuanghao11.cn

[S57] C++：编译期常量
来源：http://adm.xingfuxueyuan.xyz

constexpr int N = 10;
来源：http://vil.jiagoushi.top

[S58] C++：命名空间
来源：http://hfv.ydjk.org.cn

namespace ns { int f() { return 1; } }
来源：http://jro.fanxiaobao.xyz

[S59] C++：静态断言
来源：http://ayh.cashguo.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ljy.epnwcf.com

[S60] C++：遍历并删除元素
来源：http://sdh.quarkkingdee.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bco.gotoacloud.top

================================================================================
来源：http://mvn.vehdjk.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gfg.fengsongda.top

================================================================================
来源：http://bkt.dashuyun.cn

[T01] Kotlin：Hello World
来源：http://qhe.zhaomingkeji.xyz

println("Hello")
来源：http://aol.xuetiantiany.cn

[T02] Kotlin：变量
来源：http://tvt.kuanghao11.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mno.dashuyun.cn

[T03] Kotlin：字符串模板
来源：http://yca.c1oappe.top

"值: $b"
来源：http://zna.havefunace.top

[T04] Kotlin：空安全
来源：http://gcd.bbcook.cn

val n: String? = null;  n?.length
来源：http://msz.gotoacloud.top

[T05] Kotlin：when 表达式
来源：http://tzm.hnqzz.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://doc.316326.xyz

[T06] Kotlin：集合映射
来源：http://ujr.sjlbkw.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ttf.fzhhl.top

[T07] Kotlin：集合过滤
来源：http://hjw.chenlongwang.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ays.fzhhl.top

[T08] Kotlin：数据类
来源：http://dee.xylfe.cn

data class User(val name: String, val age: Int)
来源：http://iou.zhaomingkeji.xyz

[T09] Kotlin：扩展函数
来源：http://eaf.xingfuxueyuan.xyz

fun String.exclaim() = this + "!"
来源：http://pjg.gotoacloud.top

[T10] Kotlin：默认参数
来源：http://eph.xuetiantiany.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://koo.svipenyu.cn

[T11] Kotlin：协程
来源：http://loj.aizwys.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hjj.pengpengdd.cyou

[T12] Kotlin：解构声明
来源：http://nmc.ywan-chungtsiang.top

val (a, b) = Pair(1, 2)
来源：http://gwg.smart0.xyz

[T13] Kotlin：只读 Map
来源：http://wca.ywan-chungtsiang.top

val m = mapOf("a" to 1)
来源：http://czr.birdmap.top

[T14] Kotlin：循环
来源：http://sqj.jiagoushi.top

for (i in 1..10) println(i)
来源：http://biv.nanxuanxn.top

[T15] Kotlin：接口
来源：http://itr.guannengcc.top

interface Shape { fun area(): Double }
来源：http://ktq.yuxming.cn

[T16] Swift：Hello World
来源：http://rwi.meibo888.top

print("Hello")
来源：http://rna.bbcook.cn

[T17] Swift：变量与常量
来源：http://zrd.gotoacloud.top

var a = 1;  let b = 2
来源：http://kkv.yj20258.top

[T18] Swift：字符串插值
来源：http://rws.yangfankeji.com

"值: \(b)"
来源：http://jzf.gzhubu.top

[T19] Swift：可选绑定
来源：http://ztl.xuanzx.com

if let n = opt { print(n) }
来源：http://ssm.yj20258888.top

[T20] Swift：数组操作
来源：http://tle.sxryk.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fml.haohaochexian.top

[T21] Swift：遍历
来源：http://sem.vqdsnc.cn

for x in a { print(x) }
来源：http://pcb.shzxlz.cn

[T22] Swift：字典
来源：http://tzf.zdqjudy.top

var d = ["a": 1];  d["b"] = 2
来源：http://ada.zhijiandao.cn

[T23] Swift：函数
来源：http://vid.hcnkem.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://khe.vehdjk.com

[T24] Swift：闭包
来源：http://cxe.hnqzz.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://utz.shzxlz.cn

[T25] Swift：结构体
来源：http://thk.jinqigufen.top

struct P { var x: Int }
来源：http://nbn.zhaomingkeji.xyz

[T26] Swift：类与重写
来源：http://eot.kuanghao11.cn

class A: Base { override func f() {} }
来源：http://ijc.yuxming.cn

[T27] Swift：错误处理
来源：http://zlq.shanyushiyangkeji.top

do { try f() } catch { print(error) }
来源：http://vya.haohaochexian.top

[T28] Swift：枚举
来源：http://dqk.shzxlz.cn

enum Color { case red, green }
来源：http://mkt.vehdjk.com

[T29] Swift：guard 提前返回
来源：http://yue.pycfn.com

guard let x = opt else { return }
来源：http://bhi.gogol.net.cn

[T30] Swift：协议
来源：http://hsu.shanyushiyangtech.top

protocol Shape { func area() -> Double }
来源：http://xoa.yonumen.top

[T31] Lua：Hello World
来源：http://rjp.yvedp.cn

print("Hello")
来源：http://zli.hnxiangtu.top

[T32] Lua：局部变量
来源：http://num.hywenlv.cn

local a = 1
来源：http://ghp.yj20258.top

[T33] Lua：表（数组）
来源：http://ghh.haohaochexian.top

local t = {1, 2, 3};  t[4] = 4
来源：http://nhu.nanxinkj.top

[T34] Lua：遍历表
来源：http://ndy.ydjk.org.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://laj.hongshengwenyu.top

[T35] Lua：字典表
来源：http://rcb.zhaomingkeji.xyz

local d = { a = 1 };  d.b = 2
来源：http://dsd.pycfn.com

[T36] Lua：函数
来源：http://apu.feifeiyinyue.top

function add(a, b) return a + b end
来源：http://zmp.meibo888.top

[T37] Lua：字符串拼接
来源：http://dnl.hnqzz.top

"a" .. "b"
来源：http://khh.fanxiaobao.xyz

[T38] Lua：条件
来源：http://wsi.aibaodan.cn

if x > 0 then print("正") end
来源：http://ogi.shuidangran.top

[T39] Lua：模式匹配
来源：http://eon.ivvv.top

string.find(s, "%d+")
来源：http://igm.gogol.net.cn

[T40] Lua：元表
来源：http://zao.jinqigufen.top

setmetatable({}, { __index = base })
来源：http://mcg.chenjidiqi.icu

[T41] Perl：Hello World
来源：http://nna.fzhhl.top

print "Hello\n";
来源：http://klo.kuanghao11.cn

[T42] Perl：变量类型
来源：http://qys.dashuyun.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kbp.cucudq.cn

[T43] Perl：字符串插值
来源：http://ycr.sxryk.cn

"值: $a"
来源：http://lnl.fktsv.cn

[T44] Perl：条件
来源：http://pdj.ivvv.top

if ($a > 0) { print "正"; }
来源：http://maz.jianghu66.top

[T45] Perl：数组遍历
来源：http://hnx.feifeiyinyue.top

for my $x (@arr) { print $x; }
来源：http://aos.xuetiantiany.cn

[T46] Perl：哈希操作
来源：http://gub.chenjidiqi.icu

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jvx.hongshengwenyu.top

[T47] Perl：正则捕获
来源：http://zig.shzxlz.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://dru.gaohongyu789.top

[T48] Perl：正则替换
来源：http://pnq.jinqigufen.top

$s =~ s/old/new/g;
来源：http://blz.shanyushiyangkeji.top

[T49] Perl：函数
来源：http://zyx.ydzc1.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kxm.pycfn.com

[T50] Perl：逐行读文件
来源：http://ffa.yuanzhike.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ojo.ivvv.top

while (my $line = <$fh>) { print $line; }
来源：http://ghs.jianghu66.top

[T51] Scala：Hello World
来源：http://znh.snrcjt.cn

println("Hello")
来源：http://uwd.ydjk.org.cn

[T52] Scala：变量
来源：http://xfp.cqqwz.cn

val a = 1;  var b = 2
来源：http://lia.quarkkingdee.top

[T53] Scala：字符串插值
来源：http://dbo.svipenyu.cn

s"值: $b"
来源：http://acc.ydzc1.top

[T54] Scala：集合映射
来源：http://sgy.jqgfzy.top

List(1, 2, 3).map(_ * 2)
来源：http://jmu.dashuyun.cn

[T55] Scala：集合过滤
来源：http://rdk.hfpthk.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gms.ydzc1.top

[T56] Scala：样例类
来源：http://ufw.yj20258.top

case class User(name: String, age: Int)
来源：http://bdf.sxryk.cn

[T57] Scala：模式匹配
来源：http://mij.cdnleiting.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://zpe.jinghuilouyu.cn

[T58] Scala：函数定义
来源：http://hnf.zhixingplan.top

def add(a: Int, b: Int): Int = a + b
来源：http://jgs.nanxinkj.top

[T59] Scala：循环
来源：http://blb.sxryk.cn

for (i <- 1 to 10) println(i)
来源：http://ibe.xuanzx.com

[T60] Scala：折叠
来源：http://djz.aibaodan.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hdx.sjlbkw.cn

================================================================================
来源：http://rek.yvedp.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://jvv.fzhhl.top

================================================================================
来源：http://nbc.fengsongda.top

[U01] Py：创建虚拟环境
来源：http://vah.xziqi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://xuz.yj20258.top

[U02] Py：导出 / 安装依赖
来源：http://osx.bbcook.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vky.gaohongyu789.top

[U03] Py：加载 .env 配置
来源：http://hzy.zhengqikj.top

from dotenv import load_dotenv; load_dotenv()
来源：http://utu.haohaochexian.top

[U04] Py：变量调试打印
来源：http://yor.shanyushiyangtech.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mll.nwbrower.top

[U05] Py：列表去重且保序
来源：http://rvi.zhaomingkeji.xyz

list(dict.fromkeys(arr))
来源：http://dgz.hesvh.cn

[U06] Py：合并两个字典
来源：http://mve.zhongyouzk.top

{**a, **b}
来源：http://xtd.sjlbkw.cn

[U07] Py：反转字典键值
来源：http://otr.wangdashe.top

{v: k for k, v in d.items()}
来源：http://uqu.yuanzhike.top

[U08] Py：展平二维列表
来源：http://ims.yuanzhike.top

[y for x in nested for y in x]
来源：http://ikt.meibo888.top

[U09] Py：字典取最大值的键
来源：http://xgg.tian-w.cn

max(d, key=d.get)
来源：http://ulp.shuidangran.top

[U10] Py：按值排序字典
来源：http://lgj.yj20258.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nwj.smart0.xyz

[U11] Py：生成器表达式
来源：http://lpx.ydjk.org.cn

(x * 2 for x in arr)
来源：http://cdn.shuidangran.top

[U12] Py：取出现最多的 3 个元素
来源：http://xvh.xziqi.cn

Counter(arr).most_common(3)
来源：http://nwo.vehdjk.com

[U13] Py：固定长度队列
来源：http://yuc.zdqjudy.top

deque(maxlen=10)
来源：http://vux.quarkkingdee.top

[U14] Py：分组收集到列表
来源：http://gda.ydzc1.top

defaultdict(list)
来源：http://jox.gogol.net.cn

[U15] Py：高精度计时
来源：http://cbg.fktsv.cn

t = time.perf_counter()
来源：http://bah.hnxiangtu.top

[U16] Py：命令行参数解析
来源：http://sri.zdqjudy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://irx.shanyushiyangkeji.top

[U17] Py：初始化日志
来源：http://tzm.hywenlv.cn

logging.basicConfig(level=logging.INFO)
来源：http://kwo.snrcjt.cn

[U18] Py：预编译正则
来源：http://sag.ehwqpu.com

pat = re.compile(r"\d+")
来源：http://xrp.xylfe.cn

[U19] Py：正则替换带回调
来源：http://ldj.hfpthk.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://mjy.epnwcf.com

[U20] Py：缓存函数结果
来源：http://mba.tian-w.cn

@functools.lru_cache(maxsize=None)
来源：http://jku.zdqjudy.top

[U21] Py：自定义上下文管理器
来源：http://hzr.zhijiandao.cn

@contextlib.contextmanager
来源：http://xtm.mhx1999.top

[U22] Py：矩阵转置
来源：http://cnf.jinghuilouyu.cn

list(zip(*m))
来源：http://qzl.ydzc1.top

[U23] Py：分块读取大文件
来源：http://pdb.jqgufenzy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ryu.quarkkingdee.top

[U24] Py：路径操作
来源：http://hyb.hfpthk.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bqb.jinqigfzy.top

[U25] Py：CSV 按字典读
来源：http://ftr.birdmap.top

csv.DictReader(f)
来源：http://szf.gotoacloud.top

[U26] Py：并发下载
来源：http://vjm.fktsv.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://zym.yonumen.top

[U27] Py：异步 HTTP
来源：http://gyf.zhengqikj.top

aiohttp.ClientSession() 配合 async with
来源：http://xci.haohaochexian.top

[U28] Py：类型别名
来源：http://zzt.gotoacloud.top

UserId = int
来源：http://qyq.smart0.xyz

[U29] Py：属性校验
来源：http://cpe.gzhubu.top

@property 与 @x.setter 配合
来源：http://veh.vqdsnc.cn

[U30] Py：数据类
来源：http://vrl.xziqi.cn

@dataclass(slots=True)
来源：http://old.shangyingyoupin.top

[U31] Py：单测
来源：http://heq.dianchejie.cn

python -m pytest -q
来源：http://shj.wangdashe.top

[U32] Py：代码格式化
来源：http://wcl.quarkkingdee.top

ruff format . && ruff check --fix .
来源：http://iqi.zdbjq.cn

[U33] Py：打包发布
来源：http://frq.shanyushiyangkeji.top

python -m build  （依赖 pyproject.toml）
来源：http://lwi.svipenyu.cn

[U34] Py：判断编码
来源：http://gaq.c1oappe.top

chardet.detect(raw)
来源：http://his.yangfankeji.com

[U35] Py：发送邮件
来源：http://jzn.sysykeji.top

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://phv.fanxiaobao.xyz

[U36] Py：定时任务
来源：http://vnu.guowangkeji.top

schedule.every(10).minutes.do(job)
来源：http://nmg.ywan-chungtsiang.top


<!-- 参考信息 -->