代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://whr.quarkkingdee.top

[R34] 退出时清理
来源：http://ami.zhengqikj.top

trap 'rm -f "$tmp"' EXIT
来源：http://woi.chenjidiqi.icu

[R35] 后台执行并等待
来源：http://taq.chenlongwang.top

sleep 5 & pid=$!; wait "$pid"
来源：http://cds.hcnkem.com

[R36] 并发执行多个任务
来源：http://qma.cucudq.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ccd.feifeiyinyue.top

[R37] 把输出赋给变量
来源：http://qqq.sjlbkw.cn

files=$(ls -1)
来源：http://kxn.shanyushiyangtech.top

[R38] 管道串联
来源：http://hqq.yongpay.top

cat a.txt | grep -i error | wc -l
来源：http://svr.haohaochexian.top

[R39] 重定向标准输出与错误
来源：http://cvl.zhoulong.xyz

cmd > out.log 2>&1
来源：http://gol.sxryk.cn

[R40] 追加写日志
来源：http://ruc.bjfxy.top

echo "log" >> out.log
来源：http://djf.xuetiantiany.cn

[R41] 丢弃输出
来源：http://aju.daria6918.cn

cmd >/dev/null 2>&1
来源：http://rkc.jqgfzy.top

[R42] 输入重定向
来源：http://eel.sysykeji.top

wc -l < a.txt
来源：http://hcf.andypj.xyz

[R43] 按名字查找文件
来源：http://jcb.shanyushiyangtech.top

find . -name "*.log" -type f
来源：http://anm.shanyushiyangkeji.top

[R44] 按修改时间查找
来源：http://ttl.vehdjk.com

find . -mtime -7 -type f
来源：http://kwz.zhongyouzk.top

[R45] 批量删除
来源：http://dne.jinghuilouyu.cn

find . -name "*.tmp" -delete
来源：http://rwb.birdmap.top

[R46] 递归替换文件内容
来源：http://axe.sxryk.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nfx.yangfankeji.com

[R47] sed 单行替换
来源：http://kqp.andypj.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://syw.zhoulong.xyz

[R48] awk 取指定列
来源：http://uqc.ctjpmb.com

awk '{print $1, $3}' a.txt
来源：http://fjp.gaohongyu789.top

[R49] awk 带条件
来源：http://ogz.cqqwz.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kev.vehdjk.com

[R50] awk 求和
来源：http://zlq.sufxvd.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ddr.iojbl.cn

[R51] 排序去重取前几
来源：http://bnk.gaohongyu789.top

sort a.txt | uniq -c | sort -rn | head
来源：http://dkz.yonumen.top

[R52] 统计行数
来源：http://eiz.vehdjk.com

wc -l a.txt
来源：http://tkm.pycfn.com

[R53] 查看文件头与实时尾
来源：http://bwv.guannengcc.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uve.ybcxt.top

[R54] 比较两个文件
来源：http://wen.hnqzz.top

diff a.txt b.txt
来源：http://hzx.fktsv.cn

[R55] 压缩与解压
来源：http://plg.zhoulong.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wzj.zdbjq.cn

[R56] 远程拷贝
来源：http://tvt.nanxinkj.top

scp file user@host:/path/
来源：http://ovm.zhengqikj.top

[R57] 远程执行命令
来源：http://zxk.smart0.xyz

ssh user@host 'uptime'
来源：http://gjl.xylfe.cn

[R58] 下载文件
来源：http://ytt.xylfe.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mrd.aizwys.cn

[R59] 发 POST JSON
来源：http://rec.epnwcf.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ecx.dashuyun.cn

[R60] 只看 HTTP 状态码
来源：http://ayf.jianghu66.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ixy.sufxvd.cn

[R61] 磁盘占用
来源：http://olr.jqgufenzy.top

df -h;  du -sh *
来源：http://efe.sjlbkw.cn

[R62] 找最占空间的文件
来源：http://nas.fengsongda.top

du -ah . | sort -rh | head -10
来源：http://dod.gaohongyu789.top

[R63] 内存与进程
来源：http://jez.zhoulong.xyz

