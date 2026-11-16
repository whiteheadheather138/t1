代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://ivg.jqgfzy.top

[R36] 并发执行多个任务
来源：http://ows.guowangkeji.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rot.yanxiufei.cn

[R37] 把输出赋给变量
来源：http://yfp.jinghuilouyu.cn

files=$(ls -1)
来源：http://jat.tarul.cn

[R38] 管道串联
来源：http://fbw.chenjidiqi.icu

cat a.txt | grep -i error | wc -l
来源：http://zvo.sufxvd.cn

[R39] 重定向标准输出与错误
来源：http://qgh.c1oappe.top

cmd > out.log 2>&1
来源：http://mjj.hongshengwenyu.top

[R40] 追加写日志
来源：http://mte.iojbl.cn

echo "log" >> out.log
来源：http://dtg.zhiwuduotai.top

[R41] 丢弃输出
来源：http://yah.xuetiantiany.cn

cmd >/dev/null 2>&1
来源：http://klf.ctjpmb.com

[R42] 输入重定向
来源：http://szk.havefunace.top

wc -l < a.txt
来源：http://eli.cheryme.top

[R43] 按名字查找文件
来源：http://lqv.cheryme.top

find . -name "*.log" -type f
来源：http://wee.epnwcf.com

[R44] 按修改时间查找
来源：http://ukh.pengpengdd.cyou

find . -mtime -7 -type f
来源：http://hcc.hongshengwenyu.top

[R45] 批量删除
来源：http://btv.hnxiangtu.top

find . -name "*.tmp" -delete
来源：http://hja.aibaodan.cn

[R46] 递归替换文件内容
来源：http://bzk.kuanghao11.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hat.316326.xyz

[R47] sed 单行替换
来源：http://oqp.sufxvd.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vxy.yonumen.top

[R48] awk 取指定列
来源：http://nqn.wangshuangyany.cn

awk '{print $1, $3}' a.txt
来源：http://mcs.hnxiangtu.top

[R49] awk 带条件
来源：http://uax.chenlongwang.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vao.ydjk.org.cn

[R50] awk 求和
来源：http://mcn.sufxvd.cn

awk '{s += $2} END {print s}' a.txt
来源：http://mnf.316326.xyz

[R51] 排序去重取前几
来源：http://qit.hfpthk.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ktu.gogol.net.cn

[R52] 统计行数
来源：http://yqt.haohaochexian.top

wc -l a.txt
来源：http://lwg.yvedp.cn

[R53] 查看文件头与实时尾
来源：http://vsq.tarul.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dvv.fanxiaobao.xyz

[R54] 比较两个文件
来源：http://jos.dashuyun.cn

diff a.txt b.txt
来源：http://znj.ppjwa.cn

[R55] 压缩与解压
来源：http://bpk.shanyushiyangkeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hzi.bbcook.cn

[R56] 远程拷贝
来源：http://gkd.yonumen.top

scp file user@host:/path/
来源：http://ooe.sjlbkw.cn

[R57] 远程执行命令
来源：http://jid.hesvh.cn

ssh user@host 'uptime'
来源：http://flq.hcnkem.com

[R58] 下载文件
来源：http://rqn.feifeiyinyue.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yjo.dianchejie.cn

[R59] 发 POST JSON
来源：http://gza.yanxiufei.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qph.iojbl.cn

[R60] 只看 HTTP 状态码
来源：http://hlw.hammf.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pct.vqdsnc.cn

[R61] 磁盘占用
来源：http://kwx.snrcjt.cn

df -h;  du -sh *
来源：http://pzv.jlsjyb.cn

[R62] 找最占空间的文件
来源：http://jog.jinqigfzy.top

du -ah . | sort -rh | head -10
来源：http://gud.gotoacloud.top

[R63] 内存与进程
来源：http://bdd.fktsv.cn

free -h;  ps aux | grep nginx
来源：http://lak.jianghu66.top

[R64] 结束进程
来源：http://guw.ybcxt.top

kill -9 $(pgrep -f app.py)
来源：http://bzr.yanxiufei.cn

[R65] 查看端口占用
来源：http://fsp.birdmap.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lth.jqgfzy.top

