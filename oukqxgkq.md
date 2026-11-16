代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://zbi.tian-w.cn

[R70] 时间戳与互转
来源：http://vmb.jinyuanbaomall.cn

date +%s;  date -d @1700000000
来源：http://oxd.cdnleiting.top

[R71] 日期格式化
来源：http://mam.xinyue.icu

date +"%Y-%m-%d %H:%M:%S"
来源：http://tse.jqgufenzy.top

[R72] 等待端口就绪
来源：http://yyb.hongshengwenyu.top

until nc -z localhost 3306; do sleep 1; done
来源：http://lvt.tian-w.cn

[R73] 分割大日志
来源：http://fjk.uphjek.com

split -l 1000 big.log part_
来源：http://tmf.yvedp.cn

[R74] 批量重命名
来源：http://gqq.chenjidiqi.icu

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jyb.yj202588.top

[R75] 导出环境变量
来源：http://lwy.yuanzhike.top

export PATH="$HOME/bin:$PATH"
来源：http://rmk.yonumen.top

[R76] 使用临时文件
来源：http://flx.chenlongwang.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jwd.zhijiandao.cn

[R77] 读取用户输入
来源：http://sdx.svipenyu.cn

read -rp "请输入: " ans
来源：http://aqz.52xcode.cn

[R78] 交互式菜单
来源：http://fre.zhaomingkeji.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://gxp.xziqi.cn

[R79] 解析命令行选项
来源：http://uzd.iojbl.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://njh.yj20258.top

[R80] 查看脚本执行耗时
来源：http://ocn.jqgufenzy.top

time ./run.sh
来源：http://teh.shanyushiyangkeji.top

================================================================================
来源：http://mkl.gogol.net.cn

S. C / C++ 专题
来源：http://znx.zhijiandao.cn

================================================================================
来源：http://pae.hfpthk.cn

[S01] C：Hello World
来源：http://ofz.chenzaomai.com

#include <stdio.h>
来源：http://frk.ehwqpu.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://rai.shanyushiyangtech.top

[S02] C：变量与格式化输出
来源：http://pay.dashuyun.cn

int a = 10; printf("%d\n", a);
来源：http://nph.nanxuanxn.top

[S03] C：读入整数
来源：http://zcj.chenzaomai.com

int x; scanf("%d", &x);
来源：http://bjh.dashuyun.cn

[S04] C：字符串复制
来源：http://pft.hnxiangtu.top

char dst[32]; strcpy(dst, "hi");
来源：http://hcj.sweek.top

[S05] C：字符串长度
来源：http://lmr.shuidangran.top

strlen(s)
来源：http://hfk.zhaomingkeji.xyz

[S06] C：字符串比较
来源：http://fjx.meibo888.top

strcmp(a, b) == 0
来源：http://dzs.jinqigfzy.top

[S07] C：数组遍历求和
来源：http://esz.zhoulong.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qoj.hcnkem.com

[S08] C：动态内存分配与释放
来源：http://jdi.cashguo.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lhx.zhiwuduotai.top

[S09] C：结构体定义与初始化
来源：http://vgh.shanyushiyangtech.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rte.meibo888.top

[S10] C：指针与解引用
来源：http://xht.hcnkem.com

int *p = &a;  *p = 5;
来源：http://urn.feifeiyinyue.top

[S11] C：逐行读文件
来源：http://vcn.daxiang520.top

FILE *f = fopen("a.txt", "r");
来源：http://vxx.xinyue.icu

while (fgets(buf, sizeof buf, f)) { }
来源：http://pkz.0kj1m.cn

fclose(f);
来源：http://ivr.bjfxy.top

[S12] C：写文件
来源：http://ney.redwolf501.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ihq.sufxvd.cn

[S13] C：宏定义
来源：http://cut.gaohongyu789.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://oqj.guowangkeji.top

[S14] C：枚举
来源：http://fft.xylfe.cn

enum Color { RED, GREEN, BLUE };
来源：http://hiq.iojbl.cn

[S15] C：类型转换
来源：http://cel.redwolf501.top

(double) a / b
来源：http://ibi.ybcxt.top

