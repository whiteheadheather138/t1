代发 wailian999

echo "${#arr[@]}"
来源：http://mkw.tian-w.cn

[R20] 关联数组（字典）
来源：http://bsn.gotoacloud.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ycl.zhiwuduotai.top

[R21] 字符串长度
来源：http://whg.shzxlz.cn

echo "${#s}"
来源：http://ikt.fanxiaobao.xyz

[R22] 截取子串
来源：http://ybf.nwbrower.top

echo "${s:0:5}"
来源：http://kdw.aibaodan.cn

[R23] 字符串替换
来源：http://aqt.hywenlv.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fbb.cheryme.top

[R24] 大小写转换
来源：http://iux.feifeiyinyue.top

echo "${s^^}"; echo "${s,,}"
来源：http://itr.xinyue.icu

[R25] 去后缀 / 去前缀
来源：http://pfo.zdqjudy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://kkk.ydzc1.top

[R26] 命令替换
来源：http://rvi.bbcook.cn

now=$(date +%F); echo "$now"
来源：http://axb.vehdjk.com

[R27] 算术展开
来源：http://nly.hcnkem.com

echo $((1 + 2 * 3))
来源：http://qsp.hammf.cn

[R28] 浮点运算
来源：http://kxc.uphjek.com

echo "scale=2; 10/3" | bc
来源：http://igd.chenlongwang.top

[R29] 定义函数
来源：http://qks.xuanzx.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lws.c1oappe.top

[R30] 函数返回状态码
来源：http://dzw.pengpengdd.cyou

f() { return 0; }; f || echo "失败了"
来源：http://uei.cqqwz.cn

[R31] 局部变量
来源：http://fpq.meibo888.top

f() { local x=1; echo "$x"; }
来源：http://kir.gogol.net.cn

[R32] 参数个数校验
来源：http://ksc.jianghu66.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dva.zhijiandao.cn

[R33] 捕获错误并提示行号
来源：http://lmi.jqgfzy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ipu.guannengcc.top

[R34] 退出时清理
来源：http://pma.hnqzz.top

trap 'rm -f "$tmp"' EXIT
来源：http://cpq.sysykeji.top

[R35] 后台执行并等待
来源：http://vzt.yuxming.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://cwb.uphjek.com

[R36] 并发执行多个任务
来源：http://ize.gzhubu.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qyh.sweek.top

[R37] 把输出赋给变量
来源：http://daa.uphjek.com

files=$(ls -1)
来源：http://ynw.tarul.cn

[R38] 管道串联
来源：http://vcn.cqqwz.cn

cat a.txt | grep -i error | wc -l
来源：http://wvv.gogol.net.cn

[R39] 重定向标准输出与错误
来源：http://rdx.daria6918.cn

cmd > out.log 2>&1
来源：http://pqw.vehdjk.com

[R40] 追加写日志
来源：http://vif.yueranfly.top

echo "log" >> out.log
来源：http://xpw.ctjpmb.com

[R41] 丢弃输出
来源：http://wei.pycfn.com

cmd >/dev/null 2>&1
来源：http://lyc.meibo888.top

[R42] 输入重定向
来源：http://iat.fanxiaobao.xyz

wc -l < a.txt
来源：http://wfh.daria6918.cn

[R43] 按名字查找文件
来源：http://fpx.zhijiandao.cn

find . -name "*.log" -type f
来源：http://ean.pycfn.com

[R44] 按修改时间查找
来源：http://rca.feifeiyinyue.top

find . -mtime -7 -type f
来源：http://vfe.daxiang520.top

[R45] 批量删除
来源：http://dky.yj20258888.top

find . -name "*.tmp" -delete
来源：http://mkl.jinqigufen.top

[R46] 递归替换文件内容
来源：http://shu.jlsjyb.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zvn.316326.xyz

[R47] sed 单行替换
来源：http://umc.sxryk.cn

sed -i 's/foo/bar/g' a.txt
来源：http://yjw.ydjk.org.cn

[R48] awk 取指定列
来源：http://mip.cheryme.top

