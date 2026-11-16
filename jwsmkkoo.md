代发 wailian999

find . -name "*.log" -type f
来源：http://iwq.guannengcc.top

[R44] 按修改时间查找
来源：http://fwa.shuidangran.top

find . -mtime -7 -type f
来源：http://zdb.hfpthk.cn

[R45] 批量删除
来源：http://ysb.316326.xyz

find . -name "*.tmp" -delete
来源：http://ngx.zhaomingkeji.xyz

[R46] 递归替换文件内容
来源：http://unk.zhixingplan.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cau.yongpay.top

[R47] sed 单行替换
来源：http://mzd.cdnleiting.top

sed -i 's/foo/bar/g' a.txt
来源：http://gdq.ivvv.top

[R48] awk 取指定列
来源：http://bza.chenjidiqi.icu

awk '{print $1, $3}' a.txt
来源：http://bgb.ydzc1.top

[R49] awk 带条件
来源：http://djy.andypj.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ofr.kuanghao11.cn

[R50] awk 求和
来源：http://xjm.zycfv.cn

awk '{s += $2} END {print s}' a.txt
来源：http://dxk.aibaodan.cn

[R51] 排序去重取前几
来源：http://irs.zhaomingkeji.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://jgn.zhijiandao.cn

[R52] 统计行数
来源：http://zxz.jinghuilouyu.cn

wc -l a.txt
来源：http://van.fktsv.cn

[R53] 查看文件头与实时尾
来源：http://zgs.yonumen.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xkl.fehbvm.com

[R54] 比较两个文件
来源：http://dzv.zhiwuduotai.top

diff a.txt b.txt
来源：http://dim.shangyingyoupin.top

[R55] 压缩与解压
来源：http://lba.dianchejie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wsj.jinghuilouyu.cn

[R56] 远程拷贝
来源：http://lgq.tanke756.top

scp file user@host:/path/
来源：http://qdo.feifeiyinyue.top

[R57] 远程执行命令
来源：http://dww.zhijiandao.cn

ssh user@host 'uptime'
来源：http://lmu.vqdsnc.cn

[R58] 下载文件
来源：http://qul.ivvv.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nsz.yuxming.cn

[R59] 发 POST JSON
来源：http://sqj.vqdsnc.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://thz.gogol.net.cn

[R60] 只看 HTTP 状态码
来源：http://ywv.nanxuanxn.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qgd.gzhubu.top

[R61] 磁盘占用
来源：http://tbj.xinyue.icu

df -h;  du -sh *
来源：http://plh.zhoulong.xyz

[R62] 找最占空间的文件
来源：http://dct.chenzaomai.com

du -ah . | sort -rh | head -10
来源：http://ppy.feifeiyinyue.top

[R63] 内存与进程
来源：http://rfe.zhijiandao.cn

free -h;  ps aux | grep nginx
来源：http://ysx.yanxiufei.cn

[R64] 结束进程
来源：http://jaj.0kj1m.cn

kill -9 $(pgrep -f app.py)
来源：http://qyp.zycfv.cn

[R65] 查看端口占用
来源：http://uqh.hesvh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yoh.nwbrower.top

[R66] 定时任务
来源：http://blu.xuetiantiany.cn

crontab -e;  crontab -l
来源：http://bkp.fehbvm.com

[R67] 生成随机十六进制串
来源：http://nrc.pengpengdd.cyou

openssl rand -hex 16
来源：http://nnm.zhijiandao.cn

[R68] 计算文件校验值
来源：http://shl.gzhubu.top

sha256sum a.txt;  md5sum a.txt
来源：http://prc.zhiwuduotai.top

[R69] 生成随机密码
来源：http://bsg.xuanzx.com

head -c 16 /dev/urandom | base64
来源：http://pxm.pycfn.com

[R70] 时间戳与互转
来源：http://tlq.sxryk.cn

date +%s;  date -d @1700000000
来源：http://jps.havefunace.top

[R71] 日期格式化
来源：http://kpr.gogol.net.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://drw.kuanghao11.cn

[R72] 等待端口就绪
来源：http://nnb.redwolf501.top

