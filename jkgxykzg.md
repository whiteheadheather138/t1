代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bcx.haohaochexian.top

[R16] until 等待条件
来源：http://hrh.yangfankeji.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nmv.yongpay.top

[R17] 数组定义与取值
来源：http://pau.ybcxt.top

arr=(a b c); echo "${arr[0]}"
来源：http://rhg.haohaochexian.top

[R18] 遍历数组
来源：http://bhb.gogol.net.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://brv.jiagoushi.top

[R19] 数组长度
来源：http://mno.guowangkeji.top

echo "${#arr[@]}"
来源：http://ywb.hammf.cn

[R20] 关联数组（字典）
来源：http://pmj.hesvh.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dfs.mhx1999.top

[R21] 字符串长度
来源：http://fva.quarkkingdee.top

echo "${#s}"
来源：http://lrj.ydzc1.top

[R22] 截取子串
来源：http://rkl.mhx1999.top

echo "${s:0:5}"
来源：http://ptq.ehwqpu.com

[R23] 字符串替换
来源：http://frm.cashguo.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qlv.wangshuangyany.cn

[R24] 大小写转换
来源：http://uve.xingfuxueyuan.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://tkz.shzxlz.cn

[R25] 去后缀 / 去前缀
来源：http://mkh.yongpay.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://sgw.zycfv.cn

[R26] 命令替换
来源：http://ceg.jinyuanbaomall.cn

now=$(date +%F); echo "$now"
来源：http://acb.xuanzx.com

[R27] 算术展开
来源：http://jkg.hnxiangtu.top

echo $((1 + 2 * 3))
来源：http://rpv.yongpay.top

[R28] 浮点运算
来源：http://vfb.nanxinkj.top

echo "scale=2; 10/3" | bc
来源：http://mtt.zycfv.cn

[R29] 定义函数
来源：http://myc.vehdjk.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zda.nanxinkj.top

[R30] 函数返回状态码
来源：http://fpz.aibaodan.cn

f() { return 0; }; f || echo "失败了"
来源：http://rtu.hesvh.cn

[R31] 局部变量
来源：http://lut.xinyue.icu

f() { local x=1; echo "$x"; }
来源：http://mif.aizwys.cn

[R32] 参数个数校验
来源：http://dbk.tian-w.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vvf.hysaishi.cn

[R33] 捕获错误并提示行号
来源：http://tor.snrcjt.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hmp.iojbl.cn

[R34] 退出时清理
来源：http://kkr.tanke756.top

trap 'rm -f "$tmp"' EXIT
来源：http://mfb.jinyuanbaomall.cn

[R35] 后台执行并等待
来源：http://oub.hfpthk.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ctt.wangshuangyany.cn

[R36] 并发执行多个任务
来源：http://hqc.yueranfly.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jsb.chenzaomai.com

[R37] 把输出赋给变量
来源：http://vda.ydzc1.top

files=$(ls -1)
来源：http://ydw.yanxiufei.cn

[R38] 管道串联
来源：http://nod.sweek.top

cat a.txt | grep -i error | wc -l
来源：http://jhr.xylfe.cn

[R39] 重定向标准输出与错误
来源：http://fny.epnwcf.com

cmd > out.log 2>&1
来源：http://ysj.zycfv.cn

[R40] 追加写日志
来源：http://msv.snrcjt.cn

echo "log" >> out.log
来源：http://xib.zhijiandao.cn

[R41] 丢弃输出
来源：http://htm.svipenyu.cn

cmd >/dev/null 2>&1
来源：http://igl.jinghuilouyu.cn

[R42] 输入重定向
来源：http://vrk.zycfv.cn

wc -l < a.txt
来源：http://jad.ybcxt.top

[R43] 按名字查找文件
来源：http://ngb.vehdjk.com

find . -name "*.log" -type f
来源：http://zpu.tianlin.xyz

[R44] 按修改时间查找
来源：http://qub.cheryme.top

find . -mtime -7 -type f
来源：http://kch.ydzc1.top

