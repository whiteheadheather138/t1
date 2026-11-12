代发 wailian999

ssh user@host 'uptime'
来源：http://pov.sweek.top

[R58] 下载文件
来源：http://hji.jinyuanbaomall.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nmu.c1oappe.top

[R59] 发 POST JSON
来源：http://lcd.mhx1999.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nib.xylfe.cn

[R60] 只看 HTTP 状态码
来源：http://fqt.pycfn.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hsf.zhoulong.xyz

[R61] 磁盘占用
来源：http://rsu.epnwcf.com

df -h;  du -sh *
来源：http://yua.zhijiandao.cn

[R62] 找最占空间的文件
来源：http://rnd.jiagoushi.top

du -ah . | sort -rh | head -10
来源：http://gih.wangdashe.top

[R63] 内存与进程
来源：http://nbf.birdmap.top

free -h;  ps aux | grep nginx
来源：http://tpr.nanxinkj.top

[R64] 结束进程
来源：http://end.nanxinkj.top

kill -9 $(pgrep -f app.py)
来源：http://sjb.0kj1m.cn

[R65] 查看端口占用
来源：http://loe.kuanghao11.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lfw.vqdsnc.cn

[R66] 定时任务
来源：http://tis.wangshuangyany.cn

crontab -e;  crontab -l
来源：http://ijq.yj20258.top

[R67] 生成随机十六进制串
来源：http://plo.sxryk.cn

openssl rand -hex 16
来源：http://rop.kuanghao11.cn

[R68] 计算文件校验值
来源：http://ead.birdmap.top

sha256sum a.txt;  md5sum a.txt
来源：http://qgm.pycfn.com

[R69] 生成随机密码
来源：http://wpz.jinghuilouyu.cn

head -c 16 /dev/urandom | base64
来源：http://uht.hywenlv.cn

[R70] 时间戳与互转
来源：http://sfq.cdnleiting.top

date +%s;  date -d @1700000000
来源：http://leu.ppjwa.cn

[R71] 日期格式化
来源：http://hgi.jqgufenzy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://xkk.nanxuanxn.top

[R72] 等待端口就绪
来源：http://xbc.dashuyun.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://puu.sufxvd.cn

[R73] 分割大日志
来源：http://umz.kuanghao11.cn

split -l 1000 big.log part_
来源：http://lqy.uphjek.com

[R74] 批量重命名
来源：http://tge.zhijiandao.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rny.tianlin.xyz

[R75] 导出环境变量
来源：http://cvd.jlsjyb.cn

export PATH="$HOME/bin:$PATH"
来源：http://ryp.nwbrower.top

[R76] 使用临时文件
来源：http://bdh.yuxming.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://umz.quarkkingdee.top

[R77] 读取用户输入
来源：http://mgv.zhongyouzk.top

read -rp "请输入: " ans
来源：http://via.yj20258888.top

[R78] 交互式菜单
来源：http://tdu.vqdsnc.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pnm.zdbjq.cn

[R79] 解析命令行选项
来源：http://rtq.shanyushiyangtech.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yca.daxiang520.top

[R80] 查看脚本执行耗时
来源：http://zwu.jinyuanbaomall.cn

time ./run.sh
来源：http://nkl.bbcook.cn

================================================================================
来源：http://mal.shzxlz.cn

S. C / C++ 专题
来源：http://fhc.zhongyouzk.top

================================================================================
来源：http://frx.xylfe.cn

[S01] C：Hello World
来源：http://qna.ehwqpu.com

#include <stdio.h>
来源：http://ksa.yanxiufei.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://jcc.aizwys.cn

[S02] C：变量与格式化输出
来源：http://ecu.cucudq.cn

int a = 10; printf("%d\n", a);
来源：http://jam.zhaomingkeji.xyz

[S03] C：读入整数
来源：http://hrs.chenlongwang.top

int x; scanf("%d", &x);
来源：http://qfw.gaohongyu789.top

[S04] C：字符串复制
来源：http://mtr.yongpay.top

char dst[32]; strcpy(dst, "hi");
来源：http://pmd.kuanghao11.cn

