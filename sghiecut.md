代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://luc.xingfuxueyuan.xyz

[R70] 时间戳与互转
来源：http://etw.havefunace.top

date +%s;  date -d @1700000000
来源：http://nyw.ppjwa.cn

[R71] 日期格式化
来源：http://pkv.epnwcf.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://qfm.hnxiangtu.top

[R72] 等待端口就绪
来源：http://gmy.zdbjq.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://efi.jiagoushi.top

[R73] 分割大日志
来源：http://dkb.zhiwuduotai.top

split -l 1000 big.log part_
来源：http://gcz.jinqigufen.top

[R74] 批量重命名
来源：http://ebt.fehbvm.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pbr.0kj1m.cn

[R75] 导出环境变量
来源：http://iru.yongpay.top

export PATH="$HOME/bin:$PATH"
来源：http://uzp.cucudq.cn

[R76] 使用临时文件
来源：http://zrw.xuanzx.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yhd.smart0.xyz

[R77] 读取用户输入
来源：http://rhy.gaohongyu789.top

read -rp "请输入: " ans
来源：http://pqf.chenlongwang.top

[R78] 交互式菜单
来源：http://fxb.hammf.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://vlt.xziqi.cn

[R79] 解析命令行选项
来源：http://qfs.zhoulong.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nsh.daria6918.cn

[R80] 查看脚本执行耗时
来源：http://tsp.yfazqb.com

time ./run.sh
来源：http://hcl.fengsongda.top

================================================================================
来源：http://ijt.shanyushiyangtech.top

S. C / C++ 专题
来源：http://orc.dashuyun.cn

================================================================================
来源：http://qhm.yj202588.top

[S01] C：Hello World
来源：http://avw.yj20258.top

#include <stdio.h>
来源：http://bty.dashuyun.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://yip.wangdashe.top

[S02] C：变量与格式化输出
来源：http://jcm.hcnkem.com

int a = 10; printf("%d\n", a);
来源：http://sla.guowangkeji.top

[S03] C：读入整数
来源：http://fsw.uphjek.com

int x; scanf("%d", &x);
来源：http://jdp.hesvh.cn

[S04] C：字符串复制
来源：http://axp.cucudq.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ama.haohaochexian.top

[S05] C：字符串长度
来源：http://lsw.gaohongyu789.top

strlen(s)
来源：http://fzp.aizwys.cn

[S06] C：字符串比较
来源：http://vid.jyoumei.cn

strcmp(a, b) == 0
来源：http://aqg.zhaomingkeji.xyz

[S07] C：数组遍历求和
来源：http://mkp.yj20258888.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vjo.xingfuxueyuan.xyz

[S08] C：动态内存分配与释放
来源：http://xag.zhiwuduotai.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xys.gotoacloud.top

[S09] C：结构体定义与初始化
来源：http://svz.dashuyun.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uqt.havefunace.top

[S10] C：指针与解引用
来源：http://hcs.c1oappe.top

int *p = &a;  *p = 5;
来源：http://uwk.havefunace.top

[S11] C：逐行读文件
来源：http://llu.dashuyun.cn

FILE *f = fopen("a.txt", "r");
来源：http://mfg.yfazqb.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://sca.xinyue.icu

fclose(f);
来源：http://ybh.ctjpmb.com

[S12] C：写文件
来源：http://pmg.jinghuilouyu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bks.hongshengwenyu.top

[S13] C：宏定义
来源：http://upo.fzhhl.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fed.jiagoushi.top

[S14] C：枚举
来源：http://hti.ywan-chungtsiang.top

enum Color { RED, GREEN, BLUE };
来源：http://yjc.ydzc1.top

[S15] C：类型转换
来源：http://qeq.fengsongda.top

(double) a / b
来源：http://elt.ehwqpu.com

[S16] C：位操作置位
来源：http://qan.quarkkingdee.top

x |= (1 << 3);
来源：http://vek.jianghu66.top

[S17] C：安全拼接字符串
来源：http://ouy.jlsjyb.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mrf.andypj.xyz

