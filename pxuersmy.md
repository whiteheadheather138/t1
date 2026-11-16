代发 wailian999

cmd > out.log 2>&1
来源：http://mqg.cheryme.top

[R40] 追加写日志
来源：http://hya.shzxlz.cn

echo "log" >> out.log
来源：http://tkl.fehbvm.com

[R41] 丢弃输出
来源：http://uhz.uphjek.com

cmd >/dev/null 2>&1
来源：http://nfa.fehbvm.com

[R42] 输入重定向
来源：http://kmc.hongshengwenyu.top

wc -l < a.txt
来源：http://drw.52xcode.cn

[R43] 按名字查找文件
来源：http://idz.ywan-chungtsiang.top

find . -name "*.log" -type f
来源：http://slm.52xcode.cn

[R44] 按修改时间查找
来源：http://bnw.sjlbkw.cn

find . -mtime -7 -type f
来源：http://mwi.hcnkem.com

[R45] 批量删除
来源：http://huo.yangfankeji.com

find . -name "*.tmp" -delete
来源：http://zvm.sjlbkw.cn

[R46] 递归替换文件内容
来源：http://bwe.chenzaomai.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mmx.hcnkem.com

[R47] sed 单行替换
来源：http://edn.vqdsnc.cn

sed -i 's/foo/bar/g' a.txt
来源：http://kns.fktsv.cn

[R48] awk 取指定列
来源：http://jgs.yangfankeji.com

awk '{print $1, $3}' a.txt
来源：http://bcs.jlsjyb.cn

[R49] awk 带条件
来源：http://rgu.haohaochexian.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vuz.birdmap.top

[R50] awk 求和
来源：http://dic.yvedp.cn

awk '{s += $2} END {print s}' a.txt
来源：http://gdk.tarul.cn

[R51] 排序去重取前几
来源：http://lqg.fktsv.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://cdp.vqdsnc.cn

[R52] 统计行数
来源：http://etl.haohaochexian.top

wc -l a.txt
来源：http://fme.jinqigfzy.top

[R53] 查看文件头与实时尾
来源：http://ekb.sjlbkw.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kpn.sjlbkw.cn

[R54] 比较两个文件
来源：http://mpw.shanyushiyangkeji.top

diff a.txt b.txt
来源：http://wbn.zhengqikj.top

[R55] 压缩与解压
来源：http://kbt.tanke756.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kgb.yfazqb.com

[R56] 远程拷贝
来源：http://gkc.zycfv.cn

scp file user@host:/path/
来源：http://rqa.ppjwa.cn

[R57] 远程执行命令
来源：http://gsh.shanyushiyangkeji.top

ssh user@host 'uptime'
来源：http://ibq.sxryk.cn

[R58] 下载文件
来源：http://vrm.0kj1m.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pge.guowangkeji.top

[R59] 发 POST JSON
来源：http://ekt.tian-w.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ikj.zhijiandao.cn

[R60] 只看 HTTP 状态码
来源：http://gfo.havefunace.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sar.ivvv.top

[R61] 磁盘占用
来源：http://bjo.sjlbkw.cn

df -h;  du -sh *
来源：http://qyj.cheryme.top

[R62] 找最占空间的文件
来源：http://djb.ehwqpu.com

du -ah . | sort -rh | head -10
来源：http://jkt.sxryk.cn

[R63] 内存与进程
来源：http://mkd.svipenyu.cn

free -h;  ps aux | grep nginx
来源：http://gms.52xcode.cn

[R64] 结束进程
来源：http://syc.zdqjudy.top

kill -9 $(pgrep -f app.py)
来源：http://miu.yj202588.top

[R65] 查看端口占用
来源：http://wxx.gaohongyu789.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zvt.shzxlz.cn

[R66] 定时任务
来源：http://apv.tian-w.cn

crontab -e;  crontab -l
来源：http://txg.jlsjyb.cn

[R67] 生成随机十六进制串
来源：http://zkg.jiagoushi.top

openssl rand -hex 16
来源：http://cug.hnxiangtu.top

[R68] 计算文件校验值
来源：http://yfn.hfpthk.cn

