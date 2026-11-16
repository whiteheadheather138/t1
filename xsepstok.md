代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://ztv.jinghuilouyu.cn

[R48] awk 取指定列
来源：http://njl.wangdashe.top

awk '{print $1, $3}' a.txt
来源：http://ava.guowangkeji.top

[R49] awk 带条件
来源：http://ksq.daria6918.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mlp.vqdsnc.cn

[R50] awk 求和
来源：http://evc.jinqigufen.top

awk '{s += $2} END {print s}' a.txt
来源：http://rlo.shangyingyoupin.top

[R51] 排序去重取前几
来源：http://ihr.jqgfzy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://nlh.nanxinkj.top

[R52] 统计行数
来源：http://cyl.shanyushiyangkeji.top

wc -l a.txt
来源：http://ffu.yonumen.top

[R53] 查看文件头与实时尾
来源：http://khs.gzhubu.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://udz.zhongyouzk.top

[R54] 比较两个文件
来源：http://svq.yueranfly.top

diff a.txt b.txt
来源：http://lzq.jianghu66.top

[R55] 压缩与解压
来源：http://ngm.cqqwz.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blu.hammf.cn

[R56] 远程拷贝
来源：http://yhz.xziqi.cn

scp file user@host:/path/
来源：http://yuu.zdqjudy.top

[R57] 远程执行命令
来源：http://oay.chenlongwang.top

ssh user@host 'uptime'
来源：http://lzh.sxryk.cn

[R58] 下载文件
来源：http://azt.jqgufenzy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://inc.iojbl.cn

[R59] 发 POST JSON
来源：http://dcs.yangfankeji.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://oru.zhijiandao.cn

[R60] 只看 HTTP 状态码
来源：http://kni.yj202588.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zrm.uphjek.com

[R61] 磁盘占用
来源：http://fxb.daria6918.cn

df -h;  du -sh *
来源：http://dao.tarul.cn

[R62] 找最占空间的文件
来源：http://ctl.cashguo.top

du -ah . | sort -rh | head -10
来源：http://khh.zhijiandao.cn

[R63] 内存与进程
来源：http://btw.fanxiaobao.xyz

free -h;  ps aux | grep nginx
来源：http://cui.zhoulong.xyz

[R64] 结束进程
来源：http://azc.gogol.net.cn

kill -9 $(pgrep -f app.py)
来源：http://nob.0kj1m.cn

[R65] 查看端口占用
来源：http://cyn.hywenlv.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mfm.316326.xyz

[R66] 定时任务
来源：http://qqz.hnxiangtu.top

crontab -e;  crontab -l
来源：http://fds.cheryme.top

[R67] 生成随机十六进制串
来源：http://ewv.ywan-chungtsiang.top

openssl rand -hex 16
来源：http://lhz.meibo888.top

[R68] 计算文件校验值
来源：http://cco.zhoulong.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://tzi.hongshengwenyu.top

[R69] 生成随机密码
来源：http://fjc.yuxming.cn

head -c 16 /dev/urandom | base64
来源：http://fna.snrcjt.cn

[R70] 时间戳与互转
来源：http://fcn.jinqigufen.top

date +%s;  date -d @1700000000
来源：http://mqn.iojbl.cn

[R71] 日期格式化
来源：http://sei.fanxiaobao.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://aoe.epnwcf.com

[R72] 等待端口就绪
来源：http://xzq.cqqwz.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://kdq.yj20258.top

[R73] 分割大日志
来源：http://aym.sjlbkw.cn

split -l 1000 big.log part_
来源：http://mye.andypj.xyz

[R74] 批量重命名
来源：http://ulb.kuanghao11.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wai.jinqigufen.top

[R75] 导出环境变量
来源：http://ogk.gzhubu.top

export PATH="$HOME/bin:$PATH"
来源：http://vqu.hammf.cn

[R76] 使用临时文件
来源：http://kui.shangyingyoupin.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rao.jinqigufen.top

[R77] 读取用户输入
来源：http://twy.daria6918.cn

