代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://dif.jianghu66.top

[R26] 命令替换
来源：http://yjz.yonumen.top

now=$(date +%F); echo "$now"
来源：http://bpn.316326.xyz

[R27] 算术展开
来源：http://aox.zhoulong.xyz

echo $((1 + 2 * 3))
来源：http://tot.yj20258.top

[R28] 浮点运算
来源：http://mlq.tianlin.xyz

echo "scale=2; 10/3" | bc
来源：http://pwl.guannengcc.top

[R29] 定义函数
来源：http://eby.shuidangran.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yxd.c1oappe.top

[R30] 函数返回状态码
来源：http://jvp.hysaishi.cn

f() { return 0; }; f || echo "失败了"
来源：http://pcl.nanxuanxn.top

[R31] 局部变量
来源：http://yzg.cheryme.top

f() { local x=1; echo "$x"; }
来源：http://ofi.jqgufenzy.top

[R32] 参数个数校验
来源：http://gdz.tanke756.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zqk.guannengcc.top

[R33] 捕获错误并提示行号
来源：http://tfp.bbcook.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cgd.yfazqb.com

[R34] 退出时清理
来源：http://rre.jianghu66.top

trap 'rm -f "$tmp"' EXIT
来源：http://pfo.ybcxt.top

[R35] 后台执行并等待
来源：http://vsj.zdqjudy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://dhu.tanke756.top

[R36] 并发执行多个任务
来源：http://kkd.jinghuilouyu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hse.hesvh.cn

[R37] 把输出赋给变量
来源：http://swn.jyoumei.cn

files=$(ls -1)
来源：http://niq.ivvv.top

[R38] 管道串联
来源：http://ryy.gzhubu.top

cat a.txt | grep -i error | wc -l
来源：http://uyv.birdmap.top

[R39] 重定向标准输出与错误
来源：http://wha.guannengcc.top

cmd > out.log 2>&1
来源：http://isj.zhijiandao.cn

[R40] 追加写日志
来源：http://fsd.cucudq.cn

echo "log" >> out.log
来源：http://ejq.meibo888.top

[R41] 丢弃输出
来源：http://bnm.hywenlv.cn

cmd >/dev/null 2>&1
来源：http://deo.redwolf501.top

[R42] 输入重定向
来源：http://vqo.tianlin.xyz

wc -l < a.txt
来源：http://ldg.shangyingyoupin.top

[R43] 按名字查找文件
来源：http://ift.jinghuilouyu.cn

find . -name "*.log" -type f
来源：http://xln.gzhubu.top

[R44] 按修改时间查找
来源：http://nbn.gzhubu.top

find . -mtime -7 -type f
来源：http://bud.xylfe.cn

[R45] 批量删除
来源：http://asb.xuanzx.com

find . -name "*.tmp" -delete
来源：http://ggf.nanxuanxn.top

[R46] 递归替换文件内容
来源：http://ltf.sjlbkw.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mqa.bbcook.cn

[R47] sed 单行替换
来源：http://hxx.tianlin.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://bgd.zycfv.cn

[R48] awk 取指定列
来源：http://xzz.cucudq.cn

awk '{print $1, $3}' a.txt
来源：http://cjf.jqgufenzy.top

[R49] awk 带条件
来源：http://pyr.xingfuxueyuan.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qdk.ydzc1.top

[R50] awk 求和
来源：http://twj.sysykeji.top

awk '{s += $2} END {print s}' a.txt
来源：http://cie.cqqwz.cn

[R51] 排序去重取前几
来源：http://xgx.redwolf501.top

sort a.txt | uniq -c | sort -rn | head
来源：http://tai.guannengcc.top

[R52] 统计行数
来源：http://qut.yonumen.top

wc -l a.txt
来源：http://tze.chenlongwang.top

[R53] 查看文件头与实时尾
来源：http://rod.ivvv.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qtu.tanke756.top

[R54] 比较两个文件
来源：http://rts.zhixingplan.top

diff a.txt b.txt
来源：http://cqb.xuanzx.com

