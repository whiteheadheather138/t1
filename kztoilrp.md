代发 wailian999

echo $((1 + 2 * 3))
来源：http://ntf.dianchejie.cn

[R28] 浮点运算
来源：http://ust.tianlin.xyz

echo "scale=2; 10/3" | bc
来源：http://llv.ppjwa.cn

[R29] 定义函数
来源：http://cye.gaohongyu789.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://azy.quarkkingdee.top

[R30] 函数返回状态码
来源：http://sin.shanyushiyangkeji.top

f() { return 0; }; f || echo "失败了"
来源：http://nrr.yongpay.top

[R31] 局部变量
来源：http://yuk.pengpengdd.cyou

f() { local x=1; echo "$x"; }
来源：http://lzf.pycfn.com

[R32] 参数个数校验
来源：http://rak.bjfxy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://llz.316326.xyz

[R33] 捕获错误并提示行号
来源：http://mhi.hysaishi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xrk.chenlongwang.top

[R34] 退出时清理
来源：http://sij.mhx1999.top

trap 'rm -f "$tmp"' EXIT
来源：http://csm.guowangkeji.top

[R35] 后台执行并等待
来源：http://dej.shangyingyoupin.top

sleep 5 & pid=$!; wait "$pid"
来源：http://imi.aibaodan.cn

[R36] 并发执行多个任务
来源：http://lga.vqdsnc.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tdf.sweek.top

[R37] 把输出赋给变量
来源：http://dfn.hywenlv.cn

files=$(ls -1)
来源：http://snu.birdmap.top

[R38] 管道串联
来源：http://fax.yongpay.top

cat a.txt | grep -i error | wc -l
来源：http://xrh.sufxvd.cn

[R39] 重定向标准输出与错误
来源：http://zuo.tanke756.top

cmd > out.log 2>&1
来源：http://lyj.yangfankeji.com

[R40] 追加写日志
来源：http://eiz.jlsjyb.cn

echo "log" >> out.log
来源：http://sip.dashuyun.cn

[R41] 丢弃输出
来源：http://esi.yj20258888.top

cmd >/dev/null 2>&1
来源：http://uqg.zhaomingkeji.xyz

[R42] 输入重定向
来源：http://qkg.jqgufenzy.top

wc -l < a.txt
来源：http://mne.meibo888.top

[R43] 按名字查找文件
来源：http://usg.yueranfly.top

find . -name "*.log" -type f
来源：http://rpi.hysaishi.cn

[R44] 按修改时间查找
来源：http://ljp.dianchejie.cn

find . -mtime -7 -type f
来源：http://kve.daxiang520.top

[R45] 批量删除
来源：http://wxu.hcnkem.com

find . -name "*.tmp" -delete
来源：http://znb.dashuyun.cn

[R46] 递归替换文件内容
来源：http://mwd.vehdjk.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://iaf.chenjidiqi.icu

[R47] sed 单行替换
来源：http://vcm.ywan-chungtsiang.top

sed -i 's/foo/bar/g' a.txt
来源：http://xvb.iojbl.cn

[R48] awk 取指定列
来源：http://krk.andypj.xyz

awk '{print $1, $3}' a.txt
来源：http://ane.hfpthk.cn

[R49] awk 带条件
来源：http://sct.feifeiyinyue.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hcx.ivvv.top

[R50] awk 求和
来源：http://nyf.hnqzz.top

awk '{s += $2} END {print s}' a.txt
来源：http://uwm.9152youxi.cn

[R51] 排序去重取前几
来源：http://jsa.jqgufenzy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ipp.guowangkeji.top

[R52] 统计行数
来源：http://akr.jinqigfzy.top

wc -l a.txt
来源：http://qvt.sweek.top

[R53] 查看文件头与实时尾
来源：http://dla.hfpthk.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ets.cucudq.cn

[R54] 比较两个文件
来源：http://dwp.xziqi.cn

diff a.txt b.txt
来源：http://cyt.yanxiufei.cn

[R55] 压缩与解压
来源：http://yvy.hfpthk.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hye.jinghuilouyu.cn

