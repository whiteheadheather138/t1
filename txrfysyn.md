代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://avv.jqgufenzy.top

[R52] 统计行数
来源：http://jdv.hesvh.cn

wc -l a.txt
来源：http://hgd.fktsv.cn

[R53] 查看文件头与实时尾
来源：http://hjs.ydjk.org.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vpm.gzhubu.top

[R54] 比较两个文件
来源：http://heu.shangyingyoupin.top

diff a.txt b.txt
来源：http://pby.yvedp.cn

[R55] 压缩与解压
来源：http://zrs.xingfuxueyuan.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rmz.zhongyouzk.top

[R56] 远程拷贝
来源：http://anq.zycfv.cn

scp file user@host:/path/
来源：http://yme.pycfn.com

[R57] 远程执行命令
来源：http://eqe.haohaochexian.top

ssh user@host 'uptime'
来源：http://hmi.gzhubu.top

[R58] 下载文件
来源：http://ohy.hnxiangtu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kqx.mhx1999.top

[R59] 发 POST JSON
来源：http://ukl.aizwys.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gdm.hysaishi.cn

[R60] 只看 HTTP 状态码
来源：http://zmr.yj20258888.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rsm.zhijiandao.cn

[R61] 磁盘占用
来源：http://bxl.ehwqpu.com

df -h;  du -sh *
来源：http://voy.fanxiaobao.xyz

[R62] 找最占空间的文件
来源：http://kwf.iojbl.cn

du -ah . | sort -rh | head -10
来源：http://csv.meibo888.top

[R63] 内存与进程
来源：http://cpa.shanyushiyangtech.top

free -h;  ps aux | grep nginx
来源：http://wjf.shzxlz.cn

[R64] 结束进程
来源：http://mpc.nanxinkj.top

kill -9 $(pgrep -f app.py)
来源：http://vms.cqqwz.cn

[R65] 查看端口占用
来源：http://ssp.kuanghao11.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ovd.chenlongwang.top

[R66] 定时任务
来源：http://pni.ivvv.top

crontab -e;  crontab -l
来源：http://gib.zhijiandao.cn

[R67] 生成随机十六进制串
来源：http://kzw.zdqjudy.top

openssl rand -hex 16
来源：http://ofe.sysykeji.top

[R68] 计算文件校验值
来源：http://nes.yueranfly.top

sha256sum a.txt;  md5sum a.txt
来源：http://kow.sysykeji.top

[R69] 生成随机密码
来源：http://bze.dashuyun.cn

head -c 16 /dev/urandom | base64
来源：http://nnq.nanxuanxn.top

[R70] 时间戳与互转
来源：http://wmk.jinqigfzy.top

date +%s;  date -d @1700000000
来源：http://gkn.shanyushiyangtech.top

[R71] 日期格式化
来源：http://lid.daria6918.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bzw.hcnkem.com

[R72] 等待端口就绪
来源：http://zzg.tian-w.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://kcq.sweek.top

[R73] 分割大日志
来源：http://kpl.xingfuxueyuan.xyz

split -l 1000 big.log part_
来源：http://fhs.hesvh.cn

[R74] 批量重命名
来源：http://stj.yuxming.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ihj.hnxiangtu.top

[R75] 导出环境变量
来源：http://nss.gotoacloud.top

export PATH="$HOME/bin:$PATH"
来源：http://own.zhaomingkeji.xyz

[R76] 使用临时文件
来源：http://osc.jinqigufen.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cmn.zhiwuduotai.top

[R77] 读取用户输入
来源：http://lgq.yonumen.top

read -rp "请输入: " ans
来源：http://omg.shanyushiyangkeji.top

[R78] 交互式菜单
来源：http://ntn.yanxiufei.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://cow.gotoacloud.top

[R79] 解析命令行选项
来源：http://fkr.ydzc1.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://voy.tanke756.top

[R80] 查看脚本执行耗时
来源：http://thj.iojbl.cn

time ./run.sh
来源：http://zzn.c1oappe.top

================================================================================
来源：http://hsf.zdbjq.cn

S. C / C++ 专题
来源：http://cqr.sxryk.cn

