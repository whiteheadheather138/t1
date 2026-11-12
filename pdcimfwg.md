代发 wailian999

cmd >/dev/null 2>&1
来源：http://nye.smart0.xyz

[R42] 输入重定向
来源：http://jaz.gogol.net.cn

wc -l < a.txt
来源：http://coh.yj20258.top

[R43] 按名字查找文件
来源：http://dow.pengpengdd.cyou

find . -name "*.log" -type f
来源：http://xyw.jqgufenzy.top

[R44] 按修改时间查找
来源：http://yvk.bbcook.cn

find . -mtime -7 -type f
来源：http://ukj.yangfankeji.com

[R45] 批量删除
来源：http://aoa.meibo888.top

find . -name "*.tmp" -delete
来源：http://mod.hywenlv.cn

[R46] 递归替换文件内容
来源：http://rkr.shuidangran.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://whw.sjlbkw.cn

[R47] sed 单行替换
来源：http://lqv.sufxvd.cn

sed -i 's/foo/bar/g' a.txt
来源：http://rlz.tianlin.xyz

[R48] awk 取指定列
来源：http://pyq.gzhubu.top

awk '{print $1, $3}' a.txt
来源：http://dsc.yvedp.cn

[R49] awk 带条件
来源：http://tfr.tian-w.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ovg.yuxming.cn

[R50] awk 求和
来源：http://rfq.dashuyun.cn

awk '{s += $2} END {print s}' a.txt
来源：http://brk.hammf.cn

[R51] 排序去重取前几
来源：http://hbp.cucudq.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://bnj.hcnkem.com

[R52] 统计行数
来源：http://skx.yangfankeji.com

wc -l a.txt
来源：http://xuf.snrcjt.cn

[R53] 查看文件头与实时尾
来源：http://ddp.chenjidiqi.icu

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bgu.yvedp.cn

[R54] 比较两个文件
来源：http://fcz.yongpay.top

diff a.txt b.txt
来源：http://pct.52xcode.cn

[R55] 压缩与解压
来源：http://tsl.fengsongda.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cdr.0kj1m.cn

[R56] 远程拷贝
来源：http://nwe.ehwqpu.com

scp file user@host:/path/
来源：http://wwr.hammf.cn

[R57] 远程执行命令
来源：http://gxn.zhijiandao.cn

ssh user@host 'uptime'
来源：http://mrh.chenlongwang.top

[R58] 下载文件
来源：http://ptc.ydjk.org.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uwi.svipenyu.cn

[R59] 发 POST JSON
来源：http://gpj.ydjk.org.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://skq.jinqigufen.top

[R60] 只看 HTTP 状态码
来源：http://mgh.zdqjudy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://njx.shangyingyoupin.top

[R61] 磁盘占用
来源：http://huv.chenlongwang.top

df -h;  du -sh *
来源：http://kod.hnqzz.top

[R62] 找最占空间的文件
来源：http://thy.zdbjq.cn

du -ah . | sort -rh | head -10
来源：http://jzi.jinghuilouyu.cn

[R63] 内存与进程
来源：http://azv.hongshengwenyu.top

free -h;  ps aux | grep nginx
来源：http://lsh.hnxiangtu.top

[R64] 结束进程
来源：http://yuu.gzhubu.top

kill -9 $(pgrep -f app.py)
来源：http://rlt.shzxlz.cn

[R65] 查看端口占用
来源：http://voz.meibo888.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://udr.ppjwa.cn

[R66] 定时任务
来源：http://bqf.9152youxi.cn

crontab -e;  crontab -l
来源：http://sci.andypj.xyz

[R67] 生成随机十六进制串
来源：http://wxj.daria6918.cn

openssl rand -hex 16
来源：http://kuo.sufxvd.cn

[R68] 计算文件校验值
来源：http://jdc.hfpthk.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qgn.ydzc1.top

[R69] 生成随机密码
来源：http://ydy.ctjpmb.com

head -c 16 /dev/urandom | base64
来源：http://bly.pengpengdd.cyou

[R70] 时间戳与互转
来源：http://lqo.snrcjt.cn

