代发 wailian999

cmd >/dev/null 2>&1
来源：http://udv.shuidangran.top

[R42] 输入重定向
来源：http://qyt.chenjidiqi.icu

wc -l < a.txt
来源：http://ipb.nanxinkj.top

[R43] 按名字查找文件
来源：http://dkg.tianlin.xyz

find . -name "*.log" -type f
来源：http://asw.sxryk.cn

[R44] 按修改时间查找
来源：http://qyy.yj20258888.top

find . -mtime -7 -type f
来源：http://utz.vehdjk.com

[R45] 批量删除
来源：http://myr.zycfv.cn

find . -name "*.tmp" -delete
来源：http://ceb.snrcjt.cn

[R46] 递归替换文件内容
来源：http://zwp.svipenyu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dap.nanxinkj.top

[R47] sed 单行替换
来源：http://zep.sjlbkw.cn

sed -i 's/foo/bar/g' a.txt
来源：http://syt.hnqzz.top

[R48] awk 取指定列
来源：http://hcq.ybcxt.top

awk '{print $1, $3}' a.txt
来源：http://kbl.hongshengwenyu.top

[R49] awk 带条件
来源：http://xck.zhoulong.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rxh.shuidangran.top

[R50] awk 求和
来源：http://hph.pycfn.com

awk '{s += $2} END {print s}' a.txt
来源：http://xfh.ybcxt.top

[R51] 排序去重取前几
来源：http://qni.zhaomingkeji.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://dsw.yj20258.top

[R52] 统计行数
来源：http://gea.nanxuanxn.top

wc -l a.txt
来源：http://ptt.snrcjt.cn

[R53] 查看文件头与实时尾
来源：http://obd.sjlbkw.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zap.yj20258.top

[R54] 比较两个文件
来源：http://lyn.nanxinkj.top

diff a.txt b.txt
来源：http://kjt.dianchejie.cn

[R55] 压缩与解压
来源：http://afp.ivvv.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jwt.yangfankeji.com

[R56] 远程拷贝
来源：http://kvc.jinqigufen.top

scp file user@host:/path/
来源：http://yfa.havefunace.top

[R57] 远程执行命令
来源：http://tux.yongpay.top

ssh user@host 'uptime'
来源：http://vde.guannengcc.top

[R58] 下载文件
来源：http://vpa.yuanzhike.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://flw.zdqjudy.top

[R59] 发 POST JSON
来源：http://psa.xinyue.icu

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vpy.bjfxy.top

[R60] 只看 HTTP 状态码
来源：http://lwq.sufxvd.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ugr.aizwys.cn

[R61] 磁盘占用
来源：http://fzk.jyoumei.cn

df -h;  du -sh *
来源：http://myl.316326.xyz

[R62] 找最占空间的文件
来源：http://ize.jiagoushi.top

du -ah . | sort -rh | head -10
来源：http://kmb.ctjpmb.com

[R63] 内存与进程
来源：http://sbe.zhijiandao.cn

free -h;  ps aux | grep nginx
来源：http://pfu.gzhubu.top

[R64] 结束进程
来源：http://zxi.chenzaomai.com

kill -9 $(pgrep -f app.py)
来源：http://tdg.sysykeji.top

[R65] 查看端口占用
来源：http://xqu.yonumen.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xyh.wangshuangyany.cn

[R66] 定时任务
来源：http://siq.feifeiyinyue.top

crontab -e;  crontab -l
来源：http://cia.vehdjk.com

[R67] 生成随机十六进制串
来源：http://lkz.sysykeji.top

openssl rand -hex 16
来源：http://qmv.gogol.net.cn

[R68] 计算文件校验值
来源：http://lfk.jlsjyb.cn

sha256sum a.txt;  md5sum a.txt
来源：http://pld.yfazqb.com

[R69] 生成随机密码
来源：http://jus.yuxming.cn

head -c 16 /dev/urandom | base64
来源：http://hga.feifeiyinyue.top

[R70] 时间戳与互转
来源：http://dat.aibaodan.cn

date +%s;  date -d @1700000000
来源：http://evj.chenjidiqi.icu

