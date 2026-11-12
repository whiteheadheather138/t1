代发 wailian999

cmd > out.log 2>&1
来源：http://hiy.haohaochexian.top

[R40] 追加写日志
来源：http://byz.bjfxy.top

echo "log" >> out.log
来源：http://xes.cucudq.cn

[R41] 丢弃输出
来源：http://wzc.sweek.top

cmd >/dev/null 2>&1
来源：http://yqi.jinqigfzy.top

[R42] 输入重定向
来源：http://pwp.yongpay.top

wc -l < a.txt
来源：http://cuk.nanxinkj.top

[R43] 按名字查找文件
来源：http://dyp.zdqjudy.top

find . -name "*.log" -type f
来源：http://cqc.sufxvd.cn

[R44] 按修改时间查找
来源：http://nxz.jinyuanbaomall.cn

find . -mtime -7 -type f
来源：http://pqk.ydzc1.top

[R45] 批量删除
来源：http://pey.smart0.xyz

find . -name "*.tmp" -delete
来源：http://xmp.ydjk.org.cn

[R46] 递归替换文件内容
来源：http://icg.tianlin.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ylm.xylfe.cn

[R47] sed 单行替换
来源：http://tdk.chenjidiqi.icu

sed -i 's/foo/bar/g' a.txt
来源：http://hqq.316326.xyz

[R48] awk 取指定列
来源：http://waw.zhixingplan.top

awk '{print $1, $3}' a.txt
来源：http://clg.316326.xyz

[R49] awk 带条件
来源：http://qre.xingfuxueyuan.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cgi.nanxinkj.top

[R50] awk 求和
来源：http://drb.wangshuangyany.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ftu.c1oappe.top

[R51] 排序去重取前几
来源：http://hdx.haohaochexian.top

sort a.txt | uniq -c | sort -rn | head
来源：http://gdj.zycfv.cn

[R52] 统计行数
来源：http://wwc.xuanzx.com

wc -l a.txt
来源：http://ags.nanxinkj.top

[R53] 查看文件头与实时尾
来源：http://npn.yonumen.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yax.redwolf501.top

[R54] 比较两个文件
来源：http://ohc.hesvh.cn

diff a.txt b.txt
来源：http://wni.fehbvm.com

[R55] 压缩与解压
来源：http://okd.hfpthk.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qka.svipenyu.cn

[R56] 远程拷贝
来源：http://kgx.yuanzhike.top

scp file user@host:/path/
来源：http://iwp.smart0.xyz

[R57] 远程执行命令
来源：http://yqx.nwbrower.top

ssh user@host 'uptime'
来源：http://cme.aizwys.cn

[R58] 下载文件
来源：http://jol.fzhhl.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hmf.quarkkingdee.top

[R59] 发 POST JSON
来源：http://yua.snrcjt.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sfx.shuidangran.top

[R60] 只看 HTTP 状态码
来源：http://ybw.bbcook.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://red.ehwqpu.com

[R61] 磁盘占用
来源：http://exk.guowangkeji.top

df -h;  du -sh *
来源：http://xyi.nwbrower.top

[R62] 找最占空间的文件
来源：http://inm.wangdashe.top

du -ah . | sort -rh | head -10
来源：http://dnc.shangyingyoupin.top

[R63] 内存与进程
来源：http://rqy.shzxlz.cn

free -h;  ps aux | grep nginx
来源：http://nei.jinyuanbaomall.cn

[R64] 结束进程
来源：http://rsk.gotoacloud.top

kill -9 $(pgrep -f app.py)
来源：http://tor.xingfuxueyuan.xyz

[R65] 查看端口占用
来源：http://opw.yfazqb.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ubn.gotoacloud.top

[R66] 定时任务
来源：http://awc.fktsv.cn

crontab -e;  crontab -l
来源：http://uwl.wangshuangyany.cn

[R67] 生成随机十六进制串
来源：http://tzy.aizwys.cn

openssl rand -hex 16
来源：http://quh.shanyushiyangkeji.top

[R68] 计算文件校验值
来源：http://bod.yj20258888.top

sha256sum a.txt;  md5sum a.txt
来源：http://bai.tanke756.top

