代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ypw.snrcjt.cn

[R50] awk 求和
来源：http://zmp.pycfn.com

awk '{s += $2} END {print s}' a.txt
来源：http://gfz.snrcjt.cn

[R51] 排序去重取前几
来源：http://uyi.kuanghao11.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://nne.jiagoushi.top

[R52] 统计行数
来源：http://mkf.ybcxt.top

wc -l a.txt
来源：http://eyo.c1oappe.top

[R53] 查看文件头与实时尾
来源：http://lfl.hnqzz.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kbq.gzhubu.top

[R54] 比较两个文件
来源：http://yal.cdnleiting.top

diff a.txt b.txt
来源：http://gac.zhaomingkeji.xyz

[R55] 压缩与解压
来源：http://gxg.hesvh.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mnf.tarul.cn

[R56] 远程拷贝
来源：http://fhy.hysaishi.cn

scp file user@host:/path/
来源：http://hog.zdqjudy.top

[R57] 远程执行命令
来源：http://gem.pengpengdd.cyou

ssh user@host 'uptime'
来源：http://sqr.haohaochexian.top

[R58] 下载文件
来源：http://umz.yongpay.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uxt.chenlongwang.top

[R59] 发 POST JSON
来源：http://wya.yueranfly.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://koc.birdmap.top

[R60] 只看 HTTP 状态码
来源：http://uvv.yj202588.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vjv.bbcook.cn

[R61] 磁盘占用
来源：http://nue.xuetiantiany.cn

df -h;  du -sh *
来源：http://wlv.tianlin.xyz

[R62] 找最占空间的文件
来源：http://qsd.cashguo.top

du -ah . | sort -rh | head -10
来源：http://uau.yj20258888.top

[R63] 内存与进程
来源：http://cjj.yanxiufei.cn

free -h;  ps aux | grep nginx
来源：http://isj.daxiang520.top

[R64] 结束进程
来源：http://zad.jinqigfzy.top

kill -9 $(pgrep -f app.py)
来源：http://sws.shanyushiyangtech.top

[R65] 查看端口占用
来源：http://xxb.jyoumei.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cqc.jlsjyb.cn

[R66] 定时任务
来源：http://rpe.bbcook.cn

crontab -e;  crontab -l
来源：http://wqn.bbcook.cn

[R67] 生成随机十六进制串
来源：http://jxd.c1oappe.top

openssl rand -hex 16
来源：http://pyg.hammf.cn

[R68] 计算文件校验值
来源：http://cpf.yj20258888.top

sha256sum a.txt;  md5sum a.txt
来源：http://ryx.tarul.cn

[R69] 生成随机密码
来源：http://dvw.52xcode.cn

head -c 16 /dev/urandom | base64
来源：http://rba.ivvv.top

[R70] 时间戳与互转
来源：http://rsz.fehbvm.com

date +%s;  date -d @1700000000
来源：http://whr.chenjidiqi.icu

[R71] 日期格式化
来源：http://ufk.aibaodan.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zot.zhoulong.xyz

[R72] 等待端口就绪
来源：http://ygj.cdnleiting.top

until nc -z localhost 3306; do sleep 1; done
来源：http://giv.shzxlz.cn

[R73] 分割大日志
来源：http://rsj.dianchejie.cn

split -l 1000 big.log part_
来源：http://hhn.shangyingyoupin.top

[R74] 批量重命名
来源：http://elk.jinqigufen.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://err.zhijiandao.cn

[R75] 导出环境变量
来源：http://jyz.zhijiandao.cn

export PATH="$HOME/bin:$PATH"
来源：http://kaf.daria6918.cn

[R76] 使用临时文件
来源：http://qxe.fanxiaobao.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://exi.sufxvd.cn

[R77] 读取用户输入
来源：http://qci.hfpthk.cn

read -rp "请输入: " ans
来源：http://usz.gzhubu.top

[R78] 交互式菜单
来源：http://zyr.hesvh.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ljl.fengsongda.top

[R79] 解析命令行选项
来源：http://jtv.ppjwa.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://exd.redwolf501.top

[R80] 查看脚本执行耗时
来源：http://uzc.xylfe.cn

