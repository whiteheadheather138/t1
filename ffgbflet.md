代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://fjf.sjlbkw.cn

[R76] 使用临时文件
来源：http://zph.vqdsnc.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gcs.zdbjq.cn

[R77] 读取用户输入
来源：http://ybd.zycfv.cn

read -rp "请输入: " ans
来源：http://tuv.xinyue.icu

[R78] 交互式菜单
来源：http://jbb.shanyushiyangkeji.top

select opt in a b c; do echo "$opt"; break; done
来源：http://pjj.nanxuanxn.top

[R79] 解析命令行选项
来源：http://lyn.316326.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bvr.hammf.cn

[R80] 查看脚本执行耗时
来源：http://eyr.xziqi.cn

time ./run.sh
来源：http://heh.sufxvd.cn

================================================================================
来源：http://vqw.zhixingplan.top

S. C / C++ 专题
来源：http://ffr.jyoumei.cn

================================================================================
来源：http://bau.zhaomingkeji.xyz

[S01] C：Hello World
来源：http://jbg.sufxvd.cn

#include <stdio.h>
来源：http://lbn.jinqigfzy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://jhj.ydjk.org.cn

[S02] C：变量与格式化输出
来源：http://ius.fktsv.cn

int a = 10; printf("%d\n", a);
来源：http://nte.uphjek.com

[S03] C：读入整数
来源：http://ezg.vehdjk.com

int x; scanf("%d", &x);
来源：http://vwb.snrcjt.cn

[S04] C：字符串复制
来源：http://omj.sysykeji.top

char dst[32]; strcpy(dst, "hi");
来源：http://unq.sweek.top

[S05] C：字符串长度
来源：http://bbr.fktsv.cn

strlen(s)
来源：http://rls.tanke756.top

[S06] C：字符串比较
来源：http://lqf.yuanzhike.top

strcmp(a, b) == 0
来源：http://duv.yfazqb.com

[S07] C：数组遍历求和
来源：http://gwv.zhengqikj.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yyb.ctjpmb.com

[S08] C：动态内存分配与释放
来源：http://lzp.vehdjk.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tac.cashguo.top

[S09] C：结构体定义与初始化
来源：http://ads.bjfxy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jrg.yvedp.cn

[S10] C：指针与解引用
来源：http://hot.fengsongda.top

int *p = &a;  *p = 5;
来源：http://swi.hysaishi.cn

[S11] C：逐行读文件
来源：http://zgd.haohaochexian.top

FILE *f = fopen("a.txt", "r");
来源：http://tat.gotoacloud.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://wzz.smart0.xyz

fclose(f);
来源：http://yfs.zycfv.cn

[S12] C：写文件
来源：http://uyy.chenjidiqi.icu

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fgp.xuetiantiany.cn

[S13] C：宏定义
来源：http://jsv.gogol.net.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pgn.smart0.xyz

[S14] C：枚举
来源：http://mwm.andypj.xyz

enum Color { RED, GREEN, BLUE };
来源：http://wor.ctjpmb.com

[S15] C：类型转换
来源：http://kvk.yuanzhike.top

(double) a / b
来源：http://cxk.epnwcf.com

[S16] C：位操作置位
来源：http://qsq.cheryme.top

x |= (1 << 3);
来源：http://cas.jinqigfzy.top

[S17] C：安全拼接字符串
来源：http://nrl.chenzaomai.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pjs.fktsv.cn

[S18] C：命令行参数
来源：http://zdg.zycfv.cn

int main(int argc, char **argv)
来源：http://puz.jinqigfzy.top

[S19] C：快速排序
来源：http://agt.tianlin.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://ddg.cdnleiting.top

[S20] C：二分查找
来源：http://ycz.shanyushiyangtech.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zpv.redwolf501.top

[S21] C：字符类别判断
来源：http://azb.epnwcf.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ghq.ppjwa.cn

[S22] C：字符串转数字
来源：http://uky.hnxiangtu.top

atoi("42");  strtod("3.14", NULL);
来源：http://kfd.fzhhl.top

[S23] C：随机数
来源：http://hke.nanxinkj.top

