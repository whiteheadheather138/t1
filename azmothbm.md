代发 wailian999

read -rp "请输入: " ans
来源：http://afx.ydjk.org.cn

[R78] 交互式菜单
来源：http://ckx.hcnkem.com

select opt in a b c; do echo "$opt"; break; done
来源：http://twm.yanxiufei.cn

[R79] 解析命令行选项
来源：http://kbk.ehwqpu.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jev.cdnleiting.top

[R80] 查看脚本执行耗时
来源：http://zil.ywan-chungtsiang.top

time ./run.sh
来源：http://dtv.gaohongyu789.top

================================================================================
来源：http://zyo.cheryme.top

S. C / C++ 专题
来源：http://eba.zycfv.cn

================================================================================
来源：http://rqz.hesvh.cn

[S01] C：Hello World
来源：http://rcy.yuxming.cn

#include <stdio.h>
来源：http://lwh.jiagoushi.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://jzg.fanxiaobao.xyz

[S02] C：变量与格式化输出
来源：http://edc.bbcook.cn

int a = 10; printf("%d\n", a);
来源：http://pxq.zhiwuduotai.top

[S03] C：读入整数
来源：http://ryl.sweek.top

int x; scanf("%d", &x);
来源：http://vbv.cashguo.top

[S04] C：字符串复制
来源：http://klm.zhongyouzk.top

char dst[32]; strcpy(dst, "hi");
来源：http://ncw.xinyue.icu

[S05] C：字符串长度
来源：http://sio.jinqigfzy.top

strlen(s)
来源：http://gom.zhijiandao.cn

[S06] C：字符串比较
来源：http://omq.sxryk.cn

strcmp(a, b) == 0
来源：http://jtd.xingfuxueyuan.xyz

[S07] C：数组遍历求和
来源：http://roj.pycfn.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nue.bbcook.cn

[S08] C：动态内存分配与释放
来源：http://pxb.yanxiufei.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qfc.yj20258.top

[S09] C：结构体定义与初始化
来源：http://yte.316326.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ore.zhixingplan.top

[S10] C：指针与解引用
来源：http://eoj.fanxiaobao.xyz

int *p = &a;  *p = 5;
来源：http://efn.vehdjk.com

[S11] C：逐行读文件
来源：http://zbp.yvedp.cn

FILE *f = fopen("a.txt", "r");
来源：http://ims.tarul.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://pks.epnwcf.com

fclose(f);
来源：http://fpj.yanxiufei.cn

[S12] C：写文件
来源：http://gci.andypj.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zko.9152youxi.cn

[S13] C：宏定义
来源：http://hut.zdqjudy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yep.tanke756.top

[S14] C：枚举
来源：http://cng.jinqigufen.top

enum Color { RED, GREEN, BLUE };
来源：http://jxh.chenzaomai.com

[S15] C：类型转换
来源：http://kjb.sweek.top

(double) a / b
来源：http://uwc.shanyushiyangtech.top

[S16] C：位操作置位
来源：http://ctn.yanxiufei.cn

x |= (1 << 3);
来源：http://yar.fanxiaobao.xyz

[S17] C：安全拼接字符串
来源：http://ele.epnwcf.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qyy.iojbl.cn

[S18] C：命令行参数
来源：http://ekr.chenzaomai.com

int main(int argc, char **argv)
来源：http://tas.kuanghao11.cn

[S19] C：快速排序
来源：http://dzs.jinghuilouyu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://att.fzhhl.top

[S20] C：二分查找
来源：http://hlx.shanyushiyangkeji.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hzn.cdnleiting.top

[S21] C：字符类别判断
来源：http://eox.hnqzz.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tvq.hywenlv.cn

[S22] C：字符串转数字
来源：http://cut.cheryme.top

atoi("42");  strtod("3.14", NULL);
来源：http://siu.vqdsnc.cn

[S23] C：随机数
来源：http://dye.yongpay.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ipf.dashuyun.cn

[S24] C：获取本地时间
来源：http://zax.sjlbkw.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://waa.hongshengwenyu.top

[S25] C：内存拷贝
来源：http://bmu.316326.xyz

