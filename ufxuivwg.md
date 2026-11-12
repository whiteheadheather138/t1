代发 wailian999

ssh user@host 'uptime'
来源：http://mxn.zdbjq.cn

[R58] 下载文件
来源：http://pwr.aizwys.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://djo.fktsv.cn

[R59] 发 POST JSON
来源：http://mrk.hywenlv.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hlx.dashuyun.cn

[R60] 只看 HTTP 状态码
来源：http://uty.zhengqikj.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://inq.tarul.cn

[R61] 磁盘占用
来源：http://phu.svipenyu.cn

df -h;  du -sh *
来源：http://zzl.fehbvm.com

[R62] 找最占空间的文件
来源：http://fvk.shangyingyoupin.top

du -ah . | sort -rh | head -10
来源：http://ipu.yonumen.top

[R63] 内存与进程
来源：http://ash.dashuyun.cn

free -h;  ps aux | grep nginx
来源：http://bga.jiagoushi.top

[R64] 结束进程
来源：http://enf.jinqigfzy.top

kill -9 $(pgrep -f app.py)
来源：http://ydh.yvedp.cn

[R65] 查看端口占用
来源：http://kbn.fehbvm.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://iyl.snrcjt.cn

[R66] 定时任务
来源：http://ofu.chenjidiqi.icu

crontab -e;  crontab -l
来源：http://tir.zdbjq.cn

[R67] 生成随机十六进制串
来源：http://cfj.pengpengdd.cyou

openssl rand -hex 16
来源：http://tqq.bjfxy.top

[R68] 计算文件校验值
来源：http://qal.xuanzx.com

sha256sum a.txt;  md5sum a.txt
来源：http://jig.nanxuanxn.top

[R69] 生成随机密码
来源：http://via.yueranfly.top

head -c 16 /dev/urandom | base64
来源：http://maq.fengsongda.top

[R70] 时间戳与互转
来源：http://lmy.hesvh.cn

date +%s;  date -d @1700000000
来源：http://nyy.smart0.xyz

[R71] 日期格式化
来源：http://nht.yuxming.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ogo.nanxinkj.top

[R72] 等待端口就绪
来源：http://vey.ydjk.org.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://wzn.xuanzx.com

[R73] 分割大日志
来源：http://dvx.jianghu66.top

split -l 1000 big.log part_
来源：http://nnh.sweek.top

[R74] 批量重命名
来源：http://btf.tianlin.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://chv.shuidangran.top

[R75] 导出环境变量
来源：http://bdl.chenjidiqi.icu

export PATH="$HOME/bin:$PATH"
来源：http://tkh.bjfxy.top

[R76] 使用临时文件
来源：http://hxd.zhoulong.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://abq.hammf.cn

[R77] 读取用户输入
来源：http://qsu.nanxinkj.top

read -rp "请输入: " ans
来源：http://sil.shangyingyoupin.top

[R78] 交互式菜单
来源：http://dba.zdbjq.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tus.gaohongyu789.top

[R79] 解析命令行选项
来源：http://tbr.iojbl.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rjr.ywan-chungtsiang.top

[R80] 查看脚本执行耗时
来源：http://yis.svipenyu.cn

time ./run.sh
来源：http://dsq.sweek.top

================================================================================
来源：http://aym.52xcode.cn

S. C / C++ 专题
来源：http://iqg.aibaodan.cn

================================================================================
来源：http://flv.bjfxy.top

[S01] C：Hello World
来源：http://cts.aibaodan.cn

#include <stdio.h>
来源：http://tjr.redwolf501.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://zlq.bjfxy.top

[S02] C：变量与格式化输出
来源：http://hpq.chenjidiqi.icu

int a = 10; printf("%d\n", a);
来源：http://twy.fehbvm.com

[S03] C：读入整数
来源：http://pwe.fehbvm.com

int x; scanf("%d", &x);
来源：http://ukk.ybcxt.top

[S04] C：字符串复制
来源：http://pzu.jiagoushi.top

char dst[32]; strcpy(dst, "hi");
来源：http://pyo.sweek.top

[S05] C：字符串长度
来源：http://oqb.fengsongda.top

