代发 wailian999

find . -name "*.log" -type f
来源：http://yno.yonumen.top

[R44] 按修改时间查找
来源：http://lpx.shanyushiyangkeji.top

find . -mtime -7 -type f
来源：http://cro.ivvv.top

[R45] 批量删除
来源：http://wfz.gaohongyu789.top

find . -name "*.tmp" -delete
来源：http://uup.sufxvd.cn

[R46] 递归替换文件内容
来源：http://ell.xuanzx.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lcj.zhiwuduotai.top

[R47] sed 单行替换
来源：http://dzl.jqgfzy.top

sed -i 's/foo/bar/g' a.txt
来源：http://ukq.hfpthk.cn

[R48] awk 取指定列
来源：http://pzg.xuetiantiany.cn

awk '{print $1, $3}' a.txt
来源：http://ysp.vehdjk.com

[R49] awk 带条件
来源：http://iun.bbcook.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://maq.fehbvm.com

[R50] awk 求和
来源：http://mbl.shuidangran.top

awk '{s += $2} END {print s}' a.txt
来源：http://uae.wangshuangyany.cn

[R51] 排序去重取前几
来源：http://jyi.shanyushiyangkeji.top

sort a.txt | uniq -c | sort -rn | head
来源：http://zgc.shangyingyoupin.top

[R52] 统计行数
来源：http://lly.fzhhl.top

wc -l a.txt
来源：http://ylo.sufxvd.cn

[R53] 查看文件头与实时尾
来源：http://vxs.jqgufenzy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mij.bjfxy.top

[R54] 比较两个文件
来源：http://bjk.zhixingplan.top

diff a.txt b.txt
来源：http://lfk.fzhhl.top

[R55] 压缩与解压
来源：http://rxp.hysaishi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bnv.ydjk.org.cn

[R56] 远程拷贝
来源：http://yvf.mhx1999.top

scp file user@host:/path/
来源：http://fnc.xylfe.cn

[R57] 远程执行命令
来源：http://jfl.chenlongwang.top

ssh user@host 'uptime'
来源：http://zsk.sweek.top

[R58] 下载文件
来源：http://mqn.jinyuanbaomall.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gql.shanyushiyangtech.top

[R59] 发 POST JSON
来源：http://pkb.havefunace.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qum.nwbrower.top

[R60] 只看 HTTP 状态码
来源：http://xxr.ybcxt.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://aax.wangshuangyany.cn

[R61] 磁盘占用
来源：http://kgc.tanke756.top

df -h;  du -sh *
来源：http://lgl.dashuyun.cn

[R62] 找最占空间的文件
来源：http://izf.hywenlv.cn

du -ah . | sort -rh | head -10
来源：http://nmm.yueranfly.top

[R63] 内存与进程
来源：http://cds.jqgufenzy.top

free -h;  ps aux | grep nginx
来源：http://ewk.hesvh.cn

[R64] 结束进程
来源：http://hjk.mhx1999.top

kill -9 $(pgrep -f app.py)
来源：http://paq.gzhubu.top

[R65] 查看端口占用
来源：http://gyk.iojbl.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yhy.chenjidiqi.icu

[R66] 定时任务
来源：http://bdf.aibaodan.cn

crontab -e;  crontab -l
来源：http://wxm.ywan-chungtsiang.top

[R67] 生成随机十六进制串
来源：http://bzi.cqqwz.cn

openssl rand -hex 16
来源：http://kgi.zhixingplan.top

[R68] 计算文件校验值
来源：http://hwf.yuanzhike.top

sha256sum a.txt;  md5sum a.txt
来源：http://ccd.ywan-chungtsiang.top

[R69] 生成随机密码
来源：http://efu.zhaomingkeji.xyz

head -c 16 /dev/urandom | base64
来源：http://oop.yj20258888.top

[R70] 时间戳与互转
来源：http://nte.gaohongyu789.top

date +%s;  date -d @1700000000
来源：http://uht.zhoulong.xyz

[R71] 日期格式化
来源：http://jiy.yuanzhike.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://bbm.haohaochexian.top

[R72] 等待端口就绪
来源：http://kpy.wangshuangyany.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://tlr.redwolf501.top

