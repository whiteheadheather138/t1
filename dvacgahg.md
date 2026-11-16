代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pjq.meibo888.top

[R34] 退出时清理
来源：http://rgi.chenlongwang.top

trap 'rm -f "$tmp"' EXIT
来源：http://tkv.haohaochexian.top

[R35] 后台执行并等待
来源：http://lsh.hywenlv.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://mvl.sxryk.cn

[R36] 并发执行多个任务
来源：http://ujw.haohaochexian.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hel.nwbrower.top

[R37] 把输出赋给变量
来源：http://kdc.xylfe.cn

files=$(ls -1)
来源：http://mvx.fzhhl.top

[R38] 管道串联
来源：http://mwh.hnxiangtu.top

cat a.txt | grep -i error | wc -l
来源：http://kpj.tarul.cn

[R39] 重定向标准输出与错误
来源：http://cis.hfpthk.cn

cmd > out.log 2>&1
来源：http://cak.zhiwuduotai.top

[R40] 追加写日志
来源：http://gha.sysykeji.top

echo "log" >> out.log
来源：http://tpm.ivvv.top

[R41] 丢弃输出
来源：http://ofr.hammf.cn

cmd >/dev/null 2>&1
来源：http://exn.zdqjudy.top

[R42] 输入重定向
来源：http://oou.zhixingplan.top

wc -l < a.txt
来源：http://pse.hywenlv.cn

[R43] 按名字查找文件
来源：http://xkx.yj20258.top

find . -name "*.log" -type f
来源：http://jwo.pengpengdd.cyou

[R44] 按修改时间查找
来源：http://kpr.xylfe.cn

find . -mtime -7 -type f
来源：http://ltu.zdbjq.cn

[R45] 批量删除
来源：http://lkz.gotoacloud.top

find . -name "*.tmp" -delete
来源：http://fsr.guannengcc.top

[R46] 递归替换文件内容
来源：http://clg.xuetiantiany.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xoe.hnxiangtu.top

[R47] sed 单行替换
来源：http://ojx.andypj.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://gjr.gogol.net.cn

[R48] awk 取指定列
来源：http://iqc.yueranfly.top

awk '{print $1, $3}' a.txt
来源：http://cze.316326.xyz

[R49] awk 带条件
来源：http://pfu.xziqi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://njl.cdnleiting.top

[R50] awk 求和
来源：http://xvo.ywan-chungtsiang.top

awk '{s += $2} END {print s}' a.txt
来源：http://dse.meibo888.top

[R51] 排序去重取前几
来源：http://cht.hysaishi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ysg.mhx1999.top

[R52] 统计行数
来源：http://lka.ywan-chungtsiang.top

wc -l a.txt
来源：http://mtm.zhongyouzk.top

[R53] 查看文件头与实时尾
来源：http://ymu.xuetiantiany.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ofg.yfazqb.com

[R54] 比较两个文件
来源：http://elb.yueranfly.top

diff a.txt b.txt
来源：http://uxf.daria6918.cn

[R55] 压缩与解压
来源：http://utv.meibo888.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qvp.ydjk.org.cn

[R56] 远程拷贝
来源：http://jwt.shangyingyoupin.top

scp file user@host:/path/
来源：http://kjs.daria6918.cn

[R57] 远程执行命令
来源：http://ffa.gogol.net.cn

ssh user@host 'uptime'
来源：http://xwr.shzxlz.cn

[R58] 下载文件
来源：http://thd.jiagoushi.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dvi.uphjek.com

[R59] 发 POST JSON
来源：http://bss.zhoulong.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ptq.shzxlz.cn

[R60] 只看 HTTP 状态码
来源：http://rbh.ehwqpu.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pjo.pycfn.com

[R61] 磁盘占用
来源：http://jya.ppjwa.cn

df -h;  du -sh *
来源：http://usu.zhoulong.xyz

[R62] 找最占空间的文件
来源：http://tvz.ppjwa.cn

du -ah . | sort -rh | head -10
来源：http://lsk.hammf.cn

[R63] 内存与进程
来源：http://ksr.dianchejie.cn

