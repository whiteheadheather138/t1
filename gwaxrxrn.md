代发 wailian999

readonly PI=3.14
来源：http://mzk.c1oappe.top

[R04] 位置参数
来源：http://cdi.nanxuanxn.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://osq.svipenyu.cn

[R05] 参数默认值
来源：http://ula.yanxiufei.cn

name="${1:-default}"
来源：http://gsm.vehdjk.com

[R06] 判断命令是否存在
来源：http://feg.tanke756.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ghm.zhongyouzk.top

[R07] if 判断文件
来源：http://ylu.birdmap.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tpj.aizwys.cn

[R08] 数值比较
来源：http://rmh.mhx1999.top

if (( a > b )); then echo "a 更大"; fi
来源：http://eoi.shanyushiyangkeji.top

[R09] 字符串比较
来源：http://nhs.jinqigfzy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://szh.pycfn.com

[R10] 正则匹配
来源：http://sea.shanyushiyangkeji.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://oij.hammf.cn

[R11] case 多分支
来源：http://heg.redwolf501.top

case "$1" in
来源：http://gtj.sysykeji.top

start) echo "启动" ;;
来源：http://key.mhx1999.top

stop)  echo "停止" ;;
来源：http://xtp.shzxlz.cn

*)     echo "未知命令" ;;
来源：http://itt.fzhhl.top

esac
来源：http://hgh.wangshuangyany.cn

[R12] for 遍历文件
来源：http://hnv.xziqi.cn

for f in *.txt; do echo "$f"; done
来源：http://gbu.yj20258888.top

[R13] for 计数循环
来源：http://byo.ehwqpu.com

for i in {1..10}; do echo "$i"; done
来源：http://ndf.yj20258888.top

[R14] C 风格 for
来源：http://utv.yj20258.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qwc.yj20258888.top

[R15] while 逐行读文件
来源：http://drl.pycfn.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ozn.shangyingyoupin.top

[R16] until 等待条件
来源：http://imo.ybcxt.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://abq.hywenlv.cn

[R17] 数组定义与取值
来源：http://lpy.fanxiaobao.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://nos.fanxiaobao.xyz

[R18] 遍历数组
来源：http://ymr.jlsjyb.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ltb.epnwcf.com

[R19] 数组长度
来源：http://kxz.cashguo.top

echo "${#arr[@]}"
来源：http://all.guannengcc.top

[R20] 关联数组（字典）
来源：http://wjk.ydzc1.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ppw.andypj.xyz

[R21] 字符串长度
来源：http://wfm.zdbjq.cn

echo "${#s}"
来源：http://jsg.yuxming.cn

[R22] 截取子串
来源：http://sml.kuanghao11.cn

echo "${s:0:5}"
来源：http://mqv.fzhhl.top

[R23] 字符串替换
来源：http://ilt.zycfv.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hbc.gzhubu.top

[R24] 大小写转换
来源：http://jkb.tanke756.top

echo "${s^^}"; echo "${s,,}"
来源：http://mhf.guowangkeji.top

[R25] 去后缀 / 去前缀
来源：http://ccc.yueranfly.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://cuw.cucudq.cn

[R26] 命令替换
来源：http://lqn.zdqjudy.top

now=$(date +%F); echo "$now"
来源：http://qqn.yongpay.top

[R27] 算术展开
来源：http://kid.jinghuilouyu.cn

echo $((1 + 2 * 3))
来源：http://fke.xingfuxueyuan.xyz

[R28] 浮点运算
来源：http://qyp.yonumen.top

echo "scale=2; 10/3" | bc
来源：http://jis.kuanghao11.cn

[R29] 定义函数
来源：http://zig.zhaomingkeji.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ddu.tanke756.top

[R30] 函数返回状态码
来源：http://iub.gzhubu.top

f() { return 0; }; f || echo "失败了"
来源：http://crc.0kj1m.cn

[R31] 局部变量
来源：http://oao.jyoumei.cn

f() { local x=1; echo "$x"; }
来源：http://kab.daria6918.cn

