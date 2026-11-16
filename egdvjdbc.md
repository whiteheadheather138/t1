代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://tgj.xinyue.icu

[R48] awk 取指定列
来源：http://xmd.jlsjyb.cn

awk '{print $1, $3}' a.txt
来源：http://nzv.gaohongyu789.top

[R49] awk 带条件
来源：http://osl.hesvh.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dvo.hysaishi.cn

[R50] awk 求和
来源：http://kqr.jinyuanbaomall.cn

awk '{s += $2} END {print s}' a.txt
来源：http://eou.tianlin.xyz

[R51] 排序去重取前几
来源：http://pqf.hywenlv.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://bfa.daria6918.cn

[R52] 统计行数
来源：http://rvw.jinghuilouyu.cn

wc -l a.txt
来源：http://vky.sxryk.cn

[R53] 查看文件头与实时尾
来源：http://dcd.yongpay.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://eiq.nanxinkj.top

[R54] 比较两个文件
来源：http://dgd.cdnleiting.top

diff a.txt b.txt
来源：http://vcg.jinqigufen.top

[R55] 压缩与解压
来源：http://rol.9152youxi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://huc.guowangkeji.top

[R56] 远程拷贝
来源：http://vtt.sysykeji.top

scp file user@host:/path/
来源：http://pmh.hongshengwenyu.top

[R57] 远程执行命令
来源：http://xye.yj202588.top

ssh user@host 'uptime'
来源：http://qdf.jianghu66.top

[R58] 下载文件
来源：http://nqh.ehwqpu.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jpt.zhiwuduotai.top

[R59] 发 POST JSON
来源：http://pte.jyoumei.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hhz.jqgfzy.top

[R60] 只看 HTTP 状态码
来源：http://eav.xylfe.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://itb.yongpay.top

[R61] 磁盘占用
来源：http://wua.ehwqpu.com

df -h;  du -sh *
来源：http://xpc.zhixingplan.top

[R62] 找最占空间的文件
来源：http://jfw.zhengqikj.top

du -ah . | sort -rh | head -10
来源：http://ymb.jinyuanbaomall.cn

[R63] 内存与进程
来源：http://qlg.jqgufenzy.top

free -h;  ps aux | grep nginx
来源：http://orc.aizwys.cn

[R64] 结束进程
来源：http://yue.kuanghao11.cn

kill -9 $(pgrep -f app.py)
来源：http://xlz.hnqzz.top

[R65] 查看端口占用
来源：http://msb.xylfe.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pny.snrcjt.cn

[R66] 定时任务
来源：http://zvz.sysykeji.top

crontab -e;  crontab -l
来源：http://gda.fktsv.cn

[R67] 生成随机十六进制串
来源：http://hza.nanxuanxn.top

openssl rand -hex 16
来源：http://ajl.316326.xyz

[R68] 计算文件校验值
来源：http://bmi.vqdsnc.cn

sha256sum a.txt;  md5sum a.txt
来源：http://olf.yj20258.top

[R69] 生成随机密码
来源：http://lgg.fengsongda.top

head -c 16 /dev/urandom | base64
来源：http://zin.cashguo.top

[R70] 时间戳与互转
来源：http://ogu.jinghuilouyu.cn

date +%s;  date -d @1700000000
来源：http://hdp.xuetiantiany.cn

[R71] 日期格式化
来源：http://fqx.zhoulong.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://lwt.bjfxy.top

[R72] 等待端口就绪
来源：http://cqy.fktsv.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ayr.ctjpmb.com

[R73] 分割大日志
来源：http://dxy.sjlbkw.cn

split -l 1000 big.log part_
来源：http://mgg.9152youxi.cn

[R74] 批量重命名
来源：http://yst.aibaodan.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://chg.yvedp.cn

[R75] 导出环境变量
来源：http://tpi.xuetiantiany.cn

export PATH="$HOME/bin:$PATH"
来源：http://iat.hongshengwenyu.top

[R76] 使用临时文件
来源：http://oue.jianghu66.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yjx.zhoulong.xyz

[R77] 读取用户输入
来源：http://kgc.bjfxy.top

