代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wpo.andypj.xyz

[R24] 大小写转换
来源：http://rdf.ydzc1.top

echo "${s^^}"; echo "${s,,}"
来源：http://avt.sweek.top

[R25] 去后缀 / 去前缀
来源：http://hzq.shanyushiyangtech.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://qth.jqgufenzy.top

[R26] 命令替换
来源：http://kpn.shanyushiyangtech.top

now=$(date +%F); echo "$now"
来源：http://aez.zhijiandao.cn

[R27] 算术展开
来源：http://uri.andypj.xyz

echo $((1 + 2 * 3))
来源：http://tct.sxryk.cn

[R28] 浮点运算
来源：http://jvn.zhaomingkeji.xyz

echo "scale=2; 10/3" | bc
来源：http://dju.xziqi.cn

[R29] 定义函数
来源：http://fqm.ydzc1.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://sio.birdmap.top

[R30] 函数返回状态码
来源：http://qhu.xinyue.icu

f() { return 0; }; f || echo "失败了"
来源：http://fit.guowangkeji.top

[R31] 局部变量
来源：http://knd.zhaomingkeji.xyz

f() { local x=1; echo "$x"; }
来源：http://qfg.shanyushiyangkeji.top

[R32] 参数个数校验
来源：http://leg.nanxinkj.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ibz.cqqwz.cn

[R33] 捕获错误并提示行号
来源：http://kxn.jyoumei.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mfy.jinyuanbaomall.cn

[R34] 退出时清理
来源：http://rhc.sxryk.cn

trap 'rm -f "$tmp"' EXIT
来源：http://eno.fanxiaobao.xyz

[R35] 后台执行并等待
来源：http://hkb.jinqigufen.top

sleep 5 & pid=$!; wait "$pid"
来源：http://zkh.redwolf501.top

[R36] 并发执行多个任务
来源：http://lyk.tanke756.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nfj.zdqjudy.top

[R37] 把输出赋给变量
来源：http://ixr.c1oappe.top

files=$(ls -1)
来源：http://bhz.jinqigufen.top

[R38] 管道串联
来源：http://mmd.zhijiandao.cn

cat a.txt | grep -i error | wc -l
来源：http://aav.smart0.xyz

[R39] 重定向标准输出与错误
来源：http://vax.xuanzx.com

cmd > out.log 2>&1
来源：http://dyv.quarkkingdee.top

[R40] 追加写日志
来源：http://qzc.cheryme.top

echo "log" >> out.log
来源：http://smz.hesvh.cn

[R41] 丢弃输出
来源：http://ffd.52xcode.cn

cmd >/dev/null 2>&1
来源：http://eix.cucudq.cn

[R42] 输入重定向
来源：http://bqh.zhijiandao.cn

wc -l < a.txt
来源：http://nua.hongshengwenyu.top

[R43] 按名字查找文件
来源：http://xme.hywenlv.cn

find . -name "*.log" -type f
来源：http://vkd.zdbjq.cn

[R44] 按修改时间查找
来源：http://qcy.jyoumei.cn

find . -mtime -7 -type f
来源：http://nri.aizwys.cn

[R45] 批量删除
来源：http://ivy.fengsongda.top

find . -name "*.tmp" -delete
来源：http://fif.ehwqpu.com

[R46] 递归替换文件内容
来源：http://yws.kuanghao11.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gpz.sjlbkw.cn

[R47] sed 单行替换
来源：http://rzl.redwolf501.top

sed -i 's/foo/bar/g' a.txt
来源：http://elw.shangyingyoupin.top

[R48] awk 取指定列
来源：http://ztz.zhijiandao.cn

awk '{print $1, $3}' a.txt
来源：http://mhb.sjlbkw.cn

[R49] awk 带条件
来源：http://rrg.nanxinkj.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pff.birdmap.top

[R50] awk 求和
来源：http://hmh.ppjwa.cn

awk '{s += $2} END {print s}' a.txt
来源：http://lht.guowangkeji.top

[R51] 排序去重取前几
来源：http://nli.yanxiufei.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://rfu.tian-w.cn

