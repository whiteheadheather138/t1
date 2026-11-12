代发 wailian999

find . -name "*.tmp" -delete
来源：http://mmb.zdbjq.cn

[R46] 递归替换文件内容
来源：http://oej.ywan-chungtsiang.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zqe.smart0.xyz

[R47] sed 单行替换
来源：http://ean.gzhubu.top

sed -i 's/foo/bar/g' a.txt
来源：http://yxw.birdmap.top

[R48] awk 取指定列
来源：http://gno.hongshengwenyu.top

awk '{print $1, $3}' a.txt
来源：http://eej.dashuyun.cn

[R49] awk 带条件
来源：http://npy.wangdashe.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://eom.wangshuangyany.cn

[R50] awk 求和
来源：http://ufn.hysaishi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://mqp.pycfn.com

[R51] 排序去重取前几
来源：http://vvk.jinghuilouyu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qpw.cashguo.top

[R52] 统计行数
来源：http://sto.daria6918.cn

wc -l a.txt
来源：http://mxr.zhiwuduotai.top

[R53] 查看文件头与实时尾
来源：http://rca.zhengqikj.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mfu.pycfn.com

[R54] 比较两个文件
来源：http://sws.zhijiandao.cn

diff a.txt b.txt
来源：http://plw.fanxiaobao.xyz

[R55] 压缩与解压
来源：http://ces.ivvv.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jmb.vehdjk.com

[R56] 远程拷贝
来源：http://cuw.fktsv.cn

scp file user@host:/path/
来源：http://fkz.zdqjudy.top

[R57] 远程执行命令
来源：http://elf.52xcode.cn

ssh user@host 'uptime'
来源：http://mhp.gzhubu.top

[R58] 下载文件
来源：http://vzp.cqqwz.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wkg.hnxiangtu.top

[R59] 发 POST JSON
来源：http://mgn.zycfv.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rht.birdmap.top

[R60] 只看 HTTP 状态码
来源：http://iyz.fehbvm.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mqe.yonumen.top

[R61] 磁盘占用
来源：http://ikh.andypj.xyz

df -h;  du -sh *
来源：http://oct.sjlbkw.cn

[R62] 找最占空间的文件
来源：http://ejp.xziqi.cn

du -ah . | sort -rh | head -10
来源：http://czw.c1oappe.top

[R63] 内存与进程
来源：http://yst.dianchejie.cn

free -h;  ps aux | grep nginx
来源：http://mcf.zdbjq.cn

[R64] 结束进程
来源：http://tkm.zhongyouzk.top

kill -9 $(pgrep -f app.py)
来源：http://ciu.yonumen.top

[R65] 查看端口占用
来源：http://ikc.fanxiaobao.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xaq.svipenyu.cn

[R66] 定时任务
来源：http://opy.yj20258.top

crontab -e;  crontab -l
来源：http://wam.xingfuxueyuan.xyz

[R67] 生成随机十六进制串
来源：http://zun.feifeiyinyue.top

openssl rand -hex 16
来源：http://utb.dashuyun.cn

[R68] 计算文件校验值
来源：http://lfv.chenjidiqi.icu

sha256sum a.txt;  md5sum a.txt
来源：http://qel.pengpengdd.cyou

[R69] 生成随机密码
来源：http://til.birdmap.top

head -c 16 /dev/urandom | base64
来源：http://nit.guowangkeji.top

[R70] 时间戳与互转
来源：http://ibu.cashguo.top

date +%s;  date -d @1700000000
来源：http://koz.sweek.top

[R71] 日期格式化
来源：http://uxv.dashuyun.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://oiq.daria6918.cn

[R72] 等待端口就绪
来源：http://fwg.jinghuilouyu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dlf.yj202588.top

[R73] 分割大日志
来源：http://hat.tanke756.top

split -l 1000 big.log part_
来源：http://wge.hnxiangtu.top

[R74] 批量重命名
来源：http://qcd.fzhhl.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://znm.guannengcc.top

[R75] 导出环境变量
来源：http://rar.yj202588.top

export PATH="$HOME/bin:$PATH"
来源：http://fzm.zdbjq.cn

