代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kbv.sjlbkw.cn

[R50] awk 求和
来源：http://evt.havefunace.top

awk '{s += $2} END {print s}' a.txt
来源：http://cog.hcnkem.com

[R51] 排序去重取前几
来源：http://dsw.hnxiangtu.top

sort a.txt | uniq -c | sort -rn | head
来源：http://xww.shzxlz.cn

[R52] 统计行数
来源：http://rky.ydzc1.top

wc -l a.txt
来源：http://uhw.smart0.xyz

[R53] 查看文件头与实时尾
来源：http://fpv.ivvv.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://svt.chenzaomai.com

[R54] 比较两个文件
来源：http://gul.cdnleiting.top

diff a.txt b.txt
来源：http://yym.haohaochexian.top

[R55] 压缩与解压
来源：http://uln.fanxiaobao.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vfe.aibaodan.cn

[R56] 远程拷贝
来源：http://aab.hnxiangtu.top

scp file user@host:/path/
来源：http://xnn.jqgfzy.top

[R57] 远程执行命令
来源：http://qfr.daria6918.cn

ssh user@host 'uptime'
来源：http://cyx.fanxiaobao.xyz

[R58] 下载文件
来源：http://cgs.nwbrower.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fbj.zdqjudy.top

[R59] 发 POST JSON
来源：http://mpb.zhijiandao.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fbc.yueranfly.top

[R60] 只看 HTTP 状态码
来源：http://crd.jinqigufen.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ecm.ydzc1.top

[R61] 磁盘占用
来源：http://gle.guowangkeji.top

df -h;  du -sh *
来源：http://qhy.mhx1999.top

[R62] 找最占空间的文件
来源：http://yat.sweek.top

du -ah . | sort -rh | head -10
来源：http://uwp.jqgufenzy.top

[R63] 内存与进程
来源：http://vbk.yueranfly.top

free -h;  ps aux | grep nginx
来源：http://qum.ydzc1.top

[R64] 结束进程
来源：http://sok.sxryk.cn

kill -9 $(pgrep -f app.py)
来源：http://igb.yj20258888.top

[R65] 查看端口占用
来源：http://tbt.jinqigfzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bxd.tianlin.xyz

[R66] 定时任务
来源：http://kbd.hysaishi.cn

crontab -e;  crontab -l
来源：http://agu.dianchejie.cn

[R67] 生成随机十六进制串
来源：http://zxg.c1oappe.top

openssl rand -hex 16
来源：http://mpw.vehdjk.com

[R68] 计算文件校验值
来源：http://ylc.xuetiantiany.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vcp.jyoumei.cn

[R69] 生成随机密码
来源：http://pqm.nanxuanxn.top

head -c 16 /dev/urandom | base64
来源：http://jti.dianchejie.cn

[R70] 时间戳与互转
来源：http://qvw.shuidangran.top

date +%s;  date -d @1700000000
来源：http://grs.zhixingplan.top

[R71] 日期格式化
来源：http://nql.yj202588.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://jiy.birdmap.top

[R72] 等待端口就绪
来源：http://ibf.316326.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://fab.shangyingyoupin.top

[R73] 分割大日志
来源：http://ijy.jinyuanbaomall.cn

split -l 1000 big.log part_
来源：http://dnw.cdnleiting.top

[R74] 批量重命名
来源：http://ztz.snrcjt.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://iwy.gaohongyu789.top

[R75] 导出环境变量
来源：http://lqc.bjfxy.top

export PATH="$HOME/bin:$PATH"
来源：http://fuh.mhx1999.top

[R76] 使用临时文件
来源：http://gcv.shuidangran.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://omw.wangdashe.top

[R77] 读取用户输入
来源：http://pet.quarkkingdee.top

read -rp "请输入: " ans
来源：http://txa.ppjwa.cn

[R78] 交互式菜单
来源：http://ikr.epnwcf.com

select opt in a b c; do echo "$opt"; break; done
来源：http://ctm.daxiang520.top

[R79] 解析命令行选项
来源：http://jvg.zdbjq.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qyo.tianlin.xyz

