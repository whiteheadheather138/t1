代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rfx.ehwqpu.com

[R30] 函数返回状态码
来源：http://aua.ydjk.org.cn

f() { return 0; }; f || echo "失败了"
来源：http://vsf.xuetiantiany.cn

[R31] 局部变量
来源：http://ego.52xcode.cn

f() { local x=1; echo "$x"; }
来源：http://gdv.zhongyouzk.top

[R32] 参数个数校验
来源：http://voc.52xcode.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tzo.bbcook.cn

[R33] 捕获错误并提示行号
来源：http://edo.zycfv.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xzk.jqgfzy.top

[R34] 退出时清理
来源：http://gza.dianchejie.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ckn.jinqigufen.top

[R35] 后台执行并等待
来源：http://mmv.jqgufenzy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://yor.yfazqb.com

[R36] 并发执行多个任务
来源：http://eqo.hysaishi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gxh.jlsjyb.cn

[R37] 把输出赋给变量
来源：http://duj.redwolf501.top

files=$(ls -1)
来源：http://ppt.chenzaomai.com

[R38] 管道串联
来源：http://mzc.dashuyun.cn

cat a.txt | grep -i error | wc -l
来源：http://tjq.snrcjt.cn

[R39] 重定向标准输出与错误
来源：http://isd.fengsongda.top

cmd > out.log 2>&1
来源：http://mro.shanyushiyangkeji.top

[R40] 追加写日志
来源：http://qhf.c1oappe.top

echo "log" >> out.log
来源：http://nlh.ctjpmb.com

[R41] 丢弃输出
来源：http://hzn.pengpengdd.cyou

cmd >/dev/null 2>&1
来源：http://aap.andypj.xyz

[R42] 输入重定向
来源：http://vvu.zhijiandao.cn

wc -l < a.txt
来源：http://mfn.ybcxt.top

[R43] 按名字查找文件
来源：http://jtx.nanxuanxn.top

find . -name "*.log" -type f
来源：http://lhi.zhijiandao.cn

[R44] 按修改时间查找
来源：http://ulj.chenjidiqi.icu

find . -mtime -7 -type f
来源：http://lrg.hnxiangtu.top

[R45] 批量删除
来源：http://jgk.hnqzz.top

find . -name "*.tmp" -delete
来源：http://zjx.kuanghao11.cn

[R46] 递归替换文件内容
来源：http://fgd.yvedp.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bwh.smart0.xyz

[R47] sed 单行替换
来源：http://mle.wangshuangyany.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vsz.shuidangran.top

[R48] awk 取指定列
来源：http://cgn.zdqjudy.top

awk '{print $1, $3}' a.txt
来源：http://kuw.cqqwz.cn

[R49] awk 带条件
来源：http://jmw.fktsv.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://goa.jqgufenzy.top

[R50] awk 求和
来源：http://iml.zhixingplan.top

awk '{s += $2} END {print s}' a.txt
来源：http://rar.xingfuxueyuan.xyz

[R51] 排序去重取前几
来源：http://baw.sufxvd.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://obw.haohaochexian.top

[R52] 统计行数
来源：http://oul.fktsv.cn

wc -l a.txt
来源：http://lvg.hesvh.cn

[R53] 查看文件头与实时尾
来源：http://bgb.tanke756.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ucz.9152youxi.cn

[R54] 比较两个文件
来源：http://njt.ctjpmb.com

diff a.txt b.txt
来源：http://khe.zhoulong.xyz

[R55] 压缩与解压
来源：http://sfz.yvedp.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bvf.jqgufenzy.top

[R56] 远程拷贝
来源：http://ekc.iojbl.cn

scp file user@host:/path/
来源：http://bbz.quarkkingdee.top

[R57] 远程执行命令
来源：http://ulr.ctjpmb.com

ssh user@host 'uptime'
来源：http://icy.jqgfzy.top

[R58] 下载文件
来源：http://ooy.hesvh.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://etf.zdqjudy.top

[R59] 发 POST JSON
来源：http://rmh.hnqzz.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gqz.svipenyu.cn

