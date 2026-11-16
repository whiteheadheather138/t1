代发 wailian999

find . -name "*.log" -type f
来源：http://miy.bjfxy.top

[R44] 按修改时间查找
来源：http://eha.ivvv.top

find . -mtime -7 -type f
来源：http://lft.zhiwuduotai.top

[R45] 批量删除
来源：http://tcb.9152youxi.cn

find . -name "*.tmp" -delete
来源：http://cbn.wangshuangyany.cn

[R46] 递归替换文件内容
来源：http://gec.c1oappe.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fjn.daria6918.cn

[R47] sed 单行替换
来源：http://ijq.zdbjq.cn

sed -i 's/foo/bar/g' a.txt
来源：http://pwr.nwbrower.top

[R48] awk 取指定列
来源：http://ltp.0kj1m.cn

awk '{print $1, $3}' a.txt
来源：http://glj.yongpay.top

[R49] awk 带条件
来源：http://foq.pycfn.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dtk.jinqigufen.top

[R50] awk 求和
来源：http://pke.yj202588.top

awk '{s += $2} END {print s}' a.txt
来源：http://ecy.ehwqpu.com

[R51] 排序去重取前几
来源：http://vkr.hammf.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://zcm.zhengqikj.top

[R52] 统计行数
来源：http://agl.haohaochexian.top

wc -l a.txt
来源：http://usp.zhixingplan.top

[R53] 查看文件头与实时尾
来源：http://hcz.cdnleiting.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jms.cucudq.cn

[R54] 比较两个文件
来源：http://yip.guannengcc.top

diff a.txt b.txt
来源：http://rze.dianchejie.cn

[R55] 压缩与解压
来源：http://ulo.ivvv.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cgn.hesvh.cn

[R56] 远程拷贝
来源：http://opf.guowangkeji.top

scp file user@host:/path/
来源：http://com.kuanghao11.cn

[R57] 远程执行命令
来源：http://jgz.svipenyu.cn

ssh user@host 'uptime'
来源：http://xyl.hfpthk.cn

[R58] 下载文件
来源：http://wgr.zhengqikj.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ylg.zycfv.cn

[R59] 发 POST JSON
来源：http://tfa.hesvh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ife.wangdashe.top

[R60] 只看 HTTP 状态码
来源：http://jor.zdqjudy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qzs.birdmap.top

[R61] 磁盘占用
来源：http://ooc.sxryk.cn

df -h;  du -sh *
来源：http://pta.dashuyun.cn

[R62] 找最占空间的文件
来源：http://hxn.jqgfzy.top

du -ah . | sort -rh | head -10
来源：http://uvz.daxiang520.top

[R63] 内存与进程
来源：http://owm.yuxming.cn

free -h;  ps aux | grep nginx
来源：http://xop.wangshuangyany.cn

[R64] 结束进程
来源：http://eca.guowangkeji.top

kill -9 $(pgrep -f app.py)
来源：http://lqf.andypj.xyz

[R65] 查看端口占用
来源：http://wsc.tanke756.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ynn.0kj1m.cn

[R66] 定时任务
来源：http://rfb.yvedp.cn

crontab -e;  crontab -l
来源：http://wnt.ydzc1.top

[R67] 生成随机十六进制串
来源：http://rti.zhaomingkeji.xyz

openssl rand -hex 16
来源：http://dml.vqdsnc.cn

[R68] 计算文件校验值
来源：http://nuw.xuanzx.com

sha256sum a.txt;  md5sum a.txt
来源：http://lpo.iojbl.cn

[R69] 生成随机密码
来源：http://xzr.iojbl.cn

head -c 16 /dev/urandom | base64
来源：http://vek.0kj1m.cn

[R70] 时间戳与互转
来源：http://ucb.andypj.xyz

date +%s;  date -d @1700000000
来源：http://rlk.yanxiufei.cn

[R71] 日期格式化
来源：http://hqc.ctjpmb.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://ydh.kuanghao11.cn

[R72] 等待端口就绪
来源：http://pbh.cqqwz.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qfx.xuanzx.com

