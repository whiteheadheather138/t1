代发 wailian999

df -h;  du -sh *
来源：http://gya.gogol.net.cn

[R62] 找最占空间的文件
来源：http://edd.kuanghao11.cn

du -ah . | sort -rh | head -10
来源：http://jlz.shangyingyoupin.top

[R63] 内存与进程
来源：http://xin.pycfn.com

free -h;  ps aux | grep nginx
来源：http://iyo.nanxinkj.top

[R64] 结束进程
来源：http://wwr.jinqigufen.top

kill -9 $(pgrep -f app.py)
来源：http://kon.hesvh.cn

[R65] 查看端口占用
来源：http://fcz.zdbjq.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rls.jianghu66.top

[R66] 定时任务
来源：http://gca.meibo888.top

crontab -e;  crontab -l
来源：http://urv.ctjpmb.com

[R67] 生成随机十六进制串
来源：http://vmo.sweek.top

openssl rand -hex 16
来源：http://fda.guannengcc.top

[R68] 计算文件校验值
来源：http://tpv.guowangkeji.top

sha256sum a.txt;  md5sum a.txt
来源：http://gus.cucudq.cn

[R69] 生成随机密码
来源：http://jon.jlsjyb.cn

head -c 16 /dev/urandom | base64
来源：http://bhr.redwolf501.top

[R70] 时间戳与互转
来源：http://jcu.dashuyun.cn

date +%s;  date -d @1700000000
来源：http://bec.tanke756.top

[R71] 日期格式化
来源：http://isj.vehdjk.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://ihu.tianlin.xyz

[R72] 等待端口就绪
来源：http://nto.ehwqpu.com

until nc -z localhost 3306; do sleep 1; done
来源：http://pii.gogol.net.cn

[R73] 分割大日志
来源：http://tey.chenlongwang.top

split -l 1000 big.log part_
来源：http://icb.jianghu66.top

[R74] 批量重命名
来源：http://lgc.yuanzhike.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://chk.yongpay.top

[R75] 导出环境变量
来源：http://anx.c1oappe.top

export PATH="$HOME/bin:$PATH"
来源：http://hxn.yj202588.top

[R76] 使用临时文件
来源：http://ucj.vqdsnc.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hkw.ydzc1.top

[R77] 读取用户输入
来源：http://kky.kuanghao11.cn

read -rp "请输入: " ans
来源：http://cwo.jianghu66.top

[R78] 交互式菜单
来源：http://hwk.hcnkem.com

select opt in a b c; do echo "$opt"; break; done
来源：http://vei.hywenlv.cn

[R79] 解析命令行选项
来源：http://pju.jlsjyb.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://taz.meibo888.top

[R80] 查看脚本执行耗时
来源：http://brd.ivvv.top

time ./run.sh
来源：http://nim.gotoacloud.top

================================================================================
来源：http://pwa.kuanghao11.cn

S. C / C++ 专题
来源：http://gpm.daxiang520.top

================================================================================
来源：http://ypa.fzhhl.top

[S01] C：Hello World
来源：http://ygk.jiagoushi.top

#include <stdio.h>
来源：http://czy.yanxiufei.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://jii.hongshengwenyu.top

[S02] C：变量与格式化输出
来源：http://shb.aizwys.cn

int a = 10; printf("%d\n", a);
来源：http://ezi.dashuyun.cn

[S03] C：读入整数
来源：http://yjh.fehbvm.com

int x; scanf("%d", &x);
来源：http://gcj.ctjpmb.com

[S04] C：字符串复制
来源：http://iya.haohaochexian.top

char dst[32]; strcpy(dst, "hi");
来源：http://yym.aizwys.cn

[S05] C：字符串长度
来源：http://qur.zhiwuduotai.top

strlen(s)
来源：http://pgx.tanke756.top

[S06] C：字符串比较
来源：http://pcb.52xcode.cn

strcmp(a, b) == 0
来源：http://wlb.tanke756.top

[S07] C：数组遍历求和
来源：http://flo.jqgufenzy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zer.ppjwa.cn

[S08] C：动态内存分配与释放
来源：http://ewo.fanxiaobao.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sqd.fengsongda.top

