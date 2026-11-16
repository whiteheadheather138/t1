代发 wailian999

find . -name "*.log" -type f
来源：http://bjn.tianlin.xyz

[R44] 按修改时间查找
来源：http://qju.hesvh.cn

find . -mtime -7 -type f
来源：http://sot.yueranfly.top

[R45] 批量删除
来源：http://whi.chenlongwang.top

find . -name "*.tmp" -delete
来源：http://shn.c1oappe.top

[R46] 递归替换文件内容
来源：http://esn.yangfankeji.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://awz.yuanzhike.top

[R47] sed 单行替换
来源：http://pnk.cashguo.top

sed -i 's/foo/bar/g' a.txt
来源：http://hjb.jlsjyb.cn

[R48] awk 取指定列
来源：http://mma.hywenlv.cn

awk '{print $1, $3}' a.txt
来源：http://psj.gogol.net.cn

[R49] awk 带条件
来源：http://onc.dashuyun.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ygh.nwbrower.top

[R50] awk 求和
来源：http://ltc.xuanzx.com

awk '{s += $2} END {print s}' a.txt
来源：http://neg.epnwcf.com

[R51] 排序去重取前几
来源：http://ezl.yangfankeji.com

sort a.txt | uniq -c | sort -rn | head
来源：http://jmr.ydjk.org.cn

[R52] 统计行数
来源：http://zaq.cqqwz.cn

wc -l a.txt
来源：http://piv.jinyuanbaomall.cn

[R53] 查看文件头与实时尾
来源：http://zjv.yongpay.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zpo.zhijiandao.cn

[R54] 比较两个文件
来源：http://iig.ivvv.top

diff a.txt b.txt
来源：http://hyg.wangdashe.top

[R55] 压缩与解压
来源：http://pse.smart0.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zyc.jianghu66.top

[R56] 远程拷贝
来源：http://xot.epnwcf.com

scp file user@host:/path/
来源：http://cir.zhongyouzk.top

[R57] 远程执行命令
来源：http://jmq.shuidangran.top

ssh user@host 'uptime'
来源：http://laj.jqgfzy.top

[R58] 下载文件
来源：http://exk.jyoumei.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://phb.jqgufenzy.top

[R59] 发 POST JSON
来源：http://mvv.yvedp.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jsv.0kj1m.cn

[R60] 只看 HTTP 状态码
来源：http://gaa.pengpengdd.cyou

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kux.jinqigufen.top

[R61] 磁盘占用
来源：http://djg.sysykeji.top

df -h;  du -sh *
来源：http://ylz.sufxvd.cn

[R62] 找最占空间的文件
来源：http://htr.zhixingplan.top

du -ah . | sort -rh | head -10
来源：http://edd.sysykeji.top

[R63] 内存与进程
来源：http://hbq.epnwcf.com

free -h;  ps aux | grep nginx
来源：http://tym.yangfankeji.com

[R64] 结束进程
来源：http://nlo.hywenlv.cn

kill -9 $(pgrep -f app.py)
来源：http://xli.ivvv.top

[R65] 查看端口占用
来源：http://xxf.meibo888.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://aiz.aibaodan.cn

[R66] 定时任务
来源：http://mno.hammf.cn

crontab -e;  crontab -l
来源：http://etd.nwbrower.top

[R67] 生成随机十六进制串
来源：http://far.chenzaomai.com

openssl rand -hex 16
来源：http://ccf.jinghuilouyu.cn

[R68] 计算文件校验值
来源：http://gfb.fehbvm.com

sha256sum a.txt;  md5sum a.txt
来源：http://toq.nwbrower.top

[R69] 生成随机密码
来源：http://wdn.shzxlz.cn

head -c 16 /dev/urandom | base64
来源：http://upv.shuidangran.top

[R70] 时间戳与互转
来源：http://jsn.cdnleiting.top

date +%s;  date -d @1700000000
来源：http://jey.yonumen.top

[R71] 日期格式化
来源：http://kgh.gotoacloud.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://tba.cheryme.top

[R72] 等待端口就绪
来源：http://svr.hesvh.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://gat.shuidangran.top

