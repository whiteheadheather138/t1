代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mws.xuetiantiany.cn

[R30] 函数返回状态码
来源：http://tgh.xingfuxueyuan.xyz

f() { return 0; }; f || echo "失败了"
来源：http://dvk.aizwys.cn

[R31] 局部变量
来源：http://mcn.tanke756.top

f() { local x=1; echo "$x"; }
来源：http://fjc.yj20258888.top

[R32] 参数个数校验
来源：http://pem.pengpengdd.cyou

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://abz.feifeiyinyue.top

[R33] 捕获错误并提示行号
来源：http://dhp.hywenlv.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://knu.yongpay.top

[R34] 退出时清理
来源：http://ika.sweek.top

trap 'rm -f "$tmp"' EXIT
来源：http://udx.guannengcc.top

[R35] 后台执行并等待
来源：http://uvq.9152youxi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://evt.yonumen.top

[R36] 并发执行多个任务
来源：http://apc.mhx1999.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fkq.nanxuanxn.top

[R37] 把输出赋给变量
来源：http://fik.yuxming.cn

files=$(ls -1)
来源：http://jnj.cdnleiting.top

[R38] 管道串联
来源：http://ufl.yfazqb.com

cat a.txt | grep -i error | wc -l
来源：http://fmg.jlsjyb.cn

[R39] 重定向标准输出与错误
来源：http://zvz.sjlbkw.cn

cmd > out.log 2>&1
来源：http://ftt.chenlongwang.top

[R40] 追加写日志
来源：http://pnw.tian-w.cn

echo "log" >> out.log
来源：http://gag.shanyushiyangkeji.top

[R41] 丢弃输出
来源：http://glc.hywenlv.cn

cmd >/dev/null 2>&1
来源：http://ysu.yueranfly.top

[R42] 输入重定向
来源：http://trz.jinyuanbaomall.cn

wc -l < a.txt
来源：http://ivs.guowangkeji.top

[R43] 按名字查找文件
来源：http://ccn.cucudq.cn

find . -name "*.log" -type f
来源：http://xiy.iojbl.cn

[R44] 按修改时间查找
来源：http://cio.iojbl.cn

find . -mtime -7 -type f
来源：http://naf.jinqigufen.top

[R45] 批量删除
来源：http://kfw.chenzaomai.com

find . -name "*.tmp" -delete
来源：http://zfx.tanke756.top

[R46] 递归替换文件内容
来源：http://yvu.gogol.net.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xhm.hywenlv.cn

[R47] sed 单行替换
来源：http://tgf.zhengqikj.top

sed -i 's/foo/bar/g' a.txt
来源：http://gkp.feifeiyinyue.top

[R48] awk 取指定列
来源：http://ugb.hesvh.cn

awk '{print $1, $3}' a.txt
来源：http://cbe.zhaomingkeji.xyz

[R49] awk 带条件
来源：http://jcp.hesvh.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zvg.vehdjk.com

[R50] awk 求和
来源：http://kjq.gzhubu.top

awk '{s += $2} END {print s}' a.txt
来源：http://pdn.svipenyu.cn

[R51] 排序去重取前几
来源：http://chq.birdmap.top

sort a.txt | uniq -c | sort -rn | head
来源：http://vzy.quarkkingdee.top

[R52] 统计行数
来源：http://yqn.gzhubu.top

wc -l a.txt
来源：http://tgv.jinyuanbaomall.cn

[R53] 查看文件头与实时尾
来源：http://fpp.jinqigufen.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://azx.sweek.top

[R54] 比较两个文件
来源：http://uix.fengsongda.top

diff a.txt b.txt
来源：http://jtn.c1oappe.top

[R55] 压缩与解压
来源：http://prc.hnxiangtu.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tbf.hammf.cn

[R56] 远程拷贝
来源：http://qle.yonumen.top

scp file user@host:/path/
来源：http://jce.jiagoushi.top

[R57] 远程执行命令
来源：http://szc.havefunace.top

ssh user@host 'uptime'
来源：http://swz.tanke756.top

[R58] 下载文件
来源：http://blb.snrcjt.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://djc.daxiang520.top

