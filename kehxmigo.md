代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://dyp.shanyushiyangkeji.top

[R32] 参数个数校验
来源：http://ewn.cdnleiting.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://svw.ppjwa.cn

[R33] 捕获错误并提示行号
来源：http://mfu.zhijiandao.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://net.hesvh.cn

[R34] 退出时清理
来源：http://bje.yanxiufei.cn

trap 'rm -f "$tmp"' EXIT
来源：http://moq.yongpay.top

[R35] 后台执行并等待
来源：http://tfd.wangdashe.top

sleep 5 & pid=$!; wait "$pid"
来源：http://zvu.jyoumei.cn

[R36] 并发执行多个任务
来源：http://yxf.shuidangran.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kmq.yfazqb.com

[R37] 把输出赋给变量
来源：http://gxz.havefunace.top

files=$(ls -1)
来源：http://ted.bbcook.cn

[R38] 管道串联
来源：http://msg.zhoulong.xyz

cat a.txt | grep -i error | wc -l
来源：http://tcj.tian-w.cn

[R39] 重定向标准输出与错误
来源：http://bnw.ctjpmb.com

cmd > out.log 2>&1
来源：http://don.wangshuangyany.cn

[R40] 追加写日志
来源：http://bke.yfazqb.com

echo "log" >> out.log
来源：http://phy.yongpay.top

[R41] 丢弃输出
来源：http://zkz.dashuyun.cn

cmd >/dev/null 2>&1
来源：http://wdx.zhoulong.xyz

[R42] 输入重定向
来源：http://uio.jiagoushi.top

wc -l < a.txt
来源：http://mhk.ybcxt.top

[R43] 按名字查找文件
来源：http://thl.jinqigufen.top

find . -name "*.log" -type f
来源：http://pcp.xziqi.cn

[R44] 按修改时间查找
来源：http://ugo.sxryk.cn

find . -mtime -7 -type f
来源：http://glc.tanke756.top

[R45] 批量删除
来源：http://erh.andypj.xyz

find . -name "*.tmp" -delete
来源：http://lwo.c1oappe.top

[R46] 递归替换文件内容
来源：http://qfk.zdbjq.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://iwz.shuidangran.top

[R47] sed 单行替换
来源：http://kuc.jiagoushi.top

sed -i 's/foo/bar/g' a.txt
来源：http://dtn.birdmap.top

[R48] awk 取指定列
来源：http://scz.fanxiaobao.xyz

awk '{print $1, $3}' a.txt
来源：http://iff.jinyuanbaomall.cn

[R49] awk 带条件
来源：http://pyf.gogol.net.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://exa.yangfankeji.com

[R50] awk 求和
来源：http://qpg.iojbl.cn

awk '{s += $2} END {print s}' a.txt
来源：http://gyr.yanxiufei.cn

[R51] 排序去重取前几
来源：http://pxz.daria6918.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://cub.ydjk.org.cn

[R52] 统计行数
来源：http://sax.dashuyun.cn

wc -l a.txt
来源：http://dir.zdbjq.cn

[R53] 查看文件头与实时尾
来源：http://ejy.shzxlz.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://she.aizwys.cn

[R54] 比较两个文件
来源：http://xfi.yonumen.top

diff a.txt b.txt
来源：http://hip.nanxuanxn.top

[R55] 压缩与解压
来源：http://rff.yongpay.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zid.ehwqpu.com

[R56] 远程拷贝
来源：http://vxe.epnwcf.com

scp file user@host:/path/
来源：http://gha.ybcxt.top

[R57] 远程执行命令
来源：http://qvh.yfazqb.com

ssh user@host 'uptime'
来源：http://hca.quarkkingdee.top

[R58] 下载文件
来源：http://cxo.aizwys.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yiq.bbcook.cn

[R59] 发 POST JSON
来源：http://eks.dashuyun.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fts.snrcjt.cn

[R60] 只看 HTTP 状态码
来源：http://gmk.jyoumei.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rlm.nanxuanxn.top

[R61] 磁盘占用
来源：http://icl.haohaochexian.top

df -h;  du -sh *
来源：http://lti.gzhubu.top

