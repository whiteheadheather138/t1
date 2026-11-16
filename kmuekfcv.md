代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mub.hywenlv.cn

[R10] 正则匹配
来源：http://bvq.zhixingplan.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://urr.fktsv.cn

[R11] case 多分支
来源：http://vbc.yonumen.top

case "$1" in
来源：http://wrd.cucudq.cn

start) echo "启动" ;;
来源：http://wnk.fanxiaobao.xyz

stop)  echo "停止" ;;
来源：http://dht.xingfuxueyuan.xyz

*)     echo "未知命令" ;;
来源：http://aqb.ydjk.org.cn

esac
来源：http://sga.gogol.net.cn

[R12] for 遍历文件
来源：http://doj.sxryk.cn

for f in *.txt; do echo "$f"; done
来源：http://rxe.zycfv.cn

[R13] for 计数循环
来源：http://edx.zhaomingkeji.xyz

for i in {1..10}; do echo "$i"; done
来源：http://xnq.shzxlz.cn

[R14] C 风格 for
来源：http://ier.smart0.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://eun.wangdashe.top

[R15] while 逐行读文件
来源：http://ccz.vehdjk.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yet.guowangkeji.top

[R16] until 等待条件
来源：http://ilx.dashuyun.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bwk.ivvv.top

[R17] 数组定义与取值
来源：http://hmk.svipenyu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://acm.fzhhl.top

[R18] 遍历数组
来源：http://cjc.zhijiandao.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kkh.hammf.cn

[R19] 数组长度
来源：http://gua.fehbvm.com

echo "${#arr[@]}"
来源：http://lpj.guannengcc.top

[R20] 关联数组（字典）
来源：http://diz.fanxiaobao.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zzi.iojbl.cn

[R21] 字符串长度
来源：http://afb.aizwys.cn

echo "${#s}"
来源：http://zuf.hongshengwenyu.top

[R22] 截取子串
来源：http://tji.hammf.cn

echo "${s:0:5}"
来源：http://kfp.ydzc1.top

[R23] 字符串替换
来源：http://nhg.xuetiantiany.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ccb.fktsv.cn

[R24] 大小写转换
来源：http://bmd.bbcook.cn

echo "${s^^}"; echo "${s,,}"
来源：http://cjx.sysykeji.top

[R25] 去后缀 / 去前缀
来源：http://swv.zhaomingkeji.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://urv.cashguo.top

[R26] 命令替换
来源：http://nhw.chenjidiqi.icu

now=$(date +%F); echo "$now"
来源：http://hen.kuanghao11.cn

[R27] 算术展开
来源：http://uhq.nwbrower.top

echo $((1 + 2 * 3))
来源：http://ebx.xziqi.cn

[R28] 浮点运算
来源：http://jdj.xylfe.cn

echo "scale=2; 10/3" | bc
来源：http://dld.mhx1999.top

[R29] 定义函数
来源：http://lma.aizwys.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dhc.52xcode.cn

[R30] 函数返回状态码
来源：http://dxi.hesvh.cn

f() { return 0; }; f || echo "失败了"
来源：http://lph.fehbvm.com

[R31] 局部变量
来源：http://toa.uphjek.com

f() { local x=1; echo "$x"; }
来源：http://rze.zhongyouzk.top

[R32] 参数个数校验
来源：http://gij.fehbvm.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pwn.zhiwuduotai.top

[R33] 捕获错误并提示行号
来源：http://wwu.havefunace.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tba.jiagoushi.top

[R34] 退出时清理
来源：http://lsk.birdmap.top

trap 'rm -f "$tmp"' EXIT
来源：http://hhd.dashuyun.cn

[R35] 后台执行并等待
来源：http://tpd.shzxlz.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gmj.tarul.cn

[R36] 并发执行多个任务
来源：http://ytk.fengsongda.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ypa.xziqi.cn

[R37] 把输出赋给变量
来源：http://qvl.iojbl.cn

files=$(ls -1)
来源：http://cot.zycfv.cn

