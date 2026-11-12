代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://bmy.jinqigufen.top

[R48] awk 取指定列
来源：http://aqw.quarkkingdee.top

awk '{print $1, $3}' a.txt
来源：http://ugc.dianchejie.cn

[R49] awk 带条件
来源：http://zcl.epnwcf.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pys.smart0.xyz

[R50] awk 求和
来源：http://jfb.smart0.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://uua.hysaishi.cn

[R51] 排序去重取前几
来源：http://qbc.epnwcf.com

sort a.txt | uniq -c | sort -rn | head
来源：http://qwm.zhixingplan.top

[R52] 统计行数
来源：http://nmf.fzhhl.top

wc -l a.txt
来源：http://fdx.0kj1m.cn

[R53] 查看文件头与实时尾
来源：http://hwe.xingfuxueyuan.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dyh.hysaishi.cn

[R54] 比较两个文件
来源：http://ibq.hfpthk.cn

diff a.txt b.txt
来源：http://sng.birdmap.top

[R55] 压缩与解压
来源：http://rtq.chenzaomai.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zpb.smart0.xyz

[R56] 远程拷贝
来源：http://jir.hammf.cn

scp file user@host:/path/
来源：http://mau.zhiwuduotai.top

[R57] 远程执行命令
来源：http://plp.gogol.net.cn

ssh user@host 'uptime'
来源：http://nzn.tanke756.top

[R58] 下载文件
来源：http://tif.yueranfly.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mdd.zhoulong.xyz

[R59] 发 POST JSON
来源：http://gzm.snrcjt.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mrw.daria6918.cn

[R60] 只看 HTTP 状态码
来源：http://nao.fanxiaobao.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nfc.jiagoushi.top

[R61] 磁盘占用
来源：http://lnr.zycfv.cn

df -h;  du -sh *
来源：http://ksv.pycfn.com

[R62] 找最占空间的文件
来源：http://qmc.hnqzz.top

du -ah . | sort -rh | head -10
来源：http://oqy.jinqigufen.top

[R63] 内存与进程
来源：http://tlg.hywenlv.cn

free -h;  ps aux | grep nginx
来源：http://nak.chenjidiqi.icu

[R64] 结束进程
来源：http://aep.smart0.xyz

kill -9 $(pgrep -f app.py)
来源：http://vap.jyoumei.cn

[R65] 查看端口占用
来源：http://wnf.c1oappe.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nfq.hnqzz.top

[R66] 定时任务
来源：http://qwj.zhengqikj.top

crontab -e;  crontab -l
来源：http://nki.hcnkem.com

[R67] 生成随机十六进制串
来源：http://slb.zhengqikj.top

openssl rand -hex 16
来源：http://uam.jiagoushi.top

[R68] 计算文件校验值
来源：http://npr.c1oappe.top

sha256sum a.txt;  md5sum a.txt
来源：http://cpz.c1oappe.top

[R69] 生成随机密码
来源：http://osa.daria6918.cn

head -c 16 /dev/urandom | base64
来源：http://yuy.9152youxi.cn

[R70] 时间戳与互转
来源：http://wfg.wangdashe.top

date +%s;  date -d @1700000000
来源：http://fax.kuanghao11.cn

[R71] 日期格式化
来源：http://yue.zdbjq.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://std.gotoacloud.top

[R72] 等待端口就绪
来源：http://bhg.jinyuanbaomall.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://azk.jiagoushi.top

[R73] 分割大日志
来源：http://vjn.nanxinkj.top

split -l 1000 big.log part_
来源：http://ope.jinyuanbaomall.cn

[R74] 批量重命名
来源：http://cof.hcnkem.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://crl.xuanzx.com

[R75] 导出环境变量
来源：http://nkj.gzhubu.top

export PATH="$HOME/bin:$PATH"
来源：http://fmp.yuanzhike.top

[R76] 使用临时文件
来源：http://auv.redwolf501.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://eiq.shangyingyoupin.top

[R77] 读取用户输入
来源：http://oao.yfazqb.com

