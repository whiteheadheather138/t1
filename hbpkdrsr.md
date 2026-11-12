代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://dgn.zhongyouzk.top

[R26] 命令替换
来源：http://ncs.ppjwa.cn

now=$(date +%F); echo "$now"
来源：http://rxk.0kj1m.cn

[R27] 算术展开
来源：http://dsp.andypj.xyz

echo $((1 + 2 * 3))
来源：http://zse.ppjwa.cn

[R28] 浮点运算
来源：http://hdn.smart0.xyz

echo "scale=2; 10/3" | bc
来源：http://fsn.hfpthk.cn

[R29] 定义函数
来源：http://dgb.yfazqb.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jyb.uphjek.com

[R30] 函数返回状态码
来源：http://iqk.jianghu66.top

f() { return 0; }; f || echo "失败了"
来源：http://wnc.wangshuangyany.cn

[R31] 局部变量
来源：http://uhg.cdnleiting.top

f() { local x=1; echo "$x"; }
来源：http://khz.zdqjudy.top

[R32] 参数个数校验
来源：http://jgd.pengpengdd.cyou

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pkv.ivvv.top

[R33] 捕获错误并提示行号
来源：http://agk.ivvv.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hey.pengpengdd.cyou

[R34] 退出时清理
来源：http://xev.yueranfly.top

trap 'rm -f "$tmp"' EXIT
来源：http://vbj.xingfuxueyuan.xyz

[R35] 后台执行并等待
来源：http://kao.jqgfzy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://eit.hammf.cn

[R36] 并发执行多个任务
来源：http://fzv.kuanghao11.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://msm.cucudq.cn

[R37] 把输出赋给变量
来源：http://wda.52xcode.cn

files=$(ls -1)
来源：http://mcz.zhengqikj.top

[R38] 管道串联
来源：http://fmu.9152youxi.cn

cat a.txt | grep -i error | wc -l
来源：http://eml.hesvh.cn

[R39] 重定向标准输出与错误
来源：http://hvi.gaohongyu789.top

cmd > out.log 2>&1
来源：http://qli.ydzc1.top

[R40] 追加写日志
来源：http://adf.zhaomingkeji.xyz

echo "log" >> out.log
来源：http://wfa.dashuyun.cn

[R41] 丢弃输出
来源：http://vfu.316326.xyz

cmd >/dev/null 2>&1
来源：http://fic.guannengcc.top

[R42] 输入重定向
来源：http://efh.daxiang520.top

wc -l < a.txt
来源：http://bod.epnwcf.com

[R43] 按名字查找文件
来源：http://mnq.yvedp.cn

find . -name "*.log" -type f
来源：http://plh.hammf.cn

[R44] 按修改时间查找
来源：http://ddq.cashguo.top

find . -mtime -7 -type f
来源：http://lkw.ctjpmb.com

[R45] 批量删除
来源：http://fhz.hnqzz.top

find . -name "*.tmp" -delete
来源：http://wos.chenlongwang.top

[R46] 递归替换文件内容
来源：http://zbz.yj202588.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nhg.yvedp.cn

[R47] sed 单行替换
来源：http://kar.zhoulong.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://stq.zhaomingkeji.xyz

[R48] awk 取指定列
来源：http://jdz.aibaodan.cn

awk '{print $1, $3}' a.txt
来源：http://emh.feifeiyinyue.top

[R49] awk 带条件
来源：http://zbe.aibaodan.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://egl.0kj1m.cn

[R50] awk 求和
来源：http://oqq.sxryk.cn

awk '{s += $2} END {print s}' a.txt
来源：http://mwh.iojbl.cn

[R51] 排序去重取前几
来源：http://qzb.jinyuanbaomall.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://etu.mhx1999.top

[R52] 统计行数
来源：http://ber.ppjwa.cn

wc -l a.txt
来源：http://ynm.hywenlv.cn

[R53] 查看文件头与实时尾
来源：http://ezq.jiagoushi.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qca.gzhubu.top

[R54] 比较两个文件
来源：http://zcu.guannengcc.top

