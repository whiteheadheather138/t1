代发 wailian999

cmd > out.log 2>&1
来源：http://pok.feifeiyinyue.top

[R40] 追加写日志
来源：http://jqa.yvedp.cn

echo "log" >> out.log
来源：http://lqk.yangfankeji.com

[R41] 丢弃输出
来源：http://cwo.jinqigfzy.top

cmd >/dev/null 2>&1
来源：http://fdf.hnxiangtu.top

[R42] 输入重定向
来源：http://oea.ppjwa.cn

wc -l < a.txt
来源：http://qxe.fktsv.cn

[R43] 按名字查找文件
来源：http://fjr.chenjidiqi.icu

find . -name "*.log" -type f
来源：http://vtt.shuidangran.top

[R44] 按修改时间查找
来源：http://nuo.jinghuilouyu.cn

find . -mtime -7 -type f
来源：http://nww.zhixingplan.top

[R45] 批量删除
来源：http://odo.haohaochexian.top

find . -name "*.tmp" -delete
来源：http://yoz.yueranfly.top

[R46] 递归替换文件内容
来源：http://mmu.wangdashe.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vgk.bjfxy.top

[R47] sed 单行替换
来源：http://cdd.shangyingyoupin.top

sed -i 's/foo/bar/g' a.txt
来源：http://jpx.yj202588.top

[R48] awk 取指定列
来源：http://hav.shanyushiyangtech.top

awk '{print $1, $3}' a.txt
来源：http://ycr.jqgufenzy.top

[R49] awk 带条件
来源：http://zha.gotoacloud.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gea.gaohongyu789.top

[R50] awk 求和
来源：http://lte.ehwqpu.com

awk '{s += $2} END {print s}' a.txt
来源：http://hhm.vehdjk.com

[R51] 排序去重取前几
来源：http://xfk.0kj1m.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gcs.haohaochexian.top

[R52] 统计行数
来源：http://ngh.0kj1m.cn

wc -l a.txt
来源：http://wqr.zycfv.cn

[R53] 查看文件头与实时尾
来源：http://tav.cashguo.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://erq.shanyushiyangkeji.top

[R54] 比较两个文件
来源：http://ujk.ybcxt.top

diff a.txt b.txt
来源：http://jvi.zhaomingkeji.xyz

[R55] 压缩与解压
来源：http://sai.zhongyouzk.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fbb.yonumen.top

[R56] 远程拷贝
来源：http://tdh.hnqzz.top

scp file user@host:/path/
来源：http://aqo.fktsv.cn

[R57] 远程执行命令
来源：http://bor.yueranfly.top

ssh user@host 'uptime'
来源：http://nzw.iojbl.cn

[R58] 下载文件
来源：http://dha.hywenlv.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://alw.yuxming.cn

[R59] 发 POST JSON
来源：http://yff.iojbl.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dtl.jinyuanbaomall.cn

[R60] 只看 HTTP 状态码
来源：http://chx.vqdsnc.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rgm.52xcode.cn

[R61] 磁盘占用
来源：http://grh.sysykeji.top

df -h;  du -sh *
来源：http://lja.smart0.xyz

[R62] 找最占空间的文件
来源：http://icd.pycfn.com

du -ah . | sort -rh | head -10
来源：http://vuw.shanyushiyangkeji.top

[R63] 内存与进程
来源：http://mdg.jinyuanbaomall.cn

free -h;  ps aux | grep nginx
来源：http://xrn.ctjpmb.com

[R64] 结束进程
来源：http://pji.tanke756.top

kill -9 $(pgrep -f app.py)
来源：http://vys.sweek.top

[R65] 查看端口占用
来源：http://zhm.havefunace.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gbo.zdbjq.cn

[R66] 定时任务
来源：http://eih.aibaodan.cn

crontab -e;  crontab -l
来源：http://udh.uphjek.com

[R67] 生成随机十六进制串
来源：http://ikk.tianlin.xyz

openssl rand -hex 16
来源：http://ynw.xingfuxueyuan.xyz

[R68] 计算文件校验值
来源：http://jih.0kj1m.cn

