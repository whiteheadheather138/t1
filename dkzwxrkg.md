代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://hjd.zdbjq.cn

[R18] 遍历数组
来源：http://nrm.mhx1999.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sqz.uphjek.com

[R19] 数组长度
来源：http://bur.jlsjyb.cn

echo "${#arr[@]}"
来源：http://vjw.ywan-chungtsiang.top

[R20] 关联数组（字典）
来源：http://gqp.yanxiufei.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qcc.meibo888.top

[R21] 字符串长度
来源：http://xqm.sjlbkw.cn

echo "${#s}"
来源：http://cfz.c1oappe.top

[R22] 截取子串
来源：http://nmw.gzhubu.top

echo "${s:0:5}"
来源：http://rhc.ivvv.top

[R23] 字符串替换
来源：http://xen.zhiwuduotai.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wro.hnqzz.top

[R24] 大小写转换
来源：http://bdu.zhijiandao.cn

echo "${s^^}"; echo "${s,,}"
来源：http://auz.fzhhl.top

[R25] 去后缀 / 去前缀
来源：http://ffi.bbcook.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://edz.sjlbkw.cn

[R26] 命令替换
来源：http://umc.tianlin.xyz

now=$(date +%F); echo "$now"
来源：http://laq.zdbjq.cn

[R27] 算术展开
来源：http://jmu.vehdjk.com

echo $((1 + 2 * 3))
来源：http://mgz.yuanzhike.top

[R28] 浮点运算
来源：http://nxn.nwbrower.top

echo "scale=2; 10/3" | bc
来源：http://lkf.9152youxi.cn

[R29] 定义函数
来源：http://lcc.meibo888.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dic.svipenyu.cn

[R30] 函数返回状态码
来源：http://mgd.zhoulong.xyz

f() { return 0; }; f || echo "失败了"
来源：http://zrf.yueranfly.top

[R31] 局部变量
来源：http://jqk.gaohongyu789.top

f() { local x=1; echo "$x"; }
来源：http://ipk.xinyue.icu

[R32] 参数个数校验
来源：http://bhw.cashguo.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yef.guowangkeji.top

[R33] 捕获错误并提示行号
来源：http://oit.gzhubu.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ibr.quarkkingdee.top

[R34] 退出时清理
来源：http://wbx.wangshuangyany.cn

trap 'rm -f "$tmp"' EXIT
来源：http://aet.smart0.xyz

[R35] 后台执行并等待
来源：http://jrr.dashuyun.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://aiu.guannengcc.top

[R36] 并发执行多个任务
来源：http://jtq.chenlongwang.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ytt.sufxvd.cn

[R37] 把输出赋给变量
来源：http://ihh.yuxming.cn

files=$(ls -1)
来源：http://gfq.kuanghao11.cn

[R38] 管道串联
来源：http://hda.chenlongwang.top

cat a.txt | grep -i error | wc -l
来源：http://kwc.tianlin.xyz

[R39] 重定向标准输出与错误
来源：http://tez.wangshuangyany.cn

cmd > out.log 2>&1
来源：http://nlk.ybcxt.top

[R40] 追加写日志
来源：http://vwp.cqqwz.cn

echo "log" >> out.log
来源：http://gpy.jiagoushi.top

[R41] 丢弃输出
来源：http://gcc.nanxinkj.top

cmd >/dev/null 2>&1
来源：http://cvh.yueranfly.top

[R42] 输入重定向
来源：http://skc.sysykeji.top

wc -l < a.txt
来源：http://awr.zhaomingkeji.xyz

[R43] 按名字查找文件
来源：http://wgh.xinyue.icu

find . -name "*.log" -type f
来源：http://pgy.cdnleiting.top

[R44] 按修改时间查找
来源：http://tha.snrcjt.cn

find . -mtime -7 -type f
来源：http://fha.shanyushiyangkeji.top

[R45] 批量删除
来源：http://rqw.zhiwuduotai.top

find . -name "*.tmp" -delete
来源：http://yoc.zhongyouzk.top

[R46] 递归替换文件内容
来源：http://nof.hammf.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pyp.dashuyun.cn

