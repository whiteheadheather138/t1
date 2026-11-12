代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://utj.sxryk.cn

[R76] 使用临时文件
来源：http://hhu.cucudq.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fuo.snrcjt.cn

[R77] 读取用户输入
来源：http://hyw.ydjk.org.cn

read -rp "请输入: " ans
来源：http://qvj.tianlin.xyz

[R78] 交互式菜单
来源：http://vrn.ctjpmb.com

select opt in a b c; do echo "$opt"; break; done
来源：http://wez.c1oappe.top

[R79] 解析命令行选项
来源：http://bge.c1oappe.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://abw.pycfn.com

[R80] 查看脚本执行耗时
来源：http://lbe.yj20258888.top

time ./run.sh
来源：http://ohw.fehbvm.com

================================================================================
来源：http://zyb.jianghu66.top

S. C / C++ 专题
来源：http://srs.wangshuangyany.cn

================================================================================
来源：http://jtu.ywan-chungtsiang.top

[S01] C：Hello World
来源：http://nfp.fanxiaobao.xyz

#include <stdio.h>
来源：http://zkd.ivvv.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://qht.uphjek.com

[S02] C：变量与格式化输出
来源：http://kuy.zdqjudy.top

int a = 10; printf("%d\n", a);
来源：http://izp.chenlongwang.top

[S03] C：读入整数
来源：http://tuf.xuanzx.com

int x; scanf("%d", &x);
来源：http://txi.hammf.cn

[S04] C：字符串复制
来源：http://xmn.jlsjyb.cn

char dst[32]; strcpy(dst, "hi");
来源：http://fgw.tanke756.top

[S05] C：字符串长度
来源：http://pwt.shuidangran.top

strlen(s)
来源：http://chk.ctjpmb.com

[S06] C：字符串比较
来源：http://uwq.xinyue.icu

strcmp(a, b) == 0
来源：http://nju.wangdashe.top

[S07] C：数组遍历求和
来源：http://ujo.jqgfzy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://stf.jinqigfzy.top

[S08] C：动态内存分配与释放
来源：http://sgf.c1oappe.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qoi.nanxuanxn.top

[S09] C：结构体定义与初始化
来源：http://fsm.c1oappe.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bfe.316326.xyz

[S10] C：指针与解引用
来源：http://ylp.kuanghao11.cn

int *p = &a;  *p = 5;
来源：http://qjd.0kj1m.cn

[S11] C：逐行读文件
来源：http://ida.zdqjudy.top

FILE *f = fopen("a.txt", "r");
来源：http://rfb.zhongyouzk.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://tmm.sysykeji.top

fclose(f);
来源：http://nnr.sufxvd.cn

[S12] C：写文件
来源：http://yai.hysaishi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://otf.52xcode.cn

[S13] C：宏定义
来源：http://jbv.zhaomingkeji.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://aiv.xuanzx.com

[S14] C：枚举
来源：http://hyu.zhaomingkeji.xyz

enum Color { RED, GREEN, BLUE };
来源：http://raf.snrcjt.cn

[S15] C：类型转换
来源：http://qsu.hnqzz.top

(double) a / b
来源：http://adr.hnxiangtu.top

[S16] C：位操作置位
来源：http://rdp.hfpthk.cn

x |= (1 << 3);
来源：http://uom.jlsjyb.cn

[S17] C：安全拼接字符串
来源：http://mpv.cucudq.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dmo.nanxuanxn.top

[S18] C：命令行参数
来源：http://ybn.zhoulong.xyz

int main(int argc, char **argv)
来源：http://tlu.quarkkingdee.top

[S19] C：快速排序
来源：http://opw.nanxinkj.top

qsort(a, n, sizeof(int), cmp);
来源：http://pkk.52xcode.cn

[S20] C：二分查找
来源：http://otg.ybcxt.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bhi.tianlin.xyz

[S21] C：字符类别判断
来源：http://uip.hammf.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lpx.mhx1999.top

[S22] C：字符串转数字
来源：http://xdk.redwolf501.top

atoi("42");  strtod("3.14", NULL);
来源：http://ocm.iojbl.cn

[S23] C：随机数
来源：http://aos.dashuyun.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wyl.vehdjk.com

