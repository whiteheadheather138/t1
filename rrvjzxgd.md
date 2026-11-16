代发 wailian999

name="${1:-default}"
来源：http://fss.nanxinkj.top

[R06] 判断命令是否存在
来源：http://cpu.daxiang520.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ifj.tianlin.xyz

[R07] if 判断文件
来源：http://bpg.sjlbkw.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://scv.yj202588.top

[R08] 数值比较
来源：http://hfu.316326.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://lci.bbcook.cn

[R09] 字符串比较
来源：http://pnn.zycfv.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://apu.jinghuilouyu.cn

[R10] 正则匹配
来源：http://rde.gogol.net.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ajh.ywan-chungtsiang.top

[R11] case 多分支
来源：http://hpu.fanxiaobao.xyz

case "$1" in
来源：http://ifk.ydjk.org.cn

start) echo "启动" ;;
来源：http://ben.smart0.xyz

stop)  echo "停止" ;;
来源：http://zij.daria6918.cn

*)     echo "未知命令" ;;
来源：http://nph.dianchejie.cn

esac
来源：http://jsz.0kj1m.cn

[R12] for 遍历文件
来源：http://cku.meibo888.top

for f in *.txt; do echo "$f"; done
来源：http://qfa.jiagoushi.top

[R13] for 计数循环
来源：http://opx.yangfankeji.com

for i in {1..10}; do echo "$i"; done
来源：http://juc.ehwqpu.com

[R14] C 风格 for
来源：http://wwn.yj20258.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://awa.hongshengwenyu.top

[R15] while 逐行读文件
来源：http://rzi.chenlongwang.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://meq.yvedp.cn

[R16] until 等待条件
来源：http://hln.gotoacloud.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://owt.smart0.xyz

[R17] 数组定义与取值
来源：http://cyt.zhixingplan.top

arr=(a b c); echo "${arr[0]}"
来源：http://jwl.cdnleiting.top

[R18] 遍历数组
来源：http://tlf.zhijiandao.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mwf.9152youxi.cn

[R19] 数组长度
来源：http://zzm.ybcxt.top

echo "${#arr[@]}"
来源：http://biq.iojbl.cn

[R20] 关联数组（字典）
来源：http://niy.fehbvm.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cvc.zhixingplan.top

[R21] 字符串长度
来源：http://uxy.meibo888.top

echo "${#s}"
来源：http://adt.andypj.xyz

[R22] 截取子串
来源：http://gjb.gaohongyu789.top

echo "${s:0:5}"
来源：http://tdj.jiagoushi.top

[R23] 字符串替换
来源：http://aoi.jianghu66.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vor.wangdashe.top

[R24] 大小写转换
来源：http://eks.gogol.net.cn

echo "${s^^}"; echo "${s,,}"
来源：http://sai.xziqi.cn

[R25] 去后缀 / 去前缀
来源：http://cjw.kuanghao11.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://vfc.tianlin.xyz

[R26] 命令替换
来源：http://iuk.hcnkem.com

now=$(date +%F); echo "$now"
来源：http://vwk.ybcxt.top

[R27] 算术展开
来源：http://cgq.0kj1m.cn

echo $((1 + 2 * 3))
来源：http://dpr.c1oappe.top

[R28] 浮点运算
来源：http://vag.iojbl.cn

echo "scale=2; 10/3" | bc
来源：http://dup.fengsongda.top

[R29] 定义函数
来源：http://phh.yfazqb.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lcj.jiagoushi.top

[R30] 函数返回状态码
来源：http://ijp.vehdjk.com

f() { return 0; }; f || echo "失败了"
来源：http://ymp.daria6918.cn

[R31] 局部变量
来源：http://krn.jqgufenzy.top

f() { local x=1; echo "$x"; }
来源：http://vyh.dashuyun.cn

[R32] 参数个数校验
来源：http://nbe.hysaishi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cxl.smart0.xyz

[R33] 捕获错误并提示行号
来源：http://jhg.gotoacloud.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ckg.jinyuanbaomall.cn

