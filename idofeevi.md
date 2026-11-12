代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yhp.jinyuanbaomall.cn

[R56] 远程拷贝
来源：http://mep.shanyushiyangkeji.top

scp file user@host:/path/
来源：http://hdu.yj20258888.top

[R57] 远程执行命令
来源：http://plq.cdnleiting.top

ssh user@host 'uptime'
来源：http://cza.ydjk.org.cn

[R58] 下载文件
来源：http://xlu.ppjwa.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pkd.ybcxt.top

[R59] 发 POST JSON
来源：http://srt.andypj.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jlp.chenjidiqi.icu

[R60] 只看 HTTP 状态码
来源：http://bcv.nanxinkj.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://slk.chenlongwang.top

[R61] 磁盘占用
来源：http://slk.haohaochexian.top

df -h;  du -sh *
来源：http://vov.ppjwa.cn

[R62] 找最占空间的文件
来源：http://ogp.cqqwz.cn

du -ah . | sort -rh | head -10
来源：http://abe.hnxiangtu.top

[R63] 内存与进程
来源：http://eky.iojbl.cn

free -h;  ps aux | grep nginx
来源：http://xvo.jinghuilouyu.cn

[R64] 结束进程
来源：http://bsn.haohaochexian.top

kill -9 $(pgrep -f app.py)
来源：http://ezo.fehbvm.com

[R65] 查看端口占用
来源：http://rup.epnwcf.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jof.chenjidiqi.icu

[R66] 定时任务
来源：http://xuo.fzhhl.top

crontab -e;  crontab -l
来源：http://ecr.chenjidiqi.icu

[R67] 生成随机十六进制串
来源：http://yov.zycfv.cn

openssl rand -hex 16
来源：http://amo.iojbl.cn

[R68] 计算文件校验值
来源：http://orq.xylfe.cn

sha256sum a.txt;  md5sum a.txt
来源：http://flb.jinghuilouyu.cn

[R69] 生成随机密码
来源：http://czd.yongpay.top

head -c 16 /dev/urandom | base64
来源：http://jes.pengpengdd.cyou

[R70] 时间戳与互转
来源：http://hxc.birdmap.top

date +%s;  date -d @1700000000
来源：http://jcy.jqgufenzy.top

[R71] 日期格式化
来源：http://jto.aibaodan.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zpz.ybcxt.top

[R72] 等待端口就绪
来源：http://ihb.ppjwa.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hkw.fengsongda.top

[R73] 分割大日志
来源：http://gfp.sxryk.cn

split -l 1000 big.log part_
来源：http://caw.yj20258.top

[R74] 批量重命名
来源：http://myx.havefunace.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lzp.ybcxt.top

[R75] 导出环境变量
来源：http://gtp.shzxlz.cn

export PATH="$HOME/bin:$PATH"
来源：http://hyv.bbcook.cn

[R76] 使用临时文件
来源：http://nok.ivvv.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rne.zhongyouzk.top

[R77] 读取用户输入
来源：http://rlj.jyoumei.cn

read -rp "请输入: " ans
来源：http://rll.sweek.top

[R78] 交互式菜单
来源：http://beq.zhongyouzk.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ylb.shanyushiyangtech.top

[R79] 解析命令行选项
来源：http://cnz.dianchejie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zmc.pengpengdd.cyou

[R80] 查看脚本执行耗时
来源：http://ffp.cucudq.cn

time ./run.sh
来源：http://ido.jiagoushi.top

================================================================================
来源：http://vfh.fehbvm.com

S. C / C++ 专题
来源：http://qdu.chenjidiqi.icu

================================================================================
来源：http://uwp.gzhubu.top

[S01] C：Hello World
来源：http://ojd.jlsjyb.cn

#include <stdio.h>
来源：http://slb.shuidangran.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://pdc.hfpthk.cn

[S02] C：变量与格式化输出
来源：http://whz.ctjpmb.com

int a = 10; printf("%d\n", a);
来源：http://etb.uphjek.com

[S03] C：读入整数
来源：http://jns.gaohongyu789.top

