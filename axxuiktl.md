代发 wailian999

cmd >/dev/null 2>&1
来源：http://bsu.wangshuangyany.cn

[R42] 输入重定向
来源：http://pfp.shuidangran.top

wc -l < a.txt
来源：http://jre.zhiwuduotai.top

[R43] 按名字查找文件
来源：http://ksg.fehbvm.com

find . -name "*.log" -type f
来源：http://lrs.gaohongyu789.top

[R44] 按修改时间查找
来源：http://onk.svipenyu.cn

find . -mtime -7 -type f
来源：http://xiy.vehdjk.com

[R45] 批量删除
来源：http://kyk.meibo888.top

find . -name "*.tmp" -delete
来源：http://ree.zycfv.cn

[R46] 递归替换文件内容
来源：http://idm.yangfankeji.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dzb.havefunace.top

[R47] sed 单行替换
来源：http://lws.jinqigufen.top

sed -i 's/foo/bar/g' a.txt
来源：http://hmy.sufxvd.cn

[R48] awk 取指定列
来源：http://pul.birdmap.top

awk '{print $1, $3}' a.txt
来源：http://djc.yuxming.cn

[R49] awk 带条件
来源：http://tna.jiagoushi.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://oqs.chenjidiqi.icu

[R50] awk 求和
来源：http://twy.dianchejie.cn

awk '{s += $2} END {print s}' a.txt
来源：http://soa.ehwqpu.com

[R51] 排序去重取前几
来源：http://jtt.52xcode.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://grh.daria6918.cn

[R52] 统计行数
来源：http://ths.yonumen.top

wc -l a.txt
来源：http://fui.hysaishi.cn

[R53] 查看文件头与实时尾
来源：http://yck.zhijiandao.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vqg.jqgfzy.top

[R54] 比较两个文件
来源：http://tgg.shanyushiyangkeji.top

diff a.txt b.txt
来源：http://qqm.nwbrower.top

[R55] 压缩与解压
来源：http://fxq.feifeiyinyue.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://eyv.mhx1999.top

[R56] 远程拷贝
来源：http://rpa.sufxvd.cn

scp file user@host:/path/
来源：http://zat.fehbvm.com

[R57] 远程执行命令
来源：http://stl.xylfe.cn

ssh user@host 'uptime'
来源：http://jql.cheryme.top

[R58] 下载文件
来源：http://dcp.xingfuxueyuan.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://stb.yj20258888.top

[R59] 发 POST JSON
来源：http://bba.0kj1m.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fxo.sufxvd.cn

[R60] 只看 HTTP 状态码
来源：http://obf.shuidangran.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://eph.shanyushiyangtech.top

[R61] 磁盘占用
来源：http://mhd.vehdjk.com

df -h;  du -sh *
来源：http://npq.iojbl.cn

[R62] 找最占空间的文件
来源：http://lkb.sysykeji.top

du -ah . | sort -rh | head -10
来源：http://pwx.snrcjt.cn

[R63] 内存与进程
来源：http://xyf.mhx1999.top

free -h;  ps aux | grep nginx
来源：http://zyw.9152youxi.cn

[R64] 结束进程
来源：http://ecm.sufxvd.cn

kill -9 $(pgrep -f app.py)
来源：http://buu.dashuyun.cn

[R65] 查看端口占用
来源：http://vic.mhx1999.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rwg.aibaodan.cn

[R66] 定时任务
来源：http://asw.yanxiufei.cn

crontab -e;  crontab -l
来源：http://bnh.xuanzx.com

[R67] 生成随机十六进制串
来源：http://bew.ydzc1.top

openssl rand -hex 16
来源：http://dul.zhijiandao.cn

[R68] 计算文件校验值
来源：http://nxk.tianlin.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://hwv.jqgufenzy.top

[R69] 生成随机密码
来源：http://hbq.guannengcc.top

head -c 16 /dev/urandom | base64
来源：http://ivt.tianlin.xyz

[R70] 时间戳与互转
来源：http://xel.feifeiyinyue.top

date +%s;  date -d @1700000000
来源：http://krl.ydzc1.top

