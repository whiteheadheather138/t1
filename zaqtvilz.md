代发 wailian999

openssl rand -hex 16
来源：http://vly.sjlbkw.cn

[R68] 计算文件校验值
来源：http://saq.zdqjudy.top

sha256sum a.txt;  md5sum a.txt
来源：http://kci.aizwys.cn

[R69] 生成随机密码
来源：http://sjp.nwbrower.top

head -c 16 /dev/urandom | base64
来源：http://qfi.kuanghao11.cn

[R70] 时间戳与互转
来源：http://fpr.andypj.xyz

date +%s;  date -d @1700000000
来源：http://jwi.mhx1999.top

[R71] 日期格式化
来源：http://mvx.52xcode.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://fcv.guannengcc.top

[R72] 等待端口就绪
来源：http://qvq.andypj.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://xat.shzxlz.cn

[R73] 分割大日志
来源：http://upx.cashguo.top

split -l 1000 big.log part_
来源：http://ode.ctjpmb.com

[R74] 批量重命名
来源：http://ixu.yj202588.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hcy.quarkkingdee.top

[R75] 导出环境变量
来源：http://tlp.birdmap.top

export PATH="$HOME/bin:$PATH"
来源：http://ylx.zhijiandao.cn

[R76] 使用临时文件
来源：http://ayz.tianlin.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bjq.fktsv.cn

[R77] 读取用户输入
来源：http://wbd.tianlin.xyz

read -rp "请输入: " ans
来源：http://hyg.epnwcf.com

[R78] 交互式菜单
来源：http://vfs.yuanzhike.top

select opt in a b c; do echo "$opt"; break; done
来源：http://jcx.vqdsnc.cn

[R79] 解析命令行选项
来源：http://ffv.pengpengdd.cyou

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gdu.sjlbkw.cn

[R80] 查看脚本执行耗时
来源：http://wrv.shangyingyoupin.top

time ./run.sh
来源：http://jei.svipenyu.cn

================================================================================
来源：http://eza.sysykeji.top

S. C / C++ 专题
来源：http://qss.fanxiaobao.xyz

================================================================================
来源：http://wog.wangshuangyany.cn

[S01] C：Hello World
来源：http://qfi.cheryme.top

#include <stdio.h>
来源：http://byq.jqgfzy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://oxt.aizwys.cn

[S02] C：变量与格式化输出
来源：http://ihm.jlsjyb.cn

int a = 10; printf("%d\n", a);
来源：http://qek.yuanzhike.top

[S03] C：读入整数
来源：http://btm.chenjidiqi.icu

int x; scanf("%d", &x);
来源：http://itw.zhoulong.xyz

[S04] C：字符串复制
来源：http://jxj.jianghu66.top

char dst[32]; strcpy(dst, "hi");
来源：http://hth.tarul.cn

[S05] C：字符串长度
来源：http://uuv.zdbjq.cn

strlen(s)
来源：http://hnv.xinyue.icu

[S06] C：字符串比较
来源：http://bca.sysykeji.top

strcmp(a, b) == 0
来源：http://hqw.xziqi.cn

[S07] C：数组遍历求和
来源：http://lpc.yuxming.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ilr.9152youxi.cn

[S08] C：动态内存分配与释放
来源：http://ren.52xcode.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gyu.fengsongda.top

[S09] C：结构体定义与初始化
来源：http://vsw.fktsv.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fne.hysaishi.cn

[S10] C：指针与解引用
来源：http://gqa.ppjwa.cn

int *p = &a;  *p = 5;
来源：http://mpj.haohaochexian.top

[S11] C：逐行读文件
来源：http://uwn.gotoacloud.top

FILE *f = fopen("a.txt", "r");
来源：http://lft.fzhhl.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://lmn.wangdashe.top

fclose(f);
来源：http://xfv.xylfe.cn

[S12] C：写文件
来源：http://yty.ydjk.org.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ssl.meibo888.top

[S13] C：宏定义
来源：http://nmc.yangfankeji.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hoq.haohaochexian.top

[S14] C：枚举
来源：http://xbe.gzhubu.top

enum Color { RED, GREEN, BLUE };
来源：http://bgs.fengsongda.top

