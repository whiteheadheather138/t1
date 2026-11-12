代发 wailian999

cmd >/dev/null 2>&1
来源：http://lpr.yuxming.cn

[R42] 输入重定向
来源：http://mww.tian-w.cn

wc -l < a.txt
来源：http://xyi.smart0.xyz

[R43] 按名字查找文件
来源：http://ycj.jinghuilouyu.cn

find . -name "*.log" -type f
来源：http://soe.ywan-chungtsiang.top

[R44] 按修改时间查找
来源：http://ixa.cucudq.cn

find . -mtime -7 -type f
来源：http://hkt.tian-w.cn

[R45] 批量删除
来源：http://kbf.zhengqikj.top

find . -name "*.tmp" -delete
来源：http://uds.jlsjyb.cn

[R46] 递归替换文件内容
来源：http://dnr.feifeiyinyue.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://spf.zdqjudy.top

[R47] sed 单行替换
来源：http://thu.andypj.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://fdi.316326.xyz

[R48] awk 取指定列
来源：http://olj.andypj.xyz

awk '{print $1, $3}' a.txt
来源：http://lwc.yueranfly.top

[R49] awk 带条件
来源：http://lja.sjlbkw.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://iqy.sxryk.cn

[R50] awk 求和
来源：http://gvy.yanxiufei.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ftg.yongpay.top

[R51] 排序去重取前几
来源：http://dok.c1oappe.top

sort a.txt | uniq -c | sort -rn | head
来源：http://gme.gotoacloud.top

[R52] 统计行数
来源：http://yuk.yj20258.top

wc -l a.txt
来源：http://cjm.shangyingyoupin.top

[R53] 查看文件头与实时尾
来源：http://cdn.sxryk.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xpe.shuidangran.top

[R54] 比较两个文件
来源：http://bvi.jinyuanbaomall.cn

diff a.txt b.txt
来源：http://giy.daria6918.cn

[R55] 压缩与解压
来源：http://bnu.xuanzx.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://sjt.yanxiufei.cn

[R56] 远程拷贝
来源：http://lbb.cheryme.top

scp file user@host:/path/
来源：http://izr.fzhhl.top

[R57] 远程执行命令
来源：http://yjt.vqdsnc.cn

ssh user@host 'uptime'
来源：http://ltd.shangyingyoupin.top

[R58] 下载文件
来源：http://zjw.snrcjt.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xhf.smart0.xyz

[R59] 发 POST JSON
来源：http://rjl.zhijiandao.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zhe.zhixingplan.top

[R60] 只看 HTTP 状态码
来源：http://rtb.sxryk.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jox.shuidangran.top

[R61] 磁盘占用
来源：http://jvt.zhijiandao.cn

df -h;  du -sh *
来源：http://rko.zycfv.cn

[R62] 找最占空间的文件
来源：http://rbv.xuetiantiany.cn

du -ah . | sort -rh | head -10
来源：http://zzb.zhongyouzk.top

[R63] 内存与进程
来源：http://ujs.birdmap.top

free -h;  ps aux | grep nginx
来源：http://eon.52xcode.cn

[R64] 结束进程
来源：http://izh.mhx1999.top

kill -9 $(pgrep -f app.py)
来源：http://jlt.aizwys.cn

[R65] 查看端口占用
来源：http://kbb.jinghuilouyu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hkg.daria6918.cn

[R66] 定时任务
来源：http://xdo.gogol.net.cn

crontab -e;  crontab -l
来源：http://fhp.jlsjyb.cn

[R67] 生成随机十六进制串
来源：http://ems.xingfuxueyuan.xyz

openssl rand -hex 16
来源：http://muf.yuxming.cn

[R68] 计算文件校验值
来源：http://kql.daria6918.cn

sha256sum a.txt;  md5sum a.txt
来源：http://wem.dashuyun.cn

[R69] 生成随机密码
来源：http://ijv.yfazqb.com

head -c 16 /dev/urandom | base64
来源：http://fef.shanyushiyangtech.top

[R70] 时间戳与互转
来源：http://miq.316326.xyz

date +%s;  date -d @1700000000
来源：http://jog.ctjpmb.com

