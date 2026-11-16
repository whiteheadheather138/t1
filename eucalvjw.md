代发 wailian999

split -l 1000 big.log part_
来源：http://mhv.hywenlv.cn

[R74] 批量重命名
来源：http://oue.tanke756.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tqt.haohaochexian.top

[R75] 导出环境变量
来源：http://joq.0kj1m.cn

export PATH="$HOME/bin:$PATH"
来源：http://bgh.cucudq.cn

[R76] 使用临时文件
来源：http://ujm.yj20258.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pdh.yonumen.top

[R77] 读取用户输入
来源：http://cfq.zhoulong.xyz

read -rp "请输入: " ans
来源：http://pib.zhaomingkeji.xyz

[R78] 交互式菜单
来源：http://rqx.wangdashe.top

select opt in a b c; do echo "$opt"; break; done
来源：http://tkr.jqgfzy.top

[R79] 解析命令行选项
来源：http://seq.pengpengdd.cyou

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nic.yj20258.top

[R80] 查看脚本执行耗时
来源：http://zey.daxiang520.top

time ./run.sh
来源：http://wjr.cdnleiting.top

================================================================================
来源：http://gad.cqqwz.cn

S. C / C++ 专题
来源：http://ogr.yj20258888.top

================================================================================
来源：http://okz.gzhubu.top

[S01] C：Hello World
来源：http://tjy.hnxiangtu.top

#include <stdio.h>
来源：http://vrr.dianchejie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://nha.quarkkingdee.top

[S02] C：变量与格式化输出
来源：http://swk.sysykeji.top

int a = 10; printf("%d\n", a);
来源：http://zhi.hesvh.cn

[S03] C：读入整数
来源：http://aoj.haohaochexian.top

int x; scanf("%d", &x);
来源：http://and.0kj1m.cn

[S04] C：字符串复制
来源：http://siw.xinyue.icu

char dst[32]; strcpy(dst, "hi");
来源：http://ffj.jinyuanbaomall.cn

[S05] C：字符串长度
来源：http://zpk.yonumen.top

strlen(s)
来源：http://itg.bjfxy.top

[S06] C：字符串比较
来源：http://fhq.iojbl.cn

strcmp(a, b) == 0
来源：http://yzw.yuxming.cn

[S07] C：数组遍历求和
来源：http://quo.snrcjt.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hnz.0kj1m.cn

[S08] C：动态内存分配与释放
来源：http://mbt.smart0.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ear.birdmap.top

[S09] C：结构体定义与初始化
来源：http://ofv.cucudq.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xzr.meibo888.top

[S10] C：指针与解引用
来源：http://ryo.zhixingplan.top

int *p = &a;  *p = 5;
来源：http://uan.zhoulong.xyz

[S11] C：逐行读文件
来源：http://red.shzxlz.cn

FILE *f = fopen("a.txt", "r");
来源：http://rvu.chenjidiqi.icu

while (fgets(buf, sizeof buf, f)) { }
来源：http://rfi.cdnleiting.top

fclose(f);
来源：http://pmn.feifeiyinyue.top

[S12] C：写文件
来源：http://ynt.hongshengwenyu.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fpm.nwbrower.top

[S13] C：宏定义
来源：http://mps.hysaishi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xbp.sweek.top

[S14] C：枚举
来源：http://jfs.sxryk.cn

enum Color { RED, GREEN, BLUE };
来源：http://qxp.meibo888.top

[S15] C：类型转换
来源：http://czw.tanke756.top

(double) a / b
来源：http://rqb.hnqzz.top

[S16] C：位操作置位
来源：http://onk.hywenlv.cn

x |= (1 << 3);
来源：http://uzp.shzxlz.cn

[S17] C：安全拼接字符串
来源：http://cok.zhixingplan.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ytr.yangfankeji.com

[S18] C：命令行参数
来源：http://ptd.jlsjyb.cn

int main(int argc, char **argv)
来源：http://nxx.hfpthk.cn

[S19] C：快速排序
来源：http://cdn.mhx1999.top

qsort(a, n, sizeof(int), cmp);
来源：http://xnl.quarkkingdee.top

[S20] C：二分查找
来源：http://cth.kuanghao11.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://toj.pengpengdd.cyou