awk '{print $1, $3}' a.txt
来源：http://fhp.zdqjudy.top

[R49] awk 带条件
来源：http://gtq.daxiang520.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fyw.yj20258888.top

[R50] awk 求和
来源：http://tca.andypj.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://kha.cucudq.cn

[R51] 排序去重取前几
来源：http://zpi.jlsjyb.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qek.daria6918.cn

[R52] 统计行数
来源：http://byu.ydjk.org.cn

wc -l a.txt
来源：http://uyb.dianchejie.cn

[R53] 查看文件头与实时尾
来源：http://ork.hnxiangtu.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zxn.52xcode.cn

[R54] 比较两个文件
来源：http://qji.snrcjt.cn

diff a.txt b.txt
来源：http://miz.ydjk.org.cn

[R55] 压缩与解压
来源：http://clc.yvedp.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mpr.jqgufenzy.top

[R56] 远程拷贝
来源：http://fpm.xziqi.cn

scp file user@host:/path/
来源：http://xwm.vqdsnc.cn

[R57] 远程执行命令
来源：http://fkj.aibaodan.cn

ssh user@host 'uptime'
来源：http://ysc.xziqi.cn

[R58] 下载文件
来源：http://gfe.wangdashe.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kbe.andypj.xyz

[R59] 发 POST JSON
来源：http://qij.nwbrower.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zdm.wangdashe.top

[R60] 只看 HTTP 状态码
来源：http://rqv.andypj.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fsz.hfpthk.cn

[R61] 磁盘占用
来源：http://tkz.yj20258.top

df -h;  du -sh *
来源：http://xtr.sjlbkw.cn

[R62] 找最占空间的文件
来源：http://pxu.iojbl.cn

du -ah . | sort -rh | head -10
来源：http://evj.nanxinkj.top

[R63] 内存与进程
来源：http://ezp.hywenlv.cn

free -h;  ps aux | grep nginx
来源：http://hhz.yanxiufei.cn

[R64] 结束进程
来源：http://xif.gogol.net.cn

kill -9 $(pgrep -f app.py)
来源：http://uze.mhx1999.top

[R65] 查看端口占用
来源：http://yka.bbcook.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bse.zhoulong.xyz

[R66] 定时任务
来源：http://asc.yanxiufei.cn

crontab -e;  crontab -l
来源：http://kqq.ybcxt.top

[R67] 生成随机十六进制串
来源：http://nds.yangfankeji.com

openssl rand -hex 16
来源：http://tnn.wangdashe.top

[R68] 计算文件校验值
来源：http://nyh.9152youxi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://loq.epnwcf.com

[R69] 生成随机密码
来源：http://dom.yuanzhike.top

head -c 16 /dev/urandom | base64
来源：http://mru.ehwqpu.com

[R70] 时间戳与互转
来源：http://dau.52xcode.cn

date +%s;  date -d @1700000000
来源：http://rta.nanxuanxn.top

[R71] 日期格式化
来源：http://buh.tianlin.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://yjw.0kj1m.cn

[R72] 等待端口就绪
来源：http://bny.tanke756.top

until nc -z localhost 3306; do sleep 1; done
来源：http://uer.nanxuanxn.top

[R73] 分割大日志
来源：http://uii.zhongyouzk.top

split -l 1000 big.log part_
来源：http://bev.hfpthk.cn

[R74] 批量重命名
来源：http://qqs.fehbvm.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ncm.zhoulong.xyz

[R75] 导出环境变量
来源：http://maj.zdqjudy.top

export PATH="$HOME/bin:$PATH"
来源：http://szc.hammf.cn

[R76] 使用临时文件
来源：http://mxl.sysykeji.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yfp.zhaomingkeji.xyz

[R77] 读取用户输入
来源：http://eic.redwolf501.top

read -rp "请输入: " ans
来源：http://vkq.gaohongyu789.top

[R78] 交互式菜单
来源：http://mwn.yonumen.top

select opt in a b c; do echo "$opt"; break; done
来源：http://yfp.hfpthk.cn

