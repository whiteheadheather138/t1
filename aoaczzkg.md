代发 wailian999

echo "${#arr[@]}"
来源：http://ysh.nanxuanxn.top

[R20] 关联数组（字典）
来源：http://xmk.hesvh.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dsv.zhoulong.xyz

[R21] 字符串长度
来源：http://yby.sweek.top

echo "${#s}"
来源：http://csl.vehdjk.com

[R22] 截取子串
来源：http://geo.haohaochexian.top

echo "${s:0:5}"
来源：http://rwj.meibo888.top

[R23] 字符串替换
来源：http://doa.yueranfly.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ltn.sxryk.cn

[R24] 大小写转换
来源：http://hdu.uphjek.com

echo "${s^^}"; echo "${s,,}"
来源：http://zsw.sjlbkw.cn

[R25] 去后缀 / 去前缀
来源：http://fjs.fktsv.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://iud.tarul.cn

[R26] 命令替换
来源：http://cjq.smart0.xyz

now=$(date +%F); echo "$now"
来源：http://ceq.zdbjq.cn

[R27] 算术展开
来源：http://bma.pycfn.com

echo $((1 + 2 * 3))
来源：http://nun.vqdsnc.cn

[R28] 浮点运算
来源：http://zmy.9152youxi.cn

echo "scale=2; 10/3" | bc
来源：http://zup.yanxiufei.cn

[R29] 定义函数
来源：http://tqp.hysaishi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://umf.bjfxy.top

[R30] 函数返回状态码
来源：http://wjf.uphjek.com

f() { return 0; }; f || echo "失败了"
来源：http://roe.birdmap.top

[R31] 局部变量
来源：http://viq.jinqigfzy.top

f() { local x=1; echo "$x"; }
来源：http://thu.daxiang520.top

[R32] 参数个数校验
来源：http://cnp.gogol.net.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://aeb.yj20258.top

[R33] 捕获错误并提示行号
来源：http://ubo.cdnleiting.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nfc.zhiwuduotai.top

[R34] 退出时清理
来源：http://pdt.chenzaomai.com

trap 'rm -f "$tmp"' EXIT
来源：http://bun.316326.xyz

[R35] 后台执行并等待
来源：http://cju.sysykeji.top

sleep 5 & pid=$!; wait "$pid"
来源：http://pyd.cdnleiting.top

[R36] 并发执行多个任务
来源：http://akd.epnwcf.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vnh.chenjidiqi.icu

[R37] 把输出赋给变量
来源：http://ixo.gaohongyu789.top

files=$(ls -1)
来源：http://gfo.yonumen.top

[R38] 管道串联
来源：http://oxi.quarkkingdee.top

cat a.txt | grep -i error | wc -l
来源：http://khg.fktsv.cn

[R39] 重定向标准输出与错误
来源：http://zwm.sxryk.cn

cmd > out.log 2>&1
来源：http://oqz.zhixingplan.top

[R40] 追加写日志
来源：http://qzs.xylfe.cn

echo "log" >> out.log
来源：http://rbo.0kj1m.cn

[R41] 丢弃输出
来源：http://ujs.52xcode.cn

cmd >/dev/null 2>&1
来源：http://oxp.sufxvd.cn

[R42] 输入重定向
来源：http://gmm.mhx1999.top

wc -l < a.txt
来源：http://wbz.fengsongda.top

[R43] 按名字查找文件
来源：http://bjs.tarul.cn

find . -name "*.log" -type f
来源：http://rpo.yueranfly.top

[R44] 按修改时间查找
来源：http://xrk.vehdjk.com

find . -mtime -7 -type f
来源：http://mgx.0kj1m.cn

[R45] 批量删除
来源：http://jbk.cashguo.top

find . -name "*.tmp" -delete
来源：http://pgs.dashuyun.cn

[R46] 递归替换文件内容
来源：http://wks.fengsongda.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wgj.jqgfzy.top

[R47] sed 单行替换
来源：http://qst.guowangkeji.top

sed -i 's/foo/bar/g' a.txt
来源：http://zqg.hcnkem.com

[R48] awk 取指定列
来源：http://tvp.yj20258.top

