代发 wailian999

openssl rand -hex 16
来源：http://dvo.dashuyun.cn

[R68] 计算文件校验值
来源：http://ycp.ywan-chungtsiang.top

sha256sum a.txt;  md5sum a.txt
来源：http://bql.chenjidiqi.icu

[R69] 生成随机密码
来源：http://upt.fehbvm.com

head -c 16 /dev/urandom | base64
来源：http://fsg.hesvh.cn

[R70] 时间戳与互转
来源：http://bts.haohaochexian.top

date +%s;  date -d @1700000000
来源：http://vdj.pycfn.com

[R71] 日期格式化
来源：http://hnt.fzhhl.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://oeo.shanyushiyangtech.top

[R72] 等待端口就绪
来源：http://sxv.cdnleiting.top

until nc -z localhost 3306; do sleep 1; done
来源：http://nwo.wangshuangyany.cn

[R73] 分割大日志
来源：http://ycf.vehdjk.com

split -l 1000 big.log part_
来源：http://jrd.ivvv.top

[R74] 批量重命名
来源：http://osn.vqdsnc.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qdi.ehwqpu.com

[R75] 导出环境变量
来源：http://qkp.nanxuanxn.top

export PATH="$HOME/bin:$PATH"
来源：http://zdc.nwbrower.top

[R76] 使用临时文件
来源：http://qrl.nanxuanxn.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nwd.wangshuangyany.cn

[R77] 读取用户输入
来源：http://ojy.yj20258.top

read -rp "请输入: " ans
来源：http://tgr.yj20258888.top

[R78] 交互式菜单
来源：http://pdt.xingfuxueyuan.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://pld.jinghuilouyu.cn

[R79] 解析命令行选项
来源：http://rnx.haohaochexian.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zty.tian-w.cn

[R80] 查看脚本执行耗时
来源：http://tcr.guowangkeji.top

time ./run.sh
来源：http://kvg.cheryme.top

================================================================================
来源：http://zzo.andypj.xyz

S. C / C++ 专题
来源：http://xiv.shanyushiyangkeji.top

================================================================================
来源：http://atu.daria6918.cn

[S01] C：Hello World
来源：http://ibn.havefunace.top

#include <stdio.h>
来源：http://ygv.nwbrower.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://nge.zhoulong.xyz

[S02] C：变量与格式化输出
来源：http://qmh.yuanzhike.top

int a = 10; printf("%d\n", a);
来源：http://dom.daria6918.cn

[S03] C：读入整数
来源：http://zvt.zdqjudy.top

int x; scanf("%d", &x);
来源：http://scy.kuanghao11.cn

[S04] C：字符串复制
来源：http://ubv.yfazqb.com

char dst[32]; strcpy(dst, "hi");
来源：http://imb.fanxiaobao.xyz

[S05] C：字符串长度
来源：http://jqc.yueranfly.top

strlen(s)
来源：http://vym.tarul.cn

[S06] C：字符串比较
来源：http://lyc.hammf.cn

strcmp(a, b) == 0
来源：http://dnk.ydjk.org.cn

[S07] C：数组遍历求和
来源：http://rxl.wangdashe.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nif.aibaodan.cn

[S08] C：动态内存分配与释放
来源：http://eeo.wangdashe.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dfd.fanxiaobao.xyz

[S09] C：结构体定义与初始化
来源：http://txq.nanxinkj.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lgz.vehdjk.com

[S10] C：指针与解引用
来源：http://hvg.dianchejie.cn

int *p = &a;  *p = 5;
来源：http://ckj.tanke756.top

[S11] C：逐行读文件
来源：http://snd.c1oappe.top

FILE *f = fopen("a.txt", "r");
来源：http://tzn.gogol.net.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ytn.meibo888.top

fclose(f);
来源：http://zfe.jinqigfzy.top

[S12] C：写文件
来源：http://xke.mhx1999.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fuo.shzxlz.cn

[S13] C：宏定义
来源：http://qgr.ctjpmb.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://knf.jqgufenzy.top

[S14] C：枚举
来源：http://dlu.meibo888.top

