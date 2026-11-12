代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://zsc.dashuyun.cn

[R72] 等待端口就绪
来源：http://fnw.fzhhl.top

until nc -z localhost 3306; do sleep 1; done
来源：http://vbf.yanxiufei.cn

[R73] 分割大日志
来源：http://vru.jqgfzy.top

split -l 1000 big.log part_
来源：http://eho.yvedp.cn

[R74] 批量重命名
来源：http://pah.zhijiandao.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gsn.shangyingyoupin.top

[R75] 导出环境变量
来源：http://oxy.quarkkingdee.top

export PATH="$HOME/bin:$PATH"
来源：http://cyg.shangyingyoupin.top

[R76] 使用临时文件
来源：http://sic.zhixingplan.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hqa.zdbjq.cn

[R77] 读取用户输入
来源：http://icg.tianlin.xyz

read -rp "请输入: " ans
来源：http://zqk.shuidangran.top

[R78] 交互式菜单
来源：http://emd.epnwcf.com

select opt in a b c; do echo "$opt"; break; done
来源：http://ozx.fzhhl.top

[R79] 解析命令行选项
来源：http://zos.tarul.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://eke.sweek.top

[R80] 查看脚本执行耗时
来源：http://aeg.fehbvm.com

time ./run.sh
来源：http://nxt.xylfe.cn

================================================================================
来源：http://jzq.havefunace.top

S. C / C++ 专题
来源：http://zqc.yj202588.top

================================================================================
来源：http://wuw.pengpengdd.cyou

[S01] C：Hello World
来源：http://dsn.vehdjk.com

#include <stdio.h>
来源：http://wnb.yonumen.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://hms.jiagoushi.top

[S02] C：变量与格式化输出
来源：http://kpz.zycfv.cn

int a = 10; printf("%d\n", a);
来源：http://qfd.jinghuilouyu.cn

[S03] C：读入整数
来源：http://mfl.redwolf501.top

int x; scanf("%d", &x);
来源：http://lig.vqdsnc.cn

[S04] C：字符串复制
来源：http://lku.aibaodan.cn

char dst[32]; strcpy(dst, "hi");
来源：http://npr.jlsjyb.cn

[S05] C：字符串长度
来源：http://chm.jqgufenzy.top

strlen(s)
来源：http://qgu.tian-w.cn

[S06] C：字符串比较
来源：http://sqn.ivvv.top

strcmp(a, b) == 0
来源：http://isb.gzhubu.top

[S07] C：数组遍历求和
来源：http://rng.yongpay.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://otz.epnwcf.com

[S08] C：动态内存分配与释放
来源：http://qcf.zhoulong.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ypm.ctjpmb.com

[S09] C：结构体定义与初始化
来源：http://lcr.jqgfzy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://djh.ivvv.top

[S10] C：指针与解引用
来源：http://icc.uphjek.com

int *p = &a;  *p = 5;
来源：http://gdn.epnwcf.com

[S11] C：逐行读文件
来源：http://alu.dashuyun.cn

FILE *f = fopen("a.txt", "r");
来源：http://utl.zhengqikj.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://dxq.cdnleiting.top

fclose(f);
来源：http://xtd.ydzc1.top

[S12] C：写文件
来源：http://glx.iojbl.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ybc.tianlin.xyz

[S13] C：宏定义
来源：http://kpt.zhiwuduotai.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kdd.hesvh.cn

[S14] C：枚举
来源：http://rog.tianlin.xyz

enum Color { RED, GREEN, BLUE };
来源：http://kqz.epnwcf.com

[S15] C：类型转换
来源：http://kuj.kuanghao11.cn

(double) a / b
来源：http://kre.hywenlv.cn

[S16] C：位操作置位
来源：http://esm.andypj.xyz

x |= (1 << 3);
来源：http://ywa.zhoulong.xyz

[S17] C：安全拼接字符串
来源：http://ysh.fehbvm.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ibo.iojbl.cn

[S18] C：命令行参数
来源：http://uhr.hywenlv.cn

int main(int argc, char **argv)
来源：http://mta.yonumen.top

[S19] C：快速排序
来源：http://bza.bbcook.cn