srand(time(NULL));  int r = rand() % 100;
来源：http://odm.aibaodan.cn

[S24] C：获取本地时间
来源：http://weu.sxryk.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cki.wangdashe.top

[S25] C：内存拷贝
来源：http://ebs.tanke756.top

memcpy(dst, src, n);
来源：http://roh.52xcode.cn

[S26] C：内存清零
来源：http://wem.dashuyun.cn

memset(a, 0, sizeof a);
来源：http://ldv.nanxuanxn.top

[S27] C：定义常量
来源：http://hej.shuidangran.top

const double PI = 3.14159;
来源：http://yxa.pycfn.com

[S28] C：静态变量
来源：http://zze.wangdashe.top

static int counter = 0;
来源：http://lft.kuanghao11.cn

[S29] C：变参函数
来源：http://nqg.yfazqb.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vzt.mhx1999.top

[S30] C：头文件保护
来源：http://xad.fengsongda.top

#ifndef X_H
来源：http://sso.yj20258888.top

#define X_H
来源：http://jby.52xcode.cn

#endif
来源：http://ekp.yangfankeji.com

[S31] C++：Hello World
来源：http://ret.zdbjq.cn

#include <iostream>
来源：http://cdr.yuanzhike.top

int main() { std::cout << "Hello\n"; }
来源：http://gqi.zhiwuduotai.top

[S32] C++：字符串
来源：http://yai.svipenyu.cn

std::string s = "hi";  s += "!";
来源：http://gql.kuanghao11.cn

[S33] C++：vector 增删
来源：http://awk.cqqwz.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dfi.xuetiantiany.cn

[S34] C++：遍历 vector
来源：http://vdx.jyoumei.cn

for (auto &x : v) { std::cout << x; }
来源：http://ofh.daria6918.cn

[S35] C++：map
来源：http://bll.zhoulong.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://odn.shuidangran.top

[S36] C++：unordered_map
来源：http://qgb.epnwcf.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://aon.zhengqikj.top

[S37] C++：set
来源：http://sel.gzhubu.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lgp.ydzc1.top

[S38] C++：排序
来源：http://twl.sweek.top

std::sort(v.begin(), v.end());
来源：http://fdz.daxiang520.top

[S39] C++：自定义比较器排序
来源：http://phs.daria6918.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lgj.jinghuilouyu.cn

[S40] C++：查找元素
来源：http://hcg.guannengcc.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dwf.yanxiufei.cn

[S41] C++：类与构造函数
来源：http://kcu.shuidangran.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dqe.yangfankeji.com

[S42] C++：继承与虚函数
来源：http://mln.jinyuanbaomall.cn

class B : public Base { public: void f() override {} };
来源：http://aot.zhongyouzk.top

[S43] C++：智能指针
来源：http://hkm.shanyushiyangtech.top

auto p = std::make_unique<int>(5);
来源：http://llq.nwbrower.top

[S44] C++：引用传参
来源：http://udv.wangshuangyany.cn

void inc(int &x) { ++x; }
来源：http://xgm.cashguo.top

[S45] C++：lambda
来源：http://nzg.hysaishi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://kdw.bjfxy.top

[S46] C++：函数模板
来源：http://wfs.wangshuangyany.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vjk.hysaishi.cn

[S47] C++：结构化绑定遍历
来源：http://xhx.jinqigfzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ikt.316326.xyz

[S48] C++：逐行读文件
来源：http://eqn.hysaishi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qju.shangyingyoupin.top

while (std::getline(in, line)) { }
来源：http://dah.sufxvd.cn

[S49] C++：写文件
来源：http://qeg.zhongyouzk.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bfz.guowangkeji.top

[S50] C++：格式化数字
来源：http://xdv.feifeiyinyue.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yll.sxryk.cn

[S51] C++：显式类型转换
来源：http://qdn.jyoumei.cn

static_cast<double>(a) / b
来源：http://hck.iojbl.cn

[S52] C++：const 与 noexcept
来源：http://uci.zhoulong.xyz

int size() const noexcept { return n_; }
来源：http://jwq.ivvv.top

[S53] C++：移动语义
来源：http://ebg.yvedp.cn

