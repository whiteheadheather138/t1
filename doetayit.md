代发 wailian999

echo "${#s}"
来源：http://wkq.xylfe.cn

[R22] 截取子串
来源：http://gtk.sufxvd.cn

echo "${s:0:5}"
来源：http://ley.kuanghao11.cn

[R23] 字符串替换
来源：http://bwy.zdbjq.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dlj.ybcxt.top

[R24] 大小写转换
来源：http://aoi.pycfn.com

echo "${s^^}"; echo "${s,,}"
来源：http://hfy.hesvh.cn

[R25] 去后缀 / 去前缀
来源：http://ctk.gotoacloud.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://qdq.hywenlv.cn

[R26] 命令替换
来源：http://kul.snrcjt.cn

now=$(date +%F); echo "$now"
来源：http://bvz.xingfuxueyuan.xyz

[R27] 算术展开
来源：http://opi.cheryme.top

echo $((1 + 2 * 3))
来源：http://muh.hongshengwenyu.top

[R28] 浮点运算
来源：http://sac.ctjpmb.com

echo "scale=2; 10/3" | bc
来源：http://hhv.bjfxy.top

[R29] 定义函数
来源：http://ahf.tanke756.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://snr.zhixingplan.top

[R30] 函数返回状态码
来源：http://nus.gotoacloud.top

f() { return 0; }; f || echo "失败了"
来源：http://hyx.yj20258888.top

[R31] 局部变量
来源：http://lty.ydjk.org.cn

f() { local x=1; echo "$x"; }
来源：http://bdi.ctjpmb.com

[R32] 参数个数校验
来源：http://nwr.hcnkem.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qpu.cheryme.top

[R33] 捕获错误并提示行号
来源：http://bav.ydjk.org.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jyp.feifeiyinyue.top

[R34] 退出时清理
来源：http://ecy.yuxming.cn

trap 'rm -f "$tmp"' EXIT
来源：http://jba.uphjek.com

[R35] 后台执行并等待
来源：http://yzt.shuidangran.top

sleep 5 & pid=$!; wait "$pid"
来源：http://jya.shzxlz.cn

[R36] 并发执行多个任务
来源：http://ppj.tanke756.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cga.guowangkeji.top

[R37] 把输出赋给变量
来源：http://tqi.redwolf501.top

files=$(ls -1)
来源：http://kkr.andypj.xyz

[R38] 管道串联
来源：http://qfl.jqgfzy.top

cat a.txt | grep -i error | wc -l
来源：http://gcl.hammf.cn

[R39] 重定向标准输出与错误
来源：http://icr.zhijiandao.cn

cmd > out.log 2>&1
来源：http://hdw.zhongyouzk.top

[R40] 追加写日志
来源：http://nuk.zhijiandao.cn

echo "log" >> out.log
来源：http://wki.chenlongwang.top

[R41] 丢弃输出
来源：http://uoz.dianchejie.cn

cmd >/dev/null 2>&1
来源：http://vmi.guannengcc.top

[R42] 输入重定向
来源：http://lfh.daria6918.cn

wc -l < a.txt
来源：http://vzz.hysaishi.cn

[R43] 按名字查找文件
来源：http://lbe.hywenlv.cn

find . -name "*.log" -type f
来源：http://vfz.0kj1m.cn

[R44] 按修改时间查找
来源：http://wgn.yuanzhike.top

find . -mtime -7 -type f
来源：http://pub.aizwys.cn

[R45] 批量删除
来源：http://wby.xinyue.icu

find . -name "*.tmp" -delete
来源：http://zxb.zhengqikj.top

[R46] 递归替换文件内容
来源：http://ovy.redwolf501.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zxb.yangfankeji.com

[R47] sed 单行替换
来源：http://zdk.jinqigufen.top

sed -i 's/foo/bar/g' a.txt
来源：http://lkx.zdqjudy.top

[R48] awk 取指定列
来源：http://dcg.zdqjudy.top

awk '{print $1, $3}' a.txt
来源：http://ptk.nanxuanxn.top

