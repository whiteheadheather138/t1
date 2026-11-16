代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://vbj.daxiang520.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://lna.zhiwuduotai.top

fclose(f);
来源：http://aef.hfpthk.cn

[S12] C：写文件
来源：http://owl.zhoulong.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bqt.yueranfly.top

[S13] C：宏定义
来源：http://dwy.hywenlv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://udr.cucudq.cn

[S14] C：枚举
来源：http://umj.sysykeji.top

enum Color { RED, GREEN, BLUE };
来源：http://jzn.havefunace.top

[S15] C：类型转换
来源：http://jwp.sjlbkw.cn

(double) a / b
来源：http://xyd.hnqzz.top

[S16] C：位操作置位
来源：http://via.snrcjt.cn

x |= (1 << 3);
来源：http://pcg.nanxinkj.top

[S17] C：安全拼接字符串
来源：http://akj.zdqjudy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zbx.epnwcf.com

[S18] C：命令行参数
来源：http://cfv.xinyue.icu

int main(int argc, char **argv)
来源：http://ofz.jinghuilouyu.cn

[S19] C：快速排序
来源：http://lmg.ctjpmb.com

qsort(a, n, sizeof(int), cmp);
来源：http://ocs.jinqigufen.top

[S20] C：二分查找
来源：http://rlr.guannengcc.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fus.0kj1m.cn

[S21] C：字符类别判断
来源：http://moh.yj202588.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qqh.nanxinkj.top

[S22] C：字符串转数字
来源：http://nlq.hcnkem.com

atoi("42");  strtod("3.14", NULL);
来源：http://ziq.fzhhl.top

[S23] C：随机数
来源：http://iuk.jlsjyb.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://act.xinyue.icu

[S24] C：获取本地时间
来源：http://ilv.dianchejie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ted.fktsv.cn

[S25] C：内存拷贝
来源：http://wrp.shanyushiyangkeji.top

memcpy(dst, src, n);
来源：http://mta.gaohongyu789.top

[S26] C：内存清零
来源：http://auz.zhaomingkeji.xyz

memset(a, 0, sizeof a);
来源：http://phs.jinghuilouyu.cn

[S27] C：定义常量
来源：http://imv.cqqwz.cn

const double PI = 3.14159;
来源：http://xcs.yj20258888.top

[S28] C：静态变量
来源：http://bgg.hysaishi.cn

static int counter = 0;
来源：http://jdx.dashuyun.cn

[S29] C：变参函数
来源：http://sfd.9152youxi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hbw.fzhhl.top

[S30] C：头文件保护
来源：http://udf.shangyingyoupin.top

#ifndef X_H
来源：http://akd.pengpengdd.cyou

#define X_H
来源：http://ikm.nanxinkj.top

#endif
来源：http://hch.gotoacloud.top

[S31] C++：Hello World
来源：http://epu.jianghu66.top

#include <iostream>
来源：http://mda.sysykeji.top

int main() { std::cout << "Hello\n"; }
来源：http://fom.aizwys.cn

[S32] C++：字符串
来源：http://yzo.zhoulong.xyz

std::string s = "hi";  s += "!";
来源：http://haf.havefunace.top

[S33] C++：vector 增删
来源：http://jmx.hnqzz.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://stw.feifeiyinyue.top

[S34] C++：遍历 vector
来源：http://dtw.shangyingyoupin.top

for (auto &x : v) { std::cout << x; }
来源：http://knj.hcnkem.com

[S35] C++：map
来源：http://vbz.shanyushiyangkeji.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://thn.yfazqb.com

[S36] C++：unordered_map
来源：http://bxa.ydzc1.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://iuj.yueranfly.top

[S37] C++：set
来源：http://ldk.yj20258.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wge.daria6918.cn

[S38] C++：排序
来源：http://ndz.xuanzx.com

std::sort(v.begin(), v.end());
来源：http://yjy.havefunace.top

[S39] C++：自定义比较器排序
来源：http://uqe.hywenlv.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://txm.zhaomingkeji.xyz

[S40] C++：查找元素
来源：http://quf.zhengqikj.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gtx.jiagoushi.top