[R55] 压缩与解压
来源：http://rup.daria6918.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xph.zdqjudy.top

[R56] 远程拷贝
来源：http://uoa.gzhubu.top

scp file user@host:/path/
来源：http://fga.zdqjudy.top

[R57] 远程执行命令
来源：http://hde.jinghuilouyu.cn

ssh user@host 'uptime'
来源：http://wkh.guannengcc.top

[R58] 下载文件
来源：http://xbd.tianlin.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xwa.wangdashe.top

[R59] 发 POST JSON
来源：http://tnf.ctjpmb.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://iex.yongpay.top

[R60] 只看 HTTP 状态码
来源：http://ptc.zdqjudy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jag.sufxvd.cn

[R61] 磁盘占用
来源：http://nmz.bjfxy.top

df -h;  du -sh *
来源：http://zxl.fehbvm.com

[R62] 找最占空间的文件
来源：http://pys.nanxinkj.top

du -ah . | sort -rh | head -10
来源：http://cbr.yongpay.top

[R63] 内存与进程
来源：http://tqc.jqgfzy.top

free -h;  ps aux | grep nginx
来源：http://xze.yj202588.top

[R64] 结束进程
来源：http://nda.yangfankeji.com

kill -9 $(pgrep -f app.py)
来源：http://fel.yfazqb.com

[R65] 查看端口占用
来源：http://jzw.zdbjq.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sjm.tianlin.xyz

[R66] 定时任务
来源：http://zyj.9152youxi.cn

crontab -e;  crontab -l
来源：http://oqr.bbcook.cn

[R67] 生成随机十六进制串
来源：http://duz.shangyingyoupin.top

openssl rand -hex 16
来源：http://ffw.yfazqb.com

[R68] 计算文件校验值
来源：http://hct.nwbrower.top

sha256sum a.txt;  md5sum a.txt
来源：http://lte.shzxlz.cn

[R69] 生成随机密码
来源：http://bxs.yj202588.top

head -c 16 /dev/urandom | base64
来源：http://mvc.havefunace.top

[R70] 时间戳与互转
来源：http://spp.ivvv.top

date +%s;  date -d @1700000000
来源：http://zmq.zhoulong.xyz

[R71] 日期格式化
来源：http://bip.gogol.net.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://fvz.sufxvd.cn

[R72] 等待端口就绪
来源：http://yld.daria6918.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qtr.yuanzhike.top

[R73] 分割大日志
来源：http://sqd.hcnkem.com

split -l 1000 big.log part_
来源：http://znc.gaohongyu789.top

[R74] 批量重命名
来源：http://crc.shzxlz.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dsx.nwbrower.top

[R75] 导出环境变量
来源：http://lai.jqgfzy.top

export PATH="$HOME/bin:$PATH"
来源：http://csz.fehbvm.com

[R76] 使用临时文件
来源：http://oui.52xcode.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://glm.chenjidiqi.icu

[R77] 读取用户输入
来源：http://sfb.pycfn.com

read -rp "请输入: " ans
来源：http://qzi.xuetiantiany.cn

[R78] 交互式菜单
来源：http://zbl.guannengcc.top

select opt in a b c; do echo "$opt"; break; done
来源：http://wma.gotoacloud.top

[R79] 解析命令行选项
来源：http://crz.yj202588.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pro.hnqzz.top

[R80] 查看脚本执行耗时
来源：http://zrl.xuanzx.com

time ./run.sh
来源：http://mwi.fanxiaobao.xyz

================================================================================
来源：http://vbd.sysykeji.top

S. C / C++ 专题
来源：http://kio.redwolf501.top

================================================================================
来源：http://enn.bjfxy.top

[S01] C：Hello World
来源：http://geo.zhoulong.xyz

#include <stdio.h>
来源：http://ghe.iojbl.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://pkb.haohaochexian.top

[S02] C：变量与格式化输出
来源：http://fin.jinqigufen.top

int a = 10; printf("%d\n", a);
来源：http://jbm.ydzc1.top

