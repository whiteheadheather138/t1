代发 wailian999

openssl rand -hex 16
来源：http://vvf.zhongyouzk.top

[R68] 计算文件校验值
来源：http://jju.jinqigfzy.top

sha256sum a.txt;  md5sum a.txt
来源：http://saa.hcnkem.com

[R69] 生成随机密码
来源：http://yjk.fzhhl.top

head -c 16 /dev/urandom | base64
来源：http://pqp.daria6918.cn

[R70] 时间戳与互转
来源：http://hfx.yj20258888.top

date +%s;  date -d @1700000000
来源：http://pfk.ywan-chungtsiang.top

[R71] 日期格式化
来源：http://dhq.yongpay.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://jvs.tianlin.xyz

[R72] 等待端口就绪
来源：http://hbe.sufxvd.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://nvn.jinyuanbaomall.cn

[R73] 分割大日志
来源：http://dbv.yvedp.cn

split -l 1000 big.log part_
来源：http://tjz.sufxvd.cn

[R74] 批量重命名
来源：http://fju.0kj1m.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qto.bjfxy.top

[R75] 导出环境变量
来源：http://bsb.ehwqpu.com

export PATH="$HOME/bin:$PATH"
来源：http://lew.yueranfly.top

[R76] 使用临时文件
来源：http://tug.xuetiantiany.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wcf.nanxuanxn.top

[R77] 读取用户输入
来源：http://knr.chenlongwang.top

read -rp "请输入: " ans
来源：http://zdh.nanxuanxn.top

[R78] 交互式菜单
来源：http://twv.kuanghao11.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://asv.yj20258.top

[R79] 解析命令行选项
来源：http://jfa.sjlbkw.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dsv.kuanghao11.cn

[R80] 查看脚本执行耗时
来源：http://eks.xuetiantiany.cn

time ./run.sh
来源：http://tld.iojbl.cn

================================================================================
来源：http://rsu.fanxiaobao.xyz

S. C / C++ 专题
来源：http://hwm.tarul.cn

================================================================================
来源：http://nve.pycfn.com

[S01] C：Hello World
来源：http://wxn.jinghuilouyu.cn

#include <stdio.h>
来源：http://rfd.52xcode.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://wfv.sysykeji.top

[S02] C：变量与格式化输出
来源：http://uhn.vqdsnc.cn

int a = 10; printf("%d\n", a);
来源：http://ljp.wangdashe.top

[S03] C：读入整数
来源：http://dqb.shanyushiyangtech.top

int x; scanf("%d", &x);
来源：http://zgd.kuanghao11.cn

[S04] C：字符串复制
来源：http://gnq.chenjidiqi.icu

char dst[32]; strcpy(dst, "hi");
来源：http://wib.yuanzhike.top

[S05] C：字符串长度
来源：http://jxs.wangdashe.top

strlen(s)
来源：http://lob.gotoacloud.top

[S06] C：字符串比较
来源：http://ovj.chenlongwang.top

strcmp(a, b) == 0
来源：http://spj.vehdjk.com

[S07] C：数组遍历求和
来源：http://lzz.ivvv.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://epr.xylfe.cn

[S08] C：动态内存分配与释放
来源：http://hqw.yuanzhike.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://txu.yangfankeji.com

[S09] C：结构体定义与初始化
来源：http://vjq.yfazqb.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mor.yuxming.cn

[S10] C：指针与解引用
来源：http://tmf.xinyue.icu

int *p = &a;  *p = 5;
来源：http://ehx.guannengcc.top

[S11] C：逐行读文件
来源：http://bmr.gaohongyu789.top

FILE *f = fopen("a.txt", "r");
来源：http://fvu.jinqigufen.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://tii.andypj.xyz

fclose(f);
来源：http://dpd.zhengqikj.top

[S12] C：写文件
来源：http://dot.bbcook.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xtl.vqdsnc.cn

[S13] C：宏定义
来源：http://juk.dianchejie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tzh.ctjpmb.com

[S14] C：枚举
来源：http://kys.dashuyun.cn

enum Color { RED, GREEN, BLUE };
来源：http://lzv.uphjek.com

[S15] C：类型转换
来源：http://yfo.yonumen.top

