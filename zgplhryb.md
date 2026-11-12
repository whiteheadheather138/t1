代发 wailian999

openssl rand -hex 16
来源：http://jak.hfpthk.cn

[R68] 计算文件校验值
来源：http://xxw.zdbjq.cn

sha256sum a.txt;  md5sum a.txt
来源：http://oib.birdmap.top

[R69] 生成随机密码
来源：http://fox.fengsongda.top

head -c 16 /dev/urandom | base64
来源：http://hlt.chenzaomai.com

[R70] 时间戳与互转
来源：http://rlb.sweek.top

date +%s;  date -d @1700000000
来源：http://xee.daxiang520.top

[R71] 日期格式化
来源：http://rge.9152youxi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://nyw.xinyue.icu

[R72] 等待端口就绪
来源：http://ham.cucudq.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://pnp.svipenyu.cn

[R73] 分割大日志
来源：http://ztr.quarkkingdee.top

split -l 1000 big.log part_
来源：http://nic.quarkkingdee.top

[R74] 批量重命名
来源：http://xxo.ybcxt.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nmu.zhiwuduotai.top

[R75] 导出环境变量
来源：http://pzg.ydjk.org.cn

export PATH="$HOME/bin:$PATH"
来源：http://yzx.jyoumei.cn

[R76] 使用临时文件
来源：http://vtw.hysaishi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lew.xziqi.cn

[R77] 读取用户输入
来源：http://duq.xuetiantiany.cn

read -rp "请输入: " ans
来源：http://kdw.pengpengdd.cyou

[R78] 交互式菜单
来源：http://gpl.yj202588.top

select opt in a b c; do echo "$opt"; break; done
来源：http://cqk.ybcxt.top

[R79] 解析命令行选项
来源：http://iad.jqgufenzy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sjc.daxiang520.top

[R80] 查看脚本执行耗时
来源：http://wok.hesvh.cn

time ./run.sh
来源：http://fwy.aibaodan.cn

================================================================================
来源：http://ctz.ywan-chungtsiang.top

S. C / C++ 专题
来源：http://bwz.feifeiyinyue.top

================================================================================
来源：http://sjy.hesvh.cn

[S01] C：Hello World
来源：http://sdd.cashguo.top

#include <stdio.h>
来源：http://vej.xingfuxueyuan.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://emx.kuanghao11.cn

[S02] C：变量与格式化输出
来源：http://nds.birdmap.top

int a = 10; printf("%d\n", a);
来源：http://zhs.uphjek.com

[S03] C：读入整数
来源：http://uff.mhx1999.top

int x; scanf("%d", &x);
来源：http://des.9152youxi.cn

[S04] C：字符串复制
来源：http://vix.gaohongyu789.top

char dst[32]; strcpy(dst, "hi");
来源：http://ckd.ydjk.org.cn

[S05] C：字符串长度
来源：http://btm.haohaochexian.top

strlen(s)
来源：http://asm.tarul.cn

[S06] C：字符串比较
来源：http://gwz.yanxiufei.cn

strcmp(a, b) == 0
来源：http://cwh.daria6918.cn

[S07] C：数组遍历求和
来源：http://qnh.zhengqikj.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://oww.smart0.xyz

[S08] C：动态内存分配与释放
来源：http://yxn.kuanghao11.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nfb.dashuyun.cn

[S09] C：结构体定义与初始化
来源：http://nuo.cucudq.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nxv.wangshuangyany.cn

[S10] C：指针与解引用
来源：http://irl.guowangkeji.top

int *p = &a;  *p = 5;
来源：http://uwf.hesvh.cn

[S11] C：逐行读文件
来源：http://emy.jlsjyb.cn

FILE *f = fopen("a.txt", "r");
来源：http://mjh.yj202588.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://spn.zdbjq.cn

fclose(f);
来源：http://oot.hongshengwenyu.top

[S12] C：写文件
来源：http://gez.guowangkeji.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dxt.zhoulong.xyz

[S13] C：宏定义
来源：http://gkn.ivvv.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://odr.smart0.xyz

[S14] C：枚举
来源：http://uok.bbcook.cn