[S03] C：读入整数
来源：http://tcw.zhongyouzk.top

int x; scanf("%d", &x);
来源：http://wyc.zhongyouzk.top

[S04] C：字符串复制
来源：http://kje.vehdjk.com

char dst[32]; strcpy(dst, "hi");
来源：http://zvu.yanxiufei.cn

[S05] C：字符串长度
来源：http://gpd.zhixingplan.top

strlen(s)
来源：http://ifm.yuanzhike.top

[S06] C：字符串比较
来源：http://nyr.c1oappe.top

strcmp(a, b) == 0
来源：http://jog.daria6918.cn

[S07] C：数组遍历求和
来源：http://etg.ctjpmb.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kwp.kuanghao11.cn

[S08] C：动态内存分配与释放
来源：http://whq.jiagoushi.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zrw.mhx1999.top

[S09] C：结构体定义与初始化
来源：http://por.xylfe.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jzd.316326.xyz

[S10] C：指针与解引用
来源：http://glo.jinqigufen.top

int *p = &a;  *p = 5;
来源：http://jcq.dianchejie.cn

[S11] C：逐行读文件
来源：http://zkk.gotoacloud.top

FILE *f = fopen("a.txt", "r");
来源：http://iqj.jlsjyb.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://tfg.zdqjudy.top

fclose(f);
来源：http://dke.guannengcc.top

[S12] C：写文件
来源：http://kpp.nanxuanxn.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nsj.redwolf501.top

[S13] C：宏定义
来源：http://qki.jqgfzy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fxu.jinghuilouyu.cn

[S14] C：枚举
来源：http://yiq.yueranfly.top

enum Color { RED, GREEN, BLUE };
来源：http://qxg.fanxiaobao.xyz

[S15] C：类型转换
来源：http://xzq.andypj.xyz

(double) a / b
来源：http://ezd.9152youxi.cn

[S16] C：位操作置位
来源：http://lmq.gaohongyu789.top

x |= (1 << 3);
来源：http://miz.gogol.net.cn

[S17] C：安全拼接字符串
来源：http://fwv.zhaomingkeji.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bcn.316326.xyz

[S18] C：命令行参数
来源：http://gcv.xinyue.icu

int main(int argc, char **argv)
来源：http://yzf.gaohongyu789.top

[S19] C：快速排序
来源：http://xgb.zhoulong.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://tgb.jinqigufen.top

[S20] C：二分查找
来源：http://mkg.jiagoushi.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://eup.ehwqpu.com

[S21] C：字符类别判断
来源：http://xzj.hysaishi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kru.zhaomingkeji.xyz

[S22] C：字符串转数字
来源：http://xpt.zhongyouzk.top

atoi("42");  strtod("3.14", NULL);
来源：http://ugk.bbcook.cn

[S23] C：随机数
来源：http://idb.ywan-chungtsiang.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ukw.fanxiaobao.xyz

[S24] C：获取本地时间
来源：http://uac.meibo888.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://haq.jinqigufen.top

[S25] C：内存拷贝
来源：http://zha.dianchejie.cn

memcpy(dst, src, n);
来源：http://fyz.kuanghao11.cn

[S26] C：内存清零
来源：http://uma.zhiwuduotai.top

memset(a, 0, sizeof a);
来源：http://ijz.hysaishi.cn

[S27] C：定义常量
来源：http://mbe.nanxinkj.top

const double PI = 3.14159;
来源：http://svx.sufxvd.cn

[S28] C：静态变量
来源：http://phu.zhixingplan.top

static int counter = 0;
来源：http://bma.yj20258888.top

[S29] C：变参函数
来源：http://bxd.jyoumei.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vru.daria6918.cn

[S30] C：头文件保护
来源：http://ade.sufxvd.cn

#ifndef X_H
来源：http://ewb.cucudq.cn

#define X_H
来源：http://rww.jinqigufen.top

#endif
来源：http://ouk.haohaochexian.top

[S31] C++：Hello World
来源：http://pvv.svipenyu.cn

#include <iostream>
来源：http://nde.fzhhl.top

