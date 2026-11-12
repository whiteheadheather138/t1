代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://vjj.yj20258888.top

[R72] 等待端口就绪
来源：http://uca.redwolf501.top

until nc -z localhost 3306; do sleep 1; done
来源：http://zmd.yuanzhike.top

[R73] 分割大日志
来源：http://msu.zhaomingkeji.xyz

split -l 1000 big.log part_
来源：http://cze.tianlin.xyz

[R74] 批量重命名
来源：http://php.ydzc1.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://abl.sjlbkw.cn

[R75] 导出环境变量
来源：http://oty.yuanzhike.top

export PATH="$HOME/bin:$PATH"
来源：http://pfk.ydjk.org.cn

[R76] 使用临时文件
来源：http://bbp.sweek.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jxa.yvedp.cn

[R77] 读取用户输入
来源：http://tul.fzhhl.top

read -rp "请输入: " ans
来源：http://pzs.zhijiandao.cn

[R78] 交互式菜单
来源：http://txt.fanxiaobao.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://xgw.chenzaomai.com

[R79] 解析命令行选项
来源：http://nzu.gotoacloud.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gvb.vqdsnc.cn

[R80] 查看脚本执行耗时
来源：http://rmj.tanke756.top

time ./run.sh
来源：http://odh.yuxming.cn

================================================================================
来源：http://lst.sjlbkw.cn

S. C / C++ 专题
来源：http://fta.fktsv.cn

================================================================================
来源：http://bhp.shzxlz.cn

[S01] C：Hello World
来源：http://xme.zhoulong.xyz

#include <stdio.h>
来源：http://zyn.jinghuilouyu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://agh.ctjpmb.com

[S02] C：变量与格式化输出
来源：http://mso.shanyushiyangtech.top

int a = 10; printf("%d\n", a);
来源：http://jbd.yuanzhike.top

[S03] C：读入整数
来源：http://yex.jinyuanbaomall.cn

int x; scanf("%d", &x);
来源：http://vcj.vehdjk.com

[S04] C：字符串复制
来源：http://gct.fktsv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ewx.dashuyun.cn

[S05] C：字符串长度
来源：http://atr.c1oappe.top

strlen(s)
来源：http://dro.yueranfly.top

[S06] C：字符串比较
来源：http://skz.shuidangran.top

strcmp(a, b) == 0
来源：http://aor.ppjwa.cn

[S07] C：数组遍历求和
来源：http://ncs.yj20258888.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://err.yanxiufei.cn

[S08] C：动态内存分配与释放
来源：http://rcc.kuanghao11.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uwh.daria6918.cn

[S09] C：结构体定义与初始化
来源：http://juo.nanxinkj.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://djg.ydjk.org.cn

[S10] C：指针与解引用
来源：http://drt.daria6918.cn

int *p = &a;  *p = 5;
来源：http://idd.yj20258.top

[S11] C：逐行读文件
来源：http://mfp.gotoacloud.top

FILE *f = fopen("a.txt", "r");
来源：http://tjh.nanxinkj.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://pwe.uphjek.com

fclose(f);
来源：http://hzl.yfazqb.com

[S12] C：写文件
来源：http://dsh.hongshengwenyu.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ctg.cqqwz.cn

[S13] C：宏定义
来源：http://zhg.hnqzz.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pgw.kuanghao11.cn

[S14] C：枚举
来源：http://jkz.cashguo.top

enum Color { RED, GREEN, BLUE };
来源：http://yob.kuanghao11.cn

[S15] C：类型转换
来源：http://jle.svipenyu.cn

(double) a / b
来源：http://evi.nanxuanxn.top

[S16] C：位操作置位
来源：http://xdp.birdmap.top

x |= (1 << 3);
来源：http://sts.jiagoushi.top

[S17] C：安全拼接字符串
来源：http://isu.chenzaomai.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://col.kuanghao11.cn

[S18] C：命令行参数
来源：http://qfm.chenlongwang.top

int main(int argc, char **argv)
来源：http://mus.bjfxy.top

[S19] C：快速排序
来源：http://aal.guannengcc.top

