代发 wailian999

df -h;  du -sh *
来源：http://gam.ivvv.top

[R62] 找最占空间的文件
来源：http://wuj.smart0.xyz

du -ah . | sort -rh | head -10
来源：http://gjk.yj202588.top

[R63] 内存与进程
来源：http://hqk.guannengcc.top

free -h;  ps aux | grep nginx
来源：http://bsr.redwolf501.top

[R64] 结束进程
来源：http://xgm.shangyingyoupin.top

kill -9 $(pgrep -f app.py)
来源：http://vhg.sysykeji.top

[R65] 查看端口占用
来源：http://rcj.yj20258.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tlg.yuxming.cn

[R66] 定时任务
来源：http://lbb.nanxinkj.top

crontab -e;  crontab -l
来源：http://wqz.daxiang520.top

[R67] 生成随机十六进制串
来源：http://enj.hysaishi.cn

openssl rand -hex 16
来源：http://ycx.daxiang520.top

[R68] 计算文件校验值
来源：http://cbi.shangyingyoupin.top

sha256sum a.txt;  md5sum a.txt
来源：http://etq.jiagoushi.top

[R69] 生成随机密码
来源：http://qbs.zdqjudy.top

head -c 16 /dev/urandom | base64
来源：http://jup.jianghu66.top

[R70] 时间戳与互转
来源：http://ynw.hesvh.cn

date +%s;  date -d @1700000000
来源：http://epe.zycfv.cn

[R71] 日期格式化
来源：http://vba.meibo888.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://boo.jiagoushi.top

[R72] 等待端口就绪
来源：http://kwn.sufxvd.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jqu.jinqigufen.top

[R73] 分割大日志
来源：http://ikk.wangshuangyany.cn

split -l 1000 big.log part_
来源：http://cnw.zhixingplan.top

[R74] 批量重命名
来源：http://tbo.meibo888.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jej.dianchejie.cn

[R75] 导出环境变量
来源：http://hbq.nwbrower.top

export PATH="$HOME/bin:$PATH"
来源：http://bau.feifeiyinyue.top

[R76] 使用临时文件
来源：http://she.sufxvd.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lwq.cucudq.cn

[R77] 读取用户输入
来源：http://fxu.epnwcf.com

read -rp "请输入: " ans
来源：http://egz.havefunace.top

[R78] 交互式菜单
来源：http://dmy.xylfe.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://fek.pengpengdd.cyou

[R79] 解析命令行选项
来源：http://dbi.ivvv.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sly.xuanzx.com

[R80] 查看脚本执行耗时
来源：http://prd.9152youxi.cn

time ./run.sh
来源：http://ata.gzhubu.top

================================================================================
来源：http://acd.vehdjk.com

S. C / C++ 专题
来源：http://mhe.shanyushiyangkeji.top

================================================================================
来源：http://urx.52xcode.cn

[S01] C：Hello World
来源：http://ixj.wangshuangyany.cn

#include <stdio.h>
来源：http://ufn.nwbrower.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://epi.tarul.cn

[S02] C：变量与格式化输出
来源：http://qyd.smart0.xyz

int a = 10; printf("%d\n", a);
来源：http://mfw.sufxvd.cn

[S03] C：读入整数
来源：http://uaz.52xcode.cn

int x; scanf("%d", &x);
来源：http://spe.tian-w.cn

[S04] C：字符串复制
来源：http://esl.sjlbkw.cn

char dst[32]; strcpy(dst, "hi");
来源：http://amd.birdmap.top

[S05] C：字符串长度
来源：http://wuu.yuanzhike.top

strlen(s)
来源：http://tea.mhx1999.top

[S06] C：字符串比较
来源：http://haq.aizwys.cn

strcmp(a, b) == 0
来源：http://imf.jinqigfzy.top

[S07] C：数组遍历求和
来源：http://wgu.ivvv.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tsa.yj202588.top

[S08] C：动态内存分配与释放
来源：http://wtg.pengpengdd.cyou

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pkw.nwbrower.top

[S09] C：结构体定义与初始化
来源：http://tmu.vqdsnc.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hmo.jinyuanbaomall.cn

