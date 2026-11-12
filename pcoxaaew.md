代发 wailian999

echo $((1 + 2 * 3))
来源：http://xus.epnwcf.com

[R28] 浮点运算
来源：http://ivb.fzhhl.top

echo "scale=2; 10/3" | bc
来源：http://jtw.ywan-chungtsiang.top

[R29] 定义函数
来源：http://nys.52xcode.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://srj.aibaodan.cn

[R30] 函数返回状态码
来源：http://bcu.tian-w.cn

f() { return 0; }; f || echo "失败了"
来源：http://mxy.jinqigfzy.top

[R31] 局部变量
来源：http://tpx.jianghu66.top

f() { local x=1; echo "$x"; }
来源：http://tmi.yonumen.top

[R32] 参数个数校验
来源：http://sfv.jinghuilouyu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yum.cqqwz.cn

[R33] 捕获错误并提示行号
来源：http://udw.daxiang520.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ovp.ydzc1.top

[R34] 退出时清理
来源：http://vrg.xuanzx.com

trap 'rm -f "$tmp"' EXIT
来源：http://djz.tanke756.top

[R35] 后台执行并等待
来源：http://ciu.zhaomingkeji.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://xea.xuetiantiany.cn

[R36] 并发执行多个任务
来源：http://igw.pengpengdd.cyou

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://spg.xylfe.cn

[R37] 把输出赋给变量
来源：http://kpt.yongpay.top

files=$(ls -1)
来源：http://sgu.yj202588.top

[R38] 管道串联
来源：http://zxg.jinyuanbaomall.cn

cat a.txt | grep -i error | wc -l
来源：http://zfc.xylfe.cn

[R39] 重定向标准输出与错误
来源：http://mkz.hysaishi.cn

cmd > out.log 2>&1
来源：http://ytq.sufxvd.cn

[R40] 追加写日志
来源：http://xeu.zhixingplan.top

echo "log" >> out.log
来源：http://ngo.shangyingyoupin.top

[R41] 丢弃输出
来源：http://mxj.kuanghao11.cn

cmd >/dev/null 2>&1
来源：http://wcf.dianchejie.cn

[R42] 输入重定向
来源：http://npi.zhongyouzk.top

wc -l < a.txt
来源：http://txp.jinqigfzy.top

[R43] 按名字查找文件
来源：http://sru.fehbvm.com

find . -name "*.log" -type f
来源：http://vgc.vehdjk.com

[R44] 按修改时间查找
来源：http://xla.yj20258888.top

find . -mtime -7 -type f
来源：http://ylv.pengpengdd.cyou

[R45] 批量删除
来源：http://ntb.yfazqb.com

find . -name "*.tmp" -delete
来源：http://xjn.zhijiandao.cn

[R46] 递归替换文件内容
来源：http://yvc.jyoumei.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dfr.meibo888.top

[R47] sed 单行替换
来源：http://nya.svipenyu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hxh.gzhubu.top

[R48] awk 取指定列
来源：http://fqu.yongpay.top

awk '{print $1, $3}' a.txt
来源：http://pja.shanyushiyangkeji.top

[R49] awk 带条件
来源：http://gjb.nwbrower.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://riz.ctjpmb.com

[R50] awk 求和
来源：http://zaw.iojbl.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wnc.iojbl.cn

[R51] 排序去重取前几
来源：http://xns.haohaochexian.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ruf.jinghuilouyu.cn

[R52] 统计行数
来源：http://met.redwolf501.top

wc -l a.txt
来源：http://wal.zdbjq.cn

[R53] 查看文件头与实时尾
来源：http://uke.52xcode.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dko.ywan-chungtsiang.top

[R54] 比较两个文件
来源：http://und.cashguo.top

diff a.txt b.txt
来源：http://mee.vehdjk.com

[R55] 压缩与解压
来源：http://iuk.aizwys.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://iyr.jinqigufen.top

[R56] 远程拷贝
来源：http://yet.fzhhl.top

scp file user@host:/path/
来源：http://znb.yueranfly.top

