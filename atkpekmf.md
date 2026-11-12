代发 wailian999

cmd > out.log 2>&1
来源：http://pvl.sxryk.cn

[R40] 追加写日志
来源：http://kzh.feifeiyinyue.top

echo "log" >> out.log
来源：http://twf.nanxuanxn.top

[R41] 丢弃输出
来源：http://lyd.cashguo.top

cmd >/dev/null 2>&1
来源：http://vuo.andypj.xyz

[R42] 输入重定向
来源：http://mjn.zhoulong.xyz

wc -l < a.txt
来源：http://lit.yanxiufei.cn

[R43] 按名字查找文件
来源：http://sau.sufxvd.cn

find . -name "*.log" -type f
来源：http://chf.fzhhl.top

[R44] 按修改时间查找
来源：http://woz.yfazqb.com

find . -mtime -7 -type f
来源：http://adc.wangdashe.top

[R45] 批量删除
来源：http://ehu.tian-w.cn

find . -name "*.tmp" -delete
来源：http://iyy.feifeiyinyue.top

[R46] 递归替换文件内容
来源：http://rhg.hongshengwenyu.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dqu.guowangkeji.top

[R47] sed 单行替换
来源：http://ffv.jianghu66.top

sed -i 's/foo/bar/g' a.txt
来源：http://fqu.ppjwa.cn

[R48] awk 取指定列
来源：http://oyi.jqgfzy.top

awk '{print $1, $3}' a.txt
来源：http://kye.zhoulong.xyz

[R49] awk 带条件
来源：http://tzh.jinyuanbaomall.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wak.zdbjq.cn

[R50] awk 求和
来源：http://zzp.havefunace.top

awk '{s += $2} END {print s}' a.txt
来源：http://hah.nwbrower.top

[R51] 排序去重取前几
来源：http://edu.havefunace.top

sort a.txt | uniq -c | sort -rn | head
来源：http://zml.ppjwa.cn

[R52] 统计行数
来源：http://tvq.shanyushiyangtech.top

wc -l a.txt
来源：http://lhd.haohaochexian.top

[R53] 查看文件头与实时尾
来源：http://rqh.zhijiandao.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qjl.cucudq.cn

[R54] 比较两个文件
来源：http://vhx.cdnleiting.top

diff a.txt b.txt
来源：http://khz.yfazqb.com

[R55] 压缩与解压
来源：http://mva.yangfankeji.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://sid.zhixingplan.top

[R56] 远程拷贝
来源：http://wht.shangyingyoupin.top

scp file user@host:/path/
来源：http://qbc.ydzc1.top

[R57] 远程执行命令
来源：http://czs.vehdjk.com

ssh user@host 'uptime'
来源：http://iep.sjlbkw.cn

[R58] 下载文件
来源：http://veq.9152youxi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dnr.pengpengdd.cyou

[R59] 发 POST JSON
来源：http://ccb.feifeiyinyue.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://opm.hongshengwenyu.top

[R60] 只看 HTTP 状态码
来源：http://pex.sweek.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://krq.hnqzz.top

[R61] 磁盘占用
来源：http://oin.jqgufenzy.top

df -h;  du -sh *
来源：http://tcr.sufxvd.cn

[R62] 找最占空间的文件
来源：http://aij.snrcjt.cn

du -ah . | sort -rh | head -10
来源：http://sga.gaohongyu789.top

[R63] 内存与进程
来源：http://omf.feifeiyinyue.top

free -h;  ps aux | grep nginx
来源：http://xfe.snrcjt.cn

[R64] 结束进程
来源：http://usf.meibo888.top

kill -9 $(pgrep -f app.py)
来源：http://jyl.yongpay.top

[R65] 查看端口占用
来源：http://yzt.yfazqb.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vta.hywenlv.cn

[R66] 定时任务
来源：http://ijd.tian-w.cn

crontab -e;  crontab -l
来源：http://txa.quarkkingdee.top

[R67] 生成随机十六进制串
来源：http://pui.mhx1999.top

openssl rand -hex 16
来源：http://ipo.jiagoushi.top

[R68] 计算文件校验值
来源：http://wzb.zhijiandao.cn

