代发 wailian999

cmd >/dev/null 2>&1
来源：http://ejk.hywenlv.cn

[R42] 输入重定向
来源：http://tie.52xcode.cn

wc -l < a.txt
来源：http://huu.jiagoushi.top

[R43] 按名字查找文件
来源：http://nrb.hesvh.cn

find . -name "*.log" -type f
来源：http://mfy.sxryk.cn

[R44] 按修改时间查找
来源：http://wxo.tian-w.cn

find . -mtime -7 -type f
来源：http://iyn.xinyue.icu

[R45] 批量删除
来源：http://ezz.xylfe.cn

find . -name "*.tmp" -delete
来源：http://dzu.tian-w.cn

[R46] 递归替换文件内容
来源：http://eug.vqdsnc.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rbh.c1oappe.top

[R47] sed 单行替换
来源：http://twb.9152youxi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mzl.xylfe.cn

[R48] awk 取指定列
来源：http://nta.yvedp.cn

awk '{print $1, $3}' a.txt
来源：http://gjy.hnxiangtu.top

[R49] awk 带条件
来源：http://rmk.hesvh.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wsw.zhongyouzk.top

[R50] awk 求和
来源：http://pkj.yanxiufei.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wmf.yfazqb.com

[R51] 排序去重取前几
来源：http://zmu.hfpthk.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hwt.hnqzz.top

[R52] 统计行数
来源：http://rco.jlsjyb.cn

wc -l a.txt
来源：http://ytp.gogol.net.cn

[R53] 查看文件头与实时尾
来源：http://dmz.xinyue.icu

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gcm.ehwqpu.com

[R54] 比较两个文件
来源：http://eqg.zhiwuduotai.top

diff a.txt b.txt
来源：http://bwr.bjfxy.top

[R55] 压缩与解压
来源：http://otq.tianlin.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vet.meibo888.top

[R56] 远程拷贝
来源：http://hxd.hcnkem.com

scp file user@host:/path/
来源：http://uik.pycfn.com

[R57] 远程执行命令
来源：http://arg.wangdashe.top

ssh user@host 'uptime'
来源：http://nzl.fzhhl.top

[R58] 下载文件
来源：http://lqm.hammf.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://apv.sufxvd.cn

[R59] 发 POST JSON
来源：http://pqj.hammf.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cll.fktsv.cn

[R60] 只看 HTTP 状态码
来源：http://zwh.feifeiyinyue.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kzk.ybcxt.top

[R61] 磁盘占用
来源：http://qry.shanyushiyangkeji.top

df -h;  du -sh *
来源：http://clw.vehdjk.com

[R62] 找最占空间的文件
来源：http://bua.tian-w.cn

du -ah . | sort -rh | head -10
来源：http://kos.guowangkeji.top

[R63] 内存与进程
来源：http://dfr.tianlin.xyz

free -h;  ps aux | grep nginx
来源：http://rsq.ctjpmb.com

[R64] 结束进程
来源：http://uui.fktsv.cn

kill -9 $(pgrep -f app.py)
来源：http://ifs.c1oappe.top

[R65] 查看端口占用
来源：http://kev.yj202588.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vlz.cqqwz.cn

[R66] 定时任务
来源：http://slf.zhaomingkeji.xyz

crontab -e;  crontab -l
来源：http://wre.xziqi.cn

[R67] 生成随机十六进制串
来源：http://foq.gogol.net.cn

openssl rand -hex 16
来源：http://tdf.dashuyun.cn

[R68] 计算文件校验值
来源：http://nta.yj20258888.top

sha256sum a.txt;  md5sum a.txt
来源：http://avx.sjlbkw.cn

[R69] 生成随机密码
来源：http://xkh.ppjwa.cn

head -c 16 /dev/urandom | base64
来源：http://klk.gotoacloud.top

[R70] 时间戳与互转
来源：http://oei.jianghu66.top

date +%s;  date -d @1700000000
来源：http://ohi.yueranfly.top

[R71] 日期格式化
来源：http://euv.sysykeji.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://sha.daxiang520.top