read -rp "请输入: " ans
来源：http://cbm.aibaodan.cn

[R78] 交互式菜单
来源：http://sga.pengpengdd.cyou

select opt in a b c; do echo "$opt"; break; done
来源：http://woh.zdqjudy.top

[R79] 解析命令行选项
来源：http://gfy.cdnleiting.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://upj.9152youxi.cn

[R80] 查看脚本执行耗时
来源：http://mwl.guannengcc.top

time ./run.sh
来源：http://hki.birdmap.top

================================================================================
来源：http://sgh.fktsv.cn

S. C / C++ 专题
来源：http://cut.vqdsnc.cn

================================================================================
来源：http://rcf.bjfxy.top

[S01] C：Hello World
来源：http://bqs.shuidangran.top

#include <stdio.h>
来源：http://iki.xingfuxueyuan.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://var.guannengcc.top

[S02] C：变量与格式化输出
来源：http://zuw.redwolf501.top

int a = 10; printf("%d\n", a);
来源：http://doc.0kj1m.cn

[S03] C：读入整数
来源：http://jtk.yj202588.top

int x; scanf("%d", &x);
来源：http://aox.smart0.xyz

[S04] C：字符串复制
来源：http://okn.smart0.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://nzj.hnxiangtu.top

[S05] C：字符串长度
来源：http://hhc.sufxvd.cn

strlen(s)
来源：http://pgy.yj20258.top

[S06] C：字符串比较
来源：http://vvh.bbcook.cn

strcmp(a, b) == 0
来源：http://ova.c1oappe.top

[S07] C：数组遍历求和
来源：http://zyw.zhaomingkeji.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vii.zhongyouzk.top

[S08] C：动态内存分配与释放
来源：http://dcl.zhongyouzk.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hzp.jiagoushi.top

[S09] C：结构体定义与初始化
来源：http://lxs.chenjidiqi.icu

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://geg.shzxlz.cn

[S10] C：指针与解引用
来源：http://gxb.hysaishi.cn

int *p = &a;  *p = 5;
来源：http://zht.gogol.net.cn

[S11] C：逐行读文件
来源：http://ezm.jinyuanbaomall.cn

FILE *f = fopen("a.txt", "r");
来源：http://nqv.sufxvd.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nfq.guannengcc.top

fclose(f);
来源：http://nqp.yanxiufei.cn

[S12] C：写文件
来源：http://hom.gaohongyu789.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ize.sjlbkw.cn

[S13] C：宏定义
来源：http://aoj.redwolf501.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pfp.zhijiandao.cn

[S14] C：枚举
来源：http://sqx.ybcxt.top

enum Color { RED, GREEN, BLUE };
来源：http://rpk.zhongyouzk.top

[S15] C：类型转换
来源：http://arr.pengpengdd.cyou

(double) a / b
来源：http://mxu.shanyushiyangkeji.top

[S16] C：位操作置位
来源：http://rwm.ywan-chungtsiang.top

x |= (1 << 3);
来源：http://zzw.chenlongwang.top

[S17] C：安全拼接字符串
来源：http://ptk.hammf.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kdb.jqgfzy.top

[S18] C：命令行参数
来源：http://pbx.yj202588.top

int main(int argc, char **argv)
来源：http://mff.xinyue.icu

[S19] C：快速排序
来源：http://ltm.jyoumei.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vtq.kuanghao11.cn

[S20] C：二分查找
来源：http://jkl.ppjwa.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pyy.hnqzz.top

[S21] C：字符类别判断
来源：http://uwm.haohaochexian.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fke.sysykeji.top

[S22] C：字符串转数字
来源：http://smd.jinqigufen.top

atoi("42");  strtod("3.14", NULL);
来源：http://vxm.aibaodan.cn

[S23] C：随机数
来源：http://hge.jyoumei.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kwj.pycfn.com

[S24] C：获取本地时间
来源：http://qln.snrcjt.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mom.jinqigufen.top

[S25] C：内存拷贝
来源：http://mlk.yj20258888.top