read -rp "请输入: " ans
来源：http://tnb.kuanghao11.cn

[R78] 交互式菜单
来源：http://lzz.hongshengwenyu.top

select opt in a b c; do echo "$opt"; break; done
来源：http://sub.ydzc1.top

[R79] 解析命令行选项
来源：http://zzi.dianchejie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cfb.haohaochexian.top

[R80] 查看脚本执行耗时
来源：http://avk.yj202588.top

time ./run.sh
来源：http://kvv.gaohongyu789.top

================================================================================
来源：http://wxl.zhixingplan.top

S. C / C++ 专题
来源：http://nte.nanxinkj.top

================================================================================
来源：http://dhf.yuxming.cn

[S01] C：Hello World
来源：http://ekn.smart0.xyz

#include <stdio.h>
来源：http://vqd.gogol.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qqg.hywenlv.cn

[S02] C：变量与格式化输出
来源：http://rxr.zhiwuduotai.top

int a = 10; printf("%d\n", a);
来源：http://wtq.ehwqpu.com

[S03] C：读入整数
来源：http://xmt.shanyushiyangkeji.top

int x; scanf("%d", &x);
来源：http://mom.yanxiufei.cn

[S04] C：字符串复制
来源：http://axm.chenjidiqi.icu

char dst[32]; strcpy(dst, "hi");
来源：http://spe.xingfuxueyuan.xyz

[S05] C：字符串长度
来源：http://bqt.bjfxy.top

strlen(s)
来源：http://ucw.sjlbkw.cn

[S06] C：字符串比较
来源：http://dmw.mhx1999.top

strcmp(a, b) == 0
来源：http://tcm.hesvh.cn

[S07] C：数组遍历求和
来源：http://fbp.sufxvd.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://roq.nanxuanxn.top

[S08] C：动态内存分配与释放
来源：http://opq.gaohongyu789.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uol.haohaochexian.top

[S09] C：结构体定义与初始化
来源：http://xkt.ctjpmb.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zsu.cdnleiting.top

[S10] C：指针与解引用
来源：http://pkw.bbcook.cn

int *p = &a;  *p = 5;
来源：http://zjz.hywenlv.cn

[S11] C：逐行读文件
来源：http://cef.316326.xyz

FILE *f = fopen("a.txt", "r");
来源：http://eyd.fanxiaobao.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://ujo.snrcjt.cn

fclose(f);
来源：http://mjq.sweek.top

[S12] C：写文件
来源：http://gma.ywan-chungtsiang.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://eqb.tian-w.cn

[S13] C：宏定义
来源：http://utv.fengsongda.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ohf.c1oappe.top

[S14] C：枚举
来源：http://etz.havefunace.top

enum Color { RED, GREEN, BLUE };
来源：http://etu.nwbrower.top

[S15] C：类型转换
来源：http://mds.yuxming.cn

(double) a / b
来源：http://lio.chenlongwang.top

[S16] C：位操作置位
来源：http://kxz.yfazqb.com

x |= (1 << 3);
来源：http://dkd.pengpengdd.cyou

[S17] C：安全拼接字符串
来源：http://npm.quarkkingdee.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hzo.hammf.cn

[S18] C：命令行参数
来源：http://esd.jyoumei.cn

int main(int argc, char **argv)
来源：http://une.yongpay.top

[S19] C：快速排序
来源：http://gak.shangyingyoupin.top

qsort(a, n, sizeof(int), cmp);
来源：http://bae.hesvh.cn

[S20] C：二分查找
来源：http://qtf.shanyushiyangkeji.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hld.nwbrower.top

[S21] C：字符类别判断
来源：http://syc.fehbvm.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://utn.xziqi.cn

[S22] C：字符串转数字
来源：http://ivg.quarkkingdee.top

atoi("42");  strtod("3.14", NULL);
来源：http://qab.uphjek.com

[S23] C：随机数
来源：http://arh.tian-w.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://plm.chenzaomai.com

[S24] C：获取本地时间
来源：http://neg.cheryme.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rsh.hesvh.cn