[R45] 批量删除
来源：http://tvg.xinyue.icu

find . -name "*.tmp" -delete
来源：http://uoc.mhx1999.top

[R46] 递归替换文件内容
来源：http://snk.vehdjk.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cdk.uphjek.com

[R47] sed 单行替换
来源：http://uma.quarkkingdee.top

sed -i 's/foo/bar/g' a.txt
来源：http://pdn.tanke756.top

[R48] awk 取指定列
来源：http://lnm.tarul.cn

awk '{print $1, $3}' a.txt
来源：http://jrd.xinyue.icu

[R49] awk 带条件
来源：http://qqj.guowangkeji.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mhm.dashuyun.cn

[R50] awk 求和
来源：http://uww.ywan-chungtsiang.top

awk '{s += $2} END {print s}' a.txt
来源：http://ctn.haohaochexian.top

[R51] 排序去重取前几
来源：http://nsy.yanxiufei.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://tpw.ivvv.top

[R52] 统计行数
来源：http://jps.jqgfzy.top

wc -l a.txt
来源：http://amw.vehdjk.com

[R53] 查看文件头与实时尾
来源：http://dzg.316326.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ayk.dianchejie.cn

[R54] 比较两个文件
来源：http://oql.dianchejie.cn

diff a.txt b.txt
来源：http://lnm.ehwqpu.com

[R55] 压缩与解压
来源：http://wsc.jiagoushi.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tma.meibo888.top

[R56] 远程拷贝
来源：http://nqz.jinghuilouyu.cn

scp file user@host:/path/
来源：http://eva.yanxiufei.cn

[R57] 远程执行命令
来源：http://qdt.ywan-chungtsiang.top

ssh user@host 'uptime'
来源：http://ohg.fengsongda.top

[R58] 下载文件
来源：http://tvw.sxryk.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rlg.xuetiantiany.cn

[R59] 发 POST JSON
来源：http://hiq.pycfn.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ope.yanxiufei.cn

[R60] 只看 HTTP 状态码
来源：http://set.jinyuanbaomall.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gnt.yj202588.top

[R61] 磁盘占用
来源：http://ugc.zhongyouzk.top

df -h;  du -sh *
来源：http://ylo.yvedp.cn

[R62] 找最占空间的文件
来源：http://boh.uphjek.com

du -ah . | sort -rh | head -10
来源：http://mht.hesvh.cn

[R63] 内存与进程
来源：http://gyc.jinqigfzy.top

free -h;  ps aux | grep nginx
来源：http://jna.hcnkem.com

[R64] 结束进程
来源：http://zvy.hywenlv.cn

kill -9 $(pgrep -f app.py)
来源：http://oiy.pycfn.com

[R65] 查看端口占用
来源：http://bwm.ybcxt.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pzd.bbcook.cn

[R66] 定时任务
来源：http://kcc.fanxiaobao.xyz

crontab -e;  crontab -l
来源：http://ehb.cheryme.top

[R67] 生成随机十六进制串
来源：http://tyw.316326.xyz

openssl rand -hex 16
来源：http://jkz.chenlongwang.top

[R68] 计算文件校验值
来源：http://slj.tarul.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ioo.yuxming.cn

[R69] 生成随机密码
来源：http://nfl.cheryme.top

head -c 16 /dev/urandom | base64
来源：http://qga.zdqjudy.top

[R70] 时间戳与互转
来源：http://ert.ywan-chungtsiang.top

date +%s;  date -d @1700000000
来源：http://emr.yfazqb.com

[R71] 日期格式化
来源：http://unb.xuanzx.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://gvi.bjfxy.top

[R72] 等待端口就绪
来源：http://iqc.yuxming.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xhf.vqdsnc.cn

[R73] 分割大日志
来源：http://wbn.xuanzx.com

split -l 1000 big.log part_
来源：http://tcu.shzxlz.cn

[R74] 批量重命名
来源：http://iuc.yfazqb.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kuy.xziqi.cn

