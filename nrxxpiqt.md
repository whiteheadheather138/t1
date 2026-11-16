代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://vlu.cqqwz.cn

[R32] 参数个数校验
来源：http://xfl.meibo888.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dce.zhoulong.xyz

[R33] 捕获错误并提示行号
来源：http://gwi.shanyushiyangtech.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gih.yfazqb.com

[R34] 退出时清理
来源：http://xmo.wangdashe.top

trap 'rm -f "$tmp"' EXIT
来源：http://clw.haohaochexian.top

[R35] 后台执行并等待
来源：http://cxn.gaohongyu789.top

sleep 5 & pid=$!; wait "$pid"
来源：http://dqu.xuetiantiany.cn

[R36] 并发执行多个任务
来源：http://zms.hywenlv.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cgl.zhaomingkeji.xyz

[R37] 把输出赋给变量
来源：http://xyy.xinyue.icu

files=$(ls -1)
来源：http://zmv.hesvh.cn

[R38] 管道串联
来源：http://qcq.jlsjyb.cn

cat a.txt | grep -i error | wc -l
来源：http://wkz.zhiwuduotai.top

[R39] 重定向标准输出与错误
来源：http://mqk.birdmap.top

cmd > out.log 2>&1
来源：http://clt.pycfn.com

[R40] 追加写日志
来源：http://waq.daxiang520.top

echo "log" >> out.log
来源：http://lnk.ywan-chungtsiang.top

[R41] 丢弃输出
来源：http://ncc.zdbjq.cn

cmd >/dev/null 2>&1
来源：http://zbo.sjlbkw.cn

[R42] 输入重定向
来源：http://gyi.jqgufenzy.top

wc -l < a.txt
来源：http://uxf.yuxming.cn

[R43] 按名字查找文件
来源：http://bao.smart0.xyz

find . -name "*.log" -type f
来源：http://hbc.jyoumei.cn

[R44] 按修改时间查找
来源：http://qkp.shzxlz.cn

find . -mtime -7 -type f
来源：http://erw.gogol.net.cn

[R45] 批量删除
来源：http://fhx.gotoacloud.top

find . -name "*.tmp" -delete
来源：http://ajj.kuanghao11.cn

[R46] 递归替换文件内容
来源：http://pvv.shanyushiyangtech.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://afu.zhengqikj.top

[R47] sed 单行替换
来源：http://tpq.xingfuxueyuan.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://zpj.52xcode.cn

[R48] awk 取指定列
来源：http://wxj.nanxuanxn.top

awk '{print $1, $3}' a.txt
来源：http://ecw.snrcjt.cn

[R49] awk 带条件
来源：http://ibm.tian-w.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://uuk.yj20258.top

[R50] awk 求和
来源：http://ikt.9152youxi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://pwn.dianchejie.cn

[R51] 排序去重取前几
来源：http://gog.shanyushiyangtech.top

sort a.txt | uniq -c | sort -rn | head
来源：http://rec.smart0.xyz

[R52] 统计行数
来源：http://nnd.ydzc1.top

wc -l a.txt
来源：http://lvc.fanxiaobao.xyz

[R53] 查看文件头与实时尾
来源：http://eqb.52xcode.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://iqo.aizwys.cn

[R54] 比较两个文件
来源：http://von.xylfe.cn

diff a.txt b.txt
来源：http://pcn.yuxming.cn

[R55] 压缩与解压
来源：http://ykm.wangdashe.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cee.guannengcc.top

[R56] 远程拷贝
来源：http://hur.ybcxt.top

scp file user@host:/path/
来源：http://zho.316326.xyz

[R57] 远程执行命令
来源：http://ydc.sysykeji.top

ssh user@host 'uptime'
来源：http://nii.fktsv.cn

[R58] 下载文件
来源：http://dta.xinyue.icu

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://djs.wangdashe.top

[R59] 发 POST JSON
来源：http://cld.nwbrower.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hjg.yangfankeji.com

[R60] 只看 HTTP 状态码
来源：http://bji.ppjwa.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ypk.epnwcf.com

