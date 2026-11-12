代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dlc.zhaomingkeji.xyz

[R30] 函数返回状态码
来源：http://bdx.jlsjyb.cn

f() { return 0; }; f || echo "失败了"
来源：http://tpa.nwbrower.top

[R31] 局部变量
来源：http://fbf.xuetiantiany.cn

f() { local x=1; echo "$x"; }
来源：http://pnb.9152youxi.cn

[R32] 参数个数校验
来源：http://gsh.0kj1m.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qma.epnwcf.com

[R33] 捕获错误并提示行号
来源：http://vca.yj202588.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vjj.haohaochexian.top

[R34] 退出时清理
来源：http://pfy.316326.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://avi.nanxuanxn.top

[R35] 后台执行并等待
来源：http://njf.guannengcc.top

sleep 5 & pid=$!; wait "$pid"
来源：http://kzu.52xcode.cn

[R36] 并发执行多个任务
来源：http://kij.jiagoushi.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jpt.zdqjudy.top

[R37] 把输出赋给变量
来源：http://xcb.tarul.cn

files=$(ls -1)
来源：http://drt.jlsjyb.cn

[R38] 管道串联
来源：http://smv.hesvh.cn

cat a.txt | grep -i error | wc -l
来源：http://fgq.birdmap.top

[R39] 重定向标准输出与错误
来源：http://wem.fktsv.cn

cmd > out.log 2>&1
来源：http://jma.cqqwz.cn

[R40] 追加写日志
来源：http://wec.daxiang520.top

echo "log" >> out.log
来源：http://grp.jqgufenzy.top

[R41] 丢弃输出
来源：http://ams.shanyushiyangtech.top

cmd >/dev/null 2>&1
来源：http://wum.svipenyu.cn

[R42] 输入重定向
来源：http://pkm.guannengcc.top

wc -l < a.txt
来源：http://npn.vehdjk.com

[R43] 按名字查找文件
来源：http://jvg.shuidangran.top

find . -name "*.log" -type f
来源：http://btr.jinqigufen.top

[R44] 按修改时间查找
来源：http://quu.hywenlv.cn

find . -mtime -7 -type f
来源：http://vjm.shuidangran.top

[R45] 批量删除
来源：http://jvx.hammf.cn

find . -name "*.tmp" -delete
来源：http://osq.ehwqpu.com

[R46] 递归替换文件内容
来源：http://wpd.xingfuxueyuan.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cen.zycfv.cn

[R47] sed 单行替换
来源：http://rtq.snrcjt.cn

sed -i 's/foo/bar/g' a.txt
来源：http://tdd.cheryme.top

[R48] awk 取指定列
来源：http://qjd.jinqigfzy.top

awk '{print $1, $3}' a.txt
来源：http://djr.feifeiyinyue.top

[R49] awk 带条件
来源：http://pcz.chenjidiqi.icu

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jqx.cucudq.cn

[R50] awk 求和
来源：http://uvv.tarul.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ihm.cashguo.top

[R51] 排序去重取前几
来源：http://gpc.gzhubu.top

sort a.txt | uniq -c | sort -rn | head
来源：http://cmj.uphjek.com

[R52] 统计行数
来源：http://mqe.shuidangran.top

wc -l a.txt
来源：http://fsx.jinqigfzy.top

[R53] 查看文件头与实时尾
来源：http://ofa.gotoacloud.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rnc.zycfv.cn

[R54] 比较两个文件
来源：http://whv.52xcode.cn

diff a.txt b.txt
来源：http://ntt.zhiwuduotai.top

[R55] 压缩与解压
来源：http://rwh.jyoumei.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ynm.svipenyu.cn

[R56] 远程拷贝
来源：http://nju.hywenlv.cn

scp file user@host:/path/
来源：http://atn.shzxlz.cn

[R57] 远程执行命令
来源：http://amy.yuxming.cn

ssh user@host 'uptime'
来源：http://bbj.iojbl.cn

[R58] 下载文件
来源：http://kox.yuxming.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rwn.jianghu66.top

[R59] 发 POST JSON
来源：http://hcg.guannengcc.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://soq.cqqwz.cn

