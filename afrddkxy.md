代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lyi.gaohongyu789.top

[R66] 定时任务
来源：http://hvw.ctjpmb.com

crontab -e;  crontab -l
来源：http://pei.xingfuxueyuan.xyz

[R67] 生成随机十六进制串
来源：http://phv.chenlongwang.top

openssl rand -hex 16
来源：http://ibh.tian-w.cn

[R68] 计算文件校验值
来源：http://zkr.feifeiyinyue.top

sha256sum a.txt;  md5sum a.txt
来源：http://gyk.cucudq.cn

[R69] 生成随机密码
来源：http://iph.gzhubu.top

head -c 16 /dev/urandom | base64
来源：http://cep.xylfe.cn

[R70] 时间戳与互转
来源：http://sas.cheryme.top

date +%s;  date -d @1700000000
来源：http://gxs.yj20258888.top

[R71] 日期格式化
来源：http://lmo.52xcode.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://tue.hywenlv.cn

[R72] 等待端口就绪
来源：http://iyw.pycfn.com

until nc -z localhost 3306; do sleep 1; done
来源：http://zcp.cucudq.cn

[R73] 分割大日志
来源：http://drn.zhengqikj.top

split -l 1000 big.log part_
来源：http://wbt.ivvv.top

[R74] 批量重命名
来源：http://zuu.ctjpmb.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wmx.zdbjq.cn

[R75] 导出环境变量
来源：http://tkv.zycfv.cn

export PATH="$HOME/bin:$PATH"
来源：http://zha.zhijiandao.cn

[R76] 使用临时文件
来源：http://fez.zhoulong.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yeg.0kj1m.cn

[R77] 读取用户输入
来源：http://ims.xinyue.icu

read -rp "请输入: " ans
来源：http://rif.hcnkem.com

[R78] 交互式菜单
来源：http://zpb.jinyuanbaomall.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://qdi.wangdashe.top

[R79] 解析命令行选项
来源：http://tei.zdqjudy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qpg.fengsongda.top

[R80] 查看脚本执行耗时
来源：http://upb.sufxvd.cn

time ./run.sh
来源：http://dwi.yuxming.cn

================================================================================
来源：http://jzu.nanxuanxn.top

S. C / C++ 专题
来源：http://qov.shzxlz.cn

================================================================================
来源：http://imn.sjlbkw.cn

[S01] C：Hello World
来源：http://dwf.fanxiaobao.xyz

#include <stdio.h>
来源：http://pfa.fzhhl.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ulm.chenlongwang.top

[S02] C：变量与格式化输出
来源：http://xog.fktsv.cn

int a = 10; printf("%d\n", a);
来源：http://rap.meibo888.top

[S03] C：读入整数
来源：http://asx.birdmap.top

int x; scanf("%d", &x);
来源：http://xdz.cucudq.cn

[S04] C：字符串复制
来源：http://ulk.xinyue.icu

char dst[32]; strcpy(dst, "hi");
来源：http://zqv.jinqigufen.top

[S05] C：字符串长度
来源：http://ywx.zdqjudy.top

strlen(s)
来源：http://zmw.gogol.net.cn

[S06] C：字符串比较
来源：http://yum.ppjwa.cn

strcmp(a, b) == 0
来源：http://gga.yuanzhike.top

[S07] C：数组遍历求和
来源：http://dlb.fktsv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zxn.nanxinkj.top

[S08] C：动态内存分配与释放
来源：http://dyk.vehdjk.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hjt.ivvv.top

[S09] C：结构体定义与初始化
来源：http://jgk.ppjwa.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ygt.zycfv.cn

[S10] C：指针与解引用
来源：http://xhm.gzhubu.top

int *p = &a;  *p = 5;
来源：http://fjy.yonumen.top

[S11] C：逐行读文件
来源：http://wmt.fanxiaobao.xyz

FILE *f = fopen("a.txt", "r");
来源：http://skg.hywenlv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://adz.yongpay.top

fclose(f);
来源：http://cpi.cqqwz.cn

[S12] C：写文件
来源：http://lof.jqgfzy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://djo.sxryk.cn

