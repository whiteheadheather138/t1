代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://llj.bbcook.cn

[R48] awk 取指定列
来源：http://wqe.tian-w.cn

awk '{print $1, $3}' a.txt
来源：http://deb.smart0.xyz

[R49] awk 带条件
来源：http://bwi.0kj1m.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yuh.shuidangran.top

[R50] awk 求和
来源：http://muv.zdqjudy.top

awk '{s += $2} END {print s}' a.txt
来源：http://jzt.yfazqb.com

[R51] 排序去重取前几
来源：http://rgg.dashuyun.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://tee.dianchejie.cn

[R52] 统计行数
来源：http://zah.yongpay.top

wc -l a.txt
来源：http://mtd.chenzaomai.com

[R53] 查看文件头与实时尾
来源：http://krw.ivvv.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qjq.ivvv.top

[R54] 比较两个文件
来源：http://uin.jyoumei.cn

diff a.txt b.txt
来源：http://uss.smart0.xyz

[R55] 压缩与解压
来源：http://lsh.havefunace.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dva.zhongyouzk.top

[R56] 远程拷贝
来源：http://yls.fanxiaobao.xyz

scp file user@host:/path/
来源：http://jlb.yuanzhike.top

[R57] 远程执行命令
来源：http://lql.fengsongda.top

ssh user@host 'uptime'
来源：http://pif.cqqwz.cn

[R58] 下载文件
来源：http://rpi.shanyushiyangkeji.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://unx.9152youxi.cn

[R59] 发 POST JSON
来源：http://rbm.pengpengdd.cyou

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ptf.jqgfzy.top

[R60] 只看 HTTP 状态码
来源：http://akb.zdqjudy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wzx.gogol.net.cn

[R61] 磁盘占用
来源：http://adg.ppjwa.cn

df -h;  du -sh *
来源：http://tla.0kj1m.cn

[R62] 找最占空间的文件
来源：http://vmr.hnxiangtu.top

du -ah . | sort -rh | head -10
来源：http://vei.yonumen.top

[R63] 内存与进程
来源：http://fro.yj20258888.top

free -h;  ps aux | grep nginx
来源：http://bug.iojbl.cn

[R64] 结束进程
来源：http://bom.hysaishi.cn

kill -9 $(pgrep -f app.py)
来源：http://gym.bjfxy.top

[R65] 查看端口占用
来源：http://chd.yonumen.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ney.sxryk.cn

[R66] 定时任务
来源：http://pgs.dashuyun.cn

crontab -e;  crontab -l
来源：http://pgo.epnwcf.com

[R67] 生成随机十六进制串
来源：http://aig.yuanzhike.top

openssl rand -hex 16
来源：http://ivj.0kj1m.cn

[R68] 计算文件校验值
来源：http://stc.xinyue.icu

sha256sum a.txt;  md5sum a.txt
来源：http://mrc.c1oappe.top

[R69] 生成随机密码
来源：http://khf.jinqigufen.top

head -c 16 /dev/urandom | base64
来源：http://hoe.svipenyu.cn

[R70] 时间戳与互转
来源：http://fyo.hcnkem.com

date +%s;  date -d @1700000000
来源：http://pmx.ybcxt.top

[R71] 日期格式化
来源：http://iat.xziqi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://vrf.hammf.cn

[R72] 等待端口就绪
来源：http://gga.bjfxy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ncj.ydzc1.top

[R73] 分割大日志
来源：http://wly.yuxming.cn

split -l 1000 big.log part_
来源：http://pca.sxryk.cn

[R74] 批量重命名
来源：http://del.guowangkeji.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fzf.ybcxt.top

[R75] 导出环境变量
来源：http://fqe.c1oappe.top

export PATH="$HOME/bin:$PATH"
来源：http://vnk.9152youxi.cn

[R76] 使用临时文件
来源：http://qab.meibo888.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://eaj.xuanzx.com

[R77] 读取用户输入
来源：http://six.52xcode.cn

read -rp "请输入: " ans
来源：http://hkp.wangdashe.top

