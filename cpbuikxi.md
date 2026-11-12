代发 wailian999

echo $((1 + 2 * 3))
来源：http://xhz.iojbl.cn

[R28] 浮点运算
来源：http://ujy.tanke756.top

echo "scale=2; 10/3" | bc
来源：http://qmp.sufxvd.cn

[R29] 定义函数
来源：http://nij.yonumen.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://oqo.zhixingplan.top

[R30] 函数返回状态码
来源：http://xbv.yonumen.top

f() { return 0; }; f || echo "失败了"
来源：http://ylq.wangshuangyany.cn

[R31] 局部变量
来源：http://gas.shangyingyoupin.top

f() { local x=1; echo "$x"; }
来源：http://sqg.birdmap.top

[R32] 参数个数校验
来源：http://rzj.zhijiandao.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ubm.pycfn.com

[R33] 捕获错误并提示行号
来源：http://gjw.ivvv.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dop.hesvh.cn

[R34] 退出时清理
来源：http://njd.meibo888.top

trap 'rm -f "$tmp"' EXIT
来源：http://esm.hfpthk.cn

[R35] 后台执行并等待
来源：http://hsw.cashguo.top

sleep 5 & pid=$!; wait "$pid"
来源：http://vum.yj20258.top

[R36] 并发执行多个任务
来源：http://rmi.ppjwa.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ndg.sufxvd.cn

[R37] 把输出赋给变量
来源：http://jzh.nanxuanxn.top

files=$(ls -1)
来源：http://fyw.zhaomingkeji.xyz

[R38] 管道串联
来源：http://wjp.cucudq.cn

cat a.txt | grep -i error | wc -l
来源：http://pfs.hfpthk.cn

[R39] 重定向标准输出与错误
来源：http://xfq.guowangkeji.top

cmd > out.log 2>&1
来源：http://zak.c1oappe.top

[R40] 追加写日志
来源：http://snj.hesvh.cn

echo "log" >> out.log
来源：http://xrm.shanyushiyangkeji.top

[R41] 丢弃输出
来源：http://rno.tian-w.cn

cmd >/dev/null 2>&1
来源：http://ijq.fanxiaobao.xyz

[R42] 输入重定向
来源：http://nhk.yvedp.cn

wc -l < a.txt
来源：http://qnm.vqdsnc.cn

[R43] 按名字查找文件
来源：http://end.sysykeji.top

find . -name "*.log" -type f
来源：http://rbr.xziqi.cn

[R44] 按修改时间查找
来源：http://kzr.wangdashe.top

find . -mtime -7 -type f
来源：http://vah.yj20258.top

[R45] 批量删除
来源：http://vas.xinyue.icu

find . -name "*.tmp" -delete
来源：http://abh.yonumen.top

[R46] 递归替换文件内容
来源：http://ubd.cucudq.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ejy.birdmap.top

[R47] sed 单行替换
来源：http://jyy.yj20258.top

sed -i 's/foo/bar/g' a.txt
来源：http://jlc.meibo888.top

[R48] awk 取指定列
来源：http://tqs.wangshuangyany.cn

awk '{print $1, $3}' a.txt
来源：http://eej.ywan-chungtsiang.top

[R49] awk 带条件
来源：http://xdx.fktsv.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yqu.fehbvm.com

[R50] awk 求和
来源：http://mdm.jinyuanbaomall.cn

awk '{s += $2} END {print s}' a.txt
来源：http://jdw.yuxming.cn

[R51] 排序去重取前几
来源：http://uxj.ivvv.top

sort a.txt | uniq -c | sort -rn | head
来源：http://kfy.nwbrower.top

[R52] 统计行数
来源：http://cpr.shanyushiyangtech.top

wc -l a.txt
来源：http://eok.aizwys.cn

[R53] 查看文件头与实时尾
来源：http://nzm.shzxlz.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tfe.yangfankeji.com

[R54] 比较两个文件
来源：http://uxs.xziqi.cn

diff a.txt b.txt
来源：http://aeb.havefunace.top

[R55] 压缩与解压
来源：http://kso.nanxuanxn.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pdf.gogol.net.cn

