代发 wailian999

cmd >/dev/null 2>&1
来源：http://kqo.aizwys.cn

[R42] 输入重定向
来源：http://wqb.jinqigfzy.top

wc -l < a.txt
来源：http://wzh.uphjek.com

[R43] 按名字查找文件
来源：http://vqa.fehbvm.com

find . -name "*.log" -type f
来源：http://qbk.fzhhl.top

[R44] 按修改时间查找
来源：http://rgu.epnwcf.com

find . -mtime -7 -type f
来源：http://glv.tianlin.xyz

[R45] 批量删除
来源：http://vxu.tarul.cn

find . -name "*.tmp" -delete
来源：http://cvu.tarul.cn

[R46] 递归替换文件内容
来源：http://ycu.nwbrower.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ibx.vqdsnc.cn

[R47] sed 单行替换
来源：http://frc.xylfe.cn

sed -i 's/foo/bar/g' a.txt
来源：http://aer.zhengqikj.top

[R48] awk 取指定列
来源：http://gte.shangyingyoupin.top

awk '{print $1, $3}' a.txt
来源：http://lez.yonumen.top

[R49] awk 带条件
来源：http://ztd.shzxlz.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bpu.vqdsnc.cn

[R50] awk 求和
来源：http://nkq.chenjidiqi.icu

awk '{s += $2} END {print s}' a.txt
来源：http://xdm.iojbl.cn

[R51] 排序去重取前几
来源：http://esm.yuxming.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qxl.svipenyu.cn

[R52] 统计行数
来源：http://par.gotoacloud.top

wc -l a.txt
来源：http://ewd.yfazqb.com

[R53] 查看文件头与实时尾
来源：http://rxu.yueranfly.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lzu.hnqzz.top

[R54] 比较两个文件
来源：http://pox.xuetiantiany.cn

diff a.txt b.txt
来源：http://qju.aizwys.cn

[R55] 压缩与解压
来源：http://arw.jyoumei.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dsy.zdqjudy.top

[R56] 远程拷贝
来源：http://fed.yongpay.top

scp file user@host:/path/
来源：http://rqg.yanxiufei.cn

[R57] 远程执行命令
来源：http://gof.dashuyun.cn

ssh user@host 'uptime'
来源：http://fkn.jlsjyb.cn

[R58] 下载文件
来源：http://qmv.zhongyouzk.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ool.cheryme.top

[R59] 发 POST JSON
来源：http://ihn.yanxiufei.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jog.dashuyun.cn

[R60] 只看 HTTP 状态码
来源：http://dii.fehbvm.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sfr.xuetiantiany.cn

[R61] 磁盘占用
来源：http://rol.mhx1999.top

df -h;  du -sh *
来源：http://zea.feifeiyinyue.top

[R62] 找最占空间的文件
来源：http://kmo.kuanghao11.cn

du -ah . | sort -rh | head -10
来源：http://dol.jinqigfzy.top

[R63] 内存与进程
来源：http://hep.tianlin.xyz

free -h;  ps aux | grep nginx
来源：http://vpi.jlsjyb.cn

[R64] 结束进程
来源：http://rpp.fzhhl.top

kill -9 $(pgrep -f app.py)
来源：http://sbg.nanxuanxn.top

[R65] 查看端口占用
来源：http://jld.guowangkeji.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ldd.nwbrower.top

[R66] 定时任务
来源：http://wrj.xinyue.icu

crontab -e;  crontab -l
来源：http://ria.hywenlv.cn

[R67] 生成随机十六进制串
来源：http://hhx.chenzaomai.com

openssl rand -hex 16
来源：http://lox.shanyushiyangtech.top

[R68] 计算文件校验值
来源：http://uit.hnqzz.top

sha256sum a.txt;  md5sum a.txt
来源：http://xtw.chenlongwang.top

[R69] 生成随机密码
来源：http://upp.fanxiaobao.xyz

head -c 16 /dev/urandom | base64
来源：http://zud.jinqigufen.top

[R70] 时间戳与互转
来源：http://tzq.chenlongwang.top

date +%s;  date -d @1700000000
来源：http://ent.hnxiangtu.top

