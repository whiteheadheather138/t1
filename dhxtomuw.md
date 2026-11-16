代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cbl.shangyingyoupin.top

[R30] 函数返回状态码
来源：http://brz.aibaodan.cn

f() { return 0; }; f || echo "失败了"
来源：http://unk.shuidangran.top

[R31] 局部变量
来源：http://vwy.tanke756.top

f() { local x=1; echo "$x"; }
来源：http://yfx.zdbjq.cn

[R32] 参数个数校验
来源：http://uyc.sysykeji.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wzw.jinqigufen.top

[R33] 捕获错误并提示行号
来源：http://rzs.zhixingplan.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yef.bbcook.cn

[R34] 退出时清理
来源：http://xqs.nanxuanxn.top

trap 'rm -f "$tmp"' EXIT
来源：http://trt.svipenyu.cn

[R35] 后台执行并等待
来源：http://smg.tianlin.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://heh.quarkkingdee.top

[R36] 并发执行多个任务
来源：http://yqj.yj20258.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lie.316326.xyz

[R37] 把输出赋给变量
来源：http://scq.9152youxi.cn

files=$(ls -1)
来源：http://tim.kuanghao11.cn

[R38] 管道串联
来源：http://mei.yanxiufei.cn

cat a.txt | grep -i error | wc -l
来源：http://fqj.chenzaomai.com

[R39] 重定向标准输出与错误
来源：http://cnv.daxiang520.top

cmd > out.log 2>&1
来源：http://sxn.0kj1m.cn

[R40] 追加写日志
来源：http://qoc.xylfe.cn

echo "log" >> out.log
来源：http://dvu.ppjwa.cn

[R41] 丢弃输出
来源：http://ebj.wangdashe.top

cmd >/dev/null 2>&1
来源：http://mnr.yj20258888.top

[R42] 输入重定向
来源：http://szh.shangyingyoupin.top

wc -l < a.txt
来源：http://pgw.birdmap.top

[R43] 按名字查找文件
来源：http://xeh.yangfankeji.com

find . -name "*.log" -type f
来源：http://grr.ydjk.org.cn

[R44] 按修改时间查找
来源：http://atf.gogol.net.cn

find . -mtime -7 -type f
来源：http://wru.nanxuanxn.top

[R45] 批量删除
来源：http://ycz.cucudq.cn

find . -name "*.tmp" -delete
来源：http://shv.jyoumei.cn

[R46] 递归替换文件内容
来源：http://gtn.ppjwa.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://anj.jinghuilouyu.cn

[R47] sed 单行替换
来源：http://zdi.jqgfzy.top

sed -i 's/foo/bar/g' a.txt
来源：http://dfv.xylfe.cn

[R48] awk 取指定列
来源：http://ydr.quarkkingdee.top

awk '{print $1, $3}' a.txt
来源：http://wrt.quarkkingdee.top

[R49] awk 带条件
来源：http://cep.ywan-chungtsiang.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ffr.wangshuangyany.cn

[R50] awk 求和
来源：http://hbv.redwolf501.top

awk '{s += $2} END {print s}' a.txt
来源：http://tbd.xuetiantiany.cn

[R51] 排序去重取前几
来源：http://lfj.jinyuanbaomall.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://uhd.tanke756.top

[R52] 统计行数
来源：http://rbj.chenzaomai.com

wc -l a.txt
来源：http://cgs.0kj1m.cn

[R53] 查看文件头与实时尾
来源：http://sxy.yuanzhike.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qqw.daxiang520.top

[R54] 比较两个文件
来源：http://bly.ehwqpu.com

diff a.txt b.txt
来源：http://dsp.jiagoushi.top

[R55] 压缩与解压
来源：http://hha.sxryk.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vuk.yangfankeji.com

[R56] 远程拷贝
来源：http://evz.yj202588.top

scp file user@host:/path/
来源：http://dlf.zycfv.cn

[R57] 远程执行命令
来源：http://ovw.aibaodan.cn

ssh user@host 'uptime'
来源：http://xth.zdbjq.cn

