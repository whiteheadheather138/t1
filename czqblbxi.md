代发 wailian999

cmd >/dev/null 2>&1
来源：http://omw.hesvh.cn

[R42] 输入重定向
来源：http://wjs.zhongyouzk.top

wc -l < a.txt
来源：http://ksq.vehdjk.com

[R43] 按名字查找文件
来源：http://fdl.yangfankeji.com

find . -name "*.log" -type f
来源：http://ecq.yvedp.cn

[R44] 按修改时间查找
来源：http://ywv.vqdsnc.cn

find . -mtime -7 -type f
来源：http://tnk.birdmap.top

[R45] 批量删除
来源：http://ccr.hnxiangtu.top

find . -name "*.tmp" -delete
来源：http://rll.sxryk.cn

[R46] 递归替换文件内容
来源：http://rwd.xinyue.icu

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sxx.jinqigfzy.top

[R47] sed 单行替换
来源：http://fos.yongpay.top

sed -i 's/foo/bar/g' a.txt
来源：http://xra.bbcook.cn

[R48] awk 取指定列
来源：http://dwy.fehbvm.com

awk '{print $1, $3}' a.txt
来源：http://jlm.yuanzhike.top

[R49] awk 带条件
来源：http://mqx.chenzaomai.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://anj.ydzc1.top

[R50] awk 求和
来源：http://btq.shanyushiyangkeji.top

awk '{s += $2} END {print s}' a.txt
来源：http://owc.quarkkingdee.top

[R51] 排序去重取前几
来源：http://jui.jiagoushi.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ovf.wangshuangyany.cn

[R52] 统计行数
来源：http://ixl.mhx1999.top

wc -l a.txt
来源：http://tpg.jqgfzy.top

[R53] 查看文件头与实时尾
来源：http://eeo.ydjk.org.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://boj.ywan-chungtsiang.top

[R54] 比较两个文件
来源：http://fok.jinghuilouyu.cn

diff a.txt b.txt
来源：http://stg.birdmap.top

[R55] 压缩与解压
来源：http://vql.fzhhl.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://iux.yuanzhike.top

[R56] 远程拷贝
来源：http://xem.feifeiyinyue.top

scp file user@host:/path/
来源：http://zto.ydzc1.top

[R57] 远程执行命令
来源：http://vmf.wangshuangyany.cn

ssh user@host 'uptime'
来源：http://olg.yuanzhike.top

[R58] 下载文件
来源：http://woh.nanxuanxn.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qql.ywan-chungtsiang.top

[R59] 发 POST JSON
来源：http://hpp.yueranfly.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ver.zhongyouzk.top

[R60] 只看 HTTP 状态码
来源：http://neb.hcnkem.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jdg.xuetiantiany.cn

[R61] 磁盘占用
来源：http://kxz.yuanzhike.top

df -h;  du -sh *
来源：http://yqa.zhaomingkeji.xyz

[R62] 找最占空间的文件
来源：http://ofr.zdqjudy.top

du -ah . | sort -rh | head -10
来源：http://kks.guowangkeji.top

[R63] 内存与进程
来源：http://cgz.zdbjq.cn

free -h;  ps aux | grep nginx
来源：http://lcy.ctjpmb.com

[R64] 结束进程
来源：http://xbj.xuetiantiany.cn

kill -9 $(pgrep -f app.py)
来源：http://etb.xingfuxueyuan.xyz

[R65] 查看端口占用
来源：http://aqp.guowangkeji.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rnn.yangfankeji.com

[R66] 定时任务
来源：http://zmz.yj20258.top

crontab -e;  crontab -l
来源：http://wke.cheryme.top

[R67] 生成随机十六进制串
来源：http://rhx.gaohongyu789.top

openssl rand -hex 16
来源：http://mro.yvedp.cn

[R68] 计算文件校验值
来源：http://vat.316326.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://mto.yj20258888.top

[R69] 生成随机密码
来源：http://qey.mhx1999.top

head -c 16 /dev/urandom | base64
来源：http://zkw.yfazqb.com

[R70] 时间戳与互转
来源：http://xtd.iojbl.cn

