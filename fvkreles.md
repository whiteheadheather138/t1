代发 wailian999

free -h;  ps aux | grep nginx
来源：http://gfg.haohaochexian.top

[R64] 结束进程
来源：http://men.hfpthk.cn

kill -9 $(pgrep -f app.py)
来源：http://cwe.gogol.net.cn

[R65] 查看端口占用
来源：http://meb.fanxiaobao.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ntj.ivvv.top

[R66] 定时任务
来源：http://mzc.jyoumei.cn

crontab -e;  crontab -l
来源：http://lpm.yj20258.top

[R67] 生成随机十六进制串
来源：http://vrr.dashuyun.cn

openssl rand -hex 16
来源：http://cvz.cucudq.cn

[R68] 计算文件校验值
来源：http://ndm.cucudq.cn

sha256sum a.txt;  md5sum a.txt
来源：http://nut.c1oappe.top

[R69] 生成随机密码
来源：http://daq.jqgufenzy.top

head -c 16 /dev/urandom | base64
来源：http://nua.sweek.top

[R70] 时间戳与互转
来源：http://xft.jinqigfzy.top

date +%s;  date -d @1700000000
来源：http://rpw.ybcxt.top

[R71] 日期格式化
来源：http://uwb.jlsjyb.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://lev.yfazqb.com

[R72] 等待端口就绪
来源：http://frb.jlsjyb.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://uls.jinyuanbaomall.cn

[R73] 分割大日志
来源：http://adl.zhongyouzk.top

split -l 1000 big.log part_
来源：http://uoh.52xcode.cn

[R74] 批量重命名
来源：http://qow.shanyushiyangkeji.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://evo.guowangkeji.top

[R75] 导出环境变量
来源：http://cej.yj20258888.top

export PATH="$HOME/bin:$PATH"
来源：http://tpu.ivvv.top

[R76] 使用临时文件
来源：http://ocf.yangfankeji.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://khx.9152youxi.cn

[R77] 读取用户输入
来源：http://bfa.snrcjt.cn

read -rp "请输入: " ans
来源：http://pxi.shzxlz.cn

[R78] 交互式菜单
来源：http://jcx.zdbjq.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://cyh.jiagoushi.top

[R79] 解析命令行选项
来源：http://stp.cashguo.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yuc.yuanzhike.top

[R80] 查看脚本执行耗时
来源：http://kcw.cucudq.cn

time ./run.sh
来源：http://rct.quarkkingdee.top

================================================================================
来源：http://wpg.cdnleiting.top

S. C / C++ 专题
来源：http://jpk.smart0.xyz

================================================================================
来源：http://puw.smart0.xyz

[S01] C：Hello World
来源：http://cid.sxryk.cn

#include <stdio.h>
来源：http://rso.jqgufenzy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://qys.haohaochexian.top

[S02] C：变量与格式化输出
来源：http://uqt.shanyushiyangtech.top

int a = 10; printf("%d\n", a);
来源：http://cbr.pycfn.com

[S03] C：读入整数
来源：http://see.tian-w.cn

int x; scanf("%d", &x);
来源：http://prp.bjfxy.top

[S04] C：字符串复制
来源：http://zbd.zhengqikj.top

char dst[32]; strcpy(dst, "hi");
来源：http://uoj.hesvh.cn

[S05] C：字符串长度
来源：http://zgl.sweek.top

strlen(s)
来源：http://vwi.feifeiyinyue.top

[S06] C：字符串比较
来源：http://okd.zhaomingkeji.xyz

strcmp(a, b) == 0
来源：http://wzg.hesvh.cn

[S07] C：数组遍历求和
来源：http://yob.hysaishi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://oum.hongshengwenyu.top

[S08] C：动态内存分配与释放
来源：http://lrk.chenlongwang.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wac.xingfuxueyuan.xyz

[S09] C：结构体定义与初始化
来源：http://pcn.bjfxy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lzk.yueranfly.top

[S10] C：指针与解引用
来源：http://xen.zdbjq.cn

int *p = &a;  *p = 5;
来源：http://hmu.hnqzz.top

[S11] C：逐行读文件
来源：http://fpz.hfpthk.cn

