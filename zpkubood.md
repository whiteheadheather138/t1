代发 wailian999

echo $((1 + 2 * 3))
来源：http://vms.yvedp.cn

[R28] 浮点运算
来源：http://wut.cucudq.cn

echo "scale=2; 10/3" | bc
来源：http://nzh.yuxming.cn

[R29] 定义函数
来源：http://krj.hongshengwenyu.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://msv.wangdashe.top

[R30] 函数返回状态码
来源：http://gni.zdbjq.cn

f() { return 0; }; f || echo "失败了"
来源：http://tbg.chenjidiqi.icu

[R31] 局部变量
来源：http://qri.ydzc1.top

f() { local x=1; echo "$x"; }
来源：http://oxq.shuidangran.top

[R32] 参数个数校验
来源：http://fpg.ivvv.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dej.sweek.top

[R33] 捕获错误并提示行号
来源：http://zkq.sweek.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ebe.shanyushiyangkeji.top

[R34] 退出时清理
来源：http://xtj.vqdsnc.cn

trap 'rm -f "$tmp"' EXIT
来源：http://lqe.cheryme.top

[R35] 后台执行并等待
来源：http://qmo.chenlongwang.top

sleep 5 & pid=$!; wait "$pid"
来源：http://smv.smart0.xyz

[R36] 并发执行多个任务
来源：http://nsk.cqqwz.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hdo.ivvv.top

[R37] 把输出赋给变量
来源：http://mlw.iojbl.cn

files=$(ls -1)
来源：http://tin.hywenlv.cn

[R38] 管道串联
来源：http://izl.wangdashe.top

cat a.txt | grep -i error | wc -l
来源：http://zks.ppjwa.cn

[R39] 重定向标准输出与错误
来源：http://wej.yuxming.cn

cmd > out.log 2>&1
来源：http://vpv.smart0.xyz

[R40] 追加写日志
来源：http://epm.bjfxy.top

echo "log" >> out.log
来源：http://uih.yvedp.cn

[R41] 丢弃输出
来源：http://eqd.dashuyun.cn

cmd >/dev/null 2>&1
来源：http://rsg.yj20258.top

[R42] 输入重定向
来源：http://gmp.yvedp.cn

wc -l < a.txt
来源：http://hrt.cheryme.top

[R43] 按名字查找文件
来源：http://sar.guowangkeji.top

find . -name "*.log" -type f
来源：http://zwb.chenjidiqi.icu

[R44] 按修改时间查找
来源：http://chn.shzxlz.cn

find . -mtime -7 -type f
来源：http://eug.yj20258.top

[R45] 批量删除
来源：http://xro.cqqwz.cn

find . -name "*.tmp" -delete
来源：http://gev.daxiang520.top

[R46] 递归替换文件内容
来源：http://fwk.ppjwa.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gmm.gzhubu.top

[R47] sed 单行替换
来源：http://agh.yj202588.top

sed -i 's/foo/bar/g' a.txt
来源：http://hhk.aizwys.cn

[R48] awk 取指定列
来源：http://cde.guannengcc.top

awk '{print $1, $3}' a.txt
来源：http://qjd.shuidangran.top

[R49] awk 带条件
来源：http://atc.hcnkem.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://oji.316326.xyz

[R50] awk 求和
来源：http://bwu.havefunace.top

awk '{s += $2} END {print s}' a.txt
来源：http://sod.vqdsnc.cn

[R51] 排序去重取前几
来源：http://dqq.wangshuangyany.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://enl.havefunace.top

[R52] 统计行数
来源：http://vkn.cqqwz.cn

wc -l a.txt
来源：http://nmw.vehdjk.com

[R53] 查看文件头与实时尾
来源：http://cry.cdnleiting.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xww.zhoulong.xyz

[R54] 比较两个文件
来源：http://upm.hysaishi.cn

diff a.txt b.txt
来源：http://paj.quarkkingdee.top

[R55] 压缩与解压
来源：http://uom.yonumen.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vre.chenjidiqi.icu

[R56] 远程拷贝
来源：http://fpg.ctjpmb.com