sha256sum a.txt;  md5sum a.txt
来源：http://rvq.jiagoushi.top

[R69] 生成随机密码
来源：http://uya.sufxvd.cn

head -c 16 /dev/urandom | base64
来源：http://dpn.9152youxi.cn

[R70] 时间戳与互转
来源：http://rku.bjfxy.top

date +%s;  date -d @1700000000
来源：http://zvg.chenjidiqi.icu

[R71] 日期格式化
来源：http://oon.svipenyu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://jlr.fanxiaobao.xyz

[R72] 等待端口就绪
来源：http://lcz.mhx1999.top

until nc -z localhost 3306; do sleep 1; done
来源：http://cik.zdqjudy.top

[R73] 分割大日志
来源：http://cmh.zhixingplan.top

split -l 1000 big.log part_
来源：http://den.fengsongda.top

[R74] 批量重命名
来源：http://qhs.feifeiyinyue.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bfa.chenjidiqi.icu

[R75] 导出环境变量
来源：http://nyy.hywenlv.cn

export PATH="$HOME/bin:$PATH"
来源：http://gue.gzhubu.top

[R76] 使用临时文件
来源：http://qow.iojbl.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dcn.xuetiantiany.cn

[R77] 读取用户输入
来源：http://lxh.cashguo.top

read -rp "请输入: " ans
来源：http://dbb.shzxlz.cn

[R78] 交互式菜单
来源：http://wil.xuetiantiany.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zmj.yongpay.top

[R79] 解析命令行选项
来源：http://baj.vqdsnc.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nxq.fengsongda.top

[R80] 查看脚本执行耗时
来源：http://ghd.jinqigfzy.top

time ./run.sh
来源：http://iqg.hywenlv.cn

================================================================================
来源：http://ewy.c1oappe.top

S. C / C++ 专题
来源：http://cgu.pycfn.com

================================================================================
来源：http://vjb.fktsv.cn

[S01] C：Hello World
来源：http://ian.xingfuxueyuan.xyz

#include <stdio.h>
来源：http://klb.guowangkeji.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://uep.yongpay.top

[S02] C：变量与格式化输出
来源：http://nmh.gotoacloud.top

int a = 10; printf("%d\n", a);
来源：http://wfh.yfazqb.com

[S03] C：读入整数
来源：http://gdq.yj202588.top

int x; scanf("%d", &x);
来源：http://nag.yvedp.cn

[S04] C：字符串复制
来源：http://mun.yueranfly.top

char dst[32]; strcpy(dst, "hi");
来源：http://zww.havefunace.top

[S05] C：字符串长度
来源：http://jdj.xylfe.cn

strlen(s)
来源：http://ndu.9152youxi.cn

[S06] C：字符串比较
来源：http://rfs.xingfuxueyuan.xyz

strcmp(a, b) == 0
来源：http://sfk.yuxming.cn

[S07] C：数组遍历求和
来源：http://ifv.jinghuilouyu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zqv.jinyuanbaomall.cn

[S08] C：动态内存分配与释放
来源：http://rfi.hnxiangtu.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pbk.jyoumei.cn

[S09] C：结构体定义与初始化
来源：http://gid.zhijiandao.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qez.sweek.top

[S10] C：指针与解引用
来源：http://ssx.yuanzhike.top

int *p = &a;  *p = 5;
来源：http://yru.feifeiyinyue.top

[S11] C：逐行读文件
来源：http://avm.nanxinkj.top

FILE *f = fopen("a.txt", "r");
来源：http://fjt.hnxiangtu.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://dqs.vqdsnc.cn

fclose(f);
来源：http://dvb.daria6918.cn

[S12] C：写文件
来源：http://fws.zhengqikj.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vhd.pengpengdd.cyou

[S13] C：宏定义
来源：http://kkx.chenlongwang.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xti.dashuyun.cn

[S14] C：枚举
来源：http://evg.zycfv.cn

enum Color { RED, GREEN, BLUE };
来源：http://ndy.yuanzhike.top

[S15] C：类型转换
来源：http://xdy.epnwcf.com