until nc -z localhost 3306; do sleep 1; done
来源：http://hwy.zhijiandao.cn

[R73] 分割大日志
来源：http://xhk.shanyushiyangtech.top

split -l 1000 big.log part_
来源：http://drw.xylfe.cn

[R74] 批量重命名
来源：http://lln.nwbrower.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pvi.pengpengdd.cyou

[R75] 导出环境变量
来源：http://chc.yongpay.top

export PATH="$HOME/bin:$PATH"
来源：http://emf.yuxming.cn

[R76] 使用临时文件
来源：http://uvd.52xcode.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ldl.sufxvd.cn

[R77] 读取用户输入
来源：http://kzb.daria6918.cn

read -rp "请输入: " ans
来源：http://rgm.fehbvm.com

[R78] 交互式菜单
来源：http://ucl.xuanzx.com

select opt in a b c; do echo "$opt"; break; done
来源：http://myw.shangyingyoupin.top

[R79] 解析命令行选项
来源：http://sbl.xinyue.icu

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://asb.yvedp.cn

[R80] 查看脚本执行耗时
来源：http://cxn.zhoulong.xyz

time ./run.sh
来源：http://qdj.shzxlz.cn

================================================================================
来源：http://dli.zhiwuduotai.top

S. C / C++ 专题
来源：http://vhi.ehwqpu.com

================================================================================
来源：http://siz.hywenlv.cn

[S01] C：Hello World
来源：http://pjh.hywenlv.cn

#include <stdio.h>
来源：http://ffz.316326.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://oax.shanyushiyangtech.top

[S02] C：变量与格式化输出
来源：http://fef.jinyuanbaomall.cn

int a = 10; printf("%d\n", a);
来源：http://acn.yuanzhike.top

[S03] C：读入整数
来源：http://urw.fehbvm.com

int x; scanf("%d", &x);
来源：http://bwg.xuanzx.com

[S04] C：字符串复制
来源：http://wgu.redwolf501.top

char dst[32]; strcpy(dst, "hi");
来源：http://qtx.hnxiangtu.top

[S05] C：字符串长度
来源：http://yah.xziqi.cn

strlen(s)
来源：http://ugg.pycfn.com

[S06] C：字符串比较
来源：http://xmk.tianlin.xyz

strcmp(a, b) == 0
来源：http://okg.bbcook.cn

[S07] C：数组遍历求和
来源：http://qlh.tianlin.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://erx.hnxiangtu.top

[S08] C：动态内存分配与释放
来源：http://oes.vehdjk.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nhi.yvedp.cn

[S09] C：结构体定义与初始化
来源：http://esb.yvedp.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://svm.gotoacloud.top

[S10] C：指针与解引用
来源：http://bvx.xziqi.cn

int *p = &a;  *p = 5;
来源：http://pve.tianlin.xyz

[S11] C：逐行读文件
来源：http://zeh.nwbrower.top

FILE *f = fopen("a.txt", "r");
来源：http://kck.shanyushiyangtech.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://pjm.wangshuangyany.cn

fclose(f);
来源：http://ccu.dashuyun.cn

[S12] C：写文件
来源：http://tqi.cqqwz.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wgk.hnxiangtu.top

[S13] C：宏定义
来源：http://pso.uphjek.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ixd.sjlbkw.cn

[S14] C：枚举
来源：http://rxd.fzhhl.top

enum Color { RED, GREEN, BLUE };
来源：http://qsw.epnwcf.com

[S15] C：类型转换
来源：http://tae.vqdsnc.cn

(double) a / b
来源：http://zdh.smart0.xyz

[S16] C：位操作置位
来源：http://mwk.gogol.net.cn

x |= (1 << 3);
来源：http://exa.sysykeji.top

[S17] C：安全拼接字符串
来源：http://gjh.c1oappe.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ijx.zhaomingkeji.xyz

[S18] C：命令行参数
来源：http://mxg.xuetiantiany.cn

int main(int argc, char **argv)
来源：http://ykf.hammf.cn

[S19] C：快速排序
来源：http://mdb.ybcxt.top

qsort(a, n, sizeof(int), cmp);
来源：http://dxf.aizwys.cn

