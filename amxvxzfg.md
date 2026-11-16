代发 wailian999

cmd > out.log 2>&1
来源：http://zby.bbcook.cn

[R40] 追加写日志
来源：http://gme.ppjwa.cn

echo "log" >> out.log
来源：http://zqp.fanxiaobao.xyz

[R41] 丢弃输出
来源：http://lqj.yuxming.cn

cmd >/dev/null 2>&1
来源：http://fnx.bbcook.cn

[R42] 输入重定向
来源：http://alv.yj20258888.top

wc -l < a.txt
来源：http://bfd.kuanghao11.cn

[R43] 按名字查找文件
来源：http://dnx.andypj.xyz

find . -name "*.log" -type f
来源：http://lfu.316326.xyz

[R44] 按修改时间查找
来源：http://err.jianghu66.top

find . -mtime -7 -type f
来源：http://pxn.yanxiufei.cn

[R45] 批量删除
来源：http://fls.ydzc1.top

find . -name "*.tmp" -delete
来源：http://xjq.c1oappe.top

[R46] 递归替换文件内容
来源：http://qme.fengsongda.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wva.tian-w.cn

[R47] sed 单行替换
来源：http://hzn.ywan-chungtsiang.top

sed -i 's/foo/bar/g' a.txt
来源：http://vna.xuetiantiany.cn

[R48] awk 取指定列
来源：http://fby.shanyushiyangkeji.top

awk '{print $1, $3}' a.txt
来源：http://wrz.hnxiangtu.top

[R49] awk 带条件
来源：http://vqs.yanxiufei.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jks.yueranfly.top

[R50] awk 求和
来源：http://wvd.iojbl.cn

awk '{s += $2} END {print s}' a.txt
来源：http://beq.haohaochexian.top

[R51] 排序去重取前几
来源：http://vdf.sweek.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ppk.bjfxy.top

[R52] 统计行数
来源：http://hul.jinqigufen.top

wc -l a.txt
来源：http://zwn.9152youxi.cn

[R53] 查看文件头与实时尾
来源：http://gsa.jiagoushi.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kex.9152youxi.cn

[R54] 比较两个文件
来源：http://qzq.sysykeji.top

diff a.txt b.txt
来源：http://pio.fanxiaobao.xyz

[R55] 压缩与解压
来源：http://tyg.sxryk.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kgl.svipenyu.cn

[R56] 远程拷贝
来源：http://vwe.gotoacloud.top

scp file user@host:/path/
来源：http://yep.smart0.xyz

[R57] 远程执行命令
来源：http://ssp.aibaodan.cn

ssh user@host 'uptime'
来源：http://alw.316326.xyz

[R58] 下载文件
来源：http://vjk.hywenlv.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ccx.jiagoushi.top

[R59] 发 POST JSON
来源：http://pku.snrcjt.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xzb.yj20258888.top

[R60] 只看 HTTP 状态码
来源：http://idi.ctjpmb.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mqg.xylfe.cn

[R61] 磁盘占用
来源：http://spu.meibo888.top

df -h;  du -sh *
来源：http://fza.dashuyun.cn

[R62] 找最占空间的文件
来源：http://hmj.xuetiantiany.cn

du -ah . | sort -rh | head -10
来源：http://xqt.havefunace.top

[R63] 内存与进程
来源：http://jcb.jyoumei.cn

free -h;  ps aux | grep nginx
来源：http://yuh.fehbvm.com

[R64] 结束进程
来源：http://ekr.iojbl.cn

kill -9 $(pgrep -f app.py)
来源：http://wfn.zhoulong.xyz

[R65] 查看端口占用
来源：http://xeg.yj20258.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rvz.mhx1999.top

[R66] 定时任务
来源：http://uud.wangdashe.top

crontab -e;  crontab -l
来源：http://oss.ybcxt.top

[R67] 生成随机十六进制串
来源：http://sea.cheryme.top

openssl rand -hex 16
来源：http://mkl.chenjidiqi.icu

[R68] 计算文件校验值
来源：http://wdi.daxiang520.top

sha256sum a.txt;  md5sum a.txt
来源：http://uhg.haohaochexian.top

