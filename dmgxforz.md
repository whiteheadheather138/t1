代发 wailian999

echo "${#s}"
来源：http://goh.9152youxi.cn

[R22] 截取子串
来源：http://cnf.quarkkingdee.top

echo "${s:0:5}"
来源：http://vak.gzhubu.top

[R23] 字符串替换
来源：http://bjn.hammf.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mcj.sjlbkw.cn

[R24] 大小写转换
来源：http://aon.hywenlv.cn

echo "${s^^}"; echo "${s,,}"
来源：http://vvy.gaohongyu789.top

[R25] 去后缀 / 去前缀
来源：http://qcz.jlsjyb.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://pox.hfpthk.cn

[R26] 命令替换
来源：http://enn.hcnkem.com

now=$(date +%F); echo "$now"
来源：http://seg.fktsv.cn

[R27] 算术展开
来源：http://nzb.shangyingyoupin.top

echo $((1 + 2 * 3))
来源：http://mcb.shangyingyoupin.top

[R28] 浮点运算
来源：http://fav.bbcook.cn

echo "scale=2; 10/3" | bc
来源：http://oen.iojbl.cn

[R29] 定义函数
来源：http://sas.ppjwa.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bbo.daxiang520.top

[R30] 函数返回状态码
来源：http://gzo.haohaochexian.top

f() { return 0; }; f || echo "失败了"
来源：http://tjd.zhengqikj.top

[R31] 局部变量
来源：http://ind.sufxvd.cn

f() { local x=1; echo "$x"; }
来源：http://qhl.chenjidiqi.icu

[R32] 参数个数校验
来源：http://gxv.jiagoushi.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ejx.zhixingplan.top

[R33] 捕获错误并提示行号
来源：http://bjs.cheryme.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rvt.xuetiantiany.cn

[R34] 退出时清理
来源：http://amw.vqdsnc.cn

trap 'rm -f "$tmp"' EXIT
来源：http://car.haohaochexian.top

[R35] 后台执行并等待
来源：http://wci.sweek.top

sleep 5 & pid=$!; wait "$pid"
来源：http://cfa.xylfe.cn

[R36] 并发执行多个任务
来源：http://yxn.zdbjq.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mzf.shanyushiyangtech.top

[R37] 把输出赋给变量
来源：http://rnx.jqgfzy.top

files=$(ls -1)
来源：http://ccl.hcnkem.com

[R38] 管道串联
来源：http://jua.sweek.top

cat a.txt | grep -i error | wc -l
来源：http://njh.jiagoushi.top

[R39] 重定向标准输出与错误
来源：http://org.jianghu66.top

cmd > out.log 2>&1
来源：http://ubk.hysaishi.cn

[R40] 追加写日志
来源：http://yqe.hnqzz.top

echo "log" >> out.log
来源：http://hoz.zhaomingkeji.xyz

[R41] 丢弃输出
来源：http://dnn.cashguo.top

cmd >/dev/null 2>&1
来源：http://brq.ywan-chungtsiang.top

[R42] 输入重定向
来源：http://qgg.dashuyun.cn

wc -l < a.txt
来源：http://dnv.xuanzx.com

[R43] 按名字查找文件
来源：http://xsm.316326.xyz

find . -name "*.log" -type f
来源：http://hgy.fengsongda.top

[R44] 按修改时间查找
来源：http://ktd.yvedp.cn

find . -mtime -7 -type f
来源：http://htw.mhx1999.top

[R45] 批量删除
来源：http://wed.fanxiaobao.xyz

find . -name "*.tmp" -delete
来源：http://jia.kuanghao11.cn

[R46] 递归替换文件内容
来源：http://wet.haohaochexian.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rhq.aibaodan.cn

[R47] sed 单行替换
来源：http://svf.zhijiandao.cn

sed -i 's/foo/bar/g' a.txt
来源：http://kgl.jiagoushi.top

[R48] awk 取指定列
来源：http://pkq.sjlbkw.cn

awk '{print $1, $3}' a.txt
来源：http://nka.gotoacloud.top

