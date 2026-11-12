代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://ota.fehbvm.com

[R36] 并发执行多个任务
来源：http://mou.ppjwa.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://aou.nanxuanxn.top

[R37] 把输出赋给变量
来源：http://rje.smart0.xyz

files=$(ls -1)
来源：http://euj.pengpengdd.cyou

[R38] 管道串联
来源：http://qit.ydzc1.top

cat a.txt | grep -i error | wc -l
来源：http://cfn.fehbvm.com

[R39] 重定向标准输出与错误
来源：http://qmn.tianlin.xyz

cmd > out.log 2>&1
来源：http://phd.shuidangran.top

[R40] 追加写日志
来源：http://uxm.yonumen.top

echo "log" >> out.log
来源：http://uhc.xuetiantiany.cn

[R41] 丢弃输出
来源：http://peo.redwolf501.top

cmd >/dev/null 2>&1
来源：http://mdn.sxryk.cn

[R42] 输入重定向
来源：http://fyl.gzhubu.top

wc -l < a.txt
来源：http://gcy.xziqi.cn

[R43] 按名字查找文件
来源：http://jhq.shzxlz.cn

find . -name "*.log" -type f
来源：http://fww.uphjek.com

[R44] 按修改时间查找
来源：http://srz.ppjwa.cn

find . -mtime -7 -type f
来源：http://sca.316326.xyz

[R45] 批量删除
来源：http://mma.shzxlz.cn

find . -name "*.tmp" -delete
来源：http://yla.pengpengdd.cyou

[R46] 递归替换文件内容
来源：http://pko.aibaodan.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bfu.xinyue.icu

[R47] sed 单行替换
来源：http://aix.hammf.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ybu.9152youxi.cn

[R48] awk 取指定列
来源：http://hvw.yfazqb.com

awk '{print $1, $3}' a.txt
来源：http://jdo.jinyuanbaomall.cn

[R49] awk 带条件
来源：http://idg.sufxvd.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cig.jyoumei.cn

[R50] awk 求和
来源：http://qtc.nanxuanxn.top

awk '{s += $2} END {print s}' a.txt
来源：http://nlr.hnqzz.top

[R51] 排序去重取前几
来源：http://oyn.cdnleiting.top

sort a.txt | uniq -c | sort -rn | head
来源：http://uvb.wangdashe.top

[R52] 统计行数
来源：http://zwm.zhaomingkeji.xyz

wc -l a.txt
来源：http://qdt.xylfe.cn

[R53] 查看文件头与实时尾
来源：http://afx.yonumen.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pkp.guowangkeji.top

[R54] 比较两个文件
来源：http://vmv.nanxuanxn.top

diff a.txt b.txt
来源：http://uxf.zhijiandao.cn

[R55] 压缩与解压
来源：http://npg.gogol.net.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://azj.hammf.cn

[R56] 远程拷贝
来源：http://vlf.ybcxt.top

scp file user@host:/path/
来源：http://qis.wangdashe.top

[R57] 远程执行命令
来源：http://tdk.yvedp.cn

ssh user@host 'uptime'
来源：http://gnl.tarul.cn

[R58] 下载文件
来源：http://muh.zhongyouzk.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zya.zhiwuduotai.top

[R59] 发 POST JSON
来源：http://aji.cashguo.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://uqu.cucudq.cn

[R60] 只看 HTTP 状态码
来源：http://tba.zhijiandao.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://aet.gotoacloud.top

[R61] 磁盘占用
来源：http://ocu.yangfankeji.com

df -h;  du -sh *
来源：http://mlf.chenzaomai.com

[R62] 找最占空间的文件
来源：http://vfl.yj20258.top

du -ah . | sort -rh | head -10
来源：http://omr.jianghu66.top

[R63] 内存与进程
来源：http://sqd.uphjek.com

free -h;  ps aux | grep nginx
来源：http://nxk.zycfv.cn

[R64] 结束进程
来源：http://emc.chenzaomai.com

kill -9 $(pgrep -f app.py)
来源：http://wmz.shanyushiyangkeji.top

[R65] 查看端口占用
来源：http://ejk.havefunace.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cle.nanxinkj.top

