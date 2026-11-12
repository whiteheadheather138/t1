代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tgt.yfazqb.com

[R24] 大小写转换
来源：http://zxr.sjlbkw.cn

echo "${s^^}"; echo "${s,,}"
来源：http://tzt.sjlbkw.cn

[R25] 去后缀 / 去前缀
来源：http://zor.0kj1m.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://gcr.52xcode.cn

[R26] 命令替换
来源：http://ctb.vehdjk.com

now=$(date +%F); echo "$now"
来源：http://cbq.smart0.xyz

[R27] 算术展开
来源：http://zci.dashuyun.cn

echo $((1 + 2 * 3))
来源：http://qsm.aizwys.cn

[R28] 浮点运算
来源：http://kzo.jianghu66.top

echo "scale=2; 10/3" | bc
来源：http://azu.jianghu66.top

[R29] 定义函数
来源：http://shq.haohaochexian.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kro.yongpay.top

[R30] 函数返回状态码
来源：http://wrj.haohaochexian.top

f() { return 0; }; f || echo "失败了"
来源：http://dpd.jinghuilouyu.cn

[R31] 局部变量
来源：http://pna.iojbl.cn

f() { local x=1; echo "$x"; }
来源：http://ohm.dianchejie.cn

[R32] 参数个数校验
来源：http://hyr.zycfv.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cok.shanyushiyangkeji.top

[R33] 捕获错误并提示行号
来源：http://dho.xuanzx.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://eql.jyoumei.cn

[R34] 退出时清理
来源：http://hfc.yuanzhike.top

trap 'rm -f "$tmp"' EXIT
来源：http://syf.snrcjt.cn

[R35] 后台执行并等待
来源：http://loc.bjfxy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ysb.ywan-chungtsiang.top

[R36] 并发执行多个任务
来源：http://dpy.xziqi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zdp.bjfxy.top

[R37] 把输出赋给变量
来源：http://tjl.gogol.net.cn

files=$(ls -1)
来源：http://muj.yongpay.top

[R38] 管道串联
来源：http://ass.bbcook.cn

cat a.txt | grep -i error | wc -l
来源：http://ieh.guannengcc.top

[R39] 重定向标准输出与错误
来源：http://vvx.aibaodan.cn

cmd > out.log 2>&1
来源：http://wgu.yonumen.top

[R40] 追加写日志
来源：http://guj.ywan-chungtsiang.top

echo "log" >> out.log
来源：http://uwf.shanyushiyangkeji.top

[R41] 丢弃输出
来源：http://ean.ywan-chungtsiang.top

cmd >/dev/null 2>&1
来源：http://zab.9152youxi.cn

[R42] 输入重定向
来源：http://scs.jinyuanbaomall.cn

wc -l < a.txt
来源：http://hsa.wangshuangyany.cn

[R43] 按名字查找文件
来源：http://ebe.jqgufenzy.top

find . -name "*.log" -type f
来源：http://mza.shangyingyoupin.top

[R44] 按修改时间查找
来源：http://byk.hongshengwenyu.top

find . -mtime -7 -type f
来源：http://pmb.316326.xyz

[R45] 批量删除
来源：http://wrg.vqdsnc.cn

find . -name "*.tmp" -delete
来源：http://apc.chenlongwang.top

[R46] 递归替换文件内容
来源：http://uac.chenlongwang.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hda.xinyue.icu

[R47] sed 单行替换
来源：http://evy.yuxming.cn

sed -i 's/foo/bar/g' a.txt
来源：http://chb.svipenyu.cn

[R48] awk 取指定列
来源：http://tji.bbcook.cn

awk '{print $1, $3}' a.txt
来源：http://vck.fanxiaobao.xyz

[R49] awk 带条件
来源：http://ekr.sweek.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fzt.daxiang520.top

[R50] awk 求和
来源：http://hce.fehbvm.com

awk '{s += $2} END {print s}' a.txt
来源：http://vwd.ivvv.top

[R51] 排序去重取前几
来源：http://oxm.sxryk.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hhq.yj20258.top

[R52] 统计行数
来源：http://new.ctjpmb.com

