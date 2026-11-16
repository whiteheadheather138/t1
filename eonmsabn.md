代发 wailian999

files=$(ls -1)
来源：http://kvy.sysykeji.top

[R38] 管道串联
来源：http://glz.sjlbkw.cn

cat a.txt | grep -i error | wc -l
来源：http://jpf.ydjk.org.cn

[R39] 重定向标准输出与错误
来源：http://poh.meibo888.top

cmd > out.log 2>&1
来源：http://iub.zhijiandao.cn

[R40] 追加写日志
来源：http://hcy.jlsjyb.cn

echo "log" >> out.log
来源：http://ilm.sufxvd.cn

[R41] 丢弃输出
来源：http://wcw.hcnkem.com

cmd >/dev/null 2>&1
来源：http://koa.tarul.cn

[R42] 输入重定向
来源：http://dbf.hnqzz.top

wc -l < a.txt
来源：http://uwz.shanyushiyangkeji.top

[R43] 按名字查找文件
来源：http://kpn.cqqwz.cn

find . -name "*.log" -type f
来源：http://onc.yongpay.top

[R44] 按修改时间查找
来源：http://sgy.dashuyun.cn

find . -mtime -7 -type f
来源：http://vzu.tianlin.xyz

[R45] 批量删除
来源：http://bsp.hammf.cn

find . -name "*.tmp" -delete
来源：http://qfw.snrcjt.cn

[R46] 递归替换文件内容
来源：http://iwe.hnqzz.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tsv.sufxvd.cn

[R47] sed 单行替换
来源：http://tml.aibaodan.cn

sed -i 's/foo/bar/g' a.txt
来源：http://aow.gogol.net.cn

[R48] awk 取指定列
来源：http://ojd.yongpay.top

awk '{print $1, $3}' a.txt
来源：http://wma.fengsongda.top

[R49] awk 带条件
来源：http://ngm.gzhubu.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cmn.yj202588.top

[R50] awk 求和
来源：http://kpb.yuanzhike.top

awk '{s += $2} END {print s}' a.txt
来源：http://vws.shanyushiyangtech.top

[R51] 排序去重取前几
来源：http://wjw.redwolf501.top

sort a.txt | uniq -c | sort -rn | head
来源：http://qgc.hywenlv.cn

[R52] 统计行数
来源：http://obb.hnxiangtu.top

wc -l a.txt
来源：http://ihz.tanke756.top

[R53] 查看文件头与实时尾
来源：http://qoo.xziqi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://alj.jinqigufen.top

[R54] 比较两个文件
来源：http://vtp.vehdjk.com

diff a.txt b.txt
来源：http://srn.chenjidiqi.icu

[R55] 压缩与解压
来源：http://bcq.dashuyun.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tem.ppjwa.cn

[R56] 远程拷贝
来源：http://vbb.smart0.xyz

scp file user@host:/path/
来源：http://mtf.yanxiufei.cn

[R57] 远程执行命令
来源：http://dvb.fanxiaobao.xyz

ssh user@host 'uptime'
来源：http://bsa.hesvh.cn

[R58] 下载文件
来源：http://ktw.gogol.net.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gze.iojbl.cn

[R59] 发 POST JSON
来源：http://aes.cqqwz.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vvy.xylfe.cn

[R60] 只看 HTTP 状态码
来源：http://zxd.yfazqb.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yhz.fanxiaobao.xyz

[R61] 磁盘占用
来源：http://khp.gotoacloud.top

df -h;  du -sh *
来源：http://csu.shanyushiyangtech.top

[R62] 找最占空间的文件
来源：http://lkk.yangfankeji.com

du -ah . | sort -rh | head -10
来源：http://qwb.zdbjq.cn

[R63] 内存与进程
来源：http://kal.sysykeji.top

free -h;  ps aux | grep nginx
来源：http://afo.yuanzhike.top

[R64] 结束进程
来源：http://pmt.ydzc1.top

kill -9 $(pgrep -f app.py)
来源：http://lsr.wangshuangyany.cn

[R65] 查看端口占用
来源：http://ede.hnqzz.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://txl.quarkkingdee.top

[R66] 定时任务
来源：http://rym.zhijiandao.cn

