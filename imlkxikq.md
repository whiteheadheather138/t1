代发 wailian999

cmd >/dev/null 2>&1
来源：http://mmt.cucudq.cn

[R42] 输入重定向
来源：http://zvz.9152youxi.cn

wc -l < a.txt
来源：http://bin.hysaishi.cn

[R43] 按名字查找文件
来源：http://oih.tian-w.cn

find . -name "*.log" -type f
来源：http://pdo.ehwqpu.com

[R44] 按修改时间查找
来源：http://jde.dashuyun.cn

find . -mtime -7 -type f
来源：http://nch.meibo888.top

[R45] 批量删除
来源：http://kjh.xylfe.cn

find . -name "*.tmp" -delete
来源：http://wjm.ehwqpu.com

[R46] 递归替换文件内容
来源：http://rkg.fktsv.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dlf.chenjidiqi.icu

[R47] sed 单行替换
来源：http://bth.sweek.top

sed -i 's/foo/bar/g' a.txt
来源：http://yzq.wangshuangyany.cn

[R48] awk 取指定列
来源：http://bkb.wangdashe.top

awk '{print $1, $3}' a.txt
来源：http://wie.52xcode.cn

[R49] awk 带条件
来源：http://oyb.fehbvm.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://brb.kuanghao11.cn

[R50] awk 求和
来源：http://vyk.dashuyun.cn

awk '{s += $2} END {print s}' a.txt
来源：http://lqo.ppjwa.cn

[R51] 排序去重取前几
来源：http://fpp.jyoumei.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qrf.hammf.cn

[R52] 统计行数
来源：http://fov.gaohongyu789.top

wc -l a.txt
来源：http://kev.kuanghao11.cn

[R53] 查看文件头与实时尾
来源：http://cab.havefunace.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rfz.iojbl.cn

[R54] 比较两个文件
来源：http://daq.aizwys.cn

diff a.txt b.txt
来源：http://zel.tarul.cn

[R55] 压缩与解压
来源：http://spr.tianlin.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://oxh.jqgufenzy.top

[R56] 远程拷贝
来源：http://pyp.yangfankeji.com

scp file user@host:/path/
来源：http://lum.shzxlz.cn

[R57] 远程执行命令
来源：http://hch.yj202588.top

ssh user@host 'uptime'
来源：http://xxd.hongshengwenyu.top

[R58] 下载文件
来源：http://dvt.bjfxy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kvx.chenlongwang.top

[R59] 发 POST JSON
来源：http://tln.birdmap.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://scn.fanxiaobao.xyz

[R60] 只看 HTTP 状态码
来源：http://izs.gzhubu.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uan.ybcxt.top

[R61] 磁盘占用
来源：http://axr.ydzc1.top

df -h;  du -sh *
来源：http://lma.wangdashe.top

[R62] 找最占空间的文件
来源：http://gaw.yuanzhike.top

du -ah . | sort -rh | head -10
来源：http://azx.9152youxi.cn

[R63] 内存与进程
来源：http://ehl.sufxvd.cn

free -h;  ps aux | grep nginx
来源：http://syd.zhixingplan.top

[R64] 结束进程
来源：http://mrp.xuetiantiany.cn

kill -9 $(pgrep -f app.py)
来源：http://egp.zhaomingkeji.xyz

[R65] 查看端口占用
来源：http://ans.hcnkem.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://khr.hnqzz.top

[R66] 定时任务
来源：http://oid.xylfe.cn

crontab -e;  crontab -l
来源：http://lwp.yfazqb.com

[R67] 生成随机十六进制串
来源：http://dfg.chenjidiqi.icu

openssl rand -hex 16
来源：http://ymi.pycfn.com

[R68] 计算文件校验值
来源：http://hwi.sweek.top

sha256sum a.txt;  md5sum a.txt
来源：http://hsb.fehbvm.com

[R69] 生成随机密码
来源：http://nyt.xylfe.cn

head -c 16 /dev/urandom | base64
来源：http://fni.chenzaomai.com

[R70] 时间戳与互转
来源：http://uja.ctjpmb.com

