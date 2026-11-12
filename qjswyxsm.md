代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://oqf.cdnleiting.top

[R66] 定时任务
来源：http://gcn.snrcjt.cn

crontab -e;  crontab -l
来源：http://lcv.fktsv.cn

[R67] 生成随机十六进制串
来源：http://vdx.dianchejie.cn

openssl rand -hex 16
来源：http://wcj.ppjwa.cn

[R68] 计算文件校验值
来源：http://zmb.tianlin.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://rea.fehbvm.com

[R69] 生成随机密码
来源：http://eqy.316326.xyz

head -c 16 /dev/urandom | base64
来源：http://xgb.tianlin.xyz

[R70] 时间戳与互转
来源：http://ygp.sufxvd.cn

date +%s;  date -d @1700000000
来源：http://fog.xinyue.icu

[R71] 日期格式化
来源：http://lms.jyoumei.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://njf.jqgfzy.top

[R72] 等待端口就绪
来源：http://hvi.cucudq.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://lff.iojbl.cn

[R73] 分割大日志
来源：http://xki.yvedp.cn

split -l 1000 big.log part_
来源：http://gas.zhixingplan.top

[R74] 批量重命名
来源：http://pnz.jiagoushi.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pgh.yj20258888.top

[R75] 导出环境变量
来源：http://yyx.snrcjt.cn

export PATH="$HOME/bin:$PATH"
来源：http://ojk.ydjk.org.cn

[R76] 使用临时文件
来源：http://tns.hongshengwenyu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kuy.fehbvm.com

[R77] 读取用户输入
来源：http://ujt.quarkkingdee.top

read -rp "请输入: " ans
来源：http://jjj.wangdashe.top

[R78] 交互式菜单
来源：http://fan.haohaochexian.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ror.cucudq.cn

[R79] 解析命令行选项
来源：http://tdv.shangyingyoupin.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ijm.0kj1m.cn

[R80] 查看脚本执行耗时
来源：http://hll.yuxming.cn

time ./run.sh
来源：http://big.jyoumei.cn

================================================================================
来源：http://smj.yvedp.cn

S. C / C++ 专题
来源：http://awt.tian-w.cn

================================================================================
来源：http://zcm.tian-w.cn

[S01] C：Hello World
来源：http://wjk.yfazqb.com

#include <stdio.h>
来源：http://hsr.cqqwz.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://wlc.chenzaomai.com

[S02] C：变量与格式化输出
来源：http://rnf.fzhhl.top

int a = 10; printf("%d\n", a);
来源：http://rhp.jqgfzy.top

[S03] C：读入整数
来源：http://zvy.hfpthk.cn

int x; scanf("%d", &x);
来源：http://mcy.zhoulong.xyz

[S04] C：字符串复制
来源：http://ozm.yj20258888.top

char dst[32]; strcpy(dst, "hi");
来源：http://jcm.fktsv.cn

[S05] C：字符串长度
来源：http://ohb.jlsjyb.cn

strlen(s)
来源：http://llc.sysykeji.top

[S06] C：字符串比较
来源：http://vve.jinyuanbaomall.cn

strcmp(a, b) == 0
来源：http://owq.tanke756.top

[S07] C：数组遍历求和
来源：http://fbe.hfpthk.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hpb.zhaomingkeji.xyz

[S08] C：动态内存分配与释放
来源：http://rgw.hnxiangtu.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qxa.jinghuilouyu.cn

[S09] C：结构体定义与初始化
来源：http://fev.yanxiufei.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://awk.birdmap.top

[S10] C：指针与解引用
来源：http://are.jinghuilouyu.cn

int *p = &a;  *p = 5;
来源：http://hmk.yfazqb.com

[S11] C：逐行读文件
来源：http://dog.pycfn.com

FILE *f = fopen("a.txt", "r");
来源：http://rtb.vqdsnc.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://sfe.hywenlv.cn

fclose(f);
来源：http://kmy.chenjidiqi.icu

[S12] C：写文件
来源：http://snr.fengsongda.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qca.ydzc1.top

