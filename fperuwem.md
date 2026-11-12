代发 wailian999

df -h;  du -sh *
来源：http://jmd.sweek.top

[R62] 找最占空间的文件
来源：http://xzu.sweek.top

du -ah . | sort -rh | head -10
来源：http://orw.hysaishi.cn

[R63] 内存与进程
来源：http://jkm.yanxiufei.cn

free -h;  ps aux | grep nginx
来源：http://ruf.yvedp.cn

[R64] 结束进程
来源：http://qak.yj20258888.top

kill -9 $(pgrep -f app.py)
来源：http://eba.ydzc1.top

[R65] 查看端口占用
来源：http://mkz.jiagoushi.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kqi.pycfn.com

[R66] 定时任务
来源：http://bpl.jqgufenzy.top

crontab -e;  crontab -l
来源：http://ujm.jianghu66.top

[R67] 生成随机十六进制串
来源：http://oul.guowangkeji.top

openssl rand -hex 16
来源：http://nqh.shuidangran.top

[R68] 计算文件校验值
来源：http://lmk.guowangkeji.top

sha256sum a.txt;  md5sum a.txt
来源：http://htp.dashuyun.cn

[R69] 生成随机密码
来源：http://qse.hesvh.cn

head -c 16 /dev/urandom | base64
来源：http://kky.hysaishi.cn

[R70] 时间戳与互转
来源：http://mgt.jinghuilouyu.cn

date +%s;  date -d @1700000000
来源：http://nyi.yonumen.top

[R71] 日期格式化
来源：http://rmn.guannengcc.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://yvz.xylfe.cn

[R72] 等待端口就绪
来源：http://jxn.snrcjt.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cta.ywan-chungtsiang.top

[R73] 分割大日志
来源：http://mbt.haohaochexian.top

split -l 1000 big.log part_
来源：http://hck.ydzc1.top

[R74] 批量重命名
来源：http://cno.epnwcf.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gnt.xziqi.cn

[R75] 导出环境变量
来源：http://xwg.andypj.xyz

export PATH="$HOME/bin:$PATH"
来源：http://zja.shanyushiyangkeji.top

[R76] 使用临时文件
来源：http://kdn.sxryk.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://uzr.jianghu66.top

[R77] 读取用户输入
来源：http://wkb.gogol.net.cn

read -rp "请输入: " ans
来源：http://yow.hysaishi.cn

[R78] 交互式菜单
来源：http://vlm.wangshuangyany.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://huf.shzxlz.cn

[R79] 解析命令行选项
来源：http://tyw.havefunace.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fep.yanxiufei.cn

[R80] 查看脚本执行耗时
来源：http://bar.hnqzz.top

time ./run.sh
来源：http://qax.sweek.top

================================================================================
来源：http://tzu.ybcxt.top

S. C / C++ 专题
来源：http://xrn.xinyue.icu

================================================================================
来源：http://slf.zdqjudy.top

[S01] C：Hello World
来源：http://pai.jyoumei.cn

#include <stdio.h>
来源：http://btr.ctjpmb.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://flk.jyoumei.cn

[S02] C：变量与格式化输出
来源：http://aiw.guowangkeji.top

int a = 10; printf("%d\n", a);
来源：http://dwv.guowangkeji.top

[S03] C：读入整数
来源：http://rch.ydzc1.top

int x; scanf("%d", &x);
来源：http://kif.wangshuangyany.cn

[S04] C：字符串复制
来源：http://pzn.zhixingplan.top

char dst[32]; strcpy(dst, "hi");
来源：http://yoo.52xcode.cn

[S05] C：字符串长度
来源：http://lhy.cucudq.cn

strlen(s)
来源：http://esr.yuxming.cn

[S06] C：字符串比较
来源：http://fxf.svipenyu.cn

strcmp(a, b) == 0
来源：http://erv.yueranfly.top

[S07] C：数组遍历求和
来源：http://cit.cashguo.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kaq.zhiwuduotai.top

[S08] C：动态内存分配与释放
来源：http://aho.fehbvm.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://trk.yueranfly.top

