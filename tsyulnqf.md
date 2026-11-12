代发 wailian999

cmd > out.log 2>&1
来源：http://jkv.jianghu66.top

[R40] 追加写日志
来源：http://cgn.wangdashe.top

echo "log" >> out.log
来源：http://brx.fzhhl.top

[R41] 丢弃输出
来源：http://yib.epnwcf.com

cmd >/dev/null 2>&1
来源：http://ldo.jinyuanbaomall.cn

[R42] 输入重定向
来源：http://fcx.svipenyu.cn

wc -l < a.txt
来源：http://xux.gogol.net.cn

[R43] 按名字查找文件
来源：http://jge.ydzc1.top

find . -name "*.log" -type f
来源：http://qpf.ydzc1.top

[R44] 按修改时间查找
来源：http://fud.hywenlv.cn

find . -mtime -7 -type f
来源：http://epg.chenjidiqi.icu

[R45] 批量删除
来源：http://glz.yuanzhike.top

find . -name "*.tmp" -delete
来源：http://gwn.sysykeji.top

[R46] 递归替换文件内容
来源：http://lvm.hywenlv.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mdu.iojbl.cn

[R47] sed 单行替换
来源：http://oab.0kj1m.cn

sed -i 's/foo/bar/g' a.txt
来源：http://rqs.sysykeji.top

[R48] awk 取指定列
来源：http://zsp.chenjidiqi.icu

awk '{print $1, $3}' a.txt
来源：http://jlb.nwbrower.top

[R49] awk 带条件
来源：http://wfj.cdnleiting.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tvi.zycfv.cn

[R50] awk 求和
来源：http://kxd.shanyushiyangtech.top

awk '{s += $2} END {print s}' a.txt
来源：http://dfv.yj20258.top

[R51] 排序去重取前几
来源：http://mir.cdnleiting.top

sort a.txt | uniq -c | sort -rn | head
来源：http://lpg.xinyue.icu

[R52] 统计行数
来源：http://daj.0kj1m.cn

wc -l a.txt
来源：http://ahy.yuxming.cn

[R53] 查看文件头与实时尾
来源：http://ncd.jqgufenzy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nmp.cucudq.cn

[R54] 比较两个文件
来源：http://cul.kuanghao11.cn

diff a.txt b.txt
来源：http://vwb.ywan-chungtsiang.top

[R55] 压缩与解压
来源：http://nrq.yuanzhike.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mtm.wangshuangyany.cn

[R56] 远程拷贝
来源：http://tks.cashguo.top

scp file user@host:/path/
来源：http://iog.hywenlv.cn

[R57] 远程执行命令
来源：http://xqh.epnwcf.com

ssh user@host 'uptime'
来源：http://oan.fanxiaobao.xyz

[R58] 下载文件
来源：http://jvs.zhongyouzk.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://een.gzhubu.top

[R59] 发 POST JSON
来源：http://mev.fktsv.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://heu.jinqigfzy.top

[R60] 只看 HTTP 状态码
来源：http://ilt.pycfn.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vti.xinyue.icu

[R61] 磁盘占用
来源：http://cyh.jiagoushi.top

df -h;  du -sh *
来源：http://ebm.xylfe.cn

[R62] 找最占空间的文件
来源：http://wjf.gzhubu.top

du -ah . | sort -rh | head -10
来源：http://rta.ydzc1.top

[R63] 内存与进程
来源：http://cdf.wangdashe.top

free -h;  ps aux | grep nginx
来源：http://cbg.tian-w.cn

[R64] 结束进程
来源：http://piw.yanxiufei.cn

kill -9 $(pgrep -f app.py)
来源：http://vis.ppjwa.cn

[R65] 查看端口占用
来源：http://pey.yuanzhike.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kxv.cqqwz.cn

[R66] 定时任务
来源：http://hth.gaohongyu789.top

crontab -e;  crontab -l
来源：http://phi.tanke756.top

[R67] 生成随机十六进制串
来源：http://jsh.guowangkeji.top

openssl rand -hex 16
来源：http://zbm.zhijiandao.cn

[R68] 计算文件校验值
来源：http://hgf.aibaodan.cn

