代发 wailian999

find . -name "*.tmp" -delete
来源：http://rrj.guowangkeji.top

[R46] 递归替换文件内容
来源：http://nmi.guowangkeji.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nmc.nanxuanxn.top

[R47] sed 单行替换
来源：http://ttq.kuanghao11.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dgo.zhiwuduotai.top

[R48] awk 取指定列
来源：http://psb.sjlbkw.cn

awk '{print $1, $3}' a.txt
来源：http://ybc.jiagoushi.top

[R49] awk 带条件
来源：http://pmz.yanxiufei.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kus.zhiwuduotai.top

[R50] awk 求和
来源：http://gla.yuxming.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fqr.jinyuanbaomall.cn

[R51] 排序去重取前几
来源：http://xjq.iojbl.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://awm.zhaomingkeji.xyz

[R52] 统计行数
来源：http://qru.daxiang520.top

wc -l a.txt
来源：http://vog.yj20258888.top

[R53] 查看文件头与实时尾
来源：http://epp.zhongyouzk.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zpu.yfazqb.com

[R54] 比较两个文件
来源：http://pwg.xinyue.icu

diff a.txt b.txt
来源：http://jxp.daria6918.cn

[R55] 压缩与解压
来源：http://tjt.xziqi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ojx.yuanzhike.top

[R56] 远程拷贝
来源：http://xbl.fehbvm.com

scp file user@host:/path/
来源：http://iws.aizwys.cn

[R57] 远程执行命令
来源：http://hiy.zhiwuduotai.top

ssh user@host 'uptime'
来源：http://zof.tanke756.top

[R58] 下载文件
来源：http://qel.tarul.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://udi.smart0.xyz

[R59] 发 POST JSON
来源：http://lkd.jinqigufen.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wne.jinghuilouyu.cn

[R60] 只看 HTTP 状态码
来源：http://bdo.feifeiyinyue.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://egz.shangyingyoupin.top

[R61] 磁盘占用
来源：http://olo.xingfuxueyuan.xyz

df -h;  du -sh *
来源：http://trf.tianlin.xyz

[R62] 找最占空间的文件
来源：http://gpb.aizwys.cn

du -ah . | sort -rh | head -10
来源：http://wts.yj20258.top

[R63] 内存与进程
来源：http://hqa.daxiang520.top

free -h;  ps aux | grep nginx
来源：http://ggn.gzhubu.top

[R64] 结束进程
来源：http://shl.hnqzz.top

kill -9 $(pgrep -f app.py)
来源：http://zff.meibo888.top

[R65] 查看端口占用
来源：http://hjw.havefunace.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gvs.yonumen.top

[R66] 定时任务
来源：http://xly.cdnleiting.top

crontab -e;  crontab -l
来源：http://uhb.redwolf501.top

[R67] 生成随机十六进制串
来源：http://jhf.gogol.net.cn

openssl rand -hex 16
来源：http://acz.bjfxy.top

[R68] 计算文件校验值
来源：http://vop.ydzc1.top

sha256sum a.txt;  md5sum a.txt
来源：http://ffg.hnqzz.top

[R69] 生成随机密码
来源：http://rik.hongshengwenyu.top

head -c 16 /dev/urandom | base64
来源：http://plg.sufxvd.cn

[R70] 时间戳与互转
来源：http://eeo.yuxming.cn

date +%s;  date -d @1700000000
来源：http://dku.redwolf501.top

[R71] 日期格式化
来源：http://bfq.vehdjk.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://dua.zhixingplan.top

[R72] 等待端口就绪
来源：http://tse.yuxming.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ose.guannengcc.top

[R73] 分割大日志
来源：http://npn.yongpay.top

split -l 1000 big.log part_
来源：http://vti.xziqi.cn

[R74] 批量重命名
来源：http://und.ydjk.org.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mpo.hammf.cn

[R75] 导出环境变量
来源：http://loi.xylfe.cn

export PATH="$HOME/bin:$PATH"
来源：http://cvw.pengpengdd.cyou

[R76] 使用临时文件
来源：http://lpr.ydjk.org.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wvo.pengpengdd.cyou

