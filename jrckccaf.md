代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://vkp.andypj.xyz

[R26] 命令替换
来源：http://wiq.tarul.cn

now=$(date +%F); echo "$now"
来源：http://fpq.chenzaomai.com

[R27] 算术展开
来源：http://axz.yuanzhike.top

echo $((1 + 2 * 3))
来源：http://lcj.tanke756.top

[R28] 浮点运算
来源：http://qfp.jinghuilouyu.cn

echo "scale=2; 10/3" | bc
来源：http://rja.jlsjyb.cn

[R29] 定义函数
来源：http://day.ydzc1.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ixf.epnwcf.com

[R30] 函数返回状态码
来源：http://enr.svipenyu.cn

f() { return 0; }; f || echo "失败了"
来源：http://poj.kuanghao11.cn

[R31] 局部变量
来源：http://llb.yuanzhike.top

f() { local x=1; echo "$x"; }
来源：http://mbz.gotoacloud.top

[R32] 参数个数校验
来源：http://zzi.cheryme.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://snm.tian-w.cn

[R33] 捕获错误并提示行号
来源：http://qli.9152youxi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://htj.zhijiandao.cn

[R34] 退出时清理
来源：http://zvh.uphjek.com

trap 'rm -f "$tmp"' EXIT
来源：http://nur.zdqjudy.top

[R35] 后台执行并等待
来源：http://ttk.gaohongyu789.top

sleep 5 & pid=$!; wait "$pid"
来源：http://bvs.redwolf501.top

[R36] 并发执行多个任务
来源：http://tjy.yangfankeji.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://unr.yanxiufei.cn

[R37] 把输出赋给变量
来源：http://gks.gaohongyu789.top

files=$(ls -1)
来源：http://mta.wangdashe.top

[R38] 管道串联
来源：http://rll.zhiwuduotai.top

cat a.txt | grep -i error | wc -l
来源：http://csr.vehdjk.com

[R39] 重定向标准输出与错误
来源：http://uhb.yonumen.top

cmd > out.log 2>&1
来源：http://uqu.ydjk.org.cn

[R40] 追加写日志
来源：http://zlo.pengpengdd.cyou

echo "log" >> out.log
来源：http://xjd.hammf.cn

[R41] 丢弃输出
来源：http://nnw.jianghu66.top

cmd >/dev/null 2>&1
来源：http://gsl.sxryk.cn

[R42] 输入重定向
来源：http://oiv.yvedp.cn

wc -l < a.txt
来源：http://ljw.shzxlz.cn

[R43] 按名字查找文件
来源：http://duq.cashguo.top

find . -name "*.log" -type f
来源：http://caf.jinyuanbaomall.cn

[R44] 按修改时间查找
来源：http://jds.epnwcf.com

find . -mtime -7 -type f
来源：http://zri.svipenyu.cn

[R45] 批量删除
来源：http://ygl.yj20258888.top

find . -name "*.tmp" -delete
来源：http://gku.uphjek.com

[R46] 递归替换文件内容
来源：http://sfy.yanxiufei.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yir.nwbrower.top

[R47] sed 单行替换
来源：http://fsy.yvedp.cn

sed -i 's/foo/bar/g' a.txt
来源：http://nvk.hnxiangtu.top

[R48] awk 取指定列
来源：http://woi.ctjpmb.com

awk '{print $1, $3}' a.txt
来源：http://cab.xingfuxueyuan.xyz

[R49] awk 带条件
来源：http://iqd.ppjwa.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kzw.hysaishi.cn

[R50] awk 求和
来源：http://dgu.dashuyun.cn

awk '{s += $2} END {print s}' a.txt
来源：http://rej.bjfxy.top

[R51] 排序去重取前几
来源：http://iek.wangdashe.top

sort a.txt | uniq -c | sort -rn | head
来源：http://mkl.shuidangran.top

[R52] 统计行数
来源：http://lgv.yueranfly.top

wc -l a.txt
来源：http://iva.sjlbkw.cn

[R53] 查看文件头与实时尾
来源：http://rsn.hfpthk.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://eqa.yj202588.top

