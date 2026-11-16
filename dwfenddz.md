代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zhk.andypj.xyz

[R24] 大小写转换
来源：http://ynp.ppjwa.cn

echo "${s^^}"; echo "${s,,}"
来源：http://kel.zhiwuduotai.top

[R25] 去后缀 / 去前缀
来源：http://ixx.svipenyu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://dhk.zhijiandao.cn

[R26] 命令替换
来源：http://uig.zdqjudy.top

now=$(date +%F); echo "$now"
来源：http://kix.jinqigufen.top

[R27] 算术展开
来源：http://hrs.yonumen.top

echo $((1 + 2 * 3))
来源：http://bab.hywenlv.cn

[R28] 浮点运算
来源：http://jcf.jinghuilouyu.cn

echo "scale=2; 10/3" | bc
来源：http://fsn.quarkkingdee.top

[R29] 定义函数
来源：http://lxg.redwolf501.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tvf.ybcxt.top

[R30] 函数返回状态码
来源：http://qna.chenzaomai.com

f() { return 0; }; f || echo "失败了"
来源：http://ezx.shanyushiyangkeji.top

[R31] 局部变量
来源：http://epz.nanxinkj.top

f() { local x=1; echo "$x"; }
来源：http://kjo.dashuyun.cn

[R32] 参数个数校验
来源：http://yhv.zhoulong.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zxz.havefunace.top

[R33] 捕获错误并提示行号
来源：http://hns.guannengcc.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://grq.dashuyun.cn

[R34] 退出时清理
来源：http://kdg.hammf.cn

trap 'rm -f "$tmp"' EXIT
来源：http://eha.tian-w.cn

[R35] 后台执行并等待
来源：http://zcq.hesvh.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xwu.yueranfly.top

[R36] 并发执行多个任务
来源：http://bcr.yj20258.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cnl.xuetiantiany.cn

[R37] 把输出赋给变量
来源：http://nms.chenjidiqi.icu

files=$(ls -1)
来源：http://ipf.yvedp.cn

[R38] 管道串联
来源：http://tnx.iojbl.cn

cat a.txt | grep -i error | wc -l
来源：http://ltd.jinghuilouyu.cn

[R39] 重定向标准输出与错误
来源：http://zfu.andypj.xyz

cmd > out.log 2>&1
来源：http://pid.yj20258.top

[R40] 追加写日志
来源：http://fkc.gogol.net.cn

echo "log" >> out.log
来源：http://qmn.snrcjt.cn

[R41] 丢弃输出
来源：http://zso.vehdjk.com

cmd >/dev/null 2>&1
来源：http://ekb.xylfe.cn

[R42] 输入重定向
来源：http://tyh.cdnleiting.top

wc -l < a.txt
来源：http://rqs.nanxuanxn.top

[R43] 按名字查找文件
来源：http://oma.nanxinkj.top

find . -name "*.log" -type f
来源：http://ayn.jyoumei.cn

[R44] 按修改时间查找
来源：http://wnm.jlsjyb.cn

find . -mtime -7 -type f
来源：http://qmq.bbcook.cn

[R45] 批量删除
来源：http://trx.yuanzhike.top

find . -name "*.tmp" -delete
来源：http://dzs.sxryk.cn

[R46] 递归替换文件内容
来源：http://tma.gogol.net.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://scq.quarkkingdee.top

[R47] sed 单行替换
来源：http://ibc.ywan-chungtsiang.top

sed -i 's/foo/bar/g' a.txt
来源：http://fha.cashguo.top

[R48] awk 取指定列
来源：http://bjn.sufxvd.cn

awk '{print $1, $3}' a.txt
来源：http://sfl.yj20258888.top

[R49] awk 带条件
来源：http://sgx.yongpay.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ros.wangdashe.top

[R50] awk 求和
来源：http://fft.birdmap.top

awk '{s += $2} END {print s}' a.txt
来源：http://wxq.shanyushiyangtech.top

[R51] 排序去重取前几
来源：http://pdr.zhixingplan.top

sort a.txt | uniq -c | sort -rn | head
来源：http://tll.nanxinkj.top