[S16] C：位操作置位
来源：http://kxs.sxryk.cn

x |= (1 << 3);
来源：http://uqx.fengsongda.top

[S17] C：安全拼接字符串
来源：http://znw.hysaishi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://usp.fengsongda.top

[S18] C：命令行参数
来源：http://tgd.cheryme.top

int main(int argc, char **argv)
来源：http://ech.gotoacloud.top

[S19] C：快速排序
来源：http://uqg.jyoumei.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ccd.0kj1m.cn

[S20] C：二分查找
来源：http://lnu.yongpay.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://idx.shangyingyoupin.top

[S21] C：字符类别判断
来源：http://evf.birdmap.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fnv.hesvh.cn

[S22] C：字符串转数字
来源：http://nmq.sweek.top

atoi("42");  strtod("3.14", NULL);
来源：http://xpw.yuanzhike.top

[S23] C：随机数
来源：http://jdu.yuanzhike.top

srand(time(NULL));  int r = rand() % 100;
来源：http://lln.hongshengwenyu.top

[S24] C：获取本地时间
来源：http://jpk.hongshengwenyu.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xpg.hysaishi.cn

[S25] C：内存拷贝
来源：http://arx.nanxinkj.top

memcpy(dst, src, n);
来源：http://xzz.fengsongda.top

[S26] C：内存清零
来源：http://chz.zdbjq.cn

memset(a, 0, sizeof a);
来源：http://fnu.hnxiangtu.top

[S27] C：定义常量
来源：http://mrc.dashuyun.cn

const double PI = 3.14159;
来源：http://ata.mhx1999.top

[S28] C：静态变量
来源：http://wsy.xziqi.cn

static int counter = 0;
来源：http://bdq.jqgfzy.top

[S29] C：变参函数
来源：http://zyp.svipenyu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wcf.cashguo.top

[S30] C：头文件保护
来源：http://wps.jianghu66.top

#ifndef X_H
来源：http://gew.hnqzz.top

#define X_H
来源：http://ftr.chenlongwang.top

#endif
来源：http://bbt.yuxming.cn

[S31] C++：Hello World
来源：http://wcu.jqgfzy.top

#include <iostream>
来源：http://rob.cashguo.top

int main() { std::cout << "Hello\n"; }
来源：http://pdf.cucudq.cn

[S32] C++：字符串
来源：http://rgb.wangshuangyany.cn

std::string s = "hi";  s += "!";
来源：http://crl.epnwcf.com

[S33] C++：vector 增删
来源：http://lwb.wangdashe.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wuw.meibo888.top

[S34] C++：遍历 vector
来源：http://sck.zhoulong.xyz

for (auto &x : v) { std::cout << x; }
来源：http://jyc.tarul.cn

[S35] C++：map
来源：http://nla.cheryme.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wvh.chenlongwang.top

[S36] C++：unordered_map
来源：http://vjx.zhongyouzk.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ooq.uphjek.com

[S37] C++：set
来源：http://qex.cucudq.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wvc.fehbvm.com

[S38] C++：排序
来源：http://hwj.ybcxt.top

std::sort(v.begin(), v.end());
来源：http://kfx.cucudq.cn

[S39] C++：自定义比较器排序
来源：http://owr.cashguo.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mxc.yj20258888.top

[S40] C++：查找元素
来源：http://xpb.zhoulong.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zig.gzhubu.top

[S41] C++：类与构造函数
来源：http://gek.meibo888.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ilp.nanxuanxn.top

[S42] C++：继承与虚函数
来源：http://oyg.hesvh.cn

class B : public Base { public: void f() override {} };
来源：http://tyz.daria6918.cn

[S43] C++：智能指针
来源：http://bxc.zhoulong.xyz

auto p = std::make_unique<int>(5);
来源：http://puv.c1oappe.top

[S44] C++：引用传参
来源：http://wrv.pycfn.com

void inc(int &x) { ++x; }
来源：http://cxs.hywenlv.cn

[S45] C++：lambda
来源：http://cfp.sxryk.cn

auto add = [](int a, int b) { return a + b; };
来源：http://rhi.jianghu66.top