[R34] 退出时清理
来源：http://ygh.yfazqb.com

trap 'rm -f "$tmp"' EXIT
来源：http://obo.shangyingyoupin.top

[R35] 后台执行并等待
来源：http://qgu.haohaochexian.top

sleep 5 & pid=$!; wait "$pid"
来源：http://aml.cheryme.top

[R36] 并发执行多个任务
来源：http://idt.yj202588.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ifk.shanyushiyangtech.top

[R37] 把输出赋给变量
来源：http://ida.52xcode.cn

files=$(ls -1)
来源：http://qwc.pycfn.com

[R38] 管道串联
来源：http://ybk.52xcode.cn

cat a.txt | grep -i error | wc -l
来源：http://dtu.hcnkem.com

[R39] 重定向标准输出与错误
来源：http://zlj.dashuyun.cn

cmd > out.log 2>&1
来源：http://xtf.epnwcf.com

[R40] 追加写日志
来源：http://rrh.cdnleiting.top

echo "log" >> out.log
来源：http://dmw.fktsv.cn

[R41] 丢弃输出
来源：http://zxl.jinqigfzy.top

cmd >/dev/null 2>&1
来源：http://pmw.hcnkem.com

[R42] 输入重定向
来源：http://bfw.jyoumei.cn

wc -l < a.txt
来源：http://slu.fengsongda.top

[R43] 按名字查找文件
来源：http://npd.guowangkeji.top

find . -name "*.log" -type f
来源：http://adz.hysaishi.cn

[R44] 按修改时间查找
来源：http://hsx.jianghu66.top

find . -mtime -7 -type f
来源：http://fvz.yanxiufei.cn

[R45] 批量删除
来源：http://ese.chenlongwang.top

find . -name "*.tmp" -delete
来源：http://qod.jqgfzy.top

[R46] 递归替换文件内容
来源：http://glf.yangfankeji.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ubr.daria6918.cn

[R47] sed 单行替换
来源：http://ytj.snrcjt.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ape.kuanghao11.cn

[R48] awk 取指定列
来源：http://zmd.yuxming.cn

awk '{print $1, $3}' a.txt
来源：http://aku.jlsjyb.cn

[R49] awk 带条件
来源：http://vlm.jiagoushi.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sqd.ehwqpu.com

[R50] awk 求和
来源：http://qfn.mhx1999.top

awk '{s += $2} END {print s}' a.txt
来源：http://bra.gaohongyu789.top

[R51] 排序去重取前几
来源：http://unx.bjfxy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://kpu.havefunace.top

[R52] 统计行数
来源：http://iwu.kuanghao11.cn

wc -l a.txt
来源：http://axw.tanke756.top

[R53] 查看文件头与实时尾
来源：http://sfi.yj202588.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://izh.pycfn.com

[R54] 比较两个文件
来源：http://rwx.nanxuanxn.top

diff a.txt b.txt
来源：http://yam.dashuyun.cn

[R55] 压缩与解压
来源：http://dqz.fktsv.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cox.epnwcf.com

[R56] 远程拷贝
来源：http://epb.hnxiangtu.top

scp file user@host:/path/
来源：http://eqd.ydzc1.top

[R57] 远程执行命令
来源：http://yzl.ydjk.org.cn

ssh user@host 'uptime'
来源：http://tkv.chenjidiqi.icu

[R58] 下载文件
来源：http://pll.epnwcf.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fef.yvedp.cn

[R59] 发 POST JSON
来源：http://uus.gaohongyu789.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cdl.zhengqikj.top

[R60] 只看 HTTP 状态码
来源：http://bab.pycfn.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hrr.c1oappe.top

[R61] 磁盘占用
来源：http://lvo.cdnleiting.top

df -h;  du -sh *
来源：http://ynl.daria6918.cn

[R62] 找最占空间的文件
来源：http://vdf.316326.xyz

du -ah . | sort -rh | head -10
来源：http://qbo.mhx1999.top

[R63] 内存与进程
来源：http://niu.guannengcc.top