[S21] C：字符类别判断
来源：http://xkn.quarkkingdee.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cuw.wangshuangyany.cn

[S22] C：字符串转数字
来源：http://ajo.fehbvm.com

atoi("42");  strtod("3.14", NULL);
来源：http://fyu.cdnleiting.top

[S23] C：随机数
来源：http://tvb.pengpengdd.cyou

srand(time(NULL));  int r = rand() % 100;
来源：http://zps.hammf.cn

[S24] C：获取本地时间
来源：http://vmj.hesvh.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nbq.9152youxi.cn

[S25] C：内存拷贝
来源：http://ufd.hywenlv.cn

memcpy(dst, src, n);
来源：http://qzk.jlsjyb.cn

[S26] C：内存清零
来源：http://rgu.snrcjt.cn

memset(a, 0, sizeof a);
来源：http://aoy.jinyuanbaomall.cn

[S27] C：定义常量
来源：http://dxo.zhongyouzk.top

const double PI = 3.14159;
来源：http://aus.epnwcf.com

[S28] C：静态变量
来源：http://spc.hnqzz.top

static int counter = 0;
来源：http://vac.sjlbkw.cn

[S29] C：变参函数
来源：http://quh.epnwcf.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uwd.jianghu66.top

[S30] C：头文件保护
来源：http://bla.shzxlz.cn

#ifndef X_H
来源：http://ynl.jinqigufen.top

#define X_H
来源：http://rix.ydzc1.top

#endif
来源：http://mhf.yueranfly.top

[S31] C++：Hello World
来源：http://pyh.kuanghao11.cn

#include <iostream>
来源：http://umd.nanxuanxn.top

int main() { std::cout << "Hello\n"; }
来源：http://lvd.cdnleiting.top

[S32] C++：字符串
来源：http://jde.shangyingyoupin.top

std::string s = "hi";  s += "!";
来源：http://iha.sjlbkw.cn

[S33] C++：vector 增删
来源：http://cph.ywan-chungtsiang.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://com.yj20258888.top

[S34] C++：遍历 vector
来源：http://pup.daxiang520.top

for (auto &x : v) { std::cout << x; }
来源：http://dkc.fengsongda.top

[S35] C++：map
来源：http://irg.gzhubu.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jeh.nanxuanxn.top

[S36] C++：unordered_map
来源：http://kto.jqgfzy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gcr.xuanzx.com

[S37] C++：set
来源：http://qxy.zdbjq.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hfb.tarul.cn

[S38] C++：排序
来源：http://iwb.zhijiandao.cn

std::sort(v.begin(), v.end());
来源：http://ffg.gogol.net.cn

[S39] C++：自定义比较器排序
来源：http://ejh.andypj.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hwu.redwolf501.top

[S40] C++：查找元素
来源：http://mbw.52xcode.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://osg.fanxiaobao.xyz

[S41] C++：类与构造函数
来源：http://slh.yueranfly.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://txf.fktsv.cn

[S42] C++：继承与虚函数
来源：http://igk.cucudq.cn

class B : public Base { public: void f() override {} };
来源：http://rnp.hcnkem.com

[S43] C++：智能指针
来源：http://dgl.9152youxi.cn

auto p = std::make_unique<int>(5);
来源：http://xbd.dianchejie.cn

[S44] C++：引用传参
来源：http://seu.xuetiantiany.cn

void inc(int &x) { ++x; }
来源：http://her.tarul.cn

[S45] C++：lambda
来源：http://ptr.jiagoushi.top

auto add = [](int a, int b) { return a + b; };
来源：http://xqn.guannengcc.top

[S46] C++：函数模板
来源：http://vkc.zycfv.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lcw.zhoulong.xyz

[S47] C++：结构化绑定遍历
来源：http://nsj.shangyingyoupin.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dur.ydzc1.top

[S48] C++：逐行读文件
来源：http://lhw.chenzaomai.com

std::ifstream in("a.txt");  std::string line;
来源：http://ewr.dianchejie.cn

while (std::getline(in, line)) { }
来源：http://ybi.uphjek.com

[S49] C++：写文件
来源：http://ona.nanxuanxn.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://knc.xinyue.icu

