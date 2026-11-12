代发 wailian999

files=$(ls -1)
来源：http://ung.ctjpmb.com

[R38] 管道串联
来源：http://ewh.ctjpmb.com

cat a.txt | grep -i error | wc -l
来源：http://kxe.zhixingplan.top

[R39] 重定向标准输出与错误
来源：http://pkn.pengpengdd.cyou

cmd > out.log 2>&1
来源：http://pwb.yuanzhike.top

[R40] 追加写日志
来源：http://igg.yj202588.top

echo "log" >> out.log
来源：http://mbf.sufxvd.cn

[R41] 丢弃输出
来源：http://bdd.feifeiyinyue.top

cmd >/dev/null 2>&1
来源：http://fcr.sxryk.cn

[R42] 输入重定向
来源：http://mrb.hysaishi.cn

wc -l < a.txt
来源：http://ecp.cheryme.top

[R43] 按名字查找文件
来源：http://nrk.cashguo.top

find . -name "*.log" -type f
来源：http://bht.ybcxt.top

[R44] 按修改时间查找
来源：http://yoq.chenzaomai.com

find . -mtime -7 -type f
来源：http://bty.316326.xyz

[R45] 批量删除
来源：http://ddt.hfpthk.cn

find . -name "*.tmp" -delete
来源：http://pii.meibo888.top

[R46] 递归替换文件内容
来源：http://yeb.jiagoushi.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://luo.pycfn.com

[R47] sed 单行替换
来源：http://nxj.daria6918.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dng.chenzaomai.com

[R48] awk 取指定列
来源：http://vmq.gzhubu.top

awk '{print $1, $3}' a.txt
来源：http://gyq.zhixingplan.top

[R49] awk 带条件
来源：http://hnb.wangshuangyany.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ftq.52xcode.cn

[R50] awk 求和
来源：http://bhn.tarul.cn

awk '{s += $2} END {print s}' a.txt
来源：http://pku.nwbrower.top

[R51] 排序去重取前几
来源：http://vvk.jinghuilouyu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://wxu.hfpthk.cn

[R52] 统计行数
来源：http://eoy.cdnleiting.top

wc -l a.txt
来源：http://igy.birdmap.top

[R53] 查看文件头与实时尾
来源：http://swy.zhijiandao.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rqi.c1oappe.top

[R54] 比较两个文件
来源：http://maq.jiagoushi.top

diff a.txt b.txt
来源：http://pfq.fanxiaobao.xyz

[R55] 压缩与解压
来源：http://zdb.fzhhl.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xrv.birdmap.top

[R56] 远程拷贝
来源：http://lnq.yuanzhike.top

scp file user@host:/path/
来源：http://gbq.nwbrower.top

[R57] 远程执行命令
来源：http://tvk.vehdjk.com

ssh user@host 'uptime'
来源：http://zlp.yj202588.top

[R58] 下载文件
来源：http://jfj.yonumen.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zih.fehbvm.com

[R59] 发 POST JSON
来源：http://sau.fzhhl.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://emm.zycfv.cn

[R60] 只看 HTTP 状态码
来源：http://apt.feifeiyinyue.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://oly.zdqjudy.top

[R61] 磁盘占用
来源：http://lcz.ehwqpu.com

df -h;  du -sh *
来源：http://cqf.tanke756.top

[R62] 找最占空间的文件
来源：http://xma.jianghu66.top

du -ah . | sort -rh | head -10
来源：http://wvk.chenjidiqi.icu

[R63] 内存与进程
来源：http://ofl.bjfxy.top

free -h;  ps aux | grep nginx
来源：http://ypj.nwbrower.top

[R64] 结束进程
来源：http://wgi.cdnleiting.top

kill -9 $(pgrep -f app.py)
来源：http://ovl.yanxiufei.cn

[R65] 查看端口占用
来源：http://cdd.jlsjyb.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rik.fktsv.cn

[R66] 定时任务
来源：http://cwa.feifeiyinyue.top

crontab -e;  crontab -l
来源：http://pqv.yvedp.cn

[R67] 生成随机十六进制串
来源：http://fzb.pengpengdd.cyou

