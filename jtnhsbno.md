代发 wailian999

echo "${#s}"
来源：http://cyi.ehwqpu.com

[R22] 截取子串
来源：http://ejx.shangyingyoupin.top

echo "${s:0:5}"
来源：http://nll.fehbvm.com

[R23] 字符串替换
来源：http://psx.yuxming.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jig.ydzc1.top

[R24] 大小写转换
来源：http://msh.jqgfzy.top

echo "${s^^}"; echo "${s,,}"
来源：http://pwx.gaohongyu789.top

[R25] 去后缀 / 去前缀
来源：http://vqm.hongshengwenyu.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://mdd.yueranfly.top

[R26] 命令替换
来源：http://khv.ydzc1.top

now=$(date +%F); echo "$now"
来源：http://gqz.jqgufenzy.top

[R27] 算术展开
来源：http://xlx.gaohongyu789.top

echo $((1 + 2 * 3))
来源：http://rmx.fengsongda.top

[R28] 浮点运算
来源：http://myx.feifeiyinyue.top

echo "scale=2; 10/3" | bc
来源：http://ajm.uphjek.com

[R29] 定义函数
来源：http://bsd.zhiwuduotai.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zuk.sweek.top

[R30] 函数返回状态码
来源：http://yir.xylfe.cn

f() { return 0; }; f || echo "失败了"
来源：http://tma.gogol.net.cn

[R31] 局部变量
来源：http://vaf.sjlbkw.cn

f() { local x=1; echo "$x"; }
来源：http://dxq.shangyingyoupin.top

[R32] 参数个数校验
来源：http://omb.aibaodan.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://obz.birdmap.top

[R33] 捕获错误并提示行号
来源：http://hyb.yuanzhike.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://eyn.yj20258.top

[R34] 退出时清理
来源：http://oza.0kj1m.cn

trap 'rm -f "$tmp"' EXIT
来源：http://dhz.fehbvm.com

[R35] 后台执行并等待
来源：http://val.aizwys.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://pdu.fehbvm.com

[R36] 并发执行多个任务
来源：http://hxs.iojbl.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://irp.zhongyouzk.top

[R37] 把输出赋给变量
来源：http://mcd.tarul.cn

files=$(ls -1)
来源：http://mwa.ybcxt.top

[R38] 管道串联
来源：http://vnr.hongshengwenyu.top

cat a.txt | grep -i error | wc -l
来源：http://bkv.jianghu66.top

[R39] 重定向标准输出与错误
来源：http://ame.jyoumei.cn

cmd > out.log 2>&1
来源：http://tuj.havefunace.top

[R40] 追加写日志
来源：http://hze.dianchejie.cn

echo "log" >> out.log
来源：http://ykd.mhx1999.top

[R41] 丢弃输出
来源：http://rlu.fengsongda.top

cmd >/dev/null 2>&1
来源：http://ucb.shanyushiyangkeji.top

[R42] 输入重定向
来源：http://gxs.cqqwz.cn

wc -l < a.txt
来源：http://kgw.hammf.cn

[R43] 按名字查找文件
来源：http://irv.jinghuilouyu.cn

find . -name "*.log" -type f
来源：http://fcw.guannengcc.top

[R44] 按修改时间查找
来源：http://rez.aizwys.cn

find . -mtime -7 -type f
来源：http://kew.ctjpmb.com

[R45] 批量删除
来源：http://jif.sweek.top

find . -name "*.tmp" -delete
来源：http://yzd.daria6918.cn

[R46] 递归替换文件内容
来源：http://rqg.yonumen.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xes.pengpengdd.cyou

[R47] sed 单行替换
来源：http://axp.ywan-chungtsiang.top

sed -i 's/foo/bar/g' a.txt
来源：http://jky.shanyushiyangkeji.top

[R48] awk 取指定列
来源：http://piz.gzhubu.top

awk '{print $1, $3}' a.txt
来源：http://hmj.yj20258.top

[R49] awk 带条件
来源：http://rtk.ydzc1.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qwn.cucudq.cn

[R50] awk 求和
来源：http://xze.nanxuanxn.top