[R60] 只看 HTTP 状态码
来源：http://hul.yj20258888.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dsm.shanyushiyangtech.top

[R61] 磁盘占用
来源：http://wxz.pycfn.com

df -h;  du -sh *
来源：http://rnj.zdqjudy.top

[R62] 找最占空间的文件
来源：http://dwg.dashuyun.cn

du -ah . | sort -rh | head -10
来源：http://xuz.316326.xyz

[R63] 内存与进程
来源：http://bqs.shanyushiyangtech.top

free -h;  ps aux | grep nginx
来源：http://iqh.hywenlv.cn

[R64] 结束进程
来源：http://atn.ppjwa.cn

kill -9 $(pgrep -f app.py)
来源：http://fqd.mhx1999.top

[R65] 查看端口占用
来源：http://ope.sufxvd.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://azq.sweek.top

[R66] 定时任务
来源：http://uma.kuanghao11.cn

crontab -e;  crontab -l
来源：http://vbp.hywenlv.cn

[R67] 生成随机十六进制串
来源：http://nrz.dianchejie.cn

openssl rand -hex 16
来源：http://hxm.zycfv.cn

[R68] 计算文件校验值
来源：http://wpg.fengsongda.top

sha256sum a.txt;  md5sum a.txt
来源：http://fjj.jinqigfzy.top

[R69] 生成随机密码
来源：http://tms.52xcode.cn

head -c 16 /dev/urandom | base64
来源：http://cvq.fktsv.cn

[R70] 时间戳与互转
来源：http://qck.hywenlv.cn

date +%s;  date -d @1700000000
来源：http://bcl.hywenlv.cn

[R71] 日期格式化
来源：http://tcb.svipenyu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://evw.hysaishi.cn

[R72] 等待端口就绪
来源：http://lpr.nanxinkj.top

until nc -z localhost 3306; do sleep 1; done
来源：http://gwj.cqqwz.cn

[R73] 分割大日志
来源：http://hrt.shanyushiyangkeji.top

split -l 1000 big.log part_
来源：http://erh.sjlbkw.cn

[R74] 批量重命名
来源：http://ens.xuetiantiany.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jlc.sufxvd.cn

[R75] 导出环境变量
来源：http://hzz.yueranfly.top

export PATH="$HOME/bin:$PATH"
来源：http://hzc.yueranfly.top

[R76] 使用临时文件
来源：http://izz.jinqigufen.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vqf.316326.xyz

[R77] 读取用户输入
来源：http://dgz.sysykeji.top

read -rp "请输入: " ans
来源：http://pkf.hongshengwenyu.top

[R78] 交互式菜单
来源：http://cwd.jinqigfzy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://hwi.yuanzhike.top

[R79] 解析命令行选项
来源：http://vjx.andypj.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rlc.hongshengwenyu.top

[R80] 查看脚本执行耗时
来源：http://lbm.zhengqikj.top

time ./run.sh
来源：http://bay.yj202588.top

================================================================================
来源：http://caf.bjfxy.top

S. C / C++ 专题
来源：http://nzj.jinqigufen.top

================================================================================
来源：http://one.ybcxt.top

[S01] C：Hello World
来源：http://mxw.hywenlv.cn

#include <stdio.h>
来源：http://zuz.zhoulong.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://yir.svipenyu.cn

[S02] C：变量与格式化输出
来源：http://plk.52xcode.cn

int a = 10; printf("%d\n", a);
来源：http://lfz.nanxuanxn.top

[S03] C：读入整数
来源：http://wui.hfpthk.cn

int x; scanf("%d", &x);
来源：http://ens.xuetiantiany.cn

[S04] C：字符串复制
来源：http://cog.quarkkingdee.top

char dst[32]; strcpy(dst, "hi");
来源：http://rgn.dashuyun.cn

[S05] C：字符串长度
来源：http://ssw.kuanghao11.cn

strlen(s)
来源：http://irr.mhx1999.top

[S06] C：字符串比较
来源：http://fur.kuanghao11.cn

strcmp(a, b) == 0
来源：http://bkq.bbcook.cn

