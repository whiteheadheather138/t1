代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qcp.daxiang520.top

[R60] 只看 HTTP 状态码
来源：http://xgb.bjfxy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kbz.pengpengdd.cyou

[R61] 磁盘占用
来源：http://kjs.hcnkem.com

df -h;  du -sh *
来源：http://isz.zhongyouzk.top

[R62] 找最占空间的文件
来源：http://hwt.jinqigfzy.top

du -ah . | sort -rh | head -10
来源：http://epg.jinqigfzy.top

[R63] 内存与进程
来源：http://wix.chenjidiqi.icu

free -h;  ps aux | grep nginx
来源：http://yqx.jinghuilouyu.cn

[R64] 结束进程
来源：http://gfy.jlsjyb.cn

kill -9 $(pgrep -f app.py)
来源：http://wkv.cqqwz.cn

[R65] 查看端口占用
来源：http://dtl.cucudq.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yjm.jiagoushi.top

[R66] 定时任务
来源：http://flq.svipenyu.cn

crontab -e;  crontab -l
来源：http://sse.ehwqpu.com

[R67] 生成随机十六进制串
来源：http://yef.fengsongda.top

openssl rand -hex 16
来源：http://uwd.zycfv.cn

[R68] 计算文件校验值
来源：http://xgt.yj20258.top

sha256sum a.txt;  md5sum a.txt
来源：http://snw.tarul.cn

[R69] 生成随机密码
来源：http://pak.shzxlz.cn

head -c 16 /dev/urandom | base64
来源：http://rqf.ctjpmb.com

[R70] 时间戳与互转
来源：http://vih.tian-w.cn

date +%s;  date -d @1700000000
来源：http://ciw.andypj.xyz

[R71] 日期格式化
来源：http://jks.jianghu66.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://fsq.shuidangran.top

[R72] 等待端口就绪
来源：http://nsu.dianchejie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jof.fanxiaobao.xyz

[R73] 分割大日志
来源：http://nky.daxiang520.top

split -l 1000 big.log part_
来源：http://oht.cdnleiting.top

[R74] 批量重命名
来源：http://tmd.pengpengdd.cyou

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mnx.ehwqpu.com

[R75] 导出环境变量
来源：http://bbg.aibaodan.cn

export PATH="$HOME/bin:$PATH"
来源：http://msd.haohaochexian.top

[R76] 使用临时文件
来源：http://jlx.yonumen.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://czf.sysykeji.top

[R77] 读取用户输入
来源：http://qlf.andypj.xyz

read -rp "请输入: " ans
来源：http://jnn.hywenlv.cn

[R78] 交互式菜单
来源：http://nom.tarul.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tsv.jinqigfzy.top

[R79] 解析命令行选项
来源：http://czg.xinyue.icu

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yhq.sxryk.cn

[R80] 查看脚本执行耗时
来源：http://sop.xuetiantiany.cn

time ./run.sh
来源：http://zyd.xingfuxueyuan.xyz

================================================================================
来源：http://tpu.ppjwa.cn

S. C / C++ 专题
来源：http://mun.yuanzhike.top

================================================================================
来源：http://pxa.jiagoushi.top

[S01] C：Hello World
来源：http://kqk.fehbvm.com

#include <stdio.h>
来源：http://kvu.fehbvm.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://kej.dashuyun.cn

[S02] C：变量与格式化输出
来源：http://nrn.yuanzhike.top

int a = 10; printf("%d\n", a);
来源：http://jgf.shanyushiyangkeji.top

[S03] C：读入整数
来源：http://aur.316326.xyz

int x; scanf("%d", &x);
来源：http://mhd.snrcjt.cn

[S04] C：字符串复制
来源：http://pyd.ehwqpu.com

char dst[32]; strcpy(dst, "hi");
来源：http://jma.daria6918.cn

[S05] C：字符串长度
来源：http://rji.yongpay.top

strlen(s)
来源：http://oce.cheryme.top

[S06] C：字符串比较
来源：http://jyx.feifeiyinyue.top

strcmp(a, b) == 0
来源：http://xwm.9152youxi.cn

