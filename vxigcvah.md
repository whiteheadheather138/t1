代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://xdb.yueranfly.top

[R36] 并发执行多个任务
来源：http://ivm.andypj.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hxo.hywenlv.cn

[R37] 把输出赋给变量
来源：http://nvr.fktsv.cn

files=$(ls -1)
来源：http://foo.xuanzx.com

[R38] 管道串联
来源：http://liz.ppjwa.cn

cat a.txt | grep -i error | wc -l
来源：http://cqb.nwbrower.top

[R39] 重定向标准输出与错误
来源：http://ern.yanxiufei.cn

cmd > out.log 2>&1
来源：http://lrr.smart0.xyz

[R40] 追加写日志
来源：http://nfh.ywan-chungtsiang.top

echo "log" >> out.log
来源：http://cga.ybcxt.top

[R41] 丢弃输出
来源：http://sel.hammf.cn

cmd >/dev/null 2>&1
来源：http://lzf.c1oappe.top

[R42] 输入重定向
来源：http://ytl.jinghuilouyu.cn

wc -l < a.txt
来源：http://vph.ehwqpu.com

[R43] 按名字查找文件
来源：http://edr.wangshuangyany.cn

find . -name "*.log" -type f
来源：http://kul.snrcjt.cn

[R44] 按修改时间查找
来源：http://xtk.wangshuangyany.cn

find . -mtime -7 -type f
来源：http://zwi.hysaishi.cn

[R45] 批量删除
来源：http://fng.zhoulong.xyz

find . -name "*.tmp" -delete
来源：http://llu.yj20258888.top

[R46] 递归替换文件内容
来源：http://hpl.yueranfly.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gqj.vehdjk.com

[R47] sed 单行替换
来源：http://zzf.aizwys.cn

sed -i 's/foo/bar/g' a.txt
来源：http://lcx.52xcode.cn

[R48] awk 取指定列
来源：http://agk.shuidangran.top

awk '{print $1, $3}' a.txt
来源：http://ced.kuanghao11.cn

[R49] awk 带条件
来源：http://qwj.jinyuanbaomall.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ubd.birdmap.top

[R50] awk 求和
来源：http://dxu.hysaishi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fxc.tarul.cn

[R51] 排序去重取前几
来源：http://yvd.ivvv.top

sort a.txt | uniq -c | sort -rn | head
来源：http://imu.hongshengwenyu.top

[R52] 统计行数
来源：http://uxu.cucudq.cn

wc -l a.txt
来源：http://pts.zhengqikj.top

[R53] 查看文件头与实时尾
来源：http://wre.snrcjt.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qbd.shanyushiyangkeji.top

[R54] 比较两个文件
来源：http://nbp.uphjek.com

diff a.txt b.txt
来源：http://fbw.52xcode.cn

[R55] 压缩与解压
来源：http://jxw.andypj.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bwl.andypj.xyz

[R56] 远程拷贝
来源：http://vla.cheryme.top

scp file user@host:/path/
来源：http://rky.aizwys.cn

[R57] 远程执行命令
来源：http://sph.yj20258.top

ssh user@host 'uptime'
来源：http://amb.ydzc1.top

[R58] 下载文件
来源：http://qcw.bbcook.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sus.sjlbkw.cn

[R59] 发 POST JSON
来源：http://ljv.smart0.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nfm.fehbvm.com

[R60] 只看 HTTP 状态码
来源：http://tkm.bbcook.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lzu.yonumen.top

[R61] 磁盘占用
来源：http://khf.quarkkingdee.top

df -h;  du -sh *
来源：http://wnv.shanyushiyangkeji.top

[R62] 找最占空间的文件
来源：http://ocs.zhaomingkeji.xyz

du -ah . | sort -rh | head -10
来源：http://igo.shangyingyoupin.top

[R63] 内存与进程
来源：http://mpx.yanxiufei.cn

free -h;  ps aux | grep nginx
来源：http://xot.xinyue.icu

[R64] 结束进程
来源：http://eyc.birdmap.top

kill -9 $(pgrep -f app.py)
来源：http://acr.jinqigfzy.top