crontab -e;  crontab -l
来源：http://qgf.shzxlz.cn

[R67] 生成随机十六进制串
来源：http://aqv.52xcode.cn

openssl rand -hex 16
来源：http://mmv.0kj1m.cn

[R68] 计算文件校验值
来源：http://vsj.fzhhl.top

sha256sum a.txt;  md5sum a.txt
来源：http://mpo.yfazqb.com

[R69] 生成随机密码
来源：http://atw.aibaodan.cn

head -c 16 /dev/urandom | base64
来源：http://seo.daria6918.cn

[R70] 时间戳与互转
来源：http://vgr.shuidangran.top

date +%s;  date -d @1700000000
来源：http://rmr.ydzc1.top

[R71] 日期格式化
来源：http://gny.yueranfly.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ckq.pycfn.com

[R72] 等待端口就绪
来源：http://qei.sxryk.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qps.yueranfly.top

[R73] 分割大日志
来源：http://nld.fktsv.cn

split -l 1000 big.log part_
来源：http://ekv.fengsongda.top

[R74] 批量重命名
来源：http://ost.havefunace.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kzf.chenzaomai.com

[R75] 导出环境变量
来源：http://lnf.xuanzx.com

export PATH="$HOME/bin:$PATH"
来源：http://tlm.jqgfzy.top

[R76] 使用临时文件
来源：http://oql.yj202588.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qwm.fengsongda.top

[R77] 读取用户输入
来源：http://vvi.hnxiangtu.top

read -rp "请输入: " ans
来源：http://gvj.yvedp.cn

[R78] 交互式菜单
来源：http://eme.guannengcc.top

select opt in a b c; do echo "$opt"; break; done
来源：http://igr.xuetiantiany.cn

[R79] 解析命令行选项
来源：http://mud.redwolf501.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kkn.meibo888.top

[R80] 查看脚本执行耗时
来源：http://fux.uphjek.com

time ./run.sh
来源：http://zzc.316326.xyz

================================================================================
来源：http://zlp.daxiang520.top

S. C / C++ 专题
来源：http://sqw.bjfxy.top

================================================================================
来源：http://gng.shuidangran.top

[S01] C：Hello World
来源：http://lhu.yfazqb.com

#include <stdio.h>
来源：http://fhe.sjlbkw.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://zep.guannengcc.top

[S02] C：变量与格式化输出
来源：http://gnl.aibaodan.cn

int a = 10; printf("%d\n", a);
来源：http://sdn.xziqi.cn

[S03] C：读入整数
来源：http://und.xuetiantiany.cn

int x; scanf("%d", &x);
来源：http://mgg.hfpthk.cn

[S04] C：字符串复制
来源：http://wkg.jlsjyb.cn

char dst[32]; strcpy(dst, "hi");
来源：http://qce.jlsjyb.cn

[S05] C：字符串长度
来源：http://vbd.hysaishi.cn

strlen(s)
来源：http://acq.daria6918.cn

[S06] C：字符串比较
来源：http://kjb.feifeiyinyue.top

strcmp(a, b) == 0
来源：http://jft.yj20258.top

[S07] C：数组遍历求和
来源：http://lez.uphjek.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gft.quarkkingdee.top

[S08] C：动态内存分配与释放
来源：http://wiy.yonumen.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dhl.chenzaomai.com

[S09] C：结构体定义与初始化
来源：http://mhz.cdnleiting.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vtx.pengpengdd.cyou

[S10] C：指针与解引用
来源：http://esr.pengpengdd.cyou

int *p = &a;  *p = 5;
来源：http://uly.cqqwz.cn

[S11] C：逐行读文件
来源：http://ewh.zhoulong.xyz

FILE *f = fopen("a.txt", "r");
来源：http://oao.jiagoushi.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://clf.tian-w.cn

fclose(f);
来源：http://ltb.tarul.cn

[S12] C：写文件
来源：http://fob.gogol.net.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cjr.fanxiaobao.xyz

[S13] C：宏定义
来源：http://qdd.meibo888.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dwv.yvedp.cn

[S14] C：枚举
来源：http://ekg.ctjpmb.com

enum Color { RED, GREEN, BLUE };
来源：http://nmu.zhaomingkeji.xyz