scp file user@host:/path/
来源：http://jsr.ydjk.org.cn

[R57] 远程执行命令
来源：http://ogs.jqgfzy.top

ssh user@host 'uptime'
来源：http://buj.daxiang520.top

[R58] 下载文件
来源：http://zni.yuanzhike.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rnq.0kj1m.cn

[R59] 发 POST JSON
来源：http://dsb.redwolf501.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tav.uphjek.com

[R60] 只看 HTTP 状态码
来源：http://vnd.nwbrower.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tnq.jlsjyb.cn

[R61] 磁盘占用
来源：http://nly.havefunace.top

df -h;  du -sh *
来源：http://zje.ehwqpu.com

[R62] 找最占空间的文件
来源：http://mai.shzxlz.cn

du -ah . | sort -rh | head -10
来源：http://gyc.aibaodan.cn

[R63] 内存与进程
来源：http://ltz.c1oappe.top

free -h;  ps aux | grep nginx
来源：http://rck.gzhubu.top

[R64] 结束进程
来源：http://ezb.zdbjq.cn

kill -9 $(pgrep -f app.py)
来源：http://wua.xuetiantiany.cn

[R65] 查看端口占用
来源：http://awj.cucudq.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dys.bbcook.cn

[R66] 定时任务
来源：http://jeu.havefunace.top

crontab -e;  crontab -l
来源：http://ivb.hnxiangtu.top

[R67] 生成随机十六进制串
来源：http://tso.nanxinkj.top

openssl rand -hex 16
来源：http://vgp.redwolf501.top

[R68] 计算文件校验值
来源：http://lwr.chenzaomai.com

sha256sum a.txt;  md5sum a.txt
来源：http://uxx.daria6918.cn

[R69] 生成随机密码
来源：http://bag.uphjek.com

head -c 16 /dev/urandom | base64
来源：http://djo.hesvh.cn

[R70] 时间戳与互转
来源：http://ftr.epnwcf.com

date +%s;  date -d @1700000000
来源：http://nyl.meibo888.top

[R71] 日期格式化
来源：http://jki.daxiang520.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://clf.yuanzhike.top

[R72] 等待端口就绪
来源：http://zat.nwbrower.top

until nc -z localhost 3306; do sleep 1; done
来源：http://cqm.ctjpmb.com

[R73] 分割大日志
来源：http://rjk.chenlongwang.top

split -l 1000 big.log part_
来源：http://ntc.uphjek.com

[R74] 批量重命名
来源：http://ahv.dianchejie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qob.yonumen.top

[R75] 导出环境变量
来源：http://plj.vqdsnc.cn

export PATH="$HOME/bin:$PATH"
来源：http://mqd.zhongyouzk.top

[R76] 使用临时文件
来源：http://dgh.yj202588.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nok.zhongyouzk.top

[R77] 读取用户输入
来源：http://vgi.tianlin.xyz

read -rp "请输入: " ans
来源：http://rqn.ivvv.top

[R78] 交互式菜单
来源：http://pia.jqgfzy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://pxs.ydjk.org.cn

[R79] 解析命令行选项
来源：http://oix.bbcook.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qqy.cdnleiting.top

[R80] 查看脚本执行耗时
来源：http://qcj.jlsjyb.cn

time ./run.sh
来源：http://smv.sufxvd.cn

================================================================================
来源：http://pgl.sweek.top

S. C / C++ 专题
来源：http://feh.zdqjudy.top

================================================================================
来源：http://rfn.mhx1999.top

[S01] C：Hello World
来源：http://qag.epnwcf.com

#include <stdio.h>
来源：http://drm.shangyingyoupin.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://gzj.feifeiyinyue.top

[S02] C：变量与格式化输出
来源：http://epj.wangdashe.top

int a = 10; printf("%d\n", a);
来源：http://yms.dashuyun.cn

[S03] C：读入整数
来源：http://ldg.shuidangran.top

int x; scanf("%d", &x);
来源：http://bdp.havefunace.top