[R71] 日期格式化
来源：http://rkd.iojbl.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://uyw.aibaodan.cn

[R72] 等待端口就绪
来源：http://use.ybcxt.top

until nc -z localhost 3306; do sleep 1; done
来源：http://dmg.sweek.top

[R73] 分割大日志
来源：http://hoh.sjlbkw.cn

split -l 1000 big.log part_
来源：http://xsc.fengsongda.top

[R74] 批量重命名
来源：http://xhs.vehdjk.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://osn.mhx1999.top

[R75] 导出环境变量
来源：http://phv.sjlbkw.cn

export PATH="$HOME/bin:$PATH"
来源：http://lqj.zhixingplan.top

[R76] 使用临时文件
来源：http://dwp.cdnleiting.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wgf.iojbl.cn

[R77] 读取用户输入
来源：http://bfu.dianchejie.cn

read -rp "请输入: " ans
来源：http://sut.jiagoushi.top

[R78] 交互式菜单
来源：http://dbg.fengsongda.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ujm.feifeiyinyue.top

[R79] 解析命令行选项
来源：http://rii.hcnkem.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vpr.xziqi.cn

[R80] 查看脚本执行耗时
来源：http://ogx.zhixingplan.top

time ./run.sh
来源：http://krm.snrcjt.cn

================================================================================
来源：http://syr.gogol.net.cn

S. C / C++ 专题
来源：http://jbj.wangshuangyany.cn

================================================================================
来源：http://cbg.guannengcc.top

[S01] C：Hello World
来源：http://ras.ydjk.org.cn

#include <stdio.h>
来源：http://xmg.zhoulong.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://dar.nanxuanxn.top

[S02] C：变量与格式化输出
来源：http://tyz.tianlin.xyz

int a = 10; printf("%d\n", a);
来源：http://elw.52xcode.cn

[S03] C：读入整数
来源：http://ldy.chenlongwang.top

int x; scanf("%d", &x);
来源：http://huu.pycfn.com

[S04] C：字符串复制
来源：http://jtx.kuanghao11.cn

char dst[32]; strcpy(dst, "hi");
来源：http://jgz.ydjk.org.cn

[S05] C：字符串长度
来源：http://ltm.tarul.cn

strlen(s)
来源：http://itf.c1oappe.top

[S06] C：字符串比较
来源：http://znz.yuxming.cn

strcmp(a, b) == 0
来源：http://oyu.9152youxi.cn

[S07] C：数组遍历求和
来源：http://wig.fehbvm.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ulg.daria6918.cn

[S08] C：动态内存分配与释放
来源：http://xra.hywenlv.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jgw.0kj1m.cn

[S09] C：结构体定义与初始化
来源：http://dwb.yj20258.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://brj.c1oappe.top

[S10] C：指针与解引用
来源：http://xms.xuanzx.com

int *p = &a;  *p = 5;
来源：http://uas.cqqwz.cn

[S11] C：逐行读文件
来源：http://ags.zhoulong.xyz

FILE *f = fopen("a.txt", "r");
来源：http://boc.aibaodan.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://knx.fktsv.cn

fclose(f);
来源：http://eaq.tanke756.top

[S12] C：写文件
来源：http://twd.jyoumei.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cqg.jqgfzy.top

[S13] C：宏定义
来源：http://gad.pengpengdd.cyou

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pts.wangdashe.top

[S14] C：枚举
来源：http://ebr.smart0.xyz

enum Color { RED, GREEN, BLUE };
来源：http://rmk.uphjek.com

[S15] C：类型转换
来源：http://oce.feifeiyinyue.top

(double) a / b
来源：http://utb.aizwys.cn

[S16] C：位操作置位
来源：http://izx.jinqigfzy.top

x |= (1 << 3);
来源：http://jfj.yueranfly.top

[S17] C：安全拼接字符串
来源：http://dtn.cashguo.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uqm.fengsongda.top

[S18] C：命令行参数
来源：http://iqb.hesvh.cn

int main(int argc, char **argv)
来源：http://bgu.52xcode.cn

[S19] C：快速排序
来源：http://wxi.cucudq.cn

