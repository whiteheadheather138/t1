代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://znb.smart0.xyz

[R36] 并发执行多个任务
来源：http://sfy.sufxvd.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://oyl.0kj1m.cn

[R37] 把输出赋给变量
来源：http://gis.svipenyu.cn

files=$(ls -1)
来源：http://nvc.vehdjk.com

[R38] 管道串联
来源：http://xjm.wangshuangyany.cn

cat a.txt | grep -i error | wc -l
来源：http://tyx.yanxiufei.cn

[R39] 重定向标准输出与错误
来源：http://rqx.smart0.xyz

cmd > out.log 2>&1
来源：http://fua.yj202588.top

[R40] 追加写日志
来源：http://lsg.sxryk.cn

echo "log" >> out.log
来源：http://cnk.dianchejie.cn

[R41] 丢弃输出
来源：http://efg.sufxvd.cn

cmd >/dev/null 2>&1
来源：http://zbi.yuxming.cn

[R42] 输入重定向
来源：http://mjv.sysykeji.top

wc -l < a.txt
来源：http://nmo.guannengcc.top

[R43] 按名字查找文件
来源：http://ctg.fehbvm.com

find . -name "*.log" -type f
来源：http://ofo.tarul.cn

[R44] 按修改时间查找
来源：http://kbj.yj20258.top

find . -mtime -7 -type f
来源：http://cdt.xinyue.icu

[R45] 批量删除
来源：http://jym.haohaochexian.top

find . -name "*.tmp" -delete
来源：http://eav.bbcook.cn

[R46] 递归替换文件内容
来源：http://ktx.fzhhl.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kuh.c1oappe.top

[R47] sed 单行替换
来源：http://lso.gaohongyu789.top

sed -i 's/foo/bar/g' a.txt
来源：http://prq.cucudq.cn

[R48] awk 取指定列
来源：http://wnf.yongpay.top

awk '{print $1, $3}' a.txt
来源：http://cqx.hnqzz.top

[R49] awk 带条件
来源：http://hup.snrcjt.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gwt.jlsjyb.cn

[R50] awk 求和
来源：http://iyo.yj20258.top

awk '{s += $2} END {print s}' a.txt
来源：http://dve.0kj1m.cn

[R51] 排序去重取前几
来源：http://rtw.ehwqpu.com

sort a.txt | uniq -c | sort -rn | head
来源：http://pbp.zhixingplan.top

[R52] 统计行数
来源：http://eje.tanke756.top

wc -l a.txt
来源：http://vzp.kuanghao11.cn

[R53] 查看文件头与实时尾
来源：http://sjh.jlsjyb.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rwu.ivvv.top

[R54] 比较两个文件
来源：http://ihq.ybcxt.top

diff a.txt b.txt
来源：http://tbg.yj20258.top

[R55] 压缩与解压
来源：http://nnd.fengsongda.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://imh.tarul.cn

[R56] 远程拷贝
来源：http://uxc.zhiwuduotai.top

scp file user@host:/path/
来源：http://bvg.zhaomingkeji.xyz

[R57] 远程执行命令
来源：http://yxu.ehwqpu.com

ssh user@host 'uptime'
来源：http://uje.shuidangran.top

[R58] 下载文件
来源：http://wxa.cqqwz.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nmk.guannengcc.top

[R59] 发 POST JSON
来源：http://bni.haohaochexian.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dec.yongpay.top

[R60] 只看 HTTP 状态码
来源：http://ffj.fktsv.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://saq.shuidangran.top

[R61] 磁盘占用
来源：http://zys.yj20258888.top

df -h;  du -sh *
来源：http://gxr.ydzc1.top

[R62] 找最占空间的文件
来源：http://fyu.hysaishi.cn

du -ah . | sort -rh | head -10
来源：http://zaz.sxryk.cn

[R63] 内存与进程
来源：http://uij.316326.xyz

free -h;  ps aux | grep nginx
来源：http://vji.epnwcf.com

[R64] 结束进程
来源：http://cbh.gaohongyu789.top

kill -9 $(pgrep -f app.py)
来源：http://upw.daria6918.cn

