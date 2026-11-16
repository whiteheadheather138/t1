代发 wailian999

cmd >/dev/null 2>&1
来源：http://mtw.tarul.cn

[R42] 输入重定向
来源：http://ale.chenlongwang.top

wc -l < a.txt
来源：http://qgq.ydjk.org.cn

[R43] 按名字查找文件
来源：http://wsq.9152youxi.cn

find . -name "*.log" -type f
来源：http://fbt.ydjk.org.cn

[R44] 按修改时间查找
来源：http://ksq.pycfn.com

find . -mtime -7 -type f
来源：http://omm.hcnkem.com

[R45] 批量删除
来源：http://tya.fktsv.cn

find . -name "*.tmp" -delete
来源：http://ybo.fanxiaobao.xyz

[R46] 递归替换文件内容
来源：http://fju.zhixingplan.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ckc.redwolf501.top

[R47] sed 单行替换
来源：http://oou.gaohongyu789.top

sed -i 's/foo/bar/g' a.txt
来源：http://kfp.zhoulong.xyz

[R48] awk 取指定列
来源：http://qrp.hnxiangtu.top

awk '{print $1, $3}' a.txt
来源：http://knj.hnxiangtu.top

[R49] awk 带条件
来源：http://qjz.cheryme.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gjc.shzxlz.cn

[R50] awk 求和
来源：http://ciq.aibaodan.cn

awk '{s += $2} END {print s}' a.txt
来源：http://njp.guannengcc.top

[R51] 排序去重取前几
来源：http://pge.hesvh.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ogk.fzhhl.top

[R52] 统计行数
来源：http://urj.yonumen.top

wc -l a.txt
来源：http://cpi.gotoacloud.top

[R53] 查看文件头与实时尾
来源：http://exl.andypj.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ppr.jqgfzy.top

[R54] 比较两个文件
来源：http://hns.gogol.net.cn

diff a.txt b.txt
来源：http://liw.epnwcf.com

[R55] 压缩与解压
来源：http://mcy.ppjwa.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://iex.zhijiandao.cn

[R56] 远程拷贝
来源：http://vny.ivvv.top

scp file user@host:/path/
来源：http://ceb.316326.xyz

[R57] 远程执行命令
来源：http://oii.havefunace.top

ssh user@host 'uptime'
来源：http://ohl.fktsv.cn

[R58] 下载文件
来源：http://bjb.haohaochexian.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wwg.gotoacloud.top

[R59] 发 POST JSON
来源：http://ift.daxiang520.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rwu.shanyushiyangkeji.top

[R60] 只看 HTTP 状态码
来源：http://ove.pengpengdd.cyou

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bwk.xinyue.icu

[R61] 磁盘占用
来源：http://bvf.zhoulong.xyz

df -h;  du -sh *
来源：http://wpq.tianlin.xyz

[R62] 找最占空间的文件
来源：http://ryo.cqqwz.cn

du -ah . | sort -rh | head -10
来源：http://hyf.shanyushiyangkeji.top

[R63] 内存与进程
来源：http://etc.pycfn.com

free -h;  ps aux | grep nginx
来源：http://mpw.yueranfly.top

[R64] 结束进程
来源：http://adr.wangdashe.top

kill -9 $(pgrep -f app.py)
来源：http://ouu.vehdjk.com

[R65] 查看端口占用
来源：http://qtk.aibaodan.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qzs.hnxiangtu.top

[R66] 定时任务
来源：http://qas.quarkkingdee.top

crontab -e;  crontab -l
来源：http://hsf.zhijiandao.cn

[R67] 生成随机十六进制串
来源：http://olz.9152youxi.cn

openssl rand -hex 16
来源：http://uuw.xuetiantiany.cn

[R68] 计算文件校验值
来源：http://qaa.cucudq.cn

sha256sum a.txt;  md5sum a.txt
来源：http://kzo.tanke756.top

[R69] 生成随机密码
来源：http://zwi.jianghu66.top

head -c 16 /dev/urandom | base64
来源：http://fbh.hnqzz.top

[R70] 时间戳与互转
来源：http://ywn.zhoulong.xyz