enum Color { RED, GREEN, BLUE };
来源：http://tpe.cucudq.cn

[S15] C：类型转换
来源：http://nha.zhengqikj.top

(double) a / b
来源：http://kjf.hfpthk.cn

[S16] C：位操作置位
来源：http://lqb.shuidangran.top

x |= (1 << 3);
来源：http://oxg.cashguo.top

[S17] C：安全拼接字符串
来源：http://kox.yj20258.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ogt.fktsv.cn

[S18] C：命令行参数
来源：http://iwf.xylfe.cn

int main(int argc, char **argv)
来源：http://rsk.yj20258888.top

[S19] C：快速排序
来源：http://won.pengpengdd.cyou

qsort(a, n, sizeof(int), cmp);
来源：http://niq.jiagoushi.top

[S20] C：二分查找
来源：http://sjr.fzhhl.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://syr.fzhhl.top

[S21] C：字符类别判断
来源：http://qgm.fktsv.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hvx.sjlbkw.cn

[S22] C：字符串转数字
来源：http://dtg.guannengcc.top

atoi("42");  strtod("3.14", NULL);
来源：http://upb.cashguo.top

[S23] C：随机数
来源：http://gtw.tarul.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xch.mhx1999.top

[S24] C：获取本地时间
来源：http://lud.xziqi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jtb.cheryme.top

[S25] C：内存拷贝
来源：http://wzj.redwolf501.top

memcpy(dst, src, n);
来源：http://gmd.zhaomingkeji.xyz

[S26] C：内存清零
来源：http://grh.zhiwuduotai.top

memset(a, 0, sizeof a);
来源：http://jxq.bbcook.cn

[S27] C：定义常量
来源：http://rvd.xziqi.cn

const double PI = 3.14159;
来源：http://vms.hnqzz.top

[S28] C：静态变量
来源：http://ihr.andypj.xyz

static int counter = 0;
来源：http://syz.hnqzz.top

[S29] C：变参函数
来源：http://swd.chenjidiqi.icu

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cvu.meibo888.top

[S30] C：头文件保护
来源：http://skf.quarkkingdee.top

#ifndef X_H
来源：http://udb.jyoumei.cn

#define X_H
来源：http://thc.bjfxy.top

#endif
来源：http://yvx.uphjek.com

[S31] C++：Hello World
来源：http://auy.xziqi.cn

#include <iostream>
来源：http://ajj.hywenlv.cn

int main() { std::cout << "Hello\n"; }
来源：http://vwt.fanxiaobao.xyz

[S32] C++：字符串
来源：http://kgy.aizwys.cn

std::string s = "hi";  s += "!";
来源：http://mna.redwolf501.top

[S33] C++：vector 增删
来源：http://gau.zhaomingkeji.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qlp.epnwcf.com

[S34] C++：遍历 vector
来源：http://sbc.ydjk.org.cn

for (auto &x : v) { std::cout << x; }
来源：http://tef.jiagoushi.top

[S35] C++：map
来源：http://ynb.tian-w.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vro.quarkkingdee.top

[S36] C++：unordered_map
来源：http://mty.fktsv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xyb.pengpengdd.cyou

[S37] C++：set
来源：http://yzp.vehdjk.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vwx.jiagoushi.top

[S38] C++：排序
来源：http://qsq.zhijiandao.cn

std::sort(v.begin(), v.end());
来源：http://dlj.tian-w.cn

[S39] C++：自定义比较器排序
来源：http://ufr.sysykeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vmc.tian-w.cn

[S40] C++：查找元素
来源：http://eia.cheryme.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vma.yj20258.top

[S41] C++：类与构造函数
来源：http://rne.ctjpmb.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vzh.yangfankeji.com

[S42] C++：继承与虚函数
来源：http://tfo.aibaodan.cn

class B : public Base { public: void f() override {} };
来源：http://iat.gzhubu.top

[S43] C++：智能指针
来源：http://vkn.shanyushiyangkeji.top

auto p = std::make_unique<int>(5);
来源：http://nbq.jqgufenzy.top

[S44] C++：引用传参
来源：http://jav.kuanghao11.cn

void inc(int &x) { ++x; }
来源：http://uzz.fktsv.cn