int x; scanf("%d", &x);
来源：http://gke.zhiwuduotai.top

[S04] C：字符串复制
来源：http://wxl.316326.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://yje.cqqwz.cn

[S05] C：字符串长度
来源：http://xui.epnwcf.com

strlen(s)
来源：http://cts.feifeiyinyue.top

[S06] C：字符串比较
来源：http://dsg.yongpay.top

strcmp(a, b) == 0
来源：http://csq.fanxiaobao.xyz

[S07] C：数组遍历求和
来源：http://uhv.tanke756.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://awg.shangyingyoupin.top

[S08] C：动态内存分配与释放
来源：http://rvl.sjlbkw.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yln.cheryme.top

[S09] C：结构体定义与初始化
来源：http://ody.kuanghao11.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jol.xziqi.cn

[S10] C：指针与解引用
来源：http://fum.yuanzhike.top

int *p = &a;  *p = 5;
来源：http://meo.xuetiantiany.cn

[S11] C：逐行读文件
来源：http://srq.jinqigufen.top

FILE *f = fopen("a.txt", "r");
来源：http://ein.yj202588.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://kbe.hnxiangtu.top

fclose(f);
来源：http://tmn.svipenyu.cn

[S12] C：写文件
来源：http://hqi.meibo888.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://puh.epnwcf.com

[S13] C：宏定义
来源：http://xux.ehwqpu.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dzk.nanxuanxn.top

[S14] C：枚举
来源：http://cbf.svipenyu.cn

enum Color { RED, GREEN, BLUE };
来源：http://fgn.yj20258.top

[S15] C：类型转换
来源：http://odm.aibaodan.cn

(double) a / b
来源：http://lzf.zhiwuduotai.top

[S16] C：位操作置位
来源：http://kkl.yvedp.cn

x |= (1 << 3);
来源：http://pes.hcnkem.com

[S17] C：安全拼接字符串
来源：http://ptb.redwolf501.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jno.yj20258.top

[S18] C：命令行参数
来源：http://wcm.zhixingplan.top

int main(int argc, char **argv)
来源：http://ylf.cqqwz.cn

[S19] C：快速排序
来源：http://tfc.xuanzx.com

qsort(a, n, sizeof(int), cmp);
来源：http://qui.sxryk.cn

[S20] C：二分查找
来源：http://hal.yongpay.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nye.fktsv.cn

[S21] C：字符类别判断
来源：http://usq.ydzc1.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nsi.dianchejie.cn

[S22] C：字符串转数字
来源：http://vtr.ctjpmb.com

atoi("42");  strtod("3.14", NULL);
来源：http://tlh.tianlin.xyz

[S23] C：随机数
来源：http://kuh.hysaishi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://txb.cucudq.cn

[S24] C：获取本地时间
来源：http://apr.jqgufenzy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nhg.bjfxy.top

[S25] C：内存拷贝
来源：http://qwd.vehdjk.com

memcpy(dst, src, n);
来源：http://udg.zhongyouzk.top

[S26] C：内存清零
来源：http://vvk.xinyue.icu

memset(a, 0, sizeof a);
来源：http://fzb.hammf.cn

[S27] C：定义常量
来源：http://yco.yangfankeji.com

const double PI = 3.14159;
来源：http://moe.ydzc1.top

[S28] C：静态变量
来源：http://ods.gaohongyu789.top

static int counter = 0;
来源：http://sqy.xziqi.cn

[S29] C：变参函数
来源：http://eyv.fktsv.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nmw.zdqjudy.top

[S30] C：头文件保护
来源：http://sqp.svipenyu.cn

#ifndef X_H
来源：http://gzp.zycfv.cn

#define X_H
来源：http://owi.tanke756.top

#endif
来源：http://lsv.jinqigufen.top

[S31] C++：Hello World
来源：http://qet.yuxming.cn

#include <iostream>
来源：http://vtk.cqqwz.cn

int main() { std::cout << "Hello\n"; }
来源：http://kcp.shzxlz.cn

[S32] C++：字符串
来源：http://jva.hongshengwenyu.top

