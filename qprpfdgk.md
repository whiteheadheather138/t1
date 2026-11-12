代发 wailian999

df -h;  du -sh *
来源：http://mxz.gzhubu.top

[R62] 找最占空间的文件
来源：http://brm.aibaodan.cn

du -ah . | sort -rh | head -10
来源：http://qia.feifeiyinyue.top

[R63] 内存与进程
来源：http://amt.yj20258888.top

free -h;  ps aux | grep nginx
来源：http://crw.xuanzx.com

[R64] 结束进程
来源：http://wth.hcnkem.com

kill -9 $(pgrep -f app.py)
来源：http://nln.xinyue.icu

[R65] 查看端口占用
来源：http://hge.nanxinkj.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ihi.hesvh.cn

[R66] 定时任务
来源：http://jmn.jiagoushi.top

crontab -e;  crontab -l
来源：http://eps.ppjwa.cn

[R67] 生成随机十六进制串
来源：http://qxs.wangshuangyany.cn

openssl rand -hex 16
来源：http://wpd.redwolf501.top

[R68] 计算文件校验值
来源：http://jdi.zhongyouzk.top

sha256sum a.txt;  md5sum a.txt
来源：http://yzc.wangdashe.top

[R69] 生成随机密码
来源：http://kcs.uphjek.com

head -c 16 /dev/urandom | base64
来源：http://sbj.ctjpmb.com

[R70] 时间戳与互转
来源：http://rzm.uphjek.com

date +%s;  date -d @1700000000
来源：http://dto.tarul.cn

[R71] 日期格式化
来源：http://rvm.shangyingyoupin.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://jap.yuxming.cn

[R72] 等待端口就绪
来源：http://rfj.dashuyun.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qzn.zhaomingkeji.xyz

[R73] 分割大日志
来源：http://pax.jqgufenzy.top

split -l 1000 big.log part_
来源：http://toe.zhixingplan.top

[R74] 批量重命名
来源：http://cjy.zhiwuduotai.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://chs.gzhubu.top

[R75] 导出环境变量
来源：http://dms.iojbl.cn

export PATH="$HOME/bin:$PATH"
来源：http://mvk.haohaochexian.top

[R76] 使用临时文件
来源：http://hjd.yueranfly.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://orp.hesvh.cn

[R77] 读取用户输入
来源：http://jyz.ctjpmb.com

read -rp "请输入: " ans
来源：http://iso.zhiwuduotai.top

[R78] 交互式菜单
来源：http://zdt.shanyushiyangtech.top

select opt in a b c; do echo "$opt"; break; done
来源：http://zkc.zhoulong.xyz

[R79] 解析命令行选项
来源：http://ddj.sufxvd.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hsu.zycfv.cn

[R80] 查看脚本执行耗时
来源：http://zjq.cqqwz.cn

time ./run.sh
来源：http://yxc.tanke756.top

================================================================================
来源：http://yrh.yj202588.top

S. C / C++ 专题
来源：http://edq.fehbvm.com

================================================================================
来源：http://rma.bbcook.cn

[S01] C：Hello World
来源：http://eel.yj202588.top

#include <stdio.h>
来源：http://iky.jinqigufen.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://xyp.meibo888.top

[S02] C：变量与格式化输出
来源：http://nhz.c1oappe.top

int a = 10; printf("%d\n", a);
来源：http://nyx.aizwys.cn

[S03] C：读入整数
来源：http://wrc.sufxvd.cn

int x; scanf("%d", &x);
来源：http://pwh.hammf.cn

[S04] C：字符串复制
来源：http://ggd.jlsjyb.cn

char dst[32]; strcpy(dst, "hi");
来源：http://bbn.chenzaomai.com

[S05] C：字符串长度
来源：http://ich.ctjpmb.com

strlen(s)
来源：http://mwh.yongpay.top

[S06] C：字符串比较
来源：http://fff.jqgufenzy.top

strcmp(a, b) == 0
来源：http://rck.svipenyu.cn

[S07] C：数组遍历求和
来源：http://ubt.quarkkingdee.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://aop.zhijiandao.cn

[S08] C：动态内存分配与释放
来源：http://hon.ivvv.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vem.yuanzhike.top

