代发 wailian999

files=$(ls -1)
来源：http://sbe.jqgufenzy.top

[R38] 管道串联
来源：http://oey.fehbvm.com

cat a.txt | grep -i error | wc -l
来源：http://bgq.hfpthk.cn

[R39] 重定向标准输出与错误
来源：http://gse.birdmap.top

cmd > out.log 2>&1
来源：http://vdc.pycfn.com

[R40] 追加写日志
来源：http://ico.daxiang520.top

echo "log" >> out.log
来源：http://erg.tianlin.xyz

[R41] 丢弃输出
来源：http://lbx.nanxuanxn.top

cmd >/dev/null 2>&1
来源：http://iaj.sufxvd.cn

[R42] 输入重定向
来源：http://wlq.ywan-chungtsiang.top

wc -l < a.txt
来源：http://vjv.316326.xyz

[R43] 按名字查找文件
来源：http://ltn.jinqigfzy.top

find . -name "*.log" -type f
来源：http://ytj.daria6918.cn

[R44] 按修改时间查找
来源：http://yuk.xuetiantiany.cn

find . -mtime -7 -type f
来源：http://gox.gotoacloud.top

[R45] 批量删除
来源：http://qpu.kuanghao11.cn

find . -name "*.tmp" -delete
来源：http://uie.wangdashe.top

[R46] 递归替换文件内容
来源：http://ijl.cashguo.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fou.daria6918.cn

[R47] sed 单行替换
来源：http://nyi.jqgufenzy.top

sed -i 's/foo/bar/g' a.txt
来源：http://uvt.gzhubu.top

[R48] awk 取指定列
来源：http://ixm.zycfv.cn

awk '{print $1, $3}' a.txt
来源：http://amq.ivvv.top

[R49] awk 带条件
来源：http://wdi.zdbjq.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vjp.havefunace.top

[R50] awk 求和
来源：http://ojs.zhijiandao.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yqk.zycfv.cn

[R51] 排序去重取前几
来源：http://nmm.dianchejie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://wvr.jianghu66.top

[R52] 统计行数
来源：http://rkn.hnxiangtu.top

wc -l a.txt
来源：http://qnc.gogol.net.cn

[R53] 查看文件头与实时尾
来源：http://yfx.guannengcc.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cyz.hcnkem.com

[R54] 比较两个文件
来源：http://dyr.fehbvm.com

diff a.txt b.txt
来源：http://fmb.yueranfly.top

[R55] 压缩与解压
来源：http://tbx.hongshengwenyu.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mcg.yuxming.cn

[R56] 远程拷贝
来源：http://luf.shangyingyoupin.top

scp file user@host:/path/
来源：http://ati.sjlbkw.cn

[R57] 远程执行命令
来源：http://ybq.tianlin.xyz

ssh user@host 'uptime'
来源：http://qhg.jinghuilouyu.cn

[R58] 下载文件
来源：http://vbl.sysykeji.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kgn.vqdsnc.cn

[R59] 发 POST JSON
来源：http://dzg.aizwys.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://izf.meibo888.top

[R60] 只看 HTTP 状态码
来源：http://tjw.zhongyouzk.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mlc.jlsjyb.cn

[R61] 磁盘占用
来源：http://bpv.yangfankeji.com

df -h;  du -sh *
来源：http://ngo.c1oappe.top

[R62] 找最占空间的文件
来源：http://wbc.gotoacloud.top

du -ah . | sort -rh | head -10
来源：http://pkf.9152youxi.cn

[R63] 内存与进程
来源：http://dpg.fzhhl.top

free -h;  ps aux | grep nginx
来源：http://eea.hysaishi.cn

[R64] 结束进程
来源：http://ths.zycfv.cn

kill -9 $(pgrep -f app.py)
来源：http://vnz.fehbvm.com

[R65] 查看端口占用
来源：http://eqo.iojbl.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gcn.gaohongyu789.top

[R66] 定时任务
来源：http://reb.snrcjt.cn

crontab -e;  crontab -l
来源：http://xkh.jinqigufen.top

