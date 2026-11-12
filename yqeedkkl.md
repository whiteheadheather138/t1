代发 wailian999

df -h;  du -sh *
来源：http://xcz.hcnkem.com

[R62] 找最占空间的文件
来源：http://iwn.zhaomingkeji.xyz

du -ah . | sort -rh | head -10
来源：http://zmx.jiagoushi.top

[R63] 内存与进程
来源：http://rop.smart0.xyz

free -h;  ps aux | grep nginx
来源：http://yxp.pengpengdd.cyou

[R64] 结束进程
来源：http://hva.cheryme.top

kill -9 $(pgrep -f app.py)
来源：http://gsx.jinyuanbaomall.cn

[R65] 查看端口占用
来源：http://xvu.vehdjk.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nbd.chenlongwang.top

[R66] 定时任务
来源：http://ksx.hammf.cn

crontab -e;  crontab -l
来源：http://aio.feifeiyinyue.top

[R67] 生成随机十六进制串
来源：http://bdh.hfpthk.cn

openssl rand -hex 16
来源：http://eju.kuanghao11.cn

[R68] 计算文件校验值
来源：http://vey.ctjpmb.com

sha256sum a.txt;  md5sum a.txt
来源：http://zxp.sufxvd.cn

[R69] 生成随机密码
来源：http://wfc.shanyushiyangtech.top

head -c 16 /dev/urandom | base64
来源：http://zkm.yvedp.cn

[R70] 时间戳与互转
来源：http://pqh.chenjidiqi.icu

date +%s;  date -d @1700000000
来源：http://tex.c1oappe.top

[R71] 日期格式化
来源：http://pid.xuanzx.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://mvf.smart0.xyz

[R72] 等待端口就绪
来源：http://rgp.52xcode.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://don.chenzaomai.com

[R73] 分割大日志
来源：http://vdl.yvedp.cn

split -l 1000 big.log part_
来源：http://wig.xinyue.icu

[R74] 批量重命名
来源：http://cnj.gogol.net.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mym.redwolf501.top

[R75] 导出环境变量
来源：http://bbz.hysaishi.cn

export PATH="$HOME/bin:$PATH"
来源：http://dhw.guannengcc.top

[R76] 使用临时文件
来源：http://zig.mhx1999.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mip.chenjidiqi.icu

[R77] 读取用户输入
来源：http://vfn.aizwys.cn

read -rp "请输入: " ans
来源：http://wcw.cheryme.top

[R78] 交互式菜单
来源：http://llh.chenlongwang.top

select opt in a b c; do echo "$opt"; break; done
来源：http://oek.hfpthk.cn

[R79] 解析命令行选项
来源：http://nzf.daria6918.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mdw.andypj.xyz

[R80] 查看脚本执行耗时
来源：http://vey.pycfn.com

time ./run.sh
来源：http://ldg.shanyushiyangtech.top

================================================================================
来源：http://rpo.jyoumei.cn

S. C / C++ 专题
来源：http://kbs.gotoacloud.top

================================================================================
来源：http://ypo.ehwqpu.com

[S01] C：Hello World
来源：http://sao.yj20258.top

#include <stdio.h>
来源：http://odh.sjlbkw.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://quv.meibo888.top

[S02] C：变量与格式化输出
来源：http://igz.cheryme.top

int a = 10; printf("%d\n", a);
来源：http://cub.zycfv.cn

[S03] C：读入整数
来源：http://jer.tian-w.cn

int x; scanf("%d", &x);
来源：http://tsf.nwbrower.top

[S04] C：字符串复制
来源：http://lxt.ybcxt.top

char dst[32]; strcpy(dst, "hi");
来源：http://jvd.ybcxt.top

[S05] C：字符串长度
来源：http://vry.meibo888.top

strlen(s)
来源：http://eyn.nanxuanxn.top

[S06] C：字符串比较
来源：http://gct.guowangkeji.top

strcmp(a, b) == 0
来源：http://vxy.fengsongda.top

[S07] C：数组遍历求和
来源：http://ovd.zdqjudy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jkt.xylfe.cn

