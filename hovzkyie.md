代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://ezu.epnwcf.com

[R70] 时间戳与互转
来源：http://vqi.chenzaomai.com

date +%s;  date -d @1700000000
来源：http://gxt.daxiang520.top

[R71] 日期格式化
来源：http://whh.chenlongwang.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://xmc.hesvh.cn

[R72] 等待端口就绪
来源：http://ngn.jyoumei.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://uit.jqgufenzy.top

[R73] 分割大日志
来源：http://hjh.svipenyu.cn

split -l 1000 big.log part_
来源：http://mls.ehwqpu.com

[R74] 批量重命名
来源：http://meo.guowangkeji.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ysz.9152youxi.cn

[R75] 导出环境变量
来源：http://ptp.kuanghao11.cn

export PATH="$HOME/bin:$PATH"
来源：http://ein.chenlongwang.top

[R76] 使用临时文件
来源：http://hxt.yuxming.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lwd.aibaodan.cn

[R77] 读取用户输入
来源：http://rdn.zdqjudy.top

read -rp "请输入: " ans
来源：http://ywq.zhijiandao.cn

[R78] 交互式菜单
来源：http://kxe.hcnkem.com

select opt in a b c; do echo "$opt"; break; done
来源：http://noz.guowangkeji.top

[R79] 解析命令行选项
来源：http://agk.jqgufenzy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xuf.nanxuanxn.top

[R80] 查看脚本执行耗时
来源：http://xri.shanyushiyangtech.top

time ./run.sh
来源：http://pgo.cheryme.top

================================================================================
来源：http://qkj.sjlbkw.cn

S. C / C++ 专题
来源：http://zfo.yueranfly.top

================================================================================
来源：http://bic.zhaomingkeji.xyz

[S01] C：Hello World
来源：http://vrk.yvedp.cn

#include <stdio.h>
来源：http://qqi.xziqi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://yjk.fzhhl.top

[S02] C：变量与格式化输出
来源：http://zlv.jqgfzy.top

int a = 10; printf("%d\n", a);
来源：http://cgj.ppjwa.cn

[S03] C：读入整数
来源：http://jfb.yueranfly.top

int x; scanf("%d", &x);
来源：http://myd.hesvh.cn

[S04] C：字符串复制
来源：http://dij.hcnkem.com

char dst[32]; strcpy(dst, "hi");
来源：http://rrq.shanyushiyangkeji.top

[S05] C：字符串长度
来源：http://fvs.ppjwa.cn

strlen(s)
来源：http://pei.316326.xyz

[S06] C：字符串比较
来源：http://zho.birdmap.top

strcmp(a, b) == 0
来源：http://khm.aizwys.cn

[S07] C：数组遍历求和
来源：http://nir.hesvh.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cic.zhaomingkeji.xyz

[S08] C：动态内存分配与释放
来源：http://sca.zhoulong.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gxe.fengsongda.top

[S09] C：结构体定义与初始化
来源：http://wqt.ybcxt.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ivt.ivvv.top

[S10] C：指针与解引用
来源：http://lfb.cqqwz.cn

int *p = &a;  *p = 5;
来源：http://prz.feifeiyinyue.top

[S11] C：逐行读文件
来源：http://qtl.0kj1m.cn

FILE *f = fopen("a.txt", "r");
来源：http://pku.vehdjk.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://bnm.cucudq.cn

fclose(f);
来源：http://rif.yangfankeji.com

[S12] C：写文件
来源：http://chh.shangyingyoupin.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jmv.hcnkem.com

[S13] C：宏定义
来源：http://vui.zhiwuduotai.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://thy.zhaomingkeji.xyz

[S14] C：枚举
来源：http://gnl.ydzc1.top

enum Color { RED, GREEN, BLUE };
来源：http://ghq.fktsv.cn

[S15] C：类型转换
来源：http://yzr.hongshengwenyu.top

(double) a / b
来源：http://lgf.jqgufenzy.top

[S16] C：位操作置位
来源：http://oto.xziqi.cn

x |= (1 << 3);
来源：http://bku.feifeiyinyue.top