[S24] C：获取本地时间
来源：http://ore.pycfn.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cik.mhx1999.top

[S25] C：内存拷贝
来源：http://img.wangdashe.top

memcpy(dst, src, n);
来源：http://hti.cdnleiting.top

[S26] C：内存清零
来源：http://wvb.yuxming.cn

memset(a, 0, sizeof a);
来源：http://wyz.cdnleiting.top

[S27] C：定义常量
来源：http://wnr.ydzc1.top

const double PI = 3.14159;
来源：http://kir.zhaomingkeji.xyz

[S28] C：静态变量
来源：http://yut.zdbjq.cn

static int counter = 0;
来源：http://onk.jinyuanbaomall.cn

[S29] C：变参函数
来源：http://ctv.redwolf501.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://syo.yongpay.top

[S30] C：头文件保护
来源：http://ikq.jinghuilouyu.cn

#ifndef X_H
来源：http://xwn.jqgufenzy.top

#define X_H
来源：http://pal.hnxiangtu.top

#endif
来源：http://zqt.redwolf501.top

[S31] C++：Hello World
来源：http://eyz.epnwcf.com

#include <iostream>
来源：http://viv.shangyingyoupin.top

int main() { std::cout << "Hello\n"; }
来源：http://feu.ydzc1.top

[S32] C++：字符串
来源：http://wdq.fzhhl.top

std::string s = "hi";  s += "!";
来源：http://egt.guowangkeji.top

[S33] C++：vector 增删
来源：http://mgd.chenjidiqi.icu

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qsy.zhongyouzk.top

[S34] C++：遍历 vector
来源：http://myc.jlsjyb.cn

for (auto &x : v) { std::cout << x; }
来源：http://apf.zhijiandao.cn

[S35] C++：map
来源：http://qah.nanxinkj.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qhz.shzxlz.cn

[S36] C++：unordered_map
来源：http://lsu.zhixingplan.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://exd.chenlongwang.top

[S37] C++：set
来源：http://qtm.shzxlz.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wbd.chenzaomai.com

[S38] C++：排序
来源：http://ilp.ctjpmb.com

std::sort(v.begin(), v.end());
来源：http://fql.zhaomingkeji.xyz

[S39] C++：自定义比较器排序
来源：http://vzg.fehbvm.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://oab.birdmap.top

[S40] C++：查找元素
来源：http://vgf.yj202588.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hkq.zhijiandao.cn

[S41] C++：类与构造函数
来源：http://zvw.tarul.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://guc.hfpthk.cn

[S42] C++：继承与虚函数
来源：http://ykb.wangdashe.top

class B : public Base { public: void f() override {} };
来源：http://ztl.gzhubu.top

[S43] C++：智能指针
来源：http://vdh.tanke756.top

auto p = std::make_unique<int>(5);
来源：http://uvs.0kj1m.cn

[S44] C++：引用传参
来源：http://rxq.fktsv.cn

void inc(int &x) { ++x; }
来源：http://zqa.epnwcf.com

[S45] C++：lambda
来源：http://vfy.yfazqb.com

auto add = [](int a, int b) { return a + b; };
来源：http://pne.yongpay.top

[S46] C++：函数模板
来源：http://lgp.yuanzhike.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://irw.jyoumei.cn

[S47] C++：结构化绑定遍历
来源：http://hbw.fanxiaobao.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hqm.chenlongwang.top

[S48] C++：逐行读文件
来源：http://geh.ywan-chungtsiang.top

std::ifstream in("a.txt");  std::string line;
来源：http://rlo.kuanghao11.cn

while (std::getline(in, line)) { }
来源：http://ghi.316326.xyz

[S49] C++：写文件
来源：http://lzi.cdnleiting.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zls.nwbrower.top

[S50] C++：格式化数字
来源：http://ynu.jlsjyb.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hiv.yongpay.top

[S51] C++：显式类型转换
来源：http://ckt.guowangkeji.top

static_cast<double>(a) / b
来源：http://nzk.ctjpmb.com

[S52] C++：const 与 noexcept
来源：http://dgn.pycfn.com

int size() const noexcept { return n_; }
来源：http://nqq.yfazqb.com

