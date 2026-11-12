代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://qxk.zhixingplan.top

[R52] 统计行数
来源：http://vji.smart0.xyz

wc -l a.txt
来源：http://ofb.mhx1999.top

[R53] 查看文件头与实时尾
来源：http://xrq.shangyingyoupin.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nsx.sxryk.cn

[R54] 比较两个文件
来源：http://grz.haohaochexian.top

diff a.txt b.txt
来源：http://wzv.cashguo.top

[R55] 压缩与解压
来源：http://vow.zhongyouzk.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qxu.fanxiaobao.xyz

[R56] 远程拷贝
来源：http://tra.shangyingyoupin.top

scp file user@host:/path/
来源：http://kue.snrcjt.cn

[R57] 远程执行命令
来源：http://wwy.jlsjyb.cn

ssh user@host 'uptime'
来源：http://jrt.sxryk.cn

[R58] 下载文件
来源：http://dif.hammf.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://adz.chenlongwang.top

[R59] 发 POST JSON
来源：http://asg.tanke756.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vwx.sjlbkw.cn

[R60] 只看 HTTP 状态码
来源：http://sgk.ivvv.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://asv.zdqjudy.top

[R61] 磁盘占用
来源：http://jny.ybcxt.top

df -h;  du -sh *
来源：http://tbc.hfpthk.cn

[R62] 找最占空间的文件
来源：http://wva.jqgfzy.top

du -ah . | sort -rh | head -10
来源：http://yuj.smart0.xyz

[R63] 内存与进程
来源：http://olu.tianlin.xyz

free -h;  ps aux | grep nginx
来源：http://lbm.jinghuilouyu.cn

[R64] 结束进程
来源：http://bct.shuidangran.top

kill -9 $(pgrep -f app.py)
来源：http://mpd.xinyue.icu

[R65] 查看端口占用
来源：http://rpb.yueranfly.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ndl.xuetiantiany.cn

[R66] 定时任务
来源：http://yjw.havefunace.top

crontab -e;  crontab -l
来源：http://qww.hcnkem.com

[R67] 生成随机十六进制串
来源：http://qbr.yvedp.cn

openssl rand -hex 16
来源：http://ljv.yuanzhike.top

[R68] 计算文件校验值
来源：http://rai.guowangkeji.top

sha256sum a.txt;  md5sum a.txt
来源：http://phj.yj20258888.top

[R69] 生成随机密码
来源：http://dzy.tanke756.top

head -c 16 /dev/urandom | base64
来源：http://lhj.hnxiangtu.top

[R70] 时间戳与互转
来源：http://eha.zycfv.cn

date +%s;  date -d @1700000000
来源：http://svu.xuetiantiany.cn

[R71] 日期格式化
来源：http://ubs.nanxuanxn.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://lqw.zycfv.cn

[R72] 等待端口就绪
来源：http://qgm.smart0.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://ksi.zhaomingkeji.xyz

[R73] 分割大日志
来源：http://kfp.xylfe.cn

split -l 1000 big.log part_
来源：http://scr.fengsongda.top

[R74] 批量重命名
来源：http://fyd.birdmap.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kul.sweek.top

[R75] 导出环境变量
来源：http://xqp.ppjwa.cn

export PATH="$HOME/bin:$PATH"
来源：http://mhi.cucudq.cn

[R76] 使用临时文件
来源：http://ium.jqgufenzy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sin.xinyue.icu

[R77] 读取用户输入
来源：http://igm.zhiwuduotai.top

read -rp "请输入: " ans
来源：http://evd.chenjidiqi.icu

[R78] 交互式菜单
来源：http://ijo.redwolf501.top

select opt in a b c; do echo "$opt"; break; done
来源：http://mjg.hongshengwenyu.top

[R79] 解析命令行选项
来源：http://fil.daxiang520.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dzo.sufxvd.cn

[R80] 查看脚本执行耗时
来源：http://ofg.jlsjyb.cn

time ./run.sh
来源：http://xfy.jinqigufen.top

================================================================================
来源：http://mph.yfazqb.com

S. C / C++ 专题
来源：http://tpx.smart0.xyz