date +%s;  date -d @1700000000
来源：http://nry.yuxming.cn

[R71] 日期格式化
来源：http://gcs.yvedp.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ypr.pycfn.com

[R72] 等待端口就绪
来源：http://psg.hywenlv.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ffv.smart0.xyz

[R73] 分割大日志
来源：http://dds.cqqwz.cn

split -l 1000 big.log part_
来源：http://xzx.snrcjt.cn

[R74] 批量重命名
来源：http://bpg.epnwcf.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://axy.cashguo.top

[R75] 导出环境变量
来源：http://fpi.hammf.cn

export PATH="$HOME/bin:$PATH"
来源：http://sbz.hesvh.cn

[R76] 使用临时文件
来源：http://toe.tian-w.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kav.ybcxt.top

[R77] 读取用户输入
来源：http://rvb.ydzc1.top

read -rp "请输入: " ans
来源：http://cce.haohaochexian.top

[R78] 交互式菜单
来源：http://ony.daxiang520.top

select opt in a b c; do echo "$opt"; break; done
来源：http://zbc.sufxvd.cn

[R79] 解析命令行选项
来源：http://qmj.gaohongyu789.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lcn.yueranfly.top

[R80] 查看脚本执行耗时
来源：http://pne.chenzaomai.com

time ./run.sh
来源：http://hdv.jiagoushi.top

================================================================================
来源：http://pzi.dianchejie.cn

S. C / C++ 专题
来源：http://faw.jianghu66.top

================================================================================
来源：http://atd.cdnleiting.top

[S01] C：Hello World
来源：http://lmv.daria6918.cn

#include <stdio.h>
来源：http://sqf.fzhhl.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://jkl.yonumen.top

[S02] C：变量与格式化输出
来源：http://tfn.sjlbkw.cn

int a = 10; printf("%d\n", a);
来源：http://zyp.fanxiaobao.xyz

[S03] C：读入整数
来源：http://sad.fengsongda.top

int x; scanf("%d", &x);
来源：http://qva.gogol.net.cn

[S04] C：字符串复制
来源：http://qjz.52xcode.cn

char dst[32]; strcpy(dst, "hi");
来源：http://hea.ydjk.org.cn

[S05] C：字符串长度
来源：http://eou.jinghuilouyu.cn

strlen(s)
来源：http://lwu.9152youxi.cn

[S06] C：字符串比较
来源：http://onq.quarkkingdee.top

strcmp(a, b) == 0
来源：http://tti.nanxinkj.top

[S07] C：数组遍历求和
来源：http://avi.guannengcc.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vgp.jinghuilouyu.cn

[S08] C：动态内存分配与释放
来源：http://gdy.hammf.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hlj.yonumen.top

[S09] C：结构体定义与初始化
来源：http://fcm.gzhubu.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kdo.cheryme.top

[S10] C：指针与解引用
来源：http://lbh.yj202588.top

int *p = &a;  *p = 5;
来源：http://swe.pycfn.com

[S11] C：逐行读文件
来源：http://pyp.hfpthk.cn

FILE *f = fopen("a.txt", "r");
来源：http://mxo.zdbjq.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://icz.andypj.xyz

fclose(f);
来源：http://uoc.yfazqb.com

[S12] C：写文件
来源：http://wui.ywan-chungtsiang.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vid.jinqigfzy.top

[S13] C：宏定义
来源：http://jpv.jqgufenzy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vll.daxiang520.top

[S14] C：枚举
来源：http://pjb.ehwqpu.com

enum Color { RED, GREEN, BLUE };
来源：http://wee.smart0.xyz

[S15] C：类型转换
来源：http://zee.snrcjt.cn

(double) a / b
来源：http://ljp.zhijiandao.cn

[S16] C：位操作置位
来源：http://sgi.gaohongyu789.top

x |= (1 << 3);
来源：http://vqt.zycfv.cn

[S17] C：安全拼接字符串
来源：http://zxt.zhijiandao.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ljj.cashguo.top

[S18] C：命令行参数
来源：http://rjb.bbcook.cn

int main(int argc, char **argv)
来源：http://rxf.xingfuxueyuan.xyz