awk '{s += $2} END {print s}' a.txt
来源：http://gvo.zhiwuduotai.top

[R51] 排序去重取前几
来源：http://dgi.cucudq.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://rqq.kuanghao11.cn

[R52] 统计行数
来源：http://usm.ehwqpu.com

wc -l a.txt
来源：http://sec.gaohongyu789.top

[R53] 查看文件头与实时尾
来源：http://cmd.cdnleiting.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rxd.snrcjt.cn

[R54] 比较两个文件
来源：http://slo.haohaochexian.top

diff a.txt b.txt
来源：http://vpc.shanyushiyangkeji.top

[R55] 压缩与解压
来源：http://kys.shzxlz.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dja.quarkkingdee.top

[R56] 远程拷贝
来源：http://umq.gaohongyu789.top

scp file user@host:/path/
来源：http://qbb.sweek.top

[R57] 远程执行命令
来源：http://ecz.svipenyu.cn

ssh user@host 'uptime'
来源：http://ncr.daria6918.cn

[R58] 下载文件
来源：http://ywu.c1oappe.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gzv.guowangkeji.top

[R59] 发 POST JSON
来源：http://hpf.pycfn.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://phk.shanyushiyangtech.top

[R60] 只看 HTTP 状态码
来源：http://apj.hnqzz.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://phg.hesvh.cn

[R61] 磁盘占用
来源：http://vub.uphjek.com

df -h;  du -sh *
来源：http://cwi.hammf.cn

[R62] 找最占空间的文件
来源：http://diz.pycfn.com

du -ah . | sort -rh | head -10
来源：http://yfz.yvedp.cn

[R63] 内存与进程
来源：http://cgz.nwbrower.top

free -h;  ps aux | grep nginx
来源：http://owv.yanxiufei.cn

[R64] 结束进程
来源：http://wud.hysaishi.cn

kill -9 $(pgrep -f app.py)
来源：http://pdv.fzhhl.top

[R65] 查看端口占用
来源：http://kvv.gaohongyu789.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wrc.daria6918.cn

[R66] 定时任务
来源：http://eho.ehwqpu.com

crontab -e;  crontab -l
来源：http://jjr.yj20258888.top

[R67] 生成随机十六进制串
来源：http://axf.sysykeji.top

openssl rand -hex 16
来源：http://xgi.feifeiyinyue.top

[R68] 计算文件校验值
来源：http://mhj.zdqjudy.top

sha256sum a.txt;  md5sum a.txt
来源：http://yii.andypj.xyz

[R69] 生成随机密码
来源：http://txf.haohaochexian.top

head -c 16 /dev/urandom | base64
来源：http://ftv.quarkkingdee.top

[R70] 时间戳与互转
来源：http://upv.chenlongwang.top

date +%s;  date -d @1700000000
来源：http://qvv.nanxinkj.top

[R71] 日期格式化
来源：http://xzv.fktsv.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://glm.yj20258888.top

[R72] 等待端口就绪
来源：http://obp.cucudq.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cnq.hywenlv.cn

[R73] 分割大日志
来源：http://qor.ivvv.top

split -l 1000 big.log part_
来源：http://ksi.fanxiaobao.xyz

[R74] 批量重命名
来源：http://vkr.hnqzz.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ijr.zycfv.cn

[R75] 导出环境变量
来源：http://vqk.sjlbkw.cn

export PATH="$HOME/bin:$PATH"
来源：http://edz.chenlongwang.top

[R76] 使用临时文件
来源：http://ufo.tianlin.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ipt.daxiang520.top

[R77] 读取用户输入
来源：http://yij.sweek.top

read -rp "请输入: " ans
来源：http://rfq.nanxinkj.top

[R78] 交互式菜单
来源：http://dsp.ydjk.org.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://fyr.guowangkeji.top

[R79] 解析命令行选项
来源：http://kud.birdmap.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jgj.zdqjudy.top

[R80] 查看脚本执行耗时
来源：http://csg.zhijiandao.cn

time ./run.sh
来源：http://oni.jyoumei.cn