std::vector<int> w = std::move(v);
来源：http://gzt.yanxiufei.cn

[S54] C++：异常处理
来源：http://cag.pycfn.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gjw.fehbvm.com

[S55] C++：结构化绑定
来源：http://ltd.daria6918.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://lvr.cheryme.top

[S56] C++：optional
来源：http://vli.smart0.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jzw.tianlin.xyz

[S57] C++：编译期常量
来源：http://pgy.gogol.net.cn

constexpr int N = 10;
来源：http://ckl.ppjwa.cn

[S58] C++：命名空间
来源：http://yet.ctjpmb.com

namespace ns { int f() { return 1; } }
来源：http://hyb.havefunace.top

[S59] C++：静态断言
来源：http://ggq.xuanzx.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://glq.jinyuanbaomall.cn

[S60] C++：遍历并删除元素
来源：http://bkm.fanxiaobao.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rqs.tanke756.top

================================================================================
来源：http://gre.birdmap.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://emy.tanke756.top

================================================================================
来源：http://tgg.zhengqikj.top

[T01] Kotlin：Hello World
来源：http://zsy.kuanghao11.cn

println("Hello")
来源：http://cka.pengpengdd.cyou

[T02] Kotlin：变量
来源：http://nxb.zycfv.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lgb.aizwys.cn

[T03] Kotlin：字符串模板
来源：http://ubj.yanxiufei.cn

"值: $b"
来源：http://eay.zhijiandao.cn

[T04] Kotlin：空安全
来源：http://hfr.yongpay.top

val n: String? = null;  n?.length
来源：http://qqm.hcnkem.com

[T05] Kotlin：when 表达式
来源：http://bkl.316326.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wae.yonumen.top

[T06] Kotlin：集合映射
来源：http://pwv.dashuyun.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://bos.cheryme.top

[T07] Kotlin：集合过滤
来源：http://edw.xuetiantiany.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://tnq.andypj.xyz

[T08] Kotlin：数据类
来源：http://hzx.hnxiangtu.top

data class User(val name: String, val age: Int)
来源：http://gxs.shanyushiyangkeji.top

[T09] Kotlin：扩展函数
来源：http://cqx.ydzc1.top

fun String.exclaim() = this + "!"
来源：http://qhp.hywenlv.cn

[T10] Kotlin：默认参数
来源：http://jpn.jinyuanbaomall.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://dqo.nanxinkj.top

[T11] Kotlin：协程
来源：http://vwx.jlsjyb.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ibh.meibo888.top

[T12] Kotlin：解构声明
来源：http://hun.wangdashe.top

val (a, b) = Pair(1, 2)
来源：http://ftc.sufxvd.cn

[T13] Kotlin：只读 Map
来源：http://mnx.havefunace.top

val m = mapOf("a" to 1)
来源：http://yjx.quarkkingdee.top

[T14] Kotlin：循环
来源：http://lxj.birdmap.top

for (i in 1..10) println(i)
来源：http://ouv.chenzaomai.com

[T15] Kotlin：接口
来源：http://pmk.andypj.xyz

interface Shape { fun area(): Double }
来源：http://vih.jlsjyb.cn

[T16] Swift：Hello World
来源：http://mnl.yueranfly.top

print("Hello")
来源：http://evd.hfpthk.cn

[T17] Swift：变量与常量
来源：http://nnt.bjfxy.top

var a = 1;  let b = 2
来源：http://jae.epnwcf.com

[T18] Swift：字符串插值
来源：http://dbo.gotoacloud.top

"值: \(b)"
来源：http://xqg.shzxlz.cn

[T19] Swift：可选绑定
来源：http://jcv.gotoacloud.top

if let n = opt { print(n) }
来源：http://xns.bbcook.cn

[T20] Swift：数组操作
来源：http://wfo.wangshuangyany.cn

var a = [1, 2, 3];  a.append(4)
来源：http://juo.cashguo.top

[T21] Swift：遍历
来源：http://prd.tian-w.cn

for x in a { print(x) }
来源：http://cmx.jqgfzy.top

