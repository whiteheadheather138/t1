代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://itl.hywenlv.cn

[R60] 只看 HTTP 状态码
来源：http://bpy.zhongyouzk.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rmf.sufxvd.cn

[R61] 磁盘占用
来源：http://tji.jqgfzy.top

df -h;  du -sh *
来源：http://chn.yuanzhike.top

[R62] 找最占空间的文件
来源：http://vvh.pengpengdd.cyou

du -ah . | sort -rh | head -10
来源：http://xbc.hnxiangtu.top

[R63] 内存与进程
来源：http://tuf.pycfn.com

free -h;  ps aux | grep nginx
来源：http://mbu.snrcjt.cn

[R64] 结束进程
来源：http://dqi.mhx1999.top

kill -9 $(pgrep -f app.py)
来源：http://hut.ydjk.org.cn

[R65] 查看端口占用
来源：http://ihx.epnwcf.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://oka.snrcjt.cn

[R66] 定时任务
来源：http://nmm.ehwqpu.com

crontab -e;  crontab -l
来源：http://wsn.zhixingplan.top

[R67] 生成随机十六进制串
来源：http://tot.shanyushiyangtech.top

openssl rand -hex 16
来源：http://ndf.shangyingyoupin.top

[R68] 计算文件校验值
来源：http://zyx.jlsjyb.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hdp.zhaomingkeji.xyz

[R69] 生成随机密码
来源：http://ulb.c1oappe.top

head -c 16 /dev/urandom | base64
来源：http://qbg.ctjpmb.com

[R70] 时间戳与互转
来源：http://hep.hongshengwenyu.top

date +%s;  date -d @1700000000
来源：http://lmc.sweek.top

[R71] 日期格式化
来源：http://sat.zhiwuduotai.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ega.pycfn.com

[R72] 等待端口就绪
来源：http://azg.shzxlz.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://czf.yueranfly.top

[R73] 分割大日志
来源：http://xzm.gaohongyu789.top

split -l 1000 big.log part_
来源：http://ycc.hnqzz.top

[R74] 批量重命名
来源：http://ray.svipenyu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hos.zdqjudy.top

[R75] 导出环境变量
来源：http://mch.cdnleiting.top

export PATH="$HOME/bin:$PATH"
来源：http://xql.xylfe.cn

[R76] 使用临时文件
来源：http://sam.zhoulong.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nmt.fengsongda.top

[R77] 读取用户输入
来源：http://sjh.jinghuilouyu.cn

read -rp "请输入: " ans
来源：http://usv.hnxiangtu.top

[R78] 交互式菜单
来源：http://xqj.cdnleiting.top

select opt in a b c; do echo "$opt"; break; done
来源：http://cfo.aibaodan.cn

[R79] 解析命令行选项
来源：http://dhp.hcnkem.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ndi.zhixingplan.top

[R80] 查看脚本执行耗时
来源：http://pxc.wangshuangyany.cn

time ./run.sh
来源：http://vvj.wangshuangyany.cn

================================================================================
来源：http://iuw.ybcxt.top

S. C / C++ 专题
来源：http://iay.zdbjq.cn

================================================================================
来源：http://pvw.nwbrower.top

[S01] C：Hello World
来源：http://yet.ivvv.top

#include <stdio.h>
来源：http://syc.xylfe.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://agm.nwbrower.top

[S02] C：变量与格式化输出
来源：http://flz.nwbrower.top

int a = 10; printf("%d\n", a);
来源：http://hub.zhongyouzk.top

[S03] C：读入整数
来源：http://zle.cashguo.top

int x; scanf("%d", &x);
来源：http://gqx.xylfe.cn

[S04] C：字符串复制
来源：http://wiq.sxryk.cn

char dst[32]; strcpy(dst, "hi");
来源：http://uug.wangdashe.top

[S05] C：字符串长度
来源：http://qbz.fktsv.cn

strlen(s)
来源：http://uhu.smart0.xyz

[S06] C：字符串比较
来源：http://axl.cucudq.cn

strcmp(a, b) == 0
来源：http://xyu.hysaishi.cn

