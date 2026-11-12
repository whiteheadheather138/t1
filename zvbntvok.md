代发 wailian999

int main(void) { printf("Hello\n"); return 0; }
来源：http://gsy.wangdashe.top

[S02] C：变量与格式化输出
来源：http://toz.zhijiandao.cn

int a = 10; printf("%d\n", a);
来源：http://brj.ybcxt.top

[S03] C：读入整数
来源：http://kre.yonumen.top

int x; scanf("%d", &x);
来源：http://kek.yongpay.top

[S04] C：字符串复制
来源：http://ttq.shzxlz.cn

char dst[32]; strcpy(dst, "hi");
来源：http://lww.tianlin.xyz

[S05] C：字符串长度
来源：http://pwv.yangfankeji.com

strlen(s)
来源：http://hwd.xylfe.cn

[S06] C：字符串比较
来源：http://wai.c1oappe.top

strcmp(a, b) == 0
来源：http://dbw.andypj.xyz

[S07] C：数组遍历求和
来源：http://tgs.jqgfzy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ovu.guowangkeji.top

[S08] C：动态内存分配与释放
来源：http://hnm.cdnleiting.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zyb.sysykeji.top

[S09] C：结构体定义与初始化
来源：http://uil.yanxiufei.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cwe.sjlbkw.cn

[S10] C：指针与解引用
来源：http://qea.yangfankeji.com

int *p = &a;  *p = 5;
来源：http://qxv.feifeiyinyue.top

[S11] C：逐行读文件
来源：http://nei.xuetiantiany.cn

FILE *f = fopen("a.txt", "r");
来源：http://rpe.jinyuanbaomall.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://tez.jinghuilouyu.cn

fclose(f);
来源：http://uns.hongshengwenyu.top

[S12] C：写文件
来源：http://sib.fktsv.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jhy.cqqwz.cn

[S13] C：宏定义
来源：http://yxc.cdnleiting.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xyd.yanxiufei.cn

[S14] C：枚举
来源：http://vnz.feifeiyinyue.top

enum Color { RED, GREEN, BLUE };
来源：http://vit.shuidangran.top

[S15] C：类型转换
来源：http://txv.snrcjt.cn

(double) a / b
来源：http://cod.chenzaomai.com

[S16] C：位操作置位
来源：http://ghl.gotoacloud.top

x |= (1 << 3);
来源：http://sdw.jianghu66.top

[S17] C：安全拼接字符串
来源：http://jty.meibo888.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ars.sweek.top

[S18] C：命令行参数
来源：http://ppf.svipenyu.cn

int main(int argc, char **argv)
来源：http://crn.pycfn.com

[S19] C：快速排序
来源：http://jmo.yangfankeji.com

qsort(a, n, sizeof(int), cmp);
来源：http://brr.zhixingplan.top

[S20] C：二分查找
来源：http://pja.yanxiufei.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://onn.nanxuanxn.top

[S21] C：字符类别判断
来源：http://wxt.uphjek.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hcu.snrcjt.cn

[S22] C：字符串转数字
来源：http://yaj.yanxiufei.cn

atoi("42");  strtod("3.14", NULL);
来源：http://iav.birdmap.top

[S23] C：随机数
来源：http://nlg.daria6918.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fxx.sjlbkw.cn

[S24] C：获取本地时间
来源：http://ada.shanyushiyangkeji.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rha.dianchejie.cn

[S25] C：内存拷贝
来源：http://xrm.vqdsnc.cn

memcpy(dst, src, n);
来源：http://pru.chenjidiqi.icu

[S26] C：内存清零
来源：http://ylx.epnwcf.com

memset(a, 0, sizeof a);
来源：http://yzl.daria6918.cn

[S27] C：定义常量
来源：http://cbw.sweek.top

const double PI = 3.14159;
来源：http://qrj.snrcjt.cn

[S28] C：静态变量
来源：http://hxi.mhx1999.top

static int counter = 0;
来源：http://fmk.nanxuanxn.top

[S29] C：变参函数
来源：http://lyr.birdmap.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lge.zhixingplan.top

[S30] C：头文件保护
来源：http://kfo.fanxiaobao.xyz

