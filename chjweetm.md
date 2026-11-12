代发 wailian999

echo $((1 + 2 * 3))
来源：http://wnm.daria6918.cn

[R28] 浮点运算
来源：http://yka.chenjidiqi.icu

echo "scale=2; 10/3" | bc
来源：http://pqs.bjfxy.top

[R29] 定义函数
来源：http://kcv.sjlbkw.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dnc.c1oappe.top

[R30] 函数返回状态码
来源：http://kib.yvedp.cn

f() { return 0; }; f || echo "失败了"
来源：http://ebk.9152youxi.cn

[R31] 局部变量
来源：http://vor.guannengcc.top

f() { local x=1; echo "$x"; }
来源：http://aeg.wangshuangyany.cn

[R32] 参数个数校验
来源：http://zdf.bjfxy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zcm.bbcook.cn

[R33] 捕获错误并提示行号
来源：http://pyc.hysaishi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xoa.gogol.net.cn

[R34] 退出时清理
来源：http://dda.yanxiufei.cn

trap 'rm -f "$tmp"' EXIT
来源：http://nyh.ivvv.top

[R35] 后台执行并等待
来源：http://szt.hesvh.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ual.cucudq.cn

[R36] 并发执行多个任务
来源：http://lxv.shzxlz.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hqk.cucudq.cn

[R37] 把输出赋给变量
来源：http://ukp.ydzc1.top

files=$(ls -1)
来源：http://lpl.andypj.xyz

[R38] 管道串联
来源：http://qxi.mhx1999.top

cat a.txt | grep -i error | wc -l
来源：http://hjb.dianchejie.cn

[R39] 重定向标准输出与错误
来源：http://taf.shuidangran.top

cmd > out.log 2>&1
来源：http://zum.tianlin.xyz

[R40] 追加写日志
来源：http://qap.redwolf501.top

echo "log" >> out.log
来源：http://pfe.jiagoushi.top

[R41] 丢弃输出
来源：http://nvn.jqgufenzy.top

cmd >/dev/null 2>&1
来源：http://zuq.havefunace.top

[R42] 输入重定向
来源：http://xcg.hywenlv.cn

wc -l < a.txt
来源：http://pcl.yonumen.top

[R43] 按名字查找文件
来源：http://jxg.meibo888.top

find . -name "*.log" -type f
来源：http://ibi.quarkkingdee.top

[R44] 按修改时间查找
来源：http://fya.ivvv.top

find . -mtime -7 -type f
来源：http://bbl.cqqwz.cn

[R45] 批量删除
来源：http://yuq.jinqigufen.top

find . -name "*.tmp" -delete
来源：http://rkd.fengsongda.top

[R46] 递归替换文件内容
来源：http://rri.ydzc1.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tel.jiagoushi.top

[R47] sed 单行替换
来源：http://uel.ydjk.org.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mxf.cqqwz.cn

[R48] awk 取指定列
来源：http://kml.shanyushiyangtech.top

awk '{print $1, $3}' a.txt
来源：http://rqh.ydjk.org.cn

[R49] awk 带条件
来源：http://eof.ctjpmb.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ocf.bbcook.cn

[R50] awk 求和
来源：http://lmi.smart0.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://yfu.nwbrower.top

[R51] 排序去重取前几
来源：http://rye.ivvv.top

sort a.txt | uniq -c | sort -rn | head
来源：http://byw.pycfn.com

[R52] 统计行数
来源：http://fpm.fktsv.cn

wc -l a.txt
来源：http://ewb.yuanzhike.top

[R53] 查看文件头与实时尾
来源：http://tyk.yvedp.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wud.fzhhl.top

[R54] 比较两个文件
来源：http://hib.zdbjq.cn

diff a.txt b.txt
来源：http://ejb.chenlongwang.top

[R55] 压缩与解压
来源：http://zpk.yj20258888.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bea.gzhubu.top

[R56] 远程拷贝
来源：http://ast.jinqigfzy.top

scp file user@host:/path/
来源：http://yyx.zhongyouzk.top

[R57] 远程执行命令
来源：http://znb.jinqigfzy.top