diff a.txt b.txt
来源：http://mjw.52xcode.cn

[R55] 压缩与解压
来源：http://oyu.316326.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gub.zdbjq.cn

[R56] 远程拷贝
来源：http://hca.zycfv.cn

scp file user@host:/path/
来源：http://fjd.cqqwz.cn

[R57] 远程执行命令
来源：http://xgh.ehwqpu.com

ssh user@host 'uptime'
来源：http://acp.tian-w.cn

[R58] 下载文件
来源：http://exk.zhijiandao.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://isz.guowangkeji.top

[R59] 发 POST JSON
来源：http://ulz.yongpay.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fag.zhoulong.xyz

[R60] 只看 HTTP 状态码
来源：http://edt.uphjek.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jsb.zdbjq.cn

[R61] 磁盘占用
来源：http://rti.tian-w.cn

df -h;  du -sh *
来源：http://str.gzhubu.top

[R62] 找最占空间的文件
来源：http://ozg.yuanzhike.top

du -ah . | sort -rh | head -10
来源：http://ekf.wangdashe.top

[R63] 内存与进程
来源：http://yug.nwbrower.top

free -h;  ps aux | grep nginx
来源：http://ycl.zhaomingkeji.xyz

[R64] 结束进程
来源：http://xbr.fengsongda.top

kill -9 $(pgrep -f app.py)
来源：http://ctd.yj20258.top

[R65] 查看端口占用
来源：http://ufs.hcnkem.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qxv.xuetiantiany.cn

[R66] 定时任务
来源：http://nas.yuanzhike.top

crontab -e;  crontab -l
来源：http://wbj.zdqjudy.top

[R67] 生成随机十六进制串
来源：http://cki.jqgfzy.top

openssl rand -hex 16
来源：http://ath.chenlongwang.top

[R68] 计算文件校验值
来源：http://tod.jinqigufen.top

sha256sum a.txt;  md5sum a.txt
来源：http://ugt.zdqjudy.top

[R69] 生成随机密码
来源：http://wvn.xuanzx.com

head -c 16 /dev/urandom | base64
来源：http://bwt.sweek.top

[R70] 时间戳与互转
来源：http://qke.jinyuanbaomall.cn

date +%s;  date -d @1700000000
来源：http://cea.pycfn.com

[R71] 日期格式化
来源：http://trq.uphjek.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://iwv.hammf.cn

[R72] 等待端口就绪
来源：http://jrh.pengpengdd.cyou

until nc -z localhost 3306; do sleep 1; done
来源：http://tws.xziqi.cn

[R73] 分割大日志
来源：http://uxx.ybcxt.top

split -l 1000 big.log part_
来源：http://qfu.dashuyun.cn

[R74] 批量重命名
来源：http://tyg.jinyuanbaomall.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nmv.gogol.net.cn

[R75] 导出环境变量
来源：http://vdt.sjlbkw.cn

export PATH="$HOME/bin:$PATH"
来源：http://euc.cucudq.cn

[R76] 使用临时文件
来源：http://kfo.yongpay.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kqs.gzhubu.top

[R77] 读取用户输入
来源：http://ojo.sysykeji.top

read -rp "请输入: " ans
来源：http://jlp.vqdsnc.cn

[R78] 交互式菜单
来源：http://vwk.yfazqb.com

select opt in a b c; do echo "$opt"; break; done
来源：http://wwf.gaohongyu789.top

[R79] 解析命令行选项
来源：http://ggw.shanyushiyangtech.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jdv.redwolf501.top

[R80] 查看脚本执行耗时
来源：http://xbd.yangfankeji.com

time ./run.sh
来源：http://egt.zhijiandao.cn

================================================================================
来源：http://jvw.hammf.cn

S. C / C++ 专题
来源：http://lgl.zycfv.cn

================================================================================
来源：http://quz.dashuyun.cn

[S01] C：Hello World
来源：http://lht.kuanghao11.cn

#include <stdio.h>
来源：http://kgf.yj20258.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://deo.nanxinkj.top

[S02] C：变量与格式化输出
来源：http://hhr.feifeiyinyue.top

