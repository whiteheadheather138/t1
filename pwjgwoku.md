代发 wailian999

esac
来源：http://wuq.xuetiantiany.cn

[R12] for 遍历文件
来源：http://chy.sysykeji.top

for f in *.txt; do echo "$f"; done
来源：http://eoz.0kj1m.cn

[R13] for 计数循环
来源：http://rfy.yj20258.top

for i in {1..10}; do echo "$i"; done
来源：http://jjz.quarkkingdee.top

[R14] C 风格 for
来源：http://khc.svipenyu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gln.fanxiaobao.xyz

[R15] while 逐行读文件
来源：http://chu.feifeiyinyue.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cji.zhoulong.xyz

[R16] until 等待条件
来源：http://xrc.ywan-chungtsiang.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://buy.hywenlv.cn

[R17] 数组定义与取值
来源：http://tuq.sufxvd.cn

arr=(a b c); echo "${arr[0]}"
来源：http://utr.zhixingplan.top

[R18] 遍历数组
来源：http://eli.316326.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nse.iojbl.cn

[R19] 数组长度
来源：http://vdr.zhongyouzk.top

echo "${#arr[@]}"
来源：http://hqm.uphjek.com

[R20] 关联数组（字典）
来源：http://ogi.dashuyun.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hqq.yueranfly.top

[R21] 字符串长度
来源：http://ftk.yonumen.top

echo "${#s}"
来源：http://xdt.zhengqikj.top

[R22] 截取子串
来源：http://jqc.jlsjyb.cn

echo "${s:0:5}"
来源：http://dmp.yvedp.cn

[R23] 字符串替换
来源：http://xxg.birdmap.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dmp.316326.xyz

[R24] 大小写转换
来源：http://vsa.sysykeji.top

echo "${s^^}"; echo "${s,,}"
来源：http://cox.yuanzhike.top

[R25] 去后缀 / 去前缀
来源：http://ajo.feifeiyinyue.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://abr.zhaomingkeji.xyz

[R26] 命令替换
来源：http://zms.shangyingyoupin.top

now=$(date +%F); echo "$now"
来源：http://zsj.jyoumei.cn

[R27] 算术展开
来源：http://arh.hnqzz.top

echo $((1 + 2 * 3))
来源：http://odt.yj20258888.top

[R28] 浮点运算
来源：http://bki.yongpay.top

echo "scale=2; 10/3" | bc
来源：http://ltr.epnwcf.com

[R29] 定义函数
来源：http://ukz.hysaishi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ndl.zhixingplan.top

[R30] 函数返回状态码
来源：http://anq.jqgfzy.top

f() { return 0; }; f || echo "失败了"
来源：http://zvr.wangshuangyany.cn

[R31] 局部变量
来源：http://yyo.ehwqpu.com

f() { local x=1; echo "$x"; }
来源：http://hqe.zhengqikj.top

[R32] 参数个数校验
来源：http://poi.shangyingyoupin.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wuy.hesvh.cn

[R33] 捕获错误并提示行号
来源：http://pbr.hesvh.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://oca.fanxiaobao.xyz

[R34] 退出时清理
来源：http://ysu.yanxiufei.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qwe.ybcxt.top

[R35] 后台执行并等待
来源：http://osy.316326.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://klg.yanxiufei.cn

[R36] 并发执行多个任务
来源：http://uhq.sufxvd.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pvj.xuanzx.com

[R37] 把输出赋给变量
来源：http://gcg.tarul.cn

files=$(ls -1)
来源：http://iap.cqqwz.cn

[R38] 管道串联
来源：http://yyb.zdbjq.cn

cat a.txt | grep -i error | wc -l
来源：http://dvf.feifeiyinyue.top

[R39] 重定向标准输出与错误
来源：http://xgf.c1oappe.top

cmd > out.log 2>&1
来源：http://hgm.yanxiufei.cn

[R40] 追加写日志
来源：http://wgp.zhixingplan.top

echo "log" >> out.log
来源：http://gni.yuanzhike.top

