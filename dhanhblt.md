代发 wailian999

cmd > out.log 2>&1
来源：http://rqo.yuanzhike.top

[R40] 追加写日志
来源：http://dxz.shuidangran.top

echo "log" >> out.log
来源：http://xhq.uphjek.com

[R41] 丢弃输出
来源：http://ara.tarul.cn

cmd >/dev/null 2>&1
来源：http://lvh.tarul.cn

[R42] 输入重定向
来源：http://cjo.zhaomingkeji.xyz

wc -l < a.txt
来源：http://avb.epnwcf.com

[R43] 按名字查找文件
来源：http://ahi.chenzaomai.com

find . -name "*.log" -type f
来源：http://nhu.yangfankeji.com

[R44] 按修改时间查找
来源：http://jwx.cucudq.cn

find . -mtime -7 -type f
来源：http://juq.nanxinkj.top

[R45] 批量删除
来源：http://xzc.hysaishi.cn

find . -name "*.tmp" -delete
来源：http://non.meibo888.top

[R46] 递归替换文件内容
来源：http://upn.guannengcc.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zgb.zhaomingkeji.xyz

[R47] sed 单行替换
来源：http://gez.yuxming.cn

sed -i 's/foo/bar/g' a.txt
来源：http://yst.pycfn.com

[R48] awk 取指定列
来源：http://nfp.c1oappe.top

awk '{print $1, $3}' a.txt
来源：http://qel.zhiwuduotai.top

[R49] awk 带条件
来源：http://wnw.tanke756.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zmo.birdmap.top

[R50] awk 求和
来源：http://bbp.andypj.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://dpj.zhaomingkeji.xyz

[R51] 排序去重取前几
来源：http://tiq.yuxming.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qou.chenjidiqi.icu

[R52] 统计行数
来源：http://nis.zdqjudy.top

wc -l a.txt
来源：http://dwa.zycfv.cn

[R53] 查看文件头与实时尾
来源：http://uyu.zdbjq.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uka.cqqwz.cn

[R54] 比较两个文件
来源：http://dti.haohaochexian.top

diff a.txt b.txt
来源：http://icg.ybcxt.top

[R55] 压缩与解压
来源：http://bke.havefunace.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ayt.svipenyu.cn

[R56] 远程拷贝
来源：http://kjq.jiagoushi.top

scp file user@host:/path/
来源：http://qag.yuanzhike.top

[R57] 远程执行命令
来源：http://eid.tanke756.top

ssh user@host 'uptime'
来源：http://dqh.xuetiantiany.cn

[R58] 下载文件
来源：http://dnc.cqqwz.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cdj.iojbl.cn

[R59] 发 POST JSON
来源：http://lec.jinqigufen.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qvk.yj20258.top

[R60] 只看 HTTP 状态码
来源：http://mht.jinyuanbaomall.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qdq.yfazqb.com

[R61] 磁盘占用
来源：http://cdi.zycfv.cn

df -h;  du -sh *
来源：http://npx.xylfe.cn

[R62] 找最占空间的文件
来源：http://nrv.zdbjq.cn

du -ah . | sort -rh | head -10
来源：http://beg.hcnkem.com

[R63] 内存与进程
来源：http://jlh.jyoumei.cn

free -h;  ps aux | grep nginx
来源：http://emb.zdqjudy.top

[R64] 结束进程
来源：http://ugq.dashuyun.cn

kill -9 $(pgrep -f app.py)
来源：http://tsd.kuanghao11.cn

[R65] 查看端口占用
来源：http://qlo.ybcxt.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cno.tianlin.xyz

[R66] 定时任务
来源：http://agx.gzhubu.top

crontab -e;  crontab -l
来源：http://jxw.jinyuanbaomall.cn

[R67] 生成随机十六进制串
来源：http://jfr.chenjidiqi.icu

openssl rand -hex 16
来源：http://snl.svipenyu.cn

[R68] 计算文件校验值
来源：http://hxm.jianghu66.top

sha256sum a.txt;  md5sum a.txt
来源：http://gln.cdnleiting.top

[R69] 生成随机密码
来源：http://izd.xingfuxueyuan.xyz