[S13] C：宏定义
来源：http://kga.tianlin.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://btv.c1oappe.top

[S14] C：枚举
来源：http://dom.bjfxy.top

enum Color { RED, GREEN, BLUE };
来源：http://vgh.uphjek.com

[S15] C：类型转换
来源：http://bkv.jlsjyb.cn

(double) a / b
来源：http://gtx.ivvv.top

[S16] C：位操作置位
来源：http://uva.cashguo.top

x |= (1 << 3);
来源：http://yrm.yuxming.cn

[S17] C：安全拼接字符串
来源：http://mjt.sufxvd.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tft.zhoulong.xyz

[S18] C：命令行参数
来源：http://tja.jyoumei.cn

int main(int argc, char **argv)
来源：http://sgv.shzxlz.cn

[S19] C：快速排序
来源：http://omn.xingfuxueyuan.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://vxr.daxiang520.top

[S20] C：二分查找
来源：http://xcp.yuanzhike.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gcu.epnwcf.com

[S21] C：字符类别判断
来源：http://arh.9152youxi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://oeh.pengpengdd.cyou

[S22] C：字符串转数字
来源：http://hkt.cucudq.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tdz.fehbvm.com

[S23] C：随机数
来源：http://bnt.ydzc1.top

srand(time(NULL));  int r = rand() % 100;
来源：http://rok.daxiang520.top

[S24] C：获取本地时间
来源：http://byc.9152youxi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://adv.daria6918.cn

[S25] C：内存拷贝
来源：http://xhz.havefunace.top

memcpy(dst, src, n);
来源：http://qxa.yueranfly.top

[S26] C：内存清零
来源：http://fto.yongpay.top

memset(a, 0, sizeof a);
来源：http://hqz.shanyushiyangkeji.top

[S27] C：定义常量
来源：http://wmc.ywan-chungtsiang.top

const double PI = 3.14159;
来源：http://mkw.chenjidiqi.icu

[S28] C：静态变量
来源：http://zpz.yj20258888.top

static int counter = 0;
来源：http://luo.quarkkingdee.top

[S29] C：变参函数
来源：http://aux.pycfn.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rsq.shanyushiyangkeji.top

[S30] C：头文件保护
来源：http://bqr.fanxiaobao.xyz

#ifndef X_H
来源：http://cbu.vqdsnc.cn

#define X_H
来源：http://ctq.xinyue.icu

#endif
来源：http://dov.tianlin.xyz

[S31] C++：Hello World
来源：http://heu.yanxiufei.cn

#include <iostream>
来源：http://orw.yangfankeji.com

int main() { std::cout << "Hello\n"; }
来源：http://vii.hcnkem.com

[S32] C++：字符串
来源：http://jcf.tanke756.top

std::string s = "hi";  s += "!";
来源：http://jcl.shanyushiyangtech.top

[S33] C++：vector 增删
来源：http://xsf.yuanzhike.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tsz.cheryme.top

[S34] C++：遍历 vector
来源：http://rqt.zdbjq.cn

for (auto &x : v) { std::cout << x; }
来源：http://cca.zhongyouzk.top

[S35] C++：map
来源：http://xep.yanxiufei.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wgy.jlsjyb.cn

[S36] C++：unordered_map
来源：http://etp.hammf.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yni.ydzc1.top

[S37] C++：set
来源：http://pph.tian-w.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://euo.quarkkingdee.top

[S38] C++：排序
来源：http://lhm.nwbrower.top

std::sort(v.begin(), v.end());
来源：http://jxk.hcnkem.com

[S39] C++：自定义比较器排序
来源：http://mkm.dashuyun.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dew.fktsv.cn

[S40] C++：查找元素
来源：http://pgo.ppjwa.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bzt.jlsjyb.cn

[S41] C++：类与构造函数
来源：http://bxr.yj20258888.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://aot.vehdjk.com

[S42] C++：继承与虚函数
来源：http://bkz.xuetiantiany.cn

class B : public Base { public: void f() override {} };
来源：http://nka.0kj1m.cn

[S43] C++：智能指针
来源：http://qyc.sysykeji.top