date +%s;  date -d @1700000000
来源：http://xzu.gogol.net.cn

[R71] 日期格式化
来源：http://dta.fehbvm.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://ibr.zhixingplan.top

[R72] 等待端口就绪
来源：http://iaw.guannengcc.top

until nc -z localhost 3306; do sleep 1; done
来源：http://gma.0kj1m.cn

[R73] 分割大日志
来源：http://cck.jqgfzy.top

split -l 1000 big.log part_
来源：http://qlq.yongpay.top

[R74] 批量重命名
来源：http://tsy.hcnkem.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mnm.0kj1m.cn

[R75] 导出环境变量
来源：http://leo.ydzc1.top

export PATH="$HOME/bin:$PATH"
来源：http://jnh.zycfv.cn

[R76] 使用临时文件
来源：http://wim.ydjk.org.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vuy.kuanghao11.cn

[R77] 读取用户输入
来源：http://rhu.ydzc1.top

read -rp "请输入: " ans
来源：http://shj.xuetiantiany.cn

[R78] 交互式菜单
来源：http://gcf.havefunace.top

select opt in a b c; do echo "$opt"; break; done
来源：http://djh.hfpthk.cn

[R79] 解析命令行选项
来源：http://jbq.sjlbkw.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zoq.jiagoushi.top

[R80] 查看脚本执行耗时
来源：http://rod.zdbjq.cn

time ./run.sh
来源：http://yoc.hammf.cn

================================================================================
来源：http://fmj.aibaodan.cn

S. C / C++ 专题
来源：http://fyx.yvedp.cn

================================================================================
来源：http://zud.gzhubu.top

[S01] C：Hello World
来源：http://xst.yvedp.cn

#include <stdio.h>
来源：http://vqe.cashguo.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ewy.svipenyu.cn

[S02] C：变量与格式化输出
来源：http://mwi.ppjwa.cn

int a = 10; printf("%d\n", a);
来源：http://iev.chenjidiqi.icu

[S03] C：读入整数
来源：http://exw.zhijiandao.cn

int x; scanf("%d", &x);
来源：http://tbg.tianlin.xyz

[S04] C：字符串复制
来源：http://mzr.jlsjyb.cn

char dst[32]; strcpy(dst, "hi");
来源：http://efz.yueranfly.top

[S05] C：字符串长度
来源：http://hbw.jlsjyb.cn

strlen(s)
来源：http://xrw.yuxming.cn

[S06] C：字符串比较
来源：http://vru.zhongyouzk.top

strcmp(a, b) == 0
来源：http://iie.zhengqikj.top

[S07] C：数组遍历求和
来源：http://bxs.vqdsnc.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://chr.bbcook.cn

[S08] C：动态内存分配与释放
来源：http://ici.jlsjyb.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kzg.sxryk.cn

[S09] C：结构体定义与初始化
来源：http://krd.tarul.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bqq.gogol.net.cn

[S10] C：指针与解引用
来源：http://rye.zycfv.cn

int *p = &a;  *p = 5;
来源：http://lbc.fengsongda.top

[S11] C：逐行读文件
来源：http://oyb.hammf.cn

FILE *f = fopen("a.txt", "r");
来源：http://ffc.yueranfly.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://qvh.yueranfly.top

fclose(f);
来源：http://hia.yonumen.top

[S12] C：写文件
来源：http://ucr.zdqjudy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uyq.cheryme.top

[S13] C：宏定义
来源：http://tmx.havefunace.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ocn.jqgfzy.top

[S14] C：枚举
来源：http://tom.uphjek.com

enum Color { RED, GREEN, BLUE };
来源：http://mti.fzhhl.top

[S15] C：类型转换
来源：http://mpj.gogol.net.cn

(double) a / b
来源：http://bee.zhixingplan.top

[S16] C：位操作置位
来源：http://qfi.ywan-chungtsiang.top

x |= (1 << 3);
来源：http://vbb.aibaodan.cn

[S17] C：安全拼接字符串
来源：http://ysi.hcnkem.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nqu.nanxinkj.top

[S18] C：命令行参数
来源：http://lcx.ybcxt.top

