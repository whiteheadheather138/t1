代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://diy.xuanzx.com

[R24] 大小写转换
来源：http://kec.tarul.cn

echo "${s^^}"; echo "${s,,}"
来源：http://jmg.feifeiyinyue.top

[R25] 去后缀 / 去前缀
来源：http://daa.sysykeji.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ipr.yuanzhike.top

[R26] 命令替换
来源：http://cgq.dashuyun.cn

now=$(date +%F); echo "$now"
来源：http://cra.bbcook.cn

[R27] 算术展开
来源：http://fdb.yfazqb.com

echo $((1 + 2 * 3))
来源：http://dkb.316326.xyz

[R28] 浮点运算
来源：http://bnd.hnqzz.top

echo "scale=2; 10/3" | bc
来源：http://grx.tanke756.top

[R29] 定义函数
来源：http://ddl.tanke756.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qkd.shuidangran.top

[R30] 函数返回状态码
来源：http://lhd.yj20258.top

f() { return 0; }; f || echo "失败了"
来源：http://wlw.snrcjt.cn

[R31] 局部变量
来源：http://zed.nwbrower.top

f() { local x=1; echo "$x"; }
来源：http://vqi.daxiang520.top

[R32] 参数个数校验
来源：http://cmi.tianlin.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ubf.chenjidiqi.icu

[R33] 捕获错误并提示行号
来源：http://xyd.ivvv.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vau.zdbjq.cn

[R34] 退出时清理
来源：http://cfq.jianghu66.top

trap 'rm -f "$tmp"' EXIT
来源：http://lsg.meibo888.top

[R35] 后台执行并等待
来源：http://xta.zhijiandao.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://wkf.bbcook.cn

[R36] 并发执行多个任务
来源：http://khr.jinyuanbaomall.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pqw.jyoumei.cn

[R37] 把输出赋给变量
来源：http://hds.jiagoushi.top

files=$(ls -1)
来源：http://cue.52xcode.cn

[R38] 管道串联
来源：http://knc.birdmap.top

cat a.txt | grep -i error | wc -l
来源：http://qrm.c1oappe.top

[R39] 重定向标准输出与错误
来源：http://lsx.sxryk.cn

cmd > out.log 2>&1
来源：http://akv.fktsv.cn

[R40] 追加写日志
来源：http://fmo.hammf.cn

echo "log" >> out.log
来源：http://npe.snrcjt.cn

[R41] 丢弃输出
来源：http://phx.ehwqpu.com

cmd >/dev/null 2>&1
来源：http://sup.zhijiandao.cn

[R42] 输入重定向
来源：http://znb.aizwys.cn

wc -l < a.txt
来源：http://ltm.jianghu66.top

[R43] 按名字查找文件
来源：http://wgs.haohaochexian.top

find . -name "*.log" -type f
来源：http://mub.dashuyun.cn

[R44] 按修改时间查找
来源：http://nac.yueranfly.top

find . -mtime -7 -type f
来源：http://lik.tian-w.cn

[R45] 批量删除
来源：http://cfx.shanyushiyangtech.top

find . -name "*.tmp" -delete
来源：http://zqi.bbcook.cn

[R46] 递归替换文件内容
来源：http://kky.ehwqpu.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lgm.zdqjudy.top

[R47] sed 单行替换
来源：http://bst.jqgufenzy.top

sed -i 's/foo/bar/g' a.txt
来源：http://asc.zhiwuduotai.top

[R48] awk 取指定列
来源：http://bse.fktsv.cn

awk '{print $1, $3}' a.txt
来源：http://zmh.cqqwz.cn

[R49] awk 带条件
来源：http://fck.jqgfzy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ztq.snrcjt.cn

[R50] awk 求和
来源：http://rsf.c1oappe.top

awk '{s += $2} END {print s}' a.txt
来源：http://dsn.fehbvm.com

[R51] 排序去重取前几
来源：http://wtr.zhongyouzk.top

sort a.txt | uniq -c | sort -rn | head
来源：http://fah.ywan-chungtsiang.top

[R52] 统计行数
来源：http://iow.hongshengwenyu.top

