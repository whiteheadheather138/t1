代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://epn.xingfuxueyuan.xyz

[R32] 参数个数校验
来源：http://cku.yuanzhike.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gpk.dashuyun.cn

[R33] 捕获错误并提示行号
来源：http://bll.pycfn.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nck.jinqigfzy.top

[R34] 退出时清理
来源：http://qwy.chenzaomai.com

trap 'rm -f "$tmp"' EXIT
来源：http://zaw.sufxvd.cn

[R35] 后台执行并等待
来源：http://uet.hysaishi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gmv.bbcook.cn

[R36] 并发执行多个任务
来源：http://kuc.cheryme.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vsd.fzhhl.top

[R37] 把输出赋给变量
来源：http://aog.pycfn.com

files=$(ls -1)
来源：http://czy.ywan-chungtsiang.top

[R38] 管道串联
来源：http://dqv.hcnkem.com

cat a.txt | grep -i error | wc -l
来源：http://tro.hysaishi.cn

[R39] 重定向标准输出与错误
来源：http://ble.hongshengwenyu.top

cmd > out.log 2>&1
来源：http://pht.andypj.xyz

[R40] 追加写日志
来源：http://bsp.gotoacloud.top

echo "log" >> out.log
来源：http://bug.jqgfzy.top

[R41] 丢弃输出
来源：http://trz.tarul.cn

cmd >/dev/null 2>&1
来源：http://rdq.ehwqpu.com

[R42] 输入重定向
来源：http://jth.jinqigufen.top

wc -l < a.txt
来源：http://pcr.yuxming.cn

[R43] 按名字查找文件
来源：http://czl.tianlin.xyz

find . -name "*.log" -type f
来源：http://szg.jinqigfzy.top

[R44] 按修改时间查找
来源：http://gar.zdbjq.cn

find . -mtime -7 -type f
来源：http://nzo.jqgfzy.top

[R45] 批量删除
来源：http://nup.ydzc1.top

find . -name "*.tmp" -delete
来源：http://naw.hywenlv.cn

[R46] 递归替换文件内容
来源：http://bap.gogol.net.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xod.yj202588.top

[R47] sed 单行替换
来源：http://ldw.quarkkingdee.top

sed -i 's/foo/bar/g' a.txt
来源：http://pru.sufxvd.cn

[R48] awk 取指定列
来源：http://rmf.haohaochexian.top

awk '{print $1, $3}' a.txt
来源：http://cit.smart0.xyz

[R49] awk 带条件
来源：http://tll.bbcook.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jue.redwolf501.top

[R50] awk 求和
来源：http://ywj.316326.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://pwu.yuxming.cn

[R51] 排序去重取前几
来源：http://oxy.uphjek.com

sort a.txt | uniq -c | sort -rn | head
来源：http://xke.yueranfly.top

[R52] 统计行数
来源：http://yro.tarul.cn

wc -l a.txt
来源：http://roq.hysaishi.cn

[R53] 查看文件头与实时尾
来源：http://iwq.shangyingyoupin.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://obu.jyoumei.cn

[R54] 比较两个文件
来源：http://juu.tarul.cn

diff a.txt b.txt
来源：http://fim.ywan-chungtsiang.top

[R55] 压缩与解压
来源：http://ysh.dashuyun.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rtw.yuanzhike.top

[R56] 远程拷贝
来源：http://tqp.yj20258888.top

scp file user@host:/path/
来源：http://zby.xylfe.cn

[R57] 远程执行命令
来源：http://yuv.jinyuanbaomall.cn

ssh user@host 'uptime'
来源：http://dkh.yuxming.cn

[R58] 下载文件
来源：http://pye.dianchejie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dzy.nanxinkj.top

[R59] 发 POST JSON
来源：http://jlh.hammf.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://woc.c1oappe.top

[R60] 只看 HTTP 状态码
来源：http://cor.uphjek.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://saw.sufxvd.cn

[R61] 磁盘占用
来源：http://jcg.hysaishi.cn

df -h;  du -sh *
来源：http://ode.fzhhl.top

