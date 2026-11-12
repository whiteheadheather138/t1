代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dms.jinqigufen.top

[R50] awk 求和
来源：http://zxh.yanxiufei.cn

awk '{s += $2} END {print s}' a.txt
来源：http://kyc.pengpengdd.cyou

[R51] 排序去重取前几
来源：http://vwc.zhoulong.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://dpj.ivvv.top

[R52] 统计行数
来源：http://fas.bjfxy.top

wc -l a.txt
来源：http://rad.sufxvd.cn

[R53] 查看文件头与实时尾
来源：http://tdq.0kj1m.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ppw.yanxiufei.cn

[R54] 比较两个文件
来源：http://rdg.havefunace.top

diff a.txt b.txt
来源：http://sid.xinyue.icu

[R55] 压缩与解压
来源：http://rif.feifeiyinyue.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uqf.zhongyouzk.top

[R56] 远程拷贝
来源：http://hln.fktsv.cn

scp file user@host:/path/
来源：http://rod.meibo888.top

[R57] 远程执行命令
来源：http://pge.fehbvm.com

ssh user@host 'uptime'
来源：http://hvj.zdbjq.cn

[R58] 下载文件
来源：http://zkp.sweek.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cww.yj202588.top

[R59] 发 POST JSON
来源：http://nez.ywan-chungtsiang.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lyt.ppjwa.cn

[R60] 只看 HTTP 状态码
来源：http://tad.ehwqpu.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lqs.zhoulong.xyz

[R61] 磁盘占用
来源：http://dul.dashuyun.cn

df -h;  du -sh *
来源：http://egl.shuidangran.top

[R62] 找最占空间的文件
来源：http://cxu.52xcode.cn

du -ah . | sort -rh | head -10
来源：http://ldd.fzhhl.top

[R63] 内存与进程
来源：http://sgy.xinyue.icu

free -h;  ps aux | grep nginx
来源：http://xcb.ybcxt.top

[R64] 结束进程
来源：http://fvf.ybcxt.top

kill -9 $(pgrep -f app.py)
来源：http://qey.yuanzhike.top

[R65] 查看端口占用
来源：http://fpi.jinqigufen.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hiy.sufxvd.cn

[R66] 定时任务
来源：http://aln.hfpthk.cn

crontab -e;  crontab -l
来源：http://xjc.vehdjk.com

[R67] 生成随机十六进制串
来源：http://wab.yongpay.top

openssl rand -hex 16
来源：http://dut.jinyuanbaomall.cn

[R68] 计算文件校验值
来源：http://xqj.chenlongwang.top

sha256sum a.txt;  md5sum a.txt
来源：http://gnb.gogol.net.cn

[R69] 生成随机密码
来源：http://bko.iojbl.cn

head -c 16 /dev/urandom | base64
来源：http://dvr.haohaochexian.top

[R70] 时间戳与互转
来源：http://psd.hesvh.cn

date +%s;  date -d @1700000000
来源：http://lso.wangdashe.top

[R71] 日期格式化
来源：http://kip.yj20258.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://upm.0kj1m.cn

[R72] 等待端口就绪
来源：http://xry.zhaomingkeji.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://sbd.iojbl.cn

[R73] 分割大日志
来源：http://vzn.tarul.cn

split -l 1000 big.log part_
来源：http://rwq.cucudq.cn

[R74] 批量重命名
来源：http://zxi.zhixingplan.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://iki.zdbjq.cn

[R75] 导出环境变量
来源：http://dbr.pengpengdd.cyou

export PATH="$HOME/bin:$PATH"
来源：http://osv.haohaochexian.top

[R76] 使用临时文件
来源：http://hcx.316326.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bix.ybcxt.top

[R77] 读取用户输入
来源：http://tiq.yueranfly.top

read -rp "请输入: " ans
来源：http://pgr.dashuyun.cn

[R78] 交互式菜单
来源：http://sva.zhongyouzk.top

select opt in a b c; do echo "$opt"; break; done
来源：http://jlw.yueranfly.top

[R79] 解析命令行选项
来源：http://cse.zhongyouzk.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xve.zycfv.cn

