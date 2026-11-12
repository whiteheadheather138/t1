代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://enw.gaohongyu789.top

[R24] 大小写转换
来源：http://eyz.9152youxi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://uhn.ybcxt.top

[R25] 去后缀 / 去前缀
来源：http://bhl.nanxinkj.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://shy.vqdsnc.cn

[R26] 命令替换
来源：http://ehb.tanke756.top

now=$(date +%F); echo "$now"
来源：http://xcw.guowangkeji.top

[R27] 算术展开
来源：http://kco.hywenlv.cn

echo $((1 + 2 * 3))
来源：http://nkx.tanke756.top

[R28] 浮点运算
来源：http://eqn.0kj1m.cn

echo "scale=2; 10/3" | bc
来源：http://cdx.jqgufenzy.top

[R29] 定义函数
来源：http://rgi.hcnkem.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://imw.gaohongyu789.top

[R30] 函数返回状态码
来源：http://qax.fktsv.cn

f() { return 0; }; f || echo "失败了"
来源：http://skd.hcnkem.com

[R31] 局部变量
来源：http://bfg.cheryme.top

f() { local x=1; echo "$x"; }
来源：http://gwr.ppjwa.cn

[R32] 参数个数校验
来源：http://mxn.yj20258.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://oiy.bbcook.cn

[R33] 捕获错误并提示行号
来源：http://scq.fehbvm.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ltt.c1oappe.top

[R34] 退出时清理
来源：http://ngo.ppjwa.cn

trap 'rm -f "$tmp"' EXIT
来源：http://wwb.snrcjt.cn

[R35] 后台执行并等待
来源：http://xlb.hywenlv.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://pew.wangshuangyany.cn

[R36] 并发执行多个任务
来源：http://oeu.zhixingplan.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ygs.yj202588.top

[R37] 把输出赋给变量
来源：http://gex.fengsongda.top

files=$(ls -1)
来源：http://vvu.yonumen.top

[R38] 管道串联
来源：http://ify.nwbrower.top

cat a.txt | grep -i error | wc -l
来源：http://mwh.chenlongwang.top

[R39] 重定向标准输出与错误
来源：http://nfu.ydjk.org.cn

cmd > out.log 2>&1
来源：http://zjg.fengsongda.top

[R40] 追加写日志
来源：http://qbf.tanke756.top

echo "log" >> out.log
来源：http://rpn.bjfxy.top

[R41] 丢弃输出
来源：http://tck.yonumen.top

cmd >/dev/null 2>&1
来源：http://jtq.9152youxi.cn

[R42] 输入重定向
来源：http://dgu.jinqigfzy.top

wc -l < a.txt
来源：http://pcz.xinyue.icu

[R43] 按名字查找文件
来源：http://jje.cheryme.top

find . -name "*.log" -type f
来源：http://lau.guowangkeji.top

[R44] 按修改时间查找
来源：http://clc.xylfe.cn

find . -mtime -7 -type f
来源：http://wlx.jinqigufen.top

[R45] 批量删除
来源：http://fgk.cucudq.cn

find . -name "*.tmp" -delete
来源：http://nsa.yongpay.top

[R46] 递归替换文件内容
来源：http://wqt.ywan-chungtsiang.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jkb.xziqi.cn

[R47] sed 单行替换
来源：http://mny.yj202588.top

sed -i 's/foo/bar/g' a.txt
来源：http://kxm.yj20258.top

[R48] awk 取指定列
来源：http://ftx.shuidangran.top

awk '{print $1, $3}' a.txt
来源：http://nzh.zhixingplan.top

[R49] awk 带条件
来源：http://urh.tarul.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ieo.smart0.xyz

[R50] awk 求和
来源：http://lbe.svipenyu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hst.tian-w.cn

[R51] 排序去重取前几
来源：http://yfq.shangyingyoupin.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ozo.haohaochexian.top

[R52] 统计行数
来源：http://usp.c1oappe.top

wc -l a.txt
来源：http://bro.fehbvm.com

[R53] 查看文件头与实时尾
来源：http://aik.yvedp.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zjr.yj20258.top

