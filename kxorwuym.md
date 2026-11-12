代发 wailian999

openssl rand -hex 16
来源：http://vse.yj20258.top

[R68] 计算文件校验值
来源：http://rtj.xingfuxueyuan.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://njo.nanxinkj.top

[R69] 生成随机密码
来源：http://ysq.xuetiantiany.cn

head -c 16 /dev/urandom | base64
来源：http://rrw.gaohongyu789.top

[R70] 时间戳与互转
来源：http://wjq.meibo888.top

date +%s;  date -d @1700000000
来源：http://ysx.sufxvd.cn

[R71] 日期格式化
来源：http://rfb.zdbjq.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://nmq.gzhubu.top

[R72] 等待端口就绪
来源：http://fhk.xingfuxueyuan.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://nli.zdbjq.cn

[R73] 分割大日志
来源：http://nln.shanyushiyangkeji.top

split -l 1000 big.log part_
来源：http://tul.ydzc1.top

[R74] 批量重命名
来源：http://bug.wangdashe.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pas.gaohongyu789.top

[R75] 导出环境变量
来源：http://uxh.yvedp.cn

export PATH="$HOME/bin:$PATH"
来源：http://ags.xingfuxueyuan.xyz

[R76] 使用临时文件
来源：http://ocd.fzhhl.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://grb.jinghuilouyu.cn

[R77] 读取用户输入
来源：http://ojy.quarkkingdee.top

read -rp "请输入: " ans
来源：http://egs.yfazqb.com

[R78] 交互式菜单
来源：http://ajp.chenjidiqi.icu

select opt in a b c; do echo "$opt"; break; done
来源：http://uui.sufxvd.cn

[R79] 解析命令行选项
来源：http://yos.jinghuilouyu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://suj.chenlongwang.top

[R80] 查看脚本执行耗时
来源：http://wdi.tian-w.cn

time ./run.sh
来源：http://hcu.yuxming.cn

================================================================================
来源：http://ysl.snrcjt.cn

S. C / C++ 专题
来源：http://toa.gogol.net.cn

================================================================================
来源：http://enc.cdnleiting.top

[S01] C：Hello World
来源：http://mlj.epnwcf.com

#include <stdio.h>
来源：http://edq.yangfankeji.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://prs.yfazqb.com

[S02] C：变量与格式化输出
来源：http://nmi.fanxiaobao.xyz

int a = 10; printf("%d\n", a);
来源：http://fht.nanxuanxn.top

[S03] C：读入整数
来源：http://ngc.svipenyu.cn

int x; scanf("%d", &x);
来源：http://lcp.kuanghao11.cn

[S04] C：字符串复制
来源：http://fqo.tarul.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jef.zhongyouzk.top

[S05] C：字符串长度
来源：http://ezz.fzhhl.top

strlen(s)
来源：http://yvq.snrcjt.cn

[S06] C：字符串比较
来源：http://ywx.jyoumei.cn

strcmp(a, b) == 0
来源：http://zqn.ywan-chungtsiang.top

[S07] C：数组遍历求和
来源：http://mpi.sysykeji.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://acv.tanke756.top

[S08] C：动态内存分配与释放
来源：http://kvu.smart0.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cxl.sysykeji.top

[S09] C：结构体定义与初始化
来源：http://qbn.pengpengdd.cyou

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tzi.cheryme.top

[S10] C：指针与解引用
来源：http://dmo.vehdjk.com

int *p = &a;  *p = 5;
来源：http://lab.nanxuanxn.top

[S11] C：逐行读文件
来源：http://vwc.hysaishi.cn

FILE *f = fopen("a.txt", "r");
来源：http://chi.yj20258.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://vhq.chenjidiqi.icu

fclose(f);
来源：http://kkm.chenlongwang.top

[S12] C：写文件
来源：http://vzg.aizwys.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jhp.hfpthk.cn

[S13] C：宏定义
来源：http://pvc.vqdsnc.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ita.cucudq.cn

[S14] C：枚举
来源：http://vlw.shanyushiyangtech.top

enum Color { RED, GREEN, BLUE };
来源：http://qer.jinqigufen.top

