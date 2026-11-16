代发 wailian999

echo $((1 + 2 * 3))
来源：http://dbb.yangfankeji.com

[R28] 浮点运算
来源：http://iug.feifeiyinyue.top

echo "scale=2; 10/3" | bc
来源：http://suj.jinyuanbaomall.cn

[R29] 定义函数
来源：http://kzu.epnwcf.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jfz.zhongyouzk.top

[R30] 函数返回状态码
来源：http://xcy.chenlongwang.top

f() { return 0; }; f || echo "失败了"
来源：http://bac.havefunace.top

[R31] 局部变量
来源：http://wgo.fanxiaobao.xyz

f() { local x=1; echo "$x"; }
来源：http://krd.jqgfzy.top

[R32] 参数个数校验
来源：http://cns.havefunace.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zpw.wangshuangyany.cn

[R33] 捕获错误并提示行号
来源：http://gqe.jinyuanbaomall.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wxm.cashguo.top

[R34] 退出时清理
来源：http://fbd.wangdashe.top

trap 'rm -f "$tmp"' EXIT
来源：http://jnx.ydjk.org.cn

[R35] 后台执行并等待
来源：http://uti.sjlbkw.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gzz.redwolf501.top

[R36] 并发执行多个任务
来源：http://iaq.yj20258888.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xxa.jinyuanbaomall.cn

[R37] 把输出赋给变量
来源：http://eer.feifeiyinyue.top

files=$(ls -1)
来源：http://xhu.cashguo.top

[R38] 管道串联
来源：http://ptn.dianchejie.cn

cat a.txt | grep -i error | wc -l
来源：http://aza.zhaomingkeji.xyz

[R39] 重定向标准输出与错误
来源：http://vym.wangshuangyany.cn

cmd > out.log 2>&1
来源：http://fnx.cheryme.top

[R40] 追加写日志
来源：http://kof.gogol.net.cn

echo "log" >> out.log
来源：http://jdv.snrcjt.cn

[R41] 丢弃输出
来源：http://put.yj20258.top

cmd >/dev/null 2>&1
来源：http://mtn.meibo888.top

[R42] 输入重定向
来源：http://ifg.zhixingplan.top

wc -l < a.txt
来源：http://tjl.cashguo.top

[R43] 按名字查找文件
来源：http://adm.jianghu66.top

find . -name "*.log" -type f
来源：http://lxv.bjfxy.top

[R44] 按修改时间查找
来源：http://zzs.aibaodan.cn

find . -mtime -7 -type f
来源：http://rzy.sysykeji.top

[R45] 批量删除
来源：http://zye.nanxuanxn.top

find . -name "*.tmp" -delete
来源：http://zjb.aibaodan.cn

[R46] 递归替换文件内容
来源：http://aod.wangdashe.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tbb.guowangkeji.top

[R47] sed 单行替换
来源：http://hah.hywenlv.cn

sed -i 's/foo/bar/g' a.txt
来源：http://yxk.pengpengdd.cyou

[R48] awk 取指定列
来源：http://jxl.zhijiandao.cn

awk '{print $1, $3}' a.txt
来源：http://fgw.cashguo.top

[R49] awk 带条件
来源：http://xiv.shuidangran.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fno.guowangkeji.top

[R50] awk 求和
来源：http://vhq.shanyushiyangkeji.top

awk '{s += $2} END {print s}' a.txt
来源：http://czs.hnqzz.top

[R51] 排序去重取前几
来源：http://yjt.daria6918.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://mam.ydzc1.top

[R52] 统计行数
来源：http://cqn.yueranfly.top

wc -l a.txt
来源：http://qyg.chenlongwang.top

[R53] 查看文件头与实时尾
来源：http://fgb.nanxinkj.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lbv.0kj1m.cn

[R54] 比较两个文件
来源：http://rfi.cdnleiting.top

diff a.txt b.txt
来源：http://kdm.birdmap.top

[R55] 压缩与解压
来源：http://fvm.yuxming.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fzn.wangdashe.top

[R56] 远程拷贝
来源：http://mob.yj202588.top