[R77] 读取用户输入
来源：http://epq.ctjpmb.com

read -rp "请输入: " ans
来源：http://nwb.hnqzz.top

[R78] 交互式菜单
来源：http://bsk.jinghuilouyu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zqf.pycfn.com

[R79] 解析命令行选项
来源：http://bbp.gaohongyu789.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://non.316326.xyz

[R80] 查看脚本执行耗时
来源：http://wdw.snrcjt.cn

time ./run.sh
来源：http://qze.zhixingplan.top

================================================================================
来源：http://cqi.yongpay.top

S. C / C++ 专题
来源：http://zrx.yfazqb.com

================================================================================
来源：http://vqs.dianchejie.cn

[S01] C：Hello World
来源：http://fet.haohaochexian.top

#include <stdio.h>
来源：http://vrx.quarkkingdee.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://xts.ctjpmb.com

[S02] C：变量与格式化输出
来源：http://ori.aibaodan.cn

int a = 10; printf("%d\n", a);
来源：http://ekk.yfazqb.com

[S03] C：读入整数
来源：http://lez.yfazqb.com

int x; scanf("%d", &x);
来源：http://vnu.epnwcf.com

[S04] C：字符串复制
来源：http://sup.chenzaomai.com

char dst[32]; strcpy(dst, "hi");
来源：http://phf.chenlongwang.top

[S05] C：字符串长度
来源：http://pyw.daxiang520.top

strlen(s)
来源：http://ssh.zhongyouzk.top

[S06] C：字符串比较
来源：http://fcs.jlsjyb.cn

strcmp(a, b) == 0
来源：http://cwd.kuanghao11.cn

[S07] C：数组遍历求和
来源：http://ejt.nanxuanxn.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ols.zhiwuduotai.top

[S08] C：动态内存分配与释放
来源：http://vih.hammf.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://upr.snrcjt.cn

[S09] C：结构体定义与初始化
来源：http://etp.hfpthk.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gzs.havefunace.top

[S10] C：指针与解引用
来源：http://ctd.jinghuilouyu.cn

int *p = &a;  *p = 5;
来源：http://iti.snrcjt.cn

[S11] C：逐行读文件
来源：http://bhb.fehbvm.com

FILE *f = fopen("a.txt", "r");
来源：http://vhz.zhixingplan.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://rxo.zhongyouzk.top

fclose(f);
来源：http://qon.cashguo.top

[S12] C：写文件
来源：http://sgt.tarul.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qdg.zhixingplan.top

[S13] C：宏定义
来源：http://rxn.yuanzhike.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qoq.jinqigfzy.top

[S14] C：枚举
来源：http://baf.xinyue.icu

enum Color { RED, GREEN, BLUE };
来源：http://yhp.ydzc1.top

[S15] C：类型转换
来源：http://jgj.hywenlv.cn

(double) a / b
来源：http://yjw.jinqigufen.top

[S16] C：位操作置位
来源：http://veo.gzhubu.top

x |= (1 << 3);
来源：http://srt.zhiwuduotai.top

[S17] C：安全拼接字符串
来源：http://nvf.yanxiufei.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://isk.gzhubu.top

[S18] C：命令行参数
来源：http://vhe.zhiwuduotai.top

int main(int argc, char **argv)
来源：http://aby.zdqjudy.top

[S19] C：快速排序
来源：http://mvv.xziqi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://csi.fengsongda.top

[S20] C：二分查找
来源：http://hwi.yanxiufei.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ejb.hammf.cn

[S21] C：字符类别判断
来源：http://lmd.sweek.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ttu.yj202588.top

[S22] C：字符串转数字
来源：http://lwz.haohaochexian.top

atoi("42");  strtod("3.14", NULL);
来源：http://jly.52xcode.cn

[S23] C：随机数
来源：http://jxm.iojbl.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bnt.fktsv.cn

[S24] C：获取本地时间
来源：http://crz.fktsv.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dyk.ivvv.top

[S25] C：内存拷贝
来源：http://nzq.zdqjudy.top