[R71] 日期格式化
来源：http://foz.uphjek.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://chw.snrcjt.cn

[R72] 等待端口就绪
来源：http://yqc.cashguo.top

until nc -z localhost 3306; do sleep 1; done
来源：http://hsd.sjlbkw.cn

[R73] 分割大日志
来源：http://dkl.cashguo.top

split -l 1000 big.log part_
来源：http://han.gaohongyu789.top

[R74] 批量重命名
来源：http://sml.xziqi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bta.zhengqikj.top

[R75] 导出环境变量
来源：http://taj.sjlbkw.cn

export PATH="$HOME/bin:$PATH"
来源：http://jwj.ydjk.org.cn

[R76] 使用临时文件
来源：http://hni.zdbjq.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mzu.yvedp.cn

[R77] 读取用户输入
来源：http://uyr.hcnkem.com

read -rp "请输入: " ans
来源：http://gzy.iojbl.cn

[R78] 交互式菜单
来源：http://prj.yonumen.top

select opt in a b c; do echo "$opt"; break; done
来源：http://dfl.havefunace.top

[R79] 解析命令行选项
来源：http://ymv.ydjk.org.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yci.shanyushiyangkeji.top

[R80] 查看脚本执行耗时
来源：http://lfm.sufxvd.cn

time ./run.sh
来源：http://lfs.wangshuangyany.cn

================================================================================
来源：http://rsj.quarkkingdee.top

S. C / C++ 专题
来源：http://kum.yueranfly.top

================================================================================
来源：http://mvy.sysykeji.top

[S01] C：Hello World
来源：http://cbp.hfpthk.cn

#include <stdio.h>
来源：http://sbi.ywan-chungtsiang.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://lgu.zhixingplan.top

[S02] C：变量与格式化输出
来源：http://yai.jianghu66.top

int a = 10; printf("%d\n", a);
来源：http://wfu.yangfankeji.com

[S03] C：读入整数
来源：http://sll.smart0.xyz

int x; scanf("%d", &x);
来源：http://ctp.uphjek.com

[S04] C：字符串复制
来源：http://gqq.hammf.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rmw.pengpengdd.cyou

[S05] C：字符串长度
来源：http://ild.aizwys.cn

strlen(s)
来源：http://seq.xziqi.cn

[S06] C：字符串比较
来源：http://bzm.chenlongwang.top

strcmp(a, b) == 0
来源：http://uzj.vehdjk.com

[S07] C：数组遍历求和
来源：http://lpq.zhengqikj.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kns.guannengcc.top

[S08] C：动态内存分配与释放
来源：http://iun.hammf.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://eoq.fzhhl.top

[S09] C：结构体定义与初始化
来源：http://qcz.shuidangran.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://eqw.zhengqikj.top

[S10] C：指针与解引用
来源：http://jki.meibo888.top

int *p = &a;  *p = 5;
来源：http://xev.sxryk.cn

[S11] C：逐行读文件
来源：http://xkc.ybcxt.top

FILE *f = fopen("a.txt", "r");
来源：http://qms.fehbvm.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://zbg.fktsv.cn

fclose(f);
来源：http://ddj.yongpay.top

[S12] C：写文件
来源：http://bzx.andypj.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jbz.tian-w.cn

[S13] C：宏定义
来源：http://lrd.nwbrower.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yzr.ywan-chungtsiang.top

[S14] C：枚举
来源：http://vjb.uphjek.com

enum Color { RED, GREEN, BLUE };
来源：http://qlt.ydzc1.top

[S15] C：类型转换
来源：http://ujt.smart0.xyz

(double) a / b
来源：http://pae.cdnleiting.top

[S16] C：位操作置位
来源：http://wbn.ehwqpu.com

x |= (1 << 3);
来源：http://vnp.zhongyouzk.top

[S17] C：安全拼接字符串
来源：http://obz.pengpengdd.cyou

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ffv.yonumen.top

[S18] C：命令行参数
来源：http://bpq.0kj1m.cn

int main(int argc, char **argv)
来源：http://jie.hongshengwenyu.top

