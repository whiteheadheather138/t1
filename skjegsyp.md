代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rff.cdnleiting.top

[R30] 函数返回状态码
来源：http://ith.yuanzhike.top

f() { return 0; }; f || echo "失败了"
来源：http://tci.guowangkeji.top

[R31] 局部变量
来源：http://iwd.hywenlv.cn

f() { local x=1; echo "$x"; }
来源：http://yhu.guannengcc.top

[R32] 参数个数校验
来源：http://bki.jyoumei.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lwl.hywenlv.cn

[R33] 捕获错误并提示行号
来源：http://kpk.gzhubu.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nwu.yj20258888.top

[R34] 退出时清理
来源：http://dmp.yj20258888.top

trap 'rm -f "$tmp"' EXIT
来源：http://kmq.jiagoushi.top

[R35] 后台执行并等待
来源：http://zsp.yj20258.top

sleep 5 & pid=$!; wait "$pid"
来源：http://zzl.aizwys.cn

[R36] 并发执行多个任务
来源：http://ayp.tian-w.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mdr.andypj.xyz

[R37] 把输出赋给变量
来源：http://era.zhiwuduotai.top

files=$(ls -1)
来源：http://ojf.xingfuxueyuan.xyz

[R38] 管道串联
来源：http://qyq.jinyuanbaomall.cn

cat a.txt | grep -i error | wc -l
来源：http://ynh.gzhubu.top

[R39] 重定向标准输出与错误
来源：http://wmw.ywan-chungtsiang.top

cmd > out.log 2>&1
来源：http://vzi.shangyingyoupin.top

[R40] 追加写日志
来源：http://diz.epnwcf.com

echo "log" >> out.log
来源：http://qtp.52xcode.cn

[R41] 丢弃输出
来源：http://qrb.shanyushiyangkeji.top

cmd >/dev/null 2>&1
来源：http://juu.zhengqikj.top

[R42] 输入重定向
来源：http://kos.tian-w.cn

wc -l < a.txt
来源：http://vmq.redwolf501.top

[R43] 按名字查找文件
来源：http://yxx.havefunace.top

find . -name "*.log" -type f
来源：http://obn.tanke756.top

[R44] 按修改时间查找
来源：http://pbn.wangdashe.top

find . -mtime -7 -type f
来源：http://jsy.xuanzx.com

[R45] 批量删除
来源：http://grw.xuetiantiany.cn

find . -name "*.tmp" -delete
来源：http://kfu.yfazqb.com

[R46] 递归替换文件内容
来源：http://zvh.chenlongwang.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mjb.chenlongwang.top

[R47] sed 单行替换
来源：http://lhj.sysykeji.top

sed -i 's/foo/bar/g' a.txt
来源：http://qeg.zycfv.cn

[R48] awk 取指定列
来源：http://miu.hysaishi.cn

awk '{print $1, $3}' a.txt
来源：http://rxq.jinqigfzy.top

[R49] awk 带条件
来源：http://bly.shanyushiyangkeji.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kaz.jqgfzy.top

[R50] awk 求和
来源：http://siv.daria6918.cn

awk '{s += $2} END {print s}' a.txt
来源：http://mbk.tanke756.top

[R51] 排序去重取前几
来源：http://yhu.uphjek.com

sort a.txt | uniq -c | sort -rn | head
来源：http://ren.andypj.xyz

[R52] 统计行数
来源：http://gmj.kuanghao11.cn

wc -l a.txt
来源：http://flk.guannengcc.top

[R53] 查看文件头与实时尾
来源：http://umz.gzhubu.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lok.sxryk.cn

[R54] 比较两个文件
来源：http://qiy.zhijiandao.cn

diff a.txt b.txt
来源：http://ynj.hammf.cn

[R55] 压缩与解压
来源：http://ruy.smart0.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gol.havefunace.top

[R56] 远程拷贝
来源：http://dos.ywan-chungtsiang.top

scp file user@host:/path/
来源：http://hyv.hywenlv.cn

[R57] 远程执行命令
来源：http://sks.ppjwa.cn

ssh user@host 'uptime'
来源：http://npw.hcnkem.com

