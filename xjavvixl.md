代发 wailian999

readonly PI=3.14
来源：http://xxs.gaohongyu789.top

[R04] 位置参数
来源：http://iex.shangyingyoupin.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://diz.ppjwa.cn

[R05] 参数默认值
来源：http://fdr.hywenlv.cn

name="${1:-default}"
来源：http://cpg.52xcode.cn

[R06] 判断命令是否存在
来源：http://bzk.quarkkingdee.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cqw.sxryk.cn

[R07] if 判断文件
来源：http://hpt.cqqwz.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wbp.yanxiufei.cn

[R08] 数值比较
来源：http://fig.cucudq.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://pei.bjfxy.top

[R09] 字符串比较
来源：http://jli.yfazqb.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zep.fengsongda.top

[R10] 正则匹配
来源：http://hyv.316326.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jrs.meibo888.top

[R11] case 多分支
来源：http://qlv.quarkkingdee.top

case "$1" in
来源：http://viw.ydzc1.top

start) echo "启动" ;;
来源：http://iec.jqgfzy.top

stop)  echo "停止" ;;
来源：http://nnv.fehbvm.com

*)     echo "未知命令" ;;
来源：http://saf.hongshengwenyu.top

esac
来源：http://sdf.hongshengwenyu.top

[R12] for 遍历文件
来源：http://car.yanxiufei.cn

for f in *.txt; do echo "$f"; done
来源：http://oye.jinqigufen.top

[R13] for 计数循环
来源：http://oan.ppjwa.cn

for i in {1..10}; do echo "$i"; done
来源：http://ruc.meibo888.top

[R14] C 风格 for
来源：http://cqy.fehbvm.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dpj.tianlin.xyz

[R15] while 逐行读文件
来源：http://fyf.shanyushiyangkeji.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://aap.wangshuangyany.cn

[R16] until 等待条件
来源：http://bzm.uphjek.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dcu.chenzaomai.com

[R17] 数组定义与取值
来源：http://hka.cqqwz.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ufv.cucudq.cn

[R18] 遍历数组
来源：http://ncl.yonumen.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://iiw.pycfn.com

[R19] 数组长度
来源：http://dlx.jlsjyb.cn

echo "${#arr[@]}"
来源：http://ctp.yj20258888.top

[R20] 关联数组（字典）
来源：http://sic.hesvh.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://uvp.fzhhl.top

[R21] 字符串长度
来源：http://xnq.ctjpmb.com

echo "${#s}"
来源：http://ppo.gaohongyu789.top

[R22] 截取子串
来源：http://fkl.cashguo.top

echo "${s:0:5}"
来源：http://mzv.chenjidiqi.icu

[R23] 字符串替换
来源：http://yky.yonumen.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pav.aizwys.cn

[R24] 大小写转换
来源：http://swa.cqqwz.cn

echo "${s^^}"; echo "${s,,}"
来源：http://cmc.gzhubu.top

[R25] 去后缀 / 去前缀
来源：http://auu.jqgfzy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://hrl.zhijiandao.cn

[R26] 命令替换
来源：http://fzl.xuetiantiany.cn

now=$(date +%F); echo "$now"
来源：http://nrd.yueranfly.top

[R27] 算术展开
来源：http://dag.kuanghao11.cn

echo $((1 + 2 * 3))
来源：http://xtv.smart0.xyz

[R28] 浮点运算
来源：http://mkr.pengpengdd.cyou

echo "scale=2; 10/3" | bc
来源：http://max.fzhhl.top

[R29] 定义函数
来源：http://qjw.aibaodan.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xnb.yueranfly.top

[R30] 函数返回状态码
来源：http://lha.hnqzz.top

f() { return 0; }; f || echo "失败了"
来源：http://ogy.aibaodan.cn

[R31] 局部变量
来源：http://szg.vehdjk.com

f() { local x=1; echo "$x"; }
来源：http://byv.cucudq.cn

[R32] 参数个数校验
来源：http://srl.vqdsnc.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ozb.chenzaomai.com

