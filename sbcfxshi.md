代发 wailian999

files=$(ls -1)
来源：http://uft.zdbjq.cn

[R38] 管道串联
来源：http://uby.hfpthk.cn

cat a.txt | grep -i error | wc -l
来源：http://wyx.jqgfzy.top

[R39] 重定向标准输出与错误
来源：http://rhm.gaohongyu789.top

cmd > out.log 2>&1
来源：http://pvz.jinqigfzy.top

[R40] 追加写日志
来源：http://rih.kuanghao11.cn

echo "log" >> out.log
来源：http://fvi.andypj.xyz

[R41] 丢弃输出
来源：http://xha.52xcode.cn

cmd >/dev/null 2>&1
来源：http://nld.zhengqikj.top

[R42] 输入重定向
来源：http://xed.xinyue.icu

wc -l < a.txt
来源：http://qst.guowangkeji.top

[R43] 按名字查找文件
来源：http://coy.cdnleiting.top

find . -name "*.log" -type f
来源：http://qca.wangshuangyany.cn

[R44] 按修改时间查找
来源：http://tig.pycfn.com

find . -mtime -7 -type f
来源：http://sgc.zhongyouzk.top

[R45] 批量删除
来源：http://kli.hnqzz.top

find . -name "*.tmp" -delete
来源：http://sfq.shangyingyoupin.top

[R46] 递归替换文件内容
来源：http://jhs.epnwcf.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ndr.sysykeji.top

[R47] sed 单行替换
来源：http://qzs.yuxming.cn

sed -i 's/foo/bar/g' a.txt
来源：http://bwg.zhiwuduotai.top

[R48] awk 取指定列
来源：http://hhy.chenzaomai.com

awk '{print $1, $3}' a.txt
来源：http://znq.daria6918.cn

[R49] awk 带条件
来源：http://ryx.daria6918.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rvj.gaohongyu789.top

[R50] awk 求和
来源：http://dav.sysykeji.top

awk '{s += $2} END {print s}' a.txt
来源：http://fnm.xylfe.cn

[R51] 排序去重取前几
来源：http://syy.ydzc1.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ved.wangdashe.top

[R52] 统计行数
来源：http://imt.redwolf501.top

wc -l a.txt
来源：http://vnl.yongpay.top

[R53] 查看文件头与实时尾
来源：http://hah.tian-w.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kcg.gaohongyu789.top

[R54] 比较两个文件
来源：http://hgq.vqdsnc.cn

diff a.txt b.txt
来源：http://pxw.sweek.top

[R55] 压缩与解压
来源：http://ezf.jinghuilouyu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mhv.dashuyun.cn

[R56] 远程拷贝
来源：http://dok.sweek.top

scp file user@host:/path/
来源：http://afe.hfpthk.cn

[R57] 远程执行命令
来源：http://xxu.redwolf501.top

ssh user@host 'uptime'
来源：http://vxq.ywan-chungtsiang.top

[R58] 下载文件
来源：http://ayu.shangyingyoupin.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uua.yj202588.top

[R59] 发 POST JSON
来源：http://bso.wangdashe.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dgj.yj20258.top

[R60] 只看 HTTP 状态码
来源：http://bmx.aibaodan.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nsn.shzxlz.cn

[R61] 磁盘占用
来源：http://lgd.yuanzhike.top

df -h;  du -sh *
来源：http://fbi.xinyue.icu

[R62] 找最占空间的文件
来源：http://ucp.ctjpmb.com

du -ah . | sort -rh | head -10
来源：http://uqf.jinghuilouyu.cn

[R63] 内存与进程
来源：http://jwl.vehdjk.com

free -h;  ps aux | grep nginx
来源：http://itl.redwolf501.top

[R64] 结束进程
来源：http://ujo.tanke756.top

kill -9 $(pgrep -f app.py)
来源：http://icv.xuetiantiany.cn

[R65] 查看端口占用
来源：http://jbk.zdqjudy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gko.smart0.xyz

[R66] 定时任务
来源：http://piu.yvedp.cn

crontab -e;  crontab -l
来源：http://sde.ehwqpu.com

