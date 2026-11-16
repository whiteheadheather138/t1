代发 wailian999

cmd > out.log 2>&1
来源：http://isj.shangyingyoupin.top

[R40] 追加写日志
来源：http://ekk.ppjwa.cn

echo "log" >> out.log
来源：http://tac.9152youxi.cn

[R41] 丢弃输出
来源：http://xiz.ywan-chungtsiang.top

cmd >/dev/null 2>&1
来源：http://rnc.zycfv.cn

[R42] 输入重定向
来源：http://rzq.xylfe.cn

wc -l < a.txt
来源：http://jzk.chenzaomai.com

[R43] 按名字查找文件
来源：http://odq.hywenlv.cn

find . -name "*.log" -type f
来源：http://yxe.tianlin.xyz

[R44] 按修改时间查找
来源：http://gse.aibaodan.cn

find . -mtime -7 -type f
来源：http://ooa.daria6918.cn

[R45] 批量删除
来源：http://lnf.tian-w.cn

find . -name "*.tmp" -delete
来源：http://hrb.fengsongda.top

[R46] 递归替换文件内容
来源：http://azh.xziqi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jrv.zdqjudy.top

[R47] sed 单行替换
来源：http://fys.epnwcf.com

sed -i 's/foo/bar/g' a.txt
来源：http://sjz.jlsjyb.cn

[R48] awk 取指定列
来源：http://wzu.yj20258888.top

awk '{print $1, $3}' a.txt
来源：http://ykf.zhaomingkeji.xyz

[R49] awk 带条件
来源：http://ihh.zycfv.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gyb.jinqigufen.top

[R50] awk 求和
来源：http://nwy.yuanzhike.top

awk '{s += $2} END {print s}' a.txt
来源：http://lpa.yfazqb.com

[R51] 排序去重取前几
来源：http://lnp.daxiang520.top

sort a.txt | uniq -c | sort -rn | head
来源：http://cyl.fehbvm.com

[R52] 统计行数
来源：http://dyy.chenjidiqi.icu

wc -l a.txt
来源：http://xnx.vehdjk.com

[R53] 查看文件头与实时尾
来源：http://ekb.iojbl.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qjw.hammf.cn

[R54] 比较两个文件
来源：http://gyx.vqdsnc.cn

diff a.txt b.txt
来源：http://mbm.zhixingplan.top

[R55] 压缩与解压
来源：http://zoc.yonumen.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ytp.shanyushiyangtech.top

[R56] 远程拷贝
来源：http://zrc.ppjwa.cn

scp file user@host:/path/
来源：http://aig.uphjek.com

[R57] 远程执行命令
来源：http://ldi.guowangkeji.top

ssh user@host 'uptime'
来源：http://dpr.zdqjudy.top

[R58] 下载文件
来源：http://zqh.chenlongwang.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uur.0kj1m.cn

[R59] 发 POST JSON
来源：http://zri.fzhhl.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zmh.uphjek.com

[R60] 只看 HTTP 状态码
来源：http://zir.pycfn.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jbw.fehbvm.com

[R61] 磁盘占用
来源：http://aga.yj20258.top

df -h;  du -sh *
来源：http://cnw.yfazqb.com

[R62] 找最占空间的文件
来源：http://uep.jlsjyb.cn

du -ah . | sort -rh | head -10
来源：http://nkp.ctjpmb.com

[R63] 内存与进程
来源：http://utw.zdqjudy.top

free -h;  ps aux | grep nginx
来源：http://kgz.yueranfly.top

[R64] 结束进程
来源：http://ajq.hnxiangtu.top

kill -9 $(pgrep -f app.py)
来源：http://wgn.hysaishi.cn

[R65] 查看端口占用
来源：http://vxj.ctjpmb.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ykw.jinyuanbaomall.cn

[R66] 定时任务
来源：http://ixj.jyoumei.cn

crontab -e;  crontab -l
来源：http://csy.hysaishi.cn

[R67] 生成随机十六进制串
来源：http://usw.bjfxy.top

openssl rand -hex 16
来源：http://gfr.sysykeji.top

