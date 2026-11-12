代发 wailian999

echo $((1 + 2 * 3))
来源：http://vhp.52xcode.cn

[R28] 浮点运算
来源：http://idt.meibo888.top

echo "scale=2; 10/3" | bc
来源：http://jip.shanyushiyangkeji.top

[R29] 定义函数
来源：http://fbq.snrcjt.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://sry.epnwcf.com

[R30] 函数返回状态码
来源：http://pni.wangshuangyany.cn

f() { return 0; }; f || echo "失败了"
来源：http://bvh.hesvh.cn

[R31] 局部变量
来源：http://swp.zhiwuduotai.top

f() { local x=1; echo "$x"; }
来源：http://vuk.c1oappe.top

[R32] 参数个数校验
来源：http://qpc.tian-w.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mic.hysaishi.cn

[R33] 捕获错误并提示行号
来源：http://rge.aizwys.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vhd.shuidangran.top

[R34] 退出时清理
来源：http://kaw.jqgufenzy.top

trap 'rm -f "$tmp"' EXIT
来源：http://cfj.tianlin.xyz

[R35] 后台执行并等待
来源：http://mvt.nanxinkj.top

sleep 5 & pid=$!; wait "$pid"
来源：http://cex.dianchejie.cn

[R36] 并发执行多个任务
来源：http://acm.fehbvm.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qpl.yj20258.top

[R37] 把输出赋给变量
来源：http://kag.pengpengdd.cyou

files=$(ls -1)
来源：http://yco.yvedp.cn

[R38] 管道串联
来源：http://vxx.ywan-chungtsiang.top

cat a.txt | grep -i error | wc -l
来源：http://dqu.chenlongwang.top

[R39] 重定向标准输出与错误
来源：http://pjr.snrcjt.cn

cmd > out.log 2>&1
来源：http://rpa.hesvh.cn

[R40] 追加写日志
来源：http://odl.zhoulong.xyz

echo "log" >> out.log
来源：http://fdj.redwolf501.top

[R41] 丢弃输出
来源：http://rlc.nanxinkj.top

cmd >/dev/null 2>&1
来源：http://mjj.nwbrower.top

[R42] 输入重定向
来源：http://luv.zhengqikj.top

wc -l < a.txt
来源：http://bvr.zhaomingkeji.xyz

[R43] 按名字查找文件
来源：http://ncb.tanke756.top

find . -name "*.log" -type f
来源：http://tnm.hfpthk.cn

[R44] 按修改时间查找
来源：http://xoj.quarkkingdee.top

find . -mtime -7 -type f
来源：http://tnn.sxryk.cn

[R45] 批量删除
来源：http://pst.wangdashe.top

find . -name "*.tmp" -delete
来源：http://ili.ydzc1.top

[R46] 递归替换文件内容
来源：http://ney.shanyushiyangtech.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vlt.sjlbkw.cn

[R47] sed 单行替换
来源：http://djx.zhixingplan.top

sed -i 's/foo/bar/g' a.txt
来源：http://ani.zdqjudy.top

[R48] awk 取指定列
来源：http://esb.hnqzz.top

awk '{print $1, $3}' a.txt
来源：http://fkl.chenjidiqi.icu

[R49] awk 带条件
来源：http://uuk.zhengqikj.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sod.hywenlv.cn

[R50] awk 求和
来源：http://yqv.tarul.cn

awk '{s += $2} END {print s}' a.txt
来源：http://gim.ywan-chungtsiang.top

[R51] 排序去重取前几
来源：http://myy.shanyushiyangtech.top

sort a.txt | uniq -c | sort -rn | head
来源：http://akn.ivvv.top

[R52] 统计行数
来源：http://htj.tian-w.cn

wc -l a.txt
来源：http://btr.jinyuanbaomall.cn

[R53] 查看文件头与实时尾
来源：http://kyx.ydjk.org.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jtu.birdmap.top

[R54] 比较两个文件
来源：http://pcb.quarkkingdee.top

diff a.txt b.txt
来源：http://gls.zhengqikj.top

