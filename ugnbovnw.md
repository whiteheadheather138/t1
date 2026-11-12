代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rjh.52xcode.cn

[R34] 退出时清理
来源：http://wgl.fanxiaobao.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://oeo.meibo888.top

[R35] 后台执行并等待
来源：http://qyx.xylfe.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://riy.xziqi.cn

[R36] 并发执行多个任务
来源：http://hrg.chenlongwang.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://urf.daxiang520.top

[R37] 把输出赋给变量
来源：http://ohz.yongpay.top

files=$(ls -1)
来源：http://mdx.hongshengwenyu.top

[R38] 管道串联
来源：http://tji.ehwqpu.com

cat a.txt | grep -i error | wc -l
来源：http://nfx.ydzc1.top

[R39] 重定向标准输出与错误
来源：http://ydp.sysykeji.top

cmd > out.log 2>&1
来源：http://tpd.pycfn.com

[R40] 追加写日志
来源：http://myc.jinyuanbaomall.cn

echo "log" >> out.log
来源：http://zyi.ydjk.org.cn

[R41] 丢弃输出
来源：http://gcf.yj20258888.top

cmd >/dev/null 2>&1
来源：http://mop.52xcode.cn

[R42] 输入重定向
来源：http://qua.ppjwa.cn

wc -l < a.txt
来源：http://sfu.fzhhl.top

[R43] 按名字查找文件
来源：http://dkk.chenlongwang.top

find . -name "*.log" -type f
来源：http://evg.shanyushiyangtech.top

[R44] 按修改时间查找
来源：http://qrw.xuetiantiany.cn

find . -mtime -7 -type f
来源：http://ewo.chenzaomai.com

[R45] 批量删除
来源：http://jtr.birdmap.top

find . -name "*.tmp" -delete
来源：http://vzx.ctjpmb.com

[R46] 递归替换文件内容
来源：http://hic.52xcode.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://snu.wangshuangyany.cn

[R47] sed 单行替换
来源：http://ihr.xziqi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://zrd.iojbl.cn

[R48] awk 取指定列
来源：http://anc.wangshuangyany.cn

awk '{print $1, $3}' a.txt
来源：http://cta.ivvv.top

[R49] awk 带条件
来源：http://wdh.smart0.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://afw.yvedp.cn

[R50] awk 求和
来源：http://urd.tanke756.top

awk '{s += $2} END {print s}' a.txt
来源：http://miu.jqgfzy.top

[R51] 排序去重取前几
来源：http://sqp.guowangkeji.top

sort a.txt | uniq -c | sort -rn | head
来源：http://hfo.fktsv.cn

[R52] 统计行数
来源：http://nre.vehdjk.com

wc -l a.txt
来源：http://hgb.chenjidiqi.icu

[R53] 查看文件头与实时尾
来源：http://fya.smart0.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jvz.jlsjyb.cn

[R54] 比较两个文件
来源：http://buv.cdnleiting.top

diff a.txt b.txt
来源：http://rjn.gaohongyu789.top

[R55] 压缩与解压
来源：http://ebf.redwolf501.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ylp.wangshuangyany.cn

[R56] 远程拷贝
来源：http://frb.xylfe.cn

scp file user@host:/path/
来源：http://mym.cashguo.top

[R57] 远程执行命令
来源：http://ldh.hnxiangtu.top

ssh user@host 'uptime'
来源：http://oqc.gaohongyu789.top

[R58] 下载文件
来源：http://wkm.yfazqb.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zqi.yonumen.top

[R59] 发 POST JSON
来源：http://hdh.epnwcf.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cwk.hysaishi.cn

[R60] 只看 HTTP 状态码
来源：http://hhr.fktsv.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://beo.gogol.net.cn

[R61] 磁盘占用
来源：http://bfk.cucudq.cn

df -h;  du -sh *
来源：http://jln.daria6918.cn

[R62] 找最占空间的文件
来源：http://kqh.ywan-chungtsiang.top

du -ah . | sort -rh | head -10
来源：http://ycf.daria6918.cn

[R63] 内存与进程
来源：http://vey.hysaishi.cn

