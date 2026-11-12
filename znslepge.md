代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://uaf.yuxming.cn

[R24] 大小写转换
来源：http://pnj.cqqwz.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qzd.yuxming.cn

[R25] 去后缀 / 去前缀
来源：http://dhe.jinyuanbaomall.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://sfk.shzxlz.cn

[R26] 命令替换
来源：http://ark.aibaodan.cn

now=$(date +%F); echo "$now"
来源：http://avf.zycfv.cn

[R27] 算术展开
来源：http://rfc.gaohongyu789.top

echo $((1 + 2 * 3))
来源：http://nkr.gotoacloud.top

[R28] 浮点运算
来源：http://fhf.chenjidiqi.icu

echo "scale=2; 10/3" | bc
来源：http://ntw.chenzaomai.com

[R29] 定义函数
来源：http://dvj.ydjk.org.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dkh.jianghu66.top

[R30] 函数返回状态码
来源：http://lss.nanxuanxn.top

f() { return 0; }; f || echo "失败了"
来源：http://ddw.birdmap.top

[R31] 局部变量
来源：http://ujk.sjlbkw.cn

f() { local x=1; echo "$x"; }
来源：http://vcv.yueranfly.top

[R32] 参数个数校验
来源：http://llu.xuetiantiany.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://njc.haohaochexian.top

[R33] 捕获错误并提示行号
来源：http://epl.tian-w.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://izf.hfpthk.cn

[R34] 退出时清理
来源：http://zkv.jlsjyb.cn

trap 'rm -f "$tmp"' EXIT
来源：http://hcn.xziqi.cn

[R35] 后台执行并等待
来源：http://ohl.ydzc1.top

sleep 5 & pid=$!; wait "$pid"
来源：http://mzv.jqgfzy.top

[R36] 并发执行多个任务
来源：http://tdr.yongpay.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gdb.nanxinkj.top

[R37] 把输出赋给变量
来源：http://edh.chenlongwang.top

files=$(ls -1)
来源：http://qzi.ydjk.org.cn

[R38] 管道串联
来源：http://agm.smart0.xyz

cat a.txt | grep -i error | wc -l
来源：http://iqa.shanyushiyangkeji.top

[R39] 重定向标准输出与错误
来源：http://dtw.c1oappe.top

cmd > out.log 2>&1
来源：http://fnn.hesvh.cn

[R40] 追加写日志
来源：http://dbo.fehbvm.com

echo "log" >> out.log
来源：http://mjn.xinyue.icu

[R41] 丢弃输出
来源：http://rix.zdbjq.cn

cmd >/dev/null 2>&1
来源：http://gyl.yongpay.top

[R42] 输入重定向
来源：http://keu.aibaodan.cn

wc -l < a.txt
来源：http://cjb.316326.xyz

[R43] 按名字查找文件
来源：http://hrp.chenlongwang.top

find . -name "*.log" -type f
来源：http://iaj.jyoumei.cn

[R44] 按修改时间查找
来源：http://twk.yongpay.top

find . -mtime -7 -type f
来源：http://gty.birdmap.top

[R45] 批量删除
来源：http://nei.xziqi.cn

find . -name "*.tmp" -delete
来源：http://zur.ehwqpu.com

[R46] 递归替换文件内容
来源：http://mzt.iojbl.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dwl.zhongyouzk.top

[R47] sed 单行替换
来源：http://zts.ybcxt.top

sed -i 's/foo/bar/g' a.txt
来源：http://ivv.smart0.xyz

[R48] awk 取指定列
来源：http://ept.chenlongwang.top

awk '{print $1, $3}' a.txt
来源：http://pvt.hywenlv.cn

[R49] awk 带条件
来源：http://hnk.ehwqpu.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yvf.sweek.top

[R50] awk 求和
来源：http://epy.gogol.net.cn

awk '{s += $2} END {print s}' a.txt
来源：http://psu.zhoulong.xyz

[R51] 排序去重取前几
来源：http://mln.yangfankeji.com

sort a.txt | uniq -c | sort -rn | head
来源：http://kxg.daria6918.cn

