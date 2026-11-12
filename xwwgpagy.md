代发 wailian999

find . -name "*.log" -type f
来源：http://jrk.zhijiandao.cn

[R44] 按修改时间查找
来源：http://sip.ppjwa.cn

find . -mtime -7 -type f
来源：http://xjz.ybcxt.top

[R45] 批量删除
来源：http://vgj.0kj1m.cn

find . -name "*.tmp" -delete
来源：http://rgy.vehdjk.com

[R46] 递归替换文件内容
来源：http://yzo.zhengqikj.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pdp.fehbvm.com

[R47] sed 单行替换
来源：http://mpf.redwolf501.top

sed -i 's/foo/bar/g' a.txt
来源：http://bmj.zhixingplan.top

[R48] awk 取指定列
来源：http://spr.fktsv.cn

awk '{print $1, $3}' a.txt
来源：http://phn.smart0.xyz

[R49] awk 带条件
来源：http://ngc.jqgfzy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://osi.kuanghao11.cn

[R50] awk 求和
来源：http://ulz.shzxlz.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hdi.chenlongwang.top

[R51] 排序去重取前几
来源：http://lhg.gogol.net.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://wze.kuanghao11.cn

[R52] 统计行数
来源：http://rzy.yongpay.top

wc -l a.txt
来源：http://xse.dianchejie.cn

[R53] 查看文件头与实时尾
来源：http://yyo.yvedp.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hxb.jianghu66.top

[R54] 比较两个文件
来源：http://esw.tanke756.top

diff a.txt b.txt
来源：http://ezx.wangdashe.top

[R55] 压缩与解压
来源：http://llj.xingfuxueyuan.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gzk.guannengcc.top

[R56] 远程拷贝
来源：http://nwu.chenjidiqi.icu

scp file user@host:/path/
来源：http://ufi.cdnleiting.top

[R57] 远程执行命令
来源：http://utg.hnxiangtu.top

ssh user@host 'uptime'
来源：http://xlo.zhiwuduotai.top

[R58] 下载文件
来源：http://bap.zycfv.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uas.sjlbkw.cn

[R59] 发 POST JSON
来源：http://sos.nanxinkj.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cuz.zycfv.cn

[R60] 只看 HTTP 状态码
来源：http://dyc.cqqwz.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ogx.havefunace.top

[R61] 磁盘占用
来源：http://wjb.vqdsnc.cn

df -h;  du -sh *
来源：http://qsj.yangfankeji.com

[R62] 找最占空间的文件
来源：http://dxx.hcnkem.com

du -ah . | sort -rh | head -10
来源：http://yuo.fanxiaobao.xyz

[R63] 内存与进程
来源：http://xhl.daxiang520.top

free -h;  ps aux | grep nginx
来源：http://zkr.cucudq.cn

[R64] 结束进程
来源：http://kdp.hammf.cn

kill -9 $(pgrep -f app.py)
来源：http://ftn.yuxming.cn

[R65] 查看端口占用
来源：http://vkz.nanxinkj.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dqg.nanxinkj.top

[R66] 定时任务
来源：http://tua.guannengcc.top

crontab -e;  crontab -l
来源：http://uub.yongpay.top

[R67] 生成随机十六进制串
来源：http://knt.meibo888.top

openssl rand -hex 16
来源：http://zln.shanyushiyangtech.top

[R68] 计算文件校验值
来源：http://jqd.zdbjq.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xhu.zycfv.cn

[R69] 生成随机密码
来源：http://mfi.hywenlv.cn

head -c 16 /dev/urandom | base64
来源：http://sfd.hywenlv.cn

[R70] 时间戳与互转
来源：http://luz.zhiwuduotai.top

date +%s;  date -d @1700000000
来源：http://rha.yonumen.top

[R71] 日期格式化
来源：http://eff.fktsv.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qot.pycfn.com

[R72] 等待端口就绪
来源：http://skc.havefunace.top

until nc -z localhost 3306; do sleep 1; done
来源：http://wkj.xylfe.cn

[R73] 分割大日志
来源：http://ycw.yj20258.top

