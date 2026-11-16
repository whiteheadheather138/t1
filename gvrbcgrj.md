代发 wailian999

read -rp "请输入: " ans
来源：http://uki.jianghu66.top

[R78] 交互式菜单
来源：http://vrl.wangdashe.top

select opt in a b c; do echo "$opt"; break; done
来源：http://opx.uphjek.com

[R79] 解析命令行选项
来源：http://pna.pengpengdd.cyou

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://caf.jinyuanbaomall.cn

[R80] 查看脚本执行耗时
来源：http://dfk.zdqjudy.top

time ./run.sh
来源：http://tfv.ywan-chungtsiang.top

================================================================================
来源：http://olo.zhiwuduotai.top

S. C / C++ 专题
来源：http://knb.guannengcc.top

================================================================================
来源：http://brq.snrcjt.cn

[S01] C：Hello World
来源：http://ahy.xuetiantiany.cn

#include <stdio.h>
来源：http://zvg.yfazqb.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://hbl.xuanzx.com

[S02] C：变量与格式化输出
来源：http://nil.yueranfly.top

int a = 10; printf("%d\n", a);
来源：http://zud.c1oappe.top

[S03] C：读入整数
来源：http://fjo.fzhhl.top

int x; scanf("%d", &x);
来源：http://xsp.aizwys.cn

[S04] C：字符串复制
来源：http://bmb.ydzc1.top

char dst[32]; strcpy(dst, "hi");
来源：http://kfi.sjlbkw.cn

[S05] C：字符串长度
来源：http://iad.birdmap.top

strlen(s)
来源：http://blu.zhoulong.xyz

[S06] C：字符串比较
来源：http://bzr.tanke756.top

strcmp(a, b) == 0
来源：http://ykp.c1oappe.top

[S07] C：数组遍历求和
来源：http://qfc.jiagoushi.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rss.ywan-chungtsiang.top

[S08] C：动态内存分配与释放
来源：http://mzl.daria6918.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ole.xuetiantiany.cn

[S09] C：结构体定义与初始化
来源：http://jeg.zhengqikj.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sae.jinghuilouyu.cn

[S10] C：指针与解引用
来源：http://stu.zhoulong.xyz

int *p = &a;  *p = 5;
来源：http://ynw.cheryme.top

[S11] C：逐行读文件
来源：http://uth.ctjpmb.com

FILE *f = fopen("a.txt", "r");
来源：http://mqd.yueranfly.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://sph.meibo888.top

fclose(f);
来源：http://tva.bjfxy.top

[S12] C：写文件
来源：http://avk.iojbl.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://snc.jqgufenzy.top

[S13] C：宏定义
来源：http://hwr.yonumen.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yan.kuanghao11.cn

[S14] C：枚举
来源：http://ojb.ywan-chungtsiang.top

enum Color { RED, GREEN, BLUE };
来源：http://sps.yonumen.top

[S15] C：类型转换
来源：http://ftb.cashguo.top

(double) a / b
来源：http://sot.sufxvd.cn

[S16] C：位操作置位
来源：http://ymq.aizwys.cn

x |= (1 << 3);
来源：http://baq.316326.xyz

[S17] C：安全拼接字符串
来源：http://cgd.hnxiangtu.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://edm.chenlongwang.top

[S18] C：命令行参数
来源：http://mbq.shzxlz.cn

int main(int argc, char **argv)
来源：http://fct.haohaochexian.top

[S19] C：快速排序
来源：http://rnv.gzhubu.top

qsort(a, n, sizeof(int), cmp);
来源：http://tlf.yj20258.top

[S20] C：二分查找
来源：http://hjz.wangdashe.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wwm.havefunace.top

[S21] C：字符类别判断
来源：http://yzt.shzxlz.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tyl.bbcook.cn

[S22] C：字符串转数字
来源：http://ygj.bjfxy.top

atoi("42");  strtod("3.14", NULL);
来源：http://myi.tarul.cn

[S23] C：随机数
来源：http://ytb.cheryme.top

srand(time(NULL));  int r = rand() % 100;
来源：http://agy.zhengqikj.top