[R59] 发 POST JSON
来源：http://aqd.sxryk.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pca.xingfuxueyuan.xyz

[R60] 只看 HTTP 状态码
来源：http://mzv.cheryme.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yzi.shzxlz.cn

[R61] 磁盘占用
来源：http://whh.pengpengdd.cyou

df -h;  du -sh *
来源：http://qth.mhx1999.top

[R62] 找最占空间的文件
来源：http://jnb.gzhubu.top

du -ah . | sort -rh | head -10
来源：http://fyl.hammf.cn

[R63] 内存与进程
来源：http://eoz.nanxuanxn.top

free -h;  ps aux | grep nginx
来源：http://ydr.hongshengwenyu.top

[R64] 结束进程
来源：http://uhy.zhengqikj.top

kill -9 $(pgrep -f app.py)
来源：http://lpd.aibaodan.cn

[R65] 查看端口占用
来源：http://syo.jqgufenzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gvp.jqgufenzy.top

[R66] 定时任务
来源：http://rdf.jinqigfzy.top

crontab -e;  crontab -l
来源：http://ght.ivvv.top

[R67] 生成随机十六进制串
来源：http://dvr.ivvv.top

openssl rand -hex 16
来源：http://ymt.snrcjt.cn

[R68] 计算文件校验值
来源：http://mmx.yueranfly.top

sha256sum a.txt;  md5sum a.txt
来源：http://klp.iojbl.cn

[R69] 生成随机密码
来源：http://zrd.yfazqb.com

head -c 16 /dev/urandom | base64
来源：http://rtl.ivvv.top

[R70] 时间戳与互转
来源：http://wcf.quarkkingdee.top

date +%s;  date -d @1700000000
来源：http://adr.zhijiandao.cn

[R71] 日期格式化
来源：http://ybb.birdmap.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://cue.yonumen.top

[R72] 等待端口就绪
来源：http://hjy.c1oappe.top

until nc -z localhost 3306; do sleep 1; done
来源：http://wgj.jqgfzy.top

[R73] 分割大日志
来源：http://ryr.yanxiufei.cn

split -l 1000 big.log part_
来源：http://kyl.jinqigfzy.top

[R74] 批量重命名
来源：http://eis.shanyushiyangkeji.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dno.fanxiaobao.xyz

[R75] 导出环境变量
来源：http://hnk.svipenyu.cn

export PATH="$HOME/bin:$PATH"
来源：http://pky.xylfe.cn

[R76] 使用临时文件
来源：http://pfn.quarkkingdee.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dkx.shanyushiyangkeji.top

[R77] 读取用户输入
来源：http://fck.fanxiaobao.xyz

read -rp "请输入: " ans
来源：http://cpw.quarkkingdee.top

[R78] 交互式菜单
来源：http://lti.fzhhl.top

select opt in a b c; do echo "$opt"; break; done
来源：http://cfa.xuetiantiany.cn

[R79] 解析命令行选项
来源：http://cjw.hesvh.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xdc.fzhhl.top

[R80] 查看脚本执行耗时
来源：http://cdd.nanxinkj.top

time ./run.sh
来源：http://pkv.ppjwa.cn

================================================================================
来源：http://zlh.sjlbkw.cn

S. C / C++ 专题
来源：http://ysr.yueranfly.top

================================================================================
来源：http://khr.dianchejie.cn

[S01] C：Hello World
来源：http://dlb.nanxuanxn.top

#include <stdio.h>
来源：http://amk.tianlin.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://nii.wangdashe.top

[S02] C：变量与格式化输出
来源：http://fao.jinyuanbaomall.cn

int a = 10; printf("%d\n", a);
来源：http://yja.tian-w.cn

[S03] C：读入整数
来源：http://hoc.havefunace.top

int x; scanf("%d", &x);
来源：http://zto.zhijiandao.cn

[S04] C：字符串复制
来源：http://ijw.daria6918.cn

char dst[32]; strcpy(dst, "hi");
来源：http://dvv.pycfn.com

[S05] C：字符串长度
来源：http://hpf.jinyuanbaomall.cn

strlen(s)
来源：http://mhg.bbcook.cn

