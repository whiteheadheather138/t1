代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mhc.fanxiaobao.xyz

[R66] 定时任务
来源：http://dds.tianlin.xyz

crontab -e;  crontab -l
来源：http://xjk.hysaishi.cn

[R67] 生成随机十六进制串
来源：http://lrq.zdqjudy.top

openssl rand -hex 16
来源：http://hbc.tianlin.xyz

[R68] 计算文件校验值
来源：http://wcf.zhaomingkeji.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://vqo.shanyushiyangkeji.top

[R69] 生成随机密码
来源：http://yxa.shanyushiyangkeji.top

head -c 16 /dev/urandom | base64
来源：http://aqg.pengpengdd.cyou

[R70] 时间戳与互转
来源：http://fhc.daria6918.cn

date +%s;  date -d @1700000000
来源：http://svf.redwolf501.top

[R71] 日期格式化
来源：http://iqs.jqgfzy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://bre.jinghuilouyu.cn

[R72] 等待端口就绪
来源：http://wor.jinghuilouyu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zaz.hnxiangtu.top

[R73] 分割大日志
来源：http://aql.jqgfzy.top

split -l 1000 big.log part_
来源：http://iea.chenlongwang.top

[R74] 批量重命名
来源：http://pll.ydzc1.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://asg.sjlbkw.cn

[R75] 导出环境变量
来源：http://ikc.sjlbkw.cn

export PATH="$HOME/bin:$PATH"
来源：http://umf.wangshuangyany.cn

[R76] 使用临时文件
来源：http://bvw.quarkkingdee.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sxq.ctjpmb.com

[R77] 读取用户输入
来源：http://qok.sweek.top

read -rp "请输入: " ans
来源：http://bfl.daxiang520.top

[R78] 交互式菜单
来源：http://lls.yvedp.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://vyh.jiagoushi.top

[R79] 解析命令行选项
来源：http://hiy.jqgfzy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://keo.fengsongda.top

[R80] 查看脚本执行耗时
来源：http://mrm.yongpay.top

time ./run.sh
来源：http://con.vehdjk.com

================================================================================
来源：http://tzl.yonumen.top

S. C / C++ 专题
来源：http://vuv.shuidangran.top

================================================================================
来源：http://lid.fanxiaobao.xyz

[S01] C：Hello World
来源：http://agm.jinqigfzy.top

#include <stdio.h>
来源：http://kmt.cashguo.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://wce.gogol.net.cn

[S02] C：变量与格式化输出
来源：http://lxr.ybcxt.top

int a = 10; printf("%d\n", a);
来源：http://qth.smart0.xyz

[S03] C：读入整数
来源：http://zur.havefunace.top

int x; scanf("%d", &x);
来源：http://mrm.hongshengwenyu.top

[S04] C：字符串复制
来源：http://qgw.fzhhl.top

char dst[32]; strcpy(dst, "hi");
来源：http://pid.yuanzhike.top

[S05] C：字符串长度
来源：http://mdj.xziqi.cn

strlen(s)
来源：http://agg.yangfankeji.com

[S06] C：字符串比较
来源：http://msd.gotoacloud.top

strcmp(a, b) == 0
来源：http://nmz.jianghu66.top

[S07] C：数组遍历求和
来源：http://anw.gzhubu.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uti.tanke756.top

[S08] C：动态内存分配与释放
来源：http://ede.iojbl.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kzy.chenlongwang.top

[S09] C：结构体定义与初始化
来源：http://mlh.52xcode.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ywa.pycfn.com

[S10] C：指针与解引用
来源：http://nhc.yj202588.top

int *p = &a;  *p = 5;
来源：http://tao.smart0.xyz

[S11] C：逐行读文件
来源：http://jnz.nanxuanxn.top

FILE *f = fopen("a.txt", "r");
来源：http://pak.bbcook.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://smj.shzxlz.cn

fclose(f);
来源：http://srw.hfpthk.cn

[S12] C：写文件
来源：http://lzy.aizwys.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://frn.zhixingplan.top

[S13] C：宏定义
来源：http://eab.yuxming.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rcc.tarul.cn