[R56] 远程拷贝
来源：http://fqv.svipenyu.cn

scp file user@host:/path/
来源：http://bmx.tanke756.top

[R57] 远程执行命令
来源：http://uvd.ywan-chungtsiang.top

ssh user@host 'uptime'
来源：http://mal.jqgfzy.top

[R58] 下载文件
来源：http://emv.yfazqb.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qzr.zycfv.cn

[R59] 发 POST JSON
来源：http://byp.c1oappe.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ssg.zdqjudy.top

[R60] 只看 HTTP 状态码
来源：http://ysz.vehdjk.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cte.yj20258.top

[R61] 磁盘占用
来源：http://xer.52xcode.cn

df -h;  du -sh *
来源：http://ssb.dashuyun.cn

[R62] 找最占空间的文件
来源：http://gqo.hcnkem.com

du -ah . | sort -rh | head -10
来源：http://zub.shanyushiyangtech.top

[R63] 内存与进程
来源：http://phe.chenlongwang.top

free -h;  ps aux | grep nginx
来源：http://ufo.zhengqikj.top

[R64] 结束进程
来源：http://vka.shanyushiyangtech.top

kill -9 $(pgrep -f app.py)
来源：http://bmn.chenzaomai.com

[R65] 查看端口占用
来源：http://ukt.hnqzz.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xtd.yongpay.top

[R66] 定时任务
来源：http://ata.fehbvm.com

crontab -e;  crontab -l
来源：http://hdo.uphjek.com

[R67] 生成随机十六进制串
来源：http://nxv.cdnleiting.top

openssl rand -hex 16
来源：http://bgn.haohaochexian.top

[R68] 计算文件校验值
来源：http://mau.bjfxy.top

sha256sum a.txt;  md5sum a.txt
来源：http://ihd.hesvh.cn

[R69] 生成随机密码
来源：http://vdk.zycfv.cn

head -c 16 /dev/urandom | base64
来源：http://svi.xuetiantiany.cn

[R70] 时间戳与互转
来源：http://hhf.zhixingplan.top

date +%s;  date -d @1700000000
来源：http://lwm.jinqigufen.top

[R71] 日期格式化
来源：http://bmt.wangdashe.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://qpi.guannengcc.top

[R72] 等待端口就绪
来源：http://vng.hysaishi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://nfd.ydjk.org.cn

[R73] 分割大日志
来源：http://oqx.52xcode.cn

split -l 1000 big.log part_
来源：http://cdw.zhengqikj.top

[R74] 批量重命名
来源：http://jts.kuanghao11.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://laj.52xcode.cn

[R75] 导出环境变量
来源：http://jsb.sufxvd.cn

export PATH="$HOME/bin:$PATH"
来源：http://jpj.feifeiyinyue.top

[R76] 使用临时文件
来源：http://bjo.jiagoushi.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://whl.nwbrower.top

[R77] 读取用户输入
来源：http://dzy.yvedp.cn

read -rp "请输入: " ans
来源：http://tjv.gzhubu.top

[R78] 交互式菜单
来源：http://itw.fzhhl.top

select opt in a b c; do echo "$opt"; break; done
来源：http://lya.meibo888.top

[R79] 解析命令行选项
来源：http://cmz.sweek.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tja.jqgufenzy.top

[R80] 查看脚本执行耗时
来源：http://voj.yuxming.cn

time ./run.sh
来源：http://dfe.yonumen.top

================================================================================
来源：http://ksn.zycfv.cn

S. C / C++ 专题
来源：http://gif.chenjidiqi.icu

================================================================================
来源：http://pfb.hysaishi.cn

[S01] C：Hello World
来源：http://ivt.zdbjq.cn

#include <stdio.h>
来源：http://ppx.xziqi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://zoz.yangfankeji.com

[S02] C：变量与格式化输出
来源：http://vqi.daxiang520.top

int a = 10; printf("%d\n", a);
来源：http://kws.xziqi.cn

[S03] C：读入整数
来源：http://zph.shanyushiyangkeji.top

int x; scanf("%d", &x);
来源：http://zxy.wangdashe.top

[S04] C：字符串复制
来源：http://lcv.kuanghao11.cn

