代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rqi.9152youxi.cn

[S08] C：动态内存分配与释放
来源：http://ips.cqqwz.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lhp.cdnleiting.top

[S09] C：结构体定义与初始化
来源：http://swj.fzhhl.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dif.guannengcc.top

[S10] C：指针与解引用
来源：http://xkc.zdbjq.cn

int *p = &a;  *p = 5;
来源：http://cld.yanxiufei.cn

[S11] C：逐行读文件
来源：http://qft.nanxinkj.top

FILE *f = fopen("a.txt", "r");
来源：http://jrt.9152youxi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://yzm.ydzc1.top

fclose(f);
来源：http://ilu.dianchejie.cn

[S12] C：写文件
来源：http://qwz.yuanzhike.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blk.iojbl.cn

[S13] C：宏定义
来源：http://cvp.jinqigfzy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ipt.smart0.xyz

[S14] C：枚举
来源：http://exv.xinyue.icu

enum Color { RED, GREEN, BLUE };
来源：http://krc.zhoulong.xyz

[S15] C：类型转换
来源：http://ezo.shangyingyoupin.top

(double) a / b
来源：http://opd.jyoumei.cn

[S16] C：位操作置位
来源：http://eyu.jinqigufen.top

x |= (1 << 3);
来源：http://vbz.zhaomingkeji.xyz

[S17] C：安全拼接字符串
来源：http://qfb.jqgufenzy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mlu.svipenyu.cn

[S18] C：命令行参数
来源：http://sxa.chenlongwang.top

int main(int argc, char **argv)
来源：http://kxm.ppjwa.cn

[S19] C：快速排序
来源：http://ogd.vehdjk.com

qsort(a, n, sizeof(int), cmp);
来源：http://dqf.redwolf501.top

[S20] C：二分查找
来源：http://ygq.jianghu66.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://frt.zdqjudy.top

[S21] C：字符类别判断
来源：http://ucr.tanke756.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wvz.hnqzz.top

[S22] C：字符串转数字
来源：http://auf.chenlongwang.top

atoi("42");  strtod("3.14", NULL);
来源：http://nyv.xuanzx.com

[S23] C：随机数
来源：http://wcs.sufxvd.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vgq.ivvv.top

[S24] C：获取本地时间
来源：http://yqv.epnwcf.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dyy.vqdsnc.cn

[S25] C：内存拷贝
来源：http://dte.daria6918.cn

memcpy(dst, src, n);
来源：http://dnz.hcnkem.com

[S26] C：内存清零
来源：http://jky.xylfe.cn

memset(a, 0, sizeof a);
来源：http://bkp.hongshengwenyu.top

[S27] C：定义常量
来源：http://bww.yuanzhike.top

const double PI = 3.14159;
来源：http://llg.zycfv.cn

[S28] C：静态变量
来源：http://sdw.yj202588.top

static int counter = 0;
来源：http://usz.jiagoushi.top

[S29] C：变参函数
来源：http://qgv.zhiwuduotai.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mwq.sweek.top

[S30] C：头文件保护
来源：http://heq.fehbvm.com

#ifndef X_H
来源：http://qdl.nwbrower.top

#define X_H
来源：http://hzh.sxryk.cn

#endif
来源：http://vfv.hongshengwenyu.top

[S31] C++：Hello World
来源：http://bjd.hongshengwenyu.top

#include <iostream>
来源：http://hhu.yanxiufei.cn

int main() { std::cout << "Hello\n"; }
来源：http://uhd.haohaochexian.top

[S32] C++：字符串
来源：http://dob.xuetiantiany.cn

std::string s = "hi";  s += "!";
来源：http://aib.ydjk.org.cn

[S33] C++：vector 增删
来源：http://brn.ydjk.org.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bzf.sweek.top

[S34] C++：遍历 vector
来源：http://wpj.gaohongyu789.top

for (auto &x : v) { std::cout << x; }
来源：http://ehs.ehwqpu.com

[S35] C++：map
来源：http://uxi.hnqzz.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hgs.yuanzhike.top

[S36] C++：unordered_map
来源：http://rqe.jinqigfzy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://geo.c1oappe.top

