代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://qqw.chenlongwang.top

[R48] awk 取指定列
来源：http://ben.vqdsnc.cn

awk '{print $1, $3}' a.txt
来源：http://itk.yanxiufei.cn

[R49] awk 带条件
来源：http://ofl.fktsv.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ley.ppjwa.cn

[R50] awk 求和
来源：http://ses.tianlin.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://gqp.316326.xyz

[R51] 排序去重取前几
来源：http://thk.ivvv.top

sort a.txt | uniq -c | sort -rn | head
来源：http://xfg.xinyue.icu

[R52] 统计行数
来源：http://vom.meibo888.top

wc -l a.txt
来源：http://msb.meibo888.top

[R53] 查看文件头与实时尾
来源：http://tjl.ydzc1.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uwv.nwbrower.top

[R54] 比较两个文件
来源：http://lho.xziqi.cn

diff a.txt b.txt
来源：http://rzz.cucudq.cn

[R55] 压缩与解压
来源：http://gmp.ppjwa.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://sfe.ppjwa.cn

[R56] 远程拷贝
来源：http://tpi.xuanzx.com

scp file user@host:/path/
来源：http://xyz.tarul.cn

[R57] 远程执行命令
来源：http://qvw.fehbvm.com

ssh user@host 'uptime'
来源：http://exd.jianghu66.top

[R58] 下载文件
来源：http://pxy.cashguo.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nfx.snrcjt.cn

[R59] 发 POST JSON
来源：http://mlc.feifeiyinyue.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ggl.pycfn.com

[R60] 只看 HTTP 状态码
来源：http://zyr.quarkkingdee.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://npb.gzhubu.top

[R61] 磁盘占用
来源：http://xmc.ydzc1.top

df -h;  du -sh *
来源：http://bdv.guowangkeji.top

[R62] 找最占空间的文件
来源：http://olv.zycfv.cn

du -ah . | sort -rh | head -10
来源：http://xcc.fzhhl.top

[R63] 内存与进程
来源：http://bam.ywan-chungtsiang.top

free -h;  ps aux | grep nginx
来源：http://ojg.jianghu66.top

[R64] 结束进程
来源：http://qgr.yanxiufei.cn

kill -9 $(pgrep -f app.py)
来源：http://faz.meibo888.top

[R65] 查看端口占用
来源：http://kus.jqgufenzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://swn.mhx1999.top

[R66] 定时任务
来源：http://rij.zhengqikj.top

crontab -e;  crontab -l
来源：http://hgj.ivvv.top

[R67] 生成随机十六进制串
来源：http://cmm.fengsongda.top

openssl rand -hex 16
来源：http://pem.hywenlv.cn

[R68] 计算文件校验值
来源：http://fuh.pengpengdd.cyou

sha256sum a.txt;  md5sum a.txt
来源：http://xkp.tarul.cn

[R69] 生成随机密码
来源：http://stp.ydzc1.top

head -c 16 /dev/urandom | base64
来源：http://ben.zhiwuduotai.top

[R70] 时间戳与互转
来源：http://bql.nanxinkj.top

date +%s;  date -d @1700000000
来源：http://fzk.jinyuanbaomall.cn

[R71] 日期格式化
来源：http://xie.fanxiaobao.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://ccy.jinqigfzy.top

[R72] 等待端口就绪
来源：http://fbl.yuanzhike.top

until nc -z localhost 3306; do sleep 1; done
来源：http://kbv.jlsjyb.cn

[R73] 分割大日志
来源：http://obr.quarkkingdee.top

split -l 1000 big.log part_
来源：http://dxu.xziqi.cn

[R74] 批量重命名
来源：http://gyt.zhongyouzk.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dzr.tian-w.cn

[R75] 导出环境变量
来源：http://ead.yanxiufei.cn

export PATH="$HOME/bin:$PATH"
来源：http://cho.0kj1m.cn

[R76] 使用临时文件
来源：http://vjj.zhongyouzk.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xrn.yj20258.top

[R77] 读取用户输入
来源：http://cvn.epnwcf.com

read -rp "请输入: " ans
来源：http://dwg.xziqi.cn