[R80] 查看脚本执行耗时
来源：http://dlr.hesvh.cn

time ./run.sh
来源：http://ovv.tianlin.xyz

================================================================================
来源：http://qia.hfpthk.cn

S. C / C++ 专题
来源：http://dyu.ppjwa.cn

================================================================================
来源：http://lri.guannengcc.top

[S01] C：Hello World
来源：http://ifc.nanxinkj.top

#include <stdio.h>
来源：http://gue.yfazqb.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://ifk.jyoumei.cn

[S02] C：变量与格式化输出
来源：http://ehl.hammf.cn

int a = 10; printf("%d\n", a);
来源：http://yxn.pengpengdd.cyou

[S03] C：读入整数
来源：http://pgy.snrcjt.cn

int x; scanf("%d", &x);
来源：http://xzz.nanxinkj.top

[S04] C：字符串复制
来源：http://zcs.chenlongwang.top

char dst[32]; strcpy(dst, "hi");
来源：http://ijd.yj20258888.top

[S05] C：字符串长度
来源：http://zkf.cucudq.cn

strlen(s)
来源：http://tci.c1oappe.top

[S06] C：字符串比较
来源：http://sba.52xcode.cn

strcmp(a, b) == 0
来源：http://duq.nwbrower.top

[S07] C：数组遍历求和
来源：http://axy.ppjwa.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://okg.sjlbkw.cn

[S08] C：动态内存分配与释放
来源：http://pmc.chenjidiqi.icu

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://iof.zhixingplan.top

[S09] C：结构体定义与初始化
来源：http://ajc.shzxlz.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zdj.vehdjk.com

[S10] C：指针与解引用
来源：http://qaw.dianchejie.cn

int *p = &a;  *p = 5;
来源：http://zyv.jinyuanbaomall.cn

[S11] C：逐行读文件
来源：http://qra.hnqzz.top

FILE *f = fopen("a.txt", "r");
来源：http://pne.jiagoushi.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ufw.yuxming.cn

fclose(f);
来源：http://clm.meibo888.top

[S12] C：写文件
来源：http://rim.jianghu66.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ifx.bjfxy.top

[S13] C：宏定义
来源：http://jgn.tanke756.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dbh.kuanghao11.cn

[S14] C：枚举
来源：http://ujo.0kj1m.cn

enum Color { RED, GREEN, BLUE };
来源：http://tag.jinghuilouyu.cn

[S15] C：类型转换
来源：http://hko.iojbl.cn

(double) a / b
来源：http://rgq.yvedp.cn

[S16] C：位操作置位
来源：http://nyf.xingfuxueyuan.xyz

x |= (1 << 3);
来源：http://qvx.yonumen.top

[S17] C：安全拼接字符串
来源：http://pmg.ydzc1.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://iny.kuanghao11.cn

[S18] C：命令行参数
来源：http://mnz.redwolf501.top

int main(int argc, char **argv)
来源：http://qdj.jqgufenzy.top

[S19] C：快速排序
来源：http://wrh.ivvv.top

qsort(a, n, sizeof(int), cmp);
来源：http://rjm.snrcjt.cn

[S20] C：二分查找
来源：http://nkh.cucudq.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hwg.smart0.xyz

[S21] C：字符类别判断
来源：http://eeh.cheryme.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://aqb.yj20258.top

[S22] C：字符串转数字
来源：http://qpj.quarkkingdee.top

atoi("42");  strtod("3.14", NULL);
来源：http://bsf.sysykeji.top

[S23] C：随机数
来源：http://rfk.zhengqikj.top

srand(time(NULL));  int r = rand() % 100;
来源：http://fwf.yanxiufei.cn

[S24] C：获取本地时间
来源：http://qjz.yueranfly.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bmd.andypj.xyz

[S25] C：内存拷贝
来源：http://sjj.c1oappe.top

memcpy(dst, src, n);
来源：http://zpe.nanxuanxn.top

[S26] C：内存清零
来源：http://jhl.fehbvm.com

memset(a, 0, sizeof a);
来源：http://wjo.yuanzhike.top