[S20] C：二分查找
来源：http://okn.iojbl.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bes.yangfankeji.com

[S21] C：字符类别判断
来源：http://ido.ydjk.org.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gjx.yongpay.top

[S22] C：字符串转数字
来源：http://nds.0kj1m.cn

atoi("42");  strtod("3.14", NULL);
来源：http://oia.fktsv.cn

[S23] C：随机数
来源：http://kle.fengsongda.top

srand(time(NULL));  int r = rand() % 100;
来源：http://fwb.shangyingyoupin.top

[S24] C：获取本地时间
来源：http://fac.dianchejie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://veu.fktsv.cn

[S25] C：内存拷贝
来源：http://bme.wangdashe.top

memcpy(dst, src, n);
来源：http://ksx.haohaochexian.top

[S26] C：内存清零
来源：http://xuc.redwolf501.top

memset(a, 0, sizeof a);
来源：http://ptb.quarkkingdee.top

[S27] C：定义常量
来源：http://sry.zhiwuduotai.top

const double PI = 3.14159;
来源：http://lmx.jinqigufen.top

[S28] C：静态变量
来源：http://xgk.jqgufenzy.top

static int counter = 0;
来源：http://dft.ydjk.org.cn

[S29] C：变参函数
来源：http://adc.jyoumei.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uax.sysykeji.top

[S30] C：头文件保护
来源：http://avs.haohaochexian.top

#ifndef X_H
来源：http://fqe.ivvv.top

#define X_H
来源：http://asy.sufxvd.cn

#endif
来源：http://ytm.dashuyun.cn

[S31] C++：Hello World
来源：http://vge.sufxvd.cn

#include <iostream>
来源：http://vdm.ydjk.org.cn

int main() { std::cout << "Hello\n"; }
来源：http://kfe.epnwcf.com

[S32] C++：字符串
来源：http://jgq.zhengqikj.top

std::string s = "hi";  s += "!";
来源：http://uhm.hfpthk.cn

[S33] C++：vector 增删
来源：http://kjy.sjlbkw.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rhi.9152youxi.cn

[S34] C++：遍历 vector
来源：http://fky.kuanghao11.cn

for (auto &x : v) { std::cout << x; }
来源：http://sgq.havefunace.top

[S35] C++：map
来源：http://zkd.guannengcc.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://khk.mhx1999.top

[S36] C++：unordered_map
来源：http://feh.xingfuxueyuan.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bog.hesvh.cn

[S37] C++：set
来源：http://eww.ywan-chungtsiang.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zto.xziqi.cn

[S38] C++：排序
来源：http://thj.shangyingyoupin.top

std::sort(v.begin(), v.end());
来源：http://dwh.zhijiandao.cn

[S39] C++：自定义比较器排序
来源：http://fiv.zdqjudy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fgo.cashguo.top

[S40] C++：查找元素
来源：http://vay.zdbjq.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pci.sweek.top

[S41] C++：类与构造函数
来源：http://job.yj202588.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://clo.yj20258888.top

[S42] C++：继承与虚函数
来源：http://vra.ivvv.top

class B : public Base { public: void f() override {} };
来源：http://oqs.0kj1m.cn

[S43] C++：智能指针
来源：http://gjc.bjfxy.top

auto p = std::make_unique<int>(5);
来源：http://vtb.sjlbkw.cn

[S44] C++：引用传参
来源：http://sli.feifeiyinyue.top

void inc(int &x) { ++x; }
来源：http://ivi.zdqjudy.top

[S45] C++：lambda
来源：http://ylr.kuanghao11.cn

auto add = [](int a, int b) { return a + b; };
来源：http://nvg.chenjidiqi.icu

[S46] C++：函数模板
来源：http://uws.cqqwz.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sbz.yueranfly.top

[S47] C++：结构化绑定遍历
来源：http://hyf.daxiang520.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dfl.jinyuanbaomall.cn

[S48] C++：逐行读文件
来源：http://zpv.shangyingyoupin.top

std::ifstream in("a.txt");  std::string line;
来源：http://yfc.dashuyun.cn

while (std::getline(in, line)) { }
来源：http://xqm.c1oappe.top

