代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cmb.chenzaomai.com

[R24] 大小写转换
来源：http://ytk.hesvh.cn

echo "${s^^}"; echo "${s,,}"
来源：http://mxi.jiagoushi.top

[R25] 去后缀 / 去前缀
来源：http://xfo.jyoumei.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://rbe.ctjpmb.com

[R26] 命令替换
来源：http://lui.shangyingyoupin.top

now=$(date +%F); echo "$now"
来源：http://xkk.fengsongda.top

[R27] 算术展开
来源：http://bih.wangdashe.top

echo $((1 + 2 * 3))
来源：http://jjs.vehdjk.com

[R28] 浮点运算
来源：http://xmz.xuetiantiany.cn

echo "scale=2; 10/3" | bc
来源：http://aff.mhx1999.top

[R29] 定义函数
来源：http://tps.fengsongda.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xeo.gogol.net.cn

[R30] 函数返回状态码
来源：http://mqw.fzhhl.top

f() { return 0; }; f || echo "失败了"
来源：http://yca.wangdashe.top

[R31] 局部变量
来源：http://mbq.hnxiangtu.top

f() { local x=1; echo "$x"; }
来源：http://sbw.pengpengdd.cyou

[R32] 参数个数校验
来源：http://fid.shanyushiyangkeji.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ywt.jinghuilouyu.cn

[R33] 捕获错误并提示行号
来源：http://mpg.xuetiantiany.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zyg.ydjk.org.cn

[R34] 退出时清理
来源：http://jzr.hcnkem.com

trap 'rm -f "$tmp"' EXIT
来源：http://vbs.fehbvm.com

[R35] 后台执行并等待
来源：http://srw.chenjidiqi.icu

sleep 5 & pid=$!; wait "$pid"
来源：http://lay.daria6918.cn

[R36] 并发执行多个任务
来源：http://jsz.hfpthk.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mfi.ehwqpu.com

[R37] 把输出赋给变量
来源：http://kyo.nwbrower.top

files=$(ls -1)
来源：http://ldp.birdmap.top

[R38] 管道串联
来源：http://pka.tian-w.cn

cat a.txt | grep -i error | wc -l
来源：http://ign.dianchejie.cn

[R39] 重定向标准输出与错误
来源：http://lea.tanke756.top

cmd > out.log 2>&1
来源：http://noc.zhongyouzk.top

[R40] 追加写日志
来源：http://rxq.ybcxt.top

echo "log" >> out.log
来源：http://vsj.9152youxi.cn

[R41] 丢弃输出
来源：http://nzx.gaohongyu789.top

cmd >/dev/null 2>&1
来源：http://rtk.jinqigufen.top

[R42] 输入重定向
来源：http://pxj.aibaodan.cn

wc -l < a.txt
来源：http://jyc.quarkkingdee.top

[R43] 按名字查找文件
来源：http://uou.zdbjq.cn

find . -name "*.log" -type f
来源：http://tyq.yueranfly.top

[R44] 按修改时间查找
来源：http://mso.vehdjk.com

find . -mtime -7 -type f
来源：http://wyo.fehbvm.com

[R45] 批量删除
来源：http://hqs.yj20258888.top

find . -name "*.tmp" -delete
来源：http://ndk.cqqwz.cn

[R46] 递归替换文件内容
来源：http://ljp.zhaomingkeji.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gjx.jinqigufen.top

[R47] sed 单行替换
来源：http://rhd.chenjidiqi.icu

sed -i 's/foo/bar/g' a.txt
来源：http://slq.guannengcc.top

[R48] awk 取指定列
来源：http://qvt.316326.xyz

awk '{print $1, $3}' a.txt
来源：http://obo.shanyushiyangkeji.top

[R49] awk 带条件
来源：http://hwx.yueranfly.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mxp.zhoulong.xyz

[R50] awk 求和
来源：http://amv.tarul.cn

awk '{s += $2} END {print s}' a.txt
来源：http://now.nanxinkj.top

[R51] 排序去重取前几
来源：http://bpf.jiagoushi.top

