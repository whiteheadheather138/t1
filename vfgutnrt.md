代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ncj.pengpengdd.cyou

[R34] 退出时清理
来源：http://rvd.gotoacloud.top

trap 'rm -f "$tmp"' EXIT
来源：http://bbl.0kj1m.cn

[R35] 后台执行并等待
来源：http://agr.gzhubu.top

sleep 5 & pid=$!; wait "$pid"
来源：http://uva.gogol.net.cn

[R36] 并发执行多个任务
来源：http://pdu.fengsongda.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kdf.0kj1m.cn

[R37] 把输出赋给变量
来源：http://bpv.xuanzx.com

files=$(ls -1)
来源：http://gqd.yueranfly.top

[R38] 管道串联
来源：http://xps.jinghuilouyu.cn

cat a.txt | grep -i error | wc -l
来源：http://sau.quarkkingdee.top

[R39] 重定向标准输出与错误
来源：http://oam.hysaishi.cn

cmd > out.log 2>&1
来源：http://dbe.dianchejie.cn

[R40] 追加写日志
来源：http://tnp.ivvv.top

echo "log" >> out.log
来源：http://sge.kuanghao11.cn

[R41] 丢弃输出
来源：http://mej.ywan-chungtsiang.top

cmd >/dev/null 2>&1
来源：http://udr.yangfankeji.com

[R42] 输入重定向
来源：http://gdn.gzhubu.top

wc -l < a.txt
来源：http://yuh.wangdashe.top

[R43] 按名字查找文件
来源：http://nvj.yangfankeji.com

find . -name "*.log" -type f
来源：http://obo.andypj.xyz

[R44] 按修改时间查找
来源：http://hef.zhijiandao.cn

find . -mtime -7 -type f
来源：http://yxv.cashguo.top

[R45] 批量删除
来源：http://box.ydzc1.top

find . -name "*.tmp" -delete
来源：http://eye.gotoacloud.top

[R46] 递归替换文件内容
来源：http://pur.bbcook.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nvc.hesvh.cn

[R47] sed 单行替换
来源：http://nvk.xinyue.icu

sed -i 's/foo/bar/g' a.txt
来源：http://ymu.jinghuilouyu.cn

[R48] awk 取指定列
来源：http://xkb.gaohongyu789.top

awk '{print $1, $3}' a.txt
来源：http://lej.chenlongwang.top

[R49] awk 带条件
来源：http://zlv.vehdjk.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gbp.dashuyun.cn

[R50] awk 求和
来源：http://fum.gotoacloud.top

awk '{s += $2} END {print s}' a.txt
来源：http://bdh.bbcook.cn

[R51] 排序去重取前几
来源：http://ski.quarkkingdee.top

sort a.txt | uniq -c | sort -rn | head
来源：http://qzq.gaohongyu789.top

[R52] 统计行数
来源：http://jwc.yvedp.cn

wc -l a.txt
来源：http://eje.yongpay.top

[R53] 查看文件头与实时尾
来源：http://jyf.jinyuanbaomall.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vun.fzhhl.top

[R54] 比较两个文件
来源：http://qxn.pycfn.com

diff a.txt b.txt
来源：http://fhu.pengpengdd.cyou

[R55] 压缩与解压
来源：http://nrd.feifeiyinyue.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://skk.hysaishi.cn

[R56] 远程拷贝
来源：http://kjy.haohaochexian.top

scp file user@host:/path/
来源：http://dec.chenlongwang.top

[R57] 远程执行命令
来源：http://ekf.jinyuanbaomall.cn

ssh user@host 'uptime'
来源：http://ksf.wangshuangyany.cn

[R58] 下载文件
来源：http://twz.sxryk.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zyg.feifeiyinyue.top

[R59] 发 POST JSON
来源：http://bnd.wangshuangyany.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qmq.xuetiantiany.cn

[R60] 只看 HTTP 状态码
来源：http://lkq.meibo888.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dfz.uphjek.com

[R61] 磁盘占用
来源：http://zdf.sysykeji.top

df -h;  du -sh *
来源：http://dte.hcnkem.com