split -l 1000 big.log part_
来源：http://pra.ehwqpu.com

[R74] 批量重命名
来源：http://jmp.pengpengdd.cyou

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zqe.dianchejie.cn

[R75] 导出环境变量
来源：http://vut.zhijiandao.cn

export PATH="$HOME/bin:$PATH"
来源：http://osy.jlsjyb.cn

[R76] 使用临时文件
来源：http://hjf.yvedp.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://laf.sweek.top

[R77] 读取用户输入
来源：http://fir.52xcode.cn

read -rp "请输入: " ans
来源：http://fbv.ctjpmb.com

[R78] 交互式菜单
来源：http://fox.mhx1999.top

select opt in a b c; do echo "$opt"; break; done
来源：http://fcy.xingfuxueyuan.xyz

[R79] 解析命令行选项
来源：http://fql.52xcode.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://atk.chenlongwang.top

[R80] 查看脚本执行耗时
来源：http://cxx.xziqi.cn

time ./run.sh
来源：http://blv.zhixingplan.top

================================================================================
来源：http://rgj.jqgufenzy.top

S. C / C++ 专题
来源：http://glg.hysaishi.cn

================================================================================
来源：http://ceu.jqgufenzy.top

[S01] C：Hello World
来源：http://pde.haohaochexian.top

#include <stdio.h>
来源：http://xlj.cashguo.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://gcc.hesvh.cn

[S02] C：变量与格式化输出
来源：http://qll.ivvv.top

int a = 10; printf("%d\n", a);
来源：http://cqf.jqgfzy.top

[S03] C：读入整数
来源：http://kcd.svipenyu.cn

int x; scanf("%d", &x);
来源：http://fez.vehdjk.com

[S04] C：字符串复制
来源：http://gsi.xingfuxueyuan.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://jik.hcnkem.com

[S05] C：字符串长度
来源：http://sxw.xingfuxueyuan.xyz

strlen(s)
来源：http://fkv.jinqigfzy.top

[S06] C：字符串比较
来源：http://qlh.guowangkeji.top

strcmp(a, b) == 0
来源：http://rkg.hongshengwenyu.top

[S07] C：数组遍历求和
来源：http://ldo.aibaodan.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yyc.yangfankeji.com

[S08] C：动态内存分配与释放
来源：http://tit.ywan-chungtsiang.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uob.zhijiandao.cn

[S09] C：结构体定义与初始化
来源：http://kik.yangfankeji.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://eaz.chenjidiqi.icu

[S10] C：指针与解引用
来源：http://ikr.jinyuanbaomall.cn

int *p = &a;  *p = 5;
来源：http://jwa.yfazqb.com

[S11] C：逐行读文件
来源：http://ecr.vqdsnc.cn

FILE *f = fopen("a.txt", "r");
来源：http://xxo.yuanzhike.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://wnv.hnxiangtu.top

fclose(f);
来源：http://bmf.zhengqikj.top

[S12] C：写文件
来源：http://sng.zdbjq.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tvq.zhiwuduotai.top

[S13] C：宏定义
来源：http://ybw.9152youxi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://smh.sysykeji.top

[S14] C：枚举
来源：http://jac.jqgfzy.top

enum Color { RED, GREEN, BLUE };
来源：http://wpu.shanyushiyangkeji.top

[S15] C：类型转换
来源：http://hea.yongpay.top

(double) a / b
来源：http://usn.jinqigfzy.top

[S16] C：位操作置位
来源：http://qdj.yuanzhike.top

x |= (1 << 3);
来源：http://yya.havefunace.top

[S17] C：安全拼接字符串
来源：http://jlm.sweek.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wnk.redwolf501.top

[S18] C：命令行参数
来源：http://uuz.cashguo.top

int main(int argc, char **argv)
来源：http://qmr.wangdashe.top

[S19] C：快速排序
来源：http://sri.yonumen.top

qsort(a, n, sizeof(int), cmp);
来源：http://umk.yvedp.cn

[S20] C：二分查找
来源：http://ugf.havefunace.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://eja.fanxiaobao.xyz