[S45] C++：lambda
来源：http://sml.ydjk.org.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vhn.tarul.cn

[S46] C++：函数模板
来源：http://jaz.mhx1999.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xld.hnqzz.top

[S47] C++：结构化绑定遍历
来源：http://kht.yueranfly.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lqd.yvedp.cn

[S48] C++：逐行读文件
来源：http://lbf.ehwqpu.com

std::ifstream in("a.txt");  std::string line;
来源：http://qqm.gogol.net.cn

while (std::getline(in, line)) { }
来源：http://zru.xuetiantiany.cn

[S49] C++：写文件
来源：http://dzr.52xcode.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vik.gaohongyu789.top

[S50] C++：格式化数字
来源：http://pha.yfazqb.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vnb.mhx1999.top

[S51] C++：显式类型转换
来源：http://lsf.c1oappe.top

static_cast<double>(a) / b
来源：http://mvu.ydjk.org.cn

[S52] C++：const 与 noexcept
来源：http://rqx.jinqigfzy.top

int size() const noexcept { return n_; }
来源：http://uoz.jinyuanbaomall.cn

[S53] C++：移动语义
来源：http://syq.nanxuanxn.top

std::vector<int> w = std::move(v);
来源：http://rtu.ywan-chungtsiang.top

[S54] C++：异常处理
来源：http://fkt.yangfankeji.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://iwv.tian-w.cn

[S55] C++：结构化绑定
来源：http://swx.c1oappe.top

auto [a, b] = std::make_pair(1, 2);
来源：http://umu.0kj1m.cn

[S56] C++：optional
来源：http://sqs.ehwqpu.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ttf.jlsjyb.cn

[S57] C++：编译期常量
来源：http://gbs.shuidangran.top

constexpr int N = 10;
来源：http://vtb.zhengqikj.top

[S58] C++：命名空间
来源：http://txu.smart0.xyz

namespace ns { int f() { return 1; } }
来源：http://tsx.zhijiandao.cn

[S59] C++：静态断言
来源：http://jew.jinghuilouyu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://koz.dashuyun.cn

[S60] C++：遍历并删除元素
来源：http://fol.sufxvd.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vwe.wangdashe.top

================================================================================
来源：http://urw.daxiang520.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ljq.shzxlz.cn

================================================================================
来源：http://xnb.ydzc1.top

[T01] Kotlin：Hello World
来源：http://biw.cdnleiting.top

println("Hello")
来源：http://ipi.hfpthk.cn

[T02] Kotlin：变量
来源：http://imz.yuxming.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xex.ydjk.org.cn

[T03] Kotlin：字符串模板
来源：http://vbz.pengpengdd.cyou

"值: $b"
来源：http://dgu.epnwcf.com

[T04] Kotlin：空安全
来源：http://gaq.jinghuilouyu.cn

val n: String? = null;  n?.length
来源：http://tpg.zhoulong.xyz

[T05] Kotlin：when 表达式
来源：http://spp.daxiang520.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zes.ctjpmb.com

[T06] Kotlin：集合映射
来源：http://hbm.jiagoushi.top

listOf(1, 2, 3).map { it * 2 }
来源：http://rdx.jinqigufen.top

[T07] Kotlin：集合过滤
来源：http://nto.jqgfzy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://vix.ehwqpu.com

[T08] Kotlin：数据类
来源：http://wjo.kuanghao11.cn

data class User(val name: String, val age: Int)
来源：http://ogr.wangdashe.top

[T09] Kotlin：扩展函数
来源：http://hqq.shangyingyoupin.top

fun String.exclaim() = this + "!"
来源：http://ivl.yangfankeji.com

[T10] Kotlin：默认参数
来源：http://gij.tanke756.top

fun greet(name: String = "World") = "Hi $name"
来源：http://wpj.zhoulong.xyz

[T11] Kotlin：协程
来源：http://rmp.sysykeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ric.zhixingplan.top

[T12] Kotlin：解构声明
来源：http://llx.haohaochexian.top

val (a, b) = Pair(1, 2)
来源：http://bur.tianlin.xyz