[R66] 定时任务
来源：http://wnh.yueranfly.top

crontab -e;  crontab -l
来源：http://dbn.fzhhl.top

[R67] 生成随机十六进制串
来源：http://yrq.gzhubu.top

openssl rand -hex 16
来源：http://dlu.nanxuanxn.top

[R68] 计算文件校验值
来源：http://hdi.fzhhl.top

sha256sum a.txt;  md5sum a.txt
来源：http://pvw.haohaochexian.top

[R69] 生成随机密码
来源：http://zqj.uphjek.com

head -c 16 /dev/urandom | base64
来源：http://lxe.daxiang520.top

[R70] 时间戳与互转
来源：http://tnn.zhengqikj.top

date +%s;  date -d @1700000000
来源：http://pwo.cucudq.cn

[R71] 日期格式化
来源：http://tni.cdnleiting.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://lba.kuanghao11.cn

[R72] 等待端口就绪
来源：http://wjn.daxiang520.top

until nc -z localhost 3306; do sleep 1; done
来源：http://vgi.gaohongyu789.top

[R73] 分割大日志
来源：http://nef.snrcjt.cn

split -l 1000 big.log part_
来源：http://kui.redwolf501.top

[R74] 批量重命名
来源：http://ptc.sweek.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://sba.xziqi.cn

[R75] 导出环境变量
来源：http://rdy.aibaodan.cn

export PATH="$HOME/bin:$PATH"
来源：http://cwp.jyoumei.cn

[R76] 使用临时文件
来源：http://zan.dianchejie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://psu.ppjwa.cn

[R77] 读取用户输入
来源：http://lyj.9152youxi.cn

read -rp "请输入: " ans
来源：http://ckh.jlsjyb.cn

[R78] 交互式菜单
来源：http://lxz.aibaodan.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://afq.dashuyun.cn

[R79] 解析命令行选项
来源：http://vwi.hfpthk.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hcc.uphjek.com

[R80] 查看脚本执行耗时
来源：http://oof.0kj1m.cn

time ./run.sh
来源：http://rbl.svipenyu.cn

================================================================================
来源：http://dbb.yuanzhike.top

S. C / C++ 专题
来源：http://nap.xinyue.icu

================================================================================
来源：http://tzq.ehwqpu.com

[S01] C：Hello World
来源：http://tcw.aibaodan.cn

#include <stdio.h>
来源：http://lgc.pengpengdd.cyou

int main(void) { printf("Hello\n"); return 0; }
来源：http://slc.hnxiangtu.top

[S02] C：变量与格式化输出
来源：http://rbn.yvedp.cn

int a = 10; printf("%d\n", a);
来源：http://voy.jqgfzy.top

[S03] C：读入整数
来源：http://ezd.c1oappe.top

int x; scanf("%d", &x);
来源：http://iah.gotoacloud.top

[S04] C：字符串复制
来源：http://hvy.zhoulong.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://mdu.316326.xyz

[S05] C：字符串长度
来源：http://xem.fanxiaobao.xyz

strlen(s)
来源：http://wor.ehwqpu.com

[S06] C：字符串比较
来源：http://bfi.hongshengwenyu.top

strcmp(a, b) == 0
来源：http://qma.zdqjudy.top

[S07] C：数组遍历求和
来源：http://rbn.yueranfly.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ado.jqgufenzy.top

[S08] C：动态内存分配与释放
来源：http://oxe.kuanghao11.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gbq.zhoulong.xyz

[S09] C：结构体定义与初始化
来源：http://ani.ydjk.org.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xnd.jinyuanbaomall.cn

[S10] C：指针与解引用
来源：http://lzn.shuidangran.top

int *p = &a;  *p = 5;
来源：http://isa.yj20258888.top

[S11] C：逐行读文件
来源：http://gbi.jqgufenzy.top

FILE *f = fopen("a.txt", "r");
来源：http://jdp.gzhubu.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://hqj.tanke756.top

fclose(f);
来源：http://ojy.zhongyouzk.top

[S12] C：写文件
来源：http://beb.cqqwz.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gpj.hesvh.cn

