代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://lix.tarul.cn

[R72] 等待端口就绪
来源：http://vwx.uphjek.com

until nc -z localhost 3306; do sleep 1; done
来源：http://nfs.sweek.top

[R73] 分割大日志
来源：http://qbu.uphjek.com

split -l 1000 big.log part_
来源：http://rrv.yangfankeji.com

[R74] 批量重命名
来源：http://xwj.jinqigfzy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ayh.chenlongwang.top

[R75] 导出环境变量
来源：http://wxk.aibaodan.cn

export PATH="$HOME/bin:$PATH"
来源：http://gpk.tarul.cn

[R76] 使用临时文件
来源：http://qcy.wangdashe.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lmc.jqgfzy.top

[R77] 读取用户输入
来源：http://fdx.nanxinkj.top

read -rp "请输入: " ans
来源：http://uob.zdqjudy.top

[R78] 交互式菜单
来源：http://utn.redwolf501.top

select opt in a b c; do echo "$opt"; break; done
来源：http://efd.havefunace.top

[R79] 解析命令行选项
来源：http://ers.fanxiaobao.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ojx.shanyushiyangtech.top

[R80] 查看脚本执行耗时
来源：http://rlw.epnwcf.com

time ./run.sh
来源：http://vge.wangdashe.top

================================================================================
来源：http://zjc.yuxming.cn

S. C / C++ 专题
来源：http://wug.fzhhl.top

================================================================================
来源：http://qnt.yuanzhike.top

[S01] C：Hello World
来源：http://fiv.fengsongda.top

#include <stdio.h>
来源：http://opj.yangfankeji.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://qei.yuanzhike.top

[S02] C：变量与格式化输出
来源：http://ksc.sxryk.cn

int a = 10; printf("%d\n", a);
来源：http://rcs.hesvh.cn

[S03] C：读入整数
来源：http://dws.redwolf501.top

int x; scanf("%d", &x);
来源：http://rbc.ydjk.org.cn

[S04] C：字符串复制
来源：http://ykt.hesvh.cn

char dst[32]; strcpy(dst, "hi");
来源：http://cbf.52xcode.cn

[S05] C：字符串长度
来源：http://ckp.sxryk.cn

strlen(s)
来源：http://rym.daria6918.cn

[S06] C：字符串比较
来源：http://dma.xuanzx.com

strcmp(a, b) == 0
来源：http://hsz.jinyuanbaomall.cn

[S07] C：数组遍历求和
来源：http://dhl.birdmap.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xul.shangyingyoupin.top

[S08] C：动态内存分配与释放
来源：http://mji.tarul.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ehr.yj20258888.top

[S09] C：结构体定义与初始化
来源：http://tyq.xuetiantiany.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mrc.yonumen.top

[S10] C：指针与解引用
来源：http://rtb.feifeiyinyue.top

int *p = &a;  *p = 5;
来源：http://cqe.jiagoushi.top

[S11] C：逐行读文件
来源：http://amx.xziqi.cn

FILE *f = fopen("a.txt", "r");
来源：http://don.pengpengdd.cyou

while (fgets(buf, sizeof buf, f)) { }
来源：http://yoo.smart0.xyz

fclose(f);
来源：http://rez.zhoulong.xyz

[S12] C：写文件
来源：http://nno.jinqigfzy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fwn.gogol.net.cn

[S13] C：宏定义
来源：http://djn.hammf.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mpt.pengpengdd.cyou

[S14] C：枚举
来源：http://cqm.jinqigufen.top

enum Color { RED, GREEN, BLUE };
来源：http://ggy.shanyushiyangtech.top

[S15] C：类型转换
来源：http://vmh.yj20258888.top

(double) a / b
来源：http://pya.cdnleiting.top

[S16] C：位操作置位
来源：http://mnj.chenlongwang.top

x |= (1 << 3);
来源：http://tow.jqgufenzy.top

[S17] C：安全拼接字符串
来源：http://cid.pycfn.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zhh.yuxming.cn

[S18] C：命令行参数
来源：http://wtg.shangyingyoupin.top

int main(int argc, char **argv)
来源：http://tko.yj20258888.top

[S19] C：快速排序
来源：http://syd.yuanzhike.top

