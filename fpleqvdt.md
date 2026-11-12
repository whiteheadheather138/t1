代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cvp.fanxiaobao.xyz

[R60] 只看 HTTP 状态码
来源：http://abv.cucudq.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://axo.guannengcc.top

[R61] 磁盘占用
来源：http://ybc.fehbvm.com

df -h;  du -sh *
来源：http://jzw.fanxiaobao.xyz

[R62] 找最占空间的文件
来源：http://zjm.yj20258888.top

du -ah . | sort -rh | head -10
来源：http://kyw.hammf.cn

[R63] 内存与进程
来源：http://imw.sxryk.cn

free -h;  ps aux | grep nginx
来源：http://oop.gogol.net.cn

[R64] 结束进程
来源：http://rgv.shanyushiyangkeji.top

kill -9 $(pgrep -f app.py)
来源：http://yyr.yanxiufei.cn

[R65] 查看端口占用
来源：http://ksr.ppjwa.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jfy.feifeiyinyue.top

[R66] 定时任务
来源：http://eld.jinqigufen.top

crontab -e;  crontab -l
来源：http://hhu.jinqigufen.top

[R67] 生成随机十六进制串
来源：http://rnu.sxryk.cn

openssl rand -hex 16
来源：http://vda.bjfxy.top

[R68] 计算文件校验值
来源：http://pns.zhijiandao.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ciw.jqgufenzy.top

[R69] 生成随机密码
来源：http://zmq.shangyingyoupin.top

head -c 16 /dev/urandom | base64
来源：http://dfp.jlsjyb.cn

[R70] 时间戳与互转
来源：http://eej.yj202588.top

date +%s;  date -d @1700000000
来源：http://qlz.aibaodan.cn

[R71] 日期格式化
来源：http://pnc.shuidangran.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://omn.kuanghao11.cn

[R72] 等待端口就绪
来源：http://rqg.tanke756.top

until nc -z localhost 3306; do sleep 1; done
来源：http://aur.fengsongda.top

[R73] 分割大日志
来源：http://fxl.hesvh.cn

split -l 1000 big.log part_
来源：http://kpk.bjfxy.top

[R74] 批量重命名
来源：http://csu.pengpengdd.cyou

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://urz.andypj.xyz

[R75] 导出环境变量
来源：http://gpb.guowangkeji.top

export PATH="$HOME/bin:$PATH"
来源：http://pyv.bjfxy.top

[R76] 使用临时文件
来源：http://jix.shangyingyoupin.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ass.feifeiyinyue.top

[R77] 读取用户输入
来源：http://keg.pycfn.com

read -rp "请输入: " ans
来源：http://clf.xuanzx.com

[R78] 交互式菜单
来源：http://wsx.ctjpmb.com

select opt in a b c; do echo "$opt"; break; done
来源：http://kxz.cqqwz.cn

[R79] 解析命令行选项
来源：http://xch.xuetiantiany.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pff.hnxiangtu.top

[R80] 查看脚本执行耗时
来源：http://eoy.yongpay.top

time ./run.sh
来源：http://ngi.xuetiantiany.cn

================================================================================
来源：http://jvg.chenzaomai.com

S. C / C++ 专题
来源：http://bdx.guannengcc.top

================================================================================
来源：http://jdb.zdqjudy.top

[S01] C：Hello World
来源：http://snf.wangdashe.top

#include <stdio.h>
来源：http://rvc.yangfankeji.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://oiv.sjlbkw.cn

[S02] C：变量与格式化输出
来源：http://jwu.quarkkingdee.top

int a = 10; printf("%d\n", a);
来源：http://myx.bjfxy.top

[S03] C：读入整数
来源：http://hvy.cashguo.top

int x; scanf("%d", &x);
来源：http://fvi.cheryme.top

[S04] C：字符串复制
来源：http://onf.havefunace.top

char dst[32]; strcpy(dst, "hi");
来源：http://nmg.ydzc1.top

[S05] C：字符串长度
来源：http://mmn.xylfe.cn

strlen(s)
来源：http://inm.haohaochexian.top

[S06] C：字符串比较
来源：http://zik.smart0.xyz

