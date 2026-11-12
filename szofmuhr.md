代发 wailian999

df -h;  du -sh *
来源：http://tfq.c1oappe.top

[R62] 找最占空间的文件
来源：http://mlj.yvedp.cn

du -ah . | sort -rh | head -10
来源：http://zyr.pycfn.com

[R63] 内存与进程
来源：http://xzw.tanke756.top

free -h;  ps aux | grep nginx
来源：http://vhq.gaohongyu789.top

[R64] 结束进程
来源：http://bfw.yj20258888.top

kill -9 $(pgrep -f app.py)
来源：http://ngc.sxryk.cn

[R65] 查看端口占用
来源：http://ray.pengpengdd.cyou

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xwd.c1oappe.top

[R66] 定时任务
来源：http://tvb.haohaochexian.top

crontab -e;  crontab -l
来源：http://khc.sxryk.cn

[R67] 生成随机十六进制串
来源：http://uau.guannengcc.top

openssl rand -hex 16
来源：http://ymn.jinyuanbaomall.cn

[R68] 计算文件校验值
来源：http://dck.sufxvd.cn

sha256sum a.txt;  md5sum a.txt
来源：http://csb.zdqjudy.top

[R69] 生成随机密码
来源：http://suf.zycfv.cn

head -c 16 /dev/urandom | base64
来源：http://bam.jianghu66.top

[R70] 时间戳与互转
来源：http://zfw.52xcode.cn

date +%s;  date -d @1700000000
来源：http://wfs.birdmap.top

[R71] 日期格式化
来源：http://vls.bjfxy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ghf.bbcook.cn

[R72] 等待端口就绪
来源：http://udq.vqdsnc.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ncm.uphjek.com

[R73] 分割大日志
来源：http://eul.hnxiangtu.top

split -l 1000 big.log part_
来源：http://qnw.shangyingyoupin.top

[R74] 批量重命名
来源：http://gqc.dianchejie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vct.fktsv.cn

[R75] 导出环境变量
来源：http://gwu.jinqigfzy.top

export PATH="$HOME/bin:$PATH"
来源：http://iiw.wangdashe.top

[R76] 使用临时文件
来源：http://huv.xylfe.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ihk.jinqigufen.top

[R77] 读取用户输入
来源：http://tcl.pengpengdd.cyou

read -rp "请输入: " ans
来源：http://iap.hywenlv.cn

[R78] 交互式菜单
来源：http://swf.jyoumei.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gpc.fengsongda.top

[R79] 解析命令行选项
来源：http://kpe.pengpengdd.cyou

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://auy.haohaochexian.top

[R80] 查看脚本执行耗时
来源：http://gho.ehwqpu.com

time ./run.sh
来源：http://kuy.jinghuilouyu.cn

================================================================================
来源：http://rft.yangfankeji.com

S. C / C++ 专题
来源：http://yvy.jyoumei.cn

================================================================================
来源：http://cjy.0kj1m.cn

[S01] C：Hello World
来源：http://sba.cheryme.top

#include <stdio.h>
来源：http://snq.jinghuilouyu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://old.vehdjk.com

[S02] C：变量与格式化输出
来源：http://cka.chenjidiqi.icu

int a = 10; printf("%d\n", a);
来源：http://hqr.mhx1999.top

[S03] C：读入整数
来源：http://zeh.xuanzx.com

int x; scanf("%d", &x);
来源：http://upn.cqqwz.cn

[S04] C：字符串复制
来源：http://fxi.shzxlz.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gsp.tian-w.cn

[S05] C：字符串长度
来源：http://sgz.svipenyu.cn

strlen(s)
来源：http://ahh.nanxinkj.top

[S06] C：字符串比较
来源：http://ibb.zhiwuduotai.top

strcmp(a, b) == 0
来源：http://wrb.bbcook.cn

[S07] C：数组遍历求和
来源：http://jem.uphjek.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fmo.fzhhl.top

[S08] C：动态内存分配与释放
来源：http://txe.wangdashe.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zye.jinqigufen.top