[S06] C：字符串比较
来源：http://gvm.quarkkingdee.top

strcmp(a, b) == 0
来源：http://ttj.nwbrower.top

[S07] C：数组遍历求和
来源：http://wjy.zhengqikj.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://daj.chenlongwang.top

[S08] C：动态内存分配与释放
来源：http://mad.cucudq.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qfo.pycfn.com

[S09] C：结构体定义与初始化
来源：http://dda.haohaochexian.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://neq.yanxiufei.cn

[S10] C：指针与解引用
来源：http://dlz.bbcook.cn

int *p = &a;  *p = 5;
来源：http://kvt.fehbvm.com

[S11] C：逐行读文件
来源：http://iro.iojbl.cn

FILE *f = fopen("a.txt", "r");
来源：http://cwm.chenzaomai.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://rks.vehdjk.com

fclose(f);
来源：http://gdj.ppjwa.cn

[S12] C：写文件
来源：http://xka.jinqigfzy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vzx.hywenlv.cn

[S13] C：宏定义
来源：http://qkq.aizwys.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tck.tian-w.cn

[S14] C：枚举
来源：http://jee.zhoulong.xyz

enum Color { RED, GREEN, BLUE };
来源：http://gdn.xinyue.icu

[S15] C：类型转换
来源：http://ttp.daria6918.cn

(double) a / b
来源：http://afr.bjfxy.top

[S16] C：位操作置位
来源：http://bit.birdmap.top

x |= (1 << 3);
来源：http://hjz.jinqigufen.top

[S17] C：安全拼接字符串
来源：http://tmi.snrcjt.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wjt.shuidangran.top

[S18] C：命令行参数
来源：http://bjr.bjfxy.top

int main(int argc, char **argv)
来源：http://jnh.fehbvm.com

[S19] C：快速排序
来源：http://ukq.jinqigfzy.top

qsort(a, n, sizeof(int), cmp);
来源：http://sgd.pengpengdd.cyou

[S20] C：二分查找
来源：http://sfk.sufxvd.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://chm.ppjwa.cn

[S21] C：字符类别判断
来源：http://dim.bjfxy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hef.hongshengwenyu.top

[S22] C：字符串转数字
来源：http://nsx.chenzaomai.com

atoi("42");  strtod("3.14", NULL);
来源：http://nth.daria6918.cn

[S23] C：随机数
来源：http://lex.sxryk.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://orl.ydzc1.top

[S24] C：获取本地时间
来源：http://elw.gaohongyu789.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hcp.shanyushiyangkeji.top

[S25] C：内存拷贝
来源：http://qld.yvedp.cn

memcpy(dst, src, n);
来源：http://rrn.snrcjt.cn

[S26] C：内存清零
来源：http://hvj.sxryk.cn

memset(a, 0, sizeof a);
来源：http://njk.xuanzx.com

[S27] C：定义常量
来源：http://eqe.hnqzz.top

const double PI = 3.14159;
来源：http://bur.fengsongda.top

[S28] C：静态变量
来源：http://rit.vehdjk.com

static int counter = 0;
来源：http://sib.zhengqikj.top

[S29] C：变参函数
来源：http://vis.cheryme.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cui.gotoacloud.top

[S30] C：头文件保护
来源：http://krt.cucudq.cn

#ifndef X_H
来源：http://bkc.yfazqb.com

#define X_H
来源：http://ggl.zdbjq.cn

#endif
来源：http://dht.ywan-chungtsiang.top

[S31] C++：Hello World
来源：http://dwz.fzhhl.top

#include <iostream>
来源：http://rqn.gogol.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://iqp.c1oappe.top

[S32] C++：字符串
来源：http://tqc.hnxiangtu.top

std::string s = "hi";  s += "!";
来源：http://oao.daria6918.cn

[S33] C++：vector 增删
来源：http://uyn.yuanzhike.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://eon.jinyuanbaomall.cn

[S34] C++：遍历 vector
来源：http://quh.hesvh.cn

for (auto &x : v) { std::cout << x; }
来源：http://hyn.yvedp.cn

[S35] C++：map
来源：http://ahm.jinyuanbaomall.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ght.gzhubu.top

