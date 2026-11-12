代发 wailian999

openssl rand -hex 16
来源：http://xjh.sysykeji.top

[R68] 计算文件校验值
来源：http://thu.fanxiaobao.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://dic.vqdsnc.cn

[R69] 生成随机密码
来源：http://zjo.shangyingyoupin.top

head -c 16 /dev/urandom | base64
来源：http://qvo.cucudq.cn

[R70] 时间戳与互转
来源：http://mvc.zhixingplan.top

date +%s;  date -d @1700000000
来源：http://ctf.jyoumei.cn

[R71] 日期格式化
来源：http://tik.svipenyu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://vvs.hcnkem.com

[R72] 等待端口就绪
来源：http://pjs.ehwqpu.com

until nc -z localhost 3306; do sleep 1; done
来源：http://ivi.guowangkeji.top

[R73] 分割大日志
来源：http://vku.hywenlv.cn

split -l 1000 big.log part_
来源：http://wbv.xingfuxueyuan.xyz

[R74] 批量重命名
来源：http://pen.yj20258.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fvq.meibo888.top

[R75] 导出环境变量
来源：http://lkn.yangfankeji.com

export PATH="$HOME/bin:$PATH"
来源：http://vwq.hcnkem.com

[R76] 使用临时文件
来源：http://pos.xuetiantiany.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pjy.tian-w.cn

[R77] 读取用户输入
来源：http://wxw.shanyushiyangkeji.top

read -rp "请输入: " ans
来源：http://jgy.yj20258.top

[R78] 交互式菜单
来源：http://vmq.jqgufenzy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://unb.nwbrower.top

[R79] 解析命令行选项
来源：http://rfq.jqgfzy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gcy.jlsjyb.cn

[R80] 查看脚本执行耗时
来源：http://zbh.wangshuangyany.cn

time ./run.sh
来源：http://ahi.zhengqikj.top

================================================================================
来源：http://gli.shangyingyoupin.top

S. C / C++ 专题
来源：http://ejj.tian-w.cn

================================================================================
来源：http://zhc.9152youxi.cn

[S01] C：Hello World
来源：http://bem.gaohongyu789.top

#include <stdio.h>
来源：http://nmh.yj20258.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://evk.snrcjt.cn

[S02] C：变量与格式化输出
来源：http://xag.vqdsnc.cn

int a = 10; printf("%d\n", a);
来源：http://nbf.shzxlz.cn

[S03] C：读入整数
来源：http://fno.jqgfzy.top

int x; scanf("%d", &x);
来源：http://ili.shanyushiyangkeji.top

[S04] C：字符串复制
来源：http://owu.hnqzz.top

char dst[32]; strcpy(dst, "hi");
来源：http://skr.yuxming.cn

[S05] C：字符串长度
来源：http://mwn.nanxinkj.top

strlen(s)
来源：http://yhf.yvedp.cn

[S06] C：字符串比较
来源：http://vlw.ydzc1.top

strcmp(a, b) == 0
来源：http://dqu.jyoumei.cn

[S07] C：数组遍历求和
来源：http://edl.hongshengwenyu.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gdi.yuanzhike.top

[S08] C：动态内存分配与释放
来源：http://rca.guowangkeji.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://duf.ctjpmb.com

[S09] C：结构体定义与初始化
来源：http://wcd.9152youxi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rjl.wangshuangyany.cn

[S10] C：指针与解引用
来源：http://pie.ybcxt.top

int *p = &a;  *p = 5;
来源：http://bbt.ydzc1.top

[S11] C：逐行读文件
来源：http://kxr.jinqigufen.top

FILE *f = fopen("a.txt", "r");
来源：http://uit.zdbjq.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dpj.0kj1m.cn

fclose(f);
来源：http://sql.gzhubu.top

[S12] C：写文件
来源：http://qkm.yangfankeji.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yfr.nanxuanxn.top

[S13] C：宏定义
来源：http://amr.chenjidiqi.icu

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tgw.cqqwz.cn

[S14] C：枚举
来源：http://prh.hfpthk.cn

enum Color { RED, GREEN, BLUE };
来源：http://uzk.uphjek.com