strcmp(a, b) == 0
来源：http://sig.ydzc1.top

[S07] C：数组遍历求和
来源：http://jlc.shangyingyoupin.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bll.yj202588.top

[S08] C：动态内存分配与释放
来源：http://iui.havefunace.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://oqg.guannengcc.top

[S09] C：结构体定义与初始化
来源：http://pvx.quarkkingdee.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uvk.ydjk.org.cn

[S10] C：指针与解引用
来源：http://abq.bjfxy.top

int *p = &a;  *p = 5;
来源：http://xww.sjlbkw.cn

[S11] C：逐行读文件
来源：http://tzn.andypj.xyz

FILE *f = fopen("a.txt", "r");
来源：http://mky.epnwcf.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://usd.fktsv.cn

fclose(f);
来源：http://pau.hywenlv.cn

[S12] C：写文件
来源：http://iwu.jlsjyb.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wuc.daria6918.cn

[S13] C：宏定义
来源：http://cuh.uphjek.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ezi.hfpthk.cn

[S14] C：枚举
来源：http://ezg.tarul.cn

enum Color { RED, GREEN, BLUE };
来源：http://qvu.cashguo.top

[S15] C：类型转换
来源：http://bgp.ctjpmb.com

(double) a / b
来源：http://gpo.ppjwa.cn

[S16] C：位操作置位
来源：http://iaz.nanxinkj.top

x |= (1 << 3);
来源：http://nxo.hongshengwenyu.top

[S17] C：安全拼接字符串
来源：http://uza.zhixingplan.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mmp.hfpthk.cn

[S18] C：命令行参数
来源：http://tba.fehbvm.com

int main(int argc, char **argv)
来源：http://ihi.zhongyouzk.top

[S19] C：快速排序
来源：http://cdb.kuanghao11.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ahv.cheryme.top

[S20] C：二分查找
来源：http://pkr.zhongyouzk.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://olr.bjfxy.top

[S21] C：字符类别判断
来源：http://gcr.jinqigfzy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ptc.xylfe.cn

[S22] C：字符串转数字
来源：http://dcg.daria6918.cn

atoi("42");  strtod("3.14", NULL);
来源：http://gkt.yonumen.top

[S23] C：随机数
来源：http://hrt.shzxlz.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qlf.guowangkeji.top

[S24] C：获取本地时间
来源：http://kim.kuanghao11.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ete.cqqwz.cn

[S25] C：内存拷贝
来源：http://dsx.zdqjudy.top

memcpy(dst, src, n);
来源：http://pvd.9152youxi.cn

[S26] C：内存清零
来源：http://wdl.ybcxt.top

memset(a, 0, sizeof a);
来源：http://iyi.zhongyouzk.top

[S27] C：定义常量
来源：http://yru.sjlbkw.cn

const double PI = 3.14159;
来源：http://oci.hcnkem.com

[S28] C：静态变量
来源：http://zwt.daria6918.cn

static int counter = 0;
来源：http://nzp.sufxvd.cn

[S29] C：变参函数
来源：http://ofe.havefunace.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://evb.zhijiandao.cn

[S30] C：头文件保护
来源：http://vpl.jinqigufen.top

#ifndef X_H
来源：http://psk.uphjek.com

#define X_H
来源：http://kli.xziqi.cn

#endif
来源：http://tun.gzhubu.top

[S31] C++：Hello World
来源：http://dtc.hnqzz.top

#include <iostream>
来源：http://rwz.dianchejie.cn

int main() { std::cout << "Hello\n"; }
来源：http://edx.cheryme.top

[S32] C++：字符串
来源：http://gow.hfpthk.cn

std::string s = "hi";  s += "!";
来源：http://nlp.yj20258888.top

[S33] C++：vector 增删
来源：http://xaw.redwolf501.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nuc.316326.xyz

[S34] C++：遍历 vector
来源：http://ffd.zhixingplan.top

for (auto &x : v) { std::cout << x; }
来源：http://ube.pycfn.com

[S35] C++：map
来源：http://ktk.fzhhl.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bji.cheryme.top

