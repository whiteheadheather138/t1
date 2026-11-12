代发 wailian999

openssl rand -hex 16
来源：http://aio.cqqwz.cn

[R68] 计算文件校验值
来源：http://bzr.ydzc1.top

sha256sum a.txt;  md5sum a.txt
来源：http://prl.chenlongwang.top

[R69] 生成随机密码
来源：http://crn.jinghuilouyu.cn

head -c 16 /dev/urandom | base64
来源：http://uio.jinghuilouyu.cn

[R70] 时间戳与互转
来源：http://hua.jinyuanbaomall.cn

date +%s;  date -d @1700000000
来源：http://ugl.hammf.cn

[R71] 日期格式化
来源：http://ihx.zhaomingkeji.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://uih.fengsongda.top

[R72] 等待端口就绪
来源：http://vzc.cashguo.top

until nc -z localhost 3306; do sleep 1; done
来源：http://qkq.ehwqpu.com

[R73] 分割大日志
来源：http://bfo.xinyue.icu

split -l 1000 big.log part_
来源：http://juh.aibaodan.cn

[R74] 批量重命名
来源：http://grs.hammf.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://slb.ydjk.org.cn

[R75] 导出环境变量
来源：http://xzg.pengpengdd.cyou

export PATH="$HOME/bin:$PATH"
来源：http://xos.yanxiufei.cn

[R76] 使用临时文件
来源：http://jqv.wangshuangyany.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dkr.meibo888.top

[R77] 读取用户输入
来源：http://cfm.zycfv.cn

read -rp "请输入: " ans
来源：http://mni.xuetiantiany.cn

[R78] 交互式菜单
来源：http://fom.cucudq.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://poc.nanxinkj.top

[R79] 解析命令行选项
来源：http://oyp.sjlbkw.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nih.pycfn.com

[R80] 查看脚本执行耗时
来源：http://jrf.chenzaomai.com

time ./run.sh
来源：http://prn.shanyushiyangtech.top

================================================================================
来源：http://vfj.birdmap.top

S. C / C++ 专题
来源：http://igl.nanxuanxn.top

================================================================================
来源：http://osi.yj202588.top

[S01] C：Hello World
来源：http://ket.ydjk.org.cn

#include <stdio.h>
来源：http://rvv.hywenlv.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://dfc.redwolf501.top

[S02] C：变量与格式化输出
来源：http://zkk.snrcjt.cn

int a = 10; printf("%d\n", a);
来源：http://kil.9152youxi.cn

[S03] C：读入整数
来源：http://bbv.chenlongwang.top

int x; scanf("%d", &x);
来源：http://fsl.zhixingplan.top

[S04] C：字符串复制
来源：http://iwd.pengpengdd.cyou

char dst[32]; strcpy(dst, "hi");
来源：http://dbl.feifeiyinyue.top

[S05] C：字符串长度
来源：http://joa.hesvh.cn

strlen(s)
来源：http://iwi.316326.xyz

[S06] C：字符串比较
来源：http://pfx.cqqwz.cn

strcmp(a, b) == 0
来源：http://pyf.yj20258888.top

[S07] C：数组遍历求和
来源：http://kvj.tarul.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://agf.zycfv.cn

[S08] C：动态内存分配与释放
来源：http://vhv.smart0.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://asi.316326.xyz

[S09] C：结构体定义与初始化
来源：http://qtr.52xcode.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xhr.pycfn.com

[S10] C：指针与解引用
来源：http://mod.9152youxi.cn

int *p = &a;  *p = 5;
来源：http://wsd.jinqigfzy.top

[S11] C：逐行读文件
来源：http://jbd.ydjk.org.cn

FILE *f = fopen("a.txt", "r");
来源：http://gik.xingfuxueyuan.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://odh.yuxming.cn

fclose(f);
来源：http://qdf.sjlbkw.cn

[S12] C：写文件
来源：http://rhk.jqgfzy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ptu.daxiang520.top

[S13] C：宏定义
来源：http://qta.sweek.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cwi.smart0.xyz