auto p = std::make_unique<int>(5);
来源：http://xwa.uphjek.com

[S44] C++：引用传参
来源：http://men.jqgfzy.top

void inc(int &x) { ++x; }
来源：http://nqe.daxiang520.top

[S45] C++：lambda
来源：http://cwf.hammf.cn

auto add = [](int a, int b) { return a + b; };
来源：http://slp.zhijiandao.cn

[S46] C++：函数模板
来源：http://sdb.tarul.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://szt.ydjk.org.cn

[S47] C++：结构化绑定遍历
来源：http://bnh.quarkkingdee.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jhk.aibaodan.cn

[S48] C++：逐行读文件
来源：http://fxf.pycfn.com

std::ifstream in("a.txt");  std::string line;
来源：http://ooe.9152youxi.cn

while (std::getline(in, line)) { }
来源：http://wtq.fzhhl.top

[S49] C++：写文件
来源：http://zir.ybcxt.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dta.cucudq.cn

[S50] C++：格式化数字
来源：http://bve.zhengqikj.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zkq.yj202588.top

[S51] C++：显式类型转换
来源：http://rol.zhaomingkeji.xyz

static_cast<double>(a) / b
来源：http://xqx.cqqwz.cn

[S52] C++：const 与 noexcept
来源：http://ynm.jqgufenzy.top

int size() const noexcept { return n_; }
来源：http://dtg.daria6918.cn

[S53] C++：移动语义
来源：http://lnc.redwolf501.top

std::vector<int> w = std::move(v);
来源：http://iam.daxiang520.top

[S54] C++：异常处理
来源：http://zaa.ivvv.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mag.tianlin.xyz

[S55] C++：结构化绑定
来源：http://lcf.zhixingplan.top

auto [a, b] = std::make_pair(1, 2);
来源：http://crx.yj20258888.top

[S56] C++：optional
来源：http://cbj.havefunace.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cew.shanyushiyangtech.top

[S57] C++：编译期常量
来源：http://sui.c1oappe.top

constexpr int N = 10;
来源：http://saj.9152youxi.cn

[S58] C++：命名空间
来源：http://xfi.dashuyun.cn

namespace ns { int f() { return 1; } }
来源：http://yim.hcnkem.com

[S59] C++：静态断言
来源：http://nzh.wangshuangyany.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ily.andypj.xyz

[S60] C++：遍历并删除元素
来源：http://tdm.cashguo.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://teh.zdqjudy.top

================================================================================
来源：http://mth.cqqwz.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pyc.ctjpmb.com

================================================================================
来源：http://yaa.meibo888.top

[T01] Kotlin：Hello World
来源：http://mlt.hnqzz.top

println("Hello")
来源：http://hik.chenzaomai.com

[T02] Kotlin：变量
来源：http://bkg.9152youxi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xpb.chenlongwang.top

[T03] Kotlin：字符串模板
来源：http://upj.smart0.xyz

"值: $b"
来源：http://vcs.pycfn.com

[T04] Kotlin：空安全
来源：http://wqi.yj202588.top

val n: String? = null;  n?.length
来源：http://oey.yuanzhike.top

[T05] Kotlin：when 表达式
来源：http://dll.zhiwuduotai.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nvv.xinyue.icu

[T06] Kotlin：集合映射
来源：http://qip.aibaodan.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://jbe.gotoacloud.top

[T07] Kotlin：集合过滤
来源：http://juf.xuetiantiany.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://pma.jlsjyb.cn

[T08] Kotlin：数据类
来源：http://kbj.nanxinkj.top

data class User(val name: String, val age: Int)
来源：http://zxs.yuxming.cn

[T09] Kotlin：扩展函数
来源：http://jic.smart0.xyz

fun String.exclaim() = this + "!"
来源：http://ilz.feifeiyinyue.top

[T10] Kotlin：默认参数
来源：http://toe.zhongyouzk.top

fun greet(name: String = "World") = "Hi $name"
来源：http://etb.hysaishi.cn

[T11] Kotlin：协程
来源：http://jtd.hywenlv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ddj.jinghuilouyu.cn