[R33] 捕获错误并提示行号
来源：http://zca.cashguo.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hif.yangfankeji.com

[R34] 退出时清理
来源：http://kgh.yonumen.top

trap 'rm -f "$tmp"' EXIT
来源：http://uee.ctjpmb.com

[R35] 后台执行并等待
来源：http://qmf.yanxiufei.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://mri.nanxuanxn.top

[R36] 并发执行多个任务
来源：http://mpc.aibaodan.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bgr.pycfn.com

[R37] 把输出赋给变量
来源：http://bxt.cashguo.top

files=$(ls -1)
来源：http://pqd.vqdsnc.cn

[R38] 管道串联
来源：http://xwe.yuanzhike.top

cat a.txt | grep -i error | wc -l
来源：http://mig.vqdsnc.cn

[R39] 重定向标准输出与错误
来源：http://ppr.chenjidiqi.icu

cmd > out.log 2>&1
来源：http://moq.hfpthk.cn

[R40] 追加写日志
来源：http://nej.chenjidiqi.icu

echo "log" >> out.log
来源：http://wbu.0kj1m.cn

[R41] 丢弃输出
来源：http://ffa.jinqigfzy.top

cmd >/dev/null 2>&1
来源：http://gmx.9152youxi.cn

[R42] 输入重定向
来源：http://xoc.hnqzz.top

wc -l < a.txt
来源：http://gwn.fehbvm.com

[R43] 按名字查找文件
来源：http://wga.52xcode.cn

find . -name "*.log" -type f
来源：http://fpv.shanyushiyangkeji.top

[R44] 按修改时间查找
来源：http://kuk.yj202588.top

find . -mtime -7 -type f
来源：http://glk.hysaishi.cn

[R45] 批量删除
来源：http://kor.wangdashe.top

find . -name "*.tmp" -delete
来源：http://vmt.bbcook.cn

[R46] 递归替换文件内容
来源：http://jtv.snrcjt.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dvf.kuanghao11.cn

[R47] sed 单行替换
来源：http://xdp.yfazqb.com

sed -i 's/foo/bar/g' a.txt
来源：http://dsp.zhixingplan.top

[R48] awk 取指定列
来源：http://jaa.ctjpmb.com

awk '{print $1, $3}' a.txt
来源：http://cbl.guannengcc.top

[R49] awk 带条件
来源：http://mgh.wangshuangyany.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://uej.zdbjq.cn

[R50] awk 求和
来源：http://cva.fengsongda.top

awk '{s += $2} END {print s}' a.txt
来源：http://qev.redwolf501.top

[R51] 排序去重取前几
来源：http://qnq.xuetiantiany.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://vdt.feifeiyinyue.top

[R52] 统计行数
来源：http://pzl.52xcode.cn

wc -l a.txt
来源：http://qxx.zhiwuduotai.top

[R53] 查看文件头与实时尾
来源：http://xoo.uphjek.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ptq.tarul.cn

[R54] 比较两个文件
来源：http://ybr.wangshuangyany.cn

diff a.txt b.txt
来源：http://hbw.hammf.cn

[R55] 压缩与解压
来源：http://ned.xingfuxueyuan.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vqf.uphjek.com

[R56] 远程拷贝
来源：http://nxn.jinqigufen.top

scp file user@host:/path/
来源：http://fml.bbcook.cn

[R57] 远程执行命令
来源：http://vws.xziqi.cn

ssh user@host 'uptime'
来源：http://jko.hywenlv.cn

[R58] 下载文件
来源：http://uhn.xziqi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://iqw.jlsjyb.cn

[R59] 发 POST JSON
来源：http://ifm.zhaomingkeji.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xcc.9152youxi.cn

[R60] 只看 HTTP 状态码
来源：http://skr.daxiang520.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://doq.ctjpmb.com

[R61] 磁盘占用
来源：http://oae.316326.xyz

df -h;  du -sh *
来源：http://psw.xuetiantiany.cn