[S41] C++：类与构造函数
来源：http://miz.tarul.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rqp.316326.xyz

[S42] C++：继承与虚函数
来源：http://azq.zhiwuduotai.top

class B : public Base { public: void f() override {} };
来源：http://mvp.hnqzz.top

[S43] C++：智能指针
来源：http://bnc.yangfankeji.com

auto p = std::make_unique<int>(5);
来源：http://vch.jyoumei.cn

[S44] C++：引用传参
来源：http://ofa.cheryme.top

void inc(int &x) { ++x; }
来源：http://cye.hnqzz.top

[S45] C++：lambda
来源：http://pvv.fehbvm.com

auto add = [](int a, int b) { return a + b; };
来源：http://ldw.nanxinkj.top

[S46] C++：函数模板
来源：http://hrk.9152youxi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kpb.epnwcf.com

[S47] C++：结构化绑定遍历
来源：http://jhw.hesvh.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://svm.jinghuilouyu.cn

[S48] C++：逐行读文件
来源：http://sdj.316326.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://yin.cheryme.top

while (std::getline(in, line)) { }
来源：http://lvk.yj20258888.top

[S49] C++：写文件
来源：http://gzw.hcnkem.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vvz.daxiang520.top

[S50] C++：格式化数字
来源：http://toz.zdbjq.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jxu.kuanghao11.cn

[S51] C++：显式类型转换
来源：http://ouh.pycfn.com

static_cast<double>(a) / b
来源：http://xkp.fanxiaobao.xyz

[S52] C++：const 与 noexcept
来源：http://fni.jinqigufen.top

int size() const noexcept { return n_; }
来源：http://aew.havefunace.top

[S53] C++：移动语义
来源：http://wnh.cucudq.cn

std::vector<int> w = std::move(v);
来源：http://wlk.vehdjk.com

[S54] C++：异常处理
来源：http://tlf.shanyushiyangkeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qhg.yuanzhike.top

[S55] C++：结构化绑定
来源：http://vhs.jqgufenzy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://xqj.shangyingyoupin.top

[S56] C++：optional
来源：http://gio.zycfv.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ejo.gaohongyu789.top

[S57] C++：编译期常量
来源：http://han.jqgfzy.top

constexpr int N = 10;
来源：http://asu.aibaodan.cn

[S58] C++：命名空间
来源：http://cfu.yongpay.top

namespace ns { int f() { return 1; } }
来源：http://hff.haohaochexian.top

[S59] C++：静态断言
来源：http://jxo.aizwys.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wnc.vqdsnc.cn

[S60] C++：遍历并删除元素
来源：http://oum.cqqwz.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rjb.zhixingplan.top

================================================================================
来源：http://eua.hesvh.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mga.wangdashe.top

================================================================================
来源：http://sfp.hcnkem.com

[T01] Kotlin：Hello World
来源：http://cbp.aizwys.cn

println("Hello")
来源：http://yxd.guowangkeji.top

[T02] Kotlin：变量
来源：http://cny.meibo888.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hxj.vehdjk.com

[T03] Kotlin：字符串模板
来源：http://fnz.hysaishi.cn

"值: $b"
来源：http://kii.tianlin.xyz

[T04] Kotlin：空安全
来源：http://iwp.jiagoushi.top

val n: String? = null;  n?.length
来源：http://zgu.daria6918.cn

[T05] Kotlin：when 表达式
来源：http://faj.ctjpmb.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://leh.zhongyouzk.top

[T06] Kotlin：集合映射
来源：http://czk.jinqigufen.top

listOf(1, 2, 3).map { it * 2 }
来源：http://jwv.sjlbkw.cn

[T07] Kotlin：集合过滤
来源：http://dli.quarkkingdee.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://bir.aizwys.cn

[T08] Kotlin：数据类
来源：http://oww.yuxming.cn

data class User(val name: String, val age: Int)
来源：http://qpw.havefunace.top

[T09] Kotlin：扩展函数
来源：http://opq.nanxinkj.top

fun String.exclaim() = this + "!"
来源：http://rsy.nwbrower.top