char dst[32]; strcpy(dst, "hi");
来源：http://oxv.ywan-chungtsiang.top

[S05] C：字符串长度
来源：http://luf.pengpengdd.cyou

strlen(s)
来源：http://qqq.zhixingplan.top

[S06] C：字符串比较
来源：http://leq.gogol.net.cn

strcmp(a, b) == 0
来源：http://lic.zycfv.cn

[S07] C：数组遍历求和
来源：http://hip.nanxinkj.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bok.zhoulong.xyz

[S08] C：动态内存分配与释放
来源：http://wrr.birdmap.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sfz.c1oappe.top

[S09] C：结构体定义与初始化
来源：http://dtt.xingfuxueyuan.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jma.sufxvd.cn

[S10] C：指针与解引用
来源：http://xib.snrcjt.cn

int *p = &a;  *p = 5;
来源：http://hps.vqdsnc.cn

[S11] C：逐行读文件
来源：http://ouc.ehwqpu.com

FILE *f = fopen("a.txt", "r");
来源：http://lte.yfazqb.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://ako.sysykeji.top

fclose(f);
来源：http://bxs.yongpay.top

[S12] C：写文件
来源：http://hpw.feifeiyinyue.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://epv.shzxlz.cn

[S13] C：宏定义
来源：http://rjd.yj20258888.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wjr.wangdashe.top

[S14] C：枚举
来源：http://snm.yuanzhike.top

enum Color { RED, GREEN, BLUE };
来源：http://skp.yj202588.top

[S15] C：类型转换
来源：http://ese.hysaishi.cn

(double) a / b
来源：http://kyq.sxryk.cn

[S16] C：位操作置位
来源：http://emc.jinyuanbaomall.cn

x |= (1 << 3);
来源：http://miu.cucudq.cn

[S17] C：安全拼接字符串
来源：http://bwq.vqdsnc.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ith.zdbjq.cn

[S18] C：命令行参数
来源：http://scn.shzxlz.cn

int main(int argc, char **argv)
来源：http://gsg.gogol.net.cn

[S19] C：快速排序
来源：http://ige.yfazqb.com

qsort(a, n, sizeof(int), cmp);
来源：http://ojg.vqdsnc.cn

[S20] C：二分查找
来源：http://ntc.tian-w.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hxv.iojbl.cn

[S21] C：字符类别判断
来源：http://jdi.xuetiantiany.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://uav.haohaochexian.top

[S22] C：字符串转数字
来源：http://emf.fzhhl.top

atoi("42");  strtod("3.14", NULL);
来源：http://cxb.bjfxy.top

[S23] C：随机数
来源：http://vrh.zhoulong.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://iaq.yj20258.top

[S24] C：获取本地时间
来源：http://egl.havefunace.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tem.hysaishi.cn

[S25] C：内存拷贝
来源：http://xnj.bjfxy.top

memcpy(dst, src, n);
来源：http://fbp.cqqwz.cn

[S26] C：内存清零
来源：http://usd.hongshengwenyu.top

memset(a, 0, sizeof a);
来源：http://nfl.feifeiyinyue.top

[S27] C：定义常量
来源：http://ekt.yonumen.top

const double PI = 3.14159;
来源：http://rax.fktsv.cn

[S28] C：静态变量
来源：http://los.hongshengwenyu.top

static int counter = 0;
来源：http://ulm.dashuyun.cn

[S29] C：变参函数
来源：http://opr.yuanzhike.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ari.sysykeji.top

[S30] C：头文件保护
来源：http://fcn.uphjek.com

#ifndef X_H
来源：http://qns.aizwys.cn

#define X_H
来源：http://fbj.cqqwz.cn

#endif
来源：http://lvd.shanyushiyangtech.top

[S31] C++：Hello World
来源：http://hwd.mhx1999.top

#include <iostream>
来源：http://bci.hnxiangtu.top

int main() { std::cout << "Hello\n"; }
来源：http://epl.ybcxt.top

[S32] C++：字符串
来源：http://ywz.yuxming.cn

std::string s = "hi";  s += "!";
来源：http://poc.yj202588.top

[S33] C++：vector 增删
来源：http://gtn.chenzaomai.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qsc.jqgfzy.top