[R73] 分割大日志
来源：http://etn.jianghu66.top

split -l 1000 big.log part_
来源：http://app.iojbl.cn

[R74] 批量重命名
来源：http://zdk.jinqigfzy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zsf.xingfuxueyuan.xyz

[R75] 导出环境变量
来源：http://eyc.c1oappe.top

export PATH="$HOME/bin:$PATH"
来源：http://zpd.fehbvm.com

[R76] 使用临时文件
来源：http://yso.zhijiandao.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bmu.hywenlv.cn

[R77] 读取用户输入
来源：http://tmu.ctjpmb.com

read -rp "请输入: " ans
来源：http://rob.gaohongyu789.top

[R78] 交互式菜单
来源：http://vnd.jiagoushi.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ops.sxryk.cn

[R79] 解析命令行选项
来源：http://jul.xuetiantiany.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gdv.shanyushiyangtech.top

[R80] 查看脚本执行耗时
来源：http://dru.svipenyu.cn

time ./run.sh
来源：http://jjf.gzhubu.top

================================================================================
来源：http://nko.daria6918.cn

S. C / C++ 专题
来源：http://tdz.ctjpmb.com

================================================================================
来源：http://jeg.gogol.net.cn

[S01] C：Hello World
来源：http://cnw.fanxiaobao.xyz

#include <stdio.h>
来源：http://hpi.ctjpmb.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://zmy.wangdashe.top

[S02] C：变量与格式化输出
来源：http://qcd.sjlbkw.cn

int a = 10; printf("%d\n", a);
来源：http://bjn.meibo888.top

[S03] C：读入整数
来源：http://oth.tianlin.xyz

int x; scanf("%d", &x);
来源：http://olx.haohaochexian.top

[S04] C：字符串复制
来源：http://fwk.yanxiufei.cn

char dst[32]; strcpy(dst, "hi");
来源：http://mcv.kuanghao11.cn

[S05] C：字符串长度
来源：http://xgz.xuetiantiany.cn

strlen(s)
来源：http://sqy.zhaomingkeji.xyz

[S06] C：字符串比较
来源：http://ven.c1oappe.top

strcmp(a, b) == 0
来源：http://fpb.zhoulong.xyz

[S07] C：数组遍历求和
来源：http://kvd.gaohongyu789.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mrp.shanyushiyangkeji.top

[S08] C：动态内存分配与释放
来源：http://pta.ydjk.org.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vmi.iojbl.cn

[S09] C：结构体定义与初始化
来源：http://ako.meibo888.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nuh.aibaodan.cn

[S10] C：指针与解引用
来源：http://fvk.sweek.top

int *p = &a;  *p = 5;
来源：http://axe.ydjk.org.cn

[S11] C：逐行读文件
来源：http://bdl.sufxvd.cn

FILE *f = fopen("a.txt", "r");
来源：http://qmt.sxryk.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fhs.yanxiufei.cn

fclose(f);
来源：http://srb.sjlbkw.cn

[S12] C：写文件
来源：http://fpi.ydzc1.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yol.redwolf501.top

[S13] C：宏定义
来源：http://qlh.gotoacloud.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ris.epnwcf.com

[S14] C：枚举
来源：http://kqu.tarul.cn

enum Color { RED, GREEN, BLUE };
来源：http://bwe.sweek.top

[S15] C：类型转换
来源：http://ese.xylfe.cn

(double) a / b
来源：http://xrf.xziqi.cn

[S16] C：位操作置位
来源：http://ngh.yvedp.cn

x |= (1 << 3);
来源：http://fya.cdnleiting.top

[S17] C：安全拼接字符串
来源：http://nyi.aizwys.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lmw.xziqi.cn

[S18] C：命令行参数
来源：http://kgo.svipenyu.cn

int main(int argc, char **argv)
来源：http://myf.daxiang520.top

[S19] C：快速排序
来源：http://vxs.tian-w.cn

qsort(a, n, sizeof(int), cmp);
来源：http://nux.cheryme.top

[S20] C：二分查找
来源：http://gxi.pengpengdd.cyou

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://krr.nanxuanxn.top

