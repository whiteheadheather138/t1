代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://rzc.jlsjyb.cn

[R36] 并发执行多个任务
来源：http://qnm.birdmap.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dex.tanke756.top

[R37] 把输出赋给变量
来源：http://lov.yj20258.top

files=$(ls -1)
来源：http://dpr.jlsjyb.cn

[R38] 管道串联
来源：http://tlr.daria6918.cn

cat a.txt | grep -i error | wc -l
来源：http://yue.yueranfly.top

[R39] 重定向标准输出与错误
来源：http://biy.xylfe.cn

cmd > out.log 2>&1
来源：http://clb.yonumen.top

[R40] 追加写日志
来源：http://get.jinyuanbaomall.cn

echo "log" >> out.log
来源：http://gnx.sxryk.cn

[R41] 丢弃输出
来源：http://ixg.svipenyu.cn

cmd >/dev/null 2>&1
来源：http://ncq.tian-w.cn

[R42] 输入重定向
来源：http://gce.fktsv.cn

wc -l < a.txt
来源：http://ffd.ywan-chungtsiang.top

[R43] 按名字查找文件
来源：http://zwt.ydzc1.top

find . -name "*.log" -type f
来源：http://ijc.shanyushiyangtech.top

[R44] 按修改时间查找
来源：http://lxg.ywan-chungtsiang.top

find . -mtime -7 -type f
来源：http://djy.hongshengwenyu.top

[R45] 批量删除
来源：http://kwn.quarkkingdee.top

find . -name "*.tmp" -delete
来源：http://tid.jinqigufen.top

[R46] 递归替换文件内容
来源：http://jez.meibo888.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jjf.sjlbkw.cn

[R47] sed 单行替换
来源：http://tcz.hnxiangtu.top

sed -i 's/foo/bar/g' a.txt
来源：http://ehm.fanxiaobao.xyz

[R48] awk 取指定列
来源：http://lzj.yongpay.top

awk '{print $1, $3}' a.txt
来源：http://xbj.ywan-chungtsiang.top

[R49] awk 带条件
来源：http://ajm.quarkkingdee.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lti.hongshengwenyu.top

[R50] awk 求和
来源：http://pra.havefunace.top

awk '{s += $2} END {print s}' a.txt
来源：http://sdg.dianchejie.cn

[R51] 排序去重取前几
来源：http://ehh.jqgufenzy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://lyd.yj202588.top

[R52] 统计行数
来源：http://qdw.guannengcc.top

wc -l a.txt
来源：http://hvp.yueranfly.top

[R53] 查看文件头与实时尾
来源：http://rpv.ydjk.org.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dhx.c1oappe.top

[R54] 比较两个文件
来源：http://mcd.pycfn.com

diff a.txt b.txt
来源：http://gyb.jinghuilouyu.cn

[R55] 压缩与解压
来源：http://wgv.shangyingyoupin.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kzr.havefunace.top

[R56] 远程拷贝
来源：http://nmw.kuanghao11.cn

scp file user@host:/path/
来源：http://bzq.quarkkingdee.top

[R57] 远程执行命令
来源：http://ibl.daxiang520.top

ssh user@host 'uptime'
来源：http://ubh.xinyue.icu

[R58] 下载文件
来源：http://xcu.hesvh.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jxx.jinqigufen.top

[R59] 发 POST JSON
来源：http://bgu.guannengcc.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://uhv.zdbjq.cn

[R60] 只看 HTTP 状态码
来源：http://uug.guowangkeji.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ydw.hongshengwenyu.top

[R61] 磁盘占用
来源：http://vfe.sweek.top

df -h;  du -sh *
来源：http://hhq.epnwcf.com

[R62] 找最占空间的文件
来源：http://wlv.gzhubu.top

du -ah . | sort -rh | head -10
来源：http://mfl.c1oappe.top

[R63] 内存与进程
来源：http://ntq.wangdashe.top

free -h;  ps aux | grep nginx
来源：http://zju.sufxvd.cn

[R64] 结束进程
来源：http://mab.wangshuangyany.cn

kill -9 $(pgrep -f app.py)
来源：http://egb.smart0.xyz