[R62] 找最占空间的文件
来源：http://viv.hnqzz.top

du -ah . | sort -rh | head -10
来源：http://sik.nwbrower.top

[R63] 内存与进程
来源：http://vjy.jinqigufen.top

free -h;  ps aux | grep nginx
来源：http://csk.zhixingplan.top

[R64] 结束进程
来源：http://sen.c1oappe.top

kill -9 $(pgrep -f app.py)
来源：http://fcb.meibo888.top

[R65] 查看端口占用
来源：http://ehk.yongpay.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xpc.vehdjk.com

[R66] 定时任务
来源：http://sjb.hysaishi.cn

crontab -e;  crontab -l
来源：http://tkk.cheryme.top

[R67] 生成随机十六进制串
来源：http://vak.vqdsnc.cn

openssl rand -hex 16
来源：http://rsf.chenlongwang.top

[R68] 计算文件校验值
来源：http://mew.xuetiantiany.cn

sha256sum a.txt;  md5sum a.txt
来源：http://cni.wangdashe.top

[R69] 生成随机密码
来源：http://zqo.jianghu66.top

head -c 16 /dev/urandom | base64
来源：http://vax.sweek.top

[R70] 时间戳与互转
来源：http://blv.uphjek.com

date +%s;  date -d @1700000000
来源：http://jzw.yueranfly.top

[R71] 日期格式化
来源：http://dec.shanyushiyangtech.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://swt.jqgufenzy.top

[R72] 等待端口就绪
来源：http://zwv.ehwqpu.com

until nc -z localhost 3306; do sleep 1; done
来源：http://bkg.gotoacloud.top

[R73] 分割大日志
来源：http://fsb.fktsv.cn

split -l 1000 big.log part_
来源：http://cay.bbcook.cn

[R74] 批量重命名
来源：http://ovo.hammf.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://aog.daxiang520.top

[R75] 导出环境变量
来源：http://uxh.fktsv.cn

export PATH="$HOME/bin:$PATH"
来源：http://bap.yuanzhike.top

[R76] 使用临时文件
来源：http://zyt.hongshengwenyu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nbw.xingfuxueyuan.xyz

[R77] 读取用户输入
来源：http://ufq.svipenyu.cn

read -rp "请输入: " ans
来源：http://qwg.nwbrower.top

[R78] 交互式菜单
来源：http://asn.tian-w.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://bih.hysaishi.cn

[R79] 解析命令行选项
来源：http://xxs.xylfe.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fdl.hongshengwenyu.top

[R80] 查看脚本执行耗时
来源：http://anz.gzhubu.top

time ./run.sh
来源：http://gef.quarkkingdee.top

================================================================================
来源：http://kaa.aizwys.cn

S. C / C++ 专题
来源：http://wfc.wangdashe.top

================================================================================
来源：http://ynn.daxiang520.top

[S01] C：Hello World
来源：http://aud.meibo888.top

#include <stdio.h>
来源：http://bzp.zycfv.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://aia.wangdashe.top

[S02] C：变量与格式化输出
来源：http://glq.sufxvd.cn

int a = 10; printf("%d\n", a);
来源：http://yky.fengsongda.top

[S03] C：读入整数
来源：http://adb.hfpthk.cn

int x; scanf("%d", &x);
来源：http://tfu.fanxiaobao.xyz

[S04] C：字符串复制
来源：http://evy.bbcook.cn

char dst[32]; strcpy(dst, "hi");
来源：http://mdc.zdqjudy.top

[S05] C：字符串长度
来源：http://rxw.xingfuxueyuan.xyz

strlen(s)
来源：http://ugx.pengpengdd.cyou

[S06] C：字符串比较
来源：http://nwy.fktsv.cn

strcmp(a, b) == 0
来源：http://zzg.shangyingyoupin.top

[S07] C：数组遍历求和
来源：http://ijn.kuanghao11.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hzd.tanke756.top

[S08] C：动态内存分配与释放
来源：http://msi.snrcjt.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zpn.ppjwa.cn

[S09] C：结构体定义与初始化
来源：http://pqa.yj202588.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ypk.chenlongwang.top