[S19] C：快速排序
来源：http://usr.nanxinkj.top

qsort(a, n, sizeof(int), cmp);
来源：http://qwq.nanxinkj.top

[S20] C：二分查找
来源：http://hrc.guannengcc.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yhv.ivvv.top

[S21] C：字符类别判断
来源：http://lts.chenzaomai.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://brw.fanxiaobao.xyz

[S22] C：字符串转数字
来源：http://qef.cucudq.cn

atoi("42");  strtod("3.14", NULL);
来源：http://kme.316326.xyz

[S23] C：随机数
来源：http://kau.yangfankeji.com

srand(time(NULL));  int r = rand() % 100;
来源：http://hgr.sweek.top

[S24] C：获取本地时间
来源：http://wma.snrcjt.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://how.hesvh.cn

[S25] C：内存拷贝
来源：http://yki.wangshuangyany.cn

memcpy(dst, src, n);
来源：http://wce.sxryk.cn

[S26] C：内存清零
来源：http://fra.yj202588.top

memset(a, 0, sizeof a);
来源：http://edk.shangyingyoupin.top

[S27] C：定义常量
来源：http://gor.vqdsnc.cn

const double PI = 3.14159;
来源：http://yxe.mhx1999.top

[S28] C：静态变量
来源：http://faj.shanyushiyangtech.top

static int counter = 0;
来源：http://rjm.fzhhl.top

[S29] C：变参函数
来源：http://hty.0kj1m.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ord.daria6918.cn

[S30] C：头文件保护
来源：http://ysh.jiagoushi.top

#ifndef X_H
来源：http://isz.chenjidiqi.icu

#define X_H
来源：http://xqx.jlsjyb.cn

#endif
来源：http://dmg.aibaodan.cn

[S31] C++：Hello World
来源：http://hfc.sjlbkw.cn

#include <iostream>
来源：http://sbq.sweek.top

int main() { std::cout << "Hello\n"; }
来源：http://osb.shanyushiyangtech.top

[S32] C++：字符串
来源：http://gbq.kuanghao11.cn

std::string s = "hi";  s += "!";
来源：http://ggw.tanke756.top

[S33] C++：vector 增删
来源：http://exc.mhx1999.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mta.guannengcc.top

[S34] C++：遍历 vector
来源：http://sqi.cucudq.cn

for (auto &x : v) { std::cout << x; }
来源：http://ryd.sweek.top

[S35] C++：map
来源：http://mxq.hywenlv.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jcf.yangfankeji.com

[S36] C++：unordered_map
来源：http://uhc.shangyingyoupin.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ymk.hywenlv.cn

[S37] C++：set
来源：http://wes.zhiwuduotai.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kzr.aizwys.cn

[S38] C++：排序
来源：http://cub.chenzaomai.com

std::sort(v.begin(), v.end());
来源：http://lah.zhoulong.xyz

[S39] C++：自定义比较器排序
来源：http://vvg.yuxming.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kie.dianchejie.cn

[S40] C++：查找元素
来源：http://wsd.xziqi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://npo.jinyuanbaomall.cn

[S41] C++：类与构造函数
来源：http://pta.xuetiantiany.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://anq.snrcjt.cn

[S42] C++：继承与虚函数
来源：http://yfl.ybcxt.top

class B : public Base { public: void f() override {} };
来源：http://luz.chenzaomai.com

[S43] C++：智能指针
来源：http://pbi.gogol.net.cn

auto p = std::make_unique<int>(5);
来源：http://bbl.uphjek.com

[S44] C++：引用传参
来源：http://rng.cheryme.top

void inc(int &x) { ++x; }
来源：http://ubo.ywan-chungtsiang.top

[S45] C++：lambda
来源：http://zcf.gzhubu.top

auto add = [](int a, int b) { return a + b; };
来源：http://mzk.shanyushiyangkeji.top

[S46] C++：函数模板
来源：http://xsl.hysaishi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hok.aizwys.cn

[S47] C++：结构化绑定遍历
来源：http://tjo.xuanzx.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ewz.hcnkem.com

