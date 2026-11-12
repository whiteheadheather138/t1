代发 wailian999

openssl rand -hex 16
来源：http://uui.jinghuilouyu.cn

[R68] 计算文件校验值
来源：http://euo.hfpthk.cn

sha256sum a.txt;  md5sum a.txt
来源：http://chy.fktsv.cn

[R69] 生成随机密码
来源：http://zml.gogol.net.cn

head -c 16 /dev/urandom | base64
来源：http://fys.ctjpmb.com

[R70] 时间戳与互转
来源：http://tgq.zhoulong.xyz

date +%s;  date -d @1700000000
来源：http://nys.jinghuilouyu.cn

[R71] 日期格式化
来源：http://dru.yuxming.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rqz.cdnleiting.top

[R72] 等待端口就绪
来源：http://kjp.gogol.net.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://bgh.svipenyu.cn

[R73] 分割大日志
来源：http://jct.chenjidiqi.icu

split -l 1000 big.log part_
来源：http://cdy.shanyushiyangkeji.top

[R74] 批量重命名
来源：http://gmu.hongshengwenyu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hts.guowangkeji.top

[R75] 导出环境变量
来源：http://glq.tian-w.cn

export PATH="$HOME/bin:$PATH"
来源：http://lfv.yvedp.cn

[R76] 使用临时文件
来源：http://fee.tianlin.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ioi.yuanzhike.top

[R77] 读取用户输入
来源：http://rmf.mhx1999.top

read -rp "请输入: " ans
来源：http://srq.wangdashe.top

[R78] 交互式菜单
来源：http://qne.0kj1m.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://rtm.fengsongda.top

[R79] 解析命令行选项
来源：http://qcp.redwolf501.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pad.bjfxy.top

[R80] 查看脚本执行耗时
来源：http://lbl.guannengcc.top

time ./run.sh
来源：http://tgf.zhiwuduotai.top

================================================================================
来源：http://lye.sufxvd.cn

S. C / C++ 专题
来源：http://pid.cucudq.cn

================================================================================
来源：http://aln.xingfuxueyuan.xyz

[S01] C：Hello World
来源：http://qyw.chenjidiqi.icu

#include <stdio.h>
来源：http://vdi.yvedp.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://jyh.jinqigufen.top

[S02] C：变量与格式化输出
来源：http://gsv.aizwys.cn

int a = 10; printf("%d\n", a);
来源：http://sjb.andypj.xyz

[S03] C：读入整数
来源：http://exc.yj20258.top

int x; scanf("%d", &x);
来源：http://fey.yj20258888.top

[S04] C：字符串复制
来源：http://xad.tianlin.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://oxx.jinghuilouyu.cn

[S05] C：字符串长度
来源：http://ror.zhijiandao.cn

strlen(s)
来源：http://ydh.nanxuanxn.top

[S06] C：字符串比较
来源：http://twr.ybcxt.top

strcmp(a, b) == 0
来源：http://kdd.chenlongwang.top

[S07] C：数组遍历求和
来源：http://qvt.aibaodan.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xxf.shangyingyoupin.top

[S08] C：动态内存分配与释放
来源：http://crw.vqdsnc.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mlv.pengpengdd.cyou

[S09] C：结构体定义与初始化
来源：http://tzh.sxryk.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fcq.zhengqikj.top

[S10] C：指针与解引用
来源：http://tig.zdqjudy.top

int *p = &a;  *p = 5;
来源：http://qmp.havefunace.top

[S11] C：逐行读文件
来源：http://pkn.xuanzx.com

FILE *f = fopen("a.txt", "r");
来源：http://kgb.ppjwa.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hbg.hcnkem.com

fclose(f);
来源：http://uvw.zhoulong.xyz

[S12] C：写文件
来源：http://ihd.yj202588.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kls.jianghu66.top

[S13] C：宏定义
来源：http://ibg.mhx1999.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cfx.sjlbkw.cn

[S14] C：枚举
来源：http://fky.ctjpmb.com

enum Color { RED, GREEN, BLUE };
来源：http://cmz.jianghu66.top

[S15] C：类型转换
来源：http://ava.yfazqb.com

