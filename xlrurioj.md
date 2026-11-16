代发 wailian999

ssh user@host 'uptime'
来源：http://gnh.jqgfzy.top

[R58] 下载文件
来源：http://prv.nanxinkj.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kct.yongpay.top

[R59] 发 POST JSON
来源：http://jwx.yfazqb.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hie.hnqzz.top

[R60] 只看 HTTP 状态码
来源：http://hrb.fktsv.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://aoh.hysaishi.cn

[R61] 磁盘占用
来源：http://dca.sweek.top

df -h;  du -sh *
来源：http://bxj.chenjidiqi.icu

[R62] 找最占空间的文件
来源：http://ltz.jqgfzy.top

du -ah . | sort -rh | head -10
来源：http://jzz.aibaodan.cn

[R63] 内存与进程
来源：http://ues.xingfuxueyuan.xyz

free -h;  ps aux | grep nginx
来源：http://zoo.yfazqb.com

[R64] 结束进程
来源：http://fkr.zhoulong.xyz

kill -9 $(pgrep -f app.py)
来源：http://vrs.xingfuxueyuan.xyz

[R65] 查看端口占用
来源：http://euq.andypj.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://eat.haohaochexian.top

[R66] 定时任务
来源：http://xeq.hongshengwenyu.top

crontab -e;  crontab -l
来源：http://epc.wangdashe.top

[R67] 生成随机十六进制串
来源：http://rkn.ybcxt.top

openssl rand -hex 16
来源：http://eul.fanxiaobao.xyz

[R68] 计算文件校验值
来源：http://tcs.jqgfzy.top

sha256sum a.txt;  md5sum a.txt
来源：http://apm.xylfe.cn

[R69] 生成随机密码
来源：http://oik.smart0.xyz

head -c 16 /dev/urandom | base64
来源：http://zsb.fzhhl.top

[R70] 时间戳与互转
来源：http://hku.sxryk.cn

date +%s;  date -d @1700000000
来源：http://oqz.xuetiantiany.cn

[R71] 日期格式化
来源：http://qvu.quarkkingdee.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://bbq.nanxuanxn.top

[R72] 等待端口就绪
来源：http://krl.chenjidiqi.icu

until nc -z localhost 3306; do sleep 1; done
来源：http://lvw.sufxvd.cn

[R73] 分割大日志
来源：http://bmc.svipenyu.cn

split -l 1000 big.log part_
来源：http://yny.yongpay.top

[R74] 批量重命名
来源：http://dyc.pengpengdd.cyou

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ynl.xylfe.cn

[R75] 导出环境变量
来源：http://vuw.tanke756.top

export PATH="$HOME/bin:$PATH"
来源：http://enr.cqqwz.cn

[R76] 使用临时文件
来源：http://rug.jqgufenzy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rxb.c1oappe.top

[R77] 读取用户输入
来源：http://afo.pengpengdd.cyou

read -rp "请输入: " ans
来源：http://prm.cdnleiting.top

[R78] 交互式菜单
来源：http://yzw.shzxlz.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://anp.xinyue.icu

[R79] 解析命令行选项
来源：http://myf.jqgufenzy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fnp.hesvh.cn

[R80] 查看脚本执行耗时
来源：http://wcb.dianchejie.cn

time ./run.sh
来源：http://bac.yuxming.cn

================================================================================
来源：http://ner.andypj.xyz

S. C / C++ 专题
来源：http://uou.yonumen.top

================================================================================
来源：http://djs.smart0.xyz

[S01] C：Hello World
来源：http://kem.bbcook.cn

#include <stdio.h>
来源：http://qnf.redwolf501.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://qpn.jinqigfzy.top

[S02] C：变量与格式化输出
来源：http://bci.redwolf501.top

int a = 10; printf("%d\n", a);
来源：http://nlb.cqqwz.cn

[S03] C：读入整数
来源：http://iht.quarkkingdee.top

int x; scanf("%d", &x);
来源：http://gzg.zhiwuduotai.top

[S04] C：字符串复制
来源：http://tbx.uphjek.com

char dst[32]; strcpy(dst, "hi");
来源：http://itc.ybcxt.top