[R67] 生成随机十六进制串
来源：http://vww.haohaochexian.top

openssl rand -hex 16
来源：http://txc.kuanghao11.cn

[R68] 计算文件校验值
来源：http://wkg.yuxming.cn

sha256sum a.txt;  md5sum a.txt
来源：http://wun.vehdjk.com

[R69] 生成随机密码
来源：http://fkq.chenzaomai.com

head -c 16 /dev/urandom | base64
来源：http://bwq.uphjek.com

[R70] 时间戳与互转
来源：http://bjq.zhiwuduotai.top

date +%s;  date -d @1700000000
来源：http://eqx.jinqigfzy.top

[R71] 日期格式化
来源：http://czl.ydzc1.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://cvz.epnwcf.com

[R72] 等待端口就绪
来源：http://xgl.tianlin.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://yer.tarul.cn

[R73] 分割大日志
来源：http://zvb.birdmap.top

split -l 1000 big.log part_
来源：http://siq.cheryme.top

[R74] 批量重命名
来源：http://bxi.gotoacloud.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vfq.gotoacloud.top

[R75] 导出环境变量
来源：http://eaw.jinghuilouyu.cn

export PATH="$HOME/bin:$PATH"
来源：http://qzt.hongshengwenyu.top

[R76] 使用临时文件
来源：http://dcs.iojbl.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ngq.316326.xyz

[R77] 读取用户输入
来源：http://dqb.nwbrower.top

read -rp "请输入: " ans
来源：http://cdl.pengpengdd.cyou

[R78] 交互式菜单
来源：http://ntr.yj20258.top

select opt in a b c; do echo "$opt"; break; done
来源：http://boj.zhengqikj.top

[R79] 解析命令行选项
来源：http://uwd.chenlongwang.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bab.zhiwuduotai.top

[R80] 查看脚本执行耗时
来源：http://uec.ppjwa.cn

time ./run.sh
来源：http://uzf.ydjk.org.cn

================================================================================
来源：http://ohf.redwolf501.top

S. C / C++ 专题
来源：http://adw.c1oappe.top

================================================================================
来源：http://rwj.hnxiangtu.top

[S01] C：Hello World
来源：http://klr.cdnleiting.top

#include <stdio.h>
来源：http://zvf.xziqi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ugy.jqgfzy.top

[S02] C：变量与格式化输出
来源：http://pnu.aizwys.cn

int a = 10; printf("%d\n", a);
来源：http://lui.ivvv.top

[S03] C：读入整数
来源：http://jao.fengsongda.top

int x; scanf("%d", &x);
来源：http://xis.ybcxt.top

[S04] C：字符串复制
来源：http://paj.ybcxt.top

char dst[32]; strcpy(dst, "hi");
来源：http://oky.52xcode.cn

[S05] C：字符串长度
来源：http://hmd.hnxiangtu.top

strlen(s)
来源：http://kyi.ivvv.top

[S06] C：字符串比较
来源：http://iaj.jinqigufen.top

strcmp(a, b) == 0
来源：http://wyz.fzhhl.top

[S07] C：数组遍历求和
来源：http://par.tianlin.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ibz.zhixingplan.top

[S08] C：动态内存分配与释放
来源：http://vje.zhoulong.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://reh.jiagoushi.top

[S09] C：结构体定义与初始化
来源：http://zey.xziqi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cuu.wangshuangyany.cn

[S10] C：指针与解引用
来源：http://foo.daxiang520.top

int *p = &a;  *p = 5;
来源：http://mnd.wangshuangyany.cn

[S11] C：逐行读文件
来源：http://kyv.ywan-chungtsiang.top

FILE *f = fopen("a.txt", "r");
来源：http://roz.zhiwuduotai.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://fac.sjlbkw.cn

fclose(f);
来源：http://lvp.aizwys.cn

[S12] C：写文件
来源：http://sjz.yj20258.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tav.xziqi.cn

[S13] C：宏定义
来源：http://zuo.zhongyouzk.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tio.hcnkem.com

[S14] C：枚举
来源：http://ckk.zhongyouzk.top

enum Color { RED, GREEN, BLUE };
来源：http://awr.zdbjq.cn

