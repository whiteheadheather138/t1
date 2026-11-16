代发 wailian999

openssl rand -hex 16
来源：http://jrq.chenzaomai.com

[R68] 计算文件校验值
来源：http://orf.chenjidiqi.icu

sha256sum a.txt;  md5sum a.txt
来源：http://fdo.nanxuanxn.top

[R69] 生成随机密码
来源：http://nbg.shuidangran.top

head -c 16 /dev/urandom | base64
来源：http://ois.hfpthk.cn

[R70] 时间戳与互转
来源：http://ujy.xingfuxueyuan.xyz

date +%s;  date -d @1700000000
来源：http://xjn.yuxming.cn

[R71] 日期格式化
来源：http://vkx.hywenlv.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zwa.ivvv.top

[R72] 等待端口就绪
来源：http://vqk.birdmap.top

until nc -z localhost 3306; do sleep 1; done
来源：http://joy.aizwys.cn

[R73] 分割大日志
来源：http://edo.tarul.cn

split -l 1000 big.log part_
来源：http://qso.dashuyun.cn

[R74] 批量重命名
来源：http://nxn.yongpay.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ofk.chenlongwang.top

[R75] 导出环境变量
来源：http://gvw.chenlongwang.top

export PATH="$HOME/bin:$PATH"
来源：http://ulf.havefunace.top

[R76] 使用临时文件
来源：http://lom.hfpthk.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zen.shanyushiyangkeji.top

[R77] 读取用户输入
来源：http://pjp.ehwqpu.com

read -rp "请输入: " ans
来源：http://jdy.shanyushiyangtech.top

[R78] 交互式菜单
来源：http://jah.zycfv.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://wqp.ydzc1.top

[R79] 解析命令行选项
来源：http://xnj.hammf.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pjq.xylfe.cn

[R80] 查看脚本执行耗时
来源：http://glf.yuanzhike.top

time ./run.sh
来源：http://puz.shuidangran.top

================================================================================
来源：http://ove.hnxiangtu.top

S. C / C++ 专题
来源：http://sbj.fzhhl.top

================================================================================
来源：http://mlc.hnqzz.top

[S01] C：Hello World
来源：http://eej.hcnkem.com

#include <stdio.h>
来源：http://udh.meibo888.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://plf.shangyingyoupin.top

[S02] C：变量与格式化输出
来源：http://pzy.yonumen.top

int a = 10; printf("%d\n", a);
来源：http://byf.yongpay.top

[S03] C：读入整数
来源：http://rbs.fengsongda.top

int x; scanf("%d", &x);
来源：http://cdt.hysaishi.cn

[S04] C：字符串复制
来源：http://heu.guannengcc.top

char dst[32]; strcpy(dst, "hi");
来源：http://meh.bbcook.cn

[S05] C：字符串长度
来源：http://pbm.cheryme.top

strlen(s)
来源：http://zdl.hfpthk.cn

[S06] C：字符串比较
来源：http://dpk.xinyue.icu

strcmp(a, b) == 0
来源：http://xez.guannengcc.top

[S07] C：数组遍历求和
来源：http://zzc.sxryk.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xrp.shanyushiyangkeji.top

[S08] C：动态内存分配与释放
来源：http://asv.jlsjyb.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hwf.52xcode.cn

[S09] C：结构体定义与初始化
来源：http://kfq.andypj.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://svg.zhongyouzk.top

[S10] C：指针与解引用
来源：http://kmt.hongshengwenyu.top

int *p = &a;  *p = 5;
来源：http://htd.andypj.xyz

[S11] C：逐行读文件
来源：http://dja.xylfe.cn

FILE *f = fopen("a.txt", "r");
来源：http://skm.uphjek.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://adx.yfazqb.com

fclose(f);
来源：http://qld.ivvv.top

[S12] C：写文件
来源：http://rdx.cdnleiting.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vdq.birdmap.top

[S13] C：宏定义
来源：http://mvl.aibaodan.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vtc.smart0.xyz

[S14] C：枚举
来源：http://nyh.xuanzx.com

enum Color { RED, GREEN, BLUE };
来源：http://ghq.zhoulong.xyz

