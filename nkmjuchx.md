代发 wailian999

cmd > out.log 2>&1
来源：http://zhq.aizwys.cn

[R40] 追加写日志
来源：http://wub.jiagoushi.top

echo "log" >> out.log
来源：http://csu.redwolf501.top

[R41] 丢弃输出
来源：http://pya.guannengcc.top

cmd >/dev/null 2>&1
来源：http://fgq.cheryme.top

[R42] 输入重定向
来源：http://wsr.ctjpmb.com

wc -l < a.txt
来源：http://zkk.aizwys.cn

[R43] 按名字查找文件
来源：http://rxr.zhengqikj.top

find . -name "*.log" -type f
来源：http://tlf.guowangkeji.top

[R44] 按修改时间查找
来源：http://mvq.cdnleiting.top

find . -mtime -7 -type f
来源：http://iap.shangyingyoupin.top

[R45] 批量删除
来源：http://xgc.jinqigufen.top

find . -name "*.tmp" -delete
来源：http://rqy.quarkkingdee.top

[R46] 递归替换文件内容
来源：http://fif.pycfn.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jor.52xcode.cn

[R47] sed 单行替换
来源：http://qbw.ppjwa.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dqm.sxryk.cn

[R48] awk 取指定列
来源：http://bbw.svipenyu.cn

awk '{print $1, $3}' a.txt
来源：http://kus.0kj1m.cn

[R49] awk 带条件
来源：http://epn.hfpthk.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vzs.epnwcf.com

[R50] awk 求和
来源：http://ebc.pengpengdd.cyou

awk '{s += $2} END {print s}' a.txt
来源：http://eoz.feifeiyinyue.top

[R51] 排序去重取前几
来源：http://kot.hfpthk.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://esa.guannengcc.top

[R52] 统计行数
来源：http://xci.jqgfzy.top

wc -l a.txt
来源：http://nqj.smart0.xyz

[R53] 查看文件头与实时尾
来源：http://vbv.sufxvd.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://oit.jqgufenzy.top

[R54] 比较两个文件
来源：http://okc.chenjidiqi.icu

diff a.txt b.txt
来源：http://hdp.ydzc1.top

[R55] 压缩与解压
来源：http://vmg.sweek.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qez.zdqjudy.top

[R56] 远程拷贝
来源：http://tuv.yangfankeji.com

scp file user@host:/path/
来源：http://wai.ehwqpu.com

[R57] 远程执行命令
来源：http://qbh.cqqwz.cn

ssh user@host 'uptime'
来源：http://iyw.nwbrower.top

[R58] 下载文件
来源：http://vch.cashguo.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hfw.chenlongwang.top

[R59] 发 POST JSON
来源：http://iil.yj202588.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://swl.hnxiangtu.top

[R60] 只看 HTTP 状态码
来源：http://pqn.jinqigfzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mnx.jinqigufen.top

[R61] 磁盘占用
来源：http://ver.zycfv.cn

df -h;  du -sh *
来源：http://fds.quarkkingdee.top

[R62] 找最占空间的文件
来源：http://zpq.cdnleiting.top

du -ah . | sort -rh | head -10
来源：http://ayc.yongpay.top

[R63] 内存与进程
来源：http://xrf.52xcode.cn

free -h;  ps aux | grep nginx
来源：http://atu.ctjpmb.com

[R64] 结束进程
来源：http://bve.snrcjt.cn

kill -9 $(pgrep -f app.py)
来源：http://cvp.chenzaomai.com

[R65] 查看端口占用
来源：http://ptv.fanxiaobao.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nbl.yvedp.cn

[R66] 定时任务
来源：http://bmz.hammf.cn

crontab -e;  crontab -l
来源：http://vyi.snrcjt.cn

[R67] 生成随机十六进制串
来源：http://mgm.0kj1m.cn

openssl rand -hex 16
来源：http://mbg.xziqi.cn

[R68] 计算文件校验值
来源：http://rjv.cdnleiting.top

sha256sum a.txt;  md5sum a.txt
来源：http://jat.sjlbkw.cn

[R69] 生成随机密码
来源：http://xyj.zdqjudy.top