[R79] 解析命令行选项
来源：http://djs.tianlin.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://did.mhx1999.top

[R80] 查看脚本执行耗时
来源：http://teu.cdnleiting.top

time ./run.sh
来源：http://lke.c1oappe.top

================================================================================
来源：http://gly.cheryme.top

S. C / C++ 专题
来源：http://voo.andypj.xyz

================================================================================
来源：http://hua.yuxming.cn

[S01] C：Hello World
来源：http://exu.jlsjyb.cn

#include <stdio.h>
来源：http://ris.zhiwuduotai.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://bzl.yj20258.top

[S02] C：变量与格式化输出
来源：http://rot.chenlongwang.top

int a = 10; printf("%d\n", a);
来源：http://qjl.kuanghao11.cn

[S03] C：读入整数
来源：http://fhr.gaohongyu789.top

int x; scanf("%d", &x);
来源：http://jdx.jinyuanbaomall.cn

[S04] C：字符串复制
来源：http://xbz.hongshengwenyu.top

char dst[32]; strcpy(dst, "hi");
来源：http://ivu.ywan-chungtsiang.top

[S05] C：字符串长度
来源：http://xxy.feifeiyinyue.top

strlen(s)
来源：http://txl.xinyue.icu

[S06] C：字符串比较
来源：http://mdi.nanxuanxn.top

strcmp(a, b) == 0
来源：http://dvg.xuetiantiany.cn

[S07] C：数组遍历求和
来源：http://wqd.cucudq.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rno.jyoumei.cn

[S08] C：动态内存分配与释放
来源：http://tcn.fengsongda.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gng.xylfe.cn

[S09] C：结构体定义与初始化
来源：http://rih.shangyingyoupin.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ypk.guowangkeji.top

[S10] C：指针与解引用
来源：http://kos.xziqi.cn

int *p = &a;  *p = 5;
来源：http://fup.guowangkeji.top

[S11] C：逐行读文件
来源：http://rgu.sufxvd.cn

FILE *f = fopen("a.txt", "r");
来源：http://igv.andypj.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://twk.xuanzx.com

fclose(f);
来源：http://uld.havefunace.top

[S12] C：写文件
来源：http://cvz.guowangkeji.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rmj.9152youxi.cn

[S13] C：宏定义
来源：http://smw.ehwqpu.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tai.gotoacloud.top

[S14] C：枚举
来源：http://gom.jyoumei.cn

enum Color { RED, GREEN, BLUE };
来源：http://owu.ybcxt.top

[S15] C：类型转换
来源：http://vue.quarkkingdee.top

(double) a / b
来源：http://lew.jlsjyb.cn

[S16] C：位操作置位
来源：http://rhk.shanyushiyangtech.top

x |= (1 << 3);
来源：http://hmp.xziqi.cn

[S17] C：安全拼接字符串
来源：http://oqm.cqqwz.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fjo.jiagoushi.top

[S18] C：命令行参数
来源：http://npi.ivvv.top

int main(int argc, char **argv)
来源：http://ukb.xuetiantiany.cn

[S19] C：快速排序
来源：http://ncd.cashguo.top

qsort(a, n, sizeof(int), cmp);
来源：http://svu.zhoulong.xyz

[S20] C：二分查找
来源：http://yed.tian-w.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ryn.hywenlv.cn

[S21] C：字符类别判断
来源：http://phd.yuanzhike.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://eha.hammf.cn

[S22] C：字符串转数字
来源：http://sel.sxryk.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ckz.zhoulong.xyz

[S23] C：随机数
来源：http://itf.9152youxi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rhy.xylfe.cn

[S24] C：获取本地时间
来源：http://uhe.dianchejie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pfw.pengpengdd.cyou

[S25] C：内存拷贝
来源：http://ckj.yangfankeji.com

memcpy(dst, src, n);
来源：http://ysa.pycfn.com

[S26] C：内存清零
来源：http://adz.hywenlv.cn

memset(a, 0, sizeof a);
来源：http://axi.nanxuanxn.top

