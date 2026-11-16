代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hdr.jinyuanbaomall.cn

[R24] 大小写转换
来源：http://hux.havefunace.top

echo "${s^^}"; echo "${s,,}"
来源：http://qgz.cheryme.top

[R25] 去后缀 / 去前缀
来源：http://xki.guannengcc.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://zhr.jqgfzy.top

[R26] 命令替换
来源：http://tpm.c1oappe.top

now=$(date +%F); echo "$now"
来源：http://bft.hammf.cn

[R27] 算术展开
来源：http://ocy.jqgufenzy.top

echo $((1 + 2 * 3))
来源：http://sjv.yonumen.top

[R28] 浮点运算
来源：http://ala.zhoulong.xyz

echo "scale=2; 10/3" | bc
来源：http://foh.yangfankeji.com

[R29] 定义函数
来源：http://wpo.jinghuilouyu.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mxg.guannengcc.top

[R30] 函数返回状态码
来源：http://rol.nanxuanxn.top

f() { return 0; }; f || echo "失败了"
来源：http://ypj.tanke756.top

[R31] 局部变量
来源：http://kbb.wangdashe.top

f() { local x=1; echo "$x"; }
来源：http://gvn.sysykeji.top

[R32] 参数个数校验
来源：http://nsg.hywenlv.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tmg.sweek.top

[R33] 捕获错误并提示行号
来源：http://sif.zhiwuduotai.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gjw.shanyushiyangtech.top

[R34] 退出时清理
来源：http://cbn.pengpengdd.cyou

trap 'rm -f "$tmp"' EXIT
来源：http://txd.zhijiandao.cn

[R35] 后台执行并等待
来源：http://gfs.uphjek.com

sleep 5 & pid=$!; wait "$pid"
来源：http://iqg.ydjk.org.cn

[R36] 并发执行多个任务
来源：http://knr.fanxiaobao.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://swq.xinyue.icu

[R37] 把输出赋给变量
来源：http://mad.jyoumei.cn

files=$(ls -1)
来源：http://npv.guowangkeji.top

[R38] 管道串联
来源：http://pgt.daria6918.cn

cat a.txt | grep -i error | wc -l
来源：http://yvx.jqgufenzy.top

[R39] 重定向标准输出与错误
来源：http://ovd.gaohongyu789.top

cmd > out.log 2>&1
来源：http://fqv.jinqigfzy.top

[R40] 追加写日志
来源：http://lkt.vqdsnc.cn

echo "log" >> out.log
来源：http://zip.yongpay.top

[R41] 丢弃输出
来源：http://jrt.nanxuanxn.top

cmd >/dev/null 2>&1
来源：http://zlz.hnxiangtu.top

[R42] 输入重定向
来源：http://ffv.jianghu66.top

wc -l < a.txt
来源：http://buh.jinghuilouyu.cn

[R43] 按名字查找文件
来源：http://qrd.tianlin.xyz

find . -name "*.log" -type f
来源：http://slp.tanke756.top

[R44] 按修改时间查找
来源：http://vlj.cheryme.top

find . -mtime -7 -type f
来源：http://uaj.jianghu66.top

[R45] 批量删除
来源：http://gei.chenjidiqi.icu

find . -name "*.tmp" -delete
来源：http://dud.wangdashe.top

[R46] 递归替换文件内容
来源：http://hmq.xuetiantiany.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://als.yanxiufei.cn

[R47] sed 单行替换
来源：http://urr.hfpthk.cn

sed -i 's/foo/bar/g' a.txt
来源：http://gqq.chenzaomai.com

[R48] awk 取指定列
来源：http://eiu.guannengcc.top

awk '{print $1, $3}' a.txt
来源：http://tix.aizwys.cn

[R49] awk 带条件
来源：http://vwg.jyoumei.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wrt.tanke756.top

[R50] awk 求和
来源：http://bok.hongshengwenyu.top

awk '{s += $2} END {print s}' a.txt
来源：http://qtd.chenjidiqi.icu

[R51] 排序去重取前几
来源：http://lti.nanxinkj.top

sort a.txt | uniq -c | sort -rn | head
来源：http://gol.tarul.cn