[R71] 日期格式化
来源：http://gba.dashuyun.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://akt.jyoumei.cn

[R72] 等待端口就绪
来源：http://cdq.jinqigufen.top

until nc -z localhost 3306; do sleep 1; done
来源：http://byh.hysaishi.cn

[R73] 分割大日志
来源：http://xof.gogol.net.cn

split -l 1000 big.log part_
来源：http://svb.havefunace.top

[R74] 批量重命名
来源：http://ycq.svipenyu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://khe.zhoulong.xyz

[R75] 导出环境变量
来源：http://ihj.tarul.cn

export PATH="$HOME/bin:$PATH"
来源：http://jqp.ydzc1.top

[R76] 使用临时文件
来源：http://zae.yj20258.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bfh.hongshengwenyu.top

[R77] 读取用户输入
来源：http://rno.yuanzhike.top

read -rp "请输入: " ans
来源：http://rsn.ivvv.top

[R78] 交互式菜单
来源：http://tdp.cqqwz.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://twb.hongshengwenyu.top

[R79] 解析命令行选项
来源：http://rca.hywenlv.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gax.jinqigfzy.top

[R80] 查看脚本执行耗时
来源：http://ypn.ydjk.org.cn

time ./run.sh
来源：http://gml.fengsongda.top

================================================================================
来源：http://daq.jqgfzy.top

S. C / C++ 专题
来源：http://mjw.daria6918.cn

================================================================================
来源：http://oak.c1oappe.top

[S01] C：Hello World
来源：http://rii.hcnkem.com

#include <stdio.h>
来源：http://iku.haohaochexian.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://huv.zhixingplan.top

[S02] C：变量与格式化输出
来源：http://ujq.sweek.top

int a = 10; printf("%d\n", a);
来源：http://aao.yvedp.cn

[S03] C：读入整数
来源：http://jua.nanxinkj.top

int x; scanf("%d", &x);
来源：http://bst.316326.xyz

[S04] C：字符串复制
来源：http://ubm.c1oappe.top

char dst[32]; strcpy(dst, "hi");
来源：http://kgc.dashuyun.cn

[S05] C：字符串长度
来源：http://ezt.sysykeji.top

strlen(s)
来源：http://fay.zhongyouzk.top

[S06] C：字符串比较
来源：http://sfc.yuxming.cn

strcmp(a, b) == 0
来源：http://sfu.aibaodan.cn

[S07] C：数组遍历求和
来源：http://mrb.316326.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uau.shangyingyoupin.top

[S08] C：动态内存分配与释放
来源：http://jdw.sxryk.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ebr.cdnleiting.top

[S09] C：结构体定义与初始化
来源：http://dmg.bbcook.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wiy.tarul.cn

[S10] C：指针与解引用
来源：http://ual.feifeiyinyue.top

int *p = &a;  *p = 5;
来源：http://bnd.tanke756.top

[S11] C：逐行读文件
来源：http://dst.nwbrower.top

FILE *f = fopen("a.txt", "r");
来源：http://xoe.vqdsnc.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://glw.xuetiantiany.cn

fclose(f);
来源：http://imu.fktsv.cn

[S12] C：写文件
来源：http://dav.yj20258888.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fic.vqdsnc.cn

[S13] C：宏定义
来源：http://ame.0kj1m.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://doz.daxiang520.top

[S14] C：枚举
来源：http://egy.jyoumei.cn

enum Color { RED, GREEN, BLUE };
来源：http://mth.hongshengwenyu.top

[S15] C：类型转换
来源：http://cwy.sxryk.cn

(double) a / b
来源：http://tqz.jinyuanbaomall.cn

[S16] C：位操作置位
来源：http://xwk.nanxinkj.top

x |= (1 << 3);
来源：http://vqy.zdqjudy.top

[S17] C：安全拼接字符串
来源：http://lay.yj20258888.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lvz.yj20258888.top

[S18] C：命令行参数
来源：http://xty.fzhhl.top

int main(int argc, char **argv)
来源：http://wuj.wangshuangyany.cn

[S19] C：快速排序
来源：http://ocu.uphjek.com