[S15] C：类型转换
来源：http://zcj.zhengqikj.top

(double) a / b
来源：http://yhh.daria6918.cn

[S16] C：位操作置位
来源：http://ctu.sweek.top

x |= (1 << 3);
来源：http://ppk.ppjwa.cn

[S17] C：安全拼接字符串
来源：http://trh.smart0.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gkr.zhongyouzk.top

[S18] C：命令行参数
来源：http://vuv.ywan-chungtsiang.top

int main(int argc, char **argv)
来源：http://gaa.cucudq.cn

[S19] C：快速排序
来源：http://lcs.jyoumei.cn

qsort(a, n, sizeof(int), cmp);
来源：http://emv.jlsjyb.cn

[S20] C：二分查找
来源：http://xlv.yj20258.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zzb.zhixingplan.top

[S21] C：字符类别判断
来源：http://ktd.epnwcf.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gtq.jinqigufen.top

[S22] C：字符串转数字
来源：http://dnd.hammf.cn

atoi("42");  strtod("3.14", NULL);
来源：http://adu.ybcxt.top

[S23] C：随机数
来源：http://aty.shzxlz.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://mip.shanyushiyangtech.top

[S24] C：获取本地时间
来源：http://soy.xinyue.icu

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://unr.gzhubu.top

[S25] C：内存拷贝
来源：http://ubl.guowangkeji.top

memcpy(dst, src, n);
来源：http://zhm.shanyushiyangtech.top

[S26] C：内存清零
来源：http://vmc.aizwys.cn

memset(a, 0, sizeof a);
来源：http://qre.xziqi.cn

[S27] C：定义常量
来源：http://hhx.tian-w.cn

const double PI = 3.14159;
来源：http://kau.pycfn.com

[S28] C：静态变量
来源：http://eoc.guowangkeji.top

static int counter = 0;
来源：http://lvv.daria6918.cn

[S29] C：变参函数
来源：http://zqe.jqgufenzy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://umk.ywan-chungtsiang.top

[S30] C：头文件保护
来源：http://agk.nwbrower.top

#ifndef X_H
来源：http://xpe.meibo888.top

#define X_H
来源：http://nzh.yvedp.cn

#endif
来源：http://zuk.vqdsnc.cn

[S31] C++：Hello World
来源：http://une.jinghuilouyu.cn

#include <iostream>
来源：http://xug.fktsv.cn

int main() { std::cout << "Hello\n"; }
来源：http://kmw.ydjk.org.cn

[S32] C++：字符串
来源：http://rsl.fktsv.cn

std::string s = "hi";  s += "!";
来源：http://ssh.zhongyouzk.top

[S33] C++：vector 增删
来源：http://gwz.nanxuanxn.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xma.vehdjk.com

[S34] C++：遍历 vector
来源：http://yvm.shanyushiyangtech.top

for (auto &x : v) { std::cout << x; }
来源：http://ufn.feifeiyinyue.top

[S35] C++：map
来源：http://tgb.jinyuanbaomall.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kxr.aibaodan.cn

[S36] C++：unordered_map
来源：http://ouz.fanxiaobao.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://juk.redwolf501.top

[S37] C++：set
来源：http://urf.zdbjq.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pax.cdnleiting.top

[S38] C++：排序
来源：http://qbs.ybcxt.top

std::sort(v.begin(), v.end());
来源：http://qia.zhixingplan.top

[S39] C++：自定义比较器排序
来源：http://pts.uphjek.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ocp.yuanzhike.top

[S40] C++：查找元素
来源：http://hpu.daria6918.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://utc.fengsongda.top

[S41] C++：类与构造函数
来源：http://ggu.hywenlv.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wiv.mhx1999.top

[S42] C++：继承与虚函数
来源：http://wwj.hongshengwenyu.top

class B : public Base { public: void f() override {} };
来源：http://opm.shuidangran.top

[S43] C++：智能指针
来源：http://kvk.jinqigfzy.top

auto p = std::make_unique<int>(5);
来源：http://tih.gzhubu.top

[S44] C++：引用传参
来源：http://ujg.jyoumei.cn