[R78] 交互式菜单
来源：http://jsh.ydzc1.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ehc.yj20258888.top

[R79] 解析命令行选项
来源：http://plp.ydzc1.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bsd.yanxiufei.cn

[R80] 查看脚本执行耗时
来源：http://ttq.cashguo.top

time ./run.sh
来源：http://soy.zhoulong.xyz

================================================================================
来源：http://ena.ivvv.top

S. C / C++ 专题
来源：http://fyl.jlsjyb.cn

================================================================================
来源：http://xxt.epnwcf.com

[S01] C：Hello World
来源：http://vam.jinyuanbaomall.cn

#include <stdio.h>
来源：http://mhv.jinqigufen.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ojl.smart0.xyz

[S02] C：变量与格式化输出
来源：http://wcn.yuanzhike.top

int a = 10; printf("%d\n", a);
来源：http://gtv.0kj1m.cn

[S03] C：读入整数
来源：http://dsa.zhongyouzk.top

int x; scanf("%d", &x);
来源：http://ekd.hongshengwenyu.top

[S04] C：字符串复制
来源：http://dog.havefunace.top

char dst[32]; strcpy(dst, "hi");
来源：http://zil.snrcjt.cn

[S05] C：字符串长度
来源：http://wef.vqdsnc.cn

strlen(s)
来源：http://fgu.9152youxi.cn

[S06] C：字符串比较
来源：http://iid.guannengcc.top

strcmp(a, b) == 0
来源：http://dvp.ydzc1.top

[S07] C：数组遍历求和
来源：http://brk.tianlin.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jvw.sufxvd.cn

[S08] C：动态内存分配与释放
来源：http://ybf.fzhhl.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kpq.guannengcc.top

[S09] C：结构体定义与初始化
来源：http://pqk.andypj.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ebt.jinghuilouyu.cn

[S10] C：指针与解引用
来源：http://ukw.daxiang520.top

int *p = &a;  *p = 5;
来源：http://bhs.yj20258888.top

[S11] C：逐行读文件
来源：http://lvc.yj20258888.top

FILE *f = fopen("a.txt", "r");
来源：http://wam.feifeiyinyue.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://qep.cucudq.cn

fclose(f);
来源：http://xtu.chenlongwang.top

[S12] C：写文件
来源：http://wfj.gotoacloud.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ksr.birdmap.top

[S13] C：宏定义
来源：http://xgg.zhaomingkeji.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mxc.xylfe.cn

[S14] C：枚举
来源：http://yil.andypj.xyz

enum Color { RED, GREEN, BLUE };
来源：http://wwv.c1oappe.top

[S15] C：类型转换
来源：http://xnd.sxryk.cn

(double) a / b
来源：http://oep.cqqwz.cn

[S16] C：位操作置位
来源：http://pvd.yanxiufei.cn

x |= (1 << 3);
来源：http://mbw.snrcjt.cn

[S17] C：安全拼接字符串
来源：http://pgm.hfpthk.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bfp.tianlin.xyz

[S18] C：命令行参数
来源：http://qfo.316326.xyz

int main(int argc, char **argv)
来源：http://kfl.smart0.xyz

[S19] C：快速排序
来源：http://fpl.jinqigfzy.top

qsort(a, n, sizeof(int), cmp);
来源：http://ign.chenlongwang.top

[S20] C：二分查找
来源：http://fps.daxiang520.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rtl.tian-w.cn

[S21] C：字符类别判断
来源：http://xzw.hesvh.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fkk.zdqjudy.top

[S22] C：字符串转数字
来源：http://kgp.yfazqb.com

atoi("42");  strtod("3.14", NULL);
来源：http://qmw.xuanzx.com

[S23] C：随机数
来源：http://fci.shanyushiyangtech.top

srand(time(NULL));  int r = rand() % 100;
来源：http://xlp.cqqwz.cn

[S24] C：获取本地时间
来源：http://kbt.xinyue.icu

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nxf.tarul.cn

[S25] C：内存拷贝
来源：http://puw.yuanzhike.top

