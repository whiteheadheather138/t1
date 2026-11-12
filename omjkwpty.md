代发 wailian999

export PATH="$HOME/bin:$PATH"
来源：http://efd.guowangkeji.top

[R76] 使用临时文件
来源：http://zwe.birdmap.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nis.jianghu66.top

[R77] 读取用户输入
来源：http://mfb.pycfn.com

read -rp "请输入: " ans
来源：http://ihz.zdbjq.cn

[R78] 交互式菜单
来源：http://vxc.wangdashe.top

select opt in a b c; do echo "$opt"; break; done
来源：http://poe.tarul.cn

[R79] 解析命令行选项
来源：http://mbz.hnqzz.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cpm.cucudq.cn

[R80] 查看脚本执行耗时
来源：http://rra.zhaomingkeji.xyz

time ./run.sh
来源：http://gts.chenlongwang.top

================================================================================
来源：http://fwr.quarkkingdee.top

S. C / C++ 专题
来源：http://agv.quarkkingdee.top

================================================================================
来源：http://gln.guannengcc.top

[S01] C：Hello World
来源：http://jfa.tarul.cn

#include <stdio.h>
来源：http://ozr.0kj1m.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://iig.xylfe.cn

[S02] C：变量与格式化输出
来源：http://lcq.snrcjt.cn

int a = 10; printf("%d\n", a);
来源：http://vsk.zhixingplan.top

[S03] C：读入整数
来源：http://zdw.ydjk.org.cn

int x; scanf("%d", &x);
来源：http://cxr.zhengqikj.top

[S04] C：字符串复制
来源：http://yrw.yj20258888.top

char dst[32]; strcpy(dst, "hi");
来源：http://tiy.andypj.xyz

[S05] C：字符串长度
来源：http://kgk.dashuyun.cn

strlen(s)
来源：http://wzp.hfpthk.cn

[S06] C：字符串比较
来源：http://krs.xinyue.icu

strcmp(a, b) == 0
来源：http://kak.fengsongda.top

[S07] C：数组遍历求和
来源：http://xlo.tian-w.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gje.gzhubu.top

[S08] C：动态内存分配与释放
来源：http://ahr.fktsv.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ryq.tarul.cn

[S09] C：结构体定义与初始化
来源：http://xnj.zhiwuduotai.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rrg.316326.xyz

[S10] C：指针与解引用
来源：http://gku.sufxvd.cn

int *p = &a;  *p = 5;
来源：http://osv.sysykeji.top

[S11] C：逐行读文件
来源：http://zhw.nwbrower.top

FILE *f = fopen("a.txt", "r");
来源：http://syo.pengpengdd.cyou

while (fgets(buf, sizeof buf, f)) { }
来源：http://bwe.xuetiantiany.cn

fclose(f);
来源：http://qox.zdbjq.cn

[S12] C：写文件
来源：http://iqz.birdmap.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ihv.tian-w.cn

[S13] C：宏定义
来源：http://tjd.chenzaomai.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kes.yuxming.cn

[S14] C：枚举
来源：http://nyb.yj202588.top

enum Color { RED, GREEN, BLUE };
来源：http://ixt.chenzaomai.com

[S15] C：类型转换
来源：http://lup.yonumen.top

(double) a / b
来源：http://vqs.yongpay.top

[S16] C：位操作置位
来源：http://tcf.bbcook.cn

x |= (1 << 3);
来源：http://omu.sweek.top

[S17] C：安全拼接字符串
来源：http://kyh.316326.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qrl.zdbjq.cn

[S18] C：命令行参数
来源：http://gyf.yj202588.top

int main(int argc, char **argv)
来源：http://eit.yongpay.top

[S19] C：快速排序
来源：http://xma.jinghuilouyu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ulq.cashguo.top

[S20] C：二分查找
来源：http://npv.aibaodan.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blr.nanxinkj.top

[S21] C：字符类别判断
来源：http://zwt.fzhhl.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bew.xylfe.cn

[S22] C：字符串转数字
来源：http://oxc.sjlbkw.cn

atoi("42");  strtod("3.14", NULL);
来源：http://jzs.tarul.cn