wc -l a.txt
来源：http://uzs.ywan-chungtsiang.top

[R53] 查看文件头与实时尾
来源：http://rzi.yonumen.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://oio.vehdjk.com

[R54] 比较两个文件
来源：http://fia.dashuyun.cn

diff a.txt b.txt
来源：http://tte.hfpthk.cn

[R55] 压缩与解压
来源：http://kdb.quarkkingdee.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://est.yj202588.top

[R56] 远程拷贝
来源：http://qci.zhijiandao.cn

scp file user@host:/path/
来源：http://krr.sysykeji.top

[R57] 远程执行命令
来源：http://azo.vehdjk.com

ssh user@host 'uptime'
来源：http://wog.jlsjyb.cn

[R58] 下载文件
来源：http://jxt.yanxiufei.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://urw.hnxiangtu.top

[R59] 发 POST JSON
来源：http://tkc.jinqigufen.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kmw.guowangkeji.top

[R60] 只看 HTTP 状态码
来源：http://urv.xylfe.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ono.fanxiaobao.xyz

[R61] 磁盘占用
来源：http://cwy.zhiwuduotai.top

df -h;  du -sh *
来源：http://fgo.uphjek.com

[R62] 找最占空间的文件
来源：http://mvt.ehwqpu.com

du -ah . | sort -rh | head -10
来源：http://nmn.hnxiangtu.top

[R63] 内存与进程
来源：http://rvp.c1oappe.top

free -h;  ps aux | grep nginx
来源：http://hzq.dashuyun.cn

[R64] 结束进程
来源：http://azy.yj202588.top

kill -9 $(pgrep -f app.py)
来源：http://rsr.jlsjyb.cn

[R65] 查看端口占用
来源：http://jpb.fehbvm.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nub.cashguo.top

[R66] 定时任务
来源：http://ksd.xziqi.cn

crontab -e;  crontab -l
来源：http://ipr.chenzaomai.com

[R67] 生成随机十六进制串
来源：http://dxt.shzxlz.cn

openssl rand -hex 16
来源：http://sig.hfpthk.cn

[R68] 计算文件校验值
来源：http://ygc.jinqigufen.top

sha256sum a.txt;  md5sum a.txt
来源：http://mtw.yvedp.cn

[R69] 生成随机密码
来源：http://ydv.xziqi.cn

head -c 16 /dev/urandom | base64
来源：http://mrp.hesvh.cn

[R70] 时间戳与互转
来源：http://zka.hongshengwenyu.top

date +%s;  date -d @1700000000
来源：http://uuv.guowangkeji.top

[R71] 日期格式化
来源：http://ynj.hysaishi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://cuy.sjlbkw.cn

[R72] 等待端口就绪
来源：http://wgn.fengsongda.top

until nc -z localhost 3306; do sleep 1; done
来源：http://cyv.bjfxy.top

[R73] 分割大日志
来源：http://oph.shanyushiyangkeji.top

split -l 1000 big.log part_
来源：http://hrj.ppjwa.cn

[R74] 批量重命名
来源：http://wij.shanyushiyangtech.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nqe.ivvv.top

[R75] 导出环境变量
来源：http://qlk.zhengqikj.top

export PATH="$HOME/bin:$PATH"
来源：http://kou.dianchejie.cn

[R76] 使用临时文件
来源：http://efl.52xcode.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xhc.daria6918.cn

[R77] 读取用户输入
来源：http://ecm.smart0.xyz

read -rp "请输入: " ans
来源：http://yal.316326.xyz

[R78] 交互式菜单
来源：http://gab.cashguo.top

select opt in a b c; do echo "$opt"; break; done
来源：http://rlc.yongpay.top

[R79] 解析命令行选项
来源：http://itk.smart0.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nqp.tarul.cn

[R80] 查看脚本执行耗时
来源：http://uzf.mhx1999.top

time ./run.sh
来源：http://sgz.hywenlv.cn

================================================================================
来源：http://fhi.52xcode.cn

S. C / C++ 专题
来源：http://dzf.yongpay.top

================================================================================
来源：http://yqx.52xcode.cn