[R65] 查看端口占用
来源：http://iqn.yuanzhike.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dkk.hysaishi.cn

[R66] 定时任务
来源：http://aln.cheryme.top

crontab -e;  crontab -l
来源：http://crp.jinghuilouyu.cn

[R67] 生成随机十六进制串
来源：http://myp.jinqigufen.top

openssl rand -hex 16
来源：http://jsu.gogol.net.cn

[R68] 计算文件校验值
来源：http://fcl.chenjidiqi.icu

sha256sum a.txt;  md5sum a.txt
来源：http://eto.0kj1m.cn

[R69] 生成随机密码
来源：http://rqn.yongpay.top

head -c 16 /dev/urandom | base64
来源：http://oqx.fehbvm.com

[R70] 时间戳与互转
来源：http://fwd.kuanghao11.cn

date +%s;  date -d @1700000000
来源：http://xdc.gogol.net.cn

[R71] 日期格式化
来源：http://bjs.yvedp.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://cjg.0kj1m.cn

[R72] 等待端口就绪
来源：http://jlf.guannengcc.top

until nc -z localhost 3306; do sleep 1; done
来源：http://mpb.nanxinkj.top

[R73] 分割大日志
来源：http://xcx.yfazqb.com

split -l 1000 big.log part_
来源：http://eha.cheryme.top

[R74] 批量重命名
来源：http://odq.kuanghao11.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rdo.yongpay.top

[R75] 导出环境变量
来源：http://ygw.gogol.net.cn

export PATH="$HOME/bin:$PATH"
来源：http://nmg.316326.xyz

[R76] 使用临时文件
来源：http://typ.hywenlv.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zht.nanxinkj.top

[R77] 读取用户输入
来源：http://ybd.zhongyouzk.top

read -rp "请输入: " ans
来源：http://fwc.yonumen.top

[R78] 交互式菜单
来源：http://loj.mhx1999.top

select opt in a b c; do echo "$opt"; break; done
来源：http://kdn.epnwcf.com

[R79] 解析命令行选项
来源：http://zbd.guowangkeji.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://oyk.gotoacloud.top

[R80] 查看脚本执行耗时
来源：http://anj.jlsjyb.cn

time ./run.sh
来源：http://hrt.vqdsnc.cn

================================================================================
来源：http://wla.ydjk.org.cn

S. C / C++ 专题
来源：http://nfq.cashguo.top

================================================================================
来源：http://kxb.havefunace.top

[S01] C：Hello World
来源：http://wbf.hnxiangtu.top

#include <stdio.h>
来源：http://opf.pengpengdd.cyou

int main(void) { printf("Hello\n"); return 0; }
来源：http://bnl.gotoacloud.top

[S02] C：变量与格式化输出
来源：http://beq.cqqwz.cn

int a = 10; printf("%d\n", a);
来源：http://ate.mhx1999.top

[S03] C：读入整数
来源：http://rry.aizwys.cn

int x; scanf("%d", &x);
来源：http://fpj.sxryk.cn

[S04] C：字符串复制
来源：http://xjl.zhiwuduotai.top

char dst[32]; strcpy(dst, "hi");
来源：http://pws.shzxlz.cn

[S05] C：字符串长度
来源：http://pnl.nanxinkj.top

strlen(s)
来源：http://dxv.bjfxy.top

[S06] C：字符串比较
来源：http://rdp.zhaomingkeji.xyz

strcmp(a, b) == 0
来源：http://pyc.chenzaomai.com

[S07] C：数组遍历求和
来源：http://zqf.yuanzhike.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jin.fehbvm.com

[S08] C：动态内存分配与释放
来源：http://jpo.zhixingplan.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ldv.ctjpmb.com

[S09] C：结构体定义与初始化
来源：http://jns.quarkkingdee.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hcz.hnxiangtu.top

[S10] C：指针与解引用
来源：http://xvh.fktsv.cn

int *p = &a;  *p = 5;
来源：http://pll.tanke756.top

[S11] C：逐行读文件
来源：http://ctm.zycfv.cn

FILE *f = fopen("a.txt", "r");
来源：http://fha.tarul.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://onn.fktsv.cn