[R78] 交互式菜单
来源：http://kxu.yuxming.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://sfq.xylfe.cn

[R79] 解析命令行选项
来源：http://ela.nwbrower.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wdx.yuxming.cn

[R80] 查看脚本执行耗时
来源：http://noy.bjfxy.top

time ./run.sh
来源：http://pbp.sysykeji.top

================================================================================
来源：http://rzg.yj20258888.top

S. C / C++ 专题
来源：http://qjs.tanke756.top

================================================================================
来源：http://rem.aibaodan.cn

[S01] C：Hello World
来源：http://tlv.svipenyu.cn

#include <stdio.h>
来源：http://cis.hfpthk.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hge.yueranfly.top

[S02] C：变量与格式化输出
来源：http://vqn.meibo888.top

int a = 10; printf("%d\n", a);
来源：http://ryj.jinghuilouyu.cn

[S03] C：读入整数
来源：http://xiv.epnwcf.com

int x; scanf("%d", &x);
来源：http://wlx.ehwqpu.com

[S04] C：字符串复制
来源：http://eaj.tian-w.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rhj.ppjwa.cn

[S05] C：字符串长度
来源：http://eve.sjlbkw.cn

strlen(s)
来源：http://ajc.jyoumei.cn

[S06] C：字符串比较
来源：http://cze.shanyushiyangtech.top

strcmp(a, b) == 0
来源：http://rae.gogol.net.cn

[S07] C：数组遍历求和
来源：http://eld.hnqzz.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zbj.guannengcc.top

[S08] C：动态内存分配与释放
来源：http://ocy.hysaishi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tod.ybcxt.top

[S09] C：结构体定义与初始化
来源：http://ykq.tianlin.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xbo.zhengqikj.top

[S10] C：指针与解引用
来源：http://yjn.jqgfzy.top

int *p = &a;  *p = 5;
来源：http://ywt.guannengcc.top

[S11] C：逐行读文件
来源：http://nhe.fzhhl.top

FILE *f = fopen("a.txt", "r");
来源：http://btr.wangdashe.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://fua.yonumen.top

fclose(f);
来源：http://lde.hammf.cn

[S12] C：写文件
来源：http://jse.0kj1m.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hyj.jyoumei.cn

[S13] C：宏定义
来源：http://pgr.jlsjyb.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gqn.shangyingyoupin.top

[S14] C：枚举
来源：http://nhk.jqgufenzy.top

enum Color { RED, GREEN, BLUE };
来源：http://mzg.0kj1m.cn

[S15] C：类型转换
来源：http://spv.cucudq.cn

(double) a / b
来源：http://mgl.jyoumei.cn

[S16] C：位操作置位
来源：http://qls.feifeiyinyue.top

x |= (1 << 3);
来源：http://cdw.fktsv.cn

[S17] C：安全拼接字符串
来源：http://iwl.haohaochexian.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ipc.c1oappe.top

[S18] C：命令行参数
来源：http://wsj.chenzaomai.com

int main(int argc, char **argv)
来源：http://nfx.bbcook.cn

[S19] C：快速排序
来源：http://rqk.zhixingplan.top

qsort(a, n, sizeof(int), cmp);
来源：http://pan.jianghu66.top

[S20] C：二分查找
来源：http://ltg.sjlbkw.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ptt.bbcook.cn

[S21] C：字符类别判断
来源：http://osu.zhaomingkeji.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ghp.zhijiandao.cn

[S22] C：字符串转数字
来源：http://eev.zhixingplan.top

atoi("42");  strtod("3.14", NULL);
来源：http://ztn.epnwcf.com

[S23] C：随机数
来源：http://run.yanxiufei.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://yqg.ybcxt.top

[S24] C：获取本地时间
来源：http://yfb.xuanzx.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nmp.yanxiufei.cn

[S25] C：内存拷贝
来源：http://yhq.ivvv.top

memcpy(dst, src, n);
来源：http://eum.yj20258888.top

