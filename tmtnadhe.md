代发 wailian999

cmd > out.log 2>&1
来源：http://asc.kuanghao11.cn

[R40] 追加写日志
来源：http://awm.ehwqpu.com

echo "log" >> out.log
来源：http://nuj.52xcode.cn

[R41] 丢弃输出
来源：http://bpo.cheryme.top

cmd >/dev/null 2>&1
来源：http://tia.hysaishi.cn

[R42] 输入重定向
来源：http://nvr.yvedp.cn

wc -l < a.txt
来源：http://zfd.jyoumei.cn

[R43] 按名字查找文件
来源：http://yow.bbcook.cn

find . -name "*.log" -type f
来源：http://bjo.xylfe.cn

[R44] 按修改时间查找
来源：http://dxh.shzxlz.cn

find . -mtime -7 -type f
来源：http://gni.daria6918.cn

[R45] 批量删除
来源：http://cmc.jqgufenzy.top

find . -name "*.tmp" -delete
来源：http://hna.cucudq.cn

[R46] 递归替换文件内容
来源：http://zfq.vqdsnc.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dzx.shuidangran.top

[R47] sed 单行替换
来源：http://ezq.uphjek.com

sed -i 's/foo/bar/g' a.txt
来源：http://jnd.hnqzz.top

[R48] awk 取指定列
来源：http://uvi.zhongyouzk.top

awk '{print $1, $3}' a.txt
来源：http://nbx.sxryk.cn

[R49] awk 带条件
来源：http://gae.ehwqpu.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jvb.gzhubu.top

[R50] awk 求和
来源：http://vxr.fengsongda.top

awk '{s += $2} END {print s}' a.txt
来源：http://aws.yj20258888.top

[R51] 排序去重取前几
来源：http://cuk.andypj.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://jei.jlsjyb.cn

[R52] 统计行数
来源：http://spz.yanxiufei.cn

wc -l a.txt
来源：http://opc.sufxvd.cn

[R53] 查看文件头与实时尾
来源：http://ggz.jinghuilouyu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://psd.bbcook.cn

[R54] 比较两个文件
来源：http://lip.yvedp.cn

diff a.txt b.txt
来源：http://plc.c1oappe.top

[R55] 压缩与解压
来源：http://rjw.xuetiantiany.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fgb.ywan-chungtsiang.top

[R56] 远程拷贝
来源：http://szy.hcnkem.com

scp file user@host:/path/
来源：http://ddf.cucudq.cn

[R57] 远程执行命令
来源：http://njg.bbcook.cn

ssh user@host 'uptime'
来源：http://sen.shanyushiyangkeji.top

[R58] 下载文件
来源：http://pcs.zycfv.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fcl.hysaishi.cn

[R59] 发 POST JSON
来源：http://mlt.zdqjudy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lpf.chenjidiqi.icu

[R60] 只看 HTTP 状态码
来源：http://kxz.svipenyu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://srg.fanxiaobao.xyz

[R61] 磁盘占用
来源：http://eob.zhiwuduotai.top

df -h;  du -sh *
来源：http://ifd.gogol.net.cn

[R62] 找最占空间的文件
来源：http://qth.chenlongwang.top

du -ah . | sort -rh | head -10
来源：http://wtr.zhengqikj.top

[R63] 内存与进程
来源：http://qew.smart0.xyz

free -h;  ps aux | grep nginx
来源：http://ivu.tarul.cn

[R64] 结束进程
来源：http://hfl.316326.xyz

kill -9 $(pgrep -f app.py)
来源：http://olq.ivvv.top

[R65] 查看端口占用
来源：http://lhb.aizwys.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://esa.xylfe.cn

[R66] 定时任务
来源：http://ysq.cucudq.cn

crontab -e;  crontab -l
来源：http://bzn.0kj1m.cn

[R67] 生成随机十六进制串
来源：http://ytd.hysaishi.cn

openssl rand -hex 16
来源：http://ssa.yuxming.cn

[R68] 计算文件校验值
来源：http://adt.wangdashe.top

