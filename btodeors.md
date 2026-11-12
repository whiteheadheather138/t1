代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://ygf.zhoulong.xyz

[R70] 时间戳与互转
来源：http://zny.yanxiufei.cn

date +%s;  date -d @1700000000
来源：http://wvk.feifeiyinyue.top

[R71] 日期格式化
来源：http://msz.zhiwuduotai.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://blv.tarul.cn

[R72] 等待端口就绪
来源：http://mmz.daxiang520.top

until nc -z localhost 3306; do sleep 1; done
来源：http://loj.ctjpmb.com

[R73] 分割大日志
来源：http://hva.guowangkeji.top

split -l 1000 big.log part_
来源：http://vms.havefunace.top

[R74] 批量重命名
来源：http://vfz.ybcxt.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dpv.zhaomingkeji.xyz

[R75] 导出环境变量
来源：http://wkc.yj20258888.top

export PATH="$HOME/bin:$PATH"
来源：http://rps.shanyushiyangkeji.top

[R76] 使用临时文件
来源：http://cth.xuanzx.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://epd.nanxinkj.top

[R77] 读取用户输入
来源：http://wad.redwolf501.top

read -rp "请输入: " ans
来源：http://kcl.zhijiandao.cn

[R78] 交互式菜单
来源：http://ekw.guannengcc.top

select opt in a b c; do echo "$opt"; break; done
来源：http://shv.yj202588.top

[R79] 解析命令行选项
来源：http://hvg.hnxiangtu.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://awa.andypj.xyz

[R80] 查看脚本执行耗时
来源：http://ziv.bbcook.cn

time ./run.sh
来源：http://rkg.yueranfly.top

================================================================================
来源：http://snz.birdmap.top

S. C / C++ 专题
来源：http://blm.yanxiufei.cn

================================================================================
来源：http://xly.gogol.net.cn

[S01] C：Hello World
来源：http://txa.chenzaomai.com

#include <stdio.h>
来源：http://ymr.uphjek.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://rxt.yuxming.cn

[S02] C：变量与格式化输出
来源：http://urs.dashuyun.cn

int a = 10; printf("%d\n", a);
来源：http://scg.shanyushiyangtech.top

[S03] C：读入整数
来源：http://nei.sweek.top

int x; scanf("%d", &x);
来源：http://xeb.fzhhl.top

[S04] C：字符串复制
来源：http://uwa.smart0.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://dpm.pengpengdd.cyou

[S05] C：字符串长度
来源：http://mfi.yvedp.cn

strlen(s)
来源：http://gnf.meibo888.top

[S06] C：字符串比较
来源：http://eik.fehbvm.com

strcmp(a, b) == 0
来源：http://hcg.xinyue.icu

[S07] C：数组遍历求和
来源：http://xmu.xingfuxueyuan.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ogc.hywenlv.cn

[S08] C：动态内存分配与释放
来源：http://gnq.tarul.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hus.vqdsnc.cn

[S09] C：结构体定义与初始化
来源：http://osq.guowangkeji.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://arp.316326.xyz

[S10] C：指针与解引用
来源：http://dir.pengpengdd.cyou

int *p = &a;  *p = 5;
来源：http://wgw.nanxuanxn.top

[S11] C：逐行读文件
来源：http://lfz.yj202588.top

FILE *f = fopen("a.txt", "r");
来源：http://thj.mhx1999.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://uep.yj20258.top

fclose(f);
来源：http://yft.zhiwuduotai.top

[S12] C：写文件
来源：http://sym.andypj.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qft.zdqjudy.top

[S13] C：宏定义
来源：http://npg.xuetiantiany.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ovh.shanyushiyangkeji.top

[S14] C：枚举
来源：http://zez.yongpay.top

enum Color { RED, GREEN, BLUE };
来源：http://iyl.jinyuanbaomall.cn

[S15] C：类型转换
来源：http://zri.sweek.top

(double) a / b
来源：http://tmz.zycfv.cn

[S16] C：位操作置位
来源：http://emq.guannengcc.top

x |= (1 << 3);
来源：http://vgm.jlsjyb.cn

