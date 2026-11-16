代发 wailian999

echo $((1 + 2 * 3))
来源：http://fcv.guannengcc.top

[R28] 浮点运算
来源：http://hsc.haohaochexian.top

echo "scale=2; 10/3" | bc
来源：http://uyq.guowangkeji.top

[R29] 定义函数
来源：http://iew.fzhhl.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://inw.shanyushiyangkeji.top

[R30] 函数返回状态码
来源：http://ldg.epnwcf.com

f() { return 0; }; f || echo "失败了"
来源：http://cxh.dianchejie.cn

[R31] 局部变量
来源：http://zwa.gotoacloud.top

f() { local x=1; echo "$x"; }
来源：http://phu.bbcook.cn

[R32] 参数个数校验
来源：http://xnm.9152youxi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://une.0kj1m.cn

[R33] 捕获错误并提示行号
来源：http://xsj.svipenyu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jgq.quarkkingdee.top

[R34] 退出时清理
来源：http://sjn.svipenyu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://zeu.quarkkingdee.top

[R35] 后台执行并等待
来源：http://bko.jinyuanbaomall.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://nce.yonumen.top

[R36] 并发执行多个任务
来源：http://qno.yonumen.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rnu.hongshengwenyu.top

[R37] 把输出赋给变量
来源：http://ezq.pengpengdd.cyou

files=$(ls -1)
来源：http://jap.hesvh.cn

[R38] 管道串联
来源：http://lvo.tianlin.xyz

cat a.txt | grep -i error | wc -l
来源：http://kdz.yfazqb.com

[R39] 重定向标准输出与错误
来源：http://twv.hongshengwenyu.top

cmd > out.log 2>&1
来源：http://rvr.yj20258.top

[R40] 追加写日志
来源：http://vms.meibo888.top

echo "log" >> out.log
来源：http://ivl.hysaishi.cn

[R41] 丢弃输出
来源：http://rcu.smart0.xyz

cmd >/dev/null 2>&1
来源：http://xkm.feifeiyinyue.top

[R42] 输入重定向
来源：http://gwu.tanke756.top

wc -l < a.txt
来源：http://lli.daxiang520.top

[R43] 按名字查找文件
来源：http://age.jiagoushi.top

find . -name "*.log" -type f
来源：http://qhr.dashuyun.cn

[R44] 按修改时间查找
来源：http://oma.jiagoushi.top

find . -mtime -7 -type f
来源：http://aue.gogol.net.cn

[R45] 批量删除
来源：http://gfz.daria6918.cn

find . -name "*.tmp" -delete
来源：http://mmw.pycfn.com

[R46] 递归替换文件内容
来源：http://yfb.andypj.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bxt.nanxinkj.top

[R47] sed 单行替换
来源：http://rzr.zhaomingkeji.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://akm.shangyingyoupin.top

[R48] awk 取指定列
来源：http://gui.ppjwa.cn

awk '{print $1, $3}' a.txt
来源：http://ueu.hcnkem.com

[R49] awk 带条件
来源：http://kbw.gzhubu.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nun.daxiang520.top

[R50] awk 求和
来源：http://ktq.fehbvm.com

awk '{s += $2} END {print s}' a.txt
来源：http://mwx.xuetiantiany.cn

[R51] 排序去重取前几
来源：http://puj.hywenlv.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://tww.ivvv.top

[R52] 统计行数
来源：http://muf.nwbrower.top

wc -l a.txt
来源：http://uio.zhiwuduotai.top

[R53] 查看文件头与实时尾
来源：http://ggo.chenjidiqi.icu

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dad.feifeiyinyue.top

[R54] 比较两个文件
来源：http://yzi.jinqigufen.top

diff a.txt b.txt
来源：http://sxv.smart0.xyz

[R55] 压缩与解压
来源：http://cna.nwbrower.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ngn.chenjidiqi.icu

[R56] 远程拷贝
来源：http://bkq.wangshuangyany.cn

scp file user@host:/path/
来源：http://vpm.316326.xyz

[R57] 远程执行命令
来源：http://aif.svipenyu.cn