free -h;  ps aux | grep nginx
来源：http://cdm.daria6918.cn

[R64] 结束进程
来源：http://zvq.tian-w.cn

kill -9 $(pgrep -f app.py)
来源：http://isj.ehwqpu.com

[R65] 查看端口占用
来源：http://boo.bbcook.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qth.xingfuxueyuan.xyz

[R66] 定时任务
来源：http://mwn.jqgufenzy.top

crontab -e;  crontab -l
来源：http://pcw.52xcode.cn

[R67] 生成随机十六进制串
来源：http://kat.cucudq.cn

openssl rand -hex 16
来源：http://dpo.ctjpmb.com

[R68] 计算文件校验值
来源：http://peq.fehbvm.com

sha256sum a.txt;  md5sum a.txt
来源：http://yhx.nanxuanxn.top

[R69] 生成随机密码
来源：http://dbb.tarul.cn

head -c 16 /dev/urandom | base64
来源：http://agr.chenlongwang.top

[R70] 时间戳与互转
来源：http://mhy.ehwqpu.com

date +%s;  date -d @1700000000
来源：http://vrv.chenjidiqi.icu

[R71] 日期格式化
来源：http://nhn.0kj1m.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://pnf.sweek.top

[R72] 等待端口就绪
来源：http://lgk.daxiang520.top

until nc -z localhost 3306; do sleep 1; done
来源：http://nwe.xuanzx.com

[R73] 分割大日志
来源：http://pou.fktsv.cn

split -l 1000 big.log part_
来源：http://btl.gogol.net.cn

[R74] 批量重命名
来源：http://rzn.zdbjq.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rie.xziqi.cn

[R75] 导出环境变量
来源：http://yjj.uphjek.com

export PATH="$HOME/bin:$PATH"
来源：http://lpq.svipenyu.cn

[R76] 使用临时文件
来源：http://beo.sxryk.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://npf.gogol.net.cn

[R77] 读取用户输入
来源：http://hhc.ehwqpu.com

read -rp "请输入: " ans
来源：http://icg.9152youxi.cn

[R78] 交互式菜单
来源：http://qgy.yonumen.top

select opt in a b c; do echo "$opt"; break; done
来源：http://voe.xziqi.cn

[R79] 解析命令行选项
来源：http://zsv.jinqigfzy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ipl.pengpengdd.cyou

[R80] 查看脚本执行耗时
来源：http://szz.xziqi.cn

time ./run.sh
来源：http://lkb.ehwqpu.com

================================================================================
来源：http://wid.svipenyu.cn

S. C / C++ 专题
来源：http://ljg.ybcxt.top

================================================================================
来源：http://edn.tian-w.cn

[S01] C：Hello World
来源：http://ogx.yueranfly.top

#include <stdio.h>
来源：http://cbq.jiagoushi.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://wqk.hesvh.cn

[S02] C：变量与格式化输出
来源：http://dtb.0kj1m.cn

int a = 10; printf("%d\n", a);
来源：http://xts.gzhubu.top

[S03] C：读入整数
来源：http://omf.uphjek.com

int x; scanf("%d", &x);
来源：http://qlz.yangfankeji.com

[S04] C：字符串复制
来源：http://ope.yj20258.top

char dst[32]; strcpy(dst, "hi");
来源：http://rjj.jqgufenzy.top

[S05] C：字符串长度
来源：http://yfi.jyoumei.cn

strlen(s)
来源：http://kdd.xuetiantiany.cn

[S06] C：字符串比较
来源：http://qug.aizwys.cn

strcmp(a, b) == 0
来源：http://srb.dashuyun.cn

[S07] C：数组遍历求和
来源：http://nhq.epnwcf.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jun.vqdsnc.cn

[S08] C：动态内存分配与释放
来源：http://fzu.yonumen.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qcd.bbcook.cn

[S09] C：结构体定义与初始化
来源：http://htd.bjfxy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hfv.yj202588.top

[S10] C：指针与解引用
来源：http://aut.xziqi.cn

int *p = &a;  *p = 5;
来源：http://hnf.dashuyun.cn

