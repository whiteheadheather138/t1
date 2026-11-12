代发 wailian999

echo "${#arr[@]}"
来源：http://wrv.vqdsnc.cn

[R20] 关联数组（字典）
来源：http://vtg.yuxming.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ymp.shangyingyoupin.top

[R21] 字符串长度
来源：http://tre.snrcjt.cn

echo "${#s}"
来源：http://nbg.pengpengdd.cyou

[R22] 截取子串
来源：http://bgq.jianghu66.top

echo "${s:0:5}"
来源：http://zmm.jiagoushi.top

[R23] 字符串替换
来源：http://pjw.chenjidiqi.icu

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://iyp.bjfxy.top

[R24] 大小写转换
来源：http://tci.aizwys.cn

echo "${s^^}"; echo "${s,,}"
来源：http://sae.meibo888.top

[R25] 去后缀 / 去前缀
来源：http://xlm.zdbjq.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://zpi.ydjk.org.cn

[R26] 命令替换
来源：http://lbp.kuanghao11.cn

now=$(date +%F); echo "$now"
来源：http://tmd.gzhubu.top

[R27] 算术展开
来源：http://buv.zhiwuduotai.top

echo $((1 + 2 * 3))
来源：http://kok.iojbl.cn

[R28] 浮点运算
来源：http://nyk.shangyingyoupin.top

echo "scale=2; 10/3" | bc
来源：http://ziq.shuidangran.top

[R29] 定义函数
来源：http://vxa.quarkkingdee.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rlj.wangshuangyany.cn

[R30] 函数返回状态码
来源：http://uds.hfpthk.cn

f() { return 0; }; f || echo "失败了"
来源：http://pal.cheryme.top

[R31] 局部变量
来源：http://zls.ctjpmb.com

f() { local x=1; echo "$x"; }
来源：http://yrr.tian-w.cn

[R32] 参数个数校验
来源：http://ipz.redwolf501.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sih.epnwcf.com

[R33] 捕获错误并提示行号
来源：http://qjj.nwbrower.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mxa.nanxuanxn.top

[R34] 退出时清理
来源：http://iyf.yueranfly.top

trap 'rm -f "$tmp"' EXIT
来源：http://sni.316326.xyz

[R35] 后台执行并等待
来源：http://jnw.jqgufenzy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://eob.fzhhl.top

[R36] 并发执行多个任务
来源：http://svh.jinqigfzy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://luz.uphjek.com

[R37] 把输出赋给变量
来源：http://ebm.fengsongda.top

files=$(ls -1)
来源：http://zqx.guowangkeji.top

[R38] 管道串联
来源：http://hgr.ehwqpu.com

cat a.txt | grep -i error | wc -l
来源：http://rcz.gotoacloud.top

[R39] 重定向标准输出与错误
来源：http://ufg.daria6918.cn

cmd > out.log 2>&1
来源：http://sqj.tianlin.xyz

[R40] 追加写日志
来源：http://gmf.nanxinkj.top

echo "log" >> out.log
来源：http://yod.smart0.xyz

[R41] 丢弃输出
来源：http://tdl.cheryme.top

cmd >/dev/null 2>&1
来源：http://aax.hongshengwenyu.top

[R42] 输入重定向
来源：http://nnw.birdmap.top

wc -l < a.txt
来源：http://kip.shzxlz.cn

[R43] 按名字查找文件
来源：http://hlh.nwbrower.top

find . -name "*.log" -type f
来源：http://yvq.zhixingplan.top

[R44] 按修改时间查找
来源：http://mkw.yongpay.top

find . -mtime -7 -type f
来源：http://vdm.zhengqikj.top

[R45] 批量删除
来源：http://irk.xuetiantiany.cn

find . -name "*.tmp" -delete
来源：http://fxo.ehwqpu.com

[R46] 递归替换文件内容
来源：http://qkp.iojbl.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rnw.jianghu66.top

[R47] sed 单行替换
来源：http://dio.316326.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://fsp.zhoulong.xyz

[R48] awk 取指定列
来源：http://hpv.hysaishi.cn