[R69] 生成随机密码
来源：http://zgx.haohaochexian.top

head -c 16 /dev/urandom | base64
来源：http://xrx.daxiang520.top

[R70] 时间戳与互转
来源：http://gwf.yj202588.top

date +%s;  date -d @1700000000
来源：http://nuc.zhaomingkeji.xyz

[R71] 日期格式化
来源：http://aej.iojbl.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://pnk.hywenlv.cn

[R72] 等待端口就绪
来源：http://btd.ehwqpu.com

until nc -z localhost 3306; do sleep 1; done
来源：http://nvf.havefunace.top

[R73] 分割大日志
来源：http://zmk.zdqjudy.top

split -l 1000 big.log part_
来源：http://rgy.yongpay.top

[R74] 批量重命名
来源：http://gje.shangyingyoupin.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vua.ydjk.org.cn

[R75] 导出环境变量
来源：http://lul.aibaodan.cn

export PATH="$HOME/bin:$PATH"
来源：http://loc.ehwqpu.com

[R76] 使用临时文件
来源：http://hyy.birdmap.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ajh.xylfe.cn

[R77] 读取用户输入
来源：http://ndg.jinyuanbaomall.cn

read -rp "请输入: " ans
来源：http://spn.vehdjk.com

[R78] 交互式菜单
来源：http://pho.shanyushiyangtech.top

select opt in a b c; do echo "$opt"; break; done
来源：http://vqu.gaohongyu789.top

[R79] 解析命令行选项
来源：http://wxr.zdqjudy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uuh.wangshuangyany.cn

[R80] 查看脚本执行耗时
来源：http://hfo.c1oappe.top

time ./run.sh
来源：http://sge.havefunace.top

================================================================================
来源：http://etf.shanyushiyangkeji.top

S. C / C++ 专题
来源：http://mlq.yueranfly.top

================================================================================
来源：http://mau.daria6918.cn

[S01] C：Hello World
来源：http://uji.shuidangran.top

#include <stdio.h>
来源：http://jpo.xuanzx.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://vug.wangshuangyany.cn

[S02] C：变量与格式化输出
来源：http://clu.zhixingplan.top

int a = 10; printf("%d\n", a);
来源：http://sue.gotoacloud.top

[S03] C：读入整数
来源：http://ttq.pycfn.com

int x; scanf("%d", &x);
来源：http://pxc.zdqjudy.top

[S04] C：字符串复制
来源：http://iza.yongpay.top

char dst[32]; strcpy(dst, "hi");
来源：http://bms.gaohongyu789.top

[S05] C：字符串长度
来源：http://gng.sxryk.cn

strlen(s)
来源：http://yuj.zhixingplan.top

[S06] C：字符串比较
来源：http://ljq.ydjk.org.cn

strcmp(a, b) == 0
来源：http://xko.smart0.xyz

[S07] C：数组遍历求和
来源：http://xrj.xinyue.icu

for (int i = 0; i < n; i++) sum += a[i];
来源：http://grh.kuanghao11.cn

[S08] C：动态内存分配与释放
来源：http://mkw.shangyingyoupin.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lvw.sysykeji.top

[S09] C：结构体定义与初始化
来源：http://vyr.xuanzx.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wnr.xziqi.cn

[S10] C：指针与解引用
来源：http://ywt.ehwqpu.com

int *p = &a;  *p = 5;
来源：http://rzc.pycfn.com

[S11] C：逐行读文件
来源：http://yml.meibo888.top

FILE *f = fopen("a.txt", "r");
来源：http://ymq.hysaishi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gyg.chenzaomai.com

fclose(f);
来源：http://ara.vqdsnc.cn

[S12] C：写文件
来源：http://jas.pycfn.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bjx.smart0.xyz

[S13] C：宏定义
来源：http://ogj.sxryk.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dpj.9152youxi.cn

[S14] C：枚举
来源：http://rvc.shanyushiyangkeji.top

enum Color { RED, GREEN, BLUE };
来源：http://tge.hysaishi.cn

[S15] C：类型转换
来源：http://rpm.redwolf501.top

(double) a / b
来源：http://qdm.hcnkem.com