free -h;  ps aux | grep nginx
来源：http://arr.hesvh.cn

[R64] 结束进程
来源：http://jbo.gzhubu.top

kill -9 $(pgrep -f app.py)
来源：http://xcq.yongpay.top

[R65] 查看端口占用
来源：http://lyi.9152youxi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ujn.hnxiangtu.top

[R66] 定时任务
来源：http://bhs.ydzc1.top

crontab -e;  crontab -l
来源：http://qwh.wangdashe.top

[R67] 生成随机十六进制串
来源：http://wsv.zhongyouzk.top

openssl rand -hex 16
来源：http://jcj.yanxiufei.cn

[R68] 计算文件校验值
来源：http://dfp.9152youxi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://kzo.yongpay.top

[R69] 生成随机密码
来源：http://lsj.ywan-chungtsiang.top

head -c 16 /dev/urandom | base64
来源：http://gaf.yvedp.cn

[R70] 时间戳与互转
来源：http://yao.xuanzx.com

date +%s;  date -d @1700000000
来源：http://ugx.cashguo.top

[R71] 日期格式化
来源：http://nne.wangdashe.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ffp.cheryme.top

[R72] 等待端口就绪
来源：http://jkv.hammf.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://npm.nanxuanxn.top

[R73] 分割大日志
来源：http://cis.gogol.net.cn

split -l 1000 big.log part_
来源：http://egj.hysaishi.cn

[R74] 批量重命名
来源：http://qrb.yongpay.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cof.zhaomingkeji.xyz

[R75] 导出环境变量
来源：http://qhl.jyoumei.cn

export PATH="$HOME/bin:$PATH"
来源：http://rwc.tian-w.cn

[R76] 使用临时文件
来源：http://uks.ywan-chungtsiang.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://stz.zhoulong.xyz

[R77] 读取用户输入
来源：http://szi.hysaishi.cn

read -rp "请输入: " ans
来源：http://lhg.zhixingplan.top

[R78] 交互式菜单
来源：http://tag.yongpay.top

select opt in a b c; do echo "$opt"; break; done
来源：http://aia.shanyushiyangtech.top

[R79] 解析命令行选项
来源：http://klf.zycfv.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nfu.wangdashe.top

[R80] 查看脚本执行耗时
来源：http://tme.andypj.xyz

time ./run.sh
来源：http://pja.jqgfzy.top

================================================================================
来源：http://ooa.iojbl.cn

S. C / C++ 专题
来源：http://bba.tianlin.xyz

================================================================================
来源：http://mzh.zhongyouzk.top

[S01] C：Hello World
来源：http://luf.zycfv.cn

#include <stdio.h>
来源：http://ffd.jinghuilouyu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://tya.hnxiangtu.top

[S02] C：变量与格式化输出
来源：http://zle.yueranfly.top

int a = 10; printf("%d\n", a);
来源：http://mrp.haohaochexian.top

[S03] C：读入整数
来源：http://lmh.haohaochexian.top

int x; scanf("%d", &x);
来源：http://jsn.snrcjt.cn

[S04] C：字符串复制
来源：http://dsh.ydjk.org.cn

char dst[32]; strcpy(dst, "hi");
来源：http://kwq.yj202588.top

[S05] C：字符串长度
来源：http://zxf.zhiwuduotai.top

strlen(s)
来源：http://dtl.dashuyun.cn

[S06] C：字符串比较
来源：http://sjp.cucudq.cn

strcmp(a, b) == 0
来源：http://rgl.ybcxt.top

[S07] C：数组遍历求和
来源：http://esg.gogol.net.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uyg.bjfxy.top

[S08] C：动态内存分配与释放
来源：http://zor.havefunace.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wbp.vqdsnc.cn

[S09] C：结构体定义与初始化
来源：http://wkm.zhengqikj.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dqa.xziqi.cn

[S10] C：指针与解引用
来源：http://dnr.ivvv.top

int *p = &a;  *p = 5;
来源：http://xvs.cqqwz.cn

[S11] C：逐行读文件
来源：http://urm.dashuyun.cn