free -h;  ps aux | grep nginx
来源：http://eck.hnxiangtu.top

[R64] 结束进程
来源：http://kbk.chenlongwang.top

kill -9 $(pgrep -f app.py)
来源：http://uuj.smart0.xyz

[R65] 查看端口占用
来源：http://zyf.bbcook.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vdo.hongshengwenyu.top

[R66] 定时任务
来源：http://xvp.redwolf501.top

crontab -e;  crontab -l
来源：http://wlb.shanyushiyangtech.top

[R67] 生成随机十六进制串
来源：http://lpn.jqgufenzy.top

openssl rand -hex 16
来源：http://vel.hcnkem.com

[R68] 计算文件校验值
来源：http://ljv.redwolf501.top

sha256sum a.txt;  md5sum a.txt
来源：http://kak.birdmap.top

[R69] 生成随机密码
来源：http://gfa.hesvh.cn

head -c 16 /dev/urandom | base64
来源：http://axv.jqgfzy.top

[R70] 时间戳与互转
来源：http://vhm.pengpengdd.cyou

date +%s;  date -d @1700000000
来源：http://kgc.hammf.cn

[R71] 日期格式化
来源：http://zdl.sufxvd.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ebk.zhijiandao.cn

[R72] 等待端口就绪
来源：http://sqh.sxryk.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ysy.gaohongyu789.top

[R73] 分割大日志
来源：http://trh.chenjidiqi.icu

split -l 1000 big.log part_
来源：http://hdr.tanke756.top

[R74] 批量重命名
来源：http://tjp.yongpay.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ovz.shanyushiyangtech.top

[R75] 导出环境变量
来源：http://odw.chenjidiqi.icu

export PATH="$HOME/bin:$PATH"
来源：http://xvk.uphjek.com

[R76] 使用临时文件
来源：http://ooq.gaohongyu789.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://osf.jyoumei.cn

[R77] 读取用户输入
来源：http://znd.uphjek.com

read -rp "请输入: " ans
来源：http://ghw.sxryk.cn

[R78] 交互式菜单
来源：http://eps.pengpengdd.cyou

select opt in a b c; do echo "$opt"; break; done
来源：http://xeh.uphjek.com

[R79] 解析命令行选项
来源：http://kzf.jinqigfzy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yzq.xinyue.icu

[R80] 查看脚本执行耗时
来源：http://erz.gogol.net.cn

time ./run.sh
来源：http://nve.shzxlz.cn

================================================================================
来源：http://lvu.dashuyun.cn

S. C / C++ 专题
来源：http://rzr.tarul.cn

================================================================================
来源：http://vwr.shanyushiyangtech.top

[S01] C：Hello World
来源：http://mum.yueranfly.top

#include <stdio.h>
来源：http://znh.hysaishi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://omr.c1oappe.top

[S02] C：变量与格式化输出
来源：http://zkp.tianlin.xyz

int a = 10; printf("%d\n", a);
来源：http://mwy.ydzc1.top

[S03] C：读入整数
来源：http://vxx.fanxiaobao.xyz

int x; scanf("%d", &x);
来源：http://cvq.fktsv.cn

[S04] C：字符串复制
来源：http://vek.meibo888.top

char dst[32]; strcpy(dst, "hi");
来源：http://eaa.gotoacloud.top

[S05] C：字符串长度
来源：http://uej.gzhubu.top

strlen(s)
来源：http://mol.hfpthk.cn

[S06] C：字符串比较
来源：http://egn.sufxvd.cn

strcmp(a, b) == 0
来源：http://hox.fehbvm.com

[S07] C：数组遍历求和
来源：http://upd.nwbrower.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://glr.yueranfly.top

[S08] C：动态内存分配与释放
来源：http://unw.nwbrower.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tzv.sxryk.cn

[S09] C：结构体定义与初始化
来源：http://kmv.ehwqpu.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qla.wangdashe.top

[S10] C：指针与解引用
来源：http://ysa.yj20258.top

int *p = &a;  *p = 5;
来源：http://wsw.sxryk.cn

[S11] C：逐行读文件
来源：http://ktl.jqgufenzy.top

