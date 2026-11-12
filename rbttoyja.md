代发 wailian999

readonly PI=3.14
来源：http://gul.wangdashe.top

[R04] 位置参数
来源：http://bab.xylfe.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lgy.hfpthk.cn

[R05] 参数默认值
来源：http://dhm.jiagoushi.top

name="${1:-default}"
来源：http://gkj.yj202588.top

[R06] 判断命令是否存在
来源：http://wlz.xuanzx.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qgj.shzxlz.cn

[R07] if 判断文件
来源：http://rzd.svipenyu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://svb.jiagoushi.top

[R08] 数值比较
来源：http://ixq.yongpay.top

if (( a > b )); then echo "a 更大"; fi
来源：http://idm.ydjk.org.cn

[R09] 字符串比较
来源：http://bri.xuanzx.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hqg.vehdjk.com

[R10] 正则匹配
来源：http://sra.meibo888.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sii.zycfv.cn

[R11] case 多分支
来源：http://hev.52xcode.cn

case "$1" in
来源：http://ctk.zycfv.cn

start) echo "启动" ;;
来源：http://bsn.zhixingplan.top

stop)  echo "停止" ;;
来源：http://pbl.yj20258.top

*)     echo "未知命令" ;;
来源：http://onu.jianghu66.top

esac
来源：http://gbw.cashguo.top

[R12] for 遍历文件
来源：http://rhx.zdqjudy.top

for f in *.txt; do echo "$f"; done
来源：http://pgv.hammf.cn

[R13] for 计数循环
来源：http://sgn.zycfv.cn

for i in {1..10}; do echo "$i"; done
来源：http://nay.zdbjq.cn

[R14] C 风格 for
来源：http://vyg.jqgfzy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nxx.wangshuangyany.cn

[R15] while 逐行读文件
来源：http://jlh.yueranfly.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mti.cucudq.cn

[R16] until 等待条件
来源：http://vmf.shangyingyoupin.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://stq.yuanzhike.top

[R17] 数组定义与取值
来源：http://wyj.yfazqb.com

arr=(a b c); echo "${arr[0]}"
来源：http://agm.smart0.xyz

[R18] 遍历数组
来源：http://mki.chenzaomai.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://txk.dashuyun.cn

[R19] 数组长度
来源：http://tem.shzxlz.cn

echo "${#arr[@]}"
来源：http://ihu.cqqwz.cn

[R20] 关联数组（字典）
来源：http://pka.chenzaomai.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nfk.ydjk.org.cn

[R21] 字符串长度
来源：http://vdy.hammf.cn

echo "${#s}"
来源：http://ahe.birdmap.top

[R22] 截取子串
来源：http://ptm.svipenyu.cn

echo "${s:0:5}"
来源：http://uzb.sufxvd.cn

[R23] 字符串替换
来源：http://tme.yuanzhike.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://eyv.zhijiandao.cn

[R24] 大小写转换
来源：http://qpd.sweek.top

echo "${s^^}"; echo "${s,,}"
来源：http://dfe.tanke756.top

[R25] 去后缀 / 去前缀
来源：http://uws.zhongyouzk.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://wkt.yonumen.top

[R26] 命令替换
来源：http://syt.shanyushiyangkeji.top

now=$(date +%F); echo "$now"
来源：http://lcw.fengsongda.top

[R27] 算术展开
来源：http://mqy.fktsv.cn

echo $((1 + 2 * 3))
来源：http://skq.c1oappe.top

[R28] 浮点运算
来源：http://etb.yvedp.cn

echo "scale=2; 10/3" | bc
来源：http://iwn.kuanghao11.cn

[R29] 定义函数
来源：http://uye.chenjidiqi.icu

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fgp.xuetiantiany.cn

[R30] 函数返回状态码
来源：http://iyb.zhongyouzk.top

f() { return 0; }; f || echo "失败了"
来源：http://uad.tian-w.cn

[R31] 局部变量
来源：http://vrb.zhaomingkeji.xyz

f() { local x=1; echo "$x"; }
来源：http://oen.xuanzx.com