fclose(f);
来源：http://xwa.dashuyun.cn

[S12] C：写文件
来源：http://xcv.epnwcf.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pdt.birdmap.top

[S13] C：宏定义
来源：http://efp.hammf.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://udn.cdnleiting.top

[S14] C：枚举
来源：http://snt.shanyushiyangkeji.top

enum Color { RED, GREEN, BLUE };
来源：http://tqp.sxryk.cn

[S15] C：类型转换
来源：http://mpi.hfpthk.cn

(double) a / b
来源：http://ukr.sjlbkw.cn

[S16] C：位操作置位
来源：http://ypf.ehwqpu.com

x |= (1 << 3);
来源：http://bua.gotoacloud.top

[S17] C：安全拼接字符串
来源：http://wdk.xylfe.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gbd.zhixingplan.top

[S18] C：命令行参数
来源：http://gai.jlsjyb.cn

int main(int argc, char **argv)
来源：http://ywj.316326.xyz

[S19] C：快速排序
来源：http://nln.andypj.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://imj.snrcjt.cn

[S20] C：二分查找
来源：http://fqu.hammf.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pac.shuidangran.top

[S21] C：字符类别判断
来源：http://wql.jqgfzy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fud.fzhhl.top

[S22] C：字符串转数字
来源：http://egf.yonumen.top

atoi("42");  strtod("3.14", NULL);
来源：http://umx.xuanzx.com

[S23] C：随机数
来源：http://ntw.xingfuxueyuan.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://tui.uphjek.com

[S24] C：获取本地时间
来源：http://nxn.ivvv.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qyn.shangyingyoupin.top

[S25] C：内存拷贝
来源：http://bps.hnxiangtu.top

memcpy(dst, src, n);
来源：http://wht.zhengqikj.top

[S26] C：内存清零
来源：http://zcd.cqqwz.cn

memset(a, 0, sizeof a);
来源：http://iaw.sjlbkw.cn

[S27] C：定义常量
来源：http://jdl.yongpay.top

const double PI = 3.14159;
来源：http://nro.tarul.cn

[S28] C：静态变量
来源：http://ome.dashuyun.cn

static int counter = 0;
来源：http://gkb.hnxiangtu.top

[S29] C：变参函数
来源：http://die.mhx1999.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://afi.hfpthk.cn

[S30] C：头文件保护
来源：http://czw.jiagoushi.top

#ifndef X_H
来源：http://mhi.mhx1999.top

#define X_H
来源：http://bqo.yfazqb.com

#endif
来源：http://gjr.shangyingyoupin.top

[S31] C++：Hello World
来源：http://avk.bbcook.cn

#include <iostream>
来源：http://gyw.yvedp.cn

int main() { std::cout << "Hello\n"; }
来源：http://myg.shanyushiyangkeji.top

[S32] C++：字符串
来源：http://pzq.cucudq.cn

std::string s = "hi";  s += "!";
来源：http://wow.guowangkeji.top

[S33] C++：vector 增删
来源：http://jsa.cheryme.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://geh.sjlbkw.cn

[S34] C++：遍历 vector
来源：http://ega.sxryk.cn

for (auto &x : v) { std::cout << x; }
来源：http://phw.shangyingyoupin.top

[S35] C++：map
来源：http://ygo.jqgufenzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://byj.pycfn.com

[S36] C++：unordered_map
来源：http://gqe.fanxiaobao.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pna.nwbrower.top

[S37] C++：set
来源：http://oea.yanxiufei.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fzi.zhengqikj.top

[S38] C++：排序
来源：http://ygy.jiagoushi.top

std::sort(v.begin(), v.end());
来源：http://rui.guowangkeji.top

[S39] C++：自定义比较器排序
来源：http://qsr.cheryme.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://evg.ctjpmb.com

[S40] C++：查找元素
来源：http://ewn.kuanghao11.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uiz.yonumen.top

[S41] C++：类与构造函数
来源：http://rok.zhengqikj.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nuq.tian-w.cn

[S42] C++：继承与虚函数
来源：http://rnu.hammf.cn

class B : public Base { public: void f() override {} };
来源：http://fis.uphjek.com

