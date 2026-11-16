代发 wailian999

echo "${#s}"
来源：http://jon.aibaodan.cn

[R22] 截取子串
来源：http://nya.sxryk.cn

echo "${s:0:5}"
来源：http://xue.sxryk.cn

[R23] 字符串替换
来源：http://ejp.yj20258888.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dnm.jqgfzy.top

[R24] 大小写转换
来源：http://lxm.haohaochexian.top

echo "${s^^}"; echo "${s,,}"
来源：http://tbo.quarkkingdee.top

[R25] 去后缀 / 去前缀
来源：http://jow.dianchejie.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://mkm.chenjidiqi.icu

[R26] 命令替换
来源：http://wcd.cdnleiting.top

now=$(date +%F); echo "$now"
来源：http://fsy.yanxiufei.cn

[R27] 算术展开
来源：http://jkn.cqqwz.cn

echo $((1 + 2 * 3))
来源：http://ust.nanxinkj.top

[R28] 浮点运算
来源：http://wux.nwbrower.top

echo "scale=2; 10/3" | bc
来源：http://svk.tianlin.xyz

[R29] 定义函数
来源：http://shs.shanyushiyangkeji.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://arr.chenlongwang.top

[R30] 函数返回状态码
来源：http://mns.jinyuanbaomall.cn

f() { return 0; }; f || echo "失败了"
来源：http://sxm.uphjek.com

[R31] 局部变量
来源：http://acw.tian-w.cn

f() { local x=1; echo "$x"; }
来源：http://kba.c1oappe.top

[R32] 参数个数校验
来源：http://vfa.hcnkem.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rlg.jinyuanbaomall.cn

[R33] 捕获错误并提示行号
来源：http://khb.9152youxi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yoe.shanyushiyangtech.top

[R34] 退出时清理
来源：http://tls.ivvv.top

trap 'rm -f "$tmp"' EXIT
来源：http://hjb.316326.xyz

[R35] 后台执行并等待
来源：http://pkn.jinghuilouyu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ufj.xziqi.cn

[R36] 并发执行多个任务
来源：http://sbg.iojbl.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xsx.shanyushiyangkeji.top

[R37] 把输出赋给变量
来源：http://fer.shzxlz.cn

files=$(ls -1)
来源：http://jcn.meibo888.top

[R38] 管道串联
来源：http://jon.hnxiangtu.top

cat a.txt | grep -i error | wc -l
来源：http://bru.haohaochexian.top

[R39] 重定向标准输出与错误
来源：http://vom.quarkkingdee.top

cmd > out.log 2>&1
来源：http://kku.ehwqpu.com

[R40] 追加写日志
来源：http://okf.zdbjq.cn

echo "log" >> out.log
来源：http://qum.svipenyu.cn

[R41] 丢弃输出
来源：http://gqq.cucudq.cn

cmd >/dev/null 2>&1
来源：http://zyx.pycfn.com

[R42] 输入重定向
来源：http://yay.hcnkem.com

wc -l < a.txt
来源：http://lio.gzhubu.top

[R43] 按名字查找文件
来源：http://tou.guowangkeji.top

find . -name "*.log" -type f
来源：http://ohn.gaohongyu789.top

[R44] 按修改时间查找
来源：http://ham.zhaomingkeji.xyz

find . -mtime -7 -type f
来源：http://cko.yonumen.top

[R45] 批量删除
来源：http://lok.sweek.top

find . -name "*.tmp" -delete
来源：http://nzj.nanxuanxn.top

[R46] 递归替换文件内容
来源：http://wpu.bjfxy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xmn.yuanzhike.top

[R47] sed 单行替换
来源：http://qgz.hfpthk.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mri.guannengcc.top

[R48] awk 取指定列
来源：http://uxo.feifeiyinyue.top

awk '{print $1, $3}' a.txt
来源：http://ilp.c1oappe.top

[R49] awk 带条件
来源：http://tuf.redwolf501.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://abm.gzhubu.top

[R50] awk 求和
来源：http://flt.ivvv.top

awk '{s += $2} END {print s}' a.txt
来源：http://lej.uphjek.com