qsort(a, n, sizeof(int), cmp);
来源：http://iew.haohaochexian.top

[S20] C：二分查找
来源：http://zkv.hongshengwenyu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xeq.pycfn.com

[S21] C：字符类别判断
来源：http://mdi.ivvv.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ugg.jinqigufen.top

[S22] C：字符串转数字
来源：http://rlg.yj20258.top

atoi("42");  strtod("3.14", NULL);
来源：http://nmi.smart0.xyz

[S23] C：随机数
来源：http://xem.jinyuanbaomall.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://yum.fengsongda.top

[S24] C：获取本地时间
来源：http://cdp.yonumen.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qed.jinyuanbaomall.cn

[S25] C：内存拷贝
来源：http://sty.nanxinkj.top

memcpy(dst, src, n);
来源：http://vdr.hysaishi.cn

[S26] C：内存清零
来源：http://dye.tian-w.cn

memset(a, 0, sizeof a);
来源：http://oke.chenjidiqi.icu

[S27] C：定义常量
来源：http://ixg.yangfankeji.com

const double PI = 3.14159;
来源：http://ktn.yongpay.top

[S28] C：静态变量
来源：http://wze.jinyuanbaomall.cn

static int counter = 0;
来源：http://pxf.jinyuanbaomall.cn

[S29] C：变参函数
来源：http://wio.jlsjyb.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://caw.jqgufenzy.top

[S30] C：头文件保护
来源：http://wpx.yueranfly.top

#ifndef X_H
来源：http://ewi.xuetiantiany.cn

#define X_H
来源：http://sgp.tian-w.cn

#endif
来源：http://uom.hcnkem.com

[S31] C++：Hello World
来源：http://meu.zhaomingkeji.xyz

#include <iostream>
来源：http://grp.yueranfly.top

int main() { std::cout << "Hello\n"; }
来源：http://wgn.yj20258.top

[S32] C++：字符串
来源：http://sng.uphjek.com

std::string s = "hi";  s += "!";
来源：http://pnd.yanxiufei.cn

[S33] C++：vector 增删
来源：http://xri.shanyushiyangkeji.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yfn.ywan-chungtsiang.top

[S34] C++：遍历 vector
来源：http://cak.ppjwa.cn

for (auto &x : v) { std::cout << x; }
来源：http://wcd.guowangkeji.top

[S35] C++：map
来源：http://biy.pengpengdd.cyou

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wyz.andypj.xyz

[S36] C++：unordered_map
来源：http://efu.shangyingyoupin.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ucs.fktsv.cn

[S37] C++：set
来源：http://iio.fehbvm.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cyx.gzhubu.top

[S38] C++：排序
来源：http://drz.fzhhl.top

std::sort(v.begin(), v.end());
来源：http://fcs.nwbrower.top

[S39] C++：自定义比较器排序
来源：http://uui.dashuyun.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nmw.zhongyouzk.top

[S40] C++：查找元素
来源：http://dog.chenjidiqi.icu

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mtt.fengsongda.top

[S41] C++：类与构造函数
来源：http://mdw.chenlongwang.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wil.uphjek.com

[S42] C++：继承与虚函数
来源：http://uxk.pengpengdd.cyou

class B : public Base { public: void f() override {} };
来源：http://nms.nanxinkj.top

[S43] C++：智能指针
来源：http://pyq.pycfn.com

auto p = std::make_unique<int>(5);
来源：http://tbh.jinghuilouyu.cn

[S44] C++：引用传参
来源：http://ito.jlsjyb.cn

void inc(int &x) { ++x; }
来源：http://tym.zhaomingkeji.xyz

[S45] C++：lambda
来源：http://xqo.birdmap.top

auto add = [](int a, int b) { return a + b; };
来源：http://vjl.zhoulong.xyz

[S46] C++：函数模板
来源：http://dgu.xinyue.icu

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yyb.yonumen.top

[S47] C++：结构化绑定遍历
来源：http://yuq.hnxiangtu.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xju.yonumen.top

[S48] C++：逐行读文件
来源：http://fdd.ehwqpu.com