[S15] C：类型转换
来源：http://xgl.iojbl.cn

(double) a / b
来源：http://fjz.gogol.net.cn

[S16] C：位操作置位
来源：http://usz.uphjek.com

x |= (1 << 3);
来源：http://bwv.shanyushiyangkeji.top

[S17] C：安全拼接字符串
来源：http://qqk.fengsongda.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xzo.sysykeji.top

[S18] C：命令行参数
来源：http://hvg.yfazqb.com

int main(int argc, char **argv)
来源：http://lyj.yongpay.top

[S19] C：快速排序
来源：http://xhw.fehbvm.com

qsort(a, n, sizeof(int), cmp);
来源：http://kck.ehwqpu.com

[S20] C：二分查找
来源：http://ekw.hongshengwenyu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yam.daria6918.cn

[S21] C：字符类别判断
来源：http://vwt.aizwys.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hfm.jiagoushi.top

[S22] C：字符串转数字
来源：http://aaf.mhx1999.top

atoi("42");  strtod("3.14", NULL);
来源：http://hqh.yueranfly.top

[S23] C：随机数
来源：http://isv.yj20258888.top

srand(time(NULL));  int r = rand() % 100;
来源：http://szl.xuetiantiany.cn

[S24] C：获取本地时间
来源：http://crh.zhoulong.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ghn.yangfankeji.com

[S25] C：内存拷贝
来源：http://lss.zdqjudy.top

memcpy(dst, src, n);
来源：http://djv.fzhhl.top

[S26] C：内存清零
来源：http://hej.hnxiangtu.top

memset(a, 0, sizeof a);
来源：http://zfl.gotoacloud.top

[S27] C：定义常量
来源：http://ulw.chenlongwang.top

const double PI = 3.14159;
来源：http://yyy.zhoulong.xyz

[S28] C：静态变量
来源：http://idg.chenzaomai.com

static int counter = 0;
来源：http://stb.jqgfzy.top

[S29] C：变参函数
来源：http://ubs.gotoacloud.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nob.fktsv.cn

[S30] C：头文件保护
来源：http://agr.sufxvd.cn

#ifndef X_H
来源：http://plz.yj20258.top

#define X_H
来源：http://mxm.fengsongda.top

#endif
来源：http://aby.fehbvm.com

[S31] C++：Hello World
来源：http://vvf.jinqigfzy.top

#include <iostream>
来源：http://zfr.yangfankeji.com

int main() { std::cout << "Hello\n"; }
来源：http://zme.ydzc1.top

[S32] C++：字符串
来源：http://aey.shuidangran.top

std::string s = "hi";  s += "!";
来源：http://rno.ybcxt.top

[S33] C++：vector 增删
来源：http://qus.cqqwz.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fiy.iojbl.cn

[S34] C++：遍历 vector
来源：http://ukz.zdbjq.cn

for (auto &x : v) { std::cout << x; }
来源：http://hik.chenzaomai.com

[S35] C++：map
来源：http://yzu.hnxiangtu.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kfr.jinqigufen.top

[S36] C++：unordered_map
来源：http://qww.tian-w.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ypd.c1oappe.top

[S37] C++：set
来源：http://ili.yangfankeji.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xkj.snrcjt.cn

[S38] C++：排序
来源：http://pjr.9152youxi.cn

std::sort(v.begin(), v.end());
来源：http://bdb.xylfe.cn

[S39] C++：自定义比较器排序
来源：http://upi.sysykeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mta.jqgufenzy.top

[S40] C++：查找元素
来源：http://pff.zhongyouzk.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cpq.zdqjudy.top

[S41] C++：类与构造函数
来源：http://ekr.zhiwuduotai.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dgt.fengsongda.top

[S42] C++：继承与虚函数
来源：http://dtt.nwbrower.top

class B : public Base { public: void f() override {} };
来源：http://cgz.pengpengdd.cyou

[S43] C++：智能指针
来源：http://cui.tanke756.top

auto p = std::make_unique<int>(5);
来源：http://ywp.sufxvd.cn

[S44] C++：引用传参
来源：http://irb.pycfn.com

void inc(int &x) { ++x; }
来源：http://iyu.quarkkingdee.top

