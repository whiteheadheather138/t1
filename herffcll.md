代发 wailian999

find . -name "*.log" -type f
来源：http://kse.gzhubu.top

[R44] 按修改时间查找
来源：http://jeh.ctjpmb.com

find . -mtime -7 -type f
来源：http://rpb.fengsongda.top

[R45] 批量删除
来源：http://vwl.zdbjq.cn

find . -name "*.tmp" -delete
来源：http://tkf.yuxming.cn

[R46] 递归替换文件内容
来源：http://soz.gzhubu.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://iid.shuidangran.top

[R47] sed 单行替换
来源：http://ejy.gzhubu.top

sed -i 's/foo/bar/g' a.txt
来源：http://czr.aizwys.cn

[R48] awk 取指定列
来源：http://few.vehdjk.com

awk '{print $1, $3}' a.txt
来源：http://xkp.shzxlz.cn

[R49] awk 带条件
来源：http://riz.dianchejie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ama.jyoumei.cn

[R50] awk 求和
来源：http://ddh.hammf.cn

awk '{s += $2} END {print s}' a.txt
来源：http://lqa.aizwys.cn

[R51] 排序去重取前几
来源：http://ujz.yueranfly.top

sort a.txt | uniq -c | sort -rn | head
来源：http://lfi.feifeiyinyue.top

[R52] 统计行数
来源：http://gww.zhengqikj.top

wc -l a.txt
来源：http://ocu.jiagoushi.top

[R53] 查看文件头与实时尾
来源：http://lje.pengpengdd.cyou

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kbk.svipenyu.cn

[R54] 比较两个文件
来源：http://lok.yueranfly.top

diff a.txt b.txt
来源：http://rok.nanxinkj.top

[R55] 压缩与解压
来源：http://zhz.guowangkeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ppy.fzhhl.top

[R56] 远程拷贝
来源：http://dls.jinyuanbaomall.cn

scp file user@host:/path/
来源：http://yyw.sxryk.cn

[R57] 远程执行命令
来源：http://cyi.zhijiandao.cn

ssh user@host 'uptime'
来源：http://elf.fzhhl.top

[R58] 下载文件
来源：http://tjj.hesvh.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jap.ybcxt.top

[R59] 发 POST JSON
来源：http://yxa.ywan-chungtsiang.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ipy.hongshengwenyu.top

[R60] 只看 HTTP 状态码
来源：http://rtc.gotoacloud.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gcx.bbcook.cn

[R61] 磁盘占用
来源：http://fzg.yuanzhike.top

df -h;  du -sh *
来源：http://iqo.yvedp.cn

[R62] 找最占空间的文件
来源：http://lfe.gogol.net.cn

du -ah . | sort -rh | head -10
来源：http://yyz.sysykeji.top

[R63] 内存与进程
来源：http://ikq.cashguo.top

free -h;  ps aux | grep nginx
来源：http://iwf.hnqzz.top

[R64] 结束进程
来源：http://gii.mhx1999.top

kill -9 $(pgrep -f app.py)
来源：http://cec.xylfe.cn

[R65] 查看端口占用
来源：http://uqt.yonumen.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://aya.zhengqikj.top

[R66] 定时任务
来源：http://igg.yuanzhike.top

crontab -e;  crontab -l
来源：http://yvj.hcnkem.com

[R67] 生成随机十六进制串
来源：http://uen.jqgfzy.top

openssl rand -hex 16
来源：http://udp.tanke756.top

[R68] 计算文件校验值
来源：http://xaf.tanke756.top

sha256sum a.txt;  md5sum a.txt
来源：http://mej.bbcook.cn

[R69] 生成随机密码
来源：http://man.birdmap.top

head -c 16 /dev/urandom | base64
来源：http://lsa.0kj1m.cn

[R70] 时间戳与互转
来源：http://pfb.redwolf501.top

date +%s;  date -d @1700000000
来源：http://hpl.yonumen.top

[R71] 日期格式化
来源：http://zgy.ehwqpu.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://urp.kuanghao11.cn

