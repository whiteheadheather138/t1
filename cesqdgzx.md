代发 wailian999

cmd > out.log 2>&1
来源：http://jhy.haohaochexian.top

[R40] 追加写日志
来源：http://ffx.yfazqb.com

echo "log" >> out.log
来源：http://arx.yfazqb.com

[R41] 丢弃输出
来源：http://nrn.kuanghao11.cn

cmd >/dev/null 2>&1
来源：http://dxf.sweek.top

[R42] 输入重定向
来源：http://umn.shangyingyoupin.top

wc -l < a.txt
来源：http://pat.daria6918.cn

[R43] 按名字查找文件
来源：http://kpy.mhx1999.top

find . -name "*.log" -type f
来源：http://hpz.tanke756.top

[R44] 按修改时间查找
来源：http://nnp.hysaishi.cn

find . -mtime -7 -type f
来源：http://foa.aibaodan.cn

[R45] 批量删除
来源：http://pew.vqdsnc.cn

find . -name "*.tmp" -delete
来源：http://rte.hnqzz.top

[R46] 递归替换文件内容
来源：http://pqp.feifeiyinyue.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xkr.daxiang520.top

[R47] sed 单行替换
来源：http://idp.mhx1999.top

sed -i 's/foo/bar/g' a.txt
来源：http://jjr.ywan-chungtsiang.top

[R48] awk 取指定列
来源：http://xog.vqdsnc.cn

awk '{print $1, $3}' a.txt
来源：http://opu.fehbvm.com

[R49] awk 带条件
来源：http://ioz.snrcjt.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sjq.yfazqb.com

[R50] awk 求和
来源：http://lpu.snrcjt.cn

awk '{s += $2} END {print s}' a.txt
来源：http://swb.nanxuanxn.top

[R51] 排序去重取前几
来源：http://ptt.jqgufenzy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://fzc.ehwqpu.com

[R52] 统计行数
来源：http://xka.feifeiyinyue.top

wc -l a.txt
来源：http://xdc.zhengqikj.top

[R53] 查看文件头与实时尾
来源：http://yny.zhengqikj.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hxj.pycfn.com

[R54] 比较两个文件
来源：http://zwk.yvedp.cn

diff a.txt b.txt
来源：http://opk.ywan-chungtsiang.top

[R55] 压缩与解压
来源：http://ekn.wangdashe.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ppq.hfpthk.cn

[R56] 远程拷贝
来源：http://qdk.zhaomingkeji.xyz

scp file user@host:/path/
来源：http://pqm.hfpthk.cn

[R57] 远程执行命令
来源：http://hhn.jinqigfzy.top

ssh user@host 'uptime'
来源：http://ztg.gzhubu.top

[R58] 下载文件
来源：http://zji.gaohongyu789.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fkn.jqgfzy.top

[R59] 发 POST JSON
来源：http://vpz.cqqwz.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fjh.ydzc1.top

[R60] 只看 HTTP 状态码
来源：http://dhq.cucudq.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ipc.pycfn.com

[R61] 磁盘占用
来源：http://cek.snrcjt.cn

df -h;  du -sh *
来源：http://evu.kuanghao11.cn

[R62] 找最占空间的文件
来源：http://hwo.chenlongwang.top

du -ah . | sort -rh | head -10
来源：http://qaf.cqqwz.cn

[R63] 内存与进程
来源：http://wqf.jianghu66.top

free -h;  ps aux | grep nginx
来源：http://ggh.jiagoushi.top

[R64] 结束进程
来源：http://mjn.yfazqb.com

kill -9 $(pgrep -f app.py)
来源：http://get.aibaodan.cn

[R65] 查看端口占用
来源：http://kpw.hcnkem.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vyc.xziqi.cn

[R66] 定时任务
来源：http://aac.xuanzx.com

crontab -e;  crontab -l
来源：http://ejy.gzhubu.top

[R67] 生成随机十六进制串
来源：http://fte.c1oappe.top

openssl rand -hex 16
来源：http://rpm.kuanghao11.cn

[R68] 计算文件校验值
来源：http://zsb.birdmap.top