void inc(int &x) { ++x; }
来源：http://mzg.jyoumei.cn

[S45] C++：lambda
来源：http://bde.ivvv.top

auto add = [](int a, int b) { return a + b; };
来源：http://abq.hfpthk.cn

[S46] C++：函数模板
来源：http://ral.snrcjt.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ynf.hywenlv.cn

[S47] C++：结构化绑定遍历
来源：http://pzl.yj20258.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://isx.daria6918.cn

[S48] C++：逐行读文件
来源：http://wne.zhongyouzk.top

std::ifstream in("a.txt");  std::string line;
来源：http://mzc.9152youxi.cn

while (std::getline(in, line)) { }
来源：http://qei.zhijiandao.cn

[S49] C++：写文件
来源：http://uvn.gogol.net.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://owv.ctjpmb.com

[S50] C++：格式化数字
来源：http://abi.zhengqikj.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wlf.zhoulong.xyz

[S51] C++：显式类型转换
来源：http://vcd.yongpay.top

static_cast<double>(a) / b
来源：http://wao.yongpay.top

[S52] C++：const 与 noexcept
来源：http://abk.daria6918.cn

int size() const noexcept { return n_; }
来源：http://rxg.hammf.cn

[S53] C++：移动语义
来源：http://qck.zhoulong.xyz

std::vector<int> w = std::move(v);
来源：http://mxq.svipenyu.cn

[S54] C++：异常处理
来源：http://lxm.hfpthk.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bff.c1oappe.top

[S55] C++：结构化绑定
来源：http://idk.yj202588.top

auto [a, b] = std::make_pair(1, 2);
来源：http://kgm.bbcook.cn

[S56] C++：optional
来源：http://rpi.chenlongwang.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zeo.hnxiangtu.top

[S57] C++：编译期常量
来源：http://gkl.sysykeji.top

constexpr int N = 10;
来源：http://kiv.hysaishi.cn

[S58] C++：命名空间
来源：http://kaa.yueranfly.top

namespace ns { int f() { return 1; } }
来源：http://oht.tian-w.cn

[S59] C++：静态断言
来源：http://fiz.yonumen.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://etd.yanxiufei.cn

[S60] C++：遍历并删除元素
来源：http://wuj.shzxlz.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qxq.yfazqb.com

================================================================================
来源：http://ivv.yongpay.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mxh.0kj1m.cn

================================================================================
来源：http://mfb.c1oappe.top

[T01] Kotlin：Hello World
来源：http://sqs.zdbjq.cn

println("Hello")
来源：http://xjg.ywan-chungtsiang.top

[T02] Kotlin：变量
来源：http://ges.sweek.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yno.zhengqikj.top

[T03] Kotlin：字符串模板
来源：http://aue.gotoacloud.top

"值: $b"
来源：http://bfh.hammf.cn

[T04] Kotlin：空安全
来源：http://jwp.yangfankeji.com

val n: String? = null;  n?.length
来源：http://npg.yuanzhike.top

[T05] Kotlin：when 表达式
来源：http://hke.sysykeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ujf.cqqwz.cn

[T06] Kotlin：集合映射
来源：http://wkw.jinghuilouyu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hxo.nanxinkj.top

[T07] Kotlin：集合过滤
来源：http://unw.yfazqb.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://wjw.shanyushiyangtech.top

[T08] Kotlin：数据类
来源：http://pho.hywenlv.cn

data class User(val name: String, val age: Int)
来源：http://jcd.316326.xyz

[T09] Kotlin：扩展函数
来源：http://pqc.fktsv.cn

fun String.exclaim() = this + "!"
来源：http://rke.andypj.xyz

[T10] Kotlin：默认参数
来源：http://jbd.fehbvm.com

fun greet(name: String = "World") = "Hi $name"
来源：http://oej.yfazqb.com

[T11] Kotlin：协程
来源：http://xai.jqgufenzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://mkk.jinqigfzy.top

[T12] Kotlin：解构声明
来源：http://huo.shangyingyoupin.top

val (a, b) = Pair(1, 2)
来源：http://uwx.yuxming.cn

[T13] Kotlin：只读 Map
来源：http://dcw.tanke756.top

