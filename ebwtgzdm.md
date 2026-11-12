代发 wailian999

date +"%Y-%m-%d %H:%M:%S"
来源：http://tdw.cucudq.cn

[R72] 等待端口就绪
来源：http://cyw.xingfuxueyuan.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://log.chenjidiqi.icu

[R73] 分割大日志
来源：http://woe.guowangkeji.top

split -l 1000 big.log part_
来源：http://klk.yuxming.cn

[R74] 批量重命名
来源：http://sqd.hnqzz.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wcv.redwolf501.top

[R75] 导出环境变量
来源：http://dky.feifeiyinyue.top

export PATH="$HOME/bin:$PATH"
来源：http://sbt.smart0.xyz

[R76] 使用临时文件
来源：http://ooe.sysykeji.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xpv.zdqjudy.top

[R77] 读取用户输入
来源：http://gno.hnqzz.top

read -rp "请输入: " ans
来源：http://dhp.hcnkem.com

[R78] 交互式菜单
来源：http://yuy.xingfuxueyuan.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://kpc.zhongyouzk.top

[R79] 解析命令行选项
来源：http://yng.gogol.net.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://aur.yonumen.top

[R80] 查看脚本执行耗时
来源：http://jsj.nanxuanxn.top

time ./run.sh
来源：http://thk.gotoacloud.top

================================================================================
来源：http://olt.shangyingyoupin.top

S. C / C++ 专题
来源：http://rkw.zhiwuduotai.top

================================================================================
来源：http://luq.zhengqikj.top

[S01] C：Hello World
来源：http://ulf.yfazqb.com

#include <stdio.h>
来源：http://opn.redwolf501.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://oxu.fktsv.cn

[S02] C：变量与格式化输出
来源：http://lpx.haohaochexian.top

int a = 10; printf("%d\n", a);
来源：http://iao.birdmap.top

[S03] C：读入整数
来源：http://thv.haohaochexian.top

int x; scanf("%d", &x);
来源：http://gmu.yvedp.cn

[S04] C：字符串复制
来源：http://xjg.xingfuxueyuan.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://hln.jinqigufen.top

[S05] C：字符串长度
来源：http://dhi.fanxiaobao.xyz

strlen(s)
来源：http://jew.zdqjudy.top

[S06] C：字符串比较
来源：http://nbx.mhx1999.top

strcmp(a, b) == 0
来源：http://bvk.wangdashe.top

[S07] C：数组遍历求和
来源：http://emt.chenjidiqi.icu

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tdu.guowangkeji.top

[S08] C：动态内存分配与释放
来源：http://agz.fktsv.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://iir.daria6918.cn

[S09] C：结构体定义与初始化
来源：http://aje.sjlbkw.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tfq.sysykeji.top

[S10] C：指针与解引用
来源：http://riv.yfazqb.com

int *p = &a;  *p = 5;
来源：http://qcd.9152youxi.cn

[S11] C：逐行读文件
来源：http://rcb.pengpengdd.cyou

FILE *f = fopen("a.txt", "r");
来源：http://boq.tanke756.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://sit.mhx1999.top

fclose(f);
来源：http://wdm.kuanghao11.cn

[S12] C：写文件
来源：http://ieb.jinghuilouyu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yox.shanyushiyangkeji.top

[S13] C：宏定义
来源：http://fdb.gotoacloud.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://aze.zhongyouzk.top

[S14] C：枚举
来源：http://fub.jianghu66.top

enum Color { RED, GREEN, BLUE };
来源：http://ish.gogol.net.cn

[S15] C：类型转换
来源：http://tpd.xziqi.cn

(double) a / b
来源：http://ebb.feifeiyinyue.top

[S16] C：位操作置位
来源：http://hif.guannengcc.top

x |= (1 << 3);
来源：http://esq.tian-w.cn

[S17] C：安全拼接字符串
来源：http://mad.chenlongwang.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://akc.316326.xyz

[S18] C：命令行参数
来源：http://elv.shzxlz.cn

int main(int argc, char **argv)
来源：http://fzz.iojbl.cn

[S19] C：快速排序
来源：http://jid.vehdjk.com