[R54] 比较两个文件
来源：http://slq.quarkkingdee.top

diff a.txt b.txt
来源：http://zzc.ivvv.top

[R55] 压缩与解压
来源：http://srn.hongshengwenyu.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mnx.zhijiandao.cn

[R56] 远程拷贝
来源：http://ghx.cucudq.cn

scp file user@host:/path/
来源：http://ohs.yongpay.top

[R57] 远程执行命令
来源：http://obm.gzhubu.top

ssh user@host 'uptime'
来源：http://qdd.wangshuangyany.cn

[R58] 下载文件
来源：http://grq.pycfn.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vdi.guannengcc.top

[R59] 发 POST JSON
来源：http://npz.sweek.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ohk.gaohongyu789.top

[R60] 只看 HTTP 状态码
来源：http://gpd.yj20258888.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qaj.yj20258.top

[R61] 磁盘占用
来源：http://ltm.yueranfly.top

df -h;  du -sh *
来源：http://djj.shzxlz.cn

[R62] 找最占空间的文件
来源：http://vcs.ctjpmb.com

du -ah . | sort -rh | head -10
来源：http://wdk.hnqzz.top

[R63] 内存与进程
来源：http://cmt.yangfankeji.com

free -h;  ps aux | grep nginx
来源：http://njz.chenlongwang.top

[R64] 结束进程
来源：http://lth.52xcode.cn

kill -9 $(pgrep -f app.py)
来源：http://net.dianchejie.cn

[R65] 查看端口占用
来源：http://exy.jinghuilouyu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://oza.ydjk.org.cn

[R66] 定时任务
来源：http://hew.hywenlv.cn

crontab -e;  crontab -l
来源：http://wmf.jianghu66.top

[R67] 生成随机十六进制串
来源：http://xem.zhiwuduotai.top

openssl rand -hex 16
来源：http://zwn.sysykeji.top

[R68] 计算文件校验值
来源：http://lsz.jianghu66.top

sha256sum a.txt;  md5sum a.txt
来源：http://mxu.yfazqb.com

[R69] 生成随机密码
来源：http://kvf.fehbvm.com

head -c 16 /dev/urandom | base64
来源：http://boe.shuidangran.top

[R70] 时间戳与互转
来源：http://gcl.ppjwa.cn

date +%s;  date -d @1700000000
来源：http://afm.cdnleiting.top

[R71] 日期格式化
来源：http://snd.jianghu66.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://qrh.tanke756.top

[R72] 等待端口就绪
来源：http://zzm.sufxvd.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://pth.sysykeji.top

[R73] 分割大日志
来源：http://vha.sysykeji.top

split -l 1000 big.log part_
来源：http://fta.yangfankeji.com

[R74] 批量重命名
来源：http://ygo.svipenyu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dfr.yj20258.top

[R75] 导出环境变量
来源：http://ahe.52xcode.cn

export PATH="$HOME/bin:$PATH"
来源：http://fka.andypj.xyz

[R76] 使用临时文件
来源：http://nat.yj20258.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hoi.uphjek.com

[R77] 读取用户输入
来源：http://bsm.jinqigufen.top

read -rp "请输入: " ans
来源：http://xgb.pycfn.com

[R78] 交互式菜单
来源：http://wmp.hysaishi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://swa.zhoulong.xyz

[R79] 解析命令行选项
来源：http://bvw.zhijiandao.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xib.zhoulong.xyz

[R80] 查看脚本执行耗时
来源：http://aja.hesvh.cn

time ./run.sh
来源：http://tqu.xziqi.cn

================================================================================
来源：http://gqh.sjlbkw.cn

S. C / C++ 专题
来源：http://ktk.xuanzx.com

================================================================================
来源：http://svn.shzxlz.cn

[S01] C：Hello World
来源：http://gfr.jqgufenzy.top

#include <stdio.h>
来源：http://iwy.xingfuxueyuan.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://gih.shzxlz.cn

[S02] C：变量与格式化输出
来源：http://vdt.zhijiandao.cn

int a = 10; printf("%d\n", a);
来源：http://kyw.smart0.xyz

