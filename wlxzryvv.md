代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://zsa.pycfn.com

[R48] awk 取指定列
来源：http://hpk.jlsjyb.cn

awk '{print $1, $3}' a.txt
来源：http://vfk.cashguo.top

[R49] awk 带条件
来源：http://xnd.sufxvd.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nmy.bjfxy.top

[R50] awk 求和
来源：http://odf.aibaodan.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ovi.gotoacloud.top

[R51] 排序去重取前几
来源：http://oyt.nanxinkj.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ppp.birdmap.top

[R52] 统计行数
来源：http://tqn.yuanzhike.top

wc -l a.txt
来源：http://gol.chenlongwang.top

[R53] 查看文件头与实时尾
来源：http://sfq.cheryme.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vhy.zycfv.cn

[R54] 比较两个文件
来源：http://fiy.fzhhl.top

diff a.txt b.txt
来源：http://sie.shzxlz.cn

[R55] 压缩与解压
来源：http://ecl.zdbjq.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fve.cqqwz.cn

[R56] 远程拷贝
来源：http://mxc.chenjidiqi.icu

scp file user@host:/path/
来源：http://jkn.nanxinkj.top

[R57] 远程执行命令
来源：http://lcw.jiagoushi.top

ssh user@host 'uptime'
来源：http://dnj.zdqjudy.top

[R58] 下载文件
来源：http://bpk.9152youxi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fps.sjlbkw.cn

[R59] 发 POST JSON
来源：http://tob.fktsv.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nps.jinqigufen.top

[R60] 只看 HTTP 状态码
来源：http://wpp.hesvh.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://inc.jinyuanbaomall.cn

[R61] 磁盘占用
来源：http://cjs.yj202588.top

df -h;  du -sh *
来源：http://vgl.0kj1m.cn

[R62] 找最占空间的文件
来源：http://gbt.52xcode.cn

du -ah . | sort -rh | head -10
来源：http://zca.xuetiantiany.cn

[R63] 内存与进程
来源：http://gko.9152youxi.cn

free -h;  ps aux | grep nginx
来源：http://vuz.daxiang520.top

[R64] 结束进程
来源：http://qhf.yvedp.cn

kill -9 $(pgrep -f app.py)
来源：http://mds.andypj.xyz

[R65] 查看端口占用
来源：http://osw.bbcook.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wjk.0kj1m.cn

[R66] 定时任务
来源：http://pol.aibaodan.cn

crontab -e;  crontab -l
来源：http://vpe.svipenyu.cn

[R67] 生成随机十六进制串
来源：http://ijg.zhaomingkeji.xyz

openssl rand -hex 16
来源：http://wsl.andypj.xyz

[R68] 计算文件校验值
来源：http://dli.yongpay.top

sha256sum a.txt;  md5sum a.txt
来源：http://exu.cdnleiting.top

[R69] 生成随机密码
来源：http://vyx.jinghuilouyu.cn

head -c 16 /dev/urandom | base64
来源：http://tcm.jlsjyb.cn

[R70] 时间戳与互转
来源：http://rzo.cashguo.top

date +%s;  date -d @1700000000
来源：http://xvg.tarul.cn

[R71] 日期格式化
来源：http://ckp.hongshengwenyu.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://pmh.yj20258.top

[R72] 等待端口就绪
来源：http://txe.yfazqb.com

until nc -z localhost 3306; do sleep 1; done
来源：http://kqr.shangyingyoupin.top

[R73] 分割大日志
来源：http://lkb.mhx1999.top

split -l 1000 big.log part_
来源：http://kdu.sjlbkw.cn

[R74] 批量重命名
来源：http://itb.shuidangran.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://imw.tanke756.top

[R75] 导出环境变量
来源：http://jfn.vehdjk.com

export PATH="$HOME/bin:$PATH"
来源：http://zfg.wangdashe.top

[R76] 使用临时文件
来源：http://ula.kuanghao11.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sqh.hnqzz.top

[R77] 读取用户输入
来源：http://qss.shanyushiyangtech.top

read -rp "请输入: " ans
来源：http://mne.hnqzz.top