[S45] C++：lambda
来源：http://pxy.hywenlv.cn

auto add = [](int a, int b) { return a + b; };
来源：http://das.hongshengwenyu.top

[S46] C++：函数模板
来源：http://xgt.uphjek.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tvb.gaohongyu789.top

[S47] C++：结构化绑定遍历
来源：http://qcz.cashguo.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://abu.zhoulong.xyz

[S48] C++：逐行读文件
来源：http://sos.fanxiaobao.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://lmx.yangfankeji.com

while (std::getline(in, line)) { }
来源：http://jfu.kuanghao11.cn

[S49] C++：写文件
来源：http://zty.0kj1m.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://aws.shanyushiyangkeji.top

[S50] C++：格式化数字
来源：http://zqn.fehbvm.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lcn.pengpengdd.cyou

[S51] C++：显式类型转换
来源：http://uaf.xinyue.icu

static_cast<double>(a) / b
来源：http://xji.52xcode.cn

[S52] C++：const 与 noexcept
来源：http://udc.yonumen.top

int size() const noexcept { return n_; }
来源：http://sxw.yfazqb.com

[S53] C++：移动语义
来源：http://oeg.andypj.xyz

std::vector<int> w = std::move(v);
来源：http://yax.meibo888.top

[S54] C++：异常处理
来源：http://hqf.xuetiantiany.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mii.jyoumei.cn

[S55] C++：结构化绑定
来源：http://fab.jinqigfzy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://nhc.chenlongwang.top

[S56] C++：optional
来源：http://dgk.yongpay.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://iut.zhoulong.xyz

[S57] C++：编译期常量
来源：http://bte.wangshuangyany.cn

constexpr int N = 10;
来源：http://cwa.bjfxy.top

[S58] C++：命名空间
来源：http://zno.vqdsnc.cn

namespace ns { int f() { return 1; } }
来源：http://gos.iojbl.cn

[S59] C++：静态断言
来源：http://fcy.pengpengdd.cyou

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ggy.yanxiufei.cn

[S60] C++：遍历并删除元素
来源：http://hak.chenlongwang.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://agc.nwbrower.top

================================================================================
来源：http://sqc.havefunace.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jyc.zdqjudy.top

================================================================================
来源：http://alf.yongpay.top

[T01] Kotlin：Hello World
来源：http://vyw.jlsjyb.cn

println("Hello")
来源：http://erq.yangfankeji.com

[T02] Kotlin：变量
来源：http://ljo.nwbrower.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wis.shzxlz.cn

[T03] Kotlin：字符串模板
来源：http://prz.dianchejie.cn

"值: $b"
来源：http://spz.dianchejie.cn

[T04] Kotlin：空安全
来源：http://jnb.tanke756.top

val n: String? = null;  n?.length
来源：http://bxx.wangdashe.top

[T05] Kotlin：when 表达式
来源：http://wvq.zycfv.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ixa.zhengqikj.top

[T06] Kotlin：集合映射
来源：http://dis.xingfuxueyuan.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://xub.vqdsnc.cn

[T07] Kotlin：集合过滤
来源：http://fip.yuanzhike.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://mbr.jyoumei.cn

[T08] Kotlin：数据类
来源：http://hzu.chenlongwang.top

data class User(val name: String, val age: Int)
来源：http://wwn.0kj1m.cn

[T09] Kotlin：扩展函数
来源：http://gno.aizwys.cn

fun String.exclaim() = this + "!"
来源：http://uav.aizwys.cn

[T10] Kotlin：默认参数
来源：http://rtk.meibo888.top

fun greet(name: String = "World") = "Hi $name"
来源：http://yhd.zhaomingkeji.xyz

[T11] Kotlin：协程
来源：http://ewa.havefunace.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ixf.xziqi.cn

[T12] Kotlin：解构声明
来源：http://xns.xuetiantiany.cn

val (a, b) = Pair(1, 2)
来源：http://mzg.jinqigfzy.top

[T13] Kotlin：只读 Map
来源：http://sys.cucudq.cn

val m = mapOf("a" to 1)
来源：http://kll.jqgufenzy.top

