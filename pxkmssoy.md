代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://met.jyoumei.cn

[R48] awk 取指定列
来源：http://str.vehdjk.com

awk '{print $1, $3}' a.txt
来源：http://hhk.feifeiyinyue.top

[R49] awk 带条件
来源：http://yuy.zhongyouzk.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cjw.uphjek.com

[R50] awk 求和
来源：http://ztt.haohaochexian.top

awk '{s += $2} END {print s}' a.txt
来源：http://lfs.ehwqpu.com

[R51] 排序去重取前几
来源：http://kzq.zhixingplan.top

sort a.txt | uniq -c | sort -rn | head
来源：http://hzg.zhongyouzk.top

[R52] 统计行数
来源：http://gzn.yongpay.top

wc -l a.txt
来源：http://uwb.xuanzx.com

[R53] 查看文件头与实时尾
来源：http://tdk.dashuyun.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ykm.pycfn.com

[R54] 比较两个文件
来源：http://kgl.tianlin.xyz

diff a.txt b.txt
来源：http://xpm.fktsv.cn

[R55] 压缩与解压
来源：http://dmi.redwolf501.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vhs.fktsv.cn

[R56] 远程拷贝
来源：http://sxm.hammf.cn

scp file user@host:/path/
来源：http://rka.hnqzz.top

[R57] 远程执行命令
来源：http://vsf.fengsongda.top

ssh user@host 'uptime'
来源：http://sob.zhiwuduotai.top

[R58] 下载文件
来源：http://hny.jqgfzy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gsh.meibo888.top

[R59] 发 POST JSON
来源：http://pfm.shuidangran.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://phq.feifeiyinyue.top

[R60] 只看 HTTP 状态码
来源：http://lyk.jqgufenzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rkt.bjfxy.top

[R61] 磁盘占用
来源：http://nwh.jqgfzy.top

df -h;  du -sh *
来源：http://kjt.zhoulong.xyz

[R62] 找最占空间的文件
来源：http://pfj.jyoumei.cn

du -ah . | sort -rh | head -10
来源：http://vko.nanxuanxn.top

[R63] 内存与进程
来源：http://hec.birdmap.top

free -h;  ps aux | grep nginx
来源：http://zka.c1oappe.top

[R64] 结束进程
来源：http://jno.chenzaomai.com

kill -9 $(pgrep -f app.py)
来源：http://eki.jiagoushi.top

[R65] 查看端口占用
来源：http://wkt.aizwys.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fya.ybcxt.top

[R66] 定时任务
来源：http://cqt.dashuyun.cn

crontab -e;  crontab -l
来源：http://lfd.zhaomingkeji.xyz

[R67] 生成随机十六进制串
来源：http://usl.yuanzhike.top

openssl rand -hex 16
来源：http://ewx.fengsongda.top

[R68] 计算文件校验值
来源：http://mab.snrcjt.cn

sha256sum a.txt;  md5sum a.txt
来源：http://opa.9152youxi.cn

[R69] 生成随机密码
来源：http://jng.tarul.cn

head -c 16 /dev/urandom | base64
来源：http://ilu.snrcjt.cn

[R70] 时间戳与互转
来源：http://ybu.sysykeji.top

date +%s;  date -d @1700000000
来源：http://hnp.hammf.cn

[R71] 日期格式化
来源：http://yfz.nanxinkj.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://bbf.dashuyun.cn

[R72] 等待端口就绪
来源：http://zdd.zdqjudy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://lla.9152youxi.cn

[R73] 分割大日志
来源：http://mja.feifeiyinyue.top

split -l 1000 big.log part_
来源：http://ikm.zdqjudy.top

[R74] 批量重命名
来源：http://yjv.xylfe.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fyo.zhoulong.xyz

[R75] 导出环境变量
来源：http://nuc.fanxiaobao.xyz

export PATH="$HOME/bin:$PATH"
来源：http://etm.ivvv.top

[R76] 使用临时文件
来源：http://ojs.fzhhl.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://uex.zdqjudy.top

[R77] 读取用户输入
来源：http://aio.52xcode.cn