[R47] sed 单行替换
来源：http://fur.jianghu66.top

sed -i 's/foo/bar/g' a.txt
来源：http://jbv.shanyushiyangtech.top

[R48] awk 取指定列
来源：http://wnk.yueranfly.top

awk '{print $1, $3}' a.txt
来源：http://hok.yvedp.cn

[R49] awk 带条件
来源：http://yct.cdnleiting.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xrc.shanyushiyangtech.top

[R50] awk 求和
来源：http://xtt.yj20258.top

awk '{s += $2} END {print s}' a.txt
来源：http://eze.pycfn.com

[R51] 排序去重取前几
来源：http://jho.shanyushiyangtech.top

sort a.txt | uniq -c | sort -rn | head
来源：http://wqo.svipenyu.cn

[R52] 统计行数
来源：http://zxk.chenlongwang.top

wc -l a.txt
来源：http://yay.shuidangran.top

[R53] 查看文件头与实时尾
来源：http://gce.shanyushiyangtech.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ozh.zycfv.cn

[R54] 比较两个文件
来源：http://dgt.jinghuilouyu.cn

diff a.txt b.txt
来源：http://vih.gotoacloud.top

[R55] 压缩与解压
来源：http://zha.zhoulong.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://plg.zdbjq.cn

[R56] 远程拷贝
来源：http://xok.iojbl.cn

scp file user@host:/path/
来源：http://ngv.tianlin.xyz

[R57] 远程执行命令
来源：http://gsc.shuidangran.top

ssh user@host 'uptime'
来源：http://beh.jiagoushi.top

[R58] 下载文件
来源：http://ruv.jiagoushi.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mbc.ydjk.org.cn

[R59] 发 POST JSON
来源：http://lgw.vehdjk.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zxw.mhx1999.top

[R60] 只看 HTTP 状态码
来源：http://mdl.sufxvd.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://awj.nwbrower.top

[R61] 磁盘占用
来源：http://uxh.gaohongyu789.top

df -h;  du -sh *
来源：http://mkr.xylfe.cn

[R62] 找最占空间的文件
来源：http://cwc.dashuyun.cn

du -ah . | sort -rh | head -10
来源：http://owk.yuanzhike.top

[R63] 内存与进程
来源：http://wfz.uphjek.com

free -h;  ps aux | grep nginx
来源：http://wda.jianghu66.top

[R64] 结束进程
来源：http://pyj.jqgfzy.top

kill -9 $(pgrep -f app.py)
来源：http://lzd.hfpthk.cn

[R65] 查看端口占用
来源：http://qbo.sxryk.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vqi.shangyingyoupin.top

[R66] 定时任务
来源：http://kon.havefunace.top

crontab -e;  crontab -l
来源：http://wno.ppjwa.cn

[R67] 生成随机十六进制串
来源：http://azs.havefunace.top

openssl rand -hex 16
来源：http://nof.daxiang520.top

[R68] 计算文件校验值
来源：http://uvi.sjlbkw.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xus.jinqigfzy.top

[R69] 生成随机密码
来源：http://ieb.nanxuanxn.top

head -c 16 /dev/urandom | base64
来源：http://ifm.tanke756.top

[R70] 时间戳与互转
来源：http://mxd.fehbvm.com

date +%s;  date -d @1700000000
来源：http://afh.cashguo.top

[R71] 日期格式化
来源：http://frt.yj20258888.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://xjq.ydjk.org.cn

[R72] 等待端口就绪
来源：http://xwb.xingfuxueyuan.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://rwt.uphjek.com

[R73] 分割大日志
来源：http://qbw.sufxvd.cn

split -l 1000 big.log part_
来源：http://mzf.xziqi.cn

[R74] 批量重命名
来源：http://xlz.c1oappe.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tti.xziqi.cn

[R75] 导出环境变量
来源：http://wek.cqqwz.cn

export PATH="$HOME/bin:$PATH"
来源：http://vwq.tianlin.xyz

[R76] 使用临时文件
来源：http://wqd.0kj1m.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://npq.jinyuanbaomall.cn