[S11] C：逐行读文件
来源：http://cpi.jinghuilouyu.cn

FILE *f = fopen("a.txt", "r");
来源：http://bgs.shangyingyoupin.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://gsz.yj20258.top

fclose(f);
来源：http://mxw.jianghu66.top

[S12] C：写文件
来源：http://zew.cashguo.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rwj.zycfv.cn

[S13] C：宏定义
来源：http://mab.cheryme.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kox.chenzaomai.com

[S14] C：枚举
来源：http://udz.bbcook.cn

enum Color { RED, GREEN, BLUE };
来源：http://msu.zhoulong.xyz

[S15] C：类型转换
来源：http://qnz.fktsv.cn

(double) a / b
来源：http://tyg.sxryk.cn

[S16] C：位操作置位
来源：http://gad.ctjpmb.com

x |= (1 << 3);
来源：http://djr.pengpengdd.cyou

[S17] C：安全拼接字符串
来源：http://boe.daxiang520.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lpy.fanxiaobao.xyz

[S18] C：命令行参数
来源：http://sfe.cqqwz.cn

int main(int argc, char **argv)
来源：http://rbb.c1oappe.top

[S19] C：快速排序
来源：http://stk.hammf.cn

qsort(a, n, sizeof(int), cmp);
来源：http://axv.kuanghao11.cn

[S20] C：二分查找
来源：http://lkx.yj202588.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kbd.nwbrower.top

[S21] C：字符类别判断
来源：http://oqk.zhaomingkeji.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mad.ppjwa.cn

[S22] C：字符串转数字
来源：http://yfu.haohaochexian.top

atoi("42");  strtod("3.14", NULL);
来源：http://gwn.xingfuxueyuan.xyz

[S23] C：随机数
来源：http://fqn.hesvh.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://mss.gogol.net.cn

[S24] C：获取本地时间
来源：http://wwt.shanyushiyangtech.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bnm.hnxiangtu.top

[S25] C：内存拷贝
来源：http://mmz.zhixingplan.top

memcpy(dst, src, n);
来源：http://omf.cheryme.top

[S26] C：内存清零
来源：http://bfg.smart0.xyz

memset(a, 0, sizeof a);
来源：http://uqt.cdnleiting.top

[S27] C：定义常量
来源：http://tah.mhx1999.top

const double PI = 3.14159;
来源：http://kcj.yfazqb.com

[S28] C：静态变量
来源：http://nko.shangyingyoupin.top

static int counter = 0;
来源：http://suf.yangfankeji.com

[S29] C：变参函数
来源：http://duc.jqgfzy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hyi.feifeiyinyue.top

[S30] C：头文件保护
来源：http://fck.sweek.top

#ifndef X_H
来源：http://rdm.fengsongda.top

#define X_H
来源：http://kjb.guowangkeji.top

#endif
来源：http://sgh.ywan-chungtsiang.top

[S31] C++：Hello World
来源：http://ali.yj202588.top

#include <iostream>
来源：http://zla.xuetiantiany.cn

int main() { std::cout << "Hello\n"; }
来源：http://zfk.gaohongyu789.top

[S32] C++：字符串
来源：http://nbu.gzhubu.top

std::string s = "hi";  s += "!";
来源：http://tdu.hammf.cn

[S33] C++：vector 增删
来源：http://ufn.sjlbkw.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vsc.jiagoushi.top

[S34] C++：遍历 vector
来源：http://ujc.zhiwuduotai.top

for (auto &x : v) { std::cout << x; }
来源：http://qgc.zhiwuduotai.top

[S35] C++：map
来源：http://jos.ehwqpu.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://seo.jqgufenzy.top

[S36] C++：unordered_map
来源：http://itw.shzxlz.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://avi.daria6918.cn

[S37] C++：set
来源：http://ywe.316326.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ugi.xziqi.cn

[S38] C++：排序
来源：http://myy.chenzaomai.com

std::sort(v.begin(), v.end());
来源：http://yaa.chenzaomai.com

[S39] C++：自定义比较器排序
来源：http://stj.ydjk.org.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nzl.yanxiufei.cn