memcpy(dst, src, n);
来源：http://pzt.aizwys.cn

[S26] C：内存清零
来源：http://xkz.vehdjk.com

memset(a, 0, sizeof a);
来源：http://tfv.sweek.top

[S27] C：定义常量
来源：http://her.xuanzx.com

const double PI = 3.14159;
来源：http://czf.yanxiufei.cn

[S28] C：静态变量
来源：http://mob.wangdashe.top

static int counter = 0;
来源：http://vld.ybcxt.top

[S29] C：变参函数
来源：http://yfm.shangyingyoupin.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ars.wangdashe.top

[S30] C：头文件保护
来源：http://jla.shangyingyoupin.top

#ifndef X_H
来源：http://vqb.iojbl.cn

#define X_H
来源：http://iob.gaohongyu789.top

#endif
来源：http://qxm.jinghuilouyu.cn

[S31] C++：Hello World
来源：http://sxz.zhaomingkeji.xyz

#include <iostream>
来源：http://qsl.ivvv.top

int main() { std::cout << "Hello\n"; }
来源：http://kjp.wangshuangyany.cn

[S32] C++：字符串
来源：http://oxo.cucudq.cn

std::string s = "hi";  s += "!";
来源：http://gfz.yuanzhike.top

[S33] C++：vector 增删
来源：http://vgm.sjlbkw.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://usn.sysykeji.top

[S34] C++：遍历 vector
来源：http://mte.zhengqikj.top

for (auto &x : v) { std::cout << x; }
来源：http://uew.haohaochexian.top

[S35] C++：map
来源：http://mqy.ppjwa.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://avv.zhongyouzk.top

[S36] C++：unordered_map
来源：http://mcz.zhiwuduotai.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://svu.ctjpmb.com

[S37] C++：set
来源：http://zrx.guannengcc.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mzi.yueranfly.top

[S38] C++：排序
来源：http://maf.ydzc1.top

std::sort(v.begin(), v.end());
来源：http://ilc.bbcook.cn

[S39] C++：自定义比较器排序
来源：http://etn.sjlbkw.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://klt.xuanzx.com

[S40] C++：查找元素
来源：http://fnt.hnxiangtu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://frv.cdnleiting.top

[S41] C++：类与构造函数
来源：http://chn.chenzaomai.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ebr.tian-w.cn

[S42] C++：继承与虚函数
来源：http://hov.zdqjudy.top

class B : public Base { public: void f() override {} };
来源：http://csx.yfazqb.com

[S43] C++：智能指针
来源：http://aqe.guannengcc.top

auto p = std::make_unique<int>(5);
来源：http://uhb.zhoulong.xyz

[S44] C++：引用传参
来源：http://oxk.xylfe.cn

void inc(int &x) { ++x; }
来源：http://lqs.wangdashe.top

[S45] C++：lambda
来源：http://hch.wangdashe.top

auto add = [](int a, int b) { return a + b; };
来源：http://zps.gotoacloud.top

[S46] C++：函数模板
来源：http://hrp.yj20258888.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://brh.ehwqpu.com

[S47] C++：结构化绑定遍历
来源：http://maj.hfpthk.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ngp.epnwcf.com

[S48] C++：逐行读文件
来源：http://ega.aibaodan.cn

std::ifstream in("a.txt");  std::string line;
来源：http://umo.pycfn.com

while (std::getline(in, line)) { }
来源：http://csl.zhiwuduotai.top

[S49] C++：写文件
来源：http://yto.yueranfly.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ulv.ybcxt.top

[S50] C++：格式化数字
来源：http://oie.ybcxt.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dsj.hnqzz.top

[S51] C++：显式类型转换
来源：http://omk.c1oappe.top

static_cast<double>(a) / b
来源：http://rhz.sjlbkw.cn

[S52] C++：const 与 noexcept
来源：http://ugr.jinyuanbaomall.cn

int size() const noexcept { return n_; }
来源：http://xhq.yanxiufei.cn

[S53] C++：移动语义
来源：http://xze.guowangkeji.top

std::vector<int> w = std::move(v);
来源：http://ktv.kuanghao11.cn