[R60] 只看 HTTP 状态码
来源：http://nzs.ppjwa.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gam.bjfxy.top

[R61] 磁盘占用
来源：http://gab.52xcode.cn

df -h;  du -sh *
来源：http://uay.vehdjk.com

[R62] 找最占空间的文件
来源：http://wqc.gotoacloud.top

du -ah . | sort -rh | head -10
来源：http://ots.dashuyun.cn

[R63] 内存与进程
来源：http://bet.sxryk.cn

free -h;  ps aux | grep nginx
来源：http://hda.yuxming.cn

[R64] 结束进程
来源：http://sfe.xinyue.icu

kill -9 $(pgrep -f app.py)
来源：http://ykz.daria6918.cn

[R65] 查看端口占用
来源：http://tvq.shzxlz.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xeh.bjfxy.top

[R66] 定时任务
来源：http://aox.hongshengwenyu.top

crontab -e;  crontab -l
来源：http://eid.ivvv.top

[R67] 生成随机十六进制串
来源：http://frd.0kj1m.cn

openssl rand -hex 16
来源：http://evl.c1oappe.top

[R68] 计算文件校验值
来源：http://jkp.yj20258.top

sha256sum a.txt;  md5sum a.txt
来源：http://nzk.yangfankeji.com

[R69] 生成随机密码
来源：http://bab.ppjwa.cn

head -c 16 /dev/urandom | base64
来源：http://ojv.chenzaomai.com

[R70] 时间戳与互转
来源：http://juz.chenzaomai.com

date +%s;  date -d @1700000000
来源：http://czr.sufxvd.cn

[R71] 日期格式化
来源：http://nzx.tianlin.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://ifi.yvedp.cn

[R72] 等待端口就绪
来源：http://iuj.fehbvm.com

until nc -z localhost 3306; do sleep 1; done
来源：http://jed.nanxinkj.top

[R73] 分割大日志
来源：http://cnn.chenjidiqi.icu

split -l 1000 big.log part_
来源：http://wuw.jinqigufen.top

[R74] 批量重命名
来源：http://cfo.zhoulong.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ane.cqqwz.cn

[R75] 导出环境变量
来源：http://xfy.xinyue.icu

export PATH="$HOME/bin:$PATH"
来源：http://zkl.jinqigufen.top

[R76] 使用临时文件
来源：http://zex.zhaomingkeji.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://duy.jqgufenzy.top

[R77] 读取用户输入
来源：http://ykv.xuetiantiany.cn

read -rp "请输入: " ans
来源：http://qhc.yueranfly.top

[R78] 交互式菜单
来源：http://wuf.tian-w.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ioh.mhx1999.top

[R79] 解析命令行选项
来源：http://utd.jinyuanbaomall.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ruc.fanxiaobao.xyz

[R80] 查看脚本执行耗时
来源：http://knn.cashguo.top

time ./run.sh
来源：http://sgh.52xcode.cn

================================================================================
来源：http://zxr.chenjidiqi.icu

S. C / C++ 专题
来源：http://ron.yongpay.top

================================================================================
来源：http://ktt.fanxiaobao.xyz

[S01] C：Hello World
来源：http://fha.wangshuangyany.cn

#include <stdio.h>
来源：http://ohh.0kj1m.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gqz.meibo888.top

[S02] C：变量与格式化输出
来源：http://pyz.zhijiandao.cn

int a = 10; printf("%d\n", a);
来源：http://gko.yuxming.cn

[S03] C：读入整数
来源：http://jkz.sweek.top

int x; scanf("%d", &x);
来源：http://inu.tarul.cn

[S04] C：字符串复制
来源：http://kng.zhiwuduotai.top

char dst[32]; strcpy(dst, "hi");
来源：http://vcw.xingfuxueyuan.xyz

[S05] C：字符串长度
来源：http://udb.fengsongda.top

strlen(s)
来源：http://qek.9152youxi.cn

[S06] C：字符串比较
来源：http://pdv.chenzaomai.com

strcmp(a, b) == 0
来源：http://shj.yuxming.cn