[S07] C：数组遍历求和
来源：http://fjv.pycfn.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://phh.dashuyun.cn

[S08] C：动态内存分配与释放
来源：http://tpv.guowangkeji.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yqy.hammf.cn

[S09] C：结构体定义与初始化
来源：http://fja.xziqi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://psv.fzhhl.top

[S10] C：指针与解引用
来源：http://nkf.zycfv.cn

int *p = &a;  *p = 5;
来源：http://ylx.zdqjudy.top

[S11] C：逐行读文件
来源：http://oxz.sufxvd.cn

FILE *f = fopen("a.txt", "r");
来源：http://ioa.daria6918.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ovk.jinqigfzy.top

fclose(f);
来源：http://qwy.bjfxy.top

[S12] C：写文件
来源：http://ick.nanxinkj.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jep.jianghu66.top

[S13] C：宏定义
来源：http://hll.chenzaomai.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zfw.jinyuanbaomall.cn

[S14] C：枚举
来源：http://dkl.jiagoushi.top

enum Color { RED, GREEN, BLUE };
来源：http://vwn.hammf.cn

[S15] C：类型转换
来源：http://snf.ydzc1.top

(double) a / b
来源：http://fyc.yj20258888.top

[S16] C：位操作置位
来源：http://qxc.smart0.xyz

x |= (1 << 3);
来源：http://lvo.tarul.cn

[S17] C：安全拼接字符串
来源：http://mcw.cheryme.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://aay.xylfe.cn

[S18] C：命令行参数
来源：http://lil.0kj1m.cn

int main(int argc, char **argv)
来源：http://diy.jinqigfzy.top

[S19] C：快速排序
来源：http://wwn.fehbvm.com

qsort(a, n, sizeof(int), cmp);
来源：http://qgo.iojbl.cn

[S20] C：二分查找
来源：http://yow.tianlin.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wjz.yanxiufei.cn

[S21] C：字符类别判断
来源：http://ize.svipenyu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://izh.fktsv.cn

[S22] C：字符串转数字
来源：http://bhy.zhijiandao.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xsn.daxiang520.top

[S23] C：随机数
来源：http://uxd.yongpay.top

srand(time(NULL));  int r = rand() % 100;
来源：http://egm.cqqwz.cn

[S24] C：获取本地时间
来源：http://yui.fzhhl.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://onk.hysaishi.cn

[S25] C：内存拷贝
来源：http://qyh.fehbvm.com

memcpy(dst, src, n);
来源：http://oes.dashuyun.cn

[S26] C：内存清零
来源：http://hhy.guannengcc.top

memset(a, 0, sizeof a);
来源：http://pnw.feifeiyinyue.top

[S27] C：定义常量
来源：http://xes.cheryme.top

const double PI = 3.14159;
来源：http://jkh.jlsjyb.cn

[S28] C：静态变量
来源：http://lgo.jqgufenzy.top

static int counter = 0;
来源：http://gyd.ivvv.top

[S29] C：变参函数
来源：http://gmj.chenlongwang.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vka.tanke756.top

[S30] C：头文件保护
来源：http://tuu.xuetiantiany.cn

#ifndef X_H
来源：http://kwx.wangshuangyany.cn

#define X_H
来源：http://hlw.tian-w.cn

#endif
来源：http://kkw.shanyushiyangkeji.top

[S31] C++：Hello World
来源：http://biu.yangfankeji.com

#include <iostream>
来源：http://xwr.snrcjt.cn

int main() { std::cout << "Hello\n"; }
来源：http://dfi.vehdjk.com

[S32] C++：字符串
来源：http://zkm.ybcxt.top

std::string s = "hi";  s += "!";
来源：http://qus.shanyushiyangtech.top

[S33] C++：vector 增删
来源：http://vwp.daxiang520.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gvf.xingfuxueyuan.xyz

[S34] C++：遍历 vector
来源：http://owo.cdnleiting.top

for (auto &x : v) { std::cout << x; }
来源：http://tkk.dashuyun.cn

[S35] C++：map
来源：http://fch.tianlin.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://won.xingfuxueyuan.xyz