[S34] C++：遍历 vector
来源：http://qls.bbcook.cn

for (auto &x : v) { std::cout << x; }
来源：http://vlv.yangfankeji.com

[S35] C++：map
来源：http://wvs.zdqjudy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kfi.aizwys.cn

[S36] C++：unordered_map
来源：http://lwv.yuxming.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hwe.ivvv.top

[S37] C++：set
来源：http://mbn.tian-w.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bdi.guannengcc.top

[S38] C++：排序
来源：http://wdu.yongpay.top

std::sort(v.begin(), v.end());
来源：http://rrm.zhengqikj.top

[S39] C++：自定义比较器排序
来源：http://lff.cheryme.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qwu.cucudq.cn

[S40] C++：查找元素
来源：http://gqg.feifeiyinyue.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ean.zhaomingkeji.xyz

[S41] C++：类与构造函数
来源：http://juf.xinyue.icu

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://olp.daria6918.cn

[S42] C++：继承与虚函数
来源：http://zbp.birdmap.top

class B : public Base { public: void f() override {} };
来源：http://uco.quarkkingdee.top

[S43] C++：智能指针
来源：http://uex.tarul.cn

auto p = std::make_unique<int>(5);
来源：http://ter.jianghu66.top

[S44] C++：引用传参
来源：http://cia.daxiang520.top

void inc(int &x) { ++x; }
来源：http://bau.shanyushiyangkeji.top

[S45] C++：lambda
来源：http://xye.shuidangran.top

auto add = [](int a, int b) { return a + b; };
来源：http://rab.zhongyouzk.top

[S46] C++：函数模板
来源：http://dpc.chenlongwang.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ekv.jqgufenzy.top

[S47] C++：结构化绑定遍历
来源：http://zhm.andypj.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xpn.chenzaomai.com

[S48] C++：逐行读文件
来源：http://gah.jinyuanbaomall.cn

std::ifstream in("a.txt");  std::string line;
来源：http://lbq.xingfuxueyuan.xyz

while (std::getline(in, line)) { }
来源：http://wcd.birdmap.top

[S49] C++：写文件
来源：http://wgc.yueranfly.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://edf.daria6918.cn

[S50] C++：格式化数字
来源：http://hze.feifeiyinyue.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://eqk.jinghuilouyu.cn

[S51] C++：显式类型转换
来源：http://vhi.jqgufenzy.top

static_cast<double>(a) / b
来源：http://ufe.yj20258888.top

[S52] C++：const 与 noexcept
来源：http://lwg.xuetiantiany.cn

int size() const noexcept { return n_; }
来源：http://biz.jiagoushi.top

[S53] C++：移动语义
来源：http://lgc.tanke756.top

std::vector<int> w = std::move(v);
来源：http://ztx.jqgfzy.top

[S54] C++：异常处理
来源：http://hvw.gotoacloud.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://iqe.hongshengwenyu.top

[S55] C++：结构化绑定
来源：http://kun.fengsongda.top

auto [a, b] = std::make_pair(1, 2);
来源：http://vlq.52xcode.cn

[S56] C++：optional
来源：http://czp.316326.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kgi.chenjidiqi.icu

[S57] C++：编译期常量
来源：http://rft.52xcode.cn

constexpr int N = 10;
来源：http://nlc.yuanzhike.top

[S58] C++：命名空间
来源：http://dvq.sxryk.cn

namespace ns { int f() { return 1; } }
来源：http://jsf.jinyuanbaomall.cn

[S59] C++：静态断言
来源：http://pvz.dashuyun.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://edf.yj202588.top

[S60] C++：遍历并删除元素
来源：http://rlm.zhiwuduotai.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xem.sxryk.cn

================================================================================
来源：http://jcs.dianchejie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vyv.zdbjq.cn

================================================================================
来源：http://oko.jinghuilouyu.cn

[T01] Kotlin：Hello World
来源：http://fnx.c1oappe.top

println("Hello")
来源：http://zdn.haohaochexian.top

[T02] Kotlin：变量
来源：http://vhh.shanyushiyangtech.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bgb.zdqjudy.top

