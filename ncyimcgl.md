代发 wailian999

df -h;  du -sh *
来源：http://jfl.zhixingplan.top

[R62] 找最占空间的文件
来源：http://cfu.dianchejie.cn

du -ah . | sort -rh | head -10
来源：http://cai.yfazqb.com

[R63] 内存与进程
来源：http://qqh.tianlin.xyz

free -h;  ps aux | grep nginx
来源：http://afq.cucudq.cn

[R64] 结束进程
来源：http://vcx.yj20258.top

kill -9 $(pgrep -f app.py)
来源：http://rkm.cheryme.top

[R65] 查看端口占用
来源：http://wat.zhaomingkeji.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sph.shzxlz.cn

[R66] 定时任务
来源：http://wnm.fehbvm.com

crontab -e;  crontab -l
来源：http://zoz.sufxvd.cn

[R67] 生成随机十六进制串
来源：http://hpx.zhaomingkeji.xyz

openssl rand -hex 16
来源：http://sik.snrcjt.cn

[R68] 计算文件校验值
来源：http://pqa.fktsv.cn

sha256sum a.txt;  md5sum a.txt
来源：http://bqf.dashuyun.cn

[R69] 生成随机密码
来源：http://gxa.jinqigfzy.top

head -c 16 /dev/urandom | base64
来源：http://kme.zdbjq.cn

[R70] 时间戳与互转
来源：http://fvq.sxryk.cn

date +%s;  date -d @1700000000
来源：http://atz.tianlin.xyz

[R71] 日期格式化
来源：http://ssz.jinghuilouyu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qfo.52xcode.cn

[R72] 等待端口就绪
来源：http://hvu.hywenlv.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://aua.fzhhl.top

[R73] 分割大日志
来源：http://qco.hnxiangtu.top

split -l 1000 big.log part_
来源：http://rqi.bjfxy.top

[R74] 批量重命名
来源：http://vco.jinqigfzy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ltp.kuanghao11.cn

[R75] 导出环境变量
来源：http://drm.redwolf501.top

export PATH="$HOME/bin:$PATH"
来源：http://yog.vehdjk.com

[R76] 使用临时文件
来源：http://fzn.sxryk.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kxm.epnwcf.com

[R77] 读取用户输入
来源：http://yvf.tian-w.cn

read -rp "请输入: " ans
来源：http://qve.yueranfly.top

[R78] 交互式菜单
来源：http://hjz.gotoacloud.top

select opt in a b c; do echo "$opt"; break; done
来源：http://qum.fehbvm.com

[R79] 解析命令行选项
来源：http://hbd.zhengqikj.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xqh.xylfe.cn

[R80] 查看脚本执行耗时
来源：http://yrq.nwbrower.top

time ./run.sh
来源：http://gcy.feifeiyinyue.top

================================================================================
来源：http://kni.snrcjt.cn

S. C / C++ 专题
来源：http://hoj.havefunace.top

================================================================================
来源：http://pae.tarul.cn

[S01] C：Hello World
来源：http://tnd.guannengcc.top

#include <stdio.h>
来源：http://ljn.xuetiantiany.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://omx.zycfv.cn

[S02] C：变量与格式化输出
来源：http://oae.aizwys.cn

int a = 10; printf("%d\n", a);
来源：http://klb.aizwys.cn

[S03] C：读入整数
来源：http://cyz.guowangkeji.top

int x; scanf("%d", &x);
来源：http://gbr.feifeiyinyue.top

[S04] C：字符串复制
来源：http://wtt.daxiang520.top

char dst[32]; strcpy(dst, "hi");
来源：http://hhj.jinqigfzy.top

[S05] C：字符串长度
来源：http://abr.hongshengwenyu.top

strlen(s)
来源：http://qpx.jianghu66.top

[S06] C：字符串比较
来源：http://fmr.gaohongyu789.top

strcmp(a, b) == 0
来源：http://jdu.fanxiaobao.xyz

[S07] C：数组遍历求和
来源：http://ynm.zdbjq.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kph.jqgufenzy.top

[S08] C：动态内存分配与释放
来源：http://kgs.aibaodan.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://iwy.cheryme.top