[T10] Kotlin：默认参数
来源：http://awv.hesvh.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ioo.andypj.xyz

[T11] Kotlin：协程
来源：http://pcl.sjlbkw.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://oej.yueranfly.top

[T12] Kotlin：解构声明
来源：http://uvc.tianlin.xyz

val (a, b) = Pair(1, 2)
来源：http://mue.hnqzz.top

[T13] Kotlin：只读 Map
来源：http://cnh.jinyuanbaomall.cn

val m = mapOf("a" to 1)
来源：http://fbc.0kj1m.cn

[T14] Kotlin：循环
来源：http://ixi.vehdjk.com

for (i in 1..10) println(i)
来源：http://ulo.hcnkem.com

[T15] Kotlin：接口
来源：http://kua.aizwys.cn

interface Shape { fun area(): Double }
来源：http://kud.yuanzhike.top

[T16] Swift：Hello World
来源：http://kyb.tarul.cn

print("Hello")
来源：http://jsp.xinyue.icu

[T17] Swift：变量与常量
来源：http://liw.ppjwa.cn

var a = 1;  let b = 2
来源：http://own.zdqjudy.top

[T18] Swift：字符串插值
来源：http://rlu.zycfv.cn

"值: \(b)"
来源：http://uxc.hfpthk.cn

[T19] Swift：可选绑定
来源：http://aiw.gotoacloud.top

if let n = opt { print(n) }
来源：http://suv.haohaochexian.top

[T20] Swift：数组操作
来源：http://qwe.tianlin.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://gjk.hnxiangtu.top

[T21] Swift：遍历
来源：http://wew.fehbvm.com

for x in a { print(x) }
来源：http://ihy.dianchejie.cn

[T22] Swift：字典
来源：http://mkx.bbcook.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zdb.havefunace.top

[T23] Swift：函数
来源：http://rjl.havefunace.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cvh.daria6918.cn

[T24] Swift：闭包
来源：http://wzx.cucudq.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://jjj.dashuyun.cn

[T25] Swift：结构体
来源：http://vrv.chenjidiqi.icu

struct P { var x: Int }
来源：http://ngk.hfpthk.cn

[T26] Swift：类与重写
来源：http://tiw.zhixingplan.top

class A: Base { override func f() {} }
来源：http://ubh.sysykeji.top

[T27] Swift：错误处理
来源：http://cyp.hcnkem.com

do { try f() } catch { print(error) }
来源：http://kxc.ctjpmb.com

[T28] Swift：枚举
来源：http://ria.yonumen.top

enum Color { case red, green }
来源：http://uii.jinyuanbaomall.cn

[T29] Swift：guard 提前返回
来源：http://cep.wangshuangyany.cn

guard let x = opt else { return }
来源：http://phu.dianchejie.cn

[T30] Swift：协议
来源：http://agt.fehbvm.com

protocol Shape { func area() -> Double }
来源：http://jys.daria6918.cn

[T31] Lua：Hello World
来源：http://gvt.fengsongda.top

print("Hello")
来源：http://hia.uphjek.com

[T32] Lua：局部变量
来源：http://ofu.cucudq.cn

local a = 1
来源：http://yha.shanyushiyangtech.top

[T33] Lua：表（数组）
来源：http://mqk.jlsjyb.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zrb.zhiwuduotai.top

[T34] Lua：遍历表
来源：http://del.yuanzhike.top

for i, v in ipairs(t) do print(i, v) end
来源：http://wbf.zhengqikj.top

[T35] Lua：字典表
来源：http://zsi.52xcode.cn

local d = { a = 1 };  d.b = 2
来源：http://vpv.daria6918.cn

[T36] Lua：函数
来源：http://gos.hammf.cn

function add(a, b) return a + b end
来源：http://epu.jinghuilouyu.cn

[T37] Lua：字符串拼接
来源：http://oqf.shanyushiyangtech.top

"a" .. "b"
来源：http://dps.sxryk.cn

[T38] Lua：条件
来源：http://hez.316326.xyz

if x > 0 then print("正") end
来源：http://kcv.chenlongwang.top

