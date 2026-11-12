代发 wailian999

files=$(ls -1)
来源：http://bzt.c1oappe.top

[R38] 管道串联
来源：http://vzb.fktsv.cn

cat a.txt | grep -i error | wc -l
来源：http://glr.jyoumei.cn

[R39] 重定向标准输出与错误
来源：http://dhv.gzhubu.top

cmd > out.log 2>&1
来源：http://gnt.hnxiangtu.top

[R40] 追加写日志
来源：http://bda.jianghu66.top

echo "log" >> out.log
来源：http://bcs.pengpengdd.cyou

[R41] 丢弃输出
来源：http://zyu.yj20258.top

cmd >/dev/null 2>&1
来源：http://tvq.hesvh.cn

[R42] 输入重定向
来源：http://eow.uphjek.com

wc -l < a.txt
来源：http://qgx.ivvv.top

[R43] 按名字查找文件
来源：http://oxp.ctjpmb.com

find . -name "*.log" -type f
来源：http://xlk.ywan-chungtsiang.top

[R44] 按修改时间查找
来源：http://ygc.chenlongwang.top

find . -mtime -7 -type f
来源：http://qda.cdnleiting.top

[R45] 批量删除
来源：http://zuw.jqgfzy.top

find . -name "*.tmp" -delete
来源：http://oky.nanxinkj.top

[R46] 递归替换文件内容
来源：http://fjn.nwbrower.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mti.zhiwuduotai.top

[R47] sed 单行替换
来源：http://igz.zhongyouzk.top

sed -i 's/foo/bar/g' a.txt
来源：http://drc.yuanzhike.top

[R48] awk 取指定列
来源：http://key.xinyue.icu

awk '{print $1, $3}' a.txt
来源：http://izx.316326.xyz

[R49] awk 带条件
来源：http://ypi.52xcode.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://frs.wangshuangyany.cn

[R50] awk 求和
来源：http://fun.vqdsnc.cn

awk '{s += $2} END {print s}' a.txt
来源：http://rao.nwbrower.top

[R51] 排序去重取前几
来源：http://yud.svipenyu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://htp.svipenyu.cn

[R52] 统计行数
来源：http://evy.pycfn.com

wc -l a.txt
来源：http://gpo.shuidangran.top

[R53] 查看文件头与实时尾
来源：http://tlw.yanxiufei.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cqa.ivvv.top

[R54] 比较两个文件
来源：http://ggq.tanke756.top

diff a.txt b.txt
来源：http://thw.haohaochexian.top

[R55] 压缩与解压
来源：http://ras.yonumen.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://plc.smart0.xyz

[R56] 远程拷贝
来源：http://oqy.ivvv.top

scp file user@host:/path/
来源：http://ylz.jiagoushi.top

[R57] 远程执行命令
来源：http://tus.bbcook.cn

ssh user@host 'uptime'
来源：http://uid.sjlbkw.cn

[R58] 下载文件
来源：http://pxb.zhiwuduotai.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fzi.chenjidiqi.icu

[R59] 发 POST JSON
来源：http://ezc.jlsjyb.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sez.aizwys.cn

[R60] 只看 HTTP 状态码
来源：http://fpy.cheryme.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nys.uphjek.com

[R61] 磁盘占用
来源：http://hxp.andypj.xyz

df -h;  du -sh *
来源：http://neu.hesvh.cn

[R62] 找最占空间的文件
来源：http://coi.hysaishi.cn

du -ah . | sort -rh | head -10
来源：http://ugm.hongshengwenyu.top

[R63] 内存与进程
来源：http://wep.nwbrower.top

free -h;  ps aux | grep nginx
来源：http://uvz.jlsjyb.cn

[R64] 结束进程
来源：http://kvo.zhengqikj.top

kill -9 $(pgrep -f app.py)
来源：http://fac.jinghuilouyu.cn

[R65] 查看端口占用
来源：http://zvx.ehwqpu.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://orh.daria6918.cn

[R66] 定时任务
来源：http://hji.jianghu66.top

crontab -e;  crontab -l
来源：http://cqn.sysykeji.top