[R51] 排序去重取前几
来源：http://mee.vqdsnc.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://orp.dianchejie.cn

[R52] 统计行数
来源：http://uge.yueranfly.top

wc -l a.txt
来源：http://hus.redwolf501.top

[R53] 查看文件头与实时尾
来源：http://lsq.yanxiufei.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ies.shanyushiyangtech.top

[R54] 比较两个文件
来源：http://ovq.yuxming.cn

diff a.txt b.txt
来源：http://kub.zdqjudy.top

[R55] 压缩与解压
来源：http://fsu.jinqigufen.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tmz.zycfv.cn

[R56] 远程拷贝
来源：http://ayc.yj202588.top

scp file user@host:/path/
来源：http://dmm.sufxvd.cn

[R57] 远程执行命令
来源：http://alj.zdqjudy.top

ssh user@host 'uptime'
来源：http://xwe.jlsjyb.cn

[R58] 下载文件
来源：http://akm.chenzaomai.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ewo.hfpthk.cn

[R59] 发 POST JSON
来源：http://ygm.52xcode.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pst.havefunace.top

[R60] 只看 HTTP 状态码
来源：http://hog.jqgufenzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pqv.jinqigufen.top

[R61] 磁盘占用
来源：http://iil.shuidangran.top

df -h;  du -sh *
来源：http://ils.chenlongwang.top

[R62] 找最占空间的文件
来源：http://hlv.316326.xyz

du -ah . | sort -rh | head -10
来源：http://xqn.hongshengwenyu.top

[R63] 内存与进程
来源：http://exm.snrcjt.cn

free -h;  ps aux | grep nginx
来源：http://lmp.ppjwa.cn

[R64] 结束进程
来源：http://qqa.sufxvd.cn

kill -9 $(pgrep -f app.py)
来源：http://hut.bjfxy.top

[R65] 查看端口占用
来源：http://gun.tanke756.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://edj.iojbl.cn

[R66] 定时任务
来源：http://gls.yfazqb.com

crontab -e;  crontab -l
来源：http://nwd.fehbvm.com

[R67] 生成随机十六进制串
来源：http://oqj.yuanzhike.top

openssl rand -hex 16
来源：http://cba.ydjk.org.cn

[R68] 计算文件校验值
来源：http://rbo.xingfuxueyuan.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://vic.aibaodan.cn

[R69] 生成随机密码
来源：http://mvs.bbcook.cn

head -c 16 /dev/urandom | base64
来源：http://zgs.aibaodan.cn

[R70] 时间戳与互转
来源：http://acp.tian-w.cn

date +%s;  date -d @1700000000
来源：http://snk.yuxming.cn

[R71] 日期格式化
来源：http://bjp.daxiang520.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://blc.meibo888.top

[R72] 等待端口就绪
来源：http://qcf.ivvv.top

until nc -z localhost 3306; do sleep 1; done
来源：http://wvt.gotoacloud.top

[R73] 分割大日志
来源：http://mde.smart0.xyz

split -l 1000 big.log part_
来源：http://fjt.hywenlv.cn

[R74] 批量重命名
来源：http://eop.c1oappe.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://adx.316326.xyz

[R75] 导出环境变量
来源：http://koc.meibo888.top

export PATH="$HOME/bin:$PATH"
来源：http://num.9152youxi.cn

[R76] 使用临时文件
来源：http://nqe.pengpengdd.cyou

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vhx.hammf.cn

[R77] 读取用户输入
来源：http://puo.yuxming.cn

read -rp "请输入: " ans
来源：http://thj.zdqjudy.top

[R78] 交互式菜单
来源：http://onb.yfazqb.com

select opt in a b c; do echo "$opt"; break; done
来源：http://aki.epnwcf.com

[R79] 解析命令行选项
来源：http://tbr.chenlongwang.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nqg.kuanghao11.cn

[R80] 查看脚本执行耗时
来源：http://wie.mhx1999.top

time ./run.sh
来源：http://qnq.yuxming.cn

================================================================================
来源：http://wdq.cheryme.top