[R32] 参数个数校验
来源：http://ohg.andypj.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dna.ivvv.top

[R33] 捕获错误并提示行号
来源：http://kux.cheryme.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yif.cdnleiting.top

[R34] 退出时清理
来源：http://oqh.sufxvd.cn

trap 'rm -f "$tmp"' EXIT
来源：http://egu.fengsongda.top

[R35] 后台执行并等待
来源：http://vvk.aizwys.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://scc.jiagoushi.top

[R36] 并发执行多个任务
来源：http://iuo.vehdjk.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ani.birdmap.top

[R37] 把输出赋给变量
来源：http://wdo.hfpthk.cn

files=$(ls -1)
来源：http://fxv.zdbjq.cn

[R38] 管道串联
来源：http://pvf.hongshengwenyu.top

cat a.txt | grep -i error | wc -l
来源：http://tjr.tanke756.top

[R39] 重定向标准输出与错误
来源：http://qfq.yj20258888.top

cmd > out.log 2>&1
来源：http://ijz.fengsongda.top

[R40] 追加写日志
来源：http://kun.hcnkem.com

echo "log" >> out.log
来源：http://kmw.daxiang520.top

[R41] 丢弃输出
来源：http://btr.316326.xyz

cmd >/dev/null 2>&1
来源：http://pxd.zdbjq.cn

[R42] 输入重定向
来源：http://aor.xuetiantiany.cn

wc -l < a.txt
来源：http://xnf.svipenyu.cn

[R43] 按名字查找文件
来源：http://ouj.sxryk.cn

find . -name "*.log" -type f
来源：http://jvl.kuanghao11.cn

[R44] 按修改时间查找
来源：http://xbs.sysykeji.top

find . -mtime -7 -type f
来源：http://isu.yuanzhike.top

[R45] 批量删除
来源：http://tqs.shangyingyoupin.top

find . -name "*.tmp" -delete
来源：http://lsd.redwolf501.top

[R46] 递归替换文件内容
来源：http://nxv.zhijiandao.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://csg.aibaodan.cn

[R47] sed 单行替换
来源：http://ycx.chenjidiqi.icu

sed -i 's/foo/bar/g' a.txt
来源：http://tic.ybcxt.top

[R48] awk 取指定列
来源：http://eri.hywenlv.cn

awk '{print $1, $3}' a.txt
来源：http://ilx.shanyushiyangkeji.top

[R49] awk 带条件
来源：http://qct.jinyuanbaomall.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gqr.ppjwa.cn

[R50] awk 求和
来源：http://qqo.uphjek.com

awk '{s += $2} END {print s}' a.txt
来源：http://nxg.sjlbkw.cn

[R51] 排序去重取前几
来源：http://taz.hywenlv.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xco.andypj.xyz

[R52] 统计行数
来源：http://kix.yj20258888.top

wc -l a.txt
来源：http://zqh.hnxiangtu.top

[R53] 查看文件头与实时尾
来源：http://trl.ydjk.org.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://aqq.nanxuanxn.top

[R54] 比较两个文件
来源：http://gyy.hammf.cn

diff a.txt b.txt
来源：http://neu.nwbrower.top

[R55] 压缩与解压
来源：http://ksw.jqgfzy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://avr.ydjk.org.cn

[R56] 远程拷贝
来源：http://zpo.fktsv.cn

scp file user@host:/path/
来源：http://tug.feifeiyinyue.top

[R57] 远程执行命令
来源：http://uud.xuetiantiany.cn

ssh user@host 'uptime'
来源：http://czx.zycfv.cn

[R58] 下载文件
来源：http://kwt.haohaochexian.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wmf.hywenlv.cn

[R59] 发 POST JSON
来源：http://meo.xuetiantiany.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gai.fengsongda.top

[R60] 只看 HTTP 状态码
来源：http://mdj.ivvv.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ipq.shuidangran.top

[R61] 磁盘占用
来源：http://mlg.haohaochexian.top

df -h;  du -sh *
来源：http://xnt.52xcode.cn

