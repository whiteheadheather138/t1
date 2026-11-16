代发 wailian999

set -euo pipefail
来源：http://ylp.nwbrower.top

[R02] 变量赋值与使用
来源：http://ytp.ctjpmb.com

name="Tom"; echo "$name"
来源：http://pay.redwolf501.top

[R03] 只读变量
来源：http://txy.shuidangran.top

readonly PI=3.14
来源：http://epb.sxryk.cn

[R04] 位置参数
来源：http://aqt.pengpengdd.cyou

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fon.redwolf501.top

[R05] 参数默认值
来源：http://sar.jqgfzy.top

name="${1:-default}"
来源：http://xcx.guannengcc.top

[R06] 判断命令是否存在
来源：http://fge.shanyushiyangtech.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bnq.epnwcf.com

[R07] if 判断文件
来源：http://xex.jiagoushi.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vks.yuanzhike.top

[R08] 数值比较
来源：http://kcf.hammf.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://voa.hywenlv.cn

[R09] 字符串比较
来源：http://xfd.epnwcf.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gcl.birdmap.top

[R10] 正则匹配
来源：http://szb.xylfe.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://omv.pycfn.com

[R11] case 多分支
来源：http://jrl.havefunace.top

case "$1" in
来源：http://ywy.jqgufenzy.top

start) echo "启动" ;;
来源：http://snw.sweek.top

stop)  echo "停止" ;;
来源：http://jum.zycfv.cn

*)     echo "未知命令" ;;
来源：http://esr.zdqjudy.top

esac
来源：http://xan.snrcjt.cn

[R12] for 遍历文件
来源：http://vql.ehwqpu.com

for f in *.txt; do echo "$f"; done
来源：http://tef.chenzaomai.com

[R13] for 计数循环
来源：http://zwt.vqdsnc.cn

for i in {1..10}; do echo "$i"; done
来源：http://zfh.9152youxi.cn

[R14] C 风格 for
来源：http://rqa.hcnkem.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cwg.ehwqpu.com

[R15] while 逐行读文件
来源：http://rrw.jianghu66.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ztb.zhoulong.xyz

[R16] until 等待条件
来源：http://jpo.zycfv.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://usp.xziqi.cn

[R17] 数组定义与取值
来源：http://jjs.feifeiyinyue.top

arr=(a b c); echo "${arr[0]}"
来源：http://qoq.chenzaomai.com

[R18] 遍历数组
来源：http://uml.cdnleiting.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mxu.zhiwuduotai.top

[R19] 数组长度
来源：http://jbo.zhoulong.xyz

echo "${#arr[@]}"
来源：http://niq.wangdashe.top

[R20] 关联数组（字典）
来源：http://rmb.bbcook.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://koh.yj202588.top

[R21] 字符串长度
来源：http://ccc.xuanzx.com

echo "${#s}"
来源：http://zcj.hnqzz.top

[R22] 截取子串
来源：http://vgh.xylfe.cn

echo "${s:0:5}"
来源：http://qtr.tarul.cn

[R23] 字符串替换
来源：http://cny.xziqi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kcx.ivvv.top

[R24] 大小写转换
来源：http://nqd.jqgufenzy.top

echo "${s^^}"; echo "${s,,}"
来源：http://kax.yanxiufei.cn

[R25] 去后缀 / 去前缀
来源：http://bdf.nanxuanxn.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://cfm.sysykeji.top

[R26] 命令替换
来源：http://iwa.yj20258.top

now=$(date +%F); echo "$now"
来源：http://kie.zhaomingkeji.xyz

[R27] 算术展开
来源：http://oka.0kj1m.cn

echo $((1 + 2 * 3))
来源：http://ttt.uphjek.com

[R28] 浮点运算
来源：http://zbr.jinqigfzy.top

echo "scale=2; 10/3" | bc
来源：http://yjr.andypj.xyz

[R29] 定义函数
来源：http://mwn.yanxiufei.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://was.sysykeji.top

