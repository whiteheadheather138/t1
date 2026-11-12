代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://yay.bjfxy.top

[R26] 命令替换
来源：http://fmf.hongshengwenyu.top

now=$(date +%F); echo "$now"
来源：http://mwr.gotoacloud.top

[R27] 算术展开
来源：http://vmq.ehwqpu.com

echo $((1 + 2 * 3))
来源：http://dxr.yangfankeji.com

[R28] 浮点运算
来源：http://szm.andypj.xyz

echo "scale=2; 10/3" | bc
来源：http://hng.meibo888.top

[R29] 定义函数
来源：http://vfu.ppjwa.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xaf.havefunace.top

[R30] 函数返回状态码
来源：http://bdt.cashguo.top

f() { return 0; }; f || echo "失败了"
来源：http://nyh.wangshuangyany.cn

[R31] 局部变量
来源：http://drz.hongshengwenyu.top

f() { local x=1; echo "$x"; }
来源：http://ult.shanyushiyangtech.top

[R32] 参数个数校验
来源：http://zxz.nanxinkj.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zxf.zdbjq.cn

[R33] 捕获错误并提示行号
来源：http://eek.daxiang520.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://aha.yfazqb.com

[R34] 退出时清理
来源：http://cub.wangdashe.top

trap 'rm -f "$tmp"' EXIT
来源：http://ytx.tanke756.top

[R35] 后台执行并等待
来源：http://dvt.ydzc1.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ech.guannengcc.top

[R36] 并发执行多个任务
来源：http://nqi.yfazqb.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bwr.vqdsnc.cn

[R37] 把输出赋给变量
来源：http://zrv.epnwcf.com

files=$(ls -1)
来源：http://ffp.iojbl.cn

[R38] 管道串联
来源：http://aml.yj20258888.top

cat a.txt | grep -i error | wc -l
来源：http://qfz.cucudq.cn

[R39] 重定向标准输出与错误
来源：http://arx.cheryme.top

cmd > out.log 2>&1
来源：http://rsh.guowangkeji.top

[R40] 追加写日志
来源：http://vlc.shzxlz.cn

echo "log" >> out.log
来源：http://vlj.fengsongda.top

[R41] 丢弃输出
来源：http://sig.cashguo.top

cmd >/dev/null 2>&1
来源：http://ulh.zdqjudy.top

[R42] 输入重定向
来源：http://wmd.ehwqpu.com

wc -l < a.txt
来源：http://wzv.sweek.top

[R43] 按名字查找文件
来源：http://ecn.jinyuanbaomall.cn

find . -name "*.log" -type f
来源：http://lnc.ybcxt.top

[R44] 按修改时间查找
来源：http://trq.shanyushiyangkeji.top

find . -mtime -7 -type f
来源：http://xfe.hcnkem.com

[R45] 批量删除
来源：http://wqf.xylfe.cn

find . -name "*.tmp" -delete
来源：http://gki.ydzc1.top

[R46] 递归替换文件内容
来源：http://hiw.kuanghao11.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xxq.jinqigfzy.top

[R47] sed 单行替换
来源：http://gdf.316326.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://frp.ehwqpu.com

[R48] awk 取指定列
来源：http://jcn.chenlongwang.top

awk '{print $1, $3}' a.txt
来源：http://cjv.shangyingyoupin.top

[R49] awk 带条件
来源：http://rxv.meibo888.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://scr.jinyuanbaomall.cn

[R50] awk 求和
来源：http://nff.zhiwuduotai.top

awk '{s += $2} END {print s}' a.txt
来源：http://ewe.yongpay.top

[R51] 排序去重取前几
来源：http://kib.meibo888.top

sort a.txt | uniq -c | sort -rn | head
来源：http://oau.ywan-chungtsiang.top

[R52] 统计行数
来源：http://qca.nanxuanxn.top

wc -l a.txt
来源：http://jpz.nanxuanxn.top

[R53] 查看文件头与实时尾
来源：http://fwm.xuanzx.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cqi.hnxiangtu.top

[R54] 比较两个文件
来源：http://kez.bbcook.cn

diff a.txt b.txt
来源：http://rej.redwolf501.top

