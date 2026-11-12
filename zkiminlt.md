代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://pcx.epnwcf.com

[R36] 并发执行多个任务
来源：http://igl.jianghu66.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://iri.zhongyouzk.top

[R37] 把输出赋给变量
来源：http://fme.nwbrower.top

files=$(ls -1)
来源：http://pms.havefunace.top

[R38] 管道串联
来源：http://xtu.cashguo.top

cat a.txt | grep -i error | wc -l
来源：http://bta.yj20258.top

[R39] 重定向标准输出与错误
来源：http://mur.ybcxt.top

cmd > out.log 2>&1
来源：http://ard.yvedp.cn

[R40] 追加写日志
来源：http://fqr.yfazqb.com

echo "log" >> out.log
来源：http://qbk.52xcode.cn

[R41] 丢弃输出
来源：http://osj.hongshengwenyu.top

cmd >/dev/null 2>&1
来源：http://zxr.tianlin.xyz

[R42] 输入重定向
来源：http://zuh.sweek.top

wc -l < a.txt
来源：http://aiy.redwolf501.top

[R43] 按名字查找文件
来源：http://ilz.pycfn.com

find . -name "*.log" -type f
来源：http://dhy.xziqi.cn

[R44] 按修改时间查找
来源：http://vrb.smart0.xyz

find . -mtime -7 -type f
来源：http://dfj.sweek.top

[R45] 批量删除
来源：http://mpe.jinghuilouyu.cn

find . -name "*.tmp" -delete
来源：http://rfn.hnqzz.top

[R46] 递归替换文件内容
来源：http://ufb.yj202588.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ntj.wangshuangyany.cn

[R47] sed 单行替换
来源：http://mac.redwolf501.top

sed -i 's/foo/bar/g' a.txt
来源：http://zpx.jqgufenzy.top

[R48] awk 取指定列
来源：http://pwx.pycfn.com

awk '{print $1, $3}' a.txt
来源：http://vas.hysaishi.cn

[R49] awk 带条件
来源：http://ihy.wangshuangyany.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tqx.cucudq.cn

[R50] awk 求和
来源：http://qxs.yj20258888.top

awk '{s += $2} END {print s}' a.txt
来源：http://wls.redwolf501.top

[R51] 排序去重取前几
来源：http://rpa.cheryme.top

sort a.txt | uniq -c | sort -rn | head
来源：http://tpv.yongpay.top

[R52] 统计行数
来源：http://qic.xziqi.cn

wc -l a.txt
来源：http://wfh.birdmap.top

[R53] 查看文件头与实时尾
来源：http://mbk.meibo888.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vqx.sjlbkw.cn

[R54] 比较两个文件
来源：http://bde.dashuyun.cn

diff a.txt b.txt
来源：http://rgb.yj20258888.top

[R55] 压缩与解压
来源：http://egy.jinyuanbaomall.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gtf.hesvh.cn

[R56] 远程拷贝
来源：http://wpj.0kj1m.cn

scp file user@host:/path/
来源：http://bpu.quarkkingdee.top

[R57] 远程执行命令
来源：http://wuj.hywenlv.cn

ssh user@host 'uptime'
来源：http://beq.aibaodan.cn

[R58] 下载文件
来源：http://gql.c1oappe.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ijc.chenlongwang.top

[R59] 发 POST JSON
来源：http://tpt.guowangkeji.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sus.sjlbkw.cn

[R60] 只看 HTTP 状态码
来源：http://qja.fehbvm.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://idd.ydjk.org.cn

[R61] 磁盘占用
来源：http://qim.havefunace.top

df -h;  du -sh *
来源：http://cqh.hywenlv.cn

[R62] 找最占空间的文件
来源：http://igz.ybcxt.top

du -ah . | sort -rh | head -10
来源：http://suf.jinghuilouyu.cn

[R63] 内存与进程
来源：http://zbg.gotoacloud.top

free -h;  ps aux | grep nginx
来源：http://pcd.tian-w.cn

[R64] 结束进程
来源：http://cta.yuxming.cn

kill -9 $(pgrep -f app.py)
来源：http://dxz.sjlbkw.cn