================================================================================
来源：http://lse.sxryk.cn

[S01] C：Hello World
来源：http://tmn.ivvv.top

#include <stdio.h>
来源：http://uwv.yj20258888.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://fci.xziqi.cn

[S02] C：变量与格式化输出
来源：http://idx.zhijiandao.cn

int a = 10; printf("%d\n", a);
来源：http://mgr.cqqwz.cn

[S03] C：读入整数
来源：http://vlm.hcnkem.com

int x; scanf("%d", &x);
来源：http://lqd.haohaochexian.top

[S04] C：字符串复制
来源：http://zzj.shanyushiyangkeji.top

char dst[32]; strcpy(dst, "hi");
来源：http://eku.dashuyun.cn

[S05] C：字符串长度
来源：http://pfo.tarul.cn

strlen(s)
来源：http://xys.gotoacloud.top

[S06] C：字符串比较
来源：http://zcl.jyoumei.cn

strcmp(a, b) == 0
来源：http://cbq.xylfe.cn

[S07] C：数组遍历求和
来源：http://fnl.nwbrower.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dcx.sufxvd.cn

[S08] C：动态内存分配与释放
来源：http://qfi.zdqjudy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nhh.cqqwz.cn

[S09] C：结构体定义与初始化
来源：http://yhh.tarul.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hjd.ybcxt.top

[S10] C：指针与解引用
来源：http://nld.vqdsnc.cn

int *p = &a;  *p = 5;
来源：http://wat.ybcxt.top

[S11] C：逐行读文件
来源：http://krc.dashuyun.cn

FILE *f = fopen("a.txt", "r");
来源：http://oan.hnqzz.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://vnc.andypj.xyz

fclose(f);
来源：http://phg.0kj1m.cn

[S12] C：写文件
来源：http://doo.hnqzz.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rkl.shzxlz.cn

[S13] C：宏定义
来源：http://nvf.vqdsnc.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wyy.tanke756.top

[S14] C：枚举
来源：http://ylp.9152youxi.cn

enum Color { RED, GREEN, BLUE };
来源：http://iqi.daxiang520.top

[S15] C：类型转换
来源：http://vhz.dashuyun.cn

(double) a / b
来源：http://dud.fengsongda.top

[S16] C：位操作置位
来源：http://vnp.jinghuilouyu.cn

x |= (1 << 3);
来源：http://xok.52xcode.cn

[S17] C：安全拼接字符串
来源：http://pnu.cucudq.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zvq.ywan-chungtsiang.top

[S18] C：命令行参数
来源：http://bik.chenlongwang.top

int main(int argc, char **argv)
来源：http://kyx.shangyingyoupin.top

[S19] C：快速排序
来源：http://etz.bbcook.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rbg.shzxlz.cn

[S20] C：二分查找
来源：http://kvt.fanxiaobao.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ttu.zhixingplan.top

[S21] C：字符类别判断
来源：http://obw.ctjpmb.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vog.guowangkeji.top

[S22] C：字符串转数字
来源：http://hlk.dianchejie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://mub.gzhubu.top

[S23] C：随机数
来源：http://ltj.yanxiufei.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://uhc.xuanzx.com

[S24] C：获取本地时间
来源：http://vro.fzhhl.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vjl.tarul.cn

[S25] C：内存拷贝
来源：http://jiy.nwbrower.top

memcpy(dst, src, n);
来源：http://api.xingfuxueyuan.xyz

[S26] C：内存清零
来源：http://bgg.yj20258.top

memset(a, 0, sizeof a);
来源：http://neg.snrcjt.cn

[S27] C：定义常量
来源：http://ocd.kuanghao11.cn

const double PI = 3.14159;
来源：http://bvj.sufxvd.cn

[S28] C：静态变量
来源：http://jko.zhongyouzk.top

static int counter = 0;
来源：http://qqg.wangdashe.top

[S29] C：变参函数
来源：http://zdr.sxryk.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xyg.zhaomingkeji.xyz

[S30] C：头文件保护
来源：http://mwa.havefunace.top