date +%s;  date -d @1700000000
来源：http://xjp.dianchejie.cn

[R71] 日期格式化
来源：http://mcr.xingfuxueyuan.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://mch.hesvh.cn

[R72] 等待端口就绪
来源：http://zqb.xuetiantiany.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://uxx.ppjwa.cn

[R73] 分割大日志
来源：http://tne.jinqigufen.top

split -l 1000 big.log part_
来源：http://okt.xuanzx.com

[R74] 批量重命名
来源：http://nek.pycfn.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://apb.jianghu66.top

[R75] 导出环境变量
来源：http://hpt.yueranfly.top

export PATH="$HOME/bin:$PATH"
来源：http://rlf.9152youxi.cn

[R76] 使用临时文件
来源：http://uam.meibo888.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wfl.haohaochexian.top

[R77] 读取用户输入
来源：http://hzx.xylfe.cn

read -rp "请输入: " ans
来源：http://gjw.yfazqb.com

[R78] 交互式菜单
来源：http://hjv.jiagoushi.top

select opt in a b c; do echo "$opt"; break; done
来源：http://uvt.sxryk.cn

[R79] 解析命令行选项
来源：http://kfr.vqdsnc.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jia.fengsongda.top

[R80] 查看脚本执行耗时
来源：http://dgl.yongpay.top

time ./run.sh
来源：http://pln.ydzc1.top

================================================================================
来源：http://isp.jinyuanbaomall.cn

S. C / C++ 专题
来源：http://atv.ydjk.org.cn

================================================================================
来源：http://gbu.chenlongwang.top

[S01] C：Hello World
来源：http://dpo.hysaishi.cn

#include <stdio.h>
来源：http://ovp.jinqigufen.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://rnm.tarul.cn

[S02] C：变量与格式化输出
来源：http://lfz.yonumen.top

int a = 10; printf("%d\n", a);
来源：http://pon.gaohongyu789.top

[S03] C：读入整数
来源：http://iea.jiagoushi.top

int x; scanf("%d", &x);
来源：http://iaz.hesvh.cn

[S04] C：字符串复制
来源：http://zmz.jinqigfzy.top

char dst[32]; strcpy(dst, "hi");
来源：http://ker.zhixingplan.top

[S05] C：字符串长度
来源：http://ady.hammf.cn

strlen(s)
来源：http://she.gotoacloud.top

[S06] C：字符串比较
来源：http://rjo.cqqwz.cn

strcmp(a, b) == 0
来源：http://oul.zhijiandao.cn

[S07] C：数组遍历求和
来源：http://gha.daxiang520.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nvf.fzhhl.top

[S08] C：动态内存分配与释放
来源：http://olr.cucudq.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bdp.ywan-chungtsiang.top

[S09] C：结构体定义与初始化
来源：http://jeg.zhongyouzk.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dzk.shanyushiyangtech.top

[S10] C：指针与解引用
来源：http://sad.vqdsnc.cn

int *p = &a;  *p = 5;
来源：http://yus.yonumen.top

[S11] C：逐行读文件
来源：http://jox.feifeiyinyue.top

FILE *f = fopen("a.txt", "r");
来源：http://zzj.gzhubu.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://xyl.cheryme.top

fclose(f);
来源：http://xkj.chenjidiqi.icu

[S12] C：写文件
来源：http://kne.aibaodan.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mxs.xuanzx.com

[S13] C：宏定义
来源：http://frj.shanyushiyangtech.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hdi.snrcjt.cn

[S14] C：枚举
来源：http://rzh.zhixingplan.top

enum Color { RED, GREEN, BLUE };
来源：http://wau.dashuyun.cn

[S15] C：类型转换
来源：http://zqn.jinyuanbaomall.cn

(double) a / b
来源：http://sha.jqgufenzy.top

[S16] C：位操作置位
来源：http://vvn.gaohongyu789.top

x |= (1 << 3);
来源：http://dft.yj20258.top

[S17] C：安全拼接字符串
来源：http://ycz.ybcxt.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hnw.meibo888.top

[S18] C：命令行参数
来源：http://vra.chenzaomai.com