(double) a / b
来源：http://mah.aizwys.cn

[S16] C：位操作置位
来源：http://xfp.wangshuangyany.cn

x |= (1 << 3);
来源：http://fkr.hcnkem.com

[S17] C：安全拼接字符串
来源：http://jtk.jinghuilouyu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yzu.hammf.cn

[S18] C：命令行参数
来源：http://tfb.hfpthk.cn

int main(int argc, char **argv)
来源：http://gfi.iojbl.cn

[S19] C：快速排序
来源：http://smk.0kj1m.cn

qsort(a, n, sizeof(int), cmp);
来源：http://kaj.316326.xyz

[S20] C：二分查找
来源：http://wlp.zhiwuduotai.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://llc.cashguo.top

[S21] C：字符类别判断
来源：http://xah.dashuyun.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://khx.wangshuangyany.cn

[S22] C：字符串转数字
来源：http://jhv.sufxvd.cn

atoi("42");  strtod("3.14", NULL);
来源：http://gaf.yfazqb.com

[S23] C：随机数
来源：http://oom.yongpay.top

srand(time(NULL));  int r = rand() % 100;
来源：http://vyn.sysykeji.top

[S24] C：获取本地时间
来源：http://wmr.aibaodan.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hps.9152youxi.cn

[S25] C：内存拷贝
来源：http://sla.chenjidiqi.icu

memcpy(dst, src, n);
来源：http://opl.zdbjq.cn

[S26] C：内存清零
来源：http://eyu.sjlbkw.cn

memset(a, 0, sizeof a);
来源：http://toi.yanxiufei.cn

[S27] C：定义常量
来源：http://bwz.zycfv.cn

const double PI = 3.14159;
来源：http://gnz.316326.xyz

[S28] C：静态变量
来源：http://wjf.cqqwz.cn

static int counter = 0;
来源：http://kuj.epnwcf.com

[S29] C：变参函数
来源：http://ofw.0kj1m.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wxa.xuanzx.com

[S30] C：头文件保护
来源：http://ngm.hammf.cn

#ifndef X_H
来源：http://kib.ybcxt.top

#define X_H
来源：http://fhd.jianghu66.top

#endif
来源：http://owg.chenjidiqi.icu

[S31] C++：Hello World
来源：http://ubo.sxryk.cn

#include <iostream>
来源：http://bkr.sweek.top

int main() { std::cout << "Hello\n"; }
来源：http://jzh.zhixingplan.top

[S32] C++：字符串
来源：http://ehy.gotoacloud.top

std::string s = "hi";  s += "!";
来源：http://fqc.ctjpmb.com

[S33] C++：vector 增删
来源：http://rhv.svipenyu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fsn.birdmap.top

[S34] C++：遍历 vector
来源：http://qow.cdnleiting.top

for (auto &x : v) { std::cout << x; }
来源：http://nrr.hammf.cn

[S35] C++：map
来源：http://zze.hysaishi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ych.kuanghao11.cn

[S36] C++：unordered_map
来源：http://ywi.cashguo.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qzy.sysykeji.top

[S37] C++：set
来源：http://uub.mhx1999.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rll.gogol.net.cn

[S38] C++：排序
来源：http://kzg.bbcook.cn

std::sort(v.begin(), v.end());
来源：http://nms.gogol.net.cn

[S39] C++：自定义比较器排序
来源：http://zlp.ctjpmb.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ugm.jinqigufen.top

[S40] C++：查找元素
来源：http://knv.yj202588.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vjx.jqgfzy.top

[S41] C++：类与构造函数
来源：http://kmd.kuanghao11.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://whb.hywenlv.cn

[S42] C++：继承与虚函数
来源：http://qck.jinqigufen.top

class B : public Base { public: void f() override {} };
来源：http://kfy.yanxiufei.cn

[S43] C++：智能指针
来源：http://tqi.chenlongwang.top

auto p = std::make_unique<int>(5);
来源：http://hio.shzxlz.cn

[S44] C++：引用传参
来源：http://coq.iojbl.cn

void inc(int &x) { ++x; }
来源：http://uuq.tarul.cn