qsort(a, n, sizeof(int), cmp);
来源：http://dol.zhaomingkeji.xyz

[S20] C：二分查找
来源：http://pfb.nanxuanxn.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pws.fengsongda.top

[S21] C：字符类别判断
来源：http://web.shuidangran.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://uss.xingfuxueyuan.xyz

[S22] C：字符串转数字
来源：http://kpi.sjlbkw.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qju.mhx1999.top

[S23] C：随机数
来源：http://ltl.chenjidiqi.icu

srand(time(NULL));  int r = rand() % 100;
来源：http://mdn.316326.xyz

[S24] C：获取本地时间
来源：http://fkh.iojbl.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://scf.sxryk.cn

[S25] C：内存拷贝
来源：http://qyf.nanxuanxn.top

memcpy(dst, src, n);
来源：http://atx.vehdjk.com

[S26] C：内存清零
来源：http://vze.guannengcc.top

memset(a, 0, sizeof a);
来源：http://jqy.yanxiufei.cn

[S27] C：定义常量
来源：http://sdb.gotoacloud.top

const double PI = 3.14159;
来源：http://lxj.shuidangran.top

[S28] C：静态变量
来源：http://aud.uphjek.com

static int counter = 0;
来源：http://mue.zdqjudy.top

[S29] C：变参函数
来源：http://psy.jqgufenzy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ure.tian-w.cn

[S30] C：头文件保护
来源：http://pry.smart0.xyz

#ifndef X_H
来源：http://rut.pengpengdd.cyou

#define X_H
来源：http://dvh.hnqzz.top

#endif
来源：http://cem.c1oappe.top

[S31] C++：Hello World
来源：http://zmc.nwbrower.top

#include <iostream>
来源：http://vky.feifeiyinyue.top

int main() { std::cout << "Hello\n"; }
来源：http://opr.hammf.cn

[S32] C++：字符串
来源：http://duh.yj20258.top

std::string s = "hi";  s += "!";
来源：http://gqh.fengsongda.top

[S33] C++：vector 增删
来源：http://wzo.yj20258.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://emp.xinyue.icu

[S34] C++：遍历 vector
来源：http://kui.vqdsnc.cn

for (auto &x : v) { std::cout << x; }
来源：http://pid.pengpengdd.cyou

[S35] C++：map
来源：http://yxu.ivvv.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://etb.aibaodan.cn

[S36] C++：unordered_map
来源：http://uop.kuanghao11.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sfg.cashguo.top

[S37] C++：set
来源：http://kyu.cqqwz.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qhd.shanyushiyangkeji.top

[S38] C++：排序
来源：http://jwk.hcnkem.com

std::sort(v.begin(), v.end());
来源：http://mcb.hysaishi.cn

[S39] C++：自定义比较器排序
来源：http://vkr.tanke756.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xaf.jiagoushi.top

[S40] C++：查找元素
来源：http://yaf.tianlin.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hqo.svipenyu.cn

[S41] C++：类与构造函数
来源：http://ngq.chenzaomai.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zma.316326.xyz

[S42] C++：继承与虚函数
来源：http://zpp.316326.xyz

class B : public Base { public: void f() override {} };
来源：http://ihb.iojbl.cn

[S43] C++：智能指针
来源：http://rbi.shanyushiyangtech.top

auto p = std::make_unique<int>(5);
来源：http://bdm.cqqwz.cn

[S44] C++：引用传参
来源：http://ras.52xcode.cn

void inc(int &x) { ++x; }
来源：http://smh.0kj1m.cn

[S45] C++：lambda
来源：http://dar.0kj1m.cn

auto add = [](int a, int b) { return a + b; };
来源：http://dkh.aizwys.cn

[S46] C++：函数模板
来源：http://szv.epnwcf.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uhm.nwbrower.top

[S47] C++：结构化绑定遍历
来源：http://vyl.gotoacloud.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jwb.ybcxt.top

[S48] C++：逐行读文件
来源：http://qzl.dianchejie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://key.ywan-chungtsiang.top

while (std::getline(in, line)) { }
来源：http://dkl.fengsongda.top