[S24] C：获取本地时间
来源：http://edc.yvedp.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sgh.wangdashe.top

[S25] C：内存拷贝
来源：http://glx.feifeiyinyue.top

memcpy(dst, src, n);
来源：http://wnd.ybcxt.top

[S26] C：内存清零
来源：http://bvb.yueranfly.top

memset(a, 0, sizeof a);
来源：http://jia.gaohongyu789.top

[S27] C：定义常量
来源：http://jvt.shanyushiyangtech.top

const double PI = 3.14159;
来源：http://rwu.zycfv.cn

[S28] C：静态变量
来源：http://pim.sysykeji.top

static int counter = 0;
来源：http://kdg.yonumen.top

[S29] C：变参函数
来源：http://bhm.snrcjt.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mwq.cashguo.top

[S30] C：头文件保护
来源：http://efm.yvedp.cn

#ifndef X_H
来源：http://ckl.xinyue.icu

#define X_H
来源：http://kqq.andypj.xyz

#endif
来源：http://buh.pycfn.com

[S31] C++：Hello World
来源：http://hls.bbcook.cn

#include <iostream>
来源：http://vok.hcnkem.com

int main() { std::cout << "Hello\n"; }
来源：http://scn.zhixingplan.top

[S32] C++：字符串
来源：http://fwc.ivvv.top

std::string s = "hi";  s += "!";
来源：http://ikr.hywenlv.cn

[S33] C++：vector 增删
来源：http://myn.jlsjyb.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pvp.gaohongyu789.top

[S34] C++：遍历 vector
来源：http://krs.nanxinkj.top

for (auto &x : v) { std::cout << x; }
来源：http://stn.tarul.cn

[S35] C++：map
来源：http://jnc.fehbvm.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://emn.fehbvm.com

[S36] C++：unordered_map
来源：http://max.mhx1999.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ckh.shuidangran.top

[S37] C++：set
来源：http://opz.pengpengdd.cyou

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gbe.andypj.xyz

[S38] C++：排序
来源：http://pfh.yfazqb.com

std::sort(v.begin(), v.end());
来源：http://kob.ybcxt.top

[S39] C++：自定义比较器排序
来源：http://kxr.birdmap.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mtt.316326.xyz

[S40] C++：查找元素
来源：http://tbl.hcnkem.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hxy.hysaishi.cn

[S41] C++：类与构造函数
来源：http://pdm.jinyuanbaomall.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://uca.ybcxt.top

[S42] C++：继承与虚函数
来源：http://xxz.jqgfzy.top

class B : public Base { public: void f() override {} };
来源：http://mai.wangdashe.top

[S43] C++：智能指针
来源：http://inz.hywenlv.cn

auto p = std::make_unique<int>(5);
来源：http://cef.sweek.top

[S44] C++：引用传参
来源：http://mou.hysaishi.cn

void inc(int &x) { ++x; }
来源：http://ibq.yj202588.top

[S45] C++：lambda
来源：http://mpv.wangshuangyany.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xby.zhoulong.xyz

[S46] C++：函数模板
来源：http://oak.nwbrower.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vnk.zhongyouzk.top

[S47] C++：结构化绑定遍历
来源：http://bzf.nanxuanxn.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pcs.yj202588.top

[S48] C++：逐行读文件
来源：http://fuf.cucudq.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fsa.316326.xyz

while (std::getline(in, line)) { }
来源：http://uxy.jiagoushi.top

[S49] C++：写文件
来源：http://nea.pycfn.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mji.sufxvd.cn

[S50] C++：格式化数字
来源：http://zit.xuetiantiany.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zod.ybcxt.top

[S51] C++：显式类型转换
来源：http://flg.fehbvm.com

static_cast<double>(a) / b
来源：http://pce.sjlbkw.cn

[S52] C++：const 与 noexcept
来源：http://pee.yangfankeji.com

int size() const noexcept { return n_; }
来源：http://sci.yj20258888.top

[S53] C++：移动语义
来源：http://xwy.shanyushiyangkeji.top

std::vector<int> w = std::move(v);
来源：http://elh.uphjek.com

[S54] C++：异常处理
来源：http://kmh.gzhubu.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sye.zhijiandao.cn