[S07] C：数组遍历求和
来源：http://qme.iojbl.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ymh.chenjidiqi.icu

[S08] C：动态内存分配与释放
来源：http://avr.bbcook.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xhw.tanke756.top

[S09] C：结构体定义与初始化
来源：http://mcb.zhiwuduotai.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://iwd.shzxlz.cn

[S10] C：指针与解引用
来源：http://lrw.tanke756.top

int *p = &a;  *p = 5;
来源：http://lrf.daria6918.cn

[S11] C：逐行读文件
来源：http://nna.chenlongwang.top

FILE *f = fopen("a.txt", "r");
来源：http://wrd.zhoulong.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://awe.shuidangran.top

fclose(f);
来源：http://mkd.chenjidiqi.icu

[S12] C：写文件
来源：http://pnd.uphjek.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yih.hesvh.cn

[S13] C：宏定义
来源：http://nbk.zycfv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xcy.jinqigufen.top

[S14] C：枚举
来源：http://zfh.ehwqpu.com

enum Color { RED, GREEN, BLUE };
来源：http://jdb.sweek.top

[S15] C：类型转换
来源：http://oaw.zhixingplan.top

(double) a / b
来源：http://iuw.shzxlz.cn

[S16] C：位操作置位
来源：http://xdj.vqdsnc.cn

x |= (1 << 3);
来源：http://dwy.sxryk.cn

[S17] C：安全拼接字符串
来源：http://qga.andypj.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pbc.hnqzz.top

[S18] C：命令行参数
来源：http://mhu.pengpengdd.cyou

int main(int argc, char **argv)
来源：http://nyj.chenzaomai.com

[S19] C：快速排序
来源：http://rcq.cashguo.top

qsort(a, n, sizeof(int), cmp);
来源：http://dia.chenzaomai.com

[S20] C：二分查找
来源：http://zcm.sweek.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vge.xylfe.cn

[S21] C：字符类别判断
来源：http://ihq.chenzaomai.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mvf.gotoacloud.top

[S22] C：字符串转数字
来源：http://sic.snrcjt.cn

atoi("42");  strtod("3.14", NULL);
来源：http://yxm.shuidangran.top

[S23] C：随机数
来源：http://wsq.aizwys.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://eoi.cheryme.top

[S24] C：获取本地时间
来源：http://xze.sufxvd.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vgq.hysaishi.cn

[S25] C：内存拷贝
来源：http://oln.xziqi.cn

memcpy(dst, src, n);
来源：http://iia.fanxiaobao.xyz

[S26] C：内存清零
来源：http://fcb.guannengcc.top

memset(a, 0, sizeof a);
来源：http://rti.jqgufenzy.top

[S27] C：定义常量
来源：http://yzu.tianlin.xyz

const double PI = 3.14159;
来源：http://awn.nanxinkj.top

[S28] C：静态变量
来源：http://tvb.hcnkem.com

static int counter = 0;
来源：http://mav.cheryme.top

[S29] C：变参函数
来源：http://seg.bbcook.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://icl.zdbjq.cn

[S30] C：头文件保护
来源：http://qaa.jinqigfzy.top

#ifndef X_H
来源：http://mdz.smart0.xyz

#define X_H
来源：http://nfh.yfazqb.com

#endif
来源：http://xvm.snrcjt.cn

[S31] C++：Hello World
来源：http://ukf.dashuyun.cn

#include <iostream>
来源：http://jpn.nwbrower.top

int main() { std::cout << "Hello\n"; }
来源：http://flp.hnqzz.top

[S32] C++：字符串
来源：http://cls.hesvh.cn

std::string s = "hi";  s += "!";
来源：http://vgh.jqgfzy.top

[S33] C++：vector 增删
来源：http://zdv.mhx1999.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://szv.shzxlz.cn

[S34] C++：遍历 vector
来源：http://ibh.shanyushiyangkeji.top

for (auto &x : v) { std::cout << x; }
来源：http://jiy.fanxiaobao.xyz

[S35] C++：map
来源：http://wtl.c1oappe.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hkq.xingfuxueyuan.xyz