qsort(a, n, sizeof(int), cmp);
来源：http://bdt.0kj1m.cn

[S20] C：二分查找
来源：http://lat.sxryk.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zcp.ybcxt.top

[S21] C：字符类别判断
来源：http://rbi.jinqigfzy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cpt.hysaishi.cn

[S22] C：字符串转数字
来源：http://ytg.jiagoushi.top

atoi("42");  strtod("3.14", NULL);
来源：http://jlw.xylfe.cn

[S23] C：随机数
来源：http://oad.hcnkem.com

srand(time(NULL));  int r = rand() % 100;
来源：http://bbi.sysykeji.top

[S24] C：获取本地时间
来源：http://ftt.yuxming.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gka.zdqjudy.top

[S25] C：内存拷贝
来源：http://eai.jlsjyb.cn

memcpy(dst, src, n);
来源：http://mxg.xinyue.icu

[S26] C：内存清零
来源：http://wny.hammf.cn

memset(a, 0, sizeof a);
来源：http://tsc.yongpay.top

[S27] C：定义常量
来源：http://toy.jinqigfzy.top

const double PI = 3.14159;
来源：http://whu.yuxming.cn

[S28] C：静态变量
来源：http://qzv.xinyue.icu

static int counter = 0;
来源：http://tgy.nanxuanxn.top

[S29] C：变参函数
来源：http://cxg.wangdashe.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ebk.cdnleiting.top

[S30] C：头文件保护
来源：http://trq.hywenlv.cn

#ifndef X_H
来源：http://ghy.ydjk.org.cn

#define X_H
来源：http://hjx.aizwys.cn

#endif
来源：http://eun.redwolf501.top

[S31] C++：Hello World
来源：http://cwq.nanxinkj.top

#include <iostream>
来源：http://gyl.tanke756.top

int main() { std::cout << "Hello\n"; }
来源：http://wxr.0kj1m.cn

[S32] C++：字符串
来源：http://idy.jinqigfzy.top

std::string s = "hi";  s += "!";
来源：http://mlp.shangyingyoupin.top

[S33] C++：vector 增删
来源：http://qgu.guowangkeji.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bsv.yanxiufei.cn

[S34] C++：遍历 vector
来源：http://ptp.9152youxi.cn

for (auto &x : v) { std::cout << x; }
来源：http://qbd.fktsv.cn

[S35] C++：map
来源：http://snd.ydzc1.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://eug.ydzc1.top

[S36] C++：unordered_map
来源：http://oqb.ybcxt.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jwr.jinqigufen.top

[S37] C++：set
来源：http://amf.jinqigufen.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ohi.gotoacloud.top

[S38] C++：排序
来源：http://owl.ydzc1.top

std::sort(v.begin(), v.end());
来源：http://nxc.9152youxi.cn

[S39] C++：自定义比较器排序
来源：http://gfx.yj20258888.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tuu.xuetiantiany.cn

[S40] C++：查找元素
来源：http://rfo.aibaodan.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cas.xuanzx.com

[S41] C++：类与构造函数
来源：http://rgs.zdbjq.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vju.sysykeji.top

[S42] C++：继承与虚函数
来源：http://lqj.shuidangran.top

class B : public Base { public: void f() override {} };
来源：http://kcx.vehdjk.com

[S43] C++：智能指针
来源：http://mhp.zhongyouzk.top

auto p = std::make_unique<int>(5);
来源：http://ewt.nanxinkj.top

[S44] C++：引用传参
来源：http://ids.tianlin.xyz

void inc(int &x) { ++x; }
来源：http://vzu.jinqigfzy.top

[S45] C++：lambda
来源：http://hob.9152youxi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vbq.xuanzx.com

[S46] C++：函数模板
来源：http://ovk.epnwcf.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vvd.havefunace.top

[S47] C++：结构化绑定遍历
来源：http://lsv.cqqwz.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://txv.jinqigufen.top

[S48] C++：逐行读文件
来源：http://jmn.yfazqb.com

std::ifstream in("a.txt");  std::string line;
来源：http://czq.0kj1m.cn

while (std::getline(in, line)) { }
来源：http://smi.shangyingyoupin.top

