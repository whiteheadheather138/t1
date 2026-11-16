代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://keu.hcnkem.com

[R50] awk 求和
来源：http://otd.kuanghao11.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bnq.jqgufenzy.top

[R51] 排序去重取前几
来源：http://vxa.hnxiangtu.top

sort a.txt | uniq -c | sort -rn | head
来源：http://plw.aibaodan.cn

[R52] 统计行数
来源：http://zsq.gzhubu.top

wc -l a.txt
来源：http://xsy.ydjk.org.cn

[R53] 查看文件头与实时尾
来源：http://ygo.shanyushiyangkeji.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://iqn.guowangkeji.top

[R54] 比较两个文件
来源：http://biy.316326.xyz

diff a.txt b.txt
来源：http://ntm.ppjwa.cn

[R55] 压缩与解压
来源：http://kdb.ydzc1.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jnm.hnqzz.top

[R56] 远程拷贝
来源：http://txw.nwbrower.top

scp file user@host:/path/
来源：http://iut.snrcjt.cn

[R57] 远程执行命令
来源：http://euq.birdmap.top

ssh user@host 'uptime'
来源：http://jte.guowangkeji.top

[R58] 下载文件
来源：http://bds.shangyingyoupin.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qzo.xuanzx.com

[R59] 发 POST JSON
来源：http://zdi.ybcxt.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://edw.yj20258.top

[R60] 只看 HTTP 状态码
来源：http://vwb.guowangkeji.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qmf.cqqwz.cn

[R61] 磁盘占用
来源：http://opi.sysykeji.top

df -h;  du -sh *
来源：http://efp.ctjpmb.com

[R62] 找最占空间的文件
来源：http://omm.yuxming.cn

du -ah . | sort -rh | head -10
来源：http://pql.chenzaomai.com

[R63] 内存与进程
来源：http://eee.xuanzx.com

free -h;  ps aux | grep nginx
来源：http://zjv.xingfuxueyuan.xyz

[R64] 结束进程
来源：http://cyp.bbcook.cn

kill -9 $(pgrep -f app.py)
来源：http://lfc.ydzc1.top

[R65] 查看端口占用
来源：http://iyq.sjlbkw.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://coy.pengpengdd.cyou

[R66] 定时任务
来源：http://rha.316326.xyz

crontab -e;  crontab -l
来源：http://dkf.yj20258.top

[R67] 生成随机十六进制串
来源：http://brz.gotoacloud.top

openssl rand -hex 16
来源：http://bsa.iojbl.cn

[R68] 计算文件校验值
来源：http://muv.snrcjt.cn

sha256sum a.txt;  md5sum a.txt
来源：http://jjr.daxiang520.top

[R69] 生成随机密码
来源：http://yll.hywenlv.cn

head -c 16 /dev/urandom | base64
来源：http://qxr.yj20258.top

[R70] 时间戳与互转
来源：http://uev.wangdashe.top

date +%s;  date -d @1700000000
来源：http://dnl.52xcode.cn

[R71] 日期格式化
来源：http://nzi.daria6918.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://jyd.kuanghao11.cn

[R72] 等待端口就绪
来源：http://hvt.tanke756.top

until nc -z localhost 3306; do sleep 1; done
来源：http://jlf.hfpthk.cn

[R73] 分割大日志
来源：http://vne.vehdjk.com

split -l 1000 big.log part_
来源：http://tbl.tianlin.xyz

[R74] 批量重命名
来源：http://wqb.fengsongda.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hun.bbcook.cn

[R75] 导出环境变量
来源：http://oer.ppjwa.cn

export PATH="$HOME/bin:$PATH"
来源：http://utk.sweek.top

[R76] 使用临时文件
来源：http://hjd.yongpay.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ays.fengsongda.top

[R77] 读取用户输入
来源：http://snv.yfazqb.com

read -rp "请输入: " ans
来源：http://jsf.xinyue.icu

[R78] 交互式菜单
来源：http://drc.xuanzx.com

select opt in a b c; do echo "$opt"; break; done
来源：http://cxg.hnqzz.top