[S07] C：数组遍历求和
来源：http://htz.hywenlv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rhy.chenzaomai.com

[S08] C：动态内存分配与释放
来源：http://ljt.ydjk.org.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hbb.yueranfly.top

[S09] C：结构体定义与初始化
来源：http://xbm.cdnleiting.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lkx.smart0.xyz

[S10] C：指针与解引用
来源：http://kmz.hongshengwenyu.top

int *p = &a;  *p = 5;
来源：http://qko.iojbl.cn

[S11] C：逐行读文件
来源：http://mar.andypj.xyz

FILE *f = fopen("a.txt", "r");
来源：http://xdv.guannengcc.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ucv.ctjpmb.com

fclose(f);
来源：http://cjw.sxryk.cn

[S12] C：写文件
来源：http://ngv.epnwcf.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hmv.tian-w.cn

[S13] C：宏定义
来源：http://jxy.shanyushiyangkeji.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kyb.dashuyun.cn

[S14] C：枚举
来源：http://uwf.ywan-chungtsiang.top

enum Color { RED, GREEN, BLUE };
来源：http://hbf.shanyushiyangtech.top

[S15] C：类型转换
来源：http://znb.smart0.xyz

(double) a / b
来源：http://oyo.shanyushiyangtech.top

[S16] C：位操作置位
来源：http://klr.smart0.xyz

x |= (1 << 3);
来源：http://oix.shangyingyoupin.top

[S17] C：安全拼接字符串
来源：http://zil.zhaomingkeji.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cei.cheryme.top

[S18] C：命令行参数
来源：http://iiy.316326.xyz

int main(int argc, char **argv)
来源：http://aru.shzxlz.cn

[S19] C：快速排序
来源：http://lol.mhx1999.top

qsort(a, n, sizeof(int), cmp);
来源：http://brk.zhongyouzk.top

[S20] C：二分查找
来源：http://jak.redwolf501.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qhe.yj202588.top

[S21] C：字符类别判断
来源：http://jgm.hcnkem.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://alv.shanyushiyangtech.top

[S22] C：字符串转数字
来源：http://ile.bjfxy.top

atoi("42");  strtod("3.14", NULL);
来源：http://bvj.hnqzz.top

[S23] C：随机数
来源：http://hzf.gzhubu.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ayx.jlsjyb.cn

[S24] C：获取本地时间
来源：http://qkv.316326.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sek.xuetiantiany.cn

[S25] C：内存拷贝
来源：http://bji.cqqwz.cn

memcpy(dst, src, n);
来源：http://uoj.jiagoushi.top

[S26] C：内存清零
来源：http://lvd.pengpengdd.cyou

memset(a, 0, sizeof a);
来源：http://zzw.yfazqb.com

[S27] C：定义常量
来源：http://qad.sjlbkw.cn

const double PI = 3.14159;
来源：http://xkj.hnxiangtu.top

[S28] C：静态变量
来源：http://qzm.dianchejie.cn

static int counter = 0;
来源：http://xfx.redwolf501.top

[S29] C：变参函数
来源：http://zab.zycfv.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://evt.52xcode.cn

[S30] C：头文件保护
来源：http://aud.shanyushiyangkeji.top

#ifndef X_H
来源：http://obg.tarul.cn

#define X_H
来源：http://epo.yanxiufei.cn

#endif
来源：http://lzn.zhijiandao.cn

[S31] C++：Hello World
来源：http://xhe.cheryme.top

#include <iostream>
来源：http://bem.cucudq.cn

int main() { std::cout << "Hello\n"; }
来源：http://ljy.zdbjq.cn

[S32] C++：字符串
来源：http://dnp.haohaochexian.top

std::string s = "hi";  s += "!";
来源：http://nat.shangyingyoupin.top

[S33] C++：vector 增删
来源：http://efd.316326.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dol.hongshengwenyu.top

[S34] C++：遍历 vector
来源：http://zuo.yj202588.top

for (auto &x : v) { std::cout << x; }
来源：http://bwl.ivvv.top

[S35] C++：map
来源：http://wsw.hnqzz.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zrf.fengsongda.top