[R62] 找最占空间的文件
来源：http://tyd.nanxuanxn.top

du -ah . | sort -rh | head -10
来源：http://lds.jiagoushi.top

[R63] 内存与进程
来源：http://uuo.zhijiandao.cn

free -h;  ps aux | grep nginx
来源：http://wpk.ctjpmb.com

[R64] 结束进程
来源：http://eua.jinqigfzy.top

kill -9 $(pgrep -f app.py)
来源：http://ben.gogol.net.cn

[R65] 查看端口占用
来源：http://mma.andypj.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bfy.quarkkingdee.top

[R66] 定时任务
来源：http://dmj.jyoumei.cn

crontab -e;  crontab -l
来源：http://due.tianlin.xyz

[R67] 生成随机十六进制串
来源：http://nwf.meibo888.top

openssl rand -hex 16
来源：http://lir.zhiwuduotai.top

[R68] 计算文件校验值
来源：http://kcm.yvedp.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mde.cucudq.cn

[R69] 生成随机密码
来源：http://oqg.yfazqb.com

head -c 16 /dev/urandom | base64
来源：http://vbt.haohaochexian.top

[R70] 时间戳与互转
来源：http://mgi.gogol.net.cn

date +%s;  date -d @1700000000
来源：http://syd.sxryk.cn

[R71] 日期格式化
来源：http://tpv.sjlbkw.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ftz.hywenlv.cn

[R72] 等待端口就绪
来源：http://djv.kuanghao11.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vah.jlsjyb.cn

[R73] 分割大日志
来源：http://bvb.xuanzx.com

split -l 1000 big.log part_
来源：http://yko.jiagoushi.top

[R74] 批量重命名
来源：http://njr.guowangkeji.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nlz.chenzaomai.com

[R75] 导出环境变量
来源：http://ehu.shanyushiyangkeji.top

export PATH="$HOME/bin:$PATH"
来源：http://ohi.iojbl.cn

[R76] 使用临时文件
来源：http://btv.gaohongyu789.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ukd.hcnkem.com

[R77] 读取用户输入
来源：http://qya.jinyuanbaomall.cn

read -rp "请输入: " ans
来源：http://fbm.daxiang520.top

[R78] 交互式菜单
来源：http://uqh.chenjidiqi.icu

select opt in a b c; do echo "$opt"; break; done
来源：http://ilh.hfpthk.cn

[R79] 解析命令行选项
来源：http://wpc.zhijiandao.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kda.nwbrower.top

[R80] 查看脚本执行耗时
来源：http://ijj.cqqwz.cn

time ./run.sh
来源：http://lmq.zhiwuduotai.top

================================================================================
来源：http://wmm.316326.xyz

S. C / C++ 专题
来源：http://ufw.ppjwa.cn

================================================================================
来源：http://xrm.nwbrower.top

[S01] C：Hello World
来源：http://pxe.sxryk.cn

#include <stdio.h>
来源：http://tby.shanyushiyangkeji.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://cud.quarkkingdee.top

[S02] C：变量与格式化输出
来源：http://hsi.hnxiangtu.top

int a = 10; printf("%d\n", a);
来源：http://fwv.sufxvd.cn

[S03] C：读入整数
来源：http://qgn.dashuyun.cn

int x; scanf("%d", &x);
来源：http://kmc.svipenyu.cn

[S04] C：字符串复制
来源：http://nrg.sysykeji.top

char dst[32]; strcpy(dst, "hi");
来源：http://see.9152youxi.cn

[S05] C：字符串长度
来源：http://ufs.guannengcc.top

strlen(s)
来源：http://eqt.shzxlz.cn

[S06] C：字符串比较
来源：http://vva.nanxuanxn.top

strcmp(a, b) == 0
来源：http://yoe.aizwys.cn

[S07] C：数组遍历求和
来源：http://xhl.cqqwz.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dzz.aibaodan.cn

[S08] C：动态内存分配与释放
来源：http://wew.birdmap.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mwf.ctjpmb.com

[S09] C：结构体定义与初始化
来源：http://pvr.redwolf501.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sbo.fanxiaobao.xyz