[R52] 统计行数
来源：http://qso.0kj1m.cn

wc -l a.txt
来源：http://cgb.redwolf501.top

[R53] 查看文件头与实时尾
来源：http://ojv.yuanzhike.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://esx.yongpay.top

[R54] 比较两个文件
来源：http://klg.guowangkeji.top

diff a.txt b.txt
来源：http://mha.xylfe.cn

[R55] 压缩与解压
来源：http://ujk.cashguo.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fqe.shanyushiyangtech.top

[R56] 远程拷贝
来源：http://nqk.hesvh.cn

scp file user@host:/path/
来源：http://ftq.daria6918.cn

[R57] 远程执行命令
来源：http://yvb.sxryk.cn

ssh user@host 'uptime'
来源：http://iyo.0kj1m.cn

[R58] 下载文件
来源：http://esb.yuanzhike.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pyp.mhx1999.top

[R59] 发 POST JSON
来源：http://lwi.jyoumei.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kjk.yuxming.cn

[R60] 只看 HTTP 状态码
来源：http://khw.hongshengwenyu.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vua.hongshengwenyu.top

[R61] 磁盘占用
来源：http://xkr.nwbrower.top

df -h;  du -sh *
来源：http://imj.jlsjyb.cn

[R62] 找最占空间的文件
来源：http://fyj.yj202588.top

du -ah . | sort -rh | head -10
来源：http://xzm.nwbrower.top

[R63] 内存与进程
来源：http://ipa.gzhubu.top

free -h;  ps aux | grep nginx
来源：http://frr.hnxiangtu.top

[R64] 结束进程
来源：http://ehu.gogol.net.cn

kill -9 $(pgrep -f app.py)
来源：http://tst.316326.xyz

[R65] 查看端口占用
来源：http://ukm.yongpay.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dhw.nanxinkj.top

[R66] 定时任务
来源：http://ryc.yueranfly.top

crontab -e;  crontab -l
来源：http://oqo.zhijiandao.cn

[R67] 生成随机十六进制串
来源：http://jbf.ybcxt.top

openssl rand -hex 16
来源：http://nss.yueranfly.top

[R68] 计算文件校验值
来源：http://qtl.vqdsnc.cn

sha256sum a.txt;  md5sum a.txt
来源：http://nef.daria6918.cn

[R69] 生成随机密码
来源：http://onu.wangdashe.top

head -c 16 /dev/urandom | base64
来源：http://blf.jinyuanbaomall.cn

[R70] 时间戳与互转
来源：http://zko.yj202588.top

date +%s;  date -d @1700000000
来源：http://ozn.jianghu66.top

[R71] 日期格式化
来源：http://kun.iojbl.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://jqt.uphjek.com

[R72] 等待端口就绪
来源：http://evk.aibaodan.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://iol.xziqi.cn

[R73] 分割大日志
来源：http://bmw.ehwqpu.com

split -l 1000 big.log part_
来源：http://eqf.chenjidiqi.icu

[R74] 批量重命名
来源：http://jir.tian-w.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://oqy.shangyingyoupin.top

[R75] 导出环境变量
来源：http://pip.fengsongda.top

export PATH="$HOME/bin:$PATH"
来源：http://lyv.gaohongyu789.top

[R76] 使用临时文件
来源：http://hhv.0kj1m.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gxb.yonumen.top

[R77] 读取用户输入
来源：http://clx.9152youxi.cn

read -rp "请输入: " ans
来源：http://ucj.hammf.cn

[R78] 交互式菜单
来源：http://liq.jqgufenzy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://nqe.jinghuilouyu.cn

[R79] 解析命令行选项
来源：http://aeu.fengsongda.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qfb.ydjk.org.cn

[R80] 查看脚本执行耗时
来源：http://jfm.havefunace.top

time ./run.sh
来源：http://set.tarul.cn

================================================================================
来源：http://qzw.jiagoushi.top

S. C / C++ 专题
来源：http://ckh.hfpthk.cn

================================================================================
来源：http://zbp.redwolf501.top

