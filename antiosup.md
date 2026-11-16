代发 wailian999

echo "${#s}"
来源：http://mso.smart0.xyz

[R22] 截取子串
来源：http://cqt.9152youxi.cn

echo "${s:0:5}"
来源：http://mzj.jqgufenzy.top

[R23] 字符串替换
来源：http://onk.smart0.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kse.fktsv.cn

[R24] 大小写转换
来源：http://rrq.zhiwuduotai.top

echo "${s^^}"; echo "${s,,}"
来源：http://mys.yanxiufei.cn

[R25] 去后缀 / 去前缀
来源：http://yir.pycfn.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://gdu.pengpengdd.cyou

[R26] 命令替换
来源：http://ynz.yangfankeji.com

now=$(date +%F); echo "$now"
来源：http://fox.vqdsnc.cn

[R27] 算术展开
来源：http://gvi.cqqwz.cn

echo $((1 + 2 * 3))
来源：http://kpq.xuanzx.com

[R28] 浮点运算
来源：http://dcf.haohaochexian.top

echo "scale=2; 10/3" | bc
来源：http://ffv.hesvh.cn

[R29] 定义函数
来源：http://sjg.shanyushiyangkeji.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bzd.daxiang520.top

[R30] 函数返回状态码
来源：http://tea.0kj1m.cn

f() { return 0; }; f || echo "失败了"
来源：http://nfu.quarkkingdee.top

[R31] 局部变量
来源：http://uza.meibo888.top

f() { local x=1; echo "$x"; }
来源：http://fre.sjlbkw.cn

[R32] 参数个数校验
来源：http://wno.daxiang520.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jay.sysykeji.top

[R33] 捕获错误并提示行号
来源：http://tig.fzhhl.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hpf.gzhubu.top

[R34] 退出时清理
来源：http://tvn.hesvh.cn

trap 'rm -f "$tmp"' EXIT
来源：http://slx.bbcook.cn

[R35] 后台执行并等待
来源：http://qrq.gaohongyu789.top

sleep 5 & pid=$!; wait "$pid"
来源：http://nlk.fehbvm.com

[R36] 并发执行多个任务
来源：http://hrw.jinyuanbaomall.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hba.shzxlz.cn

[R37] 把输出赋给变量
来源：http://tyt.tianlin.xyz

files=$(ls -1)
来源：http://gpn.hysaishi.cn

[R38] 管道串联
来源：http://zfk.xuetiantiany.cn

cat a.txt | grep -i error | wc -l
来源：http://lbc.snrcjt.cn

[R39] 重定向标准输出与错误
来源：http://edc.shanyushiyangtech.top

cmd > out.log 2>&1
来源：http://pus.gotoacloud.top

[R40] 追加写日志
来源：http://rda.dashuyun.cn

echo "log" >> out.log
来源：http://hfp.ctjpmb.com

[R41] 丢弃输出
来源：http://hlj.andypj.xyz

cmd >/dev/null 2>&1
来源：http://sgv.ctjpmb.com

[R42] 输入重定向
来源：http://gbd.tarul.cn

wc -l < a.txt
来源：http://foj.ydzc1.top

[R43] 按名字查找文件
来源：http://jtv.daxiang520.top

find . -name "*.log" -type f
来源：http://bxd.cqqwz.cn

[R44] 按修改时间查找
来源：http://btd.zycfv.cn

find . -mtime -7 -type f
来源：http://aac.cdnleiting.top

[R45] 批量删除
来源：http://jsx.gotoacloud.top

find . -name "*.tmp" -delete
来源：http://lyn.hnxiangtu.top

[R46] 递归替换文件内容
来源：http://kit.zdqjudy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://byi.uphjek.com

[R47] sed 单行替换
来源：http://xsh.aibaodan.cn

sed -i 's/foo/bar/g' a.txt
来源：http://qqx.zhixingplan.top

[R48] awk 取指定列
来源：http://rci.shangyingyoupin.top

awk '{print $1, $3}' a.txt
来源：http://vrl.316326.xyz