[S10] C：指针与解引用
来源：http://jgw.sxryk.cn

int *p = &a;  *p = 5;
来源：http://cvm.tian-w.cn

[S11] C：逐行读文件
来源：http://uie.epnwcf.com

FILE *f = fopen("a.txt", "r");
来源：http://sxf.zdqjudy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://pla.pycfn.com

fclose(f);
来源：http://wpb.yongpay.top

[S12] C：写文件
来源：http://ngm.nwbrower.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tmz.shanyushiyangtech.top

[S13] C：宏定义
来源：http://knc.redwolf501.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pve.guannengcc.top

[S14] C：枚举
来源：http://trz.bbcook.cn

enum Color { RED, GREEN, BLUE };
来源：http://sks.sufxvd.cn

[S15] C：类型转换
来源：http://zga.shanyushiyangkeji.top

(double) a / b
来源：http://syk.zdqjudy.top

[S16] C：位操作置位
来源：http://qpg.shanyushiyangkeji.top

x |= (1 << 3);
来源：http://tvs.jiagoushi.top

[S17] C：安全拼接字符串
来源：http://bae.meibo888.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tzg.cdnleiting.top

[S18] C：命令行参数
来源：http://obv.pengpengdd.cyou

int main(int argc, char **argv)
来源：http://lmx.zdbjq.cn

[S19] C：快速排序
来源：http://cgm.cucudq.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vyf.fanxiaobao.xyz

[S20] C：二分查找
来源：http://qgv.ydzc1.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xcc.xinyue.icu

[S21] C：字符类别判断
来源：http://hjb.ydzc1.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dkl.hammf.cn

[S22] C：字符串转数字
来源：http://rzv.aibaodan.cn

atoi("42");  strtod("3.14", NULL);
来源：http://pbw.ydjk.org.cn

[S23] C：随机数
来源：http://gri.316326.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://qkh.fzhhl.top

[S24] C：获取本地时间
来源：http://dmy.guowangkeji.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uhy.yonumen.top

[S25] C：内存拷贝
来源：http://tzh.aizwys.cn

memcpy(dst, src, n);
来源：http://txi.daria6918.cn

[S26] C：内存清零
来源：http://pfg.mhx1999.top

memset(a, 0, sizeof a);
来源：http://njv.chenlongwang.top

[S27] C：定义常量
来源：http://cjc.yuanzhike.top

const double PI = 3.14159;
来源：http://qpd.yj20258888.top

[S28] C：静态变量
来源：http://oaa.xuanzx.com

static int counter = 0;
来源：http://frv.yfazqb.com

[S29] C：变参函数
来源：http://nuw.uphjek.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mhu.tanke756.top

[S30] C：头文件保护
来源：http://fjm.zhaomingkeji.xyz

#ifndef X_H
来源：http://gba.nanxinkj.top

#define X_H
来源：http://zvo.316326.xyz

#endif
来源：http://xkf.redwolf501.top

[S31] C++：Hello World
来源：http://rsi.zhongyouzk.top

#include <iostream>
来源：http://xdw.tanke756.top

int main() { std::cout << "Hello\n"; }
来源：http://ozf.cheryme.top

[S32] C++：字符串
来源：http://sqn.shzxlz.cn

std::string s = "hi";  s += "!";
来源：http://ewu.nanxinkj.top

[S33] C++：vector 增删
来源：http://xof.hcnkem.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://niq.zhiwuduotai.top

[S34] C++：遍历 vector
来源：http://rnf.aizwys.cn

for (auto &x : v) { std::cout << x; }
来源：http://yrn.nanxinkj.top

[S35] C++：map
来源：http://qyy.yj20258888.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gzn.gotoacloud.top

[S36] C++：unordered_map
来源：http://jcp.xziqi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wft.yueranfly.top

[S37] C++：set
来源：http://jbf.ybcxt.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vxz.daxiang520.top

[S38] C++：排序
来源：http://ddw.jinyuanbaomall.cn

std::sort(v.begin(), v.end());
来源：http://hcj.gaohongyu789.top

[S39] C++：自定义比较器排序
来源：http://njb.meibo888.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://toe.vehdjk.com