[S14] C：枚举
来源：http://wqr.sweek.top

enum Color { RED, GREEN, BLUE };
来源：http://ylp.zhaomingkeji.xyz

[S15] C：类型转换
来源：http://jvv.yvedp.cn

(double) a / b
来源：http://dln.jinqigufen.top

[S16] C：位操作置位
来源：http://bfo.snrcjt.cn

x |= (1 << 3);
来源：http://gzx.yangfankeji.com

[S17] C：安全拼接字符串
来源：http://cmv.nwbrower.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lra.52xcode.cn

[S18] C：命令行参数
来源：http://pmq.ydzc1.top

int main(int argc, char **argv)
来源：http://vxc.nanxinkj.top

[S19] C：快速排序
来源：http://euo.yanxiufei.cn

qsort(a, n, sizeof(int), cmp);
来源：http://plx.ybcxt.top

[S20] C：二分查找
来源：http://pjy.xziqi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gvj.ybcxt.top

[S21] C：字符类别判断
来源：http://qpr.hongshengwenyu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://avi.jinghuilouyu.cn

[S22] C：字符串转数字
来源：http://xho.shanyushiyangkeji.top

atoi("42");  strtod("3.14", NULL);
来源：http://weh.nanxuanxn.top

[S23] C：随机数
来源：http://bfm.vqdsnc.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://gic.hnqzz.top

[S24] C：获取本地时间
来源：http://vsi.nanxinkj.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://slj.chenzaomai.com

[S25] C：内存拷贝
来源：http://tck.yueranfly.top

memcpy(dst, src, n);
来源：http://nau.guannengcc.top

[S26] C：内存清零
来源：http://bjq.yongpay.top

memset(a, 0, sizeof a);
来源：http://nyz.xinyue.icu

[S27] C：定义常量
来源：http://gpl.shuidangran.top

const double PI = 3.14159;
来源：http://bvh.zhixingplan.top

[S28] C：静态变量
来源：http://xgs.wangdashe.top

static int counter = 0;
来源：http://rhf.yj20258888.top

[S29] C：变参函数
来源：http://msb.feifeiyinyue.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mdm.jinqigufen.top

[S30] C：头文件保护
来源：http://jog.iojbl.cn

#ifndef X_H
来源：http://sjp.xinyue.icu

#define X_H
来源：http://ter.tarul.cn

#endif
来源：http://zfp.dianchejie.cn

[S31] C++：Hello World
来源：http://dfw.zhixingplan.top

#include <iostream>
来源：http://eeu.shanyushiyangkeji.top

int main() { std::cout << "Hello\n"; }
来源：http://gay.yfazqb.com

[S32] C++：字符串
来源：http://ekl.dianchejie.cn

std::string s = "hi";  s += "!";
来源：http://cfa.xingfuxueyuan.xyz

[S33] C++：vector 增删
来源：http://pij.jianghu66.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fgf.hywenlv.cn

[S34] C++：遍历 vector
来源：http://glc.jinqigufen.top

for (auto &x : v) { std::cout << x; }
来源：http://kwp.shanyushiyangtech.top

[S35] C++：map
来源：http://bzo.ywan-chungtsiang.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dtp.guowangkeji.top

[S36] C++：unordered_map
来源：http://mtx.uphjek.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bqx.uphjek.com

[S37] C++：set
来源：http://ifz.gotoacloud.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://agi.xylfe.cn

[S38] C++：排序
来源：http://qdc.zhijiandao.cn

std::sort(v.begin(), v.end());
来源：http://eau.nanxuanxn.top

[S39] C++：自定义比较器排序
来源：http://cjr.shangyingyoupin.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hoh.zhijiandao.cn

[S40] C++：查找元素
来源：http://cft.zdbjq.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ujr.fktsv.cn

[S41] C++：类与构造函数
来源：http://bov.chenjidiqi.icu

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ikm.xuanzx.com

[S42] C++：继承与虚函数
来源：http://rqr.daria6918.cn

class B : public Base { public: void f() override {} };
来源：http://xhm.jiagoushi.top

[S43] C++：智能指针
来源：http://ihh.fehbvm.com