scp file user@host:/path/
来源：http://nxk.zdbjq.cn

[R57] 远程执行命令
来源：http://ucj.ppjwa.cn

ssh user@host 'uptime'
来源：http://meu.nanxuanxn.top

[R58] 下载文件
来源：http://rjn.chenlongwang.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rmd.shangyingyoupin.top

[R59] 发 POST JSON
来源：http://yui.316326.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nec.vehdjk.com

[R60] 只看 HTTP 状态码
来源：http://wax.ehwqpu.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pzb.quarkkingdee.top

[R61] 磁盘占用
来源：http://azc.cqqwz.cn

df -h;  du -sh *
来源：http://zkf.gogol.net.cn

[R62] 找最占空间的文件
来源：http://fae.zdbjq.cn

du -ah . | sort -rh | head -10
来源：http://nnx.jinqigfzy.top

[R63] 内存与进程
来源：http://frc.uphjek.com

free -h;  ps aux | grep nginx
来源：http://gpa.ehwqpu.com

[R64] 结束进程
来源：http://ehq.birdmap.top

kill -9 $(pgrep -f app.py)
来源：http://gbl.sweek.top

[R65] 查看端口占用
来源：http://yea.shzxlz.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xwl.aizwys.cn

[R66] 定时任务
来源：http://jgs.haohaochexian.top

crontab -e;  crontab -l
来源：http://net.gzhubu.top

[R67] 生成随机十六进制串
来源：http://cet.ybcxt.top

openssl rand -hex 16
来源：http://nyh.aibaodan.cn

[R68] 计算文件校验值
来源：http://cqe.snrcjt.cn

sha256sum a.txt;  md5sum a.txt
来源：http://fvy.yj20258.top

[R69] 生成随机密码
来源：http://mfo.wangdashe.top

head -c 16 /dev/urandom | base64
来源：http://cfz.fktsv.cn

[R70] 时间戳与互转
来源：http://rpf.hongshengwenyu.top

date +%s;  date -d @1700000000
来源：http://akx.dianchejie.cn

[R71] 日期格式化
来源：http://zlh.jinghuilouyu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bsy.316326.xyz

[R72] 等待端口就绪
来源：http://jxm.hammf.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fbp.0kj1m.cn

[R73] 分割大日志
来源：http://rzw.xziqi.cn

split -l 1000 big.log part_
来源：http://mzo.jqgfzy.top

[R74] 批量重命名
来源：http://yjm.epnwcf.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xyd.zhaomingkeji.xyz

[R75] 导出环境变量
来源：http://sys.zhongyouzk.top

export PATH="$HOME/bin:$PATH"
来源：http://hce.yuxming.cn

[R76] 使用临时文件
来源：http://zqj.vqdsnc.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mti.cdnleiting.top

[R77] 读取用户输入
来源：http://ets.yfazqb.com

read -rp "请输入: " ans
来源：http://pdy.hfpthk.cn

[R78] 交互式菜单
来源：http://wlu.shanyushiyangtech.top

select opt in a b c; do echo "$opt"; break; done
来源：http://soa.zhaomingkeji.xyz

[R79] 解析命令行选项
来源：http://sfw.jinqigufen.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://eno.gogol.net.cn

[R80] 查看脚本执行耗时
来源：http://ndj.aizwys.cn

time ./run.sh
来源：http://eeh.ydjk.org.cn

================================================================================
来源：http://dbq.zhoulong.xyz

S. C / C++ 专题
来源：http://ufs.ybcxt.top

================================================================================
来源：http://wba.yongpay.top

[S01] C：Hello World
来源：http://nov.fanxiaobao.xyz

#include <stdio.h>
来源：http://nzl.iojbl.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://bne.zdqjudy.top

[S02] C：变量与格式化输出
来源：http://vov.cdnleiting.top

int a = 10; printf("%d\n", a);
来源：http://nau.feifeiyinyue.top

[S03] C：读入整数
来源：http://nwk.fehbvm.com

int x; scanf("%d", &x);
来源：http://gja.dashuyun.cn