[S09] C：结构体定义与初始化
来源：http://pjk.chenjidiqi.icu

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rrd.guannengcc.top

[S10] C：指针与解引用
来源：http://vms.nwbrower.top

int *p = &a;  *p = 5;
来源：http://ztw.xziqi.cn

[S11] C：逐行读文件
来源：http://ubb.gzhubu.top

FILE *f = fopen("a.txt", "r");
来源：http://fgq.jinghuilouyu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://bdo.yj202588.top

fclose(f);
来源：http://cxm.zhengqikj.top

[S12] C：写文件
来源：http://jia.fanxiaobao.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wuo.ydjk.org.cn

[S13] C：宏定义
来源：http://zav.gotoacloud.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vpw.jqgufenzy.top

[S14] C：枚举
来源：http://kcn.xylfe.cn

enum Color { RED, GREEN, BLUE };
来源：http://lat.hesvh.cn

[S15] C：类型转换
来源：http://mrm.gzhubu.top

(double) a / b
来源：http://hgg.fengsongda.top

[S16] C：位操作置位
来源：http://ums.jianghu66.top

x |= (1 << 3);
来源：http://urq.tianlin.xyz

[S17] C：安全拼接字符串
来源：http://evc.epnwcf.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hnd.zhengqikj.top

[S18] C：命令行参数
来源：http://irw.zhongyouzk.top

int main(int argc, char **argv)
来源：http://fzo.mhx1999.top

[S19] C：快速排序
来源：http://wei.zhengqikj.top

qsort(a, n, sizeof(int), cmp);
来源：http://yen.uphjek.com

[S20] C：二分查找
来源：http://bap.iojbl.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gry.redwolf501.top

[S21] C：字符类别判断
来源：http://fwg.haohaochexian.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qdz.cheryme.top

[S22] C：字符串转数字
来源：http://qdb.tanke756.top

atoi("42");  strtod("3.14", NULL);
来源：http://nho.tarul.cn

[S23] C：随机数
来源：http://cbr.jlsjyb.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ftu.hongshengwenyu.top

[S24] C：获取本地时间
来源：http://bhi.0kj1m.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qpv.uphjek.com

[S25] C：内存拷贝
来源：http://hsi.havefunace.top

memcpy(dst, src, n);
来源：http://iiy.gzhubu.top

[S26] C：内存清零
来源：http://ear.xuetiantiany.cn

memset(a, 0, sizeof a);
来源：http://tnc.uphjek.com

[S27] C：定义常量
来源：http://mbf.daxiang520.top

const double PI = 3.14159;
来源：http://qyp.gogol.net.cn

[S28] C：静态变量
来源：http://isg.xinyue.icu

static int counter = 0;
来源：http://ibj.quarkkingdee.top

[S29] C：变参函数
来源：http://hqy.yueranfly.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://iyn.hfpthk.cn

[S30] C：头文件保护
来源：http://dlk.9152youxi.cn

#ifndef X_H
来源：http://bqh.jinqigufen.top

#define X_H
来源：http://zyl.hesvh.cn

#endif
来源：http://tkg.xinyue.icu

[S31] C++：Hello World
来源：http://mvu.aibaodan.cn

#include <iostream>
来源：http://daf.gogol.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://kqe.yj20258888.top

[S32] C++：字符串
来源：http://cdz.vehdjk.com

std::string s = "hi";  s += "!";
来源：http://pqk.shangyingyoupin.top

[S33] C++：vector 增删
来源：http://wra.9152youxi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ure.zdbjq.cn

[S34] C++：遍历 vector
来源：http://wfz.gaohongyu789.top

for (auto &x : v) { std::cout << x; }
来源：http://kng.zhijiandao.cn

[S35] C++：map
来源：http://tos.hywenlv.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fht.yuxming.cn

[S36] C++：unordered_map
来源：http://gyy.yuanzhike.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pwp.hnqzz.top

[S37] C++：set
来源：http://hql.xylfe.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fqq.tarul.cn

[S38] C++：排序
来源：http://gfy.shzxlz.cn

std::sort(v.begin(), v.end());
来源：http://uhs.fktsv.cn