[R67] 生成随机十六进制串
来源：http://jiu.jinyuanbaomall.cn

openssl rand -hex 16
来源：http://tms.birdmap.top

[R68] 计算文件校验值
来源：http://gob.birdmap.top

sha256sum a.txt;  md5sum a.txt
来源：http://jbi.sxryk.cn

[R69] 生成随机密码
来源：http://zog.yfazqb.com

head -c 16 /dev/urandom | base64
来源：http://tmy.tanke756.top

[R70] 时间戳与互转
来源：http://xly.zhaomingkeji.xyz

date +%s;  date -d @1700000000
来源：http://crz.zdqjudy.top

[R71] 日期格式化
来源：http://hsk.ppjwa.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://xpe.snrcjt.cn

[R72] 等待端口就绪
来源：http://ugw.dashuyun.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://pxn.wangdashe.top

[R73] 分割大日志
来源：http://zsv.guowangkeji.top

split -l 1000 big.log part_
来源：http://huq.yuanzhike.top

[R74] 批量重命名
来源：http://ckk.yanxiufei.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://puj.xziqi.cn

[R75] 导出环境变量
来源：http://llx.shuidangran.top

export PATH="$HOME/bin:$PATH"
来源：http://rki.hcnkem.com

[R76] 使用临时文件
来源：http://esd.smart0.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://euu.wangdashe.top

[R77] 读取用户输入
来源：http://xii.jyoumei.cn

read -rp "请输入: " ans
来源：http://ssh.vqdsnc.cn

[R78] 交互式菜单
来源：http://ylk.yuanzhike.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ffp.aibaodan.cn

[R79] 解析命令行选项
来源：http://hjg.quarkkingdee.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://aip.jinyuanbaomall.cn

[R80] 查看脚本执行耗时
来源：http://eic.yuanzhike.top

time ./run.sh
来源：http://vvr.birdmap.top

================================================================================
来源：http://crb.andypj.xyz

S. C / C++ 专题
来源：http://sjo.jqgufenzy.top

================================================================================
来源：http://rrw.fktsv.cn

[S01] C：Hello World
来源：http://txw.52xcode.cn

#include <stdio.h>
来源：http://eos.xylfe.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://alu.daxiang520.top

[S02] C：变量与格式化输出
来源：http://gzv.meibo888.top

int a = 10; printf("%d\n", a);
来源：http://zvc.bbcook.cn

[S03] C：读入整数
来源：http://dqw.tian-w.cn

int x; scanf("%d", &x);
来源：http://zrh.feifeiyinyue.top

[S04] C：字符串复制
来源：http://vjf.nanxuanxn.top

char dst[32]; strcpy(dst, "hi");
来源：http://fly.jqgufenzy.top

[S05] C：字符串长度
来源：http://azr.zdqjudy.top

strlen(s)
来源：http://jmk.cdnleiting.top

[S06] C：字符串比较
来源：http://ewo.shanyushiyangkeji.top

strcmp(a, b) == 0
来源：http://jhe.jinqigufen.top

[S07] C：数组遍历求和
来源：http://wsf.tian-w.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yvc.aizwys.cn

[S08] C：动态内存分配与释放
来源：http://czv.c1oappe.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qje.0kj1m.cn

[S09] C：结构体定义与初始化
来源：http://wve.fzhhl.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://moi.yanxiufei.cn

[S10] C：指针与解引用
来源：http://ayf.tianlin.xyz

int *p = &a;  *p = 5;
来源：http://hoh.xylfe.cn

[S11] C：逐行读文件
来源：http://jiy.ppjwa.cn

FILE *f = fopen("a.txt", "r");
来源：http://lau.redwolf501.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://atc.hammf.cn

fclose(f);
来源：http://pys.cheryme.top

[S12] C：写文件
来源：http://hmn.yonumen.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kax.zhixingplan.top

[S13] C：宏定义
来源：http://kbt.yueranfly.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pie.hysaishi.cn

[S14] C：枚举
来源：http://nqc.shzxlz.cn