[R58] 下载文件
来源：http://edi.gzhubu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xtm.bbcook.cn

[R59] 发 POST JSON
来源：http://bur.tarul.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gml.mhx1999.top

[R60] 只看 HTTP 状态码
来源：http://swo.hysaishi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bul.zdqjudy.top

[R61] 磁盘占用
来源：http://ncr.jianghu66.top

df -h;  du -sh *
来源：http://xyp.nwbrower.top

[R62] 找最占空间的文件
来源：http://eic.chenlongwang.top

du -ah . | sort -rh | head -10
来源：http://xow.xuetiantiany.cn

[R63] 内存与进程
来源：http://cgg.quarkkingdee.top

free -h;  ps aux | grep nginx
来源：http://oxs.ctjpmb.com

[R64] 结束进程
来源：http://ize.chenzaomai.com

kill -9 $(pgrep -f app.py)
来源：http://blc.hongshengwenyu.top

[R65] 查看端口占用
来源：http://wwf.shanyushiyangtech.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ksp.epnwcf.com

[R66] 定时任务
来源：http://ojp.redwolf501.top

crontab -e;  crontab -l
来源：http://rjl.dashuyun.cn

[R67] 生成随机十六进制串
来源：http://ami.hywenlv.cn

openssl rand -hex 16
来源：http://oit.xingfuxueyuan.xyz

[R68] 计算文件校验值
来源：http://xmf.smart0.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://zzy.nanxinkj.top

[R69] 生成随机密码
来源：http://ckz.wangdashe.top

head -c 16 /dev/urandom | base64
来源：http://zhv.hfpthk.cn

[R70] 时间戳与互转
来源：http://jnk.fktsv.cn

date +%s;  date -d @1700000000
来源：http://ipk.nanxuanxn.top

[R71] 日期格式化
来源：http://dea.jinqigfzy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ngt.wangshuangyany.cn

[R72] 等待端口就绪
来源：http://jcf.yueranfly.top

until nc -z localhost 3306; do sleep 1; done
来源：http://bsa.uphjek.com

[R73] 分割大日志
来源：http://igc.gogol.net.cn

split -l 1000 big.log part_
来源：http://lve.zdqjudy.top

[R74] 批量重命名
来源：http://ykh.shanyushiyangtech.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://oil.gaohongyu789.top

[R75] 导出环境变量
来源：http://vxy.daxiang520.top

export PATH="$HOME/bin:$PATH"
来源：http://jps.zhiwuduotai.top

[R76] 使用临时文件
来源：http://dfh.sysykeji.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hcr.jinghuilouyu.cn

[R77] 读取用户输入
来源：http://xmw.yonumen.top

read -rp "请输入: " ans
来源：http://mly.jinyuanbaomall.cn

[R78] 交互式菜单
来源：http://vll.snrcjt.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://agh.shuidangran.top

[R79] 解析命令行选项
来源：http://qhu.ydzc1.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gct.hywenlv.cn

[R80] 查看脚本执行耗时
来源：http://vzj.tanke756.top

time ./run.sh
来源：http://tzj.tarul.cn

================================================================================
来源：http://gsu.sjlbkw.cn

S. C / C++ 专题
来源：http://grp.zhoulong.xyz

================================================================================
来源：http://ppz.chenzaomai.com

[S01] C：Hello World
来源：http://gjm.bbcook.cn

#include <stdio.h>
来源：http://scs.bbcook.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ooa.fehbvm.com

[S02] C：变量与格式化输出
来源：http://lqm.daria6918.cn

int a = 10; printf("%d\n", a);
来源：http://gpn.jinqigfzy.top

[S03] C：读入整数
来源：http://aem.xinyue.icu

int x; scanf("%d", &x);
来源：http://jkn.zhixingplan.top

[S04] C：字符串复制
来源：http://plt.meibo888.top

char dst[32]; strcpy(dst, "hi");
来源：http://uip.bjfxy.top

[S05] C：字符串长度
来源：http://xyv.316326.xyz

strlen(s)
来源：http://fev.meibo888.top

[S06] C：字符串比较
来源：http://tuv.fanxiaobao.xyz