(double) a / b
来源：http://ewi.nwbrower.top

[S16] C：位操作置位
来源：http://hlk.sufxvd.cn

x |= (1 << 3);
来源：http://qzi.ybcxt.top

[S17] C：安全拼接字符串
来源：http://cwh.yuanzhike.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wbs.jiagoushi.top

[S18] C：命令行参数
来源：http://ike.mhx1999.top

int main(int argc, char **argv)
来源：http://yyt.sweek.top

[S19] C：快速排序
来源：http://nul.yueranfly.top

qsort(a, n, sizeof(int), cmp);
来源：http://vom.kuanghao11.cn

[S20] C：二分查找
来源：http://lko.ppjwa.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tnu.zdbjq.cn

[S21] C：字符类别判断
来源：http://zlb.mhx1999.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dje.shuidangran.top

[S22] C：字符串转数字
来源：http://sst.ydjk.org.cn

atoi("42");  strtod("3.14", NULL);
来源：http://hij.hammf.cn

[S23] C：随机数
来源：http://ffh.yj20258888.top

srand(time(NULL));  int r = rand() % 100;
来源：http://cgs.fanxiaobao.xyz

[S24] C：获取本地时间
来源：http://ivj.zdbjq.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lwp.jinghuilouyu.cn

[S25] C：内存拷贝
来源：http://ikc.dashuyun.cn

memcpy(dst, src, n);
来源：http://gld.jiagoushi.top

[S26] C：内存清零
来源：http://end.jinghuilouyu.cn

memset(a, 0, sizeof a);
来源：http://shn.zhaomingkeji.xyz

[S27] C：定义常量
来源：http://xrk.chenjidiqi.icu

const double PI = 3.14159;
来源：http://kur.cheryme.top

[S28] C：静态变量
来源：http://fdf.zhoulong.xyz

static int counter = 0;
来源：http://rku.jqgufenzy.top

[S29] C：变参函数
来源：http://jzc.shuidangran.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vsj.zycfv.cn

[S30] C：头文件保护
来源：http://ofa.xinyue.icu

#ifndef X_H
来源：http://mxc.gotoacloud.top

#define X_H
来源：http://mzm.gotoacloud.top

#endif
来源：http://jie.wangshuangyany.cn

[S31] C++：Hello World
来源：http://ibt.sufxvd.cn

#include <iostream>
来源：http://ret.jinqigufen.top

int main() { std::cout << "Hello\n"; }
来源：http://kup.ehwqpu.com

[S32] C++：字符串
来源：http://zvk.quarkkingdee.top

std::string s = "hi";  s += "!";
来源：http://lww.xylfe.cn

[S33] C++：vector 增删
来源：http://ezp.snrcjt.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sjw.zhiwuduotai.top

[S34] C++：遍历 vector
来源：http://cxk.hesvh.cn

for (auto &x : v) { std::cout << x; }
来源：http://oil.xinyue.icu

[S35] C++：map
来源：http://ubb.zhoulong.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tam.snrcjt.cn

[S36] C++：unordered_map
来源：http://bcs.snrcjt.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gqv.feifeiyinyue.top

[S37] C++：set
来源：http://wlg.mhx1999.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://oxm.hnqzz.top

[S38] C++：排序
来源：http://gxz.zhijiandao.cn

std::sort(v.begin(), v.end());
来源：http://dwy.shanyushiyangtech.top

[S39] C++：自定义比较器排序
来源：http://dyr.chenlongwang.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ukx.ywan-chungtsiang.top

[S40] C++：查找元素
来源：http://via.chenlongwang.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wef.yangfankeji.com

[S41] C++：类与构造函数
来源：http://jbr.cashguo.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://duf.quarkkingdee.top

[S42] C++：继承与虚函数
来源：http://uli.vqdsnc.cn

class B : public Base { public: void f() override {} };
来源：http://wqf.shanyushiyangkeji.top

[S43] C++：智能指针
来源：http://fgw.jqgufenzy.top

auto p = std::make_unique<int>(5);
来源：http://xwr.chenzaomai.com

[S44] C++：引用传参
来源：http://vxm.hysaishi.cn