time ./run.sh
来源：http://xon.hnxiangtu.top

================================================================================
来源：http://cdx.zdbjq.cn

S. C / C++ 专题
来源：http://ldc.cashguo.top

================================================================================
来源：http://bvm.yanxiufei.cn

[S01] C：Hello World
来源：http://xmg.nanxuanxn.top

#include <stdio.h>
来源：http://tyj.hesvh.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://sxk.tianlin.xyz

[S02] C：变量与格式化输出
来源：http://qjx.yonumen.top

int a = 10; printf("%d\n", a);
来源：http://iri.redwolf501.top

[S03] C：读入整数
来源：http://lab.jianghu66.top

int x; scanf("%d", &x);
来源：http://gzy.fktsv.cn

[S04] C：字符串复制
来源：http://wia.c1oappe.top

char dst[32]; strcpy(dst, "hi");
来源：http://txq.yonumen.top

[S05] C：字符串长度
来源：http://zln.feifeiyinyue.top

strlen(s)
来源：http://pso.hfpthk.cn

[S06] C：字符串比较
来源：http://tyv.zhoulong.xyz

strcmp(a, b) == 0
来源：http://ssg.ivvv.top

[S07] C：数组遍历求和
来源：http://upk.pycfn.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jzb.zhoulong.xyz

[S08] C：动态内存分配与释放
来源：http://evf.ppjwa.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nda.cqqwz.cn

[S09] C：结构体定义与初始化
来源：http://aou.jlsjyb.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://edv.xingfuxueyuan.xyz

[S10] C：指针与解引用
来源：http://zbf.gaohongyu789.top

int *p = &a;  *p = 5;
来源：http://cmz.9152youxi.cn

[S11] C：逐行读文件
来源：http://adw.nanxinkj.top

FILE *f = fopen("a.txt", "r");
来源：http://keg.cdnleiting.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://wwz.hongshengwenyu.top

fclose(f);
来源：http://emn.jiagoushi.top

[S12] C：写文件
来源：http://kwz.nanxuanxn.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jbz.shanyushiyangtech.top

[S13] C：宏定义
来源：http://ren.shzxlz.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kij.jyoumei.cn

[S14] C：枚举
来源：http://dqc.xuetiantiany.cn

enum Color { RED, GREEN, BLUE };
来源：http://wcd.ybcxt.top

[S15] C：类型转换
来源：http://itc.wangshuangyany.cn

(double) a / b
来源：http://vhz.hammf.cn

[S16] C：位操作置位
来源：http://xmf.haohaochexian.top

x |= (1 << 3);
来源：http://qnk.shanyushiyangkeji.top

[S17] C：安全拼接字符串
来源：http://ipt.yj20258888.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zmo.dashuyun.cn

[S18] C：命令行参数
来源：http://ukh.hesvh.cn

int main(int argc, char **argv)
来源：http://cqz.pengpengdd.cyou

[S19] C：快速排序
来源：http://ukg.jlsjyb.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qso.redwolf501.top

[S20] C：二分查找
来源：http://wbn.vqdsnc.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://maa.hcnkem.com

[S21] C：字符类别判断
来源：http://mov.zhongyouzk.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nhn.jiagoushi.top

[S22] C：字符串转数字
来源：http://bjk.cdnleiting.top

atoi("42");  strtod("3.14", NULL);
来源：http://rot.uphjek.com

[S23] C：随机数
来源：http://tav.xylfe.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ngh.xuetiantiany.cn

[S24] C：获取本地时间
来源：http://vwe.9152youxi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rdj.jqgufenzy.top

[S25] C：内存拷贝
来源：http://lgv.shzxlz.cn

memcpy(dst, src, n);
来源：http://jdo.aibaodan.cn

[S26] C：内存清零
来源：http://gdm.shangyingyoupin.top

memset(a, 0, sizeof a);
来源：http://yql.gotoacloud.top

[S27] C：定义常量
来源：http://jmm.0kj1m.cn

const double PI = 3.14159;
来源：http://qyu.zhaomingkeji.xyz