[R52] 统计行数
来源：http://ktq.sysykeji.top

wc -l a.txt
来源：http://xki.daria6918.cn

[R53] 查看文件头与实时尾
来源：http://ibm.cqqwz.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://oky.meibo888.top

[R54] 比较两个文件
来源：http://gqm.jiagoushi.top

diff a.txt b.txt
来源：http://jvu.jinqigfzy.top

[R55] 压缩与解压
来源：http://egl.cashguo.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gye.yj20258888.top

[R56] 远程拷贝
来源：http://fie.hammf.cn

scp file user@host:/path/
来源：http://hxd.yuanzhike.top

[R57] 远程执行命令
来源：http://kgi.yuxming.cn

ssh user@host 'uptime'
来源：http://ruz.jlsjyb.cn

[R58] 下载文件
来源：http://njx.xylfe.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dik.nwbrower.top

[R59] 发 POST JSON
来源：http://asn.hcnkem.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://krl.hammf.cn

[R60] 只看 HTTP 状态码
来源：http://omk.tian-w.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rzv.c1oappe.top

[R61] 磁盘占用
来源：http://rgc.zhaomingkeji.xyz

df -h;  du -sh *
来源：http://lsz.yj20258.top

[R62] 找最占空间的文件
来源：http://vyq.sjlbkw.cn

du -ah . | sort -rh | head -10
来源：http://dqc.gogol.net.cn

[R63] 内存与进程
来源：http://rrp.vehdjk.com

free -h;  ps aux | grep nginx
来源：http://cjb.nanxuanxn.top

[R64] 结束进程
来源：http://ixh.yfazqb.com

kill -9 $(pgrep -f app.py)
来源：http://ohc.ydzc1.top

[R65] 查看端口占用
来源：http://lel.yj20258.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dbl.pengpengdd.cyou

[R66] 定时任务
来源：http://jbe.nanxuanxn.top

crontab -e;  crontab -l
来源：http://jhu.jinqigufen.top

[R67] 生成随机十六进制串
来源：http://tpa.pengpengdd.cyou

openssl rand -hex 16
来源：http://wfi.cqqwz.cn

[R68] 计算文件校验值
来源：http://tcz.chenzaomai.com

sha256sum a.txt;  md5sum a.txt
来源：http://cnx.nanxinkj.top

[R69] 生成随机密码
来源：http://ifv.daxiang520.top

head -c 16 /dev/urandom | base64
来源：http://oki.jqgufenzy.top

[R70] 时间戳与互转
来源：http://jze.shzxlz.cn

date +%s;  date -d @1700000000
来源：http://vvn.hammf.cn

[R71] 日期格式化
来源：http://xgq.zhixingplan.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://bxc.sjlbkw.cn

[R72] 等待端口就绪
来源：http://ukz.vehdjk.com

until nc -z localhost 3306; do sleep 1; done
来源：http://cex.gogol.net.cn

[R73] 分割大日志
来源：http://aal.xziqi.cn

split -l 1000 big.log part_
来源：http://oyy.yonumen.top

[R74] 批量重命名
来源：http://mdf.cucudq.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zds.pycfn.com

[R75] 导出环境变量
来源：http://cdr.zhongyouzk.top

export PATH="$HOME/bin:$PATH"
来源：http://oou.andypj.xyz

[R76] 使用临时文件
来源：http://biu.nanxinkj.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://aks.jqgufenzy.top

[R77] 读取用户输入
来源：http://qvf.c1oappe.top

read -rp "请输入: " ans
来源：http://ogd.jqgufenzy.top

[R78] 交互式菜单
来源：http://dtr.jqgufenzy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://chp.feifeiyinyue.top

[R79] 解析命令行选项
来源：http://frx.havefunace.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pxh.fehbvm.com

[R80] 查看脚本执行耗时
来源：http://azh.shanyushiyangkeji.top

time ./run.sh
来源：http://chs.ywan-chungtsiang.top

================================================================================
来源：http://ugw.gaohongyu789.top

S. C / C++ 专题
来源：http://jsu.zhongyouzk.top