[R68] 计算文件校验值
来源：http://ijp.aibaodan.cn

sha256sum a.txt;  md5sum a.txt
来源：http://rpi.cqqwz.cn

[R69] 生成随机密码
来源：http://ygz.hesvh.cn

head -c 16 /dev/urandom | base64
来源：http://fyk.xingfuxueyuan.xyz

[R70] 时间戳与互转
来源：http://sdi.cheryme.top

date +%s;  date -d @1700000000
来源：http://qhl.fanxiaobao.xyz

[R71] 日期格式化
来源：http://tri.cucudq.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://juq.sysykeji.top

[R72] 等待端口就绪
来源：http://anz.zhaomingkeji.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://sci.sweek.top

[R73] 分割大日志
来源：http://car.zhoulong.xyz

split -l 1000 big.log part_
来源：http://qmr.yuanzhike.top

[R74] 批量重命名
来源：http://osj.havefunace.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dqk.yanxiufei.cn

[R75] 导出环境变量
来源：http://wkr.sxryk.cn

export PATH="$HOME/bin:$PATH"
来源：http://kov.birdmap.top

[R76] 使用临时文件
来源：http://lmu.jinghuilouyu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rpb.nanxinkj.top

[R77] 读取用户输入
来源：http://jva.vehdjk.com

read -rp "请输入: " ans
来源：http://toj.hywenlv.cn

[R78] 交互式菜单
来源：http://igi.hywenlv.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nig.hesvh.cn

[R79] 解析命令行选项
来源：http://xgm.uphjek.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://oew.yvedp.cn

[R80] 查看脚本执行耗时
来源：http://qcv.gaohongyu789.top

time ./run.sh
来源：http://kru.hammf.cn

================================================================================
来源：http://mpg.pengpengdd.cyou

S. C / C++ 专题
来源：http://kic.gotoacloud.top

================================================================================
来源：http://fgh.vehdjk.com

[S01] C：Hello World
来源：http://jgi.cucudq.cn

#include <stdio.h>
来源：http://ntf.chenzaomai.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://mdl.xuanzx.com

[S02] C：变量与格式化输出
来源：http://zlq.316326.xyz

int a = 10; printf("%d\n", a);
来源：http://wvh.hysaishi.cn

[S03] C：读入整数
来源：http://lbu.daxiang520.top

int x; scanf("%d", &x);
来源：http://gjo.jinqigfzy.top

[S04] C：字符串复制
来源：http://grt.yj202588.top

char dst[32]; strcpy(dst, "hi");
来源：http://adw.yj20258888.top

[S05] C：字符串长度
来源：http://ksf.fktsv.cn

strlen(s)
来源：http://ccv.xinyue.icu

[S06] C：字符串比较
来源：http://eff.nwbrower.top

strcmp(a, b) == 0
来源：http://bsa.jinyuanbaomall.cn

[S07] C：数组遍历求和
来源：http://zon.tian-w.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rmq.dianchejie.cn

[S08] C：动态内存分配与释放
来源：http://mrz.fzhhl.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gts.cashguo.top

[S09] C：结构体定义与初始化
来源：http://dwf.9152youxi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cut.tarul.cn

[S10] C：指针与解引用
来源：http://fht.haohaochexian.top

int *p = &a;  *p = 5;
来源：http://ano.shanyushiyangtech.top

[S11] C：逐行读文件
来源：http://dhh.fktsv.cn

FILE *f = fopen("a.txt", "r");
来源：http://qmz.jinghuilouyu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xgk.shanyushiyangkeji.top

fclose(f);
来源：http://dce.9152youxi.cn

[S12] C：写文件
来源：http://iym.gogol.net.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nfv.sxryk.cn

[S13] C：宏定义
来源：http://uxy.smart0.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cus.cucudq.cn

[S14] C：枚举
来源：http://uyu.hnxiangtu.top

enum Color { RED, GREEN, BLUE };
来源：http://amo.sysykeji.top

[S15] C：类型转换
来源：http://eey.jiagoushi.top

(double) a / b
来源：http://cbg.chenzaomai.com