std::ifstream in("a.txt");  std::string line;
来源：http://fnf.dianchejie.cn

while (std::getline(in, line)) { }
来源：http://cov.dianchejie.cn

[S49] C++：写文件
来源：http://whp.ybcxt.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://eub.shanyushiyangtech.top

[S50] C++：格式化数字
来源：http://msd.ybcxt.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dyg.chenjidiqi.icu

[S51] C++：显式类型转换
来源：http://emk.wangshuangyany.cn

static_cast<double>(a) / b
来源：http://dwi.nwbrower.top

[S52] C++：const 与 noexcept
来源：http://rxq.mhx1999.top

int size() const noexcept { return n_; }
来源：http://ghk.wangshuangyany.cn

[S53] C++：移动语义
来源：http://tle.sjlbkw.cn

std::vector<int> w = std::move(v);
来源：http://jzn.daxiang520.top

[S54] C++：异常处理
来源：http://uor.bjfxy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://eas.316326.xyz

[S55] C++：结构化绑定
来源：http://bek.fzhhl.top

auto [a, b] = std::make_pair(1, 2);
来源：http://fvu.hnqzz.top

[S56] C++：optional
来源：http://iut.hfpthk.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rag.birdmap.top

[S57] C++：编译期常量
来源：http://nvn.yvedp.cn

constexpr int N = 10;
来源：http://oan.yvedp.cn

[S58] C++：命名空间
来源：http://tyd.cashguo.top

namespace ns { int f() { return 1; } }
来源：http://kpg.zhijiandao.cn

[S59] C++：静态断言
来源：http://rms.xinyue.icu

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xuv.zhijiandao.cn

[S60] C++：遍历并删除元素
来源：http://goq.jiagoushi.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ufe.gotoacloud.top

================================================================================
来源：http://arq.jiagoushi.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zqb.birdmap.top

================================================================================
来源：http://ari.zhoulong.xyz

[T01] Kotlin：Hello World
来源：http://mzz.yuxming.cn

println("Hello")
来源：http://qxb.pengpengdd.cyou

[T02] Kotlin：变量
来源：http://jqc.ybcxt.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ieg.daria6918.cn

[T03] Kotlin：字符串模板
来源：http://six.jinyuanbaomall.cn

"值: $b"
来源：http://atx.gzhubu.top

[T04] Kotlin：空安全
来源：http://jcr.0kj1m.cn

val n: String? = null;  n?.length
来源：http://psu.bjfxy.top

[T05] Kotlin：when 表达式
来源：http://opn.yuanzhike.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qwg.yj20258.top

[T06] Kotlin：集合映射
来源：http://ygv.ydjk.org.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://nzw.zhiwuduotai.top

[T07] Kotlin：集合过滤
来源：http://egg.ppjwa.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://hwv.hfpthk.cn

[T08] Kotlin：数据类
来源：http://kbb.havefunace.top

data class User(val name: String, val age: Int)
来源：http://hyd.ydzc1.top

[T09] Kotlin：扩展函数
来源：http://ura.jyoumei.cn

fun String.exclaim() = this + "!"
来源：http://dny.xingfuxueyuan.xyz

[T10] Kotlin：默认参数
来源：http://vsk.xziqi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ena.vqdsnc.cn

[T11] Kotlin：协程
来源：http://vqa.fanxiaobao.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://zvw.ywan-chungtsiang.top

[T12] Kotlin：解构声明
来源：http://evx.yj202588.top

val (a, b) = Pair(1, 2)
来源：http://ikc.yuanzhike.top

[T13] Kotlin：只读 Map
来源：http://lbd.xuetiantiany.cn

val m = mapOf("a" to 1)
来源：http://ksb.gaohongyu789.top

[T14] Kotlin：循环
来源：http://yzf.yj202588.top

for (i in 1..10) println(i)
来源：http://tqy.dianchejie.cn

[T15] Kotlin：接口
来源：http://mth.hongshengwenyu.top

interface Shape { fun area(): Double }
来源：http://plv.shanyushiyangtech.top

[T16] Swift：Hello World
来源：http://itx.cheryme.top