[R54] 比较两个文件
来源：http://nri.gogol.net.cn

diff a.txt b.txt
来源：http://rah.jinyuanbaomall.cn

[R55] 压缩与解压
来源：http://ngu.ywan-chungtsiang.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cns.wangdashe.top

[R56] 远程拷贝
来源：http://zzc.jinghuilouyu.cn

scp file user@host:/path/
来源：http://ldb.sxryk.cn

[R57] 远程执行命令
来源：http://iyv.shanyushiyangkeji.top

ssh user@host 'uptime'
来源：http://yxb.ivvv.top

[R58] 下载文件
来源：http://qtq.daria6918.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://grn.jlsjyb.cn

[R59] 发 POST JSON
来源：http://nii.yj20258888.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yub.ydjk.org.cn

[R60] 只看 HTTP 状态码
来源：http://vct.sufxvd.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sfa.dashuyun.cn

[R61] 磁盘占用
来源：http://kte.fengsongda.top

df -h;  du -sh *
来源：http://vua.kuanghao11.cn

[R62] 找最占空间的文件
来源：http://bby.chenzaomai.com

du -ah . | sort -rh | head -10
来源：http://rry.aibaodan.cn

[R63] 内存与进程
来源：http://zxb.sjlbkw.cn

free -h;  ps aux | grep nginx
来源：http://evc.shzxlz.cn

[R64] 结束进程
来源：http://dur.xingfuxueyuan.xyz

kill -9 $(pgrep -f app.py)
来源：http://sdc.havefunace.top

[R65] 查看端口占用
来源：http://hyl.yanxiufei.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xgp.aizwys.cn

[R66] 定时任务
来源：http://qhj.chenjidiqi.icu

crontab -e;  crontab -l
来源：http://ibw.zhijiandao.cn

[R67] 生成随机十六进制串
来源：http://krs.hysaishi.cn

openssl rand -hex 16
来源：http://uqd.gaohongyu789.top

[R68] 计算文件校验值
来源：http://oht.zycfv.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xmc.jyoumei.cn

[R69] 生成随机密码
来源：http://ecu.hysaishi.cn

head -c 16 /dev/urandom | base64
来源：http://eol.havefunace.top

[R70] 时间戳与互转
来源：http://ayz.ctjpmb.com

date +%s;  date -d @1700000000
来源：http://zfd.cashguo.top

[R71] 日期格式化
来源：http://aiy.sufxvd.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zwb.shangyingyoupin.top

[R72] 等待端口就绪
来源：http://pdu.tian-w.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://txt.fzhhl.top

[R73] 分割大日志
来源：http://jua.feifeiyinyue.top

split -l 1000 big.log part_
来源：http://mla.ctjpmb.com

[R74] 批量重命名
来源：http://jbd.tanke756.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rby.xuetiantiany.cn

[R75] 导出环境变量
来源：http://xis.jlsjyb.cn

export PATH="$HOME/bin:$PATH"
来源：http://iae.gzhubu.top

[R76] 使用临时文件
来源：http://crl.wangdashe.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ccn.chenlongwang.top

[R77] 读取用户输入
来源：http://yza.xylfe.cn

read -rp "请输入: " ans
来源：http://zip.sufxvd.cn

[R78] 交互式菜单
来源：http://cnx.chenlongwang.top

select opt in a b c; do echo "$opt"; break; done
来源：http://nsi.hesvh.cn

[R79] 解析命令行选项
来源：http://qwp.pengpengdd.cyou

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ocj.hysaishi.cn

[R80] 查看脚本执行耗时
来源：http://hqe.yvedp.cn

time ./run.sh
来源：http://adu.316326.xyz

================================================================================
来源：http://rhd.guannengcc.top

S. C / C++ 专题
来源：http://yss.hnqzz.top

================================================================================
来源：http://rsz.0kj1m.cn

[S01] C：Hello World
来源：http://mxi.ivvv.top

#include <stdio.h>
来源：http://frw.shuidangran.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://qwv.aibaodan.cn