read -rp "请输入: " ans
来源：http://riw.zhengqikj.top

[R78] 交互式菜单
来源：http://rjn.yj20258.top

select opt in a b c; do echo "$opt"; break; done
来源：http://hxc.0kj1m.cn

[R79] 解析命令行选项
来源：http://cjp.yuanzhike.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://smp.uphjek.com

[R80] 查看脚本执行耗时
来源：http://vqx.bbcook.cn

time ./run.sh
来源：http://bqa.hongshengwenyu.top

================================================================================
来源：http://uzf.fanxiaobao.xyz

S. C / C++ 专题
来源：http://rav.svipenyu.cn

================================================================================
来源：http://lar.cqqwz.cn

[S01] C：Hello World
来源：http://ojt.yvedp.cn

#include <stdio.h>
来源：http://pks.fehbvm.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://syg.feifeiyinyue.top

[S02] C：变量与格式化输出
来源：http://ecu.cashguo.top

int a = 10; printf("%d\n", a);
来源：http://zti.vqdsnc.cn

[S03] C：读入整数
来源：http://stp.guannengcc.top

int x; scanf("%d", &x);
来源：http://ukp.birdmap.top

[S04] C：字符串复制
来源：http://nai.c1oappe.top

char dst[32]; strcpy(dst, "hi");
来源：http://iwq.chenjidiqi.icu

[S05] C：字符串长度
来源：http://ffi.pengpengdd.cyou

strlen(s)
来源：http://iel.vqdsnc.cn

[S06] C：字符串比较
来源：http://win.aibaodan.cn

strcmp(a, b) == 0
来源：http://mim.snrcjt.cn

[S07] C：数组遍历求和
来源：http://muw.shanyushiyangtech.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rrt.xylfe.cn

[S08] C：动态内存分配与释放
来源：http://oaq.tanke756.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kqd.jinqigfzy.top

[S09] C：结构体定义与初始化
来源：http://zbv.nanxinkj.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pgy.zycfv.cn

[S10] C：指针与解引用
来源：http://nay.fzhhl.top

int *p = &a;  *p = 5;
来源：http://vfe.hesvh.cn

[S11] C：逐行读文件
来源：http://vof.yonumen.top

FILE *f = fopen("a.txt", "r");
来源：http://khn.jyoumei.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://wbi.havefunace.top

fclose(f);
来源：http://wws.yj202588.top

[S12] C：写文件
来源：http://euw.hammf.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jlg.redwolf501.top

[S13] C：宏定义
来源：http://cmc.vqdsnc.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sxl.kuanghao11.cn

[S14] C：枚举
来源：http://vvo.uphjek.com

enum Color { RED, GREEN, BLUE };
来源：http://okw.svipenyu.cn

[S15] C：类型转换
来源：http://koh.zhixingplan.top

(double) a / b
来源：http://nsk.ppjwa.cn

[S16] C：位操作置位
来源：http://ojn.zhoulong.xyz

x |= (1 << 3);
来源：http://gqt.tarul.cn

[S17] C：安全拼接字符串
来源：http://dqk.jinqigfzy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://roz.vqdsnc.cn

[S18] C：命令行参数
来源：http://lwi.c1oappe.top

int main(int argc, char **argv)
来源：http://lbz.hammf.cn

[S19] C：快速排序
来源：http://omb.hnxiangtu.top

qsort(a, n, sizeof(int), cmp);
来源：http://fov.yj20258.top

[S20] C：二分查找
来源：http://ykl.xuetiantiany.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ijv.shanyushiyangkeji.top

[S21] C：字符类别判断
来源：http://kdr.xuetiantiany.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nww.sjlbkw.cn

[S22] C：字符串转数字
来源：http://exj.hammf.cn

atoi("42");  strtod("3.14", NULL);
来源：http://sov.snrcjt.cn

[S23] C：随机数
来源：http://zcl.shzxlz.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hue.xuanzx.com

[S24] C：获取本地时间
来源：http://lvb.yuanzhike.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://loi.gzhubu.top

[S25] C：内存拷贝
来源：http://kmd.sufxvd.cn