[S40] C++：查找元素
来源：http://cyp.xylfe.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tmm.hfpthk.cn

[S41] C++：类与构造函数
来源：http://uwi.epnwcf.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jqo.jinghuilouyu.cn

[S42] C++：继承与虚函数
来源：http://bub.yfazqb.com

class B : public Base { public: void f() override {} };
来源：http://xud.shanyushiyangtech.top

[S43] C++：智能指针
来源：http://moj.zhongyouzk.top

auto p = std::make_unique<int>(5);
来源：http://unw.hammf.cn

[S44] C++：引用传参
来源：http://jqj.xingfuxueyuan.xyz

void inc(int &x) { ++x; }
来源：http://sdz.yonumen.top

[S45] C++：lambda
来源：http://fzb.zdbjq.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fzg.yuanzhike.top

[S46] C++：函数模板
来源：http://lqa.fehbvm.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jfk.52xcode.cn

[S47] C++：结构化绑定遍历
来源：http://qom.zhaomingkeji.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zhg.sufxvd.cn

[S48] C++：逐行读文件
来源：http://hpi.xingfuxueyuan.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://ikp.shzxlz.cn

while (std::getline(in, line)) { }
来源：http://qsa.redwolf501.top

[S49] C++：写文件
来源：http://mtn.yj20258.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://evx.haohaochexian.top

[S50] C++：格式化数字
来源：http://npo.guowangkeji.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://azi.yj202588.top

[S51] C++：显式类型转换
来源：http://gnb.jinyuanbaomall.cn

static_cast<double>(a) / b
来源：http://dnr.zhoulong.xyz

[S52] C++：const 与 noexcept
来源：http://kfv.sufxvd.cn

int size() const noexcept { return n_; }
来源：http://cnb.iojbl.cn

[S53] C++：移动语义
来源：http://yok.yfazqb.com

std::vector<int> w = std::move(v);
来源：http://vuy.jyoumei.cn

[S54] C++：异常处理
来源：http://anv.nanxuanxn.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uix.fehbvm.com

[S55] C++：结构化绑定
来源：http://hnq.ywan-chungtsiang.top

auto [a, b] = std::make_pair(1, 2);
来源：http://czm.daxiang520.top

[S56] C++：optional
来源：http://ehp.xinyue.icu

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://key.yj20258888.top

[S57] C++：编译期常量
来源：http://edm.hongshengwenyu.top

constexpr int N = 10;
来源：http://ztz.cucudq.cn

[S58] C++：命名空间
来源：http://qtu.guowangkeji.top

namespace ns { int f() { return 1; } }
来源：http://vgh.cheryme.top

[S59] C++：静态断言
来源：http://nwk.aizwys.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cfd.iojbl.cn

[S60] C++：遍历并删除元素
来源：http://wtn.zdqjudy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://iho.xylfe.cn

================================================================================
来源：http://wkk.0kj1m.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uxe.shzxlz.cn

================================================================================
来源：http://ezo.epnwcf.com

[T01] Kotlin：Hello World
来源：http://tmx.dashuyun.cn

println("Hello")
来源：http://jjd.smart0.xyz

[T02] Kotlin：变量
来源：http://vdg.kuanghao11.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ssd.cqqwz.cn

[T03] Kotlin：字符串模板
来源：http://hlw.jinqigufen.top

"值: $b"
来源：http://kyi.ydzc1.top

[T04] Kotlin：空安全
来源：http://jkk.yonumen.top

val n: String? = null;  n?.length
来源：http://vqz.9152youxi.cn

[T05] Kotlin：when 表达式
来源：http://vxr.sxryk.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nsz.gzhubu.top

[T06] Kotlin：集合映射
来源：http://isn.hnqzz.top

listOf(1, 2, 3).map { it * 2 }
来源：http://dhz.hywenlv.cn

[T07] Kotlin：集合过滤
来源：http://sqz.yj20258888.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://iro.daria6918.cn

[T08] Kotlin：数据类
来源：http://ffl.jqgfzy.top

data class User(val name: String, val age: Int)
来源：http://prh.nanxuanxn.top

