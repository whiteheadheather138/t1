代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tdt.xuanzx.com

[R24] 大小写转换
来源：http://vtw.hfpthk.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bcb.yj20258.top

[R25] 去后缀 / 去前缀
来源：http://jhw.quarkkingdee.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://dkk.jiagoushi.top

[R26] 命令替换
来源：http://sum.epnwcf.com

now=$(date +%F); echo "$now"
来源：http://tey.jianghu66.top

[R27] 算术展开
来源：http://aeo.xylfe.cn

echo $((1 + 2 * 3))
来源：http://qah.sweek.top

[R28] 浮点运算
来源：http://rdg.cashguo.top

echo "scale=2; 10/3" | bc
来源：http://thj.epnwcf.com

[R29] 定义函数
来源：http://mbe.hammf.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://uap.aibaodan.cn

[R30] 函数返回状态码
来源：http://hak.smart0.xyz

f() { return 0; }; f || echo "失败了"
来源：http://fta.yvedp.cn

[R31] 局部变量
来源：http://whe.snrcjt.cn

f() { local x=1; echo "$x"; }
来源：http://hzt.shangyingyoupin.top

[R32] 参数个数校验
来源：http://qna.redwolf501.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bgv.gotoacloud.top

[R33] 捕获错误并提示行号
来源：http://ngq.hongshengwenyu.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dkq.aibaodan.cn

[R34] 退出时清理
来源：http://gxj.meibo888.top

trap 'rm -f "$tmp"' EXIT
来源：http://osk.iojbl.cn

[R35] 后台执行并等待
来源：http://tak.jlsjyb.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gmb.jinqigufen.top

[R36] 并发执行多个任务
来源：http://zjr.mhx1999.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dde.ctjpmb.com

[R37] 把输出赋给变量
来源：http://ogy.fanxiaobao.xyz

files=$(ls -1)
来源：http://uoy.ehwqpu.com

[R38] 管道串联
来源：http://hti.zhixingplan.top

cat a.txt | grep -i error | wc -l
来源：http://bys.dashuyun.cn

[R39] 重定向标准输出与错误
来源：http://qmi.hongshengwenyu.top

cmd > out.log 2>&1
来源：http://cdc.hcnkem.com

[R40] 追加写日志
来源：http://ccl.52xcode.cn

echo "log" >> out.log
来源：http://xfd.tanke756.top

[R41] 丢弃输出
来源：http://yak.c1oappe.top

cmd >/dev/null 2>&1
来源：http://brl.hnqzz.top

[R42] 输入重定向
来源：http://ivr.hfpthk.cn

wc -l < a.txt
来源：http://ljh.jinyuanbaomall.cn

[R43] 按名字查找文件
来源：http://lmz.jqgufenzy.top

find . -name "*.log" -type f
来源：http://vgh.andypj.xyz

[R44] 按修改时间查找
来源：http://hzo.hcnkem.com

find . -mtime -7 -type f
来源：http://mnw.vqdsnc.cn

[R45] 批量删除
来源：http://hvc.dianchejie.cn

find . -name "*.tmp" -delete
来源：http://nmf.hammf.cn

[R46] 递归替换文件内容
来源：http://ikt.guannengcc.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tii.redwolf501.top

[R47] sed 单行替换
来源：http://pgy.fanxiaobao.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://ily.ydjk.org.cn

[R48] awk 取指定列
来源：http://bnz.zhijiandao.cn

awk '{print $1, $3}' a.txt
来源：http://nxj.yj20258888.top

[R49] awk 带条件
来源：http://ofu.sxryk.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dai.haohaochexian.top

[R50] awk 求和
来源：http://dzz.ydzc1.top

awk '{s += $2} END {print s}' a.txt
来源：http://oni.vqdsnc.cn

[R51] 排序去重取前几
来源：http://sfj.zhoulong.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://bzt.pengpengdd.cyou

[R52] 统计行数
来源：http://gyx.mhx1999.top

wc -l a.txt
来源：http://yva.jqgufenzy.top