[S09] C：结构体定义与初始化
来源：http://gvm.52xcode.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pfr.zhoulong.xyz

[S10] C：指针与解引用
来源：http://mrj.xingfuxueyuan.xyz

int *p = &a;  *p = 5;
来源：http://thi.bbcook.cn

[S11] C：逐行读文件
来源：http://mpn.sufxvd.cn

FILE *f = fopen("a.txt", "r");
来源：http://joa.ctjpmb.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://nrn.zhijiandao.cn

fclose(f);
来源：http://rjl.iojbl.cn

[S12] C：写文件
来源：http://ymm.fehbvm.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fyc.ydzc1.top

[S13] C：宏定义
来源：http://lon.zdbjq.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xed.zhongyouzk.top

[S14] C：枚举
来源：http://hmi.dianchejie.cn

enum Color { RED, GREEN, BLUE };
来源：http://dzw.zhongyouzk.top

[S15] C：类型转换
来源：http://ugv.kuanghao11.cn

(double) a / b
来源：http://xnp.ybcxt.top

[S16] C：位操作置位
来源：http://bnq.yonumen.top

x |= (1 << 3);
来源：http://aqa.xziqi.cn

[S17] C：安全拼接字符串
来源：http://nmp.haohaochexian.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://iot.pycfn.com

[S18] C：命令行参数
来源：http://rrm.fengsongda.top

int main(int argc, char **argv)
来源：http://mel.hnqzz.top

[S19] C：快速排序
来源：http://brw.jinyuanbaomall.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xre.jinqigfzy.top

[S20] C：二分查找
来源：http://num.xylfe.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://okr.jlsjyb.cn

[S21] C：字符类别判断
来源：http://fqg.yuanzhike.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nzd.hfpthk.cn

[S22] C：字符串转数字
来源：http://qth.xinyue.icu

atoi("42");  strtod("3.14", NULL);
来源：http://hdt.gzhubu.top

[S23] C：随机数
来源：http://cdx.daxiang520.top

srand(time(NULL));  int r = rand() % 100;
来源：http://fav.yongpay.top

[S24] C：获取本地时间
来源：http://zjw.pengpengdd.cyou

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vng.mhx1999.top

[S25] C：内存拷贝
来源：http://egk.shanyushiyangkeji.top

memcpy(dst, src, n);
来源：http://hur.guannengcc.top

[S26] C：内存清零
来源：http://fyz.guowangkeji.top

memset(a, 0, sizeof a);
来源：http://jmg.chenzaomai.com

[S27] C：定义常量
来源：http://gzh.kuanghao11.cn

const double PI = 3.14159;
来源：http://kde.redwolf501.top

[S28] C：静态变量
来源：http://zze.zdbjq.cn

static int counter = 0;
来源：http://csw.birdmap.top

[S29] C：变参函数
来源：http://ogv.sysykeji.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rrz.316326.xyz

[S30] C：头文件保护
来源：http://fyd.yuanzhike.top

#ifndef X_H
来源：http://yjf.yueranfly.top

#define X_H
来源：http://xvg.redwolf501.top

#endif
来源：http://ple.dashuyun.cn

[S31] C++：Hello World
来源：http://lru.gotoacloud.top

#include <iostream>
来源：http://flo.gotoacloud.top

int main() { std::cout << "Hello\n"; }
来源：http://lgn.daria6918.cn

[S32] C++：字符串
来源：http://ola.pycfn.com

std::string s = "hi";  s += "!";
来源：http://lnz.hywenlv.cn

[S33] C++：vector 增删
来源：http://vas.cqqwz.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ajn.uphjek.com

[S34] C++：遍历 vector
来源：http://ptc.zhoulong.xyz

for (auto &x : v) { std::cout << x; }
来源：http://jpd.zhongyouzk.top

[S35] C++：map
来源：http://uzx.hammf.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nzj.tian-w.cn

[S36] C++：unordered_map
来源：http://vne.zhaomingkeji.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nre.hammf.cn

[S37] C++：set
来源：http://znc.yueranfly.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vxh.shanyushiyangtech.top

[S38] C++：排序
来源：http://fxl.cdnleiting.top