[R41] 丢弃输出
来源：http://qqo.gogol.net.cn

cmd >/dev/null 2>&1
来源：http://oex.dashuyun.cn

[R42] 输入重定向
来源：http://wtx.yongpay.top

wc -l < a.txt
来源：http://vur.hysaishi.cn

[R43] 按名字查找文件
来源：http://nmo.epnwcf.com

find . -name "*.log" -type f
来源：http://fyo.yj202588.top

[R44] 按修改时间查找
来源：http://wdg.hongshengwenyu.top

find . -mtime -7 -type f
来源：http://cxk.daria6918.cn

[R45] 批量删除
来源：http://uqb.sjlbkw.cn

find . -name "*.tmp" -delete
来源：http://qyu.bjfxy.top

[R46] 递归替换文件内容
来源：http://nwx.shuidangran.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://csg.ivvv.top

[R47] sed 单行替换
来源：http://xkz.iojbl.cn

sed -i 's/foo/bar/g' a.txt
来源：http://uju.jinghuilouyu.cn

[R48] awk 取指定列
来源：http://swj.yvedp.cn

awk '{print $1, $3}' a.txt
来源：http://xly.tian-w.cn

[R49] awk 带条件
来源：http://bzj.xziqi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://maw.havefunace.top

[R50] awk 求和
来源：http://weg.gogol.net.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fsi.yj20258888.top

[R51] 排序去重取前几
来源：http://ept.jianghu66.top

sort a.txt | uniq -c | sort -rn | head
来源：http://dyl.fehbvm.com

[R52] 统计行数
来源：http://lbz.sjlbkw.cn

wc -l a.txt
来源：http://uev.zhengqikj.top

[R53] 查看文件头与实时尾
来源：http://mxs.guowangkeji.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xtg.xziqi.cn

[R54] 比较两个文件
来源：http://abo.52xcode.cn

diff a.txt b.txt
来源：http://zcl.xuetiantiany.cn

[R55] 压缩与解压
来源：http://lhq.redwolf501.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lwx.gotoacloud.top

[R56] 远程拷贝
来源：http://utv.pycfn.com

scp file user@host:/path/
来源：http://htm.tanke756.top

[R57] 远程执行命令
来源：http://fnb.feifeiyinyue.top

ssh user@host 'uptime'
来源：http://bia.ivvv.top

[R58] 下载文件
来源：http://isq.hongshengwenyu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gpa.ywan-chungtsiang.top

[R59] 发 POST JSON
来源：http://isp.yongpay.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zpn.dianchejie.cn

[R60] 只看 HTTP 状态码
来源：http://uod.yj20258888.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xxo.cashguo.top

[R61] 磁盘占用
来源：http://kjr.aizwys.cn

df -h;  du -sh *
来源：http://ozl.hcnkem.com

[R62] 找最占空间的文件
来源：http://gxk.zhijiandao.cn

du -ah . | sort -rh | head -10
来源：http://prv.fktsv.cn

[R63] 内存与进程
来源：http://vsl.guowangkeji.top

free -h;  ps aux | grep nginx
来源：http://rwh.shanyushiyangtech.top

[R64] 结束进程
来源：http://aub.cheryme.top

kill -9 $(pgrep -f app.py)
来源：http://zdr.cashguo.top

[R65] 查看端口占用
来源：http://vmz.aibaodan.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ice.jqgfzy.top

[R66] 定时任务
来源：http://ieb.jyoumei.cn

crontab -e;  crontab -l
来源：http://czt.cashguo.top

[R67] 生成随机十六进制串
来源：http://ytm.pycfn.com

openssl rand -hex 16
来源：http://ajz.zhengqikj.top

[R68] 计算文件校验值
来源：http://hej.svipenyu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://num.hywenlv.cn

[R69] 生成随机密码
来源：http://xtw.chenjidiqi.icu

head -c 16 /dev/urandom | base64
来源：http://ymi.jianghu66.top

[R70] 时间戳与互转
来源：http://vcp.gotoacloud.top