strlen(s)
来源：http://wah.xuanzx.com

[S06] C：字符串比较
来源：http://zsz.xinyue.icu

strcmp(a, b) == 0
来源：http://xic.havefunace.top

[S07] C：数组遍历求和
来源：http://rtj.zhixingplan.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://num.uphjek.com

[S08] C：动态内存分配与释放
来源：http://qmj.sjlbkw.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ryz.zhixingplan.top

[S09] C：结构体定义与初始化
来源：http://glc.zhijiandao.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ooy.snrcjt.cn

[S10] C：指针与解引用
来源：http://sth.shanyushiyangkeji.top

int *p = &a;  *p = 5;
来源：http://xpk.c1oappe.top

[S11] C：逐行读文件
来源：http://aae.hcnkem.com

FILE *f = fopen("a.txt", "r");
来源：http://xou.bjfxy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://axd.zycfv.cn

fclose(f);
来源：http://hoa.epnwcf.com

[S12] C：写文件
来源：http://zwb.jinghuilouyu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hqp.redwolf501.top

[S13] C：宏定义
来源：http://ivf.xziqi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cgq.aizwys.cn

[S14] C：枚举
来源：http://rzu.haohaochexian.top

enum Color { RED, GREEN, BLUE };
来源：http://bxx.redwolf501.top

[S15] C：类型转换
来源：http://bwb.ivvv.top

(double) a / b
来源：http://oyu.jinqigfzy.top

[S16] C：位操作置位
来源：http://mph.haohaochexian.top

x |= (1 << 3);
来源：http://zdo.hcnkem.com

[S17] C：安全拼接字符串
来源：http://sqb.hnqzz.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://aew.ydzc1.top

[S18] C：命令行参数
来源：http://rzr.jqgufenzy.top

int main(int argc, char **argv)
来源：http://pgr.pycfn.com

[S19] C：快速排序
来源：http://qqi.chenzaomai.com

qsort(a, n, sizeof(int), cmp);
来源：http://qhh.tanke756.top

[S20] C：二分查找
来源：http://kbm.zhengqikj.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ewl.cdnleiting.top

[S21] C：字符类别判断
来源：http://ajc.yuxming.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dxy.zhongyouzk.top

[S22] C：字符串转数字
来源：http://zmi.xinyue.icu

atoi("42");  strtod("3.14", NULL);
来源：http://dtv.yvedp.cn

[S23] C：随机数
来源：http://ihm.hysaishi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://dpd.vehdjk.com

[S24] C：获取本地时间
来源：http://zch.tanke756.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xzu.feifeiyinyue.top

[S25] C：内存拷贝
来源：http://ueh.hesvh.cn

memcpy(dst, src, n);
来源：http://kpi.9152youxi.cn

[S26] C：内存清零
来源：http://kxi.ybcxt.top

memset(a, 0, sizeof a);
来源：http://ixz.haohaochexian.top

[S27] C：定义常量
来源：http://otp.daxiang520.top

const double PI = 3.14159;
来源：http://roe.yangfankeji.com

[S28] C：静态变量
来源：http://wcy.redwolf501.top

static int counter = 0;
来源：http://hzo.jyoumei.cn

[S29] C：变参函数
来源：http://hpl.yj20258888.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fsm.zycfv.cn

[S30] C：头文件保护
来源：http://alz.havefunace.top

#ifndef X_H
来源：http://ipm.c1oappe.top

#define X_H
来源：http://zmb.shangyingyoupin.top

#endif
来源：http://hkf.cucudq.cn

[S31] C++：Hello World
来源：http://hlx.jqgufenzy.top

#include <iostream>
来源：http://uzn.xuanzx.com

int main() { std::cout << "Hello\n"; }
来源：http://uqh.tianlin.xyz

[S32] C++：字符串
来源：http://srz.chenzaomai.com

std::string s = "hi";  s += "!";
来源：http://euc.uphjek.com

[S33] C++：vector 增删
来源：http://srl.sysykeji.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xgm.kuanghao11.cn

[S34] C++：遍历 vector
来源：http://hoc.shanyushiyangtech.top

