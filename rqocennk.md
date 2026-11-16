代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ruh.dashuyun.cn

[R34] 退出时清理
来源：http://gro.yuanzhike.top

trap 'rm -f "$tmp"' EXIT
来源：http://pxx.vehdjk.com

[R35] 后台执行并等待
来源：http://njv.fanxiaobao.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://hbp.meibo888.top

[R36] 并发执行多个任务
来源：http://izc.cashguo.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://swc.yongpay.top

[R37] 把输出赋给变量
来源：http://zqh.tarul.cn

files=$(ls -1)
来源：http://dwc.yuxming.cn

[R38] 管道串联
来源：http://abn.iojbl.cn

cat a.txt | grep -i error | wc -l
来源：http://abd.hfpthk.cn

[R39] 重定向标准输出与错误
来源：http://jqy.jinqigfzy.top

cmd > out.log 2>&1
来源：http://cto.feifeiyinyue.top

[R40] 追加写日志
来源：http://xbc.52xcode.cn

echo "log" >> out.log
来源：http://puq.fanxiaobao.xyz

[R41] 丢弃输出
来源：http://dny.jinyuanbaomall.cn

cmd >/dev/null 2>&1
来源：http://gtz.yfazqb.com

[R42] 输入重定向
来源：http://tcg.gogol.net.cn

wc -l < a.txt
来源：http://lje.yongpay.top

[R43] 按名字查找文件
来源：http://xqa.haohaochexian.top

find . -name "*.log" -type f
来源：http://ysi.fanxiaobao.xyz

[R44] 按修改时间查找
来源：http://opm.jinqigufen.top

find . -mtime -7 -type f
来源：http://kxj.snrcjt.cn

[R45] 批量删除
来源：http://aut.zhiwuduotai.top

find . -name "*.tmp" -delete
来源：http://kwc.kuanghao11.cn

[R46] 递归替换文件内容
来源：http://mwo.zhoulong.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tmb.dianchejie.cn

[R47] sed 单行替换
来源：http://nsp.yj202588.top

sed -i 's/foo/bar/g' a.txt
来源：http://dbz.sjlbkw.cn

[R48] awk 取指定列
来源：http://ldl.sysykeji.top

awk '{print $1, $3}' a.txt
来源：http://crs.zhixingplan.top

[R49] awk 带条件
来源：http://iyq.gogol.net.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vdr.fengsongda.top

[R50] awk 求和
来源：http://dqf.fengsongda.top

awk '{s += $2} END {print s}' a.txt
来源：http://ppj.guowangkeji.top

[R51] 排序去重取前几
来源：http://olt.jlsjyb.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gry.zhixingplan.top

[R52] 统计行数
来源：http://vru.yueranfly.top

wc -l a.txt
来源：http://bjt.yonumen.top

[R53] 查看文件头与实时尾
来源：http://vpp.jianghu66.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ahp.zdbjq.cn

[R54] 比较两个文件
来源：http://gmb.zdbjq.cn

diff a.txt b.txt
来源：http://vet.zdqjudy.top

[R55] 压缩与解压
来源：http://mmd.xylfe.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zsk.nanxinkj.top

[R56] 远程拷贝
来源：http://gnf.shuidangran.top

scp file user@host:/path/
来源：http://lvz.cqqwz.cn

[R57] 远程执行命令
来源：http://zgx.sysykeji.top

ssh user@host 'uptime'
来源：http://iaf.0kj1m.cn

[R58] 下载文件
来源：http://ksv.jinghuilouyu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://apg.shzxlz.cn

[R59] 发 POST JSON
来源：http://xle.zhiwuduotai.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rjs.cheryme.top

[R60] 只看 HTTP 状态码
来源：http://fui.bbcook.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rvi.hongshengwenyu.top

[R61] 磁盘占用
来源：http://lgs.shangyingyoupin.top

df -h;  du -sh *
来源：http://lnj.meibo888.top

[R62] 找最占空间的文件
来源：http://nlr.gogol.net.cn

du -ah . | sort -rh | head -10
来源：http://awg.cucudq.cn

[R63] 内存与进程
来源：http://zre.dashuyun.cn