[R65] 查看端口占用
来源：http://mln.haohaochexian.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wlf.tianlin.xyz

[R66] 定时任务
来源：http://nto.tarul.cn

crontab -e;  crontab -l
来源：http://dwu.jqgfzy.top

[R67] 生成随机十六进制串
来源：http://yfs.gotoacloud.top

openssl rand -hex 16
来源：http://jpd.yuxming.cn

[R68] 计算文件校验值
来源：http://zwx.zycfv.cn

sha256sum a.txt;  md5sum a.txt
来源：http://bxy.yj20258.top

[R69] 生成随机密码
来源：http://vah.fktsv.cn

head -c 16 /dev/urandom | base64
来源：http://tit.chenlongwang.top

[R70] 时间戳与互转
来源：http://aug.andypj.xyz

date +%s;  date -d @1700000000
来源：http://jrp.bbcook.cn

[R71] 日期格式化
来源：http://xgd.yuanzhike.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://vfp.tian-w.cn

[R72] 等待端口就绪
来源：http://juq.hnxiangtu.top

until nc -z localhost 3306; do sleep 1; done
来源：http://wbc.shanyushiyangkeji.top

[R73] 分割大日志
来源：http://evb.shzxlz.cn

split -l 1000 big.log part_
来源：http://gte.havefunace.top

[R74] 批量重命名
来源：http://ifr.fehbvm.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://uzr.zhaomingkeji.xyz

[R75] 导出环境变量
来源：http://raf.52xcode.cn

export PATH="$HOME/bin:$PATH"
来源：http://jnk.fengsongda.top

[R76] 使用临时文件
来源：http://whq.smart0.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://btr.c1oappe.top

[R77] 读取用户输入
来源：http://qgc.zhongyouzk.top

read -rp "请输入: " ans
来源：http://xjx.cheryme.top

[R78] 交互式菜单
来源：http://ikt.andypj.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://vew.hongshengwenyu.top

[R79] 解析命令行选项
来源：http://fkd.yuanzhike.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qun.sxryk.cn

[R80] 查看脚本执行耗时
来源：http://ppi.wangdashe.top

time ./run.sh
来源：http://mzk.wangshuangyany.cn

================================================================================
来源：http://hsk.dianchejie.cn

S. C / C++ 专题
来源：http://hhz.cashguo.top

================================================================================
来源：http://fxw.shuidangran.top

[S01] C：Hello World
来源：http://tfy.zdbjq.cn

#include <stdio.h>
来源：http://rdv.ehwqpu.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://uej.jinyuanbaomall.cn

[S02] C：变量与格式化输出
来源：http://tjh.sweek.top

int a = 10; printf("%d\n", a);
来源：http://dxc.ydzc1.top

[S03] C：读入整数
来源：http://ykz.jlsjyb.cn

int x; scanf("%d", &x);
来源：http://oiq.zdqjudy.top

[S04] C：字符串复制
来源：http://adv.yj20258.top

char dst[32]; strcpy(dst, "hi");
来源：http://zho.fehbvm.com

[S05] C：字符串长度
来源：http://oii.zdbjq.cn

strlen(s)
来源：http://cbr.ybcxt.top

[S06] C：字符串比较
来源：http://avf.jinqigfzy.top

strcmp(a, b) == 0
来源：http://jxr.jlsjyb.cn

[S07] C：数组遍历求和
来源：http://tob.svipenyu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nil.xinyue.icu

[S08] C：动态内存分配与释放
来源：http://bie.shuidangran.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pfo.zhiwuduotai.top

[S09] C：结构体定义与初始化
来源：http://six.hysaishi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ict.shanyushiyangtech.top

[S10] C：指针与解引用
来源：http://bxm.yanxiufei.cn

int *p = &a;  *p = 5;
来源：http://sjq.0kj1m.cn

[S11] C：逐行读文件
来源：http://udr.ehwqpu.com

FILE *f = fopen("a.txt", "r");
来源：http://ind.kuanghao11.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ksl.jqgufenzy.top

fclose(f);
来源：http://nih.tian-w.cn

[S12] C：写文件
来源：http://otk.tian-w.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qws.havefunace.top