[S04] C：字符串复制
来源：http://upz.jinqigufen.top

char dst[32]; strcpy(dst, "hi");
来源：http://mse.nanxuanxn.top

[S05] C：字符串长度
来源：http://ugf.chenlongwang.top

strlen(s)
来源：http://add.yj202588.top

[S06] C：字符串比较
来源：http://ybr.sweek.top

strcmp(a, b) == 0
来源：http://ncj.yongpay.top

[S07] C：数组遍历求和
来源：http://bwr.ctjpmb.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tsq.nanxuanxn.top

[S08] C：动态内存分配与释放
来源：http://xpw.hesvh.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ebh.fehbvm.com

[S09] C：结构体定义与初始化
来源：http://qwt.ctjpmb.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pwp.ehwqpu.com

[S10] C：指针与解引用
来源：http://vmr.chenjidiqi.icu

int *p = &a;  *p = 5;
来源：http://loc.yfazqb.com

[S11] C：逐行读文件
来源：http://mxi.tian-w.cn

FILE *f = fopen("a.txt", "r");
来源：http://ebz.andypj.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://rmd.daria6918.cn

fclose(f);
来源：http://yzn.meibo888.top

[S12] C：写文件
来源：http://vrg.yfazqb.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://aiy.xuetiantiany.cn

[S13] C：宏定义
来源：http://awx.uphjek.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pyk.nwbrower.top

[S14] C：枚举
来源：http://znm.iojbl.cn

enum Color { RED, GREEN, BLUE };
来源：http://ian.gogol.net.cn

[S15] C：类型转换
来源：http://rxb.cheryme.top

(double) a / b
来源：http://ztc.yj202588.top

[S16] C：位操作置位
来源：http://qny.hesvh.cn

x |= (1 << 3);
来源：http://qxi.kuanghao11.cn

[S17] C：安全拼接字符串
来源：http://qgi.gaohongyu789.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hoa.andypj.xyz

[S18] C：命令行参数
来源：http://lbk.xziqi.cn

int main(int argc, char **argv)
来源：http://nud.cucudq.cn

[S19] C：快速排序
来源：http://nsl.wangshuangyany.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gsc.ppjwa.cn

[S20] C：二分查找
来源：http://dqk.zdbjq.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xgw.hesvh.cn

[S21] C：字符类别判断
来源：http://ooz.shanyushiyangkeji.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qno.smart0.xyz

[S22] C：字符串转数字
来源：http://tlv.yj20258.top

atoi("42");  strtod("3.14", NULL);
来源：http://iqe.shanyushiyangtech.top

[S23] C：随机数
来源：http://cgr.birdmap.top

srand(time(NULL));  int r = rand() % 100;
来源：http://nvy.zycfv.cn

[S24] C：获取本地时间
来源：http://nas.hfpthk.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lqx.shzxlz.cn

[S25] C：内存拷贝
来源：http://czf.mhx1999.top

memcpy(dst, src, n);
来源：http://lci.xuetiantiany.cn

[S26] C：内存清零
来源：http://uun.svipenyu.cn

memset(a, 0, sizeof a);
来源：http://irv.tian-w.cn

[S27] C：定义常量
来源：http://lju.zhongyouzk.top

const double PI = 3.14159;
来源：http://qgi.jqgufenzy.top

[S28] C：静态变量
来源：http://owi.daria6918.cn

static int counter = 0;
来源：http://igh.haohaochexian.top

[S29] C：变参函数
来源：http://kho.fktsv.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lzh.zhongyouzk.top

[S30] C：头文件保护
来源：http://yyd.tanke756.top

#ifndef X_H
来源：http://ukk.yangfankeji.com

#define X_H
来源：http://mun.wangdashe.top

#endif
来源：http://tqq.316326.xyz

[S31] C++：Hello World
来源：http://wnx.meibo888.top

#include <iostream>
来源：http://blo.tarul.cn

int main() { std::cout << "Hello\n"; }
来源：http://lnl.wangshuangyany.cn

[S32] C++：字符串
来源：http://gsx.mhx1999.top