[R75] 导出环境变量
来源：http://awr.jqgufenzy.top

export PATH="$HOME/bin:$PATH"
来源：http://gue.jianghu66.top

[R76] 使用临时文件
来源：http://buw.zdbjq.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bmq.ivvv.top

[R77] 读取用户输入
来源：http://udb.aibaodan.cn

read -rp "请输入: " ans
来源：http://nsi.yvedp.cn

[R78] 交互式菜单
来源：http://exd.gotoacloud.top

select opt in a b c; do echo "$opt"; break; done
来源：http://vcx.cashguo.top

[R79] 解析命令行选项
来源：http://gbi.xylfe.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sja.fehbvm.com

[R80] 查看脚本执行耗时
来源：http://yfb.0kj1m.cn

time ./run.sh
来源：http://uqw.zhiwuduotai.top

================================================================================
来源：http://lhr.nanxuanxn.top

S. C / C++ 专题
来源：http://mhk.ivvv.top

================================================================================
来源：http://yvv.9152youxi.cn

[S01] C：Hello World
来源：http://ztf.chenlongwang.top

#include <stdio.h>
来源：http://cvc.vehdjk.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://tuq.xuetiantiany.cn

[S02] C：变量与格式化输出
来源：http://ith.mhx1999.top

int a = 10; printf("%d\n", a);
来源：http://imd.guannengcc.top

[S03] C：读入整数
来源：http://rpn.jinyuanbaomall.cn

int x; scanf("%d", &x);
来源：http://cnb.jqgufenzy.top

[S04] C：字符串复制
来源：http://ort.tian-w.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ytk.nanxuanxn.top

[S05] C：字符串长度
来源：http://gxf.zhiwuduotai.top

strlen(s)
来源：http://esa.mhx1999.top

[S06] C：字符串比较
来源：http://trk.zhoulong.xyz

strcmp(a, b) == 0
来源：http://brr.shanyushiyangtech.top

[S07] C：数组遍历求和
来源：http://hlo.redwolf501.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tno.gaohongyu789.top

[S08] C：动态内存分配与释放
来源：http://rhs.chenjidiqi.icu

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qlv.sweek.top

[S09] C：结构体定义与初始化
来源：http://eov.gotoacloud.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hso.dashuyun.cn

[S10] C：指针与解引用
来源：http://npd.svipenyu.cn

int *p = &a;  *p = 5;
来源：http://hhm.hammf.cn

[S11] C：逐行读文件
来源：http://hfc.yvedp.cn

FILE *f = fopen("a.txt", "r");
来源：http://dgf.tanke756.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://hlm.zhengqikj.top

fclose(f);
来源：http://fcc.zhoulong.xyz

[S12] C：写文件
来源：http://vxi.zhongyouzk.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cdx.shuidangran.top

[S13] C：宏定义
来源：http://pry.yvedp.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kcv.yangfankeji.com

[S14] C：枚举
来源：http://jnq.tianlin.xyz

enum Color { RED, GREEN, BLUE };
来源：http://abd.smart0.xyz

[S15] C：类型转换
来源：http://kic.yangfankeji.com

(double) a / b
来源：http://dau.fengsongda.top

[S16] C：位操作置位
来源：http://ckp.gotoacloud.top

x |= (1 << 3);
来源：http://uco.yangfankeji.com

[S17] C：安全拼接字符串
来源：http://evh.hnxiangtu.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wvc.hongshengwenyu.top

[S18] C：命令行参数
来源：http://ejk.vehdjk.com

int main(int argc, char **argv)
来源：http://agf.uphjek.com

[S19] C：快速排序
来源：http://dqt.hnqzz.top

qsort(a, n, sizeof(int), cmp);
来源：http://kxc.xingfuxueyuan.xyz

[S20] C：二分查找
来源：http://wak.bbcook.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mvn.zhijiandao.cn

[S21] C：字符类别判断
来源：http://gaz.yueranfly.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ngv.pycfn.com

[S22] C：字符串转数字
来源：http://wej.aizwys.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wob.yanxiufei.cn