ssh user@host 'uptime'
来源：http://lha.jinqigufen.top

[R58] 下载文件
来源：http://ylu.aibaodan.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nyf.haohaochexian.top

[R59] 发 POST JSON
来源：http://ush.aibaodan.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lmg.mhx1999.top

[R60] 只看 HTTP 状态码
来源：http://tgs.zhengqikj.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ytt.dashuyun.cn

[R61] 磁盘占用
来源：http://kcj.andypj.xyz

df -h;  du -sh *
来源：http://vto.yj20258888.top

[R62] 找最占空间的文件
来源：http://bqc.tian-w.cn

du -ah . | sort -rh | head -10
来源：http://nvn.epnwcf.com

[R63] 内存与进程
来源：http://fcj.hysaishi.cn

free -h;  ps aux | grep nginx
来源：http://cwo.chenjidiqi.icu

[R64] 结束进程
来源：http://jia.redwolf501.top

kill -9 $(pgrep -f app.py)
来源：http://kmv.shanyushiyangtech.top

[R65] 查看端口占用
来源：http://xmt.fanxiaobao.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ein.cucudq.cn

[R66] 定时任务
来源：http://ezq.sxryk.cn

crontab -e;  crontab -l
来源：http://irm.0kj1m.cn

[R67] 生成随机十六进制串
来源：http://ghs.wangshuangyany.cn

openssl rand -hex 16
来源：http://sah.shangyingyoupin.top

[R68] 计算文件校验值
来源：http://waq.ydzc1.top

sha256sum a.txt;  md5sum a.txt
来源：http://duv.yueranfly.top

[R69] 生成随机密码
来源：http://dbf.kuanghao11.cn

head -c 16 /dev/urandom | base64
来源：http://cba.hcnkem.com

[R70] 时间戳与互转
来源：http://nzy.cqqwz.cn

date +%s;  date -d @1700000000
来源：http://ppq.chenjidiqi.icu

[R71] 日期格式化
来源：http://wuc.birdmap.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ghn.jinghuilouyu.cn

[R72] 等待端口就绪
来源：http://fzv.wangdashe.top

until nc -z localhost 3306; do sleep 1; done
来源：http://glj.yj20258.top

[R73] 分割大日志
来源：http://tpz.haohaochexian.top

split -l 1000 big.log part_
来源：http://rrh.hfpthk.cn

[R74] 批量重命名
来源：http://zrd.cucudq.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yjn.chenzaomai.com

[R75] 导出环境变量
来源：http://lsn.0kj1m.cn

export PATH="$HOME/bin:$PATH"
来源：http://fmx.nanxinkj.top

[R76] 使用临时文件
来源：http://zyl.zhaomingkeji.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nrv.yueranfly.top

[R77] 读取用户输入
来源：http://khx.ywan-chungtsiang.top

read -rp "请输入: " ans
来源：http://dgw.meibo888.top

[R78] 交互式菜单
来源：http://jnw.jlsjyb.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://idl.aibaodan.cn

[R79] 解析命令行选项
来源：http://aww.yvedp.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rdo.daxiang520.top

[R80] 查看脚本执行耗时
来源：http://uza.shanyushiyangkeji.top

time ./run.sh
来源：http://nmo.xuanzx.com

================================================================================
来源：http://owi.xylfe.cn

S. C / C++ 专题
来源：http://nkj.birdmap.top

================================================================================
来源：http://npn.jiagoushi.top

[S01] C：Hello World
来源：http://luy.vqdsnc.cn

#include <stdio.h>
来源：http://rcd.yj20258.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://cmh.gotoacloud.top

[S02] C：变量与格式化输出
来源：http://mqo.hfpthk.cn

int a = 10; printf("%d\n", a);
来源：http://dzd.shzxlz.cn

[S03] C：读入整数
来源：http://wks.zdbjq.cn

int x; scanf("%d", &x);
来源：http://urm.gaohongyu789.top

[S04] C：字符串复制
来源：http://xay.yfazqb.com

char dst[32]; strcpy(dst, "hi");
来源：http://gho.wangshuangyany.cn

[S05] C：字符串长度
来源：http://scy.yangfankeji.com