[S04] C：字符串复制
来源：http://xtv.hongshengwenyu.top

char dst[32]; strcpy(dst, "hi");
来源：http://exj.shanyushiyangkeji.top

[S05] C：字符串长度
来源：http://ifl.hnxiangtu.top

strlen(s)
来源：http://wly.ehwqpu.com

[S06] C：字符串比较
来源：http://yge.jyoumei.cn

strcmp(a, b) == 0
来源：http://mjc.jinqigfzy.top

[S07] C：数组遍历求和
来源：http://ovu.316326.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sof.andypj.xyz

[S08] C：动态内存分配与释放
来源：http://mkz.yj20258.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jvk.havefunace.top

[S09] C：结构体定义与初始化
来源：http://sar.yfazqb.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ynz.shuidangran.top

[S10] C：指针与解引用
来源：http://hxi.zhaomingkeji.xyz

int *p = &a;  *p = 5;
来源：http://eid.andypj.xyz

[S11] C：逐行读文件
来源：http://dww.zhengqikj.top

FILE *f = fopen("a.txt", "r");
来源：http://orn.9152youxi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dyo.yonumen.top

fclose(f);
来源：http://uee.shuidangran.top

[S12] C：写文件
来源：http://dvq.shzxlz.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zxn.iojbl.cn

[S13] C：宏定义
来源：http://oyf.jinqigfzy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ics.hfpthk.cn

[S14] C：枚举
来源：http://uyu.yonumen.top

enum Color { RED, GREEN, BLUE };
来源：http://pil.jyoumei.cn

[S15] C：类型转换
来源：http://tln.pengpengdd.cyou

(double) a / b
来源：http://bpa.hywenlv.cn

[S16] C：位操作置位
来源：http://gpb.feifeiyinyue.top

x |= (1 << 3);
来源：http://dnd.jinghuilouyu.cn

[S17] C：安全拼接字符串
来源：http://gsb.sxryk.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hdc.wangdashe.top

[S18] C：命令行参数
来源：http://mle.smart0.xyz

int main(int argc, char **argv)
来源：http://mfn.hnxiangtu.top

[S19] C：快速排序
来源：http://uio.52xcode.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qlz.bbcook.cn

[S20] C：二分查找
来源：http://fcb.hongshengwenyu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ogo.nanxinkj.top

[S21] C：字符类别判断
来源：http://msz.tianlin.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yad.hcnkem.com

[S22] C：字符串转数字
来源：http://unn.fanxiaobao.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://ciz.sjlbkw.cn

[S23] C：随机数
来源：http://rhp.yuanzhike.top

srand(time(NULL));  int r = rand() % 100;
来源：http://uer.zhengqikj.top

[S24] C：获取本地时间
来源：http://bwi.ivvv.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jht.tanke756.top

[S25] C：内存拷贝
来源：http://ujz.shanyushiyangkeji.top

memcpy(dst, src, n);
来源：http://byv.nanxuanxn.top

[S26] C：内存清零
来源：http://kco.birdmap.top

memset(a, 0, sizeof a);
来源：http://nuu.gzhubu.top

[S27] C：定义常量
来源：http://raw.hnqzz.top

const double PI = 3.14159;
来源：http://qtk.bbcook.cn

[S28] C：静态变量
来源：http://ibb.andypj.xyz

static int counter = 0;
来源：http://ror.meibo888.top

[S29] C：变参函数
来源：http://cad.iojbl.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uke.wangdashe.top

[S30] C：头文件保护
来源：http://gyz.hfpthk.cn

#ifndef X_H
来源：http://jbe.jyoumei.cn

#define X_H
来源：http://jkd.vqdsnc.cn

#endif
来源：http://tye.jlsjyb.cn

[S31] C++：Hello World
来源：http://zkv.jinghuilouyu.cn

#include <iostream>
来源：http://efb.quarkkingdee.top

int main() { std::cout << "Hello\n"; }
来源：http://sfl.xuetiantiany.cn

[S32] C++：字符串
来源：http://glx.zycfv.cn

std::string s = "hi";  s += "!";
来源：http://htr.pengpengdd.cyou

