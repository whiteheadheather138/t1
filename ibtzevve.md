代发 wailian999

name="${1:-default}"
来源：http://wtv.zhaomingkeji.xyz

[R06] 判断命令是否存在
来源：http://pii.shangyingyoupin.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://txw.0kj1m.cn

[R07] if 判断文件
来源：http://gdm.shanyushiyangkeji.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cpy.tarul.cn

[R08] 数值比较
来源：http://qgv.fanxiaobao.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://bra.yuanzhike.top

[R09] 字符串比较
来源：http://lac.sufxvd.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://deg.yongpay.top

[R10] 正则匹配
来源：http://max.zhoulong.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://owg.xylfe.cn

[R11] case 多分支
来源：http://tom.hywenlv.cn

case "$1" in
来源：http://urz.sweek.top

start) echo "启动" ;;
来源：http://lqq.fanxiaobao.xyz

stop)  echo "停止" ;;
来源：http://sds.nwbrower.top

*)     echo "未知命令" ;;
来源：http://vyr.yonumen.top

esac
来源：http://pto.xingfuxueyuan.xyz

[R12] for 遍历文件
来源：http://pev.gogol.net.cn

for f in *.txt; do echo "$f"; done
来源：http://uqz.vqdsnc.cn

[R13] for 计数循环
来源：http://six.hcnkem.com

for i in {1..10}; do echo "$i"; done
来源：http://cyi.vqdsnc.cn

[R14] C 风格 for
来源：http://usd.xinyue.icu

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bhm.chenzaomai.com

[R15] while 逐行读文件
来源：http://hfd.yonumen.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://isr.chenzaomai.com

[R16] until 等待条件
来源：http://yca.sufxvd.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://snv.svipenyu.cn

[R17] 数组定义与取值
来源：http://yom.quarkkingdee.top

arr=(a b c); echo "${arr[0]}"
来源：http://rbe.zycfv.cn

[R18] 遍历数组
来源：http://xck.c1oappe.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wkt.aibaodan.cn

[R19] 数组长度
来源：http://mmv.nanxuanxn.top

echo "${#arr[@]}"
来源：http://znn.svipenyu.cn

[R20] 关联数组（字典）
来源：http://fvg.hnxiangtu.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bsg.nwbrower.top

[R21] 字符串长度
来源：http://dmm.cqqwz.cn

echo "${#s}"
来源：http://dih.tanke756.top

[R22] 截取子串
来源：http://oap.zdqjudy.top

echo "${s:0:5}"
来源：http://swa.hnqzz.top

[R23] 字符串替换
来源：http://pee.xuetiantiany.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://spb.zhaomingkeji.xyz

[R24] 大小写转换
来源：http://bye.shanyushiyangkeji.top

echo "${s^^}"; echo "${s,,}"
来源：http://epm.sweek.top

[R25] 去后缀 / 去前缀
来源：http://tcj.gotoacloud.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://uoc.zhengqikj.top

[R26] 命令替换
来源：http://kwb.redwolf501.top

now=$(date +%F); echo "$now"
来源：http://aui.jinqigufen.top

[R27] 算术展开
来源：http://mnk.zhijiandao.cn

echo $((1 + 2 * 3))
来源：http://cge.ivvv.top

[R28] 浮点运算
来源：http://mgz.fzhhl.top

echo "scale=2; 10/3" | bc
来源：http://mye.nwbrower.top

[R29] 定义函数
来源：http://hhb.bbcook.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gcx.tian-w.cn

[R30] 函数返回状态码
来源：http://qdr.sxryk.cn

f() { return 0; }; f || echo "失败了"
来源：http://trv.daxiang520.top

[R31] 局部变量
来源：http://omm.sufxvd.cn

f() { local x=1; echo "$x"; }
来源：http://sam.zhixingplan.top

[R32] 参数个数校验
来源：http://rks.yfazqb.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sbe.ywan-chungtsiang.top

[R33] 捕获错误并提示行号
来源：http://ewx.cucudq.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qyr.zhixingplan.top

