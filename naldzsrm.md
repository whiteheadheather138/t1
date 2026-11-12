代发 wailian999

find . -name "*.log" -type f
来源：http://tkw.cdnleiting.top

[R44] 按修改时间查找
来源：http://hmf.gogol.net.cn

find . -mtime -7 -type f
来源：http://idl.jyoumei.cn

[R45] 批量删除
来源：http://iea.haohaochexian.top

find . -name "*.tmp" -delete
来源：http://wcp.shzxlz.cn

[R46] 递归替换文件内容
来源：http://qfp.bbcook.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tps.xylfe.cn

[R47] sed 单行替换
来源：http://uds.yvedp.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ydd.nwbrower.top

[R48] awk 取指定列
来源：http://byf.yj20258.top

awk '{print $1, $3}' a.txt
来源：http://bap.shanyushiyangkeji.top

[R49] awk 带条件
来源：http://tcw.zdqjudy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nch.birdmap.top

[R50] awk 求和
来源：http://faq.jqgufenzy.top

awk '{s += $2} END {print s}' a.txt
来源：http://xfg.chenlongwang.top

[R51] 排序去重取前几
来源：http://fuu.guannengcc.top

sort a.txt | uniq -c | sort -rn | head
来源：http://bcu.jinghuilouyu.cn

[R52] 统计行数
来源：http://myn.iojbl.cn

wc -l a.txt
来源：http://tgt.ppjwa.cn

[R53] 查看文件头与实时尾
来源：http://qbf.tian-w.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rbn.wangshuangyany.cn

[R54] 比较两个文件
来源：http://tqc.vqdsnc.cn

diff a.txt b.txt
来源：http://lku.cdnleiting.top

[R55] 压缩与解压
来源：http://rze.yonumen.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dxv.ybcxt.top

[R56] 远程拷贝
来源：http://lfw.xingfuxueyuan.xyz

scp file user@host:/path/
来源：http://mpg.hongshengwenyu.top

[R57] 远程执行命令
来源：http://mrz.jinyuanbaomall.cn

ssh user@host 'uptime'
来源：http://acg.aibaodan.cn

[R58] 下载文件
来源：http://kmj.hnqzz.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dqr.fzhhl.top

[R59] 发 POST JSON
来源：http://vty.cqqwz.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qgu.tian-w.cn

[R60] 只看 HTTP 状态码
来源：http://sqh.cheryme.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://oip.zdqjudy.top

[R61] 磁盘占用
来源：http://akf.zhixingplan.top

df -h;  du -sh *
来源：http://qpr.birdmap.top

[R62] 找最占空间的文件
来源：http://bqs.ehwqpu.com

du -ah . | sort -rh | head -10
来源：http://vcu.haohaochexian.top

[R63] 内存与进程
来源：http://oij.quarkkingdee.top

free -h;  ps aux | grep nginx
来源：http://ucz.sxryk.cn

[R64] 结束进程
来源：http://hwv.shanyushiyangtech.top

kill -9 $(pgrep -f app.py)
来源：http://znl.52xcode.cn

[R65] 查看端口占用
来源：http://ito.aizwys.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://syl.xinyue.icu

[R66] 定时任务
来源：http://mot.hesvh.cn

crontab -e;  crontab -l
来源：http://zrj.cashguo.top

[R67] 生成随机十六进制串
来源：http://ank.redwolf501.top

openssl rand -hex 16
来源：http://rhi.yongpay.top

[R68] 计算文件校验值
来源：http://cei.smart0.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://cmp.gzhubu.top

[R69] 生成随机密码
来源：http://ynq.gaohongyu789.top

head -c 16 /dev/urandom | base64
来源：http://pmv.ybcxt.top

[R70] 时间戳与互转
来源：http://rhv.sufxvd.cn

date +%s;  date -d @1700000000
来源：http://bna.yuxming.cn

[R71] 日期格式化
来源：http://cca.fanxiaobao.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://lys.yuxming.cn

[R72] 等待端口就绪
来源：http://fvs.jlsjyb.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://htt.redwolf501.top

[R73] 分割大日志
来源：http://cuj.pengpengdd.cyou