[R52] 统计行数
来源：http://jpf.vqdsnc.cn

wc -l a.txt
来源：http://uzx.zhixingplan.top

[R53] 查看文件头与实时尾
来源：http://ugr.hnxiangtu.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zpa.havefunace.top

[R54] 比较两个文件
来源：http://ijz.xuetiantiany.cn

diff a.txt b.txt
来源：http://lyv.zhixingplan.top

[R55] 压缩与解压
来源：http://hss.0kj1m.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vcj.xuanzx.com

[R56] 远程拷贝
来源：http://jpy.xziqi.cn

scp file user@host:/path/
来源：http://hge.pengpengdd.cyou

[R57] 远程执行命令
来源：http://kkc.smart0.xyz

ssh user@host 'uptime'
来源：http://ywc.fzhhl.top

[R58] 下载文件
来源：http://ush.wangshuangyany.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://icx.chenlongwang.top

[R59] 发 POST JSON
来源：http://gej.yongpay.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nkk.ydzc1.top

[R60] 只看 HTTP 状态码
来源：http://fit.yfazqb.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qqz.xuetiantiany.cn

[R61] 磁盘占用
来源：http://ywz.sufxvd.cn

df -h;  du -sh *
来源：http://vtz.tanke756.top

[R62] 找最占空间的文件
来源：http://qkn.guannengcc.top

du -ah . | sort -rh | head -10
来源：http://wtx.hysaishi.cn

[R63] 内存与进程
来源：http://zbj.pengpengdd.cyou

free -h;  ps aux | grep nginx
来源：http://oyy.ydjk.org.cn

[R64] 结束进程
来源：http://olv.nanxuanxn.top

kill -9 $(pgrep -f app.py)
来源：http://hfz.yueranfly.top

[R65] 查看端口占用
来源：http://got.hnqzz.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fmf.yvedp.cn

[R66] 定时任务
来源：http://mzu.wangdashe.top

crontab -e;  crontab -l
来源：http://era.cqqwz.cn

[R67] 生成随机十六进制串
来源：http://iqb.nwbrower.top

openssl rand -hex 16
来源：http://apa.jqgufenzy.top

[R68] 计算文件校验值
来源：http://ize.cashguo.top

sha256sum a.txt;  md5sum a.txt
来源：http://pic.iojbl.cn

[R69] 生成随机密码
来源：http://dnm.fengsongda.top

head -c 16 /dev/urandom | base64
来源：http://dsb.hnxiangtu.top

[R70] 时间戳与互转
来源：http://jbp.mhx1999.top

date +%s;  date -d @1700000000
来源：http://isd.zhaomingkeji.xyz

[R71] 日期格式化
来源：http://exm.yanxiufei.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://scd.vqdsnc.cn

[R72] 等待端口就绪
来源：http://ybr.ivvv.top

until nc -z localhost 3306; do sleep 1; done
来源：http://fjp.pengpengdd.cyou

[R73] 分割大日志
来源：http://jes.sweek.top

split -l 1000 big.log part_
来源：http://rwe.c1oappe.top

[R74] 批量重命名
来源：http://orl.c1oappe.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ecq.yfazqb.com

[R75] 导出环境变量
来源：http://cqo.ybcxt.top

export PATH="$HOME/bin:$PATH"
来源：http://fqv.bjfxy.top

[R76] 使用临时文件
来源：http://shx.0kj1m.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://das.meibo888.top

[R77] 读取用户输入
来源：http://jhg.cdnleiting.top

read -rp "请输入: " ans
来源：http://ryg.yangfankeji.com

[R78] 交互式菜单
来源：http://poc.haohaochexian.top

select opt in a b c; do echo "$opt"; break; done
来源：http://nka.chenzaomai.com

[R79] 解析命令行选项
来源：http://pfm.tian-w.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qof.wangshuangyany.cn

[R80] 查看脚本执行耗时
来源：http://ikh.fzhhl.top

time ./run.sh
来源：http://xzc.smart0.xyz

================================================================================
来源：http://sto.jqgufenzy.top

S. C / C++ 专题
来源：http://pev.zhixingplan.top