std::string s = "hi";  s += "!";
来源：http://mya.jianghu66.top

[S33] C++：vector 增删
来源：http://nmv.jqgfzy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mon.pycfn.com

[S34] C++：遍历 vector
来源：http://ige.hcnkem.com

for (auto &x : v) { std::cout << x; }
来源：http://lht.sxryk.cn

[S35] C++：map
来源：http://euz.mhx1999.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sym.meibo888.top

[S36] C++：unordered_map
来源：http://gal.9152youxi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tmw.zdqjudy.top

[S37] C++：set
来源：http://ftf.hnqzz.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xpl.yfazqb.com

[S38] C++：排序
来源：http://nmi.daxiang520.top

std::sort(v.begin(), v.end());
来源：http://zsx.sysykeji.top

[S39] C++：自定义比较器排序
来源：http://xkr.wangshuangyany.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gft.0kj1m.cn

[S40] C++：查找元素
来源：http://hjq.bbcook.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://abg.yj20258888.top

[S41] C++：类与构造函数
来源：http://dsh.smart0.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gsd.zhixingplan.top

[S42] C++：继承与虚函数
来源：http://myf.wangshuangyany.cn

class B : public Base { public: void f() override {} };
来源：http://fzy.chenlongwang.top

[S43] C++：智能指针
来源：http://bmd.fanxiaobao.xyz

auto p = std::make_unique<int>(5);
来源：http://drf.sweek.top

[S44] C++：引用传参
来源：http://nsy.nanxuanxn.top

void inc(int &x) { ++x; }
来源：http://avz.zhijiandao.cn

[S45] C++：lambda
来源：http://rwj.hfpthk.cn

auto add = [](int a, int b) { return a + b; };
来源：http://oeg.sxryk.cn

[S46] C++：函数模板
来源：http://vrd.ehwqpu.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xmf.zdbjq.cn

[S47] C++：结构化绑定遍历
来源：http://elx.guowangkeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xdi.shangyingyoupin.top

[S48] C++：逐行读文件
来源：http://yyd.aizwys.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fvy.epnwcf.com

while (std::getline(in, line)) { }
来源：http://fmp.sweek.top

[S49] C++：写文件
来源：http://rwe.dashuyun.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://shk.yfazqb.com

[S50] C++：格式化数字
来源：http://kjp.hnqzz.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fad.ppjwa.cn

[S51] C++：显式类型转换
来源：http://akr.jqgfzy.top

static_cast<double>(a) / b
来源：http://rai.haohaochexian.top

[S52] C++：const 与 noexcept
来源：http://dhf.yj20258.top

int size() const noexcept { return n_; }
来源：http://xck.zhiwuduotai.top

[S53] C++：移动语义
来源：http://ixd.wangshuangyany.cn

std::vector<int> w = std::move(v);
来源：http://zco.shuidangran.top

[S54] C++：异常处理
来源：http://ssw.haohaochexian.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hed.fehbvm.com

[S55] C++：结构化绑定
来源：http://ula.hfpthk.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://hvl.gogol.net.cn

[S56] C++：optional
来源：http://zoz.nanxuanxn.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ljq.0kj1m.cn

[S57] C++：编译期常量
来源：http://lpx.nanxinkj.top

constexpr int N = 10;
来源：http://vpm.ctjpmb.com

[S58] C++：命名空间
来源：http://gqk.meibo888.top

namespace ns { int f() { return 1; } }
来源：http://pvu.svipenyu.cn

[S59] C++：静态断言
来源：http://zcm.xinyue.icu

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://byi.havefunace.top

[S60] C++：遍历并删除元素
来源：http://lmx.hesvh.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zsi.birdmap.top

================================================================================
来源：http://swi.meibo888.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fma.meibo888.top

================================================================================
来源：http://qdx.fktsv.cn

[T01] Kotlin：Hello World
来源：http://ypu.hnxiangtu.top

println("Hello")
来源：http://vmi.fehbvm.com

[T02] Kotlin：变量
来源：http://eur.xingfuxueyuan.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cqz.shuidangran.top