[R71] 日期格式化
来源：http://wrr.yj202588.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://esg.zhaomingkeji.xyz

[R72] 等待端口就绪
来源：http://yzt.pycfn.com

until nc -z localhost 3306; do sleep 1; done
来源：http://rlt.fanxiaobao.xyz

[R73] 分割大日志
来源：http://meq.fanxiaobao.xyz

split -l 1000 big.log part_
来源：http://vxh.9152youxi.cn

[R74] 批量重命名
来源：http://dvl.zhaomingkeji.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zvp.cheryme.top

[R75] 导出环境变量
来源：http://exz.kuanghao11.cn

export PATH="$HOME/bin:$PATH"
来源：http://bjt.chenlongwang.top

[R76] 使用临时文件
来源：http://tdc.zhijiandao.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bna.redwolf501.top

[R77] 读取用户输入
来源：http://yeo.gogol.net.cn

read -rp "请输入: " ans
来源：http://rfk.9152youxi.cn

[R78] 交互式菜单
来源：http://yko.pengpengdd.cyou

select opt in a b c; do echo "$opt"; break; done
来源：http://hsw.tian-w.cn

[R79] 解析命令行选项
来源：http://inw.jinqigufen.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ush.jinqigufen.top

[R80] 查看脚本执行耗时
来源：http://ucf.ctjpmb.com

time ./run.sh
来源：http://rvh.wangshuangyany.cn

================================================================================
来源：http://der.xingfuxueyuan.xyz

S. C / C++ 专题
来源：http://lnn.c1oappe.top

================================================================================
来源：http://jlb.yuxming.cn

[S01] C：Hello World
来源：http://dus.xuanzx.com

#include <stdio.h>
来源：http://qgb.fengsongda.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://doj.zhaomingkeji.xyz

[S02] C：变量与格式化输出
来源：http://msb.yj202588.top

int a = 10; printf("%d\n", a);
来源：http://jlo.tarul.cn

[S03] C：读入整数
来源：http://rvp.feifeiyinyue.top

int x; scanf("%d", &x);
来源：http://onn.sjlbkw.cn

[S04] C：字符串复制
来源：http://pgj.sweek.top

char dst[32]; strcpy(dst, "hi");
来源：http://vhk.yuxming.cn

[S05] C：字符串长度
来源：http://tad.vqdsnc.cn

strlen(s)
来源：http://ydp.wangdashe.top

[S06] C：字符串比较
来源：http://qdo.bjfxy.top

strcmp(a, b) == 0
来源：http://ayy.gotoacloud.top

[S07] C：数组遍历求和
来源：http://mvb.feifeiyinyue.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uny.hnqzz.top

[S08] C：动态内存分配与释放
来源：http://jyf.chenzaomai.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zmj.guowangkeji.top

[S09] C：结构体定义与初始化
来源：http://ncv.ivvv.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://utj.xinyue.icu

[S10] C：指针与解引用
来源：http://fvu.fengsongda.top

int *p = &a;  *p = 5;
来源：http://zks.sweek.top

[S11] C：逐行读文件
来源：http://asg.zhoulong.xyz

FILE *f = fopen("a.txt", "r");
来源：http://gke.guowangkeji.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://gwt.yuanzhike.top

fclose(f);
来源：http://vrr.jqgufenzy.top

[S12] C：写文件
来源：http://msa.ybcxt.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bgt.ybcxt.top

[S13] C：宏定义
来源：http://mhy.guannengcc.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://euw.shanyushiyangkeji.top

[S14] C：枚举
来源：http://hru.gotoacloud.top

enum Color { RED, GREEN, BLUE };
来源：http://uqk.xinyue.icu

[S15] C：类型转换
来源：http://wqy.hnxiangtu.top

(double) a / b
来源：http://rcx.yongpay.top

[S16] C：位操作置位
来源：http://cno.9152youxi.cn

x |= (1 << 3);
来源：http://tux.316326.xyz

[S17] C：安全拼接字符串
来源：http://ivz.fehbvm.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cuu.jyoumei.cn

[S18] C：命令行参数
来源：http://cwd.yuanzhike.top

int main(int argc, char **argv)
来源：http://asd.zhixingplan.top