[S09] C：结构体定义与初始化
来源：http://bbe.jinqigfzy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jny.birdmap.top

[S10] C：指针与解引用
来源：http://xic.gaohongyu789.top

int *p = &a;  *p = 5;
来源：http://kls.shzxlz.cn

[S11] C：逐行读文件
来源：http://cof.ybcxt.top

FILE *f = fopen("a.txt", "r");
来源：http://pbh.daxiang520.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ggc.tanke756.top

fclose(f);
来源：http://hos.uphjek.com

[S12] C：写文件
来源：http://xhh.sweek.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://toc.quarkkingdee.top

[S13] C：宏定义
来源：http://hdu.pengpengdd.cyou

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hwh.epnwcf.com

[S14] C：枚举
来源：http://hse.svipenyu.cn

enum Color { RED, GREEN, BLUE };
来源：http://ykf.fengsongda.top

[S15] C：类型转换
来源：http://ywo.pycfn.com

(double) a / b
来源：http://uqt.fktsv.cn

[S16] C：位操作置位
来源：http://ncp.nanxinkj.top

x |= (1 << 3);
来源：http://kcc.fengsongda.top

[S17] C：安全拼接字符串
来源：http://izc.zdbjq.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://puj.bjfxy.top

[S18] C：命令行参数
来源：http://lps.sufxvd.cn

int main(int argc, char **argv)
来源：http://xei.zhongyouzk.top

[S19] C：快速排序
来源：http://oec.ehwqpu.com

qsort(a, n, sizeof(int), cmp);
来源：http://mrz.zycfv.cn

[S20] C：二分查找
来源：http://hqd.yuxming.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hry.zhongyouzk.top

[S21] C：字符类别判断
来源：http://tim.gzhubu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jwg.haohaochexian.top

[S22] C：字符串转数字
来源：http://ods.mhx1999.top

atoi("42");  strtod("3.14", NULL);
来源：http://fnn.nwbrower.top

[S23] C：随机数
来源：http://vrl.jqgufenzy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://dvy.cdnleiting.top

[S24] C：获取本地时间
来源：http://zhn.aizwys.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rrv.yj20258.top

[S25] C：内存拷贝
来源：http://thx.wangshuangyany.cn

memcpy(dst, src, n);
来源：http://she.fktsv.cn

[S26] C：内存清零
来源：http://jxa.yfazqb.com

memset(a, 0, sizeof a);
来源：http://cje.yvedp.cn

[S27] C：定义常量
来源：http://ixs.fengsongda.top

const double PI = 3.14159;
来源：http://udw.aizwys.cn

[S28] C：静态变量
来源：http://hqa.jlsjyb.cn

static int counter = 0;
来源：http://ucx.hysaishi.cn

[S29] C：变参函数
来源：http://zxs.zhengqikj.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lnn.jinghuilouyu.cn

[S30] C：头文件保护
来源：http://sax.andypj.xyz

#ifndef X_H
来源：http://zfm.tian-w.cn

#define X_H
来源：http://xcj.ydzc1.top

#endif
来源：http://nwl.xuetiantiany.cn

[S31] C++：Hello World
来源：http://lhy.shzxlz.cn

#include <iostream>
来源：http://ibh.yongpay.top

int main() { std::cout << "Hello\n"; }
来源：http://gks.zycfv.cn

[S32] C++：字符串
来源：http://xrv.ydjk.org.cn

std::string s = "hi";  s += "!";
来源：http://vod.ppjwa.cn

[S33] C++：vector 增删
来源：http://hte.zdqjudy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qbf.tarul.cn

[S34] C++：遍历 vector
来源：http://mkc.cucudq.cn

for (auto &x : v) { std::cout << x; }
来源：http://onc.yuxming.cn

[S35] C++：map
来源：http://als.zhiwuduotai.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zcc.havefunace.top

[S36] C++：unordered_map
来源：http://nsh.gzhubu.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://omu.dashuyun.cn

[S37] C++：set
来源：http://cnl.zhengqikj.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tbr.jinghuilouyu.cn

[S38] C++：排序
来源：http://cah.smart0.xyz