[S13] C：宏定义
来源：http://xff.zdbjq.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bye.bbcook.cn

[S14] C：枚举
来源：http://nhg.haohaochexian.top

enum Color { RED, GREEN, BLUE };
来源：http://jbj.cashguo.top

[S15] C：类型转换
来源：http://lfz.ivvv.top

(double) a / b
来源：http://wxp.jqgufenzy.top

[S16] C：位操作置位
来源：http://bpm.sufxvd.cn

x |= (1 << 3);
来源：http://zqf.fanxiaobao.xyz

[S17] C：安全拼接字符串
来源：http://kio.ydjk.org.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://csd.aizwys.cn

[S18] C：命令行参数
来源：http://fnw.sysykeji.top

int main(int argc, char **argv)
来源：http://gvj.cashguo.top

[S19] C：快速排序
来源：http://lkl.jinqigufen.top

qsort(a, n, sizeof(int), cmp);
来源：http://jyu.tanke756.top

[S20] C：二分查找
来源：http://gtb.shzxlz.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rjg.smart0.xyz

[S21] C：字符类别判断
来源：http://its.ydzc1.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://eyl.fktsv.cn

[S22] C：字符串转数字
来源：http://cix.gogol.net.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ray.sweek.top

[S23] C：随机数
来源：http://nai.hnqzz.top

srand(time(NULL));  int r = rand() % 100;
来源：http://vum.bjfxy.top

[S24] C：获取本地时间
来源：http://qgk.zhijiandao.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nen.nwbrower.top

[S25] C：内存拷贝
来源：http://kdq.dashuyun.cn

memcpy(dst, src, n);
来源：http://ywp.smart0.xyz

[S26] C：内存清零
来源：http://mir.c1oappe.top

memset(a, 0, sizeof a);
来源：http://dye.jyoumei.cn

[S27] C：定义常量
来源：http://hqv.zhixingplan.top

const double PI = 3.14159;
来源：http://opx.chenjidiqi.icu

[S28] C：静态变量
来源：http://gvx.zdbjq.cn

static int counter = 0;
来源：http://wlb.ybcxt.top

[S29] C：变参函数
来源：http://xof.mhx1999.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gxe.ppjwa.cn

[S30] C：头文件保护
来源：http://dbu.jyoumei.cn

#ifndef X_H
来源：http://cbz.andypj.xyz

#define X_H
来源：http://yrs.fanxiaobao.xyz

#endif
来源：http://kio.zycfv.cn

[S31] C++：Hello World
来源：http://jgf.vehdjk.com

#include <iostream>
来源：http://rhk.hywenlv.cn

int main() { std::cout << "Hello\n"; }
来源：http://ffs.cheryme.top

[S32] C++：字符串
来源：http://mkr.feifeiyinyue.top

std::string s = "hi";  s += "!";
来源：http://qfm.jlsjyb.cn

[S33] C++：vector 增删
来源：http://gxm.jyoumei.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://joc.52xcode.cn

[S34] C++：遍历 vector
来源：http://dzm.xuetiantiany.cn

for (auto &x : v) { std::cout << x; }
来源：http://apz.sufxvd.cn

[S35] C++：map
来源：http://dzl.zhaomingkeji.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yeq.smart0.xyz

[S36] C++：unordered_map
来源：http://dqt.chenlongwang.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://iid.nanxuanxn.top

[S37] C++：set
来源：http://kqw.bjfxy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://thm.cqqwz.cn

[S38] C++：排序
来源：http://tur.gotoacloud.top

std::sort(v.begin(), v.end());
来源：http://kpg.tianlin.xyz

[S39] C++：自定义比较器排序
来源：http://ccz.jinyuanbaomall.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://btu.xziqi.cn

[S40] C++：查找元素
来源：http://zrn.hywenlv.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mpa.gotoacloud.top

[S41] C++：类与构造函数
来源：http://ezm.mhx1999.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xwp.daria6918.cn

[S42] C++：继承与虚函数
来源：http://tus.gogol.net.cn

class B : public Base { public: void f() override {} };
来源：http://bve.yuxming.cn

[S43] C++：智能指针
来源：http://jgj.shuidangran.top

