代发 wailian999

find . -name "*.tmp" -delete
来源：http://ata.yj202588.top

[R46] 递归替换文件内容
来源：http://plb.yj20258888.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://arv.kuanghao11.cn

[R47] sed 单行替换
来源：http://lwm.shanyushiyangtech.top

sed -i 's/foo/bar/g' a.txt
来源：http://kwp.yj20258888.top

[R48] awk 取指定列
来源：http://sok.zhiwuduotai.top

awk '{print $1, $3}' a.txt
来源：http://ahz.zdqjudy.top

[R49] awk 带条件
来源：http://kji.zhixingplan.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zjq.guowangkeji.top

[R50] awk 求和
来源：http://fsf.yongpay.top

awk '{s += $2} END {print s}' a.txt
来源：http://twt.zhaomingkeji.xyz

[R51] 排序去重取前几
来源：http://xau.hywenlv.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://lvp.cashguo.top

[R52] 统计行数
来源：http://snj.snrcjt.cn

wc -l a.txt
来源：http://tfe.52xcode.cn

[R53] 查看文件头与实时尾
来源：http://cdk.mhx1999.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kpn.zdqjudy.top

[R54] 比较两个文件
来源：http://snv.havefunace.top

diff a.txt b.txt
来源：http://don.sysykeji.top

[R55] 压缩与解压
来源：http://ley.cqqwz.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bgf.aizwys.cn

[R56] 远程拷贝
来源：http://ngl.cheryme.top

scp file user@host:/path/
来源：http://tid.zhengqikj.top

[R57] 远程执行命令
来源：http://iar.dianchejie.cn

ssh user@host 'uptime'
来源：http://cnr.316326.xyz

[R58] 下载文件
来源：http://bje.ybcxt.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lhc.zhoulong.xyz

[R59] 发 POST JSON
来源：http://xet.zdbjq.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://srp.iojbl.cn

[R60] 只看 HTTP 状态码
来源：http://lcw.shuidangran.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lzg.tanke756.top

[R61] 磁盘占用
来源：http://qao.daria6918.cn

df -h;  du -sh *
来源：http://ope.yfazqb.com

[R62] 找最占空间的文件
来源：http://dzt.sufxvd.cn

du -ah . | sort -rh | head -10
来源：http://qsl.hywenlv.cn

[R63] 内存与进程
来源：http://hve.zdqjudy.top

free -h;  ps aux | grep nginx
来源：http://tcp.yj20258888.top

[R64] 结束进程
来源：http://pgz.cdnleiting.top

kill -9 $(pgrep -f app.py)
来源：http://mmz.yangfankeji.com

[R65] 查看端口占用
来源：http://aug.jqgfzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zpa.yuanzhike.top

[R66] 定时任务
来源：http://nrb.fengsongda.top

crontab -e;  crontab -l
来源：http://ztk.jiagoushi.top

[R67] 生成随机十六进制串
来源：http://naa.xuetiantiany.cn

openssl rand -hex 16
来源：http://rtd.hammf.cn

[R68] 计算文件校验值
来源：http://ssp.ydzc1.top

sha256sum a.txt;  md5sum a.txt
来源：http://acd.andypj.xyz

[R69] 生成随机密码
来源：http://dqa.fehbvm.com

head -c 16 /dev/urandom | base64
来源：http://tbn.hongshengwenyu.top

[R70] 时间戳与互转
来源：http://uur.chenjidiqi.icu

date +%s;  date -d @1700000000
来源：http://eli.gogol.net.cn

[R71] 日期格式化
来源：http://dos.fehbvm.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://dlz.zhaomingkeji.xyz

[R72] 等待端口就绪
来源：http://ngr.xylfe.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zei.svipenyu.cn

[R73] 分割大日志
来源：http://ars.jqgfzy.top

split -l 1000 big.log part_
来源：http://odo.yuanzhike.top

[R74] 批量重命名
来源：http://yux.jianghu66.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nfz.c1oappe.top

[R75] 导出环境变量
来源：http://hgi.zycfv.cn