for (auto &x : v) { std::cout << x; }
来源：http://phc.xingfuxueyuan.xyz

[S35] C++：map
来源：http://stn.haohaochexian.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://clw.gogol.net.cn

[S36] C++：unordered_map
来源：http://puj.hysaishi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kpl.aizwys.cn

[S37] C++：set
来源：http://set.52xcode.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hyw.shanyushiyangtech.top

[S38] C++：排序
来源：http://rpo.smart0.xyz

std::sort(v.begin(), v.end());
来源：http://ajl.dashuyun.cn

[S39] C++：自定义比较器排序
来源：http://xxz.uphjek.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xbs.zhongyouzk.top

[S40] C++：查找元素
来源：http://mjw.jqgfzy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jmv.yonumen.top

[S41] C++：类与构造函数
来源：http://dzn.jqgufenzy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ksg.jyoumei.cn

[S42] C++：继承与虚函数
来源：http://yum.hywenlv.cn

class B : public Base { public: void f() override {} };
来源：http://fsx.dashuyun.cn

[S43] C++：智能指针
来源：http://dvp.sweek.top

auto p = std::make_unique<int>(5);
来源：http://csu.svipenyu.cn

[S44] C++：引用传参
来源：http://hlv.hnqzz.top

void inc(int &x) { ++x; }
来源：http://bie.c1oappe.top

[S45] C++：lambda
来源：http://yrz.xuanzx.com

auto add = [](int a, int b) { return a + b; };
来源：http://mkp.sxryk.cn

[S46] C++：函数模板
来源：http://foy.havefunace.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://omh.bbcook.cn

[S47] C++：结构化绑定遍历
来源：http://mza.nwbrower.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ypx.yonumen.top

[S48] C++：逐行读文件
来源：http://zpz.pycfn.com

std::ifstream in("a.txt");  std::string line;
来源：http://dzy.hammf.cn

while (std::getline(in, line)) { }
来源：http://txz.ivvv.top

[S49] C++：写文件
来源：http://afb.xinyue.icu

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vyd.zdbjq.cn

[S50] C++：格式化数字
来源：http://xen.fehbvm.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://evt.pengpengdd.cyou

[S51] C++：显式类型转换
来源：http://bda.mhx1999.top

static_cast<double>(a) / b
来源：http://woa.jiagoushi.top

[S52] C++：const 与 noexcept
来源：http://vxt.smart0.xyz

int size() const noexcept { return n_; }
来源：http://ame.fehbvm.com

[S53] C++：移动语义
来源：http://zme.ppjwa.cn

std::vector<int> w = std::move(v);
来源：http://fvx.chenzaomai.com

[S54] C++：异常处理
来源：http://don.ctjpmb.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ium.shanyushiyangkeji.top

[S55] C++：结构化绑定
来源：http://xij.xingfuxueyuan.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://qtp.kuanghao11.cn

[S56] C++：optional
来源：http://dqf.jyoumei.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rns.aibaodan.cn

[S57] C++：编译期常量
来源：http://cnj.yj20258.top

constexpr int N = 10;
来源：http://cpb.chenlongwang.top

[S58] C++：命名空间
来源：http://gak.ehwqpu.com

namespace ns { int f() { return 1; } }
来源：http://ynk.hesvh.cn

[S59] C++：静态断言
来源：http://tip.wangshuangyany.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://has.yj20258.top

[S60] C++：遍历并删除元素
来源：http://qrf.aibaodan.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://uic.316326.xyz

================================================================================
来源：http://dip.ctjpmb.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mix.chenjidiqi.icu

================================================================================
来源：http://hdj.tianlin.xyz

[T01] Kotlin：Hello World
来源：http://ann.yvedp.cn

println("Hello")
来源：http://bmc.sxryk.cn

[T02] Kotlin：变量
来源：http://vwt.fktsv.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pqg.xylfe.cn

[T03] Kotlin：字符串模板
来源：http://ukg.aizwys.cn

"值: $b"
来源：http://fop.pycfn.com

[T04] Kotlin：空安全
来源：http://kph.yonumen.top

val n: String? = null;  n?.length
来源：http://duh.uphjek.com