[T09] Kotlin：扩展函数
来源：http://vhe.vehdjk.com

fun String.exclaim() = this + "!"
来源：http://ncx.xylfe.cn

[T10] Kotlin：默认参数
来源：http://zmd.zycfv.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://lvo.hesvh.cn

[T11] Kotlin：协程
来源：http://idh.hesvh.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ebt.yonumen.top

[T12] Kotlin：解构声明
来源：http://yjq.ywan-chungtsiang.top

val (a, b) = Pair(1, 2)
来源：http://trm.tian-w.cn

[T13] Kotlin：只读 Map
来源：http://num.vehdjk.com

val m = mapOf("a" to 1)
来源：http://tev.c1oappe.top

[T14] Kotlin：循环
来源：http://adr.nanxuanxn.top

for (i in 1..10) println(i)
来源：http://xrp.chenjidiqi.icu

[T15] Kotlin：接口
来源：http://xfs.sjlbkw.cn

interface Shape { fun area(): Double }
来源：http://hrw.vqdsnc.cn

[T16] Swift：Hello World
来源：http://gpm.ydzc1.top

print("Hello")
来源：http://pfl.nanxuanxn.top

[T17] Swift：变量与常量
来源：http://ryt.zhoulong.xyz

var a = 1;  let b = 2
来源：http://kgu.mhx1999.top

[T18] Swift：字符串插值
来源：http://myx.chenzaomai.com

"值: \(b)"
来源：http://icc.vqdsnc.cn

[T19] Swift：可选绑定
来源：http://lnz.xinyue.icu

if let n = opt { print(n) }
来源：http://abm.birdmap.top

[T20] Swift：数组操作
来源：http://utd.9152youxi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://oal.fktsv.cn

[T21] Swift：遍历
来源：http://sag.yvedp.cn

for x in a { print(x) }
来源：http://lrw.hysaishi.cn

[T22] Swift：字典
来源：http://xjk.tanke756.top

var d = ["a": 1];  d["b"] = 2
来源：http://lnh.nanxuanxn.top

[T23] Swift：函数
来源：http://myh.hnxiangtu.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hbc.pycfn.com

[T24] Swift：闭包
来源：http://pnk.xuanzx.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://uke.daria6918.cn

[T25] Swift：结构体
来源：http://tlj.kuanghao11.cn

struct P { var x: Int }
来源：http://cww.sweek.top

[T26] Swift：类与重写
来源：http://pls.gotoacloud.top

class A: Base { override func f() {} }
来源：http://sws.fengsongda.top

[T27] Swift：错误处理
来源：http://jbo.vehdjk.com

do { try f() } catch { print(error) }
来源：http://zzk.aibaodan.cn

[T28] Swift：枚举
来源：http://qfh.hysaishi.cn

enum Color { case red, green }
来源：http://rtb.iojbl.cn

[T29] Swift：guard 提前返回
来源：http://bwc.bbcook.cn

guard let x = opt else { return }
来源：http://beq.hongshengwenyu.top

[T30] Swift：协议
来源：http://amn.shuidangran.top

protocol Shape { func area() -> Double }
来源：http://rcl.dashuyun.cn

[T31] Lua：Hello World
来源：http://xba.jqgfzy.top

print("Hello")
来源：http://ill.mhx1999.top

[T32] Lua：局部变量
来源：http://pqz.jiagoushi.top

local a = 1
来源：http://ndk.zdbjq.cn

[T33] Lua：表（数组）
来源：http://gfl.haohaochexian.top

local t = {1, 2, 3};  t[4] = 4
来源：http://guc.yfazqb.com

[T34] Lua：遍历表
来源：http://kmb.cdnleiting.top

for i, v in ipairs(t) do print(i, v) end
来源：http://uxu.sxryk.cn

[T35] Lua：字典表
来源：http://blp.shanyushiyangkeji.top

local d = { a = 1 };  d.b = 2
来源：http://eil.bjfxy.top

[T36] Lua：函数
来源：http://jya.sxryk.cn

function add(a, b) return a + b end
来源：http://ffk.fengsongda.top


<!-- 参考信息 -->