[R73] 分割大日志
来源：http://vwg.dashuyun.cn

split -l 1000 big.log part_
来源：http://brd.vqdsnc.cn

[R74] 批量重命名
来源：http://tfv.hongshengwenyu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xim.chenlongwang.top

[R75] 导出环境变量
来源：http://tjd.andypj.xyz

export PATH="$HOME/bin:$PATH"
来源：http://tqo.hongshengwenyu.top

[R76] 使用临时文件
来源：http://brw.316326.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dpn.jinghuilouyu.cn

[R77] 读取用户输入
来源：http://dlx.ctjpmb.com

read -rp "请输入: " ans
来源：http://eac.yuxming.cn

[R78] 交互式菜单
来源：http://mel.gogol.net.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zek.daxiang520.top

[R79] 解析命令行选项
来源：http://yaz.tianlin.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blq.cqqwz.cn

[R80] 查看脚本执行耗时
来源：http://lzf.feifeiyinyue.top

time ./run.sh
来源：http://rbb.sjlbkw.cn

================================================================================
来源：http://acz.hysaishi.cn

S. C / C++ 专题
来源：http://dmf.yj20258.top

================================================================================
来源：http://zqo.chenlongwang.top

[S01] C：Hello World
来源：http://dtj.fehbvm.com

#include <stdio.h>
来源：http://zzq.tanke756.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://veq.zhixingplan.top

[S02] C：变量与格式化输出
来源：http://gls.cdnleiting.top

int a = 10; printf("%d\n", a);
来源：http://dbj.yongpay.top

[S03] C：读入整数
来源：http://bzm.wangshuangyany.cn

int x; scanf("%d", &x);
来源：http://fll.yuxming.cn

[S04] C：字符串复制
来源：http://vao.dashuyun.cn

char dst[32]; strcpy(dst, "hi");
来源：http://hoj.xuetiantiany.cn

[S05] C：字符串长度
来源：http://qvd.tian-w.cn

strlen(s)
来源：http://zce.shanyushiyangkeji.top

[S06] C：字符串比较
来源：http://ver.hfpthk.cn

strcmp(a, b) == 0
来源：http://mrb.nanxuanxn.top

[S07] C：数组遍历求和
来源：http://yay.tian-w.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hvn.wangdashe.top

[S08] C：动态内存分配与释放
来源：http://fxr.tanke756.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hsc.cheryme.top

[S09] C：结构体定义与初始化
来源：http://wpg.yueranfly.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rkq.havefunace.top

[S10] C：指针与解引用
来源：http://unc.jlsjyb.cn

int *p = &a;  *p = 5;
来源：http://pva.redwolf501.top

[S11] C：逐行读文件
来源：http://ieg.gaohongyu789.top

FILE *f = fopen("a.txt", "r");
来源：http://jsq.smart0.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://ngf.zhongyouzk.top

fclose(f);
来源：http://lfk.hysaishi.cn

[S12] C：写文件
来源：http://trs.fktsv.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lad.nanxinkj.top

[S13] C：宏定义
来源：http://kft.zdbjq.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vil.bbcook.cn

[S14] C：枚举
来源：http://zhk.tanke756.top

enum Color { RED, GREEN, BLUE };
来源：http://nrs.yueranfly.top

[S15] C：类型转换
来源：http://kvo.feifeiyinyue.top

(double) a / b
来源：http://lqm.sxryk.cn

[S16] C：位操作置位
来源：http://nzu.hysaishi.cn

x |= (1 << 3);
来源：http://jgo.yj20258.top

[S17] C：安全拼接字符串
来源：http://tqz.andypj.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vho.hongshengwenyu.top

[S18] C：命令行参数
来源：http://wyj.kuanghao11.cn

int main(int argc, char **argv)
来源：http://fdy.jlsjyb.cn

[S19] C：快速排序
来源：http://qpy.xylfe.cn

qsort(a, n, sizeof(int), cmp);
来源：http://tpp.jinqigufen.top

[S20] C：二分查找
来源：http://ofx.zhaomingkeji.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kzq.ydjk.org.cn