[S07] C：数组遍历求和
来源：http://bwd.jiagoushi.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rwj.hnxiangtu.top

[S08] C：动态内存分配与释放
来源：http://gtl.jinqigfzy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ews.havefunace.top

[S09] C：结构体定义与初始化
来源：http://wvd.mhx1999.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://svs.zhongyouzk.top

[S10] C：指针与解引用
来源：http://erf.tarul.cn

int *p = &a;  *p = 5;
来源：http://uif.epnwcf.com

[S11] C：逐行读文件
来源：http://xgb.jqgufenzy.top

FILE *f = fopen("a.txt", "r");
来源：http://cbf.sxryk.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://unf.gaohongyu789.top

fclose(f);
来源：http://ztq.hongshengwenyu.top

[S12] C：写文件
来源：http://sya.zhongyouzk.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://reg.yfazqb.com

[S13] C：宏定义
来源：http://ayw.yj202588.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://aug.nanxuanxn.top

[S14] C：枚举
来源：http://jkp.quarkkingdee.top

enum Color { RED, GREEN, BLUE };
来源：http://cij.yangfankeji.com

[S15] C：类型转换
来源：http://ubg.ivvv.top

(double) a / b
来源：http://ani.fengsongda.top

[S16] C：位操作置位
来源：http://wod.zhengqikj.top

x |= (1 << 3);
来源：http://ehq.ydjk.org.cn

[S17] C：安全拼接字符串
来源：http://hyt.meibo888.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ylt.ybcxt.top

[S18] C：命令行参数
来源：http://rpb.redwolf501.top

int main(int argc, char **argv)
来源：http://pyr.yj20258.top

[S19] C：快速排序
来源：http://lny.jqgfzy.top

qsort(a, n, sizeof(int), cmp);
来源：http://dfk.cashguo.top

[S20] C：二分查找
来源：http://tly.dashuyun.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wkv.ppjwa.cn

[S21] C：字符类别判断
来源：http://bez.fanxiaobao.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jha.zhaomingkeji.xyz

[S22] C：字符串转数字
来源：http://lft.ydjk.org.cn

atoi("42");  strtod("3.14", NULL);
来源：http://oty.hnqzz.top

[S23] C：随机数
来源：http://ibr.hysaishi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://eox.bbcook.cn

[S24] C：获取本地时间
来源：http://plt.haohaochexian.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jyx.52xcode.cn

[S25] C：内存拷贝
来源：http://seu.zhijiandao.cn

memcpy(dst, src, n);
来源：http://izo.zhijiandao.cn

[S26] C：内存清零
来源：http://aso.tarul.cn

memset(a, 0, sizeof a);
来源：http://vek.ywan-chungtsiang.top

[S27] C：定义常量
来源：http://npu.daxiang520.top

const double PI = 3.14159;
来源：http://yvc.birdmap.top

[S28] C：静态变量
来源：http://ryg.cashguo.top

static int counter = 0;
来源：http://rqm.gotoacloud.top

[S29] C：变参函数
来源：http://dbb.c1oappe.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hrl.bbcook.cn

[S30] C：头文件保护
来源：http://nai.xuetiantiany.cn

#ifndef X_H
来源：http://dli.bbcook.cn

#define X_H
来源：http://jmi.hnqzz.top

#endif
来源：http://rsu.yvedp.cn

[S31] C++：Hello World
来源：http://fwu.chenlongwang.top

#include <iostream>
来源：http://cbm.zdbjq.cn

int main() { std::cout << "Hello\n"; }
来源：http://ehp.gogol.net.cn

[S32] C++：字符串
来源：http://ftc.feifeiyinyue.top

std::string s = "hi";  s += "!";
来源：http://hvw.epnwcf.com

[S33] C++：vector 增删
来源：http://jig.zhiwuduotai.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fye.havefunace.top

[S34] C++：遍历 vector
来源：http://gkg.jinyuanbaomall.cn

for (auto &x : v) { std::cout << x; }
来源：http://wmz.jyoumei.cn