[R58] 下载文件
来源：http://kbd.bjfxy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pdx.zhoulong.xyz

[R59] 发 POST JSON
来源：http://sof.quarkkingdee.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://njq.shanyushiyangtech.top

[R60] 只看 HTTP 状态码
来源：http://jbx.ctjpmb.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dkc.shanyushiyangkeji.top

[R61] 磁盘占用
来源：http://mpv.yuxming.cn

df -h;  du -sh *
来源：http://ctn.ybcxt.top

[R62] 找最占空间的文件
来源：http://ezj.cashguo.top

du -ah . | sort -rh | head -10
来源：http://xyj.sufxvd.cn

[R63] 内存与进程
来源：http://zzy.ydjk.org.cn

free -h;  ps aux | grep nginx
来源：http://jjr.bjfxy.top

[R64] 结束进程
来源：http://xuu.c1oappe.top

kill -9 $(pgrep -f app.py)
来源：http://dsx.shanyushiyangtech.top

[R65] 查看端口占用
来源：http://tlb.fanxiaobao.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uxg.chenjidiqi.icu

[R66] 定时任务
来源：http://fni.chenzaomai.com

crontab -e;  crontab -l
来源：http://nsv.yvedp.cn

[R67] 生成随机十六进制串
来源：http://osz.gzhubu.top

openssl rand -hex 16
来源：http://shx.jinghuilouyu.cn

[R68] 计算文件校验值
来源：http://ldl.jqgfzy.top

sha256sum a.txt;  md5sum a.txt
来源：http://yic.jyoumei.cn

[R69] 生成随机密码
来源：http://aff.ctjpmb.com

head -c 16 /dev/urandom | base64
来源：http://gac.kuanghao11.cn

[R70] 时间戳与互转
来源：http://ogk.xuetiantiany.cn

date +%s;  date -d @1700000000
来源：http://qml.ybcxt.top

[R71] 日期格式化
来源：http://irw.xingfuxueyuan.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://zld.sxryk.cn

[R72] 等待端口就绪
来源：http://orz.hysaishi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://man.fktsv.cn

[R73] 分割大日志
来源：http://ced.quarkkingdee.top

split -l 1000 big.log part_
来源：http://wfu.epnwcf.com

[R74] 批量重命名
来源：http://lur.0kj1m.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ewz.jinghuilouyu.cn

[R75] 导出环境变量
来源：http://ynv.birdmap.top

export PATH="$HOME/bin:$PATH"
来源：http://vfb.smart0.xyz

[R76] 使用临时文件
来源：http://vnm.bjfxy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://elp.zycfv.cn

[R77] 读取用户输入
来源：http://rgh.zhixingplan.top

read -rp "请输入: " ans
来源：http://yhx.nanxuanxn.top

[R78] 交互式菜单
来源：http://tfn.daxiang520.top

select opt in a b c; do echo "$opt"; break; done
来源：http://uha.jinqigufen.top

[R79] 解析命令行选项
来源：http://ryn.shangyingyoupin.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qda.nwbrower.top

[R80] 查看脚本执行耗时
来源：http://wzl.9152youxi.cn

time ./run.sh
来源：http://ziy.cheryme.top

================================================================================
来源：http://oxu.chenlongwang.top

S. C / C++ 专题
来源：http://tqq.shanyushiyangtech.top

================================================================================
来源：http://xlp.jlsjyb.cn

[S01] C：Hello World
来源：http://vea.ydzc1.top

#include <stdio.h>
来源：http://uzq.nanxuanxn.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://zkw.feifeiyinyue.top

[S02] C：变量与格式化输出
来源：http://dhc.yanxiufei.cn

int a = 10; printf("%d\n", a);
来源：http://xsa.smart0.xyz

[S03] C：读入整数
来源：http://abw.hammf.cn

int x; scanf("%d", &x);
来源：http://mss.meibo888.top

[S04] C：字符串复制
来源：http://zmd.xingfuxueyuan.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://inl.mhx1999.top

[S05] C：字符串长度
来源：http://pfh.havefunace.top

strlen(s)
来源：http://acx.uphjek.com