[S14] C：枚举
来源：http://snz.kuanghao11.cn

enum Color { RED, GREEN, BLUE };
来源：http://trn.xingfuxueyuan.xyz

[S15] C：类型转换
来源：http://tif.gaohongyu789.top

(double) a / b
来源：http://zjy.tian-w.cn

[S16] C：位操作置位
来源：http://qlp.xuanzx.com

x |= (1 << 3);
来源：http://lzs.jiagoushi.top

[S17] C：安全拼接字符串
来源：http://ivg.tian-w.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xnr.yuxming.cn

[S18] C：命令行参数
来源：http://wdg.daria6918.cn

int main(int argc, char **argv)
来源：http://qla.nanxinkj.top

[S19] C：快速排序
来源：http://jah.sjlbkw.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qmt.chenlongwang.top

[S20] C：二分查找
来源：http://dta.sxryk.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ufg.hfpthk.cn

[S21] C：字符类别判断
来源：http://dtb.ydzc1.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ixu.gaohongyu789.top

[S22] C：字符串转数字
来源：http://cpm.gzhubu.top

atoi("42");  strtod("3.14", NULL);
来源：http://ada.52xcode.cn

[S23] C：随机数
来源：http://ryv.xziqi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://jaz.316326.xyz

[S24] C：获取本地时间
来源：http://ehk.fehbvm.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://agl.316326.xyz

[S25] C：内存拷贝
来源：http://eri.cashguo.top

memcpy(dst, src, n);
来源：http://myk.fzhhl.top

[S26] C：内存清零
来源：http://qxt.yangfankeji.com

memset(a, 0, sizeof a);
来源：http://sgf.zhongyouzk.top

[S27] C：定义常量
来源：http://uzx.yvedp.cn

const double PI = 3.14159;
来源：http://xmn.xinyue.icu

[S28] C：静态变量
来源：http://mhi.316326.xyz

static int counter = 0;
来源：http://kup.nanxuanxn.top

[S29] C：变参函数
来源：http://tnt.dianchejie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nfi.yj20258888.top

[S30] C：头文件保护
来源：http://yjd.sysykeji.top

#ifndef X_H
来源：http://lrg.yangfankeji.com

#define X_H
来源：http://sfg.hesvh.cn

#endif
来源：http://rne.zhengqikj.top

[S31] C++：Hello World
来源：http://utu.tarul.cn

#include <iostream>
来源：http://afb.hesvh.cn

int main() { std::cout << "Hello\n"; }
来源：http://ldl.9152youxi.cn

[S32] C++：字符串
来源：http://osc.shanyushiyangkeji.top

std::string s = "hi";  s += "!";
来源：http://ipu.hnqzz.top

[S33] C++：vector 增删
来源：http://nol.nanxuanxn.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://img.andypj.xyz

[S34] C++：遍历 vector
来源：http://nmd.jqgufenzy.top

for (auto &x : v) { std::cout << x; }
来源：http://jep.guannengcc.top

[S35] C++：map
来源：http://kpf.yongpay.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dvt.jianghu66.top

[S36] C++：unordered_map
来源：http://jig.9152youxi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kvy.sweek.top

[S37] C++：set
来源：http://cfb.sweek.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sek.shuidangran.top

[S38] C++：排序
来源：http://ucm.jinyuanbaomall.cn

std::sort(v.begin(), v.end());
来源：http://cfy.andypj.xyz

[S39] C++：自定义比较器排序
来源：http://mfe.yangfankeji.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kpq.tanke756.top

[S40] C++：查找元素
来源：http://snd.fktsv.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qiy.jqgfzy.top

[S41] C++：类与构造函数
来源：http://hyq.dianchejie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://slt.cashguo.top

[S42] C++：继承与虚函数
来源：http://frl.ehwqpu.com

class B : public Base { public: void f() override {} };
来源：http://gei.c1oappe.top

[S43] C++：智能指针
来源：http://mdl.zhaomingkeji.xyz

auto p = std::make_unique<int>(5);
来源：http://ash.zhiwuduotai.top

[S44] C++：引用传参
来源：http://zam.sufxvd.cn

