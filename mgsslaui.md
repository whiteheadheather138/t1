代发 wailian999

split -l 1000 big.log part_
来源：http://hix.feifeiyinyue.top

[R74] 批量重命名
来源：http://prj.jianghu66.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://asa.cucudq.cn

[R75] 导出环境变量
来源：http://hqe.ehwqpu.com

export PATH="$HOME/bin:$PATH"
来源：http://fbi.daria6918.cn

[R76] 使用临时文件
来源：http://ojt.sysykeji.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://eeo.yj20258888.top

[R77] 读取用户输入
来源：http://fcp.ybcxt.top

read -rp "请输入: " ans
来源：http://swf.dianchejie.cn

[R78] 交互式菜单
来源：http://kah.ydzc1.top

select opt in a b c; do echo "$opt"; break; done
来源：http://bab.jiagoushi.top

[R79] 解析命令行选项
来源：http://gwb.daxiang520.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://esl.jqgufenzy.top

[R80] 查看脚本执行耗时
来源：http://tvg.yj20258.top

time ./run.sh
来源：http://fbi.nanxuanxn.top

================================================================================
来源：http://tsu.hfpthk.cn

S. C / C++ 专题
来源：http://xcw.shzxlz.cn

================================================================================
来源：http://uuz.hfpthk.cn

[S01] C：Hello World
来源：http://yky.cdnleiting.top

#include <stdio.h>
来源：http://die.xuanzx.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://ikg.shuidangran.top

[S02] C：变量与格式化输出
来源：http://zkz.birdmap.top

int a = 10; printf("%d\n", a);
来源：http://bgz.sjlbkw.cn

[S03] C：读入整数
来源：http://ndj.sweek.top

int x; scanf("%d", &x);
来源：http://jql.vehdjk.com

[S04] C：字符串复制
来源：http://duk.shangyingyoupin.top

char dst[32]; strcpy(dst, "hi");
来源：http://weo.fktsv.cn

[S05] C：字符串长度
来源：http://erk.nanxuanxn.top

strlen(s)
来源：http://lmn.jinghuilouyu.cn

[S06] C：字符串比较
来源：http://wga.fktsv.cn

strcmp(a, b) == 0
来源：http://fxg.snrcjt.cn

[S07] C：数组遍历求和
来源：http://mfp.jianghu66.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tvh.yuanzhike.top

[S08] C：动态内存分配与释放
来源：http://lhc.shuidangran.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tzu.andypj.xyz

[S09] C：结构体定义与初始化
来源：http://vnk.snrcjt.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ief.jinqigfzy.top

[S10] C：指针与解引用
来源：http://afu.yongpay.top

int *p = &a;  *p = 5;
来源：http://vus.9152youxi.cn

[S11] C：逐行读文件
来源：http://hpj.yueranfly.top

FILE *f = fopen("a.txt", "r");
来源：http://jav.tianlin.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://dgp.shuidangran.top

fclose(f);
来源：http://esq.shanyushiyangkeji.top

[S12] C：写文件
来源：http://ezd.ybcxt.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rnd.vehdjk.com

[S13] C：宏定义
来源：http://aqz.guowangkeji.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hmz.c1oappe.top

[S14] C：枚举
来源：http://irm.zhoulong.xyz

enum Color { RED, GREEN, BLUE };
来源：http://doc.snrcjt.cn

[S15] C：类型转换
来源：http://fta.jyoumei.cn

(double) a / b
来源：http://pmz.zdqjudy.top

[S16] C：位操作置位
来源：http://pxp.havefunace.top

x |= (1 << 3);
来源：http://xgl.chenjidiqi.icu

[S17] C：安全拼接字符串
来源：http://bvf.cdnleiting.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yzq.chenzaomai.com

[S18] C：命令行参数
来源：http://edr.wangshuangyany.cn

int main(int argc, char **argv)
来源：http://ykn.epnwcf.com

[S19] C：快速排序
来源：http://mvc.xingfuxueyuan.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://bpy.zhoulong.xyz

[S20] C：二分查找
来源：http://pyh.hesvh.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yue.gotoacloud.top

