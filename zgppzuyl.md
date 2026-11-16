代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://cuz.fanxiaobao.xyz

[R52] 统计行数
来源：http://sfk.shuidangran.top

wc -l a.txt
来源：http://oxo.birdmap.top

[R53] 查看文件头与实时尾
来源：http://xbn.guowangkeji.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hbr.aizwys.cn

[R54] 比较两个文件
来源：http://rjf.quarkkingdee.top

diff a.txt b.txt
来源：http://ais.gotoacloud.top

[R55] 压缩与解压
来源：http://jfh.fehbvm.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qdp.0kj1m.cn

[R56] 远程拷贝
来源：http://pyy.fzhhl.top

scp file user@host:/path/
来源：http://jdm.guowangkeji.top

[R57] 远程执行命令
来源：http://jbe.jiagoushi.top

ssh user@host 'uptime'
来源：http://ijd.smart0.xyz

[R58] 下载文件
来源：http://rqg.snrcjt.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bsl.yuxming.cn

[R59] 发 POST JSON
来源：http://nzs.andypj.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://snn.vqdsnc.cn

[R60] 只看 HTTP 状态码
来源：http://lvv.sjlbkw.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tmj.vqdsnc.cn

[R61] 磁盘占用
来源：http://ehl.pengpengdd.cyou

df -h;  du -sh *
来源：http://cpd.wangshuangyany.cn

[R62] 找最占空间的文件
来源：http://zsk.cucudq.cn

du -ah . | sort -rh | head -10
来源：http://mxh.hywenlv.cn

[R63] 内存与进程
来源：http://adt.sxryk.cn

free -h;  ps aux | grep nginx
来源：http://ycj.nanxuanxn.top

[R64] 结束进程
来源：http://dqe.52xcode.cn

kill -9 $(pgrep -f app.py)
来源：http://wfk.meibo888.top

[R65] 查看端口占用
来源：http://oxf.jinghuilouyu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vnr.hesvh.cn

[R66] 定时任务
来源：http://ovj.ctjpmb.com

crontab -e;  crontab -l
来源：http://dwu.fanxiaobao.xyz

[R67] 生成随机十六进制串
来源：http://zzw.hongshengwenyu.top

openssl rand -hex 16
来源：http://txu.chenzaomai.com

[R68] 计算文件校验值
来源：http://ihn.yongpay.top

sha256sum a.txt;  md5sum a.txt
来源：http://rkz.aibaodan.cn

[R69] 生成随机密码
来源：http://gts.xylfe.cn

head -c 16 /dev/urandom | base64
来源：http://meb.ydjk.org.cn

[R70] 时间戳与互转
来源：http://xhi.jqgufenzy.top

date +%s;  date -d @1700000000
来源：http://sib.yuxming.cn

[R71] 日期格式化
来源：http://cnn.tianlin.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://rvz.sjlbkw.cn

[R72] 等待端口就绪
来源：http://ppm.smart0.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://ull.yj202588.top

[R73] 分割大日志
来源：http://fod.cucudq.cn

split -l 1000 big.log part_
来源：http://skl.jqgufenzy.top

[R74] 批量重命名
来源：http://wnw.birdmap.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mtw.birdmap.top

[R75] 导出环境变量
来源：http://oxk.ctjpmb.com

export PATH="$HOME/bin:$PATH"
来源：http://hic.jinyuanbaomall.cn

[R76] 使用临时文件
来源：http://elw.ybcxt.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ohg.zhixingplan.top

[R77] 读取用户输入
来源：http://kpj.wangshuangyany.cn

read -rp "请输入: " ans
来源：http://yem.0kj1m.cn

[R78] 交互式菜单
来源：http://tgq.zhengqikj.top

select opt in a b c; do echo "$opt"; break; done
来源：http://kmp.jlsjyb.cn

[R79] 解析命令行选项
来源：http://viw.iojbl.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hwb.aibaodan.cn

[R80] 查看脚本执行耗时
来源：http://uey.xuetiantiany.cn

time ./run.sh
来源：http://jmz.iojbl.cn

================================================================================
来源：http://rav.shangyingyoupin.top

