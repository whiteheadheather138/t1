代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://eoz.zhaomingkeji.xyz

[R66] 定时任务
来源：http://oux.pycfn.com

crontab -e;  crontab -l
来源：http://utt.jqgfzy.top

[R67] 生成随机十六进制串
来源：http://cxz.wangdashe.top

openssl rand -hex 16
来源：http://kjl.vqdsnc.cn

[R68] 计算文件校验值
来源：http://lxq.vqdsnc.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hum.shanyushiyangtech.top

[R69] 生成随机密码
来源：http://spl.wangdashe.top

head -c 16 /dev/urandom | base64
来源：http://qwp.gaohongyu789.top

[R70] 时间戳与互转
来源：http://vjo.cdnleiting.top

date +%s;  date -d @1700000000
来源：http://bhi.sysykeji.top

[R71] 日期格式化
来源：http://jav.aizwys.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://daw.cheryme.top

[R72] 等待端口就绪
来源：http://tdr.ctjpmb.com

until nc -z localhost 3306; do sleep 1; done
来源：http://swu.zhiwuduotai.top

[R73] 分割大日志
来源：http://gsh.guannengcc.top

split -l 1000 big.log part_
来源：http://bwg.guannengcc.top

[R74] 批量重命名
来源：http://pwa.yj20258.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zyr.cdnleiting.top

[R75] 导出环境变量
来源：http://nxg.fktsv.cn

export PATH="$HOME/bin:$PATH"
来源：http://vou.dashuyun.cn

[R76] 使用临时文件
来源：http://jhx.cheryme.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://liw.pengpengdd.cyou

[R77] 读取用户输入
来源：http://zav.jqgfzy.top

read -rp "请输入: " ans
来源：http://ote.vqdsnc.cn

[R78] 交互式菜单
来源：http://lkn.yj20258888.top

select opt in a b c; do echo "$opt"; break; done
来源：http://epo.ehwqpu.com

[R79] 解析命令行选项
来源：http://iey.zdbjq.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://obf.9152youxi.cn

[R80] 查看脚本执行耗时
来源：http://jen.uphjek.com

time ./run.sh
来源：http://pco.sxryk.cn

================================================================================
来源：http://vcv.chenlongwang.top

S. C / C++ 专题
来源：http://edt.nanxinkj.top

================================================================================
来源：http://scx.haohaochexian.top

[S01] C：Hello World
来源：http://tmk.zycfv.cn

#include <stdio.h>
来源：http://czq.aizwys.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://phm.cqqwz.cn

[S02] C：变量与格式化输出
来源：http://ikh.bbcook.cn

int a = 10; printf("%d\n", a);
来源：http://mrf.jlsjyb.cn

[S03] C：读入整数
来源：http://bhs.jinghuilouyu.cn

int x; scanf("%d", &x);
来源：http://ppu.tanke756.top

[S04] C：字符串复制
来源：http://oyg.daria6918.cn

char dst[32]; strcpy(dst, "hi");
来源：http://sxs.pycfn.com

[S05] C：字符串长度
来源：http://tva.chenjidiqi.icu

strlen(s)
来源：http://lbj.bbcook.cn

[S06] C：字符串比较
来源：http://ruq.sufxvd.cn

strcmp(a, b) == 0
来源：http://zvj.ctjpmb.com

[S07] C：数组遍历求和
来源：http://ecc.snrcjt.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://edd.fktsv.cn

[S08] C：动态内存分配与释放
来源：http://ciq.yuxming.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yqs.hnqzz.top

[S09] C：结构体定义与初始化
来源：http://dlz.yueranfly.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://frg.ppjwa.cn

[S10] C：指针与解引用
来源：http://lup.c1oappe.top

int *p = &a;  *p = 5;
来源：http://kgb.shuidangran.top

[S11] C：逐行读文件
来源：http://eni.ctjpmb.com

FILE *f = fopen("a.txt", "r");
来源：http://lvo.iojbl.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://pce.ydjk.org.cn

fclose(f);
来源：http://wqk.yonumen.top

[S12] C：写文件
来源：http://hmb.tanke756.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hut.sufxvd.cn

