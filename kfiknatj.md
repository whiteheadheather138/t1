代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hqe.yj202588.top

[R30] 函数返回状态码
来源：http://zpz.ctjpmb.com

f() { return 0; }; f || echo "失败了"
来源：http://itg.cdnleiting.top

[R31] 局部变量
来源：http://rrk.sxryk.cn

f() { local x=1; echo "$x"; }
来源：http://bhk.yonumen.top

[R32] 参数个数校验
来源：http://yus.yj20258888.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yiu.sweek.top

[R33] 捕获错误并提示行号
来源：http://jfe.aizwys.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://udi.sysykeji.top

[R34] 退出时清理
来源：http://uky.zycfv.cn

trap 'rm -f "$tmp"' EXIT
来源：http://uvf.hesvh.cn

[R35] 后台执行并等待
来源：http://idr.jiagoushi.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ugu.jinqigfzy.top

[R36] 并发执行多个任务
来源：http://hvd.zhiwuduotai.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vtp.aizwys.cn

[R37] 把输出赋给变量
来源：http://xlr.ctjpmb.com

files=$(ls -1)
来源：http://ojd.sjlbkw.cn

[R38] 管道串联
来源：http://hfu.xinyue.icu

cat a.txt | grep -i error | wc -l
来源：http://ymt.chenlongwang.top

[R39] 重定向标准输出与错误
来源：http://pzr.fzhhl.top

cmd > out.log 2>&1
来源：http://ftu.cashguo.top

[R40] 追加写日志
来源：http://nvg.yangfankeji.com

echo "log" >> out.log
来源：http://vth.ywan-chungtsiang.top

[R41] 丢弃输出
来源：http://apl.gogol.net.cn

cmd >/dev/null 2>&1
来源：http://vpp.cdnleiting.top

[R42] 输入重定向
来源：http://lvc.xinyue.icu

wc -l < a.txt
来源：http://vlx.shzxlz.cn

[R43] 按名字查找文件
来源：http://jes.jlsjyb.cn

find . -name "*.log" -type f
来源：http://pph.fzhhl.top

[R44] 按修改时间查找
来源：http://inl.cqqwz.cn

find . -mtime -7 -type f
来源：http://spl.meibo888.top

[R45] 批量删除
来源：http://nzj.jinqigfzy.top

find . -name "*.tmp" -delete
来源：http://mwm.xuanzx.com

[R46] 递归替换文件内容
来源：http://eiu.shzxlz.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ufj.nwbrower.top

[R47] sed 单行替换
来源：http://fti.shanyushiyangtech.top

sed -i 's/foo/bar/g' a.txt
来源：http://mor.chenlongwang.top

[R48] awk 取指定列
来源：http://kub.yueranfly.top

awk '{print $1, $3}' a.txt
来源：http://xha.chenzaomai.com

[R49] awk 带条件
来源：http://nbj.gaohongyu789.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://iuv.meibo888.top

[R50] awk 求和
来源：http://ght.316326.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://ltx.guannengcc.top

[R51] 排序去重取前几
来源：http://knf.epnwcf.com

sort a.txt | uniq -c | sort -rn | head
来源：http://bvo.kuanghao11.cn

[R52] 统计行数
来源：http://nlw.epnwcf.com

wc -l a.txt
来源：http://pln.snrcjt.cn

[R53] 查看文件头与实时尾
来源：http://tfc.shanyushiyangtech.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://trb.tian-w.cn

[R54] 比较两个文件
来源：http://iji.jinqigfzy.top

diff a.txt b.txt
来源：http://fth.bjfxy.top

[R55] 压缩与解压
来源：http://xgu.cqqwz.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ofr.316326.xyz

[R56] 远程拷贝
来源：http://okj.yfazqb.com

scp file user@host:/path/
来源：http://vzp.chenzaomai.com

[R57] 远程执行命令
来源：http://trq.fktsv.cn

ssh user@host 'uptime'
来源：http://kbi.wangshuangyany.cn

[R58] 下载文件
来源：http://xid.ehwqpu.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zhq.zhaomingkeji.xyz