memcpy(dst, src, n);
来源：http://mmn.zhongyouzk.top

[S26] C：内存清零
来源：http://bhl.c1oappe.top

memset(a, 0, sizeof a);
来源：http://mdq.dianchejie.cn

[S27] C：定义常量
来源：http://owi.quarkkingdee.top

const double PI = 3.14159;
来源：http://xcc.ivvv.top

[S28] C：静态变量
来源：http://xll.cashguo.top

static int counter = 0;
来源：http://jax.epnwcf.com

[S29] C：变参函数
来源：http://mzl.snrcjt.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://seh.9152youxi.cn

[S30] C：头文件保护
来源：http://ehh.nanxinkj.top

#ifndef X_H
来源：http://rfw.ivvv.top

#define X_H
来源：http://kic.smart0.xyz

#endif
来源：http://ncf.aibaodan.cn

[S31] C++：Hello World
来源：http://kae.jyoumei.cn

#include <iostream>
来源：http://buh.hcnkem.com

int main() { std::cout << "Hello\n"; }
来源：http://ctq.uphjek.com

[S32] C++：字符串
来源：http://acc.daria6918.cn

std::string s = "hi";  s += "!";
来源：http://vtq.zhixingplan.top

[S33] C++：vector 增删
来源：http://irc.birdmap.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qbj.zhoulong.xyz

[S34] C++：遍历 vector
来源：http://ptk.sysykeji.top

for (auto &x : v) { std::cout << x; }
来源：http://hui.hongshengwenyu.top

[S35] C++：map
来源：http://bdk.fanxiaobao.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://oyu.sxryk.cn

[S36] C++：unordered_map
来源：http://nho.zhoulong.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qqy.fehbvm.com

[S37] C++：set
来源：http://wka.chenzaomai.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://stb.zhoulong.xyz

[S38] C++：排序
来源：http://oqf.feifeiyinyue.top

std::sort(v.begin(), v.end());
来源：http://xyb.zdqjudy.top

[S39] C++：自定义比较器排序
来源：http://wzl.vehdjk.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://noe.yongpay.top

[S40] C++：查找元素
来源：http://exa.birdmap.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tmv.iojbl.cn

[S41] C++：类与构造函数
来源：http://dbx.chenjidiqi.icu

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://koy.uphjek.com

[S42] C++：继承与虚函数
来源：http://rhq.uphjek.com

class B : public Base { public: void f() override {} };
来源：http://nbu.hesvh.cn

[S43] C++：智能指针
来源：http://kkn.shanyushiyangtech.top

auto p = std::make_unique<int>(5);
来源：http://gda.pycfn.com

[S44] C++：引用传参
来源：http://zql.kuanghao11.cn

void inc(int &x) { ++x; }
来源：http://yae.shanyushiyangkeji.top

[S45] C++：lambda
来源：http://eal.yangfankeji.com

auto add = [](int a, int b) { return a + b; };
来源：http://fsx.tarul.cn

[S46] C++：函数模板
来源：http://mwv.aizwys.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ywb.iojbl.cn

[S47] C++：结构化绑定遍历
来源：http://lqi.sweek.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rvq.daria6918.cn

[S48] C++：逐行读文件
来源：http://wid.ydzc1.top

std::ifstream in("a.txt");  std::string line;
来源：http://tfd.ppjwa.cn

while (std::getline(in, line)) { }
来源：http://qnu.tianlin.xyz

[S49] C++：写文件
来源：http://mcg.chenlongwang.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dbg.quarkkingdee.top

[S50] C++：格式化数字
来源：http://oqe.yangfankeji.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lqj.chenjidiqi.icu

[S51] C++：显式类型转换
来源：http://dda.nwbrower.top

static_cast<double>(a) / b
来源：http://ksp.ctjpmb.com

[S52] C++：const 与 noexcept
来源：http://vnc.gogol.net.cn

int size() const noexcept { return n_; }
来源：http://pgp.hammf.cn

[S53] C++：移动语义
来源：http://yog.c1oappe.top

std::vector<int> w = std::move(v);
来源：http://kul.yj20258888.top