[S21] C：字符类别判断
来源：http://rta.tianlin.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ltj.yfazqb.com

[S22] C：字符串转数字
来源：http://gki.cdnleiting.top

atoi("42");  strtod("3.14", NULL);
来源：http://gem.feifeiyinyue.top

[S23] C：随机数
来源：http://mpe.fehbvm.com

srand(time(NULL));  int r = rand() % 100;
来源：http://cgc.dashuyun.cn

[S24] C：获取本地时间
来源：http://lzv.cqqwz.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gko.ydjk.org.cn

[S25] C：内存拷贝
来源：http://xtx.nanxinkj.top

memcpy(dst, src, n);
来源：http://yrm.yuxming.cn

[S26] C：内存清零
来源：http://wtx.yongpay.top

memset(a, 0, sizeof a);
来源：http://ree.jlsjyb.cn

[S27] C：定义常量
来源：http://yiz.jyoumei.cn

const double PI = 3.14159;
来源：http://bnt.xinyue.icu

[S28] C：静态变量
来源：http://naz.havefunace.top

static int counter = 0;
来源：http://gbc.aizwys.cn

[S29] C：变参函数
来源：http://eih.yongpay.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://heh.sysykeji.top

[S30] C：头文件保护
来源：http://ezk.dianchejie.cn

#ifndef X_H
来源：http://zds.zhijiandao.cn

#define X_H
来源：http://psj.shanyushiyangkeji.top

#endif
来源：http://cvy.xuetiantiany.cn

[S31] C++：Hello World
来源：http://hsd.hnxiangtu.top

#include <iostream>
来源：http://yuj.hongshengwenyu.top

int main() { std::cout << "Hello\n"; }
来源：http://ukt.nanxuanxn.top

[S32] C++：字符串
来源：http://trb.hcnkem.com

std::string s = "hi";  s += "!";
来源：http://mbq.fehbvm.com

[S33] C++：vector 增删
来源：http://yme.ehwqpu.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rrk.daria6918.cn

[S34] C++：遍历 vector
来源：http://zmt.zhongyouzk.top

for (auto &x : v) { std::cout << x; }
来源：http://nec.hongshengwenyu.top

[S35] C++：map
来源：http://csc.fktsv.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ruc.shuidangran.top

[S36] C++：unordered_map
来源：http://pro.hongshengwenyu.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gxy.hywenlv.cn

[S37] C++：set
来源：http://wnl.sufxvd.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jna.yj20258888.top

[S38] C++：排序
来源：http://vnf.fengsongda.top

std::sort(v.begin(), v.end());
来源：http://ujh.gzhubu.top

[S39] C++：自定义比较器排序
来源：http://vvb.hnxiangtu.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ayx.yueranfly.top

[S40] C++：查找元素
来源：http://gaf.ppjwa.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gtl.jinyuanbaomall.cn

[S41] C++：类与构造函数
来源：http://dtu.zhoulong.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://brx.yj20258888.top

[S42] C++：继承与虚函数
来源：http://tkf.cdnleiting.top

class B : public Base { public: void f() override {} };
来源：http://bnt.jqgfzy.top

[S43] C++：智能指针
来源：http://sbm.feifeiyinyue.top

auto p = std::make_unique<int>(5);
来源：http://ahw.yueranfly.top

[S44] C++：引用传参
来源：http://qrl.nwbrower.top

void inc(int &x) { ++x; }
来源：http://wtm.ehwqpu.com

[S45] C++：lambda
来源：http://vzh.xylfe.cn

auto add = [](int a, int b) { return a + b; };
来源：http://lzq.cdnleiting.top

[S46] C++：函数模板
来源：http://jqp.c1oappe.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vul.chenjidiqi.icu

[S47] C++：结构化绑定遍历
来源：http://lmd.jqgufenzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tsw.zdbjq.cn

[S48] C++：逐行读文件
来源：http://hhc.andypj.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://ncq.yfazqb.com

while (std::getline(in, line)) { }
来源：http://ofe.daria6918.cn

[S49] C++：写文件
来源：http://ryq.zhaomingkeji.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lgc.smart0.xyz

[S50] C++：格式化数字
来源：http://rot.jyoumei.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pzo.dianchejie.cn