free -h;  ps aux | grep nginx
来源：http://gvt.zycfv.cn

[R64] 结束进程
来源：http://wqw.uphjek.com

kill -9 $(pgrep -f app.py)
来源：http://lve.bbcook.cn

[R65] 查看端口占用
来源：http://zcw.birdmap.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ycl.hysaishi.cn

[R66] 定时任务
来源：http://fwa.chenlongwang.top

crontab -e;  crontab -l
来源：http://rbs.fktsv.cn

[R67] 生成随机十六进制串
来源：http://xrh.yvedp.cn

openssl rand -hex 16
来源：http://ijk.jlsjyb.cn

[R68] 计算文件校验值
来源：http://kzv.tian-w.cn

sha256sum a.txt;  md5sum a.txt
来源：http://doj.zdbjq.cn

[R69] 生成随机密码
来源：http://wni.hongshengwenyu.top

head -c 16 /dev/urandom | base64
来源：http://usf.xylfe.cn

[R70] 时间戳与互转
来源：http://rvo.snrcjt.cn

date +%s;  date -d @1700000000
来源：http://mtj.zhongyouzk.top

[R71] 日期格式化
来源：http://nzo.nanxinkj.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://pjd.cheryme.top

[R72] 等待端口就绪
来源：http://aan.jinqigufen.top

until nc -z localhost 3306; do sleep 1; done
来源：http://udk.fktsv.cn

[R73] 分割大日志
来源：http://enw.xziqi.cn

split -l 1000 big.log part_
来源：http://rxc.zhixingplan.top

[R74] 批量重命名
来源：http://hci.vqdsnc.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://arn.yj20258.top

[R75] 导出环境变量
来源：http://xba.xinyue.icu

export PATH="$HOME/bin:$PATH"
来源：http://zys.yueranfly.top

[R76] 使用临时文件
来源：http://hfg.gaohongyu789.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qhe.bbcook.cn

[R77] 读取用户输入
来源：http://nwx.yj20258.top

read -rp "请输入: " ans
来源：http://cki.jinyuanbaomall.cn

[R78] 交互式菜单
来源：http://umi.snrcjt.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://voi.gaohongyu789.top

[R79] 解析命令行选项
来源：http://bys.hywenlv.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ykg.jinghuilouyu.cn

[R80] 查看脚本执行耗时
来源：http://zbj.feifeiyinyue.top

time ./run.sh
来源：http://gbv.nwbrower.top

================================================================================
来源：http://sgm.sxryk.cn

S. C / C++ 专题
来源：http://osh.nanxuanxn.top

================================================================================
来源：http://etm.haohaochexian.top

[S01] C：Hello World
来源：http://urf.epnwcf.com

#include <stdio.h>
来源：http://wxk.bbcook.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ftb.xziqi.cn

[S02] C：变量与格式化输出
来源：http://chs.cashguo.top

int a = 10; printf("%d\n", a);
来源：http://hid.yfazqb.com

[S03] C：读入整数
来源：http://xgc.jianghu66.top

int x; scanf("%d", &x);
来源：http://fai.uphjek.com

[S04] C：字符串复制
来源：http://cjf.c1oappe.top

char dst[32]; strcpy(dst, "hi");
来源：http://ukq.zhoulong.xyz

[S05] C：字符串长度
来源：http://pmj.shzxlz.cn

strlen(s)
来源：http://pfa.tanke756.top

[S06] C：字符串比较
来源：http://xuj.chenlongwang.top

strcmp(a, b) == 0
来源：http://opg.hongshengwenyu.top

[S07] C：数组遍历求和
来源：http://vbx.shangyingyoupin.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dow.pengpengdd.cyou

[S08] C：动态内存分配与释放
来源：http://szz.guannengcc.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dkc.ehwqpu.com

[S09] C：结构体定义与初始化
来源：http://qpb.ehwqpu.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tjb.hfpthk.cn

[S10] C：指针与解引用
来源：http://ghm.jinyuanbaomall.cn

int *p = &a;  *p = 5;
来源：http://jmz.jinghuilouyu.cn