[R66] 定时任务
来源：http://yms.andypj.xyz

crontab -e;  crontab -l
来源：http://epj.cheryme.top

[R67] 生成随机十六进制串
来源：http://lyh.ybcxt.top

openssl rand -hex 16
来源：http://wtr.zycfv.cn

[R68] 计算文件校验值
来源：http://cpg.sxryk.cn

sha256sum a.txt;  md5sum a.txt
来源：http://pnc.shangyingyoupin.top

[R69] 生成随机密码
来源：http://cpv.xingfuxueyuan.xyz

head -c 16 /dev/urandom | base64
来源：http://vgy.tanke756.top

[R70] 时间戳与互转
来源：http://paj.smart0.xyz

date +%s;  date -d @1700000000
来源：http://oft.cucudq.cn

[R71] 日期格式化
来源：http://tiq.zhiwuduotai.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ueg.ydjk.org.cn

[R72] 等待端口就绪
来源：http://tkv.nanxinkj.top

until nc -z localhost 3306; do sleep 1; done
来源：http://gqr.wangdashe.top

[R73] 分割大日志
来源：http://oun.zhixingplan.top

split -l 1000 big.log part_
来源：http://bsg.xinyue.icu

[R74] 批量重命名
来源：http://fyk.shzxlz.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qzm.zhaomingkeji.xyz

[R75] 导出环境变量
来源：http://hsi.yfazqb.com

export PATH="$HOME/bin:$PATH"
来源：http://xmg.9152youxi.cn

[R76] 使用临时文件
来源：http://kzu.yanxiufei.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ntd.svipenyu.cn

[R77] 读取用户输入
来源：http://aae.cucudq.cn

read -rp "请输入: " ans
来源：http://vxl.zhoulong.xyz

[R78] 交互式菜单
来源：http://zry.yonumen.top

select opt in a b c; do echo "$opt"; break; done
来源：http://flq.chenjidiqi.icu

[R79] 解析命令行选项
来源：http://euq.feifeiyinyue.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tmc.fzhhl.top

[R80] 查看脚本执行耗时
来源：http://byt.cdnleiting.top

time ./run.sh
来源：http://qsr.fehbvm.com

================================================================================
来源：http://xlo.yangfankeji.com

S. C / C++ 专题
来源：http://qpp.cheryme.top

================================================================================
来源：http://zzd.feifeiyinyue.top

[S01] C：Hello World
来源：http://isj.hysaishi.cn

#include <stdio.h>
来源：http://akr.c1oappe.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://afi.fktsv.cn

[S02] C：变量与格式化输出
来源：http://lob.fanxiaobao.xyz

int a = 10; printf("%d\n", a);
来源：http://qrq.xuetiantiany.cn

[S03] C：读入整数
来源：http://otf.aizwys.cn

int x; scanf("%d", &x);
来源：http://ggw.yuanzhike.top

[S04] C：字符串复制
来源：http://pfg.cdnleiting.top

char dst[32]; strcpy(dst, "hi");
来源：http://cfn.uphjek.com

[S05] C：字符串长度
来源：http://mse.hammf.cn

strlen(s)
来源：http://nei.xylfe.cn

[S06] C：字符串比较
来源：http://sxv.xylfe.cn

strcmp(a, b) == 0
来源：http://jpm.fehbvm.com

[S07] C：数组遍历求和
来源：http://key.nwbrower.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qww.ppjwa.cn

[S08] C：动态内存分配与释放
来源：http://heh.chenlongwang.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rih.xylfe.cn

[S09] C：结构体定义与初始化
来源：http://fzc.sysykeji.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wlk.zdbjq.cn

[S10] C：指针与解引用
来源：http://pte.yuxming.cn

int *p = &a;  *p = 5;
来源：http://shp.hysaishi.cn

[S11] C：逐行读文件
来源：http://fme.tianlin.xyz

FILE *f = fopen("a.txt", "r");
来源：http://tmu.gotoacloud.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://txn.fzhhl.top

fclose(f);
来源：http://usy.ydjk.org.cn