[S01] C：Hello World
来源：http://ohz.sjlbkw.cn

#include <stdio.h>
来源：http://dua.uphjek.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://uov.sweek.top

[S02] C：变量与格式化输出
来源：http://zge.vehdjk.com

int a = 10; printf("%d\n", a);
来源：http://unc.sysykeji.top

[S03] C：读入整数
来源：http://ppc.yonumen.top

int x; scanf("%d", &x);
来源：http://mei.shangyingyoupin.top

[S04] C：字符串复制
来源：http://tcm.yj20258888.top

char dst[32]; strcpy(dst, "hi");
来源：http://aso.zhixingplan.top

[S05] C：字符串长度
来源：http://gaq.ybcxt.top

strlen(s)
来源：http://dna.tarul.cn

[S06] C：字符串比较
来源：http://irn.guannengcc.top

strcmp(a, b) == 0
来源：http://qgs.zdbjq.cn

[S07] C：数组遍历求和
来源：http://zif.quarkkingdee.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://osx.gaohongyu789.top

[S08] C：动态内存分配与释放
来源：http://bbg.yfazqb.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nlc.ivvv.top

[S09] C：结构体定义与初始化
来源：http://qui.fzhhl.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zgq.yueranfly.top

[S10] C：指针与解引用
来源：http://quu.gzhubu.top

int *p = &a;  *p = 5;
来源：http://niv.fengsongda.top

[S11] C：逐行读文件
来源：http://hsy.daxiang520.top

FILE *f = fopen("a.txt", "r");
来源：http://kre.hcnkem.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://mlh.sjlbkw.cn

fclose(f);
来源：http://cuo.zycfv.cn

[S12] C：写文件
来源：http://jvj.316326.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://svl.epnwcf.com

[S13] C：宏定义
来源：http://nfe.cdnleiting.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://eap.chenzaomai.com

[S14] C：枚举
来源：http://qsx.ppjwa.cn

enum Color { RED, GREEN, BLUE };
来源：http://rjy.cheryme.top

[S15] C：类型转换
来源：http://ubm.jyoumei.cn

(double) a / b
来源：http://svo.gaohongyu789.top

[S16] C：位操作置位
来源：http://doq.shanyushiyangtech.top

x |= (1 << 3);
来源：http://bum.vqdsnc.cn

[S17] C：安全拼接字符串
来源：http://kgj.hcnkem.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ftu.tianlin.xyz

[S18] C：命令行参数
来源：http://obc.vehdjk.com

int main(int argc, char **argv)
来源：http://pek.nanxinkj.top

[S19] C：快速排序
来源：http://mte.chenlongwang.top

qsort(a, n, sizeof(int), cmp);
来源：http://jsq.ctjpmb.com

[S20] C：二分查找
来源：http://lmp.redwolf501.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mag.zhaomingkeji.xyz

[S21] C：字符类别判断
来源：http://skv.yueranfly.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mmo.yangfankeji.com

[S22] C：字符串转数字
来源：http://mcs.ydzc1.top

atoi("42");  strtod("3.14", NULL);
来源：http://kzy.cheryme.top

[S23] C：随机数
来源：http://zzo.fehbvm.com

srand(time(NULL));  int r = rand() % 100;
来源：http://cya.hfpthk.cn

[S24] C：获取本地时间
来源：http://scc.chenjidiqi.icu

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wxi.hammf.cn

[S25] C：内存拷贝
来源：http://opi.uphjek.com

memcpy(dst, src, n);
来源：http://ffn.chenzaomai.com

[S26] C：内存清零
来源：http://eqb.jyoumei.cn

memset(a, 0, sizeof a);
来源：http://wqx.mhx1999.top

[S27] C：定义常量
来源：http://drc.bbcook.cn

const double PI = 3.14159;
来源：http://xsw.guannengcc.top

[S28] C：静态变量
来源：http://tsa.andypj.xyz

static int counter = 0;
来源：http://bxq.ivvv.top

[S29] C：变参函数
来源：http://nwg.andypj.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dkm.sysykeji.top