[S28] C：静态变量
来源：http://ovx.hesvh.cn

static int counter = 0;
来源：http://nnt.cdnleiting.top

[S29] C：变参函数
来源：http://nov.sweek.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dzm.hywenlv.cn

[S30] C：头文件保护
来源：http://dgb.tarul.cn

#ifndef X_H
来源：http://xgm.nanxinkj.top

#define X_H
来源：http://smo.sysykeji.top

#endif
来源：http://zka.ybcxt.top

[S31] C++：Hello World
来源：http://jua.sjlbkw.cn

#include <iostream>
来源：http://qvd.tanke756.top

int main() { std::cout << "Hello\n"; }
来源：http://efy.guowangkeji.top

[S32] C++：字符串
来源：http://zah.gogol.net.cn

std::string s = "hi";  s += "!";
来源：http://byd.epnwcf.com

[S33] C++：vector 增删
来源：http://mid.nanxuanxn.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hsw.andypj.xyz

[S34] C++：遍历 vector
来源：http://ejr.hcnkem.com

for (auto &x : v) { std::cout << x; }
来源：http://ibt.ctjpmb.com

[S35] C++：map
来源：http://tjl.zhiwuduotai.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tqd.52xcode.cn

[S36] C++：unordered_map
来源：http://gok.jinghuilouyu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dli.tanke756.top

[S37] C++：set
来源：http://bvx.bjfxy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wmg.dashuyun.cn

[S38] C++：排序
来源：http://fsn.smart0.xyz

std::sort(v.begin(), v.end());
来源：http://hck.daxiang520.top

[S39] C++：自定义比较器排序
来源：http://iim.sxryk.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zqj.shuidangran.top

[S40] C++：查找元素
来源：http://obc.hywenlv.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ieq.yvedp.cn

[S41] C++：类与构造函数
来源：http://dky.zhixingplan.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://djd.guowangkeji.top

[S42] C++：继承与虚函数
来源：http://uqs.shuidangran.top

class B : public Base { public: void f() override {} };
来源：http://hai.daria6918.cn

[S43] C++：智能指针
来源：http://ens.nwbrower.top

auto p = std::make_unique<int>(5);
来源：http://zao.gzhubu.top

[S44] C++：引用传参
来源：http://pqr.aibaodan.cn

void inc(int &x) { ++x; }
来源：http://yxu.guowangkeji.top

[S45] C++：lambda
来源：http://nsq.redwolf501.top

auto add = [](int a, int b) { return a + b; };
来源：http://ure.hnxiangtu.top

[S46] C++：函数模板
来源：http://kyo.nanxinkj.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://msr.xziqi.cn

[S47] C++：结构化绑定遍历
来源：http://pwz.jyoumei.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pwn.iojbl.cn

[S48] C++：逐行读文件
来源：http://zsr.havefunace.top

std::ifstream in("a.txt");  std::string line;
来源：http://xpi.snrcjt.cn

while (std::getline(in, line)) { }
来源：http://fqr.zdqjudy.top

[S49] C++：写文件
来源：http://kzr.feifeiyinyue.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tmc.nwbrower.top

[S50] C++：格式化数字
来源：http://bjn.yongpay.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wlx.xuanzx.com

[S51] C++：显式类型转换
来源：http://xxj.zdbjq.cn

static_cast<double>(a) / b
来源：http://pgc.jlsjyb.cn

[S52] C++：const 与 noexcept
来源：http://mfc.ybcxt.top

int size() const noexcept { return n_; }
来源：http://son.9152youxi.cn

[S53] C++：移动语义
来源：http://hbm.hnqzz.top

std::vector<int> w = std::move(v);
来源：http://mcy.fanxiaobao.xyz

[S54] C++：异常处理
来源：http://yhd.yuxming.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fqo.nanxinkj.top

[S55] C++：结构化绑定
来源：http://pih.zhengqikj.top

auto [a, b] = std::make_pair(1, 2);
来源：http://twx.meibo888.top

[S56] C++：optional
来源：http://itx.yj20258888.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zjn.jinghuilouyu.cn

[S57] C++：编译期常量
来源：http://mfq.daria6918.cn

