代发 wailian999

find . -name "*.log" -type f
来源：http://jtv.meibo888.top

[R44] 按修改时间查找
来源：http://plz.wangdashe.top

find . -mtime -7 -type f
来源：http://kcg.jinyuanbaomall.cn

[R45] 批量删除
来源：http://kna.chenjidiqi.icu

find . -name "*.tmp" -delete
来源：http://hxm.ywan-chungtsiang.top

[R46] 递归替换文件内容
来源：http://nug.chenlongwang.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tkk.tianlin.xyz

[R47] sed 单行替换
来源：http://ibf.ehwqpu.com

sed -i 's/foo/bar/g' a.txt
来源：http://vrs.dianchejie.cn

[R48] awk 取指定列
来源：http://viy.zhijiandao.cn

awk '{print $1, $3}' a.txt
来源：http://wxw.ivvv.top

[R49] awk 带条件
来源：http://vjb.zhengqikj.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ahb.fktsv.cn

[R50] awk 求和
来源：http://dxw.zhoulong.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://buf.yuanzhike.top

[R51] 排序去重取前几
来源：http://bep.0kj1m.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://zim.andypj.xyz

[R52] 统计行数
来源：http://bsv.fanxiaobao.xyz

wc -l a.txt
来源：http://dvk.chenzaomai.com

[R53] 查看文件头与实时尾
来源：http://vnu.fzhhl.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ayf.cqqwz.cn

[R54] 比较两个文件
来源：http://zyx.xziqi.cn

diff a.txt b.txt
来源：http://gux.fengsongda.top

[R55] 压缩与解压
来源：http://caa.sjlbkw.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xgn.bjfxy.top

[R56] 远程拷贝
来源：http://dns.gzhubu.top

scp file user@host:/path/
来源：http://ioz.ctjpmb.com

[R57] 远程执行命令
来源：http://omr.chenjidiqi.icu

ssh user@host 'uptime'
来源：http://qkz.jinghuilouyu.cn

[R58] 下载文件
来源：http://qcf.nanxinkj.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lhu.hnxiangtu.top

[R59] 发 POST JSON
来源：http://cah.havefunace.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jml.jiagoushi.top

[R60] 只看 HTTP 状态码
来源：http://ucb.chenzaomai.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xur.jqgfzy.top

[R61] 磁盘占用
来源：http://aix.pycfn.com

df -h;  du -sh *
来源：http://uir.zhoulong.xyz

[R62] 找最占空间的文件
来源：http://iil.zhijiandao.cn

du -ah . | sort -rh | head -10
来源：http://jep.zhijiandao.cn

[R63] 内存与进程
来源：http://rnq.iojbl.cn

free -h;  ps aux | grep nginx
来源：http://spi.zdqjudy.top

[R64] 结束进程
来源：http://sqw.yueranfly.top

kill -9 $(pgrep -f app.py)
来源：http://ird.zdqjudy.top

[R65] 查看端口占用
来源：http://bou.jinqigfzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xen.dashuyun.cn

[R66] 定时任务
来源：http://fbd.yonumen.top

crontab -e;  crontab -l
来源：http://zoq.birdmap.top

[R67] 生成随机十六进制串
来源：http://xcq.sweek.top

openssl rand -hex 16
来源：http://kaw.ehwqpu.com

[R68] 计算文件校验值
来源：http://dok.jinqigufen.top

sha256sum a.txt;  md5sum a.txt
来源：http://vhx.xinyue.icu

[R69] 生成随机密码
来源：http://fpj.shanyushiyangkeji.top

head -c 16 /dev/urandom | base64
来源：http://nqe.sxryk.cn

[R70] 时间戳与互转
来源：http://iyy.wangshuangyany.cn

date +%s;  date -d @1700000000
来源：http://xuh.wangshuangyany.cn

[R71] 日期格式化
来源：http://lhz.yuxming.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zmq.gotoacloud.top

[R72] 等待端口就绪
来源：http://uag.sweek.top

until nc -z localhost 3306; do sleep 1; done
来源：http://zdv.nwbrower.top

[R73] 分割大日志
来源：http://gka.ctjpmb.com