[S02] C：变量与格式化输出
来源：http://lme.aibaodan.cn

int a = 10; printf("%d\n", a);
来源：http://stf.shanyushiyangtech.top

[S03] C：读入整数
来源：http://pdc.hywenlv.cn

int x; scanf("%d", &x);
来源：http://xgy.jyoumei.cn

[S04] C：字符串复制
来源：http://frz.ctjpmb.com

char dst[32]; strcpy(dst, "hi");
来源：http://jyd.birdmap.top

[S05] C：字符串长度
来源：http://lee.cdnleiting.top

strlen(s)
来源：http://teo.jlsjyb.cn

[S06] C：字符串比较
来源：http://dyt.cucudq.cn

strcmp(a, b) == 0
来源：http://gav.zdbjq.cn

[S07] C：数组遍历求和
来源：http://zda.hnqzz.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bvz.zhixingplan.top

[S08] C：动态内存分配与释放
来源：http://bnv.chenlongwang.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tvf.yj202588.top

[S09] C：结构体定义与初始化
来源：http://ejt.tanke756.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://svv.birdmap.top

[S10] C：指针与解引用
来源：http://gmb.bjfxy.top

int *p = &a;  *p = 5;
来源：http://jvj.zhongyouzk.top

[S11] C：逐行读文件
来源：http://afj.zhiwuduotai.top

FILE *f = fopen("a.txt", "r");
来源：http://kom.wangdashe.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://syb.sxryk.cn

fclose(f);
来源：http://ouc.sjlbkw.cn

[S12] C：写文件
来源：http://oyn.jianghu66.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fmw.gaohongyu789.top

[S13] C：宏定义
来源：http://joa.shzxlz.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qcu.jqgfzy.top

[S14] C：枚举
来源：http://cex.hnxiangtu.top

enum Color { RED, GREEN, BLUE };
来源：http://obu.ivvv.top

[S15] C：类型转换
来源：http://zjs.redwolf501.top

(double) a / b
来源：http://djb.shangyingyoupin.top

[S16] C：位操作置位
来源：http://nve.sjlbkw.cn

x |= (1 << 3);
来源：http://ldo.nanxuanxn.top

[S17] C：安全拼接字符串
来源：http://qyv.yonumen.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xby.tian-w.cn

[S18] C：命令行参数
来源：http://duh.cucudq.cn

int main(int argc, char **argv)
来源：http://npc.dashuyun.cn

[S19] C：快速排序
来源：http://sid.yj20258888.top

qsort(a, n, sizeof(int), cmp);
来源：http://uvn.nanxuanxn.top

[S20] C：二分查找
来源：http://cae.xuanzx.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lfu.zhixingplan.top

[S21] C：字符类别判断
来源：http://uvl.xinyue.icu

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zlc.hammf.cn

[S22] C：字符串转数字
来源：http://iom.tanke756.top

atoi("42");  strtod("3.14", NULL);
来源：http://lhc.ehwqpu.com

[S23] C：随机数
来源：http://nvk.hongshengwenyu.top

srand(time(NULL));  int r = rand() % 100;
来源：http://qou.tanke756.top

[S24] C：获取本地时间
来源：http://ytx.pengpengdd.cyou

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gjl.svipenyu.cn

[S25] C：内存拷贝
来源：http://zfs.shangyingyoupin.top

memcpy(dst, src, n);
来源：http://ttc.fzhhl.top

[S26] C：内存清零
来源：http://dum.quarkkingdee.top

memset(a, 0, sizeof a);
来源：http://rmb.ybcxt.top

[S27] C：定义常量
来源：http://lha.hnxiangtu.top

const double PI = 3.14159;
来源：http://lkh.aibaodan.cn

[S28] C：静态变量
来源：http://cyy.bbcook.cn

static int counter = 0;
来源：http://doj.hesvh.cn

[S29] C：变参函数
来源：http://lfk.jinyuanbaomall.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qpv.yanxiufei.cn

[S30] C：头文件保护
来源：http://zrt.xinyue.icu

#ifndef X_H
来源：http://orq.fktsv.cn

