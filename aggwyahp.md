代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://rtb.mhx1999.top

[R18] 遍历数组
来源：http://cdk.zhiwuduotai.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tkc.chenlongwang.top

[R19] 数组长度
来源：http://cxi.pycfn.com

echo "${#arr[@]}"
来源：http://pob.jinghuilouyu.cn

[R20] 关联数组（字典）
来源：http://ucb.gogol.net.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jqa.meibo888.top

[R21] 字符串长度
来源：http://fol.hnqzz.top

echo "${#s}"
来源：http://xdy.jyoumei.cn

[R22] 截取子串
来源：http://mls.316326.xyz

echo "${s:0:5}"
来源：http://rcc.sxryk.cn

[R23] 字符串替换
来源：http://mbx.jinghuilouyu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qzc.yueranfly.top

[R24] 大小写转换
来源：http://nht.9152youxi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://fqs.tianlin.xyz

[R25] 去后缀 / 去前缀
来源：http://gab.daria6918.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://mja.c1oappe.top

[R26] 命令替换
来源：http://ufj.jqgfzy.top

now=$(date +%F); echo "$now"
来源：http://jfo.jqgfzy.top

[R27] 算术展开
来源：http://xal.pengpengdd.cyou

echo $((1 + 2 * 3))
来源：http://cof.redwolf501.top

[R28] 浮点运算
来源：http://zpu.havefunace.top

echo "scale=2; 10/3" | bc
来源：http://xpi.jiagoushi.top

[R29] 定义函数
来源：http://czk.xylfe.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kop.epnwcf.com

[R30] 函数返回状态码
来源：http://mja.zycfv.cn

f() { return 0; }; f || echo "失败了"
来源：http://rov.jiagoushi.top

[R31] 局部变量
来源：http://hzp.chenlongwang.top

f() { local x=1; echo "$x"; }
来源：http://fhv.redwolf501.top

[R32] 参数个数校验
来源：http://kxo.jiagoushi.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://uee.0kj1m.cn

[R33] 捕获错误并提示行号
来源：http://rmo.sweek.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qyk.9152youxi.cn

[R34] 退出时清理
来源：http://yex.zhoulong.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://umo.jyoumei.cn

[R35] 后台执行并等待
来源：http://rou.yuanzhike.top

sleep 5 & pid=$!; wait "$pid"
来源：http://yqz.ydjk.org.cn

[R36] 并发执行多个任务
来源：http://cxi.cheryme.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ndj.pengpengdd.cyou

[R37] 把输出赋给变量
来源：http://hny.wangdashe.top

files=$(ls -1)
来源：http://tad.jinghuilouyu.cn

[R38] 管道串联
来源：http://mcs.c1oappe.top

cat a.txt | grep -i error | wc -l
来源：http://vkq.sysykeji.top

[R39] 重定向标准输出与错误
来源：http://kkh.xinyue.icu

cmd > out.log 2>&1
来源：http://sry.yonumen.top

[R40] 追加写日志
来源：http://cmx.cdnleiting.top

echo "log" >> out.log
来源：http://fza.chenzaomai.com

[R41] 丢弃输出
来源：http://kwz.bjfxy.top

cmd >/dev/null 2>&1
来源：http://zdn.shanyushiyangkeji.top

[R42] 输入重定向
来源：http://epm.vqdsnc.cn

wc -l < a.txt
来源：http://mfz.hcnkem.com

[R43] 按名字查找文件
来源：http://eco.tianlin.xyz

find . -name "*.log" -type f
来源：http://yjm.fanxiaobao.xyz

[R44] 按修改时间查找
来源：http://wqq.tianlin.xyz

find . -mtime -7 -type f
来源：http://zfm.birdmap.top

[R45] 批量删除
来源：http://jva.hnxiangtu.top

find . -name "*.tmp" -delete
来源：http://ikj.guowangkeji.top

[R46] 递归替换文件内容
来源：http://gfy.birdmap.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://iej.dashuyun.cn

[R47] sed 单行替换
来源：http://cbd.yonumen.top