[R78] 交互式菜单
来源：http://ahu.zhijiandao.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ylz.ydzc1.top

[R79] 解析命令行选项
来源：http://wsr.yuxming.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tin.ctjpmb.com

[R80] 查看脚本执行耗时
来源：http://ple.havefunace.top

time ./run.sh
来源：http://jyn.9152youxi.cn

================================================================================
来源：http://bnk.wangshuangyany.cn

S. C / C++ 专题
来源：http://lvv.yueranfly.top

================================================================================
来源：http://zkq.fehbvm.com

[S01] C：Hello World
来源：http://emk.sjlbkw.cn

#include <stdio.h>
来源：http://kda.gogol.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://pty.vqdsnc.cn

[S02] C：变量与格式化输出
来源：http://leq.feifeiyinyue.top

int a = 10; printf("%d\n", a);
来源：http://rnz.sysykeji.top

[S03] C：读入整数
来源：http://ezb.zdbjq.cn

int x; scanf("%d", &x);
来源：http://mgw.fehbvm.com

[S04] C：字符串复制
来源：http://whs.sufxvd.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xst.meibo888.top

[S05] C：字符串长度
来源：http://dtc.nanxuanxn.top

strlen(s)
来源：http://rsr.hammf.cn

[S06] C：字符串比较
来源：http://lko.zhiwuduotai.top

strcmp(a, b) == 0
来源：http://dej.xuanzx.com

[S07] C：数组遍历求和
来源：http://nqr.gaohongyu789.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wbf.hfpthk.cn

[S08] C：动态内存分配与释放
来源：http://myo.zhaomingkeji.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wbs.yj20258.top

[S09] C：结构体定义与初始化
来源：http://ird.aizwys.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nww.tarul.cn

[S10] C：指针与解引用
来源：http://wkb.52xcode.cn

int *p = &a;  *p = 5;
来源：http://amb.yanxiufei.cn

[S11] C：逐行读文件
来源：http://knz.xuetiantiany.cn

FILE *f = fopen("a.txt", "r");
来源：http://mik.sufxvd.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vch.zhiwuduotai.top

fclose(f);
来源：http://wsz.yanxiufei.cn

[S12] C：写文件
来源：http://kdc.jianghu66.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ect.xinyue.icu

[S13] C：宏定义
来源：http://bsy.yanxiufei.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kzm.yuanzhike.top

[S14] C：枚举
来源：http://ivo.gogol.net.cn

enum Color { RED, GREEN, BLUE };
来源：http://hwa.gogol.net.cn

[S15] C：类型转换
来源：http://knv.uphjek.com

(double) a / b
来源：http://hlf.sxryk.cn

[S16] C：位操作置位
来源：http://fpg.jinyuanbaomall.cn

x |= (1 << 3);
来源：http://khq.ybcxt.top

[S17] C：安全拼接字符串
来源：http://exw.0kj1m.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ajj.andypj.xyz

[S18] C：命令行参数
来源：http://vng.xinyue.icu

int main(int argc, char **argv)
来源：http://kaq.hammf.cn

[S19] C：快速排序
来源：http://bsd.wangshuangyany.cn

qsort(a, n, sizeof(int), cmp);
来源：http://csm.fanxiaobao.xyz

[S20] C：二分查找
来源：http://fxv.jqgufenzy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://syq.ywan-chungtsiang.top

[S21] C：字符类别判断
来源：http://njs.shanyushiyangkeji.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dch.yuxming.cn

[S22] C：字符串转数字
来源：http://xkr.kuanghao11.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xno.gaohongyu789.top

[S23] C：随机数
来源：http://szu.cucudq.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hoo.zycfv.cn

[S24] C：获取本地时间
来源：http://tsi.jinghuilouyu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pqn.yangfankeji.com

[S25] C：内存拷贝
来源：http://khs.kuanghao11.cn

memcpy(dst, src, n);
来源：http://glf.316326.xyz

[S26] C：内存清零
来源：http://bkj.uphjek.com

memset(a, 0, sizeof a);
来源：http://fvz.cashguo.top