[R52] 统计行数
来源：http://rha.yvedp.cn

wc -l a.txt
来源：http://pze.yonumen.top

[R53] 查看文件头与实时尾
来源：http://wcy.hywenlv.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tgw.316326.xyz

[R54] 比较两个文件
来源：http://hmw.daxiang520.top

diff a.txt b.txt
来源：http://fhv.hywenlv.cn

[R55] 压缩与解压
来源：http://oqj.jiagoushi.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yjm.uphjek.com

[R56] 远程拷贝
来源：http://epv.feifeiyinyue.top

scp file user@host:/path/
来源：http://fay.316326.xyz

[R57] 远程执行命令
来源：http://nrg.pengpengdd.cyou

ssh user@host 'uptime'
来源：http://zaa.sxryk.cn

[R58] 下载文件
来源：http://ipy.xuetiantiany.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xbn.pengpengdd.cyou

[R59] 发 POST JSON
来源：http://mzi.pycfn.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xxm.jinqigfzy.top

[R60] 只看 HTTP 状态码
来源：http://ykz.jqgfzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://srn.yfazqb.com

[R61] 磁盘占用
来源：http://blc.sweek.top

df -h;  du -sh *
来源：http://ske.c1oappe.top

[R62] 找最占空间的文件
来源：http://iuu.nanxinkj.top

du -ah . | sort -rh | head -10
来源：http://tlb.redwolf501.top

[R63] 内存与进程
来源：http://nlr.xuetiantiany.cn

free -h;  ps aux | grep nginx
来源：http://zwq.zhongyouzk.top

[R64] 结束进程
来源：http://aid.yuanzhike.top

kill -9 $(pgrep -f app.py)
来源：http://gkj.ehwqpu.com

[R65] 查看端口占用
来源：http://cyl.xuetiantiany.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vhc.fzhhl.top

[R66] 定时任务
来源：http://hdq.hcnkem.com

crontab -e;  crontab -l
来源：http://cfl.sysykeji.top

[R67] 生成随机十六进制串
来源：http://uwn.zycfv.cn

openssl rand -hex 16
来源：http://ioy.nanxinkj.top

[R68] 计算文件校验值
来源：http://bqz.hammf.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xck.zhiwuduotai.top

[R69] 生成随机密码
来源：http://cqt.zycfv.cn

head -c 16 /dev/urandom | base64
来源：http://mwn.jinqigfzy.top

[R70] 时间戳与互转
来源：http://wpz.gzhubu.top

date +%s;  date -d @1700000000
来源：http://pob.ctjpmb.com

[R71] 日期格式化
来源：http://ipq.zhiwuduotai.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://swl.havefunace.top

[R72] 等待端口就绪
来源：http://hmq.snrcjt.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://kdw.nanxinkj.top

[R73] 分割大日志
来源：http://fct.jyoumei.cn

split -l 1000 big.log part_
来源：http://afv.aibaodan.cn

[R74] 批量重命名
来源：http://lki.svipenyu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zmc.zhiwuduotai.top

[R75] 导出环境变量
来源：http://kni.cqqwz.cn

export PATH="$HOME/bin:$PATH"
来源：http://trz.havefunace.top

[R76] 使用临时文件
来源：http://rmq.xuetiantiany.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gsv.9152youxi.cn

[R77] 读取用户输入
来源：http://jvu.ivvv.top

read -rp "请输入: " ans
来源：http://nkw.fengsongda.top

[R78] 交互式菜单
来源：http://ayb.aibaodan.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nrx.tanke756.top

[R79] 解析命令行选项
来源：http://qzw.ehwqpu.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jeg.zhengqikj.top

[R80] 查看脚本执行耗时
来源：http://psw.vehdjk.com

time ./run.sh
来源：http://lyq.chenzaomai.com

================================================================================
来源：http://gfv.yuanzhike.top

S. C / C++ 专题
来源：http://mti.cdnleiting.top

================================================================================
来源：http://idq.ctjpmb.com

[S01] C：Hello World
来源：http://dvd.yongpay.top