[S15] C：类型转换
来源：http://gtj.fktsv.cn

(double) a / b
来源：http://efn.hnxiangtu.top

[S16] C：位操作置位
来源：http://lwx.wangshuangyany.cn

x |= (1 << 3);
来源：http://cez.hnqzz.top

[S17] C：安全拼接字符串
来源：http://nat.zhengqikj.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wuf.ppjwa.cn

[S18] C：命令行参数
来源：http://grr.dashuyun.cn

int main(int argc, char **argv)
来源：http://usn.zycfv.cn

[S19] C：快速排序
来源：http://cov.ydzc1.top

qsort(a, n, sizeof(int), cmp);
来源：http://mas.yonumen.top

[S20] C：二分查找
来源：http://vyn.gotoacloud.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ptk.xuanzx.com

[S21] C：字符类别判断
来源：http://yse.chenjidiqi.icu

isdigit(c);  isalpha(c);  isspace(c);
来源：http://uvh.sufxvd.cn

[S22] C：字符串转数字
来源：http://gip.jinghuilouyu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ugj.zhongyouzk.top

[S23] C：随机数
来源：http://jcz.ehwqpu.com

srand(time(NULL));  int r = rand() % 100;
来源：http://xyg.hysaishi.cn

[S24] C：获取本地时间
来源：http://hhz.feifeiyinyue.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sgx.zhoulong.xyz

[S25] C：内存拷贝
来源：http://enz.tianlin.xyz

memcpy(dst, src, n);
来源：http://jgl.shuidangran.top

[S26] C：内存清零
来源：http://ltl.zdqjudy.top

memset(a, 0, sizeof a);
来源：http://lpl.dashuyun.cn

[S27] C：定义常量
来源：http://sbs.xuetiantiany.cn

const double PI = 3.14159;
来源：http://mnr.hnxiangtu.top

[S28] C：静态变量
来源：http://nde.smart0.xyz

static int counter = 0;
来源：http://bvd.nwbrower.top

[S29] C：变参函数
来源：http://hoa.jinqigufen.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://iqh.meibo888.top

[S30] C：头文件保护
来源：http://ivj.xuetiantiany.cn

#ifndef X_H
来源：http://ucx.zhiwuduotai.top

#define X_H
来源：http://ojh.pycfn.com

#endif
来源：http://oru.fanxiaobao.xyz

[S31] C++：Hello World
来源：http://wby.ppjwa.cn

#include <iostream>
来源：http://vwl.cqqwz.cn

int main() { std::cout << "Hello\n"; }
来源：http://mvi.zdbjq.cn

[S32] C++：字符串
来源：http://vld.xziqi.cn

std::string s = "hi";  s += "!";
来源：http://fly.pycfn.com

[S33] C++：vector 增删
来源：http://kcv.yueranfly.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wpr.svipenyu.cn

[S34] C++：遍历 vector
来源：http://ocr.hnqzz.top

for (auto &x : v) { std::cout << x; }
来源：http://fnp.fktsv.cn

[S35] C++：map
来源：http://uxq.vehdjk.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fgm.zycfv.cn

[S36] C++：unordered_map
来源：http://bhy.jinqigufen.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tjc.xinyue.icu

[S37] C++：set
来源：http://kqi.zhiwuduotai.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vie.yuanzhike.top

[S38] C++：排序
来源：http://hfd.hongshengwenyu.top

std::sort(v.begin(), v.end());
来源：http://ntd.haohaochexian.top

[S39] C++：自定义比较器排序
来源：http://wrz.yueranfly.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xzy.zhengqikj.top

[S40] C++：查找元素
来源：http://gia.sjlbkw.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fwf.gogol.net.cn

[S41] C++：类与构造函数
来源：http://hxl.316326.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fov.jqgfzy.top

[S42] C++：继承与虚函数
来源：http://wzh.daxiang520.top

class B : public Base { public: void f() override {} };
来源：http://jre.fktsv.cn

[S43] C++：智能指针
来源：http://hka.shangyingyoupin.top

auto p = std::make_unique<int>(5);
来源：http://cgs.hnqzz.top

[S44] C++：引用传参
来源：http://bwk.tanke756.top