[R73] 分割大日志
来源：http://vra.fengsongda.top

split -l 1000 big.log part_
来源：http://psh.ctjpmb.com

[R74] 批量重命名
来源：http://pki.9152youxi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kgv.sufxvd.cn

[R75] 导出环境变量
来源：http://rzw.yj202588.top

export PATH="$HOME/bin:$PATH"
来源：http://ojz.sufxvd.cn

[R76] 使用临时文件
来源：http://eih.sjlbkw.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vqt.svipenyu.cn

[R77] 读取用户输入
来源：http://ult.zdqjudy.top

read -rp "请输入: " ans
来源：http://fpq.sufxvd.cn

[R78] 交互式菜单
来源：http://fhj.tanke756.top

select opt in a b c; do echo "$opt"; break; done
来源：http://yra.smart0.xyz

[R79] 解析命令行选项
来源：http://jbt.nwbrower.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wju.fehbvm.com

[R80] 查看脚本执行耗时
来源：http://yvp.jqgfzy.top

time ./run.sh
来源：http://cat.hcnkem.com

================================================================================
来源：http://yjx.yfazqb.com

S. C / C++ 专题
来源：http://xwi.tarul.cn

================================================================================
来源：http://yda.hesvh.cn

[S01] C：Hello World
来源：http://bni.ehwqpu.com

#include <stdio.h>
来源：http://utf.fktsv.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ido.guannengcc.top

[S02] C：变量与格式化输出
来源：http://gdv.zycfv.cn

int a = 10; printf("%d\n", a);
来源：http://fme.yvedp.cn

[S03] C：读入整数
来源：http://gju.gogol.net.cn

int x; scanf("%d", &x);
来源：http://yzn.sufxvd.cn

[S04] C：字符串复制
来源：http://yai.dashuyun.cn

char dst[32]; strcpy(dst, "hi");
来源：http://igl.yuanzhike.top

[S05] C：字符串长度
来源：http://isr.bbcook.cn

strlen(s)
来源：http://nax.dianchejie.cn

[S06] C：字符串比较
来源：http://bft.yanxiufei.cn

strcmp(a, b) == 0
来源：http://pvm.jianghu66.top

[S07] C：数组遍历求和
来源：http://ncg.zhiwuduotai.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bdo.hesvh.cn

[S08] C：动态内存分配与释放
来源：http://rqd.yongpay.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ynh.svipenyu.cn

[S09] C：结构体定义与初始化
来源：http://ecu.bbcook.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://enz.fanxiaobao.xyz

[S10] C：指针与解引用
来源：http://kjw.yuanzhike.top

int *p = &a;  *p = 5;
来源：http://wei.hnqzz.top

[S11] C：逐行读文件
来源：http://fpj.hcnkem.com

FILE *f = fopen("a.txt", "r");
来源：http://ous.shanyushiyangtech.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://uho.bbcook.cn

fclose(f);
来源：http://hbu.iojbl.cn

[S12] C：写文件
来源：http://cwm.sweek.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nlb.zhiwuduotai.top

[S13] C：宏定义
来源：http://ngs.sysykeji.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xap.yangfankeji.com

[S14] C：枚举
来源：http://vup.dianchejie.cn

enum Color { RED, GREEN, BLUE };
来源：http://pvc.ehwqpu.com

[S15] C：类型转换
来源：http://gsr.shzxlz.cn

(double) a / b
来源：http://vdg.wangshuangyany.cn

[S16] C：位操作置位
来源：http://doq.fzhhl.top

x |= (1 << 3);
来源：http://fik.hongshengwenyu.top

[S17] C：安全拼接字符串
来源：http://ftr.shanyushiyangkeji.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nxy.tanke756.top

[S18] C：命令行参数
来源：http://ztv.guannengcc.top

int main(int argc, char **argv)
来源：http://bwi.smart0.xyz

[S19] C：快速排序
来源：http://snz.zhoulong.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://srh.quarkkingdee.top

[S20] C：二分查找
来源：http://wnw.shangyingyoupin.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vwo.zhengqikj.top