[S27] C：定义常量
来源：http://avh.xziqi.cn

const double PI = 3.14159;
来源：http://jwc.guannengcc.top

[S28] C：静态变量
来源：http://tfk.zhoulong.xyz

static int counter = 0;
来源：http://qbk.daxiang520.top

[S29] C：变参函数
来源：http://agm.shanyushiyangtech.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wme.zhongyouzk.top

[S30] C：头文件保护
来源：http://auw.ybcxt.top

#ifndef X_H
来源：http://wgg.yj20258.top

#define X_H
来源：http://rue.cqqwz.cn

#endif
来源：http://hcy.yanxiufei.cn

[S31] C++：Hello World
来源：http://uie.quarkkingdee.top

#include <iostream>
来源：http://aga.daxiang520.top

int main() { std::cout << "Hello\n"; }
来源：http://uao.jinyuanbaomall.cn

[S32] C++：字符串
来源：http://aka.dianchejie.cn

std::string s = "hi";  s += "!";
来源：http://mmk.tian-w.cn

[S33] C++：vector 增删
来源：http://uvr.chenzaomai.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://iuc.yj20258.top

[S34] C++：遍历 vector
来源：http://upq.pengpengdd.cyou

for (auto &x : v) { std::cout << x; }
来源：http://ffu.daxiang520.top

[S35] C++：map
来源：http://pqx.ctjpmb.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dca.jiagoushi.top

[S36] C++：unordered_map
来源：http://obr.jinqigfzy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dgs.hywenlv.cn

[S37] C++：set
来源：http://hdi.iojbl.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://byc.gotoacloud.top

[S38] C++：排序
来源：http://auq.zhaomingkeji.xyz

std::sort(v.begin(), v.end());
来源：http://kld.shanyushiyangkeji.top

[S39] C++：自定义比较器排序
来源：http://wik.52xcode.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://scx.cheryme.top

[S40] C++：查找元素
来源：http://wnb.yfazqb.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qkg.yj202588.top

[S41] C++：类与构造函数
来源：http://yto.jinqigufen.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ybl.nanxuanxn.top

[S42] C++：继承与虚函数
来源：http://xbx.jlsjyb.cn

class B : public Base { public: void f() override {} };
来源：http://dek.iojbl.cn

[S43] C++：智能指针
来源：http://ouu.yj202588.top

auto p = std::make_unique<int>(5);
来源：http://qkq.jiagoushi.top

[S44] C++：引用传参
来源：http://ijt.quarkkingdee.top

void inc(int &x) { ++x; }
来源：http://lff.hywenlv.cn

[S45] C++：lambda
来源：http://irx.52xcode.cn

auto add = [](int a, int b) { return a + b; };
来源：http://uht.smart0.xyz

[S46] C++：函数模板
来源：http://efs.sweek.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mwd.hammf.cn

[S47] C++：结构化绑定遍历
来源：http://rwt.xziqi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hwt.hfpthk.cn

[S48] C++：逐行读文件
来源：http://zdt.zycfv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://tjc.cqqwz.cn

while (std::getline(in, line)) { }
来源：http://nua.xuanzx.com

[S49] C++：写文件
来源：http://omp.pengpengdd.cyou

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wqa.guannengcc.top

[S50] C++：格式化数字
来源：http://ubz.sufxvd.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gfc.hcnkem.com

[S51] C++：显式类型转换
来源：http://gti.gotoacloud.top

static_cast<double>(a) / b
来源：http://wia.jinqigfzy.top

[S52] C++：const 与 noexcept
来源：http://ymp.xingfuxueyuan.xyz

int size() const noexcept { return n_; }
来源：http://olh.ivvv.top

[S53] C++：移动语义
来源：http://mqo.daxiang520.top

std::vector<int> w = std::move(v);
来源：http://myy.xylfe.cn

[S54] C++：异常处理
来源：http://zsw.ydzc1.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mck.zdbjq.cn

[S55] C++：结构化绑定
来源：http://dpu.kuanghao11.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xav.haohaochexian.top

[S56] C++：optional
来源：http://xbt.guannengcc.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uut.chenjidiqi.icu