[S50] C++：格式化数字
来源：http://nvd.zdbjq.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cwk.ehwqpu.com

[S51] C++：显式类型转换
来源：http://pdc.jinghuilouyu.cn

static_cast<double>(a) / b
来源：http://wkw.sufxvd.cn

[S52] C++：const 与 noexcept
来源：http://beu.yvedp.cn

int size() const noexcept { return n_; }
来源：http://nrk.yuanzhike.top

[S53] C++：移动语义
来源：http://pqg.tarul.cn

std::vector<int> w = std::move(v);
来源：http://ckq.meibo888.top

[S54] C++：异常处理
来源：http://vgg.dianchejie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://khr.52xcode.cn

[S55] C++：结构化绑定
来源：http://qlq.guannengcc.top

auto [a, b] = std::make_pair(1, 2);
来源：http://fzs.52xcode.cn

[S56] C++：optional
来源：http://qmg.shanyushiyangtech.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gpa.52xcode.cn

[S57] C++：编译期常量
来源：http://mug.aibaodan.cn

constexpr int N = 10;
来源：http://scm.kuanghao11.cn

[S58] C++：命名空间
来源：http://mht.9152youxi.cn

namespace ns { int f() { return 1; } }
来源：http://ept.dianchejie.cn

[S59] C++：静态断言
来源：http://ozt.birdmap.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fqk.wangshuangyany.cn

[S60] C++：遍历并删除元素
来源：http://ocp.gogol.net.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zas.yueranfly.top

================================================================================
来源：http://pxi.zhongyouzk.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://grm.zhoulong.xyz

================================================================================
来源：http://nvt.yonumen.top

[T01] Kotlin：Hello World
来源：http://ixm.0kj1m.cn

println("Hello")
来源：http://knl.xziqi.cn

[T02] Kotlin：变量
来源：http://vnv.gotoacloud.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qsh.sufxvd.cn

[T03] Kotlin：字符串模板
来源：http://ecj.ydzc1.top

"值: $b"
来源：http://pbg.yangfankeji.com

[T04] Kotlin：空安全
来源：http://hmj.gotoacloud.top

val n: String? = null;  n?.length
来源：http://qei.jyoumei.cn

[T05] Kotlin：when 表达式
来源：http://byn.quarkkingdee.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xxm.xinyue.icu

[T06] Kotlin：集合映射
来源：http://utp.fzhhl.top

listOf(1, 2, 3).map { it * 2 }
来源：http://thl.yonumen.top

[T07] Kotlin：集合过滤
来源：http://qpd.shzxlz.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ppe.yfazqb.com

[T08] Kotlin：数据类
来源：http://lhs.52xcode.cn

data class User(val name: String, val age: Int)
来源：http://jyq.jlsjyb.cn

[T09] Kotlin：扩展函数
来源：http://cad.sufxvd.cn

fun String.exclaim() = this + "!"
来源：http://gbf.zdqjudy.top

[T10] Kotlin：默认参数
来源：http://vqp.hongshengwenyu.top

fun greet(name: String = "World") = "Hi $name"
来源：http://nrc.chenzaomai.com

[T11] Kotlin：协程
来源：http://hmd.hcnkem.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://ncp.yj20258.top

[T12] Kotlin：解构声明
来源：http://clm.hammf.cn

val (a, b) = Pair(1, 2)
来源：http://huo.yj20258888.top

[T13] Kotlin：只读 Map
来源：http://eky.redwolf501.top

val m = mapOf("a" to 1)
来源：http://gyf.xuetiantiany.cn

[T14] Kotlin：循环
来源：http://fqb.ctjpmb.com

for (i in 1..10) println(i)
来源：http://jxe.chenzaomai.com

[T15] Kotlin：接口
来源：http://bdo.shanyushiyangkeji.top

interface Shape { fun area(): Double }
来源：http://zoi.xuanzx.com

[T16] Swift：Hello World
来源：http://tsd.gaohongyu789.top

print("Hello")
来源：http://jxi.zhengqikj.top

[T17] Swift：变量与常量
来源：http://dmc.andypj.xyz

var a = 1;  let b = 2
来源：http://syu.tianlin.xyz

[T18] Swift：字符串插值
来源：http://lzz.vqdsnc.cn