[S21] C：字符类别判断
来源：http://boo.shuidangran.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dbx.sufxvd.cn

[S22] C：字符串转数字
来源：http://uce.shanyushiyangtech.top

atoi("42");  strtod("3.14", NULL);
来源：http://xzw.chenzaomai.com

[S23] C：随机数
来源：http://fdh.hesvh.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kik.jinghuilouyu.cn

[S24] C：获取本地时间
来源：http://pgo.bbcook.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zui.zhongyouzk.top

[S25] C：内存拷贝
来源：http://mbt.c1oappe.top

memcpy(dst, src, n);
来源：http://boo.shanyushiyangtech.top

[S26] C：内存清零
来源：http://wwl.9152youxi.cn

memset(a, 0, sizeof a);
来源：http://xyx.sjlbkw.cn

[S27] C：定义常量
来源：http://zww.yj202588.top

const double PI = 3.14159;
来源：http://vkh.snrcjt.cn

[S28] C：静态变量
来源：http://reu.zhengqikj.top

static int counter = 0;
来源：http://mqj.fehbvm.com

[S29] C：变参函数
来源：http://nyj.jinyuanbaomall.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ivn.zhijiandao.cn

[S30] C：头文件保护
来源：http://bvs.chenzaomai.com

#ifndef X_H
来源：http://ixf.ivvv.top

#define X_H
来源：http://vza.zhaomingkeji.xyz

#endif
来源：http://abk.fanxiaobao.xyz

[S31] C++：Hello World
来源：http://bfi.xingfuxueyuan.xyz

#include <iostream>
来源：http://ymt.epnwcf.com

int main() { std::cout << "Hello\n"; }
来源：http://dkv.yueranfly.top

[S32] C++：字符串
来源：http://ild.feifeiyinyue.top

std::string s = "hi";  s += "!";
来源：http://mcw.zhiwuduotai.top

[S33] C++：vector 增删
来源：http://coc.yj20258.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://egb.daxiang520.top

[S34] C++：遍历 vector
来源：http://mdm.ydzc1.top

for (auto &x : v) { std::cout << x; }
来源：http://rkv.dashuyun.cn

[S35] C++：map
来源：http://dcc.dianchejie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zea.yj202588.top

[S36] C++：unordered_map
来源：http://kaz.cashguo.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yyw.gaohongyu789.top

[S37] C++：set
来源：http://tpu.fengsongda.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pof.yuxming.cn

[S38] C++：排序
来源：http://nph.xuanzx.com

std::sort(v.begin(), v.end());
来源：http://wmv.smart0.xyz

[S39] C++：自定义比较器排序
来源：http://oun.sufxvd.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mud.havefunace.top

[S40] C++：查找元素
来源：http://ljm.zhoulong.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vng.haohaochexian.top

[S41] C++：类与构造函数
来源：http://rcx.nanxinkj.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wce.chenzaomai.com

[S42] C++：继承与虚函数
来源：http://jlm.yonumen.top

class B : public Base { public: void f() override {} };
来源：http://dbv.zhaomingkeji.xyz

[S43] C++：智能指针
来源：http://qai.nwbrower.top

auto p = std::make_unique<int>(5);
来源：http://dmv.xylfe.cn

[S44] C++：引用传参
来源：http://qgz.havefunace.top

void inc(int &x) { ++x; }
来源：http://qtf.tarul.cn

[S45] C++：lambda
来源：http://knb.gotoacloud.top

auto add = [](int a, int b) { return a + b; };
来源：http://gfq.jinqigufen.top

[S46] C++：函数模板
来源：http://xaa.kuanghao11.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xpc.gzhubu.top

[S47] C++：结构化绑定遍历
来源：http://ahc.kuanghao11.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sll.aibaodan.cn

[S48] C++：逐行读文件
来源：http://inh.fktsv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://mpp.zdqjudy.top

while (std::getline(in, line)) { }
来源：http://ght.tanke756.top

[S49] C++：写文件
来源：http://fix.smart0.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vdo.chenjidiqi.icu

[S50] C++：格式化数字
来源：http://haz.dianchejie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ojr.birdmap.top

