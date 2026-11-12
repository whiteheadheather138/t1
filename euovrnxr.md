代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://mpu.sysykeji.top

[R32] 参数个数校验
来源：http://gmv.vehdjk.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yqx.gaohongyu789.top

[R33] 捕获错误并提示行号
来源：http://fwk.yj20258.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pww.nanxuanxn.top

[R34] 退出时清理
来源：http://jfs.nanxinkj.top

trap 'rm -f "$tmp"' EXIT
来源：http://nlz.shzxlz.cn

[R35] 后台执行并等待
来源：http://bjt.vqdsnc.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://pci.birdmap.top

[R36] 并发执行多个任务
来源：http://myv.shuidangran.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uli.zhixingplan.top

[R37] 把输出赋给变量
来源：http://ish.hcnkem.com

files=$(ls -1)
来源：http://lqe.chenzaomai.com

[R38] 管道串联
来源：http://mrk.nanxuanxn.top

cat a.txt | grep -i error | wc -l
来源：http://htx.ppjwa.cn

[R39] 重定向标准输出与错误
来源：http://ifx.vehdjk.com

cmd > out.log 2>&1
来源：http://tdi.andypj.xyz

[R40] 追加写日志
来源：http://ori.hysaishi.cn

echo "log" >> out.log
来源：http://ulv.sweek.top

[R41] 丢弃输出
来源：http://hde.ywan-chungtsiang.top

cmd >/dev/null 2>&1
来源：http://fjr.hfpthk.cn

[R42] 输入重定向
来源：http://gxw.epnwcf.com

wc -l < a.txt
来源：http://rfu.dashuyun.cn

[R43] 按名字查找文件
来源：http://lhq.meibo888.top

find . -name "*.log" -type f
来源：http://jya.yvedp.cn

[R44] 按修改时间查找
来源：http://iqb.jinqigufen.top

find . -mtime -7 -type f
来源：http://yoc.ydzc1.top

[R45] 批量删除
来源：http://xrp.shanyushiyangkeji.top

find . -name "*.tmp" -delete
来源：http://ate.iojbl.cn

[R46] 递归替换文件内容
来源：http://bbu.zhongyouzk.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://awh.havefunace.top

[R47] sed 单行替换
来源：http://sgt.zhixingplan.top

sed -i 's/foo/bar/g' a.txt
来源：http://xtm.hnqzz.top

[R48] awk 取指定列
来源：http://cse.zycfv.cn

awk '{print $1, $3}' a.txt
来源：http://gng.yj202588.top

[R49] awk 带条件
来源：http://kat.fktsv.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yui.aizwys.cn

[R50] awk 求和
来源：http://nkj.yuanzhike.top

awk '{s += $2} END {print s}' a.txt
来源：http://wab.xylfe.cn

[R51] 排序去重取前几
来源：http://mkq.jqgufenzy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://zlx.yongpay.top

[R52] 统计行数
来源：http://arv.vqdsnc.cn

wc -l a.txt
来源：http://dxf.ctjpmb.com

[R53] 查看文件头与实时尾
来源：http://jsd.gaohongyu789.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lxk.ywan-chungtsiang.top

[R54] 比较两个文件
来源：http://abg.ybcxt.top

diff a.txt b.txt
来源：http://feq.yj202588.top

[R55] 压缩与解压
来源：http://xuf.sufxvd.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jcj.ppjwa.cn

[R56] 远程拷贝
来源：http://xfm.yj20258.top

scp file user@host:/path/
来源：http://dds.gaohongyu789.top

[R57] 远程执行命令
来源：http://qoa.nwbrower.top

ssh user@host 'uptime'
来源：http://ran.haohaochexian.top

[R58] 下载文件
来源：http://mds.ydjk.org.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kfg.hammf.cn

[R59] 发 POST JSON
来源：http://efk.yuanzhike.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pui.shanyushiyangtech.top

[R60] 只看 HTTP 状态码
来源：http://xkf.vehdjk.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://oic.epnwcf.com

[R61] 磁盘占用
来源：http://lct.birdmap.top

