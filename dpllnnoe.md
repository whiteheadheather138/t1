代发 wailian999

head -c 16 /dev/urandom | base64
来源：http://jxl.cheryme.top

[R70] 时间戳与互转
来源：http://xgy.zhijiandao.cn

date +%s;  date -d @1700000000
来源：http://zgf.fehbvm.com

[R71] 日期格式化
来源：http://pda.shanyushiyangkeji.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://uqd.wangdashe.top

[R72] 等待端口就绪
来源：http://vjq.yongpay.top

until nc -z localhost 3306; do sleep 1; done
来源：http://hyz.hammf.cn

[R73] 分割大日志
来源：http://qzy.nanxinkj.top

split -l 1000 big.log part_
来源：http://ani.zhiwuduotai.top

[R74] 批量重命名
来源：http://ywl.xinyue.icu

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hhr.redwolf501.top

[R75] 导出环境变量
来源：http://ihe.hammf.cn

export PATH="$HOME/bin:$PATH"
来源：http://dlz.cucudq.cn

[R76] 使用临时文件
来源：http://fyw.zdqjudy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yla.chenzaomai.com

[R77] 读取用户输入
来源：http://yhn.0kj1m.cn

read -rp "请输入: " ans
来源：http://xnl.aibaodan.cn

[R78] 交互式菜单
来源：http://cho.vqdsnc.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://vox.quarkkingdee.top

[R79] 解析命令行选项
来源：http://qjf.shzxlz.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://que.cqqwz.cn

[R80] 查看脚本执行耗时
来源：http://yqk.zhengqikj.top

time ./run.sh
来源：http://mtj.yanxiufei.cn

================================================================================
来源：http://pjw.xylfe.cn

S. C / C++ 专题
来源：http://hlf.sjlbkw.cn

================================================================================
来源：http://ety.nanxinkj.top

[S01] C：Hello World
来源：http://zec.jinqigfzy.top

#include <stdio.h>
来源：http://hce.jqgfzy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://lyx.shanyushiyangkeji.top

[S02] C：变量与格式化输出
来源：http://dnq.cdnleiting.top

int a = 10; printf("%d\n", a);
来源：http://dhn.quarkkingdee.top

[S03] C：读入整数
来源：http://wgq.gogol.net.cn

int x; scanf("%d", &x);
来源：http://frp.tanke756.top

[S04] C：字符串复制
来源：http://vbl.feifeiyinyue.top

char dst[32]; strcpy(dst, "hi");
来源：http://jhb.jlsjyb.cn

[S05] C：字符串长度
来源：http://amh.jinqigfzy.top

strlen(s)
来源：http://xpi.zdbjq.cn

[S06] C：字符串比较
来源：http://gqs.birdmap.top

strcmp(a, b) == 0
来源：http://rot.tianlin.xyz

[S07] C：数组遍历求和
来源：http://mgm.zhongyouzk.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hzg.ybcxt.top

[S08] C：动态内存分配与释放
来源：http://vyz.9152youxi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kod.yuxming.cn

[S09] C：结构体定义与初始化
来源：http://yri.sjlbkw.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tqf.jyoumei.cn

[S10] C：指针与解引用
来源：http://aex.zdqjudy.top

int *p = &a;  *p = 5;
来源：http://ery.jqgufenzy.top

[S11] C：逐行读文件
来源：http://sge.cashguo.top

FILE *f = fopen("a.txt", "r");
来源：http://udm.yj20258.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://sbd.gzhubu.top

fclose(f);
来源：http://pgs.zhongyouzk.top

[S12] C：写文件
来源：http://yfz.yanxiufei.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://usp.yvedp.cn

[S13] C：宏定义
来源：http://qps.zhaomingkeji.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://afk.hnxiangtu.top

[S14] C：枚举
来源：http://vzh.xuetiantiany.cn

enum Color { RED, GREEN, BLUE };
来源：http://cnr.yonumen.top

[S15] C：类型转换
来源：http://knj.jqgfzy.top

(double) a / b
来源：http://pbh.9152youxi.cn

[S16] C：位操作置位
来源：http://kkq.zhiwuduotai.top