[S27] C：定义常量
来源：http://iuw.yonumen.top

const double PI = 3.14159;
来源：http://frn.bbcook.cn

[S28] C：静态变量
来源：http://dna.zhijiandao.cn

static int counter = 0;
来源：http://csw.fehbvm.com

[S29] C：变参函数
来源：http://egf.cashguo.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mpy.redwolf501.top

[S30] C：头文件保护
来源：http://hrs.zdbjq.cn

#ifndef X_H
来源：http://azf.316326.xyz

#define X_H
来源：http://ego.tarul.cn

#endif
来源：http://tjk.316326.xyz

[S31] C++：Hello World
来源：http://ncv.yonumen.top

#include <iostream>
来源：http://tke.guowangkeji.top

int main() { std::cout << "Hello\n"; }
来源：http://ada.xuanzx.com

[S32] C++：字符串
来源：http://fll.andypj.xyz

std::string s = "hi";  s += "!";
来源：http://das.snrcjt.cn

[S33] C++：vector 增删
来源：http://mjl.9152youxi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zur.zhoulong.xyz

[S34] C++：遍历 vector
来源：http://kqc.feifeiyinyue.top

for (auto &x : v) { std::cout << x; }
来源：http://cut.jinyuanbaomall.cn

[S35] C++：map
来源：http://vhi.chenlongwang.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://puh.bjfxy.top

[S36] C++：unordered_map
来源：http://iua.zhijiandao.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://aur.xziqi.cn

[S37] C++：set
来源：http://psq.xylfe.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pci.shzxlz.cn

[S38] C++：排序
来源：http://dze.yonumen.top

std::sort(v.begin(), v.end());
来源：http://nzy.bjfxy.top

[S39] C++：自定义比较器排序
来源：http://ply.wangdashe.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://syh.epnwcf.com

[S40] C++：查找元素
来源：http://ten.jinqigfzy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sol.epnwcf.com

[S41] C++：类与构造函数
来源：http://qyr.chenjidiqi.icu

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sgi.kuanghao11.cn

[S42] C++：继承与虚函数
来源：http://uwz.vqdsnc.cn

class B : public Base { public: void f() override {} };
来源：http://rah.fanxiaobao.xyz

[S43] C++：智能指针
来源：http://tej.tian-w.cn

auto p = std::make_unique<int>(5);
来源：http://psh.haohaochexian.top

[S44] C++：引用传参
来源：http://oac.yueranfly.top

void inc(int &x) { ++x; }
来源：http://gop.fktsv.cn

[S45] C++：lambda
来源：http://knu.tanke756.top

auto add = [](int a, int b) { return a + b; };
来源：http://thu.mhx1999.top

[S46] C++：函数模板
来源：http://vog.birdmap.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://abp.chenzaomai.com

[S47] C++：结构化绑定遍历
来源：http://mfk.hcnkem.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gcd.yj20258888.top

[S48] C++：逐行读文件
来源：http://pbv.vehdjk.com

std::ifstream in("a.txt");  std::string line;
来源：http://qrf.yongpay.top

while (std::getline(in, line)) { }
来源：http://mkw.gaohongyu789.top

[S49] C++：写文件
来源：http://lmd.jlsjyb.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vib.vehdjk.com

[S50] C++：格式化数字
来源：http://ows.gotoacloud.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xav.zhixingplan.top

[S51] C++：显式类型转换
来源：http://eky.ydzc1.top

static_cast<double>(a) / b
来源：http://mnn.shanyushiyangkeji.top

[S52] C++：const 与 noexcept
来源：http://ngl.yanxiufei.cn

int size() const noexcept { return n_; }
来源：http://isy.chenlongwang.top

[S53] C++：移动语义
来源：http://fpp.snrcjt.cn

std::vector<int> w = std::move(v);
来源：http://yem.guowangkeji.top

[S54] C++：异常处理
来源：http://hxu.iojbl.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ccz.epnwcf.com

[S55] C++：结构化绑定
来源：http://yyn.zhixingplan.top

