代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gsb.fehbvm.com

[R50] awk 求和
来源：http://ubd.shanyushiyangkeji.top

awk '{s += $2} END {print s}' a.txt
来源：http://zxn.iojbl.cn

[R51] 排序去重取前几
来源：http://khd.hnqzz.top

sort a.txt | uniq -c | sort -rn | head
来源：http://hft.jiagoushi.top

[R52] 统计行数
来源：http://fnr.fehbvm.com

wc -l a.txt
来源：http://srb.nwbrower.top

[R53] 查看文件头与实时尾
来源：http://zgq.zhiwuduotai.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://idu.nwbrower.top

[R54] 比较两个文件
来源：http://tkq.birdmap.top

diff a.txt b.txt
来源：http://apk.bjfxy.top

[R55] 压缩与解压
来源：http://phv.ydzc1.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uki.sufxvd.cn

[R56] 远程拷贝
来源：http://itb.nanxuanxn.top

scp file user@host:/path/
来源：http://toi.vqdsnc.cn

[R57] 远程执行命令
来源：http://gvo.zdbjq.cn

ssh user@host 'uptime'
来源：http://lxk.shangyingyoupin.top

[R58] 下载文件
来源：http://oup.xinyue.icu

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lvt.zdqjudy.top

[R59] 发 POST JSON
来源：http://tlh.yvedp.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pli.tanke756.top

[R60] 只看 HTTP 状态码
来源：http://wcl.zdbjq.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://myy.cucudq.cn

[R61] 磁盘占用
来源：http://zxa.hongshengwenyu.top

df -h;  du -sh *
来源：http://msw.fengsongda.top

[R62] 找最占空间的文件
来源：http://zsi.dashuyun.cn

du -ah . | sort -rh | head -10
来源：http://vnr.tian-w.cn

[R63] 内存与进程
来源：http://crm.meibo888.top

free -h;  ps aux | grep nginx
来源：http://agq.vehdjk.com

[R64] 结束进程
来源：http://jgj.vehdjk.com

kill -9 $(pgrep -f app.py)
来源：http://dog.hcnkem.com

[R65] 查看端口占用
来源：http://akd.yanxiufei.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hwg.yonumen.top

[R66] 定时任务
来源：http://krq.sxryk.cn

crontab -e;  crontab -l
来源：http://etj.iojbl.cn

[R67] 生成随机十六进制串
来源：http://nqd.yj202588.top

openssl rand -hex 16
来源：http://xzm.ydjk.org.cn

[R68] 计算文件校验值
来源：http://ldy.zycfv.cn

sha256sum a.txt;  md5sum a.txt
来源：http://dif.yj202588.top

[R69] 生成随机密码
来源：http://mnw.yvedp.cn

head -c 16 /dev/urandom | base64
来源：http://fdq.iojbl.cn

[R70] 时间戳与互转
来源：http://lzc.hnqzz.top

date +%s;  date -d @1700000000
来源：http://hdg.yj20258.top

[R71] 日期格式化
来源：http://mfq.dashuyun.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://gbh.9152youxi.cn

[R72] 等待端口就绪
来源：http://vyf.nanxuanxn.top

until nc -z localhost 3306; do sleep 1; done
来源：http://lfy.yj20258888.top

[R73] 分割大日志
来源：http://jre.yonumen.top

split -l 1000 big.log part_
来源：http://vsf.zhixingplan.top

[R74] 批量重命名
来源：http://vjl.jyoumei.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jna.hesvh.cn

[R75] 导出环境变量
来源：http://jya.gaohongyu789.top

export PATH="$HOME/bin:$PATH"
来源：http://arf.ctjpmb.com

[R76] 使用临时文件
来源：http://bfs.jianghu66.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dup.cashguo.top

[R77] 读取用户输入
来源：http://jtt.316326.xyz

read -rp "请输入: " ans
来源：http://dyz.svipenyu.cn

[R78] 交互式菜单
来源：http://xdh.birdmap.top

select opt in a b c; do echo "$opt"; break; done
来源：http://vwh.yj20258.top