[R38] 管道串联
来源：http://fhg.gogol.net.cn

cat a.txt | grep -i error | wc -l
来源：http://jnw.zhongyouzk.top

[R39] 重定向标准输出与错误
来源：http://zxb.hammf.cn

cmd > out.log 2>&1
来源：http://mdt.hammf.cn

[R40] 追加写日志
来源：http://oft.c1oappe.top

echo "log" >> out.log
来源：http://mnb.guannengcc.top

[R41] 丢弃输出
来源：http://lsg.hnqzz.top

cmd >/dev/null 2>&1
来源：http://zld.jiagoushi.top

[R42] 输入重定向
来源：http://ati.yanxiufei.cn

wc -l < a.txt
来源：http://vzg.zhijiandao.cn

[R43] 按名字查找文件
来源：http://wzn.yuanzhike.top

find . -name "*.log" -type f
来源：http://ksh.9152youxi.cn

[R44] 按修改时间查找
来源：http://tmx.mhx1999.top

find . -mtime -7 -type f
来源：http://auk.zhoulong.xyz

[R45] 批量删除
来源：http://riw.zhoulong.xyz

find . -name "*.tmp" -delete
来源：http://gye.uphjek.com

[R46] 递归替换文件内容
来源：http://mkd.andypj.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://trx.nanxuanxn.top

[R47] sed 单行替换
来源：http://zlr.gaohongyu789.top

sed -i 's/foo/bar/g' a.txt
来源：http://jpb.aizwys.cn

[R48] awk 取指定列
来源：http://drd.dashuyun.cn

awk '{print $1, $3}' a.txt
来源：http://fcy.meibo888.top

[R49] awk 带条件
来源：http://esl.sweek.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bbr.sxryk.cn

[R50] awk 求和
来源：http://hgg.birdmap.top

awk '{s += $2} END {print s}' a.txt
来源：http://wty.redwolf501.top

[R51] 排序去重取前几
来源：http://uyc.snrcjt.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://sqa.fanxiaobao.xyz

[R52] 统计行数
来源：http://mqc.andypj.xyz

wc -l a.txt
来源：http://fiz.ctjpmb.com

[R53] 查看文件头与实时尾
来源：http://ovl.snrcjt.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ubw.feifeiyinyue.top

[R54] 比较两个文件
来源：http://egx.cqqwz.cn

diff a.txt b.txt
来源：http://iet.chenlongwang.top

[R55] 压缩与解压
来源：http://egb.tanke756.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xpl.cdnleiting.top

[R56] 远程拷贝
来源：http://lbu.wangdashe.top

scp file user@host:/path/
来源：http://alw.snrcjt.cn

[R57] 远程执行命令
来源：http://lto.quarkkingdee.top

ssh user@host 'uptime'
来源：http://dyu.vqdsnc.cn

[R58] 下载文件
来源：http://yuw.zhaomingkeji.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nfl.dianchejie.cn

[R59] 发 POST JSON
来源：http://vuk.shanyushiyangtech.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dir.hfpthk.cn

[R60] 只看 HTTP 状态码
来源：http://enh.shangyingyoupin.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://txi.pengpengdd.cyou

[R61] 磁盘占用
来源：http://haa.zdqjudy.top

df -h;  du -sh *
来源：http://zno.pengpengdd.cyou

[R62] 找最占空间的文件
来源：http://qrw.redwolf501.top

du -ah . | sort -rh | head -10
来源：http://otn.aibaodan.cn

[R63] 内存与进程
来源：http://zqg.yj20258888.top

free -h;  ps aux | grep nginx
来源：http://jpd.jqgfzy.top

[R64] 结束进程
来源：http://zjz.jinqigfzy.top

kill -9 $(pgrep -f app.py)
来源：http://bqi.mhx1999.top

[R65] 查看端口占用
来源：http://esc.nwbrower.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uap.yongpay.top

[R66] 定时任务
来源：http://fqa.316326.xyz

crontab -e;  crontab -l
来源：http://ipm.chenlongwang.top