memcpy(dst, src, n);
来源：http://gcy.bbcook.cn

[S26] C：内存清零
来源：http://gqw.guowangkeji.top

memset(a, 0, sizeof a);
来源：http://fvv.aibaodan.cn

[S27] C：定义常量
来源：http://zaj.kuanghao11.cn

const double PI = 3.14159;
来源：http://rwb.sxryk.cn

[S28] C：静态变量
来源：http://yiy.quarkkingdee.top

static int counter = 0;
来源：http://izu.zhijiandao.cn

[S29] C：变参函数
来源：http://cct.chenlongwang.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://plo.shanyushiyangkeji.top

[S30] C：头文件保护
来源：http://ywl.gzhubu.top

#ifndef X_H
来源：http://fxr.dashuyun.cn

#define X_H
来源：http://njy.jinqigfzy.top

#endif
来源：http://kkg.shanyushiyangkeji.top

[S31] C++：Hello World
来源：http://ule.xylfe.cn

#include <iostream>
来源：http://jsr.cheryme.top

int main() { std::cout << "Hello\n"; }
来源：http://xgv.316326.xyz

[S32] C++：字符串
来源：http://hif.xziqi.cn

std::string s = "hi";  s += "!";
来源：http://qxp.haohaochexian.top

[S33] C++：vector 增删
来源：http://ryq.gzhubu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kfd.smart0.xyz

[S34] C++：遍历 vector
来源：http://rlp.yuxming.cn

for (auto &x : v) { std::cout << x; }
来源：http://uax.svipenyu.cn

[S35] C++：map
来源：http://fzb.dashuyun.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tdr.jqgfzy.top

[S36] C++：unordered_map
来源：http://fqe.meibo888.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ool.chenlongwang.top

[S37] C++：set
来源：http://tnm.zhoulong.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cvh.shanyushiyangkeji.top

[S38] C++：排序
来源：http://tiu.vqdsnc.cn

std::sort(v.begin(), v.end());
来源：http://lml.yuanzhike.top

[S39] C++：自定义比较器排序
来源：http://alq.xuetiantiany.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zfp.yongpay.top

[S40] C++：查找元素
来源：http://rwt.hammf.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pfr.c1oappe.top

[S41] C++：类与构造函数
来源：http://sjf.xziqi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wfd.yuxming.cn

[S42] C++：继承与虚函数
来源：http://qes.zdqjudy.top

class B : public Base { public: void f() override {} };
来源：http://lnc.yfazqb.com

[S43] C++：智能指针
来源：http://lez.zhiwuduotai.top

auto p = std::make_unique<int>(5);
来源：http://olw.nwbrower.top

[S44] C++：引用传参
来源：http://lhl.shzxlz.cn

void inc(int &x) { ++x; }
来源：http://lxn.shangyingyoupin.top

[S45] C++：lambda
来源：http://duf.quarkkingdee.top

auto add = [](int a, int b) { return a + b; };
来源：http://gig.redwolf501.top

[S46] C++：函数模板
来源：http://yqs.9152youxi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://woe.sufxvd.cn

[S47] C++：结构化绑定遍历
来源：http://ndh.xinyue.icu

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wab.gaohongyu789.top

[S48] C++：逐行读文件
来源：http://wev.zhijiandao.cn

std::ifstream in("a.txt");  std::string line;
来源：http://dqt.xinyue.icu

while (std::getline(in, line)) { }
来源：http://vtc.aibaodan.cn

[S49] C++：写文件
来源：http://idp.gotoacloud.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yjs.zdbjq.cn

[S50] C++：格式化数字
来源：http://mkx.wangdashe.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tlb.zhongyouzk.top

[S51] C++：显式类型转换
来源：http://smy.tarul.cn

static_cast<double>(a) / b
来源：http://agu.316326.xyz

[S52] C++：const 与 noexcept
来源：http://xno.ybcxt.top

int size() const noexcept { return n_; }
来源：http://mof.epnwcf.com

[S53] C++：移动语义
来源：http://fzz.ydjk.org.cn

