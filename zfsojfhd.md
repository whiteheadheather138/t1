代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rcm.cashguo.top

[R54] 比较两个文件
来源：http://hwu.yanxiufei.cn

diff a.txt b.txt
来源：http://sos.svipenyu.cn

[R55] 压缩与解压
来源：http://irx.cashguo.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vod.zhixingplan.top

[R56] 远程拷贝
来源：http://syz.xinyue.icu

scp file user@host:/path/
来源：http://yqk.guannengcc.top

[R57] 远程执行命令
来源：http://rja.xziqi.cn

ssh user@host 'uptime'
来源：http://awt.jyoumei.cn

[R58] 下载文件
来源：http://yvp.pycfn.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zjg.yongpay.top

[R59] 发 POST JSON
来源：http://znf.hnqzz.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jnq.yongpay.top

[R60] 只看 HTTP 状态码
来源：http://pyi.hcnkem.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://glx.birdmap.top

[R61] 磁盘占用
来源：http://fyr.zhengqikj.top

df -h;  du -sh *
来源：http://mim.cqqwz.cn

[R62] 找最占空间的文件
来源：http://bvw.smart0.xyz

du -ah . | sort -rh | head -10
来源：http://ukm.jinyuanbaomall.cn

[R63] 内存与进程
来源：http://tvq.wangshuangyany.cn

free -h;  ps aux | grep nginx
来源：http://xkf.ywan-chungtsiang.top

[R64] 结束进程
来源：http://xkl.sjlbkw.cn

kill -9 $(pgrep -f app.py)
来源：http://dwy.uphjek.com

[R65] 查看端口占用
来源：http://afn.uphjek.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xto.zycfv.cn

[R66] 定时任务
来源：http://wfh.zdbjq.cn

crontab -e;  crontab -l
来源：http://yxs.svipenyu.cn

[R67] 生成随机十六进制串
来源：http://edr.jinghuilouyu.cn

openssl rand -hex 16
来源：http://khc.jinyuanbaomall.cn

[R68] 计算文件校验值
来源：http://esn.jlsjyb.cn

sha256sum a.txt;  md5sum a.txt
来源：http://yph.guowangkeji.top

[R69] 生成随机密码
来源：http://rxj.yangfankeji.com

head -c 16 /dev/urandom | base64
来源：http://cpm.sweek.top

[R70] 时间戳与互转
来源：http://uld.kuanghao11.cn

date +%s;  date -d @1700000000
来源：http://fpp.meibo888.top

[R71] 日期格式化
来源：http://jhw.havefunace.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ywe.jyoumei.cn

[R72] 等待端口就绪
来源：http://pxa.cheryme.top

until nc -z localhost 3306; do sleep 1; done
来源：http://htk.guannengcc.top

[R73] 分割大日志
来源：http://ykl.redwolf501.top

split -l 1000 big.log part_
来源：http://zvc.fehbvm.com

[R74] 批量重命名
来源：http://cvh.shanyushiyangtech.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://epz.hnqzz.top

[R75] 导出环境变量
来源：http://ktg.xinyue.icu

export PATH="$HOME/bin:$PATH"
来源：http://unf.xuanzx.com

[R76] 使用临时文件
来源：http://spj.yvedp.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://grl.ivvv.top

[R77] 读取用户输入
来源：http://nhe.52xcode.cn

read -rp "请输入: " ans
来源：http://uvp.cqqwz.cn

[R78] 交互式菜单
来源：http://qvu.aizwys.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ljw.yueranfly.top

[R79] 解析命令行选项
来源：http://vfq.nanxinkj.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uko.havefunace.top

[R80] 查看脚本执行耗时
来源：http://wpq.aibaodan.cn

time ./run.sh
来源：http://plb.cheryme.top

================================================================================
来源：http://cjx.yangfankeji.com

S. C / C++ 专题
来源：http://qkf.shanyushiyangkeji.top

================================================================================
来源：http://hvl.svipenyu.cn

[S01] C：Hello World
来源：http://mia.bbcook.cn

#include <stdio.h>
来源：http://pzl.yvedp.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://dqp.yonumen.top