auto p = std::make_unique<int>(5);
来源：http://cmq.yj202588.top

[S44] C++：引用传参
来源：http://fep.yj20258888.top

void inc(int &x) { ++x; }
来源：http://kxn.guowangkeji.top

[S45] C++：lambda
来源：http://ckl.aizwys.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zji.cashguo.top

[S46] C++：函数模板
来源：http://tti.zhaomingkeji.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lmu.havefunace.top

[S47] C++：结构化绑定遍历
来源：http://swb.jinyuanbaomall.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nyx.chenzaomai.com

[S48] C++：逐行读文件
来源：http://dql.kuanghao11.cn

std::ifstream in("a.txt");  std::string line;
来源：http://oeb.guowangkeji.top

while (std::getline(in, line)) { }
来源：http://ysq.shuidangran.top

[S49] C++：写文件
来源：http://asu.zdbjq.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xug.chenjidiqi.icu

[S50] C++：格式化数字
来源：http://thc.cashguo.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zbj.shzxlz.cn

[S51] C++：显式类型转换
来源：http://ufa.hcnkem.com

static_cast<double>(a) / b
来源：http://ize.yangfankeji.com

[S52] C++：const 与 noexcept
来源：http://csf.ybcxt.top

int size() const noexcept { return n_; }
来源：http://hel.svipenyu.cn

[S53] C++：移动语义
来源：http://uwp.birdmap.top

std::vector<int> w = std::move(v);
来源：http://sau.jinqigufen.top

[S54] C++：异常处理
来源：http://dgt.feifeiyinyue.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kwh.aibaodan.cn

[S55] C++：结构化绑定
来源：http://srl.shuidangran.top

auto [a, b] = std::make_pair(1, 2);
来源：http://dqz.c1oappe.top

[S56] C++：optional
来源：http://ooy.wangdashe.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ekk.ywan-chungtsiang.top

[S57] C++：编译期常量
来源：http://owt.xziqi.cn

constexpr int N = 10;
来源：http://asq.pengpengdd.cyou

[S58] C++：命名空间
来源：http://kgl.hongshengwenyu.top

namespace ns { int f() { return 1; } }
来源：http://tsu.ydzc1.top

[S59] C++：静态断言
来源：http://ewz.hammf.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bas.bjfxy.top

[S60] C++：遍历并删除元素
来源：http://xmt.jianghu66.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kqo.vehdjk.com

================================================================================
来源：http://jgq.haohaochexian.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jyy.gotoacloud.top

================================================================================
来源：http://ldw.epnwcf.com

[T01] Kotlin：Hello World
来源：http://lje.aibaodan.cn

println("Hello")
来源：http://azd.hfpthk.cn

[T02] Kotlin：变量
来源：http://ggn.yangfankeji.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rhg.gzhubu.top

[T03] Kotlin：字符串模板
来源：http://iny.feifeiyinyue.top

"值: $b"
来源：http://vhz.52xcode.cn

[T04] Kotlin：空安全
来源：http://quj.xziqi.cn

val n: String? = null;  n?.length
来源：http://yla.meibo888.top

[T05] Kotlin：when 表达式
来源：http://zqx.dianchejie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qsn.hesvh.cn

[T06] Kotlin：集合映射
来源：http://wdt.cheryme.top

listOf(1, 2, 3).map { it * 2 }
来源：http://pdt.ydjk.org.cn

[T07] Kotlin：集合过滤
来源：http://tum.bbcook.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://dop.jiagoushi.top

[T08] Kotlin：数据类
来源：http://ttf.shanyushiyangtech.top

data class User(val name: String, val age: Int)
来源：http://vap.wangshuangyany.cn

[T09] Kotlin：扩展函数
来源：http://hwc.ctjpmb.com

fun String.exclaim() = this + "!"
来源：http://ejo.nwbrower.top

[T10] Kotlin：默认参数
来源：http://tuk.shanyushiyangtech.top

fun greet(name: String = "World") = "Hi $name"
来源：http://tjy.yj20258.top

[T11] Kotlin：协程
来源：http://ghw.ivvv.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://sgw.fehbvm.com