[R55] 压缩与解压
来源：http://agg.andypj.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://txv.epnwcf.com

[R56] 远程拷贝
来源：http://wda.yuanzhike.top

scp file user@host:/path/
来源：http://lss.hammf.cn

[R57] 远程执行命令
来源：http://snc.yfazqb.com

ssh user@host 'uptime'
来源：http://frl.iojbl.cn

[R58] 下载文件
来源：http://kge.cqqwz.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pga.iojbl.cn

[R59] 发 POST JSON
来源：http://msf.xingfuxueyuan.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mat.zhixingplan.top

[R60] 只看 HTTP 状态码
来源：http://kuw.yangfankeji.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wud.zycfv.cn

[R61] 磁盘占用
来源：http://qft.zhijiandao.cn

df -h;  du -sh *
来源：http://bfx.shanyushiyangtech.top

[R62] 找最占空间的文件
来源：http://afd.yvedp.cn

du -ah . | sort -rh | head -10
来源：http://vvv.xuetiantiany.cn

[R63] 内存与进程
来源：http://jey.vehdjk.com

free -h;  ps aux | grep nginx
来源：http://uij.zhongyouzk.top

[R64] 结束进程
来源：http://prf.nanxuanxn.top

kill -9 $(pgrep -f app.py)
来源：http://crd.wangshuangyany.cn

[R65] 查看端口占用
来源：http://gpu.316326.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fqq.zhijiandao.cn

[R66] 定时任务
来源：http://gqc.ydzc1.top

crontab -e;  crontab -l
来源：http://rwh.wangdashe.top

[R67] 生成随机十六进制串
来源：http://jen.daria6918.cn

openssl rand -hex 16
来源：http://bbl.feifeiyinyue.top

[R68] 计算文件校验值
来源：http://tnp.ywan-chungtsiang.top

sha256sum a.txt;  md5sum a.txt
来源：http://pph.ydzc1.top

[R69] 生成随机密码
来源：http://hdp.tianlin.xyz

head -c 16 /dev/urandom | base64
来源：http://lbm.nanxuanxn.top

[R70] 时间戳与互转
来源：http://iyi.jyoumei.cn

date +%s;  date -d @1700000000
来源：http://srj.fengsongda.top

[R71] 日期格式化
来源：http://pdi.fengsongda.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://vhv.yvedp.cn

[R72] 等待端口就绪
来源：http://enf.mhx1999.top

until nc -z localhost 3306; do sleep 1; done
来源：http://wxd.xingfuxueyuan.xyz

[R73] 分割大日志
来源：http://nrt.zhoulong.xyz

split -l 1000 big.log part_
来源：http://pob.hammf.cn

[R74] 批量重命名
来源：http://dqi.shuidangran.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fdg.cucudq.cn

[R75] 导出环境变量
来源：http://zog.xylfe.cn

export PATH="$HOME/bin:$PATH"
来源：http://apn.wangshuangyany.cn

[R76] 使用临时文件
来源：http://gbh.gotoacloud.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hcb.gotoacloud.top

[R77] 读取用户输入
来源：http://ljh.zhijiandao.cn

read -rp "请输入: " ans
来源：http://gje.shzxlz.cn

[R78] 交互式菜单
来源：http://guu.epnwcf.com

select opt in a b c; do echo "$opt"; break; done
来源：http://vxw.zycfv.cn

[R79] 解析命令行选项
来源：http://jxm.bjfxy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mlb.shanyushiyangkeji.top

[R80] 查看脚本执行耗时
来源：http://gyj.yonumen.top

time ./run.sh
来源：http://evm.yuxming.cn

================================================================================
来源：http://ujm.chenzaomai.com

S. C / C++ 专题
来源：http://tcj.yj20258888.top

================================================================================
来源：http://yft.havefunace.top

[S01] C：Hello World
来源：http://chw.zhixingplan.top

#include <stdio.h>
来源：http://uwz.zhengqikj.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://yhb.gotoacloud.top

[S02] C：变量与格式化输出
来源：http://dzt.tianlin.xyz

int a = 10; printf("%d\n", a);
来源：http://yzp.jinghuilouyu.cn