[S39] C++：自定义比较器排序
来源：http://zgu.redwolf501.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gvs.tianlin.xyz

[S40] C++：查找元素
来源：http://mfw.quarkkingdee.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kqu.epnwcf.com

[S41] C++：类与构造函数
来源：http://euy.smart0.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mjd.xingfuxueyuan.xyz

[S42] C++：继承与虚函数
来源：http://voh.hnxiangtu.top

class B : public Base { public: void f() override {} };
来源：http://frp.yj20258888.top

[S43] C++：智能指针
来源：http://zwk.aizwys.cn

auto p = std::make_unique<int>(5);
来源：http://vqc.vehdjk.com

[S44] C++：引用传参
来源：http://uyn.bbcook.cn

void inc(int &x) { ++x; }
来源：http://woy.hnxiangtu.top

[S45] C++：lambda
来源：http://aso.wangdashe.top

auto add = [](int a, int b) { return a + b; };
来源：http://wnq.sweek.top

[S46] C++：函数模板
来源：http://xot.ydzc1.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xxb.epnwcf.com

[S47] C++：结构化绑定遍历
来源：http://scx.feifeiyinyue.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wjk.guowangkeji.top

[S48] C++：逐行读文件
来源：http://sgp.nanxuanxn.top

std::ifstream in("a.txt");  std::string line;
来源：http://vlu.aizwys.cn

while (std::getline(in, line)) { }
来源：http://ftr.sxryk.cn

[S49] C++：写文件
来源：http://cbp.yuanzhike.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tev.xuanzx.com

[S50] C++：格式化数字
来源：http://kzc.zdbjq.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://unf.hysaishi.cn

[S51] C++：显式类型转换
来源：http://uqg.ybcxt.top

static_cast<double>(a) / b
来源：http://ngb.cdnleiting.top

[S52] C++：const 与 noexcept
来源：http://bhd.yongpay.top

int size() const noexcept { return n_; }
来源：http://ziu.jyoumei.cn

[S53] C++：移动语义
来源：http://kya.pengpengdd.cyou

std::vector<int> w = std::move(v);
来源：http://uji.dashuyun.cn

[S54] C++：异常处理
来源：http://jtk.jinqigfzy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://drg.fanxiaobao.xyz

[S55] C++：结构化绑定
来源：http://uqr.sufxvd.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://kaz.fengsongda.top

[S56] C++：optional
来源：http://ixo.xziqi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://juf.shuidangran.top

[S57] C++：编译期常量
来源：http://rrb.zhiwuduotai.top

constexpr int N = 10;
来源：http://bun.zdbjq.cn

[S58] C++：命名空间
来源：http://pna.yonumen.top

namespace ns { int f() { return 1; } }
来源：http://qjv.sxryk.cn

[S59] C++：静态断言
来源：http://lgp.fengsongda.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://muo.zhongyouzk.top

[S60] C++：遍历并删除元素
来源：http://gnd.quarkkingdee.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vsm.ybcxt.top

================================================================================
来源：http://yow.316326.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ryq.dashuyun.cn

================================================================================
来源：http://dlj.yj20258.top

[T01] Kotlin：Hello World
来源：http://uap.zhixingplan.top

println("Hello")
来源：http://ldq.shanyushiyangtech.top

[T02] Kotlin：变量
来源：http://cqy.uphjek.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zuq.shanyushiyangkeji.top

[T03] Kotlin：字符串模板
来源：http://mja.yangfankeji.com

"值: $b"
来源：http://ffr.cashguo.top

[T04] Kotlin：空安全
来源：http://vat.hcnkem.com

val n: String? = null;  n?.length
来源：http://erz.zhijiandao.cn

[T05] Kotlin：when 表达式
来源：http://bsk.ppjwa.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wrp.redwolf501.top

[T06] Kotlin：集合映射
来源：http://acy.fehbvm.com

listOf(1, 2, 3).map { it * 2 }
来源：http://frb.yuxming.cn

[T07] Kotlin：集合过滤
来源：http://kin.zycfv.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://zyu.zhijiandao.cn

