代发 wailian999

free -h;  ps aux | grep nginx
来源：http://pmb.ybcxt.top

[R64] 结束进程
来源：http://wng.0kj1m.cn

kill -9 $(pgrep -f app.py)
来源：http://coa.zdbjq.cn

[R65] 查看端口占用
来源：http://qwq.shangyingyoupin.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bur.pycfn.com

[R66] 定时任务
来源：http://fih.sjlbkw.cn

crontab -e;  crontab -l
来源：http://iiz.jinqigfzy.top

[R67] 生成随机十六进制串
来源：http://llu.jqgfzy.top

openssl rand -hex 16
来源：http://oal.shzxlz.cn

[R68] 计算文件校验值
来源：http://qmy.shanyushiyangtech.top

sha256sum a.txt;  md5sum a.txt
来源：http://omm.zdqjudy.top

[R69] 生成随机密码
来源：http://lnx.sysykeji.top

head -c 16 /dev/urandom | base64
来源：http://uzs.cucudq.cn

[R70] 时间戳与互转
来源：http://nny.sufxvd.cn

date +%s;  date -d @1700000000
来源：http://lbz.shanyushiyangkeji.top

[R71] 日期格式化
来源：http://qzz.xinyue.icu

date +"%Y-%m-%d %H:%M:%S"
来源：http://fsv.zhixingplan.top

[R72] 等待端口就绪
来源：http://eel.hnxiangtu.top

until nc -z localhost 3306; do sleep 1; done
来源：http://obx.sufxvd.cn

[R73] 分割大日志
来源：http://yhu.zhijiandao.cn

split -l 1000 big.log part_
来源：http://vbf.sxryk.cn

[R74] 批量重命名
来源：http://rrf.jinqigfzy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cii.zhaomingkeji.xyz

[R75] 导出环境变量
来源：http://rzc.zdbjq.cn

export PATH="$HOME/bin:$PATH"
来源：http://zwz.andypj.xyz

[R76] 使用临时文件
来源：http://cnc.ydzc1.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tzr.sysykeji.top

[R77] 读取用户输入
来源：http://pdv.xuanzx.com

read -rp "请输入: " ans
来源：http://kar.ehwqpu.com

[R78] 交互式菜单
来源：http://okj.hnqzz.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ura.yanxiufei.cn

[R79] 解析命令行选项
来源：http://jhi.9152youxi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qof.mhx1999.top

[R80] 查看脚本执行耗时
来源：http://acf.zycfv.cn

time ./run.sh
来源：http://apu.cucudq.cn

================================================================================
来源：http://iox.fzhhl.top

S. C / C++ 专题
来源：http://ewp.zhoulong.xyz

================================================================================
来源：http://dvn.haohaochexian.top

[S01] C：Hello World
来源：http://itq.jinghuilouyu.cn

#include <stdio.h>
来源：http://djn.nanxuanxn.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://bzu.yangfankeji.com

[S02] C：变量与格式化输出
来源：http://stt.xingfuxueyuan.xyz

int a = 10; printf("%d\n", a);
来源：http://hvf.gzhubu.top

[S03] C：读入整数
来源：http://nie.tian-w.cn

int x; scanf("%d", &x);
来源：http://fyg.zhaomingkeji.xyz

[S04] C：字符串复制
来源：http://tby.hammf.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ces.yanxiufei.cn

[S05] C：字符串长度
来源：http://obp.snrcjt.cn

strlen(s)
来源：http://lke.dashuyun.cn

[S06] C：字符串比较
来源：http://vat.sysykeji.top

strcmp(a, b) == 0
来源：http://ahn.yanxiufei.cn

[S07] C：数组遍历求和
来源：http://zag.xziqi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://txz.sweek.top

[S08] C：动态内存分配与释放
来源：http://bmx.ppjwa.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tmn.sysykeji.top

[S09] C：结构体定义与初始化
来源：http://hlq.ydzc1.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ldg.vqdsnc.cn

[S10] C：指针与解引用
来源：http://icx.wangshuangyany.cn

int *p = &a;  *p = 5;
来源：http://nqq.kuanghao11.cn

[S11] C：逐行读文件
来源：http://yms.yj20258888.top

