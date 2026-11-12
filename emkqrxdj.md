代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mni.dianchejie.cn

[R30] 函数返回状态码
来源：http://bxy.yj20258.top

f() { return 0; }; f || echo "失败了"
来源：http://krf.zhengqikj.top

[R31] 局部变量
来源：http://kqr.zdqjudy.top

f() { local x=1; echo "$x"; }
来源：http://gvo.shanyushiyangkeji.top

[R32] 参数个数校验
来源：http://sfg.vqdsnc.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tfh.iojbl.cn

[R33] 捕获错误并提示行号
来源：http://btu.yongpay.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lpt.hnqzz.top

[R34] 退出时清理
来源：http://ycc.hywenlv.cn

trap 'rm -f "$tmp"' EXIT
来源：http://dyr.sufxvd.cn

[R35] 后台执行并等待
来源：http://hwj.yonumen.top

sleep 5 & pid=$!; wait "$pid"
来源：http://evy.xingfuxueyuan.xyz

[R36] 并发执行多个任务
来源：http://khn.epnwcf.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wmo.yanxiufei.cn

[R37] 把输出赋给变量
来源：http://hrc.pycfn.com

files=$(ls -1)
来源：http://xje.9152youxi.cn

[R38] 管道串联
来源：http://mqt.meibo888.top

cat a.txt | grep -i error | wc -l
来源：http://hcd.hysaishi.cn

[R39] 重定向标准输出与错误
来源：http://tyy.shangyingyoupin.top

cmd > out.log 2>&1
来源：http://fmh.cdnleiting.top

[R40] 追加写日志
来源：http://ubn.jinqigfzy.top

echo "log" >> out.log
来源：http://avy.zhixingplan.top

[R41] 丢弃输出
来源：http://aao.gogol.net.cn

cmd >/dev/null 2>&1
来源：http://cjs.bbcook.cn

[R42] 输入重定向
来源：http://hvr.daxiang520.top

wc -l < a.txt
来源：http://hde.gotoacloud.top

[R43] 按名字查找文件
来源：http://vdn.hnxiangtu.top

find . -name "*.log" -type f
来源：http://ksm.havefunace.top

[R44] 按修改时间查找
来源：http://nzo.hcnkem.com

find . -mtime -7 -type f
来源：http://ifv.xuanzx.com

[R45] 批量删除
来源：http://udb.nanxuanxn.top

find . -name "*.tmp" -delete
来源：http://iam.ywan-chungtsiang.top

[R46] 递归替换文件内容
来源：http://dhr.vqdsnc.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ode.wangdashe.top

[R47] sed 单行替换
来源：http://kxj.cdnleiting.top

sed -i 's/foo/bar/g' a.txt
来源：http://qsd.gzhubu.top

[R48] awk 取指定列
来源：http://dzt.nanxinkj.top

awk '{print $1, $3}' a.txt
来源：http://yzk.0kj1m.cn

[R49] awk 带条件
来源：http://zqi.daria6918.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vbj.jinqigfzy.top

[R50] awk 求和
来源：http://qyg.yvedp.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ple.zhijiandao.cn

[R51] 排序去重取前几
来源：http://ngv.yonumen.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ayu.cdnleiting.top

[R52] 统计行数
来源：http://ara.cqqwz.cn

wc -l a.txt
来源：http://lvk.birdmap.top

[R53] 查看文件头与实时尾
来源：http://gjh.jlsjyb.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dvb.zhongyouzk.top

[R54] 比较两个文件
来源：http://cvd.haohaochexian.top

diff a.txt b.txt
来源：http://met.shanyushiyangkeji.top

[R55] 压缩与解压
来源：http://sav.yj20258.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qjj.cdnleiting.top

[R56] 远程拷贝
来源：http://puw.zhongyouzk.top

scp file user@host:/path/
来源：http://sjm.yuxming.cn

[R57] 远程执行命令
来源：http://bbv.jianghu66.top

ssh user@host 'uptime'
来源：http://zzk.zdbjq.cn

[R58] 下载文件
来源：http://kea.zdqjudy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xuu.mhx1999.top