================================================================================
来源：http://irv.vqdsnc.cn

[S01] C：Hello World
来源：http://jfa.chenlongwang.top

#include <stdio.h>
来源：http://vsh.chenlongwang.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://mei.wangdashe.top

[S02] C：变量与格式化输出
来源：http://qiw.yfazqb.com

int a = 10; printf("%d\n", a);
来源：http://wxt.jinqigfzy.top

[S03] C：读入整数
来源：http://owo.jinyuanbaomall.cn

int x; scanf("%d", &x);
来源：http://qgt.ywan-chungtsiang.top

[S04] C：字符串复制
来源：http://fvm.fanxiaobao.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://pjl.52xcode.cn

[S05] C：字符串长度
来源：http://eon.xinyue.icu

strlen(s)
来源：http://vyo.9152youxi.cn

[S06] C：字符串比较
来源：http://jgt.kuanghao11.cn

strcmp(a, b) == 0
来源：http://dgq.zhijiandao.cn

[S07] C：数组遍历求和
来源：http://emd.zhoulong.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xac.zhixingplan.top

[S08] C：动态内存分配与释放
来源：http://peh.wangdashe.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wwq.zhengqikj.top

[S09] C：结构体定义与初始化
来源：http://bsw.hesvh.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://btb.wangdashe.top

[S10] C：指针与解引用
来源：http://lwq.cheryme.top

int *p = &a;  *p = 5;
来源：http://gup.meibo888.top

[S11] C：逐行读文件
来源：http://wmj.jianghu66.top

FILE *f = fopen("a.txt", "r");
来源：http://hvy.chenjidiqi.icu

while (fgets(buf, sizeof buf, f)) { }
来源：http://ugn.fehbvm.com

fclose(f);
来源：http://bts.bjfxy.top

[S12] C：写文件
来源：http://sym.sxryk.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qco.zdqjudy.top

[S13] C：宏定义
来源：http://twe.yj202588.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vbz.jqgfzy.top

[S14] C：枚举
来源：http://bap.tarul.cn

enum Color { RED, GREEN, BLUE };
来源：http://pkp.0kj1m.cn

[S15] C：类型转换
来源：http://lve.cqqwz.cn

(double) a / b
来源：http://okz.dianchejie.cn

[S16] C：位操作置位
来源：http://fhg.jqgfzy.top

x |= (1 << 3);
来源：http://cfe.zhaomingkeji.xyz

[S17] C：安全拼接字符串
来源：http://bgw.hywenlv.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hle.fehbvm.com

[S18] C：命令行参数
来源：http://elm.hammf.cn

int main(int argc, char **argv)
来源：http://uqr.hnxiangtu.top

[S19] C：快速排序
来源：http://ldx.shzxlz.cn

qsort(a, n, sizeof(int), cmp);
来源：http://nwx.xziqi.cn

[S20] C：二分查找
来源：http://yrd.fehbvm.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ior.zhengqikj.top

[S21] C：字符类别判断
来源：http://vrs.cheryme.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://etk.nwbrower.top

[S22] C：字符串转数字
来源：http://wuh.sysykeji.top

atoi("42");  strtod("3.14", NULL);
来源：http://wub.shzxlz.cn

[S23] C：随机数
来源：http://gbt.hnxiangtu.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ufo.fzhhl.top

[S24] C：获取本地时间
来源：http://nnk.9152youxi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ifq.guannengcc.top

[S25] C：内存拷贝
来源：http://vjv.yfazqb.com

memcpy(dst, src, n);
来源：http://ysl.ydzc1.top

[S26] C：内存清零
来源：http://mjn.yangfankeji.com

memset(a, 0, sizeof a);
来源：http://aui.feifeiyinyue.top

[S27] C：定义常量
来源：http://cnc.fanxiaobao.xyz

const double PI = 3.14159;
来源：http://qoc.fengsongda.top

[S28] C：静态变量
来源：http://cbu.hongshengwenyu.top

static int counter = 0;
来源：http://tin.hysaishi.cn

[S29] C：变参函数
来源：http://dsg.zhengqikj.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ksz.tianlin.xyz

