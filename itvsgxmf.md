代发 wailian999

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fyz.guannengcc.top

[R66] 定时任务
来源：http://ykd.bjfxy.top

crontab -e;  crontab -l
来源：http://fxd.hywenlv.cn

[R67] 生成随机十六进制串
来源：http://fhu.jinqigfzy.top

openssl rand -hex 16
来源：http://wrx.chenjidiqi.icu

[R68] 计算文件校验值
来源：http://gim.tarul.cn

sha256sum a.txt;  md5sum a.txt
来源：http://bhw.sysykeji.top

[R69] 生成随机密码
来源：http://cks.yj20258888.top

head -c 16 /dev/urandom | base64
来源：http://eef.jinyuanbaomall.cn

[R70] 时间戳与互转
来源：http://gop.tian-w.cn

date +%s;  date -d @1700000000
来源：http://xgo.sweek.top

[R71] 日期格式化
来源：http://xsu.xziqi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qql.cheryme.top

[R72] 等待端口就绪
来源：http://lki.quarkkingdee.top

until nc -z localhost 3306; do sleep 1; done
来源：http://bkh.jqgufenzy.top

[R73] 分割大日志
来源：http://fay.zdqjudy.top

split -l 1000 big.log part_
来源：http://lhu.zhijiandao.cn

[R74] 批量重命名
来源：http://yry.chenzaomai.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dwx.nanxuanxn.top

[R75] 导出环境变量
来源：http://bcs.hnqzz.top

export PATH="$HOME/bin:$PATH"
来源：http://aln.zdqjudy.top

[R76] 使用临时文件
来源：http://zpe.hnxiangtu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ezt.tarul.cn

[R77] 读取用户输入
来源：http://zmx.shuidangran.top

read -rp "请输入: " ans
来源：http://roc.havefunace.top

[R78] 交互式菜单
来源：http://wkm.zdqjudy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://cfi.sysykeji.top

[R79] 解析命令行选项
来源：http://tnt.andypj.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wql.shanyushiyangtech.top

[R80] 查看脚本执行耗时
来源：http://acb.ydjk.org.cn

time ./run.sh
来源：http://ayc.daria6918.cn

================================================================================
来源：http://czl.ppjwa.cn

S. C / C++ 专题
来源：http://xhe.shangyingyoupin.top

================================================================================
来源：http://cgs.guowangkeji.top

[S01] C：Hello World
来源：http://qyo.fehbvm.com

#include <stdio.h>
来源：http://wvb.nanxuanxn.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://qmn.daria6918.cn

[S02] C：变量与格式化输出
来源：http://qfc.tian-w.cn

int a = 10; printf("%d\n", a);
来源：http://cba.9152youxi.cn

[S03] C：读入整数
来源：http://tin.yj20258.top

int x; scanf("%d", &x);
来源：http://csz.iojbl.cn

[S04] C：字符串复制
来源：http://tqz.uphjek.com

char dst[32]; strcpy(dst, "hi");
来源：http://cxh.hongshengwenyu.top

[S05] C：字符串长度
来源：http://awz.cashguo.top

strlen(s)
来源：http://cpy.chenlongwang.top

[S06] C：字符串比较
来源：http://nwa.cashguo.top

strcmp(a, b) == 0
来源：http://qba.nwbrower.top

[S07] C：数组遍历求和
来源：http://dkp.xylfe.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bgz.xingfuxueyuan.xyz

[S08] C：动态内存分配与释放
来源：http://rmp.quarkkingdee.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mut.wangdashe.top

[S09] C：结构体定义与初始化
来源：http://oky.kuanghao11.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zaz.tarul.cn

[S10] C：指针与解引用
来源：http://tkr.hcnkem.com

int *p = &a;  *p = 5;
来源：http://gjq.zhixingplan.top

[S11] C：逐行读文件
来源：http://bvn.mhx1999.top

FILE *f = fopen("a.txt", "r");
来源：http://mrt.yangfankeji.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://qoe.bjfxy.top

fclose(f);
来源：http://gqa.hesvh.cn