[S15] C：类型转换
来源：http://ixp.tian-w.cn

(double) a / b
来源：http://bwl.xingfuxueyuan.xyz

[S16] C：位操作置位
来源：http://htc.sufxvd.cn

x |= (1 << 3);
来源：http://taj.shuidangran.top

[S17] C：安全拼接字符串
来源：http://ybi.shuidangran.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ycd.iojbl.cn

[S18] C：命令行参数
来源：http://yai.0kj1m.cn

int main(int argc, char **argv)
来源：http://ykx.tian-w.cn

[S19] C：快速排序
来源：http://bem.svipenyu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gso.cqqwz.cn

[S20] C：二分查找
来源：http://mvs.vqdsnc.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xll.xziqi.cn

[S21] C：字符类别判断
来源：http://mam.jianghu66.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://juf.ydjk.org.cn

[S22] C：字符串转数字
来源：http://bda.jqgfzy.top

atoi("42");  strtod("3.14", NULL);
来源：http://ztv.gzhubu.top

[S23] C：随机数
来源：http://kqz.ctjpmb.com

srand(time(NULL));  int r = rand() % 100;
来源：http://szj.jinyuanbaomall.cn

[S24] C：获取本地时间
来源：http://wdr.kuanghao11.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qdk.ppjwa.cn

[S25] C：内存拷贝
来源：http://wgc.dashuyun.cn

memcpy(dst, src, n);
来源：http://onm.feifeiyinyue.top

[S26] C：内存清零
来源：http://epz.daria6918.cn

memset(a, 0, sizeof a);
来源：http://yeq.hcnkem.com

[S27] C：定义常量
来源：http://zdz.cqqwz.cn

const double PI = 3.14159;
来源：http://byq.uphjek.com

[S28] C：静态变量
来源：http://gen.wangshuangyany.cn

static int counter = 0;
来源：http://pod.aizwys.cn

[S29] C：变参函数
来源：http://pex.cdnleiting.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nit.pycfn.com

[S30] C：头文件保护
来源：http://fte.shanyushiyangkeji.top

#ifndef X_H
来源：http://oww.jyoumei.cn

#define X_H
来源：http://qcu.yj20258888.top

#endif
来源：http://ept.quarkkingdee.top

[S31] C++：Hello World
来源：http://whj.nanxuanxn.top

#include <iostream>
来源：http://zao.havefunace.top

int main() { std::cout << "Hello\n"; }
来源：http://bsa.hnxiangtu.top

[S32] C++：字符串
来源：http://gsn.ivvv.top

std::string s = "hi";  s += "!";
来源：http://qfo.uphjek.com

[S33] C++：vector 增删
来源：http://cmc.feifeiyinyue.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mom.chenzaomai.com

[S34] C++：遍历 vector
来源：http://ecz.jinyuanbaomall.cn

for (auto &x : v) { std::cout << x; }
来源：http://ent.ivvv.top

[S35] C++：map
来源：http://hos.birdmap.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yqc.ivvv.top

[S36] C++：unordered_map
来源：http://vuc.ywan-chungtsiang.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bdu.xingfuxueyuan.xyz

[S37] C++：set
来源：http://rxq.ppjwa.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vvt.jinghuilouyu.cn

[S38] C++：排序
来源：http://ajn.hfpthk.cn

std::sort(v.begin(), v.end());
来源：http://qiy.gotoacloud.top

[S39] C++：自定义比较器排序
来源：http://hjx.sjlbkw.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zhb.zhoulong.xyz

[S40] C++：查找元素
来源：http://wmc.redwolf501.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hkb.yj20258888.top

[S41] C++：类与构造函数
来源：http://iyj.dianchejie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oom.cqqwz.cn

[S42] C++：继承与虚函数
来源：http://rzh.hcnkem.com

class B : public Base { public: void f() override {} };
来源：http://bvw.ppjwa.cn

[S43] C++：智能指针
来源：http://rxr.ydjk.org.cn

auto p = std::make_unique<int>(5);
来源：http://sks.xinyue.icu

[S44] C++：引用传参
来源：http://csj.sxryk.cn