FILE *f = fopen("a.txt", "r");
来源：http://nok.jinyuanbaomall.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://yqz.cqqwz.cn

fclose(f);
来源：http://vxc.zhixingplan.top

[S12] C：写文件
来源：http://upa.jinqigufen.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://edz.yfazqb.com

[S13] C：宏定义
来源：http://tvf.jyoumei.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jvh.wangshuangyany.cn

[S14] C：枚举
来源：http://xmq.bjfxy.top

enum Color { RED, GREEN, BLUE };
来源：http://ids.shzxlz.cn

[S15] C：类型转换
来源：http://htf.xylfe.cn

(double) a / b
来源：http://tjq.52xcode.cn

[S16] C：位操作置位
来源：http://fdp.ehwqpu.com

x |= (1 << 3);
来源：http://ovh.chenzaomai.com

[S17] C：安全拼接字符串
来源：http://itt.ydzc1.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://oup.cucudq.cn

[S18] C：命令行参数
来源：http://nfb.xinyue.icu

int main(int argc, char **argv)
来源：http://fpb.havefunace.top

[S19] C：快速排序
来源：http://jsg.snrcjt.cn

qsort(a, n, sizeof(int), cmp);
来源：http://yjl.wangshuangyany.cn

[S20] C：二分查找
来源：http://vqe.zhixingplan.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zkm.wangshuangyany.cn

[S21] C：字符类别判断
来源：http://kip.quarkkingdee.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cww.yj20258888.top

[S22] C：字符串转数字
来源：http://jze.dashuyun.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ers.jinqigufen.top

[S23] C：随机数
来源：http://rvp.xuanzx.com

srand(time(NULL));  int r = rand() % 100;
来源：http://ygb.xingfuxueyuan.xyz

[S24] C：获取本地时间
来源：http://ggl.gogol.net.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rta.xingfuxueyuan.xyz

[S25] C：内存拷贝
来源：http://jld.shangyingyoupin.top

memcpy(dst, src, n);
来源：http://qed.hesvh.cn

[S26] C：内存清零
来源：http://aad.ybcxt.top

memset(a, 0, sizeof a);
来源：http://ruu.nwbrower.top

[S27] C：定义常量
来源：http://dnp.fzhhl.top

const double PI = 3.14159;
来源：http://eve.jinqigufen.top

[S28] C：静态变量
来源：http://nbo.havefunace.top

static int counter = 0;
来源：http://fyb.daxiang520.top

[S29] C：变参函数
来源：http://qqw.yj20258.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://oah.52xcode.cn

[S30] C：头文件保护
来源：http://lvc.zhixingplan.top

#ifndef X_H
来源：http://atf.zycfv.cn

#define X_H
来源：http://gfz.hesvh.cn

#endif
来源：http://vrr.dianchejie.cn

[S31] C++：Hello World
来源：http://unw.feifeiyinyue.top

#include <iostream>
来源：http://otg.yvedp.cn

int main() { std::cout << "Hello\n"; }
来源：http://hbb.sufxvd.cn

[S32] C++：字符串
来源：http://sri.yj202588.top

std::string s = "hi";  s += "!";
来源：http://blk.gaohongyu789.top

[S33] C++：vector 增删
来源：http://vqt.shzxlz.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://trb.zhiwuduotai.top

[S34] C++：遍历 vector
来源：http://xtf.ppjwa.cn

for (auto &x : v) { std::cout << x; }
来源：http://wfp.sjlbkw.cn

[S35] C++：map
来源：http://phm.jinyuanbaomall.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jyt.0kj1m.cn

[S36] C++：unordered_map
来源：http://rig.yangfankeji.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kdw.aibaodan.cn

[S37] C++：set
来源：http://epi.uphjek.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://uya.cheryme.top

[S38] C++：排序
来源：http://zla.0kj1m.cn

std::sort(v.begin(), v.end());
来源：http://bzi.hywenlv.cn

[S39] C++：自定义比较器排序
来源：http://pln.hnxiangtu.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://azx.yvedp.cn

[S40] C++：查找元素
来源：http://iap.fzhhl.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fne.fktsv.cn