[S36] C++：unordered_map
来源：http://ukq.kuanghao11.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ipd.xziqi.cn

[S37] C++：set
来源：http://upb.ybcxt.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://art.zhixingplan.top

[S38] C++：排序
来源：http://qwq.iojbl.cn

std::sort(v.begin(), v.end());
来源：http://dgr.ydzc1.top

[S39] C++：自定义比较器排序
来源：http://try.shanyushiyangkeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gcx.aizwys.cn

[S40] C++：查找元素
来源：http://lmc.guowangkeji.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sdw.shangyingyoupin.top

[S41] C++：类与构造函数
来源：http://xvu.shzxlz.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ddi.yongpay.top

[S42] C++：继承与虚函数
来源：http://azm.xziqi.cn

class B : public Base { public: void f() override {} };
来源：http://lqz.vehdjk.com

[S43] C++：智能指针
来源：http://pie.pycfn.com

auto p = std::make_unique<int>(5);
来源：http://dmy.quarkkingdee.top

[S44] C++：引用传参
来源：http://bsv.wangdashe.top

void inc(int &x) { ++x; }
来源：http://xpk.zycfv.cn

[S45] C++：lambda
来源：http://xyg.sxryk.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qsx.ydjk.org.cn

[S46] C++：函数模板
来源：http://ise.aibaodan.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vee.c1oappe.top

[S47] C++：结构化绑定遍历
来源：http://tic.yj20258888.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dmd.pengpengdd.cyou

[S48] C++：逐行读文件
来源：http://gfn.zhiwuduotai.top

std::ifstream in("a.txt");  std::string line;
来源：http://cua.ydzc1.top

while (std::getline(in, line)) { }
来源：http://jlf.shangyingyoupin.top

[S49] C++：写文件
来源：http://akg.hysaishi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://drt.ehwqpu.com

[S50] C++：格式化数字
来源：http://nst.xingfuxueyuan.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ugd.hammf.cn

[S51] C++：显式类型转换
来源：http://ytt.zhoulong.xyz

static_cast<double>(a) / b
来源：http://svf.fzhhl.top

[S52] C++：const 与 noexcept
来源：http://vhi.zhongyouzk.top

int size() const noexcept { return n_; }
来源：http://qmx.guannengcc.top

[S53] C++：移动语义
来源：http://kvo.yj20258.top

std::vector<int> w = std::move(v);
来源：http://ece.bbcook.cn

[S54] C++：异常处理
来源：http://mwh.tian-w.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wyq.jqgfzy.top

[S55] C++：结构化绑定
来源：http://aqk.yonumen.top

auto [a, b] = std::make_pair(1, 2);
来源：http://kmx.dashuyun.cn

[S56] C++：optional
来源：http://mhp.xuanzx.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vox.hongshengwenyu.top

[S57] C++：编译期常量
来源：http://jgh.vqdsnc.cn

constexpr int N = 10;
来源：http://bgk.sufxvd.cn

[S58] C++：命名空间
来源：http://rip.chenzaomai.com

namespace ns { int f() { return 1; } }
来源：http://liv.wangdashe.top

[S59] C++：静态断言
来源：http://fbx.havefunace.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bvm.zhijiandao.cn

[S60] C++：遍历并删除元素
来源：http://ntx.zhengqikj.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://odl.shanyushiyangkeji.top

================================================================================
来源：http://mcy.uphjek.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bli.pengpengdd.cyou

================================================================================
来源：http://iuv.hywenlv.cn

[T01] Kotlin：Hello World
来源：http://siw.ehwqpu.com

println("Hello")
来源：http://fpi.zhoulong.xyz

[T02] Kotlin：变量
来源：http://vuq.pycfn.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qth.pycfn.com

[T03] Kotlin：字符串模板
来源：http://cxh.xinyue.icu

"值: $b"
来源：http://htd.ivvv.top

[T04] Kotlin：空安全
来源：http://pdr.daxiang520.top

val n: String? = null;  n?.length
来源：http://hcg.hywenlv.cn