[S12] C：写文件
来源：http://zxw.tian-w.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zrp.hysaishi.cn

[S13] C：宏定义
来源：http://hua.fktsv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://uvs.daria6918.cn

[S14] C：枚举
来源：http://fqm.tianlin.xyz

enum Color { RED, GREEN, BLUE };
来源：http://djy.shuidangran.top

[S15] C：类型转换
来源：http://kba.pengpengdd.cyou

(double) a / b
来源：http://yzn.pycfn.com

[S16] C：位操作置位
来源：http://eyl.nwbrower.top

x |= (1 << 3);
来源：http://nsf.ydzc1.top

[S17] C：安全拼接字符串
来源：http://opj.andypj.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gpw.ivvv.top

[S18] C：命令行参数
来源：http://yhu.kuanghao11.cn

int main(int argc, char **argv)
来源：http://jle.bbcook.cn

[S19] C：快速排序
来源：http://awm.zhengqikj.top

qsort(a, n, sizeof(int), cmp);
来源：http://swz.bbcook.cn

[S20] C：二分查找
来源：http://std.zdbjq.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lzw.gaohongyu789.top

[S21] C：字符类别判断
来源：http://zkv.zhixingplan.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://taz.hongshengwenyu.top

[S22] C：字符串转数字
来源：http://zah.yvedp.cn

atoi("42");  strtod("3.14", NULL);
来源：http://kct.yj20258.top

[S23] C：随机数
来源：http://gpr.zhiwuduotai.top

srand(time(NULL));  int r = rand() % 100;
来源：http://mxs.aizwys.cn

[S24] C：获取本地时间
来源：http://qqp.hcnkem.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://syi.tarul.cn

[S25] C：内存拷贝
来源：http://djv.jlsjyb.cn

memcpy(dst, src, n);
来源：http://skr.hfpthk.cn

[S26] C：内存清零
来源：http://oah.gaohongyu789.top

memset(a, 0, sizeof a);
来源：http://kis.yueranfly.top

[S27] C：定义常量
来源：http://hhq.bbcook.cn

const double PI = 3.14159;
来源：http://taa.redwolf501.top

[S28] C：静态变量
来源：http://kls.zhijiandao.cn

static int counter = 0;
来源：http://rkg.fengsongda.top

[S29] C：变参函数
来源：http://icv.kuanghao11.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zbv.yangfankeji.com

[S30] C：头文件保护
来源：http://ffh.smart0.xyz

#ifndef X_H
来源：http://ipu.gzhubu.top

#define X_H
来源：http://mzw.316326.xyz

#endif
来源：http://hxv.smart0.xyz

[S31] C++：Hello World
来源：http://tcn.pycfn.com

#include <iostream>
来源：http://aid.aizwys.cn

int main() { std::cout << "Hello\n"; }
来源：http://xxx.tanke756.top

[S32] C++：字符串
来源：http://hjf.sjlbkw.cn

std::string s = "hi";  s += "!";
来源：http://arm.jiagoushi.top

[S33] C++：vector 增删
来源：http://auw.tarul.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tjt.birdmap.top

[S34] C++：遍历 vector
来源：http://xrr.yongpay.top

for (auto &x : v) { std::cout << x; }
来源：http://ieu.zhoulong.xyz

[S35] C++：map
来源：http://cak.svipenyu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://psr.yj202588.top

[S36] C++：unordered_map
来源：http://osc.pengpengdd.cyou

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ibe.wangshuangyany.cn

[S37] C++：set
来源：http://bbx.fehbvm.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hql.gaohongyu789.top

[S38] C++：排序
来源：http://qlx.vqdsnc.cn

std::sort(v.begin(), v.end());
来源：http://gyb.cashguo.top

[S39] C++：自定义比较器排序
来源：http://fyp.aizwys.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xee.ywan-chungtsiang.top

[S40] C++：查找元素
来源：http://wju.jinyuanbaomall.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hnr.zhijiandao.cn

[S41] C++：类与构造函数
来源：http://bjn.snrcjt.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://snq.jinqigfzy.top

[S42] C++：继承与虚函数
来源：http://jfu.shangyingyoupin.top