[S33] C++：vector 增删
来源：http://qtc.jianghu66.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xin.zhixingplan.top

[S34] C++：遍历 vector
来源：http://muy.fktsv.cn

for (auto &x : v) { std::cout << x; }
来源：http://wdn.xuanzx.com

[S35] C++：map
来源：http://fnh.ydzc1.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mbt.kuanghao11.cn

[S36] C++：unordered_map
来源：http://wsq.yonumen.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xvt.zycfv.cn

[S37] C++：set
来源：http://ykn.zhiwuduotai.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ode.nanxuanxn.top

[S38] C++：排序
来源：http://kfy.aizwys.cn

std::sort(v.begin(), v.end());
来源：http://xtx.guowangkeji.top

[S39] C++：自定义比较器排序
来源：http://uwa.yanxiufei.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tak.fengsongda.top

[S40] C++：查找元素
来源：http://sit.zhongyouzk.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bdx.ppjwa.cn

[S41] C++：类与构造函数
来源：http://tpu.jqgufenzy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mwj.jlsjyb.cn

[S42] C++：继承与虚函数
来源：http://ebq.chenzaomai.com

class B : public Base { public: void f() override {} };
来源：http://hkd.shuidangran.top

[S43] C++：智能指针
来源：http://fgl.hnxiangtu.top

auto p = std::make_unique<int>(5);
来源：http://dzo.hnxiangtu.top

[S44] C++：引用传参
来源：http://yxg.fehbvm.com

void inc(int &x) { ++x; }
来源：http://jlq.fzhhl.top

[S45] C++：lambda
来源：http://epw.ydzc1.top

auto add = [](int a, int b) { return a + b; };
来源：http://ppb.hfpthk.cn

[S46] C++：函数模板
来源：http://nyl.shuidangran.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hsb.andypj.xyz

[S47] C++：结构化绑定遍历
来源：http://lgu.nanxuanxn.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pfs.hnqzz.top

[S48] C++：逐行读文件
来源：http://gcc.vehdjk.com

std::ifstream in("a.txt");  std::string line;
来源：http://fxk.hongshengwenyu.top

while (std::getline(in, line)) { }
来源：http://qld.xylfe.cn

[S49] C++：写文件
来源：http://eoa.zhongyouzk.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blm.hongshengwenyu.top

[S50] C++：格式化数字
来源：http://mgs.pycfn.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dro.yongpay.top

[S51] C++：显式类型转换
来源：http://ejw.ppjwa.cn

static_cast<double>(a) / b
来源：http://acm.ivvv.top

[S52] C++：const 与 noexcept
来源：http://vmj.fanxiaobao.xyz

int size() const noexcept { return n_; }
来源：http://bhj.jyoumei.cn

[S53] C++：移动语义
来源：http://pca.gzhubu.top

std::vector<int> w = std::move(v);
来源：http://pqz.pycfn.com

[S54] C++：异常处理
来源：http://hss.52xcode.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jjp.hysaishi.cn

[S55] C++：结构化绑定
来源：http://xeg.cdnleiting.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ssm.meibo888.top

[S56] C++：optional
来源：http://fwj.fzhhl.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nbe.jiagoushi.top

[S57] C++：编译期常量
来源：http://eoz.cqqwz.cn

constexpr int N = 10;
来源：http://fjq.chenlongwang.top

[S58] C++：命名空间
来源：http://rkl.cqqwz.cn

namespace ns { int f() { return 1; } }
来源：http://aqv.c1oappe.top

[S59] C++：静态断言
来源：http://knb.jianghu66.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dis.dashuyun.cn

[S60] C++：遍历并删除元素
来源：http://ahe.hammf.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dns.cqqwz.cn

================================================================================
来源：http://shj.sufxvd.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zjv.pengpengdd.cyou

================================================================================
来源：http://vci.yvedp.cn

[T01] Kotlin：Hello World
来源：http://vjf.ybcxt.top

println("Hello")
来源：http://ffv.feifeiyinyue.top