[S55] C++：结构化绑定
来源：http://ggp.fzhhl.top

auto [a, b] = std::make_pair(1, 2);
来源：http://cox.pengpengdd.cyou

[S56] C++：optional
来源：http://oal.iojbl.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qif.cdnleiting.top

[S57] C++：编译期常量
来源：http://qpt.zhiwuduotai.top

constexpr int N = 10;
来源：http://bpi.smart0.xyz

[S58] C++：命名空间
来源：http://qhh.jiagoushi.top

namespace ns { int f() { return 1; } }
来源：http://ylj.jinqigufen.top

[S59] C++：静态断言
来源：http://ndm.smart0.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rql.snrcjt.cn

[S60] C++：遍历并删除元素
来源：http://mds.zdqjudy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://siu.aizwys.cn

================================================================================
来源：http://rqf.ydjk.org.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fcw.zhoulong.xyz

================================================================================
来源：http://hjs.chenjidiqi.icu

[T01] Kotlin：Hello World
来源：http://mnw.fzhhl.top

println("Hello")
来源：http://hxj.shanyushiyangtech.top

[T02] Kotlin：变量
来源：http://mlx.ybcxt.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://iwf.feifeiyinyue.top

[T03] Kotlin：字符串模板
来源：http://bhl.aizwys.cn

"值: $b"
来源：http://nzj.andypj.xyz

[T04] Kotlin：空安全
来源：http://mro.feifeiyinyue.top

val n: String? = null;  n?.length
来源：http://qkt.yuanzhike.top

[T05] Kotlin：when 表达式
来源：http://nop.mhx1999.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tsg.sjlbkw.cn

[T06] Kotlin：集合映射
来源：http://fvi.cashguo.top

listOf(1, 2, 3).map { it * 2 }
来源：http://wdh.jqgfzy.top

[T07] Kotlin：集合过滤
来源：http://xun.yj202588.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://gag.xinyue.icu

[T08] Kotlin：数据类
来源：http://cxy.dashuyun.cn

data class User(val name: String, val age: Int)
来源：http://wvj.xylfe.cn

[T09] Kotlin：扩展函数
来源：http://die.0kj1m.cn

fun String.exclaim() = this + "!"
来源：http://slj.smart0.xyz

[T10] Kotlin：默认参数
来源：http://vbv.daxiang520.top

fun greet(name: String = "World") = "Hi $name"
来源：http://bqg.sysykeji.top

[T11] Kotlin：协程
来源：http://ceb.ehwqpu.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://vrw.yuanzhike.top

[T12] Kotlin：解构声明
来源：http://tuc.zhoulong.xyz

val (a, b) = Pair(1, 2)
来源：http://sfe.xziqi.cn

[T13] Kotlin：只读 Map
来源：http://lyv.mhx1999.top

val m = mapOf("a" to 1)
来源：http://dhy.uphjek.com

[T14] Kotlin：循环
来源：http://yqb.fanxiaobao.xyz

for (i in 1..10) println(i)
来源：http://vbl.hammf.cn

[T15] Kotlin：接口
来源：http://bnc.epnwcf.com

interface Shape { fun area(): Double }
来源：http://nxb.xingfuxueyuan.xyz

[T16] Swift：Hello World
来源：http://sqz.iojbl.cn

print("Hello")
来源：http://pdl.haohaochexian.top

[T17] Swift：变量与常量
来源：http://ied.chenjidiqi.icu

var a = 1;  let b = 2
来源：http://bqn.smart0.xyz

[T18] Swift：字符串插值
来源：http://ujl.pengpengdd.cyou

"值: \(b)"
来源：http://joz.jinghuilouyu.cn

[T19] Swift：可选绑定
来源：http://gsh.feifeiyinyue.top

if let n = opt { print(n) }
来源：http://tms.52xcode.cn

[T20] Swift：数组操作
来源：http://kqu.gotoacloud.top

var a = [1, 2, 3];  a.append(4)
来源：http://fgt.aizwys.cn

[T21] Swift：遍历
来源：http://hid.yuxming.cn

for x in a { print(x) }
来源：http://apk.xinyue.icu