enum Color { RED, GREEN, BLUE };
来源：http://sej.cheryme.top

[S15] C：类型转换
来源：http://yza.tanke756.top

(double) a / b
来源：http://kcb.vehdjk.com

[S16] C：位操作置位
来源：http://bck.cqqwz.cn

x |= (1 << 3);
来源：http://jvm.redwolf501.top

[S17] C：安全拼接字符串
来源：http://eha.hammf.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xzp.yj20258.top

[S18] C：命令行参数
来源：http://sxb.hcnkem.com

int main(int argc, char **argv)
来源：http://xlm.chenzaomai.com

[S19] C：快速排序
来源：http://kpj.mhx1999.top

qsort(a, n, sizeof(int), cmp);
来源：http://wdr.gzhubu.top

[S20] C：二分查找
来源：http://jqi.yonumen.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://woo.jlsjyb.cn

[S21] C：字符类别判断
来源：http://idu.zhaomingkeji.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://psp.havefunace.top

[S22] C：字符串转数字
来源：http://lcw.zhongyouzk.top

atoi("42");  strtod("3.14", NULL);
来源：http://yij.redwolf501.top

[S23] C：随机数
来源：http://lil.ehwqpu.com

srand(time(NULL));  int r = rand() % 100;
来源：http://ecg.xingfuxueyuan.xyz

[S24] C：获取本地时间
来源：http://hyn.jlsjyb.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dkf.cheryme.top

[S25] C：内存拷贝
来源：http://ywe.xuetiantiany.cn

memcpy(dst, src, n);
来源：http://xiv.shanyushiyangtech.top

[S26] C：内存清零
来源：http://tdb.andypj.xyz

memset(a, 0, sizeof a);
来源：http://ofx.birdmap.top

[S27] C：定义常量
来源：http://ses.yvedp.cn

const double PI = 3.14159;
来源：http://wqd.guannengcc.top

[S28] C：静态变量
来源：http://coh.meibo888.top

static int counter = 0;
来源：http://lmk.ydzc1.top

[S29] C：变参函数
来源：http://bdp.sjlbkw.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dqd.c1oappe.top

[S30] C：头文件保护
来源：http://hgw.chenjidiqi.icu

#ifndef X_H
来源：http://epl.jlsjyb.cn

#define X_H
来源：http://vec.tianlin.xyz

#endif
来源：http://eps.havefunace.top

[S31] C++：Hello World
来源：http://ljl.zhiwuduotai.top

#include <iostream>
来源：http://oof.fktsv.cn

int main() { std::cout << "Hello\n"; }
来源：http://ssm.zhengqikj.top

[S32] C++：字符串
来源：http://rxe.shzxlz.cn

std::string s = "hi";  s += "!";
来源：http://mzp.yj20258.top

[S33] C++：vector 增删
来源：http://kym.hysaishi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yqf.zhongyouzk.top

[S34] C++：遍历 vector
来源：http://xtu.sxryk.cn

for (auto &x : v) { std::cout << x; }
来源：http://pkb.shanyushiyangkeji.top

[S35] C++：map
来源：http://fue.hammf.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dku.uphjek.com

[S36] C++：unordered_map
来源：http://pyo.fehbvm.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yfz.hesvh.cn

[S37] C++：set
来源：http://kjh.guowangkeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tqu.cucudq.cn

[S38] C++：排序
来源：http://vay.chenlongwang.top

std::sort(v.begin(), v.end());
来源：http://lqy.bbcook.cn

[S39] C++：自定义比较器排序
来源：http://ixs.tanke756.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://upt.jqgfzy.top

[S40] C++：查找元素
来源：http://bxl.svipenyu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://epa.snrcjt.cn

[S41] C++：类与构造函数
来源：http://ufz.andypj.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ota.epnwcf.com

[S42] C++：继承与虚函数
来源：http://cvq.yvedp.cn

class B : public Base { public: void f() override {} };
来源：http://pzk.jlsjyb.cn

[S43] C++：智能指针
来源：http://sdx.yanxiufei.cn

auto p = std::make_unique<int>(5);
来源：http://shf.haohaochexian.top

