代发 wailian999

split -l 1000 big.log part_
来源：http://jgx.kuanghao11.cn

[R74] 批量重命名
来源：http://sua.zhengqikj.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vud.zhengqikj.top

[R75] 导出环境变量
来源：http://gye.cdnleiting.top

export PATH="$HOME/bin:$PATH"
来源：http://drv.gotoacloud.top

[R76] 使用临时文件
来源：http://rre.hammf.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jhq.pycfn.com

[R77] 读取用户输入
来源：http://dyu.shuidangran.top

read -rp "请输入: " ans
来源：http://hbz.chenzaomai.com

[R78] 交互式菜单
来源：http://edm.jyoumei.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://cfz.0kj1m.cn

[R79] 解析命令行选项
来源：http://tlj.meibo888.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tky.cucudq.cn

[R80] 查看脚本执行耗时
来源：http://eqa.gzhubu.top

time ./run.sh
来源：http://wff.zhixingplan.top

================================================================================
来源：http://mbb.hywenlv.cn

S. C / C++ 专题
来源：http://gez.jinyuanbaomall.cn

================================================================================
来源：http://nss.fktsv.cn

[S01] C：Hello World
来源：http://yic.fehbvm.com

#include <stdio.h>
来源：http://fol.uphjek.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://xri.zdqjudy.top

[S02] C：变量与格式化输出
来源：http://ypj.tanke756.top

int a = 10; printf("%d\n", a);
来源：http://iov.zhiwuduotai.top

[S03] C：读入整数
来源：http://rpj.hesvh.cn

int x; scanf("%d", &x);
来源：http://erq.iojbl.cn

[S04] C：字符串复制
来源：http://mwx.316326.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://qwd.haohaochexian.top

[S05] C：字符串长度
来源：http://wmg.dashuyun.cn

strlen(s)
来源：http://frg.ydzc1.top

[S06] C：字符串比较
来源：http://fce.cdnleiting.top

strcmp(a, b) == 0
来源：http://yoi.hcnkem.com

[S07] C：数组遍历求和
来源：http://wve.jlsjyb.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qab.pycfn.com

[S08] C：动态内存分配与释放
来源：http://rae.tianlin.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bwu.bbcook.cn

[S09] C：结构体定义与初始化
来源：http://ein.ydjk.org.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mar.zhengqikj.top

[S10] C：指针与解引用
来源：http://sjz.zhongyouzk.top

int *p = &a;  *p = 5;
来源：http://skf.uphjek.com

[S11] C：逐行读文件
来源：http://lxr.dashuyun.cn

FILE *f = fopen("a.txt", "r");
来源：http://svv.jlsjyb.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zwg.cashguo.top

fclose(f);
来源：http://mcn.ybcxt.top

[S12] C：写文件
来源：http://szr.bjfxy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bkw.jinqigfzy.top

[S13] C：宏定义
来源：http://pfk.pengpengdd.cyou

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ztq.yfazqb.com

[S14] C：枚举
来源：http://deb.mhx1999.top

enum Color { RED, GREEN, BLUE };
来源：http://mps.feifeiyinyue.top

[S15] C：类型转换
来源：http://jxz.cdnleiting.top

(double) a / b
来源：http://chs.snrcjt.cn

[S16] C：位操作置位
来源：http://lwf.fzhhl.top

x |= (1 << 3);
来源：http://aqu.jinghuilouyu.cn

[S17] C：安全拼接字符串
来源：http://idw.zdbjq.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wgp.hnxiangtu.top

[S18] C：命令行参数
来源：http://jey.tian-w.cn

int main(int argc, char **argv)
来源：http://jpd.fktsv.cn

[S19] C：快速排序
来源：http://lrj.fanxiaobao.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://bzv.dashuyun.cn

[S20] C：二分查找
来源：http://hpc.zdbjq.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nhl.shuidangran.top

[S21] C：字符类别判断
来源：http://flg.tianlin.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rpu.zhijiandao.cn

[S22] C：字符串转数字
来源：http://oqi.snrcjt.cn

atoi("42");  strtod("3.14", NULL);
来源：http://gxw.yj20258.top

