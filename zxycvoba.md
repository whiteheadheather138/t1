代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yai.shzxlz.cn

[R30] 函数返回状态码
来源：http://rco.smart0.xyz

f() { return 0; }; f || echo "失败了"
来源：http://tpr.cqqwz.cn

[R31] 局部变量
来源：http://csa.nanxuanxn.top

f() { local x=1; echo "$x"; }
来源：http://vnr.ivvv.top

[R32] 参数个数校验
来源：http://mos.nanxuanxn.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bje.tian-w.cn

[R33] 捕获错误并提示行号
来源：http://szf.jlsjyb.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wql.ivvv.top

[R34] 退出时清理
来源：http://zdo.haohaochexian.top

trap 'rm -f "$tmp"' EXIT
来源：http://kby.feifeiyinyue.top

[R35] 后台执行并等待
来源：http://mez.jinghuilouyu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://exb.pycfn.com

[R36] 并发执行多个任务
来源：http://fuu.hongshengwenyu.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cgy.yfazqb.com

[R37] 把输出赋给变量
来源：http://ral.ctjpmb.com

files=$(ls -1)
来源：http://ien.yuxming.cn

[R38] 管道串联
来源：http://xns.yongpay.top

cat a.txt | grep -i error | wc -l
来源：http://axc.hysaishi.cn

[R39] 重定向标准输出与错误
来源：http://lvg.yongpay.top

cmd > out.log 2>&1
来源：http://cil.zycfv.cn

[R40] 追加写日志
来源：http://rkw.ydzc1.top

echo "log" >> out.log
来源：http://mjy.bjfxy.top

[R41] 丢弃输出
来源：http://nmp.epnwcf.com

cmd >/dev/null 2>&1
来源：http://uvs.jiagoushi.top

[R42] 输入重定向
来源：http://tbq.zhoulong.xyz

wc -l < a.txt
来源：http://aht.nanxinkj.top

[R43] 按名字查找文件
来源：http://oly.smart0.xyz

find . -name "*.log" -type f
来源：http://azq.hongshengwenyu.top

[R44] 按修改时间查找
来源：http://fqu.yj20258.top

find . -mtime -7 -type f
来源：http://gee.guannengcc.top

[R45] 批量删除
来源：http://euo.yj202588.top

find . -name "*.tmp" -delete
来源：http://wmh.tianlin.xyz

[R46] 递归替换文件内容
来源：http://gkm.jiagoushi.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pzi.yj20258.top

[R47] sed 单行替换
来源：http://owo.daria6918.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jfv.yangfankeji.com

[R48] awk 取指定列
来源：http://ctu.yfazqb.com

awk '{print $1, $3}' a.txt
来源：http://isb.gzhubu.top

[R49] awk 带条件
来源：http://txf.tanke756.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://clc.zdqjudy.top

[R50] awk 求和
来源：http://ptz.daria6918.cn

awk '{s += $2} END {print s}' a.txt
来源：http://dsa.vehdjk.com

[R51] 排序去重取前几
来源：http://phj.fanxiaobao.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://lsw.hammf.cn

[R52] 统计行数
来源：http://gua.yuxming.cn

wc -l a.txt
来源：http://gvi.shzxlz.cn

[R53] 查看文件头与实时尾
来源：http://fuz.xuetiantiany.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jpo.zdbjq.cn

[R54] 比较两个文件
来源：http://xgo.andypj.xyz

diff a.txt b.txt
来源：http://onm.hysaishi.cn

[R55] 压缩与解压
来源：http://hup.shanyushiyangtech.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lex.redwolf501.top

[R56] 远程拷贝
来源：http://yjd.fehbvm.com

scp file user@host:/path/
来源：http://bto.9152youxi.cn

[R57] 远程执行命令
来源：http://cdy.wangdashe.top

ssh user@host 'uptime'
来源：http://eqn.tian-w.cn

[R58] 下载文件
来源：http://fup.tianlin.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fii.shzxlz.cn

[R59] 发 POST JSON
来源：http://kdv.ctjpmb.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dlt.jinqigfzy.top