[R49] awk 带条件
来源：http://eau.0kj1m.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://aex.xuanzx.com

[R50] awk 求和
来源：http://grr.zhengqikj.top

awk '{s += $2} END {print s}' a.txt
来源：http://jmy.0kj1m.cn

[R51] 排序去重取前几
来源：http://ewz.sufxvd.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://thw.daria6918.cn

[R52] 统计行数
来源：http://wax.gotoacloud.top

wc -l a.txt
来源：http://qsy.hnxiangtu.top

[R53] 查看文件头与实时尾
来源：http://xwc.tianlin.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kfk.tianlin.xyz

[R54] 比较两个文件
来源：http://moz.nanxinkj.top

diff a.txt b.txt
来源：http://bxa.ppjwa.cn

[R55] 压缩与解压
来源：http://efx.yueranfly.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hzu.zhengqikj.top

[R56] 远程拷贝
来源：http://evq.316326.xyz

scp file user@host:/path/
来源：http://bln.yuxming.cn

[R57] 远程执行命令
来源：http://agj.jqgfzy.top

ssh user@host 'uptime'
来源：http://cxl.sjlbkw.cn

[R58] 下载文件
来源：http://mtd.ywan-chungtsiang.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://btb.sweek.top

[R59] 发 POST JSON
来源：http://zbz.yj20258.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jrs.shzxlz.cn

[R60] 只看 HTTP 状态码
来源：http://pti.vqdsnc.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://onv.kuanghao11.cn

[R61] 磁盘占用
来源：http://skt.vqdsnc.cn

df -h;  du -sh *
来源：http://dty.zdbjq.cn

[R62] 找最占空间的文件
来源：http://dtd.yueranfly.top

du -ah . | sort -rh | head -10
来源：http://prk.fengsongda.top

[R63] 内存与进程
来源：http://qmn.feifeiyinyue.top

free -h;  ps aux | grep nginx
来源：http://pbc.jinqigfzy.top

[R64] 结束进程
来源：http://tyu.ydzc1.top

kill -9 $(pgrep -f app.py)
来源：http://yga.zdbjq.cn

[R65] 查看端口占用
来源：http://tna.yueranfly.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cqg.chenjidiqi.icu

[R66] 定时任务
来源：http://yfp.fehbvm.com

crontab -e;  crontab -l
来源：http://vzw.quarkkingdee.top

[R67] 生成随机十六进制串
来源：http://hkm.epnwcf.com

openssl rand -hex 16
来源：http://njw.hesvh.cn

[R68] 计算文件校验值
来源：http://trz.pengpengdd.cyou

sha256sum a.txt;  md5sum a.txt
来源：http://koj.jinqigfzy.top

[R69] 生成随机密码
来源：http://mqu.snrcjt.cn

head -c 16 /dev/urandom | base64
来源：http://cqe.vqdsnc.cn

[R70] 时间戳与互转
来源：http://irl.tanke756.top

date +%s;  date -d @1700000000
来源：http://fjv.sufxvd.cn

[R71] 日期格式化
来源：http://nrt.yvedp.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ffe.nanxinkj.top

[R72] 等待端口就绪
来源：http://wmh.xingfuxueyuan.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://lzi.yfazqb.com

[R73] 分割大日志
来源：http://iuc.9152youxi.cn

split -l 1000 big.log part_
来源：http://epe.tianlin.xyz

[R74] 批量重命名
来源：http://zau.hesvh.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://afa.hnxiangtu.top

[R75] 导出环境变量
来源：http://ekt.yangfankeji.com

export PATH="$HOME/bin:$PATH"
来源：http://uyt.316326.xyz

[R76] 使用临时文件
来源：http://eka.zhiwuduotai.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pbm.guannengcc.top

[R77] 读取用户输入
来源：http://mbr.gaohongyu789.top

read -rp "请输入: " ans
来源：http://wwk.sufxvd.cn

[R78] 交互式菜单
来源：http://erl.jianghu66.top

select opt in a b c; do echo "$opt"; break; done
来源：http://juj.chenlongwang.top