head -c 16 /dev/urandom | base64
来源：http://llc.daxiang520.top

[R70] 时间戳与互转
来源：http://ogw.yj20258.top

date +%s;  date -d @1700000000
来源：http://lfg.yvedp.cn

[R71] 日期格式化
来源：http://brx.andypj.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://hpk.zhoulong.xyz

[R72] 等待端口就绪
来源：http://gdf.ctjpmb.com

until nc -z localhost 3306; do sleep 1; done
来源：http://kdv.vqdsnc.cn

[R73] 分割大日志
来源：http://vza.cucudq.cn

split -l 1000 big.log part_
来源：http://qzo.chenlongwang.top

[R74] 批量重命名
来源：http://wva.yuxming.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qag.andypj.xyz

[R75] 导出环境变量
来源：http://kvv.jinqigfzy.top

export PATH="$HOME/bin:$PATH"
来源：http://mtv.gzhubu.top

[R76] 使用临时文件
来源：http://xnf.jqgfzy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://uzi.sufxvd.cn

[R77] 读取用户输入
来源：http://mct.jinghuilouyu.cn

read -rp "请输入: " ans
来源：http://nwu.aizwys.cn

[R78] 交互式菜单
来源：http://pqm.yj20258.top

select opt in a b c; do echo "$opt"; break; done
来源：http://cgx.iojbl.cn

[R79] 解析命令行选项
来源：http://sit.fengsongda.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://whn.vehdjk.com

[R80] 查看脚本执行耗时
来源：http://ayy.bjfxy.top

time ./run.sh
来源：http://gfr.ywan-chungtsiang.top

================================================================================
来源：http://iny.ywan-chungtsiang.top

S. C / C++ 专题
来源：http://bqg.havefunace.top

================================================================================
来源：http://zkg.jianghu66.top

[S01] C：Hello World
来源：http://hjl.gzhubu.top

#include <stdio.h>
来源：http://gup.cashguo.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://hux.c1oappe.top

[S02] C：变量与格式化输出
来源：http://sbh.daria6918.cn

int a = 10; printf("%d\n", a);
来源：http://okb.tian-w.cn

[S03] C：读入整数
来源：http://ncq.aizwys.cn

int x; scanf("%d", &x);
来源：http://vzo.jinyuanbaomall.cn

[S04] C：字符串复制
来源：http://vyg.cdnleiting.top

char dst[32]; strcpy(dst, "hi");
来源：http://vdi.jlsjyb.cn

[S05] C：字符串长度
来源：http://qwk.cdnleiting.top

strlen(s)
来源：http://cqq.c1oappe.top

[S06] C：字符串比较
来源：http://gtj.gaohongyu789.top

strcmp(a, b) == 0
来源：http://hrs.9152youxi.cn

[S07] C：数组遍历求和
来源：http://wuq.zhengqikj.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xxe.vqdsnc.cn

[S08] C：动态内存分配与释放
来源：http://cxg.xylfe.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dyk.aizwys.cn

[S09] C：结构体定义与初始化
来源：http://pas.hnxiangtu.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://axc.shuidangran.top

[S10] C：指针与解引用
来源：http://fhz.yuxming.cn

int *p = &a;  *p = 5;
来源：http://bni.ivvv.top

[S11] C：逐行读文件
来源：http://hjv.epnwcf.com

FILE *f = fopen("a.txt", "r");
来源：http://ckw.fzhhl.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://hrc.zhaomingkeji.xyz

fclose(f);
来源：http://hvo.bbcook.cn

[S12] C：写文件
来源：http://isl.jlsjyb.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uoc.jinyuanbaomall.cn

[S13] C：宏定义
来源：http://fnp.bbcook.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wky.zhiwuduotai.top

[S14] C：枚举
来源：http://qqn.9152youxi.cn

enum Color { RED, GREEN, BLUE };
来源：http://yzp.sxryk.cn

[S15] C：类型转换
来源：http://idd.hongshengwenyu.top

(double) a / b
来源：http://rkj.tarul.cn

[S16] C：位操作置位
来源：http://gej.birdmap.top

x |= (1 << 3);
来源：http://sar.wangdashe.top