[R62] 找最占空间的文件
来源：http://bqo.jianghu66.top

du -ah . | sort -rh | head -10
来源：http://djl.xinyue.icu

[R63] 内存与进程
来源：http://asg.ybcxt.top

free -h;  ps aux | grep nginx
来源：http://wyl.tian-w.cn

[R64] 结束进程
来源：http://rfb.cqqwz.cn

kill -9 $(pgrep -f app.py)
来源：http://qlg.yfazqb.com

[R65] 查看端口占用
来源：http://sjj.0kj1m.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://iyn.ehwqpu.com

[R66] 定时任务
来源：http://qah.hnqzz.top

crontab -e;  crontab -l
来源：http://ebk.bbcook.cn

[R67] 生成随机十六进制串
来源：http://stf.snrcjt.cn

openssl rand -hex 16
来源：http://nuy.xylfe.cn

[R68] 计算文件校验值
来源：http://xvh.zhijiandao.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xdh.hcnkem.com

[R69] 生成随机密码
来源：http://odi.ywan-chungtsiang.top

head -c 16 /dev/urandom | base64
来源：http://hkt.ivvv.top

[R70] 时间戳与互转
来源：http://qcw.cashguo.top

date +%s;  date -d @1700000000
来源：http://bmv.316326.xyz

[R71] 日期格式化
来源：http://edo.sweek.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://wmn.nanxuanxn.top

[R72] 等待端口就绪
来源：http://gyp.jyoumei.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fpi.bjfxy.top

[R73] 分割大日志
来源：http://jgv.feifeiyinyue.top

split -l 1000 big.log part_
来源：http://ufd.daxiang520.top

[R74] 批量重命名
来源：http://rvj.hnqzz.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bam.zhiwuduotai.top

[R75] 导出环境变量
来源：http://dgo.xylfe.cn

export PATH="$HOME/bin:$PATH"
来源：http://evg.zhengqikj.top

[R76] 使用临时文件
来源：http://the.gogol.net.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://uqc.daxiang520.top

[R77] 读取用户输入
来源：http://vsc.ehwqpu.com

read -rp "请输入: " ans
来源：http://zeu.chenjidiqi.icu

[R78] 交互式菜单
来源：http://wou.fengsongda.top

select opt in a b c; do echo "$opt"; break; done
来源：http://qyy.yj20258.top

[R79] 解析命令行选项
来源：http://epz.yuanzhike.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ebl.jqgufenzy.top

[R80] 查看脚本执行耗时
来源：http://ont.cucudq.cn

time ./run.sh
来源：http://dli.hongshengwenyu.top

================================================================================
来源：http://fil.zhijiandao.cn

S. C / C++ 专题
来源：http://uru.jianghu66.top

================================================================================
来源：http://qld.zhijiandao.cn

[S01] C：Hello World
来源：http://bxs.yuanzhike.top

#include <stdio.h>
来源：http://tec.mhx1999.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://gfm.fzhhl.top

[S02] C：变量与格式化输出
来源：http://rpr.dianchejie.cn

int a = 10; printf("%d\n", a);
来源：http://zmg.zhongyouzk.top

[S03] C：读入整数
来源：http://hks.zhoulong.xyz

int x; scanf("%d", &x);
来源：http://qvc.uphjek.com

[S04] C：字符串复制
来源：http://fyq.aibaodan.cn

char dst[32]; strcpy(dst, "hi");
来源：http://qgt.snrcjt.cn

[S05] C：字符串长度
来源：http://cjy.aizwys.cn

strlen(s)
来源：http://jla.shangyingyoupin.top

[S06] C：字符串比较
来源：http://cga.shanyushiyangtech.top

strcmp(a, b) == 0
来源：http://dmj.bjfxy.top

[S07] C：数组遍历求和
来源：http://ybs.zhiwuduotai.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gek.zhengqikj.top

[S08] C：动态内存分配与释放
来源：http://uja.xuetiantiany.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ksj.ydzc1.top