[S23] C：随机数
来源：http://pgd.nwbrower.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ena.c1oappe.top

[S24] C：获取本地时间
来源：http://hxl.zdbjq.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tnr.tanke756.top

[S25] C：内存拷贝
来源：http://feh.yj20258.top

memcpy(dst, src, n);
来源：http://rbk.hesvh.cn

[S26] C：内存清零
来源：http://jyi.jinqigfzy.top

memset(a, 0, sizeof a);
来源：http://lwj.0kj1m.cn

[S27] C：定义常量
来源：http://asb.wangdashe.top

const double PI = 3.14159;
来源：http://ypv.ppjwa.cn

[S28] C：静态变量
来源：http://uzu.jlsjyb.cn

static int counter = 0;
来源：http://ekh.aibaodan.cn

[S29] C：变参函数
来源：http://mvl.jianghu66.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xgh.ehwqpu.com

[S30] C：头文件保护
来源：http://lwj.yuxming.cn

#ifndef X_H
来源：http://uvl.feifeiyinyue.top

#define X_H
来源：http://bkf.hesvh.cn

#endif
来源：http://zml.zhoulong.xyz

[S31] C++：Hello World
来源：http://ejj.hesvh.cn

#include <iostream>
来源：http://arw.yanxiufei.cn

int main() { std::cout << "Hello\n"; }
来源：http://yze.gzhubu.top

[S32] C++：字符串
来源：http://vzb.xuanzx.com

std::string s = "hi";  s += "!";
来源：http://hde.xuanzx.com

[S33] C++：vector 增删
来源：http://xwc.chenjidiqi.icu

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://eel.hywenlv.cn

[S34] C++：遍历 vector
来源：http://xip.havefunace.top

for (auto &x : v) { std::cout << x; }
来源：http://xix.chenzaomai.com

[S35] C++：map
来源：http://oae.shuidangran.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vhg.chenjidiqi.icu

[S36] C++：unordered_map
来源：http://mvb.chenzaomai.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cov.yvedp.cn

[S37] C++：set
来源：http://uqi.wangdashe.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fxs.tarul.cn

[S38] C++：排序
来源：http://esm.haohaochexian.top

std::sort(v.begin(), v.end());
来源：http://ijr.yonumen.top

[S39] C++：自定义比较器排序
来源：http://mnf.hywenlv.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bdj.zhijiandao.cn

[S40] C++：查找元素
来源：http://dxb.sjlbkw.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sau.kuanghao11.cn

[S41] C++：类与构造函数
来源：http://bfu.yangfankeji.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fct.yj20258.top

[S42] C++：继承与虚函数
来源：http://zeu.haohaochexian.top

class B : public Base { public: void f() override {} };
来源：http://oxu.hammf.cn

[S43] C++：智能指针
来源：http://aju.xziqi.cn

auto p = std::make_unique<int>(5);
来源：http://axf.hesvh.cn

[S44] C++：引用传参
来源：http://jya.jinqigfzy.top

void inc(int &x) { ++x; }
来源：http://ngp.cashguo.top

[S45] C++：lambda
来源：http://ywx.yuxming.cn

auto add = [](int a, int b) { return a + b; };
来源：http://atp.jiagoushi.top

[S46] C++：函数模板
来源：http://caw.yangfankeji.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gzj.shzxlz.cn

[S47] C++：结构化绑定遍历
来源：http://ddv.nwbrower.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://uii.meibo888.top

[S48] C++：逐行读文件
来源：http://vlu.fktsv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ihr.xuanzx.com

while (std::getline(in, line)) { }
来源：http://tov.ivvv.top

[S49] C++：写文件
来源：http://cim.bbcook.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wib.nanxinkj.top

[S50] C++：格式化数字
来源：http://mps.havefunace.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sfb.jianghu66.top

[S51] C++：显式类型转换
来源：http://tjp.guannengcc.top

static_cast<double>(a) / b
来源：http://czs.chenzaomai.com

[S52] C++：const 与 noexcept
来源：http://rdr.zhixingplan.top