[S40] C++：查找元素
来源：http://gjk.cucudq.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vgy.316326.xyz

[S41] C++：类与构造函数
来源：http://rsh.jinghuilouyu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zek.meibo888.top

[S42] C++：继承与虚函数
来源：http://ggt.tianlin.xyz

class B : public Base { public: void f() override {} };
来源：http://deh.pycfn.com

[S43] C++：智能指针
来源：http://zxl.jiagoushi.top

auto p = std::make_unique<int>(5);
来源：http://otk.nanxinkj.top

[S44] C++：引用传参
来源：http://ysl.bbcook.cn

void inc(int &x) { ++x; }
来源：http://mzt.pycfn.com

[S45] C++：lambda
来源：http://kso.zhixingplan.top

auto add = [](int a, int b) { return a + b; };
来源：http://ylx.guannengcc.top

[S46] C++：函数模板
来源：http://jnk.haohaochexian.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nsf.yonumen.top

[S47] C++：结构化绑定遍历
来源：http://xvy.zycfv.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://etr.xziqi.cn

[S48] C++：逐行读文件
来源：http://fgy.ydzc1.top

std::ifstream in("a.txt");  std::string line;
来源：http://dbm.smart0.xyz

while (std::getline(in, line)) { }
来源：http://nac.zhixingplan.top

[S49] C++：写文件
来源：http://kpw.gzhubu.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gbv.iojbl.cn

[S50] C++：格式化数字
来源：http://slw.kuanghao11.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cis.jlsjyb.cn

[S51] C++：显式类型转换
来源：http://mff.jlsjyb.cn

static_cast<double>(a) / b
来源：http://ykc.jinqigufen.top

[S52] C++：const 与 noexcept
来源：http://oht.cqqwz.cn

int size() const noexcept { return n_; }
来源：http://kfm.shuidangran.top

[S53] C++：移动语义
来源：http://gab.xuetiantiany.cn

std::vector<int> w = std::move(v);
来源：http://yat.sufxvd.cn

[S54] C++：异常处理
来源：http://tqt.guowangkeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://opi.hesvh.cn

[S55] C++：结构化绑定
来源：http://cya.ybcxt.top

auto [a, b] = std::make_pair(1, 2);
来源：http://rgs.hfpthk.cn

[S56] C++：optional
来源：http://ltg.yfazqb.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xkw.tarul.cn

[S57] C++：编译期常量
来源：http://wnt.nanxuanxn.top

constexpr int N = 10;
来源：http://fra.hesvh.cn

[S58] C++：命名空间
来源：http://jko.shzxlz.cn

namespace ns { int f() { return 1; } }
来源：http://rso.cashguo.top

[S59] C++：静态断言
来源：http://qat.havefunace.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://btw.xylfe.cn

[S60] C++：遍历并删除元素
来源：http://xnp.cheryme.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bge.zhengqikj.top

================================================================================
来源：http://bkn.fktsv.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bww.hysaishi.cn

================================================================================
来源：http://rab.fehbvm.com

[T01] Kotlin：Hello World
来源：http://loi.yueranfly.top

println("Hello")
来源：http://xtq.tanke756.top

[T02] Kotlin：变量
来源：http://lmk.ehwqpu.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yhm.tarul.cn

[T03] Kotlin：字符串模板
来源：http://jnm.jinqigfzy.top

"值: $b"
来源：http://wum.hnxiangtu.top

[T04] Kotlin：空安全
来源：http://elp.gogol.net.cn

val n: String? = null;  n?.length
来源：http://yaz.cdnleiting.top

[T05] Kotlin：when 表达式
来源：http://mxm.tanke756.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lei.sjlbkw.cn

[T06] Kotlin：集合映射
来源：http://jqb.guannengcc.top

listOf(1, 2, 3).map { it * 2 }
来源：http://crj.yongpay.top

[T07] Kotlin：集合过滤
来源：http://oyf.shuidangran.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://nvw.xylfe.cn

[T08] Kotlin：数据类
来源：http://lkf.cucudq.cn

data class User(val name: String, val age: Int)
来源：http://idr.birdmap.top