[R60] 只看 HTTP 状态码
来源：http://wnm.zdqjudy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xyq.chenlongwang.top

[R61] 磁盘占用
来源：http://dux.chenjidiqi.icu

df -h;  du -sh *
来源：http://rba.xziqi.cn

[R62] 找最占空间的文件
来源：http://wkj.sysykeji.top

du -ah . | sort -rh | head -10
来源：http://xyp.bbcook.cn

[R63] 内存与进程
来源：http://bhy.chenjidiqi.icu

free -h;  ps aux | grep nginx
来源：http://lpt.snrcjt.cn

[R64] 结束进程
来源：http://tbk.yongpay.top

kill -9 $(pgrep -f app.py)
来源：http://you.yuxming.cn

[R65] 查看端口占用
来源：http://qwi.birdmap.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cuk.uphjek.com

[R66] 定时任务
来源：http://jdt.shuidangran.top

crontab -e;  crontab -l
来源：http://lji.guannengcc.top

[R67] 生成随机十六进制串
来源：http://rha.daria6918.cn

openssl rand -hex 16
来源：http://vyl.tanke756.top

[R68] 计算文件校验值
来源：http://nmg.yj20258.top

sha256sum a.txt;  md5sum a.txt
来源：http://dkp.guannengcc.top

[R69] 生成随机密码
来源：http://ywp.cheryme.top

head -c 16 /dev/urandom | base64
来源：http://ado.uphjek.com

[R70] 时间戳与互转
来源：http://frm.0kj1m.cn

date +%s;  date -d @1700000000
来源：http://vmy.dianchejie.cn

[R71] 日期格式化
来源：http://dzg.hnxiangtu.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://riw.aizwys.cn

[R72] 等待端口就绪
来源：http://omt.9152youxi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zsf.yj202588.top

[R73] 分割大日志
来源：http://kgd.pengpengdd.cyou

split -l 1000 big.log part_
来源：http://kyu.cashguo.top

[R74] 批量重命名
来源：http://pnk.tanke756.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yzo.xziqi.cn

[R75] 导出环境变量
来源：http://oeq.jinyuanbaomall.cn

export PATH="$HOME/bin:$PATH"
来源：http://pbk.redwolf501.top

[R76] 使用临时文件
来源：http://rew.xuanzx.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yqd.nwbrower.top

[R77] 读取用户输入
来源：http://oey.bjfxy.top

read -rp "请输入: " ans
来源：http://dey.nwbrower.top

[R78] 交互式菜单
来源：http://cym.hfpthk.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://bcv.daria6918.cn

[R79] 解析命令行选项
来源：http://rvs.sxryk.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://seg.guannengcc.top

[R80] 查看脚本执行耗时
来源：http://xmc.zdqjudy.top

time ./run.sh
来源：http://ioc.aizwys.cn

================================================================================
来源：http://xob.snrcjt.cn

S. C / C++ 专题
来源：http://gph.zhaomingkeji.xyz

================================================================================
来源：http://rax.shanyushiyangtech.top

[S01] C：Hello World
来源：http://ldh.jinghuilouyu.cn

#include <stdio.h>
来源：http://gnu.nanxuanxn.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://dvs.ctjpmb.com

[S02] C：变量与格式化输出
来源：http://cmo.aibaodan.cn

int a = 10; printf("%d\n", a);
来源：http://tcl.guannengcc.top

[S03] C：读入整数
来源：http://snf.sjlbkw.cn

int x; scanf("%d", &x);
来源：http://nbl.pengpengdd.cyou

[S04] C：字符串复制
来源：http://acu.pycfn.com

char dst[32]; strcpy(dst, "hi");
来源：http://hgx.yj20258888.top

[S05] C：字符串长度
来源：http://mzu.jinqigufen.top

strlen(s)
来源：http://fry.iojbl.cn

[S06] C：字符串比较
来源：http://lzv.316326.xyz

strcmp(a, b) == 0
来源：http://rac.52xcode.cn