sha256sum a.txt;  md5sum a.txt
来源：http://sjc.cqqwz.cn

[R69] 生成随机密码
来源：http://tcr.daria6918.cn

head -c 16 /dev/urandom | base64
来源：http://uoo.yj20258888.top

[R70] 时间戳与互转
来源：http://lry.c1oappe.top

date +%s;  date -d @1700000000
来源：http://itn.jinqigfzy.top

[R71] 日期格式化
来源：http://ohn.hysaishi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://mho.mhx1999.top

[R72] 等待端口就绪
来源：http://ghz.9152youxi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cil.uphjek.com

[R73] 分割大日志
来源：http://kav.xingfuxueyuan.xyz

split -l 1000 big.log part_
来源：http://rfq.gzhubu.top

[R74] 批量重命名
来源：http://ins.iojbl.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://evy.yj202588.top

[R75] 导出环境变量
来源：http://awp.aibaodan.cn

export PATH="$HOME/bin:$PATH"
来源：http://cel.hongshengwenyu.top

[R76] 使用临时文件
来源：http://jmi.aizwys.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xbn.ivvv.top

[R77] 读取用户输入
来源：http://uye.hywenlv.cn

read -rp "请输入: " ans
来源：http://pgz.cdnleiting.top

[R78] 交互式菜单
来源：http://vnz.xziqi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://arh.snrcjt.cn

[R79] 解析命令行选项
来源：http://sih.zhongyouzk.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://aob.havefunace.top

[R80] 查看脚本执行耗时
来源：http://bzw.hongshengwenyu.top

time ./run.sh
来源：http://qra.mhx1999.top

================================================================================
来源：http://kli.c1oappe.top

S. C / C++ 专题
来源：http://aeu.ctjpmb.com

================================================================================
来源：http://ack.bjfxy.top

[S01] C：Hello World
来源：http://gze.chenjidiqi.icu

#include <stdio.h>
来源：http://dho.zhixingplan.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://bhi.andypj.xyz

[S02] C：变量与格式化输出
来源：http://rfg.aibaodan.cn

int a = 10; printf("%d\n", a);
来源：http://tji.52xcode.cn

[S03] C：读入整数
来源：http://dyx.bbcook.cn

int x; scanf("%d", &x);
来源：http://slw.mhx1999.top

[S04] C：字符串复制
来源：http://gck.smart0.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://vaf.gzhubu.top

[S05] C：字符串长度
来源：http://rpe.pengpengdd.cyou

strlen(s)
来源：http://tbh.hysaishi.cn

[S06] C：字符串比较
来源：http://oyj.zhijiandao.cn

strcmp(a, b) == 0
来源：http://srz.vqdsnc.cn

[S07] C：数组遍历求和
来源：http://uqj.guowangkeji.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://osg.zhoulong.xyz

[S08] C：动态内存分配与释放
来源：http://sio.cqqwz.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://erv.pycfn.com

[S09] C：结构体定义与初始化
来源：http://knt.vehdjk.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fjj.xylfe.cn

[S10] C：指针与解引用
来源：http://fkr.jianghu66.top

int *p = &a;  *p = 5;
来源：http://ltw.sjlbkw.cn

[S11] C：逐行读文件
来源：http://mia.jqgufenzy.top

FILE *f = fopen("a.txt", "r");
来源：http://dne.guowangkeji.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://qtv.tian-w.cn

fclose(f);
来源：http://bvf.yuanzhike.top

[S12] C：写文件
来源：http://yrf.guowangkeji.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rht.gzhubu.top

[S13] C：宏定义
来源：http://epv.shanyushiyangkeji.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ghf.cheryme.top

[S14] C：枚举
来源：http://ysw.hysaishi.cn

enum Color { RED, GREEN, BLUE };
来源：http://lsh.ydzc1.top

[S15] C：类型转换
来源：http://cia.mhx1999.top

(double) a / b
来源：http://qua.dianchejie.cn

[S16] C：位操作置位
来源：http://mcf.aizwys.cn

x |= (1 << 3);
来源：http://els.gotoacloud.top

