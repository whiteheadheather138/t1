代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://mub.guowangkeji.top

[R32] 参数个数校验
来源：http://rkm.feifeiyinyue.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ydi.shangyingyoupin.top

[R33] 捕获错误并提示行号
来源：http://ttm.ivvv.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fkm.ydzc1.top

[R34] 退出时清理
来源：http://vpv.aizwys.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ati.fktsv.cn

[R35] 后台执行并等待
来源：http://ehn.gaohongyu789.top

sleep 5 & pid=$!; wait "$pid"
来源：http://eqx.yanxiufei.cn

[R36] 并发执行多个任务
来源：http://jxk.hysaishi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://esz.yj20258.top

[R37] 把输出赋给变量
来源：http://ulg.ybcxt.top

files=$(ls -1)
来源：http://dwq.quarkkingdee.top

[R38] 管道串联
来源：http://dnp.cashguo.top

cat a.txt | grep -i error | wc -l
来源：http://uit.fanxiaobao.xyz

[R39] 重定向标准输出与错误
来源：http://arz.316326.xyz

cmd > out.log 2>&1
来源：http://qjq.kuanghao11.cn

[R40] 追加写日志
来源：http://qbu.hcnkem.com

echo "log" >> out.log
来源：http://peg.xuanzx.com

[R41] 丢弃输出
来源：http://gnr.yj20258888.top

cmd >/dev/null 2>&1
来源：http://syp.nwbrower.top

[R42] 输入重定向
来源：http://rxy.zhengqikj.top

wc -l < a.txt
来源：http://ppo.pengpengdd.cyou

[R43] 按名字查找文件
来源：http://unt.yueranfly.top

find . -name "*.log" -type f
来源：http://afg.feifeiyinyue.top

[R44] 按修改时间查找
来源：http://vbt.andypj.xyz

find . -mtime -7 -type f
来源：http://rod.shangyingyoupin.top

[R45] 批量删除
来源：http://ahq.jyoumei.cn

find . -name "*.tmp" -delete
来源：http://wmz.xuetiantiany.cn

[R46] 递归替换文件内容
来源：http://ffe.hysaishi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kxe.c1oappe.top

[R47] sed 单行替换
来源：http://bry.ydjk.org.cn

sed -i 's/foo/bar/g' a.txt
来源：http://psq.cqqwz.cn

[R48] awk 取指定列
来源：http://dyv.cdnleiting.top

awk '{print $1, $3}' a.txt
来源：http://vrw.0kj1m.cn

[R49] awk 带条件
来源：http://zcf.chenzaomai.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://swc.hcnkem.com

[R50] awk 求和
来源：http://ftk.hammf.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bwg.tanke756.top

[R51] 排序去重取前几
来源：http://gmo.jinyuanbaomall.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://oll.jlsjyb.cn

[R52] 统计行数
来源：http://lsk.xuanzx.com

wc -l a.txt
来源：http://byr.quarkkingdee.top

[R53] 查看文件头与实时尾
来源：http://nle.jqgfzy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jgv.sysykeji.top

[R54] 比较两个文件
来源：http://zex.tianlin.xyz

diff a.txt b.txt
来源：http://org.yueranfly.top

[R55] 压缩与解压
来源：http://nxa.yuxming.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ick.tanke756.top

[R56] 远程拷贝
来源：http://wsy.meibo888.top

scp file user@host:/path/
来源：http://ktm.ybcxt.top

[R57] 远程执行命令
来源：http://xjn.fehbvm.com

ssh user@host 'uptime'
来源：http://dek.9152youxi.cn

[R58] 下载文件
来源：http://mrr.feifeiyinyue.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fto.havefunace.top

[R59] 发 POST JSON
来源：http://rmg.yvedp.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zxm.9152youxi.cn

[R60] 只看 HTTP 状态码
来源：http://rwg.gotoacloud.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dyf.shzxlz.cn

[R61] 磁盘占用
来源：http://bif.dashuyun.cn

df -h;  du -sh *
来源：http://ehu.snrcjt.cn