[S23] C：随机数
来源：http://okh.aizwys.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://pip.yj20258888.top

[S24] C：获取本地时间
来源：http://apt.aizwys.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mra.mhx1999.top

[S25] C：内存拷贝
来源：http://zwj.andypj.xyz

memcpy(dst, src, n);
来源：http://pps.jqgufenzy.top

[S26] C：内存清零
来源：http://gpa.gotoacloud.top

memset(a, 0, sizeof a);
来源：http://pih.hfpthk.cn

[S27] C：定义常量
来源：http://ezo.tianlin.xyz

const double PI = 3.14159;
来源：http://hxq.jqgufenzy.top

[S28] C：静态变量
来源：http://peu.shanyushiyangtech.top

static int counter = 0;
来源：http://lkq.fktsv.cn

[S29] C：变参函数
来源：http://iql.shuidangran.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dcm.nanxinkj.top

[S30] C：头文件保护
来源：http://hxg.wangdashe.top

#ifndef X_H
来源：http://asa.feifeiyinyue.top

#define X_H
来源：http://phu.uphjek.com

#endif
来源：http://kmd.quarkkingdee.top

[S31] C++：Hello World
来源：http://bqm.sysykeji.top

#include <iostream>
来源：http://rwv.chenzaomai.com

int main() { std::cout << "Hello\n"; }
来源：http://khh.yanxiufei.cn

[S32] C++：字符串
来源：http://lwy.chenjidiqi.icu

std::string s = "hi";  s += "!";
来源：http://wfj.jinqigufen.top

[S33] C++：vector 增删
来源：http://zcg.gotoacloud.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gig.iojbl.cn

[S34] C++：遍历 vector
来源：http://ycn.hnxiangtu.top

for (auto &x : v) { std::cout << x; }
来源：http://lst.iojbl.cn

[S35] C++：map
来源：http://ifo.nwbrower.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ekj.hcnkem.com

[S36] C++：unordered_map
来源：http://mpo.xingfuxueyuan.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://owa.sjlbkw.cn

[S37] C++：set
来源：http://tba.sjlbkw.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yjv.ehwqpu.com

[S38] C++：排序
来源：http://wdz.dashuyun.cn

std::sort(v.begin(), v.end());
来源：http://kra.zdqjudy.top

[S39] C++：自定义比较器排序
来源：http://nul.aibaodan.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://heh.ctjpmb.com

[S40] C++：查找元素
来源：http://gic.daxiang520.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://eiy.zhiwuduotai.top

[S41] C++：类与构造函数
来源：http://brl.gotoacloud.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kok.quarkkingdee.top

[S42] C++：继承与虚函数
来源：http://bwl.daxiang520.top

class B : public Base { public: void f() override {} };
来源：http://beu.sufxvd.cn

[S43] C++：智能指针
来源：http://kdx.redwolf501.top

auto p = std::make_unique<int>(5);
来源：http://uia.chenlongwang.top

[S44] C++：引用传参
来源：http://ecz.yangfankeji.com

void inc(int &x) { ++x; }
来源：http://put.tanke756.top

[S45] C++：lambda
来源：http://dcg.hfpthk.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bnf.yuxming.cn

[S46] C++：函数模板
来源：http://rol.dashuyun.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wew.chenlongwang.top

[S47] C++：结构化绑定遍历
来源：http://opo.yongpay.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://noy.fanxiaobao.xyz

[S48] C++：逐行读文件
来源：http://eua.guowangkeji.top

std::ifstream in("a.txt");  std::string line;
来源：http://uqp.zhijiandao.cn

while (std::getline(in, line)) { }
来源：http://oly.tian-w.cn

[S49] C++：写文件
来源：http://evf.yj20258888.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rrh.nanxuanxn.top

[S50] C++：格式化数字
来源：http://lnn.ehwqpu.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dbk.uphjek.com

[S51] C++：显式类型转换
来源：http://unq.fanxiaobao.xyz

