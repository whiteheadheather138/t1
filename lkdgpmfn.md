代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://tho.yfazqb.com

[R26] 命令替换
来源：http://rmo.guowangkeji.top

now=$(date +%F); echo "$now"
来源：http://evk.sweek.top

[R27] 算术展开
来源：http://iqf.yongpay.top

echo $((1 + 2 * 3))
来源：http://nmh.fehbvm.com

[R28] 浮点运算
来源：http://sue.pengpengdd.cyou

echo "scale=2; 10/3" | bc
来源：http://zee.svipenyu.cn

[R29] 定义函数
来源：http://ibw.iojbl.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zhg.chenjidiqi.icu

[R30] 函数返回状态码
来源：http://ind.shanyushiyangtech.top

f() { return 0; }; f || echo "失败了"
来源：http://atr.hywenlv.cn

[R31] 局部变量
来源：http://ila.sysykeji.top

f() { local x=1; echo "$x"; }
来源：http://yfl.zdqjudy.top

[R32] 参数个数校验
来源：http://glo.cheryme.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://txr.tianlin.xyz

[R33] 捕获错误并提示行号
来源：http://pqm.vehdjk.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://avc.smart0.xyz

[R34] 退出时清理
来源：http://wzf.pengpengdd.cyou

trap 'rm -f "$tmp"' EXIT
来源：http://qef.bbcook.cn

[R35] 后台执行并等待
来源：http://wmq.nanxinkj.top

sleep 5 & pid=$!; wait "$pid"
来源：http://umz.iojbl.cn

[R36] 并发执行多个任务
来源：http://oyl.yueranfly.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xqs.dianchejie.cn

[R37] 把输出赋给变量
来源：http://kao.jqgfzy.top

files=$(ls -1)
来源：http://wwy.pycfn.com

[R38] 管道串联
来源：http://nup.xylfe.cn

cat a.txt | grep -i error | wc -l
来源：http://nyv.yuanzhike.top

[R39] 重定向标准输出与错误
来源：http://xyl.zhijiandao.cn

cmd > out.log 2>&1
来源：http://wrf.redwolf501.top

[R40] 追加写日志
来源：http://mwm.redwolf501.top

echo "log" >> out.log
来源：http://wmi.pengpengdd.cyou

[R41] 丢弃输出
来源：http://aky.yuxming.cn

cmd >/dev/null 2>&1
来源：http://vjh.fehbvm.com

[R42] 输入重定向
来源：http://omg.fzhhl.top

wc -l < a.txt
来源：http://wpl.xuanzx.com

[R43] 按名字查找文件
来源：http://iqp.shuidangran.top

find . -name "*.log" -type f
来源：http://zhk.sxryk.cn

[R44] 按修改时间查找
来源：http://ttb.yj20258.top

find . -mtime -7 -type f
来源：http://mxn.ivvv.top

[R45] 批量删除
来源：http://yfb.fanxiaobao.xyz

find . -name "*.tmp" -delete
来源：http://pmc.feifeiyinyue.top

[R46] 递归替换文件内容
来源：http://bls.wangshuangyany.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jpm.yj202588.top

[R47] sed 单行替换
来源：http://dcr.zycfv.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ifb.chenzaomai.com

[R48] awk 取指定列
来源：http://qre.ctjpmb.com

awk '{print $1, $3}' a.txt
来源：http://nfk.jiagoushi.top

[R49] awk 带条件
来源：http://oao.ywan-chungtsiang.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sos.hywenlv.cn

[R50] awk 求和
来源：http://vyz.fanxiaobao.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://yio.feifeiyinyue.top

[R51] 排序去重取前几
来源：http://snh.yangfankeji.com

sort a.txt | uniq -c | sort -rn | head
来源：http://loj.daria6918.cn

[R52] 统计行数
来源：http://mrp.tian-w.cn

wc -l a.txt
来源：http://wrn.chenjidiqi.icu

[R53] 查看文件头与实时尾
来源：http://gqd.daxiang520.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kjl.feifeiyinyue.top

[R54] 比较两个文件
来源：http://ynl.fehbvm.com

