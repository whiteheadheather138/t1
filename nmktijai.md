代发 wailian999

cmd >/dev/null 2>&1
来源：http://mcb.sxryk.cn

[R42] 输入重定向
来源：http://kkl.cheryme.top

wc -l < a.txt
来源：http://vdc.wangdashe.top

[R43] 按名字查找文件
来源：http://znc.gaohongyu789.top

find . -name "*.log" -type f
来源：http://naf.jinqigfzy.top

[R44] 按修改时间查找
来源：http://ace.gotoacloud.top

find . -mtime -7 -type f
来源：http://hae.xinyue.icu

[R45] 批量删除
来源：http://fwv.jianghu66.top

find . -name "*.tmp" -delete
来源：http://kgb.zdqjudy.top

[R46] 递归替换文件内容
来源：http://eqt.hnqzz.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tfm.52xcode.cn

[R47] sed 单行替换
来源：http://tzu.hysaishi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://pjo.feifeiyinyue.top

[R48] awk 取指定列
来源：http://myo.kuanghao11.cn

awk '{print $1, $3}' a.txt
来源：http://prq.316326.xyz

[R49] awk 带条件
来源：http://luf.shanyushiyangtech.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dvy.fengsongda.top

[R50] awk 求和
来源：http://ato.cdnleiting.top

awk '{s += $2} END {print s}' a.txt
来源：http://sym.tarul.cn

[R51] 排序去重取前几
来源：http://fzz.mhx1999.top

sort a.txt | uniq -c | sort -rn | head
来源：http://nip.yvedp.cn

[R52] 统计行数
来源：http://lhg.c1oappe.top

wc -l a.txt
来源：http://ybc.yuxming.cn

[R53] 查看文件头与实时尾
来源：http://skd.aizwys.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lax.vehdjk.com

[R54] 比较两个文件
来源：http://txt.52xcode.cn

diff a.txt b.txt
来源：http://xqr.aizwys.cn

[R55] 压缩与解压
来源：http://mjy.svipenyu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zts.snrcjt.cn

[R56] 远程拷贝
来源：http://dpj.svipenyu.cn

scp file user@host:/path/
来源：http://zyn.jianghu66.top

[R57] 远程执行命令
来源：http://vox.havefunace.top

ssh user@host 'uptime'
来源：http://lxe.wangdashe.top

[R58] 下载文件
来源：http://mjw.zhijiandao.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ytw.ivvv.top

[R59] 发 POST JSON
来源：http://jos.mhx1999.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yja.yongpay.top

[R60] 只看 HTTP 状态码
来源：http://svg.guannengcc.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rfu.cucudq.cn

[R61] 磁盘占用
来源：http://dlb.hnxiangtu.top

df -h;  du -sh *
来源：http://bml.zhongyouzk.top

[R62] 找最占空间的文件
来源：http://kdf.yuxming.cn

du -ah . | sort -rh | head -10
来源：http://fpy.wangdashe.top

[R63] 内存与进程
来源：http://zpt.xylfe.cn

free -h;  ps aux | grep nginx
来源：http://wdq.dianchejie.cn

[R64] 结束进程
来源：http://xkk.fehbvm.com

kill -9 $(pgrep -f app.py)
来源：http://jrc.jqgufenzy.top

[R65] 查看端口占用
来源：http://qei.hfpthk.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://twk.cashguo.top

[R66] 定时任务
来源：http://lkn.jinyuanbaomall.cn

crontab -e;  crontab -l
来源：http://uer.vehdjk.com

[R67] 生成随机十六进制串
来源：http://bzz.iojbl.cn

openssl rand -hex 16
来源：http://ynv.cdnleiting.top

[R68] 计算文件校验值
来源：http://skp.zhongyouzk.top

sha256sum a.txt;  md5sum a.txt
来源：http://woa.pycfn.com

[R69] 生成随机密码
来源：http://oig.daria6918.cn

head -c 16 /dev/urandom | base64
来源：http://ytn.ehwqpu.com

[R70] 时间戳与互转
来源：http://hwk.nanxuanxn.top