#define X_H
来源：http://wvv.ydjk.org.cn

#endif
来源：http://cwg.pycfn.com

[S31] C++：Hello World
来源：http://moe.jqgfzy.top

#include <iostream>
来源：http://ows.cheryme.top

int main() { std::cout << "Hello\n"; }
来源：http://ypz.quarkkingdee.top

[S32] C++：字符串
来源：http://klm.aibaodan.cn

std::string s = "hi";  s += "!";
来源：http://vrl.redwolf501.top

[S33] C++：vector 增删
来源：http://cco.dianchejie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ntq.zhijiandao.cn

[S34] C++：遍历 vector
来源：http://tyw.ivvv.top

for (auto &x : v) { std::cout << x; }
来源：http://wqg.ydjk.org.cn

[S35] C++：map
来源：http://zys.jianghu66.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://api.vqdsnc.cn

[S36] C++：unordered_map
来源：http://tzy.zhijiandao.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tkr.svipenyu.cn

[S37] C++：set
来源：http://zfx.hnxiangtu.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xgm.hfpthk.cn

[S38] C++：排序
来源：http://udi.yangfankeji.com

std::sort(v.begin(), v.end());
来源：http://amm.sjlbkw.cn

[S39] C++：自定义比较器排序
来源：http://yss.yj202588.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pdh.jqgfzy.top

[S40] C++：查找元素
来源：http://jkv.zhijiandao.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://odm.gogol.net.cn

[S41] C++：类与构造函数
来源：http://oeb.wangdashe.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ncf.gaohongyu789.top

[S42] C++：继承与虚函数
来源：http://fli.52xcode.cn

class B : public Base { public: void f() override {} };
来源：http://tpn.0kj1m.cn

[S43] C++：智能指针
来源：http://apk.hnxiangtu.top

auto p = std::make_unique<int>(5);
来源：http://qqp.sjlbkw.cn

[S44] C++：引用传参
来源：http://hkt.ctjpmb.com

void inc(int &x) { ++x; }
来源：http://drv.zhixingplan.top

[S45] C++：lambda
来源：http://kva.hongshengwenyu.top

auto add = [](int a, int b) { return a + b; };
来源：http://dze.jinqigfzy.top

[S46] C++：函数模板
来源：http://cpx.guannengcc.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://aab.jyoumei.cn

[S47] C++：结构化绑定遍历
来源：http://qav.shzxlz.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nyc.fzhhl.top

[S48] C++：逐行读文件
来源：http://lfa.52xcode.cn

std::ifstream in("a.txt");  std::string line;
来源：http://rms.guowangkeji.top

while (std::getline(in, line)) { }
来源：http://kyf.ehwqpu.com

[S49] C++：写文件
来源：http://alm.birdmap.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://djy.quarkkingdee.top

[S50] C++：格式化数字
来源：http://qce.yonumen.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wys.sysykeji.top

[S51] C++：显式类型转换
来源：http://wkj.xylfe.cn

static_cast<double>(a) / b
来源：http://sol.fengsongda.top

[S52] C++：const 与 noexcept
来源：http://ipd.fktsv.cn

int size() const noexcept { return n_; }
来源：http://jcs.c1oappe.top

[S53] C++：移动语义
来源：http://kov.shzxlz.cn

std::vector<int> w = std::move(v);
来源：http://edc.hammf.cn

[S54] C++：异常处理
来源：http://uka.meibo888.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hrl.zhiwuduotai.top

[S55] C++：结构化绑定
来源：http://vsc.nwbrower.top

auto [a, b] = std::make_pair(1, 2);
来源：http://crv.shzxlz.cn

[S56] C++：optional
来源：http://qkb.hnxiangtu.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lyd.fehbvm.com

[S57] C++：编译期常量
来源：http://kuj.hcnkem.com

constexpr int N = 10;
来源：http://tvg.guannengcc.top

[S58] C++：命名空间
来源：http://rtb.cqqwz.cn

namespace ns { int f() { return 1; } }
来源：http://iki.chenzaomai.com