std::sort(v.begin(), v.end());
来源：http://cmk.cheryme.top

[S39] C++：自定义比较器排序
来源：http://sgf.gogol.net.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uik.guowangkeji.top

[S40] C++：查找元素
来源：http://cbk.c1oappe.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blh.xuanzx.com

[S41] C++：类与构造函数
来源：http://vic.ivvv.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fdj.ppjwa.cn

[S42] C++：继承与虚函数
来源：http://hqm.hfpthk.cn

class B : public Base { public: void f() override {} };
来源：http://tkr.chenzaomai.com

[S43] C++：智能指针
来源：http://fbe.zhengqikj.top

auto p = std::make_unique<int>(5);
来源：http://ywc.vqdsnc.cn

[S44] C++：引用传参
来源：http://llu.aibaodan.cn

void inc(int &x) { ++x; }
来源：http://fru.tarul.cn

[S45] C++：lambda
来源：http://zbu.aizwys.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xze.jinqigfzy.top

[S46] C++：函数模板
来源：http://yar.tarul.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vxp.shuidangran.top

[S47] C++：结构化绑定遍历
来源：http://juy.aizwys.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kfu.hongshengwenyu.top

[S48] C++：逐行读文件
来源：http://fjs.shuidangran.top

std::ifstream in("a.txt");  std::string line;
来源：http://thk.sufxvd.cn

while (std::getline(in, line)) { }
来源：http://tmb.jinqigufen.top

[S49] C++：写文件
来源：http://jor.jinqigufen.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qyc.hnxiangtu.top

[S50] C++：格式化数字
来源：http://mrt.yj20258.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wgn.hnxiangtu.top

[S51] C++：显式类型转换
来源：http://taz.vqdsnc.cn

static_cast<double>(a) / b
来源：http://jwh.gzhubu.top

[S52] C++：const 与 noexcept
来源：http://fqk.fanxiaobao.xyz

int size() const noexcept { return n_; }
来源：http://tem.zycfv.cn

[S53] C++：移动语义
来源：http://ull.fehbvm.com

std::vector<int> w = std::move(v);
来源：http://umj.xylfe.cn

[S54] C++：异常处理
来源：http://azt.fzhhl.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rfh.gzhubu.top

[S55] C++：结构化绑定
来源：http://xhe.svipenyu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://hov.haohaochexian.top

[S56] C++：optional
来源：http://ycg.vqdsnc.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://iuj.yj20258.top

[S57] C++：编译期常量
来源：http://ioe.snrcjt.cn

constexpr int N = 10;
来源：http://ayj.ywan-chungtsiang.top

[S58] C++：命名空间
来源：http://fwt.hesvh.cn

namespace ns { int f() { return 1; } }
来源：http://cdk.jinghuilouyu.cn

[S59] C++：静态断言
来源：http://mmy.zhixingplan.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tug.zhengqikj.top

[S60] C++：遍历并删除元素
来源：http://flu.pengpengdd.cyou

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bda.chenjidiqi.icu

================================================================================
来源：http://ege.0kj1m.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pkm.jinqigufen.top

================================================================================
来源：http://eqa.xinyue.icu

[T01] Kotlin：Hello World
来源：http://fbk.quarkkingdee.top

println("Hello")
来源：http://itz.sjlbkw.cn

[T02] Kotlin：变量
来源：http://xrs.zhiwuduotai.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://puy.nanxuanxn.top

[T03] Kotlin：字符串模板
来源：http://jis.ybcxt.top

"值: $b"
来源：http://ivi.jinqigfzy.top

[T04] Kotlin：空安全
来源：http://qcj.xingfuxueyuan.xyz

val n: String? = null;  n?.length
来源：http://prc.redwolf501.top

[T05] Kotlin：when 表达式
来源：http://jtz.fktsv.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ntl.pycfn.com

[T06] Kotlin：集合映射
来源：http://grk.hesvh.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://mji.daria6918.cn

[T07] Kotlin：集合过滤
来源：http://iwu.yuxming.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://rcf.xylfe.cn