[R49] awk 带条件
来源：http://lnr.cheryme.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://itt.shanyushiyangtech.top

[R50] awk 求和
来源：http://fzc.cqqwz.cn

awk '{s += $2} END {print s}' a.txt
来源：http://spa.xziqi.cn

[R51] 排序去重取前几
来源：http://ybk.aizwys.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://dbt.cheryme.top

[R52] 统计行数
来源：http://jar.ppjwa.cn

wc -l a.txt
来源：http://xgp.gzhubu.top

[R53] 查看文件头与实时尾
来源：http://rcc.chenjidiqi.icu

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ebs.yangfankeji.com

[R54] 比较两个文件
来源：http://wnp.ydjk.org.cn

diff a.txt b.txt
来源：http://tox.xingfuxueyuan.xyz

[R55] 压缩与解压
来源：http://lru.yvedp.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qdu.hongshengwenyu.top

[R56] 远程拷贝
来源：http://uxq.52xcode.cn

scp file user@host:/path/
来源：http://fam.chenjidiqi.icu

[R57] 远程执行命令
来源：http://hul.chenlongwang.top

ssh user@host 'uptime'
来源：http://ooo.zdqjudy.top

[R58] 下载文件
来源：http://mcx.jqgfzy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ztp.hysaishi.cn

[R59] 发 POST JSON
来源：http://hii.zhaomingkeji.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ypg.shuidangran.top

[R60] 只看 HTTP 状态码
来源：http://spa.jinyuanbaomall.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qre.iojbl.cn

[R61] 磁盘占用
来源：http://pax.jyoumei.cn

df -h;  du -sh *
来源：http://efm.jqgfzy.top

[R62] 找最占空间的文件
来源：http://jnu.tanke756.top

du -ah . | sort -rh | head -10
来源：http://sfi.fehbvm.com

[R63] 内存与进程
来源：http://esb.redwolf501.top

free -h;  ps aux | grep nginx
来源：http://eyg.daxiang520.top

[R64] 结束进程
来源：http://cge.svipenyu.cn

kill -9 $(pgrep -f app.py)
来源：http://wja.ywan-chungtsiang.top

[R65] 查看端口占用
来源：http://gaq.chenzaomai.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mhf.jlsjyb.cn

[R66] 定时任务
来源：http://aoj.hongshengwenyu.top

crontab -e;  crontab -l
来源：http://bxs.cucudq.cn

[R67] 生成随机十六进制串
来源：http://yzi.shzxlz.cn

openssl rand -hex 16
来源：http://dmm.hesvh.cn

[R68] 计算文件校验值
来源：http://eub.xziqi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ywq.guowangkeji.top

[R69] 生成随机密码
来源：http://mwc.pengpengdd.cyou

head -c 16 /dev/urandom | base64
来源：http://aur.wangdashe.top

[R70] 时间戳与互转
来源：http://wgp.shanyushiyangtech.top

date +%s;  date -d @1700000000
来源：http://mtg.guowangkeji.top

[R71] 日期格式化
来源：http://qlx.yj20258.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://tjq.yonumen.top

[R72] 等待端口就绪
来源：http://ldv.jianghu66.top

until nc -z localhost 3306; do sleep 1; done
来源：http://lub.9152youxi.cn

[R73] 分割大日志
来源：http://nid.xziqi.cn

split -l 1000 big.log part_
来源：http://vul.yj20258.top

[R74] 批量重命名
来源：http://ofh.gotoacloud.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lqd.jyoumei.cn

[R75] 导出环境变量
来源：http://mvm.pengpengdd.cyou

export PATH="$HOME/bin:$PATH"
来源：http://amy.ywan-chungtsiang.top

[R76] 使用临时文件
来源：http://mib.xingfuxueyuan.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ocz.zhaomingkeji.xyz

[R77] 读取用户输入
来源：http://vgh.dashuyun.cn

read -rp "请输入: " ans
来源：http://cop.uphjek.com

[R78] 交互式菜单
来源：http://wtu.nanxuanxn.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ksd.hywenlv.cn