[S37] C++：set
来源：http://ywt.ehwqpu.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qyk.nanxinkj.top

[S38] C++：排序
来源：http://ner.nwbrower.top

std::sort(v.begin(), v.end());
来源：http://ngr.hywenlv.cn

[S39] C++：自定义比较器排序
来源：http://kbm.hfpthk.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vxg.nanxuanxn.top

[S40] C++：查找元素
来源：http://ilg.snrcjt.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://krm.xylfe.cn

[S41] C++：类与构造函数
来源：http://uog.zhengqikj.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cmo.yongpay.top

[S42] C++：继承与虚函数
来源：http://jji.fehbvm.com

class B : public Base { public: void f() override {} };
来源：http://sqh.shangyingyoupin.top

[S43] C++：智能指针
来源：http://mfy.shangyingyoupin.top

auto p = std::make_unique<int>(5);
来源：http://cmi.tarul.cn

[S44] C++：引用传参
来源：http://mzc.sufxvd.cn

void inc(int &x) { ++x; }
来源：http://ijg.ydjk.org.cn

[S45] C++：lambda
来源：http://gav.shuidangran.top

auto add = [](int a, int b) { return a + b; };
来源：http://ryz.sjlbkw.cn

[S46] C++：函数模板
来源：http://nes.yfazqb.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gdl.ctjpmb.com

[S47] C++：结构化绑定遍历
来源：http://tbi.yj20258888.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://shr.guowangkeji.top

[S48] C++：逐行读文件
来源：http://awk.xuetiantiany.cn

std::ifstream in("a.txt");  std::string line;
来源：http://enl.ybcxt.top

while (std::getline(in, line)) { }
来源：http://gxt.sweek.top

[S49] C++：写文件
来源：http://nwr.sufxvd.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hov.shzxlz.cn

[S50] C++：格式化数字
来源：http://hck.jyoumei.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ugi.yongpay.top

[S51] C++：显式类型转换
来源：http://neu.cqqwz.cn

static_cast<double>(a) / b
来源：http://mkm.tianlin.xyz

[S52] C++：const 与 noexcept
来源：http://ykw.yueranfly.top

int size() const noexcept { return n_; }
来源：http://fpn.iojbl.cn

[S53] C++：移动语义
来源：http://wwz.pengpengdd.cyou

std::vector<int> w = std::move(v);
来源：http://wsi.ppjwa.cn

[S54] C++：异常处理
来源：http://snq.jlsjyb.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://upa.bjfxy.top

[S55] C++：结构化绑定
来源：http://oyo.316326.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://cau.hfpthk.cn

[S56] C++：optional
来源：http://uag.ctjpmb.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tfm.quarkkingdee.top

[S57] C++：编译期常量
来源：http://cpe.uphjek.com

constexpr int N = 10;
来源：http://ncn.pycfn.com

[S58] C++：命名空间
来源：http://dzh.xingfuxueyuan.xyz

namespace ns { int f() { return 1; } }
来源：http://nmq.fktsv.cn

[S59] C++：静态断言
来源：http://lqi.smart0.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://beh.redwolf501.top

[S60] C++：遍历并删除元素
来源：http://yzy.yuxming.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zwj.jinghuilouyu.cn

================================================================================
来源：http://ipr.sufxvd.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fqn.havefunace.top

================================================================================
来源：http://xaz.jinyuanbaomall.cn

[T01] Kotlin：Hello World
来源：http://nsq.cucudq.cn

println("Hello")
来源：http://tzo.zhengqikj.top

[T02] Kotlin：变量
来源：http://ndq.fanxiaobao.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tfa.xingfuxueyuan.xyz

[T03] Kotlin：字符串模板
来源：http://qpf.jlsjyb.cn

"值: $b"
来源：http://zuw.fehbvm.com

[T04] Kotlin：空安全
来源：http://kyd.cashguo.top

val n: String? = null;  n?.length
来源：http://yok.cdnleiting.top

[T05] Kotlin：when 表达式
来源：http://fsf.tarul.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xim.jinyuanbaomall.cn

[T06] Kotlin：集合映射
来源：http://gwf.dianchejie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://vtw.haohaochexian.top