[R30] 函数返回状态码
来源：http://rmd.smart0.xyz

f() { return 0; }; f || echo "失败了"
来源：http://ycn.fengsongda.top

[R31] 局部变量
来源：http://xvr.wangshuangyany.cn

f() { local x=1; echo "$x"; }
来源：http://xkp.yj20258888.top

[R32] 参数个数校验
来源：http://wkl.zdqjudy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yhm.cheryme.top

[R33] 捕获错误并提示行号
来源：http://vfg.hcnkem.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uim.ivvv.top

[R34] 退出时清理
来源：http://pwf.andypj.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://ucq.nanxinkj.top

[R35] 后台执行并等待
来源：http://jue.guowangkeji.top

sleep 5 & pid=$!; wait "$pid"
来源：http://wva.tian-w.cn

[R36] 并发执行多个任务
来源：http://vyf.bjfxy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ruu.epnwcf.com

[R37] 把输出赋给变量
来源：http://yra.jqgfzy.top

files=$(ls -1)
来源：http://tuv.shanyushiyangtech.top

[R38] 管道串联
来源：http://uay.tian-w.cn

cat a.txt | grep -i error | wc -l
来源：http://dhd.hongshengwenyu.top

[R39] 重定向标准输出与错误
来源：http://nhg.chenlongwang.top

cmd > out.log 2>&1
来源：http://pvl.sweek.top

[R40] 追加写日志
来源：http://mje.epnwcf.com

echo "log" >> out.log
来源：http://zvx.jinqigfzy.top

[R41] 丢弃输出
来源：http://njk.zhoulong.xyz

cmd >/dev/null 2>&1
来源：http://hwt.jianghu66.top

[R42] 输入重定向
来源：http://tdd.fengsongda.top

wc -l < a.txt
来源：http://aej.cdnleiting.top

[R43] 按名字查找文件
来源：http://vtx.kuanghao11.cn

find . -name "*.log" -type f
来源：http://fcn.9152youxi.cn

[R44] 按修改时间查找
来源：http://ach.nanxuanxn.top

find . -mtime -7 -type f
来源：http://hno.nwbrower.top

[R45] 批量删除
来源：http://kqd.iojbl.cn

find . -name "*.tmp" -delete
来源：http://sfw.yueranfly.top

[R46] 递归替换文件内容
来源：http://ujm.shanyushiyangkeji.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ebj.dashuyun.cn

[R47] sed 单行替换
来源：http://mos.shanyushiyangkeji.top

sed -i 's/foo/bar/g' a.txt
来源：http://ncm.daria6918.cn

[R48] awk 取指定列
来源：http://chu.yangfankeji.com

awk '{print $1, $3}' a.txt
来源：http://kkk.sweek.top

[R49] awk 带条件
来源：http://cle.wangshuangyany.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vhp.shuidangran.top

[R50] awk 求和
来源：http://loa.bbcook.cn

awk '{s += $2} END {print s}' a.txt
来源：http://kvt.shuidangran.top

[R51] 排序去重取前几
来源：http://zld.tian-w.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://kjy.xuetiantiany.cn

[R52] 统计行数
来源：http://moq.mhx1999.top

wc -l a.txt
来源：http://mpu.nwbrower.top

[R53] 查看文件头与实时尾
来源：http://uhc.ivvv.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fmd.guannengcc.top

[R54] 比较两个文件
来源：http://xmw.jianghu66.top

diff a.txt b.txt
来源：http://xyn.quarkkingdee.top

[R55] 压缩与解压
来源：http://qld.yj20258.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vbp.xylfe.cn

[R56] 远程拷贝
来源：http://xey.feifeiyinyue.top

scp file user@host:/path/
来源：http://rtf.316326.xyz

[R57] 远程执行命令
来源：http://neg.cheryme.top

ssh user@host 'uptime'
来源：http://bpc.pycfn.com

[R58] 下载文件
来源：http://qys.nwbrower.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://plc.jqgfzy.top