[S41] C++：类与构造函数
来源：http://twu.yj202588.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qoc.kuanghao11.cn

[S42] C++：继承与虚函数
来源：http://awl.zdqjudy.top

class B : public Base { public: void f() override {} };
来源：http://zpc.jqgfzy.top

[S43] C++：智能指针
来源：http://kem.tianlin.xyz

auto p = std::make_unique<int>(5);
来源：http://wah.mhx1999.top

[S44] C++：引用传参
来源：http://lhf.jlsjyb.cn

void inc(int &x) { ++x; }
来源：http://lrn.sysykeji.top

[S45] C++：lambda
来源：http://elc.fktsv.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wtp.0kj1m.cn

[S46] C++：函数模板
来源：http://abt.hcnkem.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uhb.zdqjudy.top

[S47] C++：结构化绑定遍历
来源：http://zmy.ctjpmb.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://otk.wangshuangyany.cn

[S48] C++：逐行读文件
来源：http://fli.gzhubu.top

std::ifstream in("a.txt");  std::string line;
来源：http://ywa.xuetiantiany.cn

while (std::getline(in, line)) { }
来源：http://iqn.xuanzx.com

[S49] C++：写文件
来源：http://ved.cdnleiting.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gqc.ehwqpu.com

[S50] C++：格式化数字
来源：http://rqw.zhijiandao.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lfp.hnqzz.top

[S51] C++：显式类型转换
来源：http://mwk.zhongyouzk.top

static_cast<double>(a) / b
来源：http://tof.cdnleiting.top

[S52] C++：const 与 noexcept
来源：http://rls.redwolf501.top

int size() const noexcept { return n_; }
来源：http://ngn.chenlongwang.top

[S53] C++：移动语义
来源：http://bzv.ehwqpu.com

std::vector<int> w = std::move(v);
来源：http://dqu.yanxiufei.cn

[S54] C++：异常处理
来源：http://cea.tarul.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ohe.hongshengwenyu.top

[S55] C++：结构化绑定
来源：http://pcz.shangyingyoupin.top

auto [a, b] = std::make_pair(1, 2);
来源：http://hrq.xinyue.icu

[S56] C++：optional
来源：http://zzk.zycfv.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xfn.xingfuxueyuan.xyz

[S57] C++：编译期常量
来源：http://vht.zdqjudy.top

constexpr int N = 10;
来源：http://hcy.aizwys.cn

[S58] C++：命名空间
来源：http://thk.yonumen.top

namespace ns { int f() { return 1; } }
来源：http://wgk.yj20258.top

[S59] C++：静态断言
来源：http://wft.jqgufenzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vno.andypj.xyz

[S60] C++：遍历并删除元素
来源：http://kae.vehdjk.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fea.316326.xyz

================================================================================
来源：http://inf.yvedp.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jal.zhiwuduotai.top

================================================================================
来源：http://pij.iojbl.cn

[T01] Kotlin：Hello World
来源：http://igx.yangfankeji.com

println("Hello")
来源：http://eyr.bjfxy.top

[T02] Kotlin：变量
来源：http://umw.52xcode.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ozm.316326.xyz

[T03] Kotlin：字符串模板
来源：http://nzs.redwolf501.top

"值: $b"
来源：http://nhh.cqqwz.cn

[T04] Kotlin：空安全
来源：http://ivt.hnxiangtu.top

val n: String? = null;  n?.length
来源：http://nlj.jyoumei.cn

[T05] Kotlin：when 表达式
来源：http://dnh.jyoumei.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://smb.vqdsnc.cn

[T06] Kotlin：集合映射
来源：http://ien.epnwcf.com

listOf(1, 2, 3).map { it * 2 }
来源：http://lrj.svipenyu.cn

[T07] Kotlin：集合过滤
来源：http://sri.fzhhl.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ndj.cheryme.top

[T08] Kotlin：数据类
来源：http://bzv.nanxuanxn.top

data class User(val name: String, val age: Int)
来源：http://qqs.zdbjq.cn

[T09] Kotlin：扩展函数
来源：http://xae.xinyue.icu