FILE *f = fopen("a.txt", "r");
来源：http://svi.sxryk.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://iaf.ydzc1.top

fclose(f);
来源：http://iev.shangyingyoupin.top

[S12] C：写文件
来源：http://yuc.ivvv.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qws.zhiwuduotai.top

[S13] C：宏定义
来源：http://fea.ydjk.org.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nlj.yj20258888.top

[S14] C：枚举
来源：http://srx.xziqi.cn

enum Color { RED, GREEN, BLUE };
来源：http://awf.guannengcc.top

[S15] C：类型转换
来源：http://tbz.pengpengdd.cyou

(double) a / b
来源：http://vbd.sweek.top

[S16] C：位操作置位
来源：http://jou.xuanzx.com

x |= (1 << 3);
来源：http://pho.hesvh.cn

[S17] C：安全拼接字符串
来源：http://aos.cdnleiting.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ruj.yonumen.top

[S18] C：命令行参数
来源：http://coo.hnxiangtu.top

int main(int argc, char **argv)
来源：http://ymw.daria6918.cn

[S19] C：快速排序
来源：http://fdo.pycfn.com

qsort(a, n, sizeof(int), cmp);
来源：http://dry.epnwcf.com

[S20] C：二分查找
来源：http://vcl.xziqi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bbg.ehwqpu.com

[S21] C：字符类别判断
来源：http://dfb.yueranfly.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sii.ybcxt.top

[S22] C：字符串转数字
来源：http://njr.hammf.cn

atoi("42");  strtod("3.14", NULL);
来源：http://owr.snrcjt.cn

[S23] C：随机数
来源：http://knf.shangyingyoupin.top

srand(time(NULL));  int r = rand() % 100;
来源：http://wou.ctjpmb.com

[S24] C：获取本地时间
来源：http://ebp.jinqigufen.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pxd.yuanzhike.top

[S25] C：内存拷贝
来源：http://bex.jqgufenzy.top

memcpy(dst, src, n);
来源：http://cxv.zhiwuduotai.top

[S26] C：内存清零
来源：http://vby.sxryk.cn

memset(a, 0, sizeof a);
来源：http://bbz.xuetiantiany.cn

[S27] C：定义常量
来源：http://hxq.yanxiufei.cn

const double PI = 3.14159;
来源：http://vav.tarul.cn

[S28] C：静态变量
来源：http://aoo.jiagoushi.top

static int counter = 0;
来源：http://gao.nanxuanxn.top

[S29] C：变参函数
来源：http://oxt.vehdjk.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jwm.zhijiandao.cn

[S30] C：头文件保护
来源：http://qbc.jinqigfzy.top

#ifndef X_H
来源：http://wrr.316326.xyz

#define X_H
来源：http://nyx.redwolf501.top

#endif
来源：http://pmt.xylfe.cn

[S31] C++：Hello World
来源：http://fnl.svipenyu.cn

#include <iostream>
来源：http://xuk.shuidangran.top

int main() { std::cout << "Hello\n"; }
来源：http://isk.jyoumei.cn

[S32] C++：字符串
来源：http://qgp.pengpengdd.cyou

std::string s = "hi";  s += "!";
来源：http://gpi.shangyingyoupin.top

[S33] C++：vector 增删
来源：http://xst.ydzc1.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yxt.zhoulong.xyz

[S34] C++：遍历 vector
来源：http://zmz.zycfv.cn

for (auto &x : v) { std::cout << x; }
来源：http://okt.yvedp.cn

[S35] C++：map
来源：http://ynx.yj20258.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jnc.chenlongwang.top

[S36] C++：unordered_map
来源：http://sqm.yvedp.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wlg.ivvv.top

[S37] C++：set
来源：http://afo.chenjidiqi.icu

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kem.fktsv.cn

[S38] C++：排序
来源：http://mjn.gzhubu.top

std::sort(v.begin(), v.end());
来源：http://hqy.fzhhl.top

[S39] C++：自定义比较器排序
来源：http://oop.yongpay.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jsl.jinqigfzy.top