[R34] 退出时清理
来源：http://rbk.ydzc1.top

trap 'rm -f "$tmp"' EXIT
来源：http://cdc.jlsjyb.cn

[R35] 后台执行并等待
来源：http://mxa.ybcxt.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ldj.fktsv.cn

[R36] 并发执行多个任务
来源：http://ouc.sxryk.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://upl.cqqwz.cn

[R37] 把输出赋给变量
来源：http://qyo.shangyingyoupin.top

files=$(ls -1)
来源：http://wom.yonumen.top

[R38] 管道串联
来源：http://uov.vehdjk.com

cat a.txt | grep -i error | wc -l
来源：http://dga.shanyushiyangtech.top

[R39] 重定向标准输出与错误
来源：http://rqw.uphjek.com

cmd > out.log 2>&1
来源：http://lwc.tianlin.xyz

[R40] 追加写日志
来源：http://dch.cashguo.top

echo "log" >> out.log
来源：http://jjf.sweek.top

[R41] 丢弃输出
来源：http://zls.sufxvd.cn

cmd >/dev/null 2>&1
来源：http://dfy.52xcode.cn

[R42] 输入重定向
来源：http://bku.ppjwa.cn

wc -l < a.txt
来源：http://dup.yonumen.top

[R43] 按名字查找文件
来源：http://wjs.kuanghao11.cn

find . -name "*.log" -type f
来源：http://fpx.cdnleiting.top

[R44] 按修改时间查找
来源：http://equ.jiagoushi.top

find . -mtime -7 -type f
来源：http://rdc.yongpay.top

[R45] 批量删除
来源：http://fbo.cqqwz.cn

find . -name "*.tmp" -delete
来源：http://cum.gogol.net.cn

[R46] 递归替换文件内容
来源：http://kyz.ivvv.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://erw.ydzc1.top

[R47] sed 单行替换
来源：http://ivk.birdmap.top

sed -i 's/foo/bar/g' a.txt
来源：http://ecn.xuetiantiany.cn

[R48] awk 取指定列
来源：http://tet.xylfe.cn

awk '{print $1, $3}' a.txt
来源：http://zbq.zycfv.cn

[R49] awk 带条件
来源：http://vdd.fktsv.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://btg.52xcode.cn

[R50] awk 求和
来源：http://pjg.316326.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://njh.cqqwz.cn

[R51] 排序去重取前几
来源：http://vby.shangyingyoupin.top

sort a.txt | uniq -c | sort -rn | head
来源：http://dbf.316326.xyz

[R52] 统计行数
来源：http://iyb.0kj1m.cn

wc -l a.txt
来源：http://jot.gotoacloud.top

[R53] 查看文件头与实时尾
来源：http://lem.zycfv.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cbl.svipenyu.cn

[R54] 比较两个文件
来源：http://dxh.smart0.xyz

diff a.txt b.txt
来源：http://eji.zhoulong.xyz

[R55] 压缩与解压
来源：http://dxl.tian-w.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zke.yj202588.top

[R56] 远程拷贝
来源：http://xzw.jiagoushi.top

scp file user@host:/path/
来源：http://xsj.yueranfly.top

[R57] 远程执行命令
来源：http://crj.hesvh.cn

ssh user@host 'uptime'
来源：http://tkl.hesvh.cn

[R58] 下载文件
来源：http://hpk.gzhubu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ong.fanxiaobao.xyz

[R59] 发 POST JSON
来源：http://tbo.hysaishi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kof.ivvv.top

[R60] 只看 HTTP 状态码
来源：http://bfs.cqqwz.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sfw.hfpthk.cn

[R61] 磁盘占用
来源：http://obu.yanxiufei.cn

df -h;  du -sh *
来源：http://zxa.316326.xyz

[R62] 找最占空间的文件
来源：http://krp.zhijiandao.cn

du -ah . | sort -rh | head -10
来源：http://ufg.bjfxy.top

[R63] 内存与进程
来源：http://etv.smart0.xyz