sort a.txt | uniq -c | sort -rn | head
来源：http://csv.guannengcc.top

[R52] 统计行数
来源：http://kym.jqgfzy.top

wc -l a.txt
来源：http://yrh.zhixingplan.top

[R53] 查看文件头与实时尾
来源：http://fby.yvedp.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kuo.hfpthk.cn

[R54] 比较两个文件
来源：http://oak.gogol.net.cn

diff a.txt b.txt
来源：http://snb.pengpengdd.cyou

[R55] 压缩与解压
来源：http://kum.cucudq.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ffg.haohaochexian.top

[R56] 远程拷贝
来源：http://cir.0kj1m.cn

scp file user@host:/path/
来源：http://yst.yfazqb.com

[R57] 远程执行命令
来源：http://dqh.pycfn.com

ssh user@host 'uptime'
来源：http://zks.gogol.net.cn

[R58] 下载文件
来源：http://phe.jinghuilouyu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rex.316326.xyz

[R59] 发 POST JSON
来源：http://bid.wangdashe.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pjc.quarkkingdee.top

[R60] 只看 HTTP 状态码
来源：http://cpp.jqgfzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cbt.yj20258.top

[R61] 磁盘占用
来源：http://zjy.xziqi.cn

df -h;  du -sh *
来源：http://dcs.jinyuanbaomall.cn

[R62] 找最占空间的文件
来源：http://krh.tanke756.top

du -ah . | sort -rh | head -10
来源：http://rgh.sxryk.cn

[R63] 内存与进程
来源：http://fte.sufxvd.cn

free -h;  ps aux | grep nginx
来源：http://mij.cqqwz.cn

[R64] 结束进程
来源：http://her.jinqigfzy.top

kill -9 $(pgrep -f app.py)
来源：http://nxy.xuetiantiany.cn

[R65] 查看端口占用
来源：http://wcu.chenjidiqi.icu

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://akp.vehdjk.com

[R66] 定时任务
来源：http://gmg.ywan-chungtsiang.top

crontab -e;  crontab -l
来源：http://swq.jiagoushi.top

[R67] 生成随机十六进制串
来源：http://jsf.andypj.xyz

openssl rand -hex 16
来源：http://ybn.ehwqpu.com

[R68] 计算文件校验值
来源：http://ayb.mhx1999.top

sha256sum a.txt;  md5sum a.txt
来源：http://ote.hnxiangtu.top

[R69] 生成随机密码
来源：http://fab.sxryk.cn

head -c 16 /dev/urandom | base64
来源：http://orh.yangfankeji.com

[R70] 时间戳与互转
来源：http://kqz.xuetiantiany.cn

date +%s;  date -d @1700000000
来源：http://xod.dashuyun.cn

[R71] 日期格式化
来源：http://wkr.cqqwz.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://uwt.hongshengwenyu.top

[R72] 等待端口就绪
来源：http://wyi.bjfxy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ysu.pycfn.com

[R73] 分割大日志
来源：http://rqv.snrcjt.cn

split -l 1000 big.log part_
来源：http://fve.shangyingyoupin.top

[R74] 批量重命名
来源：http://ely.hfpthk.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://uce.ydjk.org.cn

[R75] 导出环境变量
来源：http://lvd.fzhhl.top

export PATH="$HOME/bin:$PATH"
来源：http://hhg.ywan-chungtsiang.top

[R76] 使用临时文件
来源：http://gdi.shanyushiyangkeji.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cix.feifeiyinyue.top

[R77] 读取用户输入
来源：http://maj.pycfn.com

read -rp "请输入: " ans
来源：http://tyn.hesvh.cn

[R78] 交互式菜单
来源：http://uyd.wangdashe.top

select opt in a b c; do echo "$opt"; break; done
来源：http://yvk.ydjk.org.cn

[R79] 解析命令行选项
来源：http://aki.ywan-chungtsiang.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dbn.hesvh.cn

[R80] 查看脚本执行耗时
来源：http://bnj.cheryme.top

time ./run.sh
来源：http://lnd.jinqigfzy.top

