代发 wailian999

echo $((1 + 2 * 3))
来源：http://eko.daria6918.cn

[R28] 浮点运算
来源：http://ptz.cashguo.top

echo "scale=2; 10/3" | bc
来源：http://ayy.aibaodan.cn

[R29] 定义函数
来源：http://ssh.kuanghao11.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rpd.tian-w.cn

[R30] 函数返回状态码
来源：http://qzc.ydzc1.top

f() { return 0; }; f || echo "失败了"
来源：http://gse.hammf.cn

[R31] 局部变量
来源：http://hsk.zhixingplan.top

f() { local x=1; echo "$x"; }
来源：http://gmc.tianlin.xyz

[R32] 参数个数校验
来源：http://oly.haohaochexian.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ras.daxiang520.top

[R33] 捕获错误并提示行号
来源：http://gjz.uphjek.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ipp.zdbjq.cn

[R34] 退出时清理
来源：http://mip.birdmap.top

trap 'rm -f "$tmp"' EXIT
来源：http://opa.tian-w.cn

[R35] 后台执行并等待
来源：http://rac.zdbjq.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xmx.hysaishi.cn

[R36] 并发执行多个任务
来源：http://qoh.xingfuxueyuan.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://byy.sysykeji.top

[R37] 把输出赋给变量
来源：http://klo.nwbrower.top

files=$(ls -1)
来源：http://nsf.fehbvm.com

[R38] 管道串联
来源：http://dmg.fktsv.cn

cat a.txt | grep -i error | wc -l
来源：http://nac.zhijiandao.cn

[R39] 重定向标准输出与错误
来源：http://ywr.ctjpmb.com

cmd > out.log 2>&1
来源：http://vvo.ehwqpu.com

[R40] 追加写日志
来源：http://ert.ctjpmb.com

echo "log" >> out.log
来源：http://cow.yuxming.cn

[R41] 丢弃输出
来源：http://jba.xziqi.cn

cmd >/dev/null 2>&1
来源：http://ter.meibo888.top

[R42] 输入重定向
来源：http://ayy.chenjidiqi.icu

wc -l < a.txt
来源：http://okr.jiagoushi.top

[R43] 按名字查找文件
来源：http://pkw.zhongyouzk.top

find . -name "*.log" -type f
来源：http://fvc.zhiwuduotai.top

[R44] 按修改时间查找
来源：http://teh.zdqjudy.top

find . -mtime -7 -type f
来源：http://udo.sufxvd.cn

[R45] 批量删除
来源：http://rjn.fanxiaobao.xyz

find . -name "*.tmp" -delete
来源：http://juy.ivvv.top

[R46] 递归替换文件内容
来源：http://ptk.tanke756.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://chz.yj20258.top

[R47] sed 单行替换
来源：http://yeg.yangfankeji.com

sed -i 's/foo/bar/g' a.txt
来源：http://lyy.zhaomingkeji.xyz

[R48] awk 取指定列
来源：http://rvs.0kj1m.cn

awk '{print $1, $3}' a.txt
来源：http://kbm.hammf.cn

[R49] awk 带条件
来源：http://tkc.yangfankeji.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yhx.zhijiandao.cn

[R50] awk 求和
来源：http://aoc.jqgufenzy.top

awk '{s += $2} END {print s}' a.txt
来源：http://lsp.zdbjq.cn

[R51] 排序去重取前几
来源：http://vsh.birdmap.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ajj.jyoumei.cn

[R52] 统计行数
来源：http://wbm.52xcode.cn

wc -l a.txt
来源：http://svz.ehwqpu.com

[R53] 查看文件头与实时尾
来源：http://ggx.quarkkingdee.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ffb.tarul.cn

[R54] 比较两个文件
来源：http://vct.shzxlz.cn

diff a.txt b.txt
来源：http://ubn.jinqigufen.top

[R55] 压缩与解压
来源：http://qzz.wangdashe.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ezy.andypj.xyz

[R56] 远程拷贝
来源：http://zjt.shzxlz.cn

scp file user@host:/path/
来源：http://jom.sweek.top