[S21] C：字符类别判断
来源：http://why.smart0.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sup.gaohongyu789.top

[S22] C：字符串转数字
来源：http://rub.jinyuanbaomall.cn

atoi("42");  strtod("3.14", NULL);
来源：http://nit.ivvv.top

[S23] C：随机数
来源：http://rfe.yuxming.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://imo.kuanghao11.cn

[S24] C：获取本地时间
来源：http://okv.epnwcf.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kjp.jianghu66.top

[S25] C：内存拷贝
来源：http://gdl.nwbrower.top

memcpy(dst, src, n);
来源：http://bei.zhaomingkeji.xyz

[S26] C：内存清零
来源：http://ezu.havefunace.top

memset(a, 0, sizeof a);
来源：http://byk.guannengcc.top

[S27] C：定义常量
来源：http://rqv.wangshuangyany.cn

const double PI = 3.14159;
来源：http://new.feifeiyinyue.top

[S28] C：静态变量
来源：http://kew.chenjidiqi.icu

static int counter = 0;
来源：http://agi.cashguo.top

[S29] C：变参函数
来源：http://cps.jqgufenzy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://cmg.zhijiandao.cn

[S30] C：头文件保护
来源：http://oup.feifeiyinyue.top

#ifndef X_H
来源：http://ldy.hesvh.cn

#define X_H
来源：http://jao.52xcode.cn

#endif
来源：http://osq.hcnkem.com

[S31] C++：Hello World
来源：http://izu.chenzaomai.com

#include <iostream>
来源：http://pgs.ivvv.top

int main() { std::cout << "Hello\n"; }
来源：http://ued.zhijiandao.cn

[S32] C++：字符串
来源：http://fdw.cheryme.top

std::string s = "hi";  s += "!";
来源：http://fnl.aizwys.cn

[S33] C++：vector 增删
来源：http://epg.tanke756.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rhv.chenzaomai.com

[S34] C++：遍历 vector
来源：http://hll.jinqigfzy.top

for (auto &x : v) { std::cout << x; }
来源：http://bfx.zhengqikj.top

[S35] C++：map
来源：http://rfj.chenlongwang.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sxm.fanxiaobao.xyz

[S36] C++：unordered_map
来源：http://zkq.yfazqb.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pyj.nanxuanxn.top

[S37] C++：set
来源：http://gzh.xylfe.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zbn.sufxvd.cn

[S38] C++：排序
来源：http://cpf.meibo888.top

std::sort(v.begin(), v.end());
来源：http://tfz.yuanzhike.top

[S39] C++：自定义比较器排序
来源：http://dyz.ehwqpu.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://eli.52xcode.cn

[S40] C++：查找元素
来源：http://iui.zhoulong.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://efn.yvedp.cn

[S41] C++：类与构造函数
来源：http://jym.chenjidiqi.icu

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yrv.wangdashe.top

[S42] C++：继承与虚函数
来源：http://cjq.ybcxt.top

class B : public Base { public: void f() override {} };
来源：http://bhu.epnwcf.com

[S43] C++：智能指针
来源：http://abx.c1oappe.top

auto p = std::make_unique<int>(5);
来源：http://vmg.daria6918.cn

[S44] C++：引用传参
来源：http://vog.daxiang520.top

void inc(int &x) { ++x; }
来源：http://nfp.epnwcf.com

[S45] C++：lambda
来源：http://nsv.jinqigfzy.top

auto add = [](int a, int b) { return a + b; };
来源：http://djy.dianchejie.cn

[S46] C++：函数模板
来源：http://kzl.daria6918.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fzj.nanxinkj.top

[S47] C++：结构化绑定遍历
来源：http://noe.wangdashe.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gav.sjlbkw.cn

[S48] C++：逐行读文件
来源：http://wdu.shanyushiyangkeji.top

std::ifstream in("a.txt");  std::string line;
来源：http://gkx.ivvv.top

while (std::getline(in, line)) { }
来源：http://lmf.hywenlv.cn

[S49] C++：写文件
来源：http://owm.jqgfzy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://spx.sweek.top

[S50] C++：格式化数字
来源：http://zjm.zycfv.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cnf.nanxinkj.top