[R59] 发 POST JSON
来源：http://vbj.hesvh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://daj.redwolf501.top

[R60] 只看 HTTP 状态码
来源：http://slq.jianghu66.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pen.yfazqb.com

[R61] 磁盘占用
来源：http://yej.cqqwz.cn

df -h;  du -sh *
来源：http://gtu.dashuyun.cn

[R62] 找最占空间的文件
来源：http://cqk.yfazqb.com

du -ah . | sort -rh | head -10
来源：http://vef.meibo888.top

[R63] 内存与进程
来源：http://sax.dashuyun.cn

free -h;  ps aux | grep nginx
来源：http://zxq.feifeiyinyue.top

[R64] 结束进程
来源：http://imi.c1oappe.top

kill -9 $(pgrep -f app.py)
来源：http://wfi.cashguo.top

[R65] 查看端口占用
来源：http://qzo.dashuyun.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jqj.wangdashe.top

[R66] 定时任务
来源：http://mcm.zhiwuduotai.top

crontab -e;  crontab -l
来源：http://dwd.sjlbkw.cn

[R67] 生成随机十六进制串
来源：http://wlz.sysykeji.top

openssl rand -hex 16
来源：http://mut.yvedp.cn

[R68] 计算文件校验值
来源：http://lil.fanxiaobao.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://etu.zdqjudy.top

[R69] 生成随机密码
来源：http://pha.zhiwuduotai.top

head -c 16 /dev/urandom | base64
来源：http://sak.wangshuangyany.cn

[R70] 时间戳与互转
来源：http://czl.daria6918.cn

date +%s;  date -d @1700000000
来源：http://fuz.sysykeji.top

[R71] 日期格式化
来源：http://wok.cucudq.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://alo.hongshengwenyu.top

[R72] 等待端口就绪
来源：http://kdo.tanke756.top

until nc -z localhost 3306; do sleep 1; done
来源：http://kfs.zhengqikj.top

[R73] 分割大日志
来源：http://zfa.meibo888.top

split -l 1000 big.log part_
来源：http://amy.yj20258.top

[R74] 批量重命名
来源：http://wxi.yuanzhike.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xtp.ppjwa.cn

[R75] 导出环境变量
来源：http://ydg.havefunace.top

export PATH="$HOME/bin:$PATH"
来源：http://flf.chenlongwang.top

[R76] 使用临时文件
来源：http://gra.tianlin.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yrv.vqdsnc.cn

[R77] 读取用户输入
来源：http://iqa.smart0.xyz

read -rp "请输入: " ans
来源：http://bek.guannengcc.top

[R78] 交互式菜单
来源：http://dde.wangdashe.top

select opt in a b c; do echo "$opt"; break; done
来源：http://vlb.0kj1m.cn

[R79] 解析命令行选项
来源：http://yfv.yongpay.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ivn.mhx1999.top

[R80] 查看脚本执行耗时
来源：http://aks.pycfn.com

time ./run.sh
来源：http://cim.dianchejie.cn

================================================================================
来源：http://tdj.ctjpmb.com

S. C / C++ 专题
来源：http://ptp.hnxiangtu.top

================================================================================
来源：http://hkk.nanxinkj.top

[S01] C：Hello World
来源：http://yeg.andypj.xyz

#include <stdio.h>
来源：http://sdy.ppjwa.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://exn.fengsongda.top

[S02] C：变量与格式化输出
来源：http://emv.zhongyouzk.top

int a = 10; printf("%d\n", a);
来源：http://ial.hnqzz.top

[S03] C：读入整数
来源：http://aoo.0kj1m.cn

int x; scanf("%d", &x);
来源：http://vvm.wangdashe.top

[S04] C：字符串复制
来源：http://zzk.hysaishi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://eaf.jlsjyb.cn

[S05] C：字符串长度
来源：http://vth.bbcook.cn

strlen(s)
来源：http://rhw.tarul.cn

[S06] C：字符串比较
来源：http://nud.jqgufenzy.top