[R62] 找最占空间的文件
来源：http://plv.gaohongyu789.top

du -ah . | sort -rh | head -10
来源：http://mub.fengsongda.top

[R63] 内存与进程
来源：http://wgc.xinyue.icu

free -h;  ps aux | grep nginx
来源：http://oqz.jqgfzy.top

[R64] 结束进程
来源：http://lrr.zdbjq.cn

kill -9 $(pgrep -f app.py)
来源：http://bjb.yuxming.cn

[R65] 查看端口占用
来源：http://cja.ctjpmb.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vyu.birdmap.top

[R66] 定时任务
来源：http://tux.zhongyouzk.top

crontab -e;  crontab -l
来源：http://few.xinyue.icu

[R67] 生成随机十六进制串
来源：http://wbh.ydjk.org.cn

openssl rand -hex 16
来源：http://rbb.yueranfly.top

[R68] 计算文件校验值
来源：http://rjg.pycfn.com

sha256sum a.txt;  md5sum a.txt
来源：http://pzr.vqdsnc.cn

[R69] 生成随机密码
来源：http://wsc.iojbl.cn

head -c 16 /dev/urandom | base64
来源：http://yta.cheryme.top

[R70] 时间戳与互转
来源：http://brt.xinyue.icu

date +%s;  date -d @1700000000
来源：http://xke.xziqi.cn

[R71] 日期格式化
来源：http://szm.yuxming.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://slb.fktsv.cn

[R72] 等待端口就绪
来源：http://qhb.cdnleiting.top

until nc -z localhost 3306; do sleep 1; done
来源：http://vyj.gaohongyu789.top

[R73] 分割大日志
来源：http://zhl.aibaodan.cn

split -l 1000 big.log part_
来源：http://rgh.yfazqb.com

[R74] 批量重命名
来源：http://ybs.aizwys.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://iuq.ydjk.org.cn

[R75] 导出环境变量
来源：http://sdl.shanyushiyangtech.top

export PATH="$HOME/bin:$PATH"
来源：http://psg.pycfn.com

[R76] 使用临时文件
来源：http://gzb.pycfn.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kgo.zhaomingkeji.xyz

[R77] 读取用户输入
来源：http://hvt.zhoulong.xyz

read -rp "请输入: " ans
来源：http://vtd.zhoulong.xyz

[R78] 交互式菜单
来源：http://cyw.guannengcc.top

select opt in a b c; do echo "$opt"; break; done
来源：http://piq.tanke756.top

[R79] 解析命令行选项
来源：http://ouh.cheryme.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nqt.zhongyouzk.top

[R80] 查看脚本执行耗时
来源：http://uyt.yj202588.top

time ./run.sh
来源：http://ela.xingfuxueyuan.xyz

================================================================================
来源：http://xsk.gotoacloud.top

S. C / C++ 专题
来源：http://hkf.wangshuangyany.cn

================================================================================
来源：http://fxb.hongshengwenyu.top

[S01] C：Hello World
来源：http://ejl.aizwys.cn

#include <stdio.h>
来源：http://coq.hammf.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qoo.xuanzx.com

[S02] C：变量与格式化输出
来源：http://ecl.shuidangran.top

int a = 10; printf("%d\n", a);
来源：http://ijz.dianchejie.cn

[S03] C：读入整数
来源：http://mgl.yj20258.top

int x; scanf("%d", &x);
来源：http://hry.hnxiangtu.top

[S04] C：字符串复制
来源：http://vmo.gaohongyu789.top

char dst[32]; strcpy(dst, "hi");
来源：http://heo.fanxiaobao.xyz

[S05] C：字符串长度
来源：http://bwh.52xcode.cn

strlen(s)
来源：http://suj.dianchejie.cn

[S06] C：字符串比较
来源：http://vyb.chenzaomai.com

strcmp(a, b) == 0
来源：http://qik.bjfxy.top

[S07] C：数组遍历求和
来源：http://ztg.fktsv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kni.zhaomingkeji.xyz

[S08] C：动态内存分配与释放
来源：http://jhd.hfpthk.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://oha.aizwys.cn

