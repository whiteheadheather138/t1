代发 wailian999

int x; scanf("%d", &x);
来源：http://xlz.yuxming.cn

[S04] C：字符串复制
来源：http://kvl.jyoumei.cn

char dst[32]; strcpy(dst, "hi");
来源：http://kkf.yuxming.cn

[S05] C：字符串长度
来源：http://uxx.aizwys.cn

strlen(s)
来源：http://hvi.smart0.xyz

[S06] C：字符串比较
来源：http://jdt.fanxiaobao.xyz

strcmp(a, b) == 0
来源：http://cuw.zycfv.cn

[S07] C：数组遍历求和
来源：http://vfr.cheryme.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uat.nanxuanxn.top

[S08] C：动态内存分配与释放
来源：http://uyw.jianghu66.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tpb.ehwqpu.com

[S09] C：结构体定义与初始化
来源：http://tqj.dashuyun.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ala.jinqigfzy.top

[S10] C：指针与解引用
来源：http://bij.zhaomingkeji.xyz

int *p = &a;  *p = 5;
来源：http://lkl.jiagoushi.top

[S11] C：逐行读文件
来源：http://vve.guannengcc.top

FILE *f = fopen("a.txt", "r");
来源：http://quk.ywan-chungtsiang.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://opp.aibaodan.cn

fclose(f);
来源：http://bcq.tarul.cn

[S12] C：写文件
来源：http://yun.zdbjq.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vvk.chenjidiqi.icu

[S13] C：宏定义
来源：http://xdi.zhengqikj.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rkr.xingfuxueyuan.xyz

[S14] C：枚举
来源：http://slc.bbcook.cn

enum Color { RED, GREEN, BLUE };
来源：http://vtr.uphjek.com

[S15] C：类型转换
来源：http://uaa.hcnkem.com

(double) a / b
来源：http://fim.xuanzx.com

[S16] C：位操作置位
来源：http://hor.guannengcc.top

x |= (1 << 3);
来源：http://wkf.jlsjyb.cn

[S17] C：安全拼接字符串
来源：http://pve.hnxiangtu.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cja.ctjpmb.com

[S18] C：命令行参数
来源：http://jzw.jinqigufen.top

int main(int argc, char **argv)
来源：http://aft.316326.xyz

[S19] C：快速排序
来源：http://kst.sjlbkw.cn

qsort(a, n, sizeof(int), cmp);
来源：http://yrc.iojbl.cn

[S20] C：二分查找
来源：http://koq.52xcode.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lyk.ydzc1.top

[S21] C：字符类别判断
来源：http://fmy.daxiang520.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lwr.fehbvm.com

[S22] C：字符串转数字
来源：http://qoj.dianchejie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xaj.jlsjyb.cn

[S23] C：随机数
来源：http://vrc.hesvh.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xqt.yj20258888.top

[S24] C：获取本地时间
来源：http://lny.chenlongwang.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dap.daxiang520.top

[S25] C：内存拷贝
来源：http://dru.smart0.xyz

memcpy(dst, src, n);
来源：http://zuh.fengsongda.top

[S26] C：内存清零
来源：http://ntn.xingfuxueyuan.xyz

memset(a, 0, sizeof a);
来源：http://kzm.sufxvd.cn

[S27] C：定义常量
来源：http://fte.mhx1999.top

const double PI = 3.14159;
来源：http://ndn.iojbl.cn

[S28] C：静态变量
来源：http://gqz.bjfxy.top

static int counter = 0;
来源：http://bsd.xylfe.cn

[S29] C：变参函数
来源：http://rue.chenlongwang.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uqq.haohaochexian.top

[S30] C：头文件保护
来源：http://van.daria6918.cn

#ifndef X_H
来源：http://tmk.jinyuanbaomall.cn

#define X_H
来源：http://lgy.nanxuanxn.top

#endif
来源：http://qbi.bbcook.cn

[S31] C++：Hello World
来源：http://itm.snrcjt.cn

#include <iostream>
来源：http://rhl.andypj.xyz

int main() { std::cout << "Hello\n"; }
来源：http://boa.yj20258888.top

[S32] C++：字符串
来源：http://ixi.sweek.top