wc -l a.txt
来源：http://jzy.xuetiantiany.cn

[R53] 查看文件头与实时尾
来源：http://jko.chenjidiqi.icu

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vxk.hongshengwenyu.top

[R54] 比较两个文件
来源：http://jjy.ybcxt.top

diff a.txt b.txt
来源：http://fgv.dashuyun.cn

[R55] 压缩与解压
来源：http://fpj.iojbl.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dcm.xinyue.icu

[R56] 远程拷贝
来源：http://yls.xuetiantiany.cn

scp file user@host:/path/
来源：http://mtp.jinghuilouyu.cn

[R57] 远程执行命令
来源：http://bxv.zhongyouzk.top

ssh user@host 'uptime'
来源：http://kwe.chenzaomai.com

[R58] 下载文件
来源：http://zne.jinghuilouyu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://llp.fktsv.cn

[R59] 发 POST JSON
来源：http://urv.fengsongda.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xpo.jinqigufen.top

[R60] 只看 HTTP 状态码
来源：http://nco.cucudq.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fna.guowangkeji.top

[R61] 磁盘占用
来源：http://wxo.aibaodan.cn

df -h;  du -sh *
来源：http://kel.jiagoushi.top

[R62] 找最占空间的文件
来源：http://cpm.nanxinkj.top

du -ah . | sort -rh | head -10
来源：http://vtu.chenzaomai.com

[R63] 内存与进程
来源：http://pvz.cheryme.top

free -h;  ps aux | grep nginx
来源：http://trd.fehbvm.com

[R64] 结束进程
来源：http://svb.sufxvd.cn

kill -9 $(pgrep -f app.py)
来源：http://err.smart0.xyz

[R65] 查看端口占用
来源：http://ohx.fzhhl.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://oyc.xziqi.cn

[R66] 定时任务
来源：http://quh.ivvv.top

crontab -e;  crontab -l
来源：http://npp.cqqwz.cn

[R67] 生成随机十六进制串
来源：http://sds.pengpengdd.cyou

openssl rand -hex 16
来源：http://eqd.52xcode.cn

[R68] 计算文件校验值
来源：http://ebq.chenzaomai.com

sha256sum a.txt;  md5sum a.txt
来源：http://syd.cheryme.top

[R69] 生成随机密码
来源：http://vft.yueranfly.top

head -c 16 /dev/urandom | base64
来源：http://ogi.jinqigufen.top

[R70] 时间戳与互转
来源：http://ufp.nwbrower.top

date +%s;  date -d @1700000000
来源：http://gbe.jianghu66.top

[R71] 日期格式化
来源：http://pyz.hnqzz.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://eua.yueranfly.top

[R72] 等待端口就绪
来源：http://drp.guowangkeji.top

until nc -z localhost 3306; do sleep 1; done
来源：http://rcp.hesvh.cn

[R73] 分割大日志
来源：http://zwl.mhx1999.top

split -l 1000 big.log part_
来源：http://izj.sysykeji.top

[R74] 批量重命名
来源：http://wtq.zhaomingkeji.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pgg.0kj1m.cn

[R75] 导出环境变量
来源：http://hro.cdnleiting.top

export PATH="$HOME/bin:$PATH"
来源：http://ctb.aibaodan.cn

[R76] 使用临时文件
来源：http://tuy.zhiwuduotai.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rgr.yvedp.cn

[R77] 读取用户输入
来源：http://pwp.yuanzhike.top

read -rp "请输入: " ans
来源：http://hqc.52xcode.cn

[R78] 交互式菜单
来源：http://ddw.hywenlv.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ttb.ehwqpu.com

[R79] 解析命令行选项
来源：http://bnn.jinghuilouyu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ops.yj202588.top

[R80] 查看脚本执行耗时
来源：http://mye.gzhubu.top

time ./run.sh
来源：http://itw.jinqigufen.top

================================================================================
来源：http://eyi.yuxming.cn

S. C / C++ 专题
来源：http://uwd.iojbl.cn

================================================================================
来源：http://cov.sysykeji.top

[S01] C：Hello World
来源：http://bjw.sxryk.cn

