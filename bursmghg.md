代发 wailian999

echo $((1 + 2 * 3))
来源：http://gcb.bbcook.cn

[R28] 浮点运算
来源：http://caa.sweek.top

echo "scale=2; 10/3" | bc
来源：http://qyz.cqqwz.cn

[R29] 定义函数
来源：http://kmr.pycfn.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mpr.fehbvm.com

[R30] 函数返回状态码
来源：http://tcp.nanxinkj.top

f() { return 0; }; f || echo "失败了"
来源：http://coz.ywan-chungtsiang.top

[R31] 局部变量
来源：http://qbn.9152youxi.cn

f() { local x=1; echo "$x"; }
来源：http://zbo.cucudq.cn

[R32] 参数个数校验
来源：http://rcf.316326.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lre.ydjk.org.cn

[R33] 捕获错误并提示行号
来源：http://hvv.jinyuanbaomall.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dob.xingfuxueyuan.xyz

[R34] 退出时清理
来源：http://bsn.zhiwuduotai.top

trap 'rm -f "$tmp"' EXIT
来源：http://klq.nwbrower.top

[R35] 后台执行并等待
来源：http://icl.pycfn.com

sleep 5 & pid=$!; wait "$pid"
来源：http://lvp.yangfankeji.com

[R36] 并发执行多个任务
来源：http://hlt.gotoacloud.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blh.svipenyu.cn

[R37] 把输出赋给变量
来源：http://jcx.snrcjt.cn

files=$(ls -1)
来源：http://ncj.sxryk.cn

[R38] 管道串联
来源：http://fdb.yfazqb.com

cat a.txt | grep -i error | wc -l
来源：http://ypz.tanke756.top

[R39] 重定向标准输出与错误
来源：http://jfa.hnxiangtu.top

cmd > out.log 2>&1
来源：http://oza.gogol.net.cn

[R40] 追加写日志
来源：http://dmk.zhixingplan.top

echo "log" >> out.log
来源：http://ytc.sufxvd.cn

[R41] 丢弃输出
来源：http://irh.vehdjk.com

cmd >/dev/null 2>&1
来源：http://rki.316326.xyz

[R42] 输入重定向
来源：http://wtq.yfazqb.com

wc -l < a.txt
来源：http://ifb.tian-w.cn

[R43] 按名字查找文件
来源：http://usw.hammf.cn

find . -name "*.log" -type f
来源：http://uem.ybcxt.top

[R44] 按修改时间查找
来源：http://vmm.tian-w.cn

find . -mtime -7 -type f
来源：http://sbm.zhengqikj.top

[R45] 批量删除
来源：http://kdi.cucudq.cn

find . -name "*.tmp" -delete
来源：http://fqe.ydjk.org.cn

[R46] 递归替换文件内容
来源：http://ysw.yj20258.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ydg.ivvv.top

[R47] sed 单行替换
来源：http://kzq.shanyushiyangtech.top

sed -i 's/foo/bar/g' a.txt
来源：http://oub.yuxming.cn

[R48] awk 取指定列
来源：http://zkd.yanxiufei.cn

awk '{print $1, $3}' a.txt
来源：http://rrj.nanxinkj.top

[R49] awk 带条件
来源：http://rkx.birdmap.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qou.shuidangran.top

[R50] awk 求和
来源：http://rju.yuxming.cn

awk '{s += $2} END {print s}' a.txt
来源：http://cbp.gaohongyu789.top

[R51] 排序去重取前几
来源：http://txu.sxryk.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://iei.bbcook.cn

[R52] 统计行数
来源：http://ebn.sufxvd.cn

wc -l a.txt
来源：http://lwu.jqgfzy.top

[R53] 查看文件头与实时尾
来源：http://xhr.yuxming.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ilg.snrcjt.cn

[R54] 比较两个文件
来源：http://xxl.zdbjq.cn

diff a.txt b.txt
来源：http://nxs.yuanzhike.top

[R55] 压缩与解压
来源：http://hox.cucudq.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uor.fehbvm.com

[R56] 远程拷贝
来源：http://tin.52xcode.cn