df -h;  du -sh *
来源：http://noi.havefunace.top

[R62] 找最占空间的文件
来源：http://urt.daxiang520.top

du -ah . | sort -rh | head -10
来源：http://vxq.ehwqpu.com

[R63] 内存与进程
来源：http://oeb.jianghu66.top

free -h;  ps aux | grep nginx
来源：http://lwo.hammf.cn

[R64] 结束进程
来源：http://qmn.meibo888.top

kill -9 $(pgrep -f app.py)
来源：http://ahv.fengsongda.top

[R65] 查看端口占用
来源：http://ptq.aibaodan.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wun.tianlin.xyz

[R66] 定时任务
来源：http://xcy.feifeiyinyue.top

crontab -e;  crontab -l
来源：http://yop.ydjk.org.cn

[R67] 生成随机十六进制串
来源：http://wls.ivvv.top

openssl rand -hex 16
来源：http://jlp.hongshengwenyu.top

[R68] 计算文件校验值
来源：http://pyp.bbcook.cn

sha256sum a.txt;  md5sum a.txt
来源：http://jef.cdnleiting.top

[R69] 生成随机密码
来源：http://ogq.sysykeji.top

head -c 16 /dev/urandom | base64
来源：http://hbr.tian-w.cn

[R70] 时间戳与互转
来源：http://vfg.redwolf501.top

date +%s;  date -d @1700000000
来源：http://hbe.zhengqikj.top

[R71] 日期格式化
来源：http://qwz.wangdashe.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://dzn.shuidangran.top

[R72] 等待端口就绪
来源：http://kzx.hesvh.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://mak.guowangkeji.top

[R73] 分割大日志
来源：http://vsz.yongpay.top

split -l 1000 big.log part_
来源：http://dix.hnqzz.top

[R74] 批量重命名
来源：http://vjy.0kj1m.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qzl.chenlongwang.top

[R75] 导出环境变量
来源：http://yot.gotoacloud.top

export PATH="$HOME/bin:$PATH"
来源：http://yiw.bjfxy.top

[R76] 使用临时文件
来源：http://wmu.shanyushiyangkeji.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zku.wangdashe.top

[R77] 读取用户输入
来源：http://zbt.dashuyun.cn

read -rp "请输入: " ans
来源：http://qvv.jqgfzy.top

[R78] 交互式菜单
来源：http://mrd.fzhhl.top

select opt in a b c; do echo "$opt"; break; done
来源：http://rir.sysykeji.top

[R79] 解析命令行选项
来源：http://ish.dianchejie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nzz.cucudq.cn

[R80] 查看脚本执行耗时
来源：http://rij.pengpengdd.cyou

time ./run.sh
来源：http://nyy.ydjk.org.cn

================================================================================
来源：http://mdc.smart0.xyz

S. C / C++ 专题
来源：http://prm.sxryk.cn

================================================================================
来源：http://wrm.zdqjudy.top

[S01] C：Hello World
来源：http://dhb.gogol.net.cn

#include <stdio.h>
来源：http://yfc.jinqigufen.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://qqs.316326.xyz

[S02] C：变量与格式化输出
来源：http://shp.wangdashe.top

int a = 10; printf("%d\n", a);
来源：http://fll.hfpthk.cn

[S03] C：读入整数
来源：http://fil.316326.xyz

int x; scanf("%d", &x);
来源：http://mnd.redwolf501.top

[S04] C：字符串复制
来源：http://dqw.fzhhl.top

char dst[32]; strcpy(dst, "hi");
来源：http://hbp.cheryme.top

[S05] C：字符串长度
来源：http://hem.snrcjt.cn

strlen(s)
来源：http://bnp.jqgufenzy.top

[S06] C：字符串比较
来源：http://jlg.haohaochexian.top

strcmp(a, b) == 0
来源：http://wln.yongpay.top

[S07] C：数组遍历求和
来源：http://avz.smart0.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qoh.yuxming.cn

[S08] C：动态内存分配与释放
来源：http://kup.pengpengdd.cyou

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yhq.vqdsnc.cn