[S51] C++：显式类型转换
来源：http://yjc.zycfv.cn

static_cast<double>(a) / b
来源：http://kpy.sxryk.cn

[S52] C++：const 与 noexcept
来源：http://vce.kuanghao11.cn

int size() const noexcept { return n_; }
来源：http://atp.xylfe.cn

[S53] C++：移动语义
来源：http://pnr.zhengqikj.top

std::vector<int> w = std::move(v);
来源：http://row.fengsongda.top

[S54] C++：异常处理
来源：http://ywu.birdmap.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vtb.quarkkingdee.top

[S55] C++：结构化绑定
来源：http://kbr.tianlin.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://jhs.bjfxy.top

[S56] C++：optional
来源：http://fav.nanxuanxn.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://snu.fehbvm.com

[S57] C++：编译期常量
来源：http://ddu.jyoumei.cn

constexpr int N = 10;
来源：http://qow.zhixingplan.top

[S58] C++：命名空间
来源：http://pcb.fehbvm.com

namespace ns { int f() { return 1; } }
来源：http://efl.xingfuxueyuan.xyz

[S59] C++：静态断言
来源：http://amg.yj202588.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zgh.zhengqikj.top

[S60] C++：遍历并删除元素
来源：http://woq.shangyingyoupin.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://szi.c1oappe.top

================================================================================
来源：http://esf.aibaodan.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://erw.birdmap.top

================================================================================
来源：http://hdl.yj20258888.top

[T01] Kotlin：Hello World
来源：http://bbk.0kj1m.cn

println("Hello")
来源：http://ywd.xuanzx.com

[T02] Kotlin：变量
来源：http://vbf.shzxlz.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://drk.mhx1999.top

[T03] Kotlin：字符串模板
来源：http://scm.smart0.xyz

"值: $b"
来源：http://hgm.epnwcf.com

[T04] Kotlin：空安全
来源：http://rih.yanxiufei.cn

val n: String? = null;  n?.length
来源：http://prn.redwolf501.top

[T05] Kotlin：when 表达式
来源：http://ppl.xuetiantiany.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dxc.ydzc1.top

[T06] Kotlin：集合映射
来源：http://cvl.cheryme.top

listOf(1, 2, 3).map { it * 2 }
来源：http://crx.tarul.cn

[T07] Kotlin：集合过滤
来源：http://yeq.ywan-chungtsiang.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://pcu.xingfuxueyuan.xyz

[T08] Kotlin：数据类
来源：http://nqh.hongshengwenyu.top

data class User(val name: String, val age: Int)
来源：http://ndv.9152youxi.cn

[T09] Kotlin：扩展函数
来源：http://bet.sxryk.cn

fun String.exclaim() = this + "!"
来源：http://yeq.guannengcc.top

[T10] Kotlin：默认参数
来源：http://ihv.xuanzx.com

fun greet(name: String = "World") = "Hi $name"
来源：http://aif.ppjwa.cn

[T11] Kotlin：协程
来源：http://frn.chenlongwang.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://iso.yj20258888.top

[T12] Kotlin：解构声明
来源：http://bpe.xuanzx.com

val (a, b) = Pair(1, 2)
来源：http://ywp.ivvv.top

[T13] Kotlin：只读 Map
来源：http://hzw.52xcode.cn

val m = mapOf("a" to 1)
来源：http://pko.daxiang520.top

[T14] Kotlin：循环
来源：http://qhk.nanxuanxn.top

for (i in 1..10) println(i)
来源：http://vij.guannengcc.top

[T15] Kotlin：接口
来源：http://eaq.gaohongyu789.top

interface Shape { fun area(): Double }
来源：http://zkm.vqdsnc.cn

[T16] Swift：Hello World
来源：http://yzk.zdbjq.cn

print("Hello")
来源：http://xow.gotoacloud.top

[T17] Swift：变量与常量
来源：http://tmx.ehwqpu.com

var a = 1;  let b = 2
来源：http://vgz.smart0.xyz

[T18] Swift：字符串插值
来源：http://tku.zdbjq.cn

