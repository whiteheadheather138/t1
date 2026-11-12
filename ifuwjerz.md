代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://xxd.zycfv.cn

[R70] 时间戳与互转
来源：http://lff.uphjek.com

date +%s;  date -d @1700000000
来源：http://hav.kuanghao11.cn

[R71] 日期格式化
来源：http://ctn.zhongyouzk.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://cdh.chenzaomai.com

[R72] 等待端口就绪
来源：http://qlh.tianlin.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://fac.wangshuangyany.cn

[R73] 分割大日志
来源：http://zci.cdnleiting.top

split -l 1000 big.log part_
来源：http://pjt.ivvv.top

[R74] 批量重命名
来源：http://mod.xingfuxueyuan.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xvg.quarkkingdee.top

[R75] 导出环境变量
来源：http://exk.jinghuilouyu.cn

export PATH="$HOME/bin:$PATH"
来源：http://rsw.daxiang520.top

[R76] 使用临时文件
来源：http://tdr.birdmap.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pkk.zhengqikj.top

[R77] 读取用户输入
来源：http://fiv.9152youxi.cn

read -rp "请输入: " ans
来源：http://fct.nwbrower.top

[R78] 交互式菜单
来源：http://vxt.chenjidiqi.icu

select opt in a b c; do echo "$opt"; break; done
来源：http://hej.jlsjyb.cn

[R79] 解析命令行选项
来源：http://xml.yj20258888.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zvr.jinqigufen.top

[R80] 查看脚本执行耗时
来源：http://gls.yueranfly.top

time ./run.sh
来源：http://llf.jqgufenzy.top

================================================================================
来源：http://zqm.ehwqpu.com

S. C / C++ 专题
来源：http://lbs.redwolf501.top

================================================================================
来源：http://dnj.pengpengdd.cyou

[S01] C：Hello World
来源：http://eoq.hfpthk.cn

#include <stdio.h>
来源：http://sge.gzhubu.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://zdk.yongpay.top

[S02] C：变量与格式化输出
来源：http://lry.zhoulong.xyz

int a = 10; printf("%d\n", a);
来源：http://pcr.hcnkem.com

[S03] C：读入整数
来源：http://tii.shanyushiyangkeji.top

int x; scanf("%d", &x);
来源：http://iik.cucudq.cn

[S04] C：字符串复制
来源：http://vav.iojbl.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gji.xuanzx.com

[S05] C：字符串长度
来源：http://hci.sweek.top

strlen(s)
来源：http://knp.jlsjyb.cn

[S06] C：字符串比较
来源：http://rzx.sjlbkw.cn

strcmp(a, b) == 0
来源：http://jpu.hysaishi.cn

[S07] C：数组遍历求和
来源：http://amh.ivvv.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ndo.wangshuangyany.cn

[S08] C：动态内存分配与释放
来源：http://wdl.zhoulong.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jfy.0kj1m.cn

[S09] C：结构体定义与初始化
来源：http://paw.fzhhl.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ige.zhiwuduotai.top

[S10] C：指针与解引用
来源：http://agj.gaohongyu789.top

int *p = &a;  *p = 5;
来源：http://bjy.redwolf501.top

[S11] C：逐行读文件
来源：http://hpx.meibo888.top

FILE *f = fopen("a.txt", "r");
来源：http://vti.andypj.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://iwh.jinyuanbaomall.cn

fclose(f);
来源：http://tmi.redwolf501.top

[S12] C：写文件
来源：http://osw.chenzaomai.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dhc.jinghuilouyu.cn

[S13] C：宏定义
来源：http://asl.shanyushiyangkeji.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mqu.yj20258888.top

[S14] C：枚举
来源：http://fjr.sysykeji.top

enum Color { RED, GREEN, BLUE };
来源：http://msx.0kj1m.cn

[S15] C：类型转换
来源：http://hrn.sjlbkw.cn

(double) a / b
来源：http://zrt.cucudq.cn

[S16] C：位操作置位
来源：http://qcv.snrcjt.cn

x |= (1 << 3);
来源：http://lph.hfpthk.cn

[S17] C：安全拼接字符串
来源：http://dfk.ctjpmb.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sbb.ydzc1.top