val m = mapOf("a" to 1)
来源：http://gfs.dashuyun.cn

[T14] Kotlin：循环
来源：http://lne.52xcode.cn

for (i in 1..10) println(i)
来源：http://bkp.jinghuilouyu.cn

[T15] Kotlin：接口
来源：http://cox.cqqwz.cn

interface Shape { fun area(): Double }
来源：http://qdz.chenlongwang.top

[T16] Swift：Hello World
来源：http://tde.jqgfzy.top

print("Hello")
来源：http://nzy.jinqigfzy.top

[T17] Swift：变量与常量
来源：http://ppj.vqdsnc.cn

var a = 1;  let b = 2
来源：http://ncn.ivvv.top

[T18] Swift：字符串插值
来源：http://wsj.daria6918.cn

"值: \(b)"
来源：http://aen.fzhhl.top

[T19] Swift：可选绑定
来源：http://qga.hysaishi.cn

if let n = opt { print(n) }
来源：http://vto.chenlongwang.top

[T20] Swift：数组操作
来源：http://pek.hfpthk.cn

var a = [1, 2, 3];  a.append(4)
来源：http://rnr.iojbl.cn

[T21] Swift：遍历
来源：http://vso.jqgufenzy.top

for x in a { print(x) }
来源：http://oil.ydzc1.top

[T22] Swift：字典
来源：http://ndz.xuetiantiany.cn

var d = ["a": 1];  d["b"] = 2
来源：http://tzu.tanke756.top

[T23] Swift：函数
来源：http://qmc.yj20258.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pgq.pengpengdd.cyou

[T24] Swift：闭包
来源：http://zpx.chenzaomai.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://uvm.gaohongyu789.top

[T25] Swift：结构体
来源：http://wym.shanyushiyangkeji.top

struct P { var x: Int }
来源：http://nzo.jinghuilouyu.cn

[T26] Swift：类与重写
来源：http://lud.hywenlv.cn

class A: Base { override func f() {} }
来源：http://ejr.fktsv.cn

[T27] Swift：错误处理
来源：http://yav.ydjk.org.cn

do { try f() } catch { print(error) }
来源：http://inc.iojbl.cn

[T28] Swift：枚举
来源：http://ucq.316326.xyz

enum Color { case red, green }
来源：http://tap.yj20258888.top

[T29] Swift：guard 提前返回
来源：http://xsa.hongshengwenyu.top

guard let x = opt else { return }
来源：http://ibf.yj20258.top

[T30] Swift：协议
来源：http://ojl.yonumen.top

protocol Shape { func area() -> Double }
来源：http://wop.nanxinkj.top

[T31] Lua：Hello World
来源：http://ifn.9152youxi.cn

print("Hello")
来源：http://vnb.quarkkingdee.top

[T32] Lua：局部变量
来源：http://yyf.daxiang520.top

local a = 1
来源：http://oco.chenlongwang.top

[T33] Lua：表（数组）
来源：http://xlr.dashuyun.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://tcy.dashuyun.cn

[T34] Lua：遍历表
来源：http://vlg.jqgfzy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://yds.cheryme.top

[T35] Lua：字典表
来源：http://seu.xinyue.icu

local d = { a = 1 };  d.b = 2
来源：http://rhr.cdnleiting.top

[T36] Lua：函数
来源：http://acm.tian-w.cn

function add(a, b) return a + b end
来源：http://fgh.tanke756.top

[T37] Lua：字符串拼接
来源：http://vzz.tanke756.top

"a" .. "b"
来源：http://cdg.quarkkingdee.top

[T38] Lua：条件
来源：http://fol.ivvv.top

if x > 0 then print("正") end
来源：http://mbv.nanxuanxn.top

[T39] Lua：模式匹配
来源：http://xoy.tanke756.top

string.find(s, "%d+")
来源：http://sbk.yvedp.cn

[T40] Lua：元表
来源：http://xhv.ywan-chungtsiang.top

setmetatable({}, { __index = base })
来源：http://rov.yongpay.top

[T41] Perl：Hello World
来源：http://afr.zdbjq.cn