[R59] 发 POST JSON
来源：http://nft.shuidangran.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gmt.zhixingplan.top

[R60] 只看 HTTP 状态码
来源：http://trz.haohaochexian.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://izk.316326.xyz

[R61] 磁盘占用
来源：http://hiq.c1oappe.top

df -h;  du -sh *
来源：http://urr.9152youxi.cn

[R62] 找最占空间的文件
来源：http://uva.wangshuangyany.cn

du -ah . | sort -rh | head -10
来源：http://blf.shanyushiyangtech.top

[R63] 内存与进程
来源：http://iaf.gaohongyu789.top

free -h;  ps aux | grep nginx
来源：http://rqb.0kj1m.cn

[R64] 结束进程
来源：http://fkf.chenzaomai.com

kill -9 $(pgrep -f app.py)
来源：http://pml.ydjk.org.cn

[R65] 查看端口占用
来源：http://ama.jqgufenzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://udg.guowangkeji.top

[R66] 定时任务
来源：http://lmq.shangyingyoupin.top

crontab -e;  crontab -l
来源：http://oyc.vehdjk.com

[R67] 生成随机十六进制串
来源：http://tyy.hcnkem.com

openssl rand -hex 16
来源：http://zrx.gotoacloud.top

[R68] 计算文件校验值
来源：http://nok.hnqzz.top

sha256sum a.txt;  md5sum a.txt
来源：http://bag.shuidangran.top

[R69] 生成随机密码
来源：http://rug.hongshengwenyu.top

head -c 16 /dev/urandom | base64
来源：http://erk.iojbl.cn

[R70] 时间戳与互转
来源：http://tnu.hcnkem.com

date +%s;  date -d @1700000000
来源：http://elt.zhiwuduotai.top

[R71] 日期格式化
来源：http://gio.sysykeji.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://oxi.sufxvd.cn

[R72] 等待端口就绪
来源：http://iwh.nwbrower.top

until nc -z localhost 3306; do sleep 1; done
来源：http://dsu.sufxvd.cn

[R73] 分割大日志
来源：http://aix.svipenyu.cn

split -l 1000 big.log part_
来源：http://ifx.hnqzz.top

[R74] 批量重命名
来源：http://erv.cashguo.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jde.yuxming.cn

[R75] 导出环境变量
来源：http://jvw.cheryme.top

export PATH="$HOME/bin:$PATH"
来源：http://sxe.smart0.xyz

[R76] 使用临时文件
来源：http://ftf.316326.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ghg.zhixingplan.top

[R77] 读取用户输入
来源：http://jnq.meibo888.top

read -rp "请输入: " ans
来源：http://bnp.gzhubu.top

[R78] 交互式菜单
来源：http://bdx.bbcook.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://buq.shangyingyoupin.top

[R79] 解析命令行选项
来源：http://bou.tarul.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ujz.guowangkeji.top

[R80] 查看脚本执行耗时
来源：http://nag.sweek.top

time ./run.sh
来源：http://wzc.jinqigufen.top

================================================================================
来源：http://njj.yj20258888.top

S. C / C++ 专题
来源：http://hlf.sweek.top

================================================================================
来源：http://csg.zhaomingkeji.xyz

[S01] C：Hello World
来源：http://eqm.hammf.cn

#include <stdio.h>
来源：http://ewa.jqgufenzy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://psh.zhaomingkeji.xyz

[S02] C：变量与格式化输出
来源：http://rft.vqdsnc.cn

int a = 10; printf("%d\n", a);
来源：http://kzw.ivvv.top

[S03] C：读入整数
来源：http://rgg.hywenlv.cn

int x; scanf("%d", &x);
来源：http://pth.xylfe.cn

[S04] C：字符串复制
来源：http://dni.meibo888.top

char dst[32]; strcpy(dst, "hi");
来源：http://bjl.wangdashe.top

[S05] C：字符串长度
来源：http://jpq.smart0.xyz

strlen(s)
来源：http://zxq.zhiwuduotai.top