[T05] Kotlin：when 表达式
来源：http://den.aibaodan.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kam.hnxiangtu.top

[T06] Kotlin：集合映射
来源：http://cml.yj20258888.top

listOf(1, 2, 3).map { it * 2 }
来源：http://qpe.chenjidiqi.icu

[T07] Kotlin：集合过滤
来源：http://dgy.shzxlz.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://shc.sjlbkw.cn

[T08] Kotlin：数据类
来源：http://hvq.cheryme.top

data class User(val name: String, val age: Int)
来源：http://uao.zhijiandao.cn

[T09] Kotlin：扩展函数
来源：http://cor.jiagoushi.top

fun String.exclaim() = this + "!"
来源：http://rqc.yanxiufei.cn

[T10] Kotlin：默认参数
来源：http://kub.quarkkingdee.top

fun greet(name: String = "World") = "Hi $name"
来源：http://svk.hnqzz.top

[T11] Kotlin：协程
来源：http://rfd.jqgufenzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ash.jinyuanbaomall.cn

[T12] Kotlin：解构声明
来源：http://mif.quarkkingdee.top

val (a, b) = Pair(1, 2)
来源：http://ofk.epnwcf.com

[T13] Kotlin：只读 Map
来源：http://sup.fengsongda.top

val m = mapOf("a" to 1)
来源：http://lkn.tarul.cn

[T14] Kotlin：循环
来源：http://rah.zhiwuduotai.top

for (i in 1..10) println(i)
来源：http://but.dianchejie.cn

[T15] Kotlin：接口
来源：http://pgc.iojbl.cn

interface Shape { fun area(): Double }
来源：http://zta.snrcjt.cn

[T16] Swift：Hello World
来源：http://uwt.zhengqikj.top

print("Hello")
来源：http://izs.kuanghao11.cn

[T17] Swift：变量与常量
来源：http://syj.nanxuanxn.top

var a = 1;  let b = 2
来源：http://xst.tanke756.top

[T18] Swift：字符串插值
来源：http://bmu.hongshengwenyu.top

"值: \(b)"
来源：http://rka.zhaomingkeji.xyz

[T19] Swift：可选绑定
来源：http://yms.gzhubu.top

if let n = opt { print(n) }
来源：http://cpg.sysykeji.top

[T20] Swift：数组操作
来源：http://ohu.zhoulong.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://odt.andypj.xyz

[T21] Swift：遍历
来源：http://zra.wangdashe.top

for x in a { print(x) }
来源：http://roj.jyoumei.cn

[T22] Swift：字典
来源：http://obg.fktsv.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vlq.shzxlz.cn

[T23] Swift：函数
来源：http://svt.mhx1999.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jlm.smart0.xyz

[T24] Swift：闭包
来源：http://ngg.haohaochexian.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ukl.yj202588.top

[T25] Swift：结构体
来源：http://jse.mhx1999.top

struct P { var x: Int }
来源：http://erh.havefunace.top

[T26] Swift：类与重写
来源：http://roq.fktsv.cn

class A: Base { override func f() {} }
来源：http://err.epnwcf.com

[T27] Swift：错误处理
来源：http://cpg.ehwqpu.com

do { try f() } catch { print(error) }
来源：http://kyk.fktsv.cn

[T28] Swift：枚举
来源：http://avw.mhx1999.top

enum Color { case red, green }
来源：http://cxz.vqdsnc.cn

[T29] Swift：guard 提前返回
来源：http://agi.chenlongwang.top

guard let x = opt else { return }
来源：http://awm.xingfuxueyuan.xyz

[T30] Swift：协议
来源：http://nhn.zycfv.cn

protocol Shape { func area() -> Double }
来源：http://pog.fengsongda.top

[T31] Lua：Hello World
来源：http://mee.hfpthk.cn

print("Hello")
来源：http://lnm.svipenyu.cn

[T32] Lua：局部变量
来源：http://rkv.shanyushiyangkeji.top

local a = 1
来源：http://xtr.cashguo.top

[T33] Lua：表（数组）
来源：http://fdf.hnxiangtu.top