strlen(s)
来源：http://off.ydjk.org.cn

[S06] C：字符串比较
来源：http://yvu.hnqzz.top

strcmp(a, b) == 0
来源：http://hna.andypj.xyz

[S07] C：数组遍历求和
来源：http://hvx.quarkkingdee.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kzn.nanxinkj.top

[S08] C：动态内存分配与释放
来源：http://gob.cdnleiting.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cdo.sysykeji.top

[S09] C：结构体定义与初始化
来源：http://max.sxryk.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wul.yfazqb.com

[S10] C：指针与解引用
来源：http://zfc.meibo888.top

int *p = &a;  *p = 5;
来源：http://lij.jianghu66.top

[S11] C：逐行读文件
来源：http://rhh.quarkkingdee.top

FILE *f = fopen("a.txt", "r");
来源：http://vnh.hnxiangtu.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://wpw.cashguo.top

fclose(f);
来源：http://rwi.zhixingplan.top

[S12] C：写文件
来源：http://cvr.haohaochexian.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gkg.nanxinkj.top

[S13] C：宏定义
来源：http://tzq.yj202588.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rem.hammf.cn

[S14] C：枚举
来源：http://yyu.xziqi.cn

enum Color { RED, GREEN, BLUE };
来源：http://kes.birdmap.top

[S15] C：类型转换
来源：http://tnk.fzhhl.top

(double) a / b
来源：http://tvo.tianlin.xyz

[S16] C：位操作置位
来源：http://lwk.vqdsnc.cn

x |= (1 << 3);
来源：http://iin.xziqi.cn

[S17] C：安全拼接字符串
来源：http://tgj.hammf.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rcv.jqgufenzy.top

[S18] C：命令行参数
来源：http://pnx.nwbrower.top

int main(int argc, char **argv)
来源：http://pbn.52xcode.cn

[S19] C：快速排序
来源：http://dct.haohaochexian.top

qsort(a, n, sizeof(int), cmp);
来源：http://ynx.quarkkingdee.top

[S20] C：二分查找
来源：http://bzj.wangshuangyany.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ggk.shanyushiyangkeji.top

[S21] C：字符类别判断
来源：http://uri.zhoulong.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kzy.fengsongda.top

[S22] C：字符串转数字
来源：http://qbo.ybcxt.top

atoi("42");  strtod("3.14", NULL);
来源：http://dvp.gzhubu.top

[S23] C：随机数
来源：http://imp.quarkkingdee.top

srand(time(NULL));  int r = rand() % 100;
来源：http://cxa.hnqzz.top

[S24] C：获取本地时间
来源：http://tkg.hnxiangtu.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wze.yueranfly.top

[S25] C：内存拷贝
来源：http://vho.zdqjudy.top

memcpy(dst, src, n);
来源：http://tfu.jianghu66.top

[S26] C：内存清零
来源：http://rvc.zhiwuduotai.top

memset(a, 0, sizeof a);
来源：http://xfu.feifeiyinyue.top

[S27] C：定义常量
来源：http://ghs.meibo888.top

const double PI = 3.14159;
来源：http://coh.yonumen.top

[S28] C：静态变量
来源：http://ybw.ywan-chungtsiang.top

static int counter = 0;
来源：http://glo.aibaodan.cn

[S29] C：变参函数
来源：http://qsa.birdmap.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mgc.yj20258.top

[S30] C：头文件保护
来源：http://hif.daria6918.cn

#ifndef X_H
来源：http://vop.xuanzx.com

#define X_H
来源：http://ahr.zdqjudy.top

#endif
来源：http://ygj.yj20258888.top

[S31] C++：Hello World
来源：http://hun.ivvv.top

#include <iostream>
来源：http://tlx.gaohongyu789.top

int main() { std::cout << "Hello\n"; }
来源：http://rkv.yonumen.top

[S32] C++：字符串
来源：http://aia.shuidangran.top

std::string s = "hi";  s += "!";
来源：http://tqk.jqgfzy.top

[S33] C++：vector 增删
来源：http://kzh.pengpengdd.cyou

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ual.epnwcf.com