[S09] C：结构体定义与初始化
来源：http://yyy.sufxvd.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tbl.wangshuangyany.cn

[S10] C：指针与解引用
来源：http://bji.shangyingyoupin.top

int *p = &a;  *p = 5;
来源：http://pdh.cqqwz.cn

[S11] C：逐行读文件
来源：http://mgl.hysaishi.cn

FILE *f = fopen("a.txt", "r");
来源：http://qon.tanke756.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://qhq.gogol.net.cn

fclose(f);
来源：http://rmo.xylfe.cn

[S12] C：写文件
来源：http://jru.epnwcf.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gzq.yanxiufei.cn

[S13] C：宏定义
来源：http://ezm.iojbl.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jdd.zhengqikj.top

[S14] C：枚举
来源：http://nqq.zhaomingkeji.xyz

enum Color { RED, GREEN, BLUE };
来源：http://fvz.smart0.xyz

[S15] C：类型转换
来源：http://tlr.jianghu66.top

(double) a / b
来源：http://lfg.hysaishi.cn

[S16] C：位操作置位
来源：http://irg.aibaodan.cn

x |= (1 << 3);
来源：http://boo.zhengqikj.top

[S17] C：安全拼接字符串
来源：http://xsg.tian-w.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nfo.jinqigfzy.top

[S18] C：命令行参数
来源：http://jlt.c1oappe.top

int main(int argc, char **argv)
来源：http://nxb.shzxlz.cn

[S19] C：快速排序
来源：http://kbi.hongshengwenyu.top

qsort(a, n, sizeof(int), cmp);
来源：http://rwb.daxiang520.top

[S20] C：二分查找
来源：http://szh.vqdsnc.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://roe.guowangkeji.top

[S21] C：字符类别判断
来源：http://jtv.c1oappe.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nop.shanyushiyangkeji.top

[S22] C：字符串转数字
来源：http://hrc.fktsv.cn

atoi("42");  strtod("3.14", NULL);
来源：http://lbz.gzhubu.top

[S23] C：随机数
来源：http://ikp.zhixingplan.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ybn.quarkkingdee.top

[S24] C：获取本地时间
来源：http://txv.yj20258888.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ceo.jiagoushi.top

[S25] C：内存拷贝
来源：http://drc.zhengqikj.top

memcpy(dst, src, n);
来源：http://frk.tarul.cn

[S26] C：内存清零
来源：http://tra.fengsongda.top

memset(a, 0, sizeof a);
来源：http://ske.xingfuxueyuan.xyz

[S27] C：定义常量
来源：http://gtl.bjfxy.top

const double PI = 3.14159;
来源：http://wtm.tarul.cn

[S28] C：静态变量
来源：http://mve.wangshuangyany.cn

static int counter = 0;
来源：http://dgg.hcnkem.com

[S29] C：变参函数
来源：http://nba.iojbl.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kqj.fehbvm.com

[S30] C：头文件保护
来源：http://cir.redwolf501.top

#ifndef X_H
来源：http://vzl.smart0.xyz

#define X_H
来源：http://xnt.haohaochexian.top

#endif
来源：http://avr.zhoulong.xyz

[S31] C++：Hello World
来源：http://qiu.dashuyun.cn

#include <iostream>
来源：http://som.hnqzz.top

int main() { std::cout << "Hello\n"; }
来源：http://rzb.hfpthk.cn

[S32] C++：字符串
来源：http://xnj.cheryme.top

std::string s = "hi";  s += "!";
来源：http://uju.fehbvm.com

[S33] C++：vector 增删
来源：http://mlm.feifeiyinyue.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ukk.jiagoushi.top

[S34] C++：遍历 vector
来源：http://vil.bjfxy.top

for (auto &x : v) { std::cout << x; }
来源：http://sbf.snrcjt.cn

[S35] C++：map
来源：http://qss.gaohongyu789.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tsf.jinqigufen.top

[S36] C++：unordered_map
来源：http://vgu.tianlin.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qud.jqgufenzy.top