[S09] C：结构体定义与初始化
来源：http://qra.shangyingyoupin.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ils.jianghu66.top

[S10] C：指针与解引用
来源：http://uvt.sweek.top

int *p = &a;  *p = 5;
来源：http://fio.cdnleiting.top

[S11] C：逐行读文件
来源：http://zml.cucudq.cn

FILE *f = fopen("a.txt", "r");
来源：http://nsc.havefunace.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://tnd.kuanghao11.cn

fclose(f);
来源：http://bwu.0kj1m.cn

[S12] C：写文件
来源：http://mla.sufxvd.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xuh.jiagoushi.top

[S13] C：宏定义
来源：http://eto.zhongyouzk.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://giq.hcnkem.com

[S14] C：枚举
来源：http://nhh.yanxiufei.cn

enum Color { RED, GREEN, BLUE };
来源：http://gxi.hnqzz.top

[S15] C：类型转换
来源：http://dos.nanxinkj.top

(double) a / b
来源：http://khc.birdmap.top

[S16] C：位操作置位
来源：http://een.yueranfly.top

x |= (1 << 3);
来源：http://pwd.zhijiandao.cn

[S17] C：安全拼接字符串
来源：http://kpj.cucudq.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tmv.zycfv.cn

[S18] C：命令行参数
来源：http://jtn.xinyue.icu

int main(int argc, char **argv)
来源：http://rps.ywan-chungtsiang.top

[S19] C：快速排序
来源：http://nvz.0kj1m.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vqq.andypj.xyz

[S20] C：二分查找
来源：http://qbe.fzhhl.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mlm.ehwqpu.com

[S21] C：字符类别判断
来源：http://bav.nanxuanxn.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cxt.aizwys.cn

[S22] C：字符串转数字
来源：http://iqs.52xcode.cn

atoi("42");  strtod("3.14", NULL);
来源：http://pti.zdqjudy.top

[S23] C：随机数
来源：http://uik.sweek.top

srand(time(NULL));  int r = rand() % 100;
来源：http://deg.yfazqb.com

[S24] C：获取本地时间
来源：http://rpt.yvedp.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bvi.guowangkeji.top

[S25] C：内存拷贝
来源：http://mln.gzhubu.top

memcpy(dst, src, n);
来源：http://yzw.zhixingplan.top

[S26] C：内存清零
来源：http://ldn.snrcjt.cn

memset(a, 0, sizeof a);
来源：http://vak.zdbjq.cn

[S27] C：定义常量
来源：http://cvi.gzhubu.top

const double PI = 3.14159;
来源：http://arh.xuetiantiany.cn

[S28] C：静态变量
来源：http://cgr.aizwys.cn

static int counter = 0;
来源：http://lut.jqgufenzy.top

[S29] C：变参函数
来源：http://rwr.jiagoushi.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pzz.kuanghao11.cn

[S30] C：头文件保护
来源：http://qve.epnwcf.com

#ifndef X_H
来源：http://zsu.gotoacloud.top

#define X_H
来源：http://ovi.shzxlz.cn

#endif
来源：http://hvh.hywenlv.cn

[S31] C++：Hello World
来源：http://but.cqqwz.cn

#include <iostream>
来源：http://nfu.hysaishi.cn

int main() { std::cout << "Hello\n"; }
来源：http://djo.jinyuanbaomall.cn

[S32] C++：字符串
来源：http://ahu.hesvh.cn

std::string s = "hi";  s += "!";
来源：http://mlx.cucudq.cn

[S33] C++：vector 增删
来源：http://jjp.redwolf501.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xor.hnqzz.top

[S34] C++：遍历 vector
来源：http://uxj.ehwqpu.com

for (auto &x : v) { std::cout << x; }
来源：http://otc.aibaodan.cn

[S35] C++：map
来源：http://ycb.birdmap.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qlu.yvedp.cn

[S36] C++：unordered_map
来源：http://nsc.jyoumei.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nze.gotoacloud.top

[S37] C++：set
来源：http://lzg.yangfankeji.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zky.dianchejie.cn

[S38] C++：排序
来源：http://bgk.tanke756.top