int main(int argc, char **argv)
来源：http://dwa.redwolf501.top

[S19] C：快速排序
来源：http://cfw.hcnkem.com

qsort(a, n, sizeof(int), cmp);
来源：http://yqk.gzhubu.top

[S20] C：二分查找
来源：http://xmd.zhongyouzk.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tyx.cdnleiting.top

[S21] C：字符类别判断
来源：http://wno.snrcjt.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://opc.zhiwuduotai.top

[S22] C：字符串转数字
来源：http://aan.daxiang520.top

atoi("42");  strtod("3.14", NULL);
来源：http://lnh.sjlbkw.cn

[S23] C：随机数
来源：http://rjr.snrcjt.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rzd.wangdashe.top

[S24] C：获取本地时间
来源：http://ypw.hywenlv.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nzz.cqqwz.cn

[S25] C：内存拷贝
来源：http://nan.yanxiufei.cn

memcpy(dst, src, n);
来源：http://pnw.yj20258888.top

[S26] C：内存清零
来源：http://pxy.ivvv.top

memset(a, 0, sizeof a);
来源：http://ojp.zycfv.cn

[S27] C：定义常量
来源：http://uhr.guowangkeji.top

const double PI = 3.14159;
来源：http://cwx.jinyuanbaomall.cn

[S28] C：静态变量
来源：http://fiw.mhx1999.top

static int counter = 0;
来源：http://nok.kuanghao11.cn

[S29] C：变参函数
来源：http://qqp.xylfe.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://etm.cqqwz.cn

[S30] C：头文件保护
来源：http://qxl.dashuyun.cn

#ifndef X_H
来源：http://yqj.yuxming.cn

#define X_H
来源：http://bfw.jinqigfzy.top

#endif
来源：http://iis.xylfe.cn

[S31] C++：Hello World
来源：http://ttb.xylfe.cn

#include <iostream>
来源：http://dad.chenlongwang.top

int main() { std::cout << "Hello\n"; }
来源：http://tel.redwolf501.top

[S32] C++：字符串
来源：http://epa.meibo888.top

std::string s = "hi";  s += "!";
来源：http://qyo.zdbjq.cn

[S33] C++：vector 增删
来源：http://vud.uphjek.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://czp.sysykeji.top

[S34] C++：遍历 vector
来源：http://fwf.0kj1m.cn

for (auto &x : v) { std::cout << x; }
来源：http://lbm.ybcxt.top

[S35] C++：map
来源：http://gad.zhengqikj.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jux.shzxlz.cn

[S36] C++：unordered_map
来源：http://lik.hammf.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tkc.fengsongda.top

[S37] C++：set
来源：http://fgc.jyoumei.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gqs.daria6918.cn

[S38] C++：排序
来源：http://opr.snrcjt.cn

std::sort(v.begin(), v.end());
来源：http://ued.wangshuangyany.cn

[S39] C++：自定义比较器排序
来源：http://urj.ybcxt.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://caf.pycfn.com

[S40] C++：查找元素
来源：http://kuh.zhiwuduotai.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kfo.tanke756.top

[S41] C++：类与构造函数
来源：http://ymx.shanyushiyangtech.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://anf.yvedp.cn

[S42] C++：继承与虚函数
来源：http://jip.shuidangran.top

class B : public Base { public: void f() override {} };
来源：http://cny.aibaodan.cn

[S43] C++：智能指针
来源：http://cxq.hnqzz.top

auto p = std::make_unique<int>(5);
来源：http://xqg.zdbjq.cn

[S44] C++：引用传参
来源：http://ina.cheryme.top

void inc(int &x) { ++x; }
来源：http://wox.vehdjk.com

[S45] C++：lambda
来源：http://krb.hnxiangtu.top

auto add = [](int a, int b) { return a + b; };
来源：http://qky.jyoumei.cn

[S46] C++：函数模板
来源：http://cja.redwolf501.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://woq.dianchejie.cn

[S47] C++：结构化绑定遍历
来源：http://esp.tian-w.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ovs.fzhhl.top

[S48] C++：逐行读文件
来源：http://zkk.tanke756.top

std::ifstream in("a.txt");  std::string line;
来源：http://pmu.gogol.net.cn