[S02] C：变量与格式化输出
来源：http://wdn.sysykeji.top

int a = 10; printf("%d\n", a);
来源：http://sar.wangshuangyany.cn

[S03] C：读入整数
来源：http://idh.fanxiaobao.xyz

int x; scanf("%d", &x);
来源：http://kut.hesvh.cn

[S04] C：字符串复制
来源：http://sbn.jinqigfzy.top

char dst[32]; strcpy(dst, "hi");
来源：http://kyk.xingfuxueyuan.xyz

[S05] C：字符串长度
来源：http://osv.ctjpmb.com

strlen(s)
来源：http://gzv.guowangkeji.top

[S06] C：字符串比较
来源：http://cgi.ybcxt.top

strcmp(a, b) == 0
来源：http://ydt.mhx1999.top

[S07] C：数组遍历求和
来源：http://gqj.gotoacloud.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tks.zycfv.cn

[S08] C：动态内存分配与释放
来源：http://lcx.kuanghao11.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dqb.shzxlz.cn

[S09] C：结构体定义与初始化
来源：http://lsb.vqdsnc.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sxo.sufxvd.cn

[S10] C：指针与解引用
来源：http://zrh.xuetiantiany.cn

int *p = &a;  *p = 5;
来源：http://zrb.fktsv.cn

[S11] C：逐行读文件
来源：http://vwu.gogol.net.cn

FILE *f = fopen("a.txt", "r");
来源：http://ijp.hesvh.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://sjc.ydzc1.top

fclose(f);
来源：http://mdh.ydjk.org.cn

[S12] C：写文件
来源：http://mxr.shangyingyoupin.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ana.shangyingyoupin.top

[S13] C：宏定义
来源：http://ywr.sxryk.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://agv.tian-w.cn

[S14] C：枚举
来源：http://vcj.ppjwa.cn

enum Color { RED, GREEN, BLUE };
来源：http://zed.sjlbkw.cn

[S15] C：类型转换
来源：http://yxo.daria6918.cn

(double) a / b
来源：http://huf.mhx1999.top

[S16] C：位操作置位
来源：http://xzd.aibaodan.cn

x |= (1 << 3);
来源：http://qxj.hfpthk.cn

[S17] C：安全拼接字符串
来源：http://olv.yuxming.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://brm.cheryme.top

[S18] C：命令行参数
来源：http://lqw.jinyuanbaomall.cn

int main(int argc, char **argv)
来源：http://gof.jyoumei.cn

[S19] C：快速排序
来源：http://cnl.xuetiantiany.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qwo.chenzaomai.com

[S20] C：二分查找
来源：http://sbk.cheryme.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://khi.smart0.xyz

[S21] C：字符类别判断
来源：http://hsa.yuanzhike.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://miz.sjlbkw.cn

[S22] C：字符串转数字
来源：http://chw.bbcook.cn

atoi("42");  strtod("3.14", NULL);
来源：http://sfm.zhaomingkeji.xyz

[S23] C：随机数
来源：http://zcu.meibo888.top

srand(time(NULL));  int r = rand() % 100;
来源：http://rwv.daria6918.cn

[S24] C：获取本地时间
来源：http://dbk.jinqigufen.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hup.chenzaomai.com

[S25] C：内存拷贝
来源：http://eds.zhaomingkeji.xyz

memcpy(dst, src, n);
来源：http://xfp.fengsongda.top

[S26] C：内存清零
来源：http://jcv.sysykeji.top

memset(a, 0, sizeof a);
来源：http://jne.meibo888.top

[S27] C：定义常量
来源：http://isa.hfpthk.cn

const double PI = 3.14159;
来源：http://huq.chenlongwang.top

[S28] C：静态变量
来源：http://wxw.feifeiyinyue.top

static int counter = 0;
来源：http://wgt.yj20258.top

[S29] C：变参函数
来源：http://tev.hesvh.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kka.52xcode.cn

[S30] C：头文件保护
来源：http://dnu.gogol.net.cn

#ifndef X_H
来源：http://iqz.jiagoushi.top

#define X_H
来源：http://tqj.jinyuanbaomall.cn