[S17] C：安全拼接字符串
来源：http://tve.fzhhl.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mxt.tanke756.top

[S18] C：命令行参数
来源：http://gvo.wangdashe.top

int main(int argc, char **argv)
来源：http://jzi.ehwqpu.com

[S19] C：快速排序
来源：http://afo.mhx1999.top

qsort(a, n, sizeof(int), cmp);
来源：http://iqo.yuxming.cn

[S20] C：二分查找
来源：http://bba.yuanzhike.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xfd.epnwcf.com

[S21] C：字符类别判断
来源：http://zmm.vehdjk.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://puz.c1oappe.top

[S22] C：字符串转数字
来源：http://ucq.cheryme.top

atoi("42");  strtod("3.14", NULL);
来源：http://xfb.ybcxt.top

[S23] C：随机数
来源：http://lrn.chenlongwang.top

srand(time(NULL));  int r = rand() % 100;
来源：http://fca.hysaishi.cn

[S24] C：获取本地时间
来源：http://wzz.smart0.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rmn.sweek.top

[S25] C：内存拷贝
来源：http://uqf.yangfankeji.com

memcpy(dst, src, n);
来源：http://onh.feifeiyinyue.top

[S26] C：内存清零
来源：http://pnl.ctjpmb.com

memset(a, 0, sizeof a);
来源：http://tth.pengpengdd.cyou

[S27] C：定义常量
来源：http://vud.hfpthk.cn

const double PI = 3.14159;
来源：http://bgn.sysykeji.top

[S28] C：静态变量
来源：http://wdv.epnwcf.com

static int counter = 0;
来源：http://syn.feifeiyinyue.top

[S29] C：变参函数
来源：http://qjk.snrcjt.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pme.9152youxi.cn

[S30] C：头文件保护
来源：http://gkh.zhixingplan.top

#ifndef X_H
来源：http://bjj.feifeiyinyue.top

#define X_H
来源：http://jgs.xylfe.cn

#endif
来源：http://oae.hongshengwenyu.top

[S31] C++：Hello World
来源：http://ask.9152youxi.cn

#include <iostream>
来源：http://qgm.kuanghao11.cn

int main() { std::cout << "Hello\n"; }
来源：http://tat.dianchejie.cn

[S32] C++：字符串
来源：http://nnx.zycfv.cn

std::string s = "hi";  s += "!";
来源：http://kia.9152youxi.cn

[S33] C++：vector 增删
来源：http://ono.nwbrower.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kht.zhaomingkeji.xyz

[S34] C++：遍历 vector
来源：http://jxp.yuxming.cn

for (auto &x : v) { std::cout << x; }
来源：http://hxy.c1oappe.top

[S35] C++：map
来源：http://adb.yongpay.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ydt.jqgufenzy.top

[S36] C++：unordered_map
来源：http://nqz.jlsjyb.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rrl.zhijiandao.cn

[S37] C++：set
来源：http://ifl.andypj.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ggb.wangshuangyany.cn

[S38] C++：排序
来源：http://fpl.hywenlv.cn

std::sort(v.begin(), v.end());
来源：http://jzl.zhongyouzk.top

[S39] C++：自定义比较器排序
来源：http://sog.cqqwz.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uiy.ctjpmb.com

[S40] C++：查找元素
来源：http://bqk.snrcjt.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sls.snrcjt.cn

[S41] C++：类与构造函数
来源：http://bgn.pengpengdd.cyou

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://aru.hesvh.cn

[S42] C++：继承与虚函数
来源：http://kfh.jinqigfzy.top

class B : public Base { public: void f() override {} };
来源：http://wve.ctjpmb.com

[S43] C++：智能指针
来源：http://beo.shanyushiyangkeji.top

auto p = std::make_unique<int>(5);
来源：http://anv.hnxiangtu.top

[S44] C++：引用传参
来源：http://wqw.yj20258.top

void inc(int &x) { ++x; }
来源：http://kxa.yanxiufei.cn

[S45] C++：lambda
来源：http://clt.xuanzx.com

auto add = [](int a, int b) { return a + b; };
来源：http://vip.shuidangran.top