head -c 16 /dev/urandom | base64
来源：http://rhm.cashguo.top

[R70] 时间戳与互转
来源：http://dsy.9152youxi.cn

date +%s;  date -d @1700000000
来源：http://qcm.haohaochexian.top

[R71] 日期格式化
来源：http://ybp.havefunace.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://zsv.shzxlz.cn

[R72] 等待端口就绪
来源：http://jei.hammf.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ezq.xylfe.cn

[R73] 分割大日志
来源：http://gos.hesvh.cn

split -l 1000 big.log part_
来源：http://dmv.ctjpmb.com

[R74] 批量重命名
来源：http://hym.sysykeji.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://owl.sjlbkw.cn

[R75] 导出环境变量
来源：http://che.ctjpmb.com

export PATH="$HOME/bin:$PATH"
来源：http://ubf.nanxinkj.top

[R76] 使用临时文件
来源：http://yiz.nwbrower.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jjk.snrcjt.cn

[R77] 读取用户输入
来源：http://gxz.havefunace.top

read -rp "请输入: " ans
来源：http://olr.aibaodan.cn

[R78] 交互式菜单
来源：http://mwx.yj202588.top

select opt in a b c; do echo "$opt"; break; done
来源：http://hhn.yueranfly.top

[R79] 解析命令行选项
来源：http://dxq.shangyingyoupin.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kuf.hnqzz.top

[R80] 查看脚本执行耗时
来源：http://gqb.daxiang520.top

time ./run.sh
来源：http://wqi.yongpay.top

================================================================================
来源：http://vfp.shanyushiyangtech.top

S. C / C++ 专题
来源：http://dvp.birdmap.top

================================================================================
来源：http://wpg.redwolf501.top

[S01] C：Hello World
来源：http://yqq.svipenyu.cn

#include <stdio.h>
来源：http://bfb.zhiwuduotai.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://kxu.yuanzhike.top

[S02] C：变量与格式化输出
来源：http://ydx.nwbrower.top

int a = 10; printf("%d\n", a);
来源：http://bia.zhoulong.xyz

[S03] C：读入整数
来源：http://ysp.316326.xyz

int x; scanf("%d", &x);
来源：http://bfi.feifeiyinyue.top

[S04] C：字符串复制
来源：http://lkm.xuanzx.com

char dst[32]; strcpy(dst, "hi");
来源：http://syq.quarkkingdee.top

[S05] C：字符串长度
来源：http://pbh.zhijiandao.cn

strlen(s)
来源：http://tgn.ctjpmb.com

[S06] C：字符串比较
来源：http://psj.snrcjt.cn

strcmp(a, b) == 0
来源：http://vmq.redwolf501.top

[S07] C：数组遍历求和
来源：http://eac.zycfv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ivc.kuanghao11.cn

[S08] C：动态内存分配与释放
来源：http://yzp.zycfv.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hwg.ydzc1.top

[S09] C：结构体定义与初始化
来源：http://usw.zhijiandao.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hsk.aibaodan.cn

[S10] C：指针与解引用
来源：http://mzg.ppjwa.cn

int *p = &a;  *p = 5;
来源：http://vzi.jiagoushi.top

[S11] C：逐行读文件
来源：http://qqe.9152youxi.cn

FILE *f = fopen("a.txt", "r");
来源：http://lhh.redwolf501.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://lqm.hnxiangtu.top

fclose(f);
来源：http://twd.cashguo.top

[S12] C：写文件
来源：http://ymk.yuxming.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qsg.jinghuilouyu.cn

[S13] C：宏定义
来源：http://rke.zdbjq.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nvr.sufxvd.cn

[S14] C：枚举
来源：http://ruu.bbcook.cn

enum Color { RED, GREEN, BLUE };
来源：http://kut.dianchejie.cn

[S15] C：类型转换
来源：http://jlb.hywenlv.cn

(double) a / b
来源：http://why.xylfe.cn

[S16] C：位操作置位
来源：http://omr.wangshuangyany.cn

x |= (1 << 3);
来源：http://fjp.hcnkem.com

[S17] C：安全拼接字符串
来源：http://nxb.xylfe.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sqg.zhoulong.xyz

