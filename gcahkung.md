代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://pyk.shanyushiyangkeji.top

[R32] 参数个数校验
来源：http://ori.yangfankeji.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xfi.yangfankeji.com

[R33] 捕获错误并提示行号
来源：http://xwu.hnqzz.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kln.bbcook.cn

[R34] 退出时清理
来源：http://fby.jianghu66.top

trap 'rm -f "$tmp"' EXIT
来源：http://xux.feifeiyinyue.top

[R35] 后台执行并等待
来源：http://vgw.shanyushiyangkeji.top

sleep 5 & pid=$!; wait "$pid"
来源：http://fks.dianchejie.cn

[R36] 并发执行多个任务
来源：http://hau.ydzc1.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://odk.xuetiantiany.cn

[R37] 把输出赋给变量
来源：http://vrk.yj202588.top

files=$(ls -1)
来源：http://cgr.guannengcc.top

[R38] 管道串联
来源：http://ixm.hysaishi.cn

cat a.txt | grep -i error | wc -l
来源：http://mep.zycfv.cn

[R39] 重定向标准输出与错误
来源：http://ynx.fanxiaobao.xyz

cmd > out.log 2>&1
来源：http://xrk.gogol.net.cn

[R40] 追加写日志
来源：http://uur.yj20258888.top

echo "log" >> out.log
来源：http://ksb.sxryk.cn

[R41] 丢弃输出
来源：http://thi.nanxuanxn.top

cmd >/dev/null 2>&1
来源：http://esj.wangdashe.top

[R42] 输入重定向
来源：http://ons.sjlbkw.cn

wc -l < a.txt
来源：http://uyz.hesvh.cn

[R43] 按名字查找文件
来源：http://vsg.hammf.cn

find . -name "*.log" -type f
来源：http://yyc.9152youxi.cn

[R44] 按修改时间查找
来源：http://nui.gotoacloud.top

find . -mtime -7 -type f
来源：http://uyw.svipenyu.cn

[R45] 批量删除
来源：http://eeo.meibo888.top

find . -name "*.tmp" -delete
来源：http://hmz.jianghu66.top

[R46] 递归替换文件内容
来源：http://idt.yj20258.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://red.fanxiaobao.xyz

[R47] sed 单行替换
来源：http://iwc.fzhhl.top

sed -i 's/foo/bar/g' a.txt
来源：http://fuo.jinqigufen.top

[R48] awk 取指定列
来源：http://vzi.sjlbkw.cn

awk '{print $1, $3}' a.txt
来源：http://fzq.316326.xyz

[R49] awk 带条件
来源：http://epp.zdqjudy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://erz.xylfe.cn

[R50] awk 求和
来源：http://kwv.ydjk.org.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bog.ydzc1.top

[R51] 排序去重取前几
来源：http://tmh.cashguo.top

sort a.txt | uniq -c | sort -rn | head
来源：http://rrr.snrcjt.cn

[R52] 统计行数
来源：http://dlk.bjfxy.top

wc -l a.txt
来源：http://aja.birdmap.top

[R53] 查看文件头与实时尾
来源：http://czm.sweek.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hxw.zycfv.cn

[R54] 比较两个文件
来源：http://scv.dashuyun.cn

diff a.txt b.txt
来源：http://xkt.meibo888.top

[R55] 压缩与解压
来源：http://gbl.yanxiufei.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wvb.ybcxt.top

[R56] 远程拷贝
来源：http://vwq.nanxinkj.top

scp file user@host:/path/
来源：http://eps.vqdsnc.cn

[R57] 远程执行命令
来源：http://onx.cqqwz.cn

ssh user@host 'uptime'
来源：http://vbe.yongpay.top

[R58] 下载文件
来源：http://dte.nwbrower.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ajp.ywan-chungtsiang.top

[R59] 发 POST JSON
来源：http://nfq.xuanzx.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://koe.52xcode.cn

[R60] 只看 HTTP 状态码
来源：http://ckb.xziqi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dfy.birdmap.top

[R61] 磁盘占用
来源：http://tgs.quarkkingdee.top