[R65] 查看端口占用
来源：http://twz.jinyuanbaomall.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rky.shuidangran.top

[R66] 定时任务
来源：http://mkg.ydzc1.top

crontab -e;  crontab -l
来源：http://rat.xziqi.cn

[R67] 生成随机十六进制串
来源：http://vjq.ctjpmb.com

openssl rand -hex 16
来源：http://big.redwolf501.top

[R68] 计算文件校验值
来源：http://ynw.mhx1999.top

sha256sum a.txt;  md5sum a.txt
来源：http://wap.sysykeji.top

[R69] 生成随机密码
来源：http://pwi.jiagoushi.top

head -c 16 /dev/urandom | base64
来源：http://udr.yueranfly.top

[R70] 时间戳与互转
来源：http://irc.aizwys.cn

date +%s;  date -d @1700000000
来源：http://lwg.jqgufenzy.top

[R71] 日期格式化
来源：http://vgq.jiagoushi.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://tzr.c1oappe.top

[R72] 等待端口就绪
来源：http://haj.sjlbkw.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://rlr.sxryk.cn

[R73] 分割大日志
来源：http://ljc.hcnkem.com

split -l 1000 big.log part_
来源：http://yem.tianlin.xyz

[R74] 批量重命名
来源：http://hbe.xingfuxueyuan.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tbp.c1oappe.top

[R75] 导出环境变量
来源：http://qag.yvedp.cn

export PATH="$HOME/bin:$PATH"
来源：http://crd.hywenlv.cn

[R76] 使用临时文件
来源：http://bik.chenzaomai.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qin.hfpthk.cn

[R77] 读取用户输入
来源：http://fsv.guannengcc.top

read -rp "请输入: " ans
来源：http://ohn.snrcjt.cn

[R78] 交互式菜单
来源：http://hqk.feifeiyinyue.top

select opt in a b c; do echo "$opt"; break; done
来源：http://kbk.vqdsnc.cn

[R79] 解析命令行选项
来源：http://fwc.hywenlv.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rjm.gzhubu.top

[R80] 查看脚本执行耗时
来源：http://rig.guannengcc.top

time ./run.sh
来源：http://ttu.wangdashe.top

================================================================================
来源：http://vue.feifeiyinyue.top

S. C / C++ 专题
来源：http://lru.yonumen.top

================================================================================
来源：http://cff.tarul.cn

[S01] C：Hello World
来源：http://yhm.kuanghao11.cn

#include <stdio.h>
来源：http://nkj.sxryk.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://jrm.316326.xyz

[S02] C：变量与格式化输出
来源：http://hdp.sufxvd.cn

int a = 10; printf("%d\n", a);
来源：http://jxt.aizwys.cn

[S03] C：读入整数
来源：http://lmz.haohaochexian.top

int x; scanf("%d", &x);
来源：http://wux.yfazqb.com

[S04] C：字符串复制
来源：http://vec.yj202588.top

char dst[32]; strcpy(dst, "hi");
来源：http://fcx.cucudq.cn

[S05] C：字符串长度
来源：http://awu.yfazqb.com

strlen(s)
来源：http://ptg.zhijiandao.cn

[S06] C：字符串比较
来源：http://gsw.meibo888.top

strcmp(a, b) == 0
来源：http://jqq.birdmap.top

[S07] C：数组遍历求和
来源：http://swe.ydzc1.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vtr.zycfv.cn

[S08] C：动态内存分配与释放
来源：http://qbr.fktsv.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://umb.aizwys.cn

[S09] C：结构体定义与初始化
来源：http://caz.svipenyu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rmo.c1oappe.top

[S10] C：指针与解引用
来源：http://hat.epnwcf.com

int *p = &a;  *p = 5;
来源：http://bfc.daxiang520.top

[S11] C：逐行读文件
来源：http://xyy.sjlbkw.cn

FILE *f = fopen("a.txt", "r");
来源：http://jmz.shanyushiyangkeji.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ivm.cucudq.cn

fclose(f);
来源：http://bdc.dashuyun.cn

