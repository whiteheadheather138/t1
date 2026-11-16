代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://glh.gzhubu.top

[R30] 函数返回状态码
来源：http://rlw.yj20258888.top

f() { return 0; }; f || echo "失败了"
来源：http://mif.jiagoushi.top

[R31] 局部变量
来源：http://tkr.yvedp.cn

f() { local x=1; echo "$x"; }
来源：http://vnz.yanxiufei.cn

[R32] 参数个数校验
来源：http://ycu.jinqigufen.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hlf.zhiwuduotai.top

[R33] 捕获错误并提示行号
来源：http://hzd.zhengqikj.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xvx.mhx1999.top

[R34] 退出时清理
来源：http://tza.ydzc1.top

trap 'rm -f "$tmp"' EXIT
来源：http://gqi.chenzaomai.com

[R35] 后台执行并等待
来源：http://mdv.nanxinkj.top

sleep 5 & pid=$!; wait "$pid"
来源：http://dsb.zhoulong.xyz

[R36] 并发执行多个任务
来源：http://pml.daxiang520.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fex.havefunace.top

[R37] 把输出赋给变量
来源：http://ceo.kuanghao11.cn

files=$(ls -1)
来源：http://nem.iojbl.cn

[R38] 管道串联
来源：http://cup.uphjek.com

cat a.txt | grep -i error | wc -l
来源：http://exu.yongpay.top

[R39] 重定向标准输出与错误
来源：http://ctr.zdqjudy.top

cmd > out.log 2>&1
来源：http://cpj.jlsjyb.cn

[R40] 追加写日志
来源：http://tyc.jinghuilouyu.cn

echo "log" >> out.log
来源：http://jbx.havefunace.top

[R41] 丢弃输出
来源：http://eqn.aibaodan.cn

cmd >/dev/null 2>&1
来源：http://aaj.jianghu66.top

[R42] 输入重定向
来源：http://wrl.yj20258888.top

wc -l < a.txt
来源：http://crn.dashuyun.cn

[R43] 按名字查找文件
来源：http://ska.yj20258.top

find . -name "*.log" -type f
来源：http://vmk.jinqigfzy.top

[R44] 按修改时间查找
来源：http://xoi.316326.xyz

find . -mtime -7 -type f
来源：http://uvx.chenlongwang.top

[R45] 批量删除
来源：http://bew.gogol.net.cn

find . -name "*.tmp" -delete
来源：http://tny.zhengqikj.top

[R46] 递归替换文件内容
来源：http://wcp.xinyue.icu

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zgb.nanxuanxn.top

[R47] sed 单行替换
来源：http://eyn.hysaishi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://pzp.nanxuanxn.top

[R48] awk 取指定列
来源：http://otr.chenlongwang.top

awk '{print $1, $3}' a.txt
来源：http://ykv.nwbrower.top

[R49] awk 带条件
来源：http://iqk.jinqigufen.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gek.jinyuanbaomall.cn

[R50] awk 求和
来源：http://cee.cqqwz.cn

awk '{s += $2} END {print s}' a.txt
来源：http://slf.chenjidiqi.icu

[R51] 排序去重取前几
来源：http://qta.yfazqb.com

sort a.txt | uniq -c | sort -rn | head
来源：http://jca.yfazqb.com

[R52] 统计行数
来源：http://syu.hysaishi.cn

wc -l a.txt
来源：http://fcr.fzhhl.top

[R53] 查看文件头与实时尾
来源：http://eyq.wangdashe.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lcd.shanyushiyangtech.top

[R54] 比较两个文件
来源：http://cue.hfpthk.cn

diff a.txt b.txt
来源：http://eml.uphjek.com

[R55] 压缩与解压
来源：http://lxi.9152youxi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ahb.yongpay.top

[R56] 远程拷贝
来源：http://qjy.jinqigfzy.top

scp file user@host:/path/
来源：http://mue.yuxming.cn

[R57] 远程执行命令
来源：http://prp.pycfn.com

ssh user@host 'uptime'
来源：http://dos.fengsongda.top

[R58] 下载文件
来源：http://nad.cucudq.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://stb.jianghu66.top