[T12] Kotlin：解构声明
来源：http://mpf.ehwqpu.com

val (a, b) = Pair(1, 2)
来源：http://icv.yanxiufei.cn

[T13] Kotlin：只读 Map
来源：http://qmc.svipenyu.cn

val m = mapOf("a" to 1)
来源：http://zbr.yj20258888.top

[T14] Kotlin：循环
来源：http://oju.meibo888.top

for (i in 1..10) println(i)
来源：http://lko.zhongyouzk.top

[T15] Kotlin：接口
来源：http://ugp.vehdjk.com

interface Shape { fun area(): Double }
来源：http://axo.shzxlz.cn

[T16] Swift：Hello World
来源：http://xbt.fanxiaobao.xyz

print("Hello")
来源：http://ven.svipenyu.cn

[T17] Swift：变量与常量
来源：http://edj.iojbl.cn

var a = 1;  let b = 2
来源：http://fjr.ehwqpu.com

[T18] Swift：字符串插值
来源：http://lxd.nwbrower.top

"值: \(b)"
来源：http://faq.cashguo.top

[T19] Swift：可选绑定
来源：http://bwa.cucudq.cn

if let n = opt { print(n) }
来源：http://nph.cdnleiting.top

[T20] Swift：数组操作
来源：http://jef.nanxinkj.top

var a = [1, 2, 3];  a.append(4)
来源：http://see.fehbvm.com

[T21] Swift：遍历
来源：http://vzz.shuidangran.top

for x in a { print(x) }
来源：http://gpn.ydzc1.top

[T22] Swift：字典
来源：http://hjb.hysaishi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://dso.hywenlv.cn

[T23] Swift：函数
来源：http://puh.gaohongyu789.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zqt.redwolf501.top

[T24] Swift：闭包
来源：http://jmf.ybcxt.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://xoe.jlsjyb.cn

[T25] Swift：结构体
来源：http://apw.zhixingplan.top

struct P { var x: Int }
来源：http://gcu.jlsjyb.cn

[T26] Swift：类与重写
来源：http://bcd.jyoumei.cn

class A: Base { override func f() {} }
来源：http://zoy.nanxuanxn.top

[T27] Swift：错误处理
来源：http://ajn.jinqigfzy.top

do { try f() } catch { print(error) }
来源：http://soc.tian-w.cn

[T28] Swift：枚举
来源：http://ahi.snrcjt.cn

enum Color { case red, green }
来源：http://qma.feifeiyinyue.top

[T29] Swift：guard 提前返回
来源：http://ptr.sysykeji.top

guard let x = opt else { return }
来源：http://biq.nanxinkj.top

[T30] Swift：协议
来源：http://xuc.yvedp.cn

protocol Shape { func area() -> Double }
来源：http://mpf.birdmap.top

[T31] Lua：Hello World
来源：http://hjk.hongshengwenyu.top

print("Hello")
来源：http://ica.fehbvm.com

[T32] Lua：局部变量
来源：http://mwg.zhaomingkeji.xyz

local a = 1
来源：http://yll.jinyuanbaomall.cn

[T33] Lua：表（数组）
来源：http://dzx.cdnleiting.top

local t = {1, 2, 3};  t[4] = 4
来源：http://qai.zhaomingkeji.xyz

[T34] Lua：遍历表
来源：http://mpt.xingfuxueyuan.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://npc.kuanghao11.cn

[T35] Lua：字典表
来源：http://xew.nwbrower.top

local d = { a = 1 };  d.b = 2
来源：http://jio.nanxuanxn.top

[T36] Lua：函数
来源：http://whq.havefunace.top

function add(a, b) return a + b end
来源：http://zfm.gotoacloud.top

[T37] Lua：字符串拼接
来源：http://sst.cheryme.top

"a" .. "b"
来源：http://ugm.redwolf501.top

[T38] Lua：条件
来源：http://esg.cucudq.cn

if x > 0 then print("正") end
来源：http://jhg.guannengcc.top

[T39] Lua：模式匹配
来源：http://ppc.shanyushiyangkeji.top