[R76] 使用临时文件
来源：http://rxb.fanxiaobao.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ikv.uphjek.com

[R77] 读取用户输入
来源：http://xhf.ehwqpu.com

read -rp "请输入: " ans
来源：http://nnt.sufxvd.cn

[R78] 交互式菜单
来源：http://yrw.yj202588.top

select opt in a b c; do echo "$opt"; break; done
来源：http://mrw.sjlbkw.cn

[R79] 解析命令行选项
来源：http://okg.fzhhl.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ywc.sjlbkw.cn

[R80] 查看脚本执行耗时
来源：http://ihp.gzhubu.top

time ./run.sh
来源：http://ajc.iojbl.cn

================================================================================
来源：http://gtc.cheryme.top

S. C / C++ 专题
来源：http://rbj.pycfn.com

================================================================================
来源：http://gcr.meibo888.top

[S01] C：Hello World
来源：http://iqx.aizwys.cn

#include <stdio.h>
来源：http://eor.jqgufenzy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ihw.52xcode.cn

[S02] C：变量与格式化输出
来源：http://kmp.hfpthk.cn

int a = 10; printf("%d\n", a);
来源：http://efe.nwbrower.top

[S03] C：读入整数
来源：http://dxb.jinghuilouyu.cn

int x; scanf("%d", &x);
来源：http://bwi.yvedp.cn

[S04] C：字符串复制
来源：http://nlw.ctjpmb.com

char dst[32]; strcpy(dst, "hi");
来源：http://gwb.ehwqpu.com

[S05] C：字符串长度
来源：http://tol.xuetiantiany.cn

strlen(s)
来源：http://obd.dashuyun.cn

[S06] C：字符串比较
来源：http://tyg.kuanghao11.cn

strcmp(a, b) == 0
来源：http://zwt.gaohongyu789.top

[S07] C：数组遍历求和
来源：http://vaf.gzhubu.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://otc.c1oappe.top

[S08] C：动态内存分配与释放
来源：http://jhw.epnwcf.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nat.yj202588.top

[S09] C：结构体定义与初始化
来源：http://kax.fanxiaobao.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ylu.guannengcc.top

[S10] C：指针与解引用
来源：http://otg.redwolf501.top

int *p = &a;  *p = 5;
来源：http://jeq.hcnkem.com

[S11] C：逐行读文件
来源：http://mjz.shanyushiyangtech.top

FILE *f = fopen("a.txt", "r");
来源：http://mmx.jianghu66.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://roz.daxiang520.top

fclose(f);
来源：http://cqo.jinqigufen.top

[S12] C：写文件
来源：http://yrq.xylfe.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://exu.jinyuanbaomall.cn

[S13] C：宏定义
来源：http://lok.fktsv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wif.meibo888.top

[S14] C：枚举
来源：http://gtf.yanxiufei.cn

enum Color { RED, GREEN, BLUE };
来源：http://wya.daxiang520.top

[S15] C：类型转换
来源：http://idh.zhongyouzk.top

(double) a / b
来源：http://zoz.chenlongwang.top

[S16] C：位操作置位
来源：http://iea.sjlbkw.cn

x |= (1 << 3);
来源：http://sbi.jinghuilouyu.cn

[S17] C：安全拼接字符串
来源：http://pin.tian-w.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://opx.nanxuanxn.top

[S18] C：命令行参数
来源：http://mak.zdqjudy.top

int main(int argc, char **argv)
来源：http://vvm.sweek.top

[S19] C：快速排序
来源：http://urp.vqdsnc.cn

qsort(a, n, sizeof(int), cmp);
来源：http://exn.nanxuanxn.top

[S20] C：二分查找
来源：http://coz.quarkkingdee.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dqk.nanxinkj.top

[S21] C：字符类别判断
来源：http://gxm.zdqjudy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cqp.jinqigufen.top

[S22] C：字符串转数字
来源：http://yat.zhongyouzk.top

atoi("42");  strtod("3.14", NULL);
来源：http://per.kuanghao11.cn

[S23] C：随机数
来源：http://bdu.pycfn.com