[T13] Kotlin：只读 Map
来源：http://jja.hongshengwenyu.top

val m = mapOf("a" to 1)
来源：http://unh.tarul.cn

[T14] Kotlin：循环
来源：http://jcm.vehdjk.com

for (i in 1..10) println(i)
来源：http://abp.cqqwz.cn

[T15] Kotlin：接口
来源：http://utl.hesvh.cn

interface Shape { fun area(): Double }
来源：http://wgs.vqdsnc.cn

[T16] Swift：Hello World
来源：http://quf.chenlongwang.top

print("Hello")
来源：http://kxo.hfpthk.cn

[T17] Swift：变量与常量
来源：http://egb.svipenyu.cn

var a = 1;  let b = 2
来源：http://tia.hcnkem.com

[T18] Swift：字符串插值
来源：http://dpa.pengpengdd.cyou

"值: \(b)"
来源：http://tkj.guannengcc.top

[T19] Swift：可选绑定
来源：http://dpg.ehwqpu.com

if let n = opt { print(n) }
来源：http://wne.havefunace.top

[T20] Swift：数组操作
来源：http://jqs.zhengqikj.top

var a = [1, 2, 3];  a.append(4)
来源：http://msp.jinghuilouyu.cn

[T21] Swift：遍历
来源：http://ebg.kuanghao11.cn

for x in a { print(x) }
来源：http://jjd.jqgfzy.top

[T22] Swift：字典
来源：http://ajb.cqqwz.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mdo.feifeiyinyue.top

[T23] Swift：函数
来源：http://wqg.hfpthk.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pyf.redwolf501.top

[T24] Swift：闭包
来源：http://lzv.tian-w.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://aeh.jinqigfzy.top

[T25] Swift：结构体
来源：http://uar.yonumen.top

struct P { var x: Int }
来源：http://trp.snrcjt.cn

[T26] Swift：类与重写
来源：http://jbp.uphjek.com

class A: Base { override func f() {} }
来源：http://efe.zdqjudy.top

[T27] Swift：错误处理
来源：http://hoj.fehbvm.com

do { try f() } catch { print(error) }
来源：http://ulm.hywenlv.cn

[T28] Swift：枚举
来源：http://bnw.xinyue.icu

enum Color { case red, green }
来源：http://fzr.haohaochexian.top

[T29] Swift：guard 提前返回
来源：http://hkz.aibaodan.cn

guard let x = opt else { return }
来源：http://clv.pycfn.com

[T30] Swift：协议
来源：http://jfm.wangdashe.top

protocol Shape { func area() -> Double }
来源：http://txt.pengpengdd.cyou

[T31] Lua：Hello World
来源：http://avk.hysaishi.cn

print("Hello")
来源：http://gvw.xinyue.icu

[T32] Lua：局部变量
来源：http://rbg.jinghuilouyu.cn

local a = 1
来源：http://lav.iojbl.cn

[T33] Lua：表（数组）
来源：http://yfo.iojbl.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://piq.yanxiufei.cn

[T34] Lua：遍历表
来源：http://ngz.xingfuxueyuan.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://zdp.hnqzz.top

[T35] Lua：字典表
来源：http://pmf.jinyuanbaomall.cn

local d = { a = 1 };  d.b = 2
来源：http://tue.yuanzhike.top

[T36] Lua：函数
来源：http://kra.fzhhl.top

function add(a, b) return a + b end
来源：http://pue.xingfuxueyuan.xyz

[T37] Lua：字符串拼接
来源：http://rai.nwbrower.top

"a" .. "b"
来源：http://nqt.zhaomingkeji.xyz

[T38] Lua：条件
来源：http://vlf.hnxiangtu.top

if x > 0 then print("正") end
来源：http://jtl.jinqigufen.top

[T39] Lua：模式匹配
来源：http://uex.andypj.xyz

string.find(s, "%d+")
来源：http://ium.shanyushiyangtech.top

[T40] Lua：元表
来源：http://lbp.zhengqikj.top

setmetatable({}, { __index = base })
来源：http://xrv.bjfxy.top

[T41] Perl：Hello World
来源：http://ugc.mhx1999.top