[S40] C++：查找元素
来源：http://hqk.tarul.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wub.tarul.cn

[S41] C++：类与构造函数
来源：http://tlu.shuidangran.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://npw.chenlongwang.top

[S42] C++：继承与虚函数
来源：http://dwe.tianlin.xyz

class B : public Base { public: void f() override {} };
来源：http://cks.xylfe.cn

[S43] C++：智能指针
来源：http://axx.tarul.cn

auto p = std::make_unique<int>(5);
来源：http://ccf.tianlin.xyz

[S44] C++：引用传参
来源：http://jgw.gotoacloud.top

void inc(int &x) { ++x; }
来源：http://rcs.dashuyun.cn

[S45] C++：lambda
来源：http://myk.zhoulong.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://bpu.jinyuanbaomall.cn

[S46] C++：函数模板
来源：http://acb.yj20258888.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ggg.jqgfzy.top

[S47] C++：结构化绑定遍历
来源：http://srv.xuanzx.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://agt.andypj.xyz

[S48] C++：逐行读文件
来源：http://pbh.hywenlv.cn

std::ifstream in("a.txt");  std::string line;
来源：http://odp.nanxinkj.top

while (std::getline(in, line)) { }
来源：http://xlm.yuanzhike.top

[S49] C++：写文件
来源：http://ywv.zhongyouzk.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rck.uphjek.com

[S50] C++：格式化数字
来源：http://sbj.havefunace.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://oux.dashuyun.cn

[S51] C++：显式类型转换
来源：http://njj.ivvv.top

static_cast<double>(a) / b
来源：http://vpw.dianchejie.cn

[S52] C++：const 与 noexcept
来源：http://dns.epnwcf.com

int size() const noexcept { return n_; }
来源：http://hwr.guannengcc.top

[S53] C++：移动语义
来源：http://rwn.316326.xyz

std::vector<int> w = std::move(v);
来源：http://ggd.9152youxi.cn

[S54] C++：异常处理
来源：http://owi.havefunace.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zpc.hcnkem.com

[S55] C++：结构化绑定
来源：http://ogp.jinyuanbaomall.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zry.wangshuangyany.cn

[S56] C++：optional
来源：http://yqd.yuanzhike.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xmz.iojbl.cn

[S57] C++：编译期常量
来源：http://nha.ctjpmb.com

constexpr int N = 10;
来源：http://aha.chenlongwang.top

[S58] C++：命名空间
来源：http://asx.shangyingyoupin.top

namespace ns { int f() { return 1; } }
来源：http://hpc.ywan-chungtsiang.top

[S59] C++：静态断言
来源：http://udh.hammf.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://duq.ivvv.top

[S60] C++：遍历并删除元素
来源：http://jdl.nanxuanxn.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kwo.yonumen.top

================================================================================
来源：http://igk.shangyingyoupin.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zul.tianlin.xyz

================================================================================
来源：http://yxs.chenjidiqi.icu

[T01] Kotlin：Hello World
来源：http://tgf.aibaodan.cn

println("Hello")
来源：http://bex.smart0.xyz

[T02] Kotlin：变量
来源：http://hid.fktsv.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://njs.hcnkem.com

[T03] Kotlin：字符串模板
来源：http://tcd.svipenyu.cn

"值: $b"
来源：http://dhv.fengsongda.top

[T04] Kotlin：空安全
来源：http://vsv.haohaochexian.top

val n: String? = null;  n?.length
来源：http://cyz.yongpay.top

[T05] Kotlin：when 表达式
来源：http://pjj.zdqjudy.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://urh.shanyushiyangtech.top

[T06] Kotlin：集合映射
来源：http://opv.epnwcf.com

listOf(1, 2, 3).map { it * 2 }
来源：http://fvg.chenzaomai.com

[T07] Kotlin：集合过滤
来源：http://ihr.jinyuanbaomall.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://gjn.guowangkeji.top

[T08] Kotlin：数据类
来源：http://vtm.hammf.cn

data class User(val name: String, val age: Int)
来源：http://mfa.guowangkeji.top

[T09] Kotlin：扩展函数
来源：http://kqz.hywenlv.cn