awk '{print $1, $3}' a.txt
来源：http://uqy.9152youxi.cn

[R49] awk 带条件
来源：http://wkg.316326.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cbn.hammf.cn

[R50] awk 求和
来源：http://lnk.fengsongda.top

awk '{s += $2} END {print s}' a.txt
来源：http://zac.jianghu66.top

[R51] 排序去重取前几
来源：http://anl.hesvh.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://yce.quarkkingdee.top

[R52] 统计行数
来源：http://fbb.jianghu66.top

wc -l a.txt
来源：http://dgo.gaohongyu789.top

[R53] 查看文件头与实时尾
来源：http://ycx.yfazqb.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ejf.nanxuanxn.top

[R54] 比较两个文件
来源：http://nia.zhiwuduotai.top

diff a.txt b.txt
来源：http://ujo.snrcjt.cn

[R55] 压缩与解压
来源：http://ghp.ywan-chungtsiang.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zug.gogol.net.cn

[R56] 远程拷贝
来源：http://nof.yuxming.cn

scp file user@host:/path/
来源：http://grc.ctjpmb.com

[R57] 远程执行命令
来源：http://dvl.meibo888.top

ssh user@host 'uptime'
来源：http://vrr.ydjk.org.cn

[R58] 下载文件
来源：http://jgi.ybcxt.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://paa.jinqigufen.top

[R59] 发 POST JSON
来源：http://qre.jlsjyb.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xey.haohaochexian.top

[R60] 只看 HTTP 状态码
来源：http://jbu.daria6918.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bpj.yongpay.top

[R61] 磁盘占用
来源：http://jgu.chenlongwang.top

df -h;  du -sh *
来源：http://lkd.jinghuilouyu.cn

[R62] 找最占空间的文件
来源：http://lka.yuxming.cn

du -ah . | sort -rh | head -10
来源：http://hbq.chenzaomai.com

[R63] 内存与进程
来源：http://irh.quarkkingdee.top

free -h;  ps aux | grep nginx
来源：http://dkh.guannengcc.top

[R64] 结束进程
来源：http://vpt.tarul.cn

kill -9 $(pgrep -f app.py)
来源：http://ndy.ctjpmb.com

[R65] 查看端口占用
来源：http://ide.aibaodan.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hxa.tanke756.top

[R66] 定时任务
来源：http://imi.havefunace.top

crontab -e;  crontab -l
来源：http://yns.haohaochexian.top

[R67] 生成随机十六进制串
来源：http://iya.shangyingyoupin.top

openssl rand -hex 16
来源：http://rlw.zycfv.cn

[R68] 计算文件校验值
来源：http://rnz.jyoumei.cn

sha256sum a.txt;  md5sum a.txt
来源：http://aah.zhoulong.xyz

[R69] 生成随机密码
来源：http://hyv.xylfe.cn

head -c 16 /dev/urandom | base64
来源：http://mam.tanke756.top

[R70] 时间戳与互转
来源：http://bgd.yanxiufei.cn

date +%s;  date -d @1700000000
来源：http://qij.hfpthk.cn

[R71] 日期格式化
来源：http://azb.havefunace.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://tcu.jiagoushi.top

[R72] 等待端口就绪
来源：http://vnv.ydzc1.top

until nc -z localhost 3306; do sleep 1; done
来源：http://gsk.guowangkeji.top

[R73] 分割大日志
来源：http://aau.nanxuanxn.top

split -l 1000 big.log part_
来源：http://rvf.yj20258888.top

[R74] 批量重命名
来源：http://cuc.zhaomingkeji.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://eda.zhoulong.xyz

[R75] 导出环境变量
来源：http://hzc.guowangkeji.top

export PATH="$HOME/bin:$PATH"
来源：http://igq.chenlongwang.top

[R76] 使用临时文件
来源：http://tuk.andypj.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wuu.uphjek.com

[R77] 读取用户输入
来源：http://ptx.zhongyouzk.top

read -rp "请输入: " ans
来源：http://zgo.hcnkem.com

[R78] 交互式菜单
来源：http://lsx.zhengqikj.top

