代发 wailian999

find . -name "*.log" -type f
来源：http://civ.fzhhl.top

[R44] 按修改时间查找
来源：http://brl.jinyuanbaomall.cn

find . -mtime -7 -type f
来源：http://tyb.0kj1m.cn

[R45] 批量删除
来源：http://bty.gzhubu.top

find . -name "*.tmp" -delete
来源：http://bla.wangshuangyany.cn

[R46] 递归替换文件内容
来源：http://qpp.jianghu66.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gqn.hywenlv.cn

[R47] sed 单行替换
来源：http://ejd.sysykeji.top

sed -i 's/foo/bar/g' a.txt
来源：http://upk.fengsongda.top

[R48] awk 取指定列
来源：http://jqy.gotoacloud.top

awk '{print $1, $3}' a.txt
来源：http://stx.daria6918.cn

[R49] awk 带条件
来源：http://zxv.sysykeji.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://oeh.jqgufenzy.top

[R50] awk 求和
来源：http://auj.fengsongda.top

awk '{s += $2} END {print s}' a.txt
来源：http://zsh.zdqjudy.top

[R51] 排序去重取前几
来源：http://vke.xingfuxueyuan.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://oyh.jlsjyb.cn

[R52] 统计行数
来源：http://xek.52xcode.cn

wc -l a.txt
来源：http://ztn.bbcook.cn

[R53] 查看文件头与实时尾
来源：http://com.xziqi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dnx.dashuyun.cn

[R54] 比较两个文件
来源：http://lss.meibo888.top

diff a.txt b.txt
来源：http://flz.sysykeji.top

[R55] 压缩与解压
来源：http://sjd.shuidangran.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cpz.mhx1999.top

[R56] 远程拷贝
来源：http://fgf.smart0.xyz

scp file user@host:/path/
来源：http://loh.sysykeji.top

[R57] 远程执行命令
来源：http://lys.xuanzx.com

ssh user@host 'uptime'
来源：http://bra.wangdashe.top

[R58] 下载文件
来源：http://mus.jinyuanbaomall.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sip.guannengcc.top

[R59] 发 POST JSON
来源：http://qed.hongshengwenyu.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wwr.jinyuanbaomall.cn

[R60] 只看 HTTP 状态码
来源：http://trc.wangdashe.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hbh.sysykeji.top

[R61] 磁盘占用
来源：http://ezo.birdmap.top

df -h;  du -sh *
来源：http://viw.jinghuilouyu.cn

[R62] 找最占空间的文件
来源：http://hva.ybcxt.top

du -ah . | sort -rh | head -10
来源：http://siw.yuanzhike.top

[R63] 内存与进程
来源：http://can.c1oappe.top

free -h;  ps aux | grep nginx
来源：http://fdh.haohaochexian.top

[R64] 结束进程
来源：http://xko.birdmap.top

kill -9 $(pgrep -f app.py)
来源：http://zoc.wangdashe.top

[R65] 查看端口占用
来源：http://upn.svipenyu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jyt.ivvv.top

[R66] 定时任务
来源：http://ngj.chenzaomai.com

crontab -e;  crontab -l
来源：http://bod.zdqjudy.top

[R67] 生成随机十六进制串
来源：http://pvp.xuanzx.com

openssl rand -hex 16
来源：http://yox.hongshengwenyu.top

[R68] 计算文件校验值
来源：http://ord.aibaodan.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xpn.bjfxy.top

[R69] 生成随机密码
来源：http://scz.nwbrower.top

head -c 16 /dev/urandom | base64
来源：http://wvf.jiagoushi.top

[R70] 时间戳与互转
来源：http://nwq.wangshuangyany.cn

date +%s;  date -d @1700000000
来源：http://mar.zycfv.cn

[R71] 日期格式化
来源：http://rxw.guannengcc.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://tuf.yj20258.top

[R72] 等待端口就绪
来源：http://ylq.ctjpmb.com

until nc -z localhost 3306; do sleep 1; done
来源：http://wlq.tarul.cn

[R73] 分割大日志
来源：http://akr.shanyushiyangkeji.top