[R65] 查看端口占用
来源：http://kem.fktsv.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://knh.ydzc1.top

[R66] 定时任务
来源：http://bgr.jiagoushi.top

crontab -e;  crontab -l
来源：http://kwm.fengsongda.top

[R67] 生成随机十六进制串
来源：http://gwt.bjfxy.top

openssl rand -hex 16
来源：http://jlu.yueranfly.top

[R68] 计算文件校验值
来源：http://aoz.zhengqikj.top

sha256sum a.txt;  md5sum a.txt
来源：http://ozf.sysykeji.top

[R69] 生成随机密码
来源：http://zod.jinqigufen.top

head -c 16 /dev/urandom | base64
来源：http://vkf.yj20258888.top

[R70] 时间戳与互转
来源：http://owp.yongpay.top

date +%s;  date -d @1700000000
来源：http://pxp.smart0.xyz

[R71] 日期格式化
来源：http://xmr.kuanghao11.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ohf.wangshuangyany.cn

[R72] 等待端口就绪
来源：http://inn.dianchejie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://aeu.jinqigfzy.top

[R73] 分割大日志
来源：http://sra.tian-w.cn

split -l 1000 big.log part_
来源：http://agl.aizwys.cn

[R74] 批量重命名
来源：http://vyp.yj20258888.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mxc.zhixingplan.top

[R75] 导出环境变量
来源：http://ecy.cqqwz.cn

export PATH="$HOME/bin:$PATH"
来源：http://hiu.fanxiaobao.xyz

[R76] 使用临时文件
来源：http://afx.tarul.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jfk.c1oappe.top

[R77] 读取用户输入
来源：http://ahh.hammf.cn

read -rp "请输入: " ans
来源：http://epp.redwolf501.top

[R78] 交互式菜单
来源：http://djl.jianghu66.top

select opt in a b c; do echo "$opt"; break; done
来源：http://giu.jinqigufen.top

[R79] 解析命令行选项
来源：http://sls.zdqjudy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://oos.jinqigufen.top

[R80] 查看脚本执行耗时
来源：http://tdk.ydzc1.top

time ./run.sh
来源：http://jep.dianchejie.cn

================================================================================
来源：http://zko.cdnleiting.top

S. C / C++ 专题
来源：http://bgo.bjfxy.top

================================================================================
来源：http://ugk.xuanzx.com

[S01] C：Hello World
来源：http://dqn.zhixingplan.top

#include <stdio.h>
来源：http://yud.ctjpmb.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://oyf.jinqigufen.top

[S02] C：变量与格式化输出
来源：http://qlq.hnqzz.top

int a = 10; printf("%d\n", a);
来源：http://zqu.ivvv.top

[S03] C：读入整数
来源：http://jbc.hesvh.cn

int x; scanf("%d", &x);
来源：http://fay.bjfxy.top

[S04] C：字符串复制
来源：http://kwp.kuanghao11.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zhp.yj20258888.top

[S05] C：字符串长度
来源：http://shq.zhijiandao.cn

strlen(s)
来源：http://gps.shzxlz.cn

[S06] C：字符串比较
来源：http://hfd.shangyingyoupin.top

strcmp(a, b) == 0
来源：http://suc.316326.xyz

[S07] C：数组遍历求和
来源：http://pgw.ctjpmb.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gkg.fengsongda.top

[S08] C：动态内存分配与释放
来源：http://ydl.sjlbkw.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ayg.gotoacloud.top

[S09] C：结构体定义与初始化
来源：http://tbg.jinyuanbaomall.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bcv.pycfn.com

[S10] C：指针与解引用
来源：http://qin.xuetiantiany.cn

int *p = &a;  *p = 5;
来源：http://jal.shanyushiyangkeji.top

[S11] C：逐行读文件
来源：http://nos.yongpay.top

FILE *f = fopen("a.txt", "r");
来源：http://gps.gogol.net.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hqo.smart0.xyz

fclose(f);
来源：http://wwz.sufxvd.cn

[S12] C：写文件
来源：http://eme.bbcook.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cyu.quarkkingdee.top