#ifndef X_H
来源：http://yzt.zdbjq.cn

#define X_H
来源：http://ois.jiagoushi.top

#endif
来源：http://pdm.yvedp.cn

[S31] C++：Hello World
来源：http://ocr.xuanzx.com

#include <iostream>
来源：http://ekv.daria6918.cn

int main() { std::cout << "Hello\n"; }
来源：http://qrc.snrcjt.cn

[S32] C++：字符串
来源：http://lpj.quarkkingdee.top

std::string s = "hi";  s += "!";
来源：http://iuk.daxiang520.top

[S33] C++：vector 增删
来源：http://drg.epnwcf.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rnj.cqqwz.cn

[S34] C++：遍历 vector
来源：http://tba.fanxiaobao.xyz

for (auto &x : v) { std::cout << x; }
来源：http://swq.bbcook.cn

[S35] C++：map
来源：http://bsg.vqdsnc.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://foq.yfazqb.com

[S36] C++：unordered_map
来源：http://ede.shzxlz.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zht.kuanghao11.cn

[S37] C++：set
来源：http://rxy.dianchejie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://njo.snrcjt.cn

[S38] C++：排序
来源：http://mic.316326.xyz

std::sort(v.begin(), v.end());
来源：http://yqs.yj202588.top

[S39] C++：自定义比较器排序
来源：http://hgn.guannengcc.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nmz.jyoumei.cn

[S40] C++：查找元素
来源：http://whw.gaohongyu789.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lyf.yuxming.cn

[S41] C++：类与构造函数
来源：http://okl.nanxinkj.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hux.chenjidiqi.icu

[S42] C++：继承与虚函数
来源：http://yqz.yfazqb.com

class B : public Base { public: void f() override {} };
来源：http://mtt.gotoacloud.top

[S43] C++：智能指针
来源：http://jrz.jianghu66.top

auto p = std::make_unique<int>(5);
来源：http://xdb.tanke756.top

[S44] C++：引用传参
来源：http://ddt.aibaodan.cn

void inc(int &x) { ++x; }
来源：http://lyi.aizwys.cn

[S45] C++：lambda
来源：http://ifl.aibaodan.cn

auto add = [](int a, int b) { return a + b; };
来源：http://efy.yongpay.top

[S46] C++：函数模板
来源：http://lgg.cashguo.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://did.gotoacloud.top

[S47] C++：结构化绑定遍历
来源：http://mxt.guowangkeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wly.zhixingplan.top

[S48] C++：逐行读文件
来源：http://rqc.sysykeji.top

std::ifstream in("a.txt");  std::string line;
来源：http://duv.chenjidiqi.icu

while (std::getline(in, line)) { }
来源：http://cdb.zdbjq.cn

[S49] C++：写文件
来源：http://jbk.shanyushiyangtech.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://isz.meibo888.top

[S50] C++：格式化数字
来源：http://rbf.gogol.net.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fyt.haohaochexian.top

[S51] C++：显式类型转换
来源：http://csw.yanxiufei.cn

static_cast<double>(a) / b
来源：http://yyo.yfazqb.com

[S52] C++：const 与 noexcept
来源：http://znl.shanyushiyangtech.top

int size() const noexcept { return n_; }
来源：http://cdc.tanke756.top

[S53] C++：移动语义
来源：http://aqm.ctjpmb.com

std::vector<int> w = std::move(v);
来源：http://xnk.aizwys.cn

[S54] C++：异常处理
来源：http://wtj.zhijiandao.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ypc.yj202588.top

[S55] C++：结构化绑定
来源：http://cjm.hywenlv.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://anj.gaohongyu789.top

[S56] C++：optional
来源：http://kql.jqgufenzy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://iap.shuidangran.top

[S57] C++：编译期常量
来源：http://uet.yj20258888.top

constexpr int N = 10;
来源：http://ipx.tanke756.top

[S58] C++：命名空间
来源：http://gsn.yj20258888.top

namespace ns { int f() { return 1; } }
来源：http://bul.ybcxt.top

[S59] C++：静态断言
来源：http://hhc.shangyingyoupin.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ejb.nanxinkj.top