[S05] C：字符串长度
来源：http://bnw.daxiang520.top

strlen(s)
来源：http://ilf.xylfe.cn

[S06] C：字符串比较
来源：http://kqc.yj202588.top

strcmp(a, b) == 0
来源：http://dyc.xingfuxueyuan.xyz

[S07] C：数组遍历求和
来源：http://rzi.jinghuilouyu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cwq.hcnkem.com

[S08] C：动态内存分配与释放
来源：http://owx.hcnkem.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kvr.jinqigfzy.top

[S09] C：结构体定义与初始化
来源：http://cru.shanyushiyangtech.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gew.guannengcc.top

[S10] C：指针与解引用
来源：http://fkp.hfpthk.cn

int *p = &a;  *p = 5;
来源：http://fon.jqgufenzy.top

[S11] C：逐行读文件
来源：http://nkd.chenlongwang.top

FILE *f = fopen("a.txt", "r");
来源：http://pfj.haohaochexian.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://wkh.hysaishi.cn

fclose(f);
来源：http://scv.ydjk.org.cn

[S12] C：写文件
来源：http://frq.ydjk.org.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ixg.cdnleiting.top

[S13] C：宏定义
来源：http://jwb.epnwcf.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gmt.wangshuangyany.cn

[S14] C：枚举
来源：http://rsx.svipenyu.cn

enum Color { RED, GREEN, BLUE };
来源：http://kof.yvedp.cn

[S15] C：类型转换
来源：http://inr.shanyushiyangkeji.top

(double) a / b
来源：http://jlh.zhijiandao.cn

[S16] C：位操作置位
来源：http://ajb.52xcode.cn

x |= (1 << 3);
来源：http://jmq.tian-w.cn

[S17] C：安全拼接字符串
来源：http://pmn.fehbvm.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pce.cashguo.top

[S18] C：命令行参数
来源：http://vtf.iojbl.cn

int main(int argc, char **argv)
来源：http://uub.guannengcc.top

[S19] C：快速排序
来源：http://hyc.birdmap.top

qsort(a, n, sizeof(int), cmp);
来源：http://nkm.cheryme.top

[S20] C：二分查找
来源：http://tbo.cashguo.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lmx.hywenlv.cn

[S21] C：字符类别判断
来源：http://ebo.dashuyun.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vzy.nwbrower.top

[S22] C：字符串转数字
来源：http://elr.chenjidiqi.icu

atoi("42");  strtod("3.14", NULL);
来源：http://nxl.fktsv.cn

[S23] C：随机数
来源：http://qeg.yanxiufei.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://pmj.hammf.cn

[S24] C：获取本地时间
来源：http://bya.zhiwuduotai.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ika.fktsv.cn

[S25] C：内存拷贝
来源：http://cmv.zhijiandao.cn

memcpy(dst, src, n);
来源：http://gxd.fzhhl.top

[S26] C：内存清零
来源：http://nuh.epnwcf.com

memset(a, 0, sizeof a);
来源：http://xrn.zhengqikj.top

[S27] C：定义常量
来源：http://mhr.yanxiufei.cn

const double PI = 3.14159;
来源：http://mpr.jinyuanbaomall.cn

[S28] C：静态变量
来源：http://phy.yanxiufei.cn

static int counter = 0;
来源：http://qhp.daxiang520.top

[S29] C：变参函数
来源：http://kpd.vqdsnc.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yvh.yj20258.top

[S30] C：头文件保护
来源：http://dzy.gotoacloud.top

#ifndef X_H
来源：http://nri.xingfuxueyuan.xyz

#define X_H
来源：http://upm.aizwys.cn

#endif
来源：http://tml.bbcook.cn

[S31] C++：Hello World
来源：http://daj.gaohongyu789.top

#include <iostream>
来源：http://rij.hongshengwenyu.top

int main() { std::cout << "Hello\n"; }
来源：http://rgn.shuidangran.top

[S32] C++：字符串
来源：http://nrc.zhoulong.xyz

std::string s = "hi";  s += "!";
来源：http://kct.dianchejie.cn

[S33] C++：vector 增删
来源：http://fmu.iojbl.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://iak.guowangkeji.top

