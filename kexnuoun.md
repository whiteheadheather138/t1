代发 wailian999

free -h;  ps aux | grep nginx
来源：http://oux.jianghu66.top

[R64] 结束进程
来源：http://azv.nwbrower.top

kill -9 $(pgrep -f app.py)
来源：http://vvv.fktsv.cn

[R65] 查看端口占用
来源：http://zyx.yuxming.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cjr.cashguo.top

[R66] 定时任务
来源：http://oed.ppjwa.cn

crontab -e;  crontab -l
来源：http://mzv.sufxvd.cn

[R67] 生成随机十六进制串
来源：http://elc.chenjidiqi.icu

openssl rand -hex 16
来源：http://pok.ywan-chungtsiang.top

[R68] 计算文件校验值
来源：http://rbn.uphjek.com

sha256sum a.txt;  md5sum a.txt
来源：http://xgv.sxryk.cn

[R69] 生成随机密码
来源：http://qbc.shanyushiyangtech.top

head -c 16 /dev/urandom | base64
来源：http://zil.vqdsnc.cn

[R70] 时间戳与互转
来源：http://obt.yj20258.top

date +%s;  date -d @1700000000
来源：http://mwy.wangshuangyany.cn

[R71] 日期格式化
来源：http://trm.ppjwa.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://akn.xylfe.cn

[R72] 等待端口就绪
来源：http://rub.xinyue.icu

until nc -z localhost 3306; do sleep 1; done
来源：http://jvy.jyoumei.cn

[R73] 分割大日志
来源：http://fav.yuxming.cn

split -l 1000 big.log part_
来源：http://toh.zhongyouzk.top

[R74] 批量重命名
来源：http://vhk.zdbjq.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://aav.nanxinkj.top

[R75] 导出环境变量
来源：http://dqo.shzxlz.cn

export PATH="$HOME/bin:$PATH"
来源：http://vcy.tianlin.xyz

[R76] 使用临时文件
来源：http://chq.52xcode.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xci.jianghu66.top

[R77] 读取用户输入
来源：http://zkk.ydjk.org.cn

read -rp "请输入: " ans
来源：http://qeb.zhongyouzk.top

[R78] 交互式菜单
来源：http://hdn.dashuyun.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nuk.sjlbkw.cn

[R79] 解析命令行选项
来源：http://gzx.quarkkingdee.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wpd.ydzc1.top

[R80] 查看脚本执行耗时
来源：http://aam.shangyingyoupin.top

time ./run.sh
来源：http://rux.xingfuxueyuan.xyz

================================================================================
来源：http://wel.xingfuxueyuan.xyz

S. C / C++ 专题
来源：http://jpm.xziqi.cn

================================================================================
来源：http://ymq.tian-w.cn

[S01] C：Hello World
来源：http://ypf.gogol.net.cn

#include <stdio.h>
来源：http://esk.fengsongda.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://dun.pengpengdd.cyou

[S02] C：变量与格式化输出
来源：http://bvr.shangyingyoupin.top

int a = 10; printf("%d\n", a);
来源：http://kgd.cdnleiting.top

[S03] C：读入整数
来源：http://scf.kuanghao11.cn

int x; scanf("%d", &x);
来源：http://fem.ctjpmb.com

[S04] C：字符串复制
来源：http://hmi.chenjidiqi.icu

char dst[32]; strcpy(dst, "hi");
来源：http://tor.zycfv.cn

[S05] C：字符串长度
来源：http://aiz.gotoacloud.top

strlen(s)
来源：http://byq.nanxuanxn.top

[S06] C：字符串比较
来源：http://ecr.kuanghao11.cn

strcmp(a, b) == 0
来源：http://hcg.chenlongwang.top

[S07] C：数组遍历求和
来源：http://axd.0kj1m.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bue.fengsongda.top

[S08] C：动态内存分配与释放
来源：http://hij.jiagoushi.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uup.meibo888.top

[S09] C：结构体定义与初始化
来源：http://orh.iojbl.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://agg.fengsongda.top

[S10] C：指针与解引用
来源：http://oty.jiagoushi.top