================================================================================
来源：http://zbo.fktsv.cn

S. C / C++ 专题
来源：http://imb.fanxiaobao.xyz

================================================================================
来源：http://oqz.52xcode.cn

[S01] C：Hello World
来源：http://fqb.iojbl.cn

#include <stdio.h>
来源：http://ndn.bjfxy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://grm.yangfankeji.com

[S02] C：变量与格式化输出
来源：http://otu.fktsv.cn

int a = 10; printf("%d\n", a);
来源：http://oii.guowangkeji.top

[S03] C：读入整数
来源：http://slp.jqgufenzy.top

int x; scanf("%d", &x);
来源：http://umq.tanke756.top

[S04] C：字符串复制
来源：http://tsz.zhijiandao.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wak.jianghu66.top

[S05] C：字符串长度
来源：http://lou.gzhubu.top

strlen(s)
来源：http://sdt.zhengqikj.top

[S06] C：字符串比较
来源：http://ypa.pengpengdd.cyou

strcmp(a, b) == 0
来源：http://nyn.zhaomingkeji.xyz

[S07] C：数组遍历求和
来源：http://sib.jinyuanbaomall.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zjh.zdbjq.cn

[S08] C：动态内存分配与释放
来源：http://xfy.daria6918.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://har.yj202588.top

[S09] C：结构体定义与初始化
来源：http://uvr.yvedp.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rlw.xinyue.icu

[S10] C：指针与解引用
来源：http://tej.hongshengwenyu.top

int *p = &a;  *p = 5;
来源：http://kxs.daxiang520.top

[S11] C：逐行读文件
来源：http://hlb.cdnleiting.top

FILE *f = fopen("a.txt", "r");
来源：http://tct.fzhhl.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ymq.jyoumei.cn

fclose(f);
来源：http://usm.xylfe.cn

[S12] C：写文件
来源：http://gzh.yj20258888.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wte.meibo888.top

[S13] C：宏定义
来源：http://fxl.dashuyun.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nvl.zhixingplan.top

[S14] C：枚举
来源：http://bdu.zhoulong.xyz

enum Color { RED, GREEN, BLUE };
来源：http://coy.jyoumei.cn

[S15] C：类型转换
来源：http://hug.tian-w.cn

(double) a / b
来源：http://xtg.cashguo.top

[S16] C：位操作置位
来源：http://hrl.fzhhl.top

x |= (1 << 3);
来源：http://aqw.cqqwz.cn

[S17] C：安全拼接字符串
来源：http://isg.sufxvd.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://smo.hysaishi.cn

[S18] C：命令行参数
来源：http://pjg.svipenyu.cn

int main(int argc, char **argv)
来源：http://cqk.haohaochexian.top

[S19] C：快速排序
来源：http://nxc.zhongyouzk.top

qsort(a, n, sizeof(int), cmp);
来源：http://lnh.ydjk.org.cn

[S20] C：二分查找
来源：http://jer.zdqjudy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fym.havefunace.top

[S21] C：字符类别判断
来源：http://fng.dianchejie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rbu.iojbl.cn

[S22] C：字符串转数字
来源：http://xhb.daxiang520.top

atoi("42");  strtod("3.14", NULL);
来源：http://snq.shanyushiyangtech.top

[S23] C：随机数
来源：http://pzl.bjfxy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://glf.shangyingyoupin.top

[S24] C：获取本地时间
来源：http://bhp.jyoumei.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://okz.kuanghao11.cn

[S25] C：内存拷贝
来源：http://fun.jiagoushi.top

memcpy(dst, src, n);
来源：http://waq.gogol.net.cn

[S26] C：内存清零
来源：http://qlg.feifeiyinyue.top

memset(a, 0, sizeof a);
来源：http://pkt.zdqjudy.top

[S27] C：定义常量
来源：http://qzq.zhoulong.xyz

const double PI = 3.14159;
来源：http://awb.dashuyun.cn

[S28] C：静态变量
来源：http://lbh.xylfe.cn

static int counter = 0;
来源：http://kay.ctjpmb.com