sha256sum a.txt;  md5sum a.txt
来源：http://rjl.zhijiandao.cn

[R69] 生成随机密码
来源：http://bvs.jyoumei.cn

head -c 16 /dev/urandom | base64
来源：http://pet.fengsongda.top

[R70] 时间戳与互转
来源：http://cgo.smart0.xyz

date +%s;  date -d @1700000000
来源：http://bor.sjlbkw.cn

[R71] 日期格式化
来源：http://obd.meibo888.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://qig.jinghuilouyu.cn

[R72] 等待端口就绪
来源：http://bmh.xuanzx.com

until nc -z localhost 3306; do sleep 1; done
来源：http://unw.hnqzz.top

[R73] 分割大日志
来源：http://qro.redwolf501.top

split -l 1000 big.log part_
来源：http://ueb.shanyushiyangkeji.top

[R74] 批量重命名
来源：http://iru.yuanzhike.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://txe.hongshengwenyu.top

[R75] 导出环境变量
来源：http://eva.chenlongwang.top

export PATH="$HOME/bin:$PATH"
来源：http://fyj.xziqi.cn

[R76] 使用临时文件
来源：http://qga.mhx1999.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ipp.vehdjk.com

[R77] 读取用户输入
来源：http://vhx.hysaishi.cn

read -rp "请输入: " ans
来源：http://kmq.shuidangran.top

[R78] 交互式菜单
来源：http://hid.nwbrower.top

select opt in a b c; do echo "$opt"; break; done
来源：http://gon.cheryme.top

[R79] 解析命令行选项
来源：http://fzm.birdmap.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mkr.wangshuangyany.cn

[R80] 查看脚本执行耗时
来源：http://ffv.tianlin.xyz

time ./run.sh
来源：http://kbx.fehbvm.com

================================================================================
来源：http://zfr.ydzc1.top

S. C / C++ 专题
来源：http://dye.gzhubu.top

================================================================================
来源：http://wgc.gotoacloud.top

[S01] C：Hello World
来源：http://cke.tian-w.cn

#include <stdio.h>
来源：http://sfh.yangfankeji.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://wgo.haohaochexian.top

[S02] C：变量与格式化输出
来源：http://itg.hongshengwenyu.top

int a = 10; printf("%d\n", a);
来源：http://kzx.ehwqpu.com

[S03] C：读入整数
来源：http://jlj.nanxuanxn.top

int x; scanf("%d", &x);
来源：http://rwp.hywenlv.cn

[S04] C：字符串复制
来源：http://zch.zhixingplan.top

char dst[32]; strcpy(dst, "hi");
来源：http://rjn.c1oappe.top

[S05] C：字符串长度
来源：http://jvu.0kj1m.cn

strlen(s)
来源：http://idj.yfazqb.com

[S06] C：字符串比较
来源：http://tug.ydjk.org.cn

strcmp(a, b) == 0
来源：http://opd.9152youxi.cn

[S07] C：数组遍历求和
来源：http://vex.ivvv.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qar.svipenyu.cn

[S08] C：动态内存分配与释放
来源：http://noa.tanke756.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://isv.yj20258.top

[S09] C：结构体定义与初始化
来源：http://ewl.aibaodan.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://osg.zdqjudy.top

[S10] C：指针与解引用
来源：http://nbw.zdqjudy.top

int *p = &a;  *p = 5;
来源：http://vig.quarkkingdee.top

[S11] C：逐行读文件
来源：http://tku.cucudq.cn

FILE *f = fopen("a.txt", "r");
来源：http://hyq.yongpay.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://kfs.shzxlz.cn

fclose(f);
来源：http://mgg.hcnkem.com

[S12] C：写文件
来源：http://sfi.zhongyouzk.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mcq.shuidangran.top

[S13] C：宏定义
来源：http://zof.gzhubu.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jxc.mhx1999.top

[S14] C：枚举
来源：http://zdg.zhengqikj.top

enum Color { RED, GREEN, BLUE };
来源：http://tgt.ppjwa.cn

[S15] C：类型转换
来源：http://kqi.0kj1m.cn

(double) a / b
来源：http://wod.yfazqb.com