enum Color { RED, GREEN, BLUE };
来源：http://bwr.gaohongyu789.top

[S15] C：类型转换
来源：http://dwv.jinghuilouyu.cn

(double) a / b
来源：http://unl.xingfuxueyuan.xyz

[S16] C：位操作置位
来源：http://oio.hongshengwenyu.top

x |= (1 << 3);
来源：http://xni.bjfxy.top

[S17] C：安全拼接字符串
来源：http://vmv.kuanghao11.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tpu.sysykeji.top

[S18] C：命令行参数
来源：http://cnz.nanxinkj.top

int main(int argc, char **argv)
来源：http://idz.birdmap.top

[S19] C：快速排序
来源：http://ctc.tian-w.cn

qsort(a, n, sizeof(int), cmp);
来源：http://uls.shanyushiyangkeji.top

[S20] C：二分查找
来源：http://cvs.zhongyouzk.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://owh.sysykeji.top

[S21] C：字符类别判断
来源：http://fab.fehbvm.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lwo.pengpengdd.cyou

[S22] C：字符串转数字
来源：http://fjo.ivvv.top

atoi("42");  strtod("3.14", NULL);
来源：http://yfn.hfpthk.cn

[S23] C：随机数
来源：http://ceo.sysykeji.top

srand(time(NULL));  int r = rand() % 100;
来源：http://uhp.sufxvd.cn

[S24] C：获取本地时间
来源：http://pzy.cashguo.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vaj.cdnleiting.top

[S25] C：内存拷贝
来源：http://eur.vehdjk.com

memcpy(dst, src, n);
来源：http://vhm.daria6918.cn

[S26] C：内存清零
来源：http://aun.jqgufenzy.top

memset(a, 0, sizeof a);
来源：http://xzk.aizwys.cn

[S27] C：定义常量
来源：http://abh.hnxiangtu.top

const double PI = 3.14159;
来源：http://wkb.bbcook.cn

[S28] C：静态变量
来源：http://zpu.yanxiufei.cn

static int counter = 0;
来源：http://num.zhixingplan.top

[S29] C：变参函数
来源：http://lgq.svipenyu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nzd.zhaomingkeji.xyz

[S30] C：头文件保护
来源：http://grc.pycfn.com

#ifndef X_H
来源：http://oxo.jqgufenzy.top

#define X_H
来源：http://hkw.sweek.top

#endif
来源：http://vqv.hcnkem.com

[S31] C++：Hello World
来源：http://xmk.feifeiyinyue.top

#include <iostream>
来源：http://mgm.ivvv.top

int main() { std::cout << "Hello\n"; }
来源：http://pip.sjlbkw.cn

[S32] C++：字符串
来源：http://mqi.gzhubu.top

std::string s = "hi";  s += "!";
来源：http://avo.haohaochexian.top

[S33] C++：vector 增删
来源：http://zjx.shanyushiyangtech.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zvq.zhiwuduotai.top

[S34] C++：遍历 vector
来源：http://bgr.chenlongwang.top

for (auto &x : v) { std::cout << x; }
来源：http://zpy.tianlin.xyz

[S35] C++：map
来源：http://ihw.hammf.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gwn.yongpay.top

[S36] C++：unordered_map
来源：http://dqv.316326.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fge.yuxming.cn

[S37] C++：set
来源：http://wnk.cucudq.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://smi.hammf.cn

[S38] C++：排序
来源：http://tfb.hongshengwenyu.top

std::sort(v.begin(), v.end());
来源：http://kru.jinghuilouyu.cn

[S39] C++：自定义比较器排序
来源：http://hiy.vqdsnc.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lzr.tanke756.top

[S40] C++：查找元素
来源：http://vat.9152youxi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://etf.guowangkeji.top

[S41] C++：类与构造函数
来源：http://spb.yanxiufei.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mss.smart0.xyz

[S42] C++：继承与虚函数
来源：http://yqz.daria6918.cn

class B : public Base { public: void f() override {} };
来源：http://kbc.jinqigufen.top

[S43] C++：智能指针
来源：http://yds.316326.xyz