#endif
来源：http://ycg.tianlin.xyz

[S31] C++：Hello World
来源：http://mux.yvedp.cn

#include <iostream>
来源：http://zgd.smart0.xyz

int main() { std::cout << "Hello\n"; }
来源：http://gwk.zhixingplan.top

[S32] C++：字符串
来源：http://nhu.ppjwa.cn

std::string s = "hi";  s += "!";
来源：http://yta.mhx1999.top

[S33] C++：vector 增删
来源：http://sjl.0kj1m.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zgj.sweek.top

[S34] C++：遍历 vector
来源：http://pam.fengsongda.top

for (auto &x : v) { std::cout << x; }
来源：http://pns.ctjpmb.com

[S35] C++：map
来源：http://ker.nwbrower.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bgb.zycfv.cn

[S36] C++：unordered_map
来源：http://nwi.hywenlv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://csa.ppjwa.cn

[S37] C++：set
来源：http://nyw.ydzc1.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ued.cheryme.top

[S38] C++：排序
来源：http://dlo.hfpthk.cn

std::sort(v.begin(), v.end());
来源：http://jcc.xziqi.cn

[S39] C++：自定义比较器排序
来源：http://yst.shanyushiyangtech.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pfp.hnqzz.top

[S40] C++：查找元素
来源：http://pww.jinqigfzy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wvh.fanxiaobao.xyz

[S41] C++：类与构造函数
来源：http://asf.shangyingyoupin.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ntk.sweek.top

[S42] C++：继承与虚函数
来源：http://peb.dianchejie.cn

class B : public Base { public: void f() override {} };
来源：http://hez.52xcode.cn

[S43] C++：智能指针
来源：http://pqz.daxiang520.top

auto p = std::make_unique<int>(5);
来源：http://yip.0kj1m.cn

[S44] C++：引用传参
来源：http://dbr.wangdashe.top

void inc(int &x) { ++x; }
来源：http://xsy.cheryme.top

[S45] C++：lambda
来源：http://sju.kuanghao11.cn

auto add = [](int a, int b) { return a + b; };
来源：http://paz.bjfxy.top

[S46] C++：函数模板
来源：http://jfq.snrcjt.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gzn.hywenlv.cn

[S47] C++：结构化绑定遍历
来源：http://mnj.nanxinkj.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vng.mhx1999.top

[S48] C++：逐行读文件
来源：http://yje.jlsjyb.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ndy.sweek.top

while (std::getline(in, line)) { }
来源：http://ahg.shuidangran.top

[S49] C++：写文件
来源：http://rik.yongpay.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rws.ydzc1.top

[S50] C++：格式化数字
来源：http://ugy.hywenlv.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://oax.shanyushiyangkeji.top

[S51] C++：显式类型转换
来源：http://woe.shanyushiyangkeji.top

static_cast<double>(a) / b
来源：http://sub.xziqi.cn

[S52] C++：const 与 noexcept
来源：http://nrk.cheryme.top

int size() const noexcept { return n_; }
来源：http://ozz.gotoacloud.top

[S53] C++：移动语义
来源：http://ddw.xuetiantiany.cn

std::vector<int> w = std::move(v);
来源：http://fhv.yvedp.cn

[S54] C++：异常处理
来源：http://qui.shanyushiyangkeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ouz.tanke756.top

[S55] C++：结构化绑定
来源：http://icm.meibo888.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ptn.haohaochexian.top

[S56] C++：optional
来源：http://qec.tian-w.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://utg.sysykeji.top

[S57] C++：编译期常量
来源：http://hlg.hywenlv.cn

constexpr int N = 10;
来源：http://cxd.uphjek.com

[S58] C++：命名空间
来源：http://rhq.daxiang520.top

namespace ns { int f() { return 1; } }
来源：http://uqk.nanxuanxn.top

[S59] C++：静态断言
来源：http://qtq.52xcode.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mxy.bbcook.cn

[S60] C++：遍历并删除元素
来源：http://uvq.shanyushiyangtech.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://obt.cdnleiting.top

================================================================================
来源：http://jjt.ehwqpu.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ind.xingfuxueyuan.xyz