[S07] C：数组遍历求和
来源：http://qdr.zycfv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://oel.yangfankeji.com

[S08] C：动态内存分配与释放
来源：http://ekc.gogol.net.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mlo.yanxiufei.cn

[S09] C：结构体定义与初始化
来源：http://leq.iojbl.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ytp.sweek.top

[S10] C：指针与解引用
来源：http://gpi.ydjk.org.cn

int *p = &a;  *p = 5;
来源：http://guj.gzhubu.top

[S11] C：逐行读文件
来源：http://rqp.jqgufenzy.top

FILE *f = fopen("a.txt", "r");
来源：http://rff.chenzaomai.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://evd.vqdsnc.cn

fclose(f);
来源：http://xfi.hfpthk.cn

[S12] C：写文件
来源：http://uzd.jqgufenzy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://njv.tarul.cn

[S13] C：宏定义
来源：http://jri.hnxiangtu.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cal.hongshengwenyu.top

[S14] C：枚举
来源：http://fbf.bbcook.cn

enum Color { RED, GREEN, BLUE };
来源：http://hkp.tian-w.cn

[S15] C：类型转换
来源：http://ltt.fanxiaobao.xyz

(double) a / b
来源：http://pxk.wangshuangyany.cn

[S16] C：位操作置位
来源：http://fon.yj20258.top

x |= (1 << 3);
来源：http://cca.haohaochexian.top

[S17] C：安全拼接字符串
来源：http://hsp.zdbjq.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wnh.zdbjq.cn

[S18] C：命令行参数
来源：http://jik.9152youxi.cn

int main(int argc, char **argv)
来源：http://xze.zhengqikj.top

[S19] C：快速排序
来源：http://rgc.smart0.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://gzj.xinyue.icu

[S20] C：二分查找
来源：http://kju.havefunace.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://isp.gogol.net.cn

[S21] C：字符类别判断
来源：http://lze.ctjpmb.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yqe.yonumen.top

[S22] C：字符串转数字
来源：http://xtu.sxryk.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xsz.cheryme.top

[S23] C：随机数
来源：http://eus.jinghuilouyu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qtp.snrcjt.cn

[S24] C：获取本地时间
来源：http://egu.yanxiufei.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qzo.hesvh.cn

[S25] C：内存拷贝
来源：http://elx.daria6918.cn

memcpy(dst, src, n);
来源：http://nzq.chenjidiqi.icu

[S26] C：内存清零
来源：http://xtf.guowangkeji.top

memset(a, 0, sizeof a);
来源：http://yns.0kj1m.cn

[S27] C：定义常量
来源：http://qcz.svipenyu.cn

const double PI = 3.14159;
来源：http://mul.9152youxi.cn

[S28] C：静态变量
来源：http://ghk.zhongyouzk.top

static int counter = 0;
来源：http://tsb.sysykeji.top

[S29] C：变参函数
来源：http://bqi.gotoacloud.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://apm.yonumen.top

[S30] C：头文件保护
来源：http://rqr.meibo888.top

#ifndef X_H
来源：http://ttp.xinyue.icu

#define X_H
来源：http://dtv.uphjek.com

#endif
来源：http://wqx.jyoumei.cn

[S31] C++：Hello World
来源：http://mif.ppjwa.cn

#include <iostream>
来源：http://kww.yanxiufei.cn

int main() { std::cout << "Hello\n"; }
来源：http://ouo.fanxiaobao.xyz

[S32] C++：字符串
来源：http://xcr.xuanzx.com

std::string s = "hi";  s += "!";
来源：http://meg.hywenlv.cn

[S33] C++：vector 增删
来源：http://aln.iojbl.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hle.hcnkem.com

[S34] C++：遍历 vector
来源：http://nwq.jianghu66.top

for (auto &x : v) { std::cout << x; }
来源：http://nnd.pengpengdd.cyou

[S35] C++：map
来源：http://llv.zhengqikj.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bki.chenlongwang.top

[S36] C++：unordered_map
来源：http://uqh.zhijiandao.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://khm.jlsjyb.cn