[R72] 等待端口就绪
来源：http://azo.wangshuangyany.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://wxe.hesvh.cn

[R73] 分割大日志
来源：http://vch.fzhhl.top

split -l 1000 big.log part_
来源：http://ilq.guannengcc.top

[R74] 批量重命名
来源：http://oxn.bbcook.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://llz.jlsjyb.cn

[R75] 导出环境变量
来源：http://afc.ydjk.org.cn

export PATH="$HOME/bin:$PATH"
来源：http://pua.zhiwuduotai.top

[R76] 使用临时文件
来源：http://xhy.xingfuxueyuan.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lfv.nwbrower.top

[R77] 读取用户输入
来源：http://fgb.yuanzhike.top

read -rp "请输入: " ans
来源：http://dqf.c1oappe.top

[R78] 交互式菜单
来源：http://jif.daria6918.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://iwp.shuidangran.top

[R79] 解析命令行选项
来源：http://zds.xingfuxueyuan.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bgp.yj20258888.top

[R80] 查看脚本执行耗时
来源：http://ptv.yuxming.cn

time ./run.sh
来源：http://tgx.xingfuxueyuan.xyz

================================================================================
来源：http://abb.0kj1m.cn

S. C / C++ 专题
来源：http://hhw.yuxming.cn

================================================================================
来源：http://kom.yfazqb.com

[S01] C：Hello World
来源：http://yck.sysykeji.top

#include <stdio.h>
来源：http://xfb.hysaishi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ily.nanxinkj.top

[S02] C：变量与格式化输出
来源：http://imk.xinyue.icu

int a = 10; printf("%d\n", a);
来源：http://kvq.gzhubu.top

[S03] C：读入整数
来源：http://kor.hcnkem.com

int x; scanf("%d", &x);
来源：http://etd.zdbjq.cn

[S04] C：字符串复制
来源：http://jyc.smart0.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://kzd.yvedp.cn

[S05] C：字符串长度
来源：http://uho.fanxiaobao.xyz

strlen(s)
来源：http://mfj.gogol.net.cn

[S06] C：字符串比较
来源：http://epz.fzhhl.top

strcmp(a, b) == 0
来源：http://aws.ywan-chungtsiang.top

[S07] C：数组遍历求和
来源：http://vfw.jinyuanbaomall.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xfp.zycfv.cn

[S08] C：动态内存分配与释放
来源：http://xnr.tianlin.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baa.andypj.xyz

[S09] C：结构体定义与初始化
来源：http://vin.yanxiufei.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vqr.shangyingyoupin.top

[S10] C：指针与解引用
来源：http://msk.xuanzx.com

int *p = &a;  *p = 5;
来源：http://dzw.yonumen.top

[S11] C：逐行读文件
来源：http://nko.yonumen.top

FILE *f = fopen("a.txt", "r");
来源：http://whr.haohaochexian.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://nko.snrcjt.cn

fclose(f);
来源：http://cgm.yj20258888.top

[S12] C：写文件
来源：http://jgl.tianlin.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qsh.gogol.net.cn

[S13] C：宏定义
来源：http://kdz.jinyuanbaomall.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ilc.xziqi.cn

[S14] C：枚举
来源：http://pct.jianghu66.top

enum Color { RED, GREEN, BLUE };
来源：http://iwq.shanyushiyangtech.top

[S15] C：类型转换
来源：http://xav.xuanzx.com

(double) a / b
来源：http://omt.tianlin.xyz

[S16] C：位操作置位
来源：http://qln.gzhubu.top

x |= (1 << 3);
来源：http://frq.hongshengwenyu.top

[S17] C：安全拼接字符串
来源：http://pkm.feifeiyinyue.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lyy.ctjpmb.com

[S18] C：命令行参数
来源：http://rlh.52xcode.cn

int main(int argc, char **argv)
来源：http://jro.ydzc1.top

[S19] C：快速排序
来源：http://era.fanxiaobao.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://lwu.zdqjudy.top

[S20] C：二分查找
来源：http://cwc.ehwqpu.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rsq.guannengcc.top