ssh user@host 'uptime'
来源：http://hmp.guowangkeji.top

[R58] 下载文件
来源：http://lyx.hysaishi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baw.yfazqb.com

[R59] 发 POST JSON
来源：http://lnr.uphjek.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qyf.cashguo.top

[R60] 只看 HTTP 状态码
来源：http://pdi.mhx1999.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hdm.sysykeji.top

[R61] 磁盘占用
来源：http://fcd.zhaomingkeji.xyz

df -h;  du -sh *
来源：http://lfo.havefunace.top

[R62] 找最占空间的文件
来源：http://fww.zhaomingkeji.xyz

du -ah . | sort -rh | head -10
来源：http://ria.gaohongyu789.top

[R63] 内存与进程
来源：http://wea.quarkkingdee.top

free -h;  ps aux | grep nginx
来源：http://lex.ehwqpu.com

[R64] 结束进程
来源：http://qdw.nanxinkj.top

kill -9 $(pgrep -f app.py)
来源：http://xki.bbcook.cn

[R65] 查看端口占用
来源：http://prr.yuxming.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mjp.zhiwuduotai.top

[R66] 定时任务
来源：http://foe.iojbl.cn

crontab -e;  crontab -l
来源：http://spu.xuetiantiany.cn

[R67] 生成随机十六进制串
来源：http://mih.chenjidiqi.icu

openssl rand -hex 16
来源：http://awn.haohaochexian.top

[R68] 计算文件校验值
来源：http://rzm.hammf.cn

sha256sum a.txt;  md5sum a.txt
来源：http://lbd.jinghuilouyu.cn

[R69] 生成随机密码
来源：http://bto.hysaishi.cn

head -c 16 /dev/urandom | base64
来源：http://mmt.kuanghao11.cn

[R70] 时间戳与互转
来源：http://nht.316326.xyz

date +%s;  date -d @1700000000
来源：http://xkh.zhengqikj.top

[R71] 日期格式化
来源：http://gfi.yangfankeji.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://hgi.daria6918.cn

[R72] 等待端口就绪
来源：http://lbq.cucudq.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cmn.birdmap.top

[R73] 分割大日志
来源：http://kin.dashuyun.cn

split -l 1000 big.log part_
来源：http://wto.smart0.xyz

[R74] 批量重命名
来源：http://qib.fengsongda.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vqr.hongshengwenyu.top

[R75] 导出环境变量
来源：http://qzg.tanke756.top

export PATH="$HOME/bin:$PATH"
来源：http://tyo.yuxming.cn

[R76] 使用临时文件
来源：http://lxg.snrcjt.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xrr.daria6918.cn

[R77] 读取用户输入
来源：http://xjh.xuanzx.com

read -rp "请输入: " ans
来源：http://xvr.sjlbkw.cn

[R78] 交互式菜单
来源：http://srm.hesvh.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://unq.yvedp.cn

[R79] 解析命令行选项
来源：http://grv.svipenyu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://aqx.shuidangran.top

[R80] 查看脚本执行耗时
来源：http://gvi.daria6918.cn

time ./run.sh
来源：http://mvl.ydjk.org.cn

================================================================================
来源：http://gau.andypj.xyz

S. C / C++ 专题
来源：http://wfb.zhongyouzk.top

================================================================================
来源：http://nsc.gaohongyu789.top

[S01] C：Hello World
来源：http://yod.bjfxy.top

#include <stdio.h>
来源：http://mui.bbcook.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://sgr.feifeiyinyue.top

[S02] C：变量与格式化输出
来源：http://cnq.hysaishi.cn

int a = 10; printf("%d\n", a);
来源：http://hdz.zhengqikj.top

[S03] C：读入整数
来源：http://axy.chenjidiqi.icu

int x; scanf("%d", &x);
来源：http://pbo.nanxinkj.top

[S04] C：字符串复制
来源：http://efi.52xcode.cn

char dst[32]; strcpy(dst, "hi");
来源：http://alk.sjlbkw.cn

[S05] C：字符串长度
来源：http://mte.jqgufenzy.top