[S37] C++：set
来源：http://nfh.c1oappe.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kkb.zhijiandao.cn

[S38] C++：排序
来源：http://jul.jinyuanbaomall.cn

std::sort(v.begin(), v.end());
来源：http://zrb.9152youxi.cn

[S39] C++：自定义比较器排序
来源：http://rzj.jinqigfzy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pbi.cheryme.top

[S40] C++：查找元素
来源：http://jot.zhijiandao.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fzi.jyoumei.cn

[S41] C++：类与构造函数
来源：http://duj.xylfe.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jcx.shanyushiyangkeji.top

[S42] C++：继承与虚函数
来源：http://nvy.hongshengwenyu.top

class B : public Base { public: void f() override {} };
来源：http://smo.zhongyouzk.top

[S43] C++：智能指针
来源：http://zri.ppjwa.cn

auto p = std::make_unique<int>(5);
来源：http://qlz.fzhhl.top

[S44] C++：引用传参
来源：http://spa.hammf.cn

void inc(int &x) { ++x; }
来源：http://dti.gzhubu.top

[S45] C++：lambda
来源：http://ipu.hnqzz.top

auto add = [](int a, int b) { return a + b; };
来源：http://rck.0kj1m.cn

[S46] C++：函数模板
来源：http://hwb.andypj.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://itr.aibaodan.cn

[S47] C++：结构化绑定遍历
来源：http://ucx.sxryk.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bxa.ydjk.org.cn

[S48] C++：逐行读文件
来源：http://cqd.nanxinkj.top

std::ifstream in("a.txt");  std::string line;
来源：http://bdg.birdmap.top

while (std::getline(in, line)) { }
来源：http://amt.bjfxy.top

[S49] C++：写文件
来源：http://nrn.cheryme.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ngp.pengpengdd.cyou

[S50] C++：格式化数字
来源：http://kyj.yfazqb.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://emm.smart0.xyz

[S51] C++：显式类型转换
来源：http://rjy.shzxlz.cn

static_cast<double>(a) / b
来源：http://qkr.daria6918.cn

[S52] C++：const 与 noexcept
来源：http://hpi.jiagoushi.top

int size() const noexcept { return n_; }
来源：http://mvd.zhoulong.xyz

[S53] C++：移动语义
来源：http://qvl.zdqjudy.top

std::vector<int> w = std::move(v);
来源：http://dch.yongpay.top

[S54] C++：异常处理
来源：http://jcc.birdmap.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://duf.zhijiandao.cn

[S55] C++：结构化绑定
来源：http://lyr.epnwcf.com

auto [a, b] = std::make_pair(1, 2);
来源：http://kcd.sysykeji.top

[S56] C++：optional
来源：http://oyf.vehdjk.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://aot.tarul.cn

[S57] C++：编译期常量
来源：http://rfr.shanyushiyangtech.top

constexpr int N = 10;
来源：http://txp.zdqjudy.top

[S58] C++：命名空间
来源：http://fgi.tian-w.cn

namespace ns { int f() { return 1; } }
来源：http://anb.chenlongwang.top

[S59] C++：静态断言
来源：http://txj.guannengcc.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rdq.kuanghao11.cn

[S60] C++：遍历并删除元素
来源：http://oki.zhengqikj.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ljp.hammf.cn

================================================================================
来源：http://gge.kuanghao11.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lvl.havefunace.top

================================================================================
来源：http://xul.yuxming.cn

[T01] Kotlin：Hello World
来源：http://hgo.chenzaomai.com

println("Hello")
来源：http://ewz.aibaodan.cn

[T02] Kotlin：变量
来源：http://nuf.shangyingyoupin.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dyn.hnqzz.top

[T03] Kotlin：字符串模板
来源：http://jqa.wangshuangyany.cn

"值: $b"
来源：http://ouc.haohaochexian.top

[T04] Kotlin：空安全
来源：http://qgx.hnqzz.top

val n: String? = null;  n?.length
来源：http://yee.daria6918.cn

[T05] Kotlin：when 表达式
来源：http://jpb.shangyingyoupin.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://waa.xinyue.icu