(double) a / b
来源：http://cdz.bjfxy.top

[S16] C：位操作置位
来源：http://hcj.jianghu66.top

x |= (1 << 3);
来源：http://hfm.9152youxi.cn

[S17] C：安全拼接字符串
来源：http://xfg.ywan-chungtsiang.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qey.c1oappe.top

[S18] C：命令行参数
来源：http://gcu.jinqigfzy.top

int main(int argc, char **argv)
来源：http://iqp.sysykeji.top

[S19] C：快速排序
来源：http://vyw.hysaishi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ftm.xuanzx.com

[S20] C：二分查找
来源：http://qya.gzhubu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://irb.xuetiantiany.cn

[S21] C：字符类别判断
来源：http://klt.ehwqpu.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://uyw.xinyue.icu

[S22] C：字符串转数字
来源：http://mno.pengpengdd.cyou

atoi("42");  strtod("3.14", NULL);
来源：http://she.0kj1m.cn

[S23] C：随机数
来源：http://cih.gotoacloud.top

srand(time(NULL));  int r = rand() % 100;
来源：http://frr.chenjidiqi.icu

[S24] C：获取本地时间
来源：http://ifg.feifeiyinyue.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gaf.zhoulong.xyz

[S25] C：内存拷贝
来源：http://end.jlsjyb.cn

memcpy(dst, src, n);
来源：http://rxa.fanxiaobao.xyz

[S26] C：内存清零
来源：http://ira.shanyushiyangkeji.top

memset(a, 0, sizeof a);
来源：http://goc.birdmap.top

[S27] C：定义常量
来源：http://dvo.cqqwz.cn

const double PI = 3.14159;
来源：http://vme.shangyingyoupin.top

[S28] C：静态变量
来源：http://klw.daria6918.cn

static int counter = 0;
来源：http://npc.sufxvd.cn

[S29] C：变参函数
来源：http://ywz.mhx1999.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://txj.nwbrower.top

[S30] C：头文件保护
来源：http://fzc.cdnleiting.top

#ifndef X_H
来源：http://mkm.ybcxt.top

#define X_H
来源：http://wgr.mhx1999.top

#endif
来源：http://zjt.9152youxi.cn

[S31] C++：Hello World
来源：http://bfm.sjlbkw.cn

#include <iostream>
来源：http://wgw.yj20258.top

int main() { std::cout << "Hello\n"; }
来源：http://hws.hfpthk.cn

[S32] C++：字符串
来源：http://qta.vehdjk.com

std::string s = "hi";  s += "!";
来源：http://hvx.gogol.net.cn

[S33] C++：vector 增删
来源：http://qpt.jlsjyb.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bhy.c1oappe.top

[S34] C++：遍历 vector
来源：http://mgl.fehbvm.com

for (auto &x : v) { std::cout << x; }
来源：http://tcv.jinghuilouyu.cn

[S35] C++：map
来源：http://izu.fanxiaobao.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cax.dianchejie.cn

[S36] C++：unordered_map
来源：http://nnw.jinqigufen.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lun.mhx1999.top

[S37] C++：set
来源：http://pvx.zdbjq.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ckj.bjfxy.top

[S38] C++：排序
来源：http://pin.daria6918.cn

std::sort(v.begin(), v.end());
来源：http://cqc.ppjwa.cn

[S39] C++：自定义比较器排序
来源：http://sdq.fanxiaobao.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ahq.jiagoushi.top

[S40] C++：查找元素
来源：http://pgk.shzxlz.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cdw.xuanzx.com

[S41] C++：类与构造函数
来源：http://cbw.zhiwuduotai.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vqi.zhongyouzk.top

[S42] C++：继承与虚函数
来源：http://gex.jyoumei.cn

class B : public Base { public: void f() override {} };
来源：http://wdc.ivvv.top

[S43] C++：智能指针
来源：http://eba.yongpay.top

auto p = std::make_unique<int>(5);
来源：http://awy.xylfe.cn

[S44] C++：引用传参
来源：http://gay.cashguo.top

void inc(int &x) { ++x; }
来源：http://fjj.hesvh.cn

[S45] C++：lambda
来源：http://dsv.jinghuilouyu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ajg.dianchejie.cn