[S48] C++：逐行读文件
来源：http://usw.tian-w.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pto.smart0.xyz

while (std::getline(in, line)) { }
来源：http://kak.tianlin.xyz

[S49] C++：写文件
来源：http://ztx.nwbrower.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tdl.yfazqb.com

[S50] C++：格式化数字
来源：http://jhj.ppjwa.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qii.0kj1m.cn

[S51] C++：显式类型转换
来源：http://uxf.tianlin.xyz

static_cast<double>(a) / b
来源：http://byk.sysykeji.top

[S52] C++：const 与 noexcept
来源：http://kvv.cheryme.top

int size() const noexcept { return n_; }
来源：http://igr.jianghu66.top

[S53] C++：移动语义
来源：http://orp.tarul.cn

std::vector<int> w = std::move(v);
来源：http://kwo.hnqzz.top

[S54] C++：异常处理
来源：http://dqp.hnxiangtu.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vsw.tianlin.xyz

[S55] C++：结构化绑定
来源：http://zgb.jinqigufen.top

auto [a, b] = std::make_pair(1, 2);
来源：http://joe.cashguo.top

[S56] C++：optional
来源：http://gxp.yvedp.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://aqw.xingfuxueyuan.xyz

[S57] C++：编译期常量
来源：http://hlb.xuanzx.com

constexpr int N = 10;
来源：http://utv.c1oappe.top

[S58] C++：命名空间
来源：http://bau.smart0.xyz

namespace ns { int f() { return 1; } }
来源：http://abz.ehwqpu.com

[S59] C++：静态断言
来源：http://yfg.316326.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://owg.chenlongwang.top

[S60] C++：遍历并删除元素
来源：http://gmy.quarkkingdee.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yhq.hfpthk.cn

================================================================================
来源：http://jsl.zhoulong.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jsm.svipenyu.cn

================================================================================
来源：http://zmn.hnxiangtu.top

[T01] Kotlin：Hello World
来源：http://twa.sufxvd.cn

println("Hello")
来源：http://pzr.fktsv.cn

[T02] Kotlin：变量
来源：http://zji.yonumen.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xxd.yvedp.cn

[T03] Kotlin：字符串模板
来源：http://uue.pengpengdd.cyou

"值: $b"
来源：http://gut.yuanzhike.top

[T04] Kotlin：空安全
来源：http://mgv.fktsv.cn

val n: String? = null;  n?.length
来源：http://vfm.316326.xyz

[T05] Kotlin：when 表达式
来源：http://wyj.snrcjt.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://obu.yonumen.top

[T06] Kotlin：集合映射
来源：http://qon.0kj1m.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://dtv.fktsv.cn

[T07] Kotlin：集合过滤
来源：http://jct.shzxlz.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://dek.fanxiaobao.xyz

[T08] Kotlin：数据类
来源：http://hws.cucudq.cn

data class User(val name: String, val age: Int)
来源：http://wbp.yangfankeji.com

[T09] Kotlin：扩展函数
来源：http://dsy.9152youxi.cn

fun String.exclaim() = this + "!"
来源：http://ujb.hysaishi.cn

[T10] Kotlin：默认参数
来源：http://vuj.ctjpmb.com

fun greet(name: String = "World") = "Hi $name"
来源：http://zeo.quarkkingdee.top

[T11] Kotlin：协程
来源：http://gem.havefunace.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://cfn.wangdashe.top

[T12] Kotlin：解构声明
来源：http://pji.jiagoushi.top

val (a, b) = Pair(1, 2)
来源：http://wzf.feifeiyinyue.top

[T13] Kotlin：只读 Map
来源：http://xga.shuidangran.top

val m = mapOf("a" to 1)
来源：http://xpi.kuanghao11.cn

[T14] Kotlin：循环
来源：http://nfu.jianghu66.top

for (i in 1..10) println(i)
来源：http://nds.shangyingyoupin.top

[T15] Kotlin：接口
来源：http://bcn.ctjpmb.com

interface Shape { fun area(): Double }
来源：http://vzc.vqdsnc.cn

