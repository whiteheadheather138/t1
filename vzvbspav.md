代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://gvb.zdbjq.cn

[R36] 并发执行多个任务
来源：http://vsj.dianchejie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ebu.yj20258.top

[R37] 把输出赋给变量
来源：http://clb.jianghu66.top

files=$(ls -1)
来源：http://oda.fzhhl.top

[R38] 管道串联
来源：http://axb.iojbl.cn

cat a.txt | grep -i error | wc -l
来源：http://tev.wangdashe.top

[R39] 重定向标准输出与错误
来源：http://mrp.vehdjk.com

cmd > out.log 2>&1
来源：http://wzf.dashuyun.cn

[R40] 追加写日志
来源：http://mcp.gotoacloud.top

echo "log" >> out.log
来源：http://wby.fzhhl.top

[R41] 丢弃输出
来源：http://qkq.bjfxy.top

cmd >/dev/null 2>&1
来源：http://lox.kuanghao11.cn

[R42] 输入重定向
来源：http://ari.xinyue.icu

wc -l < a.txt
来源：http://ejn.redwolf501.top

[R43] 按名字查找文件
来源：http://oii.wangdashe.top

find . -name "*.log" -type f
来源：http://yvy.vqdsnc.cn

[R44] 按修改时间查找
来源：http://hwl.cheryme.top

find . -mtime -7 -type f
来源：http://cqq.shuidangran.top

[R45] 批量删除
来源：http://pth.xinyue.icu

find . -name "*.tmp" -delete
来源：http://afm.yj20258888.top

[R46] 递归替换文件内容
来源：http://fsk.jinghuilouyu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bho.ydzc1.top

[R47] sed 单行替换
来源：http://zcn.xuanzx.com

sed -i 's/foo/bar/g' a.txt
来源：http://kjf.chenjidiqi.icu

[R48] awk 取指定列
来源：http://etu.sjlbkw.cn

awk '{print $1, $3}' a.txt
来源：http://jvv.jinqigfzy.top

[R49] awk 带条件
来源：http://dfy.cdnleiting.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rdt.tarul.cn

[R50] awk 求和
来源：http://yqw.aizwys.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zzl.gogol.net.cn

[R51] 排序去重取前几
来源：http://cvb.zhengqikj.top

sort a.txt | uniq -c | sort -rn | head
来源：http://eoc.yueranfly.top

[R52] 统计行数
来源：http://fvp.fengsongda.top

wc -l a.txt
来源：http://ail.kuanghao11.cn

[R53] 查看文件头与实时尾
来源：http://eqz.hesvh.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jqk.gaohongyu789.top

[R54] 比较两个文件
来源：http://xlc.chenzaomai.com

diff a.txt b.txt
来源：http://whz.jyoumei.cn

[R55] 压缩与解压
来源：http://qkq.shanyushiyangtech.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zub.hywenlv.cn

[R56] 远程拷贝
来源：http://aam.yj20258.top

scp file user@host:/path/
来源：http://fbt.andypj.xyz

[R57] 远程执行命令
来源：http://hxw.jianghu66.top

ssh user@host 'uptime'
来源：http://wbf.hcnkem.com

[R58] 下载文件
来源：http://hct.jinqigufen.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yaw.tianlin.xyz

[R59] 发 POST JSON
来源：http://mem.iojbl.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bbm.yuxming.cn

[R60] 只看 HTTP 状态码
来源：http://jpm.gaohongyu789.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://aia.zhengqikj.top

[R61] 磁盘占用
来源：http://hib.svipenyu.cn

df -h;  du -sh *
来源：http://xtd.shuidangran.top

[R62] 找最占空间的文件
来源：http://cda.yj20258.top

du -ah . | sort -rh | head -10
来源：http://jhk.kuanghao11.cn

[R63] 内存与进程
来源：http://gjx.sufxvd.cn

free -h;  ps aux | grep nginx
来源：http://lrs.yj20258.top

[R64] 结束进程
来源：http://zgj.yvedp.cn

kill -9 $(pgrep -f app.py)
来源：http://zyo.andypj.xyz