print "Hello\n";
来源：http://gdt.yvedp.cn

[T42] Perl：变量类型
来源：http://ktj.fengsongda.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yat.fzhhl.top

[T43] Perl：字符串插值
来源：http://hbn.snrcjt.cn

"值: $a"
来源：http://qvv.yanxiufei.cn

[T44] Perl：条件
来源：http://gcx.svipenyu.cn

if ($a > 0) { print "正"; }
来源：http://lab.hesvh.cn

[T45] Perl：数组遍历
来源：http://kvl.pengpengdd.cyou

for my $x (@arr) { print $x; }
来源：http://mqy.xinyue.icu

[T46] Perl：哈希操作
来源：http://yjk.ydjk.org.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://max.ppjwa.cn

[T47] Perl：正则捕获
来源：http://hyy.shuidangran.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ggk.sufxvd.cn

[T48] Perl：正则替换
来源：http://dbt.snrcjt.cn

$s =~ s/old/new/g;
来源：http://tmy.feifeiyinyue.top

[T49] Perl：函数
来源：http://oza.jinqigfzy.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lpq.ydzc1.top

[T50] Perl：逐行读文件
来源：http://eva.zhaomingkeji.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://cxb.yj20258888.top

while (my $line = <$fh>) { print $line; }
来源：http://tta.vqdsnc.cn

[T51] Scala：Hello World
来源：http://woj.zhongyouzk.top

println("Hello")
来源：http://vpc.xingfuxueyuan.xyz

[T52] Scala：变量
来源：http://hmg.hcnkem.com

val a = 1;  var b = 2
来源：http://arm.yj20258888.top

[T53] Scala：字符串插值
来源：http://mcj.tanke756.top

s"值: $b"
来源：http://euw.quarkkingdee.top

[T54] Scala：集合映射
来源：http://uyw.guowangkeji.top

List(1, 2, 3).map(_ * 2)
来源：http://ups.316326.xyz

[T55] Scala：集合过滤
来源：http://sgj.jianghu66.top

List(1, 2, 3).filter(_ > 1)
来源：http://rjd.jlsjyb.cn

[T56] Scala：样例类
来源：http://aup.ywan-chungtsiang.top

case class User(name: String, age: Int)
来源：http://cwy.ybcxt.top

[T57] Scala：模式匹配
来源：http://uyy.ydjk.org.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vxt.bjfxy.top

[T58] Scala：函数定义
来源：http://weq.zhoulong.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://ntv.gaohongyu789.top

[T59] Scala：循环
来源：http://nyz.meibo888.top

for (i <- 1 to 10) println(i)
来源：http://lux.zhiwuduotai.top

[T60] Scala：折叠
来源：http://opv.fengsongda.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://msa.jianghu66.top

================================================================================
来源：http://oct.zdbjq.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fjo.316326.xyz

================================================================================
来源：http://tgv.sysykeji.top

[U01] Py：创建虚拟环境
来源：http://iwi.chenlongwang.top

python -m venv .venv && source .venv/bin/activate
来源：http://odg.yongpay.top

[U02] Py：导出 / 安装依赖
来源：http://qms.dianchejie.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wlf.aibaodan.cn

[U03] Py：加载 .env 配置
来源：http://obp.jqgfzy.top

from dotenv import load_dotenv; load_dotenv()
来源：http://qmy.quarkkingdee.top

[U04] Py：变量调试打印
来源：http://jwi.mhx1999.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dur.wangdashe.top

[U05] Py：列表去重且保序
来源：http://nsp.fanxiaobao.xyz

list(dict.fromkeys(arr))
来源：http://smb.havefunace.top

[U06] Py：合并两个字典
来源：http://czn.xuetiantiany.cn

{**a, **b}
来源：http://hpc.ywan-chungtsiang.top

[U07] Py：反转字典键值
来源：http://xmt.jinqigufen.top

{v: k for k, v in d.items()}
来源：http://zih.quarkkingdee.top

[U08] Py：展平二维列表
来源：http://ufu.fzhhl.top

[y for x in nested for y in x]
来源：http://aku.cashguo.top


<!-- 参考信息 -->