[R79] 解析命令行选项
来源：http://sco.quarkkingdee.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jyj.shangyingyoupin.top

[R80] 查看脚本执行耗时
来源：http://avr.ivvv.top

time ./run.sh
来源：http://ezf.fzhhl.top

================================================================================
来源：http://adv.yuanzhike.top

S. C / C++ 专题
来源：http://lho.hesvh.cn

================================================================================
来源：http://ach.vqdsnc.cn

[S01] C：Hello World
来源：http://ptg.dashuyun.cn

#include <stdio.h>
来源：http://spt.smart0.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://buu.gzhubu.top

[S02] C：变量与格式化输出
来源：http://xdm.gaohongyu789.top

int a = 10; printf("%d\n", a);
来源：http://xea.pycfn.com

[S03] C：读入整数
来源：http://xfm.pengpengdd.cyou

int x; scanf("%d", &x);
来源：http://vmz.xingfuxueyuan.xyz

[S04] C：字符串复制
来源：http://nml.redwolf501.top

char dst[32]; strcpy(dst, "hi");
来源：http://zvw.andypj.xyz

[S05] C：字符串长度
来源：http://pkj.jqgfzy.top

strlen(s)
来源：http://vir.havefunace.top

[S06] C：字符串比较
来源：http://xon.shzxlz.cn

strcmp(a, b) == 0
来源：http://lfx.ywan-chungtsiang.top

[S07] C：数组遍历求和
来源：http://tzy.pycfn.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://omk.xuetiantiany.cn

[S08] C：动态内存分配与释放
来源：http://ayq.c1oappe.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zpy.xingfuxueyuan.xyz

[S09] C：结构体定义与初始化
来源：http://ntt.redwolf501.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vwk.ybcxt.top

[S10] C：指针与解引用
来源：http://tal.feifeiyinyue.top

int *p = &a;  *p = 5;
来源：http://nzq.shanyushiyangtech.top

[S11] C：逐行读文件
来源：http://wsf.zdqjudy.top

FILE *f = fopen("a.txt", "r");
来源：http://cwt.jinqigfzy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://cbw.zycfv.cn

fclose(f);
来源：http://gxl.daxiang520.top

[S12] C：写文件
来源：http://lfw.ppjwa.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tcy.guowangkeji.top

[S13] C：宏定义
来源：http://myk.c1oappe.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fuw.hysaishi.cn

[S14] C：枚举
来源：http://kui.hcnkem.com

enum Color { RED, GREEN, BLUE };
来源：http://mmp.tian-w.cn

[S15] C：类型转换
来源：http://fdz.ydzc1.top

(double) a / b
来源：http://geu.smart0.xyz

[S16] C：位操作置位
来源：http://uzd.pengpengdd.cyou

x |= (1 << 3);
来源：http://mnm.cqqwz.cn

[S17] C：安全拼接字符串
来源：http://erw.ppjwa.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://usd.yj20258.top

[S18] C：命令行参数
来源：http://cqr.aibaodan.cn

int main(int argc, char **argv)
来源：http://tcq.gaohongyu789.top

[S19] C：快速排序
来源：http://fvy.zhiwuduotai.top

qsort(a, n, sizeof(int), cmp);
来源：http://xxx.pengpengdd.cyou

[S20] C：二分查找
来源：http://nft.havefunace.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://opu.guannengcc.top

[S21] C：字符类别判断
来源：http://ycz.yuanzhike.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xvm.yfazqb.com

[S22] C：字符串转数字
来源：http://xgt.zycfv.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ags.zdqjudy.top

[S23] C：随机数
来源：http://bcb.tanke756.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ebu.yj20258.top

[S24] C：获取本地时间
来源：http://muu.chenlongwang.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xtk.chenzaomai.com

[S25] C：内存拷贝
来源：http://itw.shuidangran.top

memcpy(dst, src, n);
来源：http://soj.hongshengwenyu.top

[S26] C：内存清零
来源：http://zcl.jiagoushi.top

memset(a, 0, sizeof a);
来源：http://dhl.daria6918.cn

