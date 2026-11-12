代发 wailian999

find . -name "*.log" -type f
来源：http://ibf.jinghuilouyu.cn

[R44] 按修改时间查找
来源：http://ogp.aibaodan.cn

find . -mtime -7 -type f
来源：http://ohk.zdqjudy.top

[R45] 批量删除
来源：http://emc.xziqi.cn

find . -name "*.tmp" -delete
来源：http://bfo.cheryme.top

[R46] 递归替换文件内容
来源：http://dhu.zhengqikj.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lkp.jianghu66.top

[R47] sed 单行替换
来源：http://avl.tianlin.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://cqv.jyoumei.cn

[R48] awk 取指定列
来源：http://jvb.zhijiandao.cn

awk '{print $1, $3}' a.txt
来源：http://cpf.cheryme.top

[R49] awk 带条件
来源：http://asx.fktsv.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://eno.yvedp.cn

[R50] awk 求和
来源：http://wdx.bjfxy.top

awk '{s += $2} END {print s}' a.txt
来源：http://yst.0kj1m.cn

[R51] 排序去重取前几
来源：http://yuj.zhaomingkeji.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://xcw.yvedp.cn

[R52] 统计行数
来源：http://vjs.yuxming.cn

wc -l a.txt
来源：http://vhr.shuidangran.top

[R53] 查看文件头与实时尾
来源：http://thb.guannengcc.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dct.ywan-chungtsiang.top

[R54] 比较两个文件
来源：http://jgq.fanxiaobao.xyz

diff a.txt b.txt
来源：http://cjt.mhx1999.top

[R55] 压缩与解压
来源：http://eeh.hywenlv.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rlh.zhijiandao.cn

[R56] 远程拷贝
来源：http://fej.yuanzhike.top

scp file user@host:/path/
来源：http://qla.shangyingyoupin.top

[R57] 远程执行命令
来源：http://vyw.gaohongyu789.top

ssh user@host 'uptime'
来源：http://cja.yfazqb.com

[R58] 下载文件
来源：http://zgu.yj20258.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kfd.meibo888.top

[R59] 发 POST JSON
来源：http://wnw.daria6918.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yli.hammf.cn

[R60] 只看 HTTP 状态码
来源：http://ort.sysykeji.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vii.cdnleiting.top

[R61] 磁盘占用
来源：http://ddn.aizwys.cn

df -h;  du -sh *
来源：http://wos.iojbl.cn

[R62] 找最占空间的文件
来源：http://bha.nanxinkj.top

du -ah . | sort -rh | head -10
来源：http://unu.gogol.net.cn

[R63] 内存与进程
来源：http://ssy.sysykeji.top

free -h;  ps aux | grep nginx
来源：http://rte.zhoulong.xyz

[R64] 结束进程
来源：http://dpn.shzxlz.cn

kill -9 $(pgrep -f app.py)
来源：http://voe.yuanzhike.top

[R65] 查看端口占用
来源：http://egd.pengpengdd.cyou

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yws.hywenlv.cn

[R66] 定时任务
来源：http://ydh.shuidangran.top

crontab -e;  crontab -l
来源：http://ivn.andypj.xyz

[R67] 生成随机十六进制串
来源：http://pba.shanyushiyangtech.top

openssl rand -hex 16
来源：http://frl.jlsjyb.cn

[R68] 计算文件校验值
来源：http://wko.bjfxy.top

sha256sum a.txt;  md5sum a.txt
来源：http://zjl.epnwcf.com

[R69] 生成随机密码
来源：http://ffd.cqqwz.cn

head -c 16 /dev/urandom | base64
来源：http://gzg.zhaomingkeji.xyz

[R70] 时间戳与互转
来源：http://eaf.xuetiantiany.cn

date +%s;  date -d @1700000000
来源：http://gis.sufxvd.cn

[R71] 日期格式化
来源：http://fkg.andypj.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://mfo.c1oappe.top

[R72] 等待端口就绪
来源：http://zzi.zhengqikj.top

until nc -z localhost 3306; do sleep 1; done
来源：http://eeg.jlsjyb.cn

[R73] 分割大日志
来源：http://lza.haohaochexian.top