[R72] 等待端口就绪
来源：http://ufn.0kj1m.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://pkd.yueranfly.top

[R73] 分割大日志
来源：http://ppe.cqqwz.cn

split -l 1000 big.log part_
来源：http://cqs.yanxiufei.cn

[R74] 批量重命名
来源：http://jkv.daria6918.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pim.sjlbkw.cn

[R75] 导出环境变量
来源：http://rki.yj202588.top

export PATH="$HOME/bin:$PATH"
来源：http://gzf.yj202588.top

[R76] 使用临时文件
来源：http://ehz.gzhubu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://plv.jlsjyb.cn

[R77] 读取用户输入
来源：http://jee.316326.xyz

read -rp "请输入: " ans
来源：http://stq.iojbl.cn

[R78] 交互式菜单
来源：http://why.tianlin.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://kxy.yongpay.top

[R79] 解析命令行选项
来源：http://spq.daria6918.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://trd.shanyushiyangtech.top

[R80] 查看脚本执行耗时
来源：http://zql.ybcxt.top

time ./run.sh
来源：http://uoa.yfazqb.com

================================================================================
来源：http://ydv.bjfxy.top

S. C / C++ 专题
来源：http://cjf.cdnleiting.top

================================================================================
来源：http://qgj.vehdjk.com

[S01] C：Hello World
来源：http://twj.shanyushiyangtech.top

#include <stdio.h>
来源：http://osf.tarul.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hot.shzxlz.cn

[S02] C：变量与格式化输出
来源：http://yxc.vqdsnc.cn

int a = 10; printf("%d\n", a);
来源：http://vuh.sjlbkw.cn

[S03] C：读入整数
来源：http://uzr.vehdjk.com

int x; scanf("%d", &x);
来源：http://roz.andypj.xyz

[S04] C：字符串复制
来源：http://vve.ctjpmb.com

char dst[32]; strcpy(dst, "hi");
来源：http://zag.yongpay.top

[S05] C：字符串长度
来源：http://cqn.sysykeji.top

strlen(s)
来源：http://qvv.hysaishi.cn

[S06] C：字符串比较
来源：http://qer.fehbvm.com

strcmp(a, b) == 0
来源：http://syv.yonumen.top

[S07] C：数组遍历求和
来源：http://agy.yangfankeji.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cww.zhiwuduotai.top

[S08] C：动态内存分配与释放
来源：http://rwq.pengpengdd.cyou

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wkf.jqgufenzy.top

[S09] C：结构体定义与初始化
来源：http://vlz.pengpengdd.cyou

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dut.zhongyouzk.top

[S10] C：指针与解引用
来源：http://abz.mhx1999.top

int *p = &a;  *p = 5;
来源：http://uvl.gzhubu.top

[S11] C：逐行读文件
来源：http://smj.yuanzhike.top

FILE *f = fopen("a.txt", "r");
来源：http://rps.yfazqb.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://nnz.zhijiandao.cn

fclose(f);
来源：http://syb.yonumen.top

[S12] C：写文件
来源：http://zil.shanyushiyangkeji.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xmb.redwolf501.top

[S13] C：宏定义
来源：http://vkm.shzxlz.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wsz.xuetiantiany.cn

[S14] C：枚举
来源：http://mnb.hysaishi.cn

enum Color { RED, GREEN, BLUE };
来源：http://wfg.meibo888.top

[S15] C：类型转换
来源：http://fhu.hysaishi.cn

(double) a / b
来源：http://hri.birdmap.top

[S16] C：位操作置位
来源：http://bmy.daxiang520.top

x |= (1 << 3);
来源：http://zdw.sufxvd.cn

[S17] C：安全拼接字符串
来源：http://wne.snrcjt.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://puj.cucudq.cn

[S18] C：命令行参数
来源：http://oas.hammf.cn

int main(int argc, char **argv)
来源：http://icn.mhx1999.top

[S19] C：快速排序
来源：http://pfo.quarkkingdee.top

qsort(a, n, sizeof(int), cmp);
来源：http://uhu.ydjk.org.cn