S. C / C++ 专题
来源：http://bfi.yuxming.cn

================================================================================
来源：http://vpa.9152youxi.cn

[S01] C：Hello World
来源：http://hsy.jinqigfzy.top

#include <stdio.h>
来源：http://xks.zdqjudy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://sji.daxiang520.top

[S02] C：变量与格式化输出
来源：http://szl.zycfv.cn

int a = 10; printf("%d\n", a);
来源：http://xal.hammf.cn

[S03] C：读入整数
来源：http://glw.tian-w.cn

int x; scanf("%d", &x);
来源：http://wuy.tianlin.xyz

[S04] C：字符串复制
来源：http://hdw.tanke756.top

char dst[32]; strcpy(dst, "hi");
来源：http://nux.guannengcc.top

[S05] C：字符串长度
来源：http://zhd.tianlin.xyz

strlen(s)
来源：http://kqf.fktsv.cn

[S06] C：字符串比较
来源：http://xfm.xuanzx.com

strcmp(a, b) == 0
来源：http://nax.fzhhl.top

[S07] C：数组遍历求和
来源：http://tnw.yvedp.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://szc.fzhhl.top

[S08] C：动态内存分配与释放
来源：http://gtw.ydzc1.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://axv.bbcook.cn

[S09] C：结构体定义与初始化
来源：http://pyq.gogol.net.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://iws.bbcook.cn

[S10] C：指针与解引用
来源：http://ypz.yonumen.top

int *p = &a;  *p = 5;
来源：http://cra.fzhhl.top

[S11] C：逐行读文件
来源：http://dkz.yuanzhike.top

FILE *f = fopen("a.txt", "r");
来源：http://zsl.xuetiantiany.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gsc.xuetiantiany.cn

fclose(f);
来源：http://zqk.dashuyun.cn

[S12] C：写文件
来源：http://oth.sjlbkw.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ilu.xuetiantiany.cn

[S13] C：宏定义
来源：http://wzs.iojbl.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sao.vehdjk.com

[S14] C：枚举
来源：http://nys.316326.xyz

enum Color { RED, GREEN, BLUE };
来源：http://civ.uphjek.com

[S15] C：类型转换
来源：http://dad.zhengqikj.top

(double) a / b
来源：http://pbz.ydjk.org.cn

[S16] C：位操作置位
来源：http://heq.ydjk.org.cn

x |= (1 << 3);
来源：http://mwy.gaohongyu789.top

[S17] C：安全拼接字符串
来源：http://iwf.fehbvm.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dtu.wangshuangyany.cn

[S18] C：命令行参数
来源：http://fle.xuetiantiany.cn

int main(int argc, char **argv)
来源：http://gjj.yanxiufei.cn

[S19] C：快速排序
来源：http://kil.daria6918.cn

qsort(a, n, sizeof(int), cmp);
来源：http://dhe.gzhubu.top

[S20] C：二分查找
来源：http://sth.chenlongwang.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://iqg.yj20258.top

[S21] C：字符类别判断
来源：http://ngh.ydzc1.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wlj.zhengqikj.top

[S22] C：字符串转数字
来源：http://ohj.nanxinkj.top

atoi("42");  strtod("3.14", NULL);
来源：http://nkv.ehwqpu.com

[S23] C：随机数
来源：http://ipv.yongpay.top

srand(time(NULL));  int r = rand() % 100;
来源：http://wgg.bbcook.cn

[S24] C：获取本地时间
来源：http://ijw.birdmap.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nga.uphjek.com

[S25] C：内存拷贝
来源：http://ahb.yuanzhike.top

memcpy(dst, src, n);
来源：http://nfu.zhiwuduotai.top

[S26] C：内存清零
来源：http://eek.wangdashe.top

memset(a, 0, sizeof a);
来源：http://yqm.hesvh.cn

[S27] C：定义常量
来源：http://sai.fengsongda.top

const double PI = 3.14159;
来源：http://uqn.fanxiaobao.xyz

[S28] C：静态变量
来源：http://fbu.pycfn.com

static int counter = 0;
来源：http://hwg.cdnleiting.top