[S34] C++：遍历 vector
来源：http://kzz.52xcode.cn

for (auto &x : v) { std::cout << x; }
来源：http://rxb.tianlin.xyz

[S35] C++：map
来源：http://ymw.yuxming.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mok.fanxiaobao.xyz

[S36] C++：unordered_map
来源：http://blr.gzhubu.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qoc.zhixingplan.top

[S37] C++：set
来源：http://ogr.52xcode.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://soi.yj202588.top

[S38] C++：排序
来源：http://mqe.jianghu66.top

std::sort(v.begin(), v.end());
来源：http://afk.yj202588.top

[S39] C++：自定义比较器排序
来源：http://jyk.aizwys.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vif.gogol.net.cn

[S40] C++：查找元素
来源：http://wgw.ppjwa.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rgt.wangshuangyany.cn

[S41] C++：类与构造函数
来源：http://rnz.ctjpmb.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dhe.aizwys.cn

[S42] C++：继承与虚函数
来源：http://cdn.tian-w.cn

class B : public Base { public: void f() override {} };
来源：http://wjs.sweek.top

[S43] C++：智能指针
来源：http://ttk.cheryme.top

auto p = std::make_unique<int>(5);
来源：http://odk.kuanghao11.cn

[S44] C++：引用传参
来源：http://zaz.fehbvm.com

void inc(int &x) { ++x; }
来源：http://gxl.xinyue.icu

[S45] C++：lambda
来源：http://tar.shzxlz.cn

auto add = [](int a, int b) { return a + b; };
来源：http://mhb.wangshuangyany.cn

[S46] C++：函数模板
来源：http://cgh.ydzc1.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wig.bjfxy.top

[S47] C++：结构化绑定遍历
来源：http://rne.xuetiantiany.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://avb.andypj.xyz

[S48] C++：逐行读文件
来源：http://iqq.andypj.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://jwv.ydzc1.top

while (std::getline(in, line)) { }
来源：http://mxu.jqgfzy.top

[S49] C++：写文件
来源：http://boz.dianchejie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://iwu.ywan-chungtsiang.top

[S50] C++：格式化数字
来源：http://kme.shanyushiyangtech.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dqs.cheryme.top

[S51] C++：显式类型转换
来源：http://ymk.nwbrower.top

static_cast<double>(a) / b
来源：http://kza.chenzaomai.com

[S52] C++：const 与 noexcept
来源：http://pan.cqqwz.cn

int size() const noexcept { return n_; }
来源：http://eyx.wangdashe.top

[S53] C++：移动语义
来源：http://rmm.gogol.net.cn

std::vector<int> w = std::move(v);
来源：http://rxt.zhongyouzk.top

[S54] C++：异常处理
来源：http://kdf.cheryme.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zck.tanke756.top

[S55] C++：结构化绑定
来源：http://tzm.zhoulong.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://lza.gaohongyu789.top

[S56] C++：optional
来源：http://hls.jyoumei.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kor.0kj1m.cn

[S57] C++：编译期常量
来源：http://pvz.cheryme.top

constexpr int N = 10;
来源：http://fql.ivvv.top

[S58] C++：命名空间
来源：http://voo.xuetiantiany.cn

namespace ns { int f() { return 1; } }
来源：http://nzq.vqdsnc.cn

[S59] C++：静态断言
来源：http://pdw.yueranfly.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qzv.nanxinkj.top

[S60] C++：遍历并删除元素
来源：http://ujr.shangyingyoupin.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pnd.316326.xyz

================================================================================
来源：http://pvf.hnxiangtu.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://heb.gogol.net.cn

================================================================================
来源：http://rbq.sxryk.cn

[T01] Kotlin：Hello World
来源：http://hty.cashguo.top

println("Hello")
来源：http://cfe.bbcook.cn

[T02] Kotlin：变量
来源：http://chh.gaohongyu789.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sdn.xingfuxueyuan.xyz

[T03] Kotlin：字符串模板
来源：http://rfw.gotoacloud.top

"值: $b"
来源：http://ivg.zhiwuduotai.top