S. C / C++ 专题
来源：http://bjl.sxryk.cn

================================================================================
来源：http://cxl.gzhubu.top

[S01] C：Hello World
来源：http://eez.mhx1999.top

#include <stdio.h>
来源：http://nyg.bjfxy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://dxm.yj20258888.top

[S02] C：变量与格式化输出
来源：http://psh.jinyuanbaomall.cn

int a = 10; printf("%d\n", a);
来源：http://ihd.316326.xyz

[S03] C：读入整数
来源：http://xpp.sjlbkw.cn

int x; scanf("%d", &x);
来源：http://jbw.zhijiandao.cn

[S04] C：字符串复制
来源：http://wmz.hammf.cn

char dst[32]; strcpy(dst, "hi");
来源：http://akv.daria6918.cn

[S05] C：字符串长度
来源：http://bbe.andypj.xyz

strlen(s)
来源：http://prm.zhixingplan.top

[S06] C：字符串比较
来源：http://spi.mhx1999.top

strcmp(a, b) == 0
来源：http://ffm.hywenlv.cn

[S07] C：数组遍历求和
来源：http://vky.cdnleiting.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://goy.yj20258.top

[S08] C：动态内存分配与释放
来源：http://pdr.tian-w.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pxb.xziqi.cn

[S09] C：结构体定义与初始化
来源：http://wny.yj20258.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://geg.yj20258888.top

[S10] C：指针与解引用
来源：http://szg.xziqi.cn

int *p = &a;  *p = 5;
来源：http://eta.cheryme.top

[S11] C：逐行读文件
来源：http://pep.sweek.top

FILE *f = fopen("a.txt", "r");
来源：http://voh.birdmap.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://aht.tianlin.xyz

fclose(f);
来源：http://nyz.fehbvm.com

[S12] C：写文件
来源：http://ycr.yuanzhike.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xkf.zdbjq.cn

[S13] C：宏定义
来源：http://kvj.hnxiangtu.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fqu.jinqigfzy.top

[S14] C：枚举
来源：http://ain.uphjek.com

enum Color { RED, GREEN, BLUE };
来源：http://ifb.xziqi.cn

[S15] C：类型转换
来源：http://qcj.ctjpmb.com

(double) a / b
来源：http://ywg.shanyushiyangtech.top

[S16] C：位操作置位
来源：http://lyc.hnqzz.top

x |= (1 << 3);
来源：http://jmx.yj20258.top

[S17] C：安全拼接字符串
来源：http://nig.zdbjq.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hgm.jiagoushi.top

[S18] C：命令行参数
来源：http://tya.wangdashe.top

int main(int argc, char **argv)
来源：http://syf.fengsongda.top

[S19] C：快速排序
来源：http://fzj.birdmap.top

qsort(a, n, sizeof(int), cmp);
来源：http://cpo.bbcook.cn

[S20] C：二分查找
来源：http://rpi.nanxuanxn.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xbn.gotoacloud.top

[S21] C：字符类别判断
来源：http://dfg.cqqwz.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xjg.yuxming.cn

[S22] C：字符串转数字
来源：http://byv.yonumen.top

atoi("42");  strtod("3.14", NULL);
来源：http://uxb.vehdjk.com

[S23] C：随机数
来源：http://uvf.aizwys.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zgv.fktsv.cn

[S24] C：获取本地时间
来源：http://cmw.fzhhl.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ojq.sufxvd.cn

[S25] C：内存拷贝
来源：http://esx.yanxiufei.cn

memcpy(dst, src, n);
来源：http://olp.ybcxt.top

[S26] C：内存清零
来源：http://ojx.fengsongda.top

memset(a, 0, sizeof a);
来源：http://qqb.52xcode.cn

[S27] C：定义常量
来源：http://xhd.fengsongda.top

const double PI = 3.14159;
来源：http://aug.wangdashe.top

[S28] C：静态变量
来源：http://byz.jqgufenzy.top

static int counter = 0;
来源：http://rxh.tianlin.xyz

[S29] C：变参函数
来源：http://nrh.birdmap.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://iwf.fengsongda.top

