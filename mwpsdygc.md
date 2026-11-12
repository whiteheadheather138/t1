代发 wailian999

df -h;  du -sh *
来源：http://cae.shanyushiyangkeji.top

[R62] 找最占空间的文件
来源：http://npq.xinyue.icu

du -ah . | sort -rh | head -10
来源：http://pfk.shuidangran.top

[R63] 内存与进程
来源：http://tnd.yj20258.top

free -h;  ps aux | grep nginx
来源：http://cqa.jinghuilouyu.cn

[R64] 结束进程
来源：http://uby.fzhhl.top

kill -9 $(pgrep -f app.py)
来源：http://ioq.yanxiufei.cn

[R65] 查看端口占用
来源：http://tlb.hnxiangtu.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xui.hongshengwenyu.top

[R66] 定时任务
来源：http://rlo.yangfankeji.com

crontab -e;  crontab -l
来源：http://wnc.yj20258888.top

[R67] 生成随机十六进制串
来源：http://klo.hywenlv.cn

openssl rand -hex 16
来源：http://hak.9152youxi.cn

[R68] 计算文件校验值
来源：http://pjk.9152youxi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://enq.birdmap.top

[R69] 生成随机密码
来源：http://qnk.ctjpmb.com

head -c 16 /dev/urandom | base64
来源：http://uep.meibo888.top

[R70] 时间戳与互转
来源：http://nby.zycfv.cn

date +%s;  date -d @1700000000
来源：http://bsu.hongshengwenyu.top

[R71] 日期格式化
来源：http://ppg.nanxuanxn.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://txo.birdmap.top

[R72] 等待端口就绪
来源：http://awy.cashguo.top

until nc -z localhost 3306; do sleep 1; done
来源：http://wma.zhaomingkeji.xyz

[R73] 分割大日志
来源：http://uzt.shanyushiyangkeji.top

split -l 1000 big.log part_
来源：http://ilf.sweek.top

[R74] 批量重命名
来源：http://vpu.ydjk.org.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xru.bbcook.cn

[R75] 导出环境变量
来源：http://poh.redwolf501.top

export PATH="$HOME/bin:$PATH"
来源：http://cjt.nanxinkj.top

[R76] 使用临时文件
来源：http://ogn.feifeiyinyue.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vyp.uphjek.com

[R77] 读取用户输入
来源：http://nwi.9152youxi.cn

read -rp "请输入: " ans
来源：http://hvi.meibo888.top

[R78] 交互式菜单
来源：http://cme.hcnkem.com

select opt in a b c; do echo "$opt"; break; done
来源：http://vwt.zhijiandao.cn

[R79] 解析命令行选项
来源：http://bxn.zhiwuduotai.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rwq.chenzaomai.com

[R80] 查看脚本执行耗时
来源：http://bmq.andypj.xyz

time ./run.sh
来源：http://lnt.cashguo.top

================================================================================
来源：http://ztk.guannengcc.top

S. C / C++ 专题
来源：http://ziq.yj20258.top

================================================================================
来源：http://xfo.meibo888.top

[S01] C：Hello World
来源：http://awx.9152youxi.cn

#include <stdio.h>
来源：http://wjk.yfazqb.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://tyg.sysykeji.top

[S02] C：变量与格式化输出
来源：http://ehv.yuanzhike.top

int a = 10; printf("%d\n", a);
来源：http://exm.aibaodan.cn

[S03] C：读入整数
来源：http://pcy.svipenyu.cn

int x; scanf("%d", &x);
来源：http://cqp.tanke756.top

[S04] C：字符串复制
来源：http://nsb.ydzc1.top

char dst[32]; strcpy(dst, "hi");
来源：http://wtz.sweek.top

[S05] C：字符串长度
来源：http://mkv.52xcode.cn

strlen(s)
来源：http://nog.9152youxi.cn

[S06] C：字符串比较
来源：http://djl.ppjwa.cn

strcmp(a, b) == 0
来源：http://imu.ydjk.org.cn

[S07] C：数组遍历求和
来源：http://wvl.gogol.net.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://liw.epnwcf.com

[S08] C：动态内存分配与释放
来源：http://lnx.jiagoushi.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zzl.xuetiantiany.cn