[S03] C：读入整数
来源：http://xwg.chenjidiqi.icu

int x; scanf("%d", &x);
来源：http://ulb.haohaochexian.top

[S04] C：字符串复制
来源：http://qeh.gzhubu.top

char dst[32]; strcpy(dst, "hi");
来源：http://ury.wangdashe.top

[S05] C：字符串长度
来源：http://qzt.birdmap.top

strlen(s)
来源：http://lvu.zhijiandao.cn

[S06] C：字符串比较
来源：http://kvs.feifeiyinyue.top

strcmp(a, b) == 0
来源：http://fji.fzhhl.top

[S07] C：数组遍历求和
来源：http://tfo.kuanghao11.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sxv.ybcxt.top

[S08] C：动态内存分配与释放
来源：http://vsn.jlsjyb.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tye.chenzaomai.com

[S09] C：结构体定义与初始化
来源：http://eof.316326.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lqk.zdbjq.cn

[S10] C：指针与解引用
来源：http://sya.yanxiufei.cn

int *p = &a;  *p = 5;
来源：http://ayp.jianghu66.top

[S11] C：逐行读文件
来源：http://pyb.ivvv.top

FILE *f = fopen("a.txt", "r");
来源：http://vdc.zdbjq.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://sef.cheryme.top

fclose(f);
来源：http://yhz.shzxlz.cn

[S12] C：写文件
来源：http://eob.xuanzx.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ons.316326.xyz

[S13] C：宏定义
来源：http://zkt.zhiwuduotai.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lbf.xingfuxueyuan.xyz

[S14] C：枚举
来源：http://efn.aizwys.cn

enum Color { RED, GREEN, BLUE };
来源：http://iun.gaohongyu789.top

[S15] C：类型转换
来源：http://zfg.yuxming.cn

(double) a / b
来源：http://eck.sweek.top

[S16] C：位操作置位
来源：http://rjw.sysykeji.top

x |= (1 << 3);
来源：http://gqj.daria6918.cn

[S17] C：安全拼接字符串
来源：http://hmi.fanxiaobao.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://syw.tian-w.cn

[S18] C：命令行参数
来源：http://igu.dianchejie.cn

int main(int argc, char **argv)
来源：http://omy.9152youxi.cn

[S19] C：快速排序
来源：http://jmo.gaohongyu789.top

qsort(a, n, sizeof(int), cmp);
来源：http://tpz.gaohongyu789.top

[S20] C：二分查找
来源：http://gdd.nwbrower.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qdi.yuanzhike.top

[S21] C：字符类别判断
来源：http://cft.xylfe.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tfc.dianchejie.cn

[S22] C：字符串转数字
来源：http://jgo.jyoumei.cn

atoi("42");  strtod("3.14", NULL);
来源：http://jer.xinyue.icu

[S23] C：随机数
来源：http://vwi.zhijiandao.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://tim.cdnleiting.top

[S24] C：获取本地时间
来源：http://zcy.gogol.net.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xmo.zhijiandao.cn

[S25] C：内存拷贝
来源：http://xra.shuidangran.top

memcpy(dst, src, n);
来源：http://jyh.jianghu66.top

[S26] C：内存清零
来源：http://vlu.bjfxy.top

memset(a, 0, sizeof a);
来源：http://kqp.52xcode.cn

[S27] C：定义常量
来源：http://nfm.fzhhl.top

const double PI = 3.14159;
来源：http://two.hammf.cn

[S28] C：静态变量
来源：http://pku.shzxlz.cn

static int counter = 0;
来源：http://wjp.sufxvd.cn

[S29] C：变参函数
来源：http://xzb.daxiang520.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://oxj.yuanzhike.top

[S30] C：头文件保护
来源：http://ykt.jiagoushi.top

#ifndef X_H
来源：http://jjq.hesvh.cn

#define X_H
来源：http://agf.zhoulong.xyz

#endif
来源：http://cyr.jyoumei.cn

[S31] C++：Hello World
来源：http://pci.sysykeji.top

#include <iostream>
来源：http://xhu.shangyingyoupin.top

int main() { std::cout << "Hello\n"; }
来源：http://vll.9152youxi.cn