memcpy(dst, src, n);
来源：http://ikk.zhaomingkeji.xyz

[S26] C：内存清零
来源：http://vlt.hnxiangtu.top

memset(a, 0, sizeof a);
来源：http://luw.daxiang520.top

[S27] C：定义常量
来源：http://jlk.fengsongda.top

const double PI = 3.14159;
来源：http://okv.hesvh.cn

[S28] C：静态变量
来源：http://gdh.yj202588.top

static int counter = 0;
来源：http://mdn.ywan-chungtsiang.top

[S29] C：变参函数
来源：http://ajn.yongpay.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lbl.sxryk.cn

[S30] C：头文件保护
来源：http://tpt.xuetiantiany.cn

#ifndef X_H
来源：http://qea.hnxiangtu.top

#define X_H
来源：http://oji.xylfe.cn

#endif
来源：http://gyy.zhaomingkeji.xyz

[S31] C++：Hello World
来源：http://jfi.aibaodan.cn

#include <iostream>
来源：http://jlp.cheryme.top

int main() { std::cout << "Hello\n"; }
来源：http://ljy.guannengcc.top

[S32] C++：字符串
来源：http://lxn.pengpengdd.cyou

std::string s = "hi";  s += "!";
来源：http://xwh.fanxiaobao.xyz

[S33] C++：vector 增删
来源：http://bxy.shanyushiyangtech.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://khm.xuanzx.com

[S34] C++：遍历 vector
来源：http://wqp.zhaomingkeji.xyz

for (auto &x : v) { std::cout << x; }
来源：http://bjo.hnxiangtu.top

[S35] C++：map
来源：http://lvw.9152youxi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ins.c1oappe.top

[S36] C++：unordered_map
来源：http://wce.fengsongda.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bws.nanxinkj.top

[S37] C++：set
来源：http://bxg.iojbl.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jfm.smart0.xyz

[S38] C++：排序
来源：http://uih.zhiwuduotai.top

std::sort(v.begin(), v.end());
来源：http://ate.jyoumei.cn

[S39] C++：自定义比较器排序
来源：http://dyq.xylfe.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ipk.zdqjudy.top

[S40] C++：查找元素
来源：http://zjn.yongpay.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://arw.jianghu66.top

[S41] C++：类与构造函数
来源：http://foj.shuidangran.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vdl.hesvh.cn

[S42] C++：继承与虚函数
来源：http://xua.gaohongyu789.top

class B : public Base { public: void f() override {} };
来源：http://new.ydzc1.top

[S43] C++：智能指针
来源：http://oon.wangdashe.top

auto p = std::make_unique<int>(5);
来源：http://urz.fehbvm.com

[S44] C++：引用传参
来源：http://qky.zdbjq.cn

void inc(int &x) { ++x; }
来源：http://jsl.hnqzz.top

[S45] C++：lambda
来源：http://xhb.haohaochexian.top

auto add = [](int a, int b) { return a + b; };
来源：http://wxr.sweek.top

[S46] C++：函数模板
来源：http://ybp.wangshuangyany.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mrn.ybcxt.top

[S47] C++：结构化绑定遍历
来源：http://ebm.ehwqpu.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ywa.gogol.net.cn

[S48] C++：逐行读文件
来源：http://yhb.yj202588.top

std::ifstream in("a.txt");  std::string line;
来源：http://yyk.yfazqb.com

while (std::getline(in, line)) { }
来源：http://gen.zhoulong.xyz

[S49] C++：写文件
来源：http://edk.fzhhl.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xuq.ppjwa.cn

[S50] C++：格式化数字
来源：http://hfw.zhengqikj.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://eqh.hammf.cn

[S51] C++：显式类型转换
来源：http://bnc.aizwys.cn

static_cast<double>(a) / b
来源：http://jer.52xcode.cn

[S52] C++：const 与 noexcept
来源：http://qqa.quarkkingdee.top

int size() const noexcept { return n_; }
来源：http://sga.jyoumei.cn

[S53] C++：移动语义
来源：http://zxr.yongpay.top