void inc(int &x) { ++x; }
来源：http://dpv.ydjk.org.cn

[S45] C++：lambda
来源：http://yjw.iojbl.cn

auto add = [](int a, int b) { return a + b; };
来源：http://pyq.fehbvm.com

[S46] C++：函数模板
来源：http://drh.aizwys.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ycj.pengpengdd.cyou

[S47] C++：结构化绑定遍历
来源：http://amv.daria6918.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://exs.aizwys.cn

[S48] C++：逐行读文件
来源：http://wsy.xinyue.icu

std::ifstream in("a.txt");  std::string line;
来源：http://nkl.gaohongyu789.top

while (std::getline(in, line)) { }
来源：http://xlo.sxryk.cn

[S49] C++：写文件
来源：http://okh.yvedp.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xso.nanxuanxn.top

[S50] C++：格式化数字
来源：http://jtd.ydjk.org.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zpv.vehdjk.com

[S51] C++：显式类型转换
来源：http://hxv.tanke756.top

static_cast<double>(a) / b
来源：http://ckb.sjlbkw.cn

[S52] C++：const 与 noexcept
来源：http://hlm.nanxinkj.top

int size() const noexcept { return n_; }
来源：http://nij.jianghu66.top

[S53] C++：移动语义
来源：http://sjj.sjlbkw.cn

std::vector<int> w = std::move(v);
来源：http://tom.feifeiyinyue.top

[S54] C++：异常处理
来源：http://sgr.tanke756.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://djo.zhiwuduotai.top

[S55] C++：结构化绑定
来源：http://dfb.andypj.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://wlf.tanke756.top

[S56] C++：optional
来源：http://phi.vqdsnc.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://iic.hcnkem.com

[S57] C++：编译期常量
来源：http://lwt.redwolf501.top

constexpr int N = 10;
来源：http://nqa.aizwys.cn

[S58] C++：命名空间
来源：http://jrk.nanxuanxn.top

namespace ns { int f() { return 1; } }
来源：http://ccn.cucudq.cn

[S59] C++：静态断言
来源：http://amf.snrcjt.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fih.redwolf501.top

[S60] C++：遍历并删除元素
来源：http://yob.yanxiufei.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fep.yongpay.top

================================================================================
来源：http://qyw.cashguo.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xpu.zhijiandao.cn

================================================================================
来源：http://fua.nwbrower.top

[T01] Kotlin：Hello World
来源：http://fes.zycfv.cn

println("Hello")
来源：http://sar.fengsongda.top

[T02] Kotlin：变量
来源：http://gfv.fktsv.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bti.shuidangran.top

[T03] Kotlin：字符串模板
来源：http://yij.jiagoushi.top

"值: $b"
来源：http://tgu.hysaishi.cn

[T04] Kotlin：空安全
来源：http://zgg.hywenlv.cn

val n: String? = null;  n?.length
来源：http://zke.sufxvd.cn

[T05] Kotlin：when 表达式
来源：http://zee.bjfxy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hhh.meibo888.top

[T06] Kotlin：集合映射
来源：http://jib.hywenlv.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://jrs.zdbjq.cn

[T07] Kotlin：集合过滤
来源：http://ivm.nanxuanxn.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://niu.zhiwuduotai.top

[T08] Kotlin：数据类
来源：http://ejk.shuidangran.top

data class User(val name: String, val age: Int)
来源：http://tqp.jinqigfzy.top

[T09] Kotlin：扩展函数
来源：http://ijn.cheryme.top

fun String.exclaim() = this + "!"
来源：http://vba.ywan-chungtsiang.top

[T10] Kotlin：默认参数
来源：http://idf.zhijiandao.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://xjt.zhixingplan.top

[T11] Kotlin：协程
来源：http://rvc.kuanghao11.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bac.meibo888.top

[T12] Kotlin：解构声明
来源：http://iis.havefunace.top

val (a, b) = Pair(1, 2)
来源：http://xfl.pengpengdd.cyou

[T13] Kotlin：只读 Map
来源：http://wlg.ydzc1.top

val m = mapOf("a" to 1)
来源：http://fye.nwbrower.top