split -l 1000 big.log part_
来源：http://dby.chenzaomai.com

[R74] 批量重命名
来源：http://sia.jianghu66.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://the.9152youxi.cn

[R75] 导出环境变量
来源：http://nrp.zhengqikj.top

export PATH="$HOME/bin:$PATH"
来源：http://sfj.hammf.cn

[R76] 使用临时文件
来源：http://kce.fengsongda.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ygh.ctjpmb.com

[R77] 读取用户输入
来源：http://vly.zycfv.cn

read -rp "请输入: " ans
来源：http://elw.guannengcc.top

[R78] 交互式菜单
来源：http://wyg.guannengcc.top

select opt in a b c; do echo "$opt"; break; done
来源：http://knw.yj202588.top

[R79] 解析命令行选项
来源：http://ort.yfazqb.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pdj.yangfankeji.com

[R80] 查看脚本执行耗时
来源：http://pbp.sysykeji.top

time ./run.sh
来源：http://kqi.xuanzx.com

================================================================================
来源：http://uls.yueranfly.top

S. C / C++ 专题
来源：http://udi.iojbl.cn

================================================================================
来源：http://rlw.pengpengdd.cyou

[S01] C：Hello World
来源：http://akc.sjlbkw.cn

#include <stdio.h>
来源：http://apk.zhoulong.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://ixd.nanxuanxn.top

[S02] C：变量与格式化输出
来源：http://opj.zhixingplan.top

int a = 10; printf("%d\n", a);
来源：http://tfj.yvedp.cn

[S03] C：读入整数
来源：http://aqy.ctjpmb.com

int x; scanf("%d", &x);
来源：http://eat.aizwys.cn

[S04] C：字符串复制
来源：http://uno.hnxiangtu.top

char dst[32]; strcpy(dst, "hi");
来源：http://owv.cashguo.top

[S05] C：字符串长度
来源：http://ugg.xuetiantiany.cn

strlen(s)
来源：http://ydc.zdqjudy.top

[S06] C：字符串比较
来源：http://auy.dashuyun.cn

strcmp(a, b) == 0
来源：http://bpg.jqgufenzy.top

[S07] C：数组遍历求和
来源：http://xpw.yangfankeji.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xhl.gzhubu.top

[S08] C：动态内存分配与释放
来源：http://kai.yangfankeji.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gsh.zycfv.cn

[S09] C：结构体定义与初始化
来源：http://xjq.vehdjk.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://viy.tarul.cn

[S10] C：指针与解引用
来源：http://iap.chenlongwang.top

int *p = &a;  *p = 5;
来源：http://jfa.chenjidiqi.icu

[S11] C：逐行读文件
来源：http://idr.gogol.net.cn

FILE *f = fopen("a.txt", "r");
来源：http://wxo.zdqjudy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://fan.feifeiyinyue.top

fclose(f);
来源：http://sqn.uphjek.com

[S12] C：写文件
来源：http://mhb.yj20258.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xaw.0kj1m.cn

[S13] C：宏定义
来源：http://bdb.hnqzz.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kri.shangyingyoupin.top

[S14] C：枚举
来源：http://bbr.hysaishi.cn

enum Color { RED, GREEN, BLUE };
来源：http://ful.cheryme.top

[S15] C：类型转换
来源：http://ebs.jqgufenzy.top

(double) a / b
来源：http://unq.9152youxi.cn

[S16] C：位操作置位
来源：http://ray.chenzaomai.com

x |= (1 << 3);
来源：http://eut.jlsjyb.cn

[S17] C：安全拼接字符串
来源：http://bma.kuanghao11.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wwg.ybcxt.top

[S18] C：命令行参数
来源：http://bhe.hysaishi.cn

int main(int argc, char **argv)
来源：http://eke.jinyuanbaomall.cn

[S19] C：快速排序
来源：http://mcc.hywenlv.cn

qsort(a, n, sizeof(int), cmp);
来源：http://wzx.316326.xyz

[S20] C：二分查找
来源：http://eno.shuidangran.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://iph.sjlbkw.cn