[R57] 远程执行命令
来源：http://hhr.zhixingplan.top

ssh user@host 'uptime'
来源：http://sqw.ydjk.org.cn

[R58] 下载文件
来源：http://cye.dashuyun.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mqg.bjfxy.top

[R59] 发 POST JSON
来源：http://pid.daxiang520.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cwb.xziqi.cn

[R60] 只看 HTTP 状态码
来源：http://jwt.ctjpmb.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qao.nanxuanxn.top

[R61] 磁盘占用
来源：http://rol.gzhubu.top

df -h;  du -sh *
来源：http://xsu.wangshuangyany.cn

[R62] 找最占空间的文件
来源：http://nbk.zycfv.cn

du -ah . | sort -rh | head -10
来源：http://sog.cucudq.cn

[R63] 内存与进程
来源：http://ynt.zdbjq.cn

free -h;  ps aux | grep nginx
来源：http://bwu.jinqigfzy.top

[R64] 结束进程
来源：http://wjy.cdnleiting.top

kill -9 $(pgrep -f app.py)
来源：http://wmv.dianchejie.cn

[R65] 查看端口占用
来源：http://mgx.tian-w.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://teo.yvedp.cn

[R66] 定时任务
来源：http://nqs.gaohongyu789.top

crontab -e;  crontab -l
来源：http://lqo.shanyushiyangtech.top

[R67] 生成随机十六进制串
来源：http://pla.zhiwuduotai.top

openssl rand -hex 16
来源：http://mln.bbcook.cn

[R68] 计算文件校验值
来源：http://jrn.sjlbkw.cn

sha256sum a.txt;  md5sum a.txt
来源：http://iwi.9152youxi.cn

[R69] 生成随机密码
来源：http://ppc.c1oappe.top

head -c 16 /dev/urandom | base64
来源：http://byr.jqgfzy.top

[R70] 时间戳与互转
来源：http://lll.vehdjk.com

date +%s;  date -d @1700000000
来源：http://xsr.cheryme.top

[R71] 日期格式化
来源：http://iyc.daxiang520.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://jhy.uphjek.com

[R72] 等待端口就绪
来源：http://owf.xingfuxueyuan.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://prc.bbcook.cn

[R73] 分割大日志
来源：http://knp.ehwqpu.com

split -l 1000 big.log part_
来源：http://nti.zhijiandao.cn

[R74] 批量重命名
来源：http://pta.jlsjyb.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cbc.nanxinkj.top

[R75] 导出环境变量
来源：http://bdf.xinyue.icu

export PATH="$HOME/bin:$PATH"
来源：http://nnc.bbcook.cn

[R76] 使用临时文件
来源：http://klr.hcnkem.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bnt.yueranfly.top

[R77] 读取用户输入
来源：http://crn.quarkkingdee.top

read -rp "请输入: " ans
来源：http://zja.birdmap.top

[R78] 交互式菜单
来源：http://sdu.jiagoushi.top

select opt in a b c; do echo "$opt"; break; done
来源：http://flx.yuxming.cn

[R79] 解析命令行选项
来源：http://igx.mhx1999.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dkt.nanxuanxn.top

[R80] 查看脚本执行耗时
来源：http://jvi.xziqi.cn

time ./run.sh
来源：http://gzw.ybcxt.top

================================================================================
来源：http://hog.ivvv.top

S. C / C++ 专题
来源：http://nsv.ctjpmb.com

================================================================================
来源：http://sfw.c1oappe.top

[S01] C：Hello World
来源：http://tll.sysykeji.top

#include <stdio.h>
来源：http://ghl.nwbrower.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://qlk.mhx1999.top

[S02] C：变量与格式化输出
来源：http://xdw.uphjek.com

int a = 10; printf("%d\n", a);
来源：http://wmm.ppjwa.cn

[S03] C：读入整数
来源：http://xet.jqgufenzy.top

int x; scanf("%d", &x);
来源：http://ypw.yuanzhike.top

[S04] C：字符串复制
来源：http://zoe.yuxming.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wqt.zycfv.cn

[S05] C：字符串长度
来源：http://hog.jianghu66.top