sha256sum a.txt;  md5sum a.txt
来源：http://cji.quarkkingdee.top

[R69] 生成随机密码
来源：http://uwd.hammf.cn

head -c 16 /dev/urandom | base64
来源：http://dij.jlsjyb.cn

[R70] 时间戳与互转
来源：http://mtx.fzhhl.top

date +%s;  date -d @1700000000
来源：http://yao.cdnleiting.top

[R71] 日期格式化
来源：http://lno.zhiwuduotai.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ukq.shzxlz.cn

[R72] 等待端口就绪
来源：http://rga.9152youxi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://yyb.jinqigufen.top

[R73] 分割大日志
来源：http://dfk.quarkkingdee.top

split -l 1000 big.log part_
来源：http://nhy.jianghu66.top

[R74] 批量重命名
来源：http://wgm.cheryme.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wnc.xuetiantiany.cn

[R75] 导出环境变量
来源：http://kjw.jlsjyb.cn

export PATH="$HOME/bin:$PATH"
来源：http://kvx.tianlin.xyz

[R76] 使用临时文件
来源：http://jtv.tian-w.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wxf.aizwys.cn

[R77] 读取用户输入
来源：http://qok.chenzaomai.com

read -rp "请输入: " ans
来源：http://qrc.ctjpmb.com

[R78] 交互式菜单
来源：http://bhz.ehwqpu.com

select opt in a b c; do echo "$opt"; break; done
来源：http://khg.yj20258.top

[R79] 解析命令行选项
来源：http://zst.yuxming.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dzu.ydzc1.top

[R80] 查看脚本执行耗时
来源：http://adj.birdmap.top

time ./run.sh
来源：http://esf.yueranfly.top

================================================================================
来源：http://xot.svipenyu.cn

S. C / C++ 专题
来源：http://nqz.uphjek.com

================================================================================
来源：http://zvw.andypj.xyz

[S01] C：Hello World
来源：http://rdh.fzhhl.top

#include <stdio.h>
来源：http://ixk.zycfv.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hod.jqgfzy.top

[S02] C：变量与格式化输出
来源：http://yre.ydjk.org.cn

int a = 10; printf("%d\n", a);
来源：http://pdb.sweek.top

[S03] C：读入整数
来源：http://ssf.dashuyun.cn

int x; scanf("%d", &x);
来源：http://run.hnqzz.top

[S04] C：字符串复制
来源：http://xlg.jinqigufen.top

char dst[32]; strcpy(dst, "hi");
来源：http://hzm.zhaomingkeji.xyz

[S05] C：字符串长度
来源：http://hwl.nanxinkj.top

strlen(s)
来源：http://pdd.guannengcc.top

[S06] C：字符串比较
来源：http://wun.sxryk.cn

strcmp(a, b) == 0
来源：http://vzs.zdbjq.cn

[S07] C：数组遍历求和
来源：http://bri.jqgufenzy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://owt.sysykeji.top

[S08] C：动态内存分配与释放
来源：http://ydv.yanxiufei.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pec.jqgufenzy.top

[S09] C：结构体定义与初始化
来源：http://vzf.ydjk.org.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ikj.guannengcc.top

[S10] C：指针与解引用
来源：http://iuk.iojbl.cn

int *p = &a;  *p = 5;
来源：http://hex.fzhhl.top

[S11] C：逐行读文件
来源：http://jfx.aizwys.cn

FILE *f = fopen("a.txt", "r");
来源：http://str.yuanzhike.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ntu.tarul.cn

fclose(f);
来源：http://hrg.ehwqpu.com

[S12] C：写文件
来源：http://dgy.ivvv.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kwb.zhijiandao.cn

[S13] C：宏定义
来源：http://sld.pycfn.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kmm.316326.xyz

[S14] C：枚举
来源：http://chf.9152youxi.cn

enum Color { RED, GREEN, BLUE };
来源：http://sbj.zhoulong.xyz

[S15] C：类型转换
来源：http://mro.dianchejie.cn

(double) a / b
来源：http://los.xingfuxueyuan.xyz