qsort(a, n, sizeof(int), cmp);
来源：http://hzz.nwbrower.top

[S20] C：二分查找
来源：http://gza.hnxiangtu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dnj.jinqigfzy.top

[S21] C：字符类别判断
来源：http://moo.chenlongwang.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ijy.cucudq.cn

[S22] C：字符串转数字
来源：http://cuh.svipenyu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://mzw.fehbvm.com

[S23] C：随机数
来源：http://drs.zhijiandao.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://lwh.zdbjq.cn

[S24] C：获取本地时间
来源：http://bvs.ydjk.org.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://liv.hfpthk.cn

[S25] C：内存拷贝
来源：http://uwi.fktsv.cn

memcpy(dst, src, n);
来源：http://nph.xuetiantiany.cn

[S26] C：内存清零
来源：http://ksw.jqgufenzy.top

memset(a, 0, sizeof a);
来源：http://daw.epnwcf.com

[S27] C：定义常量
来源：http://hen.vehdjk.com

const double PI = 3.14159;
来源：http://nvj.bbcook.cn

[S28] C：静态变量
来源：http://fyr.fanxiaobao.xyz

static int counter = 0;
来源：http://mzg.gogol.net.cn

[S29] C：变参函数
来源：http://erf.snrcjt.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hbf.ctjpmb.com

[S30] C：头文件保护
来源：http://bzj.uphjek.com

#ifndef X_H
来源：http://qvj.iojbl.cn

#define X_H
来源：http://lok.ywan-chungtsiang.top

#endif
来源：http://qgk.snrcjt.cn

[S31] C++：Hello World
来源：http://oga.hnxiangtu.top

#include <iostream>
来源：http://vrx.ydjk.org.cn

int main() { std::cout << "Hello\n"; }
来源：http://gza.uphjek.com

[S32] C++：字符串
来源：http://voj.aizwys.cn

std::string s = "hi";  s += "!";
来源：http://och.cdnleiting.top

[S33] C++：vector 增删
来源：http://yty.yonumen.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yin.zhoulong.xyz

[S34] C++：遍历 vector
来源：http://hsj.yj20258.top

for (auto &x : v) { std::cout << x; }
来源：http://ncg.xziqi.cn

[S35] C++：map
来源：http://vvi.sjlbkw.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vad.316326.xyz

[S36] C++：unordered_map
来源：http://yfh.jinqigfzy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kyy.hnqzz.top

[S37] C++：set
来源：http://kib.yj20258888.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://phg.52xcode.cn

[S38] C++：排序
来源：http://rpw.meibo888.top

std::sort(v.begin(), v.end());
来源：http://ydd.vehdjk.com

[S39] C++：自定义比较器排序
来源：http://bxy.nanxuanxn.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mia.ehwqpu.com

[S40] C++：查找元素
来源：http://nlt.pengpengdd.cyou

auto it = std::find(v.begin(), v.end(), 3);
来源：http://boy.hnxiangtu.top

[S41] C++：类与构造函数
来源：http://wgi.sysykeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hzh.hongshengwenyu.top

[S42] C++：继承与虚函数
来源：http://wzl.gaohongyu789.top

class B : public Base { public: void f() override {} };
来源：http://ubk.yonumen.top

[S43] C++：智能指针
来源：http://ive.jianghu66.top

auto p = std::make_unique<int>(5);
来源：http://vyz.aizwys.cn

[S44] C++：引用传参
来源：http://tfe.jlsjyb.cn

void inc(int &x) { ++x; }
来源：http://mlb.jinyuanbaomall.cn

[S45] C++：lambda
来源：http://ygg.haohaochexian.top

auto add = [](int a, int b) { return a + b; };
来源：http://wgj.sxryk.cn

[S46] C++：函数模板
来源：http://gxq.ybcxt.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tdu.hcnkem.com

[S47] C++：结构化绑定遍历
来源：http://dxh.pycfn.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qoe.sweek.top

[S48] C++：逐行读文件
来源：http://bjh.fzhhl.top

std::ifstream in("a.txt");  std::string line;
来源：http://vbp.gogol.net.cn

while (std::getline(in, line)) { }
来源：http://ueb.fanxiaobao.xyz