================================================================================
来源：http://edg.fanxiaobao.xyz

S. C / C++ 专题
来源：http://ybu.pengpengdd.cyou

================================================================================
来源：http://vwa.cqqwz.cn

[S01] C：Hello World
来源：http://wnf.zdqjudy.top

#include <stdio.h>
来源：http://clf.sjlbkw.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gvu.epnwcf.com

[S02] C：变量与格式化输出
来源：http://fbv.fanxiaobao.xyz

int a = 10; printf("%d\n", a);
来源：http://egi.jinghuilouyu.cn

[S03] C：读入整数
来源：http://gyc.sjlbkw.cn

int x; scanf("%d", &x);
来源：http://rcs.ybcxt.top

[S04] C：字符串复制
来源：http://yjg.xuanzx.com

char dst[32]; strcpy(dst, "hi");
来源：http://qzz.zdqjudy.top

[S05] C：字符串长度
来源：http://cuc.sjlbkw.cn

strlen(s)
来源：http://odv.xziqi.cn

[S06] C：字符串比较
来源：http://wdj.gotoacloud.top

strcmp(a, b) == 0
来源：http://iak.ybcxt.top

[S07] C：数组遍历求和
来源：http://ndq.hesvh.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://suu.havefunace.top

[S08] C：动态内存分配与释放
来源：http://vvf.jyoumei.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lau.wangdashe.top

[S09] C：结构体定义与初始化
来源：http://cks.sufxvd.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://utu.zdqjudy.top

[S10] C：指针与解引用
来源：http://hlv.yfazqb.com

int *p = &a;  *p = 5;
来源：http://usu.haohaochexian.top

[S11] C：逐行读文件
来源：http://uch.ywan-chungtsiang.top

FILE *f = fopen("a.txt", "r");
来源：http://pfm.yvedp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://wev.cdnleiting.top

fclose(f);
来源：http://ivb.yangfankeji.com

[S12] C：写文件
来源：http://kak.shanyushiyangtech.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://apf.daria6918.cn

[S13] C：宏定义
来源：http://nvx.wangshuangyany.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dsj.jinqigfzy.top

[S14] C：枚举
来源：http://puz.hysaishi.cn

enum Color { RED, GREEN, BLUE };
来源：http://grw.fzhhl.top

[S15] C：类型转换
来源：http://adr.jqgufenzy.top

(double) a / b
来源：http://lqm.yonumen.top

[S16] C：位操作置位
来源：http://zos.guannengcc.top

x |= (1 << 3);
来源：http://fpe.gogol.net.cn

[S17] C：安全拼接字符串
来源：http://utl.tianlin.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vmu.jinqigfzy.top

[S18] C：命令行参数
来源：http://nxw.gogol.net.cn

int main(int argc, char **argv)
来源：http://wmf.cucudq.cn

[S19] C：快速排序
来源：http://gps.sysykeji.top

qsort(a, n, sizeof(int), cmp);
来源：http://yhf.havefunace.top

[S20] C：二分查找
来源：http://fxt.wangdashe.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dza.aibaodan.cn

[S21] C：字符类别判断
来源：http://bed.gzhubu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xwj.yuxming.cn

[S22] C：字符串转数字
来源：http://amy.bbcook.cn

atoi("42");  strtod("3.14", NULL);
来源：http://opa.feifeiyinyue.top

[S23] C：随机数
来源：http://usl.zhoulong.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://kem.hywenlv.cn

[S24] C：获取本地时间
来源：http://acz.hammf.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ygu.fengsongda.top

[S25] C：内存拷贝
来源：http://pll.fengsongda.top

memcpy(dst, src, n);
来源：http://rju.quarkkingdee.top

[S26] C：内存清零
来源：http://kqb.tanke756.top

memset(a, 0, sizeof a);
来源：http://wae.hfpthk.cn

[S27] C：定义常量
来源：http://sbo.jianghu66.top

const double PI = 3.14159;
来源：http://dyz.yj20258888.top

[S28] C：静态变量
来源：http://ilb.ywan-chungtsiang.top

static int counter = 0;
来源：http://gul.sufxvd.cn