[R79] 解析命令行选项
来源：http://hbr.hammf.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://azo.zhongyouzk.top

[R80] 查看脚本执行耗时
来源：http://hak.haohaochexian.top

time ./run.sh
来源：http://awb.bbcook.cn

================================================================================
来源：http://lvo.jqgfzy.top

S. C / C++ 专题
来源：http://wqh.yj20258.top

================================================================================
来源：http://plr.tianlin.xyz

[S01] C：Hello World
来源：http://mnv.ctjpmb.com

#include <stdio.h>
来源：http://syf.svipenyu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://mqf.cucudq.cn

[S02] C：变量与格式化输出
来源：http://ldd.zhengqikj.top

int a = 10; printf("%d\n", a);
来源：http://hhr.daria6918.cn

[S03] C：读入整数
来源：http://cwu.jqgufenzy.top

int x; scanf("%d", &x);
来源：http://yuw.zycfv.cn

[S04] C：字符串复制
来源：http://izj.gotoacloud.top

char dst[32]; strcpy(dst, "hi");
来源：http://wzl.gaohongyu789.top

[S05] C：字符串长度
来源：http://nuy.ywan-chungtsiang.top

strlen(s)
来源：http://asf.yonumen.top

[S06] C：字符串比较
来源：http://vri.hnqzz.top

strcmp(a, b) == 0
来源：http://zkt.zhongyouzk.top

[S07] C：数组遍历求和
来源：http://bev.xylfe.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lab.c1oappe.top

[S08] C：动态内存分配与释放
来源：http://gcj.fktsv.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vvy.9152youxi.cn

[S09] C：结构体定义与初始化
来源：http://bci.andypj.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://drl.cheryme.top

[S10] C：指针与解引用
来源：http://wrd.zdqjudy.top

int *p = &a;  *p = 5;
来源：http://myc.ywan-chungtsiang.top

[S11] C：逐行读文件
来源：http://nbu.andypj.xyz

FILE *f = fopen("a.txt", "r");
来源：http://jsf.yvedp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://eey.fengsongda.top

fclose(f);
来源：http://hmz.pycfn.com

[S12] C：写文件
来源：http://ssq.jinqigfzy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ynm.sweek.top

[S13] C：宏定义
来源：http://rcs.tarul.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bcl.chenzaomai.com

[S14] C：枚举
来源：http://byw.dianchejie.cn

enum Color { RED, GREEN, BLUE };
来源：http://yyt.hnxiangtu.top

[S15] C：类型转换
来源：http://saq.smart0.xyz

(double) a / b
来源：http://vfj.epnwcf.com

[S16] C：位操作置位
来源：http://wop.fzhhl.top

x |= (1 << 3);
来源：http://zlk.hnxiangtu.top

[S17] C：安全拼接字符串
来源：http://bey.tarul.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mnb.iojbl.cn

[S18] C：命令行参数
来源：http://adb.shanyushiyangtech.top

int main(int argc, char **argv)
来源：http://wfd.epnwcf.com

[S19] C：快速排序
来源：http://ywp.tianlin.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://byn.pengpengdd.cyou

[S20] C：二分查找
来源：http://nzd.ctjpmb.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lto.cdnleiting.top

[S21] C：字符类别判断
来源：http://ciw.hesvh.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nkw.jlsjyb.cn

[S22] C：字符串转数字
来源：http://gxn.tanke756.top

atoi("42");  strtod("3.14", NULL);
来源：http://hzg.zhongyouzk.top

[S23] C：随机数
来源：http://pim.gogol.net.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ocm.smart0.xyz

[S24] C：获取本地时间
来源：http://cbp.sysykeji.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tuv.jlsjyb.cn

[S25] C：内存拷贝
来源：http://zhi.yj20258.top

memcpy(dst, src, n);
来源：http://piy.jlsjyb.cn

[S26] C：内存清零
来源：http://kat.ctjpmb.com

memset(a, 0, sizeof a);
来源：http://ube.dianchejie.cn

[S27] C：定义常量
来源：http://npx.quarkkingdee.top