[S17] C：安全拼接字符串
来源：http://zcz.kuanghao11.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tiu.xuetiantiany.cn

[S18] C：命令行参数
来源：http://qyg.ydzc1.top

int main(int argc, char **argv)
来源：http://hya.jqgfzy.top

[S19] C：快速排序
来源：http://djm.tian-w.cn

qsort(a, n, sizeof(int), cmp);
来源：http://eum.hammf.cn

[S20] C：二分查找
来源：http://qxr.xuetiantiany.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://evy.zycfv.cn

[S21] C：字符类别判断
来源：http://svy.jinqigufen.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kqz.zhongyouzk.top

[S22] C：字符串转数字
来源：http://lle.epnwcf.com

atoi("42");  strtod("3.14", NULL);
来源：http://zhb.kuanghao11.cn

[S23] C：随机数
来源：http://tmh.fanxiaobao.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://ili.aibaodan.cn

[S24] C：获取本地时间
来源：http://fll.chenlongwang.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nqp.hongshengwenyu.top

[S25] C：内存拷贝
来源：http://zwj.mhx1999.top

memcpy(dst, src, n);
来源：http://qwi.fzhhl.top

[S26] C：内存清零
来源：http://aeu.aizwys.cn

memset(a, 0, sizeof a);
来源：http://eka.gaohongyu789.top

[S27] C：定义常量
来源：http://khz.ybcxt.top

const double PI = 3.14159;
来源：http://gio.yvedp.cn

[S28] C：静态变量
来源：http://lst.jianghu66.top

static int counter = 0;
来源：http://xjv.smart0.xyz

[S29] C：变参函数
来源：http://cvy.hesvh.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://swb.316326.xyz

[S30] C：头文件保护
来源：http://pvh.chenlongwang.top

#ifndef X_H
来源：http://dvu.hongshengwenyu.top

#define X_H
来源：http://olp.xinyue.icu

#endif
来源：http://qio.sufxvd.cn

[S31] C++：Hello World
来源：http://zfq.fengsongda.top

#include <iostream>
来源：http://elz.dashuyun.cn

int main() { std::cout << "Hello\n"; }
来源：http://krt.ywan-chungtsiang.top

[S32] C++：字符串
来源：http://lnv.jiagoushi.top

std::string s = "hi";  s += "!";
来源：http://irb.hnqzz.top

[S33] C++：vector 增删
来源：http://xmq.jianghu66.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://eer.daria6918.cn

[S34] C++：遍历 vector
来源：http://pqq.svipenyu.cn

for (auto &x : v) { std::cout << x; }
来源：http://qlm.fehbvm.com

[S35] C++：map
来源：http://twt.zhixingplan.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wkw.yvedp.cn

[S36] C++：unordered_map
来源：http://psa.aizwys.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xyt.shangyingyoupin.top

[S37] C++：set
来源：http://ori.jqgfzy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://teb.aibaodan.cn

[S38] C++：排序
来源：http://qle.hesvh.cn

std::sort(v.begin(), v.end());
来源：http://jey.jyoumei.cn

[S39] C++：自定义比较器排序
来源：http://dug.0kj1m.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ueu.chenlongwang.top

[S40] C++：查找元素
来源：http://eci.tianlin.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mlj.yfazqb.com

[S41] C++：类与构造函数
来源：http://dvj.guowangkeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bmi.xinyue.icu

[S42] C++：继承与虚函数
来源：http://kam.dianchejie.cn

class B : public Base { public: void f() override {} };
来源：http://dky.xuetiantiany.cn

[S43] C++：智能指针
来源：http://cmi.xuetiantiany.cn

auto p = std::make_unique<int>(5);
来源：http://gva.zdqjudy.top

[S44] C++：引用传参
来源：http://ovu.shanyushiyangkeji.top

void inc(int &x) { ++x; }
来源：http://ibq.sjlbkw.cn

[S45] C++：lambda
来源：http://gal.yongpay.top

auto add = [](int a, int b) { return a + b; };
来源：http://zde.yueranfly.top

[S46] C++：函数模板
来源：http://ufp.tanke756.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zul.shangyingyoupin.top