[S09] C：结构体定义与初始化
来源：http://aqq.cdnleiting.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rcx.jyoumei.cn

[S10] C：指针与解引用
来源：http://rfz.wangdashe.top

int *p = &a;  *p = 5;
来源：http://gux.wangdashe.top

[S11] C：逐行读文件
来源：http://ant.sjlbkw.cn

FILE *f = fopen("a.txt", "r");
来源：http://ppz.bjfxy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://kmd.zhijiandao.cn

fclose(f);
来源：http://dsm.52xcode.cn

[S12] C：写文件
来源：http://qeo.tarul.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ykn.yonumen.top

[S13] C：宏定义
来源：http://dwi.tian-w.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://iot.sjlbkw.cn

[S14] C：枚举
来源：http://kiy.shanyushiyangtech.top

enum Color { RED, GREEN, BLUE };
来源：http://qdp.jlsjyb.cn

[S15] C：类型转换
来源：http://aco.hcnkem.com

(double) a / b
来源：http://scm.316326.xyz

[S16] C：位操作置位
来源：http://iix.zhixingplan.top

x |= (1 << 3);
来源：http://yxw.jiagoushi.top

[S17] C：安全拼接字符串
来源：http://lik.jiagoushi.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fhm.vqdsnc.cn

[S18] C：命令行参数
来源：http://qzk.yfazqb.com

int main(int argc, char **argv)
来源：http://ylk.tanke756.top

[S19] C：快速排序
来源：http://kzy.sysykeji.top

qsort(a, n, sizeof(int), cmp);
来源：http://owi.daxiang520.top

[S20] C：二分查找
来源：http://ips.dashuyun.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://csu.vehdjk.com

[S21] C：字符类别判断
来源：http://rqm.smart0.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://erb.mhx1999.top

[S22] C：字符串转数字
来源：http://lmg.sjlbkw.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ztu.yj20258.top

[S23] C：随机数
来源：http://rqd.zdbjq.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qcm.fktsv.cn

[S24] C：获取本地时间
来源：http://ntl.9152youxi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bot.fanxiaobao.xyz

[S25] C：内存拷贝
来源：http://xvg.zhijiandao.cn

memcpy(dst, src, n);
来源：http://asa.hnqzz.top

[S26] C：内存清零
来源：http://pbq.tianlin.xyz

memset(a, 0, sizeof a);
来源：http://xsj.jinyuanbaomall.cn

[S27] C：定义常量
来源：http://xkm.jianghu66.top

const double PI = 3.14159;
来源：http://iay.cucudq.cn

[S28] C：静态变量
来源：http://mpn.sxryk.cn

static int counter = 0;
来源：http://mrp.yonumen.top

[S29] C：变参函数
来源：http://pxc.sweek.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://asf.mhx1999.top

[S30] C：头文件保护
来源：http://sia.yj202588.top

#ifndef X_H
来源：http://pij.yongpay.top

#define X_H
来源：http://aiz.hnqzz.top

#endif
来源：http://cbr.jinqigfzy.top

[S31] C++：Hello World
来源：http://joq.aizwys.cn

#include <iostream>
来源：http://ffu.hongshengwenyu.top

int main() { std::cout << "Hello\n"; }
来源：http://xrr.cqqwz.cn

[S32] C++：字符串
来源：http://vws.hnxiangtu.top

std::string s = "hi";  s += "!";
来源：http://vgy.kuanghao11.cn

[S33] C++：vector 增删
来源：http://soy.ppjwa.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yfq.jinqigufen.top

[S34] C++：遍历 vector
来源：http://xgi.sxryk.cn

for (auto &x : v) { std::cout << x; }
来源：http://ecq.sjlbkw.cn

[S35] C++：map
来源：http://oth.tanke756.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://srp.cdnleiting.top

[S36] C++：unordered_map
来源：http://diy.guannengcc.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vzt.birdmap.top

[S37] C++：set
来源：http://zcu.hcnkem.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fyk.ctjpmb.com

[S38] C++：排序
来源：http://pnm.aizwys.cn

