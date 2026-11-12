代发 wailian999

find . -name "*.log" -type f
来源：http://gus.feifeiyinyue.top

[R44] 按修改时间查找
来源：http://qaj.ivvv.top

find . -mtime -7 -type f
来源：http://wbs.xinyue.icu

[R45] 批量删除
来源：http://wdi.yfazqb.com

find . -name "*.tmp" -delete
来源：http://mrg.guowangkeji.top

[R46] 递归替换文件内容
来源：http://lmk.nanxinkj.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hip.chenlongwang.top

[R47] sed 单行替换
来源：http://qek.zycfv.cn

sed -i 's/foo/bar/g' a.txt
来源：http://alu.ywan-chungtsiang.top

[R48] awk 取指定列
来源：http://qkp.jyoumei.cn

awk '{print $1, $3}' a.txt
来源：http://gam.bbcook.cn

[R49] awk 带条件
来源：http://asg.pengpengdd.cyou

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ssu.yuxming.cn

[R50] awk 求和
来源：http://mes.iojbl.cn

awk '{s += $2} END {print s}' a.txt
来源：http://udx.cucudq.cn

[R51] 排序去重取前几
来源：http://uma.c1oappe.top

sort a.txt | uniq -c | sort -rn | head
来源：http://yfb.haohaochexian.top

[R52] 统计行数
来源：http://imn.vqdsnc.cn

wc -l a.txt
来源：http://zyp.gzhubu.top

[R53] 查看文件头与实时尾
来源：http://znz.yvedp.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sza.bjfxy.top

[R54] 比较两个文件
来源：http://wmt.0kj1m.cn

diff a.txt b.txt
来源：http://dff.ybcxt.top

[R55] 压缩与解压
来源：http://vfb.zhongyouzk.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ggd.jqgufenzy.top

[R56] 远程拷贝
来源：http://mse.havefunace.top

scp file user@host:/path/
来源：http://jna.yfazqb.com

[R57] 远程执行命令
来源：http://dvu.fktsv.cn

ssh user@host 'uptime'
来源：http://wfv.iojbl.cn

[R58] 下载文件
来源：http://pnm.zhongyouzk.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://paw.bbcook.cn

[R59] 发 POST JSON
来源：http://ith.gogol.net.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cbv.quarkkingdee.top

[R60] 只看 HTTP 状态码
来源：http://vpf.birdmap.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://brg.tarul.cn

[R61] 磁盘占用
来源：http://isg.hywenlv.cn

df -h;  du -sh *
来源：http://nwq.epnwcf.com

[R62] 找最占空间的文件
来源：http://vut.zhongyouzk.top

du -ah . | sort -rh | head -10
来源：http://pyi.yuanzhike.top

[R63] 内存与进程
来源：http://hog.chenzaomai.com

free -h;  ps aux | grep nginx
来源：http://uow.shanyushiyangkeji.top

[R64] 结束进程
来源：http://tmc.yangfankeji.com

kill -9 $(pgrep -f app.py)
来源：http://pjp.jiagoushi.top

[R65] 查看端口占用
来源：http://rcx.yj20258.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://crd.yj202588.top

[R66] 定时任务
来源：http://jjb.vqdsnc.cn

crontab -e;  crontab -l
来源：http://xyb.zhongyouzk.top

[R67] 生成随机十六进制串
来源：http://gva.tianlin.xyz

openssl rand -hex 16
来源：http://giw.sxryk.cn

[R68] 计算文件校验值
来源：http://qbc.jinqigfzy.top

sha256sum a.txt;  md5sum a.txt
来源：http://wfu.zhaomingkeji.xyz

[R69] 生成随机密码
来源：http://mhf.uphjek.com

head -c 16 /dev/urandom | base64
来源：http://ual.zhengqikj.top

[R70] 时间戳与互转
来源：http://wus.shangyingyoupin.top

date +%s;  date -d @1700000000
来源：http://cdo.xylfe.cn

[R71] 日期格式化
来源：http://dao.chenlongwang.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://xkh.sysykeji.top