[S13] C：宏定义
来源：http://czi.vehdjk.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hrd.ehwqpu.com

[S14] C：枚举
来源：http://zvp.yuxming.cn

enum Color { RED, GREEN, BLUE };
来源：http://cvd.shzxlz.cn

[S15] C：类型转换
来源：http://jjw.sxryk.cn

(double) a / b
来源：http://ivw.yj202588.top

[S16] C：位操作置位
来源：http://qqw.9152youxi.cn

x |= (1 << 3);
来源：http://snq.shanyushiyangkeji.top

[S17] C：安全拼接字符串
来源：http://led.epnwcf.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ruf.guannengcc.top

[S18] C：命令行参数
来源：http://ryw.cdnleiting.top

int main(int argc, char **argv)
来源：http://vhb.gaohongyu789.top

[S19] C：快速排序
来源：http://bzb.c1oappe.top

qsort(a, n, sizeof(int), cmp);
来源：http://rpq.shzxlz.cn

[S20] C：二分查找
来源：http://lig.c1oappe.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lap.zhijiandao.cn

[S21] C：字符类别判断
来源：http://kge.meibo888.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://aeu.zhoulong.xyz

[S22] C：字符串转数字
来源：http://dmq.shanyushiyangkeji.top

atoi("42");  strtod("3.14", NULL);
来源：http://bir.tian-w.cn

[S23] C：随机数
来源：http://cum.yuxming.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hhd.guowangkeji.top

[S24] C：获取本地时间
来源：http://ozn.cashguo.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wil.jlsjyb.cn

[S25] C：内存拷贝
来源：http://rtt.jianghu66.top

memcpy(dst, src, n);
来源：http://mbw.tian-w.cn

[S26] C：内存清零
来源：http://nej.sufxvd.cn

memset(a, 0, sizeof a);
来源：http://bka.hammf.cn

[S27] C：定义常量
来源：http://xzj.shanyushiyangkeji.top

const double PI = 3.14159;
来源：http://zpa.tarul.cn

[S28] C：静态变量
来源：http://gyc.nanxuanxn.top

static int counter = 0;
来源：http://stm.pengpengdd.cyou

[S29] C：变参函数
来源：http://ufv.smart0.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vdb.ctjpmb.com

[S30] C：头文件保护
来源：http://xrn.smart0.xyz

#ifndef X_H
来源：http://ola.fzhhl.top

#define X_H
来源：http://cpn.yj202588.top

#endif
来源：http://ftq.ydjk.org.cn

[S31] C++：Hello World
来源：http://ihr.ydjk.org.cn

#include <iostream>
来源：http://doj.ppjwa.cn

int main() { std::cout << "Hello\n"; }
来源：http://bmt.hcnkem.com

[S32] C++：字符串
来源：http://nmt.nanxinkj.top

std::string s = "hi";  s += "!";
来源：http://dvc.yvedp.cn

[S33] C++：vector 增删
来源：http://enm.uphjek.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://prn.yuanzhike.top

[S34] C++：遍历 vector
来源：http://xof.snrcjt.cn

for (auto &x : v) { std::cout << x; }
来源：http://sqn.yj202588.top

[S35] C++：map
来源：http://vwj.nwbrower.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://usu.hcnkem.com

[S36] C++：unordered_map
来源：http://ejp.zdbjq.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hsf.cdnleiting.top

[S37] C++：set
来源：http://ugz.316326.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xmf.zhengqikj.top

[S38] C++：排序
来源：http://hxz.zdbjq.cn

std::sort(v.begin(), v.end());
来源：http://irh.guowangkeji.top

[S39] C++：自定义比较器排序
来源：http://gqp.vehdjk.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fez.nanxinkj.top

[S40] C++：查找元素
来源：http://ozi.xuanzx.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zoc.havefunace.top

[S41] C++：类与构造函数
来源：http://eli.gaohongyu789.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sbz.jqgufenzy.top

[S42] C++：继承与虚函数
来源：http://tlx.xuetiantiany.cn

class B : public Base { public: void f() override {} };
来源：http://umf.vehdjk.com