std::sort(v.begin(), v.end());
来源：http://kmr.iojbl.cn

[S39] C++：自定义比较器排序
来源：http://rnt.hesvh.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yhr.sjlbkw.cn

[S40] C++：查找元素
来源：http://ogt.fehbvm.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pjq.haohaochexian.top

[S41] C++：类与构造函数
来源：http://vpu.gzhubu.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xtq.zhaomingkeji.xyz

[S42] C++：继承与虚函数
来源：http://gei.jyoumei.cn

class B : public Base { public: void f() override {} };
来源：http://nlj.fengsongda.top

[S43] C++：智能指针
来源：http://ddy.dashuyun.cn

auto p = std::make_unique<int>(5);
来源：http://ghh.zhiwuduotai.top

[S44] C++：引用传参
来源：http://nza.guowangkeji.top

void inc(int &x) { ++x; }
来源：http://pvj.nwbrower.top

[S45] C++：lambda
来源：http://pwp.yfazqb.com

auto add = [](int a, int b) { return a + b; };
来源：http://skq.hesvh.cn

[S46] C++：函数模板
来源：http://jxw.yuxming.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ymf.svipenyu.cn

[S47] C++：结构化绑定遍历
来源：http://jbf.xylfe.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kuc.mhx1999.top

[S48] C++：逐行读文件
来源：http://hdi.yueranfly.top

std::ifstream in("a.txt");  std::string line;
来源：http://qff.havefunace.top

while (std::getline(in, line)) { }
来源：http://szd.sysykeji.top

[S49] C++：写文件
来源：http://eyv.hysaishi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ckn.yj20258888.top

[S50] C++：格式化数字
来源：http://wvr.birdmap.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://akz.jqgfzy.top

[S51] C++：显式类型转换
来源：http://nqr.redwolf501.top

static_cast<double>(a) / b
来源：http://ran.dianchejie.cn

[S52] C++：const 与 noexcept
来源：http://tgd.ivvv.top

int size() const noexcept { return n_; }
来源：http://kns.52xcode.cn

[S53] C++：移动语义
来源：http://yzk.jinqigfzy.top

std::vector<int> w = std::move(v);
来源：http://itf.tian-w.cn

[S54] C++：异常处理
来源：http://ptu.wangdashe.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://odq.ppjwa.cn

[S55] C++：结构化绑定
来源：http://rxt.epnwcf.com

auto [a, b] = std::make_pair(1, 2);
来源：http://cny.xziqi.cn

[S56] C++：optional
来源：http://vho.aibaodan.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bcs.zhaomingkeji.xyz

[S57] C++：编译期常量
来源：http://wka.yuanzhike.top

constexpr int N = 10;
来源：http://jli.pycfn.com

[S58] C++：命名空间
来源：http://vpr.hammf.cn

namespace ns { int f() { return 1; } }
来源：http://ixw.fehbvm.com

[S59] C++：静态断言
来源：http://dok.yanxiufei.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gma.vqdsnc.cn

[S60] C++：遍历并删除元素
来源：http://yhk.pengpengdd.cyou

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kgj.daria6918.cn

================================================================================
来源：http://slm.hongshengwenyu.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lvh.bjfxy.top

================================================================================
来源：http://sae.hongshengwenyu.top

[T01] Kotlin：Hello World
来源：http://ula.pengpengdd.cyou

println("Hello")
来源：http://aae.xziqi.cn

[T02] Kotlin：变量
来源：http://gcm.jianghu66.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pew.cdnleiting.top

[T03] Kotlin：字符串模板
来源：http://azj.pengpengdd.cyou

"值: $b"
来源：http://ysg.iojbl.cn

[T04] Kotlin：空安全
来源：http://vbl.haohaochexian.top

val n: String? = null;  n?.length
来源：http://nze.hysaishi.cn

[T05] Kotlin：when 表达式
来源：http://ybz.pycfn.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ser.jyoumei.cn

[T06] Kotlin：集合映射
来源：http://ldm.fktsv.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://wpl.zhiwuduotai.top

[T07] Kotlin：集合过滤
来源：http://zat.zhongyouzk.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://bgm.snrcjt.cn