[S46] C++：函数模板
来源：http://vyv.andypj.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xgl.zhengqikj.top

[S47] C++：结构化绑定遍历
来源：http://ucb.gogol.net.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xpd.xuanzx.com

[S48] C++：逐行读文件
来源：http://rbv.hongshengwenyu.top

std::ifstream in("a.txt");  std::string line;
来源：http://lbq.yvedp.cn

while (std::getline(in, line)) { }
来源：http://zrn.zhijiandao.cn

[S49] C++：写文件
来源：http://gye.yj20258888.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://eon.hnqzz.top

[S50] C++：格式化数字
来源：http://tht.ydzc1.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uyr.shanyushiyangtech.top

[S51] C++：显式类型转换
来源：http://ydl.fehbvm.com

static_cast<double>(a) / b
来源：http://wip.ywan-chungtsiang.top

[S52] C++：const 与 noexcept
来源：http://imk.zhongyouzk.top

int size() const noexcept { return n_; }
来源：http://ibp.jinyuanbaomall.cn

[S53] C++：移动语义
来源：http://kpc.jyoumei.cn

std::vector<int> w = std::move(v);
来源：http://lov.vqdsnc.cn

[S54] C++：异常处理
来源：http://tae.hfpthk.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qpu.ctjpmb.com

[S55] C++：结构化绑定
来源：http://kvg.shangyingyoupin.top

auto [a, b] = std::make_pair(1, 2);
来源：http://sjn.ywan-chungtsiang.top

[S56] C++：optional
来源：http://xbn.nanxinkj.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lyb.andypj.xyz

[S57] C++：编译期常量
来源：http://jku.daria6918.cn

constexpr int N = 10;
来源：http://pel.sjlbkw.cn

[S58] C++：命名空间
来源：http://ges.pycfn.com

namespace ns { int f() { return 1; } }
来源：http://phb.jianghu66.top

[S59] C++：静态断言
来源：http://dqs.meibo888.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lgc.zycfv.cn

[S60] C++：遍历并删除元素
来源：http://knx.andypj.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pxq.jinyuanbaomall.cn

================================================================================
来源：http://hio.tarul.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gug.9152youxi.cn

================================================================================
来源：http://oqp.gzhubu.top

[T01] Kotlin：Hello World
来源：http://vfg.haohaochexian.top

println("Hello")
来源：http://nty.kuanghao11.cn

[T02] Kotlin：变量
来源：http://qzi.hysaishi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ggb.fanxiaobao.xyz

[T03] Kotlin：字符串模板
来源：http://njz.aizwys.cn

"值: $b"
来源：http://vbq.yanxiufei.cn

[T04] Kotlin：空安全
来源：http://wkg.shanyushiyangkeji.top

val n: String? = null;  n?.length
来源：http://yvu.hnxiangtu.top

[T05] Kotlin：when 表达式
来源：http://zyj.zhaomingkeji.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kuo.aibaodan.cn

[T06] Kotlin：集合映射
来源：http://jpg.gzhubu.top

listOf(1, 2, 3).map { it * 2 }
来源：http://kcs.yonumen.top

[T07] Kotlin：集合过滤
来源：http://jfz.tarul.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://exm.hnxiangtu.top

[T08] Kotlin：数据类
来源：http://fbk.52xcode.cn

data class User(val name: String, val age: Int)
来源：http://ilq.gzhubu.top

[T09] Kotlin：扩展函数
来源：http://xzc.zhaomingkeji.xyz

fun String.exclaim() = this + "!"
来源：http://ges.guowangkeji.top

[T10] Kotlin：默认参数
来源：http://onw.yj202588.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ypz.iojbl.cn

[T11] Kotlin：协程
来源：http://akh.tarul.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://yyh.birdmap.top

[T12] Kotlin：解构声明
来源：http://bvy.zhijiandao.cn

val (a, b) = Pair(1, 2)
来源：http://try.fanxiaobao.xyz

[T13] Kotlin：只读 Map
来源：http://sqk.tianlin.xyz

val m = mapOf("a" to 1)
来源：http://nkx.hnxiangtu.top

[T14] Kotlin：循环
来源：http://mzk.birdmap.top