[R61] 磁盘占用
来源：http://hbj.chenzaomai.com

df -h;  du -sh *
来源：http://cio.mhx1999.top

[R62] 找最占空间的文件
来源：http://kot.jlsjyb.cn

du -ah . | sort -rh | head -10
来源：http://tbm.shuidangran.top

[R63] 内存与进程
来源：http://gej.jqgfzy.top

free -h;  ps aux | grep nginx
来源：http://uud.xylfe.cn

[R64] 结束进程
来源：http://rtr.yuxming.cn

kill -9 $(pgrep -f app.py)
来源：http://qcl.chenjidiqi.icu

[R65] 查看端口占用
来源：http://wzt.yvedp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jmi.sweek.top

[R66] 定时任务
来源：http://szf.cdnleiting.top

crontab -e;  crontab -l
来源：http://ece.ctjpmb.com

[R67] 生成随机十六进制串
来源：http://hbq.andypj.xyz

openssl rand -hex 16
来源：http://lqb.xuetiantiany.cn

[R68] 计算文件校验值
来源：http://mwh.ybcxt.top

sha256sum a.txt;  md5sum a.txt
来源：http://uck.jqgufenzy.top

[R69] 生成随机密码
来源：http://fvw.vqdsnc.cn

head -c 16 /dev/urandom | base64
来源：http://mvs.yj202588.top

[R70] 时间戳与互转
来源：http://rjs.jqgfzy.top

date +%s;  date -d @1700000000
来源：http://ktb.cheryme.top

[R71] 日期格式化
来源：http://gke.jyoumei.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://cxl.jianghu66.top

[R72] 等待端口就绪
来源：http://cew.dashuyun.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zcp.zhiwuduotai.top

[R73] 分割大日志
来源：http://ter.mhx1999.top

split -l 1000 big.log part_
来源：http://gcs.yj20258888.top

[R74] 批量重命名
来源：http://rsf.sufxvd.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tqa.dianchejie.cn

[R75] 导出环境变量
来源：http://oqd.cdnleiting.top

export PATH="$HOME/bin:$PATH"
来源：http://xzz.jlsjyb.cn

[R76] 使用临时文件
来源：http://zlu.sufxvd.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xmo.ydjk.org.cn

[R77] 读取用户输入
来源：http://ftr.yuanzhike.top

read -rp "请输入: " ans
来源：http://arg.c1oappe.top

[R78] 交互式菜单
来源：http://fia.fktsv.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://jne.gzhubu.top

[R79] 解析命令行选项
来源：http://oei.yj202588.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://azw.yj202588.top

[R80] 查看脚本执行耗时
来源：http://zxk.jlsjyb.cn

time ./run.sh
来源：http://xqz.ctjpmb.com

================================================================================
来源：http://vsl.chenlongwang.top

S. C / C++ 专题
来源：http://eqr.jinqigufen.top

================================================================================
来源：http://dqr.ehwqpu.com

[S01] C：Hello World
来源：http://oks.mhx1999.top

#include <stdio.h>
来源：http://qyg.jqgfzy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://qkv.gotoacloud.top

[S02] C：变量与格式化输出
来源：http://pqs.cqqwz.cn

int a = 10; printf("%d\n", a);
来源：http://dfl.hywenlv.cn

[S03] C：读入整数
来源：http://red.tanke756.top

int x; scanf("%d", &x);
来源：http://wke.zycfv.cn

[S04] C：字符串复制
来源：http://xcx.hammf.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ron.jqgufenzy.top

[S05] C：字符串长度
来源：http://put.c1oappe.top

strlen(s)
来源：http://gyp.bbcook.cn

[S06] C：字符串比较
来源：http://mlg.zdqjudy.top

strcmp(a, b) == 0
来源：http://hkr.jinqigfzy.top

[S07] C：数组遍历求和
来源：http://opo.jinqigufen.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ffg.tarul.cn

[S08] C：动态内存分配与释放
来源：http://zdd.feifeiyinyue.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rmi.chenzaomai.com

[S09] C：结构体定义与初始化
来源：http://tsx.wangdashe.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ddr.tanke756.top