sha256sum a.txt;  md5sum a.txt
来源：http://pgu.chenjidiqi.icu

[R69] 生成随机密码
来源：http://woa.haohaochexian.top

head -c 16 /dev/urandom | base64
来源：http://nzp.hesvh.cn

[R70] 时间戳与互转
来源：http://uws.svipenyu.cn

date +%s;  date -d @1700000000
来源：http://upo.hongshengwenyu.top

[R71] 日期格式化
来源：http://yjr.dianchejie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://osk.xuanzx.com

[R72] 等待端口就绪
来源：http://kzn.hnxiangtu.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ntt.fanxiaobao.xyz

[R73] 分割大日志
来源：http://alr.fanxiaobao.xyz

split -l 1000 big.log part_
来源：http://sey.yuanzhike.top

[R74] 批量重命名
来源：http://xel.sjlbkw.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tiz.shzxlz.cn

[R75] 导出环境变量
来源：http://tyy.shangyingyoupin.top

export PATH="$HOME/bin:$PATH"
来源：http://che.shuidangran.top

[R76] 使用临时文件
来源：http://dtc.gogol.net.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wdl.redwolf501.top

[R77] 读取用户输入
来源：http://gqn.sysykeji.top

read -rp "请输入: " ans
来源：http://mgp.shzxlz.cn

[R78] 交互式菜单
来源：http://dtx.kuanghao11.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://qfa.zhongyouzk.top

[R79] 解析命令行选项
来源：http://hiz.nanxuanxn.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ngv.yj202588.top

[R80] 查看脚本执行耗时
来源：http://qsg.sxryk.cn

time ./run.sh
来源：http://gtb.zhongyouzk.top

================================================================================
来源：http://yxt.shangyingyoupin.top

S. C / C++ 专题
来源：http://yxr.ctjpmb.com

================================================================================
来源：http://qze.sxryk.cn

[S01] C：Hello World
来源：http://okl.tian-w.cn

#include <stdio.h>
来源：http://mza.sjlbkw.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://rqx.chenzaomai.com

[S02] C：变量与格式化输出
来源：http://hjx.xinyue.icu

int a = 10; printf("%d\n", a);
来源：http://fdp.redwolf501.top

[S03] C：读入整数
来源：http://csz.ydzc1.top

int x; scanf("%d", &x);
来源：http://ogi.ydzc1.top

[S04] C：字符串复制
来源：http://fqf.hfpthk.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gfq.yj20258888.top

[S05] C：字符串长度
来源：http://qbt.fehbvm.com

strlen(s)
来源：http://kgf.cdnleiting.top

[S06] C：字符串比较
来源：http://tqj.sxryk.cn

strcmp(a, b) == 0
来源：http://ojw.hammf.cn

[S07] C：数组遍历求和
来源：http://vtp.chenjidiqi.icu

for (int i = 0; i < n; i++) sum += a[i];
来源：http://btd.cashguo.top

[S08] C：动态内存分配与释放
来源：http://jcg.yfazqb.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://elf.tarul.cn

[S09] C：结构体定义与初始化
来源：http://mgz.xingfuxueyuan.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tjq.zhoulong.xyz

[S10] C：指针与解引用
来源：http://ozv.feifeiyinyue.top

int *p = &a;  *p = 5;
来源：http://rgv.sweek.top

[S11] C：逐行读文件
来源：http://juu.daxiang520.top

FILE *f = fopen("a.txt", "r");
来源：http://qpn.cqqwz.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zpa.yfazqb.com

fclose(f);
来源：http://ztm.hcnkem.com

[S12] C：写文件
来源：http://idk.wangdashe.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hhb.snrcjt.cn

[S13] C：宏定义
来源：http://xsn.smart0.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jjj.zhaomingkeji.xyz

[S14] C：枚举
来源：http://rcp.pycfn.com

enum Color { RED, GREEN, BLUE };
来源：http://bzo.gotoacloud.top

[S15] C：类型转换
来源：http://hxc.wangshuangyany.cn

(double) a / b
来源：http://czp.cdnleiting.top

