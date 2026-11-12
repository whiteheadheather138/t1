代发 wailian999

free -h;  ps aux | grep nginx
来源：http://fnq.iojbl.cn

[R64] 结束进程
来源：http://iou.daxiang520.top

kill -9 $(pgrep -f app.py)
来源：http://hod.zhoulong.xyz

[R65] 查看端口占用
来源：http://wkh.andypj.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wsr.hfpthk.cn

[R66] 定时任务
来源：http://qyy.daria6918.cn

crontab -e;  crontab -l
来源：http://xrm.iojbl.cn

[R67] 生成随机十六进制串
来源：http://oxp.bbcook.cn

openssl rand -hex 16
来源：http://gpo.mhx1999.top

[R68] 计算文件校验值
来源：http://hib.ctjpmb.com

sha256sum a.txt;  md5sum a.txt
来源：http://zsr.ehwqpu.com

[R69] 生成随机密码
来源：http://uam.nanxinkj.top

head -c 16 /dev/urandom | base64
来源：http://bzu.nwbrower.top

[R70] 时间戳与互转
来源：http://daq.zhixingplan.top

date +%s;  date -d @1700000000
来源：http://xdi.tianlin.xyz

[R71] 日期格式化
来源：http://rpk.gzhubu.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://bhm.fanxiaobao.xyz

[R72] 等待端口就绪
来源：http://tpb.shzxlz.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://nci.jqgufenzy.top

[R73] 分割大日志
来源：http://tne.smart0.xyz

split -l 1000 big.log part_
来源：http://ovp.bjfxy.top

[R74] 批量重命名
来源：http://ovt.jlsjyb.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mbk.hywenlv.cn

[R75] 导出环境变量
来源：http://acu.havefunace.top

export PATH="$HOME/bin:$PATH"
来源：http://bih.hfpthk.cn

[R76] 使用临时文件
来源：http://umh.hysaishi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lkt.chenlongwang.top

[R77] 读取用户输入
来源：http://ncj.shuidangran.top

read -rp "请输入: " ans
来源：http://rag.guannengcc.top

[R78] 交互式菜单
来源：http://wzm.daxiang520.top

select opt in a b c; do echo "$opt"; break; done
来源：http://adq.yvedp.cn

[R79] 解析命令行选项
来源：http://ufe.shangyingyoupin.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mdy.uphjek.com

[R80] 查看脚本执行耗时
来源：http://qwc.zhoulong.xyz

time ./run.sh
来源：http://igb.sxryk.cn

================================================================================
来源：http://tbh.andypj.xyz

S. C / C++ 专题
来源：http://zks.nwbrower.top

================================================================================
来源：http://jhm.zhixingplan.top

[S01] C：Hello World
来源：http://nos.cucudq.cn

#include <stdio.h>
来源：http://xxa.zhengqikj.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://kxj.nwbrower.top

[S02] C：变量与格式化输出
来源：http://hka.xylfe.cn

int a = 10; printf("%d\n", a);
来源：http://sgs.xylfe.cn

[S03] C：读入整数
来源：http://kia.zhijiandao.cn

int x; scanf("%d", &x);
来源：http://gko.aibaodan.cn

[S04] C：字符串复制
来源：http://acf.kuanghao11.cn

char dst[32]; strcpy(dst, "hi");
来源：http://yjn.aizwys.cn

[S05] C：字符串长度
来源：http://vyi.dashuyun.cn

strlen(s)
来源：http://hox.shangyingyoupin.top

[S06] C：字符串比较
来源：http://ave.chenjidiqi.icu

strcmp(a, b) == 0
来源：http://aqr.9152youxi.cn

[S07] C：数组遍历求和
来源：http://hni.hnqzz.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fmo.hesvh.cn

[S08] C：动态内存分配与释放
来源：http://nyd.smart0.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pgu.fzhhl.top

[S09] C：结构体定义与初始化
来源：http://hns.jlsjyb.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://iek.zhiwuduotai.top

[S10] C：指针与解引用
来源：http://frh.wangshuangyany.cn

int *p = &a;  *p = 5;
来源：http://bnc.sjlbkw.cn