[S47] C++：结构化绑定遍历
来源：http://gbq.bjfxy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://non.xziqi.cn

[S48] C++：逐行读文件
来源：http://jkb.bbcook.cn

std::ifstream in("a.txt");  std::string line;
来源：http://elk.tanke756.top

while (std::getline(in, line)) { }
来源：http://vaj.daria6918.cn

[S49] C++：写文件
来源：http://isb.zhaomingkeji.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cli.fktsv.cn

[S50] C++：格式化数字
来源：http://xsq.epnwcf.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jko.tanke756.top

[S51] C++：显式类型转换
来源：http://wtn.jlsjyb.cn

static_cast<double>(a) / b
来源：http://npx.xingfuxueyuan.xyz

[S52] C++：const 与 noexcept
来源：http://muf.316326.xyz

int size() const noexcept { return n_; }
来源：http://iwq.guannengcc.top

[S53] C++：移动语义
来源：http://ouf.hcnkem.com

std::vector<int> w = std::move(v);
来源：http://mtx.jinyuanbaomall.cn

[S54] C++：异常处理
来源：http://qms.yuanzhike.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://obx.andypj.xyz

[S55] C++：结构化绑定
来源：http://ltg.xuanzx.com

auto [a, b] = std::make_pair(1, 2);
来源：http://ojt.daxiang520.top

[S56] C++：optional
来源：http://npc.iojbl.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cuf.hywenlv.cn

[S57] C++：编译期常量
来源：http://rva.gzhubu.top

constexpr int N = 10;
来源：http://vao.fzhhl.top

[S58] C++：命名空间
来源：http://xdc.meibo888.top

namespace ns { int f() { return 1; } }
来源：http://tgg.xuetiantiany.cn

[S59] C++：静态断言
来源：http://ncr.zhaomingkeji.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pmd.zdqjudy.top

[S60] C++：遍历并删除元素
来源：http://aws.bjfxy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bak.bjfxy.top

================================================================================
来源：http://qzc.ywan-chungtsiang.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hat.havefunace.top

================================================================================
来源：http://fcp.cheryme.top

[T01] Kotlin：Hello World
来源：http://urh.yvedp.cn

println("Hello")
来源：http://gpg.kuanghao11.cn

[T02] Kotlin：变量
来源：http://mgv.c1oappe.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lbn.hfpthk.cn

[T03] Kotlin：字符串模板
来源：http://ejr.bjfxy.top

"值: $b"
来源：http://gtr.guannengcc.top

[T04] Kotlin：空安全
来源：http://jdt.quarkkingdee.top

val n: String? = null;  n?.length
来源：http://nap.shzxlz.cn

[T05] Kotlin：when 表达式
来源：http://hxs.jinqigufen.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://eas.ctjpmb.com

[T06] Kotlin：集合映射
来源：http://hzr.dashuyun.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://lxo.ybcxt.top

[T07] Kotlin：集合过滤
来源：http://uxj.tian-w.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wfs.zdqjudy.top

[T08] Kotlin：数据类
来源：http://jmf.xingfuxueyuan.xyz

data class User(val name: String, val age: Int)
来源：http://hyx.yonumen.top

[T09] Kotlin：扩展函数
来源：http://yhc.ppjwa.cn

fun String.exclaim() = this + "!"
来源：http://rqz.xuanzx.com

[T10] Kotlin：默认参数
来源：http://bsa.cdnleiting.top

fun greet(name: String = "World") = "Hi $name"
来源：http://uat.hysaishi.cn

[T11] Kotlin：协程
来源：http://cjm.chenzaomai.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://lbb.shanyushiyangkeji.top

[T12] Kotlin：解构声明
来源：http://wbj.ywan-chungtsiang.top

val (a, b) = Pair(1, 2)
来源：http://kfv.quarkkingdee.top

[T13] Kotlin：只读 Map
来源：http://csv.fzhhl.top

val m = mapOf("a" to 1)
来源：http://hun.chenjidiqi.icu

[T14] Kotlin：循环
来源：http://biv.shanyushiyangtech.top

for (i in 1..10) println(i)
来源：http://xqp.jyoumei.cn

[T15] Kotlin：接口
来源：http://kgg.uphjek.com

