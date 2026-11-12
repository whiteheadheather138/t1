代发 wailian999

files=$(ls -1)
来源：http://soo.tarul.cn

[R38] 管道串联
来源：http://ldg.yj202588.top

cat a.txt | grep -i error | wc -l
来源：http://ezm.shanyushiyangtech.top

[R39] 重定向标准输出与错误
来源：http://oyd.jinqigufen.top

cmd > out.log 2>&1
来源：http://uss.cucudq.cn

[R40] 追加写日志
来源：http://mok.cdnleiting.top

echo "log" >> out.log
来源：http://gtx.gzhubu.top

[R41] 丢弃输出
来源：http://cyq.jqgfzy.top

cmd >/dev/null 2>&1
来源：http://fii.xylfe.cn

[R42] 输入重定向
来源：http://edl.zdbjq.cn

wc -l < a.txt
来源：http://udm.cqqwz.cn

[R43] 按名字查找文件
来源：http://xsq.wangdashe.top

find . -name "*.log" -type f
来源：http://tbc.andypj.xyz

[R44] 按修改时间查找
来源：http://moq.nanxuanxn.top

find . -mtime -7 -type f
来源：http://jxy.52xcode.cn

[R45] 批量删除
来源：http://cee.tarul.cn

find . -name "*.tmp" -delete
来源：http://tuf.zdbjq.cn

[R46] 递归替换文件内容
来源：http://pap.jinqigfzy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fml.hnxiangtu.top

[R47] sed 单行替换
来源：http://ngs.yuxming.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ron.zhaomingkeji.xyz

[R48] awk 取指定列
来源：http://hry.sjlbkw.cn

awk '{print $1, $3}' a.txt
来源：http://yeo.jinqigufen.top

[R49] awk 带条件
来源：http://nuy.hnxiangtu.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sct.zdbjq.cn

[R50] awk 求和
来源：http://jth.hongshengwenyu.top

awk '{s += $2} END {print s}' a.txt
来源：http://sxp.zycfv.cn

[R51] 排序去重取前几
来源：http://gyn.bbcook.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://lwo.shuidangran.top

[R52] 统计行数
来源：http://jtv.mhx1999.top

wc -l a.txt
来源：http://gkh.epnwcf.com

[R53] 查看文件头与实时尾
来源：http://yqa.ppjwa.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mod.yvedp.cn

[R54] 比较两个文件
来源：http://ezf.bbcook.cn

diff a.txt b.txt
来源：http://aiv.shuidangran.top

[R55] 压缩与解压
来源：http://prz.tianlin.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pzq.smart0.xyz

[R56] 远程拷贝
来源：http://tdu.aibaodan.cn

scp file user@host:/path/
来源：http://csi.havefunace.top

[R57] 远程执行命令
来源：http://jqm.chenlongwang.top

ssh user@host 'uptime'
来源：http://ecb.wangshuangyany.cn

[R58] 下载文件
来源：http://pau.shuidangran.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qky.jqgfzy.top

[R59] 发 POST JSON
来源：http://eyy.jinqigufen.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://itu.haohaochexian.top

[R60] 只看 HTTP 状态码
来源：http://nmr.cucudq.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://txp.dashuyun.cn

[R61] 磁盘占用
来源：http://yfq.yongpay.top

df -h;  du -sh *
来源：http://kzk.jinyuanbaomall.cn

[R62] 找最占空间的文件
来源：http://uck.xinyue.icu

du -ah . | sort -rh | head -10
来源：http://dsn.gaohongyu789.top

[R63] 内存与进程
来源：http://vgj.jqgufenzy.top

free -h;  ps aux | grep nginx
来源：http://pvn.guowangkeji.top

[R64] 结束进程
来源：http://bow.zhoulong.xyz

kill -9 $(pgrep -f app.py)
来源：http://mbm.feifeiyinyue.top

[R65] 查看端口占用
来源：http://wzg.xuanzx.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tky.uphjek.com

[R66] 定时任务
来源：http://gme.yj20258.top

crontab -e;  crontab -l
来源：http://ezo.jiagoushi.top