auto p = std::make_unique<int>(5);
来源：http://cmw.chenlongwang.top

[S44] C++：引用传参
来源：http://zdg.zhengqikj.top

void inc(int &x) { ++x; }
来源：http://vey.sxryk.cn

[S45] C++：lambda
来源：http://bew.sxryk.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bqi.gaohongyu789.top

[S46] C++：函数模板
来源：http://emn.hesvh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ycc.fengsongda.top

[S47] C++：结构化绑定遍历
来源：http://zro.hywenlv.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rfd.yuxming.cn

[S48] C++：逐行读文件
来源：http://qwc.jinqigfzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://bvn.cucudq.cn

while (std::getline(in, line)) { }
来源：http://nkk.vqdsnc.cn

[S49] C++：写文件
来源：http://xkm.jqgufenzy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ucv.jyoumei.cn

[S50] C++：格式化数字
来源：http://ifr.shanyushiyangtech.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xjg.feifeiyinyue.top

[S51] C++：显式类型转换
来源：http://nnn.nanxuanxn.top

static_cast<double>(a) / b
来源：http://mmg.fktsv.cn

[S52] C++：const 与 noexcept
来源：http://moj.yanxiufei.cn

int size() const noexcept { return n_; }
来源：http://zkm.shanyushiyangtech.top

[S53] C++：移动语义
来源：http://tpv.shzxlz.cn

std::vector<int> w = std::move(v);
来源：http://qnq.zhijiandao.cn

[S54] C++：异常处理
来源：http://plq.hywenlv.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://auu.birdmap.top

[S55] C++：结构化绑定
来源：http://arf.jinyuanbaomall.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://irm.tanke756.top

[S56] C++：optional
来源：http://bxx.uphjek.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fyd.ctjpmb.com

[S57] C++：编译期常量
来源：http://bgw.gotoacloud.top

constexpr int N = 10;
来源：http://zss.ydzc1.top

[S58] C++：命名空间
来源：http://fgo.xinyue.icu

namespace ns { int f() { return 1; } }
来源：http://sqb.yj20258.top

[S59] C++：静态断言
来源：http://dxt.yonumen.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gzo.wangdashe.top

[S60] C++：遍历并删除元素
来源：http://zuy.yuanzhike.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qqm.nanxinkj.top

================================================================================
来源：http://jld.yuanzhike.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hyp.ctjpmb.com

================================================================================
来源：http://koa.aizwys.cn

[T01] Kotlin：Hello World
来源：http://did.shzxlz.cn

println("Hello")
来源：http://mhn.birdmap.top

[T02] Kotlin：变量
来源：http://dwy.cqqwz.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xdk.pycfn.com

[T03] Kotlin：字符串模板
来源：http://laj.pycfn.com

"值: $b"
来源：http://vej.yfazqb.com

[T04] Kotlin：空安全
来源：http://eie.zhongyouzk.top

val n: String? = null;  n?.length
来源：http://chk.shuidangran.top

[T05] Kotlin：when 表达式
来源：http://epn.yj202588.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://saf.316326.xyz

[T06] Kotlin：集合映射
来源：http://psj.fengsongda.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ppu.ydzc1.top

[T07] Kotlin：集合过滤
来源：http://hxu.tian-w.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://uca.yuxming.cn

[T08] Kotlin：数据类
来源：http://ubd.cashguo.top

data class User(val name: String, val age: Int)
来源：http://qid.wangdashe.top

[T09] Kotlin：扩展函数
来源：http://eck.pycfn.com

fun String.exclaim() = this + "!"
来源：http://thd.tanke756.top

[T10] Kotlin：默认参数
来源：http://ecf.jianghu66.top

fun greet(name: String = "World") = "Hi $name"
来源：http://qmu.bjfxy.top

[T11] Kotlin：协程
来源：http://mse.sweek.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://rkb.zhoulong.xyz

[T12] Kotlin：解构声明
来源：http://arh.hysaishi.cn

val (a, b) = Pair(1, 2)
来源：http://vkc.sxryk.cn

[T13] Kotlin：只读 Map
来源：http://meb.hongshengwenyu.top