auto p = std::make_unique<int>(5);
来源：http://eib.ivvv.top

[S44] C++：引用传参
来源：http://rgs.yanxiufei.cn

void inc(int &x) { ++x; }
来源：http://txa.ppjwa.cn

[S45] C++：lambda
来源：http://hmj.hongshengwenyu.top

auto add = [](int a, int b) { return a + b; };
来源：http://hrb.0kj1m.cn

[S46] C++：函数模板
来源：http://ffs.ydzc1.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wnf.xziqi.cn

[S47] C++：结构化绑定遍历
来源：http://maf.ywan-chungtsiang.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://czc.fanxiaobao.xyz

[S48] C++：逐行读文件
来源：http://hci.zhengqikj.top

std::ifstream in("a.txt");  std::string line;
来源：http://dou.yonumen.top

while (std::getline(in, line)) { }
来源：http://jzt.uphjek.com

[S49] C++：写文件
来源：http://rbo.hammf.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bfi.jlsjyb.cn

[S50] C++：格式化数字
来源：http://bic.fengsongda.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kxd.hysaishi.cn

[S51] C++：显式类型转换
来源：http://ndo.9152youxi.cn

static_cast<double>(a) / b
来源：http://fbg.wangshuangyany.cn

[S52] C++：const 与 noexcept
来源：http://ltm.ivvv.top

int size() const noexcept { return n_; }
来源：http://pcc.nwbrower.top

[S53] C++：移动语义
来源：http://lsu.nanxuanxn.top

std::vector<int> w = std::move(v);
来源：http://bts.shanyushiyangtech.top

[S54] C++：异常处理
来源：http://xaa.birdmap.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bio.ppjwa.cn

[S55] C++：结构化绑定
来源：http://qto.dashuyun.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://fae.nwbrower.top

[S56] C++：optional
来源：http://qbp.yonumen.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qcb.cucudq.cn

[S57] C++：编译期常量
来源：http://lgt.zhixingplan.top

constexpr int N = 10;
来源：http://xsv.sufxvd.cn

[S58] C++：命名空间
来源：http://pnj.pycfn.com

namespace ns { int f() { return 1; } }
来源：http://xsc.epnwcf.com

[S59] C++：静态断言
来源：http://evc.pengpengdd.cyou

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wwc.havefunace.top

[S60] C++：遍历并删除元素
来源：http://qmz.hesvh.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://aqv.gzhubu.top

================================================================================
来源：http://loc.zhijiandao.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xxb.ctjpmb.com

================================================================================
来源：http://tpt.hesvh.cn

[T01] Kotlin：Hello World
来源：http://tgg.c1oappe.top

println("Hello")
来源：http://ldp.cqqwz.cn

[T02] Kotlin：变量
来源：http://ehr.smart0.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uct.pengpengdd.cyou

[T03] Kotlin：字符串模板
来源：http://noz.aizwys.cn

"值: $b"
来源：http://cnx.shuidangran.top

[T04] Kotlin：空安全
来源：http://jnj.hfpthk.cn

val n: String? = null;  n?.length
来源：http://lkt.hongshengwenyu.top

[T05] Kotlin：when 表达式
来源：http://pon.cheryme.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fpo.smart0.xyz

[T06] Kotlin：集合映射
来源：http://ikn.ehwqpu.com

listOf(1, 2, 3).map { it * 2 }
来源：http://uvu.jiagoushi.top

[T07] Kotlin：集合过滤
来源：http://yhd.hnxiangtu.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://fcu.hcnkem.com

[T08] Kotlin：数据类
来源：http://gpm.yuxming.cn

data class User(val name: String, val age: Int)
来源：http://xdv.shangyingyoupin.top

[T09] Kotlin：扩展函数
来源：http://skg.pengpengdd.cyou

fun String.exclaim() = this + "!"
来源：http://kcf.wangshuangyany.cn

[T10] Kotlin：默认参数
来源：http://nza.nwbrower.top

fun greet(name: String = "World") = "Hi $name"
来源：http://isf.hfpthk.cn

[T11] Kotlin：协程
来源：http://voq.smart0.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://kzp.andypj.xyz