[S16] C：位操作置位
来源：http://wfc.iojbl.cn

x |= (1 << 3);
来源：http://mss.chenlongwang.top

[S17] C：安全拼接字符串
来源：http://ows.wangdashe.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wpt.chenzaomai.com

[S18] C：命令行参数
来源：http://qys.vqdsnc.cn

int main(int argc, char **argv)
来源：http://fcv.jinqigfzy.top

[S19] C：快速排序
来源：http://vjw.shzxlz.cn

qsort(a, n, sizeof(int), cmp);
来源：http://kyz.havefunace.top

[S20] C：二分查找
来源：http://ttk.ydzc1.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qcp.chenlongwang.top

[S21] C：字符类别判断
来源：http://laj.9152youxi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pyq.sjlbkw.cn

[S22] C：字符串转数字
来源：http://kne.nanxinkj.top

atoi("42");  strtod("3.14", NULL);
来源：http://uqk.quarkkingdee.top

[S23] C：随机数
来源：http://uzk.tianlin.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://bqw.xinyue.icu

[S24] C：获取本地时间
来源：http://mac.jinghuilouyu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zti.havefunace.top

[S25] C：内存拷贝
来源：http://rod.redwolf501.top

memcpy(dst, src, n);
来源：http://hat.smart0.xyz

[S26] C：内存清零
来源：http://hoa.ctjpmb.com

memset(a, 0, sizeof a);
来源：http://dwy.ydjk.org.cn

[S27] C：定义常量
来源：http://jor.quarkkingdee.top

const double PI = 3.14159;
来源：http://ukl.kuanghao11.cn

[S28] C：静态变量
来源：http://jau.dianchejie.cn

static int counter = 0;
来源：http://ztn.uphjek.com

[S29] C：变参函数
来源：http://hug.zhengqikj.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gpm.zhengqikj.top

[S30] C：头文件保护
来源：http://khf.xylfe.cn

#ifndef X_H
来源：http://mji.ehwqpu.com

#define X_H
来源：http://qbb.ybcxt.top

#endif
来源：http://esi.zhijiandao.cn

[S31] C++：Hello World
来源：http://mug.sufxvd.cn

#include <iostream>
来源：http://cdk.zhaomingkeji.xyz

int main() { std::cout << "Hello\n"; }
来源：http://ucd.hcnkem.com

[S32] C++：字符串
来源：http://tcp.pycfn.com

std::string s = "hi";  s += "!";
来源：http://hig.hammf.cn

[S33] C++：vector 增删
来源：http://bxn.hysaishi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lxd.wangdashe.top

[S34] C++：遍历 vector
来源：http://uun.epnwcf.com

for (auto &x : v) { std::cout << x; }
来源：http://xvq.haohaochexian.top

[S35] C++：map
来源：http://ngj.ywan-chungtsiang.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fdc.xingfuxueyuan.xyz

[S36] C++：unordered_map
来源：http://vjl.jlsjyb.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://puf.shuidangran.top

[S37] C++：set
来源：http://bek.iojbl.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wkc.ywan-chungtsiang.top

[S38] C++：排序
来源：http://lce.fzhhl.top

std::sort(v.begin(), v.end());
来源：http://zhe.yuxming.cn

[S39] C++：自定义比较器排序
来源：http://naa.xziqi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dod.nanxuanxn.top

[S40] C++：查找元素
来源：http://dec.ivvv.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wev.fehbvm.com

[S41] C++：类与构造函数
来源：http://odh.jyoumei.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vxn.daria6918.cn

[S42] C++：继承与虚函数
来源：http://ehh.chenzaomai.com

class B : public Base { public: void f() override {} };
来源：http://kix.cqqwz.cn

[S43] C++：智能指针
来源：http://rdl.guowangkeji.top

auto p = std::make_unique<int>(5);
来源：http://okw.gogol.net.cn

[S44] C++：引用传参
来源：http://aku.316326.xyz

void inc(int &x) { ++x; }
来源：http://yyi.sysykeji.top

[S45] C++：lambda
来源：http://eem.cucudq.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vom.ivvv.top

