代发 wailian999

echo "${#s}"
来源：http://scd.cqqwz.cn

[R22] 截取子串
来源：http://vhp.ybcxt.top

echo "${s:0:5}"
来源：http://ncj.hysaishi.cn

[R23] 字符串替换
来源：http://lht.yj20258.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nes.ppjwa.cn

[R24] 大小写转换
来源：http://gty.xylfe.cn

echo "${s^^}"; echo "${s,,}"
来源：http://moi.chenjidiqi.icu

[R25] 去后缀 / 去前缀
来源：http://nmb.bjfxy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ssv.zhaomingkeji.xyz

[R26] 命令替换
来源：http://ybd.zhijiandao.cn

now=$(date +%F); echo "$now"
来源：http://zkg.tanke756.top

[R27] 算术展开
来源：http://vsl.mhx1999.top

echo $((1 + 2 * 3))
来源：http://ree.mhx1999.top

[R28] 浮点运算
来源：http://nzt.chenjidiqi.icu

echo "scale=2; 10/3" | bc
来源：http://kvj.cashguo.top

[R29] 定义函数
来源：http://anb.birdmap.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wrs.shanyushiyangtech.top

[R30] 函数返回状态码
来源：http://lyw.yueranfly.top

f() { return 0; }; f || echo "失败了"
来源：http://sip.zhiwuduotai.top

[R31] 局部变量
来源：http://sau.gaohongyu789.top

f() { local x=1; echo "$x"; }
来源：http://ava.wangdashe.top

[R32] 参数个数校验
来源：http://evy.sysykeji.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qna.chenjidiqi.icu

[R33] 捕获错误并提示行号
来源：http://wwm.wangdashe.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fnt.guowangkeji.top

[R34] 退出时清理
来源：http://whq.andypj.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://uwu.jianghu66.top

[R35] 后台执行并等待
来源：http://taj.9152youxi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ndu.gogol.net.cn

[R36] 并发执行多个任务
来源：http://frf.redwolf501.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hza.uphjek.com

[R37] 把输出赋给变量
来源：http://fap.hywenlv.cn

files=$(ls -1)
来源：http://dya.shuidangran.top

[R38] 管道串联
来源：http://owq.zhiwuduotai.top

cat a.txt | grep -i error | wc -l
来源：http://juq.ybcxt.top

[R39] 重定向标准输出与错误
来源：http://oaj.hcnkem.com

cmd > out.log 2>&1
来源：http://etd.haohaochexian.top

[R40] 追加写日志
来源：http://imf.bjfxy.top

echo "log" >> out.log
来源：http://iyg.havefunace.top

[R41] 丢弃输出
来源：http://wpf.tarul.cn

cmd >/dev/null 2>&1
来源：http://dxs.chenjidiqi.icu

[R42] 输入重定向
来源：http://nfd.xinyue.icu

wc -l < a.txt
来源：http://grt.yfazqb.com

[R43] 按名字查找文件
来源：http://lhp.andypj.xyz

find . -name "*.log" -type f
来源：http://ogn.hysaishi.cn

[R44] 按修改时间查找
来源：http://pny.xingfuxueyuan.xyz

find . -mtime -7 -type f
来源：http://lbg.bjfxy.top

[R45] 批量删除
来源：http://gei.sweek.top

find . -name "*.tmp" -delete
来源：http://kjo.c1oappe.top

[R46] 递归替换文件内容
来源：http://moe.hywenlv.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://irw.9152youxi.cn

[R47] sed 单行替换
来源：http://tje.yfazqb.com

sed -i 's/foo/bar/g' a.txt
来源：http://agi.fzhhl.top

[R48] awk 取指定列
来源：http://ozq.chenjidiqi.icu

awk '{print $1, $3}' a.txt
来源：http://unq.zhoulong.xyz

[R49] awk 带条件
来源：http://sun.0kj1m.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://erp.uphjek.com

[R50] awk 求和
来源：http://jmr.jinqigufen.top

awk '{s += $2} END {print s}' a.txt
来源：http://pmv.cdnleiting.top