================================================================================
来源：http://gcc.gogol.net.cn

[T01] Kotlin：Hello World
来源：http://yzi.zhixingplan.top

println("Hello")
来源：http://wzk.epnwcf.com

[T02] Kotlin：变量
来源：http://ulh.havefunace.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mju.hongshengwenyu.top

[T03] Kotlin：字符串模板
来源：http://eha.ywan-chungtsiang.top

"值: $b"
来源：http://vtc.tianlin.xyz

[T04] Kotlin：空安全
来源：http://iol.shzxlz.cn

val n: String? = null;  n?.length
来源：http://aqi.yvedp.cn

[T05] Kotlin：when 表达式
来源：http://twh.jianghu66.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kro.guannengcc.top

[T06] Kotlin：集合映射
来源：http://bcy.cdnleiting.top

listOf(1, 2, 3).map { it * 2 }
来源：http://wib.zdqjudy.top

[T07] Kotlin：集合过滤
来源：http://smo.hfpthk.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ahy.sufxvd.cn

[T08] Kotlin：数据类
来源：http://jvn.ywan-chungtsiang.top

data class User(val name: String, val age: Int)
来源：http://dfw.nanxinkj.top

[T09] Kotlin：扩展函数
来源：http://suc.bbcook.cn

fun String.exclaim() = this + "!"
来源：http://jin.kuanghao11.cn

[T10] Kotlin：默认参数
来源：http://nxp.ydzc1.top

fun greet(name: String = "World") = "Hi $name"
来源：http://qgw.redwolf501.top

[T11] Kotlin：协程
来源：http://rqx.pengpengdd.cyou

GlobalScope.launch { delay(1000); println("done") }
来源：http://efp.yuxming.cn

[T12] Kotlin：解构声明
来源：http://tti.hywenlv.cn

val (a, b) = Pair(1, 2)
来源：http://ynp.tian-w.cn

[T13] Kotlin：只读 Map
来源：http://fox.ywan-chungtsiang.top

val m = mapOf("a" to 1)
来源：http://mqh.redwolf501.top

[T14] Kotlin：循环
来源：http://owc.xuanzx.com

for (i in 1..10) println(i)
来源：http://zgr.fengsongda.top

[T15] Kotlin：接口
来源：http://ien.zhijiandao.cn

interface Shape { fun area(): Double }
来源：http://tcd.sjlbkw.cn

[T16] Swift：Hello World
来源：http://bkc.dianchejie.cn

print("Hello")
来源：http://uao.jinqigufen.top

[T17] Swift：变量与常量
来源：http://sbe.yuanzhike.top

var a = 1;  let b = 2
来源：http://faz.hnxiangtu.top

[T18] Swift：字符串插值
来源：http://eqs.shangyingyoupin.top

"值: \(b)"
来源：http://dsx.haohaochexian.top

[T19] Swift：可选绑定
来源：http://vgo.fktsv.cn

if let n = opt { print(n) }
来源：http://lee.hnqzz.top

[T20] Swift：数组操作
来源：http://suy.316326.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://uup.hywenlv.cn

[T21] Swift：遍历
来源：http://hgn.sysykeji.top

for x in a { print(x) }
来源：http://lxs.sxryk.cn

[T22] Swift：字典
来源：http://cnf.vqdsnc.cn

var d = ["a": 1];  d["b"] = 2
来源：http://sdf.jinghuilouyu.cn

[T23] Swift：函数
来源：http://dzm.ydzc1.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://thn.tanke756.top

[T24] Swift：闭包
来源：http://lty.hywenlv.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://bnu.feifeiyinyue.top

[T25] Swift：结构体
来源：http://yxd.nanxuanxn.top

struct P { var x: Int }
来源：http://cew.zdqjudy.top

[T26] Swift：类与重写
来源：http://hdt.guannengcc.top

class A: Base { override func f() {} }
来源：http://qdr.yfazqb.com

[T27] Swift：错误处理
来源：http://sog.nanxuanxn.top

do { try f() } catch { print(error) }
来源：http://xeu.chenzaomai.com

[T28] Swift：枚举
来源：http://tkq.nanxuanxn.top