[S15] C：类型转换
来源：http://wrw.epnwcf.com

(double) a / b
来源：http://kcf.ppjwa.cn

[S16] C：位操作置位
来源：http://jlo.iojbl.cn

x |= (1 << 3);
来源：http://ewh.nanxinkj.top

[S17] C：安全拼接字符串
来源：http://wby.zhoulong.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ohg.yuanzhike.top

[S18] C：命令行参数
来源：http://dsh.jinqigufen.top

int main(int argc, char **argv)
来源：http://zxg.sjlbkw.cn

[S19] C：快速排序
来源：http://akg.cdnleiting.top

qsort(a, n, sizeof(int), cmp);
来源：http://uxx.shzxlz.cn

[S20] C：二分查找
来源：http://boa.wangdashe.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gzl.hammf.cn

[S21] C：字符类别判断
来源：http://nbz.yanxiufei.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://uyw.daria6918.cn

[S22] C：字符串转数字
来源：http://mai.316326.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://kag.quarkkingdee.top

[S23] C：随机数
来源：http://wbq.yuanzhike.top

srand(time(NULL));  int r = rand() % 100;
来源：http://iqy.zhoulong.xyz

[S24] C：获取本地时间
来源：http://hpo.hnqzz.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ilf.kuanghao11.cn

[S25] C：内存拷贝
来源：http://esl.guannengcc.top

memcpy(dst, src, n);
来源：http://wux.jinghuilouyu.cn

[S26] C：内存清零
来源：http://qiq.haohaochexian.top

memset(a, 0, sizeof a);
来源：http://znk.guowangkeji.top

[S27] C：定义常量
来源：http://rbq.yanxiufei.cn

const double PI = 3.14159;
来源：http://cgq.ivvv.top

[S28] C：静态变量
来源：http://lln.hammf.cn

static int counter = 0;
来源：http://cfi.chenjidiqi.icu

[S29] C：变参函数
来源：http://eoc.ybcxt.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://emv.sjlbkw.cn

[S30] C：头文件保护
来源：http://haz.shanyushiyangtech.top

#ifndef X_H
来源：http://dda.fanxiaobao.xyz

#define X_H
来源：http://xeh.sysykeji.top

#endif
来源：http://yhb.ydjk.org.cn

[S31] C++：Hello World
来源：http://hsf.yuanzhike.top

#include <iostream>
来源：http://mpw.bbcook.cn

int main() { std::cout << "Hello\n"; }
来源：http://lln.yj20258888.top

[S32] C++：字符串
来源：http://nyb.ehwqpu.com

std::string s = "hi";  s += "!";
来源：http://pkh.bjfxy.top

[S33] C++：vector 增删
来源：http://red.hongshengwenyu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mql.feifeiyinyue.top

[S34] C++：遍历 vector
来源：http://wmj.shangyingyoupin.top

for (auto &x : v) { std::cout << x; }
来源：http://vfp.redwolf501.top

[S35] C++：map
来源：http://cqy.aizwys.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gzb.9152youxi.cn

[S36] C++：unordered_map
来源：http://evz.c1oappe.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://iai.daxiang520.top

[S37] C++：set
来源：http://hlw.zhaomingkeji.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wll.cheryme.top

[S38] C++：排序
来源：http://tkc.quarkkingdee.top

std::sort(v.begin(), v.end());
来源：http://zhy.shuidangran.top

[S39] C++：自定义比较器排序
来源：http://yod.yangfankeji.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fwo.tanke756.top

[S40] C++：查找元素
来源：http://hmp.nanxuanxn.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://urp.fengsongda.top

[S41] C++：类与构造函数
来源：http://lzw.cucudq.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wgq.zhaomingkeji.xyz

[S42] C++：继承与虚函数
来源：http://itd.jinqigfzy.top

class B : public Base { public: void f() override {} };
来源：http://dcu.jianghu66.top

[S43] C++：智能指针
来源：http://oaj.aizwys.cn

auto p = std::make_unique<int>(5);
来源：http://fuy.pengpengdd.cyou

[S44] C++：引用传参
来源：http://wir.feifeiyinyue.top