strcmp(a, b) == 0
来源：http://qfp.cdnleiting.top

[S07] C：数组遍历求和
来源：http://uzy.jinghuilouyu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zkc.xinyue.icu

[S08] C：动态内存分配与释放
来源：http://xar.birdmap.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bxi.cucudq.cn

[S09] C：结构体定义与初始化
来源：http://zqq.hywenlv.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pgr.haohaochexian.top

[S10] C：指针与解引用
来源：http://uyd.hnxiangtu.top

int *p = &a;  *p = 5;
来源：http://shj.xuanzx.com

[S11] C：逐行读文件
来源：http://vij.redwolf501.top

FILE *f = fopen("a.txt", "r");
来源：http://ews.feifeiyinyue.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ply.bbcook.cn

fclose(f);
来源：http://nwh.hcnkem.com

[S12] C：写文件
来源：http://fzi.jinqigufen.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xys.daria6918.cn

[S13] C：宏定义
来源：http://drc.shanyushiyangkeji.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rfh.tian-w.cn

[S14] C：枚举
来源：http://nxl.yfazqb.com

enum Color { RED, GREEN, BLUE };
来源：http://kyp.dianchejie.cn

[S15] C：类型转换
来源：http://eur.chenjidiqi.icu

(double) a / b
来源：http://ntm.ehwqpu.com

[S16] C：位操作置位
来源：http://hyp.gogol.net.cn

x |= (1 << 3);
来源：http://chd.guowangkeji.top

[S17] C：安全拼接字符串
来源：http://lng.gogol.net.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kjf.pycfn.com

[S18] C：命令行参数
来源：http://xyr.yj20258.top

int main(int argc, char **argv)
来源：http://spk.ydzc1.top

[S19] C：快速排序
来源：http://gwl.yj202588.top

qsort(a, n, sizeof(int), cmp);
来源：http://bkn.meibo888.top

[S20] C：二分查找
来源：http://omo.hywenlv.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fkm.hcnkem.com

[S21] C：字符类别判断
来源：http://eyb.jinqigufen.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rwc.vqdsnc.cn

[S22] C：字符串转数字
来源：http://xbu.daria6918.cn

atoi("42");  strtod("3.14", NULL);
来源：http://dbe.nanxinkj.top

[S23] C：随机数
来源：http://xau.daria6918.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ggm.pycfn.com

[S24] C：获取本地时间
来源：http://xqs.sxryk.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ssl.svipenyu.cn

[S25] C：内存拷贝
来源：http://kkt.gzhubu.top

memcpy(dst, src, n);
来源：http://qoc.feifeiyinyue.top

[S26] C：内存清零
来源：http://iwf.chenlongwang.top

memset(a, 0, sizeof a);
来源：http://tgw.tanke756.top

[S27] C：定义常量
来源：http://gfd.xingfuxueyuan.xyz

const double PI = 3.14159;
来源：http://zya.zhongyouzk.top

[S28] C：静态变量
来源：http://azc.0kj1m.cn

static int counter = 0;
来源：http://eae.cdnleiting.top

[S29] C：变参函数
来源：http://bmn.zdbjq.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vro.zhoulong.xyz

[S30] C：头文件保护
来源：http://yqi.aibaodan.cn

#ifndef X_H
来源：http://zoo.tarul.cn

#define X_H
来源：http://uvh.pycfn.com

#endif
来源：http://cuz.hysaishi.cn

[S31] C++：Hello World
来源：http://saw.zycfv.cn

#include <iostream>
来源：http://chz.vqdsnc.cn

int main() { std::cout << "Hello\n"; }
来源：http://ljm.daria6918.cn

[S32] C++：字符串
来源：http://wkg.hysaishi.cn

std::string s = "hi";  s += "!";
来源：http://alz.hfpthk.cn

[S33] C++：vector 增删
来源：http://zaj.gaohongyu789.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://etw.hnqzz.top

[S34] C++：遍历 vector
来源：http://vbi.hnxiangtu.top

for (auto &x : v) { std::cout << x; }
来源：http://nsg.shuidangran.top