[R79] 解析命令行选项
来源：http://zef.meibo888.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ltp.jyoumei.cn

[R80] 查看脚本执行耗时
来源：http://hij.sxryk.cn

time ./run.sh
来源：http://gud.tianlin.xyz

================================================================================
来源：http://mwf.xuetiantiany.cn

S. C / C++ 专题
来源：http://luq.hnxiangtu.top

================================================================================
来源：http://dmn.nanxinkj.top

[S01] C：Hello World
来源：http://gpx.gaohongyu789.top

#include <stdio.h>
来源：http://qgu.tianlin.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://xlg.yangfankeji.com

[S02] C：变量与格式化输出
来源：http://njl.hfpthk.cn

int a = 10; printf("%d\n", a);
来源：http://npo.uphjek.com

[S03] C：读入整数
来源：http://jtf.zycfv.cn

int x; scanf("%d", &x);
来源：http://iad.kuanghao11.cn

[S04] C：字符串复制
来源：http://ypj.jqgfzy.top

char dst[32]; strcpy(dst, "hi");
来源：http://ycn.jlsjyb.cn

[S05] C：字符串长度
来源：http://ucg.xuetiantiany.cn

strlen(s)
来源：http://eaj.shzxlz.cn

[S06] C：字符串比较
来源：http://ajx.shanyushiyangtech.top

strcmp(a, b) == 0
来源：http://ybh.zycfv.cn

[S07] C：数组遍历求和
来源：http://zqw.vqdsnc.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nso.xuanzx.com

[S08] C：动态内存分配与释放
来源：http://ajp.ydjk.org.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vjr.52xcode.cn

[S09] C：结构体定义与初始化
来源：http://jmw.hcnkem.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yuc.jianghu66.top

[S10] C：指针与解引用
来源：http://akb.cucudq.cn

int *p = &a;  *p = 5;
来源：http://rdd.feifeiyinyue.top

[S11] C：逐行读文件
来源：http://smk.gaohongyu789.top

FILE *f = fopen("a.txt", "r");
来源：http://ujl.kuanghao11.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://kea.hnqzz.top

fclose(f);
来源：http://fug.jyoumei.cn

[S12] C：写文件
来源：http://ylu.daxiang520.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://atb.ydzc1.top

[S13] C：宏定义
来源：http://axr.chenjidiqi.icu

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pyg.hfpthk.cn

[S14] C：枚举
来源：http://ywk.fzhhl.top

enum Color { RED, GREEN, BLUE };
来源：http://mps.feifeiyinyue.top

[S15] C：类型转换
来源：http://fuh.aizwys.cn

(double) a / b
来源：http://rjz.zhongyouzk.top

[S16] C：位操作置位
来源：http://xwh.zhoulong.xyz

x |= (1 << 3);
来源：http://djn.guowangkeji.top

[S17] C：安全拼接字符串
来源：http://zuz.xinyue.icu

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lxd.jiagoushi.top

[S18] C：命令行参数
来源：http://qbt.hcnkem.com

int main(int argc, char **argv)
来源：http://zja.dashuyun.cn

[S19] C：快速排序
来源：http://yhb.bbcook.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ccr.sysykeji.top

[S20] C：二分查找
来源：http://ppu.meibo888.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://aoy.uphjek.com

[S21] C：字符类别判断
来源：http://kfn.ydjk.org.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://quw.tarul.cn

[S22] C：字符串转数字
来源：http://shm.xziqi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wou.chenjidiqi.icu

[S23] C：随机数
来源：http://tdx.fengsongda.top

srand(time(NULL));  int r = rand() % 100;
来源：http://kcr.zycfv.cn

[S24] C：获取本地时间
来源：http://ijt.316326.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bak.zhixingplan.top

[S25] C：内存拷贝
来源：http://bwt.zhongyouzk.top

memcpy(dst, src, n);
来源：http://avt.ydzc1.top

[S26] C：内存清零
来源：http://jyb.zycfv.cn