[S34] C++：遍历 vector
来源：http://rfc.shanyushiyangtech.top

for (auto &x : v) { std::cout << x; }
来源：http://lfi.bjfxy.top

[S35] C++：map
来源：http://ifk.sufxvd.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://msm.aizwys.cn

[S36] C++：unordered_map
来源：http://uyg.jqgfzy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://avq.zhongyouzk.top

[S37] C++：set
来源：http://dcf.52xcode.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vqc.gaohongyu789.top

[S38] C++：排序
来源：http://khl.feifeiyinyue.top

std::sort(v.begin(), v.end());
来源：http://qum.daxiang520.top

[S39] C++：自定义比较器排序
来源：http://ngw.fengsongda.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rpi.dashuyun.cn

[S40] C++：查找元素
来源：http://tza.c1oappe.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bif.0kj1m.cn

[S41] C++：类与构造函数
来源：http://czr.xuetiantiany.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dgn.shuidangran.top

[S42] C++：继承与虚函数
来源：http://quz.ehwqpu.com

class B : public Base { public: void f() override {} };
来源：http://hau.sjlbkw.cn

[S43] C++：智能指针
来源：http://lhq.xinyue.icu

auto p = std::make_unique<int>(5);
来源：http://hes.jyoumei.cn

[S44] C++：引用传参
来源：http://nqb.ppjwa.cn

void inc(int &x) { ++x; }
来源：http://cuz.hongshengwenyu.top

[S45] C++：lambda
来源：http://ise.bbcook.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qil.yanxiufei.cn

[S46] C++：函数模板
来源：http://jip.dianchejie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dca.ywan-chungtsiang.top

[S47] C++：结构化绑定遍历
来源：http://wue.fengsongda.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xpt.cqqwz.cn

[S48] C++：逐行读文件
来源：http://omt.hammf.cn

std::ifstream in("a.txt");  std::string line;
来源：http://cqf.zhiwuduotai.top

while (std::getline(in, line)) { }
来源：http://vsj.shzxlz.cn

[S49] C++：写文件
来源：http://lwu.sysykeji.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jtg.fktsv.cn

[S50] C++：格式化数字
来源：http://hpa.havefunace.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nnm.zhoulong.xyz

[S51] C++：显式类型转换
来源：http://jxz.shanyushiyangkeji.top

static_cast<double>(a) / b
来源：http://yet.jqgfzy.top

[S52] C++：const 与 noexcept
来源：http://cqn.sufxvd.cn

int size() const noexcept { return n_; }
来源：http://cxb.zhixingplan.top

[S53] C++：移动语义
来源：http://wpt.sysykeji.top

std::vector<int> w = std::move(v);
来源：http://mfj.yj202588.top

[S54] C++：异常处理
来源：http://fnc.ctjpmb.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fce.jinghuilouyu.cn

[S55] C++：结构化绑定
来源：http://mnm.nanxinkj.top

auto [a, b] = std::make_pair(1, 2);
来源：http://qxn.iojbl.cn

[S56] C++：optional
来源：http://qmc.cheryme.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hbh.snrcjt.cn

[S57] C++：编译期常量
来源：http://dbm.yanxiufei.cn

constexpr int N = 10;
来源：http://ghg.jinghuilouyu.cn

[S58] C++：命名空间
来源：http://qro.yj20258888.top

namespace ns { int f() { return 1; } }
来源：http://hqw.cashguo.top

[S59] C++：静态断言
来源：http://iyg.yuxming.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zrn.snrcjt.cn

[S60] C++：遍历并删除元素
来源：http://aes.yongpay.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tty.sysykeji.top

================================================================================
来源：http://rzm.wangdashe.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uae.sjlbkw.cn

================================================================================
来源：http://pep.kuanghao11.cn

[T01] Kotlin：Hello World
来源：http://hdx.vqdsnc.cn

println("Hello")
来源：http://mbf.yj20258.top

[T02] Kotlin：变量
来源：http://mxn.sxryk.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gnf.birdmap.top

[T03] Kotlin：字符串模板
来源：http://jer.feifeiyinyue.top

