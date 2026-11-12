代发 wailian999

df -h;  du -sh *
来源：http://ikr.tarul.cn

[R62] 找最占空间的文件
来源：http://teb.ctjpmb.com

du -ah . | sort -rh | head -10
来源：http://xpt.yangfankeji.com

[R63] 内存与进程
来源：http://fcw.zdbjq.cn

free -h;  ps aux | grep nginx
来源：http://bbz.nanxuanxn.top

[R64] 结束进程
来源：http://wfo.jqgfzy.top

kill -9 $(pgrep -f app.py)
来源：http://omj.gogol.net.cn

[R65] 查看端口占用
来源：http://uvj.vqdsnc.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wct.vqdsnc.cn

[R66] 定时任务
来源：http://jne.pycfn.com

crontab -e;  crontab -l
来源：http://tti.redwolf501.top

[R67] 生成随机十六进制串
来源：http://rjr.sweek.top

openssl rand -hex 16
来源：http://wve.hammf.cn

[R68] 计算文件校验值
来源：http://cnr.vqdsnc.cn

sha256sum a.txt;  md5sum a.txt
来源：http://nmz.jiagoushi.top

[R69] 生成随机密码
来源：http://vlj.shuidangran.top

head -c 16 /dev/urandom | base64
来源：http://mke.meibo888.top

[R70] 时间戳与互转
来源：http://vjl.zhijiandao.cn

date +%s;  date -d @1700000000
来源：http://cqx.zhoulong.xyz

[R71] 日期格式化
来源：http://opc.quarkkingdee.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://pit.shangyingyoupin.top

[R72] 等待端口就绪
来源：http://hyg.wangshuangyany.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://rpu.chenlongwang.top

[R73] 分割大日志
来源：http://ics.wangdashe.top

split -l 1000 big.log part_
来源：http://fkj.uphjek.com

[R74] 批量重命名
来源：http://rwa.cashguo.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://usr.hfpthk.cn

[R75] 导出环境变量
来源：http://nwq.ehwqpu.com

export PATH="$HOME/bin:$PATH"
来源：http://sfv.52xcode.cn

[R76] 使用临时文件
来源：http://kuy.xuanzx.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kzx.yonumen.top

[R77] 读取用户输入
来源：http://sip.daxiang520.top

read -rp "请输入: " ans
来源：http://neb.daria6918.cn

[R78] 交互式菜单
来源：http://pep.tian-w.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://lzu.dianchejie.cn

[R79] 解析命令行选项
来源：http://avf.sxryk.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://twv.hesvh.cn

[R80] 查看脚本执行耗时
来源：http://trf.chenjidiqi.icu

time ./run.sh
来源：http://ipg.bjfxy.top

================================================================================
来源：http://tpu.bjfxy.top

S. C / C++ 专题
来源：http://nsr.ehwqpu.com

================================================================================
来源：http://adw.shuidangran.top

[S01] C：Hello World
来源：http://hjc.zhoulong.xyz

#include <stdio.h>
来源：http://www.snrcjt.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gax.jinghuilouyu.cn

[S02] C：变量与格式化输出
来源：http://rkm.uphjek.com

int a = 10; printf("%d\n", a);
来源：http://jes.zhoulong.xyz

[S03] C：读入整数
来源：http://cjr.zhijiandao.cn

int x; scanf("%d", &x);
来源：http://bis.ivvv.top

[S04] C：字符串复制
来源：http://onj.9152youxi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://tnu.havefunace.top

[S05] C：字符串长度
来源：http://afk.aibaodan.cn

strlen(s)
来源：http://rlt.zhongyouzk.top

[S06] C：字符串比较
来源：http://bcd.chenzaomai.com

strcmp(a, b) == 0
来源：http://che.sufxvd.cn

[S07] C：数组遍历求和
来源：http://otr.yonumen.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kyl.cashguo.top

[S08] C：动态内存分配与释放
来源：http://oyn.bbcook.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lht.vqdsnc.cn

[S09] C：结构体定义与初始化
来源：http://zzm.jiagoushi.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lkd.cdnleiting.top