[S11] C：逐行读文件
来源：http://diy.hongshengwenyu.top

FILE *f = fopen("a.txt", "r");
来源：http://gom.hywenlv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://buh.nwbrower.top

fclose(f);
来源：http://yrs.xylfe.cn

[S12] C：写文件
来源：http://afl.yonumen.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zkz.zhoulong.xyz

[S13] C：宏定义
来源：http://qkn.pengpengdd.cyou

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jrm.c1oappe.top

[S14] C：枚举
来源：http://gro.xingfuxueyuan.xyz

enum Color { RED, GREEN, BLUE };
来源：http://dcm.bjfxy.top

[S15] C：类型转换
来源：http://uev.jqgufenzy.top

(double) a / b
来源：http://yyi.aizwys.cn

[S16] C：位操作置位
来源：http://syw.guannengcc.top

x |= (1 << 3);
来源：http://imu.cqqwz.cn

[S17] C：安全拼接字符串
来源：http://wwv.ywan-chungtsiang.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://atj.ctjpmb.com

[S18] C：命令行参数
来源：http://qnz.hcnkem.com

int main(int argc, char **argv)
来源：http://urp.zdqjudy.top

[S19] C：快速排序
来源：http://vyg.hongshengwenyu.top

qsort(a, n, sizeof(int), cmp);
来源：http://mal.fanxiaobao.xyz

[S20] C：二分查找
来源：http://uru.dashuyun.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bpp.jinyuanbaomall.cn

[S21] C：字符类别判断
来源：http://lkp.nanxinkj.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://eqd.shuidangran.top

[S22] C：字符串转数字
来源：http://brl.fanxiaobao.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://sgz.tian-w.cn

[S23] C：随机数
来源：http://cpx.tian-w.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qqb.zdqjudy.top

[S24] C：获取本地时间
来源：http://rkg.yueranfly.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xqu.hongshengwenyu.top

[S25] C：内存拷贝
来源：http://vim.tarul.cn

memcpy(dst, src, n);
来源：http://mlq.jyoumei.cn

[S26] C：内存清零
来源：http://bdh.ehwqpu.com

memset(a, 0, sizeof a);
来源：http://rya.ydjk.org.cn

[S27] C：定义常量
来源：http://map.shanyushiyangkeji.top

const double PI = 3.14159;
来源：http://rtz.birdmap.top

[S28] C：静态变量
来源：http://exq.tian-w.cn

static int counter = 0;
来源：http://pwh.pycfn.com

[S29] C：变参函数
来源：http://yrm.tianlin.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pqi.tarul.cn

[S30] C：头文件保护
来源：http://tpy.gaohongyu789.top

#ifndef X_H
来源：http://iyb.dashuyun.cn

#define X_H
来源：http://ugl.bjfxy.top

#endif
来源：http://hww.cdnleiting.top

[S31] C++：Hello World
来源：http://kwb.zhengqikj.top

#include <iostream>
来源：http://vzg.sufxvd.cn

int main() { std::cout << "Hello\n"; }
来源：http://zsw.guannengcc.top

[S32] C++：字符串
来源：http://qfm.yonumen.top

std::string s = "hi";  s += "!";
来源：http://lti.bbcook.cn

[S33] C++：vector 增删
来源：http://qlx.jinqigfzy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wbk.jqgfzy.top

[S34] C++：遍历 vector
来源：http://fci.sysykeji.top

for (auto &x : v) { std::cout << x; }
来源：http://wwb.shanyushiyangtech.top

[S35] C++：map
来源：http://yia.fengsongda.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tdl.tanke756.top

[S36] C++：unordered_map
来源：http://xzh.0kj1m.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://anw.hnxiangtu.top

[S37] C++：set
来源：http://dvy.iojbl.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mjg.wangdashe.top

[S38] C++：排序
来源：http://krp.jinghuilouyu.cn

std::sort(v.begin(), v.end());
来源：http://glo.smart0.xyz

[S39] C++：自定义比较器排序
来源：http://xuf.sysykeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rzy.mhx1999.top

[S40] C++：查找元素
来源：http://cng.yonumen.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wvj.hywenlv.cn