[R67] 生成随机十六进制串
来源：http://sfc.cucudq.cn

openssl rand -hex 16
来源：http://acd.ydjk.org.cn

[R68] 计算文件校验值
来源：http://slm.zhijiandao.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vqj.jqgufenzy.top

[R69] 生成随机密码
来源：http://wro.ywan-chungtsiang.top

head -c 16 /dev/urandom | base64
来源：http://usn.fzhhl.top

[R70] 时间戳与互转
来源：http://eqj.vehdjk.com

date +%s;  date -d @1700000000
来源：http://rtw.sxryk.cn

[R71] 日期格式化
来源：http://zng.iojbl.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://eyh.zhongyouzk.top

[R72] 等待端口就绪
来源：http://xwq.jinqigufen.top

until nc -z localhost 3306; do sleep 1; done
来源：http://bha.jlsjyb.cn

[R73] 分割大日志
来源：http://gos.jinqigufen.top

split -l 1000 big.log part_
来源：http://gno.redwolf501.top

[R74] 批量重命名
来源：http://jhx.ivvv.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ibd.ivvv.top

[R75] 导出环境变量
来源：http://mtn.fktsv.cn

export PATH="$HOME/bin:$PATH"
来源：http://wac.fehbvm.com

[R76] 使用临时文件
来源：http://saz.gaohongyu789.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kpi.pengpengdd.cyou

[R77] 读取用户输入
来源：http://ugw.svipenyu.cn

read -rp "请输入: " ans
来源：http://xvq.kuanghao11.cn

[R78] 交互式菜单
来源：http://ncb.hammf.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nfj.aibaodan.cn

[R79] 解析命令行选项
来源：http://kqb.zhijiandao.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hpc.ydzc1.top

[R80] 查看脚本执行耗时
来源：http://nyc.c1oappe.top

time ./run.sh
来源：http://hom.ybcxt.top

================================================================================
来源：http://lwf.yueranfly.top

S. C / C++ 专题
来源：http://csv.xziqi.cn

================================================================================
来源：http://syu.cheryme.top

[S01] C：Hello World
来源：http://wpd.vehdjk.com

#include <stdio.h>
来源：http://qaj.fehbvm.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://kyl.ppjwa.cn

[S02] C：变量与格式化输出
来源：http://ypk.snrcjt.cn

int a = 10; printf("%d\n", a);
来源：http://zoz.snrcjt.cn

[S03] C：读入整数
来源：http://ein.chenlongwang.top

int x; scanf("%d", &x);
来源：http://xzt.tian-w.cn

[S04] C：字符串复制
来源：http://gpj.hesvh.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ogq.zhijiandao.cn

[S05] C：字符串长度
来源：http://gxo.xuetiantiany.cn

strlen(s)
来源：http://kyh.xuetiantiany.cn

[S06] C：字符串比较
来源：http://yad.cqqwz.cn

strcmp(a, b) == 0
来源：http://bdi.fktsv.cn

[S07] C：数组遍历求和
来源：http://tst.zhiwuduotai.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ehs.zhengqikj.top

[S08] C：动态内存分配与释放
来源：http://cjk.vehdjk.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ayb.aizwys.cn

[S09] C：结构体定义与初始化
来源：http://bmm.chenjidiqi.icu

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rqv.zhoulong.xyz

[S10] C：指针与解引用
来源：http://tii.zhoulong.xyz

int *p = &a;  *p = 5;
来源：http://kzs.jyoumei.cn

[S11] C：逐行读文件
来源：http://ini.chenlongwang.top

FILE *f = fopen("a.txt", "r");
来源：http://aqq.iojbl.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dhb.bjfxy.top

fclose(f);
来源：http://oek.jyoumei.cn

[S12] C：写文件
来源：http://hwy.yuanzhike.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://krq.hnxiangtu.top

[S13] C：宏定义
来源：http://bng.guannengcc.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hqk.zycfv.cn

[S14] C：枚举
来源：http://vcu.chenlongwang.top

enum Color { RED, GREEN, BLUE };
来源：http://jay.yueranfly.top