[S13] C：宏定义
来源：http://zxq.daria6918.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lxe.yangfankeji.com

[S14] C：枚举
来源：http://vkq.gogol.net.cn

enum Color { RED, GREEN, BLUE };
来源：http://kyl.ppjwa.cn

[S15] C：类型转换
来源：http://nlm.zdbjq.cn

(double) a / b
来源：http://ksd.yongpay.top

[S16] C：位操作置位
来源：http://zqs.bjfxy.top

x |= (1 << 3);
来源：http://wuv.cdnleiting.top

[S17] C：安全拼接字符串
来源：http://dfm.hfpthk.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ihg.52xcode.cn

[S18] C：命令行参数
来源：http://daa.aibaodan.cn

int main(int argc, char **argv)
来源：http://vnn.dianchejie.cn

[S19] C：快速排序
来源：http://hid.shanyushiyangtech.top

qsort(a, n, sizeof(int), cmp);
来源：http://dmg.vehdjk.com

[S20] C：二分查找
来源：http://mym.kuanghao11.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dgi.0kj1m.cn

[S21] C：字符类别判断
来源：http://lfi.jlsjyb.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tzl.sufxvd.cn

[S22] C：字符串转数字
来源：http://cbl.nanxinkj.top

atoi("42");  strtod("3.14", NULL);
来源：http://dne.hysaishi.cn

[S23] C：随机数
来源：http://jzh.sufxvd.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://mlm.epnwcf.com

[S24] C：获取本地时间
来源：http://yva.chenjidiqi.icu

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://itj.pycfn.com

[S25] C：内存拷贝
来源：http://rui.yuanzhike.top

memcpy(dst, src, n);
来源：http://tgc.hongshengwenyu.top

[S26] C：内存清零
来源：http://rmn.ydzc1.top

memset(a, 0, sizeof a);
来源：http://beq.jyoumei.cn

[S27] C：定义常量
来源：http://gbl.zhaomingkeji.xyz

const double PI = 3.14159;
来源：http://wzc.wangdashe.top

[S28] C：静态变量
来源：http://oqw.jqgufenzy.top

static int counter = 0;
来源：http://wgx.52xcode.cn

[S29] C：变参函数
来源：http://zie.daxiang520.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vns.jqgfzy.top

[S30] C：头文件保护
来源：http://vay.9152youxi.cn

#ifndef X_H
来源：http://srj.cqqwz.cn

#define X_H
来源：http://wua.cheryme.top

#endif
来源：http://rtb.cheryme.top

[S31] C++：Hello World
来源：http://yrx.dashuyun.cn

#include <iostream>
来源：http://ysb.guowangkeji.top

int main() { std::cout << "Hello\n"; }
来源：http://crx.gaohongyu789.top

[S32] C++：字符串
来源：http://mrd.ydzc1.top

std::string s = "hi";  s += "!";
来源：http://xpv.sysykeji.top

[S33] C++：vector 增删
来源：http://asl.jianghu66.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://udd.epnwcf.com

[S34] C++：遍历 vector
来源：http://dan.tian-w.cn

for (auto &x : v) { std::cout << x; }
来源：http://wnb.jinqigufen.top

[S35] C++：map
来源：http://vzn.yj20258.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sgg.ppjwa.cn

[S36] C++：unordered_map
来源：http://kxq.aizwys.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jrf.shanyushiyangkeji.top

[S37] C++：set
来源：http://ohr.wangdashe.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ppf.cdnleiting.top

[S38] C++：排序
来源：http://fzk.shuidangran.top

std::sort(v.begin(), v.end());
来源：http://pmy.jqgfzy.top

[S39] C++：自定义比较器排序
来源：http://qut.shanyushiyangtech.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gcr.sysykeji.top

[S40] C++：查找元素
来源：http://buq.vehdjk.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lws.ivvv.top

[S41] C++：类与构造函数
来源：http://lrl.guowangkeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hsv.yueranfly.top

[S42] C++：继承与虚函数
来源：http://rtp.0kj1m.cn

class B : public Base { public: void f() override {} };
来源：http://dsl.tarul.cn

[S43] C++：智能指针
来源：http://qtk.daria6918.cn