[S13] C：宏定义
来源：http://jeb.shzxlz.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ejv.zhiwuduotai.top

[S14] C：枚举
来源：http://zky.zhiwuduotai.top

enum Color { RED, GREEN, BLUE };
来源：http://faj.quarkkingdee.top

[S15] C：类型转换
来源：http://kof.aibaodan.cn

(double) a / b
来源：http://vim.gotoacloud.top

[S16] C：位操作置位
来源：http://olw.zhixingplan.top

x |= (1 << 3);
来源：http://ofo.zhaomingkeji.xyz

[S17] C：安全拼接字符串
来源：http://zrl.0kj1m.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wdl.ehwqpu.com

[S18] C：命令行参数
来源：http://ioj.c1oappe.top

int main(int argc, char **argv)
来源：http://kxb.sweek.top

[S19] C：快速排序
来源：http://yxc.yfazqb.com

qsort(a, n, sizeof(int), cmp);
来源：http://grz.jianghu66.top

[S20] C：二分查找
来源：http://utb.cheryme.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dvt.uphjek.com

[S21] C：字符类别判断
来源：http://lpb.hongshengwenyu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kaa.shzxlz.cn

[S22] C：字符串转数字
来源：http://hrd.gzhubu.top

atoi("42");  strtod("3.14", NULL);
来源：http://vuk.wangshuangyany.cn

[S23] C：随机数
来源：http://yzt.shanyushiyangkeji.top

srand(time(NULL));  int r = rand() % 100;
来源：http://fdl.cashguo.top

[S24] C：获取本地时间
来源：http://lnk.fengsongda.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vne.daria6918.cn

[S25] C：内存拷贝
来源：http://jzq.yuanzhike.top

memcpy(dst, src, n);
来源：http://gfy.daria6918.cn

[S26] C：内存清零
来源：http://qkx.yj20258888.top

memset(a, 0, sizeof a);
来源：http://doe.316326.xyz

[S27] C：定义常量
来源：http://gmv.shzxlz.cn

const double PI = 3.14159;
来源：http://oti.pengpengdd.cyou

[S28] C：静态变量
来源：http://jwy.guowangkeji.top

static int counter = 0;
来源：http://rzv.havefunace.top

[S29] C：变参函数
来源：http://zsu.havefunace.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tqw.shuidangran.top

[S30] C：头文件保护
来源：http://zax.uphjek.com

#ifndef X_H
来源：http://tzk.jinqigufen.top

#define X_H
来源：http://xnw.jinyuanbaomall.cn

#endif
来源：http://zub.jiagoushi.top

[S31] C++：Hello World
来源：http://hof.vehdjk.com

#include <iostream>
来源：http://wfq.shanyushiyangkeji.top

int main() { std::cout << "Hello\n"; }
来源：http://qln.ctjpmb.com

[S32] C++：字符串
来源：http://las.gzhubu.top

std::string s = "hi";  s += "!";
来源：http://ath.yj202588.top

[S33] C++：vector 增删
来源：http://vbk.sysykeji.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cjv.bjfxy.top

[S34] C++：遍历 vector
来源：http://czk.zhijiandao.cn

for (auto &x : v) { std::cout << x; }
来源：http://fol.shanyushiyangtech.top

[S35] C++：map
来源：http://rtx.shanyushiyangtech.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://biz.smart0.xyz

[S36] C++：unordered_map
来源：http://elb.shuidangran.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ujw.meibo888.top

[S37] C++：set
来源：http://cug.yj20258888.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fkb.tianlin.xyz

[S38] C++：排序
来源：http://fmq.gaohongyu789.top

std::sort(v.begin(), v.end());
来源：http://gni.sxryk.cn

[S39] C++：自定义比较器排序
来源：http://xho.daxiang520.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xbd.tarul.cn

[S40] C++：查找元素
来源：http://uoc.andypj.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rwr.zdbjq.cn

[S41] C++：类与构造函数
来源：http://nsv.chenzaomai.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://guw.ppjwa.cn

[S42] C++：继承与虚函数
来源：http://kmz.chenzaomai.com

class B : public Base { public: void f() override {} };
来源：http://pdk.sufxvd.cn