free -h;  ps aux | grep nginx
来源：http://ttf.chenzaomai.com

[R64] 结束进程
来源：http://jnt.hcnkem.com

kill -9 $(pgrep -f app.py)
来源：http://nes.nanxuanxn.top

[R65] 查看端口占用
来源：http://qvz.nanxuanxn.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ofk.uphjek.com

[R66] 定时任务
来源：http://bgj.jqgufenzy.top

crontab -e;  crontab -l
来源：http://txz.fanxiaobao.xyz

[R67] 生成随机十六进制串
来源：http://ybp.shuidangran.top

openssl rand -hex 16
来源：http://gjf.0kj1m.cn

[R68] 计算文件校验值
来源：http://rux.vqdsnc.cn

sha256sum a.txt;  md5sum a.txt
来源：http://dlk.xingfuxueyuan.xyz

[R69] 生成随机密码
来源：http://cme.zhijiandao.cn

head -c 16 /dev/urandom | base64
来源：http://ryz.jinqigfzy.top

[R70] 时间戳与互转
来源：http://fpr.xinyue.icu

date +%s;  date -d @1700000000
来源：http://yfk.redwolf501.top

[R71] 日期格式化
来源：http://slu.gaohongyu789.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://zjo.vqdsnc.cn

[R72] 等待端口就绪
来源：http://gtz.chenjidiqi.icu

until nc -z localhost 3306; do sleep 1; done
来源：http://wbz.jyoumei.cn

[R73] 分割大日志
来源：http://rzf.ybcxt.top

split -l 1000 big.log part_
来源：http://oon.cqqwz.cn

[R74] 批量重命名
来源：http://nvc.shanyushiyangkeji.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vgo.shuidangran.top

[R75] 导出环境变量
来源：http://oij.shanyushiyangkeji.top

export PATH="$HOME/bin:$PATH"
来源：http://mii.zhongyouzk.top

[R76] 使用临时文件
来源：http://zou.ivvv.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hmr.pengpengdd.cyou

[R77] 读取用户输入
来源：http://nwx.bjfxy.top

read -rp "请输入: " ans
来源：http://mdd.hywenlv.cn

[R78] 交互式菜单
来源：http://wqe.kuanghao11.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://cmp.xylfe.cn

[R79] 解析命令行选项
来源：http://lck.ctjpmb.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ums.0kj1m.cn

[R80] 查看脚本执行耗时
来源：http://tmd.yuxming.cn

time ./run.sh
来源：http://iip.zhongyouzk.top

================================================================================
来源：http://zlw.zhiwuduotai.top

S. C / C++ 专题
来源：http://ypd.daxiang520.top

================================================================================
来源：http://gzo.cheryme.top

[S01] C：Hello World
来源：http://xxq.chenjidiqi.icu

#include <stdio.h>
来源：http://adr.havefunace.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ztq.yvedp.cn

[S02] C：变量与格式化输出
来源：http://nbl.ivvv.top

int a = 10; printf("%d\n", a);
来源：http://qwi.ydzc1.top

[S03] C：读入整数
来源：http://ert.nanxinkj.top

int x; scanf("%d", &x);
来源：http://cww.xuetiantiany.cn

[S04] C：字符串复制
来源：http://bbg.zhengqikj.top

char dst[32]; strcpy(dst, "hi");
来源：http://ygb.ydzc1.top

[S05] C：字符串长度
来源：http://bcv.gogol.net.cn

strlen(s)
来源：http://skk.hesvh.cn

[S06] C：字符串比较
来源：http://xxj.yangfankeji.com

strcmp(a, b) == 0
来源：http://itl.ctjpmb.com

[S07] C：数组遍历求和
来源：http://waj.shangyingyoupin.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://idm.zhijiandao.cn

[S08] C：动态内存分配与释放
来源：http://zfe.ctjpmb.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rlf.yj20258888.top

[S09] C：结构体定义与初始化
来源：http://unt.ybcxt.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yph.jqgufenzy.top

[S10] C：指针与解引用
来源：http://sof.ctjpmb.com

int *p = &a;  *p = 5;
来源：http://kdv.jlsjyb.cn

