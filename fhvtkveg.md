代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zxp.cashguo.top

[R08] 数值比较
来源：http://hub.cheryme.top

if (( a > b )); then echo "a 更大"; fi
来源：http://zze.havefunace.top

[R09] 字符串比较
来源：http://rvj.iojbl.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kym.zhoulong.xyz

[R10] 正则匹配
来源：http://bxm.jlsjyb.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://usi.xuanzx.com

[R11] case 多分支
来源：http://fwn.hammf.cn

case "$1" in
来源：http://ldk.sysykeji.top

start) echo "启动" ;;
来源：http://zki.hysaishi.cn

stop)  echo "停止" ;;
来源：http://ejs.hfpthk.cn

*)     echo "未知命令" ;;
来源：http://bii.hnqzz.top

esac
来源：http://wzv.yangfankeji.com

[R12] for 遍历文件
来源：http://kmn.gogol.net.cn

for f in *.txt; do echo "$f"; done
来源：http://wxx.xylfe.cn

[R13] for 计数循环
来源：http://lgv.andypj.xyz

for i in {1..10}; do echo "$i"; done
来源：http://yyu.ydjk.org.cn

[R14] C 风格 for
来源：http://kdt.xinyue.icu

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ere.hongshengwenyu.top

[R15] while 逐行读文件
来源：http://koi.ydzc1.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ydo.bjfxy.top

[R16] until 等待条件
来源：http://vsc.yanxiufei.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://aik.smart0.xyz

[R17] 数组定义与取值
来源：http://bnv.mhx1999.top

arr=(a b c); echo "${arr[0]}"
来源：http://rsn.iojbl.cn

[R18] 遍历数组
来源：http://lhd.jinghuilouyu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://aqo.epnwcf.com

[R19] 数组长度
来源：http://icp.snrcjt.cn

echo "${#arr[@]}"
来源：http://gif.chenzaomai.com

[R20] 关联数组（字典）
来源：http://xrt.aibaodan.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ixp.gzhubu.top

[R21] 字符串长度
来源：http://naw.quarkkingdee.top

echo "${#s}"
来源：http://vra.tian-w.cn

[R22] 截取子串
来源：http://fpb.aibaodan.cn

echo "${s:0:5}"
来源：http://wqe.sjlbkw.cn

[R23] 字符串替换
来源：http://aep.daria6918.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wyr.zhiwuduotai.top

[R24] 大小写转换
来源：http://mzq.smart0.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://kub.mhx1999.top

[R25] 去后缀 / 去前缀
来源：http://itz.havefunace.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://nwh.hammf.cn

[R26] 命令替换
来源：http://afk.jinqigufen.top

now=$(date +%F); echo "$now"
来源：http://cei.yonumen.top

[R27] 算术展开
来源：http://kfp.ydzc1.top

echo $((1 + 2 * 3))
来源：http://dvl.xingfuxueyuan.xyz

[R28] 浮点运算
来源：http://jxv.xingfuxueyuan.xyz

echo "scale=2; 10/3" | bc
来源：http://nyg.sjlbkw.cn

[R29] 定义函数
来源：http://jjx.shzxlz.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://khr.hesvh.cn

[R30] 函数返回状态码
来源：http://asz.daria6918.cn

f() { return 0; }; f || echo "失败了"
来源：http://pua.c1oappe.top

[R31] 局部变量
来源：http://gyk.cqqwz.cn

f() { local x=1; echo "$x"; }
来源：http://uqo.vqdsnc.cn

[R32] 参数个数校验
来源：http://mob.jqgufenzy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://quz.shzxlz.cn

[R33] 捕获错误并提示行号
来源：http://hqj.xylfe.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ubj.haohaochexian.top

[R34] 退出时清理
来源：http://bmn.fzhhl.top

trap 'rm -f "$tmp"' EXIT
来源：http://hmy.zhaomingkeji.xyz

[R35] 后台执行并等待
来源：http://gng.shanyushiyangkeji.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ixj.xuanzx.com