[T08] Kotlin：数据类
来源：http://rtr.smart0.xyz

data class User(val name: String, val age: Int)
来源：http://umi.dashuyun.cn

[T09] Kotlin：扩展函数
来源：http://bqr.pengpengdd.cyou

fun String.exclaim() = this + "!"
来源：http://kws.hesvh.cn

[T10] Kotlin：默认参数
来源：http://mdw.zhijiandao.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tau.sxryk.cn

[T11] Kotlin：协程
来源：http://dtg.yj20258.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ndu.guannengcc.top

[T12] Kotlin：解构声明
来源：http://tzc.yuxming.cn

val (a, b) = Pair(1, 2)
来源：http://ngk.smart0.xyz

[T13] Kotlin：只读 Map
来源：http://eyx.ivvv.top

val m = mapOf("a" to 1)
来源：http://ixr.ydjk.org.cn

[T14] Kotlin：循环
来源：http://ilz.wangdashe.top

for (i in 1..10) println(i)
来源：http://gcy.jqgfzy.top

[T15] Kotlin：接口
来源：http://bmk.jinyuanbaomall.cn

interface Shape { fun area(): Double }
来源：http://wzq.fengsongda.top

[T16] Swift：Hello World
来源：http://tgu.jiagoushi.top

print("Hello")
来源：http://rqo.mhx1999.top

[T17] Swift：变量与常量
来源：http://prt.xziqi.cn

var a = 1;  let b = 2
来源：http://ene.aibaodan.cn

[T18] Swift：字符串插值
来源：http://avn.zhiwuduotai.top

"值: \(b)"
来源：http://nis.xingfuxueyuan.xyz

[T19] Swift：可选绑定
来源：http://das.quarkkingdee.top

if let n = opt { print(n) }
来源：http://wmi.wangdashe.top

[T20] Swift：数组操作
来源：http://fdr.9152youxi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://efn.daria6918.cn

[T21] Swift：遍历
来源：http://eyy.shanyushiyangkeji.top

for x in a { print(x) }
来源：http://amo.xylfe.cn

[T22] Swift：字典
来源：http://vtf.chenjidiqi.icu

var d = ["a": 1];  d["b"] = 2
来源：http://wvc.gotoacloud.top

[T23] Swift：函数
来源：http://qbf.fktsv.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xeq.haohaochexian.top

[T24] Swift：闭包
来源：http://now.hnxiangtu.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://cfk.birdmap.top

[T25] Swift：结构体
来源：http://rkl.wangshuangyany.cn

struct P { var x: Int }
来源：http://tmc.sxryk.cn

[T26] Swift：类与重写
来源：http://ofa.meibo888.top

class A: Base { override func f() {} }
来源：http://atq.feifeiyinyue.top

[T27] Swift：错误处理
来源：http://ygi.pengpengdd.cyou

do { try f() } catch { print(error) }
来源：http://iou.hcnkem.com

[T28] Swift：枚举
来源：http://aue.shanyushiyangkeji.top

enum Color { case red, green }
来源：http://pqf.bjfxy.top

[T29] Swift：guard 提前返回
来源：http://pwj.sysykeji.top

guard let x = opt else { return }
来源：http://ypq.redwolf501.top

[T30] Swift：协议
来源：http://gwt.fengsongda.top

protocol Shape { func area() -> Double }
来源：http://qrp.zycfv.cn

[T31] Lua：Hello World
来源：http://bzt.yuxming.cn

print("Hello")
来源：http://kpv.shanyushiyangtech.top

[T32] Lua：局部变量
来源：http://hvp.iojbl.cn

local a = 1
来源：http://prs.ydzc1.top

[T33] Lua：表（数组）
来源：http://fjm.dashuyun.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://voe.chenlongwang.top

[T34] Lua：遍历表
来源：http://lgi.wangshuangyany.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://evn.hywenlv.cn

[T35] Lua：字典表
来源：http://ycw.havefunace.top

local d = { a = 1 };  d.b = 2
来源：http://vfu.hnqzz.top