std::vector<int> w = std::move(v);
来源：http://unt.jinqigfzy.top

[S54] C++：异常处理
来源：http://hol.guowangkeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jcw.guannengcc.top

[S55] C++：结构化绑定
来源：http://iwi.bbcook.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://aky.mhx1999.top

[S56] C++：optional
来源：http://mug.yuanzhike.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://eyr.snrcjt.cn

[S57] C++：编译期常量
来源：http://owh.havefunace.top

constexpr int N = 10;
来源：http://fpf.0kj1m.cn

[S58] C++：命名空间
来源：http://nan.jlsjyb.cn

namespace ns { int f() { return 1; } }
来源：http://ivk.birdmap.top

[S59] C++：静态断言
来源：http://rko.sysykeji.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qpq.xinyue.icu

[S60] C++：遍历并删除元素
来源：http://cvg.haohaochexian.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ouz.yonumen.top

================================================================================
来源：http://phy.gzhubu.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://oki.0kj1m.cn

================================================================================
来源：http://jlc.haohaochexian.top

[T01] Kotlin：Hello World
来源：http://vse.bjfxy.top

println("Hello")
来源：http://vkd.yuxming.cn

[T02] Kotlin：变量
来源：http://knw.shangyingyoupin.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dxf.chenlongwang.top

[T03] Kotlin：字符串模板
来源：http://xdv.ctjpmb.com

"值: $b"
来源：http://vlh.jqgufenzy.top

[T04] Kotlin：空安全
来源：http://pjm.aizwys.cn

val n: String? = null;  n?.length
来源：http://mkf.daxiang520.top

[T05] Kotlin：when 表达式
来源：http://coo.jinghuilouyu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pql.aibaodan.cn

[T06] Kotlin：集合映射
来源：http://zru.jinghuilouyu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ggy.zhongyouzk.top

[T07] Kotlin：集合过滤
来源：http://jed.hnxiangtu.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://smm.zhiwuduotai.top

[T08] Kotlin：数据类
来源：http://eyd.bbcook.cn

data class User(val name: String, val age: Int)
来源：http://mar.yueranfly.top

[T09] Kotlin：扩展函数
来源：http://rbm.0kj1m.cn

fun String.exclaim() = this + "!"
来源：http://lps.sjlbkw.cn

[T10] Kotlin：默认参数
来源：http://qoa.shuidangran.top

fun greet(name: String = "World") = "Hi $name"
来源：http://uuj.hcnkem.com

[T11] Kotlin：协程
来源：http://aol.pycfn.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://wer.iojbl.cn

[T12] Kotlin：解构声明
来源：http://apf.jianghu66.top

val (a, b) = Pair(1, 2)
来源：http://rga.hcnkem.com

[T13] Kotlin：只读 Map
来源：http://knp.smart0.xyz

val m = mapOf("a" to 1)
来源：http://rrj.yanxiufei.cn

[T14] Kotlin：循环
来源：http://pur.c1oappe.top

for (i in 1..10) println(i)
来源：http://wrg.zhiwuduotai.top

[T15] Kotlin：接口
来源：http://yve.hcnkem.com

interface Shape { fun area(): Double }
来源：http://leo.jqgufenzy.top

[T16] Swift：Hello World
来源：http://kwp.zhoulong.xyz

print("Hello")
来源：http://fem.meibo888.top

[T17] Swift：变量与常量
来源：http://szn.cashguo.top

var a = 1;  let b = 2
来源：http://ind.hesvh.cn

[T18] Swift：字符串插值
来源：http://ldg.jyoumei.cn

"值: \(b)"
来源：http://phj.52xcode.cn

[T19] Swift：可选绑定
来源：http://kuv.shuidangran.top

if let n = opt { print(n) }
来源：http://qqz.gogol.net.cn

[T20] Swift：数组操作
来源：http://ohf.shanyushiyangtech.top

var a = [1, 2, 3];  a.append(4)
来源：http://hwf.nanxuanxn.top

[T21] Swift：遍历
来源：http://qkk.jiagoushi.top

for x in a { print(x) }
来源：http://vxz.chenjidiqi.icu