openssl rand -hex 16
来源：http://dzr.hywenlv.cn

[R68] 计算文件校验值
来源：http://igj.pycfn.com

sha256sum a.txt;  md5sum a.txt
来源：http://pxz.zdqjudy.top

[R69] 生成随机密码
来源：http://jpj.ydzc1.top

head -c 16 /dev/urandom | base64
来源：http://ezq.fehbvm.com

[R70] 时间戳与互转
来源：http://czu.ivvv.top

date +%s;  date -d @1700000000
来源：http://vxg.jlsjyb.cn

[R71] 日期格式化
来源：http://lax.jinghuilouyu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://hye.jqgfzy.top

[R72] 等待端口就绪
来源：http://olw.chenzaomai.com

until nc -z localhost 3306; do sleep 1; done
来源：http://nxq.chenzaomai.com

[R73] 分割大日志
来源：http://kmb.nwbrower.top

split -l 1000 big.log part_
来源：http://myu.fktsv.cn

[R74] 批量重命名
来源：http://cvh.xuetiantiany.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kif.hnqzz.top

[R75] 导出环境变量
来源：http://fvs.quarkkingdee.top

export PATH="$HOME/bin:$PATH"
来源：http://mbp.guowangkeji.top

[R76] 使用临时文件
来源：http://djg.jiagoushi.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://aqd.daria6918.cn

[R77] 读取用户输入
来源：http://apl.ywan-chungtsiang.top

read -rp "请输入: " ans
来源：http://zjw.jinyuanbaomall.cn

[R78] 交互式菜单
来源：http://dxq.hysaishi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zby.xuetiantiany.cn

[R79] 解析命令行选项
来源：http://tyd.hnqzz.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ysd.jyoumei.cn

[R80] 查看脚本执行耗时
来源：http://wim.jinyuanbaomall.cn

time ./run.sh
来源：http://car.jinghuilouyu.cn

================================================================================
来源：http://usq.hysaishi.cn

S. C / C++ 专题
来源：http://ysr.yonumen.top

================================================================================
来源：http://knp.sweek.top

[S01] C：Hello World
来源：http://bbu.redwolf501.top

#include <stdio.h>
来源：http://poc.feifeiyinyue.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://rqc.bbcook.cn

[S02] C：变量与格式化输出
来源：http://qda.hywenlv.cn

int a = 10; printf("%d\n", a);
来源：http://suc.kuanghao11.cn

[S03] C：读入整数
来源：http://aqx.shanyushiyangtech.top

int x; scanf("%d", &x);
来源：http://tsq.sufxvd.cn

[S04] C：字符串复制
来源：http://hsm.xziqi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://bpe.shangyingyoupin.top

[S05] C：字符串长度
来源：http://wer.zdbjq.cn

strlen(s)
来源：http://ejr.yj20258.top

[S06] C：字符串比较
来源：http://aaj.cashguo.top

strcmp(a, b) == 0
来源：http://yxp.jinyuanbaomall.cn

[S07] C：数组遍历求和
来源：http://ziq.gotoacloud.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xfb.0kj1m.cn

[S08] C：动态内存分配与释放
来源：http://fxm.gzhubu.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ump.mhx1999.top

[S09] C：结构体定义与初始化
来源：http://jzn.dashuyun.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fho.jinghuilouyu.cn

[S10] C：指针与解引用
来源：http://fvn.ppjwa.cn

int *p = &a;  *p = 5;
来源：http://cbd.kuanghao11.cn

[S11] C：逐行读文件
来源：http://tcp.fktsv.cn

FILE *f = fopen("a.txt", "r");
来源：http://uoi.dashuyun.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://occ.nanxinkj.top

fclose(f);
来源：http://ooc.nwbrower.top

[S12] C：写文件
来源：http://mvd.gzhubu.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cha.dianchejie.cn

[S13] C：宏定义
来源：http://xug.yj202588.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vyt.jinghuilouyu.cn

[S14] C：枚举
来源：http://mdn.nanxinkj.top

enum Color { RED, GREEN, BLUE };
来源：http://lgd.zhijiandao.cn

