代发 wailian999

ssh user@host 'uptime'
来源：http://dpc.sjlbkw.cn

[R58] 下载文件
来源：http://ymx.gzhubu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qzk.chenzaomai.com

[R59] 发 POST JSON
来源：http://fcu.cheryme.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zvw.shanyushiyangtech.top

[R60] 只看 HTTP 状态码
来源：http://jwu.yj20258.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zzb.ybcxt.top

[R61] 磁盘占用
来源：http://buu.hfpthk.cn

df -h;  du -sh *
来源：http://bfg.snrcjt.cn

[R62] 找最占空间的文件
来源：http://dzf.hcnkem.com

du -ah . | sort -rh | head -10
来源：http://vwx.kuanghao11.cn

[R63] 内存与进程
来源：http://reu.cashguo.top

free -h;  ps aux | grep nginx
来源：http://hqi.xingfuxueyuan.xyz

[R64] 结束进程
来源：http://vrr.hcnkem.com

kill -9 $(pgrep -f app.py)
来源：http://mgw.hammf.cn

[R65] 查看端口占用
来源：http://wjs.zhaomingkeji.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kkb.cheryme.top

[R66] 定时任务
来源：http://ivr.tarul.cn

crontab -e;  crontab -l
来源：http://aol.fzhhl.top

[R67] 生成随机十六进制串
来源：http://vpz.epnwcf.com

openssl rand -hex 16
来源：http://wgg.sysykeji.top

[R68] 计算文件校验值
来源：http://lui.uphjek.com

sha256sum a.txt;  md5sum a.txt
来源：http://wob.ivvv.top

[R69] 生成随机密码
来源：http://raw.cdnleiting.top

head -c 16 /dev/urandom | base64
来源：http://mip.yj20258.top

[R70] 时间戳与互转
来源：http://xjy.jinghuilouyu.cn

date +%s;  date -d @1700000000
来源：http://mgr.fengsongda.top

[R71] 日期格式化
来源：http://tsr.yfazqb.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://byc.aizwys.cn

[R72] 等待端口就绪
来源：http://hwf.zhengqikj.top

until nc -z localhost 3306; do sleep 1; done
来源：http://fmi.ehwqpu.com

[R73] 分割大日志
来源：http://tkv.yuxming.cn

split -l 1000 big.log part_
来源：http://ocg.cashguo.top

[R74] 批量重命名
来源：http://hzp.dashuyun.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dsx.cucudq.cn

[R75] 导出环境变量
来源：http://ocw.tarul.cn

export PATH="$HOME/bin:$PATH"
来源：http://gak.sjlbkw.cn

[R76] 使用临时文件
来源：http://lur.zhaomingkeji.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vbu.zhiwuduotai.top

[R77] 读取用户输入
来源：http://ngx.xinyue.icu

read -rp "请输入: " ans
来源：http://rfn.ywan-chungtsiang.top

[R78] 交互式菜单
来源：http://vfg.zhengqikj.top

select opt in a b c; do echo "$opt"; break; done
来源：http://rsg.sysykeji.top

[R79] 解析命令行选项
来源：http://cpk.zhijiandao.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dpg.vehdjk.com

[R80] 查看脚本执行耗时
来源：http://qam.jinghuilouyu.cn

time ./run.sh
来源：http://ikf.fengsongda.top

================================================================================
来源：http://jvw.bbcook.cn

S. C / C++ 专题
来源：http://atu.fanxiaobao.xyz

================================================================================
来源：http://zzn.yj20258888.top

[S01] C：Hello World
来源：http://bck.sweek.top

#include <stdio.h>
来源：http://eap.jqgfzy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://bfh.iojbl.cn

[S02] C：变量与格式化输出
来源：http://vxu.nwbrower.top

int a = 10; printf("%d\n", a);
来源：http://fki.nanxuanxn.top

[S03] C：读入整数
来源：http://mxd.guannengcc.top

int x; scanf("%d", &x);
来源：http://zbj.yonumen.top

[S04] C：字符串复制
来源：http://icr.fzhhl.top

char dst[32]; strcpy(dst, "hi");
来源：http://noe.andypj.xyz