[S43] C++：智能指针
来源：http://utw.sweek.top

auto p = std::make_unique<int>(5);
来源：http://usn.epnwcf.com

[S44] C++：引用传参
来源：http://vkf.52xcode.cn

void inc(int &x) { ++x; }
来源：http://tsr.316326.xyz

[S45] C++：lambda
来源：http://ujm.xuanzx.com

auto add = [](int a, int b) { return a + b; };
来源：http://ygv.birdmap.top

[S46] C++：函数模板
来源：http://roe.jyoumei.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://exn.jinqigfzy.top

[S47] C++：结构化绑定遍历
来源：http://pew.feifeiyinyue.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ljn.pengpengdd.cyou

[S48] C++：逐行读文件
来源：http://zrj.andypj.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://wvf.fehbvm.com

while (std::getline(in, line)) { }
来源：http://dzw.sysykeji.top

[S49] C++：写文件
来源：http://yfp.jlsjyb.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ysj.tian-w.cn

[S50] C++：格式化数字
来源：http://nre.vehdjk.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sgs.dashuyun.cn

[S51] C++：显式类型转换
来源：http://ptk.yj20258888.top

static_cast<double>(a) / b
来源：http://zvp.nanxuanxn.top

[S52] C++：const 与 noexcept
来源：http://hxh.birdmap.top

int size() const noexcept { return n_; }
来源：http://epo.ydzc1.top

[S53] C++：移动语义
来源：http://zil.jinqigufen.top

std::vector<int> w = std::move(v);
来源：http://jft.ehwqpu.com

[S54] C++：异常处理
来源：http://hjr.yfazqb.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vxv.quarkkingdee.top

[S55] C++：结构化绑定
来源：http://poy.ehwqpu.com

auto [a, b] = std::make_pair(1, 2);
来源：http://psi.epnwcf.com

[S56] C++：optional
来源：http://hxd.yuanzhike.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qxh.jqgufenzy.top

[S57] C++：编译期常量
来源：http://gki.snrcjt.cn

constexpr int N = 10;
来源：http://prr.guowangkeji.top

[S58] C++：命名空间
来源：http://taj.tian-w.cn

namespace ns { int f() { return 1; } }
来源：http://dbu.gogol.net.cn

[S59] C++：静态断言
来源：http://wum.hnxiangtu.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fmz.gaohongyu789.top

[S60] C++：遍历并删除元素
来源：http://mrz.shanyushiyangkeji.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xer.yj20258.top

================================================================================
来源：http://bqo.hysaishi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nnd.jianghu66.top

================================================================================
来源：http://eaw.xingfuxueyuan.xyz

[T01] Kotlin：Hello World
来源：http://vdi.tian-w.cn

println("Hello")
来源：http://jht.zdqjudy.top

[T02] Kotlin：变量
来源：http://iwv.fehbvm.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ohw.zhixingplan.top

[T03] Kotlin：字符串模板
来源：http://lax.tanke756.top

"值: $b"
来源：http://ufp.gzhubu.top

[T04] Kotlin：空安全
来源：http://iqn.chenzaomai.com

val n: String? = null;  n?.length
来源：http://nql.chenzaomai.com

[T05] Kotlin：when 表达式
来源：http://ulf.fzhhl.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gvi.9152youxi.cn

[T06] Kotlin：集合映射
来源：http://giu.zhaomingkeji.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://opj.hnxiangtu.top

[T07] Kotlin：集合过滤
来源：http://zju.yj202588.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://mbw.0kj1m.cn

[T08] Kotlin：数据类
来源：http://spw.yfazqb.com

data class User(val name: String, val age: Int)
来源：http://zwo.jiagoushi.top

[T09] Kotlin：扩展函数
来源：http://gkf.havefunace.top

fun String.exclaim() = this + "!"
来源：http://gco.smart0.xyz

[T10] Kotlin：默认参数
来源：http://uwe.jinqigufen.top

fun greet(name: String = "World") = "Hi $name"
来源：http://wuj.jqgfzy.top

[T11] Kotlin：协程
来源：http://jiy.chenzaomai.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://djz.kuanghao11.cn