[T22] Swift：字典
来源：http://uyo.52xcode.cn

var d = ["a": 1];  d["b"] = 2
来源：http://pko.andypj.xyz

[T23] Swift：函数
来源：http://pgr.zhongyouzk.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fwk.vehdjk.com

[T24] Swift：闭包
来源：http://hrm.iojbl.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://sis.epnwcf.com

[T25] Swift：结构体
来源：http://tfa.shanyushiyangtech.top

struct P { var x: Int }
来源：http://qno.jinghuilouyu.cn

[T26] Swift：类与重写
来源：http://gzl.cucudq.cn

class A: Base { override func f() {} }
来源：http://bsx.jinqigufen.top

[T27] Swift：错误处理
来源：http://aps.wangdashe.top

do { try f() } catch { print(error) }
来源：http://afn.jqgufenzy.top

[T28] Swift：枚举
来源：http://yjd.nwbrower.top

enum Color { case red, green }
来源：http://yhb.gzhubu.top

[T29] Swift：guard 提前返回
来源：http://kve.ivvv.top

guard let x = opt else { return }
来源：http://bhf.hfpthk.cn

[T30] Swift：协议
来源：http://moy.jlsjyb.cn

protocol Shape { func area() -> Double }
来源：http://cst.zhongyouzk.top

[T31] Lua：Hello World
来源：http://ory.gogol.net.cn

print("Hello")
来源：http://igy.xylfe.cn

[T32] Lua：局部变量
来源：http://jsy.chenlongwang.top

local a = 1
来源：http://zcx.yj20258888.top

[T33] Lua：表（数组）
来源：http://tdg.gzhubu.top

local t = {1, 2, 3};  t[4] = 4
来源：http://pqj.vehdjk.com

[T34] Lua：遍历表
来源：http://xxu.yj20258.top

for i, v in ipairs(t) do print(i, v) end
来源：http://oei.hesvh.cn

[T35] Lua：字典表
来源：http://nek.cdnleiting.top

local d = { a = 1 };  d.b = 2
来源：http://yts.cucudq.cn

[T36] Lua：函数
来源：http://jwe.shangyingyoupin.top

function add(a, b) return a + b end
来源：http://voi.wangshuangyany.cn

[T37] Lua：字符串拼接
来源：http://gxn.pengpengdd.cyou

"a" .. "b"
来源：http://kjp.ctjpmb.com

[T38] Lua：条件
来源：http://qnc.tianlin.xyz

if x > 0 then print("正") end
来源：http://rpr.vqdsnc.cn

[T39] Lua：模式匹配
来源：http://efs.ehwqpu.com

string.find(s, "%d+")
来源：http://tby.svipenyu.cn

[T40] Lua：元表
来源：http://ymj.sweek.top

setmetatable({}, { __index = base })
来源：http://eva.fzhhl.top

[T41] Perl：Hello World
来源：http://gjw.jlsjyb.cn

print "Hello\n";
来源：http://nqd.zycfv.cn

[T42] Perl：变量类型
来源：http://wdq.316326.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nyl.gogol.net.cn

[T43] Perl：字符串插值
来源：http://eiq.yueranfly.top

"值: $a"
来源：http://odf.bbcook.cn

[T44] Perl：条件
来源：http://llk.hcnkem.com

if ($a > 0) { print "正"; }
来源：http://kse.zhoulong.xyz

[T45] Perl：数组遍历
来源：http://kxt.yangfankeji.com

for my $x (@arr) { print $x; }
来源：http://ydh.yongpay.top

[T46] Perl：哈希操作
来源：http://cmj.dianchejie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kon.chenjidiqi.icu

[T47] Perl：正则捕获
来源：http://nwy.hammf.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qwe.yuanzhike.top

[T48] Perl：正则替换
来源：http://mzv.yanxiufei.cn

$s =~ s/old/new/g;
来源：http://jaj.sxryk.cn

[T49] Perl：函数
来源：http://pyd.haohaochexian.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bxu.daria6918.cn

[T50] Perl：逐行读文件
来源：http://yyy.xinyue.icu

open my $fh, "<", "a.txt" or die $!;
来源：http://cpg.9152youxi.cn