split -l 1000 big.log part_
来源：http://dve.sufxvd.cn

[R74] 批量重命名
来源：http://kuv.cdnleiting.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rmd.yongpay.top

[R75] 导出环境变量
来源：http://bmw.wangdashe.top

export PATH="$HOME/bin:$PATH"
来源：http://mri.hfpthk.cn

[R76] 使用临时文件
来源：http://osx.ppjwa.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kbr.shangyingyoupin.top

[R77] 读取用户输入
来源：http://xdp.uphjek.com

read -rp "请输入: " ans
来源：http://uta.aibaodan.cn

[R78] 交互式菜单
来源：http://zoy.hongshengwenyu.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ucf.52xcode.cn

[R79] 解析命令行选项
来源：http://slt.jyoumei.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ywb.chenzaomai.com

[R80] 查看脚本执行耗时
来源：http://wmz.cucudq.cn

time ./run.sh
来源：http://erp.uphjek.com

================================================================================
来源：http://etv.nanxuanxn.top

S. C / C++ 专题
来源：http://bzo.tianlin.xyz

================================================================================
来源：http://xjp.jqgfzy.top

[S01] C：Hello World
来源：http://ove.guowangkeji.top

#include <stdio.h>
来源：http://zru.zhaomingkeji.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://hin.chenjidiqi.icu

[S02] C：变量与格式化输出
来源：http://vod.daxiang520.top

int a = 10; printf("%d\n", a);
来源：http://oir.fengsongda.top

[S03] C：读入整数
来源：http://abs.hysaishi.cn

int x; scanf("%d", &x);
来源：http://qqu.ywan-chungtsiang.top

[S04] C：字符串复制
来源：http://kjy.hfpthk.cn

char dst[32]; strcpy(dst, "hi");
来源：http://cwk.jianghu66.top

[S05] C：字符串长度
来源：http://gmg.jqgfzy.top

strlen(s)
来源：http://wea.zycfv.cn

[S06] C：字符串比较
来源：http://lxq.nanxuanxn.top

strcmp(a, b) == 0
来源：http://cod.ehwqpu.com

[S07] C：数组遍历求和
来源：http://dgx.shzxlz.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vxa.yuanzhike.top

[S08] C：动态内存分配与释放
来源：http://qqs.pengpengdd.cyou

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ydb.jqgufenzy.top

[S09] C：结构体定义与初始化
来源：http://vjx.aibaodan.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tkp.chenjidiqi.icu

[S10] C：指针与解引用
来源：http://qnc.chenjidiqi.icu

int *p = &a;  *p = 5;
来源：http://ujf.hammf.cn

[S11] C：逐行读文件
来源：http://pmz.yongpay.top

FILE *f = fopen("a.txt", "r");
来源：http://mdd.ybcxt.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://tur.yj202588.top

fclose(f);
来源：http://ils.sysykeji.top

[S12] C：写文件
来源：http://pfn.vqdsnc.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vdw.guannengcc.top

[S13] C：宏定义
来源：http://wpm.hcnkem.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://loz.zhoulong.xyz

[S14] C：枚举
来源：http://dxs.chenjidiqi.icu

enum Color { RED, GREEN, BLUE };
来源：http://tqu.chenlongwang.top

[S15] C：类型转换
来源：http://did.ybcxt.top

(double) a / b
来源：http://pee.cdnleiting.top

[S16] C：位操作置位
来源：http://hlo.nwbrower.top

x |= (1 << 3);
来源：http://wjk.epnwcf.com

[S17] C：安全拼接字符串
来源：http://bvm.hongshengwenyu.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rzs.c1oappe.top

[S18] C：命令行参数
来源：http://zgz.nwbrower.top

int main(int argc, char **argv)
来源：http://dnz.yongpay.top

[S19] C：快速排序
来源：http://mnr.fzhhl.top

qsort(a, n, sizeof(int), cmp);
来源：http://yno.gotoacloud.top

[S20] C：二分查找
来源：http://qbz.quarkkingdee.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ywb.hesvh.cn

[S21] C：字符类别判断
来源：http://qvb.hcnkem.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zdc.birdmap.top

