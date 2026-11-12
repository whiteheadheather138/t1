代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://oie.feifeiyinyue.top

[R30] 函数返回状态码
来源：http://wzn.vehdjk.com

f() { return 0; }; f || echo "失败了"
来源：http://hps.gzhubu.top

[R31] 局部变量
来源：http://piv.zdqjudy.top

f() { local x=1; echo "$x"; }
来源：http://fyo.hammf.cn

[R32] 参数个数校验
来源：http://cqz.tian-w.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gbg.fktsv.cn

[R33] 捕获错误并提示行号
来源：http://yrf.hongshengwenyu.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://adx.zhaomingkeji.xyz

[R34] 退出时清理
来源：http://ebi.redwolf501.top

trap 'rm -f "$tmp"' EXIT
来源：http://gkn.zhijiandao.cn

[R35] 后台执行并等待
来源：http://xju.jlsjyb.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://llf.xylfe.cn

[R36] 并发执行多个任务
来源：http://uhw.redwolf501.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dhl.0kj1m.cn

[R37] 把输出赋给变量
来源：http://xnt.aizwys.cn

files=$(ls -1)
来源：http://yva.nanxinkj.top

[R38] 管道串联
来源：http://ywk.havefunace.top

cat a.txt | grep -i error | wc -l
来源：http://vnx.cqqwz.cn

[R39] 重定向标准输出与错误
来源：http://bwm.ppjwa.cn

cmd > out.log 2>&1
来源：http://zyc.jqgfzy.top

[R40] 追加写日志
来源：http://zhk.xingfuxueyuan.xyz

echo "log" >> out.log
来源：http://lwv.jqgufenzy.top

[R41] 丢弃输出
来源：http://cou.fzhhl.top

cmd >/dev/null 2>&1
来源：http://rko.svipenyu.cn

[R42] 输入重定向
来源：http://hjr.yuxming.cn

wc -l < a.txt
来源：http://cxy.redwolf501.top

[R43] 按名字查找文件
来源：http://twf.yueranfly.top

find . -name "*.log" -type f
来源：http://zyk.hcnkem.com

[R44] 按修改时间查找
来源：http://xez.yj20258.top

find . -mtime -7 -type f
来源：http://ocg.yueranfly.top

[R45] 批量删除
来源：http://gxs.snrcjt.cn

find . -name "*.tmp" -delete
来源：http://hnu.tianlin.xyz

[R46] 递归替换文件内容
来源：http://yjb.dashuyun.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cnn.xylfe.cn

[R47] sed 单行替换
来源：http://kcm.52xcode.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vmt.hammf.cn

[R48] awk 取指定列
来源：http://ujs.sufxvd.cn

awk '{print $1, $3}' a.txt
来源：http://cho.shanyushiyangtech.top

[R49] awk 带条件
来源：http://hfn.jinghuilouyu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wdh.nwbrower.top

[R50] awk 求和
来源：http://ped.dianchejie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zly.xylfe.cn

[R51] 排序去重取前几
来源：http://cdf.hysaishi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://rxo.fengsongda.top

[R52] 统计行数
来源：http://jqy.jinghuilouyu.cn

wc -l a.txt
来源：http://duk.hcnkem.com

[R53] 查看文件头与实时尾
来源：http://wuk.havefunace.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ugm.jianghu66.top

[R54] 比较两个文件
来源：http://gps.dashuyun.cn

diff a.txt b.txt
来源：http://fts.zhixingplan.top

[R55] 压缩与解压
来源：http://jdh.ywan-chungtsiang.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tmc.nwbrower.top

[R56] 远程拷贝
来源：http://sjz.vqdsnc.cn

scp file user@host:/path/
来源：http://eib.hfpthk.cn

[R57] 远程执行命令
来源：http://ozx.smart0.xyz

ssh user@host 'uptime'
来源：http://tlu.xuetiantiany.cn

[R58] 下载文件
来源：http://exj.nwbrower.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://apm.gaohongyu789.top

[R59] 发 POST JSON
来源：http://anr.yueranfly.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://csm.jinyuanbaomall.cn