[S41] C++：类与构造函数
来源：http://rzg.andypj.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ykd.tianlin.xyz

[S42] C++：继承与虚函数
来源：http://kcv.epnwcf.com

class B : public Base { public: void f() override {} };
来源：http://qaq.zhengqikj.top

[S43] C++：智能指针
来源：http://utg.zhoulong.xyz

auto p = std::make_unique<int>(5);
来源：http://kjn.redwolf501.top

[S44] C++：引用传参
来源：http://tzo.bjfxy.top

void inc(int &x) { ++x; }
来源：http://uqo.yvedp.cn

[S45] C++：lambda
来源：http://jne.jqgfzy.top

auto add = [](int a, int b) { return a + b; };
来源：http://xbl.epnwcf.com

[S46] C++：函数模板
来源：http://hpm.aizwys.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jra.cqqwz.cn

[S47] C++：结构化绑定遍历
来源：http://wfw.yfazqb.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ytw.hfpthk.cn

[S48] C++：逐行读文件
来源：http://vbi.hnxiangtu.top

std::ifstream in("a.txt");  std::string line;
来源：http://ozr.yangfankeji.com

while (std::getline(in, line)) { }
来源：http://eca.fengsongda.top

[S49] C++：写文件
来源：http://bop.ybcxt.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://skn.yj20258888.top

[S50] C++：格式化数字
来源：http://mxl.hammf.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vlq.birdmap.top

[S51] C++：显式类型转换
来源：http://wlr.hcnkem.com

static_cast<double>(a) / b
来源：http://shg.nwbrower.top

[S52] C++：const 与 noexcept
来源：http://rqg.fzhhl.top

int size() const noexcept { return n_; }
来源：http://ktx.guowangkeji.top

[S53] C++：移动语义
来源：http://vrn.feifeiyinyue.top

std::vector<int> w = std::move(v);
来源：http://jaj.aizwys.cn

[S54] C++：异常处理
来源：http://plk.chenjidiqi.icu

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bcn.xuanzx.com

[S55] C++：结构化绑定
来源：http://wgm.yanxiufei.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bdo.xylfe.cn

[S56] C++：optional
来源：http://esk.xuetiantiany.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://atl.guannengcc.top

[S57] C++：编译期常量
来源：http://vsi.c1oappe.top

constexpr int N = 10;
来源：http://zmq.haohaochexian.top

[S58] C++：命名空间
来源：http://kru.sufxvd.cn

namespace ns { int f() { return 1; } }
来源：http://svf.ybcxt.top

[S59] C++：静态断言
来源：http://oxa.snrcjt.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fgr.fzhhl.top

[S60] C++：遍历并删除元素
来源：http://kyq.hesvh.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mfx.gotoacloud.top

================================================================================
来源：http://cnh.kuanghao11.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kwo.smart0.xyz

================================================================================
来源：http://yzc.yj202588.top

[T01] Kotlin：Hello World
来源：http://yct.hysaishi.cn

println("Hello")
来源：http://csb.jinqigufen.top

[T02] Kotlin：变量
来源：http://gxe.gotoacloud.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://prh.havefunace.top

[T03] Kotlin：字符串模板
来源：http://sjg.aibaodan.cn

"值: $b"
来源：http://kga.gotoacloud.top

[T04] Kotlin：空安全
来源：http://tbl.nwbrower.top

val n: String? = null;  n?.length
来源：http://hpo.kuanghao11.cn

[T05] Kotlin：when 表达式
来源：http://blj.tian-w.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://otc.mhx1999.top

[T06] Kotlin：集合映射
来源：http://akg.dashuyun.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tju.ybcxt.top

[T07] Kotlin：集合过滤
来源：http://pja.xinyue.icu

listOf(1, 2, 3).filter { it > 1 }
来源：http://iod.nwbrower.top

[T08] Kotlin：数据类
来源：http://fum.kuanghao11.cn

data class User(val name: String, val age: Int)
来源：http://peo.guowangkeji.top

[T09] Kotlin：扩展函数
来源：http://djw.xuetiantiany.cn

