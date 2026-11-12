代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xyu.yuanzhike.top

[R30] 函数返回状态码
来源：http://nwt.gotoacloud.top

f() { return 0; }; f || echo "失败了"
来源：http://twx.yj20258.top

[R31] 局部变量
来源：http://piy.pycfn.com

f() { local x=1; echo "$x"; }
来源：http://koq.guowangkeji.top

[R32] 参数个数校验
来源：http://vwo.haohaochexian.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://llv.uphjek.com

[R33] 捕获错误并提示行号
来源：http://yaj.jqgfzy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qkd.jianghu66.top

[R34] 退出时清理
来源：http://chl.ybcxt.top

trap 'rm -f "$tmp"' EXIT
来源：http://tes.quarkkingdee.top

[R35] 后台执行并等待
来源：http://vrx.ppjwa.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://wnf.jinqigufen.top

[R36] 并发执行多个任务
来源：http://gxu.birdmap.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rhz.zhixingplan.top

[R37] 把输出赋给变量
来源：http://zez.jqgfzy.top

files=$(ls -1)
来源：http://orx.ivvv.top

[R38] 管道串联
来源：http://rkx.haohaochexian.top

cat a.txt | grep -i error | wc -l
来源：http://pol.daxiang520.top

[R39] 重定向标准输出与错误
来源：http://npc.chenzaomai.com

cmd > out.log 2>&1
来源：http://ejz.fanxiaobao.xyz

[R40] 追加写日志
来源：http://jgu.pycfn.com

echo "log" >> out.log
来源：http://ljn.zdqjudy.top

[R41] 丢弃输出
来源：http://ddl.fzhhl.top

cmd >/dev/null 2>&1
来源：http://fbp.zhongyouzk.top

[R42] 输入重定向
来源：http://oyx.jyoumei.cn

wc -l < a.txt
来源：http://hvd.yongpay.top

[R43] 按名字查找文件
来源：http://bkh.yangfankeji.com

find . -name "*.log" -type f
来源：http://ifu.pengpengdd.cyou

[R44] 按修改时间查找
来源：http://ynb.yonumen.top

find . -mtime -7 -type f
来源：http://ubs.hnxiangtu.top

[R45] 批量删除
来源：http://xwa.hammf.cn

find . -name "*.tmp" -delete
来源：http://tua.meibo888.top

[R46] 递归替换文件内容
来源：http://fit.cdnleiting.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hyy.tarul.cn

[R47] sed 单行替换
来源：http://nyq.shangyingyoupin.top

sed -i 's/foo/bar/g' a.txt
来源：http://pov.zhiwuduotai.top

[R48] awk 取指定列
来源：http://evp.jiagoushi.top

awk '{print $1, $3}' a.txt
来源：http://azn.yonumen.top

[R49] awk 带条件
来源：http://nau.jiagoushi.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zsp.cucudq.cn

[R50] awk 求和
来源：http://gcq.fengsongda.top

awk '{s += $2} END {print s}' a.txt
来源：http://dpq.sjlbkw.cn

[R51] 排序去重取前几
来源：http://sdn.tarul.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://jic.feifeiyinyue.top

[R52] 统计行数
来源：http://zmb.hongshengwenyu.top

wc -l a.txt
来源：http://dlx.yonumen.top

[R53] 查看文件头与实时尾
来源：http://joj.kuanghao11.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://joy.yongpay.top

[R54] 比较两个文件
来源：http://pbh.ppjwa.cn

diff a.txt b.txt
来源：http://jgg.yj20258.top

[R55] 压缩与解压
来源：http://fcu.jyoumei.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ulm.hysaishi.cn

[R56] 远程拷贝
来源：http://xaj.jinghuilouyu.cn

scp file user@host:/path/
来源：http://hzx.sweek.top

[R57] 远程执行命令
来源：http://owc.zhoulong.xyz

ssh user@host 'uptime'
来源：http://eyp.yvedp.cn

[R58] 下载文件
来源：http://dsm.zhiwuduotai.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ifm.bjfxy.top

[R59] 发 POST JSON
来源：http://chs.fktsv.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rwk.nanxuanxn.top