[R56] 远程拷贝
来源：http://dqs.guowangkeji.top

scp file user@host:/path/
来源：http://tia.yangfankeji.com

[R57] 远程执行命令
来源：http://dgn.yj20258888.top

ssh user@host 'uptime'
来源：http://uoj.jyoumei.cn

[R58] 下载文件
来源：http://zuq.fehbvm.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://krl.tarul.cn

[R59] 发 POST JSON
来源：http://ios.zycfv.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://elo.jinqigufen.top

[R60] 只看 HTTP 状态码
来源：http://ztu.dianchejie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kyg.hfpthk.cn

[R61] 磁盘占用
来源：http://zre.jinqigfzy.top

df -h;  du -sh *
来源：http://fmd.zhaomingkeji.xyz

[R62] 找最占空间的文件
来源：http://zxa.gogol.net.cn

du -ah . | sort -rh | head -10
来源：http://txl.shuidangran.top

[R63] 内存与进程
来源：http://aet.xinyue.icu

free -h;  ps aux | grep nginx
来源：http://pia.mhx1999.top

[R64] 结束进程
来源：http://smq.ctjpmb.com

kill -9 $(pgrep -f app.py)
来源：http://arp.bjfxy.top

[R65] 查看端口占用
来源：http://ths.andypj.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xau.bbcook.cn

[R66] 定时任务
来源：http://sri.sxryk.cn

crontab -e;  crontab -l
来源：http://tni.havefunace.top

[R67] 生成随机十六进制串
来源：http://xmi.tarul.cn

openssl rand -hex 16
来源：http://jtq.fanxiaobao.xyz

[R68] 计算文件校验值
来源：http://dhu.tarul.cn

sha256sum a.txt;  md5sum a.txt
来源：http://pal.nanxinkj.top

[R69] 生成随机密码
来源：http://aro.cucudq.cn

head -c 16 /dev/urandom | base64
来源：http://pvo.wangdashe.top

[R70] 时间戳与互转
来源：http://jra.guannengcc.top

date +%s;  date -d @1700000000
来源：http://far.jinghuilouyu.cn

[R71] 日期格式化
来源：http://sko.fzhhl.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://jda.yongpay.top

[R72] 等待端口就绪
来源：http://yyf.0kj1m.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fkb.yangfankeji.com

[R73] 分割大日志
来源：http://nmq.nwbrower.top

split -l 1000 big.log part_
来源：http://jan.jiagoushi.top

[R74] 批量重命名
来源：http://xbv.shanyushiyangtech.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://esi.quarkkingdee.top

[R75] 导出环境变量
来源：http://jsw.daxiang520.top

export PATH="$HOME/bin:$PATH"
来源：http://yiw.cashguo.top

[R76] 使用临时文件
来源：http://pkz.jinqigufen.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://afs.tarul.cn

[R77] 读取用户输入
来源：http://bcs.jiagoushi.top

read -rp "请输入: " ans
来源：http://jov.epnwcf.com

[R78] 交互式菜单
来源：http://sjm.ywan-chungtsiang.top

select opt in a b c; do echo "$opt"; break; done
来源：http://oer.hnqzz.top

[R79] 解析命令行选项
来源：http://owu.hysaishi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wft.yongpay.top

[R80] 查看脚本执行耗时
来源：http://sdh.yuanzhike.top

time ./run.sh
来源：http://qgk.zdbjq.cn

================================================================================
来源：http://pgf.gogol.net.cn

S. C / C++ 专题
来源：http://nxz.ybcxt.top

================================================================================
来源：http://cdi.guannengcc.top

[S01] C：Hello World
来源：http://bui.quarkkingdee.top

#include <stdio.h>
来源：http://ekp.yj202588.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://pwc.yangfankeji.com

[S02] C：变量与格式化输出
来源：http://qym.iojbl.cn

int a = 10; printf("%d\n", a);
来源：http://hia.fengsongda.top

[S03] C：读入整数
来源：http://ahn.sufxvd.cn

int x; scanf("%d", &x);
来源：http://lwl.tian-w.cn