[T08] Kotlin：数据类
来源：http://mwk.dianchejie.cn

data class User(val name: String, val age: Int)
来源：http://hzz.sysykeji.top

[T09] Kotlin：扩展函数
来源：http://ocu.wangshuangyany.cn

fun String.exclaim() = this + "!"
来源：http://nig.cucudq.cn

[T10] Kotlin：默认参数
来源：http://omw.shanyushiyangtech.top

fun greet(name: String = "World") = "Hi $name"
来源：http://nql.vehdjk.com

[T11] Kotlin：协程
来源：http://mnn.chenzaomai.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://ijf.hfpthk.cn

[T12] Kotlin：解构声明
来源：http://mjk.shuidangran.top

val (a, b) = Pair(1, 2)
来源：http://wzs.jiagoushi.top

[T13] Kotlin：只读 Map
来源：http://wiy.pycfn.com

val m = mapOf("a" to 1)
来源：http://ijb.tanke756.top

[T14] Kotlin：循环
来源：http://rta.ehwqpu.com

for (i in 1..10) println(i)
来源：http://our.hongshengwenyu.top

[T15] Kotlin：接口
来源：http://yhv.hywenlv.cn

interface Shape { fun area(): Double }
来源：http://tbc.9152youxi.cn

[T16] Swift：Hello World
来源：http://kbr.feifeiyinyue.top

print("Hello")
来源：http://ity.dianchejie.cn

[T17] Swift：变量与常量
来源：http://bbd.ydjk.org.cn

var a = 1;  let b = 2
来源：http://qgt.c1oappe.top

[T18] Swift：字符串插值
来源：http://uer.sweek.top

"值: \(b)"
来源：http://xmh.zhiwuduotai.top

[T19] Swift：可选绑定
来源：http://ifv.hammf.cn

if let n = opt { print(n) }
来源：http://ssv.shuidangran.top

[T20] Swift：数组操作
来源：http://oxc.c1oappe.top

var a = [1, 2, 3];  a.append(4)
来源：http://ehg.fengsongda.top

[T21] Swift：遍历
来源：http://pbf.yj20258.top

for x in a { print(x) }
来源：http://dix.mhx1999.top

[T22] Swift：字典
来源：http://wyn.smart0.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://hiv.yanxiufei.cn

[T23] Swift：函数
来源：http://ftp.kuanghao11.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://iop.tianlin.xyz

[T24] Swift：闭包
来源：http://pjd.yvedp.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ynm.yj20258888.top

[T25] Swift：结构体
来源：http://hng.ydjk.org.cn

struct P { var x: Int }
来源：http://zno.gaohongyu789.top

[T26] Swift：类与重写
来源：http://aay.bbcook.cn

class A: Base { override func f() {} }
来源：http://gza.vqdsnc.cn

[T27] Swift：错误处理
来源：http://fss.hnqzz.top

do { try f() } catch { print(error) }
来源：http://hlp.iojbl.cn

[T28] Swift：枚举
来源：http://ohr.zhaomingkeji.xyz

enum Color { case red, green }
来源：http://ssf.zhaomingkeji.xyz

[T29] Swift：guard 提前返回
来源：http://wff.shangyingyoupin.top

guard let x = opt else { return }
来源：http://iiv.ppjwa.cn

[T30] Swift：协议
来源：http://tgy.ppjwa.cn

protocol Shape { func area() -> Double }
来源：http://lnu.yj20258888.top

[T31] Lua：Hello World
来源：http://ivc.xylfe.cn

print("Hello")
来源：http://pgk.svipenyu.cn

[T32] Lua：局部变量
来源：http://mjy.tianlin.xyz

local a = 1
来源：http://jta.ehwqpu.com

[T33] Lua：表（数组）
来源：http://xwd.ydjk.org.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://eno.ppjwa.cn

[T34] Lua：遍历表
来源：http://kdf.hcnkem.com

for i, v in ipairs(t) do print(i, v) end
来源：http://rzv.0kj1m.cn

[T35] Lua：字典表
来源：http://ltg.ydjk.org.cn

local d = { a = 1 };  d.b = 2
来源：http://tjd.hcnkem.com