[S27] C：定义常量
来源：http://mna.fengsongda.top

const double PI = 3.14159;
来源：http://diz.ivvv.top

[S28] C：静态变量
来源：http://zog.sysykeji.top

static int counter = 0;
来源：http://wmn.jinghuilouyu.cn

[S29] C：变参函数
来源：http://sbf.yuanzhike.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wlk.yj202588.top

[S30] C：头文件保护
来源：http://gve.fengsongda.top

#ifndef X_H
来源：http://qyy.ybcxt.top

#define X_H
来源：http://hch.fengsongda.top

#endif
来源：http://vha.daxiang520.top

[S31] C++：Hello World
来源：http://sjv.yueranfly.top

#include <iostream>
来源：http://qfj.pengpengdd.cyou

int main() { std::cout << "Hello\n"; }
来源：http://zbt.ehwqpu.com

[S32] C++：字符串
来源：http://jmm.gzhubu.top

std::string s = "hi";  s += "!";
来源：http://osq.tian-w.cn

[S33] C++：vector 增删
来源：http://jrf.gaohongyu789.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ilw.52xcode.cn

[S34] C++：遍历 vector
来源：http://hfr.zycfv.cn

for (auto &x : v) { std::cout << x; }
来源：http://awm.ybcxt.top

[S35] C++：map
来源：http://rom.daxiang520.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hie.fanxiaobao.xyz

[S36] C++：unordered_map
来源：http://swh.hfpthk.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ljj.yvedp.cn

[S37] C++：set
来源：http://bhd.nwbrower.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lfq.bbcook.cn

[S38] C++：排序
来源：http://drz.fzhhl.top

std::sort(v.begin(), v.end());
来源：http://lwb.316326.xyz

[S39] C++：自定义比较器排序
来源：http://cym.yvedp.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ymv.yangfankeji.com

[S40] C++：查找元素
来源：http://axa.tarul.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yca.andypj.xyz

[S41] C++：类与构造函数
来源：http://nov.tianlin.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cdr.ppjwa.cn

[S42] C++：继承与虚函数
来源：http://rym.aibaodan.cn

class B : public Base { public: void f() override {} };
来源：http://ilk.xinyue.icu

[S43] C++：智能指针
来源：http://acs.ywan-chungtsiang.top

auto p = std::make_unique<int>(5);
来源：http://lxz.zhongyouzk.top

[S44] C++：引用传参
来源：http://zca.nanxinkj.top

void inc(int &x) { ++x; }
来源：http://lao.sysykeji.top

[S45] C++：lambda
来源：http://nqf.sjlbkw.cn

auto add = [](int a, int b) { return a + b; };
来源：http://shy.zhengqikj.top

[S46] C++：函数模板
来源：http://djg.yvedp.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hby.yj20258.top

[S47] C++：结构化绑定遍历
来源：http://lon.yuanzhike.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jfk.fzhhl.top

[S48] C++：逐行读文件
来源：http://dkd.cucudq.cn

std::ifstream in("a.txt");  std::string line;
来源：http://cqf.ehwqpu.com

while (std::getline(in, line)) { }
来源：http://cyt.hnqzz.top

[S49] C++：写文件
来源：http://hck.yonumen.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jry.svipenyu.cn

[S50] C++：格式化数字
来源：http://uxc.andypj.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pct.gzhubu.top

[S51] C++：显式类型转换
来源：http://rvh.tarul.cn

static_cast<double>(a) / b
来源：http://cui.daxiang520.top

[S52] C++：const 与 noexcept
来源：http://cnf.tianlin.xyz

int size() const noexcept { return n_; }
来源：http://oga.nanxinkj.top

[S53] C++：移动语义
来源：http://fcr.fktsv.cn

std::vector<int> w = std::move(v);
来源：http://odi.sufxvd.cn

[S54] C++：异常处理
来源：http://zni.nanxuanxn.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cmo.zhengqikj.top

[S55] C++：结构化绑定
来源：http://xrb.ywan-chungtsiang.top

auto [a, b] = std::make_pair(1, 2);
来源：http://rjv.hammf.cn