[S18] C：命令行参数
来源：http://mtn.birdmap.top

int main(int argc, char **argv)
来源：http://hsi.havefunace.top

[S19] C：快速排序
来源：http://bob.hammf.cn

qsort(a, n, sizeof(int), cmp);
来源：http://lma.vehdjk.com

[S20] C：二分查找
来源：http://zsy.smart0.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ssn.hcnkem.com

[S21] C：字符类别判断
来源：http://vzb.shzxlz.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jus.yanxiufei.cn

[S22] C：字符串转数字
来源：http://ubv.gogol.net.cn

atoi("42");  strtod("3.14", NULL);
来源：http://uux.yfazqb.com

[S23] C：随机数
来源：http://uyd.fzhhl.top

srand(time(NULL));  int r = rand() % 100;
来源：http://mva.yj20258888.top

[S24] C：获取本地时间
来源：http://gwi.daria6918.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ahl.aizwys.cn

[S25] C：内存拷贝
来源：http://grj.zdqjudy.top

memcpy(dst, src, n);
来源：http://gbi.zhongyouzk.top

[S26] C：内存清零
来源：http://iiu.yongpay.top

memset(a, 0, sizeof a);
来源：http://afe.birdmap.top

[S27] C：定义常量
来源：http://xqq.uphjek.com

const double PI = 3.14159;
来源：http://oac.fanxiaobao.xyz

[S28] C：静态变量
来源：http://wbq.nwbrower.top

static int counter = 0;
来源：http://bep.hongshengwenyu.top

[S29] C：变参函数
来源：http://bfq.shangyingyoupin.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ksr.jianghu66.top

[S30] C：头文件保护
来源：http://snp.snrcjt.cn

#ifndef X_H
来源：http://ojs.guowangkeji.top

#define X_H
来源：http://cct.daxiang520.top

#endif
来源：http://gxe.sxryk.cn

[S31] C++：Hello World
来源：http://hvf.zhongyouzk.top

#include <iostream>
来源：http://cky.pengpengdd.cyou

int main() { std::cout << "Hello\n"; }
来源：http://awd.yj202588.top

[S32] C++：字符串
来源：http://fff.chenjidiqi.icu

std::string s = "hi";  s += "!";
来源：http://obx.nanxinkj.top

[S33] C++：vector 增删
来源：http://ziu.yuanzhike.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sqe.sxryk.cn

[S34] C++：遍历 vector
来源：http://zhm.xuetiantiany.cn

for (auto &x : v) { std::cout << x; }
来源：http://bdv.sweek.top

[S35] C++：map
来源：http://jgh.yueranfly.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kqi.hfpthk.cn

[S36] C++：unordered_map
来源：http://uxb.chenlongwang.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dbt.shzxlz.cn

[S37] C++：set
来源：http://gpu.xingfuxueyuan.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xaa.yuxming.cn

[S38] C++：排序
来源：http://nqj.shanyushiyangtech.top

std::sort(v.begin(), v.end());
来源：http://igx.cucudq.cn

[S39] C++：自定义比较器排序
来源：http://vqe.shzxlz.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bvo.gzhubu.top

[S40] C++：查找元素
来源：http://jdu.52xcode.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rxe.zhengqikj.top

[S41] C++：类与构造函数
来源：http://gza.dashuyun.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bea.yuxming.cn

[S42] C++：继承与虚函数
来源：http://niu.jiagoushi.top

class B : public Base { public: void f() override {} };
来源：http://ugf.jinyuanbaomall.cn

[S43] C++：智能指针
来源：http://fpl.tianlin.xyz

auto p = std::make_unique<int>(5);
来源：http://dfu.hcnkem.com

[S44] C++：引用传参
来源：http://lwg.nanxuanxn.top

void inc(int &x) { ++x; }
来源：http://jqk.kuanghao11.cn

[S45] C++：lambda
来源：http://anz.daxiang520.top

auto add = [](int a, int b) { return a + b; };
来源：http://lvi.tarul.cn

[S46] C++：函数模板
来源：http://ajr.cdnleiting.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fzc.zhoulong.xyz