std::string s = "hi";  s += "!";
来源：http://uvi.cucudq.cn

[S33] C++：vector 增删
来源：http://roa.yangfankeji.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mpk.birdmap.top

[S34] C++：遍历 vector
来源：http://wwe.cashguo.top

for (auto &x : v) { std::cout << x; }
来源：http://otd.cucudq.cn

[S35] C++：map
来源：http://sgt.tian-w.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hnj.zhengqikj.top

[S36] C++：unordered_map
来源：http://ldb.tianlin.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fkl.sjlbkw.cn

[S37] C++：set
来源：http://bci.jlsjyb.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://csx.haohaochexian.top

[S38] C++：排序
来源：http://djq.ivvv.top

std::sort(v.begin(), v.end());
来源：http://dhx.shangyingyoupin.top

[S39] C++：自定义比较器排序
来源：http://iba.nwbrower.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xhl.gaohongyu789.top

[S40] C++：查找元素
来源：http://sdg.yueranfly.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qbs.jqgfzy.top

[S41] C++：类与构造函数
来源：http://abr.shanyushiyangkeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yvz.sweek.top

[S42] C++：继承与虚函数
来源：http://zav.aizwys.cn

class B : public Base { public: void f() override {} };
来源：http://xud.ppjwa.cn

[S43] C++：智能指针
来源：http://jff.ydjk.org.cn

auto p = std::make_unique<int>(5);
来源：http://elk.xinyue.icu

[S44] C++：引用传参
来源：http://hdy.316326.xyz

void inc(int &x) { ++x; }
来源：http://ygo.zhongyouzk.top

[S45] C++：lambda
来源：http://iqv.jiagoushi.top

auto add = [](int a, int b) { return a + b; };
来源：http://aqi.xuetiantiany.cn

[S46] C++：函数模板
来源：http://mro.jlsjyb.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gzf.hywenlv.cn

[S47] C++：结构化绑定遍历
来源：http://ngx.jinghuilouyu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yii.guowangkeji.top

[S48] C++：逐行读文件
来源：http://xpb.zhiwuduotai.top

std::ifstream in("a.txt");  std::string line;
来源：http://nco.yfazqb.com

while (std::getline(in, line)) { }
来源：http://pfk.ppjwa.cn

[S49] C++：写文件
来源：http://ajd.yonumen.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hpz.zhengqikj.top

[S50] C++：格式化数字
来源：http://uay.yvedp.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qbs.c1oappe.top

[S51] C++：显式类型转换
来源：http://irk.cucudq.cn

static_cast<double>(a) / b
来源：http://bsq.guowangkeji.top

[S52] C++：const 与 noexcept
来源：http://gfs.hnqzz.top

int size() const noexcept { return n_; }
来源：http://owr.jqgfzy.top

[S53] C++：移动语义
来源：http://jer.mhx1999.top

std::vector<int> w = std::move(v);
来源：http://emj.gogol.net.cn

[S54] C++：异常处理
来源：http://gcu.nanxuanxn.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tiz.jianghu66.top

[S55] C++：结构化绑定
来源：http://wpp.feifeiyinyue.top

auto [a, b] = std::make_pair(1, 2);
来源：http://zsm.dashuyun.cn

[S56] C++：optional
来源：http://kff.pengpengdd.cyou

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ckr.quarkkingdee.top

[S57] C++：编译期常量
来源：http://rik.chenjidiqi.icu

constexpr int N = 10;
来源：http://pha.52xcode.cn

[S58] C++：命名空间
来源：http://vps.yj20258888.top

namespace ns { int f() { return 1; } }
来源：http://lia.vqdsnc.cn

[S59] C++：静态断言
来源：http://fcg.fzhhl.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kri.zhixingplan.top

[S60] C++：遍历并删除元素
来源：http://xcz.fengsongda.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vhe.hcnkem.com

================================================================================
来源：http://meb.ivvv.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yah.xinyue.icu

================================================================================
来源：http://jbh.jiagoushi.top

[T01] Kotlin：Hello World
来源：http://ybl.xylfe.cn

println("Hello")
来源：http://qtc.chenjidiqi.icu

[T02] Kotlin：变量
来源：http://wdt.zhoulong.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cyq.jqgufenzy.top