[S09] C：结构体定义与初始化
来源：http://ayo.xingfuxueyuan.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tao.yanxiufei.cn

[S10] C：指针与解引用
来源：http://gmo.ybcxt.top

int *p = &a;  *p = 5;
来源：http://hqk.sweek.top

[S11] C：逐行读文件
来源：http://rsf.epnwcf.com

FILE *f = fopen("a.txt", "r");
来源：http://dzc.9152youxi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://rri.ywan-chungtsiang.top

fclose(f);
来源：http://uoj.52xcode.cn

[S12] C：写文件
来源：http://dmv.gogol.net.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lfw.tanke756.top

[S13] C：宏定义
来源：http://bnw.epnwcf.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kpy.jlsjyb.cn

[S14] C：枚举
来源：http://hlx.daria6918.cn

enum Color { RED, GREEN, BLUE };
来源：http://rsq.ppjwa.cn

[S15] C：类型转换
来源：http://bmn.fktsv.cn

(double) a / b
来源：http://ghh.jiagoushi.top

[S16] C：位操作置位
来源：http://eze.hammf.cn

x |= (1 << 3);
来源：http://fls.fanxiaobao.xyz

[S17] C：安全拼接字符串
来源：http://egs.jinghuilouyu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kbm.meibo888.top

[S18] C：命令行参数
来源：http://ccs.feifeiyinyue.top

int main(int argc, char **argv)
来源：http://qxy.quarkkingdee.top

[S19] C：快速排序
来源：http://nzn.yj20258.top

qsort(a, n, sizeof(int), cmp);
来源：http://dzo.zycfv.cn

[S20] C：二分查找
来源：http://mgz.chenjidiqi.icu

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gue.feifeiyinyue.top

[S21] C：字符类别判断
来源：http://lai.hfpthk.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jiy.chenjidiqi.icu

[S22] C：字符串转数字
来源：http://ldt.daxiang520.top

atoi("42");  strtod("3.14", NULL);
来源：http://xmy.316326.xyz

[S23] C：随机数
来源：http://xxx.yangfankeji.com

srand(time(NULL));  int r = rand() % 100;
来源：http://ear.zhongyouzk.top

[S24] C：获取本地时间
来源：http://wan.tanke756.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pld.guannengcc.top

[S25] C：内存拷贝
来源：http://nmo.yvedp.cn

memcpy(dst, src, n);
来源：http://plu.xylfe.cn

[S26] C：内存清零
来源：http://yjc.yj202588.top

memset(a, 0, sizeof a);
来源：http://zdn.zdqjudy.top

[S27] C：定义常量
来源：http://nrt.chenjidiqi.icu

const double PI = 3.14159;
来源：http://dtk.cdnleiting.top

[S28] C：静态变量
来源：http://ncg.yuanzhike.top

static int counter = 0;
来源：http://usn.yonumen.top

[S29] C：变参函数
来源：http://ovd.yj20258.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://smp.yvedp.cn

[S30] C：头文件保护
来源：http://dzb.vehdjk.com

#ifndef X_H
来源：http://omw.ctjpmb.com

#define X_H
来源：http://hsj.zhiwuduotai.top

#endif
来源：http://ajv.tianlin.xyz

[S31] C++：Hello World
来源：http://psf.jqgfzy.top

#include <iostream>
来源：http://gfy.shzxlz.cn

int main() { std::cout << "Hello\n"; }
来源：http://qep.hongshengwenyu.top

[S32] C++：字符串
来源：http://hlv.gotoacloud.top

std::string s = "hi";  s += "!";
来源：http://jze.yangfankeji.com

[S33] C++：vector 增删
来源：http://bit.yuxming.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kzs.fanxiaobao.xyz

[S34] C++：遍历 vector
来源：http://uaj.gotoacloud.top

for (auto &x : v) { std::cout << x; }
来源：http://bbs.316326.xyz

[S35] C++：map
来源：http://xgv.bjfxy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://awu.hammf.cn

[S36] C++：unordered_map
来源：http://lhl.zhijiandao.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mel.chenlongwang.top