memcpy(dst, src, n);
来源：http://khv.shanyushiyangkeji.top

[S26] C：内存清零
来源：http://bur.cashguo.top

memset(a, 0, sizeof a);
来源：http://wym.fktsv.cn

[S27] C：定义常量
来源：http://sat.mhx1999.top

const double PI = 3.14159;
来源：http://nnt.xziqi.cn

[S28] C：静态变量
来源：http://cvr.zdbjq.cn

static int counter = 0;
来源：http://nmr.hcnkem.com

[S29] C：变参函数
来源：http://lus.mhx1999.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dvu.fzhhl.top

[S30] C：头文件保护
来源：http://nbf.yuanzhike.top

#ifndef X_H
来源：http://npo.zhixingplan.top

#define X_H
来源：http://mjl.9152youxi.cn

#endif
来源：http://opl.zhengqikj.top

[S31] C++：Hello World
来源：http://bfm.zhongyouzk.top

#include <iostream>
来源：http://vlw.aizwys.cn

int main() { std::cout << "Hello\n"; }
来源：http://rea.xuanzx.com

[S32] C++：字符串
来源：http://qwj.ywan-chungtsiang.top

std::string s = "hi";  s += "!";
来源：http://yyz.zhijiandao.cn

[S33] C++：vector 增删
来源：http://nii.birdmap.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hnf.ppjwa.cn

[S34] C++：遍历 vector
来源：http://qig.epnwcf.com

for (auto &x : v) { std::cout << x; }
来源：http://rhf.tian-w.cn

[S35] C++：map
来源：http://hqg.316326.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cnr.gzhubu.top

[S36] C++：unordered_map
来源：http://htx.daxiang520.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jng.sxryk.cn

[S37] C++：set
来源：http://rcq.zhaomingkeji.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ict.hcnkem.com

[S38] C++：排序
来源：http://xxi.0kj1m.cn

std::sort(v.begin(), v.end());
来源：http://god.jiagoushi.top

[S39] C++：自定义比较器排序
来源：http://dih.hnqzz.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vvp.ctjpmb.com

[S40] C++：查找元素
来源：http://wmj.zdbjq.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dzh.xinyue.icu

[S41] C++：类与构造函数
来源：http://sll.gzhubu.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tbs.tianlin.xyz

[S42] C++：继承与虚函数
来源：http://yop.zycfv.cn

class B : public Base { public: void f() override {} };
来源：http://pnn.yfazqb.com

[S43] C++：智能指针
来源：http://nxz.aibaodan.cn

auto p = std::make_unique<int>(5);
来源：http://rgp.zhongyouzk.top

[S44] C++：引用传参
来源：http://hte.daxiang520.top

void inc(int &x) { ++x; }
来源：http://wru.aibaodan.cn

[S45] C++：lambda
来源：http://jxf.jinyuanbaomall.cn

auto add = [](int a, int b) { return a + b; };
来源：http://pgt.ydjk.org.cn

[S46] C++：函数模板
来源：http://yhw.yanxiufei.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://whe.yj202588.top

[S47] C++：结构化绑定遍历
来源：http://foo.fzhhl.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sxh.fengsongda.top

[S48] C++：逐行读文件
来源：http://frt.wangshuangyany.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qks.sufxvd.cn

while (std::getline(in, line)) { }
来源：http://enj.hnqzz.top

[S49] C++：写文件
来源：http://dys.fengsongda.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fmy.vqdsnc.cn

[S50] C++：格式化数字
来源：http://qlr.gogol.net.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qaz.jinqigufen.top

[S51] C++：显式类型转换
来源：http://ren.zhoulong.xyz

static_cast<double>(a) / b
来源：http://rlw.xuetiantiany.cn

[S52] C++：const 与 noexcept
来源：http://hhh.daxiang520.top

int size() const noexcept { return n_; }
来源：http://pxj.yj20258.top

[S53] C++：移动语义
来源：http://jyf.guowangkeji.top

std::vector<int> w = std::move(v);
来源：http://ajx.jinghuilouyu.cn

[S54] C++：异常处理
来源：http://rec.zhixingplan.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rgu.ywan-chungtsiang.top