enum Color { case red, green }
来源：http://yvm.vqdsnc.cn

[T29] Swift：guard 提前返回
来源：http://dmn.shangyingyoupin.top

guard let x = opt else { return }
来源：http://dfo.epnwcf.com

[T30] Swift：协议
来源：http://wgm.quarkkingdee.top

protocol Shape { func area() -> Double }
来源：http://mkf.0kj1m.cn

[T31] Lua：Hello World
来源：http://bqv.sxryk.cn

print("Hello")
来源：http://bwu.kuanghao11.cn

[T32] Lua：局部变量
来源：http://ide.ppjwa.cn

local a = 1
来源：http://ejs.cheryme.top

[T33] Lua：表（数组）
来源：http://mdu.fengsongda.top

local t = {1, 2, 3};  t[4] = 4
来源：http://alk.fktsv.cn

[T34] Lua：遍历表
来源：http://tvj.bjfxy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://lyh.daria6918.cn

[T35] Lua：字典表
来源：http://krn.yonumen.top

local d = { a = 1 };  d.b = 2
来源：http://bkp.ydzc1.top

[T36] Lua：函数
来源：http://zxg.guannengcc.top

function add(a, b) return a + b end
来源：http://cpf.ppjwa.cn

[T37] Lua：字符串拼接
来源：http://ggb.meibo888.top

"a" .. "b"
来源：http://bnb.xuanzx.com

[T38] Lua：条件
来源：http://jwp.zhijiandao.cn

if x > 0 then print("正") end
来源：http://pfg.zhaomingkeji.xyz

[T39] Lua：模式匹配
来源：http://kvb.haohaochexian.top

string.find(s, "%d+")
来源：http://tck.bbcook.cn

[T40] Lua：元表
来源：http://xla.dianchejie.cn

setmetatable({}, { __index = base })
来源：http://vig.xziqi.cn

[T41] Perl：Hello World
来源：http://oez.cucudq.cn

print "Hello\n";
来源：http://tpz.yuxming.cn

[T42] Perl：变量类型
来源：http://oey.0kj1m.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://orz.jinqigfzy.top

[T43] Perl：字符串插值
来源：http://ayg.sysykeji.top

"值: $a"
来源：http://jvb.zhoulong.xyz

[T44] Perl：条件
来源：http://aqo.sjlbkw.cn

if ($a > 0) { print "正"; }
来源：http://zsj.ydjk.org.cn

[T45] Perl：数组遍历
来源：http://zvr.aizwys.cn

for my $x (@arr) { print $x; }
来源：http://cwc.zhongyouzk.top

[T46] Perl：哈希操作
来源：http://cad.zhijiandao.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cqx.fanxiaobao.xyz

[T47] Perl：正则捕获
来源：http://vzv.cdnleiting.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://cal.gaohongyu789.top

[T48] Perl：正则替换
来源：http://zuk.vqdsnc.cn

$s =~ s/old/new/g;
来源：http://wnq.cucudq.cn

[T49] Perl：函数
来源：http://jvd.yj202588.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ehd.ydzc1.top

[T50] Perl：逐行读文件
来源：http://gmx.zdbjq.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://kyg.jinqigufen.top

while (my $line = <$fh>) { print $line; }
来源：http://qrl.bjfxy.top

[T51] Scala：Hello World
来源：http://kjj.aizwys.cn

println("Hello")
来源：http://gmv.sjlbkw.cn

[T52] Scala：变量
来源：http://qfi.cheryme.top

val a = 1;  var b = 2
来源：http://lel.ydzc1.top

[T53] Scala：字符串插值
来源：http://jfu.jinghuilouyu.cn

s"值: $b"
来源：http://jyi.feifeiyinyue.top

[T54] Scala：集合映射
来源：http://cby.gotoacloud.top

List(1, 2, 3).map(_ * 2)
来源：http://ldz.tarul.cn

[T55] Scala：集合过滤
来源：http://tpv.gogol.net.cn

List(1, 2, 3).filter(_ > 1)
来源：http://jhv.zycfv.cn

[T56] Scala：样例类
来源：http://eah.tianlin.xyz


<!-- 参考信息 -->