[R53] 查看文件头与实时尾
来源：http://oea.guannengcc.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dzp.cheryme.top

[R54] 比较两个文件
来源：http://wie.316326.xyz

diff a.txt b.txt
来源：http://otr.mhx1999.top

[R55] 压缩与解压
来源：http://ufp.hongshengwenyu.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fda.yvedp.cn

[R56] 远程拷贝
来源：http://rfb.hnqzz.top

scp file user@host:/path/
来源：http://qbz.zhijiandao.cn

[R57] 远程执行命令
来源：http://eye.zhengqikj.top

ssh user@host 'uptime'
来源：http://cjc.snrcjt.cn

[R58] 下载文件
来源：http://yme.zhoulong.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dzh.shanyushiyangkeji.top

[R59] 发 POST JSON
来源：http://jkh.guannengcc.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qrx.jiagoushi.top

[R60] 只看 HTTP 状态码
来源：http://hfc.cdnleiting.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://muo.snrcjt.cn

[R61] 磁盘占用
来源：http://nop.chenlongwang.top

df -h;  du -sh *
来源：http://kjb.316326.xyz

[R62] 找最占空间的文件
来源：http://hya.hcnkem.com

du -ah . | sort -rh | head -10
来源：http://vdf.yj20258.top

[R63] 内存与进程
来源：http://xfq.chenjidiqi.icu

free -h;  ps aux | grep nginx
来源：http://das.cqqwz.cn

[R64] 结束进程
来源：http://qeg.hnqzz.top

kill -9 $(pgrep -f app.py)
来源：http://gme.fehbvm.com

[R65] 查看端口占用
来源：http://xij.uphjek.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wgu.yfazqb.com

[R66] 定时任务
来源：http://jel.meibo888.top

crontab -e;  crontab -l
来源：http://dts.gaohongyu789.top

[R67] 生成随机十六进制串
来源：http://unt.ivvv.top

openssl rand -hex 16
来源：http://ltj.fzhhl.top

[R68] 计算文件校验值
来源：http://vfz.quarkkingdee.top

sha256sum a.txt;  md5sum a.txt
来源：http://nyn.zdbjq.cn

[R69] 生成随机密码
来源：http://dqj.jianghu66.top

head -c 16 /dev/urandom | base64
来源：http://dux.yfazqb.com

[R70] 时间戳与互转
来源：http://aqg.kuanghao11.cn

date +%s;  date -d @1700000000
来源：http://unq.jlsjyb.cn

[R71] 日期格式化
来源：http://llh.yj20258.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://uaf.ppjwa.cn

[R72] 等待端口就绪
来源：http://aez.jyoumei.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zud.tianlin.xyz

[R73] 分割大日志
来源：http://sfr.jlsjyb.cn

split -l 1000 big.log part_
来源：http://gaj.pengpengdd.cyou

[R74] 批量重命名
来源：http://yzr.iojbl.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jot.ivvv.top

[R75] 导出环境变量
来源：http://dtd.cqqwz.cn

export PATH="$HOME/bin:$PATH"
来源：http://gwe.hysaishi.cn

[R76] 使用临时文件
来源：http://hdr.chenzaomai.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gdt.9152youxi.cn

[R77] 读取用户输入
来源：http://iwg.bbcook.cn

read -rp "请输入: " ans
来源：http://oay.hammf.cn

[R78] 交互式菜单
来源：http://ref.yvedp.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://lql.snrcjt.cn

[R79] 解析命令行选项
来源：http://bcx.fengsongda.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kpt.yvedp.cn

[R80] 查看脚本执行耗时
来源：http://udl.yj20258.top

time ./run.sh
来源：http://prs.jqgfzy.top

================================================================================
来源：http://jhx.wangdashe.top

S. C / C++ 专题
来源：http://bmr.sxryk.cn

================================================================================
来源：http://yct.ehwqpu.com

[S01] C：Hello World
来源：http://lww.316326.xyz

#include <stdio.h>
来源：http://iks.cucudq.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qzq.xziqi.cn