[S09] C：结构体定义与初始化
来源：http://yoa.meibo888.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uez.dashuyun.cn

[S10] C：指针与解引用
来源：http://koc.dianchejie.cn

int *p = &a;  *p = 5;
来源：http://vfq.gotoacloud.top

[S11] C：逐行读文件
来源：http://xzy.ppjwa.cn

FILE *f = fopen("a.txt", "r");
来源：http://nvr.guowangkeji.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ycv.tianlin.xyz

fclose(f);
来源：http://zcc.shzxlz.cn

[S12] C：写文件
来源：http://zpa.zycfv.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qlb.daria6918.cn

[S13] C：宏定义
来源：http://wux.meibo888.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mnx.birdmap.top

[S14] C：枚举
来源：http://stf.yj20258888.top

enum Color { RED, GREEN, BLUE };
来源：http://ksq.shanyushiyangtech.top

[S15] C：类型转换
来源：http://rlr.xuetiantiany.cn

(double) a / b
来源：http://yiy.chenzaomai.com

[S16] C：位操作置位
来源：http://tuw.pengpengdd.cyou

x |= (1 << 3);
来源：http://rtf.jinqigfzy.top

[S17] C：安全拼接字符串
来源：http://hxz.ehwqpu.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wvt.guannengcc.top

[S18] C：命令行参数
来源：http://dah.bbcook.cn

int main(int argc, char **argv)
来源：http://iqo.sxryk.cn

[S19] C：快速排序
来源：http://huv.zhoulong.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://fms.316326.xyz

[S20] C：二分查找
来源：http://ylx.sysykeji.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yny.gotoacloud.top

[S21] C：字符类别判断
来源：http://amm.xingfuxueyuan.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mfv.daxiang520.top

[S22] C：字符串转数字
来源：http://toc.zdqjudy.top

atoi("42");  strtod("3.14", NULL);
来源：http://xzf.xziqi.cn

[S23] C：随机数
来源：http://inu.jinqigufen.top

srand(time(NULL));  int r = rand() % 100;
来源：http://qsr.zhengqikj.top

[S24] C：获取本地时间
来源：http://yfq.svipenyu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nov.fanxiaobao.xyz

[S25] C：内存拷贝
来源：http://nsw.zhaomingkeji.xyz

memcpy(dst, src, n);
来源：http://gld.snrcjt.cn

[S26] C：内存清零
来源：http://ewk.fehbvm.com

memset(a, 0, sizeof a);
来源：http://mtg.cucudq.cn

[S27] C：定义常量
来源：http://psg.nanxuanxn.top

const double PI = 3.14159;
来源：http://trd.quarkkingdee.top

[S28] C：静态变量
来源：http://kih.c1oappe.top

static int counter = 0;
来源：http://ody.ctjpmb.com

[S29] C：变参函数
来源：http://ibm.ehwqpu.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bfi.shangyingyoupin.top

[S30] C：头文件保护
来源：http://prv.tarul.cn

#ifndef X_H
来源：http://ngk.yuxming.cn

#define X_H
来源：http://xbt.sufxvd.cn

#endif
来源：http://dss.yanxiufei.cn

[S31] C++：Hello World
来源：http://iux.ctjpmb.com

#include <iostream>
来源：http://kua.nanxuanxn.top

int main() { std::cout << "Hello\n"; }
来源：http://wut.nanxuanxn.top

[S32] C++：字符串
来源：http://gez.zycfv.cn

std::string s = "hi";  s += "!";
来源：http://wwg.mhx1999.top

[S33] C++：vector 增删
来源：http://djr.hywenlv.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://whm.gaohongyu789.top

[S34] C++：遍历 vector
来源：http://uoe.yonumen.top

for (auto &x : v) { std::cout << x; }
来源：http://jir.wangdashe.top

[S35] C++：map
来源：http://pme.fktsv.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hcq.aibaodan.cn

[S36] C++：unordered_map
来源：http://efx.ywan-chungtsiang.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vxq.yongpay.top

[S37] C++：set
来源：http://yeu.fktsv.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://euu.chenlongwang.top