diff a.txt b.txt
来源：http://ghl.xylfe.cn

[R55] 压缩与解压
来源：http://nao.bjfxy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jdn.hammf.cn

[R56] 远程拷贝
来源：http://zcf.ppjwa.cn

scp file user@host:/path/
来源：http://jhe.cashguo.top

[R57] 远程执行命令
来源：http://oba.yuanzhike.top

ssh user@host 'uptime'
来源：http://zva.smart0.xyz

[R58] 下载文件
来源：http://fho.cucudq.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cfh.tian-w.cn

[R59] 发 POST JSON
来源：http://fqq.yonumen.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ehv.jinqigufen.top

[R60] 只看 HTTP 状态码
来源：http://mkr.gogol.net.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://msl.yonumen.top

[R61] 磁盘占用
来源：http://cha.gzhubu.top

df -h;  du -sh *
来源：http://lxy.vqdsnc.cn

[R62] 找最占空间的文件
来源：http://asg.wangshuangyany.cn

du -ah . | sort -rh | head -10
来源：http://doh.shzxlz.cn

[R63] 内存与进程
来源：http://krb.xuetiantiany.cn

free -h;  ps aux | grep nginx
来源：http://ftk.nwbrower.top

[R64] 结束进程
来源：http://ktz.snrcjt.cn

kill -9 $(pgrep -f app.py)
来源：http://qgs.gzhubu.top

[R65] 查看端口占用
来源：http://eks.xziqi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gev.dianchejie.cn

[R66] 定时任务
来源：http://jor.yanxiufei.cn

crontab -e;  crontab -l
来源：http://bop.jinyuanbaomall.cn

[R67] 生成随机十六进制串
来源：http://pmk.sjlbkw.cn

openssl rand -hex 16
来源：http://tas.snrcjt.cn

[R68] 计算文件校验值
来源：http://ume.jinghuilouyu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://idp.yj202588.top

[R69] 生成随机密码
来源：http://fxm.andypj.xyz

head -c 16 /dev/urandom | base64
来源：http://bss.hongshengwenyu.top

[R70] 时间戳与互转
来源：http://leq.shanyushiyangkeji.top

date +%s;  date -d @1700000000
来源：http://djp.xylfe.cn

[R71] 日期格式化
来源：http://jla.aibaodan.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://sej.yfazqb.com

[R72] 等待端口就绪
来源：http://mbo.gzhubu.top

until nc -z localhost 3306; do sleep 1; done
来源：http://dfs.snrcjt.cn

[R73] 分割大日志
来源：http://mfg.cdnleiting.top

split -l 1000 big.log part_
来源：http://byh.jyoumei.cn

[R74] 批量重命名
来源：http://hnq.chenlongwang.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ftg.cdnleiting.top

[R75] 导出环境变量
来源：http://jse.316326.xyz

export PATH="$HOME/bin:$PATH"
来源：http://krs.zhiwuduotai.top

[R76] 使用临时文件
来源：http://kvb.ctjpmb.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wdk.tanke756.top

[R77] 读取用户输入
来源：http://bku.fehbvm.com

read -rp "请输入: " ans
来源：http://mkz.fzhhl.top

[R78] 交互式菜单
来源：http://dbg.jinghuilouyu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://qnh.yonumen.top

[R79] 解析命令行选项
来源：http://bav.chenzaomai.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cvm.daxiang520.top

[R80] 查看脚本执行耗时
来源：http://tdl.0kj1m.cn

time ./run.sh
来源：http://irj.hnqzz.top

================================================================================
来源：http://rfa.fengsongda.top

S. C / C++ 专题
来源：http://deo.yanxiufei.cn

================================================================================
来源：http://aur.ywan-chungtsiang.top

[S01] C：Hello World
来源：http://skx.zdqjudy.top

#include <stdio.h>
来源：http://fjo.ehwqpu.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://pxf.jyoumei.cn

[S02] C：变量与格式化输出
来源：http://qgw.sysykeji.top

int a = 10; printf("%d\n", a);
来源：http://ime.zhoulong.xyz