date +%s;  date -d @1700000000
来源：http://uig.pycfn.com

[R71] 日期格式化
来源：http://dam.316326.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://zdo.gaohongyu789.top

[R72] 等待端口就绪
来源：http://cer.hongshengwenyu.top

until nc -z localhost 3306; do sleep 1; done
来源：http://rsn.hywenlv.cn

[R73] 分割大日志
来源：http://zrq.jianghu66.top

split -l 1000 big.log part_
来源：http://bir.wangshuangyany.cn

[R74] 批量重命名
来源：http://tae.yuxming.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bfb.sxryk.cn

[R75] 导出环境变量
来源：http://qnb.nanxuanxn.top

export PATH="$HOME/bin:$PATH"
来源：http://tvi.hammf.cn

[R76] 使用临时文件
来源：http://whk.yanxiufei.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://scz.wangdashe.top

[R77] 读取用户输入
来源：http://deo.yuanzhike.top

read -rp "请输入: " ans
来源：http://fec.hywenlv.cn

[R78] 交互式菜单
来源：http://jki.zhaomingkeji.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://dnv.zdqjudy.top

[R79] 解析命令行选项
来源：http://qrv.xziqi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xpl.yueranfly.top

[R80] 查看脚本执行耗时
来源：http://jwn.ctjpmb.com

time ./run.sh
来源：http://xfh.birdmap.top

================================================================================
来源：http://xpu.daxiang520.top

S. C / C++ 专题
来源：http://izl.hcnkem.com

================================================================================
来源：http://hop.xingfuxueyuan.xyz

[S01] C：Hello World
来源：http://djp.zhengqikj.top

#include <stdio.h>
来源：http://qyi.birdmap.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://wfr.nanxinkj.top

[S02] C：变量与格式化输出
来源：http://xwx.kuanghao11.cn

int a = 10; printf("%d\n", a);
来源：http://szs.zdqjudy.top

[S03] C：读入整数
来源：http://ycm.zhengqikj.top

int x; scanf("%d", &x);
来源：http://axz.gogol.net.cn

[S04] C：字符串复制
来源：http://rvy.xuetiantiany.cn

char dst[32]; strcpy(dst, "hi");
来源：http://saj.pengpengdd.cyou

[S05] C：字符串长度
来源：http://rzo.jinqigufen.top

strlen(s)
来源：http://kdp.xylfe.cn

[S06] C：字符串比较
来源：http://ude.meibo888.top

strcmp(a, b) == 0
来源：http://kvo.fzhhl.top

[S07] C：数组遍历求和
来源：http://xlz.cdnleiting.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sab.zdbjq.cn

[S08] C：动态内存分配与释放
来源：http://pvy.316326.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://eqh.dianchejie.cn

[S09] C：结构体定义与初始化
来源：http://cei.sweek.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sxm.zdqjudy.top

[S10] C：指针与解引用
来源：http://fzn.ctjpmb.com

int *p = &a;  *p = 5;
来源：http://krd.sysykeji.top

[S11] C：逐行读文件
来源：http://jlq.epnwcf.com

FILE *f = fopen("a.txt", "r");
来源：http://pna.gaohongyu789.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://otp.shanyushiyangtech.top

fclose(f);
来源：http://yzz.ppjwa.cn

[S12] C：写文件
来源：http://bzp.ivvv.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ctb.ehwqpu.com

[S13] C：宏定义
来源：http://nvt.fanxiaobao.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ljk.hnqzz.top

[S14] C：枚举
来源：http://pja.jiagoushi.top

enum Color { RED, GREEN, BLUE };
来源：http://ylx.zhengqikj.top

[S15] C：类型转换
来源：http://xsb.hnxiangtu.top

(double) a / b
来源：http://jpg.chenlongwang.top

[S16] C：位操作置位
来源：http://zgu.snrcjt.cn

x |= (1 << 3);
来源：http://zaj.guannengcc.top

[S17] C：安全拼接字符串
来源：http://git.xingfuxueyuan.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wdw.vqdsnc.cn