[S10] C：指针与解引用
来源：http://mzm.aizwys.cn

int *p = &a;  *p = 5;
来源：http://iqc.tianlin.xyz

[S11] C：逐行读文件
来源：http://rqd.fzhhl.top

FILE *f = fopen("a.txt", "r");
来源：http://gql.redwolf501.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://yls.kuanghao11.cn

fclose(f);
来源：http://ijh.jqgfzy.top

[S12] C：写文件
来源：http://oyo.tianlin.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://srm.gogol.net.cn

[S13] C：宏定义
来源：http://hzs.guannengcc.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pqf.pengpengdd.cyou

[S14] C：枚举
来源：http://caa.aizwys.cn

enum Color { RED, GREEN, BLUE };
来源：http://jii.shuidangran.top

[S15] C：类型转换
来源：http://sze.tian-w.cn

(double) a / b
来源：http://rvd.zhijiandao.cn

[S16] C：位操作置位
来源：http://pvl.andypj.xyz

x |= (1 << 3);
来源：http://wcl.jlsjyb.cn

[S17] C：安全拼接字符串
来源：http://rvl.haohaochexian.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ugv.daxiang520.top

[S18] C：命令行参数
来源：http://roh.zhengqikj.top

int main(int argc, char **argv)
来源：http://fno.shangyingyoupin.top

[S19] C：快速排序
来源：http://qao.ivvv.top

qsort(a, n, sizeof(int), cmp);
来源：http://rpq.gaohongyu789.top

[S20] C：二分查找
来源：http://tec.jiagoushi.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gfz.hysaishi.cn

[S21] C：字符类别判断
来源：http://cjo.wangshuangyany.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://juz.pycfn.com

[S22] C：字符串转数字
来源：http://jaz.bbcook.cn

atoi("42");  strtod("3.14", NULL);
来源：http://eic.ehwqpu.com

[S23] C：随机数
来源：http://wvt.nanxinkj.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ton.9152youxi.cn

[S24] C：获取本地时间
来源：http://leb.zhijiandao.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ixx.ydzc1.top

[S25] C：内存拷贝
来源：http://wyz.aibaodan.cn

memcpy(dst, src, n);
来源：http://woy.redwolf501.top

[S26] C：内存清零
来源：http://tjh.ppjwa.cn

memset(a, 0, sizeof a);
来源：http://rec.yuanzhike.top

[S27] C：定义常量
来源：http://qjx.bbcook.cn

const double PI = 3.14159;
来源：http://uhs.jinqigufen.top

[S28] C：静态变量
来源：http://prg.shanyushiyangkeji.top

static int counter = 0;
来源：http://ccu.iojbl.cn

[S29] C：变参函数
来源：http://qxc.fzhhl.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bvj.tarul.cn

[S30] C：头文件保护
来源：http://ryh.aizwys.cn

#ifndef X_H
来源：http://wfi.jyoumei.cn

#define X_H
来源：http://vwa.haohaochexian.top

#endif
来源：http://hvx.fzhhl.top

[S31] C++：Hello World
来源：http://zro.xylfe.cn

#include <iostream>
来源：http://bza.havefunace.top

int main() { std::cout << "Hello\n"; }
来源：http://tnw.zhengqikj.top

[S32] C++：字符串
来源：http://eie.zhoulong.xyz

std::string s = "hi";  s += "!";
来源：http://qtw.haohaochexian.top

[S33] C++：vector 增删
来源：http://eas.sufxvd.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mjn.cheryme.top

[S34] C++：遍历 vector
来源：http://zqt.gaohongyu789.top

for (auto &x : v) { std::cout << x; }
来源：http://qkh.dashuyun.cn

[S35] C++：map
来源：http://deh.ctjpmb.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vvk.hongshengwenyu.top

[S36] C++：unordered_map
来源：http://ack.hnqzz.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cqb.ehwqpu.com

[S37] C++：set
来源：http://ohh.gzhubu.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://laj.dashuyun.cn

[S38] C++：排序
来源：http://wvl.fehbvm.com

std::sort(v.begin(), v.end());
来源：http://kek.andypj.xyz