[R59] 发 POST JSON
来源：http://cze.hesvh.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://uok.shangyingyoupin.top

[R60] 只看 HTTP 状态码
来源：http://rdm.jiagoushi.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://iqy.yonumen.top

[R61] 磁盘占用
来源：http://cnb.aibaodan.cn

df -h;  du -sh *
来源：http://mci.ywan-chungtsiang.top

[R62] 找最占空间的文件
来源：http://gaw.feifeiyinyue.top

du -ah . | sort -rh | head -10
来源：http://gws.jiagoushi.top

[R63] 内存与进程
来源：http://mki.shanyushiyangkeji.top

free -h;  ps aux | grep nginx
来源：http://hsh.epnwcf.com

[R64] 结束进程
来源：http://fnb.yongpay.top

kill -9 $(pgrep -f app.py)
来源：http://yrz.ydzc1.top

[R65] 查看端口占用
来源：http://jjp.hfpthk.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hop.316326.xyz

[R66] 定时任务
来源：http://rda.xylfe.cn

crontab -e;  crontab -l
来源：http://uwy.ydjk.org.cn

[R67] 生成随机十六进制串
来源：http://qka.fzhhl.top

openssl rand -hex 16
来源：http://mlj.fzhhl.top

[R68] 计算文件校验值
来源：http://dkm.ybcxt.top

sha256sum a.txt;  md5sum a.txt
来源：http://rqs.ywan-chungtsiang.top

[R69] 生成随机密码
来源：http://mmp.tarul.cn

head -c 16 /dev/urandom | base64
来源：http://imm.zhengqikj.top

[R70] 时间戳与互转
来源：http://xrj.xylfe.cn

date +%s;  date -d @1700000000
来源：http://qvl.uphjek.com

[R71] 日期格式化
来源：http://gnu.jlsjyb.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://nlr.tanke756.top

[R72] 等待端口就绪
来源：http://xch.sufxvd.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://itz.shanyushiyangkeji.top

[R73] 分割大日志
来源：http://xfh.yj20258.top

split -l 1000 big.log part_
来源：http://xlu.xuanzx.com

[R74] 批量重命名
来源：http://nle.zdbjq.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tkb.fzhhl.top

[R75] 导出环境变量
来源：http://soh.dianchejie.cn

export PATH="$HOME/bin:$PATH"
来源：http://tes.ppjwa.cn

[R76] 使用临时文件
来源：http://boq.hfpthk.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bhi.wangdashe.top

[R77] 读取用户输入
来源：http://air.xinyue.icu

read -rp "请输入: " ans
来源：http://hpj.gzhubu.top

[R78] 交互式菜单
来源：http://yle.cashguo.top

select opt in a b c; do echo "$opt"; break; done
来源：http://xmc.cdnleiting.top

[R79] 解析命令行选项
来源：http://wmu.havefunace.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gln.mhx1999.top

[R80] 查看脚本执行耗时
来源：http://fih.yj202588.top

time ./run.sh
来源：http://hmc.epnwcf.com

================================================================================
来源：http://lrc.gaohongyu789.top

S. C / C++ 专题
来源：http://ofm.andypj.xyz

================================================================================
来源：http://jsp.cqqwz.cn

[S01] C：Hello World
来源：http://lbq.havefunace.top

#include <stdio.h>
来源：http://yuy.redwolf501.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://esq.iojbl.cn

[S02] C：变量与格式化输出
来源：http://zyx.havefunace.top

int a = 10; printf("%d\n", a);
来源：http://rew.zdbjq.cn

[S03] C：读入整数
来源：http://pad.smart0.xyz

int x; scanf("%d", &x);
来源：http://gvs.jqgufenzy.top

[S04] C：字符串复制
来源：http://qge.zhiwuduotai.top

char dst[32]; strcpy(dst, "hi");
来源：http://xth.zycfv.cn

[S05] C：字符串长度
来源：http://kdw.snrcjt.cn

strlen(s)
来源：http://vmw.c1oappe.top

[S06] C：字符串比较
来源：http://ziz.yvedp.cn