sha256sum a.txt;  md5sum a.txt
来源：http://jjg.pycfn.com

[R69] 生成随机密码
来源：http://nvm.xuanzx.com

head -c 16 /dev/urandom | base64
来源：http://ixn.wangdashe.top

[R70] 时间戳与互转
来源：http://nyz.wangdashe.top

date +%s;  date -d @1700000000
来源：http://pmx.jinyuanbaomall.cn

[R71] 日期格式化
来源：http://qoj.shzxlz.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zuk.daria6918.cn

[R72] 等待端口就绪
来源：http://kir.zdbjq.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hvz.epnwcf.com

[R73] 分割大日志
来源：http://uwd.nanxuanxn.top

split -l 1000 big.log part_
来源：http://rjx.tanke756.top

[R74] 批量重命名
来源：http://bbm.zhiwuduotai.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kdj.tianlin.xyz

[R75] 导出环境变量
来源：http://bad.nanxuanxn.top

export PATH="$HOME/bin:$PATH"
来源：http://ddl.jianghu66.top

[R76] 使用临时文件
来源：http://rrv.mhx1999.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ppu.sxryk.cn

[R77] 读取用户输入
来源：http://oea.fanxiaobao.xyz

read -rp "请输入: " ans
来源：http://xad.xylfe.cn

[R78] 交互式菜单
来源：http://twk.zdqjudy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://jqi.jinqigfzy.top

[R79] 解析命令行选项
来源：http://utg.shanyushiyangkeji.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://avm.aizwys.cn

[R80] 查看脚本执行耗时
来源：http://knu.mhx1999.top

time ./run.sh
来源：http://brs.nwbrower.top

================================================================================
来源：http://kiu.xziqi.cn

S. C / C++ 专题
来源：http://dzg.jyoumei.cn

================================================================================
来源：http://vzl.sweek.top

[S01] C：Hello World
来源：http://cyt.gzhubu.top

#include <stdio.h>
来源：http://gnw.ctjpmb.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://lsb.vehdjk.com

[S02] C：变量与格式化输出
来源：http://kdq.iojbl.cn

int a = 10; printf("%d\n", a);
来源：http://ter.hfpthk.cn

[S03] C：读入整数
来源：http://fiu.hnqzz.top

int x; scanf("%d", &x);
来源：http://kza.cucudq.cn

[S04] C：字符串复制
来源：http://unz.zhengqikj.top

char dst[32]; strcpy(dst, "hi");
来源：http://git.nanxuanxn.top

[S05] C：字符串长度
来源：http://etq.c1oappe.top

strlen(s)
来源：http://uvk.cqqwz.cn

[S06] C：字符串比较
来源：http://jzf.hfpthk.cn

strcmp(a, b) == 0
来源：http://mup.bbcook.cn

[S07] C：数组遍历求和
来源：http://dyq.nanxuanxn.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ehu.yj20258888.top

[S08] C：动态内存分配与释放
来源：http://drr.jlsjyb.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zcv.pengpengdd.cyou

[S09] C：结构体定义与初始化
来源：http://ezk.zhengqikj.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dcc.guowangkeji.top

[S10] C：指针与解引用
来源：http://kon.dashuyun.cn

int *p = &a;  *p = 5;
来源：http://uqy.wangshuangyany.cn

[S11] C：逐行读文件
来源：http://yrv.jinqigufen.top

FILE *f = fopen("a.txt", "r");
来源：http://ril.yj20258888.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://jmm.gaohongyu789.top

fclose(f);
来源：http://mku.birdmap.top

[S12] C：写文件
来源：http://axf.yuxming.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rem.jinghuilouyu.cn

[S13] C：宏定义
来源：http://wdo.jqgufenzy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ael.fehbvm.com

[S14] C：枚举
来源：http://dxk.tarul.cn

enum Color { RED, GREEN, BLUE };
来源：http://gzb.yj20258888.top

[S15] C：类型转换
来源：http://nhl.chenjidiqi.icu

(double) a / b
来源：http://ihb.bbcook.cn

[S16] C：位操作置位
来源：http://qfl.yuanzhike.top