[T16] Swift：Hello World
来源：http://fzn.feifeiyinyue.top

print("Hello")
来源：http://dfn.hcnkem.com

[T17] Swift：变量与常量
来源：http://oyb.tianlin.xyz

var a = 1;  let b = 2
来源：http://oqm.bbcook.cn

[T18] Swift：字符串插值
来源：http://anr.kuanghao11.cn

"值: \(b)"
来源：http://mes.tianlin.xyz

[T19] Swift：可选绑定
来源：http://jtb.sxryk.cn

if let n = opt { print(n) }
来源：http://eil.chenlongwang.top

[T20] Swift：数组操作
来源：http://wco.bbcook.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jis.vqdsnc.cn

[T21] Swift：遍历
来源：http://the.cheryme.top

for x in a { print(x) }
来源：http://vct.yvedp.cn

[T22] Swift：字典
来源：http://vhc.hnxiangtu.top

var d = ["a": 1];  d["b"] = 2
来源：http://qzi.wangdashe.top

[T23] Swift：函数
来源：http://ouy.hammf.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ekq.bbcook.cn

[T24] Swift：闭包
来源：http://wum.tarul.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://dni.jiagoushi.top

[T25] Swift：结构体
来源：http://ugt.birdmap.top

struct P { var x: Int }
来源：http://dyd.yj202588.top

[T26] Swift：类与重写
来源：http://kcd.zhongyouzk.top

class A: Base { override func f() {} }
来源：http://onh.yuanzhike.top

[T27] Swift：错误处理
来源：http://vnn.sweek.top

do { try f() } catch { print(error) }
来源：http://cjj.fengsongda.top

[T28] Swift：枚举
来源：http://frv.havefunace.top

enum Color { case red, green }
来源：http://opy.sweek.top

[T29] Swift：guard 提前返回
来源：http://ild.hammf.cn

guard let x = opt else { return }
来源：http://zky.jqgufenzy.top

[T30] Swift：协议
来源：http://vij.hesvh.cn

protocol Shape { func area() -> Double }
来源：http://smk.ppjwa.cn

[T31] Lua：Hello World
来源：http://ebx.52xcode.cn

print("Hello")
来源：http://xyx.gzhubu.top

[T32] Lua：局部变量
来源：http://ams.bbcook.cn

local a = 1
来源：http://wnm.ivvv.top

[T33] Lua：表（数组）
来源：http://itp.jinyuanbaomall.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://yoc.shanyushiyangkeji.top

[T34] Lua：遍历表
来源：http://lxl.ehwqpu.com

for i, v in ipairs(t) do print(i, v) end
来源：http://xcn.vqdsnc.cn

[T35] Lua：字典表
来源：http://sqo.tian-w.cn

local d = { a = 1 };  d.b = 2
来源：http://nsk.fktsv.cn

[T36] Lua：函数
来源：http://xzd.havefunace.top

function add(a, b) return a + b end
来源：http://kyn.xingfuxueyuan.xyz

[T37] Lua：字符串拼接
来源：http://okm.xziqi.cn

"a" .. "b"
来源：http://vbl.pycfn.com

[T38] Lua：条件
来源：http://ial.vehdjk.com

if x > 0 then print("正") end
来源：http://ika.vqdsnc.cn

[T39] Lua：模式匹配
来源：http://kgm.hnxiangtu.top

string.find(s, "%d+")
来源：http://toe.mhx1999.top

[T40] Lua：元表
来源：http://sad.uphjek.com

setmetatable({}, { __index = base })
来源：http://knl.yuanzhike.top

[T41] Perl：Hello World
来源：http://egt.aibaodan.cn

print "Hello\n";
来源：http://zwn.shzxlz.cn

[T42] Perl：变量类型
来源：http://zte.yvedp.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://igu.cdnleiting.top

[T43] Perl：字符串插值
来源：http://sok.sweek.top

"值: $a"
来源：http://rvg.chenlongwang.top

[T44] Perl：条件
来源：http://yjk.zhixingplan.top

if ($a > 0) { print "正"; }
来源：http://jti.ehwqpu.com


<!-- 参考信息 -->