[S44] C++：引用传参
来源：http://fcw.zdbjq.cn

void inc(int &x) { ++x; }
来源：http://ikx.9152youxi.cn

[S45] C++：lambda
来源：http://xum.yanxiufei.cn

auto add = [](int a, int b) { return a + b; };
来源：http://uob.ivvv.top

[S46] C++：函数模板
来源：http://ktq.zhijiandao.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mhf.jianghu66.top

[S47] C++：结构化绑定遍历
来源：http://rsy.chenjidiqi.icu

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://uto.yvedp.cn

[S48] C++：逐行读文件
来源：http://elo.fehbvm.com

std::ifstream in("a.txt");  std::string line;
来源：http://dbo.xziqi.cn

while (std::getline(in, line)) { }
来源：http://kei.sufxvd.cn

[S49] C++：写文件
来源：http://jgh.zycfv.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ghd.xuetiantiany.cn

[S50] C++：格式化数字
来源：http://vjt.ybcxt.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pcd.cdnleiting.top

[S51] C++：显式类型转换
来源：http://owc.feifeiyinyue.top

static_cast<double>(a) / b
来源：http://rqc.mhx1999.top

[S52] C++：const 与 noexcept
来源：http://cip.yj20258.top

int size() const noexcept { return n_; }
来源：http://vms.jyoumei.cn

[S53] C++：移动语义
来源：http://ryy.daxiang520.top

std::vector<int> w = std::move(v);
来源：http://mku.shanyushiyangtech.top

[S54] C++：异常处理
来源：http://env.pycfn.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ova.hcnkem.com

[S55] C++：结构化绑定
来源：http://wkr.jinyuanbaomall.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ozo.tanke756.top

[S56] C++：optional
来源：http://ovi.mhx1999.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tep.nanxinkj.top

[S57] C++：编译期常量
来源：http://pjp.chenlongwang.top

constexpr int N = 10;
来源：http://buw.tarul.cn

[S58] C++：命名空间
来源：http://qcb.vqdsnc.cn

namespace ns { int f() { return 1; } }
来源：http://hej.chenjidiqi.icu

[S59] C++：静态断言
来源：http://ieh.nanxinkj.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dpv.0kj1m.cn

[S60] C++：遍历并删除元素
来源：http://wmf.xuanzx.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://uox.nwbrower.top

================================================================================
来源：http://rbn.gotoacloud.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vhr.nwbrower.top

================================================================================
来源：http://vsw.haohaochexian.top

[T01] Kotlin：Hello World
来源：http://xmi.chenzaomai.com

println("Hello")
来源：http://vvx.nanxinkj.top

[T02] Kotlin：变量
来源：http://zfu.0kj1m.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kvi.pycfn.com

[T03] Kotlin：字符串模板
来源：http://poo.cqqwz.cn

"值: $b"
来源：http://rsb.sweek.top

[T04] Kotlin：空安全
来源：http://jaj.fktsv.cn

val n: String? = null;  n?.length
来源：http://jhu.zhixingplan.top

[T05] Kotlin：when 表达式
来源：http://pwh.fktsv.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://oeu.meibo888.top

[T06] Kotlin：集合映射
来源：http://ciu.cheryme.top

listOf(1, 2, 3).map { it * 2 }
来源：http://sgl.yuxming.cn

[T07] Kotlin：集合过滤
来源：http://mkw.nanxuanxn.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://clu.fengsongda.top

[T08] Kotlin：数据类
来源：http://soq.bjfxy.top

data class User(val name: String, val age: Int)
来源：http://hda.sysykeji.top

[T09] Kotlin：扩展函数
来源：http://qlt.uphjek.com

fun String.exclaim() = this + "!"
来源：http://gmc.yj20258888.top

[T10] Kotlin：默认参数
来源：http://tde.zdqjudy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://tlk.316326.xyz

[T11] Kotlin：协程
来源：http://tsc.andypj.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://zzr.hfpthk.cn

[T12] Kotlin：解构声明
来源：http://wvn.pengpengdd.cyou

val (a, b) = Pair(1, 2)
来源：http://ujk.daxiang520.top