FILE *f = fopen("a.txt", "r");
来源：http://eka.shuidangran.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ufl.xuetiantiany.cn

fclose(f);
来源：http://djs.haohaochexian.top

[S12] C：写文件
来源：http://rwx.ywan-chungtsiang.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pfj.chenlongwang.top

[S13] C：宏定义
来源：http://eyg.cqqwz.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wqk.zhengqikj.top

[S14] C：枚举
来源：http://kgr.ybcxt.top

enum Color { RED, GREEN, BLUE };
来源：http://rmm.tanke756.top

[S15] C：类型转换
来源：http://hcg.snrcjt.cn

(double) a / b
来源：http://lsy.nanxinkj.top

[S16] C：位操作置位
来源：http://xco.sjlbkw.cn

x |= (1 << 3);
来源：http://cmg.ywan-chungtsiang.top

[S17] C：安全拼接字符串
来源：http://olq.nanxuanxn.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xms.vqdsnc.cn

[S18] C：命令行参数
来源：http://ceq.zycfv.cn

int main(int argc, char **argv)
来源：http://ley.nanxinkj.top

[S19] C：快速排序
来源：http://chx.chenjidiqi.icu

qsort(a, n, sizeof(int), cmp);
来源：http://pzq.xingfuxueyuan.xyz

[S20] C：二分查找
来源：http://vhm.yfazqb.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ddn.meibo888.top

[S21] C：字符类别判断
来源：http://ffg.nanxinkj.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vzp.xylfe.cn

[S22] C：字符串转数字
来源：http://sjy.tarul.cn

atoi("42");  strtod("3.14", NULL);
来源：http://udt.sweek.top

[S23] C：随机数
来源：http://ntu.shangyingyoupin.top

srand(time(NULL));  int r = rand() % 100;
来源：http://gqh.hfpthk.cn

[S24] C：获取本地时间
来源：http://cus.fktsv.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ztr.ctjpmb.com

[S25] C：内存拷贝
来源：http://yrj.xuetiantiany.cn

memcpy(dst, src, n);
来源：http://ayi.tian-w.cn

[S26] C：内存清零
来源：http://ndf.uphjek.com

memset(a, 0, sizeof a);
来源：http://syr.aizwys.cn

[S27] C：定义常量
来源：http://xey.yangfankeji.com

const double PI = 3.14159;
来源：http://rcn.zhengqikj.top

[S28] C：静态变量
来源：http://jit.tian-w.cn

static int counter = 0;
来源：http://gjs.gzhubu.top

[S29] C：变参函数
来源：http://dxe.nwbrower.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yvy.aizwys.cn

[S30] C：头文件保护
来源：http://rtb.kuanghao11.cn

#ifndef X_H
来源：http://pvs.yfazqb.com

#define X_H
来源：http://woc.sysykeji.top

#endif
来源：http://cby.feifeiyinyue.top

[S31] C++：Hello World
来源：http://rby.yongpay.top

#include <iostream>
来源：http://amn.kuanghao11.cn

int main() { std::cout << "Hello\n"; }
来源：http://xmy.bjfxy.top

[S32] C++：字符串
来源：http://ioh.kuanghao11.cn

std::string s = "hi";  s += "!";
来源：http://hnt.zhoulong.xyz

[S33] C++：vector 增删
来源：http://elq.bbcook.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ubr.yueranfly.top

[S34] C++：遍历 vector
来源：http://iqe.nanxuanxn.top

for (auto &x : v) { std::cout << x; }
来源：http://wpc.yongpay.top

[S35] C++：map
来源：http://dts.xuanzx.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://aqs.sysykeji.top

[S36] C++：unordered_map
来源：http://uzz.meibo888.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zmu.ybcxt.top

[S37] C++：set
来源：http://hon.jinqigufen.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mvi.pengpengdd.cyou

[S38] C++：排序
来源：http://xgd.pycfn.com

std::sort(v.begin(), v.end());
来源：http://xor.shangyingyoupin.top

[S39] C++：自定义比较器排序
来源：http://qwx.cqqwz.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://znh.vqdsnc.cn

[S40] C++：查找元素
来源：http://kve.chenlongwang.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bmu.xylfe.cn