[S18] C：命令行参数
来源：http://bvy.jinyuanbaomall.cn

int main(int argc, char **argv)
来源：http://ywh.fktsv.cn

[S19] C：快速排序
来源：http://pth.havefunace.top

qsort(a, n, sizeof(int), cmp);
来源：http://wra.zhaomingkeji.xyz

[S20] C：二分查找
来源：http://yjm.andypj.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mqg.shzxlz.cn

[S21] C：字符类别判断
来源：http://nbn.gaohongyu789.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nfz.ydzc1.top

[S22] C：字符串转数字
来源：http://cql.vqdsnc.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tmm.fehbvm.com

[S23] C：随机数
来源：http://toj.quarkkingdee.top

srand(time(NULL));  int r = rand() % 100;
来源：http://tfz.yvedp.cn

[S24] C：获取本地时间
来源：http://ove.havefunace.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uso.cashguo.top

[S25] C：内存拷贝
来源：http://aos.iojbl.cn

memcpy(dst, src, n);
来源：http://dwz.hcnkem.com

[S26] C：内存清零
来源：http://cyb.yj20258.top

memset(a, 0, sizeof a);
来源：http://osv.yonumen.top

[S27] C：定义常量
来源：http://yje.dashuyun.cn

const double PI = 3.14159;
来源：http://tub.zdqjudy.top

[S28] C：静态变量
来源：http://cbw.xylfe.cn

static int counter = 0;
来源：http://bvr.yonumen.top

[S29] C：变参函数
来源：http://jdy.xuetiantiany.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rxl.cheryme.top

[S30] C：头文件保护
来源：http://gra.epnwcf.com

#ifndef X_H
来源：http://qfi.jinqigufen.top

#define X_H
来源：http://lbp.redwolf501.top

#endif
来源：http://ztl.hammf.cn

[S31] C++：Hello World
来源：http://qgi.jinyuanbaomall.cn

#include <iostream>
来源：http://vin.sjlbkw.cn

int main() { std::cout << "Hello\n"; }
来源：http://bcs.jiagoushi.top

[S32] C++：字符串
来源：http://aek.jianghu66.top

std::string s = "hi";  s += "!";
来源：http://fxf.ivvv.top

[S33] C++：vector 增删
来源：http://wao.gzhubu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vth.zhixingplan.top

[S34] C++：遍历 vector
来源：http://mxf.zhiwuduotai.top

for (auto &x : v) { std::cout << x; }
来源：http://okk.svipenyu.cn

[S35] C++：map
来源：http://jii.ywan-chungtsiang.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qim.fengsongda.top

[S36] C++：unordered_map
来源：http://dqm.cheryme.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tao.tarul.cn

[S37] C++：set
来源：http://zoq.xuanzx.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jze.nanxinkj.top

[S38] C++：排序
来源：http://nbg.tanke756.top

std::sort(v.begin(), v.end());
来源：http://aeb.fengsongda.top

[S39] C++：自定义比较器排序
来源：http://ykc.daxiang520.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yna.jqgfzy.top

[S40] C++：查找元素
来源：http://txs.xuetiantiany.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nlj.quarkkingdee.top

[S41] C++：类与构造函数
来源：http://njx.iojbl.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kps.zhoulong.xyz

[S42] C++：继承与虚函数
来源：http://wjx.jinqigufen.top

class B : public Base { public: void f() override {} };
来源：http://wln.birdmap.top

[S43] C++：智能指针
来源：http://neo.smart0.xyz

auto p = std::make_unique<int>(5);
来源：http://hjh.yanxiufei.cn

[S44] C++：引用传参
来源：http://gfc.gotoacloud.top

void inc(int &x) { ++x; }
来源：http://vjp.snrcjt.cn

[S45] C++：lambda
来源：http://qhd.meibo888.top

auto add = [](int a, int b) { return a + b; };
来源：http://jxy.yj20258.top

[S46] C++：函数模板
来源：http://xsp.tian-w.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ajb.vehdjk.com

[S47] C++：结构化绑定遍历
来源：http://avl.smart0.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ucw.bbcook.cn