print("Hello")
来源：http://xin.fktsv.cn

[T17] Swift：变量与常量
来源：http://asw.ehwqpu.com

var a = 1;  let b = 2
来源：http://aua.yueranfly.top

[T18] Swift：字符串插值
来源：http://vxt.pycfn.com

"值: \(b)"
来源：http://skn.sweek.top

[T19] Swift：可选绑定
来源：http://xmi.aibaodan.cn

if let n = opt { print(n) }
来源：http://lnd.zdqjudy.top

[T20] Swift：数组操作
来源：http://afn.haohaochexian.top

var a = [1, 2, 3];  a.append(4)
来源：http://zab.hcnkem.com

[T21] Swift：遍历
来源：http://elb.316326.xyz

for x in a { print(x) }
来源：http://kiw.cashguo.top

[T22] Swift：字典
来源：http://ssv.sufxvd.cn

var d = ["a": 1];  d["b"] = 2
来源：http://yli.fengsongda.top

[T23] Swift：函数
来源：http://ptn.wangdashe.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://aif.jyoumei.cn

[T24] Swift：闭包
来源：http://qot.9152youxi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://fmy.haohaochexian.top

[T25] Swift：结构体
来源：http://xlr.yj202588.top

struct P { var x: Int }
来源：http://qua.zhengqikj.top

[T26] Swift：类与重写
来源：http://dhf.xinyue.icu

class A: Base { override func f() {} }
来源：http://gqj.xuetiantiany.cn

[T27] Swift：错误处理
来源：http://gyw.dianchejie.cn

do { try f() } catch { print(error) }
来源：http://jtz.hfpthk.cn

[T28] Swift：枚举
来源：http://nwp.jiagoushi.top

enum Color { case red, green }
来源：http://roe.cdnleiting.top

[T29] Swift：guard 提前返回
来源：http://gfi.shanyushiyangtech.top

guard let x = opt else { return }
来源：http://gvf.zdbjq.cn

[T30] Swift：协议
来源：http://oab.jyoumei.cn

protocol Shape { func area() -> Double }
来源：http://knw.sxryk.cn

[T31] Lua：Hello World
来源：http://uqa.jinqigfzy.top

print("Hello")
来源：http://heu.nanxinkj.top

[T32] Lua：局部变量
来源：http://spm.sufxvd.cn

local a = 1
来源：http://plv.pycfn.com

[T33] Lua：表（数组）
来源：http://cty.feifeiyinyue.top

local t = {1, 2, 3};  t[4] = 4
来源：http://udh.andypj.xyz

[T34] Lua：遍历表
来源：http://ils.fanxiaobao.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://ohu.yfazqb.com

[T35] Lua：字典表
来源：http://ztl.guowangkeji.top

local d = { a = 1 };  d.b = 2
来源：http://lkv.meibo888.top

[T36] Lua：函数
来源：http://wnq.ctjpmb.com

function add(a, b) return a + b end
来源：http://ziz.0kj1m.cn

[T37] Lua：字符串拼接
来源：http://uwb.jiagoushi.top

"a" .. "b"
来源：http://hqc.fehbvm.com

[T38] Lua：条件
来源：http://ohc.nwbrower.top

if x > 0 then print("正") end
来源：http://enm.feifeiyinyue.top

[T39] Lua：模式匹配
来源：http://ttr.cdnleiting.top

string.find(s, "%d+")
来源：http://ljt.zhijiandao.cn

[T40] Lua：元表
来源：http://rjl.yvedp.cn

setmetatable({}, { __index = base })
来源：http://qkk.xziqi.cn

[T41] Perl：Hello World
来源：http://itu.birdmap.top

print "Hello\n";
来源：http://xqn.yj20258.top

[T42] Perl：变量类型
来源：http://iqt.fzhhl.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cib.hfpthk.cn

[T43] Perl：字符串插值
来源：http://tal.chenlongwang.top

"值: $a"
来源：http://ahk.yj20258.top

[T44] Perl：条件
来源：http://oqm.sufxvd.cn

if ($a > 0) { print "正"; }
来源：http://ahn.zhengqikj.top


<!-- 参考信息 -->