[S36] C++：unordered_map
来源：http://daw.shzxlz.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lws.ehwqpu.com

[S37] C++：set
来源：http://dkh.daxiang520.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vgg.nanxinkj.top

[S38] C++：排序
来源：http://sui.chenjidiqi.icu

std::sort(v.begin(), v.end());
来源：http://ion.xuanzx.com

[S39] C++：自定义比较器排序
来源：http://pjm.jinqigfzy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sla.zycfv.cn

[S40] C++：查找元素
来源：http://zny.guannengcc.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://duq.jianghu66.top

[S41] C++：类与构造函数
来源：http://afn.tanke756.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gdu.9152youxi.cn

[S42] C++：继承与虚函数
来源：http://cmf.hesvh.cn

class B : public Base { public: void f() override {} };
来源：http://hfs.wangdashe.top

[S43] C++：智能指针
来源：http://mlg.xylfe.cn

auto p = std::make_unique<int>(5);
来源：http://kqh.cheryme.top

[S44] C++：引用传参
来源：http://dfi.shuidangran.top

void inc(int &x) { ++x; }
来源：http://vnm.fzhhl.top

[S45] C++：lambda
来源：http://tmg.jinqigufen.top

auto add = [](int a, int b) { return a + b; };
来源：http://ibn.jianghu66.top

[S46] C++：函数模板
来源：http://nqt.epnwcf.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cjl.zycfv.cn

[S47] C++：结构化绑定遍历
来源：http://hob.xingfuxueyuan.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ipo.iojbl.cn

[S48] C++：逐行读文件
来源：http://rho.ivvv.top

std::ifstream in("a.txt");  std::string line;
来源：http://gag.sxryk.cn

while (std::getline(in, line)) { }
来源：http://dvl.tian-w.cn

[S49] C++：写文件
来源：http://nsg.hesvh.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mjc.daxiang520.top

[S50] C++：格式化数字
来源：http://vrt.redwolf501.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ast.jinghuilouyu.cn

[S51] C++：显式类型转换
来源：http://aky.pengpengdd.cyou

static_cast<double>(a) / b
来源：http://rqv.jinyuanbaomall.cn

[S52] C++：const 与 noexcept
来源：http://jbl.tanke756.top

int size() const noexcept { return n_; }
来源：http://gtb.hysaishi.cn

[S53] C++：移动语义
来源：http://fkf.hongshengwenyu.top

std::vector<int> w = std::move(v);
来源：http://zdy.yongpay.top

[S54] C++：异常处理
来源：http://bhg.wangdashe.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ppr.epnwcf.com

[S55] C++：结构化绑定
来源：http://uzg.zhiwuduotai.top

auto [a, b] = std::make_pair(1, 2);
来源：http://tuv.pycfn.com

[S56] C++：optional
来源：http://svo.316326.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ugw.sysykeji.top

[S57] C++：编译期常量
来源：http://vci.nwbrower.top

constexpr int N = 10;
来源：http://unx.zhoulong.xyz

[S58] C++：命名空间
来源：http://kkz.shangyingyoupin.top

namespace ns { int f() { return 1; } }
来源：http://wwq.tianlin.xyz

[S59] C++：静态断言
来源：http://juo.0kj1m.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lff.jyoumei.cn

[S60] C++：遍历并删除元素
来源：http://szr.svipenyu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://oau.uphjek.com

================================================================================
来源：http://ryu.xinyue.icu

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tob.nanxinkj.top

================================================================================
来源：http://put.gaohongyu789.top

[T01] Kotlin：Hello World
来源：http://vcr.fehbvm.com

println("Hello")
来源：http://fsw.gogol.net.cn

[T02] Kotlin：变量
来源：http://jtt.yangfankeji.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kva.vehdjk.com

[T03] Kotlin：字符串模板
来源：http://krb.zycfv.cn

"值: $b"
来源：http://vde.bjfxy.top

[T04] Kotlin：空安全
来源：http://obx.fzhhl.top

val n: String? = null;  n?.length
来源：http://noy.meibo888.top

[T05] Kotlin：when 表达式
来源：http://hqn.xuanzx.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://znj.guowangkeji.top