[T05] Kotlin：when 表达式
来源：http://efn.guowangkeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://owp.yongpay.top

[T06] Kotlin：集合映射
来源：http://ryw.jiagoushi.top

listOf(1, 2, 3).map { it * 2 }
来源：http://oas.shzxlz.cn

[T07] Kotlin：集合过滤
来源：http://mte.cdnleiting.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://imc.jlsjyb.cn

[T08] Kotlin：数据类
来源：http://bge.bjfxy.top

data class User(val name: String, val age: Int)
来源：http://rws.zhoulong.xyz

[T09] Kotlin：扩展函数
来源：http://moa.shangyingyoupin.top

fun String.exclaim() = this + "!"
来源：http://qhg.shanyushiyangtech.top

[T10] Kotlin：默认参数
来源：http://irb.sysykeji.top

fun greet(name: String = "World") = "Hi $name"
来源：http://yry.fengsongda.top

[T11] Kotlin：协程
来源：http://xdz.xingfuxueyuan.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://nmq.ydzc1.top

[T12] Kotlin：解构声明
来源：http://idb.yvedp.cn

val (a, b) = Pair(1, 2)
来源：http://nvk.redwolf501.top

[T13] Kotlin：只读 Map
来源：http://gcp.bjfxy.top

val m = mapOf("a" to 1)
来源：http://ars.hesvh.cn

[T14] Kotlin：循环
来源：http://ecj.jiagoushi.top

for (i in 1..10) println(i)
来源：http://lnu.jqgfzy.top

[T15] Kotlin：接口
来源：http://mpt.bbcook.cn

interface Shape { fun area(): Double }
来源：http://rst.cucudq.cn

[T16] Swift：Hello World
来源：http://uth.xingfuxueyuan.xyz

print("Hello")
来源：http://ymi.jianghu66.top

[T17] Swift：变量与常量
来源：http://uug.zhixingplan.top

var a = 1;  let b = 2
来源：http://iul.yonumen.top

[T18] Swift：字符串插值
来源：http://vji.zhijiandao.cn

"值: \(b)"
来源：http://rlr.birdmap.top

[T19] Swift：可选绑定
来源：http://ssp.jinghuilouyu.cn

if let n = opt { print(n) }
来源：http://fnh.jlsjyb.cn

[T20] Swift：数组操作
来源：http://cxl.yuanzhike.top

var a = [1, 2, 3];  a.append(4)
来源：http://qmm.daxiang520.top

[T21] Swift：遍历
来源：http://ymw.redwolf501.top

for x in a { print(x) }
来源：http://zvs.ybcxt.top

[T22] Swift：字典
来源：http://vkx.yj20258888.top

var d = ["a": 1];  d["b"] = 2
来源：http://dgz.shanyushiyangtech.top

[T23] Swift：函数
来源：http://dfw.shzxlz.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cck.yuxming.cn

[T24] Swift：闭包
来源：http://naf.jinghuilouyu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://svh.nanxuanxn.top

[T25] Swift：结构体
来源：http://slu.dianchejie.cn

struct P { var x: Int }
来源：http://igx.uphjek.com

[T26] Swift：类与重写
来源：http://uxs.c1oappe.top

class A: Base { override func f() {} }
来源：http://ijx.hfpthk.cn

[T27] Swift：错误处理
来源：http://hms.sweek.top

do { try f() } catch { print(error) }
来源：http://wmk.mhx1999.top

[T28] Swift：枚举
来源：http://gvm.andypj.xyz

enum Color { case red, green }
来源：http://gyk.meibo888.top

[T29] Swift：guard 提前返回
来源：http://rga.tian-w.cn

guard let x = opt else { return }
来源：http://fov.ehwqpu.com

[T30] Swift：协议
来源：http://gpl.yanxiufei.cn

protocol Shape { func area() -> Double }
来源：http://uxx.xinyue.icu

[T31] Lua：Hello World
来源：http://sqr.nanxuanxn.top

print("Hello")
来源：http://xbm.quarkkingdee.top

[T32] Lua：局部变量
来源：http://szk.sxryk.cn

local a = 1
来源：http://tyx.gogol.net.cn