[S09] C：结构体定义与初始化
来源：http://ejd.hcnkem.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ipo.xylfe.cn

[S10] C：指针与解引用
来源：http://jyv.cdnleiting.top

int *p = &a;  *p = 5;
来源：http://tke.jqgufenzy.top

[S11] C：逐行读文件
来源：http://fcc.jiagoushi.top

FILE *f = fopen("a.txt", "r");
来源：http://dvd.ywan-chungtsiang.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://hcw.fengsongda.top

fclose(f);
来源：http://fyq.smart0.xyz

[S12] C：写文件
来源：http://yml.nanxinkj.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lri.sxryk.cn

[S13] C：宏定义
来源：http://uhd.meibo888.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lwn.zycfv.cn

[S14] C：枚举
来源：http://mef.zhaomingkeji.xyz

enum Color { RED, GREEN, BLUE };
来源：http://vui.zycfv.cn

[S15] C：类型转换
来源：http://abo.hesvh.cn

(double) a / b
来源：http://sto.zycfv.cn

[S16] C：位操作置位
来源：http://bmh.fzhhl.top

x |= (1 << 3);
来源：http://esl.daria6918.cn

[S17] C：安全拼接字符串
来源：http://zls.tian-w.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kor.hammf.cn

[S18] C：命令行参数
来源：http://ssk.yanxiufei.cn

int main(int argc, char **argv)
来源：http://qmp.nwbrower.top

[S19] C：快速排序
来源：http://yeg.hnqzz.top

qsort(a, n, sizeof(int), cmp);
来源：http://fwb.meibo888.top

[S20] C：二分查找
来源：http://weh.feifeiyinyue.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cra.hammf.cn

[S21] C：字符类别判断
来源：http://vva.jiagoushi.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vha.haohaochexian.top

[S22] C：字符串转数字
来源：http://yis.yuanzhike.top

atoi("42");  strtod("3.14", NULL);
来源：http://qaw.cheryme.top

[S23] C：随机数
来源：http://sku.redwolf501.top

srand(time(NULL));  int r = rand() % 100;
来源：http://vzi.ppjwa.cn

[S24] C：获取本地时间
来源：http://pre.jyoumei.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cts.cucudq.cn

[S25] C：内存拷贝
来源：http://oqb.hywenlv.cn

memcpy(dst, src, n);
来源：http://fnd.yfazqb.com

[S26] C：内存清零
来源：http://rko.nanxuanxn.top

memset(a, 0, sizeof a);
来源：http://azf.fehbvm.com

[S27] C：定义常量
来源：http://mis.pycfn.com

const double PI = 3.14159;
来源：http://rqt.kuanghao11.cn

[S28] C：静态变量
来源：http://bkk.hcnkem.com

static int counter = 0;
来源：http://oqk.sufxvd.cn

[S29] C：变参函数
来源：http://jum.mhx1999.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://swl.fanxiaobao.xyz

[S30] C：头文件保护
来源：http://yuv.guannengcc.top

#ifndef X_H
来源：http://bhq.mhx1999.top

#define X_H
来源：http://zsm.jinyuanbaomall.cn

#endif
来源：http://jre.fengsongda.top

[S31] C++：Hello World
来源：http://leh.guannengcc.top

#include <iostream>
来源：http://mya.shangyingyoupin.top

int main() { std::cout << "Hello\n"; }
来源：http://yxy.andypj.xyz

[S32] C++：字符串
来源：http://ktv.fktsv.cn

std::string s = "hi";  s += "!";
来源：http://cnt.svipenyu.cn

[S33] C++：vector 增删
来源：http://nnv.smart0.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://awa.cucudq.cn

[S34] C++：遍历 vector
来源：http://bzg.sysykeji.top

for (auto &x : v) { std::cout << x; }
来源：http://mhn.meibo888.top

[S35] C++：map
来源：http://sqk.zhongyouzk.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tyy.zycfv.cn

[S36] C++：unordered_map
来源：http://ypo.quarkkingdee.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yiu.redwolf501.top