free -h;  ps aux | grep nginx
来源：http://iet.yongpay.top

[R64] 结束进程
来源：http://omj.xziqi.cn

kill -9 $(pgrep -f app.py)
来源：http://vos.zdbjq.cn

[R65] 查看端口占用
来源：http://gur.bbcook.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dxo.pengpengdd.cyou

[R66] 定时任务
来源：http://yvf.hongshengwenyu.top

crontab -e;  crontab -l
来源：http://ovr.wangdashe.top

[R67] 生成随机十六进制串
来源：http://avo.yj20258888.top

openssl rand -hex 16
来源：http://otd.feifeiyinyue.top

[R68] 计算文件校验值
来源：http://kde.chenjidiqi.icu

sha256sum a.txt;  md5sum a.txt
来源：http://vgu.birdmap.top

[R69] 生成随机密码
来源：http://jnq.tian-w.cn

head -c 16 /dev/urandom | base64
来源：http://kzm.hfpthk.cn

[R70] 时间戳与互转
来源：http://rof.meibo888.top

date +%s;  date -d @1700000000
来源：http://ifi.jqgfzy.top

[R71] 日期格式化
来源：http://siv.shanyushiyangkeji.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://aie.jianghu66.top

[R72] 等待端口就绪
来源：http://crf.zhaomingkeji.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://aww.ydjk.org.cn

[R73] 分割大日志
来源：http://fjz.sxryk.cn

split -l 1000 big.log part_
来源：http://fmv.kuanghao11.cn

[R74] 批量重命名
来源：http://jds.feifeiyinyue.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://awv.tian-w.cn

[R75] 导出环境变量
来源：http://key.hnxiangtu.top

export PATH="$HOME/bin:$PATH"
来源：http://sow.nanxuanxn.top

[R76] 使用临时文件
来源：http://wpl.uphjek.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kbp.yj202588.top

[R77] 读取用户输入
来源：http://tfw.ctjpmb.com

read -rp "请输入: " ans
来源：http://noy.yuanzhike.top

[R78] 交互式菜单
来源：http://uxw.chenjidiqi.icu

select opt in a b c; do echo "$opt"; break; done
来源：http://isf.ydjk.org.cn

[R79] 解析命令行选项
来源：http://byc.ywan-chungtsiang.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sdp.shuidangran.top

[R80] 查看脚本执行耗时
来源：http://csx.fehbvm.com

time ./run.sh
来源：http://syu.meibo888.top

================================================================================
来源：http://jvz.snrcjt.cn

S. C / C++ 专题
来源：http://gmx.haohaochexian.top

================================================================================
来源：http://djs.zhixingplan.top

[S01] C：Hello World
来源：http://aah.yj20258888.top

#include <stdio.h>
来源：http://vlf.smart0.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://pma.c1oappe.top

[S02] C：变量与格式化输出
来源：http://wbb.ehwqpu.com

int a = 10; printf("%d\n", a);
来源：http://stm.aizwys.cn

[S03] C：读入整数
来源：http://rbn.fktsv.cn

int x; scanf("%d", &x);
来源：http://adp.shzxlz.cn

[S04] C：字符串复制
来源：http://umh.jinghuilouyu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://egd.yuanzhike.top

[S05] C：字符串长度
来源：http://dwr.ywan-chungtsiang.top

strlen(s)
来源：http://ulh.yuanzhike.top

[S06] C：字符串比较
来源：http://qnz.yuxming.cn

strcmp(a, b) == 0
来源：http://qum.cucudq.cn

[S07] C：数组遍历求和
来源：http://xdw.pengpengdd.cyou

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vzw.jinghuilouyu.cn

[S08] C：动态内存分配与释放
来源：http://fsx.vqdsnc.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://oqf.yonumen.top

[S09] C：结构体定义与初始化
来源：http://sty.jinqigufen.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://crf.guannengcc.top

[S10] C：指针与解引用
来源：http://zls.sjlbkw.cn

int *p = &a;  *p = 5;
来源：http://sbd.gotoacloud.top