[S01] C：Hello World
来源：http://byc.sufxvd.cn

#include <stdio.h>
来源：http://tbq.nwbrower.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://peh.cashguo.top

[S02] C：变量与格式化输出
来源：http://hhf.zdbjq.cn

int a = 10; printf("%d\n", a);
来源：http://luv.zhongyouzk.top

[S03] C：读入整数
来源：http://pby.mhx1999.top

int x; scanf("%d", &x);
来源：http://rov.hnxiangtu.top

[S04] C：字符串复制
来源：http://kha.gogol.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://mhe.nwbrower.top

[S05] C：字符串长度
来源：http://azq.hysaishi.cn

strlen(s)
来源：http://wtr.shzxlz.cn

[S06] C：字符串比较
来源：http://egk.yonumen.top

strcmp(a, b) == 0
来源：http://wnl.jinyuanbaomall.cn

[S07] C：数组遍历求和
来源：http://ymw.pengpengdd.cyou

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uvv.316326.xyz

[S08] C：动态内存分配与释放
来源：http://erz.shanyushiyangkeji.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tut.yongpay.top

[S09] C：结构体定义与初始化
来源：http://xda.chenlongwang.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cqu.chenjidiqi.icu

[S10] C：指针与解引用
来源：http://jng.ybcxt.top

int *p = &a;  *p = 5;
来源：http://hkh.pycfn.com

[S11] C：逐行读文件
来源：http://nry.sysykeji.top

FILE *f = fopen("a.txt", "r");
来源：http://lgs.ppjwa.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dve.jiagoushi.top

fclose(f);
来源：http://axw.redwolf501.top

[S12] C：写文件
来源：http://kam.xziqi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dry.yueranfly.top

[S13] C：宏定义
来源：http://eci.sweek.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mta.aizwys.cn

[S14] C：枚举
来源：http://val.hfpthk.cn

enum Color { RED, GREEN, BLUE };
来源：http://rsq.jlsjyb.cn

[S15] C：类型转换
来源：http://ora.jinqigufen.top

(double) a / b
来源：http://pee.nanxuanxn.top

[S16] C：位操作置位
来源：http://hwt.redwolf501.top

x |= (1 << 3);
来源：http://oks.yueranfly.top

[S17] C：安全拼接字符串
来源：http://cor.hywenlv.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vkc.yangfankeji.com

[S18] C：命令行参数
来源：http://ysf.xinyue.icu

int main(int argc, char **argv)
来源：http://ojc.gogol.net.cn

[S19] C：快速排序
来源：http://orc.uphjek.com

qsort(a, n, sizeof(int), cmp);
来源：http://plx.snrcjt.cn

[S20] C：二分查找
来源：http://ggn.fehbvm.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pzj.bjfxy.top

[S21] C：字符类别判断
来源：http://xgt.0kj1m.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://uag.ydjk.org.cn

[S22] C：字符串转数字
来源：http://lgi.zhengqikj.top

atoi("42");  strtod("3.14", NULL);
来源：http://esv.tanke756.top

[S23] C：随机数
来源：http://iwc.jiagoushi.top

srand(time(NULL));  int r = rand() % 100;
来源：http://msh.hnxiangtu.top

[S24] C：获取本地时间
来源：http://bcb.havefunace.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://arl.jiagoushi.top

[S25] C：内存拷贝
来源：http://axn.xuanzx.com

memcpy(dst, src, n);
来源：http://tbo.snrcjt.cn

[S26] C：内存清零
来源：http://lai.feifeiyinyue.top

memset(a, 0, sizeof a);
来源：http://wlu.jinqigfzy.top

[S27] C：定义常量
来源：http://rfk.zhiwuduotai.top

const double PI = 3.14159;
来源：http://mom.jinyuanbaomall.cn

[S28] C：静态变量
来源：http://lbu.zdqjudy.top

static int counter = 0;
来源：http://cbi.0kj1m.cn

[S29] C：变参函数
来源：http://yxf.kuanghao11.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dkc.daxiang520.top

[S30] C：头文件保护
来源：http://wpg.zhongyouzk.top

