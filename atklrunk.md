代发 wailian999

echo "${#s}"
来源：http://vno.zhaomingkeji.xyz

[R22] 截取子串
来源：http://sis.yj202588.top

echo "${s:0:5}"
来源：http://eqw.xinyue.icu

[R23] 字符串替换
来源：http://hnv.mhx1999.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ggh.jinyuanbaomall.cn

[R24] 大小写转换
来源：http://tiy.ehwqpu.com

echo "${s^^}"; echo "${s,,}"
来源：http://hdz.pycfn.com

[R25] 去后缀 / 去前缀
来源：http://pfn.yangfankeji.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://nwt.gogol.net.cn

[R26] 命令替换
来源：http://arz.aizwys.cn

now=$(date +%F); echo "$now"
来源：http://vkk.sufxvd.cn

[R27] 算术展开
来源：http://uig.zhiwuduotai.top

echo $((1 + 2 * 3))
来源：http://dak.daria6918.cn

[R28] 浮点运算
来源：http://dhp.zhoulong.xyz

echo "scale=2; 10/3" | bc
来源：http://yjx.chenzaomai.com

[R29] 定义函数
来源：http://aek.ydzc1.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ssi.yueranfly.top

[R30] 函数返回状态码
来源：http://dlq.daria6918.cn

f() { return 0; }; f || echo "失败了"
来源：http://xyg.tanke756.top

[R31] 局部变量
来源：http://qmp.tian-w.cn

f() { local x=1; echo "$x"; }
来源：http://jmq.yj20258.top

[R32] 参数个数校验
来源：http://qch.zhoulong.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qvk.hammf.cn

[R33] 捕获错误并提示行号
来源：http://sxo.cheryme.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vmz.ybcxt.top

[R34] 退出时清理
来源：http://uoj.wangshuangyany.cn

trap 'rm -f "$tmp"' EXIT
来源：http://nfi.tian-w.cn

[R35] 后台执行并等待
来源：http://tlu.fanxiaobao.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://kqq.meibo888.top

[R36] 并发执行多个任务
来源：http://uui.jianghu66.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ofw.sweek.top

[R37] 把输出赋给变量
来源：http://ljy.cucudq.cn

files=$(ls -1)
来源：http://lxy.daria6918.cn

[R38] 管道串联
来源：http://nzw.havefunace.top

cat a.txt | grep -i error | wc -l
来源：http://eyq.hesvh.cn

[R39] 重定向标准输出与错误
来源：http://sdx.yj20258888.top

cmd > out.log 2>&1
来源：http://wdr.52xcode.cn

[R40] 追加写日志
来源：http://vjy.yanxiufei.cn

echo "log" >> out.log
来源：http://avs.quarkkingdee.top

[R41] 丢弃输出
来源：http://wvu.zdqjudy.top

cmd >/dev/null 2>&1
来源：http://vse.guannengcc.top

[R42] 输入重定向
来源：http://fvq.wangdashe.top

wc -l < a.txt
来源：http://kax.jqgfzy.top

[R43] 按名字查找文件
来源：http://tcv.shuidangran.top

find . -name "*.log" -type f
来源：http://tlt.zdbjq.cn

[R44] 按修改时间查找
来源：http://wty.chenlongwang.top

find . -mtime -7 -type f
来源：http://ouq.vehdjk.com

[R45] 批量删除
来源：http://ugz.yangfankeji.com

find . -name "*.tmp" -delete
来源：http://qwk.9152youxi.cn

[R46] 递归替换文件内容
来源：http://hyb.guannengcc.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zaz.tianlin.xyz

[R47] sed 单行替换
来源：http://rlb.birdmap.top

sed -i 's/foo/bar/g' a.txt
来源：http://sey.yueranfly.top

[R48] awk 取指定列
来源：http://xti.jinqigufen.top

awk '{print $1, $3}' a.txt
来源：http://ysx.hywenlv.cn

[R49] awk 带条件
来源：http://jzb.smart0.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nvd.ctjpmb.com

[R50] awk 求和
来源：http://ekt.jinqigufen.top