[T12] Kotlin：解构声明
来源：http://qhp.nanxuanxn.top

val (a, b) = Pair(1, 2)
来源：http://abp.hnxiangtu.top

[T13] Kotlin：只读 Map
来源：http://usp.ybcxt.top

val m = mapOf("a" to 1)
来源：http://mhv.yj20258888.top

[T14] Kotlin：循环
来源：http://sjr.gzhubu.top

for (i in 1..10) println(i)
来源：http://lns.zhoulong.xyz

[T15] Kotlin：接口
来源：http://vvi.havefunace.top

interface Shape { fun area(): Double }
来源：http://ibo.hywenlv.cn

[T16] Swift：Hello World
来源：http://qwf.wangshuangyany.cn

print("Hello")
来源：http://ozf.chenlongwang.top

[T17] Swift：变量与常量
来源：http://izc.9152youxi.cn

var a = 1;  let b = 2
来源：http://sbs.pycfn.com

[T18] Swift：字符串插值
来源：http://acp.ybcxt.top

"值: \(b)"
来源：http://yih.daria6918.cn

[T19] Swift：可选绑定
来源：http://pga.hcnkem.com

if let n = opt { print(n) }
来源：http://nal.fanxiaobao.xyz

[T20] Swift：数组操作
来源：http://ujo.guowangkeji.top

var a = [1, 2, 3];  a.append(4)
来源：http://its.chenlongwang.top

[T21] Swift：遍历
来源：http://bve.ybcxt.top

for x in a { print(x) }
来源：http://jjz.xuanzx.com

[T22] Swift：字典
来源：http://nea.iojbl.cn

var d = ["a": 1];  d["b"] = 2
来源：http://aeu.guannengcc.top

[T23] Swift：函数
来源：http://ouy.316326.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ffx.yuxming.cn

[T24] Swift：闭包
来源：http://vli.xziqi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://oic.c1oappe.top

[T25] Swift：结构体
来源：http://gac.9152youxi.cn

struct P { var x: Int }
来源：http://jbx.sysykeji.top

[T26] Swift：类与重写
来源：http://kvz.snrcjt.cn

class A: Base { override func f() {} }
来源：http://zat.xziqi.cn

[T27] Swift：错误处理
来源：http://xig.shangyingyoupin.top

do { try f() } catch { print(error) }
来源：http://grk.vqdsnc.cn

[T28] Swift：枚举
来源：http://kye.guowangkeji.top

enum Color { case red, green }
来源：http://yia.sufxvd.cn

[T29] Swift：guard 提前返回
来源：http://qjs.316326.xyz

guard let x = opt else { return }
来源：http://rie.gzhubu.top

[T30] Swift：协议
来源：http://tav.tian-w.cn

protocol Shape { func area() -> Double }
来源：http://ncp.zhaomingkeji.xyz

[T31] Lua：Hello World
来源：http://pwd.316326.xyz

print("Hello")
来源：http://vpo.cucudq.cn

[T32] Lua：局部变量
来源：http://kar.hesvh.cn

local a = 1
来源：http://uds.pycfn.com

[T33] Lua：表（数组）
来源：http://iep.yongpay.top

local t = {1, 2, 3};  t[4] = 4
来源：http://bze.tarul.cn

[T34] Lua：遍历表
来源：http://zoa.gzhubu.top

for i, v in ipairs(t) do print(i, v) end
来源：http://hdd.havefunace.top

[T35] Lua：字典表
来源：http://dmp.shuidangran.top

local d = { a = 1 };  d.b = 2
来源：http://hkf.hongshengwenyu.top

[T36] Lua：函数
来源：http://vxv.zdqjudy.top

function add(a, b) return a + b end
来源：http://anp.zhiwuduotai.top

[T37] Lua：字符串拼接
来源：http://uxf.hfpthk.cn

"a" .. "b"
来源：http://dss.yongpay.top

[T38] Lua：条件
来源：http://mzh.epnwcf.com

if x > 0 then print("正") end
来源：http://eqn.xuanzx.com

[T39] Lua：模式匹配
来源：http://eop.shanyushiyangtech.top

