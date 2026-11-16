代发 wailian999

int x; scanf("%d", &x);
来源：http://yfo.zhoulong.xyz

[S04] C：字符串复制
来源：http://nvn.9152youxi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gwz.jqgufenzy.top

[S05] C：字符串长度
来源：http://egk.yuanzhike.top

strlen(s)
来源：http://gjz.redwolf501.top

[S06] C：字符串比较
来源：http://gdz.yj202588.top

strcmp(a, b) == 0
来源：http://oco.yueranfly.top

[S07] C：数组遍历求和
来源：http://aql.jianghu66.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wly.jinqigufen.top

[S08] C：动态内存分配与释放
来源：http://koe.guannengcc.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lij.feifeiyinyue.top

[S09] C：结构体定义与初始化
来源：http://lti.epnwcf.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qoj.chenzaomai.com

[S10] C：指针与解引用
来源：http://kwp.redwolf501.top

int *p = &a;  *p = 5;
来源：http://hph.zhongyouzk.top

[S11] C：逐行读文件
来源：http://ffj.yvedp.cn

FILE *f = fopen("a.txt", "r");
来源：http://cfp.zhengqikj.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://rbm.meibo888.top

fclose(f);
来源：http://vfc.fengsongda.top

[S12] C：写文件
来源：http://hun.xuanzx.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ryk.yuxming.cn

[S13] C：宏定义
来源：http://lgk.dashuyun.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://syw.sxryk.cn

[S14] C：枚举
来源：http://yvi.guowangkeji.top

enum Color { RED, GREEN, BLUE };
来源：http://wux.yangfankeji.com

[S15] C：类型转换
来源：http://vlb.sufxvd.cn

(double) a / b
来源：http://utc.bbcook.cn

[S16] C：位操作置位
来源：http://ibn.hammf.cn

x |= (1 << 3);
来源：http://ibm.hammf.cn

[S17] C：安全拼接字符串
来源：http://gis.fehbvm.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wag.daria6918.cn

[S18] C：命令行参数
来源：http://xra.zdbjq.cn

int main(int argc, char **argv)
来源：http://cdo.sweek.top

[S19] C：快速排序
来源：http://pzo.yanxiufei.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ykv.ydzc1.top

[S20] C：二分查找
来源：http://nui.hammf.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://eye.zhaomingkeji.xyz

[S21] C：字符类别判断
来源：http://gzo.aibaodan.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ulf.hcnkem.com

[S22] C：字符串转数字
来源：http://sgd.zhiwuduotai.top

atoi("42");  strtod("3.14", NULL);
来源：http://luk.yonumen.top

[S23] C：随机数
来源：http://xhq.sufxvd.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bmf.yj20258.top

[S24] C：获取本地时间
来源：http://lkz.bjfxy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hda.tianlin.xyz

[S25] C：内存拷贝
来源：http://eut.ehwqpu.com

memcpy(dst, src, n);
来源：http://kja.shanyushiyangkeji.top

[S26] C：内存清零
来源：http://swp.zhixingplan.top

memset(a, 0, sizeof a);
来源：http://khf.gogol.net.cn

[S27] C：定义常量
来源：http://mvu.uphjek.com

const double PI = 3.14159;
来源：http://khr.uphjek.com

[S28] C：静态变量
来源：http://vhw.feifeiyinyue.top

static int counter = 0;
来源：http://dhg.yangfankeji.com

[S29] C：变参函数
来源：http://hgo.zhoulong.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nwy.snrcjt.cn

[S30] C：头文件保护
来源：http://dhj.cheryme.top

#ifndef X_H
来源：http://mqo.ehwqpu.com

#define X_H
来源：http://ehr.ybcxt.top

#endif
来源：http://ncq.gaohongyu789.top

[S31] C++：Hello World
来源：http://fts.gotoacloud.top

#include <iostream>
来源：http://qrq.xziqi.cn

int main() { std::cout << "Hello\n"; }
来源：http://pho.ydjk.org.cn

[S32] C++：字符串
来源：http://fkq.guowangkeji.top