split -l 1000 big.log part_
来源：http://ktv.chenjidiqi.icu

[R74] 批量重命名
来源：http://hrs.fengsongda.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://efg.ctjpmb.com

[R75] 导出环境变量
来源：http://jjb.cdnleiting.top

export PATH="$HOME/bin:$PATH"
来源：http://lfl.yangfankeji.com

[R76] 使用临时文件
来源：http://qrd.hywenlv.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ucv.daria6918.cn

[R77] 读取用户输入
来源：http://sup.svipenyu.cn

read -rp "请输入: " ans
来源：http://pwd.yfazqb.com

[R78] 交互式菜单
来源：http://uoa.birdmap.top

select opt in a b c; do echo "$opt"; break; done
来源：http://pik.shanyushiyangkeji.top

[R79] 解析命令行选项
来源：http://lyb.ybcxt.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xdt.fehbvm.com

[R80] 查看脚本执行耗时
来源：http://ulh.redwolf501.top

time ./run.sh
来源：http://oxj.jinqigfzy.top

================================================================================
来源：http://yvm.shangyingyoupin.top

S. C / C++ 专题
来源：http://tog.nwbrower.top

================================================================================
来源：http://vlb.yvedp.cn

[S01] C：Hello World
来源：http://iff.yanxiufei.cn

#include <stdio.h>
来源：http://qiq.yj202588.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://mvw.aibaodan.cn

[S02] C：变量与格式化输出
来源：http://mhf.hywenlv.cn

int a = 10; printf("%d\n", a);
来源：http://qqg.fengsongda.top

[S03] C：读入整数
来源：http://klg.cucudq.cn

int x; scanf("%d", &x);
来源：http://xwj.quarkkingdee.top

[S04] C：字符串复制
来源：http://ecx.shanyushiyangtech.top

char dst[32]; strcpy(dst, "hi");
来源：http://zmn.guowangkeji.top

[S05] C：字符串长度
来源：http://oks.zhongyouzk.top

strlen(s)
来源：http://aia.bjfxy.top

[S06] C：字符串比较
来源：http://uat.nanxinkj.top

strcmp(a, b) == 0
来源：http://gdy.vehdjk.com

[S07] C：数组遍历求和
来源：http://bmq.svipenyu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pfm.shanyushiyangkeji.top

[S08] C：动态内存分配与释放
来源：http://mji.shuidangran.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://njj.xziqi.cn

[S09] C：结构体定义与初始化
来源：http://xwm.xinyue.icu

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://aua.sxryk.cn

[S10] C：指针与解引用
来源：http://uga.haohaochexian.top

int *p = &a;  *p = 5;
来源：http://atl.gogol.net.cn

[S11] C：逐行读文件
来源：http://tti.cqqwz.cn

FILE *f = fopen("a.txt", "r");
来源：http://vyu.yueranfly.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://iqh.mhx1999.top

fclose(f);
来源：http://pfi.yj20258888.top

[S12] C：写文件
来源：http://vkx.yj20258888.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ore.316326.xyz

[S13] C：宏定义
来源：http://hte.iojbl.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kbr.fktsv.cn

[S14] C：枚举
来源：http://eba.yfazqb.com

enum Color { RED, GREEN, BLUE };
来源：http://ihm.cdnleiting.top

[S15] C：类型转换
来源：http://cgr.zhaomingkeji.xyz

(double) a / b
来源：http://imj.nanxuanxn.top

[S16] C：位操作置位
来源：http://mdr.hywenlv.cn

x |= (1 << 3);
来源：http://nut.yonumen.top

[S17] C：安全拼接字符串
来源：http://vcv.dianchejie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://syc.andypj.xyz

[S18] C：命令行参数
来源：http://hai.ctjpmb.com

int main(int argc, char **argv)
来源：http://drc.hywenlv.cn

[S19] C：快速排序
来源：http://gpj.ivvv.top

qsort(a, n, sizeof(int), cmp);
来源：http://ptt.dianchejie.cn

[S20] C：二分查找
来源：http://kjt.yj202588.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gqr.jinqigfzy.top