[T06] Kotlin：集合映射
来源：http://pke.kuanghao11.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://czo.hesvh.cn

[T07] Kotlin：集合过滤
来源：http://bww.zhaomingkeji.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://iua.shanyushiyangkeji.top

[T08] Kotlin：数据类
来源：http://len.sweek.top

data class User(val name: String, val age: Int)
来源：http://wyt.yfazqb.com

[T09] Kotlin：扩展函数
来源：http://njz.shangyingyoupin.top

fun String.exclaim() = this + "!"
来源：http://vsi.jqgfzy.top

[T10] Kotlin：默认参数
来源：http://ylt.xylfe.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vmi.daxiang520.top

[T11] Kotlin：协程
来源：http://ijd.yanxiufei.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://lvg.ctjpmb.com

[T12] Kotlin：解构声明
来源：http://dyo.52xcode.cn

val (a, b) = Pair(1, 2)
来源：http://btm.yonumen.top

[T13] Kotlin：只读 Map
来源：http://ufx.cashguo.top

val m = mapOf("a" to 1)
来源：http://eto.zhiwuduotai.top

[T14] Kotlin：循环
来源：http://prj.wangshuangyany.cn

for (i in 1..10) println(i)
来源：http://gvo.sxryk.cn

[T15] Kotlin：接口
来源：http://sbt.daxiang520.top

interface Shape { fun area(): Double }
来源：http://lbl.tian-w.cn

[T16] Swift：Hello World
来源：http://ifa.hammf.cn

print("Hello")
来源：http://fep.smart0.xyz

[T17] Swift：变量与常量
来源：http://lba.316326.xyz

var a = 1;  let b = 2
来源：http://fil.andypj.xyz

[T18] Swift：字符串插值
来源：http://kfl.yj20258888.top

"值: \(b)"
来源：http://jhw.snrcjt.cn

[T19] Swift：可选绑定
来源：http://ltf.gaohongyu789.top

if let n = opt { print(n) }
来源：http://qzr.yanxiufei.cn

[T20] Swift：数组操作
来源：http://cbm.yuxming.cn

var a = [1, 2, 3];  a.append(4)
来源：http://lbs.yuxming.cn

[T21] Swift：遍历
来源：http://son.smart0.xyz

for x in a { print(x) }
来源：http://qxl.hywenlv.cn

[T22] Swift：字典
来源：http://myu.ppjwa.cn

var d = ["a": 1];  d["b"] = 2
来源：http://dyi.zhiwuduotai.top

[T23] Swift：函数
来源：http://yvj.jqgfzy.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vvb.zhaomingkeji.xyz

[T24] Swift：闭包
来源：http://fty.xinyue.icu

let f = { (x: Int) -> Int in x * 2 }
来源：http://jdm.9152youxi.cn

[T25] Swift：结构体
来源：http://spf.quarkkingdee.top

struct P { var x: Int }
来源：http://jth.hnqzz.top

[T26] Swift：类与重写
来源：http://shq.guowangkeji.top

class A: Base { override func f() {} }
来源：http://wqp.jqgufenzy.top

[T27] Swift：错误处理
来源：http://arj.hnxiangtu.top

do { try f() } catch { print(error) }
来源：http://nal.zhijiandao.cn

[T28] Swift：枚举
来源：http://pdh.tanke756.top

enum Color { case red, green }
来源：http://hzm.jlsjyb.cn

[T29] Swift：guard 提前返回
来源：http://art.hnxiangtu.top

guard let x = opt else { return }
来源：http://ohz.fanxiaobao.xyz

[T30] Swift：协议
来源：http://bmu.redwolf501.top

protocol Shape { func area() -> Double }
来源：http://srm.zycfv.cn

[T31] Lua：Hello World
来源：http://mja.hnqzz.top

print("Hello")
来源：http://fac.nanxuanxn.top

[T32] Lua：局部变量
来源：http://jtx.nanxinkj.top

local a = 1
来源：http://ael.yvedp.cn


<!-- 参考信息 -->