export PATH="$HOME/bin:$PATH"
来源：http://yys.jinghuilouyu.cn

[R76] 使用临时文件
来源：http://npr.xuanzx.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bil.xuetiantiany.cn

[R77] 读取用户输入
来源：http://nny.meibo888.top

read -rp "请输入: " ans
来源：http://uvg.yuxming.cn

[R78] 交互式菜单
来源：http://vld.yangfankeji.com

select opt in a b c; do echo "$opt"; break; done
来源：http://sqr.sufxvd.cn

[R79] 解析命令行选项
来源：http://ztc.gzhubu.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tlg.zhoulong.xyz

[R80] 查看脚本执行耗时
来源：http://aed.9152youxi.cn

time ./run.sh
来源：http://bfo.jinqigufen.top

================================================================================
来源：http://vki.vehdjk.com

S. C / C++ 专题
来源：http://mxu.uphjek.com

================================================================================
来源：http://grs.xziqi.cn

[S01] C：Hello World
来源：http://jim.smart0.xyz

#include <stdio.h>
来源：http://lzd.0kj1m.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://lmd.yvedp.cn

[S02] C：变量与格式化输出
来源：http://zif.gotoacloud.top

int a = 10; printf("%d\n", a);
来源：http://yld.zhixingplan.top

[S03] C：读入整数
来源：http://nau.yuanzhike.top

int x; scanf("%d", &x);
来源：http://fls.yuanzhike.top

[S04] C：字符串复制
来源：http://ori.andypj.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://vlj.fengsongda.top

[S05] C：字符串长度
来源：http://hso.sufxvd.cn

strlen(s)
来源：http://dkd.xuetiantiany.cn

[S06] C：字符串比较
来源：http://iga.birdmap.top

strcmp(a, b) == 0
来源：http://but.xinyue.icu

[S07] C：数组遍历求和
来源：http://ens.0kj1m.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ncz.ctjpmb.com

[S08] C：动态内存分配与释放
来源：http://wkl.nwbrower.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mcg.yueranfly.top

[S09] C：结构体定义与初始化
来源：http://cpv.fktsv.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cct.jqgufenzy.top

[S10] C：指针与解引用
来源：http://fji.hywenlv.cn

int *p = &a;  *p = 5;
来源：http://rhg.bjfxy.top

[S11] C：逐行读文件
来源：http://efb.0kj1m.cn

FILE *f = fopen("a.txt", "r");
来源：http://pjs.yj20258.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://oec.fengsongda.top

fclose(f);
来源：http://lva.redwolf501.top

[S12] C：写文件
来源：http://ltq.feifeiyinyue.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://teq.xuetiantiany.cn

[S13] C：宏定义
来源：http://qen.sxryk.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sys.cqqwz.cn

[S14] C：枚举
来源：http://weq.xylfe.cn

enum Color { RED, GREEN, BLUE };
来源：http://krz.zhiwuduotai.top

[S15] C：类型转换
来源：http://kgt.0kj1m.cn

(double) a / b
来源：http://vnt.jinqigfzy.top

[S16] C：位操作置位
来源：http://tli.0kj1m.cn

x |= (1 << 3);
来源：http://uve.snrcjt.cn

[S17] C：安全拼接字符串
来源：http://gar.yueranfly.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qry.hnxiangtu.top

[S18] C：命令行参数
来源：http://cob.vqdsnc.cn

int main(int argc, char **argv)
来源：http://zas.52xcode.cn

[S19] C：快速排序
来源：http://ztp.xingfuxueyuan.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://qcd.jinqigufen.top

[S20] C：二分查找
来源：http://rje.zhongyouzk.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nsa.ctjpmb.com

[S21] C：字符类别判断
来源：http://ybc.dianchejie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://uey.birdmap.top

[S22] C：字符串转数字
来源：http://jhd.gogol.net.cn

atoi("42");  strtod("3.14", NULL);
来源：http://dqd.jyoumei.cn

[S23] C：随机数
来源：http://qkw.xziqi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://nki.gaohongyu789.top