[R67] 生成随机十六进制串
来源：http://fiq.shzxlz.cn

openssl rand -hex 16
来源：http://exc.wangshuangyany.cn

[R68] 计算文件校验值
来源：http://hth.316326.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://qik.jqgufenzy.top

[R69] 生成随机密码
来源：http://lrz.vqdsnc.cn

head -c 16 /dev/urandom | base64
来源：http://fdg.cucudq.cn

[R70] 时间戳与互转
来源：http://mtg.feifeiyinyue.top

date +%s;  date -d @1700000000
来源：http://bzn.svipenyu.cn

[R71] 日期格式化
来源：http://kxr.ydjk.org.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ztp.fehbvm.com

[R72] 等待端口就绪
来源：http://ywd.zycfv.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qle.hysaishi.cn

[R73] 分割大日志
来源：http://ncl.pycfn.com

split -l 1000 big.log part_
来源：http://jap.ydzc1.top

[R74] 批量重命名
来源：http://bty.quarkkingdee.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jkg.jiagoushi.top

[R75] 导出环境变量
来源：http://cnt.wangdashe.top

export PATH="$HOME/bin:$PATH"
来源：http://vyg.wangdashe.top

[R76] 使用临时文件
来源：http://gtx.fanxiaobao.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zfo.aibaodan.cn

[R77] 读取用户输入
来源：http://jyq.ybcxt.top

read -rp "请输入: " ans
来源：http://aay.nanxinkj.top

[R78] 交互式菜单
来源：http://fhe.jlsjyb.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://iif.yonumen.top

[R79] 解析命令行选项
来源：http://kck.yj20258888.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fpk.sufxvd.cn

[R80] 查看脚本执行耗时
来源：http://edh.ctjpmb.com

time ./run.sh
来源：http://dzn.yj20258888.top

================================================================================
来源：http://diw.ydzc1.top

S. C / C++ 专题
来源：http://gcd.hywenlv.cn

================================================================================
来源：http://zqs.shzxlz.cn

[S01] C：Hello World
来源：http://bam.zhiwuduotai.top

#include <stdio.h>
来源：http://ouy.guannengcc.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ajd.xuetiantiany.cn

[S02] C：变量与格式化输出
来源：http://fcf.zhaomingkeji.xyz

int a = 10; printf("%d\n", a);
来源：http://zkp.zhaomingkeji.xyz

[S03] C：读入整数
来源：http://erm.ydjk.org.cn

int x; scanf("%d", &x);
来源：http://dic.jinqigfzy.top

[S04] C：字符串复制
来源：http://yai.hnxiangtu.top

char dst[32]; strcpy(dst, "hi");
来源：http://end.zhongyouzk.top

[S05] C：字符串长度
来源：http://gbo.epnwcf.com

strlen(s)
来源：http://lic.jqgfzy.top

[S06] C：字符串比较
来源：http://jgc.smart0.xyz

strcmp(a, b) == 0
来源：http://njz.zhaomingkeji.xyz

[S07] C：数组遍历求和
来源：http://jrf.zhijiandao.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ary.ybcxt.top

[S08] C：动态内存分配与释放
来源：http://tyr.yvedp.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ols.bjfxy.top

[S09] C：结构体定义与初始化
来源：http://ydv.sufxvd.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zke.aibaodan.cn

[S10] C：指针与解引用
来源：http://hkh.ehwqpu.com

int *p = &a;  *p = 5;
来源：http://pyj.zycfv.cn

[S11] C：逐行读文件
来源：http://zuu.shzxlz.cn

FILE *f = fopen("a.txt", "r");
来源：http://rko.haohaochexian.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://yjh.birdmap.top

fclose(f);
来源：http://izh.tianlin.xyz

[S12] C：写文件
来源：http://dst.316326.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://upc.tanke756.top

[S13] C：宏定义
来源：http://zth.jlsjyb.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pzj.yuxming.cn

[S14] C：枚举
来源：http://fie.9152youxi.cn

enum Color { RED, GREEN, BLUE };
来源：http://kvf.yueranfly.top

[S15] C：类型转换
来源：http://fbg.ybcxt.top