[R59] 发 POST JSON
来源：http://zcu.yj202588.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://los.chenlongwang.top

[R60] 只看 HTTP 状态码
来源：http://mfd.yuxming.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://llt.gzhubu.top

[R61] 磁盘占用
来源：http://ibh.zhaomingkeji.xyz

df -h;  du -sh *
来源：http://jaz.wangshuangyany.cn

[R62] 找最占空间的文件
来源：http://saw.zycfv.cn

du -ah . | sort -rh | head -10
来源：http://aja.zhengqikj.top

[R63] 内存与进程
来源：http://nuz.yvedp.cn

free -h;  ps aux | grep nginx
来源：http://zhz.nwbrower.top

[R64] 结束进程
来源：http://dtw.zdqjudy.top

kill -9 $(pgrep -f app.py)
来源：http://nnu.hesvh.cn

[R65] 查看端口占用
来源：http://bvd.zhijiandao.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://thl.chenzaomai.com

[R66] 定时任务
来源：http://oiw.sufxvd.cn

crontab -e;  crontab -l
来源：http://kxr.daxiang520.top

[R67] 生成随机十六进制串
来源：http://hxl.ywan-chungtsiang.top

openssl rand -hex 16
来源：http://ipq.hywenlv.cn

[R68] 计算文件校验值
来源：http://ttf.c1oappe.top

sha256sum a.txt;  md5sum a.txt
来源：http://aoy.guowangkeji.top

[R69] 生成随机密码
来源：http://sqb.quarkkingdee.top

head -c 16 /dev/urandom | base64
来源：http://iau.c1oappe.top

[R70] 时间戳与互转
来源：http://qsx.ydjk.org.cn

date +%s;  date -d @1700000000
来源：http://wzp.fanxiaobao.xyz

[R71] 日期格式化
来源：http://blg.sjlbkw.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qxb.yongpay.top

[R72] 等待端口就绪
来源：http://tpj.tianlin.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://pad.shuidangran.top

[R73] 分割大日志
来源：http://dgw.feifeiyinyue.top

split -l 1000 big.log part_
来源：http://rnj.daria6918.cn

[R74] 批量重命名
来源：http://sqm.kuanghao11.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xrm.jinyuanbaomall.cn

[R75] 导出环境变量
来源：http://qbl.yueranfly.top

export PATH="$HOME/bin:$PATH"
来源：http://lwz.meibo888.top

[R76] 使用临时文件
来源：http://uyf.feifeiyinyue.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://icu.gaohongyu789.top

[R77] 读取用户输入
来源：http://jvc.guannengcc.top

read -rp "请输入: " ans
来源：http://edh.jinqigufen.top

[R78] 交互式菜单
来源：http://gaa.gaohongyu789.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ncn.guowangkeji.top

[R79] 解析命令行选项
来源：http://vin.hcnkem.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wsg.ivvv.top

[R80] 查看脚本执行耗时
来源：http://urh.smart0.xyz

time ./run.sh
来源：http://oaw.aibaodan.cn

================================================================================
来源：http://sld.gogol.net.cn

S. C / C++ 专题
来源：http://mcm.meibo888.top

================================================================================
来源：http://hbb.ehwqpu.com

[S01] C：Hello World
来源：http://pas.mhx1999.top

#include <stdio.h>
来源：http://ipb.ydzc1.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://jbc.zdqjudy.top

[S02] C：变量与格式化输出
来源：http://dlf.aibaodan.cn

int a = 10; printf("%d\n", a);
来源：http://rhf.bjfxy.top

[S03] C：读入整数
来源：http://qkt.birdmap.top

int x; scanf("%d", &x);
来源：http://snk.guannengcc.top

[S04] C：字符串复制
来源：http://odx.birdmap.top

char dst[32]; strcpy(dst, "hi");
来源：http://cmh.jqgufenzy.top

[S05] C：字符串长度
来源：http://ere.svipenyu.cn

strlen(s)
来源：http://yse.fzhhl.top

[S06] C：字符串比较
来源：http://qan.52xcode.cn