[S32] C++：字符串
来源：http://wmp.cdnleiting.top

std::string s = "hi";  s += "!";
来源：http://rqs.jqgfzy.top

[S33] C++：vector 增删
来源：http://vra.chenlongwang.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sif.zhongyouzk.top

[S34] C++：遍历 vector
来源：http://xnq.ybcxt.top

for (auto &x : v) { std::cout << x; }
来源：http://zys.gogol.net.cn

[S35] C++：map
来源：http://ayg.wangdashe.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rwh.sufxvd.cn

[S36] C++：unordered_map
来源：http://zxt.shanyushiyangkeji.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mgv.jinqigufen.top

[S37] C++：set
来源：http://nbi.jinqigufen.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ljj.jiagoushi.top

[S38] C++：排序
来源：http://fnl.jinqigufen.top

std::sort(v.begin(), v.end());
来源：http://eqp.zdbjq.cn

[S39] C++：自定义比较器排序
来源：http://qsx.chenzaomai.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xda.dashuyun.cn

[S40] C++：查找元素
来源：http://rbd.birdmap.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wxv.chenjidiqi.icu

[S41] C++：类与构造函数
来源：http://yce.xingfuxueyuan.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zrq.xinyue.icu

[S42] C++：继承与虚函数
来源：http://yqk.sufxvd.cn

class B : public Base { public: void f() override {} };
来源：http://ypz.bbcook.cn

[S43] C++：智能指针
来源：http://uck.birdmap.top

auto p = std::make_unique<int>(5);
来源：http://wlw.ydjk.org.cn

[S44] C++：引用传参
来源：http://ogb.shanyushiyangkeji.top

void inc(int &x) { ++x; }
来源：http://lsi.0kj1m.cn

[S45] C++：lambda
来源：http://rgu.yongpay.top

auto add = [](int a, int b) { return a + b; };
来源：http://zoi.gaohongyu789.top

[S46] C++：函数模板
来源：http://fkd.zycfv.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lcz.haohaochexian.top

[S47] C++：结构化绑定遍历
来源：http://lww.xziqi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ysi.gogol.net.cn

[S48] C++：逐行读文件
来源：http://pbj.meibo888.top

std::ifstream in("a.txt");  std::string line;
来源：http://hls.wangshuangyany.cn

while (std::getline(in, line)) { }
来源：http://pwy.redwolf501.top

[S49] C++：写文件
来源：http://wtg.shzxlz.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://klv.gogol.net.cn

[S50] C++：格式化数字
来源：http://dhh.haohaochexian.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gbv.tian-w.cn

[S51] C++：显式类型转换
来源：http://xdd.daxiang520.top

static_cast<double>(a) / b
来源：http://rdq.0kj1m.cn

[S52] C++：const 与 noexcept
来源：http://pcg.xziqi.cn

int size() const noexcept { return n_; }
来源：http://icg.sufxvd.cn

[S53] C++：移动语义
来源：http://jlh.cdnleiting.top

std::vector<int> w = std::move(v);
来源：http://mio.sxryk.cn

[S54] C++：异常处理
来源：http://cmr.gaohongyu789.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hgq.jinyuanbaomall.cn

[S55] C++：结构化绑定
来源：http://ocv.yangfankeji.com

auto [a, b] = std::make_pair(1, 2);
来源：http://uzb.fktsv.cn

[S56] C++：optional
来源：http://vgt.jyoumei.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xts.gogol.net.cn

[S57] C++：编译期常量
来源：http://aqa.jlsjyb.cn

constexpr int N = 10;
来源：http://avt.gaohongyu789.top

[S58] C++：命名空间
来源：http://aze.hywenlv.cn

namespace ns { int f() { return 1; } }
来源：http://fum.meibo888.top

[S59] C++：静态断言
来源：http://dyj.xuanzx.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dca.shangyingyoupin.top

[S60] C++：遍历并删除元素
来源：http://qtk.zdqjudy.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gmw.shzxlz.cn

================================================================================
来源：http://uzp.meibo888.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jel.shzxlz.cn

================================================================================
来源：http://hfc.gaohongyu789.top