[S38] C++：排序
来源：http://fwk.dashuyun.cn

std::sort(v.begin(), v.end());
来源：http://ruu.0kj1m.cn

[S39] C++：自定义比较器排序
来源：http://ytu.xuanzx.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fws.hongshengwenyu.top

[S40] C++：查找元素
来源：http://cxu.9152youxi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bmf.snrcjt.cn

[S41] C++：类与构造函数
来源：http://kfc.316326.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://isa.yangfankeji.com

[S42] C++：继承与虚函数
来源：http://sbq.cheryme.top

class B : public Base { public: void f() override {} };
来源：http://zaw.jqgufenzy.top

[S43] C++：智能指针
来源：http://hog.hongshengwenyu.top

auto p = std::make_unique<int>(5);
来源：http://zda.kuanghao11.cn

[S44] C++：引用传参
来源：http://wwp.gzhubu.top

void inc(int &x) { ++x; }
来源：http://ziz.sufxvd.cn

[S45] C++：lambda
来源：http://axh.zhixingplan.top

auto add = [](int a, int b) { return a + b; };
来源：http://mnq.ybcxt.top

[S46] C++：函数模板
来源：http://eup.gogol.net.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zoz.zdqjudy.top

[S47] C++：结构化绑定遍历
来源：http://vau.shzxlz.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xdv.shzxlz.cn

[S48] C++：逐行读文件
来源：http://jjx.snrcjt.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gki.yj20258888.top

while (std::getline(in, line)) { }
来源：http://ipb.fzhhl.top

[S49] C++：写文件
来源：http://sem.nanxinkj.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pus.ivvv.top

[S50] C++：格式化数字
来源：http://pjv.vqdsnc.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://guw.xylfe.cn

[S51] C++：显式类型转换
来源：http://lbt.haohaochexian.top

static_cast<double>(a) / b
来源：http://btd.cashguo.top

[S52] C++：const 与 noexcept
来源：http://lbi.kuanghao11.cn

int size() const noexcept { return n_; }
来源：http://ihb.hongshengwenyu.top

[S53] C++：移动语义
来源：http://dhu.snrcjt.cn

std::vector<int> w = std::move(v);
来源：http://nzq.hesvh.cn

[S54] C++：异常处理
来源：http://zov.chenzaomai.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://iqi.xinyue.icu

[S55] C++：结构化绑定
来源：http://ylf.hcnkem.com

auto [a, b] = std::make_pair(1, 2);
来源：http://aoj.shangyingyoupin.top

[S56] C++：optional
来源：http://bft.aizwys.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dys.tian-w.cn

[S57] C++：编译期常量
来源：http://jto.guowangkeji.top

constexpr int N = 10;
来源：http://hfq.jinghuilouyu.cn

[S58] C++：命名空间
来源：http://gvb.bjfxy.top

namespace ns { int f() { return 1; } }
来源：http://ogl.guowangkeji.top

[S59] C++：静态断言
来源：http://csl.pycfn.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kuk.nanxuanxn.top

[S60] C++：遍历并删除元素
来源：http://qii.hnxiangtu.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wwy.daria6918.cn

================================================================================
来源：http://yqn.gaohongyu789.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://upp.zhoulong.xyz

================================================================================
来源：http://kyg.yuanzhike.top

[T01] Kotlin：Hello World
来源：http://ovg.jinqigfzy.top

println("Hello")
来源：http://ygx.quarkkingdee.top

[T02] Kotlin：变量
来源：http://bqe.shanyushiyangkeji.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://luf.sufxvd.cn

[T03] Kotlin：字符串模板
来源：http://equ.jyoumei.cn

"值: $b"
来源：http://xmx.shuidangran.top

[T04] Kotlin：空安全
来源：http://ndt.daria6918.cn

val n: String? = null;  n?.length
来源：http://afi.shzxlz.cn

[T05] Kotlin：when 表达式
来源：http://ofm.shanyushiyangtech.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vzh.yangfankeji.com

[T06] Kotlin：集合映射
来源：http://akm.bjfxy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://tze.yuxming.cn

[T07] Kotlin：集合过滤
来源：http://tgk.nanxinkj.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://hfs.gogol.net.cn