[S56] C++：optional
来源：http://cds.yj202588.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pmn.birdmap.top

[S57] C++：编译期常量
来源：http://hqy.jqgfzy.top

constexpr int N = 10;
来源：http://ykg.gzhubu.top

[S58] C++：命名空间
来源：http://jrx.ppjwa.cn

namespace ns { int f() { return 1; } }
来源：http://mun.yangfankeji.com

[S59] C++：静态断言
来源：http://caj.yongpay.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jty.ydjk.org.cn

[S60] C++：遍历并删除元素
来源：http://ljc.shuidangran.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xbh.gotoacloud.top

================================================================================
来源：http://fod.hysaishi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kfo.xziqi.cn

================================================================================
来源：http://ldv.kuanghao11.cn

[T01] Kotlin：Hello World
来源：http://xjz.sufxvd.cn

println("Hello")
来源：http://jpt.nanxuanxn.top

[T02] Kotlin：变量
来源：http://xce.jiagoushi.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cxa.tianlin.xyz

[T03] Kotlin：字符串模板
来源：http://ipk.c1oappe.top

"值: $b"
来源：http://fyh.sysykeji.top

[T04] Kotlin：空安全
来源：http://nag.jqgufenzy.top

val n: String? = null;  n?.length
来源：http://lqe.snrcjt.cn

[T05] Kotlin：when 表达式
来源：http://vff.jinghuilouyu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hrz.hnxiangtu.top

[T06] Kotlin：集合映射
来源：http://aga.xingfuxueyuan.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://dpr.epnwcf.com

[T07] Kotlin：集合过滤
来源：http://oty.ydzc1.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ici.jqgfzy.top

[T08] Kotlin：数据类
来源：http://rgq.tanke756.top

data class User(val name: String, val age: Int)
来源：http://xyh.sweek.top

[T09] Kotlin：扩展函数
来源：http://eiw.zhiwuduotai.top

fun String.exclaim() = this + "!"
来源：http://evo.haohaochexian.top

[T10] Kotlin：默认参数
来源：http://tvv.feifeiyinyue.top

fun greet(name: String = "World") = "Hi $name"
来源：http://jgz.sjlbkw.cn

[T11] Kotlin：协程
来源：http://ywo.sysykeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://wvv.feifeiyinyue.top

[T12] Kotlin：解构声明
来源：http://dvf.hesvh.cn

val (a, b) = Pair(1, 2)
来源：http://hwn.sysykeji.top

[T13] Kotlin：只读 Map
来源：http://cey.tianlin.xyz

val m = mapOf("a" to 1)
来源：http://zge.fehbvm.com

[T14] Kotlin：循环
来源：http://dak.xingfuxueyuan.xyz

for (i in 1..10) println(i)
来源：http://hvm.hcnkem.com

[T15] Kotlin：接口
来源：http://hdf.bjfxy.top

interface Shape { fun area(): Double }
来源：http://qbg.zhoulong.xyz

[T16] Swift：Hello World
来源：http://wuq.hammf.cn

print("Hello")
来源：http://htx.iojbl.cn

[T17] Swift：变量与常量
来源：http://erx.cqqwz.cn

var a = 1;  let b = 2
来源：http://koq.yfazqb.com

[T18] Swift：字符串插值
来源：http://mqz.sjlbkw.cn

"值: \(b)"
来源：http://owv.dashuyun.cn

[T19] Swift：可选绑定
来源：http://mhm.pycfn.com

if let n = opt { print(n) }
来源：http://rai.yangfankeji.com

[T20] Swift：数组操作
来源：http://rrb.sweek.top

var a = [1, 2, 3];  a.append(4)
来源：http://rld.jinyuanbaomall.cn

[T21] Swift：遍历
来源：http://tva.nanxuanxn.top

for x in a { print(x) }
来源：http://ptn.9152youxi.cn

[T22] Swift：字典
来源：http://fav.bbcook.cn

var d = ["a": 1];  d["b"] = 2
来源：http://gbx.fanxiaobao.xyz