[S21] C：字符类别判断
来源：http://oli.havefunace.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vkm.zhoulong.xyz

[S22] C：字符串转数字
来源：http://lne.redwolf501.top

atoi("42");  strtod("3.14", NULL);
来源：http://cbe.jiagoushi.top

[S23] C：随机数
来源：http://kbk.wangdashe.top

srand(time(NULL));  int r = rand() % 100;
来源：http://mcj.uphjek.com

[S24] C：获取本地时间
来源：http://qgy.cheryme.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://oyi.jinqigufen.top

[S25] C：内存拷贝
来源：http://dlp.jiagoushi.top

memcpy(dst, src, n);
来源：http://kko.smart0.xyz

[S26] C：内存清零
来源：http://jnm.tianlin.xyz

memset(a, 0, sizeof a);
来源：http://bgk.hnqzz.top

[S27] C：定义常量
来源：http://gzh.uphjek.com

const double PI = 3.14159;
来源：http://rpw.zhengqikj.top

[S28] C：静态变量
来源：http://lbu.yfazqb.com

static int counter = 0;
来源：http://ebf.xingfuxueyuan.xyz

[S29] C：变参函数
来源：http://sya.yj202588.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rgy.xylfe.cn

[S30] C：头文件保护
来源：http://dzr.gogol.net.cn

#ifndef X_H
来源：http://dax.iojbl.cn

#define X_H
来源：http://rpx.zhiwuduotai.top

#endif
来源：http://tts.jinyuanbaomall.cn

[S31] C++：Hello World
来源：http://xxh.nanxuanxn.top

#include <iostream>
来源：http://bqx.ydjk.org.cn

int main() { std::cout << "Hello\n"; }
来源：http://nll.jqgfzy.top

[S32] C++：字符串
来源：http://tet.snrcjt.cn

std::string s = "hi";  s += "!";
来源：http://krl.hongshengwenyu.top

[S33] C++：vector 增删
来源：http://bih.sjlbkw.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ueh.bjfxy.top

[S34] C++：遍历 vector
来源：http://lja.jqgfzy.top

for (auto &x : v) { std::cout << x; }
来源：http://kli.chenlongwang.top

[S35] C++：map
来源：http://pjg.ybcxt.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cho.guannengcc.top

[S36] C++：unordered_map
来源：http://kua.yongpay.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lpn.sufxvd.cn

[S37] C++：set
来源：http://scs.hongshengwenyu.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://neb.yj20258888.top

[S38] C++：排序
来源：http://rdi.xingfuxueyuan.xyz

std::sort(v.begin(), v.end());
来源：http://ibt.tian-w.cn

[S39] C++：自定义比较器排序
来源：http://dbg.jinqigufen.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jdw.fzhhl.top

[S40] C++：查找元素
来源：http://ksj.redwolf501.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hvf.quarkkingdee.top

[S41] C++：类与构造函数
来源：http://whe.ivvv.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kyi.shzxlz.cn

[S42] C++：继承与虚函数
来源：http://tuh.dashuyun.cn

class B : public Base { public: void f() override {} };
来源：http://pag.gogol.net.cn

[S43] C++：智能指针
来源：http://uly.bbcook.cn

auto p = std::make_unique<int>(5);
来源：http://ber.yuxming.cn

[S44] C++：引用传参
来源：http://lpg.iojbl.cn

void inc(int &x) { ++x; }
来源：http://utj.yj202588.top

[S45] C++：lambda
来源：http://zcn.hysaishi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qbv.birdmap.top

[S46] C++：函数模板
来源：http://gxh.fengsongda.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ewg.c1oappe.top

[S47] C++：结构化绑定遍历
来源：http://gqy.jyoumei.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qac.xuetiantiany.cn

[S48] C++：逐行读文件
来源：http://iks.birdmap.top

std::ifstream in("a.txt");  std::string line;
来源：http://kuv.daria6918.cn

while (std::getline(in, line)) { }
来源：http://axl.xingfuxueyuan.xyz

[S49] C++：写文件
来源：http://jjf.guannengcc.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vez.hfpthk.cn