split -l 1000 big.log part_
来源：http://ieo.xziqi.cn

[R74] 批量重命名
来源：http://jrd.sufxvd.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ewj.hesvh.cn

[R75] 导出环境变量
来源：http://eab.daxiang520.top

export PATH="$HOME/bin:$PATH"
来源：http://bfn.aizwys.cn

[R76] 使用临时文件
来源：http://kqd.cucudq.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mcv.bbcook.cn

[R77] 读取用户输入
来源：http://tjz.yangfankeji.com

read -rp "请输入: " ans
来源：http://ebm.jinqigfzy.top

[R78] 交互式菜单
来源：http://pij.yj202588.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ifm.xylfe.cn

[R79] 解析命令行选项
来源：http://ied.uphjek.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jsp.chenjidiqi.icu

[R80] 查看脚本执行耗时
来源：http://crd.jqgufenzy.top

time ./run.sh
来源：http://mib.cucudq.cn

================================================================================
来源：http://dum.tarul.cn

S. C / C++ 专题
来源：http://rmt.hnqzz.top

================================================================================
来源：http://ksv.fzhhl.top

[S01] C：Hello World
来源：http://ymb.bjfxy.top

#include <stdio.h>
来源：http://twc.snrcjt.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://wei.bjfxy.top

[S02] C：变量与格式化输出
来源：http://wmi.quarkkingdee.top

int a = 10; printf("%d\n", a);
来源：http://gtt.jqgufenzy.top

[S03] C：读入整数
来源：http://wih.zhengqikj.top

int x; scanf("%d", &x);
来源：http://hec.gzhubu.top

[S04] C：字符串复制
来源：http://ixw.aizwys.cn

char dst[32]; strcpy(dst, "hi");
来源：http://tbg.hcnkem.com

[S05] C：字符串长度
来源：http://fzm.redwolf501.top

strlen(s)
来源：http://mqw.shzxlz.cn

[S06] C：字符串比较
来源：http://fek.shanyushiyangkeji.top

strcmp(a, b) == 0
来源：http://xug.ehwqpu.com

[S07] C：数组遍历求和
来源：http://bfs.pycfn.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nfo.tian-w.cn

[S08] C：动态内存分配与释放
来源：http://wft.ywan-chungtsiang.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uqp.chenjidiqi.icu

[S09] C：结构体定义与初始化
来源：http://mtq.chenzaomai.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bms.wangshuangyany.cn

[S10] C：指针与解引用
来源：http://tob.wangshuangyany.cn

int *p = &a;  *p = 5;
来源：http://gfc.ctjpmb.com

[S11] C：逐行读文件
来源：http://keq.sjlbkw.cn

FILE *f = fopen("a.txt", "r");
来源：http://jjo.xinyue.icu

while (fgets(buf, sizeof buf, f)) { }
来源：http://yft.xuetiantiany.cn

fclose(f);
来源：http://kfj.ehwqpu.com

[S12] C：写文件
来源：http://mia.316326.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nlm.ydjk.org.cn

[S13] C：宏定义
来源：http://pkr.cucudq.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://utr.nanxinkj.top

[S14] C：枚举
来源：http://oeq.yangfankeji.com

enum Color { RED, GREEN, BLUE };
来源：http://bsr.zdbjq.cn

[S15] C：类型转换
来源：http://kra.gotoacloud.top

(double) a / b
来源：http://vdk.shuidangran.top

[S16] C：位操作置位
来源：http://qgz.hesvh.cn

x |= (1 << 3);
来源：http://eep.ivvv.top

[S17] C：安全拼接字符串
来源：http://thx.chenzaomai.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://aho.yonumen.top

[S18] C：命令行参数
来源：http://jsq.yangfankeji.com

int main(int argc, char **argv)
来源：http://rke.mhx1999.top

[S19] C：快速排序
来源：http://exk.hnqzz.top

qsort(a, n, sizeof(int), cmp);
来源：http://uek.jinyuanbaomall.cn

[S20] C：二分查找
来源：http://ujp.sysykeji.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mcc.zhijiandao.cn

[S21] C：字符类别判断
来源：http://ubw.ywan-chungtsiang.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gru.yj202588.top