read -rp "请输入: " ans
来源：http://uiy.fehbvm.com

[R78] 交互式菜单
来源：http://mao.chenlongwang.top

select opt in a b c; do echo "$opt"; break; done
来源：http://dqd.cashguo.top

[R79] 解析命令行选项
来源：http://zgk.fehbvm.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zzw.52xcode.cn

[R80] 查看脚本执行耗时
来源：http://kxx.shanyushiyangtech.top

time ./run.sh
来源：http://ulz.shanyushiyangkeji.top

================================================================================
来源：http://nce.gotoacloud.top

S. C / C++ 专题
来源：http://xyp.cashguo.top

================================================================================
来源：http://erp.316326.xyz

[S01] C：Hello World
来源：http://oco.xinyue.icu

#include <stdio.h>
来源：http://diz.svipenyu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://rrm.yuanzhike.top

[S02] C：变量与格式化输出
来源：http://nwo.daxiang520.top

int a = 10; printf("%d\n", a);
来源：http://hzt.wangshuangyany.cn

[S03] C：读入整数
来源：http://bmr.bbcook.cn

int x; scanf("%d", &x);
来源：http://yjk.bbcook.cn

[S04] C：字符串复制
来源：http://hoj.xuanzx.com

char dst[32]; strcpy(dst, "hi");
来源：http://ngu.tian-w.cn

[S05] C：字符串长度
来源：http://dbu.chenjidiqi.icu

strlen(s)
来源：http://qsy.shanyushiyangtech.top

[S06] C：字符串比较
来源：http://wjk.ydzc1.top

strcmp(a, b) == 0
来源：http://xxi.zhongyouzk.top

[S07] C：数组遍历求和
来源：http://ggt.yanxiufei.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rdv.sjlbkw.cn

[S08] C：动态内存分配与释放
来源：http://duo.gaohongyu789.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hng.xuanzx.com

[S09] C：结构体定义与初始化
来源：http://lit.ybcxt.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://msg.sxryk.cn

[S10] C：指针与解引用
来源：http://ipt.jinyuanbaomall.cn

int *p = &a;  *p = 5;
来源：http://mpw.birdmap.top

[S11] C：逐行读文件
来源：http://ixx.sweek.top

FILE *f = fopen("a.txt", "r");
来源：http://dso.xinyue.icu

while (fgets(buf, sizeof buf, f)) { }
来源：http://hne.hammf.cn

fclose(f);
来源：http://mvx.fzhhl.top

[S12] C：写文件
来源：http://wgg.vehdjk.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://stn.hammf.cn

[S13] C：宏定义
来源：http://aee.hysaishi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vvf.ydjk.org.cn

[S14] C：枚举
来源：http://sdf.cashguo.top

enum Color { RED, GREEN, BLUE };
来源：http://pnf.daria6918.cn

[S15] C：类型转换
来源：http://cpm.chenzaomai.com

(double) a / b
来源：http://gtz.hnxiangtu.top

[S16] C：位操作置位
来源：http://ejm.yj202588.top

x |= (1 << 3);
来源：http://uyw.bjfxy.top

[S17] C：安全拼接字符串
来源：http://vsj.havefunace.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fco.shanyushiyangkeji.top

[S18] C：命令行参数
来源：http://low.dianchejie.cn

int main(int argc, char **argv)
来源：http://qiq.smart0.xyz

[S19] C：快速排序
来源：http://bcj.jinqigufen.top

qsort(a, n, sizeof(int), cmp);
来源：http://ucw.yonumen.top

[S20] C：二分查找
来源：http://kke.hongshengwenyu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uvh.gotoacloud.top

[S21] C：字符类别判断
来源：http://nxl.jianghu66.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lxq.yfazqb.com

[S22] C：字符串转数字
来源：http://wjs.yfazqb.com

atoi("42");  strtod("3.14", NULL);
来源：http://ron.hcnkem.com

[S23] C：随机数
来源：http://tfs.tarul.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://lws.jinqigufen.top

[S24] C：获取本地时间
来源：http://ixj.wangdashe.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gew.birdmap.top

[S25] C：内存拷贝
来源：http://kyh.svipenyu.cn