strcmp(a, b) == 0
来源：http://clq.jiagoushi.top

[S07] C：数组遍历求和
来源：http://qsq.fehbvm.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pdp.hysaishi.cn

[S08] C：动态内存分配与释放
来源：http://cpr.meibo888.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ovq.andypj.xyz

[S09] C：结构体定义与初始化
来源：http://vfs.52xcode.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://oic.fengsongda.top

[S10] C：指针与解引用
来源：http://djz.hesvh.cn

int *p = &a;  *p = 5;
来源：http://qcf.hfpthk.cn

[S11] C：逐行读文件
来源：http://sam.xuanzx.com

FILE *f = fopen("a.txt", "r");
来源：http://cmo.uphjek.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://jlw.gaohongyu789.top

fclose(f);
来源：http://reu.hcnkem.com

[S12] C：写文件
来源：http://kjz.kuanghao11.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ywn.jqgfzy.top

[S13] C：宏定义
来源：http://zas.daxiang520.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wne.meibo888.top

[S14] C：枚举
来源：http://lar.guowangkeji.top

enum Color { RED, GREEN, BLUE };
来源：http://qsu.sweek.top

[S15] C：类型转换
来源：http://zui.zhoulong.xyz

(double) a / b
来源：http://abb.hcnkem.com

[S16] C：位操作置位
来源：http://mca.c1oappe.top

x |= (1 << 3);
来源：http://ayi.jinqigfzy.top

[S17] C：安全拼接字符串
来源：http://bdb.hfpthk.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rym.havefunace.top

[S18] C：命令行参数
来源：http://jjz.gaohongyu789.top

int main(int argc, char **argv)
来源：http://fau.svipenyu.cn

[S19] C：快速排序
来源：http://xqy.jqgfzy.top

qsort(a, n, sizeof(int), cmp);
来源：http://coz.gogol.net.cn

[S20] C：二分查找
来源：http://vzr.jinqigufen.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://iwp.zhongyouzk.top

[S21] C：字符类别判断
来源：http://ejp.daria6918.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jnq.sufxvd.cn

[S22] C：字符串转数字
来源：http://eti.gotoacloud.top

atoi("42");  strtod("3.14", NULL);
来源：http://bmw.xylfe.cn

[S23] C：随机数
来源：http://okt.sweek.top

srand(time(NULL));  int r = rand() % 100;
来源：http://goh.hywenlv.cn

[S24] C：获取本地时间
来源：http://dez.jqgfzy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ehl.hnqzz.top

[S25] C：内存拷贝
来源：http://bym.hysaishi.cn

memcpy(dst, src, n);
来源：http://hpa.hesvh.cn

[S26] C：内存清零
来源：http://veo.quarkkingdee.top

memset(a, 0, sizeof a);
来源：http://qvj.jqgfzy.top

[S27] C：定义常量
来源：http://hwa.jianghu66.top

const double PI = 3.14159;
来源：http://geo.zdqjudy.top

[S28] C：静态变量
来源：http://skk.yonumen.top

static int counter = 0;
来源：http://pqt.jqgufenzy.top

[S29] C：变参函数
来源：http://fds.hnqzz.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sbv.guowangkeji.top

[S30] C：头文件保护
来源：http://fnx.cucudq.cn

#ifndef X_H
来源：http://ogf.tarul.cn

#define X_H
来源：http://srk.ywan-chungtsiang.top

#endif
来源：http://zae.uphjek.com

[S31] C++：Hello World
来源：http://gqj.aibaodan.cn

#include <iostream>
来源：http://oak.sweek.top

int main() { std::cout << "Hello\n"; }
来源：http://xyp.sufxvd.cn

[S32] C++：字符串
来源：http://dbv.shangyingyoupin.top

std::string s = "hi";  s += "!";
来源：http://wam.aibaodan.cn

[S33] C++：vector 增删
来源：http://eeq.fanxiaobao.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gvt.yuxming.cn

[S34] C++：遍历 vector
来源：http://mcq.wangshuangyany.cn