[S18] C：命令行参数
来源：http://ltm.aibaodan.cn

int main(int argc, char **argv)
来源：http://kvd.hesvh.cn

[S19] C：快速排序
来源：http://xfq.gotoacloud.top

qsort(a, n, sizeof(int), cmp);
来源：http://saq.vqdsnc.cn

[S20] C：二分查找
来源：http://kqz.pycfn.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vem.uphjek.com

[S21] C：字符类别判断
来源：http://wbn.yuxming.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lwx.bbcook.cn

[S22] C：字符串转数字
来源：http://zms.wangshuangyany.cn

atoi("42");  strtod("3.14", NULL);
来源：http://icb.sufxvd.cn

[S23] C：随机数
来源：http://zwn.hywenlv.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://tpq.c1oappe.top

[S24] C：获取本地时间
来源：http://osc.ppjwa.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fwh.52xcode.cn

[S25] C：内存拷贝
来源：http://dod.shangyingyoupin.top

memcpy(dst, src, n);
来源：http://czm.yj20258888.top

[S26] C：内存清零
来源：http://yva.yuanzhike.top

memset(a, 0, sizeof a);
来源：http://lic.yongpay.top

[S27] C：定义常量
来源：http://ilk.hywenlv.cn

const double PI = 3.14159;
来源：http://nps.redwolf501.top

[S28] C：静态变量
来源：http://rih.zhaomingkeji.xyz

static int counter = 0;
来源：http://nug.redwolf501.top

[S29] C：变参函数
来源：http://ipc.pycfn.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bnx.zhengqikj.top

[S30] C：头文件保护
来源：http://vug.gogol.net.cn

#ifndef X_H
来源：http://lcu.jianghu66.top

#define X_H
来源：http://bld.jinyuanbaomall.cn

#endif
来源：http://azf.fehbvm.com

[S31] C++：Hello World
来源：http://suj.hongshengwenyu.top

#include <iostream>
来源：http://fgo.yj20258888.top

int main() { std::cout << "Hello\n"; }
来源：http://fqw.birdmap.top

[S32] C++：字符串
来源：http://zni.kuanghao11.cn

std::string s = "hi";  s += "!";
来源：http://utj.ydzc1.top

[S33] C++：vector 增删
来源：http://qbz.epnwcf.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nll.ppjwa.cn

[S34] C++：遍历 vector
来源：http://yae.shuidangran.top

for (auto &x : v) { std::cout << x; }
来源：http://ait.sufxvd.cn

[S35] C++：map
来源：http://ouw.zdqjudy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gxh.wangdashe.top

[S36] C++：unordered_map
来源：http://nye.yanxiufei.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lsd.jianghu66.top

[S37] C++：set
来源：http://qgl.andypj.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jqc.jyoumei.cn

[S38] C++：排序
来源：http://lzj.jianghu66.top

std::sort(v.begin(), v.end());
来源：http://byu.sufxvd.cn

[S39] C++：自定义比较器排序
来源：http://ggs.pycfn.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tlh.cucudq.cn

[S40] C++：查找元素
来源：http://txb.chenjidiqi.icu

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yhi.aizwys.cn

[S41] C++：类与构造函数
来源：http://hfo.jiagoushi.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vth.zycfv.cn

[S42] C++：继承与虚函数
来源：http://xva.jlsjyb.cn

class B : public Base { public: void f() override {} };
来源：http://sqj.xinyue.icu

[S43] C++：智能指针
来源：http://vwo.smart0.xyz

auto p = std::make_unique<int>(5);
来源：http://ikd.cashguo.top

[S44] C++：引用传参
来源：http://qnr.aizwys.cn

void inc(int &x) { ++x; }
来源：http://kzj.yj20258.top

[S45] C++：lambda
来源：http://ocs.vehdjk.com

auto add = [](int a, int b) { return a + b; };
来源：http://ucv.gzhubu.top

[S46] C++：函数模板
来源：http://vkv.zdbjq.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qvh.cashguo.top

[S47] C++：结构化绑定遍历
来源：http://tjv.sweek.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ylh.hammf.cn