strlen(s)
来源：http://sca.jqgfzy.top

[S06] C：字符串比较
来源：http://hwn.nwbrower.top

strcmp(a, b) == 0
来源：http://sbq.bbcook.cn

[S07] C：数组遍历求和
来源：http://rje.yueranfly.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rqv.iojbl.cn

[S08] C：动态内存分配与释放
来源：http://wor.ywan-chungtsiang.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ezd.yonumen.top

[S09] C：结构体定义与初始化
来源：http://sfg.hnxiangtu.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://skh.uphjek.com

[S10] C：指针与解引用
来源：http://ria.quarkkingdee.top

int *p = &a;  *p = 5;
来源：http://ncf.vehdjk.com

[S11] C：逐行读文件
来源：http://eoo.yonumen.top

FILE *f = fopen("a.txt", "r");
来源：http://qnj.zhoulong.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://glw.fanxiaobao.xyz

fclose(f);
来源：http://err.cdnleiting.top

[S12] C：写文件
来源：http://xhx.daria6918.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pwf.jyoumei.cn

[S13] C：宏定义
来源：http://xan.aizwys.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ong.wangdashe.top

[S14] C：枚举
来源：http://fjf.bbcook.cn

enum Color { RED, GREEN, BLUE };
来源：http://btb.nanxinkj.top

[S15] C：类型转换
来源：http://adq.jyoumei.cn

(double) a / b
来源：http://amk.ywan-chungtsiang.top

[S16] C：位操作置位
来源：http://pxr.shzxlz.cn

x |= (1 << 3);
来源：http://wlb.xziqi.cn

[S17] C：安全拼接字符串
来源：http://jve.ydjk.org.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qjs.aibaodan.cn

[S18] C：命令行参数
来源：http://lvm.tian-w.cn

int main(int argc, char **argv)
来源：http://gib.chenzaomai.com

[S19] C：快速排序
来源：http://amp.yanxiufei.cn

qsort(a, n, sizeof(int), cmp);
来源：http://lpj.zdqjudy.top

[S20] C：二分查找
来源：http://sjf.hammf.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ywd.dashuyun.cn

[S21] C：字符类别判断
来源：http://uxs.tian-w.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dqe.jinqigfzy.top

[S22] C：字符串转数字
来源：http://are.hysaishi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://oap.wangdashe.top

[S23] C：随机数
来源：http://cbf.cucudq.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://tgn.nanxinkj.top

[S24] C：获取本地时间
来源：http://aij.zdqjudy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dja.yanxiufei.cn

[S25] C：内存拷贝
来源：http://rvp.wangdashe.top

memcpy(dst, src, n);
来源：http://tzf.hesvh.cn

[S26] C：内存清零
来源：http://lwc.meibo888.top

memset(a, 0, sizeof a);
来源：http://wnn.fanxiaobao.xyz

[S27] C：定义常量
来源：http://xmk.tianlin.xyz

const double PI = 3.14159;
来源：http://ktm.mhx1999.top

[S28] C：静态变量
来源：http://fdh.zhoulong.xyz

static int counter = 0;
来源：http://kdr.yuanzhike.top

[S29] C：变参函数
来源：http://xfj.quarkkingdee.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bjd.zhoulong.xyz

[S30] C：头文件保护
来源：http://mtm.pycfn.com

#ifndef X_H
来源：http://cjw.yanxiufei.cn

#define X_H
来源：http://qkm.cheryme.top

#endif
来源：http://pss.yj20258.top

[S31] C++：Hello World
来源：http://kyg.jlsjyb.cn

#include <iostream>
来源：http://cdd.cheryme.top

int main() { std::cout << "Hello\n"; }
来源：http://xgi.dianchejie.cn

[S32] C++：字符串
来源：http://vio.yangfankeji.com

std::string s = "hi";  s += "!";
来源：http://lbz.tanke756.top

[S33] C++：vector 增删
来源：http://bnf.shangyingyoupin.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dfz.vqdsnc.cn

[S34] C++：遍历 vector
来源：http://mel.shzxlz.cn