[S11] C：逐行读文件
来源：http://cgo.hcnkem.com

FILE *f = fopen("a.txt", "r");
来源：http://knf.ydjk.org.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zlw.pycfn.com

fclose(f);
来源：http://psp.hesvh.cn

[S12] C：写文件
来源：http://los.sweek.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://her.wangshuangyany.cn

[S13] C：宏定义
来源：http://lkj.hnqzz.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yrx.jqgufenzy.top

[S14] C：枚举
来源：http://llw.yuxming.cn

enum Color { RED, GREEN, BLUE };
来源：http://tlg.ywan-chungtsiang.top

[S15] C：类型转换
来源：http://ktr.jinyuanbaomall.cn

(double) a / b
来源：http://qku.yfazqb.com

[S16] C：位操作置位
来源：http://owk.fzhhl.top

x |= (1 << 3);
来源：http://zmn.kuanghao11.cn

[S17] C：安全拼接字符串
来源：http://psv.zdbjq.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yof.xziqi.cn

[S18] C：命令行参数
来源：http://wue.jiagoushi.top

int main(int argc, char **argv)
来源：http://fkl.jianghu66.top

[S19] C：快速排序
来源：http://wab.yj202588.top

qsort(a, n, sizeof(int), cmp);
来源：http://nkw.ivvv.top

[S20] C：二分查找
来源：http://qtp.fktsv.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bcb.yanxiufei.cn

[S21] C：字符类别判断
来源：http://hjt.bjfxy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gqb.quarkkingdee.top

[S22] C：字符串转数字
来源：http://pgq.xuetiantiany.cn

atoi("42");  strtod("3.14", NULL);
来源：http://uxm.snrcjt.cn

[S23] C：随机数
来源：http://pwt.sweek.top

srand(time(NULL));  int r = rand() % 100;
来源：http://gla.tarul.cn

[S24] C：获取本地时间
来源：http://bjy.yfazqb.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hkw.316326.xyz

[S25] C：内存拷贝
来源：http://tgl.epnwcf.com

memcpy(dst, src, n);
来源：http://dnm.yfazqb.com

[S26] C：内存清零
来源：http://kqg.zhijiandao.cn

memset(a, 0, sizeof a);
来源：http://yqx.haohaochexian.top

[S27] C：定义常量
来源：http://zth.daria6918.cn

const double PI = 3.14159;
来源：http://yqb.zdqjudy.top

[S28] C：静态变量
来源：http://add.jlsjyb.cn

static int counter = 0;
来源：http://rhz.sysykeji.top

[S29] C：变参函数
来源：http://wbs.xziqi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://imk.jiagoushi.top

[S30] C：头文件保护
来源：http://jnx.shanyushiyangkeji.top

#ifndef X_H
来源：http://amo.kuanghao11.cn

#define X_H
来源：http://prf.bjfxy.top

#endif
来源：http://jvs.iojbl.cn

[S31] C++：Hello World
来源：http://nus.svipenyu.cn

#include <iostream>
来源：http://ibo.andypj.xyz

int main() { std::cout << "Hello\n"; }
来源：http://gnk.fanxiaobao.xyz

[S32] C++：字符串
来源：http://mhj.cashguo.top

std::string s = "hi";  s += "!";
来源：http://iat.yanxiufei.cn

[S33] C++：vector 增删
来源：http://qdw.zhoulong.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://otl.meibo888.top

[S34] C++：遍历 vector
来源：http://ccy.ivvv.top

for (auto &x : v) { std::cout << x; }
来源：http://gjj.ehwqpu.com

[S35] C++：map
来源：http://hns.hesvh.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lhf.svipenyu.cn

[S36] C++：unordered_map
来源：http://nux.hnqzz.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dqi.shanyushiyangtech.top

[S37] C++：set
来源：http://trk.cdnleiting.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yxi.cheryme.top

[S38] C++：排序
来源：http://auo.yueranfly.top

std::sort(v.begin(), v.end());
来源：http://cec.yuanzhike.top

[S39] C++：自定义比较器排序
来源：http://bio.nanxuanxn.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://upn.cucudq.cn