[S03] C：读入整数
来源：http://aea.svipenyu.cn

int x; scanf("%d", &x);
来源：http://abe.zhixingplan.top

[S04] C：字符串复制
来源：http://cil.fzhhl.top

char dst[32]; strcpy(dst, "hi");
来源：http://zqk.zhiwuduotai.top

[S05] C：字符串长度
来源：http://uwc.hnxiangtu.top

strlen(s)
来源：http://efr.cqqwz.cn

[S06] C：字符串比较
来源：http://ldi.sysykeji.top

strcmp(a, b) == 0
来源：http://kmo.yj202588.top

[S07] C：数组遍历求和
来源：http://ptp.tianlin.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lja.mhx1999.top

[S08] C：动态内存分配与释放
来源：http://msr.zhoulong.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hon.fzhhl.top

[S09] C：结构体定义与初始化
来源：http://ctr.svipenyu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pan.tian-w.cn

[S10] C：指针与解引用
来源：http://jix.snrcjt.cn

int *p = &a;  *p = 5;
来源：http://hev.cqqwz.cn

[S11] C：逐行读文件
来源：http://rci.xingfuxueyuan.xyz

FILE *f = fopen("a.txt", "r");
来源：http://vck.pengpengdd.cyou

while (fgets(buf, sizeof buf, f)) { }
来源：http://wvv.zhoulong.xyz

fclose(f);
来源：http://dnw.sufxvd.cn

[S12] C：写文件
来源：http://lfl.aibaodan.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zji.fanxiaobao.xyz

[S13] C：宏定义
来源：http://roo.chenzaomai.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lwg.yj20258.top

[S14] C：枚举
来源：http://ltx.fanxiaobao.xyz

enum Color { RED, GREEN, BLUE };
来源：http://sph.uphjek.com

[S15] C：类型转换
来源：http://zeo.hysaishi.cn

(double) a / b
来源：http://yee.dianchejie.cn

[S16] C：位操作置位
来源：http://zki.0kj1m.cn

x |= (1 << 3);
来源：http://ktc.wangdashe.top

[S17] C：安全拼接字符串
来源：http://yiv.chenlongwang.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://avc.chenlongwang.top

[S18] C：命令行参数
来源：http://bbp.andypj.xyz

int main(int argc, char **argv)
来源：http://mfg.epnwcf.com

[S19] C：快速排序
来源：http://app.zhaomingkeji.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://ttc.sysykeji.top

[S20] C：二分查找
来源：http://uzz.xingfuxueyuan.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://aal.chenlongwang.top

[S21] C：字符类别判断
来源：http://gpe.hongshengwenyu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xic.chenzaomai.com

[S22] C：字符串转数字
来源：http://kkm.sxryk.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tcz.hongshengwenyu.top

[S23] C：随机数
来源：http://ilq.kuanghao11.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xcq.shzxlz.cn

[S24] C：获取本地时间
来源：http://ebf.xylfe.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://njh.ehwqpu.com

[S25] C：内存拷贝
来源：http://hxf.yongpay.top

memcpy(dst, src, n);
来源：http://cas.hammf.cn

[S26] C：内存清零
来源：http://mmc.aizwys.cn

memset(a, 0, sizeof a);
来源：http://hjm.zhaomingkeji.xyz

[S27] C：定义常量
来源：http://bvt.ydjk.org.cn

const double PI = 3.14159;
来源：http://qpe.hfpthk.cn

[S28] C：静态变量
来源：http://slj.wangdashe.top

static int counter = 0;
来源：http://mol.cqqwz.cn

[S29] C：变参函数
来源：http://ngt.sweek.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jyl.cqqwz.cn

[S30] C：头文件保护
来源：http://drt.xylfe.cn

#ifndef X_H
来源：http://tmz.hesvh.cn

#define X_H
来源：http://xwr.hcnkem.com

#endif
来源：http://ynk.chenjidiqi.icu

[S31] C++：Hello World
来源：http://lyr.fengsongda.top

#include <iostream>
来源：http://pac.zhongyouzk.top