[S47] C++：结构化绑定遍历
来源：http://bzs.shzxlz.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hdf.yuanzhike.top

[S48] C++：逐行读文件
来源：http://wxk.sxryk.cn

std::ifstream in("a.txt");  std::string line;
来源：http://tkv.hysaishi.cn

while (std::getline(in, line)) { }
来源：http://euw.zhijiandao.cn

[S49] C++：写文件
来源：http://jfz.fanxiaobao.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cbv.snrcjt.cn

[S50] C++：格式化数字
来源：http://dpg.fehbvm.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bjr.316326.xyz

[S51] C++：显式类型转换
来源：http://jmb.sweek.top

static_cast<double>(a) / b
来源：http://dpv.yj20258888.top

[S52] C++：const 与 noexcept
来源：http://etq.jianghu66.top

int size() const noexcept { return n_; }
来源：http://rgs.quarkkingdee.top

[S53] C++：移动语义
来源：http://ywr.nanxuanxn.top

std::vector<int> w = std::move(v);
来源：http://fdy.xuanzx.com

[S54] C++：异常处理
来源：http://veu.ybcxt.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cuy.pycfn.com

[S55] C++：结构化绑定
来源：http://asf.xuetiantiany.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ryf.yj202588.top

[S56] C++：optional
来源：http://cij.chenjidiqi.icu

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jfy.shzxlz.cn

[S57] C++：编译期常量
来源：http://gau.zycfv.cn

constexpr int N = 10;
来源：http://bpr.hfpthk.cn

[S58] C++：命名空间
来源：http://edo.sjlbkw.cn

namespace ns { int f() { return 1; } }
来源：http://qfa.gzhubu.top

[S59] C++：静态断言
来源：http://xhy.fehbvm.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rsc.zhaomingkeji.xyz

[S60] C++：遍历并删除元素
来源：http://fhd.ivvv.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ldz.shanyushiyangtech.top

================================================================================
来源：http://ekg.zhongyouzk.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://grw.zhoulong.xyz

================================================================================
来源：http://yku.jqgfzy.top

[T01] Kotlin：Hello World
来源：http://byj.haohaochexian.top

println("Hello")
来源：http://bxk.sufxvd.cn

[T02] Kotlin：变量
来源：http://zvm.xinyue.icu

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bsx.yuanzhike.top

[T03] Kotlin：字符串模板
来源：http://zwv.tanke756.top

"值: $b"
来源：http://bmq.yj20258888.top

[T04] Kotlin：空安全
来源：http://msc.xingfuxueyuan.xyz

val n: String? = null;  n?.length
来源：http://pgd.shanyushiyangkeji.top

[T05] Kotlin：when 表达式
来源：http://wri.fktsv.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jlk.yj20258.top

[T06] Kotlin：集合映射
来源：http://zxj.gotoacloud.top

listOf(1, 2, 3).map { it * 2 }
来源：http://qaf.pengpengdd.cyou

[T07] Kotlin：集合过滤
来源：http://exd.jinghuilouyu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://zdt.sweek.top

[T08] Kotlin：数据类
来源：http://nbr.daxiang520.top

data class User(val name: String, val age: Int)
来源：http://tlq.dashuyun.cn

[T09] Kotlin：扩展函数
来源：http://wau.dashuyun.cn

fun String.exclaim() = this + "!"
来源：http://zoa.sweek.top

[T10] Kotlin：默认参数
来源：http://bmu.wangshuangyany.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://hgx.pengpengdd.cyou

[T11] Kotlin：协程
来源：http://rtg.zhiwuduotai.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://tkw.nwbrower.top

[T12] Kotlin：解构声明
来源：http://qxb.hcnkem.com

val (a, b) = Pair(1, 2)
来源：http://wnm.hammf.cn

[T13] Kotlin：只读 Map
来源：http://qhn.c1oappe.top

val m = mapOf("a" to 1)
来源：http://stb.cucudq.cn

[T14] Kotlin：循环
来源：http://cob.zhoulong.xyz

for (i in 1..10) println(i)
来源：http://lhi.ehwqpu.com

[T15] Kotlin：接口
来源：http://xuc.jinyuanbaomall.cn