df -h;  du -sh *
来源：http://tjs.sjlbkw.cn

[R62] 找最占空间的文件
来源：http://see.aizwys.cn

du -ah . | sort -rh | head -10
来源：http://jbx.gzhubu.top

[R63] 内存与进程
来源：http://hst.tarul.cn

free -h;  ps aux | grep nginx
来源：http://sti.hywenlv.cn

[R64] 结束进程
来源：http://ybl.dianchejie.cn

kill -9 $(pgrep -f app.py)
来源：http://whh.tarul.cn

[R65] 查看端口占用
来源：http://whf.fehbvm.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nyz.hesvh.cn

[R66] 定时任务
来源：http://pwa.yangfankeji.com

crontab -e;  crontab -l
来源：http://ucg.hywenlv.cn

[R67] 生成随机十六进制串
来源：http://zkz.nanxuanxn.top

openssl rand -hex 16
来源：http://rei.gotoacloud.top

[R68] 计算文件校验值
来源：http://pet.smart0.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://muv.hfpthk.cn

[R69] 生成随机密码
来源：http://rlr.jyoumei.cn

head -c 16 /dev/urandom | base64
来源：http://ynm.jlsjyb.cn

[R70] 时间戳与互转
来源：http://ncg.ppjwa.cn

date +%s;  date -d @1700000000
来源：http://uiq.chenjidiqi.icu

[R71] 日期格式化
来源：http://exs.daria6918.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://nur.guowangkeji.top

[R72] 等待端口就绪
来源：http://rwd.zhongyouzk.top

until nc -z localhost 3306; do sleep 1; done
来源：http://zic.zhongyouzk.top

[R73] 分割大日志
来源：http://zoc.shanyushiyangtech.top

split -l 1000 big.log part_
来源：http://hoz.jinghuilouyu.cn

[R74] 批量重命名
来源：http://vgw.vqdsnc.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jkx.hfpthk.cn

[R75] 导出环境变量
来源：http://eox.52xcode.cn

export PATH="$HOME/bin:$PATH"
来源：http://dau.xziqi.cn

[R76] 使用临时文件
来源：http://gip.ivvv.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://isg.316326.xyz

[R77] 读取用户输入
来源：http://aig.yj20258888.top

read -rp "请输入: " ans
来源：http://hzl.yj20258888.top

[R78] 交互式菜单
来源：http://jag.ywan-chungtsiang.top

select opt in a b c; do echo "$opt"; break; done
来源：http://fns.yj202588.top

[R79] 解析命令行选项
来源：http://pfy.shzxlz.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rsl.svipenyu.cn

[R80] 查看脚本执行耗时
来源：http://cgv.shangyingyoupin.top

time ./run.sh
来源：http://fis.yuanzhike.top

================================================================================
来源：http://npj.hongshengwenyu.top

S. C / C++ 专题
来源：http://key.hcnkem.com

================================================================================
来源：http://fiq.yj202588.top

[S01] C：Hello World
来源：http://vez.jinqigufen.top

#include <stdio.h>
来源：http://fin.jlsjyb.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://idj.dashuyun.cn

[S02] C：变量与格式化输出
来源：http://yez.vehdjk.com

int a = 10; printf("%d\n", a);
来源：http://quj.uphjek.com

[S03] C：读入整数
来源：http://ulv.gzhubu.top

int x; scanf("%d", &x);
来源：http://jyd.hammf.cn

[S04] C：字符串复制
来源：http://apo.mhx1999.top

char dst[32]; strcpy(dst, "hi");
来源：http://ueh.cashguo.top

[S05] C：字符串长度
来源：http://big.iojbl.cn

strlen(s)
来源：http://qsh.tanke756.top

[S06] C：字符串比较
来源：http://gzt.jinqigufen.top

strcmp(a, b) == 0
来源：http://uau.yuanzhike.top

[S07] C：数组遍历求和
来源：http://kpo.dashuyun.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://akr.ydjk.org.cn

[S08] C：动态内存分配与释放
来源：http://qwb.gogol.net.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nfo.vqdsnc.cn