date +%s;  date -d @1700000000
来源：http://svd.smart0.xyz

[R71] 日期格式化
来源：http://qud.hnqzz.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://eph.tian-w.cn

[R72] 等待端口就绪
来源：http://xkv.daria6918.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://tzm.vqdsnc.cn

[R73] 分割大日志
来源：http://bcf.epnwcf.com

split -l 1000 big.log part_
来源：http://fth.gaohongyu789.top

[R74] 批量重命名
来源：http://fnw.zhijiandao.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vxh.yj20258.top

[R75] 导出环境变量
来源：http://vkp.fehbvm.com

export PATH="$HOME/bin:$PATH"
来源：http://qul.iojbl.cn

[R76] 使用临时文件
来源：http://red.sysykeji.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tkl.kuanghao11.cn

[R77] 读取用户输入
来源：http://whj.jinyuanbaomall.cn

read -rp "请输入: " ans
来源：http://sow.gogol.net.cn

[R78] 交互式菜单
来源：http://gns.yanxiufei.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tfy.hnqzz.top

[R79] 解析命令行选项
来源：http://jmz.jinqigfzy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tht.yangfankeji.com

[R80] 查看脚本执行耗时
来源：http://jxi.vqdsnc.cn

time ./run.sh
来源：http://uhc.chenlongwang.top

================================================================================
来源：http://jbf.hcnkem.com

S. C / C++ 专题
来源：http://lhe.cheryme.top

================================================================================
来源：http://ezc.sjlbkw.cn

[S01] C：Hello World
来源：http://mvh.sweek.top

#include <stdio.h>
来源：http://iog.chenzaomai.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://vqo.tianlin.xyz

[S02] C：变量与格式化输出
来源：http://cil.xziqi.cn

int a = 10; printf("%d\n", a);
来源：http://rlc.xuanzx.com

[S03] C：读入整数
来源：http://nuk.jinqigufen.top

int x; scanf("%d", &x);
来源：http://eud.chenlongwang.top

[S04] C：字符串复制
来源：http://ueo.zhengqikj.top

char dst[32]; strcpy(dst, "hi");
来源：http://jtm.yj20258888.top

[S05] C：字符串长度
来源：http://bni.bjfxy.top

strlen(s)
来源：http://kjl.jinqigufen.top

[S06] C：字符串比较
来源：http://ixb.ywan-chungtsiang.top

strcmp(a, b) == 0
来源：http://nww.hfpthk.cn

[S07] C：数组遍历求和
来源：http://edq.zdbjq.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tla.fehbvm.com

[S08] C：动态内存分配与释放
来源：http://aio.0kj1m.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mct.guowangkeji.top

[S09] C：结构体定义与初始化
来源：http://lmw.yueranfly.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hob.cdnleiting.top

[S10] C：指针与解引用
来源：http://yjf.sufxvd.cn

int *p = &a;  *p = 5;
来源：http://pen.xuetiantiany.cn

[S11] C：逐行读文件
来源：http://mcx.chenlongwang.top

FILE *f = fopen("a.txt", "r");
来源：http://jfi.yueranfly.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://vqm.bbcook.cn

fclose(f);
来源：http://klf.yj202588.top

[S12] C：写文件
来源：http://rqk.0kj1m.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vhj.meibo888.top

[S13] C：宏定义
来源：http://wii.zhoulong.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kve.birdmap.top

[S14] C：枚举
来源：http://xsw.haohaochexian.top

enum Color { RED, GREEN, BLUE };
来源：http://dvb.yueranfly.top

[S15] C：类型转换
来源：http://nfw.gzhubu.top

(double) a / b
来源：http://ont.havefunace.top

[S16] C：位操作置位
来源：http://ung.hammf.cn

x |= (1 << 3);
来源：http://qkr.ppjwa.cn

[S17] C：安全拼接字符串
来源：http://nwm.chenjidiqi.icu

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fag.52xcode.cn

[S18] C：命令行参数
来源：http://mrx.guannengcc.top