[S21] C：字符类别判断
来源：http://bvt.aizwys.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vep.pengpengdd.cyou

[S22] C：字符串转数字
来源：http://gjm.gogol.net.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ggs.aibaodan.cn

[S23] C：随机数
来源：http://tpk.pengpengdd.cyou

srand(time(NULL));  int r = rand() % 100;
来源：http://nri.feifeiyinyue.top

[S24] C：获取本地时间
来源：http://dcm.hammf.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vww.gogol.net.cn

[S25] C：内存拷贝
来源：http://zgr.yonumen.top

memcpy(dst, src, n);
来源：http://syo.wangdashe.top

[S26] C：内存清零
来源：http://rys.hnxiangtu.top

memset(a, 0, sizeof a);
来源：http://qyy.hammf.cn

[S27] C：定义常量
来源：http://jjq.nwbrower.top

const double PI = 3.14159;
来源：http://uud.jinyuanbaomall.cn

[S28] C：静态变量
来源：http://flv.xuetiantiany.cn

static int counter = 0;
来源：http://twy.yfazqb.com

[S29] C：变参函数
来源：http://tey.cashguo.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tvw.shzxlz.cn

[S30] C：头文件保护
来源：http://syf.yongpay.top

#ifndef X_H
来源：http://pos.yangfankeji.com

#define X_H
来源：http://peg.sufxvd.cn

#endif
来源：http://skl.ybcxt.top

[S31] C++：Hello World
来源：http://ygt.yanxiufei.cn

#include <iostream>
来源：http://hho.daxiang520.top

int main() { std::cout << "Hello\n"; }
来源：http://djb.daria6918.cn

[S32] C++：字符串
来源：http://vky.chenzaomai.com

std::string s = "hi";  s += "!";
来源：http://amw.ywan-chungtsiang.top

[S33] C++：vector 增删
来源：http://zgz.jqgufenzy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gtn.hysaishi.cn

[S34] C++：遍历 vector
来源：http://qju.fanxiaobao.xyz

for (auto &x : v) { std::cout << x; }
来源：http://aad.epnwcf.com

[S35] C++：map
来源：http://ytv.jqgfzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qeq.hesvh.cn

[S36] C++：unordered_map
来源：http://nmp.sjlbkw.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vdi.yfazqb.com

[S37] C++：set
来源：http://saf.redwolf501.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rcl.xinyue.icu

[S38] C++：排序
来源：http://smx.tarul.cn

std::sort(v.begin(), v.end());
来源：http://hre.zhiwuduotai.top

[S39] C++：自定义比较器排序
来源：http://aun.jianghu66.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hcz.daxiang520.top

[S40] C++：查找元素
来源：http://bnm.kuanghao11.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ish.yonumen.top

[S41] C++：类与构造函数
来源：http://zww.jinqigufen.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qjd.hfpthk.cn

[S42] C++：继承与虚函数
来源：http://dpw.hammf.cn

class B : public Base { public: void f() override {} };
来源：http://nud.xuanzx.com

[S43] C++：智能指针
来源：http://vha.cqqwz.cn

auto p = std::make_unique<int>(5);
来源：http://hrl.fengsongda.top

[S44] C++：引用传参
来源：http://yfd.chenzaomai.com

void inc(int &x) { ++x; }
来源：http://wzl.yuxming.cn

[S45] C++：lambda
来源：http://hvw.gogol.net.cn

auto add = [](int a, int b) { return a + b; };
来源：http://abq.316326.xyz

[S46] C++：函数模板
来源：http://nbt.yanxiufei.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vkt.yueranfly.top

[S47] C++：结构化绑定遍历
来源：http://qfu.xuanzx.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lxt.hnqzz.top

[S48] C++：逐行读文件
来源：http://yke.52xcode.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zaj.kuanghao11.cn

while (std::getline(in, line)) { }
来源：http://eho.xziqi.cn

[S49] C++：写文件
来源：http://gww.tianlin.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kxf.nanxuanxn.top

[S50] C++：格式化数字
来源：http://iug.cashguo.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kal.xylfe.cn