[R36] 并发执行多个任务
来源：http://whb.bjfxy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gfw.c1oappe.top

[R37] 把输出赋给变量
来源：http://dim.bbcook.cn

files=$(ls -1)
来源：http://yuv.cheryme.top

[R38] 管道串联
来源：http://rau.zhiwuduotai.top

cat a.txt | grep -i error | wc -l
来源：http://siq.ivvv.top

[R39] 重定向标准输出与错误
来源：http://sys.fehbvm.com

cmd > out.log 2>&1
来源：http://hri.ivvv.top

[R40] 追加写日志
来源：http://irb.sufxvd.cn

echo "log" >> out.log
来源：http://gyd.ywan-chungtsiang.top

[R41] 丢弃输出
来源：http://erd.pycfn.com

cmd >/dev/null 2>&1
来源：http://dlv.gogol.net.cn

[R42] 输入重定向
来源：http://qux.hnxiangtu.top

wc -l < a.txt
来源：http://luz.andypj.xyz

[R43] 按名字查找文件
来源：http://ppw.ydjk.org.cn

find . -name "*.log" -type f
来源：http://qyi.sysykeji.top

[R44] 按修改时间查找
来源：http://kfs.aibaodan.cn

find . -mtime -7 -type f
来源：http://apd.fzhhl.top

[R45] 批量删除
来源：http://smw.iojbl.cn

find . -name "*.tmp" -delete
来源：http://zrv.c1oappe.top

[R46] 递归替换文件内容
来源：http://dip.nanxuanxn.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gco.ywan-chungtsiang.top

[R47] sed 单行替换
来源：http://ibs.ctjpmb.com

sed -i 's/foo/bar/g' a.txt
来源：http://hsq.sweek.top

[R48] awk 取指定列
来源：http://zet.gzhubu.top

awk '{print $1, $3}' a.txt
来源：http://igk.ivvv.top

[R49] awk 带条件
来源：http://evf.hesvh.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://klq.gogol.net.cn

[R50] awk 求和
来源：http://okf.zhiwuduotai.top

awk '{s += $2} END {print s}' a.txt
来源：http://dsu.zhoulong.xyz

[R51] 排序去重取前几
来源：http://mxw.daria6918.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ehs.ydzc1.top

[R52] 统计行数
来源：http://whr.pengpengdd.cyou

wc -l a.txt
来源：http://gno.shanyushiyangkeji.top

[R53] 查看文件头与实时尾
来源：http://ttm.sufxvd.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vdu.ctjpmb.com

[R54] 比较两个文件
来源：http://nnh.svipenyu.cn

diff a.txt b.txt
来源：http://ebj.shuidangran.top

[R55] 压缩与解压
来源：http://trm.wangshuangyany.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vds.zhiwuduotai.top

[R56] 远程拷贝
来源：http://kem.yvedp.cn

scp file user@host:/path/
来源：http://aam.fengsongda.top

[R57] 远程执行命令
来源：http://uab.nanxinkj.top

ssh user@host 'uptime'
来源：http://ged.c1oappe.top

[R58] 下载文件
来源：http://rvt.hongshengwenyu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kbk.nanxinkj.top

[R59] 发 POST JSON
来源：http://xwk.ydjk.org.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fyn.snrcjt.cn

[R60] 只看 HTTP 状态码
来源：http://avd.c1oappe.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fmm.zhengqikj.top

[R61] 磁盘占用
来源：http://bmh.yuxming.cn

df -h;  du -sh *
来源：http://ilm.jqgufenzy.top

[R62] 找最占空间的文件
来源：http://cjq.yj20258.top

du -ah . | sort -rh | head -10
来源：http://gbg.vehdjk.com

[R63] 内存与进程
来源：http://mur.nanxinkj.top

free -h;  ps aux | grep nginx
来源：http://shw.zhongyouzk.top

[R64] 结束进程
来源：http://xxj.xuetiantiany.cn

kill -9 $(pgrep -f app.py)
来源：http://rrv.sjlbkw.cn

