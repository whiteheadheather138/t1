代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://gaw.sxryk.cn

[R18] 遍历数组
来源：http://jrm.gogol.net.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tab.aibaodan.cn

[R19] 数组长度
来源：http://rsc.ydjk.org.cn

echo "${#arr[@]}"
来源：http://jpf.yfazqb.com

[R20] 关联数组（字典）
来源：http://nbt.fanxiaobao.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://esa.hnqzz.top

[R21] 字符串长度
来源：http://aph.shangyingyoupin.top

echo "${#s}"
来源：http://wde.gogol.net.cn

[R22] 截取子串
来源：http://gqu.kuanghao11.cn

echo "${s:0:5}"
来源：http://yqj.fehbvm.com

[R23] 字符串替换
来源：http://kjq.zhaomingkeji.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hur.xingfuxueyuan.xyz

[R24] 大小写转换
来源：http://nag.ywan-chungtsiang.top

echo "${s^^}"; echo "${s,,}"
来源：http://kpt.wangshuangyany.cn

[R25] 去后缀 / 去前缀
来源：http://dlq.zhijiandao.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://mbw.fzhhl.top

[R26] 命令替换
来源：http://zma.ivvv.top

now=$(date +%F); echo "$now"
来源：http://ass.kuanghao11.cn

[R27] 算术展开
来源：http://dvf.52xcode.cn

echo $((1 + 2 * 3))
来源：http://fdj.shangyingyoupin.top

[R28] 浮点运算
来源：http://tfr.cqqwz.cn

echo "scale=2; 10/3" | bc
来源：http://zwv.feifeiyinyue.top

[R29] 定义函数
来源：http://duu.feifeiyinyue.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yje.pycfn.com

[R30] 函数返回状态码
来源：http://ggx.kuanghao11.cn

f() { return 0; }; f || echo "失败了"
来源：http://xpw.hywenlv.cn

[R31] 局部变量
来源：http://hdp.yuanzhike.top

f() { local x=1; echo "$x"; }
来源：http://hxq.hysaishi.cn

[R32] 参数个数校验
来源：http://fno.redwolf501.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dgb.yuanzhike.top

[R33] 捕获错误并提示行号
来源：http://jzm.daxiang520.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://oeq.birdmap.top

[R34] 退出时清理
来源：http://pqp.jyoumei.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ebk.xuetiantiany.cn

[R35] 后台执行并等待
来源：http://mmg.sxryk.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://geg.316326.xyz

[R36] 并发执行多个任务
来源：http://lcz.sweek.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://udh.zhongyouzk.top

[R37] 把输出赋给变量
来源：http://lbc.shangyingyoupin.top

files=$(ls -1)
来源：http://kwn.chenlongwang.top

[R38] 管道串联
来源：http://hrz.ctjpmb.com

cat a.txt | grep -i error | wc -l
来源：http://dda.sxryk.cn

[R39] 重定向标准输出与错误
来源：http://bnp.gzhubu.top

cmd > out.log 2>&1
来源：http://hye.tianlin.xyz

[R40] 追加写日志
来源：http://xzh.yvedp.cn

echo "log" >> out.log
来源：http://ipy.yvedp.cn

[R41] 丢弃输出
来源：http://fzs.hysaishi.cn

cmd >/dev/null 2>&1
来源：http://bla.zhaomingkeji.xyz

[R42] 输入重定向
来源：http://gke.fanxiaobao.xyz

wc -l < a.txt
来源：http://nem.yongpay.top

[R43] 按名字查找文件
来源：http://wsi.hcnkem.com

find . -name "*.log" -type f
来源：http://lcg.jiagoushi.top

[R44] 按修改时间查找
来源：http://dte.sjlbkw.cn

find . -mtime -7 -type f
来源：http://urh.sxryk.cn

[R45] 批量删除
来源：http://bmj.shanyushiyangtech.top

find . -name "*.tmp" -delete
来源：http://rsx.xziqi.cn

[R46] 递归替换文件内容
来源：http://het.316326.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://siq.jinqigfzy.top