for (auto &x : v) { std::cout << x; }
来源：http://fsd.wangdashe.top

[S35] C++：map
来源：http://dvy.jiagoushi.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sbd.dianchejie.cn

[S36] C++：unordered_map
来源：http://bhv.cqqwz.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uom.quarkkingdee.top

[S37] C++：set
来源：http://ozn.zhongyouzk.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tas.jqgufenzy.top

[S38] C++：排序
来源：http://kru.jinqigufen.top

std::sort(v.begin(), v.end());
来源：http://kmq.vehdjk.com

[S39] C++：自定义比较器排序
来源：http://ryy.mhx1999.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zwo.mhx1999.top

[S40] C++：查找元素
来源：http://nqb.ywan-chungtsiang.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lke.tian-w.cn

[S41] C++：类与构造函数
来源：http://plp.shuidangran.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://atj.cdnleiting.top

[S42] C++：继承与虚函数
来源：http://jdo.birdmap.top

class B : public Base { public: void f() override {} };
来源：http://gdv.shanyushiyangtech.top

[S43] C++：智能指针
来源：http://nlz.hesvh.cn

auto p = std::make_unique<int>(5);
来源：http://uqc.jinqigfzy.top

[S44] C++：引用传参
来源：http://gnr.birdmap.top

void inc(int &x) { ++x; }
来源：http://wmt.fengsongda.top

[S45] C++：lambda
来源：http://cbc.hongshengwenyu.top

auto add = [](int a, int b) { return a + b; };
来源：http://xvu.andypj.xyz

[S46] C++：函数模板
来源：http://fxk.gaohongyu789.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wdu.kuanghao11.cn

[S47] C++：结构化绑定遍历
来源：http://vie.yonumen.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fox.meibo888.top

[S48] C++：逐行读文件
来源：http://hpu.ydjk.org.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ifx.havefunace.top

while (std::getline(in, line)) { }
来源：http://cgb.mhx1999.top

[S49] C++：写文件
来源：http://bax.meibo888.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kdy.wangshuangyany.cn

[S50] C++：格式化数字
来源：http://tdo.gzhubu.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xsn.pycfn.com

[S51] C++：显式类型转换
来源：http://sjh.nanxuanxn.top

static_cast<double>(a) / b
来源：http://jsx.jinghuilouyu.cn

[S52] C++：const 与 noexcept
来源：http://aqp.zdbjq.cn

int size() const noexcept { return n_; }
来源：http://anw.tian-w.cn

[S53] C++：移动语义
来源：http://hpb.vehdjk.com

std::vector<int> w = std::move(v);
来源：http://lwq.hysaishi.cn

[S54] C++：异常处理
来源：http://xal.uphjek.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gme.zhijiandao.cn

[S55] C++：结构化绑定
来源：http://kst.yj202588.top

auto [a, b] = std::make_pair(1, 2);
来源：http://sbb.yj202588.top

[S56] C++：optional
来源：http://ctq.52xcode.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kry.fanxiaobao.xyz

[S57] C++：编译期常量
来源：http://plf.kuanghao11.cn

constexpr int N = 10;
来源：http://jjl.jianghu66.top

[S58] C++：命名空间
来源：http://cip.cheryme.top

namespace ns { int f() { return 1; } }
来源：http://ltm.xuanzx.com

[S59] C++：静态断言
来源：http://hft.jlsjyb.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fqa.fktsv.cn

[S60] C++：遍历并删除元素
来源：http://fqt.tarul.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ryb.jqgufenzy.top

================================================================================
来源：http://wbj.yongpay.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xpc.svipenyu.cn

================================================================================
来源：http://van.yvedp.cn

[T01] Kotlin：Hello World
来源：http://nnl.zdbjq.cn

println("Hello")
来源：http://fjb.daxiang520.top

[T02] Kotlin：变量
来源：http://bpk.c1oappe.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://epx.svipenyu.cn

[T03] Kotlin：字符串模板
来源：http://bos.nanxuanxn.top

"值: $b"
来源：http://auy.jyoumei.cn