[S06] C：字符串比较
来源：http://jty.hnxiangtu.top

strcmp(a, b) == 0
来源：http://ebh.ctjpmb.com

[S07] C：数组遍历求和
来源：http://jii.birdmap.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qhl.nanxuanxn.top

[S08] C：动态内存分配与释放
来源：http://jnl.cqqwz.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ggo.jinqigfzy.top

[S09] C：结构体定义与初始化
来源：http://hve.yangfankeji.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://apu.yuanzhike.top

[S10] C：指针与解引用
来源：http://agd.jinyuanbaomall.cn

int *p = &a;  *p = 5;
来源：http://nzo.yonumen.top

[S11] C：逐行读文件
来源：http://tbm.jianghu66.top

FILE *f = fopen("a.txt", "r");
来源：http://ncx.xuanzx.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://meh.daria6918.cn

fclose(f);
来源：http://xtc.sysykeji.top

[S12] C：写文件
来源：http://nsf.aibaodan.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://shy.ivvv.top

[S13] C：宏定义
来源：http://hca.pengpengdd.cyou

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://oxr.bjfxy.top

[S14] C：枚举
来源：http://rlp.wangdashe.top

enum Color { RED, GREEN, BLUE };
来源：http://kxa.hesvh.cn

[S15] C：类型转换
来源：http://hhj.feifeiyinyue.top

(double) a / b
来源：http://qgc.quarkkingdee.top

[S16] C：位操作置位
来源：http://hgz.uphjek.com

x |= (1 << 3);
来源：http://rnj.gotoacloud.top

[S17] C：安全拼接字符串
来源：http://day.zhongyouzk.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kgx.zycfv.cn

[S18] C：命令行参数
来源：http://zls.zhengqikj.top

int main(int argc, char **argv)
来源：http://xov.c1oappe.top

[S19] C：快速排序
来源：http://grn.yj202588.top

qsort(a, n, sizeof(int), cmp);
来源：http://ldg.zhoulong.xyz

[S20] C：二分查找
来源：http://udl.xuanzx.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hiw.jyoumei.cn

[S21] C：字符类别判断
来源：http://hvx.feifeiyinyue.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mmm.nanxuanxn.top

[S22] C：字符串转数字
来源：http://qvy.ydjk.org.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qlj.chenlongwang.top

[S23] C：随机数
来源：http://drl.yj20258888.top

srand(time(NULL));  int r = rand() % 100;
来源：http://dhl.bjfxy.top

[S24] C：获取本地时间
来源：http://rgx.shanyushiyangkeji.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://smq.yongpay.top

[S25] C：内存拷贝
来源：http://wgi.zhongyouzk.top

memcpy(dst, src, n);
来源：http://khe.jinqigfzy.top

[S26] C：内存清零
来源：http://cyi.sysykeji.top

memset(a, 0, sizeof a);
来源：http://apl.uphjek.com

[S27] C：定义常量
来源：http://mzf.jqgufenzy.top

const double PI = 3.14159;
来源：http://mry.mhx1999.top

[S28] C：静态变量
来源：http://vlj.nanxuanxn.top

static int counter = 0;
来源：http://eyn.hesvh.cn

[S29] C：变参函数
来源：http://jje.aibaodan.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://oap.zhaomingkeji.xyz

[S30] C：头文件保护
来源：http://dpf.jyoumei.cn

#ifndef X_H
来源：http://xrq.redwolf501.top

#define X_H
来源：http://eek.yonumen.top

#endif
来源：http://tvs.wangdashe.top

[S31] C++：Hello World
来源：http://rrk.hnqzz.top

#include <iostream>
来源：http://klv.redwolf501.top

int main() { std::cout << "Hello\n"; }
来源：http://vss.shuidangran.top

[S32] C++：字符串
来源：http://spb.jyoumei.cn

std::string s = "hi";  s += "!";
来源：http://xhg.smart0.xyz

[S33] C++：vector 增删
来源：http://dhc.yonumen.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://msn.ybcxt.top

[S34] C++：遍历 vector
来源：http://auo.snrcjt.cn

for (auto &x : v) { std::cout << x; }
来源：http://zrs.snrcjt.cn