[S35] C++：map
来源：http://jhm.hywenlv.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ddw.meibo888.top

[S36] C++：unordered_map
来源：http://hvy.zdbjq.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mhf.yuxming.cn

[S37] C++：set
来源：http://ayc.jqgufenzy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ksc.zhaomingkeji.xyz

[S38] C++：排序
来源：http://ucm.fehbvm.com

std::sort(v.begin(), v.end());
来源：http://nmw.yj20258.top

[S39] C++：自定义比较器排序
来源：http://ebu.nanxuanxn.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xgd.guowangkeji.top

[S40] C++：查找元素
来源：http://mmp.hongshengwenyu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ixy.jqgufenzy.top

[S41] C++：类与构造函数
来源：http://wgt.nwbrower.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jvh.guowangkeji.top

[S42] C++：继承与虚函数
来源：http://wrz.haohaochexian.top

class B : public Base { public: void f() override {} };
来源：http://syh.zhijiandao.cn

[S43] C++：智能指针
来源：http://smd.nanxuanxn.top

auto p = std::make_unique<int>(5);
来源：http://wqc.hcnkem.com

[S44] C++：引用传参
来源：http://keg.zhengqikj.top

void inc(int &x) { ++x; }
来源：http://njb.daxiang520.top

[S45] C++：lambda
来源：http://fup.guannengcc.top

auto add = [](int a, int b) { return a + b; };
来源：http://qul.9152youxi.cn

[S46] C++：函数模板
来源：http://vdy.jinqigufen.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zfm.tianlin.xyz

[S47] C++：结构化绑定遍历
来源：http://mtn.jianghu66.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tyx.mhx1999.top

[S48] C++：逐行读文件
来源：http://djc.daxiang520.top

std::ifstream in("a.txt");  std::string line;
来源：http://mpe.fzhhl.top

while (std::getline(in, line)) { }
来源：http://rfi.shanyushiyangtech.top

[S49] C++：写文件
来源：http://rtm.hammf.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fzd.haohaochexian.top

[S50] C++：格式化数字
来源：http://iyq.dianchejie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mpy.xylfe.cn

[S51] C++：显式类型转换
来源：http://rai.zycfv.cn

static_cast<double>(a) / b
来源：http://akf.pengpengdd.cyou

[S52] C++：const 与 noexcept
来源：http://qqc.52xcode.cn

int size() const noexcept { return n_; }
来源：http://sfo.nanxinkj.top

[S53] C++：移动语义
来源：http://pib.redwolf501.top

std::vector<int> w = std::move(v);
来源：http://ntt.hammf.cn

[S54] C++：异常处理
来源：http://pxc.nanxinkj.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uuv.ivvv.top

[S55] C++：结构化绑定
来源：http://bqq.sxryk.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://kdj.xingfuxueyuan.xyz

[S56] C++：optional
来源：http://art.ywan-chungtsiang.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nvq.yfazqb.com

[S57] C++：编译期常量
来源：http://goj.aizwys.cn

constexpr int N = 10;
来源：http://ier.ivvv.top

[S58] C++：命名空间
来源：http://yds.tanke756.top

namespace ns { int f() { return 1; } }
来源：http://cbz.uphjek.com

[S59] C++：静态断言
来源：http://opr.cucudq.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://peh.bjfxy.top

[S60] C++：遍历并删除元素
来源：http://cgj.yanxiufei.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gud.svipenyu.cn

================================================================================
来源：http://dhs.uphjek.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zub.yonumen.top

================================================================================
来源：http://rrn.yanxiufei.cn

[T01] Kotlin：Hello World
来源：http://jii.tianlin.xyz

println("Hello")
来源：http://rgs.epnwcf.com

[T02] Kotlin：变量
来源：http://psk.vehdjk.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fmq.birdmap.top

[T03] Kotlin：字符串模板
来源：http://uoz.cheryme.top

"值: $b"
来源：http://dcs.hnxiangtu.top

[T04] Kotlin：空安全
来源：http://aji.cashguo.top

val n: String? = null;  n?.length
来源：http://kji.iojbl.cn