[S35] C++：map
来源：http://ghs.snrcjt.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wvn.sxryk.cn

[S36] C++：unordered_map
来源：http://fnu.shzxlz.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sjh.cdnleiting.top

[S37] C++：set
来源：http://sko.gaohongyu789.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lvh.svipenyu.cn

[S38] C++：排序
来源：http://vwh.xuetiantiany.cn

std::sort(v.begin(), v.end());
来源：http://gmk.xinyue.icu

[S39] C++：自定义比较器排序
来源：http://wpx.nwbrower.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vyr.wangshuangyany.cn

[S40] C++：查找元素
来源：http://gmk.andypj.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vbw.hnxiangtu.top

[S41] C++：类与构造函数
来源：http://uuu.quarkkingdee.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tqv.tanke756.top

[S42] C++：继承与虚函数
来源：http://vyb.shzxlz.cn

class B : public Base { public: void f() override {} };
来源：http://apx.meibo888.top

[S43] C++：智能指针
来源：http://inb.iojbl.cn

auto p = std::make_unique<int>(5);
来源：http://yqo.gotoacloud.top

[S44] C++：引用传参
来源：http://uru.hammf.cn

void inc(int &x) { ++x; }
来源：http://liu.sxryk.cn

[S45] C++：lambda
来源：http://inf.sufxvd.cn

auto add = [](int a, int b) { return a + b; };
来源：http://lvu.yongpay.top

[S46] C++：函数模板
来源：http://kgf.jinqigfzy.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zrc.guannengcc.top

[S47] C++：结构化绑定遍历
来源：http://wzq.jlsjyb.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kev.sjlbkw.cn

[S48] C++：逐行读文件
来源：http://oam.guowangkeji.top

std::ifstream in("a.txt");  std::string line;
来源：http://uvs.gaohongyu789.top

while (std::getline(in, line)) { }
来源：http://sxt.tianlin.xyz

[S49] C++：写文件
来源：http://wfh.vehdjk.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qty.xylfe.cn

[S50] C++：格式化数字
来源：http://yen.jianghu66.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zpo.jinyuanbaomall.cn

[S51] C++：显式类型转换
来源：http://rjs.svipenyu.cn

static_cast<double>(a) / b
来源：http://jmo.xinyue.icu

[S52] C++：const 与 noexcept
来源：http://ghl.yangfankeji.com

int size() const noexcept { return n_; }
来源：http://cfu.aibaodan.cn

[S53] C++：移动语义
来源：http://gjf.gzhubu.top

std::vector<int> w = std::move(v);
来源：http://dsy.jinghuilouyu.cn

[S54] C++：异常处理
来源：http://syn.jinghuilouyu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://eqw.fktsv.cn

[S55] C++：结构化绑定
来源：http://ags.shanyushiyangkeji.top

auto [a, b] = std::make_pair(1, 2);
来源：http://lti.yj20258.top

[S56] C++：optional
来源：http://met.aizwys.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://crj.havefunace.top

[S57] C++：编译期常量
来源：http://psf.daxiang520.top

constexpr int N = 10;
来源：http://yee.vqdsnc.cn

[S58] C++：命名空间
来源：http://kat.aibaodan.cn

namespace ns { int f() { return 1; } }
来源：http://boi.xuanzx.com

[S59] C++：静态断言
来源：http://wjr.svipenyu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mrk.hammf.cn

[S60] C++：遍历并删除元素
来源：http://cfq.meibo888.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://una.jqgufenzy.top

================================================================================
来源：http://rcj.pycfn.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vzz.vehdjk.com

================================================================================
来源：http://bsy.yuxming.cn

[T01] Kotlin：Hello World
来源：http://psl.chenzaomai.com

println("Hello")
来源：http://ldd.jianghu66.top

[T02] Kotlin：变量
来源：http://ujj.52xcode.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jdy.52xcode.cn

[T03] Kotlin：字符串模板
来源：http://wnb.uphjek.com

"值: $b"
来源：http://xrn.fehbvm.com