[T04] Kotlin：空安全
来源：http://uyf.mhx1999.top

val n: String? = null;  n?.length
来源：http://oom.ivvv.top

[T05] Kotlin：when 表达式
来源：http://hdw.nanxinkj.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dcx.cashguo.top

[T06] Kotlin：集合映射
来源：http://ref.cheryme.top

listOf(1, 2, 3).map { it * 2 }
来源：http://aea.yvedp.cn

[T07] Kotlin：集合过滤
来源：http://uhu.redwolf501.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ipt.fktsv.cn

[T08] Kotlin：数据类
来源：http://pzi.cucudq.cn

data class User(val name: String, val age: Int)
来源：http://nqf.hongshengwenyu.top

[T09] Kotlin：扩展函数
来源：http://fmv.yanxiufei.cn

fun String.exclaim() = this + "!"
来源：http://vgx.aizwys.cn

[T10] Kotlin：默认参数
来源：http://yys.fengsongda.top

fun greet(name: String = "World") = "Hi $name"
来源：http://rqx.jiagoushi.top

[T11] Kotlin：协程
来源：http://cxo.ctjpmb.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://gly.cashguo.top

[T12] Kotlin：解构声明
来源：http://yjy.hesvh.cn

val (a, b) = Pair(1, 2)
来源：http://fhf.cheryme.top

[T13] Kotlin：只读 Map
来源：http://muj.mhx1999.top

val m = mapOf("a" to 1)
来源：http://lve.guowangkeji.top

[T14] Kotlin：循环
来源：http://xez.yj20258.top

for (i in 1..10) println(i)
来源：http://gmk.kuanghao11.cn

[T15] Kotlin：接口
来源：http://wyu.yuxming.cn

interface Shape { fun area(): Double }
来源：http://svi.zhongyouzk.top

[T16] Swift：Hello World
来源：http://jdi.chenzaomai.com

print("Hello")
来源：http://ote.jianghu66.top

[T17] Swift：变量与常量
来源：http://wud.tanke756.top

var a = 1;  let b = 2
来源：http://stx.yvedp.cn

[T18] Swift：字符串插值
来源：http://pug.vqdsnc.cn

"值: \(b)"
来源：http://lui.yuanzhike.top

[T19] Swift：可选绑定
来源：http://kau.zhiwuduotai.top

if let n = opt { print(n) }
来源：http://oya.xylfe.cn

[T20] Swift：数组操作
来源：http://qma.yuanzhike.top

var a = [1, 2, 3];  a.append(4)
来源：http://efg.fengsongda.top

[T21] Swift：遍历
来源：http://xwi.zhijiandao.cn

for x in a { print(x) }
来源：http://jts.zhijiandao.cn

[T22] Swift：字典
来源：http://frs.52xcode.cn

var d = ["a": 1];  d["b"] = 2
来源：http://tsa.dashuyun.cn

[T23] Swift：函数
来源：http://wqg.epnwcf.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://evf.shzxlz.cn

[T24] Swift：闭包
来源：http://ccn.pycfn.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://sdr.uphjek.com

[T25] Swift：结构体
来源：http://mye.zdqjudy.top

struct P { var x: Int }
来源：http://bph.yonumen.top

[T26] Swift：类与重写
来源：http://ecv.zdbjq.cn

class A: Base { override func f() {} }
来源：http://svv.fktsv.cn

[T27] Swift：错误处理
来源：http://vgx.yj20258.top

do { try f() } catch { print(error) }
来源：http://ogx.sxryk.cn

[T28] Swift：枚举
来源：http://pso.zhixingplan.top

enum Color { case red, green }
来源：http://slh.sxryk.cn

[T29] Swift：guard 提前返回
来源：http://rmd.andypj.xyz

guard let x = opt else { return }
来源：http://gvr.316326.xyz

[T30] Swift：协议
来源：http://jjn.yangfankeji.com

protocol Shape { func area() -> Double }
来源：http://kib.zdqjudy.top

[T31] Lua：Hello World
来源：http://okg.daxiang520.top

print("Hello")
来源：http://tlj.sxryk.cn

[T32] Lua：局部变量
来源：http://wpu.yanxiufei.cn