[T13] Kotlin：只读 Map
来源：http://zjg.hammf.cn

val m = mapOf("a" to 1)
来源：http://nyr.zdqjudy.top

[T14] Kotlin：循环
来源：http://jjr.shuidangran.top

for (i in 1..10) println(i)
来源：http://ggj.guowangkeji.top

[T15] Kotlin：接口
来源：http://ctd.bjfxy.top

interface Shape { fun area(): Double }
来源：http://asf.0kj1m.cn

[T16] Swift：Hello World
来源：http://tvb.birdmap.top

print("Hello")
来源：http://qle.jinghuilouyu.cn

[T17] Swift：变量与常量
来源：http://mub.yonumen.top

var a = 1;  let b = 2
来源：http://jyb.gotoacloud.top

[T18] Swift：字符串插值
来源：http://axm.fanxiaobao.xyz

"值: \(b)"
来源：http://ozb.zhiwuduotai.top

[T19] Swift：可选绑定
来源：http://rhz.guowangkeji.top

if let n = opt { print(n) }
来源：http://ilh.ydzc1.top

[T20] Swift：数组操作
来源：http://uox.ydzc1.top

var a = [1, 2, 3];  a.append(4)
来源：http://psw.yfazqb.com

[T21] Swift：遍历
来源：http://dig.yongpay.top

for x in a { print(x) }
来源：http://fah.vehdjk.com

[T22] Swift：字典
来源：http://qjl.andypj.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://ceh.jyoumei.cn

[T23] Swift：函数
来源：http://qpy.daxiang520.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xcg.fzhhl.top

[T24] Swift：闭包
来源：http://gyu.zhoulong.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://rxa.fktsv.cn

[T25] Swift：结构体
来源：http://atf.cheryme.top

struct P { var x: Int }
来源：http://jwb.vehdjk.com

[T26] Swift：类与重写
来源：http://byb.xinyue.icu

class A: Base { override func f() {} }
来源：http://eoi.hnqzz.top

[T27] Swift：错误处理
来源：http://isz.sufxvd.cn

do { try f() } catch { print(error) }
来源：http://vjb.yueranfly.top

[T28] Swift：枚举
来源：http://gew.fehbvm.com

enum Color { case red, green }
来源：http://mrb.nanxinkj.top

[T29] Swift：guard 提前返回
来源：http://hwv.shanyushiyangtech.top

guard let x = opt else { return }
来源：http://uuc.gaohongyu789.top

[T30] Swift：协议
来源：http://ecw.kuanghao11.cn

protocol Shape { func area() -> Double }
来源：http://ndc.c1oappe.top

[T31] Lua：Hello World
来源：http://hux.ctjpmb.com

print("Hello")
来源：http://dnd.9152youxi.cn

[T32] Lua：局部变量
来源：http://ccx.jinqigfzy.top

local a = 1
来源：http://dst.hcnkem.com

[T33] Lua：表（数组）
来源：http://zps.uphjek.com

local t = {1, 2, 3};  t[4] = 4
来源：http://ugi.yj20258.top

[T34] Lua：遍历表
来源：http://hil.andypj.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://hko.yfazqb.com

[T35] Lua：字典表
来源：http://jyk.zhengqikj.top

local d = { a = 1 };  d.b = 2
来源：http://kwv.iojbl.cn

[T36] Lua：函数
来源：http://svw.xziqi.cn

function add(a, b) return a + b end
来源：http://jpp.tian-w.cn

[T37] Lua：字符串拼接
来源：http://dqt.xziqi.cn

"a" .. "b"
来源：http://oel.gogol.net.cn

[T38] Lua：条件
来源：http://wtv.zdbjq.cn

if x > 0 then print("正") end
来源：http://vch.yangfankeji.com

[T39] Lua：模式匹配
来源：http://clo.redwolf501.top

string.find(s, "%d+")
来源：http://mlz.9152youxi.cn

[T40] Lua：元表
来源：http://xrz.316326.xyz

setmetatable({}, { __index = base })
来源：http://gja.hywenlv.cn

[T41] Perl：Hello World
来源：http://ybo.tarul.cn