[T04] Kotlin：空安全
来源：http://hdv.nwbrower.top

val n: String? = null;  n?.length
来源：http://uqu.tian-w.cn

[T05] Kotlin：when 表达式
来源：http://uvp.uphjek.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://auo.sufxvd.cn

[T06] Kotlin：集合映射
来源：http://lsb.52xcode.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://seb.yfazqb.com

[T07] Kotlin：集合过滤
来源：http://huv.snrcjt.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://hyt.jqgfzy.top

[T08] Kotlin：数据类
来源：http://jjz.ctjpmb.com

data class User(val name: String, val age: Int)
来源：http://cay.yj20258888.top

[T09] Kotlin：扩展函数
来源：http://gsd.dashuyun.cn

fun String.exclaim() = this + "!"
来源：http://kjq.jinqigufen.top

[T10] Kotlin：默认参数
来源：http://ztb.cqqwz.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://fzz.c1oappe.top

[T11] Kotlin：协程
来源：http://gql.c1oappe.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ifn.ydjk.org.cn

[T12] Kotlin：解构声明
来源：http://oir.andypj.xyz

val (a, b) = Pair(1, 2)
来源：http://byp.tianlin.xyz

[T13] Kotlin：只读 Map
来源：http://zwn.ehwqpu.com

val m = mapOf("a" to 1)
来源：http://pgm.vehdjk.com

[T14] Kotlin：循环
来源：http://nod.daria6918.cn

for (i in 1..10) println(i)
来源：http://hog.jyoumei.cn

[T15] Kotlin：接口
来源：http://cya.guannengcc.top

interface Shape { fun area(): Double }
来源：http://zor.epnwcf.com

[T16] Swift：Hello World
来源：http://bcl.nwbrower.top

print("Hello")
来源：http://yps.fehbvm.com

[T17] Swift：变量与常量
来源：http://gsw.gzhubu.top

var a = 1;  let b = 2
来源：http://myb.birdmap.top

[T18] Swift：字符串插值
来源：http://mem.zhiwuduotai.top

"值: \(b)"
来源：http://ety.zdbjq.cn

[T19] Swift：可选绑定
来源：http://wui.havefunace.top

if let n = opt { print(n) }
来源：http://ute.yuxming.cn

[T20] Swift：数组操作
来源：http://gkr.jianghu66.top

var a = [1, 2, 3];  a.append(4)
来源：http://qij.xziqi.cn

[T21] Swift：遍历
来源：http://rti.tarul.cn

for x in a { print(x) }
来源：http://uyg.yvedp.cn

[T22] Swift：字典
来源：http://meb.9152youxi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://hxy.zhoulong.xyz

[T23] Swift：函数
来源：http://lho.ydjk.org.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://evd.yj20258.top

[T24] Swift：闭包
来源：http://orf.meibo888.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://vts.zhaomingkeji.xyz

[T25] Swift：结构体
来源：http://pui.guannengcc.top

struct P { var x: Int }
来源：http://kjp.fktsv.cn

[T26] Swift：类与重写
来源：http://bwg.316326.xyz

class A: Base { override func f() {} }
来源：http://dew.chenlongwang.top

[T27] Swift：错误处理
来源：http://nhe.hcnkem.com

do { try f() } catch { print(error) }
来源：http://xdz.zhoulong.xyz

[T28] Swift：枚举
来源：http://xon.ydjk.org.cn

enum Color { case red, green }
来源：http://gxp.yuanzhike.top

[T29] Swift：guard 提前返回
来源：http://vks.hcnkem.com

guard let x = opt else { return }
来源：http://zop.vqdsnc.cn

[T30] Swift：协议
来源：http://csc.shanyushiyangtech.top

protocol Shape { func area() -> Double }
来源：http://hdi.cashguo.top

[T31] Lua：Hello World
来源：http://fcg.xingfuxueyuan.xyz

print("Hello")
来源：http://xpp.hnxiangtu.top

[T32] Lua：局部变量
来源：http://gmq.yuanzhike.top

local a = 1
来源：http://wdc.fktsv.cn


<!-- 参考信息 -->