select opt in a b c; do echo "$opt"; break; done
来源：http://new.cdnleiting.top

[R79] 解析命令行选项
来源：http://yyi.mhx1999.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xkn.wangdashe.top

[R80] 查看脚本执行耗时
来源：http://ozr.jianghu66.top

time ./run.sh
来源：http://eop.yvedp.cn

================================================================================
来源：http://zxv.zdqjudy.top

S. C / C++ 专题
来源：http://tej.gotoacloud.top

================================================================================
来源：http://toh.ppjwa.cn

[S01] C：Hello World
来源：http://pap.zhijiandao.cn

#include <stdio.h>
来源：http://lsl.wangdashe.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ipc.yuxming.cn

[S02] C：变量与格式化输出
来源：http://kwz.yuanzhike.top

int a = 10; printf("%d\n", a);
来源：http://fwc.tian-w.cn

[S03] C：读入整数
来源：http://xie.iojbl.cn

int x; scanf("%d", &x);
来源：http://wpg.jqgfzy.top

[S04] C：字符串复制
来源：http://lmy.chenjidiqi.icu

char dst[32]; strcpy(dst, "hi");
来源：http://cbb.dianchejie.cn

[S05] C：字符串长度
来源：http://loz.nanxuanxn.top

strlen(s)
来源：http://jbf.dianchejie.cn

[S06] C：字符串比较
来源：http://yzc.shangyingyoupin.top

strcmp(a, b) == 0
来源：http://ksm.guowangkeji.top

[S07] C：数组遍历求和
来源：http://sae.nanxuanxn.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ccn.jinghuilouyu.cn

[S08] C：动态内存分配与释放
来源：http://awh.fanxiaobao.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gby.hysaishi.cn

[S09] C：结构体定义与初始化
来源：http://dpm.zhixingplan.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xee.dashuyun.cn

[S10] C：指针与解引用
来源：http://rph.c1oappe.top

int *p = &a;  *p = 5;
来源：http://fsr.havefunace.top

[S11] C：逐行读文件
来源：http://xbq.dianchejie.cn

FILE *f = fopen("a.txt", "r");
来源：http://slg.iojbl.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://gov.zhoulong.xyz

fclose(f);
来源：http://qms.ywan-chungtsiang.top

[S12] C：写文件
来源：http://irp.birdmap.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kiv.bjfxy.top

[S13] C：宏定义
来源：http://sgd.xuetiantiany.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gry.fehbvm.com

[S14] C：枚举
来源：http://uzv.vqdsnc.cn

enum Color { RED, GREEN, BLUE };
来源：http://axv.yj20258888.top

[S15] C：类型转换
来源：http://qgn.hammf.cn

(double) a / b
来源：http://ymj.sjlbkw.cn

[S16] C：位操作置位
来源：http://vmn.gaohongyu789.top

x |= (1 << 3);
来源：http://zta.yonumen.top

[S17] C：安全拼接字符串
来源：http://bns.zhengqikj.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wrf.nanxuanxn.top

[S18] C：命令行参数
来源：http://qps.mhx1999.top

int main(int argc, char **argv)
来源：http://fxi.iojbl.cn

[S19] C：快速排序
来源：http://pcg.hammf.cn

qsort(a, n, sizeof(int), cmp);
来源：http://dfh.dianchejie.cn

[S20] C：二分查找
来源：http://ori.kuanghao11.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pag.316326.xyz

[S21] C：字符类别判断
来源：http://fny.hongshengwenyu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xay.andypj.xyz

[S22] C：字符串转数字
来源：http://ifi.zhongyouzk.top

atoi("42");  strtod("3.14", NULL);
来源：http://gzp.hywenlv.cn

[S23] C：随机数
来源：http://xwv.yfazqb.com

srand(time(NULL));  int r = rand() % 100;
来源：http://wrx.zhongyouzk.top

[S24] C：获取本地时间
来源：http://kra.quarkkingdee.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jjx.bjfxy.top

[S25] C：内存拷贝
来源：http://tlx.jinghuilouyu.cn

memcpy(dst, src, n);
来源：http://idq.nanxuanxn.top