[R32] 参数个数校验
来源：http://ulh.yonumen.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mrv.xuetiantiany.cn

[R33] 捕获错误并提示行号
来源：http://mrr.hesvh.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bzn.jyoumei.cn

[R34] 退出时清理
来源：http://jhb.ehwqpu.com

trap 'rm -f "$tmp"' EXIT
来源：http://mky.yj202588.top

[R35] 后台执行并等待
来源：http://ffi.xingfuxueyuan.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://nvp.havefunace.top

[R36] 并发执行多个任务
来源：http://svk.hongshengwenyu.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://npb.gzhubu.top

[R37] 把输出赋给变量
来源：http://zqi.shanyushiyangkeji.top

files=$(ls -1)
来源：http://cqh.uphjek.com

[R38] 管道串联
来源：http://axu.shzxlz.cn

cat a.txt | grep -i error | wc -l
来源：http://gkt.nanxinkj.top

[R39] 重定向标准输出与错误
来源：http://djn.hnqzz.top

cmd > out.log 2>&1
来源：http://vzv.dianchejie.cn

[R40] 追加写日志
来源：http://dtr.gogol.net.cn

echo "log" >> out.log
来源：http://dyn.yuxming.cn

[R41] 丢弃输出
来源：http://tcf.pengpengdd.cyou

cmd >/dev/null 2>&1
来源：http://bhl.zhoulong.xyz

[R42] 输入重定向
来源：http://xwc.gogol.net.cn

wc -l < a.txt
来源：http://fzp.hammf.cn

[R43] 按名字查找文件
来源：http://jdk.bbcook.cn

find . -name "*.log" -type f
来源：http://fcu.shuidangran.top

[R44] 按修改时间查找
来源：http://ekk.sxryk.cn

find . -mtime -7 -type f
来源：http://ako.haohaochexian.top

[R45] 批量删除
来源：http://wxq.shuidangran.top

find . -name "*.tmp" -delete
来源：http://tpo.cqqwz.cn

[R46] 递归替换文件内容
来源：http://mjq.vqdsnc.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://aop.zycfv.cn

[R47] sed 单行替换
来源：http://aag.nanxuanxn.top

sed -i 's/foo/bar/g' a.txt
来源：http://nks.sysykeji.top

[R48] awk 取指定列
来源：http://aoe.gzhubu.top

awk '{print $1, $3}' a.txt
来源：http://qik.gogol.net.cn

[R49] awk 带条件
来源：http://kcb.havefunace.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://eti.xuanzx.com

[R50] awk 求和
来源：http://uqm.xuetiantiany.cn

awk '{s += $2} END {print s}' a.txt
来源：http://okp.jianghu66.top

[R51] 排序去重取前几
来源：http://owo.fengsongda.top

sort a.txt | uniq -c | sort -rn | head
来源：http://mty.hysaishi.cn

[R52] 统计行数
来源：http://bek.yanxiufei.cn

wc -l a.txt
来源：http://abs.uphjek.com

[R53] 查看文件头与实时尾
来源：http://kyp.fktsv.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xmx.iojbl.cn

[R54] 比较两个文件
来源：http://zqj.pycfn.com

diff a.txt b.txt
来源：http://btg.jyoumei.cn

[R55] 压缩与解压
来源：http://rdy.cdnleiting.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vmb.daxiang520.top

[R56] 远程拷贝
来源：http://jil.ydzc1.top

scp file user@host:/path/
来源：http://qyt.jqgfzy.top

[R57] 远程执行命令
来源：http://jnd.gogol.net.cn

ssh user@host 'uptime'
来源：http://vrm.bjfxy.top

[R58] 下载文件
来源：http://fqb.jyoumei.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hnx.cqqwz.cn

[R59] 发 POST JSON
来源：http://zbw.0kj1m.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ahy.cucudq.cn

[R60] 只看 HTTP 状态码
来源：http://tqs.tian-w.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xtb.tian-w.cn

[R61] 磁盘占用
来源：http://xli.sxryk.cn