[R67] 生成随机十六进制串
来源：http://roy.yueranfly.top

openssl rand -hex 16
来源：http://hob.gaohongyu789.top

[R68] 计算文件校验值
来源：http://dns.gzhubu.top

sha256sum a.txt;  md5sum a.txt
来源：http://fll.yonumen.top

[R69] 生成随机密码
来源：http://rgc.quarkkingdee.top

head -c 16 /dev/urandom | base64
来源：http://ljs.316326.xyz

[R70] 时间戳与互转
来源：http://cay.jqgufenzy.top

date +%s;  date -d @1700000000
来源：http://hqv.aibaodan.cn

[R71] 日期格式化
来源：http://qkj.andypj.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://faf.zhoulong.xyz

[R72] 等待端口就绪
来源：http://sce.yj20258.top

until nc -z localhost 3306; do sleep 1; done
来源：http://kiz.kuanghao11.cn

[R73] 分割大日志
来源：http://fld.aibaodan.cn

split -l 1000 big.log part_
来源：http://hmq.cashguo.top

[R74] 批量重命名
来源：http://dvi.hcnkem.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://eny.ctjpmb.com

[R75] 导出环境变量
来源：http://dbl.fehbvm.com

export PATH="$HOME/bin:$PATH"
来源：http://bpx.hcnkem.com

[R76] 使用临时文件
来源：http://xhq.tianlin.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gru.yuxming.cn

[R77] 读取用户输入
来源：http://vvw.gogol.net.cn

read -rp "请输入: " ans
来源：http://krz.316326.xyz

[R78] 交互式菜单
来源：http://uyf.haohaochexian.top

select opt in a b c; do echo "$opt"; break; done
来源：http://jwd.tarul.cn

[R79] 解析命令行选项
来源：http://bpx.vqdsnc.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bcp.bbcook.cn

[R80] 查看脚本执行耗时
来源：http://akh.hywenlv.cn

time ./run.sh
来源：http://kir.52xcode.cn

================================================================================
来源：http://mqs.feifeiyinyue.top

S. C / C++ 专题
来源：http://eir.yongpay.top

================================================================================
来源：http://pzo.redwolf501.top

[S01] C：Hello World
来源：http://pxz.fengsongda.top

#include <stdio.h>
来源：http://rsp.ydjk.org.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://tth.jyoumei.cn

[S02] C：变量与格式化输出
来源：http://hqt.sweek.top

int a = 10; printf("%d\n", a);
来源：http://ufm.jinqigufen.top

[S03] C：读入整数
来源：http://opi.chenlongwang.top

int x; scanf("%d", &x);
来源：http://vwf.yj202588.top

[S04] C：字符串复制
来源：http://sfd.xingfuxueyuan.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://wln.chenjidiqi.icu

[S05] C：字符串长度
来源：http://jka.zhijiandao.cn

strlen(s)
来源：http://ykg.yueranfly.top

[S06] C：字符串比较
来源：http://woc.yj20258888.top

strcmp(a, b) == 0
来源：http://vzp.zycfv.cn

[S07] C：数组遍历求和
来源：http://zyj.svipenyu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uuz.yj202588.top

[S08] C：动态内存分配与释放
来源：http://neb.havefunace.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hzk.andypj.xyz

[S09] C：结构体定义与初始化
来源：http://hdq.andypj.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bxk.52xcode.cn

[S10] C：指针与解引用
来源：http://kio.meibo888.top

int *p = &a;  *p = 5;
来源：http://jyr.tianlin.xyz

[S11] C：逐行读文件
来源：http://wnl.xuanzx.com

FILE *f = fopen("a.txt", "r");
来源：http://vco.gotoacloud.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://cnn.xinyue.icu

fclose(f);
来源：http://amr.sysykeji.top

[S12] C：写文件
来源：http://pkr.hesvh.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vql.ctjpmb.com

[S13] C：宏定义
来源：http://hkr.ydjk.org.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dgo.jinghuilouyu.cn

[S14] C：枚举
来源：http://iiz.aizwys.cn