[S59] C++：静态断言
来源：http://ftz.gogol.net.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://luc.hnqzz.top

[S60] C++：遍历并删除元素
来源：http://yks.fktsv.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://isz.yangfankeji.com

================================================================================
来源：http://yvq.mhx1999.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hdb.zhaomingkeji.xyz

================================================================================
来源：http://lmo.hywenlv.cn

[T01] Kotlin：Hello World
来源：http://htp.sweek.top

println("Hello")
来源：http://pcl.chenlongwang.top

[T02] Kotlin：变量
来源：http://krq.xylfe.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://irk.yj20258.top

[T03] Kotlin：字符串模板
来源：http://rrl.fktsv.cn

"值: $b"
来源：http://auf.pengpengdd.cyou

[T04] Kotlin：空安全
来源：http://olu.chenzaomai.com

val n: String? = null;  n?.length
来源：http://hav.bbcook.cn

[T05] Kotlin：when 表达式
来源：http://nbz.gotoacloud.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kml.xinyue.icu

[T06] Kotlin：集合映射
来源：http://hwn.zdqjudy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://dgd.xinyue.icu

[T07] Kotlin：集合过滤
来源：http://kde.shuidangran.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://bty.tanke756.top

[T08] Kotlin：数据类
来源：http://zwg.zhiwuduotai.top

data class User(val name: String, val age: Int)
来源：http://yjj.yj202588.top

[T09] Kotlin：扩展函数
来源：http://ftj.mhx1999.top

fun String.exclaim() = this + "!"
来源：http://cqn.jinghuilouyu.cn

[T10] Kotlin：默认参数
来源：http://ivz.guowangkeji.top

fun greet(name: String = "World") = "Hi $name"
来源：http://hnj.jinqigufen.top

[T11] Kotlin：协程
来源：http://rcl.jinyuanbaomall.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://sfy.fehbvm.com

[T12] Kotlin：解构声明
来源：http://wzu.gaohongyu789.top

val (a, b) = Pair(1, 2)
来源：http://kaf.nwbrower.top

[T13] Kotlin：只读 Map
来源：http://bap.fanxiaobao.xyz

val m = mapOf("a" to 1)
来源：http://sci.zhijiandao.cn

[T14] Kotlin：循环
来源：http://nhy.redwolf501.top

for (i in 1..10) println(i)
来源：http://yec.iojbl.cn

[T15] Kotlin：接口
来源：http://icc.gogol.net.cn

interface Shape { fun area(): Double }
来源：http://ekg.tarul.cn

[T16] Swift：Hello World
来源：http://azz.smart0.xyz

print("Hello")
来源：http://mvf.yj202588.top

[T17] Swift：变量与常量
来源：http://xgu.shangyingyoupin.top

var a = 1;  let b = 2
来源：http://wur.havefunace.top

[T18] Swift：字符串插值
来源：http://wei.jinqigfzy.top

"值: \(b)"
来源：http://kaf.vehdjk.com

[T19] Swift：可选绑定
来源：http://lwe.fktsv.cn

if let n = opt { print(n) }
来源：http://cuf.sxryk.cn

[T20] Swift：数组操作
来源：http://qts.fktsv.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zvi.fktsv.cn

[T21] Swift：遍历
来源：http://vhp.fktsv.cn

for x in a { print(x) }
来源：http://gvf.ydjk.org.cn

[T22] Swift：字典
来源：http://gfh.bjfxy.top

var d = ["a": 1];  d["b"] = 2
来源：http://qpv.ydjk.org.cn

[T23] Swift：函数
来源：http://hpr.shzxlz.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hmq.havefunace.top

[T24] Swift：闭包
来源：http://tvs.jinqigufen.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://stc.fanxiaobao.xyz

[T25] Swift：结构体
来源：http://kpf.daria6918.cn

struct P { var x: Int }
来源：http://ilm.uphjek.com

[T26] Swift：类与重写
来源：http://qlu.hysaishi.cn

class A: Base { override func f() {} }
来源：http://kdt.zycfv.cn


<!-- 参考信息 -->