[S16] C：位操作置位
来源：http://vsu.sjlbkw.cn

x |= (1 << 3);
来源：http://qgi.zhiwuduotai.top

[S17] C：安全拼接字符串
来源：http://uxy.yj20258888.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ahj.hnqzz.top

[S18] C：命令行参数
来源：http://tnc.andypj.xyz

int main(int argc, char **argv)
来源：http://xpl.ywan-chungtsiang.top

[S19] C：快速排序
来源：http://nlo.c1oappe.top

qsort(a, n, sizeof(int), cmp);
来源：http://zwq.sysykeji.top

[S20] C：二分查找
来源：http://gtp.jinqigufen.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gxb.hfpthk.cn

[S21] C：字符类别判断
来源：http://fuc.chenzaomai.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://uak.sysykeji.top

[S22] C：字符串转数字
来源：http://lfl.yongpay.top

atoi("42");  strtod("3.14", NULL);
来源：http://ofm.iojbl.cn

[S23] C：随机数
来源：http://efg.gaohongyu789.top

srand(time(NULL));  int r = rand() % 100;
来源：http://hmq.aizwys.cn

[S24] C：获取本地时间
来源：http://zht.dashuyun.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gws.guowangkeji.top

[S25] C：内存拷贝
来源：http://awf.jinyuanbaomall.cn

memcpy(dst, src, n);
来源：http://gwo.fehbvm.com

[S26] C：内存清零
来源：http://mjx.daxiang520.top

memset(a, 0, sizeof a);
来源：http://vpp.jlsjyb.cn

[S27] C：定义常量
来源：http://dfh.0kj1m.cn

const double PI = 3.14159;
来源：http://mme.guannengcc.top

[S28] C：静态变量
来源：http://kxp.daria6918.cn

static int counter = 0;
来源：http://okx.snrcjt.cn

[S29] C：变参函数
来源：http://kee.gogol.net.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qlk.mhx1999.top

[S30] C：头文件保护
来源：http://icw.guowangkeji.top

#ifndef X_H
来源：http://miy.yonumen.top

#define X_H
来源：http://ise.mhx1999.top

#endif
来源：http://gvu.yfazqb.com

[S31] C++：Hello World
来源：http://bbo.zhiwuduotai.top

#include <iostream>
来源：http://qvv.ydjk.org.cn

int main() { std::cout << "Hello\n"; }
来源：http://rkq.xinyue.icu

[S32] C++：字符串
来源：http://zhe.cdnleiting.top

std::string s = "hi";  s += "!";
来源：http://wap.zhixingplan.top

[S33] C++：vector 增删
来源：http://tvz.yonumen.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://joj.xuanzx.com

[S34] C++：遍历 vector
来源：http://mav.havefunace.top

for (auto &x : v) { std::cout << x; }
来源：http://gei.zycfv.cn

[S35] C++：map
来源：http://kbl.wangdashe.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lpz.gaohongyu789.top

[S36] C++：unordered_map
来源：http://jvl.c1oappe.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rkh.ctjpmb.com

[S37] C++：set
来源：http://bqv.ydzc1.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jtt.jlsjyb.cn

[S38] C++：排序
来源：http://uzj.yonumen.top

std::sort(v.begin(), v.end());
来源：http://kug.vqdsnc.cn

[S39] C++：自定义比较器排序
来源：http://set.cheryme.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zri.cheryme.top

[S40] C++：查找元素
来源：http://ncm.pycfn.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yoz.jinyuanbaomall.cn

[S41] C++：类与构造函数
来源：http://dar.yj20258888.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fdr.jinqigufen.top

[S42] C++：继承与虚函数
来源：http://pgc.daria6918.cn

class B : public Base { public: void f() override {} };
来源：http://jev.hfpthk.cn

[S43] C++：智能指针
来源：http://vzn.jiagoushi.top

auto p = std::make_unique<int>(5);
来源：http://snt.ppjwa.cn

[S44] C++：引用传参
来源：http://lis.xuetiantiany.cn

void inc(int &x) { ++x; }
来源：http://zyh.yj202588.top

[S45] C++：lambda
来源：http://far.sufxvd.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hkx.xuanzx.com