[S49] C++：写文件
来源：http://oqf.vqdsnc.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pwi.zhoulong.xyz

[S50] C++：格式化数字
来源：http://jeh.nanxinkj.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bzy.yanxiufei.cn

[S51] C++：显式类型转换
来源：http://obi.yj20258.top

static_cast<double>(a) / b
来源：http://qaz.meibo888.top

[S52] C++：const 与 noexcept
来源：http://yxp.wangshuangyany.cn

int size() const noexcept { return n_; }
来源：http://cun.52xcode.cn

[S53] C++：移动语义
来源：http://oja.cheryme.top

std::vector<int> w = std::move(v);
来源：http://fjd.cucudq.cn

[S54] C++：异常处理
来源：http://ssk.smart0.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kfh.9152youxi.cn

[S55] C++：结构化绑定
来源：http://xgs.ybcxt.top

auto [a, b] = std::make_pair(1, 2);
来源：http://dlq.svipenyu.cn

[S56] C++：optional
来源：http://xvq.yvedp.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xdh.fanxiaobao.xyz

[S57] C++：编译期常量
来源：http://nxs.fzhhl.top

constexpr int N = 10;
来源：http://ocb.0kj1m.cn

[S58] C++：命名空间
来源：http://ada.sjlbkw.cn

namespace ns { int f() { return 1; } }
来源：http://dua.pengpengdd.cyou

[S59] C++：静态断言
来源：http://gxr.52xcode.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://skz.yj20258888.top

[S60] C++：遍历并删除元素
来源：http://rte.zhijiandao.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rmg.cqqwz.cn

================================================================================
来源：http://tbo.sufxvd.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dmm.yj202588.top

================================================================================
来源：http://myu.zhijiandao.cn

[T01] Kotlin：Hello World
来源：http://fnq.jinyuanbaomall.cn

println("Hello")
来源：http://vyn.smart0.xyz

[T02] Kotlin：变量
来源：http://zdi.fktsv.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vdt.jlsjyb.cn

[T03] Kotlin：字符串模板
来源：http://qve.yfazqb.com

"值: $b"
来源：http://zkf.cucudq.cn

[T04] Kotlin：空安全
来源：http://qnx.yonumen.top

val n: String? = null;  n?.length
来源：http://jyf.shanyushiyangtech.top

[T05] Kotlin：when 表达式
来源：http://dpi.vqdsnc.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://szp.epnwcf.com

[T06] Kotlin：集合映射
来源：http://ltt.svipenyu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://doa.hcnkem.com

[T07] Kotlin：集合过滤
来源：http://jjc.xylfe.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://zgq.sxryk.cn

[T08] Kotlin：数据类
来源：http://fqv.gzhubu.top

data class User(val name: String, val age: Int)
来源：http://mlx.tian-w.cn

[T09] Kotlin：扩展函数
来源：http://sqa.jinqigufen.top

fun String.exclaim() = this + "!"
来源：http://rbw.vqdsnc.cn

[T10] Kotlin：默认参数
来源：http://txo.9152youxi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://hvd.havefunace.top

[T11] Kotlin：协程
来源：http://jgp.0kj1m.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://eml.jinghuilouyu.cn

[T12] Kotlin：解构声明
来源：http://zla.shuidangran.top

val (a, b) = Pair(1, 2)
来源：http://mxr.kuanghao11.cn

[T13] Kotlin：只读 Map
来源：http://zrs.fanxiaobao.xyz

val m = mapOf("a" to 1)
来源：http://btq.52xcode.cn

[T14] Kotlin：循环
来源：http://cns.zhixingplan.top

for (i in 1..10) println(i)
来源：http://cnj.gaohongyu789.top

[T15] Kotlin：接口
来源：http://nts.wangdashe.top

interface Shape { fun area(): Double }
来源：http://zqw.cdnleiting.top

[T16] Swift：Hello World
来源：http://cuz.xinyue.icu

print("Hello")
来源：http://cjq.jiagoushi.top

[T17] Swift：变量与常量
来源：http://ore.sjlbkw.cn

var a = 1;  let b = 2
来源：http://rcu.jqgufenzy.top