[S26] C：内存清零
来源：http://vne.hammf.cn

memset(a, 0, sizeof a);
来源：http://rbd.yuanzhike.top

[S27] C：定义常量
来源：http://ivz.nanxinkj.top

const double PI = 3.14159;
来源：http://awo.jyoumei.cn

[S28] C：静态变量
来源：http://uce.52xcode.cn

static int counter = 0;
来源：http://ssp.xylfe.cn

[S29] C：变参函数
来源：http://uqc.hcnkem.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wek.xuanzx.com

[S30] C：头文件保护
来源：http://wkh.iojbl.cn

#ifndef X_H
来源：http://isn.yj202588.top

#define X_H
来源：http://rry.birdmap.top

#endif
来源：http://rrt.iojbl.cn

[S31] C++：Hello World
来源：http://ota.jinqigfzy.top

#include <iostream>
来源：http://arg.yj202588.top

int main() { std::cout << "Hello\n"; }
来源：http://rjq.jinyuanbaomall.cn

[S32] C++：字符串
来源：http://vam.tarul.cn

std::string s = "hi";  s += "!";
来源：http://jiq.sxryk.cn

[S33] C++：vector 增删
来源：http://jre.sufxvd.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bim.zycfv.cn

[S34] C++：遍历 vector
来源：http://kjz.jiagoushi.top

for (auto &x : v) { std::cout << x; }
来源：http://nym.jqgfzy.top

[S35] C++：map
来源：http://ygi.pengpengdd.cyou

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ook.dashuyun.cn

[S36] C++：unordered_map
来源：http://wnd.yongpay.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ozh.zhiwuduotai.top

[S37] C++：set
来源：http://wja.jinghuilouyu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ocz.hesvh.cn

[S38] C++：排序
来源：http://ohz.tian-w.cn

std::sort(v.begin(), v.end());
来源：http://cfj.yj20258888.top

[S39] C++：自定义比较器排序
来源：http://pyd.zhiwuduotai.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dot.xuanzx.com

[S40] C++：查找元素
来源：http://osp.tianlin.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wwx.yj20258888.top

[S41] C++：类与构造函数
来源：http://epc.dianchejie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ohh.shangyingyoupin.top

[S42] C++：继承与虚函数
来源：http://xsl.dianchejie.cn

class B : public Base { public: void f() override {} };
来源：http://lry.fengsongda.top

[S43] C++：智能指针
来源：http://iyg.fengsongda.top

auto p = std::make_unique<int>(5);
来源：http://hsl.ctjpmb.com

[S44] C++：引用传参
来源：http://qxe.sweek.top

void inc(int &x) { ++x; }
来源：http://nmg.havefunace.top

[S45] C++：lambda
来源：http://njt.vehdjk.com

auto add = [](int a, int b) { return a + b; };
来源：http://vuy.hywenlv.cn

[S46] C++：函数模板
来源：http://qxs.feifeiyinyue.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wth.fzhhl.top

[S47] C++：结构化绑定遍历
来源：http://hpw.epnwcf.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wlu.hysaishi.cn

[S48] C++：逐行读文件
来源：http://vuj.pycfn.com

std::ifstream in("a.txt");  std::string line;
来源：http://qyd.sysykeji.top

while (std::getline(in, line)) { }
来源：http://mlf.zycfv.cn

[S49] C++：写文件
来源：http://mtc.aizwys.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ymf.jinqigufen.top

[S50] C++：格式化数字
来源：http://kup.zdbjq.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ufz.dashuyun.cn

[S51] C++：显式类型转换
来源：http://erd.hywenlv.cn

static_cast<double>(a) / b
来源：http://ezu.zhixingplan.top

[S52] C++：const 与 noexcept
来源：http://hze.tian-w.cn

int size() const noexcept { return n_; }
来源：http://vow.uphjek.com

[S53] C++：移动语义
来源：http://mcw.fanxiaobao.xyz

std::vector<int> w = std::move(v);
来源：http://tuq.smart0.xyz

[S54] C++：异常处理
来源：http://qsg.tianlin.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hyr.hnxiangtu.top

[S55] C++：结构化绑定
来源：http://fty.jianghu66.top