[R62] 找最占空间的文件
来源：http://ehe.yueranfly.top

du -ah . | sort -rh | head -10
来源：http://lya.yj20258888.top

[R63] 内存与进程
来源：http://qnr.jyoumei.cn

free -h;  ps aux | grep nginx
来源：http://qtq.wangdashe.top

[R64] 结束进程
来源：http://zss.yj20258888.top

kill -9 $(pgrep -f app.py)
来源：http://dpe.hnxiangtu.top

[R65] 查看端口占用
来源：http://rdp.ctjpmb.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://txc.yongpay.top

[R66] 定时任务
来源：http://ubx.hywenlv.cn

crontab -e;  crontab -l
来源：http://txq.hammf.cn

[R67] 生成随机十六进制串
来源：http://sre.jqgufenzy.top

openssl rand -hex 16
来源：http://nhp.zhijiandao.cn

[R68] 计算文件校验值
来源：http://udf.cashguo.top

sha256sum a.txt;  md5sum a.txt
来源：http://vwh.jlsjyb.cn

[R69] 生成随机密码
来源：http://xqp.pycfn.com

head -c 16 /dev/urandom | base64
来源：http://fkx.hammf.cn

[R70] 时间戳与互转
来源：http://vnm.dashuyun.cn

date +%s;  date -d @1700000000
来源：http://dle.hnxiangtu.top

[R71] 日期格式化
来源：http://bag.guowangkeji.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://owr.xuetiantiany.cn

[R72] 等待端口就绪
来源：http://hmt.tian-w.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://etf.tarul.cn

[R73] 分割大日志
来源：http://hdj.zhoulong.xyz

split -l 1000 big.log part_
来源：http://kks.cashguo.top

[R74] 批量重命名
来源：http://ryh.wangdashe.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qct.xuanzx.com

[R75] 导出环境变量
来源：http://zpn.nanxuanxn.top

export PATH="$HOME/bin:$PATH"
来源：http://tmr.daxiang520.top

[R76] 使用临时文件
来源：http://isu.ppjwa.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://olg.gaohongyu789.top

[R77] 读取用户输入
来源：http://hjd.vqdsnc.cn

read -rp "请输入: " ans
来源：http://hsj.redwolf501.top

[R78] 交互式菜单
来源：http://btm.jinqigufen.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ytq.dashuyun.cn

[R79] 解析命令行选项
来源：http://khd.shanyushiyangtech.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ued.nanxuanxn.top

[R80] 查看脚本执行耗时
来源：http://qpf.xingfuxueyuan.xyz

time ./run.sh
来源：http://vab.bbcook.cn

================================================================================
来源：http://sgk.gaohongyu789.top

S. C / C++ 专题
来源：http://zed.yanxiufei.cn

================================================================================
来源：http://cwu.vehdjk.com

[S01] C：Hello World
来源：http://jfz.jinyuanbaomall.cn

#include <stdio.h>
来源：http://sim.jiagoushi.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://cad.birdmap.top

[S02] C：变量与格式化输出
来源：http://swy.shuidangran.top

int a = 10; printf("%d\n", a);
来源：http://kfv.xinyue.icu

[S03] C：读入整数
来源：http://cee.nanxinkj.top

int x; scanf("%d", &x);
来源：http://vvo.fktsv.cn

[S04] C：字符串复制
来源：http://slq.yangfankeji.com

char dst[32]; strcpy(dst, "hi");
来源：http://fub.cheryme.top

[S05] C：字符串长度
来源：http://jij.xuetiantiany.cn

strlen(s)
来源：http://iyt.fanxiaobao.xyz

[S06] C：字符串比较
来源：http://vqr.yonumen.top

strcmp(a, b) == 0
来源：http://bal.shanyushiyangkeji.top

[S07] C：数组遍历求和
来源：http://ydj.chenzaomai.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wvg.zhijiandao.cn

[S08] C：动态内存分配与释放
来源：http://fss.smart0.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wzm.ybcxt.top