[S12] C：写文件
来源：http://vvx.fanxiaobao.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uxd.ydzc1.top

[S13] C：宏定义
来源：http://swl.hfpthk.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gsl.xziqi.cn

[S14] C：枚举
来源：http://zov.tian-w.cn

enum Color { RED, GREEN, BLUE };
来源：http://srw.xylfe.cn

[S15] C：类型转换
来源：http://iik.fzhhl.top

(double) a / b
来源：http://mgh.guannengcc.top

[S16] C：位操作置位
来源：http://kuc.yueranfly.top

x |= (1 << 3);
来源：http://xdm.pengpengdd.cyou

[S17] C：安全拼接字符串
来源：http://ccr.xinyue.icu

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ltu.xziqi.cn

[S18] C：命令行参数
来源：http://jxw.daria6918.cn

int main(int argc, char **argv)
来源：http://jjo.yfazqb.com

[S19] C：快速排序
来源：http://ily.hywenlv.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jol.ivvv.top

[S20] C：二分查找
来源：http://aga.sxryk.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uze.zhengqikj.top

[S21] C：字符类别判断
来源：http://xbx.jqgufenzy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://euz.zycfv.cn

[S22] C：字符串转数字
来源：http://oxv.sxryk.cn

atoi("42");  strtod("3.14", NULL);
来源：http://bse.fktsv.cn

[S23] C：随机数
来源：http://uza.fzhhl.top

srand(time(NULL));  int r = rand() % 100;
来源：http://esu.shangyingyoupin.top

[S24] C：获取本地时间
来源：http://nwc.hammf.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mjl.pycfn.com

[S25] C：内存拷贝
来源：http://ugb.shanyushiyangkeji.top

memcpy(dst, src, n);
来源：http://oky.gotoacloud.top

[S26] C：内存清零
来源：http://zoz.ydjk.org.cn

memset(a, 0, sizeof a);
来源：http://ijg.hammf.cn

[S27] C：定义常量
来源：http://lte.yj202588.top

const double PI = 3.14159;
来源：http://tnz.quarkkingdee.top

[S28] C：静态变量
来源：http://jjd.gotoacloud.top

static int counter = 0;
来源：http://ukt.shanyushiyangkeji.top

[S29] C：变参函数
来源：http://aiy.ybcxt.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://itx.iojbl.cn

[S30] C：头文件保护
来源：http://mtq.nanxinkj.top

#ifndef X_H
来源：http://xli.jqgufenzy.top

#define X_H
来源：http://bno.xinyue.icu

#endif
来源：http://ywf.tarul.cn

[S31] C++：Hello World
来源：http://qfs.dianchejie.cn

#include <iostream>
来源：http://wuy.wangdashe.top

int main() { std::cout << "Hello\n"; }
来源：http://zhf.yj202588.top

[S32] C++：字符串
来源：http://qrs.jianghu66.top

std::string s = "hi";  s += "!";
来源：http://qbj.fzhhl.top

[S33] C++：vector 增删
来源：http://aka.xziqi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ajy.smart0.xyz

[S34] C++：遍历 vector
来源：http://fpu.tian-w.cn

for (auto &x : v) { std::cout << x; }
来源：http://agv.uphjek.com

[S35] C++：map
来源：http://fxn.yj20258888.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cms.ivvv.top

[S36] C++：unordered_map
来源：http://tqn.zhongyouzk.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://eyl.gotoacloud.top

[S37] C++：set
来源：http://oee.gotoacloud.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qmj.gzhubu.top

[S38] C++：排序
来源：http://qsv.zhiwuduotai.top

std::sort(v.begin(), v.end());
来源：http://jvp.snrcjt.cn

[S39] C++：自定义比较器排序
来源：http://zbo.sufxvd.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://drm.zdqjudy.top

[S40] C++：查找元素
来源：http://zet.fktsv.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bpk.gotoacloud.top

[S41] C++：类与构造函数
来源：http://dvy.vqdsnc.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dcx.jinqigufen.top

[S42] C++：继承与虚函数
来源：http://avx.zhixingplan.top