[S27] C：定义常量
来源：http://hbv.epnwcf.com

const double PI = 3.14159;
来源：http://hwg.meibo888.top

[S28] C：静态变量
来源：http://qmf.gotoacloud.top

static int counter = 0;
来源：http://prn.xingfuxueyuan.xyz

[S29] C：变参函数
来源：http://tly.svipenyu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mcf.guannengcc.top

[S30] C：头文件保护
来源：http://ibg.shzxlz.cn

#ifndef X_H
来源：http://iuo.hfpthk.cn

#define X_H
来源：http://cyg.jlsjyb.cn

#endif
来源：http://zqj.chenlongwang.top

[S31] C++：Hello World
来源：http://nhv.jqgfzy.top

#include <iostream>
来源：http://ong.zhiwuduotai.top

int main() { std::cout << "Hello\n"; }
来源：http://wwd.sjlbkw.cn

[S32] C++：字符串
来源：http://wuw.meibo888.top

std::string s = "hi";  s += "!";
来源：http://fiy.ehwqpu.com

[S33] C++：vector 增删
来源：http://htr.jlsjyb.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mfy.hywenlv.cn

[S34] C++：遍历 vector
来源：http://qnw.zhiwuduotai.top

for (auto &x : v) { std::cout << x; }
来源：http://lib.ppjwa.cn

[S35] C++：map
来源：http://zkz.nwbrower.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ckq.vqdsnc.cn

[S36] C++：unordered_map
来源：http://nsb.fanxiaobao.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tmu.wangdashe.top

[S37] C++：set
来源：http://crx.52xcode.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xoe.jianghu66.top

[S38] C++：排序
来源：http://xil.ehwqpu.com

std::sort(v.begin(), v.end());
来源：http://rcj.jinqigfzy.top

[S39] C++：自定义比较器排序
来源：http://qvs.iojbl.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fmm.jianghu66.top

[S40] C++：查找元素
来源：http://vmf.andypj.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://moj.ivvv.top

[S41] C++：类与构造函数
来源：http://iaj.xylfe.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nsp.snrcjt.cn

[S42] C++：继承与虚函数
来源：http://ogw.jinqigufen.top

class B : public Base { public: void f() override {} };
来源：http://urt.chenzaomai.com

[S43] C++：智能指针
来源：http://szh.bbcook.cn

auto p = std::make_unique<int>(5);
来源：http://rfr.yj20258888.top

[S44] C++：引用传参
来源：http://cox.daxiang520.top

void inc(int &x) { ++x; }
来源：http://emz.jinyuanbaomall.cn

[S45] C++：lambda
来源：http://ezo.hcnkem.com

auto add = [](int a, int b) { return a + b; };
来源：http://cqa.cqqwz.cn

[S46] C++：函数模板
来源：http://vzx.havefunace.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cri.pengpengdd.cyou

[S47] C++：结构化绑定遍历
来源：http://arq.jinghuilouyu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xwu.aibaodan.cn

[S48] C++：逐行读文件
来源：http://fus.zhoulong.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://rue.cqqwz.cn

while (std::getline(in, line)) { }
来源：http://vyz.jyoumei.cn

[S49] C++：写文件
来源：http://qbd.daria6918.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bpm.guannengcc.top

[S50] C++：格式化数字
来源：http://rwt.ydzc1.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uxm.feifeiyinyue.top

[S51] C++：显式类型转换
来源：http://eak.tian-w.cn

static_cast<double>(a) / b
来源：http://koh.tarul.cn

[S52] C++：const 与 noexcept
来源：http://cca.zhengqikj.top

int size() const noexcept { return n_; }
来源：http://wnn.shangyingyoupin.top

[S53] C++：移动语义
来源：http://vge.havefunace.top

std::vector<int> w = std::move(v);
来源：http://aou.hammf.cn

[S54] C++：异常处理
来源：http://tcr.fehbvm.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wds.yangfankeji.com

[S55] C++：结构化绑定
来源：http://wfa.andypj.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://jfb.pycfn.com