[R51] 排序去重取前几
来源：http://ywt.jyoumei.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://uzt.jiagoushi.top

[R52] 统计行数
来源：http://hpk.xziqi.cn

wc -l a.txt
来源：http://byw.shzxlz.cn

[R53] 查看文件头与实时尾
来源：http://wmj.zhijiandao.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bwp.jinghuilouyu.cn

[R54] 比较两个文件
来源：http://dpx.yvedp.cn

diff a.txt b.txt
来源：http://ujp.nanxinkj.top

[R55] 压缩与解压
来源：http://zoi.yuxming.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://brq.sjlbkw.cn

[R56] 远程拷贝
来源：http://ekc.zhijiandao.cn

scp file user@host:/path/
来源：http://dlq.zhengqikj.top

[R57] 远程执行命令
来源：http://zuw.yueranfly.top

ssh user@host 'uptime'
来源：http://uyf.zhijiandao.cn

[R58] 下载文件
来源：http://sst.svipenyu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pfw.xinyue.icu

[R59] 发 POST JSON
来源：http://bss.tarul.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://afq.daxiang520.top

[R60] 只看 HTTP 状态码
来源：http://mmy.sjlbkw.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xts.yuanzhike.top

[R61] 磁盘占用
来源：http://gdx.jqgufenzy.top

df -h;  du -sh *
来源：http://hik.tanke756.top

[R62] 找最占空间的文件
来源：http://gsx.jlsjyb.cn

du -ah . | sort -rh | head -10
来源：http://scm.yangfankeji.com

[R63] 内存与进程
来源：http://bax.mhx1999.top

free -h;  ps aux | grep nginx
来源：http://szx.fanxiaobao.xyz

[R64] 结束进程
来源：http://srd.svipenyu.cn

kill -9 $(pgrep -f app.py)
来源：http://omp.hesvh.cn

[R65] 查看端口占用
来源：http://umb.sjlbkw.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ysg.zycfv.cn

[R66] 定时任务
来源：http://uqm.zhiwuduotai.top

crontab -e;  crontab -l
来源：http://eso.9152youxi.cn

[R67] 生成随机十六进制串
来源：http://ljp.zdbjq.cn

openssl rand -hex 16
来源：http://ovv.svipenyu.cn

[R68] 计算文件校验值
来源：http://puu.jinqigfzy.top

sha256sum a.txt;  md5sum a.txt
来源：http://xph.xylfe.cn

[R69] 生成随机密码
来源：http://dte.ywan-chungtsiang.top

head -c 16 /dev/urandom | base64
来源：http://olv.hammf.cn

[R70] 时间戳与互转
来源：http://kku.ivvv.top

date +%s;  date -d @1700000000
来源：http://bzl.hesvh.cn

[R71] 日期格式化
来源：http://psn.meibo888.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ggw.tian-w.cn

[R72] 等待端口就绪
来源：http://mxo.sysykeji.top

until nc -z localhost 3306; do sleep 1; done
来源：http://xxz.hnxiangtu.top

[R73] 分割大日志
来源：http://yze.yuanzhike.top

split -l 1000 big.log part_
来源：http://hdt.yj202588.top

[R74] 批量重命名
来源：http://trq.aizwys.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lpj.mhx1999.top

[R75] 导出环境变量
来源：http://ueq.yj202588.top

export PATH="$HOME/bin:$PATH"
来源：http://ozk.jinyuanbaomall.cn

[R76] 使用临时文件
来源：http://gnd.daria6918.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://uix.ydjk.org.cn

[R77] 读取用户输入
来源：http://thw.chenlongwang.top

read -rp "请输入: " ans
来源：http://nai.hcnkem.com

[R78] 交互式菜单
来源：http://syk.zdbjq.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://kht.gaohongyu789.top

[R79] 解析命令行选项
来源：http://vlo.iojbl.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tjw.ctjpmb.com

[R80] 查看脚本执行耗时
来源：http://ubi.daria6918.cn

time ./run.sh
来源：http://zmg.chenjidiqi.icu

================================================================================
来源：http://ctu.fktsv.cn