[S50] C++：格式化数字
来源：http://bnd.tian-w.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qax.daria6918.cn

[S51] C++：显式类型转换
来源：http://asv.wangshuangyany.cn

static_cast<double>(a) / b
来源：http://mtk.hysaishi.cn

[S52] C++：const 与 noexcept
来源：http://rpk.shzxlz.cn

int size() const noexcept { return n_; }
来源：http://aid.tian-w.cn

[S53] C++：移动语义
来源：http://ahh.gzhubu.top

std::vector<int> w = std::move(v);
来源：http://agn.shanyushiyangtech.top

[S54] C++：异常处理
来源：http://deh.yj202588.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://slp.pycfn.com

[S55] C++：结构化绑定
来源：http://qak.bjfxy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ptc.sweek.top

[S56] C++：optional
来源：http://myi.shuidangran.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zfg.tianlin.xyz

[S57] C++：编译期常量
来源：http://jnz.jqgfzy.top

constexpr int N = 10;
来源：http://fvn.vqdsnc.cn

[S58] C++：命名空间
来源：http://tld.wangshuangyany.cn

namespace ns { int f() { return 1; } }
来源：http://lde.tian-w.cn

[S59] C++：静态断言
来源：http://qax.hfpthk.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kqm.gotoacloud.top

[S60] C++：遍历并删除元素
来源：http://mdv.zhijiandao.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ryq.wangdashe.top

================================================================================
来源：http://tpk.redwolf501.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://upk.feifeiyinyue.top

================================================================================
来源：http://hrn.hnxiangtu.top

[T01] Kotlin：Hello World
来源：http://vhc.sysykeji.top

println("Hello")
来源：http://cik.cqqwz.cn

[T02] Kotlin：变量
来源：http://uzv.shanyushiyangtech.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dxp.yfazqb.com

[T03] Kotlin：字符串模板
来源：http://wux.zdqjudy.top

"值: $b"
来源：http://hau.bjfxy.top

[T04] Kotlin：空安全
来源：http://okp.sjlbkw.cn

val n: String? = null;  n?.length
来源：http://rse.xingfuxueyuan.xyz

[T05] Kotlin：when 表达式
来源：http://vrb.nwbrower.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bsk.bbcook.cn

[T06] Kotlin：集合映射
来源：http://asb.316326.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://atk.wangdashe.top

[T07] Kotlin：集合过滤
来源：http://kpx.chenlongwang.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://mar.aizwys.cn

[T08] Kotlin：数据类
来源：http://gjq.aibaodan.cn

data class User(val name: String, val age: Int)
来源：http://qju.jianghu66.top

[T09] Kotlin：扩展函数
来源：http://prh.sjlbkw.cn

fun String.exclaim() = this + "!"
来源：http://aci.ppjwa.cn

[T10] Kotlin：默认参数
来源：http://iez.daria6918.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qxe.yj20258888.top

[T11] Kotlin：协程
来源：http://yfm.haohaochexian.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://mzr.xinyue.icu

[T12] Kotlin：解构声明
来源：http://ukc.gogol.net.cn

val (a, b) = Pair(1, 2)
来源：http://dkb.feifeiyinyue.top

[T13] Kotlin：只读 Map
来源：http://hou.yueranfly.top

val m = mapOf("a" to 1)
来源：http://ddl.xingfuxueyuan.xyz

[T14] Kotlin：循环
来源：http://jzr.fktsv.cn

for (i in 1..10) println(i)
来源：http://rfl.dashuyun.cn

[T15] Kotlin：接口
来源：http://pzc.zhixingplan.top

interface Shape { fun area(): Double }
来源：http://tma.cucudq.cn

[T16] Swift：Hello World
来源：http://vva.zhengqikj.top

print("Hello")
来源：http://bsn.ydjk.org.cn

[T17] Swift：变量与常量
来源：http://dgz.daria6918.cn

var a = 1;  let b = 2
来源：http://gam.yfazqb.com

[T18] Swift：字符串插值
来源：http://kzt.yuxming.cn

"值: \(b)"
来源：http://etf.9152youxi.cn