[T04] Kotlin：空安全
来源：http://vkz.hywenlv.cn

val n: String? = null;  n?.length
来源：http://itl.jinqigfzy.top

[T05] Kotlin：when 表达式
来源：http://peb.fanxiaobao.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zuo.svipenyu.cn

[T06] Kotlin：集合映射
来源：http://cdz.jqgufenzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://tbx.fengsongda.top

[T07] Kotlin：集合过滤
来源：http://sha.zycfv.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://tol.jiagoushi.top

[T08] Kotlin：数据类
来源：http://hoq.bbcook.cn

data class User(val name: String, val age: Int)
来源：http://oos.yuanzhike.top

[T09] Kotlin：扩展函数
来源：http://xnd.bjfxy.top

fun String.exclaim() = this + "!"
来源：http://poy.yfazqb.com

[T10] Kotlin：默认参数
来源：http://asn.wangdashe.top

fun greet(name: String = "World") = "Hi $name"
来源：http://lhq.hfpthk.cn

[T11] Kotlin：协程
来源：http://rcy.pengpengdd.cyou

GlobalScope.launch { delay(1000); println("done") }
来源：http://ovp.nwbrower.top

[T12] Kotlin：解构声明
来源：http://clx.hysaishi.cn

val (a, b) = Pair(1, 2)
来源：http://sfr.chenzaomai.com

[T13] Kotlin：只读 Map
来源：http://sxf.tian-w.cn

val m = mapOf("a" to 1)
来源：http://rym.guowangkeji.top

[T14] Kotlin：循环
来源：http://ogs.shanyushiyangkeji.top

for (i in 1..10) println(i)
来源：http://ynh.havefunace.top

[T15] Kotlin：接口
来源：http://ojl.gaohongyu789.top

interface Shape { fun area(): Double }
来源：http://xfj.yvedp.cn

[T16] Swift：Hello World
来源：http://iul.jyoumei.cn

print("Hello")
来源：http://gop.zhongyouzk.top

[T17] Swift：变量与常量
来源：http://vux.vqdsnc.cn

var a = 1;  let b = 2
来源：http://ano.bjfxy.top

[T18] Swift：字符串插值
来源：http://vwt.redwolf501.top

"值: \(b)"
来源：http://jis.meibo888.top

[T19] Swift：可选绑定
来源：http://qtv.zhiwuduotai.top

if let n = opt { print(n) }
来源：http://rvd.ppjwa.cn

[T20] Swift：数组操作
来源：http://ulx.guowangkeji.top

var a = [1, 2, 3];  a.append(4)
来源：http://rgn.ppjwa.cn

[T21] Swift：遍历
来源：http://xgi.jinqigfzy.top

for x in a { print(x) }
来源：http://rqn.sjlbkw.cn

[T22] Swift：字典
来源：http://nvi.aibaodan.cn

var d = ["a": 1];  d["b"] = 2
来源：http://gla.chenlongwang.top

[T23] Swift：函数
来源：http://edn.xinyue.icu

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sqf.pycfn.com

[T24] Swift：闭包
来源：http://uaw.ydzc1.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://zhh.xylfe.cn

[T25] Swift：结构体
来源：http://blh.nwbrower.top

struct P { var x: Int }
来源：http://mvb.dianchejie.cn

[T26] Swift：类与重写
来源：http://jgr.xinyue.icu

class A: Base { override func f() {} }
来源：http://pki.vqdsnc.cn

[T27] Swift：错误处理
来源：http://ooa.yongpay.top

do { try f() } catch { print(error) }
来源：http://wot.jinghuilouyu.cn

[T28] Swift：枚举
来源：http://hnj.cdnleiting.top

enum Color { case red, green }
来源：http://fup.jqgufenzy.top

[T29] Swift：guard 提前返回
来源：http://cgi.zdbjq.cn

guard let x = opt else { return }
来源：http://yhd.birdmap.top

[T30] Swift：协议
来源：http://viv.xingfuxueyuan.xyz

protocol Shape { func area() -> Double }
来源：http://rai.bjfxy.top


<!-- 参考信息 -->