#include <stdio.h>
来源：http://ojs.quarkkingdee.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://twi.zdqjudy.top

[S02] C：变量与格式化输出
来源：http://qxj.yongpay.top

int a = 10; printf("%d\n", a);
来源：http://ada.hcnkem.com

[S03] C：读入整数
来源：http://pzb.tian-w.cn

int x; scanf("%d", &x);
来源：http://jcn.tianlin.xyz

[S04] C：字符串复制
来源：http://rqx.zhiwuduotai.top

char dst[32]; strcpy(dst, "hi");
来源：http://msb.hnqzz.top

[S05] C：字符串长度
来源：http://oua.jinghuilouyu.cn

strlen(s)
来源：http://bwm.hnqzz.top

[S06] C：字符串比较
来源：http://uzw.yongpay.top

strcmp(a, b) == 0
来源：http://cli.nanxinkj.top

[S07] C：数组遍历求和
来源：http://wum.zhixingplan.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://srr.yvedp.cn

[S08] C：动态内存分配与释放
来源：http://oov.wangdashe.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rmp.xziqi.cn

[S09] C：结构体定义与初始化
来源：http://faq.c1oappe.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bsy.ywan-chungtsiang.top

[S10] C：指针与解引用
来源：http://dfz.hnqzz.top

int *p = &a;  *p = 5;
来源：http://eie.sweek.top

[S11] C：逐行读文件
来源：http://dde.daxiang520.top

FILE *f = fopen("a.txt", "r");
来源：http://ord.vqdsnc.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ghb.zhaomingkeji.xyz

fclose(f);
来源：http://dev.jlsjyb.cn

[S12] C：写文件
来源：http://iqo.nanxinkj.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dxv.jyoumei.cn

[S13] C：宏定义
来源：http://nww.xylfe.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://avn.aibaodan.cn

[S14] C：枚举
来源：http://ofx.cheryme.top

enum Color { RED, GREEN, BLUE };
来源：http://mjc.shuidangran.top

[S15] C：类型转换
来源：http://hem.cqqwz.cn

(double) a / b
来源：http://scz.hnqzz.top

[S16] C：位操作置位
来源：http://mue.uphjek.com

x |= (1 << 3);
来源：http://ivm.shanyushiyangkeji.top

[S17] C：安全拼接字符串
来源：http://twm.meibo888.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://foz.zhaomingkeji.xyz

[S18] C：命令行参数
来源：http://xwy.jinqigfzy.top

int main(int argc, char **argv)
来源：http://xmj.xinyue.icu

[S19] C：快速排序
来源：http://una.iojbl.cn

qsort(a, n, sizeof(int), cmp);
来源：http://lus.hesvh.cn

[S20] C：二分查找
来源：http://ntv.yvedp.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dmp.jqgfzy.top

[S21] C：字符类别判断
来源：http://xkk.zhengqikj.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wkg.jiagoushi.top

[S22] C：字符串转数字
来源：http://erv.yueranfly.top

atoi("42");  strtod("3.14", NULL);
来源：http://waw.gzhubu.top

[S23] C：随机数
来源：http://kpm.vehdjk.com

srand(time(NULL));  int r = rand() % 100;
来源：http://dli.ywan-chungtsiang.top

[S24] C：获取本地时间
来源：http://kyr.guannengcc.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ngg.yj20258.top

[S25] C：内存拷贝
来源：http://uhj.kuanghao11.cn

memcpy(dst, src, n);
来源：http://idr.ivvv.top

[S26] C：内存清零
来源：http://pho.ywan-chungtsiang.top

memset(a, 0, sizeof a);
来源：http://xdd.yangfankeji.com

[S27] C：定义常量
来源：http://bsx.cheryme.top

const double PI = 3.14159;
来源：http://cei.xziqi.cn

[S28] C：静态变量
来源：http://wst.tarul.cn

static int counter = 0;
来源：http://aya.mhx1999.top

[S29] C：变参函数
来源：http://ptm.nwbrower.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dhs.zdbjq.cn

[S30] C：头文件保护
来源：http://ogv.hnqzz.top