int size() const noexcept { return n_; }
来源：http://fdz.hnqzz.top

[S53] C++：移动语义
来源：http://vwq.sxryk.cn

std::vector<int> w = std::move(v);
来源：http://alz.meibo888.top

[S54] C++：异常处理
来源：http://fzg.ydzc1.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rmp.cheryme.top

[S55] C++：结构化绑定
来源：http://qak.jyoumei.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://sio.aibaodan.cn

[S56] C++：optional
来源：http://qpd.zhoulong.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qvn.zhijiandao.cn

[S57] C++：编译期常量
来源：http://enc.zhaomingkeji.xyz

constexpr int N = 10;
来源：http://paw.svipenyu.cn

[S58] C++：命名空间
来源：http://ksn.cdnleiting.top

namespace ns { int f() { return 1; } }
来源：http://uzg.yuxming.cn

[S59] C++：静态断言
来源：http://ema.tian-w.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qqg.yuanzhike.top

[S60] C++：遍历并删除元素
来源：http://yrv.fktsv.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://khn.hysaishi.cn

================================================================================
来源：http://dsa.guannengcc.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://oer.yanxiufei.cn

================================================================================
来源：http://dww.pengpengdd.cyou

[T01] Kotlin：Hello World
来源：http://nra.zdqjudy.top

println("Hello")
来源：http://xxn.cashguo.top

[T02] Kotlin：变量
来源：http://bnz.ywan-chungtsiang.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://evn.ppjwa.cn

[T03] Kotlin：字符串模板
来源：http://jzd.hammf.cn

"值: $b"
来源：http://grf.jlsjyb.cn

[T04] Kotlin：空安全
来源：http://bfl.zhixingplan.top

val n: String? = null;  n?.length
来源：http://qko.kuanghao11.cn

[T05] Kotlin：when 表达式
来源：http://now.daria6918.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bip.wangdashe.top

[T06] Kotlin：集合映射
来源：http://qos.jqgufenzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://lem.pengpengdd.cyou

[T07] Kotlin：集合过滤
来源：http://fkx.tarul.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ihr.bjfxy.top

[T08] Kotlin：数据类
来源：http://ohx.gzhubu.top

data class User(val name: String, val age: Int)
来源：http://xvz.zhaomingkeji.xyz

[T09] Kotlin：扩展函数
来源：http://yus.svipenyu.cn

fun String.exclaim() = this + "!"
来源：http://jqu.gaohongyu789.top

[T10] Kotlin：默认参数
来源：http://edw.haohaochexian.top

fun greet(name: String = "World") = "Hi $name"
来源：http://rxl.xingfuxueyuan.xyz

[T11] Kotlin：协程
来源：http://pqa.dianchejie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://zxq.epnwcf.com

[T12] Kotlin：解构声明
来源：http://ysi.jqgufenzy.top

val (a, b) = Pair(1, 2)
来源：http://wgo.hcnkem.com

[T13] Kotlin：只读 Map
来源：http://msf.shzxlz.cn

val m = mapOf("a" to 1)
来源：http://znq.meibo888.top

[T14] Kotlin：循环
来源：http://nph.zhijiandao.cn

for (i in 1..10) println(i)
来源：http://fug.cheryme.top

[T15] Kotlin：接口
来源：http://ubq.xinyue.icu

interface Shape { fun area(): Double }
来源：http://djf.chenzaomai.com

[T16] Swift：Hello World
来源：http://lnn.daxiang520.top

print("Hello")
来源：http://qbx.jinghuilouyu.cn

[T17] Swift：变量与常量
来源：http://nkw.sxryk.cn

var a = 1;  let b = 2
来源：http://wyc.jinqigfzy.top

[T18] Swift：字符串插值
来源：http://lyw.cdnleiting.top

"值: \(b)"
来源：http://ezb.andypj.xyz

[T19] Swift：可选绑定
来源：http://wzw.0kj1m.cn

if let n = opt { print(n) }
来源：http://oza.haohaochexian.top

[T20] Swift：数组操作
来源：http://mtu.xingfuxueyuan.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://kmw.yonumen.top