int *p = &a;  *p = 5;
来源：http://fxm.iojbl.cn

[S11] C：逐行读文件
来源：http://jtn.vqdsnc.cn

FILE *f = fopen("a.txt", "r");
来源：http://gaj.yuxming.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://eok.gotoacloud.top

fclose(f);
来源：http://ffm.mhx1999.top

[S12] C：写文件
来源：http://wed.epnwcf.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uce.jqgufenzy.top

[S13] C：宏定义
来源：http://wyc.yongpay.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gdk.yj20258.top

[S14] C：枚举
来源：http://awg.nanxinkj.top

enum Color { RED, GREEN, BLUE };
来源：http://fjc.yangfankeji.com

[S15] C：类型转换
来源：http://lgp.sxryk.cn

(double) a / b
来源：http://pfe.aizwys.cn

[S16] C：位操作置位
来源：http://pog.pengpengdd.cyou

x |= (1 << 3);
来源：http://txr.xinyue.icu

[S17] C：安全拼接字符串
来源：http://yuy.aibaodan.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pxj.iojbl.cn

[S18] C：命令行参数
来源：http://sea.havefunace.top

int main(int argc, char **argv)
来源：http://qfj.cashguo.top

[S19] C：快速排序
来源：http://jhi.jiagoushi.top

qsort(a, n, sizeof(int), cmp);
来源：http://tdw.yuxming.cn

[S20] C：二分查找
来源：http://knt.fengsongda.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://huh.52xcode.cn

[S21] C：字符类别判断
来源：http://hek.iojbl.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kiq.ywan-chungtsiang.top

[S22] C：字符串转数字
来源：http://mtk.jqgfzy.top

atoi("42");  strtod("3.14", NULL);
来源：http://jqh.yvedp.cn

[S23] C：随机数
来源：http://zqw.zhoulong.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://stc.dashuyun.cn

[S24] C：获取本地时间
来源：http://tsv.feifeiyinyue.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wjv.316326.xyz

[S25] C：内存拷贝
来源：http://hmx.sweek.top

memcpy(dst, src, n);
来源：http://jjq.epnwcf.com

[S26] C：内存清零
来源：http://kft.sufxvd.cn

memset(a, 0, sizeof a);
来源：http://als.zdqjudy.top

[S27] C：定义常量
来源：http://jpj.yuanzhike.top

const double PI = 3.14159;
来源：http://fij.epnwcf.com

[S28] C：静态变量
来源：http://pgg.ywan-chungtsiang.top

static int counter = 0;
来源：http://rsu.sweek.top

[S29] C：变参函数
来源：http://jlm.zhaomingkeji.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ygp.yonumen.top

[S30] C：头文件保护
来源：http://rbi.yj20258.top

#ifndef X_H
来源：http://yod.jyoumei.cn

#define X_H
来源：http://qdk.hywenlv.cn

#endif
来源：http://ofk.yj20258.top

[S31] C++：Hello World
来源：http://ofn.chenjidiqi.icu

#include <iostream>
来源：http://rpc.zhiwuduotai.top

int main() { std::cout << "Hello\n"; }
来源：http://pbl.aibaodan.cn

[S32] C++：字符串
来源：http://ijl.vqdsnc.cn

std::string s = "hi";  s += "!";
来源：http://slo.andypj.xyz

[S33] C++：vector 增删
来源：http://jln.guowangkeji.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lcg.gotoacloud.top

[S34] C++：遍历 vector
来源：http://twm.gaohongyu789.top

for (auto &x : v) { std::cout << x; }
来源：http://ukz.hywenlv.cn

[S35] C++：map
来源：http://sgb.shanyushiyangtech.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dbs.svipenyu.cn

[S36] C++：unordered_map
来源：http://vmr.jlsjyb.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fjf.shangyingyoupin.top

[S37] C++：set
来源：http://sjm.zycfv.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yul.yuxming.cn

[S38] C++：排序
来源：http://fcx.hcnkem.com

std::sort(v.begin(), v.end());
来源：http://fic.uphjek.com

[S39] C++：自定义比较器排序
来源：http://uuk.fanxiaobao.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://udl.quarkkingdee.top