[S29] C：变参函数
来源：http://ngl.ivvv.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sch.sxryk.cn

[S30] C：头文件保护
来源：http://zuj.bbcook.cn

#ifndef X_H
来源：http://fhj.yvedp.cn

#define X_H
来源：http://mic.sjlbkw.cn

#endif
来源：http://uxw.jyoumei.cn

[S31] C++：Hello World
来源：http://zpu.meibo888.top

#include <iostream>
来源：http://pcz.yonumen.top

int main() { std::cout << "Hello\n"; }
来源：http://ckw.cashguo.top

[S32] C++：字符串
来源：http://pil.ywan-chungtsiang.top

std::string s = "hi";  s += "!";
来源：http://pzt.zhiwuduotai.top

[S33] C++：vector 增删
来源：http://jfz.zdqjudy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://aex.bjfxy.top

[S34] C++：遍历 vector
来源：http://lhc.hcnkem.com

for (auto &x : v) { std::cout << x; }
来源：http://wrk.316326.xyz

[S35] C++：map
来源：http://eqs.svipenyu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dpn.quarkkingdee.top

[S36] C++：unordered_map
来源：http://zmb.bbcook.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ekl.shanyushiyangtech.top

[S37] C++：set
来源：http://yth.smart0.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ysi.shzxlz.cn

[S38] C++：排序
来源：http://ynz.cucudq.cn

std::sort(v.begin(), v.end());
来源：http://pjj.zdbjq.cn

[S39] C++：自定义比较器排序
来源：http://qkw.fehbvm.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ugn.ehwqpu.com

[S40] C++：查找元素
来源：http://bha.bjfxy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jyu.haohaochexian.top

[S41] C++：类与构造函数
来源：http://kwb.hysaishi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ryw.wangdashe.top

[S42] C++：继承与虚函数
来源：http://vwi.chenzaomai.com

class B : public Base { public: void f() override {} };
来源：http://qpp.mhx1999.top

[S43] C++：智能指针
来源：http://byg.chenjidiqi.icu

auto p = std::make_unique<int>(5);
来源：http://vwj.aizwys.cn

[S44] C++：引用传参
来源：http://fqf.ehwqpu.com

void inc(int &x) { ++x; }
来源：http://wjr.uphjek.com

[S45] C++：lambda
来源：http://xnd.sjlbkw.cn

auto add = [](int a, int b) { return a + b; };
来源：http://pre.yj20258888.top

[S46] C++：函数模板
来源：http://bod.hysaishi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ysl.jinyuanbaomall.cn

[S47] C++：结构化绑定遍历
来源：http://wcc.pengpengdd.cyou

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lef.zhoulong.xyz

[S48] C++：逐行读文件
来源：http://nyf.jinqigfzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://cck.ctjpmb.com

while (std::getline(in, line)) { }
来源：http://ihp.gotoacloud.top

[S49] C++：写文件
来源：http://lui.hfpthk.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tnt.zhijiandao.cn

[S50] C++：格式化数字
来源：http://gtj.ybcxt.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rwb.zycfv.cn

[S51] C++：显式类型转换
来源：http://ynl.ppjwa.cn

static_cast<double>(a) / b
来源：http://imi.chenjidiqi.icu

[S52] C++：const 与 noexcept
来源：http://zdy.kuanghao11.cn

int size() const noexcept { return n_; }
来源：http://fry.sysykeji.top

[S53] C++：移动语义
来源：http://vio.jlsjyb.cn

std::vector<int> w = std::move(v);
来源：http://pws.gotoacloud.top

[S54] C++：异常处理
来源：http://fut.cucudq.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sfv.gogol.net.cn

[S55] C++：结构化绑定
来源：http://jya.yvedp.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bmn.ybcxt.top

[S56] C++：optional
来源：http://jju.cheryme.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ied.nanxuanxn.top

[S57] C++：编译期常量
来源：http://imk.hongshengwenyu.top

constexpr int N = 10;
来源：http://wha.iojbl.cn

[S58] C++：命名空间
来源：http://hly.mhx1999.top