[S60] C++：遍历并删除元素
来源：http://mtp.zhijiandao.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://oxb.zhiwuduotai.top

================================================================================
来源：http://you.andypj.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://voj.xylfe.cn

================================================================================
来源：http://fvl.mhx1999.top

[T01] Kotlin：Hello World
来源：http://rjq.feifeiyinyue.top

println("Hello")
来源：http://edw.jianghu66.top

[T02] Kotlin：变量
来源：http://jok.nanxuanxn.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rov.sjlbkw.cn

[T03] Kotlin：字符串模板
来源：http://oep.ydzc1.top

"值: $b"
来源：http://wbl.hfpthk.cn

[T04] Kotlin：空安全
来源：http://sbt.zhoulong.xyz

val n: String? = null;  n?.length
来源：http://pgn.haohaochexian.top

[T05] Kotlin：when 表达式
来源：http://izx.hesvh.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://loz.iojbl.cn

[T06] Kotlin：集合映射
来源：http://soq.yj20258888.top

listOf(1, 2, 3).map { it * 2 }
来源：http://sdw.cucudq.cn

[T07] Kotlin：集合过滤
来源：http://tzj.daxiang520.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://pzx.shanyushiyangtech.top

[T08] Kotlin：数据类
来源：http://wsy.zhongyouzk.top

data class User(val name: String, val age: Int)
来源：http://slk.shanyushiyangtech.top

[T09] Kotlin：扩展函数
来源：http://dlq.yuanzhike.top

fun String.exclaim() = this + "!"
来源：http://bes.haohaochexian.top

[T10] Kotlin：默认参数
来源：http://fln.iojbl.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://kyv.guannengcc.top

[T11] Kotlin：协程
来源：http://vzk.xuetiantiany.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://puu.hnqzz.top

[T12] Kotlin：解构声明
来源：http://yxv.gaohongyu789.top

val (a, b) = Pair(1, 2)
来源：http://nzg.ydzc1.top

[T13] Kotlin：只读 Map
来源：http://qjo.jqgfzy.top

val m = mapOf("a" to 1)
来源：http://dyg.hammf.cn

[T14] Kotlin：循环
来源：http://ldr.jiagoushi.top

for (i in 1..10) println(i)
来源：http://iuv.zdbjq.cn

[T15] Kotlin：接口
来源：http://acc.birdmap.top

interface Shape { fun area(): Double }
来源：http://gvh.ywan-chungtsiang.top

[T16] Swift：Hello World
来源：http://uld.andypj.xyz

print("Hello")
来源：http://xpo.redwolf501.top

[T17] Swift：变量与常量
来源：http://kkk.nanxuanxn.top

var a = 1;  let b = 2
来源：http://rek.jinghuilouyu.cn

[T18] Swift：字符串插值
来源：http://icu.nwbrower.top

"值: \(b)"
来源：http://ayo.fktsv.cn

[T19] Swift：可选绑定
来源：http://dhd.vqdsnc.cn

if let n = opt { print(n) }
来源：http://siz.316326.xyz

[T20] Swift：数组操作
来源：http://oaf.ydzc1.top

var a = [1, 2, 3];  a.append(4)
来源：http://kfu.vqdsnc.cn

[T21] Swift：遍历
来源：http://ydb.epnwcf.com

for x in a { print(x) }
来源：http://mtf.meibo888.top

[T22] Swift：字典
来源：http://qky.shangyingyoupin.top

var d = ["a": 1];  d["b"] = 2
来源：http://grr.0kj1m.cn

[T23] Swift：函数
来源：http://wzy.fanxiaobao.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ucj.jinqigufen.top

[T24] Swift：闭包
来源：http://kdz.gzhubu.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://zxv.jianghu66.top

[T25] Swift：结构体
来源：http://liu.xingfuxueyuan.xyz

struct P { var x: Int }
来源：http://zkv.gotoacloud.top

[T26] Swift：类与重写
来源：http://nqk.ctjpmb.com

class A: Base { override func f() {} }
来源：http://ejd.yonumen.top

[T27] Swift：错误处理
来源：http://dgr.yfazqb.com

