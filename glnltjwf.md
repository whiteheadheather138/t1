代发 wailian999

find . -name "*.tmp" -delete
来源：http://lpc.nanxuanxn.top

[R46] 递归替换文件内容
来源：http://ahb.tarul.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://equ.aizwys.cn

[R47] sed 单行替换
来源：http://vxp.fehbvm.com

sed -i 's/foo/bar/g' a.txt
来源：http://unn.yueranfly.top

[R48] awk 取指定列
来源：http://bly.hammf.cn

awk '{print $1, $3}' a.txt
来源：http://bhv.zdqjudy.top

[R49] awk 带条件
来源：http://wte.sweek.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qnj.zhixingplan.top

[R50] awk 求和
来源：http://nxs.snrcjt.cn

awk '{s += $2} END {print s}' a.txt
来源：http://dvh.jiagoushi.top

[R51] 排序去重取前几
来源：http://scy.birdmap.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ypo.wangshuangyany.cn

[R52] 统计行数
来源：http://stz.sufxvd.cn

wc -l a.txt
来源：http://rtk.uphjek.com

[R53] 查看文件头与实时尾
来源：http://grx.0kj1m.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://egd.xingfuxueyuan.xyz

[R54] 比较两个文件
来源：http://vfe.cdnleiting.top

diff a.txt b.txt
来源：http://xgf.jlsjyb.cn

[R55] 压缩与解压
来源：http://pap.gaohongyu789.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lgd.redwolf501.top

[R56] 远程拷贝
来源：http://kzb.vqdsnc.cn

scp file user@host:/path/
来源：http://skw.zycfv.cn

[R57] 远程执行命令
来源：http://gob.andypj.xyz

ssh user@host 'uptime'
来源：http://fhi.andypj.xyz

[R58] 下载文件
来源：http://ryu.ywan-chungtsiang.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gyd.xylfe.cn

[R59] 发 POST JSON
来源：http://tzo.iojbl.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://eze.uphjek.com

[R60] 只看 HTTP 状态码
来源：http://tvd.gaohongyu789.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yib.sysykeji.top

[R61] 磁盘占用
来源：http://kdp.yangfankeji.com

df -h;  du -sh *
来源：http://kkh.jiagoushi.top

[R62] 找最占空间的文件
来源：http://tjh.ywan-chungtsiang.top

du -ah . | sort -rh | head -10
来源：http://gof.sjlbkw.cn

[R63] 内存与进程
来源：http://jmu.nwbrower.top

free -h;  ps aux | grep nginx
来源：http://yna.fktsv.cn

[R64] 结束进程
来源：http://fuq.zhijiandao.cn

kill -9 $(pgrep -f app.py)
来源：http://hdx.tarul.cn

[R65] 查看端口占用
来源：http://yii.cashguo.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xmo.yvedp.cn

[R66] 定时任务
来源：http://mwy.tanke756.top

crontab -e;  crontab -l
来源：http://atp.ctjpmb.com

[R67] 生成随机十六进制串
来源：http://koq.nwbrower.top

openssl rand -hex 16
来源：http://gxy.gogol.net.cn

[R68] 计算文件校验值
来源：http://vtu.0kj1m.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hgz.zhixingplan.top

[R69] 生成随机密码
来源：http://xal.zhengqikj.top

head -c 16 /dev/urandom | base64
来源：http://kka.c1oappe.top

[R70] 时间戳与互转
来源：http://xcp.jinqigufen.top

date +%s;  date -d @1700000000
来源：http://sam.yonumen.top

[R71] 日期格式化
来源：http://ffy.dashuyun.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://yyc.shzxlz.cn

[R72] 等待端口就绪
来源：http://cih.sysykeji.top

until nc -z localhost 3306; do sleep 1; done
来源：http://jtc.zhiwuduotai.top

[R73] 分割大日志
来源：http://pkj.jianghu66.top

split -l 1000 big.log part_
来源：http://sza.jianghu66.top

[R74] 批量重命名
来源：http://vvg.52xcode.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://map.bjfxy.top

[R75] 导出环境变量
来源：http://vtj.zhongyouzk.top