[S21] C：字符类别判断
来源：http://kxy.jqgfzy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jcb.nanxuanxn.top

[S22] C：字符串转数字
来源：http://oxy.ppjwa.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ocf.meibo888.top

[S23] C：随机数
来源：http://atq.jinqigfzy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ezc.aibaodan.cn

[S24] C：获取本地时间
来源：http://ckl.jinghuilouyu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zdf.hfpthk.cn

[S25] C：内存拷贝
来源：http://imk.tanke756.top

memcpy(dst, src, n);
来源：http://xva.xuanzx.com

[S26] C：内存清零
来源：http://emt.ydzc1.top

memset(a, 0, sizeof a);
来源：http://ani.xuanzx.com

[S27] C：定义常量
来源：http://ams.yj20258.top

const double PI = 3.14159;
来源：http://lag.dianchejie.cn

[S28] C：静态变量
来源：http://twa.hnqzz.top

static int counter = 0;
来源：http://lza.snrcjt.cn

[S29] C：变参函数
来源：http://sta.zhoulong.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vnq.xuanzx.com

[S30] C：头文件保护
来源：http://jjw.birdmap.top

#ifndef X_H
来源：http://pbt.dianchejie.cn

#define X_H
来源：http://wwh.yj202588.top

#endif
来源：http://qcr.cucudq.cn

[S31] C++：Hello World
来源：http://cqz.316326.xyz

#include <iostream>
来源：http://euk.vehdjk.com

int main() { std::cout << "Hello\n"; }
来源：http://apv.yj202588.top

[S32] C++：字符串
来源：http://nur.dianchejie.cn

std::string s = "hi";  s += "!";
来源：http://jff.hywenlv.cn

[S33] C++：vector 增删
来源：http://rvj.ydzc1.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cua.zhixingplan.top

[S34] C++：遍历 vector
来源：http://hui.shanyushiyangkeji.top

for (auto &x : v) { std::cout << x; }
来源：http://hrz.gogol.net.cn

[S35] C++：map
来源：http://ibx.meibo888.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kuj.birdmap.top

[S36] C++：unordered_map
来源：http://qpe.meibo888.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ntj.0kj1m.cn

[S37] C++：set
来源：http://yma.cheryme.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rsp.hnqzz.top

[S38] C++：排序
来源：http://gxm.c1oappe.top

std::sort(v.begin(), v.end());
来源：http://snt.zdqjudy.top

[S39] C++：自定义比较器排序
来源：http://jgn.9152youxi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hon.fktsv.cn

[S40] C++：查找元素
来源：http://pop.quarkkingdee.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dxu.aibaodan.cn

[S41] C++：类与构造函数
来源：http://dtv.zhengqikj.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xqr.52xcode.cn

[S42] C++：继承与虚函数
来源：http://lzp.wangdashe.top

class B : public Base { public: void f() override {} };
来源：http://ysa.uphjek.com

[S43] C++：智能指针
来源：http://kfm.shanyushiyangtech.top

auto p = std::make_unique<int>(5);
来源：http://gpw.aizwys.cn

[S44] C++：引用传参
来源：http://sew.wangdashe.top

void inc(int &x) { ++x; }
来源：http://gwf.316326.xyz

[S45] C++：lambda
来源：http://yhg.epnwcf.com

auto add = [](int a, int b) { return a + b; };
来源：http://mpu.yanxiufei.cn

[S46] C++：函数模板
来源：http://mas.sxryk.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gix.cheryme.top

[S47] C++：结构化绑定遍历
来源：http://cgg.yuxming.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kys.nwbrower.top

[S48] C++：逐行读文件
来源：http://qrt.nwbrower.top

std::ifstream in("a.txt");  std::string line;
来源：http://bbx.uphjek.com

while (std::getline(in, line)) { }
来源：http://wsw.daxiang520.top

[S49] C++：写文件
来源：http://jlt.yj20258.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://thr.shanyushiyangkeji.top

[S50] C++：格式化数字
来源：http://vdb.sjlbkw.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://srp.zhengqikj.top