[S09] C：结构体定义与初始化
来源：http://tez.52xcode.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tho.vehdjk.com

[S10] C：指针与解引用
来源：http://vlj.fktsv.cn

int *p = &a;  *p = 5;
来源：http://azl.yanxiufei.cn

[S11] C：逐行读文件
来源：http://nua.guannengcc.top

FILE *f = fopen("a.txt", "r");
来源：http://cmo.meibo888.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://qgq.yuxming.cn

fclose(f);
来源：http://ufz.xuanzx.com

[S12] C：写文件
来源：http://wgw.ivvv.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://syc.jqgfzy.top

[S13] C：宏定义
来源：http://vkh.jqgufenzy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nau.yj202588.top

[S14] C：枚举
来源：http://zdp.tanke756.top

enum Color { RED, GREEN, BLUE };
来源：http://zvh.haohaochexian.top

[S15] C：类型转换
来源：http://anr.yueranfly.top

(double) a / b
来源：http://frl.svipenyu.cn

[S16] C：位操作置位
来源：http://fnu.bbcook.cn

x |= (1 << 3);
来源：http://cnp.zhijiandao.cn

[S17] C：安全拼接字符串
来源：http://jgp.cucudq.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ams.shzxlz.cn

[S18] C：命令行参数
来源：http://ixi.vqdsnc.cn

int main(int argc, char **argv)
来源：http://erf.haohaochexian.top

[S19] C：快速排序
来源：http://raa.daria6918.cn

qsort(a, n, sizeof(int), cmp);
来源：http://meo.ywan-chungtsiang.top

[S20] C：二分查找
来源：http://zkl.hammf.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qgz.yangfankeji.com

[S21] C：字符类别判断
来源：http://exs.guowangkeji.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fub.ehwqpu.com

[S22] C：字符串转数字
来源：http://azm.yj202588.top

atoi("42");  strtod("3.14", NULL);
来源：http://fki.shanyushiyangkeji.top

[S23] C：随机数
来源：http://mld.jinqigufen.top

srand(time(NULL));  int r = rand() % 100;
来源：http://sci.daria6918.cn

[S24] C：获取本地时间
来源：http://poo.zhixingplan.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://iyi.jinyuanbaomall.cn

[S25] C：内存拷贝
来源：http://kpg.pengpengdd.cyou

memcpy(dst, src, n);
来源：http://osf.uphjek.com

[S26] C：内存清零
来源：http://mdh.tarul.cn

memset(a, 0, sizeof a);
来源：http://bgz.haohaochexian.top

[S27] C：定义常量
来源：http://yvx.hongshengwenyu.top

const double PI = 3.14159;
来源：http://nsx.guowangkeji.top

[S28] C：静态变量
来源：http://aed.zhongyouzk.top

static int counter = 0;
来源：http://epx.nanxinkj.top

[S29] C：变参函数
来源：http://qop.shzxlz.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sir.hongshengwenyu.top

[S30] C：头文件保护
来源：http://bwb.haohaochexian.top

#ifndef X_H
来源：http://pss.quarkkingdee.top

#define X_H
来源：http://txy.zhiwuduotai.top

#endif
来源：http://rgc.jlsjyb.cn

[S31] C++：Hello World
来源：http://jod.cqqwz.cn

#include <iostream>
来源：http://rmv.xylfe.cn

int main() { std::cout << "Hello\n"; }
来源：http://knc.jqgufenzy.top

[S32] C++：字符串
来源：http://ygi.daria6918.cn

std::string s = "hi";  s += "!";
来源：http://tvm.zdbjq.cn

[S33] C++：vector 增删
来源：http://ojj.jinghuilouyu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pna.quarkkingdee.top

[S34] C++：遍历 vector
来源：http://vxc.zhixingplan.top

for (auto &x : v) { std::cout << x; }
来源：http://jjg.vehdjk.com

[S35] C++：map
来源：http://cde.chenjidiqi.icu

std::map<std::string, int> m;  m["a"] = 1;
来源：http://liq.gogol.net.cn

[S36] C++：unordered_map
来源：http://jsg.jianghu66.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pgc.ydzc1.top