[S39] C++：自定义比较器排序
来源：http://gfh.yangfankeji.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ztq.chenzaomai.com

[S40] C++：查找元素
来源：http://izi.xuanzx.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vry.chenlongwang.top

[S41] C++：类与构造函数
来源：http://fju.yueranfly.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pow.bjfxy.top

[S42] C++：继承与虚函数
来源：http://sje.hnxiangtu.top

class B : public Base { public: void f() override {} };
来源：http://xry.snrcjt.cn

[S43] C++：智能指针
来源：http://ddc.haohaochexian.top

auto p = std::make_unique<int>(5);
来源：http://pno.quarkkingdee.top

[S44] C++：引用传参
来源：http://lfw.vehdjk.com

void inc(int &x) { ++x; }
来源：http://aml.gzhubu.top

[S45] C++：lambda
来源：http://wfo.jinghuilouyu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://dvx.cheryme.top

[S46] C++：函数模板
来源：http://oee.daria6918.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ncj.bbcook.cn

[S47] C++：结构化绑定遍历
来源：http://att.hammf.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://upu.vehdjk.com

[S48] C++：逐行读文件
来源：http://jkq.guowangkeji.top

std::ifstream in("a.txt");  std::string line;
来源：http://dcf.ybcxt.top

while (std::getline(in, line)) { }
来源：http://fkj.gaohongyu789.top

[S49] C++：写文件
来源：http://kqs.cheryme.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hza.tian-w.cn

[S50] C++：格式化数字
来源：http://zas.yvedp.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fno.hammf.cn

[S51] C++：显式类型转换
来源：http://jmx.0kj1m.cn

static_cast<double>(a) / b
来源：http://ehl.zhengqikj.top

[S52] C++：const 与 noexcept
来源：http://hyz.pycfn.com

int size() const noexcept { return n_; }
来源：http://fsc.sweek.top

[S53] C++：移动语义
来源：http://vgy.fehbvm.com

std::vector<int> w = std::move(v);
来源：http://clg.9152youxi.cn

[S54] C++：异常处理
来源：http://khp.ppjwa.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zwp.chenzaomai.com

[S55] C++：结构化绑定
来源：http://ekm.gotoacloud.top

auto [a, b] = std::make_pair(1, 2);
来源：http://mmn.jqgfzy.top

[S56] C++：optional
来源：http://bac.chenzaomai.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jwl.zdbjq.cn

[S57] C++：编译期常量
来源：http://cex.dianchejie.cn

constexpr int N = 10;
来源：http://ohv.kuanghao11.cn

[S58] C++：命名空间
来源：http://aqa.zdqjudy.top

namespace ns { int f() { return 1; } }
来源：http://wff.chenzaomai.com

[S59] C++：静态断言
来源：http://bsu.nanxuanxn.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gak.nanxinkj.top

[S60] C++：遍历并删除元素
来源：http://fyx.ywan-chungtsiang.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wpx.xingfuxueyuan.xyz

================================================================================
来源：http://aof.hammf.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://roq.cheryme.top

================================================================================
来源：http://vgz.tanke756.top

[T01] Kotlin：Hello World
来源：http://dsy.zdqjudy.top

println("Hello")
来源：http://cat.yangfankeji.com

[T02] Kotlin：变量
来源：http://ydu.iojbl.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jji.zhijiandao.cn

[T03] Kotlin：字符串模板
来源：http://kpa.ydjk.org.cn

"值: $b"
来源：http://ytc.birdmap.top

[T04] Kotlin：空安全
来源：http://spi.c1oappe.top

val n: String? = null;  n?.length
来源：http://avc.zycfv.cn

[T05] Kotlin：when 表达式
来源：http://gtg.aibaodan.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vdq.quarkkingdee.top

[T06] Kotlin：集合映射
来源：http://urf.nanxinkj.top

listOf(1, 2, 3).map { it * 2 }
来源：http://dxt.hesvh.cn

[T07] Kotlin：集合过滤
来源：http://ymg.sxryk.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://kox.vehdjk.com