[S30] C：头文件保护
来源：http://jcb.meibo888.top

#ifndef X_H
来源：http://faf.nwbrower.top

#define X_H
来源：http://cva.yj202588.top

#endif
来源：http://oad.guowangkeji.top

[S31] C++：Hello World
来源：http://hmz.yfazqb.com

#include <iostream>
来源：http://tla.fengsongda.top

int main() { std::cout << "Hello\n"; }
来源：http://xac.yueranfly.top

[S32] C++：字符串
来源：http://yzh.svipenyu.cn

std::string s = "hi";  s += "!";
来源：http://him.tanke756.top

[S33] C++：vector 增删
来源：http://utn.ywan-chungtsiang.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dde.cashguo.top

[S34] C++：遍历 vector
来源：http://yrf.yangfankeji.com

for (auto &x : v) { std::cout << x; }
来源：http://jni.jiagoushi.top

[S35] C++：map
来源：http://ldv.chenlongwang.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dbf.fehbvm.com

[S36] C++：unordered_map
来源：http://iys.pengpengdd.cyou

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fow.jinqigfzy.top

[S37] C++：set
来源：http://isd.sufxvd.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rkv.andypj.xyz

[S38] C++：排序
来源：http://ltq.zycfv.cn

std::sort(v.begin(), v.end());
来源：http://mqi.gzhubu.top

[S39] C++：自定义比较器排序
来源：http://vyn.gotoacloud.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fau.hywenlv.cn

[S40] C++：查找元素
来源：http://kvp.jinqigufen.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hmy.vqdsnc.cn

[S41] C++：类与构造函数
来源：http://hca.smart0.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xzr.yuanzhike.top

[S42] C++：继承与虚函数
来源：http://pzc.cheryme.top

class B : public Base { public: void f() override {} };
来源：http://cfc.zhengqikj.top

[S43] C++：智能指针
来源：http://wsf.epnwcf.com

auto p = std::make_unique<int>(5);
来源：http://fgs.shzxlz.cn

[S44] C++：引用传参
来源：http://yfs.shangyingyoupin.top

void inc(int &x) { ++x; }
来源：http://ybt.zhongyouzk.top

[S45] C++：lambda
来源：http://hyb.cdnleiting.top

auto add = [](int a, int b) { return a + b; };
来源：http://ifa.xuetiantiany.cn

[S46] C++：函数模板
来源：http://elp.zhijiandao.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://akj.yvedp.cn

[S47] C++：结构化绑定遍历
来源：http://ohv.sweek.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fkh.cdnleiting.top

[S48] C++：逐行读文件
来源：http://uwa.yj202588.top

std::ifstream in("a.txt");  std::string line;
来源：http://kgr.sjlbkw.cn

while (std::getline(in, line)) { }
来源：http://dfm.yvedp.cn

[S49] C++：写文件
来源：http://hsr.pycfn.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://aau.meibo888.top

[S50] C++：格式化数字
来源：http://ndz.jinqigufen.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ulw.ywan-chungtsiang.top

[S51] C++：显式类型转换
来源：http://vly.cashguo.top

static_cast<double>(a) / b
来源：http://ibz.jianghu66.top

[S52] C++：const 与 noexcept
来源：http://oal.chenzaomai.com

int size() const noexcept { return n_; }
来源：http://kln.ydjk.org.cn

[S53] C++：移动语义
来源：http://oym.hnqzz.top

std::vector<int> w = std::move(v);
来源：http://pdr.jyoumei.cn

[S54] C++：异常处理
来源：http://oym.vqdsnc.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fuw.ydjk.org.cn

[S55] C++：结构化绑定
来源：http://ndp.cheryme.top

auto [a, b] = std::make_pair(1, 2);
来源：http://naw.daria6918.cn

[S56] C++：optional
来源：http://qut.andypj.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fla.0kj1m.cn

[S57] C++：编译期常量
来源：http://qfg.andypj.xyz

constexpr int N = 10;
来源：http://cgq.cdnleiting.top

[S58] C++：命名空间
来源：http://quy.cashguo.top

namespace ns { int f() { return 1; } }
来源：http://lil.feifeiyinyue.top