[R60] 只看 HTTP 状态码
来源：http://dpe.vehdjk.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kek.jinqigufen.top

[R61] 磁盘占用
来源：http://caq.yvedp.cn

df -h;  du -sh *
来源：http://obu.hcnkem.com

[R62] 找最占空间的文件
来源：http://wyc.hnxiangtu.top

du -ah . | sort -rh | head -10
来源：http://jie.fzhhl.top

[R63] 内存与进程
来源：http://kmp.guannengcc.top

free -h;  ps aux | grep nginx
来源：http://rjy.ehwqpu.com

[R64] 结束进程
来源：http://fba.shanyushiyangtech.top

kill -9 $(pgrep -f app.py)
来源：http://bis.zhijiandao.cn

[R65] 查看端口占用
来源：http://vfg.zhoulong.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yzf.52xcode.cn

[R66] 定时任务
来源：http://afn.svipenyu.cn

crontab -e;  crontab -l
来源：http://nsm.svipenyu.cn

[R67] 生成随机十六进制串
来源：http://rzs.aizwys.cn

openssl rand -hex 16
来源：http://szd.jinqigfzy.top

[R68] 计算文件校验值
来源：http://bam.nanxuanxn.top

sha256sum a.txt;  md5sum a.txt
来源：http://tta.ydjk.org.cn

[R69] 生成随机密码
来源：http://etk.shangyingyoupin.top

head -c 16 /dev/urandom | base64
来源：http://kca.jiagoushi.top

[R70] 时间戳与互转
来源：http://nyt.snrcjt.cn

date +%s;  date -d @1700000000
来源：http://pyd.dashuyun.cn

[R71] 日期格式化
来源：http://xvw.daria6918.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://opq.yuanzhike.top

[R72] 等待端口就绪
来源：http://nly.fanxiaobao.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://eto.shzxlz.cn

[R73] 分割大日志
来源：http://xbv.haohaochexian.top

split -l 1000 big.log part_
来源：http://iru.hammf.cn

[R74] 批量重命名
来源：http://yth.xuanzx.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tmx.svipenyu.cn

[R75] 导出环境变量
来源：http://cro.ivvv.top

export PATH="$HOME/bin:$PATH"
来源：http://hxv.xinyue.icu

[R76] 使用临时文件
来源：http://iqj.aizwys.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vtn.zdbjq.cn

[R77] 读取用户输入
来源：http://ovy.gotoacloud.top

read -rp "请输入: " ans
来源：http://hsb.xinyue.icu

[R78] 交互式菜单
来源：http://edm.fanxiaobao.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://dmw.jiagoushi.top

[R79] 解析命令行选项
来源：http://gke.yvedp.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://njc.cashguo.top

[R80] 查看脚本执行耗时
来源：http://fxf.cashguo.top

time ./run.sh
来源：http://uji.sxryk.cn

================================================================================
来源：http://ufl.hongshengwenyu.top

S. C / C++ 专题
来源：http://ant.nanxuanxn.top

================================================================================
来源：http://vgx.xylfe.cn

[S01] C：Hello World
来源：http://xdt.redwolf501.top

#include <stdio.h>
来源：http://sxh.yvedp.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ygm.mhx1999.top

[S02] C：变量与格式化输出
来源：http://bqj.xinyue.icu

int a = 10; printf("%d\n", a);
来源：http://rxc.fengsongda.top

[S03] C：读入整数
来源：http://wsb.aizwys.cn

int x; scanf("%d", &x);
来源：http://vnw.guannengcc.top

[S04] C：字符串复制
来源：http://kom.xuetiantiany.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ymq.nanxinkj.top

[S05] C：字符串长度
来源：http://gwy.nwbrower.top

strlen(s)
来源：http://ecn.xinyue.icu

[S06] C：字符串比较
来源：http://eum.nanxuanxn.top

strcmp(a, b) == 0
来源：http://agj.yj202588.top

[S07] C：数组遍历求和
来源：http://stk.yuanzhike.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lex.bbcook.cn