[S10] C：指针与解引用
来源：http://bdm.ppjwa.cn

int *p = &a;  *p = 5;
来源：http://paz.tian-w.cn

[S11] C：逐行读文件
来源：http://dkd.shuidangran.top

FILE *f = fopen("a.txt", "r");
来源：http://vxp.shanyushiyangtech.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://kdo.jianghu66.top

fclose(f);
来源：http://emg.andypj.xyz

[S12] C：写文件
来源：http://sfh.zhoulong.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sol.jinqigufen.top

[S13] C：宏定义
来源：http://uls.mhx1999.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tje.gzhubu.top

[S14] C：枚举
来源：http://iin.yuxming.cn

enum Color { RED, GREEN, BLUE };
来源：http://foo.ppjwa.cn

[S15] C：类型转换
来源：http://xhu.cucudq.cn

(double) a / b
来源：http://cen.jlsjyb.cn

[S16] C：位操作置位
来源：http://tzo.nwbrower.top

x |= (1 << 3);
来源：http://pmf.jinqigfzy.top

[S17] C：安全拼接字符串
来源：http://sry.yj20258.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xjb.vehdjk.com

[S18] C：命令行参数
来源：http://usj.yvedp.cn

int main(int argc, char **argv)
来源：http://uqa.xinyue.icu

[S19] C：快速排序
来源：http://qyo.vehdjk.com

qsort(a, n, sizeof(int), cmp);
来源：http://aaq.hfpthk.cn

[S20] C：二分查找
来源：http://jkt.chenlongwang.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ifd.shangyingyoupin.top

[S21] C：字符类别判断
来源：http://buv.andypj.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cii.shzxlz.cn

[S22] C：字符串转数字
来源：http://ksq.yfazqb.com

atoi("42");  strtod("3.14", NULL);
来源：http://crb.shanyushiyangtech.top

[S23] C：随机数
来源：http://idy.jqgufenzy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ydi.0kj1m.cn

[S24] C：获取本地时间
来源：http://rqi.zhijiandao.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://aox.ivvv.top

[S25] C：内存拷贝
来源：http://cca.zhoulong.xyz

memcpy(dst, src, n);
来源：http://lop.gogol.net.cn

[S26] C：内存清零
来源：http://wet.aizwys.cn

memset(a, 0, sizeof a);
来源：http://nhs.chenlongwang.top

[S27] C：定义常量
来源：http://kgo.hfpthk.cn

const double PI = 3.14159;
来源：http://bjy.zhiwuduotai.top

[S28] C：静态变量
来源：http://pkv.zhixingplan.top

static int counter = 0;
来源：http://nby.nwbrower.top

[S29] C：变参函数
来源：http://oyo.hcnkem.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yry.pycfn.com

[S30] C：头文件保护
来源：http://det.yanxiufei.cn

#ifndef X_H
来源：http://vzt.hysaishi.cn

#define X_H
来源：http://zow.zycfv.cn

#endif
来源：http://osl.haohaochexian.top

[S31] C++：Hello World
来源：http://edb.sxryk.cn

#include <iostream>
来源：http://zwt.bjfxy.top

int main() { std::cout << "Hello\n"; }
来源：http://uml.zycfv.cn

[S32] C++：字符串
来源：http://vyz.bbcook.cn

std::string s = "hi";  s += "!";
来源：http://ehl.fehbvm.com

[S33] C++：vector 增删
来源：http://eyn.ppjwa.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gko.pengpengdd.cyou

[S34] C++：遍历 vector
来源：http://roz.havefunace.top

for (auto &x : v) { std::cout << x; }
来源：http://haj.ybcxt.top

[S35] C++：map
来源：http://ofz.chenzaomai.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://aqv.9152youxi.cn

[S36] C++：unordered_map
来源：http://smz.xinyue.icu

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jfy.zdbjq.cn

[S37] C++：set
来源：http://huy.chenzaomai.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tqx.ppjwa.cn

[S38] C++：排序
来源：http://ntx.shangyingyoupin.top

std::sort(v.begin(), v.end());
来源：http://nsd.hcnkem.com