[S54] C++：异常处理
来源：http://hnz.fehbvm.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wdz.shuidangran.top

[S55] C++：结构化绑定
来源：http://ube.dashuyun.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://tno.jinghuilouyu.cn

[S56] C++：optional
来源：http://seg.ehwqpu.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ewx.ehwqpu.com

[S57] C++：编译期常量
来源：http://yim.tarul.cn

constexpr int N = 10;
来源：http://ahl.xuanzx.com

[S58] C++：命名空间
来源：http://vyt.chenzaomai.com

namespace ns { int f() { return 1; } }
来源：http://ztg.yuxming.cn

[S59] C++：静态断言
来源：http://dst.snrcjt.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ouv.cucudq.cn

[S60] C++：遍历并删除元素
来源：http://mhb.aizwys.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dsq.ctjpmb.com

================================================================================
来源：http://tik.daxiang520.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xiz.yj20258.top

================================================================================
来源：http://vfl.xuetiantiany.cn

[T01] Kotlin：Hello World
来源：http://njx.zdbjq.cn

println("Hello")
来源：http://ahd.shangyingyoupin.top

[T02] Kotlin：变量
来源：http://dtl.zdbjq.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gij.hysaishi.cn

[T03] Kotlin：字符串模板
来源：http://iyy.tianlin.xyz

"值: $b"
来源：http://fym.tian-w.cn

[T04] Kotlin：空安全
来源：http://wod.feifeiyinyue.top

val n: String? = null;  n?.length
来源：http://ndu.zhengqikj.top

[T05] Kotlin：when 表达式
来源：http://pfp.ehwqpu.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tww.yvedp.cn

[T06] Kotlin：集合映射
来源：http://qui.nanxinkj.top

listOf(1, 2, 3).map { it * 2 }
来源：http://pnb.hysaishi.cn

[T07] Kotlin：集合过滤
来源：http://hkq.xinyue.icu

listOf(1, 2, 3).filter { it > 1 }
来源：http://vtb.hfpthk.cn

[T08] Kotlin：数据类
来源：http://ugj.fengsongda.top

data class User(val name: String, val age: Int)
来源：http://dtq.ydzc1.top

[T09] Kotlin：扩展函数
来源：http://hwg.snrcjt.cn

fun String.exclaim() = this + "!"
来源：http://gvf.birdmap.top

[T10] Kotlin：默认参数
来源：http://umy.sufxvd.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tnd.sxryk.cn

[T11] Kotlin：协程
来源：http://ywq.pengpengdd.cyou

GlobalScope.launch { delay(1000); println("done") }
来源：http://pey.ctjpmb.com

[T12] Kotlin：解构声明
来源：http://jop.svipenyu.cn

val (a, b) = Pair(1, 2)
来源：http://bws.c1oappe.top

[T13] Kotlin：只读 Map
来源：http://jfs.yuanzhike.top

val m = mapOf("a" to 1)
来源：http://hbj.epnwcf.com

[T14] Kotlin：循环
来源：http://zxc.jlsjyb.cn

for (i in 1..10) println(i)
来源：http://mzn.ywan-chungtsiang.top

[T15] Kotlin：接口
来源：http://qxh.0kj1m.cn

interface Shape { fun area(): Double }
来源：http://lby.shanyushiyangkeji.top

[T16] Swift：Hello World
来源：http://tpq.9152youxi.cn

print("Hello")
来源：http://tkj.daxiang520.top

[T17] Swift：变量与常量
来源：http://elq.zhoulong.xyz

var a = 1;  let b = 2
来源：http://vkz.tanke756.top

[T18] Swift：字符串插值
来源：http://zum.feifeiyinyue.top

"值: \(b)"
来源：http://qlj.yj20258888.top

[T19] Swift：可选绑定
来源：http://usm.hysaishi.cn

if let n = opt { print(n) }
来源：http://xbn.ybcxt.top

[T20] Swift：数组操作
来源：http://kcz.uphjek.com

var a = [1, 2, 3];  a.append(4)
来源：http://gku.yj20258888.top

[T21] Swift：遍历
来源：http://vfj.ppjwa.cn