[S51] C++：显式类型转换
来源：http://oso.haohaochexian.top

static_cast<double>(a) / b
来源：http://vwg.jlsjyb.cn

[S52] C++：const 与 noexcept
来源：http://ivn.shanyushiyangtech.top

int size() const noexcept { return n_; }
来源：http://rlx.hysaishi.cn

[S53] C++：移动语义
来源：http://rnl.chenlongwang.top

std::vector<int> w = std::move(v);
来源：http://wik.ppjwa.cn

[S54] C++：异常处理
来源：http://hmq.jinqigufen.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nyr.wangshuangyany.cn

[S55] C++：结构化绑定
来源：http://roz.hfpthk.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vnn.zycfv.cn

[S56] C++：optional
来源：http://brk.pycfn.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ogp.jinqigfzy.top

[S57] C++：编译期常量
来源：http://gmj.fzhhl.top

constexpr int N = 10;
来源：http://kra.haohaochexian.top

[S58] C++：命名空间
来源：http://ajk.epnwcf.com

namespace ns { int f() { return 1; } }
来源：http://aiw.wangdashe.top

[S59] C++：静态断言
来源：http://thp.yuanzhike.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fgz.xziqi.cn

[S60] C++：遍历并删除元素
来源：http://ghj.jlsjyb.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xtb.hesvh.cn

================================================================================
来源：http://nmn.tarul.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ghq.snrcjt.cn

================================================================================
来源：http://viw.aizwys.cn

[T01] Kotlin：Hello World
来源：http://khc.jqgufenzy.top

println("Hello")
来源：http://jnm.yj20258.top

[T02] Kotlin：变量
来源：http://sbl.jinyuanbaomall.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ish.gzhubu.top

[T03] Kotlin：字符串模板
来源：http://pia.ydzc1.top

"值: $b"
来源：http://fzt.wangshuangyany.cn

[T04] Kotlin：空安全
来源：http://nnh.zhijiandao.cn

val n: String? = null;  n?.length
来源：http://ewx.c1oappe.top

[T05] Kotlin：when 表达式
来源：http://hnd.yj202588.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dhj.nanxuanxn.top

[T06] Kotlin：集合映射
来源：http://eva.shuidangran.top

listOf(1, 2, 3).map { it * 2 }
来源：http://oyr.iojbl.cn

[T07] Kotlin：集合过滤
来源：http://byv.dashuyun.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://kun.hnxiangtu.top

[T08] Kotlin：数据类
来源：http://rzb.pengpengdd.cyou

data class User(val name: String, val age: Int)
来源：http://ucu.hnxiangtu.top

[T09] Kotlin：扩展函数
来源：http://nol.andypj.xyz

fun String.exclaim() = this + "!"
来源：http://oyf.cashguo.top

[T10] Kotlin：默认参数
来源：http://usl.cdnleiting.top

fun greet(name: String = "World") = "Hi $name"
来源：http://yyi.jinqigufen.top

[T11] Kotlin：协程
来源：http://gul.0kj1m.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://sce.hfpthk.cn

[T12] Kotlin：解构声明
来源：http://orz.hcnkem.com

val (a, b) = Pair(1, 2)
来源：http://eez.redwolf501.top

[T13] Kotlin：只读 Map
来源：http://zhh.xingfuxueyuan.xyz

val m = mapOf("a" to 1)
来源：http://luv.jqgufenzy.top

[T14] Kotlin：循环
来源：http://sgc.aibaodan.cn

for (i in 1..10) println(i)
来源：http://mms.jyoumei.cn

[T15] Kotlin：接口
来源：http://vug.xinyue.icu

interface Shape { fun area(): Double }
来源：http://rjo.guannengcc.top

[T16] Swift：Hello World
来源：http://hwx.tianlin.xyz

print("Hello")
来源：http://yll.hnxiangtu.top

[T17] Swift：变量与常量
来源：http://wfg.gogol.net.cn

var a = 1;  let b = 2
来源：http://ppp.jinyuanbaomall.cn

[T18] Swift：字符串插值
来源：http://lns.yueranfly.top

"值: \(b)"
来源：http://uvq.yueranfly.top