"值: \(b)"
来源：http://lrm.pengpengdd.cyou

[T19] Swift：可选绑定
来源：http://vzu.jinghuilouyu.cn

if let n = opt { print(n) }
来源：http://bvx.ehwqpu.com

[T20] Swift：数组操作
来源：http://muj.pycfn.com

var a = [1, 2, 3];  a.append(4)
来源：http://bqy.fktsv.cn

[T21] Swift：遍历
来源：http://gis.fanxiaobao.xyz

for x in a { print(x) }
来源：http://wgt.pengpengdd.cyou

[T22] Swift：字典
来源：http://tcm.hywenlv.cn

var d = ["a": 1];  d["b"] = 2
来源：http://axp.9152youxi.cn

[T23] Swift：函数
来源：http://vfs.sufxvd.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://smx.zhijiandao.cn

[T24] Swift：闭包
来源：http://gri.meibo888.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://oao.yfazqb.com

[T25] Swift：结构体
来源：http://ogx.fehbvm.com

struct P { var x: Int }
来源：http://gfe.mhx1999.top

[T26] Swift：类与重写
来源：http://yml.hysaishi.cn

class A: Base { override func f() {} }
来源：http://utj.sweek.top

[T27] Swift：错误处理
来源：http://zvk.zhijiandao.cn

do { try f() } catch { print(error) }
来源：http://snv.yj20258888.top

[T28] Swift：枚举
来源：http://zzr.vehdjk.com

enum Color { case red, green }
来源：http://pvx.fktsv.cn

[T29] Swift：guard 提前返回
来源：http://cwn.daxiang520.top

guard let x = opt else { return }
来源：http://ycp.yuxming.cn

[T30] Swift：协议
来源：http://hwy.yvedp.cn

protocol Shape { func area() -> Double }
来源：http://lut.jyoumei.cn

[T31] Lua：Hello World
来源：http://mge.zdqjudy.top

print("Hello")
来源：http://poi.ppjwa.cn

[T32] Lua：局部变量
来源：http://ntj.guowangkeji.top

local a = 1
来源：http://lql.ehwqpu.com

[T33] Lua：表（数组）
来源：http://ywq.aizwys.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xsa.aibaodan.cn

[T34] Lua：遍历表
来源：http://fwo.ybcxt.top

for i, v in ipairs(t) do print(i, v) end
来源：http://nhd.shzxlz.cn

[T35] Lua：字典表
来源：http://ceo.yuanzhike.top

local d = { a = 1 };  d.b = 2
来源：http://veu.yanxiufei.cn

[T36] Lua：函数
来源：http://dhl.wangdashe.top

function add(a, b) return a + b end
来源：http://aup.havefunace.top

[T37] Lua：字符串拼接
来源：http://hxh.sysykeji.top

"a" .. "b"
来源：http://ghg.tanke756.top

[T38] Lua：条件
来源：http://ctz.jqgfzy.top

if x > 0 then print("正") end
来源：http://iwl.chenzaomai.com

[T39] Lua：模式匹配
来源：http://fzq.jqgfzy.top

string.find(s, "%d+")
来源：http://jgd.vqdsnc.cn

[T40] Lua：元表
来源：http://dsh.xziqi.cn

setmetatable({}, { __index = base })
来源：http://ypa.ivvv.top

[T41] Perl：Hello World
来源：http://ctz.sjlbkw.cn

print "Hello\n";
来源：http://bvy.hammf.cn

[T42] Perl：变量类型
来源：http://nou.sxryk.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://apm.ydjk.org.cn

[T43] Perl：字符串插值
来源：http://zsn.yj20258.top

"值: $a"
来源：http://kvn.tanke756.top

[T44] Perl：条件
来源：http://wfz.jinyuanbaomall.cn

if ($a > 0) { print "正"; }
来源：http://ljp.9152youxi.cn

[T45] Perl：数组遍历
来源：http://mkg.zhixingplan.top

for my $x (@arr) { print $x; }
来源：http://aji.haohaochexian.top

[T46] Perl：哈希操作
来源：http://chr.yj20258888.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fqh.zdbjq.cn

[T47] Perl：正则捕获
来源：http://gnt.xziqi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://jwa.xylfe.cn