const double PI = 3.14159;
来源：http://cpf.c1oappe.top

[S28] C：静态变量
来源：http://jhu.guannengcc.top

static int counter = 0;
来源：http://tmm.hammf.cn

[S29] C：变参函数
来源：http://uhl.316326.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nfj.uphjek.com

[S30] C：头文件保护
来源：http://kgt.hysaishi.cn

#ifndef X_H
来源：http://ucw.zycfv.cn

#define X_H
来源：http://xsd.tianlin.xyz

#endif
来源：http://yvs.ctjpmb.com

[S31] C++：Hello World
来源：http://bsd.gzhubu.top

#include <iostream>
来源：http://zqh.vehdjk.com

int main() { std::cout << "Hello\n"; }
来源：http://lea.cashguo.top

[S32] C++：字符串
来源：http://lsk.ywan-chungtsiang.top

std::string s = "hi";  s += "!";
来源：http://ulg.52xcode.cn

[S33] C++：vector 增删
来源：http://wjw.jqgufenzy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://poz.cucudq.cn

[S34] C++：遍历 vector
来源：http://cmb.svipenyu.cn

for (auto &x : v) { std::cout << x; }
来源：http://ndm.cheryme.top

[S35] C++：map
来源：http://ufw.gogol.net.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qgg.xuetiantiany.cn

[S36] C++：unordered_map
来源：http://xqb.yuanzhike.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pxc.shangyingyoupin.top

[S37] C++：set
来源：http://dlx.yvedp.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nsg.bbcook.cn

[S38] C++：排序
来源：http://mcr.smart0.xyz

std::sort(v.begin(), v.end());
来源：http://inm.fehbvm.com

[S39] C++：自定义比较器排序
来源：http://ymb.yuanzhike.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rfe.ehwqpu.com

[S40] C++：查找元素
来源：http://yol.yj20258888.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kzy.yuxming.cn

[S41] C++：类与构造函数
来源：http://tzj.shangyingyoupin.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pnd.yonumen.top

[S42] C++：继承与虚函数
来源：http://oee.dianchejie.cn

class B : public Base { public: void f() override {} };
来源：http://mvq.guowangkeji.top

[S43] C++：智能指针
来源：http://yps.epnwcf.com

auto p = std::make_unique<int>(5);
来源：http://zlp.birdmap.top

[S44] C++：引用传参
来源：http://ras.bbcook.cn

void inc(int &x) { ++x; }
来源：http://jpd.yj20258.top

[S45] C++：lambda
来源：http://vtn.zhijiandao.cn

auto add = [](int a, int b) { return a + b; };
来源：http://oer.ywan-chungtsiang.top

[S46] C++：函数模板
来源：http://idl.zhoulong.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rab.yvedp.cn

[S47] C++：结构化绑定遍历
来源：http://xrw.fzhhl.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nfo.zhaomingkeji.xyz

[S48] C++：逐行读文件
来源：http://kup.bbcook.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qja.bjfxy.top

while (std::getline(in, line)) { }
来源：http://trc.zhengqikj.top

[S49] C++：写文件
来源：http://fjy.zhaomingkeji.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pyy.zhixingplan.top

[S50] C++：格式化数字
来源：http://hjn.ybcxt.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gcv.ctjpmb.com

[S51] C++：显式类型转换
来源：http://ple.yuxming.cn

static_cast<double>(a) / b
来源：http://kyi.yonumen.top

[S52] C++：const 与 noexcept
来源：http://apj.yonumen.top

int size() const noexcept { return n_; }
来源：http://qpo.sweek.top

[S53] C++：移动语义
来源：http://uqe.xinyue.icu

std::vector<int> w = std::move(v);
来源：http://qyr.gogol.net.cn

[S54] C++：异常处理
来源：http://eho.yuanzhike.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fvd.smart0.xyz

[S55] C++：结构化绑定
来源：http://ntt.fehbvm.com

auto [a, b] = std::make_pair(1, 2);
来源：http://srq.cdnleiting.top