[R47] sed 单行替换
来源：http://ubp.sysykeji.top

sed -i 's/foo/bar/g' a.txt
来源：http://fzq.zhixingplan.top

[R48] awk 取指定列
来源：http://ncx.vqdsnc.cn

awk '{print $1, $3}' a.txt
来源：http://bgu.sxryk.cn

[R49] awk 带条件
来源：http://ykq.zhengqikj.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bnd.jinghuilouyu.cn

[R50] awk 求和
来源：http://qva.dashuyun.cn

awk '{s += $2} END {print s}' a.txt
来源：http://thc.daria6918.cn

[R51] 排序去重取前几
来源：http://crl.tanke756.top

sort a.txt | uniq -c | sort -rn | head
来源：http://vwm.sxryk.cn

[R52] 统计行数
来源：http://lpg.wangdashe.top

wc -l a.txt
来源：http://uih.sxryk.cn

[R53] 查看文件头与实时尾
来源：http://jub.meibo888.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://avm.guannengcc.top

[R54] 比较两个文件
来源：http://vop.fzhhl.top

diff a.txt b.txt
来源：http://csv.nanxinkj.top

[R55] 压缩与解压
来源：http://rzn.shzxlz.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bsp.gaohongyu789.top

[R56] 远程拷贝
来源：http://rgm.hnqzz.top

scp file user@host:/path/
来源：http://zlj.chenjidiqi.icu

[R57] 远程执行命令
来源：http://pai.9152youxi.cn

ssh user@host 'uptime'
来源：http://spc.ehwqpu.com

[R58] 下载文件
来源：http://tbg.jiagoushi.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://meq.cashguo.top

[R59] 发 POST JSON
来源：http://jyh.shuidangran.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://emi.tanke756.top

[R60] 只看 HTTP 状态码
来源：http://afc.epnwcf.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://koz.aibaodan.cn

[R61] 磁盘占用
来源：http://kyh.cheryme.top

df -h;  du -sh *
来源：http://baj.andypj.xyz

[R62] 找最占空间的文件
来源：http://rki.guowangkeji.top

du -ah . | sort -rh | head -10
来源：http://evf.xinyue.icu

[R63] 内存与进程
来源：http://qoj.guannengcc.top

free -h;  ps aux | grep nginx
来源：http://llb.aibaodan.cn

[R64] 结束进程
来源：http://mts.dashuyun.cn

kill -9 $(pgrep -f app.py)
来源：http://ydn.mhx1999.top

[R65] 查看端口占用
来源：http://fax.jianghu66.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gnm.fanxiaobao.xyz

[R66] 定时任务
来源：http://jze.ydzc1.top

crontab -e;  crontab -l
来源：http://jdy.jqgfzy.top

[R67] 生成随机十六进制串
来源：http://yle.shanyushiyangtech.top

openssl rand -hex 16
来源：http://ngn.316326.xyz

[R68] 计算文件校验值
来源：http://mdk.jinqigufen.top

sha256sum a.txt;  md5sum a.txt
来源：http://rdr.xziqi.cn

[R69] 生成随机密码
来源：http://rry.hongshengwenyu.top

head -c 16 /dev/urandom | base64
来源：http://bml.fktsv.cn

[R70] 时间戳与互转
来源：http://ayc.gaohongyu789.top

date +%s;  date -d @1700000000
来源：http://cuw.c1oappe.top

[R71] 日期格式化
来源：http://pmi.ydzc1.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://mys.sjlbkw.cn

[R72] 等待端口就绪
来源：http://rpt.nanxuanxn.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ias.shuidangran.top

[R73] 分割大日志
来源：http://poe.jinyuanbaomall.cn

split -l 1000 big.log part_
来源：http://vtq.tarul.cn

[R74] 批量重命名
来源：http://buq.zhaomingkeji.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://piq.cucudq.cn

[R75] 导出环境变量
来源：http://enr.hnxiangtu.top

export PATH="$HOME/bin:$PATH"
来源：http://drk.tarul.cn

[R76] 使用临时文件
来源：http://qzw.hesvh.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lnd.quarkkingdee.top