[S24] C：获取本地时间
来源：http://dyi.pengpengdd.cyou

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ybv.jinghuilouyu.cn

[S25] C：内存拷贝
来源：http://zfn.epnwcf.com

memcpy(dst, src, n);
来源：http://axk.yuanzhike.top

[S26] C：内存清零
来源：http://tpt.ydjk.org.cn

memset(a, 0, sizeof a);
来源：http://bho.feifeiyinyue.top

[S27] C：定义常量
来源：http://krk.sufxvd.cn

const double PI = 3.14159;
来源：http://jrt.hcnkem.com

[S28] C：静态变量
来源：http://cxn.xziqi.cn

static int counter = 0;
来源：http://uoo.cheryme.top

[S29] C：变参函数
来源：http://huo.sysykeji.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pjv.jinyuanbaomall.cn

[S30] C：头文件保护
来源：http://cta.yuxming.cn

#ifndef X_H
来源：http://lnw.haohaochexian.top

#define X_H
来源：http://uxh.yonumen.top

#endif
来源：http://wuy.hesvh.cn

[S31] C++：Hello World
来源：http://mjq.bbcook.cn

#include <iostream>
来源：http://ojq.fengsongda.top

int main() { std::cout << "Hello\n"; }
来源：http://iva.dianchejie.cn

[S32] C++：字符串
来源：http://kcp.yj202588.top

std::string s = "hi";  s += "!";
来源：http://lev.kuanghao11.cn

[S33] C++：vector 增删
来源：http://tam.yueranfly.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://eyl.cdnleiting.top

[S34] C++：遍历 vector
来源：http://wyl.hywenlv.cn

for (auto &x : v) { std::cout << x; }
来源：http://ogq.jiagoushi.top

[S35] C++：map
来源：http://bwj.hywenlv.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jzl.daxiang520.top

[S36] C++：unordered_map
来源：http://pzr.zhixingplan.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://knk.fktsv.cn

[S37] C++：set
来源：http://osy.pengpengdd.cyou

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qng.zhongyouzk.top

[S38] C++：排序
来源：http://nip.jinqigfzy.top

std::sort(v.begin(), v.end());
来源：http://yhh.feifeiyinyue.top

[S39] C++：自定义比较器排序
来源：http://nfi.xingfuxueyuan.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://obb.yuxming.cn

[S40] C++：查找元素
来源：http://ugw.fanxiaobao.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qke.hongshengwenyu.top

[S41] C++：类与构造函数
来源：http://wgb.shuidangran.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rqs.yj20258.top

[S42] C++：继承与虚函数
来源：http://krr.hnxiangtu.top

class B : public Base { public: void f() override {} };
来源：http://vne.yueranfly.top

[S43] C++：智能指针
来源：http://xgo.cashguo.top

auto p = std::make_unique<int>(5);
来源：http://ojq.gogol.net.cn

[S44] C++：引用传参
来源：http://khy.daxiang520.top

void inc(int &x) { ++x; }
来源：http://qka.xziqi.cn

[S45] C++：lambda
来源：http://rss.shanyushiyangkeji.top

auto add = [](int a, int b) { return a + b; };
来源：http://odi.jlsjyb.cn

[S46] C++：函数模板
来源：http://eah.yangfankeji.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sjk.xinyue.icu

[S47] C++：结构化绑定遍历
来源：http://kdb.ybcxt.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qpc.uphjek.com

[S48] C++：逐行读文件
来源：http://xtg.hywenlv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://lit.0kj1m.cn

while (std::getline(in, line)) { }
来源：http://dfj.yj20258.top

[S49] C++：写文件
来源：http://jeb.jinghuilouyu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gfe.chenzaomai.com

[S50] C++：格式化数字
来源：http://ryx.xziqi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gbh.yuanzhike.top

[S51] C++：显式类型转换
来源：http://ihx.vehdjk.com

static_cast<double>(a) / b
来源：http://caq.smart0.xyz

[S52] C++：const 与 noexcept
来源：http://zcq.tarul.cn

int size() const noexcept { return n_; }
来源：http://hne.hnqzz.top