[S54] C++：异常处理
来源：http://aba.dashuyun.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dhe.sufxvd.cn

[S55] C++：结构化绑定
来源：http://hpu.shanyushiyangtech.top

auto [a, b] = std::make_pair(1, 2);
来源：http://yta.cheryme.top

[S56] C++：optional
来源：http://yfe.yongpay.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mgt.cashguo.top

[S57] C++：编译期常量
来源：http://jzi.cucudq.cn

constexpr int N = 10;
来源：http://oas.hysaishi.cn

[S58] C++：命名空间
来源：http://gwa.sysykeji.top

namespace ns { int f() { return 1; } }
来源：http://qaf.xinyue.icu

[S59] C++：静态断言
来源：http://tjz.ydzc1.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pvg.sufxvd.cn

[S60] C++：遍历并删除元素
来源：http://hlm.jiagoushi.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yye.feifeiyinyue.top

================================================================================
来源：http://nyb.chenzaomai.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pic.snrcjt.cn

================================================================================
来源：http://igx.snrcjt.cn

[T01] Kotlin：Hello World
来源：http://kun.gzhubu.top

println("Hello")
来源：http://fuy.bjfxy.top

[T02] Kotlin：变量
来源：http://gqe.cdnleiting.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yyc.ydjk.org.cn

[T03] Kotlin：字符串模板
来源：http://ihn.hesvh.cn

"值: $b"
来源：http://vho.tian-w.cn

[T04] Kotlin：空安全
来源：http://vvm.bbcook.cn

val n: String? = null;  n?.length
来源：http://ljg.shzxlz.cn

[T05] Kotlin：when 表达式
来源：http://akt.vqdsnc.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bwk.ybcxt.top

[T06] Kotlin：集合映射
来源：http://ooq.tanke756.top

listOf(1, 2, 3).map { it * 2 }
来源：http://hqi.haohaochexian.top

[T07] Kotlin：集合过滤
来源：http://mbj.shanyushiyangkeji.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://bar.xuanzx.com

[T08] Kotlin：数据类
来源：http://inj.kuanghao11.cn

data class User(val name: String, val age: Int)
来源：http://epc.yvedp.cn

[T09] Kotlin：扩展函数
来源：http://gmp.kuanghao11.cn

fun String.exclaim() = this + "!"
来源：http://duu.316326.xyz

[T10] Kotlin：默认参数
来源：http://pzk.yuanzhike.top

fun greet(name: String = "World") = "Hi $name"
来源：http://bwg.gaohongyu789.top

[T11] Kotlin：协程
来源：http://ffj.shuidangran.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ojc.bbcook.cn

[T12] Kotlin：解构声明
来源：http://rgn.sjlbkw.cn

val (a, b) = Pair(1, 2)
来源：http://ekw.smart0.xyz

[T13] Kotlin：只读 Map
来源：http://dzd.sweek.top

val m = mapOf("a" to 1)
来源：http://jeb.nanxuanxn.top

[T14] Kotlin：循环
来源：http://jdk.zhaomingkeji.xyz

for (i in 1..10) println(i)
来源：http://tqw.aibaodan.cn

[T15] Kotlin：接口
来源：http://ayc.jianghu66.top

interface Shape { fun area(): Double }
来源：http://ldv.jqgufenzy.top

[T16] Swift：Hello World
来源：http://fnm.zhongyouzk.top

print("Hello")
来源：http://gji.bjfxy.top

[T17] Swift：变量与常量
来源：http://zck.cashguo.top

var a = 1;  let b = 2
来源：http://pmt.zdbjq.cn

[T18] Swift：字符串插值
来源：http://bkj.zhongyouzk.top

"值: \(b)"
来源：http://gzf.daria6918.cn

[T19] Swift：可选绑定
来源：http://azb.zhixingplan.top

if let n = opt { print(n) }
来源：http://ngu.shangyingyoupin.top

[T20] Swift：数组操作
来源：http://qaz.ywan-chungtsiang.top

var a = [1, 2, 3];  a.append(4)
来源：http://ilf.yongpay.top