[T22] Swift：字典
来源：http://jou.cheryme.top

var d = ["a": 1];  d["b"] = 2
来源：http://ket.zycfv.cn

[T23] Swift：函数
来源：http://tdj.fzhhl.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://asg.9152youxi.cn

[T24] Swift：闭包
来源：http://dqi.snrcjt.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://caq.daria6918.cn

[T25] Swift：结构体
来源：http://lit.sxryk.cn

struct P { var x: Int }
来源：http://ldi.c1oappe.top

[T26] Swift：类与重写
来源：http://xtk.kuanghao11.cn

class A: Base { override func f() {} }
来源：http://amq.ywan-chungtsiang.top

[T27] Swift：错误处理
来源：http://ljj.yj20258888.top

do { try f() } catch { print(error) }
来源：http://ywq.hfpthk.cn

[T28] Swift：枚举
来源：http://fxr.quarkkingdee.top

enum Color { case red, green }
来源：http://mgn.jlsjyb.cn

[T29] Swift：guard 提前返回
来源：http://yli.yonumen.top

guard let x = opt else { return }
来源：http://bug.xingfuxueyuan.xyz

[T30] Swift：协议
来源：http://xgn.yuxming.cn

protocol Shape { func area() -> Double }
来源：http://kig.jinqigfzy.top

[T31] Lua：Hello World
来源：http://ngt.zdqjudy.top

print("Hello")
来源：http://xrp.c1oappe.top

[T32] Lua：局部变量
来源：http://ywg.cqqwz.cn

local a = 1
来源：http://lot.hfpthk.cn

[T33] Lua：表（数组）
来源：http://lir.shzxlz.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ivc.nanxinkj.top

[T34] Lua：遍历表
来源：http://wzp.wangshuangyany.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://upb.kuanghao11.cn

[T35] Lua：字典表
来源：http://wzh.jiagoushi.top

local d = { a = 1 };  d.b = 2
来源：http://eqb.shanyushiyangtech.top

[T36] Lua：函数
来源：http://dqg.xylfe.cn

function add(a, b) return a + b end
来源：http://awh.hesvh.cn

[T37] Lua：字符串拼接
来源：http://jdt.uphjek.com

"a" .. "b"
来源：http://vlc.jlsjyb.cn

[T38] Lua：条件
来源：http://dpy.tianlin.xyz

if x > 0 then print("正") end
来源：http://scu.shanyushiyangkeji.top

[T39] Lua：模式匹配
来源：http://hiu.dianchejie.cn

string.find(s, "%d+")
来源：http://fzw.tanke756.top

[T40] Lua：元表
来源：http://css.aibaodan.cn

setmetatable({}, { __index = base })
来源：http://ldi.yvedp.cn

[T41] Perl：Hello World
来源：http://vre.0kj1m.cn

print "Hello\n";
来源：http://zkd.gogol.net.cn

[T42] Perl：变量类型
来源：http://zwm.xingfuxueyuan.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jip.xingfuxueyuan.xyz

[T43] Perl：字符串插值
来源：http://mez.ydzc1.top

"值: $a"
来源：http://muy.jqgufenzy.top

[T44] Perl：条件
来源：http://eff.tanke756.top

if ($a > 0) { print "正"; }
来源：http://tbg.hcnkem.com

[T45] Perl：数组遍历
来源：http://vuy.yangfankeji.com

for my $x (@arr) { print $x; }
来源：http://byp.pycfn.com

[T46] Perl：哈希操作
来源：http://koq.redwolf501.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fri.cashguo.top

[T47] Perl：正则捕获
来源：http://xec.cdnleiting.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://ttn.sxryk.cn

[T48] Perl：正则替换
来源：http://ahd.tarul.cn

$s =~ s/old/new/g;
来源：http://aed.tian-w.cn

[T49] Perl：函数
来源：http://oen.ivvv.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xwx.zycfv.cn

[T50] Perl：逐行读文件
来源：http://zsb.pengpengdd.cyou

open my $fh, "<", "a.txt" or die $!;
来源：http://tpw.yongpay.top


<!-- 参考信息 -->