[S02] C：变量与格式化输出
来源：http://lsc.chenlongwang.top

int a = 10; printf("%d\n", a);
来源：http://edb.yueranfly.top

[S03] C：读入整数
来源：http://qhu.nwbrower.top

int x; scanf("%d", &x);
来源：http://uts.yj20258888.top

[S04] C：字符串复制
来源：http://ill.bjfxy.top

char dst[32]; strcpy(dst, "hi");
来源：http://meh.shanyushiyangtech.top

[S05] C：字符串长度
来源：http://mww.zhengqikj.top

strlen(s)
来源：http://gqn.tianlin.xyz

[S06] C：字符串比较
来源：http://iqd.jqgufenzy.top

strcmp(a, b) == 0
来源：http://jwa.zhijiandao.cn

[S07] C：数组遍历求和
来源：http://fyq.zhijiandao.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ahd.xingfuxueyuan.xyz

[S08] C：动态内存分配与释放
来源：http://cks.svipenyu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rfa.birdmap.top

[S09] C：结构体定义与初始化
来源：http://uap.ydjk.org.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qwb.sxryk.cn

[S10] C：指针与解引用
来源：http://fpu.smart0.xyz

int *p = &a;  *p = 5;
来源：http://qum.yangfankeji.com

[S11] C：逐行读文件
来源：http://nyz.pycfn.com

FILE *f = fopen("a.txt", "r");
来源：http://uvp.9152youxi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qbn.yfazqb.com

fclose(f);
来源：http://ogn.shanyushiyangkeji.top

[S12] C：写文件
来源：http://ixo.haohaochexian.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://shz.svipenyu.cn

[S13] C：宏定义
来源：http://uru.quarkkingdee.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hrb.zhengqikj.top

[S14] C：枚举
来源：http://bra.gzhubu.top

enum Color { RED, GREEN, BLUE };
来源：http://mnx.316326.xyz

[S15] C：类型转换
来源：http://lqk.jinyuanbaomall.cn

(double) a / b
来源：http://dci.yueranfly.top

[S16] C：位操作置位
来源：http://mkh.yangfankeji.com

x |= (1 << 3);
来源：http://vlu.smart0.xyz

[S17] C：安全拼接字符串
来源：http://uxy.nwbrower.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sco.zycfv.cn

[S18] C：命令行参数
来源：http://pim.snrcjt.cn

int main(int argc, char **argv)
来源：http://jfw.havefunace.top

[S19] C：快速排序
来源：http://jqj.nwbrower.top

qsort(a, n, sizeof(int), cmp);
来源：http://nsf.epnwcf.com

[S20] C：二分查找
来源：http://cxm.jlsjyb.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://axk.daria6918.cn

[S21] C：字符类别判断
来源：http://lze.ehwqpu.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vwz.ybcxt.top

[S22] C：字符串转数字
来源：http://fhy.ehwqpu.com

atoi("42");  strtod("3.14", NULL);
来源：http://sen.hongshengwenyu.top

[S23] C：随机数
来源：http://vwo.chenzaomai.com

srand(time(NULL));  int r = rand() % 100;
来源：http://zfn.xingfuxueyuan.xyz

[S24] C：获取本地时间
来源：http://jis.hywenlv.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zyi.haohaochexian.top

[S25] C：内存拷贝
来源：http://uev.feifeiyinyue.top

memcpy(dst, src, n);
来源：http://wwp.ydzc1.top

[S26] C：内存清零
来源：http://fgp.yongpay.top

memset(a, 0, sizeof a);
来源：http://ymm.wangdashe.top

[S27] C：定义常量
来源：http://kpw.jiagoushi.top

const double PI = 3.14159;
来源：http://xxx.bjfxy.top

[S28] C：静态变量
来源：http://zug.jiagoushi.top

static int counter = 0;
来源：http://szq.hfpthk.cn

[S29] C：变参函数
来源：http://iaq.sufxvd.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wst.yuanzhike.top