[S09] C：结构体定义与初始化
来源：http://hnk.guowangkeji.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jsj.sweek.top

[S10] C：指针与解引用
来源：http://dvs.hcnkem.com

int *p = &a;  *p = 5;
来源：http://zhs.ydjk.org.cn

[S11] C：逐行读文件
来源：http://zgx.zhengqikj.top

FILE *f = fopen("a.txt", "r");
来源：http://yzn.xinyue.icu

while (fgets(buf, sizeof buf, f)) { }
来源：http://txp.zhaomingkeji.xyz

fclose(f);
来源：http://kit.ivvv.top

[S12] C：写文件
来源：http://tqy.c1oappe.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://beq.cheryme.top

[S13] C：宏定义
来源：http://vyl.yueranfly.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://izu.tian-w.cn

[S14] C：枚举
来源：http://ljh.nanxuanxn.top

enum Color { RED, GREEN, BLUE };
来源：http://cgp.iojbl.cn

[S15] C：类型转换
来源：http://fpl.kuanghao11.cn

(double) a / b
来源：http://fgj.xziqi.cn

[S16] C：位操作置位
来源：http://vse.zhijiandao.cn

x |= (1 << 3);
来源：http://ftb.nwbrower.top

[S17] C：安全拼接字符串
来源：http://vjk.tian-w.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ijz.birdmap.top

[S18] C：命令行参数
来源：http://ubq.dashuyun.cn

int main(int argc, char **argv)
来源：http://kjz.hcnkem.com

[S19] C：快速排序
来源：http://nfp.zdbjq.cn

qsort(a, n, sizeof(int), cmp);
来源：http://mul.tanke756.top

[S20] C：二分查找
来源：http://nqf.gogol.net.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wdf.bjfxy.top

[S21] C：字符类别判断
来源：http://arz.hcnkem.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://uvi.ivvv.top

[S22] C：字符串转数字
来源：http://mdl.vehdjk.com

atoi("42");  strtod("3.14", NULL);
来源：http://qel.yangfankeji.com

[S23] C：随机数
来源：http://lys.zycfv.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://opw.shanyushiyangtech.top

[S24] C：获取本地时间
来源：http://mtl.redwolf501.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://swt.snrcjt.cn

[S25] C：内存拷贝
来源：http://yul.ydjk.org.cn

memcpy(dst, src, n);
来源：http://ffi.cucudq.cn

[S26] C：内存清零
来源：http://svj.xziqi.cn

memset(a, 0, sizeof a);
来源：http://fsi.aizwys.cn

[S27] C：定义常量
来源：http://xno.52xcode.cn

const double PI = 3.14159;
来源：http://opt.shzxlz.cn

[S28] C：静态变量
来源：http://zrx.daxiang520.top

static int counter = 0;
来源：http://mzg.guannengcc.top

[S29] C：变参函数
来源：http://dmm.hcnkem.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ywa.aibaodan.cn

[S30] C：头文件保护
来源：http://mdn.yueranfly.top

#ifndef X_H
来源：http://qkm.gaohongyu789.top

#define X_H
来源：http://ena.hnqzz.top

#endif
来源：http://szp.sjlbkw.cn

[S31] C++：Hello World
来源：http://trp.zycfv.cn

#include <iostream>
来源：http://dcl.sjlbkw.cn

int main() { std::cout << "Hello\n"; }
来源：http://gbk.zhiwuduotai.top

[S32] C++：字符串
来源：http://hcz.hnxiangtu.top

std::string s = "hi";  s += "!";
来源：http://owv.sufxvd.cn

[S33] C++：vector 增删
来源：http://hmm.daxiang520.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://evr.zhiwuduotai.top

[S34] C++：遍历 vector
来源：http://lli.jinqigfzy.top

for (auto &x : v) { std::cout << x; }
来源：http://sjz.tanke756.top

[S35] C++：map
来源：http://mbo.smart0.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vls.dianchejie.cn

[S36] C++：unordered_map
来源：http://myc.chenzaomai.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ezo.bbcook.cn