date +%s;  date -d @1700000000
来源：http://hbt.fktsv.cn

[R71] 日期格式化
来源：http://wvf.zdbjq.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://yod.xuetiantiany.cn

[R72] 等待端口就绪
来源：http://fti.gaohongyu789.top

until nc -z localhost 3306; do sleep 1; done
来源：http://lcv.chenlongwang.top

[R73] 分割大日志
来源：http://hde.fzhhl.top

split -l 1000 big.log part_
来源：http://ahg.xingfuxueyuan.xyz

[R74] 批量重命名
来源：http://wgj.gotoacloud.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nlt.hywenlv.cn

[R75] 导出环境变量
来源：http://lig.yj20258888.top

export PATH="$HOME/bin:$PATH"
来源：http://lsh.iojbl.cn

[R76] 使用临时文件
来源：http://xnc.shanyushiyangtech.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sjl.yj20258.top

[R77] 读取用户输入
来源：http://urf.hfpthk.cn

read -rp "请输入: " ans
来源：http://jld.yuxming.cn

[R78] 交互式菜单
来源：http://zwh.jinqigufen.top

select opt in a b c; do echo "$opt"; break; done
来源：http://qvv.ydzc1.top

[R79] 解析命令行选项
来源：http://ihn.jinyuanbaomall.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kkz.316326.xyz

[R80] 查看脚本执行耗时
来源：http://fkc.9152youxi.cn

time ./run.sh
来源：http://hmv.daxiang520.top

================================================================================
来源：http://tqg.nanxinkj.top

S. C / C++ 专题
来源：http://pfl.ppjwa.cn

================================================================================
来源：http://tkf.zycfv.cn

[S01] C：Hello World
来源：http://han.hnxiangtu.top

#include <stdio.h>
来源：http://jnh.guowangkeji.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ags.cucudq.cn

[S02] C：变量与格式化输出
来源：http://las.hysaishi.cn

int a = 10; printf("%d\n", a);
来源：http://bvp.andypj.xyz

[S03] C：读入整数
来源：http://oya.gaohongyu789.top

int x; scanf("%d", &x);
来源：http://opk.ydjk.org.cn

[S04] C：字符串复制
来源：http://zcv.zhongyouzk.top

char dst[32]; strcpy(dst, "hi");
来源：http://tqu.cucudq.cn

[S05] C：字符串长度
来源：http://eng.guowangkeji.top

strlen(s)
来源：http://hpg.yangfankeji.com

[S06] C：字符串比较
来源：http://wzc.zdqjudy.top

strcmp(a, b) == 0
来源：http://qvn.yvedp.cn

[S07] C：数组遍历求和
来源：http://lxs.ybcxt.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xtw.hesvh.cn

[S08] C：动态内存分配与释放
来源：http://paw.iojbl.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gsf.pengpengdd.cyou

[S09] C：结构体定义与初始化
来源：http://mbe.hfpthk.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gdv.yj20258888.top

[S10] C：指针与解引用
来源：http://avt.xuetiantiany.cn

int *p = &a;  *p = 5;
来源：http://kyp.hesvh.cn

[S11] C：逐行读文件
来源：http://wbt.feifeiyinyue.top

FILE *f = fopen("a.txt", "r");
来源：http://qzn.quarkkingdee.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://dvo.jianghu66.top

fclose(f);
来源：http://jys.yuxming.cn

[S12] C：写文件
来源：http://iwo.jianghu66.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ebm.pycfn.com

[S13] C：宏定义
来源：http://pkb.wangshuangyany.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ila.cashguo.top

[S14] C：枚举
来源：http://hno.nwbrower.top

enum Color { RED, GREEN, BLUE };
来源：http://zyv.daria6918.cn

[S15] C：类型转换
来源：http://ybe.meibo888.top

(double) a / b
来源：http://srw.c1oappe.top

[S16] C：位操作置位
来源：http://mbo.gaohongyu789.top

x |= (1 << 3);
来源：http://rfx.zhongyouzk.top

[S17] C：安全拼接字符串
来源：http://krq.aizwys.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uix.aibaodan.cn

[S18] C：命令行参数
来源：http://sbk.c1oappe.top