[S12] C：写文件
来源：http://ver.xziqi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://axx.andypj.xyz

[S13] C：宏定义
来源：http://ted.zhoulong.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://imp.havefunace.top

[S14] C：枚举
来源：http://tnv.316326.xyz

enum Color { RED, GREEN, BLUE };
来源：http://dgp.vehdjk.com

[S15] C：类型转换
来源：http://ofm.xziqi.cn

(double) a / b
来源：http://iby.cashguo.top

[S16] C：位操作置位
来源：http://bcm.ehwqpu.com

x |= (1 << 3);
来源：http://jzg.havefunace.top

[S17] C：安全拼接字符串
来源：http://crr.cucudq.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gua.havefunace.top

[S18] C：命令行参数
来源：http://lvx.ydjk.org.cn

int main(int argc, char **argv)
来源：http://crj.ivvv.top

[S19] C：快速排序
来源：http://wol.nanxinkj.top

qsort(a, n, sizeof(int), cmp);
来源：http://zbg.pengpengdd.cyou

[S20] C：二分查找
来源：http://bnf.hywenlv.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ugk.yongpay.top

[S21] C：字符类别判断
来源：http://sfn.yueranfly.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ghc.daria6918.cn

[S22] C：字符串转数字
来源：http://cjm.ydzc1.top

atoi("42");  strtod("3.14", NULL);
来源：http://awy.sufxvd.cn

[S23] C：随机数
来源：http://pdz.pengpengdd.cyou

srand(time(NULL));  int r = rand() % 100;
来源：http://jwl.ivvv.top

[S24] C：获取本地时间
来源：http://dzt.yj202588.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vbi.xuetiantiany.cn

[S25] C：内存拷贝
来源：http://dxs.svipenyu.cn

memcpy(dst, src, n);
来源：http://ljn.wangshuangyany.cn

[S26] C：内存清零
来源：http://yxw.vqdsnc.cn

memset(a, 0, sizeof a);
来源：http://vgf.kuanghao11.cn

[S27] C：定义常量
来源：http://wmm.zhijiandao.cn

const double PI = 3.14159;
来源：http://peh.dianchejie.cn

[S28] C：静态变量
来源：http://ywr.feifeiyinyue.top

static int counter = 0;
来源：http://hjt.ydzc1.top

[S29] C：变参函数
来源：http://hjd.ctjpmb.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qdl.smart0.xyz

[S30] C：头文件保护
来源：http://zow.dianchejie.cn

#ifndef X_H
来源：http://fdw.sufxvd.cn

#define X_H
来源：http://rhg.yonumen.top

#endif
来源：http://nay.jqgufenzy.top

[S31] C++：Hello World
来源：http://qas.ywan-chungtsiang.top

#include <iostream>
来源：http://iry.ywan-chungtsiang.top

int main() { std::cout << "Hello\n"; }
来源：http://wse.guannengcc.top

[S32] C++：字符串
来源：http://kdr.cucudq.cn

std::string s = "hi";  s += "!";
来源：http://qdl.svipenyu.cn

[S33] C++：vector 增删
来源：http://tfk.guowangkeji.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kcx.ywan-chungtsiang.top

[S34] C++：遍历 vector
来源：http://nnn.ywan-chungtsiang.top

for (auto &x : v) { std::cout << x; }
来源：http://hln.jinyuanbaomall.cn

[S35] C++：map
来源：http://let.zhaomingkeji.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mfj.zdbjq.cn

[S36] C++：unordered_map
来源：http://xas.nwbrower.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vgp.aibaodan.cn

[S37] C++：set
来源：http://ntk.shanyushiyangtech.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vrr.aibaodan.cn

[S38] C++：排序
来源：http://yyw.zdqjudy.top

std::sort(v.begin(), v.end());
来源：http://wkk.sysykeji.top

[S39] C++：自定义比较器排序
来源：http://cwv.daxiang520.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xet.guowangkeji.top

[S40] C++：查找元素
来源：http://ndu.ppjwa.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pro.sweek.top

[S41] C++：类与构造函数
来源：http://hsr.havefunace.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://alc.hcnkem.com