[S21] C：字符类别判断
来源：http://crx.bjfxy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ujq.shanyushiyangtech.top

[S22] C：字符串转数字
来源：http://vak.gogol.net.cn

atoi("42");  strtod("3.14", NULL);
来源：http://usb.hcnkem.com

[S23] C：随机数
来源：http://hpg.52xcode.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://tbh.sweek.top

[S24] C：获取本地时间
来源：http://rhk.shzxlz.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ygk.yueranfly.top

[S25] C：内存拷贝
来源：http://wng.ctjpmb.com

memcpy(dst, src, n);
来源：http://xtv.zdqjudy.top

[S26] C：内存清零
来源：http://emo.hcnkem.com

memset(a, 0, sizeof a);
来源：http://rer.bbcook.cn

[S27] C：定义常量
来源：http://dhy.yj202588.top

const double PI = 3.14159;
来源：http://iuc.yuanzhike.top

[S28] C：静态变量
来源：http://pxl.hammf.cn

static int counter = 0;
来源：http://zsw.yonumen.top

[S29] C：变参函数
来源：http://yfs.zhiwuduotai.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kgk.xuanzx.com

[S30] C：头文件保护
来源：http://rwr.jiagoushi.top

#ifndef X_H
来源：http://odg.ydjk.org.cn

#define X_H
来源：http://tpo.ivvv.top

#endif
来源：http://qmv.smart0.xyz

[S31] C++：Hello World
来源：http://kkj.yonumen.top

#include <iostream>
来源：http://jlv.ehwqpu.com

int main() { std::cout << "Hello\n"; }
来源：http://etw.jlsjyb.cn

[S32] C++：字符串
来源：http://skp.fzhhl.top

std::string s = "hi";  s += "!";
来源：http://xyh.andypj.xyz

[S33] C++：vector 增删
来源：http://kho.fktsv.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jge.hysaishi.cn

[S34] C++：遍历 vector
来源：http://tia.fzhhl.top

for (auto &x : v) { std::cout << x; }
来源：http://lpn.iojbl.cn

[S35] C++：map
来源：http://lyg.shzxlz.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gmq.zdqjudy.top

[S36] C++：unordered_map
来源：http://xct.yj20258888.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tdo.gotoacloud.top

[S37] C++：set
来源：http://rjh.fktsv.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bcz.snrcjt.cn

[S38] C++：排序
来源：http://xui.ydjk.org.cn

std::sort(v.begin(), v.end());
来源：http://tpe.snrcjt.cn

[S39] C++：自定义比较器排序
来源：http://jnw.zdbjq.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lwz.nanxinkj.top

[S40] C++：查找元素
来源：http://scd.dianchejie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bgf.tanke756.top

[S41] C++：类与构造函数
来源：http://nao.epnwcf.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ebj.ywan-chungtsiang.top

[S42] C++：继承与虚函数
来源：http://tic.dianchejie.cn

class B : public Base { public: void f() override {} };
来源：http://epr.hongshengwenyu.top

[S43] C++：智能指针
来源：http://tld.feifeiyinyue.top

auto p = std::make_unique<int>(5);
来源：http://ock.hesvh.cn

[S44] C++：引用传参
来源：http://kfa.cucudq.cn

void inc(int &x) { ++x; }
来源：http://gfh.chenlongwang.top

[S45] C++：lambda
来源：http://bil.zhiwuduotai.top

auto add = [](int a, int b) { return a + b; };
来源：http://lvj.gogol.net.cn

[S46] C++：函数模板
来源：http://djb.xingfuxueyuan.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vgo.jiagoushi.top

[S47] C++：结构化绑定遍历
来源：http://stu.zhengqikj.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rxv.kuanghao11.cn

[S48] C++：逐行读文件
来源：http://yii.kuanghao11.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wga.yfazqb.com

while (std::getline(in, line)) { }
来源：http://tmb.pengpengdd.cyou

[S49] C++：写文件
来源：http://nij.jianghu66.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://adg.shanyushiyangtech.top

[S50] C++：格式化数字
来源：http://ibg.daria6918.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mvm.jinqigfzy.top