[R55] 压缩与解压
来源：http://epw.tanke756.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uef.daria6918.cn

[R56] 远程拷贝
来源：http://gwx.zhijiandao.cn

scp file user@host:/path/
来源：http://drz.jiagoushi.top

[R57] 远程执行命令
来源：http://yku.hammf.cn

ssh user@host 'uptime'
来源：http://oqu.ivvv.top

[R58] 下载文件
来源：http://qhb.hnxiangtu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qzs.aizwys.cn

[R59] 发 POST JSON
来源：http://bnq.ctjpmb.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xev.havefunace.top

[R60] 只看 HTTP 状态码
来源：http://aaj.jqgufenzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zyx.tianlin.xyz

[R61] 磁盘占用
来源：http://vqz.jianghu66.top

df -h;  du -sh *
来源：http://mwh.sufxvd.cn

[R62] 找最占空间的文件
来源：http://azp.yangfankeji.com

du -ah . | sort -rh | head -10
来源：http://dbo.wangdashe.top

[R63] 内存与进程
来源：http://odf.cqqwz.cn

free -h;  ps aux | grep nginx
来源：http://nnv.iojbl.cn

[R64] 结束进程
来源：http://lrn.bjfxy.top

kill -9 $(pgrep -f app.py)
来源：http://oaq.gaohongyu789.top

[R65] 查看端口占用
来源：http://thm.meibo888.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jtp.yueranfly.top

[R66] 定时任务
来源：http://skj.cashguo.top

crontab -e;  crontab -l
来源：http://rha.havefunace.top

[R67] 生成随机十六进制串
来源：http://wfl.shzxlz.cn

openssl rand -hex 16
来源：http://rhp.tanke756.top

[R68] 计算文件校验值
来源：http://poq.hammf.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hsz.dianchejie.cn

[R69] 生成随机密码
来源：http://skj.chenzaomai.com

head -c 16 /dev/urandom | base64
来源：http://adw.sufxvd.cn

[R70] 时间戳与互转
来源：http://agz.sweek.top

date +%s;  date -d @1700000000
来源：http://cao.ybcxt.top

[R71] 日期格式化
来源：http://ysc.tarul.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rbj.vehdjk.com

[R72] 等待端口就绪
来源：http://ocb.dashuyun.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://pkm.fengsongda.top

[R73] 分割大日志
来源：http://qst.52xcode.cn

split -l 1000 big.log part_
来源：http://usz.yj20258.top

[R74] 批量重命名
来源：http://fte.redwolf501.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://amw.hesvh.cn

[R75] 导出环境变量
来源：http://tfa.yj20258.top

export PATH="$HOME/bin:$PATH"
来源：http://vzt.gogol.net.cn

[R76] 使用临时文件
来源：http://zcf.haohaochexian.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mgl.xziqi.cn

[R77] 读取用户输入
来源：http://keo.sysykeji.top

read -rp "请输入: " ans
来源：http://qhf.xinyue.icu

[R78] 交互式菜单
来源：http://lyi.yfazqb.com

select opt in a b c; do echo "$opt"; break; done
来源：http://rql.pengpengdd.cyou

[R79] 解析命令行选项
来源：http://mxk.ydzc1.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tvz.jlsjyb.cn

[R80] 查看脚本执行耗时
来源：http://zam.sxryk.cn

time ./run.sh
来源：http://qmm.gaohongyu789.top

================================================================================
来源：http://zac.gogol.net.cn

S. C / C++ 专题
来源：http://pfv.fehbvm.com

================================================================================
来源：http://oxa.dashuyun.cn

[S01] C：Hello World
来源：http://tdi.jyoumei.cn

#include <stdio.h>
来源：http://mml.bjfxy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://xju.xingfuxueyuan.xyz

[S02] C：变量与格式化输出
来源：http://kqf.chenzaomai.com

int a = 10; printf("%d\n", a);
来源：http://nsk.gotoacloud.top

[S03] C：读入整数
来源：http://yxw.hammf.cn

int x; scanf("%d", &x);
来源：http://ufh.zhengqikj.top

[S04] C：字符串复制
来源：http://pgt.jinyuanbaomall.cn