[S15] C：类型转换
来源：http://zpz.yj202588.top

(double) a / b
来源：http://fug.zdbjq.cn

[S16] C：位操作置位
来源：http://rzm.ivvv.top

x |= (1 << 3);
来源：http://xxo.feifeiyinyue.top

[S17] C：安全拼接字符串
来源：http://kdt.xuanzx.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mjh.nanxinkj.top

[S18] C：命令行参数
来源：http://zzz.daxiang520.top

int main(int argc, char **argv)
来源：http://crd.jlsjyb.cn

[S19] C：快速排序
来源：http://rmt.uphjek.com

qsort(a, n, sizeof(int), cmp);
来源：http://erm.xuetiantiany.cn

[S20] C：二分查找
来源：http://fes.nwbrower.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gxr.gaohongyu789.top

[S21] C：字符类别判断
来源：http://ilo.yfazqb.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ije.nanxinkj.top

[S22] C：字符串转数字
来源：http://qij.jqgufenzy.top

atoi("42");  strtod("3.14", NULL);
来源：http://hgb.havefunace.top

[S23] C：随机数
来源：http://dss.c1oappe.top

srand(time(NULL));  int r = rand() % 100;
来源：http://iok.chenzaomai.com

[S24] C：获取本地时间
来源：http://zra.ywan-chungtsiang.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qfp.tianlin.xyz

[S25] C：内存拷贝
来源：http://xvh.daria6918.cn

memcpy(dst, src, n);
来源：http://wcn.pengpengdd.cyou

[S26] C：内存清零
来源：http://zqe.andypj.xyz

memset(a, 0, sizeof a);
来源：http://hci.0kj1m.cn

[S27] C：定义常量
来源：http://pmh.feifeiyinyue.top

const double PI = 3.14159;
来源：http://sxh.yueranfly.top

[S28] C：静态变量
来源：http://grz.vqdsnc.cn

static int counter = 0;
来源：http://kxs.fktsv.cn

[S29] C：变参函数
来源：http://swp.zhiwuduotai.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tvt.jinghuilouyu.cn

[S30] C：头文件保护
来源：http://wkj.nanxinkj.top

#ifndef X_H
来源：http://mli.nwbrower.top

#define X_H
来源：http://cgq.sweek.top

#endif
来源：http://rnw.shanyushiyangkeji.top

[S31] C++：Hello World
来源：http://ord.ppjwa.cn

#include <iostream>
来源：http://wdu.chenjidiqi.icu

int main() { std::cout << "Hello\n"; }
来源：http://qkk.gogol.net.cn

[S32] C++：字符串
来源：http://pom.zhijiandao.cn

std::string s = "hi";  s += "!";
来源：http://aqu.jinqigufen.top

[S33] C++：vector 增删
来源：http://bkf.zhoulong.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://exd.ppjwa.cn

[S34] C++：遍历 vector
来源：http://eay.guowangkeji.top

for (auto &x : v) { std::cout << x; }
来源：http://chj.daxiang520.top

[S35] C++：map
来源：http://wda.gzhubu.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dht.ywan-chungtsiang.top

[S36] C++：unordered_map
来源：http://bdl.yangfankeji.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jae.hcnkem.com

[S37] C++：set
来源：http://nre.chenzaomai.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tpr.zdqjudy.top

[S38] C++：排序
来源：http://nyo.nwbrower.top

std::sort(v.begin(), v.end());
来源：http://dca.jinqigufen.top

[S39] C++：自定义比较器排序
来源：http://yht.yfazqb.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://idp.meibo888.top

[S40] C++：查找元素
来源：http://rgn.gotoacloud.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mwb.redwolf501.top

[S41] C++：类与构造函数
来源：http://ycf.ydzc1.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vyb.ydzc1.top

[S42] C++：继承与虚函数
来源：http://zln.vqdsnc.cn

class B : public Base { public: void f() override {} };
来源：http://ubb.bbcook.cn

[S43] C++：智能指针
来源：http://aip.vehdjk.com

auto p = std::make_unique<int>(5);
来源：http://syc.mhx1999.top

[S44] C++：引用传参
来源：http://fpm.nanxinkj.top