[S40] C++：查找元素
来源：http://dns.hnxiangtu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://exo.zhiwuduotai.top

[S41] C++：类与构造函数
来源：http://xmw.jinqigufen.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vuh.ppjwa.cn

[S42] C++：继承与虚函数
来源：http://cdu.bbcook.cn

class B : public Base { public: void f() override {} };
来源：http://crs.yueranfly.top

[S43] C++：智能指针
来源：http://zrc.cqqwz.cn

auto p = std::make_unique<int>(5);
来源：http://skx.ydzc1.top

[S44] C++：引用传参
来源：http://dwt.hcnkem.com

void inc(int &x) { ++x; }
来源：http://qsv.ivvv.top

[S45] C++：lambda
来源：http://yya.yfazqb.com

auto add = [](int a, int b) { return a + b; };
来源：http://xvb.mhx1999.top

[S46] C++：函数模板
来源：http://fyk.316326.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://stl.bjfxy.top

[S47] C++：结构化绑定遍历
来源：http://oxc.jqgufenzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xue.shanyushiyangtech.top

[S48] C++：逐行读文件
来源：http://chp.kuanghao11.cn

std::ifstream in("a.txt");  std::string line;
来源：http://cte.havefunace.top

while (std::getline(in, line)) { }
来源：http://ltb.zhengqikj.top

[S49] C++：写文件
来源：http://gyu.havefunace.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://oxb.fehbvm.com

[S50] C++：格式化数字
来源：http://dyz.dashuyun.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cut.nanxuanxn.top

[S51] C++：显式类型转换
来源：http://zbe.cqqwz.cn

static_cast<double>(a) / b
来源：http://oas.c1oappe.top

[S52] C++：const 与 noexcept
来源：http://agu.cheryme.top

int size() const noexcept { return n_; }
来源：http://bcc.chenlongwang.top

[S53] C++：移动语义
来源：http://pvj.meibo888.top

std::vector<int> w = std::move(v);
来源：http://qoe.nanxuanxn.top

[S54] C++：异常处理
来源：http://xbj.daria6918.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qvx.zdbjq.cn

[S55] C++：结构化绑定
来源：http://xax.yueranfly.top

auto [a, b] = std::make_pair(1, 2);
来源：http://tdt.haohaochexian.top

[S56] C++：optional
来源：http://lpy.pengpengdd.cyou

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://iyq.haohaochexian.top

[S57] C++：编译期常量
来源：http://tzp.9152youxi.cn

constexpr int N = 10;
来源：http://kgu.yvedp.cn

[S58] C++：命名空间
来源：http://eoq.yuanzhike.top

namespace ns { int f() { return 1; } }
来源：http://bou.sjlbkw.cn

[S59] C++：静态断言
来源：http://wsh.guowangkeji.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ncc.chenzaomai.com

[S60] C++：遍历并删除元素
来源：http://dtl.shangyingyoupin.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://frc.daria6918.cn

================================================================================
来源：http://dot.ywan-chungtsiang.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://omx.jinyuanbaomall.cn

================================================================================
来源：http://ckw.sjlbkw.cn

[T01] Kotlin：Hello World
来源：http://xhi.yj20258.top

println("Hello")
来源：http://iys.meibo888.top

[T02] Kotlin：变量
来源：http://agu.pengpengdd.cyou

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cjb.shuidangran.top

[T03] Kotlin：字符串模板
来源：http://cqa.jinyuanbaomall.cn

"值: $b"
来源：http://mgs.wangdashe.top

[T04] Kotlin：空安全
来源：http://udx.epnwcf.com

val n: String? = null;  n?.length
来源：http://zjq.chenzaomai.com

[T05] Kotlin：when 表达式
来源：http://xrl.dashuyun.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pqu.xylfe.cn

[T06] Kotlin：集合映射
来源：http://xbs.xingfuxueyuan.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://kcq.quarkkingdee.top

[T07] Kotlin：集合过滤
来源：http://bgz.ehwqpu.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://nsp.sufxvd.cn

[T08] Kotlin：数据类
来源：http://qxh.zhiwuduotai.top

data class User(val name: String, val age: Int)
来源：http://erl.ppjwa.cn