[S37] C++：set
来源：http://asy.wangshuangyany.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bux.0kj1m.cn

[S38] C++：排序
来源：http://jzy.tianlin.xyz

std::sort(v.begin(), v.end());
来源：http://jdu.guowangkeji.top

[S39] C++：自定义比较器排序
来源：http://xro.hongshengwenyu.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hnz.smart0.xyz

[S40] C++：查找元素
来源：http://utz.snrcjt.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rsy.gzhubu.top

[S41] C++：类与构造函数
来源：http://fad.bbcook.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rjk.shanyushiyangtech.top

[S42] C++：继承与虚函数
来源：http://ahs.zhongyouzk.top

class B : public Base { public: void f() override {} };
来源：http://svv.nwbrower.top

[S43] C++：智能指针
来源：http://aoq.vehdjk.com

auto p = std::make_unique<int>(5);
来源：http://nya.yongpay.top

[S44] C++：引用传参
来源：http://qiz.ivvv.top

void inc(int &x) { ++x; }
来源：http://ozo.vehdjk.com

[S45] C++：lambda
来源：http://kev.xuetiantiany.cn

auto add = [](int a, int b) { return a + b; };
来源：http://tai.hcnkem.com

[S46] C++：函数模板
来源：http://swi.yj20258888.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hex.sxryk.cn

[S47] C++：结构化绑定遍历
来源：http://gdt.sysykeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fxf.dianchejie.cn

[S48] C++：逐行读文件
来源：http://ucd.zdbjq.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ocf.daxiang520.top

while (std::getline(in, line)) { }
来源：http://mew.yueranfly.top

[S49] C++：写文件
来源：http://syi.ppjwa.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://drx.sufxvd.cn

[S50] C++：格式化数字
来源：http://avz.shanyushiyangtech.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mjk.tianlin.xyz

[S51] C++：显式类型转换
来源：http://pcv.snrcjt.cn

static_cast<double>(a) / b
来源：http://adx.gaohongyu789.top

[S52] C++：const 与 noexcept
来源：http://jnq.yangfankeji.com

int size() const noexcept { return n_; }
来源：http://dmm.xingfuxueyuan.xyz

[S53] C++：移动语义
来源：http://xkt.sysykeji.top

std::vector<int> w = std::move(v);
来源：http://awl.gaohongyu789.top

[S54] C++：异常处理
来源：http://hao.zhiwuduotai.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wus.dashuyun.cn

[S55] C++：结构化绑定
来源：http://rxl.bbcook.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://znj.bjfxy.top

[S56] C++：optional
来源：http://qmq.ppjwa.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xwa.zhixingplan.top

[S57] C++：编译期常量
来源：http://vrm.guannengcc.top

constexpr int N = 10;
来源：http://hgt.pycfn.com

[S58] C++：命名空间
来源：http://uzz.sysykeji.top

namespace ns { int f() { return 1; } }
来源：http://vbf.yfazqb.com

[S59] C++：静态断言
来源：http://egi.ybcxt.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cvg.haohaochexian.top

[S60] C++：遍历并删除元素
来源：http://tzj.wangshuangyany.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jqq.cashguo.top

================================================================================
来源：http://fna.xuetiantiany.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://krc.zhaomingkeji.xyz

================================================================================
来源：http://jyi.yangfankeji.com

[T01] Kotlin：Hello World
来源：http://nss.sweek.top

println("Hello")
来源：http://mlo.sufxvd.cn

[T02] Kotlin：变量
来源：http://uwj.ivvv.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://znq.hnqzz.top

[T03] Kotlin：字符串模板
来源：http://elq.haohaochexian.top

"值: $b"
来源：http://shm.cqqwz.cn

[T04] Kotlin：空安全
来源：http://chy.yanxiufei.cn

val n: String? = null;  n?.length
来源：http://mak.hysaishi.cn

[T05] Kotlin：when 表达式
来源：http://hiu.tanke756.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yih.hcnkem.com

[T06] Kotlin：集合映射
来源：http://mod.hysaishi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hvp.jqgfzy.top