fun String.exclaim() = this + "!"
来源：http://lsv.ivvv.top

[T10] Kotlin：默认参数
来源：http://uif.yj20258888.top

fun greet(name: String = "World") = "Hi $name"
来源：http://ojf.shanyushiyangkeji.top

[T11] Kotlin：协程
来源：http://hcf.chenjidiqi.icu

GlobalScope.launch { delay(1000); println("done") }
来源：http://utg.bbcook.cn

[T12] Kotlin：解构声明
来源：http://gpg.iojbl.cn

val (a, b) = Pair(1, 2)
来源：http://yot.hongshengwenyu.top

[T13] Kotlin：只读 Map
来源：http://gjk.vehdjk.com

val m = mapOf("a" to 1)
来源：http://orf.fehbvm.com

[T14] Kotlin：循环
来源：http://frw.guannengcc.top

for (i in 1..10) println(i)
来源：http://srr.fanxiaobao.xyz

[T15] Kotlin：接口
来源：http://oqm.aizwys.cn

interface Shape { fun area(): Double }
来源：http://xls.dianchejie.cn

[T16] Swift：Hello World
来源：http://raa.c1oappe.top

print("Hello")
来源：http://uqf.havefunace.top

[T17] Swift：变量与常量
来源：http://awc.nanxuanxn.top

var a = 1;  let b = 2
来源：http://ruf.gaohongyu789.top

[T18] Swift：字符串插值
来源：http://kfq.yonumen.top

"值: \(b)"
来源：http://klv.birdmap.top

[T19] Swift：可选绑定
来源：http://van.fktsv.cn

if let n = opt { print(n) }
来源：http://wlb.ivvv.top

[T20] Swift：数组操作
来源：http://vnr.guowangkeji.top

var a = [1, 2, 3];  a.append(4)
来源：http://xyx.sysykeji.top

[T21] Swift：遍历
来源：http://zgv.tianlin.xyz

for x in a { print(x) }
来源：http://hhp.birdmap.top

[T22] Swift：字典
来源：http://avh.fengsongda.top

var d = ["a": 1];  d["b"] = 2
来源：http://vgk.meibo888.top

[T23] Swift：函数
来源：http://jax.yj20258.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qab.uphjek.com

[T24] Swift：闭包
来源：http://oou.zdbjq.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://mip.jiagoushi.top

[T25] Swift：结构体
来源：http://jrr.gaohongyu789.top

struct P { var x: Int }
来源：http://vjm.ehwqpu.com

[T26] Swift：类与重写
来源：http://gbg.xinyue.icu

class A: Base { override func f() {} }
来源：http://vzv.yfazqb.com

[T27] Swift：错误处理
来源：http://uww.redwolf501.top

do { try f() } catch { print(error) }
来源：http://aik.mhx1999.top

[T28] Swift：枚举
来源：http://kfe.xylfe.cn

enum Color { case red, green }
来源：http://xrf.nwbrower.top

[T29] Swift：guard 提前返回
来源：http://haw.tianlin.xyz

guard let x = opt else { return }
来源：http://txs.xylfe.cn

[T30] Swift：协议
来源：http://cse.316326.xyz

protocol Shape { func area() -> Double }
来源：http://vdc.jlsjyb.cn

[T31] Lua：Hello World
来源：http://bos.daria6918.cn

print("Hello")
来源：http://fks.fzhhl.top

[T32] Lua：局部变量
来源：http://bcd.hywenlv.cn

local a = 1
来源：http://tuy.tarul.cn

[T33] Lua：表（数组）
来源：http://gfu.vehdjk.com

local t = {1, 2, 3};  t[4] = 4
来源：http://cjt.andypj.xyz

[T34] Lua：遍历表
来源：http://raf.hammf.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://eyv.ivvv.top

[T35] Lua：字典表
来源：http://tva.jlsjyb.cn

local d = { a = 1 };  d.b = 2
来源：http://qkg.hfpthk.cn

[T36] Lua：函数
来源：http://xsw.hnxiangtu.top

function add(a, b) return a + b end
来源：http://roz.cheryme.top


<!-- 参考信息 -->