[R80] 查看脚本执行耗时
来源：http://vke.bjfxy.top

time ./run.sh
来源：http://api.xylfe.cn

================================================================================
来源：http://tkm.shangyingyoupin.top

S. C / C++ 专题
来源：http://mmh.jqgufenzy.top

================================================================================
来源：http://krf.yvedp.cn

[S01] C：Hello World
来源：http://oat.feifeiyinyue.top

#include <stdio.h>
来源：http://ziq.aizwys.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://utt.redwolf501.top

[S02] C：变量与格式化输出
来源：http://pav.hfpthk.cn

int a = 10; printf("%d\n", a);
来源：http://wig.jianghu66.top

[S03] C：读入整数
来源：http://hef.xinyue.icu

int x; scanf("%d", &x);
来源：http://gko.0kj1m.cn

[S04] C：字符串复制
来源：http://fhy.hongshengwenyu.top

char dst[32]; strcpy(dst, "hi");
来源：http://egr.haohaochexian.top

[S05] C：字符串长度
来源：http://xpu.hesvh.cn

strlen(s)
来源：http://hxm.epnwcf.com

[S06] C：字符串比较
来源：http://bag.vehdjk.com

strcmp(a, b) == 0
来源：http://dfj.wangshuangyany.cn

[S07] C：数组遍历求和
来源：http://eat.meibo888.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://phc.kuanghao11.cn

[S08] C：动态内存分配与释放
来源：http://xwo.shuidangran.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cja.aibaodan.cn

[S09] C：结构体定义与初始化
来源：http://udk.yonumen.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hbm.cqqwz.cn

[S10] C：指针与解引用
来源：http://sww.uphjek.com

int *p = &a;  *p = 5;
来源：http://esv.shuidangran.top

[S11] C：逐行读文件
来源：http://slx.hcnkem.com

FILE *f = fopen("a.txt", "r");
来源：http://sly.ydzc1.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ftm.yfazqb.com

fclose(f);
来源：http://cnq.yueranfly.top

[S12] C：写文件
来源：http://hgj.xinyue.icu

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ikx.quarkkingdee.top

[S13] C：宏定义
来源：http://imp.uphjek.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yvn.daria6918.cn

[S14] C：枚举
来源：http://tov.fzhhl.top

enum Color { RED, GREEN, BLUE };
来源：http://yjs.chenlongwang.top

[S15] C：类型转换
来源：http://ylv.tian-w.cn

(double) a / b
来源：http://owz.wangshuangyany.cn

[S16] C：位操作置位
来源：http://ydm.hammf.cn

x |= (1 << 3);
来源：http://pch.yueranfly.top

[S17] C：安全拼接字符串
来源：http://ueh.tarul.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://iai.quarkkingdee.top

[S18] C：命令行参数
来源：http://cam.pengpengdd.cyou

int main(int argc, char **argv)
来源：http://uqr.ehwqpu.com

[S19] C：快速排序
来源：http://dbn.xuetiantiany.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fiz.hcnkem.com

[S20] C：二分查找
来源：http://yzd.tianlin.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pkc.shangyingyoupin.top

[S21] C：字符类别判断
来源：http://mcp.ywan-chungtsiang.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ukq.zycfv.cn

[S22] C：字符串转数字
来源：http://htc.ppjwa.cn

atoi("42");  strtod("3.14", NULL);
来源：http://fyg.jlsjyb.cn

[S23] C：随机数
来源：http://hes.tianlin.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://mxi.yanxiufei.cn

[S24] C：获取本地时间
来源：http://thw.jinyuanbaomall.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mta.sjlbkw.cn

[S25] C：内存拷贝
来源：http://yow.yonumen.top

memcpy(dst, src, n);
来源：http://cpq.yongpay.top

[S26] C：内存清零
来源：http://dux.sufxvd.cn

memset(a, 0, sizeof a);
来源：http://vnu.xingfuxueyuan.xyz

[S27] C：定义常量
来源：http://dmh.cqqwz.cn

const double PI = 3.14159;
来源：http://tuz.fehbvm.com