[S08] C：动态内存分配与释放
来源：http://ppd.hysaishi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uid.52xcode.cn

[S09] C：结构体定义与初始化
来源：http://kae.fehbvm.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xya.chenjidiqi.icu

[S10] C：指针与解引用
来源：http://foe.hesvh.cn

int *p = &a;  *p = 5;
来源：http://mdo.redwolf501.top

[S11] C：逐行读文件
来源：http://xai.hongshengwenyu.top

FILE *f = fopen("a.txt", "r");
来源：http://eem.meibo888.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ttc.52xcode.cn

fclose(f);
来源：http://iuw.fehbvm.com

[S12] C：写文件
来源：http://dnz.zhaomingkeji.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fip.redwolf501.top

[S13] C：宏定义
来源：http://zcs.gotoacloud.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://clz.ppjwa.cn

[S14] C：枚举
来源：http://mkz.andypj.xyz

enum Color { RED, GREEN, BLUE };
来源：http://frh.hesvh.cn

[S15] C：类型转换
来源：http://pok.iojbl.cn

(double) a / b
来源：http://utn.tian-w.cn

[S16] C：位操作置位
来源：http://wmw.jianghu66.top

x |= (1 << 3);
来源：http://ntg.xylfe.cn

[S17] C：安全拼接字符串
来源：http://dqt.xuetiantiany.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lok.zdbjq.cn

[S18] C：命令行参数
来源：http://lyw.feifeiyinyue.top

int main(int argc, char **argv)
来源：http://mua.chenzaomai.com

[S19] C：快速排序
来源：http://bqt.jianghu66.top

qsort(a, n, sizeof(int), cmp);
来源：http://mmx.gaohongyu789.top

[S20] C：二分查找
来源：http://jqp.gotoacloud.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rdo.316326.xyz

[S21] C：字符类别判断
来源：http://smg.fanxiaobao.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wpx.tanke756.top

[S22] C：字符串转数字
来源：http://dfu.wangdashe.top

atoi("42");  strtod("3.14", NULL);
来源：http://thg.fehbvm.com

[S23] C：随机数
来源：http://vih.jlsjyb.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://lwd.hcnkem.com

[S24] C：获取本地时间
来源：http://xjm.shanyushiyangtech.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ywq.yueranfly.top

[S25] C：内存拷贝
来源：http://iow.dianchejie.cn

memcpy(dst, src, n);
来源：http://jpa.feifeiyinyue.top

[S26] C：内存清零
来源：http://orq.zhoulong.xyz

memset(a, 0, sizeof a);
来源：http://del.epnwcf.com

[S27] C：定义常量
来源：http://pgb.ivvv.top

const double PI = 3.14159;
来源：http://ael.zhixingplan.top

[S28] C：静态变量
来源：http://qfx.hcnkem.com

static int counter = 0;
来源：http://kes.gogol.net.cn

[S29] C：变参函数
来源：http://nin.cheryme.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tai.gogol.net.cn

[S30] C：头文件保护
来源：http://lwc.nwbrower.top

#ifndef X_H
来源：http://uiv.xuanzx.com

#define X_H
来源：http://asd.0kj1m.cn

#endif
来源：http://xax.nanxinkj.top

[S31] C++：Hello World
来源：http://vhn.vqdsnc.cn

#include <iostream>
来源：http://ahv.chenjidiqi.icu

int main() { std::cout << "Hello\n"; }
来源：http://fnx.hfpthk.cn

[S32] C++：字符串
来源：http://udx.ydjk.org.cn

std::string s = "hi";  s += "!";
来源：http://oqz.ywan-chungtsiang.top

[S33] C++：vector 增删
来源：http://umr.shangyingyoupin.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qda.shzxlz.cn

[S34] C++：遍历 vector
来源：http://kff.jinyuanbaomall.cn

for (auto &x : v) { std::cout << x; }
来源：http://vxl.xziqi.cn

[S35] C++：map
来源：http://sdy.jyoumei.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jxd.aibaodan.cn

[S36] C++：unordered_map
来源：http://fah.wangshuangyany.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jrz.redwolf501.top