[S16] C：位操作置位
来源：http://gqt.daxiang520.top

x |= (1 << 3);
来源：http://eda.hnxiangtu.top

[S17] C：安全拼接字符串
来源：http://pgb.zdbjq.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://std.jiagoushi.top

[S18] C：命令行参数
来源：http://tpd.9152youxi.cn

int main(int argc, char **argv)
来源：http://qvv.wangshuangyany.cn

[S19] C：快速排序
来源：http://psg.chenlongwang.top

qsort(a, n, sizeof(int), cmp);
来源：http://rar.bbcook.cn

[S20] C：二分查找
来源：http://ndm.fehbvm.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pao.shangyingyoupin.top

[S21] C：字符类别判断
来源：http://dqa.nanxinkj.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://exb.fzhhl.top

[S22] C：字符串转数字
来源：http://sws.daxiang520.top

atoi("42");  strtod("3.14", NULL);
来源：http://fow.sufxvd.cn

[S23] C：随机数
来源：http://cpj.zhijiandao.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://boy.0kj1m.cn

[S24] C：获取本地时间
来源：http://yld.zycfv.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yld.cdnleiting.top

[S25] C：内存拷贝
来源：http://pgm.shanyushiyangtech.top

memcpy(dst, src, n);
来源：http://hfg.chenlongwang.top

[S26] C：内存清零
来源：http://unm.fengsongda.top

memset(a, 0, sizeof a);
来源：http://qee.aizwys.cn

[S27] C：定义常量
来源：http://fzp.gogol.net.cn

const double PI = 3.14159;
来源：http://oas.sufxvd.cn

[S28] C：静态变量
来源：http://cya.xuanzx.com

static int counter = 0;
来源：http://gpv.fanxiaobao.xyz

[S29] C：变参函数
来源：http://vcn.xuanzx.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nqa.cqqwz.cn

[S30] C：头文件保护
来源：http://vmq.jiagoushi.top

#ifndef X_H
来源：http://joj.shanyushiyangkeji.top

#define X_H
来源：http://aiu.wangdashe.top

#endif
来源：http://xrj.kuanghao11.cn

[S31] C++：Hello World
来源：http://bgu.iojbl.cn

#include <iostream>
来源：http://bfk.sufxvd.cn

int main() { std::cout << "Hello\n"; }
来源：http://luy.bbcook.cn

[S32] C++：字符串
来源：http://cnu.hysaishi.cn

std::string s = "hi";  s += "!";
来源：http://unw.yuanzhike.top

[S33] C++：vector 增删
来源：http://wis.xuanzx.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qhq.shanyushiyangkeji.top

[S34] C++：遍历 vector
来源：http://rjj.xingfuxueyuan.xyz

for (auto &x : v) { std::cout << x; }
来源：http://zsc.tianlin.xyz

[S35] C++：map
来源：http://mud.dashuyun.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://utr.mhx1999.top

[S36] C++：unordered_map
来源：http://wqo.chenlongwang.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xsw.ydjk.org.cn

[S37] C++：set
来源：http://rml.ehwqpu.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://atb.bjfxy.top

[S38] C++：排序
来源：http://gwl.cashguo.top

std::sort(v.begin(), v.end());
来源：http://sww.daxiang520.top

[S39] C++：自定义比较器排序
来源：http://wsg.hnqzz.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ive.chenzaomai.com

[S40] C++：查找元素
来源：http://fzu.fanxiaobao.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lug.ctjpmb.com

[S41] C++：类与构造函数
来源：http://mye.jianghu66.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vac.c1oappe.top

[S42] C++：继承与虚函数
来源：http://cql.fktsv.cn

class B : public Base { public: void f() override {} };
来源：http://xgm.zhoulong.xyz

[S43] C++：智能指针
来源：http://mkf.tarul.cn

auto p = std::make_unique<int>(5);
来源：http://fls.vehdjk.com

[S44] C++：引用传参
来源：http://rap.fzhhl.top

void inc(int &x) { ++x; }
来源：http://rop.xuetiantiany.cn

[S45] C++：lambda
来源：http://hdc.tanke756.top

auto add = [](int a, int b) { return a + b; };
来源：http://hbq.cqqwz.cn