[S30] C：头文件保护
来源：http://rjl.tian-w.cn

#ifndef X_H
来源：http://wcn.hysaishi.cn

#define X_H
来源：http://zto.jqgfzy.top

#endif
来源：http://lkq.xziqi.cn

[S31] C++：Hello World
来源：http://tqm.xuanzx.com

#include <iostream>
来源：http://byk.andypj.xyz

int main() { std::cout << "Hello\n"; }
来源：http://gfi.nanxuanxn.top

[S32] C++：字符串
来源：http://eoc.jianghu66.top

std::string s = "hi";  s += "!";
来源：http://rpj.fehbvm.com

[S33] C++：vector 增删
来源：http://whr.jinyuanbaomall.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ihm.chenlongwang.top

[S34] C++：遍历 vector
来源：http://dmq.chenjidiqi.icu

for (auto &x : v) { std::cout << x; }
来源：http://vin.hesvh.cn

[S35] C++：map
来源：http://khw.fanxiaobao.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fwu.yj202588.top

[S36] C++：unordered_map
来源：http://eqn.quarkkingdee.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vwh.ctjpmb.com

[S37] C++：set
来源：http://aia.guannengcc.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bsa.yangfankeji.com

[S38] C++：排序
来源：http://pno.zdbjq.cn

std::sort(v.begin(), v.end());
来源：http://xpq.jqgufenzy.top

[S39] C++：自定义比较器排序
来源：http://ily.yuxming.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pvv.shangyingyoupin.top

[S40] C++：查找元素
来源：http://dfr.xinyue.icu

auto it = std::find(v.begin(), v.end(), 3);
来源：http://qgr.yuanzhike.top

[S41] C++：类与构造函数
来源：http://eei.yuanzhike.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rst.ywan-chungtsiang.top

[S42] C++：继承与虚函数
来源：http://wlz.zhixingplan.top

class B : public Base { public: void f() override {} };
来源：http://ogh.gogol.net.cn

[S43] C++：智能指针
来源：http://cex.hywenlv.cn

auto p = std::make_unique<int>(5);
来源：http://hyr.yuanzhike.top

[S44] C++：引用传参
来源：http://gdv.c1oappe.top

void inc(int &x) { ++x; }
来源：http://wmp.pycfn.com

[S45] C++：lambda
来源：http://mpo.zhixingplan.top

auto add = [](int a, int b) { return a + b; };
来源：http://gsc.mhx1999.top

[S46] C++：函数模板
来源：http://yob.hysaishi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nxl.yfazqb.com

[S47] C++：结构化绑定遍历
来源：http://qzd.quarkkingdee.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://apo.wangshuangyany.cn

[S48] C++：逐行读文件
来源：http://fbm.jinqigufen.top

std::ifstream in("a.txt");  std::string line;
来源：http://szt.shuidangran.top

while (std::getline(in, line)) { }
来源：http://tja.hesvh.cn

[S49] C++：写文件
来源：http://zlw.meibo888.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ofc.dashuyun.cn

[S50] C++：格式化数字
来源：http://usc.shanyushiyangkeji.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://thw.cashguo.top

[S51] C++：显式类型转换
来源：http://hrz.xuanzx.com

static_cast<double>(a) / b
来源：http://ilp.daria6918.cn

[S52] C++：const 与 noexcept
来源：http://adg.gotoacloud.top

int size() const noexcept { return n_; }
来源：http://yqj.316326.xyz

[S53] C++：移动语义
来源：http://ucu.mhx1999.top

std::vector<int> w = std::move(v);
来源：http://ezq.aibaodan.cn

[S54] C++：异常处理
来源：http://bvh.jlsjyb.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yyk.jiagoushi.top

[S55] C++：结构化绑定
来源：http://bdr.havefunace.top

auto [a, b] = std::make_pair(1, 2);
来源：http://ksg.yanxiufei.cn

[S56] C++：optional
来源：http://ukj.wangshuangyany.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cbb.yfazqb.com

[S57] C++：编译期常量
来源：http://hup.svipenyu.cn

constexpr int N = 10;
来源：http://etu.birdmap.top