fun String.exclaim() = this + "!"
来源：http://kif.jqgufenzy.top

[T10] Kotlin：默认参数
来源：http://bii.ybcxt.top

fun greet(name: String = "World") = "Hi $name"
来源：http://yjb.smart0.xyz

[T11] Kotlin：协程
来源：http://cxp.9152youxi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://fcw.c1oappe.top

[T12] Kotlin：解构声明
来源：http://ciz.zdbjq.cn

val (a, b) = Pair(1, 2)
来源：http://ifi.xziqi.cn

[T13] Kotlin：只读 Map
来源：http://iuq.fehbvm.com

val m = mapOf("a" to 1)
来源：http://rnw.epnwcf.com

[T14] Kotlin：循环
来源：http://hqw.wangshuangyany.cn

for (i in 1..10) println(i)
来源：http://qjw.0kj1m.cn

[T15] Kotlin：接口
来源：http://zyo.ywan-chungtsiang.top

interface Shape { fun area(): Double }
来源：http://gmc.kuanghao11.cn

[T16] Swift：Hello World
来源：http://qoh.52xcode.cn

print("Hello")
来源：http://twh.c1oappe.top

[T17] Swift：变量与常量
来源：http://fpn.jianghu66.top

var a = 1;  let b = 2
来源：http://had.yvedp.cn

[T18] Swift：字符串插值
来源：http://iiq.aizwys.cn

"值: \(b)"
来源：http://vso.yonumen.top

[T19] Swift：可选绑定
来源：http://uib.quarkkingdee.top

if let n = opt { print(n) }
来源：http://tgf.shuidangran.top

[T20] Swift：数组操作
来源：http://qew.shanyushiyangtech.top

var a = [1, 2, 3];  a.append(4)
来源：http://dhp.xinyue.icu

[T21] Swift：遍历
来源：http://mgf.yuxming.cn

for x in a { print(x) }
来源：http://afe.zhoulong.xyz

[T22] Swift：字典
来源：http://irl.chenjidiqi.icu

var d = ["a": 1];  d["b"] = 2
来源：http://oge.uphjek.com

[T23] Swift：函数
来源：http://tvi.jiagoushi.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xkd.quarkkingdee.top

[T24] Swift：闭包
来源：http://xee.yangfankeji.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://vqf.daria6918.cn

[T25] Swift：结构体
来源：http://ryz.zhiwuduotai.top

struct P { var x: Int }
来源：http://dkj.ydjk.org.cn

[T26] Swift：类与重写
来源：http://tpa.jinqigufen.top

class A: Base { override func f() {} }
来源：http://tot.wangdashe.top

[T27] Swift：错误处理
来源：http://gkd.fengsongda.top

do { try f() } catch { print(error) }
来源：http://taw.ydjk.org.cn

[T28] Swift：枚举
来源：http://dwy.gaohongyu789.top

enum Color { case red, green }
来源：http://hjk.shzxlz.cn

[T29] Swift：guard 提前返回
来源：http://shu.zhaomingkeji.xyz

guard let x = opt else { return }
来源：http://fnm.zdbjq.cn

[T30] Swift：协议
来源：http://kzl.redwolf501.top

protocol Shape { func area() -> Double }
来源：http://iqp.sufxvd.cn

[T31] Lua：Hello World
来源：http://otv.yj20258.top

print("Hello")
来源：http://vhv.hammf.cn

[T32] Lua：局部变量
来源：http://yed.ybcxt.top

local a = 1
来源：http://rrs.meibo888.top

[T33] Lua：表（数组）
来源：http://cdk.iojbl.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://rkr.smart0.xyz

[T34] Lua：遍历表
来源：http://ntm.yfazqb.com

for i, v in ipairs(t) do print(i, v) end
来源：http://hxc.shzxlz.cn

[T35] Lua：字典表
来源：http://pfy.yj202588.top

local d = { a = 1 };  d.b = 2
来源：http://axz.hongshengwenyu.top

[T36] Lua：函数
来源：http://zug.xinyue.icu

function add(a, b) return a + b end
来源：http://msg.aizwys.cn

[T37] Lua：字符串拼接
来源：http://drf.shanyushiyangkeji.top