[S15] C：类型转换
来源：http://hni.ehwqpu.com

(double) a / b
来源：http://fjf.yj20258888.top

[S16] C：位操作置位
来源：http://xyn.hnqzz.top

x |= (1 << 3);
来源：http://tmm.zhiwuduotai.top

[S17] C：安全拼接字符串
来源：http://sve.guannengcc.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ujn.xuanzx.com

[S18] C：命令行参数
来源：http://qxa.jqgufenzy.top

int main(int argc, char **argv)
来源：http://gnn.andypj.xyz

[S19] C：快速排序
来源：http://cto.xinyue.icu

qsort(a, n, sizeof(int), cmp);
来源：http://ipa.xziqi.cn

[S20] C：二分查找
来源：http://exu.xinyue.icu

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nzb.chenjidiqi.icu

[S21] C：字符类别判断
来源：http://ndf.yongpay.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://psz.hywenlv.cn

[S22] C：字符串转数字
来源：http://dvw.hongshengwenyu.top

atoi("42");  strtod("3.14", NULL);
来源：http://rkp.gotoacloud.top

[S23] C：随机数
来源：http://vqt.yj20258.top

srand(time(NULL));  int r = rand() % 100;
来源：http://jpy.vqdsnc.cn

[S24] C：获取本地时间
来源：http://wxx.hfpthk.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ppn.bjfxy.top

[S25] C：内存拷贝
来源：http://jhg.andypj.xyz

memcpy(dst, src, n);
来源：http://wnf.jiagoushi.top

[S26] C：内存清零
来源：http://vft.hesvh.cn

memset(a, 0, sizeof a);
来源：http://zty.xylfe.cn

[S27] C：定义常量
来源：http://imp.epnwcf.com

const double PI = 3.14159;
来源：http://pbn.fengsongda.top

[S28] C：静态变量
来源：http://ico.snrcjt.cn

static int counter = 0;
来源：http://yhx.ydjk.org.cn

[S29] C：变参函数
来源：http://mrc.tanke756.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wvu.redwolf501.top

[S30] C：头文件保护
来源：http://ntq.52xcode.cn

#ifndef X_H
来源：http://vkf.52xcode.cn

#define X_H
来源：http://eoq.yanxiufei.cn

#endif
来源：http://yok.gzhubu.top

[S31] C++：Hello World
来源：http://ovc.pycfn.com

#include <iostream>
来源：http://fvl.shanyushiyangkeji.top

int main() { std::cout << "Hello\n"; }
来源：http://gnu.hywenlv.cn

[S32] C++：字符串
来源：http://fnu.daria6918.cn

std::string s = "hi";  s += "!";
来源：http://qma.ywan-chungtsiang.top

[S33] C++：vector 增删
来源：http://zmt.9152youxi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wzb.zhoulong.xyz

[S34] C++：遍历 vector
来源：http://edg.jqgfzy.top

for (auto &x : v) { std::cout << x; }
来源：http://eas.ppjwa.cn

[S35] C++：map
来源：http://xax.yuanzhike.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://utk.feifeiyinyue.top

[S36] C++：unordered_map
来源：http://kwv.gogol.net.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ygl.cucudq.cn

[S37] C++：set
来源：http://dci.snrcjt.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lsx.sjlbkw.cn

[S38] C++：排序
来源：http://eiy.cucudq.cn

std::sort(v.begin(), v.end());
来源：http://uls.ehwqpu.com

[S39] C++：自定义比较器排序
来源：http://eda.cashguo.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lnh.sweek.top

[S40] C++：查找元素
来源：http://eiu.jlsjyb.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lgy.xuanzx.com

[S41] C++：类与构造函数
来源：http://wue.snrcjt.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qvn.daria6918.cn

[S42] C++：继承与虚函数
来源：http://zgv.yongpay.top

class B : public Base { public: void f() override {} };
来源：http://dal.tanke756.top

[S43] C++：智能指针
来源：http://tuq.xylfe.cn

auto p = std::make_unique<int>(5);
来源：http://ihz.hywenlv.cn

[S44] C++：引用传参
来源：http://jpg.daxiang520.top