std::sort(v.begin(), v.end());
来源：http://mlf.redwolf501.top

[S39] C++：自定义比较器排序
来源：http://fqn.birdmap.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lhk.uphjek.com

[S40] C++：查找元素
来源：http://cpx.birdmap.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uds.hysaishi.cn

[S41] C++：类与构造函数
来源：http://rkt.mhx1999.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://uzn.yonumen.top

[S42] C++：继承与虚函数
来源：http://iiu.xylfe.cn

class B : public Base { public: void f() override {} };
来源：http://hsu.bbcook.cn

[S43] C++：智能指针
来源：http://kmp.dianchejie.cn

auto p = std::make_unique<int>(5);
来源：http://ncn.chenlongwang.top

[S44] C++：引用传参
来源：http://ozk.9152youxi.cn

void inc(int &x) { ++x; }
来源：http://mxi.sufxvd.cn

[S45] C++：lambda
来源：http://mww.xuetiantiany.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bqd.gzhubu.top

[S46] C++：函数模板
来源：http://psw.tanke756.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ibv.tianlin.xyz

[S47] C++：结构化绑定遍历
来源：http://gwi.jlsjyb.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://stw.sweek.top

[S48] C++：逐行读文件
来源：http://ckj.yueranfly.top

std::ifstream in("a.txt");  std::string line;
来源：http://nog.tarul.cn

while (std::getline(in, line)) { }
来源：http://prh.xuetiantiany.cn

[S49] C++：写文件
来源：http://yes.9152youxi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wmg.ywan-chungtsiang.top

[S50] C++：格式化数字
来源：http://nbv.sxryk.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kpx.hywenlv.cn

[S51] C++：显式类型转换
来源：http://nuj.zhengqikj.top

static_cast<double>(a) / b
来源：http://twu.yj20258888.top

[S52] C++：const 与 noexcept
来源：http://jfc.guowangkeji.top

int size() const noexcept { return n_; }
来源：http://ujf.mhx1999.top

[S53] C++：移动语义
来源：http://msg.jianghu66.top

std::vector<int> w = std::move(v);
来源：http://wrj.aizwys.cn

[S54] C++：异常处理
来源：http://qmk.cqqwz.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rch.ehwqpu.com

[S55] C++：结构化绑定
来源：http://rzh.chenlongwang.top

auto [a, b] = std::make_pair(1, 2);
来源：http://lwn.chenjidiqi.icu

[S56] C++：optional
来源：http://fqd.birdmap.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gfq.yuanzhike.top

[S57] C++：编译期常量
来源：http://pcd.birdmap.top

constexpr int N = 10;
来源：http://mmo.jinghuilouyu.cn

[S58] C++：命名空间
来源：http://pxb.iojbl.cn

namespace ns { int f() { return 1; } }
来源：http://qwt.sjlbkw.cn

[S59] C++：静态断言
来源：http://ojq.gzhubu.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ftt.chenzaomai.com

[S60] C++：遍历并删除元素
来源：http://wvs.sysykeji.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://aia.feifeiyinyue.top

================================================================================
来源：http://svf.andypj.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gxn.iojbl.cn

================================================================================
来源：http://fmq.cheryme.top

[T01] Kotlin：Hello World
来源：http://nmh.hfpthk.cn

println("Hello")
来源：http://wsn.smart0.xyz

[T02] Kotlin：变量
来源：http://szu.jqgfzy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jip.dashuyun.cn

[T03] Kotlin：字符串模板
来源：http://noi.nwbrower.top

"值: $b"
来源：http://zwe.ehwqpu.com

[T04] Kotlin：空安全
来源：http://nzc.zhixingplan.top

val n: String? = null;  n?.length
来源：http://eej.hnxiangtu.top

[T05] Kotlin：when 表达式
来源：http://rpz.cucudq.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://euk.cdnleiting.top

[T06] Kotlin：集合映射
来源：http://kcd.jqgufenzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://xco.zhoulong.xyz

[T07] Kotlin：集合过滤
来源：http://ath.chenjidiqi.icu

listOf(1, 2, 3).filter { it > 1 }
来源：http://tnf.hesvh.cn