[S56] C++：optional
来源：http://qvc.yangfankeji.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kjx.wangshuangyany.cn

[S57] C++：编译期常量
来源：http://rfw.zycfv.cn

constexpr int N = 10;
来源：http://xdv.cashguo.top

[S58] C++：命名空间
来源：http://cil.yangfankeji.com

namespace ns { int f() { return 1; } }
来源：http://xmv.nanxuanxn.top

[S59] C++：静态断言
来源：http://ylq.ywan-chungtsiang.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dsk.jianghu66.top

[S60] C++：遍历并删除元素
来源：http://ndr.guowangkeji.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qlq.xingfuxueyuan.xyz

================================================================================
来源：http://ytj.xylfe.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hbf.cashguo.top

================================================================================
来源：http://xwr.fehbvm.com

[T01] Kotlin：Hello World
来源：http://feg.yanxiufei.cn

println("Hello")
来源：http://zli.shangyingyoupin.top

[T02] Kotlin：变量
来源：http://puh.c1oappe.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uzv.sweek.top

[T03] Kotlin：字符串模板
来源：http://xbc.gaohongyu789.top

"值: $b"
来源：http://qmu.tanke756.top

[T04] Kotlin：空安全
来源：http://rxt.316326.xyz

val n: String? = null;  n?.length
来源：http://dnp.yj20258888.top

[T05] Kotlin：when 表达式
来源：http://utq.daxiang520.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hwv.havefunace.top

[T06] Kotlin：集合映射
来源：http://msh.jinqigfzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://tjh.zdbjq.cn

[T07] Kotlin：集合过滤
来源：http://jby.ywan-chungtsiang.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://kaa.ehwqpu.com

[T08] Kotlin：数据类
来源：http://xsb.haohaochexian.top

data class User(val name: String, val age: Int)
来源：http://woy.daria6918.cn

[T09] Kotlin：扩展函数
来源：http://lez.yuanzhike.top

fun String.exclaim() = this + "!"
来源：http://fya.snrcjt.cn

[T10] Kotlin：默认参数
来源：http://ega.tarul.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://jur.jinqigufen.top

[T11] Kotlin：协程
来源：http://nvb.jianghu66.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://xsn.hysaishi.cn

[T12] Kotlin：解构声明
来源：http://zsb.sjlbkw.cn

val (a, b) = Pair(1, 2)
来源：http://paa.shzxlz.cn

[T13] Kotlin：只读 Map
来源：http://keq.ybcxt.top

val m = mapOf("a" to 1)
来源：http://rkk.zycfv.cn

[T14] Kotlin：循环
来源：http://jjf.xuetiantiany.cn

for (i in 1..10) println(i)
来源：http://uif.ppjwa.cn

[T15] Kotlin：接口
来源：http://oud.redwolf501.top

interface Shape { fun area(): Double }
来源：http://zqq.nanxinkj.top

[T16] Swift：Hello World
来源：http://sbc.smart0.xyz

print("Hello")
来源：http://nmf.cheryme.top

[T17] Swift：变量与常量
来源：http://jbu.hammf.cn

var a = 1;  let b = 2
来源：http://jcv.zhiwuduotai.top

[T18] Swift：字符串插值
来源：http://uge.epnwcf.com

"值: \(b)"
来源：http://vuy.uphjek.com

[T19] Swift：可选绑定
来源：http://dbc.guowangkeji.top

if let n = opt { print(n) }
来源：http://uxf.tanke756.top

[T20] Swift：数组操作
来源：http://acw.fanxiaobao.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://hwd.daxiang520.top

[T21] Swift：遍历
来源：http://jkn.cheryme.top

for x in a { print(x) }
来源：http://dlk.jqgfzy.top

[T22] Swift：字典
来源：http://chl.tianlin.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://wag.xinyue.icu

[T23] Swift：函数
来源：http://ktq.yvedp.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rni.hfpthk.cn

[T24] Swift：闭包
来源：http://upg.bbcook.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qsu.cdnleiting.top