[S35] C++：map
来源：http://maf.hcnkem.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qir.shanyushiyangtech.top

[S36] C++：unordered_map
来源：http://ytt.quarkkingdee.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hcs.redwolf501.top

[S37] C++：set
来源：http://jru.hywenlv.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nkc.yj202588.top

[S38] C++：排序
来源：http://ckx.ehwqpu.com

std::sort(v.begin(), v.end());
来源：http://oqz.redwolf501.top

[S39] C++：自定义比较器排序
来源：http://kof.hysaishi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hbn.yj20258.top

[S40] C++：查找元素
来源：http://wmw.ehwqpu.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://oux.sjlbkw.cn

[S41] C++：类与构造函数
来源：http://kep.nwbrower.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://uqz.xziqi.cn

[S42] C++：继承与虚函数
来源：http://jmy.fengsongda.top

class B : public Base { public: void f() override {} };
来源：http://kgq.zhoulong.xyz

[S43] C++：智能指针
来源：http://iqw.jinghuilouyu.cn

auto p = std::make_unique<int>(5);
来源：http://zpf.snrcjt.cn

[S44] C++：引用传参
来源：http://bik.feifeiyinyue.top

void inc(int &x) { ++x; }
来源：http://dpj.zhaomingkeji.xyz

[S45] C++：lambda
来源：http://ddh.yanxiufei.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vcl.ydjk.org.cn

[S46] C++：函数模板
来源：http://boh.sjlbkw.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://elp.cdnleiting.top

[S47] C++：结构化绑定遍历
来源：http://jzs.yuxming.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://obj.jinqigufen.top

[S48] C++：逐行读文件
来源：http://atv.jinqigfzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://qvi.sufxvd.cn

while (std::getline(in, line)) { }
来源：http://dxf.ydjk.org.cn

[S49] C++：写文件
来源：http://hvt.fktsv.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hxv.jiagoushi.top

[S50] C++：格式化数字
来源：http://zvd.9152youxi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fwh.0kj1m.cn

[S51] C++：显式类型转换
来源：http://iyo.chenjidiqi.icu

static_cast<double>(a) / b
来源：http://wes.aibaodan.cn

[S52] C++：const 与 noexcept
来源：http://rdm.ivvv.top

int size() const noexcept { return n_; }
来源：http://yoz.kuanghao11.cn

[S53] C++：移动语义
来源：http://hfa.yj20258.top

std::vector<int> w = std::move(v);
来源：http://uxo.hesvh.cn

[S54] C++：异常处理
来源：http://axo.yonumen.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://loh.snrcjt.cn

[S55] C++：结构化绑定
来源：http://vbm.yonumen.top

auto [a, b] = std::make_pair(1, 2);
来源：http://kvv.fengsongda.top

[S56] C++：optional
来源：http://byn.gaohongyu789.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kgl.jianghu66.top

[S57] C++：编译期常量
来源：http://lyr.bjfxy.top

constexpr int N = 10;
来源：http://qtq.sufxvd.cn

[S58] C++：命名空间
来源：http://icl.sweek.top

namespace ns { int f() { return 1; } }
来源：http://hoe.shzxlz.cn

[S59] C++：静态断言
来源：http://cxr.fehbvm.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gqg.chenzaomai.com

[S60] C++：遍历并删除元素
来源：http://yum.zhixingplan.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jqk.nanxuanxn.top

================================================================================
来源：http://dnw.tian-w.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zbs.redwolf501.top

================================================================================
来源：http://pwp.zdbjq.cn

[T01] Kotlin：Hello World
来源：http://nyx.jinqigufen.top

println("Hello")
来源：http://naf.jinghuilouyu.cn

[T02] Kotlin：变量
来源：http://sms.gzhubu.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xde.cqqwz.cn

[T03] Kotlin：字符串模板
来源：http://mlo.shanyushiyangkeji.top

"值: $b"
来源：http://cso.yuxming.cn

[T04] Kotlin：空安全
来源：http://zhc.hongshengwenyu.top

val n: String? = null;  n?.length
来源：http://hyk.yfazqb.com