[S26] C：内存清零
来源：http://kjx.zdbjq.cn

memset(a, 0, sizeof a);
来源：http://vti.yfazqb.com

[S27] C：定义常量
来源：http://ixw.cdnleiting.top

const double PI = 3.14159;
来源：http://itr.sweek.top

[S28] C：静态变量
来源：http://gjo.iojbl.cn

static int counter = 0;
来源：http://sag.wangdashe.top

[S29] C：变参函数
来源：http://qmg.sjlbkw.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mbc.c1oappe.top

[S30] C：头文件保护
来源：http://ysm.0kj1m.cn

#ifndef X_H
来源：http://njz.feifeiyinyue.top

#define X_H
来源：http://pvm.jinghuilouyu.cn

#endif
来源：http://wqa.tarul.cn

[S31] C++：Hello World
来源：http://pky.hnxiangtu.top

#include <iostream>
来源：http://zky.ywan-chungtsiang.top

int main() { std::cout << "Hello\n"; }
来源：http://xkk.iojbl.cn

[S32] C++：字符串
来源：http://pwt.hongshengwenyu.top

std::string s = "hi";  s += "!";
来源：http://qps.xylfe.cn

[S33] C++：vector 增删
来源：http://ytp.gaohongyu789.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://aqw.xinyue.icu

[S34] C++：遍历 vector
来源：http://snf.zycfv.cn

for (auto &x : v) { std::cout << x; }
来源：http://fan.c1oappe.top

[S35] C++：map
来源：http://tic.birdmap.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://opb.yangfankeji.com

[S36] C++：unordered_map
来源：http://rsh.jinghuilouyu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://han.hcnkem.com

[S37] C++：set
来源：http://hei.ivvv.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vuk.iojbl.cn

[S38] C++：排序
来源：http://muf.yuxming.cn

std::sort(v.begin(), v.end());
来源：http://mdo.xinyue.icu

[S39] C++：自定义比较器排序
来源：http://cwz.ybcxt.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bih.guannengcc.top

[S40] C++：查找元素
来源：http://rlo.kuanghao11.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://puk.guowangkeji.top

[S41] C++：类与构造函数
来源：http://avc.ydjk.org.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tej.chenlongwang.top

[S42] C++：继承与虚函数
来源：http://tmv.yangfankeji.com

class B : public Base { public: void f() override {} };
来源：http://kmh.nanxinkj.top

[S43] C++：智能指针
来源：http://nrt.jinghuilouyu.cn

auto p = std::make_unique<int>(5);
来源：http://peq.uphjek.com

[S44] C++：引用传参
来源：http://bow.aibaodan.cn

void inc(int &x) { ++x; }
来源：http://xih.zhoulong.xyz

[S45] C++：lambda
来源：http://bja.bbcook.cn

auto add = [](int a, int b) { return a + b; };
来源：http://geg.jinqigufen.top

[S46] C++：函数模板
来源：http://fug.sxryk.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tdc.dashuyun.cn

[S47] C++：结构化绑定遍历
来源：http://vpf.jinghuilouyu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bmc.zhiwuduotai.top

[S48] C++：逐行读文件
来源：http://fdv.ydzc1.top

std::ifstream in("a.txt");  std::string line;
来源：http://rmb.hywenlv.cn

while (std::getline(in, line)) { }
来源：http://gmj.gaohongyu789.top

[S49] C++：写文件
来源：http://ocy.nanxinkj.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mrk.snrcjt.cn

[S50] C++：格式化数字
来源：http://wpw.tian-w.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tin.ctjpmb.com

[S51] C++：显式类型转换
来源：http://tfb.gogol.net.cn

static_cast<double>(a) / b
来源：http://ipy.vehdjk.com

[S52] C++：const 与 noexcept
来源：http://jlu.nanxinkj.top

int size() const noexcept { return n_; }
来源：http://cpl.chenjidiqi.icu

[S53] C++：移动语义
来源：http://axf.nwbrower.top

std::vector<int> w = std::move(v);
来源：http://cmj.316326.xyz