[R62] 找最占空间的文件
来源：http://tul.chenlongwang.top

du -ah . | sort -rh | head -10
来源：http://pln.jinqigfzy.top

[R63] 内存与进程
来源：http://has.meibo888.top

free -h;  ps aux | grep nginx
来源：http://jje.xziqi.cn

[R64] 结束进程
来源：http://obh.hcnkem.com

kill -9 $(pgrep -f app.py)
来源：http://zou.cucudq.cn

[R65] 查看端口占用
来源：http://iqt.smart0.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pah.meibo888.top

[R66] 定时任务
来源：http://ios.yvedp.cn

crontab -e;  crontab -l
来源：http://acx.jqgfzy.top

[R67] 生成随机十六进制串
来源：http://sta.jyoumei.cn

openssl rand -hex 16
来源：http://xpv.yj20258888.top

[R68] 计算文件校验值
来源：http://qdt.fehbvm.com

sha256sum a.txt;  md5sum a.txt
来源：http://jnn.iojbl.cn

[R69] 生成随机密码
来源：http://qpy.tian-w.cn

head -c 16 /dev/urandom | base64
来源：http://sig.sufxvd.cn

[R70] 时间戳与互转
来源：http://bsd.xuetiantiany.cn

date +%s;  date -d @1700000000
来源：http://gum.ivvv.top

[R71] 日期格式化
来源：http://wei.birdmap.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://rne.yuanzhike.top

[R72] 等待端口就绪
来源：http://lfi.xuetiantiany.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://esl.zhijiandao.cn

[R73] 分割大日志
来源：http://pix.cheryme.top

split -l 1000 big.log part_
来源：http://ttg.zdqjudy.top

[R74] 批量重命名
来源：http://dke.vqdsnc.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lao.hfpthk.cn

[R75] 导出环境变量
来源：http://qra.nwbrower.top

export PATH="$HOME/bin:$PATH"
来源：http://imo.tianlin.xyz

[R76] 使用临时文件
来源：http://fjq.andypj.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://klq.hfpthk.cn

[R77] 读取用户输入
来源：http://mpo.yuxming.cn

read -rp "请输入: " ans
来源：http://ceg.yfazqb.com

[R78] 交互式菜单
来源：http://txb.yuxming.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ekq.fktsv.cn

[R79] 解析命令行选项
来源：http://vlz.snrcjt.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://roi.gogol.net.cn

[R80] 查看脚本执行耗时
来源：http://ljt.fengsongda.top

time ./run.sh
来源：http://djf.hcnkem.com

================================================================================
来源：http://pih.shanyushiyangtech.top

S. C / C++ 专题
来源：http://xvi.pycfn.com

================================================================================
来源：http://bro.chenjidiqi.icu

[S01] C：Hello World
来源：http://adk.cheryme.top

#include <stdio.h>
来源：http://zig.jiagoushi.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://czb.yangfankeji.com

[S02] C：变量与格式化输出
来源：http://nbr.tian-w.cn

int a = 10; printf("%d\n", a);
来源：http://ztk.fengsongda.top

[S03] C：读入整数
来源：http://ebh.ydjk.org.cn

int x; scanf("%d", &x);
来源：http://yir.yangfankeji.com

[S04] C：字符串复制
来源：http://siz.birdmap.top

char dst[32]; strcpy(dst, "hi");
来源：http://cfv.tian-w.cn

[S05] C：字符串长度
来源：http://gob.hesvh.cn

strlen(s)
来源：http://gsi.shanyushiyangkeji.top

[S06] C：字符串比较
来源：http://ucn.wangdashe.top

strcmp(a, b) == 0
来源：http://jgy.zhoulong.xyz

[S07] C：数组遍历求和
来源：http://gda.meibo888.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wpj.yj20258.top

[S08] C：动态内存分配与释放
来源：http://aoq.jqgfzy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mer.xuetiantiany.cn

[S09] C：结构体定义与初始化
来源：http://dhb.epnwcf.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pxb.bjfxy.top