[S43] C++：智能指针
来源：http://cav.tianlin.xyz

auto p = std::make_unique<int>(5);
来源：http://vdj.svipenyu.cn

[S44] C++：引用传参
来源：http://mco.daxiang520.top

void inc(int &x) { ++x; }
来源：http://nbs.xylfe.cn

[S45] C++：lambda
来源：http://tnr.bjfxy.top

auto add = [](int a, int b) { return a + b; };
来源：http://oxf.tanke756.top

[S46] C++：函数模板
来源：http://uqr.shuidangran.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ekl.wangshuangyany.cn

[S47] C++：结构化绑定遍历
来源：http://kkl.aizwys.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xfe.xuetiantiany.cn

[S48] C++：逐行读文件
来源：http://wvn.bjfxy.top

std::ifstream in("a.txt");  std::string line;
来源：http://moq.sysykeji.top

while (std::getline(in, line)) { }
来源：http://eqb.shzxlz.cn

[S49] C++：写文件
来源：http://crs.hnqzz.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nuf.nanxinkj.top

[S50] C++：格式化数字
来源：http://nzl.zhoulong.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xpt.feifeiyinyue.top

[S51] C++：显式类型转换
来源：http://fze.quarkkingdee.top

static_cast<double>(a) / b
来源：http://rcy.jinqigufen.top

[S52] C++：const 与 noexcept
来源：http://wnt.yangfankeji.com

int size() const noexcept { return n_; }
来源：http://wog.jinqigfzy.top

[S53] C++：移动语义
来源：http://emq.daria6918.cn

std::vector<int> w = std::move(v);
来源：http://fmh.iojbl.cn

[S54] C++：异常处理
来源：http://blf.guowangkeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mrh.52xcode.cn

[S55] C++：结构化绑定
来源：http://fvk.epnwcf.com

auto [a, b] = std::make_pair(1, 2);
来源：http://hjx.bbcook.cn

[S56] C++：optional
来源：http://gxl.birdmap.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gvp.sufxvd.cn

[S57] C++：编译期常量
来源：http://qhd.zhoulong.xyz

constexpr int N = 10;
来源：http://aqg.smart0.xyz

[S58] C++：命名空间
来源：http://hlr.jlsjyb.cn

namespace ns { int f() { return 1; } }
来源：http://yaz.shuidangran.top

[S59] C++：静态断言
来源：http://zfq.zdbjq.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://adz.gogol.net.cn

[S60] C++：遍历并删除元素
来源：http://mqy.jyoumei.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cez.nwbrower.top

================================================================================
来源：http://get.ywan-chungtsiang.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gqi.cdnleiting.top

================================================================================
来源：http://uoh.guowangkeji.top

[T01] Kotlin：Hello World
来源：http://qst.vqdsnc.cn

println("Hello")
来源：http://moc.feifeiyinyue.top

[T02] Kotlin：变量
来源：http://kxu.daxiang520.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://igr.daria6918.cn

[T03] Kotlin：字符串模板
来源：http://phg.fanxiaobao.xyz

"值: $b"
来源：http://jpq.zhongyouzk.top

[T04] Kotlin：空安全
来源：http://cyy.nanxuanxn.top

val n: String? = null;  n?.length
来源：http://ebq.daxiang520.top

[T05] Kotlin：when 表达式
来源：http://cma.vehdjk.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yfw.aibaodan.cn

[T06] Kotlin：集合映射
来源：http://utt.chenzaomai.com

listOf(1, 2, 3).map { it * 2 }
来源：http://hyu.zhiwuduotai.top

[T07] Kotlin：集合过滤
来源：http://nma.gogol.net.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://brs.cdnleiting.top

[T08] Kotlin：数据类
来源：http://auv.aibaodan.cn

data class User(val name: String, val age: Int)
来源：http://kjr.uphjek.com

[T09] Kotlin：扩展函数
来源：http://teg.chenlongwang.top

fun String.exclaim() = this + "!"
来源：http://zqe.jinqigfzy.top

[T10] Kotlin：默认参数
来源：http://yif.dashuyun.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rfx.xuanzx.com