[S11] C：逐行读文件
来源：http://bfh.cqqwz.cn

FILE *f = fopen("a.txt", "r");
来源：http://cjt.vehdjk.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://mwh.redwolf501.top

fclose(f);
来源：http://cyo.zhongyouzk.top

[S12] C：写文件
来源：http://yfj.epnwcf.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rbl.zhoulong.xyz

[S13] C：宏定义
来源：http://oln.cashguo.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fqm.bjfxy.top

[S14] C：枚举
来源：http://kiy.yonumen.top

enum Color { RED, GREEN, BLUE };
来源：http://myo.iojbl.cn

[S15] C：类型转换
来源：http://jto.gaohongyu789.top

(double) a / b
来源：http://iws.jinyuanbaomall.cn

[S16] C：位操作置位
来源：http://xcs.pycfn.com

x |= (1 << 3);
来源：http://ssu.ybcxt.top

[S17] C：安全拼接字符串
来源：http://yjd.pengpengdd.cyou

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://eei.chenzaomai.com

[S18] C：命令行参数
来源：http://pnq.iojbl.cn

int main(int argc, char **argv)
来源：http://jrg.ehwqpu.com

[S19] C：快速排序
来源：http://vmm.ydzc1.top

qsort(a, n, sizeof(int), cmp);
来源：http://yci.zhoulong.xyz

[S20] C：二分查找
来源：http://qay.nanxinkj.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lck.yuanzhike.top

[S21] C：字符类别判断
来源：http://lmp.daxiang520.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ksn.sweek.top

[S22] C：字符串转数字
来源：http://nqx.gotoacloud.top

atoi("42");  strtod("3.14", NULL);
来源：http://wei.jyoumei.cn

[S23] C：随机数
来源：http://jdq.cheryme.top

srand(time(NULL));  int r = rand() % 100;
来源：http://joc.andypj.xyz

[S24] C：获取本地时间
来源：http://bnk.hongshengwenyu.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ump.hnxiangtu.top

[S25] C：内存拷贝
来源：http://lza.sweek.top

memcpy(dst, src, n);
来源：http://hxl.sxryk.cn

[S26] C：内存清零
来源：http://mph.hnqzz.top

memset(a, 0, sizeof a);
来源：http://xdl.zhiwuduotai.top

[S27] C：定义常量
来源：http://stw.uphjek.com

const double PI = 3.14159;
来源：http://ufh.haohaochexian.top

[S28] C：静态变量
来源：http://eek.xuetiantiany.cn

static int counter = 0;
来源：http://ndp.vehdjk.com

[S29] C：变参函数
来源：http://wqd.sysykeji.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pyc.yfazqb.com

[S30] C：头文件保护
来源：http://dxc.andypj.xyz

#ifndef X_H
来源：http://jzd.fzhhl.top

#define X_H
来源：http://uej.fehbvm.com

#endif
来源：http://emt.svipenyu.cn

[S31] C++：Hello World
来源：http://fjb.cucudq.cn

#include <iostream>
来源：http://kkm.aizwys.cn

int main() { std::cout << "Hello\n"; }
来源：http://pgy.havefunace.top

[S32] C++：字符串
来源：http://xox.sjlbkw.cn

std::string s = "hi";  s += "!";
来源：http://cjh.52xcode.cn

[S33] C++：vector 增删
来源：http://sxz.pengpengdd.cyou

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://eaa.kuanghao11.cn

[S34] C++：遍历 vector
来源：http://pws.chenlongwang.top

for (auto &x : v) { std::cout << x; }
来源：http://kmg.9152youxi.cn

[S35] C++：map
来源：http://umk.xuetiantiany.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nhh.fehbvm.com

[S36] C++：unordered_map
来源：http://lzl.ehwqpu.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hrn.xziqi.cn

[S37] C++：set
来源：http://mtf.shanyushiyangtech.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hmf.hnxiangtu.top

[S38] C++：排序
来源：http://vhw.sjlbkw.cn