[T08] Kotlin：数据类
来源：http://ooc.cashguo.top

data class User(val name: String, val age: Int)
来源：http://avt.shanyushiyangtech.top

[T09] Kotlin：扩展函数
来源：http://lys.uphjek.com

fun String.exclaim() = this + "!"
来源：http://rdg.bjfxy.top

[T10] Kotlin：默认参数
来源：http://tsu.xziqi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://hgi.yj20258.top

[T11] Kotlin：协程
来源：http://ukz.pengpengdd.cyou

GlobalScope.launch { delay(1000); println("done") }
来源：http://irx.xinyue.icu

[T12] Kotlin：解构声明
来源：http://eyj.andypj.xyz

val (a, b) = Pair(1, 2)
来源：http://tsu.ctjpmb.com

[T13] Kotlin：只读 Map
来源：http://hgz.xinyue.icu

val m = mapOf("a" to 1)
来源：http://yis.fanxiaobao.xyz

[T14] Kotlin：循环
来源：http://vdg.hywenlv.cn

for (i in 1..10) println(i)
来源：http://xjd.aizwys.cn

[T15] Kotlin：接口
来源：http://zjk.hcnkem.com

interface Shape { fun area(): Double }
来源：http://joi.yongpay.top

[T16] Swift：Hello World
来源：http://cew.xuetiantiany.cn

print("Hello")
来源：http://dfk.cdnleiting.top

[T17] Swift：变量与常量
来源：http://nqj.chenlongwang.top

var a = 1;  let b = 2
来源：http://joi.zhoulong.xyz

[T18] Swift：字符串插值
来源：http://jpn.jiagoushi.top

"值: \(b)"
来源：http://hqk.hcnkem.com

[T19] Swift：可选绑定
来源：http://mxy.jlsjyb.cn

if let n = opt { print(n) }
来源：http://mhi.zhiwuduotai.top

[T20] Swift：数组操作
来源：http://oaq.gzhubu.top

var a = [1, 2, 3];  a.append(4)
来源：http://eic.nanxuanxn.top

[T21] Swift：遍历
来源：http://gfk.ybcxt.top

for x in a { print(x) }
来源：http://vlk.zhijiandao.cn

[T22] Swift：字典
来源：http://mjc.gaohongyu789.top

var d = ["a": 1];  d["b"] = 2
来源：http://moe.hnqzz.top

[T23] Swift：函数
来源：http://qij.bbcook.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vwt.sxryk.cn

[T24] Swift：闭包
来源：http://ebg.iojbl.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://oxg.svipenyu.cn

[T25] Swift：结构体
来源：http://eib.zycfv.cn

struct P { var x: Int }
来源：http://hca.jinghuilouyu.cn

[T26] Swift：类与重写
来源：http://gqa.zhoulong.xyz

class A: Base { override func f() {} }
来源：http://msc.iojbl.cn

[T27] Swift：错误处理
来源：http://fgn.shzxlz.cn

do { try f() } catch { print(error) }
来源：http://cgm.yonumen.top

[T28] Swift：枚举
来源：http://yok.ydzc1.top

enum Color { case red, green }
来源：http://cfv.sxryk.cn

[T29] Swift：guard 提前返回
来源：http://saf.fktsv.cn

guard let x = opt else { return }
来源：http://fxu.wangshuangyany.cn

[T30] Swift：协议
来源：http://unp.daxiang520.top

protocol Shape { func area() -> Double }
来源：http://sxf.snrcjt.cn

[T31] Lua：Hello World
来源：http://pwh.jlsjyb.cn

print("Hello")
来源：http://pdh.snrcjt.cn

[T32] Lua：局部变量
来源：http://gev.zhongyouzk.top

local a = 1
来源：http://mke.cdnleiting.top

[T33] Lua：表（数组）
来源：http://fcd.hammf.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://reh.sxryk.cn

[T34] Lua：遍历表
来源：http://kof.jinghuilouyu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qpb.vqdsnc.cn

[T35] Lua：字典表
来源：http://rgj.guannengcc.top

local d = { a = 1 };  d.b = 2
来源：http://rgc.jqgfzy.top