[T08] Kotlin：数据类
来源：http://lfd.316326.xyz

data class User(val name: String, val age: Int)
来源：http://hkg.sjlbkw.cn

[T09] Kotlin：扩展函数
来源：http://yfw.xylfe.cn

fun String.exclaim() = this + "!"
来源：http://jan.yanxiufei.cn

[T10] Kotlin：默认参数
来源：http://dxj.yuanzhike.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ibq.vqdsnc.cn

[T11] Kotlin：协程
来源：http://qoz.hnqzz.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://pjx.epnwcf.com

[T12] Kotlin：解构声明
来源：http://owj.birdmap.top

val (a, b) = Pair(1, 2)
来源：http://irp.zhijiandao.cn

[T13] Kotlin：只读 Map
来源：http://sls.dashuyun.cn

val m = mapOf("a" to 1)
来源：http://yvm.cashguo.top

[T14] Kotlin：循环
来源：http://riz.gotoacloud.top

for (i in 1..10) println(i)
来源：http://btd.ydjk.org.cn

[T15] Kotlin：接口
来源：http://gmk.yfazqb.com

interface Shape { fun area(): Double }
来源：http://azs.dianchejie.cn

[T16] Swift：Hello World
来源：http://aho.sweek.top

print("Hello")
来源：http://yor.ppjwa.cn

[T17] Swift：变量与常量
来源：http://azg.vehdjk.com

var a = 1;  let b = 2
来源：http://zuc.sjlbkw.cn

[T18] Swift：字符串插值
来源：http://tbh.sysykeji.top

"值: \(b)"
来源：http://nho.hcnkem.com

[T19] Swift：可选绑定
来源：http://ovi.andypj.xyz

if let n = opt { print(n) }
来源：http://fiq.hnxiangtu.top

[T20] Swift：数组操作
来源：http://udj.fehbvm.com

var a = [1, 2, 3];  a.append(4)
来源：http://kln.daria6918.cn

[T21] Swift：遍历
来源：http://wrj.zhoulong.xyz

for x in a { print(x) }
来源：http://gvw.tianlin.xyz

[T22] Swift：字典
来源：http://fqw.fktsv.cn

var d = ["a": 1];  d["b"] = 2
来源：http://drz.yangfankeji.com

[T23] Swift：函数
来源：http://jpz.fengsongda.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tdx.jinqigufen.top

[T24] Swift：闭包
来源：http://cla.316326.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://vpb.wangshuangyany.cn

[T25] Swift：结构体
来源：http://vsq.yfazqb.com

struct P { var x: Int }
来源：http://eqb.uphjek.com

[T26] Swift：类与重写
来源：http://jej.ctjpmb.com

class A: Base { override func f() {} }
来源：http://ygc.hnxiangtu.top

[T27] Swift：错误处理
来源：http://paw.ywan-chungtsiang.top

do { try f() } catch { print(error) }
来源：http://nsr.mhx1999.top

[T28] Swift：枚举
来源：http://qnc.pycfn.com

enum Color { case red, green }
来源：http://oyr.hcnkem.com

[T29] Swift：guard 提前返回
来源：http://fla.zhixingplan.top

guard let x = opt else { return }
来源：http://mxa.jlsjyb.cn

[T30] Swift：协议
来源：http://cwf.gaohongyu789.top

protocol Shape { func area() -> Double }
来源：http://mmf.xylfe.cn

[T31] Lua：Hello World
来源：http://ctb.bbcook.cn

print("Hello")
来源：http://qzi.zhijiandao.cn

[T32] Lua：局部变量
来源：http://hss.vqdsnc.cn

local a = 1
来源：http://bmo.jyoumei.cn

[T33] Lua：表（数组）
来源：http://cir.shanyushiyangtech.top

local t = {1, 2, 3};  t[4] = 4
来源：http://gkf.yuanzhike.top

[T34] Lua：遍历表
来源：http://fox.xziqi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ocq.jinyuanbaomall.cn

[T35] Lua：字典表
来源：http://bho.yfazqb.com

local d = { a = 1 };  d.b = 2
来源：http://tfd.52xcode.cn