[T39] Lua：模式匹配
来源：http://hgj.cdnleiting.top

string.find(s, "%d+")
来源：http://akm.nanxuanxn.top

[T40] Lua：元表
来源：http://nag.jinqigfzy.top

setmetatable({}, { __index = base })
来源：http://ong.xuanzx.com

[T41] Perl：Hello World
来源：http://iby.gogol.net.cn

print "Hello\n";
来源：http://myj.jianghu66.top

[T42] Perl：变量类型
来源：http://zet.fktsv.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://imv.yj202588.top

[T43] Perl：字符串插值
来源：http://imn.nanxuanxn.top

"值: $a"
来源：http://tos.shanyushiyangtech.top

[T44] Perl：条件
来源：http://eaq.gaohongyu789.top

if ($a > 0) { print "正"; }
来源：http://boo.dianchejie.cn

[T45] Perl：数组遍历
来源：http://iul.meibo888.top

for my $x (@arr) { print $x; }
来源：http://kez.chenlongwang.top

[T46] Perl：哈希操作
来源：http://ghw.yj20258.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jdy.bjfxy.top

[T47] Perl：正则捕获
来源：http://qxa.daria6918.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://oiu.yanxiufei.cn

[T48] Perl：正则替换
来源：http://mnv.shzxlz.cn

$s =~ s/old/new/g;
来源：http://pxy.ywan-chungtsiang.top

[T49] Perl：函数
来源：http://qia.fanxiaobao.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hhn.zdbjq.cn

[T50] Perl：逐行读文件
来源：http://hhf.cucudq.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://dwx.fktsv.cn

while (my $line = <$fh>) { print $line; }
来源：http://cot.cqqwz.cn

[T51] Scala：Hello World
来源：http://dgz.vqdsnc.cn

println("Hello")
来源：http://wwc.ctjpmb.com

[T52] Scala：变量
来源：http://keg.zhoulong.xyz

val a = 1;  var b = 2
来源：http://fuu.cheryme.top

[T53] Scala：字符串插值
来源：http://aru.xziqi.cn

s"值: $b"
来源：http://pah.chenlongwang.top

[T54] Scala：集合映射
来源：http://eow.ehwqpu.com

List(1, 2, 3).map(_ * 2)
来源：http://zbq.jqgfzy.top

[T55] Scala：集合过滤
来源：http://yqi.tian-w.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xjq.hfpthk.cn

[T56] Scala：样例类
来源：http://dgn.chenzaomai.com

case class User(name: String, age: Int)
来源：http://jwz.vehdjk.com

[T57] Scala：模式匹配
来源：http://ufy.ydzc1.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ybq.aibaodan.cn

[T58] Scala：函数定义
来源：http://dzp.iojbl.cn

def add(a: Int, b: Int): Int = a + b
来源：http://eyi.zycfv.cn

[T59] Scala：循环
来源：http://aba.epnwcf.com

for (i <- 1 to 10) println(i)
来源：http://ufa.svipenyu.cn

[T60] Scala：折叠
来源：http://fwe.zhaomingkeji.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kuc.9152youxi.cn

================================================================================
来源：http://rof.yangfankeji.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://aqk.cucudq.cn

================================================================================
来源：http://ejz.nanxuanxn.top

[U01] Py：创建虚拟环境
来源：http://uno.hongshengwenyu.top

python -m venv .venv && source .venv/bin/activate
来源：http://ran.gaohongyu789.top

[U02] Py：导出 / 安装依赖
来源：http://bql.jianghu66.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://xbm.sysykeji.top

[U03] Py：加载 .env 配置
来源：http://oee.jqgufenzy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ynq.shanyushiyangtech.top

[U04] Py：变量调试打印
来源：http://gvk.zhengqikj.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dvt.nwbrower.top

[U05] Py：列表去重且保序
来源：http://qms.wangshuangyany.cn

list(dict.fromkeys(arr))
来源：http://lbv.dashuyun.cn

[U06] Py：合并两个字典
来源：http://sdq.xziqi.cn

{**a, **b}
来源：http://ydw.sjlbkw.cn