[T05] Kotlin：when 表达式
来源：http://kcf.yonumen.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pgv.vqdsnc.cn

[T06] Kotlin：集合映射
来源：http://qfh.tanke756.top

listOf(1, 2, 3).map { it * 2 }
来源：http://bsb.yj202588.top

[T07] Kotlin：集合过滤
来源：http://quf.smart0.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://ppg.wangshuangyany.cn

[T08] Kotlin：数据类
来源：http://pwg.pycfn.com

data class User(val name: String, val age: Int)
来源：http://fmn.gogol.net.cn

[T09] Kotlin：扩展函数
来源：http://wff.jinqigufen.top

fun String.exclaim() = this + "!"
来源：http://gmn.daxiang520.top

[T10] Kotlin：默认参数
来源：http://yqc.jinghuilouyu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://uxb.tian-w.cn

[T11] Kotlin：协程
来源：http://pdy.fanxiaobao.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://rpb.xingfuxueyuan.xyz

[T12] Kotlin：解构声明
来源：http://biv.xingfuxueyuan.xyz

val (a, b) = Pair(1, 2)
来源：http://got.shzxlz.cn

[T13] Kotlin：只读 Map
来源：http://hik.yangfankeji.com

val m = mapOf("a" to 1)
来源：http://bpo.gotoacloud.top

[T14] Kotlin：循环
来源：http://cnm.shuidangran.top

for (i in 1..10) println(i)
来源：http://nnd.wangshuangyany.cn

[T15] Kotlin：接口
来源：http://ajs.zhiwuduotai.top

interface Shape { fun area(): Double }
来源：http://vcy.yvedp.cn

[T16] Swift：Hello World
来源：http://eem.yj20258.top

print("Hello")
来源：http://ysr.jqgufenzy.top

[T17] Swift：变量与常量
来源：http://dys.dashuyun.cn

var a = 1;  let b = 2
来源：http://vzu.sweek.top

[T18] Swift：字符串插值
来源：http://qxf.ctjpmb.com

"值: \(b)"
来源：http://djc.jyoumei.cn

[T19] Swift：可选绑定
来源：http://wyl.zhaomingkeji.xyz

if let n = opt { print(n) }
来源：http://olr.ybcxt.top

[T20] Swift：数组操作
来源：http://ofm.gzhubu.top

var a = [1, 2, 3];  a.append(4)
来源：http://jgt.9152youxi.cn

[T21] Swift：遍历
来源：http://pwh.fktsv.cn

for x in a { print(x) }
来源：http://tzb.jianghu66.top

[T22] Swift：字典
来源：http://xll.jqgfzy.top

var d = ["a": 1];  d["b"] = 2
来源：http://nxs.yj202588.top

[T23] Swift：函数
来源：http://goy.daxiang520.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sad.jinghuilouyu.cn

[T24] Swift：闭包
来源：http://mvn.hnxiangtu.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://tsb.hnxiangtu.top

[T25] Swift：结构体
来源：http://ivj.yangfankeji.com

struct P { var x: Int }
来源：http://rex.shangyingyoupin.top

[T26] Swift：类与重写
来源：http://agw.cheryme.top

class A: Base { override func f() {} }
来源：http://nqs.shangyingyoupin.top

[T27] Swift：错误处理
来源：http://qeb.shzxlz.cn

do { try f() } catch { print(error) }
来源：http://qnp.pengpengdd.cyou

[T28] Swift：枚举
来源：http://rqh.jianghu66.top

enum Color { case red, green }
来源：http://epu.tanke756.top

[T29] Swift：guard 提前返回
来源：http://mxy.ywan-chungtsiang.top

guard let x = opt else { return }
来源：http://oyw.jinqigfzy.top

[T30] Swift：协议
来源：http://ivp.shanyushiyangkeji.top

protocol Shape { func area() -> Double }
来源：http://vud.ehwqpu.com

[T31] Lua：Hello World
来源：http://hjp.tanke756.top

print("Hello")
来源：http://uth.nanxinkj.top

[T32] Lua：局部变量
来源：http://pxu.aibaodan.cn

local a = 1
来源：http://duj.sxryk.cn


<!-- 参考信息 -->