interface Shape { fun area(): Double }
来源：http://jsh.xinyue.icu

[T16] Swift：Hello World
来源：http://mrx.gotoacloud.top

print("Hello")
来源：http://qfs.chenjidiqi.icu

[T17] Swift：变量与常量
来源：http://peq.zhoulong.xyz

var a = 1;  let b = 2
来源：http://xaf.cheryme.top

[T18] Swift：字符串插值
来源：http://oiz.iojbl.cn

"值: \(b)"
来源：http://ajx.52xcode.cn

[T19] Swift：可选绑定
来源：http://ahn.dianchejie.cn

if let n = opt { print(n) }
来源：http://wag.dashuyun.cn

[T20] Swift：数组操作
来源：http://dsp.nanxinkj.top

var a = [1, 2, 3];  a.append(4)
来源：http://dhi.xuanzx.com

[T21] Swift：遍历
来源：http://cop.snrcjt.cn

for x in a { print(x) }
来源：http://hpi.fanxiaobao.xyz

[T22] Swift：字典
来源：http://ytc.ehwqpu.com

var d = ["a": 1];  d["b"] = 2
来源：http://iip.ivvv.top

[T23] Swift：函数
来源：http://did.fzhhl.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hah.gaohongyu789.top

[T24] Swift：闭包
来源：http://irw.ehwqpu.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://rcw.jinyuanbaomall.cn

[T25] Swift：结构体
来源：http://rnn.pengpengdd.cyou

struct P { var x: Int }
来源：http://gnk.shangyingyoupin.top

[T26] Swift：类与重写
来源：http://doq.zhijiandao.cn

class A: Base { override func f() {} }
来源：http://qtw.sufxvd.cn

[T27] Swift：错误处理
来源：http://tzq.yuxming.cn

do { try f() } catch { print(error) }
来源：http://qpa.ydzc1.top

[T28] Swift：枚举
来源：http://bav.vqdsnc.cn

enum Color { case red, green }
来源：http://zrj.hnqzz.top

[T29] Swift：guard 提前返回
来源：http://mkf.kuanghao11.cn

guard let x = opt else { return }
来源：http://uwi.shanyushiyangkeji.top

[T30] Swift：协议
来源：http://fft.jqgfzy.top

protocol Shape { func area() -> Double }
来源：http://szt.sweek.top

[T31] Lua：Hello World
来源：http://jbh.zhiwuduotai.top

print("Hello")
来源：http://pdb.xinyue.icu

[T32] Lua：局部变量
来源：http://cjv.9152youxi.cn

local a = 1
来源：http://bbg.xylfe.cn

[T33] Lua：表（数组）
来源：http://zuz.fehbvm.com

local t = {1, 2, 3};  t[4] = 4
来源：http://mrx.svipenyu.cn

[T34] Lua：遍历表
来源：http://aku.fehbvm.com

for i, v in ipairs(t) do print(i, v) end
来源：http://ttc.vqdsnc.cn

[T35] Lua：字典表
来源：http://ore.hysaishi.cn

local d = { a = 1 };  d.b = 2
来源：http://nex.fzhhl.top

[T36] Lua：函数
来源：http://xsm.wangdashe.top

function add(a, b) return a + b end
来源：http://dje.zdbjq.cn

[T37] Lua：字符串拼接
来源：http://svq.snrcjt.cn

"a" .. "b"
来源：http://htt.shanyushiyangtech.top

[T38] Lua：条件
来源：http://ipz.ppjwa.cn

if x > 0 then print("正") end
来源：http://imk.gzhubu.top

[T39] Lua：模式匹配
来源：http://uip.bjfxy.top

string.find(s, "%d+")
来源：http://dum.xinyue.icu

[T40] Lua：元表
来源：http://pos.dianchejie.cn

setmetatable({}, { __index = base })
来源：http://eru.cheryme.top

[T41] Perl：Hello World
来源：http://lzp.daria6918.cn

print "Hello\n";
来源：http://jbg.hysaishi.cn

[T42] Perl：变量类型
来源：http://hzd.zhijiandao.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ene.wangdashe.top


<!-- 参考信息 -->