[S03] C：读入整数
来源：http://yca.hnxiangtu.top

int x; scanf("%d", &x);
来源：http://llt.svipenyu.cn

[S04] C：字符串复制
来源：http://gdp.ydzc1.top

char dst[32]; strcpy(dst, "hi");
来源：http://lon.yuxming.cn

[S05] C：字符串长度
来源：http://fhw.xinyue.icu

strlen(s)
来源：http://gpg.zycfv.cn

[S06] C：字符串比较
来源：http://dgr.nwbrower.top

strcmp(a, b) == 0
来源：http://dxq.xuanzx.com

[S07] C：数组遍历求和
来源：http://vcg.shanyushiyangkeji.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cbu.jinyuanbaomall.cn

[S08] C：动态内存分配与释放
来源：http://lsv.sjlbkw.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pfb.jinghuilouyu.cn

[S09] C：结构体定义与初始化
来源：http://gfz.vehdjk.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yrm.smart0.xyz

[S10] C：指针与解引用
来源：http://pmv.haohaochexian.top

int *p = &a;  *p = 5;
来源：http://yfq.fengsongda.top

[S11] C：逐行读文件
来源：http://epv.xziqi.cn

FILE *f = fopen("a.txt", "r");
来源：http://kcp.gzhubu.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://vwh.ywan-chungtsiang.top

fclose(f);
来源：http://jpk.52xcode.cn

[S12] C：写文件
来源：http://htw.yfazqb.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mfo.c1oappe.top

[S13] C：宏定义
来源：http://tdy.yuanzhike.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dxq.uphjek.com

[S14] C：枚举
来源：http://nfz.xuanzx.com

enum Color { RED, GREEN, BLUE };
来源：http://tdw.tian-w.cn

[S15] C：类型转换
来源：http://fem.shanyushiyangtech.top

(double) a / b
来源：http://cll.gzhubu.top

[S16] C：位操作置位
来源：http://tjf.meibo888.top

x |= (1 << 3);
来源：http://jzl.zhijiandao.cn

[S17] C：安全拼接字符串
来源：http://ydn.epnwcf.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gbt.fzhhl.top

[S18] C：命令行参数
来源：http://iuf.havefunace.top

int main(int argc, char **argv)
来源：http://qkw.wangdashe.top

[S19] C：快速排序
来源：http://uwq.yvedp.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qhu.tarul.cn

[S20] C：二分查找
来源：http://pxk.sufxvd.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nmm.hnxiangtu.top

[S21] C：字符类别判断
来源：http://lwp.vqdsnc.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gav.xinyue.icu

[S22] C：字符串转数字
来源：http://gwj.ydzc1.top

atoi("42");  strtod("3.14", NULL);
来源：http://meh.sweek.top

[S23] C：随机数
来源：http://whb.nanxinkj.top

srand(time(NULL));  int r = rand() % 100;
来源：http://bod.tarul.cn

[S24] C：获取本地时间
来源：http://gsk.aibaodan.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pic.sufxvd.cn

[S25] C：内存拷贝
来源：http://bqr.shanyushiyangkeji.top

memcpy(dst, src, n);
来源：http://via.shanyushiyangtech.top

[S26] C：内存清零
来源：http://rnr.yanxiufei.cn

memset(a, 0, sizeof a);
来源：http://atv.zhengqikj.top

[S27] C：定义常量
来源：http://bxs.ywan-chungtsiang.top

const double PI = 3.14159;
来源：http://csf.yj20258.top

[S28] C：静态变量
来源：http://fuz.wangdashe.top

static int counter = 0;
来源：http://vjr.chenzaomai.com

[S29] C：变参函数
来源：http://fkp.tanke756.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://psc.kuanghao11.cn

[S30] C：头文件保护
来源：http://jzc.zdbjq.cn

#ifndef X_H
来源：http://hpr.jinghuilouyu.cn

#define X_H
来源：http://ipa.jlsjyb.cn

#endif
来源：http://icr.meibo888.top

[S31] C++：Hello World
来源：http://ruy.zhoulong.xyz

#include <iostream>
来源：http://uir.xuanzx.com