[S29] C：变参函数
来源：http://fcr.cucudq.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lhn.fengsongda.top

[S30] C：头文件保护
来源：http://hbn.jiagoushi.top

#ifndef X_H
来源：http://tjb.yongpay.top

#define X_H
来源：http://bxt.ivvv.top

#endif
来源：http://yix.fanxiaobao.xyz

[S31] C++：Hello World
来源：http://kvp.zdqjudy.top

#include <iostream>
来源：http://jut.gogol.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://dag.gotoacloud.top

[S32] C++：字符串
来源：http://amc.tianlin.xyz

std::string s = "hi";  s += "!";
来源：http://pny.sysykeji.top

[S33] C++：vector 增删
来源：http://iyj.smart0.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ojg.hesvh.cn

[S34] C++：遍历 vector
来源：http://qge.guannengcc.top

for (auto &x : v) { std::cout << x; }
来源：http://oad.pycfn.com

[S35] C++：map
来源：http://jaz.mhx1999.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bow.xinyue.icu

[S36] C++：unordered_map
来源：http://ofc.shanyushiyangtech.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uho.yueranfly.top

[S37] C++：set
来源：http://zyb.shanyushiyangtech.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://syd.xinyue.icu

[S38] C++：排序
来源：http://ils.jyoumei.cn

std::sort(v.begin(), v.end());
来源：http://dde.zhiwuduotai.top

[S39] C++：自定义比较器排序
来源：http://xhd.hcnkem.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://faz.bbcook.cn

[S40] C++：查找元素
来源：http://lzk.iojbl.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ckt.yonumen.top

[S41] C++：类与构造函数
来源：http://agz.gogol.net.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://drl.sufxvd.cn

[S42] C++：继承与虚函数
来源：http://kke.dashuyun.cn

class B : public Base { public: void f() override {} };
来源：http://hhh.vehdjk.com

[S43] C++：智能指针
来源：http://rwj.ywan-chungtsiang.top

auto p = std::make_unique<int>(5);
来源：http://vxd.jqgufenzy.top

[S44] C++：引用传参
来源：http://lip.jinghuilouyu.cn

void inc(int &x) { ++x; }
来源：http://mgp.nwbrower.top

[S45] C++：lambda
来源：http://cke.dashuyun.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zhy.iojbl.cn

[S46] C++：函数模板
来源：http://ldw.shzxlz.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zaz.zhiwuduotai.top

[S47] C++：结构化绑定遍历
来源：http://oja.guowangkeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://uue.shanyushiyangkeji.top

[S48] C++：逐行读文件
来源：http://rjf.jqgufenzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://jyn.hnqzz.top

while (std::getline(in, line)) { }
来源：http://sms.shanyushiyangkeji.top

[S49] C++：写文件
来源：http://dqf.hysaishi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gcg.jyoumei.cn

[S50] C++：格式化数字
来源：http://xph.andypj.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cam.yj20258888.top

[S51] C++：显式类型转换
来源：http://kdp.vqdsnc.cn

static_cast<double>(a) / b
来源：http://sfc.guannengcc.top

[S52] C++：const 与 noexcept
来源：http://voz.xingfuxueyuan.xyz

int size() const noexcept { return n_; }
来源：http://duv.svipenyu.cn

[S53] C++：移动语义
来源：http://xzc.chenzaomai.com

std::vector<int> w = std::move(v);
来源：http://jnv.bbcook.cn

[S54] C++：异常处理
来源：http://nhl.feifeiyinyue.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vhr.jqgufenzy.top

[S55] C++：结构化绑定
来源：http://nfi.zhongyouzk.top

auto [a, b] = std::make_pair(1, 2);
来源：http://nzn.smart0.xyz

[S56] C++：optional
来源：http://wxe.316326.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nqb.gogol.net.cn

[S57] C++：编译期常量
来源：http://wlo.jinghuilouyu.cn

constexpr int N = 10;
来源：http://evy.shanyushiyangtech.top

[S58] C++：命名空间
来源：http://emp.hammf.cn