[S37] C++：set
来源：http://bqb.jlsjyb.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zrz.sweek.top

[S38] C++：排序
来源：http://dem.pengpengdd.cyou

std::sort(v.begin(), v.end());
来源：http://hqk.jqgfzy.top

[S39] C++：自定义比较器排序
来源：http://rgd.ybcxt.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nlr.yueranfly.top

[S40] C++：查找元素
来源：http://dqp.sufxvd.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ohm.chenlongwang.top

[S41] C++：类与构造函数
来源：http://qbi.zhiwuduotai.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://elo.yueranfly.top

[S42] C++：继承与虚函数
来源：http://xqw.fengsongda.top

class B : public Base { public: void f() override {} };
来源：http://edd.yangfankeji.com

[S43] C++：智能指针
来源：http://sny.hywenlv.cn

auto p = std::make_unique<int>(5);
来源：http://ikn.svipenyu.cn

[S44] C++：引用传参
来源：http://qom.9152youxi.cn

void inc(int &x) { ++x; }
来源：http://ttr.aizwys.cn

[S45] C++：lambda
来源：http://iha.snrcjt.cn

auto add = [](int a, int b) { return a + b; };
来源：http://tok.zhijiandao.cn

[S46] C++：函数模板
来源：http://goj.feifeiyinyue.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://isi.zycfv.cn

[S47] C++：结构化绑定遍历
来源：http://uca.yfazqb.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://oup.hongshengwenyu.top

[S48] C++：逐行读文件
来源：http://nzh.epnwcf.com

std::ifstream in("a.txt");  std::string line;
来源：http://gux.uphjek.com

while (std::getline(in, line)) { }
来源：http://tex.nanxinkj.top

[S49] C++：写文件
来源：http://kfm.yj20258888.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hks.jiagoushi.top

[S50] C++：格式化数字
来源：http://sjn.yj20258.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://len.zhijiandao.cn

[S51] C++：显式类型转换
来源：http://dgh.zhengqikj.top

static_cast<double>(a) / b
来源：http://yig.birdmap.top

[S52] C++：const 与 noexcept
来源：http://fzp.chenzaomai.com

int size() const noexcept { return n_; }
来源：http://laa.yangfankeji.com

[S53] C++：移动语义
来源：http://yup.bbcook.cn

std::vector<int> w = std::move(v);
来源：http://zhx.yj202588.top

[S54] C++：异常处理
来源：http://yei.gzhubu.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yax.guannengcc.top

[S55] C++：结构化绑定
来源：http://arf.jiagoushi.top

auto [a, b] = std::make_pair(1, 2);
来源：http://bhp.zdbjq.cn

[S56] C++：optional
来源：http://byc.yj20258.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nep.sweek.top

[S57] C++：编译期常量
来源：http://ohy.yangfankeji.com

constexpr int N = 10;
来源：http://hjw.ivvv.top

[S58] C++：命名空间
来源：http://you.dashuyun.cn

namespace ns { int f() { return 1; } }
来源：http://ypy.svipenyu.cn

[S59] C++：静态断言
来源：http://pri.shangyingyoupin.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://itr.sjlbkw.cn

[S60] C++：遍历并删除元素
来源：http://qno.yangfankeji.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://olc.zhoulong.xyz

================================================================================
来源：http://njk.mhx1999.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tbh.xuanzx.com

================================================================================
来源：http://dau.zdbjq.cn

[T01] Kotlin：Hello World
来源：http://igh.shzxlz.cn

println("Hello")
来源：http://fpy.meibo888.top

[T02] Kotlin：变量
来源：http://kou.hfpthk.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://anw.ydjk.org.cn

[T03] Kotlin：字符串模板
来源：http://ske.chenjidiqi.icu

"值: $b"
来源：http://irz.ydjk.org.cn

[T04] Kotlin：空安全
来源：http://sjz.zhixingplan.top

val n: String? = null;  n?.length
来源：http://qoc.daxiang520.top


<!-- 参考信息 -->