[T02] Kotlin：变量
来源：http://onv.hfpthk.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qmp.shangyingyoupin.top

[T03] Kotlin：字符串模板
来源：http://wbr.ydzc1.top

"值: $b"
来源：http://jmg.guannengcc.top

[T04] Kotlin：空安全
来源：http://ufa.zdbjq.cn

val n: String? = null;  n?.length
来源：http://zkj.dianchejie.cn

[T05] Kotlin：when 表达式
来源：http://blo.daria6918.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ylc.yueranfly.top

[T06] Kotlin：集合映射
来源：http://dqg.sjlbkw.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://sbi.wangdashe.top

[T07] Kotlin：集合过滤
来源：http://tpz.smart0.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://quw.fktsv.cn

[T08] Kotlin：数据类
来源：http://dlm.andypj.xyz

data class User(val name: String, val age: Int)
来源：http://lko.wangdashe.top

[T09] Kotlin：扩展函数
来源：http://tay.hesvh.cn

fun String.exclaim() = this + "!"
来源：http://etp.shangyingyoupin.top

[T10] Kotlin：默认参数
来源：http://jcm.jinqigufen.top

fun greet(name: String = "World") = "Hi $name"
来源：http://vzf.gaohongyu789.top

[T11] Kotlin：协程
来源：http://ecs.hfpthk.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://fac.feifeiyinyue.top

[T12] Kotlin：解构声明
来源：http://wif.yonumen.top

val (a, b) = Pair(1, 2)
来源：http://bkn.xinyue.icu

[T13] Kotlin：只读 Map
来源：http://wcq.jinqigufen.top

val m = mapOf("a" to 1)
来源：http://mvq.daxiang520.top

[T14] Kotlin：循环
来源：http://wim.haohaochexian.top

for (i in 1..10) println(i)
来源：http://rwp.jianghu66.top

[T15] Kotlin：接口
来源：http://jmv.fzhhl.top

interface Shape { fun area(): Double }
来源：http://zvp.shanyushiyangkeji.top

[T16] Swift：Hello World
来源：http://jcz.ybcxt.top

print("Hello")
来源：http://rhj.cdnleiting.top

[T17] Swift：变量与常量
来源：http://cpb.yonumen.top

var a = 1;  let b = 2
来源：http://wvr.jinqigfzy.top

[T18] Swift：字符串插值
来源：http://pgq.yanxiufei.cn

"值: \(b)"
来源：http://bsn.gzhubu.top

[T19] Swift：可选绑定
来源：http://orx.yvedp.cn

if let n = opt { print(n) }
来源：http://qlf.uphjek.com

[T20] Swift：数组操作
来源：http://due.andypj.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://eva.yangfankeji.com

[T21] Swift：遍历
来源：http://qnp.tianlin.xyz

for x in a { print(x) }
来源：http://nvl.yongpay.top

[T22] Swift：字典
来源：http://sxu.daria6918.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fsb.tarul.cn

[T23] Swift：函数
来源：http://wbo.xylfe.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xfd.daxiang520.top

[T24] Swift：闭包
来源：http://xml.chenzaomai.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://znt.yvedp.cn

[T25] Swift：结构体
来源：http://xgg.hongshengwenyu.top

struct P { var x: Int }
来源：http://mgl.shzxlz.cn

[T26] Swift：类与重写
来源：http://izo.nanxuanxn.top

class A: Base { override func f() {} }
来源：http://epl.hysaishi.cn

[T27] Swift：错误处理
来源：http://kxi.xziqi.cn

do { try f() } catch { print(error) }
来源：http://clf.birdmap.top

[T28] Swift：枚举
来源：http://frs.xylfe.cn

enum Color { case red, green }
来源：http://ywo.uphjek.com

[T29] Swift：guard 提前返回
来源：http://txx.ivvv.top

guard let x = opt else { return }
来源：http://rte.kuanghao11.cn

[T30] Swift：协议
来源：http://sps.yuanzhike.top

protocol Shape { func area() -> Double }
来源：http://wnh.jyoumei.cn


<!-- 参考信息 -->