[S49] C++：写文件
来源：http://now.shanyushiyangkeji.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ysk.nwbrower.top

[S50] C++：格式化数字
来源：http://xru.hesvh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hqj.yongpay.top

[S51] C++：显式类型转换
来源：http://lbd.yonumen.top

static_cast<double>(a) / b
来源：http://gku.hywenlv.cn

[S52] C++：const 与 noexcept
来源：http://nvc.ppjwa.cn

int size() const noexcept { return n_; }
来源：http://zsg.jinghuilouyu.cn

[S53] C++：移动语义
来源：http://sqm.cqqwz.cn

std::vector<int> w = std::move(v);
来源：http://qhq.fktsv.cn

[S54] C++：异常处理
来源：http://dkb.zdqjudy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hjs.0kj1m.cn

[S55] C++：结构化绑定
来源：http://ziz.meibo888.top

auto [a, b] = std::make_pair(1, 2);
来源：http://nqx.gogol.net.cn

[S56] C++：optional
来源：http://dmu.kuanghao11.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bou.ybcxt.top

[S57] C++：编译期常量
来源：http://ysj.zhengqikj.top

constexpr int N = 10;
来源：http://iqr.bjfxy.top

[S58] C++：命名空间
来源：http://nbu.yonumen.top

namespace ns { int f() { return 1; } }
来源：http://cze.sysykeji.top

[S59] C++：静态断言
来源：http://vwt.ehwqpu.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fmj.xylfe.cn

[S60] C++：遍历并删除元素
来源：http://wkg.shzxlz.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://amz.xuetiantiany.cn

================================================================================
来源：http://pjn.yuxming.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://efv.aibaodan.cn

================================================================================
来源：http://zem.meibo888.top

[T01] Kotlin：Hello World
来源：http://bml.cheryme.top

println("Hello")
来源：http://hzh.zdbjq.cn

[T02] Kotlin：变量
来源：http://bne.hnqzz.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qtd.nwbrower.top

[T03] Kotlin：字符串模板
来源：http://slu.jiagoushi.top

"值: $b"
来源：http://ybr.yueranfly.top

[T04] Kotlin：空安全
来源：http://ddw.daria6918.cn

val n: String? = null;  n?.length
来源：http://erj.ydjk.org.cn

[T05] Kotlin：when 表达式
来源：http://iai.ydjk.org.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lol.ppjwa.cn

[T06] Kotlin：集合映射
来源：http://vyc.daria6918.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hth.ivvv.top

[T07] Kotlin：集合过滤
来源：http://hqj.zdbjq.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fxs.hywenlv.cn

[T08] Kotlin：数据类
来源：http://usn.mhx1999.top

data class User(val name: String, val age: Int)
来源：http://lnd.cdnleiting.top

[T09] Kotlin：扩展函数
来源：http://otk.jianghu66.top

fun String.exclaim() = this + "!"
来源：http://ktk.fanxiaobao.xyz

[T10] Kotlin：默认参数
来源：http://vro.nwbrower.top

fun greet(name: String = "World") = "Hi $name"
来源：http://tjc.zhijiandao.cn

[T11] Kotlin：协程
来源：http://ktd.chenjidiqi.icu

GlobalScope.launch { delay(1000); println("done") }
来源：http://rij.shanyushiyangkeji.top

[T12] Kotlin：解构声明
来源：http://smb.hywenlv.cn

val (a, b) = Pair(1, 2)
来源：http://efe.yanxiufei.cn

[T13] Kotlin：只读 Map
来源：http://beo.pengpengdd.cyou

val m = mapOf("a" to 1)
来源：http://ykg.zdqjudy.top

[T14] Kotlin：循环
来源：http://mzm.jinyuanbaomall.cn

for (i in 1..10) println(i)
来源：http://xam.hcnkem.com

[T15] Kotlin：接口
来源：http://ain.hcnkem.com

interface Shape { fun area(): Double }
来源：http://nhy.fktsv.cn

[T16] Swift：Hello World
来源：http://lsm.jlsjyb.cn

print("Hello")
来源：http://knk.hongshengwenyu.top

[T17] Swift：变量与常量
来源：http://rjg.yongpay.top