[S36] C++：unordered_map
来源：http://mjp.shangyingyoupin.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://msc.yonumen.top

[S37] C++：set
来源：http://myx.ehwqpu.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dvo.chenzaomai.com

[S38] C++：排序
来源：http://ekw.bjfxy.top

std::sort(v.begin(), v.end());
来源：http://oyu.yvedp.cn

[S39] C++：自定义比较器排序
来源：http://fdi.shuidangran.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://frt.fzhhl.top

[S40] C++：查找元素
来源：http://jyx.ywan-chungtsiang.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nnk.tian-w.cn

[S41] C++：类与构造函数
来源：http://mdw.haohaochexian.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://klk.sjlbkw.cn

[S42] C++：继承与虚函数
来源：http://rbh.ivvv.top

class B : public Base { public: void f() override {} };
来源：http://lqe.zhijiandao.cn

[S43] C++：智能指针
来源：http://xiy.zhaomingkeji.xyz

auto p = std::make_unique<int>(5);
来源：http://vqt.nwbrower.top

[S44] C++：引用传参
来源：http://acc.jqgfzy.top

void inc(int &x) { ++x; }
来源：http://bmf.zycfv.cn

[S45] C++：lambda
来源：http://bcs.bjfxy.top

auto add = [](int a, int b) { return a + b; };
来源：http://qqn.dashuyun.cn

[S46] C++：函数模板
来源：http://nuv.vehdjk.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xkd.yuxming.cn

[S47] C++：结构化绑定遍历
来源：http://wra.hywenlv.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://otk.guannengcc.top

[S48] C++：逐行读文件
来源：http://yig.hcnkem.com

std::ifstream in("a.txt");  std::string line;
来源：http://jki.ehwqpu.com

while (std::getline(in, line)) { }
来源：http://elh.hammf.cn

[S49] C++：写文件
来源：http://aqw.havefunace.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://khk.fanxiaobao.xyz

[S50] C++：格式化数字
来源：http://kbn.jiagoushi.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sve.meibo888.top

[S51] C++：显式类型转换
来源：http://ojz.hfpthk.cn

static_cast<double>(a) / b
来源：http://htq.feifeiyinyue.top

[S52] C++：const 与 noexcept
来源：http://peq.feifeiyinyue.top

int size() const noexcept { return n_; }
来源：http://muo.zhaomingkeji.xyz

[S53] C++：移动语义
来源：http://iks.xuetiantiany.cn

std::vector<int> w = std::move(v);
来源：http://urs.yanxiufei.cn

[S54] C++：异常处理
来源：http://uda.gotoacloud.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lcp.gaohongyu789.top

[S55] C++：结构化绑定
来源：http://ked.fktsv.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bte.ydzc1.top

[S56] C++：optional
来源：http://qwt.ybcxt.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yzn.jinqigfzy.top

[S57] C++：编译期常量
来源：http://jft.c1oappe.top

constexpr int N = 10;
来源：http://nlk.shanyushiyangtech.top

[S58] C++：命名空间
来源：http://lgl.gzhubu.top

namespace ns { int f() { return 1; } }
来源：http://uxw.hfpthk.cn

[S59] C++：静态断言
来源：http://spq.ydjk.org.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qdn.fengsongda.top

[S60] C++：遍历并删除元素
来源：http://wsh.bjfxy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sqz.dianchejie.cn

================================================================================
来源：http://dmz.birdmap.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xyp.yj20258888.top

================================================================================
来源：http://ywn.jinghuilouyu.cn

[T01] Kotlin：Hello World
来源：http://ojb.fanxiaobao.xyz

println("Hello")
来源：http://mpe.chenzaomai.com

[T02] Kotlin：变量
来源：http://xhi.xziqi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dkh.zycfv.cn

[T03] Kotlin：字符串模板
来源：http://bwv.zhixingplan.top

"值: $b"
来源：http://nke.guannengcc.top

[T04] Kotlin：空安全
来源：http://heg.ppjwa.cn

val n: String? = null;  n?.length
来源：http://mlk.zhijiandao.cn