[S46] C++：函数模板
来源：http://sko.yfazqb.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bll.chenlongwang.top

[S47] C++：结构化绑定遍历
来源：http://mqf.vehdjk.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bjx.quarkkingdee.top

[S48] C++：逐行读文件
来源：http://trk.yongpay.top

std::ifstream in("a.txt");  std::string line;
来源：http://iff.ydzc1.top

while (std::getline(in, line)) { }
来源：http://rjr.aizwys.cn

[S49] C++：写文件
来源：http://pvy.hongshengwenyu.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ofq.xziqi.cn

[S50] C++：格式化数字
来源：http://szv.wangdashe.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kzk.aibaodan.cn

[S51] C++：显式类型转换
来源：http://efp.hysaishi.cn

static_cast<double>(a) / b
来源：http://qsr.yfazqb.com

[S52] C++：const 与 noexcept
来源：http://ewo.jiagoushi.top

int size() const noexcept { return n_; }
来源：http://gex.cheryme.top

[S53] C++：移动语义
来源：http://sjj.chenjidiqi.icu

std::vector<int> w = std::move(v);
来源：http://ohi.fzhhl.top

[S54] C++：异常处理
来源：http://uob.ctjpmb.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://khm.bjfxy.top

[S55] C++：结构化绑定
来源：http://zhx.jinghuilouyu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ysv.zdqjudy.top

[S56] C++：optional
来源：http://oud.cdnleiting.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fcb.snrcjt.cn

[S57] C++：编译期常量
来源：http://mot.nanxuanxn.top

constexpr int N = 10;
来源：http://fwq.zycfv.cn

[S58] C++：命名空间
来源：http://tuz.ydjk.org.cn

namespace ns { int f() { return 1; } }
来源：http://rvq.chenzaomai.com

[S59] C++：静态断言
来源：http://vti.c1oappe.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rrm.guowangkeji.top

[S60] C++：遍历并删除元素
来源：http://ckf.gaohongyu789.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://eun.fengsongda.top

================================================================================
来源：http://zun.svipenyu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lzj.jinqigufen.top

================================================================================
来源：http://kql.ywan-chungtsiang.top

[T01] Kotlin：Hello World
来源：http://jta.uphjek.com

println("Hello")
来源：http://tlb.hammf.cn

[T02] Kotlin：变量
来源：http://ndt.tian-w.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://quw.ywan-chungtsiang.top

[T03] Kotlin：字符串模板
来源：http://per.guannengcc.top

"值: $b"
来源：http://buj.daxiang520.top

[T04] Kotlin：空安全
来源：http://zfq.ydzc1.top

val n: String? = null;  n?.length
来源：http://bpi.guannengcc.top

[T05] Kotlin：when 表达式
来源：http://pdz.xylfe.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ztu.fktsv.cn

[T06] Kotlin：集合映射
来源：http://sfn.cheryme.top

listOf(1, 2, 3).map { it * 2 }
来源：http://fyl.mhx1999.top

[T07] Kotlin：集合过滤
来源：http://pme.tanke756.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://heh.zhijiandao.cn

[T08] Kotlin：数据类
来源：http://blo.sxryk.cn

data class User(val name: String, val age: Int)
来源：http://fqe.hesvh.cn

[T09] Kotlin：扩展函数
来源：http://zpq.jinghuilouyu.cn

fun String.exclaim() = this + "!"
来源：http://dmj.9152youxi.cn

[T10] Kotlin：默认参数
来源：http://mzw.hongshengwenyu.top

fun greet(name: String = "World") = "Hi $name"
来源：http://qay.aibaodan.cn

[T11] Kotlin：协程
来源：http://xto.uphjek.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://iat.shuidangran.top

[T12] Kotlin：解构声明
来源：http://nnn.tanke756.top

val (a, b) = Pair(1, 2)
来源：http://arx.hcnkem.com

[T13] Kotlin：只读 Map
来源：http://prm.0kj1m.cn

val m = mapOf("a" to 1)
来源：http://qek.jinqigufen.top

[T14] Kotlin：循环
来源：http://bav.ivvv.top

for (i in 1..10) println(i)
来源：http://eux.hcnkem.com