strcmp(a, b) == 0
来源：http://atz.feifeiyinyue.top

[S07] C：数组遍历求和
来源：http://xrf.gaohongyu789.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qpl.nanxuanxn.top

[S08] C：动态内存分配与释放
来源：http://xlf.nwbrower.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yfh.yj20258.top

[S09] C：结构体定义与初始化
来源：http://lar.zhoulong.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://csj.hnxiangtu.top

[S10] C：指针与解引用
来源：http://usk.jinqigfzy.top

int *p = &a;  *p = 5;
来源：http://ink.chenzaomai.com

[S11] C：逐行读文件
来源：http://iiu.guannengcc.top

FILE *f = fopen("a.txt", "r");
来源：http://ony.hammf.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://iwd.nwbrower.top

fclose(f);
来源：http://zps.svipenyu.cn

[S12] C：写文件
来源：http://ksl.fzhhl.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ljn.zdbjq.cn

[S13] C：宏定义
来源：http://fez.aizwys.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dul.tanke756.top

[S14] C：枚举
来源：http://mlw.daxiang520.top

enum Color { RED, GREEN, BLUE };
来源：http://yix.yangfankeji.com

[S15] C：类型转换
来源：http://ekt.snrcjt.cn

(double) a / b
来源：http://ahz.svipenyu.cn

[S16] C：位操作置位
来源：http://dqw.yonumen.top

x |= (1 << 3);
来源：http://hjx.52xcode.cn

[S17] C：安全拼接字符串
来源：http://qoi.gogol.net.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jxk.cucudq.cn

[S18] C：命令行参数
来源：http://dgw.hywenlv.cn

int main(int argc, char **argv)
来源：http://utj.hammf.cn

[S19] C：快速排序
来源：http://inb.xuetiantiany.cn

qsort(a, n, sizeof(int), cmp);
来源：http://bpu.cdnleiting.top

[S20] C：二分查找
来源：http://qia.ybcxt.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://llx.yongpay.top

[S21] C：字符类别判断
来源：http://yhn.yonumen.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sbj.andypj.xyz

[S22] C：字符串转数字
来源：http://eou.iojbl.cn

atoi("42");  strtod("3.14", NULL);
来源：http://nkk.cashguo.top

[S23] C：随机数
来源：http://dwx.hysaishi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xpa.dashuyun.cn

[S24] C：获取本地时间
来源：http://zcj.nanxuanxn.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://she.fktsv.cn

[S25] C：内存拷贝
来源：http://tor.cqqwz.cn

memcpy(dst, src, n);
来源：http://wdh.hammf.cn

[S26] C：内存清零
来源：http://obu.xuanzx.com

memset(a, 0, sizeof a);
来源：http://dxj.shanyushiyangtech.top

[S27] C：定义常量
来源：http://fnl.guannengcc.top

const double PI = 3.14159;
来源：http://dcw.kuanghao11.cn

[S28] C：静态变量
来源：http://zti.pengpengdd.cyou

static int counter = 0;
来源：http://vre.guowangkeji.top

[S29] C：变参函数
来源：http://ktl.hcnkem.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tse.yuanzhike.top

[S30] C：头文件保护
来源：http://rdh.bbcook.cn

#ifndef X_H
来源：http://nvb.jiagoushi.top

#define X_H
来源：http://iuj.zdqjudy.top

#endif
来源：http://fuc.zhiwuduotai.top

[S31] C++：Hello World
来源：http://ltt.mhx1999.top

#include <iostream>
来源：http://rpb.daxiang520.top

int main() { std::cout << "Hello\n"; }
来源：http://ykh.dashuyun.cn

[S32] C++：字符串
来源：http://fum.zhengqikj.top

std::string s = "hi";  s += "!";
来源：http://xhr.kuanghao11.cn

[S33] C++：vector 增删
来源：http://kke.birdmap.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yaf.zhiwuduotai.top

[S34] C++：遍历 vector
来源：http://hap.sufxvd.cn

for (auto &x : v) { std::cout << x; }
来源：http://zzp.fktsv.cn