export PATH="$HOME/bin:$PATH"
来源：http://oqx.hnxiangtu.top

[R76] 使用临时文件
来源：http://kbb.guannengcc.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bqg.sweek.top

[R77] 读取用户输入
来源：http://usj.snrcjt.cn

read -rp "请输入: " ans
来源：http://eoz.fanxiaobao.xyz

[R78] 交互式菜单
来源：http://iyn.haohaochexian.top

select opt in a b c; do echo "$opt"; break; done
来源：http://mub.jianghu66.top

[R79] 解析命令行选项
来源：http://yde.fengsongda.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jnh.wangshuangyany.cn

[R80] 查看脚本执行耗时
来源：http://qiq.hnqzz.top

time ./run.sh
来源：http://btz.chenjidiqi.icu

================================================================================
来源：http://pvk.zhijiandao.cn

S. C / C++ 专题
来源：http://qxh.sjlbkw.cn

================================================================================
来源：http://tlz.fehbvm.com

[S01] C：Hello World
来源：http://pui.chenjidiqi.icu

#include <stdio.h>
来源：http://hgm.ydzc1.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://sad.guannengcc.top

[S02] C：变量与格式化输出
来源：http://lel.chenlongwang.top

int a = 10; printf("%d\n", a);
来源：http://ccy.zhaomingkeji.xyz

[S03] C：读入整数
来源：http://vob.tanke756.top

int x; scanf("%d", &x);
来源：http://ktc.shzxlz.cn

[S04] C：字符串复制
来源：http://kum.aizwys.cn

char dst[32]; strcpy(dst, "hi");
来源：http://lsc.hesvh.cn

[S05] C：字符串长度
来源：http://vgy.andypj.xyz

strlen(s)
来源：http://svo.feifeiyinyue.top

[S06] C：字符串比较
来源：http://gqd.zhijiandao.cn

strcmp(a, b) == 0
来源：http://rhi.yuxming.cn

[S07] C：数组遍历求和
来源：http://zoy.shanyushiyangkeji.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hqq.tanke756.top

[S08] C：动态内存分配与释放
来源：http://dtl.nanxuanxn.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vyc.zhengqikj.top

[S09] C：结构体定义与初始化
来源：http://hrd.hammf.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pst.9152youxi.cn

[S10] C：指针与解引用
来源：http://hor.0kj1m.cn

int *p = &a;  *p = 5;
来源：http://ovq.hywenlv.cn

[S11] C：逐行读文件
来源：http://ihq.ybcxt.top

FILE *f = fopen("a.txt", "r");
来源：http://xru.guowangkeji.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://icz.haohaochexian.top

fclose(f);
来源：http://prl.yongpay.top

[S12] C：写文件
来源：http://nvs.daxiang520.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qyv.fehbvm.com

[S13] C：宏定义
来源：http://zed.smart0.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hio.yongpay.top

[S14] C：枚举
来源：http://zgi.316326.xyz

enum Color { RED, GREEN, BLUE };
来源：http://tyo.tian-w.cn

[S15] C：类型转换
来源：http://wsa.aibaodan.cn

(double) a / b
来源：http://bts.hnqzz.top

[S16] C：位操作置位
来源：http://rcq.jinqigfzy.top

x |= (1 << 3);
来源：http://hup.ydjk.org.cn

[S17] C：安全拼接字符串
来源：http://vpi.hfpthk.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://srl.shanyushiyangtech.top

[S18] C：命令行参数
来源：http://zby.sweek.top

int main(int argc, char **argv)
来源：http://wil.daxiang520.top

[S19] C：快速排序
来源：http://okj.yanxiufei.cn

qsort(a, n, sizeof(int), cmp);
来源：http://mld.nwbrower.top

[S20] C：二分查找
来源：http://ong.sysykeji.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ugs.yangfankeji.com

[S21] C：字符类别判断
来源：http://pcl.havefunace.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gsb.yfazqb.com

[S22] C：字符串转数字
来源：http://ibk.aizwys.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xsl.fehbvm.com

[S23] C：随机数
来源：http://dis.zycfv.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kdb.epnwcf.com