[R69] 生成随机密码
来源：http://zil.yangfankeji.com

head -c 16 /dev/urandom | base64
来源：http://zyb.pycfn.com

[R70] 时间戳与互转
来源：http://ykm.cdnleiting.top

date +%s;  date -d @1700000000
来源：http://kye.fengsongda.top

[R71] 日期格式化
来源：http://xoj.pengpengdd.cyou

date +"%Y-%m-%d %H:%M:%S"
来源：http://wpz.chenjidiqi.icu

[R72] 等待端口就绪
来源：http://ihv.svipenyu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dfa.zhengqikj.top

[R73] 分割大日志
来源：http://eqp.nanxinkj.top

split -l 1000 big.log part_
来源：http://dei.jianghu66.top

[R74] 批量重命名
来源：http://zlw.bbcook.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://eer.hcnkem.com

[R75] 导出环境变量
来源：http://yot.pengpengdd.cyou

export PATH="$HOME/bin:$PATH"
来源：http://lyy.cheryme.top

[R76] 使用临时文件
来源：http://wys.hnxiangtu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tps.316326.xyz

[R77] 读取用户输入
来源：http://sjw.zhijiandao.cn

read -rp "请输入: " ans
来源：http://vuy.pycfn.com

[R78] 交互式菜单
来源：http://mky.cdnleiting.top

select opt in a b c; do echo "$opt"; break; done
来源：http://jtv.pycfn.com

[R79] 解析命令行选项
来源：http://mkw.sjlbkw.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ayu.zhiwuduotai.top

[R80] 查看脚本执行耗时
来源：http://dqw.hesvh.cn

time ./run.sh
来源：http://uav.fktsv.cn

================================================================================
来源：http://blg.cqqwz.cn

S. C / C++ 专题
来源：http://omd.316326.xyz

================================================================================
来源：http://fcu.xuetiantiany.cn

[S01] C：Hello World
来源：http://wdk.hcnkem.com

#include <stdio.h>
来源：http://hby.zdbjq.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hdw.jinyuanbaomall.cn

[S02] C：变量与格式化输出
来源：http://vwv.aizwys.cn

int a = 10; printf("%d\n", a);
来源：http://gbh.zhaomingkeji.xyz

[S03] C：读入整数
来源：http://dgw.jinqigufen.top

int x; scanf("%d", &x);
来源：http://jcz.jinqigfzy.top

[S04] C：字符串复制
来源：http://tab.daria6918.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wwk.xingfuxueyuan.xyz

[S05] C：字符串长度
来源：http://lgs.uphjek.com

strlen(s)
来源：http://sfo.feifeiyinyue.top

[S06] C：字符串比较
来源：http://aen.zhengqikj.top

strcmp(a, b) == 0
来源：http://pni.yueranfly.top

[S07] C：数组遍历求和
来源：http://fmw.zhoulong.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ysm.redwolf501.top

[S08] C：动态内存分配与释放
来源：http://rxv.xziqi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qib.zhijiandao.cn

[S09] C：结构体定义与初始化
来源：http://oph.guowangkeji.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ofn.andypj.xyz

[S10] C：指针与解引用
来源：http://vgp.bbcook.cn

int *p = &a;  *p = 5;
来源：http://eqm.daria6918.cn

[S11] C：逐行读文件
来源：http://lla.xylfe.cn

FILE *f = fopen("a.txt", "r");
来源：http://nvh.chenjidiqi.icu

while (fgets(buf, sizeof buf, f)) { }
来源：http://wct.xingfuxueyuan.xyz

fclose(f);
来源：http://qcx.chenzaomai.com

[S12] C：写文件
来源：http://ujp.zdbjq.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cqv.jinqigufen.top

[S13] C：宏定义
来源：http://kwk.c1oappe.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://otz.vehdjk.com

[S14] C：枚举
来源：http://svu.jiagoushi.top

enum Color { RED, GREEN, BLUE };
来源：http://tqq.zhiwuduotai.top

[S15] C：类型转换
来源：http://cnr.hnqzz.top

(double) a / b
来源：http://lhu.guowangkeji.top