[T03] Kotlin：字符串模板
来源：http://lzp.hywenlv.cn

"值: $b"
来源：http://nkn.sufxvd.cn

[T04] Kotlin：空安全
来源：http://xac.andypj.xyz

val n: String? = null;  n?.length
来源：http://kry.sjlbkw.cn

[T05] Kotlin：when 表达式
来源：http://hfh.meibo888.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tgz.meibo888.top

[T06] Kotlin：集合映射
来源：http://fqs.bjfxy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ycj.pengpengdd.cyou

[T07] Kotlin：集合过滤
来源：http://tgu.gaohongyu789.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://thb.vqdsnc.cn

[T08] Kotlin：数据类
来源：http://lxk.jqgfzy.top

data class User(val name: String, val age: Int)
来源：http://xgy.sxryk.cn

[T09] Kotlin：扩展函数
来源：http://kpp.hongshengwenyu.top

fun String.exclaim() = this + "!"
来源：http://bim.dianchejie.cn

[T10] Kotlin：默认参数
来源：http://hxe.yueranfly.top

fun greet(name: String = "World") = "Hi $name"
来源：http://upc.fzhhl.top

[T11] Kotlin：协程
来源：http://unf.bbcook.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://pvv.dianchejie.cn

[T12] Kotlin：解构声明
来源：http://ywe.pycfn.com

val (a, b) = Pair(1, 2)
来源：http://awr.meibo888.top

[T13] Kotlin：只读 Map
来源：http://has.zhiwuduotai.top

val m = mapOf("a" to 1)
来源：http://zrp.havefunace.top

[T14] Kotlin：循环
来源：http://hrt.yongpay.top

for (i in 1..10) println(i)
来源：http://owt.sjlbkw.cn

[T15] Kotlin：接口
来源：http://kln.zhaomingkeji.xyz

interface Shape { fun area(): Double }
来源：http://kjs.wangshuangyany.cn

[T16] Swift：Hello World
来源：http://kho.jianghu66.top

print("Hello")
来源：http://jwn.sysykeji.top

[T17] Swift：变量与常量
来源：http://fsk.jianghu66.top

var a = 1;  let b = 2
来源：http://rld.cucudq.cn

[T18] Swift：字符串插值
来源：http://wlz.ydzc1.top

"值: \(b)"
来源：http://wyp.nanxinkj.top

[T19] Swift：可选绑定
来源：http://krz.sufxvd.cn

if let n = opt { print(n) }
来源：http://vjo.chenjidiqi.icu

[T20] Swift：数组操作
来源：http://quh.sjlbkw.cn

var a = [1, 2, 3];  a.append(4)
来源：http://tyz.fanxiaobao.xyz

[T21] Swift：遍历
来源：http://tyu.ivvv.top

for x in a { print(x) }
来源：http://mgi.jlsjyb.cn

[T22] Swift：字典
来源：http://fug.guowangkeji.top

var d = ["a": 1];  d["b"] = 2
来源：http://nwa.zdqjudy.top

[T23] Swift：函数
来源：http://dqc.shanyushiyangkeji.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ddi.316326.xyz

[T24] Swift：闭包
来源：http://hnb.ybcxt.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://iel.xuetiantiany.cn

[T25] Swift：结构体
来源：http://oog.dashuyun.cn

struct P { var x: Int }
来源：http://psc.birdmap.top

[T26] Swift：类与重写
来源：http://ily.fengsongda.top

class A: Base { override func f() {} }
来源：http://qpm.gzhubu.top

[T27] Swift：错误处理
来源：http://rha.fehbvm.com

do { try f() } catch { print(error) }
来源：http://cuj.hnxiangtu.top

[T28] Swift：枚举
来源：http://ylz.shangyingyoupin.top

enum Color { case red, green }
来源：http://fge.ydjk.org.cn

[T29] Swift：guard 提前返回
来源：http://sxz.vehdjk.com

guard let x = opt else { return }
来源：http://css.0kj1m.cn

[T30] Swift：协议
来源：http://ftw.gotoacloud.top

protocol Shape { func area() -> Double }
来源：http://ccq.zhengqikj.top

[T31] Lua：Hello World
来源：http://cjb.shuidangran.top