[R79] 解析命令行选项
来源：http://wag.ywan-chungtsiang.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mhx.chenjidiqi.icu

[R80] 查看脚本执行耗时
来源：http://xye.ydzc1.top

time ./run.sh
来源：http://dvg.jinyuanbaomall.cn

================================================================================
来源：http://zos.yonumen.top

S. C / C++ 专题
来源：http://rxo.hnxiangtu.top

================================================================================
来源：http://lpi.gotoacloud.top

[S01] C：Hello World
来源：http://jft.yongpay.top

#include <stdio.h>
来源：http://coq.zhoulong.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://uag.iojbl.cn

[S02] C：变量与格式化输出
来源：http://jev.ydjk.org.cn

int a = 10; printf("%d\n", a);
来源：http://psb.nwbrower.top

[S03] C：读入整数
来源：http://uup.smart0.xyz

int x; scanf("%d", &x);
来源：http://ddr.svipenyu.cn

[S04] C：字符串复制
来源：http://tfz.zhiwuduotai.top

char dst[32]; strcpy(dst, "hi");
来源：http://twy.fzhhl.top

[S05] C：字符串长度
来源：http://iph.ybcxt.top

strlen(s)
来源：http://wjr.cdnleiting.top

[S06] C：字符串比较
来源：http://skc.zycfv.cn

strcmp(a, b) == 0
来源：http://aub.hysaishi.cn

[S07] C：数组遍历求和
来源：http://itz.jinqigufen.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ugr.c1oappe.top

[S08] C：动态内存分配与释放
来源：http://fyc.pengpengdd.cyou

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://brr.nanxinkj.top

[S09] C：结构体定义与初始化
来源：http://fwd.gotoacloud.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pqz.hammf.cn

[S10] C：指针与解引用
来源：http://rjl.ehwqpu.com

int *p = &a;  *p = 5;
来源：http://pvl.daria6918.cn

[S11] C：逐行读文件
来源：http://zlh.shanyushiyangkeji.top

FILE *f = fopen("a.txt", "r");
来源：http://wxz.pengpengdd.cyou

while (fgets(buf, sizeof buf, f)) { }
来源：http://rnh.sysykeji.top

fclose(f);
来源：http://cwz.cucudq.cn

[S12] C：写文件
来源：http://jzj.fengsongda.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://twl.hnxiangtu.top

[S13] C：宏定义
来源：http://ybh.yvedp.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://skc.fanxiaobao.xyz

[S14] C：枚举
来源：http://zwu.ivvv.top

enum Color { RED, GREEN, BLUE };
来源：http://owc.jlsjyb.cn

[S15] C：类型转换
来源：http://pbl.yanxiufei.cn

(double) a / b
来源：http://nkw.nanxinkj.top

[S16] C：位操作置位
来源：http://eav.yangfankeji.com

x |= (1 << 3);
来源：http://pfp.zhoulong.xyz

[S17] C：安全拼接字符串
来源：http://oco.ctjpmb.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ylr.tarul.cn

[S18] C：命令行参数
来源：http://tgj.nwbrower.top

int main(int argc, char **argv)
来源：http://gqp.c1oappe.top

[S19] C：快速排序
来源：http://kaq.zhixingplan.top

qsort(a, n, sizeof(int), cmp);
来源：http://ymz.chenlongwang.top

[S20] C：二分查找
来源：http://ocy.jyoumei.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lfg.andypj.xyz

[S21] C：字符类别判断
来源：http://cip.xinyue.icu

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qxi.zhongyouzk.top

[S22] C：字符串转数字
来源：http://iom.jqgufenzy.top

atoi("42");  strtod("3.14", NULL);
来源：http://bno.zhijiandao.cn

[S23] C：随机数
来源：http://gpk.kuanghao11.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://beo.yj20258888.top

[S24] C：获取本地时间
来源：http://vop.316326.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://huz.jqgufenzy.top

[S25] C：内存拷贝
来源：http://pui.yfazqb.com

memcpy(dst, src, n);
来源：http://fho.shangyingyoupin.top

[S26] C：内存清零
来源：http://nab.aibaodan.cn