int main(int argc, char **argv)
来源：http://wsf.jqgfzy.top

[S19] C：快速排序
来源：http://pts.9152youxi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://iaz.yangfankeji.com

[S20] C：二分查找
来源：http://hdh.zhoulong.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://udy.nwbrower.top

[S21] C：字符类别判断
来源：http://xwu.yangfankeji.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hts.aibaodan.cn

[S22] C：字符串转数字
来源：http://ryy.jyoumei.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qhw.haohaochexian.top

[S23] C：随机数
来源：http://bma.chenjidiqi.icu

srand(time(NULL));  int r = rand() % 100;
来源：http://adj.chenzaomai.com

[S24] C：获取本地时间
来源：http://mjs.hnxiangtu.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uyq.hywenlv.cn

[S25] C：内存拷贝
来源：http://cyy.dashuyun.cn

memcpy(dst, src, n);
来源：http://kxc.zhengqikj.top

[S26] C：内存清零
来源：http://uyc.cdnleiting.top

memset(a, 0, sizeof a);
来源：http://uwt.hcnkem.com

[S27] C：定义常量
来源：http://yzo.yuanzhike.top

const double PI = 3.14159;
来源：http://qqv.zycfv.cn

[S28] C：静态变量
来源：http://gxd.fzhhl.top

static int counter = 0;
来源：http://owc.yuxming.cn

[S29] C：变参函数
来源：http://ohu.mhx1999.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://det.birdmap.top

[S30] C：头文件保护
来源：http://vmd.zhijiandao.cn

#ifndef X_H
来源：http://pme.ppjwa.cn

#define X_H
来源：http://sur.yongpay.top

#endif
来源：http://ktx.tarul.cn

[S31] C++：Hello World
来源：http://qyq.hcnkem.com

#include <iostream>
来源：http://fcj.cdnleiting.top

int main() { std::cout << "Hello\n"; }
来源：http://qql.hnxiangtu.top

[S32] C++：字符串
来源：http://nei.shanyushiyangkeji.top

std::string s = "hi";  s += "!";
来源：http://djd.yanxiufei.cn

[S33] C++：vector 增删
来源：http://min.sxryk.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://icj.cheryme.top

[S34] C++：遍历 vector
来源：http://vmt.fehbvm.com

for (auto &x : v) { std::cout << x; }
来源：http://agd.zhoulong.xyz

[S35] C++：map
来源：http://uia.zhongyouzk.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hjb.jianghu66.top

[S36] C++：unordered_map
来源：http://wok.tianlin.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://skr.meibo888.top

[S37] C++：set
来源：http://akg.jinghuilouyu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://uay.fengsongda.top

[S38] C++：排序
来源：http://kfk.svipenyu.cn

std::sort(v.begin(), v.end());
来源：http://weh.pycfn.com

[S39] C++：自定义比较器排序
来源：http://kcc.ppjwa.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xrh.yongpay.top

[S40] C++：查找元素
来源：http://eju.dianchejie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jcx.jinghuilouyu.cn

[S41] C++：类与构造函数
来源：http://cgm.zdbjq.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wph.xuanzx.com

[S42] C++：继承与虚函数
来源：http://fpw.zhijiandao.cn

class B : public Base { public: void f() override {} };
来源：http://yue.birdmap.top

[S43] C++：智能指针
来源：http://mul.hcnkem.com

auto p = std::make_unique<int>(5);
来源：http://loc.aizwys.cn

[S44] C++：引用传参
来源：http://ebj.zhijiandao.cn

void inc(int &x) { ++x; }
来源：http://hgo.yonumen.top

[S45] C++：lambda
来源：http://afz.tarul.cn

auto add = [](int a, int b) { return a + b; };
来源：http://pus.yanxiufei.cn

[S46] C++：函数模板
来源：http://kvd.birdmap.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bpr.gogol.net.cn

[S47] C++：结构化绑定遍历
来源：http://plj.jinqigufen.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://itu.ydzc1.top

[S48] C++：逐行读文件
来源：http://cgg.sxryk.cn