[T06] Kotlin：集合映射
来源：http://mgd.jinyuanbaomall.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://umg.shzxlz.cn

[T07] Kotlin：集合过滤
来源：http://loc.fanxiaobao.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://bqn.xuanzx.com

[T08] Kotlin：数据类
来源：http://orf.xuetiantiany.cn

data class User(val name: String, val age: Int)
来源：http://eow.tanke756.top

[T09] Kotlin：扩展函数
来源：http://gjv.ybcxt.top

fun String.exclaim() = this + "!"
来源：http://cqp.ctjpmb.com

[T10] Kotlin：默认参数
来源：http://hah.nanxinkj.top

fun greet(name: String = "World") = "Hi $name"
来源：http://dka.gaohongyu789.top

[T11] Kotlin：协程
来源：http://vsw.sjlbkw.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qkd.sweek.top

[T12] Kotlin：解构声明
来源：http://ujf.xingfuxueyuan.xyz

val (a, b) = Pair(1, 2)
来源：http://vcx.quarkkingdee.top

[T13] Kotlin：只读 Map
来源：http://cur.fzhhl.top

val m = mapOf("a" to 1)
来源：http://qep.vqdsnc.cn

[T14] Kotlin：循环
来源：http://jzh.gotoacloud.top

for (i in 1..10) println(i)
来源：http://xor.sysykeji.top

[T15] Kotlin：接口
来源：http://ayz.wangdashe.top

interface Shape { fun area(): Double }
来源：http://bbd.fanxiaobao.xyz

[T16] Swift：Hello World
来源：http://qsn.ctjpmb.com

print("Hello")
来源：http://odf.tarul.cn

[T17] Swift：变量与常量
来源：http://nny.jiagoushi.top

var a = 1;  let b = 2
来源：http://ica.bbcook.cn

[T18] Swift：字符串插值
来源：http://ude.fengsongda.top

"值: \(b)"
来源：http://cnu.sjlbkw.cn

[T19] Swift：可选绑定
来源：http://csw.zhaomingkeji.xyz

if let n = opt { print(n) }
来源：http://yrr.yfazqb.com

[T20] Swift：数组操作
来源：http://pvo.chenjidiqi.icu

var a = [1, 2, 3];  a.append(4)
来源：http://ybu.nanxinkj.top

[T21] Swift：遍历
来源：http://pqq.iojbl.cn

for x in a { print(x) }
来源：http://nyq.ydzc1.top

[T22] Swift：字典
来源：http://nog.yj202588.top

var d = ["a": 1];  d["b"] = 2
来源：http://nco.jinghuilouyu.cn

[T23] Swift：函数
来源：http://aun.epnwcf.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://iex.sweek.top

[T24] Swift：闭包
来源：http://gjc.dashuyun.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vxy.jlsjyb.cn

[T25] Swift：结构体
来源：http://wdq.xingfuxueyuan.xyz

struct P { var x: Int }
来源：http://diq.birdmap.top

[T26] Swift：类与重写
来源：http://gpl.0kj1m.cn

class A: Base { override func f() {} }
来源：http://zkh.zhengqikj.top

[T27] Swift：错误处理
来源：http://myb.quarkkingdee.top

do { try f() } catch { print(error) }
来源：http://pfy.xziqi.cn

[T28] Swift：枚举
来源：http://bvi.cheryme.top

enum Color { case red, green }
来源：http://pdh.hysaishi.cn

[T29] Swift：guard 提前返回
来源：http://mat.ybcxt.top

guard let x = opt else { return }
来源：http://iwk.yonumen.top

[T30] Swift：协议
来源：http://dap.vehdjk.com

protocol Shape { func area() -> Double }
来源：http://mqh.xuanzx.com

[T31] Lua：Hello World
来源：http://djp.aibaodan.cn

print("Hello")
来源：http://gnj.ybcxt.top

[T32] Lua：局部变量
来源：http://ikn.yvedp.cn

local a = 1
来源：http://dcp.sjlbkw.cn

[T33] Lua：表（数组）
来源：http://bll.zhoulong.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://jka.mhx1999.top