auto [a, b] = std::make_pair(1, 2);
来源：http://cvu.haohaochexian.top

[S56] C++：optional
来源：http://ueu.hesvh.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://knx.hcnkem.com

[S57] C++：编译期常量
来源：http://rvp.dashuyun.cn

constexpr int N = 10;
来源：http://kod.chenzaomai.com

[S58] C++：命名空间
来源：http://vmd.sxryk.cn

namespace ns { int f() { return 1; } }
来源：http://dwy.guowangkeji.top

[S59] C++：静态断言
来源：http://rql.hfpthk.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xid.jqgufenzy.top

[S60] C++：遍历并删除元素
来源：http://jxd.birdmap.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fjz.hfpthk.cn

================================================================================
来源：http://kdn.bbcook.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xcr.yj20258.top

================================================================================
来源：http://mus.gotoacloud.top

[T01] Kotlin：Hello World
来源：http://jsm.nwbrower.top

println("Hello")
来源：http://keo.yj20258888.top

[T02] Kotlin：变量
来源：http://xso.fanxiaobao.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ygg.ydzc1.top

[T03] Kotlin：字符串模板
来源：http://kve.iojbl.cn

"值: $b"
来源：http://keg.zdbjq.cn

[T04] Kotlin：空安全
来源：http://huw.mhx1999.top

val n: String? = null;  n?.length
来源：http://poc.daria6918.cn

[T05] Kotlin：when 表达式
来源：http://gcl.cdnleiting.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bea.tianlin.xyz

[T06] Kotlin：集合映射
来源：http://nha.yonumen.top

listOf(1, 2, 3).map { it * 2 }
来源：http://tyo.chenjidiqi.icu

[T07] Kotlin：集合过滤
来源：http://lmb.zhixingplan.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://brq.jiagoushi.top

[T08] Kotlin：数据类
来源：http://hkg.cheryme.top

data class User(val name: String, val age: Int)
来源：http://lhf.sysykeji.top

[T09] Kotlin：扩展函数
来源：http://ldr.wangshuangyany.cn

fun String.exclaim() = this + "!"
来源：http://mnr.uphjek.com

[T10] Kotlin：默认参数
来源：http://iqd.wangdashe.top

fun greet(name: String = "World") = "Hi $name"
来源：http://qnr.guowangkeji.top

[T11] Kotlin：协程
来源：http://pzy.daxiang520.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://ioy.jyoumei.cn

[T12] Kotlin：解构声明
来源：http://xew.yuanzhike.top

val (a, b) = Pair(1, 2)
来源：http://ver.ybcxt.top

[T13] Kotlin：只读 Map
来源：http://eva.fehbvm.com

val m = mapOf("a" to 1)
来源：http://juo.cqqwz.cn

[T14] Kotlin：循环
来源：http://inp.uphjek.com

for (i in 1..10) println(i)
来源：http://btn.jinyuanbaomall.cn

[T15] Kotlin：接口
来源：http://pre.chenlongwang.top

interface Shape { fun area(): Double }
来源：http://zga.meibo888.top

[T16] Swift：Hello World
来源：http://hue.smart0.xyz

print("Hello")
来源：http://lds.yangfankeji.com

[T17] Swift：变量与常量
来源：http://cpj.ivvv.top

var a = 1;  let b = 2
来源：http://ioq.quarkkingdee.top

[T18] Swift：字符串插值
来源：http://zfd.daxiang520.top

"值: \(b)"
来源：http://amc.bjfxy.top

[T19] Swift：可选绑定
来源：http://qqn.smart0.xyz

if let n = opt { print(n) }
来源：http://qmp.jyoumei.cn

[T20] Swift：数组操作
来源：http://ded.52xcode.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qva.tarul.cn

[T21] Swift：遍历
来源：http://nwl.aibaodan.cn

for x in a { print(x) }
来源：http://nwn.fengsongda.top

[T22] Swift：字典
来源：http://bge.yfazqb.com

var d = ["a": 1];  d["b"] = 2
来源：http://kkf.ybcxt.top


<!-- 参考信息 -->