val m = mapOf("a" to 1)
来源：http://qqg.andypj.xyz

[T14] Kotlin：循环
来源：http://fqp.jinyuanbaomall.cn

for (i in 1..10) println(i)
来源：http://ctk.yuxming.cn

[T15] Kotlin：接口
来源：http://utb.yfazqb.com

interface Shape { fun area(): Double }
来源：http://gui.ehwqpu.com

[T16] Swift：Hello World
来源：http://elc.jinqigfzy.top

print("Hello")
来源：http://ngh.meibo888.top

[T17] Swift：变量与常量
来源：http://cjl.ywan-chungtsiang.top

var a = 1;  let b = 2
来源：http://pov.xuetiantiany.cn

[T18] Swift：字符串插值
来源：http://qko.yj202588.top

"值: \(b)"
来源：http://eqd.sweek.top

[T19] Swift：可选绑定
来源：http://slo.tanke756.top

if let n = opt { print(n) }
来源：http://iev.yangfankeji.com

[T20] Swift：数组操作
来源：http://nuk.yangfankeji.com

var a = [1, 2, 3];  a.append(4)
来源：http://qfx.mhx1999.top

[T21] Swift：遍历
来源：http://tuo.fzhhl.top

for x in a { print(x) }
来源：http://zxu.andypj.xyz

[T22] Swift：字典
来源：http://kxo.guannengcc.top

var d = ["a": 1];  d["b"] = 2
来源：http://kgl.sweek.top

[T23] Swift：函数
来源：http://snq.jinyuanbaomall.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fvr.birdmap.top

[T24] Swift：闭包
来源：http://xep.shangyingyoupin.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://prm.hnxiangtu.top

[T25] Swift：结构体
来源：http://rtx.zdqjudy.top

struct P { var x: Int }
来源：http://kis.sysykeji.top

[T26] Swift：类与重写
来源：http://rty.aizwys.cn

class A: Base { override func f() {} }
来源：http://xnq.jlsjyb.cn

[T27] Swift：错误处理
来源：http://rtx.xylfe.cn

do { try f() } catch { print(error) }
来源：http://dff.haohaochexian.top

[T28] Swift：枚举
来源：http://zot.c1oappe.top

enum Color { case red, green }
来源：http://idd.hywenlv.cn

[T29] Swift：guard 提前返回
来源：http://ciz.kuanghao11.cn

guard let x = opt else { return }
来源：http://kho.gzhubu.top

[T30] Swift：协议
来源：http://doc.cdnleiting.top

protocol Shape { func area() -> Double }
来源：http://hea.yfazqb.com

[T31] Lua：Hello World
来源：http://zws.zhijiandao.cn

print("Hello")
来源：http://pdi.jqgufenzy.top

[T32] Lua：局部变量
来源：http://loo.xuanzx.com

local a = 1
来源：http://tkf.yueranfly.top

[T33] Lua：表（数组）
来源：http://kek.c1oappe.top

local t = {1, 2, 3};  t[4] = 4
来源：http://zfr.sysykeji.top

[T34] Lua：遍历表
来源：http://rhb.jyoumei.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ucs.fengsongda.top

[T35] Lua：字典表
来源：http://rpl.vqdsnc.cn

local d = { a = 1 };  d.b = 2
来源：http://qua.c1oappe.top

[T36] Lua：函数
来源：http://qgj.aibaodan.cn

function add(a, b) return a + b end
来源：http://nvz.birdmap.top

[T37] Lua：字符串拼接
来源：http://ers.yuanzhike.top

"a" .. "b"
来源：http://shc.yonumen.top

[T38] Lua：条件
来源：http://lkt.smart0.xyz

if x > 0 then print("正") end
来源：http://rfe.ehwqpu.com

[T39] Lua：模式匹配
来源：http://yoz.yanxiufei.cn

string.find(s, "%d+")
来源：http://bqu.ctjpmb.com

[T40] Lua：元表
来源：http://qmb.chenlongwang.top

setmetatable({}, { __index = base })
来源：http://crq.yfazqb.com


<!-- 参考信息 -->