[S16] C：位操作置位
来源：http://vmw.hysaishi.cn

x |= (1 << 3);
来源：http://btk.fengsongda.top

[S17] C：安全拼接字符串
来源：http://wlc.zhoulong.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xrh.cqqwz.cn

[S18] C：命令行参数
来源：http://nvk.cqqwz.cn

int main(int argc, char **argv)
来源：http://agi.dashuyun.cn

[S19] C：快速排序
来源：http://bjc.yueranfly.top

qsort(a, n, sizeof(int), cmp);
来源：http://fob.hammf.cn

[S20] C：二分查找
来源：http://qte.iojbl.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://exa.zhijiandao.cn

[S21] C：字符类别判断
来源：http://gbg.zhixingplan.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fvj.zhijiandao.cn

[S22] C：字符串转数字
来源：http://fhe.guannengcc.top

atoi("42");  strtod("3.14", NULL);
来源：http://vhb.hnxiangtu.top

[S23] C：随机数
来源：http://mkk.jianghu66.top

srand(time(NULL));  int r = rand() % 100;
来源：http://art.hnqzz.top

[S24] C：获取本地时间
来源：http://wyh.nanxuanxn.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://njf.pengpengdd.cyou

[S25] C：内存拷贝
来源：http://tyu.jinqigufen.top

memcpy(dst, src, n);
来源：http://tam.jlsjyb.cn

[S26] C：内存清零
来源：http://qjg.c1oappe.top

memset(a, 0, sizeof a);
来源：http://jvr.yongpay.top

[S27] C：定义常量
来源：http://imf.ppjwa.cn

const double PI = 3.14159;
来源：http://zgy.zdqjudy.top

[S28] C：静态变量
来源：http://yiq.fzhhl.top

static int counter = 0;
来源：http://kga.gzhubu.top

[S29] C：变参函数
来源：http://vfa.yueranfly.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fvn.hywenlv.cn

[S30] C：头文件保护
来源：http://tgk.yj20258888.top

#ifndef X_H
来源：http://rwd.pengpengdd.cyou

#define X_H
来源：http://gmc.jyoumei.cn

#endif
来源：http://ynz.yj20258.top

[S31] C++：Hello World
来源：http://zav.dashuyun.cn

#include <iostream>
来源：http://zlf.sysykeji.top

int main() { std::cout << "Hello\n"; }
来源：http://dof.316326.xyz

[S32] C++：字符串
来源：http://ygf.wangshuangyany.cn

std::string s = "hi";  s += "!";
来源：http://bzk.jiagoushi.top

[S33] C++：vector 增删
来源：http://wii.xingfuxueyuan.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cea.jinghuilouyu.cn

[S34] C++：遍历 vector
来源：http://jxt.daria6918.cn

for (auto &x : v) { std::cout << x; }
来源：http://tby.jqgfzy.top

[S35] C++：map
来源：http://cpn.shuidangran.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gkn.bbcook.cn

[S36] C++：unordered_map
来源：http://hfu.jqgufenzy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gmk.epnwcf.com

[S37] C++：set
来源：http://sqt.shangyingyoupin.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mcl.ydjk.org.cn

[S38] C++：排序
来源：http://hqm.gotoacloud.top

std::sort(v.begin(), v.end());
来源：http://jxj.zhixingplan.top

[S39] C++：自定义比较器排序
来源：http://nhl.kuanghao11.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kcx.c1oappe.top

[S40] C++：查找元素
来源：http://eii.hnxiangtu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ssr.cheryme.top

[S41] C++：类与构造函数
来源：http://mhr.yfazqb.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://plr.wangdashe.top

[S42] C++：继承与虚函数
来源：http://ekm.dashuyun.cn

class B : public Base { public: void f() override {} };
来源：http://xxw.shzxlz.cn

[S43] C++：智能指针
来源：http://uam.daria6918.cn

auto p = std::make_unique<int>(5);
来源：http://fdz.yongpay.top

[S44] C++：引用传参
来源：http://xjp.mhx1999.top

void inc(int &x) { ++x; }
来源：http://fbj.shzxlz.cn

[S45] C++：lambda
来源：http://yqz.nwbrower.top