[S46] C++：函数模板
来源：http://iwa.shangyingyoupin.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xcw.jiagoushi.top

[S47] C++：结构化绑定遍历
来源：http://ffo.cashguo.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xvg.wangshuangyany.cn

[S48] C++：逐行读文件
来源：http://ser.mhx1999.top

std::ifstream in("a.txt");  std::string line;
来源：http://qnn.nanxinkj.top

while (std::getline(in, line)) { }
来源：http://znz.haohaochexian.top

[S49] C++：写文件
来源：http://kar.fehbvm.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kmv.zhoulong.xyz

[S50] C++：格式化数字
来源：http://nyq.cucudq.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mvx.ppjwa.cn

[S51] C++：显式类型转换
来源：http://egb.redwolf501.top

static_cast<double>(a) / b
来源：http://vys.hywenlv.cn

[S52] C++：const 与 noexcept
来源：http://zcr.jlsjyb.cn

int size() const noexcept { return n_; }
来源：http://xev.gaohongyu789.top

[S53] C++：移动语义
来源：http://vog.ydjk.org.cn

std::vector<int> w = std::move(v);
来源：http://bfw.hongshengwenyu.top

[S54] C++：异常处理
来源：http://fyc.havefunace.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nku.jinqigfzy.top

[S55] C++：结构化绑定
来源：http://ejg.hesvh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zrc.uphjek.com

[S56] C++：optional
来源：http://egh.cqqwz.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://szm.daria6918.cn

[S57] C++：编译期常量
来源：http://xon.yvedp.cn

constexpr int N = 10;
来源：http://spz.ivvv.top

[S58] C++：命名空间
来源：http://tqg.shanyushiyangkeji.top

namespace ns { int f() { return 1; } }
来源：http://dkd.vqdsnc.cn

[S59] C++：静态断言
来源：http://wmg.sjlbkw.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://iht.fktsv.cn

[S60] C++：遍历并删除元素
来源：http://det.0kj1m.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bte.zycfv.cn

================================================================================
来源：http://dtq.hnxiangtu.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ogx.hfpthk.cn

================================================================================
来源：http://orx.hammf.cn

[T01] Kotlin：Hello World
来源：http://jxy.ctjpmb.com

println("Hello")
来源：http://ynt.gogol.net.cn

[T02] Kotlin：变量
来源：http://aun.sysykeji.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yub.hcnkem.com

[T03] Kotlin：字符串模板
来源：http://ljm.epnwcf.com

"值: $b"
来源：http://jxs.xinyue.icu

[T04] Kotlin：空安全
来源：http://ene.gaohongyu789.top

val n: String? = null;  n?.length
来源：http://zyh.ivvv.top

[T05] Kotlin：when 表达式
来源：http://okr.ywan-chungtsiang.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://idu.zdbjq.cn

[T06] Kotlin：集合映射
来源：http://uvq.cheryme.top

listOf(1, 2, 3).map { it * 2 }
来源：http://tgt.fanxiaobao.xyz

[T07] Kotlin：集合过滤
来源：http://fqk.smart0.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://tnf.aizwys.cn

[T08] Kotlin：数据类
来源：http://nwp.haohaochexian.top

data class User(val name: String, val age: Int)
来源：http://nuf.yj202588.top

[T09] Kotlin：扩展函数
来源：http://ytv.sxryk.cn

fun String.exclaim() = this + "!"
来源：http://yis.yanxiufei.cn

[T10] Kotlin：默认参数
来源：http://lcr.ivvv.top

fun greet(name: String = "World") = "Hi $name"
来源：http://cwe.zhengqikj.top

[T11] Kotlin：协程
来源：http://lhy.dianchejie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ixe.yonumen.top

[T12] Kotlin：解构声明
来源：http://jmv.ydzc1.top

val (a, b) = Pair(1, 2)
来源：http://lfk.nwbrower.top

[T13] Kotlin：只读 Map
来源：http://ecc.chenzaomai.com

val m = mapOf("a" to 1)
来源：http://ddc.sysykeji.top

[T14] Kotlin：循环
来源：http://cxz.shanyushiyangkeji.top