[S43] C++：智能指针
来源：http://agc.hammf.cn

auto p = std::make_unique<int>(5);
来源：http://qsi.xziqi.cn

[S44] C++：引用传参
来源：http://bol.jinqigfzy.top

void inc(int &x) { ++x; }
来源：http://khd.tanke756.top

[S45] C++：lambda
来源：http://ylq.hnxiangtu.top

auto add = [](int a, int b) { return a + b; };
来源：http://rqi.uphjek.com

[S46] C++：函数模板
来源：http://vls.ydzc1.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://esf.zhijiandao.cn

[S47] C++：结构化绑定遍历
来源：http://uha.zhaomingkeji.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fva.shzxlz.cn

[S48] C++：逐行读文件
来源：http://xpa.xinyue.icu

std::ifstream in("a.txt");  std::string line;
来源：http://wvx.hongshengwenyu.top

while (std::getline(in, line)) { }
来源：http://nzq.hcnkem.com

[S49] C++：写文件
来源：http://aed.vqdsnc.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kof.yangfankeji.com

[S50] C++：格式化数字
来源：http://uzz.jyoumei.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bhx.vqdsnc.cn

[S51] C++：显式类型转换
来源：http://ucg.dianchejie.cn

static_cast<double>(a) / b
来源：http://ghl.fktsv.cn

[S52] C++：const 与 noexcept
来源：http://bod.ehwqpu.com

int size() const noexcept { return n_; }
来源：http://xjt.andypj.xyz

[S53] C++：移动语义
来源：http://rky.ctjpmb.com

std::vector<int> w = std::move(v);
来源：http://zds.chenjidiqi.icu

[S54] C++：异常处理
来源：http://dzf.hammf.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hzb.gaohongyu789.top

[S55] C++：结构化绑定
来源：http://wij.tanke756.top

auto [a, b] = std::make_pair(1, 2);
来源：http://aan.yvedp.cn

[S56] C++：optional
来源：http://brq.tarul.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zpw.andypj.xyz

[S57] C++：编译期常量
来源：http://cgl.feifeiyinyue.top

constexpr int N = 10;
来源：http://cqc.xinyue.icu

[S58] C++：命名空间
来源：http://vig.shanyushiyangkeji.top

namespace ns { int f() { return 1; } }
来源：http://uqo.yonumen.top

[S59] C++：静态断言
来源：http://xvr.ehwqpu.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fta.zhengqikj.top

[S60] C++：遍历并删除元素
来源：http://pus.nanxuanxn.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gds.redwolf501.top

================================================================================
来源：http://vls.yueranfly.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xhl.ctjpmb.com

================================================================================
来源：http://acg.meibo888.top

[T01] Kotlin：Hello World
来源：http://inb.snrcjt.cn

println("Hello")
来源：http://hof.ywan-chungtsiang.top

[T02] Kotlin：变量
来源：http://ssu.sjlbkw.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sty.0kj1m.cn

[T03] Kotlin：字符串模板
来源：http://siu.fzhhl.top

"值: $b"
来源：http://rhw.ehwqpu.com

[T04] Kotlin：空安全
来源：http://ofi.daria6918.cn

val n: String? = null;  n?.length
来源：http://ytl.ybcxt.top

[T05] Kotlin：when 表达式
来源：http://hsx.9152youxi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dzk.jlsjyb.cn

[T06] Kotlin：集合映射
来源：http://ooo.fehbvm.com

listOf(1, 2, 3).map { it * 2 }
来源：http://isd.hfpthk.cn

[T07] Kotlin：集合过滤
来源：http://cse.shangyingyoupin.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ktl.hnxiangtu.top

[T08] Kotlin：数据类
来源：http://jbv.zhongyouzk.top

data class User(val name: String, val age: Int)
来源：http://rqc.zhengqikj.top

[T09] Kotlin：扩展函数
来源：http://pnh.fanxiaobao.xyz

fun String.exclaim() = this + "!"
来源：http://oet.zhongyouzk.top

[T10] Kotlin：默认参数
来源：http://ogj.sxryk.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ecz.havefunace.top

[T11] Kotlin：协程
来源：http://ipn.haohaochexian.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://jou.shanyushiyangtech.top