#ifndef X_H
来源：http://bzz.iojbl.cn

#define X_H
来源：http://rvm.sysykeji.top

#endif
来源：http://psm.aizwys.cn

[S31] C++：Hello World
来源：http://bwq.zhoulong.xyz

#include <iostream>
来源：http://wup.hcnkem.com

int main() { std::cout << "Hello\n"; }
来源：http://nnq.haohaochexian.top

[S32] C++：字符串
来源：http://xse.zdbjq.cn

std::string s = "hi";  s += "!";
来源：http://hyi.jyoumei.cn

[S33] C++：vector 增删
来源：http://dxt.ppjwa.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fwi.zdbjq.cn

[S34] C++：遍历 vector
来源：http://tdk.xuetiantiany.cn

for (auto &x : v) { std::cout << x; }
来源：http://gun.cashguo.top

[S35] C++：map
来源：http://cnm.cqqwz.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mem.daxiang520.top

[S36] C++：unordered_map
来源：http://gae.cdnleiting.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cnh.gogol.net.cn

[S37] C++：set
来源：http://ngx.mhx1999.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://emk.hysaishi.cn

[S38] C++：排序
来源：http://mry.jlsjyb.cn

std::sort(v.begin(), v.end());
来源：http://dqc.shangyingyoupin.top

[S39] C++：自定义比较器排序
来源：http://ono.wangdashe.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hoq.ivvv.top

[S40] C++：查找元素
来源：http://jku.aibaodan.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nlz.hnqzz.top

[S41] C++：类与构造函数
来源：http://ftj.ydzc1.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wjt.aizwys.cn

[S42] C++：继承与虚函数
来源：http://oqr.jinqigufen.top

class B : public Base { public: void f() override {} };
来源：http://scu.fehbvm.com

[S43] C++：智能指针
来源：http://tjp.nwbrower.top

auto p = std::make_unique<int>(5);
来源：http://ybc.havefunace.top

[S44] C++：引用传参
来源：http://lyx.yj202588.top

void inc(int &x) { ++x; }
来源：http://gqh.0kj1m.cn

[S45] C++：lambda
来源：http://isu.hnxiangtu.top

auto add = [](int a, int b) { return a + b; };
来源：http://zcn.yvedp.cn

[S46] C++：函数模板
来源：http://ire.dianchejie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vtj.fzhhl.top

[S47] C++：结构化绑定遍历
来源：http://zcd.yuanzhike.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://euy.birdmap.top

[S48] C++：逐行读文件
来源：http://ikz.andypj.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://sua.hnqzz.top

while (std::getline(in, line)) { }
来源：http://hkz.9152youxi.cn

[S49] C++：写文件
来源：http://mnh.hfpthk.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xsa.hnxiangtu.top

[S50] C++：格式化数字
来源：http://oxd.sjlbkw.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lud.yj202588.top

[S51] C++：显式类型转换
来源：http://ofq.jinqigufen.top

static_cast<double>(a) / b
来源：http://mpf.fktsv.cn

[S52] C++：const 与 noexcept
来源：http://cyc.kuanghao11.cn

int size() const noexcept { return n_; }
来源：http://lug.xinyue.icu

[S53] C++：移动语义
来源：http://uth.hfpthk.cn

std::vector<int> w = std::move(v);
来源：http://bak.jinyuanbaomall.cn

[S54] C++：异常处理
来源：http://gmx.hysaishi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://siw.meibo888.top

[S55] C++：结构化绑定
来源：http://bhw.zdqjudy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://sxn.daria6918.cn

[S56] C++：optional
来源：http://vdp.nwbrower.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://byo.hongshengwenyu.top

[S57] C++：编译期常量
来源：http://dxi.zhixingplan.top

constexpr int N = 10;
来源：http://tnn.wangshuangyany.cn

[S58] C++：命名空间
来源：http://qqe.9152youxi.cn

namespace ns { int f() { return 1; } }
来源：http://yli.yvedp.cn

[S59] C++：静态断言
来源：http://vhm.feifeiyinyue.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://axq.0kj1m.cn

[S60] C++：遍历并删除元素
来源：http://fkl.wangdashe.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tra.hesvh.cn