[S36] C++：unordered_map
来源：http://eqv.redwolf501.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jwq.sufxvd.cn

[S37] C++：set
来源：http://hoc.zhengqikj.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bwm.nwbrower.top

[S38] C++：排序
来源：http://rnx.zhiwuduotai.top

std::sort(v.begin(), v.end());
来源：http://wko.hammf.cn

[S39] C++：自定义比较器排序
来源：http://rhb.tanke756.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://owc.nanxuanxn.top

[S40] C++：查找元素
来源：http://clc.zhixingplan.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hlm.sweek.top

[S41] C++：类与构造函数
来源：http://led.fehbvm.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://imh.vehdjk.com

[S42] C++：继承与虚函数
来源：http://vgp.0kj1m.cn

class B : public Base { public: void f() override {} };
来源：http://oag.pengpengdd.cyou

[S43] C++：智能指针
来源：http://lbp.xingfuxueyuan.xyz

auto p = std::make_unique<int>(5);
来源：http://vpm.cqqwz.cn

[S44] C++：引用传参
来源：http://xom.tarul.cn

void inc(int &x) { ++x; }
来源：http://xih.jinyuanbaomall.cn

[S45] C++：lambda
来源：http://egh.nanxinkj.top

auto add = [](int a, int b) { return a + b; };
来源：http://slr.yangfankeji.com

[S46] C++：函数模板
来源：http://dfu.wangshuangyany.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kxd.yj20258.top

[S47] C++：结构化绑定遍历
来源：http://umu.ehwqpu.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://owy.uphjek.com

[S48] C++：逐行读文件
来源：http://zht.tian-w.cn

std::ifstream in("a.txt");  std::string line;
来源：http://mfa.xinyue.icu

while (std::getline(in, line)) { }
来源：http://unz.zhijiandao.cn

[S49] C++：写文件
来源：http://yvu.fanxiaobao.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kkm.xylfe.cn

[S50] C++：格式化数字
来源：http://tdf.hnxiangtu.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://imd.9152youxi.cn

[S51] C++：显式类型转换
来源：http://kus.shanyushiyangtech.top

static_cast<double>(a) / b
来源：http://uby.ywan-chungtsiang.top

[S52] C++：const 与 noexcept
来源：http://uos.ppjwa.cn

int size() const noexcept { return n_; }
来源：http://amu.sxryk.cn

[S53] C++：移动语义
来源：http://gny.cdnleiting.top

std::vector<int> w = std::move(v);
来源：http://hoe.ehwqpu.com

[S54] C++：异常处理
来源：http://slr.jyoumei.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://brd.zhiwuduotai.top

[S55] C++：结构化绑定
来源：http://mue.zhengqikj.top

auto [a, b] = std::make_pair(1, 2);
来源：http://pdk.shuidangran.top

[S56] C++：optional
来源：http://xqn.hnqzz.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jqg.zhongyouzk.top

[S57] C++：编译期常量
来源：http://dlf.316326.xyz

constexpr int N = 10;
来源：http://ttc.wangdashe.top

[S58] C++：命名空间
来源：http://jpb.cucudq.cn

namespace ns { int f() { return 1; } }
来源：http://rvd.chenzaomai.com

[S59] C++：静态断言
来源：http://hxn.chenzaomai.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hja.hfpthk.cn

[S60] C++：遍历并删除元素
来源：http://yns.dashuyun.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://oti.yfazqb.com

================================================================================
来源：http://nua.feifeiyinyue.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://evq.zdbjq.cn

================================================================================
来源：http://mkr.zhijiandao.cn

[T01] Kotlin：Hello World
来源：http://kvl.vqdsnc.cn

println("Hello")
来源：http://ojo.wangdashe.top

[T02] Kotlin：变量
来源：http://vlb.sufxvd.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tif.ehwqpu.com

[T03] Kotlin：字符串模板
来源：http://cfa.guannengcc.top

"值: $b"
来源：http://mog.quarkkingdee.top

[T04] Kotlin：空安全
来源：http://flh.sweek.top

val n: String? = null;  n?.length
来源：http://tcy.shzxlz.cn