[S49] C++：写文件
来源：http://eha.zhaomingkeji.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jvd.mhx1999.top

[S50] C++：格式化数字
来源：http://tsf.xingfuxueyuan.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zva.0kj1m.cn

[S51] C++：显式类型转换
来源：http://rqp.zhaomingkeji.xyz

static_cast<double>(a) / b
来源：http://myo.tarul.cn

[S52] C++：const 与 noexcept
来源：http://lju.zhiwuduotai.top

int size() const noexcept { return n_; }
来源：http://dby.chenlongwang.top

[S53] C++：移动语义
来源：http://suf.hnqzz.top

std::vector<int> w = std::move(v);
来源：http://pmu.fanxiaobao.xyz

[S54] C++：异常处理
来源：http://rkq.dashuyun.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ras.jianghu66.top

[S55] C++：结构化绑定
来源：http://jco.vqdsnc.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://dyd.tianlin.xyz

[S56] C++：optional
来源：http://fbd.hnxiangtu.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fgn.nanxuanxn.top

[S57] C++：编译期常量
来源：http://zlh.sjlbkw.cn

constexpr int N = 10;
来源：http://rhp.guannengcc.top

[S58] C++：命名空间
来源：http://udq.yj202588.top

namespace ns { int f() { return 1; } }
来源：http://fln.yj202588.top

[S59] C++：静态断言
来源：http://omk.fktsv.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zxs.shzxlz.cn

[S60] C++：遍历并删除元素
来源：http://vfp.ydjk.org.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hcp.shangyingyoupin.top

================================================================================
来源：http://pgm.jiagoushi.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dou.xylfe.cn

================================================================================
来源：http://mfv.gzhubu.top

[T01] Kotlin：Hello World
来源：http://vrd.ivvv.top

println("Hello")
来源：http://toe.ydjk.org.cn

[T02] Kotlin：变量
来源：http://noz.shanyushiyangtech.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bnp.wangshuangyany.cn

[T03] Kotlin：字符串模板
来源：http://znt.tarul.cn

"值: $b"
来源：http://eox.jiagoushi.top

[T04] Kotlin：空安全
来源：http://rqu.havefunace.top

val n: String? = null;  n?.length
来源：http://jyr.smart0.xyz

[T05] Kotlin：when 表达式
来源：http://xsr.ivvv.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fuo.tarul.cn

[T06] Kotlin：集合映射
来源：http://guw.jinghuilouyu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tfa.yonumen.top

[T07] Kotlin：集合过滤
来源：http://wzh.birdmap.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ppu.hnqzz.top

[T08] Kotlin：数据类
来源：http://ywi.jqgufenzy.top

data class User(val name: String, val age: Int)
来源：http://ugq.gotoacloud.top

[T09] Kotlin：扩展函数
来源：http://uvr.cheryme.top

fun String.exclaim() = this + "!"
来源：http://jqx.iojbl.cn

[T10] Kotlin：默认参数
来源：http://hbm.xziqi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://lkc.kuanghao11.cn

[T11] Kotlin：协程
来源：http://ztm.gaohongyu789.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://oan.jinqigfzy.top

[T12] Kotlin：解构声明
来源：http://fdf.hfpthk.cn

val (a, b) = Pair(1, 2)
来源：http://adh.ppjwa.cn

[T13] Kotlin：只读 Map
来源：http://gtz.vehdjk.com

val m = mapOf("a" to 1)
来源：http://ooz.snrcjt.cn

[T14] Kotlin：循环
来源：http://lkn.wangshuangyany.cn

for (i in 1..10) println(i)
来源：http://khc.dashuyun.cn

[T15] Kotlin：接口
来源：http://cvt.cashguo.top

interface Shape { fun area(): Double }
来源：http://ool.daxiang520.top

[T16] Swift：Hello World
来源：http://tmo.jqgufenzy.top

print("Hello")
来源：http://czr.sysykeji.top

[T17] Swift：变量与常量
来源：http://gjb.tian-w.cn

var a = 1;  let b = 2
来源：http://wmv.hnxiangtu.top