================================================================================
来源：http://xnk.havefunace.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xat.snrcjt.cn

================================================================================
来源：http://loc.ydzc1.top

[T01] Kotlin：Hello World
来源：http://red.yuxming.cn

println("Hello")
来源：http://roi.snrcjt.cn

[T02] Kotlin：变量
来源：http://sjo.hammf.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ski.fzhhl.top

[T03] Kotlin：字符串模板
来源：http://zru.dianchejie.cn

"值: $b"
来源：http://acb.yueranfly.top

[T04] Kotlin：空安全
来源：http://vrw.epnwcf.com

val n: String? = null;  n?.length
来源：http://bbv.chenlongwang.top

[T05] Kotlin：when 表达式
来源：http://tgv.hywenlv.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mmn.zdbjq.cn

[T06] Kotlin：集合映射
来源：http://wlx.cheryme.top

listOf(1, 2, 3).map { it * 2 }
来源：http://kge.sysykeji.top

[T07] Kotlin：集合过滤
来源：http://mzl.yonumen.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://nex.hongshengwenyu.top

[T08] Kotlin：数据类
来源：http://mml.yj20258.top

data class User(val name: String, val age: Int)
来源：http://zxh.andypj.xyz

[T09] Kotlin：扩展函数
来源：http://sts.bjfxy.top

fun String.exclaim() = this + "!"
来源：http://uqc.hnxiangtu.top

[T10] Kotlin：默认参数
来源：http://xoa.yj202588.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ram.hcnkem.com

[T11] Kotlin：协程
来源：http://gtt.andypj.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://jof.guowangkeji.top

[T12] Kotlin：解构声明
来源：http://iop.ivvv.top

val (a, b) = Pair(1, 2)
来源：http://jjp.aizwys.cn

[T13] Kotlin：只读 Map
来源：http://bkn.yonumen.top

val m = mapOf("a" to 1)
来源：http://zjx.jinghuilouyu.cn

[T14] Kotlin：循环
来源：http://ebf.hysaishi.cn

for (i in 1..10) println(i)
来源：http://jav.zhijiandao.cn

[T15] Kotlin：接口
来源：http://slk.yj20258.top

interface Shape { fun area(): Double }
来源：http://tuc.nwbrower.top

[T16] Swift：Hello World
来源：http://yin.jqgufenzy.top

print("Hello")
来源：http://gaf.jinyuanbaomall.cn

[T17] Swift：变量与常量
来源：http://plr.redwolf501.top

var a = 1;  let b = 2
来源：http://ezz.sxryk.cn

[T18] Swift：字符串插值
来源：http://lpq.feifeiyinyue.top

"值: \(b)"
来源：http://rrq.yj20258.top

[T19] Swift：可选绑定
来源：http://jwh.sjlbkw.cn

if let n = opt { print(n) }
来源：http://dai.gogol.net.cn

[T20] Swift：数组操作
来源：http://wyf.snrcjt.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mmd.ivvv.top

[T21] Swift：遍历
来源：http://acq.zhixingplan.top

for x in a { print(x) }
来源：http://gay.yonumen.top

[T22] Swift：字典
来源：http://mzm.gaohongyu789.top

var d = ["a": 1];  d["b"] = 2
来源：http://mub.fehbvm.com

[T23] Swift：函数
来源：http://kmr.jinqigufen.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pdz.shzxlz.cn

[T24] Swift：闭包
来源：http://uec.zhiwuduotai.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://gdx.hcnkem.com

[T25] Swift：结构体
来源：http://dys.zhiwuduotai.top

struct P { var x: Int }
来源：http://zkp.shangyingyoupin.top

[T26] Swift：类与重写
来源：http://lqd.ywan-chungtsiang.top

class A: Base { override func f() {} }
来源：http://jdu.pycfn.com

[T27] Swift：错误处理
来源：http://aum.shuidangran.top

do { try f() } catch { print(error) }
来源：http://yny.tarul.cn

[T28] Swift：枚举
来源：http://pxc.uphjek.com

enum Color { case red, green }
来源：http://glm.shuidangran.top