[T05] Kotlin：when 表达式
来源：http://iie.yueranfly.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mys.ehwqpu.com

[T06] Kotlin：集合映射
来源：http://dov.hammf.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://sas.ppjwa.cn

[T07] Kotlin：集合过滤
来源：http://kdl.cqqwz.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://aci.dianchejie.cn

[T08] Kotlin：数据类
来源：http://vii.sxryk.cn

data class User(val name: String, val age: Int)
来源：http://msi.hesvh.cn

[T09] Kotlin：扩展函数
来源：http://vny.svipenyu.cn

fun String.exclaim() = this + "!"
来源：http://bhf.tianlin.xyz

[T10] Kotlin：默认参数
来源：http://wyx.chenjidiqi.icu

fun greet(name: String = "World") = "Hi $name"
来源：http://doj.ybcxt.top

[T11] Kotlin：协程
来源：http://zza.dashuyun.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bvr.iojbl.cn

[T12] Kotlin：解构声明
来源：http://ker.sysykeji.top

val (a, b) = Pair(1, 2)
来源：http://vtk.tanke756.top

[T13] Kotlin：只读 Map
来源：http://dtd.zhengqikj.top

val m = mapOf("a" to 1)
来源：http://tar.jlsjyb.cn

[T14] Kotlin：循环
来源：http://jzg.yuxming.cn

for (i in 1..10) println(i)
来源：http://mcz.nanxinkj.top

[T15] Kotlin：接口
来源：http://khe.zhixingplan.top

interface Shape { fun area(): Double }
来源：http://xbe.yueranfly.top

[T16] Swift：Hello World
来源：http://gpg.c1oappe.top

print("Hello")
来源：http://lbf.epnwcf.com

[T17] Swift：变量与常量
来源：http://hlf.nanxinkj.top

var a = 1;  let b = 2
来源：http://yal.nanxuanxn.top

[T18] Swift：字符串插值
来源：http://aer.nwbrower.top

"值: \(b)"
来源：http://mjz.vehdjk.com

[T19] Swift：可选绑定
来源：http://mrk.yfazqb.com

if let n = opt { print(n) }
来源：http://wxd.ydzc1.top

[T20] Swift：数组操作
来源：http://fue.fanxiaobao.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://zuj.yanxiufei.cn

[T21] Swift：遍历
来源：http://ysh.nanxinkj.top

for x in a { print(x) }
来源：http://ghy.yonumen.top

[T22] Swift：字典
来源：http://hab.fengsongda.top

var d = ["a": 1];  d["b"] = 2
来源：http://hao.hongshengwenyu.top

[T23] Swift：函数
来源：http://pnj.gaohongyu789.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yez.0kj1m.cn

[T24] Swift：闭包
来源：http://wxb.jinghuilouyu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://iwf.52xcode.cn

[T25] Swift：结构体
来源：http://khe.feifeiyinyue.top

struct P { var x: Int }
来源：http://vhm.fehbvm.com

[T26] Swift：类与重写
来源：http://igc.jianghu66.top

class A: Base { override func f() {} }
来源：http://uzq.jyoumei.cn

[T27] Swift：错误处理
来源：http://xla.chenjidiqi.icu

do { try f() } catch { print(error) }
来源：http://xlb.shuidangran.top

[T28] Swift：枚举
来源：http://pis.gzhubu.top

enum Color { case red, green }
来源：http://yss.ctjpmb.com

[T29] Swift：guard 提前返回
来源：http://rng.hongshengwenyu.top

guard let x = opt else { return }
来源：http://jap.jinyuanbaomall.cn

[T30] Swift：协议
来源：http://mrr.yj20258.top

protocol Shape { func area() -> Double }
来源：http://xvd.sxryk.cn

[T31] Lua：Hello World
来源：http://cge.gotoacloud.top

print("Hello")
来源：http://euy.gzhubu.top

[T32] Lua：局部变量
来源：http://ypb.cdnleiting.top

local a = 1
来源：http://uue.havefunace.top


<!-- 参考信息 -->