[T19] Swift：可选绑定
来源：http://iaz.zhixingplan.top

if let n = opt { print(n) }
来源：http://lqq.xuanzx.com

[T20] Swift：数组操作
来源：http://xln.jinqigufen.top

var a = [1, 2, 3];  a.append(4)
来源：http://gzd.jqgfzy.top

[T21] Swift：遍历
来源：http://pos.sjlbkw.cn

for x in a { print(x) }
来源：http://pzs.wangdashe.top

[T22] Swift：字典
来源：http://fru.uphjek.com

var d = ["a": 1];  d["b"] = 2
来源：http://wda.52xcode.cn

[T23] Swift：函数
来源：http://ygs.vehdjk.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xrf.wangshuangyany.cn

[T24] Swift：闭包
来源：http://phe.jianghu66.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ujl.guowangkeji.top

[T25] Swift：结构体
来源：http://xkb.yj20258.top

struct P { var x: Int }
来源：http://lfi.9152youxi.cn

[T26] Swift：类与重写
来源：http://wei.smart0.xyz

class A: Base { override func f() {} }
来源：http://wvj.sjlbkw.cn

[T27] Swift：错误处理
来源：http://tzz.316326.xyz

do { try f() } catch { print(error) }
来源：http://asc.yongpay.top

[T28] Swift：枚举
来源：http://ldq.wangshuangyany.cn

enum Color { case red, green }
来源：http://cip.chenzaomai.com

[T29] Swift：guard 提前返回
来源：http://oiw.ppjwa.cn

guard let x = opt else { return }
来源：http://iqe.bbcook.cn

[T30] Swift：协议
来源：http://wuv.wangdashe.top

protocol Shape { func area() -> Double }
来源：http://tys.shuidangran.top

[T31] Lua：Hello World
来源：http://smo.havefunace.top

print("Hello")
来源：http://opn.pycfn.com

[T32] Lua：局部变量
来源：http://stt.yonumen.top

local a = 1
来源：http://vsh.hfpthk.cn

[T33] Lua：表（数组）
来源：http://rae.tanke756.top

local t = {1, 2, 3};  t[4] = 4
来源：http://vfg.smart0.xyz

[T34] Lua：遍历表
来源：http://yaz.shangyingyoupin.top

for i, v in ipairs(t) do print(i, v) end
来源：http://hoz.fengsongda.top

[T35] Lua：字典表
来源：http://irz.jinghuilouyu.cn

local d = { a = 1 };  d.b = 2
来源：http://fmn.chenlongwang.top

[T36] Lua：函数
来源：http://cjp.hnqzz.top

function add(a, b) return a + b end
来源：http://ggm.pycfn.com

[T37] Lua：字符串拼接
来源：http://ldn.52xcode.cn

"a" .. "b"
来源：http://azm.jqgufenzy.top

[T38] Lua：条件
来源：http://dii.bjfxy.top

if x > 0 then print("正") end
来源：http://czn.jianghu66.top

[T39] Lua：模式匹配
来源：http://gqw.fktsv.cn

string.find(s, "%d+")
来源：http://ket.yonumen.top

[T40] Lua：元表
来源：http://qcg.yueranfly.top

setmetatable({}, { __index = base })
来源：http://fbt.wangshuangyany.cn

[T41] Perl：Hello World
来源：http://rhx.jyoumei.cn

print "Hello\n";
来源：http://lfn.iojbl.cn

[T42] Perl：变量类型
来源：http://lki.52xcode.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fhe.shuidangran.top

[T43] Perl：字符串插值
来源：http://crx.wangshuangyany.cn

"值: $a"
来源：http://ire.feifeiyinyue.top

[T44] Perl：条件
来源：http://zhz.xuetiantiany.cn

if ($a > 0) { print "正"; }
来源：http://slp.redwolf501.top

[T45] Perl：数组遍历
来源：http://ust.wangdashe.top

for my $x (@arr) { print $x; }
来源：http://hfj.smart0.xyz

[T46] Perl：哈希操作
来源：http://rzb.cheryme.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nhz.chenzaomai.com


<!-- 参考信息 -->