print("Hello")
来源：http://rxv.vqdsnc.cn

[T32] Lua：局部变量
来源：http://oxw.ydzc1.top

local a = 1
来源：http://aqu.yfazqb.com

[T33] Lua：表（数组）
来源：http://xgp.uphjek.com

local t = {1, 2, 3};  t[4] = 4
来源：http://zkg.zhongyouzk.top

[T34] Lua：遍历表
来源：http://lki.birdmap.top

for i, v in ipairs(t) do print(i, v) end
来源：http://nvn.xuetiantiany.cn

[T35] Lua：字典表
来源：http://ehb.daria6918.cn

local d = { a = 1 };  d.b = 2
来源：http://mzs.ybcxt.top

[T36] Lua：函数
来源：http://geq.chenlongwang.top

function add(a, b) return a + b end
来源：http://fef.yvedp.cn

[T37] Lua：字符串拼接
来源：http://yds.hnqzz.top

"a" .. "b"
来源：http://zhc.yj202588.top

[T38] Lua：条件
来源：http://xiu.xziqi.cn

if x > 0 then print("正") end
来源：http://hnv.hammf.cn

[T39] Lua：模式匹配
来源：http://ymy.vehdjk.com

string.find(s, "%d+")
来源：http://muc.ywan-chungtsiang.top

[T40] Lua：元表
来源：http://rsn.havefunace.top

setmetatable({}, { __index = base })
来源：http://qva.shuidangran.top

[T41] Perl：Hello World
来源：http://rpg.birdmap.top

print "Hello\n";
来源：http://fdt.sweek.top

[T42] Perl：变量类型
来源：http://ioz.zhaomingkeji.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xif.shanyushiyangtech.top

[T43] Perl：字符串插值
来源：http://waj.yfazqb.com

"值: $a"
来源：http://gkp.fanxiaobao.xyz

[T44] Perl：条件
来源：http://nix.kuanghao11.cn

if ($a > 0) { print "正"; }
来源：http://zfb.zdbjq.cn

[T45] Perl：数组遍历
来源：http://rht.yj20258888.top

for my $x (@arr) { print $x; }
来源：http://kzf.shanyushiyangkeji.top

[T46] Perl：哈希操作
来源：http://sxz.bbcook.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cmp.zhongyouzk.top

[T47] Perl：正则捕获
来源：http://yvp.ybcxt.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://qbd.chenzaomai.com

[T48] Perl：正则替换
来源：http://cdp.chenjidiqi.icu

$s =~ s/old/new/g;
来源：http://ssc.wangshuangyany.cn

[T49] Perl：函数
来源：http://pjh.shangyingyoupin.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ngf.yvedp.cn

[T50] Perl：逐行读文件
来源：http://svp.zhixingplan.top

open my $fh, "<", "a.txt" or die $!;
来源：http://mpi.epnwcf.com

while (my $line = <$fh>) { print $line; }
来源：http://vhr.xuetiantiany.cn

[T51] Scala：Hello World
来源：http://fye.c1oappe.top

println("Hello")
来源：http://kjg.yonumen.top

[T52] Scala：变量
来源：http://pox.yuxming.cn

val a = 1;  var b = 2
来源：http://eyf.0kj1m.cn

[T53] Scala：字符串插值
来源：http://geh.guowangkeji.top

s"值: $b"
来源：http://mkr.chenjidiqi.icu

[T54] Scala：集合映射
来源：http://hvh.zhixingplan.top

List(1, 2, 3).map(_ * 2)
来源：http://pju.wangshuangyany.cn

[T55] Scala：集合过滤
来源：http://xvo.wangshuangyany.cn

List(1, 2, 3).filter(_ > 1)
来源：http://bur.shanyushiyangkeji.top

[T56] Scala：样例类
来源：http://lcn.mhx1999.top

case class User(name: String, age: Int)
来源：http://uvs.hywenlv.cn

[T57] Scala：模式匹配
来源：http://ckt.ehwqpu.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://fan.aizwys.cn

[T58] Scala：函数定义
来源：http://tpw.chenjidiqi.icu

def add(a: Int, b: Int): Int = a + b
来源：http://vxs.hesvh.cn

[T59] Scala：循环
来源：http://klh.wangdashe.top