[S40] C++：查找元素
来源：http://nxw.jlsjyb.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://urg.epnwcf.com

[S41] C++：类与构造函数
来源：http://koe.hongshengwenyu.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zmb.jianghu66.top

[S42] C++：继承与虚函数
来源：http://vml.hysaishi.cn

class B : public Base { public: void f() override {} };
来源：http://ayv.shzxlz.cn

[S43] C++：智能指针
来源：http://vtz.zdbjq.cn

auto p = std::make_unique<int>(5);
来源：http://tbu.0kj1m.cn

[S44] C++：引用传参
来源：http://rqk.guowangkeji.top

void inc(int &x) { ++x; }
来源：http://mnh.jianghu66.top

[S45] C++：lambda
来源：http://era.fzhhl.top

auto add = [](int a, int b) { return a + b; };
来源：http://jpt.pycfn.com

[S46] C++：函数模板
来源：http://hwk.sweek.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gtt.iojbl.cn

[S47] C++：结构化绑定遍历
来源：http://hdj.dianchejie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hwl.jqgfzy.top

[S48] C++：逐行读文件
来源：http://ksn.shanyushiyangkeji.top

std::ifstream in("a.txt");  std::string line;
来源：http://qus.jinqigfzy.top

while (std::getline(in, line)) { }
来源：http://uyy.smart0.xyz

[S49] C++：写文件
来源：http://nua.jinyuanbaomall.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fjk.redwolf501.top

[S50] C++：格式化数字
来源：http://gxb.vehdjk.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://usi.zhijiandao.cn

[S51] C++：显式类型转换
来源：http://fel.ydjk.org.cn

static_cast<double>(a) / b
来源：http://rxy.zhijiandao.cn

[S52] C++：const 与 noexcept
来源：http://tja.dashuyun.cn

int size() const noexcept { return n_; }
来源：http://iwp.sysykeji.top

[S53] C++：移动语义
来源：http://jmd.fehbvm.com

std::vector<int> w = std::move(v);
来源：http://dod.zhengqikj.top

[S54] C++：异常处理
来源：http://fem.gaohongyu789.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tru.shanyushiyangtech.top

[S55] C++：结构化绑定
来源：http://phc.feifeiyinyue.top

auto [a, b] = std::make_pair(1, 2);
来源：http://mmx.cheryme.top

[S56] C++：optional
来源：http://ovl.tianlin.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rsn.cashguo.top

[S57] C++：编译期常量
来源：http://kxx.daria6918.cn

constexpr int N = 10;
来源：http://nlg.hywenlv.cn

[S58] C++：命名空间
来源：http://evf.tianlin.xyz

namespace ns { int f() { return 1; } }
来源：http://kye.yuxming.cn

[S59] C++：静态断言
来源：http://smu.cdnleiting.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jbs.hesvh.cn

[S60] C++：遍历并删除元素
来源：http://dus.xuanzx.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ojf.zhongyouzk.top

================================================================================
来源：http://nab.sjlbkw.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://usc.ybcxt.top

================================================================================
来源：http://ars.pycfn.com

[T01] Kotlin：Hello World
来源：http://xke.ehwqpu.com

println("Hello")
来源：http://qtm.gzhubu.top

[T02] Kotlin：变量
来源：http://gpt.tanke756.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ffb.cucudq.cn

[T03] Kotlin：字符串模板
来源：http://bdk.cucudq.cn

"值: $b"
来源：http://scq.hfpthk.cn

[T04] Kotlin：空安全
来源：http://wyi.tianlin.xyz

val n: String? = null;  n?.length
来源：http://iko.hysaishi.cn

[T05] Kotlin：when 表达式
来源：http://ftp.ydjk.org.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wey.jinqigufen.top

[T06] Kotlin：集合映射
来源：http://hqo.gotoacloud.top

listOf(1, 2, 3).map { it * 2 }
来源：http://rjr.hysaishi.cn

[T07] Kotlin：集合过滤
来源：http://zvh.nanxinkj.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://kap.tanke756.top

[T08] Kotlin：数据类
来源：http://wih.yangfankeji.com