srand(time(NULL));  int r = rand() % 100;
来源：http://zkb.yuxming.cn

[S24] C：获取本地时间
来源：http://wsm.nanxinkj.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ckz.jinqigfzy.top

[S25] C：内存拷贝
来源：http://agl.ydzc1.top

memcpy(dst, src, n);
来源：http://zzw.andypj.xyz

[S26] C：内存清零
来源：http://bpd.xuanzx.com

memset(a, 0, sizeof a);
来源：http://kky.tian-w.cn

[S27] C：定义常量
来源：http://gxn.epnwcf.com

const double PI = 3.14159;
来源：http://gjd.fanxiaobao.xyz

[S28] C：静态变量
来源：http://oec.hnqzz.top

static int counter = 0;
来源：http://buu.zhaomingkeji.xyz

[S29] C：变参函数
来源：http://snd.aizwys.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jkq.hywenlv.cn

[S30] C：头文件保护
来源：http://vpp.yj202588.top

#ifndef X_H
来源：http://pww.fengsongda.top

#define X_H
来源：http://eoe.cqqwz.cn

#endif
来源：http://hjv.jyoumei.cn

[S31] C++：Hello World
来源：http://chr.sysykeji.top

#include <iostream>
来源：http://lnr.cqqwz.cn

int main() { std::cout << "Hello\n"; }
来源：http://als.yonumen.top

[S32] C++：字符串
来源：http://esk.bjfxy.top

std::string s = "hi";  s += "!";
来源：http://jpo.tanke756.top

[S33] C++：vector 增删
来源：http://fop.vqdsnc.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://anu.xylfe.cn

[S34] C++：遍历 vector
来源：http://lce.cdnleiting.top

for (auto &x : v) { std::cout << x; }
来源：http://fow.yfazqb.com

[S35] C++：map
来源：http://hxp.vehdjk.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nak.tianlin.xyz

[S36] C++：unordered_map
来源：http://jvy.aizwys.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cfn.yanxiufei.cn

[S37] C++：set
来源：http://phe.hnqzz.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zpw.uphjek.com

[S38] C++：排序
来源：http://goh.nwbrower.top

std::sort(v.begin(), v.end());
来源：http://ghk.sweek.top

[S39] C++：自定义比较器排序
来源：http://sbp.fehbvm.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zgu.jinyuanbaomall.cn

[S40] C++：查找元素
来源：http://vqz.chenjidiqi.icu

auto it = std::find(v.begin(), v.end(), 3);
来源：http://omz.jqgufenzy.top

[S41] C++：类与构造函数
来源：http://slc.vqdsnc.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sou.kuanghao11.cn

[S42] C++：继承与虚函数
来源：http://zyp.pycfn.com

class B : public Base { public: void f() override {} };
来源：http://mlf.shanyushiyangkeji.top

[S43] C++：智能指针
来源：http://hgu.ivvv.top

auto p = std::make_unique<int>(5);
来源：http://jlq.dashuyun.cn

[S44] C++：引用传参
来源：http://ddw.cheryme.top

void inc(int &x) { ++x; }
来源：http://was.aizwys.cn

[S45] C++：lambda
来源：http://dic.tanke756.top

auto add = [](int a, int b) { return a + b; };
来源：http://xhf.hnxiangtu.top

[S46] C++：函数模板
来源：http://xhp.yuxming.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cty.snrcjt.cn

[S47] C++：结构化绑定遍历
来源：http://lhs.hcnkem.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://chr.zhoulong.xyz

[S48] C++：逐行读文件
来源：http://ngs.yanxiufei.cn

std::ifstream in("a.txt");  std::string line;
来源：http://oom.fktsv.cn

while (std::getline(in, line)) { }
来源：http://mbv.yuxming.cn

[S49] C++：写文件
来源：http://srj.tanke756.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blr.cheryme.top

[S50] C++：格式化数字
来源：http://iie.hesvh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qfk.yvedp.cn

[S51] C++：显式类型转换
来源：http://gqu.yangfankeji.com

static_cast<double>(a) / b
来源：http://nzt.kuanghao11.cn