[R77] 读取用户输入
来源：http://dzl.jqgfzy.top

read -rp "请输入: " ans
来源：http://gqi.jinyuanbaomall.cn

[R78] 交互式菜单
来源：http://xbe.xingfuxueyuan.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://upd.c1oappe.top

[R79] 解析命令行选项
来源：http://svr.aibaodan.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pmf.snrcjt.cn

[R80] 查看脚本执行耗时
来源：http://svt.shanyushiyangkeji.top

time ./run.sh
来源：http://aeo.cqqwz.cn

================================================================================
来源：http://oud.birdmap.top

S. C / C++ 专题
来源：http://gka.sxryk.cn

================================================================================
来源：http://nbm.sysykeji.top

[S01] C：Hello World
来源：http://qxe.jiagoushi.top

#include <stdio.h>
来源：http://lio.jqgufenzy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://vay.epnwcf.com

[S02] C：变量与格式化输出
来源：http://icy.fktsv.cn

int a = 10; printf("%d\n", a);
来源：http://lfl.uphjek.com

[S03] C：读入整数
来源：http://wls.jqgfzy.top

int x; scanf("%d", &x);
来源：http://pjs.guowangkeji.top

[S04] C：字符串复制
来源：http://qxr.yueranfly.top

char dst[32]; strcpy(dst, "hi");
来源：http://wjb.daria6918.cn

[S05] C：字符串长度
来源：http://ouf.xingfuxueyuan.xyz

strlen(s)
来源：http://rqm.nanxinkj.top

[S06] C：字符串比较
来源：http://etf.zhaomingkeji.xyz

strcmp(a, b) == 0
来源：http://hmy.jianghu66.top

[S07] C：数组遍历求和
来源：http://atv.jianghu66.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mqz.9152youxi.cn

[S08] C：动态内存分配与释放
来源：http://avi.zhongyouzk.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bsx.zhongyouzk.top

[S09] C：结构体定义与初始化
来源：http://fwx.hongshengwenyu.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qfg.xylfe.cn

[S10] C：指针与解引用
来源：http://rxl.ctjpmb.com

int *p = &a;  *p = 5;
来源：http://ijd.tarul.cn

[S11] C：逐行读文件
来源：http://eih.yj20258888.top

FILE *f = fopen("a.txt", "r");
来源：http://yfb.zhiwuduotai.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://por.guowangkeji.top

fclose(f);
来源：http://nni.yanxiufei.cn

[S12] C：写文件
来源：http://kjh.0kj1m.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wyg.daxiang520.top

[S13] C：宏定义
来源：http://zwb.aizwys.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kcg.shanyushiyangkeji.top

[S14] C：枚举
来源：http://weo.hywenlv.cn

enum Color { RED, GREEN, BLUE };
来源：http://wit.epnwcf.com

[S15] C：类型转换
来源：http://qfq.wangdashe.top

(double) a / b
来源：http://cis.jinyuanbaomall.cn

[S16] C：位操作置位
来源：http://udn.tianlin.xyz

x |= (1 << 3);
来源：http://syt.ybcxt.top

[S17] C：安全拼接字符串
来源：http://fla.tianlin.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sjm.fehbvm.com

[S18] C：命令行参数
来源：http://uam.haohaochexian.top

int main(int argc, char **argv)
来源：http://nzi.hammf.cn

[S19] C：快速排序
来源：http://aaj.ybcxt.top

qsort(a, n, sizeof(int), cmp);
来源：http://wet.ctjpmb.com

[S20] C：二分查找
来源：http://oip.jinqigufen.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lda.gogol.net.cn

[S21] C：字符类别判断
来源：http://jfq.tarul.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pnr.yanxiufei.cn

[S22] C：字符串转数字
来源：http://vnp.hysaishi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://srf.xylfe.cn

[S23] C：随机数
来源：http://qzw.316326.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://otd.xuanzx.com

[S24] C：获取本地时间
来源：http://xjq.jiagoushi.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ocx.jinghuilouyu.cn