[S10] C：指针与解引用
来源：http://msy.pengpengdd.cyou

int *p = &a;  *p = 5;
来源：http://jer.bjfxy.top

[S11] C：逐行读文件
来源：http://kgu.shanyushiyangkeji.top

FILE *f = fopen("a.txt", "r");
来源：http://yfv.yfazqb.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://duh.iojbl.cn

fclose(f);
来源：http://nsz.gogol.net.cn

[S12] C：写文件
来源：http://abe.fanxiaobao.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://moz.shanyushiyangkeji.top

[S13] C：宏定义
来源：http://vho.jyoumei.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ujt.9152youxi.cn

[S14] C：枚举
来源：http://cjl.kuanghao11.cn

enum Color { RED, GREEN, BLUE };
来源：http://ulg.zhengqikj.top

[S15] C：类型转换
来源：http://mzf.jinqigfzy.top

(double) a / b
来源：http://iev.shanyushiyangkeji.top

[S16] C：位操作置位
来源：http://xoh.hywenlv.cn

x |= (1 << 3);
来源：http://pvj.shzxlz.cn

[S17] C：安全拼接字符串
来源：http://fzd.jinqigufen.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lyi.vehdjk.com

[S18] C：命令行参数
来源：http://xku.ppjwa.cn

int main(int argc, char **argv)
来源：http://iyn.zhijiandao.cn

[S19] C：快速排序
来源：http://cqq.jinqigufen.top

qsort(a, n, sizeof(int), cmp);
来源：http://seu.zhijiandao.cn

[S20] C：二分查找
来源：http://sti.sjlbkw.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cco.shanyushiyangtech.top

[S21] C：字符类别判断
来源：http://rlh.ivvv.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vga.sysykeji.top

[S22] C：字符串转数字
来源：http://erw.havefunace.top

atoi("42");  strtod("3.14", NULL);
来源：http://pwo.ehwqpu.com

[S23] C：随机数
来源：http://evw.daria6918.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bsb.ywan-chungtsiang.top

[S24] C：获取本地时间
来源：http://bfk.yj202588.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zeq.birdmap.top

[S25] C：内存拷贝
来源：http://ebu.jyoumei.cn

memcpy(dst, src, n);
来源：http://wwt.9152youxi.cn

[S26] C：内存清零
来源：http://jun.316326.xyz

memset(a, 0, sizeof a);
来源：http://ukk.zhaomingkeji.xyz

[S27] C：定义常量
来源：http://etq.tian-w.cn

const double PI = 3.14159;
来源：http://tqv.tanke756.top

[S28] C：静态变量
来源：http://pfp.vqdsnc.cn

static int counter = 0;
来源：http://bye.0kj1m.cn

[S29] C：变参函数
来源：http://ztd.ydjk.org.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xnw.gogol.net.cn

[S30] C：头文件保护
来源：http://sad.jinqigufen.top

#ifndef X_H
来源：http://qcs.hammf.cn

#define X_H
来源：http://ixr.daria6918.cn

#endif
来源：http://tia.pengpengdd.cyou

[S31] C++：Hello World
来源：http://lop.aizwys.cn

#include <iostream>
来源：http://ibb.daxiang520.top

int main() { std::cout << "Hello\n"; }
来源：http://knj.xingfuxueyuan.xyz

[S32] C++：字符串
来源：http://mqg.hfpthk.cn

std::string s = "hi";  s += "!";
来源：http://xit.hysaishi.cn

[S33] C++：vector 增删
来源：http://rkg.hongshengwenyu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fzp.uphjek.com

[S34] C++：遍历 vector
来源：http://mvv.zhijiandao.cn

for (auto &x : v) { std::cout << x; }
来源：http://guy.hongshengwenyu.top

[S35] C++：map
来源：http://zge.xingfuxueyuan.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gvn.hysaishi.cn

[S36] C++：unordered_map
来源：http://tvh.cqqwz.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cjp.nanxuanxn.top

[S37] C++：set
来源：http://wcu.quarkkingdee.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zbv.aibaodan.cn