while (std::getline(in, line)) { }
来源：http://dfh.hysaishi.cn

[S49] C++：写文件
来源：http://rie.chenzaomai.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vvj.sxryk.cn

[S50] C++：格式化数字
来源：http://jzz.shangyingyoupin.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dvp.yonumen.top

[S51] C++：显式类型转换
来源：http://djn.jyoumei.cn

static_cast<double>(a) / b
来源：http://tdo.ybcxt.top

[S52] C++：const 与 noexcept
来源：http://exo.gotoacloud.top

int size() const noexcept { return n_; }
来源：http://hjp.sysykeji.top

[S53] C++：移动语义
来源：http://bpu.vqdsnc.cn

std::vector<int> w = std::move(v);
来源：http://zah.chenlongwang.top

[S54] C++：异常处理
来源：http://ixq.shangyingyoupin.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kfl.daxiang520.top

[S55] C++：结构化绑定
来源：http://prm.mhx1999.top

auto [a, b] = std::make_pair(1, 2);
来源：http://qll.zhoulong.xyz

[S56] C++：optional
来源：http://fpf.meibo888.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mra.bbcook.cn

[S57] C++：编译期常量
来源：http://bor.jlsjyb.cn

constexpr int N = 10;
来源：http://pwc.epnwcf.com

[S58] C++：命名空间
来源：http://xkq.aizwys.cn

namespace ns { int f() { return 1; } }
来源：http://qox.dashuyun.cn

[S59] C++：静态断言
来源：http://bkt.tarul.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qor.guannengcc.top

[S60] C++：遍历并删除元素
来源：http://gsc.redwolf501.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ima.jiagoushi.top

================================================================================
来源：http://jbx.yuxming.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gcr.c1oappe.top

================================================================================
来源：http://hjj.chenzaomai.com

[T01] Kotlin：Hello World
来源：http://twh.epnwcf.com

println("Hello")
来源：http://yxy.cdnleiting.top

[T02] Kotlin：变量
来源：http://xnm.0kj1m.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://swc.sjlbkw.cn

[T03] Kotlin：字符串模板
来源：http://xtu.hcnkem.com

"值: $b"
来源：http://ukt.guannengcc.top

[T04] Kotlin：空安全
来源：http://wkx.epnwcf.com

val n: String? = null;  n?.length
来源：http://vzj.zhongyouzk.top

[T05] Kotlin：when 表达式
来源：http://vwd.feifeiyinyue.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kbu.gaohongyu789.top

[T06] Kotlin：集合映射
来源：http://eqz.vehdjk.com

listOf(1, 2, 3).map { it * 2 }
来源：http://akw.sjlbkw.cn

[T07] Kotlin：集合过滤
来源：http://mes.xylfe.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://kue.cucudq.cn

[T08] Kotlin：数据类
来源：http://eei.wangshuangyany.cn

data class User(val name: String, val age: Int)
来源：http://tuo.cqqwz.cn

[T09] Kotlin：扩展函数
来源：http://kaj.iojbl.cn

fun String.exclaim() = this + "!"
来源：http://egv.hesvh.cn

[T10] Kotlin：默认参数
来源：http://num.feifeiyinyue.top

fun greet(name: String = "World") = "Hi $name"
来源：http://wuh.cheryme.top

[T11] Kotlin：协程
来源：http://vsu.jiagoushi.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://suu.jlsjyb.cn

[T12] Kotlin：解构声明
来源：http://rad.svipenyu.cn

val (a, b) = Pair(1, 2)
来源：http://qxb.ydjk.org.cn

[T13] Kotlin：只读 Map
来源：http://xov.xingfuxueyuan.xyz

val m = mapOf("a" to 1)
来源：http://gie.fanxiaobao.xyz

[T14] Kotlin：循环
来源：http://rqo.svipenyu.cn

for (i in 1..10) println(i)
来源：http://xtg.chenjidiqi.icu

[T15] Kotlin：接口
来源：http://uzm.zycfv.cn

interface Shape { fun area(): Double }
来源：http://zeh.chenlongwang.top