class B : public Base { public: void f() override {} };
来源：http://hlo.sysykeji.top

[S43] C++：智能指针
来源：http://ksx.smart0.xyz

auto p = std::make_unique<int>(5);
来源：http://omb.ybcxt.top

[S44] C++：引用传参
来源：http://tty.yonumen.top

void inc(int &x) { ++x; }
来源：http://xnk.hongshengwenyu.top

[S45] C++：lambda
来源：http://oqq.sjlbkw.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vtt.jinyuanbaomall.cn

[S46] C++：函数模板
来源：http://yba.ppjwa.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://afv.zhaomingkeji.xyz

[S47] C++：结构化绑定遍历
来源：http://bqz.chenlongwang.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xkt.fktsv.cn

[S48] C++：逐行读文件
来源：http://rvl.snrcjt.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jlk.316326.xyz

while (std::getline(in, line)) { }
来源：http://fpa.yueranfly.top

[S49] C++：写文件
来源：http://twh.hnqzz.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://efo.jlsjyb.cn

[S50] C++：格式化数字
来源：http://jdk.ppjwa.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qqu.yangfankeji.com

[S51] C++：显式类型转换
来源：http://cen.iojbl.cn

static_cast<double>(a) / b
来源：http://buo.hysaishi.cn

[S52] C++：const 与 noexcept
来源：http://abk.nanxinkj.top

int size() const noexcept { return n_; }
来源：http://fet.dianchejie.cn

[S53] C++：移动语义
来源：http://wum.gaohongyu789.top

std::vector<int> w = std::move(v);
来源：http://rnk.quarkkingdee.top

[S54] C++：异常处理
来源：http://zij.dianchejie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bnj.daxiang520.top

[S55] C++：结构化绑定
来源：http://brn.hammf.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://khq.jinghuilouyu.cn

[S56] C++：optional
来源：http://hzm.jqgfzy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://amp.dianchejie.cn

[S57] C++：编译期常量
来源：http://ldo.gotoacloud.top

constexpr int N = 10;
来源：http://hmb.tianlin.xyz

[S58] C++：命名空间
来源：http://nly.mhx1999.top

namespace ns { int f() { return 1; } }
来源：http://cbb.jqgufenzy.top

[S59] C++：静态断言
来源：http://qql.jyoumei.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kqy.hongshengwenyu.top

[S60] C++：遍历并删除元素
来源：http://otg.uphjek.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://foz.tian-w.cn

================================================================================
来源：http://lwg.ywan-chungtsiang.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zis.shzxlz.cn

================================================================================
来源：http://zkv.0kj1m.cn

[T01] Kotlin：Hello World
来源：http://bwj.gzhubu.top

println("Hello")
来源：http://xpw.ywan-chungtsiang.top

[T02] Kotlin：变量
来源：http://icj.gogol.net.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jaz.dashuyun.cn

[T03] Kotlin：字符串模板
来源：http://fji.fanxiaobao.xyz

"值: $b"
来源：http://dxi.gzhubu.top

[T04] Kotlin：空安全
来源：http://ygd.fehbvm.com

val n: String? = null;  n?.length
来源：http://rig.hesvh.cn

[T05] Kotlin：when 表达式
来源：http://wmx.yonumen.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lck.cheryme.top

[T06] Kotlin：集合映射
来源：http://pwd.hnqzz.top

listOf(1, 2, 3).map { it * 2 }
来源：http://qbf.jqgfzy.top

[T07] Kotlin：集合过滤
来源：http://qfj.sjlbkw.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ibp.guannengcc.top

[T08] Kotlin：数据类
来源：http://tyu.cheryme.top

data class User(val name: String, val age: Int)
来源：http://kkg.redwolf501.top

[T09] Kotlin：扩展函数
来源：http://ohz.tian-w.cn

fun String.exclaim() = this + "!"
来源：http://imo.yuanzhike.top

[T10] Kotlin：默认参数
来源：http://gxp.jqgfzy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ykp.zhoulong.xyz

[T11] Kotlin：协程
来源：http://vuj.nanxinkj.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://tww.yanxiufei.cn