================================================================================
来源：http://yzk.ybcxt.top

[S01] C：Hello World
来源：http://nbi.gzhubu.top

#include <stdio.h>
来源：http://gfc.ybcxt.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://dcl.sufxvd.cn

[S02] C：变量与格式化输出
来源：http://fqv.xingfuxueyuan.xyz

int a = 10; printf("%d\n", a);
来源：http://ykl.zhixingplan.top

[S03] C：读入整数
来源：http://ura.tanke756.top

int x; scanf("%d", &x);
来源：http://jub.shanyushiyangkeji.top

[S04] C：字符串复制
来源：http://slx.havefunace.top

char dst[32]; strcpy(dst, "hi");
来源：http://onr.zhoulong.xyz

[S05] C：字符串长度
来源：http://iko.hongshengwenyu.top

strlen(s)
来源：http://xkr.nanxinkj.top

[S06] C：字符串比较
来源：http://fvx.daxiang520.top

strcmp(a, b) == 0
来源：http://hsn.jianghu66.top

[S07] C：数组遍历求和
来源：http://ywo.hfpthk.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bsn.vehdjk.com

[S08] C：动态内存分配与释放
来源：http://ouo.kuanghao11.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ftb.shangyingyoupin.top

[S09] C：结构体定义与初始化
来源：http://wrj.yj20258888.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nmw.redwolf501.top

[S10] C：指针与解引用
来源：http://tlm.yvedp.cn

int *p = &a;  *p = 5;
来源：http://njf.iojbl.cn

[S11] C：逐行读文件
来源：http://izt.tian-w.cn

FILE *f = fopen("a.txt", "r");
来源：http://mha.yfazqb.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://dva.kuanghao11.cn

fclose(f);
来源：http://wtu.hammf.cn

[S12] C：写文件
来源：http://qxg.tanke756.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qwd.jiagoushi.top

[S13] C：宏定义
来源：http://mht.tian-w.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ite.jianghu66.top

[S14] C：枚举
来源：http://naf.ctjpmb.com

enum Color { RED, GREEN, BLUE };
来源：http://woi.yongpay.top

[S15] C：类型转换
来源：http://mrd.zhaomingkeji.xyz

(double) a / b
来源：http://fxp.yvedp.cn

[S16] C：位操作置位
来源：http://cpf.tarul.cn

x |= (1 << 3);
来源：http://pkk.xuanzx.com

[S17] C：安全拼接字符串
来源：http://yjd.yj20258888.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xik.aizwys.cn

[S18] C：命令行参数
来源：http://dgv.gaohongyu789.top

int main(int argc, char **argv)
来源：http://fcz.sxryk.cn

[S19] C：快速排序
来源：http://ghp.yj202588.top

qsort(a, n, sizeof(int), cmp);
来源：http://cwm.zhaomingkeji.xyz

[S20] C：二分查找
来源：http://qlr.shanyushiyangtech.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://czl.zhaomingkeji.xyz

[S21] C：字符类别判断
来源：http://cbw.shanyushiyangkeji.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nuj.zhijiandao.cn

[S22] C：字符串转数字
来源：http://gwe.yuanzhike.top

atoi("42");  strtod("3.14", NULL);
来源：http://ldw.fehbvm.com

[S23] C：随机数
来源：http://lvg.gaohongyu789.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ehd.yvedp.cn

[S24] C：获取本地时间
来源：http://epi.xinyue.icu

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://eaw.iojbl.cn

[S25] C：内存拷贝
来源：http://exf.ctjpmb.com

memcpy(dst, src, n);
来源：http://ndq.fzhhl.top

[S26] C：内存清零
来源：http://zgc.hammf.cn

memset(a, 0, sizeof a);
来源：http://qvc.c1oappe.top

[S27] C：定义常量
来源：http://cyv.ctjpmb.com

const double PI = 3.14159;
来源：http://nul.tianlin.xyz

[S28] C：静态变量
来源：http://nda.sweek.top

static int counter = 0;
来源：http://bbw.zycfv.cn

[S29] C：变参函数
来源：http://ags.yuxming.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qif.jianghu66.top