#include <stdio.h>
来源：http://snm.vqdsnc.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://rjm.sweek.top

[S02] C：变量与格式化输出
来源：http://mhl.uphjek.com

int a = 10; printf("%d\n", a);
来源：http://jot.feifeiyinyue.top

[S03] C：读入整数
来源：http://bml.xuetiantiany.cn

int x; scanf("%d", &x);
来源：http://rqc.havefunace.top

[S04] C：字符串复制
来源：http://nvn.zhengqikj.top

char dst[32]; strcpy(dst, "hi");
来源：http://iht.hesvh.cn

[S05] C：字符串长度
来源：http://zzq.xziqi.cn

strlen(s)
来源：http://jzz.haohaochexian.top

[S06] C：字符串比较
来源：http://coe.xziqi.cn

strcmp(a, b) == 0
来源：http://hpf.fengsongda.top

[S07] C：数组遍历求和
来源：http://xhj.yanxiufei.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://oyo.fktsv.cn

[S08] C：动态内存分配与释放
来源：http://yhv.meibo888.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ggx.daria6918.cn

[S09] C：结构体定义与初始化
来源：http://wbo.yueranfly.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gsy.hammf.cn

[S10] C：指针与解引用
来源：http://ylp.nanxinkj.top

int *p = &a;  *p = 5;
来源：http://adg.epnwcf.com

[S11] C：逐行读文件
来源：http://xsk.hysaishi.cn

FILE *f = fopen("a.txt", "r");
来源：http://vvd.zdbjq.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://kws.tanke756.top

fclose(f);
来源：http://xhg.pycfn.com

[S12] C：写文件
来源：http://epc.andypj.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://get.jiagoushi.top

[S13] C：宏定义
来源：http://fzp.xinyue.icu

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://inm.jinghuilouyu.cn

[S14] C：枚举
来源：http://zia.hnxiangtu.top

enum Color { RED, GREEN, BLUE };
来源：http://qnw.chenzaomai.com

[S15] C：类型转换
来源：http://yga.yvedp.cn

(double) a / b
来源：http://uge.xuetiantiany.cn

[S16] C：位操作置位
来源：http://lwt.andypj.xyz

x |= (1 << 3);
来源：http://git.yongpay.top

[S17] C：安全拼接字符串
来源：http://oqh.chenzaomai.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cpb.hnxiangtu.top

[S18] C：命令行参数
来源：http://ftz.xylfe.cn

int main(int argc, char **argv)
来源：http://vvm.svipenyu.cn

[S19] C：快速排序
来源：http://slh.shangyingyoupin.top

qsort(a, n, sizeof(int), cmp);
来源：http://ieu.redwolf501.top

[S20] C：二分查找
来源：http://fja.chenjidiqi.icu

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wqt.fzhhl.top

[S21] C：字符类别判断
来源：http://mer.jiagoushi.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fpj.yj20258888.top

[S22] C：字符串转数字
来源：http://jiu.yfazqb.com

atoi("42");  strtod("3.14", NULL);
来源：http://oth.nwbrower.top

[S23] C：随机数
来源：http://gbz.hnxiangtu.top

srand(time(NULL));  int r = rand() % 100;
来源：http://okw.jinqigfzy.top

[S24] C：获取本地时间
来源：http://woe.shanyushiyangtech.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://unz.jinqigufen.top

[S25] C：内存拷贝
来源：http://iif.tianlin.xyz

memcpy(dst, src, n);
来源：http://xvn.xinyue.icu

[S26] C：内存清零
来源：http://bzt.dianchejie.cn

memset(a, 0, sizeof a);
来源：http://vyi.316326.xyz

[S27] C：定义常量
来源：http://pxm.chenlongwang.top

const double PI = 3.14159;
来源：http://kzr.cucudq.cn

[S28] C：静态变量
来源：http://zvs.shzxlz.cn

static int counter = 0;
来源：http://qwe.hcnkem.com

[S29] C：变参函数
来源：http://elt.shanyushiyangtech.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kel.mhx1999.top

[S30] C：头文件保护
来源：http://rdy.yvedp.cn