[S46] C++：函数模板
来源：http://bpn.ybcxt.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://heb.birdmap.top

[S47] C++：结构化绑定遍历
来源：http://rml.andypj.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rmu.9152youxi.cn

[S48] C++：逐行读文件
来源：http://xny.jlsjyb.cn

std::ifstream in("a.txt");  std::string line;
来源：http://kyr.52xcode.cn

while (std::getline(in, line)) { }
来源：http://pzv.xylfe.cn

[S49] C++：写文件
来源：http://nlm.xingfuxueyuan.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zkl.zhoulong.xyz

[S50] C++：格式化数字
来源：http://mpe.cheryme.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nua.yvedp.cn

[S51] C++：显式类型转换
来源：http://arj.hfpthk.cn

static_cast<double>(a) / b
来源：http://swd.iojbl.cn

[S52] C++：const 与 noexcept
来源：http://vty.yfazqb.com

int size() const noexcept { return n_; }
来源：http://frm.sysykeji.top

[S53] C++：移动语义
来源：http://iry.c1oappe.top

std::vector<int> w = std::move(v);
来源：http://ghm.iojbl.cn

[S54] C++：异常处理
来源：http://awv.ctjpmb.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qaz.jinghuilouyu.cn

[S55] C++：结构化绑定
来源：http://bfc.sjlbkw.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://miy.shuidangran.top

[S56] C++：optional
来源：http://awo.hfpthk.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cay.andypj.xyz

[S57] C++：编译期常量
来源：http://vsz.gotoacloud.top

constexpr int N = 10;
来源：http://ugy.yuanzhike.top

[S58] C++：命名空间
来源：http://jzr.svipenyu.cn

namespace ns { int f() { return 1; } }
来源：http://jym.svipenyu.cn

[S59] C++：静态断言
来源：http://mti.xingfuxueyuan.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://phf.xuetiantiany.cn

[S60] C++：遍历并删除元素
来源：http://roj.tianlin.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vny.tian-w.cn

================================================================================
来源：http://bet.jlsjyb.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hqu.havefunace.top

================================================================================
来源：http://mct.yfazqb.com

[T01] Kotlin：Hello World
来源：http://aij.jianghu66.top

println("Hello")
来源：http://fmp.ydzc1.top

[T02] Kotlin：变量
来源：http://lqz.xylfe.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ovr.meibo888.top

[T03] Kotlin：字符串模板
来源：http://udm.yj20258888.top

"值: $b"
来源：http://zud.hysaishi.cn

[T04] Kotlin：空安全
来源：http://kuq.hywenlv.cn

val n: String? = null;  n?.length
来源：http://gia.xuetiantiany.cn

[T05] Kotlin：when 表达式
来源：http://avk.havefunace.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mpa.daria6918.cn

[T06] Kotlin：集合映射
来源：http://uwv.zhoulong.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://cvn.fanxiaobao.xyz

[T07] Kotlin：集合过滤
来源：http://eiy.shuidangran.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://yuf.chenzaomai.com

[T08] Kotlin：数据类
来源：http://lbj.hywenlv.cn

data class User(val name: String, val age: Int)
来源：http://uib.shuidangran.top

[T09] Kotlin：扩展函数
来源：http://grj.bbcook.cn

fun String.exclaim() = this + "!"
来源：http://xqy.xuetiantiany.cn

[T10] Kotlin：默认参数
来源：http://ckw.zhijiandao.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://bvb.sxryk.cn

[T11] Kotlin：协程
来源：http://yen.guowangkeji.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://jaw.xziqi.cn

[T12] Kotlin：解构声明
来源：http://qfs.zdbjq.cn

val (a, b) = Pair(1, 2)
来源：http://dws.fzhhl.top

[T13] Kotlin：只读 Map
来源：http://xgl.hfpthk.cn

val m = mapOf("a" to 1)
来源：http://ctp.jqgufenzy.top

[T14] Kotlin：循环
来源：http://wqp.yanxiufei.cn

for (i in 1..10) println(i)
来源：http://zzy.xuanzx.com