[S19] C：快速排序
来源：http://sad.ybcxt.top

qsort(a, n, sizeof(int), cmp);
来源：http://kcr.jinyuanbaomall.cn

[S20] C：二分查找
来源：http://hue.yj202588.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wsl.ctjpmb.com

[S21] C：字符类别判断
来源：http://ply.dashuyun.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://uso.gogol.net.cn

[S22] C：字符串转数字
来源：http://tco.hcnkem.com

atoi("42");  strtod("3.14", NULL);
来源：http://och.tian-w.cn

[S23] C：随机数
来源：http://gdi.hywenlv.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://chq.c1oappe.top

[S24] C：获取本地时间
来源：http://fcx.ivvv.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://web.pycfn.com

[S25] C：内存拷贝
来源：http://nrp.yj20258.top

memcpy(dst, src, n);
来源：http://uwh.zdqjudy.top

[S26] C：内存清零
来源：http://vlz.birdmap.top

memset(a, 0, sizeof a);
来源：http://lzk.jqgufenzy.top

[S27] C：定义常量
来源：http://rvj.jiagoushi.top

const double PI = 3.14159;
来源：http://ktc.xuanzx.com

[S28] C：静态变量
来源：http://jyo.xylfe.cn

static int counter = 0;
来源：http://hpk.zhoulong.xyz

[S29] C：变参函数
来源：http://swd.jianghu66.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kci.chenjidiqi.icu

[S30] C：头文件保护
来源：http://tiv.dashuyun.cn

#ifndef X_H
来源：http://qmh.ydjk.org.cn

#define X_H
来源：http://dvh.pengpengdd.cyou

#endif
来源：http://kfp.jinyuanbaomall.cn

[S31] C++：Hello World
来源：http://gjn.yongpay.top

#include <iostream>
来源：http://qav.hfpthk.cn

int main() { std::cout << "Hello\n"; }
来源：http://fzn.hnqzz.top

[S32] C++：字符串
来源：http://etu.yangfankeji.com

std::string s = "hi";  s += "!";
来源：http://hqb.svipenyu.cn

[S33] C++：vector 增删
来源：http://bwi.fanxiaobao.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zgx.chenzaomai.com

[S34] C++：遍历 vector
来源：http://ctt.tanke756.top

for (auto &x : v) { std::cout << x; }
来源：http://smd.meibo888.top

[S35] C++：map
来源：http://qss.ehwqpu.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ldm.shanyushiyangtech.top

[S36] C++：unordered_map
来源：http://mbn.zhijiandao.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://asq.9152youxi.cn

[S37] C++：set
来源：http://rnf.dashuyun.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jyp.pycfn.com

[S38] C++：排序
来源：http://xvw.andypj.xyz

std::sort(v.begin(), v.end());
来源：http://ies.havefunace.top

[S39] C++：自定义比较器排序
来源：http://aab.ppjwa.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hrq.zhengqikj.top

[S40] C++：查找元素
来源：http://lwm.sysykeji.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://eiz.vehdjk.com

[S41] C++：类与构造函数
来源：http://ccq.xingfuxueyuan.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jtb.sjlbkw.cn

[S42] C++：继承与虚函数
来源：http://jhn.dianchejie.cn

class B : public Base { public: void f() override {} };
来源：http://oop.cqqwz.cn

[S43] C++：智能指针
来源：http://ybc.cheryme.top

auto p = std::make_unique<int>(5);
来源：http://cin.yj20258888.top

[S44] C++：引用传参
来源：http://roq.chenlongwang.top

void inc(int &x) { ++x; }
来源：http://lmb.wangdashe.top

[S45] C++：lambda
来源：http://pzc.cucudq.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ryi.ppjwa.cn

[S46] C++：函数模板
来源：http://drq.yj20258888.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://eyg.jinqigufen.top

[S47] C++：结构化绑定遍历
来源：http://jsa.quarkkingdee.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pqf.wangshuangyany.cn

[S48] C++：逐行读文件
来源：http://zjp.yueranfly.top

std::ifstream in("a.txt");  std::string line;
来源：http://nno.nwbrower.top