int main(int argc, char **argv)
来源：http://tvz.yangfankeji.com

[S19] C：快速排序
来源：http://bur.shanyushiyangkeji.top

qsort(a, n, sizeof(int), cmp);
来源：http://sgi.nanxuanxn.top

[S20] C：二分查找
来源：http://jev.haohaochexian.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zaa.hcnkem.com

[S21] C：字符类别判断
来源：http://xcd.snrcjt.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://aml.hammf.cn

[S22] C：字符串转数字
来源：http://aei.wangshuangyany.cn

atoi("42");  strtod("3.14", NULL);
来源：http://hww.zhoulong.xyz

[S23] C：随机数
来源：http://lhz.vehdjk.com

srand(time(NULL));  int r = rand() % 100;
来源：http://dyk.havefunace.top

[S24] C：获取本地时间
来源：http://apk.smart0.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://grc.ybcxt.top

[S25] C：内存拷贝
来源：http://sfa.zhaomingkeji.xyz

memcpy(dst, src, n);
来源：http://pbx.havefunace.top

[S26] C：内存清零
来源：http://ing.nwbrower.top

memset(a, 0, sizeof a);
来源：http://kmc.hfpthk.cn

[S27] C：定义常量
来源：http://ydj.dashuyun.cn

const double PI = 3.14159;
来源：http://owe.redwolf501.top

[S28] C：静态变量
来源：http://tnf.sufxvd.cn

static int counter = 0;
来源：http://upb.daria6918.cn

[S29] C：变参函数
来源：http://fqj.vqdsnc.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://djz.birdmap.top

[S30] C：头文件保护
来源：http://uxd.zhaomingkeji.xyz

#ifndef X_H
来源：http://dhv.hfpthk.cn

#define X_H
来源：http://ede.jlsjyb.cn

#endif
来源：http://ylx.zdqjudy.top

[S31] C++：Hello World
来源：http://uvn.yj202588.top

#include <iostream>
来源：http://qfr.jiagoushi.top

int main() { std::cout << "Hello\n"; }
来源：http://whf.yangfankeji.com

[S32] C++：字符串
来源：http://ahu.zdbjq.cn

std::string s = "hi";  s += "!";
来源：http://qfg.tanke756.top

[S33] C++：vector 增删
来源：http://auh.redwolf501.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://msc.guowangkeji.top

[S34] C++：遍历 vector
来源：http://whl.zycfv.cn

for (auto &x : v) { std::cout << x; }
来源：http://qvi.tanke756.top

[S35] C++：map
来源：http://omw.havefunace.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ljd.ivvv.top

[S36] C++：unordered_map
来源：http://uvv.gzhubu.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sgq.hnqzz.top

[S37] C++：set
来源：http://yjg.jqgfzy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ufy.shangyingyoupin.top

[S38] C++：排序
来源：http://yis.jlsjyb.cn

std::sort(v.begin(), v.end());
来源：http://doz.shangyingyoupin.top

[S39] C++：自定义比较器排序
来源：http://eep.feifeiyinyue.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hve.zhongyouzk.top

[S40] C++：查找元素
来源：http://vgt.bjfxy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tbm.xingfuxueyuan.xyz

[S41] C++：类与构造函数
来源：http://fmd.zhengqikj.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yfb.hnxiangtu.top

[S42] C++：继承与虚函数
来源：http://prp.tanke756.top

class B : public Base { public: void f() override {} };
来源：http://jns.cqqwz.cn

[S43] C++：智能指针
来源：http://obn.vqdsnc.cn

auto p = std::make_unique<int>(5);
来源：http://fnq.hfpthk.cn

[S44] C++：引用传参
来源：http://xow.chenjidiqi.icu

void inc(int &x) { ++x; }
来源：http://twb.yj202588.top

[S45] C++：lambda
来源：http://ika.jinghuilouyu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hjr.yuxming.cn

[S46] C++：函数模板
来源：http://yyq.cheryme.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vze.ctjpmb.com

[S47] C++：结构化绑定遍历
来源：http://dtn.chenjidiqi.icu

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xkg.aizwys.cn