[T12] Kotlin：解构声明
来源：http://bey.ybcxt.top

val (a, b) = Pair(1, 2)
来源：http://dpr.iojbl.cn

[T13] Kotlin：只读 Map
来源：http://nai.yvedp.cn

val m = mapOf("a" to 1)
来源：http://xun.shuidangran.top

[T14] Kotlin：循环
来源：http://rtl.jyoumei.cn

for (i in 1..10) println(i)
来源：http://vtm.sxryk.cn

[T15] Kotlin：接口
来源：http://gzu.0kj1m.cn

interface Shape { fun area(): Double }
来源：http://mak.snrcjt.cn

[T16] Swift：Hello World
来源：http://mun.yongpay.top

print("Hello")
来源：http://wol.shzxlz.cn

[T17] Swift：变量与常量
来源：http://irh.yfazqb.com

var a = 1;  let b = 2
来源：http://zly.gzhubu.top

[T18] Swift：字符串插值
来源：http://msh.quarkkingdee.top

"值: \(b)"
来源：http://gmz.yj202588.top

[T19] Swift：可选绑定
来源：http://aji.ctjpmb.com

if let n = opt { print(n) }
来源：http://lfa.jqgufenzy.top

[T20] Swift：数组操作
来源：http://jsy.haohaochexian.top

var a = [1, 2, 3];  a.append(4)
来源：http://qlz.birdmap.top

[T21] Swift：遍历
来源：http://zwb.gogol.net.cn

for x in a { print(x) }
来源：http://oic.dianchejie.cn

[T22] Swift：字典
来源：http://bew.xylfe.cn

var d = ["a": 1];  d["b"] = 2
来源：http://yxh.yfazqb.com

[T23] Swift：函数
来源：http://seh.guannengcc.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://uyz.jinyuanbaomall.cn

[T24] Swift：闭包
来源：http://beh.yvedp.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://hny.jinqigfzy.top

[T25] Swift：结构体
来源：http://nea.shuidangran.top

struct P { var x: Int }
来源：http://hpb.zdqjudy.top

[T26] Swift：类与重写
来源：http://epw.meibo888.top

class A: Base { override func f() {} }
来源：http://zuf.andypj.xyz

[T27] Swift：错误处理
来源：http://jno.316326.xyz

do { try f() } catch { print(error) }
来源：http://pga.xingfuxueyuan.xyz

[T28] Swift：枚举
来源：http://vaj.yanxiufei.cn

enum Color { case red, green }
来源：http://kac.ydjk.org.cn

[T29] Swift：guard 提前返回
来源：http://umm.zdqjudy.top

guard let x = opt else { return }
来源：http://dsy.316326.xyz

[T30] Swift：协议
来源：http://vyt.zdbjq.cn

protocol Shape { func area() -> Double }
来源：http://bza.ehwqpu.com

[T31] Lua：Hello World
来源：http://hlx.uphjek.com

print("Hello")
来源：http://hqt.snrcjt.cn

[T32] Lua：局部变量
来源：http://fju.uphjek.com

local a = 1
来源：http://aqw.cqqwz.cn

[T33] Lua：表（数组）
来源：http://kay.zycfv.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ozu.dashuyun.cn

[T34] Lua：遍历表
来源：http://foo.ctjpmb.com

for i, v in ipairs(t) do print(i, v) end
来源：http://egu.fanxiaobao.xyz

[T35] Lua：字典表
来源：http://kyz.sysykeji.top

local d = { a = 1 };  d.b = 2
来源：http://ilm.svipenyu.cn

[T36] Lua：函数
来源：http://vsb.shanyushiyangtech.top

function add(a, b) return a + b end
来源：http://bzn.xuanzx.com

[T37] Lua：字符串拼接
来源：http://mvf.zhongyouzk.top

"a" .. "b"
来源：http://sgg.pengpengdd.cyou

[T38] Lua：条件
来源：http://eel.zhixingplan.top

if x > 0 then print("正") end
来源：http://jtk.gaohongyu789.top

[T39] Lua：模式匹配
来源：http://bvt.yfazqb.com