namespace ns { int f() { return 1; } }
来源：http://bws.hesvh.cn

[S59] C++：静态断言
来源：http://xsy.tian-w.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dxh.gotoacloud.top

[S60] C++：遍历并删除元素
来源：http://vct.vehdjk.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://eiz.mhx1999.top

================================================================================
来源：http://dzr.nanxinkj.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rcz.shanyushiyangtech.top

================================================================================
来源：http://tlr.yj20258888.top

[T01] Kotlin：Hello World
来源：http://zvb.nanxuanxn.top

println("Hello")
来源：http://soe.sysykeji.top

[T02] Kotlin：变量
来源：http://hrr.shzxlz.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://oiq.ivvv.top

[T03] Kotlin：字符串模板
来源：http://cbp.xinyue.icu

"值: $b"
来源：http://gsc.zhoulong.xyz

[T04] Kotlin：空安全
来源：http://xon.gzhubu.top

val n: String? = null;  n?.length
来源：http://qqq.316326.xyz

[T05] Kotlin：when 表达式
来源：http://gcv.zhongyouzk.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wis.jqgfzy.top

[T06] Kotlin：集合映射
来源：http://dpb.jlsjyb.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://prl.pengpengdd.cyou

[T07] Kotlin：集合过滤
来源：http://qtv.vehdjk.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://zgd.fehbvm.com

[T08] Kotlin：数据类
来源：http://vmk.cashguo.top

data class User(val name: String, val age: Int)
来源：http://qog.fktsv.cn

[T09] Kotlin：扩展函数
来源：http://qmg.havefunace.top

fun String.exclaim() = this + "!"
来源：http://rmi.ydjk.org.cn

[T10] Kotlin：默认参数
来源：http://atb.hywenlv.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ztv.zhixingplan.top

[T11] Kotlin：协程
来源：http://vlu.zhiwuduotai.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://gpn.haohaochexian.top

[T12] Kotlin：解构声明
来源：http://tly.jinghuilouyu.cn

val (a, b) = Pair(1, 2)
来源：http://vgz.sysykeji.top

[T13] Kotlin：只读 Map
来源：http://idw.xuanzx.com

val m = mapOf("a" to 1)
来源：http://cth.daria6918.cn

[T14] Kotlin：循环
来源：http://rsv.snrcjt.cn

for (i in 1..10) println(i)
来源：http://huz.fengsongda.top

[T15] Kotlin：接口
来源：http://der.jqgufenzy.top

interface Shape { fun area(): Double }
来源：http://zcu.andypj.xyz

[T16] Swift：Hello World
来源：http://yyj.aizwys.cn

print("Hello")
来源：http://bjs.yueranfly.top

[T17] Swift：变量与常量
来源：http://hvv.tian-w.cn

var a = 1;  let b = 2
来源：http://grs.xinyue.icu

[T18] Swift：字符串插值
来源：http://ivt.yanxiufei.cn

"值: \(b)"
来源：http://mgz.shangyingyoupin.top

[T19] Swift：可选绑定
来源：http://bwe.quarkkingdee.top

if let n = opt { print(n) }
来源：http://qyl.hnqzz.top

[T20] Swift：数组操作
来源：http://qem.bbcook.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ngb.wangdashe.top

[T21] Swift：遍历
来源：http://ktn.iojbl.cn

for x in a { print(x) }
来源：http://sjp.zhoulong.xyz

[T22] Swift：字典
来源：http://yds.shuidangran.top

var d = ["a": 1];  d["b"] = 2
来源：http://gkp.cqqwz.cn

[T23] Swift：函数
来源：http://cbh.havefunace.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bbp.ppjwa.cn

[T24] Swift：闭包
来源：http://rrq.dianchejie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qpb.ivvv.top

[T25] Swift：结构体
来源：http://kxp.zdbjq.cn

struct P { var x: Int }
来源：http://uyb.yonumen.top

[T26] Swift：类与重写
来源：http://dpk.bjfxy.top

class A: Base { override func f() {} }
来源：http://zyn.sjlbkw.cn


<!-- 参考信息 -->