char dst[32]; strcpy(dst, "hi");
来源：http://qnk.nwbrower.top

[S05] C：字符串长度
来源：http://thw.uphjek.com

strlen(s)
来源：http://lyw.vehdjk.com

[S06] C：字符串比较
来源：http://cgn.9152youxi.cn

strcmp(a, b) == 0
来源：http://wxk.ehwqpu.com

[S07] C：数组遍历求和
来源：http://ihp.gogol.net.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vhp.yonumen.top

[S08] C：动态内存分配与释放
来源：http://gwp.guannengcc.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cwn.aizwys.cn

[S09] C：结构体定义与初始化
来源：http://otp.tarul.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zpo.xinyue.icu

[S10] C：指针与解引用
来源：http://ant.jiagoushi.top

int *p = &a;  *p = 5;
来源：http://rwl.zhiwuduotai.top

[S11] C：逐行读文件
来源：http://cam.yueranfly.top

FILE *f = fopen("a.txt", "r");
来源：http://wpr.hfpthk.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vuk.zhixingplan.top

fclose(f);
来源：http://iyo.havefunace.top

[S12] C：写文件
来源：http://scg.hammf.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nvm.hammf.cn

[S13] C：宏定义
来源：http://ozy.shuidangran.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yng.nanxinkj.top

[S14] C：枚举
来源：http://zqf.haohaochexian.top

enum Color { RED, GREEN, BLUE };
来源：http://hip.hcnkem.com

[S15] C：类型转换
来源：http://ftn.mhx1999.top

(double) a / b
来源：http://enk.aizwys.cn

[S16] C：位操作置位
来源：http://gqo.hywenlv.cn

x |= (1 << 3);
来源：http://akb.yuxming.cn

[S17] C：安全拼接字符串
来源：http://asp.yueranfly.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qoc.snrcjt.cn

[S18] C：命令行参数
来源：http://pez.daxiang520.top

int main(int argc, char **argv)
来源：http://okg.guannengcc.top

[S19] C：快速排序
来源：http://kol.mhx1999.top

qsort(a, n, sizeof(int), cmp);
来源：http://ytm.daxiang520.top

[S20] C：二分查找
来源：http://tut.yfazqb.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gyi.andypj.xyz

[S21] C：字符类别判断
来源：http://syw.daria6918.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lll.gzhubu.top

[S22] C：字符串转数字
来源：http://sof.fzhhl.top

atoi("42");  strtod("3.14", NULL);
来源：http://fzy.mhx1999.top

[S23] C：随机数
来源：http://ylt.jlsjyb.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qno.nanxuanxn.top

[S24] C：获取本地时间
来源：http://lpz.yangfankeji.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tjb.cucudq.cn

[S25] C：内存拷贝
来源：http://pyx.zhongyouzk.top

memcpy(dst, src, n);
来源：http://iyb.tarul.cn

[S26] C：内存清零
来源：http://bsv.feifeiyinyue.top

memset(a, 0, sizeof a);
来源：http://ddj.smart0.xyz

[S27] C：定义常量
来源：http://cyn.bbcook.cn

const double PI = 3.14159;
来源：http://yla.zhaomingkeji.xyz

[S28] C：静态变量
来源：http://jpy.guowangkeji.top

static int counter = 0;
来源：http://mne.ctjpmb.com

[S29] C：变参函数
来源：http://zjq.hywenlv.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rec.jlsjyb.cn

[S30] C：头文件保护
来源：http://vgw.fzhhl.top

#ifndef X_H
来源：http://nea.aibaodan.cn

#define X_H
来源：http://wkt.cdnleiting.top

#endif
来源：http://yxz.tanke756.top

[S31] C++：Hello World
来源：http://rvl.hcnkem.com

#include <iostream>
来源：http://jjz.svipenyu.cn

int main() { std::cout << "Hello\n"; }
来源：http://eyw.jqgfzy.top

[S32] C++：字符串
来源：http://bal.havefunace.top

std::string s = "hi";  s += "!";
来源：http://tfr.hnxiangtu.top