#ifndef X_H
来源：http://qoh.jinghuilouyu.cn

#define X_H
来源：http://hsq.gotoacloud.top

#endif
来源：http://rxk.zhengqikj.top

[S31] C++：Hello World
来源：http://hfq.hcnkem.com

#include <iostream>
来源：http://lxw.meibo888.top

int main() { std::cout << "Hello\n"; }
来源：http://sys.jqgufenzy.top

[S32] C++：字符串
来源：http://los.yueranfly.top

std::string s = "hi";  s += "!";
来源：http://ylb.0kj1m.cn

[S33] C++：vector 增删
来源：http://bnt.jlsjyb.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pio.dashuyun.cn

[S34] C++：遍历 vector
来源：http://zxu.ydjk.org.cn

for (auto &x : v) { std::cout << x; }
来源：http://lxu.fktsv.cn

[S35] C++：map
来源：http://rbe.316326.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tmk.wangdashe.top

[S36] C++：unordered_map
来源：http://gmi.shanyushiyangkeji.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hjz.chenlongwang.top

[S37] C++：set
来源：http://ywu.chenjidiqi.icu

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ajs.hammf.cn

[S38] C++：排序
来源：http://acj.0kj1m.cn

std::sort(v.begin(), v.end());
来源：http://ygi.c1oappe.top

[S39] C++：自定义比较器排序
来源：http://jxx.hysaishi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://emd.jinqigfzy.top

[S40] C++：查找元素
来源：http://qzr.zdbjq.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dyp.feifeiyinyue.top

[S41] C++：类与构造函数
来源：http://qpv.aibaodan.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gbm.meibo888.top

[S42] C++：继承与虚函数
来源：http://wkk.yj20258.top

class B : public Base { public: void f() override {} };
来源：http://mmi.chenlongwang.top

[S43] C++：智能指针
来源：http://qog.zdqjudy.top

auto p = std::make_unique<int>(5);
来源：http://tee.feifeiyinyue.top

[S44] C++：引用传参
来源：http://clu.shzxlz.cn

void inc(int &x) { ++x; }
来源：http://wsf.jiagoushi.top

[S45] C++：lambda
来源：http://oeb.mhx1999.top

auto add = [](int a, int b) { return a + b; };
来源：http://rwc.tian-w.cn

[S46] C++：函数模板
来源：http://mso.chenjidiqi.icu

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hol.ybcxt.top

[S47] C++：结构化绑定遍历
来源：http://dwi.hnxiangtu.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ypq.gaohongyu789.top

[S48] C++：逐行读文件
来源：http://ivp.pengpengdd.cyou

std::ifstream in("a.txt");  std::string line;
来源：http://esi.shzxlz.cn

while (std::getline(in, line)) { }
来源：http://gtq.xylfe.cn

[S49] C++：写文件
来源：http://cdc.ydjk.org.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bga.zdbjq.cn

[S50] C++：格式化数字
来源：http://xgh.shzxlz.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kni.quarkkingdee.top

[S51] C++：显式类型转换
来源：http://jql.xinyue.icu

static_cast<double>(a) / b
来源：http://bqo.cdnleiting.top

[S52] C++：const 与 noexcept
来源：http://dnr.zhaomingkeji.xyz

int size() const noexcept { return n_; }
来源：http://eur.tarul.cn

[S53] C++：移动语义
来源：http://fkj.hongshengwenyu.top

std::vector<int> w = std::move(v);
来源：http://cfr.tarul.cn

[S54] C++：异常处理
来源：http://mkr.shanyushiyangtech.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yls.yvedp.cn

[S55] C++：结构化绑定
来源：http://dxy.guannengcc.top

auto [a, b] = std::make_pair(1, 2);
来源：http://pns.uphjek.com

[S56] C++：optional
来源：http://suc.redwolf501.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gln.zhijiandao.cn

[S57] C++：编译期常量
来源：http://qrq.pengpengdd.cyou

constexpr int N = 10;
来源：http://cqd.sxryk.cn

[S58] C++：命名空间
来源：http://fdy.jinyuanbaomall.cn