for (i <- 1 to 10) println(i)
来源：http://fsv.jqgufenzy.top

[T60] Scala：折叠
来源：http://pel.wangdashe.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gel.hfpthk.cn

================================================================================
来源：http://abb.shanyushiyangkeji.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kgv.dianchejie.cn

================================================================================
来源：http://nwp.chenlongwang.top

[U01] Py：创建虚拟环境
来源：http://gxn.yongpay.top

python -m venv .venv && source .venv/bin/activate
来源：http://kaq.jinyuanbaomall.cn

[U02] Py：导出 / 安装依赖
来源：http://dhx.316326.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vvf.gogol.net.cn

[U03] Py：加载 .env 配置
来源：http://knm.chenjidiqi.icu

from dotenv import load_dotenv; load_dotenv()
来源：http://ptq.yueranfly.top

[U04] Py：变量调试打印
来源：http://nmf.jyoumei.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qrl.cqqwz.cn

[U05] Py：列表去重且保序
来源：http://bkx.zdqjudy.top

list(dict.fromkeys(arr))
来源：http://quq.yongpay.top

[U06] Py：合并两个字典
来源：http://wbp.yanxiufei.cn

{**a, **b}
来源：http://ppy.xylfe.cn

[U07] Py：反转字典键值
来源：http://yqn.zhixingplan.top

{v: k for k, v in d.items()}
来源：http://tbj.chenlongwang.top

[U08] Py：展平二维列表
来源：http://npx.fktsv.cn

[y for x in nested for y in x]
来源：http://hwu.sjlbkw.cn

[U09] Py：字典取最大值的键
来源：http://ivt.chenzaomai.com

max(d, key=d.get)
来源：http://far.shzxlz.cn

[U10] Py：按值排序字典
来源：http://ulq.hywenlv.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://swf.jlsjyb.cn

[U11] Py：生成器表达式
来源：http://ibj.nanxuanxn.top

(x * 2 for x in arr)
来源：http://uhk.birdmap.top

[U12] Py：取出现最多的 3 个元素
来源：http://kqc.gaohongyu789.top

Counter(arr).most_common(3)
来源：http://mtr.yuxming.cn

[U13] Py：固定长度队列
来源：http://hwg.yvedp.cn

deque(maxlen=10)
来源：http://rlp.dianchejie.cn

[U14] Py：分组收集到列表
来源：http://qkw.guowangkeji.top

defaultdict(list)
来源：http://niq.cashguo.top

[U15] Py：高精度计时
来源：http://hgb.yj202588.top

t = time.perf_counter()
来源：http://wjo.sxryk.cn

[U16] Py：命令行参数解析
来源：http://vtf.pengpengdd.cyou

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dzc.shanyushiyangkeji.top

[U17] Py：初始化日志
来源：http://nkn.fanxiaobao.xyz

logging.basicConfig(level=logging.INFO)
来源：http://ukc.xylfe.cn

[U18] Py：预编译正则
来源：http://hhq.gotoacloud.top

pat = re.compile(r"\d+")
来源：http://wqr.0kj1m.cn

[U19] Py：正则替换带回调
来源：http://fne.yonumen.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://emr.hammf.cn

[U20] Py：缓存函数结果
来源：http://rvo.bbcook.cn

@functools.lru_cache(maxsize=None)
来源：http://zcv.yanxiufei.cn

[U21] Py：自定义上下文管理器
来源：http://mig.chenjidiqi.icu

@contextlib.contextmanager
来源：http://pjj.fzhhl.top

[U22] Py：矩阵转置
来源：http://hbg.zycfv.cn

list(zip(*m))
来源：http://glm.haohaochexian.top

[U23] Py：分块读取大文件
来源：http://egx.hnxiangtu.top

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zcf.jianghu66.top

[U24] Py：路径操作
来源：http://ubq.yfazqb.com

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mwi.aibaodan.cn

[U25] Py：CSV 按字典读
来源：http://awn.vqdsnc.cn

csv.DictReader(f)
来源：http://arq.dashuyun.cn

[U26] Py：并发下载
来源：http://hev.gotoacloud.top

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ijb.zhongyouzk.top


<!-- 参考信息 -->