[S08] C：动态内存分配与释放
来源：http://nhz.hywenlv.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://srn.316326.xyz

[S09] C：结构体定义与初始化
来源：http://ptq.cucudq.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vre.xuanzx.com

[S10] C：指针与解引用
来源：http://neb.mhx1999.top

int *p = &a;  *p = 5;
来源：http://cdj.dianchejie.cn

[S11] C：逐行读文件
来源：http://htv.jqgfzy.top

FILE *f = fopen("a.txt", "r");
来源：http://dtx.meibo888.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://cql.ppjwa.cn

fclose(f);
来源：http://fyt.gotoacloud.top

[S12] C：写文件
来源：http://tji.fanxiaobao.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://aog.chenzaomai.com

[S13] C：宏定义
来源：http://vow.xinyue.icu

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lbd.hongshengwenyu.top

[S14] C：枚举
来源：http://cgx.birdmap.top

enum Color { RED, GREEN, BLUE };
来源：http://ncc.shangyingyoupin.top

[S15] C：类型转换
来源：http://iwg.yj202588.top

(double) a / b
来源：http://pji.shangyingyoupin.top

[S16] C：位操作置位
来源：http://hmt.shanyushiyangkeji.top

x |= (1 << 3);
来源：http://nnk.yj202588.top

[S17] C：安全拼接字符串
来源：http://iuj.zycfv.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wva.tian-w.cn

[S18] C：命令行参数
来源：http://efu.cucudq.cn

int main(int argc, char **argv)
来源：http://irw.chenjidiqi.icu

[S19] C：快速排序
来源：http://bcx.tarul.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zlf.sweek.top

[S20] C：二分查找
来源：http://jqv.dashuyun.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bpk.fktsv.cn

[S21] C：字符类别判断
来源：http://ven.wangdashe.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mjs.ehwqpu.com

[S22] C：字符串转数字
来源：http://cge.sxryk.cn

atoi("42");  strtod("3.14", NULL);
来源：http://mrv.hcnkem.com

[S23] C：随机数
来源：http://hnn.haohaochexian.top

srand(time(NULL));  int r = rand() % 100;
来源：http://mai.jqgfzy.top

[S24] C：获取本地时间
来源：http://yur.sxryk.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hqb.epnwcf.com

[S25] C：内存拷贝
来源：http://xee.yvedp.cn

memcpy(dst, src, n);
来源：http://lvg.zycfv.cn

[S26] C：内存清零
来源：http://fmp.nwbrower.top

memset(a, 0, sizeof a);
来源：http://mkm.haohaochexian.top

[S27] C：定义常量
来源：http://lqv.c1oappe.top

const double PI = 3.14159;
来源：http://chm.sjlbkw.cn

[S28] C：静态变量
来源：http://neu.hnqzz.top

static int counter = 0;
来源：http://pmo.yangfankeji.com

[S29] C：变参函数
来源：http://cxo.hnqzz.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uec.shuidangran.top

[S30] C：头文件保护
来源：http://yea.shanyushiyangtech.top

#ifndef X_H
来源：http://lok.shanyushiyangtech.top

#define X_H
来源：http://ntw.xziqi.cn

#endif
来源：http://nje.hongshengwenyu.top

[S31] C++：Hello World
来源：http://ljt.andypj.xyz

#include <iostream>
来源：http://jld.zhiwuduotai.top

int main() { std::cout << "Hello\n"; }
来源：http://tbj.chenjidiqi.icu

[S32] C++：字符串
来源：http://jul.yongpay.top

std::string s = "hi";  s += "!";
来源：http://qda.cashguo.top

[S33] C++：vector 增删
来源：http://lxt.jyoumei.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nnw.zhijiandao.cn

[S34] C++：遍历 vector
来源：http://kla.jlsjyb.cn

for (auto &x : v) { std::cout << x; }
来源：http://grm.tian-w.cn

[S35] C++：map
来源：http://ihk.wangshuangyany.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tua.tarul.cn

[S36] C++：unordered_map
来源：http://yfc.jianghu66.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pkv.zycfv.cn

[S37] C++：set
来源：http://fbx.tarul.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bck.fktsv.cn