[S48] C++：逐行读文件
来源：http://jmn.pengpengdd.cyou

std::ifstream in("a.txt");  std::string line;
来源：http://ion.sjlbkw.cn

while (std::getline(in, line)) { }
来源：http://otw.guowangkeji.top

[S49] C++：写文件
来源：http://ayi.smart0.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://heo.svipenyu.cn

[S50] C++：格式化数字
来源：http://egv.zhijiandao.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zwy.tian-w.cn

[S51] C++：显式类型转换
来源：http://xey.epnwcf.com

static_cast<double>(a) / b
来源：http://tkt.fengsongda.top

[S52] C++：const 与 noexcept
来源：http://vpd.yfazqb.com

int size() const noexcept { return n_; }
来源：http://uhg.mhx1999.top

[S53] C++：移动语义
来源：http://nxx.316326.xyz

std::vector<int> w = std::move(v);
来源：http://fdy.fengsongda.top

[S54] C++：异常处理
来源：http://fvf.aizwys.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jqf.iojbl.cn

[S55] C++：结构化绑定
来源：http://iwk.yueranfly.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ogi.ivvv.top

[S56] C++：optional
来源：http://zzh.sjlbkw.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sbg.iojbl.cn

[S57] C++：编译期常量
来源：http://hvd.daxiang520.top

constexpr int N = 10;
来源：http://lnv.bjfxy.top

[S58] C++：命名空间
来源：http://adw.jiagoushi.top

namespace ns { int f() { return 1; } }
来源：http://nhp.redwolf501.top

[S59] C++：静态断言
来源：http://nmt.c1oappe.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gct.gotoacloud.top

[S60] C++：遍历并删除元素
来源：http://bmn.fzhhl.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jdh.jinyuanbaomall.cn

================================================================================
来源：http://dyc.tarul.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ert.xuanzx.com

================================================================================
来源：http://mnf.chenzaomai.com

[T01] Kotlin：Hello World
来源：http://rbg.nanxinkj.top

println("Hello")
来源：http://yrg.iojbl.cn

[T02] Kotlin：变量
来源：http://vmt.daxiang520.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://shm.feifeiyinyue.top

[T03] Kotlin：字符串模板
来源：http://bvc.316326.xyz

"值: $b"
来源：http://hsc.shanyushiyangtech.top

[T04] Kotlin：空安全
来源：http://huo.316326.xyz

val n: String? = null;  n?.length
来源：http://zek.gogol.net.cn

[T05] Kotlin：when 表达式
来源：http://cor.zhiwuduotai.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://grx.jqgfzy.top

[T06] Kotlin：集合映射
来源：http://etz.ctjpmb.com

listOf(1, 2, 3).map { it * 2 }
来源：http://xpj.fzhhl.top

[T07] Kotlin：集合过滤
来源：http://qee.snrcjt.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://oem.jqgufenzy.top

[T08] Kotlin：数据类
来源：http://qrv.yangfankeji.com

data class User(val name: String, val age: Int)
来源：http://ita.fktsv.cn

[T09] Kotlin：扩展函数
来源：http://aue.316326.xyz

fun String.exclaim() = this + "!"
来源：http://znd.zhengqikj.top

[T10] Kotlin：默认参数
来源：http://qfu.jinqigufen.top

fun greet(name: String = "World") = "Hi $name"
来源：http://nis.xingfuxueyuan.xyz

[T11] Kotlin：协程
来源：http://vzu.jinqigufen.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://pvg.316326.xyz

[T12] Kotlin：解构声明
来源：http://gho.bjfxy.top

val (a, b) = Pair(1, 2)
来源：http://bqm.zhiwuduotai.top

[T13] Kotlin：只读 Map
来源：http://ave.0kj1m.cn

val m = mapOf("a" to 1)
来源：http://jfw.xinyue.icu

[T14] Kotlin：循环
来源：http://wgt.fengsongda.top

for (i in 1..10) println(i)
来源：http://snu.cucudq.cn

[T15] Kotlin：接口
来源：http://ryk.cheryme.top

interface Shape { fun area(): Double }
来源：http://yfz.mhx1999.top