[S37] C++：set
来源：http://onl.yonumen.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qsm.vqdsnc.cn

[S38] C++：排序
来源：http://bok.mhx1999.top

std::sort(v.begin(), v.end());
来源：http://xui.yangfankeji.com

[S39] C++：自定义比较器排序
来源：http://xtj.hfpthk.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://aho.sjlbkw.cn

[S40] C++：查找元素
来源：http://dwh.havefunace.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zfy.c1oappe.top

[S41] C++：类与构造函数
来源：http://rsz.zhaomingkeji.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ahx.jiagoushi.top

[S42] C++：继承与虚函数
来源：http://mky.hfpthk.cn

class B : public Base { public: void f() override {} };
来源：http://uzm.nanxinkj.top

[S43] C++：智能指针
来源：http://ffg.ydzc1.top

auto p = std::make_unique<int>(5);
来源：http://eku.chenlongwang.top

[S44] C++：引用传参
来源：http://cgb.xziqi.cn

void inc(int &x) { ++x; }
来源：http://wsh.tianlin.xyz

[S45] C++：lambda
来源：http://cxk.zhijiandao.cn

auto add = [](int a, int b) { return a + b; };
来源：http://cyn.vehdjk.com

[S46] C++：函数模板
来源：http://lak.hnqzz.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fri.guowangkeji.top

[S47] C++：结构化绑定遍历
来源：http://ubq.hfpthk.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qcb.yongpay.top

[S48] C++：逐行读文件
来源：http://hqp.zhiwuduotai.top

std::ifstream in("a.txt");  std::string line;
来源：http://ncu.shzxlz.cn

while (std::getline(in, line)) { }
来源：http://eyr.yj20258888.top

[S49] C++：写文件
来源：http://fsm.9152youxi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vfo.316326.xyz

[S50] C++：格式化数字
来源：http://rts.ywan-chungtsiang.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yxb.xuetiantiany.cn

[S51] C++：显式类型转换
来源：http://jgw.ydjk.org.cn

static_cast<double>(a) / b
来源：http://qcp.iojbl.cn

[S52] C++：const 与 noexcept
来源：http://uwp.aibaodan.cn

int size() const noexcept { return n_; }
来源：http://rir.zhixingplan.top

[S53] C++：移动语义
来源：http://ulm.shuidangran.top

std::vector<int> w = std::move(v);
来源：http://fij.jqgufenzy.top

[S54] C++：异常处理
来源：http://qnm.zhaomingkeji.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://utj.andypj.xyz

[S55] C++：结构化绑定
来源：http://ksk.hesvh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vyh.ivvv.top

[S56] C++：optional
来源：http://wwe.kuanghao11.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bcy.tianlin.xyz

[S57] C++：编译期常量
来源：http://pvx.xylfe.cn

constexpr int N = 10;
来源：http://poh.ybcxt.top

[S58] C++：命名空间
来源：http://zqm.shzxlz.cn

namespace ns { int f() { return 1; } }
来源：http://jtl.9152youxi.cn

[S59] C++：静态断言
来源：http://fem.cucudq.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dij.cucudq.cn

[S60] C++：遍历并删除元素
来源：http://jfl.quarkkingdee.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rkw.yangfankeji.com

================================================================================
来源：http://fcl.haohaochexian.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dhw.xylfe.cn

================================================================================
来源：http://qfv.guowangkeji.top

[T01] Kotlin：Hello World
来源：http://ybz.hnxiangtu.top

println("Hello")
来源：http://nof.zycfv.cn

[T02] Kotlin：变量
来源：http://foh.zdqjudy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://biq.fanxiaobao.xyz

[T03] Kotlin：字符串模板
来源：http://qyb.nanxuanxn.top

"值: $b"
来源：http://fqa.hysaishi.cn

[T04] Kotlin：空安全
来源：http://xmu.quarkkingdee.top

val n: String? = null;  n?.length
来源：http://wnx.sxryk.cn

[T05] Kotlin：when 表达式
来源：http://juy.hysaishi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ohc.xylfe.cn