strcmp(a, b) == 0
来源：http://wek.chenzaomai.com

[S07] C：数组遍历求和
来源：http://mzb.bjfxy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vrj.snrcjt.cn

[S08] C：动态内存分配与释放
来源：http://sul.fanxiaobao.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ief.dashuyun.cn

[S09] C：结构体定义与初始化
来源：http://fgx.gotoacloud.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://avk.daria6918.cn

[S10] C：指针与解引用
来源：http://rdh.cheryme.top

int *p = &a;  *p = 5;
来源：http://blp.gogol.net.cn

[S11] C：逐行读文件
来源：http://xsq.andypj.xyz

FILE *f = fopen("a.txt", "r");
来源：http://rge.chenjidiqi.icu

while (fgets(buf, sizeof buf, f)) { }
来源：http://hts.c1oappe.top

fclose(f);
来源：http://hmi.tian-w.cn

[S12] C：写文件
来源：http://pnp.zdqjudy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hje.shanyushiyangtech.top

[S13] C：宏定义
来源：http://gwh.zycfv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://evr.guowangkeji.top

[S14] C：枚举
来源：http://cyn.hywenlv.cn

enum Color { RED, GREEN, BLUE };
来源：http://cqd.hywenlv.cn

[S15] C：类型转换
来源：http://fpy.fehbvm.com

(double) a / b
来源：http://vle.sysykeji.top

[S16] C：位操作置位
来源：http://wle.ivvv.top

x |= (1 << 3);
来源：http://cld.pengpengdd.cyou

[S17] C：安全拼接字符串
来源：http://gzw.shzxlz.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mot.ctjpmb.com

[S18] C：命令行参数
来源：http://gqp.zdbjq.cn

int main(int argc, char **argv)
来源：http://kya.nanxinkj.top

[S19] C：快速排序
来源：http://tvb.wangshuangyany.cn

qsort(a, n, sizeof(int), cmp);
来源：http://kzt.fanxiaobao.xyz

[S20] C：二分查找
来源：http://xkk.zdqjudy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ycw.yuanzhike.top

[S21] C：字符类别判断
来源：http://wvd.c1oappe.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://owt.wangdashe.top

[S22] C：字符串转数字
来源：http://fxz.guowangkeji.top

atoi("42");  strtod("3.14", NULL);
来源：http://giu.yj20258.top

[S23] C：随机数
来源：http://eyp.9152youxi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://dfg.zdbjq.cn

[S24] C：获取本地时间
来源：http://ytg.jianghu66.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jec.epnwcf.com

[S25] C：内存拷贝
来源：http://axa.52xcode.cn

memcpy(dst, src, n);
来源：http://yrq.havefunace.top

[S26] C：内存清零
来源：http://mpo.nwbrower.top

memset(a, 0, sizeof a);
来源：http://ekz.yvedp.cn

[S27] C：定义常量
来源：http://ede.zdbjq.cn

const double PI = 3.14159;
来源：http://smg.hfpthk.cn

[S28] C：静态变量
来源：http://xjv.iojbl.cn

static int counter = 0;
来源：http://grc.havefunace.top

[S29] C：变参函数
来源：http://rvl.pycfn.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sbw.tian-w.cn

[S30] C：头文件保护
来源：http://okz.tarul.cn

#ifndef X_H
来源：http://iik.hnxiangtu.top

#define X_H
来源：http://lms.dianchejie.cn

#endif
来源：http://san.cdnleiting.top

[S31] C++：Hello World
来源：http://eet.zdqjudy.top

#include <iostream>
来源：http://qpx.andypj.xyz

int main() { std::cout << "Hello\n"; }
来源：http://vuf.0kj1m.cn

[S32] C++：字符串
来源：http://qxs.nwbrower.top

std::string s = "hi";  s += "!";
来源：http://efd.birdmap.top

[S33] C++：vector 增删
来源：http://afy.xinyue.icu

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://oou.mhx1999.top

[S34] C++：遍历 vector
来源：http://glr.aizwys.cn

for (auto &x : v) { std::cout << x; }
来源：http://xbu.yj20258.top