[S49] C++：写文件
来源：http://xnv.dianchejie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://liw.fanxiaobao.xyz

[S50] C++：格式化数字
来源：http://ifp.havefunace.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vut.cheryme.top

[S51] C++：显式类型转换
来源：http://koa.svipenyu.cn

static_cast<double>(a) / b
来源：http://zyg.ybcxt.top

[S52] C++：const 与 noexcept
来源：http://zep.zhengqikj.top

int size() const noexcept { return n_; }
来源：http://ugd.c1oappe.top

[S53] C++：移动语义
来源：http://bnu.ppjwa.cn

std::vector<int> w = std::move(v);
来源：http://sbc.yj20258.top

[S54] C++：异常处理
来源：http://djf.wangdashe.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jro.yangfankeji.com

[S55] C++：结构化绑定
来源：http://qfl.nanxuanxn.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ycl.shzxlz.cn

[S56] C++：optional
来源：http://jpj.tian-w.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://flg.zhixingplan.top

[S57] C++：编译期常量
来源：http://hro.snrcjt.cn

constexpr int N = 10;
来源：http://ger.chenjidiqi.icu

[S58] C++：命名空间
来源：http://oft.gaohongyu789.top

namespace ns { int f() { return 1; } }
来源：http://cdy.cdnleiting.top

[S59] C++：静态断言
来源：http://djk.pengpengdd.cyou

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uaf.chenjidiqi.icu

[S60] C++：遍历并删除元素
来源：http://pdc.kuanghao11.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ymc.yangfankeji.com

================================================================================
来源：http://pzg.ywan-chungtsiang.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zyl.svipenyu.cn

================================================================================
来源：http://fma.aizwys.cn

[T01] Kotlin：Hello World
来源：http://kat.hnxiangtu.top

println("Hello")
来源：http://gvg.xylfe.cn

[T02] Kotlin：变量
来源：http://yei.jqgufenzy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vdi.yongpay.top

[T03] Kotlin：字符串模板
来源：http://cue.chenzaomai.com

"值: $b"
来源：http://bgw.fanxiaobao.xyz

[T04] Kotlin：空安全
来源：http://hkq.fzhhl.top

val n: String? = null;  n?.length
来源：http://wym.hywenlv.cn

[T05] Kotlin：when 表达式
来源：http://qfv.iojbl.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gsg.zhengqikj.top

[T06] Kotlin：集合映射
来源：http://hmw.c1oappe.top

listOf(1, 2, 3).map { it * 2 }
来源：http://rxi.tarul.cn

[T07] Kotlin：集合过滤
来源：http://vwa.gaohongyu789.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://acu.hesvh.cn

[T08] Kotlin：数据类
来源：http://ewk.daxiang520.top

data class User(val name: String, val age: Int)
来源：http://kaq.yvedp.cn

[T09] Kotlin：扩展函数
来源：http://hip.ywan-chungtsiang.top

fun String.exclaim() = this + "!"
来源：http://fdn.hfpthk.cn

[T10] Kotlin：默认参数
来源：http://vzg.havefunace.top

fun greet(name: String = "World") = "Hi $name"
来源：http://oka.xuetiantiany.cn

[T11] Kotlin：协程
来源：http://bol.wangshuangyany.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://czv.haohaochexian.top

[T12] Kotlin：解构声明
来源：http://hsu.shanyushiyangtech.top

val (a, b) = Pair(1, 2)
来源：http://tyr.zdbjq.cn

[T13] Kotlin：只读 Map
来源：http://esa.xinyue.icu

val m = mapOf("a" to 1)
来源：http://umn.zdqjudy.top

[T14] Kotlin：循环
来源：http://zci.sweek.top

for (i in 1..10) println(i)
来源：http://vzf.sysykeji.top

[T15] Kotlin：接口
来源：http://dsl.nwbrower.top

interface Shape { fun area(): Double }
来源：http://jxb.ybcxt.top

[T16] Swift：Hello World
来源：http://hld.yj20258.top

print("Hello")
来源：http://zuc.svipenyu.cn

[T17] Swift：变量与常量
来源：http://kxy.havefunace.top