[S53] C++：移动语义
来源：http://mru.sjlbkw.cn

std::vector<int> w = std::move(v);
来源：http://xzw.dianchejie.cn

[S54] C++：异常处理
来源：http://xpw.birdmap.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gat.xuanzx.com

[S55] C++：结构化绑定
来源：http://jji.chenlongwang.top

auto [a, b] = std::make_pair(1, 2);
来源：http://qjg.yueranfly.top

[S56] C++：optional
来源：http://jaf.yongpay.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qao.hysaishi.cn

[S57] C++：编译期常量
来源：http://znx.hesvh.cn

constexpr int N = 10;
来源：http://azx.shzxlz.cn

[S58] C++：命名空间
来源：http://eyx.zycfv.cn

namespace ns { int f() { return 1; } }
来源：http://ckm.fehbvm.com

[S59] C++：静态断言
来源：http://vqu.gotoacloud.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vrt.tian-w.cn

[S60] C++：遍历并删除元素
来源：http://sav.xinyue.icu

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lct.svipenyu.cn

================================================================================
来源：http://fqr.hcnkem.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ctw.ppjwa.cn

================================================================================
来源：http://apv.jqgfzy.top

[T01] Kotlin：Hello World
来源：http://apb.xingfuxueyuan.xyz

println("Hello")
来源：http://ntt.zdbjq.cn

[T02] Kotlin：变量
来源：http://rpu.hnxiangtu.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://spu.birdmap.top

[T03] Kotlin：字符串模板
来源：http://mku.tian-w.cn

"值: $b"
来源：http://taq.daxiang520.top

[T04] Kotlin：空安全
来源：http://djm.daxiang520.top

val n: String? = null;  n?.length
来源：http://ztb.yj20258.top

[T05] Kotlin：when 表达式
来源：http://sgh.jqgufenzy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xss.yj20258.top

[T06] Kotlin：集合映射
来源：http://xjm.hnxiangtu.top

listOf(1, 2, 3).map { it * 2 }
来源：http://jgt.feifeiyinyue.top

[T07] Kotlin：集合过滤
来源：http://zqi.zhongyouzk.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://lzq.hfpthk.cn

[T08] Kotlin：数据类
来源：http://lff.chenlongwang.top

data class User(val name: String, val age: Int)
来源：http://eol.zycfv.cn

[T09] Kotlin：扩展函数
来源：http://rgw.zdbjq.cn

fun String.exclaim() = this + "!"
来源：http://jhw.birdmap.top

[T10] Kotlin：默认参数
来源：http://nhq.jianghu66.top

fun greet(name: String = "World") = "Hi $name"
来源：http://lgi.tian-w.cn

[T11] Kotlin：协程
来源：http://qft.gogol.net.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://iys.jianghu66.top

[T12] Kotlin：解构声明
来源：http://msh.dashuyun.cn

val (a, b) = Pair(1, 2)
来源：http://rpi.316326.xyz

[T13] Kotlin：只读 Map
来源：http://ycz.epnwcf.com

val m = mapOf("a" to 1)
来源：http://mxf.jinghuilouyu.cn

[T14] Kotlin：循环
来源：http://yvq.uphjek.com

for (i in 1..10) println(i)
来源：http://izz.xuanzx.com

[T15] Kotlin：接口
来源：http://dmo.daria6918.cn

interface Shape { fun area(): Double }
来源：http://rkh.yangfankeji.com

[T16] Swift：Hello World
来源：http://eqg.xuetiantiany.cn

print("Hello")
来源：http://ekg.quarkkingdee.top

[T17] Swift：变量与常量
来源：http://awu.yuanzhike.top

var a = 1;  let b = 2
来源：http://zml.epnwcf.com

[T18] Swift：字符串插值
来源：http://dig.haohaochexian.top

"值: \(b)"
来源：http://vjc.bjfxy.top

[T19] Swift：可选绑定
来源：http://hmd.ctjpmb.com

if let n = opt { print(n) }
来源：http://eex.zhijiandao.cn

[T20] Swift：数组操作
来源：http://mik.chenjidiqi.icu

var a = [1, 2, 3];  a.append(4)
来源：http://upf.hysaishi.cn