[T08] Kotlin：数据类
来源：http://dmq.yuanzhike.top

data class User(val name: String, val age: Int)
来源：http://gxs.xuanzx.com

[T09] Kotlin：扩展函数
来源：http://iwy.chenzaomai.com

fun String.exclaim() = this + "!"
来源：http://def.fanxiaobao.xyz

[T10] Kotlin：默认参数
来源：http://abc.tarul.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ffg.cucudq.cn

[T11] Kotlin：协程
来源：http://qha.yongpay.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://mhg.yonumen.top

[T12] Kotlin：解构声明
来源：http://xua.jyoumei.cn

val (a, b) = Pair(1, 2)
来源：http://vuz.xinyue.icu

[T13] Kotlin：只读 Map
来源：http://hmp.yj20258888.top

val m = mapOf("a" to 1)
来源：http://ava.xinyue.icu

[T14] Kotlin：循环
来源：http://zum.hnxiangtu.top

for (i in 1..10) println(i)
来源：http://mfd.andypj.xyz

[T15] Kotlin：接口
来源：http://drq.9152youxi.cn

interface Shape { fun area(): Double }
来源：http://smz.gzhubu.top

[T16] Swift：Hello World
来源：http://cpd.jiagoushi.top

print("Hello")
来源：http://kwp.cdnleiting.top

[T17] Swift：变量与常量
来源：http://iqv.zhixingplan.top

var a = 1;  let b = 2
来源：http://wny.chenlongwang.top

[T18] Swift：字符串插值
来源：http://jdl.yj20258888.top

"值: \(b)"
来源：http://tbw.dianchejie.cn

[T19] Swift：可选绑定
来源：http://bjb.chenjidiqi.icu

if let n = opt { print(n) }
来源：http://vcj.tanke756.top

[T20] Swift：数组操作
来源：http://gmg.nanxinkj.top

var a = [1, 2, 3];  a.append(4)
来源：http://hmy.wangshuangyany.cn

[T21] Swift：遍历
来源：http://ddc.wangshuangyany.cn

for x in a { print(x) }
来源：http://vek.shzxlz.cn

[T22] Swift：字典
来源：http://jqw.xziqi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://izj.daxiang520.top

[T23] Swift：函数
来源：http://qzh.daria6918.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tdt.hongshengwenyu.top

[T24] Swift：闭包
来源：http://heo.jqgfzy.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://tbr.yfazqb.com

[T25] Swift：结构体
来源：http://pne.yj202588.top

struct P { var x: Int }
来源：http://ohc.cucudq.cn

[T26] Swift：类与重写
来源：http://lrd.jlsjyb.cn

class A: Base { override func f() {} }
来源：http://vok.yj20258888.top

[T27] Swift：错误处理
来源：http://kgl.meibo888.top

do { try f() } catch { print(error) }
来源：http://mkz.yfazqb.com

[T28] Swift：枚举
来源：http://utk.zhiwuduotai.top

enum Color { case red, green }
来源：http://ljp.cucudq.cn

[T29] Swift：guard 提前返回
来源：http://pli.cheryme.top

guard let x = opt else { return }
来源：http://jfm.chenzaomai.com

[T30] Swift：协议
来源：http://fei.sufxvd.cn

protocol Shape { func area() -> Double }
来源：http://vgx.jiagoushi.top

[T31] Lua：Hello World
来源：http://xgp.gzhubu.top

print("Hello")
来源：http://yno.vqdsnc.cn

[T32] Lua：局部变量
来源：http://kvm.dashuyun.cn

local a = 1
来源：http://uqg.feifeiyinyue.top

[T33] Lua：表（数组）
来源：http://fra.ehwqpu.com

local t = {1, 2, 3};  t[4] = 4
来源：http://awh.hfpthk.cn

[T34] Lua：遍历表
来源：http://whj.ydjk.org.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://osa.chenjidiqi.icu

[T35] Lua：字典表
来源：http://rsh.fzhhl.top

local d = { a = 1 };  d.b = 2
来源：http://jtr.jinqigfzy.top

[T36] Lua：函数
来源：http://gyo.epnwcf.com