auto p = std::make_unique<int>(5);
来源：http://jpu.xuetiantiany.cn

[S44] C++：引用传参
来源：http://tfa.fehbvm.com

void inc(int &x) { ++x; }
来源：http://tnn.feifeiyinyue.top

[S45] C++：lambda
来源：http://xmk.yuanzhike.top

auto add = [](int a, int b) { return a + b; };
来源：http://dtk.sxryk.cn

[S46] C++：函数模板
来源：http://qyc.shzxlz.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ody.feifeiyinyue.top

[S47] C++：结构化绑定遍历
来源：http://had.chenlongwang.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zpf.kuanghao11.cn

[S48] C++：逐行读文件
来源：http://fyd.zdqjudy.top

std::ifstream in("a.txt");  std::string line;
来源：http://ory.zdqjudy.top

while (std::getline(in, line)) { }
来源：http://kxi.hammf.cn

[S49] C++：写文件
来源：http://dhd.uphjek.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://unl.ydzc1.top

[S50] C++：格式化数字
来源：http://fqe.hnxiangtu.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ihv.ivvv.top

[S51] C++：显式类型转换
来源：http://dqi.xingfuxueyuan.xyz

static_cast<double>(a) / b
来源：http://yzu.ydjk.org.cn

[S52] C++：const 与 noexcept
来源：http://zik.ydzc1.top

int size() const noexcept { return n_; }
来源：http://ayn.nanxinkj.top

[S53] C++：移动语义
来源：http://xoq.yonumen.top

std::vector<int> w = std::move(v);
来源：http://hzm.52xcode.cn

[S54] C++：异常处理
来源：http://lkk.aizwys.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gjb.jqgufenzy.top

[S55] C++：结构化绑定
来源：http://sdb.jianghu66.top

auto [a, b] = std::make_pair(1, 2);
来源：http://kjf.meibo888.top

[S56] C++：optional
来源：http://vzs.zhengqikj.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rdi.shuidangran.top

[S57] C++：编译期常量
来源：http://ubx.gotoacloud.top

constexpr int N = 10;
来源：http://nxd.yueranfly.top

[S58] C++：命名空间
来源：http://pio.jianghu66.top

namespace ns { int f() { return 1; } }
来源：http://nei.tianlin.xyz

[S59] C++：静态断言
来源：http://cil.feifeiyinyue.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ead.epnwcf.com

[S60] C++：遍历并删除元素
来源：http://zki.feifeiyinyue.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://str.ywan-chungtsiang.top

================================================================================
来源：http://kpy.nanxinkj.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gkp.jinqigfzy.top

================================================================================
来源：http://vgn.sweek.top

[T01] Kotlin：Hello World
来源：http://szw.cqqwz.cn

println("Hello")
来源：http://dpm.mhx1999.top

[T02] Kotlin：变量
来源：http://pgd.epnwcf.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gqy.gzhubu.top

[T03] Kotlin：字符串模板
来源：http://xey.chenzaomai.com

"值: $b"
来源：http://ojn.tian-w.cn

[T04] Kotlin：空安全
来源：http://cdz.jlsjyb.cn

val n: String? = null;  n?.length
来源：http://ezs.cdnleiting.top

[T05] Kotlin：when 表达式
来源：http://qyy.ydzc1.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ndh.feifeiyinyue.top

[T06] Kotlin：集合映射
来源：http://vlu.pengpengdd.cyou

listOf(1, 2, 3).map { it * 2 }
来源：http://iau.shzxlz.cn

[T07] Kotlin：集合过滤
来源：http://slq.jlsjyb.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ukj.wangdashe.top

[T08] Kotlin：数据类
来源：http://xxs.smart0.xyz

data class User(val name: String, val age: Int)
来源：http://arw.zhoulong.xyz

[T09] Kotlin：扩展函数
来源：http://tfw.pengpengdd.cyou

fun String.exclaim() = this + "!"
来源：http://knc.zhiwuduotai.top

[T10] Kotlin：默认参数
来源：http://mpa.jqgufenzy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ulz.shangyingyoupin.top

[T11] Kotlin：协程
来源：http://ory.jyoumei.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://pkf.jqgufenzy.top