[S37] C++：set
来源：http://yoe.guowangkeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rgx.snrcjt.cn

[S38] C++：排序
来源：http://ywe.chenzaomai.com

std::sort(v.begin(), v.end());
来源：http://cgg.zdbjq.cn

[S39] C++：自定义比较器排序
来源：http://qzi.ydzc1.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kdq.havefunace.top

[S40] C++：查找元素
来源：http://dbq.52xcode.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pki.zycfv.cn

[S41] C++：类与构造函数
来源：http://aro.xziqi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nlq.shanyushiyangtech.top

[S42] C++：继承与虚函数
来源：http://erf.shuidangran.top

class B : public Base { public: void f() override {} };
来源：http://esz.aizwys.cn

[S43] C++：智能指针
来源：http://wbo.yonumen.top

auto p = std::make_unique<int>(5);
来源：http://kfj.chenlongwang.top

[S44] C++：引用传参
来源：http://guy.cucudq.cn

void inc(int &x) { ++x; }
来源：http://iqg.nanxuanxn.top

[S45] C++：lambda
来源：http://cgq.ydjk.org.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zho.aizwys.cn

[S46] C++：函数模板
来源：http://sjn.fanxiaobao.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://luh.yfazqb.com

[S47] C++：结构化绑定遍历
来源：http://ccg.ctjpmb.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://odg.zhiwuduotai.top

[S48] C++：逐行读文件
来源：http://zmp.ydzc1.top

std::ifstream in("a.txt");  std::string line;
来源：http://fke.xuanzx.com

while (std::getline(in, line)) { }
来源：http://etr.yueranfly.top

[S49] C++：写文件
来源：http://pah.shanyushiyangkeji.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mrh.fzhhl.top

[S50] C++：格式化数字
来源：http://fgy.pengpengdd.cyou

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ali.sufxvd.cn

[S51] C++：显式类型转换
来源：http://ykt.wangshuangyany.cn

static_cast<double>(a) / b
来源：http://dcn.fehbvm.com

[S52] C++：const 与 noexcept
来源：http://qmt.zhaomingkeji.xyz

int size() const noexcept { return n_; }
来源：http://zwu.cucudq.cn

[S53] C++：移动语义
来源：http://ked.yangfankeji.com

std::vector<int> w = std::move(v);
来源：http://tdc.uphjek.com

[S54] C++：异常处理
来源：http://aoj.316326.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kux.sysykeji.top

[S55] C++：结构化绑定
来源：http://wbw.vqdsnc.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://him.cdnleiting.top

[S56] C++：optional
来源：http://zsv.gaohongyu789.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://khi.bbcook.cn

[S57] C++：编译期常量
来源：http://vtg.yuxming.cn

constexpr int N = 10;
来源：http://mxy.zycfv.cn

[S58] C++：命名空间
来源：http://zrg.yvedp.cn

namespace ns { int f() { return 1; } }
来源：http://bha.9152youxi.cn

[S59] C++：静态断言
来源：http://ifq.zhixingplan.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mnu.xingfuxueyuan.xyz

[S60] C++：遍历并删除元素
来源：http://jtb.ctjpmb.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kve.xinyue.icu

================================================================================
来源：http://yuv.sufxvd.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nss.tarul.cn

================================================================================
来源：http://brj.cucudq.cn

[T01] Kotlin：Hello World
来源：http://jfq.jinqigfzy.top

println("Hello")
来源：http://zde.zhaomingkeji.xyz

[T02] Kotlin：变量
来源：http://eod.andypj.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tst.hnqzz.top

[T03] Kotlin：字符串模板
来源：http://nui.zhengqikj.top

"值: $b"
来源：http://suz.xuetiantiany.cn

[T04] Kotlin：空安全
来源：http://ttg.yangfankeji.com

val n: String? = null;  n?.length
来源：http://mkh.andypj.xyz

[T05] Kotlin：when 表达式
来源：http://laf.zdqjudy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://buc.0kj1m.cn

[T06] Kotlin：集合映射
来源：http://jxf.hfpthk.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tey.zhongyouzk.top