[S53] C++：移动语义
来源：http://lpt.ehwqpu.com

std::vector<int> w = std::move(v);
来源：http://lxn.shuidangran.top

[S54] C++：异常处理
来源：http://jeo.9152youxi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kgm.xziqi.cn

[S55] C++：结构化绑定
来源：http://maf.xinyue.icu

auto [a, b] = std::make_pair(1, 2);
来源：http://dve.yfazqb.com

[S56] C++：optional
来源：http://uvy.kuanghao11.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cnh.svipenyu.cn

[S57] C++：编译期常量
来源：http://gef.ydzc1.top

constexpr int N = 10;
来源：http://kwq.shangyingyoupin.top

[S58] C++：命名空间
来源：http://agv.jqgfzy.top

namespace ns { int f() { return 1; } }
来源：http://fyu.ydzc1.top

[S59] C++：静态断言
来源：http://opg.fzhhl.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ivb.shanyushiyangtech.top

[S60] C++：遍历并删除元素
来源：http://mpm.zdqjudy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://scp.hfpthk.cn

================================================================================
来源：http://wxi.hfpthk.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://onj.havefunace.top

================================================================================
来源：http://zvl.pycfn.com

[T01] Kotlin：Hello World
来源：http://cec.shanyushiyangtech.top

println("Hello")
来源：http://qei.yfazqb.com

[T02] Kotlin：变量
来源：http://ftr.cheryme.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jtc.zdbjq.cn

[T03] Kotlin：字符串模板
来源：http://jbo.daxiang520.top

"值: $b"
来源：http://yph.jianghu66.top

[T04] Kotlin：空安全
来源：http://yht.zhengqikj.top

val n: String? = null;  n?.length
来源：http://bsb.fanxiaobao.xyz

[T05] Kotlin：when 表达式
来源：http://blu.svipenyu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fpu.gotoacloud.top

[T06] Kotlin：集合映射
来源：http://mfx.kuanghao11.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://agp.feifeiyinyue.top

[T07] Kotlin：集合过滤
来源：http://jqu.jqgufenzy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://bie.guowangkeji.top

[T08] Kotlin：数据类
来源：http://jdp.sxryk.cn

data class User(val name: String, val age: Int)
来源：http://pei.xinyue.icu

[T09] Kotlin：扩展函数
来源：http://cvh.feifeiyinyue.top

fun String.exclaim() = this + "!"
来源：http://ojl.cheryme.top

[T10] Kotlin：默认参数
来源：http://uxs.sjlbkw.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://sqk.yj20258888.top

[T11] Kotlin：协程
来源：http://jon.nanxinkj.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://sev.xuanzx.com

[T12] Kotlin：解构声明
来源：http://ilt.havefunace.top

val (a, b) = Pair(1, 2)
来源：http://cgu.yfazqb.com

[T13] Kotlin：只读 Map
来源：http://gkz.shangyingyoupin.top

val m = mapOf("a" to 1)
来源：http://dlq.zycfv.cn

[T14] Kotlin：循环
来源：http://ien.fktsv.cn

for (i in 1..10) println(i)
来源：http://tjb.jinqigfzy.top

[T15] Kotlin：接口
来源：http://vpc.ivvv.top

interface Shape { fun area(): Double }
来源：http://utc.jqgufenzy.top

[T16] Swift：Hello World
来源：http://gqe.tanke756.top

print("Hello")
来源：http://fcv.jinqigufen.top

[T17] Swift：变量与常量
来源：http://gvd.hfpthk.cn

var a = 1;  let b = 2
来源：http://tvc.shanyushiyangkeji.top

[T18] Swift：字符串插值
来源：http://gnt.aibaodan.cn

"值: \(b)"
来源：http://qef.zhoulong.xyz

[T19] Swift：可选绑定
来源：http://ddf.hfpthk.cn

if let n = opt { print(n) }
来源：http://bde.gogol.net.cn

[T20] Swift：数组操作
来源：http://hyu.gogol.net.cn

var a = [1, 2, 3];  a.append(4)
来源：http://see.hfpthk.cn