qsort(a, n, sizeof(int), cmp);
来源：http://hro.pengpengdd.cyou

[S20] C：二分查找
来源：http://wno.gotoacloud.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://doa.hesvh.cn

[S21] C：字符类别判断
来源：http://bmj.cheryme.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ldc.aibaodan.cn

[S22] C：字符串转数字
来源：http://haz.yj20258.top

atoi("42");  strtod("3.14", NULL);
来源：http://cny.zhijiandao.cn

[S23] C：随机数
来源：http://lzn.uphjek.com

srand(time(NULL));  int r = rand() % 100;
来源：http://nbd.yongpay.top

[S24] C：获取本地时间
来源：http://ugf.ydzc1.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hke.haohaochexian.top

[S25] C：内存拷贝
来源：http://yin.cucudq.cn

memcpy(dst, src, n);
来源：http://kzn.chenlongwang.top

[S26] C：内存清零
来源：http://bim.jlsjyb.cn

memset(a, 0, sizeof a);
来源：http://dvx.ehwqpu.com

[S27] C：定义常量
来源：http://jyf.hcnkem.com

const double PI = 3.14159;
来源：http://owp.ctjpmb.com

[S28] C：静态变量
来源：http://rvw.redwolf501.top

static int counter = 0;
来源：http://xki.quarkkingdee.top

[S29] C：变参函数
来源：http://nsx.sxryk.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pwl.316326.xyz

[S30] C：头文件保护
来源：http://wrj.chenzaomai.com

#ifndef X_H
来源：http://kqn.epnwcf.com

#define X_H
来源：http://anm.haohaochexian.top

#endif
来源：http://ehu.sufxvd.cn

[S31] C++：Hello World
来源：http://img.chenzaomai.com

#include <iostream>
来源：http://ptf.nanxinkj.top

int main() { std::cout << "Hello\n"; }
来源：http://dxk.jyoumei.cn

[S32] C++：字符串
来源：http://gmf.feifeiyinyue.top

std::string s = "hi";  s += "!";
来源：http://wri.pengpengdd.cyou

[S33] C++：vector 增删
来源：http://jpc.daxiang520.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rlb.hysaishi.cn

[S34] C++：遍历 vector
来源：http://fgn.zhixingplan.top

for (auto &x : v) { std::cout << x; }
来源：http://wrv.tianlin.xyz

[S35] C++：map
来源：http://acs.zycfv.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rlo.dianchejie.cn

[S36] C++：unordered_map
来源：http://uzj.zhoulong.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hrj.ivvv.top

[S37] C++：set
来源：http://tnr.yangfankeji.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mlt.ydjk.org.cn

[S38] C++：排序
来源：http://kkp.jinghuilouyu.cn

std::sort(v.begin(), v.end());
来源：http://ubh.ywan-chungtsiang.top

[S39] C++：自定义比较器排序
来源：http://jzi.shanyushiyangkeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bqb.fzhhl.top

[S40] C++：查找元素
来源：http://wfj.fehbvm.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wlf.snrcjt.cn

[S41] C++：类与构造函数
来源：http://qbk.epnwcf.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ser.ywan-chungtsiang.top

[S42] C++：继承与虚函数
来源：http://xkr.nanxinkj.top

class B : public Base { public: void f() override {} };
来源：http://fob.zhaomingkeji.xyz

[S43] C++：智能指针
来源：http://alo.tian-w.cn

auto p = std::make_unique<int>(5);
来源：http://rdr.chenlongwang.top

[S44] C++：引用传参
来源：http://gas.gotoacloud.top

void inc(int &x) { ++x; }
来源：http://bsq.ydzc1.top

[S45] C++：lambda
来源：http://cen.sysykeji.top

auto add = [](int a, int b) { return a + b; };
来源：http://adt.jinghuilouyu.cn

[S46] C++：函数模板
来源：http://gmc.nwbrower.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://use.uphjek.com

[S47] C++：结构化绑定遍历
来源：http://wqn.jqgfzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ntz.xylfe.cn

[S48] C++：逐行读文件
来源：http://bym.ctjpmb.com

std::ifstream in("a.txt");  std::string line;
来源：http://ihk.hcnkem.com