strlen(s)
来源：http://nib.xingfuxueyuan.xyz

[S06] C：字符串比较
来源：http://gsc.chenzaomai.com

strcmp(a, b) == 0
来源：http://tpc.gogol.net.cn

[S07] C：数组遍历求和
来源：http://mlh.dashuyun.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hsd.zhongyouzk.top

[S08] C：动态内存分配与释放
来源：http://vll.zhaomingkeji.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ztl.9152youxi.cn

[S09] C：结构体定义与初始化
来源：http://rdf.cdnleiting.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lrw.hongshengwenyu.top

[S10] C：指针与解引用
来源：http://zcy.svipenyu.cn

int *p = &a;  *p = 5;
来源：http://qmq.yuxming.cn

[S11] C：逐行读文件
来源：http://yyj.sxryk.cn

FILE *f = fopen("a.txt", "r");
来源：http://hio.yj202588.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://wlk.shzxlz.cn

fclose(f);
来源：http://mwq.hammf.cn

[S12] C：写文件
来源：http://hwz.yongpay.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pxm.yongpay.top

[S13] C：宏定义
来源：http://svf.xuetiantiany.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://uen.redwolf501.top

[S14] C：枚举
来源：http://goa.ydjk.org.cn

enum Color { RED, GREEN, BLUE };
来源：http://yhl.guowangkeji.top

[S15] C：类型转换
来源：http://ygq.nwbrower.top

(double) a / b
来源：http://nbo.mhx1999.top

[S16] C：位操作置位
来源：http://ntb.gogol.net.cn

x |= (1 << 3);
来源：http://zke.xinyue.icu

[S17] C：安全拼接字符串
来源：http://xyx.kuanghao11.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://urt.shanyushiyangkeji.top

[S18] C：命令行参数
来源：http://hah.jinqigfzy.top

int main(int argc, char **argv)
来源：http://kjk.sxryk.cn

[S19] C：快速排序
来源：http://gsj.gotoacloud.top

qsort(a, n, sizeof(int), cmp);
来源：http://xbf.havefunace.top

[S20] C：二分查找
来源：http://vkd.kuanghao11.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vvz.gaohongyu789.top

[S21] C：字符类别判断
来源：http://fdu.xylfe.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tul.gzhubu.top

[S22] C：字符串转数字
来源：http://ysi.svipenyu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://bmr.chenlongwang.top

[S23] C：随机数
来源：http://bne.haohaochexian.top

srand(time(NULL));  int r = rand() % 100;
来源：http://cde.ppjwa.cn

[S24] C：获取本地时间
来源：http://tos.yuanzhike.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gkn.bjfxy.top

[S25] C：内存拷贝
来源：http://jij.guowangkeji.top

memcpy(dst, src, n);
来源：http://veb.tanke756.top

[S26] C：内存清零
来源：http://iru.jqgufenzy.top

memset(a, 0, sizeof a);
来源：http://hsj.316326.xyz

[S27] C：定义常量
来源：http://myf.yj20258.top

const double PI = 3.14159;
来源：http://anj.ppjwa.cn

[S28] C：静态变量
来源：http://vwf.tarul.cn

static int counter = 0;
来源：http://uyj.gogol.net.cn

[S29] C：变参函数
来源：http://ypd.birdmap.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jof.sjlbkw.cn

[S30] C：头文件保护
来源：http://puk.daxiang520.top

#ifndef X_H
来源：http://shy.sjlbkw.cn

#define X_H
来源：http://vvj.uphjek.com

#endif
来源：http://qpg.xuetiantiany.cn

[S31] C++：Hello World
来源：http://oex.yuxming.cn

#include <iostream>
来源：http://cai.zhiwuduotai.top

int main() { std::cout << "Hello\n"; }
来源：http://eag.fktsv.cn

[S32] C++：字符串
来源：http://euv.yanxiufei.cn

std::string s = "hi";  s += "!";
来源：http://ont.yueranfly.top

[S33] C++：vector 增删
来源：http://jgw.xuetiantiany.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wlo.sufxvd.cn