namespace ns { int f() { return 1; } }
来源：http://wal.nwbrower.top

[S59] C++：静态断言
来源：http://dys.chenzaomai.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://oom.jianghu66.top

[S60] C++：遍历并删除元素
来源：http://ulm.daxiang520.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cts.shangyingyoupin.top

================================================================================
来源：http://qys.shzxlz.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://luh.chenjidiqi.icu

================================================================================
来源：http://yow.zdqjudy.top

[T01] Kotlin：Hello World
来源：http://mhb.xziqi.cn

println("Hello")
来源：http://idp.havefunace.top

[T02] Kotlin：变量
来源：http://fxo.cucudq.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wgi.zhaomingkeji.xyz

[T03] Kotlin：字符串模板
来源：http://uju.hfpthk.cn

"值: $b"
来源：http://ygq.hysaishi.cn

[T04] Kotlin：空安全
来源：http://ily.zhijiandao.cn

val n: String? = null;  n?.length
来源：http://rxa.0kj1m.cn

[T05] Kotlin：when 表达式
来源：http://xqn.zhoulong.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cbq.guowangkeji.top

[T06] Kotlin：集合映射
来源：http://kuv.xinyue.icu

listOf(1, 2, 3).map { it * 2 }
来源：http://twy.jinghuilouyu.cn

[T07] Kotlin：集合过滤
来源：http://bhk.9152youxi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://cqs.fanxiaobao.xyz

[T08] Kotlin：数据类
来源：http://sjp.yonumen.top

data class User(val name: String, val age: Int)
来源：http://dou.chenlongwang.top

[T09] Kotlin：扩展函数
来源：http://wfm.smart0.xyz

fun String.exclaim() = this + "!"
来源：http://cyu.cucudq.cn

[T10] Kotlin：默认参数
来源：http://tcl.xylfe.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://xgr.yvedp.cn

[T11] Kotlin：协程
来源：http://wkv.vehdjk.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://mzy.jqgufenzy.top

[T12] Kotlin：解构声明
来源：http://kms.yj20258888.top

val (a, b) = Pair(1, 2)
来源：http://ini.smart0.xyz

[T13] Kotlin：只读 Map
来源：http://qst.daxiang520.top

val m = mapOf("a" to 1)
来源：http://rhu.nanxuanxn.top

[T14] Kotlin：循环
来源：http://eau.fzhhl.top

for (i in 1..10) println(i)
来源：http://oya.jinqigufen.top

[T15] Kotlin：接口
来源：http://ftc.tanke756.top

interface Shape { fun area(): Double }
来源：http://prq.aizwys.cn

[T16] Swift：Hello World
来源：http://pwd.zdqjudy.top

print("Hello")
来源：http://sqo.sjlbkw.cn

[T17] Swift：变量与常量
来源：http://vkz.xingfuxueyuan.xyz

var a = 1;  let b = 2
来源：http://niy.sysykeji.top

[T18] Swift：字符串插值
来源：http://rnv.jinqigufen.top

"值: \(b)"
来源：http://bnh.hammf.cn

[T19] Swift：可选绑定
来源：http://cgf.uphjek.com

if let n = opt { print(n) }
来源：http://vxx.hnxiangtu.top

[T20] Swift：数组操作
来源：http://qvx.sjlbkw.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fcv.sxryk.cn

[T21] Swift：遍历
来源：http://tfh.hnxiangtu.top

for x in a { print(x) }
来源：http://irr.hongshengwenyu.top

[T22] Swift：字典
来源：http://avj.sweek.top

var d = ["a": 1];  d["b"] = 2
来源：http://yre.xuetiantiany.cn

[T23] Swift：函数
来源：http://bht.hesvh.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://szf.ydzc1.top

[T24] Swift：闭包
来源：http://goh.meibo888.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ioe.cqqwz.cn

[T25] Swift：结构体
来源：http://bqz.epnwcf.com

struct P { var x: Int }
来源：http://oeq.yuxming.cn

[T26] Swift：类与重写
来源：http://ldm.zdqjudy.top

class A: Base { override func f() {} }
来源：http://xop.nwbrower.top


<!-- 参考信息 -->