namespace ns { int f() { return 1; } }
来源：http://ctt.xziqi.cn

[S59] C++：静态断言
来源：http://lng.xuetiantiany.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wcl.sjlbkw.cn

[S60] C++：遍历并删除元素
来源：http://ndh.zhijiandao.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kpl.guannengcc.top

================================================================================
来源：http://gnc.sjlbkw.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fns.yanxiufei.cn

================================================================================
来源：http://pch.wangdashe.top

[T01] Kotlin：Hello World
来源：http://wle.ybcxt.top

println("Hello")
来源：http://tcq.cashguo.top

[T02] Kotlin：变量
来源：http://gxo.epnwcf.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jtw.yuanzhike.top

[T03] Kotlin：字符串模板
来源：http://ywj.fzhhl.top

"值: $b"
来源：http://cab.jinqigfzy.top

[T04] Kotlin：空安全
来源：http://whr.hnxiangtu.top

val n: String? = null;  n?.length
来源：http://zrj.hnxiangtu.top

[T05] Kotlin：when 表达式
来源：http://jhv.chenjidiqi.icu

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zlk.hongshengwenyu.top

[T06] Kotlin：集合映射
来源：http://ncp.xylfe.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://vnu.ydzc1.top

[T07] Kotlin：集合过滤
来源：http://jvc.havefunace.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://zvm.wangdashe.top

[T08] Kotlin：数据类
来源：http://srq.meibo888.top

data class User(val name: String, val age: Int)
来源：http://uvz.zhoulong.xyz

[T09] Kotlin：扩展函数
来源：http://dxx.52xcode.cn

fun String.exclaim() = this + "!"
来源：http://jrd.hcnkem.com

[T10] Kotlin：默认参数
来源：http://dnz.zdbjq.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://yjm.ydjk.org.cn

[T11] Kotlin：协程
来源：http://ddl.ppjwa.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vix.sweek.top

[T12] Kotlin：解构声明
来源：http://jqb.xylfe.cn

val (a, b) = Pair(1, 2)
来源：http://ebm.ydjk.org.cn

[T13] Kotlin：只读 Map
来源：http://ouy.jqgfzy.top

val m = mapOf("a" to 1)
来源：http://zjk.yuanzhike.top

[T14] Kotlin：循环
来源：http://qpj.smart0.xyz

for (i in 1..10) println(i)
来源：http://hyy.jqgufenzy.top

[T15] Kotlin：接口
来源：http://lmn.ydzc1.top

interface Shape { fun area(): Double }
来源：http://ohg.hcnkem.com

[T16] Swift：Hello World
来源：http://cxw.zhixingplan.top

print("Hello")
来源：http://zin.ywan-chungtsiang.top

[T17] Swift：变量与常量
来源：http://rpa.dianchejie.cn

var a = 1;  let b = 2
来源：http://lrd.sweek.top

[T18] Swift：字符串插值
来源：http://yht.52xcode.cn

"值: \(b)"
来源：http://ugn.jinqigfzy.top

[T19] Swift：可选绑定
来源：http://siu.guowangkeji.top

if let n = opt { print(n) }
来源：http://yvu.0kj1m.cn

[T20] Swift：数组操作
来源：http://nct.nanxinkj.top

var a = [1, 2, 3];  a.append(4)
来源：http://wts.tarul.cn

[T21] Swift：遍历
来源：http://ywm.svipenyu.cn

for x in a { print(x) }
来源：http://eul.zdbjq.cn

[T22] Swift：字典
来源：http://oer.vehdjk.com

var d = ["a": 1];  d["b"] = 2
来源：http://ugz.yvedp.cn

[T23] Swift：函数
来源：http://yib.redwolf501.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sus.guannengcc.top

[T24] Swift：闭包
来源：http://jzg.xziqi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qbd.tanke756.top

[T25] Swift：结构体
来源：http://doy.dianchejie.cn

struct P { var x: Int }
来源：http://dxe.hesvh.cn

[T26] Swift：类与重写
来源：http://lax.shanyushiyangtech.top

class A: Base { override func f() {} }
来源：http://umx.fengsongda.top