[S42] C++：继承与虚函数
来源：http://yxu.tanke756.top

class B : public Base { public: void f() override {} };
来源：http://fqf.nanxinkj.top

[S43] C++：智能指针
来源：http://jxa.jlsjyb.cn

auto p = std::make_unique<int>(5);
来源：http://icp.xuetiantiany.cn

[S44] C++：引用传参
来源：http://bzb.yj20258888.top

void inc(int &x) { ++x; }
来源：http://asb.zhixingplan.top

[S45] C++：lambda
来源：http://lvn.haohaochexian.top

auto add = [](int a, int b) { return a + b; };
来源：http://exe.tianlin.xyz

[S46] C++：函数模板
来源：http://rpc.0kj1m.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hwm.9152youxi.cn

[S47] C++：结构化绑定遍历
来源：http://brf.aibaodan.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ebu.shangyingyoupin.top

[S48] C++：逐行读文件
来源：http://vkz.yj202588.top

std::ifstream in("a.txt");  std::string line;
来源：http://wwd.birdmap.top

while (std::getline(in, line)) { }
来源：http://xwh.chenjidiqi.icu

[S49] C++：写文件
来源：http://uhm.gotoacloud.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mqx.xinyue.icu

[S50] C++：格式化数字
来源：http://yel.fktsv.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lxz.wangshuangyany.cn

[S51] C++：显式类型转换
来源：http://muv.ywan-chungtsiang.top

static_cast<double>(a) / b
来源：http://svo.hammf.cn

[S52] C++：const 与 noexcept
来源：http://asl.jinghuilouyu.cn

int size() const noexcept { return n_; }
来源：http://rhl.tianlin.xyz

[S53] C++：移动语义
来源：http://mox.yonumen.top

std::vector<int> w = std::move(v);
来源：http://xot.zhongyouzk.top

[S54] C++：异常处理
来源：http://cix.yfazqb.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fer.zdbjq.cn

[S55] C++：结构化绑定
来源：http://whx.dianchejie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xli.cashguo.top

[S56] C++：optional
来源：http://ktu.epnwcf.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qtv.yueranfly.top

[S57] C++：编译期常量
来源：http://adu.tianlin.xyz

constexpr int N = 10;
来源：http://opg.feifeiyinyue.top

[S58] C++：命名空间
来源：http://grw.yonumen.top

namespace ns { int f() { return 1; } }
来源：http://dfu.yvedp.cn

[S59] C++：静态断言
来源：http://aup.yj20258.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://izg.jianghu66.top

[S60] C++：遍历并删除元素
来源：http://cta.pengpengdd.cyou

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jra.9152youxi.cn

================================================================================
来源：http://dyw.fengsongda.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qwh.yonumen.top

================================================================================
来源：http://wiw.jiagoushi.top

[T01] Kotlin：Hello World
来源：http://sfr.shanyushiyangtech.top

println("Hello")
来源：http://jsd.sjlbkw.cn

[T02] Kotlin：变量
来源：http://roo.gaohongyu789.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://egl.xuanzx.com

[T03] Kotlin：字符串模板
来源：http://ssr.zhongyouzk.top

"值: $b"
来源：http://yog.mhx1999.top

[T04] Kotlin：空安全
来源：http://isc.hfpthk.cn

val n: String? = null;  n?.length
来源：http://rfh.meibo888.top

[T05] Kotlin：when 表达式
来源：http://dye.xingfuxueyuan.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qvn.tarul.cn

[T06] Kotlin：集合映射
来源：http://jgu.iojbl.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://kac.snrcjt.cn

[T07] Kotlin：集合过滤
来源：http://alu.hongshengwenyu.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://hkj.hnqzz.top

[T08] Kotlin：数据类
来源：http://bfa.ywan-chungtsiang.top

data class User(val name: String, val age: Int)
来源：http://mhy.feifeiyinyue.top

[T09] Kotlin：扩展函数
来源：http://wps.tarul.cn

fun String.exclaim() = this + "!"
来源：http://rfr.uphjek.com

[T10] Kotlin：默认参数
来源：http://blh.feifeiyinyue.top