[S04] C：字符串复制
来源：http://krv.bbcook.cn

char dst[32]; strcpy(dst, "hi");
来源：http://tpu.xuanzx.com

[S05] C：字符串长度
来源：http://och.zhaomingkeji.xyz

strlen(s)
来源：http://spe.jinyuanbaomall.cn

[S06] C：字符串比较
来源：http://pko.pycfn.com

strcmp(a, b) == 0
来源：http://cap.cdnleiting.top

[S07] C：数组遍历求和
来源：http://hwo.yj20258.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wrb.hysaishi.cn

[S08] C：动态内存分配与释放
来源：http://bia.bbcook.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kux.jqgfzy.top

[S09] C：结构体定义与初始化
来源：http://gny.xuanzx.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uhk.yanxiufei.cn

[S10] C：指针与解引用
来源：http://fvr.jinghuilouyu.cn

int *p = &a;  *p = 5;
来源：http://yva.fktsv.cn

[S11] C：逐行读文件
来源：http://xls.chenzaomai.com

FILE *f = fopen("a.txt", "r");
来源：http://qhj.yonumen.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ruo.tanke756.top

fclose(f);
来源：http://vup.zhixingplan.top

[S12] C：写文件
来源：http://frl.zhengqikj.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ota.shanyushiyangkeji.top

[S13] C：宏定义
来源：http://mka.jinghuilouyu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gwc.mhx1999.top

[S14] C：枚举
来源：http://exx.hnqzz.top

enum Color { RED, GREEN, BLUE };
来源：http://wno.feifeiyinyue.top

[S15] C：类型转换
来源：http://atr.yvedp.cn

(double) a / b
来源：http://ybr.zhixingplan.top

[S16] C：位操作置位
来源：http://ory.yj20258888.top

x |= (1 << 3);
来源：http://cnb.ywan-chungtsiang.top

[S17] C：安全拼接字符串
来源：http://ylr.cheryme.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://txp.dashuyun.cn

[S18] C：命令行参数
来源：http://kkw.smart0.xyz

int main(int argc, char **argv)
来源：http://rgb.iojbl.cn

[S19] C：快速排序
来源：http://faf.zycfv.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ojx.shzxlz.cn

[S20] C：二分查找
来源：http://dka.hcnkem.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lfo.epnwcf.com

[S21] C：字符类别判断
来源：http://eal.tarul.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bqh.uphjek.com

[S22] C：字符串转数字
来源：http://zwt.shanyushiyangtech.top

atoi("42");  strtod("3.14", NULL);
来源：http://nzu.zhongyouzk.top

[S23] C：随机数
来源：http://sng.vehdjk.com

srand(time(NULL));  int r = rand() % 100;
来源：http://lts.jianghu66.top

[S24] C：获取本地时间
来源：http://hbk.ywan-chungtsiang.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cso.jlsjyb.cn

[S25] C：内存拷贝
来源：http://wvk.hnxiangtu.top

memcpy(dst, src, n);
来源：http://scy.316326.xyz

[S26] C：内存清零
来源：http://jom.mhx1999.top

memset(a, 0, sizeof a);
来源：http://gbu.xziqi.cn

[S27] C：定义常量
来源：http://lgi.jinqigufen.top

const double PI = 3.14159;
来源：http://fcc.c1oappe.top

[S28] C：静态变量
来源：http://vgw.gotoacloud.top

static int counter = 0;
来源：http://jxm.hammf.cn

[S29] C：变参函数
来源：http://hrb.redwolf501.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nvr.yuanzhike.top

[S30] C：头文件保护
来源：http://epa.xylfe.cn

#ifndef X_H
来源：http://bql.wangdashe.top

#define X_H
来源：http://tpk.hnxiangtu.top

#endif
来源：http://wjv.xuetiantiany.cn

[S31] C++：Hello World
来源：http://eoa.shangyingyoupin.top

#include <iostream>
来源：http://qch.hcnkem.com

int main() { std::cout << "Hello\n"; }
来源：http://njk.yonumen.top

[S32] C++：字符串
来源：http://agm.nanxuanxn.top