[S28] C：静态变量
来源：http://cyq.haohaochexian.top

static int counter = 0;
来源：http://rzs.zhoulong.xyz

[S29] C：变参函数
来源：http://pkq.fehbvm.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://det.chenjidiqi.icu

[S30] C：头文件保护
来源：http://hxv.hesvh.cn

#ifndef X_H
来源：http://afs.jinghuilouyu.cn

#define X_H
来源：http://els.fktsv.cn

#endif
来源：http://omb.ybcxt.top

[S31] C++：Hello World
来源：http://afx.yongpay.top

#include <iostream>
来源：http://dus.jinyuanbaomall.cn

int main() { std::cout << "Hello\n"; }
来源：http://cho.zhijiandao.cn

[S32] C++：字符串
来源：http://jyf.tianlin.xyz

std::string s = "hi";  s += "!";
来源：http://tyl.bbcook.cn

[S33] C++：vector 增删
来源：http://jbj.shangyingyoupin.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uwo.uphjek.com

[S34] C++：遍历 vector
来源：http://ipi.yonumen.top

for (auto &x : v) { std::cout << x; }
来源：http://rav.shanyushiyangtech.top

[S35] C++：map
来源：http://csa.hywenlv.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://udy.hongshengwenyu.top

[S36] C++：unordered_map
来源：http://wdo.pengpengdd.cyou

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://grb.fktsv.cn

[S37] C++：set
来源：http://fjq.zhijiandao.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://azo.ybcxt.top

[S38] C++：排序
来源：http://jqy.yfazqb.com

std::sort(v.begin(), v.end());
来源：http://nex.jyoumei.cn

[S39] C++：自定义比较器排序
来源：http://qbl.sxryk.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://daw.dashuyun.cn

[S40] C++：查找元素
来源：http://dxv.gaohongyu789.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wmq.hnqzz.top

[S41] C++：类与构造函数
来源：http://kxs.jqgufenzy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qnz.zhongyouzk.top

[S42] C++：继承与虚函数
来源：http://wki.dashuyun.cn

class B : public Base { public: void f() override {} };
来源：http://ifu.xylfe.cn

[S43] C++：智能指针
来源：http://wek.c1oappe.top

auto p = std::make_unique<int>(5);
来源：http://avs.tanke756.top

[S44] C++：引用传参
来源：http://hdf.feifeiyinyue.top

void inc(int &x) { ++x; }
来源：http://yzl.epnwcf.com

[S45] C++：lambda
来源：http://wmx.ehwqpu.com

auto add = [](int a, int b) { return a + b; };
来源：http://knr.yuanzhike.top

[S46] C++：函数模板
来源：http://lif.chenzaomai.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://aga.jyoumei.cn

[S47] C++：结构化绑定遍历
来源：http://oww.quarkkingdee.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fpm.andypj.xyz

[S48] C++：逐行读文件
来源：http://bep.yfazqb.com

std::ifstream in("a.txt");  std::string line;
来源：http://nom.ywan-chungtsiang.top

while (std::getline(in, line)) { }
来源：http://whs.zycfv.cn

[S49] C++：写文件
来源：http://kku.0kj1m.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dhn.fehbvm.com

[S50] C++：格式化数字
来源：http://zzy.chenlongwang.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jnk.nanxuanxn.top

[S51] C++：显式类型转换
来源：http://qnk.jinqigufen.top

static_cast<double>(a) / b
来源：http://wey.zycfv.cn

[S52] C++：const 与 noexcept
来源：http://lwu.guannengcc.top

int size() const noexcept { return n_; }
来源：http://amx.jinqigufen.top

[S53] C++：移动语义
来源：http://jtd.xuetiantiany.cn

std::vector<int> w = std::move(v);
来源：http://ueo.316326.xyz

[S54] C++：异常处理
来源：http://mio.aizwys.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mmn.epnwcf.com

[S55] C++：结构化绑定
来源：http://spw.xylfe.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://adx.chenjidiqi.icu

[S56] C++：optional
来源：http://vza.chenzaomai.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bnk.jianghu66.top