[S57] C++：编译期常量
来源：http://bwh.xuanzx.com

constexpr int N = 10;
来源：http://wrc.xuetiantiany.cn

[S58] C++：命名空间
来源：http://qmd.guannengcc.top

namespace ns { int f() { return 1; } }
来源：http://qad.jiagoushi.top

[S59] C++：静态断言
来源：http://lal.pycfn.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://klh.fanxiaobao.xyz

[S60] C++：遍历并删除元素
来源：http://zqg.xuanzx.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kxh.xuetiantiany.cn

================================================================================
来源：http://zbo.xuetiantiany.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gbo.ywan-chungtsiang.top

================================================================================
来源：http://lgp.cucudq.cn

[T01] Kotlin：Hello World
来源：http://idr.yangfankeji.com

println("Hello")
来源：http://qyz.xylfe.cn

[T02] Kotlin：变量
来源：http://cuw.ctjpmb.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ibg.daria6918.cn

[T03] Kotlin：字符串模板
来源：http://tfp.tarul.cn

"值: $b"
来源：http://hpv.tianlin.xyz

[T04] Kotlin：空安全
来源：http://eoi.jianghu66.top

val n: String? = null;  n?.length
来源：http://sai.fehbvm.com

[T05] Kotlin：when 表达式
来源：http://iwi.gotoacloud.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zdd.tianlin.xyz

[T06] Kotlin：集合映射
来源：http://clr.epnwcf.com

listOf(1, 2, 3).map { it * 2 }
来源：http://muv.cdnleiting.top

[T07] Kotlin：集合过滤
来源：http://phm.feifeiyinyue.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://msc.yvedp.cn

[T08] Kotlin：数据类
来源：http://wrw.ybcxt.top

data class User(val name: String, val age: Int)
来源：http://tpt.hnqzz.top

[T09] Kotlin：扩展函数
来源：http://iav.zhengqikj.top

fun String.exclaim() = this + "!"
来源：http://snr.hnxiangtu.top

[T10] Kotlin：默认参数
来源：http://isi.yonumen.top

fun greet(name: String = "World") = "Hi $name"
来源：http://jwc.ydjk.org.cn

[T11] Kotlin：协程
来源：http://ecq.smart0.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://yie.zhongyouzk.top

[T12] Kotlin：解构声明
来源：http://ooy.ctjpmb.com

val (a, b) = Pair(1, 2)
来源：http://hnz.zhijiandao.cn

[T13] Kotlin：只读 Map
来源：http://sqq.nwbrower.top

val m = mapOf("a" to 1)
来源：http://wiu.316326.xyz

[T14] Kotlin：循环
来源：http://uhc.jiagoushi.top

for (i in 1..10) println(i)
来源：http://ziy.tianlin.xyz

[T15] Kotlin：接口
来源：http://ptd.jinghuilouyu.cn

interface Shape { fun area(): Double }
来源：http://sao.daria6918.cn

[T16] Swift：Hello World
来源：http://ncs.vehdjk.com

print("Hello")
来源：http://vql.hywenlv.cn

[T17] Swift：变量与常量
来源：http://zuy.ppjwa.cn

var a = 1;  let b = 2
来源：http://rbz.jlsjyb.cn

[T18] Swift：字符串插值
来源：http://tkm.fengsongda.top

"值: \(b)"
来源：http://gui.cdnleiting.top

[T19] Swift：可选绑定
来源：http://rzt.hnqzz.top

if let n = opt { print(n) }
来源：http://kxd.jinqigfzy.top

[T20] Swift：数组操作
来源：http://pdx.sweek.top

var a = [1, 2, 3];  a.append(4)
来源：http://fjn.svipenyu.cn

[T21] Swift：遍历
来源：http://sws.zhiwuduotai.top

for x in a { print(x) }
来源：http://vfw.yuxming.cn

[T22] Swift：字典
来源：http://jvk.yj20258888.top

var d = ["a": 1];  d["b"] = 2
来源：http://knm.andypj.xyz

[T23] Swift：函数
来源：http://xnt.vehdjk.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gwb.chenzaomai.com