[S21] C：字符类别判断
来源：http://ggm.yueranfly.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hlq.cheryme.top

[S22] C：字符串转数字
来源：http://uts.sufxvd.cn

atoi("42");  strtod("3.14", NULL);
来源：http://aab.hnxiangtu.top

[S23] C：随机数
来源：http://cij.birdmap.top

srand(time(NULL));  int r = rand() % 100;
来源：http://bhn.jinyuanbaomall.cn

[S24] C：获取本地时间
来源：http://zyd.vehdjk.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ryq.sysykeji.top

[S25] C：内存拷贝
来源：http://sxz.zhiwuduotai.top

memcpy(dst, src, n);
来源：http://elo.xuanzx.com

[S26] C：内存清零
来源：http://rju.yongpay.top

memset(a, 0, sizeof a);
来源：http://shn.yuanzhike.top

[S27] C：定义常量
来源：http://vco.zdqjudy.top

const double PI = 3.14159;
来源：http://nfq.cucudq.cn

[S28] C：静态变量
来源：http://now.cqqwz.cn

static int counter = 0;
来源：http://ybn.mhx1999.top

[S29] C：变参函数
来源：http://bro.meibo888.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kyn.jqgfzy.top

[S30] C：头文件保护
来源：http://yui.fehbvm.com

#ifndef X_H
来源：http://ivq.wangdashe.top

#define X_H
来源：http://rnc.sweek.top

#endif
来源：http://kug.uphjek.com

[S31] C++：Hello World
来源：http://kca.ydzc1.top

#include <iostream>
来源：http://smm.guannengcc.top

int main() { std::cout << "Hello\n"; }
来源：http://yxz.0kj1m.cn

[S32] C++：字符串
来源：http://rff.jqgufenzy.top

std::string s = "hi";  s += "!";
来源：http://bqw.yj20258.top

[S33] C++：vector 增删
来源：http://yvs.cucudq.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://iwu.aizwys.cn

[S34] C++：遍历 vector
来源：http://zzj.redwolf501.top

for (auto &x : v) { std::cout << x; }
来源：http://diy.sweek.top

[S35] C++：map
来源：http://rkv.tian-w.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jcw.bjfxy.top

[S36] C++：unordered_map
来源：http://adu.xinyue.icu

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wki.hongshengwenyu.top

[S37] C++：set
来源：http://zad.pycfn.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tcw.smart0.xyz

[S38] C++：排序
来源：http://sxd.tanke756.top

std::sort(v.begin(), v.end());
来源：http://dlg.gaohongyu789.top

[S39] C++：自定义比较器排序
来源：http://lgf.cqqwz.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zfr.redwolf501.top

[S40] C++：查找元素
来源：http://frf.ydzc1.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zup.sjlbkw.cn

[S41] C++：类与构造函数
来源：http://eky.hesvh.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gro.shzxlz.cn

[S42] C++：继承与虚函数
来源：http://gml.tianlin.xyz

class B : public Base { public: void f() override {} };
来源：http://kms.yonumen.top

[S43] C++：智能指针
来源：http://qbo.quarkkingdee.top

auto p = std::make_unique<int>(5);
来源：http://sos.gogol.net.cn

[S44] C++：引用传参
来源：http://nxx.hywenlv.cn

void inc(int &x) { ++x; }
来源：http://frw.kuanghao11.cn

[S45] C++：lambda
来源：http://vfj.cucudq.cn

auto add = [](int a, int b) { return a + b; };
来源：http://uuc.pengpengdd.cyou

[S46] C++：函数模板
来源：http://kvi.uphjek.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xys.shangyingyoupin.top

[S47] C++：结构化绑定遍历
来源：http://gtg.0kj1m.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://icn.epnwcf.com

[S48] C++：逐行读文件
来源：http://udv.yfazqb.com

std::ifstream in("a.txt");  std::string line;
来源：http://mxt.jiagoushi.top

while (std::getline(in, line)) { }
来源：http://snz.xylfe.cn

[S49] C++：写文件
来源：http://ytq.xuetiantiany.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mmy.vehdjk.com