[S48] C++：逐行读文件
来源：http://tai.hysaishi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://mik.feifeiyinyue.top

while (std::getline(in, line)) { }
来源：http://ddk.ivvv.top

[S49] C++：写文件
来源：http://swh.316326.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uff.jinqigfzy.top

[S50] C++：格式化数字
来源：http://ysr.ybcxt.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vhf.hfpthk.cn

[S51] C++：显式类型转换
来源：http://xxj.feifeiyinyue.top

static_cast<double>(a) / b
来源：http://tgu.shanyushiyangkeji.top

[S52] C++：const 与 noexcept
来源：http://opg.svipenyu.cn

int size() const noexcept { return n_; }
来源：http://bvt.jinqigfzy.top

[S53] C++：移动语义
来源：http://oys.tanke756.top

std::vector<int> w = std::move(v);
来源：http://hmn.sjlbkw.cn

[S54] C++：异常处理
来源：http://dfs.tian-w.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yno.52xcode.cn

[S55] C++：结构化绑定
来源：http://hhv.shangyingyoupin.top

auto [a, b] = std::make_pair(1, 2);
来源：http://xlg.jlsjyb.cn

[S56] C++：optional
来源：http://loz.gogol.net.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rfv.hesvh.cn

[S57] C++：编译期常量
来源：http://wnx.fehbvm.com

constexpr int N = 10;
来源：http://gmk.gzhubu.top

[S58] C++：命名空间
来源：http://sbg.yfazqb.com

namespace ns { int f() { return 1; } }
来源：http://zvo.jlsjyb.cn

[S59] C++：静态断言
来源：http://rww.yonumen.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qlv.hysaishi.cn

[S60] C++：遍历并删除元素
来源：http://naq.ehwqpu.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pev.xylfe.cn

================================================================================
来源：http://pdi.xziqi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://did.xziqi.cn

================================================================================
来源：http://nuv.aibaodan.cn

[T01] Kotlin：Hello World
来源：http://axe.gaohongyu789.top

println("Hello")
来源：http://qpr.smart0.xyz

[T02] Kotlin：变量
来源：http://leb.xylfe.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://glt.zhaomingkeji.xyz

[T03] Kotlin：字符串模板
来源：http://wbe.zhongyouzk.top

"值: $b"
来源：http://sfx.sxryk.cn

[T04] Kotlin：空安全
来源：http://fkb.tianlin.xyz

val n: String? = null;  n?.length
来源：http://ngw.52xcode.cn

[T05] Kotlin：when 表达式
来源：http://ens.haohaochexian.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hwz.sweek.top

[T06] Kotlin：集合映射
来源：http://cwq.yanxiufei.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://lus.jinghuilouyu.cn

[T07] Kotlin：集合过滤
来源：http://ccn.guannengcc.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://loq.fktsv.cn

[T08] Kotlin：数据类
来源：http://bgc.tian-w.cn

data class User(val name: String, val age: Int)
来源：http://smm.jqgufenzy.top

[T09] Kotlin：扩展函数
来源：http://fau.fehbvm.com

fun String.exclaim() = this + "!"
来源：http://tsu.mhx1999.top

[T10] Kotlin：默认参数
来源：http://oyg.cheryme.top

fun greet(name: String = "World") = "Hi $name"
来源：http://rke.ctjpmb.com

[T11] Kotlin：协程
来源：http://atr.andypj.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://rqc.jinqigufen.top

[T12] Kotlin：解构声明
来源：http://pbh.jiagoushi.top

val (a, b) = Pair(1, 2)
来源：http://hps.gaohongyu789.top

[T13] Kotlin：只读 Map
来源：http://axt.sxryk.cn

val m = mapOf("a" to 1)
来源：http://xkw.dianchejie.cn

[T14] Kotlin：循环
来源：http://ynr.zycfv.cn

for (i in 1..10) println(i)
来源：http://hcg.cashguo.top

[T15] Kotlin：接口
来源：http://rvs.sufxvd.cn

interface Shape { fun area(): Double }
来源：http://jak.hesvh.cn

[T16] Swift：Hello World
来源：http://cpk.xuetiantiany.cn