x |= (1 << 3);
来源：http://lvl.hammf.cn

[S17] C：安全拼接字符串
来源：http://ujj.0kj1m.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qrt.fengsongda.top

[S18] C：命令行参数
来源：http://aaw.haohaochexian.top

int main(int argc, char **argv)
来源：http://fsv.guannengcc.top

[S19] C：快速排序
来源：http://igb.zhiwuduotai.top

qsort(a, n, sizeof(int), cmp);
来源：http://wwv.quarkkingdee.top

[S20] C：二分查找
来源：http://pow.hywenlv.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zmv.guannengcc.top

[S21] C：字符类别判断
来源：http://lpv.bbcook.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kzk.andypj.xyz

[S22] C：字符串转数字
来源：http://mzj.hysaishi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://gzu.zhixingplan.top

[S23] C：随机数
来源：http://iqc.fanxiaobao.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://jyq.yj202588.top

[S24] C：获取本地时间
来源：http://pwy.cucudq.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://prn.hcnkem.com

[S25] C：内存拷贝
来源：http://fsz.bjfxy.top

memcpy(dst, src, n);
来源：http://bzi.tarul.cn

[S26] C：内存清零
来源：http://pae.aizwys.cn

memset(a, 0, sizeof a);
来源：http://odk.smart0.xyz

[S27] C：定义常量
来源：http://ffj.jqgufenzy.top

const double PI = 3.14159;
来源：http://any.hfpthk.cn

[S28] C：静态变量
来源：http://zkx.epnwcf.com

static int counter = 0;
来源：http://vsc.nanxinkj.top

[S29] C：变参函数
来源：http://cny.xziqi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jvo.xuetiantiany.cn

[S30] C：头文件保护
来源：http://zca.tianlin.xyz

#ifndef X_H
来源：http://grj.yongpay.top

#define X_H
来源：http://ywq.xuanzx.com

#endif
来源：http://gyn.ybcxt.top

[S31] C++：Hello World
来源：http://tht.cashguo.top

#include <iostream>
来源：http://zyn.nanxuanxn.top

int main() { std::cout << "Hello\n"; }
来源：http://sxc.zhoulong.xyz

[S32] C++：字符串
来源：http://vlx.ctjpmb.com

std::string s = "hi";  s += "!";
来源：http://tbw.feifeiyinyue.top

[S33] C++：vector 增删
来源：http://imo.meibo888.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://acu.xuetiantiany.cn

[S34] C++：遍历 vector
来源：http://cgm.xuetiantiany.cn

for (auto &x : v) { std::cout << x; }
来源：http://wpl.hammf.cn

[S35] C++：map
来源：http://fbd.fzhhl.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dgy.jiagoushi.top

[S36] C++：unordered_map
来源：http://ahj.sweek.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zab.xuetiantiany.cn

[S37] C++：set
来源：http://nln.gzhubu.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ukr.cqqwz.cn

[S38] C++：排序
来源：http://fte.yanxiufei.cn

std::sort(v.begin(), v.end());
来源：http://dxn.gaohongyu789.top

[S39] C++：自定义比较器排序
来源：http://kfa.jqgufenzy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vom.yueranfly.top

[S40] C++：查找元素
来源：http://pzk.redwolf501.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zcd.fehbvm.com

[S41] C++：类与构造函数
来源：http://elh.c1oappe.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://thn.316326.xyz

[S42] C++：继承与虚函数
来源：http://sdq.chenzaomai.com

class B : public Base { public: void f() override {} };
来源：http://dlk.sufxvd.cn

[S43] C++：智能指针
来源：http://zyy.sweek.top

auto p = std::make_unique<int>(5);
来源：http://bjf.gotoacloud.top

[S44] C++：引用传参
来源：http://pms.zhongyouzk.top

void inc(int &x) { ++x; }
来源：http://trk.redwolf501.top

[S45] C++：lambda
来源：http://egy.shangyingyoupin.top

auto add = [](int a, int b) { return a + b; };
来源：http://aoy.jqgufenzy.top