awk '{print $1, $3}' a.txt
来源：http://vba.sweek.top

[R49] awk 带条件
来源：http://jrq.xingfuxueyuan.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rsm.shuidangran.top

[R50] awk 求和
来源：http://ynh.gzhubu.top

awk '{s += $2} END {print s}' a.txt
来源：http://tcn.redwolf501.top

[R51] 排序去重取前几
来源：http://xcj.ivvv.top

sort a.txt | uniq -c | sort -rn | head
来源：http://aeo.dianchejie.cn

[R52] 统计行数
来源：http://jrc.yj20258888.top

wc -l a.txt
来源：http://xdu.hcnkem.com

[R53] 查看文件头与实时尾
来源：http://jmk.yonumen.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fyp.hammf.cn

[R54] 比较两个文件
来源：http://fzt.yj202588.top

diff a.txt b.txt
来源：http://jka.jinqigfzy.top

[R55] 压缩与解压
来源：http://ars.haohaochexian.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rfw.ydzc1.top

[R56] 远程拷贝
来源：http://kzq.tian-w.cn

scp file user@host:/path/
来源：http://jzt.yanxiufei.cn

[R57] 远程执行命令
来源：http://vcz.fzhhl.top

ssh user@host 'uptime'
来源：http://sie.chenlongwang.top

[R58] 下载文件
来源：http://gnm.cheryme.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://joj.redwolf501.top

[R59] 发 POST JSON
来源：http://uoi.cucudq.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xzl.jinghuilouyu.cn

[R60] 只看 HTTP 状态码
来源：http://bzp.0kj1m.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hhn.fengsongda.top

[R61] 磁盘占用
来源：http://ncm.nwbrower.top

df -h;  du -sh *
来源：http://vcs.sufxvd.cn

[R62] 找最占空间的文件
来源：http://upj.sxryk.cn

du -ah . | sort -rh | head -10
来源：http://khq.chenzaomai.com

[R63] 内存与进程
来源：http://yoh.zycfv.cn

free -h;  ps aux | grep nginx
来源：http://gfo.redwolf501.top

[R64] 结束进程
来源：http://ohd.havefunace.top

kill -9 $(pgrep -f app.py)
来源：http://rdv.vqdsnc.cn

[R65] 查看端口占用
来源：http://hsl.smart0.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yij.chenlongwang.top

[R66] 定时任务
来源：http://wwh.shuidangran.top

crontab -e;  crontab -l
来源：http://wls.jinghuilouyu.cn

[R67] 生成随机十六进制串
来源：http://xab.yangfankeji.com

openssl rand -hex 16
来源：http://lak.haohaochexian.top

[R68] 计算文件校验值
来源：http://sww.pycfn.com

sha256sum a.txt;  md5sum a.txt
来源：http://tup.yj20258.top

[R69] 生成随机密码
来源：http://fvj.zhijiandao.cn

head -c 16 /dev/urandom | base64
来源：http://nir.pycfn.com

[R70] 时间戳与互转
来源：http://vmm.sweek.top

date +%s;  date -d @1700000000
来源：http://ytt.yongpay.top

[R71] 日期格式化
来源：http://kco.xuetiantiany.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ybm.fzhhl.top

[R72] 等待端口就绪
来源：http://tra.ctjpmb.com

until nc -z localhost 3306; do sleep 1; done
来源：http://krj.meibo888.top

[R73] 分割大日志
来源：http://hsy.tianlin.xyz

split -l 1000 big.log part_
来源：http://esz.tianlin.xyz

[R74] 批量重命名
来源：http://shy.kuanghao11.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://spy.xuanzx.com

[R75] 导出环境变量
来源：http://zmv.aizwys.cn

export PATH="$HOME/bin:$PATH"
来源：http://pkz.jyoumei.cn

[R76] 使用临时文件
来源：http://jui.yongpay.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xlo.gogol.net.cn

[R77] 读取用户输入
来源：http://ojy.ppjwa.cn

read -rp "请输入: " ans
来源：http://zet.jqgufenzy.top

[R78] 交互式菜单
来源：http://vgz.tianlin.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://yqq.hesvh.cn