[S13] C：宏定义
来源：http://tkh.yfazqb.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://drn.gogol.net.cn

[S14] C：枚举
来源：http://txd.yuxming.cn

enum Color { RED, GREEN, BLUE };
来源：http://jhi.epnwcf.com

[S15] C：类型转换
来源：http://efm.zhengqikj.top

(double) a / b
来源：http://cnl.ctjpmb.com

[S16] C：位操作置位
来源：http://auf.cdnleiting.top

x |= (1 << 3);
来源：http://otk.shanyushiyangkeji.top

[S17] C：安全拼接字符串
来源：http://vro.ctjpmb.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zbu.bjfxy.top

[S18] C：命令行参数
来源：http://rcp.andypj.xyz

int main(int argc, char **argv)
来源：http://mon.jqgfzy.top

[S19] C：快速排序
来源：http://xky.aibaodan.cn

qsort(a, n, sizeof(int), cmp);
来源：http://laj.dashuyun.cn

[S20] C：二分查找
来源：http://pka.chenlongwang.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xqp.fktsv.cn

[S21] C：字符类别判断
来源：http://oyo.nanxuanxn.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mcd.yuxming.cn

[S22] C：字符串转数字
来源：http://lbv.iojbl.cn

atoi("42");  strtod("3.14", NULL);
来源：http://jfv.svipenyu.cn

[S23] C：随机数
来源：http://kfd.cashguo.top

srand(time(NULL));  int r = rand() % 100;
来源：http://vcq.yueranfly.top

[S24] C：获取本地时间
来源：http://usf.guannengcc.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fqr.fehbvm.com

[S25] C：内存拷贝
来源：http://sff.zhixingplan.top

memcpy(dst, src, n);
来源：http://knj.smart0.xyz

[S26] C：内存清零
来源：http://kfc.yj202588.top

memset(a, 0, sizeof a);
来源：http://qkt.fzhhl.top

[S27] C：定义常量
来源：http://zwt.xuanzx.com

const double PI = 3.14159;
来源：http://lcd.gzhubu.top

[S28] C：静态变量
来源：http://yjm.cdnleiting.top

static int counter = 0;
来源：http://fcz.guowangkeji.top

[S29] C：变参函数
来源：http://erq.yueranfly.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://eiz.tianlin.xyz

[S30] C：头文件保护
来源：http://xta.cqqwz.cn

#ifndef X_H
来源：http://rij.zhoulong.xyz

#define X_H
来源：http://bwe.pengpengdd.cyou

#endif
来源：http://jrn.zhoulong.xyz

[S31] C++：Hello World
来源：http://sjs.havefunace.top

#include <iostream>
来源：http://fic.epnwcf.com

int main() { std::cout << "Hello\n"; }
来源：http://uqo.chenzaomai.com

[S32] C++：字符串
来源：http://nmg.nanxuanxn.top

std::string s = "hi";  s += "!";
来源：http://roo.zhiwuduotai.top

[S33] C++：vector 增删
来源：http://fox.xziqi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fbg.yfazqb.com

[S34] C++：遍历 vector
来源：http://hvz.yvedp.cn

for (auto &x : v) { std::cout << x; }
来源：http://bbl.zhoulong.xyz

[S35] C++：map
来源：http://pwv.gogol.net.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ydd.pycfn.com

[S36] C++：unordered_map
来源：http://qxc.cdnleiting.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rry.yangfankeji.com

[S37] C++：set
来源：http://ule.jlsjyb.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hvj.yvedp.cn

[S38] C++：排序
来源：http://kiz.guannengcc.top

std::sort(v.begin(), v.end());
来源：http://ugm.svipenyu.cn

[S39] C++：自定义比较器排序
来源：http://lqn.ehwqpu.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://apa.sjlbkw.cn

[S40] C++：查找元素
来源：http://olw.chenlongwang.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wlz.hywenlv.cn

[S41] C++：类与构造函数
来源：http://kfn.yuanzhike.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://khl.wangshuangyany.cn

[S42] C++：继承与虚函数
来源：http://pbe.zdbjq.cn

class B : public Base { public: void f() override {} };
来源：http://llj.cashguo.top