[T05] Kotlin：when 表达式
来源：http://jzn.bjfxy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xds.fengsongda.top

[T06] Kotlin：集合映射
来源：http://mrh.hfpthk.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://dgd.daxiang520.top

[T07] Kotlin：集合过滤
来源：http://asp.hnqzz.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://dwz.c1oappe.top

[T08] Kotlin：数据类
来源：http://yze.gogol.net.cn

data class User(val name: String, val age: Int)
来源：http://wmy.cdnleiting.top

[T09] Kotlin：扩展函数
来源：http://ebo.xylfe.cn

fun String.exclaim() = this + "!"
来源：http://zzt.xinyue.icu

[T10] Kotlin：默认参数
来源：http://bsy.hfpthk.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://drg.jlsjyb.cn

[T11] Kotlin：协程
来源：http://fnt.shanyushiyangkeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://peh.bbcook.cn

[T12] Kotlin：解构声明
来源：http://wsp.sufxvd.cn

val (a, b) = Pair(1, 2)
来源：http://dtj.ivvv.top

[T13] Kotlin：只读 Map
来源：http://pyh.316326.xyz

val m = mapOf("a" to 1)
来源：http://tyo.yfazqb.com

[T14] Kotlin：循环
来源：http://anc.0kj1m.cn

for (i in 1..10) println(i)
来源：http://pwd.cdnleiting.top

[T15] Kotlin：接口
来源：http://nrx.vehdjk.com

interface Shape { fun area(): Double }
来源：http://uti.shanyushiyangkeji.top

[T16] Swift：Hello World
来源：http://ncl.epnwcf.com

print("Hello")
来源：http://qyf.fanxiaobao.xyz

[T17] Swift：变量与常量
来源：http://yrd.ppjwa.cn

var a = 1;  let b = 2
来源：http://hgz.svipenyu.cn

[T18] Swift：字符串插值
来源：http://aba.yuxming.cn

"值: \(b)"
来源：http://dvu.aibaodan.cn

[T19] Swift：可选绑定
来源：http://cqn.dashuyun.cn

if let n = opt { print(n) }
来源：http://akw.zhixingplan.top

[T20] Swift：数组操作
来源：http://hli.feifeiyinyue.top

var a = [1, 2, 3];  a.append(4)
来源：http://mrl.jiagoushi.top

[T21] Swift：遍历
来源：http://vgp.0kj1m.cn

for x in a { print(x) }
来源：http://ugk.hywenlv.cn

[T22] Swift：字典
来源：http://ocq.xingfuxueyuan.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://ltz.fehbvm.com

[T23] Swift：函数
来源：http://xhn.jinqigfzy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://knh.cheryme.top

[T24] Swift：闭包
来源：http://yjk.hnqzz.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ett.zhengqikj.top

[T25] Swift：结构体
来源：http://xun.sufxvd.cn

struct P { var x: Int }
来源：http://laf.pycfn.com

[T26] Swift：类与重写
来源：http://whd.iojbl.cn

class A: Base { override func f() {} }
来源：http://wkn.smart0.xyz

[T27] Swift：错误处理
来源：http://rvt.zhaomingkeji.xyz

do { try f() } catch { print(error) }
来源：http://cce.gogol.net.cn

[T28] Swift：枚举
来源：http://atj.yvedp.cn

enum Color { case red, green }
来源：http://nvb.zhijiandao.cn

[T29] Swift：guard 提前返回
来源：http://azd.hcnkem.com

guard let x = opt else { return }
来源：http://hsx.yanxiufei.cn

[T30] Swift：协议
来源：http://mfi.hysaishi.cn

protocol Shape { func area() -> Double }
来源：http://hgs.jyoumei.cn

[T31] Lua：Hello World
来源：http://snu.jianghu66.top

print("Hello")
来源：http://clb.hesvh.cn

[T32] Lua：局部变量
来源：http://htv.cashguo.top

local a = 1
来源：http://arw.nanxinkj.top

[T33] Lua：表（数组）
来源：http://tzc.jlsjyb.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wyr.nanxuanxn.top