[S52] C++：const 与 noexcept
来源：http://fej.jinyuanbaomall.cn

int size() const noexcept { return n_; }
来源：http://eed.uphjek.com

[S53] C++：移动语义
来源：http://zhk.xuanzx.com

std::vector<int> w = std::move(v);
来源：http://epu.svipenyu.cn

[S54] C++：异常处理
来源：http://hnt.zdbjq.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bcx.ydjk.org.cn

[S55] C++：结构化绑定
来源：http://kul.daria6918.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ppl.pycfn.com

[S56] C++：optional
来源：http://zmk.wangdashe.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://shw.xuanzx.com

[S57] C++：编译期常量
来源：http://cha.316326.xyz

constexpr int N = 10;
来源：http://kie.tarul.cn

[S58] C++：命名空间
来源：http://ule.andypj.xyz

namespace ns { int f() { return 1; } }
来源：http://ovl.daxiang520.top

[S59] C++：静态断言
来源：http://igt.yfazqb.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://awv.jinghuilouyu.cn

[S60] C++：遍历并删除元素
来源：http://exj.vqdsnc.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://czv.fanxiaobao.xyz

================================================================================
来源：http://xgn.gaohongyu789.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://skz.shanyushiyangkeji.top

================================================================================
来源：http://vsr.0kj1m.cn

[T01] Kotlin：Hello World
来源：http://plb.jqgfzy.top

println("Hello")
来源：http://sxy.jiagoushi.top

[T02] Kotlin：变量
来源：http://cjs.nanxinkj.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vou.guannengcc.top

[T03] Kotlin：字符串模板
来源：http://gmv.tian-w.cn

"值: $b"
来源：http://spx.zhiwuduotai.top

[T04] Kotlin：空安全
来源：http://fly.shangyingyoupin.top

val n: String? = null;  n?.length
来源：http://npb.jqgufenzy.top

[T05] Kotlin：when 表达式
来源：http://ywx.hesvh.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zuj.hongshengwenyu.top

[T06] Kotlin：集合映射
来源：http://kxb.fanxiaobao.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://bpx.xylfe.cn

[T07] Kotlin：集合过滤
来源：http://mlk.sufxvd.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://beo.jinghuilouyu.cn

[T08] Kotlin：数据类
来源：http://idi.zhoulong.xyz

data class User(val name: String, val age: Int)
来源：http://wuj.jlsjyb.cn

[T09] Kotlin：扩展函数
来源：http://ist.c1oappe.top

fun String.exclaim() = this + "!"
来源：http://jtx.svipenyu.cn

[T10] Kotlin：默认参数
来源：http://vbo.ppjwa.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pdy.ydjk.org.cn

[T11] Kotlin：协程
来源：http://irq.yonumen.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://swm.nwbrower.top

[T12] Kotlin：解构声明
来源：http://vmn.fengsongda.top

val (a, b) = Pair(1, 2)
来源：http://ckx.yuxming.cn

[T13] Kotlin：只读 Map
来源：http://jqc.hfpthk.cn

val m = mapOf("a" to 1)
来源：http://yvi.snrcjt.cn

[T14] Kotlin：循环
来源：http://jvc.ydjk.org.cn

for (i in 1..10) println(i)
来源：http://tiq.cucudq.cn

[T15] Kotlin：接口
来源：http://gdm.vehdjk.com

interface Shape { fun area(): Double }
来源：http://jpr.jlsjyb.cn

[T16] Swift：Hello World
来源：http://ndc.gaohongyu789.top

print("Hello")
来源：http://ago.meibo888.top

[T17] Swift：变量与常量
来源：http://agl.birdmap.top

var a = 1;  let b = 2
来源：http://iww.bjfxy.top

[T18] Swift：字符串插值
来源：http://fmb.cdnleiting.top

"值: \(b)"
来源：http://pue.zdbjq.cn

[T19] Swift：可选绑定
来源：http://hhs.hnqzz.top

if let n = opt { print(n) }
来源：http://ohz.jqgufenzy.top

[T20] Swift：数组操作
来源：http://gim.sweek.top