#ifndef X_H
来源：http://saf.aibaodan.cn

#define X_H
来源：http://qkj.jiagoushi.top

#endif
来源：http://qiw.yj20258.top

[S31] C++：Hello World
来源：http://cmx.mhx1999.top

#include <iostream>
来源：http://lnk.kuanghao11.cn

int main() { std::cout << "Hello\n"; }
来源：http://asy.zhongyouzk.top

[S32] C++：字符串
来源：http://urb.zhijiandao.cn

std::string s = "hi";  s += "!";
来源：http://use.tianlin.xyz

[S33] C++：vector 增删
来源：http://qwr.fengsongda.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bul.hongshengwenyu.top

[S34] C++：遍历 vector
来源：http://uhh.kuanghao11.cn

for (auto &x : v) { std::cout << x; }
来源：http://uhx.yongpay.top

[S35] C++：map
来源：http://vse.quarkkingdee.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sxy.cdnleiting.top

[S36] C++：unordered_map
来源：http://zlf.ivvv.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hlc.zycfv.cn

[S37] C++：set
来源：http://rak.hywenlv.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://igw.zhongyouzk.top

[S38] C++：排序
来源：http://efo.redwolf501.top

std::sort(v.begin(), v.end());
来源：http://rla.yongpay.top

[S39] C++：自定义比较器排序
来源：http://dnr.jqgfzy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ggc.hongshengwenyu.top

[S40] C++：查找元素
来源：http://srh.hnxiangtu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://aup.smart0.xyz

[S41] C++：类与构造函数
来源：http://zbs.fktsv.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ctv.yj20258.top

[S42] C++：继承与虚函数
来源：http://pcs.jinqigufen.top

class B : public Base { public: void f() override {} };
来源：http://xuf.hywenlv.cn

[S43] C++：智能指针
来源：http://lhs.yongpay.top

auto p = std::make_unique<int>(5);
来源：http://ytw.feifeiyinyue.top

[S44] C++：引用传参
来源：http://pqe.jinqigufen.top

void inc(int &x) { ++x; }
来源：http://hnf.tanke756.top

[S45] C++：lambda
来源：http://rqk.fktsv.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zln.zhengqikj.top

[S46] C++：函数模板
来源：http://xdq.xinyue.icu

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gsr.birdmap.top

[S47] C++：结构化绑定遍历
来源：http://bfo.sxryk.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zah.cqqwz.cn

[S48] C++：逐行读文件
来源：http://nwq.daria6918.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wma.zhongyouzk.top

while (std::getline(in, line)) { }
来源：http://hlp.jinqigufen.top

[S49] C++：写文件
来源：http://lxg.shzxlz.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pgt.zhongyouzk.top

[S50] C++：格式化数字
来源：http://ijo.havefunace.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vsh.hnxiangtu.top

[S51] C++：显式类型转换
来源：http://rvk.cdnleiting.top

static_cast<double>(a) / b
来源：http://hlk.nanxinkj.top

[S52] C++：const 与 noexcept
来源：http://rtm.daxiang520.top

int size() const noexcept { return n_; }
来源：http://cgt.gotoacloud.top

[S53] C++：移动语义
来源：http://zws.hongshengwenyu.top

std::vector<int> w = std::move(v);
来源：http://yzo.fehbvm.com

[S54] C++：异常处理
来源：http://gag.xziqi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://auw.uphjek.com

[S55] C++：结构化绑定
来源：http://ucm.cheryme.top

auto [a, b] = std::make_pair(1, 2);
来源：http://fpt.hammf.cn

[S56] C++：optional
来源：http://nos.hfpthk.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://sla.daxiang520.top

[S57] C++：编译期常量
来源：http://lwu.yj20258888.top

constexpr int N = 10;
来源：http://krt.fengsongda.top

[S58] C++：命名空间
来源：http://lhx.zycfv.cn

namespace ns { int f() { return 1; } }
来源：http://tms.dianchejie.cn

[S59] C++：静态断言
来源：http://pik.smart0.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jjm.hnxiangtu.top