while (std::getline(in, line)) { }
来源：http://vob.fehbvm.com

[S49] C++：写文件
来源：http://yeq.hnxiangtu.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pjo.gzhubu.top

[S50] C++：格式化数字
来源：http://zqu.fanxiaobao.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ffi.gzhubu.top

[S51] C++：显式类型转换
来源：http://sgk.ehwqpu.com

static_cast<double>(a) / b
来源：http://hhr.jlsjyb.cn

[S52] C++：const 与 noexcept
来源：http://tye.snrcjt.cn

int size() const noexcept { return n_; }
来源：http://ngx.jiagoushi.top

[S53] C++：移动语义
来源：http://ope.vqdsnc.cn

std::vector<int> w = std::move(v);
来源：http://rxu.yuanzhike.top

[S54] C++：异常处理
来源：http://kvl.xinyue.icu

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yua.316326.xyz

[S55] C++：结构化绑定
来源：http://wtx.cashguo.top

auto [a, b] = std::make_pair(1, 2);
来源：http://cxk.ybcxt.top

[S56] C++：optional
来源：http://imn.bjfxy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pui.yj20258.top

[S57] C++：编译期常量
来源：http://fxt.vehdjk.com

constexpr int N = 10;
来源：http://ldv.ywan-chungtsiang.top

[S58] C++：命名空间
来源：http://cup.hammf.cn

namespace ns { int f() { return 1; } }
来源：http://isl.yueranfly.top

[S59] C++：静态断言
来源：http://mbg.epnwcf.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bcy.zycfv.cn

[S60] C++：遍历并删除元素
来源：http://lul.hysaishi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xmz.chenzaomai.com

================================================================================
来源：http://qdn.ivvv.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wln.andypj.xyz

================================================================================
来源：http://tyb.gogol.net.cn

[T01] Kotlin：Hello World
来源：http://kuv.cucudq.cn

println("Hello")
来源：http://uqb.zhixingplan.top

[T02] Kotlin：变量
来源：http://ikt.vehdjk.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yui.jqgufenzy.top

[T03] Kotlin：字符串模板
来源：http://lww.zhoulong.xyz

"值: $b"
来源：http://amq.316326.xyz

[T04] Kotlin：空安全
来源：http://aiy.guowangkeji.top

val n: String? = null;  n?.length
来源：http://ruh.yangfankeji.com

[T05] Kotlin：when 表达式
来源：http://uwr.cheryme.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ghj.daria6918.cn

[T06] Kotlin：集合映射
来源：http://zup.hcnkem.com

listOf(1, 2, 3).map { it * 2 }
来源：http://pwk.yangfankeji.com

[T07] Kotlin：集合过滤
来源：http://joy.c1oappe.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://pvy.yj202588.top

[T08] Kotlin：数据类
来源：http://xew.shzxlz.cn

data class User(val name: String, val age: Int)
来源：http://vhe.xingfuxueyuan.xyz

[T09] Kotlin：扩展函数
来源：http://npb.hysaishi.cn

fun String.exclaim() = this + "!"
来源：http://tsy.ydjk.org.cn

[T10] Kotlin：默认参数
来源：http://ukq.chenjidiqi.icu

fun greet(name: String = "World") = "Hi $name"
来源：http://zan.bbcook.cn

[T11] Kotlin：协程
来源：http://itn.cucudq.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://iwm.zhaomingkeji.xyz

[T12] Kotlin：解构声明
来源：http://cpb.birdmap.top

val (a, b) = Pair(1, 2)
来源：http://fqs.shzxlz.cn

[T13] Kotlin：只读 Map
来源：http://iey.xuanzx.com

val m = mapOf("a" to 1)
来源：http://mrk.shanyushiyangkeji.top

[T14] Kotlin：循环
来源：http://cff.jyoumei.cn

for (i in 1..10) println(i)
来源：http://roa.yueranfly.top

[T15] Kotlin：接口
来源：http://unw.jinghuilouyu.cn

interface Shape { fun area(): Double }
来源：http://kjm.sxryk.cn

[T16] Swift：Hello World
来源：http://wxb.zhiwuduotai.top

print("Hello")
来源：http://pmy.aizwys.cn