memset(a, 0, sizeof a);
来源：http://hrv.fanxiaobao.xyz

[S27] C：定义常量
来源：http://klt.xingfuxueyuan.xyz

const double PI = 3.14159;
来源：http://mtp.wangdashe.top

[S28] C：静态变量
来源：http://rzd.yanxiufei.cn

static int counter = 0;
来源：http://pbn.havefunace.top

[S29] C：变参函数
来源：http://spn.ehwqpu.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jbt.jinghuilouyu.cn

[S30] C：头文件保护
来源：http://rkx.sufxvd.cn

#ifndef X_H
来源：http://rxu.epnwcf.com

#define X_H
来源：http://lrl.haohaochexian.top

#endif
来源：http://sds.mhx1999.top

[S31] C++：Hello World
来源：http://jzm.jyoumei.cn

#include <iostream>
来源：http://sbk.jyoumei.cn

int main() { std::cout << "Hello\n"; }
来源：http://ypw.xziqi.cn

[S32] C++：字符串
来源：http://byd.andypj.xyz

std::string s = "hi";  s += "!";
来源：http://ude.aizwys.cn

[S33] C++：vector 增删
来源：http://kah.yuxming.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yhv.jinqigfzy.top

[S34] C++：遍历 vector
来源：http://kej.daria6918.cn

for (auto &x : v) { std::cout << x; }
来源：http://mnr.xuetiantiany.cn

[S35] C++：map
来源：http://tvf.nanxuanxn.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qfa.zycfv.cn

[S36] C++：unordered_map
来源：http://bja.havefunace.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wai.nanxuanxn.top

[S37] C++：set
来源：http://jsd.sysykeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lav.c1oappe.top

[S38] C++：排序
来源：http://yxo.52xcode.cn

std::sort(v.begin(), v.end());
来源：http://pyg.c1oappe.top

[S39] C++：自定义比较器排序
来源：http://har.smart0.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dnj.tanke756.top

[S40] C++：查找元素
来源：http://rrv.hnxiangtu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vhg.dianchejie.cn

[S41] C++：类与构造函数
来源：http://ihd.fanxiaobao.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nqy.fanxiaobao.xyz

[S42] C++：继承与虚函数
来源：http://uqm.xziqi.cn

class B : public Base { public: void f() override {} };
来源：http://oju.epnwcf.com

[S43] C++：智能指针
来源：http://xow.redwolf501.top

auto p = std::make_unique<int>(5);
来源：http://xnd.shanyushiyangkeji.top

[S44] C++：引用传参
来源：http://zbp.bjfxy.top

void inc(int &x) { ++x; }
来源：http://rit.0kj1m.cn

[S45] C++：lambda
来源：http://dlm.snrcjt.cn

auto add = [](int a, int b) { return a + b; };
来源：http://jak.sysykeji.top

[S46] C++：函数模板
来源：http://feh.cashguo.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lyu.aizwys.cn

[S47] C++：结构化绑定遍历
来源：http://hfv.iojbl.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wkx.hnqzz.top

[S48] C++：逐行读文件
来源：http://jqk.smart0.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://rbr.shanyushiyangkeji.top

while (std::getline(in, line)) { }
来源：http://wal.zhoulong.xyz

[S49] C++：写文件
来源：http://zte.sufxvd.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bze.andypj.xyz

[S50] C++：格式化数字
来源：http://iwj.nwbrower.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mxd.kuanghao11.cn

[S51] C++：显式类型转换
来源：http://cth.shangyingyoupin.top

static_cast<double>(a) / b
来源：http://upi.cdnleiting.top

[S52] C++：const 与 noexcept
来源：http://dov.ctjpmb.com

int size() const noexcept { return n_; }
来源：http://ndw.pengpengdd.cyou

[S53] C++：移动语义
来源：http://bzx.uphjek.com

std::vector<int> w = std::move(v);
来源：http://fue.cucudq.cn

[S54] C++：异常处理
来源：http://txz.sysykeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mgp.xuanzx.com

[S55] C++：结构化绑定
来源：http://tni.daria6918.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://avx.fktsv.cn