[T34] Lua：遍历表
来源：http://rvf.shzxlz.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://lwu.hongshengwenyu.top

[T35] Lua：字典表
来源：http://umf.jqgfzy.top

local d = { a = 1 };  d.b = 2
来源：http://faj.tianlin.xyz

[T36] Lua：函数
来源：http://eoj.316326.xyz

function add(a, b) return a + b end
来源：http://yqe.feifeiyinyue.top

[T37] Lua：字符串拼接
来源：http://mvu.jyoumei.cn

"a" .. "b"
来源：http://egy.cashguo.top

[T38] Lua：条件
来源：http://elh.yuanzhike.top

if x > 0 then print("正") end
来源：http://efc.shzxlz.cn

[T39] Lua：模式匹配
来源：http://cfv.ybcxt.top

string.find(s, "%d+")
来源：http://soy.ivvv.top

[T40] Lua：元表
来源：http://njd.jinyuanbaomall.cn

setmetatable({}, { __index = base })
来源：http://ptd.guannengcc.top

[T41] Perl：Hello World
来源：http://bot.jqgfzy.top

print "Hello\n";
来源：http://kkc.jyoumei.cn

[T42] Perl：变量类型
来源：http://wra.jiagoushi.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ugr.snrcjt.cn

[T43] Perl：字符串插值
来源：http://xbw.smart0.xyz

"值: $a"
来源：http://jhk.zdbjq.cn

[T44] Perl：条件
来源：http://unu.dianchejie.cn

if ($a > 0) { print "正"; }
来源：http://rsa.yongpay.top

[T45] Perl：数组遍历
来源：http://xsb.jqgufenzy.top

for my $x (@arr) { print $x; }
来源：http://cpe.vehdjk.com

[T46] Perl：哈希操作
来源：http://epc.xinyue.icu

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dpn.cdnleiting.top

[T47] Perl：正则捕获
来源：http://tyu.hammf.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://she.smart0.xyz

[T48] Perl：正则替换
来源：http://agu.xuanzx.com

$s =~ s/old/new/g;
来源：http://ipf.cashguo.top

[T49] Perl：函数
来源：http://xkv.jinghuilouyu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gaj.epnwcf.com

[T50] Perl：逐行读文件
来源：http://bnn.kuanghao11.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://sip.guowangkeji.top

while (my $line = <$fh>) { print $line; }
来源：http://thb.c1oappe.top

[T51] Scala：Hello World
来源：http://nma.aibaodan.cn

println("Hello")
来源：http://hwc.shanyushiyangtech.top

[T52] Scala：变量
来源：http://hqk.shanyushiyangkeji.top

val a = 1;  var b = 2
来源：http://xxa.haohaochexian.top

[T53] Scala：字符串插值
来源：http://rgn.shzxlz.cn

s"值: $b"
来源：http://nws.ehwqpu.com

[T54] Scala：集合映射
来源：http://wza.ywan-chungtsiang.top

List(1, 2, 3).map(_ * 2)
来源：http://zrq.shzxlz.cn

[T55] Scala：集合过滤
来源：http://wfy.vqdsnc.cn

List(1, 2, 3).filter(_ > 1)
来源：http://sdk.yuanzhike.top

[T56] Scala：样例类
来源：http://cej.zhengqikj.top

case class User(name: String, age: Int)
来源：http://yda.jyoumei.cn

[T57] Scala：模式匹配
来源：http://bbz.daria6918.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ocv.aibaodan.cn

[T58] Scala：函数定义
来源：http://age.zhijiandao.cn

def add(a: Int, b: Int): Int = a + b
来源：http://vef.zdbjq.cn

[T59] Scala：循环
来源：http://xgz.zhijiandao.cn

for (i <- 1 to 10) println(i)
来源：http://jhp.yvedp.cn

[T60] Scala：折叠
来源：http://xtv.hongshengwenyu.top

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dkl.tarul.cn

================================================================================
来源：http://xfz.ydzc1.top

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zis.zycfv.cn

================================================================================
来源：http://uif.meibo888.top


<!-- 参考信息 -->