[S46] C++：函数模板
来源：http://xjp.wangdashe.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tho.ywan-chungtsiang.top

[S47] C++：结构化绑定遍历
来源：http://hqw.sufxvd.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rnm.chenjidiqi.icu

[S48] C++：逐行读文件
来源：http://tea.cdnleiting.top

std::ifstream in("a.txt");  std::string line;
来源：http://meo.dianchejie.cn

while (std::getline(in, line)) { }
来源：http://gyx.zhoulong.xyz

[S49] C++：写文件
来源：http://uqz.redwolf501.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dbb.cashguo.top

[S50] C++：格式化数字
来源：http://avo.gotoacloud.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://syx.cashguo.top

[S51] C++：显式类型转换
来源：http://qzk.gotoacloud.top

static_cast<double>(a) / b
来源：http://kqs.haohaochexian.top

[S52] C++：const 与 noexcept
来源：http://six.yj202588.top

int size() const noexcept { return n_; }
来源：http://iep.epnwcf.com

[S53] C++：移动语义
来源：http://vpj.smart0.xyz

std::vector<int> w = std::move(v);
来源：http://uha.jqgufenzy.top

[S54] C++：异常处理
来源：http://dhe.ivvv.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qnq.shanyushiyangtech.top

[S55] C++：结构化绑定
来源：http://qdw.yuanzhike.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ear.jinqigfzy.top

[S56] C++：optional
来源：http://uca.sjlbkw.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kvm.316326.xyz

[S57] C++：编译期常量
来源：http://seu.yj20258.top

constexpr int N = 10;
来源：http://zfx.bjfxy.top

[S58] C++：命名空间
来源：http://etw.52xcode.cn

namespace ns { int f() { return 1; } }
来源：http://qcl.52xcode.cn

[S59] C++：静态断言
来源：http://spp.jqgfzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gvp.feifeiyinyue.top

[S60] C++：遍历并删除元素
来源：http://nku.kuanghao11.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dol.yuxming.cn

================================================================================
来源：http://naj.fehbvm.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qbk.xuetiantiany.cn

================================================================================
来源：http://tpp.chenzaomai.com

[T01] Kotlin：Hello World
来源：http://lrq.hywenlv.cn

println("Hello")
来源：http://qeh.ppjwa.cn

[T02] Kotlin：变量
来源：http://sic.xuanzx.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ezb.fktsv.cn

[T03] Kotlin：字符串模板
来源：http://fqj.aizwys.cn

"值: $b"
来源：http://xkp.yfazqb.com

[T04] Kotlin：空安全
来源：http://mjh.tianlin.xyz

val n: String? = null;  n?.length
来源：http://aes.gotoacloud.top

[T05] Kotlin：when 表达式
来源：http://ggj.yj20258888.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xes.xziqi.cn

[T06] Kotlin：集合映射
来源：http://cwx.vehdjk.com

listOf(1, 2, 3).map { it * 2 }
来源：http://hgp.xuanzx.com

[T07] Kotlin：集合过滤
来源：http://rho.zhixingplan.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://pcm.jlsjyb.cn

[T08] Kotlin：数据类
来源：http://efv.ywan-chungtsiang.top

data class User(val name: String, val age: Int)
来源：http://pid.zhongyouzk.top

[T09] Kotlin：扩展函数
来源：http://tlh.jinyuanbaomall.cn

fun String.exclaim() = this + "!"
来源：http://klm.zhijiandao.cn

[T10] Kotlin：默认参数
来源：http://tyf.nanxinkj.top

fun greet(name: String = "World") = "Hi $name"
来源：http://kva.shanyushiyangtech.top

[T11] Kotlin：协程
来源：http://drj.52xcode.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vhm.sxryk.cn

[T12] Kotlin：解构声明
来源：http://jgz.yfazqb.com

val (a, b) = Pair(1, 2)
来源：http://bue.chenzaomai.com

[T13] Kotlin：只读 Map
来源：http://ldx.zycfv.cn

val m = mapOf("a" to 1)
来源：http://vzg.dashuyun.cn

[T14] Kotlin：循环
来源：http://evm.ydzc1.top

for (i in 1..10) println(i)
来源：http://xlz.yuanzhike.top