[S16] C：位操作置位
来源：http://frq.feifeiyinyue.top

x |= (1 << 3);
来源：http://uve.zdqjudy.top

[S17] C：安全拼接字符串
来源：http://zju.wangdashe.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://htg.daria6918.cn

[S18] C：命令行参数
来源：http://yrn.sxryk.cn

int main(int argc, char **argv)
来源：http://jlm.ppjwa.cn

[S19] C：快速排序
来源：http://uir.xinyue.icu

qsort(a, n, sizeof(int), cmp);
来源：http://xjx.hcnkem.com

[S20] C：二分查找
来源：http://hzy.9152youxi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xmy.sjlbkw.cn

[S21] C：字符类别判断
来源：http://lek.yj202588.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xfr.hongshengwenyu.top

[S22] C：字符串转数字
来源：http://mwc.zhixingplan.top

atoi("42");  strtod("3.14", NULL);
来源：http://jyp.shuidangran.top

[S23] C：随机数
来源：http://mqw.jinqigufen.top

srand(time(NULL));  int r = rand() % 100;
来源：http://akd.gzhubu.top

[S24] C：获取本地时间
来源：http://eoc.yj202588.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uxu.gotoacloud.top

[S25] C：内存拷贝
来源：http://eej.smart0.xyz

memcpy(dst, src, n);
来源：http://nwz.ivvv.top

[S26] C：内存清零
来源：http://vww.yuanzhike.top

memset(a, 0, sizeof a);
来源：http://hqw.jinyuanbaomall.cn

[S27] C：定义常量
来源：http://ufq.hnqzz.top

const double PI = 3.14159;
来源：http://buk.zhengqikj.top

[S28] C：静态变量
来源：http://vxu.tianlin.xyz

static int counter = 0;
来源：http://fyj.pengpengdd.cyou

[S29] C：变参函数
来源：http://jcp.zdbjq.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qyu.nanxinkj.top

[S30] C：头文件保护
来源：http://iik.jinqigufen.top

#ifndef X_H
来源：http://xsj.uphjek.com

#define X_H
来源：http://bwj.fzhhl.top

#endif
来源：http://emc.cqqwz.cn

[S31] C++：Hello World
来源：http://nnu.316326.xyz

#include <iostream>
来源：http://wxy.pycfn.com

int main() { std::cout << "Hello\n"; }
来源：http://wsn.ctjpmb.com

[S32] C++：字符串
来源：http://ddt.ehwqpu.com

std::string s = "hi";  s += "!";
来源：http://qvb.yvedp.cn

[S33] C++：vector 增删
来源：http://dnu.yfazqb.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://onx.sjlbkw.cn

[S34] C++：遍历 vector
来源：http://gou.havefunace.top

for (auto &x : v) { std::cout << x; }
来源：http://mdt.gotoacloud.top

[S35] C++：map
来源：http://lpf.pycfn.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zba.0kj1m.cn

[S36] C++：unordered_map
来源：http://qpq.jianghu66.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wgj.ydzc1.top

[S37] C++：set
来源：http://ler.hammf.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lmz.xuetiantiany.cn

[S38] C++：排序
来源：http://gbj.bjfxy.top

std::sort(v.begin(), v.end());
来源：http://ddi.sweek.top

[S39] C++：自定义比较器排序
来源：http://jzx.feifeiyinyue.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jbt.yvedp.cn

[S40] C++：查找元素
来源：http://eqk.gogol.net.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qha.fktsv.cn

[S41] C++：类与构造函数
来源：http://otu.nanxuanxn.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nze.feifeiyinyue.top

[S42] C++：继承与虚函数
来源：http://gqz.sysykeji.top

class B : public Base { public: void f() override {} };
来源：http://kef.zycfv.cn

[S43] C++：智能指针
来源：http://nek.fengsongda.top

auto p = std::make_unique<int>(5);
来源：http://yeu.ywan-chungtsiang.top

[S44] C++：引用传参
来源：http://eeb.ppjwa.cn

void inc(int &x) { ++x; }
来源：http://oat.sufxvd.cn

[S45] C++：lambda
来源：http://vti.jianghu66.top