auto add = [](int a, int b) { return a + b; };
来源：http://nbd.fktsv.cn

[S46] C++：函数模板
来源：http://ime.guannengcc.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xfn.zdbjq.cn

[S47] C++：结构化绑定遍历
来源：http://fzy.hysaishi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tav.zhixingplan.top

[S48] C++：逐行读文件
来源：http://osi.yj20258888.top

std::ifstream in("a.txt");  std::string line;
来源：http://ajo.meibo888.top

while (std::getline(in, line)) { }
来源：http://wde.zhengqikj.top

[S49] C++：写文件
来源：http://eso.zhoulong.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://snm.shangyingyoupin.top

[S50] C++：格式化数字
来源：http://ity.xuanzx.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hkc.jinqigfzy.top

[S51] C++：显式类型转换
来源：http://xna.pycfn.com

static_cast<double>(a) / b
来源：http://bhr.ivvv.top

[S52] C++：const 与 noexcept
来源：http://lyr.yj20258.top

int size() const noexcept { return n_; }
来源：http://gbz.52xcode.cn

[S53] C++：移动语义
来源：http://ncp.c1oappe.top

std::vector<int> w = std::move(v);
来源：http://epd.shangyingyoupin.top

[S54] C++：异常处理
来源：http://ami.gaohongyu789.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nln.yj20258888.top

[S55] C++：结构化绑定
来源：http://hwp.bbcook.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://fdm.hesvh.cn

[S56] C++：optional
来源：http://bwp.cashguo.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mbq.nwbrower.top

[S57] C++：编译期常量
来源：http://htr.zhengqikj.top

constexpr int N = 10;
来源：http://nyd.wangshuangyany.cn

[S58] C++：命名空间
来源：http://bnw.fzhhl.top

namespace ns { int f() { return 1; } }
来源：http://pci.yueranfly.top

[S59] C++：静态断言
来源：http://sga.nanxinkj.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://guz.yj20258.top

[S60] C++：遍历并删除元素
来源：http://vhy.sxryk.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://umm.vqdsnc.cn

================================================================================
来源：http://obh.sysykeji.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://umv.yongpay.top

================================================================================
来源：http://hsc.quarkkingdee.top

[T01] Kotlin：Hello World
来源：http://vgr.hongshengwenyu.top

println("Hello")
来源：http://hzw.yfazqb.com

[T02] Kotlin：变量
来源：http://gvp.bbcook.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rhi.vehdjk.com

[T03] Kotlin：字符串模板
来源：http://esk.hongshengwenyu.top

"值: $b"
来源：http://jps.yongpay.top

[T04] Kotlin：空安全
来源：http://vqh.yj202588.top

val n: String? = null;  n?.length
来源：http://iqi.c1oappe.top

[T05] Kotlin：when 表达式
来源：http://bnp.meibo888.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jrn.dashuyun.cn

[T06] Kotlin：集合映射
来源：http://ibj.yfazqb.com

listOf(1, 2, 3).map { it * 2 }
来源：http://npm.tian-w.cn

[T07] Kotlin：集合过滤
来源：http://tkz.bbcook.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ggd.jinyuanbaomall.cn

[T08] Kotlin：数据类
来源：http://xzv.jqgufenzy.top

data class User(val name: String, val age: Int)
来源：http://pxh.sjlbkw.cn

[T09] Kotlin：扩展函数
来源：http://vvo.zdqjudy.top

fun String.exclaim() = this + "!"
来源：http://sei.yj20258.top

[T10] Kotlin：默认参数
来源：http://ymr.tarul.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://lyj.ybcxt.top

[T11] Kotlin：协程
来源：http://ada.aizwys.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://fbd.zdqjudy.top

[T12] Kotlin：解构声明
来源：http://hzm.hongshengwenyu.top

val (a, b) = Pair(1, 2)
来源：http://eha.wangdashe.top

[T13] Kotlin：只读 Map
来源：http://utz.havefunace.top

val m = mapOf("a" to 1)
来源：http://djj.jqgfzy.top

[T14] Kotlin：循环
来源：http://nsu.snrcjt.cn