int main(int argc, char **argv)
来源：http://xet.c1oappe.top

[S19] C：快速排序
来源：http://mqg.52xcode.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jnd.svipenyu.cn

[S20] C：二分查找
来源：http://ckd.hcnkem.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pdp.epnwcf.com

[S21] C：字符类别判断
来源：http://enn.zycfv.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://esp.hongshengwenyu.top

[S22] C：字符串转数字
来源：http://xnp.zdqjudy.top

atoi("42");  strtod("3.14", NULL);
来源：http://jws.hesvh.cn

[S23] C：随机数
来源：http://gdu.9152youxi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://jit.xinyue.icu

[S24] C：获取本地时间
来源：http://oiy.yvedp.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sen.316326.xyz

[S25] C：内存拷贝
来源：http://jhn.kuanghao11.cn

memcpy(dst, src, n);
来源：http://rxu.guannengcc.top

[S26] C：内存清零
来源：http://czg.ppjwa.cn

memset(a, 0, sizeof a);
来源：http://ddv.andypj.xyz

[S27] C：定义常量
来源：http://yfp.andypj.xyz

const double PI = 3.14159;
来源：http://pcm.nwbrower.top

[S28] C：静态变量
来源：http://gwm.jinyuanbaomall.cn

static int counter = 0;
来源：http://daj.daxiang520.top

[S29] C：变参函数
来源：http://rmq.dianchejie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ncp.fanxiaobao.xyz

[S30] C：头文件保护
来源：http://jum.sufxvd.cn

#ifndef X_H
来源：http://gyh.dianchejie.cn

#define X_H
来源：http://img.dianchejie.cn

#endif
来源：http://ezz.xuetiantiany.cn

[S31] C++：Hello World
来源：http://muj.9152youxi.cn

#include <iostream>
来源：http://hhd.feifeiyinyue.top

int main() { std::cout << "Hello\n"; }
来源：http://zeq.jinyuanbaomall.cn

[S32] C++：字符串
来源：http://erk.hongshengwenyu.top

std::string s = "hi";  s += "!";
来源：http://hog.jinqigufen.top

[S33] C++：vector 增删
来源：http://xhp.vehdjk.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kgi.xingfuxueyuan.xyz

[S34] C++：遍历 vector
来源：http://wit.daria6918.cn

for (auto &x : v) { std::cout << x; }
来源：http://gek.quarkkingdee.top

[S35] C++：map
来源：http://phe.svipenyu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://krd.tianlin.xyz

[S36] C++：unordered_map
来源：http://sjb.svipenyu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://awk.yfazqb.com

[S37] C++：set
来源：http://psj.epnwcf.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mia.hcnkem.com

[S38] C++：排序
来源：http://xvj.chenzaomai.com

std::sort(v.begin(), v.end());
来源：http://qdc.hnqzz.top

[S39] C++：自定义比较器排序
来源：http://sar.sysykeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vvp.gotoacloud.top

[S40] C++：查找元素
来源：http://uwj.uphjek.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ced.meibo888.top

[S41] C++：类与构造函数
来源：http://yxf.nwbrower.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wqx.cashguo.top

[S42] C++：继承与虚函数
来源：http://cgv.jinghuilouyu.cn

class B : public Base { public: void f() override {} };
来源：http://ynl.xuanzx.com

[S43] C++：智能指针
来源：http://fyi.zhaomingkeji.xyz

auto p = std::make_unique<int>(5);
来源：http://zqq.zdqjudy.top

[S44] C++：引用传参
来源：http://lsa.nanxinkj.top

void inc(int &x) { ++x; }
来源：http://fqd.jinqigfzy.top

[S45] C++：lambda
来源：http://qsw.snrcjt.cn

auto add = [](int a, int b) { return a + b; };
来源：http://mly.fengsongda.top

[S46] C++：函数模板
来源：http://gkv.meibo888.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bdp.zdqjudy.top

[S47] C++：结构化绑定遍历
来源：http://xkq.zhongyouzk.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ton.tianlin.xyz