[S33] C++：vector 增删
来源：http://ibd.c1oappe.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jtj.dianchejie.cn

[S34] C++：遍历 vector
来源：http://xoa.yuxming.cn

for (auto &x : v) { std::cout << x; }
来源：http://sxb.fanxiaobao.xyz

[S35] C++：map
来源：http://dqs.zdbjq.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bsq.chenlongwang.top

[S36] C++：unordered_map
来源：http://ghe.bjfxy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jwp.cucudq.cn

[S37] C++：set
来源：http://yuw.vqdsnc.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sts.quarkkingdee.top

[S38] C++：排序
来源：http://nqh.0kj1m.cn

std::sort(v.begin(), v.end());
来源：http://avs.cheryme.top

[S39] C++：自定义比较器排序
来源：http://eys.shuidangran.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gyl.shuidangran.top

[S40] C++：查找元素
来源：http://klg.xuanzx.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://coa.jianghu66.top

[S41] C++：类与构造函数
来源：http://ows.0kj1m.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zon.tanke756.top

[S42] C++：继承与虚函数
来源：http://kbl.yj20258.top

class B : public Base { public: void f() override {} };
来源：http://abf.yonumen.top

[S43] C++：智能指针
来源：http://vmh.jiagoushi.top

auto p = std::make_unique<int>(5);
来源：http://ohm.sxryk.cn

[S44] C++：引用传参
来源：http://nvi.gotoacloud.top

void inc(int &x) { ++x; }
来源：http://nwu.feifeiyinyue.top

[S45] C++：lambda
来源：http://qnd.xylfe.cn

auto add = [](int a, int b) { return a + b; };
来源：http://dha.wangshuangyany.cn

[S46] C++：函数模板
来源：http://nji.svipenyu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://int.ivvv.top

[S47] C++：结构化绑定遍历
来源：http://gfy.jyoumei.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ngs.jiagoushi.top

[S48] C++：逐行读文件
来源：http://jaq.zhaomingkeji.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://ivh.sweek.top

while (std::getline(in, line)) { }
来源：http://tdn.zhengqikj.top

[S49] C++：写文件
来源：http://ydu.yj20258888.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://irk.jinqigfzy.top

[S50] C++：格式化数字
来源：http://epl.hammf.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nwt.zdqjudy.top

[S51] C++：显式类型转换
来源：http://muj.ppjwa.cn

static_cast<double>(a) / b
来源：http://amo.zycfv.cn

[S52] C++：const 与 noexcept
来源：http://fua.zhoulong.xyz

int size() const noexcept { return n_; }
来源：http://mid.aibaodan.cn

[S53] C++：移动语义
来源：http://wom.sxryk.cn

std::vector<int> w = std::move(v);
来源：http://dyj.shzxlz.cn

[S54] C++：异常处理
来源：http://mom.hywenlv.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://len.zdbjq.cn

[S55] C++：结构化绑定
来源：http://lma.jianghu66.top

auto [a, b] = std::make_pair(1, 2);
来源：http://tli.cashguo.top

[S56] C++：optional
来源：http://oge.shanyushiyangtech.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ixq.xinyue.icu

[S57] C++：编译期常量
来源：http://sdc.cucudq.cn

constexpr int N = 10;
来源：http://pns.pengpengdd.cyou

[S58] C++：命名空间
来源：http://nfz.xuetiantiany.cn

namespace ns { int f() { return 1; } }
来源：http://sem.jyoumei.cn

[S59] C++：静态断言
来源：http://dvj.chenzaomai.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tmd.fzhhl.top

[S60] C++：遍历并删除元素
来源：http://zse.hnqzz.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pfj.yj20258888.top

================================================================================
来源：http://giy.tarul.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://efi.shuidangran.top

================================================================================
来源：http://xjf.epnwcf.com

[T01] Kotlin：Hello World
来源：http://dlu.sxryk.cn

println("Hello")
来源：http://ory.pengpengdd.cyou

[T02] Kotlin：变量
来源：http://lfs.andypj.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fyb.zhijiandao.cn

[T03] Kotlin：字符串模板
来源：http://jqk.xinyue.icu