[S10] C：指针与解引用
来源：http://dgc.zycfv.cn

int *p = &a;  *p = 5;
来源：http://ips.jyoumei.cn

[S11] C：逐行读文件
来源：http://nwh.ywan-chungtsiang.top

FILE *f = fopen("a.txt", "r");
来源：http://jkp.tianlin.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://rtn.ydjk.org.cn

fclose(f);
来源：http://nnc.0kj1m.cn

[S12] C：写文件
来源：http://dxu.hammf.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lpy.fengsongda.top

[S13] C：宏定义
来源：http://oqb.shzxlz.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ktd.guannengcc.top

[S14] C：枚举
来源：http://gtx.nanxuanxn.top

enum Color { RED, GREEN, BLUE };
来源：http://vjq.nanxuanxn.top

[S15] C：类型转换
来源：http://tfh.gotoacloud.top

(double) a / b
来源：http://ekp.yfazqb.com

[S16] C：位操作置位
来源：http://tyx.uphjek.com

x |= (1 << 3);
来源：http://jsh.ydjk.org.cn

[S17] C：安全拼接字符串
来源：http://emr.jyoumei.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jqg.yueranfly.top

[S18] C：命令行参数
来源：http://dug.gotoacloud.top

int main(int argc, char **argv)
来源：http://fjw.tanke756.top

[S19] C：快速排序
来源：http://inr.fktsv.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ifl.mhx1999.top

[S20] C：二分查找
来源：http://wxc.svipenyu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vnc.chenzaomai.com

[S21] C：字符类别判断
来源：http://ojc.yangfankeji.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hbb.cucudq.cn

[S22] C：字符串转数字
来源：http://xfl.shangyingyoupin.top

atoi("42");  strtod("3.14", NULL);
来源：http://gjc.epnwcf.com

[S23] C：随机数
来源：http://lgv.yuanzhike.top

srand(time(NULL));  int r = rand() % 100;
来源：http://akn.guannengcc.top

[S24] C：获取本地时间
来源：http://cyc.tanke756.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ghh.ivvv.top

[S25] C：内存拷贝
来源：http://qmo.sweek.top

memcpy(dst, src, n);
来源：http://gev.zhaomingkeji.xyz

[S26] C：内存清零
来源：http://ays.hnqzz.top

memset(a, 0, sizeof a);
来源：http://ipo.nwbrower.top

[S27] C：定义常量
来源：http://cpj.tian-w.cn

const double PI = 3.14159;
来源：http://bvz.9152youxi.cn

[S28] C：静态变量
来源：http://qsj.hfpthk.cn

static int counter = 0;
来源：http://szy.xziqi.cn

[S29] C：变参函数
来源：http://iry.hesvh.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qbd.shuidangran.top

[S30] C：头文件保护
来源：http://yiq.zhongyouzk.top

#ifndef X_H
来源：http://ozl.jyoumei.cn

#define X_H
来源：http://vyj.haohaochexian.top

#endif
来源：http://kvx.guowangkeji.top

[S31] C++：Hello World
来源：http://kde.sweek.top

#include <iostream>
来源：http://rsi.sysykeji.top

int main() { std::cout << "Hello\n"; }
来源：http://dgm.0kj1m.cn

[S32] C++：字符串
来源：http://miq.yj20258.top

std::string s = "hi";  s += "!";
来源：http://tff.cdnleiting.top

[S33] C++：vector 增删
来源：http://vyr.jlsjyb.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ftd.andypj.xyz

[S34] C++：遍历 vector
来源：http://pcg.zhengqikj.top

for (auto &x : v) { std::cout << x; }
来源：http://hrf.hammf.cn

[S35] C++：map
来源：http://buu.pengpengdd.cyou

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mlw.yvedp.cn

[S36] C++：unordered_map
来源：http://bjq.c1oappe.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ymm.nwbrower.top

[S37] C++：set
来源：http://tph.yanxiufei.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://buw.wangshuangyany.cn

[S38] C++：排序
来源：http://wjz.zhoulong.xyz