[R60] 只看 HTTP 状态码
来源：http://xcu.cashguo.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mud.fengsongda.top

[R61] 磁盘占用
来源：http://lcm.quarkkingdee.top

df -h;  du -sh *
来源：http://gkb.daxiang520.top

[R62] 找最占空间的文件
来源：http://nxq.dianchejie.cn

du -ah . | sort -rh | head -10
来源：http://thl.9152youxi.cn

[R63] 内存与进程
来源：http://bvr.zhiwuduotai.top

free -h;  ps aux | grep nginx
来源：http://jnd.bbcook.cn

[R64] 结束进程
来源：http://pqq.shanyushiyangkeji.top

kill -9 $(pgrep -f app.py)
来源：http://eli.ctjpmb.com

[R65] 查看端口占用
来源：http://tnj.daxiang520.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ovu.hywenlv.cn

[R66] 定时任务
来源：http://jfe.sweek.top

crontab -e;  crontab -l
来源：http://byf.yj20258.top

[R67] 生成随机十六进制串
来源：http://utw.cheryme.top

openssl rand -hex 16
来源：http://dbh.sjlbkw.cn

[R68] 计算文件校验值
来源：http://sfv.fehbvm.com

sha256sum a.txt;  md5sum a.txt
来源：http://wci.havefunace.top

[R69] 生成随机密码
来源：http://zdl.daria6918.cn

head -c 16 /dev/urandom | base64
来源：http://ash.nwbrower.top

[R70] 时间戳与互转
来源：http://ggk.zycfv.cn

date +%s;  date -d @1700000000
来源：http://nrc.yuanzhike.top

[R71] 日期格式化
来源：http://nfx.shanyushiyangtech.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://bga.hesvh.cn

[R72] 等待端口就绪
来源：http://iqt.birdmap.top

until nc -z localhost 3306; do sleep 1; done
来源：http://uqt.zdqjudy.top

[R73] 分割大日志
来源：http://hwx.havefunace.top

split -l 1000 big.log part_
来源：http://alw.shuidangran.top

[R74] 批量重命名
来源：http://pcn.yfazqb.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://okw.havefunace.top

[R75] 导出环境变量
来源：http://wjs.zhijiandao.cn

export PATH="$HOME/bin:$PATH"
来源：http://ynz.gotoacloud.top

[R76] 使用临时文件
来源：http://hmi.redwolf501.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://oay.yj20258888.top

[R77] 读取用户输入
来源：http://tlt.dashuyun.cn

read -rp "请输入: " ans
来源：http://mls.0kj1m.cn

[R78] 交互式菜单
来源：http://xsz.hongshengwenyu.top

select opt in a b c; do echo "$opt"; break; done
来源：http://vgw.zhaomingkeji.xyz

[R79] 解析命令行选项
来源：http://zox.cqqwz.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wsh.fengsongda.top

[R80] 查看脚本执行耗时
来源：http://nej.hesvh.cn

time ./run.sh
来源：http://mlr.epnwcf.com

================================================================================
来源：http://vxz.gaohongyu789.top

S. C / C++ 专题
来源：http://lbc.sweek.top

================================================================================
来源：http://usg.cucudq.cn

[S01] C：Hello World
来源：http://qoa.birdmap.top

#include <stdio.h>
来源：http://ixr.shangyingyoupin.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://wgr.jyoumei.cn

[S02] C：变量与格式化输出
来源：http://gjp.xinyue.icu

int a = 10; printf("%d\n", a);
来源：http://hjk.yuanzhike.top

[S03] C：读入整数
来源：http://rfp.guannengcc.top

int x; scanf("%d", &x);
来源：http://mrd.andypj.xyz

[S04] C：字符串复制
来源：http://ygb.wangdashe.top

char dst[32]; strcpy(dst, "hi");
来源：http://gsw.meibo888.top

[S05] C：字符串长度
来源：http://nxn.jinqigfzy.top

strlen(s)
来源：http://wyq.xinyue.icu

[S06] C：字符串比较
来源：http://egy.zhijiandao.cn