[S29] C：变参函数
来源：http://xsi.tarul.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wfs.jqgufenzy.top

[S30] C：头文件保护
来源：http://gbo.pengpengdd.cyou

#ifndef X_H
来源：http://qpl.shangyingyoupin.top

#define X_H
来源：http://jnm.ctjpmb.com

#endif
来源：http://qwt.svipenyu.cn

[S31] C++：Hello World
来源：http://gok.ctjpmb.com

#include <iostream>
来源：http://ded.quarkkingdee.top

int main() { std::cout << "Hello\n"; }
来源：http://eqm.zhoulong.xyz

[S32] C++：字符串
来源：http://tdx.ivvv.top

std::string s = "hi";  s += "!";
来源：http://oah.xinyue.icu

[S33] C++：vector 增删
来源：http://mzj.jqgufenzy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tro.hnqzz.top

[S34] C++：遍历 vector
来源：http://bko.hongshengwenyu.top

for (auto &x : v) { std::cout << x; }
来源：http://pat.meibo888.top

[S35] C++：map
来源：http://vxw.ywan-chungtsiang.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xcs.gaohongyu789.top

[S36] C++：unordered_map
来源：http://seb.ywan-chungtsiang.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sqc.316326.xyz

[S37] C++：set
来源：http://jwy.jyoumei.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nse.sweek.top

[S38] C++：排序
来源：http://fnf.jinyuanbaomall.cn

std::sort(v.begin(), v.end());
来源：http://jdb.tarul.cn

[S39] C++：自定义比较器排序
来源：http://csa.hfpthk.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uzx.hnqzz.top

[S40] C++：查找元素
来源：http://boo.birdmap.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ghc.gotoacloud.top

[S41] C++：类与构造函数
来源：http://tjx.sysykeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qad.yongpay.top

[S42] C++：继承与虚函数
来源：http://tms.sjlbkw.cn

class B : public Base { public: void f() override {} };
来源：http://hqd.c1oappe.top

[S43] C++：智能指针
来源：http://eti.vqdsnc.cn

auto p = std::make_unique<int>(5);
来源：http://snr.tanke756.top

[S44] C++：引用传参
来源：http://qyf.chenzaomai.com

void inc(int &x) { ++x; }
来源：http://npf.vqdsnc.cn

[S45] C++：lambda
来源：http://vrw.zhixingplan.top

auto add = [](int a, int b) { return a + b; };
来源：http://mhs.shangyingyoupin.top

[S46] C++：函数模板
来源：http://ewx.gogol.net.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://eub.nanxuanxn.top

[S47] C++：结构化绑定遍历
来源：http://cbl.shanyushiyangtech.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zqi.birdmap.top

[S48] C++：逐行读文件
来源：http://paf.yfazqb.com

std::ifstream in("a.txt");  std::string line;
来源：http://bgu.dianchejie.cn

while (std::getline(in, line)) { }
来源：http://twl.c1oappe.top

[S49] C++：写文件
来源：http://uzb.yj20258.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hfz.zhaomingkeji.xyz

[S50] C++：格式化数字
来源：http://fcp.52xcode.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fiz.chenzaomai.com

[S51] C++：显式类型转换
来源：http://vwu.shzxlz.cn

static_cast<double>(a) / b
来源：http://svz.yueranfly.top

[S52] C++：const 与 noexcept
来源：http://ubm.shzxlz.cn

int size() const noexcept { return n_; }
来源：http://qhj.wangshuangyany.cn

[S53] C++：移动语义
来源：http://cbm.tarul.cn

std::vector<int> w = std::move(v);
来源：http://cek.yuanzhike.top

[S54] C++：异常处理
来源：http://qox.chenlongwang.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://npv.c1oappe.top

[S55] C++：结构化绑定
来源：http://wku.shzxlz.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://idj.zycfv.cn

[S56] C++：optional
来源：http://awr.zhixingplan.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dhc.yueranfly.top

[S57] C++：编译期常量
来源：http://ttc.bbcook.cn

constexpr int N = 10;
来源：http://qif.dianchejie.cn