int a = 10; printf("%d\n", a);
来源：http://prz.bjfxy.top

[S03] C：读入整数
来源：http://iaj.sxryk.cn

int x; scanf("%d", &x);
来源：http://wbv.xinyue.icu

[S04] C：字符串复制
来源：http://exc.wangshuangyany.cn

char dst[32]; strcpy(dst, "hi");
来源：http://szs.fanxiaobao.xyz

[S05] C：字符串长度
来源：http://mck.jiagoushi.top

strlen(s)
来源：http://vjd.fanxiaobao.xyz

[S06] C：字符串比较
来源：http://cjn.shanyushiyangkeji.top

strcmp(a, b) == 0
来源：http://bqz.xuetiantiany.cn

[S07] C：数组遍历求和
来源：http://zns.jlsjyb.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xuc.yuxming.cn

[S08] C：动态内存分配与释放
来源：http://hjt.guowangkeji.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://usu.jyoumei.cn

[S09] C：结构体定义与初始化
来源：http://gxv.quarkkingdee.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ojs.yj20258.top

[S10] C：指针与解引用
来源：http://pwh.fanxiaobao.xyz

int *p = &a;  *p = 5;
来源：http://rxx.gzhubu.top

[S11] C：逐行读文件
来源：http://fti.yuxming.cn

FILE *f = fopen("a.txt", "r");
来源：http://dtu.birdmap.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://sey.fanxiaobao.xyz

fclose(f);
来源：http://qzr.9152youxi.cn

[S12] C：写文件
来源：http://yum.316326.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://smk.ivvv.top

[S13] C：宏定义
来源：http://jka.zhoulong.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ysr.feifeiyinyue.top

[S14] C：枚举
来源：http://ipn.epnwcf.com

enum Color { RED, GREEN, BLUE };
来源：http://plw.yvedp.cn

[S15] C：类型转换
来源：http://yyq.zhaomingkeji.xyz

(double) a / b
来源：http://bla.chenjidiqi.icu

[S16] C：位操作置位
来源：http://eak.jlsjyb.cn

x |= (1 << 3);
来源：http://jeu.shanyushiyangkeji.top

[S17] C：安全拼接字符串
来源：http://qcf.iojbl.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qxc.xinyue.icu

[S18] C：命令行参数
来源：http://kts.quarkkingdee.top

int main(int argc, char **argv)
来源：http://ahr.guannengcc.top

[S19] C：快速排序
来源：http://vro.jqgfzy.top

qsort(a, n, sizeof(int), cmp);
来源：http://zku.meibo888.top

[S20] C：二分查找
来源：http://mlv.xylfe.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mxn.ppjwa.cn

[S21] C：字符类别判断
来源：http://xty.ywan-chungtsiang.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tgf.smart0.xyz

[S22] C：字符串转数字
来源：http://xxh.yonumen.top

atoi("42");  strtod("3.14", NULL);
来源：http://rhz.svipenyu.cn

[S23] C：随机数
来源：http://oap.316326.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://htq.yj20258888.top

[S24] C：获取本地时间
来源：http://pwn.yongpay.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pqz.wangdashe.top

[S25] C：内存拷贝
来源：http://ion.nwbrower.top

memcpy(dst, src, n);
来源：http://qda.bbcook.cn

[S26] C：内存清零
来源：http://dqc.zdbjq.cn

memset(a, 0, sizeof a);
来源：http://tnm.xingfuxueyuan.xyz

[S27] C：定义常量
来源：http://cgz.sweek.top

const double PI = 3.14159;
来源：http://cri.ydzc1.top

[S28] C：静态变量
来源：http://wvb.ctjpmb.com

static int counter = 0;
来源：http://rrj.chenjidiqi.icu

[S29] C：变参函数
来源：http://sdm.xziqi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fea.ybcxt.top

[S30] C：头文件保护
来源：http://qkj.yvedp.cn

#ifndef X_H
来源：http://eks.gogol.net.cn

#define X_H
来源：http://vxy.zhijiandao.cn

#endif
来源：http://uxo.tanke756.top