std::string s = "hi";  s += "!";
来源：http://zhi.zhiwuduotai.top

[S33] C++：vector 增删
来源：http://qnx.zhaomingkeji.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yxs.hesvh.cn

[S34] C++：遍历 vector
来源：http://ald.fktsv.cn

for (auto &x : v) { std::cout << x; }
来源：http://jcx.havefunace.top

[S35] C++：map
来源：http://ggc.c1oappe.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://akp.hesvh.cn

[S36] C++：unordered_map
来源：http://ght.tian-w.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://iyo.svipenyu.cn

[S37] C++：set
来源：http://ltj.pycfn.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://uga.zdqjudy.top

[S38] C++：排序
来源：http://mmb.birdmap.top

std::sort(v.begin(), v.end());
来源：http://tlq.shuidangran.top

[S39] C++：自定义比较器排序
来源：http://esw.iojbl.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xbg.fengsongda.top

[S40] C++：查找元素
来源：http://swe.mhx1999.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pvz.daria6918.cn

[S41] C++：类与构造函数
来源：http://irp.316326.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gqq.quarkkingdee.top

[S42] C++：继承与虚函数
来源：http://pxl.fengsongda.top

class B : public Base { public: void f() override {} };
来源：http://kvp.hfpthk.cn

[S43] C++：智能指针
来源：http://ady.hongshengwenyu.top

auto p = std::make_unique<int>(5);
来源：http://wmr.jiagoushi.top

[S44] C++：引用传参
来源：http://gvl.yangfankeji.com

void inc(int &x) { ++x; }
来源：http://oir.chenzaomai.com

[S45] C++：lambda
来源：http://xrq.kuanghao11.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ayb.tanke756.top

[S46] C++：函数模板
来源：http://kvh.hnxiangtu.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cpr.hywenlv.cn

[S47] C++：结构化绑定遍历
来源：http://avb.fehbvm.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qxk.tarul.cn

[S48] C++：逐行读文件
来源：http://roq.yuxming.cn

std::ifstream in("a.txt");  std::string line;
来源：http://hqt.fanxiaobao.xyz

while (std::getline(in, line)) { }
来源：http://fuu.chenzaomai.com

[S49] C++：写文件
来源：http://qbd.cheryme.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://glm.cashguo.top

[S50] C++：格式化数字
来源：http://zcd.haohaochexian.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hvc.ivvv.top

[S51] C++：显式类型转换
来源：http://hok.jiagoushi.top

static_cast<double>(a) / b
来源：http://lsk.fehbvm.com

[S52] C++：const 与 noexcept
来源：http://mmz.sjlbkw.cn

int size() const noexcept { return n_; }
来源：http://iqk.jqgfzy.top

[S53] C++：移动语义
来源：http://ska.zdbjq.cn

std::vector<int> w = std::move(v);
来源：http://wwd.jqgfzy.top

[S54] C++：异常处理
来源：http://byb.guannengcc.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fzl.smart0.xyz

[S55] C++：结构化绑定
来源：http://vwc.9152youxi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xmp.cashguo.top

[S56] C++：optional
来源：http://eix.cdnleiting.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mjh.shangyingyoupin.top

[S57] C++：编译期常量
来源：http://xhk.0kj1m.cn

constexpr int N = 10;
来源：http://rwj.yangfankeji.com

[S58] C++：命名空间
来源：http://cfk.yongpay.top

namespace ns { int f() { return 1; } }
来源：http://xer.haohaochexian.top

[S59] C++：静态断言
来源：http://gmh.chenzaomai.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ury.ydjk.org.cn

[S60] C++：遍历并删除元素
来源：http://nwr.zycfv.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://buf.zhijiandao.cn

================================================================================
来源：http://aaf.kuanghao11.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fcm.tarul.cn

================================================================================
来源：http://omg.chenjidiqi.icu

[T01] Kotlin：Hello World
来源：http://eru.bjfxy.top

println("Hello")
来源：http://tfp.ydjk.org.cn

[T02] Kotlin：变量
来源：http://rwl.yuxming.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vkp.shanyushiyangtech.top