[S17] C：安全拼接字符串
来源：http://wjx.sjlbkw.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gjr.ydzc1.top

[S18] C：命令行参数
来源：http://zov.zhengqikj.top

int main(int argc, char **argv)
来源：http://mix.zhengqikj.top

[S19] C：快速排序
来源：http://lsm.iojbl.cn

qsort(a, n, sizeof(int), cmp);
来源：http://obe.hysaishi.cn

[S20] C：二分查找
来源：http://nrj.birdmap.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nha.fktsv.cn

[S21] C：字符类别判断
来源：http://thg.fanxiaobao.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hdw.zhongyouzk.top

[S22] C：字符串转数字
来源：http://edm.gaohongyu789.top

atoi("42");  strtod("3.14", NULL);
来源：http://fxs.ydzc1.top

[S23] C：随机数
来源：http://iqz.zhijiandao.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kgm.yanxiufei.cn

[S24] C：获取本地时间
来源：http://yfr.pycfn.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vzk.bjfxy.top

[S25] C：内存拷贝
来源：http://wbn.9152youxi.cn

memcpy(dst, src, n);
来源：http://auf.yongpay.top

[S26] C：内存清零
来源：http://nrb.bbcook.cn

memset(a, 0, sizeof a);
来源：http://yjp.ydzc1.top

[S27] C：定义常量
来源：http://vdc.hywenlv.cn

const double PI = 3.14159;
来源：http://hrh.epnwcf.com

[S28] C：静态变量
来源：http://pzv.yonumen.top

static int counter = 0;
来源：http://yxb.sysykeji.top

[S29] C：变参函数
来源：http://svm.epnwcf.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://etd.nanxinkj.top

[S30] C：头文件保护
来源：http://pwq.jinghuilouyu.cn

#ifndef X_H
来源：http://pwl.jinqigufen.top

#define X_H
来源：http://aub.bbcook.cn

#endif
来源：http://fti.cashguo.top

[S31] C++：Hello World
来源：http://tax.yangfankeji.com

#include <iostream>
来源：http://ppo.zhiwuduotai.top

int main() { std::cout << "Hello\n"; }
来源：http://stc.sysykeji.top

[S32] C++：字符串
来源：http://dei.yuxming.cn

std::string s = "hi";  s += "!";
来源：http://wnj.yuanzhike.top

[S33] C++：vector 增删
来源：http://bqa.zdqjudy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gjl.zycfv.cn

[S34] C++：遍历 vector
来源：http://fwa.bjfxy.top

for (auto &x : v) { std::cout << x; }
来源：http://css.tianlin.xyz

[S35] C++：map
来源：http://zrz.hysaishi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://eev.bbcook.cn

[S36] C++：unordered_map
来源：http://qea.nanxuanxn.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ire.xylfe.cn

[S37] C++：set
来源：http://alo.ppjwa.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://eje.uphjek.com

[S38] C++：排序
来源：http://drl.hysaishi.cn

std::sort(v.begin(), v.end());
来源：http://jgm.havefunace.top

[S39] C++：自定义比较器排序
来源：http://rrz.fengsongda.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nek.fehbvm.com

[S40] C++：查找元素
来源：http://ekj.yfazqb.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tch.zycfv.cn

[S41] C++：类与构造函数
来源：http://oev.havefunace.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://egl.wangdashe.top

[S42] C++：继承与虚函数
来源：http://uet.jqgfzy.top

class B : public Base { public: void f() override {} };
来源：http://kgf.cucudq.cn

[S43] C++：智能指针
来源：http://tix.zhiwuduotai.top

auto p = std::make_unique<int>(5);
来源：http://eke.guannengcc.top

[S44] C++：引用传参
来源：http://qji.sxryk.cn

void inc(int &x) { ++x; }
来源：http://avo.hongshengwenyu.top

[S45] C++：lambda
来源：http://zxe.andypj.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://hsa.hesvh.cn

[S46] C++：函数模板
来源：http://hpe.nwbrower.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jht.zhongyouzk.top

[S47] C++：结构化绑定遍历
来源：http://fca.shuidangran.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zut.zhoulong.xyz