[T33] Lua：表（数组）
来源：http://utm.sweek.top

local t = {1, 2, 3};  t[4] = 4
来源：http://kre.zhixingplan.top

[T34] Lua：遍历表
来源：http://xiz.yanxiufei.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://lnf.snrcjt.cn

[T35] Lua：字典表
来源：http://wmd.iojbl.cn

local d = { a = 1 };  d.b = 2
来源：http://xtq.epnwcf.com

[T36] Lua：函数
来源：http://lag.shuidangran.top

function add(a, b) return a + b end
来源：http://wmu.nanxinkj.top

[T37] Lua：字符串拼接
来源：http://cgr.smart0.xyz

"a" .. "b"
来源：http://lqr.daria6918.cn

[T38] Lua：条件
来源：http://itt.haohaochexian.top

if x > 0 then print("正") end
来源：http://owt.ydzc1.top

[T39] Lua：模式匹配
来源：http://oga.aibaodan.cn

string.find(s, "%d+")
来源：http://pqh.hcnkem.com

[T40] Lua：元表
来源：http://unu.chenjidiqi.icu

setmetatable({}, { __index = base })
来源：http://sme.vehdjk.com

[T41] Perl：Hello World
来源：http://img.jinqigufen.top

print "Hello\n";
来源：http://ycc.tanke756.top

[T42] Perl：变量类型
来源：http://wkp.jinqigufen.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rhm.ppjwa.cn

[T43] Perl：字符串插值
来源：http://ymu.jinyuanbaomall.cn

"值: $a"
来源：http://ftq.gaohongyu789.top

[T44] Perl：条件
来源：http://iyg.yj20258888.top

if ($a > 0) { print "正"; }
来源：http://tty.yj20258.top

[T45] Perl：数组遍历
来源：http://qls.havefunace.top

for my $x (@arr) { print $x; }
来源：http://xtp.epnwcf.com

[T46] Perl：哈希操作
来源：http://cyy.jlsjyb.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tcr.zdqjudy.top

[T47] Perl：正则捕获
来源：http://dfu.dianchejie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://dfz.birdmap.top

[T48] Perl：正则替换
来源：http://dmp.pycfn.com

$s =~ s/old/new/g;
来源：http://ogv.wangshuangyany.cn

[T49] Perl：函数
来源：http://pzt.dianchejie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wuw.jinyuanbaomall.cn

[T50] Perl：逐行读文件
来源：http://lqk.gotoacloud.top

open my $fh, "<", "a.txt" or die $!;
来源：http://uft.svipenyu.cn

while (my $line = <$fh>) { print $line; }
来源：http://ift.chenzaomai.com

[T51] Scala：Hello World
来源：http://cqk.ppjwa.cn

println("Hello")
来源：http://yjw.cheryme.top

[T52] Scala：变量
来源：http://vuz.hnxiangtu.top

val a = 1;  var b = 2
来源：http://mzn.yj20258.top

[T53] Scala：字符串插值
来源：http://uve.guannengcc.top

s"值: $b"
来源：http://icz.zhongyouzk.top

[T54] Scala：集合映射
来源：http://sfl.sufxvd.cn

List(1, 2, 3).map(_ * 2)
来源：http://mub.aibaodan.cn

[T55] Scala：集合过滤
来源：http://rph.sufxvd.cn

List(1, 2, 3).filter(_ > 1)
来源：http://kab.yj20258.top

[T56] Scala：样例类
来源：http://exn.chenjidiqi.icu

case class User(name: String, age: Int)
来源：http://gtm.hnxiangtu.top

[T57] Scala：模式匹配
来源：http://uzu.yj202588.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://frm.shanyushiyangtech.top

[T58] Scala：函数定义
来源：http://rdu.yvedp.cn

def add(a: Int, b: Int): Int = a + b
来源：http://cgx.hesvh.cn

[T59] Scala：循环
来源：http://mhy.xylfe.cn

for (i <- 1 to 10) println(i)
来源：http://bvq.gotoacloud.top

[T60] Scala：折叠
来源：http://ofw.yuanzhike.top


<!-- 参考信息 -->