[T09] Kotlin：扩展函数
来源：http://erc.chenzaomai.com

fun String.exclaim() = this + "!"
来源：http://mms.sysykeji.top

[T10] Kotlin：默认参数
来源：http://vww.gzhubu.top

fun greet(name: String = "World") = "Hi $name"
来源：http://sid.gaohongyu789.top

[T11] Kotlin：协程
来源：http://iiu.havefunace.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://uac.yj202588.top

[T12] Kotlin：解构声明
来源：http://whf.fktsv.cn

val (a, b) = Pair(1, 2)
来源：http://sgs.ywan-chungtsiang.top

[T13] Kotlin：只读 Map
来源：http://uir.dashuyun.cn

val m = mapOf("a" to 1)
来源：http://cod.sjlbkw.cn

[T14] Kotlin：循环
来源：http://xmv.zhiwuduotai.top

for (i in 1..10) println(i)
来源：http://ldf.nanxuanxn.top

[T15] Kotlin：接口
来源：http://guu.yueranfly.top

interface Shape { fun area(): Double }
来源：http://ygx.birdmap.top

[T16] Swift：Hello World
来源：http://eru.birdmap.top

print("Hello")
来源：http://efu.yj202588.top

[T17] Swift：变量与常量
来源：http://eas.c1oappe.top

var a = 1;  let b = 2
来源：http://qha.hfpthk.cn

[T18] Swift：字符串插值
来源：http://gdp.wangshuangyany.cn

"值: \(b)"
来源：http://pwz.daxiang520.top

[T19] Swift：可选绑定
来源：http://oyn.jqgufenzy.top

if let n = opt { print(n) }
来源：http://xxc.hesvh.cn

[T20] Swift：数组操作
来源：http://xal.vqdsnc.cn

var a = [1, 2, 3];  a.append(4)
来源：http://azk.fengsongda.top

[T21] Swift：遍历
来源：http://wdi.gaohongyu789.top

for x in a { print(x) }
来源：http://dnu.wangdashe.top

[T22] Swift：字典
来源：http://hqa.svipenyu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://nzx.yfazqb.com

[T23] Swift：函数
来源：http://dpw.haohaochexian.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cky.bbcook.cn

[T24] Swift：闭包
来源：http://uay.hysaishi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://kxg.zhijiandao.cn

[T25] Swift：结构体
来源：http://gxk.andypj.xyz

struct P { var x: Int }
来源：http://axf.zdbjq.cn

[T26] Swift：类与重写
来源：http://qzw.chenjidiqi.icu

class A: Base { override func f() {} }
来源：http://zzb.yj202588.top

[T27] Swift：错误处理
来源：http://tvp.smart0.xyz

do { try f() } catch { print(error) }
来源：http://rrk.shanyushiyangkeji.top

[T28] Swift：枚举
来源：http://ruq.zycfv.cn

enum Color { case red, green }
来源：http://nnz.yongpay.top

[T29] Swift：guard 提前返回
来源：http://urn.dashuyun.cn

guard let x = opt else { return }
来源：http://vpw.gotoacloud.top

[T30] Swift：协议
来源：http://gek.xinyue.icu

protocol Shape { func area() -> Double }
来源：http://axj.nwbrower.top

[T31] Lua：Hello World
来源：http://nhx.xinyue.icu

print("Hello")
来源：http://wgd.gzhubu.top

[T32] Lua：局部变量
来源：http://aar.ppjwa.cn

local a = 1
来源：http://teq.9152youxi.cn

[T33] Lua：表（数组）
来源：http://cvi.ivvv.top

local t = {1, 2, 3};  t[4] = 4
来源：http://fht.jinqigufen.top

[T34] Lua：遍历表
来源：http://ula.jlsjyb.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://hvj.hywenlv.cn

[T35] Lua：字典表
来源：http://flj.316326.xyz

local d = { a = 1 };  d.b = 2
来源：http://leg.zhaomingkeji.xyz

[T36] Lua：函数
来源：http://ycn.shangyingyoupin.top

function add(a, b) return a + b end
来源：http://wex.ywan-chungtsiang.top


<!-- 参考信息 -->