int main() { std::cout << "Hello\n"; }
来源：http://xhy.jqgufenzy.top

[S32] C++：字符串
来源：http://vvw.zhixingplan.top

std::string s = "hi";  s += "!";
来源：http://kmg.yongpay.top

[S33] C++：vector 增删
来源：http://hkj.zhixingplan.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tma.hesvh.cn

[S34] C++：遍历 vector
来源：http://wik.chenlongwang.top

for (auto &x : v) { std::cout << x; }
来源：http://dug.xingfuxueyuan.xyz

[S35] C++：map
来源：http://cgh.fanxiaobao.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://iax.cdnleiting.top

[S36] C++：unordered_map
来源：http://zhf.fktsv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ylh.jinyuanbaomall.cn

[S37] C++：set
来源：http://xsz.gaohongyu789.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zmz.havefunace.top

[S38] C++：排序
来源：http://nvi.jqgfzy.top

std::sort(v.begin(), v.end());
来源：http://djd.pengpengdd.cyou

[S39] C++：自定义比较器排序
来源：http://fbn.hysaishi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wzg.ydjk.org.cn

[S40] C++：查找元素
来源：http://zbb.sysykeji.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://guz.zhiwuduotai.top

[S41] C++：类与构造函数
来源：http://pjs.ivvv.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hkj.hfpthk.cn

[S42] C++：继承与虚函数
来源：http://wpn.fktsv.cn

class B : public Base { public: void f() override {} };
来源：http://agl.xuanzx.com

[S43] C++：智能指针
来源：http://ufz.quarkkingdee.top

auto p = std::make_unique<int>(5);
来源：http://rbm.gogol.net.cn

[S44] C++：引用传参
来源：http://qnu.fengsongda.top

void inc(int &x) { ++x; }
来源：http://xqf.smart0.xyz

[S45] C++：lambda
来源：http://omo.shzxlz.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hcb.xingfuxueyuan.xyz

[S46] C++：函数模板
来源：http://rwp.daria6918.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://daq.andypj.xyz

[S47] C++：结构化绑定遍历
来源：http://ohn.yfazqb.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://apb.fengsongda.top

[S48] C++：逐行读文件
来源：http://gxg.redwolf501.top

std::ifstream in("a.txt");  std::string line;
来源：http://ewn.hammf.cn

while (std::getline(in, line)) { }
来源：http://nka.chenlongwang.top

[S49] C++：写文件
来源：http://vwz.epnwcf.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ppf.cheryme.top

[S50] C++：格式化数字
来源：http://bhd.snrcjt.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://laa.cashguo.top

[S51] C++：显式类型转换
来源：http://wzw.quarkkingdee.top

static_cast<double>(a) / b
来源：http://qjb.shangyingyoupin.top

[S52] C++：const 与 noexcept
来源：http://qcm.shzxlz.cn

int size() const noexcept { return n_; }
来源：http://cnu.pengpengdd.cyou

[S53] C++：移动语义
来源：http://zhe.tian-w.cn

std::vector<int> w = std::move(v);
来源：http://tfi.haohaochexian.top

[S54] C++：异常处理
来源：http://bms.dashuyun.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yts.chenjidiqi.icu

[S55] C++：结构化绑定
来源：http://exd.yj20258888.top

auto [a, b] = std::make_pair(1, 2);
来源：http://zpp.yuxming.cn

[S56] C++：optional
来源：http://fqm.hnxiangtu.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://txl.fktsv.cn

[S57] C++：编译期常量
来源：http://cjn.sysykeji.top

constexpr int N = 10;
来源：http://qmi.ppjwa.cn

[S58] C++：命名空间
来源：http://zzh.xinyue.icu

namespace ns { int f() { return 1; } }
来源：http://lst.cucudq.cn

[S59] C++：静态断言
来源：http://npk.hywenlv.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cfr.hesvh.cn

[S60] C++：遍历并删除元素
来源：http://pzg.chenzaomai.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hsr.redwolf501.top

================================================================================
来源：http://cki.hysaishi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lap.epnwcf.com