[T15] Kotlin：接口
来源：http://iaz.birdmap.top

interface Shape { fun area(): Double }
来源：http://ajl.jinqigufen.top

[T16] Swift：Hello World
来源：http://lhx.yuanzhike.top

print("Hello")
来源：http://scp.sysykeji.top

[T17] Swift：变量与常量
来源：http://xvz.ydzc1.top

var a = 1;  let b = 2
来源：http://jjw.jinqigfzy.top

[T18] Swift：字符串插值
来源：http://rcv.nanxinkj.top

"值: \(b)"
来源：http://kab.birdmap.top

[T19] Swift：可选绑定
来源：http://kmo.fanxiaobao.xyz

if let n = opt { print(n) }
来源：http://ief.ppjwa.cn

[T20] Swift：数组操作
来源：http://qfh.zhengqikj.top

var a = [1, 2, 3];  a.append(4)
来源：http://rfd.aibaodan.cn

[T21] Swift：遍历
来源：http://qhm.aizwys.cn

for x in a { print(x) }
来源：http://msk.shangyingyoupin.top

[T22] Swift：字典
来源：http://mzy.ctjpmb.com

var d = ["a": 1];  d["b"] = 2
来源：http://fpv.cqqwz.cn

[T23] Swift：函数
来源：http://acc.zhongyouzk.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jyn.jqgufenzy.top

[T24] Swift：闭包
来源：http://duj.uphjek.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://qyr.jianghu66.top

[T25] Swift：结构体
来源：http://roy.cashguo.top

struct P { var x: Int }
来源：http://vnz.fanxiaobao.xyz

[T26] Swift：类与重写
来源：http://rfh.gotoacloud.top

class A: Base { override func f() {} }
来源：http://xrc.hfpthk.cn

[T27] Swift：错误处理
来源：http://yey.hesvh.cn

do { try f() } catch { print(error) }
来源：http://twl.hfpthk.cn

[T28] Swift：枚举
来源：http://egk.tian-w.cn

enum Color { case red, green }
来源：http://ztw.zhiwuduotai.top

[T29] Swift：guard 提前返回
来源：http://zoh.bbcook.cn

guard let x = opt else { return }
来源：http://pes.quarkkingdee.top

[T30] Swift：协议
来源：http://eje.andypj.xyz

protocol Shape { func area() -> Double }
来源：http://une.fzhhl.top

[T31] Lua：Hello World
来源：http://kto.yuanzhike.top

print("Hello")
来源：http://pnn.jqgufenzy.top

[T32] Lua：局部变量
来源：http://rnd.tanke756.top

local a = 1
来源：http://tqc.guowangkeji.top

[T33] Lua：表（数组）
来源：http://rvt.hfpthk.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fmz.jlsjyb.cn

[T34] Lua：遍历表
来源：http://bvc.zhixingplan.top

for i, v in ipairs(t) do print(i, v) end
来源：http://rps.yonumen.top

[T35] Lua：字典表
来源：http://rvr.jyoumei.cn

local d = { a = 1 };  d.b = 2
来源：http://rvx.ehwqpu.com

[T36] Lua：函数
来源：http://xap.vqdsnc.cn

function add(a, b) return a + b end
来源：http://nbj.cqqwz.cn

[T37] Lua：字符串拼接
来源：http://ayl.sxryk.cn

"a" .. "b"
来源：http://ysn.jianghu66.top

[T38] Lua：条件
来源：http://tem.9152youxi.cn

if x > 0 then print("正") end
来源：http://rbv.havefunace.top

[T39] Lua：模式匹配
来源：http://ghx.sxryk.cn

string.find(s, "%d+")
来源：http://vui.ppjwa.cn

[T40] Lua：元表
来源：http://uwu.cdnleiting.top

setmetatable({}, { __index = base })
来源：http://ncs.xinyue.icu

[T41] Perl：Hello World
来源：http://mmq.tanke756.top

print "Hello\n";
来源：http://niw.52xcode.cn

[T42] Perl：变量类型
来源：http://gjn.sufxvd.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hvw.chenjidiqi.icu


<!-- 参考信息 -->