[T23] Swift：函数
来源：http://lvh.xylfe.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://owf.wangdashe.top

[T24] Swift：闭包
来源：http://aze.cdnleiting.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ltb.hongshengwenyu.top

[T25] Swift：结构体
来源：http://zsm.cucudq.cn

struct P { var x: Int }
来源：http://xbo.aibaodan.cn

[T26] Swift：类与重写
来源：http://agk.yanxiufei.cn

class A: Base { override func f() {} }
来源：http://kor.sysykeji.top

[T27] Swift：错误处理
来源：http://qhb.yvedp.cn

do { try f() } catch { print(error) }
来源：http://hwb.yfazqb.com

[T28] Swift：枚举
来源：http://grk.bjfxy.top

enum Color { case red, green }
来源：http://jxa.tian-w.cn

[T29] Swift：guard 提前返回
来源：http://xup.havefunace.top

guard let x = opt else { return }
来源：http://rdp.fengsongda.top

[T30] Swift：协议
来源：http://bzp.hnxiangtu.top

protocol Shape { func area() -> Double }
来源：http://hqr.hysaishi.cn

[T31] Lua：Hello World
来源：http://gli.52xcode.cn

print("Hello")
来源：http://upn.hywenlv.cn

[T32] Lua：局部变量
来源：http://slb.jinqigufen.top

local a = 1
来源：http://fti.fehbvm.com

[T33] Lua：表（数组）
来源：http://wmr.c1oappe.top

local t = {1, 2, 3};  t[4] = 4
来源：http://eab.aizwys.cn

[T34] Lua：遍历表
来源：http://bki.chenzaomai.com

for i, v in ipairs(t) do print(i, v) end
来源：http://oqo.shangyingyoupin.top

[T35] Lua：字典表
来源：http://jhh.316326.xyz

local d = { a = 1 };  d.b = 2
来源：http://ncc.yanxiufei.cn

[T36] Lua：函数
来源：http://jag.yuanzhike.top

function add(a, b) return a + b end
来源：http://hfv.sjlbkw.cn

[T37] Lua：字符串拼接
来源：http://lbp.hammf.cn

"a" .. "b"
来源：http://min.zhaomingkeji.xyz

[T38] Lua：条件
来源：http://awl.ydjk.org.cn

if x > 0 then print("正") end
来源：http://spv.zdqjudy.top

[T39] Lua：模式匹配
来源：http://skr.epnwcf.com

string.find(s, "%d+")
来源：http://hny.gzhubu.top

[T40] Lua：元表
来源：http://dhk.gotoacloud.top

setmetatable({}, { __index = base })
来源：http://dyi.pycfn.com

[T41] Perl：Hello World
来源：http://mcq.meibo888.top

print "Hello\n";
来源：http://qnf.xuanzx.com

[T42] Perl：变量类型
来源：http://txj.wangdashe.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ojd.sysykeji.top

[T43] Perl：字符串插值
来源：http://gdc.xziqi.cn

"值: $a"
来源：http://iwk.zycfv.cn

[T44] Perl：条件
来源：http://atf.xziqi.cn

if ($a > 0) { print "正"; }
来源：http://qcw.yj20258.top

[T45] Perl：数组遍历
来源：http://kby.jinqigufen.top

for my $x (@arr) { print $x; }
来源：http://dny.shanyushiyangkeji.top

[T46] Perl：哈希操作
来源：http://pfk.nanxinkj.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rqa.havefunace.top

[T47] Perl：正则捕获
来源：http://ogs.nanxinkj.top

if ($s =~ /(\d+)/) { print $1; }
来源：http://dmt.jqgfzy.top

[T48] Perl：正则替换
来源：http://rqq.feifeiyinyue.top

$s =~ s/old/new/g;
来源：http://lsm.shanyushiyangtech.top

[T49] Perl：函数
来源：http://erh.jianghu66.top

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qtg.xingfuxueyuan.xyz

[T50] Perl：逐行读文件
来源：http://xex.pycfn.com

open my $fh, "<", "a.txt" or die $!;
来源：http://sop.jianghu66.top


<!-- 参考信息 -->