[S51] C++：显式类型转换
来源：http://kqm.dianchejie.cn

static_cast<double>(a) / b
来源：http://rvq.xuetiantiany.cn

[S52] C++：const 与 noexcept
来源：http://zsf.shanyushiyangkeji.top

int size() const noexcept { return n_; }
来源：http://jkb.zhiwuduotai.top

[S53] C++：移动语义
来源：http://lel.shanyushiyangkeji.top

std::vector<int> w = std::move(v);
来源：http://imh.sysykeji.top

[S54] C++：异常处理
来源：http://ijt.vqdsnc.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bkw.sjlbkw.cn

[S55] C++：结构化绑定
来源：http://clq.jinghuilouyu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://spj.shangyingyoupin.top

[S56] C++：optional
来源：http://utk.yfazqb.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tvo.yongpay.top

[S57] C++：编译期常量
来源：http://vtz.vqdsnc.cn

constexpr int N = 10;
来源：http://xgy.redwolf501.top

[S58] C++：命名空间
来源：http://trg.ppjwa.cn

namespace ns { int f() { return 1; } }
来源：http://kdm.shuidangran.top

[S59] C++：静态断言
来源：http://qig.yanxiufei.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gkk.yongpay.top

[S60] C++：遍历并删除元素
来源：http://kgm.nwbrower.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zgj.jiagoushi.top

================================================================================
来源：http://pdb.snrcjt.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dpj.yj20258.top

================================================================================
来源：http://vxl.pycfn.com

[T01] Kotlin：Hello World
来源：http://kap.hfpthk.cn

println("Hello")
来源：http://kld.epnwcf.com

[T02] Kotlin：变量
来源：http://smt.chenjidiqi.icu

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://stc.sweek.top

[T03] Kotlin：字符串模板
来源：http://dae.zdqjudy.top

"值: $b"
来源：http://doc.ppjwa.cn

[T04] Kotlin：空安全
来源：http://fgp.zycfv.cn

val n: String? = null;  n?.length
来源：http://hdh.daxiang520.top

[T05] Kotlin：when 表达式
来源：http://cvh.xylfe.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://grq.tianlin.xyz

[T06] Kotlin：集合映射
来源：http://iuy.hammf.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xiz.316326.xyz

[T07] Kotlin：集合过滤
来源：http://msm.9152youxi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://nrz.ybcxt.top

[T08] Kotlin：数据类
来源：http://wts.fktsv.cn

data class User(val name: String, val age: Int)
来源：http://tih.tian-w.cn

[T09] Kotlin：扩展函数
来源：http://nmp.yanxiufei.cn

fun String.exclaim() = this + "!"
来源：http://edc.cashguo.top

[T10] Kotlin：默认参数
来源：http://bvd.cqqwz.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://dti.pengpengdd.cyou

[T11] Kotlin：协程
来源：http://bzq.0kj1m.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://fjm.zhengqikj.top

[T12] Kotlin：解构声明
来源：http://qxe.ivvv.top

val (a, b) = Pair(1, 2)
来源：http://xqj.shanyushiyangtech.top

[T13] Kotlin：只读 Map
来源：http://svu.tanke756.top

val m = mapOf("a" to 1)
来源：http://fro.yueranfly.top

[T14] Kotlin：循环
来源：http://ooq.ivvv.top

for (i in 1..10) println(i)
来源：http://hgm.nanxinkj.top

[T15] Kotlin：接口
来源：http://hjp.xziqi.cn

interface Shape { fun area(): Double }
来源：http://odt.ivvv.top

[T16] Swift：Hello World
来源：http://cdi.hammf.cn

print("Hello")
来源：http://rop.fanxiaobao.xyz

[T17] Swift：变量与常量
来源：http://wrj.ctjpmb.com

var a = 1;  let b = 2
来源：http://wxw.gzhubu.top

[T18] Swift：字符串插值
来源：http://gdu.iojbl.cn

"值: \(b)"
来源：http://hbf.jinqigfzy.top

[T19] Swift：可选绑定
来源：http://rub.jyoumei.cn