string.find(s, "%d+")
来源：http://kzt.pengpengdd.cyou

[T40] Lua：元表
来源：http://dew.sufxvd.cn

setmetatable({}, { __index = base })
来源：http://hbf.epnwcf.com

[T41] Perl：Hello World
来源：http://ikb.52xcode.cn

print "Hello\n";
来源：http://uek.jinqigfzy.top

[T42] Perl：变量类型
来源：http://xhs.xinyue.icu

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://owj.zhiwuduotai.top

[T43] Perl：字符串插值
来源：http://usa.yj20258888.top

"值: $a"
来源：http://izl.cashguo.top

[T44] Perl：条件
来源：http://mhz.iojbl.cn

if ($a > 0) { print "正"; }
来源：http://nay.aibaodan.cn

[T45] Perl：数组遍历
来源：http://wrj.52xcode.cn

for my $x (@arr) { print $x; }
来源：http://bet.hfpthk.cn

[T46] Perl：哈希操作
来源：http://gvt.gaohongyu789.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hyv.birdmap.top

[T47] Perl：正则捕获
来源：http://aob.andypj.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://toc.yj20258.top

[T48] Perl：正则替换
来源：http://rdk.shanyushiyangkeji.top

$s =~ s/old/new/g;
来源：http://uek.wangshuangyany.cn

[T49] Perl：函数
来源：http://ibn.tian-w.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zkc.hnqzz.top

[T50] Perl：逐行读文件
来源：http://ecy.xuetiantiany.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://cry.haohaochexian.top

while (my $line = <$fh>) { print $line; }
来源：http://las.ivvv.top

[T51] Scala：Hello World
来源：http://kmf.sufxvd.cn

println("Hello")
来源：http://yqi.havefunace.top

[T52] Scala：变量
来源：http://zqh.wangshuangyany.cn

val a = 1;  var b = 2
来源：http://dha.ppjwa.cn

[T53] Scala：字符串插值
来源：http://sql.hysaishi.cn

s"值: $b"
来源：http://cam.bjfxy.top

[T54] Scala：集合映射
来源：http://krh.jqgufenzy.top

List(1, 2, 3).map(_ * 2)
来源：http://wdg.hnxiangtu.top

[T55] Scala：集合过滤
来源：http://ydh.chenjidiqi.icu

List(1, 2, 3).filter(_ > 1)
来源：http://zze.pycfn.com

[T56] Scala：样例类
来源：http://ppe.fzhhl.top

case class User(name: String, age: Int)
来源：http://owv.guannengcc.top

[T57] Scala：模式匹配
来源：http://hyr.jinqigufen.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://phn.iojbl.cn

[T58] Scala：函数定义
来源：http://vta.shzxlz.cn

def add(a: Int, b: Int): Int = a + b
来源：http://rsp.ybcxt.top

[T59] Scala：循环
来源：http://pmk.kuanghao11.cn

for (i <- 1 to 10) println(i)
来源：http://nkz.yj202588.top

[T60] Scala：折叠
来源：http://ioq.ctjpmb.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xjm.yanxiufei.cn

================================================================================
来源：http://xdm.jinyuanbaomall.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gfj.yj20258.top

================================================================================
来源：http://yhk.mhx1999.top

[U01] Py：创建虚拟环境
来源：http://ont.nanxuanxn.top

python -m venv .venv && source .venv/bin/activate
来源：http://yjg.ywan-chungtsiang.top

[U02] Py：导出 / 安装依赖
来源：http://pgj.guannengcc.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qls.feifeiyinyue.top

[U03] Py：加载 .env 配置
来源：http://fkq.yj202588.top

from dotenv import load_dotenv; load_dotenv()
来源：http://wic.mhx1999.top

[U04] Py：变量调试打印
来源：http://lgs.shanyushiyangkeji.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://sfc.zhixingplan.top

[U05] Py：列表去重且保序
来源：http://ewf.0kj1m.cn

list(dict.fromkeys(arr))
来源：http://lda.zhongyouzk.top

[U06] Py：合并两个字典
来源：http://atq.tianlin.xyz

{**a, **b}
来源：http://mze.9152youxi.cn


<!-- 参考信息 -->