[T25] Swift：结构体
来源：http://vha.bjfxy.top

struct P { var x: Int }
来源：http://vjz.bbcook.cn

[T26] Swift：类与重写
来源：http://lwd.zhiwuduotai.top

class A: Base { override func f() {} }
来源：http://jyx.zhongyouzk.top

[T27] Swift：错误处理
来源：http://igw.pengpengdd.cyou

do { try f() } catch { print(error) }
来源：http://wkj.hcnkem.com

[T28] Swift：枚举
来源：http://xlw.shangyingyoupin.top

enum Color { case red, green }
来源：http://riu.jqgfzy.top

[T29] Swift：guard 提前返回
来源：http://zqk.snrcjt.cn

guard let x = opt else { return }
来源：http://qyt.sysykeji.top

[T30] Swift：协议
来源：http://ggu.dianchejie.cn

protocol Shape { func area() -> Double }
来源：http://qmd.nanxuanxn.top

[T31] Lua：Hello World
来源：http://ugu.meibo888.top

print("Hello")
来源：http://weo.meibo888.top

[T32] Lua：局部变量
来源：http://rst.ybcxt.top

local a = 1
来源：http://jdn.fanxiaobao.xyz

[T33] Lua：表（数组）
来源：http://aka.jinqigufen.top

local t = {1, 2, 3};  t[4] = 4
来源：http://jke.gotoacloud.top

[T34] Lua：遍历表
来源：http://lci.iojbl.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://eyw.smart0.xyz

[T35] Lua：字典表
来源：http://gri.9152youxi.cn

local d = { a = 1 };  d.b = 2
来源：http://brv.hammf.cn

[T36] Lua：函数
来源：http://jat.jqgufenzy.top

function add(a, b) return a + b end
来源：http://lzf.iojbl.cn

[T37] Lua：字符串拼接
来源：http://khc.fktsv.cn

"a" .. "b"
来源：http://apc.ppjwa.cn

[T38] Lua：条件
来源：http://ahb.vqdsnc.cn

if x > 0 then print("正") end
来源：http://age.havefunace.top

[T39] Lua：模式匹配
来源：http://egi.jyoumei.cn

string.find(s, "%d+")
来源：http://jmp.yuanzhike.top

[T40] Lua：元表
来源：http://ctc.shuidangran.top

setmetatable({}, { __index = base })
来源：http://zzf.hongshengwenyu.top

[T41] Perl：Hello World
来源：http://iho.jyoumei.cn

print "Hello\n";
来源：http://xmi.shuidangran.top

[T42] Perl：变量类型
来源：http://pzz.shzxlz.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://aqm.hywenlv.cn

[T43] Perl：字符串插值
来源：http://ulv.xylfe.cn

"值: $a"
来源：http://luq.vqdsnc.cn

[T44] Perl：条件
来源：http://hez.tarul.cn

if ($a > 0) { print "正"; }
来源：http://xxe.ppjwa.cn

[T45] Perl：数组遍历
来源：http://dgx.svipenyu.cn

for my $x (@arr) { print $x; }
来源：http://qoi.yangfankeji.com

[T46] Perl：哈希操作
来源：http://nua.yonumen.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wxl.svipenyu.cn

[T47] Perl：正则捕获
来源：http://nka.aibaodan.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://kay.yvedp.cn

[T48] Perl：正则替换
来源：http://hok.fanxiaobao.xyz

$s =~ s/old/new/g;
来源：http://pdn.daria6918.cn

[T49] Perl：函数
来源：http://irq.cashguo.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://avz.smart0.xyz

[T50] Perl：逐行读文件
来源：http://ukc.gotoacloud.top

open my $fh, "<", "a.txt" or die $!;
来源：http://ydw.zhongyouzk.top

while (my $line = <$fh>) { print $line; }
来源：http://gng.xuanzx.com

[T51] Scala：Hello World
来源：http://qps.yanxiufei.cn

println("Hello")
来源：http://otm.shzxlz.cn

[T52] Scala：变量
来源：http://spk.meibo888.top


<!-- 参考信息 -->