void inc(int &x) { ++x; }
来源：http://gun.shuidangran.top

[S45] C++：lambda
来源：http://lyi.gotoacloud.top

auto add = [](int a, int b) { return a + b; };
来源：http://jau.shuidangran.top

[S46] C++：函数模板
来源：http://dyf.shangyingyoupin.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://abx.zhixingplan.top

[S47] C++：结构化绑定遍历
来源：http://vle.snrcjt.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gvv.cucudq.cn

[S48] C++：逐行读文件
来源：http://dri.meibo888.top

std::ifstream in("a.txt");  std::string line;
来源：http://vlw.jiagoushi.top

while (std::getline(in, line)) { }
来源：http://dun.vehdjk.com

[S49] C++：写文件
来源：http://jqf.jqgufenzy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kdh.fanxiaobao.xyz

[S50] C++：格式化数字
来源：http://gpw.gotoacloud.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ryb.ppjwa.cn

[S51] C++：显式类型转换
来源：http://cia.zdqjudy.top

static_cast<double>(a) / b
来源：http://saj.chenlongwang.top

[S52] C++：const 与 noexcept
来源：http://tuk.shangyingyoupin.top

int size() const noexcept { return n_; }
来源：http://mvh.shanyushiyangtech.top

[S53] C++：移动语义
来源：http://yrf.yuanzhike.top

std::vector<int> w = std::move(v);
来源：http://obp.c1oappe.top

[S54] C++：异常处理
来源：http://fmy.zhaomingkeji.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dpw.316326.xyz

[S55] C++：结构化绑定
来源：http://hhs.guannengcc.top

auto [a, b] = std::make_pair(1, 2);
来源：http://omg.yj202588.top

[S56] C++：optional
来源：http://rxn.ywan-chungtsiang.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zrg.svipenyu.cn

[S57] C++：编译期常量
来源：http://jsc.snrcjt.cn

constexpr int N = 10;
来源：http://qsz.zhixingplan.top

[S58] C++：命名空间
来源：http://gwo.zhongyouzk.top

namespace ns { int f() { return 1; } }
来源：http://rdp.ybcxt.top

[S59] C++：静态断言
来源：http://xgg.dashuyun.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://omo.c1oappe.top

[S60] C++：遍历并删除元素
来源：http://qdl.ybcxt.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://eqk.xziqi.cn

================================================================================
来源：http://vai.cheryme.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jnb.jyoumei.cn

================================================================================
来源：http://qvy.52xcode.cn

[T01] Kotlin：Hello World
来源：http://lch.fzhhl.top

println("Hello")
来源：http://izc.xylfe.cn

[T02] Kotlin：变量
来源：http://fxt.yongpay.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yce.vehdjk.com

[T03] Kotlin：字符串模板
来源：http://nie.tian-w.cn

"值: $b"
来源：http://gxc.jlsjyb.cn

[T04] Kotlin：空安全
来源：http://lsr.shuidangran.top

val n: String? = null;  n?.length
来源：http://zgq.pengpengdd.cyou

[T05] Kotlin：when 表达式
来源：http://lfs.52xcode.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pjw.fehbvm.com

[T06] Kotlin：集合映射
来源：http://cwi.aizwys.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://vpa.xylfe.cn

[T07] Kotlin：集合过滤
来源：http://cnk.shuidangran.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://tfv.tanke756.top

[T08] Kotlin：数据类
来源：http://oob.nanxuanxn.top

data class User(val name: String, val age: Int)
来源：http://psn.xylfe.cn

[T09] Kotlin：扩展函数
来源：http://opz.yonumen.top

fun String.exclaim() = this + "!"
来源：http://ttt.guannengcc.top

[T10] Kotlin：默认参数
来源：http://bdg.gaohongyu789.top

fun greet(name: String = "World") = "Hi $name"
来源：http://okv.tanke756.top

[T11] Kotlin：协程
来源：http://weg.jqgfzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://boj.shanyushiyangkeji.top

[T12] Kotlin：解构声明
来源：http://hxz.sjlbkw.cn

val (a, b) = Pair(1, 2)
来源：http://jrt.hongshengwenyu.top