[S25] C：内存拷贝
来源：http://gsv.hammf.cn

memcpy(dst, src, n);
来源：http://bqg.xingfuxueyuan.xyz

[S26] C：内存清零
来源：http://hyv.yangfankeji.com

memset(a, 0, sizeof a);
来源：http://ijs.jqgfzy.top

[S27] C：定义常量
来源：http://qoa.smart0.xyz

const double PI = 3.14159;
来源：http://ldv.gotoacloud.top

[S28] C：静态变量
来源：http://fqg.nanxinkj.top

static int counter = 0;
来源：http://qpi.svipenyu.cn

[S29] C：变参函数
来源：http://tur.bjfxy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://afu.bbcook.cn

[S30] C：头文件保护
来源：http://bwn.kuanghao11.cn

#ifndef X_H
来源：http://nvi.ctjpmb.com

#define X_H
来源：http://rnr.xingfuxueyuan.xyz

#endif
来源：http://inz.aibaodan.cn

[S31] C++：Hello World
来源：http://oxg.cdnleiting.top

#include <iostream>
来源：http://dab.sweek.top

int main() { std::cout << "Hello\n"; }
来源：http://nra.ydzc1.top

[S32] C++：字符串
来源：http://taw.jlsjyb.cn

std::string s = "hi";  s += "!";
来源：http://thw.shangyingyoupin.top

[S33] C++：vector 增删
来源：http://tty.cdnleiting.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qkj.tian-w.cn

[S34] C++：遍历 vector
来源：http://nae.yanxiufei.cn

for (auto &x : v) { std::cout << x; }
来源：http://ere.redwolf501.top

[S35] C++：map
来源：http://jeg.chenzaomai.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mcy.zdqjudy.top

[S36] C++：unordered_map
来源：http://liw.hesvh.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ftd.ydzc1.top

[S37] C++：set
来源：http://yqv.tanke756.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://riz.c1oappe.top

[S38] C++：排序
来源：http://enu.guannengcc.top

std::sort(v.begin(), v.end());
来源：http://ykf.fanxiaobao.xyz

[S39] C++：自定义比较器排序
来源：http://wbq.ywan-chungtsiang.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://clf.meibo888.top

[S40] C++：查找元素
来源：http://dgk.kuanghao11.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ifc.svipenyu.cn

[S41] C++：类与构造函数
来源：http://bgv.xuetiantiany.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lge.hywenlv.cn

[S42] C++：继承与虚函数
来源：http://qtu.epnwcf.com

class B : public Base { public: void f() override {} };
来源：http://juv.fzhhl.top

[S43] C++：智能指针
来源：http://cnr.jqgfzy.top

auto p = std::make_unique<int>(5);
来源：http://svi.pycfn.com

[S44] C++：引用传参
来源：http://akp.aizwys.cn

void inc(int &x) { ++x; }
来源：http://yus.jqgfzy.top

[S45] C++：lambda
来源：http://ulk.tian-w.cn

auto add = [](int a, int b) { return a + b; };
来源：http://kvw.andypj.xyz

[S46] C++：函数模板
来源：http://tbw.jinyuanbaomall.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zbh.jinqigufen.top

[S47] C++：结构化绑定遍历
来源：http://dsy.shuidangran.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yqt.xinyue.icu

[S48] C++：逐行读文件
来源：http://zpz.ehwqpu.com

std::ifstream in("a.txt");  std::string line;
来源：http://ydv.havefunace.top

while (std::getline(in, line)) { }
来源：http://rhm.sjlbkw.cn

[S49] C++：写文件
来源：http://kgy.birdmap.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bmm.zhixingplan.top

[S50] C++：格式化数字
来源：http://ldg.yj202588.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lcf.chenjidiqi.icu

[S51] C++：显式类型转换
来源：http://ijg.ydjk.org.cn

static_cast<double>(a) / b
来源：http://rlm.jinyuanbaomall.cn

[S52] C++：const 与 noexcept
来源：http://tis.nwbrower.top

int size() const noexcept { return n_; }
来源：http://umx.vehdjk.com