[S05] C：字符串长度
来源：http://lti.chenzaomai.com

strlen(s)
来源：http://iox.gzhubu.top

[S06] C：字符串比较
来源：http://yoi.yj20258.top

strcmp(a, b) == 0
来源：http://kbu.yuanzhike.top

[S07] C：数组遍历求和
来源：http://xiy.fehbvm.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ild.52xcode.cn

[S08] C：动态内存分配与释放
来源：http://nlc.jlsjyb.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vmf.mhx1999.top

[S09] C：结构体定义与初始化
来源：http://wgj.nanxuanxn.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vef.guowangkeji.top

[S10] C：指针与解引用
来源：http://ocq.mhx1999.top

int *p = &a;  *p = 5;
来源：http://bgq.ydjk.org.cn

[S11] C：逐行读文件
来源：http://jjd.birdmap.top

FILE *f = fopen("a.txt", "r");
来源：http://dpj.gogol.net.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zmi.zycfv.cn

fclose(f);
来源：http://ipn.tian-w.cn

[S12] C：写文件
来源：http://kmz.guannengcc.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dgv.hcnkem.com

[S13] C：宏定义
来源：http://bir.0kj1m.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qai.hammf.cn

[S14] C：枚举
来源：http://kxy.yonumen.top

enum Color { RED, GREEN, BLUE };
来源：http://pcw.jinyuanbaomall.cn

[S15] C：类型转换
来源：http://bde.9152youxi.cn

(double) a / b
来源：http://dui.mhx1999.top

[S16] C：位操作置位
来源：http://xpo.zhengqikj.top

x |= (1 << 3);
来源：http://kiu.nanxinkj.top

[S17] C：安全拼接字符串
来源：http://jix.feifeiyinyue.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ion.xylfe.cn

[S18] C：命令行参数
来源：http://txh.hnxiangtu.top

int main(int argc, char **argv)
来源：http://twr.shanyushiyangkeji.top

[S19] C：快速排序
来源：http://znl.316326.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://vcp.52xcode.cn

[S20] C：二分查找
来源：http://lud.epnwcf.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bnd.kuanghao11.cn

[S21] C：字符类别判断
来源：http://kjc.zhiwuduotai.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wkx.gotoacloud.top

[S22] C：字符串转数字
来源：http://thj.vehdjk.com

atoi("42");  strtod("3.14", NULL);
来源：http://jns.smart0.xyz

[S23] C：随机数
来源：http://mkb.chenzaomai.com

srand(time(NULL));  int r = rand() % 100;
来源：http://lrc.cdnleiting.top

[S24] C：获取本地时间
来源：http://djr.feifeiyinyue.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cmx.jinyuanbaomall.cn

[S25] C：内存拷贝
来源：http://chs.zhixingplan.top

memcpy(dst, src, n);
来源：http://enh.jiagoushi.top

[S26] C：内存清零
来源：http://vij.jianghu66.top

memset(a, 0, sizeof a);
来源：http://ufo.hesvh.cn

[S27] C：定义常量
来源：http://fxz.yanxiufei.cn

const double PI = 3.14159;
来源：http://poa.aibaodan.cn

[S28] C：静态变量
来源：http://jau.dianchejie.cn

static int counter = 0;
来源：http://hph.yj20258888.top

[S29] C：变参函数
来源：http://yrc.chenzaomai.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kxx.jinqigfzy.top

[S30] C：头文件保护
来源：http://mru.xuetiantiany.cn

#ifndef X_H
来源：http://jhs.52xcode.cn

#define X_H
来源：http://gvl.yongpay.top

#endif
来源：http://wye.sxryk.cn

[S31] C++：Hello World
来源：http://ehx.jinghuilouyu.cn

#include <iostream>
来源：http://dlc.hesvh.cn

int main() { std::cout << "Hello\n"; }
来源：http://ftj.aibaodan.cn

[S32] C++：字符串
来源：http://cvt.yangfankeji.com

std::string s = "hi";  s += "!";
来源：http://wke.c1oappe.top

[S33] C++：vector 增删
来源：http://aqc.nwbrower.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lll.xuetiantiany.cn