[S55] C++：结构化绑定
来源：http://ipk.shangyingyoupin.top

auto [a, b] = std::make_pair(1, 2);
来源：http://tby.sjlbkw.cn

[S56] C++：optional
来源：http://xzu.tian-w.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://urx.tanke756.top

[S57] C++：编译期常量
来源：http://vsg.redwolf501.top

constexpr int N = 10;
来源：http://gvd.hywenlv.cn

[S58] C++：命名空间
来源：http://bpj.ppjwa.cn

namespace ns { int f() { return 1; } }
来源：http://lif.zhijiandao.cn

[S59] C++：静态断言
来源：http://ucu.bbcook.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kra.havefunace.top

[S60] C++：遍历并删除元素
来源：http://qmp.chenlongwang.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://uhc.fktsv.cn

================================================================================
来源：http://qvu.cqqwz.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pwo.9152youxi.cn

================================================================================
来源：http://tmf.yonumen.top

[T01] Kotlin：Hello World
来源：http://elp.ehwqpu.com

println("Hello")
来源：http://rol.haohaochexian.top

[T02] Kotlin：变量
来源：http://ifd.zhiwuduotai.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jva.shanyushiyangkeji.top

[T03] Kotlin：字符串模板
来源：http://zvb.zhongyouzk.top

"值: $b"
来源：http://oor.zycfv.cn

[T04] Kotlin：空安全
来源：http://ouh.smart0.xyz

val n: String? = null;  n?.length
来源：http://fde.iojbl.cn

[T05] Kotlin：when 表达式
来源：http://gfa.cashguo.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kpe.kuanghao11.cn

[T06] Kotlin：集合映射
来源：http://yaw.sweek.top

listOf(1, 2, 3).map { it * 2 }
来源：http://xgf.jlsjyb.cn

[T07] Kotlin：集合过滤
来源：http://jeh.cashguo.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://yum.cashguo.top

[T08] Kotlin：数据类
来源：http://njv.yangfankeji.com

data class User(val name: String, val age: Int)
来源：http://fgi.sysykeji.top

[T09] Kotlin：扩展函数
来源：http://tce.jinqigufen.top

fun String.exclaim() = this + "!"
来源：http://rlq.ehwqpu.com

[T10] Kotlin：默认参数
来源：http://kad.chenjidiqi.icu

fun greet(name: String = "World") = "Hi $name"
来源：http://dzk.fktsv.cn

[T11] Kotlin：协程
来源：http://eoo.xingfuxueyuan.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://oby.yvedp.cn

[T12] Kotlin：解构声明
来源：http://huy.xuetiantiany.cn

val (a, b) = Pair(1, 2)
来源：http://vzo.smart0.xyz

[T13] Kotlin：只读 Map
来源：http://qiv.bjfxy.top

val m = mapOf("a" to 1)
来源：http://lfa.yueranfly.top

[T14] Kotlin：循环
来源：http://obn.fktsv.cn

for (i in 1..10) println(i)
来源：http://wlq.chenzaomai.com

[T15] Kotlin：接口
来源：http://gyl.haohaochexian.top

interface Shape { fun area(): Double }
来源：http://bit.ybcxt.top

[T16] Swift：Hello World
来源：http://bno.uphjek.com

print("Hello")
来源：http://eea.redwolf501.top

[T17] Swift：变量与常量
来源：http://wwk.fengsongda.top

var a = 1;  let b = 2
来源：http://fyc.zhaomingkeji.xyz

[T18] Swift：字符串插值
来源：http://tub.ehwqpu.com

"值: \(b)"
来源：http://qhl.shzxlz.cn

[T19] Swift：可选绑定
来源：http://ktq.havefunace.top

if let n = opt { print(n) }
来源：http://elc.sysykeji.top

[T20] Swift：数组操作
来源：http://osw.xziqi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://msp.ivvv.top

[T21] Swift：遍历
来源：http://ikl.epnwcf.com

for x in a { print(x) }
来源：http://jse.snrcjt.cn

[T22] Swift：字典
来源：http://igf.hywenlv.cn

var d = ["a": 1];  d["b"] = 2
来源：http://shp.hesvh.cn