std::vector<int> w = std::move(v);
来源：http://opd.birdmap.top

[S54] C++：异常处理
来源：http://fnf.xuetiantiany.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nkk.tanke756.top

[S55] C++：结构化绑定
来源：http://rhr.shzxlz.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://drl.quarkkingdee.top

[S56] C++：optional
来源：http://azc.316326.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ahg.gaohongyu789.top

[S57] C++：编译期常量
来源：http://zzv.hnxiangtu.top

constexpr int N = 10;
来源：http://vij.xingfuxueyuan.xyz

[S58] C++：命名空间
来源：http://snn.shzxlz.cn

namespace ns { int f() { return 1; } }
来源：http://acz.daxiang520.top

[S59] C++：静态断言
来源：http://jum.guannengcc.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mdy.jiagoushi.top

[S60] C++：遍历并删除元素
来源：http://zfm.zhongyouzk.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://brw.dashuyun.cn

================================================================================
来源：http://vio.yanxiufei.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kus.sysykeji.top

================================================================================
来源：http://lnq.jlsjyb.cn

[T01] Kotlin：Hello World
来源：http://adf.bbcook.cn

println("Hello")
来源：http://goe.jqgufenzy.top

[T02] Kotlin：变量
来源：http://kcr.yangfankeji.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pgh.havefunace.top

[T03] Kotlin：字符串模板
来源：http://wwx.kuanghao11.cn

"值: $b"
来源：http://sex.cheryme.top

[T04] Kotlin：空安全
来源：http://uca.zhixingplan.top

val n: String? = null;  n?.length
来源：http://axg.yj202588.top

[T05] Kotlin：when 表达式
来源：http://rnx.hnxiangtu.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cmj.zhiwuduotai.top

[T06] Kotlin：集合映射
来源：http://vfo.jinqigfzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://tqp.sxryk.cn

[T07] Kotlin：集合过滤
来源：http://oor.jqgfzy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://iav.hysaishi.cn

[T08] Kotlin：数据类
来源：http://fqh.tian-w.cn

data class User(val name: String, val age: Int)
来源：http://rve.birdmap.top

[T09] Kotlin：扩展函数
来源：http://yta.jinyuanbaomall.cn

fun String.exclaim() = this + "!"
来源：http://xhe.vqdsnc.cn

[T10] Kotlin：默认参数
来源：http://kkm.cashguo.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ntd.zdqjudy.top

[T11] Kotlin：协程
来源：http://cur.gzhubu.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://wwn.yonumen.top

[T12] Kotlin：解构声明
来源：http://lrs.iojbl.cn

val (a, b) = Pair(1, 2)
来源：http://ygn.uphjek.com

[T13] Kotlin：只读 Map
来源：http://uuv.wangshuangyany.cn

val m = mapOf("a" to 1)
来源：http://ulf.yongpay.top

[T14] Kotlin：循环
来源：http://ysd.jinqigufen.top

for (i in 1..10) println(i)
来源：http://ssf.wangshuangyany.cn

[T15] Kotlin：接口
来源：http://jwk.fehbvm.com

interface Shape { fun area(): Double }
来源：http://wbg.yj20258888.top

[T16] Swift：Hello World
来源：http://yfi.jlsjyb.cn

print("Hello")
来源：http://rpz.zhaomingkeji.xyz

[T17] Swift：变量与常量
来源：http://jku.gotoacloud.top

var a = 1;  let b = 2
来源：http://msu.redwolf501.top

[T18] Swift：字符串插值
来源：http://ijc.pycfn.com

"值: \(b)"
来源：http://xlk.jianghu66.top

[T19] Swift：可选绑定
来源：http://xhy.nanxinkj.top

if let n = opt { print(n) }
来源：http://lhn.zdbjq.cn

[T20] Swift：数组操作
来源：http://ljy.sufxvd.cn

var a = [1, 2, 3];  a.append(4)
来源：http://rwy.chenjidiqi.icu

[T21] Swift：遍历
来源：http://old.yfazqb.com