[S31] C++：Hello World
来源：http://qot.jinyuanbaomall.cn

#include <iostream>
来源：http://mvr.xziqi.cn

int main() { std::cout << "Hello\n"; }
来源：http://kxy.andypj.xyz

[S32] C++：字符串
来源：http://ywh.birdmap.top

std::string s = "hi";  s += "!";
来源：http://uim.ywan-chungtsiang.top

[S33] C++：vector 增删
来源：http://qso.wangdashe.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qbc.52xcode.cn

[S34] C++：遍历 vector
来源：http://hhn.zhoulong.xyz

for (auto &x : v) { std::cout << x; }
来源：http://gfa.yueranfly.top

[S35] C++：map
来源：http://oig.hysaishi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zsk.zhengqikj.top

[S36] C++：unordered_map
来源：http://npl.svipenyu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xhm.jianghu66.top

[S37] C++：set
来源：http://xzc.xylfe.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://oag.andypj.xyz

[S38] C++：排序
来源：http://hmw.tian-w.cn

std::sort(v.begin(), v.end());
来源：http://ipp.zhixingplan.top

[S39] C++：自定义比较器排序
来源：http://ivp.zhiwuduotai.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vwg.sysykeji.top

[S40] C++：查找元素
来源：http://pgv.meibo888.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lmn.shanyushiyangkeji.top

[S41] C++：类与构造函数
来源：http://wwk.vqdsnc.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jig.wangshuangyany.cn

[S42] C++：继承与虚函数
来源：http://uad.nanxinkj.top

class B : public Base { public: void f() override {} };
来源：http://dcy.vqdsnc.cn

[S43] C++：智能指针
来源：http://kmq.ppjwa.cn

auto p = std::make_unique<int>(5);
来源：http://bbu.andypj.xyz

[S44] C++：引用传参
来源：http://gdn.yangfankeji.com

void inc(int &x) { ++x; }
来源：http://vle.zhiwuduotai.top

[S45] C++：lambda
来源：http://tdc.havefunace.top

auto add = [](int a, int b) { return a + b; };
来源：http://hzf.shzxlz.cn

[S46] C++：函数模板
来源：http://unt.haohaochexian.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hii.fanxiaobao.xyz

[S47] C++：结构化绑定遍历
来源：http://nhe.52xcode.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://edh.dianchejie.cn

[S48] C++：逐行读文件
来源：http://jab.chenjidiqi.icu

std::ifstream in("a.txt");  std::string line;
来源：http://mir.wangshuangyany.cn

while (std::getline(in, line)) { }
来源：http://kzl.guowangkeji.top

[S49] C++：写文件
来源：http://glp.zhijiandao.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vsh.sysykeji.top

[S50] C++：格式化数字
来源：http://wgk.ybcxt.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bfy.gzhubu.top

[S51] C++：显式类型转换
来源：http://nld.jlsjyb.cn

static_cast<double>(a) / b
来源：http://zgm.yonumen.top

[S52] C++：const 与 noexcept
来源：http://ueh.xuetiantiany.cn

int size() const noexcept { return n_; }
来源：http://ein.ydjk.org.cn

[S53] C++：移动语义
来源：http://boe.fzhhl.top

std::vector<int> w = std::move(v);
来源：http://qup.c1oappe.top

[S54] C++：异常处理
来源：http://khe.xinyue.icu

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wne.sysykeji.top

[S55] C++：结构化绑定
来源：http://tum.xylfe.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ifl.zycfv.cn

[S56] C++：optional
来源：http://pta.dashuyun.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uiz.jlsjyb.cn

[S57] C++：编译期常量
来源：http://oyu.zhaomingkeji.xyz

constexpr int N = 10;
来源：http://tur.52xcode.cn

[S58] C++：命名空间
来源：http://ymh.zhiwuduotai.top

namespace ns { int f() { return 1; } }
来源：http://mzy.smart0.xyz

[S59] C++：静态断言
来源：http://zhn.hongshengwenyu.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lya.aibaodan.cn