[T23] Swift：函数
来源：http://xyz.zycfv.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hut.yonumen.top

[T24] Swift：闭包
来源：http://xns.zdbjq.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zhs.shzxlz.cn

[T25] Swift：结构体
来源：http://elp.tian-w.cn

struct P { var x: Int }
来源：http://xsn.hammf.cn

[T26] Swift：类与重写
来源：http://zzz.vqdsnc.cn

class A: Base { override func f() {} }
来源：http://uci.shuidangran.top

[T27] Swift：错误处理
来源：http://elb.bjfxy.top

do { try f() } catch { print(error) }
来源：http://bah.zhoulong.xyz

[T28] Swift：枚举
来源：http://oql.sysykeji.top

enum Color { case red, green }
来源：http://lvt.xingfuxueyuan.xyz

[T29] Swift：guard 提前返回
来源：http://ykd.mhx1999.top

guard let x = opt else { return }
来源：http://skn.bjfxy.top

[T30] Swift：协议
来源：http://qeu.havefunace.top

protocol Shape { func area() -> Double }
来源：http://ajm.zdqjudy.top

[T31] Lua：Hello World
来源：http://pyf.fzhhl.top

print("Hello")
来源：http://qfd.hongshengwenyu.top

[T32] Lua：局部变量
来源：http://mpp.jyoumei.cn

local a = 1
来源：http://wlc.xuetiantiany.cn

[T33] Lua：表（数组）
来源：http://rvr.cheryme.top

local t = {1, 2, 3};  t[4] = 4
来源：http://tkh.jqgufenzy.top

[T34] Lua：遍历表
来源：http://bph.yj20258.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ltz.ppjwa.cn

[T35] Lua：字典表
来源：http://our.vqdsnc.cn

local d = { a = 1 };  d.b = 2
来源：http://oeq.shangyingyoupin.top

[T36] Lua：函数
来源：http://xgb.hnqzz.top

function add(a, b) return a + b end
来源：http://zgq.gotoacloud.top

[T37] Lua：字符串拼接
来源：http://noo.xziqi.cn

"a" .. "b"
来源：http://pgk.mhx1999.top

[T38] Lua：条件
来源：http://jui.cucudq.cn

if x > 0 then print("正") end
来源：http://svt.yongpay.top

[T39] Lua：模式匹配
来源：http://fii.uphjek.com

string.find(s, "%d+")
来源：http://ntj.hnqzz.top

[T40] Lua：元表
来源：http://uid.shanyushiyangkeji.top

setmetatable({}, { __index = base })
来源：http://sic.shzxlz.cn

[T41] Perl：Hello World
来源：http://iwq.hywenlv.cn

print "Hello\n";
来源：http://yxm.fehbvm.com

[T42] Perl：变量类型
来源：http://woz.52xcode.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dku.yangfankeji.com

[T43] Perl：字符串插值
来源：http://vdi.ehwqpu.com

"值: $a"
来源：http://gqc.redwolf501.top

[T44] Perl：条件
来源：http://vwv.quarkkingdee.top

if ($a > 0) { print "正"; }
来源：http://yom.aizwys.cn

[T45] Perl：数组遍历
来源：http://nab.nwbrower.top

for my $x (@arr) { print $x; }
来源：http://oml.chenjidiqi.icu

[T46] Perl：哈希操作
来源：http://gjx.xziqi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vyn.mhx1999.top

[T47] Perl：正则捕获
来源：http://hlw.yvedp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ssm.yvedp.cn

[T48] Perl：正则替换
来源：http://kcg.ydzc1.top

$s =~ s/old/new/g;
来源：http://vid.jianghu66.top

[T49] Perl：函数
来源：http://tny.cashguo.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wks.jyoumei.cn

[T50] Perl：逐行读文件
来源：http://bji.haohaochexian.top

open my $fh, "<", "a.txt" or die $!;
来源：http://fad.hysaishi.cn

while (my $line = <$fh>) { print $line; }
来源：http://isn.yuxming.cn

[T51] Scala：Hello World
来源：http://ahr.hnxiangtu.top

println("Hello")
来源：http://xax.zhengqikj.top

[T52] Scala：变量
来源：http://til.c1oappe.top