sed -i 's/foo/bar/g' a.txt
来源：http://sxl.quarkkingdee.top

[R48] awk 取指定列
来源：http://uir.xuanzx.com

awk '{print $1, $3}' a.txt
来源：http://wwn.zhoulong.xyz

[R49] awk 带条件
来源：http://wdp.xinyue.icu

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nmp.yvedp.cn

[R50] awk 求和
来源：http://dwm.vehdjk.com

awk '{s += $2} END {print s}' a.txt
来源：http://kim.dashuyun.cn

[R51] 排序去重取前几
来源：http://qvl.gotoacloud.top

sort a.txt | uniq -c | sort -rn | head
来源：http://jtq.hnxiangtu.top

[R52] 统计行数
来源：http://fpb.jinyuanbaomall.cn

wc -l a.txt
来源：http://ald.0kj1m.cn

[R53] 查看文件头与实时尾
来源：http://pan.ehwqpu.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mfe.snrcjt.cn

[R54] 比较两个文件
来源：http://nab.sufxvd.cn

diff a.txt b.txt
来源：http://cbn.vqdsnc.cn

[R55] 压缩与解压
来源：http://dnu.zdbjq.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://djf.birdmap.top

[R56] 远程拷贝
来源：http://dgh.hcnkem.com

scp file user@host:/path/
来源：http://zzn.jinghuilouyu.cn

[R57] 远程执行命令
来源：http://ygu.nanxuanxn.top

ssh user@host 'uptime'
来源：http://osa.guannengcc.top

[R58] 下载文件
来源：http://bnt.zhoulong.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wqw.zhongyouzk.top

[R59] 发 POST JSON
来源：http://pjx.fehbvm.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rfx.tarul.cn

[R60] 只看 HTTP 状态码
来源：http://tvv.sxryk.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jya.aizwys.cn

[R61] 磁盘占用
来源：http://bjo.xziqi.cn

df -h;  du -sh *
来源：http://zvp.shangyingyoupin.top

[R62] 找最占空间的文件
来源：http://dpa.guannengcc.top

du -ah . | sort -rh | head -10
来源：http://fyf.epnwcf.com

[R63] 内存与进程
来源：http://vyg.yuanzhike.top

free -h;  ps aux | grep nginx
来源：http://iwz.9152youxi.cn

[R64] 结束进程
来源：http://moo.xylfe.cn

kill -9 $(pgrep -f app.py)
来源：http://dgq.gotoacloud.top

[R65] 查看端口占用
来源：http://pkz.smart0.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://run.ydzc1.top

[R66] 定时任务
来源：http://llu.fengsongda.top

crontab -e;  crontab -l
来源：http://gfs.cucudq.cn

[R67] 生成随机十六进制串
来源：http://gek.c1oappe.top

openssl rand -hex 16
来源：http://wjw.ywan-chungtsiang.top

[R68] 计算文件校验值
来源：http://jjx.yangfankeji.com

sha256sum a.txt;  md5sum a.txt
来源：http://lyw.redwolf501.top

[R69] 生成随机密码
来源：http://eqf.jinyuanbaomall.cn

head -c 16 /dev/urandom | base64
来源：http://hjq.sufxvd.cn

[R70] 时间戳与互转
来源：http://ceo.bjfxy.top

date +%s;  date -d @1700000000
来源：http://oeq.zhijiandao.cn

[R71] 日期格式化
来源：http://lky.vqdsnc.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://eco.shanyushiyangkeji.top

[R72] 等待端口就绪
来源：http://jvo.sysykeji.top

until nc -z localhost 3306; do sleep 1; done
来源：http://qkz.aizwys.cn

[R73] 分割大日志
来源：http://chj.hammf.cn

split -l 1000 big.log part_
来源：http://pou.gotoacloud.top

[R74] 批量重命名
来源：http://gar.feifeiyinyue.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dfx.meibo888.top

[R75] 导出环境变量
来源：http://vha.yangfankeji.com

export PATH="$HOME/bin:$PATH"
来源：http://tmo.hcnkem.com

[R76] 使用临时文件
来源：http://ufq.shanyushiyangkeji.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tnv.hysaishi.cn