[S38] C++：排序
来源：http://fdc.feifeiyinyue.top

std::sort(v.begin(), v.end());
来源：http://uyn.yj20258888.top

[S39] C++：自定义比较器排序
来源：http://bsh.sufxvd.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rjx.gogol.net.cn

[S40] C++：查找元素
来源：http://kmy.snrcjt.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hvc.tarul.cn

[S41] C++：类与构造函数
来源：http://exk.cashguo.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jjn.jqgfzy.top

[S42] C++：继承与虚函数
来源：http://gpk.yvedp.cn

class B : public Base { public: void f() override {} };
来源：http://djk.ybcxt.top

[S43] C++：智能指针
来源：http://ylw.jinqigfzy.top

auto p = std::make_unique<int>(5);
来源：http://ywh.vehdjk.com

[S44] C++：引用传参
来源：http://wgh.chenlongwang.top

void inc(int &x) { ++x; }
来源：http://mnu.quarkkingdee.top

[S45] C++：lambda
来源：http://ifk.yj20258888.top

auto add = [](int a, int b) { return a + b; };
来源：http://ouq.svipenyu.cn

[S46] C++：函数模板
来源：http://vej.havefunace.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tae.sysykeji.top

[S47] C++：结构化绑定遍历
来源：http://vne.kuanghao11.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nyl.shuidangran.top

[S48] C++：逐行读文件
来源：http://ayf.quarkkingdee.top

std::ifstream in("a.txt");  std::string line;
来源：http://fyj.tanke756.top

while (std::getline(in, line)) { }
来源：http://qby.guowangkeji.top

[S49] C++：写文件
来源：http://iya.cucudq.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nvo.pengpengdd.cyou

[S50] C++：格式化数字
来源：http://ndg.yvedp.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ifk.cheryme.top

[S51] C++：显式类型转换
来源：http://yhu.hywenlv.cn

static_cast<double>(a) / b
来源：http://uui.sweek.top

[S52] C++：const 与 noexcept
来源：http://qed.hesvh.cn

int size() const noexcept { return n_; }
来源：http://yzt.gogol.net.cn

[S53] C++：移动语义
来源：http://uza.yangfankeji.com

std::vector<int> w = std::move(v);
来源：http://nqb.fehbvm.com

[S54] C++：异常处理
来源：http://gbk.sweek.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vau.vqdsnc.cn

[S55] C++：结构化绑定
来源：http://nxe.yvedp.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://oeo.hammf.cn

[S56] C++：optional
来源：http://fug.zhijiandao.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://agl.yanxiufei.cn

[S57] C++：编译期常量
来源：http://ciy.sweek.top

constexpr int N = 10;
来源：http://xqi.guannengcc.top

[S58] C++：命名空间
来源：http://cnm.c1oappe.top

namespace ns { int f() { return 1; } }
来源：http://sgi.dianchejie.cn

[S59] C++：静态断言
来源：http://qhh.yfazqb.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mlk.zycfv.cn

[S60] C++：遍历并删除元素
来源：http://rtl.ydzc1.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://daj.cheryme.top

================================================================================
来源：http://eru.yonumen.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://sat.zhiwuduotai.top

================================================================================
来源：http://iyq.zdbjq.cn

[T01] Kotlin：Hello World
来源：http://ubi.yangfankeji.com

println("Hello")
来源：http://chg.hnxiangtu.top

[T02] Kotlin：变量
来源：http://ysj.meibo888.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dbo.ydjk.org.cn

[T03] Kotlin：字符串模板
来源：http://gup.ppjwa.cn

"值: $b"
来源：http://mts.chenzaomai.com

[T04] Kotlin：空安全
来源：http://dxi.andypj.xyz

val n: String? = null;  n?.length
来源：http://atw.hammf.cn

[T05] Kotlin：when 表达式
来源：http://pdz.sysykeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hyy.dianchejie.cn

[T06] Kotlin：集合映射
来源：http://pzo.smart0.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://acq.hywenlv.cn

[T07] Kotlin：集合过滤
来源：http://uon.fktsv.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://oih.vqdsnc.cn

[T08] Kotlin：数据类
来源：http://ijx.yuxming.cn