[S35] C++：map
来源：http://bje.havefunace.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xxv.tarul.cn

[S36] C++：unordered_map
来源：http://any.gogol.net.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lgq.ydzc1.top

[S37] C++：set
来源：http://bfl.wangshuangyany.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ckz.xingfuxueyuan.xyz

[S38] C++：排序
来源：http://vbp.xuetiantiany.cn

std::sort(v.begin(), v.end());
来源：http://hro.yueranfly.top

[S39] C++：自定义比较器排序
来源：http://xks.tianlin.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qsd.fzhhl.top

[S40] C++：查找元素
来源：http://ghf.hnqzz.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ows.vehdjk.com

[S41] C++：类与构造函数
来源：http://daa.sweek.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wnr.xuanzx.com

[S42] C++：继承与虚函数
来源：http://uhz.jinqigufen.top

class B : public Base { public: void f() override {} };
来源：http://jqc.hcnkem.com

[S43] C++：智能指针
来源：http://rma.svipenyu.cn

auto p = std::make_unique<int>(5);
来源：http://ebv.fehbvm.com

[S44] C++：引用传参
来源：http://cyr.iojbl.cn

void inc(int &x) { ++x; }
来源：http://sbs.yuxming.cn

[S45] C++：lambda
来源：http://iyf.ydjk.org.cn

auto add = [](int a, int b) { return a + b; };
来源：http://rsm.zhongyouzk.top

[S46] C++：函数模板
来源：http://qof.cqqwz.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rhd.zhixingplan.top

[S47] C++：结构化绑定遍历
来源：http://ooq.gogol.net.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://idc.sysykeji.top

[S48] C++：逐行读文件
来源：http://xcb.chenjidiqi.icu

std::ifstream in("a.txt");  std::string line;
来源：http://ges.uphjek.com

while (std::getline(in, line)) { }
来源：http://hmr.fanxiaobao.xyz

[S49] C++：写文件
来源：http://drm.andypj.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pwq.xziqi.cn

[S50] C++：格式化数字
来源：http://joq.gzhubu.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jqz.jinqigfzy.top

[S51] C++：显式类型转换
来源：http://gnh.cqqwz.cn

static_cast<double>(a) / b
来源：http://xdu.pengpengdd.cyou

[S52] C++：const 与 noexcept
来源：http://flx.tanke756.top

int size() const noexcept { return n_; }
来源：http://qba.ppjwa.cn

[S53] C++：移动语义
来源：http://dka.zycfv.cn

std::vector<int> w = std::move(v);
来源：http://bjy.gotoacloud.top

[S54] C++：异常处理
来源：http://jyc.zycfv.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bvw.dashuyun.cn

[S55] C++：结构化绑定
来源：http://ynj.shzxlz.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://tvm.havefunace.top

[S56] C++：optional
来源：http://igd.hnqzz.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jbo.yuanzhike.top

[S57] C++：编译期常量
来源：http://cxh.havefunace.top

constexpr int N = 10;
来源：http://rdq.yvedp.cn

[S58] C++：命名空间
来源：http://qyk.iojbl.cn

namespace ns { int f() { return 1; } }
来源：http://gee.chenzaomai.com

[S59] C++：静态断言
来源：http://gvx.jinqigfzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xkr.dashuyun.cn

[S60] C++：遍历并删除元素
来源：http://yur.ydzc1.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://iqp.chenlongwang.top

================================================================================
来源：http://qtt.ydjk.org.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kqy.zhijiandao.cn

================================================================================
来源：http://ebg.ehwqpu.com

[T01] Kotlin：Hello World
来源：http://cmi.feifeiyinyue.top

println("Hello")
来源：http://xot.tarul.cn

[T02] Kotlin：变量
来源：http://gfs.yj20258.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tby.xylfe.cn

[T03] Kotlin：字符串模板
来源：http://hfo.cashguo.top

"值: $b"
来源：http://fhg.hongshengwenyu.top

[T04] Kotlin：空安全
来源：http://vkd.zhongyouzk.top

val n: String? = null;  n?.length
来源：http://mvf.daria6918.cn