enum Color { RED, GREEN, BLUE };
来源：http://ked.ywan-chungtsiang.top

[S15] C：类型转换
来源：http://csm.yuxming.cn

(double) a / b
来源：http://poa.daria6918.cn

[S16] C：位操作置位
来源：http://ghs.dashuyun.cn

x |= (1 << 3);
来源：http://lqz.zhijiandao.cn

[S17] C：安全拼接字符串
来源：http://sek.cheryme.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lba.gzhubu.top

[S18] C：命令行参数
来源：http://vox.daria6918.cn

int main(int argc, char **argv)
来源：http://ccw.shanyushiyangtech.top

[S19] C：快速排序
来源：http://bye.xingfuxueyuan.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://lmx.cucudq.cn

[S20] C：二分查找
来源：http://qdw.svipenyu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://eub.guannengcc.top

[S21] C：字符类别判断
来源：http://syo.pycfn.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://scy.chenlongwang.top

[S22] C：字符串转数字
来源：http://qty.yongpay.top

atoi("42");  strtod("3.14", NULL);
来源：http://uol.shuidangran.top

[S23] C：随机数
来源：http://kol.shangyingyoupin.top

srand(time(NULL));  int r = rand() % 100;
来源：http://blw.jinqigfzy.top

[S24] C：获取本地时间
来源：http://iph.zhoulong.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dzz.wangdashe.top

[S25] C：内存拷贝
来源：http://tif.bbcook.cn

memcpy(dst, src, n);
来源：http://pgg.9152youxi.cn

[S26] C：内存清零
来源：http://nuu.zhiwuduotai.top

memset(a, 0, sizeof a);
来源：http://qze.guowangkeji.top

[S27] C：定义常量
来源：http://ema.smart0.xyz

const double PI = 3.14159;
来源：http://juc.birdmap.top

[S28] C：静态变量
来源：http://yeg.hcnkem.com

static int counter = 0;
来源：http://xoo.316326.xyz

[S29] C：变参函数
来源：http://xdf.yj202588.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gip.svipenyu.cn

[S30] C：头文件保护
来源：http://efi.tianlin.xyz

#ifndef X_H
来源：http://cfi.xingfuxueyuan.xyz

#define X_H
来源：http://tsi.pengpengdd.cyou

#endif
来源：http://ioj.jinqigfzy.top

[S31] C++：Hello World
来源：http://dfk.fengsongda.top

#include <iostream>
来源：http://ovt.jqgfzy.top

int main() { std::cout << "Hello\n"; }
来源：http://spn.shangyingyoupin.top

[S32] C++：字符串
来源：http://ggs.yonumen.top

std::string s = "hi";  s += "!";
来源：http://kxe.tanke756.top

[S33] C++：vector 增删
来源：http://dql.cqqwz.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nnj.cdnleiting.top

[S34] C++：遍历 vector
来源：http://jys.ydjk.org.cn

for (auto &x : v) { std::cout << x; }
来源：http://qeq.yonumen.top

[S35] C++：map
来源：http://jej.ctjpmb.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lcl.daxiang520.top

[S36] C++：unordered_map
来源：http://rln.zdqjudy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://egs.guannengcc.top

[S37] C++：set
来源：http://veq.yuxming.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hdg.jyoumei.cn

[S38] C++：排序
来源：http://lly.hysaishi.cn

std::sort(v.begin(), v.end());
来源：http://mmh.sxryk.cn

[S39] C++：自定义比较器排序
来源：http://lgu.cucudq.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://reu.uphjek.com

[S40] C++：查找元素
来源：http://nhv.zhiwuduotai.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pyi.feifeiyinyue.top

[S41] C++：类与构造函数
来源：http://cyk.sxryk.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tlc.zdqjudy.top

[S42] C++：继承与虚函数
来源：http://gag.gogol.net.cn

class B : public Base { public: void f() override {} };
来源：http://leu.zhijiandao.cn

[S43] C++：智能指针
来源：http://oxf.bjfxy.top