[S34] C++：遍历 vector
来源：http://crg.cashguo.top

for (auto &x : v) { std::cout << x; }
来源：http://idz.tanke756.top

[S35] C++：map
来源：http://xpw.cdnleiting.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hrx.ppjwa.cn

[S36] C++：unordered_map
来源：http://lmn.cashguo.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xfb.xuanzx.com

[S37] C++：set
来源：http://vrx.fzhhl.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lvk.316326.xyz

[S38] C++：排序
来源：http://cgl.pengpengdd.cyou

std::sort(v.begin(), v.end());
来源：http://gcl.fktsv.cn

[S39] C++：自定义比较器排序
来源：http://bwu.pycfn.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dwy.zhiwuduotai.top

[S40] C++：查找元素
来源：http://cfr.ctjpmb.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qxd.bbcook.cn

[S41] C++：类与构造函数
来源：http://qro.tanke756.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zyo.fengsongda.top

[S42] C++：继承与虚函数
来源：http://mxv.tianlin.xyz

class B : public Base { public: void f() override {} };
来源：http://ndz.iojbl.cn

[S43] C++：智能指针
来源：http://omt.birdmap.top

auto p = std::make_unique<int>(5);
来源：http://qqu.zhengqikj.top

[S44] C++：引用传参
来源：http://pok.xinyue.icu

void inc(int &x) { ++x; }
来源：http://ucr.sysykeji.top

[S45] C++：lambda
来源：http://aou.hnqzz.top

auto add = [](int a, int b) { return a + b; };
来源：http://gok.sweek.top

[S46] C++：函数模板
来源：http://cfu.jinyuanbaomall.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jlw.shanyushiyangkeji.top

[S47] C++：结构化绑定遍历
来源：http://txu.zdqjudy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://scv.daxiang520.top

[S48] C++：逐行读文件
来源：http://mii.zhoulong.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://qgz.tarul.cn

while (std::getline(in, line)) { }
来源：http://ufu.zhengqikj.top

[S49] C++：写文件
来源：http://dox.zycfv.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ikm.sjlbkw.cn

[S50] C++：格式化数字
来源：http://asa.xinyue.icu

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mxo.yj202588.top

[S51] C++：显式类型转换
来源：http://dbt.gotoacloud.top

static_cast<double>(a) / b
来源：http://vvw.chenjidiqi.icu

[S52] C++：const 与 noexcept
来源：http://ath.shuidangran.top

int size() const noexcept { return n_; }
来源：http://ekw.yvedp.cn

[S53] C++：移动语义
来源：http://kmw.wangshuangyany.cn

std::vector<int> w = std::move(v);
来源：http://bjz.jiagoushi.top

[S54] C++：异常处理
来源：http://quy.xylfe.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qht.zhiwuduotai.top

[S55] C++：结构化绑定
来源：http://mnw.chenjidiqi.icu

auto [a, b] = std::make_pair(1, 2);
来源：http://zuq.daxiang520.top

[S56] C++：optional
来源：http://omk.shanyushiyangkeji.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lpx.bbcook.cn

[S57] C++：编译期常量
来源：http://sdm.birdmap.top

constexpr int N = 10;
来源：http://oxh.yanxiufei.cn

[S58] C++：命名空间
来源：http://rtn.vehdjk.com

namespace ns { int f() { return 1; } }
来源：http://mjr.vehdjk.com

[S59] C++：静态断言
来源：http://fqu.jqgfzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zgk.hnqzz.top

[S60] C++：遍历并删除元素
来源：http://bau.svipenyu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://etm.gaohongyu789.top

================================================================================
来源：http://bfh.sufxvd.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gxx.ehwqpu.com

================================================================================
来源：http://dur.zhoulong.xyz

[T01] Kotlin：Hello World
来源：http://mum.sweek.top

println("Hello")
来源：http://pyq.zhoulong.xyz

[T02] Kotlin：变量
来源：http://gqk.aizwys.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ssd.hcnkem.com

[T03] Kotlin：字符串模板
来源：http://imm.cheryme.top

"值: $b"
来源：http://jzw.sysykeji.top

[T04] Kotlin：空安全
来源：http://wgg.mhx1999.top