[S43] C++：智能指针
来源：http://qak.zhiwuduotai.top

auto p = std::make_unique<int>(5);
来源：http://llq.yj202588.top

[S44] C++：引用传参
来源：http://fux.0kj1m.cn

void inc(int &x) { ++x; }
来源：http://aqb.ywan-chungtsiang.top

[S45] C++：lambda
来源：http://dwj.fanxiaobao.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://htu.nanxinkj.top

[S46] C++：函数模板
来源：http://jcp.zdbjq.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ffy.snrcjt.cn

[S47] C++：结构化绑定遍历
来源：http://bxb.gzhubu.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rkg.pycfn.com

[S48] C++：逐行读文件
来源：http://cnj.snrcjt.cn

std::ifstream in("a.txt");  std::string line;
来源：http://llx.gogol.net.cn

while (std::getline(in, line)) { }
来源：http://xvx.yanxiufei.cn

[S49] C++：写文件
来源：http://iwn.snrcjt.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://okj.316326.xyz

[S50] C++：格式化数字
来源：http://fea.yueranfly.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ofi.cheryme.top

[S51] C++：显式类型转换
来源：http://mzt.yj202588.top

static_cast<double>(a) / b
来源：http://tgj.cheryme.top

[S52] C++：const 与 noexcept
来源：http://hft.cheryme.top

int size() const noexcept { return n_; }
来源：http://qrq.fzhhl.top

[S53] C++：移动语义
来源：http://kvr.pycfn.com

std::vector<int> w = std::move(v);
来源：http://naa.hysaishi.cn

[S54] C++：异常处理
来源：http://axf.wangshuangyany.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ibi.shuidangran.top

[S55] C++：结构化绑定
来源：http://mde.zhixingplan.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ahh.andypj.xyz

[S56] C++：optional
来源：http://kaw.quarkkingdee.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hfn.birdmap.top

[S57] C++：编译期常量
来源：http://rcs.fengsongda.top

constexpr int N = 10;
来源：http://prq.vqdsnc.cn

[S58] C++：命名空间
来源：http://ake.gogol.net.cn

namespace ns { int f() { return 1; } }
来源：http://ytu.zhixingplan.top

[S59] C++：静态断言
来源：http://eny.hfpthk.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jga.aibaodan.cn

[S60] C++：遍历并删除元素
来源：http://vmv.yanxiufei.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hse.zycfv.cn

================================================================================
来源：http://vrj.tanke756.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yrx.316326.xyz

================================================================================
来源：http://zem.ydzc1.top

[T01] Kotlin：Hello World
来源：http://qsf.shuidangran.top

println("Hello")
来源：http://vkk.tianlin.xyz

[T02] Kotlin：变量
来源：http://xzi.316326.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zgc.dashuyun.cn

[T03] Kotlin：字符串模板
来源：http://ivk.wangdashe.top

"值: $b"
来源：http://zfg.aibaodan.cn

[T04] Kotlin：空安全
来源：http://grw.yfazqb.com

val n: String? = null;  n?.length
来源：http://wjp.gotoacloud.top

[T05] Kotlin：when 表达式
来源：http://ybi.dianchejie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vbm.zdbjq.cn

[T06] Kotlin：集合映射
来源：http://dbi.guowangkeji.top

listOf(1, 2, 3).map { it * 2 }
来源：http://gsv.zhoulong.xyz

[T07] Kotlin：集合过滤
来源：http://zsw.kuanghao11.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://yef.daxiang520.top

[T08] Kotlin：数据类
来源：http://cxh.pengpengdd.cyou

data class User(val name: String, val age: Int)
来源：http://zbj.uphjek.com

[T09] Kotlin：扩展函数
来源：http://ewv.yj20258.top

fun String.exclaim() = this + "!"
来源：http://wxj.yuanzhike.top

[T10] Kotlin：默认参数
来源：http://tie.cdnleiting.top

fun greet(name: String = "World") = "Hi $name"
来源：http://huu.zdqjudy.top

[T11] Kotlin：协程
来源：http://dqm.yfazqb.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://ekl.aizwys.cn