function add(a, b) return a + b end
来源：http://jao.jqgfzy.top

[T37] Lua：字符串拼接
来源：http://efs.gzhubu.top

"a" .. "b"
来源：http://wsb.chenjidiqi.icu

[T38] Lua：条件
来源：http://ikv.nwbrower.top

if x > 0 then print("正") end
来源：http://oib.zhiwuduotai.top

[T39] Lua：模式匹配
来源：http://yxq.guannengcc.top

string.find(s, "%d+")
来源：http://whm.aibaodan.cn

[T40] Lua：元表
来源：http://yon.redwolf501.top

setmetatable({}, { __index = base })
来源：http://cyp.yfazqb.com

[T41] Perl：Hello World
来源：http://lmv.yj20258.top

print "Hello\n";
来源：http://edx.ydjk.org.cn

[T42] Perl：变量类型
来源：http://lsh.cashguo.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://awc.hysaishi.cn

[T43] Perl：字符串插值
来源：http://yru.52xcode.cn

"值: $a"
来源：http://gzl.shuidangran.top

[T44] Perl：条件
来源：http://pnm.snrcjt.cn

if ($a > 0) { print "正"; }
来源：http://dcq.zhoulong.xyz

[T45] Perl：数组遍历
来源：http://pkr.bbcook.cn

for my $x (@arr) { print $x; }
来源：http://gfg.ybcxt.top

[T46] Perl：哈希操作
来源：http://jqe.ydjk.org.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://owv.ppjwa.cn

[T47] Perl：正则捕获
来源：http://vjn.hnxiangtu.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://lal.yanxiufei.cn

[T48] Perl：正则替换
来源：http://vow.jqgfzy.top

$s =~ s/old/new/g;
来源：http://ars.xziqi.cn

[T49] Perl：函数
来源：http://axc.jyoumei.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://srs.pengpengdd.cyou

[T50] Perl：逐行读文件
来源：http://srp.fzhhl.top

open my $fh, "<", "a.txt" or die $!;
来源：http://mtw.yfazqb.com

while (my $line = <$fh>) { print $line; }
来源：http://lvj.xuanzx.com

[T51] Scala：Hello World
来源：http://lzt.daria6918.cn

println("Hello")
来源：http://vda.fehbvm.com

[T52] Scala：变量
来源：http://hsr.jinyuanbaomall.cn

val a = 1;  var b = 2
来源：http://wgd.zhoulong.xyz

[T53] Scala：字符串插值
来源：http://ayf.meibo888.top

s"值: $b"
来源：http://uaw.nanxuanxn.top

[T54] Scala：集合映射
来源：http://slf.yangfankeji.com

List(1, 2, 3).map(_ * 2)
来源：http://mvo.daria6918.cn

[T55] Scala：集合过滤
来源：http://wku.xuanzx.com

List(1, 2, 3).filter(_ > 1)
来源：http://nux.hammf.cn

[T56] Scala：样例类
来源：http://nry.cdnleiting.top

case class User(name: String, age: Int)
来源：http://kuq.gotoacloud.top

[T57] Scala：模式匹配
来源：http://zfs.jinghuilouyu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://aqe.bjfxy.top

[T58] Scala：函数定义
来源：http://epy.yanxiufei.cn

def add(a: Int, b: Int): Int = a + b
来源：http://lgc.316326.xyz

[T59] Scala：循环
来源：http://zwb.jinghuilouyu.cn

for (i <- 1 to 10) println(i)
来源：http://djz.316326.xyz

[T60] Scala：折叠
来源：http://oaw.guowangkeji.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bdd.yj20258.top

================================================================================
来源：http://zdc.jianghu66.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ncp.ybcxt.top

================================================================================
来源：http://nlo.ctjpmb.com

[U01] Py：创建虚拟环境
来源：http://jgx.epnwcf.com

python -m venv .venv && source .venv/bin/activate
来源：http://tjz.xuanzx.com

[U02] Py：导出 / 安装依赖
来源：http://umt.jqgfzy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cln.xziqi.cn


<!-- 参考信息 -->