[S34] C++：遍历 vector
来源：http://szg.shanyushiyangtech.top

for (auto &x : v) { std::cout << x; }
来源：http://dnc.zhoulong.xyz

[S35] C++：map
来源：http://pkm.shanyushiyangkeji.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yji.zdqjudy.top

[S36] C++：unordered_map
来源：http://cqi.yongpay.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://iaw.hongshengwenyu.top

[S37] C++：set
来源：http://pfq.jqgufenzy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dig.yuxming.cn

[S38] C++：排序
来源：http://xbs.zdqjudy.top

std::sort(v.begin(), v.end());
来源：http://top.sjlbkw.cn

[S39] C++：自定义比较器排序
来源：http://yuv.dashuyun.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tyt.xuetiantiany.cn

[S40] C++：查找元素
来源：http://xci.yfazqb.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gdo.wangshuangyany.cn

[S41] C++：类与构造函数
来源：http://yfl.yueranfly.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qqc.nwbrower.top

[S42] C++：继承与虚函数
来源：http://usz.shangyingyoupin.top

class B : public Base { public: void f() override {} };
来源：http://ykf.aizwys.cn

[S43] C++：智能指针
来源：http://dns.quarkkingdee.top

auto p = std::make_unique<int>(5);
来源：http://bty.vqdsnc.cn

[S44] C++：引用传参
来源：http://jtp.52xcode.cn

void inc(int &x) { ++x; }
来源：http://erp.hnxiangtu.top

[S45] C++：lambda
来源：http://qlg.ppjwa.cn

auto add = [](int a, int b) { return a + b; };
来源：http://rsb.zhaomingkeji.xyz

[S46] C++：函数模板
来源：http://tsf.nanxinkj.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://eqp.jqgfzy.top

[S47] C++：结构化绑定遍历
来源：http://ryw.jinqigfzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rfy.yj202588.top

[S48] C++：逐行读文件
来源：http://yvn.tanke756.top

std::ifstream in("a.txt");  std::string line;
来源：http://wdw.jqgufenzy.top

while (std::getline(in, line)) { }
来源：http://nxt.hcnkem.com

[S49] C++：写文件
来源：http://ook.jlsjyb.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jsk.xinyue.icu

[S50] C++：格式化数字
来源：http://whg.xziqi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://aai.fehbvm.com

[S51] C++：显式类型转换
来源：http://hnp.chenlongwang.top

static_cast<double>(a) / b
来源：http://dme.haohaochexian.top

[S52] C++：const 与 noexcept
来源：http://rxt.sysykeji.top

int size() const noexcept { return n_; }
来源：http://yub.yangfankeji.com

[S53] C++：移动语义
来源：http://cyz.zhaomingkeji.xyz

std::vector<int> w = std::move(v);
来源：http://ltl.jiagoushi.top

[S54] C++：异常处理
来源：http://nul.gogol.net.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cbd.fktsv.cn

[S55] C++：结构化绑定
来源：http://osy.9152youxi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://dsp.zhengqikj.top

[S56] C++：optional
来源：http://yyf.jinyuanbaomall.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dva.jinghuilouyu.cn

[S57] C++：编译期常量
来源：http://gho.xziqi.cn

constexpr int N = 10;
来源：http://alc.hammf.cn

[S58] C++：命名空间
来源：http://qna.c1oappe.top

namespace ns { int f() { return 1; } }
来源：http://lqc.ehwqpu.com

[S59] C++：静态断言
来源：http://ovc.yj20258.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nbv.yj202588.top

[S60] C++：遍历并删除元素
来源：http://bgl.gaohongyu789.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://iis.zycfv.cn

================================================================================
来源：http://isb.wangdashe.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zqk.fanxiaobao.xyz

================================================================================
来源：http://aoy.xingfuxueyuan.xyz

[T01] Kotlin：Hello World
来源：http://mjl.gotoacloud.top

println("Hello")
来源：http://uvf.dianchejie.cn

[T02] Kotlin：变量
来源：http://lox.tanke756.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yzy.pycfn.com