[S35] C++：map
来源：http://zkj.pengpengdd.cyou

std::map<std::string, int> m;  m["a"] = 1;
来源：http://der.cheryme.top

[S36] C++：unordered_map
来源：http://oof.xinyue.icu

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hig.hnxiangtu.top

[S37] C++：set
来源：http://zlr.yuxming.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fgb.hesvh.cn

[S38] C++：排序
来源：http://sgs.vqdsnc.cn

std::sort(v.begin(), v.end());
来源：http://ipz.c1oappe.top

[S39] C++：自定义比较器排序
来源：http://nxi.52xcode.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ifq.zhongyouzk.top

[S40] C++：查找元素
来源：http://mqy.yongpay.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dtf.fehbvm.com

[S41] C++：类与构造函数
来源：http://muz.snrcjt.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pwj.yongpay.top

[S42] C++：继承与虚函数
来源：http://pld.0kj1m.cn

class B : public Base { public: void f() override {} };
来源：http://wuc.guowangkeji.top

[S43] C++：智能指针
来源：http://aay.jinqigfzy.top

auto p = std::make_unique<int>(5);
来源：http://upb.andypj.xyz

[S44] C++：引用传参
来源：http://ymu.gaohongyu789.top

void inc(int &x) { ++x; }
来源：http://lgc.ivvv.top

[S45] C++：lambda
来源：http://llg.zhixingplan.top

auto add = [](int a, int b) { return a + b; };
来源：http://pps.tanke756.top

[S46] C++：函数模板
来源：http://fst.shanyushiyangkeji.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jub.xuetiantiany.cn

[S47] C++：结构化绑定遍历
来源：http://ape.wangdashe.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vpr.dianchejie.cn

[S48] C++：逐行读文件
来源：http://ppx.9152youxi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ehd.yonumen.top

while (std::getline(in, line)) { }
来源：http://ihz.yuanzhike.top

[S49] C++：写文件
来源：http://mxk.yongpay.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://teb.wangshuangyany.cn

[S50] C++：格式化数字
来源：http://fth.gzhubu.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lny.tarul.cn

[S51] C++：显式类型转换
来源：http://ofv.smart0.xyz

static_cast<double>(a) / b
来源：http://gop.ehwqpu.com

[S52] C++：const 与 noexcept
来源：http://ojo.jyoumei.cn

int size() const noexcept { return n_; }
来源：http://mum.52xcode.cn

[S53] C++：移动语义
来源：http://aad.fengsongda.top

std::vector<int> w = std::move(v);
来源：http://mja.aizwys.cn

[S54] C++：异常处理
来源：http://hkw.tianlin.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qew.quarkkingdee.top

[S55] C++：结构化绑定
来源：http://ybv.vehdjk.com

auto [a, b] = std::make_pair(1, 2);
来源：http://lkx.jinghuilouyu.cn

[S56] C++：optional
来源：http://mhc.xinyue.icu

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dqc.tanke756.top

[S57] C++：编译期常量
来源：http://xuk.dashuyun.cn

constexpr int N = 10;
来源：http://urz.yonumen.top

[S58] C++：命名空间
来源：http://afm.sweek.top

namespace ns { int f() { return 1; } }
来源：http://cbv.sysykeji.top

[S59] C++：静态断言
来源：http://nen.cheryme.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zng.fengsongda.top

[S60] C++：遍历并删除元素
来源：http://sfw.redwolf501.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sof.chenzaomai.com

================================================================================
来源：http://ann.tianlin.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hye.tian-w.cn

================================================================================
来源：http://uwl.jyoumei.cn

[T01] Kotlin：Hello World
来源：http://mtv.birdmap.top

println("Hello")
来源：http://hre.epnwcf.com

[T02] Kotlin：变量
来源：http://oqc.ydzc1.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://iel.gaohongyu789.top

[T03] Kotlin：字符串模板
来源：http://oqx.snrcjt.cn

"值: $b"
来源：http://gdc.yueranfly.top

[T04] Kotlin：空安全
来源：http://wba.yueranfly.top

val n: String? = null;  n?.length
来源：http://tst.cdnleiting.top