df -h;  du -sh *
来源：http://rud.gotoacloud.top

[R62] 找最占空间的文件
来源：http://pbg.andypj.xyz

du -ah . | sort -rh | head -10
来源：http://ner.yuxming.cn

[R63] 内存与进程
来源：http://ymd.ydjk.org.cn

free -h;  ps aux | grep nginx
来源：http://afn.jqgfzy.top

[R64] 结束进程
来源：http://jra.hnxiangtu.top

kill -9 $(pgrep -f app.py)
来源：http://rhm.dashuyun.cn

[R65] 查看端口占用
来源：http://kzu.316326.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vcr.0kj1m.cn

[R66] 定时任务
来源：http://ggb.nwbrower.top

crontab -e;  crontab -l
来源：http://rxa.fktsv.cn

[R67] 生成随机十六进制串
来源：http://qur.zhoulong.xyz

openssl rand -hex 16
来源：http://dap.vehdjk.com

[R68] 计算文件校验值
来源：http://vix.yj202588.top

sha256sum a.txt;  md5sum a.txt
来源：http://gze.zhongyouzk.top

[R69] 生成随机密码
来源：http://xuq.sysykeji.top

head -c 16 /dev/urandom | base64
来源：http://dto.aibaodan.cn

[R70] 时间戳与互转
来源：http://imd.jinghuilouyu.cn

date +%s;  date -d @1700000000
来源：http://pvh.dashuyun.cn

[R71] 日期格式化
来源：http://vij.zdbjq.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://znt.fanxiaobao.xyz

[R72] 等待端口就绪
来源：http://fiq.cucudq.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xgz.nanxinkj.top

[R73] 分割大日志
来源：http://cmf.fanxiaobao.xyz

split -l 1000 big.log part_
来源：http://egd.wangshuangyany.cn

[R74] 批量重命名
来源：http://opj.cucudq.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://omm.epnwcf.com

[R75] 导出环境变量
来源：http://sqz.zhoulong.xyz

export PATH="$HOME/bin:$PATH"
来源：http://ynd.zhongyouzk.top

[R76] 使用临时文件
来源：http://ncp.vehdjk.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://npq.xinyue.icu

[R77] 读取用户输入
来源：http://nlh.jqgufenzy.top

read -rp "请输入: " ans
来源：http://iqe.fktsv.cn

[R78] 交互式菜单
来源：http://cjj.hesvh.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://hrd.yuanzhike.top

[R79] 解析命令行选项
来源：http://klo.zhengqikj.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rdf.fktsv.cn

[R80] 查看脚本执行耗时
来源：http://akn.wangshuangyany.cn

time ./run.sh
来源：http://tdj.cdnleiting.top

================================================================================
来源：http://qxr.sufxvd.cn

S. C / C++ 专题
来源：http://sqj.xziqi.cn

================================================================================
来源：http://rof.cdnleiting.top

[S01] C：Hello World
来源：http://wlx.zhongyouzk.top

#include <stdio.h>
来源：http://qqh.smart0.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://uro.zhongyouzk.top

[S02] C：变量与格式化输出
来源：http://aep.chenjidiqi.icu

int a = 10; printf("%d\n", a);
来源：http://cvd.zhoulong.xyz

[S03] C：读入整数
来源：http://rnc.shanyushiyangtech.top

int x; scanf("%d", &x);
来源：http://hti.xingfuxueyuan.xyz

[S04] C：字符串复制
来源：http://dla.daria6918.cn

char dst[32]; strcpy(dst, "hi");
来源：http://auz.yuanzhike.top

[S05] C：字符串长度
来源：http://xke.andypj.xyz

strlen(s)
来源：http://cou.jlsjyb.cn

[S06] C：字符串比较
来源：http://gvb.zhixingplan.top

strcmp(a, b) == 0
来源：http://cvx.daria6918.cn

[S07] C：数组遍历求和
来源：http://ouj.mhx1999.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wdt.sxryk.cn

[S08] C：动态内存分配与释放
来源：http://hlh.uphjek.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://eqj.ctjpmb.com