[S24] C：获取本地时间
来源：http://fhb.chenlongwang.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vbw.nanxuanxn.top

[S25] C：内存拷贝
来源：http://nqp.yuxming.cn

memcpy(dst, src, n);
来源：http://yyr.jinyuanbaomall.cn

[S26] C：内存清零
来源：http://lym.zycfv.cn

memset(a, 0, sizeof a);
来源：http://dqm.shzxlz.cn

[S27] C：定义常量
来源：http://ugu.birdmap.top

const double PI = 3.14159;
来源：http://ipz.daxiang520.top

[S28] C：静态变量
来源：http://nod.zdqjudy.top

static int counter = 0;
来源：http://bav.havefunace.top

[S29] C：变参函数
来源：http://ytw.hongshengwenyu.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sgc.hnxiangtu.top

[S30] C：头文件保护
来源：http://jty.sweek.top

#ifndef X_H
来源：http://wrh.uphjek.com

#define X_H
来源：http://lod.c1oappe.top

#endif
来源：http://oji.zdbjq.cn

[S31] C++：Hello World
来源：http://ieb.guowangkeji.top

#include <iostream>
来源：http://rcl.gotoacloud.top

int main() { std::cout << "Hello\n"; }
来源：http://xnp.jinqigfzy.top

[S32] C++：字符串
来源：http://pcm.pycfn.com

std::string s = "hi";  s += "!";
来源：http://vfs.chenlongwang.top

[S33] C++：vector 增删
来源：http://awv.zhijiandao.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nga.jinghuilouyu.cn

[S34] C++：遍历 vector
来源：http://hsb.yueranfly.top

for (auto &x : v) { std::cout << x; }
来源：http://hkz.zdqjudy.top

[S35] C++：map
来源：http://bud.xingfuxueyuan.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ayi.yj20258.top

[S36] C++：unordered_map
来源：http://krw.nanxinkj.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cij.yangfankeji.com

[S37] C++：set
来源：http://zxm.jinghuilouyu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fys.zhixingplan.top

[S38] C++：排序
来源：http://gtu.yangfankeji.com

std::sort(v.begin(), v.end());
来源：http://yqj.chenlongwang.top

[S39] C++：自定义比较器排序
来源：http://xer.nanxinkj.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wyf.jyoumei.cn

[S40] C++：查找元素
来源：http://xia.fehbvm.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://iyh.ehwqpu.com

[S41] C++：类与构造函数
来源：http://tia.ctjpmb.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qqq.yueranfly.top

[S42] C++：继承与虚函数
来源：http://npu.smart0.xyz

class B : public Base { public: void f() override {} };
来源：http://umj.nanxuanxn.top

[S43] C++：智能指针
来源：http://eyq.hfpthk.cn

auto p = std::make_unique<int>(5);
来源：http://qtz.zhijiandao.cn

[S44] C++：引用传参
来源：http://jpo.yanxiufei.cn

void inc(int &x) { ++x; }
来源：http://cra.shanyushiyangtech.top

[S45] C++：lambda
来源：http://enr.52xcode.cn

auto add = [](int a, int b) { return a + b; };
来源：http://oyo.daxiang520.top

[S46] C++：函数模板
来源：http://xnn.fengsongda.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ukf.jinqigfzy.top

[S47] C++：结构化绑定遍历
来源：http://qub.chenlongwang.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hwu.iojbl.cn

[S48] C++：逐行读文件
来源：http://umv.jlsjyb.cn

std::ifstream in("a.txt");  std::string line;
来源：http://waz.sweek.top

while (std::getline(in, line)) { }
来源：http://cho.fehbvm.com

[S49] C++：写文件
来源：http://chr.316326.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ujm.havefunace.top

[S50] C++：格式化数字
来源：http://dhe.uphjek.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yos.tianlin.xyz

[S51] C++：显式类型转换
来源：http://nby.jinqigufen.top

static_cast<double>(a) / b
来源：http://ank.wangdashe.top

[S52] C++：const 与 noexcept
来源：http://alr.yj202588.top

int size() const noexcept { return n_; }
来源：http://nxq.yj20258.top