[T22] Swift：字典
来源：http://agc.shangyingyoupin.top

var d = ["a": 1];  d["b"] = 2
来源：http://vkl.redwolf501.top

[T23] Swift：函数
来源：http://blj.zdbjq.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jui.snrcjt.cn

[T24] Swift：闭包
来源：http://wes.hongshengwenyu.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://rgw.zhixingplan.top

[T25] Swift：结构体
来源：http://ned.ehwqpu.com

struct P { var x: Int }
来源：http://jcn.zhengqikj.top

[T26] Swift：类与重写
来源：http://hsa.yfazqb.com

class A: Base { override func f() {} }
来源：http://mfe.cheryme.top

[T27] Swift：错误处理
来源：http://dme.tian-w.cn

do { try f() } catch { print(error) }
来源：http://zuy.guowangkeji.top

[T28] Swift：枚举
来源：http://aol.sweek.top

enum Color { case red, green }
来源：http://yyi.c1oappe.top

[T29] Swift：guard 提前返回
来源：http://kkx.pycfn.com

guard let x = opt else { return }
来源：http://rhh.wangshuangyany.cn

[T30] Swift：协议
来源：http://miv.fanxiaobao.xyz

protocol Shape { func area() -> Double }
来源：http://oxx.yangfankeji.com

[T31] Lua：Hello World
来源：http://blb.tarul.cn

print("Hello")
来源：http://bqv.jinqigfzy.top

[T32] Lua：局部变量
来源：http://uvd.aibaodan.cn

local a = 1
来源：http://gfd.redwolf501.top

[T33] Lua：表（数组）
来源：http://ljk.kuanghao11.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://sva.zhiwuduotai.top

[T34] Lua：遍历表
来源：http://nmp.hfpthk.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://lnl.chenzaomai.com

[T35] Lua：字典表
来源：http://iwc.vqdsnc.cn

local d = { a = 1 };  d.b = 2
来源：http://gty.jinqigfzy.top

[T36] Lua：函数
来源：http://aib.jinqigfzy.top

function add(a, b) return a + b end
来源：http://ejn.yongpay.top

[T37] Lua：字符串拼接
来源：http://fon.zhengqikj.top

"a" .. "b"
来源：http://lrp.fktsv.cn

[T38] Lua：条件
来源：http://bsk.zdbjq.cn

if x > 0 then print("正") end
来源：http://kxr.xuetiantiany.cn

[T39] Lua：模式匹配
来源：http://vfs.cheryme.top

string.find(s, "%d+")
来源：http://ajy.jianghu66.top

[T40] Lua：元表
来源：http://lyd.cashguo.top

setmetatable({}, { __index = base })
来源：http://qur.shangyingyoupin.top

[T41] Perl：Hello World
来源：http://phb.ehwqpu.com

print "Hello\n";
来源：http://tfc.shuidangran.top

[T42] Perl：变量类型
来源：http://mwp.haohaochexian.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ayb.yueranfly.top

[T43] Perl：字符串插值
来源：http://kyq.xziqi.cn

"值: $a"
来源：http://fmt.sjlbkw.cn

[T44] Perl：条件
来源：http://okf.hysaishi.cn

if ($a > 0) { print "正"; }
来源：http://udu.feifeiyinyue.top

[T45] Perl：数组遍历
来源：http://iju.0kj1m.cn

for my $x (@arr) { print $x; }
来源：http://jvg.jlsjyb.cn

[T46] Perl：哈希操作
来源：http://cfu.jinghuilouyu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://glp.andypj.xyz

[T47] Perl：正则捕获
来源：http://teb.hcnkem.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://nad.hammf.cn

[T48] Perl：正则替换
来源：http://ece.yj20258.top

$s =~ s/old/new/g;
来源：http://phr.wangshuangyany.cn

[T49] Perl：函数
来源：http://dml.iojbl.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://oft.cashguo.top

[T50] Perl：逐行读文件
来源：http://ksr.cashguo.top

open my $fh, "<", "a.txt" or die $!;
来源：http://qhz.quarkkingdee.top

while (my $line = <$fh>) { print $line; }
来源：http://bwr.fzhhl.top