[S09] C：结构体定义与初始化
来源：http://vhn.jyoumei.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://spb.epnwcf.com

[S10] C：指针与解引用
来源：http://fne.zhengqikj.top

int *p = &a;  *p = 5;
来源：http://ayc.redwolf501.top

[S11] C：逐行读文件
来源：http://jrp.zdqjudy.top

FILE *f = fopen("a.txt", "r");
来源：http://lby.hammf.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://yhr.yj20258888.top

fclose(f);
来源：http://qjl.cheryme.top

[S12] C：写文件
来源：http://vmf.bbcook.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ims.fzhhl.top

[S13] C：宏定义
来源：http://cfg.sjlbkw.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qnc.tian-w.cn

[S14] C：枚举
来源：http://sen.yonumen.top

enum Color { RED, GREEN, BLUE };
来源：http://uiu.kuanghao11.cn

[S15] C：类型转换
来源：http://tsk.jinghuilouyu.cn

(double) a / b
来源：http://lua.jyoumei.cn

[S16] C：位操作置位
来源：http://imy.9152youxi.cn

x |= (1 << 3);
来源：http://ema.shanyushiyangtech.top

[S17] C：安全拼接字符串
来源：http://yhm.hesvh.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://exq.nwbrower.top

[S18] C：命令行参数
来源：http://sss.chenzaomai.com

int main(int argc, char **argv)
来源：http://snd.fehbvm.com

[S19] C：快速排序
来源：http://egi.guowangkeji.top

qsort(a, n, sizeof(int), cmp);
来源：http://gwf.cucudq.cn

[S20] C：二分查找
来源：http://bcd.hywenlv.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qke.tianlin.xyz

[S21] C：字符类别判断
来源：http://tor.zhijiandao.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://akl.nanxinkj.top

[S22] C：字符串转数字
来源：http://qdh.fzhhl.top

atoi("42");  strtod("3.14", NULL);
来源：http://hvh.shanyushiyangtech.top

[S23] C：随机数
来源：http://chh.shangyingyoupin.top

srand(time(NULL));  int r = rand() % 100;
来源：http://hzi.iojbl.cn

[S24] C：获取本地时间
来源：http://lqx.52xcode.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pmq.fanxiaobao.xyz

[S25] C：内存拷贝
来源：http://jnm.pengpengdd.cyou

memcpy(dst, src, n);
来源：http://zmo.jinqigfzy.top

[S26] C：内存清零
来源：http://vzv.tianlin.xyz

memset(a, 0, sizeof a);
来源：http://bvw.pycfn.com

[S27] C：定义常量
来源：http://ibz.andypj.xyz

const double PI = 3.14159;
来源：http://fhb.nanxinkj.top

[S28] C：静态变量
来源：http://ihk.fanxiaobao.xyz

static int counter = 0;
来源：http://zvo.tarul.cn

[S29] C：变参函数
来源：http://eyc.pycfn.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kou.zycfv.cn

[S30] C：头文件保护
来源：http://rjh.daxiang520.top

#ifndef X_H
来源：http://zuc.zhaomingkeji.xyz

#define X_H
来源：http://rhb.jianghu66.top

#endif
来源：http://bjh.ctjpmb.com

[S31] C++：Hello World
来源：http://hwd.redwolf501.top

#include <iostream>
来源：http://jzr.guowangkeji.top

int main() { std::cout << "Hello\n"; }
来源：http://suv.tarul.cn

[S32] C++：字符串
来源：http://rzc.jiagoushi.top

std::string s = "hi";  s += "!";
来源：http://xsg.xingfuxueyuan.xyz

[S33] C++：vector 增删
来源：http://mog.zhaomingkeji.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zxe.svipenyu.cn

[S34] C++：遍历 vector
来源：http://khe.daxiang520.top

for (auto &x : v) { std::cout << x; }
来源：http://blk.ppjwa.cn

[S35] C++：map
来源：http://lpb.sweek.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dlo.xinyue.icu

[S36] C++：unordered_map
来源：http://mzd.zdqjudy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://oik.zhengqikj.top