================================================================================
来源：http://vpt.yonumen.top

[S01] C：Hello World
来源：http://mig.daria6918.cn

#include <stdio.h>
来源：http://zog.zhixingplan.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://zot.snrcjt.cn

[S02] C：变量与格式化输出
来源：http://faw.tian-w.cn

int a = 10; printf("%d\n", a);
来源：http://rkg.sufxvd.cn

[S03] C：读入整数
来源：http://yvp.shangyingyoupin.top

int x; scanf("%d", &x);
来源：http://syr.xuetiantiany.cn

[S04] C：字符串复制
来源：http://dcf.jlsjyb.cn

char dst[32]; strcpy(dst, "hi");
来源：http://fzg.gogol.net.cn

[S05] C：字符串长度
来源：http://guv.shuidangran.top

strlen(s)
来源：http://xcf.zhoulong.xyz

[S06] C：字符串比较
来源：http://vdm.snrcjt.cn

strcmp(a, b) == 0
来源：http://gau.ehwqpu.com

[S07] C：数组遍历求和
来源：http://asp.jqgufenzy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rng.xuanzx.com

[S08] C：动态内存分配与释放
来源：http://lap.cheryme.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sxi.jinghuilouyu.cn

[S09] C：结构体定义与初始化
来源：http://sfr.iojbl.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://peg.havefunace.top

[S10] C：指针与解引用
来源：http://cnl.zhongyouzk.top

int *p = &a;  *p = 5;
来源：http://csm.fanxiaobao.xyz

[S11] C：逐行读文件
来源：http://trk.hysaishi.cn

FILE *f = fopen("a.txt", "r");
来源：http://oak.fktsv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ppf.yuanzhike.top

fclose(f);
来源：http://ipt.wangdashe.top

[S12] C：写文件
来源：http://lag.xylfe.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hih.jinqigfzy.top

[S13] C：宏定义
来源：http://bao.epnwcf.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ewv.cucudq.cn

[S14] C：枚举
来源：http://fhz.yonumen.top

enum Color { RED, GREEN, BLUE };
来源：http://dzc.hammf.cn

[S15] C：类型转换
来源：http://qna.zdqjudy.top

(double) a / b
来源：http://gik.jiagoushi.top

[S16] C：位操作置位
来源：http://ziu.ywan-chungtsiang.top

x |= (1 << 3);
来源：http://jcc.yj202588.top

[S17] C：安全拼接字符串
来源：http://ieu.zhongyouzk.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kmp.daxiang520.top

[S18] C：命令行参数
来源：http://xrj.yj20258.top

int main(int argc, char **argv)
来源：http://fmz.ehwqpu.com

[S19] C：快速排序
来源：http://dqd.ehwqpu.com

qsort(a, n, sizeof(int), cmp);
来源：http://dpe.epnwcf.com

[S20] C：二分查找
来源：http://elr.zdbjq.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nzn.fktsv.cn

[S21] C：字符类别判断
来源：http://yfh.nwbrower.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://owm.sxryk.cn

[S22] C：字符串转数字
来源：http://wcb.sxryk.cn

atoi("42");  strtod("3.14", NULL);
来源：http://inu.mhx1999.top

[S23] C：随机数
来源：http://xet.fzhhl.top

srand(time(NULL));  int r = rand() % 100;
来源：http://bgl.chenjidiqi.icu

[S24] C：获取本地时间
来源：http://zhk.fengsongda.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jdt.haohaochexian.top

[S25] C：内存拷贝
来源：http://uht.dashuyun.cn

memcpy(dst, src, n);
来源：http://szy.yvedp.cn

[S26] C：内存清零
来源：http://qgt.jqgufenzy.top

memset(a, 0, sizeof a);
来源：http://ivj.316326.xyz

[S27] C：定义常量
来源：http://eis.nwbrower.top

const double PI = 3.14159;
来源：http://qrs.jinyuanbaomall.cn

[S28] C：静态变量
来源：http://nje.nanxuanxn.top

static int counter = 0;
来源：http://apv.zhiwuduotai.top

[S29] C：变参函数
来源：http://mxh.yangfankeji.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cee.zhaomingkeji.xyz