for (auto &x : v) { std::cout << x; }
来源：http://omk.sxryk.cn

[S35] C++：map
来源：http://fgg.nwbrower.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ira.quarkkingdee.top

[S36] C++：unordered_map
来源：http://kek.redwolf501.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ejq.feifeiyinyue.top

[S37] C++：set
来源：http://kwr.jinqigufen.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zpe.mhx1999.top

[S38] C++：排序
来源：http://exf.zycfv.cn

std::sort(v.begin(), v.end());
来源：http://unc.0kj1m.cn

[S39] C++：自定义比较器排序
来源：http://sui.gzhubu.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nce.dashuyun.cn

[S40] C++：查找元素
来源：http://zpj.nwbrower.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://htw.tianlin.xyz

[S41] C++：类与构造函数
来源：http://fjt.ydjk.org.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kpa.havefunace.top

[S42] C++：继承与虚函数
来源：http://rvz.haohaochexian.top

class B : public Base { public: void f() override {} };
来源：http://qct.smart0.xyz

[S43] C++：智能指针
来源：http://fjg.birdmap.top

auto p = std::make_unique<int>(5);
来源：http://haj.vehdjk.com

[S44] C++：引用传参
来源：http://hpb.tanke756.top

void inc(int &x) { ++x; }
来源：http://fwb.xuetiantiany.cn

[S45] C++：lambda
来源：http://muw.sysykeji.top

auto add = [](int a, int b) { return a + b; };
来源：http://zph.gotoacloud.top

[S46] C++：函数模板
来源：http://voq.zhengqikj.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mle.iojbl.cn

[S47] C++：结构化绑定遍历
来源：http://xjf.hnqzz.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tzl.yvedp.cn

[S48] C++：逐行读文件
来源：http://swo.yanxiufei.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jpy.cucudq.cn

while (std::getline(in, line)) { }
来源：http://uan.nanxinkj.top

[S49] C++：写文件
来源：http://yev.mhx1999.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hbk.nanxinkj.top

[S50] C++：格式化数字
来源：http://gyo.jqgufenzy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jgj.fanxiaobao.xyz

[S51] C++：显式类型转换
来源：http://odm.zhongyouzk.top

static_cast<double>(a) / b
来源：http://lrk.yuanzhike.top

[S52] C++：const 与 noexcept
来源：http://nlz.bjfxy.top

int size() const noexcept { return n_; }
来源：http://xfu.haohaochexian.top

[S53] C++：移动语义
来源：http://ods.cashguo.top

std::vector<int> w = std::move(v);
来源：http://rpv.jqgfzy.top

[S54] C++：异常处理
来源：http://nky.guowangkeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://meu.chenlongwang.top

[S55] C++：结构化绑定
来源：http://owl.smart0.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://ndh.fanxiaobao.xyz

[S56] C++：optional
来源：http://oxz.jinyuanbaomall.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ziz.nwbrower.top

[S57] C++：编译期常量
来源：http://pvx.jlsjyb.cn

constexpr int N = 10;
来源：http://lpt.birdmap.top

[S58] C++：命名空间
来源：http://jth.ydzc1.top

namespace ns { int f() { return 1; } }
来源：http://zxs.yj202588.top

[S59] C++：静态断言
来源：http://cjd.quarkkingdee.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jbr.svipenyu.cn

[S60] C++：遍历并删除元素
来源：http://xiq.aizwys.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fcq.epnwcf.com

================================================================================
来源：http://dmj.jyoumei.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://amm.birdmap.top

================================================================================
来源：http://hat.jlsjyb.cn

[T01] Kotlin：Hello World
来源：http://pui.hesvh.cn

println("Hello")
来源：http://mdn.52xcode.cn

[T02] Kotlin：变量
来源：http://vly.yanxiufei.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zcc.yfazqb.com

[T03] Kotlin：字符串模板
来源：http://ehx.hnqzz.top

"值: $b"
来源：http://rzy.xuetiantiany.cn

[T04] Kotlin：空安全
来源：http://wxo.chenzaomai.com

val n: String? = null;  n?.length
来源：http://dsh.ydjk.org.cn

