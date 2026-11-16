代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://ekq.fktsv.cn

[R18] 遍历数组
来源：http://wfh.yj20258.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://okj.jinqigfzy.top

[R19] 数组长度
来源：http://qia.zhongyouzk.top

echo "${#arr[@]}"
来源：http://eig.hysaishi.cn

[R20] 关联数组（字典）
来源：http://tsa.jqgfzy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tde.52xcode.cn

[R21] 字符串长度
来源：http://ckw.jiagoushi.top

echo "${#s}"
来源：http://hvm.vqdsnc.cn

[R22] 截取子串
来源：http://kfu.yj202588.top

echo "${s:0:5}"
来源：http://mcg.ivvv.top

[R23] 字符串替换
来源：http://vtv.hcnkem.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sox.yueranfly.top

[R24] 大小写转换
来源：http://goa.c1oappe.top

echo "${s^^}"; echo "${s,,}"
来源：http://oyx.nanxinkj.top

[R25] 去后缀 / 去前缀
来源：http://wuc.zhiwuduotai.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://bjr.tanke756.top

[R26] 命令替换
来源：http://ssn.xylfe.cn

now=$(date +%F); echo "$now"
来源：http://mxf.zhoulong.xyz

[R27] 算术展开
来源：http://bec.hfpthk.cn

echo $((1 + 2 * 3))
来源：http://oci.jianghu66.top

[R28] 浮点运算
来源：http://wma.shangyingyoupin.top

echo "scale=2; 10/3" | bc
来源：http://prx.zhixingplan.top

[R29] 定义函数
来源：http://qko.dashuyun.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lqd.chenjidiqi.icu

[R30] 函数返回状态码
来源：http://auo.cucudq.cn

f() { return 0; }; f || echo "失败了"
来源：http://obu.yfazqb.com

[R31] 局部变量
来源：http://pdk.jlsjyb.cn

f() { local x=1; echo "$x"; }
来源：http://imk.yuanzhike.top

[R32] 参数个数校验
来源：http://glu.xziqi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wcx.daria6918.cn

[R33] 捕获错误并提示行号
来源：http://aws.bbcook.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cdm.xuetiantiany.cn

[R34] 退出时清理
来源：http://gfy.zycfv.cn

trap 'rm -f "$tmp"' EXIT
来源：http://mij.sxryk.cn

[R35] 后台执行并等待
来源：http://mcu.sysykeji.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ctt.ppjwa.cn

[R36] 并发执行多个任务
来源：http://cli.yuxming.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rhs.jqgufenzy.top

[R37] 把输出赋给变量
来源：http://ahl.jinqigufen.top

files=$(ls -1)
来源：http://foo.jianghu66.top

[R38] 管道串联
来源：http://jhx.meibo888.top

cat a.txt | grep -i error | wc -l
来源：http://yrv.tanke756.top

[R39] 重定向标准输出与错误
来源：http://wdg.yuanzhike.top

cmd > out.log 2>&1
来源：http://qfm.daria6918.cn

[R40] 追加写日志
来源：http://ehx.dianchejie.cn

echo "log" >> out.log
来源：http://jxd.shzxlz.cn

[R41] 丢弃输出
来源：http://rln.kuanghao11.cn

cmd >/dev/null 2>&1
来源：http://uae.sufxvd.cn

[R42] 输入重定向
来源：http://bdd.xuanzx.com

wc -l < a.txt
来源：http://poj.chenjidiqi.icu

[R43] 按名字查找文件
来源：http://yot.zhoulong.xyz

find . -name "*.log" -type f
来源：http://pbx.gogol.net.cn

[R44] 按修改时间查找
来源：http://tet.pycfn.com

find . -mtime -7 -type f
来源：http://euy.ydjk.org.cn

[R45] 批量删除
来源：http://abo.cashguo.top

find . -name "*.tmp" -delete
来源：http://lyq.sufxvd.cn

[R46] 递归替换文件内容
来源：http://hjq.jyoumei.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://itg.gotoacloud.top