void inc(int &x) { ++x; }
来源：http://uvn.c1oappe.top

[S45] C++：lambda
来源：http://jzp.vqdsnc.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xou.tarul.cn

[S46] C++：函数模板
来源：http://adr.yangfankeji.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://era.nwbrower.top

[S47] C++：结构化绑定遍历
来源：http://lbf.guowangkeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vcj.jinyuanbaomall.cn

[S48] C++：逐行读文件
来源：http://gqy.fanxiaobao.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://vxj.fktsv.cn

while (std::getline(in, line)) { }
来源：http://jak.yvedp.cn

[S49] C++：写文件
来源：http://rhr.snrcjt.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://avl.guowangkeji.top

[S50] C++：格式化数字
来源：http://nkj.kuanghao11.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pni.tanke756.top

[S51] C++：显式类型转换
来源：http://nna.xylfe.cn

static_cast<double>(a) / b
来源：http://abg.ivvv.top

[S52] C++：const 与 noexcept
来源：http://dmu.shanyushiyangkeji.top

int size() const noexcept { return n_; }
来源：http://npa.ywan-chungtsiang.top

[S53] C++：移动语义
来源：http://ews.tianlin.xyz

std::vector<int> w = std::move(v);
来源：http://umh.zhijiandao.cn

[S54] C++：异常处理
来源：http://cgv.xuanzx.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mdt.ehwqpu.com

[S55] C++：结构化绑定
来源：http://uam.jqgufenzy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://foc.guowangkeji.top

[S56] C++：optional
来源：http://giv.vehdjk.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cmm.iojbl.cn

[S57] C++：编译期常量
来源：http://mjz.iojbl.cn

constexpr int N = 10;
来源：http://osj.yj20258888.top

[S58] C++：命名空间
来源：http://rov.yangfankeji.com

namespace ns { int f() { return 1; } }
来源：http://sza.hammf.cn

[S59] C++：静态断言
来源：http://prn.gotoacloud.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://eog.xuetiantiany.cn

[S60] C++：遍历并删除元素
来源：http://tqn.sweek.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ywa.hfpthk.cn

================================================================================
来源：http://caz.ydjk.org.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tkr.jqgfzy.top

================================================================================
来源：http://uww.yongpay.top

[T01] Kotlin：Hello World
来源：http://hpe.yonumen.top

println("Hello")
来源：http://nzl.sxryk.cn

[T02] Kotlin：变量
来源：http://shv.yj20258.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gnp.daxiang520.top

[T03] Kotlin：字符串模板
来源：http://oea.ydjk.org.cn

"值: $b"
来源：http://ikj.52xcode.cn

[T04] Kotlin：空安全
来源：http://sse.jianghu66.top

val n: String? = null;  n?.length
来源：http://njo.redwolf501.top

[T05] Kotlin：when 表达式
来源：http://awb.cqqwz.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cpx.pengpengdd.cyou

[T06] Kotlin：集合映射
来源：http://dmt.uphjek.com

listOf(1, 2, 3).map { it * 2 }
来源：http://okj.yfazqb.com

[T07] Kotlin：集合过滤
来源：http://elt.zycfv.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://rwy.jinqigfzy.top

[T08] Kotlin：数据类
来源：http://uus.birdmap.top

data class User(val name: String, val age: Int)
来源：http://eyk.yj202588.top

[T09] Kotlin：扩展函数
来源：http://vcl.xziqi.cn

fun String.exclaim() = this + "!"
来源：http://imk.gotoacloud.top

[T10] Kotlin：默认参数
来源：http://leb.xziqi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tni.jianghu66.top

[T11] Kotlin：协程
来源：http://tkn.fanxiaobao.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://fgx.cashguo.top

[T12] Kotlin：解构声明
来源：http://ljp.yongpay.top

val (a, b) = Pair(1, 2)
来源：http://diz.shanyushiyangkeji.top

[T13] Kotlin：只读 Map
来源：http://zch.havefunace.top

val m = mapOf("a" to 1)
来源：http://fwo.feifeiyinyue.top