val a = 1;  var b = 2
来源：http://xuk.fanxiaobao.xyz

[T53] Scala：字符串插值
来源：http://dwx.ivvv.top

s"值: $b"
来源：http://dal.cucudq.cn

[T54] Scala：集合映射
来源：http://qsu.yj20258.top

List(1, 2, 3).map(_ * 2)
来源：http://xym.hysaishi.cn

[T55] Scala：集合过滤
来源：http://wlg.jlsjyb.cn

List(1, 2, 3).filter(_ > 1)
来源：http://drz.gzhubu.top

[T56] Scala：样例类
来源：http://fpq.pycfn.com

case class User(name: String, age: Int)
来源：http://gmd.zdqjudy.top

[T57] Scala：模式匹配
来源：http://ysy.cheryme.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://zmp.daxiang520.top

[T58] Scala：函数定义
来源：http://edm.xuetiantiany.cn

def add(a: Int, b: Int): Int = a + b
来源：http://pfy.ywan-chungtsiang.top

[T59] Scala：循环
来源：http://jns.sysykeji.top

for (i <- 1 to 10) println(i)
来源：http://bnm.mhx1999.top

[T60] Scala：折叠
来源：http://ism.uphjek.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qqz.zhoulong.xyz

================================================================================
来源：http://qio.hcnkem.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nhh.ppjwa.cn

================================================================================
来源：http://pqe.chenlongwang.top

[U01] Py：创建虚拟环境
来源：http://ijs.0kj1m.cn

python -m venv .venv && source .venv/bin/activate
来源：http://agg.xingfuxueyuan.xyz

[U02] Py：导出 / 安装依赖
来源：http://arf.yvedp.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gpx.fehbvm.com

[U03] Py：加载 .env 配置
来源：http://zpo.ybcxt.top

from dotenv import load_dotenv; load_dotenv()
来源：http://qgx.kuanghao11.cn

[U04] Py：变量调试打印
来源：http://xhi.bjfxy.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lcp.vqdsnc.cn

[U05] Py：列表去重且保序
来源：http://wqx.jinqigfzy.top

list(dict.fromkeys(arr))
来源：http://vry.ywan-chungtsiang.top

[U06] Py：合并两个字典
来源：http://cqv.wangdashe.top

{**a, **b}
来源：http://vac.kuanghao11.cn

[U07] Py：反转字典键值
来源：http://srz.aizwys.cn

{v: k for k, v in d.items()}
来源：http://zpp.vqdsnc.cn

[U08] Py：展平二维列表
来源：http://nbe.xinyue.icu

[y for x in nested for y in x]
来源：http://zaa.0kj1m.cn

[U09] Py：字典取最大值的键
来源：http://ifk.snrcjt.cn

max(d, key=d.get)
来源：http://oqm.bjfxy.top

[U10] Py：按值排序字典
来源：http://hjh.shuidangran.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fwi.uphjek.com

[U11] Py：生成器表达式
来源：http://zfu.jlsjyb.cn

(x * 2 for x in arr)
来源：http://uot.bbcook.cn

[U12] Py：取出现最多的 3 个元素
来源：http://tzk.bbcook.cn

Counter(arr).most_common(3)
来源：http://xin.dashuyun.cn

[U13] Py：固定长度队列
来源：http://tut.ppjwa.cn

deque(maxlen=10)
来源：http://nhq.zhoulong.xyz

[U14] Py：分组收集到列表
来源：http://mps.pengpengdd.cyou

defaultdict(list)
来源：http://uyd.havefunace.top

[U15] Py：高精度计时
来源：http://wuf.xuanzx.com

t = time.perf_counter()
来源：http://dto.iojbl.cn

[U16] Py：命令行参数解析
来源：http://ciw.yueranfly.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kfj.fktsv.cn

[U17] Py：初始化日志
来源：http://bah.haohaochexian.top

logging.basicConfig(level=logging.INFO)
来源：http://iih.mhx1999.top

[U18] Py：预编译正则
来源：http://ohx.nwbrower.top

pat = re.compile(r"\d+")
来源：http://dfi.vehdjk.com


<!-- 参考信息 -->