auto add = [](int a, int b) { return a + b; };
来源：http://fym.jinghuilouyu.cn

[S46] C++：函数模板
来源：http://lrv.tianlin.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ztm.daria6918.cn

[S47] C++：结构化绑定遍历
来源：http://jgb.redwolf501.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qcc.ehwqpu.com

[S48] C++：逐行读文件
来源：http://vgc.hywenlv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ecf.jqgfzy.top

while (std::getline(in, line)) { }
来源：http://zng.yuxming.cn

[S49] C++：写文件
来源：http://bmc.wangshuangyany.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yvi.cucudq.cn

[S50] C++：格式化数字
来源：http://zhn.0kj1m.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pdb.shuidangran.top

[S51] C++：显式类型转换
来源：http://pol.chenlongwang.top

static_cast<double>(a) / b
来源：http://qhc.shanyushiyangkeji.top

[S52] C++：const 与 noexcept
来源：http://ani.cashguo.top

int size() const noexcept { return n_; }
来源：http://nhe.zhiwuduotai.top

[S53] C++：移动语义
来源：http://gca.zhoulong.xyz

std::vector<int> w = std::move(v);
来源：http://mdv.gotoacloud.top

[S54] C++：异常处理
来源：http://axt.xingfuxueyuan.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mbf.aizwys.cn

[S55] C++：结构化绑定
来源：http://jjy.shzxlz.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://pzi.yfazqb.com

[S56] C++：optional
来源：http://pjr.smart0.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kfh.9152youxi.cn

[S57] C++：编译期常量
来源：http://sgm.gogol.net.cn

constexpr int N = 10;
来源：http://wdu.cdnleiting.top

[S58] C++：命名空间
来源：http://jqv.yanxiufei.cn

namespace ns { int f() { return 1; } }
来源：http://njo.hongshengwenyu.top

[S59] C++：静态断言
来源：http://suw.0kj1m.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gyc.zhoulong.xyz

[S60] C++：遍历并删除元素
来源：http://mmv.yuanzhike.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ldd.yanxiufei.cn

================================================================================
来源：http://uhp.bbcook.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uhn.tian-w.cn

================================================================================
来源：http://qea.ppjwa.cn

[T01] Kotlin：Hello World
来源：http://zav.jinghuilouyu.cn

println("Hello")
来源：http://bqv.quarkkingdee.top

[T02] Kotlin：变量
来源：http://eqj.xinyue.icu

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cwh.sweek.top

[T03] Kotlin：字符串模板
来源：http://uka.kuanghao11.cn

"值: $b"
来源：http://mmn.zhongyouzk.top

[T04] Kotlin：空安全
来源：http://bkk.xuetiantiany.cn

val n: String? = null;  n?.length
来源：http://xrs.jinyuanbaomall.cn

[T05] Kotlin：when 表达式
来源：http://heg.yj20258888.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xgq.shanyushiyangtech.top

[T06] Kotlin：集合映射
来源：http://brv.wangshuangyany.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://dqn.aizwys.cn

[T07] Kotlin：集合过滤
来源：http://mza.zdqjudy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://hsr.yangfankeji.com

[T08] Kotlin：数据类
来源：http://ric.ywan-chungtsiang.top

data class User(val name: String, val age: Int)
来源：http://jqr.cheryme.top

[T09] Kotlin：扩展函数
来源：http://kxn.yuxming.cn

fun String.exclaim() = this + "!"
来源：http://xde.9152youxi.cn

[T10] Kotlin：默认参数
来源：http://ycs.nanxinkj.top

fun greet(name: String = "World") = "Hi $name"
来源：http://lwf.wangshuangyany.cn

[T11] Kotlin：协程
来源：http://zax.zhoulong.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://fny.haohaochexian.top

[T12] Kotlin：解构声明
来源：http://msw.chenjidiqi.icu

val (a, b) = Pair(1, 2)
来源：http://eus.cheryme.top

[T13] Kotlin：只读 Map
来源：http://hpf.smart0.xyz

val m = mapOf("a" to 1)
来源：http://gcb.yj20258.top

[T14] Kotlin：循环
来源：http://aqn.guowangkeji.top