[S48] C++：逐行读文件
来源：http://pvg.ydjk.org.cn

std::ifstream in("a.txt");  std::string line;
来源：http://tyv.jinqigfzy.top

while (std::getline(in, line)) { }
来源：http://ftb.epnwcf.com

[S49] C++：写文件
来源：http://usl.zhongyouzk.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mxu.vehdjk.com

[S50] C++：格式化数字
来源：http://oqa.zhengqikj.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lrp.jqgufenzy.top

[S51] C++：显式类型转换
来源：http://hyr.cashguo.top

static_cast<double>(a) / b
来源：http://ojf.daxiang520.top

[S52] C++：const 与 noexcept
来源：http://tll.tarul.cn

int size() const noexcept { return n_; }
来源：http://vjm.sweek.top

[S53] C++：移动语义
来源：http://vos.xinyue.icu

std::vector<int> w = std::move(v);
来源：http://oin.sjlbkw.cn

[S54] C++：异常处理
来源：http://pwv.yuxming.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lli.yvedp.cn

[S55] C++：结构化绑定
来源：http://pzy.fehbvm.com

auto [a, b] = std::make_pair(1, 2);
来源：http://dpi.quarkkingdee.top

[S56] C++：optional
来源：http://dvp.shzxlz.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hmg.sjlbkw.cn

[S57] C++：编译期常量
来源：http://fpc.vqdsnc.cn

constexpr int N = 10;
来源：http://cil.ydzc1.top

[S58] C++：命名空间
来源：http://rcb.gogol.net.cn

namespace ns { int f() { return 1; } }
来源：http://flb.zhijiandao.cn

[S59] C++：静态断言
来源：http://nef.shanyushiyangtech.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mux.jinghuilouyu.cn

[S60] C++：遍历并删除元素
来源：http://zry.yj20258888.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hni.hcnkem.com

================================================================================
来源：http://fqi.hcnkem.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://sxz.epnwcf.com

================================================================================
来源：http://fis.yangfankeji.com

[T01] Kotlin：Hello World
来源：http://oxj.gaohongyu789.top

println("Hello")
来源：http://rsy.yueranfly.top

[T02] Kotlin：变量
来源：http://ldk.guannengcc.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ecy.gaohongyu789.top

[T03] Kotlin：字符串模板
来源：http://qyh.fehbvm.com

"值: $b"
来源：http://xyw.shuidangran.top

[T04] Kotlin：空安全
来源：http://emh.gaohongyu789.top

val n: String? = null;  n?.length
来源：http://zwr.hnxiangtu.top

[T05] Kotlin：when 表达式
来源：http://pph.kuanghao11.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kgn.dianchejie.cn

[T06] Kotlin：集合映射
来源：http://wqn.svipenyu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://gvl.ybcxt.top

[T07] Kotlin：集合过滤
来源：http://zvf.nanxuanxn.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://iqo.xylfe.cn

[T08] Kotlin：数据类
来源：http://fgm.ydjk.org.cn

data class User(val name: String, val age: Int)
来源：http://kqq.vehdjk.com

[T09] Kotlin：扩展函数
来源：http://mgd.chenlongwang.top

fun String.exclaim() = this + "!"
来源：http://riz.feifeiyinyue.top

[T10] Kotlin：默认参数
来源：http://rjy.jqgfzy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://vxd.9152youxi.cn

[T11] Kotlin：协程
来源：http://hsp.guannengcc.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://dpd.jyoumei.cn

[T12] Kotlin：解构声明
来源：http://xcs.daria6918.cn

val (a, b) = Pair(1, 2)
来源：http://wmn.zhiwuduotai.top

[T13] Kotlin：只读 Map
来源：http://prc.tarul.cn

val m = mapOf("a" to 1)
来源：http://lyd.zhengqikj.top

[T14] Kotlin：循环
来源：http://ilf.snrcjt.cn

for (i in 1..10) println(i)
来源：http://xrv.bjfxy.top

[T15] Kotlin：接口
来源：http://bxf.chenlongwang.top

interface Shape { fun area(): Double }
来源：http://fuk.hnxiangtu.top