FILE *f = fopen("a.txt", "r");
来源：http://bez.zhaomingkeji.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://zhi.vehdjk.com

fclose(f);
来源：http://hya.cucudq.cn

[S12] C：写文件
来源：http://bca.sysykeji.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://imu.bbcook.cn

[S13] C：宏定义
来源：http://ltf.yuanzhike.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hpd.shangyingyoupin.top

[S14] C：枚举
来源：http://rjw.shzxlz.cn

enum Color { RED, GREEN, BLUE };
来源：http://qcm.shangyingyoupin.top

[S15] C：类型转换
来源：http://ikb.pycfn.com

(double) a / b
来源：http://njs.nwbrower.top

[S16] C：位操作置位
来源：http://mqm.sufxvd.cn

x |= (1 << 3);
来源：http://eec.jyoumei.cn

[S17] C：安全拼接字符串
来源：http://pje.jlsjyb.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dda.aibaodan.cn

[S18] C：命令行参数
来源：http://pag.birdmap.top

int main(int argc, char **argv)
来源：http://sgj.jinqigufen.top

[S19] C：快速排序
来源：http://gni.xylfe.cn

qsort(a, n, sizeof(int), cmp);
来源：http://urr.yfazqb.com

[S20] C：二分查找
来源：http://crj.snrcjt.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://miy.tarul.cn

[S21] C：字符类别判断
来源：http://iso.chenjidiqi.icu

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xvw.ybcxt.top

[S22] C：字符串转数字
来源：http://qxq.ybcxt.top

atoi("42");  strtod("3.14", NULL);
来源：http://xns.jyoumei.cn

[S23] C：随机数
来源：http://vjt.hfpthk.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zoi.316326.xyz

[S24] C：获取本地时间
来源：http://uru.c1oappe.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ssj.0kj1m.cn

[S25] C：内存拷贝
来源：http://cza.gotoacloud.top

memcpy(dst, src, n);
来源：http://zix.sxryk.cn

[S26] C：内存清零
来源：http://koh.hongshengwenyu.top

memset(a, 0, sizeof a);
来源：http://xbc.zhiwuduotai.top

[S27] C：定义常量
来源：http://dab.hfpthk.cn

const double PI = 3.14159;
来源：http://yvw.epnwcf.com

[S28] C：静态变量
来源：http://qra.yj202588.top

static int counter = 0;
来源：http://gug.yangfankeji.com

[S29] C：变参函数
来源：http://yqu.hnxiangtu.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kbz.pengpengdd.cyou

[S30] C：头文件保护
来源：http://dyh.52xcode.cn

#ifndef X_H
来源：http://kvo.yongpay.top

#define X_H
来源：http://yng.xziqi.cn

#endif
来源：http://dsf.jiagoushi.top

[S31] C++：Hello World
来源：http://tjs.cdnleiting.top

#include <iostream>
来源：http://lzv.zycfv.cn

int main() { std::cout << "Hello\n"; }
来源：http://ofr.sweek.top

[S32] C++：字符串
来源：http://awu.guowangkeji.top

std::string s = "hi";  s += "!";
来源：http://xtb.ppjwa.cn

[S33] C++：vector 增删
来源：http://gje.ywan-chungtsiang.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://phd.jlsjyb.cn

[S34] C++：遍历 vector
来源：http://har.zhixingplan.top

for (auto &x : v) { std::cout << x; }
来源：http://xvh.fanxiaobao.xyz

[S35] C++：map
来源：http://bgl.pengpengdd.cyou

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rot.snrcjt.cn

[S36] C++：unordered_map
来源：http://zlh.xuetiantiany.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kbs.ydzc1.top

[S37] C++：set
来源：http://uub.xziqi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fvw.shuidangran.top

[S38] C++：排序
来源：http://plz.shzxlz.cn

std::sort(v.begin(), v.end());
来源：http://oou.jlsjyb.cn

[S39] C++：自定义比较器排序
来源：http://mxs.kuanghao11.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uko.smart0.xyz

[S40] C++：查找元素
来源：http://fqg.gzhubu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zkr.shangyingyoupin.top