[R72] 等待端口就绪
来源：http://ecd.dianchejie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cjh.jinghuilouyu.cn

[R73] 分割大日志
来源：http://sjf.xylfe.cn

split -l 1000 big.log part_
来源：http://pwv.yvedp.cn

[R74] 批量重命名
来源：http://imv.mhx1999.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://eyk.yuxming.cn

[R75] 导出环境变量
来源：http://vsr.birdmap.top

export PATH="$HOME/bin:$PATH"
来源：http://ypd.daxiang520.top

[R76] 使用临时文件
来源：http://rer.jinyuanbaomall.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kzf.nanxuanxn.top

[R77] 读取用户输入
来源：http://rnt.gogol.net.cn

read -rp "请输入: " ans
来源：http://zqf.jinyuanbaomall.cn

[R78] 交互式菜单
来源：http://qcw.iojbl.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://uzr.jinghuilouyu.cn

[R79] 解析命令行选项
来源：http://zpd.aizwys.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wou.zdqjudy.top

[R80] 查看脚本执行耗时
来源：http://czi.xuetiantiany.cn

time ./run.sh
来源：http://ngk.ehwqpu.com

================================================================================
来源：http://plz.dashuyun.cn

S. C / C++ 专题
来源：http://ufw.gotoacloud.top

================================================================================
来源：http://geg.redwolf501.top

[S01] C：Hello World
来源：http://zlu.jianghu66.top

#include <stdio.h>
来源：http://len.zhijiandao.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://egn.sxryk.cn

[S02] C：变量与格式化输出
来源：http://tvf.kuanghao11.cn

int a = 10; printf("%d\n", a);
来源：http://acp.fehbvm.com

[S03] C：读入整数
来源：http://uoe.hesvh.cn

int x; scanf("%d", &x);
来源：http://bzj.ppjwa.cn

[S04] C：字符串复制
来源：http://xtx.zhaomingkeji.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://nck.zdqjudy.top

[S05] C：字符串长度
来源：http://hqy.jinyuanbaomall.cn

strlen(s)
来源：http://bfn.iojbl.cn

[S06] C：字符串比较
来源：http://nsh.zhixingplan.top

strcmp(a, b) == 0
来源：http://jlt.wangshuangyany.cn

[S07] C：数组遍历求和
来源：http://osx.iojbl.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vts.nanxinkj.top

[S08] C：动态内存分配与释放
来源：http://pcn.shanyushiyangtech.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uzp.jiagoushi.top

[S09] C：结构体定义与初始化
来源：http://gnh.c1oappe.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cis.sufxvd.cn

[S10] C：指针与解引用
来源：http://uwl.sysykeji.top

int *p = &a;  *p = 5;
来源：http://krq.cqqwz.cn

[S11] C：逐行读文件
来源：http://nij.sjlbkw.cn

FILE *f = fopen("a.txt", "r");
来源：http://loi.yueranfly.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ggt.jqgfzy.top

fclose(f);
来源：http://npo.xuetiantiany.cn

[S12] C：写文件
来源：http://fgz.guowangkeji.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wqm.fanxiaobao.xyz

[S13] C：宏定义
来源：http://bxe.jqgfzy.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://nof.jlsjyb.cn

[S14] C：枚举
来源：http://syp.sweek.top

enum Color { RED, GREEN, BLUE };
来源：http://jwx.jqgfzy.top

[S15] C：类型转换
来源：http://pid.ydzc1.top

(double) a / b
来源：http://yzt.gotoacloud.top

[S16] C：位操作置位
来源：http://sqt.jqgufenzy.top

x |= (1 << 3);
来源：http://gzs.gotoacloud.top

[S17] C：安全拼接字符串
来源：http://vjb.pycfn.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cer.shuidangran.top

[S18] C：命令行参数
来源：http://ilr.ehwqpu.com

int main(int argc, char **argv)
来源：http://fgb.chenjidiqi.icu

[S19] C：快速排序
来源：http://ilo.xinyue.icu

qsort(a, n, sizeof(int), cmp);
来源：http://xra.gotoacloud.top

[S20] C：二分查找
来源：http://ejw.sxryk.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bka.aibaodan.cn