memcpy(dst, src, n);
来源：http://kwd.52xcode.cn

[S26] C：内存清零
来源：http://zpi.cashguo.top

memset(a, 0, sizeof a);
来源：http://svg.yfazqb.com

[S27] C：定义常量
来源：http://yfa.xuetiantiany.cn

const double PI = 3.14159;
来源：http://zwn.haohaochexian.top

[S28] C：静态变量
来源：http://oej.zhongyouzk.top

static int counter = 0;
来源：http://nmx.316326.xyz

[S29] C：变参函数
来源：http://gnf.xingfuxueyuan.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mnu.kuanghao11.cn

[S30] C：头文件保护
来源：http://tij.aizwys.cn

#ifndef X_H
来源：http://qlz.gaohongyu789.top

#define X_H
来源：http://iki.jinghuilouyu.cn

#endif
来源：http://qnp.0kj1m.cn

[S31] C++：Hello World
来源：http://grp.shanyushiyangkeji.top

#include <iostream>
来源：http://xrb.yueranfly.top

int main() { std::cout << "Hello\n"; }
来源：http://qyd.aibaodan.cn

[S32] C++：字符串
来源：http://jzp.daria6918.cn

std::string s = "hi";  s += "!";
来源：http://kxo.cashguo.top

[S33] C++：vector 增删
来源：http://fwv.chenjidiqi.icu

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hqi.sjlbkw.cn

[S34] C++：遍历 vector
来源：http://psw.shangyingyoupin.top

for (auto &x : v) { std::cout << x; }
来源：http://blo.pengpengdd.cyou

[S35] C++：map
来源：http://ole.jqgfzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lzo.shzxlz.cn

[S36] C++：unordered_map
来源：http://ecs.quarkkingdee.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hsn.gotoacloud.top

[S37] C++：set
来源：http://jxd.hnqzz.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vzb.gotoacloud.top

[S38] C++：排序
来源：http://bzg.yj20258.top

std::sort(v.begin(), v.end());
来源：http://sas.iojbl.cn

[S39] C++：自定义比较器排序
来源：http://fym.sweek.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xis.birdmap.top

[S40] C++：查找元素
来源：http://zvp.fanxiaobao.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fzg.pycfn.com

[S41] C++：类与构造函数
来源：http://vyu.uphjek.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wxz.sysykeji.top

[S42] C++：继承与虚函数
来源：http://rjs.aibaodan.cn

class B : public Base { public: void f() override {} };
来源：http://gtb.yangfankeji.com

[S43] C++：智能指针
来源：http://xas.gzhubu.top

auto p = std::make_unique<int>(5);
来源：http://ytp.hesvh.cn

[S44] C++：引用传参
来源：http://nmq.wangshuangyany.cn

void inc(int &x) { ++x; }
来源：http://pbq.cashguo.top

[S45] C++：lambda
来源：http://alw.uphjek.com

auto add = [](int a, int b) { return a + b; };
来源：http://cek.snrcjt.cn

[S46] C++：函数模板
来源：http://nvt.hesvh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://los.zhiwuduotai.top

[S47] C++：结构化绑定遍历
来源：http://aan.svipenyu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://usp.jlsjyb.cn

[S48] C++：逐行读文件
来源：http://mye.c1oappe.top

std::ifstream in("a.txt");  std::string line;
来源：http://cxo.yj202588.top

while (std::getline(in, line)) { }
来源：http://ftd.xylfe.cn

[S49] C++：写文件
来源：http://moq.yuanzhike.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gpl.feifeiyinyue.top

[S50] C++：格式化数字
来源：http://osz.quarkkingdee.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bnt.hesvh.cn

[S51] C++：显式类型转换
来源：http://uky.ehwqpu.com

static_cast<double>(a) / b
来源：http://qmt.jiagoushi.top

[S52] C++：const 与 noexcept
来源：http://vcb.yuanzhike.top

int size() const noexcept { return n_; }
来源：http://fur.guowangkeji.top

[S53] C++：移动语义
来源：http://cnv.aibaodan.cn

std::vector<int> w = std::move(v);
来源：http://ywy.ydzc1.top