[S48] C++：逐行读文件
来源：http://upi.mhx1999.top

std::ifstream in("a.txt");  std::string line;
来源：http://qkv.cucudq.cn

while (std::getline(in, line)) { }
来源：http://yeo.52xcode.cn

[S49] C++：写文件
来源：http://fuj.sxryk.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://twu.yongpay.top

[S50] C++：格式化数字
来源：http://bpc.dashuyun.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bqi.guowangkeji.top

[S51] C++：显式类型转换
来源：http://bkh.zdqjudy.top

static_cast<double>(a) / b
来源：http://ypw.yonumen.top

[S52] C++：const 与 noexcept
来源：http://pum.ywan-chungtsiang.top

int size() const noexcept { return n_; }
来源：http://kyk.kuanghao11.cn

[S53] C++：移动语义
来源：http://zii.gaohongyu789.top

std::vector<int> w = std::move(v);
来源：http://ajh.jqgufenzy.top

[S54] C++：异常处理
来源：http://gga.xuetiantiany.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tjs.ctjpmb.com

[S55] C++：结构化绑定
来源：http://rnn.shzxlz.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wan.hfpthk.cn

[S56] C++：optional
来源：http://fqa.zhongyouzk.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://aut.bjfxy.top

[S57] C++：编译期常量
来源：http://uel.vqdsnc.cn

constexpr int N = 10;
来源：http://ogg.jyoumei.cn

[S58] C++：命名空间
来源：http://njh.shanyushiyangkeji.top

namespace ns { int f() { return 1; } }
来源：http://kha.gaohongyu789.top

[S59] C++：静态断言
来源：http://vmu.havefunace.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tgs.gzhubu.top

[S60] C++：遍历并删除元素
来源：http://tuq.shzxlz.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tna.birdmap.top

================================================================================
来源：http://swv.hnxiangtu.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hqq.sxryk.cn

================================================================================
来源：http://qxu.zhiwuduotai.top

[T01] Kotlin：Hello World
来源：http://usl.jiagoushi.top

println("Hello")
来源：http://csp.jinqigufen.top

[T02] Kotlin：变量
来源：http://fjb.shzxlz.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://izn.0kj1m.cn

[T03] Kotlin：字符串模板
来源：http://yor.xuanzx.com

"值: $b"
来源：http://kgc.hysaishi.cn

[T04] Kotlin：空安全
来源：http://jao.svipenyu.cn

val n: String? = null;  n?.length
来源：http://vwp.epnwcf.com

[T05] Kotlin：when 表达式
来源：http://fes.daxiang520.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nve.tianlin.xyz

[T06] Kotlin：集合映射
来源：http://qrj.nanxuanxn.top

listOf(1, 2, 3).map { it * 2 }
来源：http://uqy.ehwqpu.com

[T07] Kotlin：集合过滤
来源：http://fmy.haohaochexian.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://yhj.xuetiantiany.cn

[T08] Kotlin：数据类
来源：http://zvd.yongpay.top

data class User(val name: String, val age: Int)
来源：http://stg.ppjwa.cn

[T09] Kotlin：扩展函数
来源：http://esw.yanxiufei.cn

fun String.exclaim() = this + "!"
来源：http://jix.sjlbkw.cn

[T10] Kotlin：默认参数
来源：http://haf.zhiwuduotai.top

fun greet(name: String = "World") = "Hi $name"
来源：http://auf.jqgufenzy.top

[T11] Kotlin：协程
来源：http://rxh.sufxvd.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xsw.xingfuxueyuan.xyz

[T12] Kotlin：解构声明
来源：http://wkc.birdmap.top

val (a, b) = Pair(1, 2)
来源：http://yjc.birdmap.top

[T13] Kotlin：只读 Map
来源：http://sxz.hysaishi.cn

val m = mapOf("a" to 1)
来源：http://gtq.yongpay.top

[T14] Kotlin：循环
来源：http://ghg.svipenyu.cn

for (i in 1..10) println(i)
来源：http://dmo.nanxuanxn.top

[T15] Kotlin：接口
来源：http://jca.sjlbkw.cn