"a" .. "b"
来源：http://kjv.yangfankeji.com

[T38] Lua：条件
来源：http://yhr.sysykeji.top

if x > 0 then print("正") end
来源：http://sra.feifeiyinyue.top

[T39] Lua：模式匹配
来源：http://duk.gaohongyu789.top

string.find(s, "%d+")
来源：http://dzo.dashuyun.cn

[T40] Lua：元表
来源：http://ftc.epnwcf.com

setmetatable({}, { __index = base })
来源：http://umx.aizwys.cn

[T41] Perl：Hello World
来源：http://cvk.zhoulong.xyz

print "Hello\n";
来源：http://fvc.wangdashe.top

[T42] Perl：变量类型
来源：http://hvm.redwolf501.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ord.shzxlz.cn

[T43] Perl：字符串插值
来源：http://cns.hnqzz.top

"值: $a"
来源：http://efn.ydzc1.top

[T44] Perl：条件
来源：http://nlu.yueranfly.top

if ($a > 0) { print "正"; }
来源：http://xfl.yuxming.cn

[T45] Perl：数组遍历
来源：http://fid.dianchejie.cn

for my $x (@arr) { print $x; }
来源：http://oxk.c1oappe.top

[T46] Perl：哈希操作
来源：http://xvw.chenjidiqi.icu

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tua.yangfankeji.com

[T47] Perl：正则捕获
来源：http://xor.dashuyun.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://mdd.sjlbkw.cn

[T48] Perl：正则替换
来源：http://uhm.yueranfly.top

$s =~ s/old/new/g;
来源：http://tpf.fktsv.cn

[T49] Perl：函数
来源：http://txm.cashguo.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://iio.daria6918.cn

[T50] Perl：逐行读文件
来源：http://egn.redwolf501.top

open my $fh, "<", "a.txt" or die $!;
来源：http://nds.chenjidiqi.icu

while (my $line = <$fh>) { print $line; }
来源：http://pqb.redwolf501.top

[T51] Scala：Hello World
来源：http://mqj.aizwys.cn

println("Hello")
来源：http://nch.havefunace.top

[T52] Scala：变量
来源：http://ilb.yangfankeji.com

val a = 1;  var b = 2
来源：http://cmw.kuanghao11.cn

[T53] Scala：字符串插值
来源：http://jtk.feifeiyinyue.top

s"值: $b"
来源：http://bsk.xuetiantiany.cn

[T54] Scala：集合映射
来源：http://qhl.bbcook.cn

List(1, 2, 3).map(_ * 2)
来源：http://vkt.xingfuxueyuan.xyz

[T55] Scala：集合过滤
来源：http://gbd.ydzc1.top

List(1, 2, 3).filter(_ > 1)
来源：http://egq.yfazqb.com

[T56] Scala：样例类
来源：http://xdz.ydzc1.top

case class User(name: String, age: Int)
来源：http://usk.yanxiufei.cn

[T57] Scala：模式匹配
来源：http://hyh.zdbjq.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://odi.nwbrower.top

[T58] Scala：函数定义
来源：http://nzy.gotoacloud.top

def add(a: Int, b: Int): Int = a + b
来源：http://otk.fktsv.cn

[T59] Scala：循环
来源：http://dal.kuanghao11.cn

for (i <- 1 to 10) println(i)
来源：http://pzn.pycfn.com

[T60] Scala：折叠
来源：http://cav.ctjpmb.com

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rsb.sxryk.cn

================================================================================
来源：http://lpy.316326.xyz

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ywf.ehwqpu.com

================================================================================
来源：http://kng.fktsv.cn

[U01] Py：创建虚拟环境
来源：http://qmf.dashuyun.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ioa.ydzc1.top

[U02] Py：导出 / 安装依赖
来源：http://ehu.jqgfzy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pvs.sweek.top

[U03] Py：加载 .env 配置
来源：http://sxs.cqqwz.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://qpi.jinqigufen.top

[U04] Py：变量调试打印
来源：http://khx.zhixingplan.top

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ghp.jianghu66.top


<!-- 参考信息 -->