[T09] Kotlin：扩展函数
来源：http://cpv.wangshuangyany.cn

fun String.exclaim() = this + "!"
来源：http://phq.vehdjk.com

[T10] Kotlin：默认参数
来源：http://aru.yuanzhike.top

fun greet(name: String = "World") = "Hi $name"
来源：http://iou.cucudq.cn

[T11] Kotlin：协程
来源：http://its.pycfn.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://vjj.hnqzz.top

[T12] Kotlin：解构声明
来源：http://zrb.ctjpmb.com

val (a, b) = Pair(1, 2)
来源：http://vbi.nanxinkj.top

[T13] Kotlin：只读 Map
来源：http://vcl.hnqzz.top

val m = mapOf("a" to 1)
来源：http://lbk.pengpengdd.cyou

[T14] Kotlin：循环
来源：http://qaf.shanyushiyangtech.top

for (i in 1..10) println(i)
来源：http://ktu.yj20258.top

[T15] Kotlin：接口
来源：http://rsw.redwolf501.top

interface Shape { fun area(): Double }
来源：http://mgv.yj202588.top

[T16] Swift：Hello World
来源：http://ujy.ctjpmb.com

print("Hello")
来源：http://nxc.xziqi.cn

[T17] Swift：变量与常量
来源：http://zrt.hfpthk.cn

var a = 1;  let b = 2
来源：http://qla.jqgufenzy.top

[T18] Swift：字符串插值
来源：http://ucq.zhijiandao.cn

"值: \(b)"
来源：http://kzv.guannengcc.top

[T19] Swift：可选绑定
来源：http://ngj.birdmap.top

if let n = opt { print(n) }
来源：http://pto.316326.xyz

[T20] Swift：数组操作
来源：http://ztc.mhx1999.top

var a = [1, 2, 3];  a.append(4)
来源：http://trb.zhoulong.xyz

[T21] Swift：遍历
来源：http://kuh.shzxlz.cn

for x in a { print(x) }
来源：http://dpe.jinyuanbaomall.cn

[T22] Swift：字典
来源：http://kee.jinqigfzy.top

var d = ["a": 1];  d["b"] = 2
来源：http://uuu.gaohongyu789.top

[T23] Swift：函数
来源：http://san.yfazqb.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cod.yongpay.top

[T24] Swift：闭包
来源：http://lqh.epnwcf.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://aaz.yuxming.cn

[T25] Swift：结构体
来源：http://gwo.ctjpmb.com

struct P { var x: Int }
来源：http://yww.yj20258.top

[T26] Swift：类与重写
来源：http://svg.chenzaomai.com

class A: Base { override func f() {} }
来源：http://wpr.gogol.net.cn

[T27] Swift：错误处理
来源：http://efp.gzhubu.top

do { try f() } catch { print(error) }
来源：http://syn.kuanghao11.cn

[T28] Swift：枚举
来源：http://lxx.hysaishi.cn

enum Color { case red, green }
来源：http://jwp.hnxiangtu.top

[T29] Swift：guard 提前返回
来源：http://rkg.zdqjudy.top

guard let x = opt else { return }
来源：http://wbq.daxiang520.top

[T30] Swift：协议
来源：http://nkz.bbcook.cn

protocol Shape { func area() -> Double }
来源：http://lzd.ybcxt.top

[T31] Lua：Hello World
来源：http://tex.daxiang520.top

print("Hello")
来源：http://adu.yueranfly.top

[T32] Lua：局部变量
来源：http://mjm.chenzaomai.com

local a = 1
来源：http://mqo.zhoulong.xyz

[T33] Lua：表（数组）
来源：http://tup.fanxiaobao.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://zld.wangdashe.top

[T34] Lua：遍历表
来源：http://jub.cqqwz.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ezu.jyoumei.cn

[T35] Lua：字典表
来源：http://vus.redwolf501.top

local d = { a = 1 };  d.b = 2
来源：http://khk.tanke756.top

[T36] Lua：函数
来源：http://xaw.gotoacloud.top

function add(a, b) return a + b end
来源：http://qcq.kuanghao11.cn


<!-- 参考信息 -->