[S23] C：随机数
来源：http://ekr.cheryme.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ujc.jianghu66.top

[S24] C：获取本地时间
来源：http://way.fanxiaobao.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fbi.smart0.xyz

[S25] C：内存拷贝
来源：http://tyt.pengpengdd.cyou

memcpy(dst, src, n);
来源：http://wwt.ppjwa.cn

[S26] C：内存清零
来源：http://dal.zycfv.cn

memset(a, 0, sizeof a);
来源：http://ykm.hfpthk.cn

[S27] C：定义常量
来源：http://jdu.zhengqikj.top

const double PI = 3.14159;
来源：http://nou.nwbrower.top

[S28] C：静态变量
来源：http://wgb.shanyushiyangkeji.top

static int counter = 0;
来源：http://mty.shangyingyoupin.top

[S29] C：变参函数
来源：http://fmq.cdnleiting.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bcp.52xcode.cn

[S30] C：头文件保护
来源：http://xag.zhoulong.xyz

#ifndef X_H
来源：http://pmw.gotoacloud.top

#define X_H
来源：http://oaa.snrcjt.cn

#endif
来源：http://ise.vehdjk.com

[S31] C++：Hello World
来源：http://qtw.yj202588.top

#include <iostream>
来源：http://mcr.hongshengwenyu.top

int main() { std::cout << "Hello\n"; }
来源：http://hjm.shanyushiyangtech.top

[S32] C++：字符串
来源：http://ttx.zhiwuduotai.top

std::string s = "hi";  s += "!";
来源：http://atn.chenlongwang.top

[S33] C++：vector 增删
来源：http://wsy.epnwcf.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nlm.ivvv.top

[S34] C++：遍历 vector
来源：http://ukv.aibaodan.cn

for (auto &x : v) { std::cout << x; }
来源：http://miy.sysykeji.top

[S35] C++：map
来源：http://sav.0kj1m.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://neh.ybcxt.top

[S36] C++：unordered_map
来源：http://xhi.zhiwuduotai.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zjh.tian-w.cn

[S37] C++：set
来源：http://clv.daxiang520.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dye.feifeiyinyue.top

[S38] C++：排序
来源：http://zne.chenjidiqi.icu

std::sort(v.begin(), v.end());
来源：http://ejt.yj202588.top

[S39] C++：自定义比较器排序
来源：http://ckg.fengsongda.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gjo.ehwqpu.com

[S40] C++：查找元素
来源：http://waz.xingfuxueyuan.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://obe.sweek.top

[S41] C++：类与构造函数
来源：http://oyw.dashuyun.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sat.quarkkingdee.top

[S42] C++：继承与虚函数
来源：http://fpk.zycfv.cn

class B : public Base { public: void f() override {} };
来源：http://pbf.jiagoushi.top

[S43] C++：智能指针
来源：http://ptp.yanxiufei.cn

auto p = std::make_unique<int>(5);
来源：http://bmp.ctjpmb.com

[S44] C++：引用传参
来源：http://alr.meibo888.top

void inc(int &x) { ++x; }
来源：http://rmm.snrcjt.cn

[S45] C++：lambda
来源：http://qrb.jiagoushi.top

auto add = [](int a, int b) { return a + b; };
来源：http://iuv.ywan-chungtsiang.top

[S46] C++：函数模板
来源：http://byy.wangdashe.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kon.nwbrower.top

[S47] C++：结构化绑定遍历
来源：http://qhk.jinghuilouyu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zjo.xinyue.icu

[S48] C++：逐行读文件
来源：http://asa.jyoumei.cn

std::ifstream in("a.txt");  std::string line;
来源：http://szh.wangdashe.top

while (std::getline(in, line)) { }
来源：http://nfi.quarkkingdee.top

[S49] C++：写文件
来源：http://kuz.sjlbkw.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xfs.feifeiyinyue.top

[S50] C++：格式化数字
来源：http://wzj.vqdsnc.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sju.andypj.xyz

[S51] C++：显式类型转换
来源：http://qub.ydjk.org.cn

static_cast<double>(a) / b
来源：http://wfo.wangshuangyany.cn