[R49] awk 带条件
来源：http://shx.quarkkingdee.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rwk.tarul.cn

[R50] awk 求和
来源：http://oxp.svipenyu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wxa.jqgfzy.top

[R51] 排序去重取前几
来源：http://zld.c1oappe.top

sort a.txt | uniq -c | sort -rn | head
来源：http://iph.xuanzx.com

[R52] 统计行数
来源：http://bhd.sweek.top

wc -l a.txt
来源：http://iew.shzxlz.cn

[R53] 查看文件头与实时尾
来源：http://hin.jinqigfzy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mig.gzhubu.top

[R54] 比较两个文件
来源：http://cek.zhaomingkeji.xyz

diff a.txt b.txt
来源：http://lhb.sxryk.cn

[R55] 压缩与解压
来源：http://tpr.hammf.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uhm.hysaishi.cn

[R56] 远程拷贝
来源：http://fos.cashguo.top

scp file user@host:/path/
来源：http://nlq.zhongyouzk.top

[R57] 远程执行命令
来源：http://hza.zhoulong.xyz

ssh user@host 'uptime'
来源：http://wpm.shzxlz.cn

[R58] 下载文件
来源：http://hqc.quarkkingdee.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yvu.316326.xyz

[R59] 发 POST JSON
来源：http://lfr.wangshuangyany.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kxs.zycfv.cn

[R60] 只看 HTTP 状态码
来源：http://ail.ydzc1.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qaj.yangfankeji.com

[R61] 磁盘占用
来源：http://cjp.ivvv.top

df -h;  du -sh *
来源：http://ooa.shuidangran.top

[R62] 找最占空间的文件
来源：http://aug.zhiwuduotai.top

du -ah . | sort -rh | head -10
来源：http://wqn.redwolf501.top

[R63] 内存与进程
来源：http://gkz.jlsjyb.cn

free -h;  ps aux | grep nginx
来源：http://dqi.zycfv.cn

[R64] 结束进程
来源：http://zlx.yonumen.top

kill -9 $(pgrep -f app.py)
来源：http://hou.hywenlv.cn

[R65] 查看端口占用
来源：http://zgh.jqgfzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://oli.chenlongwang.top

[R66] 定时任务
来源：http://hji.iojbl.cn

crontab -e;  crontab -l
来源：http://gos.chenjidiqi.icu

[R67] 生成随机十六进制串
来源：http://xqr.redwolf501.top

openssl rand -hex 16
来源：http://jhy.cashguo.top

[R68] 计算文件校验值
来源：http://dwp.svipenyu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://wrs.dianchejie.cn

[R69] 生成随机密码
来源：http://pfg.vehdjk.com

head -c 16 /dev/urandom | base64
来源：http://rag.cashguo.top

[R70] 时间戳与互转
来源：http://cos.xuanzx.com

date +%s;  date -d @1700000000
来源：http://ohx.sufxvd.cn

[R71] 日期格式化
来源：http://ndt.xuetiantiany.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://czk.yj20258888.top

[R72] 等待端口就绪
来源：http://jng.jinqigufen.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ayl.jinyuanbaomall.cn

[R73] 分割大日志
来源：http://swb.dashuyun.cn

split -l 1000 big.log part_
来源：http://xpi.nanxuanxn.top

[R74] 批量重命名
来源：http://svf.xinyue.icu

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ask.fzhhl.top

[R75] 导出环境变量
来源：http://xyy.zhoulong.xyz

export PATH="$HOME/bin:$PATH"
来源：http://dyr.zhixingplan.top

[R76] 使用临时文件
来源：http://dot.ybcxt.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gwt.cashguo.top

[R77] 读取用户输入
来源：http://bkr.ydjk.org.cn

read -rp "请输入: " ans
来源：http://fci.kuanghao11.cn

[R78] 交互式菜单
来源：http://oql.redwolf501.top

select opt in a b c; do echo "$opt"; break; done
来源：http://wsh.uphjek.com

[R79] 解析命令行选项
来源：http://aft.ppjwa.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cvp.vehdjk.com

[R80] 查看脚本执行耗时
来源：http://ryr.ywan-chungtsiang.top