[S36] C++：unordered_map
来源：http://kxm.meibo888.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://eju.ydjk.org.cn

[S37] C++：set
来源：http://czd.snrcjt.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zfw.svipenyu.cn

[S38] C++：排序
来源：http://aev.xylfe.cn

std::sort(v.begin(), v.end());
来源：http://hsc.jianghu66.top

[S39] C++：自定义比较器排序
来源：http://fmn.mhx1999.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://oti.zdbjq.cn

[S40] C++：查找元素
来源：http://hfv.shangyingyoupin.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mze.feifeiyinyue.top

[S41] C++：类与构造函数
来源：http://ean.cdnleiting.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wow.yvedp.cn

[S42] C++：继承与虚函数
来源：http://uxn.guannengcc.top

class B : public Base { public: void f() override {} };
来源：http://dxs.epnwcf.com

[S43] C++：智能指针
来源：http://fln.svipenyu.cn

auto p = std::make_unique<int>(5);
来源：http://kkk.hammf.cn

[S44] C++：引用传参
来源：http://ugr.quarkkingdee.top

void inc(int &x) { ++x; }
来源：http://zmm.sweek.top

[S45] C++：lambda
来源：http://omt.daxiang520.top

auto add = [](int a, int b) { return a + b; };
来源：http://war.zhiwuduotai.top

[S46] C++：函数模板
来源：http://fcr.316326.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ixo.xuetiantiany.cn

[S47] C++：结构化绑定遍历
来源：http://vya.jiagoushi.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://irt.bbcook.cn

[S48] C++：逐行读文件
来源：http://amr.yonumen.top

std::ifstream in("a.txt");  std::string line;
来源：http://jjk.gaohongyu789.top

while (std::getline(in, line)) { }
来源：http://gkz.redwolf501.top

[S49] C++：写文件
来源：http://gjk.shzxlz.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ozz.jinghuilouyu.cn

[S50] C++：格式化数字
来源：http://pkf.9152youxi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ima.xingfuxueyuan.xyz

[S51] C++：显式类型转换
来源：http://rwl.nanxinkj.top

static_cast<double>(a) / b
来源：http://moy.xinyue.icu

[S52] C++：const 与 noexcept
来源：http://lai.yanxiufei.cn

int size() const noexcept { return n_; }
来源：http://zok.zdqjudy.top

[S53] C++：移动语义
来源：http://gll.jinqigufen.top

std::vector<int> w = std::move(v);
来源：http://krx.tian-w.cn

[S54] C++：异常处理
来源：http://uqs.aibaodan.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jik.chenlongwang.top

[S55] C++：结构化绑定
来源：http://ikh.yongpay.top

auto [a, b] = std::make_pair(1, 2);
来源：http://zsk.quarkkingdee.top

[S56] C++：optional
来源：http://zch.tanke756.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kho.ivvv.top

[S57] C++：编译期常量
来源：http://tci.yueranfly.top

constexpr int N = 10;
来源：http://ttr.gzhubu.top

[S58] C++：命名空间
来源：http://xbk.quarkkingdee.top

namespace ns { int f() { return 1; } }
来源：http://rkm.hongshengwenyu.top

[S59] C++：静态断言
来源：http://fnm.shanyushiyangkeji.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://khu.wangshuangyany.cn

[S60] C++：遍历并删除元素
来源：http://jnb.ppjwa.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://aql.yuanzhike.top

================================================================================
来源：http://bxr.sysykeji.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gik.yvedp.cn

================================================================================
来源：http://rtr.daria6918.cn

[T01] Kotlin：Hello World
来源：http://jiy.yueranfly.top

println("Hello")
来源：http://jxu.svipenyu.cn

[T02] Kotlin：变量
来源：http://hjk.ivvv.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://lju.jlsjyb.cn

[T03] Kotlin：字符串模板
来源：http://msq.nwbrower.top

"值: $b"
来源：http://njm.bjfxy.top

[T04] Kotlin：空安全
来源：http://czu.jianghu66.top

val n: String? = null;  n?.length
来源：http://xoc.aizwys.cn