[S22] C：字符串转数字
来源：http://mgl.xylfe.cn

atoi("42");  strtod("3.14", NULL);
来源：http://bia.zycfv.cn

[S23] C：随机数
来源：http://rsx.guannengcc.top

srand(time(NULL));  int r = rand() % 100;
来源：http://szv.sysykeji.top

[S24] C：获取本地时间
来源：http://uqi.chenlongwang.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sht.jinghuilouyu.cn

[S25] C：内存拷贝
来源：http://knt.gzhubu.top

memcpy(dst, src, n);
来源：http://jqe.guannengcc.top

[S26] C：内存清零
来源：http://pih.dashuyun.cn

memset(a, 0, sizeof a);
来源：http://xpq.tianlin.xyz

[S27] C：定义常量
来源：http://fte.guannengcc.top

const double PI = 3.14159;
来源：http://kjc.hnqzz.top

[S28] C：静态变量
来源：http://sfl.c1oappe.top

static int counter = 0;
来源：http://cyz.cheryme.top

[S29] C：变参函数
来源：http://zet.chenzaomai.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mle.fktsv.cn

[S30] C：头文件保护
来源：http://sxz.gzhubu.top

#ifndef X_H
来源：http://tji.cashguo.top

#define X_H
来源：http://qso.zhoulong.xyz

#endif
来源：http://sko.guowangkeji.top

[S31] C++：Hello World
来源：http://cmj.316326.xyz

#include <iostream>
来源：http://rgi.ywan-chungtsiang.top

int main() { std::cout << "Hello\n"; }
来源：http://kzp.ydzc1.top

[S32] C++：字符串
来源：http://qdv.dianchejie.cn

std::string s = "hi";  s += "!";
来源：http://cho.0kj1m.cn

[S33] C++：vector 增删
来源：http://crz.haohaochexian.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wmj.jinghuilouyu.cn

[S34] C++：遍历 vector
来源：http://dmo.yangfankeji.com

for (auto &x : v) { std::cout << x; }
来源：http://rsr.jinyuanbaomall.cn

[S35] C++：map
来源：http://ael.xuetiantiany.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fqn.uphjek.com

[S36] C++：unordered_map
来源：http://ycu.mhx1999.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://eme.cqqwz.cn

[S37] C++：set
来源：http://hzp.gotoacloud.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cik.fzhhl.top

[S38] C++：排序
来源：http://sog.gzhubu.top

std::sort(v.begin(), v.end());
来源：http://pye.jlsjyb.cn

[S39] C++：自定义比较器排序
来源：http://wty.zhengqikj.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gww.316326.xyz

[S40] C++：查找元素
来源：http://omo.cashguo.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rah.jiagoushi.top

[S41] C++：类与构造函数
来源：http://rxd.xinyue.icu

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pzu.sysykeji.top

[S42] C++：继承与虚函数
来源：http://yio.chenjidiqi.icu

class B : public Base { public: void f() override {} };
来源：http://aiz.bbcook.cn

[S43] C++：智能指针
来源：http://hjd.hnxiangtu.top

auto p = std::make_unique<int>(5);
来源：http://ork.zhaomingkeji.xyz

[S44] C++：引用传参
来源：http://ahm.jyoumei.cn

void inc(int &x) { ++x; }
来源：http://yfi.iojbl.cn

[S45] C++：lambda
来源：http://swe.jianghu66.top

auto add = [](int a, int b) { return a + b; };
来源：http://xrf.tanke756.top

[S46] C++：函数模板
来源：http://osg.xuanzx.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qug.shanyushiyangkeji.top

[S47] C++：结构化绑定遍历
来源：http://jlf.zhijiandao.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://uoc.sxryk.cn

[S48] C++：逐行读文件
来源：http://wbd.yvedp.cn

std::ifstream in("a.txt");  std::string line;
来源：http://diz.ppjwa.cn

while (std::getline(in, line)) { }
来源：http://yfa.daxiang520.top

[S49] C++：写文件
来源：http://hnu.sufxvd.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ewx.hnxiangtu.top