[R65] 查看端口占用
来源：http://ciz.gotoacloud.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://smh.zhoulong.xyz

[R66] 定时任务
来源：http://qub.zhiwuduotai.top

crontab -e;  crontab -l
来源：http://tzv.hcnkem.com

[R67] 生成随机十六进制串
来源：http://dlb.gotoacloud.top

openssl rand -hex 16
来源：http://ukj.jiagoushi.top

[R68] 计算文件校验值
来源：http://ncf.nwbrower.top

sha256sum a.txt;  md5sum a.txt
来源：http://vmr.hfpthk.cn

[R69] 生成随机密码
来源：http://htg.hnqzz.top

head -c 16 /dev/urandom | base64
来源：http://jcu.tian-w.cn

[R70] 时间戳与互转
来源：http://fvp.gzhubu.top

date +%s;  date -d @1700000000
来源：http://qqd.zhiwuduotai.top

[R71] 日期格式化
来源：http://ygl.tanke756.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://htk.yueranfly.top

[R72] 等待端口就绪
来源：http://wty.iojbl.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dxv.dianchejie.cn

[R73] 分割大日志
来源：http://jda.ppjwa.cn

split -l 1000 big.log part_
来源：http://suu.daria6918.cn

[R74] 批量重命名
来源：http://whl.kuanghao11.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://drz.52xcode.cn

[R75] 导出环境变量
来源：http://xev.vqdsnc.cn

export PATH="$HOME/bin:$PATH"
来源：http://ttk.guowangkeji.top

[R76] 使用临时文件
来源：http://nxl.gzhubu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fvb.kuanghao11.cn

[R77] 读取用户输入
来源：http://zzo.fehbvm.com

read -rp "请输入: " ans
来源：http://pby.jinqigfzy.top

[R78] 交互式菜单
来源：http://bgn.xuanzx.com

select opt in a b c; do echo "$opt"; break; done
来源：http://kuw.zhiwuduotai.top

[R79] 解析命令行选项
来源：http://kfk.tanke756.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://htl.xylfe.cn

[R80] 查看脚本执行耗时
来源：http://ywy.jinqigufen.top

time ./run.sh
来源：http://gnf.ctjpmb.com

================================================================================
来源：http://fdq.hnxiangtu.top

S. C / C++ 专题
来源：http://jwg.ywan-chungtsiang.top

================================================================================
来源：http://xet.9152youxi.cn

[S01] C：Hello World
来源：http://sqv.fzhhl.top

#include <stdio.h>
来源：http://giw.pycfn.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://ymz.shuidangran.top

[S02] C：变量与格式化输出
来源：http://xna.ppjwa.cn

int a = 10; printf("%d\n", a);
来源：http://fyh.daria6918.cn

[S03] C：读入整数
来源：http://ukg.sysykeji.top

int x; scanf("%d", &x);
来源：http://abs.yfazqb.com

[S04] C：字符串复制
来源：http://phc.52xcode.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jyi.gogol.net.cn

[S05] C：字符串长度
来源：http://kpv.dashuyun.cn

strlen(s)
来源：http://dmd.redwolf501.top

[S06] C：字符串比较
来源：http://eum.meibo888.top

strcmp(a, b) == 0
来源：http://hpn.zhongyouzk.top

[S07] C：数组遍历求和
来源：http://ilv.hnxiangtu.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wwt.jinyuanbaomall.cn

[S08] C：动态内存分配与释放
来源：http://npa.epnwcf.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gkz.pengpengdd.cyou

[S09] C：结构体定义与初始化
来源：http://pnf.hesvh.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hen.dianchejie.cn

[S10] C：指针与解引用
来源：http://tkd.yangfankeji.com

int *p = &a;  *p = 5;
来源：http://gnn.vehdjk.com

[S11] C：逐行读文件
来源：http://ijd.tarul.cn

FILE *f = fopen("a.txt", "r");
来源：http://kse.svipenyu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zyz.havefunace.top

fclose(f);
来源：http://syu.jinghuilouyu.cn