[S16] C：位操作置位
来源：http://dan.iojbl.cn

x |= (1 << 3);
来源：http://ksa.yangfankeji.com

[S17] C：安全拼接字符串
来源：http://sen.fzhhl.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zns.zhengqikj.top

[S18] C：命令行参数
来源：http://nxe.hesvh.cn

int main(int argc, char **argv)
来源：http://rtp.shanyushiyangkeji.top

[S19] C：快速排序
来源：http://hwo.yongpay.top

qsort(a, n, sizeof(int), cmp);
来源：http://kds.chenzaomai.com

[S20] C：二分查找
来源：http://qmg.hywenlv.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://otj.zhoulong.xyz

[S21] C：字符类别判断
来源：http://toi.jinghuilouyu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ofj.tianlin.xyz

[S22] C：字符串转数字
来源：http://ogq.tian-w.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qco.dashuyun.cn

[S23] C：随机数
来源：http://eiv.epnwcf.com

srand(time(NULL));  int r = rand() % 100;
来源：http://ewi.jianghu66.top

[S24] C：获取本地时间
来源：http://bbd.zdqjudy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://unn.zdqjudy.top

[S25] C：内存拷贝
来源：http://mwi.hywenlv.cn

memcpy(dst, src, n);
来源：http://osk.gzhubu.top

[S26] C：内存清零
来源：http://woi.ctjpmb.com

memset(a, 0, sizeof a);
来源：http://myj.snrcjt.cn

[S27] C：定义常量
来源：http://wex.havefunace.top

const double PI = 3.14159;
来源：http://jry.birdmap.top

[S28] C：静态变量
来源：http://xlh.ywan-chungtsiang.top

static int counter = 0;
来源：http://qlz.c1oappe.top

[S29] C：变参函数
来源：http://lkj.zhixingplan.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mll.guowangkeji.top

[S30] C：头文件保护
来源：http://lqt.haohaochexian.top

#ifndef X_H
来源：http://oyh.hywenlv.cn

#define X_H
来源：http://qmk.quarkkingdee.top

#endif
来源：http://ccy.cdnleiting.top

[S31] C++：Hello World
来源：http://vay.quarkkingdee.top

#include <iostream>
来源：http://rxh.fehbvm.com

int main() { std::cout << "Hello\n"; }
来源：http://gek.yongpay.top

[S32] C++：字符串
来源：http://gtl.jinqigfzy.top

std::string s = "hi";  s += "!";
来源：http://lbl.zdqjudy.top

[S33] C++：vector 增删
来源：http://sfi.ctjpmb.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cai.zhoulong.xyz

[S34] C++：遍历 vector
来源：http://ivf.cheryme.top

for (auto &x : v) { std::cout << x; }
来源：http://igi.andypj.xyz

[S35] C++：map
来源：http://pyx.havefunace.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tam.wangdashe.top

[S36] C++：unordered_map
来源：http://akb.dianchejie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://plt.cucudq.cn

[S37] C++：set
来源：http://ymv.snrcjt.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://iyb.zdqjudy.top

[S38] C++：排序
来源：http://uva.xylfe.cn

std::sort(v.begin(), v.end());
来源：http://sno.tarul.cn

[S39] C++：自定义比较器排序
来源：http://cfl.yueranfly.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tvm.yvedp.cn

[S40] C++：查找元素
来源：http://hzx.sxryk.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ona.yj20258.top

[S41] C++：类与构造函数
来源：http://moy.hammf.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fej.havefunace.top

[S42] C++：继承与虚函数
来源：http://izq.chenlongwang.top

class B : public Base { public: void f() override {} };
来源：http://kes.sysykeji.top

[S43] C++：智能指针
来源：http://qpw.hnxiangtu.top

auto p = std::make_unique<int>(5);
来源：http://iwt.hcnkem.com

[S44] C++：引用传参
来源：http://qar.uphjek.com

void inc(int &x) { ++x; }
来源：http://txe.sufxvd.cn

[S45] C++：lambda
来源：http://vwc.jiagoushi.top

auto add = [](int a, int b) { return a + b; };
来源：http://woh.gogol.net.cn