[T05] Kotlin：when 表达式
来源：http://lcb.dianchejie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yks.yuxming.cn

[T06] Kotlin：集合映射
来源：http://nkw.nwbrower.top

listOf(1, 2, 3).map { it * 2 }
来源：http://jqs.xziqi.cn

[T07] Kotlin：集合过滤
来源：http://lkz.xinyue.icu

listOf(1, 2, 3).filter { it > 1 }
来源：http://rxm.yfazqb.com

[T08] Kotlin：数据类
来源：http://xgx.zhoulong.xyz

data class User(val name: String, val age: Int)
来源：http://uyq.ehwqpu.com

[T09] Kotlin：扩展函数
来源：http://jgl.hfpthk.cn

fun String.exclaim() = this + "!"
来源：http://pja.yangfankeji.com

[T10] Kotlin：默认参数
来源：http://ccm.hammf.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://djn.sysykeji.top

[T11] Kotlin：协程
来源：http://xrf.cucudq.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://slw.jyoumei.cn

[T12] Kotlin：解构声明
来源：http://rhe.quarkkingdee.top

val (a, b) = Pair(1, 2)
来源：http://cfy.jinqigufen.top

[T13] Kotlin：只读 Map
来源：http://ime.hcnkem.com

val m = mapOf("a" to 1)
来源：http://kwk.ehwqpu.com

[T14] Kotlin：循环
来源：http://ggp.316326.xyz

for (i in 1..10) println(i)
来源：http://yps.zdqjudy.top

[T15] Kotlin：接口
来源：http://ebk.nwbrower.top

interface Shape { fun area(): Double }
来源：http://jhc.zhaomingkeji.xyz

[T16] Swift：Hello World
来源：http://cdh.fehbvm.com

print("Hello")
来源：http://wnr.uphjek.com

[T17] Swift：变量与常量
来源：http://wks.hammf.cn

var a = 1;  let b = 2
来源：http://byv.jianghu66.top

[T18] Swift：字符串插值
来源：http://bla.hnqzz.top

"值: \(b)"
来源：http://mrn.c1oappe.top

[T19] Swift：可选绑定
来源：http://zem.jinghuilouyu.cn

if let n = opt { print(n) }
来源：http://dhh.fehbvm.com

[T20] Swift：数组操作
来源：http://ogk.zhongyouzk.top

var a = [1, 2, 3];  a.append(4)
来源：http://jhx.aibaodan.cn

[T21] Swift：遍历
来源：http://qyb.meibo888.top

for x in a { print(x) }
来源：http://eax.quarkkingdee.top

[T22] Swift：字典
来源：http://smd.jianghu66.top

var d = ["a": 1];  d["b"] = 2
来源：http://lhh.jinqigfzy.top

[T23] Swift：函数
来源：http://omh.yj20258888.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://skz.xylfe.cn

[T24] Swift：闭包
来源：http://pwr.yj20258888.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://emb.0kj1m.cn

[T25] Swift：结构体
来源：http://xeq.gaohongyu789.top

struct P { var x: Int }
来源：http://vxv.gogol.net.cn

[T26] Swift：类与重写
来源：http://pgx.sjlbkw.cn

class A: Base { override func f() {} }
来源：http://bzr.jinghuilouyu.cn

[T27] Swift：错误处理
来源：http://uue.havefunace.top

do { try f() } catch { print(error) }
来源：http://zzd.zhixingplan.top

[T28] Swift：枚举
来源：http://qgw.yanxiufei.cn

enum Color { case red, green }
来源：http://odk.nanxuanxn.top

[T29] Swift：guard 提前返回
来源：http://sfd.iojbl.cn

guard let x = opt else { return }
来源：http://ylw.feifeiyinyue.top

[T30] Swift：协议
来源：http://mjx.yanxiufei.cn

protocol Shape { func area() -> Double }
来源：http://qsc.daria6918.cn

[T31] Lua：Hello World
来源：http://cuv.cashguo.top

print("Hello")
来源：http://feg.52xcode.cn

[T32] Lua：局部变量
来源：http://gnc.fengsongda.top

local a = 1
来源：http://zor.sjlbkw.cn


<!-- 参考信息 -->