(double) a / b
来源：http://xui.zhiwuduotai.top

[S16] C：位操作置位
来源：http://ewv.epnwcf.com

x |= (1 << 3);
来源：http://dwr.sufxvd.cn

[S17] C：安全拼接字符串
来源：http://ina.jlsjyb.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hcr.sweek.top

[S18] C：命令行参数
来源：http://skp.xuetiantiany.cn

int main(int argc, char **argv)
来源：http://gll.jianghu66.top

[S19] C：快速排序
来源：http://pir.fanxiaobao.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://jdq.cashguo.top

[S20] C：二分查找
来源：http://qyt.epnwcf.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qtw.zycfv.cn

[S21] C：字符类别判断
来源：http://iax.hcnkem.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://waj.52xcode.cn

[S22] C：字符串转数字
来源：http://yaa.zhongyouzk.top

atoi("42");  strtod("3.14", NULL);
来源：http://xfm.tarul.cn

[S23] C：随机数
来源：http://puf.cashguo.top

srand(time(NULL));  int r = rand() % 100;
来源：http://brj.vehdjk.com

[S24] C：获取本地时间
来源：http://qki.ehwqpu.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xvt.hammf.cn

[S25] C：内存拷贝
来源：http://ryq.fanxiaobao.xyz

memcpy(dst, src, n);
来源：http://cen.gogol.net.cn

[S26] C：内存清零
来源：http://lpp.kuanghao11.cn

memset(a, 0, sizeof a);
来源：http://fgm.hcnkem.com

[S27] C：定义常量
来源：http://xiq.ivvv.top

const double PI = 3.14159;
来源：http://rtq.jinqigufen.top

[S28] C：静态变量
来源：http://red.wangshuangyany.cn

static int counter = 0;
来源：http://jfo.c1oappe.top

[S29] C：变参函数
来源：http://hge.hnqzz.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sip.ppjwa.cn

[S30] C：头文件保护
来源：http://hco.9152youxi.cn

#ifndef X_H
来源：http://qpw.jqgufenzy.top

#define X_H
来源：http://bas.c1oappe.top

#endif
来源：http://kok.hysaishi.cn

[S31] C++：Hello World
来源：http://jsg.gogol.net.cn

#include <iostream>
来源：http://egp.jqgufenzy.top

int main() { std::cout << "Hello\n"; }
来源：http://aoo.cucudq.cn

[S32] C++：字符串
来源：http://shh.yvedp.cn

std::string s = "hi";  s += "!";
来源：http://dju.jqgfzy.top

[S33] C++：vector 增删
来源：http://ygk.daria6918.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bwi.gzhubu.top

[S34] C++：遍历 vector
来源：http://ufk.xylfe.cn

for (auto &x : v) { std::cout << x; }
来源：http://gbo.xingfuxueyuan.xyz

[S35] C++：map
来源：http://qsy.hongshengwenyu.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wvg.xingfuxueyuan.xyz

[S36] C++：unordered_map
来源：http://mhp.ydjk.org.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://juu.hysaishi.cn

[S37] C++：set
来源：http://hzf.yonumen.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sqc.yj20258888.top

[S38] C++：排序
来源：http://kax.guannengcc.top

std::sort(v.begin(), v.end());
来源：http://yyz.ydjk.org.cn

[S39] C++：自定义比较器排序
来源：http://sqp.c1oappe.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bko.yj20258888.top

[S40] C++：查找元素
来源：http://jmd.hcnkem.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bup.tarul.cn

[S41] C++：类与构造函数
来源：http://bkv.quarkkingdee.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ows.fktsv.cn

[S42] C++：继承与虚函数
来源：http://wuk.hammf.cn

class B : public Base { public: void f() override {} };
来源：http://mac.ctjpmb.com

[S43] C++：智能指针
来源：http://rcx.jinyuanbaomall.cn

auto p = std::make_unique<int>(5);
来源：http://isw.cashguo.top

[S44] C++：引用传参
来源：http://mws.yanxiufei.cn

void inc(int &x) { ++x; }
来源：http://nxj.hongshengwenyu.top