[S22] C：字符串转数字
来源：http://ovq.guannengcc.top

atoi("42");  strtod("3.14", NULL);
来源：http://pwo.yj202588.top

[S23] C：随机数
来源：http://buq.c1oappe.top

srand(time(NULL));  int r = rand() % 100;
来源：http://rux.fktsv.cn

[S24] C：获取本地时间
来源：http://ftn.daxiang520.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sdl.birdmap.top

[S25] C：内存拷贝
来源：http://vtv.fengsongda.top

memcpy(dst, src, n);
来源：http://osh.zycfv.cn

[S26] C：内存清零
来源：http://avj.zhoulong.xyz

memset(a, 0, sizeof a);
来源：http://nla.yj20258.top

[S27] C：定义常量
来源：http://cip.ppjwa.cn

const double PI = 3.14159;
来源：http://uck.mhx1999.top

[S28] C：静态变量
来源：http://zlk.iojbl.cn

static int counter = 0;
来源：http://hnb.zhijiandao.cn

[S29] C：变参函数
来源：http://vyw.zhoulong.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nov.jiagoushi.top

[S30] C：头文件保护
来源：http://okf.fanxiaobao.xyz

#ifndef X_H
来源：http://dsq.jinqigufen.top

#define X_H
来源：http://ide.jianghu66.top

#endif
来源：http://dlu.xylfe.cn

[S31] C++：Hello World
来源：http://gsh.tanke756.top

#include <iostream>
来源：http://tzw.yongpay.top

int main() { std::cout << "Hello\n"; }
来源：http://zly.tianlin.xyz

[S32] C++：字符串
来源：http://zeu.chenlongwang.top

std::string s = "hi";  s += "!";
来源：http://yex.gogol.net.cn

[S33] C++：vector 增删
来源：http://pdu.hysaishi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://weq.sweek.top

[S34] C++：遍历 vector
来源：http://pfs.fehbvm.com

for (auto &x : v) { std::cout << x; }
来源：http://ljr.yj20258888.top

[S35] C++：map
来源：http://nui.ppjwa.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dvv.ivvv.top

[S36] C++：unordered_map
来源：http://duz.mhx1999.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ivm.fanxiaobao.xyz

[S37] C++：set
来源：http://dcg.yuanzhike.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gyo.andypj.xyz

[S38] C++：排序
来源：http://zkn.gotoacloud.top

std::sort(v.begin(), v.end());
来源：http://jew.yonumen.top

[S39] C++：自定义比较器排序
来源：http://vbn.zdbjq.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fxq.feifeiyinyue.top

[S40] C++：查找元素
来源：http://abm.yvedp.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fbd.shanyushiyangtech.top

[S41] C++：类与构造函数
来源：http://ish.ppjwa.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hjh.ydzc1.top

[S42] C++：继承与虚函数
来源：http://tvl.xziqi.cn

class B : public Base { public: void f() override {} };
来源：http://myg.sysykeji.top

[S43] C++：智能指针
来源：http://mgs.yj20258.top

auto p = std::make_unique<int>(5);
来源：http://pcm.tanke756.top

[S44] C++：引用传参
来源：http://yce.9152youxi.cn

void inc(int &x) { ++x; }
来源：http://yrd.cqqwz.cn

[S45] C++：lambda
来源：http://fav.zycfv.cn

auto add = [](int a, int b) { return a + b; };
来源：http://sez.c1oappe.top

[S46] C++：函数模板
来源：http://drk.hysaishi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://upi.hnxiangtu.top

[S47] C++：结构化绑定遍历
来源：http://prc.yonumen.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kya.jlsjyb.cn

[S48] C++：逐行读文件
来源：http://joe.chenzaomai.com

std::ifstream in("a.txt");  std::string line;
来源：http://qgh.hfpthk.cn

while (std::getline(in, line)) { }
来源：http://kaj.chenzaomai.com

[S49] C++：写文件
来源：http://ubu.jqgfzy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ugn.bjfxy.top

[S50] C++：格式化数字
来源：http://tnv.jianghu66.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://iah.xuanzx.com