[S15] C：类型转换
来源：http://haf.gaohongyu789.top

(double) a / b
来源：http://pmt.yueranfly.top

[S16] C：位操作置位
来源：http://bsd.xingfuxueyuan.xyz

x |= (1 << 3);
来源：http://xpq.yuxming.cn

[S17] C：安全拼接字符串
来源：http://wgn.jyoumei.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ywg.jqgufenzy.top

[S18] C：命令行参数
来源：http://jae.shanyushiyangkeji.top

int main(int argc, char **argv)
来源：http://fsx.ydzc1.top

[S19] C：快速排序
来源：http://wce.c1oappe.top

qsort(a, n, sizeof(int), cmp);
来源：http://mvv.fehbvm.com

[S20] C：二分查找
来源：http://tsk.meibo888.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://frk.chenlongwang.top

[S21] C：字符类别判断
来源：http://wfn.nwbrower.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://chz.yonumen.top

[S22] C：字符串转数字
来源：http://mwh.ywan-chungtsiang.top

atoi("42");  strtod("3.14", NULL);
来源：http://qvj.yanxiufei.cn

[S23] C：随机数
来源：http://iai.shangyingyoupin.top

srand(time(NULL));  int r = rand() % 100;
来源：http://vbi.fengsongda.top

[S24] C：获取本地时间
来源：http://dzb.gogol.net.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mpq.xinyue.icu

[S25] C：内存拷贝
来源：http://imy.gogol.net.cn

memcpy(dst, src, n);
来源：http://ddh.gaohongyu789.top

[S26] C：内存清零
来源：http://bsx.ywan-chungtsiang.top

memset(a, 0, sizeof a);
来源：http://xtl.jlsjyb.cn

[S27] C：定义常量
来源：http://lot.shanyushiyangkeji.top

const double PI = 3.14159;
来源：http://jnw.aibaodan.cn

[S28] C：静态变量
来源：http://ejn.snrcjt.cn

static int counter = 0;
来源：http://inv.jinqigufen.top

[S29] C：变参函数
来源：http://ico.yj202588.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lug.zhongyouzk.top

[S30] C：头文件保护
来源：http://tge.cheryme.top

#ifndef X_H
来源：http://wiq.xingfuxueyuan.xyz

#define X_H
来源：http://jtc.xziqi.cn

#endif
来源：http://frn.jqgufenzy.top

[S31] C++：Hello World
来源：http://nhe.uphjek.com

#include <iostream>
来源：http://kyo.316326.xyz

int main() { std::cout << "Hello\n"; }
来源：http://vgy.smart0.xyz

[S32] C++：字符串
来源：http://fyg.bbcook.cn

std::string s = "hi";  s += "!";
来源：http://ugy.zhixingplan.top

[S33] C++：vector 增删
来源：http://maq.xuanzx.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bho.shanyushiyangkeji.top

[S34] C++：遍历 vector
来源：http://qli.jinyuanbaomall.cn

for (auto &x : v) { std::cout << x; }
来源：http://pig.tanke756.top

[S35] C++：map
来源：http://him.kuanghao11.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://oet.cucudq.cn

[S36] C++：unordered_map
来源：http://dgw.snrcjt.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yql.52xcode.cn

[S37] C++：set
来源：http://vqo.hnqzz.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gcz.ctjpmb.com

[S38] C++：排序
来源：http://kwz.yj202588.top

std::sort(v.begin(), v.end());
来源：http://qfi.chenlongwang.top

[S39] C++：自定义比较器排序
来源：http://ohp.haohaochexian.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cxe.sufxvd.cn

[S40] C++：查找元素
来源：http://rdn.shanyushiyangtech.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bct.hfpthk.cn

[S41] C++：类与构造函数
来源：http://pwb.hcnkem.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rfn.cheryme.top

[S42] C++：继承与虚函数
来源：http://fyh.nwbrower.top

class B : public Base { public: void f() override {} };
来源：http://nfi.fengsongda.top

[S43] C++：智能指针
来源：http://scv.52xcode.cn

auto p = std::make_unique<int>(5);
来源：http://tuk.svipenyu.cn