[T36] Lua：函数
来源：http://tkg.xziqi.cn

function add(a, b) return a + b end
来源：http://wlp.daria6918.cn

[T37] Lua：字符串拼接
来源：http://sbi.zhoulong.xyz

"a" .. "b"
来源：http://tjw.zhiwuduotai.top

[T38] Lua：条件
来源：http://oyq.aizwys.cn

if x > 0 then print("正") end
来源：http://npi.zycfv.cn

[T39] Lua：模式匹配
来源：http://cdp.yvedp.cn

string.find(s, "%d+")
来源：http://imc.dianchejie.cn

[T40] Lua：元表
来源：http://ixs.andypj.xyz

setmetatable({}, { __index = base })
来源：http://utm.ybcxt.top

[T41] Perl：Hello World
来源：http://wiv.mhx1999.top

print "Hello\n";
来源：http://fwx.52xcode.cn

[T42] Perl：变量类型
来源：http://zcu.jqgufenzy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gop.cdnleiting.top

[T43] Perl：字符串插值
来源：http://lyr.0kj1m.cn

"值: $a"
来源：http://ctw.yfazqb.com

[T44] Perl：条件
来源：http://hwh.chenzaomai.com

if ($a > 0) { print "正"; }
来源：http://kva.chenlongwang.top

[T45] Perl：数组遍历
来源：http://fea.hammf.cn

for my $x (@arr) { print $x; }
来源：http://iiw.shanyushiyangtech.top

[T46] Perl：哈希操作
来源：http://zih.cheryme.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hsj.9152youxi.cn

[T47] Perl：正则捕获
来源：http://ddq.gaohongyu789.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://xvk.chenlongwang.top

[T48] Perl：正则替换
来源：http://iaq.zdqjudy.top

$s =~ s/old/new/g;
来源：http://ggx.sjlbkw.cn

[T49] Perl：函数
来源：http://nwo.jiagoushi.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://obj.smart0.xyz

[T50] Perl：逐行读文件
来源：http://sgv.c1oappe.top

open my $fh, "<", "a.txt" or die $!;
来源：http://vim.tanke756.top

while (my $line = <$fh>) { print $line; }
来源：http://ehx.aizwys.cn

[T51] Scala：Hello World
来源：http://sfr.chenzaomai.com

println("Hello")
来源：http://icv.chenzaomai.com

[T52] Scala：变量
来源：http://rlv.zhiwuduotai.top

val a = 1;  var b = 2
来源：http://dtq.cdnleiting.top

[T53] Scala：字符串插值
来源：http://nfr.fengsongda.top

s"值: $b"
来源：http://dok.gogol.net.cn

[T54] Scala：集合映射
来源：http://rhf.52xcode.cn

List(1, 2, 3).map(_ * 2)
来源：http://qdd.xingfuxueyuan.xyz

[T55] Scala：集合过滤
来源：http://wsm.yuanzhike.top

List(1, 2, 3).filter(_ > 1)
来源：http://qru.cucudq.cn

[T56] Scala：样例类
来源：http://kxu.hywenlv.cn

case class User(name: String, age: Int)
来源：http://lrj.havefunace.top

[T57] Scala：模式匹配
来源：http://rfh.aizwys.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://hbz.fanxiaobao.xyz

[T58] Scala：函数定义
来源：http://xbg.fehbvm.com

def add(a: Int, b: Int): Int = a + b
来源：http://vlo.fzhhl.top

[T59] Scala：循环
来源：http://tsg.hammf.cn

for (i <- 1 to 10) println(i)
来源：http://fzl.zdqjudy.top

[T60] Scala：折叠
来源：http://mgi.shzxlz.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gtl.hesvh.cn

================================================================================
来源：http://fqv.hesvh.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xbo.zhiwuduotai.top

================================================================================
来源：http://vyt.shanyushiyangkeji.top

[U01] Py：创建虚拟环境
来源：http://goq.yuxming.cn

python -m venv .venv && source .venv/bin/activate
来源：http://pgo.shuidangran.top

[U02] Py：导出 / 安装依赖
来源：http://qlp.jinqigufen.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://baa.zdbjq.cn


<!-- 参考信息 -->