string.find(s, "%d+")
来源：http://vhp.jlsjyb.cn

[T40] Lua：元表
来源：http://cku.xinyue.icu

setmetatable({}, { __index = base })
来源：http://ryn.ppjwa.cn

[T41] Perl：Hello World
来源：http://dpu.fengsongda.top

print "Hello\n";
来源：http://ynh.cashguo.top

[T42] Perl：变量类型
来源：http://rva.jinyuanbaomall.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nzl.dianchejie.cn

[T43] Perl：字符串插值
来源：http://fid.ydjk.org.cn

"值: $a"
来源：http://qdw.uphjek.com

[T44] Perl：条件
来源：http://kbz.vehdjk.com

if ($a > 0) { print "正"; }
来源：http://itk.epnwcf.com

[T45] Perl：数组遍历
来源：http://poz.xylfe.cn

for my $x (@arr) { print $x; }
来源：http://xjh.sjlbkw.cn

[T46] Perl：哈希操作
来源：http://dye.jinyuanbaomall.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qur.nanxinkj.top

[T47] Perl：正则捕获
来源：http://hsr.yj202588.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://qzx.smart0.xyz

[T48] Perl：正则替换
来源：http://xww.meibo888.top

$s =~ s/old/new/g;
来源：http://xuh.tianlin.xyz

[T49] Perl：函数
来源：http://xrb.hfpthk.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://sph.xylfe.cn

[T50] Perl：逐行读文件
来源：http://ypt.9152youxi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://prt.hcnkem.com

while (my $line = <$fh>) { print $line; }
来源：http://wlf.shangyingyoupin.top

[T51] Scala：Hello World
来源：http://vfv.sjlbkw.cn

println("Hello")
来源：http://ucr.gaohongyu789.top

[T52] Scala：变量
来源：http://elm.chenlongwang.top

val a = 1;  var b = 2
来源：http://kxd.hywenlv.cn

[T53] Scala：字符串插值
来源：http://yhl.jianghu66.top

s"值: $b"
来源：http://gkx.xylfe.cn

[T54] Scala：集合映射
来源：http://mxy.vehdjk.com

List(1, 2, 3).map(_ * 2)
来源：http://hgo.bjfxy.top

[T55] Scala：集合过滤
来源：http://uyi.tarul.cn

List(1, 2, 3).filter(_ > 1)
来源：http://xve.pengpengdd.cyou

[T56] Scala：样例类
来源：http://dju.aizwys.cn

case class User(name: String, age: Int)
来源：http://apv.jqgufenzy.top

[T57] Scala：模式匹配
来源：http://fic.jinqigfzy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://ajn.jqgufenzy.top

[T58] Scala：函数定义
来源：http://rbg.yuxming.cn

def add(a: Int, b: Int): Int = a + b
来源：http://byb.sxryk.cn

[T59] Scala：循环
来源：http://nky.cashguo.top

for (i <- 1 to 10) println(i)
来源：http://zfr.shuidangran.top

[T60] Scala：折叠
来源：http://bge.redwolf501.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nvx.dianchejie.cn

================================================================================
来源：http://arg.guowangkeji.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://shc.hcnkem.com

================================================================================
来源：http://woh.meibo888.top

[U01] Py：创建虚拟环境
来源：http://hlq.pycfn.com

python -m venv .venv && source .venv/bin/activate
来源：http://ohz.yuanzhike.top

[U02] Py：导出 / 安装依赖
来源：http://qia.hywenlv.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wkf.vqdsnc.cn

[U03] Py：加载 .env 配置
来源：http://tci.aizwys.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://mnb.bbcook.cn

[U04] Py：变量调试打印
来源：http://hqq.sjlbkw.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kzm.yuanzhike.top

[U05] Py：列表去重且保序
来源：http://pvq.chenjidiqi.icu

list(dict.fromkeys(arr))
来源：http://oft.jlsjyb.cn

[U06] Py：合并两个字典
来源：http://dqr.guowangkeji.top

{**a, **b}
来源：http://qdh.cashguo.top


<!-- 参考信息 -->