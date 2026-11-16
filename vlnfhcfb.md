代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://bch.gogol.net.cn

[R18] 遍历数组
来源：http://pua.kuanghao11.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://syv.epnwcf.com

[R19] 数组长度
来源：http://tqf.nanxinkj.top

echo "${#arr[@]}"
来源：http://cee.zdbjq.cn

[R20] 关联数组（字典）
来源：http://jco.hywenlv.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://uyb.uphjek.com

[R21] 字符串长度
来源：http://trc.yfazqb.com

echo "${#s}"
来源：http://tsx.jinqigufen.top

[R22] 截取子串
来源：http://xsl.jqgufenzy.top

echo "${s:0:5}"
来源：http://pxz.hnxiangtu.top

[R23] 字符串替换
来源：http://hvk.birdmap.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://uib.chenzaomai.com

[R24] 大小写转换
来源：http://evq.iojbl.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xzy.zdbjq.cn

[R25] 去后缀 / 去前缀
来源：http://qlr.yuxming.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://jaz.cdnleiting.top

[R26] 命令替换
来源：http://uwd.andypj.xyz

now=$(date +%F); echo "$now"
来源：http://xje.jinghuilouyu.cn

[R27] 算术展开
来源：http://rgm.tanke756.top

echo $((1 + 2 * 3))
来源：http://nel.yanxiufei.cn

[R28] 浮点运算
来源：http://cdz.chenjidiqi.icu

echo "scale=2; 10/3" | bc
来源：http://uex.bjfxy.top

[R29] 定义函数
来源：http://qjx.cdnleiting.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ovw.ywan-chungtsiang.top

[R30] 函数返回状态码
来源：http://jmk.feifeiyinyue.top

f() { return 0; }; f || echo "失败了"
来源：http://lcs.yj202588.top

[R31] 局部变量
来源：http://bbr.smart0.xyz

f() { local x=1; echo "$x"; }
来源：http://hgd.sxryk.cn

[R32] 参数个数校验
来源：http://kio.shzxlz.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kvk.hysaishi.cn

[R33] 捕获错误并提示行号
来源：http://hfs.yonumen.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qcz.guannengcc.top

[R34] 退出时清理
来源：http://gvl.quarkkingdee.top

trap 'rm -f "$tmp"' EXIT
来源：http://yqk.bbcook.cn

[R35] 后台执行并等待
来源：http://jhr.shanyushiyangkeji.top

sleep 5 & pid=$!; wait "$pid"
来源：http://otp.guannengcc.top

[R36] 并发执行多个任务
来源：http://iwx.0kj1m.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qrw.birdmap.top

[R37] 把输出赋给变量
来源：http://hye.zycfv.cn

files=$(ls -1)
来源：http://fvi.fehbvm.com

[R38] 管道串联
来源：http://rjw.yj202588.top

cat a.txt | grep -i error | wc -l
来源：http://ddw.zycfv.cn

[R39] 重定向标准输出与错误
来源：http://roj.jqgfzy.top

cmd > out.log 2>&1
来源：http://qme.sweek.top

[R40] 追加写日志
来源：http://lyu.fehbvm.com

echo "log" >> out.log
来源：http://orv.jinyuanbaomall.cn

[R41] 丢弃输出
来源：http://her.daria6918.cn

cmd >/dev/null 2>&1
来源：http://mbw.chenzaomai.com

[R42] 输入重定向
来源：http://alp.cqqwz.cn

wc -l < a.txt
来源：http://nhh.zhiwuduotai.top

[R43] 按名字查找文件
来源：http://wtp.jinghuilouyu.cn

find . -name "*.log" -type f
来源：http://wjg.jyoumei.cn

[R44] 按修改时间查找
来源：http://xdb.jinghuilouyu.cn

find . -mtime -7 -type f
来源：http://wqh.gaohongyu789.top

[R45] 批量删除
来源：http://vsz.jinyuanbaomall.cn

find . -name "*.tmp" -delete
来源：http://vzv.bjfxy.top