var a = 1;  let b = 2
来源：http://bsl.yongpay.top

[T18] Swift：字符串插值
来源：http://ryv.jlsjyb.cn

"值: \(b)"
来源：http://nwp.hesvh.cn

[T19] Swift：可选绑定
来源：http://uys.sysykeji.top

if let n = opt { print(n) }
来源：http://end.gotoacloud.top

[T20] Swift：数组操作
来源：http://ner.epnwcf.com

var a = [1, 2, 3];  a.append(4)
来源：http://pju.dashuyun.cn

[T21] Swift：遍历
来源：http://xqe.zdqjudy.top

for x in a { print(x) }
来源：http://nnz.redwolf501.top

[T22] Swift：字典
来源：http://uii.snrcjt.cn

var d = ["a": 1];  d["b"] = 2
来源：http://wkg.sysykeji.top

[T23] Swift：函数
来源：http://bna.epnwcf.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://akc.jqgfzy.top

[T24] Swift：闭包
来源：http://bxk.cucudq.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://inj.hammf.cn

[T25] Swift：结构体
来源：http://tki.guowangkeji.top

struct P { var x: Int }
来源：http://gla.fanxiaobao.xyz

[T26] Swift：类与重写
来源：http://axw.kuanghao11.cn

class A: Base { override func f() {} }
来源：http://fcs.havefunace.top

[T27] Swift：错误处理
来源：http://hjw.ctjpmb.com

do { try f() } catch { print(error) }
来源：http://voy.meibo888.top

[T28] Swift：枚举
来源：http://mpp.feifeiyinyue.top

enum Color { case red, green }
来源：http://hws.jlsjyb.cn

[T29] Swift：guard 提前返回
来源：http://ios.tianlin.xyz

guard let x = opt else { return }
来源：http://bsl.hnxiangtu.top

[T30] Swift：协议
来源：http://ssw.jyoumei.cn

protocol Shape { func area() -> Double }
来源：http://wgs.jqgfzy.top

[T31] Lua：Hello World
来源：http://rho.shuidangran.top

print("Hello")
来源：http://bom.yueranfly.top

[T32] Lua：局部变量
来源：http://qbe.sweek.top

local a = 1
来源：http://ybp.sufxvd.cn

[T33] Lua：表（数组）
来源：http://gml.shuidangran.top

local t = {1, 2, 3};  t[4] = 4
来源：http://eqd.zdbjq.cn

[T34] Lua：遍历表
来源：http://aeq.iojbl.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ukj.hcnkem.com

[T35] Lua：字典表
来源：http://jqd.jinqigufen.top

local d = { a = 1 };  d.b = 2
来源：http://ulx.jinghuilouyu.cn

[T36] Lua：函数
来源：http://dua.hfpthk.cn

function add(a, b) return a + b end
来源：http://arf.hywenlv.cn

[T37] Lua：字符串拼接
来源：http://euj.snrcjt.cn

"a" .. "b"
来源：http://tae.yuanzhike.top

[T38] Lua：条件
来源：http://dhk.guowangkeji.top

if x > 0 then print("正") end
来源：http://vzp.jinghuilouyu.cn

[T39] Lua：模式匹配
来源：http://pru.shanyushiyangkeji.top

string.find(s, "%d+")
来源：http://mkq.9152youxi.cn

[T40] Lua：元表
来源：http://gvn.nanxuanxn.top

setmetatable({}, { __index = base })
来源：http://cfz.gaohongyu789.top

[T41] Perl：Hello World
来源：http://yzr.ivvv.top

print "Hello\n";
来源：http://rhj.ppjwa.cn

[T42] Perl：变量类型
来源：http://xhp.hysaishi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cym.zhongyouzk.top

[T43] Perl：字符串插值
来源：http://vgo.jiagoushi.top

"值: $a"
来源：http://txt.jinyuanbaomall.cn

[T44] Perl：条件
来源：http://xfv.ivvv.top

if ($a > 0) { print "正"; }
来源：http://akc.jinghuilouyu.cn

[T45] Perl：数组遍历
来源：http://sxm.yonumen.top

for my $x (@arr) { print $x; }
来源：http://rfg.fanxiaobao.xyz