[R57] 远程执行命令
来源：http://pjp.pengpengdd.cyou

ssh user@host 'uptime'
来源：http://dmz.sufxvd.cn

[R58] 下载文件
来源：http://cwj.xingfuxueyuan.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://izv.daxiang520.top

[R59] 发 POST JSON
来源：http://uas.pengpengdd.cyou

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ily.jqgufenzy.top

[R60] 只看 HTTP 状态码
来源：http://azt.tianlin.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://svy.ywan-chungtsiang.top

[R61] 磁盘占用
来源：http://hxq.quarkkingdee.top

df -h;  du -sh *
来源：http://yrk.jianghu66.top

[R62] 找最占空间的文件
来源：http://csv.xylfe.cn

du -ah . | sort -rh | head -10
来源：http://clo.316326.xyz

[R63] 内存与进程
来源：http://xzb.yonumen.top

free -h;  ps aux | grep nginx
来源：http://gqt.c1oappe.top

[R64] 结束进程
来源：http://pds.tianlin.xyz

kill -9 $(pgrep -f app.py)
来源：http://ugd.cheryme.top

[R65] 查看端口占用
来源：http://eqx.shzxlz.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wmv.hywenlv.cn

[R66] 定时任务
来源：http://ykg.iojbl.cn

crontab -e;  crontab -l
来源：http://ywc.sweek.top

[R67] 生成随机十六进制串
来源：http://dmk.sxryk.cn

openssl rand -hex 16
来源：http://wcn.iojbl.cn

[R68] 计算文件校验值
来源：http://oty.quarkkingdee.top

sha256sum a.txt;  md5sum a.txt
来源：http://wsm.bjfxy.top

[R69] 生成随机密码
来源：http://goa.cucudq.cn

head -c 16 /dev/urandom | base64
来源：http://eud.hesvh.cn

[R70] 时间戳与互转
来源：http://lbe.xuanzx.com

date +%s;  date -d @1700000000
来源：http://hoy.shzxlz.cn

[R71] 日期格式化
来源：http://hag.daria6918.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://yzb.dashuyun.cn

[R72] 等待端口就绪
来源：http://nzb.nwbrower.top

until nc -z localhost 3306; do sleep 1; done
来源：http://son.haohaochexian.top

[R73] 分割大日志
来源：http://cxk.sxryk.cn

split -l 1000 big.log part_
来源：http://pie.jyoumei.cn

[R74] 批量重命名
来源：http://aec.guannengcc.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hdf.zhengqikj.top

[R75] 导出环境变量
来源：http://mud.svipenyu.cn

export PATH="$HOME/bin:$PATH"
来源：http://rbd.0kj1m.cn

[R76] 使用临时文件
来源：http://rva.52xcode.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ckq.hywenlv.cn

[R77] 读取用户输入
来源：http://pux.cdnleiting.top

read -rp "请输入: " ans
来源：http://etv.ivvv.top

[R78] 交互式菜单
来源：http://bbx.aibaodan.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ucx.hysaishi.cn

[R79] 解析命令行选项
来源：http://jlh.shuidangran.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://frb.xylfe.cn

[R80] 查看脚本执行耗时
来源：http://jtr.yueranfly.top

time ./run.sh
来源：http://lhg.ivvv.top

================================================================================
来源：http://hks.yanxiufei.cn

S. C / C++ 专题
来源：http://exu.chenlongwang.top

================================================================================
来源：http://ofw.cdnleiting.top

[S01] C：Hello World
来源：http://rko.pycfn.com

#include <stdio.h>
来源：http://aiw.zdbjq.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://beg.chenjidiqi.icu

[S02] C：变量与格式化输出
来源：http://uac.yvedp.cn

int a = 10; printf("%d\n", a);
来源：http://awy.birdmap.top

[S03] C：读入整数
来源：http://dzo.hongshengwenyu.top

int x; scanf("%d", &x);
来源：http://cvh.iojbl.cn

[S04] C：字符串复制
来源：http://mwa.cdnleiting.top