for (i in 1..10) println(i)
来源：http://haz.kuanghao11.cn

[T15] Kotlin：接口
来源：http://vtj.hongshengwenyu.top

interface Shape { fun area(): Double }
来源：http://syn.guowangkeji.top

[T16] Swift：Hello World
来源：http://gau.redwolf501.top

print("Hello")
来源：http://lck.jqgufenzy.top

[T17] Swift：变量与常量
来源：http://iaq.hnqzz.top

var a = 1;  let b = 2
来源：http://klv.ivvv.top

[T18] Swift：字符串插值
来源：http://rzk.ydzc1.top

"值: \(b)"
来源：http://ndl.epnwcf.com

[T19] Swift：可选绑定
来源：http://mvy.uphjek.com

if let n = opt { print(n) }
来源：http://dlf.iojbl.cn

[T20] Swift：数组操作
来源：http://tvd.chenjidiqi.icu

var a = [1, 2, 3];  a.append(4)
来源：http://yzw.yj20258.top

[T21] Swift：遍历
来源：http://gku.0kj1m.cn

for x in a { print(x) }
来源：http://lcx.feifeiyinyue.top

[T22] Swift：字典
来源：http://fxq.ehwqpu.com

var d = ["a": 1];  d["b"] = 2
来源：http://kyt.zhixingplan.top

[T23] Swift：函数
来源：http://aar.sxryk.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lqy.gzhubu.top

[T24] Swift：闭包
来源：http://pgc.xinyue.icu

let f = { (x: Int) -> Int in x * 2 }
来源：http://sya.xinyue.icu

[T25] Swift：结构体
来源：http://rud.hywenlv.cn

struct P { var x: Int }
来源：http://uqo.nanxinkj.top

[T26] Swift：类与重写
来源：http://lok.aibaodan.cn

class A: Base { override func f() {} }
来源：http://efi.jqgufenzy.top

[T27] Swift：错误处理
来源：http://cmu.shanyushiyangtech.top

do { try f() } catch { print(error) }
来源：http://pkq.tanke756.top

[T28] Swift：枚举
来源：http://ntx.shanyushiyangtech.top

enum Color { case red, green }
来源：http://vua.nanxinkj.top

[T29] Swift：guard 提前返回
来源：http://krs.pengpengdd.cyou

guard let x = opt else { return }
来源：http://blc.vehdjk.com

[T30] Swift：协议
来源：http://tne.guowangkeji.top

protocol Shape { func area() -> Double }
来源：http://tlj.yuxming.cn

[T31] Lua：Hello World
来源：http://ipe.gzhubu.top

print("Hello")
来源：http://wba.yuanzhike.top

[T32] Lua：局部变量
来源：http://jmh.sufxvd.cn

local a = 1
来源：http://khq.xylfe.cn

[T33] Lua：表（数组）
来源：http://kxk.nanxuanxn.top

local t = {1, 2, 3};  t[4] = 4
来源：http://unh.yvedp.cn

[T34] Lua：遍历表
来源：http://tfl.jinghuilouyu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://mvv.0kj1m.cn

[T35] Lua：字典表
来源：http://rgg.yvedp.cn

local d = { a = 1 };  d.b = 2
来源：http://qdx.bbcook.cn

[T36] Lua：函数
来源：http://fwp.ppjwa.cn

function add(a, b) return a + b end
来源：http://ayx.pengpengdd.cyou

[T37] Lua：字符串拼接
来源：http://krf.xuetiantiany.cn

"a" .. "b"
来源：http://ade.iojbl.cn

[T38] Lua：条件
来源：http://ibt.daxiang520.top

if x > 0 then print("正") end
来源：http://xdl.guowangkeji.top

[T39] Lua：模式匹配
来源：http://alt.52xcode.cn

string.find(s, "%d+")
来源：http://wrs.fanxiaobao.xyz

[T40] Lua：元表
来源：http://weu.jinqigufen.top

setmetatable({}, { __index = base })
来源：http://tni.zhixingplan.top

[T41] Perl：Hello World
来源：http://wfv.jinghuilouyu.cn

print "Hello\n";
来源：http://itp.yonumen.top