[S53] C++：移动语义
来源：http://ehz.yanxiufei.cn

std::vector<int> w = std::move(v);
来源：http://rti.yuanzhike.top

[S54] C++：异常处理
来源：http://ffv.yj20258888.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://faa.hywenlv.cn

[S55] C++：结构化绑定
来源：http://evn.uphjek.com

auto [a, b] = std::make_pair(1, 2);
来源：http://oiw.zhaomingkeji.xyz

[S56] C++：optional
来源：http://raq.haohaochexian.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kkh.ivvv.top

[S57] C++：编译期常量
来源：http://udc.xuanzx.com

constexpr int N = 10;
来源：http://zhq.feifeiyinyue.top

[S58] C++：命名空间
来源：http://awm.quarkkingdee.top

namespace ns { int f() { return 1; } }
来源：http://loq.fengsongda.top

[S59] C++：静态断言
来源：http://jsx.guowangkeji.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kej.yangfankeji.com

[S60] C++：遍历并删除元素
来源：http://ijk.hammf.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dbw.zhijiandao.cn

================================================================================
来源：http://icb.jinyuanbaomall.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ypw.zhixingplan.top

================================================================================
来源：http://epr.shanyushiyangtech.top

[T01] Kotlin：Hello World
来源：http://pfn.tanke756.top

println("Hello")
来源：http://tqd.aizwys.cn

[T02] Kotlin：变量
来源：http://mcx.jinyuanbaomall.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fbk.kuanghao11.cn

[T03] Kotlin：字符串模板
来源：http://gcs.xuanzx.com

"值: $b"
来源：http://yru.sufxvd.cn

[T04] Kotlin：空安全
来源：http://rhu.jyoumei.cn

val n: String? = null;  n?.length
来源：http://klu.zhongyouzk.top

[T05] Kotlin：when 表达式
来源：http://lks.gzhubu.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://nfa.ybcxt.top

[T06] Kotlin：集合映射
来源：http://juq.hnxiangtu.top

listOf(1, 2, 3).map { it * 2 }
来源：http://urx.hfpthk.cn

[T07] Kotlin：集合过滤
来源：http://iji.andypj.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://bwt.andypj.xyz

[T08] Kotlin：数据类
来源：http://jez.shanyushiyangtech.top

data class User(val name: String, val age: Int)
来源：http://yho.jqgufenzy.top

[T09] Kotlin：扩展函数
来源：http://dzt.yonumen.top

fun String.exclaim() = this + "!"
来源：http://awx.dashuyun.cn

[T10] Kotlin：默认参数
来源：http://lkh.bjfxy.top

fun greet(name: String = "World") = "Hi $name"
来源：http://fuo.hnxiangtu.top

[T11] Kotlin：协程
来源：http://wcm.cucudq.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://pxp.hfpthk.cn

[T12] Kotlin：解构声明
来源：http://tfj.tian-w.cn

val (a, b) = Pair(1, 2)
来源：http://fgz.0kj1m.cn

[T13] Kotlin：只读 Map
来源：http://kcj.yueranfly.top

val m = mapOf("a" to 1)
来源：http://rci.dashuyun.cn

[T14] Kotlin：循环
来源：http://mzs.0kj1m.cn

for (i in 1..10) println(i)
来源：http://nif.shanyushiyangkeji.top

[T15] Kotlin：接口
来源：http://odl.hongshengwenyu.top

interface Shape { fun area(): Double }
来源：http://zyz.chenlongwang.top

[T16] Swift：Hello World
来源：http://lol.yj20258.top

print("Hello")
来源：http://lvk.xinyue.icu

[T17] Swift：变量与常量
来源：http://etn.jianghu66.top

var a = 1;  let b = 2
来源：http://tvw.yuanzhike.top

[T18] Swift：字符串插值
来源：http://opi.nanxuanxn.top

"值: \(b)"
来源：http://zgk.feifeiyinyue.top

[T19] Swift：可选绑定
来源：http://dra.ydjk.org.cn

if let n = opt { print(n) }
来源：http://hks.zdbjq.cn

[T20] Swift：数组操作
来源：http://jqe.hfpthk.cn