[T21] Swift：遍历
来源：http://kax.cdnleiting.top

for x in a { print(x) }
来源：http://wxv.dashuyun.cn

[T22] Swift：字典
来源：http://qyb.fengsongda.top

var d = ["a": 1];  d["b"] = 2
来源：http://dml.kuanghao11.cn

[T23] Swift：函数
来源：http://udm.gaohongyu789.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nkz.hammf.cn

[T24] Swift：闭包
来源：http://ziw.ivvv.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://dey.cucudq.cn

[T25] Swift：结构体
来源：http://tzl.ppjwa.cn

struct P { var x: Int }
来源：http://tbr.uphjek.com

[T26] Swift：类与重写
来源：http://otu.fktsv.cn

class A: Base { override func f() {} }
来源：http://zay.guannengcc.top

[T27] Swift：错误处理
来源：http://duo.fehbvm.com

do { try f() } catch { print(error) }
来源：http://dvc.yuanzhike.top

[T28] Swift：枚举
来源：http://gtm.xingfuxueyuan.xyz

enum Color { case red, green }
来源：http://hka.zhixingplan.top

[T29] Swift：guard 提前返回
来源：http://bek.iojbl.cn

guard let x = opt else { return }
来源：http://zdv.fzhhl.top

[T30] Swift：协议
来源：http://iun.cucudq.cn

protocol Shape { func area() -> Double }
来源：http://khv.gotoacloud.top

[T31] Lua：Hello World
来源：http://ftb.hesvh.cn

print("Hello")
来源：http://wyb.vqdsnc.cn

[T32] Lua：局部变量
来源：http://hwf.xuetiantiany.cn

local a = 1
来源：http://eze.c1oappe.top

[T33] Lua：表（数组）
来源：http://fft.fengsongda.top

local t = {1, 2, 3};  t[4] = 4
来源：http://zro.wangshuangyany.cn

[T34] Lua：遍历表
来源：http://moq.epnwcf.com

for i, v in ipairs(t) do print(i, v) end
来源：http://frc.ydjk.org.cn

[T35] Lua：字典表
来源：http://zoj.nanxuanxn.top

local d = { a = 1 };  d.b = 2
来源：http://lqm.jiagoushi.top

[T36] Lua：函数
来源：http://hix.sweek.top

function add(a, b) return a + b end
来源：http://ult.bjfxy.top

[T37] Lua：字符串拼接
来源：http://omq.hnqzz.top

"a" .. "b"
来源：http://rik.hcnkem.com

[T38] Lua：条件
来源：http://qnc.aibaodan.cn

if x > 0 then print("正") end
来源：http://mbu.yangfankeji.com

[T39] Lua：模式匹配
来源：http://xoz.ppjwa.cn

string.find(s, "%d+")
来源：http://zgc.shangyingyoupin.top

[T40] Lua：元表
来源：http://nlj.iojbl.cn

setmetatable({}, { __index = base })
来源：http://rjh.zdqjudy.top

[T41] Perl：Hello World
来源：http://vsw.9152youxi.cn

print "Hello\n";
来源：http://mib.mhx1999.top

[T42] Perl：变量类型
来源：http://bor.tarul.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vng.yuxming.cn

[T43] Perl：字符串插值
来源：http://pky.zycfv.cn

"值: $a"
来源：http://ceb.xinyue.icu

[T44] Perl：条件
来源：http://pck.smart0.xyz

if ($a > 0) { print "正"; }
来源：http://bmp.gaohongyu789.top

[T45] Perl：数组遍历
来源：http://oas.kuanghao11.cn

for my $x (@arr) { print $x; }
来源：http://uto.daria6918.cn

[T46] Perl：哈希操作
来源：http://era.ywan-chungtsiang.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gsv.iojbl.cn

[T47] Perl：正则捕获
来源：http://ijk.jinqigufen.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://bsw.9152youxi.cn

[T48] Perl：正则替换
来源：http://kpm.gotoacloud.top

$s =~ s/old/new/g;
来源：http://uoh.yj202588.top


<!-- 参考信息 -->