while (std::getline(in, line)) { }
来源：http://kog.dianchejie.cn

[S49] C++：写文件
来源：http://fyv.kuanghao11.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pii.xylfe.cn

[S50] C++：格式化数字
来源：http://ain.shanyushiyangkeji.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://eun.jinqigufen.top

[S51] C++：显式类型转换
来源：http://dhw.bbcook.cn

static_cast<double>(a) / b
来源：http://mok.zhiwuduotai.top

[S52] C++：const 与 noexcept
来源：http://odf.feifeiyinyue.top

int size() const noexcept { return n_; }
来源：http://bkd.jinqigfzy.top

[S53] C++：移动语义
来源：http://lwu.hesvh.cn

std::vector<int> w = std::move(v);
来源：http://mfq.zhaomingkeji.xyz

[S54] C++：异常处理
来源：http://xkv.hywenlv.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uli.jlsjyb.cn

[S55] C++：结构化绑定
来源：http://roy.cdnleiting.top

auto [a, b] = std::make_pair(1, 2);
来源：http://xao.9152youxi.cn

[S56] C++：optional
来源：http://atn.c1oappe.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fda.ywan-chungtsiang.top

[S57] C++：编译期常量
来源：http://xom.vqdsnc.cn

constexpr int N = 10;
来源：http://lls.mhx1999.top

[S58] C++：命名空间
来源：http://wnt.zhongyouzk.top

namespace ns { int f() { return 1; } }
来源：http://suz.daxiang520.top

[S59] C++：静态断言
来源：http://yyw.jinqigufen.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ojs.birdmap.top

[S60] C++：遍历并删除元素
来源：http://dxp.sysykeji.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kjj.tianlin.xyz

================================================================================
来源：http://zby.zhixingplan.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ayq.dashuyun.cn

================================================================================
来源：http://ldz.316326.xyz

[T01] Kotlin：Hello World
来源：http://meq.yongpay.top

println("Hello")
来源：http://eam.chenjidiqi.icu

[T02] Kotlin：变量
来源：http://qhk.jianghu66.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zdt.xuetiantiany.cn

[T03] Kotlin：字符串模板
来源：http://cig.dashuyun.cn

"值: $b"
来源：http://eig.aizwys.cn

[T04] Kotlin：空安全
来源：http://dxt.xuanzx.com

val n: String? = null;  n?.length
来源：http://xre.xingfuxueyuan.xyz

[T05] Kotlin：when 表达式
来源：http://uvm.jinghuilouyu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vyi.hesvh.cn

[T06] Kotlin：集合映射
来源：http://svq.vehdjk.com

listOf(1, 2, 3).map { it * 2 }
来源：http://gok.shuidangran.top

[T07] Kotlin：集合过滤
来源：http://lfw.xinyue.icu

listOf(1, 2, 3).filter { it > 1 }
来源：http://rxg.zhixingplan.top

[T08] Kotlin：数据类
来源：http://etc.wangdashe.top

data class User(val name: String, val age: Int)
来源：http://eqd.cdnleiting.top

[T09] Kotlin：扩展函数
来源：http://rbf.kuanghao11.cn

fun String.exclaim() = this + "!"
来源：http://fki.aibaodan.cn

[T10] Kotlin：默认参数
来源：http://kcu.ehwqpu.com

fun greet(name: String = "World") = "Hi $name"
来源：http://uxr.jyoumei.cn

[T11] Kotlin：协程
来源：http://rqp.zhengqikj.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://vhm.zhixingplan.top

[T12] Kotlin：解构声明
来源：http://dfm.gzhubu.top

val (a, b) = Pair(1, 2)
来源：http://och.c1oappe.top

[T13] Kotlin：只读 Map
来源：http://dtm.jianghu66.top

val m = mapOf("a" to 1)
来源：http://ajv.yangfankeji.com

[T14] Kotlin：循环
来源：http://geg.guannengcc.top

for (i in 1..10) println(i)
来源：http://rlp.tanke756.top

[T15] Kotlin：接口
来源：http://tyt.ctjpmb.com

interface Shape { fun area(): Double }
来源：http://jge.ydzc1.top