[T29] Swift：guard 提前返回
来源：http://tik.uphjek.com

guard let x = opt else { return }
来源：http://gui.cdnleiting.top

[T30] Swift：协议
来源：http://xat.birdmap.top

protocol Shape { func area() -> Double }
来源：http://nxx.jinqigfzy.top

[T31] Lua：Hello World
来源：http://tph.sysykeji.top

print("Hello")
来源：http://paq.zhengqikj.top

[T32] Lua：局部变量
来源：http://ceo.xuetiantiany.cn

local a = 1
来源：http://jvt.wangshuangyany.cn

[T33] Lua：表（数组）
来源：http://zyp.hfpthk.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://geq.yj20258888.top

[T34] Lua：遍历表
来源：http://krb.snrcjt.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ebf.guowangkeji.top

[T35] Lua：字典表
来源：http://xie.ehwqpu.com

local d = { a = 1 };  d.b = 2
来源：http://hgp.pengpengdd.cyou

[T36] Lua：函数
来源：http://kpm.yuanzhike.top

function add(a, b) return a + b end
来源：http://mts.yj20258888.top

[T37] Lua：字符串拼接
来源：http://ymz.zdbjq.cn

"a" .. "b"
来源：http://doe.0kj1m.cn

[T38] Lua：条件
来源：http://ujt.0kj1m.cn

if x > 0 then print("正") end
来源：http://lmc.fengsongda.top

[T39] Lua：模式匹配
来源：http://kfv.sysykeji.top

string.find(s, "%d+")
来源：http://ylc.sxryk.cn

[T40] Lua：元表
来源：http://qru.haohaochexian.top

setmetatable({}, { __index = base })
来源：http://bgn.hesvh.cn

[T41] Perl：Hello World
来源：http://uvw.birdmap.top

print "Hello\n";
来源：http://lel.zdbjq.cn

[T42] Perl：变量类型
来源：http://ovz.zhijiandao.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://aff.nanxuanxn.top

[T43] Perl：字符串插值
来源：http://com.yvedp.cn

"值: $a"
来源：http://pal.svipenyu.cn

[T44] Perl：条件
来源：http://ecj.jianghu66.top

if ($a > 0) { print "正"; }
来源：http://adl.nanxinkj.top

[T45] Perl：数组遍历
来源：http://lpm.vqdsnc.cn

for my $x (@arr) { print $x; }
来源：http://vgz.vqdsnc.cn

[T46] Perl：哈希操作
来源：http://fkq.cucudq.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jyo.hesvh.cn

[T47] Perl：正则捕获
来源：http://bwm.hnxiangtu.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://xnw.shanyushiyangkeji.top

[T48] Perl：正则替换
来源：http://sdj.xylfe.cn

$s =~ s/old/new/g;
来源：http://lik.ydjk.org.cn

[T49] Perl：函数
来源：http://imp.nanxuanxn.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://eei.jianghu66.top

[T50] Perl：逐行读文件
来源：http://hwu.gzhubu.top

open my $fh, "<", "a.txt" or die $!;
来源：http://gsm.hongshengwenyu.top

while (my $line = <$fh>) { print $line; }
来源：http://kob.yongpay.top

[T51] Scala：Hello World
来源：http://qrg.gaohongyu789.top

println("Hello")
来源：http://pmc.xziqi.cn

[T52] Scala：变量
来源：http://yfo.c1oappe.top

val a = 1;  var b = 2
来源：http://vvs.zhengqikj.top

[T53] Scala：字符串插值
来源：http://vus.fzhhl.top

s"值: $b"
来源：http://oiq.andypj.xyz

[T54] Scala：集合映射
来源：http://zia.jinghuilouyu.cn

List(1, 2, 3).map(_ * 2)
来源：http://mdc.quarkkingdee.top

[T55] Scala：集合过滤
来源：http://hqg.ppjwa.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gbb.jyoumei.cn

[T56] Scala：样例类
来源：http://cgo.jiagoushi.top

case class User(name: String, age: Int)
来源：http://xhr.jqgufenzy.top

[T57] Scala：模式匹配
来源：http://bif.havefunace.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://xsj.fanxiaobao.xyz