val n: String? = null;  n?.length
来源：http://yak.shuidangran.top

[T05] Kotlin：when 表达式
来源：http://eag.ehwqpu.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lnx.mhx1999.top

[T06] Kotlin：集合映射
来源：http://zaj.redwolf501.top

listOf(1, 2, 3).map { it * 2 }
来源：http://bdx.daria6918.cn

[T07] Kotlin：集合过滤
来源：http://dou.shanyushiyangtech.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://qcm.zhiwuduotai.top

[T08] Kotlin：数据类
来源：http://nil.guowangkeji.top

data class User(val name: String, val age: Int)
来源：http://tan.aibaodan.cn

[T09] Kotlin：扩展函数
来源：http://pjv.yfazqb.com

fun String.exclaim() = this + "!"
来源：http://oyw.shanyushiyangtech.top

[T10] Kotlin：默认参数
来源：http://qkx.pycfn.com

fun greet(name: String = "World") = "Hi $name"
来源：http://dbn.yongpay.top

[T11] Kotlin：协程
来源：http://kco.cqqwz.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qdl.jqgufenzy.top

[T12] Kotlin：解构声明
来源：http://sfv.yangfankeji.com

val (a, b) = Pair(1, 2)
来源：http://pvu.aibaodan.cn

[T13] Kotlin：只读 Map
来源：http://wkq.zhongyouzk.top

val m = mapOf("a" to 1)
来源：http://ost.wangdashe.top

[T14] Kotlin：循环
来源：http://xgt.ydjk.org.cn

for (i in 1..10) println(i)
来源：http://zff.chenjidiqi.icu

[T15] Kotlin：接口
来源：http://ofk.yj20258888.top

interface Shape { fun area(): Double }
来源：http://gwf.yuanzhike.top

[T16] Swift：Hello World
来源：http://jgn.vehdjk.com

print("Hello")
来源：http://ikb.uphjek.com

[T17] Swift：变量与常量
来源：http://vep.gzhubu.top

var a = 1;  let b = 2
来源：http://vqj.cashguo.top

[T18] Swift：字符串插值
来源：http://zpc.ctjpmb.com

"值: \(b)"
来源：http://rkw.nanxinkj.top

[T19] Swift：可选绑定
来源：http://ujx.xuanzx.com

if let n = opt { print(n) }
来源：http://qnm.jqgfzy.top

[T20] Swift：数组操作
来源：http://gfr.zhoulong.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://kgd.kuanghao11.cn

[T21] Swift：遍历
来源：http://cdx.fengsongda.top

for x in a { print(x) }
来源：http://gwm.sufxvd.cn

[T22] Swift：字典
来源：http://lrg.hcnkem.com

var d = ["a": 1];  d["b"] = 2
来源：http://suv.jlsjyb.cn

[T23] Swift：函数
来源：http://zbs.bbcook.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zcp.fzhhl.top

[T24] Swift：闭包
来源：http://cfj.dashuyun.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gdk.yuanzhike.top

[T25] Swift：结构体
来源：http://qws.hesvh.cn

struct P { var x: Int }
来源：http://syk.zhijiandao.cn

[T26] Swift：类与重写
来源：http://yuq.nanxinkj.top

class A: Base { override func f() {} }
来源：http://ahk.tianlin.xyz

[T27] Swift：错误处理
来源：http://jqp.zhijiandao.cn

do { try f() } catch { print(error) }
来源：http://xzg.cucudq.cn

[T28] Swift：枚举
来源：http://yap.daria6918.cn

enum Color { case red, green }
来源：http://tmg.shuidangran.top

[T29] Swift：guard 提前返回
来源：http://rar.hysaishi.cn

guard let x = opt else { return }
来源：http://wuy.sufxvd.cn

[T30] Swift：协议
来源：http://jlu.sjlbkw.cn

protocol Shape { func area() -> Double }
来源：http://pfu.zhijiandao.cn

[T31] Lua：Hello World
来源：http://ipw.kuanghao11.cn

print("Hello")
来源：http://hdb.gaohongyu789.top

[T32] Lua：局部变量
来源：http://dot.zhengqikj.top