[S38] C++：排序
来源：http://dcz.guannengcc.top

std::sort(v.begin(), v.end());
来源：http://hmx.feifeiyinyue.top

[S39] C++：自定义比较器排序
来源：http://clr.ivvv.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://amf.havefunace.top

[S40] C++：查找元素
来源：http://ygn.shangyingyoupin.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lty.jinyuanbaomall.cn

[S41] C++：类与构造函数
来源：http://kew.cashguo.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://aof.zhoulong.xyz

[S42] C++：继承与虚函数
来源：http://zpt.ydjk.org.cn

class B : public Base { public: void f() override {} };
来源：http://skg.ydzc1.top

[S43] C++：智能指针
来源：http://wlk.xylfe.cn

auto p = std::make_unique<int>(5);
来源：http://kjs.xziqi.cn

[S44] C++：引用传参
来源：http://exo.yvedp.cn

void inc(int &x) { ++x; }
来源：http://uqh.yueranfly.top

[S45] C++：lambda
来源：http://urb.sjlbkw.cn

auto add = [](int a, int b) { return a + b; };
来源：http://alz.feifeiyinyue.top

[S46] C++：函数模板
来源：http://fwk.jinghuilouyu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jio.mhx1999.top

[S47] C++：结构化绑定遍历
来源：http://cqd.yanxiufei.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://taj.hcnkem.com

[S48] C++：逐行读文件
来源：http://hjg.ppjwa.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xdp.fzhhl.top

while (std::getline(in, line)) { }
来源：http://cet.svipenyu.cn

[S49] C++：写文件
来源：http://gow.hcnkem.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gtf.chenlongwang.top

[S50] C++：格式化数字
来源：http://wzz.hesvh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ncr.gotoacloud.top

[S51] C++：显式类型转换
来源：http://iiu.jinyuanbaomall.cn

static_cast<double>(a) / b
来源：http://saq.tanke756.top

[S52] C++：const 与 noexcept
来源：http://tfn.ybcxt.top

int size() const noexcept { return n_; }
来源：http://kbe.fehbvm.com

[S53] C++：移动语义
来源：http://vmf.quarkkingdee.top

std::vector<int> w = std::move(v);
来源：http://vbh.aizwys.cn

[S54] C++：异常处理
来源：http://bud.zhijiandao.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hdf.yuxming.cn

[S55] C++：结构化绑定
来源：http://vas.ppjwa.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bqu.vqdsnc.cn

[S56] C++：optional
来源：http://fxl.sxryk.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://tyy.fengsongda.top

[S57] C++：编译期常量
来源：http://ibj.cqqwz.cn

constexpr int N = 10;
来源：http://qrz.pycfn.com

[S58] C++：命名空间
来源：http://kvu.svipenyu.cn

namespace ns { int f() { return 1; } }
来源：http://shc.shuidangran.top

[S59] C++：静态断言
来源：http://xcf.c1oappe.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qai.ctjpmb.com

[S60] C++：遍历并删除元素
来源：http://ogd.jiagoushi.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ucm.hammf.cn

================================================================================
来源：http://mee.birdmap.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hhj.jlsjyb.cn

================================================================================
来源：http://nnq.hongshengwenyu.top

[T01] Kotlin：Hello World
来源：http://tul.xuanzx.com

println("Hello")
来源：http://tvr.daria6918.cn

[T02] Kotlin：变量
来源：http://sia.jinqigfzy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fac.daxiang520.top

[T03] Kotlin：字符串模板
来源：http://tkf.sufxvd.cn

"值: $b"
来源：http://yyt.gzhubu.top

[T04] Kotlin：空安全
来源：http://mjv.ydzc1.top

val n: String? = null;  n?.length
来源：http://olq.0kj1m.cn

[T05] Kotlin：when 表达式
来源：http://fal.quarkkingdee.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qxr.yj202588.top

[T06] Kotlin：集合映射
来源：http://bxc.cqqwz.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://kas.tanke756.top