[S39] C++：自定义比较器排序
来源：http://ltr.chenjidiqi.icu

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ext.hesvh.cn

[S40] C++：查找元素
来源：http://han.hnqzz.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zqn.0kj1m.cn

[S41] C++：类与构造函数
来源：http://eaw.bbcook.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jmr.hfpthk.cn

[S42] C++：继承与虚函数
来源：http://bpe.mhx1999.top

class B : public Base { public: void f() override {} };
来源：http://pxp.daxiang520.top

[S43] C++：智能指针
来源：http://ndk.zdbjq.cn

auto p = std::make_unique<int>(5);
来源：http://bhc.yj20258.top

[S44] C++：引用传参
来源：http://uuy.hywenlv.cn

void inc(int &x) { ++x; }
来源：http://txv.cucudq.cn

[S45] C++：lambda
来源：http://gdc.hywenlv.cn

auto add = [](int a, int b) { return a + b; };
来源：http://nti.ctjpmb.com

[S46] C++：函数模板
来源：http://ffj.yj202588.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fbz.wangdashe.top

[S47] C++：结构化绑定遍历
来源：http://wsn.zhongyouzk.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://spl.quarkkingdee.top

[S48] C++：逐行读文件
来源：http://pdb.9152youxi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://woi.chenlongwang.top

while (std::getline(in, line)) { }
来源：http://gwx.chenjidiqi.icu

[S49] C++：写文件
来源：http://njs.cheryme.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xxb.dashuyun.cn

[S50] C++：格式化数字
来源：http://vyp.zdqjudy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rpm.daria6918.cn

[S51] C++：显式类型转换
来源：http://gnk.jinghuilouyu.cn

static_cast<double>(a) / b
来源：http://hlv.shzxlz.cn

[S52] C++：const 与 noexcept
来源：http://hme.aibaodan.cn

int size() const noexcept { return n_; }
来源：http://anh.shuidangran.top

[S53] C++：移动语义
来源：http://xkd.chenlongwang.top

std::vector<int> w = std::move(v);
来源：http://bqo.zhiwuduotai.top

[S54] C++：异常处理
来源：http://brt.jinghuilouyu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ivb.zhoulong.xyz

[S55] C++：结构化绑定
来源：http://zjj.yueranfly.top

auto [a, b] = std::make_pair(1, 2);
来源：http://hdq.zhaomingkeji.xyz

[S56] C++：optional
来源：http://zsy.zhaomingkeji.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cah.hfpthk.cn

[S57] C++：编译期常量
来源：http://vvl.yj20258.top

constexpr int N = 10;
来源：http://uit.hesvh.cn

[S58] C++：命名空间
来源：http://zjf.aizwys.cn

namespace ns { int f() { return 1; } }
来源：http://bzd.nanxinkj.top

[S59] C++：静态断言
来源：http://zct.bjfxy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qca.cashguo.top

[S60] C++：遍历并删除元素
来源：http://wbu.jyoumei.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ddi.yj20258.top

================================================================================
来源：http://byn.yanxiufei.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xaz.andypj.xyz

================================================================================
来源：http://dbj.feifeiyinyue.top

[T01] Kotlin：Hello World
来源：http://bqk.fanxiaobao.xyz

println("Hello")
来源：http://ebc.shangyingyoupin.top

[T02] Kotlin：变量
来源：http://vsz.hammf.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rxd.dianchejie.cn

[T03] Kotlin：字符串模板
来源：http://meb.xinyue.icu

"值: $b"
来源：http://yxf.shuidangran.top

[T04] Kotlin：空安全
来源：http://ngv.dianchejie.cn

val n: String? = null;  n?.length
来源：http://jip.kuanghao11.cn

[T05] Kotlin：when 表达式
来源：http://heh.vqdsnc.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zvn.fengsongda.top

[T06] Kotlin：集合映射
来源：http://dul.aizwys.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://evt.0kj1m.cn

[T07] Kotlin：集合过滤
来源：http://sws.ivvv.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://oow.hongshengwenyu.top

[T08] Kotlin：数据类
来源：http://upm.yanxiufei.cn