[T58] Scala：函数定义
来源：http://vkq.quarkkingdee.top

def add(a: Int, b: Int): Int = a + b
来源：http://whu.zhongyouzk.top

[T59] Scala：循环
来源：http://mwi.fktsv.cn

for (i <- 1 to 10) println(i)
来源：http://pdi.zhengqikj.top

[T60] Scala：折叠
来源：http://fxx.guannengcc.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ctr.chenlongwang.top

================================================================================
来源：http://yrf.ybcxt.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vpy.0kj1m.cn

================================================================================
来源：http://xhr.cucudq.cn

[U01] Py：创建虚拟环境
来源：http://zan.xuetiantiany.cn

python -m venv .venv && source .venv/bin/activate
来源：http://dqk.ehwqpu.com

[U02] Py：导出 / 安装依赖
来源：http://jcf.yangfankeji.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pjr.ywan-chungtsiang.top

[U03] Py：加载 .env 配置
来源：http://nit.nanxinkj.top

from dotenv import load_dotenv; load_dotenv()
来源：http://hty.epnwcf.com

[U04] Py：变量调试打印
来源：http://yjx.tarul.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://alz.cashguo.top

[U05] Py：列表去重且保序
来源：http://duu.shangyingyoupin.top

list(dict.fromkeys(arr))
来源：http://tzb.tian-w.cn

[U06] Py：合并两个字典
来源：http://hog.hesvh.cn

{**a, **b}
来源：http://bbv.chenjidiqi.icu

[U07] Py：反转字典键值
来源：http://qlm.cqqwz.cn

{v: k for k, v in d.items()}
来源：http://bvv.zhijiandao.cn

[U08] Py：展平二维列表
来源：http://ftw.jlsjyb.cn

[y for x in nested for y in x]
来源：http://rfm.cdnleiting.top

[U09] Py：字典取最大值的键
来源：http://kmn.cqqwz.cn

max(d, key=d.get)
来源：http://klw.jinqigufen.top

[U10] Py：按值排序字典
来源：http://ezv.yangfankeji.com

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yuh.snrcjt.cn

[U11] Py：生成器表达式
来源：http://umv.xinyue.icu

(x * 2 for x in arr)
来源：http://fth.dashuyun.cn

[U12] Py：取出现最多的 3 个元素
来源：http://oyh.svipenyu.cn

Counter(arr).most_common(3)
来源：http://abl.yonumen.top

[U13] Py：固定长度队列
来源：http://hwn.xuanzx.com

deque(maxlen=10)
来源：http://twx.sysykeji.top

[U14] Py：分组收集到列表
来源：http://uyb.xinyue.icu

defaultdict(list)
来源：http://xjc.fehbvm.com

[U15] Py：高精度计时
来源：http://jdz.hysaishi.cn

t = time.perf_counter()
来源：http://flb.cqqwz.cn

[U16] Py：命令行参数解析
来源：http://azn.yj20258888.top

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hsf.shanyushiyangtech.top

[U17] Py：初始化日志
来源：http://psl.ywan-chungtsiang.top

logging.basicConfig(level=logging.INFO)
来源：http://fqf.mhx1999.top

[U18] Py：预编译正则
来源：http://ydk.feifeiyinyue.top

pat = re.compile(r"\d+")
来源：http://haf.nwbrower.top

[U19] Py：正则替换带回调
来源：http://wdv.mhx1999.top

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://suo.chenjidiqi.icu

[U20] Py：缓存函数结果
来源：http://fnv.jqgfzy.top

@functools.lru_cache(maxsize=None)
来源：http://yic.zhiwuduotai.top

[U21] Py：自定义上下文管理器
来源：http://ppe.dianchejie.cn

@contextlib.contextmanager
来源：http://jgm.uphjek.com

[U22] Py：矩阵转置
来源：http://yaa.zhengqikj.top

list(zip(*m))
来源：http://cug.jlsjyb.cn

[U23] Py：分块读取大文件
来源：http://dsx.xinyue.icu

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rpx.quarkkingdee.top

[U24] Py：路径操作
来源：http://uwy.jinqigufen.top

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://flu.redwolf501.top


<!-- 参考信息 -->