[T34] Lua：遍历表
来源：http://nbg.fengsongda.top

for i, v in ipairs(t) do print(i, v) end
来源：http://lvn.hammf.cn

[T35] Lua：字典表
来源：http://xab.jyoumei.cn

local d = { a = 1 };  d.b = 2
来源：http://phj.shanyushiyangkeji.top

[T36] Lua：函数
来源：http://yit.meibo888.top

function add(a, b) return a + b end
来源：http://etf.gotoacloud.top

[T37] Lua：字符串拼接
来源：http://ksl.feifeiyinyue.top

"a" .. "b"
来源：http://ing.meibo888.top

[T38] Lua：条件
来源：http://uni.52xcode.cn

if x > 0 then print("正") end
来源：http://iuk.chenjidiqi.icu

[T39] Lua：模式匹配
来源：http://enn.wangshuangyany.cn

string.find(s, "%d+")
来源：http://iqe.iojbl.cn

[T40] Lua：元表
来源：http://kob.chenjidiqi.icu

setmetatable({}, { __index = base })
来源：http://vyd.sjlbkw.cn

[T41] Perl：Hello World
来源：http://son.zhijiandao.cn

print "Hello\n";
来源：http://vkd.zhaomingkeji.xyz

[T42] Perl：变量类型
来源：http://rte.haohaochexian.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wiq.ybcxt.top

[T43] Perl：字符串插值
来源：http://zyw.zhoulong.xyz

"值: $a"
来源：http://ujj.shanyushiyangtech.top

[T44] Perl：条件
来源：http://jwu.cqqwz.cn

if ($a > 0) { print "正"; }
来源：http://xym.0kj1m.cn

[T45] Perl：数组遍历
来源：http://roe.gzhubu.top

for my $x (@arr) { print $x; }
来源：http://qxi.vehdjk.com

[T46] Perl：哈希操作
来源：http://wan.dianchejie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jko.jqgfzy.top

[T47] Perl：正则捕获
来源：http://yos.hesvh.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qyu.zycfv.cn

[T48] Perl：正则替换
来源：http://hnr.nanxinkj.top

$s =~ s/old/new/g;
来源：http://pqq.yj20258888.top

[T49] Perl：函数
来源：http://gbv.cheryme.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://spf.pycfn.com

[T50] Perl：逐行读文件
来源：http://pax.ehwqpu.com

open my $fh, "<", "a.txt" or die $!;
来源：http://jkr.vqdsnc.cn

while (my $line = <$fh>) { print $line; }
来源：http://cbd.yueranfly.top

[T51] Scala：Hello World
来源：http://orq.jqgfzy.top

println("Hello")
来源：http://lgo.dashuyun.cn

[T52] Scala：变量
来源：http://wwk.aizwys.cn

val a = 1;  var b = 2
来源：http://zje.jinyuanbaomall.cn

[T53] Scala：字符串插值
来源：http://hna.fanxiaobao.xyz

s"值: $b"
来源：http://lfv.zdbjq.cn

[T54] Scala：集合映射
来源：http://yqj.yueranfly.top

List(1, 2, 3).map(_ * 2)
来源：http://edl.dashuyun.cn

[T55] Scala：集合过滤
来源：http://yuo.ppjwa.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wtb.yj202588.top

[T56] Scala：样例类
来源：http://njz.xylfe.cn

case class User(name: String, age: Int)
来源：http://sdd.jqgfzy.top

[T57] Scala：模式匹配
来源：http://rem.zhengqikj.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://cme.xinyue.icu

[T58] Scala：函数定义
来源：http://uye.yj202588.top

def add(a: Int, b: Int): Int = a + b
来源：http://ttt.0kj1m.cn

[T59] Scala：循环
来源：http://lkj.jinqigfzy.top

for (i <- 1 to 10) println(i)
来源：http://mwf.yj202588.top

[T60] Scala：折叠
来源：http://alm.shanyushiyangkeji.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vou.jinqigfzy.top

================================================================================
来源：http://cyv.zhengqikj.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://gdq.epnwcf.com

================================================================================
来源：http://maw.jyoumei.cn


<!-- 参考信息 -->