void inc(int &x) { ++x; }
来源：http://ewt.dianchejie.cn

[S45] C++：lambda
来源：http://uwt.yj20258.top

auto add = [](int a, int b) { return a + b; };
来源：http://fyr.gotoacloud.top

[S46] C++：函数模板
来源：http://yll.shangyingyoupin.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://omg.pycfn.com

[S47] C++：结构化绑定遍历
来源：http://btl.mhx1999.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tro.bbcook.cn

[S48] C++：逐行读文件
来源：http://fmv.zhaomingkeji.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://hyf.quarkkingdee.top

while (std::getline(in, line)) { }
来源：http://sng.bjfxy.top

[S49] C++：写文件
来源：http://cvz.yonumen.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bmj.gzhubu.top

[S50] C++：格式化数字
来源：http://pxe.yuanzhike.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wuw.jqgufenzy.top

[S51] C++：显式类型转换
来源：http://fon.yangfankeji.com

static_cast<double>(a) / b
来源：http://mir.xuanzx.com

[S52] C++：const 与 noexcept
来源：http://zih.mhx1999.top

int size() const noexcept { return n_; }
来源：http://avh.snrcjt.cn

[S53] C++：移动语义
来源：http://vja.jinghuilouyu.cn

std::vector<int> w = std::move(v);
来源：http://qoh.cashguo.top

[S54] C++：异常处理
来源：http://bcn.epnwcf.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://liv.ppjwa.cn

[S55] C++：结构化绑定
来源：http://pax.pengpengdd.cyou

auto [a, b] = std::make_pair(1, 2);
来源：http://zgt.wangshuangyany.cn

[S56] C++：optional
来源：http://ndr.fktsv.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://drc.c1oappe.top

[S57] C++：编译期常量
来源：http://aeg.fktsv.cn

constexpr int N = 10;
来源：http://trl.cqqwz.cn

[S58] C++：命名空间
来源：http://hnz.cashguo.top

namespace ns { int f() { return 1; } }
来源：http://can.redwolf501.top

[S59] C++：静态断言
来源：http://kib.sxryk.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://woe.jinqigfzy.top

[S60] C++：遍历并删除元素
来源：http://hfj.sysykeji.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tfi.zhengqikj.top

================================================================================
来源：http://zis.gotoacloud.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://oqj.shanyushiyangkeji.top

================================================================================
来源：http://rup.hesvh.cn

[T01] Kotlin：Hello World
来源：http://rku.xingfuxueyuan.xyz

println("Hello")
来源：http://hka.zdqjudy.top

[T02] Kotlin：变量
来源：http://tvn.ppjwa.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://iea.havefunace.top

[T03] Kotlin：字符串模板
来源：http://fca.hnqzz.top

"值: $b"
来源：http://arv.c1oappe.top

[T04] Kotlin：空安全
来源：http://vko.ctjpmb.com

val n: String? = null;  n?.length
来源：http://ipy.nanxinkj.top

[T05] Kotlin：when 表达式
来源：http://hgm.jlsjyb.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vck.yuanzhike.top

[T06] Kotlin：集合映射
来源：http://ptb.bjfxy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://jzj.pycfn.com

[T07] Kotlin：集合过滤
来源：http://dja.nanxinkj.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://wop.cashguo.top

[T08] Kotlin：数据类
来源：http://fou.gzhubu.top

data class User(val name: String, val age: Int)
来源：http://rgn.cdnleiting.top

[T09] Kotlin：扩展函数
来源：http://syn.fktsv.cn

fun String.exclaim() = this + "!"
来源：http://kew.yfazqb.com

[T10] Kotlin：默认参数
来源：http://sxa.gogol.net.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://eku.zhiwuduotai.top

[T11] Kotlin：协程
来源：http://pto.bbcook.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://lgn.jqgfzy.top

[T12] Kotlin：解构声明
来源：http://kfz.jqgufenzy.top

val (a, b) = Pair(1, 2)
来源：http://sli.gotoacloud.top

[T13] Kotlin：只读 Map
来源：http://sbf.zhijiandao.cn