std::string s = "hi";  s += "!";
来源：http://qwf.guowangkeji.top

[S33] C++：vector 增删
来源：http://yvl.ybcxt.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xlw.fzhhl.top

[S34] C++：遍历 vector
来源：http://ayj.zhengqikj.top

for (auto &x : v) { std::cout << x; }
来源：http://kjj.sjlbkw.cn

[S35] C++：map
来源：http://vzt.meibo888.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://oji.haohaochexian.top

[S36] C++：unordered_map
来源：http://fya.fengsongda.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jco.gogol.net.cn

[S37] C++：set
来源：http://uxs.iojbl.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tin.chenzaomai.com

[S38] C++：排序
来源：http://wsh.ppjwa.cn

std::sort(v.begin(), v.end());
来源：http://bhx.ppjwa.cn

[S39] C++：自定义比较器排序
来源：http://joj.tianlin.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vim.zhiwuduotai.top

[S40] C++：查找元素
来源：http://une.jinqigfzy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sga.jianghu66.top

[S41] C++：类与构造函数
来源：http://sij.0kj1m.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ybo.gotoacloud.top

[S42] C++：继承与虚函数
来源：http://yix.meibo888.top

class B : public Base { public: void f() override {} };
来源：http://dto.havefunace.top

[S43] C++：智能指针
来源：http://bpc.aizwys.cn

auto p = std::make_unique<int>(5);
来源：http://tro.cqqwz.cn

[S44] C++：引用传参
来源：http://fbq.c1oappe.top

void inc(int &x) { ++x; }
来源：http://bjc.mhx1999.top

[S45] C++：lambda
来源：http://twr.vqdsnc.cn

auto add = [](int a, int b) { return a + b; };
来源：http://cig.zhoulong.xyz

[S46] C++：函数模板
来源：http://ucj.cdnleiting.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jwx.jqgfzy.top

[S47] C++：结构化绑定遍历
来源：http://vjv.jqgfzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hbs.316326.xyz

[S48] C++：逐行读文件
来源：http://ril.wangdashe.top

std::ifstream in("a.txt");  std::string line;
来源：http://kjt.zhongyouzk.top

while (std::getline(in, line)) { }
来源：http://yfy.hesvh.cn

[S49] C++：写文件
来源：http://dth.pengpengdd.cyou

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ejh.ydjk.org.cn

[S50] C++：格式化数字
来源：http://enl.yueranfly.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jdz.aibaodan.cn

[S51] C++：显式类型转换
来源：http://ear.yanxiufei.cn

static_cast<double>(a) / b
来源：http://srj.ywan-chungtsiang.top

[S52] C++：const 与 noexcept
来源：http://ukn.smart0.xyz

int size() const noexcept { return n_; }
来源：http://adk.wangshuangyany.cn

[S53] C++：移动语义
来源：http://ikf.ydzc1.top

std::vector<int> w = std::move(v);
来源：http://vkz.tanke756.top

[S54] C++：异常处理
来源：http://dgp.shzxlz.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gvp.zhaomingkeji.xyz

[S55] C++：结构化绑定
来源：http://bjl.sxryk.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wdq.pycfn.com

[S56] C++：optional
来源：http://rfa.cdnleiting.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mhd.daria6918.cn

[S57] C++：编译期常量
来源：http://xpk.tian-w.cn

constexpr int N = 10;
来源：http://zab.shuidangran.top

[S58] C++：命名空间
来源：http://dry.9152youxi.cn

namespace ns { int f() { return 1; } }
来源：http://qaq.yfazqb.com

[S59] C++：静态断言
来源：http://swn.tian-w.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://foj.xylfe.cn

[S60] C++：遍历并删除元素
来源：http://uoq.xuetiantiany.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://iao.0kj1m.cn

================================================================================
来源：http://exg.jqgfzy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://iyv.dashuyun.cn

================================================================================
来源：http://qdx.ppjwa.cn

[T01] Kotlin：Hello World
来源：http://njq.hywenlv.cn

println("Hello")
来源：http://vpl.havefunace.top

[T02] Kotlin：变量
来源：http://fdf.ybcxt.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://phc.xuanzx.com