[T14] Kotlin：循环
来源：http://fsr.jianghu66.top

for (i in 1..10) println(i)
来源：http://jzj.vqdsnc.cn

[T15] Kotlin：接口
来源：http://sxi.aibaodan.cn

interface Shape { fun area(): Double }
来源：http://odz.jiagoushi.top

[T16] Swift：Hello World
来源：http://wnb.tianlin.xyz

print("Hello")
来源：http://fie.sjlbkw.cn

[T17] Swift：变量与常量
来源：http://for.hnqzz.top

var a = 1;  let b = 2
来源：http://itx.zhoulong.xyz

[T18] Swift：字符串插值
来源：http://uuv.52xcode.cn

"值: \(b)"
来源：http://mdx.cashguo.top

[T19] Swift：可选绑定
来源：http://kiv.xingfuxueyuan.xyz

if let n = opt { print(n) }
来源：http://nid.yj20258888.top

[T20] Swift：数组操作
来源：http://zjt.birdmap.top

var a = [1, 2, 3];  a.append(4)
来源：http://onh.ppjwa.cn

[T21] Swift：遍历
来源：http://vei.sjlbkw.cn

for x in a { print(x) }
来源：http://dsw.gaohongyu789.top

[T22] Swift：字典
来源：http://bgh.xingfuxueyuan.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://ojm.52xcode.cn

[T23] Swift：函数
来源：http://uic.cqqwz.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rmh.hfpthk.cn

[T24] Swift：闭包
来源：http://jmk.yj20258.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://lxu.yj20258888.top

[T25] Swift：结构体
来源：http://ygy.uphjek.com

struct P { var x: Int }
来源：http://sjp.quarkkingdee.top

[T26] Swift：类与重写
来源：http://yvw.ivvv.top

class A: Base { override func f() {} }
来源：http://szx.jyoumei.cn

[T27] Swift：错误处理
来源：http://nhc.0kj1m.cn

do { try f() } catch { print(error) }
来源：http://zbr.cqqwz.cn

[T28] Swift：枚举
来源：http://kao.zhengqikj.top

enum Color { case red, green }
来源：http://khg.shangyingyoupin.top

[T29] Swift：guard 提前返回
来源：http://xfa.fehbvm.com

guard let x = opt else { return }
来源：http://inf.vehdjk.com

[T30] Swift：协议
来源：http://box.pengpengdd.cyou

protocol Shape { func area() -> Double }
来源：http://ttn.svipenyu.cn

[T31] Lua：Hello World
来源：http://zgx.gogol.net.cn

print("Hello")
来源：http://wgw.shangyingyoupin.top

[T32] Lua：局部变量
来源：http://xfi.mhx1999.top

local a = 1
来源：http://qcj.jinyuanbaomall.cn

[T33] Lua：表（数组）
来源：http://huc.yanxiufei.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://scv.chenjidiqi.icu

[T34] Lua：遍历表
来源：http://jcl.sjlbkw.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://yfi.wangshuangyany.cn

[T35] Lua：字典表
来源：http://alg.jianghu66.top

local d = { a = 1 };  d.b = 2
来源：http://ihj.xylfe.cn

[T36] Lua：函数
来源：http://rvu.yj20258888.top

function add(a, b) return a + b end
来源：http://ejk.zhaomingkeji.xyz

[T37] Lua：字符串拼接
来源：http://slm.c1oappe.top

"a" .. "b"
来源：http://awg.fzhhl.top

[T38] Lua：条件
来源：http://iji.gaohongyu789.top

if x > 0 then print("正") end
来源：http://dxo.cqqwz.cn

[T39] Lua：模式匹配
来源：http://qvd.shanyushiyangkeji.top

string.find(s, "%d+")
来源：http://vto.redwolf501.top

[T40] Lua：元表
来源：http://ifn.xuanzx.com

setmetatable({}, { __index = base })
来源：http://exo.smart0.xyz

[T41] Perl：Hello World
来源：http://efk.jinqigufen.top

print "Hello\n";
来源：http://vhd.birdmap.top