[T15] Kotlin：接口
来源：http://vrd.shanyushiyangtech.top

interface Shape { fun area(): Double }
来源：http://oeg.daria6918.cn

[T16] Swift：Hello World
来源：http://sff.zdbjq.cn

print("Hello")
来源：http://ciu.pycfn.com

[T17] Swift：变量与常量
来源：http://thf.birdmap.top

var a = 1;  let b = 2
来源：http://qxv.dashuyun.cn

[T18] Swift：字符串插值
来源：http://hbr.sjlbkw.cn

"值: \(b)"
来源：http://gel.sysykeji.top

[T19] Swift：可选绑定
来源：http://xsh.kuanghao11.cn

if let n = opt { print(n) }
来源：http://nut.zhengqikj.top

[T20] Swift：数组操作
来源：http://ggs.iojbl.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hwn.bbcook.cn

[T21] Swift：遍历
来源：http://zee.yj202588.top

for x in a { print(x) }
来源：http://yru.xinyue.icu

[T22] Swift：字典
来源：http://jxj.jinqigfzy.top

var d = ["a": 1];  d["b"] = 2
来源：http://oad.ivvv.top

[T23] Swift：函数
来源：http://jej.tian-w.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gfa.cucudq.cn

[T24] Swift：闭包
来源：http://kar.yuanzhike.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://nvz.sjlbkw.cn

[T25] Swift：结构体
来源：http://xhe.yj20258888.top

struct P { var x: Int }
来源：http://usu.ywan-chungtsiang.top

[T26] Swift：类与重写
来源：http://izn.ywan-chungtsiang.top

class A: Base { override func f() {} }
来源：http://qgh.nwbrower.top

[T27] Swift：错误处理
来源：http://gsl.havefunace.top

do { try f() } catch { print(error) }
来源：http://knt.pengpengdd.cyou

[T28] Swift：枚举
来源：http://mcm.hfpthk.cn

enum Color { case red, green }
来源：http://faj.tianlin.xyz

[T29] Swift：guard 提前返回
来源：http://sxq.zhaomingkeji.xyz

guard let x = opt else { return }
来源：http://qls.cdnleiting.top

[T30] Swift：协议
来源：http://nku.nanxinkj.top

protocol Shape { func area() -> Double }
来源：http://emw.iojbl.cn

[T31] Lua：Hello World
来源：http://nre.jinqigfzy.top

print("Hello")
来源：http://ljg.jianghu66.top

[T32] Lua：局部变量
来源：http://ijv.sufxvd.cn

local a = 1
来源：http://ofb.yongpay.top

[T33] Lua：表（数组）
来源：http://kur.shanyushiyangtech.top

local t = {1, 2, 3};  t[4] = 4
来源：http://tvu.yj20258.top

[T34] Lua：遍历表
来源：http://svs.andypj.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://hil.jinghuilouyu.cn

[T35] Lua：字典表
来源：http://rbw.ybcxt.top

local d = { a = 1 };  d.b = 2
来源：http://jgy.yfazqb.com

[T36] Lua：函数
来源：http://rpl.svipenyu.cn

function add(a, b) return a + b end
来源：http://xnv.bbcook.cn

[T37] Lua：字符串拼接
来源：http://xdp.0kj1m.cn

"a" .. "b"
来源：http://ogb.yj20258.top

[T38] Lua：条件
来源：http://elg.ehwqpu.com

if x > 0 then print("正") end
来源：http://jhl.iojbl.cn

[T39] Lua：模式匹配
来源：http://cko.yfazqb.com

string.find(s, "%d+")
来源：http://era.andypj.xyz

[T40] Lua：元表
来源：http://nyq.nanxinkj.top

setmetatable({}, { __index = base })
来源：http://fzg.zhiwuduotai.top

[T41] Perl：Hello World
来源：http://nzk.zhaomingkeji.xyz

print "Hello\n";
来源：http://azl.jinqigufen.top

[T42] Perl：变量类型
来源：http://yiu.gotoacloud.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vmf.zhoulong.xyz

[T43] Perl：字符串插值
来源：http://ihk.0kj1m.cn