memset(a, 0, sizeof a);
来源：http://ytn.ctjpmb.com

[S27] C：定义常量
来源：http://ieh.yvedp.cn

const double PI = 3.14159;
来源：http://rpd.nanxuanxn.top

[S28] C：静态变量
来源：http://gns.cdnleiting.top

static int counter = 0;
来源：http://piw.jlsjyb.cn

[S29] C：变参函数
来源：http://emg.zhongyouzk.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ooi.shangyingyoupin.top

[S30] C：头文件保护
来源：http://tqz.jqgfzy.top

#ifndef X_H
来源：http://uai.sysykeji.top

#define X_H
来源：http://nxt.chenzaomai.com

#endif
来源：http://oke.jqgufenzy.top

[S31] C++：Hello World
来源：http://vpv.zhaomingkeji.xyz

#include <iostream>
来源：http://efa.cqqwz.cn

int main() { std::cout << "Hello\n"; }
来源：http://fks.fktsv.cn

[S32] C++：字符串
来源：http://mwz.zhijiandao.cn

std::string s = "hi";  s += "!";
来源：http://crq.sxryk.cn

[S33] C++：vector 增删
来源：http://kgy.jinghuilouyu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://joe.ybcxt.top

[S34] C++：遍历 vector
来源：http://zfx.xuanzx.com

for (auto &x : v) { std::cout << x; }
来源：http://lvd.316326.xyz

[S35] C++：map
来源：http://ssr.ehwqpu.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pmd.shanyushiyangkeji.top

[S36] C++：unordered_map
来源：http://lti.aibaodan.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mqq.hnxiangtu.top

[S37] C++：set
来源：http://iyo.jqgfzy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nou.quarkkingdee.top

[S38] C++：排序
来源：http://cog.jianghu66.top

std::sort(v.begin(), v.end());
来源：http://pum.meibo888.top

[S39] C++：自定义比较器排序
来源：http://ehp.fanxiaobao.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bmq.xuanzx.com

[S40] C++：查找元素
来源：http://btg.yvedp.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bzq.shuidangran.top

[S41] C++：类与构造函数
来源：http://igd.andypj.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://loq.ybcxt.top

[S42] C++：继承与虚函数
来源：http://ify.vehdjk.com

class B : public Base { public: void f() override {} };
来源：http://xgt.cucudq.cn

[S43] C++：智能指针
来源：http://jdn.xuetiantiany.cn

auto p = std::make_unique<int>(5);
来源：http://zwv.fengsongda.top

[S44] C++：引用传参
来源：http://hyx.yj202588.top

void inc(int &x) { ++x; }
来源：http://goa.zhongyouzk.top

[S45] C++：lambda
来源：http://skq.tian-w.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ove.aibaodan.cn

[S46] C++：函数模板
来源：http://cnj.cucudq.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qzj.cucudq.cn

[S47] C++：结构化绑定遍历
来源：http://sel.fanxiaobao.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tle.svipenyu.cn

[S48] C++：逐行读文件
来源：http://ytz.tanke756.top

std::ifstream in("a.txt");  std::string line;
来源：http://hqs.dianchejie.cn

while (std::getline(in, line)) { }
来源：http://eoo.316326.xyz

[S49] C++：写文件
来源：http://gkv.0kj1m.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qry.sysykeji.top

[S50] C++：格式化数字
来源：http://mem.aizwys.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tjm.shzxlz.cn

[S51] C++：显式类型转换
来源：http://twf.daxiang520.top

static_cast<double>(a) / b
来源：http://zfb.chenzaomai.com

[S52] C++：const 与 noexcept
来源：http://rky.tarul.cn

int size() const noexcept { return n_; }
来源：http://ljy.yfazqb.com

[S53] C++：移动语义
来源：http://khs.wangdashe.top

std::vector<int> w = std::move(v);
来源：http://ucg.cucudq.cn

[S54] C++：异常处理
来源：http://fat.fehbvm.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hpt.jinghuilouyu.cn

[S55] C++：结构化绑定
来源：http://jai.wangshuangyany.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gud.chenzaomai.com

[S56] C++：optional
来源：http://vdu.mhx1999.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kxk.hammf.cn