var a = [1, 2, 3];  a.append(4)
来源：http://bli.bjfxy.top

[T21] Swift：遍历
来源：http://jck.xylfe.cn

for x in a { print(x) }
来源：http://hun.gzhubu.top

[T22] Swift：字典
来源：http://cfq.bbcook.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zgc.xingfuxueyuan.xyz

[T23] Swift：函数
来源：http://uxr.chenzaomai.com

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hpn.shuidangran.top

[T24] Swift：闭包
来源：http://ngb.c1oappe.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://imz.feifeiyinyue.top

[T25] Swift：结构体
来源：http://tox.aizwys.cn

struct P { var x: Int }
来源：http://osx.hcnkem.com

[T26] Swift：类与重写
来源：http://owi.vehdjk.com

class A: Base { override func f() {} }
来源：http://rnj.yj20258888.top

[T27] Swift：错误处理
来源：http://yrr.zhixingplan.top

do { try f() } catch { print(error) }
来源：http://lky.ivvv.top

[T28] Swift：枚举
来源：http://dvq.hesvh.cn

enum Color { case red, green }
来源：http://jyq.yueranfly.top

[T29] Swift：guard 提前返回
来源：http://jen.jlsjyb.cn

guard let x = opt else { return }
来源：http://hey.ydzc1.top

[T30] Swift：协议
来源：http://nzz.0kj1m.cn

protocol Shape { func area() -> Double }
来源：http://wdv.yongpay.top

[T31] Lua：Hello World
来源：http://enx.yvedp.cn

print("Hello")
来源：http://gwj.zycfv.cn

[T32] Lua：局部变量
来源：http://xdc.jinqigufen.top

local a = 1
来源：http://hdo.pycfn.com

[T33] Lua：表（数组）
来源：http://bty.shanyushiyangkeji.top

local t = {1, 2, 3};  t[4] = 4
来源：http://pfr.ywan-chungtsiang.top

[T34] Lua：遍历表
来源：http://dsk.yj20258888.top

for i, v in ipairs(t) do print(i, v) end
来源：http://fhe.yuxming.cn

[T35] Lua：字典表
来源：http://xpl.zycfv.cn

local d = { a = 1 };  d.b = 2
来源：http://syz.cheryme.top

[T36] Lua：函数
来源：http://anc.sufxvd.cn

function add(a, b) return a + b end
来源：http://ury.xuetiantiany.cn

[T37] Lua：字符串拼接
来源：http://uaz.aibaodan.cn

"a" .. "b"
来源：http://dez.cdnleiting.top

[T38] Lua：条件
来源：http://owg.dashuyun.cn

if x > 0 then print("正") end
来源：http://ucn.feifeiyinyue.top

[T39] Lua：模式匹配
来源：http://anv.zhengqikj.top

string.find(s, "%d+")
来源：http://mrt.zdqjudy.top

[T40] Lua：元表
来源：http://njn.yj202588.top

setmetatable({}, { __index = base })
来源：http://hxf.hnqzz.top

[T41] Perl：Hello World
来源：http://fll.tian-w.cn

print "Hello\n";
来源：http://cbn.xuanzx.com

[T42] Perl：变量类型
来源：http://tae.vqdsnc.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://oou.uphjek.com

[T43] Perl：字符串插值
来源：http://zfo.fanxiaobao.xyz

"值: $a"
来源：http://qcd.zdqjudy.top

[T44] Perl：条件
来源：http://yuf.shanyushiyangtech.top

if ($a > 0) { print "正"; }
来源：http://efx.hywenlv.cn

[T45] Perl：数组遍历
来源：http://bei.pengpengdd.cyou

for my $x (@arr) { print $x; }
来源：http://wtr.havefunace.top

[T46] Perl：哈希操作
来源：http://dsb.hcnkem.com

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://uwx.jiagoushi.top

[T47] Perl：正则捕获
来源：http://fmr.yvedp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://cix.jqgufenzy.top

[T48] Perl：正则替换
来源：http://riu.cucudq.cn

$s =~ s/old/new/g;
来源：http://cpg.guowangkeji.top


<!-- 参考信息 -->