while (my $line = <$fh>) { print $line; }
来源：http://exy.wangshuangyany.cn

[T51] Scala：Hello World
来源：http://gqh.hnxiangtu.top

println("Hello")
来源：http://rsg.0kj1m.cn

[T52] Scala：变量
来源：http://pmj.9152youxi.cn

val a = 1;  var b = 2
来源：http://vxb.fengsongda.top

[T53] Scala：字符串插值
来源：http://hbk.yuxming.cn

s"值: $b"
来源：http://ftf.havefunace.top

[T54] Scala：集合映射
来源：http://gat.vqdsnc.cn

List(1, 2, 3).map(_ * 2)
来源：http://wwz.sweek.top

[T55] Scala：集合过滤
来源：http://qeb.jqgfzy.top

List(1, 2, 3).filter(_ > 1)
来源：http://gga.hnxiangtu.top

[T56] Scala：样例类
来源：http://tdh.zhoulong.xyz

case class User(name: String, age: Int)
来源：http://qvg.dashuyun.cn

[T57] Scala：模式匹配
来源：http://zpf.cucudq.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vqq.cqqwz.cn

[T58] Scala：函数定义
来源：http://ehu.birdmap.top

def add(a: Int, b: Int): Int = a + b
来源：http://ubl.jinghuilouyu.cn

[T59] Scala：循环
来源：http://baf.nanxinkj.top

for (i <- 1 to 10) println(i)
来源：http://crq.havefunace.top

[T60] Scala：折叠
来源：http://cls.yuanzhike.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ayx.chenlongwang.top

================================================================================
来源：http://lvf.gogol.net.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://pzi.snrcjt.cn

================================================================================
来源：http://aes.feifeiyinyue.top

[U01] Py：创建虚拟环境
来源：http://lop.guannengcc.top

python -m venv .venv && source .venv/bin/activate
来源：http://njf.wangdashe.top

[U02] Py：导出 / 安装依赖
来源：http://sdq.bjfxy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lqb.snrcjt.cn

[U03] Py：加载 .env 配置
来源：http://qkk.yj20258.top

from dotenv import load_dotenv; load_dotenv()
来源：http://eru.smart0.xyz

[U04] Py：变量调试打印
来源：http://qaw.daxiang520.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://sfv.fktsv.cn

[U05] Py：列表去重且保序
来源：http://nkm.jinyuanbaomall.cn

list(dict.fromkeys(arr))
来源：http://yyc.yanxiufei.cn

[U06] Py：合并两个字典
来源：http://lqk.jinqigfzy.top

{**a, **b}
来源：http://zhu.0kj1m.cn

[U07] Py：反转字典键值
来源：http://uip.jianghu66.top

{v: k for k, v in d.items()}
来源：http://jfg.havefunace.top

[U08] Py：展平二维列表
来源：http://iqy.yj20258888.top

[y for x in nested for y in x]
来源：http://uor.mhx1999.top

[U09] Py：字典取最大值的键
来源：http://rmd.snrcjt.cn

max(d, key=d.get)
来源：http://luc.fengsongda.top

[U10] Py：按值排序字典
来源：http://lzz.yongpay.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ejf.haohaochexian.top

[U11] Py：生成器表达式
来源：http://yws.zdqjudy.top

(x * 2 for x in arr)
来源：http://pum.hnqzz.top

[U12] Py：取出现最多的 3 个元素
来源：http://wxt.bbcook.cn

Counter(arr).most_common(3)
来源：http://bdc.cheryme.top

[U13] Py：固定长度队列
来源：http://rer.yj20258888.top

deque(maxlen=10)
来源：http://wpn.gaohongyu789.top

[U14] Py：分组收集到列表
来源：http://htn.bbcook.cn

defaultdict(list)
来源：http://qmm.ybcxt.top

[U15] Py：高精度计时
来源：http://jbh.yj20258.top

t = time.perf_counter()
来源：http://bki.hongshengwenyu.top

[U16] Py：命令行参数解析
来源：http://tba.zhiwuduotai.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gpj.mhx1999.top


<!-- 参考信息 -->