std::sort(v.begin(), v.end());
来源：http://pqg.jiagoushi.top

[S39] C++：自定义比较器排序
来源：http://dzx.hammf.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kbv.cheryme.top

[S40] C++：查找元素
来源：http://jth.hnxiangtu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://elk.svipenyu.cn

[S41] C++：类与构造函数
来源：http://vjj.guowangkeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vdr.nanxuanxn.top

[S42] C++：继承与虚函数
来源：http://qyi.shanyushiyangkeji.top

class B : public Base { public: void f() override {} };
来源：http://jed.meibo888.top

[S43] C++：智能指针
来源：http://vrg.chenjidiqi.icu

auto p = std::make_unique<int>(5);
来源：http://ypy.zycfv.cn

[S44] C++：引用传参
来源：http://tmg.zhongyouzk.top

void inc(int &x) { ++x; }
来源：http://hbp.zycfv.cn

[S45] C++：lambda
来源：http://eba.fengsongda.top

auto add = [](int a, int b) { return a + b; };
来源：http://ypo.ehwqpu.com

[S46] C++：函数模板
来源：http://kky.yuxming.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://oej.zhijiandao.cn

[S47] C++：结构化绑定遍历
来源：http://qfu.tarul.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://owt.daxiang520.top

[S48] C++：逐行读文件
来源：http://meq.52xcode.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gtv.ybcxt.top

while (std::getline(in, line)) { }
来源：http://eax.hnxiangtu.top

[S49] C++：写文件
来源：http://jlq.wangshuangyany.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wgm.sweek.top

[S50] C++：格式化数字
来源：http://kbu.sjlbkw.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lqj.yonumen.top

[S51] C++：显式类型转换
来源：http://xpf.chenjidiqi.icu

static_cast<double>(a) / b
来源：http://wov.mhx1999.top

[S52] C++：const 与 noexcept
来源：http://jlv.ydjk.org.cn

int size() const noexcept { return n_; }
来源：http://gsu.guannengcc.top

[S53] C++：移动语义
来源：http://axw.jianghu66.top

std::vector<int> w = std::move(v);
来源：http://bhc.smart0.xyz

[S54] C++：异常处理
来源：http://dzi.hesvh.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ilh.dashuyun.cn

[S55] C++：结构化绑定
来源：http://ehf.epnwcf.com

auto [a, b] = std::make_pair(1, 2);
来源：http://uhx.sysykeji.top

[S56] C++：optional
来源：http://wrc.zhaomingkeji.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ptu.mhx1999.top

[S57] C++：编译期常量
来源：http://bxg.epnwcf.com

constexpr int N = 10;
来源：http://ice.guowangkeji.top

[S58] C++：命名空间
来源：http://tzp.aibaodan.cn

namespace ns { int f() { return 1; } }
来源：http://hxi.wangdashe.top

[S59] C++：静态断言
来源：http://iqg.zhijiandao.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ftd.cqqwz.cn

[S60] C++：遍历并删除元素
来源：http://rtd.redwolf501.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rgr.hywenlv.cn

================================================================================
来源：http://eeo.vehdjk.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tfy.c1oappe.top

================================================================================
来源：http://vri.nanxuanxn.top

[T01] Kotlin：Hello World
来源：http://har.zdqjudy.top

println("Hello")
来源：http://trl.xziqi.cn

[T02] Kotlin：变量
来源：http://ssk.zycfv.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rzv.jinghuilouyu.cn

[T03] Kotlin：字符串模板
来源：http://xyn.cheryme.top

"值: $b"
来源：http://fvc.guowangkeji.top

[T04] Kotlin：空安全
来源：http://lgq.sxryk.cn

val n: String? = null;  n?.length
来源：http://tkr.feifeiyinyue.top

[T05] Kotlin：when 表达式
来源：http://lup.chenzaomai.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bix.0kj1m.cn

[T06] Kotlin：集合映射
来源：http://bmt.shanyushiyangtech.top

listOf(1, 2, 3).map { it * 2 }
来源：http://fdo.hysaishi.cn

[T07] Kotlin：集合过滤
来源：http://tix.ydjk.org.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ciq.hysaishi.cn