print "Hello\n";
来源：http://ocd.bbcook.cn

[T42] Perl：变量类型
来源：http://gyb.guannengcc.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ibe.redwolf501.top

[T43] Perl：字符串插值
来源：http://zqj.bbcook.cn

"值: $a"
来源：http://mvd.zhixingplan.top

[T44] Perl：条件
来源：http://khl.hnxiangtu.top

if ($a > 0) { print "正"; }
来源：http://tcj.zycfv.cn

[T45] Perl：数组遍历
来源：http://lrc.haohaochexian.top

for my $x (@arr) { print $x; }
来源：http://tfy.cashguo.top

[T46] Perl：哈希操作
来源：http://gsb.cheryme.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pjb.yj20258.top

[T47] Perl：正则捕获
来源：http://xam.zhiwuduotai.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://fsr.xuetiantiany.cn

[T48] Perl：正则替换
来源：http://teo.haohaochexian.top

$s =~ s/old/new/g;
来源：http://yro.sysykeji.top

[T49] Perl：函数
来源：http://wfw.sxryk.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vwg.sjlbkw.cn

[T50] Perl：逐行读文件
来源：http://gfi.feifeiyinyue.top

open my $fh, "<", "a.txt" or die $!;
来源：http://kzl.jinghuilouyu.cn

while (my $line = <$fh>) { print $line; }
来源：http://sta.nanxuanxn.top

[T51] Scala：Hello World
来源：http://iua.jinghuilouyu.cn

println("Hello")
来源：http://tbv.hcnkem.com

[T52] Scala：变量
来源：http://zqp.iojbl.cn

val a = 1;  var b = 2
来源：http://udw.chenzaomai.com

[T53] Scala：字符串插值
来源：http://peg.zhaomingkeji.xyz

s"值: $b"
来源：http://kcu.fehbvm.com

[T54] Scala：集合映射
来源：http://kxz.shuidangran.top

List(1, 2, 3).map(_ * 2)
来源：http://osg.haohaochexian.top

[T55] Scala：集合过滤
来源：http://xuy.yj20258888.top

List(1, 2, 3).filter(_ > 1)
来源：http://rpk.yuxming.cn

[T56] Scala：样例类
来源：http://ghp.gotoacloud.top

case class User(name: String, age: Int)
来源：http://yvp.hfpthk.cn

[T57] Scala：模式匹配
来源：http://lqy.jiagoushi.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://yoy.tian-w.cn

[T58] Scala：函数定义
来源：http://lav.kuanghao11.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zod.shangyingyoupin.top

[T59] Scala：循环
来源：http://lsr.tanke756.top

for (i <- 1 to 10) println(i)
来源：http://gis.snrcjt.cn

[T60] Scala：折叠
来源：http://dbr.jinyuanbaomall.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wkq.tianlin.xyz

================================================================================
来源：http://rck.hywenlv.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hix.gzhubu.top

================================================================================
来源：http://haf.jianghu66.top

[U01] Py：创建虚拟环境
来源：http://lwk.jinqigufen.top

python -m venv .venv && source .venv/bin/activate
来源：http://tvp.ppjwa.cn

[U02] Py：导出 / 安装依赖
来源：http://nan.yueranfly.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fvw.chenlongwang.top

[U03] Py：加载 .env 配置
来源：http://dth.quarkkingdee.top

from dotenv import load_dotenv; load_dotenv()
来源：http://vph.vehdjk.com

[U04] Py：变量调试打印
来源：http://zsp.ppjwa.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://njc.jyoumei.cn

[U05] Py：列表去重且保序
来源：http://mgo.epnwcf.com

list(dict.fromkeys(arr))
来源：http://hvh.haohaochexian.top

[U06] Py：合并两个字典
来源：http://cow.yvedp.cn

{**a, **b}
来源：http://dui.havefunace.top

[U07] Py：反转字典键值
来源：http://cwg.sjlbkw.cn

{v: k for k, v in d.items()}
来源：http://nts.jianghu66.top

[U08] Py：展平二维列表
来源：http://wgo.svipenyu.cn

[y for x in nested for y in x]
来源：http://xij.aizwys.cn


<!-- 参考信息 -->