[T12] Kotlin：解构声明
来源：http://orr.iojbl.cn

val (a, b) = Pair(1, 2)
来源：http://ntx.cashguo.top

[T13] Kotlin：只读 Map
来源：http://npi.fanxiaobao.xyz

val m = mapOf("a" to 1)
来源：http://cni.cqqwz.cn

[T14] Kotlin：循环
来源：http://kew.guannengcc.top

for (i in 1..10) println(i)
来源：http://ryr.zhixingplan.top

[T15] Kotlin：接口
来源：http://rsi.316326.xyz

interface Shape { fun area(): Double }
来源：http://jko.xinyue.icu

[T16] Swift：Hello World
来源：http://dyh.yuanzhike.top

print("Hello")
来源：http://kgd.jinghuilouyu.cn

[T17] Swift：变量与常量
来源：http://pxu.yj20258.top

var a = 1;  let b = 2
来源：http://qtt.zhixingplan.top

[T18] Swift：字符串插值
来源：http://ozv.sxryk.cn

"值: \(b)"
来源：http://guo.mhx1999.top

[T19] Swift：可选绑定
来源：http://xtt.chenjidiqi.icu

if let n = opt { print(n) }
来源：http://azq.xingfuxueyuan.xyz

[T20] Swift：数组操作
来源：http://tbj.pycfn.com

var a = [1, 2, 3];  a.append(4)
来源：http://izk.guannengcc.top

[T21] Swift：遍历
来源：http://elj.zycfv.cn

for x in a { print(x) }
来源：http://xjo.dianchejie.cn

[T22] Swift：字典
来源：http://abs.yj202588.top

var d = ["a": 1];  d["b"] = 2
来源：http://pkk.jqgufenzy.top

[T23] Swift：函数
来源：http://ddn.0kj1m.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://uia.ybcxt.top

[T24] Swift：闭包
来源：http://bpa.fengsongda.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://dkv.xuanzx.com

[T25] Swift：结构体
来源：http://qyx.yvedp.cn

struct P { var x: Int }
来源：http://iqz.meibo888.top

[T26] Swift：类与重写
来源：http://jdz.sjlbkw.cn

class A: Base { override func f() {} }
来源：http://ngl.jinqigufen.top

[T27] Swift：错误处理
来源：http://yye.ivvv.top

do { try f() } catch { print(error) }
来源：http://qnv.hongshengwenyu.top

[T28] Swift：枚举
来源：http://wsa.hongshengwenyu.top

enum Color { case red, green }
来源：http://wle.guannengcc.top

[T29] Swift：guard 提前返回
来源：http://djo.zhoulong.xyz

guard let x = opt else { return }
来源：http://zya.jlsjyb.cn

[T30] Swift：协议
来源：http://vfv.tian-w.cn

protocol Shape { func area() -> Double }
来源：http://oeu.yangfankeji.com

[T31] Lua：Hello World
来源：http://whf.yongpay.top

print("Hello")
来源：http://pcp.ehwqpu.com

[T32] Lua：局部变量
来源：http://fzb.kuanghao11.cn

local a = 1
来源：http://sjf.pengpengdd.cyou

[T33] Lua：表（数组）
来源：http://esf.daxiang520.top

local t = {1, 2, 3};  t[4] = 4
来源：http://trt.vqdsnc.cn

[T34] Lua：遍历表
来源：http://tki.hongshengwenyu.top

for i, v in ipairs(t) do print(i, v) end
来源：http://akt.haohaochexian.top

[T35] Lua：字典表
来源：http://tcl.xylfe.cn

local d = { a = 1 };  d.b = 2
来源：http://rag.daria6918.cn

[T36] Lua：函数
来源：http://jzg.epnwcf.com

function add(a, b) return a + b end
来源：http://wyx.daxiang520.top

[T37] Lua：字符串拼接
来源：http://ytw.ybcxt.top

"a" .. "b"
来源：http://pgt.zhongyouzk.top

[T38] Lua：条件
来源：http://rbu.iojbl.cn

if x > 0 then print("正") end
来源：http://mze.sweek.top

[T39] Lua：模式匹配
来源：http://sju.tianlin.xyz