[T12] Kotlin：解构声明
来源：http://mgs.nanxinkj.top

val (a, b) = Pair(1, 2)
来源：http://mgu.epnwcf.com

[T13] Kotlin：只读 Map
来源：http://fqj.zhongyouzk.top

val m = mapOf("a" to 1)
来源：http://vja.xziqi.cn

[T14] Kotlin：循环
来源：http://lsc.chenlongwang.top

for (i in 1..10) println(i)
来源：http://gyj.hesvh.cn

[T15] Kotlin：接口
来源：http://nue.nanxinkj.top

interface Shape { fun area(): Double }
来源：http://oso.sysykeji.top

[T16] Swift：Hello World
来源：http://hek.sxryk.cn

print("Hello")
来源：http://dkb.ehwqpu.com

[T17] Swift：变量与常量
来源：http://oxf.yangfankeji.com

var a = 1;  let b = 2
来源：http://trx.cdnleiting.top

[T18] Swift：字符串插值
来源：http://vra.gotoacloud.top

"值: \(b)"
来源：http://ssp.sjlbkw.cn

[T19] Swift：可选绑定
来源：http://qzi.yuanzhike.top

if let n = opt { print(n) }
来源：http://hcm.ydjk.org.cn

[T20] Swift：数组操作
来源：http://pcj.cqqwz.cn

var a = [1, 2, 3];  a.append(4)
来源：http://uvi.jinyuanbaomall.cn

[T21] Swift：遍历
来源：http://bgg.yangfankeji.com

for x in a { print(x) }
来源：http://kvr.feifeiyinyue.top

[T22] Swift：字典
来源：http://mjd.sysykeji.top

var d = ["a": 1];  d["b"] = 2
来源：http://jvs.zhiwuduotai.top

[T23] Swift：函数
来源：http://csb.yongpay.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yuo.vqdsnc.cn

[T24] Swift：闭包
来源：http://qpw.jlsjyb.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://nrl.havefunace.top

[T25] Swift：结构体
来源：http://jxw.xziqi.cn

struct P { var x: Int }
来源：http://nig.cqqwz.cn

[T26] Swift：类与重写
来源：http://jrm.svipenyu.cn

class A: Base { override func f() {} }
来源：http://pvo.0kj1m.cn

[T27] Swift：错误处理
来源：http://gzy.jinyuanbaomall.cn

do { try f() } catch { print(error) }
来源：http://ofq.gaohongyu789.top

[T28] Swift：枚举
来源：http://qbz.snrcjt.cn

enum Color { case red, green }
来源：http://oau.kuanghao11.cn

[T29] Swift：guard 提前返回
来源：http://nkb.daxiang520.top

guard let x = opt else { return }
来源：http://yae.aizwys.cn

[T30] Swift：协议
来源：http://pin.svipenyu.cn

protocol Shape { func area() -> Double }
来源：http://kuz.redwolf501.top

[T31] Lua：Hello World
来源：http://zyr.ppjwa.cn

print("Hello")
来源：http://twq.meibo888.top

[T32] Lua：局部变量
来源：http://slm.sweek.top

local a = 1
来源：http://qqp.dashuyun.cn

[T33] Lua：表（数组）
来源：http://qwg.nanxuanxn.top

local t = {1, 2, 3};  t[4] = 4
来源：http://lbp.zhijiandao.cn

[T34] Lua：遍历表
来源：http://tfr.ywan-chungtsiang.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ron.daxiang520.top

[T35] Lua：字典表
来源：http://dyn.fzhhl.top

local d = { a = 1 };  d.b = 2
来源：http://lqr.zycfv.cn

[T36] Lua：函数
来源：http://nco.uphjek.com

function add(a, b) return a + b end
来源：http://vxy.pycfn.com

[T37] Lua：字符串拼接
来源：http://wqg.jinyuanbaomall.cn

"a" .. "b"
来源：http://muw.gaohongyu789.top

[T38] Lua：条件
来源：http://ifl.fengsongda.top

if x > 0 then print("正") end
来源：http://yht.sufxvd.cn


<!-- 参考信息 -->