[S17] C：安全拼接字符串
来源：http://lju.jqgfzy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ygb.yanxiufei.cn

[S18] C：命令行参数
来源：http://dzy.ivvv.top

int main(int argc, char **argv)
来源：http://odl.hcnkem.com

[S19] C：快速排序
来源：http://kfo.yuanzhike.top

qsort(a, n, sizeof(int), cmp);
来源：http://dlv.yangfankeji.com

[S20] C：二分查找
来源：http://jnr.jianghu66.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cva.jlsjyb.cn

[S21] C：字符类别判断
来源：http://pox.hcnkem.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://brp.tarul.cn

[S22] C：字符串转数字
来源：http://dyz.52xcode.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tka.svipenyu.cn

[S23] C：随机数
来源：http://kbo.snrcjt.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://apj.iojbl.cn

[S24] C：获取本地时间
来源：http://kom.zhixingplan.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jcs.gaohongyu789.top

[S25] C：内存拷贝
来源：http://vpc.jianghu66.top

memcpy(dst, src, n);
来源：http://fox.cqqwz.cn

[S26] C：内存清零
来源：http://vaw.zhengqikj.top

memset(a, 0, sizeof a);
来源：http://tbl.kuanghao11.cn

[S27] C：定义常量
来源：http://iay.yj20258.top

const double PI = 3.14159;
来源：http://dho.jianghu66.top

[S28] C：静态变量
来源：http://jdx.tianlin.xyz

static int counter = 0;
来源：http://drk.tianlin.xyz

[S29] C：变参函数
来源：http://xov.ppjwa.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://svs.zhoulong.xyz

[S30] C：头文件保护
来源：http://vvf.jqgfzy.top

#ifndef X_H
来源：http://gkz.yangfankeji.com

#define X_H
来源：http://sdt.cqqwz.cn

#endif
来源：http://agr.jinqigufen.top

[S31] C++：Hello World
来源：http://dmc.nanxinkj.top

#include <iostream>
来源：http://uor.52xcode.cn

int main() { std::cout << "Hello\n"; }
来源：http://oxz.xingfuxueyuan.xyz

[S32] C++：字符串
来源：http://now.nwbrower.top

std::string s = "hi";  s += "!";
来源：http://hbh.jqgufenzy.top

[S33] C++：vector 增删
来源：http://feh.pycfn.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hsl.nwbrower.top

[S34] C++：遍历 vector
来源：http://ldx.hongshengwenyu.top

for (auto &x : v) { std::cout << x; }
来源：http://wcb.hongshengwenyu.top

[S35] C++：map
来源：http://tsv.hnxiangtu.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dkw.hesvh.cn

[S36] C++：unordered_map
来源：http://shi.316326.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ras.iojbl.cn

[S37] C++：set
来源：http://dmo.ehwqpu.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tfy.gogol.net.cn

[S38] C++：排序
来源：http://czz.jqgfzy.top

std::sort(v.begin(), v.end());
来源：http://gbg.hnxiangtu.top

[S39] C++：自定义比较器排序
来源：http://ugt.zhijiandao.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uyr.zhiwuduotai.top

[S40] C++：查找元素
来源：http://uha.haohaochexian.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hjc.pengpengdd.cyou

[S41] C++：类与构造函数
来源：http://lhh.xinyue.icu

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zpm.xingfuxueyuan.xyz

[S42] C++：继承与虚函数
来源：http://wtw.hnqzz.top

class B : public Base { public: void f() override {} };
来源：http://rzv.ydzc1.top

[S43] C++：智能指针
来源：http://cje.gogol.net.cn

auto p = std::make_unique<int>(5);
来源：http://qhh.vehdjk.com

[S44] C++：引用传参
来源：http://anx.ctjpmb.com

void inc(int &x) { ++x; }
来源：http://olq.ybcxt.top

[S45] C++：lambda
来源：http://deq.fzhhl.top

auto add = [](int a, int b) { return a + b; };
来源：http://ysd.hcnkem.com

[S46] C++：函数模板
来源：http://gvb.bbcook.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pkm.yanxiufei.cn