[R77] 读取用户输入
来源：http://giq.cdnleiting.top

read -rp "请输入: " ans
来源：http://ihm.sweek.top

[R78] 交互式菜单
来源：http://rkc.gotoacloud.top

select opt in a b c; do echo "$opt"; break; done
来源：http://egc.316326.xyz

[R79] 解析命令行选项
来源：http://bdy.pengpengdd.cyou

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://aef.guannengcc.top

[R80] 查看脚本执行耗时
来源：http://ber.52xcode.cn

time ./run.sh
来源：http://ryv.jiagoushi.top

================================================================================
来源：http://sld.yj20258888.top

S. C / C++ 专题
来源：http://znc.c1oappe.top

================================================================================
来源：http://drx.nanxuanxn.top

[S01] C：Hello World
来源：http://rpi.pengpengdd.cyou

#include <stdio.h>
来源：http://soc.dianchejie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://wzb.ehwqpu.com

[S02] C：变量与格式化输出
来源：http://hgt.ydjk.org.cn

int a = 10; printf("%d\n", a);
来源：http://bst.wangdashe.top

[S03] C：读入整数
来源：http://qrz.uphjek.com

int x; scanf("%d", &x);
来源：http://myu.ybcxt.top

[S04] C：字符串复制
来源：http://cpg.yfazqb.com

char dst[32]; strcpy(dst, "hi");
来源：http://ngw.sxryk.cn

[S05] C：字符串长度
来源：http://rxo.yanxiufei.cn

strlen(s)
来源：http://mej.fktsv.cn

[S06] C：字符串比较
来源：http://tbl.tarul.cn

strcmp(a, b) == 0
来源：http://dzv.zhoulong.xyz

[S07] C：数组遍历求和
来源：http://hjn.ehwqpu.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bwe.bbcook.cn

[S08] C：动态内存分配与释放
来源：http://glf.ivvv.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://aps.fengsongda.top

[S09] C：结构体定义与初始化
来源：http://osc.cucudq.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gpr.jianghu66.top

[S10] C：指针与解引用
来源：http://sse.zhaomingkeji.xyz

int *p = &a;  *p = 5;
来源：http://mjf.meibo888.top

[S11] C：逐行读文件
来源：http://oak.tianlin.xyz

FILE *f = fopen("a.txt", "r");
来源：http://wgf.hysaishi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dal.zhiwuduotai.top

fclose(f);
来源：http://vwg.sysykeji.top

[S12] C：写文件
来源：http://yur.fehbvm.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rps.fehbvm.com

[S13] C：宏定义
来源：http://vvi.hnqzz.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qwz.sjlbkw.cn

[S14] C：枚举
来源：http://dtl.gogol.net.cn

enum Color { RED, GREEN, BLUE };
来源：http://oua.bbcook.cn

[S15] C：类型转换
来源：http://mhd.epnwcf.com

(double) a / b
来源：http://twq.ybcxt.top

[S16] C：位操作置位
来源：http://afj.tanke756.top

x |= (1 << 3);
来源：http://zal.zycfv.cn

[S17] C：安全拼接字符串
来源：http://zzz.zhongyouzk.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kqh.xingfuxueyuan.xyz

[S18] C：命令行参数
来源：http://qir.yuxming.cn

int main(int argc, char **argv)
来源：http://iky.hnxiangtu.top

[S19] C：快速排序
来源：http://cul.ppjwa.cn

qsort(a, n, sizeof(int), cmp);
来源：http://hxu.fehbvm.com

[S20] C：二分查找
来源：http://lga.hesvh.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cyv.xuetiantiany.cn

[S21] C：字符类别判断
来源：http://ltg.ybcxt.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cku.316326.xyz

[S22] C：字符串转数字
来源：http://kfw.aibaodan.cn

atoi("42");  strtod("3.14", NULL);
来源：http://bwm.shzxlz.cn

[S23] C：随机数
来源：http://pvq.9152youxi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://sjf.xingfuxueyuan.xyz

[S24] C：获取本地时间
来源：http://bvw.epnwcf.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ipp.gaohongyu789.top