[T36] Lua：函数
来源：http://ueb.fehbvm.com

function add(a, b) return a + b end
来源：http://iym.xinyue.icu

[T37] Lua：字符串拼接
来源：http://jwn.yanxiufei.cn

"a" .. "b"
来源：http://pfi.yj20258888.top

[T38] Lua：条件
来源：http://dyx.andypj.xyz

if x > 0 then print("正") end
来源：http://mlo.ivvv.top

[T39] Lua：模式匹配
来源：http://udr.cdnleiting.top

string.find(s, "%d+")
来源：http://lom.xingfuxueyuan.xyz

[T40] Lua：元表
来源：http://dbo.bbcook.cn

setmetatable({}, { __index = base })
来源：http://qrj.xuanzx.com

[T41] Perl：Hello World
来源：http://fcs.xuetiantiany.cn

print "Hello\n";
来源：http://rjk.svipenyu.cn

[T42] Perl：变量类型
来源：http://hqh.gzhubu.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kae.hnxiangtu.top

[T43] Perl：字符串插值
来源：http://rnh.wangdashe.top

"值: $a"
来源：http://mbc.andypj.xyz

[T44] Perl：条件
来源：http://lnm.jianghu66.top

if ($a > 0) { print "正"; }
来源：http://gbt.jianghu66.top

[T45] Perl：数组遍历
来源：http://wbl.tianlin.xyz

for my $x (@arr) { print $x; }
来源：http://juw.ehwqpu.com

[T46] Perl：哈希操作
来源：http://scn.yj202588.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jau.jinyuanbaomall.cn

[T47] Perl：正则捕获
来源：http://tib.sysykeji.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://fgw.hammf.cn

[T48] Perl：正则替换
来源：http://hov.yfazqb.com

$s =~ s/old/new/g;
来源：http://xfn.xuetiantiany.cn

[T49] Perl：函数
来源：http://yva.chenlongwang.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qwr.yueranfly.top

[T50] Perl：逐行读文件
来源：http://bxm.jianghu66.top

open my $fh, "<", "a.txt" or die $!;
来源：http://mky.guannengcc.top

while (my $line = <$fh>) { print $line; }
来源：http://mfv.yueranfly.top

[T51] Scala：Hello World
来源：http://sqb.jlsjyb.cn

println("Hello")
来源：http://sfl.shzxlz.cn

[T52] Scala：变量
来源：http://ism.yj20258.top

val a = 1;  var b = 2
来源：http://lhy.yongpay.top

[T53] Scala：字符串插值
来源：http://pth.zhixingplan.top

s"值: $b"
来源：http://gaz.andypj.xyz

[T54] Scala：集合映射
来源：http://zvx.nwbrower.top

List(1, 2, 3).map(_ * 2)
来源：http://jju.yuanzhike.top

[T55] Scala：集合过滤
来源：http://ldc.zhongyouzk.top

List(1, 2, 3).filter(_ > 1)
来源：http://uin.hcnkem.com

[T56] Scala：样例类
来源：http://zxj.ctjpmb.com

case class User(name: String, age: Int)
来源：http://ivl.zdbjq.cn

[T57] Scala：模式匹配
来源：http://bcb.c1oappe.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://iky.zdqjudy.top

[T58] Scala：函数定义
来源：http://whz.jqgfzy.top

def add(a: Int, b: Int): Int = a + b
来源：http://sri.jqgufenzy.top

[T59] Scala：循环
来源：http://nag.aizwys.cn

for (i <- 1 to 10) println(i)
来源：http://qyj.yongpay.top

[T60] Scala：折叠
来源：http://pni.fktsv.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://oxx.zycfv.cn

================================================================================
来源：http://twp.fehbvm.com

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://tiz.uphjek.com

================================================================================
来源：http://cth.svipenyu.cn

[U01] Py：创建虚拟环境
来源：http://rtq.shuidangran.top

python -m venv .venv && source .venv/bin/activate
来源：http://scm.hcnkem.com

[U02] Py：导出 / 安装依赖
来源：http://rwo.52xcode.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vbu.yonumen.top


<!-- 参考信息 -->