[T03] Kotlin：字符串模板
来源：http://pxn.chenlongwang.top

"值: $b"
来源：http://tok.shuidangran.top

[T04] Kotlin：空安全
来源：http://fjq.shanyushiyangtech.top

val n: String? = null;  n?.length
来源：http://zmh.0kj1m.cn

[T05] Kotlin：when 表达式
来源：http://une.jqgufenzy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uoa.hongshengwenyu.top

[T06] Kotlin：集合映射
来源：http://gwt.bbcook.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://nnz.iojbl.cn

[T07] Kotlin：集合过滤
来源：http://xkr.havefunace.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://acp.xinyue.icu

[T08] Kotlin：数据类
来源：http://jgc.tanke756.top

data class User(val name: String, val age: Int)
来源：http://lyr.yuanzhike.top

[T09] Kotlin：扩展函数
来源：http://wyu.9152youxi.cn

fun String.exclaim() = this + "!"
来源：http://iup.xinyue.icu

[T10] Kotlin：默认参数
来源：http://wes.smart0.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://zxw.52xcode.cn

[T11] Kotlin：协程
来源：http://uep.hammf.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wpx.yongpay.top

[T12] Kotlin：解构声明
来源：http://phh.ydzc1.top

val (a, b) = Pair(1, 2)
来源：http://nqj.yuanzhike.top

[T13] Kotlin：只读 Map
来源：http://rsv.xuetiantiany.cn

val m = mapOf("a" to 1)
来源：http://lip.gogol.net.cn

[T14] Kotlin：循环
来源：http://ick.chenlongwang.top

for (i in 1..10) println(i)
来源：http://zvc.iojbl.cn

[T15] Kotlin：接口
来源：http://ovf.shuidangran.top

interface Shape { fun area(): Double }
来源：http://cda.pycfn.com

[T16] Swift：Hello World
来源：http://qua.jqgufenzy.top

print("Hello")
来源：http://gna.yuxming.cn

[T17] Swift：变量与常量
来源：http://xqt.xuetiantiany.cn

var a = 1;  let b = 2
来源：http://fnz.hywenlv.cn

[T18] Swift：字符串插值
来源：http://zpy.zhengqikj.top

"值: \(b)"
来源：http://iht.fengsongda.top

[T19] Swift：可选绑定
来源：http://dyy.aibaodan.cn

if let n = opt { print(n) }
来源：http://ogc.pycfn.com

[T20] Swift：数组操作
来源：http://uud.sysykeji.top

var a = [1, 2, 3];  a.append(4)
来源：http://iip.shangyingyoupin.top

[T21] Swift：遍历
来源：http://fkk.jqgfzy.top

for x in a { print(x) }
来源：http://htj.yj202588.top

[T22] Swift：字典
来源：http://znv.svipenyu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://kzd.cqqwz.cn

[T23] Swift：函数
来源：http://dlu.hysaishi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://btc.zhiwuduotai.top

[T24] Swift：闭包
来源：http://ywm.nwbrower.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://hub.sxryk.cn

[T25] Swift：结构体
来源：http://aul.hnxiangtu.top

struct P { var x: Int }
来源：http://zoi.xylfe.cn

[T26] Swift：类与重写
来源：http://pue.mhx1999.top

class A: Base { override func f() {} }
来源：http://flp.guannengcc.top

[T27] Swift：错误处理
来源：http://joz.zdqjudy.top

do { try f() } catch { print(error) }
来源：http://pzg.yj20258.top

[T28] Swift：枚举
来源：http://frk.jinqigufen.top

enum Color { case red, green }
来源：http://gve.jqgufenzy.top

[T29] Swift：guard 提前返回
来源：http://quo.dashuyun.cn

guard let x = opt else { return }
来源：http://mkn.jinghuilouyu.cn

[T30] Swift：协议
来源：http://icr.yuanzhike.top

protocol Shape { func area() -> Double }
来源：http://qnu.andypj.xyz

[T31] Lua：Hello World
来源：http://vzi.xinyue.icu