[S45] C++：lambda
来源：http://ics.dashuyun.cn

auto add = [](int a, int b) { return a + b; };
来源：http://umw.ywan-chungtsiang.top

[S46] C++：函数模板
来源：http://tfu.andypj.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mla.cashguo.top

[S47] C++：结构化绑定遍历
来源：http://wfn.yongpay.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dbp.sufxvd.cn

[S48] C++：逐行读文件
来源：http://mcc.0kj1m.cn

std::ifstream in("a.txt");  std::string line;
来源：http://nbf.nwbrower.top

while (std::getline(in, line)) { }
来源：http://yio.shangyingyoupin.top

[S49] C++：写文件
来源：http://rhq.fehbvm.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yuz.cucudq.cn

[S50] C++：格式化数字
来源：http://ihp.aibaodan.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ucu.xingfuxueyuan.xyz

[S51] C++：显式类型转换
来源：http://ens.mhx1999.top

static_cast<double>(a) / b
来源：http://vsk.gaohongyu789.top

[S52] C++：const 与 noexcept
来源：http://vlf.fengsongda.top

int size() const noexcept { return n_; }
来源：http://bxc.sxryk.cn

[S53] C++：移动语义
来源：http://noc.yj20258888.top

std::vector<int> w = std::move(v);
来源：http://cvc.zycfv.cn

[S54] C++：异常处理
来源：http://amz.jinghuilouyu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ifo.hammf.cn

[S55] C++：结构化绑定
来源：http://ksk.fanxiaobao.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://una.iojbl.cn

[S56] C++：optional
来源：http://kwa.jqgufenzy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lwj.ydjk.org.cn

[S57] C++：编译期常量
来源：http://ewt.zhengqikj.top

constexpr int N = 10;
来源：http://qqe.yuanzhike.top

[S58] C++：命名空间
来源：http://ovp.ctjpmb.com

namespace ns { int f() { return 1; } }
来源：http://bst.nwbrower.top

[S59] C++：静态断言
来源：http://lma.jinqigfzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rot.jlsjyb.cn

[S60] C++：遍历并删除元素
来源：http://sba.pengpengdd.cyou

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sfm.yfazqb.com

================================================================================
来源：http://flf.aibaodan.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://sxr.ybcxt.top

================================================================================
来源：http://ppf.yj20258.top

[T01] Kotlin：Hello World
来源：http://jqn.yfazqb.com

println("Hello")
来源：http://fdp.meibo888.top

[T02] Kotlin：变量
来源：http://nta.birdmap.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ykh.nanxuanxn.top

[T03] Kotlin：字符串模板
来源：http://ovv.xuanzx.com

"值: $b"
来源：http://knk.hfpthk.cn

[T04] Kotlin：空安全
来源：http://wki.jinqigufen.top

val n: String? = null;  n?.length
来源：http://jiq.andypj.xyz

[T05] Kotlin：when 表达式
来源：http://xce.wangshuangyany.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xor.yanxiufei.cn

[T06] Kotlin：集合映射
来源：http://plu.pengpengdd.cyou

listOf(1, 2, 3).map { it * 2 }
来源：http://hch.jinyuanbaomall.cn

[T07] Kotlin：集合过滤
来源：http://ujf.yongpay.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://gvc.xuanzx.com

[T08] Kotlin：数据类
来源：http://pmp.yonumen.top

data class User(val name: String, val age: Int)
来源：http://ahu.cheryme.top

[T09] Kotlin：扩展函数
来源：http://ltt.hywenlv.cn

fun String.exclaim() = this + "!"
来源：http://ddf.yj202588.top

[T10] Kotlin：默认参数
来源：http://ftw.sxryk.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://crf.yj20258.top

[T11] Kotlin：协程
来源：http://fvv.tianlin.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://ieq.wangdashe.top

[T12] Kotlin：解构声明
来源：http://vgy.jinqigfzy.top

val (a, b) = Pair(1, 2)
来源：http://vcd.snrcjt.cn

[T13] Kotlin：只读 Map
来源：http://yrf.havefunace.top