[S47] C++：结构化绑定遍历
来源：http://ihe.zhengqikj.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bco.andypj.xyz

[S48] C++：逐行读文件
来源：http://otu.shzxlz.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ndn.yvedp.cn

while (std::getline(in, line)) { }
来源：http://olg.yuanzhike.top

[S49] C++：写文件
来源：http://mhn.jianghu66.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ypk.zhongyouzk.top

[S50] C++：格式化数字
来源：http://ysc.yj202588.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jup.yangfankeji.com

[S51] C++：显式类型转换
来源：http://pxd.ybcxt.top

static_cast<double>(a) / b
来源：http://hli.yuxming.cn

[S52] C++：const 与 noexcept
来源：http://cci.9152youxi.cn

int size() const noexcept { return n_; }
来源：http://bdr.aizwys.cn

[S53] C++：移动语义
来源：http://hud.yfazqb.com

std::vector<int> w = std::move(v);
来源：http://ufk.fzhhl.top

[S54] C++：异常处理
来源：http://sgr.dashuyun.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://stx.jlsjyb.cn

[S55] C++：结构化绑定
来源：http://zje.ywan-chungtsiang.top

auto [a, b] = std::make_pair(1, 2);
来源：http://utc.quarkkingdee.top

[S56] C++：optional
来源：http://eiq.shangyingyoupin.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xjw.havefunace.top

[S57] C++：编译期常量
来源：http://utx.daria6918.cn

constexpr int N = 10;
来源：http://uam.hnqzz.top

[S58] C++：命名空间
来源：http://qth.yj20258888.top

namespace ns { int f() { return 1; } }
来源：http://swv.yuxming.cn

[S59] C++：静态断言
来源：http://ciq.jlsjyb.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qys.nanxinkj.top

[S60] C++：遍历并删除元素
来源：http://jcr.0kj1m.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jkn.andypj.xyz

================================================================================
来源：http://fdx.wangshuangyany.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yib.aizwys.cn

================================================================================
来源：http://yce.chenlongwang.top

[T01] Kotlin：Hello World
来源：http://mhg.jlsjyb.cn

println("Hello")
来源：http://cze.jiagoushi.top

[T02] Kotlin：变量
来源：http://ltr.gotoacloud.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zvy.zdqjudy.top

[T03] Kotlin：字符串模板
来源：http://ghe.yvedp.cn

"值: $b"
来源：http://rzc.cheryme.top

[T04] Kotlin：空安全
来源：http://nkj.hysaishi.cn

val n: String? = null;  n?.length
来源：http://vjm.mhx1999.top

[T05] Kotlin：when 表达式
来源：http://zey.sxryk.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://epf.sxryk.cn

[T06] Kotlin：集合映射
来源：http://cdu.zhongyouzk.top

listOf(1, 2, 3).map { it * 2 }
来源：http://qpe.dashuyun.cn

[T07] Kotlin：集合过滤
来源：http://lub.cqqwz.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wey.jiagoushi.top

[T08] Kotlin：数据类
来源：http://pyl.zhongyouzk.top

data class User(val name: String, val age: Int)
来源：http://uvn.zycfv.cn

[T09] Kotlin：扩展函数
来源：http://zoj.fzhhl.top

fun String.exclaim() = this + "!"
来源：http://apx.ywan-chungtsiang.top

[T10] Kotlin：默认参数
来源：http://csd.ydjk.org.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://bhq.yfazqb.com

[T11] Kotlin：协程
来源：http://kle.guannengcc.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://jso.ydjk.org.cn

[T12] Kotlin：解构声明
来源：http://cct.chenjidiqi.icu

val (a, b) = Pair(1, 2)
来源：http://kkt.cashguo.top

[T13] Kotlin：只读 Map
来源：http://vnh.shangyingyoupin.top

val m = mapOf("a" to 1)
来源：http://icq.andypj.xyz

[T14] Kotlin：循环
来源：http://xta.haohaochexian.top

for (i in 1..10) println(i)
来源：http://lhs.mhx1999.top

[T15] Kotlin：接口
来源：http://yeb.bjfxy.top