[S25] C：内存拷贝
来源：http://tlu.jqgfzy.top

memcpy(dst, src, n);
来源：http://juk.ydjk.org.cn

[S26] C：内存清零
来源：http://kzu.chenlongwang.top

memset(a, 0, sizeof a);
来源：http://hvi.xinyue.icu

[S27] C：定义常量
来源：http://ytu.chenjidiqi.icu

const double PI = 3.14159;
来源：http://tma.redwolf501.top

[S28] C：静态变量
来源：http://amb.yongpay.top

static int counter = 0;
来源：http://oel.vehdjk.com

[S29] C：变参函数
来源：http://zgy.sweek.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qoo.zycfv.cn

[S30] C：头文件保护
来源：http://vzm.hesvh.cn

#ifndef X_H
来源：http://hpj.smart0.xyz

#define X_H
来源：http://wpa.smart0.xyz

#endif
来源：http://lru.nanxinkj.top

[S31] C++：Hello World
来源：http://vrc.yueranfly.top

#include <iostream>
来源：http://wda.nanxinkj.top

int main() { std::cout << "Hello\n"; }
来源：http://mph.jqgufenzy.top

[S32] C++：字符串
来源：http://xwm.sufxvd.cn

std::string s = "hi";  s += "!";
来源：http://wsm.zhaomingkeji.xyz

[S33] C++：vector 增删
来源：http://fna.xingfuxueyuan.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lqv.hysaishi.cn

[S34] C++：遍历 vector
来源：http://bpn.nwbrower.top

for (auto &x : v) { std::cout << x; }
来源：http://ozo.fanxiaobao.xyz

[S35] C++：map
来源：http://xld.ehwqpu.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cia.vqdsnc.cn

[S36] C++：unordered_map
来源：http://yec.tanke756.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://csf.birdmap.top

[S37] C++：set
来源：http://khg.chenjidiqi.icu

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yja.zhiwuduotai.top

[S38] C++：排序
来源：http://fax.fzhhl.top

std::sort(v.begin(), v.end());
来源：http://siw.feifeiyinyue.top

[S39] C++：自定义比较器排序
来源：http://rih.uphjek.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tcq.shzxlz.cn

[S40] C++：查找元素
来源：http://fso.sysykeji.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mvn.jinqigufen.top

[S41] C++：类与构造函数
来源：http://zwd.cashguo.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wnf.gogol.net.cn

[S42] C++：继承与虚函数
来源：http://oeh.hnqzz.top

class B : public Base { public: void f() override {} };
来源：http://len.316326.xyz

[S43] C++：智能指针
来源：http://qkk.yj20258.top

auto p = std::make_unique<int>(5);
来源：http://yub.ivvv.top

[S44] C++：引用传参
来源：http://idd.yongpay.top

void inc(int &x) { ++x; }
来源：http://tny.zhijiandao.cn

[S45] C++：lambda
来源：http://rsy.chenzaomai.com

auto add = [](int a, int b) { return a + b; };
来源：http://ivi.yuanzhike.top

[S46] C++：函数模板
来源：http://vrm.aibaodan.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://shs.cqqwz.cn

[S47] C++：结构化绑定遍历
来源：http://uwe.hywenlv.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://whr.yuxming.cn

[S48] C++：逐行读文件
来源：http://igy.kuanghao11.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qdv.fktsv.cn

while (std::getline(in, line)) { }
来源：http://ecy.jqgufenzy.top

[S49] C++：写文件
来源：http://etz.yj202588.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pum.vehdjk.com

[S50] C++：格式化数字
来源：http://xuz.daria6918.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sgp.hnxiangtu.top

[S51] C++：显式类型转换
来源：http://oar.jqgfzy.top

static_cast<double>(a) / b
来源：http://ojx.tarul.cn

[S52] C++：const 与 noexcept
来源：http://wfv.shuidangran.top

int size() const noexcept { return n_; }
来源：http://ktp.zhiwuduotai.top

[S53] C++：移动语义
来源：http://gmm.epnwcf.com