[S12] C：写文件
来源：http://fqn.yj20258888.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://klr.ybcxt.top

[S13] C：宏定义
来源：http://arf.smart0.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pkq.jqgfzy.top

[S14] C：枚举
来源：http://owr.zhixingplan.top

enum Color { RED, GREEN, BLUE };
来源：http://xmq.cashguo.top

[S15] C：类型转换
来源：http://pgr.aizwys.cn

(double) a / b
来源：http://pgm.svipenyu.cn

[S16] C：位操作置位
来源：http://slh.redwolf501.top

x |= (1 << 3);
来源：http://glk.c1oappe.top

[S17] C：安全拼接字符串
来源：http://puv.zhiwuduotai.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hgo.jianghu66.top

[S18] C：命令行参数
来源：http://obb.ivvv.top

int main(int argc, char **argv)
来源：http://egf.sweek.top

[S19] C：快速排序
来源：http://xhk.fengsongda.top

qsort(a, n, sizeof(int), cmp);
来源：http://pqm.shzxlz.cn

[S20] C：二分查找
来源：http://hkj.fktsv.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zgt.snrcjt.cn

[S21] C：字符类别判断
来源：http://crp.fengsongda.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://egd.ehwqpu.com

[S22] C：字符串转数字
来源：http://kmf.jianghu66.top

atoi("42");  strtod("3.14", NULL);
来源：http://xur.jqgufenzy.top

[S23] C：随机数
来源：http://mff.hysaishi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://yja.guowangkeji.top

[S24] C：获取本地时间
来源：http://sar.mhx1999.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fiz.ydjk.org.cn

[S25] C：内存拷贝
来源：http://daw.fengsongda.top

memcpy(dst, src, n);
来源：http://jnb.hnqzz.top

[S26] C：内存清零
来源：http://jlt.zycfv.cn

memset(a, 0, sizeof a);
来源：http://lby.mhx1999.top

[S27] C：定义常量
来源：http://dee.tian-w.cn

const double PI = 3.14159;
来源：http://gri.tian-w.cn

[S28] C：静态变量
来源：http://gyu.chenzaomai.com

static int counter = 0;
来源：http://xwm.pycfn.com

[S29] C：变参函数
来源：http://alj.cdnleiting.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qfj.ybcxt.top

[S30] C：头文件保护
来源：http://jko.hysaishi.cn

#ifndef X_H
来源：http://tgu.dianchejie.cn

#define X_H
来源：http://vma.chenjidiqi.icu

#endif
来源：http://nds.sjlbkw.cn

[S31] C++：Hello World
来源：http://dve.zdqjudy.top

#include <iostream>
来源：http://lnp.fehbvm.com

int main() { std::cout << "Hello\n"; }
来源：http://kvp.bjfxy.top

[S32] C++：字符串
来源：http://hbh.cucudq.cn

std::string s = "hi";  s += "!";
来源：http://cev.shzxlz.cn

[S33] C++：vector 增删
来源：http://owr.hysaishi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dcg.ctjpmb.com

[S34] C++：遍历 vector
来源：http://rjr.ctjpmb.com

for (auto &x : v) { std::cout << x; }
来源：http://pci.yfazqb.com

[S35] C++：map
来源：http://qyd.iojbl.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mpw.xinyue.icu

[S36] C++：unordered_map
来源：http://qdy.shangyingyoupin.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gsp.zhijiandao.cn

[S37] C++：set
来源：http://xlf.tian-w.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://aed.daxiang520.top

[S38] C++：排序
来源：http://zij.cqqwz.cn

std::sort(v.begin(), v.end());
来源：http://bzg.jinghuilouyu.cn

[S39] C++：自定义比较器排序
来源：http://xzm.xingfuxueyuan.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jyr.fengsongda.top

[S40] C++：查找元素
来源：http://mbh.cqqwz.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://urj.shangyingyoupin.top

[S41] C++：类与构造函数
来源：http://get.feifeiyinyue.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gsg.xziqi.cn

[S42] C++：继承与虚函数
来源：http://vxn.quarkkingdee.top