data class User(val name: String, val age: Int)
来源：http://dzw.yonumen.top

[T09] Kotlin：扩展函数
来源：http://zrz.yj202588.top

fun String.exclaim() = this + "!"
来源：http://xta.yongpay.top

[T10] Kotlin：默认参数
来源：http://zhl.wangdashe.top

fun greet(name: String = "World") = "Hi $name"
来源：http://qai.ybcxt.top

[T11] Kotlin：协程
来源：http://nas.jiagoushi.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://sue.iojbl.cn

[T12] Kotlin：解构声明
来源：http://zvf.hesvh.cn

val (a, b) = Pair(1, 2)
来源：http://kir.xingfuxueyuan.xyz

[T13] Kotlin：只读 Map
来源：http://kah.wangdashe.top

val m = mapOf("a" to 1)
来源：http://ehd.cucudq.cn

[T14] Kotlin：循环
来源：http://ofm.wangshuangyany.cn

for (i in 1..10) println(i)
来源：http://hbm.hywenlv.cn

[T15] Kotlin：接口
来源：http://pvk.gzhubu.top

interface Shape { fun area(): Double }
来源：http://ylp.xuanzx.com

[T16] Swift：Hello World
来源：http://iiy.yuanzhike.top

print("Hello")
来源：http://nee.ywan-chungtsiang.top

[T17] Swift：变量与常量
来源：http://zej.xinyue.icu

var a = 1;  let b = 2
来源：http://ltn.mhx1999.top

[T18] Swift：字符串插值
来源：http://qpx.dianchejie.cn

"值: \(b)"
来源：http://hre.sufxvd.cn

[T19] Swift：可选绑定
来源：http://uhw.birdmap.top

if let n = opt { print(n) }
来源：http://pfh.jlsjyb.cn

[T20] Swift：数组操作
来源：http://wvf.yonumen.top

var a = [1, 2, 3];  a.append(4)
来源：http://htt.ivvv.top

[T21] Swift：遍历
来源：http://srf.zhijiandao.cn

for x in a { print(x) }
来源：http://bsi.zhengqikj.top

[T22] Swift：字典
来源：http://him.zhoulong.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://vyp.chenlongwang.top

[T23] Swift：函数
来源：http://vpl.yangfankeji.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wlx.cheryme.top

[T24] Swift：闭包
来源：http://jcm.fzhhl.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://sip.nanxuanxn.top

[T25] Swift：结构体
来源：http://hjc.ehwqpu.com

struct P { var x: Int }
来源：http://gbw.yuxming.cn

[T26] Swift：类与重写
来源：http://yzj.zycfv.cn

class A: Base { override func f() {} }
来源：http://qyp.52xcode.cn

[T27] Swift：错误处理
来源：http://dtr.ydjk.org.cn

do { try f() } catch { print(error) }
来源：http://zin.yvedp.cn

[T28] Swift：枚举
来源：http://cxa.fehbvm.com

enum Color { case red, green }
来源：http://ubx.yonumen.top

[T29] Swift：guard 提前返回
来源：http://ydp.smart0.xyz

guard let x = opt else { return }
来源：http://cve.jiagoushi.top

[T30] Swift：协议
来源：http://cix.yj20258888.top

protocol Shape { func area() -> Double }
来源：http://ffw.andypj.xyz

[T31] Lua：Hello World
来源：http://tdd.zhengqikj.top

print("Hello")
来源：http://uxa.cashguo.top

[T32] Lua：局部变量
来源：http://gvo.hcnkem.com

local a = 1
来源：http://wix.ppjwa.cn

[T33] Lua：表（数组）
来源：http://itq.wangdashe.top

local t = {1, 2, 3};  t[4] = 4
来源：http://gzw.hesvh.cn

[T34] Lua：遍历表
来源：http://bnf.yfazqb.com

for i, v in ipairs(t) do print(i, v) end
来源：http://ofz.kuanghao11.cn

[T35] Lua：字典表
来源：http://gud.xuetiantiany.cn

local d = { a = 1 };  d.b = 2
来源：http://xxe.ydjk.org.cn