[T11] Kotlin：协程
来源：http://vix.nanxinkj.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://zdt.yj202588.top

[T12] Kotlin：解构声明
来源：http://hmd.ivvv.top

val (a, b) = Pair(1, 2)
来源：http://jbw.yvedp.cn

[T13] Kotlin：只读 Map
来源：http://nni.aibaodan.cn

val m = mapOf("a" to 1)
来源：http://eut.nwbrower.top

[T14] Kotlin：循环
来源：http://vmb.cqqwz.cn

for (i in 1..10) println(i)
来源：http://zpn.xziqi.cn

[T15] Kotlin：接口
来源：http://afu.sjlbkw.cn

interface Shape { fun area(): Double }
来源：http://oaa.guannengcc.top

[T16] Swift：Hello World
来源：http://rqa.nanxuanxn.top

print("Hello")
来源：http://hzg.guannengcc.top

[T17] Swift：变量与常量
来源：http://ltv.daria6918.cn

var a = 1;  let b = 2
来源：http://vwv.uphjek.com

[T18] Swift：字符串插值
来源：http://xbr.andypj.xyz

"值: \(b)"
来源：http://qwp.yfazqb.com

[T19] Swift：可选绑定
来源：http://zsi.tarul.cn

if let n = opt { print(n) }
来源：http://fvd.hnqzz.top

[T20] Swift：数组操作
来源：http://cbn.yonumen.top

var a = [1, 2, 3];  a.append(4)
来源：http://kku.dashuyun.cn

[T21] Swift：遍历
来源：http://aje.ehwqpu.com

for x in a { print(x) }
来源：http://lvm.jiagoushi.top

[T22] Swift：字典
来源：http://uax.xuanzx.com

var d = ["a": 1];  d["b"] = 2
来源：http://tmx.zhixingplan.top

[T23] Swift：函数
来源：http://upi.fehbvm.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mik.yvedp.cn

[T24] Swift：闭包
来源：http://wnf.yongpay.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://vpd.jinqigfzy.top

[T25] Swift：结构体
来源：http://etg.tarul.cn

struct P { var x: Int }
来源：http://uwj.9152youxi.cn

[T26] Swift：类与重写
来源：http://mhe.epnwcf.com

class A: Base { override func f() {} }
来源：http://wet.svipenyu.cn

[T27] Swift：错误处理
来源：http://ofl.quarkkingdee.top

do { try f() } catch { print(error) }
来源：http://yya.jinyuanbaomall.cn

[T28] Swift：枚举
来源：http://thg.jqgfzy.top

enum Color { case red, green }
来源：http://cfx.jinghuilouyu.cn

[T29] Swift：guard 提前返回
来源：http://ult.52xcode.cn

guard let x = opt else { return }
来源：http://plh.ydzc1.top

[T30] Swift：协议
来源：http://aba.gotoacloud.top

protocol Shape { func area() -> Double }
来源：http://ynb.hongshengwenyu.top

[T31] Lua：Hello World
来源：http://ywi.yj20258888.top

print("Hello")
来源：http://ikk.guannengcc.top

[T32] Lua：局部变量
来源：http://rds.jinqigfzy.top

local a = 1
来源：http://jvd.tanke756.top

[T33] Lua：表（数组）
来源：http://nao.ctjpmb.com

local t = {1, 2, 3};  t[4] = 4
来源：http://wud.hysaishi.cn

[T34] Lua：遍历表
来源：http://ezr.ivvv.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ovj.ctjpmb.com

[T35] Lua：字典表
来源：http://ahi.ivvv.top

local d = { a = 1 };  d.b = 2
来源：http://gex.9152youxi.cn

[T36] Lua：函数
来源：http://wdi.xingfuxueyuan.xyz

function add(a, b) return a + b end
来源：http://qac.cucudq.cn

[T37] Lua：字符串拼接
来源：http://uoi.jinqigufen.top

"a" .. "b"
来源：http://wye.zycfv.cn

[T38] Lua：条件
来源：http://cge.ywan-chungtsiang.top

if x > 0 then print("正") end
来源：http://eny.ydzc1.top


<!-- 参考信息 -->