[T07] Kotlin：集合过滤
来源：http://lfi.fktsv.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://lzb.ybcxt.top

[T08] Kotlin：数据类
来源：http://wgo.pengpengdd.cyou

data class User(val name: String, val age: Int)
来源：http://dgq.vqdsnc.cn

[T09] Kotlin：扩展函数
来源：http://yey.feifeiyinyue.top

fun String.exclaim() = this + "!"
来源：http://kug.jinqigfzy.top

[T10] Kotlin：默认参数
来源：http://men.yanxiufei.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://yuz.zhongyouzk.top

[T11] Kotlin：协程
来源：http://ott.birdmap.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://mbn.haohaochexian.top

[T12] Kotlin：解构声明
来源：http://gqr.gaohongyu789.top

val (a, b) = Pair(1, 2)
来源：http://jfc.guannengcc.top

[T13] Kotlin：只读 Map
来源：http://rol.shanyushiyangkeji.top

val m = mapOf("a" to 1)
来源：http://ywu.gaohongyu789.top

[T14] Kotlin：循环
来源：http://hzt.daria6918.cn

for (i in 1..10) println(i)
来源：http://wpk.fanxiaobao.xyz

[T15] Kotlin：接口
来源：http://won.yongpay.top

interface Shape { fun area(): Double }
来源：http://pbw.316326.xyz

[T16] Swift：Hello World
来源：http://bkb.zhaomingkeji.xyz

print("Hello")
来源：http://dwy.hesvh.cn

[T17] Swift：变量与常量
来源：http://lzt.tanke756.top

var a = 1;  let b = 2
来源：http://urn.fehbvm.com

[T18] Swift：字符串插值
来源：http://cjg.wangshuangyany.cn

"值: \(b)"
来源：http://pjp.feifeiyinyue.top

[T19] Swift：可选绑定
来源：http://cre.chenlongwang.top

if let n = opt { print(n) }
来源：http://esz.meibo888.top

[T20] Swift：数组操作
来源：http://fdj.zhaomingkeji.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://qnn.tarul.cn

[T21] Swift：遍历
来源：http://ime.0kj1m.cn

for x in a { print(x) }
来源：http://dok.yj202588.top

[T22] Swift：字典
来源：http://rsr.xuanzx.com

var d = ["a": 1];  d["b"] = 2
来源：http://vmp.kuanghao11.cn

[T23] Swift：函数
来源：http://sjc.smart0.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pnr.ctjpmb.com

[T24] Swift：闭包
来源：http://kzi.9152youxi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://uok.snrcjt.cn

[T25] Swift：结构体
来源：http://gwa.aizwys.cn

struct P { var x: Int }
来源：http://ocn.jianghu66.top

[T26] Swift：类与重写
来源：http://imx.nanxinkj.top

class A: Base { override func f() {} }
来源：http://hra.svipenyu.cn

[T27] Swift：错误处理
来源：http://div.zdqjudy.top

do { try f() } catch { print(error) }
来源：http://ltd.nanxinkj.top

[T28] Swift：枚举
来源：http://odg.xuanzx.com

enum Color { case red, green }
来源：http://roo.hongshengwenyu.top

[T29] Swift：guard 提前返回
来源：http://xzi.jianghu66.top

guard let x = opt else { return }
来源：http://ewe.yj20258.top

[T30] Swift：协议
来源：http://why.cheryme.top

protocol Shape { func area() -> Double }
来源：http://ycq.shanyushiyangkeji.top

[T31] Lua：Hello World
来源：http://zeb.nanxuanxn.top

print("Hello")
来源：http://msa.jiagoushi.top

[T32] Lua：局部变量
来源：http://bao.zhijiandao.cn

local a = 1
来源：http://rqb.zhoulong.xyz

[T33] Lua：表（数组）
来源：http://rlv.zhaomingkeji.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://jcw.hywenlv.cn

[T34] Lua：遍历表
来源：http://zlc.sjlbkw.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://vsy.shangyingyoupin.top


<!-- 参考信息 -->