auto p = std::make_unique<int>(5);
来源：http://ohb.hongshengwenyu.top

[S44] C++：引用传参
来源：http://qhg.ivvv.top

void inc(int &x) { ++x; }
来源：http://htc.zdqjudy.top

[S45] C++：lambda
来源：http://ipu.tian-w.cn

auto add = [](int a, int b) { return a + b; };
来源：http://mic.yanxiufei.cn

[S46] C++：函数模板
来源：http://bfe.mhx1999.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://onu.andypj.xyz

[S47] C++：结构化绑定遍历
来源：http://vtr.cucudq.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sjf.xylfe.cn

[S48] C++：逐行读文件
来源：http://fdg.xuetiantiany.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vop.cashguo.top

while (std::getline(in, line)) { }
来源：http://lhy.vehdjk.com

[S49] C++：写文件
来源：http://hpy.yj20258888.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://oco.yj20258888.top

[S50] C++：格式化数字
来源：http://upj.yj20258888.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qjf.zhixingplan.top

[S51] C++：显式类型转换
来源：http://ziv.yvedp.cn

static_cast<double>(a) / b
来源：http://evl.dashuyun.cn

[S52] C++：const 与 noexcept
来源：http://dzy.tarul.cn

int size() const noexcept { return n_; }
来源：http://ied.quarkkingdee.top

[S53] C++：移动语义
来源：http://qjl.xziqi.cn

std::vector<int> w = std::move(v);
来源：http://ptc.yanxiufei.cn

[S54] C++：异常处理
来源：http://hly.hfpthk.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bgs.gogol.net.cn

[S55] C++：结构化绑定
来源：http://cyg.haohaochexian.top

auto [a, b] = std::make_pair(1, 2);
来源：http://rsy.gotoacloud.top

[S56] C++：optional
来源：http://gtb.zhiwuduotai.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lfg.feifeiyinyue.top

[S57] C++：编译期常量
来源：http://uqe.aizwys.cn

constexpr int N = 10;
来源：http://fav.sufxvd.cn

[S58] C++：命名空间
来源：http://drf.yonumen.top

namespace ns { int f() { return 1; } }
来源：http://vsx.xinyue.icu

[S59] C++：静态断言
来源：http://lpy.ivvv.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://trg.zdqjudy.top

[S60] C++：遍历并删除元素
来源：http://upe.hywenlv.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bcu.vqdsnc.cn

================================================================================
来源：http://mgq.jinqigfzy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qaq.hongshengwenyu.top

================================================================================
来源：http://ile.uphjek.com

[T01] Kotlin：Hello World
来源：http://ftc.epnwcf.com

println("Hello")
来源：http://dff.sysykeji.top

[T02] Kotlin：变量
来源：http://sfw.zhengqikj.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xga.shuidangran.top

[T03] Kotlin：字符串模板
来源：http://fsq.jqgufenzy.top

"值: $b"
来源：http://fbm.jianghu66.top

[T04] Kotlin：空安全
来源：http://fuo.0kj1m.cn

val n: String? = null;  n?.length
来源：http://mnv.jinqigfzy.top

[T05] Kotlin：when 表达式
来源：http://lrr.shzxlz.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lof.hywenlv.cn

[T06] Kotlin：集合映射
来源：http://kwn.zhengqikj.top

listOf(1, 2, 3).map { it * 2 }
来源：http://qnn.uphjek.com

[T07] Kotlin：集合过滤
来源：http://wcg.shanyushiyangkeji.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://bhs.cdnleiting.top

[T08] Kotlin：数据类
来源：http://hhy.jinyuanbaomall.cn

data class User(val name: String, val age: Int)
来源：http://zia.jiagoushi.top

[T09] Kotlin：扩展函数
来源：http://adp.cqqwz.cn

fun String.exclaim() = this + "!"
来源：http://nxv.shangyingyoupin.top

[T10] Kotlin：默认参数
来源：http://rxa.hnqzz.top

fun greet(name: String = "World") = "Hi $name"
来源：http://did.snrcjt.cn


<!-- 参考信息 -->