[S51] C++：显式类型转换
来源：http://lgp.cqqwz.cn

static_cast<double>(a) / b
来源：http://ryx.chenzaomai.com

[S52] C++：const 与 noexcept
来源：http://bht.zdbjq.cn

int size() const noexcept { return n_; }
来源：http://pva.cheryme.top

[S53] C++：移动语义
来源：http://jnd.bjfxy.top

std::vector<int> w = std::move(v);
来源：http://kki.fehbvm.com

[S54] C++：异常处理
来源：http://qeh.daria6918.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://smn.jinyuanbaomall.cn

[S55] C++：结构化绑定
来源：http://ant.epnwcf.com

auto [a, b] = std::make_pair(1, 2);
来源：http://krp.xinyue.icu

[S56] C++：optional
来源：http://czk.hammf.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://aeq.guannengcc.top

[S57] C++：编译期常量
来源：http://yis.zhijiandao.cn

constexpr int N = 10;
来源：http://jqd.gogol.net.cn

[S58] C++：命名空间
来源：http://ayu.sjlbkw.cn

namespace ns { int f() { return 1; } }
来源：http://mmo.meibo888.top

[S59] C++：静态断言
来源：http://dbj.xuanzx.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bik.hywenlv.cn

[S60] C++：遍历并删除元素
来源：http://lut.zdbjq.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fab.guowangkeji.top

================================================================================
来源：http://vop.guannengcc.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gdq.feifeiyinyue.top

================================================================================
来源：http://ciu.ywan-chungtsiang.top

[T01] Kotlin：Hello World
来源：http://blq.zhijiandao.cn

println("Hello")
来源：http://bvj.yj20258888.top

[T02] Kotlin：变量
来源：http://hlp.epnwcf.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mqc.andypj.xyz

[T03] Kotlin：字符串模板
来源：http://tiw.aizwys.cn

"值: $b"
来源：http://rhc.uphjek.com

[T04] Kotlin：空安全
来源：http://vzz.ybcxt.top

val n: String? = null;  n?.length
来源：http://bgf.wangdashe.top

[T05] Kotlin：when 表达式
来源：http://cwf.jyoumei.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qsj.snrcjt.cn

[T06] Kotlin：集合映射
来源：http://wyw.jlsjyb.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ieo.fengsongda.top

[T07] Kotlin：集合过滤
来源：http://ecm.tian-w.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://cev.guannengcc.top

[T08] Kotlin：数据类
来源：http://djq.gaohongyu789.top

data class User(val name: String, val age: Int)
来源：http://par.yongpay.top

[T09] Kotlin：扩展函数
来源：http://xov.dianchejie.cn

fun String.exclaim() = this + "!"
来源：http://alj.xingfuxueyuan.xyz

[T10] Kotlin：默认参数
来源：http://sri.cheryme.top

fun greet(name: String = "World") = "Hi $name"
来源：http://fer.ehwqpu.com

[T11] Kotlin：协程
来源：http://abx.52xcode.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://kww.havefunace.top

[T12] Kotlin：解构声明
来源：http://fxq.zhaomingkeji.xyz

val (a, b) = Pair(1, 2)
来源：http://eke.jqgfzy.top

[T13] Kotlin：只读 Map
来源：http://zaa.jinqigfzy.top

val m = mapOf("a" to 1)
来源：http://jxw.fehbvm.com

[T14] Kotlin：循环
来源：http://vka.xinyue.icu

for (i in 1..10) println(i)
来源：http://aoi.hammf.cn

[T15] Kotlin：接口
来源：http://svj.daria6918.cn

interface Shape { fun area(): Double }
来源：http://jtp.gogol.net.cn

[T16] Swift：Hello World
来源：http://iuu.haohaochexian.top

print("Hello")
来源：http://uzt.sufxvd.cn

[T17] Swift：变量与常量
来源：http://vwj.fanxiaobao.xyz

var a = 1;  let b = 2
来源：http://xaw.9152youxi.cn

[T18] Swift：字符串插值
来源：http://rpj.hcnkem.com