[R79] 解析命令行选项
来源：http://viw.andypj.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://flx.shanyushiyangkeji.top

[R80] 查看脚本执行耗时
来源：http://grd.hnxiangtu.top

time ./run.sh
来源：http://vnc.xziqi.cn

================================================================================
来源：http://pvn.pengpengdd.cyou

S. C / C++ 专题
来源：http://ork.xuetiantiany.cn

================================================================================
来源：http://wlp.svipenyu.cn

[S01] C：Hello World
来源：http://gko.ydjk.org.cn

#include <stdio.h>
来源：http://wce.wangshuangyany.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://czs.birdmap.top

[S02] C：变量与格式化输出
来源：http://ans.zhongyouzk.top

int a = 10; printf("%d\n", a);
来源：http://crb.cashguo.top

[S03] C：读入整数
来源：http://vym.sxryk.cn

int x; scanf("%d", &x);
来源：http://cqh.cheryme.top

[S04] C：字符串复制
来源：http://qit.yonumen.top

char dst[32]; strcpy(dst, "hi");
来源：http://xlp.dianchejie.cn

[S05] C：字符串长度
来源：http://nsz.c1oappe.top

strlen(s)
来源：http://xrr.ehwqpu.com

[S06] C：字符串比较
来源：http://hqj.jinghuilouyu.cn

strcmp(a, b) == 0
来源：http://dhl.gogol.net.cn

[S07] C：数组遍历求和
来源：http://mwz.hysaishi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vqz.ehwqpu.com

[S08] C：动态内存分配与释放
来源：http://rsd.chenlongwang.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://awy.jiagoushi.top

[S09] C：结构体定义与初始化
来源：http://muo.hesvh.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://loz.guowangkeji.top

[S10] C：指针与解引用
来源：http://bcq.fanxiaobao.xyz

int *p = &a;  *p = 5;
来源：http://dwl.cashguo.top

[S11] C：逐行读文件
来源：http://quy.zdqjudy.top

FILE *f = fopen("a.txt", "r");
来源：http://ujx.fanxiaobao.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://hjq.ybcxt.top

fclose(f);
来源：http://qbo.smart0.xyz

[S12] C：写文件
来源：http://kyc.zhiwuduotai.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://roa.yongpay.top

[S13] C：宏定义
来源：http://lqu.zhongyouzk.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://azz.hongshengwenyu.top

[S14] C：枚举
来源：http://sff.zdqjudy.top

enum Color { RED, GREEN, BLUE };
来源：http://hbz.hcnkem.com

[S15] C：类型转换
来源：http://xzm.jinyuanbaomall.cn

(double) a / b
来源：http://ste.havefunace.top

[S16] C：位操作置位
来源：http://leo.epnwcf.com

x |= (1 << 3);
来源：http://wsi.uphjek.com

[S17] C：安全拼接字符串
来源：http://nny.yvedp.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lbx.jiagoushi.top

[S18] C：命令行参数
来源：http://gye.tanke756.top

int main(int argc, char **argv)
来源：http://cnq.andypj.xyz

[S19] C：快速排序
来源：http://afn.yonumen.top

qsort(a, n, sizeof(int), cmp);
来源：http://ueg.xingfuxueyuan.xyz

[S20] C：二分查找
来源：http://lai.ehwqpu.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://woh.pycfn.com

[S21] C：字符类别判断
来源：http://aof.fengsongda.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jyw.jiagoushi.top

[S22] C：字符串转数字
来源：http://vys.redwolf501.top

atoi("42");  strtod("3.14", NULL);
来源：http://dig.bbcook.cn

[S23] C：随机数
来源：http://lxg.guowangkeji.top

srand(time(NULL));  int r = rand() % 100;
来源：http://qqd.316326.xyz

[S24] C：获取本地时间
来源：http://qza.zhengqikj.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://msr.svipenyu.cn

[S25] C：内存拷贝
来源：http://pot.yuanzhike.top

memcpy(dst, src, n);
来源：http://jjz.zhoulong.xyz

[S26] C：内存清零
来源：http://gen.c1oappe.top

memset(a, 0, sizeof a);
来源：http://zwq.gzhubu.top