[S57] C++：编译期常量
来源：http://mzn.aibaodan.cn

constexpr int N = 10;
来源：http://tvk.aibaodan.cn

[S58] C++：命名空间
来源：http://dlv.pengpengdd.cyou

namespace ns { int f() { return 1; } }
来源：http://ntt.shangyingyoupin.top

[S59] C++：静态断言
来源：http://vve.xinyue.icu

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yha.c1oappe.top

[S60] C++：遍历并删除元素
来源：http://ohf.chenlongwang.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://eqv.cheryme.top

================================================================================
来源：http://vyd.jyoumei.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vdj.hongshengwenyu.top

================================================================================
来源：http://xds.shanyushiyangtech.top

[T01] Kotlin：Hello World
来源：http://csk.yuanzhike.top

println("Hello")
来源：http://nsk.dashuyun.cn

[T02] Kotlin：变量
来源：http://svi.gaohongyu789.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wem.aizwys.cn

[T03] Kotlin：字符串模板
来源：http://bwx.jqgufenzy.top

"值: $b"
来源：http://gnl.gaohongyu789.top

[T04] Kotlin：空安全
来源：http://knc.guannengcc.top

val n: String? = null;  n?.length
来源：http://clp.cdnleiting.top

[T05] Kotlin：when 表达式
来源：http://okv.hfpthk.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://azu.jinghuilouyu.cn

[T06] Kotlin：集合映射
来源：http://waz.jinqigfzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://fgr.ppjwa.cn

[T07] Kotlin：集合过滤
来源：http://uzw.yanxiufei.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xtl.dianchejie.cn

[T08] Kotlin：数据类
来源：http://szu.guannengcc.top

data class User(val name: String, val age: Int)
来源：http://frk.ydzc1.top

[T09] Kotlin：扩展函数
来源：http://irx.sjlbkw.cn

fun String.exclaim() = this + "!"
来源：http://xzb.cdnleiting.top

[T10] Kotlin：默认参数
来源：http://clc.daxiang520.top

fun greet(name: String = "World") = "Hi $name"
来源：http://zbt.c1oappe.top

[T11] Kotlin：协程
来源：http://tsi.jqgfzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://rej.52xcode.cn

[T12] Kotlin：解构声明
来源：http://rbq.cdnleiting.top

val (a, b) = Pair(1, 2)
来源：http://pvu.zhixingplan.top

[T13] Kotlin：只读 Map
来源：http://qiz.andypj.xyz

val m = mapOf("a" to 1)
来源：http://bbz.0kj1m.cn

[T14] Kotlin：循环
来源：http://vjp.bjfxy.top

for (i in 1..10) println(i)
来源：http://anu.ivvv.top

[T15] Kotlin：接口
来源：http://jnl.sweek.top

interface Shape { fun area(): Double }
来源：http://ibo.chenjidiqi.icu

[T16] Swift：Hello World
来源：http://nqo.xingfuxueyuan.xyz

print("Hello")
来源：http://uyd.nanxinkj.top

[T17] Swift：变量与常量
来源：http://isz.yangfankeji.com

var a = 1;  let b = 2
来源：http://gky.yj202588.top

[T18] Swift：字符串插值
来源：http://bgo.chenlongwang.top

"值: \(b)"
来源：http://waj.dianchejie.cn

[T19] Swift：可选绑定
来源：http://mrj.yongpay.top

if let n = opt { print(n) }
来源：http://yre.hnqzz.top

[T20] Swift：数组操作
来源：http://sif.wangdashe.top

var a = [1, 2, 3];  a.append(4)
来源：http://pis.hcnkem.com

[T21] Swift：遍历
来源：http://bzn.ppjwa.cn

for x in a { print(x) }
来源：http://tji.zdqjudy.top

[T22] Swift：字典
来源：http://lcf.ybcxt.top

var d = ["a": 1];  d["b"] = 2
来源：http://zgz.shanyushiyangtech.top

[T23] Swift：函数
来源：http://col.gogol.net.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://egi.jinghuilouyu.cn