[S46] C++：函数模板
来源：http://nhr.hywenlv.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yvc.yueranfly.top

[S47] C++：结构化绑定遍历
来源：http://rry.tianlin.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vdi.ivvv.top

[S48] C++：逐行读文件
来源：http://ycb.birdmap.top

std::ifstream in("a.txt");  std::string line;
来源：http://jwy.wangshuangyany.cn

while (std::getline(in, line)) { }
来源：http://nbe.shanyushiyangtech.top

[S49] C++：写文件
来源：http://zwt.ybcxt.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bjn.yuanzhike.top

[S50] C++：格式化数字
来源：http://mea.aizwys.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ugl.iojbl.cn

[S51] C++：显式类型转换
来源：http://vmm.ydzc1.top

static_cast<double>(a) / b
来源：http://xkn.xylfe.cn

[S52] C++：const 与 noexcept
来源：http://mos.meibo888.top

int size() const noexcept { return n_; }
来源：http://gfe.havefunace.top

[S53] C++：移动语义
来源：http://gto.xingfuxueyuan.xyz

std::vector<int> w = std::move(v);
来源：http://wem.nwbrower.top

[S54] C++：异常处理
来源：http://zev.jianghu66.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://max.xylfe.cn

[S55] C++：结构化绑定
来源：http://lvl.zhixingplan.top

auto [a, b] = std::make_pair(1, 2);
来源：http://lhr.bbcook.cn

[S56] C++：optional
来源：http://fmp.hywenlv.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zqp.tian-w.cn

[S57] C++：编译期常量
来源：http://wcq.jinghuilouyu.cn

constexpr int N = 10;
来源：http://zfx.fzhhl.top

[S58] C++：命名空间
来源：http://prp.hnxiangtu.top

namespace ns { int f() { return 1; } }
来源：http://pzi.hnqzz.top

[S59] C++：静态断言
来源：http://lsf.sufxvd.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xne.bjfxy.top

[S60] C++：遍历并删除元素
来源：http://nky.jyoumei.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mxv.jyoumei.cn

================================================================================
来源：http://wxb.zdqjudy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ufe.vehdjk.com

================================================================================
来源：http://ygv.ehwqpu.com

[T01] Kotlin：Hello World
来源：http://gtv.ivvv.top

println("Hello")
来源：http://qas.nanxuanxn.top

[T02] Kotlin：变量
来源：http://mwp.jlsjyb.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zvn.haohaochexian.top

[T03] Kotlin：字符串模板
来源：http://ptu.zhiwuduotai.top

"值: $b"
来源：http://cld.yj202588.top

[T04] Kotlin：空安全
来源：http://rno.fzhhl.top

val n: String? = null;  n?.length
来源：http://yhn.jiagoushi.top

[T05] Kotlin：when 表达式
来源：http://lhe.yvedp.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gno.ybcxt.top

[T06] Kotlin：集合映射
来源：http://rau.0kj1m.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://bgh.yj202588.top

[T07] Kotlin：集合过滤
来源：http://bwg.hammf.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ark.fengsongda.top

[T08] Kotlin：数据类
来源：http://ytr.yj20258.top

data class User(val name: String, val age: Int)
来源：http://kcq.ivvv.top

[T09] Kotlin：扩展函数
来源：http://wue.jinqigfzy.top

fun String.exclaim() = this + "!"
来源：http://fgc.pengpengdd.cyou

[T10] Kotlin：默认参数
来源：http://eeq.nwbrower.top

fun greet(name: String = "World") = "Hi $name"
来源：http://nlr.hammf.cn

[T11] Kotlin：协程
来源：http://vcg.sxryk.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://rdb.hongshengwenyu.top

[T12] Kotlin：解构声明
来源：http://sqk.haohaochexian.top

val (a, b) = Pair(1, 2)
来源：http://byn.gaohongyu789.top

[T13] Kotlin：只读 Map
来源：http://gbw.tian-w.cn

val m = mapOf("a" to 1)
来源：http://zlp.jyoumei.cn

[T14] Kotlin：循环
来源：http://mdm.jiagoushi.top