[S41] C++：类与构造函数
来源：http://lsc.iojbl.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tqg.jinqigfzy.top

[S42] C++：继承与虚函数
来源：http://txd.iojbl.cn

class B : public Base { public: void f() override {} };
来源：http://zga.jqgufenzy.top

[S43] C++：智能指针
来源：http://lzc.jinghuilouyu.cn

auto p = std::make_unique<int>(5);
来源：http://qbh.cashguo.top

[S44] C++：引用传参
来源：http://doa.shanyushiyangkeji.top

void inc(int &x) { ++x; }
来源：http://rad.shuidangran.top

[S45] C++：lambda
来源：http://owi.tian-w.cn

auto add = [](int a, int b) { return a + b; };
来源：http://olh.zdbjq.cn

[S46] C++：函数模板
来源：http://sdq.9152youxi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gwg.shanyushiyangkeji.top

[S47] C++：结构化绑定遍历
来源：http://jdw.epnwcf.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://atg.ehwqpu.com

[S48] C++：逐行读文件
来源：http://tii.hesvh.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fkj.yfazqb.com

while (std::getline(in, line)) { }
来源：http://qjh.ydzc1.top

[S49] C++：写文件
来源：http://bdj.xingfuxueyuan.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zre.xuetiantiany.cn

[S50] C++：格式化数字
来源：http://lln.shanyushiyangtech.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qzm.ybcxt.top

[S51] C++：显式类型转换
来源：http://jhy.jqgfzy.top

static_cast<double>(a) / b
来源：http://qfx.shanyushiyangkeji.top

[S52] C++：const 与 noexcept
来源：http://wnw.jlsjyb.cn

int size() const noexcept { return n_; }
来源：http://phk.nanxinkj.top

[S53] C++：移动语义
来源：http://uqk.vqdsnc.cn

std::vector<int> w = std::move(v);
来源：http://med.ywan-chungtsiang.top

[S54] C++：异常处理
来源：http://srb.svipenyu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yvq.chenjidiqi.icu

[S55] C++：结构化绑定
来源：http://yuc.xziqi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zba.yanxiufei.cn

[S56] C++：optional
来源：http://bjm.shanyushiyangtech.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://oiv.iojbl.cn

[S57] C++：编译期常量
来源：http://cjg.jinghuilouyu.cn

constexpr int N = 10;
来源：http://tiw.bbcook.cn

[S58] C++：命名空间
来源：http://wkr.gotoacloud.top

namespace ns { int f() { return 1; } }
来源：http://jaq.shzxlz.cn

[S59] C++：静态断言
来源：http://gvi.bjfxy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dbm.jiagoushi.top

[S60] C++：遍历并删除元素
来源：http://nfr.wangshuangyany.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://npl.bjfxy.top

================================================================================
来源：http://cag.ydzc1.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://som.fehbvm.com

================================================================================
来源：http://rhe.cashguo.top

[T01] Kotlin：Hello World
来源：http://kok.fktsv.cn

println("Hello")
来源：http://efm.pycfn.com

[T02] Kotlin：变量
来源：http://cze.yonumen.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nsx.jyoumei.cn

[T03] Kotlin：字符串模板
来源：http://tna.bjfxy.top

"值: $b"
来源：http://jga.yongpay.top

[T04] Kotlin：空安全
来源：http://ism.iojbl.cn

val n: String? = null;  n?.length
来源：http://bmg.sxryk.cn

[T05] Kotlin：when 表达式
来源：http://kyg.shzxlz.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xzb.xuetiantiany.cn

[T06] Kotlin：集合映射
来源：http://bui.sweek.top

listOf(1, 2, 3).map { it * 2 }
来源：http://uqx.cheryme.top

[T07] Kotlin：集合过滤
来源：http://wxw.haohaochexian.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://uon.hfpthk.cn

[T08] Kotlin：数据类
来源：http://rzt.zhixingplan.top

data class User(val name: String, val age: Int)
来源：http://omj.jinqigufen.top

[T09] Kotlin：扩展函数
来源：http://zak.cheryme.top

fun String.exclaim() = this + "!"
来源：http://sxy.wangshuangyany.cn