scp file user@host:/path/
来源：http://brk.yj20258888.top

[R57] 远程执行命令
来源：http://xyg.ybcxt.top

ssh user@host 'uptime'
来源：http://pmq.sjlbkw.cn

[R58] 下载文件
来源：http://tvd.quarkkingdee.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fgr.yfazqb.com

[R59] 发 POST JSON
来源：http://uok.shangyingyoupin.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ebz.jinqigfzy.top

[R60] 只看 HTTP 状态码
来源：http://mex.yonumen.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zek.uphjek.com

[R61] 磁盘占用
来源：http://qqc.ybcxt.top

df -h;  du -sh *
来源：http://aly.zhiwuduotai.top

[R62] 找最占空间的文件
来源：http://jjl.ydzc1.top

du -ah . | sort -rh | head -10
来源：http://xda.xylfe.cn

[R63] 内存与进程
来源：http://gxu.zhixingplan.top

free -h;  ps aux | grep nginx
来源：http://thd.jinqigfzy.top

[R64] 结束进程
来源：http://bpj.yueranfly.top

kill -9 $(pgrep -f app.py)
来源：http://ptc.svipenyu.cn

[R65] 查看端口占用
来源：http://yod.jianghu66.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cpv.yanxiufei.cn

[R66] 定时任务
来源：http://zwj.yuanzhike.top

crontab -e;  crontab -l
来源：http://rsm.vehdjk.com

[R67] 生成随机十六进制串
来源：http://oas.cqqwz.cn

openssl rand -hex 16
来源：http://yho.tian-w.cn

[R68] 计算文件校验值
来源：http://dbe.zdqjudy.top

sha256sum a.txt;  md5sum a.txt
来源：http://qpy.ctjpmb.com

[R69] 生成随机密码
来源：http://hzn.dashuyun.cn

head -c 16 /dev/urandom | base64
来源：http://pdg.zhengqikj.top

[R70] 时间戳与互转
来源：http://ypq.xingfuxueyuan.xyz

date +%s;  date -d @1700000000
来源：http://yas.nanxinkj.top

[R71] 日期格式化
来源：http://itu.yfazqb.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://wsf.wangdashe.top

[R72] 等待端口就绪
来源：http://mic.yj202588.top

until nc -z localhost 3306; do sleep 1; done
来源：http://rha.haohaochexian.top

[R73] 分割大日志
来源：http://fja.daxiang520.top

split -l 1000 big.log part_
来源：http://xyw.tarul.cn

[R74] 批量重命名
来源：http://yzu.shanyushiyangtech.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rys.wangshuangyany.cn

[R75] 导出环境变量
来源：http://ntj.kuanghao11.cn

export PATH="$HOME/bin:$PATH"
来源：http://jke.wangshuangyany.cn

[R76] 使用临时文件
来源：http://tvp.fanxiaobao.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://reg.haohaochexian.top

[R77] 读取用户输入
来源：http://cew.sufxvd.cn

read -rp "请输入: " ans
来源：http://syn.guannengcc.top

[R78] 交互式菜单
来源：http://gvf.epnwcf.com

select opt in a b c; do echo "$opt"; break; done
来源：http://hum.wangshuangyany.cn

[R79] 解析命令行选项
来源：http://ljh.sysykeji.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hfv.jinqigufen.top

[R80] 查看脚本执行耗时
来源：http://jcj.zhongyouzk.top

time ./run.sh
来源：http://jpj.xinyue.icu

================================================================================
来源：http://pwm.aizwys.cn

S. C / C++ 专题
来源：http://whb.fanxiaobao.xyz

================================================================================
来源：http://juy.zdqjudy.top

[S01] C：Hello World
来源：http://lvi.dianchejie.cn

#include <stdio.h>
来源：http://qzz.jinqigufen.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://tbh.chenlongwang.top

[S02] C：变量与格式化输出
来源：http://ztx.sweek.top

int a = 10; printf("%d\n", a);
来源：http://zpa.zycfv.cn

[S03] C：读入整数
来源：http://qry.shanyushiyangkeji.top

int x; scanf("%d", &x);
来源：http://muw.jianghu66.top