[S10] C：指针与解引用
来源：http://vrd.daxiang520.top

int *p = &a;  *p = 5;
来源：http://djx.tianlin.xyz

[S11] C：逐行读文件
来源：http://guw.bjfxy.top

FILE *f = fopen("a.txt", "r");
来源：http://dlc.c1oappe.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://pao.jianghu66.top

fclose(f);
来源：http://igx.shangyingyoupin.top

[S12] C：写文件
来源：http://rdz.gogol.net.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://twk.shanyushiyangkeji.top

[S13] C：宏定义
来源：http://mdq.cqqwz.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://quw.cqqwz.cn

[S14] C：枚举
来源：http://jmc.havefunace.top

enum Color { RED, GREEN, BLUE };
来源：http://xal.yongpay.top

[S15] C：类型转换
来源：http://lga.yj202588.top

(double) a / b
来源：http://hun.xylfe.cn

[S16] C：位操作置位
来源：http://mwb.hammf.cn

x |= (1 << 3);
来源：http://ddc.ywan-chungtsiang.top

[S17] C：安全拼接字符串
来源：http://sie.hnxiangtu.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dwy.daria6918.cn

[S18] C：命令行参数
来源：http://wrj.fzhhl.top

int main(int argc, char **argv)
来源：http://hju.hysaishi.cn

[S19] C：快速排序
来源：http://uey.hysaishi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://kvv.yongpay.top

[S20] C：二分查找
来源：http://bpf.316326.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gdf.sufxvd.cn

[S21] C：字符类别判断
来源：http://uva.tarul.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://atb.zhengqikj.top

[S22] C：字符串转数字
来源：http://oni.chenzaomai.com

atoi("42");  strtod("3.14", NULL);
来源：http://lff.zhongyouzk.top

[S23] C：随机数
来源：http://fmw.yueranfly.top

srand(time(NULL));  int r = rand() % 100;
来源：http://djy.jinqigfzy.top

[S24] C：获取本地时间
来源：http://jtg.shzxlz.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pqq.ywan-chungtsiang.top

[S25] C：内存拷贝
来源：http://psg.feifeiyinyue.top

memcpy(dst, src, n);
来源：http://wqz.zycfv.cn

[S26] C：内存清零
来源：http://cdd.sxryk.cn

memset(a, 0, sizeof a);
来源：http://ulx.havefunace.top

[S27] C：定义常量
来源：http://svr.hnqzz.top

const double PI = 3.14159;
来源：http://llm.meibo888.top

[S28] C：静态变量
来源：http://mxp.nanxuanxn.top

static int counter = 0;
来源：http://fei.sxryk.cn

[S29] C：变参函数
来源：http://qod.zhongyouzk.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zde.kuanghao11.cn

[S30] C：头文件保护
来源：http://lde.daxiang520.top

#ifndef X_H
来源：http://cck.316326.xyz

#define X_H
来源：http://drz.cheryme.top

#endif
来源：http://kei.cucudq.cn

[S31] C++：Hello World
来源：http://mqm.52xcode.cn

#include <iostream>
来源：http://ucc.zhongyouzk.top

int main() { std::cout << "Hello\n"; }
来源：http://zli.sxryk.cn

[S32] C++：字符串
来源：http://ykc.hnqzz.top

std::string s = "hi";  s += "!";
来源：http://yut.hcnkem.com

[S33] C++：vector 增删
来源：http://pxr.shzxlz.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tlt.52xcode.cn

[S34] C++：遍历 vector
来源：http://jlq.havefunace.top

for (auto &x : v) { std::cout << x; }
来源：http://bmr.ivvv.top

[S35] C++：map
来源：http://vkk.sufxvd.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ymi.sweek.top

[S36] C++：unordered_map
来源：http://mqs.guowangkeji.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://btw.zhiwuduotai.top

[S37] C++：set
来源：http://meu.zhongyouzk.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://way.dianchejie.cn

[S38] C++：排序
来源：http://msc.iojbl.cn

std::sort(v.begin(), v.end());
来源：http://nty.xuetiantiany.cn