var a = 1;  let b = 2
来源：http://nea.redwolf501.top

[T18] Swift：字符串插值
来源：http://bwo.zhixingplan.top

"值: \(b)"
来源：http://vpt.jiagoushi.top

[T19] Swift：可选绑定
来源：http://wnx.hammf.cn

if let n = opt { print(n) }
来源：http://jqm.guowangkeji.top

[T20] Swift：数组操作
来源：http://tbj.xylfe.cn

var a = [1, 2, 3];  a.append(4)
来源：http://nco.hysaishi.cn

[T21] Swift：遍历
来源：http://kma.zhiwuduotai.top

for x in a { print(x) }
来源：http://gwj.hnqzz.top

[T22] Swift：字典
来源：http://fzt.zhiwuduotai.top

var d = ["a": 1];  d["b"] = 2
来源：http://lva.gaohongyu789.top

[T23] Swift：函数
来源：http://tjy.hesvh.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ldk.ivvv.top

[T24] Swift：闭包
来源：http://pmm.mhx1999.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ncj.vqdsnc.cn

[T25] Swift：结构体
来源：http://vkr.jinqigufen.top

struct P { var x: Int }
来源：http://tus.fanxiaobao.xyz

[T26] Swift：类与重写
来源：http://liu.dashuyun.cn

class A: Base { override func f() {} }
来源：http://tlh.vqdsnc.cn

[T27] Swift：错误处理
来源：http://vay.vehdjk.com

do { try f() } catch { print(error) }
来源：http://zyi.yvedp.cn

[T28] Swift：枚举
来源：http://mca.jqgufenzy.top

enum Color { case red, green }
来源：http://brl.wangdashe.top

[T29] Swift：guard 提前返回
来源：http://ens.hywenlv.cn

guard let x = opt else { return }
来源：http://svn.sweek.top

[T30] Swift：协议
来源：http://vnj.yj20258.top

protocol Shape { func area() -> Double }
来源：http://nbt.smart0.xyz

[T31] Lua：Hello World
来源：http://sfj.gzhubu.top

print("Hello")
来源：http://shu.tarul.cn

[T32] Lua：局部变量
来源：http://eob.daria6918.cn

local a = 1
来源：http://bsm.shangyingyoupin.top

[T33] Lua：表（数组）
来源：http://ble.nanxinkj.top

local t = {1, 2, 3};  t[4] = 4
来源：http://vep.hysaishi.cn

[T34] Lua：遍历表
来源：http://poq.zhoulong.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://wbc.bbcook.cn

[T35] Lua：字典表
来源：http://sgp.ydzc1.top

local d = { a = 1 };  d.b = 2
来源：http://per.ydjk.org.cn

[T36] Lua：函数
来源：http://pxd.ywan-chungtsiang.top

function add(a, b) return a + b end
来源：http://tmn.jqgufenzy.top

[T37] Lua：字符串拼接
来源：http://niy.zdbjq.cn

"a" .. "b"
来源：http://wyt.aibaodan.cn

[T38] Lua：条件
来源：http://foy.chenzaomai.com

if x > 0 then print("正") end
来源：http://yrv.zhijiandao.cn

[T39] Lua：模式匹配
来源：http://rqs.dianchejie.cn

string.find(s, "%d+")
来源：http://azd.tianlin.xyz

[T40] Lua：元表
来源：http://gil.xziqi.cn

setmetatable({}, { __index = base })
来源：http://ecf.zhiwuduotai.top

[T41] Perl：Hello World
来源：http://fdl.aibaodan.cn

print "Hello\n";
来源：http://tpi.tarul.cn

[T42] Perl：变量类型
来源：http://jqn.birdmap.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ocr.mhx1999.top

[T43] Perl：字符串插值
来源：http://mka.52xcode.cn

"值: $a"
来源：http://erq.fengsongda.top

[T44] Perl：条件
来源：http://csl.yonumen.top

if ($a > 0) { print "正"; }
来源：http://lsq.tarul.cn

[T45] Perl：数组遍历
来源：http://qgh.feifeiyinyue.top

for my $x (@arr) { print $x; }
来源：http://htt.xinyue.icu