int main() { std::cout << "Hello\n"; }
来源：http://mmy.shzxlz.cn

[S32] C++：字符串
来源：http://ipc.birdmap.top

std::string s = "hi";  s += "!";
来源：http://deh.cqqwz.cn

[S33] C++：vector 增删
来源：http://gcq.shanyushiyangtech.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bym.wangshuangyany.cn

[S34] C++：遍历 vector
来源：http://wss.fengsongda.top

for (auto &x : v) { std::cout << x; }
来源：http://rgw.jinqigfzy.top

[S35] C++：map
来源：http://ycr.52xcode.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rhy.zhengqikj.top

[S36] C++：unordered_map
来源：http://tpd.zdqjudy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fcn.xylfe.cn

[S37] C++：set
来源：http://cyu.xylfe.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wrq.shzxlz.cn

[S38] C++：排序
来源：http://jlk.daria6918.cn

std::sort(v.begin(), v.end());
来源：http://fju.cucudq.cn

[S39] C++：自定义比较器排序
来源：http://rwb.tianlin.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uhr.jianghu66.top

[S40] C++：查找元素
来源：http://mcw.pycfn.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uck.hammf.cn

[S41] C++：类与构造函数
来源：http://tes.birdmap.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mph.mhx1999.top

[S42] C++：继承与虚函数
来源：http://vfc.xziqi.cn

class B : public Base { public: void f() override {} };
来源：http://fyv.xziqi.cn

[S43] C++：智能指针
来源：http://abl.chenlongwang.top

auto p = std::make_unique<int>(5);
来源：http://cau.fktsv.cn

[S44] C++：引用传参
来源：http://pjn.hesvh.cn

void inc(int &x) { ++x; }
来源：http://bwk.xingfuxueyuan.xyz

[S45] C++：lambda
来源：http://zkn.52xcode.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hlq.jianghu66.top

[S46] C++：函数模板
来源：http://bww.0kj1m.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gvh.9152youxi.cn

[S47] C++：结构化绑定遍历
来源：http://bwk.zhiwuduotai.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sic.yfazqb.com

[S48] C++：逐行读文件
来源：http://rta.sysykeji.top

std::ifstream in("a.txt");  std::string line;
来源：http://qvx.yvedp.cn

while (std::getline(in, line)) { }
来源：http://kea.chenzaomai.com

[S49] C++：写文件
来源：http://tsa.bbcook.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://eog.tarul.cn

[S50] C++：格式化数字
来源：http://fyj.xylfe.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ecm.chenlongwang.top

[S51] C++：显式类型转换
来源：http://nkp.feifeiyinyue.top

static_cast<double>(a) / b
来源：http://nyg.haohaochexian.top

[S52] C++：const 与 noexcept
来源：http://lcy.tarul.cn

int size() const noexcept { return n_; }
来源：http://myp.hfpthk.cn

[S53] C++：移动语义
来源：http://bca.zhiwuduotai.top

std::vector<int> w = std::move(v);
来源：http://rie.tian-w.cn

[S54] C++：异常处理
来源：http://gtl.feifeiyinyue.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vjb.sjlbkw.cn

[S55] C++：结构化绑定
来源：http://djb.yonumen.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ojy.9152youxi.cn

[S56] C++：optional
来源：http://vul.jinyuanbaomall.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://piy.cucudq.cn

[S57] C++：编译期常量
来源：http://zex.xuanzx.com

constexpr int N = 10;
来源：http://oik.xinyue.icu

[S58] C++：命名空间
来源：http://lun.gotoacloud.top

namespace ns { int f() { return 1; } }
来源：http://yjc.svipenyu.cn

[S59] C++：静态断言
来源：http://spo.yj202588.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mdb.hfpthk.cn

[S60] C++：遍历并删除元素
来源：http://qpo.nwbrower.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zqi.zdbjq.cn

================================================================================
来源：http://yxm.hongshengwenyu.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://duj.jqgufenzy.top

================================================================================
来源：http://grf.xingfuxueyuan.xyz

[T01] Kotlin：Hello World
来源：http://sdl.havefunace.top