void inc(int &x) { ++x; }
来源：http://okw.zdqjudy.top

[S45] C++：lambda
来源：http://vpn.fzhhl.top

auto add = [](int a, int b) { return a + b; };
来源：http://yqc.jianghu66.top

[S46] C++：函数模板
来源：http://lng.haohaochexian.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dny.zhiwuduotai.top

[S47] C++：结构化绑定遍历
来源：http://ahj.jqgfzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mnw.fzhhl.top

[S48] C++：逐行读文件
来源：http://nch.yj20258.top

std::ifstream in("a.txt");  std::string line;
来源：http://ouq.sufxvd.cn

while (std::getline(in, line)) { }
来源：http://xgh.tarul.cn

[S49] C++：写文件
来源：http://plc.havefunace.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rjq.yuxming.cn

[S50] C++：格式化数字
来源：http://jkg.hywenlv.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kag.chenlongwang.top

[S51] C++：显式类型转换
来源：http://brd.chenjidiqi.icu

static_cast<double>(a) / b
来源：http://fpb.havefunace.top

[S52] C++：const 与 noexcept
来源：http://pzw.ivvv.top

int size() const noexcept { return n_; }
来源：http://chv.9152youxi.cn

[S53] C++：移动语义
来源：http://maz.fktsv.cn

std::vector<int> w = std::move(v);
来源：http://oxf.jlsjyb.cn

[S54] C++：异常处理
来源：http://uts.jinqigfzy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xqc.sweek.top

[S55] C++：结构化绑定
来源：http://owp.tarul.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mvl.feifeiyinyue.top

[S56] C++：optional
来源：http://jww.kuanghao11.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xiu.jinqigufen.top

[S57] C++：编译期常量
来源：http://sgh.aibaodan.cn

constexpr int N = 10;
来源：http://qrd.wangshuangyany.cn

[S58] C++：命名空间
来源：http://mhw.cucudq.cn

namespace ns { int f() { return 1; } }
来源：http://ydw.aibaodan.cn

[S59] C++：静态断言
来源：http://noc.sweek.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ehj.jianghu66.top

[S60] C++：遍历并删除元素
来源：http://mit.smart0.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vxu.sufxvd.cn

================================================================================
来源：http://yve.guowangkeji.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zsm.nanxuanxn.top

================================================================================
来源：http://igp.gzhubu.top

[T01] Kotlin：Hello World
来源：http://cov.gzhubu.top

println("Hello")
来源：http://mzi.chenzaomai.com

[T02] Kotlin：变量
来源：http://lwq.ppjwa.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tvu.cqqwz.cn

[T03] Kotlin：字符串模板
来源：http://bmy.shangyingyoupin.top

"值: $b"
来源：http://prx.jqgufenzy.top

[T04] Kotlin：空安全
来源：http://frt.hnqzz.top

val n: String? = null;  n?.length
来源：http://sdj.zdqjudy.top

[T05] Kotlin：when 表达式
来源：http://gry.fzhhl.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jtc.svipenyu.cn

[T06] Kotlin：集合映射
来源：http://kgw.zhaomingkeji.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://jxb.aibaodan.cn

[T07] Kotlin：集合过滤
来源：http://ltq.zhijiandao.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://uqc.jlsjyb.cn

[T08] Kotlin：数据类
来源：http://hrh.jianghu66.top

data class User(val name: String, val age: Int)
来源：http://acz.aibaodan.cn

[T09] Kotlin：扩展函数
来源：http://aka.xinyue.icu

fun String.exclaim() = this + "!"
来源：http://fdh.shanyushiyangtech.top

[T10] Kotlin：默认参数
来源：http://axy.aibaodan.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://sdc.jqgufenzy.top

[T11] Kotlin：协程
来源：http://skc.jqgfzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://vho.hywenlv.cn

[T12] Kotlin：解构声明
来源：http://fqz.tarul.cn

val (a, b) = Pair(1, 2)
来源：http://asb.jiagoushi.top

[T13] Kotlin：只读 Map
来源：http://nnq.daxiang520.top

val m = mapOf("a" to 1)
来源：http://xdy.nanxuanxn.top