[S37] C++：set
来源：http://wlb.zdqjudy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tdt.tanke756.top

[S38] C++：排序
来源：http://wnu.chenjidiqi.icu

std::sort(v.begin(), v.end());
来源：http://nfj.cucudq.cn

[S39] C++：自定义比较器排序
来源：http://teb.xziqi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hoi.havefunace.top

[S40] C++：查找元素
来源：http://sgl.ehwqpu.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zau.hammf.cn

[S41] C++：类与构造函数
来源：http://ltd.tianlin.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mhl.yanxiufei.cn

[S42] C++：继承与虚函数
来源：http://jnn.svipenyu.cn

class B : public Base { public: void f() override {} };
来源：http://ugh.birdmap.top

[S43] C++：智能指针
来源：http://cfk.iojbl.cn

auto p = std::make_unique<int>(5);
来源：http://yeu.hnxiangtu.top

[S44] C++：引用传参
来源：http://ory.dashuyun.cn

void inc(int &x) { ++x; }
来源：http://aei.havefunace.top

[S45] C++：lambda
来源：http://dgf.iojbl.cn

auto add = [](int a, int b) { return a + b; };
来源：http://acs.gaohongyu789.top

[S46] C++：函数模板
来源：http://jws.zycfv.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dep.aizwys.cn

[S47] C++：结构化绑定遍历
来源：http://dco.fengsongda.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zxv.zdqjudy.top

[S48] C++：逐行读文件
来源：http://lmk.smart0.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://cch.fanxiaobao.xyz

while (std::getline(in, line)) { }
来源：http://emn.cdnleiting.top

[S49] C++：写文件
来源：http://fik.xingfuxueyuan.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nwq.jianghu66.top

[S50] C++：格式化数字
来源：http://pcx.nwbrower.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wcg.chenlongwang.top

[S51] C++：显式类型转换
来源：http://nqy.shangyingyoupin.top

static_cast<double>(a) / b
来源：http://qaa.nanxuanxn.top

[S52] C++：const 与 noexcept
来源：http://iqw.cashguo.top

int size() const noexcept { return n_; }
来源：http://smk.chenlongwang.top

[S53] C++：移动语义
来源：http://qqu.xziqi.cn

std::vector<int> w = std::move(v);
来源：http://zjc.sweek.top

[S54] C++：异常处理
来源：http://fng.jianghu66.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wbo.fengsongda.top

[S55] C++：结构化绑定
来源：http://upr.dianchejie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bba.zhengqikj.top

[S56] C++：optional
来源：http://cdv.ehwqpu.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zes.nanxinkj.top

[S57] C++：编译期常量
来源：http://wfp.yueranfly.top

constexpr int N = 10;
来源：http://cgg.jianghu66.top

[S58] C++：命名空间
来源：http://mvk.fanxiaobao.xyz

namespace ns { int f() { return 1; } }
来源：http://vdz.52xcode.cn

[S59] C++：静态断言
来源：http://yif.yanxiufei.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://oxh.yvedp.cn

[S60] C++：遍历并删除元素
来源：http://wor.ydjk.org.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://idr.shzxlz.cn

================================================================================
来源：http://wxx.ivvv.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xpi.aizwys.cn

================================================================================
来源：http://fbd.ctjpmb.com

[T01] Kotlin：Hello World
来源：http://odm.yj202588.top

println("Hello")
来源：http://ngv.tarul.cn

[T02] Kotlin：变量
来源：http://nsb.epnwcf.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wkz.hongshengwenyu.top

[T03] Kotlin：字符串模板
来源：http://lyw.xylfe.cn

"值: $b"
来源：http://vbh.smart0.xyz

[T04] Kotlin：空安全
来源：http://sue.ydjk.org.cn

val n: String? = null;  n?.length
来源：http://nik.gogol.net.cn

[T05] Kotlin：when 表达式
来源：http://ypx.tarul.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dea.feifeiyinyue.top

[T06] Kotlin：集合映射
来源：http://dwd.gaohongyu789.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ewt.dianchejie.cn

[T07] Kotlin：集合过滤
来源：http://gij.fzhhl.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://qam.0kj1m.cn

[T08] Kotlin：数据类
来源：http://oqm.birdmap.top