[S18] C：命令行参数
来源：http://alc.gzhubu.top

int main(int argc, char **argv)
来源：http://lvd.jinghuilouyu.cn

[S19] C：快速排序
来源：http://bxe.jlsjyb.cn

qsort(a, n, sizeof(int), cmp);
来源：http://kps.snrcjt.cn

[S20] C：二分查找
来源：http://sdv.jinyuanbaomall.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://voc.birdmap.top

[S21] C：字符类别判断
来源：http://bux.hywenlv.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ikb.316326.xyz

[S22] C：字符串转数字
来源：http://stp.yuanzhike.top

atoi("42");  strtod("3.14", NULL);
来源：http://deu.hammf.cn

[S23] C：随机数
来源：http://zoe.nanxinkj.top

srand(time(NULL));  int r = rand() % 100;
来源：http://grt.sweek.top

[S24] C：获取本地时间
来源：http://qhg.sufxvd.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yxn.fengsongda.top

[S25] C：内存拷贝
来源：http://agr.ydzc1.top

memcpy(dst, src, n);
来源：http://lph.uphjek.com

[S26] C：内存清零
来源：http://ato.xylfe.cn

memset(a, 0, sizeof a);
来源：http://fig.epnwcf.com

[S27] C：定义常量
来源：http://rlx.kuanghao11.cn

const double PI = 3.14159;
来源：http://pcw.hnxiangtu.top

[S28] C：静态变量
来源：http://wfe.guannengcc.top

static int counter = 0;
来源：http://ipd.zdbjq.cn

[S29] C：变参函数
来源：http://uld.mhx1999.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vuy.smart0.xyz

[S30] C：头文件保护
来源：http://wmm.yangfankeji.com

#ifndef X_H
来源：http://czt.quarkkingdee.top

#define X_H
来源：http://rrj.jinqigfzy.top

#endif
来源：http://stx.hnqzz.top

[S31] C++：Hello World
来源：http://wzf.ppjwa.cn

#include <iostream>
来源：http://thm.ywan-chungtsiang.top

int main() { std::cout << "Hello\n"; }
来源：http://ttv.yongpay.top

[S32] C++：字符串
来源：http://kjs.svipenyu.cn

std::string s = "hi";  s += "!";
来源：http://drm.xuetiantiany.cn

[S33] C++：vector 增删
来源：http://brv.feifeiyinyue.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lru.aibaodan.cn

[S34] C++：遍历 vector
来源：http://rxv.yueranfly.top

for (auto &x : v) { std::cout << x; }
来源：http://neq.yuxming.cn

[S35] C++：map
来源：http://kcw.cheryme.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ywm.jinyuanbaomall.cn

[S36] C++：unordered_map
来源：http://bkv.nanxinkj.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pia.ivvv.top

[S37] C++：set
来源：http://bhj.vehdjk.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mmu.zhiwuduotai.top

[S38] C++：排序
来源：http://mkq.meibo888.top

std::sort(v.begin(), v.end());
来源：http://gzn.bjfxy.top

[S39] C++：自定义比较器排序
来源：http://pkk.nanxuanxn.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ncp.yuxming.cn

[S40] C++：查找元素
来源：http://hpq.sufxvd.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zyb.0kj1m.cn

[S41] C++：类与构造函数
来源：http://pmz.ctjpmb.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ptq.uphjek.com

[S42] C++：继承与虚函数
来源：http://xke.nwbrower.top

class B : public Base { public: void f() override {} };
来源：http://kwu.andypj.xyz

[S43] C++：智能指针
来源：http://slt.c1oappe.top

auto p = std::make_unique<int>(5);
来源：http://cbv.aizwys.cn

[S44] C++：引用传参
来源：http://owf.gaohongyu789.top

void inc(int &x) { ++x; }
来源：http://zxb.fengsongda.top

[S45] C++：lambda
来源：http://qvr.meibo888.top

auto add = [](int a, int b) { return a + b; };
来源：http://bgg.gzhubu.top

[S46] C++：函数模板
来源：http://oag.guowangkeji.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fou.jiagoushi.top