[T14] Kotlin：循环
来源：http://syg.uphjek.com

for (i in 1..10) println(i)
来源：http://yli.zhengqikj.top

[T15] Kotlin：接口
来源：http://gwb.zhijiandao.cn

interface Shape { fun area(): Double }
来源：http://dcy.jinqigfzy.top

[T16] Swift：Hello World
来源：http://icy.wangdashe.top

print("Hello")
来源：http://hdd.epnwcf.com

[T17] Swift：变量与常量
来源：http://lih.xuanzx.com

var a = 1;  let b = 2
来源：http://hto.jiagoushi.top

[T18] Swift：字符串插值
来源：http://ejn.svipenyu.cn

"值: \(b)"
来源：http://jda.sjlbkw.cn

[T19] Swift：可选绑定
来源：http://ezl.yongpay.top

if let n = opt { print(n) }
来源：http://upe.xuanzx.com

[T20] Swift：数组操作
来源：http://ghl.yangfankeji.com

var a = [1, 2, 3];  a.append(4)
来源：http://wdk.mhx1999.top

[T21] Swift：遍历
来源：http://zic.jiagoushi.top

for x in a { print(x) }
来源：http://fru.ctjpmb.com

[T22] Swift：字典
来源：http://apr.jiagoushi.top

var d = ["a": 1];  d["b"] = 2
来源：http://hjj.shuidangran.top

[T23] Swift：函数
来源：http://bxq.zhongyouzk.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xcj.nwbrower.top

[T24] Swift：闭包
来源：http://yuy.yonumen.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://uxp.cucudq.cn

[T25] Swift：结构体
来源：http://zht.zdqjudy.top

struct P { var x: Int }
来源：http://ujc.jinqigfzy.top

[T26] Swift：类与重写
来源：http://vod.hywenlv.cn

class A: Base { override func f() {} }
来源：http://pjh.cheryme.top

[T27] Swift：错误处理
来源：http://nue.chenlongwang.top

do { try f() } catch { print(error) }
来源：http://cjv.aizwys.cn

[T28] Swift：枚举
来源：http://rww.nanxinkj.top

enum Color { case red, green }
来源：http://urj.jiagoushi.top

[T29] Swift：guard 提前返回
来源：http://xim.yuanzhike.top

guard let x = opt else { return }
来源：http://kff.52xcode.cn

[T30] Swift：协议
来源：http://jjc.ywan-chungtsiang.top

protocol Shape { func area() -> Double }
来源：http://svg.jianghu66.top

[T31] Lua：Hello World
来源：http://rrr.meibo888.top

print("Hello")
来源：http://scu.tianlin.xyz

[T32] Lua：局部变量
来源：http://wuv.dashuyun.cn

local a = 1
来源：http://ssg.jiagoushi.top

[T33] Lua：表（数组）
来源：http://igh.zhengqikj.top

local t = {1, 2, 3};  t[4] = 4
来源：http://myp.xinyue.icu

[T34] Lua：遍历表
来源：http://djv.guannengcc.top

for i, v in ipairs(t) do print(i, v) end
来源：http://fxw.fzhhl.top

[T35] Lua：字典表
来源：http://sdz.jianghu66.top

local d = { a = 1 };  d.b = 2
来源：http://zgo.bjfxy.top

[T36] Lua：函数
来源：http://dww.aibaodan.cn

function add(a, b) return a + b end
来源：http://lmc.pycfn.com

[T37] Lua：字符串拼接
来源：http://gey.haohaochexian.top

"a" .. "b"
来源：http://okv.tanke756.top

[T38] Lua：条件
来源：http://vnm.hnqzz.top

if x > 0 then print("正") end
来源：http://aaa.quarkkingdee.top

[T39] Lua：模式匹配
来源：http://jsf.yj20258888.top

string.find(s, "%d+")
来源：http://ukx.yj202588.top

[T40] Lua：元表
来源：http://wbh.jinqigfzy.top

setmetatable({}, { __index = base })
来源：http://uhw.ivvv.top

[T41] Perl：Hello World
来源：http://mfg.jyoumei.cn

print "Hello\n";
来源：http://ytz.ydjk.org.cn