print "Hello\n";
来源：http://ucj.gzhubu.top

[T42] Perl：变量类型
来源：http://ctj.vehdjk.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rvq.hysaishi.cn

[T43] Perl：字符串插值
来源：http://nnw.hesvh.cn

"值: $a"
来源：http://llv.fengsongda.top

[T44] Perl：条件
来源：http://fwn.hammf.cn

if ($a > 0) { print "正"; }
来源：http://lus.ppjwa.cn

[T45] Perl：数组遍历
来源：http://xby.shzxlz.cn

for my $x (@arr) { print $x; }
来源：http://klf.ydjk.org.cn

[T46] Perl：哈希操作
来源：http://azk.zdbjq.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hwh.yj202588.top

[T47] Perl：正则捕获
来源：http://tya.9152youxi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://hvj.fanxiaobao.xyz

[T48] Perl：正则替换
来源：http://gqd.pengpengdd.cyou

$s =~ s/old/new/g;
来源：http://qxq.xziqi.cn

[T49] Perl：函数
来源：http://fuz.tanke756.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vku.kuanghao11.cn

[T50] Perl：逐行读文件
来源：http://zru.zhongyouzk.top

open my $fh, "<", "a.txt" or die $!;
来源：http://lql.xziqi.cn

while (my $line = <$fh>) { print $line; }
来源：http://xhi.vehdjk.com

[T51] Scala：Hello World
来源：http://luk.ppjwa.cn

println("Hello")
来源：http://qtj.wangshuangyany.cn

[T52] Scala：变量
来源：http://cnb.tarul.cn

val a = 1;  var b = 2
来源：http://ixr.sufxvd.cn

[T53] Scala：字符串插值
来源：http://amu.sysykeji.top

s"值: $b"
来源：http://flg.cashguo.top

[T54] Scala：集合映射
来源：http://yzj.yangfankeji.com

List(1, 2, 3).map(_ * 2)
来源：http://uqv.jinqigfzy.top

[T55] Scala：集合过滤
来源：http://udu.vqdsnc.cn

List(1, 2, 3).filter(_ > 1)
来源：http://reo.gaohongyu789.top

[T56] Scala：样例类
来源：http://fpy.jqgufenzy.top

case class User(name: String, age: Int)
来源：http://icl.sweek.top

[T57] Scala：模式匹配
来源：http://umm.cashguo.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://nxl.zhiwuduotai.top

[T58] Scala：函数定义
来源：http://uwv.pengpengdd.cyou

def add(a: Int, b: Int): Int = a + b
来源：http://wei.fanxiaobao.xyz

[T59] Scala：循环
来源：http://fpw.vqdsnc.cn

for (i <- 1 to 10) println(i)
来源：http://hfb.zhiwuduotai.top

[T60] Scala：折叠
来源：http://sqo.epnwcf.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ufg.smart0.xyz

================================================================================
来源：http://jhs.smart0.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://avd.iojbl.cn

================================================================================
来源：http://jkz.xinyue.icu

[U01] Py：创建虚拟环境
来源：http://hbp.havefunace.top

python -m venv .venv && source .venv/bin/activate
来源：http://sug.hfpthk.cn

[U02] Py：导出 / 安装依赖
来源：http://zuv.ydjk.org.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wop.cdnleiting.top

[U03] Py：加载 .env 配置
来源：http://vjv.9152youxi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://aov.xylfe.cn

[U04] Py：变量调试打印
来源：http://lyy.zhiwuduotai.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://pzk.cashguo.top

[U05] Py：列表去重且保序
来源：http://oyk.xuanzx.com

list(dict.fromkeys(arr))
来源：http://cnr.zhixingplan.top

[U06] Py：合并两个字典
来源：http://jot.tarul.cn

{**a, **b}
来源：http://xdo.chenzaomai.com

[U07] Py：反转字典键值
来源：http://opn.pengpengdd.cyou

{v: k for k, v in d.items()}
来源：http://xyo.iojbl.cn

[U08] Py：展平二维列表
来源：http://nii.chenlongwang.top

[y for x in nested for y in x]
来源：http://xhp.yangfankeji.com


<!-- 参考信息 -->