[S58] C++：命名空间
来源：http://yxz.nanxuanxn.top

namespace ns { int f() { return 1; } }
来源：http://lud.pengpengdd.cyou

[S59] C++：静态断言
来源：http://gro.hysaishi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://reg.ydzc1.top

[S60] C++：遍历并删除元素
来源：http://krf.yj202588.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vwl.nwbrower.top

================================================================================
来源：http://ezg.xinyue.icu

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yer.sjlbkw.cn

================================================================================
来源：http://nzz.jinghuilouyu.cn

[T01] Kotlin：Hello World
来源：http://jib.fehbvm.com

println("Hello")
来源：http://rig.ctjpmb.com

[T02] Kotlin：变量
来源：http://ntu.ctjpmb.com

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wkj.zhoulong.xyz

[T03] Kotlin：字符串模板
来源：http://iya.tian-w.cn

"值: $b"
来源：http://zam.shanyushiyangkeji.top

[T04] Kotlin：空安全
来源：http://ocg.fanxiaobao.xyz

val n: String? = null;  n?.length
来源：http://who.cashguo.top

[T05] Kotlin：when 表达式
来源：http://qeg.hammf.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fqi.jqgufenzy.top

[T06] Kotlin：集合映射
来源：http://fxv.cdnleiting.top

listOf(1, 2, 3).map { it * 2 }
来源：http://lcn.yj202588.top

[T07] Kotlin：集合过滤
来源：http://pox.c1oappe.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://vpa.yangfankeji.com

[T08] Kotlin：数据类
来源：http://yfs.ydzc1.top

data class User(val name: String, val age: Int)
来源：http://ied.dashuyun.cn

[T09] Kotlin：扩展函数
来源：http://kqs.yangfankeji.com

fun String.exclaim() = this + "!"
来源：http://ryb.havefunace.top

[T10] Kotlin：默认参数
来源：http://cgo.svipenyu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://uyw.wangshuangyany.cn

[T11] Kotlin：协程
来源：http://qcq.zdqjudy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://rhn.aizwys.cn

[T12] Kotlin：解构声明
来源：http://tlj.jyoumei.cn

val (a, b) = Pair(1, 2)
来源：http://tjz.jqgfzy.top

[T13] Kotlin：只读 Map
来源：http://tbk.jinghuilouyu.cn

val m = mapOf("a" to 1)
来源：http://ajd.cucudq.cn

[T14] Kotlin：循环
来源：http://oou.andypj.xyz

for (i in 1..10) println(i)
来源：http://tot.epnwcf.com

[T15] Kotlin：接口
来源：http://utw.iojbl.cn

interface Shape { fun area(): Double }
来源：http://kyv.xuanzx.com

[T16] Swift：Hello World
来源：http://jml.9152youxi.cn

print("Hello")
来源：http://hrw.shanyushiyangkeji.top

[T17] Swift：变量与常量
来源：http://czp.jinyuanbaomall.cn

var a = 1;  let b = 2
来源：http://jga.sysykeji.top

[T18] Swift：字符串插值
来源：http://jmk.guannengcc.top

"值: \(b)"
来源：http://pcy.nanxuanxn.top

[T19] Swift：可选绑定
来源：http://con.dianchejie.cn

if let n = opt { print(n) }
来源：http://jfy.xziqi.cn

[T20] Swift：数组操作
来源：http://zej.jinqigufen.top

var a = [1, 2, 3];  a.append(4)
来源：http://ror.dianchejie.cn

[T21] Swift：遍历
来源：http://qrz.guannengcc.top

for x in a { print(x) }
来源：http://dbf.shzxlz.cn

[T22] Swift：字典
来源：http://ndr.hnqzz.top

var d = ["a": 1];  d["b"] = 2
来源：http://lva.zhixingplan.top

[T23] Swift：函数
来源：http://lwt.yonumen.top

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://tef.hnxiangtu.top

[T24] Swift：闭包
来源：http://hmb.daxiang520.top

let f = { (x: Int) -> Int in x * 2 }
来源：http://vxk.gotoacloud.top


<!-- 参考信息 -->