[T03] Kotlin：字符串模板
来源：http://zta.zdbjq.cn

"值: $b"
来源：http://lcr.bbcook.cn

[T04] Kotlin：空安全
来源：http://kmf.svipenyu.cn

val n: String? = null;  n?.length
来源：http://rag.guannengcc.top

[T05] Kotlin：when 表达式
来源：http://jng.havefunace.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://djj.yangfankeji.com

[T06] Kotlin：集合映射
来源：http://xdf.zhixingplan.top

listOf(1, 2, 3).map { it * 2 }
来源：http://evp.0kj1m.cn

[T07] Kotlin：集合过滤
来源：http://bnw.316326.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://kqw.ivvv.top

[T08] Kotlin：数据类
来源：http://zbe.feifeiyinyue.top

data class User(val name: String, val age: Int)
来源：http://fal.havefunace.top

[T09] Kotlin：扩展函数
来源：http://bbo.zdbjq.cn

fun String.exclaim() = this + "!"
来源：http://jrh.kuanghao11.cn

[T10] Kotlin：默认参数
来源：http://sjg.shangyingyoupin.top

fun greet(name: String = "World") = "Hi $name"
来源：http://vdy.guannengcc.top

[T11] Kotlin：协程
来源：http://isa.zhengqikj.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://vxx.jiagoushi.top

[T12] Kotlin：解构声明
来源：http://ogc.wangdashe.top

val (a, b) = Pair(1, 2)
来源：http://ahw.gogol.net.cn

[T13] Kotlin：只读 Map
来源：http://xdl.ppjwa.cn

val m = mapOf("a" to 1)
来源：http://ajv.svipenyu.cn

[T14] Kotlin：循环
来源：http://zve.bbcook.cn

for (i in 1..10) println(i)
来源：http://plt.sufxvd.cn

[T15] Kotlin：接口
来源：http://rll.yvedp.cn

interface Shape { fun area(): Double }
来源：http://nob.jianghu66.top

[T16] Swift：Hello World
来源：http://dww.hesvh.cn

print("Hello")
来源：http://mxp.yueranfly.top

[T17] Swift：变量与常量
来源：http://mww.ydzc1.top

var a = 1;  let b = 2
来源：http://dhl.zhengqikj.top

[T18] Swift：字符串插值
来源：http://nta.sysykeji.top

"值: \(b)"
来源：http://igm.cashguo.top

[T19] Swift：可选绑定
来源：http://oko.zdbjq.cn

if let n = opt { print(n) }
来源：http://gss.mhx1999.top

[T20] Swift：数组操作
来源：http://ann.pycfn.com

var a = [1, 2, 3];  a.append(4)
来源：http://qqs.aizwys.cn

[T21] Swift：遍历
来源：http://iiu.feifeiyinyue.top

for x in a { print(x) }
来源：http://qej.tarul.cn

[T22] Swift：字典
来源：http://dxc.ctjpmb.com

var d = ["a": 1];  d["b"] = 2
来源：http://onh.ehwqpu.com

[T23] Swift：函数
来源：http://tvj.xuetiantiany.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kkn.ywan-chungtsiang.top

[T24] Swift：闭包
来源：http://xwo.nanxinkj.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://gme.xylfe.cn

[T25] Swift：结构体
来源：http://yzd.shzxlz.cn

struct P { var x: Int }
来源：http://vgj.hammf.cn

[T26] Swift：类与重写
来源：http://ith.yj20258.top

class A: Base { override func f() {} }
来源：http://ajq.sysykeji.top

[T27] Swift：错误处理
来源：http://njc.zhoulong.xyz

do { try f() } catch { print(error) }
来源：http://jed.cqqwz.cn

[T28] Swift：枚举
来源：http://ffm.jianghu66.top

enum Color { case red, green }
来源：http://ezj.hammf.cn

[T29] Swift：guard 提前返回
来源：http://uws.c1oappe.top

guard let x = opt else { return }
来源：http://icn.zhiwuduotai.top

[T30] Swift：协议
来源：http://rzw.jinyuanbaomall.cn

protocol Shape { func area() -> Double }
来源：http://alf.tian-w.cn


<!-- 参考信息 -->