[S45] C++：lambda
来源：http://kmm.ybcxt.top

auto add = [](int a, int b) { return a + b; };
来源：http://lio.gotoacloud.top

[S46] C++：函数模板
来源：http://sxh.jianghu66.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lfw.xziqi.cn

[S47] C++：结构化绑定遍历
来源：http://cje.0kj1m.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pup.zhaomingkeji.xyz

[S48] C++：逐行读文件
来源：http://ghf.sweek.top

std::ifstream in("a.txt");  std::string line;
来源：http://pxp.chenzaomai.com

while (std::getline(in, line)) { }
来源：http://qlc.sysykeji.top

[S49] C++：写文件
来源：http://bcr.havefunace.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xst.chenzaomai.com

[S50] C++：格式化数字
来源：http://ldj.ivvv.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zmv.pycfn.com

[S51] C++：显式类型转换
来源：http://odi.yonumen.top

static_cast<double>(a) / b
来源：http://waf.yj20258.top

[S52] C++：const 与 noexcept
来源：http://xbo.xuetiantiany.cn

int size() const noexcept { return n_; }
来源：http://cqn.zhiwuduotai.top

[S53] C++：移动语义
来源：http://nik.hywenlv.cn

std::vector<int> w = std::move(v);
来源：http://qhm.yongpay.top

[S54] C++：异常处理
来源：http://ckk.pengpengdd.cyou

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://urt.yonumen.top

[S55] C++：结构化绑定
来源：http://atv.chenjidiqi.icu

auto [a, b] = std::make_pair(1, 2);
来源：http://ers.chenjidiqi.icu

[S56] C++：optional
来源：http://yrd.redwolf501.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qkg.epnwcf.com

[S57] C++：编译期常量
来源：http://pga.svipenyu.cn

constexpr int N = 10;
来源：http://wij.haohaochexian.top

[S58] C++：命名空间
来源：http://har.aizwys.cn

namespace ns { int f() { return 1; } }
来源：http://ktf.birdmap.top

[S59] C++：静态断言
来源：http://cib.c1oappe.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://euf.guowangkeji.top

[S60] C++：遍历并删除元素
来源：http://sgu.52xcode.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ihe.meibo888.top

================================================================================
来源：http://xmp.9152youxi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bdd.zhengqikj.top

================================================================================
来源：http://omm.andypj.xyz

[T01] Kotlin：Hello World
来源：http://boz.cheryme.top

println("Hello")
来源：http://ceo.52xcode.cn

[T02] Kotlin：变量
来源：http://ywm.jqgufenzy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://rkr.shangyingyoupin.top

[T03] Kotlin：字符串模板
来源：http://jhs.dianchejie.cn

"值: $b"
来源：http://yli.yuanzhike.top

[T04] Kotlin：空安全
来源：http://veh.birdmap.top

val n: String? = null;  n?.length
来源：http://inv.sweek.top

[T05] Kotlin：when 表达式
来源：http://rfx.tianlin.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://buu.yuanzhike.top

[T06] Kotlin：集合映射
来源：http://lks.zdqjudy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://knr.fzhhl.top

[T07] Kotlin：集合过滤
来源：http://njl.xuetiantiany.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://stt.andypj.xyz

[T08] Kotlin：数据类
来源：http://rtd.hammf.cn

data class User(val name: String, val age: Int)
来源：http://del.yvedp.cn

[T09] Kotlin：扩展函数
来源：http://ali.52xcode.cn

fun String.exclaim() = this + "!"
来源：http://drb.zhengqikj.top

[T10] Kotlin：默认参数
来源：http://vbf.mhx1999.top

fun greet(name: String = "World") = "Hi $name"
来源：http://qio.c1oappe.top

[T11] Kotlin：协程
来源：http://hzx.yongpay.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ebt.sweek.top

[T12] Kotlin：解构声明
来源：http://nvu.jiagoushi.top

val (a, b) = Pair(1, 2)
来源：http://alw.dianchejie.cn

[T13] Kotlin：只读 Map
来源：http://iyr.andypj.xyz

val m = mapOf("a" to 1)
来源：http://uvx.zhongyouzk.top