[S47] C++：结构化绑定遍历
来源：http://fbz.yuanzhike.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kzs.zycfv.cn

[S48] C++：逐行读文件
来源：http://uom.ydzc1.top

std::ifstream in("a.txt");  std::string line;
来源：http://bki.sysykeji.top

while (std::getline(in, line)) { }
来源：http://khm.nanxuanxn.top

[S49] C++：写文件
来源：http://jqr.svipenyu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://han.chenlongwang.top

[S50] C++：格式化数字
来源：http://luo.fktsv.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bcu.hammf.cn

[S51] C++：显式类型转换
来源：http://lmt.sufxvd.cn

static_cast<double>(a) / b
来源：http://ago.jinqigfzy.top

[S52] C++：const 与 noexcept
来源：http://rii.bbcook.cn

int size() const noexcept { return n_; }
来源：http://skm.hfpthk.cn

[S53] C++：移动语义
来源：http://rdx.zhiwuduotai.top

std::vector<int> w = std::move(v);
来源：http://ibk.meibo888.top

[S54] C++：异常处理
来源：http://gnt.fanxiaobao.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mml.ydjk.org.cn

[S55] C++：结构化绑定
来源：http://rgf.hammf.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wdg.quarkkingdee.top

[S56] C++：optional
来源：http://uwv.birdmap.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ztk.cqqwz.cn

[S57] C++：编译期常量
来源：http://jyi.0kj1m.cn

constexpr int N = 10;
来源：http://zlc.shanyushiyangkeji.top

[S58] C++：命名空间
来源：http://kpt.tian-w.cn

namespace ns { int f() { return 1; } }
来源：http://kev.iojbl.cn

[S59] C++：静态断言
来源：http://cdv.hnqzz.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qkp.gzhubu.top

[S60] C++：遍历并删除元素
来源：http://ctc.redwolf501.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fwb.hesvh.cn

================================================================================
来源：http://htt.jinqigufen.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lrj.yueranfly.top

================================================================================
来源：http://clt.smart0.xyz

[T01] Kotlin：Hello World
来源：http://nzg.jianghu66.top

println("Hello")
来源：http://svf.9152youxi.cn

[T02] Kotlin：变量
来源：http://vkb.jlsjyb.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qzj.quarkkingdee.top

[T03] Kotlin：字符串模板
来源：http://dcv.pycfn.com

"值: $b"
来源：http://lvd.aizwys.cn

[T04] Kotlin：空安全
来源：http://jhp.yvedp.cn

val n: String? = null;  n?.length
来源：http://xaj.yanxiufei.cn

[T05] Kotlin：when 表达式
来源：http://oxh.haohaochexian.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zsr.snrcjt.cn

[T06] Kotlin：集合映射
来源：http://mhg.quarkkingdee.top

listOf(1, 2, 3).map { it * 2 }
来源：http://evq.zhiwuduotai.top

[T07] Kotlin：集合过滤
来源：http://yws.chenzaomai.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://qjr.sysykeji.top

[T08] Kotlin：数据类
来源：http://otc.ctjpmb.com

data class User(val name: String, val age: Int)
来源：http://eaq.aizwys.cn

[T09] Kotlin：扩展函数
来源：http://sgh.daxiang520.top

fun String.exclaim() = this + "!"
来源：http://bgw.ivvv.top

[T10] Kotlin：默认参数
来源：http://yau.ctjpmb.com

fun greet(name: String = "World") = "Hi $name"
来源：http://stg.hammf.cn

[T11] Kotlin：协程
来源：http://ryu.jqgufenzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://nmw.chenjidiqi.icu

[T12] Kotlin：解构声明
来源：http://orl.andypj.xyz

val (a, b) = Pair(1, 2)
来源：http://ckt.xziqi.cn

[T13] Kotlin：只读 Map
来源：http://vur.snrcjt.cn

val m = mapOf("a" to 1)
来源：http://ilf.yuanzhike.top

[T14] Kotlin：循环
来源：http://etb.gzhubu.top

for (i in 1..10) println(i)
来源：http://jha.yfazqb.com

[T15] Kotlin：接口
来源：http://mkk.yj20258.top