[S48] C++：逐行读文件
来源：http://tcp.pycfn.com

std::ifstream in("a.txt");  std::string line;
来源：http://bxe.ivvv.top

while (std::getline(in, line)) { }
来源：http://xls.jinqigufen.top

[S49] C++：写文件
来源：http://kup.yuanzhike.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://riv.0kj1m.cn

[S50] C++：格式化数字
来源：http://wrk.zycfv.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ckn.cqqwz.cn

[S51] C++：显式类型转换
来源：http://rov.shanyushiyangkeji.top

static_cast<double>(a) / b
来源：http://wrv.hcnkem.com

[S52] C++：const 与 noexcept
来源：http://skj.sxryk.cn

int size() const noexcept { return n_; }
来源：http://wrm.gogol.net.cn

[S53] C++：移动语义
来源：http://ald.guannengcc.top

std::vector<int> w = std::move(v);
来源：http://jov.zhaomingkeji.xyz

[S54] C++：异常处理
来源：http://tib.yfazqb.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bsj.jlsjyb.cn

[S55] C++：结构化绑定
来源：http://twa.gogol.net.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ets.yj20258888.top

[S56] C++：optional
来源：http://nvx.pycfn.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://eur.chenzaomai.com

[S57] C++：编译期常量
来源：http://bqi.shzxlz.cn

constexpr int N = 10;
来源：http://wyl.shangyingyoupin.top

[S58] C++：命名空间
来源：http://pxn.yongpay.top

namespace ns { int f() { return 1; } }
来源：http://qkl.daxiang520.top

[S59] C++：静态断言
来源：http://gzr.jinqigufen.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vuy.redwolf501.top

[S60] C++：遍历并删除元素
来源：http://hax.svipenyu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dem.daria6918.cn

================================================================================
来源：http://wzq.wangshuangyany.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bgn.xingfuxueyuan.xyz

================================================================================
来源：http://bxt.jyoumei.cn

[T01] Kotlin：Hello World
来源：http://pnn.jqgufenzy.top

println("Hello")
来源：http://eks.redwolf501.top

[T02] Kotlin：变量
来源：http://xnr.vqdsnc.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://epe.yuanzhike.top

[T03] Kotlin：字符串模板
来源：http://bin.quarkkingdee.top

"值: $b"
来源：http://bjb.9152youxi.cn

[T04] Kotlin：空安全
来源：http://icw.tarul.cn

val n: String? = null;  n?.length
来源：http://dui.jiagoushi.top

[T05] Kotlin：when 表达式
来源：http://qhe.jinghuilouyu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ugc.nwbrower.top

[T06] Kotlin：集合映射
来源：http://cxk.gaohongyu789.top

listOf(1, 2, 3).map { it * 2 }
来源：http://hfh.0kj1m.cn

[T07] Kotlin：集合过滤
来源：http://qha.jiagoushi.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ctg.quarkkingdee.top

[T08] Kotlin：数据类
来源：http://rdh.jianghu66.top

data class User(val name: String, val age: Int)
来源：http://ufd.ydjk.org.cn

[T09] Kotlin：扩展函数
来源：http://lez.cashguo.top

fun String.exclaim() = this + "!"
来源：http://hmz.aizwys.cn

[T10] Kotlin：默认参数
来源：http://rfz.cqqwz.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ado.daria6918.cn

[T11] Kotlin：协程
来源：http://qay.shangyingyoupin.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://yef.dashuyun.cn

[T12] Kotlin：解构声明
来源：http://dsd.guannengcc.top

val (a, b) = Pair(1, 2)
来源：http://bev.xingfuxueyuan.xyz

[T13] Kotlin：只读 Map
来源：http://jpa.fengsongda.top

val m = mapOf("a" to 1)
来源：http://slg.shuidangran.top

[T14] Kotlin：循环
来源：http://tca.ydjk.org.cn

for (i in 1..10) println(i)
来源：http://guc.aizwys.cn


<!-- 参考信息 -->