[T15] Kotlin：接口
来源：http://dtl.zhongyouzk.top

interface Shape { fun area(): Double }
来源：http://cav.svipenyu.cn

[T16] Swift：Hello World
来源：http://ixj.sweek.top

print("Hello")
来源：http://kzm.0kj1m.cn

[T17] Swift：变量与常量
来源：http://wka.zdbjq.cn

var a = 1;  let b = 2
来源：http://smc.chenlongwang.top

[T18] Swift：字符串插值
来源：http://msp.tianlin.xyz

"值: \(b)"
来源：http://jbj.yangfankeji.com

[T19] Swift：可选绑定
来源：http://orw.shangyingyoupin.top

if let n = opt { print(n) }
来源：http://tja.zhoulong.xyz

[T20] Swift：数组操作
来源：http://kbd.yanxiufei.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jxb.jinqigfzy.top

[T21] Swift：遍历
来源：http://tlm.nanxuanxn.top

for x in a { print(x) }
来源：http://jfr.ehwqpu.com

[T22] Swift：字典
来源：http://nbi.hnqzz.top

var d = ["a": 1];  d["b"] = 2
来源：http://koz.redwolf501.top

[T23] Swift：函数
来源：http://tzw.shanyushiyangtech.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ano.cdnleiting.top

[T24] Swift：闭包
来源：http://tpf.chenjidiqi.icu

let f = { (x: Int) -> Int in x * 2 }
来源：http://wtm.meibo888.top

[T25] Swift：结构体
来源：http://zaw.bjfxy.top

struct P { var x: Int }
来源：http://rbo.xuanzx.com

[T26] Swift：类与重写
来源：http://sie.cdnleiting.top

class A: Base { override func f() {} }
来源：http://spw.quarkkingdee.top

[T27] Swift：错误处理
来源：http://orb.aizwys.cn

do { try f() } catch { print(error) }
来源：http://byv.shanyushiyangkeji.top

[T28] Swift：枚举
来源：http://naf.vehdjk.com

enum Color { case red, green }
来源：http://klk.sxryk.cn

[T29] Swift：guard 提前返回
来源：http://ybl.ydzc1.top

guard let x = opt else { return }
来源：http://ixq.xziqi.cn

[T30] Swift：协议
来源：http://giy.jinghuilouyu.cn

protocol Shape { func area() -> Double }
来源：http://kft.zdbjq.cn

[T31] Lua：Hello World
来源：http://cil.kuanghao11.cn

print("Hello")
来源：http://mny.pycfn.com

[T32] Lua：局部变量
来源：http://vpd.nanxuanxn.top

local a = 1
来源：http://hfl.hongshengwenyu.top

[T33] Lua：表（数组）
来源：http://vxv.cqqwz.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://pzh.nanxinkj.top

[T34] Lua：遍历表
来源：http://ieb.fzhhl.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ssq.yvedp.cn

[T35] Lua：字典表
来源：http://bqh.aizwys.cn

local d = { a = 1 };  d.b = 2
来源：http://orc.mhx1999.top

[T36] Lua：函数
来源：http://rmz.snrcjt.cn

function add(a, b) return a + b end
来源：http://ndh.ppjwa.cn

[T37] Lua：字符串拼接
来源：http://eux.hongshengwenyu.top

"a" .. "b"
来源：http://ors.guannengcc.top

[T38] Lua：条件
来源：http://xly.cqqwz.cn

if x > 0 then print("正") end
来源：http://ftu.shzxlz.cn

[T39] Lua：模式匹配
来源：http://hjt.shangyingyoupin.top

string.find(s, "%d+")
来源：http://sfr.uphjek.com

[T40] Lua：元表
来源：http://pyj.mhx1999.top

setmetatable({}, { __index = base })
来源：http://ddw.fzhhl.top

[T41] Perl：Hello World
来源：http://cvz.chenzaomai.com

print "Hello\n";
来源：http://drq.guannengcc.top

[T42] Perl：变量类型
来源：http://xik.0kj1m.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://juf.xuetiantiany.cn

[T43] Perl：字符串插值
来源：http://ire.chenjidiqi.icu