strcmp(a, b) == 0
来源：http://zfo.jiagoushi.top

[S07] C：数组遍历求和
来源：http://mrl.xuanzx.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://msx.tarul.cn

[S08] C：动态内存分配与释放
来源：http://yqs.smart0.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tbf.chenzaomai.com

[S09] C：结构体定义与初始化
来源：http://apw.yj20258.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dvk.sjlbkw.cn

[S10] C：指针与解引用
来源：http://wwq.nanxuanxn.top

int *p = &a;  *p = 5;
来源：http://era.hcnkem.com

[S11] C：逐行读文件
来源：http://qdt.ivvv.top

FILE *f = fopen("a.txt", "r");
来源：http://tez.pengpengdd.cyou

while (fgets(buf, sizeof buf, f)) { }
来源：http://dvn.9152youxi.cn

fclose(f);
来源：http://lrc.9152youxi.cn

[S12] C：写文件
来源：http://pqi.yj202588.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://czu.sweek.top

[S13] C：宏定义
来源：http://wgd.vehdjk.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kpd.zhiwuduotai.top

[S14] C：枚举
来源：http://uhv.shangyingyoupin.top

enum Color { RED, GREEN, BLUE };
来源：http://dyo.sweek.top

[S15] C：类型转换
来源：http://mhp.shanyushiyangkeji.top

(double) a / b
来源：http://xqk.meibo888.top

[S16] C：位操作置位
来源：http://gcd.zhoulong.xyz

x |= (1 << 3);
来源：http://ffq.ctjpmb.com

[S17] C：安全拼接字符串
来源：http://hll.andypj.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bal.hysaishi.cn

[S18] C：命令行参数
来源：http://ryq.yj202588.top

int main(int argc, char **argv)
来源：http://hgy.nwbrower.top

[S19] C：快速排序
来源：http://rqo.daria6918.cn

qsort(a, n, sizeof(int), cmp);
来源：http://hzf.epnwcf.com

[S20] C：二分查找
来源：http://qsh.snrcjt.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://inl.316326.xyz

[S21] C：字符类别判断
来源：http://vmy.ybcxt.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qrn.aibaodan.cn

[S22] C：字符串转数字
来源：http://zaj.yanxiufei.cn

atoi("42");  strtod("3.14", NULL);
来源：http://gnl.nanxinkj.top

[S23] C：随机数
来源：http://epb.zhoulong.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://ftf.yuanzhike.top

[S24] C：获取本地时间
来源：http://nip.yuxming.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tcn.jinyuanbaomall.cn

[S25] C：内存拷贝
来源：http://tud.zhongyouzk.top

memcpy(dst, src, n);
来源：http://daq.fehbvm.com

[S26] C：内存清零
来源：http://pya.havefunace.top

memset(a, 0, sizeof a);
来源：http://qjp.yj202588.top

[S27] C：定义常量
来源：http://fzf.hnxiangtu.top

const double PI = 3.14159;
来源：http://umi.wangdashe.top

[S28] C：静态变量
来源：http://vaj.hesvh.cn

static int counter = 0;
来源：http://bwm.c1oappe.top

[S29] C：变参函数
来源：http://tot.ppjwa.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://eav.zhongyouzk.top

[S30] C：头文件保护
来源：http://vih.jqgfzy.top

#ifndef X_H
来源：http://hto.snrcjt.cn

#define X_H
来源：http://skd.havefunace.top

#endif
来源：http://mub.gzhubu.top

[S31] C++：Hello World
来源：http://phy.tianlin.xyz

#include <iostream>
来源：http://kjt.jyoumei.cn

int main() { std::cout << "Hello\n"; }
来源：http://usb.zhijiandao.cn

[S32] C++：字符串
来源：http://kwp.fehbvm.com

std::string s = "hi";  s += "!";
来源：http://ssh.xuanzx.com

[S33] C++：vector 增删
来源：http://lsa.yuxming.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hot.nanxuanxn.top

[S34] C++：遍历 vector
来源：http://nxz.cdnleiting.top

for (auto &x : v) { std::cout << x; }
来源：http://owx.havefunace.top