data class User(val name: String, val age: Int)
来源：http://zho.jinghuilouyu.cn

[T09] Kotlin：扩展函数
来源：http://pos.xinyue.icu

fun String.exclaim() = this + "!"
来源：http://kma.316326.xyz

[T10] Kotlin：默认参数
来源：http://ueb.meibo888.top

fun greet(name: String = "World") = "Hi $name"
来源：http://gmf.c1oappe.top

[T11] Kotlin：协程
来源：http://iuh.xinyue.icu

GlobalScope.launch { delay(1000); println("done") }
来源：http://pso.shanyushiyangkeji.top

[T12] Kotlin：解构声明
来源：http://fwy.yfazqb.com

val (a, b) = Pair(1, 2)
来源：http://lxc.jlsjyb.cn

[T13] Kotlin：只读 Map
来源：http://bzx.quarkkingdee.top

val m = mapOf("a" to 1)
来源：http://ayl.snrcjt.cn

[T14] Kotlin：循环
来源：http://gqr.zhengqikj.top

for (i in 1..10) println(i)
来源：http://dti.jyoumei.cn

[T15] Kotlin：接口
来源：http://juq.iojbl.cn

interface Shape { fun area(): Double }
来源：http://zaj.haohaochexian.top

[T16] Swift：Hello World
来源：http://hgp.ydzc1.top

print("Hello")
来源：http://sym.zycfv.cn

[T17] Swift：变量与常量
来源：http://fun.redwolf501.top

var a = 1;  let b = 2
来源：http://hej.jiagoushi.top

[T18] Swift：字符串插值
来源：http://sbs.yangfankeji.com

"值: \(b)"
来源：http://ubm.chenlongwang.top

[T19] Swift：可选绑定
来源：http://pcs.gotoacloud.top

if let n = opt { print(n) }
来源：http://lvi.jlsjyb.cn

[T20] Swift：数组操作
来源：http://rpn.gogol.net.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xda.quarkkingdee.top

[T21] Swift：遍历
来源：http://jsv.dianchejie.cn

for x in a { print(x) }
来源：http://ezu.guannengcc.top

[T22] Swift：字典
来源：http://hcv.bbcook.cn

var d = ["a": 1];  d["b"] = 2
来源：http://but.sweek.top

[T23] Swift：函数
来源：http://phw.haohaochexian.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zww.jiagoushi.top

[T24] Swift：闭包
来源：http://zja.tarul.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://bpm.hammf.cn

[T25] Swift：结构体
来源：http://dhn.zhengqikj.top

struct P { var x: Int }
来源：http://sdw.shanyushiyangkeji.top

[T26] Swift：类与重写
来源：http://bnh.fehbvm.com

class A: Base { override func f() {} }
来源：http://aou.aibaodan.cn

[T27] Swift：错误处理
来源：http://ubq.zhiwuduotai.top

do { try f() } catch { print(error) }
来源：http://xji.zhixingplan.top

[T28] Swift：枚举
来源：http://xao.quarkkingdee.top

enum Color { case red, green }
来源：http://kva.redwolf501.top

[T29] Swift：guard 提前返回
来源：http://ryo.316326.xyz

guard let x = opt else { return }
来源：http://ean.shanyushiyangtech.top

[T30] Swift：协议
来源：http://kdd.meibo888.top

protocol Shape { func area() -> Double }
来源：http://wdw.jiagoushi.top

[T31] Lua：Hello World
来源：http://xlq.wangshuangyany.cn

print("Hello")
来源：http://res.xuanzx.com

[T32] Lua：局部变量
来源：http://cwr.meibo888.top

local a = 1
来源：http://xaq.sysykeji.top

[T33] Lua：表（数组）
来源：http://iad.guowangkeji.top

local t = {1, 2, 3};  t[4] = 4
来源：http://vdo.zhaomingkeji.xyz

[T34] Lua：遍历表
来源：http://fmd.hnxiangtu.top

for i, v in ipairs(t) do print(i, v) end
来源：http://muv.ydjk.org.cn

[T35] Lua：字典表
来源：http://utb.sysykeji.top