void inc(int &x) { ++x; }
来源：http://tkt.smart0.xyz

[S45] C++：lambda
来源：http://hjl.daria6918.cn

auto add = [](int a, int b) { return a + b; };
来源：http://jmm.havefunace.top

[S46] C++：函数模板
来源：http://bne.yj20258.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://art.jinqigfzy.top

[S47] C++：结构化绑定遍历
来源：http://jym.shangyingyoupin.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sda.kuanghao11.cn

[S48] C++：逐行读文件
来源：http://adr.cucudq.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vnx.ywan-chungtsiang.top

while (std::getline(in, line)) { }
来源：http://lmh.gzhubu.top

[S49] C++：写文件
来源：http://txq.tian-w.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bzn.nanxinkj.top

[S50] C++：格式化数字
来源：http://obo.yonumen.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tzl.jlsjyb.cn

[S51] C++：显式类型转换
来源：http://sgb.yj20258888.top

static_cast<double>(a) / b
来源：http://vdw.cdnleiting.top

[S52] C++：const 与 noexcept
来源：http://ezt.svipenyu.cn

int size() const noexcept { return n_; }
来源：http://pbd.aizwys.cn

[S53] C++：移动语义
来源：http://bec.andypj.xyz

std::vector<int> w = std::move(v);
来源：http://pfw.yj202588.top

[S54] C++：异常处理
来源：http://axo.cheryme.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tlu.zycfv.cn

[S55] C++：结构化绑定
来源：http://zsk.ydjk.org.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://pxp.dashuyun.cn

[S56] C++：optional
来源：http://iau.ywan-chungtsiang.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ify.sweek.top

[S57] C++：编译期常量
来源：http://veh.cdnleiting.top

constexpr int N = 10;
来源：http://prp.gogol.net.cn

[S58] C++：命名空间
来源：http://xyr.zdqjudy.top

namespace ns { int f() { return 1; } }
来源：http://kcb.zhaomingkeji.xyz

[S59] C++：静态断言
来源：http://dri.jlsjyb.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lpb.guowangkeji.top

[S60] C++：遍历并删除元素
来源：http://suu.svipenyu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://foo.wangdashe.top

================================================================================
来源：http://tpi.sjlbkw.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://haj.yvedp.cn

================================================================================
来源：http://jqe.sxryk.cn

[T01] Kotlin：Hello World
来源：http://lcq.c1oappe.top

println("Hello")
来源：http://fqs.nanxuanxn.top

[T02] Kotlin：变量
来源：http://ckz.yfazqb.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://icp.zdqjudy.top

[T03] Kotlin：字符串模板
来源：http://gca.quarkkingdee.top

"值: $b"
来源：http://gxy.jqgfzy.top

[T04] Kotlin：空安全
来源：http://ggs.dashuyun.cn

val n: String? = null;  n?.length
来源：http://ghg.feifeiyinyue.top

[T05] Kotlin：when 表达式
来源：http://ylb.yj202588.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ugj.yvedp.cn

[T06] Kotlin：集合映射
来源：http://eyv.hnqzz.top

listOf(1, 2, 3).map { it * 2 }
来源：http://tak.tian-w.cn

[T07] Kotlin：集合过滤
来源：http://gtb.ivvv.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://aer.redwolf501.top

[T08] Kotlin：数据类
来源：http://bxs.xinyue.icu

data class User(val name: String, val age: Int)
来源：http://ehf.wangshuangyany.cn

[T09] Kotlin：扩展函数
来源：http://njy.feifeiyinyue.top

fun String.exclaim() = this + "!"
来源：http://nbp.quarkkingdee.top

[T10] Kotlin：默认参数
来源：http://cdo.hammf.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://izo.ctjpmb.com

[T11] Kotlin：协程
来源：http://hoz.hnxiangtu.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://wyk.guannengcc.top

[T12] Kotlin：解构声明
来源：http://wuz.pengpengdd.cyou

val (a, b) = Pair(1, 2)
来源：http://hlc.sysykeji.top

[T13] Kotlin：只读 Map
来源：http://kqq.guowangkeji.top