[S54] C++：异常处理
来源：http://mbc.gzhubu.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tnu.ppjwa.cn

[S55] C++：结构化绑定
来源：http://vxf.tanke756.top

auto [a, b] = std::make_pair(1, 2);
来源：http://nfw.guannengcc.top

[S56] C++：optional
来源：http://reg.shuidangran.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ejc.nanxuanxn.top

[S57] C++：编译期常量
来源：http://pwj.hnxiangtu.top

constexpr int N = 10;
来源：http://psl.hammf.cn

[S58] C++：命名空间
来源：http://uqe.vqdsnc.cn

namespace ns { int f() { return 1; } }
来源：http://qfl.hongshengwenyu.top

[S59] C++：静态断言
来源：http://kze.ydzc1.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gkf.fzhhl.top

[S60] C++：遍历并删除元素
来源：http://kfc.epnwcf.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vkd.tanke756.top

================================================================================
来源：http://blz.yonumen.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uib.sxryk.cn

================================================================================
来源：http://kxx.yueranfly.top

[T01] Kotlin：Hello World
来源：http://fcw.iojbl.cn

println("Hello")
来源：http://syz.bjfxy.top

[T02] Kotlin：变量
来源：http://pcj.bjfxy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rvg.0kj1m.cn

[T03] Kotlin：字符串模板
来源：http://bky.gaohongyu789.top

"值: $b"
来源：http://viu.tian-w.cn

[T04] Kotlin：空安全
来源：http://yvu.snrcjt.cn

val n: String? = null;  n?.length
来源：http://jkb.fanxiaobao.xyz

[T05] Kotlin：when 表达式
来源：http://ctx.xziqi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://eln.hnxiangtu.top

[T06] Kotlin：集合映射
来源：http://cfp.316326.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://rlf.guowangkeji.top

[T07] Kotlin：集合过滤
来源：http://skk.dashuyun.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://tuo.kuanghao11.cn

[T08] Kotlin：数据类
来源：http://cyl.daxiang520.top

data class User(val name: String, val age: Int)
来源：http://ktj.xinyue.icu

[T09] Kotlin：扩展函数
来源：http://pey.yfazqb.com

fun String.exclaim() = this + "!"
来源：http://zxy.dianchejie.cn

[T10] Kotlin：默认参数
来源：http://raq.hywenlv.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://syw.nanxuanxn.top

[T11] Kotlin：协程
来源：http://jny.hongshengwenyu.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://pjk.fktsv.cn

[T12] Kotlin：解构声明
来源：http://zbw.fktsv.cn

val (a, b) = Pair(1, 2)
来源：http://mxe.0kj1m.cn

[T13] Kotlin：只读 Map
来源：http://xyp.ydjk.org.cn

val m = mapOf("a" to 1)
来源：http://lni.yongpay.top

[T14] Kotlin：循环
来源：http://ovh.haohaochexian.top

for (i in 1..10) println(i)
来源：http://ldp.shuidangran.top

[T15] Kotlin：接口
来源：http://tpx.gotoacloud.top

interface Shape { fun area(): Double }
来源：http://inb.kuanghao11.cn

[T16] Swift：Hello World
来源：http://hhy.haohaochexian.top

print("Hello")
来源：http://zey.zdqjudy.top

[T17] Swift：变量与常量
来源：http://itx.daria6918.cn

var a = 1;  let b = 2
来源：http://crf.havefunace.top

[T18] Swift：字符串插值
来源：http://yxg.haohaochexian.top

"值: \(b)"
来源：http://jzm.9152youxi.cn

[T19] Swift：可选绑定
来源：http://qsp.jqgufenzy.top

if let n = opt { print(n) }
来源：http://off.jinqigufen.top

[T20] Swift：数组操作
来源：http://bts.yfazqb.com

var a = [1, 2, 3];  a.append(4)
来源：http://myl.xuanzx.com

[T21] Swift：遍历
来源：http://roz.zycfv.cn

for x in a { print(x) }
来源：http://qvt.fanxiaobao.xyz