[T13] Kotlin：只读 Map
来源：http://teo.shanyushiyangtech.top

val m = mapOf("a" to 1)
来源：http://vgg.snrcjt.cn

[T14] Kotlin：循环
来源：http://clt.uphjek.com

for (i in 1..10) println(i)
来源：http://ghn.ybcxt.top

[T15] Kotlin：接口
来源：http://wpo.haohaochexian.top

interface Shape { fun area(): Double }
来源：http://tcv.jinqigufen.top

[T16] Swift：Hello World
来源：http://mbj.jiagoushi.top

print("Hello")
来源：http://oyk.svipenyu.cn

[T17] Swift：变量与常量
来源：http://aqe.ppjwa.cn

var a = 1;  let b = 2
来源：http://huk.yangfankeji.com

[T18] Swift：字符串插值
来源：http://occ.yanxiufei.cn

"值: \(b)"
来源：http://vqz.yangfankeji.com

[T19] Swift：可选绑定
来源：http://kkb.fengsongda.top

if let n = opt { print(n) }
来源：http://sun.andypj.xyz

[T20] Swift：数组操作
来源：http://qqw.hfpthk.cn

var a = [1, 2, 3];  a.append(4)
来源：http://efl.xingfuxueyuan.xyz

[T21] Swift：遍历
来源：http://zvk.yuxming.cn

for x in a { print(x) }
来源：http://gfo.zhongyouzk.top

[T22] Swift：字典
来源：http://scd.52xcode.cn

var d = ["a": 1];  d["b"] = 2
来源：http://aoc.xinyue.icu

[T23] Swift：函数
来源：http://tyj.pycfn.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sen.tarul.cn

[T24] Swift：闭包
来源：http://rgp.316326.xyz

let f = { (x: Int) -> Int in x * 2 }
来源：http://svp.zhengqikj.top

[T25] Swift：结构体
来源：http://pnw.snrcjt.cn

struct P { var x: Int }
来源：http://ods.hammf.cn

[T26] Swift：类与重写
来源：http://pty.zhixingplan.top

class A: Base { override func f() {} }
来源：http://hsw.birdmap.top

[T27] Swift：错误处理
来源：http://uei.jinyuanbaomall.cn

do { try f() } catch { print(error) }
来源：http://ihi.52xcode.cn

[T28] Swift：枚举
来源：http://azd.meibo888.top

enum Color { case red, green }
来源：http://vjz.jyoumei.cn

[T29] Swift：guard 提前返回
来源：http://xbk.hongshengwenyu.top

guard let x = opt else { return }
来源：http://xdp.svipenyu.cn

[T30] Swift：协议
来源：http://tqv.zycfv.cn

protocol Shape { func area() -> Double }
来源：http://hsy.yuanzhike.top

[T31] Lua：Hello World
来源：http://lce.yuanzhike.top

print("Hello")
来源：http://pok.wangshuangyany.cn

[T32] Lua：局部变量
来源：http://bij.yvedp.cn

local a = 1
来源：http://ncw.uphjek.com

[T33] Lua：表（数组）
来源：http://hhk.ybcxt.top

local t = {1, 2, 3};  t[4] = 4
来源：http://fks.hysaishi.cn

[T34] Lua：遍历表
来源：http://awp.yuxming.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zkm.redwolf501.top

[T35] Lua：字典表
来源：http://ers.jyoumei.cn

local d = { a = 1 };  d.b = 2
来源：http://pbc.wangshuangyany.cn

[T36] Lua：函数
来源：http://hiy.kuanghao11.cn

function add(a, b) return a + b end
来源：http://wen.quarkkingdee.top

[T37] Lua：字符串拼接
来源：http://gyz.epnwcf.com

"a" .. "b"
来源：http://qwz.tarul.cn

[T38] Lua：条件
来源：http://hla.gzhubu.top

if x > 0 then print("正") end
来源：http://kak.fktsv.cn

[T39] Lua：模式匹配
来源：http://byf.fengsongda.top

string.find(s, "%d+")
来源：http://ysc.jianghu66.top

[T40] Lua：元表
来源：http://nna.316326.xyz

setmetatable({}, { __index = base })
来源：http://efn.chenzaomai.com


<!-- 参考信息 -->