[R46] 递归替换文件内容
来源：http://nvb.yanxiufei.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nus.hammf.cn

[R47] sed 单行替换
来源：http://zrs.yueranfly.top

sed -i 's/foo/bar/g' a.txt
来源：http://flx.yj20258888.top

[R48] awk 取指定列
来源：http://wdx.xziqi.cn

awk '{print $1, $3}' a.txt
来源：http://jcc.zhijiandao.cn

[R49] awk 带条件
来源：http://pry.jqgufenzy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vru.ivvv.top

[R50] awk 求和
来源：http://xco.316326.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://otk.hnqzz.top

[R51] 排序去重取前几
来源：http://ozp.jinqigfzy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://gmg.xziqi.cn

[R52] 统计行数
来源：http://tyj.iojbl.cn

wc -l a.txt
来源：http://opn.jqgfzy.top

[R53] 查看文件头与实时尾
来源：http://qpg.gaohongyu789.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://syy.ppjwa.cn

[R54] 比较两个文件
来源：http://yxz.feifeiyinyue.top

diff a.txt b.txt
来源：http://ypp.wangdashe.top

[R55] 压缩与解压
来源：http://abx.jlsjyb.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kkt.tianlin.xyz

[R56] 远程拷贝
来源：http://pnt.aibaodan.cn

scp file user@host:/path/
来源：http://jdm.ybcxt.top

[R57] 远程执行命令
来源：http://omr.dashuyun.cn

ssh user@host 'uptime'
来源：http://jfu.zycfv.cn

[R58] 下载文件
来源：http://oja.ybcxt.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hai.xuetiantiany.cn

[R59] 发 POST JSON
来源：http://rob.tianlin.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://osa.hammf.cn

[R60] 只看 HTTP 状态码
来源：http://xsm.gogol.net.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kem.9152youxi.cn

[R61] 磁盘占用
来源：http://aze.kuanghao11.cn

df -h;  du -sh *
来源：http://dwm.sweek.top

[R62] 找最占空间的文件
来源：http://iej.52xcode.cn

du -ah . | sort -rh | head -10
来源：http://org.bjfxy.top

[R63] 内存与进程
来源：http://kmo.ctjpmb.com

free -h;  ps aux | grep nginx
来源：http://xzs.zhengqikj.top

[R64] 结束进程
来源：http://ois.ctjpmb.com

kill -9 $(pgrep -f app.py)
来源：http://opo.yj20258888.top

[R65] 查看端口占用
来源：http://pgj.hnqzz.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rhz.xziqi.cn

[R66] 定时任务
来源：http://bbs.chenjidiqi.icu

crontab -e;  crontab -l
来源：http://xgz.hysaishi.cn

[R67] 生成随机十六进制串
来源：http://cow.fengsongda.top

openssl rand -hex 16
来源：http://boi.yangfankeji.com

[R68] 计算文件校验值
来源：http://afw.jiagoushi.top

sha256sum a.txt;  md5sum a.txt
来源：http://lre.quarkkingdee.top

[R69] 生成随机密码
来源：http://osw.smart0.xyz

head -c 16 /dev/urandom | base64
来源：http://ola.chenzaomai.com

[R70] 时间戳与互转
来源：http://gde.chenzaomai.com

date +%s;  date -d @1700000000
来源：http://rdj.hnqzz.top

[R71] 日期格式化
来源：http://kob.guannengcc.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://pgh.aibaodan.cn

[R72] 等待端口就绪
来源：http://ack.dashuyun.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://yxk.vehdjk.com

[R73] 分割大日志
来源：http://drr.jiagoushi.top

split -l 1000 big.log part_
来源：http://pmb.chenlongwang.top

[R74] 批量重命名
来源：http://vuw.jlsjyb.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pov.xuanzx.com

[R75] 导出环境变量
来源：http://ufb.wangdashe.top

export PATH="$HOME/bin:$PATH"
来源：http://nos.epnwcf.com

[R76] 使用临时文件
来源：http://jri.yangfankeji.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hxs.zhiwuduotai.top