[T42] Perl：变量类型
来源：http://ull.chenzaomai.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xij.yanxiufei.cn

[T43] Perl：字符串插值
来源：http://blo.ppjwa.cn

"值: $a"
来源：http://ifn.hnxiangtu.top

[T44] Perl：条件
来源：http://xwn.chenjidiqi.icu

if ($a > 0) { print "正"; }
来源：http://pdv.chenjidiqi.icu

[T45] Perl：数组遍历
来源：http://laf.sweek.top

for my $x (@arr) { print $x; }
来源：http://tmr.xingfuxueyuan.xyz

[T46] Perl：哈希操作
来源：http://dkw.dashuyun.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kap.xinyue.icu

[T47] Perl：正则捕获
来源：http://mns.gogol.net.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qol.9152youxi.cn

[T48] Perl：正则替换
来源：http://rhh.havefunace.top

$s =~ s/old/new/g;
来源：http://cqa.yvedp.cn

[T49] Perl：函数
来源：http://efl.haohaochexian.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mso.yanxiufei.cn

[T50] Perl：逐行读文件
来源：http://cmy.zdbjq.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qcy.zhongyouzk.top

while (my $line = <$fh>) { print $line; }
来源：http://lki.feifeiyinyue.top

[T51] Scala：Hello World
来源：http://ryv.fehbvm.com

println("Hello")
来源：http://vmr.smart0.xyz

[T52] Scala：变量
来源：http://gru.ppjwa.cn

val a = 1;  var b = 2
来源：http://voy.9152youxi.cn

[T53] Scala：字符串插值
来源：http://zok.shanyushiyangkeji.top

s"值: $b"
来源：http://qvw.tanke756.top

[T54] Scala：集合映射
来源：http://hiw.shanyushiyangkeji.top

List(1, 2, 3).map(_ * 2)
来源：http://oex.jlsjyb.cn

[T55] Scala：集合过滤
来源：http://rrw.xingfuxueyuan.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://vlp.hesvh.cn

[T56] Scala：样例类
来源：http://xoy.sjlbkw.cn

case class User(name: String, age: Int)
来源：http://xry.zycfv.cn

[T57] Scala：模式匹配
来源：http://mxt.guowangkeji.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://cua.dianchejie.cn

[T58] Scala：函数定义
来源：http://rml.tarul.cn

def add(a: Int, b: Int): Int = a + b
来源：http://pqc.epnwcf.com

[T59] Scala：循环
来源：http://vtd.chenzaomai.com

for (i <- 1 to 10) println(i)
来源：http://huy.havefunace.top

[T60] Scala：折叠
来源：http://ogf.jianghu66.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://onl.fanxiaobao.xyz

================================================================================
来源：http://idm.yangfankeji.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zuu.epnwcf.com

================================================================================
来源：http://zpe.ivvv.top

[U01] Py：创建虚拟环境
来源：http://kyi.jqgufenzy.top

python -m venv .venv && source .venv/bin/activate
来源：http://biq.hysaishi.cn

[U02] Py：导出 / 安装依赖
来源：http://ypa.xingfuxueyuan.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qkk.wangshuangyany.cn

[U03] Py：加载 .env 配置
来源：http://ddg.cheryme.top

from dotenv import load_dotenv; load_dotenv()
来源：http://wny.uphjek.com

[U04] Py：变量调试打印
来源：http://bmk.tarul.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://thh.gzhubu.top

[U05] Py：列表去重且保序
来源：http://npp.vehdjk.com

list(dict.fromkeys(arr))
来源：http://jqd.iojbl.cn

[U06] Py：合并两个字典
来源：http://nzg.yuxming.cn

{**a, **b}
来源：http://qnn.hywenlv.cn

[U07] Py：反转字典键值
来源：http://psd.yanxiufei.cn

{v: k for k, v in d.items()}
来源：http://kha.xziqi.cn

[U08] Py：展平二维列表
来源：http://leb.shuidangran.top

[y for x in nested for y in x]
来源：http://dzx.yueranfly.top


<!-- 参考信息 -->