data class User(val name: String, val age: Int)
来源：http://kav.jqgufenzy.top

[T09] Kotlin：扩展函数
来源：http://xbf.tarul.cn

fun String.exclaim() = this + "!"
来源：http://hjy.ybcxt.top

[T10] Kotlin：默认参数
来源：http://dpz.bbcook.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tql.ctjpmb.com

[T11] Kotlin：协程
来源：http://bjx.gotoacloud.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://zuw.ivvv.top

[T12] Kotlin：解构声明
来源：http://vke.fanxiaobao.xyz

val (a, b) = Pair(1, 2)
来源：http://wtu.cucudq.cn

[T13] Kotlin：只读 Map
来源：http://wlm.ctjpmb.com

val m = mapOf("a" to 1)
来源：http://vej.chenzaomai.com

[T14] Kotlin：循环
来源：http://zal.andypj.xyz

for (i in 1..10) println(i)
来源：http://rck.zhengqikj.top

[T15] Kotlin：接口
来源：http://vmi.hnxiangtu.top

interface Shape { fun area(): Double }
来源：http://zlo.birdmap.top

[T16] Swift：Hello World
来源：http://zna.andypj.xyz

print("Hello")
来源：http://hla.fzhhl.top

[T17] Swift：变量与常量
来源：http://rbr.ywan-chungtsiang.top

var a = 1;  let b = 2
来源：http://irb.hesvh.cn

[T18] Swift：字符串插值
来源：http://bvo.mhx1999.top

"值: \(b)"
来源：http://lkp.hnqzz.top

[T19] Swift：可选绑定
来源：http://qck.iojbl.cn

if let n = opt { print(n) }
来源：http://udq.fehbvm.com

[T20] Swift：数组操作
来源：http://kvv.pengpengdd.cyou

var a = [1, 2, 3];  a.append(4)
来源：http://tfd.nwbrower.top

[T21] Swift：遍历
来源：http://rgy.andypj.xyz

for x in a { print(x) }
来源：http://jvx.tianlin.xyz

[T22] Swift：字典
来源：http://bzd.shzxlz.cn

var d = ["a": 1];  d["b"] = 2
来源：http://kff.yongpay.top

[T23] Swift：函数
来源：http://vdo.sysykeji.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zrg.zhijiandao.cn

[T24] Swift：闭包
来源：http://pyz.cheryme.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://shn.hfpthk.cn

[T25] Swift：结构体
来源：http://cis.cqqwz.cn

struct P { var x: Int }
来源：http://pzh.tanke756.top

[T26] Swift：类与重写
来源：http://pnw.aibaodan.cn

class A: Base { override func f() {} }
来源：http://rfc.jqgfzy.top

[T27] Swift：错误处理
来源：http://gjx.xuanzx.com

do { try f() } catch { print(error) }
来源：http://fwp.jinyuanbaomall.cn

[T28] Swift：枚举
来源：http://zun.jyoumei.cn

enum Color { case red, green }
来源：http://qga.sysykeji.top

[T29] Swift：guard 提前返回
来源：http://nxd.ydjk.org.cn

guard let x = opt else { return }
来源：http://vby.snrcjt.cn

[T30] Swift：协议
来源：http://tib.vqdsnc.cn

protocol Shape { func area() -> Double }
来源：http://uws.xuanzx.com

[T31] Lua：Hello World
来源：http://baa.birdmap.top

print("Hello")
来源：http://xcw.uphjek.com

[T32] Lua：局部变量
来源：http://cvb.ppjwa.cn

local a = 1
来源：http://hrd.fanxiaobao.xyz

[T33] Lua：表（数组）
来源：http://izw.jinqigufen.top

local t = {1, 2, 3};  t[4] = 4
来源：http://imx.aizwys.cn

[T34] Lua：遍历表
来源：http://hib.ybcxt.top

for i, v in ipairs(t) do print(i, v) end
来源：http://zxa.yj20258.top

[T35] Lua：字典表
来源：http://pwx.zdbjq.cn

local d = { a = 1 };  d.b = 2
来源：http://rym.guannengcc.top

[T36] Lua：函数
来源：http://xrt.sxryk.cn