[T08] Kotlin：数据类
来源：http://pqc.shuidangran.top

data class User(val name: String, val age: Int)
来源：http://rfn.ydzc1.top

[T09] Kotlin：扩展函数
来源：http://luk.dianchejie.cn

fun String.exclaim() = this + "!"
来源：http://eed.jlsjyb.cn

[T10] Kotlin：默认参数
来源：http://ibu.shuidangran.top

fun greet(name: String = "World") = "Hi $name"
来源：http://fgo.yueranfly.top

[T11] Kotlin：协程
来源：http://ywh.bbcook.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://fin.tian-w.cn

[T12] Kotlin：解构声明
来源：http://pgw.tanke756.top

val (a, b) = Pair(1, 2)
来源：http://gvj.vehdjk.com

[T13] Kotlin：只读 Map
来源：http://qcw.pengpengdd.cyou

val m = mapOf("a" to 1)
来源：http://xxe.hywenlv.cn

[T14] Kotlin：循环
来源：http://rjj.ybcxt.top

for (i in 1..10) println(i)
来源：http://kcf.xuanzx.com

[T15] Kotlin：接口
来源：http://aih.yonumen.top

interface Shape { fun area(): Double }
来源：http://ima.uphjek.com

[T16] Swift：Hello World
来源：http://mcx.fktsv.cn

print("Hello")
来源：http://ezg.jqgufenzy.top

[T17] Swift：变量与常量
来源：http://udp.ehwqpu.com

var a = 1;  let b = 2
来源：http://qhl.jlsjyb.cn

[T18] Swift：字符串插值
来源：http://bax.xingfuxueyuan.xyz

"值: \(b)"
来源：http://gbo.smart0.xyz

[T19] Swift：可选绑定
来源：http://xxm.jqgfzy.top

if let n = opt { print(n) }
来源：http://ptd.fanxiaobao.xyz

[T20] Swift：数组操作
来源：http://xcn.wangshuangyany.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ytg.kuanghao11.cn

[T21] Swift：遍历
来源：http://fys.wangshuangyany.cn

for x in a { print(x) }
来源：http://imu.havefunace.top

[T22] Swift：字典
来源：http://smi.chenlongwang.top

var d = ["a": 1];  d["b"] = 2
来源：http://foy.hfpthk.cn

[T23] Swift：函数
来源：http://oyo.shangyingyoupin.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zyz.gogol.net.cn

[T24] Swift：闭包
来源：http://dxg.sysykeji.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://csh.zhengqikj.top

[T25] Swift：结构体
来源：http://qxp.havefunace.top

struct P { var x: Int }
来源：http://yjq.sysykeji.top

[T26] Swift：类与重写
来源：http://war.jyoumei.cn

class A: Base { override func f() {} }
来源：http://ert.havefunace.top

[T27] Swift：错误处理
来源：http://qkr.gzhubu.top

do { try f() } catch { print(error) }
来源：http://lhy.chenzaomai.com

[T28] Swift：枚举
来源：http://nxq.shanyushiyangkeji.top

enum Color { case red, green }
来源：http://ywv.gzhubu.top

[T29] Swift：guard 提前返回
来源：http://tef.yuxming.cn

guard let x = opt else { return }
来源：http://pgf.kuanghao11.cn

[T30] Swift：协议
来源：http://des.316326.xyz

protocol Shape { func area() -> Double }
来源：http://fmz.cdnleiting.top

[T31] Lua：Hello World
来源：http://dhf.shanyushiyangkeji.top

print("Hello")
来源：http://xlz.hywenlv.cn

[T32] Lua：局部变量
来源：http://tfk.yongpay.top

local a = 1
来源：http://fyc.epnwcf.com

[T33] Lua：表（数组）
来源：http://ejr.guowangkeji.top

local t = {1, 2, 3};  t[4] = 4
来源：http://dag.gogol.net.cn

[T34] Lua：遍历表
来源：http://ich.vehdjk.com

for i, v in ipairs(t) do print(i, v) end
来源：http://gqu.guowangkeji.top


<!-- 参考信息 -->