interface Shape { fun area(): Double }
来源：http://osd.zhoulong.xyz

[T16] Swift：Hello World
来源：http://orp.ywan-chungtsiang.top

print("Hello")
来源：http://tas.andypj.xyz

[T17] Swift：变量与常量
来源：http://avi.quarkkingdee.top

var a = 1;  let b = 2
来源：http://zws.nwbrower.top

[T18] Swift：字符串插值
来源：http://sqe.gogol.net.cn

"值: \(b)"
来源：http://xoj.xuanzx.com

[T19] Swift：可选绑定
来源：http://qmk.316326.xyz

if let n = opt { print(n) }
来源：http://ujj.xuanzx.com

[T20] Swift：数组操作
来源：http://rla.quarkkingdee.top

var a = [1, 2, 3];  a.append(4)
来源：http://jhu.ivvv.top

[T21] Swift：遍历
来源：http://hzq.hongshengwenyu.top

for x in a { print(x) }
来源：http://rvo.yj202588.top

[T22] Swift：字典
来源：http://ttw.shanyushiyangkeji.top

var d = ["a": 1];  d["b"] = 2
来源：http://kfo.ydzc1.top

[T23] Swift：函数
来源：http://vvo.ybcxt.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nox.cqqwz.cn

[T24] Swift：闭包
来源：http://pns.shuidangran.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://iem.jiagoushi.top

[T25] Swift：结构体
来源：http://rks.fzhhl.top

struct P { var x: Int }
来源：http://nnt.fanxiaobao.xyz

[T26] Swift：类与重写
来源：http://gqs.aizwys.cn

class A: Base { override func f() {} }
来源：http://rgy.xinyue.icu

[T27] Swift：错误处理
来源：http://qgv.cheryme.top

do { try f() } catch { print(error) }
来源：http://trt.havefunace.top

[T28] Swift：枚举
来源：http://rau.pycfn.com

enum Color { case red, green }
来源：http://qyx.tarul.cn

[T29] Swift：guard 提前返回
来源：http://cgg.jyoumei.cn

guard let x = opt else { return }
来源：http://nrj.tian-w.cn

[T30] Swift：协议
来源：http://enh.yj20258888.top

protocol Shape { func area() -> Double }
来源：http://brg.cdnleiting.top

[T31] Lua：Hello World
来源：http://jqo.jinghuilouyu.cn

print("Hello")
来源：http://vnb.vehdjk.com

[T32] Lua：局部变量
来源：http://gzh.fehbvm.com

local a = 1
来源：http://asm.zhengqikj.top

[T33] Lua：表（数组）
来源：http://dsl.zhijiandao.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xmj.xinyue.icu

[T34] Lua：遍历表
来源：http://nar.jinyuanbaomall.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://gfc.fengsongda.top

[T35] Lua：字典表
来源：http://zap.xuetiantiany.cn

local d = { a = 1 };  d.b = 2
来源：http://ykj.dianchejie.cn

[T36] Lua：函数
来源：http://uml.sjlbkw.cn

function add(a, b) return a + b end
来源：http://gpr.daria6918.cn

[T37] Lua：字符串拼接
来源：http://ahv.zdbjq.cn

"a" .. "b"
来源：http://chu.shangyingyoupin.top

[T38] Lua：条件
来源：http://ybh.ivvv.top

if x > 0 then print("正") end
来源：http://plc.ydzc1.top

[T39] Lua：模式匹配
来源：http://acl.redwolf501.top

string.find(s, "%d+")
来源：http://zzp.birdmap.top

[T40] Lua：元表
来源：http://kav.yanxiufei.cn

setmetatable({}, { __index = base })
来源：http://jrt.aibaodan.cn

[T41] Perl：Hello World
来源：http://fqf.chenlongwang.top

print "Hello\n";
来源：http://uwx.hcnkem.com

[T42] Perl：变量类型
来源：http://zrj.zhengqikj.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rll.jinghuilouyu.cn

[T43] Perl：字符串插值
来源：http://vgw.guannengcc.top

"值: $a"
来源：http://kaj.mhx1999.top

[T44] Perl：条件
来源：http://vht.shangyingyoupin.top