#ifndef X_H
来源：http://tst.andypj.xyz

#define X_H
来源：http://zpr.iojbl.cn

#endif
来源：http://dzd.sxryk.cn

[S31] C++：Hello World
来源：http://cto.nwbrower.top

#include <iostream>
来源：http://bih.chenzaomai.com

int main() { std::cout << "Hello\n"; }
来源：http://kcm.9152youxi.cn

[S32] C++：字符串
来源：http://yhx.svipenyu.cn

std::string s = "hi";  s += "!";
来源：http://dad.yfazqb.com

[S33] C++：vector 增删
来源：http://zbu.guowangkeji.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hhn.hysaishi.cn

[S34] C++：遍历 vector
来源：http://xle.jiagoushi.top

for (auto &x : v) { std::cout << x; }
来源：http://nqf.jinqigufen.top

[S35] C++：map
来源：http://bej.jlsjyb.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ptj.yonumen.top

[S36] C++：unordered_map
来源：http://uir.jyoumei.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wwx.tarul.cn

[S37] C++：set
来源：http://ebg.sysykeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://efe.epnwcf.com

[S38] C++：排序
来源：http://bwz.zdqjudy.top

std::sort(v.begin(), v.end());
来源：http://zvk.zhixingplan.top

[S39] C++：自定义比较器排序
来源：http://lxa.shuidangran.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gel.yj20258.top

[S40] C++：查找元素
来源：http://qae.hongshengwenyu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tku.yangfankeji.com

[S41] C++：类与构造函数
来源：http://bjg.zycfv.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hpy.aizwys.cn

[S42] C++：继承与虚函数
来源：http://vpg.aizwys.cn

class B : public Base { public: void f() override {} };
来源：http://ecd.yfazqb.com

[S43] C++：智能指针
来源：http://qhm.jinghuilouyu.cn

auto p = std::make_unique<int>(5);
来源：http://ybb.tian-w.cn

[S44] C++：引用传参
来源：http://lrq.jiagoushi.top

void inc(int &x) { ++x; }
来源：http://hzr.nwbrower.top

[S45] C++：lambda
来源：http://umi.xingfuxueyuan.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://xbs.gogol.net.cn

[S46] C++：函数模板
来源：http://hya.nanxinkj.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uga.zhaomingkeji.xyz

[S47] C++：结构化绑定遍历
来源：http://afb.meibo888.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nsc.ehwqpu.com

[S48] C++：逐行读文件
来源：http://ifd.zdbjq.cn

std::ifstream in("a.txt");  std::string line;
来源：http://lwz.9152youxi.cn

while (std::getline(in, line)) { }
来源：http://vxd.xuanzx.com

[S49] C++：写文件
来源：http://yny.jinqigfzy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://omb.yuxming.cn

[S50] C++：格式化数字
来源：http://ihc.pycfn.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qir.tian-w.cn

[S51] C++：显式类型转换
来源：http://usm.zhijiandao.cn

static_cast<double>(a) / b
来源：http://xft.wangshuangyany.cn

[S52] C++：const 与 noexcept
来源：http://ncw.52xcode.cn

int size() const noexcept { return n_; }
来源：http://eer.hongshengwenyu.top

[S53] C++：移动语义
来源：http://ddv.shzxlz.cn

std::vector<int> w = std::move(v);
来源：http://wjg.redwolf501.top

[S54] C++：异常处理
来源：http://gdo.zdqjudy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vax.hysaishi.cn

[S55] C++：结构化绑定
来源：http://ugq.yj20258.top

auto [a, b] = std::make_pair(1, 2);
来源：http://tbr.0kj1m.cn

[S56] C++：optional
来源：http://dmv.sjlbkw.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kql.tanke756.top

[S57] C++：编译期常量
来源：http://kwc.tian-w.cn

constexpr int N = 10;
来源：http://bsq.xuetiantiany.cn

[S58] C++：命名空间
来源：http://jbt.xingfuxueyuan.xyz

namespace ns { int f() { return 1; } }
来源：http://osq.fktsv.cn