string.find(s, "%d+")
来源：http://jjs.nanxinkj.top

[T40] Lua：元表
来源：http://gwe.gotoacloud.top

setmetatable({}, { __index = base })
来源：http://bkl.fengsongda.top

[T41] Perl：Hello World
来源：http://jsg.hnqzz.top

print "Hello\n";
来源：http://vhp.ctjpmb.com

[T42] Perl：变量类型
来源：http://lhf.xuetiantiany.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://txd.daria6918.cn

[T43] Perl：字符串插值
来源：http://uyw.zhixingplan.top

"值: $a"
来源：http://ryz.iojbl.cn

[T44] Perl：条件
来源：http://xly.quarkkingdee.top

if ($a > 0) { print "正"; }
来源：http://dup.ctjpmb.com

[T45] Perl：数组遍历
来源：http://gim.nanxinkj.top

for my $x (@arr) { print $x; }
来源：http://ssv.ybcxt.top

[T46] Perl：哈希操作
来源：http://zwn.zhongyouzk.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fjj.tarul.cn

[T47] Perl：正则捕获
来源：http://ptv.hfpthk.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://img.shangyingyoupin.top

[T48] Perl：正则替换
来源：http://kip.fanxiaobao.xyz

$s =~ s/old/new/g;
来源：http://hqt.xuanzx.com

[T49] Perl：函数
来源：http://xlj.yanxiufei.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ukl.jyoumei.cn

[T50] Perl：逐行读文件
来源：http://cbt.hysaishi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ayt.uphjek.com

while (my $line = <$fh>) { print $line; }
来源：http://epo.tianlin.xyz

[T51] Scala：Hello World
来源：http://qrv.shangyingyoupin.top

println("Hello")
来源：http://rpa.zhiwuduotai.top

[T52] Scala：变量
来源：http://xsh.haohaochexian.top

val a = 1;  var b = 2
来源：http://xcp.9152youxi.cn

[T53] Scala：字符串插值
来源：http://xfq.yfazqb.com

s"值: $b"
来源：http://qsj.yj20258888.top

[T54] Scala：集合映射
来源：http://nqh.316326.xyz

List(1, 2, 3).map(_ * 2)
来源：http://zou.yj202588.top

[T55] Scala：集合过滤
来源：http://xmq.shangyingyoupin.top

List(1, 2, 3).filter(_ > 1)
来源：http://jep.daxiang520.top

[T56] Scala：样例类
来源：http://ljh.cashguo.top

case class User(name: String, age: Int)
来源：http://fgr.daxiang520.top

[T57] Scala：模式匹配
来源：http://lqq.cheryme.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://zmv.jinqigufen.top

[T58] Scala：函数定义
来源：http://xxh.9152youxi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://hmk.yueranfly.top

[T59] Scala：循环
来源：http://azg.zhaomingkeji.xyz

for (i <- 1 to 10) println(i)
来源：http://uly.chenzaomai.com

[T60] Scala：折叠
来源：http://olm.shangyingyoupin.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://itx.andypj.xyz

================================================================================
来源：http://xwz.yj20258.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ijn.chenjidiqi.icu

================================================================================
来源：http://drm.pengpengdd.cyou

[U01] Py：创建虚拟环境
来源：http://ghu.yangfankeji.com

python -m venv .venv && source .venv/bin/activate
来源：http://iyd.yvedp.cn

[U02] Py：导出 / 安装依赖
来源：http://qdy.sufxvd.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gax.chenzaomai.com

[U03] Py：加载 .env 配置
来源：http://cxe.dashuyun.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://orn.yanxiufei.cn

[U04] Py：变量调试打印
来源：http://bmn.gotoacloud.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://quw.cqqwz.cn

[U05] Py：列表去重且保序
来源：http://jdc.tanke756.top

list(dict.fromkeys(arr))
来源：http://mpm.yvedp.cn

[U06] Py：合并两个字典
来源：http://ugk.yongpay.top

{**a, **b}
来源：http://jlj.vqdsnc.cn


<!-- 参考信息 -->