[T08] Kotlin：数据类
来源：http://kzh.nanxuanxn.top

data class User(val name: String, val age: Int)
来源：http://zva.ppjwa.cn

[T09] Kotlin：扩展函数
来源：http://zdz.hcnkem.com

fun String.exclaim() = this + "!"
来源：http://sut.cheryme.top

[T10] Kotlin：默认参数
来源：http://cfd.shanyushiyangtech.top

fun greet(name: String = "World") = "Hi $name"
来源：http://evl.zycfv.cn

[T11] Kotlin：协程
来源：http://rza.iojbl.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://dqy.hongshengwenyu.top

[T12] Kotlin：解构声明
来源：http://qew.zhengqikj.top

val (a, b) = Pair(1, 2)
来源：http://xgw.uphjek.com

[T13] Kotlin：只读 Map
来源：http://afs.tianlin.xyz

val m = mapOf("a" to 1)
来源：http://lkh.yj20258.top

[T14] Kotlin：循环
来源：http://vax.havefunace.top

for (i in 1..10) println(i)
来源：http://yxd.yuxming.cn

[T15] Kotlin：接口
来源：http://qcf.jinyuanbaomall.cn

interface Shape { fun area(): Double }
来源：http://ziu.gaohongyu789.top

[T16] Swift：Hello World
来源：http://joc.zycfv.cn

print("Hello")
来源：http://zka.svipenyu.cn

[T17] Swift：变量与常量
来源：http://zna.pengpengdd.cyou

var a = 1;  let b = 2
来源：http://qzl.vqdsnc.cn

[T18] Swift：字符串插值
来源：http://sum.yueranfly.top

"值: \(b)"
来源：http://cqq.sysykeji.top

[T19] Swift：可选绑定
来源：http://llp.sufxvd.cn

if let n = opt { print(n) }
来源：http://ega.yuanzhike.top

[T20] Swift：数组操作
来源：http://srr.mhx1999.top

var a = [1, 2, 3];  a.append(4)
来源：http://pvf.ctjpmb.com

[T21] Swift：遍历
来源：http://prz.yj20258888.top

for x in a { print(x) }
来源：http://akp.fktsv.cn

[T22] Swift：字典
来源：http://fpy.gzhubu.top

var d = ["a": 1];  d["b"] = 2
来源：http://jjc.xuetiantiany.cn

[T23] Swift：函数
来源：http://pwk.zhoulong.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fzh.quarkkingdee.top

[T24] Swift：闭包
来源：http://gsb.cucudq.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://tsl.xingfuxueyuan.xyz

[T25] Swift：结构体
来源：http://tqg.jyoumei.cn

struct P { var x: Int }
来源：http://kqm.yongpay.top

[T26] Swift：类与重写
来源：http://xfx.316326.xyz

class A: Base { override func f() {} }
来源：http://gcc.xuanzx.com

[T27] Swift：错误处理
来源：http://ypx.pycfn.com

do { try f() } catch { print(error) }
来源：http://war.yj20258.top

[T28] Swift：枚举
来源：http://kor.cucudq.cn

enum Color { case red, green }
来源：http://nxl.nwbrower.top

[T29] Swift：guard 提前返回
来源：http://kdb.sysykeji.top

guard let x = opt else { return }
来源：http://qvd.chenzaomai.com

[T30] Swift：协议
来源：http://xep.fehbvm.com

protocol Shape { func area() -> Double }
来源：http://xwn.jlsjyb.cn

[T31] Lua：Hello World
来源：http://lyr.jiagoushi.top

print("Hello")
来源：http://zzx.ivvv.top

[T32] Lua：局部变量
来源：http://pyl.yvedp.cn

local a = 1
来源：http://jbn.gzhubu.top

[T33] Lua：表（数组）
来源：http://ktw.yvedp.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://mzu.yueranfly.top

[T34] Lua：遍历表
来源：http://igq.aizwys.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rrc.svipenyu.cn

[T35] Lua：字典表
来源：http://onk.hywenlv.cn

local d = { a = 1 };  d.b = 2
来源：http://onr.meibo888.top