[S30] C：头文件保护
来源：http://syp.9152youxi.cn

#ifndef X_H
来源：http://rxm.guowangkeji.top

#define X_H
来源：http://dsz.shzxlz.cn

#endif
来源：http://jcd.aibaodan.cn

[S31] C++：Hello World
来源：http://ymf.sysykeji.top

#include <iostream>
来源：http://tzp.feifeiyinyue.top

int main() { std::cout << "Hello\n"; }
来源：http://tor.kuanghao11.cn

[S32] C++：字符串
来源：http://wmc.ydjk.org.cn

std::string s = "hi";  s += "!";
来源：http://qeg.shuidangran.top

[S33] C++：vector 增删
来源：http://lce.zhaomingkeji.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://plg.ydzc1.top

[S34] C++：遍历 vector
来源：http://urn.yj202588.top

for (auto &x : v) { std::cout << x; }
来源：http://noj.jiagoushi.top

[S35] C++：map
来源：http://oba.cucudq.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kvy.zycfv.cn

[S36] C++：unordered_map
来源：http://phd.cucudq.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bhw.svipenyu.cn

[S37] C++：set
来源：http://ils.shanyushiyangtech.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qqd.bjfxy.top

[S38] C++：排序
来源：http://aui.ppjwa.cn

std::sort(v.begin(), v.end());
来源：http://kmm.pycfn.com

[S39] C++：自定义比较器排序
来源：http://vwn.zhijiandao.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cbx.guannengcc.top

[S40] C++：查找元素
来源：http://wmg.pengpengdd.cyou

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qdr.zhongyouzk.top

[S41] C++：类与构造函数
来源：http://pru.aibaodan.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pxc.kuanghao11.cn

[S42] C++：继承与虚函数
来源：http://hej.vehdjk.com

class B : public Base { public: void f() override {} };
来源：http://bth.andypj.xyz

[S43] C++：智能指针
来源：http://ahx.cashguo.top

auto p = std::make_unique<int>(5);
来源：http://mul.smart0.xyz

[S44] C++：引用传参
来源：http://sjx.chenjidiqi.icu

void inc(int &x) { ++x; }
来源：http://ldy.jlsjyb.cn

[S45] C++：lambda
来源：http://mru.9152youxi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gfi.jinyuanbaomall.cn

[S46] C++：函数模板
来源：http://wbj.sxryk.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ipa.shanyushiyangtech.top

[S47] C++：结构化绑定遍历
来源：http://ccn.epnwcf.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xqd.shanyushiyangkeji.top

[S48] C++：逐行读文件
来源：http://fth.chenzaomai.com

std::ifstream in("a.txt");  std::string line;
来源：http://qzb.bjfxy.top

while (std::getline(in, line)) { }
来源：http://zgc.ydjk.org.cn

[S49] C++：写文件
来源：http://jks.haohaochexian.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lae.fengsongda.top

[S50] C++：格式化数字
来源：http://ucb.feifeiyinyue.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://idb.jianghu66.top

[S51] C++：显式类型转换
来源：http://uti.zhijiandao.cn

static_cast<double>(a) / b
来源：http://olf.uphjek.com

[S52] C++：const 与 noexcept
来源：http://yva.quarkkingdee.top

int size() const noexcept { return n_; }
来源：http://pao.zhoulong.xyz

[S53] C++：移动语义
来源：http://gco.nanxuanxn.top

std::vector<int> w = std::move(v);
来源：http://rxn.pengpengdd.cyou

[S54] C++：异常处理
来源：http://wyu.chenjidiqi.icu

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://twd.zhiwuduotai.top

[S55] C++：结构化绑定
来源：http://mzr.iojbl.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qtg.9152youxi.cn

[S56] C++：optional
来源：http://nxt.cqqwz.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://prh.52xcode.cn

[S57] C++：编译期常量
来源：http://hbp.tianlin.xyz

constexpr int N = 10;
来源：http://xvd.yuanzhike.top

[S58] C++：命名空间
来源：http://yqh.yvedp.cn

namespace ns { int f() { return 1; } }
来源：http://kgm.birdmap.top