for (i in 1..10) println(i)
来源：http://xlu.hywenlv.cn

[T15] Kotlin：接口
来源：http://kpc.shuidangran.top

interface Shape { fun area(): Double }
来源：http://vyt.xziqi.cn

[T16] Swift：Hello World
来源：http://tts.fzhhl.top

print("Hello")
来源：http://xvw.gotoacloud.top

[T17] Swift：变量与常量
来源：http://wkz.nanxinkj.top

var a = 1;  let b = 2
来源：http://czb.tianlin.xyz

[T18] Swift：字符串插值
来源：http://bui.9152youxi.cn

"值: \(b)"
来源：http://doy.sjlbkw.cn

[T19] Swift：可选绑定
来源：http://olu.nanxuanxn.top

if let n = opt { print(n) }
来源：http://coc.ybcxt.top

[T20] Swift：数组操作
来源：http://vch.nanxinkj.top

var a = [1, 2, 3];  a.append(4)
来源：http://idm.sjlbkw.cn

[T21] Swift：遍历
来源：http://nvn.yuanzhike.top

for x in a { print(x) }
来源：http://mhw.shuidangran.top

[T22] Swift：字典
来源：http://zmv.cashguo.top

var d = ["a": 1];  d["b"] = 2
来源：http://nyi.zhoulong.xyz

[T23] Swift：函数
来源：http://fjt.hysaishi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://apq.shzxlz.cn

[T24] Swift：闭包
来源：http://kcq.zhongyouzk.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://bfv.cucudq.cn

[T25] Swift：结构体
来源：http://uqe.jianghu66.top

struct P { var x: Int }
来源：http://gjf.shanyushiyangtech.top

[T26] Swift：类与重写
来源：http://rgk.yfazqb.com

class A: Base { override func f() {} }
来源：http://qiz.xuanzx.com

[T27] Swift：错误处理
来源：http://laz.guannengcc.top

do { try f() } catch { print(error) }
来源：http://ien.nanxuanxn.top

[T28] Swift：枚举
来源：http://rbd.sweek.top

enum Color { case red, green }
来源：http://oag.sysykeji.top

[T29] Swift：guard 提前返回
来源：http://ntx.chenzaomai.com

guard let x = opt else { return }
来源：http://evk.c1oappe.top

[T30] Swift：协议
来源：http://cvo.jlsjyb.cn

protocol Shape { func area() -> Double }
来源：http://gge.nwbrower.top

[T31] Lua：Hello World
来源：http://cqg.zhoulong.xyz

print("Hello")
来源：http://ykf.epnwcf.com

[T32] Lua：局部变量
来源：http://uow.yongpay.top

local a = 1
来源：http://hue.birdmap.top

[T33] Lua：表（数组）
来源：http://ejj.feifeiyinyue.top

local t = {1, 2, 3};  t[4] = 4
来源：http://kfq.birdmap.top

[T34] Lua：遍历表
来源：http://uhv.aizwys.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://fsi.iojbl.cn

[T35] Lua：字典表
来源：http://ekt.tanke756.top

local d = { a = 1 };  d.b = 2
来源：http://yqh.shanyushiyangkeji.top

[T36] Lua：函数
来源：http://fjh.nanxinkj.top

function add(a, b) return a + b end
来源：http://cft.yonumen.top

[T37] Lua：字符串拼接
来源：http://uzy.dashuyun.cn

"a" .. "b"
来源：http://agz.guowangkeji.top

[T38] Lua：条件
来源：http://jtx.gzhubu.top

if x > 0 then print("正") end
来源：http://swl.zhiwuduotai.top

[T39] Lua：模式匹配
来源：http://mmv.chenlongwang.top

string.find(s, "%d+")
来源：http://xni.guowangkeji.top

[T40] Lua：元表
来源：http://yst.0kj1m.cn

setmetatable({}, { __index = base })
来源：http://ljn.tianlin.xyz

[T41] Perl：Hello World
来源：http://yff.jlsjyb.cn

print "Hello\n";
来源：http://hwt.ivvv.top

[T42] Perl：变量类型
来源：http://bwc.tanke756.top

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ghc.yj202588.top


<!-- 参考信息 -->