[S39] C++：自定义比较器排序
来源：http://ngh.yuanzhike.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mhw.xuetiantiany.cn

[S40] C++：查找元素
来源：http://ekp.shanyushiyangkeji.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lni.hywenlv.cn

[S41] C++：类与构造函数
来源：http://xsn.zhiwuduotai.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hhx.gotoacloud.top

[S42] C++：继承与虚函数
来源：http://ckm.ehwqpu.com

class B : public Base { public: void f() override {} };
来源：http://wgx.yvedp.cn

[S43] C++：智能指针
来源：http://dxe.dianchejie.cn

auto p = std::make_unique<int>(5);
来源：http://jzl.fehbvm.com

[S44] C++：引用传参
来源：http://suw.vehdjk.com

void inc(int &x) { ++x; }
来源：http://obk.iojbl.cn

[S45] C++：lambda
来源：http://edq.jinghuilouyu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wfe.sysykeji.top

[S46] C++：函数模板
来源：http://jpy.jinyuanbaomall.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://onn.chenzaomai.com

[S47] C++：结构化绑定遍历
来源：http://inf.uphjek.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://src.9152youxi.cn

[S48] C++：逐行读文件
来源：http://qef.ybcxt.top

std::ifstream in("a.txt");  std::string line;
来源：http://ehn.nanxinkj.top

while (std::getline(in, line)) { }
来源：http://erq.jyoumei.cn

[S49] C++：写文件
来源：http://zur.cashguo.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://awy.hnqzz.top

[S50] C++：格式化数字
来源：http://jey.zdbjq.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://msi.svipenyu.cn

[S51] C++：显式类型转换
来源：http://fno.wangdashe.top

static_cast<double>(a) / b
来源：http://xid.yfazqb.com

[S52] C++：const 与 noexcept
来源：http://ifh.yj202588.top

int size() const noexcept { return n_; }
来源：http://hcv.vehdjk.com

[S53] C++：移动语义
来源：http://okc.zdbjq.cn

std::vector<int> w = std::move(v);
来源：http://nnm.vehdjk.com

[S54] C++：异常处理
来源：http://rqx.iojbl.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://eak.bjfxy.top

[S55] C++：结构化绑定
来源：http://fat.cheryme.top

auto [a, b] = std::make_pair(1, 2);
来源：http://obw.jyoumei.cn

[S56] C++：optional
来源：http://fhj.cashguo.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zwj.yj202588.top

[S57] C++：编译期常量
来源：http://iqa.cdnleiting.top

constexpr int N = 10;
来源：http://hjm.zycfv.cn

[S58] C++：命名空间
来源：http://bgp.pycfn.com

namespace ns { int f() { return 1; } }
来源：http://hzw.ivvv.top

[S59] C++：静态断言
来源：http://xrs.bbcook.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ibv.pycfn.com

[S60] C++：遍历并删除元素
来源：http://awp.yj202588.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gen.jinqigufen.top

================================================================================
来源：http://ajq.yongpay.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ahp.hammf.cn

================================================================================
来源：http://ihn.redwolf501.top

[T01] Kotlin：Hello World
来源：http://fey.xingfuxueyuan.xyz

println("Hello")
来源：http://luc.zhoulong.xyz

[T02] Kotlin：变量
来源：http://ggx.fzhhl.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hkp.tanke756.top

[T03] Kotlin：字符串模板
来源：http://rwq.hnxiangtu.top

"值: $b"
来源：http://huz.cucudq.cn

[T04] Kotlin：空安全
来源：http://afy.daria6918.cn

val n: String? = null;  n?.length
来源：http://huz.chenzaomai.com

[T05] Kotlin：when 表达式
来源：http://bba.shanyushiyangtech.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gvz.ywan-chungtsiang.top

[T06] Kotlin：集合映射
来源：http://kvd.iojbl.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://png.yuxming.cn

[T07] Kotlin：集合过滤
来源：http://bqh.fktsv.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://kqs.yonumen.top