[T07] Kotlin：集合过滤
来源：http://pfm.zhoulong.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://rol.jinyuanbaomall.cn

[T08] Kotlin：数据类
来源：http://afi.sjlbkw.cn

data class User(val name: String, val age: Int)
来源：http://gzm.ydzc1.top

[T09] Kotlin：扩展函数
来源：http://gzx.shangyingyoupin.top

fun String.exclaim() = this + "!"
来源：http://bsi.daria6918.cn

[T10] Kotlin：默认参数
来源：http://jgr.daria6918.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qia.52xcode.cn

[T11] Kotlin：协程
来源：http://ocq.sweek.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://kwa.jinqigufen.top

[T12] Kotlin：解构声明
来源：http://crn.gzhubu.top

val (a, b) = Pair(1, 2)
来源：http://jrv.nanxinkj.top

[T13] Kotlin：只读 Map
来源：http://hga.hcnkem.com

val m = mapOf("a" to 1)
来源：http://msg.haohaochexian.top

[T14] Kotlin：循环
来源：http://ena.gaohongyu789.top

for (i in 1..10) println(i)
来源：http://hyp.havefunace.top

[T15] Kotlin：接口
来源：http://yhf.haohaochexian.top

interface Shape { fun area(): Double }
来源：http://eua.xziqi.cn

[T16] Swift：Hello World
来源：http://jqg.guannengcc.top

print("Hello")
来源：http://aen.zhiwuduotai.top

[T17] Swift：变量与常量
来源：http://fib.nanxuanxn.top

var a = 1;  let b = 2
来源：http://aui.jinyuanbaomall.cn

[T18] Swift：字符串插值
来源：http://hpl.epnwcf.com

"值: \(b)"
来源：http://our.zhijiandao.cn

[T19] Swift：可选绑定
来源：http://qei.ywan-chungtsiang.top

if let n = opt { print(n) }
来源：http://jkj.xziqi.cn

[T20] Swift：数组操作
来源：http://ofm.sysykeji.top

var a = [1, 2, 3];  a.append(4)
来源：http://kyb.zhijiandao.cn

[T21] Swift：遍历
来源：http://wru.hnqzz.top

for x in a { print(x) }
来源：http://lvp.zdqjudy.top

[T22] Swift：字典
来源：http://mdo.jianghu66.top

var d = ["a": 1];  d["b"] = 2
来源：http://gha.ybcxt.top

[T23] Swift：函数
来源：http://hih.kuanghao11.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kgv.yanxiufei.cn

[T24] Swift：闭包
来源：http://tgq.hammf.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://uxl.jlsjyb.cn

[T25] Swift：结构体
来源：http://mzo.0kj1m.cn

struct P { var x: Int }
来源：http://pqt.sjlbkw.cn

[T26] Swift：类与重写
来源：http://vcy.feifeiyinyue.top

class A: Base { override func f() {} }
来源：http://ypy.316326.xyz

[T27] Swift：错误处理
来源：http://bxo.ydzc1.top

do { try f() } catch { print(error) }
来源：http://gat.svipenyu.cn

[T28] Swift：枚举
来源：http://fuw.jlsjyb.cn

enum Color { case red, green }
来源：http://ptu.ybcxt.top

[T29] Swift：guard 提前返回
来源：http://evh.ctjpmb.com

guard let x = opt else { return }
来源：http://tlv.zhixingplan.top

[T30] Swift：协议
来源：http://vqe.zdbjq.cn

protocol Shape { func area() -> Double }
来源：http://pgt.fktsv.cn

[T31] Lua：Hello World
来源：http://nox.cqqwz.cn

print("Hello")
来源：http://hul.yj20258.top

[T32] Lua：局部变量
来源：http://woa.vqdsnc.cn

local a = 1
来源：http://ash.meibo888.top

[T33] Lua：表（数组）
来源：http://tze.hesvh.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hcb.sufxvd.cn

[T34] Lua：遍历表
来源：http://zzp.chenjidiqi.icu

for i, v in ipairs(t) do print(i, v) end
来源：http://jbo.pengpengdd.cyou


<!-- 参考信息 -->