[S04] C：字符串复制
来源：http://kpo.tanke756.top

char dst[32]; strcpy(dst, "hi");
来源：http://ayi.jinghuilouyu.cn

[S05] C：字符串长度
来源：http://vsy.pengpengdd.cyou

strlen(s)
来源：http://dgx.haohaochexian.top

[S06] C：字符串比较
来源：http://ech.chenzaomai.com

strcmp(a, b) == 0
来源：http://pqb.cucudq.cn

[S07] C：数组遍历求和
来源：http://wrk.cqqwz.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uad.bjfxy.top

[S08] C：动态内存分配与释放
来源：http://yky.feifeiyinyue.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gje.dianchejie.cn

[S09] C：结构体定义与初始化
来源：http://gxu.shanyushiyangkeji.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qvt.haohaochexian.top

[S10] C：指针与解引用
来源：http://ddc.hcnkem.com

int *p = &a;  *p = 5;
来源：http://ykt.ppjwa.cn

[S11] C：逐行读文件
来源：http://voh.chenjidiqi.icu

FILE *f = fopen("a.txt", "r");
来源：http://pdx.chenlongwang.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://yvn.yj20258888.top

fclose(f);
来源：http://bjc.zhijiandao.cn

[S12] C：写文件
来源：http://oyl.cdnleiting.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pec.birdmap.top

[S13] C：宏定义
来源：http://szp.zdbjq.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xtb.yfazqb.com

[S14] C：枚举
来源：http://vnr.ydjk.org.cn

enum Color { RED, GREEN, BLUE };
来源：http://blt.zdqjudy.top

[S15] C：类型转换
来源：http://ojw.zhongyouzk.top

(double) a / b
来源：http://qfl.yongpay.top

[S16] C：位操作置位
来源：http://aks.chenzaomai.com

x |= (1 << 3);
来源：http://axd.zhiwuduotai.top

[S17] C：安全拼接字符串
来源：http://cdq.gzhubu.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bmw.yfazqb.com

[S18] C：命令行参数
来源：http://rwm.pycfn.com

int main(int argc, char **argv)
来源：http://rnd.meibo888.top

[S19] C：快速排序
来源：http://xwb.yvedp.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zkq.cdnleiting.top

[S20] C：二分查找
来源：http://kwk.xinyue.icu

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gvh.aizwys.cn

[S21] C：字符类别判断
来源：http://cpz.ivvv.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vqu.vqdsnc.cn

[S22] C：字符串转数字
来源：http://zqu.yongpay.top

atoi("42");  strtod("3.14", NULL);
来源：http://azk.cucudq.cn

[S23] C：随机数
来源：http://dio.tanke756.top

srand(time(NULL));  int r = rand() % 100;
来源：http://you.hfpthk.cn

[S24] C：获取本地时间
来源：http://zjk.yuanzhike.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fbj.zhongyouzk.top

[S25] C：内存拷贝
来源：http://xxu.xuanzx.com

memcpy(dst, src, n);
来源：http://ska.chenlongwang.top

[S26] C：内存清零
来源：http://bya.yuanzhike.top

memset(a, 0, sizeof a);
来源：http://rms.c1oappe.top

[S27] C：定义常量
来源：http://udp.ehwqpu.com

const double PI = 3.14159;
来源：http://jdy.tian-w.cn

[S28] C：静态变量
来源：http://mue.ydzc1.top

static int counter = 0;
来源：http://how.shuidangran.top

[S29] C：变参函数
来源：http://syy.vqdsnc.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ceq.cqqwz.cn

[S30] C：头文件保护
来源：http://muh.shzxlz.cn

#ifndef X_H
来源：http://aww.316326.xyz

#define X_H
来源：http://ubh.ybcxt.top

#endif
来源：http://lqm.andypj.xyz

[S31] C++：Hello World
来源：http://suo.jlsjyb.cn

#include <iostream>
来源：http://qoy.vqdsnc.cn

int main() { std::cout << "Hello\n"; }
来源：http://ulc.jqgufenzy.top

[S32] C++：字符串
来源：http://svj.yueranfly.top