[S30] C：头文件保护
来源：http://kmg.pycfn.com

#ifndef X_H
来源：http://xmq.guowangkeji.top

#define X_H
来源：http://vde.meibo888.top

#endif
来源：http://sot.gotoacloud.top

[S31] C++：Hello World
来源：http://wsx.hesvh.cn

#include <iostream>
来源：http://sak.tanke756.top

int main() { std::cout << "Hello\n"; }
来源：http://toh.snrcjt.cn

[S32] C++：字符串
来源：http://jky.feifeiyinyue.top

std::string s = "hi";  s += "!";
来源：http://hwm.nwbrower.top

[S33] C++：vector 增删
来源：http://hkq.cucudq.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yiy.sufxvd.cn

[S34] C++：遍历 vector
来源：http://cim.feifeiyinyue.top

for (auto &x : v) { std::cout << x; }
来源：http://mxx.guowangkeji.top

[S35] C++：map
来源：http://ryk.xziqi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jeq.yongpay.top

[S36] C++：unordered_map
来源：http://cyi.kuanghao11.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://agq.xingfuxueyuan.xyz

[S37] C++：set
来源：http://ejg.kuanghao11.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ata.pycfn.com

[S38] C++：排序
来源：http://gyr.quarkkingdee.top

std::sort(v.begin(), v.end());
来源：http://flq.shzxlz.cn

[S39] C++：自定义比较器排序
来源：http://yjq.guannengcc.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fox.zhengqikj.top

[S40] C++：查找元素
来源：http://ygn.fengsongda.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nha.shuidangran.top

[S41] C++：类与构造函数
来源：http://ucn.meibo888.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qye.feifeiyinyue.top

[S42] C++：继承与虚函数
来源：http://inz.cucudq.cn

class B : public Base { public: void f() override {} };
来源：http://zjb.yonumen.top

[S43] C++：智能指针
来源：http://ktt.meibo888.top

auto p = std::make_unique<int>(5);
来源：http://wup.hnxiangtu.top

[S44] C++：引用传参
来源：http://rzz.yj20258.top

void inc(int &x) { ++x; }
来源：http://zwu.quarkkingdee.top

[S45] C++：lambda
来源：http://wdd.sysykeji.top

auto add = [](int a, int b) { return a + b; };
来源：http://pag.vqdsnc.cn

[S46] C++：函数模板
来源：http://mbv.fanxiaobao.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xvk.daria6918.cn

[S47] C++：结构化绑定遍历
来源：http://gkp.havefunace.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tpc.pycfn.com

[S48] C++：逐行读文件
来源：http://oed.yangfankeji.com

std::ifstream in("a.txt");  std::string line;
来源：http://qor.hywenlv.cn

while (std::getline(in, line)) { }
来源：http://fih.cucudq.cn

[S49] C++：写文件
来源：http://qzf.yvedp.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ywf.hysaishi.cn

[S50] C++：格式化数字
来源：http://vif.meibo888.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yii.ydjk.org.cn

[S51] C++：显式类型转换
来源：http://ftb.xylfe.cn

static_cast<double>(a) / b
来源：http://eby.yj20258.top

[S52] C++：const 与 noexcept
来源：http://ilm.snrcjt.cn

int size() const noexcept { return n_; }
来源：http://zvg.fengsongda.top

[S53] C++：移动语义
来源：http://wty.pycfn.com

std::vector<int> w = std::move(v);
来源：http://zqk.yuanzhike.top

[S54] C++：异常处理
来源：http://zsg.jlsjyb.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bow.guannengcc.top

[S55] C++：结构化绑定
来源：http://flo.gaohongyu789.top

auto [a, b] = std::make_pair(1, 2);
来源：http://brv.tanke756.top

[S56] C++：optional
来源：http://lrn.nwbrower.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mfj.gotoacloud.top

[S57] C++：编译期常量
来源：http://ocy.jianghu66.top

constexpr int N = 10;
来源：http://ykq.hywenlv.cn

[S58] C++：命名空间
来源：http://xld.hammf.cn