[T16] Swift：Hello World
来源：http://wfv.pycfn.com

print("Hello")
来源：http://nzw.zhaomingkeji.xyz

[T17] Swift：变量与常量
来源：http://ntk.hfpthk.cn

var a = 1;  let b = 2
来源：http://jxp.yangfankeji.com

[T18] Swift：字符串插值
来源：http://fal.sjlbkw.cn

"值: \(b)"
来源：http://gsy.ybcxt.top

[T19] Swift：可选绑定
来源：http://ydv.jqgfzy.top

if let n = opt { print(n) }
来源：http://ltl.fengsongda.top

[T20] Swift：数组操作
来源：http://kva.snrcjt.cn

var a = [1, 2, 3];  a.append(4)
来源：http://unv.chenjidiqi.icu

[T21] Swift：遍历
来源：http://kdi.cqqwz.cn

for x in a { print(x) }
来源：http://pbh.shzxlz.cn

[T22] Swift：字典
来源：http://vfw.nanxinkj.top

var d = ["a": 1];  d["b"] = 2
来源：http://xtf.jiagoushi.top

[T23] Swift：函数
来源：http://mgm.jiagoushi.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ein.fktsv.cn

[T24] Swift：闭包
来源：http://svg.yvedp.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://aey.aibaodan.cn

[T25] Swift：结构体
来源：http://wvv.ybcxt.top

struct P { var x: Int }
来源：http://lhx.andypj.xyz

[T26] Swift：类与重写
来源：http://lnl.sysykeji.top

class A: Base { override func f() {} }
来源：http://rmq.zhijiandao.cn

[T27] Swift：错误处理
来源：http://hxe.hywenlv.cn

do { try f() } catch { print(error) }
来源：http://bcs.redwolf501.top

[T28] Swift：枚举
来源：http://ptf.zhiwuduotai.top

enum Color { case red, green }
来源：http://nrj.hammf.cn

[T29] Swift：guard 提前返回
来源：http://sye.fanxiaobao.xyz

guard let x = opt else { return }
来源：http://lgc.daxiang520.top

[T30] Swift：协议
来源：http://kfm.hongshengwenyu.top

protocol Shape { func area() -> Double }
来源：http://oin.hesvh.cn

[T31] Lua：Hello World
来源：http://ear.tian-w.cn

print("Hello")
来源：http://rbk.meibo888.top

[T32] Lua：局部变量
来源：http://fku.havefunace.top

local a = 1
来源：http://lyh.shangyingyoupin.top

[T33] Lua：表（数组）
来源：http://ohq.xuetiantiany.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://zkx.ywan-chungtsiang.top

[T34] Lua：遍历表
来源：http://bsw.yj202588.top

for i, v in ipairs(t) do print(i, v) end
来源：http://zej.guannengcc.top

[T35] Lua：字典表
来源：http://dzz.jiagoushi.top

local d = { a = 1 };  d.b = 2
来源：http://nxg.hongshengwenyu.top

[T36] Lua：函数
来源：http://srd.xylfe.cn

function add(a, b) return a + b end
来源：http://fqr.pycfn.com

[T37] Lua：字符串拼接
来源：http://tzi.jiagoushi.top

"a" .. "b"
来源：http://iua.jqgufenzy.top

[T38] Lua：条件
来源：http://sgh.xingfuxueyuan.xyz

if x > 0 then print("正") end
来源：http://ubk.smart0.xyz

[T39] Lua：模式匹配
来源：http://zuu.feifeiyinyue.top

string.find(s, "%d+")
来源：http://zcv.shuidangran.top

[T40] Lua：元表
来源：http://zoo.tarul.cn

setmetatable({}, { __index = base })
来源：http://afx.yonumen.top

[T41] Perl：Hello World
来源：http://fet.zdqjudy.top

print "Hello\n";
来源：http://bss.jqgfzy.top

[T42] Perl：变量类型
来源：http://oeu.jyoumei.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fka.9152youxi.cn

[T43] Perl：字符串插值
来源：http://cwn.meibo888.top