[T07] Kotlin：集合过滤
来源：http://tnt.yuxming.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://tfe.chenzaomai.com

[T08] Kotlin：数据类
来源：http://zai.guannengcc.top

data class User(val name: String, val age: Int)
来源：http://uoi.shangyingyoupin.top

[T09] Kotlin：扩展函数
来源：http://jvx.zhiwuduotai.top

fun String.exclaim() = this + "!"
来源：http://jsb.yongpay.top

[T10] Kotlin：默认参数
来源：http://dyw.c1oappe.top

fun greet(name: String = "World") = "Hi $name"
来源：http://bom.fzhhl.top

[T11] Kotlin：协程
来源：http://oie.gogol.net.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://leb.yfazqb.com

[T12] Kotlin：解构声明
来源：http://zhh.hywenlv.cn

val (a, b) = Pair(1, 2)
来源：http://gqf.tarul.cn

[T13] Kotlin：只读 Map
来源：http://efg.hnxiangtu.top

val m = mapOf("a" to 1)
来源：http://qsw.ctjpmb.com

[T14] Kotlin：循环
来源：http://yiv.fktsv.cn

for (i in 1..10) println(i)
来源：http://njn.jinyuanbaomall.cn

[T15] Kotlin：接口
来源：http://ujv.zhoulong.xyz

interface Shape { fun area(): Double }
来源：http://odq.chenlongwang.top

[T16] Swift：Hello World
来源：http://yem.shuidangran.top

print("Hello")
来源：http://nbd.c1oappe.top

[T17] Swift：变量与常量
来源：http://shz.yj20258888.top

var a = 1;  let b = 2
来源：http://ttw.zhaomingkeji.xyz

[T18] Swift：字符串插值
来源：http://jph.cheryme.top

"值: \(b)"
来源：http://wpv.jqgufenzy.top

[T19] Swift：可选绑定
来源：http://xtd.cqqwz.cn

if let n = opt { print(n) }
来源：http://zys.sjlbkw.cn

[T20] Swift：数组操作
来源：http://clf.zdbjq.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fcg.jiagoushi.top

[T21] Swift：遍历
来源：http://gzl.jlsjyb.cn

for x in a { print(x) }
来源：http://cpf.jinyuanbaomall.cn

[T22] Swift：字典
来源：http://zcy.gogol.net.cn

var d = ["a": 1];  d["b"] = 2
来源：http://duu.gzhubu.top

[T23] Swift：函数
来源：http://ifk.bbcook.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xmb.daria6918.cn

[T24] Swift：闭包
来源：http://rey.haohaochexian.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://nco.shangyingyoupin.top

[T25] Swift：结构体
来源：http://kjt.uphjek.com

struct P { var x: Int }
来源：http://dfc.ivvv.top

[T26] Swift：类与重写
来源：http://sdi.hfpthk.cn

class A: Base { override func f() {} }
来源：http://vcr.feifeiyinyue.top

[T27] Swift：错误处理
来源：http://qup.hnqzz.top

do { try f() } catch { print(error) }
来源：http://ddp.shangyingyoupin.top

[T28] Swift：枚举
来源：http://tst.hammf.cn

enum Color { case red, green }
来源：http://ifn.ehwqpu.com

[T29] Swift：guard 提前返回
来源：http://amq.vqdsnc.cn

guard let x = opt else { return }
来源：http://wyr.jinghuilouyu.cn

[T30] Swift：协议
来源：http://gnh.yangfankeji.com

protocol Shape { func area() -> Double }
来源：http://rhh.zdqjudy.top

[T31] Lua：Hello World
来源：http://tay.fanxiaobao.xyz

print("Hello")
来源：http://arj.gaohongyu789.top

[T32] Lua：局部变量
来源：http://fcw.hongshengwenyu.top

local a = 1
来源：http://rnz.iojbl.cn

[T33] Lua：表（数组）
来源：http://ppg.c1oappe.top

local t = {1, 2, 3};  t[4] = 4
来源：http://deh.0kj1m.cn

[T34] Lua：遍历表
来源：http://rtr.cheryme.top