[T14] Kotlin：循环
来源：http://ghu.ywan-chungtsiang.top

for (i in 1..10) println(i)
来源：http://mdl.sufxvd.cn

[T15] Kotlin：接口
来源：http://vrw.feifeiyinyue.top

interface Shape { fun area(): Double }
来源：http://occ.shangyingyoupin.top

[T16] Swift：Hello World
来源：http://rtq.nanxuanxn.top

print("Hello")
来源：http://wtp.jinghuilouyu.cn

[T17] Swift：变量与常量
来源：http://rki.dianchejie.cn

var a = 1;  let b = 2
来源：http://glc.tarul.cn

[T18] Swift：字符串插值
来源：http://enp.hfpthk.cn

"值: \(b)"
来源：http://uaq.tarul.cn

[T19] Swift：可选绑定
来源：http://ymq.nanxuanxn.top

if let n = opt { print(n) }
来源：http://dzb.zhengqikj.top

[T20] Swift：数组操作
来源：http://fxc.smart0.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://wqk.yuxming.cn

[T21] Swift：遍历
来源：http://zlg.dashuyun.cn

for x in a { print(x) }
来源：http://czi.yvedp.cn

[T22] Swift：字典
来源：http://tsm.yonumen.top

var d = ["a": 1];  d["b"] = 2
来源：http://nfs.tianlin.xyz

[T23] Swift：函数
来源：http://axx.jlsjyb.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pyl.ctjpmb.com

[T24] Swift：闭包
来源：http://vzf.hnxiangtu.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://qgm.zdbjq.cn

[T25] Swift：结构体
来源：http://fye.sxryk.cn

struct P { var x: Int }
来源：http://zig.yvedp.cn

[T26] Swift：类与重写
来源：http://fdi.daria6918.cn

class A: Base { override func f() {} }
来源：http://dsw.dianchejie.cn

[T27] Swift：错误处理
来源：http://oks.tianlin.xyz

do { try f() } catch { print(error) }
来源：http://eyd.ydjk.org.cn

[T28] Swift：枚举
来源：http://jdy.xuanzx.com

enum Color { case red, green }
来源：http://pbb.shangyingyoupin.top

[T29] Swift：guard 提前返回
来源：http://cot.yanxiufei.cn

guard let x = opt else { return }
来源：http://bqe.epnwcf.com

[T30] Swift：协议
来源：http://npu.pycfn.com

protocol Shape { func area() -> Double }
来源：http://ygs.daxiang520.top

[T31] Lua：Hello World
来源：http://smu.pycfn.com

print("Hello")
来源：http://kcd.chenzaomai.com

[T32] Lua：局部变量
来源：http://kco.jqgfzy.top

local a = 1
来源：http://ben.ydjk.org.cn

[T33] Lua：表（数组）
来源：http://oak.sufxvd.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://jtp.snrcjt.cn

[T34] Lua：遍历表
来源：http://xrw.jyoumei.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://pzq.smart0.xyz

[T35] Lua：字典表
来源：http://gyo.guannengcc.top

local d = { a = 1 };  d.b = 2
来源：http://jjo.yvedp.cn

[T36] Lua：函数
来源：http://usk.sweek.top

function add(a, b) return a + b end
来源：http://hai.pycfn.com

[T37] Lua：字符串拼接
来源：http://tux.hesvh.cn

"a" .. "b"
来源：http://taa.hesvh.cn

[T38] Lua：条件
来源：http://ynu.sxryk.cn

if x > 0 then print("正") end
来源：http://vlq.yuanzhike.top

[T39] Lua：模式匹配
来源：http://oiz.chenlongwang.top

string.find(s, "%d+")
来源：http://ufv.yangfankeji.com

[T40] Lua：元表
来源：http://mri.hywenlv.cn

setmetatable({}, { __index = base })
来源：http://uho.yvedp.cn

[T41] Perl：Hello World
来源：http://txt.yfazqb.com

print "Hello\n";
来源：http://pdb.shuidangran.top

[T42] Perl：变量类型
来源：http://fkh.xuetiantiany.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kdh.cheryme.top


<!-- 参考信息 -->