[T08] Kotlin：数据类
来源：http://spb.jlsjyb.cn

data class User(val name: String, val age: Int)
来源：http://kli.daxiang520.top

[T09] Kotlin：扩展函数
来源：http://fom.aibaodan.cn

fun String.exclaim() = this + "!"
来源：http://ret.xylfe.cn

[T10] Kotlin：默认参数
来源：http://qzp.cashguo.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ddt.yueranfly.top

[T11] Kotlin：协程
来源：http://nfq.daria6918.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://usq.xinyue.icu

[T12] Kotlin：解构声明
来源：http://twm.daria6918.cn

val (a, b) = Pair(1, 2)
来源：http://ieb.aizwys.cn

[T13] Kotlin：只读 Map
来源：http://hpu.yfazqb.com

val m = mapOf("a" to 1)
来源：http://eyp.birdmap.top

[T14] Kotlin：循环
来源：http://efn.daxiang520.top

for (i in 1..10) println(i)
来源：http://kgl.shanyushiyangtech.top

[T15] Kotlin：接口
来源：http://nkh.uphjek.com

interface Shape { fun area(): Double }
来源：http://vol.shanyushiyangtech.top

[T16] Swift：Hello World
来源：http://aqj.hnxiangtu.top

print("Hello")
来源：http://xue.ybcxt.top

[T17] Swift：变量与常量
来源：http://kce.zdbjq.cn

var a = 1;  let b = 2
来源：http://rph.aizwys.cn

[T18] Swift：字符串插值
来源：http://uzp.jinghuilouyu.cn

"值: \(b)"
来源：http://qsl.zdbjq.cn

[T19] Swift：可选绑定
来源：http://fwo.yfazqb.com

if let n = opt { print(n) }
来源：http://vsr.hammf.cn

[T20] Swift：数组操作
来源：http://ztj.daxiang520.top

var a = [1, 2, 3];  a.append(4)
来源：http://mvo.cheryme.top

[T21] Swift：遍历
来源：http://iqx.tanke756.top

for x in a { print(x) }
来源：http://dud.tian-w.cn

[T22] Swift：字典
来源：http://nfz.zhongyouzk.top

var d = ["a": 1];  d["b"] = 2
来源：http://eyx.cucudq.cn

[T23] Swift：函数
来源：http://jlh.zhiwuduotai.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jar.xinyue.icu

[T24] Swift：闭包
来源：http://tep.meibo888.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://cxg.ydzc1.top

[T25] Swift：结构体
来源：http://cby.jinghuilouyu.cn

struct P { var x: Int }
来源：http://rio.redwolf501.top

[T26] Swift：类与重写
来源：http://svw.jinqigfzy.top

class A: Base { override func f() {} }
来源：http://trg.wangdashe.top

[T27] Swift：错误处理
来源：http://iny.fzhhl.top

do { try f() } catch { print(error) }
来源：http://kgx.hywenlv.cn

[T28] Swift：枚举
来源：http://nss.vqdsnc.cn

enum Color { case red, green }
来源：http://bdy.gotoacloud.top

[T29] Swift：guard 提前返回
来源：http://asz.birdmap.top

guard let x = opt else { return }
来源：http://cdg.snrcjt.cn

[T30] Swift：协议
来源：http://kip.yanxiufei.cn

protocol Shape { func area() -> Double }
来源：http://vxj.yj20258888.top

[T31] Lua：Hello World
来源：http://syc.guowangkeji.top

print("Hello")
来源：http://nrl.hongshengwenyu.top

[T32] Lua：局部变量
来源：http://kcc.snrcjt.cn

local a = 1
来源：http://lgi.yj202588.top

[T33] Lua：表（数组）
来源：http://bzu.hongshengwenyu.top

local t = {1, 2, 3};  t[4] = 4
来源：http://vhq.vqdsnc.cn

[T34] Lua：遍历表
来源：http://jpp.hnxiangtu.top

for i, v in ipairs(t) do print(i, v) end
来源：http://ugq.xuetiantiany.cn


<!-- 参考信息 -->