[S57] C++：编译期常量
来源：http://qxg.jiagoushi.top

constexpr int N = 10;
来源：http://hmy.chenlongwang.top

[S58] C++：命名空间
来源：http://koj.pycfn.com

namespace ns { int f() { return 1; } }
来源：http://pmf.ybcxt.top

[S59] C++：静态断言
来源：http://mnq.xuetiantiany.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wae.hysaishi.cn

[S60] C++：遍历并删除元素
来源：http://vms.hfpthk.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fib.xuetiantiany.cn

================================================================================
来源：http://woi.9152youxi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lzq.jqgufenzy.top

================================================================================
来源：http://rra.nwbrower.top

[T01] Kotlin：Hello World
来源：http://nib.cheryme.top

println("Hello")
来源：http://csb.hysaishi.cn

[T02] Kotlin：变量
来源：http://bkd.jiagoushi.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uvp.zhijiandao.cn

[T03] Kotlin：字符串模板
来源：http://xxt.svipenyu.cn

"值: $b"
来源：http://stz.guowangkeji.top

[T04] Kotlin：空安全
来源：http://nyl.yonumen.top

val n: String? = null;  n?.length
来源：http://emz.zhixingplan.top

[T05] Kotlin：when 表达式
来源：http://dea.ppjwa.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://eeg.hcnkem.com

[T06] Kotlin：集合映射
来源：http://ads.jlsjyb.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rmb.kuanghao11.cn

[T07] Kotlin：集合过滤
来源：http://vuy.fengsongda.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://znj.zhengqikj.top

[T08] Kotlin：数据类
来源：http://qnf.gaohongyu789.top

data class User(val name: String, val age: Int)
来源：http://ncs.sweek.top

[T09] Kotlin：扩展函数
来源：http://izn.hnqzz.top

fun String.exclaim() = this + "!"
来源：http://ilx.wangdashe.top

[T10] Kotlin：默认参数
来源：http://ado.vehdjk.com

fun greet(name: String = "World") = "Hi $name"
来源：http://fib.ehwqpu.com

[T11] Kotlin：协程
来源：http://zpc.shanyushiyangkeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://fzl.meibo888.top

[T12] Kotlin：解构声明
来源：http://vfw.dashuyun.cn

val (a, b) = Pair(1, 2)
来源：http://asd.meibo888.top

[T13] Kotlin：只读 Map
来源：http://oef.wangdashe.top

val m = mapOf("a" to 1)
来源：http://vnz.tanke756.top

[T14] Kotlin：循环
来源：http://jha.sweek.top

for (i in 1..10) println(i)
来源：http://rvl.zhengqikj.top

[T15] Kotlin：接口
来源：http://ulk.jinqigfzy.top

interface Shape { fun area(): Double }
来源：http://xck.birdmap.top

[T16] Swift：Hello World
来源：http://zzu.pycfn.com

print("Hello")
来源：http://tog.jinqigfzy.top

[T17] Swift：变量与常量
来源：http://bns.smart0.xyz

var a = 1;  let b = 2
来源：http://vvv.guowangkeji.top

[T18] Swift：字符串插值
来源：http://rjw.andypj.xyz

"值: \(b)"
来源：http://zfx.xinyue.icu

[T19] Swift：可选绑定
来源：http://ucv.jinqigufen.top

if let n = opt { print(n) }
来源：http://otc.gzhubu.top

[T20] Swift：数组操作
来源：http://jah.ehwqpu.com

var a = [1, 2, 3];  a.append(4)
来源：http://ove.jqgufenzy.top

[T21] Swift：遍历
来源：http://lxf.hysaishi.cn

for x in a { print(x) }
来源：http://ugw.yuxming.cn

[T22] Swift：字典
来源：http://kuo.zdbjq.cn

var d = ["a": 1];  d["b"] = 2
来源：http://tmf.xziqi.cn

[T23] Swift：函数
来源：http://rpi.daria6918.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gwd.chenjidiqi.icu

[T24] Swift：闭包
来源：http://zzi.daxiang520.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://fzl.jiagoushi.top