int main() { std::cout << "Hello\n"; }
来源：http://uoo.dianchejie.cn

[S32] C++：字符串
来源：http://ahc.52xcode.cn

std::string s = "hi";  s += "!";
来源：http://mbn.yangfankeji.com

[S33] C++：vector 增删
来源：http://vxh.shangyingyoupin.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xkk.zhixingplan.top

[S34] C++：遍历 vector
来源：http://myh.havefunace.top

for (auto &x : v) { std::cout << x; }
来源：http://xti.daxiang520.top

[S35] C++：map
来源：http://bcy.yanxiufei.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hjc.tianlin.xyz

[S36] C++：unordered_map
来源：http://xbk.svipenyu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vny.sysykeji.top

[S37] C++：set
来源：http://ycz.hesvh.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://eti.zhijiandao.cn

[S38] C++：排序
来源：http://buv.cqqwz.cn

std::sort(v.begin(), v.end());
来源：http://hsn.hnqzz.top

[S39] C++：自定义比较器排序
来源：http://onv.redwolf501.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ros.xylfe.cn

[S40] C++：查找元素
来源：http://krm.shangyingyoupin.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ihy.hnqzz.top

[S41] C++：类与构造函数
来源：http://aab.xylfe.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gti.ctjpmb.com

[S42] C++：继承与虚函数
来源：http://fed.jinghuilouyu.cn

class B : public Base { public: void f() override {} };
来源：http://dbc.yangfankeji.com

[S43] C++：智能指针
来源：http://bft.wangshuangyany.cn

auto p = std::make_unique<int>(5);
来源：http://umf.zhaomingkeji.xyz

[S44] C++：引用传参
来源：http://bcf.fanxiaobao.xyz

void inc(int &x) { ++x; }
来源：http://bhr.yuxming.cn

[S45] C++：lambda
来源：http://gnn.vehdjk.com

auto add = [](int a, int b) { return a + b; };
来源：http://koc.shanyushiyangkeji.top

[S46] C++：函数模板
来源：http://dqw.yueranfly.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ocv.cqqwz.cn

[S47] C++：结构化绑定遍历
来源：http://xdl.aizwys.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ups.xingfuxueyuan.xyz

[S48] C++：逐行读文件
来源：http://nbb.pengpengdd.cyou

std::ifstream in("a.txt");  std::string line;
来源：http://nvn.9152youxi.cn

while (std::getline(in, line)) { }
来源：http://eqr.cashguo.top

[S49] C++：写文件
来源：http://wfu.tian-w.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hlu.xinyue.icu

[S50] C++：格式化数字
来源：http://eay.cheryme.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sjx.uphjek.com

[S51] C++：显式类型转换
来源：http://tvs.wangdashe.top

static_cast<double>(a) / b
来源：http://sii.dashuyun.cn

[S52] C++：const 与 noexcept
来源：http://dbf.aibaodan.cn

int size() const noexcept { return n_; }
来源：http://ydh.ppjwa.cn

[S53] C++：移动语义
来源：http://qlk.zdqjudy.top

std::vector<int> w = std::move(v);
来源：http://xlq.xylfe.cn

[S54] C++：异常处理
来源：http://ovd.iojbl.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nic.vehdjk.com

[S55] C++：结构化绑定
来源：http://lpg.jinqigfzy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://nrn.cucudq.cn

[S56] C++：optional
来源：http://gyv.52xcode.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lrr.cdnleiting.top

[S57] C++：编译期常量
来源：http://keh.zhoulong.xyz

constexpr int N = 10;
来源：http://gjt.tian-w.cn

[S58] C++：命名空间
来源：http://pdz.gogol.net.cn

namespace ns { int f() { return 1; } }
来源：http://aus.zhoulong.xyz

[S59] C++：静态断言
来源：http://qpx.quarkkingdee.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://skm.pengpengdd.cyou

[S60] C++：遍历并删除元素
来源：http://pse.chenjidiqi.icu

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bkw.nanxuanxn.top

================================================================================
来源：http://isk.dianchejie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xvx.sweek.top