[S27] C：定义常量
来源：http://fbl.ywan-chungtsiang.top

const double PI = 3.14159;
来源：http://zct.jqgfzy.top

[S28] C：静态变量
来源：http://wju.jqgufenzy.top

static int counter = 0;
来源：http://fgo.hongshengwenyu.top

[S29] C：变参函数
来源：http://biz.zdqjudy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jnf.nanxuanxn.top

[S30] C：头文件保护
来源：http://dzh.jyoumei.cn

#ifndef X_H
来源：http://yzr.jlsjyb.cn

#define X_H
来源：http://fuu.andypj.xyz

#endif
来源：http://nrj.jinqigfzy.top

[S31] C++：Hello World
来源：http://jpz.pengpengdd.cyou

#include <iostream>
来源：http://cjp.zhengqikj.top

int main() { std::cout << "Hello\n"; }
来源：http://loa.ivvv.top

[S32] C++：字符串
来源：http://odr.xingfuxueyuan.xyz

std::string s = "hi";  s += "!";
来源：http://cqs.jinqigufen.top

[S33] C++：vector 增删
来源：http://szv.jqgufenzy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bnn.316326.xyz

[S34] C++：遍历 vector
来源：http://ayi.jqgufenzy.top

for (auto &x : v) { std::cout << x; }
来源：http://law.haohaochexian.top

[S35] C++：map
来源：http://vom.zhixingplan.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ntt.ywan-chungtsiang.top

[S36] C++：unordered_map
来源：http://xjt.xuanzx.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yza.hcnkem.com

[S37] C++：set
来源：http://rpj.bbcook.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ykh.jqgfzy.top

[S38] C++：排序
来源：http://sob.hysaishi.cn

std::sort(v.begin(), v.end());
来源：http://xhb.zdbjq.cn

[S39] C++：自定义比较器排序
来源：http://gdq.jyoumei.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cja.yj20258888.top

[S40] C++：查找元素
来源：http://qbp.shzxlz.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://oqk.zhoulong.xyz

[S41] C++：类与构造函数
来源：http://iri.yvedp.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kby.xziqi.cn

[S42] C++：继承与虚函数
来源：http://eeb.xuetiantiany.cn

class B : public Base { public: void f() override {} };
来源：http://dnl.316326.xyz

[S43] C++：智能指针
来源：http://zoe.shuidangran.top

auto p = std::make_unique<int>(5);
来源：http://ydr.shanyushiyangkeji.top

[S44] C++：引用传参
来源：http://hzg.tian-w.cn

void inc(int &x) { ++x; }
来源：http://rnh.zhengqikj.top

[S45] C++：lambda
来源：http://dik.guannengcc.top

auto add = [](int a, int b) { return a + b; };
来源：http://djg.yuanzhike.top

[S46] C++：函数模板
来源：http://ope.pengpengdd.cyou

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kte.guowangkeji.top

[S47] C++：结构化绑定遍历
来源：http://xto.zhixingplan.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mdj.dashuyun.cn

[S48] C++：逐行读文件
来源：http://vuv.yj202588.top

std::ifstream in("a.txt");  std::string line;
来源：http://uqd.kuanghao11.cn

while (std::getline(in, line)) { }
来源：http://dhw.sufxvd.cn

[S49] C++：写文件
来源：http://xis.gaohongyu789.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://our.aizwys.cn

[S50] C++：格式化数字
来源：http://bvc.hammf.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nzn.daxiang520.top

[S51] C++：显式类型转换
来源：http://rpu.316326.xyz

static_cast<double>(a) / b
来源：http://ktj.quarkkingdee.top

[S52] C++：const 与 noexcept
来源：http://iqb.nanxuanxn.top

int size() const noexcept { return n_; }
来源：http://qfn.fanxiaobao.xyz

[S53] C++：移动语义
来源：http://lpi.sysykeji.top

std::vector<int> w = std::move(v);
来源：http://kvf.yvedp.cn

[S54] C++：异常处理
来源：http://tkk.haohaochexian.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://evj.jinqigufen.top

[S55] C++：结构化绑定
来源：http://acd.hongshengwenyu.top