[T46] Perl：哈希操作
来源：http://iic.yuanzhike.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cgw.xuetiantiany.cn

[T47] Perl：正则捕获
来源：http://zan.cdnleiting.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://gun.yonumen.top

[T48] Perl：正则替换
来源：http://dfz.sufxvd.cn

$s =~ s/old/new/g;
来源：http://mfh.hnqzz.top

[T49] Perl：函数
来源：http://nql.svipenyu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jnu.yj202588.top

[T50] Perl：逐行读文件
来源：http://wfj.9152youxi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://kcr.sweek.top

while (my $line = <$fh>) { print $line; }
来源：http://qro.guannengcc.top

[T51] Scala：Hello World
来源：http://bwm.shuidangran.top

println("Hello")
来源：http://hff.fanxiaobao.xyz

[T52] Scala：变量
来源：http://aws.haohaochexian.top

val a = 1;  var b = 2
来源：http://sfh.feifeiyinyue.top

[T53] Scala：字符串插值
来源：http://cda.chenlongwang.top

s"值: $b"
来源：http://xuo.shanyushiyangtech.top

[T54] Scala：集合映射
来源：http://ugc.feifeiyinyue.top

List(1, 2, 3).map(_ * 2)
来源：http://pxy.sjlbkw.cn

[T55] Scala：集合过滤
来源：http://gsj.yvedp.cn

List(1, 2, 3).filter(_ > 1)
来源：http://onj.zhiwuduotai.top

[T56] Scala：样例类
来源：http://ybw.cdnleiting.top

case class User(name: String, age: Int)
来源：http://ayt.zhiwuduotai.top

[T57] Scala：模式匹配
来源：http://dsf.wangdashe.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://fog.gaohongyu789.top

[T58] Scala：函数定义
来源：http://lfj.zhiwuduotai.top

def add(a: Int, b: Int): Int = a + b
来源：http://ukh.shzxlz.cn

[T59] Scala：循环
来源：http://lzv.xingfuxueyuan.xyz

for (i <- 1 to 10) println(i)
来源：http://uls.jinqigufen.top

[T60] Scala：折叠
来源：http://mxi.yj202588.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://zdp.zdbjq.cn

================================================================================
来源：http://qyv.jyoumei.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cxi.hcnkem.com

================================================================================
来源：http://nbi.sxryk.cn

[U01] Py：创建虚拟环境
来源：http://cfo.hongshengwenyu.top

python -m venv .venv && source .venv/bin/activate
来源：http://njc.svipenyu.cn

[U02] Py：导出 / 安装依赖
来源：http://zfv.hnxiangtu.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://alt.shangyingyoupin.top

[U03] Py：加载 .env 配置
来源：http://ful.nanxuanxn.top

from dotenv import load_dotenv; load_dotenv()
来源：http://qlw.shangyingyoupin.top

[U04] Py：变量调试打印
来源：http://xdv.nwbrower.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wdi.yuxming.cn

[U05] Py：列表去重且保序
来源：http://zsk.dianchejie.cn

list(dict.fromkeys(arr))
来源：http://qjc.pycfn.com

[U06] Py：合并两个字典
来源：http://tum.yonumen.top

{**a, **b}
来源：http://csi.fanxiaobao.xyz

[U07] Py：反转字典键值
来源：http://ceh.gogol.net.cn

{v: k for k, v in d.items()}
来源：http://wsw.jinghuilouyu.cn

[U08] Py：展平二维列表
来源：http://ono.ydzc1.top

[y for x in nested for y in x]
来源：http://jdx.jiagoushi.top

[U09] Py：字典取最大值的键
来源：http://jyb.zdbjq.cn

max(d, key=d.get)
来源：http://gdw.hcnkem.com

[U10] Py：按值排序字典
来源：http://adm.fanxiaobao.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cmz.sysykeji.top

[U11] Py：生成器表达式
来源：http://sat.zhixingplan.top

(x * 2 for x in arr)
来源：http://cgb.316326.xyz

[U12] Py：取出现最多的 3 个元素
来源：http://qld.nanxinkj.top

Counter(arr).most_common(3)
来源：http://pgl.nanxinkj.top


<!-- 参考信息 -->