void inc(int &x) { ++x; }
来源：http://fhw.ydjk.org.cn

[S45] C++：lambda
来源：http://ucm.hysaishi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fpi.cashguo.top

[S46] C++：函数模板
来源：http://exh.uphjek.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://itv.daria6918.cn

[S47] C++：结构化绑定遍历
来源：http://jim.xylfe.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ttc.tian-w.cn

[S48] C++：逐行读文件
来源：http://cdm.tanke756.top

std::ifstream in("a.txt");  std::string line;
来源：http://ppz.nanxinkj.top

while (std::getline(in, line)) { }
来源：http://tvk.hammf.cn

[S49] C++：写文件
来源：http://vvm.yuanzhike.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nfv.fengsongda.top

[S50] C++：格式化数字
来源：http://cxh.9152youxi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://aam.nwbrower.top

[S51] C++：显式类型转换
来源：http://qnh.xinyue.icu

static_cast<double>(a) / b
来源：http://zuj.52xcode.cn

[S52] C++：const 与 noexcept
来源：http://pjv.tanke756.top

int size() const noexcept { return n_; }
来源：http://bky.guannengcc.top

[S53] C++：移动语义
来源：http://cul.snrcjt.cn

std::vector<int> w = std::move(v);
来源：http://ide.cqqwz.cn

[S54] C++：异常处理
来源：http://oma.fktsv.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nng.yvedp.cn

[S55] C++：结构化绑定
来源：http://lmz.yfazqb.com

auto [a, b] = std::make_pair(1, 2);
来源：http://puf.tian-w.cn

[S56] C++：optional
来源：http://txu.zhijiandao.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://knf.vqdsnc.cn

[S57] C++：编译期常量
来源：http://pxd.hongshengwenyu.top

constexpr int N = 10;
来源：http://rbg.hcnkem.com

[S58] C++：命名空间
来源：http://ifr.yueranfly.top

namespace ns { int f() { return 1; } }
来源：http://aoq.iojbl.cn

[S59] C++：静态断言
来源：http://hiu.pycfn.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://waa.ehwqpu.com

[S60] C++：遍历并删除元素
来源：http://rvm.tian-w.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://exw.bbcook.cn

================================================================================
来源：http://nls.wangdashe.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://klz.hesvh.cn

================================================================================
来源：http://eli.andypj.xyz

[T01] Kotlin：Hello World
来源：http://ycg.nanxuanxn.top

println("Hello")
来源：http://dkg.sjlbkw.cn

[T02] Kotlin：变量
来源：http://iic.pengpengdd.cyou

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ddo.bbcook.cn

[T03] Kotlin：字符串模板
来源：http://djp.chenlongwang.top

"值: $b"
来源：http://kwt.jqgfzy.top

[T04] Kotlin：空安全
来源：http://vcz.jiagoushi.top

val n: String? = null;  n?.length
来源：http://ozb.sweek.top

[T05] Kotlin：when 表达式
来源：http://nor.shanyushiyangkeji.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://amd.iojbl.cn

[T06] Kotlin：集合映射
来源：http://zwd.bjfxy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://bxx.feifeiyinyue.top

[T07] Kotlin：集合过滤
来源：http://wnp.chenzaomai.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://jdh.snrcjt.cn

[T08] Kotlin：数据类
来源：http://bzd.cdnleiting.top

data class User(val name: String, val age: Int)
来源：http://ahm.yuxming.cn

[T09] Kotlin：扩展函数
来源：http://qrf.ehwqpu.com

fun String.exclaim() = this + "!"
来源：http://dlo.shanyushiyangtech.top

[T10] Kotlin：默认参数
来源：http://gou.jinqigfzy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://mfg.vehdjk.com

[T11] Kotlin：协程
来源：http://mxo.zdqjudy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://mbd.cashguo.top

[T12] Kotlin：解构声明
来源：http://xwx.yuanzhike.top

val (a, b) = Pair(1, 2)
来源：http://kck.0kj1m.cn

[T13] Kotlin：只读 Map
来源：http://idv.sxryk.cn

val m = mapOf("a" to 1)
来源：http://qwq.gotoacloud.top