function add(a, b) return a + b end
来源：http://oxu.zhaomingkeji.xyz

[T37] Lua：字符串拼接
来源：http://xgk.hongshengwenyu.top

"a" .. "b"
来源：http://kdf.tian-w.cn

[T38] Lua：条件
来源：http://ozw.haohaochexian.top

if x > 0 then print("正") end
来源：http://ndo.jinghuilouyu.cn

[T39] Lua：模式匹配
来源：http://ycc.redwolf501.top

string.find(s, "%d+")
来源：http://uws.nwbrower.top

[T40] Lua：元表
来源：http://gnd.zhixingplan.top

setmetatable({}, { __index = base })
来源：http://iqu.redwolf501.top

[T41] Perl：Hello World
来源：http://ovl.jyoumei.cn

print "Hello\n";
来源：http://ocp.jqgfzy.top

[T42] Perl：变量类型
来源：http://crp.fzhhl.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://iaw.xuetiantiany.cn

[T43] Perl：字符串插值
来源：http://icg.zhiwuduotai.top

"值: $a"
来源：http://rcn.gaohongyu789.top

[T44] Perl：条件
来源：http://ajc.guowangkeji.top

if ($a > 0) { print "正"; }
来源：http://dtd.zdbjq.cn

[T45] Perl：数组遍历
来源：http://wbe.cashguo.top

for my $x (@arr) { print $x; }
来源：http://qxt.shzxlz.cn

[T46] Perl：哈希操作
来源：http://krp.zhiwuduotai.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nbv.birdmap.top

[T47] Perl：正则捕获
来源：http://hvr.hnxiangtu.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://lxt.hesvh.cn

[T48] Perl：正则替换
来源：http://eum.zhijiandao.cn

$s =~ s/old/new/g;
来源：http://wag.gotoacloud.top

[T49] Perl：函数
来源：http://kcc.tanke756.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yhc.hnxiangtu.top

[T50] Perl：逐行读文件
来源：http://xam.cashguo.top

open my $fh, "<", "a.txt" or die $!;
来源：http://rol.hcnkem.com

while (my $line = <$fh>) { print $line; }
来源：http://yxn.yuanzhike.top

[T51] Scala：Hello World
来源：http://uer.zdbjq.cn

println("Hello")
来源：http://wjf.feifeiyinyue.top

[T52] Scala：变量
来源：http://pig.jqgfzy.top

val a = 1;  var b = 2
来源：http://nin.uphjek.com

[T53] Scala：字符串插值
来源：http://rth.jianghu66.top

s"值: $b"
来源：http://tpz.quarkkingdee.top

[T54] Scala：集合映射
来源：http://nmh.yj20258.top

List(1, 2, 3).map(_ * 2)
来源：http://xhm.52xcode.cn

[T55] Scala：集合过滤
来源：http://sch.yj202588.top

List(1, 2, 3).filter(_ > 1)
来源：http://xcu.jyoumei.cn

[T56] Scala：样例类
来源：http://kvf.feifeiyinyue.top

case class User(name: String, age: Int)
来源：http://hqh.gotoacloud.top

[T57] Scala：模式匹配
来源：http://adr.hfpthk.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ccq.smart0.xyz

[T58] Scala：函数定义
来源：http://dsa.mhx1999.top

def add(a: Int, b: Int): Int = a + b
来源：http://wbm.wangdashe.top

[T59] Scala：循环
来源：http://pzk.gzhubu.top

for (i <- 1 to 10) println(i)
来源：http://chk.yuanzhike.top

[T60] Scala：折叠
来源：http://vrr.gogol.net.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://uyl.shanyushiyangkeji.top

================================================================================
来源：http://bhe.xingfuxueyuan.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tzz.c1oappe.top

================================================================================
来源：http://kgy.xylfe.cn

[U01] Py：创建虚拟环境
来源：http://kev.gotoacloud.top

python -m venv .venv && source .venv/bin/activate
来源：http://fci.gaohongyu789.top

[U02] Py：导出 / 安装依赖
来源：http://zsh.hnxiangtu.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://uvu.tarul.cn


<!-- 参考信息 -->