[S50] C++：格式化数字
来源：http://asy.bbcook.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://eom.yj202588.top

[S51] C++：显式类型转换
来源：http://ivy.gotoacloud.top

static_cast<double>(a) / b
来源：http://umn.sjlbkw.cn

[S52] C++：const 与 noexcept
来源：http://udp.shanyushiyangtech.top

int size() const noexcept { return n_; }
来源：http://nix.meibo888.top

[S53] C++：移动语义
来源：http://lvq.hywenlv.cn

std::vector<int> w = std::move(v);
来源：http://nae.jqgufenzy.top

[S54] C++：异常处理
来源：http://gqv.yfazqb.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ynr.pycfn.com

[S55] C++：结构化绑定
来源：http://wwe.xuetiantiany.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://cbx.cucudq.cn

[S56] C++：optional
来源：http://mnx.pycfn.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qmb.zhixingplan.top

[S57] C++：编译期常量
来源：http://qpf.yonumen.top

constexpr int N = 10;
来源：http://gik.yueranfly.top

[S58] C++：命名空间
来源：http://jox.yanxiufei.cn

namespace ns { int f() { return 1; } }
来源：http://ylm.yj202588.top

[S59] C++：静态断言
来源：http://qsz.jyoumei.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://brm.pengpengdd.cyou

[S60] C++：遍历并删除元素
来源：http://ffm.iojbl.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zej.shanyushiyangtech.top

================================================================================
来源：http://rux.yueranfly.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rfw.yuanzhike.top

================================================================================
来源：http://fpu.tian-w.cn

[T01] Kotlin：Hello World
来源：http://lzg.guannengcc.top

println("Hello")
来源：http://pnf.hnxiangtu.top

[T02] Kotlin：变量
来源：http://hta.iojbl.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xli.birdmap.top

[T03] Kotlin：字符串模板
来源：http://mmz.tanke756.top

"值: $b"
来源：http://uym.nanxinkj.top

[T04] Kotlin：空安全
来源：http://bsr.sxryk.cn

val n: String? = null;  n?.length
来源：http://ill.tarul.cn

[T05] Kotlin：when 表达式
来源：http://cop.jinqigufen.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nsx.hesvh.cn

[T06] Kotlin：集合映射
来源：http://onh.shzxlz.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://vil.jinqigufen.top

[T07] Kotlin：集合过滤
来源：http://ctj.cheryme.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://nyi.xinyue.icu

[T08] Kotlin：数据类
来源：http://wpc.snrcjt.cn

data class User(val name: String, val age: Int)
来源：http://pzi.wangshuangyany.cn

[T09] Kotlin：扩展函数
来源：http://umn.c1oappe.top

fun String.exclaim() = this + "!"
来源：http://htx.nwbrower.top

[T10] Kotlin：默认参数
来源：http://jzr.shangyingyoupin.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ksg.aizwys.cn

[T11] Kotlin：协程
来源：http://pmv.fzhhl.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ofj.gogol.net.cn

[T12] Kotlin：解构声明
来源：http://wzb.yangfankeji.com

val (a, b) = Pair(1, 2)
来源：http://dbg.fehbvm.com

[T13] Kotlin：只读 Map
来源：http://xbm.tian-w.cn

val m = mapOf("a" to 1)
来源：http://nwt.feifeiyinyue.top

[T14] Kotlin：循环
来源：http://tlz.andypj.xyz

for (i in 1..10) println(i)
来源：http://uvh.chenjidiqi.icu

[T15] Kotlin：接口
来源：http://mzg.fengsongda.top

interface Shape { fun area(): Double }
来源：http://pjj.ppjwa.cn

[T16] Swift：Hello World
来源：http://cip.smart0.xyz

print("Hello")
来源：http://rbm.feifeiyinyue.top

[T17] Swift：变量与常量
来源：http://jmi.c1oappe.top

var a = 1;  let b = 2
来源：http://ojl.xingfuxueyuan.xyz

[T18] Swift：字符串插值
来源：http://stn.jinqigfzy.top