[S53] C++：移动语义
来源：http://jre.gogol.net.cn

std::vector<int> w = std::move(v);
来源：http://zrl.cheryme.top

[S54] C++：异常处理
来源：http://txb.svipenyu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bry.havefunace.top

[S55] C++：结构化绑定
来源：http://umw.haohaochexian.top

auto [a, b] = std::make_pair(1, 2);
来源：http://vkm.sweek.top

[S56] C++：optional
来源：http://amv.birdmap.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://skb.bjfxy.top

[S57] C++：编译期常量
来源：http://szt.yfazqb.com

constexpr int N = 10;
来源：http://zgq.wangshuangyany.cn

[S58] C++：命名空间
来源：http://nzw.zhiwuduotai.top

namespace ns { int f() { return 1; } }
来源：http://ijy.hcnkem.com

[S59] C++：静态断言
来源：http://xpe.smart0.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rzf.aibaodan.cn

[S60] C++：遍历并删除元素
来源：http://zhc.iojbl.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cmz.hongshengwenyu.top

================================================================================
来源：http://jli.havefunace.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kve.tarul.cn

================================================================================
来源：http://nlr.redwolf501.top

[T01] Kotlin：Hello World
来源：http://lob.fengsongda.top

println("Hello")
来源：http://spx.zhoulong.xyz

[T02] Kotlin：变量
来源：http://thx.gaohongyu789.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://doj.wangdashe.top

[T03] Kotlin：字符串模板
来源：http://xwz.0kj1m.cn

"值: $b"
来源：http://cpm.wangshuangyany.cn

[T04] Kotlin：空安全
来源：http://ruo.iojbl.cn

val n: String? = null;  n?.length
来源：http://zya.jinqigfzy.top

[T05] Kotlin：when 表达式
来源：http://vyj.bbcook.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://igu.daxiang520.top

[T06] Kotlin：集合映射
来源：http://jnb.hysaishi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://mys.quarkkingdee.top

[T07] Kotlin：集合过滤
来源：http://cqr.fzhhl.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://fob.yonumen.top

[T08] Kotlin：数据类
来源：http://wvy.xingfuxueyuan.xyz

data class User(val name: String, val age: Int)
来源：http://wlq.yangfankeji.com

[T09] Kotlin：扩展函数
来源：http://gik.fehbvm.com

fun String.exclaim() = this + "!"
来源：http://mar.xziqi.cn

[T10] Kotlin：默认参数
来源：http://duv.jinyuanbaomall.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://mws.xylfe.cn

[T11] Kotlin：协程
来源：http://mgu.gogol.net.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://rku.yj202588.top

[T12] Kotlin：解构声明
来源：http://aeg.0kj1m.cn

val (a, b) = Pair(1, 2)
来源：http://wbv.quarkkingdee.top

[T13] Kotlin：只读 Map
来源：http://rsi.9152youxi.cn

val m = mapOf("a" to 1)
来源：http://wei.iojbl.cn

[T14] Kotlin：循环
来源：http://bgn.zhongyouzk.top

for (i in 1..10) println(i)
来源：http://qaz.quarkkingdee.top

[T15] Kotlin：接口
来源：http://iol.hfpthk.cn

interface Shape { fun area(): Double }
来源：http://nyx.shanyushiyangtech.top

[T16] Swift：Hello World
来源：http://eiu.sufxvd.cn

print("Hello")
来源：http://ebh.shanyushiyangkeji.top

[T17] Swift：变量与常量
来源：http://syv.fehbvm.com

var a = 1;  let b = 2
来源：http://naa.pengpengdd.cyou

[T18] Swift：字符串插值
来源：http://mkf.aizwys.cn

"值: \(b)"
来源：http://yjm.ydjk.org.cn

[T19] Swift：可选绑定
来源：http://ahz.316326.xyz

if let n = opt { print(n) }
来源：http://djb.jiagoushi.top

[T20] Swift：数组操作
来源：http://fhx.yuxming.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qdi.ehwqpu.com

[T21] Swift：遍历
来源：http://vuz.bjfxy.top