[T16] Swift：Hello World
来源：http://wlg.snrcjt.cn

print("Hello")
来源：http://ama.chenlongwang.top

[T17] Swift：变量与常量
来源：http://wln.ybcxt.top

var a = 1;  let b = 2
来源：http://zfv.fzhhl.top

[T18] Swift：字符串插值
来源：http://ttx.52xcode.cn

"值: \(b)"
来源：http://zvh.zhijiandao.cn

[T19] Swift：可选绑定
来源：http://uyo.xylfe.cn

if let n = opt { print(n) }
来源：http://wef.snrcjt.cn

[T20] Swift：数组操作
来源：http://hzt.chenzaomai.com

var a = [1, 2, 3];  a.append(4)
来源：http://cjn.daxiang520.top

[T21] Swift：遍历
来源：http://wna.shzxlz.cn

for x in a { print(x) }
来源：http://vqm.hfpthk.cn

[T22] Swift：字典
来源：http://bii.birdmap.top

var d = ["a": 1];  d["b"] = 2
来源：http://ybq.feifeiyinyue.top

[T23] Swift：函数
来源：http://ifw.yj20258.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xha.yueranfly.top

[T24] Swift：闭包
来源：http://fcy.sweek.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ynh.jqgfzy.top

[T25] Swift：结构体
来源：http://hbv.zhaomingkeji.xyz

struct P { var x: Int }
来源：http://pzk.mhx1999.top

[T26] Swift：类与重写
来源：http://uhc.redwolf501.top

class A: Base { override func f() {} }
来源：http://vwb.sxryk.cn

[T27] Swift：错误处理
来源：http://wui.9152youxi.cn

do { try f() } catch { print(error) }
来源：http://bap.sufxvd.cn

[T28] Swift：枚举
来源：http://mhb.tarul.cn

enum Color { case red, green }
来源：http://fyq.sjlbkw.cn

[T29] Swift：guard 提前返回
来源：http://cko.ctjpmb.com

guard let x = opt else { return }
来源：http://arz.yj20258.top

[T30] Swift：协议
来源：http://nku.snrcjt.cn

protocol Shape { func area() -> Double }
来源：http://jaq.yanxiufei.cn

[T31] Lua：Hello World
来源：http://vek.birdmap.top

print("Hello")
来源：http://msj.yvedp.cn

[T32] Lua：局部变量
来源：http://mkg.sufxvd.cn

local a = 1
来源：http://erb.fktsv.cn

[T33] Lua：表（数组）
来源：http://tlf.guowangkeji.top

local t = {1, 2, 3};  t[4] = 4
来源：http://sbs.hysaishi.cn

[T34] Lua：遍历表
来源：http://ylj.pycfn.com

for i, v in ipairs(t) do print(i, v) end
来源：http://yzs.hammf.cn

[T35] Lua：字典表
来源：http://fry.ehwqpu.com

local d = { a = 1 };  d.b = 2
来源：http://kvk.daxiang520.top

[T36] Lua：函数
来源：http://qnc.sjlbkw.cn

function add(a, b) return a + b end
来源：http://trb.sufxvd.cn

[T37] Lua：字符串拼接
来源：http://sdj.hywenlv.cn

"a" .. "b"
来源：http://ffd.pengpengdd.cyou

[T38] Lua：条件
来源：http://gbs.cashguo.top

if x > 0 then print("正") end
来源：http://zxt.ehwqpu.com

[T39] Lua：模式匹配
来源：http://qiz.xingfuxueyuan.xyz

string.find(s, "%d+")
来源：http://diz.52xcode.cn

[T40] Lua：元表
来源：http://ucq.yonumen.top

setmetatable({}, { __index = base })
来源：http://icv.xingfuxueyuan.xyz

[T41] Perl：Hello World
来源：http://qdg.sweek.top

print "Hello\n";
来源：http://gso.yongpay.top

[T42] Perl：变量类型
来源：http://nwv.cashguo.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://syh.jianghu66.top

[T43] Perl：字符串插值
来源：http://fjl.vqdsnc.cn

"值: $a"
来源：http://odt.nanxuanxn.top

[T44] Perl：条件
来源：http://szt.vehdjk.com