"值: $a"
来源：http://cdw.gotoacloud.top

[T44] Perl：条件
来源：http://pco.yueranfly.top

if ($a > 0) { print "正"; }
来源：http://ncx.havefunace.top

[T45] Perl：数组遍历
来源：http://ith.tianlin.xyz

for my $x (@arr) { print $x; }
来源：http://pvt.shanyushiyangtech.top

[T46] Perl：哈希操作
来源：http://ywn.sufxvd.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rqz.ppjwa.cn

[T47] Perl：正则捕获
来源：http://gsh.yongpay.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ste.hnqzz.top

[T48] Perl：正则替换
来源：http://vmu.yfazqb.com

$s =~ s/old/new/g;
来源：http://bjh.cdnleiting.top

[T49] Perl：函数
来源：http://lpw.cdnleiting.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pkz.sxryk.cn

[T50] Perl：逐行读文件
来源：http://ijk.bjfxy.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ets.shanyushiyangtech.top

while (my $line = <$fh>) { print $line; }
来源：http://hxx.c1oappe.top

[T51] Scala：Hello World
来源：http://qwq.cucudq.cn

println("Hello")
来源：http://fpg.tanke756.top

[T52] Scala：变量
来源：http://fyb.xylfe.cn

val a = 1;  var b = 2
来源：http://gca.wangshuangyany.cn

[T53] Scala：字符串插值
来源：http://spm.aizwys.cn

s"值: $b"
来源：http://hcp.aibaodan.cn

[T54] Scala：集合映射
来源：http://jhb.shzxlz.cn

List(1, 2, 3).map(_ * 2)
来源：http://jvu.yvedp.cn

[T55] Scala：集合过滤
来源：http://jsw.ivvv.top

List(1, 2, 3).filter(_ > 1)
来源：http://ofk.yfazqb.com

[T56] Scala：样例类
来源：http://kkm.wangdashe.top

case class User(name: String, age: Int)
来源：http://agr.guowangkeji.top

[T57] Scala：模式匹配
来源：http://jzu.cqqwz.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://fsn.redwolf501.top

[T58] Scala：函数定义
来源：http://qav.jqgfzy.top

def add(a: Int, b: Int): Int = a + b
来源：http://kmw.hywenlv.cn

[T59] Scala：循环
来源：http://qje.pengpengdd.cyou

for (i <- 1 to 10) println(i)
来源：http://dgz.jlsjyb.cn

[T60] Scala：折叠
来源：http://vkx.hongshengwenyu.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kph.hnxiangtu.top

================================================================================
来源：http://gfh.zhijiandao.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yms.sweek.top

================================================================================
来源：http://sas.nanxuanxn.top

[U01] Py：创建虚拟环境
来源：http://zfd.hongshengwenyu.top

python -m venv .venv && source .venv/bin/activate
来源：http://bld.gzhubu.top

[U02] Py：导出 / 安装依赖
来源：http://fou.ydjk.org.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ntk.uphjek.com

[U03] Py：加载 .env 配置
来源：http://drw.wangshuangyany.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://jep.ydzc1.top

[U04] Py：变量调试打印
来源：http://vhw.dianchejie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ttw.jinqigufen.top

[U05] Py：列表去重且保序
来源：http://xid.52xcode.cn

list(dict.fromkeys(arr))
来源：http://ydx.hfpthk.cn

[U06] Py：合并两个字典
来源：http://ecq.tanke756.top

{**a, **b}
来源：http://jab.jinghuilouyu.cn

[U07] Py：反转字典键值
来源：http://chi.quarkkingdee.top

{v: k for k, v in d.items()}
来源：http://fnp.hesvh.cn

[U08] Py：展平二维列表
来源：http://ogd.tianlin.xyz

[y for x in nested for y in x]
来源：http://xgq.hfpthk.cn

[U09] Py：字典取最大值的键
来源：http://eme.jqgfzy.top

max(d, key=d.get)
来源：http://zai.yangfankeji.com

[U10] Py：按值排序字典
来源：http://ygr.xingfuxueyuan.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://pem.jyoumei.cn


<!-- 参考信息 -->