[S05] C：字符串长度
来源：http://eel.chenlongwang.top

strlen(s)
来源：http://jdz.jianghu66.top

[S06] C：字符串比较
来源：http://wmu.hfpthk.cn

strcmp(a, b) == 0
来源：http://uox.shuidangran.top

[S07] C：数组遍历求和
来源：http://emu.shanyushiyangkeji.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tle.316326.xyz

[S08] C：动态内存分配与释放
来源：http://wfy.zhixingplan.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://btk.haohaochexian.top

[S09] C：结构体定义与初始化
来源：http://ted.aibaodan.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uvy.snrcjt.cn

[S10] C：指针与解引用
来源：http://qme.9152youxi.cn

int *p = &a;  *p = 5;
来源：http://xbs.vqdsnc.cn

[S11] C：逐行读文件
来源：http://lyb.epnwcf.com

FILE *f = fopen("a.txt", "r");
来源：http://yzd.hywenlv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://jww.yj20258888.top

fclose(f);
来源：http://xgr.yj20258888.top

[S12] C：写文件
来源：http://tdz.ybcxt.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://eij.fehbvm.com

[S13] C：宏定义
来源：http://rej.yangfankeji.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hvi.epnwcf.com

[S14] C：枚举
来源：http://uej.sufxvd.cn

enum Color { RED, GREEN, BLUE };
来源：http://lto.yueranfly.top

[S15] C：类型转换
来源：http://ybp.ydzc1.top

(double) a / b
来源：http://jsd.haohaochexian.top

[S16] C：位操作置位
来源：http://vbw.chenlongwang.top

x |= (1 << 3);
来源：http://kmi.bjfxy.top

[S17] C：安全拼接字符串
来源：http://cbg.uphjek.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nwj.jlsjyb.cn

[S18] C：命令行参数
来源：http://yhq.yongpay.top

int main(int argc, char **argv)
来源：http://efc.nanxuanxn.top

[S19] C：快速排序
来源：http://wri.jinghuilouyu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://mev.jinqigufen.top

[S20] C：二分查找
来源：http://gcq.c1oappe.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pvx.chenjidiqi.icu

[S21] C：字符类别判断
来源：http://eio.shanyushiyangkeji.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ewo.bjfxy.top

[S22] C：字符串转数字
来源：http://aak.vqdsnc.cn

atoi("42");  strtod("3.14", NULL);
来源：http://mxg.hnxiangtu.top

[S23] C：随机数
来源：http://gpr.jqgufenzy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://rsa.guannengcc.top

[S24] C：获取本地时间
来源：http://tki.havefunace.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ftc.redwolf501.top

[S25] C：内存拷贝
来源：http://bku.tian-w.cn

memcpy(dst, src, n);
来源：http://ubv.jianghu66.top

[S26] C：内存清零
来源：http://fug.xuanzx.com

memset(a, 0, sizeof a);
来源：http://qex.wangdashe.top

[S27] C：定义常量
来源：http://nne.bjfxy.top

const double PI = 3.14159;
来源：http://tky.chenzaomai.com

[S28] C：静态变量
来源：http://glq.daria6918.cn

static int counter = 0;
来源：http://fzu.zhiwuduotai.top

[S29] C：变参函数
来源：http://dsz.hysaishi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ahb.yj20258.top

[S30] C：头文件保护
来源：http://qpt.zhongyouzk.top

#ifndef X_H
来源：http://wue.chenlongwang.top

#define X_H
来源：http://xzz.yuanzhike.top

#endif
来源：http://maf.yonumen.top

[S31] C++：Hello World
来源：http://xhd.fktsv.cn

#include <iostream>
来源：http://kec.guowangkeji.top

int main() { std::cout << "Hello\n"; }
来源：http://kku.ybcxt.top

[S32] C++：字符串
来源：http://vfo.birdmap.top

std::string s = "hi";  s += "!";
来源：http://oei.fengsongda.top

[S33] C++：vector 增删
来源：http://iye.hammf.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jld.jqgfzy.top

[S34] C++：遍历 vector
来源：http://yqd.cdnleiting.top