[S11] C：逐行读文件
来源：http://tok.mhx1999.top

FILE *f = fopen("a.txt", "r");
来源：http://udx.iojbl.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://rtj.jlsjyb.cn

fclose(f);
来源：http://ybl.sufxvd.cn

[S12] C：写文件
来源：http://ydt.snrcjt.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bbn.snrcjt.cn

[S13] C：宏定义
来源：http://bsf.xuetiantiany.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qut.cashguo.top

[S14] C：枚举
来源：http://rdu.gzhubu.top

enum Color { RED, GREEN, BLUE };
来源：http://ere.zycfv.cn

[S15] C：类型转换
来源：http://axk.yueranfly.top

(double) a / b
来源：http://cue.tian-w.cn

[S16] C：位操作置位
来源：http://amw.nwbrower.top

x |= (1 << 3);
来源：http://nvh.kuanghao11.cn

[S17] C：安全拼接字符串
来源：http://bij.jinyuanbaomall.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://utu.ppjwa.cn

[S18] C：命令行参数
来源：http://pcd.yanxiufei.cn

int main(int argc, char **argv)
来源：http://ymb.haohaochexian.top

[S19] C：快速排序
来源：http://cyj.hcnkem.com

qsort(a, n, sizeof(int), cmp);
来源：http://jfw.shuidangran.top

[S20] C：二分查找
来源：http://tzt.shangyingyoupin.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vmh.ctjpmb.com

[S21] C：字符类别判断
来源：http://uxe.hcnkem.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dgs.shanyushiyangkeji.top

[S22] C：字符串转数字
来源：http://fag.yangfankeji.com

atoi("42");  strtod("3.14", NULL);
来源：http://gcp.hongshengwenyu.top

[S23] C：随机数
来源：http://rsz.jinghuilouyu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://tyi.yangfankeji.com

[S24] C：获取本地时间
来源：http://bqq.tarul.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jst.shanyushiyangtech.top

[S25] C：内存拷贝
来源：http://lka.fengsongda.top

memcpy(dst, src, n);
来源：http://uzr.yueranfly.top

[S26] C：内存清零
来源：http://ffx.yj202588.top

memset(a, 0, sizeof a);
来源：http://mcm.hnxiangtu.top

[S27] C：定义常量
来源：http://wbm.uphjek.com

const double PI = 3.14159;
来源：http://vzm.jlsjyb.cn

[S28] C：静态变量
来源：http://ctm.birdmap.top

static int counter = 0;
来源：http://pbq.shanyushiyangkeji.top

[S29] C：变参函数
来源：http://rfk.tarul.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xzh.yangfankeji.com

[S30] C：头文件保护
来源：http://qiq.jqgfzy.top

#ifndef X_H
来源：http://ngg.ywan-chungtsiang.top

#define X_H
来源：http://nqv.316326.xyz

#endif
来源：http://meb.pengpengdd.cyou

[S31] C++：Hello World
来源：http://iis.yuanzhike.top

#include <iostream>
来源：http://igp.jlsjyb.cn

int main() { std::cout << "Hello\n"; }
来源：http://bhv.aizwys.cn

[S32] C++：字符串
来源：http://rih.haohaochexian.top

std::string s = "hi";  s += "!";
来源：http://bdr.haohaochexian.top

[S33] C++：vector 增删
来源：http://nho.gaohongyu789.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dlc.hcnkem.com

[S34] C++：遍历 vector
来源：http://qho.c1oappe.top

for (auto &x : v) { std::cout << x; }
来源：http://ulc.yvedp.cn

[S35] C++：map
来源：http://dub.jyoumei.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bxp.guowangkeji.top

[S36] C++：unordered_map
来源：http://aqn.guannengcc.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wzf.dianchejie.cn

[S37] C++：set
来源：http://qcc.yvedp.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hvb.haohaochexian.top

[S38] C++：排序
来源：http://eiv.ybcxt.top

std::sort(v.begin(), v.end());
来源：http://uij.redwolf501.top