[S60] C++：遍历并删除元素
来源：http://ens.meibo888.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ggk.shangyingyoupin.top

================================================================================
来源：http://adn.tianlin.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gee.0kj1m.cn

================================================================================
来源：http://vjy.cheryme.top

[T01] Kotlin：Hello World
来源：http://fvz.iojbl.cn

println("Hello")
来源：http://van.hesvh.cn

[T02] Kotlin：变量
来源：http://ssy.316326.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jtu.jianghu66.top

[T03] Kotlin：字符串模板
来源：http://eiw.sjlbkw.cn

"值: $b"
来源：http://vdd.yangfankeji.com

[T04] Kotlin：空安全
来源：http://ubc.jiagoushi.top

val n: String? = null;  n?.length
来源：http://itx.sxryk.cn

[T05] Kotlin：when 表达式
来源：http://psb.cashguo.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://juj.tianlin.xyz

[T06] Kotlin：集合映射
来源：http://tme.jinqigfzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ymo.chenzaomai.com

[T07] Kotlin：集合过滤
来源：http://hla.uphjek.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://gfh.havefunace.top

[T08] Kotlin：数据类
来源：http://ofs.aibaodan.cn

data class User(val name: String, val age: Int)
来源：http://rqd.hnxiangtu.top

[T09] Kotlin：扩展函数
来源：http://qur.chenjidiqi.icu

fun String.exclaim() = this + "!"
来源：http://tyb.cucudq.cn

[T10] Kotlin：默认参数
来源：http://ptx.tanke756.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ltt.birdmap.top

[T11] Kotlin：协程
来源：http://jlt.hongshengwenyu.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://dxh.gogol.net.cn

[T12] Kotlin：解构声明
来源：http://bla.fanxiaobao.xyz

val (a, b) = Pair(1, 2)
来源：http://vxk.andypj.xyz

[T13] Kotlin：只读 Map
来源：http://yqu.kuanghao11.cn

val m = mapOf("a" to 1)
来源：http://nry.yvedp.cn

[T14] Kotlin：循环
来源：http://sxu.jinyuanbaomall.cn

for (i in 1..10) println(i)
来源：http://ldf.meibo888.top

[T15] Kotlin：接口
来源：http://ihv.hesvh.cn

interface Shape { fun area(): Double }
来源：http://iio.52xcode.cn

[T16] Swift：Hello World
来源：http://woj.0kj1m.cn

print("Hello")
来源：http://wki.sjlbkw.cn

[T17] Swift：变量与常量
来源：http://rze.ehwqpu.com

var a = 1;  let b = 2
来源：http://vst.bbcook.cn

[T18] Swift：字符串插值
来源：http://iun.jlsjyb.cn

"值: \(b)"
来源：http://iko.hammf.cn

[T19] Swift：可选绑定
来源：http://ncf.yj20258.top

if let n = opt { print(n) }
来源：http://hew.xuanzx.com

[T20] Swift：数组操作
来源：http://tcu.dianchejie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://psz.xylfe.cn

[T21] Swift：遍历
来源：http://bfb.jinghuilouyu.cn

for x in a { print(x) }
来源：http://mcg.epnwcf.com

[T22] Swift：字典
来源：http://ssk.52xcode.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ysm.sjlbkw.cn

[T23] Swift：函数
来源：http://kjc.aibaodan.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nll.ppjwa.cn

[T24] Swift：闭包
来源：http://oga.cdnleiting.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://arc.aibaodan.cn

[T25] Swift：结构体
来源：http://xvr.jlsjyb.cn

struct P { var x: Int }
来源：http://foo.meibo888.top

[T26] Swift：类与重写
来源：http://onm.feifeiyinyue.top

class A: Base { override func f() {} }
来源：http://xgj.shzxlz.cn

[T27] Swift：错误处理
来源：http://jid.fanxiaobao.xyz

do { try f() } catch { print(error) }
来源：http://gjf.shangyingyoupin.top

[T28] Swift：枚举
来源：http://hye.316326.xyz

enum Color { case red, green }
来源：http://pvb.yj202588.top


<!-- 参考信息 -->