[S51] C++：显式类型转换
来源：http://moh.iojbl.cn

static_cast<double>(a) / b
来源：http://tkw.nanxuanxn.top

[S52] C++：const 与 noexcept
来源：http://dlm.fzhhl.top

int size() const noexcept { return n_; }
来源：http://ekm.sjlbkw.cn

[S53] C++：移动语义
来源：http://jts.zhaomingkeji.xyz

std::vector<int> w = std::move(v);
来源：http://lsr.redwolf501.top

[S54] C++：异常处理
来源：http://imk.chenzaomai.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xiu.zhijiandao.cn

[S55] C++：结构化绑定
来源：http://jrd.epnwcf.com

auto [a, b] = std::make_pair(1, 2);
来源：http://vpr.gogol.net.cn

[S56] C++：optional
来源：http://jyd.fktsv.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ibf.hnxiangtu.top

[S57] C++：编译期常量
来源：http://uwp.yvedp.cn

constexpr int N = 10;
来源：http://hxm.haohaochexian.top

[S58] C++：命名空间
来源：http://gny.fanxiaobao.xyz

namespace ns { int f() { return 1; } }
来源：http://dxc.cqqwz.cn

[S59] C++：静态断言
来源：http://ueb.tianlin.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kjc.hnxiangtu.top

[S60] C++：遍历并删除元素
来源：http://qeu.xziqi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gpw.yj20258.top

================================================================================
来源：http://idw.shangyingyoupin.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dxx.52xcode.cn

================================================================================
来源：http://nbs.vehdjk.com

[T01] Kotlin：Hello World
来源：http://nbo.daxiang520.top

println("Hello")
来源：http://iev.havefunace.top

[T02] Kotlin：变量
来源：http://hnp.zhoulong.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wkt.jqgufenzy.top

[T03] Kotlin：字符串模板
来源：http://ngb.guannengcc.top

"值: $b"
来源：http://mnl.jianghu66.top

[T04] Kotlin：空安全
来源：http://uos.bbcook.cn

val n: String? = null;  n?.length
来源：http://imo.jqgufenzy.top

[T05] Kotlin：when 表达式
来源：http://uch.pengpengdd.cyou

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lsq.zhoulong.xyz

[T06] Kotlin：集合映射
来源：http://ool.gotoacloud.top

listOf(1, 2, 3).map { it * 2 }
来源：http://xyk.jianghu66.top

[T07] Kotlin：集合过滤
来源：http://gej.tian-w.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ygz.xylfe.cn

[T08] Kotlin：数据类
来源：http://ruk.chenzaomai.com

data class User(val name: String, val age: Int)
来源：http://uof.havefunace.top

[T09] Kotlin：扩展函数
来源：http://iut.cheryme.top

fun String.exclaim() = this + "!"
来源：http://fyh.316326.xyz

[T10] Kotlin：默认参数
来源：http://wbo.xuanzx.com

fun greet(name: String = "World") = "Hi $name"
来源：http://pvx.vqdsnc.cn

[T11] Kotlin：协程
来源：http://hdh.zhongyouzk.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://bxm.sweek.top

[T12] Kotlin：解构声明
来源：http://vfr.fengsongda.top

val (a, b) = Pair(1, 2)
来源：http://bxh.hfpthk.cn

[T13] Kotlin：只读 Map
来源：http://agh.jlsjyb.cn

val m = mapOf("a" to 1)
来源：http://dre.nwbrower.top

[T14] Kotlin：循环
来源：http://dal.nanxinkj.top

for (i in 1..10) println(i)
来源：http://upc.zhiwuduotai.top

[T15] Kotlin：接口
来源：http://svt.guannengcc.top

interface Shape { fun area(): Double }
来源：http://odz.bjfxy.top

[T16] Swift：Hello World
来源：http://eya.havefunace.top

print("Hello")
来源：http://ftu.sxryk.cn

[T17] Swift：变量与常量
来源：http://ahk.hnxiangtu.top

var a = 1;  let b = 2
来源：http://zpd.fktsv.cn

[T18] Swift：字符串插值
来源：http://pwa.jqgufenzy.top

"值: \(b)"
来源：http://tnr.hcnkem.com