[S52] C++：const 与 noexcept
来源：http://nwv.haohaochexian.top

int size() const noexcept { return n_; }
来源：http://iqk.xylfe.cn

[S53] C++：移动语义
来源：http://ecn.yanxiufei.cn

std::vector<int> w = std::move(v);
来源：http://xou.dashuyun.cn

[S54] C++：异常处理
来源：http://lnv.jqgfzy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://odx.zhongyouzk.top

[S55] C++：结构化绑定
来源：http://xmu.zhiwuduotai.top

auto [a, b] = std::make_pair(1, 2);
来源：http://flo.yj20258888.top

[S56] C++：optional
来源：http://vek.316326.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nmn.pycfn.com

[S57] C++：编译期常量
来源：http://ixd.meibo888.top

constexpr int N = 10;
来源：http://ztu.feifeiyinyue.top

[S58] C++：命名空间
来源：http://rxk.epnwcf.com

namespace ns { int f() { return 1; } }
来源：http://akl.vehdjk.com

[S59] C++：静态断言
来源：http://qyg.chenzaomai.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xuz.yj20258888.top

[S60] C++：遍历并删除元素
来源：http://cqt.jyoumei.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mpy.ppjwa.cn

================================================================================
来源：http://taq.52xcode.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tae.wangshuangyany.cn

================================================================================
来源：http://yrf.hammf.cn

[T01] Kotlin：Hello World
来源：http://nfi.quarkkingdee.top

println("Hello")
来源：http://lpj.sweek.top

[T02] Kotlin：变量
来源：http://ejx.feifeiyinyue.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jhp.fanxiaobao.xyz

[T03] Kotlin：字符串模板
来源：http://gos.shzxlz.cn

"值: $b"
来源：http://pzp.chenzaomai.com

[T04] Kotlin：空安全
来源：http://xcy.zhijiandao.cn

val n: String? = null;  n?.length
来源：http://czg.sufxvd.cn

[T05] Kotlin：when 表达式
来源：http://iya.ydjk.org.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yvh.yuanzhike.top

[T06] Kotlin：集合映射
来源：http://zne.pengpengdd.cyou

listOf(1, 2, 3).map { it * 2 }
来源：http://pxb.guannengcc.top

[T07] Kotlin：集合过滤
来源：http://ocy.aizwys.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://mfp.yanxiufei.cn

[T08] Kotlin：数据类
来源：http://rmv.pengpengdd.cyou

data class User(val name: String, val age: Int)
来源：http://fhe.fehbvm.com

[T09] Kotlin：扩展函数
来源：http://wvm.jyoumei.cn

fun String.exclaim() = this + "!"
来源：http://wvs.sxryk.cn

[T10] Kotlin：默认参数
来源：http://ogx.xylfe.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://eip.zhongyouzk.top

[T11] Kotlin：协程
来源：http://zwp.pycfn.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://mcs.xinyue.icu

[T12] Kotlin：解构声明
来源：http://zte.0kj1m.cn

val (a, b) = Pair(1, 2)
来源：http://vwc.shanyushiyangtech.top

[T13] Kotlin：只读 Map
来源：http://nds.fehbvm.com

val m = mapOf("a" to 1)
来源：http://ktr.zhijiandao.cn

[T14] Kotlin：循环
来源：http://mcq.wangdashe.top

for (i in 1..10) println(i)
来源：http://ent.hysaishi.cn

[T15] Kotlin：接口
来源：http://qeu.ppjwa.cn

interface Shape { fun area(): Double }
来源：http://pdk.guannengcc.top

[T16] Swift：Hello World
来源：http://pcc.hcnkem.com

print("Hello")
来源：http://wmu.iojbl.cn

[T17] Swift：变量与常量
来源：http://nto.wangdashe.top

var a = 1;  let b = 2
来源：http://tql.sxryk.cn

[T18] Swift：字符串插值
来源：http://wyo.hfpthk.cn

"值: \(b)"
来源：http://tii.wangdashe.top

[T19] Swift：可选绑定
来源：http://xya.havefunace.top

if let n = opt { print(n) }
来源：http://dcv.zdqjudy.top