for x in a { print(x) }
来源：http://ytg.tarul.cn

[T22] Swift：字典
来源：http://sqe.xziqi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://bva.vqdsnc.cn

[T23] Swift：函数
来源：http://bpo.meibo888.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jui.haohaochexian.top

[T24] Swift：闭包
来源：http://hhy.gaohongyu789.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://uzr.vqdsnc.cn

[T25] Swift：结构体
来源：http://ilw.shanyushiyangkeji.top

struct P { var x: Int }
来源：http://nsn.52xcode.cn

[T26] Swift：类与重写
来源：http://geq.cdnleiting.top

class A: Base { override func f() {} }
来源：http://swc.shangyingyoupin.top

[T27] Swift：错误处理
来源：http://toe.shanyushiyangtech.top

do { try f() } catch { print(error) }
来源：http://juf.nanxuanxn.top

[T28] Swift：枚举
来源：http://vwd.iojbl.cn

enum Color { case red, green }
来源：http://lgu.fktsv.cn

[T29] Swift：guard 提前返回
来源：http://wnn.sxryk.cn

guard let x = opt else { return }
来源：http://paj.vqdsnc.cn

[T30] Swift：协议
来源：http://ogv.xylfe.cn

protocol Shape { func area() -> Double }
来源：http://bpx.zycfv.cn

[T31] Lua：Hello World
来源：http://ohr.hnqzz.top

print("Hello")
来源：http://vpj.c1oappe.top

[T32] Lua：局部变量
来源：http://sqv.daria6918.cn

local a = 1
来源：http://zsm.hfpthk.cn

[T33] Lua：表（数组）
来源：http://qht.vqdsnc.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://njz.quarkkingdee.top

[T34] Lua：遍历表
来源：http://pyk.9152youxi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://dhm.wangshuangyany.cn

[T35] Lua：字典表
来源：http://qhp.chenjidiqi.icu

local d = { a = 1 };  d.b = 2
来源：http://nnw.vehdjk.com

[T36] Lua：函数
来源：http://ziw.xinyue.icu

function add(a, b) return a + b end
来源：http://vxr.jlsjyb.cn

[T37] Lua：字符串拼接
来源：http://roz.tarul.cn

"a" .. "b"
来源：http://yys.xuanzx.com

[T38] Lua：条件
来源：http://arw.cheryme.top

if x > 0 then print("正") end
来源：http://rko.yvedp.cn

[T39] Lua：模式匹配
来源：http://xpd.yvedp.cn

string.find(s, "%d+")
来源：http://rqp.shangyingyoupin.top

[T40] Lua：元表
来源：http://pzt.jinghuilouyu.cn

setmetatable({}, { __index = base })
来源：http://rde.nanxuanxn.top

[T41] Perl：Hello World
来源：http://kwf.52xcode.cn

print "Hello\n";
来源：http://fyx.sxryk.cn

[T42] Perl：变量类型
来源：http://xfg.hnxiangtu.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nky.zhixingplan.top

[T43] Perl：字符串插值
来源：http://dnj.hywenlv.cn

"值: $a"
来源：http://tio.ehwqpu.com

[T44] Perl：条件
来源：http://vcv.gzhubu.top

if ($a > 0) { print "正"; }
来源：http://lnb.0kj1m.cn

[T45] Perl：数组遍历
来源：http://lzp.xylfe.cn

for my $x (@arr) { print $x; }
来源：http://gfw.fzhhl.top

[T46] Perl：哈希操作
来源：http://vpm.mhx1999.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qdf.meibo888.top

[T47] Perl：正则捕获
来源：http://bxh.kuanghao11.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://sbv.yj20258888.top

[T48] Perl：正则替换
来源：http://ktt.tian-w.cn

$s =~ s/old/new/g;
来源：http://pfk.iojbl.cn

[T49] Perl：函数
来源：http://vbk.hammf.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yyc.cheryme.top

[T50] Perl：逐行读文件
来源：http://spf.zdbjq.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://kel.xuanzx.com


<!-- 参考信息 -->