[S46] C++：函数模板
来源：http://rvh.aibaodan.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jlx.cqqwz.cn

[S47] C++：结构化绑定遍历
来源：http://oxr.zhiwuduotai.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ghz.9152youxi.cn

[S48] C++：逐行读文件
来源：http://goy.zhengqikj.top

std::ifstream in("a.txt");  std::string line;
来源：http://suu.sufxvd.cn

while (std::getline(in, line)) { }
来源：http://hhn.vehdjk.com

[S49] C++：写文件
来源：http://mjg.xuetiantiany.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ydl.hammf.cn

[S50] C++：格式化数字
来源：http://ghd.fktsv.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ayo.sweek.top

[S51] C++：显式类型转换
来源：http://rll.ppjwa.cn

static_cast<double>(a) / b
来源：http://qzc.yonumen.top

[S52] C++：const 与 noexcept
来源：http://dgi.smart0.xyz

int size() const noexcept { return n_; }
来源：http://ylr.yueranfly.top

[S53] C++：移动语义
来源：http://jpe.ydzc1.top

std::vector<int> w = std::move(v);
来源：http://zwr.yongpay.top

[S54] C++：异常处理
来源：http://ftd.snrcjt.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://evx.bjfxy.top

[S55] C++：结构化绑定
来源：http://ero.daria6918.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://oxv.chenjidiqi.icu

[S56] C++：optional
来源：http://zef.fzhhl.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lzm.dianchejie.cn

[S57] C++：编译期常量
来源：http://vuo.xuanzx.com

constexpr int N = 10;
来源：http://hjg.yj20258888.top

[S58] C++：命名空间
来源：http://ref.yonumen.top

namespace ns { int f() { return 1; } }
来源：http://hxr.shangyingyoupin.top

[S59] C++：静态断言
来源：http://plv.chenzaomai.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pzf.jqgfzy.top

[S60] C++：遍历并删除元素
来源：http://naf.vehdjk.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ogb.shzxlz.cn

================================================================================
来源：http://bvk.hammf.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://buc.fehbvm.com

================================================================================
来源：http://bgm.jinyuanbaomall.cn

[T01] Kotlin：Hello World
来源：http://hqx.guannengcc.top

println("Hello")
来源：http://lxg.xingfuxueyuan.xyz

[T02] Kotlin：变量
来源：http://aoq.xziqi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ybr.fengsongda.top

[T03] Kotlin：字符串模板
来源：http://gkt.birdmap.top

"值: $b"
来源：http://bqc.shangyingyoupin.top

[T04] Kotlin：空安全
来源：http://efz.hysaishi.cn

val n: String? = null;  n?.length
来源：http://vjk.52xcode.cn

[T05] Kotlin：when 表达式
来源：http://sxp.hcnkem.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jfe.snrcjt.cn

[T06] Kotlin：集合映射
来源：http://avy.aizwys.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://pgi.hysaishi.cn

[T07] Kotlin：集合过滤
来源：http://uuo.ctjpmb.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://hkj.yongpay.top

[T08] Kotlin：数据类
来源：http://jsr.jinqigufen.top

data class User(val name: String, val age: Int)
来源：http://igw.ppjwa.cn

[T09] Kotlin：扩展函数
来源：http://uha.hysaishi.cn

fun String.exclaim() = this + "!"
来源：http://ndk.ybcxt.top

[T10] Kotlin：默认参数
来源：http://pge.haohaochexian.top

fun greet(name: String = "World") = "Hi $name"
来源：http://aoc.xylfe.cn

[T11] Kotlin：协程
来源：http://zix.daria6918.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://mda.ybcxt.top

[T12] Kotlin：解构声明
来源：http://shs.zhijiandao.cn

val (a, b) = Pair(1, 2)
来源：http://opw.hcnkem.com

[T13] Kotlin：只读 Map
来源：http://ugk.sysykeji.top

val m = mapOf("a" to 1)
来源：http://fri.jyoumei.cn

[T14] Kotlin：循环
来源：http://kno.ybcxt.top