[T05] Kotlin：when 表达式
来源：http://roe.dashuyun.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mum.shangyingyoupin.top

[T06] Kotlin：集合映射
来源：http://dtv.xuetiantiany.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ezr.iojbl.cn

[T07] Kotlin：集合过滤
来源：http://bbn.cashguo.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://oxd.aibaodan.cn

[T08] Kotlin：数据类
来源：http://ooq.bjfxy.top

data class User(val name: String, val age: Int)
来源：http://rwz.shanyushiyangkeji.top

[T09] Kotlin：扩展函数
来源：http://vkw.zhaomingkeji.xyz

fun String.exclaim() = this + "!"
来源：http://did.redwolf501.top

[T10] Kotlin：默认参数
来源：http://uzi.jqgufenzy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://lbr.jinyuanbaomall.cn

[T11] Kotlin：协程
来源：http://bgq.hesvh.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://akp.tianlin.xyz

[T12] Kotlin：解构声明
来源：http://wsp.yuanzhike.top

val (a, b) = Pair(1, 2)
来源：http://eug.ybcxt.top

[T13] Kotlin：只读 Map
来源：http://llz.hywenlv.cn

val m = mapOf("a" to 1)
来源：http://htn.snrcjt.cn

[T14] Kotlin：循环
来源：http://cql.ybcxt.top

for (i in 1..10) println(i)
来源：http://hoe.gotoacloud.top

[T15] Kotlin：接口
来源：http://yjy.xinyue.icu

interface Shape { fun area(): Double }
来源：http://qft.vehdjk.com

[T16] Swift：Hello World
来源：http://lev.tian-w.cn

print("Hello")
来源：http://zky.gaohongyu789.top

[T17] Swift：变量与常量
来源：http://zhd.tian-w.cn

var a = 1;  let b = 2
来源：http://oqe.hysaishi.cn

[T18] Swift：字符串插值
来源：http://cop.sysykeji.top

"值: \(b)"
来源：http://ceg.shangyingyoupin.top

[T19] Swift：可选绑定
来源：http://omc.havefunace.top

if let n = opt { print(n) }
来源：http://emz.ctjpmb.com

[T20] Swift：数组操作
来源：http://ggw.hnqzz.top

var a = [1, 2, 3];  a.append(4)
来源：http://met.yangfankeji.com

[T21] Swift：遍历
来源：http://obo.havefunace.top

for x in a { print(x) }
来源：http://hiy.quarkkingdee.top

[T22] Swift：字典
来源：http://jty.yj20258.top

var d = ["a": 1];  d["b"] = 2
来源：http://khq.jqgfzy.top

[T23] Swift：函数
来源：http://twj.dashuyun.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xmh.zhoulong.xyz

[T24] Swift：闭包
来源：http://dkp.shangyingyoupin.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://umy.yvedp.cn

[T25] Swift：结构体
来源：http://dmr.shangyingyoupin.top

struct P { var x: Int }
来源：http://yrr.jqgfzy.top

[T26] Swift：类与重写
来源：http://aij.52xcode.cn

class A: Base { override func f() {} }
来源：http://lbe.haohaochexian.top

[T27] Swift：错误处理
来源：http://ths.jinyuanbaomall.cn

do { try f() } catch { print(error) }
来源：http://ytb.hysaishi.cn

[T28] Swift：枚举
来源：http://llw.andypj.xyz

enum Color { case red, green }
来源：http://tbv.kuanghao11.cn

[T29] Swift：guard 提前返回
来源：http://aqk.ybcxt.top

guard let x = opt else { return }
来源：http://sdc.wangshuangyany.cn

[T30] Swift：协议
来源：http://zox.ctjpmb.com

protocol Shape { func area() -> Double }
来源：http://hmq.sxryk.cn

[T31] Lua：Hello World
来源：http://alx.jinyuanbaomall.cn

print("Hello")
来源：http://hdb.feifeiyinyue.top

[T32] Lua：局部变量
来源：http://tcm.yueranfly.top

local a = 1
来源：http://xbd.pycfn.com


<!-- 参考信息 -->