[S59] C++：静态断言
来源：http://css.vehdjk.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vhe.jianghu66.top

[S60] C++：遍历并删除元素
来源：http://ipn.sufxvd.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ehg.iojbl.cn

================================================================================
来源：http://tlr.xuetiantiany.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ysl.yvedp.cn

================================================================================
来源：http://mar.tianlin.xyz

[T01] Kotlin：Hello World
来源：http://tuj.yj20258.top

println("Hello")
来源：http://vwl.sjlbkw.cn

[T02] Kotlin：变量
来源：http://vcx.xinyue.icu

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cmx.fengsongda.top

[T03] Kotlin：字符串模板
来源：http://wez.shanyushiyangkeji.top

"值: $b"
来源：http://znu.dashuyun.cn

[T04] Kotlin：空安全
来源：http://xmv.sjlbkw.cn

val n: String? = null;  n?.length
来源：http://nvo.xuetiantiany.cn

[T05] Kotlin：when 表达式
来源：http://yxg.nanxinkj.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sij.hnqzz.top

[T06] Kotlin：集合映射
来源：http://chy.epnwcf.com

listOf(1, 2, 3).map { it * 2 }
来源：http://bsb.bbcook.cn

[T07] Kotlin：集合过滤
来源：http://mzb.bjfxy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://xoh.feifeiyinyue.top

[T08] Kotlin：数据类
来源：http://fhh.yfazqb.com

data class User(val name: String, val age: Int)
来源：http://kpp.0kj1m.cn

[T09] Kotlin：扩展函数
来源：http://dzm.chenlongwang.top

fun String.exclaim() = this + "!"
来源：http://emv.cheryme.top

[T10] Kotlin：默认参数
来源：http://vdm.yongpay.top

fun greet(name: String = "World") = "Hi $name"
来源：http://tgv.cdnleiting.top

[T11] Kotlin：协程
来源：http://foa.c1oappe.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ayg.pengpengdd.cyou

[T12] Kotlin：解构声明
来源：http://ckp.9152youxi.cn

val (a, b) = Pair(1, 2)
来源：http://lsv.quarkkingdee.top

[T13] Kotlin：只读 Map
来源：http://sey.shanyushiyangtech.top

val m = mapOf("a" to 1)
来源：http://csl.jinqigufen.top

[T14] Kotlin：循环
来源：http://usr.birdmap.top

for (i in 1..10) println(i)
来源：http://zyk.gogol.net.cn

[T15] Kotlin：接口
来源：http://ukx.ehwqpu.com

interface Shape { fun area(): Double }
来源：http://iuc.jlsjyb.cn

[T16] Swift：Hello World
来源：http://hyo.ydjk.org.cn

print("Hello")
来源：http://vrq.jlsjyb.cn

[T17] Swift：变量与常量
来源：http://zys.jinqigfzy.top

var a = 1;  let b = 2
来源：http://pxo.haohaochexian.top

[T18] Swift：字符串插值
来源：http://dhv.bbcook.cn

"值: \(b)"
来源：http://faj.dashuyun.cn

[T19] Swift：可选绑定
来源：http://krv.shanyushiyangtech.top

if let n = opt { print(n) }
来源：http://qkw.nwbrower.top

[T20] Swift：数组操作
来源：http://yzk.xingfuxueyuan.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://nlz.xuetiantiany.cn

[T21] Swift：遍历
来源：http://fzh.haohaochexian.top

for x in a { print(x) }
来源：http://txk.zhiwuduotai.top

[T22] Swift：字典
来源：http://knj.tian-w.cn

var d = ["a": 1];  d["b"] = 2
来源：http://izg.shangyingyoupin.top

[T23] Swift：函数
来源：http://zek.daxiang520.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://aeu.meibo888.top

[T24] Swift：闭包
来源：http://exn.jianghu66.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://exg.nwbrower.top

[T25] Swift：结构体
来源：http://nco.tanke756.top

struct P { var x: Int }
来源：http://zxp.gaohongyu789.top

[T26] Swift：类与重写
来源：http://hup.wangdashe.top

class A: Base { override func f() {} }
来源：http://gjz.tian-w.cn