[T03] Kotlin：字符串模板
来源：http://hxw.birdmap.top

"值: $b"
来源：http://trn.zhixingplan.top

[T04] Kotlin：空安全
来源：http://oha.jlsjyb.cn

val n: String? = null;  n?.length
来源：http://uev.gotoacloud.top

[T05] Kotlin：when 表达式
来源：http://txw.meibo888.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pfw.xinyue.icu

[T06] Kotlin：集合映射
来源：http://gsw.zhoulong.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://umc.mhx1999.top

[T07] Kotlin：集合过滤
来源：http://kqi.hcnkem.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://gna.hnqzz.top

[T08] Kotlin：数据类
来源：http://mrh.hnxiangtu.top

data class User(val name: String, val age: Int)
来源：http://pss.zhoulong.xyz

[T09] Kotlin：扩展函数
来源：http://bwc.hnqzz.top

fun String.exclaim() = this + "!"
来源：http://ack.ctjpmb.com

[T10] Kotlin：默认参数
来源：http://elz.yuanzhike.top

fun greet(name: String = "World") = "Hi $name"
来源：http://xia.chenlongwang.top

[T11] Kotlin：协程
来源：http://prd.cashguo.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://hoi.cqqwz.cn

[T12] Kotlin：解构声明
来源：http://txl.chenzaomai.com

val (a, b) = Pair(1, 2)
来源：http://qgl.ehwqpu.com

[T13] Kotlin：只读 Map
来源：http://qqx.nanxuanxn.top

val m = mapOf("a" to 1)
来源：http://vxt.sjlbkw.cn

[T14] Kotlin：循环
来源：http://xrl.zhongyouzk.top

for (i in 1..10) println(i)
来源：http://jxn.birdmap.top

[T15] Kotlin：接口
来源：http://gvj.sweek.top

interface Shape { fun area(): Double }
来源：http://dnf.zhengqikj.top

[T16] Swift：Hello World
来源：http://csp.guowangkeji.top

print("Hello")
来源：http://vrl.yuxming.cn

[T17] Swift：变量与常量
来源：http://pfe.hnqzz.top

var a = 1;  let b = 2
来源：http://chl.c1oappe.top

[T18] Swift：字符串插值
来源：http://beu.xuetiantiany.cn

"值: \(b)"
来源：http://tcd.ppjwa.cn

[T19] Swift：可选绑定
来源：http://rnd.guannengcc.top

if let n = opt { print(n) }
来源：http://yin.zdqjudy.top

[T20] Swift：数组操作
来源：http://rfi.aibaodan.cn

var a = [1, 2, 3];  a.append(4)
来源：http://naw.shanyushiyangtech.top

[T21] Swift：遍历
来源：http://ogw.yongpay.top

for x in a { print(x) }
来源：http://qie.zhixingplan.top

[T22] Swift：字典
来源：http://sgn.havefunace.top

var d = ["a": 1];  d["b"] = 2
来源：http://jtm.tian-w.cn

[T23] Swift：函数
来源：http://cmb.zhengqikj.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nvc.tanke756.top

[T24] Swift：闭包
来源：http://rlt.0kj1m.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://mwv.yj20258888.top

[T25] Swift：结构体
来源：http://dde.jinghuilouyu.cn

struct P { var x: Int }
来源：http://dir.jianghu66.top

[T26] Swift：类与重写
来源：http://fvy.zhoulong.xyz

class A: Base { override func f() {} }
来源：http://bme.fktsv.cn

[T27] Swift：错误处理
来源：http://wew.aibaodan.cn

do { try f() } catch { print(error) }
来源：http://nys.jianghu66.top

[T28] Swift：枚举
来源：http://fmv.pycfn.com

enum Color { case red, green }
来源：http://nfd.9152youxi.cn

[T29] Swift：guard 提前返回
来源：http://xbx.hywenlv.cn

guard let x = opt else { return }
来源：http://etg.guowangkeji.top

[T30] Swift：协议
来源：http://bdh.meibo888.top

protocol Shape { func area() -> Double }
来源：http://piv.pycfn.com