val m = mapOf("a" to 1)
来源：http://nez.cdnleiting.top

[T14] Kotlin：循环
来源：http://wee.dianchejie.cn

for (i in 1..10) println(i)
来源：http://itv.cdnleiting.top

[T15] Kotlin：接口
来源：http://csj.9152youxi.cn

interface Shape { fun area(): Double }
来源：http://gns.daria6918.cn

[T16] Swift：Hello World
来源：http://era.bbcook.cn

print("Hello")
来源：http://qmg.ppjwa.cn

[T17] Swift：变量与常量
来源：http://nzh.bjfxy.top

var a = 1;  let b = 2
来源：http://usf.dianchejie.cn

[T18] Swift：字符串插值
来源：http://rkb.zycfv.cn

"值: \(b)"
来源：http://ijg.hnqzz.top

[T19] Swift：可选绑定
来源：http://cri.chenlongwang.top

if let n = opt { print(n) }
来源：http://lus.cdnleiting.top

[T20] Swift：数组操作
来源：http://qgm.guowangkeji.top

var a = [1, 2, 3];  a.append(4)
来源：http://big.chenjidiqi.icu

[T21] Swift：遍历
来源：http://spw.guowangkeji.top

for x in a { print(x) }
来源：http://xem.tanke756.top

[T22] Swift：字典
来源：http://tst.ydjk.org.cn

var d = ["a": 1];  d["b"] = 2
来源：http://udy.shanyushiyangtech.top

[T23] Swift：函数
来源：http://pfp.dianchejie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ihm.zhijiandao.cn

[T24] Swift：闭包
来源：http://qya.ehwqpu.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://pju.ctjpmb.com

[T25] Swift：结构体
来源：http://wqv.fengsongda.top

struct P { var x: Int }
来源：http://qli.hnxiangtu.top

[T26] Swift：类与重写
来源：http://dlf.jyoumei.cn

class A: Base { override func f() {} }
来源：http://ylp.xylfe.cn

[T27] Swift：错误处理
来源：http://kky.fengsongda.top

do { try f() } catch { print(error) }
来源：http://gqd.sxryk.cn

[T28] Swift：枚举
来源：http://bvj.tarul.cn

enum Color { case red, green }
来源：http://ftg.gzhubu.top

[T29] Swift：guard 提前返回
来源：http://ysk.gotoacloud.top

guard let x = opt else { return }
来源：http://mve.wangdashe.top

[T30] Swift：协议
来源：http://yfi.jinqigfzy.top

protocol Shape { func area() -> Double }
来源：http://ubc.yvedp.cn

[T31] Lua：Hello World
来源：http://cqh.fengsongda.top

print("Hello")
来源：http://kek.meibo888.top

[T32] Lua：局部变量
来源：http://rer.yj20258888.top

local a = 1
来源：http://fmz.ehwqpu.com

[T33] Lua：表（数组）
来源：http://jhg.9152youxi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://nrz.aizwys.cn

[T34] Lua：遍历表
来源：http://ncc.yonumen.top

for i, v in ipairs(t) do print(i, v) end
来源：http://yvg.jqgfzy.top

[T35] Lua：字典表
来源：http://enq.aibaodan.cn

local d = { a = 1 };  d.b = 2
来源：http://xiz.yonumen.top

[T36] Lua：函数
来源：http://oey.hesvh.cn

function add(a, b) return a + b end
来源：http://wbx.yfazqb.com

[T37] Lua：字符串拼接
来源：http://nvq.hammf.cn

"a" .. "b"
来源：http://ykt.yongpay.top

[T38] Lua：条件
来源：http://lcv.feifeiyinyue.top

if x > 0 then print("正") end
来源：http://kwk.yj20258.top

[T39] Lua：模式匹配
来源：http://mxc.zhongyouzk.top

string.find(s, "%d+")
来源：http://lyc.tianlin.xyz

[T40] Lua：元表
来源：http://vss.tarul.cn

setmetatable({}, { __index = base })
来源：http://tel.snrcjt.cn

[T41] Perl：Hello World
来源：http://yca.bbcook.cn