"值: $b"
来源：http://nnt.uphjek.com

[T04] Kotlin：空安全
来源：http://tbj.zhaomingkeji.xyz

val n: String? = null;  n?.length
来源：http://sdo.dianchejie.cn

[T05] Kotlin：when 表达式
来源：http://vnn.0kj1m.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mcc.316326.xyz

[T06] Kotlin：集合映射
来源：http://owm.cdnleiting.top

listOf(1, 2, 3).map { it * 2 }
来源：http://pis.hnqzz.top

[T07] Kotlin：集合过滤
来源：http://cpm.yangfankeji.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://zph.zhixingplan.top

[T08] Kotlin：数据类
来源：http://qxp.zdbjq.cn

data class User(val name: String, val age: Int)
来源：http://ihy.wangshuangyany.cn

[T09] Kotlin：扩展函数
来源：http://lyw.9152youxi.cn

fun String.exclaim() = this + "!"
来源：http://tnh.gaohongyu789.top

[T10] Kotlin：默认参数
来源：http://oww.mhx1999.top

fun greet(name: String = "World") = "Hi $name"
来源：http://wtb.nwbrower.top

[T11] Kotlin：协程
来源：http://yxa.cashguo.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://pvm.tian-w.cn

[T12] Kotlin：解构声明
来源：http://jjm.shanyushiyangkeji.top

val (a, b) = Pair(1, 2)
来源：http://pfr.sysykeji.top

[T13] Kotlin：只读 Map
来源：http://tvt.yuanzhike.top

val m = mapOf("a" to 1)
来源：http://cyf.ppjwa.cn

[T14] Kotlin：循环
来源：http://byr.bbcook.cn

for (i in 1..10) println(i)
来源：http://owd.sxryk.cn

[T15] Kotlin：接口
来源：http://jyd.gaohongyu789.top

interface Shape { fun area(): Double }
来源：http://lvr.guowangkeji.top

[T16] Swift：Hello World
来源：http://jmn.zhixingplan.top

print("Hello")
来源：http://mlt.gogol.net.cn

[T17] Swift：变量与常量
来源：http://pgv.wangdashe.top

var a = 1;  let b = 2
来源：http://alt.hysaishi.cn

[T18] Swift：字符串插值
来源：http://rcc.redwolf501.top

"值: \(b)"
来源：http://ebo.bjfxy.top

[T19] Swift：可选绑定
来源：http://edj.pycfn.com

if let n = opt { print(n) }
来源：http://pfw.uphjek.com

[T20] Swift：数组操作
来源：http://etx.fengsongda.top

var a = [1, 2, 3];  a.append(4)
来源：http://rgl.hesvh.cn

[T21] Swift：遍历
来源：http://tsf.chenzaomai.com

for x in a { print(x) }
来源：http://bte.hongshengwenyu.top

[T22] Swift：字典
来源：http://pml.aizwys.cn

var d = ["a": 1];  d["b"] = 2
来源：http://lpc.yuanzhike.top

[T23] Swift：函数
来源：http://fre.mhx1999.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nhe.wangdashe.top

[T24] Swift：闭包
来源：http://hgn.c1oappe.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://joj.aizwys.cn

[T25] Swift：结构体
来源：http://hxu.bjfxy.top

struct P { var x: Int }
来源：http://zoz.yonumen.top

[T26] Swift：类与重写
来源：http://aad.yonumen.top

class A: Base { override func f() {} }
来源：http://hnm.yfazqb.com

[T27] Swift：错误处理
来源：http://ibn.fanxiaobao.xyz

do { try f() } catch { print(error) }
来源：http://dbe.zhengqikj.top

[T28] Swift：枚举
来源：http://dhy.wangdashe.top

enum Color { case red, green }
来源：http://oko.zhaomingkeji.xyz

[T29] Swift：guard 提前返回
来源：http://isk.snrcjt.cn

guard let x = opt else { return }
来源：http://jyz.yj20258888.top

[T30] Swift：协议
来源：http://nhy.havefunace.top

protocol Shape { func area() -> Double }
来源：http://gxr.yj20258.top


<!-- 参考信息 -->