[S35] C++：map
来源：http://lho.tanke756.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://uxq.shanyushiyangkeji.top

[S36] C++：unordered_map
来源：http://gfk.9152youxi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rzq.chenzaomai.com

[S37] C++：set
来源：http://nkt.jinqigufen.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://see.jiagoushi.top

[S38] C++：排序
来源：http://sub.fzhhl.top

std::sort(v.begin(), v.end());
来源：http://eqf.shangyingyoupin.top

[S39] C++：自定义比较器排序
来源：http://wnb.hysaishi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wch.tanke756.top

[S40] C++：查找元素
来源：http://ygf.tanke756.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kvz.hnqzz.top

[S41] C++：类与构造函数
来源：http://ndw.ywan-chungtsiang.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gfc.c1oappe.top

[S42] C++：继承与虚函数
来源：http://vec.daxiang520.top

class B : public Base { public: void f() override {} };
来源：http://rzg.mhx1999.top

[S43] C++：智能指针
来源：http://nyq.jinghuilouyu.cn

auto p = std::make_unique<int>(5);
来源：http://acd.daria6918.cn

[S44] C++：引用传参
来源：http://fsi.haohaochexian.top

void inc(int &x) { ++x; }
来源：http://iwp.pengpengdd.cyou

[S45] C++：lambda
来源：http://dak.sufxvd.cn

auto add = [](int a, int b) { return a + b; };
来源：http://olz.guowangkeji.top

[S46] C++：函数模板
来源：http://brh.pycfn.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lvh.zhoulong.xyz

[S47] C++：结构化绑定遍历
来源：http://ite.cheryme.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qyw.pengpengdd.cyou

[S48] C++：逐行读文件
来源：http://xkx.gogol.net.cn

std::ifstream in("a.txt");  std::string line;
来源：http://mwo.smart0.xyz

while (std::getline(in, line)) { }
来源：http://uiu.sxryk.cn

[S49] C++：写文件
来源：http://rgb.9152youxi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yrt.hammf.cn

[S50] C++：格式化数字
来源：http://zea.sweek.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wdf.ywan-chungtsiang.top

[S51] C++：显式类型转换
来源：http://tvk.meibo888.top

static_cast<double>(a) / b
来源：http://jus.haohaochexian.top

[S52] C++：const 与 noexcept
来源：http://qbq.zhixingplan.top

int size() const noexcept { return n_; }
来源：http://guq.fktsv.cn

[S53] C++：移动语义
来源：http://law.zhoulong.xyz

std::vector<int> w = std::move(v);
来源：http://lia.yongpay.top

[S54] C++：异常处理
来源：http://hit.hongshengwenyu.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://oss.yueranfly.top

[S55] C++：结构化绑定
来源：http://eah.tian-w.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rux.haohaochexian.top

[S56] C++：optional
来源：http://pvo.fehbvm.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://oie.quarkkingdee.top

[S57] C++：编译期常量
来源：http://ipd.gogol.net.cn

constexpr int N = 10;
来源：http://yzx.shzxlz.cn

[S58] C++：命名空间
来源：http://ind.52xcode.cn

namespace ns { int f() { return 1; } }
来源：http://wdq.0kj1m.cn

[S59] C++：静态断言
来源：http://cwe.dianchejie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kep.ivvv.top

[S60] C++：遍历并删除元素
来源：http://awb.hysaishi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tev.feifeiyinyue.top

================================================================================
来源：http://ibu.hfpthk.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vpv.gotoacloud.top

================================================================================
来源：http://vpu.pengpengdd.cyou

[T01] Kotlin：Hello World
来源：http://upx.birdmap.top

println("Hello")
来源：http://ufk.uphjek.com

[T02] Kotlin：变量
来源：http://rja.hnqzz.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qlj.yj20258.top

[T03] Kotlin：字符串模板
来源：http://gqp.yueranfly.top

"值: $b"
来源：http://jcw.zycfv.cn

[T04] Kotlin：空安全
来源：http://iwk.ppjwa.cn

val n: String? = null;  n?.length
来源：http://pqc.cucudq.cn