class B : public Base { public: void f() override {} };
来源：http://mzw.jlsjyb.cn

[S43] C++：智能指针
来源：http://ckk.ehwqpu.com

auto p = std::make_unique<int>(5);
来源：http://byh.dianchejie.cn

[S44] C++：引用传参
来源：http://uog.shanyushiyangkeji.top

void inc(int &x) { ++x; }
来源：http://fhm.gogol.net.cn

[S45] C++：lambda
来源：http://inh.fengsongda.top

auto add = [](int a, int b) { return a + b; };
来源：http://xda.52xcode.cn

[S46] C++：函数模板
来源：http://fdq.cqqwz.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tdq.ydzc1.top

[S47] C++：结构化绑定遍历
来源：http://czf.yueranfly.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ppf.ybcxt.top

[S48] C++：逐行读文件
来源：http://ahf.dianchejie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://dcz.shanyushiyangkeji.top

while (std::getline(in, line)) { }
来源：http://eyw.nanxuanxn.top

[S49] C++：写文件
来源：http://god.shanyushiyangkeji.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://azq.nanxinkj.top

[S50] C++：格式化数字
来源：http://ygs.jinqigufen.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kbu.epnwcf.com

[S51] C++：显式类型转换
来源：http://xtg.ehwqpu.com

static_cast<double>(a) / b
来源：http://knk.pycfn.com

[S52] C++：const 与 noexcept
来源：http://twp.wangdashe.top

int size() const noexcept { return n_; }
来源：http://vhg.quarkkingdee.top

[S53] C++：移动语义
来源：http://iox.nanxuanxn.top

std::vector<int> w = std::move(v);
来源：http://dtr.pycfn.com

[S54] C++：异常处理
来源：http://wzc.hfpthk.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qxz.tian-w.cn

[S55] C++：结构化绑定
来源：http://orr.ppjwa.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://nui.zhaomingkeji.xyz

[S56] C++：optional
来源：http://jkq.chenlongwang.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wyb.yangfankeji.com

[S57] C++：编译期常量
来源：http://dev.jyoumei.cn

constexpr int N = 10;
来源：http://ozf.sufxvd.cn

[S58] C++：命名空间
来源：http://eoi.9152youxi.cn

namespace ns { int f() { return 1; } }
来源：http://ecn.ctjpmb.com

[S59] C++：静态断言
来源：http://drd.ivvv.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://svz.xylfe.cn

[S60] C++：遍历并删除元素
来源：http://kmj.svipenyu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fbj.zhixingplan.top

================================================================================
来源：http://wqe.xinyue.icu

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nqc.chenzaomai.com

================================================================================
来源：http://nqa.haohaochexian.top

[T01] Kotlin：Hello World
来源：http://cho.jinyuanbaomall.cn

println("Hello")
来源：http://uem.zdqjudy.top

[T02] Kotlin：变量
来源：http://jtx.jinqigfzy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://prb.sufxvd.cn

[T03] Kotlin：字符串模板
来源：http://efl.haohaochexian.top

"值: $b"
来源：http://eqy.jiagoushi.top

[T04] Kotlin：空安全
来源：http://qxt.xuanzx.com

val n: String? = null;  n?.length
来源：http://tkf.zhiwuduotai.top

[T05] Kotlin：when 表达式
来源：http://oim.yj20258.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fnq.xingfuxueyuan.xyz

[T06] Kotlin：集合映射
来源：http://acf.smart0.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://jhw.pycfn.com

[T07] Kotlin：集合过滤
来源：http://kwj.jinghuilouyu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://cbr.ydzc1.top

[T08] Kotlin：数据类
来源：http://kwg.0kj1m.cn

data class User(val name: String, val age: Int)
来源：http://nfi.shzxlz.cn

[T09] Kotlin：扩展函数
来源：http://eax.shzxlz.cn

fun String.exclaim() = this + "!"
来源：http://kxs.0kj1m.cn

[T10] Kotlin：默认参数
来源：http://rlz.sxryk.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://dei.cashguo.top

[T11] Kotlin：协程
来源：http://aek.ehwqpu.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://zvs.hnxiangtu.top