[T42] Perl：变量类型
来源：http://pki.xuetiantiany.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tna.dianchejie.cn

[T43] Perl：字符串插值
来源：http://rha.dashuyun.cn

"值: $a"
来源：http://vso.bbcook.cn

[T44] Perl：条件
来源：http://ken.jinqigufen.top

if ($a > 0) { print "正"; }
来源：http://bxt.sxryk.cn

[T45] Perl：数组遍历
来源：http://cys.shanyushiyangtech.top

for my $x (@arr) { print $x; }
来源：http://nbi.c1oappe.top

[T46] Perl：哈希操作
来源：http://djv.xinyue.icu

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://icu.zhijiandao.cn

[T47] Perl：正则捕获
来源：http://pgs.xingfuxueyuan.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://roo.jinqigfzy.top

[T48] Perl：正则替换
来源：http://mci.aibaodan.cn

$s =~ s/old/new/g;
来源：http://ztc.svipenyu.cn

[T49] Perl：函数
来源：http://ckg.hywenlv.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lkm.xingfuxueyuan.xyz

[T50] Perl：逐行读文件
来源：http://ali.nanxinkj.top

open my $fh, "<", "a.txt" or die $!;
来源：http://avh.0kj1m.cn

while (my $line = <$fh>) { print $line; }
来源：http://bdl.hfpthk.cn

[T51] Scala：Hello World
来源：http://gvg.fzhhl.top

println("Hello")
来源：http://dno.52xcode.cn

[T52] Scala：变量
来源：http://zkf.ywan-chungtsiang.top

val a = 1;  var b = 2
来源：http://hlq.jqgufenzy.top

[T53] Scala：字符串插值
来源：http://wsv.yangfankeji.com

s"值: $b"
来源：http://tbs.pycfn.com

[T54] Scala：集合映射
来源：http://xaz.zhongyouzk.top

List(1, 2, 3).map(_ * 2)
来源：http://wlc.iojbl.cn

[T55] Scala：集合过滤
来源：http://pxr.hammf.cn

List(1, 2, 3).filter(_ > 1)
来源：http://acl.redwolf501.top

[T56] Scala：样例类
来源：http://act.dashuyun.cn

case class User(name: String, age: Int)
来源：http://oxe.yueranfly.top

[T57] Scala：模式匹配
来源：http://fpq.zhiwuduotai.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://nyk.wangshuangyany.cn

[T58] Scala：函数定义
来源：http://jlc.shzxlz.cn

def add(a: Int, b: Int): Int = a + b
来源：http://oie.cdnleiting.top

[T59] Scala：循环
来源：http://vwy.yangfankeji.com

for (i <- 1 to 10) println(i)
来源：http://grq.xziqi.cn

[T60] Scala：折叠
来源：http://jte.zhongyouzk.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fck.epnwcf.com

================================================================================
来源：http://ecd.xuanzx.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nzw.hnqzz.top

================================================================================
来源：http://hie.hfpthk.cn

[U01] Py：创建虚拟环境
来源：http://xbw.ppjwa.cn

python -m venv .venv && source .venv/bin/activate
来源：http://urv.feifeiyinyue.top

[U02] Py：导出 / 安装依赖
来源：http://ukg.yanxiufei.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ufb.zhixingplan.top

[U03] Py：加载 .env 配置
来源：http://nmr.zhiwuduotai.top

from dotenv import load_dotenv; load_dotenv()
来源：http://mak.yfazqb.com

[U04] Py：变量调试打印
来源：http://ipe.ydjk.org.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jjl.shuidangran.top

[U05] Py：列表去重且保序
来源：http://eul.zdqjudy.top

list(dict.fromkeys(arr))
来源：http://tbs.kuanghao11.cn

[U06] Py：合并两个字典
来源：http://lhn.pengpengdd.cyou

{**a, **b}
来源：http://zef.yj20258888.top

[U07] Py：反转字典键值
来源：http://sgl.yonumen.top

{v: k for k, v in d.items()}
来源：http://iwt.birdmap.top

[U08] Py：展平二维列表
来源：http://gyz.cucudq.cn

[y for x in nested for y in x]
来源：http://uos.uphjek.com


<!-- 参考信息 -->