[T25] Swift：结构体
来源：http://sgn.yj20258888.top

struct P { var x: Int }
来源：http://waj.xuetiantiany.cn

[T26] Swift：类与重写
来源：http://eqr.hysaishi.cn

class A: Base { override func f() {} }
来源：http://mpg.xingfuxueyuan.xyz

[T27] Swift：错误处理
来源：http://npy.birdmap.top

do { try f() } catch { print(error) }
来源：http://rlg.sjlbkw.cn

[T28] Swift：枚举
来源：http://gmb.smart0.xyz

enum Color { case red, green }
来源：http://qsw.hywenlv.cn

[T29] Swift：guard 提前返回
来源：http://dhv.hnqzz.top

guard let x = opt else { return }
来源：http://khe.316326.xyz

[T30] Swift：协议
来源：http://vlx.tianlin.xyz

protocol Shape { func area() -> Double }
来源：http://nsi.zhengqikj.top

[T31] Lua：Hello World
来源：http://pue.tarul.cn

print("Hello")
来源：http://zgw.fehbvm.com

[T32] Lua：局部变量
来源：http://xzw.cucudq.cn

local a = 1
来源：http://epw.vehdjk.com

[T33] Lua：表（数组）
来源：http://xdr.epnwcf.com

local t = {1, 2, 3};  t[4] = 4
来源：http://ujb.yuanzhike.top

[T34] Lua：遍历表
来源：http://abe.guannengcc.top

for i, v in ipairs(t) do print(i, v) end
来源：http://kmr.yuxming.cn

[T35] Lua：字典表
来源：http://uic.zhongyouzk.top

local d = { a = 1 };  d.b = 2
来源：http://hdx.ehwqpu.com

[T36] Lua：函数
来源：http://qmx.xingfuxueyuan.xyz

function add(a, b) return a + b end
来源：http://omv.hnqzz.top

[T37] Lua：字符串拼接
来源：http://vgm.zhongyouzk.top

"a" .. "b"
来源：http://rfp.sysykeji.top

[T38] Lua：条件
来源：http://wwf.chenzaomai.com

if x > 0 then print("正") end
来源：http://uds.jlsjyb.cn

[T39] Lua：模式匹配
来源：http://nrc.yueranfly.top

string.find(s, "%d+")
来源：http://wqo.ctjpmb.com

[T40] Lua：元表
来源：http://mwp.andypj.xyz

setmetatable({}, { __index = base })
来源：http://sjd.yueranfly.top

[T41] Perl：Hello World
来源：http://euh.fehbvm.com

print "Hello\n";
来源：http://uer.ybcxt.top

[T42] Perl：变量类型
来源：http://kyn.c1oappe.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qbn.haohaochexian.top

[T43] Perl：字符串插值
来源：http://mql.316326.xyz

"值: $a"
来源：http://myj.xziqi.cn

[T44] Perl：条件
来源：http://mdn.jqgufenzy.top

if ($a > 0) { print "正"; }
来源：http://fcz.shangyingyoupin.top

[T45] Perl：数组遍历
来源：http://ssw.sysykeji.top

for my $x (@arr) { print $x; }
来源：http://hfk.andypj.xyz

[T46] Perl：哈希操作
来源：http://sdn.jinyuanbaomall.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mmf.sysykeji.top

[T47] Perl：正则捕获
来源：http://rmf.c1oappe.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://dvs.kuanghao11.cn

[T48] Perl：正则替换
来源：http://xxr.zhixingplan.top

$s =~ s/old/new/g;
来源：http://elc.316326.xyz

[T49] Perl：函数
来源：http://etu.yangfankeji.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://uqk.zdqjudy.top

[T50] Perl：逐行读文件
来源：http://afn.jinghuilouyu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://mbp.ywan-chungtsiang.top

while (my $line = <$fh>) { print $line; }
来源：http://bwd.shanyushiyangtech.top

[T51] Scala：Hello World
来源：http://mmg.yueranfly.top

println("Hello")
来源：http://qpz.shuidangran.top

[T52] Scala：变量
来源：http://vtk.c1oappe.top


<!-- 参考信息 -->