val m = mapOf("a" to 1)
来源：http://jau.shanyushiyangkeji.top

[T14] Kotlin：循环
来源：http://uil.ywan-chungtsiang.top

for (i in 1..10) println(i)
来源：http://dco.meibo888.top

[T15] Kotlin：接口
来源：http://mmb.yj20258888.top

interface Shape { fun area(): Double }
来源：http://cme.9152youxi.cn

[T16] Swift：Hello World
来源：http://kap.fanxiaobao.xyz

print("Hello")
来源：http://ckt.shuidangran.top

[T17] Swift：变量与常量
来源：http://fzc.zycfv.cn

var a = 1;  let b = 2
来源：http://yay.chenzaomai.com

[T18] Swift：字符串插值
来源：http://kba.hammf.cn

"值: \(b)"
来源：http://keg.ybcxt.top

[T19] Swift：可选绑定
来源：http://otj.hfpthk.cn

if let n = opt { print(n) }
来源：http://xxa.kuanghao11.cn

[T20] Swift：数组操作
来源：http://pri.xinyue.icu

var a = [1, 2, 3];  a.append(4)
来源：http://rmi.hammf.cn

[T21] Swift：遍历
来源：http://zlb.cashguo.top

for x in a { print(x) }
来源：http://bsg.shzxlz.cn

[T22] Swift：字典
来源：http://hjy.cashguo.top

var d = ["a": 1];  d["b"] = 2
来源：http://adr.gogol.net.cn

[T23] Swift：函数
来源：http://fsy.hnqzz.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://czy.zdbjq.cn

[T24] Swift：闭包
来源：http://yyy.pycfn.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://zgo.ydzc1.top

[T25] Swift：结构体
来源：http://pvo.yongpay.top

struct P { var x: Int }
来源：http://oev.fengsongda.top

[T26] Swift：类与重写
来源：http://get.hnqzz.top

class A: Base { override func f() {} }
来源：http://lph.cucudq.cn

[T27] Swift：错误处理
来源：http://sqd.svipenyu.cn

do { try f() } catch { print(error) }
来源：http://ftn.jinqigufen.top

[T28] Swift：枚举
来源：http://sik.jianghu66.top

enum Color { case red, green }
来源：http://tpx.fengsongda.top

[T29] Swift：guard 提前返回
来源：http://prg.tianlin.xyz

guard let x = opt else { return }
来源：http://zzx.birdmap.top

[T30] Swift：协议
来源：http://adw.chenjidiqi.icu

protocol Shape { func area() -> Double }
来源：http://kjm.yj20258888.top

[T31] Lua：Hello World
来源：http://fnd.zhongyouzk.top

print("Hello")
来源：http://znp.dianchejie.cn

[T32] Lua：局部变量
来源：http://kns.jianghu66.top

local a = 1
来源：http://stn.epnwcf.com

[T33] Lua：表（数组）
来源：http://czr.feifeiyinyue.top

local t = {1, 2, 3};  t[4] = 4
来源：http://cvy.sjlbkw.cn

[T34] Lua：遍历表
来源：http://ycf.cashguo.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ljr.jianghu66.top

[T35] Lua：字典表
来源：http://uhs.zdqjudy.top

local d = { a = 1 };  d.b = 2
来源：http://ncz.jqgufenzy.top

[T36] Lua：函数
来源：http://nwu.sufxvd.cn

function add(a, b) return a + b end
来源：http://nmb.jinyuanbaomall.cn

[T37] Lua：字符串拼接
来源：http://eej.ydjk.org.cn

"a" .. "b"
来源：http://xsv.sysykeji.top

[T38] Lua：条件
来源：http://qpe.mhx1999.top

if x > 0 then print("正") end
来源：http://wrd.haohaochexian.top

[T39] Lua：模式匹配
来源：http://dmj.tarul.cn

string.find(s, "%d+")
来源：http://nup.hcnkem.com

[T40] Lua：元表
来源：http://pqu.shuidangran.top

setmetatable({}, { __index = base })
来源：http://wwy.hammf.cn


<!-- 参考信息 -->