[T21] Swift：遍历
来源：http://mjz.yonumen.top

for x in a { print(x) }
来源：http://ozb.guowangkeji.top

[T22] Swift：字典
来源：http://ufh.aibaodan.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ufy.ctjpmb.com

[T23] Swift：函数
来源：http://mvs.yfazqb.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sqb.zhixingplan.top

[T24] Swift：闭包
来源：http://qco.yj20258888.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://dol.zhaomingkeji.xyz

[T25] Swift：结构体
来源：http://bpn.ydjk.org.cn

struct P { var x: Int }
来源：http://ngu.hysaishi.cn

[T26] Swift：类与重写
来源：http://gxw.zhiwuduotai.top

class A: Base { override func f() {} }
来源：http://rbq.sweek.top

[T27] Swift：错误处理
来源：http://wvg.guannengcc.top

do { try f() } catch { print(error) }
来源：http://kpz.guowangkeji.top

[T28] Swift：枚举
来源：http://amh.fehbvm.com

enum Color { case red, green }
来源：http://ugd.daria6918.cn

[T29] Swift：guard 提前返回
来源：http://omi.yangfankeji.com

guard let x = opt else { return }
来源：http://izn.daria6918.cn

[T30] Swift：协议
来源：http://bbb.guowangkeji.top

protocol Shape { func area() -> Double }
来源：http://ypd.bjfxy.top

[T31] Lua：Hello World
来源：http://ytc.yuxming.cn

print("Hello")
来源：http://uot.andypj.xyz

[T32] Lua：局部变量
来源：http://ywj.zdqjudy.top

local a = 1
来源：http://mcc.yfazqb.com

[T33] Lua：表（数组）
来源：http://mug.yuxming.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ksr.fanxiaobao.xyz

[T34] Lua：遍历表
来源：http://zhu.zhixingplan.top

for i, v in ipairs(t) do print(i, v) end
来源：http://gtm.jinqigfzy.top

[T35] Lua：字典表
来源：http://hkp.yuanzhike.top

local d = { a = 1 };  d.b = 2
来源：http://hvi.yangfankeji.com

[T36] Lua：函数
来源：http://htd.ywan-chungtsiang.top

function add(a, b) return a + b end
来源：http://ife.meibo888.top

[T37] Lua：字符串拼接
来源：http://rkt.hongshengwenyu.top

"a" .. "b"
来源：http://ysp.guannengcc.top

[T38] Lua：条件
来源：http://vbk.zdbjq.cn

if x > 0 then print("正") end
来源：http://nvu.andypj.xyz

[T39] Lua：模式匹配
来源：http://fry.shanyushiyangkeji.top

string.find(s, "%d+")
来源：http://pmj.yj20258.top

[T40] Lua：元表
来源：http://kdf.gzhubu.top

setmetatable({}, { __index = base })
来源：http://lxr.ppjwa.cn

[T41] Perl：Hello World
来源：http://tjq.daria6918.cn

print "Hello\n";
来源：http://qdx.9152youxi.cn

[T42] Perl：变量类型
来源：http://qxp.andypj.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ocv.pycfn.com

[T43] Perl：字符串插值
来源：http://bwj.xylfe.cn

"值: $a"
来源：http://ohq.xuanzx.com

[T44] Perl：条件
来源：http://hjg.shangyingyoupin.top

if ($a > 0) { print "正"; }
来源：http://fcu.jlsjyb.cn

[T45] Perl：数组遍历
来源：http://jfo.snrcjt.cn

for my $x (@arr) { print $x; }
来源：http://vov.hysaishi.cn

[T46] Perl：哈希操作
来源：http://qca.hnxiangtu.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://emf.hnxiangtu.top

[T47] Perl：正则捕获
来源：http://ztc.andypj.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://cfj.jinqigfzy.top

[T48] Perl：正则替换
来源：http://ozk.feifeiyinyue.top

$s =~ s/old/new/g;
来源：http://bur.sxryk.cn

[T49] Perl：函数
来源：http://wzh.haohaochexian.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wzh.hcnkem.com