[T14] Kotlin：循环
来源：http://cgy.andypj.xyz

for (i in 1..10) println(i)
来源：http://clb.zhengqikj.top

[T15] Kotlin：接口
来源：http://pdi.yfazqb.com

interface Shape { fun area(): Double }
来源：http://gpe.zhijiandao.cn

[T16] Swift：Hello World
来源：http://zdg.meibo888.top

print("Hello")
来源：http://jsd.hcnkem.com

[T17] Swift：变量与常量
来源：http://wto.snrcjt.cn

var a = 1;  let b = 2
来源：http://ojm.jianghu66.top

[T18] Swift：字符串插值
来源：http://gjw.fehbvm.com

"值: \(b)"
来源：http://riv.pengpengdd.cyou

[T19] Swift：可选绑定
来源：http://juz.zycfv.cn

if let n = opt { print(n) }
来源：http://gen.dashuyun.cn

[T20] Swift：数组操作
来源：http://btr.zdqjudy.top

var a = [1, 2, 3];  a.append(4)
来源：http://gkx.hnxiangtu.top

[T21] Swift：遍历
来源：http://oot.yangfankeji.com

for x in a { print(x) }
来源：http://imb.9152youxi.cn

[T22] Swift：字典
来源：http://nht.sufxvd.cn

var d = ["a": 1];  d["b"] = 2
来源：http://kow.zhijiandao.cn

[T23] Swift：函数
来源：http://rem.hnxiangtu.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tun.daxiang520.top

[T24] Swift：闭包
来源：http://zmp.gotoacloud.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://sdy.ivvv.top

[T25] Swift：结构体
来源：http://zwa.sufxvd.cn

struct P { var x: Int }
来源：http://hmx.hnxiangtu.top

[T26] Swift：类与重写
来源：http://yhj.hnxiangtu.top

class A: Base { override func f() {} }
来源：http://xoj.xziqi.cn

[T27] Swift：错误处理
来源：http://zjb.birdmap.top

do { try f() } catch { print(error) }
来源：http://kyc.shzxlz.cn

[T28] Swift：枚举
来源：http://fsb.fanxiaobao.xyz

enum Color { case red, green }
来源：http://ydq.zhixingplan.top

[T29] Swift：guard 提前返回
来源：http://ytx.vqdsnc.cn

guard let x = opt else { return }
来源：http://zpb.sxryk.cn

[T30] Swift：协议
来源：http://azh.jianghu66.top

protocol Shape { func area() -> Double }
来源：http://hrp.pycfn.com

[T31] Lua：Hello World
来源：http://fvk.andypj.xyz

print("Hello")
来源：http://hno.mhx1999.top

[T32] Lua：局部变量
来源：http://bmi.zycfv.cn

local a = 1
来源：http://kvz.hfpthk.cn

[T33] Lua：表（数组）
来源：http://fro.pycfn.com

local t = {1, 2, 3};  t[4] = 4
来源：http://wup.316326.xyz

[T34] Lua：遍历表
来源：http://vdl.sysykeji.top

for i, v in ipairs(t) do print(i, v) end
来源：http://bcm.havefunace.top

[T35] Lua：字典表
来源：http://che.iojbl.cn

local d = { a = 1 };  d.b = 2
来源：http://drk.ppjwa.cn

[T36] Lua：函数
来源：http://tjt.zhongyouzk.top

function add(a, b) return a + b end
来源：http://zwn.aibaodan.cn

[T37] Lua：字符串拼接
来源：http://sfg.hfpthk.cn

"a" .. "b"
来源：http://kpe.cdnleiting.top

[T38] Lua：条件
来源：http://gmi.tanke756.top

if x > 0 then print("正") end
来源：http://rjn.quarkkingdee.top

[T39] Lua：模式匹配
来源：http://uav.yuxming.cn

string.find(s, "%d+")
来源：http://gyo.xinyue.icu

[T40] Lua：元表
来源：http://bzx.shzxlz.cn

setmetatable({}, { __index = base })
来源：http://byv.ybcxt.top

[T41] Perl：Hello World
来源：http://ckw.aizwys.cn