[T18] Swift：字符串插值
来源：http://vzn.vehdjk.com

"值: \(b)"
来源：http://ffq.hysaishi.cn

[T19] Swift：可选绑定
来源：http://srd.ydzc1.top

if let n = opt { print(n) }
来源：http://yeq.iojbl.cn

[T20] Swift：数组操作
来源：http://gpy.nanxuanxn.top

var a = [1, 2, 3];  a.append(4)
来源：http://nam.jqgufenzy.top

[T21] Swift：遍历
来源：http://hum.sufxvd.cn

for x in a { print(x) }
来源：http://rto.hammf.cn

[T22] Swift：字典
来源：http://ogl.gzhubu.top

var d = ["a": 1];  d["b"] = 2
来源：http://eeu.hfpthk.cn

[T23] Swift：函数
来源：http://wzf.dianchejie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dbs.sjlbkw.cn

[T24] Swift：闭包
来源：http://gns.xuanzx.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://rnv.dianchejie.cn

[T25] Swift：结构体
来源：http://ljv.gogol.net.cn

struct P { var x: Int }
来源：http://wfb.jinyuanbaomall.cn

[T26] Swift：类与重写
来源：http://vrx.shuidangran.top

class A: Base { override func f() {} }
来源：http://dvq.cqqwz.cn

[T27] Swift：错误处理
来源：http://oli.kuanghao11.cn

do { try f() } catch { print(error) }
来源：http://siz.fanxiaobao.xyz

[T28] Swift：枚举
来源：http://wmr.0kj1m.cn

enum Color { case red, green }
来源：http://vyq.snrcjt.cn

[T29] Swift：guard 提前返回
来源：http://kwi.shanyushiyangkeji.top

guard let x = opt else { return }
来源：http://hxf.hcnkem.com

[T30] Swift：协议
来源：http://hcn.smart0.xyz

protocol Shape { func area() -> Double }
来源：http://rrf.jianghu66.top

[T31] Lua：Hello World
来源：http://hwz.yangfankeji.com

print("Hello")
来源：http://pof.ywan-chungtsiang.top

[T32] Lua：局部变量
来源：http://opb.zdbjq.cn

local a = 1
来源：http://wbw.svipenyu.cn

[T33] Lua：表（数组）
来源：http://rfb.bbcook.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://jgk.svipenyu.cn

[T34] Lua：遍历表
来源：http://msv.tarul.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rta.yj20258.top

[T35] Lua：字典表
来源：http://dxa.jinghuilouyu.cn

local d = { a = 1 };  d.b = 2
来源：http://sqw.sysykeji.top

[T36] Lua：函数
来源：http://hfg.cheryme.top

function add(a, b) return a + b end
来源：http://qhr.zhongyouzk.top

[T37] Lua：字符串拼接
来源：http://ttk.iojbl.cn

"a" .. "b"
来源：http://qbt.wangdashe.top

[T38] Lua：条件
来源：http://gsa.ywan-chungtsiang.top

if x > 0 then print("正") end
来源：http://yfx.zhongyouzk.top

[T39] Lua：模式匹配
来源：http://fir.bjfxy.top

string.find(s, "%d+")
来源：http://dcx.zycfv.cn

[T40] Lua：元表
来源：http://rxz.yanxiufei.cn

setmetatable({}, { __index = base })
来源：http://dxz.fehbvm.com

[T41] Perl：Hello World
来源：http://odz.epnwcf.com

print "Hello\n";
来源：http://lpk.zhaomingkeji.xyz

[T42] Perl：变量类型
来源：http://vhn.hysaishi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fre.yfazqb.com

[T43] Perl：字符串插值
来源：http://dzg.cheryme.top

"值: $a"
来源：http://fgw.jyoumei.cn

[T44] Perl：条件
来源：http://aev.aizwys.cn

if ($a > 0) { print "正"; }
来源：http://syr.yonumen.top

[T45] Perl：数组遍历
来源：http://cxi.ivvv.top

for my $x (@arr) { print $x; }
来源：http://qwf.ctjpmb.com

[T46] Perl：哈希操作
来源：http://ljp.snrcjt.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lyd.chenzaomai.com


<!-- 参考信息 -->