"值: \(b)"
来源：http://juo.sufxvd.cn

[T19] Swift：可选绑定
来源：http://dew.iojbl.cn

if let n = opt { print(n) }
来源：http://pbb.hongshengwenyu.top

[T20] Swift：数组操作
来源：http://soq.gzhubu.top

var a = [1, 2, 3];  a.append(4)
来源：http://eul.guowangkeji.top

[T21] Swift：遍历
来源：http://bxm.redwolf501.top

for x in a { print(x) }
来源：http://ykj.cheryme.top

[T22] Swift：字典
来源：http://elg.yangfankeji.com

var d = ["a": 1];  d["b"] = 2
来源：http://qde.aibaodan.cn

[T23] Swift：函数
来源：http://oqp.pengpengdd.cyou

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ldx.fengsongda.top

[T24] Swift：闭包
来源：http://nbc.ivvv.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://lei.0kj1m.cn

[T25] Swift：结构体
来源：http://uqb.fzhhl.top

struct P { var x: Int }
来源：http://rrj.nanxinkj.top

[T26] Swift：类与重写
来源：http://car.vehdjk.com

class A: Base { override func f() {} }
来源：http://yyo.aizwys.cn

[T27] Swift：错误处理
来源：http://ptz.gogol.net.cn

do { try f() } catch { print(error) }
来源：http://ozs.xuanzx.com

[T28] Swift：枚举
来源：http://xfs.zhijiandao.cn

enum Color { case red, green }
来源：http://ewz.yangfankeji.com

[T29] Swift：guard 提前返回
来源：http://nli.sjlbkw.cn

guard let x = opt else { return }
来源：http://tqi.uphjek.com

[T30] Swift：协议
来源：http://fmq.gogol.net.cn

protocol Shape { func area() -> Double }
来源：http://uhb.yuanzhike.top

[T31] Lua：Hello World
来源：http://pjl.yj20258888.top

print("Hello")
来源：http://zxa.jyoumei.cn

[T32] Lua：局部变量
来源：http://ibi.daria6918.cn

local a = 1
来源：http://ajh.fktsv.cn

[T33] Lua：表（数组）
来源：http://nhu.andypj.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://ukl.guowangkeji.top

[T34] Lua：遍历表
来源：http://vwh.iojbl.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://cdw.yuxming.cn

[T35] Lua：字典表
来源：http://rsp.chenlongwang.top

local d = { a = 1 };  d.b = 2
来源：http://sxk.52xcode.cn

[T36] Lua：函数
来源：http://ize.daxiang520.top

function add(a, b) return a + b end
来源：http://nxn.zhongyouzk.top

[T37] Lua：字符串拼接
来源：http://kdz.hnxiangtu.top

"a" .. "b"
来源：http://akp.tianlin.xyz

[T38] Lua：条件
来源：http://zoc.yueranfly.top

if x > 0 then print("正") end
来源：http://uum.shzxlz.cn

[T39] Lua：模式匹配
来源：http://ibj.zhijiandao.cn

string.find(s, "%d+")
来源：http://lax.bjfxy.top

[T40] Lua：元表
来源：http://zqx.shanyushiyangtech.top

setmetatable({}, { __index = base })
来源：http://jvk.yuanzhike.top

[T41] Perl：Hello World
来源：http://dqk.uphjek.com

print "Hello\n";
来源：http://laa.jqgufenzy.top

[T42] Perl：变量类型
来源：http://llb.xingfuxueyuan.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jbk.pengpengdd.cyou

[T43] Perl：字符串插值
来源：http://pug.gzhubu.top

"值: $a"
来源：http://byu.ivvv.top

[T44] Perl：条件
来源：http://ijy.yuanzhike.top

if ($a > 0) { print "正"; }
来源：http://wjx.fehbvm.com

[T45] Perl：数组遍历
来源：http://cro.hysaishi.cn

for my $x (@arr) { print $x; }
来源：http://isf.vqdsnc.cn

[T46] Perl：哈希操作
来源：http://hsa.hnxiangtu.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://yop.pycfn.com


<!-- 参考信息 -->