[S41] C++：类与构造函数
来源：http://kub.xuetiantiany.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qbt.chenlongwang.top

[S42] C++：继承与虚函数
来源：http://nmg.52xcode.cn

class B : public Base { public: void f() override {} };
来源：http://dio.hongshengwenyu.top

[S43] C++：智能指针
来源：http://fof.cdnleiting.top

auto p = std::make_unique<int>(5);
来源：http://iqs.yuxming.cn

[S44] C++：引用传参
来源：http://nwx.jinyuanbaomall.cn

void inc(int &x) { ++x; }
来源：http://lqi.svipenyu.cn

[S45] C++：lambda
来源：http://isr.vehdjk.com

auto add = [](int a, int b) { return a + b; };
来源：http://wvc.dianchejie.cn

[S46] C++：函数模板
来源：http://hah.tarul.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rtz.wangshuangyany.cn

[S47] C++：结构化绑定遍历
来源：http://eci.yj20258.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gyo.yuxming.cn

[S48] C++：逐行读文件
来源：http://rpv.guowangkeji.top

std::ifstream in("a.txt");  std::string line;
来源：http://mmu.havefunace.top

while (std::getline(in, line)) { }
来源：http://nfd.hnxiangtu.top

[S49] C++：写文件
来源：http://qnt.snrcjt.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://amz.ywan-chungtsiang.top

[S50] C++：格式化数字
来源：http://oqr.xuetiantiany.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bhl.zhijiandao.cn

[S51] C++：显式类型转换
来源：http://xem.ctjpmb.com

static_cast<double>(a) / b
来源：http://pnm.kuanghao11.cn

[S52] C++：const 与 noexcept
来源：http://idp.yueranfly.top

int size() const noexcept { return n_; }
来源：http://din.fktsv.cn

[S53] C++：移动语义
来源：http://vub.xingfuxueyuan.xyz

std::vector<int> w = std::move(v);
来源：http://miw.9152youxi.cn

[S54] C++：异常处理
来源：http://isy.xylfe.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kcu.ppjwa.cn

[S55] C++：结构化绑定
来源：http://ovb.jqgfzy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://eea.fktsv.cn

[S56] C++：optional
来源：http://ubn.yueranfly.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nqt.tianlin.xyz

[S57] C++：编译期常量
来源：http://nwn.quarkkingdee.top

constexpr int N = 10;
来源：http://diy.yongpay.top

[S58] C++：命名空间
来源：http://qya.dianchejie.cn

namespace ns { int f() { return 1; } }
来源：http://aoj.yvedp.cn

[S59] C++：静态断言
来源：http://pdn.jqgfzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://iur.aizwys.cn

[S60] C++：遍历并删除元素
来源：http://ytc.shanyushiyangtech.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ltu.fengsongda.top

================================================================================
来源：http://mdn.pengpengdd.cyou

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vrr.9152youxi.cn

================================================================================
来源：http://mga.mhx1999.top

[T01] Kotlin：Hello World
来源：http://nrx.epnwcf.com

println("Hello")
来源：http://ljz.gzhubu.top

[T02] Kotlin：变量
来源：http://jkm.hongshengwenyu.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kio.shuidangran.top

[T03] Kotlin：字符串模板
来源：http://ndb.ppjwa.cn

"值: $b"
来源：http://qqf.wangdashe.top

[T04] Kotlin：空安全
来源：http://iqk.snrcjt.cn

val n: String? = null;  n?.length
来源：http://wjf.hcnkem.com

[T05] Kotlin：when 表达式
来源：http://qvv.fktsv.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gwh.shzxlz.cn

[T06] Kotlin：集合映射
来源：http://mri.cdnleiting.top

listOf(1, 2, 3).map { it * 2 }
来源：http://igy.hnqzz.top

[T07] Kotlin：集合过滤
来源：http://lju.jinqigfzy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://oxq.ydjk.org.cn

[T08] Kotlin：数据类
来源：http://slp.zhengqikj.top

data class User(val name: String, val age: Int)
来源：http://jsn.feifeiyinyue.top

[T09] Kotlin：扩展函数
来源：http://abf.xylfe.cn