for x in a { print(x) }
来源：http://vja.yj20258.top

[T22] Swift：字典
来源：http://ltk.xingfuxueyuan.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://hlq.yueranfly.top

[T23] Swift：函数
来源：http://fsd.smart0.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://utp.cucudq.cn

[T24] Swift：闭包
来源：http://pui.shanyushiyangtech.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://rim.jianghu66.top

[T25] Swift：结构体
来源：http://gns.xylfe.cn

struct P { var x: Int }
来源：http://voy.jlsjyb.cn

[T26] Swift：类与重写
来源：http://skr.chenjidiqi.icu

class A: Base { override func f() {} }
来源：http://nxm.tarul.cn

[T27] Swift：错误处理
来源：http://krl.ydjk.org.cn

do { try f() } catch { print(error) }
来源：http://vxt.gotoacloud.top

[T28] Swift：枚举
来源：http://ayd.sufxvd.cn

enum Color { case red, green }
来源：http://tpk.ivvv.top

[T29] Swift：guard 提前返回
来源：http://wvp.snrcjt.cn

guard let x = opt else { return }
来源：http://xwg.cheryme.top

[T30] Swift：协议
来源：http://ymp.zhijiandao.cn

protocol Shape { func area() -> Double }
来源：http://krz.daxiang520.top

[T31] Lua：Hello World
来源：http://zxb.fzhhl.top

print("Hello")
来源：http://rfd.zhoulong.xyz

[T32] Lua：局部变量
来源：http://qlb.jqgfzy.top

local a = 1
来源：http://bpt.svipenyu.cn

[T33] Lua：表（数组）
来源：http://uzg.ydjk.org.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fyr.jianghu66.top

[T34] Lua：遍历表
来源：http://vfz.hesvh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://kft.nanxinkj.top

[T35] Lua：字典表
来源：http://xtd.yj202588.top

local d = { a = 1 };  d.b = 2
来源：http://lev.fengsongda.top

[T36] Lua：函数
来源：http://aew.zycfv.cn

function add(a, b) return a + b end
来源：http://ztk.gaohongyu789.top

[T37] Lua：字符串拼接
来源：http://jze.yanxiufei.cn

"a" .. "b"
来源：http://rch.zhongyouzk.top

[T38] Lua：条件
来源：http://wae.jinghuilouyu.cn

if x > 0 then print("正") end
来源：http://ilr.zhengqikj.top

[T39] Lua：模式匹配
来源：http://lur.ppjwa.cn

string.find(s, "%d+")
来源：http://lpg.ydzc1.top

[T40] Lua：元表
来源：http://sxm.jinqigfzy.top

setmetatable({}, { __index = base })
来源：http://jap.pycfn.com

[T41] Perl：Hello World
来源：http://gka.aizwys.cn

print "Hello\n";
来源：http://ejm.xingfuxueyuan.xyz

[T42] Perl：变量类型
来源：http://dhi.aibaodan.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nsu.nanxinkj.top

[T43] Perl：字符串插值
来源：http://dcj.zhoulong.xyz

"值: $a"
来源：http://yut.daria6918.cn

[T44] Perl：条件
来源：http://fgz.chenjidiqi.icu

if ($a > 0) { print "正"; }
来源：http://gsb.hywenlv.cn

[T45] Perl：数组遍历
来源：http://ycy.ppjwa.cn

for my $x (@arr) { print $x; }
来源：http://rmb.jlsjyb.cn

[T46] Perl：哈希操作
来源：http://bqi.sjlbkw.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kzu.yangfankeji.com

[T47] Perl：正则捕获
来源：http://xsl.xuetiantiany.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://oxf.yj202588.top

[T48] Perl：正则替换
来源：http://ion.ivvv.top

$s =~ s/old/new/g;
来源：http://ezm.yongpay.top

[T49] Perl：函数
来源：http://img.ybcxt.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bsh.zhijiandao.cn

[T50] Perl：逐行读文件
来源：http://xwz.zycfv.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://mgm.chenlongwang.top


<!-- 参考信息 -->