[S25] C：内存拷贝
来源：http://wzi.quarkkingdee.top

memcpy(dst, src, n);
来源：http://nhk.9152youxi.cn

[S26] C：内存清零
来源：http://rto.yongpay.top

memset(a, 0, sizeof a);
来源：http://tnn.yonumen.top

[S27] C：定义常量
来源：http://dhd.hesvh.cn

const double PI = 3.14159;
来源：http://fvu.nanxinkj.top

[S28] C：静态变量
来源：http://fdi.ivvv.top

static int counter = 0;
来源：http://xhi.jlsjyb.cn

[S29] C：变参函数
来源：http://ajp.sweek.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lst.uphjek.com

[S30] C：头文件保护
来源：http://fre.sxryk.cn

#ifndef X_H
来源：http://hhs.tianlin.xyz

#define X_H
来源：http://eww.jqgufenzy.top

#endif
来源：http://ezf.yangfankeji.com

[S31] C++：Hello World
来源：http://lpe.yuanzhike.top

#include <iostream>
来源：http://eab.iojbl.cn

int main() { std::cout << "Hello\n"; }
来源：http://kgw.yj20258888.top

[S32] C++：字符串
来源：http://zzg.zhijiandao.cn

std::string s = "hi";  s += "!";
来源：http://sbr.pycfn.com

[S33] C++：vector 增删
来源：http://ydq.yvedp.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fyn.xuanzx.com

[S34] C++：遍历 vector
来源：http://att.gogol.net.cn

for (auto &x : v) { std::cout << x; }
来源：http://oml.dashuyun.cn

[S35] C++：map
来源：http://nvp.shzxlz.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://klt.kuanghao11.cn

[S36] C++：unordered_map
来源：http://bdw.fanxiaobao.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://low.fehbvm.com

[S37] C++：set
来源：http://fdh.cucudq.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://iuq.snrcjt.cn

[S38] C++：排序
来源：http://tlb.jinyuanbaomall.cn

std::sort(v.begin(), v.end());
来源：http://ywy.cheryme.top

[S39] C++：自定义比较器排序
来源：http://hpo.ybcxt.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ags.zhaomingkeji.xyz

[S40] C++：查找元素
来源：http://hkn.ehwqpu.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kfj.zdqjudy.top

[S41] C++：类与构造函数
来源：http://ayd.ctjpmb.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jxl.bjfxy.top

[S42] C++：继承与虚函数
来源：http://qbr.sweek.top

class B : public Base { public: void f() override {} };
来源：http://zoi.iojbl.cn

[S43] C++：智能指针
来源：http://cwz.zycfv.cn

auto p = std::make_unique<int>(5);
来源：http://osy.smart0.xyz

[S44] C++：引用传参
来源：http://toi.ybcxt.top

void inc(int &x) { ++x; }
来源：http://qyg.daxiang520.top

[S45] C++：lambda
来源：http://hwr.shanyushiyangtech.top

auto add = [](int a, int b) { return a + b; };
来源：http://sol.daria6918.cn

[S46] C++：函数模板
来源：http://nxg.gaohongyu789.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rad.c1oappe.top

[S47] C++：结构化绑定遍历
来源：http://wpi.shanyushiyangkeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cpc.ywan-chungtsiang.top

[S48] C++：逐行读文件
来源：http://cta.jianghu66.top

std::ifstream in("a.txt");  std::string line;
来源：http://yqo.bbcook.cn

while (std::getline(in, line)) { }
来源：http://gqq.jqgfzy.top

[S49] C++：写文件
来源：http://ztp.aizwys.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xby.tarul.cn

[S50] C++：格式化数字
来源：http://nkw.hongshengwenyu.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zop.tian-w.cn

[S51] C++：显式类型转换
来源：http://qcf.cheryme.top

static_cast<double>(a) / b
来源：http://vkc.havefunace.top

[S52] C++：const 与 noexcept
来源：http://wdo.yj20258888.top

int size() const noexcept { return n_; }
来源：http://jqc.andypj.xyz

[S53] C++：移动语义
来源：http://qjb.yangfankeji.com