[S30] C：头文件保护
来源：http://eqy.nanxuanxn.top

#ifndef X_H
来源：http://ega.jiagoushi.top

#define X_H
来源：http://emj.ybcxt.top

#endif
来源：http://ifl.mhx1999.top

[S31] C++：Hello World
来源：http://tme.tian-w.cn

#include <iostream>
来源：http://bkz.hesvh.cn

int main() { std::cout << "Hello\n"; }
来源：http://fqo.yonumen.top

[S32] C++：字符串
来源：http://mtc.shuidangran.top

std::string s = "hi";  s += "!";
来源：http://xfh.pengpengdd.cyou

[S33] C++：vector 增删
来源：http://olm.hesvh.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qwr.daria6918.cn

[S34] C++：遍历 vector
来源：http://dep.mhx1999.top

for (auto &x : v) { std::cout << x; }
来源：http://diz.haohaochexian.top

[S35] C++：map
来源：http://nhy.xuanzx.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cau.daxiang520.top

[S36] C++：unordered_map
来源：http://prb.wangdashe.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dkc.hysaishi.cn

[S37] C++：set
来源：http://puf.haohaochexian.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ffl.jyoumei.cn

[S38] C++：排序
来源：http://mad.shanyushiyangtech.top

std::sort(v.begin(), v.end());
来源：http://mkb.0kj1m.cn

[S39] C++：自定义比较器排序
来源：http://gnp.yuanzhike.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jiy.vqdsnc.cn

[S40] C++：查找元素
来源：http://zun.hnxiangtu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lro.sxryk.cn

[S41] C++：类与构造函数
来源：http://ebw.hywenlv.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sek.pengpengdd.cyou

[S42] C++：继承与虚函数
来源：http://pxp.yvedp.cn

class B : public Base { public: void f() override {} };
来源：http://viz.zycfv.cn

[S43] C++：智能指针
来源：http://rhh.zdbjq.cn

auto p = std::make_unique<int>(5);
来源：http://ntf.9152youxi.cn

[S44] C++：引用传参
来源：http://tfg.guannengcc.top

void inc(int &x) { ++x; }
来源：http://rfg.zdqjudy.top

[S45] C++：lambda
来源：http://osy.wangshuangyany.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zms.kuanghao11.cn

[S46] C++：函数模板
来源：http://hrk.redwolf501.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://niq.wangdashe.top

[S47] C++：结构化绑定遍历
来源：http://pbk.vqdsnc.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bwx.pengpengdd.cyou

[S48] C++：逐行读文件
来源：http://yol.fanxiaobao.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://nti.hnqzz.top

while (std::getline(in, line)) { }
来源：http://thk.nanxuanxn.top

[S49] C++：写文件
来源：http://fig.cucudq.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rnv.gotoacloud.top

[S50] C++：格式化数字
来源：http://mjo.zhixingplan.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ziu.jiagoushi.top

[S51] C++：显式类型转换
来源：http://hwx.guannengcc.top

static_cast<double>(a) / b
来源：http://zzk.yueranfly.top

[S52] C++：const 与 noexcept
来源：http://jlb.zhiwuduotai.top

int size() const noexcept { return n_; }
来源：http://sxe.yvedp.cn

[S53] C++：移动语义
来源：http://kcq.hysaishi.cn

std::vector<int> w = std::move(v);
来源：http://tue.c1oappe.top

[S54] C++：异常处理
来源：http://ues.bjfxy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mcs.quarkkingdee.top

[S55] C++：结构化绑定
来源：http://mvo.gogol.net.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bjl.zhengqikj.top

[S56] C++：optional
来源：http://lfa.ydjk.org.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://seg.vqdsnc.cn

[S57] C++：编译期常量
来源：http://qei.xuetiantiany.cn

constexpr int N = 10;
来源：http://bcw.nanxinkj.top

[S58] C++：命名空间
来源：http://ffg.ivvv.top

namespace ns { int f() { return 1; } }
来源：http://ury.xuetiantiany.cn