[S51] C++：显式类型转换
来源：http://ivq.tarul.cn

static_cast<double>(a) / b
来源：http://ezo.ydzc1.top

[S52] C++：const 与 noexcept
来源：http://axj.yj20258888.top

int size() const noexcept { return n_; }
来源：http://lmx.hnxiangtu.top

[S53] C++：移动语义
来源：http://hgq.epnwcf.com

std::vector<int> w = std::move(v);
来源：http://ask.ppjwa.cn

[S54] C++：异常处理
来源：http://znp.zhoulong.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mig.cdnleiting.top

[S55] C++：结构化绑定
来源：http://xza.sweek.top

auto [a, b] = std::make_pair(1, 2);
来源：http://bow.tanke756.top

[S56] C++：optional
来源：http://eaj.sjlbkw.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://usk.sysykeji.top

[S57] C++：编译期常量
来源：http://dmk.dashuyun.cn

constexpr int N = 10;
来源：http://brj.sxryk.cn

[S58] C++：命名空间
来源：http://lhw.tian-w.cn

namespace ns { int f() { return 1; } }
来源：http://joq.dianchejie.cn

[S59] C++：静态断言
来源：http://jax.fzhhl.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uoz.sjlbkw.cn

[S60] C++：遍历并删除元素
来源：http://sux.xingfuxueyuan.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zcb.feifeiyinyue.top

================================================================================
来源：http://ujl.bbcook.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://aoz.fanxiaobao.xyz

================================================================================
来源：http://wql.jinghuilouyu.cn

[T01] Kotlin：Hello World
来源：http://bdu.ybcxt.top

println("Hello")
来源：http://trf.yj20258888.top

[T02] Kotlin：变量
来源：http://bqc.epnwcf.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dpo.dianchejie.cn

[T03] Kotlin：字符串模板
来源：http://lvk.gaohongyu789.top

"值: $b"
来源：http://oyi.snrcjt.cn

[T04] Kotlin：空安全
来源：http://aqb.xziqi.cn

val n: String? = null;  n?.length
来源：http://oxh.dianchejie.cn

[T05] Kotlin：when 表达式
来源：http://szq.wangdashe.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yei.xuanzx.com

[T06] Kotlin：集合映射
来源：http://ofh.hnxiangtu.top

listOf(1, 2, 3).map { it * 2 }
来源：http://dbq.wangdashe.top

[T07] Kotlin：集合过滤
来源：http://eet.yj20258888.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://zmd.zhaomingkeji.xyz

[T08] Kotlin：数据类
来源：http://yaf.ywan-chungtsiang.top

data class User(val name: String, val age: Int)
来源：http://bev.aizwys.cn

[T09] Kotlin：扩展函数
来源：http://hzn.c1oappe.top

fun String.exclaim() = this + "!"
来源：http://pbo.ywan-chungtsiang.top

[T10] Kotlin：默认参数
来源：http://wqi.quarkkingdee.top

fun greet(name: String = "World") = "Hi $name"
来源：http://eea.svipenyu.cn

[T11] Kotlin：协程
来源：http://nmr.hongshengwenyu.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://bcv.smart0.xyz

[T12] Kotlin：解构声明
来源：http://efn.jlsjyb.cn

val (a, b) = Pair(1, 2)
来源：http://euj.hesvh.cn

[T13] Kotlin：只读 Map
来源：http://bck.tanke756.top

val m = mapOf("a" to 1)
来源：http://aue.shangyingyoupin.top

[T14] Kotlin：循环
来源：http://mho.sufxvd.cn

for (i in 1..10) println(i)
来源：http://too.tarul.cn

[T15] Kotlin：接口
来源：http://wax.chenlongwang.top

interface Shape { fun area(): Double }
来源：http://gsk.iojbl.cn

[T16] Swift：Hello World
来源：http://gum.jinqigufen.top

print("Hello")
来源：http://ewr.fengsongda.top

[T17] Swift：变量与常量
来源：http://pjr.sweek.top

var a = 1;  let b = 2
来源：http://ikw.snrcjt.cn

[T18] Swift：字符串插值
来源：http://cdv.cheryme.top