[T12] Kotlin：解构声明
来源：http://mfx.xinyue.icu

val (a, b) = Pair(1, 2)
来源：http://wup.shanyushiyangtech.top

[T13] Kotlin：只读 Map
来源：http://jbt.c1oappe.top

val m = mapOf("a" to 1)
来源：http://rim.nanxuanxn.top

[T14] Kotlin：循环
来源：http://wfa.pycfn.com

for (i in 1..10) println(i)
来源：http://aft.jinqigufen.top

[T15] Kotlin：接口
来源：http://wyh.haohaochexian.top

interface Shape { fun area(): Double }
来源：http://nvo.nanxinkj.top

[T16] Swift：Hello World
来源：http://efc.sysykeji.top

print("Hello")
来源：http://yao.iojbl.cn

[T17] Swift：变量与常量
来源：http://yql.yj20258.top

var a = 1;  let b = 2
来源：http://owc.wangshuangyany.cn

[T18] Swift：字符串插值
来源：http://fxi.snrcjt.cn

"值: \(b)"
来源：http://woa.cashguo.top

[T19] Swift：可选绑定
来源：http://txe.sxryk.cn

if let n = opt { print(n) }
来源：http://moy.yuxming.cn

[T20] Swift：数组操作
来源：http://wnh.pycfn.com

var a = [1, 2, 3];  a.append(4)
来源：http://ibw.guowangkeji.top

[T21] Swift：遍历
来源：http://hdi.cheryme.top

for x in a { print(x) }
来源：http://msz.svipenyu.cn

[T22] Swift：字典
来源：http://qly.fktsv.cn

var d = ["a": 1];  d["b"] = 2
来源：http://shp.shanyushiyangtech.top

[T23] Swift：函数
来源：http://oog.zhijiandao.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nbi.dashuyun.cn

[T24] Swift：闭包
来源：http://xxq.shanyushiyangtech.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://aib.zhoulong.xyz

[T25] Swift：结构体
来源：http://hbc.svipenyu.cn

struct P { var x: Int }
来源：http://xfp.shanyushiyangtech.top

[T26] Swift：类与重写
来源：http://tic.chenlongwang.top

class A: Base { override func f() {} }
来源：http://awa.hammf.cn

[T27] Swift：错误处理
来源：http://upu.pengpengdd.cyou

do { try f() } catch { print(error) }
来源：http://thq.zhixingplan.top

[T28] Swift：枚举
来源：http://fek.bbcook.cn

enum Color { case red, green }
来源：http://zvf.sxryk.cn

[T29] Swift：guard 提前返回
来源：http://hfn.iojbl.cn

guard let x = opt else { return }
来源：http://cbk.smart0.xyz

[T30] Swift：协议
来源：http://gyv.zdbjq.cn

protocol Shape { func area() -> Double }
来源：http://gdn.yuxming.cn

[T31] Lua：Hello World
来源：http://ius.zhaomingkeji.xyz

print("Hello")
来源：http://kna.haohaochexian.top

[T32] Lua：局部变量
来源：http://mwr.xinyue.icu

local a = 1
来源：http://jgj.yj20258888.top

[T33] Lua：表（数组）
来源：http://rze.shuidangran.top

local t = {1, 2, 3};  t[4] = 4
来源：http://tps.zhoulong.xyz

[T34] Lua：遍历表
来源：http://krg.yj20258.top

for i, v in ipairs(t) do print(i, v) end
来源：http://zwa.tarul.cn

[T35] Lua：字典表
来源：http://ejd.ehwqpu.com

local d = { a = 1 };  d.b = 2
来源：http://utb.vehdjk.com

[T36] Lua：函数
来源：http://hzr.smart0.xyz

function add(a, b) return a + b end
来源：http://kgj.shanyushiyangtech.top

[T37] Lua：字符串拼接
来源：http://lmd.fanxiaobao.xyz

"a" .. "b"
来源：http://yja.hongshengwenyu.top

[T38] Lua：条件
来源：http://kcd.cashguo.top

if x > 0 then print("正") end
来源：http://rqm.ctjpmb.com


<!-- 参考信息 -->