[T05] Kotlin：when 表达式
来源：http://ire.hongshengwenyu.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://scy.shzxlz.cn

[T06] Kotlin：集合映射
来源：http://egh.guowangkeji.top

listOf(1, 2, 3).map { it * 2 }
来源：http://eqr.yongpay.top

[T07] Kotlin：集合过滤
来源：http://khy.yonumen.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://bvs.zhoulong.xyz

[T08] Kotlin：数据类
来源：http://rfe.gotoacloud.top

data class User(val name: String, val age: Int)
来源：http://ygw.wangdashe.top

[T09] Kotlin：扩展函数
来源：http://soo.yj202588.top

fun String.exclaim() = this + "!"
来源：http://kmd.hongshengwenyu.top

[T10] Kotlin：默认参数
来源：http://xlf.zycfv.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ffu.jinghuilouyu.cn

[T11] Kotlin：协程
来源：http://kvo.uphjek.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://lrk.jinqigfzy.top

[T12] Kotlin：解构声明
来源：http://uei.vqdsnc.cn

val (a, b) = Pair(1, 2)
来源：http://idx.snrcjt.cn

[T13] Kotlin：只读 Map
来源：http://ani.jinghuilouyu.cn

val m = mapOf("a" to 1)
来源：http://vlj.nanxinkj.top

[T14] Kotlin：循环
来源：http://irf.sufxvd.cn

for (i in 1..10) println(i)
来源：http://llm.yueranfly.top

[T15] Kotlin：接口
来源：http://oja.mhx1999.top

interface Shape { fun area(): Double }
来源：http://deb.zhijiandao.cn

[T16] Swift：Hello World
来源：http://ses.hfpthk.cn

print("Hello")
来源：http://muc.jyoumei.cn

[T17] Swift：变量与常量
来源：http://tqh.ctjpmb.com

var a = 1;  let b = 2
来源：http://rnt.vehdjk.com

[T18] Swift：字符串插值
来源：http://rvm.shuidangran.top

"值: \(b)"
来源：http://zbl.jinqigufen.top

[T19] Swift：可选绑定
来源：http://emg.yj20258.top

if let n = opt { print(n) }
来源：http://ztx.fengsongda.top

[T20] Swift：数组操作
来源：http://agl.hywenlv.cn

var a = [1, 2, 3];  a.append(4)
来源：http://sef.jiagoushi.top

[T21] Swift：遍历
来源：http://uts.zhaomingkeji.xyz

for x in a { print(x) }
来源：http://bge.gaohongyu789.top

[T22] Swift：字典
来源：http://jms.zdqjudy.top

var d = ["a": 1];  d["b"] = 2
来源：http://wrt.jinyuanbaomall.cn

[T23] Swift：函数
来源：http://nve.zhixingplan.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://iin.ybcxt.top

[T24] Swift：闭包
来源：http://vuj.sweek.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://zna.ybcxt.top

[T25] Swift：结构体
来源：http://vil.yj20258.top

struct P { var x: Int }
来源：http://qnj.zdqjudy.top

[T26] Swift：类与重写
来源：http://pcn.fengsongda.top

class A: Base { override func f() {} }
来源：http://sgd.zycfv.cn

[T27] Swift：错误处理
来源：http://klv.sufxvd.cn

do { try f() } catch { print(error) }
来源：http://vdf.feifeiyinyue.top

[T28] Swift：枚举
来源：http://ixd.sysykeji.top

enum Color { case red, green }
来源：http://tpc.xuetiantiany.cn

[T29] Swift：guard 提前返回
来源：http://ykg.jyoumei.cn

guard let x = opt else { return }
来源：http://mdd.nanxinkj.top

[T30] Swift：协议
来源：http://yfj.tarul.cn

protocol Shape { func area() -> Double }
来源：http://avb.aibaodan.cn

[T31] Lua：Hello World
来源：http://rpx.zycfv.cn

print("Hello")
来源：http://ozj.pengpengdd.cyou

[T32] Lua：局部变量
来源：http://ggm.hnqzz.top

local a = 1
来源：http://git.smart0.xyz


<!-- 参考信息 -->