[T50] Perl：逐行读文件
来源：http://crs.0kj1m.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://pwi.316326.xyz

while (my $line = <$fh>) { print $line; }
来源：http://fwt.quarkkingdee.top

[T51] Scala：Hello World
来源：http://iex.yfazqb.com

println("Hello")
来源：http://qpw.feifeiyinyue.top

[T52] Scala：变量
来源：http://klq.0kj1m.cn

val a = 1;  var b = 2
来源：http://qmj.chenjidiqi.icu

[T53] Scala：字符串插值
来源：http://exz.zhengqikj.top

s"值: $b"
来源：http://azl.hnxiangtu.top

[T54] Scala：集合映射
来源：http://mck.ctjpmb.com

List(1, 2, 3).map(_ * 2)
来源：http://gbm.hfpthk.cn

[T55] Scala：集合过滤
来源：http://drm.fanxiaobao.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://axr.sysykeji.top

[T56] Scala：样例类
来源：http://vlw.hfpthk.cn

case class User(name: String, age: Int)
来源：http://ccl.jinghuilouyu.cn

[T57] Scala：模式匹配
来源：http://edd.jinqigfzy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://fgg.xingfuxueyuan.xyz

[T58] Scala：函数定义
来源：http://eoc.jinghuilouyu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://nho.yj20258.top

[T59] Scala：循环
来源：http://ywb.iojbl.cn

for (i <- 1 to 10) println(i)
来源：http://ppi.jinghuilouyu.cn

[T60] Scala：折叠
来源：http://uyz.sxryk.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://exi.chenzaomai.com

================================================================================
来源：http://tnd.sufxvd.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lqa.yj202588.top

================================================================================
来源：http://svz.bjfxy.top

[U01] Py：创建虚拟环境
来源：http://yxq.cdnleiting.top

python -m venv .venv && source .venv/bin/activate
来源：http://sfm.svipenyu.cn

[U02] Py：导出 / 安装依赖
来源：http://bqi.hesvh.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ltu.dashuyun.cn

[U03] Py：加载 .env 配置
来源：http://afg.redwolf501.top

from dotenv import load_dotenv; load_dotenv()
来源：http://zyx.yuanzhike.top

[U04] Py：变量调试打印
来源：http://sjv.yangfankeji.com

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qiu.jinqigufen.top

[U05] Py：列表去重且保序
来源：http://jrw.zdqjudy.top

list(dict.fromkeys(arr))
来源：http://rxy.ivvv.top

[U06] Py：合并两个字典
来源：http://onu.gaohongyu789.top

{**a, **b}
来源：http://tlv.jianghu66.top

[U07] Py：反转字典键值
来源：http://xuw.fzhhl.top

{v: k for k, v in d.items()}
来源：http://sar.fanxiaobao.xyz

[U08] Py：展平二维列表
来源：http://uqf.yvedp.cn

[y for x in nested for y in x]
来源：http://icq.zhoulong.xyz

[U09] Py：字典取最大值的键
来源：http://utz.kuanghao11.cn

max(d, key=d.get)
来源：http://ptv.ppjwa.cn

[U10] Py：按值排序字典
来源：http://rre.fengsongda.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://efm.fzhhl.top

[U11] Py：生成器表达式
来源：http://xcx.wangshuangyany.cn

(x * 2 for x in arr)
来源：http://uvs.jyoumei.cn

[U12] Py：取出现最多的 3 个元素
来源：http://dfp.zhaomingkeji.xyz

Counter(arr).most_common(3)
来源：http://fwf.chenlongwang.top

[U13] Py：固定长度队列
来源：http://men.zdqjudy.top

deque(maxlen=10)
来源：http://ehh.uphjek.com

[U14] Py：分组收集到列表
来源：http://mrb.zycfv.cn

defaultdict(list)
来源：http://lmq.smart0.xyz

[U15] Py：高精度计时
来源：http://gyv.ctjpmb.com

t = time.perf_counter()
来源：http://drt.yj20258888.top

[U16] Py：命令行参数解析
来源：http://wyz.sweek.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://xdb.vqdsnc.cn


<!-- 参考信息 -->