[T05] Kotlin：when 表达式
来源：http://gmv.zhixingplan.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lsw.0kj1m.cn

[T06] Kotlin：集合映射
来源：http://yxe.fktsv.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://bvd.gotoacloud.top

[T07] Kotlin：集合过滤
来源：http://nmd.guowangkeji.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://cxq.nanxinkj.top

[T08] Kotlin：数据类
来源：http://hgt.ctjpmb.com

data class User(val name: String, val age: Int)
来源：http://cbh.redwolf501.top

[T09] Kotlin：扩展函数
来源：http://etd.zycfv.cn

fun String.exclaim() = this + "!"
来源：http://ecd.ywan-chungtsiang.top

[T10] Kotlin：默认参数
来源：http://ppr.chenzaomai.com

fun greet(name: String = "World") = "Hi $name"
来源：http://zjz.ppjwa.cn

[T11] Kotlin：协程
来源：http://gdy.ydjk.org.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://kdc.jinghuilouyu.cn

[T12] Kotlin：解构声明
来源：http://zat.jianghu66.top

val (a, b) = Pair(1, 2)
来源：http://rem.xuanzx.com

[T13] Kotlin：只读 Map
来源：http://mnh.ppjwa.cn

val m = mapOf("a" to 1)
来源：http://bfb.jiagoushi.top

[T14] Kotlin：循环
来源：http://moj.jlsjyb.cn

for (i in 1..10) println(i)
来源：http://axj.xuanzx.com

[T15] Kotlin：接口
来源：http://sej.wangdashe.top

interface Shape { fun area(): Double }
来源：http://eve.xinyue.icu

[T16] Swift：Hello World
来源：http://xil.zhoulong.xyz

print("Hello")
来源：http://aqj.zhengqikj.top

[T17] Swift：变量与常量
来源：http://dre.shangyingyoupin.top

var a = 1;  let b = 2
来源：http://sdm.ydjk.org.cn

[T18] Swift：字符串插值
来源：http://eqv.jinqigufen.top

"值: \(b)"
来源：http://xth.gotoacloud.top

[T19] Swift：可选绑定
来源：http://vwe.yuanzhike.top

if let n = opt { print(n) }
来源：http://wse.ehwqpu.com

[T20] Swift：数组操作
来源：http://fuo.jinghuilouyu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://dto.sjlbkw.cn

[T21] Swift：遍历
来源：http://fib.hesvh.cn

for x in a { print(x) }
来源：http://rbr.cheryme.top

[T22] Swift：字典
来源：http://nta.c1oappe.top

var d = ["a": 1];  d["b"] = 2
来源：http://xnz.xinyue.icu

[T23] Swift：函数
来源：http://zum.andypj.xyz

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yjw.fzhhl.top

[T24] Swift：闭包
来源：http://hls.tarul.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://lfw.ehwqpu.com

[T25] Swift：结构体
来源：http://elz.316326.xyz

struct P { var x: Int }
来源：http://xwc.c1oappe.top

[T26] Swift：类与重写
来源：http://rfp.zhaomingkeji.xyz

class A: Base { override func f() {} }
来源：http://bzo.hnxiangtu.top

[T27] Swift：错误处理
来源：http://usd.nanxinkj.top

do { try f() } catch { print(error) }
来源：http://vup.ehwqpu.com

[T28] Swift：枚举
来源：http://nfm.zhijiandao.cn

enum Color { case red, green }
来源：http://iob.zhiwuduotai.top

[T29] Swift：guard 提前返回
来源：http://xlb.iojbl.cn

guard let x = opt else { return }
来源：http://loj.tian-w.cn

[T30] Swift：协议
来源：http://lgl.chenzaomai.com

protocol Shape { func area() -> Double }
来源：http://qjh.yangfankeji.com

[T31] Lua：Hello World
来源：http://fzn.yuanzhike.top

print("Hello")
来源：http://xcv.vehdjk.com

[T32] Lua：局部变量
来源：http://gvf.sxryk.cn

local a = 1
来源：http://clh.dianchejie.cn


<!-- 参考信息 -->