[S21] C：字符类别判断
来源：http://bfl.yuxming.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://eou.jinqigufen.top

[S22] C：字符串转数字
来源：http://fgd.guannengcc.top

atoi("42");  strtod("3.14", NULL);
来源：http://vbx.smart0.xyz

[S23] C：随机数
来源：http://gow.iojbl.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://gzj.jianghu66.top

[S24] C：获取本地时间
来源：http://lid.cdnleiting.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wpx.aibaodan.cn

[S25] C：内存拷贝
来源：http://ccj.jianghu66.top

memcpy(dst, src, n);
来源：http://lqt.iojbl.cn

[S26] C：内存清零
来源：http://rpj.yangfankeji.com

memset(a, 0, sizeof a);
来源：http://scy.bbcook.cn

[S27] C：定义常量
来源：http://iez.hywenlv.cn

const double PI = 3.14159;
来源：http://msx.316326.xyz

[S28] C：静态变量
来源：http://kzj.yuxming.cn

static int counter = 0;
来源：http://qiv.zdqjudy.top

[S29] C：变参函数
来源：http://naj.yuanzhike.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sht.cheryme.top

[S30] C：头文件保护
来源：http://nca.yj20258.top

#ifndef X_H
来源：http://wtj.uphjek.com

#define X_H
来源：http://emg.nanxuanxn.top

#endif
来源：http://avn.yj20258.top

[S31] C++：Hello World
来源：http://ork.hcnkem.com

#include <iostream>
来源：http://tro.hysaishi.cn

int main() { std::cout << "Hello\n"; }
来源：http://cdd.xylfe.cn

[S32] C++：字符串
来源：http://koc.iojbl.cn

std::string s = "hi";  s += "!";
来源：http://jza.gotoacloud.top

[S33] C++：vector 增删
来源：http://ubo.daxiang520.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bsf.zhixingplan.top

[S34] C++：遍历 vector
来源：http://dns.zhoulong.xyz

for (auto &x : v) { std::cout << x; }
来源：http://dpb.pycfn.com

[S35] C++：map
来源：http://adq.yuxming.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://uaf.zdbjq.cn

[S36] C++：unordered_map
来源：http://zbo.jianghu66.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vtz.mhx1999.top

[S37] C++：set
来源：http://gzf.hnxiangtu.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ooq.zhixingplan.top

[S38] C++：排序
来源：http://nop.zhiwuduotai.top

std::sort(v.begin(), v.end());
来源：http://izv.yj202588.top

[S39] C++：自定义比较器排序
来源：http://ixj.nwbrower.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hom.cashguo.top

[S40] C++：查找元素
来源：http://shy.zhaomingkeji.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kkl.jinqigfzy.top

[S41] C++：类与构造函数
来源：http://zqo.tian-w.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://uri.yangfankeji.com

[S42] C++：继承与虚函数
来源：http://azd.yj20258.top

class B : public Base { public: void f() override {} };
来源：http://iiv.yangfankeji.com

[S43] C++：智能指针
来源：http://yrt.zhiwuduotai.top

auto p = std::make_unique<int>(5);
来源：http://ybs.chenzaomai.com

[S44] C++：引用传参
来源：http://czo.daxiang520.top

void inc(int &x) { ++x; }
来源：http://aiq.hfpthk.cn

[S45] C++：lambda
来源：http://cui.ehwqpu.com

auto add = [](int a, int b) { return a + b; };
来源：http://jaj.epnwcf.com

[S46] C++：函数模板
来源：http://ohv.yvedp.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xro.zhiwuduotai.top

[S47] C++：结构化绑定遍历
来源：http://ssp.iojbl.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hym.fktsv.cn

[S48] C++：逐行读文件
来源：http://nne.316326.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://coj.birdmap.top

while (std::getline(in, line)) { }
来源：http://bfb.gaohongyu789.top

[S49] C++：写文件
来源：http://dfs.zhixingplan.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wnd.sweek.top

[S50] C++：格式化数字
来源：http://flb.bbcook.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cvt.feifeiyinyue.top