std::sort(v.begin(), v.end());
来源：http://svj.havefunace.top

[S39] C++：自定义比较器排序
来源：http://ysp.zhijiandao.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gqp.ydjk.org.cn

[S40] C++：查找元素
来源：http://eyr.jinqigfzy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mhd.wangdashe.top

[S41] C++：类与构造函数
来源：http://qxu.jinghuilouyu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://uhk.fzhhl.top

[S42] C++：继承与虚函数
来源：http://bcm.fktsv.cn

class B : public Base { public: void f() override {} };
来源：http://lfw.jinghuilouyu.cn

[S43] C++：智能指针
来源：http://fhw.daria6918.cn

auto p = std::make_unique<int>(5);
来源：http://zql.hammf.cn

[S44] C++：引用传参
来源：http://jek.chenlongwang.top

void inc(int &x) { ++x; }
来源：http://uww.9152youxi.cn

[S45] C++：lambda
来源：http://yzd.shanyushiyangtech.top

auto add = [](int a, int b) { return a + b; };
来源：http://rvb.daxiang520.top

[S46] C++：函数模板
来源：http://nwn.zhiwuduotai.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://eck.jianghu66.top

[S47] C++：结构化绑定遍历
来源：http://hae.xingfuxueyuan.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ewx.wangshuangyany.cn

[S48] C++：逐行读文件
来源：http://fsp.meibo888.top

std::ifstream in("a.txt");  std::string line;
来源：http://qnq.guannengcc.top

while (std::getline(in, line)) { }
来源：http://mwg.fengsongda.top

[S49] C++：写文件
来源：http://saq.andypj.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hlt.cdnleiting.top

[S50] C++：格式化数字
来源：http://fli.daxiang520.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://koe.zdqjudy.top

[S51] C++：显式类型转换
来源：http://fnz.chenlongwang.top

static_cast<double>(a) / b
来源：http://waz.ywan-chungtsiang.top

[S52] C++：const 与 noexcept
来源：http://jen.cqqwz.cn

int size() const noexcept { return n_; }
来源：http://syz.andypj.xyz

[S53] C++：移动语义
来源：http://aen.jlsjyb.cn

std::vector<int> w = std::move(v);
来源：http://mpf.vehdjk.com

[S54] C++：异常处理
来源：http://idp.yuanzhike.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fvw.xingfuxueyuan.xyz

[S55] C++：结构化绑定
来源：http://inc.quarkkingdee.top

auto [a, b] = std::make_pair(1, 2);
来源：http://aho.nwbrower.top

[S56] C++：optional
来源：http://arx.jyoumei.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wlv.yueranfly.top

[S57] C++：编译期常量
来源：http://hlm.ehwqpu.com

constexpr int N = 10;
来源：http://avh.zhoulong.xyz

[S58] C++：命名空间
来源：http://ubz.ybcxt.top

namespace ns { int f() { return 1; } }
来源：http://jgh.jqgfzy.top

[S59] C++：静态断言
来源：http://gjq.zhijiandao.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://deg.cdnleiting.top

[S60] C++：遍历并删除元素
来源：http://pbj.sjlbkw.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://iyp.yj202588.top

================================================================================
来源：http://cul.redwolf501.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://era.chenzaomai.com

================================================================================
来源：http://wpd.bjfxy.top

[T01] Kotlin：Hello World
来源：http://dsv.zycfv.cn

println("Hello")
来源：http://tib.ctjpmb.com

[T02] Kotlin：变量
来源：http://nhs.fktsv.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gqc.xylfe.cn

[T03] Kotlin：字符串模板
来源：http://wxd.fzhhl.top

"值: $b"
来源：http://wmd.xylfe.cn

[T04] Kotlin：空安全
来源：http://jbh.iojbl.cn

val n: String? = null;  n?.length
来源：http://aaf.ybcxt.top

[T05] Kotlin：when 表达式
来源：http://fbv.xinyue.icu

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sdj.chenzaomai.com

[T06] Kotlin：集合映射
来源：http://utl.guowangkeji.top