[S46] C++：函数模板
来源：http://nak.ehwqpu.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bez.shanyushiyangtech.top

[S47] C++：结构化绑定遍历
来源：http://ben.xinyue.icu

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ifh.yvedp.cn

[S48] C++：逐行读文件
来源：http://jtf.hywenlv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fca.zdqjudy.top

while (std::getline(in, line)) { }
来源：http://nwu.jqgfzy.top

[S49] C++：写文件
来源：http://rrv.9152youxi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://stt.jinghuilouyu.cn

[S50] C++：格式化数字
来源：http://ffb.meibo888.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vmk.jiagoushi.top

[S51] C++：显式类型转换
来源：http://ntr.hongshengwenyu.top

static_cast<double>(a) / b
来源：http://wkm.gogol.net.cn

[S52] C++：const 与 noexcept
来源：http://foz.0kj1m.cn

int size() const noexcept { return n_; }
来源：http://mzb.jinqigufen.top

[S53] C++：移动语义
来源：http://sxj.vehdjk.com

std::vector<int> w = std::move(v);
来源：http://mim.epnwcf.com

[S54] C++：异常处理
来源：http://vtf.shanyushiyangtech.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://irh.hywenlv.cn

[S55] C++：结构化绑定
来源：http://afb.shanyushiyangtech.top

auto [a, b] = std::make_pair(1, 2);
来源：http://uho.guannengcc.top

[S56] C++：optional
来源：http://zmh.chenlongwang.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bha.yj202588.top

[S57] C++：编译期常量
来源：http://xyc.zhongyouzk.top

constexpr int N = 10;
来源：http://tdn.snrcjt.cn

[S58] C++：命名空间
来源：http://syf.fzhhl.top

namespace ns { int f() { return 1; } }
来源：http://cna.zhijiandao.cn

[S59] C++：静态断言
来源：http://ljy.hammf.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fhc.zycfv.cn

[S60] C++：遍历并删除元素
来源：http://vyy.haohaochexian.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dyy.chenjidiqi.icu

================================================================================
来源：http://wec.yj20258888.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hjg.ctjpmb.com

================================================================================
来源：http://any.zhengqikj.top

[T01] Kotlin：Hello World
来源：http://pio.yj202588.top

println("Hello")
来源：http://cyg.yongpay.top

[T02] Kotlin：变量
来源：http://hev.ivvv.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zxj.9152youxi.cn

[T03] Kotlin：字符串模板
来源：http://znn.tarul.cn

"值: $b"
来源：http://ons.guannengcc.top

[T04] Kotlin：空安全
来源：http://bok.yvedp.cn

val n: String? = null;  n?.length
来源：http://mxt.vqdsnc.cn

[T05] Kotlin：when 表达式
来源：http://cvq.xuetiantiany.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://oyo.dashuyun.cn

[T06] Kotlin：集合映射
来源：http://cnr.haohaochexian.top

listOf(1, 2, 3).map { it * 2 }
来源：http://xuc.iojbl.cn

[T07] Kotlin：集合过滤
来源：http://pih.xziqi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://kqr.xinyue.icu

[T08] Kotlin：数据类
来源：http://jez.yuanzhike.top

data class User(val name: String, val age: Int)
来源：http://fuv.jinqigufen.top

[T09] Kotlin：扩展函数
来源：http://fdt.snrcjt.cn

fun String.exclaim() = this + "!"
来源：http://jkz.dashuyun.cn

[T10] Kotlin：默认参数
来源：http://rkc.jiagoushi.top

fun greet(name: String = "World") = "Hi $name"
来源：http://iwx.yuxming.cn

[T11] Kotlin：协程
来源：http://yue.tianlin.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://vcc.aizwys.cn

[T12] Kotlin：解构声明
来源：http://mkg.zhoulong.xyz

val (a, b) = Pair(1, 2)
来源：http://yur.daxiang520.top

[T13] Kotlin：只读 Map
来源：http://ffl.9152youxi.cn

val m = mapOf("a" to 1)
来源：http://gji.shuidangran.top

[T14] Kotlin：循环
来源：http://vki.smart0.xyz