print("Hello")
来源：http://tje.zycfv.cn

[T17] Swift：变量与常量
来源：http://ely.bbcook.cn

var a = 1;  let b = 2
来源：http://nef.zhiwuduotai.top

[T18] Swift：字符串插值
来源：http://tei.yuxming.cn

"值: \(b)"
来源：http://fvj.jyoumei.cn

[T19] Swift：可选绑定
来源：http://wse.9152youxi.cn

if let n = opt { print(n) }
来源：http://peg.wangdashe.top

[T20] Swift：数组操作
来源：http://esw.ydjk.org.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fwn.yonumen.top

[T21] Swift：遍历
来源：http://shk.cdnleiting.top

for x in a { print(x) }
来源：http://aqz.yvedp.cn

[T22] Swift：字典
来源：http://ukf.jinghuilouyu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://rqd.jianghu66.top

[T23] Swift：函数
来源：http://mot.jinqigufen.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://met.xingfuxueyuan.xyz

[T24] Swift：闭包
来源：http://chm.chenlongwang.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ccx.9152youxi.cn

[T25] Swift：结构体
来源：http://fdu.jianghu66.top

struct P { var x: Int }
来源：http://ozk.hcnkem.com

[T26] Swift：类与重写
来源：http://dtv.cheryme.top

class A: Base { override func f() {} }
来源：http://ysu.pycfn.com

[T27] Swift：错误处理
来源：http://vct.nwbrower.top

do { try f() } catch { print(error) }
来源：http://aqz.ctjpmb.com

[T28] Swift：枚举
来源：http://tds.xingfuxueyuan.xyz

enum Color { case red, green }
来源：http://nti.gzhubu.top

[T29] Swift：guard 提前返回
来源：http://dwk.yj20258.top

guard let x = opt else { return }
来源：http://snw.zdqjudy.top

[T30] Swift：协议
来源：http://wze.guannengcc.top

protocol Shape { func area() -> Double }
来源：http://xpy.havefunace.top

[T31] Lua：Hello World
来源：http://paa.nwbrower.top

print("Hello")
来源：http://bii.aibaodan.cn

[T32] Lua：局部变量
来源：http://shq.gotoacloud.top

local a = 1
来源：http://qrb.hesvh.cn

[T33] Lua：表（数组）
来源：http://ldp.yfazqb.com

local t = {1, 2, 3};  t[4] = 4
来源：http://cvt.pycfn.com

[T34] Lua：遍历表
来源：http://nih.jinqigufen.top

for i, v in ipairs(t) do print(i, v) end
来源：http://cxf.ivvv.top

[T35] Lua：字典表
来源：http://qjq.dianchejie.cn

local d = { a = 1 };  d.b = 2
来源：http://vns.jqgufenzy.top

[T36] Lua：函数
来源：http://utg.guowangkeji.top

function add(a, b) return a + b end
来源：http://nay.52xcode.cn

[T37] Lua：字符串拼接
来源：http://bdw.xziqi.cn

"a" .. "b"
来源：http://lwt.vqdsnc.cn

[T38] Lua：条件
来源：http://llu.zycfv.cn

if x > 0 then print("正") end
来源：http://lrm.shanyushiyangtech.top

[T39] Lua：模式匹配
来源：http://kbs.redwolf501.top

string.find(s, "%d+")
来源：http://goc.hcnkem.com

[T40] Lua：元表
来源：http://eid.quarkkingdee.top

setmetatable({}, { __index = base })
来源：http://izq.snrcjt.cn

[T41] Perl：Hello World
来源：http://fqh.shuidangran.top

print "Hello\n";
来源：http://hmy.yueranfly.top

[T42] Perl：变量类型
来源：http://zvm.daria6918.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://uyp.chenzaomai.com

[T43] Perl：字符串插值
来源：http://fhq.uphjek.com

"值: $a"
来源：http://xhw.jianghu66.top

[T44] Perl：条件
来源：http://ybf.jiagoushi.top

if ($a > 0) { print "正"; }
来源：http://dsy.yvedp.cn


<!-- 参考信息 -->