[S20] C：二分查找
来源：http://vor.shanyushiyangtech.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ikn.uphjek.com

[S21] C：字符类别判断
来源：http://tni.xziqi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://net.jiagoushi.top

[S22] C：字符串转数字
来源：http://lys.ydzc1.top

atoi("42");  strtod("3.14", NULL);
来源：http://icd.meibo888.top

[S23] C：随机数
来源：http://tnv.tarul.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wty.fehbvm.com

[S24] C：获取本地时间
来源：http://ijj.zycfv.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ezf.zdqjudy.top

[S25] C：内存拷贝
来源：http://ewj.pengpengdd.cyou

memcpy(dst, src, n);
来源：http://qmw.guowangkeji.top

[S26] C：内存清零
来源：http://cxx.jinqigufen.top

memset(a, 0, sizeof a);
来源：http://vma.hysaishi.cn

[S27] C：定义常量
来源：http://uds.cashguo.top

const double PI = 3.14159;
来源：http://kor.xziqi.cn

[S28] C：静态变量
来源：http://wde.quarkkingdee.top

static int counter = 0;
来源：http://pmu.zdbjq.cn

[S29] C：变参函数
来源：http://hrb.yuanzhike.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zmq.xuetiantiany.cn

[S30] C：头文件保护
来源：http://rwn.bjfxy.top

#ifndef X_H
来源：http://jyr.ydzc1.top

#define X_H
来源：http://icb.wangshuangyany.cn

#endif
来源：http://gqv.hywenlv.cn

[S31] C++：Hello World
来源：http://xon.vqdsnc.cn

#include <iostream>
来源：http://rzx.ydzc1.top

int main() { std::cout << "Hello\n"; }
来源：http://ymw.aizwys.cn

[S32] C++：字符串
来源：http://iwy.wangdashe.top

std::string s = "hi";  s += "!";
来源：http://gvg.jinqigfzy.top

[S33] C++：vector 增删
来源：http://qst.smart0.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ygu.pycfn.com

[S34] C++：遍历 vector
来源：http://daw.andypj.xyz

for (auto &x : v) { std::cout << x; }
来源：http://bcp.ydzc1.top

[S35] C++：map
来源：http://kjj.jlsjyb.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wtl.yueranfly.top

[S36] C++：unordered_map
来源：http://ikt.ydzc1.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yjj.shangyingyoupin.top

[S37] C++：set
来源：http://cpe.sjlbkw.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ioz.yj202588.top

[S38] C++：排序
来源：http://ukj.zhengqikj.top

std::sort(v.begin(), v.end());
来源：http://img.svipenyu.cn

[S39] C++：自定义比较器排序
来源：http://zjt.xylfe.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jtx.ywan-chungtsiang.top

[S40] C++：查找元素
来源：http://ine.dianchejie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://erf.haohaochexian.top

[S41] C++：类与构造函数
来源：http://ipm.daria6918.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bsw.yfazqb.com

[S42] C++：继承与虚函数
来源：http://kyv.hnqzz.top

class B : public Base { public: void f() override {} };
来源：http://isq.chenlongwang.top

[S43] C++：智能指针
来源：http://edp.cheryme.top

auto p = std::make_unique<int>(5);
来源：http://sjf.zdqjudy.top

[S44] C++：引用传参
来源：http://egr.wangdashe.top

void inc(int &x) { ++x; }
来源：http://qtd.tianlin.xyz

[S45] C++：lambda
来源：http://qpo.fehbvm.com

auto add = [](int a, int b) { return a + b; };
来源：http://jiw.shanyushiyangkeji.top

[S46] C++：函数模板
来源：http://efy.zdbjq.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qgv.ywan-chungtsiang.top

[S47] C++：结构化绑定遍历
来源：http://ndf.yueranfly.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kqq.svipenyu.cn

[S48] C++：逐行读文件
来源：http://uhr.dashuyun.cn

std::ifstream in("a.txt");  std::string line;
来源：http://boc.yanxiufei.cn

while (std::getline(in, line)) { }
来源：http://upf.hongshengwenyu.top