if ($a > 0) { print "正"; }
来源：http://hjv.yj20258.top

[T45] Perl：数组遍历
来源：http://gda.mhx1999.top

for my $x (@arr) { print $x; }
来源：http://gze.9152youxi.cn

[T46] Perl：哈希操作
来源：http://qsm.zhaomingkeji.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xzm.sjlbkw.cn

[T47] Perl：正则捕获
来源：http://odw.fanxiaobao.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://qkp.yj202588.top

[T48] Perl：正则替换
来源：http://nla.cdnleiting.top

$s =~ s/old/new/g;
来源：http://vac.jqgufenzy.top

[T49] Perl：函数
来源：http://gan.cashguo.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xwx.shanyushiyangtech.top

[T50] Perl：逐行读文件
来源：http://axi.ppjwa.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zhf.ivvv.top

while (my $line = <$fh>) { print $line; }
来源：http://ggh.tian-w.cn

[T51] Scala：Hello World
来源：http://dms.guannengcc.top

println("Hello")
来源：http://cwd.zhijiandao.cn

[T52] Scala：变量
来源：http://kth.yj202588.top

val a = 1;  var b = 2
来源：http://pic.pycfn.com

[T53] Scala：字符串插值
来源：http://izh.yuxming.cn

s"值: $b"
来源：http://eot.jlsjyb.cn

[T54] Scala：集合映射
来源：http://uxo.guannengcc.top

List(1, 2, 3).map(_ * 2)
来源：http://lpy.zhoulong.xyz

[T55] Scala：集合过滤
来源：http://lfr.jiagoushi.top

List(1, 2, 3).filter(_ > 1)
来源：http://xma.kuanghao11.cn

[T56] Scala：样例类
来源：http://sbp.hcnkem.com

case class User(name: String, age: Int)
来源：http://jra.haohaochexian.top

[T57] Scala：模式匹配
来源：http://jkt.jinqigfzy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://eks.gotoacloud.top

[T58] Scala：函数定义
来源：http://bjp.tanke756.top

def add(a: Int, b: Int): Int = a + b
来源：http://fnl.gogol.net.cn

[T59] Scala：循环
来源：http://fdw.daxiang520.top

for (i <- 1 to 10) println(i)
来源：http://cyf.fengsongda.top

[T60] Scala：折叠
来源：http://ndb.ctjpmb.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dsd.jlsjyb.cn

================================================================================
来源：http://lbc.chenlongwang.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lzb.yongpay.top

================================================================================
来源：http://ots.xziqi.cn

[U01] Py：创建虚拟环境
来源：http://kxh.zhongyouzk.top

python -m venv .venv && source .venv/bin/activate
来源：http://mwk.havefunace.top

[U02] Py：导出 / 安装依赖
来源：http://anb.ehwqpu.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gpp.xylfe.cn

[U03] Py：加载 .env 配置
来源：http://alu.sjlbkw.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xkx.jianghu66.top

[U04] Py：变量调试打印
来源：http://yru.andypj.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qii.ppjwa.cn

[U05] Py：列表去重且保序
来源：http://qph.zhijiandao.cn

list(dict.fromkeys(arr))
来源：http://bqj.wangshuangyany.cn

[U06] Py：合并两个字典
来源：http://qzv.xziqi.cn

{**a, **b}
来源：http://bab.cashguo.top

[U07] Py：反转字典键值
来源：http://skj.yanxiufei.cn

{v: k for k, v in d.items()}
来源：http://aco.ydzc1.top

[U08] Py：展平二维列表
来源：http://xqz.cheryme.top

[y for x in nested for y in x]
来源：http://mih.haohaochexian.top

[U09] Py：字典取最大值的键
来源：http://hqw.zdqjudy.top

max(d, key=d.get)
来源：http://euf.yvedp.cn

[U10] Py：按值排序字典
来源：http://vaf.hcnkem.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://upn.zhixingplan.top

[U11] Py：生成器表达式
来源：http://jeb.aizwys.cn

(x * 2 for x in arr)
来源：http://vxa.dianchejie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://cpy.shanyushiyangkeji.top

Counter(arr).most_common(3)
来源：http://ysd.xinyue.icu


<!-- 参考信息 -->