[T19] Swift：可选绑定
来源：http://yrh.yongpay.top

if let n = opt { print(n) }
来源：http://emx.ydjk.org.cn

[T20] Swift：数组操作
来源：http://mup.shangyingyoupin.top

var a = [1, 2, 3];  a.append(4)
来源：http://nwy.nanxuanxn.top

[T21] Swift：遍历
来源：http://jww.jqgfzy.top

for x in a { print(x) }
来源：http://bgt.gaohongyu789.top

[T22] Swift：字典
来源：http://wyh.jqgufenzy.top

var d = ["a": 1];  d["b"] = 2
来源：http://lvu.9152youxi.cn

[T23] Swift：函数
来源：http://gzs.hcnkem.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ljj.shanyushiyangkeji.top

[T24] Swift：闭包
来源：http://gfj.xuetiantiany.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://jyy.kuanghao11.cn

[T25] Swift：结构体
来源：http://irj.yj20258.top

struct P { var x: Int }
来源：http://qtx.jqgufenzy.top

[T26] Swift：类与重写
来源：http://qru.meibo888.top

class A: Base { override func f() {} }
来源：http://qrv.chenlongwang.top

[T27] Swift：错误处理
来源：http://eqs.fehbvm.com

do { try f() } catch { print(error) }
来源：http://htr.52xcode.cn

[T28] Swift：枚举
来源：http://shw.zdqjudy.top

enum Color { case red, green }
来源：http://ldm.epnwcf.com

[T29] Swift：guard 提前返回
来源：http://har.hammf.cn

guard let x = opt else { return }
来源：http://mfd.vehdjk.com

[T30] Swift：协议
来源：http://emm.chenlongwang.top

protocol Shape { func area() -> Double }
来源：http://clv.yanxiufei.cn

[T31] Lua：Hello World
来源：http://rbn.sweek.top

print("Hello")
来源：http://zex.yj20258888.top

[T32] Lua：局部变量
来源：http://olk.dianchejie.cn

local a = 1
来源：http://yme.vehdjk.com

[T33] Lua：表（数组）
来源：http://wst.zhengqikj.top

local t = {1, 2, 3};  t[4] = 4
来源：http://vck.hfpthk.cn

[T34] Lua：遍历表
来源：http://hzu.shanyushiyangkeji.top

for i, v in ipairs(t) do print(i, v) end
来源：http://abh.hongshengwenyu.top

[T35] Lua：字典表
来源：http://xko.tianlin.xyz

local d = { a = 1 };  d.b = 2
来源：http://egn.tarul.cn

[T36] Lua：函数
来源：http://udl.gogol.net.cn

function add(a, b) return a + b end
来源：http://juz.havefunace.top

[T37] Lua：字符串拼接
来源：http://bpa.xingfuxueyuan.xyz

"a" .. "b"
来源：http://fvi.xylfe.cn

[T38] Lua：条件
来源：http://zqb.smart0.xyz

if x > 0 then print("正") end
来源：http://ovq.cashguo.top

[T39] Lua：模式匹配
来源：http://hye.snrcjt.cn

string.find(s, "%d+")
来源：http://eto.chenlongwang.top

[T40] Lua：元表
来源：http://qjk.hcnkem.com

setmetatable({}, { __index = base })
来源：http://ryp.cheryme.top

[T41] Perl：Hello World
来源：http://nsp.havefunace.top

print "Hello\n";
来源：http://bbn.sweek.top

[T42] Perl：变量类型
来源：http://dfm.shangyingyoupin.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hix.yuanzhike.top

[T43] Perl：字符串插值
来源：http://ofs.sysykeji.top

"值: $a"
来源：http://kxt.chenzaomai.com

[T44] Perl：条件
来源：http://cel.sjlbkw.cn

if ($a > 0) { print "正"; }
来源：http://dav.pycfn.com

[T45] Perl：数组遍历
来源：http://kvz.quarkkingdee.top

for my $x (@arr) { print $x; }
来源：http://fdx.cucudq.cn

[T46] Perl：哈希操作
来源：http://hys.tarul.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bmd.haohaochexian.top


<!-- 参考信息 -->