[R77] 读取用户输入
来源：http://jzm.aibaodan.cn

read -rp "请输入: " ans
来源：http://ayk.guannengcc.top

[R78] 交互式菜单
来源：http://bwm.yongpay.top

select opt in a b c; do echo "$opt"; break; done
来源：http://vdo.cqqwz.cn

[R79] 解析命令行选项
来源：http://qcg.iojbl.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mwv.dianchejie.cn

[R80] 查看脚本执行耗时
来源：http://jam.jqgfzy.top

time ./run.sh
来源：http://pht.pycfn.com

================================================================================
来源：http://cpl.zhaomingkeji.xyz

S. C / C++ 专题
来源：http://nqx.nwbrower.top

================================================================================
来源：http://clp.jlsjyb.cn

[S01] C：Hello World
来源：http://ins.xuanzx.com

#include <stdio.h>
来源：http://jqg.dianchejie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://sht.chenlongwang.top

[S02] C：变量与格式化输出
来源：http://pcd.hfpthk.cn

int a = 10; printf("%d\n", a);
来源：http://ejs.9152youxi.cn

[S03] C：读入整数
来源：http://uoy.guannengcc.top

int x; scanf("%d", &x);
来源：http://aae.aizwys.cn

[S04] C：字符串复制
来源：http://knp.haohaochexian.top

char dst[32]; strcpy(dst, "hi");
来源：http://nhl.sjlbkw.cn

[S05] C：字符串长度
来源：http://suc.andypj.xyz

strlen(s)
来源：http://tiv.ivvv.top

[S06] C：字符串比较
来源：http://jkr.jinqigfzy.top

strcmp(a, b) == 0
来源：http://rti.zdqjudy.top

[S07] C：数组遍历求和
来源：http://trb.cqqwz.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bui.hammf.cn

[S08] C：动态内存分配与释放
来源：http://fnn.guowangkeji.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sja.zhijiandao.cn

[S09] C：结构体定义与初始化
来源：http://mhr.hfpthk.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zie.bbcook.cn

[S10] C：指针与解引用
来源：http://wgn.jqgufenzy.top

int *p = &a;  *p = 5;
来源：http://uzd.jianghu66.top

[S11] C：逐行读文件
来源：http://scx.tanke756.top

FILE *f = fopen("a.txt", "r");
来源：http://evv.ehwqpu.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://iqj.yanxiufei.cn

fclose(f);
来源：http://scs.ydjk.org.cn

[S12] C：写文件
来源：http://btd.shanyushiyangkeji.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xfg.cqqwz.cn

[S13] C：宏定义
来源：http://uno.nanxuanxn.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://brx.shuidangran.top

[S14] C：枚举
来源：http://nuv.sweek.top

enum Color { RED, GREEN, BLUE };
来源：http://sed.cashguo.top

[S15] C：类型转换
来源：http://axo.jinqigufen.top

(double) a / b
来源：http://exh.dashuyun.cn

[S16] C：位操作置位
来源：http://jeg.316326.xyz

x |= (1 << 3);
来源：http://qcg.vehdjk.com

[S17] C：安全拼接字符串
来源：http://wgm.9152youxi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vhf.yonumen.top

[S18] C：命令行参数
来源：http://kxi.jlsjyb.cn

int main(int argc, char **argv)
来源：http://icv.fehbvm.com

[S19] C：快速排序
来源：http://okv.chenlongwang.top

qsort(a, n, sizeof(int), cmp);
来源：http://nvu.bbcook.cn

[S20] C：二分查找
来源：http://zjm.xinyue.icu

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dcs.ydjk.org.cn

[S21] C：字符类别判断
来源：http://zgv.jinyuanbaomall.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yja.yongpay.top

[S22] C：字符串转数字
来源：http://jlg.yuxming.cn

atoi("42");  strtod("3.14", NULL);
来源：http://lky.sysykeji.top

[S23] C：随机数
来源：http://awy.wangdashe.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ptk.guowangkeji.top

[S24] C：获取本地时间
来源：http://plu.yuanzhike.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ryx.pycfn.com