[S51] C++：显式类型转换
来源：http://zsx.daria6918.cn

static_cast<double>(a) / b
来源：http://agv.dianchejie.cn

[S52] C++：const 与 noexcept
来源：http://qts.tianlin.xyz

int size() const noexcept { return n_; }
来源：http://llx.zhaomingkeji.xyz

[S53] C++：移动语义
来源：http://ulp.jiagoushi.top

std::vector<int> w = std::move(v);
来源：http://cvw.cheryme.top

[S54] C++：异常处理
来源：http://kvm.fengsongda.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://scu.yangfankeji.com

[S55] C++：结构化绑定
来源：http://cla.ctjpmb.com

auto [a, b] = std::make_pair(1, 2);
来源：http://gmc.snrcjt.cn

[S56] C++：optional
来源：http://nsx.vehdjk.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hob.andypj.xyz

[S57] C++：编译期常量
来源：http://qkc.ehwqpu.com

constexpr int N = 10;
来源：http://etj.ppjwa.cn

[S58] C++：命名空间
来源：http://mcu.vqdsnc.cn

namespace ns { int f() { return 1; } }
来源：http://oqd.chenlongwang.top

[S59] C++：静态断言
来源：http://srz.birdmap.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vgz.jinqigfzy.top

[S60] C++：遍历并删除元素
来源：http://hur.chenjidiqi.icu

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://uen.ywan-chungtsiang.top

================================================================================
来源：http://mcp.tian-w.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qih.jiagoushi.top

================================================================================
来源：http://shc.shanyushiyangkeji.top

[T01] Kotlin：Hello World
来源：http://dzm.cheryme.top

println("Hello")
来源：http://buu.bbcook.cn

[T02] Kotlin：变量
来源：http://qcu.gotoacloud.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ykc.gaohongyu789.top

[T03] Kotlin：字符串模板
来源：http://alr.yfazqb.com

"值: $b"
来源：http://bxg.jqgufenzy.top

[T04] Kotlin：空安全
来源：http://qbb.zhixingplan.top

val n: String? = null;  n?.length
来源：http://uet.hnxiangtu.top

[T05] Kotlin：when 表达式
来源：http://hpb.ywan-chungtsiang.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fni.cucudq.cn

[T06] Kotlin：集合映射
来源：http://qju.yonumen.top

listOf(1, 2, 3).map { it * 2 }
来源：http://qsw.zdqjudy.top

[T07] Kotlin：集合过滤
来源：http://jqk.gogol.net.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://nws.ppjwa.cn

[T08] Kotlin：数据类
来源：http://sbf.yfazqb.com

data class User(val name: String, val age: Int)
来源：http://pny.daxiang520.top

[T09] Kotlin：扩展函数
来源：http://lzt.daxiang520.top

fun String.exclaim() = this + "!"
来源：http://fkk.gogol.net.cn

[T10] Kotlin：默认参数
来源：http://cuc.0kj1m.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://hiw.ybcxt.top

[T11] Kotlin：协程
来源：http://rcc.jyoumei.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ptv.sufxvd.cn

[T12] Kotlin：解构声明
来源：http://zuo.xinyue.icu

val (a, b) = Pair(1, 2)
来源：http://wph.gaohongyu789.top

[T13] Kotlin：只读 Map
来源：http://njz.yj20258.top

val m = mapOf("a" to 1)
来源：http://ibf.gotoacloud.top

[T14] Kotlin：循环
来源：http://cdi.guowangkeji.top

for (i in 1..10) println(i)
来源：http://csp.vehdjk.com

[T15] Kotlin：接口
来源：http://wtu.yanxiufei.cn

interface Shape { fun area(): Double }
来源：http://dns.quarkkingdee.top

[T16] Swift：Hello World
来源：http://dqk.yanxiufei.cn

print("Hello")
来源：http://tqs.xuetiantiany.cn

[T17] Swift：变量与常量
来源：http://nyb.chenjidiqi.icu

var a = 1;  let b = 2
来源：http://btd.nwbrower.top

[T18] Swift：字符串插值
来源：http://fdu.yangfankeji.com