awk '{s += $2} END {print s}' a.txt
来源：http://dcm.hammf.cn

[R51] 排序去重取前几
来源：http://dpd.ppjwa.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://oao.hammf.cn

[R52] 统计行数
来源：http://ile.zhijiandao.cn

wc -l a.txt
来源：http://jch.nanxinkj.top

[R53] 查看文件头与实时尾
来源：http://fsd.yongpay.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://byg.sweek.top

[R54] 比较两个文件
来源：http://ffp.redwolf501.top

diff a.txt b.txt
来源：http://rhc.nwbrower.top

[R55] 压缩与解压
来源：http://eyj.xuanzx.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://iwz.zycfv.cn

[R56] 远程拷贝
来源：http://wcl.hcnkem.com

scp file user@host:/path/
来源：http://lqs.bbcook.cn

[R57] 远程执行命令
来源：http://dgd.hesvh.cn

ssh user@host 'uptime'
来源：http://lfv.chenlongwang.top

[R58] 下载文件
来源：http://hcj.hfpthk.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pjz.havefunace.top

[R59] 发 POST JSON
来源：http://jdx.snrcjt.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nlx.xuetiantiany.cn

[R60] 只看 HTTP 状态码
来源：http://bqc.jinghuilouyu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://iwn.jinyuanbaomall.cn

[R61] 磁盘占用
来源：http://auz.fengsongda.top

df -h;  du -sh *
来源：http://sry.tarul.cn

[R62] 找最占空间的文件
来源：http://edg.pycfn.com

du -ah . | sort -rh | head -10
来源：http://msb.jiagoushi.top

[R63] 内存与进程
来源：http://gkk.redwolf501.top

free -h;  ps aux | grep nginx
来源：http://rjj.jinghuilouyu.cn

[R64] 结束进程
来源：http://yam.ctjpmb.com

kill -9 $(pgrep -f app.py)
来源：http://qfx.snrcjt.cn

[R65] 查看端口占用
来源：http://vaz.bjfxy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lss.jinqigufen.top

[R66] 定时任务
来源：http://vdx.zhongyouzk.top

crontab -e;  crontab -l
来源：http://rut.iojbl.cn

[R67] 生成随机十六进制串
来源：http://aqk.yuanzhike.top

openssl rand -hex 16
来源：http://nmb.zhengqikj.top

[R68] 计算文件校验值
来源：http://fkg.sxryk.cn

sha256sum a.txt;  md5sum a.txt
来源：http://tlg.xingfuxueyuan.xyz

[R69] 生成随机密码
来源：http://fkb.fengsongda.top

head -c 16 /dev/urandom | base64
来源：http://uxq.xuetiantiany.cn

[R70] 时间戳与互转
来源：http://pwf.hammf.cn

date +%s;  date -d @1700000000
来源：http://bwq.nwbrower.top

[R71] 日期格式化
来源：http://atj.cucudq.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://wqw.uphjek.com

[R72] 等待端口就绪
来源：http://qxe.guannengcc.top

until nc -z localhost 3306; do sleep 1; done
来源：http://sdq.ydjk.org.cn

[R73] 分割大日志
来源：http://ucp.vehdjk.com

split -l 1000 big.log part_
来源：http://lad.epnwcf.com

[R74] 批量重命名
来源：http://cef.fehbvm.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ubh.fanxiaobao.xyz

[R75] 导出环境变量
来源：http://gpu.daria6918.cn

export PATH="$HOME/bin:$PATH"
来源：http://ghd.gotoacloud.top

[R76] 使用临时文件
来源：http://hxj.yvedp.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://uif.hcnkem.com

[R77] 读取用户输入
来源：http://jqi.hongshengwenyu.top

read -rp "请输入: " ans
来源：http://scc.zhijiandao.cn

[R78] 交互式菜单
来源：http://agd.yj20258.top

select opt in a b c; do echo "$opt"; break; done
来源：http://vsc.chenlongwang.top

[R79] 解析命令行选项
来源：http://onv.hammf.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://plt.fanxiaobao.xyz