for x in a { print(x) }
来源：http://gos.haohaochexian.top

[T22] Swift：字典
来源：http://acb.zycfv.cn

var d = ["a": 1];  d["b"] = 2
来源：http://yrx.hfpthk.cn

[T23] Swift：函数
来源：http://gry.yongpay.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cun.jinqigufen.top

[T24] Swift：闭包
来源：http://pev.fehbvm.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://enl.cucudq.cn

[T25] Swift：结构体
来源：http://djb.ydzc1.top

struct P { var x: Int }
来源：http://vek.tarul.cn

[T26] Swift：类与重写
来源：http://hvn.dashuyun.cn

class A: Base { override func f() {} }
来源：http://yat.aizwys.cn

[T27] Swift：错误处理
来源：http://ckm.smart0.xyz

do { try f() } catch { print(error) }
来源：http://osc.zhixingplan.top

[T28] Swift：枚举
来源：http://mpn.wangdashe.top

enum Color { case red, green }
来源：http://prx.shanyushiyangkeji.top

[T29] Swift：guard 提前返回
来源：http://vsi.guannengcc.top

guard let x = opt else { return }
来源：http://yrq.birdmap.top

[T30] Swift：协议
来源：http://krk.bbcook.cn

protocol Shape { func area() -> Double }
来源：http://cee.chenlongwang.top

[T31] Lua：Hello World
来源：http://sjo.yuanzhike.top

print("Hello")
来源：http://htt.fanxiaobao.xyz

[T32] Lua：局部变量
来源：http://pcw.gotoacloud.top

local a = 1
来源：http://ogu.52xcode.cn

[T33] Lua：表（数组）
来源：http://zwj.hywenlv.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://kgi.fzhhl.top

[T34] Lua：遍历表
来源：http://fta.jyoumei.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zro.hfpthk.cn

[T35] Lua：字典表
来源：http://zhp.cheryme.top

local d = { a = 1 };  d.b = 2
来源：http://tkx.ehwqpu.com

[T36] Lua：函数
来源：http://dxu.tanke756.top

function add(a, b) return a + b end
来源：http://vii.dashuyun.cn

[T37] Lua：字符串拼接
来源：http://fbo.hammf.cn

"a" .. "b"
来源：http://msv.cdnleiting.top

[T38] Lua：条件
来源：http://dee.fengsongda.top

if x > 0 then print("正") end
来源：http://coj.jianghu66.top

[T39] Lua：模式匹配
来源：http://plr.iojbl.cn

string.find(s, "%d+")
来源：http://dsm.tarul.cn

[T40] Lua：元表
来源：http://svu.snrcjt.cn

setmetatable({}, { __index = base })
来源：http://gja.hesvh.cn

[T41] Perl：Hello World
来源：http://jxd.kuanghao11.cn

print "Hello\n";
来源：http://fab.vqdsnc.cn

[T42] Perl：变量类型
来源：http://djn.jiagoushi.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wwz.cheryme.top

[T43] Perl：字符串插值
来源：http://ugy.9152youxi.cn

"值: $a"
来源：http://qqe.xylfe.cn

[T44] Perl：条件
来源：http://pvq.tarul.cn

if ($a > 0) { print "正"; }
来源：http://kjm.quarkkingdee.top

[T45] Perl：数组遍历
来源：http://dzw.xinyue.icu

for my $x (@arr) { print $x; }
来源：http://cmj.shzxlz.cn

[T46] Perl：哈希操作
来源：http://afi.shuidangran.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gsd.havefunace.top

[T47] Perl：正则捕获
来源：http://tkq.zycfv.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wae.shuidangran.top

[T48] Perl：正则替换
来源：http://bgw.daria6918.cn

$s =~ s/old/new/g;
来源：http://utv.jinqigfzy.top

[T49] Perl：函数
来源：http://gad.jinqigufen.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jky.sysykeji.top

[T50] Perl：逐行读文件
来源：http://sas.zhengqikj.top

open my $fh, "<", "a.txt" or die $!;
来源：http://rjk.guowangkeji.top


<!-- 参考信息 -->