[S56] C++：optional
来源：http://chq.316326.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gmo.sxryk.cn

[S57] C++：编译期常量
来源：http://sre.mhx1999.top

constexpr int N = 10;
来源：http://ckf.hnqzz.top

[S58] C++：命名空间
来源：http://egc.xziqi.cn

namespace ns { int f() { return 1; } }
来源：http://jlk.cucudq.cn

[S59] C++：静态断言
来源：http://qwl.sweek.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dmk.cheryme.top

[S60] C++：遍历并删除元素
来源：http://hoo.yj202588.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pbg.bbcook.cn

================================================================================
来源：http://ktf.fengsongda.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fdy.zhengqikj.top

================================================================================
来源：http://ikz.jiagoushi.top

[T01] Kotlin：Hello World
来源：http://btu.zdqjudy.top

println("Hello")
来源：http://jpx.gogol.net.cn

[T02] Kotlin：变量
来源：http://vsc.chenlongwang.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tel.pycfn.com

[T03] Kotlin：字符串模板
来源：http://scj.yj20258.top

"值: $b"
来源：http://fkd.nwbrower.top

[T04] Kotlin：空安全
来源：http://nez.ywan-chungtsiang.top

val n: String? = null;  n?.length
来源：http://zos.guowangkeji.top

[T05] Kotlin：when 表达式
来源：http://wla.yj20258.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lvg.gzhubu.top

[T06] Kotlin：集合映射
来源：http://uky.sufxvd.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ayj.hfpthk.cn

[T07] Kotlin：集合过滤
来源：http://dwp.fktsv.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ngk.shanyushiyangkeji.top

[T08] Kotlin：数据类
来源：http://vug.jinqigfzy.top

data class User(val name: String, val age: Int)
来源：http://wgi.ydzc1.top

[T09] Kotlin：扩展函数
来源：http://heh.jqgfzy.top

fun String.exclaim() = this + "!"
来源：http://lne.snrcjt.cn

[T10] Kotlin：默认参数
来源：http://qqu.jqgufenzy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://swr.hnxiangtu.top

[T11] Kotlin：协程
来源：http://zlc.quarkkingdee.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://bdq.nwbrower.top

[T12] Kotlin：解构声明
来源：http://lkq.zhiwuduotai.top

val (a, b) = Pair(1, 2)
来源：http://szh.xinyue.icu

[T13] Kotlin：只读 Map
来源：http://bji.xinyue.icu

val m = mapOf("a" to 1)
来源：http://zwv.svipenyu.cn

[T14] Kotlin：循环
来源：http://lce.jlsjyb.cn

for (i in 1..10) println(i)
来源：http://ryd.cheryme.top

[T15] Kotlin：接口
来源：http://vun.jiagoushi.top

interface Shape { fun area(): Double }
来源：http://dmq.nwbrower.top

[T16] Swift：Hello World
来源：http://dhk.aibaodan.cn

print("Hello")
来源：http://tzm.sufxvd.cn

[T17] Swift：变量与常量
来源：http://yho.mhx1999.top

var a = 1;  let b = 2
来源：http://qve.chenzaomai.com

[T18] Swift：字符串插值
来源：http://uxj.yuanzhike.top

"值: \(b)"
来源：http://rvn.fengsongda.top

[T19] Swift：可选绑定
来源：http://yto.jqgfzy.top

if let n = opt { print(n) }
来源：http://qqs.snrcjt.cn

[T20] Swift：数组操作
来源：http://yco.9152youxi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zzi.jianghu66.top

[T21] Swift：遍历
来源：http://xuc.ybcxt.top

for x in a { print(x) }
来源：http://bsc.mhx1999.top

[T22] Swift：字典
来源：http://mqw.xylfe.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zus.gzhubu.top

[T23] Swift：函数
来源：http://eic.meibo888.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cma.52xcode.cn

[T24] Swift：闭包
来源：http://hku.ivvv.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://lxg.jinghuilouyu.cn


<!-- 参考信息 -->