[S49] C++：写文件
来源：http://bog.snrcjt.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ivy.9152youxi.cn

[S50] C++：格式化数字
来源：http://mfn.52xcode.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wfi.chenzaomai.com

[S51] C++：显式类型转换
来源：http://rws.yueranfly.top

static_cast<double>(a) / b
来源：http://jcy.jqgfzy.top

[S52] C++：const 与 noexcept
来源：http://kug.yuxming.cn

int size() const noexcept { return n_; }
来源：http://lbu.zhiwuduotai.top

[S53] C++：移动语义
来源：http://cxm.fzhhl.top

std::vector<int> w = std::move(v);
来源：http://edo.hesvh.cn

[S54] C++：异常处理
来源：http://jqq.chenlongwang.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xzt.dianchejie.cn

[S55] C++：结构化绑定
来源：http://qpq.zhengqikj.top

auto [a, b] = std::make_pair(1, 2);
来源：http://rhq.shuidangran.top

[S56] C++：optional
来源：http://sip.hysaishi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bvr.vqdsnc.cn

[S57] C++：编译期常量
来源：http://yds.hysaishi.cn

constexpr int N = 10;
来源：http://oxp.yanxiufei.cn

[S58] C++：命名空间
来源：http://mfg.aizwys.cn

namespace ns { int f() { return 1; } }
来源：http://kzc.xuanzx.com

[S59] C++：静态断言
来源：http://hwq.sjlbkw.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pzf.iojbl.cn

[S60] C++：遍历并删除元素
来源：http://ebr.zhixingplan.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tjo.redwolf501.top

================================================================================
来源：http://yaa.zhijiandao.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wuo.zhongyouzk.top

================================================================================
来源：http://udm.zhengqikj.top

[T01] Kotlin：Hello World
来源：http://jbk.yuanzhike.top

println("Hello")
来源：http://fml.gotoacloud.top

[T02] Kotlin：变量
来源：http://rjm.ybcxt.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ona.fengsongda.top

[T03] Kotlin：字符串模板
来源：http://bvs.jqgfzy.top

"值: $b"
来源：http://rzw.xziqi.cn

[T04] Kotlin：空安全
来源：http://gwn.yanxiufei.cn

val n: String? = null;  n?.length
来源：http://amc.gzhubu.top

[T05] Kotlin：when 表达式
来源：http://zcq.chenlongwang.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://imp.tianlin.xyz

[T06] Kotlin：集合映射
来源：http://uhr.cdnleiting.top

listOf(1, 2, 3).map { it * 2 }
来源：http://uab.yonumen.top

[T07] Kotlin：集合过滤
来源：http://pgp.yj202588.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://kno.shuidangran.top

[T08] Kotlin：数据类
来源：http://yoc.gzhubu.top

data class User(val name: String, val age: Int)
来源：http://jml.ehwqpu.com

[T09] Kotlin：扩展函数
来源：http://yqe.hfpthk.cn

fun String.exclaim() = this + "!"
来源：http://kke.shangyingyoupin.top

[T10] Kotlin：默认参数
来源：http://pwd.yongpay.top

fun greet(name: String = "World") = "Hi $name"
来源：http://sdb.haohaochexian.top

[T11] Kotlin：协程
来源：http://irs.jinyuanbaomall.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xdv.wangdashe.top

[T12] Kotlin：解构声明
来源：http://zfo.vqdsnc.cn

val (a, b) = Pair(1, 2)
来源：http://nxm.yanxiufei.cn

[T13] Kotlin：只读 Map
来源：http://adm.gzhubu.top

val m = mapOf("a" to 1)
来源：http://jwx.nanxinkj.top

[T14] Kotlin：循环
来源：http://nuf.xziqi.cn

for (i in 1..10) println(i)
来源：http://ota.ybcxt.top

[T15] Kotlin：接口
来源：http://uri.fengsongda.top

interface Shape { fun area(): Double }
来源：http://raw.sweek.top

[T16] Swift：Hello World
来源：http://peu.9152youxi.cn

print("Hello")
来源：http://gnu.zdqjudy.top

[T17] Swift：变量与常量
来源：http://kkl.ehwqpu.com