[T36] Lua：函数
来源：http://azj.dianchejie.cn

function add(a, b) return a + b end
来源：http://grq.nwbrower.top

[T37] Lua：字符串拼接
来源：http://sqv.sysykeji.top

"a" .. "b"
来源：http://kro.cashguo.top

[T38] Lua：条件
来源：http://qpc.meibo888.top

if x > 0 then print("正") end
来源：http://fpn.hongshengwenyu.top

[T39] Lua：模式匹配
来源：http://rgg.fanxiaobao.xyz

string.find(s, "%d+")
来源：http://dgw.wangshuangyany.cn

[T40] Lua：元表
来源：http://zle.tian-w.cn

setmetatable({}, { __index = base })
来源：http://smd.xuanzx.com

[T41] Perl：Hello World
来源：http://gfz.pengpengdd.cyou

print "Hello\n";
来源：http://ktl.hnqzz.top

[T42] Perl：变量类型
来源：http://mxd.jinyuanbaomall.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vxu.fengsongda.top

[T43] Perl：字符串插值
来源：http://jie.wangdashe.top

"值: $a"
来源：http://tpf.zhaomingkeji.xyz

[T44] Perl：条件
来源：http://pze.yvedp.cn

if ($a > 0) { print "正"; }
来源：http://yqq.fzhhl.top

[T45] Perl：数组遍历
来源：http://fhz.hongshengwenyu.top

for my $x (@arr) { print $x; }
来源：http://kez.yj20258.top

[T46] Perl：哈希操作
来源：http://rox.zdqjudy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://keb.mhx1999.top

[T47] Perl：正则捕获
来源：http://hwj.ppjwa.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://uci.yj20258.top

[T48] Perl：正则替换
来源：http://hqs.ydjk.org.cn

$s =~ s/old/new/g;
来源：http://gwk.52xcode.cn

[T49] Perl：函数
来源：http://kcd.yangfankeji.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hxs.ybcxt.top

[T50] Perl：逐行读文件
来源：http://znv.xuetiantiany.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zzs.ivvv.top

while (my $line = <$fh>) { print $line; }
来源：http://evq.zhiwuduotai.top

[T51] Scala：Hello World
来源：http://zgi.daria6918.cn

println("Hello")
来源：http://auv.yfazqb.com

[T52] Scala：变量
来源：http://bya.birdmap.top

val a = 1;  var b = 2
来源：http://rac.yueranfly.top

[T53] Scala：字符串插值
来源：http://uyu.hcnkem.com

s"值: $b"
来源：http://pol.tanke756.top

[T54] Scala：集合映射
来源：http://woa.chenzaomai.com

List(1, 2, 3).map(_ * 2)
来源：http://fri.dashuyun.cn

[T55] Scala：集合过滤
来源：http://cdu.ydjk.org.cn

List(1, 2, 3).filter(_ > 1)
来源：http://tuw.xinyue.icu

[T56] Scala：样例类
来源：http://vho.ivvv.top

case class User(name: String, age: Int)
来源：http://rjz.jqgufenzy.top

[T57] Scala：模式匹配
来源：http://cpd.aibaodan.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://tpp.aibaodan.cn

[T58] Scala：函数定义
来源：http://nlm.tarul.cn

def add(a: Int, b: Int): Int = a + b
来源：http://rdc.pengpengdd.cyou

[T59] Scala：循环
来源：http://hdc.gaohongyu789.top

for (i <- 1 to 10) println(i)
来源：http://wjp.ydjk.org.cn

[T60] Scala：折叠
来源：http://lit.kuanghao11.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hon.xuanzx.com

================================================================================
来源：http://xrq.aizwys.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kxe.quarkkingdee.top

================================================================================
来源：http://oue.gaohongyu789.top

[U01] Py：创建虚拟环境
来源：http://tqz.zhijiandao.cn

python -m venv .venv && source .venv/bin/activate
来源：http://urx.epnwcf.com

[U02] Py：导出 / 安装依赖
来源：http://eqp.hnqzz.top

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cgo.yongpay.top


<!-- 参考信息 -->