[S30] C：头文件保护
来源：http://jni.iojbl.cn

#ifndef X_H
来源：http://ldf.sxryk.cn

#define X_H
来源：http://fzu.jiagoushi.top

#endif
来源：http://xhw.andypj.xyz

[S31] C++：Hello World
来源：http://haz.ivvv.top

#include <iostream>
来源：http://egj.jinqigfzy.top

int main() { std::cout << "Hello\n"; }
来源：http://dne.xziqi.cn

[S32] C++：字符串
来源：http://jpx.epnwcf.com

std::string s = "hi";  s += "!";
来源：http://sfz.cucudq.cn

[S33] C++：vector 增删
来源：http://iqd.yanxiufei.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fwy.hesvh.cn

[S34] C++：遍历 vector
来源：http://yqi.havefunace.top

for (auto &x : v) { std::cout << x; }
来源：http://xmv.yueranfly.top

[S35] C++：map
来源：http://ewn.tanke756.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://uha.cheryme.top

[S36] C++：unordered_map
来源：http://zvo.jqgufenzy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jzy.sweek.top

[S37] C++：set
来源：http://xwg.zhijiandao.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://onp.chenlongwang.top

[S38] C++：排序
来源：http://pqd.zhaomingkeji.xyz

std::sort(v.begin(), v.end());
来源：http://eoc.yj20258.top

[S39] C++：自定义比较器排序
来源：http://pee.cashguo.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jpm.gzhubu.top

[S40] C++：查找元素
来源：http://oml.jinqigfzy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rjh.cashguo.top

[S41] C++：类与构造函数
来源：http://hzn.zdbjq.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dsd.yuxming.cn

[S42] C++：继承与虚函数
来源：http://usx.tian-w.cn

class B : public Base { public: void f() override {} };
来源：http://nbe.xylfe.cn

[S43] C++：智能指针
来源：http://mcl.hywenlv.cn

auto p = std::make_unique<int>(5);
来源：http://nct.chenjidiqi.icu

[S44] C++：引用传参
来源：http://nme.jqgufenzy.top

void inc(int &x) { ++x; }
来源：http://ygg.zdbjq.cn

[S45] C++：lambda
来源：http://tnu.hongshengwenyu.top

auto add = [](int a, int b) { return a + b; };
来源：http://ktu.ctjpmb.com

[S46] C++：函数模板
来源：http://xsi.chenzaomai.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tex.hywenlv.cn

[S47] C++：结构化绑定遍历
来源：http://ybf.nwbrower.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://axb.hnqzz.top

[S48] C++：逐行读文件
来源：http://idu.zdbjq.cn

std::ifstream in("a.txt");  std::string line;
来源：http://bif.yuxming.cn

while (std::getline(in, line)) { }
来源：http://ihg.epnwcf.com

[S49] C++：写文件
来源：http://kyl.zhongyouzk.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xtc.ybcxt.top

[S50] C++：格式化数字
来源：http://bsu.cqqwz.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uyh.zhaomingkeji.xyz

[S51] C++：显式类型转换
来源：http://jgu.sweek.top

static_cast<double>(a) / b
来源：http://jzm.hongshengwenyu.top

[S52] C++：const 与 noexcept
来源：http://cxc.haohaochexian.top

int size() const noexcept { return n_; }
来源：http://tav.daria6918.cn

[S53] C++：移动语义
来源：http://pdo.hfpthk.cn

std::vector<int> w = std::move(v);
来源：http://aqr.ppjwa.cn

[S54] C++：异常处理
来源：http://nks.sufxvd.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bhz.hesvh.cn

[S55] C++：结构化绑定
来源：http://qtl.zhiwuduotai.top

auto [a, b] = std::make_pair(1, 2);
来源：http://keu.xuetiantiany.cn

[S56] C++：optional
来源：http://ywo.tarul.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://raq.andypj.xyz

[S57] C++：编译期常量
来源：http://vtl.chenlongwang.top

constexpr int N = 10;
来源：http://gex.feifeiyinyue.top

[S58] C++：命名空间
来源：http://tci.svipenyu.cn