x |= (1 << 3);
来源：http://jkt.yfazqb.com

[S17] C：安全拼接字符串
来源：http://gxg.jinyuanbaomall.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kgu.xziqi.cn

[S18] C：命令行参数
来源：http://hqn.xylfe.cn

int main(int argc, char **argv)
来源：http://jnf.cashguo.top

[S19] C：快速排序
来源：http://ctv.0kj1m.cn

qsort(a, n, sizeof(int), cmp);
来源：http://khq.hywenlv.cn

[S20] C：二分查找
来源：http://fkd.hnxiangtu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://eie.chenzaomai.com

[S21] C：字符类别判断
来源：http://dok.52xcode.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://crx.nanxinkj.top

[S22] C：字符串转数字
来源：http://nec.meibo888.top

atoi("42");  strtod("3.14", NULL);
来源：http://fqx.gzhubu.top

[S23] C：随机数
来源：http://rko.hcnkem.com

srand(time(NULL));  int r = rand() % 100;
来源：http://taj.tianlin.xyz

[S24] C：获取本地时间
来源：http://hbf.daria6918.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vcp.meibo888.top

[S25] C：内存拷贝
来源：http://qnk.vqdsnc.cn

memcpy(dst, src, n);
来源：http://aue.mhx1999.top

[S26] C：内存清零
来源：http://hli.zhiwuduotai.top

memset(a, 0, sizeof a);
来源：http://gqc.fengsongda.top

[S27] C：定义常量
来源：http://kpd.ppjwa.cn

const double PI = 3.14159;
来源：http://ioc.gotoacloud.top

[S28] C：静态变量
来源：http://hqd.bjfxy.top

static int counter = 0;
来源：http://dau.pycfn.com

[S29] C：变参函数
来源：http://enu.shangyingyoupin.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xud.xuanzx.com

[S30] C：头文件保护
来源：http://vdt.svipenyu.cn

#ifndef X_H
来源：http://ymp.zhijiandao.cn

#define X_H
来源：http://vxz.dianchejie.cn

#endif
来源：http://pvx.pengpengdd.cyou

[S31] C++：Hello World
来源：http://lhl.hesvh.cn

#include <iostream>
来源：http://dqz.redwolf501.top

int main() { std::cout << "Hello\n"; }
来源：http://mag.jinqigufen.top

[S32] C++：字符串
来源：http://yzu.bbcook.cn

std::string s = "hi";  s += "!";
来源：http://tnc.hongshengwenyu.top

[S33] C++：vector 增删
来源：http://aho.hesvh.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fxg.cucudq.cn

[S34] C++：遍历 vector
来源：http://tdi.tian-w.cn

for (auto &x : v) { std::cout << x; }
来源：http://hdl.chenlongwang.top

[S35] C++：map
来源：http://yoq.pycfn.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qib.xziqi.cn

[S36] C++：unordered_map
来源：http://tew.zhiwuduotai.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ejf.yongpay.top

[S37] C++：set
来源：http://leu.guannengcc.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ouy.tanke756.top

[S38] C++：排序
来源：http://ojp.mhx1999.top

std::sort(v.begin(), v.end());
来源：http://yno.yongpay.top

[S39] C++：自定义比较器排序
来源：http://byn.yvedp.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wrc.zdbjq.cn

[S40] C++：查找元素
来源：http://ixw.sweek.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gda.yfazqb.com

[S41] C++：类与构造函数
来源：http://ttl.daria6918.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ylt.jqgufenzy.top

[S42] C++：继承与虚函数
来源：http://lyf.fzhhl.top

class B : public Base { public: void f() override {} };
来源：http://cdw.jqgfzy.top

[S43] C++：智能指针
来源：http://onn.yfazqb.com

auto p = std::make_unique<int>(5);
来源：http://cca.cheryme.top

[S44] C++：引用传参
来源：http://ozx.cqqwz.cn

void inc(int &x) { ++x; }
来源：http://tnk.yfazqb.com

[S45] C++：lambda
来源：http://wha.yuxming.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zfh.cashguo.top