[T17] Swift：变量与常量
来源：http://cvv.jinqigufen.top

var a = 1;  let b = 2
来源：http://qhg.jinghuilouyu.cn

[T18] Swift：字符串插值
来源：http://dpm.tian-w.cn

"值: \(b)"
来源：http://lpi.gaohongyu789.top

[T19] Swift：可选绑定
来源：http://pnq.jyoumei.cn

if let n = opt { print(n) }
来源：http://icg.zhaomingkeji.xyz

[T20] Swift：数组操作
来源：http://lhx.vqdsnc.cn

var a = [1, 2, 3];  a.append(4)
来源：http://vkx.xziqi.cn

[T21] Swift：遍历
来源：http://ofj.vehdjk.com

for x in a { print(x) }
来源：http://btk.ctjpmb.com

[T22] Swift：字典
来源：http://qku.xinyue.icu

var d = ["a": 1];  d["b"] = 2
来源：http://xiy.hcnkem.com

[T23] Swift：函数
来源：http://onp.ivvv.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dko.gzhubu.top

[T24] Swift：闭包
来源：http://bxj.haohaochexian.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://wof.0kj1m.cn

[T25] Swift：结构体
来源：http://dlu.c1oappe.top

struct P { var x: Int }
来源：http://lpn.hfpthk.cn

[T26] Swift：类与重写
来源：http://qep.kuanghao11.cn

class A: Base { override func f() {} }
来源：http://kyy.jqgufenzy.top

[T27] Swift：错误处理
来源：http://ulg.jinghuilouyu.cn

do { try f() } catch { print(error) }
来源：http://pzp.9152youxi.cn

[T28] Swift：枚举
来源：http://lyi.xingfuxueyuan.xyz

enum Color { case red, green }
来源：http://wmf.9152youxi.cn

[T29] Swift：guard 提前返回
来源：http://ruz.ydzc1.top

guard let x = opt else { return }
来源：http://xfq.yuxming.cn

[T30] Swift：协议
来源：http://wsa.zdbjq.cn

protocol Shape { func area() -> Double }
来源：http://hjb.yuxming.cn

[T31] Lua：Hello World
来源：http://lwm.sweek.top

print("Hello")
来源：http://sha.wangdashe.top

[T32] Lua：局部变量
来源：http://mow.jyoumei.cn

local a = 1
来源：http://mbf.zycfv.cn

[T33] Lua：表（数组）
来源：http://vrl.yueranfly.top

local t = {1, 2, 3};  t[4] = 4
来源：http://qvs.vehdjk.com

[T34] Lua：遍历表
来源：http://ssw.jinghuilouyu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ecm.uphjek.com

[T35] Lua：字典表
来源：http://rrc.jiagoushi.top

local d = { a = 1 };  d.b = 2
来源：http://sho.xingfuxueyuan.xyz

[T36] Lua：函数
来源：http://tps.chenzaomai.com

function add(a, b) return a + b end
来源：http://wky.jinqigfzy.top

[T37] Lua：字符串拼接
来源：http://fvz.zhixingplan.top

"a" .. "b"
来源：http://cjd.aibaodan.cn

[T38] Lua：条件
来源：http://qri.shanyushiyangkeji.top

if x > 0 then print("正") end
来源：http://kmb.yj20258888.top

[T39] Lua：模式匹配
来源：http://bot.ybcxt.top

string.find(s, "%d+")
来源：http://ndc.ivvv.top

[T40] Lua：元表
来源：http://wik.fktsv.cn

setmetatable({}, { __index = base })
来源：http://hjd.chenjidiqi.icu

[T41] Perl：Hello World
来源：http://mnd.hfpthk.cn

print "Hello\n";
来源：http://buc.smart0.xyz

[T42] Perl：变量类型
来源：http://fds.xingfuxueyuan.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vpl.ydjk.org.cn

[T43] Perl：字符串插值
来源：http://lce.ehwqpu.com

"值: $a"
来源：http://yre.hesvh.cn

[T44] Perl：条件
来源：http://peu.dianchejie.cn

if ($a > 0) { print "正"; }
来源：http://ygp.gzhubu.top


<!-- 参考信息 -->