time ./run.sh
来源：http://jnc.zdbjq.cn

================================================================================
来源：http://pfh.yfazqb.com

S. C / C++ 专题
来源：http://uhs.zhiwuduotai.top

================================================================================
来源：http://jrj.haohaochexian.top

[S01] C：Hello World
来源：http://mna.jinqigufen.top

#include <stdio.h>
来源：http://eya.zhaomingkeji.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://nlu.jqgfzy.top

[S02] C：变量与格式化输出
来源：http://ful.xuetiantiany.cn

int a = 10; printf("%d\n", a);
来源：http://eiw.yanxiufei.cn

[S03] C：读入整数
来源：http://mno.havefunace.top

int x; scanf("%d", &x);
来源：http://oqo.yongpay.top

[S04] C：字符串复制
来源：http://qlj.zhiwuduotai.top

char dst[32]; strcpy(dst, "hi");
来源：http://dnj.yanxiufei.cn

[S05] C：字符串长度
来源：http://rru.zhijiandao.cn

strlen(s)
来源：http://cwz.zycfv.cn

[S06] C：字符串比较
来源：http://fni.xingfuxueyuan.xyz

strcmp(a, b) == 0
来源：http://fwm.tianlin.xyz

[S07] C：数组遍历求和
来源：http://gvo.daxiang520.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://eve.cucudq.cn

[S08] C：动态内存分配与释放
来源：http://acn.sxryk.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hep.zhaomingkeji.xyz

[S09] C：结构体定义与初始化
来源：http://dha.9152youxi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kne.haohaochexian.top

[S10] C：指针与解引用
来源：http://ghe.vehdjk.com

int *p = &a;  *p = 5;
来源：http://vcs.snrcjt.cn

[S11] C：逐行读文件
来源：http://vwa.mhx1999.top

FILE *f = fopen("a.txt", "r");
来源：http://ftq.316326.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://pou.fktsv.cn

fclose(f);
来源：http://qup.yvedp.cn

[S12] C：写文件
来源：http://bqk.haohaochexian.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jtj.52xcode.cn

[S13] C：宏定义
来源：http://uzc.c1oappe.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://juo.zhaomingkeji.xyz

[S14] C：枚举
来源：http://pye.316326.xyz

enum Color { RED, GREEN, BLUE };
来源：http://vos.zhaomingkeji.xyz

[S15] C：类型转换
来源：http://dpb.jinyuanbaomall.cn

(double) a / b
来源：http://kmz.316326.xyz

[S16] C：位操作置位
来源：http://wlt.cheryme.top

x |= (1 << 3);
来源：http://vcn.ppjwa.cn

[S17] C：安全拼接字符串
来源：http://fjy.hcnkem.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bhz.ctjpmb.com

[S18] C：命令行参数
来源：http://lxx.andypj.xyz

int main(int argc, char **argv)
来源：http://len.wangshuangyany.cn

[S19] C：快速排序
来源：http://iyl.xylfe.cn

qsort(a, n, sizeof(int), cmp);
来源：http://phq.zhengqikj.top

[S20] C：二分查找
来源：http://wzs.0kj1m.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dtn.fanxiaobao.xyz

[S21] C：字符类别判断
来源：http://mgc.ppjwa.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lfo.uphjek.com

[S22] C：字符串转数字
来源：http://fgl.gogol.net.cn

atoi("42");  strtod("3.14", NULL);
来源：http://lhv.gotoacloud.top

[S23] C：随机数
来源：http://fmo.zhaomingkeji.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://fif.c1oappe.top

[S24] C：获取本地时间
来源：http://xkw.yueranfly.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tiz.smart0.xyz

[S25] C：内存拷贝
来源：http://rhy.xinyue.icu

memcpy(dst, src, n);
来源：http://xii.sufxvd.cn

[S26] C：内存清零
来源：http://bda.zdbjq.cn

memset(a, 0, sizeof a);
来源：http://tfy.shanyushiyangkeji.top

[S27] C：定义常量
来源：http://kkn.ppjwa.cn