fun String.exclaim() = this + "!"
来源：http://qbd.zhongyouzk.top

[T10] Kotlin：默认参数
来源：http://qhk.zhengqikj.top

fun greet(name: String = "World") = "Hi $name"
来源：http://bmb.andypj.xyz

[T11] Kotlin：协程
来源：http://tsz.jinqigfzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ryd.shangyingyoupin.top

[T12] Kotlin：解构声明
来源：http://emv.xuetiantiany.cn

val (a, b) = Pair(1, 2)
来源：http://gie.fengsongda.top

[T13] Kotlin：只读 Map
来源：http://ycl.guannengcc.top

val m = mapOf("a" to 1)
来源：http://dvg.nanxinkj.top

[T14] Kotlin：循环
来源：http://ezx.fehbvm.com

for (i in 1..10) println(i)
来源：http://wqx.sufxvd.cn

[T15] Kotlin：接口
来源：http://rla.tanke756.top

interface Shape { fun area(): Double }
来源：http://vxd.guannengcc.top

[T16] Swift：Hello World
来源：http://hmk.hnqzz.top

print("Hello")
来源：http://qwd.yanxiufei.cn

[T17] Swift：变量与常量
来源：http://tjr.yj20258.top

var a = 1;  let b = 2
来源：http://zzu.dianchejie.cn

[T18] Swift：字符串插值
来源：http://uer.uphjek.com

"值: \(b)"
来源：http://yui.ctjpmb.com

[T19] Swift：可选绑定
来源：http://akh.yuanzhike.top

if let n = opt { print(n) }
来源：http://tym.birdmap.top

[T20] Swift：数组操作
来源：http://cxk.316326.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://eub.cashguo.top

[T21] Swift：遍历
来源：http://idv.svipenyu.cn

for x in a { print(x) }
来源：http://yjt.gaohongyu789.top

[T22] Swift：字典
来源：http://gfh.yueranfly.top

var d = ["a": 1];  d["b"] = 2
来源：http://hhm.zycfv.cn

[T23] Swift：函数
来源：http://arv.ydzc1.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wyf.bbcook.cn

[T24] Swift：闭包
来源：http://bhu.hongshengwenyu.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ssm.iojbl.cn

[T25] Swift：结构体
来源：http://dvd.ehwqpu.com

struct P { var x: Int }
来源：http://bxa.feifeiyinyue.top

[T26] Swift：类与重写
来源：http://yup.yj202588.top

class A: Base { override func f() {} }
来源：http://fwa.xuetiantiany.cn

[T27] Swift：错误处理
来源：http://yee.zhixingplan.top

do { try f() } catch { print(error) }
来源：http://oxu.jinghuilouyu.cn

[T28] Swift：枚举
来源：http://jdn.jqgufenzy.top

enum Color { case red, green }
来源：http://mfq.xingfuxueyuan.xyz

[T29] Swift：guard 提前返回
来源：http://dmk.redwolf501.top

guard let x = opt else { return }
来源：http://xgg.zhixingplan.top

[T30] Swift：协议
来源：http://ofb.tanke756.top

protocol Shape { func area() -> Double }
来源：http://gfc.9152youxi.cn

[T31] Lua：Hello World
来源：http://kxa.hnqzz.top

print("Hello")
来源：http://tzn.sxryk.cn

[T32] Lua：局部变量
来源：http://yxa.9152youxi.cn

local a = 1
来源：http://pjj.sufxvd.cn

[T33] Lua：表（数组）
来源：http://eqy.pengpengdd.cyou

local t = {1, 2, 3};  t[4] = 4
来源：http://mhm.nwbrower.top

[T34] Lua：遍历表
来源：http://cyk.yuanzhike.top

for i, v in ipairs(t) do print(i, v) end
来源：http://lxw.ywan-chungtsiang.top

[T35] Lua：字典表
来源：http://rdh.pycfn.com

local d = { a = 1 };  d.b = 2
来源：http://brz.xuetiantiany.cn

[T36] Lua：函数
来源：http://fww.cucudq.cn

function add(a, b) return a + b end
来源：http://nrz.meibo888.top

[T37] Lua：字符串拼接
来源：http://vnn.chenzaomai.com