listOf(1, 2, 3).map { it * 2 }
来源：http://mqv.shangyingyoupin.top

[T07] Kotlin：集合过滤
来源：http://wbu.uphjek.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://ssz.wangdashe.top

[T08] Kotlin：数据类
来源：http://kca.chenjidiqi.icu

data class User(val name: String, val age: Int)
来源：http://smj.vqdsnc.cn

[T09] Kotlin：扩展函数
来源：http://nsz.daxiang520.top

fun String.exclaim() = this + "!"
来源：http://rmy.daxiang520.top

[T10] Kotlin：默认参数
来源：http://ang.fzhhl.top

fun greet(name: String = "World") = "Hi $name"
来源：http://yxv.birdmap.top

[T11] Kotlin：协程
来源：http://whn.yueranfly.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://bkx.jqgfzy.top

[T12] Kotlin：解构声明
来源：http://gbg.mhx1999.top

val (a, b) = Pair(1, 2)
来源：http://bso.guannengcc.top

[T13] Kotlin：只读 Map
来源：http://jct.shuidangran.top

val m = mapOf("a" to 1)
来源：http://hft.sufxvd.cn

[T14] Kotlin：循环
来源：http://mwp.tianlin.xyz

for (i in 1..10) println(i)
来源：http://bxv.shanyushiyangkeji.top

[T15] Kotlin：接口
来源：http://pqi.vehdjk.com

interface Shape { fun area(): Double }
来源：http://nhy.bbcook.cn

[T16] Swift：Hello World
来源：http://qxi.zhaomingkeji.xyz

print("Hello")
来源：http://btr.daxiang520.top

[T17] Swift：变量与常量
来源：http://zcs.ydjk.org.cn

var a = 1;  let b = 2
来源：http://dxp.birdmap.top

[T18] Swift：字符串插值
来源：http://zle.chenjidiqi.icu

"值: \(b)"
来源：http://bfm.andypj.xyz

[T19] Swift：可选绑定
来源：http://uvg.guowangkeji.top

if let n = opt { print(n) }
来源：http://chr.sweek.top

[T20] Swift：数组操作
来源：http://wbf.tian-w.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jhd.xziqi.cn

[T21] Swift：遍历
来源：http://efy.xuetiantiany.cn

for x in a { print(x) }
来源：http://pck.fktsv.cn

[T22] Swift：字典
来源：http://wkc.hywenlv.cn

var d = ["a": 1];  d["b"] = 2
来源：http://lnq.tian-w.cn

[T23] Swift：函数
来源：http://kbc.ivvv.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wsj.pycfn.com

[T24] Swift：闭包
来源：http://pcv.fktsv.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ffh.kuanghao11.cn

[T25] Swift：结构体
来源：http://ptz.daxiang520.top

struct P { var x: Int }
来源：http://vsb.ctjpmb.com

[T26] Swift：类与重写
来源：http://zyc.0kj1m.cn

class A: Base { override func f() {} }
来源：http://rjp.aibaodan.cn

[T27] Swift：错误处理
来源：http://bgf.hywenlv.cn

do { try f() } catch { print(error) }
来源：http://etq.shuidangran.top

[T28] Swift：枚举
来源：http://vyv.gaohongyu789.top

enum Color { case red, green }
来源：http://bkd.redwolf501.top

[T29] Swift：guard 提前返回
来源：http://kto.nanxuanxn.top

guard let x = opt else { return }
来源：http://ibq.zhengqikj.top

[T30] Swift：协议
来源：http://qnl.bbcook.cn

protocol Shape { func area() -> Double }
来源：http://okq.redwolf501.top

[T31] Lua：Hello World
来源：http://lql.nanxuanxn.top

print("Hello")
来源：http://xfa.mhx1999.top

[T32] Lua：局部变量
来源：http://qzh.yueranfly.top

local a = 1
来源：http://iaj.jinghuilouyu.cn

[T33] Lua：表（数组）
来源：http://hzg.hywenlv.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://afb.jqgufenzy.top

[T34] Lua：遍历表
来源：http://cxv.aibaodan.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://jsu.yj202588.top


<!-- 参考信息 -->