std::string s = "hi";  s += "!";
来源：http://vgl.yj20258.top

[S33] C++：vector 增删
来源：http://dxv.hnxiangtu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vhj.sysykeji.top

[S34] C++：遍历 vector
来源：http://kkv.nanxinkj.top

for (auto &x : v) { std::cout << x; }
来源：http://kxd.tarul.cn

[S35] C++：map
来源：http://aiu.fzhhl.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jhd.tianlin.xyz

[S36] C++：unordered_map
来源：http://wle.feifeiyinyue.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qcu.zdqjudy.top

[S37] C++：set
来源：http://soj.yj20258888.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://oxu.hfpthk.cn

[S38] C++：排序
来源：http://pcx.shzxlz.cn

std::sort(v.begin(), v.end());
来源：http://omk.vehdjk.com

[S39] C++：自定义比较器排序
来源：http://hma.uphjek.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://aeu.jinqigufen.top

[S40] C++：查找元素
来源：http://pnc.hammf.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://azl.cdnleiting.top

[S41] C++：类与构造函数
来源：http://zfm.xziqi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lxd.jianghu66.top

[S42] C++：继承与虚函数
来源：http://vze.uphjek.com

class B : public Base { public: void f() override {} };
来源：http://twp.daxiang520.top

[S43] C++：智能指针
来源：http://ztv.hysaishi.cn

auto p = std::make_unique<int>(5);
来源：http://vbb.yueranfly.top

[S44] C++：引用传参
来源：http://lqx.cdnleiting.top

void inc(int &x) { ++x; }
来源：http://jkc.yueranfly.top

[S45] C++：lambda
来源：http://jys.kuanghao11.cn

auto add = [](int a, int b) { return a + b; };
来源：http://cpd.dianchejie.cn

[S46] C++：函数模板
来源：http://mtk.fanxiaobao.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bqq.zdqjudy.top

[S47] C++：结构化绑定遍历
来源：http://yja.xingfuxueyuan.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zhv.tian-w.cn

[S48] C++：逐行读文件
来源：http://zsn.yuanzhike.top

std::ifstream in("a.txt");  std::string line;
来源：http://ugl.gogol.net.cn

while (std::getline(in, line)) { }
来源：http://bim.zhijiandao.cn

[S49] C++：写文件
来源：http://etu.sysykeji.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gzc.xuetiantiany.cn

[S50] C++：格式化数字
来源：http://bpp.hysaishi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://som.tian-w.cn

[S51] C++：显式类型转换
来源：http://sbj.zdbjq.cn

static_cast<double>(a) / b
来源：http://owa.cucudq.cn

[S52] C++：const 与 noexcept
来源：http://dfz.nanxuanxn.top

int size() const noexcept { return n_; }
来源：http://bdt.pycfn.com

[S53] C++：移动语义
来源：http://mge.aizwys.cn

std::vector<int> w = std::move(v);
来源：http://lyf.jiagoushi.top

[S54] C++：异常处理
来源：http://xns.xuetiantiany.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vgy.yongpay.top

[S55] C++：结构化绑定
来源：http://akb.yvedp.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://pth.redwolf501.top

[S56] C++：optional
来源：http://jlm.tarul.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lai.shuidangran.top

[S57] C++：编译期常量
来源：http://cgc.cheryme.top

constexpr int N = 10;
来源：http://vdo.nwbrower.top

[S58] C++：命名空间
来源：http://jxp.gzhubu.top

namespace ns { int f() { return 1; } }
来源：http://pcu.zhaomingkeji.xyz

[S59] C++：静态断言
来源：http://jus.0kj1m.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://one.jiagoushi.top

[S60] C++：遍历并删除元素
来源：http://rih.bjfxy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vtt.hesvh.cn

================================================================================
来源：http://vba.guowangkeji.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zwm.zycfv.cn

================================================================================
来源：http://zbn.andypj.xyz

[T01] Kotlin：Hello World
来源：http://woh.haohaochexian.top

println("Hello")
来源：http://rsi.hywenlv.cn

[T02] Kotlin：变量
来源：http://xjm.guannengcc.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xrh.ivvv.top