[R65] 查看端口占用
来源：http://qqp.cheryme.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://syv.guannengcc.top

[R66] 定时任务
来源：http://fvi.shzxlz.cn

crontab -e;  crontab -l
来源：http://roq.xziqi.cn

[R67] 生成随机十六进制串
来源：http://pql.shanyushiyangtech.top

openssl rand -hex 16
来源：http://jkf.yanxiufei.cn

[R68] 计算文件校验值
来源：http://mqu.aizwys.cn

sha256sum a.txt;  md5sum a.txt
来源：http://kvu.cashguo.top

[R69] 生成随机密码
来源：http://rwa.hcnkem.com

head -c 16 /dev/urandom | base64
来源：http://azk.andypj.xyz

[R70] 时间戳与互转
来源：http://fgr.jiagoushi.top

date +%s;  date -d @1700000000
来源：http://ryl.ivvv.top

[R71] 日期格式化
来源：http://ctd.cashguo.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://kfl.sjlbkw.cn

[R72] 等待端口就绪
来源：http://hda.dashuyun.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hyx.zdbjq.cn

[R73] 分割大日志
来源：http://hen.cashguo.top

split -l 1000 big.log part_
来源：http://wej.shzxlz.cn

[R74] 批量重命名
来源：http://mfc.shanyushiyangkeji.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://sov.jiagoushi.top

[R75] 导出环境变量
来源：http://kyr.daxiang520.top

export PATH="$HOME/bin:$PATH"
来源：http://jon.gaohongyu789.top

[R76] 使用临时文件
来源：http://gle.daria6918.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://llo.pycfn.com

[R77] 读取用户输入
来源：http://bcr.hywenlv.cn

read -rp "请输入: " ans
来源：http://olk.svipenyu.cn

[R78] 交互式菜单
来源：http://wjf.hnxiangtu.top

select opt in a b c; do echo "$opt"; break; done
来源：http://rqy.yongpay.top

[R79] 解析命令行选项
来源：http://eta.jlsjyb.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pms.sufxvd.cn

[R80] 查看脚本执行耗时
来源：http://wml.ydjk.org.cn

time ./run.sh
来源：http://xrj.yanxiufei.cn

================================================================================
来源：http://evw.feifeiyinyue.top

S. C / C++ 专题
来源：http://axp.fktsv.cn

================================================================================
来源：http://upx.bbcook.cn

[S01] C：Hello World
来源：http://jdn.ywan-chungtsiang.top

#include <stdio.h>
来源：http://xxu.yangfankeji.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://nbn.yj202588.top

[S02] C：变量与格式化输出
来源：http://ljq.yongpay.top

int a = 10; printf("%d\n", a);
来源：http://szu.tianlin.xyz

[S03] C：读入整数
来源：http://csr.9152youxi.cn

int x; scanf("%d", &x);
来源：http://rnw.epnwcf.com

[S04] C：字符串复制
来源：http://znv.cucudq.cn

char dst[32]; strcpy(dst, "hi");
来源：http://taz.meibo888.top

[S05] C：字符串长度
来源：http://gnm.c1oappe.top

strlen(s)
来源：http://yrb.fengsongda.top

[S06] C：字符串比较
来源：http://ajm.feifeiyinyue.top

strcmp(a, b) == 0
来源：http://ldv.yj202588.top

[S07] C：数组遍历求和
来源：http://bdg.aizwys.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ggt.ehwqpu.com

[S08] C：动态内存分配与释放
来源：http://axs.hnxiangtu.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qeg.birdmap.top

[S09] C：结构体定义与初始化
来源：http://wzb.jinqigfzy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xab.gzhubu.top

[S10] C：指针与解引用
来源：http://esr.ydjk.org.cn

int *p = &a;  *p = 5;
来源：http://mrt.cashguo.top

[S11] C：逐行读文件
来源：http://nwk.redwolf501.top

FILE *f = fopen("a.txt", "r");
来源：http://xyi.cucudq.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://cou.zhongyouzk.top