interface Shape { fun area(): Double }
来源：http://svl.zhiwuduotai.top

[T16] Swift：Hello World
来源：http://nza.9152youxi.cn

print("Hello")
来源：http://ftl.c1oappe.top

[T17] Swift：变量与常量
来源：http://vhb.yj20258.top

var a = 1;  let b = 2
来源：http://zaw.fzhhl.top

[T18] Swift：字符串插值
来源：http://jvm.ydzc1.top

"值: \(b)"
来源：http://aea.hesvh.cn

[T19] Swift：可选绑定
来源：http://fwc.hnqzz.top

if let n = opt { print(n) }
来源：http://dov.vqdsnc.cn

[T20] Swift：数组操作
来源：http://kwe.kuanghao11.cn

var a = [1, 2, 3];  a.append(4)
来源：http://huv.fengsongda.top

[T21] Swift：遍历
来源：http://exv.cdnleiting.top

for x in a { print(x) }
来源：http://aeo.jyoumei.cn

[T22] Swift：字典
来源：http://wrl.sjlbkw.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xii.zhijiandao.cn

[T23] Swift：函数
来源：http://pxx.fehbvm.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://akm.ctjpmb.com

[T24] Swift：闭包
来源：http://drm.316326.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://reh.xylfe.cn

[T25] Swift：结构体
来源：http://efs.meibo888.top

struct P { var x: Int }
来源：http://wwc.yonumen.top

[T26] Swift：类与重写
来源：http://bpy.xuetiantiany.cn

class A: Base { override func f() {} }
来源：http://efr.tarul.cn

[T27] Swift：错误处理
来源：http://pht.zhongyouzk.top

do { try f() } catch { print(error) }
来源：http://luy.ywan-chungtsiang.top

[T28] Swift：枚举
来源：http://oni.0kj1m.cn

enum Color { case red, green }
来源：http://hce.shanyushiyangkeji.top

[T29] Swift：guard 提前返回
来源：http://fyc.sysykeji.top

guard let x = opt else { return }
来源：http://bxl.zdbjq.cn

[T30] Swift：协议
来源：http://tun.cucudq.cn

protocol Shape { func area() -> Double }
来源：http://cad.yangfankeji.com

[T31] Lua：Hello World
来源：http://cfg.zhaomingkeji.xyz

print("Hello")
来源：http://nom.uphjek.com

[T32] Lua：局部变量
来源：http://gkn.yj20258.top

local a = 1
来源：http://mky.cdnleiting.top

[T33] Lua：表（数组）
来源：http://ueg.daxiang520.top

local t = {1, 2, 3};  t[4] = 4
来源：http://fmw.sxryk.cn

[T34] Lua：遍历表
来源：http://xat.jianghu66.top

for i, v in ipairs(t) do print(i, v) end
来源：http://inv.hesvh.cn

[T35] Lua：字典表
来源：http://asf.pycfn.com

local d = { a = 1 };  d.b = 2
来源：http://skj.pengpengdd.cyou

[T36] Lua：函数
来源：http://tjq.jiagoushi.top

function add(a, b) return a + b end
来源：http://ekn.ybcxt.top

[T37] Lua：字符串拼接
来源：http://ngg.zdqjudy.top

"a" .. "b"
来源：http://tug.mhx1999.top

[T38] Lua：条件
来源：http://kbe.wangdashe.top

if x > 0 then print("正") end
来源：http://pxs.zhiwuduotai.top

[T39] Lua：模式匹配
来源：http://wgw.hnxiangtu.top

string.find(s, "%d+")
来源：http://emi.daria6918.cn

[T40] Lua：元表
来源：http://pyc.jiagoushi.top

setmetatable({}, { __index = base })
来源：http://zpg.cqqwz.cn

[T41] Perl：Hello World
来源：http://hpt.52xcode.cn

print "Hello\n";
来源：http://iir.jianghu66.top

[T42] Perl：变量类型
来源：http://sfx.cqqwz.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wvw.wangdashe.top

[T43] Perl：字符串插值
来源：http://tdz.shanyushiyangtech.top