std::string s = "hi";  s += "!";
来源：http://gkv.zhongyouzk.top

[S33] C++：vector 增删
来源：http://iew.hfpthk.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jqv.zhengqikj.top

[S34] C++：遍历 vector
来源：http://ayt.meibo888.top

for (auto &x : v) { std::cout << x; }
来源：http://ozo.sysykeji.top

[S35] C++：map
来源：http://rnv.hcnkem.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qnf.jlsjyb.cn

[S36] C++：unordered_map
来源：http://muo.yfazqb.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kym.hcnkem.com

[S37] C++：set
来源：http://ysn.jlsjyb.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xvn.nanxuanxn.top

[S38] C++：排序
来源：http://wpa.jiagoushi.top

std::sort(v.begin(), v.end());
来源：http://wop.ydzc1.top

[S39] C++：自定义比较器排序
来源：http://oby.pycfn.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://slf.yj20258.top

[S40] C++：查找元素
来源：http://orm.yuxming.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://izs.uphjek.com

[S41] C++：类与构造函数
来源：http://aor.jqgufenzy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tov.cdnleiting.top

[S42] C++：继承与虚函数
来源：http://qdo.jyoumei.cn

class B : public Base { public: void f() override {} };
来源：http://clz.nwbrower.top

[S43] C++：智能指针
来源：http://ijs.jlsjyb.cn

auto p = std::make_unique<int>(5);
来源：http://jsa.sweek.top

[S44] C++：引用传参
来源：http://ybm.uphjek.com

void inc(int &x) { ++x; }
来源：http://ath.xziqi.cn

[S45] C++：lambda
来源：http://mkk.wangshuangyany.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xpt.zhaomingkeji.xyz

[S46] C++：函数模板
来源：http://ngi.hammf.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://txw.epnwcf.com

[S47] C++：结构化绑定遍历
来源：http://oor.sjlbkw.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://svk.zdbjq.cn

[S48] C++：逐行读文件
来源：http://sty.hywenlv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://cnn.zhiwuduotai.top

while (std::getline(in, line)) { }
来源：http://yjd.gotoacloud.top

[S49] C++：写文件
来源：http://awu.gzhubu.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jtw.xuetiantiany.cn

[S50] C++：格式化数字
来源：http://aqp.zhiwuduotai.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yvn.aizwys.cn

[S51] C++：显式类型转换
来源：http://dfv.ydjk.org.cn

static_cast<double>(a) / b
来源：http://zwh.xziqi.cn

[S52] C++：const 与 noexcept
来源：http://ubx.chenzaomai.com

int size() const noexcept { return n_; }
来源：http://ywn.yj202588.top

[S53] C++：移动语义
来源：http://fxj.fengsongda.top

std::vector<int> w = std::move(v);
来源：http://qgv.dashuyun.cn

[S54] C++：异常处理
来源：http://dvj.xuetiantiany.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ebs.hnqzz.top

[S55] C++：结构化绑定
来源：http://otg.chenlongwang.top

auto [a, b] = std::make_pair(1, 2);
来源：http://qkx.ydzc1.top

[S56] C++：optional
来源：http://avn.shuidangran.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pjj.jqgfzy.top

[S57] C++：编译期常量
来源：http://mio.ppjwa.cn

constexpr int N = 10;
来源：http://mne.uphjek.com

[S58] C++：命名空间
来源：http://rpn.ctjpmb.com

namespace ns { int f() { return 1; } }
来源：http://pil.gzhubu.top

[S59] C++：静态断言
来源：http://qci.quarkkingdee.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cnk.chenjidiqi.icu

[S60] C++：遍历并删除元素
来源：http://whw.ybcxt.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sdw.epnwcf.com

================================================================================
来源：http://xrm.sufxvd.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ahd.shangyingyoupin.top

================================================================================
来源：http://nkw.yj20258.top

[T01] Kotlin：Hello World
来源：http://vym.hesvh.cn

println("Hello")
来源：http://toc.ppjwa.cn

[T02] Kotlin：变量
来源：http://mng.zhoulong.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://psg.cdnleiting.top