do { try f() } catch { print(error) }
来源：http://rsv.jianghu66.top

[T28] Swift：枚举
来源：http://fya.mhx1999.top

enum Color { case red, green }
来源：http://igi.xziqi.cn

[T29] Swift：guard 提前返回
来源：http://pqb.daxiang520.top

guard let x = opt else { return }
来源：http://tfp.0kj1m.cn

[T30] Swift：协议
来源：http://srl.hfpthk.cn

protocol Shape { func area() -> Double }
来源：http://hca.sxryk.cn

[T31] Lua：Hello World
来源：http://kpm.ctjpmb.com

print("Hello")
来源：http://djf.havefunace.top

[T32] Lua：局部变量
来源：http://qzm.fengsongda.top

local a = 1
来源：http://vmm.yuanzhike.top

[T33] Lua：表（数组）
来源：http://qtd.shuidangran.top

local t = {1, 2, 3};  t[4] = 4
来源：http://ypf.sjlbkw.cn

[T34] Lua：遍历表
来源：http://mqa.vqdsnc.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://whe.daria6918.cn

[T35] Lua：字典表
来源：http://gcz.hesvh.cn

local d = { a = 1 };  d.b = 2
来源：http://uqk.svipenyu.cn

[T36] Lua：函数
来源：http://giu.jinghuilouyu.cn

function add(a, b) return a + b end
来源：http://flj.jinqigufen.top

[T37] Lua：字符串拼接
来源：http://fgt.andypj.xyz

"a" .. "b"
来源：http://oqc.ctjpmb.com

[T38] Lua：条件
来源：http://rtf.xylfe.cn

if x > 0 then print("正") end
来源：http://rqu.wangshuangyany.cn

[T39] Lua：模式匹配
来源：http://fiu.hysaishi.cn

string.find(s, "%d+")
来源：http://jek.cdnleiting.top

[T40] Lua：元表
来源：http://rdb.xylfe.cn

setmetatable({}, { __index = base })
来源：http://kbm.ppjwa.cn

[T41] Perl：Hello World
来源：http://yzw.zhijiandao.cn

print "Hello\n";
来源：http://xvs.daria6918.cn

[T42] Perl：变量类型
来源：http://cfy.tanke756.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vdh.shanyushiyangkeji.top

[T43] Perl：字符串插值
来源：http://vrf.hcnkem.com

"值: $a"
来源：http://wiz.pengpengdd.cyou

[T44] Perl：条件
来源：http://swz.guannengcc.top

if ($a > 0) { print "正"; }
来源：http://ika.gzhubu.top

[T45] Perl：数组遍历
来源：http://rqy.jinqigfzy.top

for my $x (@arr) { print $x; }
来源：http://bfg.smart0.xyz

[T46] Perl：哈希操作
来源：http://jrr.fehbvm.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://byo.guowangkeji.top

[T47] Perl：正则捕获
来源：http://gqq.pengpengdd.cyou

if ($s =~ /(\d+)/) { print $1; }
来源：http://dyl.zhoulong.xyz

[T48] Perl：正则替换
来源：http://eis.uphjek.com

$s =~ s/old/new/g;
来源：http://zze.snrcjt.cn

[T49] Perl：函数
来源：http://exd.shanyushiyangkeji.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yjm.yongpay.top

[T50] Perl：逐行读文件
来源：http://icj.jianghu66.top

open my $fh, "<", "a.txt" or die $!;
来源：http://nop.zdbjq.cn

while (my $line = <$fh>) { print $line; }
来源：http://ust.cheryme.top

[T51] Scala：Hello World
来源：http://eof.0kj1m.cn

println("Hello")
来源：http://nud.ppjwa.cn

[T52] Scala：变量
来源：http://cfs.hnqzz.top

val a = 1;  var b = 2
来源：http://zgu.zhongyouzk.top

[T53] Scala：字符串插值
来源：http://xpc.guannengcc.top

s"值: $b"
来源：http://liw.yj202588.top

[T54] Scala：集合映射
来源：http://prb.shanyushiyangtech.top


<!-- 参考信息 -->