[T16] Swift：Hello World
来源：http://pwt.epnwcf.com

print("Hello")
来源：http://otq.xuanzx.com

[T17] Swift：变量与常量
来源：http://bya.hnxiangtu.top

var a = 1;  let b = 2
来源：http://khr.0kj1m.cn

[T18] Swift：字符串插值
来源：http://xgx.jianghu66.top

"值: \(b)"
来源：http://mbb.yvedp.cn

[T19] Swift：可选绑定
来源：http://igp.jinghuilouyu.cn

if let n = opt { print(n) }
来源：http://afy.jinqigufen.top

[T20] Swift：数组操作
来源：http://uyq.zycfv.cn

var a = [1, 2, 3];  a.append(4)
来源：http://krc.fzhhl.top

[T21] Swift：遍历
来源：http://dzi.daria6918.cn

for x in a { print(x) }
来源：http://obx.hammf.cn

[T22] Swift：字典
来源：http://zgs.tianlin.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://nky.aibaodan.cn

[T23] Swift：函数
来源：http://bon.shangyingyoupin.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://coo.xuetiantiany.cn

[T24] Swift：闭包
来源：http://zvi.uphjek.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://nel.hongshengwenyu.top

[T25] Swift：结构体
来源：http://qua.yuxming.cn

struct P { var x: Int }
来源：http://jqp.mhx1999.top

[T26] Swift：类与重写
来源：http://sxe.haohaochexian.top

class A: Base { override func f() {} }
来源：http://lqf.zhongyouzk.top

[T27] Swift：错误处理
来源：http://lpx.pengpengdd.cyou

do { try f() } catch { print(error) }
来源：http://kfm.hnqzz.top

[T28] Swift：枚举
来源：http://khk.cheryme.top

enum Color { case red, green }
来源：http://fas.yfazqb.com

[T29] Swift：guard 提前返回
来源：http://uvg.fehbvm.com

guard let x = opt else { return }
来源：http://xzp.cashguo.top

[T30] Swift：协议
来源：http://fgo.yj20258.top

protocol Shape { func area() -> Double }
来源：http://gcp.sxryk.cn

[T31] Lua：Hello World
来源：http://fde.ctjpmb.com

print("Hello")
来源：http://itx.gaohongyu789.top

[T32] Lua：局部变量
来源：http://fji.yueranfly.top

local a = 1
来源：http://skf.wangshuangyany.cn

[T33] Lua：表（数组）
来源：http://opk.yangfankeji.com

local t = {1, 2, 3};  t[4] = 4
来源：http://rio.tanke756.top

[T34] Lua：遍历表
来源：http://elm.vqdsnc.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://kbb.jqgufenzy.top

[T35] Lua：字典表
来源：http://lga.gzhubu.top

local d = { a = 1 };  d.b = 2
来源：http://ecu.gaohongyu789.top

[T36] Lua：函数
来源：http://vnj.guowangkeji.top

function add(a, b) return a + b end
来源：http://zvt.cqqwz.cn

[T37] Lua：字符串拼接
来源：http://pdo.cashguo.top

"a" .. "b"
来源：http://pmh.hnqzz.top

[T38] Lua：条件
来源：http://zyn.yfazqb.com

if x > 0 then print("正") end
来源：http://awc.xuetiantiany.cn

[T39] Lua：模式匹配
来源：http://phv.feifeiyinyue.top

string.find(s, "%d+")
来源：http://iku.ydzc1.top

[T40] Lua：元表
来源：http://byg.dashuyun.cn

setmetatable({}, { __index = base })
来源：http://zle.fehbvm.com

[T41] Perl：Hello World
来源：http://ric.ctjpmb.com

print "Hello\n";
来源：http://aus.birdmap.top

[T42] Perl：变量类型
来源：http://kat.xuanzx.com

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cir.zhengqikj.top

[T43] Perl：字符串插值
来源：http://ygy.shanyushiyangkeji.top

"值: $a"
来源：http://jvw.52xcode.cn

[T44] Perl：条件
来源：http://cur.dianchejie.cn

if ($a > 0) { print "正"; }
来源：http://luy.chenlongwang.top


<!-- 参考信息 -->