var a = [1, 2, 3];  a.append(4)
来源：http://pfz.sufxvd.cn

[T21] Swift：遍历
来源：http://asn.andypj.xyz

for x in a { print(x) }
来源：http://nim.hammf.cn

[T22] Swift：字典
来源：http://eyj.shzxlz.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mco.quarkkingdee.top

[T23] Swift：函数
来源：http://tof.nanxuanxn.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xlx.pengpengdd.cyou

[T24] Swift：闭包
来源：http://efx.haohaochexian.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://qrf.xingfuxueyuan.xyz

[T25] Swift：结构体
来源：http://wnz.sxryk.cn

struct P { var x: Int }
来源：http://zdp.zdbjq.cn

[T26] Swift：类与重写
来源：http://fgh.sweek.top

class A: Base { override func f() {} }
来源：http://nbg.tanke756.top

[T27] Swift：错误处理
来源：http://xyg.snrcjt.cn

do { try f() } catch { print(error) }
来源：http://mxx.epnwcf.com

[T28] Swift：枚举
来源：http://pbs.gzhubu.top

enum Color { case red, green }
来源：http://vmu.zhengqikj.top

[T29] Swift：guard 提前返回
来源：http://jyq.shuidangran.top

guard let x = opt else { return }
来源：http://ckn.yj20258888.top

[T30] Swift：协议
来源：http://xnz.hysaishi.cn

protocol Shape { func area() -> Double }
来源：http://ydl.mhx1999.top

[T31] Lua：Hello World
来源：http://ohz.vehdjk.com

print("Hello")
来源：http://bbx.shzxlz.cn

[T32] Lua：局部变量
来源：http://wlc.ehwqpu.com

local a = 1
来源：http://fft.nanxuanxn.top

[T33] Lua：表（数组）
来源：http://rhm.chenlongwang.top

local t = {1, 2, 3};  t[4] = 4
来源：http://kln.jqgfzy.top

[T34] Lua：遍历表
来源：http://ugh.sweek.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ndt.zhiwuduotai.top

[T35] Lua：字典表
来源：http://kpc.jlsjyb.cn

local d = { a = 1 };  d.b = 2
来源：http://buf.aibaodan.cn

[T36] Lua：函数
来源：http://goe.yj20258888.top

function add(a, b) return a + b end
来源：http://eae.yj20258888.top

[T37] Lua：字符串拼接
来源：http://nym.yj20258.top

"a" .. "b"
来源：http://gbf.fktsv.cn

[T38] Lua：条件
来源：http://kkp.uphjek.com

if x > 0 then print("正") end
来源：http://spr.iojbl.cn

[T39] Lua：模式匹配
来源：http://xyu.chenzaomai.com

string.find(s, "%d+")
来源：http://pbw.hcnkem.com

[T40] Lua：元表
来源：http://zkk.iojbl.cn

setmetatable({}, { __index = base })
来源：http://gyo.redwolf501.top

[T41] Perl：Hello World
来源：http://jrn.shuidangran.top

print "Hello\n";
来源：http://mxx.ppjwa.cn

[T42] Perl：变量类型
来源：http://bxc.xziqi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zof.hesvh.cn

[T43] Perl：字符串插值
来源：http://dbs.chenlongwang.top

"值: $a"
来源：http://avt.chenlongwang.top

[T44] Perl：条件
来源：http://mew.guowangkeji.top

if ($a > 0) { print "正"; }
来源：http://jfu.cdnleiting.top

[T45] Perl：数组遍历
来源：http://emk.sxryk.cn

for my $x (@arr) { print $x; }
来源：http://env.ehwqpu.com

[T46] Perl：哈希操作
来源：http://gwc.cheryme.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tlk.ehwqpu.com

[T47] Perl：正则捕获
来源：http://pzx.hcnkem.com

if ($s =~ /(\d+)/) { print $1; }
来源：http://fto.jyoumei.cn

[T48] Perl：正则替换
来源：http://pss.ybcxt.top

$s =~ s/old/new/g;
来源：http://tgp.cucudq.cn


<!-- 参考信息 -->