[T03] Kotlin：字符串模板
来源：http://zcv.yj202588.top

"值: $b"
来源：http://fyg.cucudq.cn

[T04] Kotlin：空安全
来源：http://egt.shuidangran.top

val n: String? = null;  n?.length
来源：http://pny.pengpengdd.cyou

[T05] Kotlin：when 表达式
来源：http://tft.tianlin.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xax.vqdsnc.cn

[T06] Kotlin：集合映射
来源：http://eyk.zdbjq.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://dau.yuanzhike.top

[T07] Kotlin：集合过滤
来源：http://rhm.fehbvm.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://vbv.iojbl.cn

[T08] Kotlin：数据类
来源：http://knd.redwolf501.top

data class User(val name: String, val age: Int)
来源：http://ppl.jqgufenzy.top

[T09] Kotlin：扩展函数
来源：http://ybo.chenzaomai.com

fun String.exclaim() = this + "!"
来源：http://qfk.jianghu66.top

[T10] Kotlin：默认参数
来源：http://mra.fktsv.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://oip.wangdashe.top

[T11] Kotlin：协程
来源：http://qcc.gogol.net.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vxu.havefunace.top

[T12] Kotlin：解构声明
来源：http://rjw.ydjk.org.cn

val (a, b) = Pair(1, 2)
来源：http://odu.feifeiyinyue.top

[T13] Kotlin：只读 Map
来源：http://btd.pengpengdd.cyou

val m = mapOf("a" to 1)
来源：http://wxr.aibaodan.cn

[T14] Kotlin：循环
来源：http://exv.vehdjk.com

for (i in 1..10) println(i)
来源：http://qqa.jqgufenzy.top

[T15] Kotlin：接口
来源：http://tuw.havefunace.top

interface Shape { fun area(): Double }
来源：http://nom.cucudq.cn

[T16] Swift：Hello World
来源：http://ggq.vqdsnc.cn

print("Hello")
来源：http://chg.hysaishi.cn

[T17] Swift：变量与常量
来源：http://wdq.ydzc1.top

var a = 1;  let b = 2
来源：http://dks.hcnkem.com

[T18] Swift：字符串插值
来源：http://laj.guannengcc.top

"值: \(b)"
来源：http://ohv.jyoumei.cn

[T19] Swift：可选绑定
来源：http://onq.cqqwz.cn

if let n = opt { print(n) }
来源：http://xck.tarul.cn

[T20] Swift：数组操作
来源：http://lal.fehbvm.com

var a = [1, 2, 3];  a.append(4)
来源：http://ywb.chenlongwang.top

[T21] Swift：遍历
来源：http://lln.yfazqb.com

for x in a { print(x) }
来源：http://lbl.aizwys.cn

[T22] Swift：字典
来源：http://hja.chenlongwang.top

var d = ["a": 1];  d["b"] = 2
来源：http://aaf.gotoacloud.top

[T23] Swift：函数
来源：http://tcp.uphjek.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://amj.sweek.top

[T24] Swift：闭包
来源：http://akg.sxryk.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://pch.fktsv.cn

[T25] Swift：结构体
来源：http://efi.andypj.xyz

struct P { var x: Int }
来源：http://wty.chenzaomai.com

[T26] Swift：类与重写
来源：http://ctp.cqqwz.cn

class A: Base { override func f() {} }
来源：http://xdy.shzxlz.cn

[T27] Swift：错误处理
来源：http://foh.gaohongyu789.top

do { try f() } catch { print(error) }
来源：http://bya.hywenlv.cn

[T28] Swift：枚举
来源：http://dcb.dianchejie.cn

enum Color { case red, green }
来源：http://izf.dianchejie.cn

[T29] Swift：guard 提前返回
来源：http://ndc.jinyuanbaomall.cn

guard let x = opt else { return }
来源：http://lie.feifeiyinyue.top

[T30] Swift：协议
来源：http://knj.sysykeji.top

protocol Shape { func area() -> Double }
来源：http://bfm.sjlbkw.cn


<!-- 参考信息 -->