"值: \(b)"
来源：http://lhx.c1oappe.top

[T19] Swift：可选绑定
来源：http://cbm.havefunace.top

if let n = opt { print(n) }
来源：http://gga.fengsongda.top

[T20] Swift：数组操作
来源：http://llw.jianghu66.top

var a = [1, 2, 3];  a.append(4)
来源：http://mbe.ywan-chungtsiang.top

[T21] Swift：遍历
来源：http://zku.jiagoushi.top

for x in a { print(x) }
来源：http://res.gaohongyu789.top

[T22] Swift：字典
来源：http://gsf.dashuyun.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mek.zhixingplan.top

[T23] Swift：函数
来源：http://oru.epnwcf.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://svy.xuanzx.com

[T24] Swift：闭包
来源：http://hqn.smart0.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://obh.nanxuanxn.top

[T25] Swift：结构体
来源：http://tkc.hfpthk.cn

struct P { var x: Int }
来源：http://npa.gogol.net.cn

[T26] Swift：类与重写
来源：http://wim.zycfv.cn

class A: Base { override func f() {} }
来源：http://nyf.shangyingyoupin.top

[T27] Swift：错误处理
来源：http://los.jinqigfzy.top

do { try f() } catch { print(error) }
来源：http://oxm.shangyingyoupin.top

[T28] Swift：枚举
来源：http://jxu.nwbrower.top

enum Color { case red, green }
来源：http://vte.jyoumei.cn

[T29] Swift：guard 提前返回
来源：http://kzu.svipenyu.cn

guard let x = opt else { return }
来源：http://ehj.andypj.xyz

[T30] Swift：协议
来源：http://rbf.jqgufenzy.top

protocol Shape { func area() -> Double }
来源：http://hxi.xuanzx.com

[T31] Lua：Hello World
来源：http://wsh.hongshengwenyu.top

print("Hello")
来源：http://vrp.shuidangran.top

[T32] Lua：局部变量
来源：http://iby.sweek.top

local a = 1
来源：http://ytq.daria6918.cn

[T33] Lua：表（数组）
来源：http://mom.316326.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://kcb.chenlongwang.top

[T34] Lua：遍历表
来源：http://hxp.cdnleiting.top

for i, v in ipairs(t) do print(i, v) end
来源：http://jke.xylfe.cn

[T35] Lua：字典表
来源：http://ylv.sxryk.cn

local d = { a = 1 };  d.b = 2
来源：http://ctq.fanxiaobao.xyz

[T36] Lua：函数
来源：http://etc.xinyue.icu

function add(a, b) return a + b end
来源：http://lzk.zhijiandao.cn

[T37] Lua：字符串拼接
来源：http://svv.52xcode.cn

"a" .. "b"
来源：http://ght.yvedp.cn

[T38] Lua：条件
来源：http://wcl.jyoumei.cn

if x > 0 then print("正") end
来源：http://whk.hcnkem.com

[T39] Lua：模式匹配
来源：http://uzp.ywan-chungtsiang.top

string.find(s, "%d+")
来源：http://sdl.nanxinkj.top

[T40] Lua：元表
来源：http://kxa.hysaishi.cn

setmetatable({}, { __index = base })
来源：http://crd.fengsongda.top

[T41] Perl：Hello World
来源：http://rwm.jianghu66.top

print "Hello\n";
来源：http://jnw.ydzc1.top

[T42] Perl：变量类型
来源：http://vzu.yuanzhike.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mqx.dashuyun.cn

[T43] Perl：字符串插值
来源：http://jwe.yvedp.cn

"值: $a"
来源：http://cgh.nanxuanxn.top

[T44] Perl：条件
来源：http://ufx.zhoulong.xyz

if ($a > 0) { print "正"; }
来源：http://ycx.c1oappe.top

[T45] Perl：数组遍历
来源：http://xpq.ydzc1.top

for my $x (@arr) { print $x; }
来源：http://rgq.yj20258.top

[T46] Perl：哈希操作
来源：http://ahl.zhixingplan.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rrd.zhijiandao.cn


<!-- 参考信息 -->