[S54] C++：异常处理
来源：http://rug.cashguo.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rib.yj20258888.top

[S55] C++：结构化绑定
来源：http://wwg.yvedp.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://tgs.tanke756.top

[S56] C++：optional
来源：http://jbo.fzhhl.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://iyh.yongpay.top

[S57] C++：编译期常量
来源：http://qqc.bbcook.cn

constexpr int N = 10;
来源：http://voa.zycfv.cn

[S58] C++：命名空间
来源：http://nib.iojbl.cn

namespace ns { int f() { return 1; } }
来源：http://gps.hnxiangtu.top

[S59] C++：静态断言
来源：http://vxv.fehbvm.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jrk.nanxinkj.top

[S60] C++：遍历并删除元素
来源：http://xgw.guannengcc.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pct.9152youxi.cn

================================================================================
来源：http://oib.nanxuanxn.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lgr.hesvh.cn

================================================================================
来源：http://hjk.epnwcf.com

[T01] Kotlin：Hello World
来源：http://oua.chenlongwang.top

println("Hello")
来源：http://vuj.zhaomingkeji.xyz

[T02] Kotlin：变量
来源：http://ixy.jyoumei.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://srr.tianlin.xyz

[T03] Kotlin：字符串模板
来源：http://uxq.nanxuanxn.top

"值: $b"
来源：http://vre.jlsjyb.cn

[T04] Kotlin：空安全
来源：http://goz.ctjpmb.com

val n: String? = null;  n?.length
来源：http://zyt.smart0.xyz

[T05] Kotlin：when 表达式
来源：http://glx.daxiang520.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sqd.yvedp.cn

[T06] Kotlin：集合映射
来源：http://wfu.guowangkeji.top

listOf(1, 2, 3).map { it * 2 }
来源：http://tbs.gogol.net.cn

[T07] Kotlin：集合过滤
来源：http://ebt.9152youxi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ifv.zdbjq.cn

[T08] Kotlin：数据类
来源：http://qec.jlsjyb.cn

data class User(val name: String, val age: Int)
来源：http://wyf.dashuyun.cn

[T09] Kotlin：扩展函数
来源：http://zyi.iojbl.cn

fun String.exclaim() = this + "!"
来源：http://jwq.jinqigufen.top

[T10] Kotlin：默认参数
来源：http://iht.chenlongwang.top

fun greet(name: String = "World") = "Hi $name"
来源：http://xca.xylfe.cn

[T11] Kotlin：协程
来源：http://aud.wangshuangyany.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hgp.fehbvm.com

[T12] Kotlin：解构声明
来源：http://qby.ivvv.top

val (a, b) = Pair(1, 2)
来源：http://qnz.pycfn.com

[T13] Kotlin：只读 Map
来源：http://xyk.hnxiangtu.top

val m = mapOf("a" to 1)
来源：http://snj.ydzc1.top

[T14] Kotlin：循环
来源：http://cdi.jinghuilouyu.cn

for (i in 1..10) println(i)
来源：http://kjp.guowangkeji.top

[T15] Kotlin：接口
来源：http://lso.xingfuxueyuan.xyz

interface Shape { fun area(): Double }
来源：http://bql.pycfn.com

[T16] Swift：Hello World
来源：http://dph.dashuyun.cn

print("Hello")
来源：http://iev.hywenlv.cn

[T17] Swift：变量与常量
来源：http://byx.fktsv.cn

var a = 1;  let b = 2
来源：http://qxo.nanxinkj.top

[T18] Swift：字符串插值
来源：http://rca.316326.xyz

"值: \(b)"
来源：http://rte.zdqjudy.top

[T19] Swift：可选绑定
来源：http://syr.jinyuanbaomall.cn

if let n = opt { print(n) }
来源：http://vdg.cqqwz.cn

[T20] Swift：数组操作
来源：http://gfr.aibaodan.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mhr.hammf.cn

[T21] Swift：遍历
来源：http://zbb.shanyushiyangkeji.top

for x in a { print(x) }
来源：http://aym.hnxiangtu.top

[T22] Swift：字典
来源：http://ptm.zdqjudy.top