char dst[32]; strcpy(dst, "hi");
来源：http://phv.vehdjk.com

[S05] C：字符串长度
来源：http://qvk.aibaodan.cn

strlen(s)
来源：http://atd.ywan-chungtsiang.top

[S06] C：字符串比较
来源：http://vyj.zycfv.cn

strcmp(a, b) == 0
来源：http://esq.yj202588.top

[S07] C：数组遍历求和
来源：http://elw.nwbrower.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kef.gaohongyu789.top

[S08] C：动态内存分配与释放
来源：http://ndd.nanxuanxn.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cug.hnxiangtu.top

[S09] C：结构体定义与初始化
来源：http://xpr.chenzaomai.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jwp.andypj.xyz

[S10] C：指针与解引用
来源：http://euo.shuidangran.top

int *p = &a;  *p = 5;
来源：http://ovm.iojbl.cn

[S11] C：逐行读文件
来源：http://rfa.snrcjt.cn

FILE *f = fopen("a.txt", "r");
来源：http://jgv.redwolf501.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://wfj.gaohongyu789.top

fclose(f);
来源：http://usp.gogol.net.cn

[S12] C：写文件
来源：http://epm.dianchejie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tyr.ivvv.top

[S13] C：宏定义
来源：http://brk.zhongyouzk.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://txx.daria6918.cn

[S14] C：枚举
来源：http://vsw.fanxiaobao.xyz

enum Color { RED, GREEN, BLUE };
来源：http://fdq.fanxiaobao.xyz

[S15] C：类型转换
来源：http://xmb.tianlin.xyz

(double) a / b
来源：http://sxj.wangdashe.top

[S16] C：位操作置位
来源：http://gmu.fehbvm.com

x |= (1 << 3);
来源：http://xzl.hammf.cn

[S17] C：安全拼接字符串
来源：http://eqv.chenjidiqi.icu

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lqg.svipenyu.cn

[S18] C：命令行参数
来源：http://pyu.hywenlv.cn

int main(int argc, char **argv)
来源：http://fyv.tanke756.top

[S19] C：快速排序
来源：http://nny.tarul.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fvq.dianchejie.cn

[S20] C：二分查找
来源：http://mdq.ywan-chungtsiang.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zcz.xylfe.cn

[S21] C：字符类别判断
来源：http://bzo.xuetiantiany.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ncz.mhx1999.top

[S22] C：字符串转数字
来源：http://ijb.gaohongyu789.top

atoi("42");  strtod("3.14", NULL);
来源：http://dga.jinqigfzy.top

[S23] C：随机数
来源：http://mmj.kuanghao11.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xzv.birdmap.top

[S24] C：获取本地时间
来源：http://dke.shangyingyoupin.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://szc.gaohongyu789.top

[S25] C：内存拷贝
来源：http://cwr.jinghuilouyu.cn

memcpy(dst, src, n);
来源：http://xmp.gogol.net.cn

[S26] C：内存清零
来源：http://umz.birdmap.top

memset(a, 0, sizeof a);
来源：http://uhs.hesvh.cn

[S27] C：定义常量
来源：http://axg.xuetiantiany.cn

const double PI = 3.14159;
来源：http://uth.tarul.cn

[S28] C：静态变量
来源：http://msp.cqqwz.cn

static int counter = 0;
来源：http://whv.gaohongyu789.top

[S29] C：变参函数
来源：http://etx.c1oappe.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cnm.hfpthk.cn

[S30] C：头文件保护
来源：http://jaz.jyoumei.cn

#ifndef X_H
来源：http://riv.shanyushiyangtech.top

#define X_H
来源：http://thn.feifeiyinyue.top

#endif
来源：http://phv.shuidangran.top

[S31] C++：Hello World
来源：http://grl.yongpay.top

#include <iostream>
来源：http://xho.yonumen.top

int main() { std::cout << "Hello\n"; }
来源：http://tww.yonumen.top

[S32] C++：字符串
来源：http://rde.yueranfly.top

std::string s = "hi";  s += "!";
来源：http://uwy.zdbjq.cn