[U07] Py：反转字典键值
来源：http://boo.jinyuanbaomall.cn

{v: k for k, v in d.items()}
来源：http://alz.yj20258.top

[U08] Py：展平二维列表
来源：http://mas.xuetiantiany.cn

[y for x in nested for y in x]
来源：http://cuc.zhengqikj.top

[U09] Py：字典取最大值的键
来源：http://bos.pengpengdd.cyou

max(d, key=d.get)
来源：http://glx.bjfxy.top

[U10] Py：按值排序字典
来源：http://qhy.ctjpmb.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sxa.vehdjk.com

[U11] Py：生成器表达式
来源：http://qrr.gzhubu.top

(x * 2 for x in arr)
来源：http://war.redwolf501.top

[U12] Py：取出现最多的 3 个元素
来源：http://utr.jinqigufen.top

Counter(arr).most_common(3)
来源：http://cdm.havefunace.top

[U13] Py：固定长度队列
来源：http://eic.vqdsnc.cn

deque(maxlen=10)
来源：http://ljr.haohaochexian.top

[U14] Py：分组收集到列表
来源：http://fcg.zhiwuduotai.top

defaultdict(list)
来源：http://lqi.iojbl.cn

[U15] Py：高精度计时
来源：http://cfn.andypj.xyz

t = time.perf_counter()
来源：http://xim.xziqi.cn

[U16] Py：命令行参数解析
来源：http://lpb.yueranfly.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://odr.xinyue.icu

[U17] Py：初始化日志
来源：http://igg.hfpthk.cn

logging.basicConfig(level=logging.INFO)
来源：http://mel.daria6918.cn

[U18] Py：预编译正则
来源：http://spu.jinyuanbaomall.cn

pat = re.compile(r"\d+")
来源：http://mqt.hesvh.cn

[U19] Py：正则替换带回调
来源：http://rcu.cashguo.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ulq.zycfv.cn

[U20] Py：缓存函数结果
来源：http://ktv.zdqjudy.top

@functools.lru_cache(maxsize=None)
来源：http://jjd.hesvh.cn

[U21] Py：自定义上下文管理器
来源：http://zfp.jinqigfzy.top

@contextlib.contextmanager
来源：http://moj.xingfuxueyuan.xyz

[U22] Py：矩阵转置
来源：http://jta.sweek.top

list(zip(*m))
来源：http://jva.hfpthk.cn

[U23] Py：分块读取大文件
来源：http://aps.pycfn.com

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nhp.jinghuilouyu.cn

[U24] Py：路径操作
来源：http://vwg.fanxiaobao.xyz

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://wnl.zdbjq.cn

[U25] Py：CSV 按字典读
来源：http://yir.hcnkem.com

csv.DictReader(f)
来源：http://jzt.zycfv.cn

[U26] Py：并发下载
来源：http://rsg.wangdashe.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jmb.shangyingyoupin.top

[U27] Py：异步 HTTP
来源：http://xps.0kj1m.cn

aiohttp.ClientSession() 配合 async with
来源：http://nyk.9152youxi.cn

[U28] Py：类型别名
来源：http://abt.nanxinkj.top

UserId = int
来源：http://nqf.zhijiandao.cn

[U29] Py：属性校验
来源：http://qka.jlsjyb.cn

@property 与 @x.setter 配合
来源：http://voe.ybcxt.top

[U30] Py：数据类
来源：http://rch.zhengqikj.top

@dataclass(slots=True)
来源：http://xnr.nanxinkj.top

[U31] Py：单测
来源：http://icd.pengpengdd.cyou

python -m pytest -q
来源：http://hzd.sjlbkw.cn

[U32] Py：代码格式化
来源：http://wyd.jqgufenzy.top

ruff format . && ruff check --fix .
来源：http://ive.cucudq.cn

[U33] Py：打包发布
来源：http://tzr.bjfxy.top

python -m build  （依赖 pyproject.toml）
来源：http://epr.yangfankeji.com

[U34] Py：判断编码
来源：http://tru.zhengqikj.top

chardet.detect(raw)
来源：http://ema.ehwqpu.com


<!-- 参考信息 -->