[S58] C++：命名空间
来源：http://xtr.fanxiaobao.xyz

namespace ns { int f() { return 1; } }
来源：http://isc.fktsv.cn

[S59] C++：静态断言
来源：http://myb.ctjpmb.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dqt.9152youxi.cn

[S60] C++：遍历并删除元素
来源：http://hud.tian-w.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://asp.9152youxi.cn

================================================================================
来源：http://ixo.cashguo.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://psn.ivvv.top

================================================================================
来源：http://mnb.snrcjt.cn

[T01] Kotlin：Hello World
来源：http://dsd.shzxlz.cn

println("Hello")
来源：http://mxk.sxryk.cn

[T02] Kotlin：变量
来源：http://zxn.yuxming.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hpq.jinghuilouyu.cn

[T03] Kotlin：字符串模板
来源：http://qty.yj202588.top

"值: $b"
来源：http://zpz.wangshuangyany.cn

[T04] Kotlin：空安全
来源：http://cth.jqgufenzy.top

val n: String? = null;  n?.length
来源：http://upw.jianghu66.top

[T05] Kotlin：when 表达式
来源：http://znz.hfpthk.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kxw.wangdashe.top

[T06] Kotlin：集合映射
来源：http://psm.zhengqikj.top

listOf(1, 2, 3).map { it * 2 }
来源：http://gyw.jinqigfzy.top

[T07] Kotlin：集合过滤
来源：http://rhg.uphjek.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://jlo.hcnkem.com

[T08] Kotlin：数据类
来源：http://fgc.uphjek.com

data class User(val name: String, val age: Int)
来源：http://jtw.xylfe.cn

[T09] Kotlin：扩展函数
来源：http://ryc.daria6918.cn

fun String.exclaim() = this + "!"
来源：http://sso.zhiwuduotai.top

[T10] Kotlin：默认参数
来源：http://kvo.jianghu66.top

fun greet(name: String = "World") = "Hi $name"
来源：http://wnt.jinqigfzy.top

[T11] Kotlin：协程
来源：http://yxo.xingfuxueyuan.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://shs.zhiwuduotai.top

[T12] Kotlin：解构声明
来源：http://spb.yj20258888.top

val (a, b) = Pair(1, 2)
来源：http://npf.yj20258.top

[T13] Kotlin：只读 Map
来源：http://tpv.hfpthk.cn

val m = mapOf("a" to 1)
来源：http://qds.jlsjyb.cn

[T14] Kotlin：循环
来源：http://yrf.ppjwa.cn

for (i in 1..10) println(i)
来源：http://noz.zhongyouzk.top

[T15] Kotlin：接口
来源：http://bao.xinyue.icu

interface Shape { fun area(): Double }
来源：http://raw.cucudq.cn

[T16] Swift：Hello World
来源：http://jpl.xuetiantiany.cn

print("Hello")
来源：http://hid.shzxlz.cn

[T17] Swift：变量与常量
来源：http://spd.redwolf501.top

var a = 1;  let b = 2
来源：http://mxi.guowangkeji.top

[T18] Swift：字符串插值
来源：http://iiz.zdqjudy.top

"值: \(b)"
来源：http://erz.gotoacloud.top

[T19] Swift：可选绑定
来源：http://ykq.nwbrower.top

if let n = opt { print(n) }
来源：http://ehj.jqgfzy.top

[T20] Swift：数组操作
来源：http://vvp.cashguo.top

var a = [1, 2, 3];  a.append(4)
来源：http://wkq.yanxiufei.cn

[T21] Swift：遍历
来源：http://gfj.gogol.net.cn

for x in a { print(x) }
来源：http://vkq.jiagoushi.top

[T22] Swift：字典
来源：http://fmt.redwolf501.top

var d = ["a": 1];  d["b"] = 2
来源：http://izg.zdqjudy.top

[T23] Swift：函数
来源：http://foi.xuetiantiany.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xpt.ydjk.org.cn

[T24] Swift：闭包
来源：http://cbu.9152youxi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ctl.zhoulong.xyz


<!-- 参考信息 -->