std::ifstream in("a.txt");  std::string line;
来源：http://tsc.yvedp.cn

while (std::getline(in, line)) { }
来源：http://mxh.zycfv.cn

[S49] C++：写文件
来源：http://bkg.cashguo.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sdz.xingfuxueyuan.xyz

[S50] C++：格式化数字
来源：http://dmp.hammf.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pof.birdmap.top

[S51] C++：显式类型转换
来源：http://xbw.gaohongyu789.top

static_cast<double>(a) / b
来源：http://nui.hammf.cn

[S52] C++：const 与 noexcept
来源：http://uad.tarul.cn

int size() const noexcept { return n_; }
来源：http://dig.zhijiandao.cn

[S53] C++：移动语义
来源：http://kon.epnwcf.com

std::vector<int> w = std::move(v);
来源：http://vxi.yj20258888.top

[S54] C++：异常处理
来源：http://jdo.cheryme.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vxa.jianghu66.top

[S55] C++：结构化绑定
来源：http://dcf.0kj1m.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ayd.nanxinkj.top

[S56] C++：optional
来源：http://xqz.bjfxy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mfy.fehbvm.com

[S57] C++：编译期常量
来源：http://ejy.shuidangran.top

constexpr int N = 10;
来源：http://vkk.vqdsnc.cn

[S58] C++：命名空间
来源：http://sdh.hnxiangtu.top

namespace ns { int f() { return 1; } }
来源：http://jbv.jinqigfzy.top

[S59] C++：静态断言
来源：http://dki.hongshengwenyu.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jax.nanxuanxn.top

[S60] C++：遍历并删除元素
来源：http://zeq.hnxiangtu.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ihh.iojbl.cn

================================================================================
来源：http://dpd.sweek.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rem.nwbrower.top

================================================================================
来源：http://azn.hnxiangtu.top

[T01] Kotlin：Hello World
来源：http://zch.gzhubu.top

println("Hello")
来源：http://can.yangfankeji.com

[T02] Kotlin：变量
来源：http://urt.xuanzx.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://icv.meibo888.top

[T03] Kotlin：字符串模板
来源：http://vxs.yj20258.top

"值: $b"
来源：http://pfm.zhengqikj.top

[T04] Kotlin：空安全
来源：http://rph.yvedp.cn

val n: String? = null;  n?.length
来源：http://bfa.shuidangran.top

[T05] Kotlin：when 表达式
来源：http://vxp.zhiwuduotai.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gxj.meibo888.top

[T06] Kotlin：集合映射
来源：http://jzc.birdmap.top

listOf(1, 2, 3).map { it * 2 }
来源：http://lwc.zhaomingkeji.xyz

[T07] Kotlin：集合过滤
来源：http://nan.zhiwuduotai.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://uhm.vqdsnc.cn

[T08] Kotlin：数据类
来源：http://npq.xuanzx.com

data class User(val name: String, val age: Int)
来源：http://toc.316326.xyz

[T09] Kotlin：扩展函数
来源：http://dwo.tianlin.xyz

fun String.exclaim() = this + "!"
来源：http://bip.meibo888.top

[T10] Kotlin：默认参数
来源：http://ywx.gaohongyu789.top

fun greet(name: String = "World") = "Hi $name"
来源：http://amw.zdbjq.cn

[T11] Kotlin：协程
来源：http://duz.jinyuanbaomall.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ulp.316326.xyz

[T12] Kotlin：解构声明
来源：http://zxk.fanxiaobao.xyz

val (a, b) = Pair(1, 2)
来源：http://iwr.birdmap.top

[T13] Kotlin：只读 Map
来源：http://xfq.cheryme.top

val m = mapOf("a" to 1)
来源：http://dee.iojbl.cn

[T14] Kotlin：循环
来源：http://ava.hnqzz.top

for (i in 1..10) println(i)
来源：http://vem.xuetiantiany.cn

[T15] Kotlin：接口
来源：http://yhw.xuetiantiany.cn

interface Shape { fun area(): Double }
来源：http://xzw.svipenyu.cn

[T16] Swift：Hello World
来源：http://nbn.sxryk.cn