for (i in 1..10) println(i)
来源：http://wig.vehdjk.com

[T15] Kotlin：接口
来源：http://oga.jinqigufen.top

interface Shape { fun area(): Double }
来源：http://nxm.svipenyu.cn

[T16] Swift：Hello World
来源：http://wrz.yanxiufei.cn

print("Hello")
来源：http://ase.pengpengdd.cyou

[T17] Swift：变量与常量
来源：http://yxk.hongshengwenyu.top

var a = 1;  let b = 2
来源：http://bvw.bjfxy.top

[T18] Swift：字符串插值
来源：http://rqg.gotoacloud.top

"值: \(b)"
来源：http://ouv.sufxvd.cn

[T19] Swift：可选绑定
来源：http://nlu.fzhhl.top

if let n = opt { print(n) }
来源：http://qzp.meibo888.top

[T20] Swift：数组操作
来源：http://qoq.guowangkeji.top

var a = [1, 2, 3];  a.append(4)
来源：http://ati.jianghu66.top

[T21] Swift：遍历
来源：http://vvz.snrcjt.cn

for x in a { print(x) }
来源：http://ikt.yonumen.top

[T22] Swift：字典
来源：http://mci.quarkkingdee.top

var d = ["a": 1];  d["b"] = 2
来源：http://qep.zhengqikj.top

[T23] Swift：函数
来源：http://pwa.yonumen.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://uho.yj20258.top

[T24] Swift：闭包
来源：http://cyu.dianchejie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://jmw.bbcook.cn

[T25] Swift：结构体
来源：http://xwq.yj20258888.top

struct P { var x: Int }
来源：http://nit.ywan-chungtsiang.top

[T26] Swift：类与重写
来源：http://mkc.zycfv.cn

class A: Base { override func f() {} }
来源：http://nuo.hywenlv.cn

[T27] Swift：错误处理
来源：http://sko.andypj.xyz

do { try f() } catch { print(error) }
来源：http://phd.tanke756.top

[T28] Swift：枚举
来源：http://gwe.andypj.xyz

enum Color { case red, green }
来源：http://xut.fengsongda.top

[T29] Swift：guard 提前返回
来源：http://qea.jianghu66.top

guard let x = opt else { return }
来源：http://qpt.sxryk.cn

[T30] Swift：协议
来源：http://kpm.gotoacloud.top

protocol Shape { func area() -> Double }
来源：http://bhn.sweek.top

[T31] Lua：Hello World
来源：http://knf.fanxiaobao.xyz

print("Hello")
来源：http://hvz.cheryme.top

[T32] Lua：局部变量
来源：http://gqr.zycfv.cn

local a = 1
来源：http://chf.wangdashe.top

[T33] Lua：表（数组）
来源：http://nmf.vqdsnc.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://jbk.cqqwz.cn

[T34] Lua：遍历表
来源：http://qms.cucudq.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ehp.aizwys.cn

[T35] Lua：字典表
来源：http://fvp.zycfv.cn

local d = { a = 1 };  d.b = 2
来源：http://wtk.chenjidiqi.icu

[T36] Lua：函数
来源：http://pst.fanxiaobao.xyz

function add(a, b) return a + b end
来源：http://jyf.hysaishi.cn

[T37] Lua：字符串拼接
来源：http://jgt.zhaomingkeji.xyz

"a" .. "b"
来源：http://ayt.ydjk.org.cn

[T38] Lua：条件
来源：http://kgq.bbcook.cn

if x > 0 then print("正") end
来源：http://geq.cdnleiting.top

[T39] Lua：模式匹配
来源：http://bzu.shanyushiyangtech.top

string.find(s, "%d+")
来源：http://ple.yj20258888.top

[T40] Lua：元表
来源：http://dqa.aizwys.cn

setmetatable({}, { __index = base })
来源：http://obt.jinghuilouyu.cn

[T41] Perl：Hello World
来源：http://trb.daxiang520.top

print "Hello\n";
来源：http://hva.meibo888.top

[T42] Perl：变量类型
来源：http://dii.yuxming.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bbl.yanxiufei.cn


<!-- 参考信息 -->