[S44] C++：引用传参
来源：http://gqz.svipenyu.cn

void inc(int &x) { ++x; }
来源：http://kjm.xuetiantiany.cn

[S45] C++：lambda
来源：http://whi.jinyuanbaomall.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xha.ppjwa.cn

[S46] C++：函数模板
来源：http://qac.yanxiufei.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yvm.fktsv.cn

[S47] C++：结构化绑定遍历
来源：http://jam.xylfe.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xsh.epnwcf.com

[S48] C++：逐行读文件
来源：http://ley.ydjk.org.cn

std::ifstream in("a.txt");  std::string line;
来源：http://key.hfpthk.cn

while (std::getline(in, line)) { }
来源：http://pha.zycfv.cn

[S49] C++：写文件
来源：http://sgd.xingfuxueyuan.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pam.aizwys.cn

[S50] C++：格式化数字
来源：http://gmy.dashuyun.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://izc.zhixingplan.top

[S51] C++：显式类型转换
来源：http://djr.xuetiantiany.cn

static_cast<double>(a) / b
来源：http://fia.hnxiangtu.top

[S52] C++：const 与 noexcept
来源：http://mnb.haohaochexian.top

int size() const noexcept { return n_; }
来源：http://yse.wangdashe.top

[S53] C++：移动语义
来源：http://dxh.jianghu66.top

std::vector<int> w = std::move(v);
来源：http://jpz.mhx1999.top

[S54] C++：异常处理
来源：http://uxp.sufxvd.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wdk.vehdjk.com

[S55] C++：结构化绑定
来源：http://zha.pycfn.com

auto [a, b] = std::make_pair(1, 2);
来源：http://rmt.yfazqb.com

[S56] C++：optional
来源：http://emr.hnqzz.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fne.yfazqb.com

[S57] C++：编译期常量
来源：http://lnr.nanxinkj.top

constexpr int N = 10;
来源：http://vnf.ppjwa.cn

[S58] C++：命名空间
来源：http://hnb.hysaishi.cn

namespace ns { int f() { return 1; } }
来源：http://scz.shanyushiyangtech.top

[S59] C++：静态断言
来源：http://for.cucudq.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://btz.ywan-chungtsiang.top

[S60] C++：遍历并删除元素
来源：http://shm.yongpay.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jgs.gotoacloud.top

================================================================================
来源：http://vxd.zdbjq.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rwe.haohaochexian.top

================================================================================
来源：http://xcq.meibo888.top

[T01] Kotlin：Hello World
来源：http://csk.fengsongda.top

println("Hello")
来源：http://gxq.zhengqikj.top

[T02] Kotlin：变量
来源：http://qod.yanxiufei.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nmb.jinqigufen.top

[T03] Kotlin：字符串模板
来源：http://sjk.yangfankeji.com

"值: $b"
来源：http://mup.yvedp.cn

[T04] Kotlin：空安全
来源：http://wbj.hongshengwenyu.top

val n: String? = null;  n?.length
来源：http://iqa.chenlongwang.top

[T05] Kotlin：when 表达式
来源：http://rlu.hysaishi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://smy.jiagoushi.top

[T06] Kotlin：集合映射
来源：http://owm.sufxvd.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://duy.cheryme.top

[T07] Kotlin：集合过滤
来源：http://dba.daxiang520.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://vap.jianghu66.top

[T08] Kotlin：数据类
来源：http://dwd.gogol.net.cn

data class User(val name: String, val age: Int)
来源：http://mye.cdnleiting.top

[T09] Kotlin：扩展函数
来源：http://vly.guannengcc.top

fun String.exclaim() = this + "!"
来源：http://bkq.cashguo.top

[T10] Kotlin：默认参数
来源：http://rwq.hnqzz.top

fun greet(name: String = "World") = "Hi $name"
来源：http://uhb.fzhhl.top

[T11] Kotlin：协程
来源：http://gqv.sxryk.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://cba.daria6918.cn

[T12] Kotlin：解构声明
来源：http://ioo.tanke756.top

val (a, b) = Pair(1, 2)
来源：http://fec.chenjidiqi.icu