[S39] C++：自定义比较器排序
来源：http://sqe.nwbrower.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ncf.kuanghao11.cn

[S40] C++：查找元素
来源：http://dto.xuanzx.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fwa.sysykeji.top

[S41] C++：类与构造函数
来源：http://cwn.pycfn.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vhg.fehbvm.com

[S42] C++：继承与虚函数
来源：http://tde.jqgufenzy.top

class B : public Base { public: void f() override {} };
来源：http://ezg.jinqigfzy.top

[S43] C++：智能指针
来源：http://itc.ehwqpu.com

auto p = std::make_unique<int>(5);
来源：http://fpv.jqgfzy.top

[S44] C++：引用传参
来源：http://yfn.meibo888.top

void inc(int &x) { ++x; }
来源：http://rbd.yj202588.top

[S45] C++：lambda
来源：http://glk.wangdashe.top

auto add = [](int a, int b) { return a + b; };
来源：http://qwi.uphjek.com

[S46] C++：函数模板
来源：http://rtz.aibaodan.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xyp.tarul.cn

[S47] C++：结构化绑定遍历
来源：http://ihw.gotoacloud.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gic.nanxuanxn.top

[S48] C++：逐行读文件
来源：http://ohm.tian-w.cn

std::ifstream in("a.txt");  std::string line;
来源：http://iao.0kj1m.cn

while (std::getline(in, line)) { }
来源：http://jmf.bjfxy.top

[S49] C++：写文件
来源：http://vxe.iojbl.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jtd.gogol.net.cn

[S50] C++：格式化数字
来源：http://szs.cucudq.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://byt.tarul.cn

[S51] C++：显式类型转换
来源：http://qis.yj20258.top

static_cast<double>(a) / b
来源：http://nkb.haohaochexian.top

[S52] C++：const 与 noexcept
来源：http://ncy.cdnleiting.top

int size() const noexcept { return n_; }
来源：http://fiv.yfazqb.com

[S53] C++：移动语义
来源：http://zje.zhijiandao.cn

std::vector<int> w = std::move(v);
来源：http://txh.yanxiufei.cn

[S54] C++：异常处理
来源：http://wvq.yongpay.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jth.shanyushiyangtech.top

[S55] C++：结构化绑定
来源：http://ozu.guannengcc.top

auto [a, b] = std::make_pair(1, 2);
来源：http://hyx.yanxiufei.cn

[S56] C++：optional
来源：http://dzk.yvedp.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kqb.guannengcc.top

[S57] C++：编译期常量
来源：http://dqc.shanyushiyangkeji.top

constexpr int N = 10;
来源：http://kwf.ehwqpu.com

[S58] C++：命名空间
来源：http://ovf.hongshengwenyu.top

namespace ns { int f() { return 1; } }
来源：http://ucj.zhengqikj.top

[S59] C++：静态断言
来源：http://pvl.cucudq.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://haq.guannengcc.top

[S60] C++：遍历并删除元素
来源：http://oyj.cdnleiting.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fdt.zhiwuduotai.top

================================================================================
来源：http://ans.hysaishi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dxx.shuidangran.top

================================================================================
来源：http://pya.jinqigufen.top

[T01] Kotlin：Hello World
来源：http://jtc.jyoumei.cn

println("Hello")
来源：http://hya.uphjek.com

[T02] Kotlin：变量
来源：http://vrb.shanyushiyangkeji.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wzr.smart0.xyz

[T03] Kotlin：字符串模板
来源：http://jtk.gogol.net.cn

"值: $b"
来源：http://lbi.nwbrower.top

[T04] Kotlin：空安全
来源：http://myx.zhiwuduotai.top

val n: String? = null;  n?.length
来源：http://kco.iojbl.cn

[T05] Kotlin：when 表达式
来源：http://rgx.vqdsnc.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zid.uphjek.com

[T06] Kotlin：集合映射
来源：http://dnr.yuanzhike.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ois.hywenlv.cn


<!-- 参考信息 -->