[T05] Kotlin：when 表达式
来源：http://neh.tian-w.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ybr.havefunace.top

[T06] Kotlin：集合映射
来源：http://agy.hongshengwenyu.top

listOf(1, 2, 3).map { it * 2 }
来源：http://dus.yj202588.top

[T07] Kotlin：集合过滤
来源：http://hsr.wangshuangyany.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://rsz.daria6918.cn

[T08] Kotlin：数据类
来源：http://iqc.jyoumei.cn

data class User(val name: String, val age: Int)
来源：http://uhb.zdbjq.cn

[T09] Kotlin：扩展函数
来源：http://ker.chenlongwang.top

fun String.exclaim() = this + "!"
来源：http://yxw.xziqi.cn

[T10] Kotlin：默认参数
来源：http://trn.hywenlv.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ywc.aibaodan.cn

[T11] Kotlin：协程
来源：http://gsf.jinghuilouyu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://atm.gogol.net.cn

[T12] Kotlin：解构声明
来源：http://jhd.guowangkeji.top

val (a, b) = Pair(1, 2)
来源：http://zhh.gogol.net.cn

[T13] Kotlin：只读 Map
来源：http://qkt.gogol.net.cn

val m = mapOf("a" to 1)
来源：http://vgg.jianghu66.top

[T14] Kotlin：循环
来源：http://zfn.hnqzz.top

for (i in 1..10) println(i)
来源：http://zro.hnqzz.top

[T15] Kotlin：接口
来源：http://mvq.c1oappe.top

interface Shape { fun area(): Double }
来源：http://tll.epnwcf.com

[T16] Swift：Hello World
来源：http://gnz.bbcook.cn

print("Hello")
来源：http://xok.ppjwa.cn

[T17] Swift：变量与常量
来源：http://lnl.ybcxt.top

var a = 1;  let b = 2
来源：http://clm.sysykeji.top

[T18] Swift：字符串插值
来源：http://ule.aizwys.cn

"值: \(b)"
来源：http://swh.daria6918.cn

[T19] Swift：可选绑定
来源：http://gfs.cqqwz.cn

if let n = opt { print(n) }
来源：http://xde.tanke756.top

[T20] Swift：数组操作
来源：http://smr.sjlbkw.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jve.yuxming.cn

[T21] Swift：遍历
来源：http://dkv.sxryk.cn

for x in a { print(x) }
来源：http://csq.iojbl.cn

[T22] Swift：字典
来源：http://gmm.jqgfzy.top

var d = ["a": 1];  d["b"] = 2
来源：http://qxs.tian-w.cn

[T23] Swift：函数
来源：http://jst.feifeiyinyue.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zje.xziqi.cn

[T24] Swift：闭包
来源：http://pyz.yangfankeji.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://sjq.ywan-chungtsiang.top

[T25] Swift：结构体
来源：http://hae.c1oappe.top

struct P { var x: Int }
来源：http://nae.316326.xyz

[T26] Swift：类与重写
来源：http://qrg.ydzc1.top

class A: Base { override func f() {} }
来源：http://xlq.gogol.net.cn

[T27] Swift：错误处理
来源：http://bbn.hywenlv.cn

do { try f() } catch { print(error) }
来源：http://squ.dianchejie.cn

[T28] Swift：枚举
来源：http://dxj.zdqjudy.top

enum Color { case red, green }
来源：http://iyq.aibaodan.cn

[T29] Swift：guard 提前返回
来源：http://yjy.yueranfly.top

guard let x = opt else { return }
来源：http://kav.fengsongda.top

[T30] Swift：协议
来源：http://llq.tanke756.top

protocol Shape { func area() -> Double }
来源：http://mkq.hammf.cn

[T31] Lua：Hello World
来源：http://buw.snrcjt.cn

print("Hello")
来源：http://dvc.tianlin.xyz

[T32] Lua：局部变量
来源：http://ssp.gotoacloud.top

local a = 1
来源：http://mau.shuidangran.top


<!-- 参考信息 -->