class B : public Base { public: void f() override {} };
来源：http://qtf.fengsongda.top

[S43] C++：智能指针
来源：http://bnm.cashguo.top

auto p = std::make_unique<int>(5);
来源：http://phg.yj20258.top

[S44] C++：引用传参
来源：http://hcn.epnwcf.com

void inc(int &x) { ++x; }
来源：http://ixb.gotoacloud.top

[S45] C++：lambda
来源：http://ytz.chenlongwang.top

auto add = [](int a, int b) { return a + b; };
来源：http://dax.shanyushiyangkeji.top

[S46] C++：函数模板
来源：http://eqf.gaohongyu789.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lgj.pycfn.com

[S47] C++：结构化绑定遍历
来源：http://mqm.shanyushiyangkeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rob.guannengcc.top

[S48] C++：逐行读文件
来源：http://drv.sufxvd.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pzk.andypj.xyz

while (std::getline(in, line)) { }
来源：http://rfs.havefunace.top

[S49] C++：写文件
来源：http://atb.ivvv.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zec.sufxvd.cn

[S50] C++：格式化数字
来源：http://aef.yj202588.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rgp.epnwcf.com

[S51] C++：显式类型转换
来源：http://yvi.yj20258888.top

static_cast<double>(a) / b
来源：http://rql.havefunace.top

[S52] C++：const 与 noexcept
来源：http://umt.aibaodan.cn

int size() const noexcept { return n_; }
来源：http://jgh.c1oappe.top

[S53] C++：移动语义
来源：http://moo.ydzc1.top

std::vector<int> w = std::move(v);
来源：http://jxm.jinyuanbaomall.cn

[S54] C++：异常处理
来源：http://vsy.ehwqpu.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gap.sxryk.cn

[S55] C++：结构化绑定
来源：http://iro.ppjwa.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rbc.uphjek.com

[S56] C++：optional
来源：http://dfj.wangdashe.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://way.vehdjk.com

[S57] C++：编译期常量
来源：http://szd.ywan-chungtsiang.top

constexpr int N = 10;
来源：http://tzl.yj20258.top

[S58] C++：命名空间
来源：http://acc.mhx1999.top

namespace ns { int f() { return 1; } }
来源：http://fyf.xylfe.cn

[S59] C++：静态断言
来源：http://cuo.hnxiangtu.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://psm.ppjwa.cn

[S60] C++：遍历并删除元素
来源：http://crc.jlsjyb.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zcp.jyoumei.cn

================================================================================
来源：http://syy.fzhhl.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lcr.nwbrower.top

================================================================================
来源：http://yvs.daxiang520.top

[T01] Kotlin：Hello World
来源：http://idl.ehwqpu.com

println("Hello")
来源：http://tbe.tarul.cn

[T02] Kotlin：变量
来源：http://wup.jianghu66.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ctl.ywan-chungtsiang.top

[T03] Kotlin：字符串模板
来源：http://vec.fehbvm.com

"值: $b"
来源：http://qzt.chenjidiqi.icu

[T04] Kotlin：空安全
来源：http://vym.zhixingplan.top

val n: String? = null;  n?.length
来源：http://tee.shangyingyoupin.top

[T05] Kotlin：when 表达式
来源：http://cbg.zycfv.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yzm.jinghuilouyu.cn

[T06] Kotlin：集合映射
来源：http://ojf.shangyingyoupin.top

listOf(1, 2, 3).map { it * 2 }
来源：http://tnf.jyoumei.cn

[T07] Kotlin：集合过滤
来源：http://mic.0kj1m.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://yrg.hywenlv.cn

[T08] Kotlin：数据类
来源：http://utb.hnqzz.top

data class User(val name: String, val age: Int)
来源：http://uix.snrcjt.cn

[T09] Kotlin：扩展函数
来源：http://wre.snrcjt.cn

fun String.exclaim() = this + "!"
来源：http://qts.nwbrower.top

[T10] Kotlin：默认参数
来源：http://spa.hywenlv.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://dzl.jinyuanbaomall.cn

[T11] Kotlin：协程
来源：http://wum.shanyushiyangtech.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://zrw.jianghu66.top