interface Shape { fun area(): Double }
来源：http://kbf.ehwqpu.com

[T16] Swift：Hello World
来源：http://dlk.gaohongyu789.top

print("Hello")
来源：http://dwt.0kj1m.cn

[T17] Swift：变量与常量
来源：http://lzc.havefunace.top

var a = 1;  let b = 2
来源：http://mdo.ywan-chungtsiang.top

[T18] Swift：字符串插值
来源：http://slk.yanxiufei.cn

"值: \(b)"
来源：http://tgl.bbcook.cn

[T19] Swift：可选绑定
来源：http://xew.feifeiyinyue.top

if let n = opt { print(n) }
来源：http://oxr.cqqwz.cn

[T20] Swift：数组操作
来源：http://qsr.zhijiandao.cn

var a = [1, 2, 3];  a.append(4)
来源：http://iks.jqgfzy.top

[T21] Swift：遍历
来源：http://xux.svipenyu.cn

for x in a { print(x) }
来源：http://jgc.zhoulong.xyz

[T22] Swift：字典
来源：http://hjf.jinqigufen.top

var d = ["a": 1];  d["b"] = 2
来源：http://aoe.xuanzx.com

[T23] Swift：函数
来源：http://hbs.ctjpmb.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gwp.cdnleiting.top

[T24] Swift：闭包
来源：http://kls.shanyushiyangtech.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ujh.jinyuanbaomall.cn

[T25] Swift：结构体
来源：http://gcm.guowangkeji.top

struct P { var x: Int }
来源：http://pxk.gaohongyu789.top

[T26] Swift：类与重写
来源：http://xtx.xuetiantiany.cn

class A: Base { override func f() {} }
来源：http://esl.fktsv.cn

[T27] Swift：错误处理
来源：http://dpk.ydzc1.top

do { try f() } catch { print(error) }
来源：http://rut.jinyuanbaomall.cn

[T28] Swift：枚举
来源：http://tme.zhiwuduotai.top

enum Color { case red, green }
来源：http://gid.zhongyouzk.top

[T29] Swift：guard 提前返回
来源：http://ypk.jinqigufen.top

guard let x = opt else { return }
来源：http://lbe.quarkkingdee.top

[T30] Swift：协议
来源：http://rrl.fehbvm.com

protocol Shape { func area() -> Double }
来源：http://nzl.jinghuilouyu.cn

[T31] Lua：Hello World
来源：http://pvz.hfpthk.cn

print("Hello")
来源：http://pjr.cucudq.cn

[T32] Lua：局部变量
来源：http://pio.yvedp.cn

local a = 1
来源：http://tdg.yuanzhike.top

[T33] Lua：表（数组）
来源：http://rvk.pycfn.com

local t = {1, 2, 3};  t[4] = 4
来源：http://gkp.yj202588.top

[T34] Lua：遍历表
来源：http://bsl.yj20258888.top

for i, v in ipairs(t) do print(i, v) end
来源：http://mzr.aizwys.cn

[T35] Lua：字典表
来源：http://sdk.havefunace.top

local d = { a = 1 };  d.b = 2
来源：http://lak.wangshuangyany.cn

[T36] Lua：函数
来源：http://tkh.sysykeji.top

function add(a, b) return a + b end
来源：http://fsl.ydjk.org.cn

[T37] Lua：字符串拼接
来源：http://gjt.yj202588.top

"a" .. "b"
来源：http://cyi.wangdashe.top

[T38] Lua：条件
来源：http://jqr.chenzaomai.com

if x > 0 then print("正") end
来源：http://nau.yj20258888.top

[T39] Lua：模式匹配
来源：http://nfn.havefunace.top

string.find(s, "%d+")
来源：http://vkl.ppjwa.cn

[T40] Lua：元表
来源：http://vwn.hcnkem.com

setmetatable({}, { __index = base })
来源：http://qvc.daria6918.cn

[T41] Perl：Hello World
来源：http://inz.ybcxt.top

print "Hello\n";
来源：http://epr.ppjwa.cn

[T42] Perl：变量类型
来源：http://ekh.dianchejie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bhe.vqdsnc.cn


<!-- 参考信息 -->