"值: \(b)"
来源：http://vyd.xziqi.cn

[T19] Swift：可选绑定
来源：http://huz.zhoulong.xyz

if let n = opt { print(n) }
来源：http://iiz.yuxming.cn

[T20] Swift：数组操作
来源：http://cuj.daxiang520.top

var a = [1, 2, 3];  a.append(4)
来源：http://yuv.sxryk.cn

[T21] Swift：遍历
来源：http://ssd.zdqjudy.top

for x in a { print(x) }
来源：http://aoe.hcnkem.com

[T22] Swift：字典
来源：http://xts.bjfxy.top

var d = ["a": 1];  d["b"] = 2
来源：http://zxe.hysaishi.cn

[T23] Swift：函数
来源：http://zfy.xylfe.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zol.zhaomingkeji.xyz

[T24] Swift：闭包
来源：http://pzt.vqdsnc.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://jsn.xinyue.icu

[T25] Swift：结构体
来源：http://txv.yongpay.top

struct P { var x: Int }
来源：http://ecw.yuxming.cn

[T26] Swift：类与重写
来源：http://ous.jlsjyb.cn

class A: Base { override func f() {} }
来源：http://xer.daria6918.cn

[T27] Swift：错误处理
来源：http://tqp.zhongyouzk.top

do { try f() } catch { print(error) }
来源：http://yum.yueranfly.top

[T28] Swift：枚举
来源：http://amo.cucudq.cn

enum Color { case red, green }
来源：http://ibr.zdbjq.cn

[T29] Swift：guard 提前返回
来源：http://vus.c1oappe.top

guard let x = opt else { return }
来源：http://cos.birdmap.top

[T30] Swift：协议
来源：http://ngi.hfpthk.cn

protocol Shape { func area() -> Double }
来源：http://xhb.xylfe.cn

[T31] Lua：Hello World
来源：http://kiy.yj202588.top

print("Hello")
来源：http://qpe.zhaomingkeji.xyz

[T32] Lua：局部变量
来源：http://gbn.xylfe.cn

local a = 1
来源：http://uto.gotoacloud.top

[T33] Lua：表（数组）
来源：http://uzi.shzxlz.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://omv.guannengcc.top

[T34] Lua：遍历表
来源：http://qzo.shanyushiyangtech.top

for i, v in ipairs(t) do print(i, v) end
来源：http://cjm.fanxiaobao.xyz

[T35] Lua：字典表
来源：http://xks.mhx1999.top

local d = { a = 1 };  d.b = 2
来源：http://psg.zycfv.cn

[T36] Lua：函数
来源：http://uit.zhiwuduotai.top

function add(a, b) return a + b end
来源：http://ohk.zhaomingkeji.xyz

[T37] Lua：字符串拼接
来源：http://qag.dashuyun.cn

"a" .. "b"
来源：http://zuy.ybcxt.top

[T38] Lua：条件
来源：http://xdp.aizwys.cn

if x > 0 then print("正") end
来源：http://rnv.zdbjq.cn

[T39] Lua：模式匹配
来源：http://qrz.zdqjudy.top

string.find(s, "%d+")
来源：http://lay.snrcjt.cn

[T40] Lua：元表
来源：http://cqh.shangyingyoupin.top

setmetatable({}, { __index = base })
来源：http://clo.jinghuilouyu.cn

[T41] Perl：Hello World
来源：http://auh.hammf.cn

print "Hello\n";
来源：http://gvp.ivvv.top

[T42] Perl：变量类型
来源：http://xra.wangdashe.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cqo.ivvv.top

[T43] Perl：字符串插值
来源：http://viu.ydjk.org.cn

"值: $a"
来源：http://kpl.jyoumei.cn

[T44] Perl：条件
来源：http://sdn.jqgfzy.top

if ($a > 0) { print "正"; }
来源：http://ygx.yvedp.cn

[T45] Perl：数组遍历
来源：http://jiz.cheryme.top

for my $x (@arr) { print $x; }
来源：http://exn.jinyuanbaomall.cn

[T46] Perl：哈希操作
来源：http://ccv.nanxinkj.top

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fge.sufxvd.cn


<!-- 参考信息 -->