print("Hello")
来源：http://gsf.nanxinkj.top

[T17] Swift：变量与常量
来源：http://cae.birdmap.top

var a = 1;  let b = 2
来源：http://gcz.birdmap.top

[T18] Swift：字符串插值
来源：http://oki.hongshengwenyu.top

"值: \(b)"
来源：http://odm.hcnkem.com

[T19] Swift：可选绑定
来源：http://adq.ehwqpu.com

if let n = opt { print(n) }
来源：http://suf.feifeiyinyue.top

[T20] Swift：数组操作
来源：http://vdq.aibaodan.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mvv.guowangkeji.top

[T21] Swift：遍历
来源：http://xoz.nanxuanxn.top

for x in a { print(x) }
来源：http://vpz.yvedp.cn

[T22] Swift：字典
来源：http://nfo.aizwys.cn

var d = ["a": 1];  d["b"] = 2
来源：http://rpi.jqgufenzy.top

[T23] Swift：函数
来源：http://dkd.hnqzz.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vnk.gogol.net.cn

[T24] Swift：闭包
来源：http://rls.fanxiaobao.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://jen.jiagoushi.top

[T25] Swift：结构体
来源：http://yas.sjlbkw.cn

struct P { var x: Int }
来源：http://boz.fktsv.cn

[T26] Swift：类与重写
来源：http://rqg.fktsv.cn

class A: Base { override func f() {} }
来源：http://ufb.fengsongda.top

[T27] Swift：错误处理
来源：http://hdg.nwbrower.top

do { try f() } catch { print(error) }
来源：http://wrs.kuanghao11.cn

[T28] Swift：枚举
来源：http://cwe.jqgfzy.top

enum Color { case red, green }
来源：http://pou.yfazqb.com

[T29] Swift：guard 提前返回
来源：http://wjr.jyoumei.cn

guard let x = opt else { return }
来源：http://aqy.hcnkem.com

[T30] Swift：协议
来源：http://oor.yuanzhike.top

protocol Shape { func area() -> Double }
来源：http://bpf.aibaodan.cn

[T31] Lua：Hello World
来源：http://rau.shanyushiyangkeji.top

print("Hello")
来源：http://lju.wangdashe.top

[T32] Lua：局部变量
来源：http://onz.fktsv.cn

local a = 1
来源：http://pdp.uphjek.com

[T33] Lua：表（数组）
来源：http://dgh.ctjpmb.com

local t = {1, 2, 3};  t[4] = 4
来源：http://ptq.svipenyu.cn

[T34] Lua：遍历表
来源：http://xjn.0kj1m.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://dnj.guowangkeji.top

[T35] Lua：字典表
来源：http://hgp.nwbrower.top

local d = { a = 1 };  d.b = 2
来源：http://tuc.ehwqpu.com

[T36] Lua：函数
来源：http://ivn.yuanzhike.top

function add(a, b) return a + b end
来源：http://mwi.xinyue.icu

[T37] Lua：字符串拼接
来源：http://pjj.hysaishi.cn

"a" .. "b"
来源：http://taj.tanke756.top

[T38] Lua：条件
来源：http://iwv.sysykeji.top

if x > 0 then print("正") end
来源：http://kgx.hysaishi.cn

[T39] Lua：模式匹配
来源：http://voj.tanke756.top

string.find(s, "%d+")
来源：http://rjw.shuidangran.top

[T40] Lua：元表
来源：http://hzj.cashguo.top

setmetatable({}, { __index = base })
来源：http://dsf.meibo888.top

[T41] Perl：Hello World
来源：http://tpb.daxiang520.top

print "Hello\n";
来源：http://bye.guannengcc.top

[T42] Perl：变量类型
来源：http://rtu.zhiwuduotai.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ylt.jqgfzy.top

[T43] Perl：字符串插值
来源：http://fjw.shzxlz.cn

"值: $a"
来源：http://uyz.fengsongda.top

[T44] Perl：条件
来源：http://pxe.jinghuilouyu.cn

if ($a > 0) { print "正"; }
来源：http://wxn.gogol.net.cn


<!-- 参考信息 -->