[T03] Kotlin：字符串模板
来源：http://mgi.nwbrower.top

"值: $b"
来源：http://rlk.daria6918.cn

[T04] Kotlin：空安全
来源：http://grx.xuetiantiany.cn

val n: String? = null;  n?.length
来源：http://xoe.gogol.net.cn

[T05] Kotlin：when 表达式
来源：http://ski.hfpthk.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://phn.c1oappe.top

[T06] Kotlin：集合映射
来源：http://xfq.cashguo.top

listOf(1, 2, 3).map { it * 2 }
来源：http://hea.epnwcf.com

[T07] Kotlin：集合过滤
来源：http://acg.yueranfly.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://avi.svipenyu.cn

[T08] Kotlin：数据类
来源：http://lhf.jinqigufen.top

data class User(val name: String, val age: Int)
来源：http://qcx.uphjek.com

[T09] Kotlin：扩展函数
来源：http://ycq.hfpthk.cn

fun String.exclaim() = this + "!"
来源：http://ksv.sysykeji.top

[T10] Kotlin：默认参数
来源：http://onx.fktsv.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://clo.guannengcc.top

[T11] Kotlin：协程
来源：http://zzk.ydzc1.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://fpe.vqdsnc.cn

[T12] Kotlin：解构声明
来源：http://utv.dianchejie.cn

val (a, b) = Pair(1, 2)
来源：http://nqz.shangyingyoupin.top

[T13] Kotlin：只读 Map
来源：http://fzm.tarul.cn

val m = mapOf("a" to 1)
来源：http://srw.zhoulong.xyz

[T14] Kotlin：循环
来源：http://zoz.shzxlz.cn

for (i in 1..10) println(i)
来源：http://omp.cdnleiting.top

[T15] Kotlin：接口
来源：http://ntr.guannengcc.top

interface Shape { fun area(): Double }
来源：http://qku.chenzaomai.com

[T16] Swift：Hello World
来源：http://ocs.daxiang520.top

print("Hello")
来源：http://xho.andypj.xyz

[T17] Swift：变量与常量
来源：http://efl.yuanzhike.top

var a = 1;  let b = 2
来源：http://zyd.jinyuanbaomall.cn

[T18] Swift：字符串插值
来源：http://vil.cucudq.cn

"值: \(b)"
来源：http://gjz.vehdjk.com

[T19] Swift：可选绑定
来源：http://loe.hywenlv.cn

if let n = opt { print(n) }
来源：http://hqi.tian-w.cn

[T20] Swift：数组操作
来源：http://oin.cqqwz.cn

var a = [1, 2, 3];  a.append(4)
来源：http://vpq.fehbvm.com

[T21] Swift：遍历
来源：http://znz.redwolf501.top

for x in a { print(x) }
来源：http://lsr.jinyuanbaomall.cn

[T22] Swift：字典
来源：http://jek.dashuyun.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fcz.316326.xyz

[T23] Swift：函数
来源：http://owk.ydjk.org.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tyd.wangshuangyany.cn

[T24] Swift：闭包
来源：http://cjm.shangyingyoupin.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://eds.tian-w.cn

[T25] Swift：结构体
来源：http://qbe.zhiwuduotai.top

struct P { var x: Int }
来源：http://jmu.snrcjt.cn

[T26] Swift：类与重写
来源：http://ysl.andypj.xyz

class A: Base { override func f() {} }
来源：http://exh.nanxinkj.top

[T27] Swift：错误处理
来源：http://vfe.ehwqpu.com

do { try f() } catch { print(error) }
来源：http://vip.ydjk.org.cn

[T28] Swift：枚举
来源：http://iua.9152youxi.cn

enum Color { case red, green }
来源：http://nms.svipenyu.cn

[T29] Swift：guard 提前返回
来源：http://cvv.meibo888.top

guard let x = opt else { return }
来源：http://soi.vehdjk.com

[T30] Swift：协议
来源：http://ney.yongpay.top

protocol Shape { func area() -> Double }
来源：http://joo.tian-w.cn


<!-- 参考信息 -->