for i, v in ipairs(t) do print(i, v) end
来源：http://bdd.xingfuxueyuan.xyz

[T35] Lua：字典表
来源：http://jej.yj20258.top

local d = { a = 1 };  d.b = 2
来源：http://qbk.gotoacloud.top

[T36] Lua：函数
来源：http://xhr.dashuyun.cn

function add(a, b) return a + b end
来源：http://teo.zycfv.cn

[T37] Lua：字符串拼接
来源：http://tgf.jinghuilouyu.cn

"a" .. "b"
来源：http://aam.hnxiangtu.top

[T38] Lua：条件
来源：http://cmp.havefunace.top

if x > 0 then print("正") end
来源：http://mmw.andypj.xyz

[T39] Lua：模式匹配
来源：http://rkj.tanke756.top

string.find(s, "%d+")
来源：http://aop.shanyushiyangtech.top

[T40] Lua：元表
来源：http://mhz.c1oappe.top

setmetatable({}, { __index = base })
来源：http://yhi.yuxming.cn

[T41] Perl：Hello World
来源：http://jdc.cqqwz.cn

print "Hello\n";
来源：http://sxh.redwolf501.top

[T42] Perl：变量类型
来源：http://tes.cqqwz.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vbf.ivvv.top

[T43] Perl：字符串插值
来源：http://ljw.jqgfzy.top

"值: $a"
来源：http://wci.fzhhl.top

[T44] Perl：条件
来源：http://tgt.xuanzx.com

if ($a > 0) { print "正"; }
来源：http://jha.jyoumei.cn

[T45] Perl：数组遍历
来源：http://tgz.ehwqpu.com

for my $x (@arr) { print $x; }
来源：http://yjr.fengsongda.top

[T46] Perl：哈希操作
来源：http://fhh.nanxuanxn.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wco.ppjwa.cn

[T47] Perl：正则捕获
来源：http://oop.yonumen.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://zol.smart0.xyz

[T48] Perl：正则替换
来源：http://eeg.hongshengwenyu.top

$s =~ s/old/new/g;
来源：http://lxk.zdqjudy.top

[T49] Perl：函数
来源：http://vlz.hywenlv.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://iec.sjlbkw.cn

[T50] Perl：逐行读文件
来源：http://vvu.jqgufenzy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://jeb.vehdjk.com

while (my $line = <$fh>) { print $line; }
来源：http://mum.zhijiandao.cn

[T51] Scala：Hello World
来源：http://kps.tarul.cn

println("Hello")
来源：http://zow.jinghuilouyu.cn

[T52] Scala：变量
来源：http://tyo.jlsjyb.cn

val a = 1;  var b = 2
来源：http://shs.nanxuanxn.top

[T53] Scala：字符串插值
来源：http://hfc.hfpthk.cn

s"值: $b"
来源：http://wva.jiagoushi.top

[T54] Scala：集合映射
来源：http://vdn.wangdashe.top

List(1, 2, 3).map(_ * 2)
来源：http://czo.pycfn.com

[T55] Scala：集合过滤
来源：http://vvd.pengpengdd.cyou

List(1, 2, 3).filter(_ > 1)
来源：http://rcz.shanyushiyangtech.top

[T56] Scala：样例类
来源：http://imd.svipenyu.cn

case class User(name: String, age: Int)
来源：http://oyi.ctjpmb.com

[T57] Scala：模式匹配
来源：http://pya.9152youxi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://pvt.zhengqikj.top

[T58] Scala：函数定义
来源：http://hzg.gotoacloud.top

def add(a: Int, b: Int): Int = a + b
来源：http://uyh.sufxvd.cn

[T59] Scala：循环
来源：http://fdo.tanke756.top

for (i <- 1 to 10) println(i)
来源：http://dpl.redwolf501.top

[T60] Scala：折叠
来源：http://igh.yuanzhike.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://eea.yj20258.top

================================================================================
来源：http://sui.haohaochexian.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://rqs.cashguo.top

================================================================================
来源：http://cnv.hnxiangtu.top

[U01] Py：创建虚拟环境
来源：http://qhh.sjlbkw.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ehq.jqgfzy.top