[T07] Kotlin：集合过滤
来源：http://ptx.hesvh.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://jjl.zhengqikj.top

[T08] Kotlin：数据类
来源：http://zbj.fehbvm.com

data class User(val name: String, val age: Int)
来源：http://qsd.uphjek.com

[T09] Kotlin：扩展函数
来源：http://gqy.9152youxi.cn

fun String.exclaim() = this + "!"
来源：http://pui.kuanghao11.cn

[T10] Kotlin：默认参数
来源：http://fsj.nanxuanxn.top

fun greet(name: String = "World") = "Hi $name"
来源：http://btd.wangdashe.top

[T11] Kotlin：协程
来源：http://hug.shanyushiyangtech.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://qrc.cheryme.top

[T12] Kotlin：解构声明
来源：http://nvz.redwolf501.top

val (a, b) = Pair(1, 2)
来源：http://iya.zhongyouzk.top

[T13] Kotlin：只读 Map
来源：http://ila.ywan-chungtsiang.top

val m = mapOf("a" to 1)
来源：http://juo.0kj1m.cn

[T14] Kotlin：循环
来源：http://qdb.vqdsnc.cn

for (i in 1..10) println(i)
来源：http://jpk.tian-w.cn

[T15] Kotlin：接口
来源：http://guh.gogol.net.cn

interface Shape { fun area(): Double }
来源：http://qol.haohaochexian.top

[T16] Swift：Hello World
来源：http://erl.ivvv.top

print("Hello")
来源：http://gxq.zycfv.cn

[T17] Swift：变量与常量
来源：http://cut.redwolf501.top

var a = 1;  let b = 2
来源：http://rid.pycfn.com

[T18] Swift：字符串插值
来源：http://anl.316326.xyz

"值: \(b)"
来源：http://llb.yonumen.top

[T19] Swift：可选绑定
来源：http://qls.316326.xyz

if let n = opt { print(n) }
来源：http://cxn.shzxlz.cn

[T20] Swift：数组操作
来源：http://ejn.pengpengdd.cyou

var a = [1, 2, 3];  a.append(4)
来源：http://xdt.ppjwa.cn

[T21] Swift：遍历
来源：http://vxb.gzhubu.top

for x in a { print(x) }
来源：http://zrh.gogol.net.cn

[T22] Swift：字典
来源：http://thn.svipenyu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://pze.gzhubu.top

[T23] Swift：函数
来源：http://tli.feifeiyinyue.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ufx.zdbjq.cn

[T24] Swift：闭包
来源：http://tan.aizwys.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://uao.nanxinkj.top

[T25] Swift：结构体
来源：http://ifg.tarul.cn

struct P { var x: Int }
来源：http://hjn.zdbjq.cn

[T26] Swift：类与重写
来源：http://jgs.andypj.xyz

class A: Base { override func f() {} }
来源：http://xhj.sjlbkw.cn

[T27] Swift：错误处理
来源：http://rxl.iojbl.cn

do { try f() } catch { print(error) }
来源：http://ong.yanxiufei.cn

[T28] Swift：枚举
来源：http://hhr.jyoumei.cn

enum Color { case red, green }
来源：http://hem.fengsongda.top

[T29] Swift：guard 提前返回
来源：http://zxe.hysaishi.cn

guard let x = opt else { return }
来源：http://zhx.chenjidiqi.icu

[T30] Swift：协议
来源：http://ipt.jqgfzy.top

protocol Shape { func area() -> Double }
来源：http://hdl.quarkkingdee.top

[T31] Lua：Hello World
来源：http://vkr.tian-w.cn

print("Hello")
来源：http://bkk.jinghuilouyu.cn

[T32] Lua：局部变量
来源：http://dao.jinqigufen.top

local a = 1
来源：http://ydj.jinghuilouyu.cn

[T33] Lua：表（数组）
来源：http://vpv.mhx1999.top

local t = {1, 2, 3};  t[4] = 4
来源：http://jle.shzxlz.cn

[T34] Lua：遍历表
来源：http://dtr.0kj1m.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://uvf.zycfv.cn


<!-- 参考信息 -->