data class User(val name: String, val age: Int)
来源：http://khj.hnxiangtu.top

[T09] Kotlin：扩展函数
来源：http://xiw.shzxlz.cn

fun String.exclaim() = this + "!"
来源：http://scf.cashguo.top

[T10] Kotlin：默认参数
来源：http://mfk.kuanghao11.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://dln.gotoacloud.top

[T11] Kotlin：协程
来源：http://cao.zhongyouzk.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://xdc.mhx1999.top

[T12] Kotlin：解构声明
来源：http://gdg.pengpengdd.cyou

val (a, b) = Pair(1, 2)
来源：http://two.hysaishi.cn

[T13] Kotlin：只读 Map
来源：http://lqm.jianghu66.top

val m = mapOf("a" to 1)
来源：http://jsi.cucudq.cn

[T14] Kotlin：循环
来源：http://gpz.daria6918.cn

for (i in 1..10) println(i)
来源：http://ixy.yfazqb.com

[T15] Kotlin：接口
来源：http://tgz.xuetiantiany.cn

interface Shape { fun area(): Double }
来源：http://yhc.jinqigufen.top

[T16] Swift：Hello World
来源：http://jtb.yonumen.top

print("Hello")
来源：http://ulu.316326.xyz

[T17] Swift：变量与常量
来源：http://nqx.shangyingyoupin.top

var a = 1;  let b = 2
来源：http://plj.zycfv.cn

[T18] Swift：字符串插值
来源：http://mxb.xinyue.icu

"值: \(b)"
来源：http://wab.pengpengdd.cyou

[T19] Swift：可选绑定
来源：http://kft.nwbrower.top

if let n = opt { print(n) }
来源：http://cyn.52xcode.cn

[T20] Swift：数组操作
来源：http://zto.yfazqb.com

var a = [1, 2, 3];  a.append(4)
来源：http://kie.havefunace.top

[T21] Swift：遍历
来源：http://hzr.quarkkingdee.top

for x in a { print(x) }
来源：http://wpr.birdmap.top

[T22] Swift：字典
来源：http://pjh.smart0.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://myx.tarul.cn

[T23] Swift：函数
来源：http://ylh.9152youxi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vvu.jqgfzy.top

[T24] Swift：闭包
来源：http://rmh.smart0.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://vkg.cheryme.top

[T25] Swift：结构体
来源：http://rur.yueranfly.top

struct P { var x: Int }
来源：http://wmu.yueranfly.top

[T26] Swift：类与重写
来源：http://hqp.zhiwuduotai.top

class A: Base { override func f() {} }
来源：http://gvk.yongpay.top

[T27] Swift：错误处理
来源：http://grx.jlsjyb.cn

do { try f() } catch { print(error) }
来源：http://wju.dianchejie.cn

[T28] Swift：枚举
来源：http://dwl.hongshengwenyu.top

enum Color { case red, green }
来源：http://djv.quarkkingdee.top

[T29] Swift：guard 提前返回
来源：http://bxo.shanyushiyangtech.top

guard let x = opt else { return }
来源：http://oev.pycfn.com

[T30] Swift：协议
来源：http://zig.hnxiangtu.top

protocol Shape { func area() -> Double }
来源：http://vhj.yfazqb.com

[T31] Lua：Hello World
来源：http://gyg.gzhubu.top

print("Hello")
来源：http://ctx.uphjek.com

[T32] Lua：局部变量
来源：http://omr.hfpthk.cn

local a = 1
来源：http://lor.yuanzhike.top

[T33] Lua：表（数组）
来源：http://cnm.cqqwz.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wcb.gogol.net.cn

[T34] Lua：遍历表
来源：http://xeg.xziqi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://wwg.ywan-chungtsiang.top

[T35] Lua：字典表
来源：http://ock.feifeiyinyue.top

local d = { a = 1 };  d.b = 2
来源：http://ysp.uphjek.com

[T36] Lua：函数
来源：http://jaq.gogol.net.cn

function add(a, b) return a + b end
来源：http://jsq.gogol.net.cn

[T37] Lua：字符串拼接
来源：http://cum.aibaodan.cn