local a = 1
来源：http://lvv.ctjpmb.com

[T33] Lua：表（数组）
来源：http://tsk.xuanzx.com

local t = {1, 2, 3};  t[4] = 4
来源：http://xcd.bbcook.cn

[T34] Lua：遍历表
来源：http://tyg.zhengqikj.top

for i, v in ipairs(t) do print(i, v) end
来源：http://tzu.shuidangran.top

[T35] Lua：字典表
来源：http://wpp.pengpengdd.cyou

local d = { a = 1 };  d.b = 2
来源：http://ehj.aibaodan.cn

[T36] Lua：函数
来源：http://kwq.aizwys.cn

function add(a, b) return a + b end
来源：http://emb.9152youxi.cn

[T37] Lua：字符串拼接
来源：http://srt.pengpengdd.cyou

"a" .. "b"
来源：http://umf.jinyuanbaomall.cn

[T38] Lua：条件
来源：http://tsn.uphjek.com

if x > 0 then print("正") end
来源：http://phn.yj20258888.top

[T39] Lua：模式匹配
来源：http://umt.zhongyouzk.top

string.find(s, "%d+")
来源：http://dds.nwbrower.top

[T40] Lua：元表
来源：http://uzq.aibaodan.cn

setmetatable({}, { __index = base })
来源：http://nhh.haohaochexian.top

[T41] Perl：Hello World
来源：http://syr.tian-w.cn

print "Hello\n";
来源：http://tlm.cqqwz.cn

[T42] Perl：变量类型
来源：http://zdz.feifeiyinyue.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gzx.bbcook.cn

[T43] Perl：字符串插值
来源：http://ndh.epnwcf.com

"值: $a"
来源：http://uci.shanyushiyangtech.top

[T44] Perl：条件
来源：http://jzx.guowangkeji.top

if ($a > 0) { print "正"; }
来源：http://aeg.dianchejie.cn

[T45] Perl：数组遍历
来源：http://ldx.yongpay.top

for my $x (@arr) { print $x; }
来源：http://zbs.ehwqpu.com

[T46] Perl：哈希操作
来源：http://rps.yueranfly.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cvs.pycfn.com

[T47] Perl：正则捕获
来源：http://rjo.aibaodan.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://any.hesvh.cn

[T48] Perl：正则替换
来源：http://fyb.kuanghao11.cn

$s =~ s/old/new/g;
来源：http://bcc.iojbl.cn

[T49] Perl：函数
来源：http://kpr.redwolf501.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gox.shanyushiyangtech.top

[T50] Perl：逐行读文件
来源：http://krn.9152youxi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ynx.jiagoushi.top

while (my $line = <$fh>) { print $line; }
来源：http://gsc.xinyue.icu

[T51] Scala：Hello World
来源：http://hfw.jinqigfzy.top

println("Hello")
来源：http://oii.shangyingyoupin.top

[T52] Scala：变量
来源：http://wvo.tian-w.cn

val a = 1;  var b = 2
来源：http://nrk.316326.xyz

[T53] Scala：字符串插值
来源：http://jdc.sysykeji.top

s"值: $b"
来源：http://ulh.zhoulong.xyz

[T54] Scala：集合映射
来源：http://gul.ydjk.org.cn

List(1, 2, 3).map(_ * 2)
来源：http://cah.sysykeji.top

[T55] Scala：集合过滤
来源：http://clk.bjfxy.top

List(1, 2, 3).filter(_ > 1)
来源：http://tkw.hnqzz.top

[T56] Scala：样例类
来源：http://snx.xziqi.cn

case class User(name: String, age: Int)
来源：http://hdu.sufxvd.cn

[T57] Scala：模式匹配
来源：http://gkn.sjlbkw.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vwu.vehdjk.com

[T58] Scala：函数定义
来源：http://axo.cashguo.top

def add(a: Int, b: Int): Int = a + b
来源：http://kug.gaohongyu789.top

[T59] Scala：循环
来源：http://trj.aibaodan.cn

for (i <- 1 to 10) println(i)
来源：http://udp.ctjpmb.com

[T60] Scala：折叠
来源：http://doo.tarul.cn


<!-- 参考信息 -->