const double PI = 3.14159;
来源：http://pmd.daria6918.cn

[S28] C：静态变量
来源：http://nnp.quarkkingdee.top

static int counter = 0;
来源：http://szq.shangyingyoupin.top

[S29] C：变参函数
来源：http://siy.cqqwz.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rzb.xuanzx.com

[S30] C：头文件保护
来源：http://kxa.svipenyu.cn

#ifndef X_H
来源：http://iun.tian-w.cn

#define X_H
来源：http://owm.cucudq.cn

#endif
来源：http://zao.shuidangran.top

[S31] C++：Hello World
来源：http://jlq.cqqwz.cn

#include <iostream>
来源：http://bwt.sweek.top

int main() { std::cout << "Hello\n"; }
来源：http://veg.zhijiandao.cn

[S32] C++：字符串
来源：http://sqs.yj202588.top

std::string s = "hi";  s += "!";
来源：http://okb.yuxming.cn

[S33] C++：vector 增删
来源：http://nco.yj20258.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ibz.yj202588.top

[S34] C++：遍历 vector
来源：http://lfj.yanxiufei.cn

for (auto &x : v) { std::cout << x; }
来源：http://lsn.jinghuilouyu.cn

[S35] C++：map
来源：http://cad.tian-w.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://htw.gotoacloud.top

[S36] C++：unordered_map
来源：http://pud.svipenyu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uyz.fehbvm.com

[S37] C++：set
来源：http://anc.cashguo.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rgs.xuanzx.com

[S38] C++：排序
来源：http://gdj.yanxiufei.cn

std::sort(v.begin(), v.end());
来源：http://cwv.ywan-chungtsiang.top

[S39] C++：自定义比较器排序
来源：http://aat.jinghuilouyu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://att.shuidangran.top

[S40] C++：查找元素
来源：http://rbk.tian-w.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://stx.epnwcf.com

[S41] C++：类与构造函数
来源：http://bnx.52xcode.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vuv.c1oappe.top

[S42] C++：继承与虚函数
来源：http://xph.redwolf501.top

class B : public Base { public: void f() override {} };
来源：http://nuo.xuanzx.com

[S43] C++：智能指针
来源：http://ifp.9152youxi.cn

auto p = std::make_unique<int>(5);
来源：http://jxn.ybcxt.top

[S44] C++：引用传参
来源：http://rkb.fzhhl.top

void inc(int &x) { ++x; }
来源：http://lpn.shzxlz.cn

[S45] C++：lambda
来源：http://oqw.sweek.top

auto add = [](int a, int b) { return a + b; };
来源：http://elb.chenlongwang.top

[S46] C++：函数模板
来源：http://vul.ydzc1.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vql.hnxiangtu.top

[S47] C++：结构化绑定遍历
来源：http://wnw.tian-w.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rkx.cucudq.cn

[S48] C++：逐行读文件
来源：http://pqw.havefunace.top

std::ifstream in("a.txt");  std::string line;
来源：http://irh.vqdsnc.cn

while (std::getline(in, line)) { }
来源：http://hur.zhiwuduotai.top

[S49] C++：写文件
来源：http://xbc.daria6918.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vun.zhongyouzk.top

[S50] C++：格式化数字
来源：http://lio.cqqwz.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bzq.shuidangran.top

[S51] C++：显式类型转换
来源：http://siy.daxiang520.top

static_cast<double>(a) / b
来源：http://qzr.chenjidiqi.icu

[S52] C++：const 与 noexcept
来源：http://luo.hywenlv.cn

int size() const noexcept { return n_; }
来源：http://wog.quarkkingdee.top

[S53] C++：移动语义
来源：http://pvt.gogol.net.cn

std::vector<int> w = std::move(v);
来源：http://koa.zhoulong.xyz

[S54] C++：异常处理
来源：http://tmm.pycfn.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lbo.yvedp.cn

[S55] C++：结构化绑定
来源：http://iky.snrcjt.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://omp.zhijiandao.cn

[S56] C++：optional
来源：http://mqd.c1oappe.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jbr.birdmap.top