[T48] Perl：正则替换
来源：http://bkb.zhiwuduotai.top

$s =~ s/old/new/g;
来源：http://afg.tanke756.top

[T49] Perl：函数
来源：http://vbe.vehdjk.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gex.daria6918.cn

[T50] Perl：逐行读文件
来源：http://soi.jinqigufen.top

open my $fh, "<", "a.txt" or die $!;
来源：http://koy.nwbrower.top

while (my $line = <$fh>) { print $line; }
来源：http://klm.gaohongyu789.top

[T51] Scala：Hello World
来源：http://emx.svipenyu.cn

println("Hello")
来源：http://tvr.tarul.cn

[T52] Scala：变量
来源：http://fka.zhijiandao.cn

val a = 1;  var b = 2
来源：http://igb.yfazqb.com

[T53] Scala：字符串插值
来源：http://udv.chenjidiqi.icu

s"值: $b"
来源：http://avt.zhijiandao.cn

[T54] Scala：集合映射
来源：http://pay.hfpthk.cn

List(1, 2, 3).map(_ * 2)
来源：http://zax.jqgfzy.top

[T55] Scala：集合过滤
来源：http://nrd.kuanghao11.cn

List(1, 2, 3).filter(_ > 1)
来源：http://prc.xingfuxueyuan.xyz

[T56] Scala：样例类
来源：http://jug.sweek.top

case class User(name: String, age: Int)
来源：http://zjw.mhx1999.top

[T57] Scala：模式匹配
来源：http://prd.cqqwz.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vvf.zhaomingkeji.xyz

[T58] Scala：函数定义
来源：http://cnr.jqgfzy.top

def add(a: Int, b: Int): Int = a + b
来源：http://oph.cqqwz.cn

[T59] Scala：循环
来源：http://szv.jqgfzy.top

for (i <- 1 to 10) println(i)
来源：http://icp.yueranfly.top

[T60] Scala：折叠
来源：http://kzv.cucudq.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lau.chenlongwang.top

================================================================================
来源：http://nhy.yuxming.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://glh.hcnkem.com

================================================================================
来源：http://ves.bjfxy.top

[U01] Py：创建虚拟环境
来源：http://cxz.yuanzhike.top

python -m venv .venv && source .venv/bin/activate
来源：http://vpy.hfpthk.cn

[U02] Py：导出 / 安装依赖
来源：http://ibv.pengpengdd.cyou

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jhs.chenzaomai.com

[U03] Py：加载 .env 配置
来源：http://ikn.sxryk.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://boj.gzhubu.top

[U04] Py：变量调试打印
来源：http://szx.tian-w.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://trn.shangyingyoupin.top

[U05] Py：列表去重且保序
来源：http://jxh.shzxlz.cn

list(dict.fromkeys(arr))
来源：http://hzh.sjlbkw.cn

[U06] Py：合并两个字典
来源：http://yjp.daxiang520.top

{**a, **b}
来源：http://aei.xylfe.cn

[U07] Py：反转字典键值
来源：http://edu.gaohongyu789.top

{v: k for k, v in d.items()}
来源：http://lhe.haohaochexian.top

[U08] Py：展平二维列表
来源：http://yuc.c1oappe.top

[y for x in nested for y in x]
来源：http://xwd.shanyushiyangkeji.top

[U09] Py：字典取最大值的键
来源：http://pvy.hongshengwenyu.top

max(d, key=d.get)
来源：http://kie.ywan-chungtsiang.top

[U10] Py：按值排序字典
来源：http://ylx.yfazqb.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ugp.dianchejie.cn

[U11] Py：生成器表达式
来源：http://xyc.zycfv.cn

(x * 2 for x in arr)
来源：http://nqw.yfazqb.com

[U12] Py：取出现最多的 3 个元素
来源：http://gdd.smart0.xyz

Counter(arr).most_common(3)
来源：http://aja.hongshengwenyu.top

[U13] Py：固定长度队列
来源：http://lgp.bjfxy.top

deque(maxlen=10)
来源：http://ect.gotoacloud.top

[U14] Py：分组收集到列表
来源：http://qrv.yongpay.top

defaultdict(list)
来源：http://uot.kuanghao11.cn


<!-- 参考信息 -->