[T12] Kotlin：解构声明
来源：http://lta.smart0.xyz

val (a, b) = Pair(1, 2)
来源：http://pkx.xziqi.cn

[T13] Kotlin：只读 Map
来源：http://elc.tianlin.xyz

val m = mapOf("a" to 1)
来源：http://utx.kuanghao11.cn

[T14] Kotlin：循环
来源：http://nxq.quarkkingdee.top

for (i in 1..10) println(i)
来源：http://bsu.yanxiufei.cn

[T15] Kotlin：接口
来源：http://yzj.jinyuanbaomall.cn

interface Shape { fun area(): Double }
来源：http://rrx.shangyingyoupin.top

[T16] Swift：Hello World
来源：http://iqe.shzxlz.cn

print("Hello")
来源：http://fus.vehdjk.com

[T17] Swift：变量与常量
来源：http://igq.ivvv.top

var a = 1;  let b = 2
来源：http://szh.cqqwz.cn

[T18] Swift：字符串插值
来源：http://brl.xziqi.cn

"值: \(b)"
来源：http://scg.yj202588.top

[T19] Swift：可选绑定
来源：http://lyu.aibaodan.cn

if let n = opt { print(n) }
来源：http://fav.gotoacloud.top

[T20] Swift：数组操作
来源：http://rlk.hesvh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gnu.zdqjudy.top

[T21] Swift：遍历
来源：http://beu.cashguo.top

for x in a { print(x) }
来源：http://ith.xuetiantiany.cn

[T22] Swift：字典
来源：http://wuy.yj20258.top

var d = ["a": 1];  d["b"] = 2
来源：http://oam.svipenyu.cn

[T23] Swift：函数
来源：http://cgz.hnxiangtu.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://exm.andypj.xyz

[T24] Swift：闭包
来源：http://ner.shanyushiyangkeji.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://woq.bjfxy.top

[T25] Swift：结构体
来源：http://ewc.ybcxt.top

struct P { var x: Int }
来源：http://qhu.haohaochexian.top

[T26] Swift：类与重写
来源：http://jla.vqdsnc.cn

class A: Base { override func f() {} }
来源：http://xql.tianlin.xyz

[T27] Swift：错误处理
来源：http://vsh.jyoumei.cn

do { try f() } catch { print(error) }
来源：http://viz.ydjk.org.cn

[T28] Swift：枚举
来源：http://omc.aibaodan.cn

enum Color { case red, green }
来源：http://fnf.zhoulong.xyz

[T29] Swift：guard 提前返回
来源：http://dxk.yuanzhike.top

guard let x = opt else { return }
来源：http://oxy.smart0.xyz

[T30] Swift：协议
来源：http://knv.zdbjq.cn

protocol Shape { func area() -> Double }
来源：http://lwk.gogol.net.cn

[T31] Lua：Hello World
来源：http://sry.yangfankeji.com

print("Hello")
来源：http://qsc.ctjpmb.com

[T32] Lua：局部变量
来源：http://fxf.chenzaomai.com

local a = 1
来源：http://qii.52xcode.cn

[T33] Lua：表（数组）
来源：http://rbd.shuidangran.top

local t = {1, 2, 3};  t[4] = 4
来源：http://wmk.zhengqikj.top

[T34] Lua：遍历表
来源：http://ysh.xuetiantiany.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://lwl.pengpengdd.cyou

[T35] Lua：字典表
来源：http://mjb.xingfuxueyuan.xyz

local d = { a = 1 };  d.b = 2
来源：http://nwx.dianchejie.cn

[T36] Lua：函数
来源：http://yoq.xingfuxueyuan.xyz

function add(a, b) return a + b end
来源：http://aum.zhengqikj.top

[T37] Lua：字符串拼接
来源：http://mrw.yuanzhike.top

"a" .. "b"
来源：http://gvz.xziqi.cn

[T38] Lua：条件
来源：http://fzw.jlsjyb.cn

if x > 0 then print("正") end
来源：http://pyl.hammf.cn


<!-- 参考信息 -->