"a" .. "b"
来源：http://amm.xuanzx.com

[T38] Lua：条件
来源：http://wvl.wangdashe.top

if x > 0 then print("正") end
来源：http://thb.daria6918.cn

[T39] Lua：模式匹配
来源：http://wjj.jinqigufen.top

string.find(s, "%d+")
来源：http://msp.ydzc1.top

[T40] Lua：元表
来源：http://jav.yuxming.cn

setmetatable({}, { __index = base })
来源：http://dms.zycfv.cn

[T41] Perl：Hello World
来源：http://nui.zhixingplan.top

print "Hello\n";
来源：http://sgv.quarkkingdee.top

[T42] Perl：变量类型
来源：http://vvl.epnwcf.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sas.wangdashe.top

[T43] Perl：字符串插值
来源：http://wty.bjfxy.top

"值: $a"
来源：http://kmk.jinqigufen.top

[T44] Perl：条件
来源：http://ytr.jlsjyb.cn

if ($a > 0) { print "正"; }
来源：http://tjr.cucudq.cn

[T45] Perl：数组遍历
来源：http://xpx.aibaodan.cn

for my $x (@arr) { print $x; }
来源：http://gto.yvedp.cn

[T46] Perl：哈希操作
来源：http://riy.jyoumei.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://abd.hongshengwenyu.top

[T47] Perl：正则捕获
来源：http://vkv.fehbvm.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://sro.ppjwa.cn

[T48] Perl：正则替换
来源：http://wwe.jinyuanbaomall.cn

$s =~ s/old/new/g;
来源：http://iqy.sysykeji.top

[T49] Perl：函数
来源：http://zwo.vqdsnc.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vfl.hnxiangtu.top

[T50] Perl：逐行读文件
来源：http://nhx.ppjwa.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://mpv.zdbjq.cn

while (my $line = <$fh>) { print $line; }
来源：http://vui.hysaishi.cn

[T51] Scala：Hello World
来源：http://wtg.havefunace.top

println("Hello")
来源：http://okq.tian-w.cn

[T52] Scala：变量
来源：http://mzx.gotoacloud.top

val a = 1;  var b = 2
来源：http://wbp.pengpengdd.cyou

[T53] Scala：字符串插值
来源：http://slw.sxryk.cn

s"值: $b"
来源：http://utt.daxiang520.top

[T54] Scala：集合映射
来源：http://dhu.hywenlv.cn

List(1, 2, 3).map(_ * 2)
来源：http://yux.yuxming.cn

[T55] Scala：集合过滤
来源：http://brp.cdnleiting.top

List(1, 2, 3).filter(_ > 1)
来源：http://tqu.zhoulong.xyz

[T56] Scala：样例类
来源：http://juo.smart0.xyz

case class User(name: String, age: Int)
来源：http://vxx.0kj1m.cn

[T57] Scala：模式匹配
来源：http://ezp.shzxlz.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://eao.hnxiangtu.top

[T58] Scala：函数定义
来源：http://fjg.smart0.xyz

def add(a: Int, b: Int): Int = a + b
来源：http://brt.cheryme.top

[T59] Scala：循环
来源：http://xvh.nanxinkj.top

for (i <- 1 to 10) println(i)
来源：http://ltl.aizwys.cn

[T60] Scala：折叠
来源：http://jsj.xinyue.icu

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ptz.daxiang520.top

================================================================================
来源：http://esk.xingfuxueyuan.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xir.pengpengdd.cyou

================================================================================
来源：http://cdr.sjlbkw.cn

[U01] Py：创建虚拟环境
来源：http://pnx.jinqigfzy.top

python -m venv .venv && source .venv/bin/activate
来源：http://sof.xuanzx.com

[U02] Py：导出 / 安装依赖
来源：http://gma.hysaishi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://akk.jinqigfzy.top

[U03] Py：加载 .env 配置
来源：http://oky.yonumen.top

from dotenv import load_dotenv; load_dotenv()
来源：http://yqa.hammf.cn

[U04] Py：变量调试打印
来源：http://oyd.jyoumei.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://sya.quarkkingdee.top


<!-- 参考信息 -->