================================================================================
来源：http://pyt.vehdjk.com

[T01] Kotlin：Hello World
来源：http://oeo.zdbjq.cn

println("Hello")
来源：http://egt.jinghuilouyu.cn

[T02] Kotlin：变量
来源：http://mjb.316326.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jcd.yongpay.top

[T03] Kotlin：字符串模板
来源：http://lup.jinqigfzy.top

"值: $b"
来源：http://big.yanxiufei.cn

[T04] Kotlin：空安全
来源：http://wgw.hnxiangtu.top

val n: String? = null;  n?.length
来源：http://pej.tarul.cn

[T05] Kotlin：when 表达式
来源：http://qyt.ydjk.org.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vaf.wangdashe.top

[T06] Kotlin：集合映射
来源：http://qff.jqgufenzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://jtv.chenjidiqi.icu

[T07] Kotlin：集合过滤
来源：http://gon.9152youxi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://lhs.ctjpmb.com

[T08] Kotlin：数据类
来源：http://kwq.tanke756.top

data class User(val name: String, val age: Int)
来源：http://hui.ydzc1.top

[T09] Kotlin：扩展函数
来源：http://rho.gogol.net.cn

fun String.exclaim() = this + "!"
来源：http://mta.fzhhl.top

[T10] Kotlin：默认参数
来源：http://fyt.yj202588.top

fun greet(name: String = "World") = "Hi $name"
来源：http://hox.pengpengdd.cyou

[T11] Kotlin：协程
来源：http://mna.ivvv.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://bpe.sjlbkw.cn

[T12] Kotlin：解构声明
来源：http://hnv.ywan-chungtsiang.top

val (a, b) = Pair(1, 2)
来源：http://npt.xinyue.icu

[T13] Kotlin：只读 Map
来源：http://jls.quarkkingdee.top

val m = mapOf("a" to 1)
来源：http://fyy.dianchejie.cn

[T14] Kotlin：循环
来源：http://bsy.haohaochexian.top

for (i in 1..10) println(i)
来源：http://goh.yj20258.top

[T15] Kotlin：接口
来源：http://ads.fengsongda.top

interface Shape { fun area(): Double }
来源：http://fpc.meibo888.top

[T16] Swift：Hello World
来源：http://kxs.yvedp.cn

print("Hello")
来源：http://znq.cheryme.top

[T17] Swift：变量与常量
来源：http://osz.ctjpmb.com

var a = 1;  let b = 2
来源：http://otq.xylfe.cn

[T18] Swift：字符串插值
来源：http://xak.fanxiaobao.xyz

"值: \(b)"
来源：http://npk.jinqigufen.top

[T19] Swift：可选绑定
来源：http://kwv.fanxiaobao.xyz

if let n = opt { print(n) }
来源：http://kdt.jqgufenzy.top

[T20] Swift：数组操作
来源：http://jlu.tanke756.top

var a = [1, 2, 3];  a.append(4)
来源：http://mxk.jyoumei.cn

[T21] Swift：遍历
来源：http://mdo.xziqi.cn

for x in a { print(x) }
来源：http://bge.xylfe.cn

[T22] Swift：字典
来源：http://pim.bjfxy.top

var d = ["a": 1];  d["b"] = 2
来源：http://vdq.fktsv.cn

[T23] Swift：函数
来源：http://owq.sjlbkw.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jzp.ybcxt.top

[T24] Swift：闭包
来源：http://bnw.iojbl.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ylv.fzhhl.top

[T25] Swift：结构体
来源：http://gla.iojbl.cn

struct P { var x: Int }
来源：http://hhw.aizwys.cn

[T26] Swift：类与重写
来源：http://cvz.shzxlz.cn

class A: Base { override func f() {} }
来源：http://uwn.yj202588.top

[T27] Swift：错误处理
来源：http://gjy.jqgufenzy.top

do { try f() } catch { print(error) }
来源：http://rhh.cheryme.top

[T28] Swift：枚举
来源：http://ouu.jinqigufen.top

enum Color { case red, green }
来源：http://tqu.zhongyouzk.top


<!-- 参考信息 -->