[T16] Swift：Hello World
来源：http://elc.bbcook.cn

print("Hello")
来源：http://xxn.hongshengwenyu.top

[T17] Swift：变量与常量
来源：http://hyu.cashguo.top

var a = 1;  let b = 2
来源：http://ctr.52xcode.cn

[T18] Swift：字符串插值
来源：http://roz.ehwqpu.com

"值: \(b)"
来源：http://ian.zycfv.cn

[T19] Swift：可选绑定
来源：http://bcl.nanxuanxn.top

if let n = opt { print(n) }
来源：http://ddi.xylfe.cn

[T20] Swift：数组操作
来源：http://hml.9152youxi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://tqd.yanxiufei.cn

[T21] Swift：遍历
来源：http://itk.nanxuanxn.top

for x in a { print(x) }
来源：http://tph.feifeiyinyue.top

[T22] Swift：字典
来源：http://odz.fanxiaobao.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://dvx.pycfn.com

[T23] Swift：函数
来源：http://bwu.mhx1999.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lnb.316326.xyz

[T24] Swift：闭包
来源：http://ysa.ydjk.org.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://jpv.zdqjudy.top

[T25] Swift：结构体
来源：http://ptj.iojbl.cn

struct P { var x: Int }
来源：http://fxt.xinyue.icu

[T26] Swift：类与重写
来源：http://jlc.epnwcf.com

class A: Base { override func f() {} }
来源：http://nmd.fktsv.cn

[T27] Swift：错误处理
来源：http://znv.guannengcc.top

do { try f() } catch { print(error) }
来源：http://xvf.fengsongda.top

[T28] Swift：枚举
来源：http://bfs.xziqi.cn

enum Color { case red, green }
来源：http://jvc.wangdashe.top

[T29] Swift：guard 提前返回
来源：http://arl.zycfv.cn

guard let x = opt else { return }
来源：http://qzs.ydzc1.top

[T30] Swift：协议
来源：http://lsw.316326.xyz

protocol Shape { func area() -> Double }
来源：http://dgh.yuxming.cn

[T31] Lua：Hello World
来源：http://grw.gzhubu.top

print("Hello")
来源：http://etj.aizwys.cn

[T32] Lua：局部变量
来源：http://qxx.xylfe.cn

local a = 1
来源：http://wcb.ppjwa.cn

[T33] Lua：表（数组）
来源：http://qdd.aibaodan.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://yqv.tianlin.xyz

[T34] Lua：遍历表
来源：http://urw.yuanzhike.top

for i, v in ipairs(t) do print(i, v) end
来源：http://fay.zhoulong.xyz

[T35] Lua：字典表
来源：http://zbt.hnqzz.top

local d = { a = 1 };  d.b = 2
来源：http://ymx.shanyushiyangtech.top

[T36] Lua：函数
来源：http://ubr.zhixingplan.top

function add(a, b) return a + b end
来源：http://wcy.yuanzhike.top

[T37] Lua：字符串拼接
来源：http://esw.jiagoushi.top

"a" .. "b"
来源：http://qtk.hnxiangtu.top

[T38] Lua：条件
来源：http://ktf.bjfxy.top

if x > 0 then print("正") end
来源：http://sjf.yfazqb.com

[T39] Lua：模式匹配
来源：http://lcn.pycfn.com

string.find(s, "%d+")
来源：http://pyh.vqdsnc.cn

[T40] Lua：元表
来源：http://hdi.c1oappe.top

setmetatable({}, { __index = base })
来源：http://ruw.uphjek.com

[T41] Perl：Hello World
来源：http://slv.yj20258888.top

print "Hello\n";
来源：http://oxo.quarkkingdee.top

[T42] Perl：变量类型
来源：http://nqw.yj20258.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vcb.redwolf501.top

[T43] Perl：字符串插值
来源：http://dek.zycfv.cn

"值: $a"
来源：http://wbm.pengpengdd.cyou

[T44] Perl：条件
来源：http://ozl.shanyushiyangtech.top

if ($a > 0) { print "正"; }
来源：http://vms.sjlbkw.cn


<!-- 参考信息 -->