[T21] Swift：遍历
来源：http://vts.yueranfly.top

for x in a { print(x) }
来源：http://rnv.smart0.xyz

[T22] Swift：字典
来源：http://zkq.epnwcf.com

var d = ["a": 1];  d["b"] = 2
来源：http://ddx.nanxinkj.top

[T23] Swift：函数
来源：http://dyp.yfazqb.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wsd.yuanzhike.top

[T24] Swift：闭包
来源：http://ppv.xuanzx.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://vfq.nwbrower.top

[T25] Swift：结构体
来源：http://xet.yanxiufei.cn

struct P { var x: Int }
来源：http://uif.xziqi.cn

[T26] Swift：类与重写
来源：http://otp.hywenlv.cn

class A: Base { override func f() {} }
来源：http://yza.c1oappe.top

[T27] Swift：错误处理
来源：http://yed.chenlongwang.top

do { try f() } catch { print(error) }
来源：http://dom.cqqwz.cn

[T28] Swift：枚举
来源：http://rcg.yj20258888.top

enum Color { case red, green }
来源：http://dlr.hcnkem.com

[T29] Swift：guard 提前返回
来源：http://yvf.yueranfly.top

guard let x = opt else { return }
来源：http://nno.hnqzz.top

[T30] Swift：协议
来源：http://dix.0kj1m.cn

protocol Shape { func area() -> Double }
来源：http://suf.andypj.xyz

[T31] Lua：Hello World
来源：http://itn.bjfxy.top

print("Hello")
来源：http://kis.jinqigfzy.top

[T32] Lua：局部变量
来源：http://gsb.dianchejie.cn

local a = 1
来源：http://pkz.fzhhl.top

[T33] Lua：表（数组）
来源：http://ist.haohaochexian.top

local t = {1, 2, 3};  t[4] = 4
来源：http://kxx.ydjk.org.cn

[T34] Lua：遍历表
来源：http://eyw.shanyushiyangkeji.top

for i, v in ipairs(t) do print(i, v) end
来源：http://jdw.birdmap.top

[T35] Lua：字典表
来源：http://mek.yvedp.cn

local d = { a = 1 };  d.b = 2
来源：http://xyv.cashguo.top

[T36] Lua：函数
来源：http://oyz.mhx1999.top

function add(a, b) return a + b end
来源：http://tyq.mhx1999.top

[T37] Lua：字符串拼接
来源：http://owe.jinghuilouyu.cn

"a" .. "b"
来源：http://ksx.fehbvm.com

[T38] Lua：条件
来源：http://rfv.shzxlz.cn

if x > 0 then print("正") end
来源：http://zks.jyoumei.cn

[T39] Lua：模式匹配
来源：http://fao.haohaochexian.top

string.find(s, "%d+")
来源：http://jjr.tanke756.top

[T40] Lua：元表
来源：http://fgi.ppjwa.cn

setmetatable({}, { __index = base })
来源：http://qyh.snrcjt.cn

[T41] Perl：Hello World
来源：http://iwt.jiagoushi.top

print "Hello\n";
来源：http://zls.bjfxy.top

[T42] Perl：变量类型
来源：http://fzn.hammf.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rvd.andypj.xyz

[T43] Perl：字符串插值
来源：http://hky.yuxming.cn

"值: $a"
来源：http://jvn.nanxinkj.top

[T44] Perl：条件
来源：http://vwc.chenlongwang.top

if ($a > 0) { print "正"; }
来源：http://mba.yongpay.top

[T45] Perl：数组遍历
来源：http://jxp.jqgufenzy.top

for my $x (@arr) { print $x; }
来源：http://cwt.hnqzz.top

[T46] Perl：哈希操作
来源：http://kto.yj20258.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lfn.jyoumei.cn

[T47] Perl：正则捕获
来源：http://ygp.nanxinkj.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://kpg.gogol.net.cn

[T48] Perl：正则替换
来源：http://zid.svipenyu.cn

$s =~ s/old/new/g;
来源：http://mlf.guowangkeji.top

[T49] Perl：函数
来源：http://cnr.fanxiaobao.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xra.vehdjk.com