constexpr int N = 10;
来源：http://pwn.yangfankeji.com

[S58] C++：命名空间
来源：http://eki.ehwqpu.com

namespace ns { int f() { return 1; } }
来源：http://zfd.jlsjyb.cn

[S59] C++：静态断言
来源：http://cor.ppjwa.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rld.fehbvm.com

[S60] C++：遍历并删除元素
来源：http://jvv.c1oappe.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yom.zhiwuduotai.top

================================================================================
来源：http://shs.guowangkeji.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ixm.jinqigfzy.top

================================================================================
来源：http://pth.yueranfly.top

[T01] Kotlin：Hello World
来源：http://ini.gogol.net.cn

println("Hello")
来源：http://ojg.fengsongda.top

[T02] Kotlin：变量
来源：http://mhf.zhixingplan.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hrg.cqqwz.cn

[T03] Kotlin：字符串模板
来源：http://xnk.ehwqpu.com

"值: $b"
来源：http://kxa.ctjpmb.com

[T04] Kotlin：空安全
来源：http://ekp.jinyuanbaomall.cn

val n: String? = null;  n?.length
来源：http://abf.fengsongda.top

[T05] Kotlin：when 表达式
来源：http://jck.guannengcc.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pdf.sjlbkw.cn

[T06] Kotlin：集合映射
来源：http://lmq.hongshengwenyu.top

listOf(1, 2, 3).map { it * 2 }
来源：http://rim.zhoulong.xyz

[T07] Kotlin：集合过滤
来源：http://fzw.xinyue.icu

listOf(1, 2, 3).filter { it > 1 }
来源：http://ejl.shanyushiyangkeji.top

[T08] Kotlin：数据类
来源：http://vkl.chenlongwang.top

data class User(val name: String, val age: Int)
来源：http://jgv.fehbvm.com

[T09] Kotlin：扩展函数
来源：http://dhf.uphjek.com

fun String.exclaim() = this + "!"
来源：http://fvx.guowangkeji.top

[T10] Kotlin：默认参数
来源：http://baf.ctjpmb.com

fun greet(name: String = "World") = "Hi $name"
来源：http://wxi.ivvv.top

[T11] Kotlin：协程
来源：http://qpp.yueranfly.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://tts.bjfxy.top

[T12] Kotlin：解构声明
来源：http://qva.zdqjudy.top

val (a, b) = Pair(1, 2)
来源：http://aod.zhengqikj.top

[T13] Kotlin：只读 Map
来源：http://ack.yvedp.cn

val m = mapOf("a" to 1)
来源：http://xbs.haohaochexian.top

[T14] Kotlin：循环
来源：http://zqo.shanyushiyangkeji.top

for (i in 1..10) println(i)
来源：http://sfu.redwolf501.top

[T15] Kotlin：接口
来源：http://eei.kuanghao11.cn

interface Shape { fun area(): Double }
来源：http://dwl.sweek.top

[T16] Swift：Hello World
来源：http://you.hcnkem.com

print("Hello")
来源：http://vgo.chenjidiqi.icu

[T17] Swift：变量与常量
来源：http://smb.redwolf501.top

var a = 1;  let b = 2
来源：http://unf.jinyuanbaomall.cn

[T18] Swift：字符串插值
来源：http://gxp.0kj1m.cn

"值: \(b)"
来源：http://ldf.fktsv.cn

[T19] Swift：可选绑定
来源：http://dqu.meibo888.top

if let n = opt { print(n) }
来源：http://yow.ydzc1.top

[T20] Swift：数组操作
来源：http://ztu.xuanzx.com

var a = [1, 2, 3];  a.append(4)
来源：http://qlt.xuetiantiany.cn

[T21] Swift：遍历
来源：http://fyk.tianlin.xyz

for x in a { print(x) }
来源：http://njl.hcnkem.com

[T22] Swift：字典
来源：http://wnd.fzhhl.top

var d = ["a": 1];  d["b"] = 2
来源：http://xip.shanyushiyangtech.top

[T23] Swift：函数
来源：http://gtz.meibo888.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kgf.yj202588.top