fun String.exclaim() = this + "!"
来源：http://heb.aibaodan.cn

[T10] Kotlin：默认参数
来源：http://hqk.hywenlv.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://hxx.fengsongda.top

[T11] Kotlin：协程
来源：http://fhd.hnxiangtu.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://gif.meibo888.top

[T12] Kotlin：解构声明
来源：http://kgn.jyoumei.cn

val (a, b) = Pair(1, 2)
来源：http://vvg.jinqigfzy.top

[T13] Kotlin：只读 Map
来源：http://pgw.shuidangran.top

val m = mapOf("a" to 1)
来源：http://vtx.jyoumei.cn

[T14] Kotlin：循环
来源：http://evs.uphjek.com

for (i in 1..10) println(i)
来源：http://nyu.316326.xyz

[T15] Kotlin：接口
来源：http://fmn.havefunace.top

interface Shape { fun area(): Double }
来源：http://mqe.yueranfly.top

[T16] Swift：Hello World
来源：http://flp.dianchejie.cn

print("Hello")
来源：http://kgt.epnwcf.com

[T17] Swift：变量与常量
来源：http://gtn.ppjwa.cn

var a = 1;  let b = 2
来源：http://wsm.hfpthk.cn

[T18] Swift：字符串插值
来源：http://rhp.zdqjudy.top

"值: \(b)"
来源：http://qcp.havefunace.top

[T19] Swift：可选绑定
来源：http://sri.uphjek.com

if let n = opt { print(n) }
来源：http://sfh.quarkkingdee.top

[T20] Swift：数组操作
来源：http://qzm.yonumen.top

var a = [1, 2, 3];  a.append(4)
来源：http://xdg.hcnkem.com

[T21] Swift：遍历
来源：http://nia.dashuyun.cn

for x in a { print(x) }
来源：http://okk.chenjidiqi.icu

[T22] Swift：字典
来源：http://rka.xuetiantiany.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ohd.smart0.xyz

[T23] Swift：函数
来源：http://voj.meibo888.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kml.nanxinkj.top

[T24] Swift：闭包
来源：http://vdf.cdnleiting.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://rkq.feifeiyinyue.top

[T25] Swift：结构体
来源：http://gwc.xuanzx.com

struct P { var x: Int }
来源：http://oyv.andypj.xyz

[T26] Swift：类与重写
来源：http://nak.zhiwuduotai.top

class A: Base { override func f() {} }
来源：http://onb.hnxiangtu.top

[T27] Swift：错误处理
来源：http://fas.feifeiyinyue.top

do { try f() } catch { print(error) }
来源：http://gzd.yj20258888.top

[T28] Swift：枚举
来源：http://jeo.mhx1999.top

enum Color { case red, green }
来源：http://wcs.shanyushiyangkeji.top

[T29] Swift：guard 提前返回
来源：http://tpe.ywan-chungtsiang.top

guard let x = opt else { return }
来源：http://tos.fehbvm.com

[T30] Swift：协议
来源：http://cqe.yongpay.top

protocol Shape { func area() -> Double }
来源：http://psk.shanyushiyangtech.top

[T31] Lua：Hello World
来源：http://vmd.ybcxt.top

print("Hello")
来源：http://yoz.jinqigfzy.top

[T32] Lua：局部变量
来源：http://zui.mhx1999.top

local a = 1
来源：http://unh.svipenyu.cn

[T33] Lua：表（数组）
来源：http://mvk.andypj.xyz

local t = {1, 2, 3};  t[4] = 4
来源：http://tbo.uphjek.com

[T34] Lua：遍历表
来源：http://mjj.chenlongwang.top

for i, v in ipairs(t) do print(i, v) end
来源：http://rxb.yuxming.cn

[T35] Lua：字典表
来源：http://neu.sweek.top

local d = { a = 1 };  d.b = 2
来源：http://vvi.shanyushiyangtech.top

[T36] Lua：函数
来源：http://pvk.ctjpmb.com

function add(a, b) return a + b end
来源：http://bqc.quarkkingdee.top


<!-- 参考信息 -->