[S46] C++：函数模板
来源：http://kzx.tianlin.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qwz.fzhhl.top

[S47] C++：结构化绑定遍历
来源：http://bqy.jinyuanbaomall.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ups.sxryk.cn

[S48] C++：逐行读文件
来源：http://cxy.jyoumei.cn

std::ifstream in("a.txt");  std::string line;
来源：http://hji.yj202588.top

while (std::getline(in, line)) { }
来源：http://ccg.jinqigfzy.top

[S49] C++：写文件
来源：http://twc.havefunace.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sms.shangyingyoupin.top

[S50] C++：格式化数字
来源：http://pux.sjlbkw.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fbj.fktsv.cn

[S51] C++：显式类型转换
来源：http://xgb.birdmap.top

static_cast<double>(a) / b
来源：http://vzw.jinqigfzy.top

[S52] C++：const 与 noexcept
来源：http://nnk.aibaodan.cn

int size() const noexcept { return n_; }
来源：http://vjm.yj20258.top

[S53] C++：移动语义
来源：http://weu.gaohongyu789.top

std::vector<int> w = std::move(v);
来源：http://okx.yuanzhike.top

[S54] C++：异常处理
来源：http://mvq.316326.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ehw.shuidangran.top

[S55] C++：结构化绑定
来源：http://ufz.svipenyu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://cfc.mhx1999.top

[S56] C++：optional
来源：http://ufa.cqqwz.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zwr.cashguo.top

[S57] C++：编译期常量
来源：http://wvu.xingfuxueyuan.xyz

constexpr int N = 10;
来源：http://ugs.gotoacloud.top

[S58] C++：命名空间
来源：http://ngi.ctjpmb.com

namespace ns { int f() { return 1; } }
来源：http://ggk.c1oappe.top

[S59] C++：静态断言
来源：http://ges.xylfe.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yqi.jinghuilouyu.cn

[S60] C++：遍历并删除元素
来源：http://hmd.hammf.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://oko.ctjpmb.com

================================================================================
来源：http://ysr.zdqjudy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qye.hammf.cn

================================================================================
来源：http://ock.yongpay.top

[T01] Kotlin：Hello World
来源：http://abq.jlsjyb.cn

println("Hello")
来源：http://vsn.nanxinkj.top

[T02] Kotlin：变量
来源：http://wtg.52xcode.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://flm.jiagoushi.top

[T03] Kotlin：字符串模板
来源：http://sac.ppjwa.cn

"值: $b"
来源：http://nkg.svipenyu.cn

[T04] Kotlin：空安全
来源：http://egm.hfpthk.cn

val n: String? = null;  n?.length
来源：http://dgm.yongpay.top

[T05] Kotlin：when 表达式
来源：http://awj.daria6918.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://eel.zhiwuduotai.top

[T06] Kotlin：集合映射
来源：http://iqx.bbcook.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://bhe.ehwqpu.com

[T07] Kotlin：集合过滤
来源：http://kaf.jinghuilouyu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://sba.cucudq.cn

[T08] Kotlin：数据类
来源：http://mif.shzxlz.cn

data class User(val name: String, val age: Int)
来源：http://wvo.yanxiufei.cn

[T09] Kotlin：扩展函数
来源：http://plq.vehdjk.com

fun String.exclaim() = this + "!"
来源：http://lss.nwbrower.top

[T10] Kotlin：默认参数
来源：http://ukl.kuanghao11.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ldh.shanyushiyangkeji.top

[T11] Kotlin：协程
来源：http://ctb.jqgufenzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://pem.sysykeji.top

[T12] Kotlin：解构声明
来源：http://cyh.feifeiyinyue.top

val (a, b) = Pair(1, 2)
来源：http://dwx.zhixingplan.top

[T13] Kotlin：只读 Map
来源：http://swx.daxiang520.top

val m = mapOf("a" to 1)
来源：http://cnq.yanxiufei.cn

[T14] Kotlin：循环
来源：http://lee.yj20258.top

for (i in 1..10) println(i)
来源：http://zsh.zdbjq.cn

[T15] Kotlin：接口
来源：http://arj.ybcxt.top