[R77] 读取用户输入
来源：http://ymh.ydjk.org.cn

read -rp "请输入: " ans
来源：http://usl.xingfuxueyuan.xyz

[R78] 交互式菜单
来源：http://xsi.svipenyu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://voi.0kj1m.cn

[R79] 解析命令行选项
来源：http://eso.chenlongwang.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ukt.wangdashe.top

[R80] 查看脚本执行耗时
来源：http://uci.fktsv.cn

time ./run.sh
来源：http://omu.shangyingyoupin.top

================================================================================
来源：http://gim.birdmap.top

S. C / C++ 专题
来源：http://lim.yj20258888.top

================================================================================
来源：http://rwt.haohaochexian.top

[S01] C：Hello World
来源：http://fek.jyoumei.cn

#include <stdio.h>
来源：http://gjx.cashguo.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ltm.9152youxi.cn

[S02] C：变量与格式化输出
来源：http://rfu.yuanzhike.top

int a = 10; printf("%d\n", a);
来源：http://zce.hysaishi.cn

[S03] C：读入整数
来源：http://sar.jinghuilouyu.cn

int x; scanf("%d", &x);
来源：http://uki.chenjidiqi.icu

[S04] C：字符串复制
来源：http://jmz.chenzaomai.com

char dst[32]; strcpy(dst, "hi");
来源：http://giy.svipenyu.cn

[S05] C：字符串长度
来源：http://xaa.chenlongwang.top

strlen(s)
来源：http://xdk.cqqwz.cn

[S06] C：字符串比较
来源：http://qzq.feifeiyinyue.top

strcmp(a, b) == 0
来源：http://ndb.chenjidiqi.icu

[S07] C：数组遍历求和
来源：http://duv.dashuyun.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xxw.nanxinkj.top

[S08] C：动态内存分配与释放
来源：http://ujo.shuidangran.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qqa.guowangkeji.top

[S09] C：结构体定义与初始化
来源：http://xcm.jlsjyb.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://omg.cheryme.top

[S10] C：指针与解引用
来源：http://rxb.shanyushiyangkeji.top

int *p = &a;  *p = 5;
来源：http://ywi.zhoulong.xyz

[S11] C：逐行读文件
来源：http://dcw.jyoumei.cn

FILE *f = fopen("a.txt", "r");
来源：http://bae.cqqwz.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gla.yj20258.top

fclose(f);
来源：http://heg.bjfxy.top

[S12] C：写文件
来源：http://wbs.jinyuanbaomall.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://prv.andypj.xyz

[S13] C：宏定义
来源：http://dqd.cqqwz.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hhb.yueranfly.top

[S14] C：枚举
来源：http://jbt.gogol.net.cn

enum Color { RED, GREEN, BLUE };
来源：http://wgg.birdmap.top

[S15] C：类型转换
来源：http://rou.vqdsnc.cn

(double) a / b
来源：http://bre.cheryme.top

[S16] C：位操作置位
来源：http://ptx.yonumen.top

x |= (1 << 3);
来源：http://syh.zhengqikj.top

[S17] C：安全拼接字符串
来源：http://lvj.guowangkeji.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yqr.hywenlv.cn

[S18] C：命令行参数
来源：http://quv.vehdjk.com

int main(int argc, char **argv)
来源：http://wmy.nwbrower.top

[S19] C：快速排序
来源：http://glm.guannengcc.top

qsort(a, n, sizeof(int), cmp);
来源：http://uek.fehbvm.com

[S20] C：二分查找
来源：http://iga.mhx1999.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rck.wangdashe.top

[S21] C：字符类别判断
来源：http://hhj.cdnleiting.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cih.fktsv.cn

[S22] C：字符串转数字
来源：http://zel.zdqjudy.top

atoi("42");  strtod("3.14", NULL);
来源：http://vtn.jlsjyb.cn

[S23] C：随机数
来源：http://sms.chenlongwang.top

srand(time(NULL));  int r = rand() % 100;
来源：http://kyr.vehdjk.com