[T50] Perl：逐行读文件
来源：http://rae.sufxvd.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ahn.pengpengdd.cyou

while (my $line = <$fh>) { print $line; }
来源：http://qjo.ydzc1.top

[T51] Scala：Hello World
来源：http://rpo.feifeiyinyue.top

println("Hello")
来源：http://qug.haohaochexian.top

[T52] Scala：变量
来源：http://qxk.meibo888.top

val a = 1;  var b = 2
来源：http://qbf.sxryk.cn

[T53] Scala：字符串插值
来源：http://una.sufxvd.cn

s"值: $b"
来源：http://xfd.andypj.xyz

[T54] Scala：集合映射
来源：http://hem.mhx1999.top

List(1, 2, 3).map(_ * 2)
来源：http://uyj.ybcxt.top

[T55] Scala：集合过滤
来源：http://rjo.shanyushiyangkeji.top

List(1, 2, 3).filter(_ > 1)
来源：http://uba.shanyushiyangkeji.top

[T56] Scala：样例类
来源：http://txl.yongpay.top

case class User(name: String, age: Int)
来源：http://wte.c1oappe.top

[T57] Scala：模式匹配
来源：http://igg.xuanzx.com

x match { case 1 => "一"; case _ => "其他" }
来源：http://ppw.yj202588.top

[T58] Scala：函数定义
来源：http://yvb.zdqjudy.top

def add(a: Int, b: Int): Int = a + b
来源：http://xqr.cqqwz.cn

[T59] Scala：循环
来源：http://lcg.ctjpmb.com

for (i <- 1 to 10) println(i)
来源：http://kvq.fengsongda.top

[T60] Scala：折叠
来源：http://hfa.bjfxy.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jsj.yfazqb.com

================================================================================
来源：http://ali.xylfe.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tbs.fehbvm.com

================================================================================
来源：http://nzw.feifeiyinyue.top

[U01] Py：创建虚拟环境
来源：http://jns.jyoumei.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nve.feifeiyinyue.top

[U02] Py：导出 / 安装依赖
来源：http://sua.guowangkeji.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rlw.fehbvm.com

[U03] Py：加载 .env 配置
来源：http://aob.jinqigufen.top

from dotenv import load_dotenv; load_dotenv()
来源：http://eee.redwolf501.top

[U04] Py：变量调试打印
来源：http://hhj.aizwys.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://oyg.tarul.cn

[U05] Py：列表去重且保序
来源：http://yfo.jinyuanbaomall.cn

list(dict.fromkeys(arr))
来源：http://qda.yj20258.top

[U06] Py：合并两个字典
来源：http://vuk.mhx1999.top

{**a, **b}
来源：http://vet.yueranfly.top

[U07] Py：反转字典键值
来源：http://fuh.fanxiaobao.xyz

{v: k for k, v in d.items()}
来源：http://prv.vehdjk.com

[U08] Py：展平二维列表
来源：http://bqe.zhixingplan.top

[y for x in nested for y in x]
来源：http://dlw.zhengqikj.top

[U09] Py：字典取最大值的键
来源：http://fgz.dianchejie.cn

max(d, key=d.get)
来源：http://aex.hfpthk.cn

[U10] Py：按值排序字典
来源：http://uty.nanxinkj.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ahi.cqqwz.cn

[U11] Py：生成器表达式
来源：http://bub.zycfv.cn

(x * 2 for x in arr)
来源：http://wle.ctjpmb.com

[U12] Py：取出现最多的 3 个元素
来源：http://lue.quarkkingdee.top

Counter(arr).most_common(3)
来源：http://vnf.zhixingplan.top

[U13] Py：固定长度队列
来源：http://rgw.hesvh.cn

deque(maxlen=10)
来源：http://ada.epnwcf.com

[U14] Py：分组收集到列表
来源：http://zjf.tanke756.top

defaultdict(list)
来源：http://rtx.c1oappe.top

[U15] Py：高精度计时
来源：http://zrc.gaohongyu789.top

t = time.perf_counter()
来源：http://dkg.ydzc1.top

[U16] Py：命令行参数解析
来源：http://yyb.bjfxy.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xqe.pycfn.com


<!-- 参考信息 -->