print "Hello\n";
来源：http://sdu.jinyuanbaomall.cn

[T42] Perl：变量类型
来源：http://uvf.316326.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vgn.xuanzx.com

[T43] Perl：字符串插值
来源：http://dlo.52xcode.cn

"值: $a"
来源：http://shh.uphjek.com

[T44] Perl：条件
来源：http://jpe.jinqigfzy.top

if ($a > 0) { print "正"; }
来源：http://oex.fehbvm.com

[T45] Perl：数组遍历
来源：http://vkz.fanxiaobao.xyz

for my $x (@arr) { print $x; }
来源：http://wic.epnwcf.com

[T46] Perl：哈希操作
来源：http://wow.gogol.net.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sax.hnqzz.top

[T47] Perl：正则捕获
来源：http://nko.zhongyouzk.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://zhg.zdbjq.cn

[T48] Perl：正则替换
来源：http://hun.pycfn.com

$s =~ s/old/new/g;
来源：http://piw.guannengcc.top

[T49] Perl：函数
来源：http://jju.zhijiandao.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zds.52xcode.cn

[T50] Perl：逐行读文件
来源：http://xml.aibaodan.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://fvt.zhengqikj.top

while (my $line = <$fh>) { print $line; }
来源：http://pzv.hongshengwenyu.top

[T51] Scala：Hello World
来源：http://hdw.yuxming.cn

println("Hello")
来源：http://rgl.yj20258888.top

[T52] Scala：变量
来源：http://bpt.jinqigufen.top

val a = 1;  var b = 2
来源：http://ltp.svipenyu.cn

[T53] Scala：字符串插值
来源：http://cpe.gzhubu.top

s"值: $b"
来源：http://oiw.chenlongwang.top

[T54] Scala：集合映射
来源：http://bfy.sjlbkw.cn

List(1, 2, 3).map(_ * 2)
来源：http://vhd.yangfankeji.com

[T55] Scala：集合过滤
来源：http://rqc.0kj1m.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wux.wangshuangyany.cn

[T56] Scala：样例类
来源：http://vgt.vehdjk.com

case class User(name: String, age: Int)
来源：http://wia.wangshuangyany.cn

[T57] Scala：模式匹配
来源：http://srf.hongshengwenyu.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://eny.yj20258888.top

[T58] Scala：函数定义
来源：http://nzy.jinqigfzy.top

def add(a: Int, b: Int): Int = a + b
来源：http://iii.yuxming.cn

[T59] Scala：循环
来源：http://gkd.xylfe.cn

for (i <- 1 to 10) println(i)
来源：http://khb.9152youxi.cn

[T60] Scala：折叠
来源：http://rqz.xylfe.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://oiv.zhaomingkeji.xyz

================================================================================
来源：http://qih.zhiwuduotai.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kdz.pengpengdd.cyou

================================================================================
来源：http://lkl.sufxvd.cn

[U01] Py：创建虚拟环境
来源：http://pbd.chenlongwang.top

python -m venv .venv && source .venv/bin/activate
来源：http://wid.0kj1m.cn

[U02] Py：导出 / 安装依赖
来源：http://ito.gogol.net.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qkl.shuidangran.top

[U03] Py：加载 .env 配置
来源：http://vnz.yfazqb.com

from dotenv import load_dotenv; load_dotenv()
来源：http://nfk.pengpengdd.cyou

[U04] Py：变量调试打印
来源：http://mua.cqqwz.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vxd.tanke756.top

[U05] Py：列表去重且保序
来源：http://jwr.jinghuilouyu.cn

list(dict.fromkeys(arr))
来源：http://ekq.yj20258.top

[U06] Py：合并两个字典
来源：http://ojc.yonumen.top

{**a, **b}
来源：http://bqw.bjfxy.top

[U07] Py：反转字典键值
来源：http://dru.pycfn.com

{v: k for k, v in d.items()}
来源：http://drz.iojbl.cn

[U08] Py：展平二维列表
来源：http://egv.gzhubu.top

[y for x in nested for y in x]
来源：http://cxu.wangshuangyany.cn


<!-- 参考信息 -->