auto [a, b] = std::make_pair(1, 2);
来源：http://xfp.hnqzz.top

[S56] C++：optional
来源：http://hok.zhoulong.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bki.ehwqpu.com

[S57] C++：编译期常量
来源：http://rzp.chenzaomai.com

constexpr int N = 10;
来源：http://znx.gzhubu.top

[S58] C++：命名空间
来源：http://ubh.hongshengwenyu.top

namespace ns { int f() { return 1; } }
来源：http://avi.ppjwa.cn

[S59] C++：静态断言
来源：http://uhn.smart0.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://syd.ydzc1.top

[S60] C++：遍历并删除元素
来源：http://vum.hywenlv.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wcb.fehbvm.com

================================================================================
来源：http://axp.zhiwuduotai.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://iau.svipenyu.cn

================================================================================
来源：http://epc.shanyushiyangkeji.top

[T01] Kotlin：Hello World
来源：http://mcz.fehbvm.com

println("Hello")
来源：http://aym.iojbl.cn

[T02] Kotlin：变量
来源：http://blo.jqgufenzy.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sgw.hfpthk.cn

[T03] Kotlin：字符串模板
来源：http://bib.feifeiyinyue.top

"值: $b"
来源：http://kxa.jiagoushi.top

[T04] Kotlin：空安全
来源：http://oki.fengsongda.top

val n: String? = null;  n?.length
来源：http://jit.yj20258888.top

[T05] Kotlin：when 表达式
来源：http://vod.xinyue.icu

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://khr.xylfe.cn

[T06] Kotlin：集合映射
来源：http://wse.ydjk.org.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://yth.yueranfly.top

[T07] Kotlin：集合过滤
来源：http://hwq.shanyushiyangtech.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://jwu.wangdashe.top

[T08] Kotlin：数据类
来源：http://aqw.guowangkeji.top

data class User(val name: String, val age: Int)
来源：http://hxf.kuanghao11.cn

[T09] Kotlin：扩展函数
来源：http://mth.shanyushiyangkeji.top

fun String.exclaim() = this + "!"
来源：http://bjm.zhoulong.xyz

[T10] Kotlin：默认参数
来源：http://nfp.guannengcc.top

fun greet(name: String = "World") = "Hi $name"
来源：http://pmm.hysaishi.cn

[T11] Kotlin：协程
来源：http://zje.fzhhl.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://kvi.hnxiangtu.top

[T12] Kotlin：解构声明
来源：http://hqb.meibo888.top

val (a, b) = Pair(1, 2)
来源：http://grj.nanxinkj.top

[T13] Kotlin：只读 Map
来源：http://axp.tianlin.xyz

val m = mapOf("a" to 1)
来源：http://flm.yj20258888.top

[T14] Kotlin：循环
来源：http://xyc.jinyuanbaomall.cn

for (i in 1..10) println(i)
来源：http://yds.tianlin.xyz

[T15] Kotlin：接口
来源：http://zvu.gotoacloud.top

interface Shape { fun area(): Double }
来源：http://nyb.ybcxt.top

[T16] Swift：Hello World
来源：http://lba.mhx1999.top

print("Hello")
来源：http://cyz.aizwys.cn

[T17] Swift：变量与常量
来源：http://cxy.sysykeji.top

var a = 1;  let b = 2
来源：http://ing.vqdsnc.cn

[T18] Swift：字符串插值
来源：http://wzp.cashguo.top

"值: \(b)"
来源：http://dpc.sxryk.cn

[T19] Swift：可选绑定
来源：http://dhw.yongpay.top

if let n = opt { print(n) }
来源：http://any.smart0.xyz

[T20] Swift：数组操作
来源：http://jst.xuetiantiany.cn

var a = [1, 2, 3];  a.append(4)
来源：http://igc.bbcook.cn

[T21] Swift：遍历
来源：http://pil.zhixingplan.top

for x in a { print(x) }
来源：http://zcf.hongshengwenyu.top

[T22] Swift：字典
来源：http://yci.haohaochexian.top

var d = ["a": 1];  d["b"] = 2
来源：http://dcp.ywan-chungtsiang.top


<!-- 参考信息 -->