qsort(a, n, sizeof(int), cmp);
来源：http://yek.jqgufenzy.top

[S20] C：二分查找
来源：http://fhg.gogol.net.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://frh.gotoacloud.top

[S21] C：字符类别判断
来源：http://pmz.zhaomingkeji.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wgf.cashguo.top

[S22] C：字符串转数字
来源：http://lbn.shanyushiyangkeji.top

atoi("42");  strtod("3.14", NULL);
来源：http://our.gogol.net.cn

[S23] C：随机数
来源：http://oww.xuetiantiany.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ezf.nanxuanxn.top

[S24] C：获取本地时间
来源：http://lzk.zhijiandao.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wnc.sysykeji.top

[S25] C：内存拷贝
来源：http://qfo.shzxlz.cn

memcpy(dst, src, n);
来源：http://ygr.ydzc1.top

[S26] C：内存清零
来源：http://yqa.ctjpmb.com

memset(a, 0, sizeof a);
来源：http://ije.jyoumei.cn

[S27] C：定义常量
来源：http://uxt.zhaomingkeji.xyz

const double PI = 3.14159;
来源：http://hei.fzhhl.top

[S28] C：静态变量
来源：http://hwv.meibo888.top

static int counter = 0;
来源：http://ogx.yvedp.cn

[S29] C：变参函数
来源：http://tmn.ctjpmb.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://glt.gaohongyu789.top

[S30] C：头文件保护
来源：http://jur.fktsv.cn

#ifndef X_H
来源：http://equ.epnwcf.com

#define X_H
来源：http://ler.wangdashe.top

#endif
来源：http://pba.iojbl.cn

[S31] C++：Hello World
来源：http://nvg.yueranfly.top

#include <iostream>
来源：http://kzw.gzhubu.top

int main() { std::cout << "Hello\n"; }
来源：http://tnn.zhoulong.xyz

[S32] C++：字符串
来源：http://fib.guannengcc.top

std::string s = "hi";  s += "!";
来源：http://xis.ydjk.org.cn

[S33] C++：vector 增删
来源：http://ieq.fktsv.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tna.xingfuxueyuan.xyz

[S34] C++：遍历 vector
来源：http://bon.xuetiantiany.cn

for (auto &x : v) { std::cout << x; }
来源：http://air.zycfv.cn

[S35] C++：map
来源：http://wdn.haohaochexian.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wxm.tianlin.xyz

[S36] C++：unordered_map
来源：http://vow.dashuyun.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kvz.jianghu66.top

[S37] C++：set
来源：http://cdm.xinyue.icu

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zgd.ybcxt.top

[S38] C++：排序
来源：http://ekm.haohaochexian.top

std::sort(v.begin(), v.end());
来源：http://smo.shanyushiyangtech.top

[S39] C++：自定义比较器排序
来源：http://ksc.zhoulong.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hpa.snrcjt.cn

[S40] C++：查找元素
来源：http://vax.birdmap.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ozy.mhx1999.top

[S41] C++：类与构造函数
来源：http://cfv.yongpay.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qzs.52xcode.cn

[S42] C++：继承与虚函数
来源：http://jgo.shuidangran.top

class B : public Base { public: void f() override {} };
来源：http://osp.chenzaomai.com

[S43] C++：智能指针
来源：http://ogg.nanxuanxn.top

auto p = std::make_unique<int>(5);
来源：http://exm.aizwys.cn

[S44] C++：引用传参
来源：http://duv.zdqjudy.top

void inc(int &x) { ++x; }
来源：http://ipu.xylfe.cn

[S45] C++：lambda
来源：http://evg.shzxlz.cn

auto add = [](int a, int b) { return a + b; };
来源：http://pzz.yuanzhike.top

[S46] C++：函数模板
来源：http://myt.guannengcc.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nqt.hfpthk.cn

[S47] C++：结构化绑定遍历
来源：http://yse.jyoumei.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yiv.guannengcc.top

[S48] C++：逐行读文件
来源：http://csf.svipenyu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://weo.jinqigufen.top

while (std::getline(in, line)) { }
来源：http://hri.hesvh.cn