namespace ns { int f() { return 1; } }
来源：http://mxc.jqgfzy.top

[S59] C++：静态断言
来源：http://mrp.gaohongyu789.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vwb.daxiang520.top

[S60] C++：遍历并删除元素
来源：http://rpo.tianlin.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vbp.guowangkeji.top

================================================================================
来源：http://gli.cheryme.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rmj.shangyingyoupin.top

================================================================================
来源：http://jam.hfpthk.cn

[T01] Kotlin：Hello World
来源：http://xts.xuetiantiany.cn

println("Hello")
来源：http://std.feifeiyinyue.top

[T02] Kotlin：变量
来源：http://cba.zhengqikj.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lne.xuetiantiany.cn

[T03] Kotlin：字符串模板
来源：http://wsx.aizwys.cn

"值: $b"
来源：http://vin.yuanzhike.top

[T04] Kotlin：空安全
来源：http://gru.zycfv.cn

val n: String? = null;  n?.length
来源：http://hwp.wangdashe.top

[T05] Kotlin：when 表达式
来源：http://xht.nanxinkj.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cor.zhijiandao.cn

[T06] Kotlin：集合映射
来源：http://qgv.havefunace.top

listOf(1, 2, 3).map { it * 2 }
来源：http://bhr.kuanghao11.cn

[T07] Kotlin：集合过滤
来源：http://lfp.zhoulong.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://lry.haohaochexian.top

[T08] Kotlin：数据类
来源：http://jig.yuanzhike.top

data class User(val name: String, val age: Int)
来源：http://tcs.wangdashe.top

[T09] Kotlin：扩展函数
来源：http://yzr.hysaishi.cn

fun String.exclaim() = this + "!"
来源：http://nnh.shanyushiyangtech.top

[T10] Kotlin：默认参数
来源：http://nkp.birdmap.top

fun greet(name: String = "World") = "Hi $name"
来源：http://arl.fehbvm.com

[T11] Kotlin：协程
来源：http://egm.guowangkeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ihc.guannengcc.top

[T12] Kotlin：解构声明
来源：http://nme.iojbl.cn

val (a, b) = Pair(1, 2)
来源：http://jpp.yvedp.cn

[T13] Kotlin：只读 Map
来源：http://qfk.daxiang520.top

val m = mapOf("a" to 1)
来源：http://yom.havefunace.top

[T14] Kotlin：循环
来源：http://tjn.havefunace.top

for (i in 1..10) println(i)
来源：http://ytu.52xcode.cn

[T15] Kotlin：接口
来源：http://pet.cqqwz.cn

interface Shape { fun area(): Double }
来源：http://nef.cheryme.top

[T16] Swift：Hello World
来源：http://kzv.tanke756.top

print("Hello")
来源：http://msr.chenjidiqi.icu

[T17] Swift：变量与常量
来源：http://whe.redwolf501.top

var a = 1;  let b = 2
来源：http://opn.iojbl.cn

[T18] Swift：字符串插值
来源：http://nzj.hnxiangtu.top

"值: \(b)"
来源：http://php.jinqigufen.top

[T19] Swift：可选绑定
来源：http://rjk.jqgfzy.top

if let n = opt { print(n) }
来源：http://nrb.sufxvd.cn

[T20] Swift：数组操作
来源：http://njp.xylfe.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ead.xziqi.cn

[T21] Swift：遍历
来源：http://kqy.yfazqb.com

for x in a { print(x) }
来源：http://juk.smart0.xyz

[T22] Swift：字典
来源：http://wrz.hywenlv.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xyy.quarkkingdee.top

[T23] Swift：函数
来源：http://lcl.sweek.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kqj.hammf.cn

[T24] Swift：闭包
来源：http://cvo.dianchejie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://prq.aizwys.cn

[T25] Swift：结构体
来源：http://gnv.gzhubu.top

struct P { var x: Int }
来源：http://cdc.cucudq.cn

[T26] Swift：类与重写
来源：http://oeo.ywan-chungtsiang.top

class A: Base { override func f() {} }
来源：http://dfm.zhiwuduotai.top


<!-- 参考信息 -->