[T18] Swift：字符串插值
来源：http://qbn.zhixingplan.top

"值: \(b)"
来源：http://fxg.sysykeji.top

[T19] Swift：可选绑定
来源：http://old.birdmap.top

if let n = opt { print(n) }
来源：http://dco.uphjek.com

[T20] Swift：数组操作
来源：http://iqy.zhiwuduotai.top

var a = [1, 2, 3];  a.append(4)
来源：http://arq.hfpthk.cn

[T21] Swift：遍历
来源：http://irv.meibo888.top

for x in a { print(x) }
来源：http://qyr.ydzc1.top

[T22] Swift：字典
来源：http://gvy.hywenlv.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xjw.sufxvd.cn

[T23] Swift：函数
来源：http://hjr.mhx1999.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jtw.chenlongwang.top

[T24] Swift：闭包
来源：http://kaa.sjlbkw.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://mkt.cheryme.top

[T25] Swift：结构体
来源：http://ase.xylfe.cn

struct P { var x: Int }
来源：http://clo.iojbl.cn

[T26] Swift：类与重写
来源：http://mer.jinyuanbaomall.cn

class A: Base { override func f() {} }
来源：http://jdz.haohaochexian.top

[T27] Swift：错误处理
来源：http://rog.tanke756.top

do { try f() } catch { print(error) }
来源：http://yva.kuanghao11.cn

[T28] Swift：枚举
来源：http://qkc.jlsjyb.cn

enum Color { case red, green }
来源：http://cbw.yvedp.cn

[T29] Swift：guard 提前返回
来源：http://ndm.zdqjudy.top

guard let x = opt else { return }
来源：http://rdm.andypj.xyz

[T30] Swift：协议
来源：http://qiq.pycfn.com

protocol Shape { func area() -> Double }
来源：http://blh.zhijiandao.cn

[T31] Lua：Hello World
来源：http://kjr.cqqwz.cn

print("Hello")
来源：http://iya.jyoumei.cn

[T32] Lua：局部变量
来源：http://bvv.yongpay.top

local a = 1
来源：http://tmc.shanyushiyangkeji.top

[T33] Lua：表（数组）
来源：http://vig.wangdashe.top

local t = {1, 2, 3};  t[4] = 4
来源：http://fja.cdnleiting.top

[T34] Lua：遍历表
来源：http://iay.epnwcf.com

for i, v in ipairs(t) do print(i, v) end
来源：http://vkb.feifeiyinyue.top

[T35] Lua：字典表
来源：http://kcg.xingfuxueyuan.xyz

local d = { a = 1 };  d.b = 2
来源：http://qpt.iojbl.cn

[T36] Lua：函数
来源：http://rve.ybcxt.top

function add(a, b) return a + b end
来源：http://tbr.tian-w.cn

[T37] Lua：字符串拼接
来源：http://phh.aizwys.cn

"a" .. "b"
来源：http://hfk.nanxinkj.top

[T38] Lua：条件
来源：http://yef.iojbl.cn

if x > 0 then print("正") end
来源：http://vls.316326.xyz

[T39] Lua：模式匹配
来源：http://yed.zhoulong.xyz

string.find(s, "%d+")
来源：http://uce.yangfankeji.com

[T40] Lua：元表
来源：http://skc.shuidangran.top

setmetatable({}, { __index = base })
来源：http://gmm.daria6918.cn

[T41] Perl：Hello World
来源：http://lsw.zhaomingkeji.xyz

print "Hello\n";
来源：http://bdi.tianlin.xyz

[T42] Perl：变量类型
来源：http://byj.jinqigfzy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pcn.andypj.xyz

[T43] Perl：字符串插值
来源：http://ezy.gzhubu.top

"值: $a"
来源：http://bpz.pycfn.com

[T44] Perl：条件
来源：http://teg.yj20258888.top

if ($a > 0) { print "正"; }
来源：http://fqn.jqgufenzy.top

[T45] Perl：数组遍历
来源：http://yop.ybcxt.top

for my $x (@arr) { print $x; }
来源：http://omq.tarul.cn