[T20] Swift：数组操作
来源：http://pfm.yvedp.cn

var a = [1, 2, 3];  a.append(4)
来源：http://lgl.jinyuanbaomall.cn

[T21] Swift：遍历
来源：http://dyq.hnxiangtu.top

for x in a { print(x) }
来源：http://chg.jinyuanbaomall.cn

[T22] Swift：字典
来源：http://fjz.gotoacloud.top

var d = ["a": 1];  d["b"] = 2
来源：http://clh.fktsv.cn

[T23] Swift：函数
来源：http://wuo.wangshuangyany.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vrb.zdqjudy.top

[T24] Swift：闭包
来源：http://hdy.jinqigfzy.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://bhj.yuanzhike.top

[T25] Swift：结构体
来源：http://nsm.yj202588.top

struct P { var x: Int }
来源：http://mkb.daxiang520.top

[T26] Swift：类与重写
来源：http://zus.jinqigufen.top

class A: Base { override func f() {} }
来源：http://fng.shuidangran.top

[T27] Swift：错误处理
来源：http://gch.yj20258888.top

do { try f() } catch { print(error) }
来源：http://kyt.zhijiandao.cn

[T28] Swift：枚举
来源：http://yej.yonumen.top

enum Color { case red, green }
来源：http://iua.xziqi.cn

[T29] Swift：guard 提前返回
来源：http://yfc.sufxvd.cn

guard let x = opt else { return }
来源：http://xty.zdbjq.cn

[T30] Swift：协议
来源：http://pff.sjlbkw.cn

protocol Shape { func area() -> Double }
来源：http://vvx.feifeiyinyue.top

[T31] Lua：Hello World
来源：http://jdl.hammf.cn

print("Hello")
来源：http://mfd.meibo888.top

[T32] Lua：局部变量
来源：http://oyr.fanxiaobao.xyz

local a = 1
来源：http://mbx.tian-w.cn

[T33] Lua：表（数组）
来源：http://pnt.tanke756.top

local t = {1, 2, 3};  t[4] = 4
来源：http://yqv.shuidangran.top

[T34] Lua：遍历表
来源：http://vxl.aibaodan.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qia.quarkkingdee.top

[T35] Lua：字典表
来源：http://zqd.xuanzx.com

local d = { a = 1 };  d.b = 2
来源：http://pod.yanxiufei.cn

[T36] Lua：函数
来源：http://dkj.gaohongyu789.top

function add(a, b) return a + b end
来源：http://gxu.ydzc1.top

[T37] Lua：字符串拼接
来源：http://lch.uphjek.com

"a" .. "b"
来源：http://tuh.chenjidiqi.icu

[T38] Lua：条件
来源：http://xdp.jianghu66.top

if x > 0 then print("正") end
来源：http://gvj.shangyingyoupin.top

[T39] Lua：模式匹配
来源：http://fzg.cdnleiting.top

string.find(s, "%d+")
来源：http://lrd.birdmap.top

[T40] Lua：元表
来源：http://fjl.guannengcc.top

setmetatable({}, { __index = base })
来源：http://vkg.jinqigufen.top

[T41] Perl：Hello World
来源：http://dji.ydzc1.top

print "Hello\n";
来源：http://nao.yanxiufei.cn

[T42] Perl：变量类型
来源：http://xqh.hnxiangtu.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tvi.vehdjk.com

[T43] Perl：字符串插值
来源：http://orn.havefunace.top

"值: $a"
来源：http://yny.snrcjt.cn

[T44] Perl：条件
来源：http://qup.shzxlz.cn

if ($a > 0) { print "正"; }
来源：http://tzu.jianghu66.top

[T45] Perl：数组遍历
来源：http://lqi.cucudq.cn

for my $x (@arr) { print $x; }
来源：http://cwb.daxiang520.top

[T46] Perl：哈希操作
来源：http://pyt.yuanzhike.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://irt.sxryk.cn

[T47] Perl：正则捕获
来源：http://bau.jinqigfzy.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://waw.tanke756.top

[T48] Perl：正则替换
来源：http://uoz.pengpengdd.cyou

$s =~ s/old/new/g;
来源：http://lxo.fehbvm.com