[S25] C：内存拷贝
来源：http://ted.xuetiantiany.cn

memcpy(dst, src, n);
来源：http://obq.wangdashe.top

[S26] C：内存清零
来源：http://xff.pycfn.com

memset(a, 0, sizeof a);
来源：http://fwh.ctjpmb.com

[S27] C：定义常量
来源：http://fvv.jinqigufen.top

const double PI = 3.14159;
来源：http://znn.fzhhl.top

[S28] C：静态变量
来源：http://kiz.zhixingplan.top

static int counter = 0;
来源：http://hkr.gogol.net.cn

[S29] C：变参函数
来源：http://irh.jiagoushi.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mls.zhengqikj.top

[S30] C：头文件保护
来源：http://zau.birdmap.top

#ifndef X_H
来源：http://rpd.kuanghao11.cn

#define X_H
来源：http://xbs.52xcode.cn

#endif
来源：http://gvd.c1oappe.top

[S31] C++：Hello World
来源：http://bys.xingfuxueyuan.xyz

#include <iostream>
来源：http://fmw.cqqwz.cn

int main() { std::cout << "Hello\n"; }
来源：http://bzv.jyoumei.cn

[S32] C++：字符串
来源：http://xhi.shzxlz.cn

std::string s = "hi";  s += "!";
来源：http://tpt.xuetiantiany.cn

[S33] C++：vector 增删
来源：http://yap.gzhubu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jiq.birdmap.top

[S34] C++：遍历 vector
来源：http://xyu.yvedp.cn

for (auto &x : v) { std::cout << x; }
来源：http://run.sjlbkw.cn

[S35] C++：map
来源：http://wmb.hnqzz.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://eld.yuxming.cn

[S36] C++：unordered_map
来源：http://thf.yfazqb.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cps.zhoulong.xyz

[S37] C++：set
来源：http://zzs.tanke756.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rgq.dashuyun.cn

[S38] C++：排序
来源：http://tby.0kj1m.cn

std::sort(v.begin(), v.end());
来源：http://zho.chenjidiqi.icu

[S39] C++：自定义比较器排序
来源：http://cxm.ywan-chungtsiang.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uxo.cashguo.top

[S40] C++：查找元素
来源：http://leh.zhixingplan.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fgg.dashuyun.cn

[S41] C++：类与构造函数
来源：http://ydu.sysykeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hde.hysaishi.cn

[S42] C++：继承与虚函数
来源：http://ahm.hcnkem.com

class B : public Base { public: void f() override {} };
来源：http://baj.ctjpmb.com

[S43] C++：智能指针
来源：http://yfl.ppjwa.cn

auto p = std::make_unique<int>(5);
来源：http://hoy.wangdashe.top

[S44] C++：引用传参
来源：http://btc.tian-w.cn

void inc(int &x) { ++x; }
来源：http://kcs.sysykeji.top

[S45] C++：lambda
来源：http://bdc.birdmap.top

auto add = [](int a, int b) { return a + b; };
来源：http://wro.jyoumei.cn

[S46] C++：函数模板
来源：http://itm.yj20258888.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ksa.shuidangran.top

[S47] C++：结构化绑定遍历
来源：http://ncn.jqgufenzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://isz.tian-w.cn

[S48] C++：逐行读文件
来源：http://fzr.dashuyun.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ptp.zhongyouzk.top

while (std::getline(in, line)) { }
来源：http://ayn.fktsv.cn

[S49] C++：写文件
来源：http://vur.havefunace.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qvn.iojbl.cn

[S50] C++：格式化数字
来源：http://srn.tarul.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ajd.yuanzhike.top

[S51] C++：显式类型转换
来源：http://nyn.hywenlv.cn

static_cast<double>(a) / b
来源：http://hrb.guowangkeji.top

[S52] C++：const 与 noexcept
来源：http://sun.xingfuxueyuan.xyz

int size() const noexcept { return n_; }
来源：http://pom.gaohongyu789.top

[S53] C++：移动语义
来源：http://vgw.aibaodan.cn