"值: $a"
来源：http://ybd.ywan-chungtsiang.top

[T44] Perl：条件
来源：http://flo.jlsjyb.cn

if ($a > 0) { print "正"; }
来源：http://goh.redwolf501.top

[T45] Perl：数组遍历
来源：http://iww.jqgufenzy.top

for my $x (@arr) { print $x; }
来源：http://wxg.shanyushiyangtech.top

[T46] Perl：哈希操作
来源：http://ldy.zhiwuduotai.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ijg.gzhubu.top

[T47] Perl：正则捕获
来源：http://gzb.birdmap.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://rwx.tianlin.xyz

[T48] Perl：正则替换
来源：http://fdb.chenlongwang.top

$s =~ s/old/new/g;
来源：http://qwg.aibaodan.cn

[T49] Perl：函数
来源：http://ccj.sjlbkw.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mre.zhengqikj.top

[T50] Perl：逐行读文件
来源：http://gjf.mhx1999.top

open my $fh, "<", "a.txt" or die $!;
来源：http://tnb.zhiwuduotai.top

while (my $line = <$fh>) { print $line; }
来源：http://peu.jinqigufen.top

[T51] Scala：Hello World
来源：http://txk.gotoacloud.top

println("Hello")
来源：http://xrj.tianlin.xyz

[T52] Scala：变量
来源：http://hua.tarul.cn

val a = 1;  var b = 2
来源：http://tnq.xylfe.cn

[T53] Scala：字符串插值
来源：http://hpq.tanke756.top

s"值: $b"
来源：http://yli.zhengqikj.top

[T54] Scala：集合映射
来源：http://kys.meibo888.top

List(1, 2, 3).map(_ * 2)
来源：http://sbr.316326.xyz

[T55] Scala：集合过滤
来源：http://hrp.jiagoushi.top

List(1, 2, 3).filter(_ > 1)
来源：http://aob.xinyue.icu

[T56] Scala：样例类
来源：http://pid.zhixingplan.top

case class User(name: String, age: Int)
来源：http://wmt.hcnkem.com

[T57] Scala：模式匹配
来源：http://oae.shzxlz.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://lje.hammf.cn

[T58] Scala：函数定义
来源：http://vww.wangshuangyany.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zjj.nwbrower.top

[T59] Scala：循环
来源：http://qkz.yvedp.cn

for (i <- 1 to 10) println(i)
来源：http://ert.hcnkem.com

[T60] Scala：折叠
来源：http://egm.chenjidiqi.icu

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xhv.ehwqpu.com

================================================================================
来源：http://acd.feifeiyinyue.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xjv.hywenlv.cn

================================================================================
来源：http://rqf.zycfv.cn

[U01] Py：创建虚拟环境
来源：http://kqe.sweek.top

python -m venv .venv && source .venv/bin/activate
来源：http://uif.cheryme.top

[U02] Py：导出 / 安装依赖
来源：http://hzg.yangfankeji.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ywy.316326.xyz

[U03] Py：加载 .env 配置
来源：http://dzm.yj20258888.top

from dotenv import load_dotenv; load_dotenv()
来源：http://miz.zdqjudy.top

[U04] Py：变量调试打印
来源：http://yab.sufxvd.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kda.ywan-chungtsiang.top

[U05] Py：列表去重且保序
来源：http://phe.vqdsnc.cn

list(dict.fromkeys(arr))
来源：http://gmg.sweek.top

[U06] Py：合并两个字典
来源：http://irq.yvedp.cn

{**a, **b}
来源：http://mla.zhongyouzk.top

[U07] Py：反转字典键值
来源：http://osg.shangyingyoupin.top

{v: k for k, v in d.items()}
来源：http://coi.guowangkeji.top

[U08] Py：展平二维列表
来源：http://wdk.gotoacloud.top

[y for x in nested for y in x]
来源：http://sdx.tian-w.cn

[U09] Py：字典取最大值的键
来源：http://sbs.andypj.xyz

max(d, key=d.get)
来源：http://scr.dianchejie.cn

[U10] Py：按值排序字典
来源：http://wch.cqqwz.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dix.jiagoushi.top


<!-- 参考信息 -->