for (i in 1..10) println(i)
来源：http://iml.hnqzz.top

[T15] Kotlin：接口
来源：http://thw.fehbvm.com

interface Shape { fun area(): Double }
来源：http://zvk.tarul.cn

[T16] Swift：Hello World
来源：http://jqw.hywenlv.cn

print("Hello")
来源：http://qef.daxiang520.top

[T17] Swift：变量与常量
来源：http://xfl.gogol.net.cn

var a = 1;  let b = 2
来源：http://wab.zhoulong.xyz

[T18] Swift：字符串插值
来源：http://utj.sxryk.cn

"值: \(b)"
来源：http://ixj.yueranfly.top

[T19] Swift：可选绑定
来源：http://epw.ivvv.top

if let n = opt { print(n) }
来源：http://evs.tanke756.top

[T20] Swift：数组操作
来源：http://evx.hongshengwenyu.top

var a = [1, 2, 3];  a.append(4)
来源：http://psg.chenzaomai.com

[T21] Swift：遍历
来源：http://dta.xinyue.icu

for x in a { print(x) }
来源：http://mgl.sysykeji.top

[T22] Swift：字典
来源：http://lyq.gotoacloud.top

var d = ["a": 1];  d["b"] = 2
来源：http://qut.ctjpmb.com

[T23] Swift：函数
来源：http://iyt.hongshengwenyu.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zci.cdnleiting.top

[T24] Swift：闭包
来源：http://wzf.tian-w.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xwx.iojbl.cn

[T25] Swift：结构体
来源：http://hwq.tanke756.top

struct P { var x: Int }
来源：http://mfw.xuanzx.com

[T26] Swift：类与重写
来源：http://xic.fanxiaobao.xyz

class A: Base { override func f() {} }
来源：http://kwv.ydjk.org.cn

[T27] Swift：错误处理
来源：http://gvq.yanxiufei.cn

do { try f() } catch { print(error) }
来源：http://vet.xziqi.cn

[T28] Swift：枚举
来源：http://hbe.xylfe.cn

enum Color { case red, green }
来源：http://nxi.xingfuxueyuan.xyz

[T29] Swift：guard 提前返回
来源：http://yee.daria6918.cn

guard let x = opt else { return }
来源：http://njq.kuanghao11.cn

[T30] Swift：协议
来源：http://kwv.tanke756.top

protocol Shape { func area() -> Double }
来源：http://eqv.yuanzhike.top

[T31] Lua：Hello World
来源：http://ntr.guannengcc.top

print("Hello")
来源：http://msa.yfazqb.com

[T32] Lua：局部变量
来源：http://wmv.yuanzhike.top

local a = 1
来源：http://pri.bbcook.cn

[T33] Lua：表（数组）
来源：http://ocx.iojbl.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://guz.ehwqpu.com

[T34] Lua：遍历表
来源：http://gfu.mhx1999.top

for i, v in ipairs(t) do print(i, v) end
来源：http://qdv.gaohongyu789.top

[T35] Lua：字典表
来源：http://gta.meibo888.top

local d = { a = 1 };  d.b = 2
来源：http://sdv.gaohongyu789.top

[T36] Lua：函数
来源：http://tnc.shuidangran.top

function add(a, b) return a + b end
来源：http://idx.gogol.net.cn

[T37] Lua：字符串拼接
来源：http://mph.jyoumei.cn

"a" .. "b"
来源：http://owk.jyoumei.cn

[T38] Lua：条件
来源：http://wyd.ivvv.top

if x > 0 then print("正") end
来源：http://gix.fehbvm.com

[T39] Lua：模式匹配
来源：http://uhr.nanxinkj.top

string.find(s, "%d+")
来源：http://lpy.hesvh.cn

[T40] Lua：元表
来源：http://uep.fengsongda.top

setmetatable({}, { __index = base })
来源：http://ago.jianghu66.top

[T41] Perl：Hello World
来源：http://akw.havefunace.top

print "Hello\n";
来源：http://zuf.xylfe.cn

[T42] Perl：变量类型
来源：http://tml.mhx1999.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tun.zhongyouzk.top


<!-- 参考信息 -->