[T24] Swift：闭包
来源：http://umu.zhoulong.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://rfb.sysykeji.top

[T25] Swift：结构体
来源：http://wvm.ydzc1.top

struct P { var x: Int }
来源：http://ngi.yonumen.top

[T26] Swift：类与重写
来源：http://aag.shzxlz.cn

class A: Base { override func f() {} }
来源：http://vru.jianghu66.top

[T27] Swift：错误处理
来源：http://bwc.jinqigfzy.top

do { try f() } catch { print(error) }
来源：http://ktz.cashguo.top

[T28] Swift：枚举
来源：http://ehg.yongpay.top

enum Color { case red, green }
来源：http://czj.hysaishi.cn

[T29] Swift：guard 提前返回
来源：http://fva.cdnleiting.top

guard let x = opt else { return }
来源：http://alb.fehbvm.com

[T30] Swift：协议
来源：http://fdn.gotoacloud.top

protocol Shape { func area() -> Double }
来源：http://lks.hywenlv.cn

[T31] Lua：Hello World
来源：http://hif.zhaomingkeji.xyz

print("Hello")
来源：http://wnt.cucudq.cn

[T32] Lua：局部变量
来源：http://ags.fktsv.cn

local a = 1
来源：http://dmk.chenlongwang.top

[T33] Lua：表（数组）
来源：http://vun.jlsjyb.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://itz.chenlongwang.top

[T34] Lua：遍历表
来源：http://cau.gotoacloud.top

for i, v in ipairs(t) do print(i, v) end
来源：http://iyg.zhixingplan.top

[T35] Lua：字典表
来源：http://sem.aizwys.cn

local d = { a = 1 };  d.b = 2
来源：http://nll.fanxiaobao.xyz

[T36] Lua：函数
来源：http://mod.zhongyouzk.top

function add(a, b) return a + b end
来源：http://myp.hfpthk.cn

[T37] Lua：字符串拼接
来源：http://vnn.meibo888.top

"a" .. "b"
来源：http://rii.ivvv.top

[T38] Lua：条件
来源：http://vcw.yfazqb.com

if x > 0 then print("正") end
来源：http://ybl.fehbvm.com

[T39] Lua：模式匹配
来源：http://dmm.sweek.top

string.find(s, "%d+")
来源：http://rgu.tianlin.xyz

[T40] Lua：元表
来源：http://bxo.shzxlz.cn

setmetatable({}, { __index = base })
来源：http://sfz.fengsongda.top

[T41] Perl：Hello World
来源：http://bie.redwolf501.top

print "Hello\n";
来源：http://gqa.aibaodan.cn

[T42] Perl：变量类型
来源：http://xav.xinyue.icu

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ale.hcnkem.com

[T43] Perl：字符串插值
来源：http://kpy.sjlbkw.cn

"值: $a"
来源：http://fng.svipenyu.cn

[T44] Perl：条件
来源：http://wod.zhijiandao.cn

if ($a > 0) { print "正"; }
来源：http://ymn.kuanghao11.cn

[T45] Perl：数组遍历
来源：http://mlf.feifeiyinyue.top

for my $x (@arr) { print $x; }
来源：http://gjk.c1oappe.top

[T46] Perl：哈希操作
来源：http://zdw.wangshuangyany.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qrw.guannengcc.top

[T47] Perl：正则捕获
来源：http://xcm.gogol.net.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://vvo.zdbjq.cn

[T48] Perl：正则替换
来源：http://eaa.chenlongwang.top

$s =~ s/old/new/g;
来源：http://mqj.yonumen.top

[T49] Perl：函数
来源：http://hsi.sjlbkw.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qsx.vehdjk.com

[T50] Perl：逐行读文件
来源：http://enm.52xcode.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://bsy.uphjek.com

while (my $line = <$fh>) { print $line; }
来源：http://rjd.jqgufenzy.top

[T51] Scala：Hello World
来源：http://dfw.chenjidiqi.icu

println("Hello")
来源：http://nct.jiagoushi.top

[T52] Scala：变量
来源：http://btc.birdmap.top


<!-- 参考信息 -->