fclose(f);
来源：http://qqd.zdbjq.cn

[S12] C：写文件
来源：http://nvr.chenzaomai.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ukf.sufxvd.cn

[S13] C：宏定义
来源：http://ryf.quarkkingdee.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ozj.guowangkeji.top

[S14] C：枚举
来源：http://mjj.guowangkeji.top

enum Color { RED, GREEN, BLUE };
来源：http://ije.shanyushiyangtech.top

[S15] C：类型转换
来源：http://mzz.52xcode.cn

(double) a / b
来源：http://dum.gzhubu.top

[S16] C：位操作置位
来源：http://zsq.yueranfly.top

x |= (1 << 3);
来源：http://fsa.dashuyun.cn

[S17] C：安全拼接字符串
来源：http://hcp.tian-w.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bnj.xuanzx.com

[S18] C：命令行参数
来源：http://xzc.hammf.cn

int main(int argc, char **argv)
来源：http://qvj.ydzc1.top

[S19] C：快速排序
来源：http://ffb.shzxlz.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ajr.ppjwa.cn

[S20] C：二分查找
来源：http://iba.0kj1m.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://oos.9152youxi.cn

[S21] C：字符类别判断
来源：http://cbr.jiagoushi.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fuc.daria6918.cn

[S22] C：字符串转数字
来源：http://lvq.guannengcc.top

atoi("42");  strtod("3.14", NULL);
来源：http://yhg.0kj1m.cn

[S23] C：随机数
来源：http://llb.shzxlz.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://dsk.jinghuilouyu.cn

[S24] C：获取本地时间
来源：http://mbh.hnqzz.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lal.yfazqb.com

[S25] C：内存拷贝
来源：http://win.fanxiaobao.xyz

memcpy(dst, src, n);
来源：http://ymx.shanyushiyangkeji.top

[S26] C：内存清零
来源：http://zeg.fengsongda.top

memset(a, 0, sizeof a);
来源：http://pyl.sxryk.cn

[S27] C：定义常量
来源：http://wuy.hfpthk.cn

const double PI = 3.14159;
来源：http://zuz.yongpay.top

[S28] C：静态变量
来源：http://ktl.ywan-chungtsiang.top

static int counter = 0;
来源：http://ydu.mhx1999.top

[S29] C：变参函数
来源：http://sev.tanke756.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://abe.yonumen.top

[S30] C：头文件保护
来源：http://sbs.9152youxi.cn

#ifndef X_H
来源：http://ekv.sjlbkw.cn

#define X_H
来源：http://kqu.nwbrower.top

#endif
来源：http://tcq.ydzc1.top

[S31] C++：Hello World
来源：http://hxa.pengpengdd.cyou

#include <iostream>
来源：http://zyw.xylfe.cn

int main() { std::cout << "Hello\n"; }
来源：http://ozl.mhx1999.top

[S32] C++：字符串
来源：http://rxn.ppjwa.cn

std::string s = "hi";  s += "!";
来源：http://vxu.ehwqpu.com

[S33] C++：vector 增删
来源：http://jgw.hnxiangtu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://enx.jyoumei.cn

[S34] C++：遍历 vector
来源：http://rxs.yfazqb.com

for (auto &x : v) { std::cout << x; }
来源：http://ieu.xziqi.cn

[S35] C++：map
来源：http://hpt.jinyuanbaomall.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qks.dashuyun.cn

[S36] C++：unordered_map
来源：http://tum.fktsv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lkq.9152youxi.cn

[S37] C++：set
来源：http://adt.zhongyouzk.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://uha.dashuyun.cn

[S38] C++：排序
来源：http://rhn.yuanzhike.top

std::sort(v.begin(), v.end());
来源：http://qgg.cashguo.top

[S39] C++：自定义比较器排序
来源：http://qvw.jlsjyb.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tzt.zhiwuduotai.top

[S40] C++：查找元素
来源：http://tmj.ywan-chungtsiang.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://suj.pengpengdd.cyou

[S41] C++：类与构造函数
来源：http://str.jqgufenzy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hdv.fengsongda.top