for (i in 1..10) println(i)
来源：http://lun.yuanzhike.top

[T15] Kotlin：接口
来源：http://jno.hnqzz.top

interface Shape { fun area(): Double }
来源：http://bgb.ydjk.org.cn

[T16] Swift：Hello World
来源：http://rhz.zdqjudy.top

print("Hello")
来源：http://hgg.nanxuanxn.top

[T17] Swift：变量与常量
来源：http://sga.chenjidiqi.icu

var a = 1;  let b = 2
来源：http://bav.gzhubu.top

[T18] Swift：字符串插值
来源：http://jzk.ivvv.top

"值: \(b)"
来源：http://rxz.xuetiantiany.cn

[T19] Swift：可选绑定
来源：http://qic.ywan-chungtsiang.top

if let n = opt { print(n) }
来源：http://rgi.chenlongwang.top

[T20] Swift：数组操作
来源：http://siw.sjlbkw.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qsn.meibo888.top

[T21] Swift：遍历
来源：http://vor.yj20258.top

for x in a { print(x) }
来源：http://hnl.chenlongwang.top

[T22] Swift：字典
来源：http://oqp.xuanzx.com

var d = ["a": 1];  d["b"] = 2
来源：http://nuq.yongpay.top

[T23] Swift：函数
来源：http://nfp.gzhubu.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ijj.yueranfly.top

[T24] Swift：闭包
来源：http://pxn.zdbjq.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://msz.gogol.net.cn

[T25] Swift：结构体
来源：http://uyi.xylfe.cn

struct P { var x: Int }
来源：http://kjv.gzhubu.top

[T26] Swift：类与重写
来源：http://xnr.cucudq.cn

class A: Base { override func f() {} }
来源：http://emn.yuanzhike.top

[T27] Swift：错误处理
来源：http://bjg.chenzaomai.com

do { try f() } catch { print(error) }
来源：http://hyw.gogol.net.cn

[T28] Swift：枚举
来源：http://git.jinghuilouyu.cn

enum Color { case red, green }
来源：http://ibp.zdbjq.cn

[T29] Swift：guard 提前返回
来源：http://wwy.yvedp.cn

guard let x = opt else { return }
来源：http://hdy.xziqi.cn

[T30] Swift：协议
来源：http://rtz.zdqjudy.top

protocol Shape { func area() -> Double }
来源：http://xzj.tarul.cn

[T31] Lua：Hello World
来源：http://emd.sxryk.cn

print("Hello")
来源：http://xre.snrcjt.cn

[T32] Lua：局部变量
来源：http://krz.nanxuanxn.top

local a = 1
来源：http://rym.sufxvd.cn

[T33] Lua：表（数组）
来源：http://fno.wangshuangyany.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://yct.vehdjk.com

[T34] Lua：遍历表
来源：http://qqv.ctjpmb.com

for i, v in ipairs(t) do print(i, v) end
来源：http://puv.shanyushiyangkeji.top

[T35] Lua：字典表
来源：http://ltw.hcnkem.com

local d = { a = 1 };  d.b = 2
来源：http://ufb.shangyingyoupin.top

[T36] Lua：函数
来源：http://ctx.sufxvd.cn

function add(a, b) return a + b end
来源：http://snm.hnqzz.top

[T37] Lua：字符串拼接
来源：http://skv.xuanzx.com

"a" .. "b"
来源：http://rjg.bbcook.cn

[T38] Lua：条件
来源：http://yzh.jiagoushi.top

if x > 0 then print("正") end
来源：http://ksm.tanke756.top

[T39] Lua：模式匹配
来源：http://tsf.sweek.top

string.find(s, "%d+")
来源：http://use.vehdjk.com

[T40] Lua：元表
来源：http://xdo.jqgfzy.top

setmetatable({}, { __index = base })
来源：http://zti.bjfxy.top

[T41] Perl：Hello World
来源：http://qcw.dianchejie.cn

print "Hello\n";
来源：http://ils.tian-w.cn

[T42] Perl：变量类型
来源：http://ffn.gzhubu.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ijn.hongshengwenyu.top


<!-- 参考信息 -->