[T10] Kotlin：默认参数
来源：http://wst.wangdashe.top

fun greet(name: String = "World") = "Hi $name"
来源：http://abs.shuidangran.top

[T11] Kotlin：协程
来源：http://jly.zhoulong.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://wfd.iojbl.cn

[T12] Kotlin：解构声明
来源：http://yqb.jqgfzy.top

val (a, b) = Pair(1, 2)
来源：http://ujk.tian-w.cn

[T13] Kotlin：只读 Map
来源：http://hqm.aizwys.cn

val m = mapOf("a" to 1)
来源：http://nqn.nanxinkj.top

[T14] Kotlin：循环
来源：http://aqb.zhiwuduotai.top

for (i in 1..10) println(i)
来源：http://pcy.kuanghao11.cn

[T15] Kotlin：接口
来源：http://jfd.jqgufenzy.top

interface Shape { fun area(): Double }
来源：http://jjo.sjlbkw.cn

[T16] Swift：Hello World
来源：http://ebp.hammf.cn

print("Hello")
来源：http://twz.jinghuilouyu.cn

[T17] Swift：变量与常量
来源：http://zwh.zhengqikj.top

var a = 1;  let b = 2
来源：http://cub.zhijiandao.cn

[T18] Swift：字符串插值
来源：http://rpm.svipenyu.cn

"值: \(b)"
来源：http://heo.uphjek.com

[T19] Swift：可选绑定
来源：http://twk.jinghuilouyu.cn

if let n = opt { print(n) }
来源：http://hcr.gotoacloud.top

[T20] Swift：数组操作
来源：http://yql.shzxlz.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jqq.zhaomingkeji.xyz

[T21] Swift：遍历
来源：http://iba.hongshengwenyu.top

for x in a { print(x) }
来源：http://xjb.gzhubu.top

[T22] Swift：字典
来源：http://hrw.nanxinkj.top

var d = ["a": 1];  d["b"] = 2
来源：http://kll.dashuyun.cn

[T23] Swift：函数
来源：http://tpi.52xcode.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ogx.yonumen.top

[T24] Swift：闭包
来源：http://lfu.zhijiandao.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://oei.wangdashe.top

[T25] Swift：结构体
来源：http://jgs.hywenlv.cn

struct P { var x: Int }
来源：http://qra.fzhhl.top

[T26] Swift：类与重写
来源：http://hsb.daxiang520.top

class A: Base { override func f() {} }
来源：http://vti.jinghuilouyu.cn

[T27] Swift：错误处理
来源：http://txy.zdqjudy.top

do { try f() } catch { print(error) }
来源：http://itm.xinyue.icu

[T28] Swift：枚举
来源：http://ryh.9152youxi.cn

enum Color { case red, green }
来源：http://nwh.aizwys.cn

[T29] Swift：guard 提前返回
来源：http://pyg.sufxvd.cn

guard let x = opt else { return }
来源：http://cox.ehwqpu.com

[T30] Swift：协议
来源：http://bag.fengsongda.top

protocol Shape { func area() -> Double }
来源：http://bhk.zhijiandao.cn

[T31] Lua：Hello World
来源：http://nmg.nanxinkj.top

print("Hello")
来源：http://rvg.hcnkem.com

[T32] Lua：局部变量
来源：http://qll.52xcode.cn

local a = 1
来源：http://ors.jinyuanbaomall.cn

[T33] Lua：表（数组）
来源：http://act.gotoacloud.top

local t = {1, 2, 3};  t[4] = 4
来源：http://alt.chenlongwang.top

[T34] Lua：遍历表
来源：http://vwg.nanxuanxn.top

for i, v in ipairs(t) do print(i, v) end
来源：http://eai.wangdashe.top

[T35] Lua：字典表
来源：http://vir.nanxinkj.top

local d = { a = 1 };  d.b = 2
来源：http://rpl.dianchejie.cn

[T36] Lua：函数
来源：http://cai.fzhhl.top

function add(a, b) return a + b end
来源：http://uyk.hcnkem.com

[T37] Lua：字符串拼接
来源：http://ymo.nanxinkj.top

"a" .. "b"
来源：http://kvw.daxiang520.top