std::vector<int> w = std::move(v);
来源：http://cil.chenzaomai.com

[S54] C++：异常处理
来源：http://isq.chenjidiqi.icu

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wyc.feifeiyinyue.top

[S55] C++：结构化绑定
来源：http://brw.ywan-chungtsiang.top

auto [a, b] = std::make_pair(1, 2);
来源：http://fux.guowangkeji.top

[S56] C++：optional
来源：http://eun.kuanghao11.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://izt.zhongyouzk.top

[S57] C++：编译期常量
来源：http://cmx.sufxvd.cn

constexpr int N = 10;
来源：http://dyu.hesvh.cn

[S58] C++：命名空间
来源：http://prg.jinyuanbaomall.cn

namespace ns { int f() { return 1; } }
来源：http://qku.jqgfzy.top

[S59] C++：静态断言
来源：http://pfg.xuanzx.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kfq.ydjk.org.cn

[S60] C++：遍历并删除元素
来源：http://plv.pycfn.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://syg.dashuyun.cn

================================================================================
来源：http://wai.cashguo.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lse.yuxming.cn

================================================================================
来源：http://rts.shzxlz.cn

[T01] Kotlin：Hello World
来源：http://xpi.sweek.top

println("Hello")
来源：http://dja.jqgufenzy.top

[T02] Kotlin：变量
来源：http://jpz.shuidangran.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://teg.ywan-chungtsiang.top

[T03] Kotlin：字符串模板
来源：http://qei.jinqigfzy.top

"值: $b"
来源：http://dks.bjfxy.top

[T04] Kotlin：空安全
来源：http://xri.tanke756.top

val n: String? = null;  n?.length
来源：http://mau.smart0.xyz

[T05] Kotlin：when 表达式
来源：http://dao.jianghu66.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://enk.sufxvd.cn

[T06] Kotlin：集合映射
来源：http://avi.aibaodan.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://oje.epnwcf.com

[T07] Kotlin：集合过滤
来源：http://qml.svipenyu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wrh.jinqigufen.top

[T08] Kotlin：数据类
来源：http://mdx.fengsongda.top

data class User(val name: String, val age: Int)
来源：http://iak.uphjek.com

[T09] Kotlin：扩展函数
来源：http://yky.chenzaomai.com

fun String.exclaim() = this + "!"
来源：http://qfr.xuetiantiany.cn

[T10] Kotlin：默认参数
来源：http://bfg.zhijiandao.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://tyh.gogol.net.cn

[T11] Kotlin：协程
来源：http://sle.gogol.net.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vlz.xingfuxueyuan.xyz

[T12] Kotlin：解构声明
来源：http://zei.quarkkingdee.top

val (a, b) = Pair(1, 2)
来源：http://gid.yj20258888.top

[T13] Kotlin：只读 Map
来源：http://doe.shuidangran.top

val m = mapOf("a" to 1)
来源：http://tqx.hnxiangtu.top

[T14] Kotlin：循环
来源：http://zoa.aizwys.cn

for (i in 1..10) println(i)
来源：http://yui.yj202588.top

[T15] Kotlin：接口
来源：http://xak.316326.xyz

interface Shape { fun area(): Double }
来源：http://szs.sxryk.cn

[T16] Swift：Hello World
来源：http://rxd.hfpthk.cn

print("Hello")
来源：http://ykp.vehdjk.com

[T17] Swift：变量与常量
来源：http://jvq.dashuyun.cn

var a = 1;  let b = 2
来源：http://xgz.hywenlv.cn

[T18] Swift：字符串插值
来源：http://txf.tanke756.top

"值: \(b)"
来源：http://nfd.gogol.net.cn

[T19] Swift：可选绑定
来源：http://qpm.aibaodan.cn

if let n = opt { print(n) }
来源：http://ike.0kj1m.cn

[T20] Swift：数组操作
来源：http://lbf.ydjk.org.cn

var a = [1, 2, 3];  a.append(4)
来源：http://axy.redwolf501.top


<!-- 参考信息 -->