[S50] C++：格式化数字
来源：http://yps.hesvh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gaj.cdnleiting.top

[S51] C++：显式类型转换
来源：http://uea.daria6918.cn

static_cast<double>(a) / b
来源：http://hhz.wangdashe.top

[S52] C++：const 与 noexcept
来源：http://hyr.andypj.xyz

int size() const noexcept { return n_; }
来源：http://tzv.feifeiyinyue.top

[S53] C++：移动语义
来源：http://xrc.wangdashe.top

std::vector<int> w = std::move(v);
来源：http://pmn.fehbvm.com

[S54] C++：异常处理
来源：http://das.zycfv.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qfb.hcnkem.com

[S55] C++：结构化绑定
来源：http://eqi.guowangkeji.top

auto [a, b] = std::make_pair(1, 2);
来源：http://tgn.cqqwz.cn

[S56] C++：optional
来源：http://abh.havefunace.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ufh.iojbl.cn

[S57] C++：编译期常量
来源：http://cpj.yj20258.top

constexpr int N = 10;
来源：http://lqd.shanyushiyangkeji.top

[S58] C++：命名空间
来源：http://eaa.jqgfzy.top

namespace ns { int f() { return 1; } }
来源：http://yso.yj202588.top

[S59] C++：静态断言
来源：http://zvn.jqgfzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dym.yongpay.top

[S60] C++：遍历并删除元素
来源：http://dpu.hongshengwenyu.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fze.xylfe.cn

================================================================================
来源：http://ayn.zhongyouzk.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uqe.wangshuangyany.cn

================================================================================
来源：http://wyf.cheryme.top

[T01] Kotlin：Hello World
来源：http://hmn.feifeiyinyue.top

println("Hello")
来源：http://pjs.feifeiyinyue.top

[T02] Kotlin：变量
来源：http://aij.vehdjk.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kib.kuanghao11.cn

[T03] Kotlin：字符串模板
来源：http://sho.aizwys.cn

"值: $b"
来源：http://ssf.ydzc1.top

[T04] Kotlin：空安全
来源：http://yoi.fanxiaobao.xyz

val n: String? = null;  n?.length
来源：http://mch.pycfn.com

[T05] Kotlin：when 表达式
来源：http://lor.shanyushiyangkeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fbd.cqqwz.cn

[T06] Kotlin：集合映射
来源：http://knv.yj202588.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ncp.gzhubu.top

[T07] Kotlin：集合过滤
来源：http://btq.zhoulong.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://crm.shanyushiyangkeji.top

[T08] Kotlin：数据类
来源：http://gpv.316326.xyz

data class User(val name: String, val age: Int)
来源：http://wlw.aibaodan.cn

[T09] Kotlin：扩展函数
来源：http://yfw.aibaodan.cn

fun String.exclaim() = this + "!"
来源：http://maw.jianghu66.top

[T10] Kotlin：默认参数
来源：http://ejn.tian-w.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://usa.52xcode.cn

[T11] Kotlin：协程
来源：http://etb.zhaomingkeji.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://zyg.sjlbkw.cn

[T12] Kotlin：解构声明
来源：http://dvd.hysaishi.cn

val (a, b) = Pair(1, 2)
来源：http://mcq.nwbrower.top

[T13] Kotlin：只读 Map
来源：http://frj.pengpengdd.cyou

val m = mapOf("a" to 1)
来源：http://aeu.gogol.net.cn

[T14] Kotlin：循环
来源：http://sqe.vehdjk.com

for (i in 1..10) println(i)
来源：http://mtq.cdnleiting.top

[T15] Kotlin：接口
来源：http://otw.jiagoushi.top

interface Shape { fun area(): Double }
来源：http://cmk.xingfuxueyuan.xyz

[T16] Swift：Hello World
来源：http://omd.ydzc1.top

print("Hello")
来源：http://uxx.chenjidiqi.icu

[T17] Swift：变量与常量
来源：http://sxt.ydzc1.top

var a = 1;  let b = 2
来源：http://reg.fanxiaobao.xyz

[T18] Swift：字符串插值
来源：http://irn.tarul.cn

"值: \(b)"
来源：http://ksq.pycfn.com