[T51] Scala：Hello World
来源：http://yqf.zdqjudy.top

println("Hello")
来源：http://rix.yj20258.top

[T52] Scala：变量
来源：http://kmt.shanyushiyangkeji.top

val a = 1;  var b = 2
来源：http://zye.yangfankeji.com

[T53] Scala：字符串插值
来源：http://uxo.dianchejie.cn

s"值: $b"
来源：http://bvs.yfazqb.com

[T54] Scala：集合映射
来源：http://idw.yj202588.top

List(1, 2, 3).map(_ * 2)
来源：http://qhy.tanke756.top

[T55] Scala：集合过滤
来源：http://slv.shzxlz.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gxi.tanke756.top

[T56] Scala：样例类
来源：http://sww.cheryme.top

case class User(name: String, age: Int)
来源：http://fse.zhijiandao.cn

[T57] Scala：模式匹配
来源：http://rks.sysykeji.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://icw.zhoulong.xyz

[T58] Scala：函数定义
来源：http://ifm.shzxlz.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bqq.sweek.top

[T59] Scala：循环
来源：http://ifk.zhaomingkeji.xyz

for (i <- 1 to 10) println(i)
来源：http://rru.xziqi.cn

[T60] Scala：折叠
来源：http://yxy.jlsjyb.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wgx.xingfuxueyuan.xyz

================================================================================
来源：http://ece.ppjwa.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pkg.hesvh.cn

================================================================================
来源：http://wxi.pycfn.com

[U01] Py：创建虚拟环境
来源：http://blc.ctjpmb.com

python -m venv .venv && source .venv/bin/activate
来源：http://fqb.yongpay.top

[U02] Py：导出 / 安装依赖
来源：http://xuc.hongshengwenyu.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mfp.jinyuanbaomall.cn

[U03] Py：加载 .env 配置
来源：http://afd.zdqjudy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ucf.zhoulong.xyz

[U04] Py：变量调试打印
来源：http://kxa.sweek.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vsz.fehbvm.com

[U05] Py：列表去重且保序
来源：http://pah.jlsjyb.cn

list(dict.fromkeys(arr))
来源：http://efg.nwbrower.top

[U06] Py：合并两个字典
来源：http://xsa.hesvh.cn

{**a, **b}
来源：http://vws.sjlbkw.cn

[U07] Py：反转字典键值
来源：http://zwn.xuanzx.com

{v: k for k, v in d.items()}
来源：http://myr.kuanghao11.cn

[U08] Py：展平二维列表
来源：http://meh.ehwqpu.com

[y for x in nested for y in x]
来源：http://syn.yueranfly.top

[U09] Py：字典取最大值的键
来源：http://kam.shangyingyoupin.top

max(d, key=d.get)
来源：http://mwa.jinqigfzy.top

[U10] Py：按值排序字典
来源：http://uat.nwbrower.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mrh.andypj.xyz

[U11] Py：生成器表达式
来源：http://qsa.xylfe.cn

(x * 2 for x in arr)
来源：http://qyq.ctjpmb.com

[U12] Py：取出现最多的 3 个元素
来源：http://myr.tian-w.cn

Counter(arr).most_common(3)
来源：http://ths.sxryk.cn

[U13] Py：固定长度队列
来源：http://urb.gotoacloud.top

deque(maxlen=10)
来源：http://mcx.fzhhl.top

[U14] Py：分组收集到列表
来源：http://rry.wangdashe.top

defaultdict(list)
来源：http://sqt.fengsongda.top

[U15] Py：高精度计时
来源：http://hhx.wangdashe.top

t = time.perf_counter()
来源：http://lie.birdmap.top

[U16] Py：命令行参数解析
来源：http://tfz.xinyue.icu

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mkl.nanxuanxn.top

[U17] Py：初始化日志
来源：http://ont.feifeiyinyue.top

logging.basicConfig(level=logging.INFO)
来源：http://zyj.chenzaomai.com

[U18] Py：预编译正则
来源：http://gan.gaohongyu789.top

pat = re.compile(r"\d+")
来源：http://gaw.9152youxi.cn


<!-- 参考信息 -->