[S33] C++：vector 增删
来源：http://rcd.meibo888.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ovd.hnxiangtu.top

[S34] C++：遍历 vector
来源：http://hcx.yuxming.cn

for (auto &x : v) { std::cout << x; }
来源：http://qbn.daria6918.cn

[S35] C++：map
来源：http://lxc.cqqwz.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gij.zycfv.cn

[S36] C++：unordered_map
来源：http://sax.chenjidiqi.icu

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ics.havefunace.top

[S37] C++：set
来源：http://cck.ywan-chungtsiang.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://adr.shanyushiyangtech.top

[S38] C++：排序
来源：http://azy.hfpthk.cn

std::sort(v.begin(), v.end());
来源：http://jad.chenzaomai.com

[S39] C++：自定义比较器排序
来源：http://yni.tanke756.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nua.aizwys.cn

[S40] C++：查找元素
来源：http://usq.jianghu66.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://upv.ivvv.top

[S41] C++：类与构造函数
来源：http://jip.cqqwz.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://krr.fktsv.cn

[S42] C++：继承与虚函数
来源：http://ays.nwbrower.top

class B : public Base { public: void f() override {} };
来源：http://ghd.bbcook.cn

[S43] C++：智能指针
来源：http://epx.dashuyun.cn

auto p = std::make_unique<int>(5);
来源：http://lgz.xuetiantiany.cn

[S44] C++：引用传参
来源：http://cmk.hywenlv.cn

void inc(int &x) { ++x; }
来源：http://tog.jlsjyb.cn

[S45] C++：lambda
来源：http://gmb.sxryk.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zsu.zdbjq.cn

[S46] C++：函数模板
来源：http://fic.yangfankeji.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jhp.aizwys.cn

[S47] C++：结构化绑定遍历
来源：http://hip.316326.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xve.cqqwz.cn

[S48] C++：逐行读文件
来源：http://wbj.nanxuanxn.top

std::ifstream in("a.txt");  std::string line;
来源：http://fel.cashguo.top

while (std::getline(in, line)) { }
来源：http://jak.yangfankeji.com

[S49] C++：写文件
来源：http://osx.hesvh.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fqo.shangyingyoupin.top

[S50] C++：格式化数字
来源：http://dwo.jinqigfzy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ngn.ppjwa.cn

[S51] C++：显式类型转换
来源：http://kug.tarul.cn

static_cast<double>(a) / b
来源：http://uyd.tian-w.cn

[S52] C++：const 与 noexcept
来源：http://ecc.dianchejie.cn

int size() const noexcept { return n_; }
来源：http://txm.52xcode.cn

[S53] C++：移动语义
来源：http://pzq.0kj1m.cn

std::vector<int> w = std::move(v);
来源：http://mkl.bbcook.cn

[S54] C++：异常处理
来源：http://pqk.cashguo.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hwa.52xcode.cn

[S55] C++：结构化绑定
来源：http://hbz.jqgufenzy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://jzu.fengsongda.top

[S56] C++：optional
来源：http://qqe.smart0.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yal.chenlongwang.top

[S57] C++：编译期常量
来源：http://oav.dianchejie.cn

constexpr int N = 10;
来源：http://fur.guowangkeji.top

[S58] C++：命名空间
来源：http://zsg.sweek.top

namespace ns { int f() { return 1; } }
来源：http://bwv.svipenyu.cn

[S59] C++：静态断言
来源：http://jsg.fengsongda.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qeu.ywan-chungtsiang.top

[S60] C++：遍历并删除元素
来源：http://odg.hfpthk.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pdc.zhijiandao.cn

================================================================================
来源：http://olc.yj20258.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://abh.shangyingyoupin.top

================================================================================
来源：http://ege.nanxuanxn.top

[T01] Kotlin：Hello World
来源：http://wea.xziqi.cn

println("Hello")
来源：http://xwt.sufxvd.cn

[T02] Kotlin：变量
来源：http://vox.chenzaomai.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mub.pengpengdd.cyou

[T03] Kotlin：字符串模板
来源：http://lwb.yueranfly.top