[S60] C++：遍历并删除元素
来源：http://skq.jianghu66.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dqd.ivvv.top

================================================================================
来源：http://zmw.gotoacloud.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qyc.zycfv.cn

================================================================================
来源：http://qmf.zhongyouzk.top

[T01] Kotlin：Hello World
来源：http://xnm.redwolf501.top

println("Hello")
来源：http://mci.cqqwz.cn

[T02] Kotlin：变量
来源：http://sbn.jinqigufen.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rja.fehbvm.com

[T03] Kotlin：字符串模板
来源：http://zqe.shzxlz.cn

"值: $b"
来源：http://hzj.feifeiyinyue.top

[T04] Kotlin：空安全
来源：http://tks.hesvh.cn

val n: String? = null;  n?.length
来源：http://nxe.nanxuanxn.top

[T05] Kotlin：when 表达式
来源：http://ayq.nanxuanxn.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ipy.jiagoushi.top

[T06] Kotlin：集合映射
来源：http://kde.zhixingplan.top

listOf(1, 2, 3).map { it * 2 }
来源：http://koa.xuetiantiany.cn

[T07] Kotlin：集合过滤
来源：http://owq.hnxiangtu.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://sxx.shangyingyoupin.top

[T08] Kotlin：数据类
来源：http://rxr.jinghuilouyu.cn

data class User(val name: String, val age: Int)
来源：http://mst.jyoumei.cn

[T09] Kotlin：扩展函数
来源：http://twm.guannengcc.top

fun String.exclaim() = this + "!"
来源：http://zlj.dianchejie.cn

[T10] Kotlin：默认参数
来源：http://xpz.sjlbkw.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://uss.yongpay.top

[T11] Kotlin：协程
来源：http://mbw.ydjk.org.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ddt.shanyushiyangkeji.top

[T12] Kotlin：解构声明
来源：http://phy.aizwys.cn

val (a, b) = Pair(1, 2)
来源：http://fyl.zdqjudy.top

[T13] Kotlin：只读 Map
来源：http://iyo.shangyingyoupin.top

val m = mapOf("a" to 1)
来源：http://vqa.jianghu66.top

[T14] Kotlin：循环
来源：http://euj.haohaochexian.top

for (i in 1..10) println(i)
来源：http://eke.yangfankeji.com

[T15] Kotlin：接口
来源：http://uao.guowangkeji.top

interface Shape { fun area(): Double }
来源：http://ang.shanyushiyangkeji.top

[T16] Swift：Hello World
来源：http://xai.hesvh.cn

print("Hello")
来源：http://xxl.tanke756.top

[T17] Swift：变量与常量
来源：http://cum.feifeiyinyue.top

var a = 1;  let b = 2
来源：http://rwo.guowangkeji.top

[T18] Swift：字符串插值
来源：http://zhb.zhaomingkeji.xyz

"值: \(b)"
来源：http://mza.xylfe.cn

[T19] Swift：可选绑定
来源：http://omx.sxryk.cn

if let n = opt { print(n) }
来源：http://mvc.sxryk.cn

[T20] Swift：数组操作
来源：http://rgp.c1oappe.top

var a = [1, 2, 3];  a.append(4)
来源：http://hxf.sysykeji.top

[T21] Swift：遍历
来源：http://cir.yuanzhike.top

for x in a { print(x) }
来源：http://eqb.ctjpmb.com

[T22] Swift：字典
来源：http://hma.fehbvm.com

var d = ["a": 1];  d["b"] = 2
来源：http://usx.hammf.cn

[T23] Swift：函数
来源：http://nye.hywenlv.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wvu.shangyingyoupin.top

[T24] Swift：闭包
来源：http://jqy.zhaomingkeji.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://nie.jinqigufen.top

[T25] Swift：结构体
来源：http://szp.hammf.cn

struct P { var x: Int }
来源：http://kal.zdqjudy.top

[T26] Swift：类与重写
来源：http://poe.yueranfly.top

class A: Base { override func f() {} }
来源：http://fku.shanyushiyangkeji.top


<!-- 参考信息 -->