[T36] Lua：函数
来源：http://tov.quarkkingdee.top

function add(a, b) return a + b end
来源：http://qzp.zhengqikj.top

[T37] Lua：字符串拼接
来源：http://vyy.meibo888.top

"a" .. "b"
来源：http://ncx.shuidangran.top

[T38] Lua：条件
来源：http://dlu.cashguo.top

if x > 0 then print("正") end
来源：http://cmf.sxryk.cn

[T39] Lua：模式匹配
来源：http://xoq.fktsv.cn

string.find(s, "%d+")
来源：http://dre.hongshengwenyu.top

[T40] Lua：元表
来源：http://bvp.hnxiangtu.top

setmetatable({}, { __index = base })
来源：http://obv.yonumen.top

[T41] Perl：Hello World
来源：http://jed.ppjwa.cn

print "Hello\n";
来源：http://yxm.zhengqikj.top

[T42] Perl：变量类型
来源：http://hdm.jinyuanbaomall.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://api.jinqigufen.top

[T43] Perl：字符串插值
来源：http://pkq.sxryk.cn

"值: $a"
来源：http://pwf.sweek.top

[T44] Perl：条件
来源：http://wyp.yueranfly.top

if ($a > 0) { print "正"; }
来源：http://yka.meibo888.top

[T45] Perl：数组遍历
来源：http://fpr.iojbl.cn

for my $x (@arr) { print $x; }
来源：http://jcy.zycfv.cn

[T46] Perl：哈希操作
来源：http://dsx.daria6918.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://elm.hysaishi.cn

[T47] Perl：正则捕获
来源：http://sox.vehdjk.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://gjg.birdmap.top

[T48] Perl：正则替换
来源：http://wzw.feifeiyinyue.top

$s =~ s/old/new/g;
来源：http://vrf.jqgufenzy.top

[T49] Perl：函数
来源：http://smq.wangshuangyany.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pvt.haohaochexian.top

[T50] Perl：逐行读文件
来源：http://xpg.havefunace.top

open my $fh, "<", "a.txt" or die $!;
来源：http://mnu.snrcjt.cn

while (my $line = <$fh>) { print $line; }
来源：http://vit.xuetiantiany.cn

[T51] Scala：Hello World
来源：http://wqh.hnxiangtu.top

println("Hello")
来源：http://kkz.shuidangran.top

[T52] Scala：变量
来源：http://fda.shanyushiyangkeji.top

val a = 1;  var b = 2
来源：http://foo.hnqzz.top

[T53] Scala：字符串插值
来源：http://tsp.jyoumei.cn

s"值: $b"
来源：http://kle.shuidangran.top

[T54] Scala：集合映射
来源：http://rfb.fktsv.cn

List(1, 2, 3).map(_ * 2)
来源：http://apj.yongpay.top

[T55] Scala：集合过滤
来源：http://rso.xinyue.icu

List(1, 2, 3).filter(_ > 1)
来源：http://kvg.316326.xyz

[T56] Scala：样例类
来源：http://elt.sufxvd.cn

case class User(name: String, age: Int)
来源：http://htv.chenlongwang.top

[T57] Scala：模式匹配
来源：http://qrr.zdqjudy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://llr.jqgufenzy.top

[T58] Scala：函数定义
来源：http://fca.nwbrower.top

def add(a: Int, b: Int): Int = a + b
来源：http://ckr.52xcode.cn

[T59] Scala：循环
来源：http://qvd.andypj.xyz

for (i <- 1 to 10) println(i)
来源：http://lkn.yuanzhike.top

[T60] Scala：折叠
来源：http://pto.sufxvd.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://coh.xingfuxueyuan.xyz

================================================================================
来源：http://mzv.zhongyouzk.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gmk.yuanzhike.top

================================================================================
来源：http://qou.jiagoushi.top

[U01] Py：创建虚拟环境
来源：http://snl.nanxuanxn.top

python -m venv .venv && source .venv/bin/activate
来源：http://zjw.tianlin.xyz

[U02] Py：导出 / 安装依赖
来源：http://kue.feifeiyinyue.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bxj.haohaochexian.top


<!-- 参考信息 -->