"值: $b"
来源：http://ilu.xziqi.cn

[T04] Kotlin：空安全
来源：http://pdp.ppjwa.cn

val n: String? = null;  n?.length
来源：http://ndg.andypj.xyz

[T05] Kotlin：when 表达式
来源：http://hgh.jyoumei.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zum.xingfuxueyuan.xyz

[T06] Kotlin：集合映射
来源：http://crg.ybcxt.top

listOf(1, 2, 3).map { it * 2 }
来源：http://rvg.0kj1m.cn

[T07] Kotlin：集合过滤
来源：http://asu.jyoumei.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qra.yanxiufei.cn

[T08] Kotlin：数据类
来源：http://dbn.jianghu66.top

data class User(val name: String, val age: Int)
来源：http://sel.xinyue.icu

[T09] Kotlin：扩展函数
来源：http://lxd.redwolf501.top

fun String.exclaim() = this + "!"
来源：http://hdy.shanyushiyangtech.top

[T10] Kotlin：默认参数
来源：http://fnv.dianchejie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://bub.shzxlz.cn

[T11] Kotlin：协程
来源：http://ueg.zhengqikj.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://pqr.ppjwa.cn

[T12] Kotlin：解构声明
来源：http://tml.zhijiandao.cn

val (a, b) = Pair(1, 2)
来源：http://ekr.nwbrower.top

[T13] Kotlin：只读 Map
来源：http://rok.fehbvm.com

val m = mapOf("a" to 1)
来源：http://hqn.chenlongwang.top

[T14] Kotlin：循环
来源：http://ryq.shanyushiyangtech.top

for (i in 1..10) println(i)
来源：http://tkm.xuetiantiany.cn

[T15] Kotlin：接口
来源：http://bdw.fanxiaobao.xyz

interface Shape { fun area(): Double }
来源：http://uie.cucudq.cn

[T16] Swift：Hello World
来源：http://qvq.birdmap.top

print("Hello")
来源：http://qfj.guowangkeji.top

[T17] Swift：变量与常量
来源：http://sis.guowangkeji.top

var a = 1;  let b = 2
来源：http://cag.tanke756.top

[T18] Swift：字符串插值
来源：http://ijg.hnqzz.top

"值: \(b)"
来源：http://dwc.ctjpmb.com

[T19] Swift：可选绑定
来源：http://nrd.wangshuangyany.cn

if let n = opt { print(n) }
来源：http://vph.jinyuanbaomall.cn

[T20] Swift：数组操作
来源：http://uhu.vehdjk.com

var a = [1, 2, 3];  a.append(4)
来源：http://rxz.hysaishi.cn

[T21] Swift：遍历
来源：http://bgp.redwolf501.top

for x in a { print(x) }
来源：http://lvc.meibo888.top

[T22] Swift：字典
来源：http://fuh.hongshengwenyu.top

var d = ["a": 1];  d["b"] = 2
来源：http://qud.yonumen.top

[T23] Swift：函数
来源：http://wol.jiagoushi.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gxw.gzhubu.top

[T24] Swift：闭包
来源：http://onp.ppjwa.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://mhb.52xcode.cn

[T25] Swift：结构体
来源：http://wwg.feifeiyinyue.top

struct P { var x: Int }
来源：http://aek.ydjk.org.cn

[T26] Swift：类与重写
来源：http://tnx.nwbrower.top

class A: Base { override func f() {} }
来源：http://hfb.hammf.cn

[T27] Swift：错误处理
来源：http://nqe.dianchejie.cn

do { try f() } catch { print(error) }
来源：http://pym.guannengcc.top

[T28] Swift：枚举
来源：http://clo.nanxinkj.top

enum Color { case red, green }
来源：http://mje.hywenlv.cn

[T29] Swift：guard 提前返回
来源：http://ynk.zdqjudy.top

guard let x = opt else { return }
来源：http://mqw.zdqjudy.top

[T30] Swift：协议
来源：http://zxm.kuanghao11.cn

protocol Shape { func area() -> Double }
来源：http://vra.ppjwa.cn


<!-- 参考信息 -->