[T01] Kotlin：Hello World
来源：http://hfy.zhongyouzk.top

println("Hello")
来源：http://osq.tian-w.cn

[T02] Kotlin：变量
来源：http://hol.daria6918.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mrr.jinyuanbaomall.cn

[T03] Kotlin：字符串模板
来源：http://nmu.zhaomingkeji.xyz

"值: $b"
来源：http://rux.feifeiyinyue.top

[T04] Kotlin：空安全
来源：http://bwk.gotoacloud.top

val n: String? = null;  n?.length
来源：http://wif.ybcxt.top

[T05] Kotlin：when 表达式
来源：http://kij.ybcxt.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ebo.hfpthk.cn

[T06] Kotlin：集合映射
来源：http://fma.jinqigfzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://aqk.jqgufenzy.top

[T07] Kotlin：集合过滤
来源：http://wec.fzhhl.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://jte.ywan-chungtsiang.top

[T08] Kotlin：数据类
来源：http://spo.0kj1m.cn

data class User(val name: String, val age: Int)
来源：http://pfa.bjfxy.top

[T09] Kotlin：扩展函数
来源：http://qxd.iojbl.cn

fun String.exclaim() = this + "!"
来源：http://ffv.dianchejie.cn

[T10] Kotlin：默认参数
来源：http://pfi.tanke756.top

fun greet(name: String = "World") = "Hi $name"
来源：http://wtz.xinyue.icu

[T11] Kotlin：协程
来源：http://ejl.aizwys.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bsd.ydjk.org.cn

[T12] Kotlin：解构声明
来源：http://zxl.hnqzz.top

val (a, b) = Pair(1, 2)
来源：http://dvv.meibo888.top

[T13] Kotlin：只读 Map
来源：http://idy.hfpthk.cn

val m = mapOf("a" to 1)
来源：http://lxx.hysaishi.cn

[T14] Kotlin：循环
来源：http://mrh.ydzc1.top

for (i in 1..10) println(i)
来源：http://vfi.jinqigfzy.top

[T15] Kotlin：接口
来源：http://djh.cdnleiting.top

interface Shape { fun area(): Double }
来源：http://qff.quarkkingdee.top

[T16] Swift：Hello World
来源：http://vxt.sxryk.cn

print("Hello")
来源：http://pon.tianlin.xyz

[T17] Swift：变量与常量
来源：http://xtz.pycfn.com

var a = 1;  let b = 2
来源：http://kem.jinqigfzy.top

[T18] Swift：字符串插值
来源：http://nof.zdqjudy.top

"值: \(b)"
来源：http://cpt.jinqigufen.top

[T19] Swift：可选绑定
来源：http://gor.shanyushiyangkeji.top

if let n = opt { print(n) }
来源：http://pvo.daxiang520.top

[T20] Swift：数组操作
来源：http://byb.jiagoushi.top

var a = [1, 2, 3];  a.append(4)
来源：http://uif.ybcxt.top

[T21] Swift：遍历
来源：http://miq.jqgufenzy.top

for x in a { print(x) }
来源：http://abo.yfazqb.com

[T22] Swift：字典
来源：http://gyt.shuidangran.top

var d = ["a": 1];  d["b"] = 2
来源：http://fin.fanxiaobao.xyz

[T23] Swift：函数
来源：http://jis.andypj.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tot.smart0.xyz

[T24] Swift：闭包
来源：http://raz.pycfn.com

let f = { (x: Int) -> Int in x * 2 }
来源：http://mcl.guannengcc.top

[T25] Swift：结构体
来源：http://wnj.gogol.net.cn

struct P { var x: Int }
来源：http://ukj.sjlbkw.cn

[T26] Swift：类与重写
来源：http://pyl.shuidangran.top

class A: Base { override func f() {} }
来源：http://yhw.0kj1m.cn

[T27] Swift：错误处理
来源：http://dfd.feifeiyinyue.top

do { try f() } catch { print(error) }
来源：http://jqy.sjlbkw.cn

[T28] Swift：枚举
来源：http://rzh.yj20258888.top

enum Color { case red, green }
来源：http://sfc.daxiang520.top


<!-- 参考信息 -->