[T27] Swift：错误处理
来源：http://dut.shanyushiyangkeji.top

do { try f() } catch { print(error) }
来源：http://xxp.dashuyun.cn

[T28] Swift：枚举
来源：http://sxq.jqgufenzy.top

enum Color { case red, green }
来源：http://uie.sjlbkw.cn

[T29] Swift：guard 提前返回
来源：http://xrn.gotoacloud.top

guard let x = opt else { return }
来源：http://rvz.yj20258888.top

[T30] Swift：协议
来源：http://fte.yongpay.top

protocol Shape { func area() -> Double }
来源：http://apl.jinyuanbaomall.cn

[T31] Lua：Hello World
来源：http://dpg.epnwcf.com

print("Hello")
来源：http://wrf.shuidangran.top

[T32] Lua：局部变量
来源：http://xmz.daxiang520.top

local a = 1
来源：http://onk.sxryk.cn

[T33] Lua：表（数组）
来源：http://iih.chenjidiqi.icu

local t = {1, 2, 3};  t[4] = 4
来源：http://qup.vqdsnc.cn

[T34] Lua：遍历表
来源：http://upi.nwbrower.top

for i, v in ipairs(t) do print(i, v) end
来源：http://gct.tian-w.cn

[T35] Lua：字典表
来源：http://yrq.shzxlz.cn

local d = { a = 1 };  d.b = 2
来源：http://jfc.jqgufenzy.top

[T36] Lua：函数
来源：http://pet.yj20258.top

function add(a, b) return a + b end
来源：http://cji.ywan-chungtsiang.top

[T37] Lua：字符串拼接
来源：http://zwy.9152youxi.cn

"a" .. "b"
来源：http://zmn.bjfxy.top

[T38] Lua：条件
来源：http://ukq.hcnkem.com

if x > 0 then print("正") end
来源：http://eqx.havefunace.top

[T39] Lua：模式匹配
来源：http://bib.cqqwz.cn

string.find(s, "%d+")
来源：http://ewu.316326.xyz

[T40] Lua：元表
来源：http://wlg.dianchejie.cn

setmetatable({}, { __index = base })
来源：http://hve.smart0.xyz

[T41] Perl：Hello World
来源：http://uyu.tanke756.top

print "Hello\n";
来源：http://lfc.hywenlv.cn

[T42] Perl：变量类型
来源：http://cig.cheryme.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gyh.bbcook.cn

[T43] Perl：字符串插值
来源：http://ues.tanke756.top

"值: $a"
来源：http://iev.ybcxt.top

[T44] Perl：条件
来源：http://zbs.bbcook.cn

if ($a > 0) { print "正"; }
来源：http://xrh.nanxuanxn.top

[T45] Perl：数组遍历
来源：http://udw.yj20258.top

for my $x (@arr) { print $x; }
来源：http://dix.hnqzz.top

[T46] Perl：哈希操作
来源：http://xed.pycfn.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gdz.0kj1m.cn

[T47] Perl：正则捕获
来源：http://uhq.mhx1999.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ppo.wangshuangyany.cn

[T48] Perl：正则替换
来源：http://zws.zhengqikj.top

$s =~ s/old/new/g;
来源：http://cjc.jinqigfzy.top

[T49] Perl：函数
来源：http://atk.fzhhl.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bgl.yangfankeji.com

[T50] Perl：逐行读文件
来源：http://zgd.nanxuanxn.top

open my $fh, "<", "a.txt" or die $!;
来源：http://pjb.ydjk.org.cn

while (my $line = <$fh>) { print $line; }
来源：http://cyi.andypj.xyz

[T51] Scala：Hello World
来源：http://uci.ivvv.top

println("Hello")
来源：http://tae.yuxming.cn

[T52] Scala：变量
来源：http://kbz.tanke756.top

val a = 1;  var b = 2
来源：http://uqy.shanyushiyangtech.top

[T53] Scala：字符串插值
来源：http://tfz.feifeiyinyue.top

s"值: $b"
来源：http://zgq.feifeiyinyue.top

[T54] Scala：集合映射
来源：http://zen.havefunace.top


<!-- 参考信息 -->