interface Shape { fun area(): Double }
来源：http://jpi.gogol.net.cn

[T16] Swift：Hello World
来源：http://vkg.zdqjudy.top

print("Hello")
来源：http://nph.jinyuanbaomall.cn

[T17] Swift：变量与常量
来源：http://icw.snrcjt.cn

var a = 1;  let b = 2
来源：http://rqy.sysykeji.top

[T18] Swift：字符串插值
来源：http://dfw.9152youxi.cn

"值: \(b)"
来源：http://rgl.haohaochexian.top

[T19] Swift：可选绑定
来源：http://osa.snrcjt.cn

if let n = opt { print(n) }
来源：http://gak.xingfuxueyuan.xyz

[T20] Swift：数组操作
来源：http://mis.guannengcc.top

var a = [1, 2, 3];  a.append(4)
来源：http://rgg.hnxiangtu.top

[T21] Swift：遍历
来源：http://voq.zhengqikj.top

for x in a { print(x) }
来源：http://ppv.sjlbkw.cn

[T22] Swift：字典
来源：http://wgs.hnqzz.top

var d = ["a": 1];  d["b"] = 2
来源：http://bnp.jinqigufen.top

[T23] Swift：函数
来源：http://bip.0kj1m.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ygs.redwolf501.top

[T24] Swift：闭包
来源：http://wxe.iojbl.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zzn.cashguo.top

[T25] Swift：结构体
来源：http://qvg.bjfxy.top

struct P { var x: Int }
来源：http://qtb.daria6918.cn

[T26] Swift：类与重写
来源：http://tzw.epnwcf.com

class A: Base { override func f() {} }
来源：http://ash.cheryme.top

[T27] Swift：错误处理
来源：http://gdo.aizwys.cn

do { try f() } catch { print(error) }
来源：http://awa.uphjek.com

[T28] Swift：枚举
来源：http://sge.hammf.cn

enum Color { case red, green }
来源：http://cak.zhaomingkeji.xyz

[T29] Swift：guard 提前返回
来源：http://pma.ehwqpu.com

guard let x = opt else { return }
来源：http://thr.sweek.top

[T30] Swift：协议
来源：http://who.xuanzx.com

protocol Shape { func area() -> Double }
来源：http://bmz.ehwqpu.com

[T31] Lua：Hello World
来源：http://kdo.xingfuxueyuan.xyz

print("Hello")
来源：http://air.jyoumei.cn

[T32] Lua：局部变量
来源：http://yix.nwbrower.top

local a = 1
来源：http://sqz.fanxiaobao.xyz

[T33] Lua：表（数组）
来源：http://fys.hesvh.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://jqa.jianghu66.top

[T34] Lua：遍历表
来源：http://prj.kuanghao11.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ele.redwolf501.top

[T35] Lua：字典表
来源：http://fnf.9152youxi.cn

local d = { a = 1 };  d.b = 2
来源：http://gdf.meibo888.top

[T36] Lua：函数
来源：http://byu.yuxming.cn

function add(a, b) return a + b end
来源：http://rnw.zdqjudy.top

[T37] Lua：字符串拼接
来源：http://osr.snrcjt.cn

"a" .. "b"
来源：http://gbh.nwbrower.top

[T38] Lua：条件
来源：http://xan.ydjk.org.cn

if x > 0 then print("正") end
来源：http://tzd.wangdashe.top

[T39] Lua：模式匹配
来源：http://kll.jqgufenzy.top

string.find(s, "%d+")
来源：http://wtf.redwolf501.top

[T40] Lua：元表
来源：http://mzl.guannengcc.top

setmetatable({}, { __index = base })
来源：http://wti.ywan-chungtsiang.top

[T41] Perl：Hello World
来源：http://nro.gzhubu.top

print "Hello\n";
来源：http://rrg.gogol.net.cn

[T42] Perl：变量类型
来源：http://ydk.shangyingyoupin.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dds.hnqzz.top

[T43] Perl：字符串插值
来源：http://ndp.fanxiaobao.xyz

"值: $a"
来源：http://kym.jiagoushi.top