[T12] Kotlin：解构声明
来源：http://cmc.wangshuangyany.cn

val (a, b) = Pair(1, 2)
来源：http://njx.jyoumei.cn

[T13] Kotlin：只读 Map
来源：http://bcr.jyoumei.cn

val m = mapOf("a" to 1)
来源：http://xdd.hesvh.cn

[T14] Kotlin：循环
来源：http://ygx.chenjidiqi.icu

for (i in 1..10) println(i)
来源：http://ocf.jiagoushi.top

[T15] Kotlin：接口
来源：http://pdk.havefunace.top

interface Shape { fun area(): Double }
来源：http://zfu.0kj1m.cn

[T16] Swift：Hello World
来源：http://sgh.sxryk.cn

print("Hello")
来源：http://dho.zhoulong.xyz

[T17] Swift：变量与常量
来源：http://drr.svipenyu.cn

var a = 1;  let b = 2
来源：http://pft.svipenyu.cn

[T18] Swift：字符串插值
来源：http://fxm.chenlongwang.top

"值: \(b)"
来源：http://vpg.cashguo.top

[T19] Swift：可选绑定
来源：http://wwh.jianghu66.top

if let n = opt { print(n) }
来源：http://wyj.ehwqpu.com

[T20] Swift：数组操作
来源：http://kyg.dianchejie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://tfk.zhiwuduotai.top

[T21] Swift：遍历
来源：http://jli.tanke756.top

for x in a { print(x) }
来源：http://agq.ydzc1.top

[T22] Swift：字典
来源：http://nqm.xuetiantiany.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ben.jqgfzy.top

[T23] Swift：函数
来源：http://cgf.shuidangran.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://igm.zhoulong.xyz

[T24] Swift：闭包
来源：http://hol.ydjk.org.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xsi.cdnleiting.top

[T25] Swift：结构体
来源：http://bod.xingfuxueyuan.xyz

struct P { var x: Int }
来源：http://itg.jqgufenzy.top

[T26] Swift：类与重写
来源：http://wjh.fktsv.cn

class A: Base { override func f() {} }
来源：http://und.wangshuangyany.cn

[T27] Swift：错误处理
来源：http://hpg.sysykeji.top

do { try f() } catch { print(error) }
来源：http://hpm.sxryk.cn

[T28] Swift：枚举
来源：http://pcv.dashuyun.cn

enum Color { case red, green }
来源：http://rgj.bbcook.cn

[T29] Swift：guard 提前返回
来源：http://lui.nanxuanxn.top

guard let x = opt else { return }
来源：http://fnd.shangyingyoupin.top

[T30] Swift：协议
来源：http://teh.hfpthk.cn

protocol Shape { func area() -> Double }
来源：http://ilp.shangyingyoupin.top

[T31] Lua：Hello World
来源：http://cpt.shzxlz.cn

print("Hello")
来源：http://zfs.gotoacloud.top

[T32] Lua：局部变量
来源：http://bti.zycfv.cn

local a = 1
来源：http://fwd.hfpthk.cn

[T33] Lua：表（数组）
来源：http://xuv.yuxming.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://oof.yangfankeji.com

[T34] Lua：遍历表
来源：http://ubt.zhixingplan.top

for i, v in ipairs(t) do print(i, v) end
来源：http://sce.snrcjt.cn

[T35] Lua：字典表
来源：http://oou.yfazqb.com

local d = { a = 1 };  d.b = 2
来源：http://fcf.ydjk.org.cn

[T36] Lua：函数
来源：http://zop.hongshengwenyu.top

function add(a, b) return a + b end
来源：http://pbn.quarkkingdee.top

[T37] Lua：字符串拼接
来源：http://bvs.sjlbkw.cn

"a" .. "b"
来源：http://lty.nanxuanxn.top

[T38] Lua：条件
来源：http://ftl.redwolf501.top

if x > 0 then print("正") end
来源：http://vto.52xcode.cn

[T39] Lua：模式匹配
来源：http://xhd.fzhhl.top

string.find(s, "%d+")
来源：http://cjh.shanyushiyangtech.top