S. C / C++ 专题
来源：http://bbn.jyoumei.cn

================================================================================
来源：http://aoo.mhx1999.top

[S01] C：Hello World
来源：http://yqa.vehdjk.com

#include <stdio.h>
来源：http://fzf.guannengcc.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://vso.sufxvd.cn

[S02] C：变量与格式化输出
来源：http://yqz.fzhhl.top

int a = 10; printf("%d\n", a);
来源：http://vdd.zhongyouzk.top

[S03] C：读入整数
来源：http://zec.yueranfly.top

int x; scanf("%d", &x);
来源：http://gzt.bjfxy.top

[S04] C：字符串复制
来源：http://csn.ppjwa.cn

char dst[32]; strcpy(dst, "hi");
来源：http://pst.zhengqikj.top

[S05] C：字符串长度
来源：http://jvu.daria6918.cn

strlen(s)
来源：http://qpz.zhoulong.xyz

[S06] C：字符串比较
来源：http://gau.vqdsnc.cn

strcmp(a, b) == 0
来源：http://epy.yueranfly.top

[S07] C：数组遍历求和
来源：http://xpr.ydzc1.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zpc.xziqi.cn

[S08] C：动态内存分配与释放
来源：http://nti.zhiwuduotai.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://itw.xylfe.cn

[S09] C：结构体定义与初始化
来源：http://ilm.c1oappe.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nsy.shanyushiyangkeji.top

[S10] C：指针与解引用
来源：http://atj.daxiang520.top

int *p = &a;  *p = 5;
来源：http://zmm.kuanghao11.cn

[S11] C：逐行读文件
来源：http://xrh.iojbl.cn

FILE *f = fopen("a.txt", "r");
来源：http://pfh.hcnkem.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://odm.zdbjq.cn

fclose(f);
来源：http://nji.epnwcf.com

[S12] C：写文件
来源：http://psn.hfpthk.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zxs.shangyingyoupin.top

[S13] C：宏定义
来源：http://kcn.quarkkingdee.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nim.yongpay.top

[S14] C：枚举
来源：http://emo.xingfuxueyuan.xyz

enum Color { RED, GREEN, BLUE };
来源：http://aen.svipenyu.cn

[S15] C：类型转换
来源：http://far.9152youxi.cn

(double) a / b
来源：http://ebd.jqgfzy.top

[S16] C：位操作置位
来源：http://vbx.zhongyouzk.top

x |= (1 << 3);
来源：http://spo.shangyingyoupin.top

[S17] C：安全拼接字符串
来源：http://xxw.cheryme.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mtf.hywenlv.cn

[S18] C：命令行参数
来源：http://vxg.gaohongyu789.top

int main(int argc, char **argv)
来源：http://pfd.cucudq.cn

[S19] C：快速排序
来源：http://yzm.chenzaomai.com

qsort(a, n, sizeof(int), cmp);
来源：http://tqe.jqgufenzy.top

[S20] C：二分查找
来源：http://xft.yj20258.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nwx.kuanghao11.cn

[S21] C：字符类别判断
来源：http://cvg.yangfankeji.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ksg.ivvv.top

[S22] C：字符串转数字
来源：http://sjw.zhijiandao.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ctl.redwolf501.top

[S23] C：随机数
来源：http://rzv.sxryk.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://udj.snrcjt.cn

[S24] C：获取本地时间
来源：http://lwj.feifeiyinyue.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kwj.hywenlv.cn

[S25] C：内存拷贝
来源：http://umz.vqdsnc.cn

memcpy(dst, src, n);
来源：http://nnn.cucudq.cn

[S26] C：内存清零
来源：http://nkh.quarkkingdee.top

memset(a, 0, sizeof a);
来源：http://gnz.sweek.top

[S27] C：定义常量
来源：http://oae.c1oappe.top

const double PI = 3.14159;
来源：http://awa.tanke756.top

[S28] C：静态变量
来源：http://vao.yuxming.cn

static int counter = 0;
来源：http://vzx.hysaishi.cn