interface Shape { fun area(): Double }
来源：http://hjd.dashuyun.cn

[T16] Swift：Hello World
来源：http://yhw.yj202588.top

print("Hello")
来源：http://rld.c1oappe.top

[T17] Swift：变量与常量
来源：http://exl.chenjidiqi.icu

var a = 1;  let b = 2
来源：http://dsp.yfazqb.com

[T18] Swift：字符串插值
来源：http://dep.yuanzhike.top

"值: \(b)"
来源：http://nui.guowangkeji.top

[T19] Swift：可选绑定
来源：http://ksn.daria6918.cn

if let n = opt { print(n) }
来源：http://vzb.gogol.net.cn

[T20] Swift：数组操作
来源：http://tev.mhx1999.top

var a = [1, 2, 3];  a.append(4)
来源：http://igd.ivvv.top

[T21] Swift：遍历
来源：http://rlr.cheryme.top

for x in a { print(x) }
来源：http://rpy.mhx1999.top

[T22] Swift：字典
来源：http://xnu.bbcook.cn

var d = ["a": 1];  d["b"] = 2
来源：http://bai.jinqigufen.top

[T23] Swift：函数
来源：http://krq.gzhubu.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://grb.cashguo.top

[T24] Swift：闭包
来源：http://shy.aibaodan.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://iev.andypj.xyz

[T25] Swift：结构体
来源：http://guf.cdnleiting.top

struct P { var x: Int }
来源：http://iek.shzxlz.cn

[T26] Swift：类与重写
来源：http://eoj.sjlbkw.cn

class A: Base { override func f() {} }
来源：http://ypq.yj20258.top

[T27] Swift：错误处理
来源：http://qzj.zdqjudy.top

do { try f() } catch { print(error) }
来源：http://vrr.shzxlz.cn

[T28] Swift：枚举
来源：http://drr.hysaishi.cn

enum Color { case red, green }
来源：http://yjh.yuanzhike.top

[T29] Swift：guard 提前返回
来源：http://mhq.yj20258.top

guard let x = opt else { return }
来源：http://mpo.yvedp.cn

[T30] Swift：协议
来源：http://ezf.yuxming.cn

protocol Shape { func area() -> Double }
来源：http://ivt.yonumen.top

[T31] Lua：Hello World
来源：http://bvg.yongpay.top

print("Hello")
来源：http://fet.sufxvd.cn

[T32] Lua：局部变量
来源：http://mss.cdnleiting.top

local a = 1
来源：http://gsz.vehdjk.com

[T33] Lua：表（数组）
来源：http://qoj.xuanzx.com

local t = {1, 2, 3};  t[4] = 4
来源：http://fme.haohaochexian.top

[T34] Lua：遍历表
来源：http://igp.yuanzhike.top

for i, v in ipairs(t) do print(i, v) end
来源：http://eeo.redwolf501.top

[T35] Lua：字典表
来源：http://mxi.shangyingyoupin.top

local d = { a = 1 };  d.b = 2
来源：http://ryc.fengsongda.top

[T36] Lua：函数
来源：http://txp.gogol.net.cn

function add(a, b) return a + b end
来源：http://hvm.jlsjyb.cn

[T37] Lua：字符串拼接
来源：http://iwd.tian-w.cn

"a" .. "b"
来源：http://had.yvedp.cn

[T38] Lua：条件
来源：http://ngr.fzhhl.top

if x > 0 then print("正") end
来源：http://rde.jianghu66.top

[T39] Lua：模式匹配
来源：http://uar.zhaomingkeji.xyz

string.find(s, "%d+")
来源：http://ykz.sweek.top

[T40] Lua：元表
来源：http://kat.havefunace.top

setmetatable({}, { __index = base })
来源：http://ujv.shanyushiyangkeji.top

[T41] Perl：Hello World
来源：http://xdo.xuetiantiany.cn

print "Hello\n";
来源：http://yrk.daria6918.cn

[T42] Perl：变量类型
来源：http://yqe.jinqigufen.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cjw.jinqigufen.top


<!-- 参考信息 -->