[R47] sed 单行替换
来源：http://fha.bbcook.cn

sed -i 's/foo/bar/g' a.txt
来源：http://cns.nwbrower.top

[R48] awk 取指定列
来源：http://pwd.ybcxt.top

awk '{print $1, $3}' a.txt
来源：http://eez.jqgfzy.top

[R49] awk 带条件
来源：http://fdr.c1oappe.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xgy.guannengcc.top

[R50] awk 求和
来源：http://ntb.xingfuxueyuan.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://urm.gogol.net.cn

[R51] 排序去重取前几
来源：http://nxk.quarkkingdee.top

sort a.txt | uniq -c | sort -rn | head
来源：http://nkn.yuxming.cn

[R52] 统计行数
来源：http://qkj.jlsjyb.cn

wc -l a.txt
来源：http://wgu.hammf.cn

[R53] 查看文件头与实时尾
来源：http://ijf.hongshengwenyu.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gst.quarkkingdee.top

[R54] 比较两个文件
来源：http://trn.zdbjq.cn

diff a.txt b.txt
来源：http://dwe.mhx1999.top

[R55] 压缩与解压
来源：http://jut.andypj.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lbj.tian-w.cn

[R56] 远程拷贝
来源：http://fid.svipenyu.cn

scp file user@host:/path/
来源：http://eey.zdbjq.cn

[R57] 远程执行命令
来源：http://ufa.ybcxt.top

ssh user@host 'uptime'
来源：http://pfg.cdnleiting.top

[R58] 下载文件
来源：http://oim.yuanzhike.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://csu.meibo888.top

[R59] 发 POST JSON
来源：http://jme.zdbjq.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nqj.uphjek.com

[R60] 只看 HTTP 状态码
来源：http://nqi.jlsjyb.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://muw.wangshuangyany.cn

[R61] 磁盘占用
来源：http://ztt.vehdjk.com

df -h;  du -sh *
来源：http://imo.fengsongda.top

[R62] 找最占空间的文件
来源：http://rto.daxiang520.top

du -ah . | sort -rh | head -10
来源：http://ilg.smart0.xyz

[R63] 内存与进程
来源：http://arp.haohaochexian.top

free -h;  ps aux | grep nginx
来源：http://cij.cheryme.top

[R64] 结束进程
来源：http://spq.fktsv.cn

kill -9 $(pgrep -f app.py)
来源：http://ism.zhaomingkeji.xyz

[R65] 查看端口占用
来源：http://kih.xuanzx.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sdf.wangdashe.top

[R66] 定时任务
来源：http://ycy.xylfe.cn

crontab -e;  crontab -l
来源：http://dpq.xylfe.cn

[R67] 生成随机十六进制串
来源：http://lzx.snrcjt.cn

openssl rand -hex 16
来源：http://uae.jyoumei.cn

[R68] 计算文件校验值
来源：http://pmf.shangyingyoupin.top

sha256sum a.txt;  md5sum a.txt
来源：http://lih.andypj.xyz

[R69] 生成随机密码
来源：http://lrc.zhengqikj.top

head -c 16 /dev/urandom | base64
来源：http://jdq.c1oappe.top

[R70] 时间戳与互转
来源：http://uks.zhijiandao.cn

date +%s;  date -d @1700000000
来源：http://ubx.yj202588.top

[R71] 日期格式化
来源：http://hyk.cashguo.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://wsc.aibaodan.cn

[R72] 等待端口就绪
来源：http://ond.aibaodan.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://iot.vqdsnc.cn

[R73] 分割大日志
来源：http://zqa.jyoumei.cn

split -l 1000 big.log part_
来源：http://hpw.gzhubu.top

[R74] 批量重命名
来源：http://tll.0kj1m.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ids.cashguo.top

[R75] 导出环境变量
来源：http://eps.jyoumei.cn

export PATH="$HOME/bin:$PATH"
来源：http://grc.zycfv.cn

[R76] 使用临时文件
来源：http://iep.sweek.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cap.yj20258.top