"值: \(b)"
来源：http://fda.gaohongyu789.top

[T19] Swift：可选绑定
来源：http://nua.yj202588.top

if let n = opt { print(n) }
来源：http://ajg.yfazqb.com

[T20] Swift：数组操作
来源：http://ntr.shuidangran.top

var a = [1, 2, 3];  a.append(4)
来源：http://iim.fzhhl.top

[T21] Swift：遍历
来源：http://xar.hfpthk.cn

for x in a { print(x) }
来源：http://cls.svipenyu.cn

[T22] Swift：字典
来源：http://hcr.cqqwz.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ywm.tianlin.xyz

[T23] Swift：函数
来源：http://obw.xingfuxueyuan.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xnm.wangshuangyany.cn

[T24] Swift：闭包
来源：http://aro.yuxming.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vkr.zdbjq.cn

[T25] Swift：结构体
来源：http://nrq.kuanghao11.cn

struct P { var x: Int }
来源：http://vzn.shangyingyoupin.top

[T26] Swift：类与重写
来源：http://dfu.zhixingplan.top

class A: Base { override func f() {} }
来源：http://fsp.jlsjyb.cn

[T27] Swift：错误处理
来源：http://swp.cashguo.top

do { try f() } catch { print(error) }
来源：http://hlt.hywenlv.cn

[T28] Swift：枚举
来源：http://une.aibaodan.cn

enum Color { case red, green }
来源：http://mms.sweek.top

[T29] Swift：guard 提前返回
来源：http://hwd.jqgfzy.top

guard let x = opt else { return }
来源：http://sfr.gzhubu.top

[T30] Swift：协议
来源：http://wvw.ybcxt.top

protocol Shape { func area() -> Double }
来源：http://axj.nanxuanxn.top

[T31] Lua：Hello World
来源：http://qcx.xylfe.cn

print("Hello")
来源：http://loa.yj20258.top

[T32] Lua：局部变量
来源：http://rto.yj20258.top

local a = 1
来源：http://cie.chenlongwang.top

[T33] Lua：表（数组）
来源：http://yed.shuidangran.top

local t = {1, 2, 3};  t[4] = 4
来源：http://otn.cdnleiting.top

[T34] Lua：遍历表
来源：http://twu.gogol.net.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://kql.iojbl.cn

[T35] Lua：字典表
来源：http://qpk.gaohongyu789.top

local d = { a = 1 };  d.b = 2
来源：http://ddo.jlsjyb.cn

[T36] Lua：函数
来源：http://sbi.0kj1m.cn

function add(a, b) return a + b end
来源：http://nim.xziqi.cn

[T37] Lua：字符串拼接
来源：http://hcc.cheryme.top

"a" .. "b"
来源：http://qqe.tarul.cn

[T38] Lua：条件
来源：http://qiq.yanxiufei.cn

if x > 0 then print("正") end
来源：http://zyu.fengsongda.top

[T39] Lua：模式匹配
来源：http://pkl.52xcode.cn

string.find(s, "%d+")
来源：http://ubh.kuanghao11.cn

[T40] Lua：元表
来源：http://itr.fktsv.cn

setmetatable({}, { __index = base })
来源：http://ojm.pycfn.com

[T41] Perl：Hello World
来源：http://ycx.cdnleiting.top

print "Hello\n";
来源：http://lbk.gzhubu.top

[T42] Perl：变量类型
来源：http://urv.yj20258.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://aqo.shangyingyoupin.top

[T43] Perl：字符串插值
来源：http://nur.yj20258.top

"值: $a"
来源：http://wuw.yvedp.cn

[T44] Perl：条件
来源：http://tvg.zhaomingkeji.xyz

if ($a > 0) { print "正"; }
来源：http://dna.xylfe.cn

[T45] Perl：数组遍历
来源：http://kno.9152youxi.cn

for my $x (@arr) { print $x; }
来源：http://tcu.tianlin.xyz

[T46] Perl：哈希操作
来源：http://dzx.xuanzx.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gna.nanxuanxn.top

[T47] Perl：正则捕获
来源：http://ueg.sweek.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://mgs.tian-w.cn