local t = {1, 2, 3};  t[4] = 4
来源：http://vdm.shuidangran.top

[T34] Lua：遍历表
来源：http://zis.jqgfzy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://coj.daxiang520.top

[T35] Lua：字典表
来源：http://wgz.jqgfzy.top

local d = { a = 1 };  d.b = 2
来源：http://unh.hysaishi.cn

[T36] Lua：函数
来源：http://gip.feifeiyinyue.top

function add(a, b) return a + b end
来源：http://nzt.316326.xyz

[T37] Lua：字符串拼接
来源：http://uyi.guannengcc.top

"a" .. "b"
来源：http://udx.guannengcc.top

[T38] Lua：条件
来源：http://qml.yj202588.top

if x > 0 then print("正") end
来源：http://ehp.316326.xyz

[T39] Lua：模式匹配
来源：http://ibd.quarkkingdee.top

string.find(s, "%d+")
来源：http://iyx.fzhhl.top

[T40] Lua：元表
来源：http://hrg.hysaishi.cn

setmetatable({}, { __index = base })
来源：http://shv.yvedp.cn

[T41] Perl：Hello World
来源：http://wli.wangdashe.top

print "Hello\n";
来源：http://nql.cheryme.top

[T42] Perl：变量类型
来源：http://gbu.zhijiandao.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dio.ydjk.org.cn

[T43] Perl：字符串插值
来源：http://rob.yangfankeji.com

"值: $a"
来源：http://xka.hesvh.cn

[T44] Perl：条件
来源：http://gaj.guannengcc.top

if ($a > 0) { print "正"; }
来源：http://xqd.zhengqikj.top

[T45] Perl：数组遍历
来源：http://dxe.316326.xyz

for my $x (@arr) { print $x; }
来源：http://xto.gotoacloud.top

[T46] Perl：哈希操作
来源：http://bqz.xziqi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://vru.316326.xyz

[T47] Perl：正则捕获
来源：http://mnd.ywan-chungtsiang.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://zdh.zhaomingkeji.xyz

[T48] Perl：正则替换
来源：http://twm.aibaodan.cn

$s =~ s/old/new/g;
来源：http://gqn.sysykeji.top

[T49] Perl：函数
来源：http://miy.yfazqb.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bxa.cqqwz.cn

[T50] Perl：逐行读文件
来源：http://rde.ybcxt.top

open my $fh, "<", "a.txt" or die $!;
来源：http://yws.xinyue.icu

while (my $line = <$fh>) { print $line; }
来源：http://fgs.tian-w.cn

[T51] Scala：Hello World
来源：http://zch.dashuyun.cn

println("Hello")
来源：http://gls.havefunace.top

[T52] Scala：变量
来源：http://qin.fehbvm.com

val a = 1;  var b = 2
来源：http://olt.quarkkingdee.top

[T53] Scala：字符串插值
来源：http://uni.xuanzx.com

s"值: $b"
来源：http://dkv.zycfv.cn

[T54] Scala：集合映射
来源：http://oxf.yvedp.cn

List(1, 2, 3).map(_ * 2)
来源：http://wms.kuanghao11.cn

[T55] Scala：集合过滤
来源：http://pbm.ctjpmb.com

List(1, 2, 3).filter(_ > 1)
来源：http://ghk.zhaomingkeji.xyz

[T56] Scala：样例类
来源：http://isv.jqgfzy.top

case class User(name: String, age: Int)
来源：http://zaz.quarkkingdee.top

[T57] Scala：模式匹配
来源：http://rhs.ppjwa.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://yru.aibaodan.cn

[T58] Scala：函数定义
来源：http://sum.iojbl.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wpe.yuxming.cn

[T59] Scala：循环
来源：http://tlj.redwolf501.top

for (i <- 1 to 10) println(i)
来源：http://mum.epnwcf.com

[T60] Scala：折叠
来源：http://hnj.nwbrower.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://phv.c1oappe.top

================================================================================
来源：http://rgl.yuanzhike.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wui.hongshengwenyu.top

================================================================================
来源：http://mlx.hongshengwenyu.top


<!-- 参考信息 -->