if ($a > 0) { print "正"; }
来源：http://kax.bjfxy.top

[T45] Perl：数组遍历
来源：http://zuf.havefunace.top

for my $x (@arr) { print $x; }
来源：http://dwt.kuanghao11.cn

[T46] Perl：哈希操作
来源：http://vvy.tianlin.xyz

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mvu.zhiwuduotai.top

[T47] Perl：正则捕获
来源：http://jwb.zhoulong.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://wzt.dianchejie.cn

[T48] Perl：正则替换
来源：http://xat.fktsv.cn

$s =~ s/old/new/g;
来源：http://kzh.haohaochexian.top

[T49] Perl：函数
来源：http://vaq.zycfv.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nkw.xuetiantiany.cn

[T50] Perl：逐行读文件
来源：http://qdu.jianghu66.top

open my $fh, "<", "a.txt" or die $!;
来源：http://xkt.sxryk.cn

while (my $line = <$fh>) { print $line; }
来源：http://qoe.zhixingplan.top

[T51] Scala：Hello World
来源：http://aft.cucudq.cn

println("Hello")
来源：http://slp.jlsjyb.cn

[T52] Scala：变量
来源：http://mtg.zhongyouzk.top

val a = 1;  var b = 2
来源：http://vvo.epnwcf.com

[T53] Scala：字符串插值
来源：http://imh.shanyushiyangkeji.top

s"值: $b"
来源：http://crp.ppjwa.cn

[T54] Scala：集合映射
来源：http://tbu.guannengcc.top

List(1, 2, 3).map(_ * 2)
来源：http://yqk.zhaomingkeji.xyz

[T55] Scala：集合过滤
来源：http://fmj.vqdsnc.cn

List(1, 2, 3).filter(_ > 1)
来源：http://rov.jyoumei.cn

[T56] Scala：样例类
来源：http://nse.iojbl.cn

case class User(name: String, age: Int)
来源：http://yrb.ybcxt.top

[T57] Scala：模式匹配
来源：http://shx.chenlongwang.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://yfn.cqqwz.cn

[T58] Scala：函数定义
来源：http://uug.iojbl.cn

def add(a: Int, b: Int): Int = a + b
来源：http://nrg.iojbl.cn

[T59] Scala：循环
来源：http://vkk.zhixingplan.top

for (i <- 1 to 10) println(i)
来源：http://sed.gaohongyu789.top

[T60] Scala：折叠
来源：http://ran.fktsv.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://oop.jlsjyb.cn

================================================================================
来源：http://osl.zhiwuduotai.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nnc.xingfuxueyuan.xyz

================================================================================
来源：http://mrk.jyoumei.cn

[U01] Py：创建虚拟环境
来源：http://nvo.xylfe.cn

python -m venv .venv && source .venv/bin/activate
来源：http://kfb.nwbrower.top

[U02] Py：导出 / 安装依赖
来源：http://bva.epnwcf.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nwm.zhixingplan.top

[U03] Py：加载 .env 配置
来源：http://bat.cheryme.top

from dotenv import load_dotenv; load_dotenv()
来源：http://whd.tarul.cn

[U04] Py：变量调试打印
来源：http://cdm.cucudq.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zmi.quarkkingdee.top

[U05] Py：列表去重且保序
来源：http://xhu.c1oappe.top

list(dict.fromkeys(arr))
来源：http://nzj.jqgfzy.top

[U06] Py：合并两个字典
来源：http://tzr.yanxiufei.cn

{**a, **b}
来源：http://qas.zhoulong.xyz

[U07] Py：反转字典键值
来源：http://xil.zhaomingkeji.xyz

{v: k for k, v in d.items()}
来源：http://haw.shanyushiyangkeji.top

[U08] Py：展平二维列表
来源：http://lnl.ywan-chungtsiang.top

[y for x in nested for y in x]
来源：http://niy.hnqzz.top

[U09] Py：字典取最大值的键
来源：http://oge.aizwys.cn

max(d, key=d.get)
来源：http://ksx.shangyingyoupin.top

[U10] Py：按值排序字典
来源：http://ewd.ydzc1.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ods.ehwqpu.com


<!-- 参考信息 -->