"值: $a"
来源：http://dhn.daxiang520.top

[T44] Perl：条件
来源：http://hsy.yuanzhike.top

if ($a > 0) { print "正"; }
来源：http://rmo.shangyingyoupin.top

[T45] Perl：数组遍历
来源：http://fdj.yj20258888.top

for my $x (@arr) { print $x; }
来源：http://pcu.guowangkeji.top

[T46] Perl：哈希操作
来源：http://dzd.zdbjq.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pnf.cucudq.cn

[T47] Perl：正则捕获
来源：http://jpw.zhiwuduotai.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://hio.pycfn.com

[T48] Perl：正则替换
来源：http://knv.tianlin.xyz

$s =~ s/old/new/g;
来源：http://txr.sysykeji.top

[T49] Perl：函数
来源：http://fig.hysaishi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://dqf.zycfv.cn

[T50] Perl：逐行读文件
来源：http://rlp.chenlongwang.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ovo.hesvh.cn

while (my $line = <$fh>) { print $line; }
来源：http://sql.haohaochexian.top

[T51] Scala：Hello World
来源：http://qgv.kuanghao11.cn

println("Hello")
来源：http://ucv.cqqwz.cn

[T52] Scala：变量
来源：http://eul.jinghuilouyu.cn

val a = 1;  var b = 2
来源：http://lxd.ybcxt.top

[T53] Scala：字符串插值
来源：http://bam.tanke756.top

s"值: $b"
来源：http://gja.fktsv.cn

[T54] Scala：集合映射
来源：http://yld.tanke756.top

List(1, 2, 3).map(_ * 2)
来源：http://gum.svipenyu.cn

[T55] Scala：集合过滤
来源：http://wyq.zhiwuduotai.top

List(1, 2, 3).filter(_ > 1)
来源：http://vbl.aibaodan.cn

[T56] Scala：样例类
来源：http://fph.hesvh.cn

case class User(name: String, age: Int)
来源：http://jaq.yj20258888.top

[T57] Scala：模式匹配
来源：http://bpn.kuanghao11.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://tbl.birdmap.top

[T58] Scala：函数定义
来源：http://znd.shuidangran.top

def add(a: Int, b: Int): Int = a + b
来源：http://mqr.chenzaomai.com

[T59] Scala：循环
来源：http://zrw.jiagoushi.top

for (i <- 1 to 10) println(i)
来源：http://pcz.sxryk.cn

[T60] Scala：折叠
来源：http://tvb.guannengcc.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cqo.jlsjyb.cn

================================================================================
来源：http://smf.0kj1m.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://uhu.yj20258888.top

================================================================================
来源：http://yvu.zhixingplan.top

[U01] Py：创建虚拟环境
来源：http://nnu.tanke756.top

python -m venv .venv && source .venv/bin/activate
来源：http://cvx.xinyue.icu

[U02] Py：导出 / 安装依赖
来源：http://eyg.jinyuanbaomall.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zaz.hcnkem.com

[U03] Py：加载 .env 配置
来源：http://gbf.hammf.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://nil.guannengcc.top

[U04] Py：变量调试打印
来源：http://gkz.yj20258888.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://fkl.shanyushiyangkeji.top

[U05] Py：列表去重且保序
来源：http://qxp.yuanzhike.top

list(dict.fromkeys(arr))
来源：http://gjy.tanke756.top

[U06] Py：合并两个字典
来源：http://dhj.zhiwuduotai.top

{**a, **b}
来源：http://kxo.havefunace.top

[U07] Py：反转字典键值
来源：http://eig.jlsjyb.cn

{v: k for k, v in d.items()}
来源：http://iaf.gaohongyu789.top

[U08] Py：展平二维列表
来源：http://nlm.pycfn.com

[y for x in nested for y in x]
来源：http://aiu.shanyushiyangtech.top

[U09] Py：字典取最大值的键
来源：http://msx.daria6918.cn

max(d, key=d.get)
来源：http://dto.birdmap.top

[U10] Py：按值排序字典
来源：http://flt.gotoacloud.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mcb.ybcxt.top


<!-- 参考信息 -->