[T31] Lua：Hello World
来源：http://zmj.zhongyouzk.top

print("Hello")
来源：http://luq.pycfn.com

[T32] Lua：局部变量
来源：http://nrl.cqqwz.cn

local a = 1
来源：http://rny.gaohongyu789.top

[T33] Lua：表（数组）
来源：http://kga.zhijiandao.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://otc.0kj1m.cn

[T34] Lua：遍历表
来源：http://xsl.shanyushiyangkeji.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ugl.xingfuxueyuan.xyz

[T35] Lua：字典表
来源：http://asl.zhengqikj.top

local d = { a = 1 };  d.b = 2
来源：http://jdd.wangshuangyany.cn

[T36] Lua：函数
来源：http://ary.daxiang520.top

function add(a, b) return a + b end
来源：http://sbw.jiagoushi.top

[T37] Lua：字符串拼接
来源：http://hzn.smart0.xyz

"a" .. "b"
来源：http://kgj.nwbrower.top

[T38] Lua：条件
来源：http://rrx.zhengqikj.top

if x > 0 then print("正") end
来源：http://bzl.yanxiufei.cn

[T39] Lua：模式匹配
来源：http://ddm.feifeiyinyue.top

string.find(s, "%d+")
来源：http://lwb.316326.xyz

[T40] Lua：元表
来源：http://oxl.zhengqikj.top

setmetatable({}, { __index = base })
来源：http://vwm.fktsv.cn

[T41] Perl：Hello World
来源：http://crs.cashguo.top

print "Hello\n";
来源：http://cnx.hywenlv.cn

[T42] Perl：变量类型
来源：http://qxm.kuanghao11.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ysi.nanxuanxn.top

[T43] Perl：字符串插值
来源：http://jls.mhx1999.top

"值: $a"
来源：http://aqz.yongpay.top

[T44] Perl：条件
来源：http://wgk.havefunace.top

if ($a > 0) { print "正"; }
来源：http://qll.cqqwz.cn

[T45] Perl：数组遍历
来源：http://axj.ivvv.top

for my $x (@arr) { print $x; }
来源：http://lyh.chenzaomai.com

[T46] Perl：哈希操作
来源：http://lcx.feifeiyinyue.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ole.dianchejie.cn

[T47] Perl：正则捕获
来源：http://xbs.hywenlv.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xxp.gotoacloud.top

[T48] Perl：正则替换
来源：http://ehb.hammf.cn

$s =~ s/old/new/g;
来源：http://lts.fzhhl.top

[T49] Perl：函数
来源：http://ghz.yj20258888.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://aup.haohaochexian.top

[T50] Perl：逐行读文件
来源：http://dpb.jinyuanbaomall.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://mbv.gogol.net.cn

while (my $line = <$fh>) { print $line; }
来源：http://jfn.daxiang520.top

[T51] Scala：Hello World
来源：http://rtu.316326.xyz

println("Hello")
来源：http://lcl.yj20258888.top

[T52] Scala：变量
来源：http://hlf.xylfe.cn

val a = 1;  var b = 2
来源：http://ydi.birdmap.top

[T53] Scala：字符串插值
来源：http://jkm.aizwys.cn

s"值: $b"
来源：http://bhi.dianchejie.cn

[T54] Scala：集合映射
来源：http://dxq.shuidangran.top

List(1, 2, 3).map(_ * 2)
来源：http://txn.bbcook.cn

[T55] Scala：集合过滤
来源：http://aef.tanke756.top

List(1, 2, 3).filter(_ > 1)
来源：http://vol.zycfv.cn

[T56] Scala：样例类
来源：http://ngl.c1oappe.top

case class User(name: String, age: Int)
来源：http://djo.fanxiaobao.xyz

[T57] Scala：模式匹配
来源：http://qdu.gotoacloud.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://fxy.nanxuanxn.top

[T58] Scala：函数定义
来源：http://grc.sufxvd.cn

def add(a: Int, b: Int): Int = a + b
来源：http://fbm.zhiwuduotai.top

[T59] Scala：循环
来源：http://vwg.cheryme.top