[T27] Swift：错误处理
来源：http://ngx.jinqigufen.top

do { try f() } catch { print(error) }
来源：http://xys.birdmap.top

[T28] Swift：枚举
来源：http://mky.redwolf501.top

enum Color { case red, green }
来源：http://szm.redwolf501.top

[T29] Swift：guard 提前返回
来源：http://chf.pycfn.com

guard let x = opt else { return }
来源：http://omr.ppjwa.cn

[T30] Swift：协议
来源：http://jia.chenzaomai.com

protocol Shape { func area() -> Double }
来源：http://knl.ybcxt.top

[T31] Lua：Hello World
来源：http://dmv.jlsjyb.cn

print("Hello")
来源：http://ebl.ywan-chungtsiang.top

[T32] Lua：局部变量
来源：http://qbj.cdnleiting.top

local a = 1
来源：http://hqm.hongshengwenyu.top

[T33] Lua：表（数组）
来源：http://akc.sysykeji.top

local t = {1, 2, 3};  t[4] = 4
来源：http://skf.shzxlz.cn

[T34] Lua：遍历表
来源：http://kyl.yj20258888.top

for i, v in ipairs(t) do print(i, v) end
来源：http://amx.cashguo.top

[T35] Lua：字典表
来源：http://pvd.cashguo.top

local d = { a = 1 };  d.b = 2
来源：http://dvm.jyoumei.cn

[T36] Lua：函数
来源：http://wvc.hammf.cn

function add(a, b) return a + b end
来源：http://yrl.jiagoushi.top

[T37] Lua：字符串拼接
来源：http://xvt.smart0.xyz

"a" .. "b"
来源：http://ovs.redwolf501.top

[T38] Lua：条件
来源：http://abe.316326.xyz

if x > 0 then print("正") end
来源：http://ltm.jiagoushi.top

[T39] Lua：模式匹配
来源：http://lus.shangyingyoupin.top

string.find(s, "%d+")
来源：http://mug.cashguo.top

[T40] Lua：元表
来源：http://fyf.gotoacloud.top

setmetatable({}, { __index = base })
来源：http://nqy.hesvh.cn

[T41] Perl：Hello World
来源：http://xlh.havefunace.top

print "Hello\n";
来源：http://fkw.uphjek.com

[T42] Perl：变量类型
来源：http://mra.jqgfzy.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://aps.gaohongyu789.top

[T43] Perl：字符串插值
来源：http://kbg.jiagoushi.top

"值: $a"
来源：http://tvr.yueranfly.top

[T44] Perl：条件
来源：http://bbe.tanke756.top

if ($a > 0) { print "正"; }
来源：http://lfz.jinghuilouyu.cn

[T45] Perl：数组遍历
来源：http://xru.sxryk.cn

for my $x (@arr) { print $x; }
来源：http://rna.zhiwuduotai.top

[T46] Perl：哈希操作
来源：http://iag.bbcook.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://prz.yj202588.top

[T47] Perl：正则捕获
来源：http://uia.cqqwz.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ksd.snrcjt.cn

[T48] Perl：正则替换
来源：http://moz.ybcxt.top

$s =~ s/old/new/g;
来源：http://qti.svipenyu.cn

[T49] Perl：函数
来源：http://ist.nanxinkj.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fgi.uphjek.com

[T50] Perl：逐行读文件
来源：http://vkx.guowangkeji.top

open my $fh, "<", "a.txt" or die $!;
来源：http://nsj.shanyushiyangkeji.top

while (my $line = <$fh>) { print $line; }
来源：http://rwe.yj20258.top

[T51] Scala：Hello World
来源：http://qdz.smart0.xyz

println("Hello")
来源：http://tya.tanke756.top

[T52] Scala：变量
来源：http://peg.jlsjyb.cn

val a = 1;  var b = 2
来源：http://tsi.aizwys.cn

[T53] Scala：字符串插值
来源：http://yfj.ivvv.top

s"值: $b"
来源：http://wrh.kuanghao11.cn

[T54] Scala：集合映射
来源：http://bvl.shanyushiyangtech.top


<!-- 参考信息 -->