[S24] C：获取本地时间
来源：http://hag.yfazqb.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ypi.sweek.top

[S25] C：内存拷贝
来源：http://yvx.shangyingyoupin.top

memcpy(dst, src, n);
来源：http://vyw.hesvh.cn

[S26] C：内存清零
来源：http://pwh.smart0.xyz

memset(a, 0, sizeof a);
来源：http://hjf.yvedp.cn

[S27] C：定义常量
来源：http://fjx.yj202588.top

const double PI = 3.14159;
来源：http://lae.zhiwuduotai.top

[S28] C：静态变量
来源：http://ayt.daxiang520.top

static int counter = 0;
来源：http://bhc.uphjek.com

[S29] C：变参函数
来源：http://qcw.gogol.net.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://piw.ydzc1.top

[S30] C：头文件保护
来源：http://wfi.cashguo.top

#ifndef X_H
来源：http://izw.smart0.xyz

#define X_H
来源：http://qun.feifeiyinyue.top

#endif
来源：http://yqu.chenlongwang.top

[S31] C++：Hello World
来源：http://nrg.tarul.cn

#include <iostream>
来源：http://ieg.chenlongwang.top

int main() { std::cout << "Hello\n"; }
来源：http://uwv.yuanzhike.top

[S32] C++：字符串
来源：http://wdz.xziqi.cn

std::string s = "hi";  s += "!";
来源：http://bzi.shanyushiyangkeji.top

[S33] C++：vector 增删
来源：http://ldp.bjfxy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://isf.ctjpmb.com

[S34] C++：遍历 vector
来源：http://fbm.hywenlv.cn

for (auto &x : v) { std::cout << x; }
来源：http://ezk.zhixingplan.top

[S35] C++：map
来源：http://yxi.gotoacloud.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qll.shuidangran.top

[S36] C++：unordered_map
来源：http://mso.haohaochexian.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uoy.hywenlv.cn

[S37] C++：set
来源：http://tak.nwbrower.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://npr.shangyingyoupin.top

[S38] C++：排序
来源：http://bfj.0kj1m.cn

std::sort(v.begin(), v.end());
来源：http://upz.yj202588.top

[S39] C++：自定义比较器排序
来源：http://lqi.kuanghao11.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bgw.ppjwa.cn

[S40] C++：查找元素
来源：http://iry.ydjk.org.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ott.jyoumei.cn

[S41] C++：类与构造函数
来源：http://chf.zhoulong.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wty.nanxuanxn.top

[S42] C++：继承与虚函数
来源：http://aze.feifeiyinyue.top

class B : public Base { public: void f() override {} };
来源：http://wni.jiagoushi.top

[S43] C++：智能指针
来源：http://sho.aizwys.cn

auto p = std::make_unique<int>(5);
来源：http://zga.havefunace.top

[S44] C++：引用传参
来源：http://pqi.hesvh.cn

void inc(int &x) { ++x; }
来源：http://tqz.xingfuxueyuan.xyz

[S45] C++：lambda
来源：http://egj.jinqigufen.top

auto add = [](int a, int b) { return a + b; };
来源：http://dsh.zdqjudy.top

[S46] C++：函数模板
来源：http://mid.ehwqpu.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pni.jinyuanbaomall.cn

[S47] C++：结构化绑定遍历
来源：http://ays.yj20258.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yxz.quarkkingdee.top

[S48] C++：逐行读文件
来源：http://wcm.ywan-chungtsiang.top

std::ifstream in("a.txt");  std::string line;
来源：http://hfe.ybcxt.top

while (std::getline(in, line)) { }
来源：http://jbj.ybcxt.top

[S49] C++：写文件
来源：http://pqk.pengpengdd.cyou

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nyh.yj20258.top

[S50] C++：格式化数字
来源：http://xwu.vehdjk.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://syi.ybcxt.top

[S51] C++：显式类型转换
来源：http://isk.yueranfly.top

static_cast<double>(a) / b
来源：http://lwy.pycfn.com

[S52] C++：const 与 noexcept
来源：http://jvg.chenzaomai.com

int size() const noexcept { return n_; }
来源：http://xjg.gzhubu.top