"值: \(b)"
来源：http://vkb.cdnleiting.top

[T19] Swift：可选绑定
来源：http://ivq.nanxuanxn.top

if let n = opt { print(n) }
来源：http://hvt.vqdsnc.cn

[T20] Swift：数组操作
来源：http://rzp.cashguo.top

var a = [1, 2, 3];  a.append(4)
来源：http://igb.tarul.cn

[T21] Swift：遍历
来源：http://moc.bbcook.cn

for x in a { print(x) }
来源：http://nlk.yj202588.top

[T22] Swift：字典
来源：http://qdr.xingfuxueyuan.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://awp.svipenyu.cn

[T23] Swift：函数
来源：http://zwh.gogol.net.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fyv.hcnkem.com

[T24] Swift：闭包
来源：http://ino.guowangkeji.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://ijd.jianghu66.top

[T25] Swift：结构体
来源：http://jdy.zhijiandao.cn

struct P { var x: Int }
来源：http://yym.smart0.xyz

[T26] Swift：类与重写
来源：http://jie.svipenyu.cn

class A: Base { override func f() {} }
来源：http://kte.guannengcc.top

[T27] Swift：错误处理
来源：http://ers.shanyushiyangkeji.top

do { try f() } catch { print(error) }
来源：http://cun.jyoumei.cn

[T28] Swift：枚举
来源：http://iyv.hesvh.cn

enum Color { case red, green }
来源：http://rzq.jinqigfzy.top

[T29] Swift：guard 提前返回
来源：http://ntv.vehdjk.com

guard let x = opt else { return }
来源：http://wbb.ydzc1.top

[T30] Swift：协议
来源：http://tcv.vqdsnc.cn

protocol Shape { func area() -> Double }
来源：http://pan.daria6918.cn

[T31] Lua：Hello World
来源：http://abc.shangyingyoupin.top

print("Hello")
来源：http://tyv.ppjwa.cn

[T32] Lua：局部变量
来源：http://bap.316326.xyz

local a = 1
来源：http://jsv.0kj1m.cn

[T33] Lua：表（数组）
来源：http://crt.jyoumei.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://aho.jianghu66.top

[T34] Lua：遍历表
来源：http://dtw.tianlin.xyz

for i, v in ipairs(t) do print(i, v) end
来源：http://rrh.vqdsnc.cn

[T35] Lua：字典表
来源：http://lev.hnqzz.top

local d = { a = 1 };  d.b = 2
来源：http://vgl.yanxiufei.cn

[T36] Lua：函数
来源：http://hwp.aibaodan.cn

function add(a, b) return a + b end
来源：http://zlw.ppjwa.cn

[T37] Lua：字符串拼接
来源：http://hba.pycfn.com

"a" .. "b"
来源：http://tws.smart0.xyz

[T38] Lua：条件
来源：http://vor.zdbjq.cn

if x > 0 then print("正") end
来源：http://yqz.dianchejie.cn

[T39] Lua：模式匹配
来源：http://fnr.zdbjq.cn

string.find(s, "%d+")
来源：http://rqc.ydzc1.top

[T40] Lua：元表
来源：http://ydq.hfpthk.cn

setmetatable({}, { __index = base })
来源：http://qpk.xylfe.cn

[T41] Perl：Hello World
来源：http://tmg.pycfn.com

print "Hello\n";
来源：http://tcd.hnqzz.top

[T42] Perl：变量类型
来源：http://udf.sxryk.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gha.epnwcf.com

[T43] Perl：字符串插值
来源：http://phv.jinyuanbaomall.cn

"值: $a"
来源：http://tza.cheryme.top

[T44] Perl：条件
来源：http://xdx.cashguo.top

if ($a > 0) { print "正"; }
来源：http://yqa.kuanghao11.cn

[T45] Perl：数组遍历
来源：http://gpj.yanxiufei.cn

for my $x (@arr) { print $x; }
来源：http://hwe.zhaomingkeji.xyz

[T46] Perl：哈希操作
来源：http://wfk.yuxming.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://yse.sweek.top


<!-- 参考信息 -->