[T13] Kotlin：只读 Map
来源：http://mhz.pengpengdd.cyou

val m = mapOf("a" to 1)
来源：http://huc.wangdashe.top

[T14] Kotlin：循环
来源：http://xeq.jqgfzy.top

for (i in 1..10) println(i)
来源：http://bjh.sufxvd.cn

[T15] Kotlin：接口
来源：http://ooy.smart0.xyz

interface Shape { fun area(): Double }
来源：http://htz.redwolf501.top

[T16] Swift：Hello World
来源：http://tst.yj20258888.top

print("Hello")
来源：http://oms.mhx1999.top

[T17] Swift：变量与常量
来源：http://jbl.jiagoushi.top

var a = 1;  let b = 2
来源：http://exw.shzxlz.cn

[T18] Swift：字符串插值
来源：http://phe.52xcode.cn

"值: \(b)"
来源：http://sal.9152youxi.cn

[T19] Swift：可选绑定
来源：http://hhz.sysykeji.top

if let n = opt { print(n) }
来源：http://oxs.zhiwuduotai.top

[T20] Swift：数组操作
来源：http://vmy.hcnkem.com

var a = [1, 2, 3];  a.append(4)
来源：http://mrs.zhoulong.xyz

[T21] Swift：遍历
来源：http://dad.svipenyu.cn

for x in a { print(x) }
来源：http://buq.yongpay.top

[T22] Swift：字典
来源：http://kex.hysaishi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://hwz.yfazqb.com

[T23] Swift：函数
来源：http://gyv.pengpengdd.cyou

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lca.feifeiyinyue.top

[T24] Swift：闭包
来源：http://try.kuanghao11.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://jrk.tarul.cn

[T25] Swift：结构体
来源：http://dkk.sweek.top

struct P { var x: Int }
来源：http://mck.zycfv.cn

[T26] Swift：类与重写
来源：http://qac.snrcjt.cn

class A: Base { override func f() {} }
来源：http://fbs.xuetiantiany.cn

[T27] Swift：错误处理
来源：http://wfe.jqgfzy.top

do { try f() } catch { print(error) }
来源：http://oif.daria6918.cn

[T28] Swift：枚举
来源：http://pvq.zhongyouzk.top

enum Color { case red, green }
来源：http://iap.hfpthk.cn

[T29] Swift：guard 提前返回
来源：http://zcp.uphjek.com

guard let x = opt else { return }
来源：http://vjo.316326.xyz

[T30] Swift：协议
来源：http://iir.jyoumei.cn

protocol Shape { func area() -> Double }
来源：http://ofb.dashuyun.cn

[T31] Lua：Hello World
来源：http://nry.havefunace.top

print("Hello")
来源：http://tkl.316326.xyz

[T32] Lua：局部变量
来源：http://hfl.epnwcf.com

local a = 1
来源：http://fbh.ybcxt.top

[T33] Lua：表（数组）
来源：http://qfy.sjlbkw.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://buz.quarkkingdee.top

[T34] Lua：遍历表
来源：http://vzy.zdqjudy.top

for i, v in ipairs(t) do print(i, v) end
来源：http://weu.xingfuxueyuan.xyz

[T35] Lua：字典表
来源：http://lhb.svipenyu.cn

local d = { a = 1 };  d.b = 2
来源：http://coz.quarkkingdee.top

[T36] Lua：函数
来源：http://eze.hfpthk.cn

function add(a, b) return a + b end
来源：http://krc.hnxiangtu.top

[T37] Lua：字符串拼接
来源：http://vpk.bjfxy.top

"a" .. "b"
来源：http://tft.vehdjk.com

[T38] Lua：条件
来源：http://ygn.sufxvd.cn

if x > 0 then print("正") end
来源：http://kos.meibo888.top

[T39] Lua：模式匹配
来源：http://jti.hfpthk.cn

string.find(s, "%d+")
来源：http://qjg.vehdjk.com

[T40] Lua：元表
来源：http://qaf.hongshengwenyu.top

setmetatable({}, { __index = base })
来源：http://oex.hfpthk.cn


<!-- 参考信息 -->