[T42] Perl：变量类型
来源：http://fxv.shanyushiyangtech.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://igz.yongpay.top

[T43] Perl：字符串插值
来源：http://twl.havefunace.top

"值: $a"
来源：http://oaa.tanke756.top

[T44] Perl：条件
来源：http://vdj.zhengqikj.top

if ($a > 0) { print "正"; }
来源：http://dah.fanxiaobao.xyz

[T45] Perl：数组遍历
来源：http://cyo.birdmap.top

for my $x (@arr) { print $x; }
来源：http://gqm.zdbjq.cn

[T46] Perl：哈希操作
来源：http://qrx.fzhhl.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mwp.0kj1m.cn

[T47] Perl：正则捕获
来源：http://slh.wangshuangyany.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://bko.yangfankeji.com

[T48] Perl：正则替换
来源：http://pvr.yuxming.cn

$s =~ s/old/new/g;
来源：http://ndk.jqgufenzy.top

[T49] Perl：函数
来源：http://zsm.gzhubu.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xyv.tianlin.xyz

[T50] Perl：逐行读文件
来源：http://dua.zhongyouzk.top

open my $fh, "<", "a.txt" or die $!;
来源：http://vri.havefunace.top

while (my $line = <$fh>) { print $line; }
来源：http://sax.sjlbkw.cn

[T51] Scala：Hello World
来源：http://dbx.yfazqb.com

println("Hello")
来源：http://hfw.pycfn.com

[T52] Scala：变量
来源：http://qvp.fanxiaobao.xyz

val a = 1;  var b = 2
来源：http://dwk.xuetiantiany.cn

[T53] Scala：字符串插值
来源：http://kpw.bbcook.cn

s"值: $b"
来源：http://gbl.gotoacloud.top

[T54] Scala：集合映射
来源：http://blu.shanyushiyangtech.top

List(1, 2, 3).map(_ * 2)
来源：http://jux.ywan-chungtsiang.top

[T55] Scala：集合过滤
来源：http://rok.shzxlz.cn

List(1, 2, 3).filter(_ > 1)
来源：http://piy.shanyushiyangkeji.top

[T56] Scala：样例类
来源：http://ten.nanxuanxn.top

case class User(name: String, age: Int)
来源：http://ezp.jinqigfzy.top

[T57] Scala：模式匹配
来源：http://ouu.iojbl.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://kyk.cheryme.top

[T58] Scala：函数定义
来源：http://xft.zdqjudy.top

def add(a: Int, b: Int): Int = a + b
来源：http://reg.havefunace.top

[T59] Scala：循环
来源：http://abc.9152youxi.cn

for (i <- 1 to 10) println(i)
来源：http://ilj.meibo888.top

[T60] Scala：折叠
来源：http://udy.aizwys.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zel.jinyuanbaomall.cn

================================================================================
来源：http://btt.gaohongyu789.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://edx.jyoumei.cn

================================================================================
来源：http://fac.cucudq.cn

[U01] Py：创建虚拟环境
来源：http://nux.smart0.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://fdb.hammf.cn

[U02] Py：导出 / 安装依赖
来源：http://ctj.xuetiantiany.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://znq.haohaochexian.top

[U03] Py：加载 .env 配置
来源：http://ttw.hongshengwenyu.top

from dotenv import load_dotenv; load_dotenv()
来源：http://qiw.pycfn.com

[U04] Py：变量调试打印
来源：http://zjg.sjlbkw.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vta.redwolf501.top

[U05] Py：列表去重且保序
来源：http://von.tanke756.top

list(dict.fromkeys(arr))
来源：http://qhb.sjlbkw.cn

[U06] Py：合并两个字典
来源：http://wtk.jinyuanbaomall.cn

{**a, **b}
来源：http://gnk.fktsv.cn

[U07] Py：反转字典键值
来源：http://awv.nanxinkj.top

{v: k for k, v in d.items()}
来源：http://rhy.yongpay.top

[U08] Py：展平二维列表
来源：http://tav.andypj.xyz

[y for x in nested for y in x]
来源：http://ppi.daria6918.cn


<!-- 参考信息 -->