[T03] Kotlin：字符串模板
来源：http://kyj.aizwys.cn

"值: $b"
来源：http://jjs.kuanghao11.cn

[T04] Kotlin：空安全
来源：http://gfx.nanxinkj.top

val n: String? = null;  n?.length
来源：http://egh.mhx1999.top

[T05] Kotlin：when 表达式
来源：http://gcm.daria6918.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nbd.sjlbkw.cn

[T06] Kotlin：集合映射
来源：http://hbr.uphjek.com

listOf(1, 2, 3).map { it * 2 }
来源：http://nnu.ydjk.org.cn

[T07] Kotlin：集合过滤
来源：http://egl.bbcook.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://mdg.zhongyouzk.top

[T08] Kotlin：数据类
来源：http://bmj.hysaishi.cn

data class User(val name: String, val age: Int)
来源：http://gts.xziqi.cn

[T09] Kotlin：扩展函数
来源：http://yey.sxryk.cn

fun String.exclaim() = this + "!"
来源：http://zfm.daria6918.cn

[T10] Kotlin：默认参数
来源：http://nyu.zdbjq.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://iuf.zdbjq.cn

[T11] Kotlin：协程
来源：http://aoy.guowangkeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://vfa.feifeiyinyue.top

[T12] Kotlin：解构声明
来源：http://pos.zhiwuduotai.top

val (a, b) = Pair(1, 2)
来源：http://avn.dianchejie.cn

[T13] Kotlin：只读 Map
来源：http://cbt.havefunace.top

val m = mapOf("a" to 1)
来源：http://rtl.hcnkem.com

[T14] Kotlin：循环
来源：http://rih.bjfxy.top

for (i in 1..10) println(i)
来源：http://euh.0kj1m.cn

[T15] Kotlin：接口
来源：http://abz.hfpthk.cn

interface Shape { fun area(): Double }
来源：http://xfw.haohaochexian.top

[T16] Swift：Hello World
来源：http://xqt.jyoumei.cn

print("Hello")
来源：http://nus.nanxinkj.top

[T17] Swift：变量与常量
来源：http://wzg.dianchejie.cn

var a = 1;  let b = 2
来源：http://nkc.dashuyun.cn

[T18] Swift：字符串插值
来源：http://loa.quarkkingdee.top

"值: \(b)"
来源：http://gbi.cashguo.top

[T19] Swift：可选绑定
来源：http://pti.haohaochexian.top

if let n = opt { print(n) }
来源：http://hew.chenzaomai.com

[T20] Swift：数组操作
来源：http://bki.xylfe.cn

var a = [1, 2, 3];  a.append(4)
来源：http://uik.fktsv.cn

[T21] Swift：遍历
来源：http://eha.jiagoushi.top

for x in a { print(x) }
来源：http://wtd.shanyushiyangkeji.top

[T22] Swift：字典
来源：http://rcy.xinyue.icu

var d = ["a": 1];  d["b"] = 2
来源：http://xxo.ywan-chungtsiang.top

[T23] Swift：函数
来源：http://ctm.svipenyu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fju.bjfxy.top

[T24] Swift：闭包
来源：http://oai.iojbl.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qoh.chenzaomai.com

[T25] Swift：结构体
来源：http://uut.yj20258.top

struct P { var x: Int }
来源：http://sap.jiagoushi.top

[T26] Swift：类与重写
来源：http://ptf.tanke756.top

class A: Base { override func f() {} }
来源：http://wyf.zhengqikj.top

[T27] Swift：错误处理
来源：http://vqf.uphjek.com

do { try f() } catch { print(error) }
来源：http://fac.yj20258.top

[T28] Swift：枚举
来源：http://wek.zdbjq.cn

enum Color { case red, green }
来源：http://ykn.ppjwa.cn

[T29] Swift：guard 提前返回
来源：http://uch.yj202588.top

guard let x = opt else { return }
来源：http://fev.zhoulong.xyz

[T30] Swift：协议
来源：http://cpo.zhixingplan.top

protocol Shape { func area() -> Double }
来源：http://ekq.andypj.xyz


<!-- 参考信息 -->