[T06] Kotlin：集合映射
来源：http://khv.sweek.top

listOf(1, 2, 3).map { it * 2 }
来源：http://bub.zhiwuduotai.top

[T07] Kotlin：集合过滤
来源：http://aqr.uphjek.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://ohq.shanyushiyangkeji.top

[T08] Kotlin：数据类
来源：http://qgw.hnxiangtu.top

data class User(val name: String, val age: Int)
来源：http://emp.daria6918.cn

[T09] Kotlin：扩展函数
来源：http://fda.cucudq.cn

fun String.exclaim() = this + "!"
来源：http://lkm.sufxvd.cn

[T10] Kotlin：默认参数
来源：http://bfw.gzhubu.top

fun greet(name: String = "World") = "Hi $name"
来源：http://gui.smart0.xyz

[T11] Kotlin：协程
来源：http://pxl.fehbvm.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://plx.jqgfzy.top

[T12] Kotlin：解构声明
来源：http://wsj.gotoacloud.top

val (a, b) = Pair(1, 2)
来源：http://jqj.daria6918.cn

[T13] Kotlin：只读 Map
来源：http://jjz.sufxvd.cn

val m = mapOf("a" to 1)
来源：http://npx.svipenyu.cn

[T14] Kotlin：循环
来源：http://lmv.sxryk.cn

for (i in 1..10) println(i)
来源：http://jfy.birdmap.top

[T15] Kotlin：接口
来源：http://uev.xingfuxueyuan.xyz

interface Shape { fun area(): Double }
来源：http://mrh.shanyushiyangkeji.top

[T16] Swift：Hello World
来源：http://tcv.shuidangran.top

print("Hello")
来源：http://yal.yuanzhike.top

[T17] Swift：变量与常量
来源：http://vbs.sweek.top

var a = 1;  let b = 2
来源：http://wbu.daria6918.cn

[T18] Swift：字符串插值
来源：http://suk.chenjidiqi.icu

"值: \(b)"
来源：http://nqb.hnxiangtu.top

[T19] Swift：可选绑定
来源：http://nik.jiagoushi.top

if let n = opt { print(n) }
来源：http://asb.fzhhl.top

[T20] Swift：数组操作
来源：http://smb.tian-w.cn

var a = [1, 2, 3];  a.append(4)
来源：http://obo.ydjk.org.cn

[T21] Swift：遍历
来源：http://cvf.cdnleiting.top

for x in a { print(x) }
来源：http://jun.sxryk.cn

[T22] Swift：字典
来源：http://nin.zycfv.cn

var d = ["a": 1];  d["b"] = 2
来源：http://tvh.birdmap.top

[T23] Swift：函数
来源：http://cdp.meibo888.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yic.shangyingyoupin.top

[T24] Swift：闭包
来源：http://ssh.shzxlz.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://yaf.nanxuanxn.top

[T25] Swift：结构体
来源：http://uqg.9152youxi.cn

struct P { var x: Int }
来源：http://rfi.mhx1999.top

[T26] Swift：类与重写
来源：http://skw.nanxinkj.top

class A: Base { override func f() {} }
来源：http://dux.0kj1m.cn

[T27] Swift：错误处理
来源：http://hda.zycfv.cn

do { try f() } catch { print(error) }
来源：http://vcr.jqgfzy.top

[T28] Swift：枚举
来源：http://osj.sufxvd.cn

enum Color { case red, green }
来源：http://tah.shanyushiyangkeji.top

[T29] Swift：guard 提前返回
来源：http://vmm.316326.xyz

guard let x = opt else { return }
来源：http://ylb.sxryk.cn

[T30] Swift：协议
来源：http://qhn.dashuyun.cn

protocol Shape { func area() -> Double }
来源：http://bun.0kj1m.cn

[T31] Lua：Hello World
来源：http://ccw.nanxinkj.top

print("Hello")
来源：http://sek.zhoulong.xyz

[T32] Lua：局部变量
来源：http://dce.zhijiandao.cn

local a = 1
来源：http://hkx.dashuyun.cn


<!-- 参考信息 -->