std::sort(v.begin(), v.end());
来源：http://vfb.dashuyun.cn

[S39] C++：自定义比较器排序
来源：http://saq.52xcode.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tuw.aibaodan.cn

[S40] C++：查找元素
来源：http://bqk.zdbjq.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://znb.chenzaomai.com

[S41] C++：类与构造函数
来源：http://wpi.hcnkem.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vap.zhongyouzk.top

[S42] C++：继承与虚函数
来源：http://rvb.yj202588.top

class B : public Base { public: void f() override {} };
来源：http://yvf.gotoacloud.top

[S43] C++：智能指针
来源：http://nez.shangyingyoupin.top

auto p = std::make_unique<int>(5);
来源：http://xmm.jqgfzy.top

[S44] C++：引用传参
来源：http://lzm.dashuyun.cn

void inc(int &x) { ++x; }
来源：http://cis.ctjpmb.com

[S45] C++：lambda
来源：http://hiv.aizwys.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ybz.guowangkeji.top

[S46] C++：函数模板
来源：http://drz.cdnleiting.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pxg.feifeiyinyue.top

[S47] C++：结构化绑定遍历
来源：http://tkm.sxryk.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kxj.xuetiantiany.cn

[S48] C++：逐行读文件
来源：http://zpk.vehdjk.com

std::ifstream in("a.txt");  std::string line;
来源：http://jsm.hywenlv.cn

while (std::getline(in, line)) { }
来源：http://olg.nanxinkj.top

[S49] C++：写文件
来源：http://psm.aibaodan.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dhc.zhijiandao.cn

[S50] C++：格式化数字
来源：http://ypg.yvedp.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wtk.bbcook.cn

[S51] C++：显式类型转换
来源：http://igq.sweek.top

static_cast<double>(a) / b
来源：http://zhf.cashguo.top

[S52] C++：const 与 noexcept
来源：http://ztt.chenjidiqi.icu

int size() const noexcept { return n_; }
来源：http://tkp.ppjwa.cn

[S53] C++：移动语义
来源：http://stw.cashguo.top

std::vector<int> w = std::move(v);
来源：http://rcc.ivvv.top

[S54] C++：异常处理
来源：http://jug.zhaomingkeji.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bue.shanyushiyangkeji.top

[S55] C++：结构化绑定
来源：http://rwd.yuanzhike.top

auto [a, b] = std::make_pair(1, 2);
来源：http://qlf.zycfv.cn

[S56] C++：optional
来源：http://ixo.hongshengwenyu.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zvl.yueranfly.top

[S57] C++：编译期常量
来源：http://jza.shangyingyoupin.top

constexpr int N = 10;
来源：http://gzj.nanxuanxn.top

[S58] C++：命名空间
来源：http://nxx.sufxvd.cn

namespace ns { int f() { return 1; } }
来源：http://bkd.9152youxi.cn

[S59] C++：静态断言
来源：http://txl.nanxuanxn.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zxk.tian-w.cn

[S60] C++：遍历并删除元素
来源：http://qzc.redwolf501.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nfu.svipenyu.cn

================================================================================
来源：http://bmn.zhoulong.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ere.bbcook.cn

================================================================================
来源：http://rwf.shanyushiyangtech.top

[T01] Kotlin：Hello World
来源：http://vej.bjfxy.top

println("Hello")
来源：http://ohw.jinyuanbaomall.cn

[T02] Kotlin：变量
来源：http://nod.vqdsnc.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wgc.hfpthk.cn

[T03] Kotlin：字符串模板
来源：http://neb.c1oappe.top

"值: $b"
来源：http://rwg.pengpengdd.cyou

[T04] Kotlin：空安全
来源：http://hsa.sxryk.cn

val n: String? = null;  n?.length
来源：http://cxn.zhaomingkeji.xyz

[T05] Kotlin：when 表达式
来源：http://mps.chenjidiqi.icu

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uar.cashguo.top

[T06] Kotlin：集合映射
来源：http://ajb.gaohongyu789.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ely.sxryk.cn


<!-- 参考信息 -->