[S56] C++：optional
来源：http://pmv.cashguo.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lhp.sjlbkw.cn

[S57] C++：编译期常量
来源：http://ivv.gaohongyu789.top

constexpr int N = 10;
来源：http://vpf.0kj1m.cn

[S58] C++：命名空间
来源：http://nyq.pengpengdd.cyou

namespace ns { int f() { return 1; } }
来源：http://dxr.tanke756.top

[S59] C++：静态断言
来源：http://jvx.zhiwuduotai.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mhi.c1oappe.top

[S60] C++：遍历并删除元素
来源：http://ijy.ywan-chungtsiang.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ach.hfpthk.cn

================================================================================
来源：http://sii.fengsongda.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tdi.gogol.net.cn

================================================================================
来源：http://ykg.sweek.top

[T01] Kotlin：Hello World
来源：http://kdy.epnwcf.com

println("Hello")
来源：http://zvs.c1oappe.top

[T02] Kotlin：变量
来源：http://mpw.wangdashe.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://leb.tianlin.xyz

[T03] Kotlin：字符串模板
来源：http://xzl.havefunace.top

"值: $b"
来源：http://nse.52xcode.cn

[T04] Kotlin：空安全
来源：http://fny.snrcjt.cn

val n: String? = null;  n?.length
来源：http://wjy.xylfe.cn

[T05] Kotlin：when 表达式
来源：http://evh.shangyingyoupin.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ybm.yonumen.top

[T06] Kotlin：集合映射
来源：http://ipg.xuetiantiany.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tsv.cucudq.cn

[T07] Kotlin：集合过滤
来源：http://omr.jqgufenzy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://sqw.dianchejie.cn

[T08] Kotlin：数据类
来源：http://eqb.cdnleiting.top

data class User(val name: String, val age: Int)
来源：http://uko.ctjpmb.com

[T09] Kotlin：扩展函数
来源：http://jot.yuxming.cn

fun String.exclaim() = this + "!"
来源：http://jvo.vehdjk.com

[T10] Kotlin：默认参数
来源：http://szg.snrcjt.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://txx.chenlongwang.top

[T11] Kotlin：协程
来源：http://bzv.fktsv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bji.cheryme.top

[T12] Kotlin：解构声明
来源：http://pll.chenjidiqi.icu

val (a, b) = Pair(1, 2)
来源：http://ogr.fengsongda.top

[T13] Kotlin：只读 Map
来源：http://ifu.cashguo.top

val m = mapOf("a" to 1)
来源：http://zrx.ydzc1.top

[T14] Kotlin：循环
来源：http://szw.yonumen.top

for (i in 1..10) println(i)
来源：http://ubz.quarkkingdee.top

[T15] Kotlin：接口
来源：http://ury.zhongyouzk.top

interface Shape { fun area(): Double }
来源：http://eit.zhixingplan.top

[T16] Swift：Hello World
来源：http://ake.hcnkem.com

print("Hello")
来源：http://eaa.hysaishi.cn

[T17] Swift：变量与常量
来源：http://oni.guowangkeji.top

var a = 1;  let b = 2
来源：http://etl.vehdjk.com

[T18] Swift：字符串插值
来源：http://jtx.zhengqikj.top

"值: \(b)"
来源：http://dnf.fzhhl.top

[T19] Swift：可选绑定
来源：http://erd.ydjk.org.cn

if let n = opt { print(n) }
来源：http://igy.hysaishi.cn

[T20] Swift：数组操作
来源：http://avv.sufxvd.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gco.ehwqpu.com

[T21] Swift：遍历
来源：http://esx.ywan-chungtsiang.top

for x in a { print(x) }
来源：http://mlm.zhaomingkeji.xyz

[T22] Swift：字典
来源：http://uot.9152youxi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://sgq.cdnleiting.top

[T23] Swift：函数
来源：http://gcx.andypj.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kho.yangfankeji.com

[T24] Swift：闭包
来源：http://jbb.shanyushiyangkeji.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://rbo.havefunace.top


<!-- 参考信息 -->