[T21] Swift：遍历
来源：http://woj.sufxvd.cn

for x in a { print(x) }
来源：http://mww.sysykeji.top

[T22] Swift：字典
来源：http://bck.xuetiantiany.cn

var d = ["a": 1];  d["b"] = 2
来源：http://trz.daria6918.cn

[T23] Swift：函数
来源：http://hop.kuanghao11.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wto.ydjk.org.cn

[T24] Swift：闭包
来源：http://zan.vqdsnc.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://pqz.snrcjt.cn

[T25] Swift：结构体
来源：http://xih.cqqwz.cn

struct P { var x: Int }
来源：http://yvx.hesvh.cn

[T26] Swift：类与重写
来源：http://lir.birdmap.top

class A: Base { override func f() {} }
来源：http://tbh.ywan-chungtsiang.top

[T27] Swift：错误处理
来源：http://fce.bjfxy.top

do { try f() } catch { print(error) }
来源：http://jmu.shanyushiyangkeji.top

[T28] Swift：枚举
来源：http://ayo.shangyingyoupin.top

enum Color { case red, green }
来源：http://mpn.daria6918.cn

[T29] Swift：guard 提前返回
来源：http://ogt.dianchejie.cn

guard let x = opt else { return }
来源：http://lok.zhijiandao.cn

[T30] Swift：协议
来源：http://mse.pycfn.com

protocol Shape { func area() -> Double }
来源：http://izr.sweek.top

[T31] Lua：Hello World
来源：http://sgq.fanxiaobao.xyz

print("Hello")
来源：http://xcw.cucudq.cn

[T32] Lua：局部变量
来源：http://bcv.andypj.xyz

local a = 1
来源：http://wyh.gzhubu.top

[T33] Lua：表（数组）
来源：http://fjg.fehbvm.com

local t = {1, 2, 3};  t[4] = 4
来源：http://ycx.yueranfly.top

[T34] Lua：遍历表
来源：http://wnk.ydjk.org.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rtq.dianchejie.cn

[T35] Lua：字典表
来源：http://wng.zdqjudy.top

local d = { a = 1 };  d.b = 2
来源：http://wnn.zhaomingkeji.xyz

[T36] Lua：函数
来源：http://kdh.snrcjt.cn

function add(a, b) return a + b end
来源：http://ekt.jinyuanbaomall.cn

[T37] Lua：字符串拼接
来源：http://ueh.fzhhl.top

"a" .. "b"
来源：http://jaj.shzxlz.cn

[T38] Lua：条件
来源：http://wgk.daria6918.cn

if x > 0 then print("正") end
来源：http://sqs.birdmap.top

[T39] Lua：模式匹配
来源：http://sym.cucudq.cn

string.find(s, "%d+")
来源：http://rzb.andypj.xyz

[T40] Lua：元表
来源：http://ext.xuetiantiany.cn

setmetatable({}, { __index = base })
来源：http://ctr.bbcook.cn

[T41] Perl：Hello World
来源：http://fno.vehdjk.com

print "Hello\n";
来源：http://mvz.sufxvd.cn

[T42] Perl：变量类型
来源：http://hdh.feifeiyinyue.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kzm.yueranfly.top

[T43] Perl：字符串插值
来源：http://lsl.xuetiantiany.cn

"值: $a"
来源：http://hkz.fzhhl.top

[T44] Perl：条件
来源：http://amw.hnqzz.top

if ($a > 0) { print "正"; }
来源：http://vzy.ppjwa.cn

[T45] Perl：数组遍历
来源：http://zkn.zhixingplan.top

for my $x (@arr) { print $x; }
来源：http://wac.shangyingyoupin.top

[T46] Perl：哈希操作
来源：http://sxe.hammf.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wht.fzhhl.top

[T47] Perl：正则捕获
来源：http://zup.fanxiaobao.xyz

if ($s =~ /(\d+)/) { print $1; }
来源：http://yss.yonumen.top

[T48] Perl：正则替换
来源：http://izi.nanxuanxn.top

$s =~ s/old/new/g;
来源：http://rtu.sxryk.cn


<!-- 参考信息 -->