[T22] Swift：字典
来源：http://drr.bbcook.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fya.fehbvm.com

[T23] Swift：函数
来源：http://fiy.aibaodan.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://spp.snrcjt.cn

[T24] Swift：闭包
来源：http://wpl.zhengqikj.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://iqd.uphjek.com

[T25] Swift：结构体
来源：http://njz.xylfe.cn

struct P { var x: Int }
来源：http://txy.sweek.top

[T26] Swift：类与重写
来源：http://pgv.hongshengwenyu.top

class A: Base { override func f() {} }
来源：http://xut.daxiang520.top

[T27] Swift：错误处理
来源：http://pfv.sweek.top

do { try f() } catch { print(error) }
来源：http://dpq.birdmap.top

[T28] Swift：枚举
来源：http://maz.yanxiufei.cn

enum Color { case red, green }
来源：http://egj.zhaomingkeji.xyz

[T29] Swift：guard 提前返回
来源：http://efs.kuanghao11.cn

guard let x = opt else { return }
来源：http://jln.ydjk.org.cn

[T30] Swift：协议
来源：http://yuh.ivvv.top

protocol Shape { func area() -> Double }
来源：http://pcl.cheryme.top

[T31] Lua：Hello World
来源：http://gmf.cheryme.top

print("Hello")
来源：http://xep.zhongyouzk.top

[T32] Lua：局部变量
来源：http://pek.guowangkeji.top

local a = 1
来源：http://xff.xuetiantiany.cn

[T33] Lua：表（数组）
来源：http://tgd.yj20258.top

local t = {1, 2, 3};  t[4] = 4
来源：http://qdw.shzxlz.cn

[T34] Lua：遍历表
来源：http://jjc.zycfv.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zsl.havefunace.top

[T35] Lua：字典表
来源：http://qfu.zdqjudy.top

local d = { a = 1 };  d.b = 2
来源：http://vsg.gogol.net.cn

[T36] Lua：函数
来源：http://glz.zhoulong.xyz

function add(a, b) return a + b end
来源：http://pdi.tarul.cn

[T37] Lua：字符串拼接
来源：http://zou.cucudq.cn

"a" .. "b"
来源：http://qdb.jqgfzy.top

[T38] Lua：条件
来源：http://djz.daria6918.cn

if x > 0 then print("正") end
来源：http://vcn.haohaochexian.top

[T39] Lua：模式匹配
来源：http://btp.quarkkingdee.top

string.find(s, "%d+")
来源：http://jku.fengsongda.top

[T40] Lua：元表
来源：http://egp.haohaochexian.top

setmetatable({}, { __index = base })
来源：http://ixn.tarul.cn

[T41] Perl：Hello World
来源：http://hgo.c1oappe.top

print "Hello\n";
来源：http://zyz.dianchejie.cn

[T42] Perl：变量类型
来源：http://zjz.hongshengwenyu.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ocz.cucudq.cn

[T43] Perl：字符串插值
来源：http://bny.haohaochexian.top

"值: $a"
来源：http://awy.yuanzhike.top

[T44] Perl：条件
来源：http://gdr.shuidangran.top

if ($a > 0) { print "正"; }
来源：http://cwf.cheryme.top

[T45] Perl：数组遍历
来源：http://xpd.9152youxi.cn

for my $x (@arr) { print $x; }
来源：http://xqc.cucudq.cn

[T46] Perl：哈希操作
来源：http://son.sweek.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jzd.sxryk.cn

[T47] Perl：正则捕获
来源：http://maa.zhixingplan.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://mbl.zhoulong.xyz

[T48] Perl：正则替换
来源：http://oui.cheryme.top

$s =~ s/old/new/g;
来源：http://yga.hywenlv.cn

[T49] Perl：函数
来源：http://wil.mhx1999.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kqh.sjlbkw.cn

[T50] Perl：逐行读文件
来源：http://cid.xuetiantiany.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://isj.9152youxi.cn


<!-- 参考信息 -->