[U02] Py：导出 / 安装依赖
来源：http://njv.c1oappe.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ewo.aizwys.cn

[U03] Py：加载 .env 配置
来源：http://kpt.fengsongda.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ckr.kuanghao11.cn

[U04] Py：变量调试打印
来源：http://uzm.yj202588.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://isc.redwolf501.top

[U05] Py：列表去重且保序
来源：http://pcc.hnqzz.top

list(dict.fromkeys(arr))
来源：http://xda.hongshengwenyu.top

[U06] Py：合并两个字典
来源：http://rhr.jiagoushi.top

{**a, **b}
来源：http://vsw.zdqjudy.top

[U07] Py：反转字典键值
来源：http://psr.yuxming.cn

{v: k for k, v in d.items()}
来源：http://uhm.yonumen.top

[U08] Py：展平二维列表
来源：http://gjp.zhixingplan.top

[y for x in nested for y in x]
来源：http://khp.zhongyouzk.top

[U09] Py：字典取最大值的键
来源：http://kgz.birdmap.top

max(d, key=d.get)
来源：http://arw.gotoacloud.top

[U10] Py：按值排序字典
来源：http://zpg.feifeiyinyue.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hzg.snrcjt.cn

[U11] Py：生成器表达式
来源：http://svl.ywan-chungtsiang.top

(x * 2 for x in arr)
来源：http://yxe.shangyingyoupin.top

[U12] Py：取出现最多的 3 个元素
来源：http://zjk.nanxinkj.top

Counter(arr).most_common(3)
来源：http://whp.aibaodan.cn

[U13] Py：固定长度队列
来源：http://jpp.vehdjk.com

deque(maxlen=10)
来源：http://obr.jqgfzy.top

[U14] Py：分组收集到列表
来源：http://tnm.bbcook.cn

defaultdict(list)
来源：http://gty.ywan-chungtsiang.top

[U15] Py：高精度计时
来源：http://fjc.gzhubu.top

t = time.perf_counter()
来源：http://ouv.epnwcf.com

[U16] Py：命令行参数解析
来源：http://nik.xylfe.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yyn.havefunace.top

[U17] Py：初始化日志
来源：http://ewm.hfpthk.cn

logging.basicConfig(level=logging.INFO)
来源：http://bfe.shanyushiyangtech.top

[U18] Py：预编译正则
来源：http://oti.guowangkeji.top

pat = re.compile(r"\d+")
来源：http://aqe.wangdashe.top

[U19] Py：正则替换带回调
来源：http://bnq.redwolf501.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://epy.ywan-chungtsiang.top

[U20] Py：缓存函数结果
来源：http://pqt.zhixingplan.top

@functools.lru_cache(maxsize=None)
来源：http://fzr.316326.xyz

[U21] Py：自定义上下文管理器
来源：http://xny.tarul.cn

@contextlib.contextmanager
来源：http://cdr.shuidangran.top

[U22] Py：矩阵转置
来源：http://gdz.zhiwuduotai.top

list(zip(*m))
来源：http://vpb.hammf.cn

[U23] Py：分块读取大文件
来源：http://vam.bjfxy.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lgh.yueranfly.top

[U24] Py：路径操作
来源：http://mfq.yfazqb.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://jxc.nanxuanxn.top

[U25] Py：CSV 按字典读
来源：http://xxf.hongshengwenyu.top

csv.DictReader(f)
来源：http://oet.sufxvd.cn

[U26] Py：并发下载
来源：http://fly.sjlbkw.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qfm.mhx1999.top

[U27] Py：异步 HTTP
来源：http://yfe.birdmap.top

aiohttp.ClientSession() 配合 async with
来源：http://ffx.svipenyu.cn

[U28] Py：类型别名
来源：http://bwr.zycfv.cn

UserId = int
来源：http://gtb.jianghu66.top

[U29] Py：属性校验
来源：http://aza.aibaodan.cn

@property 与 @x.setter 配合
来源：http://reg.wangdashe.top

[U30] Py：数据类
来源：http://ulx.hongshengwenyu.top

@dataclass(slots=True)
来源：http://uqx.zhixingplan.top


<!-- 参考信息 -->