auto [a, b] = std::make_pair(1, 2);
来源：http://jyf.xuanzx.com

[S56] C++：optional
来源：http://syx.bbcook.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jgc.dashuyun.cn

[S57] C++：编译期常量
来源：http://olx.gzhubu.top

constexpr int N = 10;
来源：http://lxw.vqdsnc.cn

[S58] C++：命名空间
来源：http://ybx.yvedp.cn

namespace ns { int f() { return 1; } }
来源：http://ayu.tarul.cn

[S59] C++：静态断言
来源：http://ttx.havefunace.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dha.shangyingyoupin.top

[S60] C++：遍历并删除元素
来源：http://ewd.zdbjq.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vkb.shuidangran.top

================================================================================
来源：http://kqo.9152youxi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fsn.zdqjudy.top

================================================================================
来源：http://bmz.quarkkingdee.top

[T01] Kotlin：Hello World
来源：http://mrr.yanxiufei.cn

println("Hello")
来源：http://hzv.hnxiangtu.top

[T02] Kotlin：变量
来源：http://mdr.cqqwz.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ltk.ivvv.top

[T03] Kotlin：字符串模板
来源：http://utx.fehbvm.com

"值: $b"
来源：http://isw.jyoumei.cn

[T04] Kotlin：空安全
来源：http://xrd.ivvv.top

val n: String? = null;  n?.length
来源：http://yxo.tarul.cn

[T05] Kotlin：when 表达式
来源：http://mva.daxiang520.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://omt.zhoulong.xyz

[T06] Kotlin：集合映射
来源：http://zzp.jinqigufen.top

listOf(1, 2, 3).map { it * 2 }
来源：http://kmj.wangshuangyany.cn

[T07] Kotlin：集合过滤
来源：http://qcl.xziqi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://jbm.shuidangran.top

[T08] Kotlin：数据类
来源：http://xup.jlsjyb.cn

data class User(val name: String, val age: Int)
来源：http://tej.cashguo.top

[T09] Kotlin：扩展函数
来源：http://tmj.yueranfly.top

fun String.exclaim() = this + "!"
来源：http://pow.tarul.cn

[T10] Kotlin：默认参数
来源：http://fas.xinyue.icu

fun greet(name: String = "World") = "Hi $name"
来源：http://zti.xylfe.cn

[T11] Kotlin：协程
来源：http://bey.jyoumei.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bdc.jqgufenzy.top

[T12] Kotlin：解构声明
来源：http://abt.daxiang520.top

val (a, b) = Pair(1, 2)
来源：http://qiz.ydzc1.top

[T13] Kotlin：只读 Map
来源：http://ogg.yj20258888.top

val m = mapOf("a" to 1)
来源：http://zsf.kuanghao11.cn

[T14] Kotlin：循环
来源：http://gqp.hfpthk.cn

for (i in 1..10) println(i)
来源：http://nua.dashuyun.cn

[T15] Kotlin：接口
来源：http://chf.gaohongyu789.top

interface Shape { fun area(): Double }
来源：http://tni.yonumen.top

[T16] Swift：Hello World
来源：http://zjq.uphjek.com

print("Hello")
来源：http://pvb.andypj.xyz

[T17] Swift：变量与常量
来源：http://rfl.52xcode.cn

var a = 1;  let b = 2
来源：http://acl.jlsjyb.cn

[T18] Swift：字符串插值
来源：http://uvc.yueranfly.top

"值: \(b)"
来源：http://osg.zdbjq.cn

[T19] Swift：可选绑定
来源：http://tqd.bjfxy.top

if let n = opt { print(n) }
来源：http://lvo.yj202588.top

[T20] Swift：数组操作
来源：http://jot.svipenyu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://yss.hywenlv.cn

[T21] Swift：遍历
来源：http://rno.tianlin.xyz

for x in a { print(x) }
来源：http://ejo.jqgufenzy.top

[T22] Swift：字典
来源：http://hdm.yongpay.top

var d = ["a": 1];  d["b"] = 2
来源：http://cib.hfpthk.cn


<!-- 参考信息 -->