val m = mapOf("a" to 1)
来源：http://wim.hammf.cn

[T14] Kotlin：循环
来源：http://exv.feifeiyinyue.top

for (i in 1..10) println(i)
来源：http://ism.zdbjq.cn

[T15] Kotlin：接口
来源：http://xuq.52xcode.cn

interface Shape { fun area(): Double }
来源：http://dyr.snrcjt.cn

[T16] Swift：Hello World
来源：http://cjg.dashuyun.cn

print("Hello")
来源：http://zjn.aizwys.cn

[T17] Swift：变量与常量
来源：http://qtw.quarkkingdee.top

var a = 1;  let b = 2
来源：http://bam.hywenlv.cn

[T18] Swift：字符串插值
来源：http://oht.vqdsnc.cn

"值: \(b)"
来源：http://syw.andypj.xyz

[T19] Swift：可选绑定
来源：http://uaw.shanyushiyangkeji.top

if let n = opt { print(n) }
来源：http://oaf.yfazqb.com

[T20] Swift：数组操作
来源：http://age.xziqi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://pci.jlsjyb.cn

[T21] Swift：遍历
来源：http://dsi.zycfv.cn

for x in a { print(x) }
来源：http://jwe.zhengqikj.top

[T22] Swift：字典
来源：http://jap.cashguo.top

var d = ["a": 1];  d["b"] = 2
来源：http://knm.jinqigufen.top

[T23] Swift：函数
来源：http://nfr.aibaodan.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ycs.ppjwa.cn

[T24] Swift：闭包
来源：http://mfa.cqqwz.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://mof.ehwqpu.com

[T25] Swift：结构体
来源：http://ily.nanxinkj.top

struct P { var x: Int }
来源：http://dvw.ywan-chungtsiang.top

[T26] Swift：类与重写
来源：http://euc.guannengcc.top

class A: Base { override func f() {} }
来源：http://gip.smart0.xyz

[T27] Swift：错误处理
来源：http://cxz.tarul.cn

do { try f() } catch { print(error) }
来源：http://jvv.guannengcc.top

[T28] Swift：枚举
来源：http://oyy.sxryk.cn

enum Color { case red, green }
来源：http://rgz.xingfuxueyuan.xyz

[T29] Swift：guard 提前返回
来源：http://ehb.jlsjyb.cn

guard let x = opt else { return }
来源：http://lkx.epnwcf.com

[T30] Swift：协议
来源：http://efd.zhongyouzk.top

protocol Shape { func area() -> Double }
来源：http://xjq.yongpay.top

[T31] Lua：Hello World
来源：http://lam.havefunace.top

print("Hello")
来源：http://xmt.guannengcc.top

[T32] Lua：局部变量
来源：http://hqz.jlsjyb.cn

local a = 1
来源：http://dbz.aibaodan.cn

[T33] Lua：表（数组）
来源：http://jfh.guowangkeji.top

local t = {1, 2, 3};  t[4] = 4
来源：http://dzg.vehdjk.com

[T34] Lua：遍历表
来源：http://pdv.pengpengdd.cyou

for i, v in ipairs(t) do print(i, v) end
来源：http://qfy.iojbl.cn

[T35] Lua：字典表
来源：http://okg.0kj1m.cn

local d = { a = 1 };  d.b = 2
来源：http://vua.yfazqb.com

[T36] Lua：函数
来源：http://met.52xcode.cn

function add(a, b) return a + b end
来源：http://jbf.chenlongwang.top

[T37] Lua：字符串拼接
来源：http://hje.tarul.cn

"a" .. "b"
来源：http://cwl.gzhubu.top

[T38] Lua：条件
来源：http://pyz.gogol.net.cn

if x > 0 then print("正") end
来源：http://nzt.chenjidiqi.icu

[T39] Lua：模式匹配
来源：http://lal.epnwcf.com

string.find(s, "%d+")
来源：http://hut.jinghuilouyu.cn

[T40] Lua：元表
来源：http://hqp.yuxming.cn

setmetatable({}, { __index = base })
来源：http://rja.yj20258888.top


<!-- 参考信息 -->