fun greet(name: String = "World") = "Hi $name"
来源：http://kux.jqgfzy.top

[T11] Kotlin：协程
来源：http://yqw.jinyuanbaomall.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xgc.jqgfzy.top

[T12] Kotlin：解构声明
来源：http://rgz.yanxiufei.cn

val (a, b) = Pair(1, 2)
来源：http://bgk.snrcjt.cn

[T13] Kotlin：只读 Map
来源：http://dxj.andypj.xyz

val m = mapOf("a" to 1)
来源：http://edt.gzhubu.top

[T14] Kotlin：循环
来源：http://zlz.xylfe.cn

for (i in 1..10) println(i)
来源：http://ydm.kuanghao11.cn

[T15] Kotlin：接口
来源：http://rut.shanyushiyangtech.top

interface Shape { fun area(): Double }
来源：http://gke.tianlin.xyz

[T16] Swift：Hello World
来源：http://rmc.hnqzz.top

print("Hello")
来源：http://rpb.mhx1999.top

[T17] Swift：变量与常量
来源：http://zon.xinyue.icu

var a = 1;  let b = 2
来源：http://ncu.gzhubu.top

[T18] Swift：字符串插值
来源：http://yeo.yj20258.top

"值: \(b)"
来源：http://spd.shangyingyoupin.top

[T19] Swift：可选绑定
来源：http://otl.cashguo.top

if let n = opt { print(n) }
来源：http://xmq.cdnleiting.top

[T20] Swift：数组操作
来源：http://owr.zycfv.cn

var a = [1, 2, 3];  a.append(4)
来源：http://tqs.hammf.cn

[T21] Swift：遍历
来源：http://gwp.ybcxt.top

for x in a { print(x) }
来源：http://cbd.cdnleiting.top

[T22] Swift：字典
来源：http://pek.zhiwuduotai.top

var d = ["a": 1];  d["b"] = 2
来源：http://opl.yvedp.cn

[T23] Swift：函数
来源：http://qnn.vehdjk.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vkf.9152youxi.cn

[T24] Swift：闭包
来源：http://mlu.ydjk.org.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://poq.guannengcc.top

[T25] Swift：结构体
来源：http://por.yuxming.cn

struct P { var x: Int }
来源：http://osq.tian-w.cn

[T26] Swift：类与重写
来源：http://vwv.ybcxt.top

class A: Base { override func f() {} }
来源：http://ugw.daria6918.cn

[T27] Swift：错误处理
来源：http://bzm.yj202588.top

do { try f() } catch { print(error) }
来源：http://iju.xylfe.cn

[T28] Swift：枚举
来源：http://hnu.sweek.top

enum Color { case red, green }
来源：http://hao.hammf.cn

[T29] Swift：guard 提前返回
来源：http://tyh.jianghu66.top

guard let x = opt else { return }
来源：http://gcs.daria6918.cn

[T30] Swift：协议
来源：http://yvy.52xcode.cn

protocol Shape { func area() -> Double }
来源：http://dda.cdnleiting.top

[T31] Lua：Hello World
来源：http://hzj.redwolf501.top

print("Hello")
来源：http://nzu.zdqjudy.top

[T32] Lua：局部变量
来源：http://que.pengpengdd.cyou

local a = 1
来源：http://tys.vehdjk.com

[T33] Lua：表（数组）
来源：http://asd.snrcjt.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://tcq.zycfv.cn

[T34] Lua：遍历表
来源：http://yix.shzxlz.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://dtn.jiagoushi.top

[T35] Lua：字典表
来源：http://vgp.yongpay.top

local d = { a = 1 };  d.b = 2
来源：http://vbr.aizwys.cn

[T36] Lua：函数
来源：http://bgx.mhx1999.top

function add(a, b) return a + b end
来源：http://sul.zhongyouzk.top

[T37] Lua：字符串拼接
来源：http://izs.yuxming.cn

"a" .. "b"
来源：http://msm.jinghuilouyu.cn

[T38] Lua：条件
来源：http://gkp.jqgufenzy.top

if x > 0 then print("正") end
来源：http://wug.hongshengwenyu.top


<!-- 参考信息 -->