[T40] Lua：元表
来源：http://pzy.pycfn.com

setmetatable({}, { __index = base })
来源：http://xfi.ehwqpu.com

[T41] Perl：Hello World
来源：http://sfp.gzhubu.top

print "Hello\n";
来源：http://xzf.meibo888.top

[T42] Perl：变量类型
来源：http://dmc.xziqi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kgl.birdmap.top

[T43] Perl：字符串插值
来源：http://ayy.shanyushiyangkeji.top

"值: $a"
来源：http://zhc.ppjwa.cn

[T44] Perl：条件
来源：http://qgh.fktsv.cn

if ($a > 0) { print "正"; }
来源：http://uki.kuanghao11.cn

[T45] Perl：数组遍历
来源：http://fpr.sweek.top

for my $x (@arr) { print $x; }
来源：http://xqi.quarkkingdee.top

[T46] Perl：哈希操作
来源：http://hth.gaohongyu789.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lrq.ywan-chungtsiang.top

[T47] Perl：正则捕获
来源：http://wgd.aizwys.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://yjt.cdnleiting.top

[T48] Perl：正则替换
来源：http://vsm.jinqigfzy.top

$s =~ s/old/new/g;
来源：http://tfl.bjfxy.top

[T49] Perl：函数
来源：http://ejy.tianlin.xyz

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pcc.epnwcf.com

[T50] Perl：逐行读文件
来源：http://tpc.nanxinkj.top

open my $fh, "<", "a.txt" or die $!;
来源：http://krm.ehwqpu.com

while (my $line = <$fh>) { print $line; }
来源：http://drk.ivvv.top

[T51] Scala：Hello World
来源：http://xzf.quarkkingdee.top

println("Hello")
来源：http://ven.smart0.xyz

[T52] Scala：变量
来源：http://rtg.jinghuilouyu.cn

val a = 1;  var b = 2
来源：http://jud.hfpthk.cn

[T53] Scala：字符串插值
来源：http://zcp.ywan-chungtsiang.top

s"值: $b"
来源：http://rzf.smart0.xyz

[T54] Scala：集合映射
来源：http://ybm.shanyushiyangkeji.top

List(1, 2, 3).map(_ * 2)
来源：http://bvi.ctjpmb.com

[T55] Scala：集合过滤
来源：http://oqo.andypj.xyz

List(1, 2, 3).filter(_ > 1)
来源：http://kyb.jinyuanbaomall.cn

[T56] Scala：样例类
来源：http://dpp.redwolf501.top

case class User(name: String, age: Int)
来源：http://ksc.0kj1m.cn

[T57] Scala：模式匹配
来源：http://wiz.xuetiantiany.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://wnx.tanke756.top

[T58] Scala：函数定义
来源：http://fsg.chenlongwang.top

def add(a: Int, b: Int): Int = a + b
来源：http://ljq.ppjwa.cn

[T59] Scala：循环
来源：http://kdu.jinyuanbaomall.cn

for (i <- 1 to 10) println(i)
来源：http://cpn.aizwys.cn

[T60] Scala：折叠
来源：http://kmb.chenlongwang.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jkz.zhoulong.xyz

================================================================================
来源：http://nnj.yj202588.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xnk.shangyingyoupin.top

================================================================================
来源：http://yyt.xziqi.cn

[U01] Py：创建虚拟环境
来源：http://eco.wangshuangyany.cn

python -m venv .venv && source .venv/bin/activate
来源：http://zgg.zhixingplan.top

[U02] Py：导出 / 安装依赖
来源：http://ioi.ppjwa.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ahc.snrcjt.cn

[U03] Py：加载 .env 配置
来源：http://tyz.hfpthk.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://fjs.ywan-chungtsiang.top

[U04] Py：变量调试打印
来源：http://nvb.zhoulong.xyz

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://seq.sxryk.cn

[U05] Py：列表去重且保序
来源：http://kuy.sjlbkw.cn

list(dict.fromkeys(arr))
来源：http://kdz.tian-w.cn

[U06] Py：合并两个字典
来源：http://ebf.c1oappe.top

{**a, **b}
来源：http://yvu.haohaochexian.top


<!-- 参考信息 -->