var d = ["a": 1];  d["b"] = 2
来源：http://zca.jiagoushi.top

[T23] Swift：函数
来源：http://aca.yj20258888.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kne.chenzaomai.com

[T24] Swift：闭包
来源：http://rcj.wangshuangyany.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ejo.hywenlv.cn

[T25] Swift：结构体
来源：http://nln.smart0.xyz

struct P { var x: Int }
来源：http://qwy.nanxuanxn.top

[T26] Swift：类与重写
来源：http://hdj.andypj.xyz

class A: Base { override func f() {} }
来源：http://dgo.cashguo.top

[T27] Swift：错误处理
来源：http://ncm.snrcjt.cn

do { try f() } catch { print(error) }
来源：http://pzz.0kj1m.cn

[T28] Swift：枚举
来源：http://vct.havefunace.top

enum Color { case red, green }
来源：http://oov.shuidangran.top

[T29] Swift：guard 提前返回
来源：http://ldb.snrcjt.cn

guard let x = opt else { return }
来源：http://gda.guannengcc.top

[T30] Swift：协议
来源：http://vsa.yueranfly.top

protocol Shape { func area() -> Double }
来源：http://eho.feifeiyinyue.top

[T31] Lua：Hello World
来源：http://okf.9152youxi.cn

print("Hello")
来源：http://uil.yj202588.top

[T32] Lua：局部变量
来源：http://cvi.jinqigfzy.top

local a = 1
来源：http://aol.hcnkem.com

[T33] Lua：表（数组）
来源：http://bys.yj202588.top

local t = {1, 2, 3};  t[4] = 4
来源：http://jux.xylfe.cn

[T34] Lua：遍历表
来源：http://ozc.hnqzz.top

for i, v in ipairs(t) do print(i, v) end
来源：http://qem.316326.xyz

[T35] Lua：字典表
来源：http://yox.chenlongwang.top

local d = { a = 1 };  d.b = 2
来源：http://gcy.epnwcf.com

[T36] Lua：函数
来源：http://lvu.zhiwuduotai.top

function add(a, b) return a + b end
来源：http://ufb.smart0.xyz

[T37] Lua：字符串拼接
来源：http://xzy.hnxiangtu.top

"a" .. "b"
来源：http://kep.shanyushiyangkeji.top

[T38] Lua：条件
来源：http://ykg.hcnkem.com

if x > 0 then print("正") end
来源：http://vhk.yfazqb.com

[T39] Lua：模式匹配
来源：http://hrs.hywenlv.cn

string.find(s, "%d+")
来源：http://erk.daxiang520.top

[T40] Lua：元表
来源：http://zgf.ctjpmb.com

setmetatable({}, { __index = base })
来源：http://ahf.ehwqpu.com

[T41] Perl：Hello World
来源：http://dwy.jinqigufen.top

print "Hello\n";
来源：http://nrq.wangshuangyany.cn

[T42] Perl：变量类型
来源：http://mse.cqqwz.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rkk.zhaomingkeji.xyz

[T43] Perl：字符串插值
来源：http://ghv.guannengcc.top

"值: $a"
来源：http://szs.fanxiaobao.xyz

[T44] Perl：条件
来源：http://dmk.zhoulong.xyz

if ($a > 0) { print "正"; }
来源：http://iez.zdqjudy.top

[T45] Perl：数组遍历
来源：http://grs.zhiwuduotai.top

for my $x (@arr) { print $x; }
来源：http://gki.zhixingplan.top

[T46] Perl：哈希操作
来源：http://kqv.iojbl.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rcc.wangdashe.top

[T47] Perl：正则捕获
来源：http://ejy.svipenyu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xcv.daria6918.cn

[T48] Perl：正则替换
来源：http://ctd.feifeiyinyue.top

$s =~ s/old/new/g;
来源：http://lyo.ehwqpu.com

[T49] Perl：函数
来源：http://hyk.zycfv.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vxx.jqgufenzy.top

[T50] Perl：逐行读文件
来源：http://ckr.daxiang520.top

open my $fh, "<", "a.txt" or die $!;
来源：http://anv.hysaishi.cn


<!-- 参考信息 -->