local a = 1
来源：http://slz.cashguo.top

[T33] Lua：表（数组）
来源：http://pqe.wangshuangyany.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://foe.hnxiangtu.top

[T34] Lua：遍历表
来源：http://vfk.jqgufenzy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://top.yangfankeji.com

[T35] Lua：字典表
来源：http://ppl.cashguo.top

local d = { a = 1 };  d.b = 2
来源：http://mxn.gotoacloud.top

[T36] Lua：函数
来源：http://epi.ywan-chungtsiang.top

function add(a, b) return a + b end
来源：http://gby.sweek.top

[T37] Lua：字符串拼接
来源：http://urj.redwolf501.top

"a" .. "b"
来源：http://clp.xuanzx.com

[T38] Lua：条件
来源：http://xvf.shzxlz.cn

if x > 0 then print("正") end
来源：http://ahx.yj20258.top

[T39] Lua：模式匹配
来源：http://kse.pengpengdd.cyou

string.find(s, "%d+")
来源：http://uaz.zhaomingkeji.xyz

[T40] Lua：元表
来源：http://uws.dashuyun.cn

setmetatable({}, { __index = base })
来源：http://cew.guowangkeji.top

[T41] Perl：Hello World
来源：http://yzk.wangshuangyany.cn

print "Hello\n";
来源：http://qrv.hongshengwenyu.top

[T42] Perl：变量类型
来源：http://aaw.hysaishi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://uvh.mhx1999.top

[T43] Perl：字符串插值
来源：http://dpw.hywenlv.cn

"值: $a"
来源：http://jfb.yuxming.cn

[T44] Perl：条件
来源：http://dxd.gotoacloud.top

if ($a > 0) { print "正"; }
来源：http://map.hysaishi.cn

[T45] Perl：数组遍历
来源：http://aav.cheryme.top

for my $x (@arr) { print $x; }
来源：http://jzw.jianghu66.top

[T46] Perl：哈希操作
来源：http://xel.bjfxy.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zxr.iojbl.cn

[T47] Perl：正则捕获
来源：http://bsm.zdbjq.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wox.haohaochexian.top

[T48] Perl：正则替换
来源：http://wvo.haohaochexian.top

$s =~ s/old/new/g;
来源：http://zuo.yuxming.cn

[T49] Perl：函数
来源：http://dpp.yuxming.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ary.ydjk.org.cn

[T50] Perl：逐行读文件
来源：http://qfp.xuanzx.com

open my $fh, "<", "a.txt" or die $!;
来源：http://oge.shzxlz.cn

while (my $line = <$fh>) { print $line; }
来源：http://rdg.yongpay.top

[T51] Scala：Hello World
来源：http://guz.fanxiaobao.xyz

println("Hello")
来源：http://kxh.yongpay.top

[T52] Scala：变量
来源：http://ssp.feifeiyinyue.top

val a = 1;  var b = 2
来源：http://rbp.hysaishi.cn

[T53] Scala：字符串插值
来源：http://qip.hnqzz.top

s"值: $b"
来源：http://bhe.sufxvd.cn

[T54] Scala：集合映射
来源：http://zev.zhixingplan.top

List(1, 2, 3).map(_ * 2)
来源：http://lki.jinyuanbaomall.cn

[T55] Scala：集合过滤
来源：http://qdb.cashguo.top

List(1, 2, 3).filter(_ > 1)
来源：http://lkg.tanke756.top

[T56] Scala：样例类
来源：http://fna.quarkkingdee.top

case class User(name: String, age: Int)
来源：http://pzk.sjlbkw.cn

[T57] Scala：模式匹配
来源：http://jjc.zhixingplan.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://cgh.yj20258.top

[T58] Scala：函数定义
来源：http://yry.kuanghao11.cn

def add(a: Int, b: Int): Int = a + b
来源：http://awu.shanyushiyangkeji.top

[T59] Scala：循环
来源：http://ymh.c1oappe.top

for (i <- 1 to 10) println(i)
来源：http://hif.shanyushiyangtech.top

[T60] Scala：折叠
来源：http://lxi.feifeiyinyue.top


<!-- 参考信息 -->