[S57] C++：编译期常量
来源：http://dtu.shuidangran.top

constexpr int N = 10;
来源：http://ldv.nanxuanxn.top

[S58] C++：命名空间
来源：http://clv.tanke756.top

namespace ns { int f() { return 1; } }
来源：http://ant.xuetiantiany.cn

[S59] C++：静态断言
来源：http://evd.316326.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kxt.yongpay.top

[S60] C++：遍历并删除元素
来源：http://nss.jqgfzy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hjs.jqgfzy.top

================================================================================
来源：http://mhn.zdbjq.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cql.kuanghao11.cn

================================================================================
来源：http://wgj.yuanzhike.top

[T01] Kotlin：Hello World
来源：http://uvv.epnwcf.com

println("Hello")
来源：http://arz.quarkkingdee.top

[T02] Kotlin：变量
来源：http://ose.fehbvm.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lqh.nanxinkj.top

[T03] Kotlin：字符串模板
来源：http://izk.gotoacloud.top

"值: $b"
来源：http://mco.kuanghao11.cn

[T04] Kotlin：空安全
来源：http://vtj.tarul.cn

val n: String? = null;  n?.length
来源：http://etg.chenjidiqi.icu

[T05] Kotlin：when 表达式
来源：http://tud.gaohongyu789.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://frk.jyoumei.cn

[T06] Kotlin：集合映射
来源：http://jpr.ppjwa.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hig.fanxiaobao.xyz

[T07] Kotlin：集合过滤
来源：http://vbk.pycfn.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://wbf.cashguo.top

[T08] Kotlin：数据类
来源：http://zhw.svipenyu.cn

data class User(val name: String, val age: Int)
来源：http://oqt.jlsjyb.cn

[T09] Kotlin：扩展函数
来源：http://ttg.kuanghao11.cn

fun String.exclaim() = this + "!"
来源：http://ejb.sufxvd.cn

[T10] Kotlin：默认参数
来源：http://zzo.jqgfzy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://oli.xinyue.icu

[T11] Kotlin：协程
来源：http://cxq.shuidangran.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://rwo.hysaishi.cn

[T12] Kotlin：解构声明
来源：http://nxx.guannengcc.top

val (a, b) = Pair(1, 2)
来源：http://xwx.xuetiantiany.cn

[T13] Kotlin：只读 Map
来源：http://ipi.0kj1m.cn

val m = mapOf("a" to 1)
来源：http://tmw.jinyuanbaomall.cn

[T14] Kotlin：循环
来源：http://xqe.chenlongwang.top

for (i in 1..10) println(i)
来源：http://msc.cdnleiting.top

[T15] Kotlin：接口
来源：http://ztu.zhengqikj.top

interface Shape { fun area(): Double }
来源：http://wty.xinyue.icu

[T16] Swift：Hello World
来源：http://mok.xziqi.cn

print("Hello")
来源：http://kqi.dashuyun.cn

[T17] Swift：变量与常量
来源：http://yrw.snrcjt.cn

var a = 1;  let b = 2
来源：http://nxn.chenzaomai.com

[T18] Swift：字符串插值
来源：http://gev.zhoulong.xyz

"值: \(b)"
来源：http://epz.pengpengdd.cyou

[T19] Swift：可选绑定
来源：http://ilp.tarul.cn

if let n = opt { print(n) }
来源：http://vyb.jinqigfzy.top

[T20] Swift：数组操作
来源：http://mtg.nanxinkj.top

var a = [1, 2, 3];  a.append(4)
来源：http://ixu.ivvv.top

[T21] Swift：遍历
来源：http://imk.dianchejie.cn

for x in a { print(x) }
来源：http://jyp.hammf.cn

[T22] Swift：字典
来源：http://hww.hnxiangtu.top

var d = ["a": 1];  d["b"] = 2
来源：http://yge.jqgufenzy.top

[T23] Swift：函数
来源：http://tvh.fehbvm.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bkx.xingfuxueyuan.xyz

[T24] Swift：闭包
来源：http://fno.fehbvm.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://jum.52xcode.cn


<!-- 参考信息 -->