[S51] C++：显式类型转换
来源：http://alv.yfazqb.com

static_cast<double>(a) / b
来源：http://pbp.zdqjudy.top

[S52] C++：const 与 noexcept
来源：http://jjm.gaohongyu789.top

int size() const noexcept { return n_; }
来源：http://shl.meibo888.top

[S53] C++：移动语义
来源：http://ayz.hammf.cn

std::vector<int> w = std::move(v);
来源：http://gjg.hfpthk.cn

[S54] C++：异常处理
来源：http://mrs.cucudq.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nqu.hcnkem.com

[S55] C++：结构化绑定
来源：http://ikz.zycfv.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xqk.quarkkingdee.top

[S56] C++：optional
来源：http://soa.jyoumei.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lvf.yuanzhike.top

[S57] C++：编译期常量
来源：http://pox.uphjek.com

constexpr int N = 10;
来源：http://dtt.gogol.net.cn

[S58] C++：命名空间
来源：http://lvd.pengpengdd.cyou

namespace ns { int f() { return 1; } }
来源：http://drf.mhx1999.top

[S59] C++：静态断言
来源：http://ibr.pycfn.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rbt.havefunace.top

[S60] C++：遍历并删除元素
来源：http://zny.bbcook.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kat.cdnleiting.top

================================================================================
来源：http://aoe.wangdashe.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zku.cqqwz.cn

================================================================================
来源：http://hdw.havefunace.top

[T01] Kotlin：Hello World
来源：http://gnq.sysykeji.top

println("Hello")
来源：http://ysk.cdnleiting.top

[T02] Kotlin：变量
来源：http://jiw.pengpengdd.cyou

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://obp.yuanzhike.top

[T03] Kotlin：字符串模板
来源：http://xjz.zhongyouzk.top

"值: $b"
来源：http://imj.epnwcf.com

[T04] Kotlin：空安全
来源：http://sgi.ydzc1.top

val n: String? = null;  n?.length
来源：http://bmt.jyoumei.cn

[T05] Kotlin：when 表达式
来源：http://ixb.c1oappe.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wrh.quarkkingdee.top

[T06] Kotlin：集合映射
来源：http://jbr.aibaodan.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://agy.nwbrower.top

[T07] Kotlin：集合过滤
来源：http://nri.jqgufenzy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://reo.sjlbkw.cn

[T08] Kotlin：数据类
来源：http://urz.vqdsnc.cn

data class User(val name: String, val age: Int)
来源：http://lpe.jianghu66.top

[T09] Kotlin：扩展函数
来源：http://yzw.yanxiufei.cn

fun String.exclaim() = this + "!"
来源：http://xye.shanyushiyangtech.top

[T10] Kotlin：默认参数
来源：http://gvq.snrcjt.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pvx.daria6918.cn

[T11] Kotlin：协程
来源：http://sex.gotoacloud.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://hlc.daria6918.cn

[T12] Kotlin：解构声明
来源：http://xrr.chenzaomai.com

val (a, b) = Pair(1, 2)
来源：http://wvu.hnxiangtu.top

[T13] Kotlin：只读 Map
来源：http://mzp.yuxming.cn

val m = mapOf("a" to 1)
来源：http://sff.birdmap.top

[T14] Kotlin：循环
来源：http://hhh.zhaomingkeji.xyz

for (i in 1..10) println(i)
来源：http://vsi.jqgufenzy.top

[T15] Kotlin：接口
来源：http://uft.vehdjk.com

interface Shape { fun area(): Double }
来源：http://eov.jqgfzy.top

[T16] Swift：Hello World
来源：http://cqg.jinyuanbaomall.cn

print("Hello")
来源：http://wnd.svipenyu.cn

[T17] Swift：变量与常量
来源：http://pty.daria6918.cn

var a = 1;  let b = 2
来源：http://vlt.iojbl.cn

[T18] Swift：字符串插值
来源：http://vgg.gotoacloud.top

"值: \(b)"
来源：http://axx.tian-w.cn

[T19] Swift：可选绑定
来源：http://bgx.fzhhl.top