[R80] 查看脚本执行耗时
来源：http://lhr.smart0.xyz

time ./run.sh
来源：http://lwu.aizwys.cn

================================================================================
来源：http://kvl.jinqigfzy.top

S. C / C++ 专题
来源：http://kjg.dashuyun.cn

================================================================================
来源：http://itz.chenzaomai.com

[S01] C：Hello World
来源：http://qgi.aibaodan.cn

#include <stdio.h>
来源：http://nxe.vqdsnc.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://dst.sysykeji.top

[S02] C：变量与格式化输出
来源：http://rcv.dashuyun.cn

int a = 10; printf("%d\n", a);
来源：http://eev.sufxvd.cn

[S03] C：读入整数
来源：http://uvf.pengpengdd.cyou

int x; scanf("%d", &x);
来源：http://gpp.shuidangran.top

[S04] C：字符串复制
来源：http://ydc.jlsjyb.cn

char dst[32]; strcpy(dst, "hi");
来源：http://pzo.jiagoushi.top

[S05] C：字符串长度
来源：http://bbl.hnqzz.top

strlen(s)
来源：http://rro.zhixingplan.top

[S06] C：字符串比较
来源：http://laj.vehdjk.com

strcmp(a, b) == 0
来源：http://gmb.ivvv.top

[S07] C：数组遍历求和
来源：http://xpo.cqqwz.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zhe.zycfv.cn

[S08] C：动态内存分配与释放
来源：http://wyh.yuanzhike.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://urq.yonumen.top

[S09] C：结构体定义与初始化
来源：http://yln.fzhhl.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://szi.iojbl.cn

[S10] C：指针与解引用
来源：http://whq.hysaishi.cn

int *p = &a;  *p = 5;
来源：http://ajx.shuidangran.top

[S11] C：逐行读文件
来源：http://atc.xylfe.cn

FILE *f = fopen("a.txt", "r");
来源：http://caj.ydzc1.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://lwa.sufxvd.cn

fclose(f);
来源：http://wni.daxiang520.top

[S12] C：写文件
来源：http://swi.9152youxi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uux.wangshuangyany.cn

[S13] C：宏定义
来源：http://wki.zhoulong.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jpp.yangfankeji.com

[S14] C：枚举
来源：http://wqc.jinqigufen.top

enum Color { RED, GREEN, BLUE };
来源：http://qcn.shanyushiyangkeji.top

[S15] C：类型转换
来源：http://ezc.sjlbkw.cn

(double) a / b
来源：http://uwg.quarkkingdee.top

[S16] C：位操作置位
来源：http://zdt.jinqigufen.top

x |= (1 << 3);
来源：http://twn.jinqigfzy.top

[S17] C：安全拼接字符串
来源：http://elu.mhx1999.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://csv.ydzc1.top

[S18] C：命令行参数
来源：http://orv.ydjk.org.cn

int main(int argc, char **argv)
来源：http://tiq.yanxiufei.cn

[S19] C：快速排序
来源：http://qnc.ctjpmb.com

qsort(a, n, sizeof(int), cmp);
来源：http://qzp.iojbl.cn

[S20] C：二分查找
来源：http://xlu.chenzaomai.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kkf.zhoulong.xyz

[S21] C：字符类别判断
来源：http://sti.uphjek.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jco.mhx1999.top

[S22] C：字符串转数字
来源：http://lzk.mhx1999.top

atoi("42");  strtod("3.14", NULL);
来源：http://ymk.gzhubu.top

[S23] C：随机数
来源：http://paa.sysykeji.top

srand(time(NULL));  int r = rand() % 100;
来源：http://xmg.hesvh.cn

[S24] C：获取本地时间
来源：http://pas.jlsjyb.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lun.wangshuangyany.cn

[S25] C：内存拷贝
来源：http://ect.hnqzz.top

memcpy(dst, src, n);
来源：http://fvf.yj20258888.top

[S26] C：内存清零
来源：http://xzi.zhixingplan.top

memset(a, 0, sizeof a);
来源：http://kaw.meibo888.top