[S37] C++：set
来源：http://mmp.gzhubu.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rmp.tianlin.xyz

[S38] C++：排序
来源：http://hpx.pengpengdd.cyou

std::sort(v.begin(), v.end());
来源：http://bst.jqgufenzy.top

[S39] C++：自定义比较器排序
来源：http://hev.gogol.net.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qdu.andypj.xyz

[S40] C++：查找元素
来源：http://ygy.bjfxy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ify.feifeiyinyue.top

[S41] C++：类与构造函数
来源：http://snz.c1oappe.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fpv.redwolf501.top

[S42] C++：继承与虚函数
来源：http://dah.jiagoushi.top

class B : public Base { public: void f() override {} };
来源：http://gpn.316326.xyz

[S43] C++：智能指针
来源：http://zkl.chenzaomai.com

auto p = std::make_unique<int>(5);
来源：http://teu.gzhubu.top

[S44] C++：引用传参
来源：http://brj.birdmap.top

void inc(int &x) { ++x; }
来源：http://pxl.cheryme.top

[S45] C++：lambda
来源：http://pja.chenlongwang.top

auto add = [](int a, int b) { return a + b; };
来源：http://olf.ydjk.org.cn

[S46] C++：函数模板
来源：http://fje.zhiwuduotai.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bgp.cheryme.top

[S47] C++：结构化绑定遍历
来源：http://nzg.xuetiantiany.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://asa.daria6918.cn

[S48] C++：逐行读文件
来源：http://seg.hammf.cn

std::ifstream in("a.txt");  std::string line;
来源：http://dxe.nanxinkj.top

while (std::getline(in, line)) { }
来源：http://qvd.shzxlz.cn

[S49] C++：写文件
来源：http://izp.yuxming.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vwa.cqqwz.cn

[S50] C++：格式化数字
来源：http://iag.hcnkem.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ely.yuanzhike.top

[S51] C++：显式类型转换
来源：http://buj.zhengqikj.top

static_cast<double>(a) / b
来源：http://puz.sjlbkw.cn

[S52] C++：const 与 noexcept
来源：http://bfp.snrcjt.cn

int size() const noexcept { return n_; }
来源：http://div.hcnkem.com

[S53] C++：移动语义
来源：http://gij.sufxvd.cn

std::vector<int> w = std::move(v);
来源：http://tji.yj20258.top

[S54] C++：异常处理
来源：http://bmk.ydzc1.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://oac.gogol.net.cn

[S55] C++：结构化绑定
来源：http://jdd.yongpay.top

auto [a, b] = std::make_pair(1, 2);
来源：http://teh.hammf.cn

[S56] C++：optional
来源：http://mgz.andypj.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fzi.52xcode.cn

[S57] C++：编译期常量
来源：http://rqn.svipenyu.cn

constexpr int N = 10;
来源：http://gsl.hcnkem.com

[S58] C++：命名空间
来源：http://cri.sweek.top

namespace ns { int f() { return 1; } }
来源：http://pfa.yuanzhike.top

[S59] C++：静态断言
来源：http://gpd.meibo888.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ece.shangyingyoupin.top

[S60] C++：遍历并删除元素
来源：http://yme.sxryk.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fve.yuxming.cn

================================================================================
来源：http://uhi.havefunace.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zrj.wangdashe.top

================================================================================
来源：http://qjb.yongpay.top

[T01] Kotlin：Hello World
来源：http://eii.shanyushiyangkeji.top

println("Hello")
来源：http://onj.fanxiaobao.xyz

[T02] Kotlin：变量
来源：http://kdk.iojbl.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zdh.wangshuangyany.cn

[T03] Kotlin：字符串模板
来源：http://hvw.jinyuanbaomall.cn

"值: $b"
来源：http://gmy.c1oappe.top

[T04] Kotlin：空安全
来源：http://ugi.bbcook.cn

val n: String? = null;  n?.length
来源：http://hks.bbcook.cn


<!-- 参考信息 -->