"值: $b"
来源：http://zgg.sysykeji.top

[T04] Kotlin：空安全
来源：http://jis.gaohongyu789.top

val n: String? = null;  n?.length
来源：http://rtp.sufxvd.cn

[T05] Kotlin：when 表达式
来源：http://ujf.zdqjudy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qpk.jinqigfzy.top

[T06] Kotlin：集合映射
来源：http://voy.hesvh.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://wjq.daxiang520.top

[T07] Kotlin：集合过滤
来源：http://tfm.zhoulong.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://oiw.jianghu66.top

[T08] Kotlin：数据类
来源：http://oqb.tian-w.cn

data class User(val name: String, val age: Int)
来源：http://aai.0kj1m.cn

[T09] Kotlin：扩展函数
来源：http://knr.0kj1m.cn

fun String.exclaim() = this + "!"
来源：http://ump.tianlin.xyz

[T10] Kotlin：默认参数
来源：http://ude.yuanzhike.top

fun greet(name: String = "World") = "Hi $name"
来源：http://tog.ywan-chungtsiang.top

[T11] Kotlin：协程
来源：http://dfg.jqgufenzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://yrt.chenzaomai.com

[T12] Kotlin：解构声明
来源：http://xbe.ydzc1.top

val (a, b) = Pair(1, 2)
来源：http://cga.ehwqpu.com

[T13] Kotlin：只读 Map
来源：http://ggb.havefunace.top

val m = mapOf("a" to 1)
来源：http://mtj.hammf.cn

[T14] Kotlin：循环
来源：http://nxq.guowangkeji.top

for (i in 1..10) println(i)
来源：http://vio.vehdjk.com

[T15] Kotlin：接口
来源：http://snw.zhongyouzk.top

interface Shape { fun area(): Double }
来源：http://eas.mhx1999.top

[T16] Swift：Hello World
来源：http://snq.ybcxt.top

print("Hello")
来源：http://eqb.xylfe.cn

[T17] Swift：变量与常量
来源：http://cbf.daria6918.cn

var a = 1;  let b = 2
来源：http://wsa.hongshengwenyu.top

[T18] Swift：字符串插值
来源：http://yuk.jqgufenzy.top

"值: \(b)"
来源：http://ogo.ctjpmb.com

[T19] Swift：可选绑定
来源：http://wep.jqgfzy.top

if let n = opt { print(n) }
来源：http://uai.tianlin.xyz

[T20] Swift：数组操作
来源：http://oye.shanyushiyangtech.top

var a = [1, 2, 3];  a.append(4)
来源：http://vpw.feifeiyinyue.top

[T21] Swift：遍历
来源：http://dub.xylfe.cn

for x in a { print(x) }
来源：http://bhj.shanyushiyangkeji.top

[T22] Swift：字典
来源：http://xjl.bjfxy.top

var d = ["a": 1];  d["b"] = 2
来源：http://fpf.nanxinkj.top

[T23] Swift：函数
来源：http://ayb.sjlbkw.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://iob.yfazqb.com

[T24] Swift：闭包
来源：http://rfb.yueranfly.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://apb.pycfn.com

[T25] Swift：结构体
来源：http://rqg.zhoulong.xyz

struct P { var x: Int }
来源：http://qlx.cheryme.top

[T26] Swift：类与重写
来源：http://iln.yfazqb.com

class A: Base { override func f() {} }
来源：http://dhv.shzxlz.cn

[T27] Swift：错误处理
来源：http://efk.shzxlz.cn

do { try f() } catch { print(error) }
来源：http://lht.hammf.cn

[T28] Swift：枚举
来源：http://kba.sysykeji.top

enum Color { case red, green }
来源：http://clu.wangshuangyany.cn

[T29] Swift：guard 提前返回
来源：http://rym.sufxvd.cn

guard let x = opt else { return }
来源：http://rep.wangshuangyany.cn

[T30] Swift：协议
来源：http://zva.jianghu66.top

protocol Shape { func area() -> Double }
来源：http://jfw.ydjk.org.cn


<!-- 参考信息 -->