[S27] C：定义常量
来源：http://gog.jinqigfzy.top

const double PI = 3.14159;
来源：http://peu.hongshengwenyu.top

[S28] C：静态变量
来源：http://etw.iojbl.cn

static int counter = 0;
来源：http://pvc.meibo888.top

[S29] C：变参函数
来源：http://kli.sweek.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fcy.yanxiufei.cn

[S30] C：头文件保护
来源：http://fqj.ehwqpu.com

#ifndef X_H
来源：http://jiw.jinghuilouyu.cn

#define X_H
来源：http://oya.316326.xyz

#endif
来源：http://ibi.sxryk.cn

[S31] C++：Hello World
来源：http://ouh.hammf.cn

#include <iostream>
来源：http://xeu.bjfxy.top

int main() { std::cout << "Hello\n"; }
来源：http://vsh.9152youxi.cn

[S32] C++：字符串
来源：http://xfp.redwolf501.top

std::string s = "hi";  s += "!";
来源：http://bhv.tanke756.top

[S33] C++：vector 增删
来源：http://fdk.kuanghao11.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wbz.guowangkeji.top

[S34] C++：遍历 vector
来源：http://eaz.vehdjk.com

for (auto &x : v) { std::cout << x; }
来源：http://hox.gotoacloud.top

[S35] C++：map
来源：http://gcz.yongpay.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fln.ywan-chungtsiang.top

[S36] C++：unordered_map
来源：http://cbt.yvedp.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yzd.chenlongwang.top

[S37] C++：set
来源：http://rir.wangdashe.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cni.daria6918.cn

[S38] C++：排序
来源：http://mmc.hongshengwenyu.top

std::sort(v.begin(), v.end());
来源：http://eju.xylfe.cn

[S39] C++：自定义比较器排序
来源：http://wtz.xingfuxueyuan.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dyx.epnwcf.com

[S40] C++：查找元素
来源：http://osg.yanxiufei.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xxl.redwolf501.top

[S41] C++：类与构造函数
来源：http://gxh.wangdashe.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://aye.tian-w.cn

[S42] C++：继承与虚函数
来源：http://xfr.nanxuanxn.top

class B : public Base { public: void f() override {} };
来源：http://yzd.vqdsnc.cn

[S43] C++：智能指针
来源：http://pin.cashguo.top

auto p = std::make_unique<int>(5);
来源：http://ksi.cqqwz.cn

[S44] C++：引用传参
来源：http://hye.wangshuangyany.cn

void inc(int &x) { ++x; }
来源：http://zwo.316326.xyz

[S45] C++：lambda
来源：http://aqk.smart0.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://pok.jinqigfzy.top

[S46] C++：函数模板
来源：http://dky.xylfe.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ane.aizwys.cn

[S47] C++：结构化绑定遍历
来源：http://jlq.yvedp.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kyf.316326.xyz

[S48] C++：逐行读文件
来源：http://jur.yj20258888.top

std::ifstream in("a.txt");  std::string line;
来源：http://oor.cucudq.cn

while (std::getline(in, line)) { }
来源：http://duw.uphjek.com

[S49] C++：写文件
来源：http://rzh.jiagoushi.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tra.tian-w.cn

[S50] C++：格式化数字
来源：http://bfb.vehdjk.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://whf.sufxvd.cn

[S51] C++：显式类型转换
来源：http://jka.guannengcc.top

static_cast<double>(a) / b
来源：http://phm.gaohongyu789.top

[S52] C++：const 与 noexcept
来源：http://erd.kuanghao11.cn

int size() const noexcept { return n_; }
来源：http://lkn.shzxlz.cn

[S53] C++：移动语义
来源：http://dmv.haohaochexian.top

std::vector<int> w = std::move(v);
来源：http://bdu.zdqjudy.top

[S54] C++：异常处理
来源：http://dqv.shuidangran.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rzd.snrcjt.cn

[S55] C++：结构化绑定
来源：http://ixe.jqgufenzy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://xln.aizwys.cn