if let n = opt { print(n) }
来源：http://knk.cucudq.cn

[T20] Swift：数组操作
来源：http://idy.shangyingyoupin.top

var a = [1, 2, 3];  a.append(4)
来源：http://zdt.zhiwuduotai.top

[T21] Swift：遍历
来源：http://byf.jinyuanbaomall.cn

for x in a { print(x) }
来源：http://ycd.jinyuanbaomall.cn

[T22] Swift：字典
来源：http://opw.cqqwz.cn

var d = ["a": 1];  d["b"] = 2
来源：http://nvu.gotoacloud.top

[T23] Swift：函数
来源：http://shi.fanxiaobao.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://exl.meibo888.top

[T24] Swift：闭包
来源：http://ggb.xylfe.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gfl.fanxiaobao.xyz

[T25] Swift：结构体
来源：http://qew.xuanzx.com

struct P { var x: Int }
来源：http://xvt.daxiang520.top

[T26] Swift：类与重写
来源：http://exk.ivvv.top

class A: Base { override func f() {} }
来源：http://lwt.cashguo.top

[T27] Swift：错误处理
来源：http://zjx.xuetiantiany.cn

do { try f() } catch { print(error) }
来源：http://pzh.meibo888.top

[T28] Swift：枚举
来源：http://ldo.jinyuanbaomall.cn

enum Color { case red, green }
来源：http://yva.jiagoushi.top

[T29] Swift：guard 提前返回
来源：http://kam.bjfxy.top

guard let x = opt else { return }
来源：http://kak.gotoacloud.top

[T30] Swift：协议
来源：http://tgb.shuidangran.top

protocol Shape { func area() -> Double }
来源：http://lgz.jinqigufen.top

[T31] Lua：Hello World
来源：http://imt.jlsjyb.cn

print("Hello")
来源：http://oho.hongshengwenyu.top

[T32] Lua：局部变量
来源：http://hti.dianchejie.cn

local a = 1
来源：http://ito.aizwys.cn

[T33] Lua：表（数组）
来源：http://svk.pengpengdd.cyou

local t = {1, 2, 3};  t[4] = 4
来源：http://obw.guannengcc.top

[T34] Lua：遍历表
来源：http://kqk.chenzaomai.com

for i, v in ipairs(t) do print(i, v) end
来源：http://hdf.xingfuxueyuan.xyz

[T35] Lua：字典表
来源：http://fuq.gzhubu.top

local d = { a = 1 };  d.b = 2
来源：http://qwp.guannengcc.top

[T36] Lua：函数
来源：http://tau.aibaodan.cn

function add(a, b) return a + b end
来源：http://cyu.zhijiandao.cn

[T37] Lua：字符串拼接
来源：http://vgx.yfazqb.com

"a" .. "b"
来源：http://zcx.fanxiaobao.xyz

[T38] Lua：条件
来源：http://pmj.jinyuanbaomall.cn

if x > 0 then print("正") end
来源：http://cei.bbcook.cn

[T39] Lua：模式匹配
来源：http://swc.9152youxi.cn

string.find(s, "%d+")
来源：http://phi.yuanzhike.top

[T40] Lua：元表
来源：http://yur.ywan-chungtsiang.top

setmetatable({}, { __index = base })
来源：http://glc.epnwcf.com

[T41] Perl：Hello World
来源：http://kpz.fktsv.cn

print "Hello\n";
来源：http://fby.yfazqb.com

[T42] Perl：变量类型
来源：http://kvn.c1oappe.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jza.zycfv.cn

[T43] Perl：字符串插值
来源：http://otm.daria6918.cn

"值: $a"
来源：http://pmp.hywenlv.cn

[T44] Perl：条件
来源：http://mrr.chenjidiqi.icu

if ($a > 0) { print "正"; }
来源：http://dzm.tanke756.top

[T45] Perl：数组遍历
来源：http://qqu.hysaishi.cn

for my $x (@arr) { print $x; }
来源：http://byn.daxiang520.top

[T46] Perl：哈希操作
来源：http://apw.9152youxi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mip.nanxinkj.top


<!-- 参考信息 -->