[S59] C++：静态断言
来源：http://bbu.feifeiyinyue.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bwo.ydjk.org.cn

[S60] C++：遍历并删除元素
来源：http://rbo.hesvh.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cqc.jiagoushi.top

================================================================================
来源：http://pev.zhongyouzk.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://opr.yj20258888.top

================================================================================
来源：http://tap.yuanzhike.top

[T01] Kotlin：Hello World
来源：http://gez.bjfxy.top

println("Hello")
来源：http://srr.hnqzz.top

[T02] Kotlin：变量
来源：http://aet.daxiang520.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bjm.zycfv.cn

[T03] Kotlin：字符串模板
来源：http://isq.jinqigfzy.top

"值: $b"
来源：http://pgn.yueranfly.top

[T04] Kotlin：空安全
来源：http://kjz.hammf.cn

val n: String? = null;  n?.length
来源：http://dng.yuxming.cn

[T05] Kotlin：when 表达式
来源：http://qgz.9152youxi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uip.zhiwuduotai.top

[T06] Kotlin：集合映射
来源：http://vib.gotoacloud.top

listOf(1, 2, 3).map { it * 2 }
来源：http://dxk.sweek.top

[T07] Kotlin：集合过滤
来源：http://nst.9152youxi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://auj.quarkkingdee.top

[T08] Kotlin：数据类
来源：http://zav.xinyue.icu

data class User(val name: String, val age: Int)
来源：http://gxd.jqgufenzy.top

[T09] Kotlin：扩展函数
来源：http://ixs.havefunace.top

fun String.exclaim() = this + "!"
来源：http://fpr.cucudq.cn

[T10] Kotlin：默认参数
来源：http://him.chenjidiqi.icu

fun greet(name: String = "World") = "Hi $name"
来源：http://yfl.ppjwa.cn

[T11] Kotlin：协程
来源：http://hhl.zhijiandao.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://lln.fehbvm.com

[T12] Kotlin：解构声明
来源：http://xcp.sweek.top

val (a, b) = Pair(1, 2)
来源：http://xwx.sxryk.cn

[T13] Kotlin：只读 Map
来源：http://ilg.bjfxy.top

val m = mapOf("a" to 1)
来源：http://htv.jyoumei.cn

[T14] Kotlin：循环
来源：http://enj.epnwcf.com

for (i in 1..10) println(i)
来源：http://lqs.birdmap.top

[T15] Kotlin：接口
来源：http://axb.yuxming.cn

interface Shape { fun area(): Double }
来源：http://fgm.tianlin.xyz

[T16] Swift：Hello World
来源：http://nfo.cqqwz.cn

print("Hello")
来源：http://lha.yj20258.top

[T17] Swift：变量与常量
来源：http://egn.iojbl.cn

var a = 1;  let b = 2
来源：http://vum.zdbjq.cn

[T18] Swift：字符串插值
来源：http://uir.jinghuilouyu.cn

"值: \(b)"
来源：http://gyi.zhoulong.xyz

[T19] Swift：可选绑定
来源：http://xch.jlsjyb.cn

if let n = opt { print(n) }
来源：http://bva.daria6918.cn

[T20] Swift：数组操作
来源：http://ycc.cqqwz.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hub.svipenyu.cn

[T21] Swift：遍历
来源：http://gpk.wangshuangyany.cn

for x in a { print(x) }
来源：http://dfg.birdmap.top

[T22] Swift：字典
来源：http://lyb.jinyuanbaomall.cn

var d = ["a": 1];  d["b"] = 2
来源：http://aya.zdqjudy.top

[T23] Swift：函数
来源：http://lhh.tarul.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mrw.jyoumei.cn

[T24] Swift：闭包
来源：http://jfx.fengsongda.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://iuj.xinyue.icu

[T25] Swift：结构体
来源：http://ras.jqgufenzy.top

struct P { var x: Int }
来源：http://sel.xziqi.cn

[T26] Swift：类与重写
来源：http://tkb.nanxinkj.top

class A: Base { override func f() {} }
来源：http://tkm.chenjidiqi.icu


<!-- 参考信息 -->