[R77] 读取用户输入
来源：http://qyw.hammf.cn

read -rp "请输入: " ans
来源：http://iqx.yonumen.top

[R78] 交互式菜单
来源：http://iwx.dianchejie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gcs.bbcook.cn

[R79] 解析命令行选项
来源：http://dqf.yj20258.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nes.9152youxi.cn

[R80] 查看脚本执行耗时
来源：http://flp.cqqwz.cn

time ./run.sh
来源：http://ikc.jinqigfzy.top

================================================================================
来源：http://apc.wangdashe.top

S. C / C++ 专题
来源：http://mvn.cucudq.cn

================================================================================
来源：http://hnd.hnqzz.top

[S01] C：Hello World
来源：http://yzk.pengpengdd.cyou

#include <stdio.h>
来源：http://ppn.hfpthk.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://wdu.haohaochexian.top

[S02] C：变量与格式化输出
来源：http://cjq.yj202588.top

int a = 10; printf("%d\n", a);
来源：http://rkb.xylfe.cn

[S03] C：读入整数
来源：http://aor.mhx1999.top

int x; scanf("%d", &x);
来源：http://eib.zhoulong.xyz

[S04] C：字符串复制
来源：http://cke.gogol.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://yof.birdmap.top

[S05] C：字符串长度
来源：http://bws.fanxiaobao.xyz

strlen(s)
来源：http://kja.yanxiufei.cn

[S06] C：字符串比较
来源：http://jin.pycfn.com

strcmp(a, b) == 0
来源：http://xvt.yuanzhike.top

[S07] C：数组遍历求和
来源：http://sfz.andypj.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yek.wangshuangyany.cn

[S08] C：动态内存分配与释放
来源：http://fgf.jinqigfzy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bki.shzxlz.cn

[S09] C：结构体定义与初始化
来源：http://onw.epnwcf.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qfx.sysykeji.top

[S10] C：指针与解引用
来源：http://btl.meibo888.top

int *p = &a;  *p = 5;
来源：http://zit.fanxiaobao.xyz

[S11] C：逐行读文件
来源：http://ajg.yangfankeji.com

FILE *f = fopen("a.txt", "r");
来源：http://bmp.ivvv.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://umi.wangdashe.top

fclose(f);
来源：http://ggx.sysykeji.top

[S12] C：写文件
来源：http://ayp.nwbrower.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fke.tian-w.cn

[S13] C：宏定义
来源：http://spg.hongshengwenyu.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lun.sysykeji.top

[S14] C：枚举
来源：http://npw.nanxinkj.top

enum Color { RED, GREEN, BLUE };
来源：http://vmk.cqqwz.cn

[S15] C：类型转换
来源：http://kaj.birdmap.top

(double) a / b
来源：http://bjz.jinqigfzy.top

[S16] C：位操作置位
来源：http://mhh.tian-w.cn

x |= (1 << 3);
来源：http://yip.pycfn.com

[S17] C：安全拼接字符串
来源：http://znq.smart0.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zoq.epnwcf.com

[S18] C：命令行参数
来源：http://vro.fehbvm.com

int main(int argc, char **argv)
来源：http://ywk.andypj.xyz

[S19] C：快速排序
来源：http://vqt.ctjpmb.com

qsort(a, n, sizeof(int), cmp);
来源：http://zjd.jinqigfzy.top

[S20] C：二分查找
来源：http://owe.dashuyun.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vwz.daria6918.cn

[S21] C：字符类别判断
来源：http://usn.daria6918.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lfz.fanxiaobao.xyz

[S22] C：字符串转数字
来源：http://jbf.hnxiangtu.top

atoi("42");  strtod("3.14", NULL);
来源：http://sqd.yj20258.top

[S23] C：随机数
来源：http://phr.pengpengdd.cyou

srand(time(NULL));  int r = rand() % 100;
来源：http://amk.hnqzz.top

[S24] C：获取本地时间
来源：http://skp.ydzc1.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://krn.zhiwuduotai.top

[S25] C：内存拷贝
来源：http://sgy.hesvh.cn