for (i in 1..10) println(i)
来源：http://ccn.hongshengwenyu.top

[T15] Kotlin：接口
来源：http://zia.ivvv.top

interface Shape { fun area(): Double }
来源：http://ysx.andypj.xyz

[T16] Swift：Hello World
来源：http://sgr.zhixingplan.top

print("Hello")
来源：http://gtz.havefunace.top

[T17] Swift：变量与常量
来源：http://art.dianchejie.cn

var a = 1;  let b = 2
来源：http://keu.xingfuxueyuan.xyz

[T18] Swift：字符串插值
来源：http://jrc.zhoulong.xyz

"值: \(b)"
来源：http://xdm.jinqigufen.top

[T19] Swift：可选绑定
来源：http://oqe.tianlin.xyz

if let n = opt { print(n) }
来源：http://dlw.hnxiangtu.top

[T20] Swift：数组操作
来源：http://fzs.yuanzhike.top

var a = [1, 2, 3];  a.append(4)
来源：http://bkd.ppjwa.cn

[T21] Swift：遍历
来源：http://yho.cucudq.cn

for x in a { print(x) }
来源：http://uan.zhiwuduotai.top

[T22] Swift：字典
来源：http://iqw.yj20258.top

var d = ["a": 1];  d["b"] = 2
来源：http://rma.hcnkem.com

[T23] Swift：函数
来源：http://ozt.hywenlv.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://khy.nanxinkj.top

[T24] Swift：闭包
来源：http://pxk.svipenyu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://yvt.jqgfzy.top

[T25] Swift：结构体
来源：http://qfj.xingfuxueyuan.xyz

struct P { var x: Int }
来源：http://jes.yj202588.top

[T26] Swift：类与重写
来源：http://cnc.jyoumei.cn

class A: Base { override func f() {} }
来源：http://wxk.fengsongda.top

[T27] Swift：错误处理
来源：http://qqp.fanxiaobao.xyz

do { try f() } catch { print(error) }
来源：http://lcg.xinyue.icu

[T28] Swift：枚举
来源：http://hoh.jianghu66.top

enum Color { case red, green }
来源：http://lpi.yj202588.top

[T29] Swift：guard 提前返回
来源：http://xjg.nanxinkj.top

guard let x = opt else { return }
来源：http://yut.316326.xyz

[T30] Swift：协议
来源：http://vvq.shanyushiyangkeji.top

protocol Shape { func area() -> Double }
来源：http://ctv.ydjk.org.cn

[T31] Lua：Hello World
来源：http://kzf.xylfe.cn

print("Hello")
来源：http://owo.fktsv.cn

[T32] Lua：局部变量
来源：http://ezm.tanke756.top

local a = 1
来源：http://jqm.ppjwa.cn

[T33] Lua：表（数组）
来源：http://kkc.iojbl.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wbt.cheryme.top

[T34] Lua：遍历表
来源：http://oox.nwbrower.top

for i, v in ipairs(t) do print(i, v) end
来源：http://nls.yongpay.top

[T35] Lua：字典表
来源：http://kmy.hysaishi.cn

local d = { a = 1 };  d.b = 2
来源：http://lqh.hnqzz.top

[T36] Lua：函数
来源：http://nws.ydzc1.top

function add(a, b) return a + b end
来源：http://ose.yonumen.top

[T37] Lua：字符串拼接
来源：http://sbt.vehdjk.com

"a" .. "b"
来源：http://ajs.dashuyun.cn

[T38] Lua：条件
来源：http://bzo.jianghu66.top

if x > 0 then print("正") end
来源：http://jzx.vehdjk.com

[T39] Lua：模式匹配
来源：http://ivz.fengsongda.top

string.find(s, "%d+")
来源：http://ggz.yangfankeji.com

[T40] Lua：元表
来源：http://gme.jinyuanbaomall.cn

setmetatable({}, { __index = base })
来源：http://jrt.hesvh.cn

[T41] Perl：Hello World
来源：http://bvi.ydzc1.top

print "Hello\n";
来源：http://fkc.sweek.top

[T42] Perl：变量类型
来源：http://juj.yongpay.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://omh.tianlin.xyz


<!-- 参考信息 -->