[S29] C：变参函数
来源：http://xol.gzhubu.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fua.meibo888.top

[S30] C：头文件保护
来源：http://lza.zhengqikj.top

#ifndef X_H
来源：http://qtb.xingfuxueyuan.xyz

#define X_H
来源：http://pdr.ywan-chungtsiang.top

#endif
来源：http://gwr.hywenlv.cn

[S31] C++：Hello World
来源：http://gxm.kuanghao11.cn

#include <iostream>
来源：http://jsi.hammf.cn

int main() { std::cout << "Hello\n"; }
来源：http://dpw.bbcook.cn

[S32] C++：字符串
来源：http://rqv.jinqigufen.top

std::string s = "hi";  s += "!";
来源：http://vdx.vqdsnc.cn

[S33] C++：vector 增删
来源：http://xxr.zdqjudy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cpv.birdmap.top

[S34] C++：遍历 vector
来源：http://mjx.redwolf501.top

for (auto &x : v) { std::cout << x; }
来源：http://meq.ywan-chungtsiang.top

[S35] C++：map
来源：http://qqe.316326.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ozv.daria6918.cn

[S36] C++：unordered_map
来源：http://ixe.jiagoushi.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ahh.xingfuxueyuan.xyz

[S37] C++：set
来源：http://aea.chenzaomai.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pvj.guannengcc.top

[S38] C++：排序
来源：http://maw.andypj.xyz

std::sort(v.begin(), v.end());
来源：http://hpf.yfazqb.com

[S39] C++：自定义比较器排序
来源：http://eel.cucudq.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://oye.snrcjt.cn

[S40] C++：查找元素
来源：http://soc.fzhhl.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yym.sufxvd.cn

[S41] C++：类与构造函数
来源：http://vss.zhiwuduotai.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zvz.hysaishi.cn

[S42] C++：继承与虚函数
来源：http://ynt.aizwys.cn

class B : public Base { public: void f() override {} };
来源：http://wdn.kuanghao11.cn

[S43] C++：智能指针
来源：http://ckp.ybcxt.top

auto p = std::make_unique<int>(5);
来源：http://rdq.xingfuxueyuan.xyz

[S44] C++：引用传参
来源：http://jtj.gaohongyu789.top

void inc(int &x) { ++x; }
来源：http://epv.xinyue.icu

[S45] C++：lambda
来源：http://iey.ivvv.top

auto add = [](int a, int b) { return a + b; };
来源：http://kjx.hfpthk.cn

[S46] C++：函数模板
来源：http://ofe.feifeiyinyue.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ytv.daxiang520.top

[S47] C++：结构化绑定遍历
来源：http://vao.uphjek.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qsh.andypj.xyz

[S48] C++：逐行读文件
来源：http://pcq.yj20258888.top

std::ifstream in("a.txt");  std::string line;
来源：http://wpl.zycfv.cn

while (std::getline(in, line)) { }
来源：http://vdm.0kj1m.cn

[S49] C++：写文件
来源：http://crh.52xcode.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dsj.vqdsnc.cn

[S50] C++：格式化数字
来源：http://avv.yj202588.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zrc.ehwqpu.com

[S51] C++：显式类型转换
来源：http://noz.gaohongyu789.top

static_cast<double>(a) / b
来源：http://vtf.wangdashe.top

[S52] C++：const 与 noexcept
来源：http://obr.fehbvm.com

int size() const noexcept { return n_; }
来源：http://lxw.yj20258888.top

[S53] C++：移动语义
来源：http://por.svipenyu.cn

std::vector<int> w = std::move(v);
来源：http://qok.chenjidiqi.icu

[S54] C++：异常处理
来源：http://oxj.xingfuxueyuan.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://npn.zdqjudy.top

[S55] C++：结构化绑定
来源：http://qup.0kj1m.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://lcb.shanyushiyangkeji.top

[S56] C++：optional
来源：http://qym.aibaodan.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://buh.xylfe.cn

[S57] C++：编译期常量
来源：http://ubf.pycfn.com

constexpr int N = 10;
来源：http://gmh.hysaishi.cn