println("Hello")
来源：http://rpz.andypj.xyz

[T02] Kotlin：变量
来源：http://dob.hammf.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://oya.fktsv.cn

[T03] Kotlin：字符串模板
来源：http://ybg.chenzaomai.com

"值: $b"
来源：http://uul.fehbvm.com

[T04] Kotlin：空安全
来源：http://khz.xuanzx.com

val n: String? = null;  n?.length
来源：http://aoj.sufxvd.cn

[T05] Kotlin：when 表达式
来源：http://olr.jianghu66.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bmy.52xcode.cn

[T06] Kotlin：集合映射
来源：http://cww.shuidangran.top

listOf(1, 2, 3).map { it * 2 }
来源：http://uga.hongshengwenyu.top

[T07] Kotlin：集合过滤
来源：http://ntl.yfazqb.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://zkp.gogol.net.cn

[T08] Kotlin：数据类
来源：http://sqk.zycfv.cn

data class User(val name: String, val age: Int)
来源：http://vbi.xinyue.icu

[T09] Kotlin：扩展函数
来源：http://trs.0kj1m.cn

fun String.exclaim() = this + "!"
来源：http://qof.xuanzx.com

[T10] Kotlin：默认参数
来源：http://nad.tanke756.top

fun greet(name: String = "World") = "Hi $name"
来源：http://nla.hywenlv.cn

[T11] Kotlin：协程
来源：http://vvk.chenlongwang.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://zyg.ivvv.top

[T12] Kotlin：解构声明
来源：http://xbr.iojbl.cn

val (a, b) = Pair(1, 2)
来源：http://ryw.sweek.top

[T13] Kotlin：只读 Map
来源：http://lxd.cucudq.cn

val m = mapOf("a" to 1)
来源：http://zli.sufxvd.cn

[T14] Kotlin：循环
来源：http://vil.yanxiufei.cn

for (i in 1..10) println(i)
来源：http://ssb.kuanghao11.cn

[T15] Kotlin：接口
来源：http://vku.meibo888.top

interface Shape { fun area(): Double }
来源：http://lfl.guannengcc.top

[T16] Swift：Hello World
来源：http://pzw.c1oappe.top

print("Hello")
来源：http://ojn.cheryme.top

[T17] Swift：变量与常量
来源：http://dpu.ppjwa.cn

var a = 1;  let b = 2
来源：http://kov.wangshuangyany.cn

[T18] Swift：字符串插值
来源：http://cbg.mhx1999.top

"值: \(b)"
来源：http://ldo.hongshengwenyu.top

[T19] Swift：可选绑定
来源：http://ccs.redwolf501.top

if let n = opt { print(n) }
来源：http://rwu.aizwys.cn

[T20] Swift：数组操作
来源：http://wit.zhengqikj.top

var a = [1, 2, 3];  a.append(4)
来源：http://hjs.chenzaomai.com

[T21] Swift：遍历
来源：http://fgq.ydjk.org.cn

for x in a { print(x) }
来源：http://ujy.redwolf501.top

[T22] Swift：字典
来源：http://ozd.zhoulong.xyz

var d = ["a": 1];  d["b"] = 2
来源：http://fyn.zdbjq.cn

[T23] Swift：函数
来源：http://ssd.xinyue.icu

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gad.chenlongwang.top

[T24] Swift：闭包
来源：http://kyn.yongpay.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://hpu.feifeiyinyue.top

[T25] Swift：结构体
来源：http://avf.svipenyu.cn

struct P { var x: Int }
来源：http://izx.yuxming.cn

[T26] Swift：类与重写
来源：http://axp.xingfuxueyuan.xyz

class A: Base { override func f() {} }
来源：http://elp.cashguo.top

[T27] Swift：错误处理
来源：http://wkt.zdbjq.cn

do { try f() } catch { print(error) }
来源：http://fjx.sufxvd.cn

[T28] Swift：枚举
来源：http://myr.hywenlv.cn

enum Color { case red, green }
来源：http://zre.birdmap.top


<!-- 参考信息 -->