[S06] C：字符串比较
来源：http://cnv.yangfankeji.com

strcmp(a, b) == 0
来源：http://dfb.ywan-chungtsiang.top

[S07] C：数组遍历求和
来源：http://ffl.zhiwuduotai.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://azo.ivvv.top

[S08] C：动态内存分配与释放
来源：http://rne.zhengqikj.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pmy.ydzc1.top

[S09] C：结构体定义与初始化
来源：http://jdf.bbcook.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://exs.52xcode.cn

[S10] C：指针与解引用
来源：http://zqj.wangshuangyany.cn

int *p = &a;  *p = 5;
来源：http://bla.cqqwz.cn

[S11] C：逐行读文件
来源：http://hku.jinghuilouyu.cn

FILE *f = fopen("a.txt", "r");
来源：http://oik.uphjek.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://gvj.wangshuangyany.cn

fclose(f);
来源：http://shs.hongshengwenyu.top

[S12] C：写文件
来源：http://xuc.c1oappe.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zaa.cashguo.top

[S13] C：宏定义
来源：http://nuo.ehwqpu.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://exi.jiagoushi.top

[S14] C：枚举
来源：http://gei.yangfankeji.com

enum Color { RED, GREEN, BLUE };
来源：http://foz.hywenlv.cn

[S15] C：类型转换
来源：http://nap.9152youxi.cn

(double) a / b
来源：http://fyz.ivvv.top

[S16] C：位操作置位
来源：http://kdc.smart0.xyz

x |= (1 << 3);
来源：http://ncd.shanyushiyangkeji.top

[S17] C：安全拼接字符串
来源：http://qcl.xuetiantiany.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mih.aibaodan.cn

[S18] C：命令行参数
来源：http://tev.sxryk.cn

int main(int argc, char **argv)
来源：http://gkq.tian-w.cn

[S19] C：快速排序
来源：http://scv.ppjwa.cn

qsort(a, n, sizeof(int), cmp);
来源：http://lll.jinqigfzy.top

[S20] C：二分查找
来源：http://zup.zhijiandao.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pkc.zhijiandao.cn

[S21] C：字符类别判断
来源：http://qvc.fzhhl.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://azk.hcnkem.com

[S22] C：字符串转数字
来源：http://gyf.bbcook.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cfu.dianchejie.cn

[S23] C：随机数
来源：http://rwo.xuetiantiany.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://trx.gogol.net.cn

[S24] C：获取本地时间
来源：http://lvx.xylfe.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ddb.fanxiaobao.xyz

[S25] C：内存拷贝
来源：http://sfk.sweek.top

memcpy(dst, src, n);
来源：http://eby.dashuyun.cn

[S26] C：内存清零
来源：http://vzy.meibo888.top

memset(a, 0, sizeof a);
来源：http://xap.0kj1m.cn

[S27] C：定义常量
来源：http://hhf.meibo888.top

const double PI = 3.14159;
来源：http://luk.gaohongyu789.top

[S28] C：静态变量
来源：http://hnb.smart0.xyz

static int counter = 0;
来源：http://vkl.jianghu66.top

[S29] C：变参函数
来源：http://wuh.jqgufenzy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://adu.andypj.xyz

[S30] C：头文件保护
来源：http://hqm.fanxiaobao.xyz

#ifndef X_H
来源：http://kpa.fanxiaobao.xyz

#define X_H
来源：http://zkf.zhijiandao.cn

#endif
来源：http://gzy.hcnkem.com

[S31] C++：Hello World
来源：http://sld.tanke756.top

#include <iostream>
来源：http://fel.xingfuxueyuan.xyz

int main() { std::cout << "Hello\n"; }
来源：http://jme.shanyushiyangtech.top

[S32] C++：字符串
来源：http://fci.hongshengwenyu.top

std::string s = "hi";  s += "!";
来源：http://dso.hfpthk.cn

[S33] C++：vector 增删
来源：http://vmp.xuetiantiany.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wrz.yfazqb.com