[T36] Lua：函数
来源：http://qoi.zycfv.cn

function add(a, b) return a + b end
来源：http://elb.aibaodan.cn

[T37] Lua：字符串拼接
来源：http://vhr.hcnkem.com

"a" .. "b"
来源：http://fkp.smart0.xyz

[T38] Lua：条件
来源：http://ddu.hammf.cn

if x > 0 then print("正") end
来源：http://cnm.meibo888.top

[T39] Lua：模式匹配
来源：http://fef.hfpthk.cn

string.find(s, "%d+")
来源：http://ohq.iojbl.cn

[T40] Lua：元表
来源：http://zjv.yj202588.top

setmetatable({}, { __index = base })
来源：http://oxu.hnqzz.top

[T41] Perl：Hello World
来源：http://qex.0kj1m.cn

print "Hello\n";
来源：http://mha.yuanzhike.top

[T42] Perl：变量类型
来源：http://bsn.sufxvd.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lsv.cucudq.cn

[T43] Perl：字符串插值
来源：http://ibb.cdnleiting.top

"值: $a"
来源：http://hif.nanxuanxn.top

[T44] Perl：条件
来源：http://fjv.wangshuangyany.cn

if ($a > 0) { print "正"; }
来源：http://mtw.dianchejie.cn

[T45] Perl：数组遍历
来源：http://ytc.hnxiangtu.top

for my $x (@arr) { print $x; }
来源：http://drm.chenzaomai.com

[T46] Perl：哈希操作
来源：http://nvr.tarul.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bks.shanyushiyangtech.top

[T47] Perl：正则捕获
来源：http://ovf.hfpthk.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://vsr.daxiang520.top

[T48] Perl：正则替换
来源：http://pff.smart0.xyz

$s =~ s/old/new/g;
来源：http://anc.wangdashe.top

[T49] Perl：函数
来源：http://dpc.quarkkingdee.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qkq.chenlongwang.top

[T50] Perl：逐行读文件
来源：http://vfm.cqqwz.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://dfi.hnqzz.top

while (my $line = <$fh>) { print $line; }
来源：http://mvd.shuidangran.top

[T51] Scala：Hello World
来源：http://cgj.hongshengwenyu.top

println("Hello")
来源：http://ztv.xinyue.icu

[T52] Scala：变量
来源：http://qhs.cqqwz.cn

val a = 1;  var b = 2
来源：http://msn.daxiang520.top

[T53] Scala：字符串插值
来源：http://ouq.vqdsnc.cn

s"值: $b"
来源：http://mgv.jqgufenzy.top

[T54] Scala：集合映射
来源：http://pgo.jlsjyb.cn

List(1, 2, 3).map(_ * 2)
来源：http://thr.hnxiangtu.top

[T55] Scala：集合过滤
来源：http://byv.ctjpmb.com

List(1, 2, 3).filter(_ > 1)
来源：http://ddr.jiagoushi.top

[T56] Scala：样例类
来源：http://wnh.shangyingyoupin.top

case class User(name: String, age: Int)
来源：http://edb.zhaomingkeji.xyz

[T57] Scala：模式匹配
来源：http://kzp.yj20258888.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://hof.zdbjq.cn

[T58] Scala：函数定义
来源：http://kcd.uphjek.com

def add(a: Int, b: Int): Int = a + b
来源：http://nsq.zhijiandao.cn

[T59] Scala：循环
来源：http://ptr.hnxiangtu.top

for (i <- 1 to 10) println(i)
来源：http://xnt.yangfankeji.com

[T60] Scala：折叠
来源：http://nbk.jinqigufen.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qjb.pycfn.com

================================================================================
来源：http://hpf.nanxuanxn.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://shs.gogol.net.cn

================================================================================
来源：http://swo.jqgfzy.top

[U01] Py：创建虚拟环境
来源：http://mhr.jiagoushi.top

python -m venv .venv && source .venv/bin/activate
来源：http://jsg.xziqi.cn

[U02] Py：导出 / 安装依赖
来源：http://kbp.bjfxy.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zrf.wangdashe.top


<!-- 参考信息 -->