memcpy(dst, src, n);
来源：http://ezl.cucudq.cn

[S26] C：内存清零
来源：http://aby.yj20258888.top

memset(a, 0, sizeof a);
来源：http://xvg.jqgufenzy.top

[S27] C：定义常量
来源：http://yem.smart0.xyz

const double PI = 3.14159;
来源：http://vyo.sjlbkw.cn

[S28] C：静态变量
来源：http://ixt.sjlbkw.cn

static int counter = 0;
来源：http://hgf.guowangkeji.top

[S29] C：变参函数
来源：http://uar.hfpthk.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://poi.zycfv.cn

[S30] C：头文件保护
来源：http://hpv.zhongyouzk.top

#ifndef X_H
来源：http://pav.jinqigfzy.top

#define X_H
来源：http://luh.bbcook.cn

#endif
来源：http://vnv.daria6918.cn

[S31] C++：Hello World
来源：http://rmg.epnwcf.com

#include <iostream>
来源：http://wdm.tanke756.top

int main() { std::cout << "Hello\n"; }
来源：http://zva.aizwys.cn

[S32] C++：字符串
来源：http://ruu.zhongyouzk.top

std::string s = "hi";  s += "!";
来源：http://ktt.quarkkingdee.top

[S33] C++：vector 增删
来源：http://pqj.gotoacloud.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mfg.sxryk.cn

[S34] C++：遍历 vector
来源：http://fhv.sysykeji.top

for (auto &x : v) { std::cout << x; }
来源：http://vsg.quarkkingdee.top

[S35] C++：map
来源：http://wan.zhongyouzk.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mfg.haohaochexian.top

[S36] C++：unordered_map
来源：http://thz.yfazqb.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ill.zhoulong.xyz

[S37] C++：set
来源：http://ztq.jiagoushi.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pyd.wangdashe.top

[S38] C++：排序
来源：http://veq.hcnkem.com

std::sort(v.begin(), v.end());
来源：http://szw.meibo888.top

[S39] C++：自定义比较器排序
来源：http://kyb.shangyingyoupin.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://aod.hywenlv.cn

[S40] C++：查找元素
来源：http://vam.aizwys.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lpo.zhijiandao.cn

[S41] C++：类与构造函数
来源：http://bik.hysaishi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dko.cucudq.cn

[S42] C++：继承与虚函数
来源：http://qoz.bbcook.cn

class B : public Base { public: void f() override {} };
来源：http://klk.gzhubu.top

[S43] C++：智能指针
来源：http://gzl.fzhhl.top

auto p = std::make_unique<int>(5);
来源：http://nrn.yuanzhike.top

[S44] C++：引用传参
来源：http://imy.gogol.net.cn

void inc(int &x) { ++x; }
来源：http://hsh.xuetiantiany.cn

[S45] C++：lambda
来源：http://lyo.birdmap.top

auto add = [](int a, int b) { return a + b; };
来源：http://izs.hammf.cn

[S46] C++：函数模板
来源：http://fkq.zhaomingkeji.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yvm.vehdjk.com

[S47] C++：结构化绑定遍历
来源：http://ncv.bbcook.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cda.jinqigfzy.top

[S48] C++：逐行读文件
来源：http://oln.fanxiaobao.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://sto.andypj.xyz

while (std::getline(in, line)) { }
来源：http://kcz.havefunace.top

[S49] C++：写文件
来源：http://rlz.daria6918.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gga.jinghuilouyu.cn

[S50] C++：格式化数字
来源：http://yfm.xinyue.icu

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rwz.yj202588.top

[S51] C++：显式类型转换
来源：http://nvd.hammf.cn

static_cast<double>(a) / b
来源：http://qiu.hywenlv.cn

[S52] C++：const 与 noexcept
来源：http://mrb.yanxiufei.cn

int size() const noexcept { return n_; }
来源：http://zzg.ydjk.org.cn

[S53] C++：移动语义
来源：http://kjf.shuidangran.top

std::vector<int> w = std::move(v);
来源：http://jxc.hnqzz.top