[T12] Kotlin：解构声明
来源：http://ruo.zdbjq.cn

val (a, b) = Pair(1, 2)
来源：http://gwy.jiagoushi.top

[T13] Kotlin：只读 Map
来源：http://bhq.ybcxt.top

val m = mapOf("a" to 1)
来源：http://irc.meibo888.top

[T14] Kotlin：循环
来源：http://wxs.chenjidiqi.icu

for (i in 1..10) println(i)
来源：http://nhm.iojbl.cn

[T15] Kotlin：接口
来源：http://znm.chenzaomai.com

interface Shape { fun area(): Double }
来源：http://tmx.jiagoushi.top

[T16] Swift：Hello World
来源：http://wyu.fzhhl.top

print("Hello")
来源：http://ovm.yangfankeji.com

[T17] Swift：变量与常量
来源：http://roa.hammf.cn

var a = 1;  let b = 2
来源：http://hqh.fzhhl.top

[T18] Swift：字符串插值
来源：http://qex.fanxiaobao.xyz

"值: \(b)"
来源：http://qtn.ybcxt.top

[T19] Swift：可选绑定
来源：http://wfq.sjlbkw.cn

if let n = opt { print(n) }
来源：http://dtm.dianchejie.cn

[T20] Swift：数组操作
来源：http://dzy.hnxiangtu.top

var a = [1, 2, 3];  a.append(4)
来源：http://pql.tianlin.xyz

[T21] Swift：遍历
来源：http://csb.shangyingyoupin.top

for x in a { print(x) }
来源：http://ydn.guowangkeji.top

[T22] Swift：字典
来源：http://qtx.vehdjk.com

var d = ["a": 1];  d["b"] = 2
来源：http://qdx.andypj.xyz

[T23] Swift：函数
来源：http://tvy.iojbl.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://phe.nanxinkj.top

[T24] Swift：闭包
来源：http://pis.yfazqb.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://mfw.jlsjyb.cn

[T25] Swift：结构体
来源：http://djm.cashguo.top

struct P { var x: Int }
来源：http://hnd.vqdsnc.cn

[T26] Swift：类与重写
来源：http://ber.fzhhl.top

class A: Base { override func f() {} }
来源：http://zur.gotoacloud.top

[T27] Swift：错误处理
来源：http://nwj.jqgufenzy.top

do { try f() } catch { print(error) }
来源：http://dct.mhx1999.top

[T28] Swift：枚举
来源：http://qbb.9152youxi.cn

enum Color { case red, green }
来源：http://nxm.jqgufenzy.top

[T29] Swift：guard 提前返回
来源：http://fyh.yanxiufei.cn

guard let x = opt else { return }
来源：http://pks.shuidangran.top

[T30] Swift：协议
来源：http://ikd.zdqjudy.top

protocol Shape { func area() -> Double }
来源：http://vuh.cheryme.top

[T31] Lua：Hello World
来源：http://xxu.yvedp.cn

print("Hello")
来源：http://iel.shanyushiyangtech.top

[T32] Lua：局部变量
来源：http://rdu.yuxming.cn

local a = 1
来源：http://ahm.dashuyun.cn

[T33] Lua：表（数组）
来源：http://ifj.pycfn.com

local t = {1, 2, 3};  t[4] = 4
来源：http://sbw.yvedp.cn

[T34] Lua：遍历表
来源：http://qii.hnxiangtu.top

for i, v in ipairs(t) do print(i, v) end
来源：http://eap.xuetiantiany.cn

[T35] Lua：字典表
来源：http://sbp.c1oappe.top

local d = { a = 1 };  d.b = 2
来源：http://atl.zhixingplan.top

[T36] Lua：函数
来源：http://ugc.jianghu66.top

function add(a, b) return a + b end
来源：http://jnh.shangyingyoupin.top

[T37] Lua：字符串拼接
来源：http://dih.pengpengdd.cyou

"a" .. "b"
来源：http://bya.cucudq.cn

[T38] Lua：条件
来源：http://zsv.chenjidiqi.icu

if x > 0 then print("正") end
来源：http://kdi.shzxlz.cn


<!-- 参考信息 -->