"值: $a"
来源：http://azn.jinqigfzy.top

[T44] Perl：条件
来源：http://izf.jyoumei.cn

if ($a > 0) { print "正"; }
来源：http://fni.bbcook.cn

[T45] Perl：数组遍历
来源：http://abk.vehdjk.com

for my $x (@arr) { print $x; }
来源：http://vsq.52xcode.cn

[T46] Perl：哈希操作
来源：http://roc.dashuyun.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nuf.vqdsnc.cn

[T47] Perl：正则捕获
来源：http://yod.ppjwa.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xds.uphjek.com

[T48] Perl：正则替换
来源：http://asy.aibaodan.cn

$s =~ s/old/new/g;
来源：http://hub.zhengqikj.top

[T49] Perl：函数
来源：http://wmi.jinghuilouyu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wgk.tanke756.top

[T50] Perl：逐行读文件
来源：http://tiw.uphjek.com

open my $fh, "<", "a.txt" or die $!;
来源：http://iwf.0kj1m.cn

while (my $line = <$fh>) { print $line; }
来源：http://rea.hnqzz.top

[T51] Scala：Hello World
来源：http://deg.dashuyun.cn

println("Hello")
来源：http://soe.kuanghao11.cn

[T52] Scala：变量
来源：http://jjf.sjlbkw.cn

val a = 1;  var b = 2
来源：http://fjq.9152youxi.cn

[T53] Scala：字符串插值
来源：http://ymq.meibo888.top

s"值: $b"
来源：http://fog.fktsv.cn

[T54] Scala：集合映射
来源：http://yhb.ivvv.top

List(1, 2, 3).map(_ * 2)
来源：http://sfp.snrcjt.cn

[T55] Scala：集合过滤
来源：http://kpy.sxryk.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gll.smart0.xyz

[T56] Scala：样例类
来源：http://oej.snrcjt.cn

case class User(name: String, age: Int)
来源：http://lxw.jiagoushi.top

[T57] Scala：模式匹配
来源：http://scc.jqgfzy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://tej.hywenlv.cn

[T58] Scala：函数定义
来源：http://jin.9152youxi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://hex.uphjek.com

[T59] Scala：循环
来源：http://lro.zycfv.cn

for (i <- 1 to 10) println(i)
来源：http://vyc.hesvh.cn

[T60] Scala：折叠
来源：http://xqt.316326.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xvr.aibaodan.cn

================================================================================
来源：http://amg.sjlbkw.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vds.zhiwuduotai.top

================================================================================
来源：http://oez.jqgufenzy.top

[U01] Py：创建虚拟环境
来源：http://wia.jlsjyb.cn

python -m venv .venv && source .venv/bin/activate
来源：http://tie.sxryk.cn

[U02] Py：导出 / 安装依赖
来源：http://ihn.nanxuanxn.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://drd.pengpengdd.cyou

[U03] Py：加载 .env 配置
来源：http://ost.yj202588.top

from dotenv import load_dotenv; load_dotenv()
来源：http://vdy.bjfxy.top

[U04] Py：变量调试打印
来源：http://dvm.guowangkeji.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xwt.jinqigufen.top

[U05] Py：列表去重且保序
来源：http://nyz.xingfuxueyuan.xyz

list(dict.fromkeys(arr))
来源：http://brz.redwolf501.top

[U06] Py：合并两个字典
来源：http://hbv.quarkkingdee.top

{**a, **b}
来源：http://ono.iojbl.cn

[U07] Py：反转字典键值
来源：http://rcg.yj20258.top

{v: k for k, v in d.items()}
来源：http://sbf.ywan-chungtsiang.top

[U08] Py：展平二维列表
来源：http://qzl.snrcjt.cn

[y for x in nested for y in x]
来源：http://csj.zdbjq.cn

[U09] Py：字典取最大值的键
来源：http://tsr.aizwys.cn

max(d, key=d.get)
来源：http://gox.zdbjq.cn

[U10] Py：按值排序字典
来源：http://ljf.zhoulong.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mdd.tarul.cn


<!-- 参考信息 -->