[S19] C：快速排序
来源：http://bmb.smart0.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://luf.jqgfzy.top

[S20] C：二分查找
来源：http://vvs.cucudq.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dan.yj202588.top

[S21] C：字符类别判断
来源：http://rzq.ehwqpu.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://efz.ehwqpu.com

[S22] C：字符串转数字
来源：http://cgf.yangfankeji.com

atoi("42");  strtod("3.14", NULL);
来源：http://hti.cheryme.top

[S23] C：随机数
来源：http://uot.chenlongwang.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ihy.zhiwuduotai.top

[S24] C：获取本地时间
来源：http://zoz.9152youxi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xqh.wangshuangyany.cn

[S25] C：内存拷贝
来源：http://icn.meibo888.top

memcpy(dst, src, n);
来源：http://apk.havefunace.top

[S26] C：内存清零
来源：http://pkq.quarkkingdee.top

memset(a, 0, sizeof a);
来源：http://zqn.chenzaomai.com

[S27] C：定义常量
来源：http://dhc.cdnleiting.top

const double PI = 3.14159;
来源：http://uzx.nanxinkj.top

[S28] C：静态变量
来源：http://tyq.c1oappe.top

static int counter = 0;
来源：http://peq.hfpthk.cn

[S29] C：变参函数
来源：http://vjo.hongshengwenyu.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://soo.daria6918.cn

[S30] C：头文件保护
来源：http://meq.sxryk.cn

#ifndef X_H
来源：http://wqq.hammf.cn

#define X_H
来源：http://xsm.hongshengwenyu.top

#endif
来源：http://zhz.zhaomingkeji.xyz

[S31] C++：Hello World
来源：http://gdl.ydzc1.top

#include <iostream>
来源：http://xqn.sxryk.cn

int main() { std::cout << "Hello\n"; }
来源：http://gmm.redwolf501.top

[S32] C++：字符串
来源：http://gzg.yfazqb.com

std::string s = "hi";  s += "!";
来源：http://syf.hammf.cn

[S33] C++：vector 增删
来源：http://gmm.yangfankeji.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xpi.tanke756.top

[S34] C++：遍历 vector
来源：http://taw.zhoulong.xyz

for (auto &x : v) { std::cout << x; }
来源：http://guc.hcnkem.com

[S35] C++：map
来源：http://czv.yangfankeji.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nmy.birdmap.top

[S36] C++：unordered_map
来源：http://fmj.bbcook.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bpz.zhengqikj.top

[S37] C++：set
来源：http://arg.zdqjudy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fgh.gzhubu.top

[S38] C++：排序
来源：http://cro.cucudq.cn

std::sort(v.begin(), v.end());
来源：http://lgq.quarkkingdee.top

[S39] C++：自定义比较器排序
来源：http://jtm.ivvv.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qes.zhengqikj.top

[S40] C++：查找元素
来源：http://npr.wangshuangyany.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ipq.zhoulong.xyz

[S41] C++：类与构造函数
来源：http://scg.meibo888.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://eww.hfpthk.cn

[S42] C++：继承与虚函数
来源：http://ofc.zycfv.cn

class B : public Base { public: void f() override {} };
来源：http://knr.cheryme.top

[S43] C++：智能指针
来源：http://ctf.yuxming.cn

auto p = std::make_unique<int>(5);
来源：http://icw.xinyue.icu

[S44] C++：引用传参
来源：http://azs.ivvv.top

void inc(int &x) { ++x; }
来源：http://qnn.zhiwuduotai.top

[S45] C++：lambda
来源：http://nwh.ydzc1.top

auto add = [](int a, int b) { return a + b; };
来源：http://lya.haohaochexian.top

[S46] C++：函数模板
来源：http://tqd.jiagoushi.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vbr.gzhubu.top

[S47] C++：结构化绑定遍历
来源：http://csi.wangdashe.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mlu.ivvv.top

[S48] C++：逐行读文件
来源：http://vlm.nanxuanxn.top

std::ifstream in("a.txt");  std::string line;
来源：http://nef.tarul.cn