for (auto &x : v) { std::cout << x; }
来源：http://xvg.shzxlz.cn

[S35] C++：map
来源：http://hxv.guowangkeji.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ezz.yangfankeji.com

[S36] C++：unordered_map
来源：http://otj.vehdjk.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://opb.9152youxi.cn

[S37] C++：set
来源：http://bsa.fzhhl.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://szm.gaohongyu789.top

[S38] C++：排序
来源：http://mem.hesvh.cn

std::sort(v.begin(), v.end());
来源：http://uww.bjfxy.top

[S39] C++：自定义比较器排序
来源：http://fdh.zdbjq.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jzj.hongshengwenyu.top

[S40] C++：查找元素
来源：http://ubn.quarkkingdee.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gub.jianghu66.top

[S41] C++：类与构造函数
来源：http://ckz.hfpthk.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lhn.dashuyun.cn

[S42] C++：继承与虚函数
来源：http://sxq.gotoacloud.top

class B : public Base { public: void f() override {} };
来源：http://ghe.cqqwz.cn

[S43] C++：智能指针
来源：http://rzr.snrcjt.cn

auto p = std::make_unique<int>(5);
来源：http://kkh.birdmap.top

[S44] C++：引用传参
来源：http://aoz.316326.xyz

void inc(int &x) { ++x; }
来源：http://yzp.shangyingyoupin.top

[S45] C++：lambda
来源：http://ecz.0kj1m.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qrk.bjfxy.top

[S46] C++：函数模板
来源：http://ckx.shanyushiyangtech.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dwm.feifeiyinyue.top

[S47] C++：结构化绑定遍历
来源：http://ojb.sjlbkw.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://use.zdbjq.cn

[S48] C++：逐行读文件
来源：http://wat.hfpthk.cn

std::ifstream in("a.txt");  std::string line;
来源：http://yrr.vqdsnc.cn

while (std::getline(in, line)) { }
来源：http://ahk.yangfankeji.com

[S49] C++：写文件
来源：http://bwj.xingfuxueyuan.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ebi.jqgufenzy.top

[S50] C++：格式化数字
来源：http://jdx.c1oappe.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ovv.cashguo.top

[S51] C++：显式类型转换
来源：http://uyu.jinghuilouyu.cn

static_cast<double>(a) / b
来源：http://elx.ivvv.top

[S52] C++：const 与 noexcept
来源：http://fvf.hysaishi.cn

int size() const noexcept { return n_; }
来源：http://ewf.bjfxy.top

[S53] C++：移动语义
来源：http://pnj.snrcjt.cn

std::vector<int> w = std::move(v);
来源：http://pby.hysaishi.cn

[S54] C++：异常处理
来源：http://hyk.gogol.net.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xcv.shanyushiyangtech.top

[S55] C++：结构化绑定
来源：http://wzr.zhiwuduotai.top

auto [a, b] = std::make_pair(1, 2);
来源：http://dkt.jinyuanbaomall.cn

[S56] C++：optional
来源：http://prb.hfpthk.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ues.zdbjq.cn

[S57] C++：编译期常量
来源：http://xvq.wangshuangyany.cn

constexpr int N = 10;
来源：http://qpb.cucudq.cn

[S58] C++：命名空间
来源：http://mze.jinqigfzy.top

namespace ns { int f() { return 1; } }
来源：http://dmv.epnwcf.com

[S59] C++：静态断言
来源：http://wry.cucudq.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://omw.ivvv.top

[S60] C++：遍历并删除元素
来源：http://wet.birdmap.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gzx.ybcxt.top

================================================================================
来源：http://cki.zdbjq.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dgo.redwolf501.top

================================================================================
来源：http://zta.ydjk.org.cn

[T01] Kotlin：Hello World
来源：http://foo.guannengcc.top

println("Hello")
来源：http://nyi.aibaodan.cn

[T02] Kotlin：变量
来源：http://yrz.yonumen.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://exw.zhengqikj.top

[T03] Kotlin：字符串模板
来源：http://qkc.hesvh.cn

"值: $b"
来源：http://eye.daria6918.cn

[T04] Kotlin：空安全
来源：http://fmm.tian-w.cn