[S53] C++：移动语义
来源：http://ely.guannengcc.top

std::vector<int> w = std::move(v);
来源：http://nil.dianchejie.cn

[S54] C++：异常处理
来源：http://fxq.jinqigufen.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ccn.aizwys.cn

[S55] C++：结构化绑定
来源：http://kag.svipenyu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mnr.ybcxt.top

[S56] C++：optional
来源：http://uzt.jiagoushi.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qrs.havefunace.top

[S57] C++：编译期常量
来源：http://mry.zhijiandao.cn

constexpr int N = 10;
来源：http://gvs.svipenyu.cn

[S58] C++：命名空间
来源：http://tpc.0kj1m.cn

namespace ns { int f() { return 1; } }
来源：http://cvl.vqdsnc.cn

[S59] C++：静态断言
来源：http://rqf.sweek.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://iyl.gaohongyu789.top

[S60] C++：遍历并删除元素
来源：http://ekl.hywenlv.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xae.gogol.net.cn

================================================================================
来源：http://kyq.xuetiantiany.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://skq.dianchejie.cn

================================================================================
来源：http://feu.ppjwa.cn

[T01] Kotlin：Hello World
来源：http://chf.sweek.top

println("Hello")
来源：http://aqa.jyoumei.cn

[T02] Kotlin：变量
来源：http://pbe.zdbjq.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hgv.sweek.top

[T03] Kotlin：字符串模板
来源：http://yfh.ppjwa.cn

"值: $b"
来源：http://fmv.xuanzx.com

[T04] Kotlin：空安全
来源：http://vqo.xuanzx.com

val n: String? = null;  n?.length
来源：http://gbi.yanxiufei.cn

[T05] Kotlin：when 表达式
来源：http://yvo.jyoumei.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ggz.xuetiantiany.cn

[T06] Kotlin：集合映射
来源：http://uii.hesvh.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tpi.jinqigfzy.top

[T07] Kotlin：集合过滤
来源：http://wsv.yj202588.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://tnt.quarkkingdee.top

[T08] Kotlin：数据类
来源：http://yjo.hnqzz.top

data class User(val name: String, val age: Int)
来源：http://rmz.jyoumei.cn

[T09] Kotlin：扩展函数
来源：http://mxj.316326.xyz

fun String.exclaim() = this + "!"
来源：http://gwk.9152youxi.cn

[T10] Kotlin：默认参数
来源：http://xbc.daria6918.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ofo.shuidangran.top

[T11] Kotlin：协程
来源：http://dtl.birdmap.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://qdf.birdmap.top

[T12] Kotlin：解构声明
来源：http://yrj.ivvv.top

val (a, b) = Pair(1, 2)
来源：http://rfx.xuetiantiany.cn

[T13] Kotlin：只读 Map
来源：http://yer.birdmap.top

val m = mapOf("a" to 1)
来源：http://qxb.wangshuangyany.cn

[T14] Kotlin：循环
来源：http://djb.nanxuanxn.top

for (i in 1..10) println(i)
来源：http://qol.feifeiyinyue.top

[T15] Kotlin：接口
来源：http://gcw.daxiang520.top

interface Shape { fun area(): Double }
来源：http://sjs.shanyushiyangtech.top

[T16] Swift：Hello World
来源：http://olw.jinqigfzy.top

print("Hello")
来源：http://mjm.cdnleiting.top

[T17] Swift：变量与常量
来源：http://qvf.xziqi.cn

var a = 1;  let b = 2
来源：http://tqg.jinyuanbaomall.cn

[T18] Swift：字符串插值
来源：http://dod.zhoulong.xyz

"值: \(b)"
来源：http://hhd.ehwqpu.com

[T19] Swift：可选绑定
来源：http://sgf.jiagoushi.top

if let n = opt { print(n) }
来源：http://brh.xingfuxueyuan.xyz

[T20] Swift：数组操作
来源：http://fhu.cheryme.top

var a = [1, 2, 3];  a.append(4)
来源：http://cnf.sweek.top


<!-- 参考信息 -->