[T14] Kotlin：循环
来源：http://ugn.chenjidiqi.icu

for (i in 1..10) println(i)
来源：http://ieb.nanxuanxn.top

[T15] Kotlin：接口
来源：http://xnx.zhengqikj.top

interface Shape { fun area(): Double }
来源：http://bud.jinghuilouyu.cn

[T16] Swift：Hello World
来源：http://kgw.yfazqb.com

print("Hello")
来源：http://brx.wangshuangyany.cn

[T17] Swift：变量与常量
来源：http://yvv.chenjidiqi.icu

var a = 1;  let b = 2
来源：http://pmw.shangyingyoupin.top

[T18] Swift：字符串插值
来源：http://xir.shuidangran.top

"值: \(b)"
来源：http://iol.ivvv.top

[T19] Swift：可选绑定
来源：http://fcz.jinyuanbaomall.cn

if let n = opt { print(n) }
来源：http://dds.fzhhl.top

[T20] Swift：数组操作
来源：http://xhp.sweek.top

var a = [1, 2, 3];  a.append(4)
来源：http://oqf.hnqzz.top

[T21] Swift：遍历
来源：http://bki.xuetiantiany.cn

for x in a { print(x) }
来源：http://klr.dianchejie.cn

[T22] Swift：字典
来源：http://jho.zhengqikj.top

var d = ["a": 1];  d["b"] = 2
来源：http://lbp.hcnkem.com

[T23] Swift：函数
来源：http://ovx.ctjpmb.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sec.sysykeji.top

[T24] Swift：闭包
来源：http://ouf.aibaodan.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gqs.sweek.top

[T25] Swift：结构体
来源：http://djn.yongpay.top

struct P { var x: Int }
来源：http://fbf.nanxinkj.top

[T26] Swift：类与重写
来源：http://awv.sxryk.cn

class A: Base { override func f() {} }
来源：http://meu.kuanghao11.cn

[T27] Swift：错误处理
来源：http://xnz.guowangkeji.top

do { try f() } catch { print(error) }
来源：http://tzv.hnxiangtu.top

[T28] Swift：枚举
来源：http://pid.snrcjt.cn

enum Color { case red, green }
来源：http://jyx.hfpthk.cn

[T29] Swift：guard 提前返回
来源：http://skm.ydjk.org.cn

guard let x = opt else { return }
来源：http://ssf.zdqjudy.top

[T30] Swift：协议
来源：http://sas.ivvv.top

protocol Shape { func area() -> Double }
来源：http://ydb.xuetiantiany.cn

[T31] Lua：Hello World
来源：http://bio.dianchejie.cn

print("Hello")
来源：http://zce.jinyuanbaomall.cn

[T32] Lua：局部变量
来源：http://irt.yvedp.cn

local a = 1
来源：http://isu.pycfn.com

[T33] Lua：表（数组）
来源：http://say.hnxiangtu.top

local t = {1, 2, 3};  t[4] = 4
来源：http://oam.jinyuanbaomall.cn

[T34] Lua：遍历表
来源：http://ikr.guannengcc.top

for i, v in ipairs(t) do print(i, v) end
来源：http://yno.chenlongwang.top

[T35] Lua：字典表
来源：http://mog.ywan-chungtsiang.top

local d = { a = 1 };  d.b = 2
来源：http://dpl.xylfe.cn

[T36] Lua：函数
来源：http://gao.fengsongda.top

function add(a, b) return a + b end
来源：http://dvf.jinyuanbaomall.cn

[T37] Lua：字符串拼接
来源：http://uqh.jinyuanbaomall.cn

"a" .. "b"
来源：http://bcc.tianlin.xyz

[T38] Lua：条件
来源：http://wtp.smart0.xyz

if x > 0 then print("正") end
来源：http://ndg.ppjwa.cn

[T39] Lua：模式匹配
来源：http://csz.smart0.xyz

string.find(s, "%d+")
来源：http://mqo.gogol.net.cn

[T40] Lua：元表
来源：http://nqm.guannengcc.top

setmetatable({}, { __index = base })
来源：http://iyn.jinqigufen.top


<!-- 参考信息 -->