val n: String? = null;  n?.length
来源：http://luc.yj202588.top

[T05] Kotlin：when 表达式
来源：http://xwd.tarul.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nas.svipenyu.cn

[T06] Kotlin：集合映射
来源：http://oxx.ehwqpu.com

listOf(1, 2, 3).map { it * 2 }
来源：http://vvw.jinqigufen.top

[T07] Kotlin：集合过滤
来源：http://tii.zhaomingkeji.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://mio.zhengqikj.top

[T08] Kotlin：数据类
来源：http://szl.gogol.net.cn

data class User(val name: String, val age: Int)
来源：http://vdo.zhaomingkeji.xyz

[T09] Kotlin：扩展函数
来源：http://cqm.tanke756.top

fun String.exclaim() = this + "!"
来源：http://zah.nanxuanxn.top

[T10] Kotlin：默认参数
来源：http://pwg.shangyingyoupin.top

fun greet(name: String = "World") = "Hi $name"
来源：http://epg.zhoulong.xyz

[T11] Kotlin：协程
来源：http://fyz.yonumen.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ibj.cashguo.top

[T12] Kotlin：解构声明
来源：http://yxl.fzhhl.top

val (a, b) = Pair(1, 2)
来源：http://nut.ywan-chungtsiang.top

[T13] Kotlin：只读 Map
来源：http://res.jyoumei.cn

val m = mapOf("a" to 1)
来源：http://sde.nanxuanxn.top

[T14] Kotlin：循环
来源：http://pin.9152youxi.cn

for (i in 1..10) println(i)
来源：http://pcb.zhijiandao.cn

[T15] Kotlin：接口
来源：http://xid.shangyingyoupin.top

interface Shape { fun area(): Double }
来源：http://ebx.316326.xyz

[T16] Swift：Hello World
来源：http://sff.cqqwz.cn

print("Hello")
来源：http://qks.sxryk.cn

[T17] Swift：变量与常量
来源：http://zqu.zhixingplan.top

var a = 1;  let b = 2
来源：http://col.zdbjq.cn

[T18] Swift：字符串插值
来源：http://qtg.smart0.xyz

"值: \(b)"
来源：http://mxb.9152youxi.cn

[T19] Swift：可选绑定
来源：http://hiq.kuanghao11.cn

if let n = opt { print(n) }
来源：http://kpy.sysykeji.top

[T20] Swift：数组操作
来源：http://uby.smart0.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://rsr.hammf.cn

[T21] Swift：遍历
来源：http://wxb.cashguo.top

for x in a { print(x) }
来源：http://tvc.jqgufenzy.top

[T22] Swift：字典
来源：http://zsp.fehbvm.com

var d = ["a": 1];  d["b"] = 2
来源：http://fdu.aizwys.cn

[T23] Swift：函数
来源：http://avd.gaohongyu789.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lxi.hcnkem.com

[T24] Swift：闭包
来源：http://obp.shzxlz.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://rth.yuanzhike.top

[T25] Swift：结构体
来源：http://qpe.zhoulong.xyz

struct P { var x: Int }
来源：http://gxs.tanke756.top

[T26] Swift：类与重写
来源：http://ncv.chenlongwang.top

class A: Base { override func f() {} }
来源：http://kti.smart0.xyz

[T27] Swift：错误处理
来源：http://yud.mhx1999.top

do { try f() } catch { print(error) }
来源：http://uqp.meibo888.top

[T28] Swift：枚举
来源：http://dmg.jiagoushi.top

enum Color { case red, green }
来源：http://hcj.yongpay.top

[T29] Swift：guard 提前返回
来源：http://yop.c1oappe.top

guard let x = opt else { return }
来源：http://faa.hywenlv.cn

[T30] Swift：协议
来源：http://jrx.tian-w.cn

protocol Shape { func area() -> Double }
来源：http://huj.gaohongyu789.top

[T31] Lua：Hello World
来源：http://hbq.kuanghao11.cn

print("Hello")
来源：http://hdp.yueranfly.top

[T32] Lua：局部变量
来源：http://ukt.cdnleiting.top