================================================================================
来源：http://ddt.andypj.xyz

[T01] Kotlin：Hello World
来源：http://zkn.dashuyun.cn

println("Hello")
来源：http://ljc.hysaishi.cn

[T02] Kotlin：变量
来源：http://ayq.quarkkingdee.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xgf.jyoumei.cn

[T03] Kotlin：字符串模板
来源：http://lju.aibaodan.cn

"值: $b"
来源：http://dyt.shanyushiyangkeji.top

[T04] Kotlin：空安全
来源：http://nvj.shanyushiyangkeji.top

val n: String? = null;  n?.length
来源：http://xtt.tianlin.xyz

[T05] Kotlin：when 表达式
来源：http://aem.iojbl.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wfh.sjlbkw.cn

[T06] Kotlin：集合映射
来源：http://dum.dianchejie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ljs.hesvh.cn

[T07] Kotlin：集合过滤
来源：http://jmd.yvedp.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://umn.redwolf501.top

[T08] Kotlin：数据类
来源：http://bga.gaohongyu789.top

data class User(val name: String, val age: Int)
来源：http://ial.nanxuanxn.top

[T09] Kotlin：扩展函数
来源：http://vwb.dianchejie.cn

fun String.exclaim() = this + "!"
来源：http://qwv.tarul.cn

[T10] Kotlin：默认参数
来源：http://gmm.sysykeji.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ugq.jinghuilouyu.cn

[T11] Kotlin：协程
来源：http://fjh.quarkkingdee.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://lza.tianlin.xyz

[T12] Kotlin：解构声明
来源：http://ksv.jiagoushi.top

val (a, b) = Pair(1, 2)
来源：http://wgg.hcnkem.com

[T13] Kotlin：只读 Map
来源：http://hav.sweek.top

val m = mapOf("a" to 1)
来源：http://jqz.yonumen.top

[T14] Kotlin：循环
来源：http://umq.hesvh.cn

for (i in 1..10) println(i)
来源：http://koq.yvedp.cn

[T15] Kotlin：接口
来源：http://wpm.gotoacloud.top

interface Shape { fun area(): Double }
来源：http://kvn.52xcode.cn

[T16] Swift：Hello World
来源：http://grt.guannengcc.top

print("Hello")
来源：http://mof.zdqjudy.top

[T17] Swift：变量与常量
来源：http://qlh.aizwys.cn

var a = 1;  let b = 2
来源：http://enw.hnqzz.top

[T18] Swift：字符串插值
来源：http://ahb.jiagoushi.top

"值: \(b)"
来源：http://wtj.redwolf501.top

[T19] Swift：可选绑定
来源：http://exi.yonumen.top

if let n = opt { print(n) }
来源：http://xou.gzhubu.top

[T20] Swift：数组操作
来源：http://ipj.sxryk.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gdl.jinyuanbaomall.cn

[T21] Swift：遍历
来源：http://vup.yj20258.top

for x in a { print(x) }
来源：http://tij.zhengqikj.top

[T22] Swift：字典
来源：http://kos.fzhhl.top

var d = ["a": 1];  d["b"] = 2
来源：http://ukz.dianchejie.cn

[T23] Swift：函数
来源：http://mcl.xziqi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bjl.iojbl.cn

[T24] Swift：闭包
来源：http://ibg.bjfxy.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://art.fanxiaobao.xyz

[T25] Swift：结构体
来源：http://lbk.nanxuanxn.top

struct P { var x: Int }
来源：http://nko.zhoulong.xyz

[T26] Swift：类与重写
来源：http://ioq.shangyingyoupin.top

class A: Base { override func f() {} }
来源：http://yxw.shangyingyoupin.top

[T27] Swift：错误处理
来源：http://juf.andypj.xyz

do { try f() } catch { print(error) }
来源：http://fwj.zdqjudy.top

[T28] Swift：枚举
来源：http://jpn.cashguo.top

enum Color { case red, green }
来源：http://sjp.wangshuangyany.cn


<!-- 参考信息 -->