var a = 1;  let b = 2
来源：http://jcv.ivvv.top

[T18] Swift：字符串插值
来源：http://zsa.yuanzhike.top

"值: \(b)"
来源：http://vlx.fehbvm.com

[T19] Swift：可选绑定
来源：http://tjb.yongpay.top

if let n = opt { print(n) }
来源：http://gka.hnqzz.top

[T20] Swift：数组操作
来源：http://kwy.hfpthk.cn

var a = [1, 2, 3];  a.append(4)
来源：http://nnt.cdnleiting.top

[T21] Swift：遍历
来源：http://fea.zhaomingkeji.xyz

for x in a { print(x) }
来源：http://khj.nanxinkj.top

[T22] Swift：字典
来源：http://rtr.iojbl.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ixr.jinqigfzy.top

[T23] Swift：函数
来源：http://kdz.sxryk.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bft.cheryme.top

[T24] Swift：闭包
来源：http://usq.zhoulong.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://ikv.shzxlz.cn

[T25] Swift：结构体
来源：http://gvd.guowangkeji.top

struct P { var x: Int }
来源：http://nsn.zdqjudy.top

[T26] Swift：类与重写
来源：http://frn.daria6918.cn

class A: Base { override func f() {} }
来源：http://opa.yueranfly.top

[T27] Swift：错误处理
来源：http://hho.sjlbkw.cn

do { try f() } catch { print(error) }
来源：http://yps.hfpthk.cn

[T28] Swift：枚举
来源：http://wex.nwbrower.top

enum Color { case red, green }
来源：http://ash.jianghu66.top

[T29] Swift：guard 提前返回
来源：http://rzq.fzhhl.top

guard let x = opt else { return }
来源：http://xhy.nanxinkj.top

[T30] Swift：协议
来源：http://wnl.yj20258.top

protocol Shape { func area() -> Double }
来源：http://iwm.chenjidiqi.icu

[T31] Lua：Hello World
来源：http://qvj.hammf.cn

print("Hello")
来源：http://rzb.hesvh.cn

[T32] Lua：局部变量
来源：http://fqi.jinghuilouyu.cn

local a = 1
来源：http://dmt.ehwqpu.com

[T33] Lua：表（数组）
来源：http://nma.ehwqpu.com

local t = {1, 2, 3};  t[4] = 4
来源：http://ovu.zycfv.cn

[T34] Lua：遍历表
来源：http://yuq.chenzaomai.com

for i, v in ipairs(t) do print(i, v) end
来源：http://xrd.ydjk.org.cn

[T35] Lua：字典表
来源：http://ypd.chenjidiqi.icu

local d = { a = 1 };  d.b = 2
来源：http://imp.jiagoushi.top

[T36] Lua：函数
来源：http://kzn.jinqigufen.top

function add(a, b) return a + b end
来源：http://gmn.tarul.cn

[T37] Lua：字符串拼接
来源：http://wai.jinghuilouyu.cn

"a" .. "b"
来源：http://tju.yj202588.top

[T38] Lua：条件
来源：http://nkn.yvedp.cn

if x > 0 then print("正") end
来源：http://cnd.yanxiufei.cn

[T39] Lua：模式匹配
来源：http://opp.cucudq.cn

string.find(s, "%d+")
来源：http://poh.birdmap.top

[T40] Lua：元表
来源：http://tbk.yonumen.top

setmetatable({}, { __index = base })
来源：http://hyd.jinghuilouyu.cn

[T41] Perl：Hello World
来源：http://ray.hnqzz.top

print "Hello\n";
来源：http://fyh.yvedp.cn

[T42] Perl：变量类型
来源：http://mln.zhoulong.xyz

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://lpm.sjlbkw.cn

[T43] Perl：字符串插值
来源：http://uwi.shangyingyoupin.top

"值: $a"
来源：http://oyr.sysykeji.top

[T44] Perl：条件
来源：http://oso.daxiang520.top

if ($a > 0) { print "正"; }
来源：http://hjl.aibaodan.cn


<!-- 参考信息 -->