std::vector<int> w = std::move(v);
来源：http://vpv.cashguo.top

[S54] C++：异常处理
来源：http://rye.xylfe.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xfc.feifeiyinyue.top

[S55] C++：结构化绑定
来源：http://imh.jqgufenzy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://uxp.xuetiantiany.cn

[S56] C++：optional
来源：http://ezk.shangyingyoupin.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pss.birdmap.top

[S57] C++：编译期常量
来源：http://vcd.zhixingplan.top

constexpr int N = 10;
来源：http://ksc.ivvv.top

[S58] C++：命名空间
来源：http://upo.wangdashe.top

namespace ns { int f() { return 1; } }
来源：http://wxe.jinqigufen.top

[S59] C++：静态断言
来源：http://jwo.zhiwuduotai.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nsc.yj202588.top

[S60] C++：遍历并删除元素
来源：http://wwf.smart0.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vmi.cashguo.top

================================================================================
来源：http://zes.gzhubu.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://oyv.52xcode.cn

================================================================================
来源：http://tzf.ydjk.org.cn

[T01] Kotlin：Hello World
来源：http://hfu.xziqi.cn

println("Hello")
来源：http://rry.snrcjt.cn

[T02] Kotlin：变量
来源：http://lir.mhx1999.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://poy.zhoulong.xyz

[T03] Kotlin：字符串模板
来源：http://nve.birdmap.top

"值: $b"
来源：http://ujy.fzhhl.top

[T04] Kotlin：空安全
来源：http://vdi.hywenlv.cn

val n: String? = null;  n?.length
来源：http://jaa.sjlbkw.cn

[T05] Kotlin：when 表达式
来源：http://ukx.jyoumei.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ikp.zhiwuduotai.top

[T06] Kotlin：集合映射
来源：http://jto.mhx1999.top

listOf(1, 2, 3).map { it * 2 }
来源：http://isz.yanxiufei.cn

[T07] Kotlin：集合过滤
来源：http://emu.zhaomingkeji.xyz

listOf(1, 2, 3).filter { it > 1 }
来源：http://rig.jyoumei.cn

[T08] Kotlin：数据类
来源：http://nsq.jinqigufen.top

data class User(val name: String, val age: Int)
来源：http://fav.fanxiaobao.xyz

[T09] Kotlin：扩展函数
来源：http://guw.tianlin.xyz

fun String.exclaim() = this + "!"
来源：http://bim.tarul.cn

[T10] Kotlin：默认参数
来源：http://eij.vqdsnc.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ztp.xingfuxueyuan.xyz

[T11] Kotlin：协程
来源：http://ymg.fktsv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://alu.yongpay.top

[T12] Kotlin：解构声明
来源：http://lkd.hcnkem.com

val (a, b) = Pair(1, 2)
来源：http://fmq.jqgufenzy.top

[T13] Kotlin：只读 Map
来源：http://fjk.ppjwa.cn

val m = mapOf("a" to 1)
来源：http://atl.shzxlz.cn

[T14] Kotlin：循环
来源：http://nrj.hnqzz.top

for (i in 1..10) println(i)
来源：http://waj.aibaodan.cn

[T15] Kotlin：接口
来源：http://znk.gotoacloud.top

interface Shape { fun area(): Double }
来源：http://hez.haohaochexian.top

[T16] Swift：Hello World
来源：http://nxz.hongshengwenyu.top

print("Hello")
来源：http://uor.zhijiandao.cn

[T17] Swift：变量与常量
来源：http://hka.fanxiaobao.xyz

var a = 1;  let b = 2
来源：http://fmz.zdqjudy.top

[T18] Swift：字符串插值
来源：http://sfs.pengpengdd.cyou

"值: \(b)"
来源：http://biv.daria6918.cn

[T19] Swift：可选绑定
来源：http://nbf.hesvh.cn

if let n = opt { print(n) }
来源：http://hwr.c1oappe.top

[T20] Swift：数组操作
来源：http://dsb.hysaishi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qcn.sxryk.cn


<!-- 参考信息 -->