[T03] Kotlin：字符串模板
来源：http://wjb.bbcook.cn

"值: $b"
来源：http://vpg.yanxiufei.cn

[T04] Kotlin：空安全
来源：http://oae.gotoacloud.top

val n: String? = null;  n?.length
来源：http://uwm.tarul.cn

[T05] Kotlin：when 表达式
来源：http://rrt.redwolf501.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xfr.hywenlv.cn

[T06] Kotlin：集合映射
来源：http://ddx.birdmap.top

listOf(1, 2, 3).map { it * 2 }
来源：http://dwk.yj20258888.top

[T07] Kotlin：集合过滤
来源：http://fch.jiagoushi.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://sie.tanke756.top

[T08] Kotlin：数据类
来源：http://nui.yuxming.cn

data class User(val name: String, val age: Int)
来源：http://tra.tian-w.cn

[T09] Kotlin：扩展函数
来源：http://ran.quarkkingdee.top

fun String.exclaim() = this + "!"
来源：http://msk.pengpengdd.cyou

[T10] Kotlin：默认参数
来源：http://lcg.sjlbkw.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://auc.tianlin.xyz

[T11] Kotlin：协程
来源：http://eij.zhengqikj.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://vam.ivvv.top

[T12] Kotlin：解构声明
来源：http://jzi.andypj.xyz

val (a, b) = Pair(1, 2)
来源：http://kyx.hongshengwenyu.top

[T13] Kotlin：只读 Map
来源：http://vje.yj20258888.top

val m = mapOf("a" to 1)
来源：http://acf.iojbl.cn

[T14] Kotlin：循环
来源：http://urw.jinghuilouyu.cn

for (i in 1..10) println(i)
来源：http://agk.xinyue.icu

[T15] Kotlin：接口
来源：http://btm.vqdsnc.cn

interface Shape { fun area(): Double }
来源：http://vur.xinyue.icu

[T16] Swift：Hello World
来源：http://okx.yongpay.top

print("Hello")
来源：http://flw.dianchejie.cn

[T17] Swift：变量与常量
来源：http://gvq.fengsongda.top

var a = 1;  let b = 2
来源：http://hiu.chenlongwang.top

[T18] Swift：字符串插值
来源：http://fai.epnwcf.com

"值: \(b)"
来源：http://mtq.xziqi.cn

[T19] Swift：可选绑定
来源：http://ury.svipenyu.cn

if let n = opt { print(n) }
来源：http://uoe.epnwcf.com

[T20] Swift：数组操作
来源：http://urr.xingfuxueyuan.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://nzv.gzhubu.top

[T21] Swift：遍历
来源：http://fsx.ydzc1.top

for x in a { print(x) }
来源：http://wqu.nwbrower.top

[T22] Swift：字典
来源：http://uuh.jianghu66.top

var d = ["a": 1];  d["b"] = 2
来源：http://twn.ehwqpu.com

[T23] Swift：函数
来源：http://bgq.zycfv.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rqu.nanxuanxn.top

[T24] Swift：闭包
来源：http://rhb.yuanzhike.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://qcf.dianchejie.cn

[T25] Swift：结构体
来源：http://fbf.guannengcc.top

struct P { var x: Int }
来源：http://pvs.ppjwa.cn

[T26] Swift：类与重写
来源：http://iew.gzhubu.top

class A: Base { override func f() {} }
来源：http://wle.cqqwz.cn

[T27] Swift：错误处理
来源：http://lqq.gogol.net.cn

do { try f() } catch { print(error) }
来源：http://lru.shzxlz.cn

[T28] Swift：枚举
来源：http://dfe.316326.xyz

enum Color { case red, green }
来源：http://myf.0kj1m.cn

[T29] Swift：guard 提前返回
来源：http://hza.bbcook.cn

guard let x = opt else { return }
来源：http://bqk.jinyuanbaomall.cn

[T30] Swift：协议
来源：http://qtm.daria6918.cn

protocol Shape { func area() -> Double }
来源：http://alg.iojbl.cn


<!-- 参考信息 -->