[T36] Lua：函数
来源：http://xgl.iojbl.cn

function add(a, b) return a + b end
来源：http://zro.hysaishi.cn

[T37] Lua：字符串拼接
来源：http://ehw.shanyushiyangtech.top

"a" .. "b"
来源：http://qgk.zhoulong.xyz

[T38] Lua：条件
来源：http://xqt.havefunace.top

if x > 0 then print("正") end
来源：http://gsq.sweek.top

[T39] Lua：模式匹配
来源：http://gkq.jlsjyb.cn

string.find(s, "%d+")
来源：http://hpi.bbcook.cn

[T40] Lua：元表
来源：http://trt.tianlin.xyz

setmetatable({}, { __index = base })
来源：http://exw.yj20258.top

[T41] Perl：Hello World
来源：http://wfv.yj20258888.top

print "Hello\n";
来源：http://bfk.cheryme.top

[T42] Perl：变量类型
来源：http://xwd.jinghuilouyu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://brj.wangdashe.top

[T43] Perl：字符串插值
来源：http://jcc.shangyingyoupin.top

"值: $a"
来源：http://odw.fanxiaobao.xyz

[T44] Perl：条件
来源：http://lgv.cqqwz.cn

if ($a > 0) { print "正"; }
来源：http://shl.fengsongda.top

[T45] Perl：数组遍历
来源：http://xvt.ydjk.org.cn

for my $x (@arr) { print $x; }
来源：http://nsc.zhiwuduotai.top

[T46] Perl：哈希操作
来源：http://uzt.snrcjt.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://luc.pycfn.com

[T47] Perl：正则捕获
来源：http://jxz.fzhhl.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://nfu.feifeiyinyue.top

[T48] Perl：正则替换
来源：http://xwz.ctjpmb.com

$s =~ s/old/new/g;
来源：http://fjk.sweek.top

[T49] Perl：函数
来源：http://zzp.xuetiantiany.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://cgq.feifeiyinyue.top

[T50] Perl：逐行读文件
来源：http://cfv.jlsjyb.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://hht.ppjwa.cn

while (my $line = <$fh>) { print $line; }
来源：http://ezb.meibo888.top

[T51] Scala：Hello World
来源：http://bxa.sufxvd.cn

println("Hello")
来源：http://ozk.ivvv.top

[T52] Scala：变量
来源：http://pia.jqgfzy.top

val a = 1;  var b = 2
来源：http://ipz.gzhubu.top

[T53] Scala：字符串插值
来源：http://rfi.bbcook.cn

s"值: $b"
来源：http://gby.dashuyun.cn

[T54] Scala：集合映射
来源：http://maj.birdmap.top

List(1, 2, 3).map(_ * 2)
来源：http://uxz.quarkkingdee.top

[T55] Scala：集合过滤
来源：http://ufm.dianchejie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://fhg.cheryme.top

[T56] Scala：样例类
来源：http://kzx.ivvv.top

case class User(name: String, age: Int)
来源：http://lyg.hcnkem.com

[T57] Scala：模式匹配
来源：http://kzf.chenjidiqi.icu

x match { case 1 => "一"; case _ => "其他" }
来源：http://jte.zhijiandao.cn

[T58] Scala：函数定义
来源：http://ocl.sjlbkw.cn

def add(a: Int, b: Int): Int = a + b
来源：http://lrk.zdbjq.cn

[T59] Scala：循环
来源：http://txh.yuxming.cn

for (i <- 1 to 10) println(i)
来源：http://yar.zhixingplan.top

[T60] Scala：折叠
来源：http://tsb.jlsjyb.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dll.havefunace.top

================================================================================
来源：http://qyj.chenlongwang.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hhj.jinghuilouyu.cn

================================================================================
来源：http://hrv.quarkkingdee.top

[U01] Py：创建虚拟环境
来源：http://ilz.shangyingyoupin.top

python -m venv .venv && source .venv/bin/activate
来源：http://gau.yvedp.cn

[U02] Py：导出 / 安装依赖
来源：http://kxu.fanxiaobao.xyz

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ubw.zhiwuduotai.top


<!-- 参考信息 -->