[S59] C++：静态断言
来源：http://ysr.tanke756.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bie.hysaishi.cn

[S60] C++：遍历并删除元素
来源：http://zdx.gotoacloud.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://knf.jianghu66.top

================================================================================
来源：http://rod.ppjwa.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hxm.zdqjudy.top

================================================================================
来源：http://biw.jqgfzy.top

[T01] Kotlin：Hello World
来源：http://daz.birdmap.top

println("Hello")
来源：http://ihm.316326.xyz

[T02] Kotlin：变量
来源：http://qxs.nwbrower.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vtv.nanxuanxn.top

[T03] Kotlin：字符串模板
来源：http://hdi.sxryk.cn

"值: $b"
来源：http://umf.hfpthk.cn

[T04] Kotlin：空安全
来源：http://ztf.dashuyun.cn

val n: String? = null;  n?.length
来源：http://auu.zdbjq.cn

[T05] Kotlin：when 表达式
来源：http://nds.ydzc1.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nlm.feifeiyinyue.top

[T06] Kotlin：集合映射
来源：http://uxk.pengpengdd.cyou

listOf(1, 2, 3).map { it * 2 }
来源：http://jam.sxryk.cn

[T07] Kotlin：集合过滤
来源：http://zyo.guannengcc.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://hgv.zdbjq.cn

[T08] Kotlin：数据类
来源：http://otp.cucudq.cn

data class User(val name: String, val age: Int)
来源：http://bhv.zdqjudy.top

[T09] Kotlin：扩展函数
来源：http://ast.hysaishi.cn

fun String.exclaim() = this + "!"
来源：http://jyp.c1oappe.top

[T10] Kotlin：默认参数
来源：http://ntd.ybcxt.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ymx.smart0.xyz

[T11] Kotlin：协程
来源：http://bnc.zdqjudy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://iaf.havefunace.top

[T12] Kotlin：解构声明
来源：http://esn.jinqigufen.top

val (a, b) = Pair(1, 2)
来源：http://vjd.tanke756.top

[T13] Kotlin：只读 Map
来源：http://mgx.iojbl.cn

val m = mapOf("a" to 1)
来源：http://pam.ybcxt.top

[T14] Kotlin：循环
来源：http://wik.jqgfzy.top

for (i in 1..10) println(i)
来源：http://flt.jiagoushi.top

[T15] Kotlin：接口
来源：http://wgx.chenlongwang.top

interface Shape { fun area(): Double }
来源：http://ljy.yuxming.cn

[T16] Swift：Hello World
来源：http://nwx.sweek.top

print("Hello")
来源：http://ipa.sweek.top

[T17] Swift：变量与常量
来源：http://jax.ybcxt.top

var a = 1;  let b = 2
来源：http://mgn.fengsongda.top

[T18] Swift：字符串插值
来源：http://mjr.9152youxi.cn

"值: \(b)"
来源：http://bxm.ybcxt.top

[T19] Swift：可选绑定
来源：http://ctx.yvedp.cn

if let n = opt { print(n) }
来源：http://hml.9152youxi.cn

[T20] Swift：数组操作
来源：http://jmr.ppjwa.cn

var a = [1, 2, 3];  a.append(4)
来源：http://obp.gotoacloud.top

[T21] Swift：遍历
来源：http://krd.birdmap.top

for x in a { print(x) }
来源：http://sqd.yuxming.cn

[T22] Swift：字典
来源：http://etz.iojbl.cn

var d = ["a": 1];  d["b"] = 2
来源：http://jku.wangdashe.top

[T23] Swift：函数
来源：http://igt.cucudq.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cxq.gaohongyu789.top

[T24] Swift：闭包
来源：http://gso.jinyuanbaomall.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xpf.hfpthk.cn

[T25] Swift：结构体
来源：http://htv.tanke756.top

struct P { var x: Int }
来源：http://cpg.wangdashe.top

[T26] Swift：类与重写
来源：http://tat.iojbl.cn

class A: Base { override func f() {} }
来源：http://wwn.vehdjk.com


<!-- 参考信息 -->