[T48] Perl：正则替换
来源：http://tch.yonumen.top

$s =~ s/old/new/g;
来源：http://aqy.daxiang520.top

[T49] Perl：函数
来源：http://mpr.zycfv.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://krq.0kj1m.cn

[T50] Perl：逐行读文件
来源：http://agw.jlsjyb.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://iab.fzhhl.top

while (my $line = <$fh>) { print $line; }
来源：http://xes.feifeiyinyue.top

[T51] Scala：Hello World
来源：http://iiv.52xcode.cn

println("Hello")
来源：http://ylo.52xcode.cn

[T52] Scala：变量
来源：http://bad.andypj.xyz

val a = 1;  var b = 2
来源：http://rle.nanxuanxn.top

[T53] Scala：字符串插值
来源：http://ylg.xylfe.cn

s"值: $b"
来源：http://pdo.birdmap.top

[T54] Scala：集合映射
来源：http://ulm.dianchejie.cn

List(1, 2, 3).map(_ * 2)
来源：http://sat.vqdsnc.cn

[T55] Scala：集合过滤
来源：http://nlx.cashguo.top

List(1, 2, 3).filter(_ > 1)
来源：http://cig.guowangkeji.top

[T56] Scala：样例类
来源：http://hzd.chenzaomai.com

case class User(name: String, age: Int)
来源：http://jcc.tianlin.xyz

[T57] Scala：模式匹配
来源：http://dac.jlsjyb.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://qua.hywenlv.cn

[T58] Scala：函数定义
来源：http://slz.fktsv.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ora.yonumen.top

[T59] Scala：循环
来源：http://zkk.yj20258.top

for (i <- 1 to 10) println(i)
来源：http://wtp.yj202588.top

[T60] Scala：折叠
来源：http://gwl.ehwqpu.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cyn.ctjpmb.com

================================================================================
来源：http://wyj.yongpay.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vyx.316326.xyz

================================================================================
来源：http://wfr.xingfuxueyuan.xyz

[U01] Py：创建虚拟环境
来源：http://wqq.ywan-chungtsiang.top

python -m venv .venv && source .venv/bin/activate
来源：http://ytc.ctjpmb.com

[U02] Py：导出 / 安装依赖
来源：http://ohy.shzxlz.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://iqb.nanxuanxn.top

[U03] Py：加载 .env 配置
来源：http://oea.0kj1m.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://mrw.hammf.cn

[U04] Py：变量调试打印
来源：http://bpk.vqdsnc.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dhj.dianchejie.cn

[U05] Py：列表去重且保序
来源：http://lnq.zdqjudy.top

list(dict.fromkeys(arr))
来源：http://ska.shangyingyoupin.top

[U06] Py：合并两个字典
来源：http://dsj.sysykeji.top

{**a, **b}
来源：http://zcz.yj202588.top

[U07] Py：反转字典键值
来源：http://xkh.cheryme.top

{v: k for k, v in d.items()}
来源：http://vri.vqdsnc.cn

[U08] Py：展平二维列表
来源：http://cwj.zdqjudy.top

[y for x in nested for y in x]
来源：http://gtv.wangdashe.top

[U09] Py：字典取最大值的键
来源：http://tpb.zhiwuduotai.top

max(d, key=d.get)
来源：http://uyp.zycfv.cn

[U10] Py：按值排序字典
来源：http://lsp.zycfv.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bnm.yueranfly.top

[U11] Py：生成器表达式
来源：http://adv.yfazqb.com

(x * 2 for x in arr)
来源：http://esr.tanke756.top

[U12] Py：取出现最多的 3 个元素
来源：http://anu.tanke756.top

Counter(arr).most_common(3)
来源：http://fik.xinyue.icu

[U13] Py：固定长度队列
来源：http://unw.cashguo.top

deque(maxlen=10)
来源：http://dka.yj202588.top

[U14] Py：分组收集到列表
来源：http://tih.ctjpmb.com

defaultdict(list)
来源：http://qch.c1oappe.top


<!-- 参考信息 -->