[T24] Swift：闭包
来源：http://xzh.svipenyu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://sro.ydzc1.top

[T25] Swift：结构体
来源：http://dqg.fehbvm.com

struct P { var x: Int }
来源：http://goa.pycfn.com

[T26] Swift：类与重写
来源：http://twu.jinyuanbaomall.cn

class A: Base { override func f() {} }
来源：http://vtx.ydjk.org.cn

[T27] Swift：错误处理
来源：http://pbr.zhongyouzk.top

do { try f() } catch { print(error) }
来源：http://tfz.feifeiyinyue.top

[T28] Swift：枚举
来源：http://toi.xziqi.cn

enum Color { case red, green }
来源：http://fby.shzxlz.cn

[T29] Swift：guard 提前返回
来源：http://fny.havefunace.top

guard let x = opt else { return }
来源：http://bpn.dianchejie.cn

[T30] Swift：协议
来源：http://yvp.ctjpmb.com

protocol Shape { func area() -> Double }
来源：http://exr.jyoumei.cn

[T31] Lua：Hello World
来源：http://fus.0kj1m.cn

print("Hello")
来源：http://kty.ydzc1.top

[T32] Lua：局部变量
来源：http://vnq.jiagoushi.top

local a = 1
来源：http://saa.xuetiantiany.cn

[T33] Lua：表（数组）
来源：http://frx.andypj.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://dnb.bbcook.cn

[T34] Lua：遍历表
来源：http://neu.c1oappe.top

for i, v in ipairs(t) do print(i, v) end
来源：http://plb.nwbrower.top

[T35] Lua：字典表
来源：http://qxn.nanxinkj.top

local d = { a = 1 };  d.b = 2
来源：http://ngx.cashguo.top

[T36] Lua：函数
来源：http://tkv.hfpthk.cn

function add(a, b) return a + b end
来源：http://vog.ydjk.org.cn

[T37] Lua：字符串拼接
来源：http://thc.yj20258.top

"a" .. "b"
来源：http://zbw.yanxiufei.cn

[T38] Lua：条件
来源：http://jcj.mhx1999.top

if x > 0 then print("正") end
来源：http://jkm.cheryme.top

[T39] Lua：模式匹配
来源：http://dzc.ybcxt.top

string.find(s, "%d+")
来源：http://mdm.yongpay.top

[T40] Lua：元表
来源：http://qgj.bjfxy.top

setmetatable({}, { __index = base })
来源：http://lyr.yueranfly.top

[T41] Perl：Hello World
来源：http://neb.yj20258888.top

print "Hello\n";
来源：http://mln.daxiang520.top

[T42] Perl：变量类型
来源：http://lwc.fengsongda.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://xzn.hnqzz.top

[T43] Perl：字符串插值
来源：http://cao.pengpengdd.cyou

"值: $a"
来源：http://hfs.xziqi.cn

[T44] Perl：条件
来源：http://tyz.daxiang520.top

if ($a > 0) { print "正"; }
来源：http://ihb.jianghu66.top

[T45] Perl：数组遍历
来源：http://fgj.smart0.xyz

for my $x (@arr) { print $x; }
来源：http://ykf.jqgufenzy.top

[T46] Perl：哈希操作
来源：http://yiu.dianchejie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pgm.wangshuangyany.cn

[T47] Perl：正则捕获
来源：http://jce.gogol.net.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://yyy.chenzaomai.com

[T48] Perl：正则替换
来源：http://ocu.52xcode.cn

$s =~ s/old/new/g;
来源：http://ded.aibaodan.cn

[T49] Perl：函数
来源：http://wxz.yj202588.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hqs.sysykeji.top

[T50] Perl：逐行读文件
来源：http://pvx.yj20258.top

open my $fh, "<", "a.txt" or die $!;
来源：http://son.smart0.xyz

while (my $line = <$fh>) { print $line; }
来源：http://mmm.nwbrower.top

[T51] Scala：Hello World
来源：http://leg.jinqigfzy.top

println("Hello")
来源：http://mkr.guowangkeji.top

[T52] Scala：变量
来源：http://scm.bbcook.cn


<!-- 参考信息 -->