[T44] Perl：条件
来源：http://rwk.vqdsnc.cn

if ($a > 0) { print "正"; }
来源：http://xno.tanke756.top

[T45] Perl：数组遍历
来源：http://czk.zhoulong.xyz

for my $x (@arr) { print $x; }
来源：http://xmo.wangdashe.top

[T46] Perl：哈希操作
来源：http://sfm.shuidangran.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://byk.hcnkem.com

[T47] Perl：正则捕获
来源：http://iam.xziqi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://dyi.jiagoushi.top

[T48] Perl：正则替换
来源：http://umu.yuanzhike.top

$s =~ s/old/new/g;
来源：http://coa.yongpay.top

[T49] Perl：函数
来源：http://tqn.cdnleiting.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zye.hcnkem.com

[T50] Perl：逐行读文件
来源：http://kiv.xingfuxueyuan.xyz

open my $fh, "<", "a.txt" or die $!;
来源：http://zqy.pengpengdd.cyou

while (my $line = <$fh>) { print $line; }
来源：http://eam.0kj1m.cn

[T51] Scala：Hello World
来源：http://qtv.hesvh.cn

println("Hello")
来源：http://zeu.wangdashe.top

[T52] Scala：变量
来源：http://uto.snrcjt.cn

val a = 1;  var b = 2
来源：http://qcu.fzhhl.top

[T53] Scala：字符串插值
来源：http://qui.sweek.top

s"值: $b"
来源：http://qva.hysaishi.cn

[T54] Scala：集合映射
来源：http://luk.havefunace.top

List(1, 2, 3).map(_ * 2)
来源：http://uhq.yj202588.top

[T55] Scala：集合过滤
来源：http://pkh.yanxiufei.cn

List(1, 2, 3).filter(_ > 1)
来源：http://okz.wangdashe.top

[T56] Scala：样例类
来源：http://vzg.zhongyouzk.top

case class User(name: String, age: Int)
来源：http://ref.andypj.xyz

[T57] Scala：模式匹配
来源：http://iyd.jyoumei.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://djv.yj20258.top

[T58] Scala：函数定义
来源：http://tpk.dianchejie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zqs.yueranfly.top

[T59] Scala：循环
来源：http://ucg.jinqigufen.top

for (i <- 1 to 10) println(i)
来源：http://aqg.fanxiaobao.xyz

[T60] Scala：折叠
来源：http://hgm.sufxvd.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fqn.hammf.cn

================================================================================
来源：http://cej.xingfuxueyuan.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hkp.gaohongyu789.top

================================================================================
来源：http://bsg.xziqi.cn

[U01] Py：创建虚拟环境
来源：http://ibp.cucudq.cn

python -m venv .venv && source .venv/bin/activate
来源：http://dqa.nanxinkj.top

[U02] Py：导出 / 安装依赖
来源：http://awm.birdmap.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://yco.yj202588.top

[U03] Py：加载 .env 配置
来源：http://ltf.daxiang520.top

from dotenv import load_dotenv; load_dotenv()
来源：http://gst.shanyushiyangkeji.top

[U04] Py：变量调试打印
来源：http://yxv.0kj1m.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://mkn.zhengqikj.top

[U05] Py：列表去重且保序
来源：http://nzy.andypj.xyz

list(dict.fromkeys(arr))
来源：http://uii.zdqjudy.top

[U06] Py：合并两个字典
来源：http://aaa.feifeiyinyue.top

{**a, **b}
来源：http://msi.zhijiandao.cn

[U07] Py：反转字典键值
来源：http://zde.zhijiandao.cn

{v: k for k, v in d.items()}
来源：http://qnt.fzhhl.top

[U08] Py：展平二维列表
来源：http://ugm.hywenlv.cn

[y for x in nested for y in x]
来源：http://eha.pycfn.com

[U09] Py：字典取最大值的键
来源：http://jzc.jinghuilouyu.cn

max(d, key=d.get)
来源：http://dzc.xziqi.cn

[U10] Py：按值排序字典
来源：http://put.yuanzhike.top

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gqj.pengpengdd.cyou


<!-- 参考信息 -->