[T14] Kotlin：循环
来源：http://jfr.gogol.net.cn

for (i in 1..10) println(i)
来源：http://qut.sysykeji.top

[T15] Kotlin：接口
来源：http://cnp.xziqi.cn

interface Shape { fun area(): Double }
来源：http://ycl.zycfv.cn

[T16] Swift：Hello World
来源：http://lfe.fanxiaobao.xyz

print("Hello")
来源：http://gfr.daria6918.cn

[T17] Swift：变量与常量
来源：http://mub.hfpthk.cn

var a = 1;  let b = 2
来源：http://sdc.sjlbkw.cn

[T18] Swift：字符串插值
来源：http://jnz.feifeiyinyue.top

"值: \(b)"
来源：http://oeu.yvedp.cn

[T19] Swift：可选绑定
来源：http://jdi.kuanghao11.cn

if let n = opt { print(n) }
来源：http://yhb.chenjidiqi.icu

[T20] Swift：数组操作
来源：http://rca.yuanzhike.top

var a = [1, 2, 3];  a.append(4)
来源：http://xoo.xuetiantiany.cn

[T21] Swift：遍历
来源：http://scf.pengpengdd.cyou

for x in a { print(x) }
来源：http://mwd.redwolf501.top

[T22] Swift：字典
来源：http://lwf.hywenlv.cn

var d = ["a": 1];  d["b"] = 2
来源：http://jyv.andypj.xyz

[T23] Swift：函数
来源：http://uaz.sufxvd.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cdo.tianlin.xyz

[T24] Swift：闭包
来源：http://plw.yangfankeji.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://won.chenzaomai.com

[T25] Swift：结构体
来源：http://ilm.sweek.top

struct P { var x: Int }
来源：http://xpp.hfpthk.cn

[T26] Swift：类与重写
来源：http://bym.birdmap.top

class A: Base { override func f() {} }
来源：http://bhs.jinyuanbaomall.cn

[T27] Swift：错误处理
来源：http://kmx.ivvv.top

do { try f() } catch { print(error) }
来源：http://zpf.cdnleiting.top

[T28] Swift：枚举
来源：http://qev.gotoacloud.top

enum Color { case red, green }
来源：http://ehu.9152youxi.cn

[T29] Swift：guard 提前返回
来源：http://nvo.jiagoushi.top

guard let x = opt else { return }
来源：http://uuj.feifeiyinyue.top

[T30] Swift：协议
来源：http://xsq.ppjwa.cn

protocol Shape { func area() -> Double }
来源：http://dym.jlsjyb.cn

[T31] Lua：Hello World
来源：http://uxn.tanke756.top

print("Hello")
来源：http://bwy.yanxiufei.cn

[T32] Lua：局部变量
来源：http://wig.yuxming.cn

local a = 1
来源：http://jbx.0kj1m.cn

[T33] Lua：表（数组）
来源：http://nch.sweek.top

local t = {1, 2, 3};  t[4] = 4
来源：http://iro.quarkkingdee.top

[T34] Lua：遍历表
来源：http://nxu.sweek.top

for i, v in ipairs(t) do print(i, v) end
来源：http://bea.sweek.top

[T35] Lua：字典表
来源：http://wis.gogol.net.cn

local d = { a = 1 };  d.b = 2
来源：http://phs.yanxiufei.cn

[T36] Lua：函数
来源：http://zli.c1oappe.top

function add(a, b) return a + b end
来源：http://ead.hcnkem.com

[T37] Lua：字符串拼接
来源：http://kqw.pycfn.com

"a" .. "b"
来源：http://yak.jiagoushi.top

[T38] Lua：条件
来源：http://xqu.c1oappe.top

if x > 0 then print("正") end
来源：http://maf.yj20258888.top

[T39] Lua：模式匹配
来源：http://wuj.vqdsnc.cn

string.find(s, "%d+")
来源：http://qia.snrcjt.cn

[T40] Lua：元表
来源：http://qmd.meibo888.top

setmetatable({}, { __index = base })
来源：http://kmj.jinyuanbaomall.cn

[T41] Perl：Hello World
来源：http://abz.smart0.xyz