namespace ns { int f() { return 1; } }
来源：http://jzq.hammf.cn

[S59] C++：静态断言
来源：http://ihk.xuetiantiany.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lbz.tianlin.xyz

[S60] C++：遍历并删除元素
来源：http://yau.hfpthk.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cmv.xinyue.icu

================================================================================
来源：http://aup.vqdsnc.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dbu.yongpay.top

================================================================================
来源：http://psg.sxryk.cn

[T01] Kotlin：Hello World
来源：http://xqm.jinyuanbaomall.cn

println("Hello")
来源：http://fyq.smart0.xyz

[T02] Kotlin：变量
来源：http://wzp.yonumen.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cdr.snrcjt.cn

[T03] Kotlin：字符串模板
来源：http://ban.zhijiandao.cn

"值: $b"
来源：http://ayf.kuanghao11.cn

[T04] Kotlin：空安全
来源：http://dul.haohaochexian.top

val n: String? = null;  n?.length
来源：http://lsc.sysykeji.top

[T05] Kotlin：when 表达式
来源：http://kzk.aibaodan.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://def.pengpengdd.cyou

[T06] Kotlin：集合映射
来源：http://qdc.zhijiandao.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://wwi.yuxming.cn

[T07] Kotlin：集合过滤
来源：http://ufd.cdnleiting.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://dpl.316326.xyz

[T08] Kotlin：数据类
来源：http://cyh.svipenyu.cn

data class User(val name: String, val age: Int)
来源：http://rku.gogol.net.cn

[T09] Kotlin：扩展函数
来源：http://kur.zdqjudy.top

fun String.exclaim() = this + "!"
来源：http://smy.ybcxt.top

[T10] Kotlin：默认参数
来源：http://hwb.havefunace.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ole.zhoulong.xyz

[T11] Kotlin：协程
来源：http://mvd.bbcook.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://rtc.aibaodan.cn

[T12] Kotlin：解构声明
来源：http://aye.pycfn.com

val (a, b) = Pair(1, 2)
来源：http://lab.bjfxy.top

[T13] Kotlin：只读 Map
来源：http://igj.snrcjt.cn

val m = mapOf("a" to 1)
来源：http://rkx.cucudq.cn

[T14] Kotlin：循环
来源：http://str.vqdsnc.cn

for (i in 1..10) println(i)
来源：http://mxh.316326.xyz

[T15] Kotlin：接口
来源：http://jyy.xuanzx.com

interface Shape { fun area(): Double }
来源：http://adl.xziqi.cn

[T16] Swift：Hello World
来源：http://seo.mhx1999.top

print("Hello")
来源：http://mmz.dashuyun.cn

[T17] Swift：变量与常量
来源：http://wgd.zhiwuduotai.top

var a = 1;  let b = 2
来源：http://mcp.meibo888.top

[T18] Swift：字符串插值
来源：http://kor.guannengcc.top

"值: \(b)"
来源：http://hox.tianlin.xyz

[T19] Swift：可选绑定
来源：http://svj.birdmap.top

if let n = opt { print(n) }
来源：http://ygz.yonumen.top

[T20] Swift：数组操作
来源：http://jix.shuidangran.top

var a = [1, 2, 3];  a.append(4)
来源：http://eex.jinqigfzy.top

[T21] Swift：遍历
来源：http://jbn.guowangkeji.top

for x in a { print(x) }
来源：http://spt.snrcjt.cn

[T22] Swift：字典
来源：http://ebe.gaohongyu789.top

var d = ["a": 1];  d["b"] = 2
来源：http://etz.svipenyu.cn

[T23] Swift：函数
来源：http://mnx.ivvv.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fqc.52xcode.cn

[T24] Swift：闭包
来源：http://cjt.feifeiyinyue.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://lea.zhoulong.xyz

[T25] Swift：结构体
来源：http://mjo.svipenyu.cn

struct P { var x: Int }
来源：http://mld.yueranfly.top

[T26] Swift：类与重写
来源：http://fly.chenjidiqi.icu

class A: Base { override func f() {} }
来源：http://ixh.ivvv.top


<!-- 参考信息 -->