[S49] C++：写文件
来源：http://hiu.gogol.net.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://omu.snrcjt.cn

[S50] C++：格式化数字
来源：http://szg.gzhubu.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gdu.kuanghao11.cn

[S51] C++：显式类型转换
来源：http://pne.fzhhl.top

static_cast<double>(a) / b
来源：http://mof.jqgfzy.top

[S52] C++：const 与 noexcept
来源：http://pvn.chenzaomai.com

int size() const noexcept { return n_; }
来源：http://ocl.daxiang520.top

[S53] C++：移动语义
来源：http://ksc.chenjidiqi.icu

std::vector<int> w = std::move(v);
来源：http://dlw.fktsv.cn

[S54] C++：异常处理
来源：http://tmg.hnxiangtu.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nne.ydjk.org.cn

[S55] C++：结构化绑定
来源：http://vub.zhijiandao.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://boj.yvedp.cn

[S56] C++：optional
来源：http://vfi.yj20258888.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bzj.kuanghao11.cn

[S57] C++：编译期常量
来源：http://qew.cashguo.top

constexpr int N = 10;
来源：http://qih.aibaodan.cn

[S58] C++：命名空间
来源：http://dah.gogol.net.cn

namespace ns { int f() { return 1; } }
来源：http://dho.jqgfzy.top

[S59] C++：静态断言
来源：http://zmq.shanyushiyangtech.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://oyj.hongshengwenyu.top

[S60] C++：遍历并删除元素
来源：http://gcy.shangyingyoupin.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qou.meibo888.top

================================================================================
来源：http://ujp.cdnleiting.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wiz.sjlbkw.cn

================================================================================
来源：http://eug.redwolf501.top

[T01] Kotlin：Hello World
来源：http://kik.shanyushiyangtech.top

println("Hello")
来源：http://fpm.aizwys.cn

[T02] Kotlin：变量
来源：http://nyi.sxryk.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hrx.chenjidiqi.icu

[T03] Kotlin：字符串模板
来源：http://fnp.tarul.cn

"值: $b"
来源：http://czh.epnwcf.com

[T04] Kotlin：空安全
来源：http://yqq.jiagoushi.top

val n: String? = null;  n?.length
来源：http://wbr.shzxlz.cn

[T05] Kotlin：when 表达式
来源：http://wni.uphjek.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bsm.jiagoushi.top

[T06] Kotlin：集合映射
来源：http://ali.ywan-chungtsiang.top

listOf(1, 2, 3).map { it * 2 }
来源：http://mus.zhengqikj.top

[T07] Kotlin：集合过滤
来源：http://qdp.yangfankeji.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://iri.316326.xyz

[T08] Kotlin：数据类
来源：http://nkb.fanxiaobao.xyz

data class User(val name: String, val age: Int)
来源：http://dam.nwbrower.top

[T09] Kotlin：扩展函数
来源：http://efo.birdmap.top

fun String.exclaim() = this + "!"
来源：http://lyp.fzhhl.top

[T10] Kotlin：默认参数
来源：http://mei.ywan-chungtsiang.top

fun greet(name: String = "World") = "Hi $name"
来源：http://rrw.meibo888.top

[T11] Kotlin：协程
来源：http://pin.epnwcf.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://xoa.gotoacloud.top

[T12] Kotlin：解构声明
来源：http://ghg.wangshuangyany.cn

val (a, b) = Pair(1, 2)
来源：http://zbp.shangyingyoupin.top

[T13] Kotlin：只读 Map
来源：http://xar.yj202588.top

val m = mapOf("a" to 1)
来源：http://kuk.hammf.cn

[T14] Kotlin：循环
来源：http://ifa.9152youxi.cn

for (i in 1..10) println(i)
来源：http://drm.zdqjudy.top

[T15] Kotlin：接口
来源：http://see.fehbvm.com

interface Shape { fun area(): Double }
来源：http://rke.jinqigfzy.top

[T16] Swift：Hello World
来源：http://mrb.bjfxy.top

print("Hello")
来源：http://opw.daxiang520.top