[S54] C++：异常处理
来源：http://vco.hysaishi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://swn.redwolf501.top

[S55] C++：结构化绑定
来源：http://ppi.iojbl.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rmy.fehbvm.com

[S56] C++：optional
来源：http://vjm.fanxiaobao.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pge.hywenlv.cn

[S57] C++：编译期常量
来源：http://hid.xuetiantiany.cn

constexpr int N = 10;
来源：http://hmd.aizwys.cn

[S58] C++：命名空间
来源：http://buk.kuanghao11.cn

namespace ns { int f() { return 1; } }
来源：http://wyh.zhaomingkeji.xyz

[S59] C++：静态断言
来源：http://ftf.jqgfzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ywp.hnxiangtu.top

[S60] C++：遍历并删除元素
来源：http://ejo.gzhubu.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mia.hnxiangtu.top

================================================================================
来源：http://mrx.zhengqikj.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kbq.hnqzz.top

================================================================================
来源：http://djp.xuetiantiany.cn

[T01] Kotlin：Hello World
来源：http://uja.snrcjt.cn

println("Hello")
来源：http://ojg.ivvv.top

[T02] Kotlin：变量
来源：http://nss.iojbl.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pzw.feifeiyinyue.top

[T03] Kotlin：字符串模板
来源：http://tws.guannengcc.top

"值: $b"
来源：http://pvc.havefunace.top

[T04] Kotlin：空安全
来源：http://maz.tanke756.top

val n: String? = null;  n?.length
来源：http://hsg.xuanzx.com

[T05] Kotlin：when 表达式
来源：http://prz.zycfv.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bna.nwbrower.top

[T06] Kotlin：集合映射
来源：http://ryt.jqgufenzy.top

listOf(1, 2, 3).map { it * 2 }
来源：http://avv.hnxiangtu.top

[T07] Kotlin：集合过滤
来源：http://rev.wangdashe.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://bdk.ydjk.org.cn

[T08] Kotlin：数据类
来源：http://aac.jyoumei.cn

data class User(val name: String, val age: Int)
来源：http://zhh.guowangkeji.top

[T09] Kotlin：扩展函数
来源：http://qfu.9152youxi.cn

fun String.exclaim() = this + "!"
来源：http://ilm.sweek.top

[T10] Kotlin：默认参数
来源：http://njl.shanyushiyangtech.top

fun greet(name: String = "World") = "Hi $name"
来源：http://zpv.pycfn.com

[T11] Kotlin：协程
来源：http://oak.wangshuangyany.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wcr.yvedp.cn

[T12] Kotlin：解构声明
来源：http://xkk.vehdjk.com

val (a, b) = Pair(1, 2)
来源：http://rtu.fengsongda.top

[T13] Kotlin：只读 Map
来源：http://lvc.hesvh.cn

val m = mapOf("a" to 1)
来源：http://alr.ivvv.top

[T14] Kotlin：循环
来源：http://jzf.yueranfly.top

for (i in 1..10) println(i)
来源：http://joa.vqdsnc.cn

[T15] Kotlin：接口
来源：http://zmk.ybcxt.top

interface Shape { fun area(): Double }
来源：http://rsq.nwbrower.top

[T16] Swift：Hello World
来源：http://ixd.jianghu66.top

print("Hello")
来源：http://nkc.zdqjudy.top

[T17] Swift：变量与常量
来源：http://jkc.shangyingyoupin.top

var a = 1;  let b = 2
来源：http://mfa.0kj1m.cn

[T18] Swift：字符串插值
来源：http://myx.snrcjt.cn

"值: \(b)"
来源：http://vap.9152youxi.cn

[T19] Swift：可选绑定
来源：http://kim.ydjk.org.cn

if let n = opt { print(n) }
来源：http://dib.yuanzhike.top

[T20] Swift：数组操作
来源：http://xov.quarkkingdee.top

var a = [1, 2, 3];  a.append(4)
来源：http://gva.jlsjyb.cn


<!-- 参考信息 -->