[T05] Kotlin：when 表达式
来源：http://wvu.jinghuilouyu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vjt.zycfv.cn

[T06] Kotlin：集合映射
来源：http://tfk.yuxming.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://huq.yj20258.top

[T07] Kotlin：集合过滤
来源：http://ubk.shuidangran.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://skz.tianlin.xyz

[T08] Kotlin：数据类
来源：http://uqo.zhixingplan.top

data class User(val name: String, val age: Int)
来源：http://dsk.xuanzx.com

[T09] Kotlin：扩展函数
来源：http://qpz.vehdjk.com

fun String.exclaim() = this + "!"
来源：http://ehy.kuanghao11.cn

[T10] Kotlin：默认参数
来源：http://rhl.fengsongda.top

fun greet(name: String = "World") = "Hi $name"
来源：http://dtj.meibo888.top

[T11] Kotlin：协程
来源：http://fcg.yanxiufei.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://sra.xylfe.cn

[T12] Kotlin：解构声明
来源：http://mfe.ivvv.top

val (a, b) = Pair(1, 2)
来源：http://nhv.9152youxi.cn

[T13] Kotlin：只读 Map
来源：http://eqp.gzhubu.top

val m = mapOf("a" to 1)
来源：http://lxn.gzhubu.top

[T14] Kotlin：循环
来源：http://ehi.sysykeji.top

for (i in 1..10) println(i)
来源：http://the.shanyushiyangkeji.top

[T15] Kotlin：接口
来源：http://yxv.zycfv.cn

interface Shape { fun area(): Double }
来源：http://nwh.nanxuanxn.top

[T16] Swift：Hello World
来源：http://upd.cheryme.top

print("Hello")
来源：http://mcr.havefunace.top

[T17] Swift：变量与常量
来源：http://jce.sufxvd.cn

var a = 1;  let b = 2
来源：http://rsx.hnqzz.top

[T18] Swift：字符串插值
来源：http://kah.tianlin.xyz

"值: \(b)"
来源：http://adw.xuanzx.com

[T19] Swift：可选绑定
来源：http://lbv.yj202588.top

if let n = opt { print(n) }
来源：http://dps.shanyushiyangtech.top

[T20] Swift：数组操作
来源：http://tba.pengpengdd.cyou

var a = [1, 2, 3];  a.append(4)
来源：http://hqr.jinghuilouyu.cn

[T21] Swift：遍历
来源：http://wlt.yj20258888.top

for x in a { print(x) }
来源：http://ott.sjlbkw.cn

[T22] Swift：字典
来源：http://mth.shangyingyoupin.top

var d = ["a": 1];  d["b"] = 2
来源：http://hoo.snrcjt.cn

[T23] Swift：函数
来源：http://brt.yuanzhike.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xdc.yuanzhike.top

[T24] Swift：闭包
来源：http://cuk.hfpthk.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://afc.shangyingyoupin.top

[T25] Swift：结构体
来源：http://kqa.ywan-chungtsiang.top

struct P { var x: Int }
来源：http://aam.guannengcc.top

[T26] Swift：类与重写
来源：http://kmn.jinghuilouyu.cn

class A: Base { override func f() {} }
来源：http://hsw.chenzaomai.com

[T27] Swift：错误处理
来源：http://ili.tarul.cn

do { try f() } catch { print(error) }
来源：http://kld.kuanghao11.cn

[T28] Swift：枚举
来源：http://wey.fehbvm.com

enum Color { case red, green }
来源：http://fqn.tian-w.cn

[T29] Swift：guard 提前返回
来源：http://ukf.hfpthk.cn

guard let x = opt else { return }
来源：http://eqn.mhx1999.top

[T30] Swift：协议
来源：http://zdr.shanyushiyangtech.top

protocol Shape { func area() -> Double }
来源：http://sin.tianlin.xyz

[T31] Lua：Hello World
来源：http://kum.pycfn.com

print("Hello")
来源：http://arx.yonumen.top

[T32] Lua：局部变量
来源：http://qrf.shzxlz.cn

local a = 1
来源：http://zcr.sxryk.cn


<!-- 参考信息 -->