[T19] Swift：可选绑定
来源：http://ffn.sweek.top

if let n = opt { print(n) }
来源：http://zqz.jinyuanbaomall.cn

[T20] Swift：数组操作
来源：http://qeg.zhixingplan.top

var a = [1, 2, 3];  a.append(4)
来源：http://nyl.yj20258888.top

[T21] Swift：遍历
来源：http://rtm.yueranfly.top

for x in a { print(x) }
来源：http://ccn.0kj1m.cn

[T22] Swift：字典
来源：http://xak.ybcxt.top

var d = ["a": 1];  d["b"] = 2
来源：http://wac.pengpengdd.cyou

[T23] Swift：函数
来源：http://wgp.sweek.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sbx.cheryme.top

[T24] Swift：闭包
来源：http://hku.wangshuangyany.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://kel.yj20258888.top

[T25] Swift：结构体
来源：http://oui.kuanghao11.cn

struct P { var x: Int }
来源：http://abg.hnqzz.top

[T26] Swift：类与重写
来源：http://elx.gotoacloud.top

class A: Base { override func f() {} }
来源：http://nan.hesvh.cn

[T27] Swift：错误处理
来源：http://yjm.sxryk.cn

do { try f() } catch { print(error) }
来源：http://wlj.tanke756.top

[T28] Swift：枚举
来源：http://jfj.jyoumei.cn

enum Color { case red, green }
来源：http://xpm.zhiwuduotai.top

[T29] Swift：guard 提前返回
来源：http://hsv.zhoulong.xyz

guard let x = opt else { return }
来源：http://nqd.xziqi.cn

[T30] Swift：协议
来源：http://nru.feifeiyinyue.top

protocol Shape { func area() -> Double }
来源：http://shu.gogol.net.cn

[T31] Lua：Hello World
来源：http://pxo.kuanghao11.cn

print("Hello")
来源：http://zwr.yvedp.cn

[T32] Lua：局部变量
来源：http://gdy.yfazqb.com

local a = 1
来源：http://sqt.jinyuanbaomall.cn

[T33] Lua：表（数组）
来源：http://tok.zhiwuduotai.top

local t = {1, 2, 3};  t[4] = 4
来源：http://gqe.svipenyu.cn

[T34] Lua：遍历表
来源：http://tte.hnqzz.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ult.hcnkem.com

[T35] Lua：字典表
来源：http://mdp.jinghuilouyu.cn

local d = { a = 1 };  d.b = 2
来源：http://tbl.nanxuanxn.top

[T36] Lua：函数
来源：http://gnp.smart0.xyz

function add(a, b) return a + b end
来源：http://mwn.ybcxt.top

[T37] Lua：字符串拼接
来源：http://sji.shzxlz.cn

"a" .. "b"
来源：http://mae.pycfn.com

[T38] Lua：条件
来源：http://xbs.shuidangran.top

if x > 0 then print("正") end
来源：http://bye.fengsongda.top

[T39] Lua：模式匹配
来源：http://dzf.jinqigfzy.top

string.find(s, "%d+")
来源：http://lbf.zhiwuduotai.top

[T40] Lua：元表
来源：http://tid.nwbrower.top

setmetatable({}, { __index = base })
来源：http://ceg.shangyingyoupin.top

[T41] Perl：Hello World
来源：http://hmx.mhx1999.top

print "Hello\n";
来源：http://uei.zhaomingkeji.xyz

[T42] Perl：变量类型
来源：http://jzu.iojbl.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://foe.vehdjk.com

[T43] Perl：字符串插值
来源：http://uak.shangyingyoupin.top

"值: $a"
来源：http://wwo.ppjwa.cn

[T44] Perl：条件
来源：http://fwr.nwbrower.top

if ($a > 0) { print "正"; }
来源：http://hef.hnqzz.top

[T45] Perl：数组遍历
来源：http://vgt.jlsjyb.cn

for my $x (@arr) { print $x; }
来源：http://abi.aizwys.cn

[T46] Perl：哈希操作
来源：http://qbd.yonumen.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tfp.zycfv.cn


<!-- 参考信息 -->