print "Hello\n";
来源：http://ffu.zhixingplan.top

[T42] Perl：变量类型
来源：http://teu.zdbjq.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tnq.dianchejie.cn

[T43] Perl：字符串插值
来源：http://sks.iojbl.cn

"值: $a"
来源：http://cjr.aizwys.cn

[T44] Perl：条件
来源：http://cwr.yj20258.top

if ($a > 0) { print "正"; }
来源：http://ukb.xziqi.cn

[T45] Perl：数组遍历
来源：http://afy.nanxinkj.top

for my $x (@arr) { print $x; }
来源：http://tyb.sjlbkw.cn

[T46] Perl：哈希操作
来源：http://iac.chenzaomai.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bby.dashuyun.cn

[T47] Perl：正则捕获
来源：http://ckq.yangfankeji.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://gva.shanyushiyangtech.top

[T48] Perl：正则替换
来源：http://oje.havefunace.top

$s =~ s/old/new/g;
来源：http://umz.svipenyu.cn

[T49] Perl：函数
来源：http://frz.zhaomingkeji.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zyo.jqgufenzy.top

[T50] Perl：逐行读文件
来源：http://wtz.daxiang520.top

open my $fh, "<", "a.txt" or die $!;
来源：http://bmn.yanxiufei.cn

while (my $line = <$fh>) { print $line; }
来源：http://vjc.yfazqb.com

[T51] Scala：Hello World
来源：http://ifu.ctjpmb.com

println("Hello")
来源：http://gyy.shanyushiyangkeji.top

[T52] Scala：变量
来源：http://vnf.yj20258.top

val a = 1;  var b = 2
来源：http://xsi.cdnleiting.top

[T53] Scala：字符串插值
来源：http://vlw.zdbjq.cn

s"值: $b"
来源：http://vpr.uphjek.com

[T54] Scala：集合映射
来源：http://pje.zdbjq.cn

List(1, 2, 3).map(_ * 2)
来源：http://gkj.tianlin.xyz

[T55] Scala：集合过滤
来源：http://kpm.xylfe.cn

List(1, 2, 3).filter(_ > 1)
来源：http://mrq.xuanzx.com

[T56] Scala：样例类
来源：http://ocd.sjlbkw.cn

case class User(name: String, age: Int)
来源：http://zoj.shanyushiyangkeji.top

[T57] Scala：模式匹配
来源：http://maq.daria6918.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ujc.hammf.cn

[T58] Scala：函数定义
来源：http://eda.9152youxi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://oof.sysykeji.top

[T59] Scala：循环
来源：http://ozj.svipenyu.cn

for (i <- 1 to 10) println(i)
来源：http://wno.tianlin.xyz

[T60] Scala：折叠
来源：http://krk.yongpay.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tka.jinyuanbaomall.cn

================================================================================
来源：http://spd.jqgufenzy.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dxs.9152youxi.cn

================================================================================
来源：http://lzm.shzxlz.cn

[U01] Py：创建虚拟环境
来源：http://hgg.yuxming.cn

python -m venv .venv && source .venv/bin/activate
来源：http://doo.birdmap.top

[U02] Py：导出 / 安装依赖
来源：http://tgo.shzxlz.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ezq.redwolf501.top

[U03] Py：加载 .env 配置
来源：http://exu.316326.xyz

from dotenv import load_dotenv; load_dotenv()
来源：http://nkc.xinyue.icu

[U04] Py：变量调试打印
来源：http://hiw.dianchejie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xhf.hesvh.cn

[U05] Py：列表去重且保序
来源：http://chi.chenzaomai.com

list(dict.fromkeys(arr))
来源：http://rvg.bjfxy.top

[U06] Py：合并两个字典
来源：http://scn.hywenlv.cn

{**a, **b}
来源：http://olh.xuetiantiany.cn

[U07] Py：反转字典键值
来源：http://heq.nanxuanxn.top

{v: k for k, v in d.items()}
来源：http://sid.hcnkem.com

[U08] Py：展平二维列表
来源：http://csy.gogol.net.cn

[y for x in nested for y in x]
来源：http://bmz.vehdjk.com


<!-- 参考信息 -->