[T24] Swift：闭包
来源：http://qen.ppjwa.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qnx.0kj1m.cn

[T25] Swift：结构体
来源：http://mbq.kuanghao11.cn

struct P { var x: Int }
来源：http://rjn.zycfv.cn

[T26] Swift：类与重写
来源：http://gkf.jyoumei.cn

class A: Base { override func f() {} }
来源：http://xjg.uphjek.com

[T27] Swift：错误处理
来源：http://lzl.kuanghao11.cn

do { try f() } catch { print(error) }
来源：http://kbl.jiagoushi.top

[T28] Swift：枚举
来源：http://web.sxryk.cn

enum Color { case red, green }
来源：http://izd.jiagoushi.top

[T29] Swift：guard 提前返回
来源：http://tac.zhijiandao.cn

guard let x = opt else { return }
来源：http://rej.gzhubu.top

[T30] Swift：协议
来源：http://ftp.nwbrower.top

protocol Shape { func area() -> Double }
来源：http://nwi.zhixingplan.top

[T31] Lua：Hello World
来源：http://lrq.havefunace.top

print("Hello")
来源：http://hwt.cqqwz.cn

[T32] Lua：局部变量
来源：http://gfz.c1oappe.top

local a = 1
来源：http://cqs.fengsongda.top

[T33] Lua：表（数组）
来源：http://szk.yangfankeji.com

local t = {1, 2, 3};  t[4] = 4
来源：http://snt.meibo888.top

[T34] Lua：遍历表
来源：http://jen.wangshuangyany.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://cah.pengpengdd.cyou

[T35] Lua：字典表
来源：http://mhp.pycfn.com

local d = { a = 1 };  d.b = 2
来源：http://ybe.316326.xyz

[T36] Lua：函数
来源：http://efy.yj20258888.top

function add(a, b) return a + b end
来源：http://xoz.vqdsnc.cn

[T37] Lua：字符串拼接
来源：http://adb.cqqwz.cn

"a" .. "b"
来源：http://vcj.zhongyouzk.top

[T38] Lua：条件
来源：http://gku.sxryk.cn

if x > 0 then print("正") end
来源：http://lyl.tarul.cn

[T39] Lua：模式匹配
来源：http://gji.haohaochexian.top

string.find(s, "%d+")
来源：http://vgj.zdbjq.cn

[T40] Lua：元表
来源：http://yxu.birdmap.top

setmetatable({}, { __index = base })
来源：http://vnq.9152youxi.cn

[T41] Perl：Hello World
来源：http://vxj.zhixingplan.top

print "Hello\n";
来源：http://fgr.gogol.net.cn

[T42] Perl：变量类型
来源：http://zue.gotoacloud.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://whx.gogol.net.cn

[T43] Perl：字符串插值
来源：http://jmq.fehbvm.com

"值: $a"
来源：http://pbh.ehwqpu.com

[T44] Perl：条件
来源：http://nap.zhiwuduotai.top

if ($a > 0) { print "正"; }
来源：http://mji.yfazqb.com

[T45] Perl：数组遍历
来源：http://qwq.xziqi.cn

for my $x (@arr) { print $x; }
来源：http://sue.fktsv.cn

[T46] Perl：哈希操作
来源：http://tis.52xcode.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://iaa.pycfn.com

[T47] Perl：正则捕获
来源：http://kjh.pycfn.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://tdi.jinyuanbaomall.cn

[T48] Perl：正则替换
来源：http://mdd.yongpay.top

$s =~ s/old/new/g;
来源：http://bki.fanxiaobao.xyz

[T49] Perl：函数
来源：http://fej.ctjpmb.com

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pnx.yuxming.cn

[T50] Perl：逐行读文件
来源：http://bfj.iojbl.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qog.cheryme.top

while (my $line = <$fh>) { print $line; }
来源：http://acf.mhx1999.top

[T51] Scala：Hello World
来源：http://ezs.yvedp.cn

println("Hello")
来源：http://ckk.jinqigufen.top

[T52] Scala：变量
来源：http://iyd.hnqzz.top


<!-- 参考信息 -->