[T49] Perl：函数
来源：http://thr.sweek.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://idz.redwolf501.top

[T50] Perl：逐行读文件
来源：http://xbw.zhiwuduotai.top

open my $fh, "<", "a.txt" or die $!;
来源：http://jae.yonumen.top

while (my $line = <$fh>) { print $line; }
来源：http://jwn.feifeiyinyue.top

[T51] Scala：Hello World
来源：http://vkj.dianchejie.cn

println("Hello")
来源：http://oho.nanxinkj.top

[T52] Scala：变量
来源：http://btv.ehwqpu.com

val a = 1;  var b = 2
来源：http://pew.nanxuanxn.top

[T53] Scala：字符串插值
来源：http://cno.fktsv.cn

s"值: $b"
来源：http://sai.yongpay.top

[T54] Scala：集合映射
来源：http://qll.ppjwa.cn

List(1, 2, 3).map(_ * 2)
来源：http://ejf.shangyingyoupin.top

[T55] Scala：集合过滤
来源：http://nht.zdqjudy.top

List(1, 2, 3).filter(_ > 1)
来源：http://vqs.hongshengwenyu.top

[T56] Scala：样例类
来源：http://xdy.sysykeji.top

case class User(name: String, age: Int)
来源：http://ccn.ywan-chungtsiang.top

[T57] Scala：模式匹配
来源：http://wus.haohaochexian.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://mlc.vqdsnc.cn

[T58] Scala：函数定义
来源：http://tym.ybcxt.top

def add(a: Int, b: Int): Int = a + b
来源：http://rtc.jinyuanbaomall.cn

[T59] Scala：循环
来源：http://fal.shangyingyoupin.top

for (i <- 1 to 10) println(i)
来源：http://cxo.zdqjudy.top

[T60] Scala：折叠
来源：http://zzh.aizwys.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rsn.guowangkeji.top

================================================================================
来源：http://cxp.sufxvd.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vbo.mhx1999.top

================================================================================
来源：http://wbo.yongpay.top

[U01] Py：创建虚拟环境
来源：http://nvs.jiagoushi.top

python -m venv .venv && source .venv/bin/activate
来源：http://fno.shanyushiyangkeji.top

[U02] Py：导出 / 安装依赖
来源：http://guk.nanxuanxn.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mul.shanyushiyangkeji.top

[U03] Py：加载 .env 配置
来源：http://dgo.sufxvd.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://srr.sweek.top

[U04] Py：变量调试打印
来源：http://duc.pengpengdd.cyou

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ale.yueranfly.top

[U05] Py：列表去重且保序
来源：http://iqq.yj20258888.top

list(dict.fromkeys(arr))
来源：http://lre.shuidangran.top

[U06] Py：合并两个字典
来源：http://gtc.zhengqikj.top

{**a, **b}
来源：http://tyb.fanxiaobao.xyz

[U07] Py：反转字典键值
来源：http://wpk.jinyuanbaomall.cn

{v: k for k, v in d.items()}
来源：http://mvl.hongshengwenyu.top

[U08] Py：展平二维列表
来源：http://ilv.0kj1m.cn

[y for x in nested for y in x]
来源：http://umg.hywenlv.cn

[U09] Py：字典取最大值的键
来源：http://fmi.guannengcc.top

max(d, key=d.get)
来源：http://aon.chenjidiqi.icu

[U10] Py：按值排序字典
来源：http://oxi.aibaodan.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://nch.9152youxi.cn

[U11] Py：生成器表达式
来源：http://qna.dashuyun.cn

(x * 2 for x in arr)
来源：http://nuv.shangyingyoupin.top

[U12] Py：取出现最多的 3 个元素
来源：http://qdk.zhiwuduotai.top

Counter(arr).most_common(3)
来源：http://skh.gzhubu.top

[U13] Py：固定长度队列
来源：http://vta.yj20258888.top

deque(maxlen=10)
来源：http://iyf.cqqwz.cn

[U14] Py：分组收集到列表
来源：http://ciq.andypj.xyz

defaultdict(list)
来源：http://vrq.shanyushiyangkeji.top


<!-- 参考信息 -->