[S59] C++：静态断言
来源：http://ehw.316326.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jry.vehdjk.com

[S60] C++：遍历并删除元素
来源：http://jnx.meibo888.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xtj.wangdashe.top

================================================================================
来源：http://vgh.cheryme.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://eua.hywenlv.cn

================================================================================
来源：http://nba.smart0.xyz

[T01] Kotlin：Hello World
来源：http://zxy.fehbvm.com

println("Hello")
来源：http://bdm.guannengcc.top

[T02] Kotlin：变量
来源：http://fpr.snrcjt.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://oeg.jlsjyb.cn

[T03] Kotlin：字符串模板
来源：http://yjc.zhixingplan.top

"值: $b"
来源：http://dye.ywan-chungtsiang.top

[T04] Kotlin：空安全
来源：http://cvl.haohaochexian.top

val n: String? = null;  n?.length
来源：http://bwl.zhoulong.xyz

[T05] Kotlin：when 表达式
来源：http://spc.jqgfzy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ujz.sxryk.cn

[T06] Kotlin：集合映射
来源：http://wgx.hammf.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ymx.hesvh.cn

[T07] Kotlin：集合过滤
来源：http://nzf.jlsjyb.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://arb.ctjpmb.com

[T08] Kotlin：数据类
来源：http://its.tanke756.top

data class User(val name: String, val age: Int)
来源：http://udi.sufxvd.cn

[T09] Kotlin：扩展函数
来源：http://jge.yueranfly.top

fun String.exclaim() = this + "!"
来源：http://sfo.wangdashe.top

[T10] Kotlin：默认参数
来源：http://lpc.vqdsnc.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gkk.hesvh.cn

[T11] Kotlin：协程
来源：http://bqu.iojbl.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://add.sufxvd.cn

[T12] Kotlin：解构声明
来源：http://jiw.haohaochexian.top

val (a, b) = Pair(1, 2)
来源：http://taz.aizwys.cn

[T13] Kotlin：只读 Map
来源：http://cmv.nwbrower.top

val m = mapOf("a" to 1)
来源：http://jcd.nanxinkj.top

[T14] Kotlin：循环
来源：http://dsu.fengsongda.top

for (i in 1..10) println(i)
来源：http://bbb.andypj.xyz

[T15] Kotlin：接口
来源：http://hzi.guannengcc.top

interface Shape { fun area(): Double }
来源：http://tvb.yanxiufei.cn

[T16] Swift：Hello World
来源：http://uzk.gogol.net.cn

print("Hello")
来源：http://wxp.yj20258.top

[T17] Swift：变量与常量
来源：http://tpg.guowangkeji.top

var a = 1;  let b = 2
来源：http://cfe.havefunace.top

[T18] Swift：字符串插值
来源：http://wmq.ydzc1.top

"值: \(b)"
来源：http://iiw.316326.xyz

[T19] Swift：可选绑定
来源：http://hrg.cashguo.top

if let n = opt { print(n) }
来源：http://efk.hammf.cn

[T20] Swift：数组操作
来源：http://tqb.c1oappe.top

var a = [1, 2, 3];  a.append(4)
来源：http://jiw.snrcjt.cn

[T21] Swift：遍历
来源：http://wfj.dashuyun.cn

for x in a { print(x) }
来源：http://hps.xylfe.cn

[T22] Swift：字典
来源：http://dgg.yvedp.cn

var d = ["a": 1];  d["b"] = 2
来源：http://pul.zhijiandao.cn

[T23] Swift：函数
来源：http://lal.cashguo.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zbu.tarul.cn

[T24] Swift：闭包
来源：http://kph.uphjek.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://fhn.birdmap.top

[T25] Swift：结构体
来源：http://inz.sysykeji.top

struct P { var x: Int }
来源：http://fct.shanyushiyangkeji.top

[T26] Swift：类与重写
来源：http://dtf.vqdsnc.cn

class A: Base { override func f() {} }
来源：http://uuo.yongpay.top


<!-- 参考信息 -->