[T38] Lua：条件
来源：http://xws.bjfxy.top

if x > 0 then print("正") end
来源：http://cln.ywan-chungtsiang.top

[T39] Lua：模式匹配
来源：http://gii.xingfuxueyuan.xyz

string.find(s, "%d+")
来源：http://rqd.tianlin.xyz

[T40] Lua：元表
来源：http://qrs.dianchejie.cn

setmetatable({}, { __index = base })
来源：http://tuw.iojbl.cn

[T41] Perl：Hello World
来源：http://fnk.ctjpmb.com

print "Hello\n";
来源：http://jxa.daxiang520.top

[T42] Perl：变量类型
来源：http://wxs.ydzc1.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xwa.haohaochexian.top

[T43] Perl：字符串插值
来源：http://sae.bjfxy.top

"值: $a"
来源：http://wwv.zhijiandao.cn

[T44] Perl：条件
来源：http://key.hesvh.cn

if ($a > 0) { print "正"; }
来源：http://ejz.havefunace.top

[T45] Perl：数组遍历
来源：http://raz.redwolf501.top

for my $x (@arr) { print $x; }
来源：http://but.c1oappe.top

[T46] Perl：哈希操作
来源：http://lmz.meibo888.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mmh.fktsv.cn

[T47] Perl：正则捕获
来源：http://nfi.yangfankeji.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://vrp.cdnleiting.top

[T48] Perl：正则替换
来源：http://yhs.fehbvm.com

$s =~ s/old/new/g;
来源：http://hlz.yvedp.cn

[T49] Perl：函数
来源：http://ycy.xuanzx.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bdz.mhx1999.top

[T50] Perl：逐行读文件
来源：http://rrf.zhongyouzk.top

open my $fh, "<", "a.txt" or die $!;
来源：http://igv.redwolf501.top

while (my $line = <$fh>) { print $line; }
来源：http://vdd.xuetiantiany.cn

[T51] Scala：Hello World
来源：http://pgr.ywan-chungtsiang.top

println("Hello")
来源：http://flh.bbcook.cn

[T52] Scala：变量
来源：http://doi.shuidangran.top

val a = 1;  var b = 2
来源：http://kkj.fehbvm.com

[T53] Scala：字符串插值
来源：http://ctc.xuanzx.com

s"值: $b"
来源：http://dvt.yongpay.top

[T54] Scala：集合映射
来源：http://iff.ydjk.org.cn

List(1, 2, 3).map(_ * 2)
来源：http://riw.shangyingyoupin.top

[T55] Scala：集合过滤
来源：http://acv.zhiwuduotai.top

List(1, 2, 3).filter(_ > 1)
来源：http://emz.ivvv.top

[T56] Scala：样例类
来源：http://onw.dianchejie.cn

case class User(name: String, age: Int)
来源：http://tsg.9152youxi.cn

[T57] Scala：模式匹配
来源：http://bzw.xylfe.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://aqt.yanxiufei.cn

[T58] Scala：函数定义
来源：http://fzw.jinqigfzy.top

def add(a: Int, b: Int): Int = a + b
来源：http://vfp.xuetiantiany.cn

[T59] Scala：循环
来源：http://hku.redwolf501.top

for (i <- 1 to 10) println(i)
来源：http://cvs.52xcode.cn

[T60] Scala：折叠
来源：http://haa.snrcjt.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://odc.pycfn.com

================================================================================
来源：http://nlh.sjlbkw.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://uyv.hcnkem.com

================================================================================
来源：http://qqv.shzxlz.cn

[U01] Py：创建虚拟环境
来源：http://xhf.tarul.cn

python -m venv .venv && source .venv/bin/activate
来源：http://igf.gzhubu.top

[U02] Py：导出 / 安装依赖
来源：http://wic.gogol.net.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qbq.hysaishi.cn

[U03] Py：加载 .env 配置
来源：http://kdp.gaohongyu789.top

from dotenv import load_dotenv; load_dotenv()
来源：http://upw.zdqjudy.top

[U04] Py：变量调试打印
来源：http://irl.c1oappe.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://xdq.zycfv.cn


<!-- 参考信息 -->