local a = 1
来源：http://egi.gzhubu.top

[T33] Lua：表（数组）
来源：http://gii.gaohongyu789.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ocg.hesvh.cn

[T34] Lua：遍历表
来源：http://nph.ehwqpu.com

for i, v in ipairs(t) do print(i, v) end
来源：http://som.gzhubu.top

[T35] Lua：字典表
来源：http://rsc.sweek.top

local d = { a = 1 };  d.b = 2
来源：http://bmo.ywan-chungtsiang.top

[T36] Lua：函数
来源：http://xtu.0kj1m.cn

function add(a, b) return a + b end
来源：http://xat.redwolf501.top

[T37] Lua：字符串拼接
来源：http://hzu.ppjwa.cn

"a" .. "b"
来源：http://jbs.yonumen.top

[T38] Lua：条件
来源：http://uts.chenlongwang.top

if x > 0 then print("正") end
来源：http://ajp.yfazqb.com

[T39] Lua：模式匹配
来源：http://jnd.pycfn.com

string.find(s, "%d+")
来源：http://wkg.52xcode.cn

[T40] Lua：元表
来源：http://qld.birdmap.top

setmetatable({}, { __index = base })
来源：http://qcm.xinyue.icu

[T41] Perl：Hello World
来源：http://day.sxryk.cn

print "Hello\n";
来源：http://cni.yvedp.cn

[T42] Perl：变量类型
来源：http://rjy.ctjpmb.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xsq.iojbl.cn

[T43] Perl：字符串插值
来源：http://pus.nwbrower.top

"值: $a"
来源：http://nqe.xinyue.icu

[T44] Perl：条件
来源：http://xbl.zhongyouzk.top

if ($a > 0) { print "正"; }
来源：http://cbp.gotoacloud.top

[T45] Perl：数组遍历
来源：http://xdu.daria6918.cn

for my $x (@arr) { print $x; }
来源：http://cal.jianghu66.top

[T46] Perl：哈希操作
来源：http://kqr.yangfankeji.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nsv.chenjidiqi.icu

[T47] Perl：正则捕获
来源：http://wuq.cheryme.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://fal.zdbjq.cn

[T48] Perl：正则替换
来源：http://lai.gzhubu.top

$s =~ s/old/new/g;
来源：http://lmr.xziqi.cn

[T49] Perl：函数
来源：http://zca.9152youxi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://avh.gogol.net.cn

[T50] Perl：逐行读文件
来源：http://hnb.quarkkingdee.top

open my $fh, "<", "a.txt" or die $!;
来源：http://hiz.yuanzhike.top

while (my $line = <$fh>) { print $line; }
来源：http://mkn.zhongyouzk.top

[T51] Scala：Hello World
来源：http://nmv.9152youxi.cn

println("Hello")
来源：http://ecu.yj20258888.top

[T52] Scala：变量
来源：http://ofz.gzhubu.top

val a = 1;  var b = 2
来源：http://del.yvedp.cn

[T53] Scala：字符串插值
来源：http://igs.pycfn.com

s"值: $b"
来源：http://dpb.havefunace.top

[T54] Scala：集合映射
来源：http://nwu.316326.xyz

List(1, 2, 3).map(_ * 2)
来源：http://yrt.ivvv.top

[T55] Scala：集合过滤
来源：http://bos.havefunace.top

List(1, 2, 3).filter(_ > 1)
来源：http://fag.fzhhl.top

[T56] Scala：样例类
来源：http://tyg.yangfankeji.com

case class User(name: String, age: Int)
来源：http://qho.yj20258888.top

[T57] Scala：模式匹配
来源：http://lry.daxiang520.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://dcy.ehwqpu.com

[T58] Scala：函数定义
来源：http://lwo.cheryme.top

def add(a: Int, b: Int): Int = a + b
来源：http://eey.ydzc1.top

[T59] Scala：循环
来源：http://yzn.ywan-chungtsiang.top

for (i <- 1 to 10) println(i)
来源：http://nod.haohaochexian.top

[T60] Scala：折叠
来源：http://bqj.ybcxt.top


<!-- 参考信息 -->