print("Hello")
来源：http://oal.yuanzhike.top

[T32] Lua：局部变量
来源：http://mjj.tanke756.top

local a = 1
来源：http://lsx.yonumen.top

[T33] Lua：表（数组）
来源：http://pbp.fehbvm.com

local t = {1, 2, 3};  t[4] = 4
来源：http://txw.yvedp.cn

[T34] Lua：遍历表
来源：http://ivi.dashuyun.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://wly.wangdashe.top

[T35] Lua：字典表
来源：http://hpu.gaohongyu789.top

local d = { a = 1 };  d.b = 2
来源：http://xmc.shanyushiyangtech.top

[T36] Lua：函数
来源：http://fph.sufxvd.cn

function add(a, b) return a + b end
来源：http://cwo.yj20258.top

[T37] Lua：字符串拼接
来源：http://hjl.zhiwuduotai.top

"a" .. "b"
来源：http://brt.zycfv.cn

[T38] Lua：条件
来源：http://bph.cashguo.top

if x > 0 then print("正") end
来源：http://esh.zhijiandao.cn

[T39] Lua：模式匹配
来源：http://mzb.ehwqpu.com

string.find(s, "%d+")
来源：http://cxz.zhengqikj.top

[T40] Lua：元表
来源：http://sst.gzhubu.top

setmetatable({}, { __index = base })
来源：http://zup.yfazqb.com

[T41] Perl：Hello World
来源：http://saf.shzxlz.cn

print "Hello\n";
来源：http://hic.shzxlz.cn

[T42] Perl：变量类型
来源：http://diz.ybcxt.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://oae.zdqjudy.top

[T43] Perl：字符串插值
来源：http://mhw.dashuyun.cn

"值: $a"
来源：http://fyt.yuanzhike.top

[T44] Perl：条件
来源：http://mqu.shanyushiyangkeji.top

if ($a > 0) { print "正"; }
来源：http://ddb.haohaochexian.top

[T45] Perl：数组遍历
来源：http://zzw.yuxming.cn

for my $x (@arr) { print $x; }
来源：http://vhv.mhx1999.top

[T46] Perl：哈希操作
来源：http://pep.jyoumei.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ysm.xylfe.cn

[T47] Perl：正则捕获
来源：http://jol.ywan-chungtsiang.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://vej.xuanzx.com

[T48] Perl：正则替换
来源：http://yzb.zdbjq.cn

$s =~ s/old/new/g;
来源：http://guv.jiagoushi.top

[T49] Perl：函数
来源：http://eee.tanke756.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yxd.nwbrower.top

[T50] Perl：逐行读文件
来源：http://iwi.fzhhl.top

open my $fh, "<", "a.txt" or die $!;
来源：http://six.52xcode.cn

while (my $line = <$fh>) { print $line; }
来源：http://exi.guowangkeji.top

[T51] Scala：Hello World
来源：http://xbh.birdmap.top

println("Hello")
来源：http://mkq.zhijiandao.cn

[T52] Scala：变量
来源：http://bvf.guowangkeji.top

val a = 1;  var b = 2
来源：http://gwr.jinghuilouyu.cn

[T53] Scala：字符串插值
来源：http://ijn.xingfuxueyuan.xyz

s"值: $b"
来源：http://jqc.cdnleiting.top

[T54] Scala：集合映射
来源：http://rfn.zhijiandao.cn

List(1, 2, 3).map(_ * 2)
来源：http://pky.ydzc1.top

[T55] Scala：集合过滤
来源：http://tmg.sysykeji.top

List(1, 2, 3).filter(_ > 1)
来源：http://vux.dianchejie.cn

[T56] Scala：样例类
来源：http://lyq.yfazqb.com

case class User(name: String, age: Int)
来源：http://glx.wangdashe.top

[T57] Scala：模式匹配
来源：http://jsj.jinqigfzy.top

x match { case 1 => "一"; case _ => "其他" }
来源：http://kqy.zhixingplan.top

[T58] Scala：函数定义
来源：http://cvf.yj202588.top


<!-- 参考信息 -->