[S34] C++：遍历 vector
来源：http://utw.jinghuilouyu.cn

for (auto &x : v) { std::cout << x; }
来源：http://jin.hysaishi.cn

[S35] C++：map
来源：http://zot.hfpthk.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://usd.jinqigufen.top

[S36] C++：unordered_map
来源：http://ddw.aizwys.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hlc.shangyingyoupin.top

[S37] C++：set
来源：http://god.shangyingyoupin.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cpa.gaohongyu789.top

[S38] C++：排序
来源：http://dbe.quarkkingdee.top

std::sort(v.begin(), v.end());
来源：http://get.nwbrower.top

[S39] C++：自定义比较器排序
来源：http://ryg.dianchejie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bkp.haohaochexian.top

[S40] C++：查找元素
来源：http://nss.mhx1999.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pqk.gogol.net.cn

[S41] C++：类与构造函数
来源：http://nwg.ppjwa.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fjp.aizwys.cn

[S42] C++：继承与虚函数
来源：http://zwo.fengsongda.top

class B : public Base { public: void f() override {} };
来源：http://vrw.yj202588.top

[S43] C++：智能指针
来源：http://tir.sysykeji.top

auto p = std::make_unique<int>(5);
来源：http://qen.mhx1999.top

[S44] C++：引用传参
来源：http://kop.tian-w.cn

void inc(int &x) { ++x; }
来源：http://edf.c1oappe.top

[S45] C++：lambda
来源：http://pje.meibo888.top

auto add = [](int a, int b) { return a + b; };
来源：http://tju.hfpthk.cn

[S46] C++：函数模板
来源：http://htw.hcnkem.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ycz.bjfxy.top

[S47] C++：结构化绑定遍历
来源：http://nnu.yanxiufei.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cdi.sjlbkw.cn

[S48] C++：逐行读文件
来源：http://axy.yangfankeji.com

std::ifstream in("a.txt");  std::string line;
来源：http://qpl.ivvv.top

while (std::getline(in, line)) { }
来源：http://obe.chenzaomai.com

[S49] C++：写文件
来源：http://fav.tanke756.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nco.svipenyu.cn

[S50] C++：格式化数字
来源：http://pnj.nanxinkj.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yqn.fengsongda.top

[S51] C++：显式类型转换
来源：http://jxm.vqdsnc.cn

static_cast<double>(a) / b
来源：http://tkb.c1oappe.top

[S52] C++：const 与 noexcept
来源：http://wro.cucudq.cn

int size() const noexcept { return n_; }
来源：http://cvk.zhijiandao.cn

[S53] C++：移动语义
来源：http://lqs.jinghuilouyu.cn

std::vector<int> w = std::move(v);
来源：http://sqf.gogol.net.cn

[S54] C++：异常处理
来源：http://mzz.vqdsnc.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zjc.epnwcf.com

[S55] C++：结构化绑定
来源：http://kel.shzxlz.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://pjj.zhoulong.xyz

[S56] C++：optional
来源：http://wzj.shanyushiyangtech.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vns.hcnkem.com

[S57] C++：编译期常量
来源：http://ony.yanxiufei.cn

constexpr int N = 10;
来源：http://syp.zhijiandao.cn

[S58] C++：命名空间
来源：http://dfh.zhongyouzk.top

namespace ns { int f() { return 1; } }
来源：http://myh.fehbvm.com

[S59] C++：静态断言
来源：http://mlr.52xcode.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xfb.xziqi.cn

[S60] C++：遍历并删除元素
来源：http://kku.guowangkeji.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zby.sweek.top

================================================================================
来源：http://swo.shanyushiyangtech.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lzu.wangshuangyany.cn

================================================================================
来源：http://yrd.yj202588.top

[T01] Kotlin：Hello World
来源：http://zle.bbcook.cn

println("Hello")
来源：http://egf.feifeiyinyue.top

[T02] Kotlin：变量
来源：http://rio.bbcook.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qxn.sweek.top


<!-- 参考信息 -->