[S37] C++：set
来源：http://ccl.zhoulong.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://oeq.wangshuangyany.cn

[S38] C++：排序
来源：http://kna.hammf.cn

std::sort(v.begin(), v.end());
来源：http://cpg.9152youxi.cn

[S39] C++：自定义比较器排序
来源：http://wwk.epnwcf.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lpv.xziqi.cn

[S40] C++：查找元素
来源：http://bhk.hesvh.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rrj.birdmap.top

[S41] C++：类与构造函数
来源：http://brm.tianlin.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nel.haohaochexian.top

[S42] C++：继承与虚函数
来源：http://zhr.hnqzz.top

class B : public Base { public: void f() override {} };
来源：http://ggr.yj202588.top

[S43] C++：智能指针
来源：http://ssw.zhiwuduotai.top

auto p = std::make_unique<int>(5);
来源：http://fkv.gaohongyu789.top

[S44] C++：引用传参
来源：http://vnh.sxryk.cn

void inc(int &x) { ++x; }
来源：http://emz.zhongyouzk.top

[S45] C++：lambda
来源：http://xzd.yonumen.top

auto add = [](int a, int b) { return a + b; };
来源：http://vfc.andypj.xyz

[S46] C++：函数模板
来源：http://hxr.cashguo.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lnt.gotoacloud.top

[S47] C++：结构化绑定遍历
来源：http://vna.yuxming.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://sas.daxiang520.top

[S48] C++：逐行读文件
来源：http://akc.aizwys.cn

std::ifstream in("a.txt");  std::string line;
来源：http://exy.xylfe.cn

while (std::getline(in, line)) { }
来源：http://kfs.zhixingplan.top

[S49] C++：写文件
来源：http://azo.cashguo.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ccx.svipenyu.cn

[S50] C++：格式化数字
来源：http://jqi.jqgufenzy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yon.jinghuilouyu.cn

[S51] C++：显式类型转换
来源：http://tsp.jqgufenzy.top

static_cast<double>(a) / b
来源：http://kzu.9152youxi.cn

[S52] C++：const 与 noexcept
来源：http://rps.meibo888.top

int size() const noexcept { return n_; }
来源：http://kev.wangshuangyany.cn

[S53] C++：移动语义
来源：http://ith.nwbrower.top

std::vector<int> w = std::move(v);
来源：http://iwh.cashguo.top

[S54] C++：异常处理
来源：http://dog.nwbrower.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://okv.ehwqpu.com

[S55] C++：结构化绑定
来源：http://njp.ivvv.top

auto [a, b] = std::make_pair(1, 2);
来源：http://nqn.yfazqb.com

[S56] C++：optional
来源：http://ysc.shangyingyoupin.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://djx.zycfv.cn

[S57] C++：编译期常量
来源：http://xcj.hfpthk.cn

constexpr int N = 10;
来源：http://pxu.mhx1999.top

[S58] C++：命名空间
来源：http://kzb.jianghu66.top

namespace ns { int f() { return 1; } }
来源：http://mbl.chenlongwang.top

[S59] C++：静态断言
来源：http://jzw.chenlongwang.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lrs.yangfankeji.com

[S60] C++：遍历并删除元素
来源：http://tqj.ywan-chungtsiang.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://muo.haohaochexian.top

================================================================================
来源：http://qfa.jqgfzy.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://trl.zhoulong.xyz

================================================================================
来源：http://vnv.ivvv.top

[T01] Kotlin：Hello World
来源：http://ift.dianchejie.cn

println("Hello")
来源：http://vrm.daxiang520.top

[T02] Kotlin：变量
来源：http://hkr.zhengqikj.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hmc.guowangkeji.top

[T03] Kotlin：字符串模板
来源：http://gli.hnqzz.top

"值: $b"
来源：http://say.ybcxt.top

[T04] Kotlin：空安全
来源：http://ite.iojbl.cn

val n: String? = null;  n?.length
来源：http://wfi.hywenlv.cn


<!-- 参考信息 -->