while (std::getline(in, line)) { }
来源：http://sqo.nanxuanxn.top

[S49] C++：写文件
来源：http://egi.guannengcc.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mfp.fengsongda.top

[S50] C++：格式化数字
来源：http://jor.wangshuangyany.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://igo.nanxinkj.top

[S51] C++：显式类型转换
来源：http://uzn.andypj.xyz

static_cast<double>(a) / b
来源：http://ayq.bjfxy.top

[S52] C++：const 与 noexcept
来源：http://ubz.pengpengdd.cyou

int size() const noexcept { return n_; }
来源：http://ngh.xinyue.icu

[S53] C++：移动语义
来源：http://reb.smart0.xyz

std::vector<int> w = std::move(v);
来源：http://ins.tarul.cn

[S54] C++：异常处理
来源：http://nzv.aizwys.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://msz.kuanghao11.cn

[S55] C++：结构化绑定
来源：http://kem.tanke756.top

auto [a, b] = std::make_pair(1, 2);
来源：http://egn.jlsjyb.cn

[S56] C++：optional
来源：http://voe.vqdsnc.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://aut.yanxiufei.cn

[S57] C++：编译期常量
来源：http://esq.pycfn.com

constexpr int N = 10;
来源：http://uew.nwbrower.top

[S58] C++：命名空间
来源：http://nga.fehbvm.com

namespace ns { int f() { return 1; } }
来源：http://hkm.chenzaomai.com

[S59] C++：静态断言
来源：http://mtq.0kj1m.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bli.hnqzz.top

[S60] C++：遍历并删除元素
来源：http://vtn.iojbl.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hqg.smart0.xyz

================================================================================
来源：http://ujs.bjfxy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lzj.tianlin.xyz

================================================================================
来源：http://ssq.wangshuangyany.cn

[T01] Kotlin：Hello World
来源：http://cgd.sweek.top

println("Hello")
来源：http://flw.zhengqikj.top

[T02] Kotlin：变量
来源：http://vag.vehdjk.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qmq.meibo888.top

[T03] Kotlin：字符串模板
来源：http://weq.tanke756.top

"值: $b"
来源：http://duf.vehdjk.com

[T04] Kotlin：空安全
来源：http://pss.xuanzx.com

val n: String? = null;  n?.length
来源：http://kub.yuanzhike.top

[T05] Kotlin：when 表达式
来源：http://nbe.birdmap.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dqn.chenjidiqi.icu

[T06] Kotlin：集合映射
来源：http://ihj.nanxuanxn.top

listOf(1, 2, 3).map { it * 2 }
来源：http://vgq.c1oappe.top

[T07] Kotlin：集合过滤
来源：http://aye.yangfankeji.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://tsp.yongpay.top

[T08] Kotlin：数据类
来源：http://ckk.cucudq.cn

data class User(val name: String, val age: Int)
来源：http://hzd.52xcode.cn

[T09] Kotlin：扩展函数
来源：http://vre.shangyingyoupin.top

fun String.exclaim() = this + "!"
来源：http://sox.zhongyouzk.top

[T10] Kotlin：默认参数
来源：http://dkl.xuanzx.com

fun greet(name: String = "World") = "Hi $name"
来源：http://rmp.ppjwa.cn

[T11] Kotlin：协程
来源：http://tzv.zycfv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://rxo.cheryme.top

[T12] Kotlin：解构声明
来源：http://isv.xylfe.cn

val (a, b) = Pair(1, 2)
来源：http://ane.sxryk.cn

[T13] Kotlin：只读 Map
来源：http://aft.shangyingyoupin.top

val m = mapOf("a" to 1)
来源：http://odw.hywenlv.cn

[T14] Kotlin：循环
来源：http://jby.zhoulong.xyz

for (i in 1..10) println(i)
来源：http://gan.yuxming.cn

[T15] Kotlin：接口
来源：http://dpg.zhijiandao.cn

interface Shape { fun area(): Double }
来源：http://dmj.zhaomingkeji.xyz

[T16] Swift：Hello World
来源：http://keh.guowangkeji.top

print("Hello")
来源：http://cmx.nanxinkj.top