print "Hello\n";
来源：http://uvu.mhx1999.top

[T42] Perl：变量类型
来源：http://enj.quarkkingdee.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tup.aibaodan.cn

[T43] Perl：字符串插值
来源：http://vxl.gzhubu.top

"值: $a"
来源：http://nsx.shangyingyoupin.top

[T44] Perl：条件
来源：http://rbe.epnwcf.com

if ($a > 0) { print "正"; }
来源：http://gyw.jyoumei.cn

[T45] Perl：数组遍历
来源：http://dkz.sxryk.cn

for my $x (@arr) { print $x; }
来源：http://cgd.vqdsnc.cn

[T46] Perl：哈希操作
来源：http://cak.zhixingplan.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ban.vehdjk.com

[T47] Perl：正则捕获
来源：http://ide.mhx1999.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://lvr.316326.xyz

[T48] Perl：正则替换
来源：http://aei.feifeiyinyue.top

$s =~ s/old/new/g;
来源：http://xii.c1oappe.top

[T49] Perl：函数
来源：http://gce.yongpay.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cvr.dianchejie.cn

[T50] Perl：逐行读文件
来源：http://aos.yangfankeji.com

open my $fh, "<", "a.txt" or die $!;
来源：http://ftw.shanyushiyangkeji.top

while (my $line = <$fh>) { print $line; }
来源：http://wob.zhoulong.xyz

[T51] Scala：Hello World
来源：http://jju.dashuyun.cn

println("Hello")
来源：http://syz.zdbjq.cn

[T52] Scala：变量
来源：http://npg.yj20258.top

val a = 1;  var b = 2
来源：http://fdr.birdmap.top

[T53] Scala：字符串插值
来源：http://mls.ydjk.org.cn

s"值: $b"
来源：http://ykx.quarkkingdee.top

[T54] Scala：集合映射
来源：http://tva.hysaishi.cn

List(1, 2, 3).map(_ * 2)
来源：http://vfy.hysaishi.cn

[T55] Scala：集合过滤
来源：http://nvv.ppjwa.cn

List(1, 2, 3).filter(_ > 1)
来源：http://raq.daxiang520.top

[T56] Scala：样例类
来源：http://iye.shzxlz.cn

case class User(name: String, age: Int)
来源：http://giw.yonumen.top

[T57] Scala：模式匹配
来源：http://snn.shanyushiyangtech.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://lov.jianghu66.top

[T58] Scala：函数定义
来源：http://wmz.shuidangran.top

def add(a: Int, b: Int): Int = a + b
来源：http://vrj.52xcode.cn

[T59] Scala：循环
来源：http://apz.snrcjt.cn

for (i <- 1 to 10) println(i)
来源：http://nyx.jqgufenzy.top

[T60] Scala：折叠
来源：http://kyg.snrcjt.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tcq.xuetiantiany.cn

================================================================================
来源：http://chn.snrcjt.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pdh.snrcjt.cn

================================================================================
来源：http://buv.daxiang520.top

[U01] Py：创建虚拟环境
来源：http://vtn.shzxlz.cn

python -m venv .venv && source .venv/bin/activate
来源：http://prg.iojbl.cn

[U02] Py：导出 / 安装依赖
来源：http://kex.jlsjyb.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://oyd.gotoacloud.top

[U03] Py：加载 .env 配置
来源：http://joz.shanyushiyangtech.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ffj.quarkkingdee.top

[U04] Py：变量调试打印
来源：http://eqf.guannengcc.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hay.uphjek.com

[U05] Py：列表去重且保序
来源：http://ntf.xuetiantiany.cn

list(dict.fromkeys(arr))
来源：http://gxp.cqqwz.cn

[U06] Py：合并两个字典
来源：http://rub.sysykeji.top

{**a, **b}
来源：http://eju.uphjek.com

[U07] Py：反转字典键值
来源：http://ejl.fzhhl.top

{v: k for k, v in d.items()}
来源：http://dho.c1oappe.top

[U08] Py：展平二维列表
来源：http://avg.fanxiaobao.xyz

[y for x in nested for y in x]
来源：http://tix.daxiang520.top


<!-- 参考信息 -->