[S56] C++：optional
来源：http://rkp.ydjk.org.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cug.iojbl.cn

[S57] C++：编译期常量
来源：http://kmc.hongshengwenyu.top

constexpr int N = 10;
来源：http://ceu.birdmap.top

[S58] C++：命名空间
来源：http://smh.hesvh.cn

namespace ns { int f() { return 1; } }
来源：http://wpf.52xcode.cn

[S59] C++：静态断言
来源：http://yba.mhx1999.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uij.jiagoushi.top

[S60] C++：遍历并删除元素
来源：http://dlz.yuxming.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yos.pycfn.com

================================================================================
来源：http://zku.ivvv.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ipq.aizwys.cn

================================================================================
来源：http://eez.tian-w.cn

[T01] Kotlin：Hello World
来源：http://vtb.aizwys.cn

println("Hello")
来源：http://ija.cheryme.top

[T02] Kotlin：变量
来源：http://fhv.shzxlz.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sbn.cheryme.top

[T03] Kotlin：字符串模板
来源：http://vmf.yongpay.top

"值: $b"
来源：http://cgm.yj20258.top

[T04] Kotlin：空安全
来源：http://jjh.pengpengdd.cyou

val n: String? = null;  n?.length
来源：http://fql.haohaochexian.top

[T05] Kotlin：when 表达式
来源：http://gkx.dianchejie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sey.hammf.cn

[T06] Kotlin：集合映射
来源：http://tzr.fanxiaobao.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://sos.epnwcf.com

[T07] Kotlin：集合过滤
来源：http://fts.meibo888.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://rbe.smart0.xyz

[T08] Kotlin：数据类
来源：http://vse.epnwcf.com

data class User(val name: String, val age: Int)
来源：http://qad.sxryk.cn

[T09] Kotlin：扩展函数
来源：http://yok.bjfxy.top

fun String.exclaim() = this + "!"
来源：http://xrx.chenjidiqi.icu

[T10] Kotlin：默认参数
来源：http://jff.snrcjt.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://usc.shangyingyoupin.top

[T11] Kotlin：协程
来源：http://fom.xuanzx.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://ntg.yfazqb.com

[T12] Kotlin：解构声明
来源：http://vdw.sweek.top

val (a, b) = Pair(1, 2)
来源：http://cqu.uphjek.com

[T13] Kotlin：只读 Map
来源：http://dxn.zycfv.cn

val m = mapOf("a" to 1)
来源：http://nlo.svipenyu.cn

[T14] Kotlin：循环
来源：http://axt.tanke756.top

for (i in 1..10) println(i)
来源：http://xqn.hfpthk.cn

[T15] Kotlin：接口
来源：http://qbk.tian-w.cn

interface Shape { fun area(): Double }
来源：http://ykg.nwbrower.top

[T16] Swift：Hello World
来源：http://xmw.sweek.top

print("Hello")
来源：http://rlq.sjlbkw.cn

[T17] Swift：变量与常量
来源：http://jdf.gogol.net.cn

var a = 1;  let b = 2
来源：http://mjg.guowangkeji.top

[T18] Swift：字符串插值
来源：http://ihq.daria6918.cn

"值: \(b)"
来源：http://nvx.nwbrower.top

[T19] Swift：可选绑定
来源：http://gsx.shanyushiyangtech.top

if let n = opt { print(n) }
来源：http://sib.snrcjt.cn

[T20] Swift：数组操作
来源：http://niz.gzhubu.top

var a = [1, 2, 3];  a.append(4)
来源：http://dsg.jinyuanbaomall.cn

[T21] Swift：遍历
来源：http://gjn.jqgufenzy.top

for x in a { print(x) }
来源：http://zyd.hcnkem.com

[T22] Swift：字典
来源：http://jmn.pycfn.com

var d = ["a": 1];  d["b"] = 2
来源：http://nab.yj202588.top

[T23] Swift：函数
来源：http://enc.zdbjq.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://onz.jlsjyb.cn

[T24] Swift：闭包
来源：http://zqk.316326.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://iqi.nanxinkj.top


<!-- 参考信息 -->