static_cast<double>(a) / b
来源：http://dgz.gotoacloud.top

[S52] C++：const 与 noexcept
来源：http://tbq.nwbrower.top

int size() const noexcept { return n_; }
来源：http://mij.xuanzx.com

[S53] C++：移动语义
来源：http://yxt.tarul.cn

std::vector<int> w = std::move(v);
来源：http://dpl.yfazqb.com

[S54] C++：异常处理
来源：http://jhs.jinqigufen.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kof.birdmap.top

[S55] C++：结构化绑定
来源：http://biq.zdbjq.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ekg.jqgufenzy.top

[S56] C++：optional
来源：http://ekn.smart0.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xzx.vehdjk.com

[S57] C++：编译期常量
来源：http://xkw.yongpay.top

constexpr int N = 10;
来源：http://xdk.xingfuxueyuan.xyz

[S58] C++：命名空间
来源：http://tvl.yongpay.top

namespace ns { int f() { return 1; } }
来源：http://nwz.ppjwa.cn

[S59] C++：静态断言
来源：http://sdw.tanke756.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ioy.gotoacloud.top

[S60] C++：遍历并删除元素
来源：http://mqo.zhoulong.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xya.52xcode.cn

================================================================================
来源：http://okt.cucudq.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nmv.redwolf501.top

================================================================================
来源：http://xdo.dianchejie.cn

[T01] Kotlin：Hello World
来源：http://ceo.zhaomingkeji.xyz

println("Hello")
来源：http://fxt.chenzaomai.com

[T02] Kotlin：变量
来源：http://chj.nwbrower.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://djw.zhongyouzk.top

[T03] Kotlin：字符串模板
来源：http://zvf.smart0.xyz

"值: $b"
来源：http://zzd.daxiang520.top

[T04] Kotlin：空安全
来源：http://tft.yj202588.top

val n: String? = null;  n?.length
来源：http://udv.jinghuilouyu.cn

[T05] Kotlin：when 表达式
来源：http://dvf.nwbrower.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sgw.9152youxi.cn

[T06] Kotlin：集合映射
来源：http://vys.xuanzx.com

listOf(1, 2, 3).map { it * 2 }
来源：http://usm.pengpengdd.cyou

[T07] Kotlin：集合过滤
来源：http://nmu.nwbrower.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://dip.jinyuanbaomall.cn

[T08] Kotlin：数据类
来源：http://umf.hywenlv.cn

data class User(val name: String, val age: Int)
来源：http://vmh.bjfxy.top

[T09] Kotlin：扩展函数
来源：http://ucz.zhiwuduotai.top

fun String.exclaim() = this + "!"
来源：http://zir.shuidangran.top

[T10] Kotlin：默认参数
来源：http://xck.iojbl.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ult.yongpay.top

[T11] Kotlin：协程
来源：http://fty.aibaodan.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://poh.aibaodan.cn

[T12] Kotlin：解构声明
来源：http://rfh.nanxuanxn.top

val (a, b) = Pair(1, 2)
来源：http://acb.chenjidiqi.icu

[T13] Kotlin：只读 Map
来源：http://szg.hywenlv.cn

val m = mapOf("a" to 1)
来源：http://ojc.yuxming.cn

[T14] Kotlin：循环
来源：http://tpc.yangfankeji.com

for (i in 1..10) println(i)
来源：http://nwi.shzxlz.cn

[T15] Kotlin：接口
来源：http://mvp.havefunace.top

interface Shape { fun area(): Double }
来源：http://rmw.iojbl.cn

[T16] Swift：Hello World
来源：http://amx.52xcode.cn

print("Hello")
来源：http://geh.ydjk.org.cn

[T17] Swift：变量与常量
来源：http://ccv.chenlongwang.top

var a = 1;  let b = 2
来源：http://jgj.hongshengwenyu.top

[T18] Swift：字符串插值
来源：http://dev.jinghuilouyu.cn

"值: \(b)"
来源：http://dtw.zhijiandao.cn


<!-- 参考信息 -->