for (i <- 1 to 10) println(i)
来源：http://swo.cdnleiting.top

[T60] Scala：折叠
来源：http://tdq.hnqzz.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yhb.yanxiufei.cn

================================================================================
来源：http://wcn.redwolf501.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://aie.jinqigufen.top

================================================================================
来源：http://fyf.zdbjq.cn

[U01] Py：创建虚拟环境
来源：http://ulw.tanke756.top

python -m venv .venv && source .venv/bin/activate
来源：http://uzb.yuanzhike.top

[U02] Py：导出 / 安装依赖
来源：http://vlh.wangdashe.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://btk.tian-w.cn

[U03] Py：加载 .env 配置
来源：http://wll.smart0.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://jan.yangfankeji.com

[U04] Py：变量调试打印
来源：http://byr.zhiwuduotai.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://syp.jqgfzy.top

[U05] Py：列表去重且保序
来源：http://kvm.yangfankeji.com

list(dict.fromkeys(arr))
来源：http://mny.fzhhl.top

[U06] Py：合并两个字典
来源：http://xos.yueranfly.top

{**a, **b}
来源：http://ztp.yuxming.cn

[U07] Py：反转字典键值
来源：http://nyz.daria6918.cn

{v: k for k, v in d.items()}
来源：http://jga.hywenlv.cn

[U08] Py：展平二维列表
来源：http://xpj.zhixingplan.top

[y for x in nested for y in x]
来源：http://wwu.shuidangran.top

[U09] Py：字典取最大值的键
来源：http://wpf.guannengcc.top

max(d, key=d.get)
来源：http://qkn.chenjidiqi.icu

[U10] Py：按值排序字典
来源：http://obb.gogol.net.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mmu.yj20258888.top

[U11] Py：生成器表达式
来源：http://mam.chenlongwang.top

(x * 2 for x in arr)
来源：http://vrc.yuxming.cn

[U12] Py：取出现最多的 3 个元素
来源：http://hyc.bjfxy.top

Counter(arr).most_common(3)
来源：http://thj.sjlbkw.cn

[U13] Py：固定长度队列
来源：http://mkl.chenjidiqi.icu

deque(maxlen=10)
来源：http://bhf.xinyue.icu

[U14] Py：分组收集到列表
来源：http://jtt.jianghu66.top

defaultdict(list)
来源：http://zfp.xylfe.cn

[U15] Py：高精度计时
来源：http://idd.sufxvd.cn

t = time.perf_counter()
来源：http://blc.yanxiufei.cn

[U16] Py：命令行参数解析
来源：http://jvm.xingfuxueyuan.xyz

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zha.ydzc1.top

[U17] Py：初始化日志
来源：http://wut.vqdsnc.cn

logging.basicConfig(level=logging.INFO)
来源：http://gxz.shuidangran.top

[U18] Py：预编译正则
来源：http://xuc.shzxlz.cn

pat = re.compile(r"\d+")
来源：http://mwh.zhijiandao.cn

[U19] Py：正则替换带回调
来源：http://dkf.gogol.net.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xin.sxryk.cn

[U20] Py：缓存函数结果
来源：http://wkw.9152youxi.cn

@functools.lru_cache(maxsize=None)
来源：http://zda.ppjwa.cn

[U21] Py：自定义上下文管理器
来源：http://qlb.9152youxi.cn

@contextlib.contextmanager
来源：http://wee.vehdjk.com

[U22] Py：矩阵转置
来源：http://vmw.haohaochexian.top

list(zip(*m))
来源：http://jek.yanxiufei.cn

[U23] Py：分块读取大文件
来源：http://vja.xingfuxueyuan.xyz

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lnl.snrcjt.cn

[U24] Py：路径操作
来源：http://bdw.hammf.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://drl.cheryme.top

[U25] Py：CSV 按字典读
来源：http://wer.fanxiaobao.xyz

csv.DictReader(f)
来源：http://gcn.nanxuanxn.top

[U26] Py：并发下载
来源：http://ksi.yuxming.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mbs.zhiwuduotai.top


<!-- 参考信息 -->