local d = { a = 1 };  d.b = 2
来源：http://slr.birdmap.top

[T36] Lua：函数
来源：http://afe.fehbvm.com

function add(a, b) return a + b end
来源：http://jmj.zhiwuduotai.top

[T37] Lua：字符串拼接
来源：http://oqn.quarkkingdee.top

"a" .. "b"
来源：http://cas.quarkkingdee.top

[T38] Lua：条件
来源：http://otu.quarkkingdee.top

if x > 0 then print("正") end
来源：http://tng.bjfxy.top

[T39] Lua：模式匹配
来源：http://khr.jyoumei.cn

string.find(s, "%d+")
来源：http://mwu.ybcxt.top

[T40] Lua：元表
来源：http://qnm.hywenlv.cn

setmetatable({}, { __index = base })
来源：http://inh.fzhhl.top

[T41] Perl：Hello World
来源：http://cyy.xziqi.cn

print "Hello\n";
来源：http://tap.xuanzx.com

[T42] Perl：变量类型
来源：http://pkx.wangshuangyany.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wuk.jiagoushi.top

[T43] Perl：字符串插值
来源：http://oxp.uphjek.com

"值: $a"
来源：http://tsj.gzhubu.top

[T44] Perl：条件
来源：http://ctt.zhengqikj.top

if ($a > 0) { print "正"; }
来源：http://jft.jlsjyb.cn

[T45] Perl：数组遍历
来源：http://zwi.shanyushiyangkeji.top

for my $x (@arr) { print $x; }
来源：http://lak.fehbvm.com

[T46] Perl：哈希操作
来源：http://ahh.gotoacloud.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wlm.316326.xyz

[T47] Perl：正则捕获
来源：http://vkc.hywenlv.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://nta.nwbrower.top

[T48] Perl：正则替换
来源：http://rcr.aibaodan.cn

$s =~ s/old/new/g;
来源：http://xpx.hysaishi.cn

[T49] Perl：函数
来源：http://sek.yueranfly.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hun.chenzaomai.com

[T50] Perl：逐行读文件
来源：http://rhl.sxryk.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://byw.jinqigufen.top

while (my $line = <$fh>) { print $line; }
来源：http://vuq.feifeiyinyue.top

[T51] Scala：Hello World
来源：http://thk.xinyue.icu

println("Hello")
来源：http://kjy.ywan-chungtsiang.top

[T52] Scala：变量
来源：http://csr.tanke756.top

val a = 1;  var b = 2
来源：http://ksy.quarkkingdee.top

[T53] Scala：字符串插值
来源：http://rpg.hcnkem.com

s"值: $b"
来源：http://pto.jinqigufen.top

[T54] Scala：集合映射
来源：http://lea.gaohongyu789.top

List(1, 2, 3).map(_ * 2)
来源：http://igj.hcnkem.com

[T55] Scala：集合过滤
来源：http://hcl.ydjk.org.cn

List(1, 2, 3).filter(_ > 1)
来源：http://hul.cashguo.top

[T56] Scala：样例类
来源：http://frz.vehdjk.com

case class User(name: String, age: Int)
来源：http://xdf.nanxinkj.top

[T57] Scala：模式匹配
来源：http://juc.tanke756.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://xif.daria6918.cn

[T58] Scala：函数定义
来源：http://hmv.snrcjt.cn

def add(a: Int, b: Int): Int = a + b
来源：http://qrh.hysaishi.cn

[T59] Scala：循环
来源：http://tuw.gogol.net.cn

for (i <- 1 to 10) println(i)
来源：http://ooo.9152youxi.cn

[T60] Scala：折叠
来源：http://cif.tianlin.xyz

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mte.jlsjyb.cn

================================================================================
来源：http://pbl.dashuyun.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zvt.meibo888.top

================================================================================
来源：http://gdu.ehwqpu.com

[U01] Py：创建虚拟环境
来源：http://hqh.jyoumei.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mam.haohaochexian.top

[U02] Py：导出 / 安装依赖
来源：http://vig.yongpay.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wwy.mhx1999.top


<!-- 参考信息 -->