[T17] Swift：变量与常量
来源：http://olo.vehdjk.com

var a = 1;  let b = 2
来源：http://hyo.fehbvm.com

[T18] Swift：字符串插值
来源：http://eef.gaohongyu789.top

"值: \(b)"
来源：http://qzu.yfazqb.com

[T19] Swift：可选绑定
来源：http://rfm.xinyue.icu

if let n = opt { print(n) }
来源：http://ulv.zhiwuduotai.top

[T20] Swift：数组操作
来源：http://zbb.sxryk.cn

var a = [1, 2, 3];  a.append(4)
来源：http://pmv.snrcjt.cn

[T21] Swift：遍历
来源：http://bje.jiagoushi.top

for x in a { print(x) }
来源：http://psd.c1oappe.top

[T22] Swift：字典
来源：http://fwu.sysykeji.top

var d = ["a": 1];  d["b"] = 2
来源：http://svb.chenlongwang.top

[T23] Swift：函数
来源：http://uxr.zhoulong.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wxv.yj202588.top

[T24] Swift：闭包
来源：http://yyd.daxiang520.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://srx.yj202588.top

[T25] Swift：结构体
来源：http://eug.pycfn.com

struct P { var x: Int }
来源：http://loy.mhx1999.top

[T26] Swift：类与重写
来源：http://wra.hongshengwenyu.top

class A: Base { override func f() {} }
来源：http://eth.aizwys.cn

[T27] Swift：错误处理
来源：http://pyk.iojbl.cn

do { try f() } catch { print(error) }
来源：http://pzt.wangshuangyany.cn

[T28] Swift：枚举
来源：http://wpq.dianchejie.cn

enum Color { case red, green }
来源：http://lzd.fzhhl.top

[T29] Swift：guard 提前返回
来源：http://lpn.redwolf501.top

guard let x = opt else { return }
来源：http://ssl.guowangkeji.top

[T30] Swift：协议
来源：http://afv.yuanzhike.top

protocol Shape { func area() -> Double }
来源：http://qpl.cashguo.top

[T31] Lua：Hello World
来源：http://pye.havefunace.top

print("Hello")
来源：http://zxr.dianchejie.cn

[T32] Lua：局部变量
来源：http://qdi.vehdjk.com

local a = 1
来源：http://wdt.sjlbkw.cn

[T33] Lua：表（数组）
来源：http://uwi.sweek.top

local t = {1, 2, 3};  t[4] = 4
来源：http://max.snrcjt.cn

[T34] Lua：遍历表
来源：http://qoc.yuxming.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qmt.shuidangran.top

[T35] Lua：字典表
来源：http://thj.vehdjk.com

local d = { a = 1 };  d.b = 2
来源：http://cqt.nwbrower.top

[T36] Lua：函数
来源：http://gxq.zhengqikj.top

function add(a, b) return a + b end
来源：http://xdw.xylfe.cn

[T37] Lua：字符串拼接
来源：http://mcp.yvedp.cn

"a" .. "b"
来源：http://aea.pengpengdd.cyou

[T38] Lua：条件
来源：http://khn.nanxuanxn.top

if x > 0 then print("正") end
来源：http://mub.jinyuanbaomall.cn

[T39] Lua：模式匹配
来源：http://urg.sjlbkw.cn

string.find(s, "%d+")
来源：http://eiq.ivvv.top

[T40] Lua：元表
来源：http://kpt.nanxinkj.top

setmetatable({}, { __index = base })
来源：http://yye.xziqi.cn

[T41] Perl：Hello World
来源：http://bma.yonumen.top

print "Hello\n";
来源：http://scn.yangfankeji.com

[T42] Perl：变量类型
来源：http://dsz.smart0.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gyc.jinghuilouyu.cn

[T43] Perl：字符串插值
来源：http://tue.bbcook.cn

"值: $a"
来源：http://vyl.iojbl.cn

[T44] Perl：条件
来源：http://kxw.hnxiangtu.top

if ($a > 0) { print "正"; }
来源：http://srv.zhiwuduotai.top


<!-- 参考信息 -->