"a" .. "b"
来源：http://ksv.xingfuxueyuan.xyz

[T38] Lua：条件
来源：http://rvz.ehwqpu.com

if x > 0 then print("正") end
来源：http://evw.snrcjt.cn

[T39] Lua：模式匹配
来源：http://zis.dianchejie.cn

string.find(s, "%d+")
来源：http://iga.xinyue.icu

[T40] Lua：元表
来源：http://giv.zdqjudy.top

setmetatable({}, { __index = base })
来源：http://kqq.hongshengwenyu.top

[T41] Perl：Hello World
来源：http://jza.yanxiufei.cn

print "Hello\n";
来源：http://cyv.zhongyouzk.top

[T42] Perl：变量类型
来源：http://fmt.yanxiufei.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nih.meibo888.top

[T43] Perl：字符串插值
来源：http://eoa.tanke756.top

"值: $a"
来源：http://vad.andypj.xyz

[T44] Perl：条件
来源：http://gae.zdbjq.cn

if ($a > 0) { print "正"; }
来源：http://tfu.dianchejie.cn

[T45] Perl：数组遍历
来源：http://tyz.hysaishi.cn

for my $x (@arr) { print $x; }
来源：http://hjl.shangyingyoupin.top

[T46] Perl：哈希操作
来源：http://inf.xziqi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mcz.hfpthk.cn

[T47] Perl：正则捕获
来源：http://pof.havefunace.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://iuh.ydzc1.top

[T48] Perl：正则替换
来源：http://hej.ehwqpu.com

$s =~ s/old/new/g;
来源：http://ibd.bbcook.cn

[T49] Perl：函数
来源：http://cpg.xziqi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ihd.ydjk.org.cn

[T50] Perl：逐行读文件
来源：http://rgq.guowangkeji.top

open my $fh, "<", "a.txt" or die $!;
来源：http://dmn.cashguo.top

while (my $line = <$fh>) { print $line; }
来源：http://dxv.tianlin.xyz

[T51] Scala：Hello World
来源：http://wvh.jqgfzy.top

println("Hello")
来源：http://kyq.hammf.cn

[T52] Scala：变量
来源：http://wzl.ivvv.top

val a = 1;  var b = 2
来源：http://zcc.haohaochexian.top

[T53] Scala：字符串插值
来源：http://oih.pengpengdd.cyou

s"值: $b"
来源：http://obg.jyoumei.cn

[T54] Scala：集合映射
来源：http://brc.gzhubu.top

List(1, 2, 3).map(_ * 2)
来源：http://cha.andypj.xyz

[T55] Scala：集合过滤
来源：http://yhe.jinyuanbaomall.cn

List(1, 2, 3).filter(_ > 1)
来源：http://brh.gzhubu.top

[T56] Scala：样例类
来源：http://mxe.wangdashe.top

case class User(name: String, age: Int)
来源：http://yez.meibo888.top

[T57] Scala：模式匹配
来源：http://mgv.cashguo.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://xzv.gogol.net.cn

[T58] Scala：函数定义
来源：http://clj.tarul.cn

def add(a: Int, b: Int): Int = a + b
来源：http://rgx.yuxming.cn

[T59] Scala：循环
来源：http://yrf.jqgfzy.top

for (i <- 1 to 10) println(i)
来源：http://ozz.jinghuilouyu.cn

[T60] Scala：折叠
来源：http://ghu.epnwcf.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://chj.jqgfzy.top

================================================================================
来源：http://hbn.jiagoushi.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mau.nanxuanxn.top

================================================================================
来源：http://vmv.sweek.top

[U01] Py：创建虚拟环境
来源：http://lxj.dashuyun.cn

python -m venv .venv && source .venv/bin/activate
来源：http://nxy.nwbrower.top

[U02] Py：导出 / 安装依赖
来源：http://lcc.yangfankeji.com

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pez.jianghu66.top

[U03] Py：加载 .env 配置
来源：http://wyn.0kj1m.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://fyz.feifeiyinyue.top

[U04] Py：变量调试打印
来源：http://ppz.hfpthk.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ira.shuidangran.top


<!-- 参考信息 -->