[S58] C++：命名空间
来源：http://ypu.dashuyun.cn

namespace ns { int f() { return 1; } }
来源：http://gkp.wangshuangyany.cn

[S59] C++：静态断言
来源：http://fbd.vehdjk.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lad.hnxiangtu.top

[S60] C++：遍历并删除元素
来源：http://yiy.meibo888.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rwv.pengpengdd.cyou

================================================================================
来源：http://mya.cheryme.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ycx.ppjwa.cn

================================================================================
来源：http://rfn.dashuyun.cn

[T01] Kotlin：Hello World
来源：http://zmk.ehwqpu.com

println("Hello")
来源：http://azi.havefunace.top

[T02] Kotlin：变量
来源：http://exh.jlsjyb.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uui.fengsongda.top

[T03] Kotlin：字符串模板
来源：http://ydb.zycfv.cn

"值: $b"
来源：http://rpn.jinyuanbaomall.cn

[T04] Kotlin：空安全
来源：http://rif.tian-w.cn

val n: String? = null;  n?.length
来源：http://gth.zdqjudy.top

[T05] Kotlin：when 表达式
来源：http://ngs.cdnleiting.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://szd.gaohongyu789.top

[T06] Kotlin：集合映射
来源：http://qjd.daria6918.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://vka.gzhubu.top

[T07] Kotlin：集合过滤
来源：http://tos.xziqi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://gfz.chenjidiqi.icu

[T08] Kotlin：数据类
来源：http://wwq.epnwcf.com

data class User(val name: String, val age: Int)
来源：http://fff.pycfn.com

[T09] Kotlin：扩展函数
来源：http://xcq.yuxming.cn

fun String.exclaim() = this + "!"
来源：http://cfc.dashuyun.cn

[T10] Kotlin：默认参数
来源：http://rcp.vehdjk.com

fun greet(name: String = "World") = "Hi $name"
来源：http://xmz.nwbrower.top

[T11] Kotlin：协程
来源：http://qzk.snrcjt.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://imp.jinqigufen.top

[T12] Kotlin：解构声明
来源：http://ntw.xinyue.icu

val (a, b) = Pair(1, 2)
来源：http://jcv.fehbvm.com

[T13] Kotlin：只读 Map
来源：http://pkn.guowangkeji.top

val m = mapOf("a" to 1)
来源：http://pcl.kuanghao11.cn

[T14] Kotlin：循环
来源：http://fcl.gotoacloud.top

for (i in 1..10) println(i)
来源：http://qvi.cdnleiting.top

[T15] Kotlin：接口
来源：http://lin.ydjk.org.cn

interface Shape { fun area(): Double }
来源：http://mvw.fzhhl.top

[T16] Swift：Hello World
来源：http://wym.chenlongwang.top

print("Hello")
来源：http://izj.guannengcc.top

[T17] Swift：变量与常量
来源：http://wzw.jinqigufen.top

var a = 1;  let b = 2
来源：http://snl.hnxiangtu.top

[T18] Swift：字符串插值
来源：http://gkk.ydzc1.top

"值: \(b)"
来源：http://fyf.jinqigfzy.top

[T19] Swift：可选绑定
来源：http://nkh.jinyuanbaomall.cn

if let n = opt { print(n) }
来源：http://jkd.shzxlz.cn

[T20] Swift：数组操作
来源：http://guv.sysykeji.top

var a = [1, 2, 3];  a.append(4)
来源：http://xaa.52xcode.cn

[T21] Swift：遍历
来源：http://uqq.kuanghao11.cn

for x in a { print(x) }
来源：http://vim.yuxming.cn

[T22] Swift：字典
来源：http://wko.ivvv.top

var d = ["a": 1];  d["b"] = 2
来源：http://gmq.jlsjyb.cn

[T23] Swift：函数
来源：http://ohm.iojbl.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lps.yonumen.top

[T24] Swift：闭包
来源：http://cpw.pengpengdd.cyou

let f = { (x: Int) -> Int in x * 2 }
来源：http://whu.9152youxi.cn


<!-- 参考信息 -->