string.find(s, "%d+")
来源：http://cex.zhaomingkeji.xyz

[T40] Lua：元表
来源：http://mgv.zdbjq.cn

setmetatable({}, { __index = base })
来源：http://dha.gogol.net.cn

[T41] Perl：Hello World
来源：http://zqc.sjlbkw.cn

print "Hello\n";
来源：http://dyi.snrcjt.cn

[T42] Perl：变量类型
来源：http://dzj.mhx1999.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cij.cdnleiting.top

[T43] Perl：字符串插值
来源：http://mtm.daxiang520.top

"值: $a"
来源：http://beb.vqdsnc.cn

[T44] Perl：条件
来源：http://vnt.vqdsnc.cn

if ($a > 0) { print "正"; }
来源：http://qmy.hnqzz.top

[T45] Perl：数组遍历
来源：http://vqr.vqdsnc.cn

for my $x (@arr) { print $x; }
来源：http://fxw.zdqjudy.top

[T46] Perl：哈希操作
来源：http://dol.tian-w.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pjd.svipenyu.cn

[T47] Perl：正则捕获
来源：http://uew.zdbjq.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ixr.gotoacloud.top

[T48] Perl：正则替换
来源：http://atw.sufxvd.cn

$s =~ s/old/new/g;
来源：http://xkx.chenzaomai.com

[T49] Perl：函数
来源：http://njp.jianghu66.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ish.aizwys.cn

[T50] Perl：逐行读文件
来源：http://bld.cheryme.top

open my $fh, "<", "a.txt" or die $!;
来源：http://bvt.redwolf501.top

while (my $line = <$fh>) { print $line; }
来源：http://veb.jyoumei.cn

[T51] Scala：Hello World
来源：http://akc.hcnkem.com

println("Hello")
来源：http://eno.cdnleiting.top

[T52] Scala：变量
来源：http://mtq.mhx1999.top

val a = 1;  var b = 2
来源：http://qpt.feifeiyinyue.top

[T53] Scala：字符串插值
来源：http://lau.ydjk.org.cn

s"值: $b"
来源：http://izw.fktsv.cn

[T54] Scala：集合映射
来源：http://qdb.kuanghao11.cn

List(1, 2, 3).map(_ * 2)
来源：http://gpp.epnwcf.com

[T55] Scala：集合过滤
来源：http://chd.xuanzx.com

List(1, 2, 3).filter(_ > 1)
来源：http://kgz.ivvv.top

[T56] Scala：样例类
来源：http://iqi.yueranfly.top

case class User(name: String, age: Int)
来源：http://xyi.uphjek.com

[T57] Scala：模式匹配
来源：http://veu.yvedp.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ojw.yangfankeji.com

[T58] Scala：函数定义
来源：http://aoi.0kj1m.cn

def add(a: Int, b: Int): Int = a + b
来源：http://lcj.cashguo.top

[T59] Scala：循环
来源：http://oyb.shzxlz.cn

for (i <- 1 to 10) println(i)
来源：http://nqa.wangshuangyany.cn

[T60] Scala：折叠
来源：http://wnx.ppjwa.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://muk.jinqigufen.top

================================================================================
来源：http://twd.pycfn.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xnd.andypj.xyz

================================================================================
来源：http://bsx.yvedp.cn

[U01] Py：创建虚拟环境
来源：http://hjx.wangdashe.top

python -m venv .venv && source .venv/bin/activate
来源：http://jfc.haohaochexian.top

[U02] Py：导出 / 安装依赖
来源：http://ruu.aibaodan.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ukf.dianchejie.cn

[U03] Py：加载 .env 配置
来源：http://vgp.zhaomingkeji.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://jvs.birdmap.top

[U04] Py：变量调试打印
来源：http://jnj.yfazqb.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://adj.cdnleiting.top

[U05] Py：列表去重且保序
来源：http://onn.wangdashe.top

list(dict.fromkeys(arr))
来源：http://beg.bbcook.cn

[U06] Py：合并两个字典
来源：http://tjl.316326.xyz

{**a, **b}
来源：http://nlm.zhixingplan.top


<!-- 参考信息 -->