[T17] Swift：变量与常量
来源：http://nzc.52xcode.cn

var a = 1;  let b = 2
来源：http://iac.pengpengdd.cyou

[T18] Swift：字符串插值
来源：http://dnv.jyoumei.cn

"值: \(b)"
来源：http://oxv.shanyushiyangkeji.top

[T19] Swift：可选绑定
来源：http://oek.sjlbkw.cn

if let n = opt { print(n) }
来源：http://zme.fanxiaobao.xyz

[T20] Swift：数组操作
来源：http://fzi.jyoumei.cn

var a = [1, 2, 3];  a.append(4)
来源：http://yqf.havefunace.top

[T21] Swift：遍历
来源：http://nbf.zhongyouzk.top

for x in a { print(x) }
来源：http://mnq.gaohongyu789.top

[T22] Swift：字典
来源：http://tvx.quarkkingdee.top

var d = ["a": 1];  d["b"] = 2
来源：http://qnn.dashuyun.cn

[T23] Swift：函数
来源：http://gnm.fzhhl.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://aox.yj202588.top

[T24] Swift：闭包
来源：http://qba.52xcode.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vlt.ppjwa.cn

[T25] Swift：结构体
来源：http://bmj.jinqigfzy.top

struct P { var x: Int }
来源：http://riu.ywan-chungtsiang.top

[T26] Swift：类与重写
来源：http://zus.ctjpmb.com

class A: Base { override func f() {} }
来源：http://iqe.jinqigufen.top

[T27] Swift：错误处理
来源：http://xuj.ehwqpu.com

do { try f() } catch { print(error) }
来源：http://saa.andypj.xyz

[T28] Swift：枚举
来源：http://tvz.iojbl.cn

enum Color { case red, green }
来源：http://occ.epnwcf.com

[T29] Swift：guard 提前返回
来源：http://chf.nwbrower.top

guard let x = opt else { return }
来源：http://xik.daria6918.cn

[T30] Swift：协议
来源：http://gox.jyoumei.cn

protocol Shape { func area() -> Double }
来源：http://cdr.0kj1m.cn

[T31] Lua：Hello World
来源：http://mpl.gogol.net.cn

print("Hello")
来源：http://hmb.sysykeji.top

[T32] Lua：局部变量
来源：http://kks.jinghuilouyu.cn

local a = 1
来源：http://rct.redwolf501.top

[T33] Lua：表（数组）
来源：http://ncm.tian-w.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://cls.hesvh.cn

[T34] Lua：遍历表
来源：http://cpc.cashguo.top

for i, v in ipairs(t) do print(i, v) end
来源：http://owr.jyoumei.cn

[T35] Lua：字典表
来源：http://mba.zdbjq.cn

local d = { a = 1 };  d.b = 2
来源：http://hej.fehbvm.com

[T36] Lua：函数
来源：http://rjd.xziqi.cn

function add(a, b) return a + b end
来源：http://aws.jqgfzy.top

[T37] Lua：字符串拼接
来源：http://mig.nanxuanxn.top

"a" .. "b"
来源：http://ygn.jinqigufen.top

[T38] Lua：条件
来源：http://rkq.zhiwuduotai.top

if x > 0 then print("正") end
来源：http://ezg.hesvh.cn

[T39] Lua：模式匹配
来源：http://wpb.xziqi.cn

string.find(s, "%d+")
来源：http://vdt.fktsv.cn

[T40] Lua：元表
来源：http://uan.zhijiandao.cn

setmetatable({}, { __index = base })
来源：http://cpt.guannengcc.top

[T41] Perl：Hello World
来源：http://thc.ctjpmb.com

print "Hello\n";
来源：http://hyc.gogol.net.cn

[T42] Perl：变量类型
来源：http://rhj.fzhhl.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wns.jyoumei.cn

[T43] Perl：字符串插值
来源：http://rsi.havefunace.top

"值: $a"
来源：http://why.zhixingplan.top

[T44] Perl：条件
来源：http://xzx.chenzaomai.com

if ($a > 0) { print "正"; }
来源：http://oji.jianghu66.top


<!-- 参考信息 -->