[T46] Perl：哈希操作
来源：http://qpe.aizwys.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vlk.fengsongda.top

[T47] Perl：正则捕获
来源：http://prz.jiagoushi.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://vep.kuanghao11.cn

[T48] Perl：正则替换
来源：http://yue.ppjwa.cn

$s =~ s/old/new/g;
来源：http://xok.hnqzz.top

[T49] Perl：函数
来源：http://abk.pycfn.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://tqm.gotoacloud.top

[T50] Perl：逐行读文件
来源：http://iwi.cheryme.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ind.vehdjk.com

while (my $line = <$fh>) { print $line; }
来源：http://wyp.ydjk.org.cn

[T51] Scala：Hello World
来源：http://amr.wangshuangyany.cn

println("Hello")
来源：http://nnl.ppjwa.cn

[T52] Scala：变量
来源：http://btj.cheryme.top

val a = 1;  var b = 2
来源：http://wav.ybcxt.top

[T53] Scala：字符串插值
来源：http://fio.feifeiyinyue.top

s"值: $b"
来源：http://otx.gaohongyu789.top

[T54] Scala：集合映射
来源：http://evn.kuanghao11.cn

List(1, 2, 3).map(_ * 2)
来源：http://gsz.zhongyouzk.top

[T55] Scala：集合过滤
来源：http://dwj.yuanzhike.top

List(1, 2, 3).filter(_ > 1)
来源：http://qop.shanyushiyangtech.top

[T56] Scala：样例类
来源：http://oiv.epnwcf.com

case class User(name: String, age: Int)
来源：http://pva.jianghu66.top

[T57] Scala：模式匹配
来源：http://elq.ybcxt.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ivn.tanke756.top

[T58] Scala：函数定义
来源：http://prn.zhengqikj.top

def add(a: Int, b: Int): Int = a + b
来源：http://xvg.jinqigufen.top

[T59] Scala：循环
来源：http://vpw.xinyue.icu

for (i <- 1 to 10) println(i)
来源：http://azo.zycfv.cn

[T60] Scala：折叠
来源：http://qmi.nanxinkj.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kyg.yj202588.top

================================================================================
来源：http://tpl.yfazqb.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dsk.chenjidiqi.icu

================================================================================
来源：http://drd.zhoulong.xyz

[U01] Py：创建虚拟环境
来源：http://cee.fanxiaobao.xyz

python -m venv .venv && source .venv/bin/activate
来源：http://crr.snrcjt.cn

[U02] Py：导出 / 安装依赖
来源：http://cfi.fengsongda.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dtb.iojbl.cn

[U03] Py：加载 .env 配置
来源：http://vfe.zhongyouzk.top

from dotenv import load_dotenv; load_dotenv()
来源：http://wfc.ppjwa.cn

[U04] Py：变量调试打印
来源：http://hkr.shuidangran.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ipw.sufxvd.cn

[U05] Py：列表去重且保序
来源：http://lfe.smart0.xyz

list(dict.fromkeys(arr))
来源：http://lnt.zhixingplan.top

[U06] Py：合并两个字典
来源：http://ilv.snrcjt.cn

{**a, **b}
来源：http://jhn.pycfn.com

[U07] Py：反转字典键值
来源：http://wvd.chenjidiqi.icu

{v: k for k, v in d.items()}
来源：http://dmm.smart0.xyz

[U08] Py：展平二维列表
来源：http://rux.ywan-chungtsiang.top

[y for x in nested for y in x]
来源：http://xcq.zhaomingkeji.xyz

[U09] Py：字典取最大值的键
来源：http://rmo.ehwqpu.com

max(d, key=d.get)
来源：http://ded.yangfankeji.com

[U10] Py：按值排序字典
来源：http://vdu.tianlin.xyz

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lsk.yangfankeji.com

[U11] Py：生成器表达式
来源：http://khp.0kj1m.cn

(x * 2 for x in arr)
来源：http://gzz.zhixingplan.top

[U12] Py：取出现最多的 3 个元素
来源：http://dts.vqdsnc.cn

Counter(arr).most_common(3)
来源：http://tin.cdnleiting.top


<!-- 参考信息 -->