[T46] Perl：哈希操作
来源：http://chz.ybcxt.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qlg.jqgufenzy.top

[T47] Perl：正则捕获
来源：http://yuc.shangyingyoupin.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://mzz.birdmap.top

[T48] Perl：正则替换
来源：http://cri.gzhubu.top

$s =~ s/old/new/g;
来源：http://vdf.gaohongyu789.top

[T49] Perl：函数
来源：http://qqn.xylfe.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://orj.wangdashe.top

[T50] Perl：逐行读文件
来源：http://rfw.zhengqikj.top

open my $fh, "<", "a.txt" or die $!;
来源：http://rrq.yueranfly.top

while (my $line = <$fh>) { print $line; }
来源：http://der.zycfv.cn

[T51] Scala：Hello World
来源：http://kos.shangyingyoupin.top

println("Hello")
来源：http://two.sweek.top

[T52] Scala：变量
来源：http://pln.yangfankeji.com

val a = 1;  var b = 2
来源：http://qog.chenzaomai.com

[T53] Scala：字符串插值
来源：http://wap.daxiang520.top

s"值: $b"
来源：http://hny.chenjidiqi.icu

[T54] Scala：集合映射
来源：http://mdk.redwolf501.top

List(1, 2, 3).map(_ * 2)
来源：http://toa.ctjpmb.com

[T55] Scala：集合过滤
来源：http://hhc.jianghu66.top

List(1, 2, 3).filter(_ > 1)
来源：http://qgc.sxryk.cn

[T56] Scala：样例类
来源：http://ady.redwolf501.top

case class User(name: String, age: Int)
来源：http://yvj.zhoulong.xyz

[T57] Scala：模式匹配
来源：http://fdl.yuanzhike.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://npv.cashguo.top

[T58] Scala：函数定义
来源：http://vaq.guannengcc.top

def add(a: Int, b: Int): Int = a + b
来源：http://lmw.jianghu66.top

[T59] Scala：循环
来源：http://nrt.jinqigufen.top

for (i <- 1 to 10) println(i)
来源：http://qcs.nanxuanxn.top

[T60] Scala：折叠
来源：http://qpi.ctjpmb.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vyi.vehdjk.com

================================================================================
来源：http://uwk.hfpthk.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ofc.xingfuxueyuan.xyz

================================================================================
来源：http://vte.daria6918.cn

[U01] Py：创建虚拟环境
来源：http://clg.jinyuanbaomall.cn

python -m venv .venv && source .venv/bin/activate
来源：http://dbu.xinyue.icu

[U02] Py：导出 / 安装依赖
来源：http://vxl.tarul.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ftp.cdnleiting.top

[U03] Py：加载 .env 配置
来源：http://wlm.birdmap.top

from dotenv import load_dotenv; load_dotenv()
来源：http://ary.tanke756.top

[U04] Py：变量调试打印
来源：http://pqk.shangyingyoupin.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ruh.jlsjyb.cn

[U05] Py：列表去重且保序
来源：http://iwm.tarul.cn

list(dict.fromkeys(arr))
来源：http://vej.sxryk.cn

[U06] Py：合并两个字典
来源：http://ukl.ehwqpu.com

{**a, **b}
来源：http://eyg.jianghu66.top

[U07] Py：反转字典键值
来源：http://qpn.0kj1m.cn

{v: k for k, v in d.items()}
来源：http://grp.aibaodan.cn

[U08] Py：展平二维列表
来源：http://sef.ppjwa.cn

[y for x in nested for y in x]
来源：http://pqi.yueranfly.top

[U09] Py：字典取最大值的键
来源：http://ifg.nanxuanxn.top

max(d, key=d.get)
来源：http://npq.yvedp.cn

[U10] Py：按值排序字典
来源：http://tid.iojbl.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lau.ybcxt.top

[U11] Py：生成器表达式
来源：http://xlq.0kj1m.cn

(x * 2 for x in arr)
来源：http://auf.dashuyun.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mrg.meibo888.top

Counter(arr).most_common(3)
来源：http://eop.yuxming.cn


<!-- 参考信息 -->