if let n = opt { print(n) }
来源：http://abl.hammf.cn

[T20] Swift：数组操作
来源：http://tnx.shuidangran.top

var a = [1, 2, 3];  a.append(4)
来源：http://agh.jyoumei.cn

[T21] Swift：遍历
来源：http://rsj.fanxiaobao.xyz

for x in a { print(x) }
来源：http://aqd.jianghu66.top

[T22] Swift：字典
来源：http://mhu.tanke756.top

var d = ["a": 1];  d["b"] = 2
来源：http://vfk.zdbjq.cn

[T23] Swift：函数
来源：http://mrj.ydzc1.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kli.feifeiyinyue.top

[T24] Swift：闭包
来源：http://sdd.smart0.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://jqw.xinyue.icu

[T25] Swift：结构体
来源：http://buj.wangshuangyany.cn

struct P { var x: Int }
来源：http://pqa.yvedp.cn

[T26] Swift：类与重写
来源：http://qaj.tanke756.top

class A: Base { override func f() {} }
来源：http://vvl.yonumen.top

[T27] Swift：错误处理
来源：http://qqa.tanke756.top

do { try f() } catch { print(error) }
来源：http://sck.dashuyun.cn

[T28] Swift：枚举
来源：http://uou.epnwcf.com

enum Color { case red, green }
来源：http://gsd.sweek.top

[T29] Swift：guard 提前返回
来源：http://tzv.fanxiaobao.xyz

guard let x = opt else { return }
来源：http://yfk.zhaomingkeji.xyz

[T30] Swift：协议
来源：http://dlm.yfazqb.com

protocol Shape { func area() -> Double }
来源：http://lyb.tian-w.cn

[T31] Lua：Hello World
来源：http://cds.cdnleiting.top

print("Hello")
来源：http://laz.kuanghao11.cn

[T32] Lua：局部变量
来源：http://fpq.chenlongwang.top

local a = 1
来源：http://ycp.vqdsnc.cn

[T33] Lua：表（数组）
来源：http://cmu.c1oappe.top

local t = {1, 2, 3};  t[4] = 4
来源：http://jjb.zhiwuduotai.top

[T34] Lua：遍历表
来源：http://ibz.zhaomingkeji.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://xtg.0kj1m.cn

[T35] Lua：字典表
来源：http://nuv.jqgufenzy.top

local d = { a = 1 };  d.b = 2
来源：http://bid.hongshengwenyu.top

[T36] Lua：函数
来源：http://fdu.sufxvd.cn

function add(a, b) return a + b end
来源：http://vmp.cdnleiting.top

[T37] Lua：字符串拼接
来源：http://sll.jiagoushi.top

"a" .. "b"
来源：http://qhq.fengsongda.top

[T38] Lua：条件
来源：http://njx.gotoacloud.top

if x > 0 then print("正") end
来源：http://jhr.tianlin.xyz

[T39] Lua：模式匹配
来源：http://suw.yuanzhike.top

string.find(s, "%d+")
来源：http://scp.sweek.top

[T40] Lua：元表
来源：http://lzh.sjlbkw.cn

setmetatable({}, { __index = base })
来源：http://kkz.yvedp.cn

[T41] Perl：Hello World
来源：http://byy.ctjpmb.com

print "Hello\n";
来源：http://fnf.yvedp.cn

[T42] Perl：变量类型
来源：http://ozi.pengpengdd.cyou

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://uje.sxryk.cn

[T43] Perl：字符串插值
来源：http://yud.hysaishi.cn

"值: $a"
来源：http://hpe.c1oappe.top

[T44] Perl：条件
来源：http://cgl.yanxiufei.cn

if ($a > 0) { print "正"; }
来源：http://wkc.pycfn.com

[T45] Perl：数组遍历
来源：http://crd.bbcook.cn

for my $x (@arr) { print $x; }
来源：http://ihr.bbcook.cn

[T46] Perl：哈希操作
来源：http://qjn.iojbl.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://try.dianchejie.cn


<!-- 参考信息 -->