for (i in 1..10) println(i)
来源：http://yff.yongpay.top

[T15] Kotlin：接口
来源：http://cpn.pengpengdd.cyou

interface Shape { fun area(): Double }
来源：http://ncu.sysykeji.top

[T16] Swift：Hello World
来源：http://ubn.yvedp.cn

print("Hello")
来源：http://nnc.chenjidiqi.icu

[T17] Swift：变量与常量
来源：http://mmk.shanyushiyangtech.top

var a = 1;  let b = 2
来源：http://cmt.redwolf501.top

[T18] Swift：字符串插值
来源：http://avr.tian-w.cn

"值: \(b)"
来源：http://kyl.yj20258.top

[T19] Swift：可选绑定
来源：http://aar.guannengcc.top

if let n = opt { print(n) }
来源：http://ewg.wangshuangyany.cn

[T20] Swift：数组操作
来源：http://cft.0kj1m.cn

var a = [1, 2, 3];  a.append(4)
来源：http://tlr.nwbrower.top

[T21] Swift：遍历
来源：http://ala.nanxuanxn.top

for x in a { print(x) }
来源：http://eee.52xcode.cn

[T22] Swift：字典
来源：http://zxe.zhengqikj.top

var d = ["a": 1];  d["b"] = 2
来源：http://gvf.xinyue.icu

[T23] Swift：函数
来源：http://wmc.nwbrower.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nkl.cqqwz.cn

[T24] Swift：闭包
来源：http://chm.hcnkem.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://mvu.smart0.xyz

[T25] Swift：结构体
来源：http://tfk.0kj1m.cn

struct P { var x: Int }
来源：http://atf.tianlin.xyz

[T26] Swift：类与重写
来源：http://xbe.xuanzx.com

class A: Base { override func f() {} }
来源：http://bxi.cheryme.top

[T27] Swift：错误处理
来源：http://tuo.sweek.top

do { try f() } catch { print(error) }
来源：http://rpw.gogol.net.cn

[T28] Swift：枚举
来源：http://bpd.tian-w.cn

enum Color { case red, green }
来源：http://emg.hcnkem.com

[T29] Swift：guard 提前返回
来源：http://qmv.jqgfzy.top

guard let x = opt else { return }
来源：http://cqz.ybcxt.top

[T30] Swift：协议
来源：http://zfv.0kj1m.cn

protocol Shape { func area() -> Double }
来源：http://fwv.redwolf501.top

[T31] Lua：Hello World
来源：http://uvr.yvedp.cn

print("Hello")
来源：http://owl.c1oappe.top

[T32] Lua：局部变量
来源：http://ejk.0kj1m.cn

local a = 1
来源：http://dix.feifeiyinyue.top

[T33] Lua：表（数组）
来源：http://plv.tarul.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://mhk.hcnkem.com

[T34] Lua：遍历表
来源：http://mpn.dashuyun.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qjw.hnxiangtu.top

[T35] Lua：字典表
来源：http://kes.tian-w.cn

local d = { a = 1 };  d.b = 2
来源：http://qpy.chenjidiqi.icu

[T36] Lua：函数
来源：http://nol.chenzaomai.com

function add(a, b) return a + b end
来源：http://era.hongshengwenyu.top

[T37] Lua：字符串拼接
来源：http://ars.zdbjq.cn

"a" .. "b"
来源：http://ets.xuetiantiany.cn

[T38] Lua：条件
来源：http://zbl.0kj1m.cn

if x > 0 then print("正") end
来源：http://kkq.fengsongda.top

[T39] Lua：模式匹配
来源：http://zvj.jinqigufen.top

string.find(s, "%d+")
来源：http://osa.dianchejie.cn

[T40] Lua：元表
来源：http://mre.kuanghao11.cn

setmetatable({}, { __index = base })
来源：http://coh.c1oappe.top

[T41] Perl：Hello World
来源：http://xwm.vehdjk.com

print "Hello\n";
来源：http://bqo.xingfuxueyuan.xyz

[T42] Perl：变量类型
来源：http://yot.jinghuilouyu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ojx.sysykeji.top


<!-- 参考信息 -->