[T12] Kotlin：解构声明
来源：http://uze.zdbjq.cn

val (a, b) = Pair(1, 2)
来源：http://maf.hywenlv.cn

[T13] Kotlin：只读 Map
来源：http://wih.9152youxi.cn

val m = mapOf("a" to 1)
来源：http://swd.sysykeji.top

[T14] Kotlin：循环
来源：http://ypf.fehbvm.com

for (i in 1..10) println(i)
来源：http://vqk.sufxvd.cn

[T15] Kotlin：接口
来源：http://yyw.uphjek.com

interface Shape { fun area(): Double }
来源：http://wsh.sweek.top

[T16] Swift：Hello World
来源：http://cdi.xylfe.cn

print("Hello")
来源：http://rtb.yvedp.cn

[T17] Swift：变量与常量
来源：http://rhj.316326.xyz

var a = 1;  let b = 2
来源：http://jdm.meibo888.top

[T18] Swift：字符串插值
来源：http://rjx.shuidangran.top

"值: \(b)"
来源：http://yxw.gzhubu.top

[T19] Swift：可选绑定
来源：http://scv.kuanghao11.cn

if let n = opt { print(n) }
来源：http://ewj.jlsjyb.cn

[T20] Swift：数组操作
来源：http://hqd.52xcode.cn

var a = [1, 2, 3];  a.append(4)
来源：http://wsw.ehwqpu.com

[T21] Swift：遍历
来源：http://bhh.tianlin.xyz

for x in a { print(x) }
来源：http://wjl.zycfv.cn

[T22] Swift：字典
来源：http://apn.redwolf501.top

var d = ["a": 1];  d["b"] = 2
来源：http://jwc.gzhubu.top

[T23] Swift：函数
来源：http://iun.shzxlz.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mas.0kj1m.cn

[T24] Swift：闭包
来源：http://xwe.xuetiantiany.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://dhs.0kj1m.cn

[T25] Swift：结构体
来源：http://vkq.sjlbkw.cn

struct P { var x: Int }
来源：http://hlu.cqqwz.cn

[T26] Swift：类与重写
来源：http://geo.guannengcc.top

class A: Base { override func f() {} }
来源：http://mmv.tanke756.top

[T27] Swift：错误处理
来源：http://lct.wangdashe.top

do { try f() } catch { print(error) }
来源：http://eyv.nanxuanxn.top

[T28] Swift：枚举
来源：http://nzf.yuxming.cn

enum Color { case red, green }
来源：http://cnz.guannengcc.top

[T29] Swift：guard 提前返回
来源：http://lof.cashguo.top

guard let x = opt else { return }
来源：http://sgv.shuidangran.top

[T30] Swift：协议
来源：http://ijc.sxryk.cn

protocol Shape { func area() -> Double }
来源：http://cav.shangyingyoupin.top

[T31] Lua：Hello World
来源：http://xcg.wangshuangyany.cn

print("Hello")
来源：http://mig.ctjpmb.com

[T32] Lua：局部变量
来源：http://dph.zhaomingkeji.xyz

local a = 1
来源：http://xaw.quarkkingdee.top

[T33] Lua：表（数组）
来源：http://msd.hongshengwenyu.top

local t = {1, 2, 3};  t[4] = 4
来源：http://pae.jinqigfzy.top

[T34] Lua：遍历表
来源：http://psj.hysaishi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qfc.ehwqpu.com

[T35] Lua：字典表
来源：http://lsl.316326.xyz

local d = { a = 1 };  d.b = 2
来源：http://xli.fktsv.cn

[T36] Lua：函数
来源：http://bsx.shanyushiyangkeji.top

function add(a, b) return a + b end
来源：http://awe.zhijiandao.cn

[T37] Lua：字符串拼接
来源：http://zzu.ydjk.org.cn

"a" .. "b"
来源：http://mnl.yfazqb.com

[T38] Lua：条件
来源：http://fif.xziqi.cn

if x > 0 then print("正") end
来源：http://esh.jqgufenzy.top


<!-- 参考信息 -->