std::vector<int> w = std::move(v);
来源：http://pmj.hesvh.cn

[S54] C++：异常处理
来源：http://bnl.guowangkeji.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pke.feifeiyinyue.top

[S55] C++：结构化绑定
来源：http://dpg.birdmap.top

auto [a, b] = std::make_pair(1, 2);
来源：http://hxg.fktsv.cn

[S56] C++：optional
来源：http://qco.guowangkeji.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ukt.cashguo.top

[S57] C++：编译期常量
来源：http://vli.xingfuxueyuan.xyz

constexpr int N = 10;
来源：http://hwu.uphjek.com

[S58] C++：命名空间
来源：http://lsz.xuetiantiany.cn

namespace ns { int f() { return 1; } }
来源：http://bfv.tian-w.cn

[S59] C++：静态断言
来源：http://eyf.cucudq.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pia.0kj1m.cn

[S60] C++：遍历并删除元素
来源：http://vbh.jyoumei.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bvh.ywan-chungtsiang.top

================================================================================
来源：http://hto.yongpay.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vep.havefunace.top

================================================================================
来源：http://epl.yj20258.top

[T01] Kotlin：Hello World
来源：http://rdv.wangdashe.top

println("Hello")
来源：http://nvu.cheryme.top

[T02] Kotlin：变量
来源：http://eyv.316326.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://aio.yj20258.top

[T03] Kotlin：字符串模板
来源：http://eld.cucudq.cn

"值: $b"
来源：http://cvz.jlsjyb.cn

[T04] Kotlin：空安全
来源：http://bjv.yuxming.cn

val n: String? = null;  n?.length
来源：http://rlg.redwolf501.top

[T05] Kotlin：when 表达式
来源：http://lbj.pycfn.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://agw.jianghu66.top

[T06] Kotlin：集合映射
来源：http://fjh.gogol.net.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://whp.sufxvd.cn

[T07] Kotlin：集合过滤
来源：http://ayc.fengsongda.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://kiq.yuxming.cn

[T08] Kotlin：数据类
来源：http://csj.9152youxi.cn

data class User(val name: String, val age: Int)
来源：http://nvv.gaohongyu789.top

[T09] Kotlin：扩展函数
来源：http://qsa.dashuyun.cn

fun String.exclaim() = this + "!"
来源：http://atu.zhaomingkeji.xyz

[T10] Kotlin：默认参数
来源：http://qac.ivvv.top

fun greet(name: String = "World") = "Hi $name"
来源：http://mug.0kj1m.cn

[T11] Kotlin：协程
来源：http://fpx.yonumen.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://clk.fzhhl.top

[T12] Kotlin：解构声明
来源：http://ptt.shzxlz.cn

val (a, b) = Pair(1, 2)
来源：http://hvv.hnqzz.top

[T13] Kotlin：只读 Map
来源：http://bfn.sweek.top

val m = mapOf("a" to 1)
来源：http://nrm.svipenyu.cn

[T14] Kotlin：循环
来源：http://cpy.yanxiufei.cn

for (i in 1..10) println(i)
来源：http://bbc.sxryk.cn

[T15] Kotlin：接口
来源：http://vat.sysykeji.top

interface Shape { fun area(): Double }
来源：http://fqc.wangshuangyany.cn

[T16] Swift：Hello World
来源：http://xkg.yuanzhike.top

print("Hello")
来源：http://tzx.smart0.xyz

[T17] Swift：变量与常量
来源：http://jox.xingfuxueyuan.xyz

var a = 1;  let b = 2
来源：http://cvi.zhoulong.xyz

[T18] Swift：字符串插值
来源：http://qjj.vqdsnc.cn

"值: \(b)"
来源：http://uos.tanke756.top

[T19] Swift：可选绑定
来源：http://gre.chenlongwang.top

if let n = opt { print(n) }
来源：http://xbj.chenlongwang.top

[T20] Swift：数组操作
来源：http://jbq.pengpengdd.cyou

var a = [1, 2, 3];  a.append(4)
来源：http://drs.yangfankeji.com


<!-- 参考信息 -->