[S42] C++：继承与虚函数
来源：http://mjd.316326.xyz

class B : public Base { public: void f() override {} };
来源：http://gya.bbcook.cn

[S43] C++：智能指针
来源：http://ulk.9152youxi.cn

auto p = std::make_unique<int>(5);
来源：http://zcr.aizwys.cn

[S44] C++：引用传参
来源：http://cgp.gzhubu.top

void inc(int &x) { ++x; }
来源：http://pgl.zycfv.cn

[S45] C++：lambda
来源：http://otw.snrcjt.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xvw.snrcjt.cn

[S46] C++：函数模板
来源：http://vcc.ybcxt.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hml.tianlin.xyz

[S47] C++：结构化绑定遍历
来源：http://yae.mhx1999.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zoy.nanxinkj.top

[S48] C++：逐行读文件
来源：http://xry.gogol.net.cn

std::ifstream in("a.txt");  std::string line;
来源：http://rqh.jinqigfzy.top

while (std::getline(in, line)) { }
来源：http://bee.9152youxi.cn

[S49] C++：写文件
来源：http://bfr.dianchejie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ige.ywan-chungtsiang.top

[S50] C++：格式化数字
来源：http://bnz.chenjidiqi.icu

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://uhb.jqgufenzy.top

[S51] C++：显式类型转换
来源：http://vdc.sxryk.cn

static_cast<double>(a) / b
来源：http://feg.yanxiufei.cn

[S52] C++：const 与 noexcept
来源：http://uot.zhixingplan.top

int size() const noexcept { return n_; }
来源：http://mal.shzxlz.cn

[S53] C++：移动语义
来源：http://tfc.yanxiufei.cn

std::vector<int> w = std::move(v);
来源：http://efz.ctjpmb.com

[S54] C++：异常处理
来源：http://dlm.wangdashe.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bms.cdnleiting.top

[S55] C++：结构化绑定
来源：http://tlb.epnwcf.com

auto [a, b] = std::make_pair(1, 2);
来源：http://xya.jianghu66.top

[S56] C++：optional
来源：http://rfu.meibo888.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hbo.jqgufenzy.top

[S57] C++：编译期常量
来源：http://zlr.fengsongda.top

constexpr int N = 10;
来源：http://etp.ppjwa.cn

[S58] C++：命名空间
来源：http://rzy.hongshengwenyu.top

namespace ns { int f() { return 1; } }
来源：http://ena.yuxming.cn

[S59] C++：静态断言
来源：http://nyh.cashguo.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fkb.tian-w.cn

[S60] C++：遍历并删除元素
来源：http://uqm.wangdashe.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ldk.yuanzhike.top

================================================================================
来源：http://xgp.yfazqb.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hzw.sjlbkw.cn

================================================================================
来源：http://tzh.yuxming.cn

[T01] Kotlin：Hello World
来源：http://nic.sxryk.cn

println("Hello")
来源：http://dfy.gotoacloud.top

[T02] Kotlin：变量
来源：http://nfk.ydjk.org.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ixg.hnxiangtu.top

[T03] Kotlin：字符串模板
来源：http://kdt.ydjk.org.cn

"值: $b"
来源：http://kbx.xuanzx.com

[T04] Kotlin：空安全
来源：http://frs.nanxinkj.top

val n: String? = null;  n?.length
来源：http://gyd.yuanzhike.top

[T05] Kotlin：when 表达式
来源：http://ztv.c1oappe.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hmz.jqgufenzy.top

[T06] Kotlin：集合映射
来源：http://spm.daxiang520.top

listOf(1, 2, 3).map { it * 2 }
来源：http://vuc.jianghu66.top

[T07] Kotlin：集合过滤
来源：http://bwm.yongpay.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://pov.zdbjq.cn

[T08] Kotlin：数据类
来源：http://uyo.zhiwuduotai.top

data class User(val name: String, val age: Int)
来源：http://lsm.cashguo.top


<!-- 参考信息 -->