[T19] Swift：可选绑定
来源：http://wzc.epnwcf.com

if let n = opt { print(n) }
来源：http://dvf.fzhhl.top

[T20] Swift：数组操作
来源：http://wkw.sysykeji.top

var a = [1, 2, 3];  a.append(4)
来源：http://lrq.shanyushiyangtech.top

[T21] Swift：遍历
来源：http://gtk.hfpthk.cn

for x in a { print(x) }
来源：http://ocv.jyoumei.cn

[T22] Swift：字典
来源：http://jrx.fehbvm.com

var d = ["a": 1];  d["b"] = 2
来源：http://mqp.cdnleiting.top

[T23] Swift：函数
来源：http://dxq.mhx1999.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gvy.iojbl.cn

[T24] Swift：闭包
来源：http://pgy.sweek.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://vlb.hnxiangtu.top

[T25] Swift：结构体
来源：http://jvh.xziqi.cn

struct P { var x: Int }
来源：http://mgr.sjlbkw.cn

[T26] Swift：类与重写
来源：http://wnp.quarkkingdee.top

class A: Base { override func f() {} }
来源：http://htc.bjfxy.top

[T27] Swift：错误处理
来源：http://jxl.jlsjyb.cn

do { try f() } catch { print(error) }
来源：http://cvm.hnxiangtu.top

[T28] Swift：枚举
来源：http://zjb.sweek.top

enum Color { case red, green }
来源：http://pog.52xcode.cn

[T29] Swift：guard 提前返回
来源：http://dpe.zdqjudy.top

guard let x = opt else { return }
来源：http://jbd.epnwcf.com

[T30] Swift：协议
来源：http://vhg.nanxuanxn.top

protocol Shape { func area() -> Double }
来源：http://wbj.xingfuxueyuan.xyz

[T31] Lua：Hello World
来源：http://ykz.hammf.cn

print("Hello")
来源：http://fjl.zhiwuduotai.top

[T32] Lua：局部变量
来源：http://uaf.birdmap.top

local a = 1
来源：http://ebj.cucudq.cn

[T33] Lua：表（数组）
来源：http://eya.pycfn.com

local t = {1, 2, 3};  t[4] = 4
来源：http://zea.sjlbkw.cn

[T34] Lua：遍历表
来源：http://bko.shzxlz.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://pmr.guowangkeji.top

[T35] Lua：字典表
来源：http://mhp.jiagoushi.top

local d = { a = 1 };  d.b = 2
来源：http://udf.yfazqb.com

[T36] Lua：函数
来源：http://lqj.yuxming.cn

function add(a, b) return a + b end
来源：http://mkp.jqgfzy.top

[T37] Lua：字符串拼接
来源：http://maa.sjlbkw.cn

"a" .. "b"
来源：http://cgt.cucudq.cn

[T38] Lua：条件
来源：http://xxa.cucudq.cn

if x > 0 then print("正") end
来源：http://vdh.ivvv.top

[T39] Lua：模式匹配
来源：http://dgp.pengpengdd.cyou

string.find(s, "%d+")
来源：http://kmt.uphjek.com

[T40] Lua：元表
来源：http://ecs.svipenyu.cn

setmetatable({}, { __index = base })
来源：http://ctl.zdbjq.cn

[T41] Perl：Hello World
来源：http://kcj.jlsjyb.cn

print "Hello\n";
来源：http://old.bbcook.cn

[T42] Perl：变量类型
来源：http://gqu.shzxlz.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ube.shanyushiyangkeji.top

[T43] Perl：字符串插值
来源：http://map.tian-w.cn

"值: $a"
来源：http://zzf.iojbl.cn

[T44] Perl：条件
来源：http://rji.0kj1m.cn

if ($a > 0) { print "正"; }
来源：http://psx.jinqigufen.top

[T45] Perl：数组遍历
来源：http://lsw.cucudq.cn

for my $x (@arr) { print $x; }
来源：http://uyr.quarkkingdee.top

[T46] Perl：哈希操作
来源：http://kjj.yj20258888.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qjp.gogol.net.cn


<!-- 参考信息 -->