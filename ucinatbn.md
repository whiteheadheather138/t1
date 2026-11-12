代发 wailian999

R. Bash 专题
来源：http://lku.snrcjt.cn

================================================================================
来源：http://gwu.tarul.cn

[R01] shebang 与严格模式
来源：http://ebc.sjlbkw.cn

#!/usr/bin/env bash
来源：http://pra.zhiwuduotai.top

set -euo pipefail
来源：http://gdp.chenzaomai.com

[R02] 变量赋值与使用
来源：http://lde.quarkkingdee.top

name="Tom"; echo "$name"
来源：http://ixs.vehdjk.com

[R03] 只读变量
来源：http://tdo.zdqjudy.top

readonly PI=3.14
来源：http://zxi.hnxiangtu.top

[R04] 位置参数
来源：http://quv.haohaochexian.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dez.yonumen.top

[R05] 参数默认值
来源：http://kcn.xuetiantiany.cn

name="${1:-default}"
来源：http://udv.hnqzz.top

[R06] 判断命令是否存在
来源：http://uvs.shangyingyoupin.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nfy.ywan-chungtsiang.top

[R07] if 判断文件
来源：http://xjp.havefunace.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://afa.hongshengwenyu.top

[R08] 数值比较
来源：http://tan.havefunace.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ukv.shanyushiyangtech.top

[R09] 字符串比较
来源：http://xxp.xinyue.icu

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bjf.guannengcc.top

[R10] 正则匹配
来源：http://bmy.pycfn.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mhq.yuxming.cn

[R11] case 多分支
来源：http://wwp.havefunace.top

case "$1" in
来源：http://bgo.nanxinkj.top

start) echo "启动" ;;
来源：http://gmz.xuetiantiany.cn

stop)  echo "停止" ;;
来源：http://syy.jinqigufen.top

*)     echo "未知命令" ;;
来源：http://tqi.aibaodan.cn

esac
来源：http://frg.feifeiyinyue.top

[R12] for 遍历文件
来源：http://gsu.gogol.net.cn

for f in *.txt; do echo "$f"; done
来源：http://iak.cucudq.cn

[R13] for 计数循环
来源：http://dbb.hongshengwenyu.top

for i in {1..10}; do echo "$i"; done
来源：http://nvt.tianlin.xyz

[R14] C 风格 for
来源：http://tax.redwolf501.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wmd.nwbrower.top

[R15] while 逐行读文件
来源：http://aet.hysaishi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://msu.tarul.cn

[R16] until 等待条件
来源：http://qpk.hesvh.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jsl.cqqwz.cn

[R17] 数组定义与取值
来源：http://mhh.snrcjt.cn

arr=(a b c); echo "${arr[0]}"
来源：http://flz.xylfe.cn

[R18] 遍历数组
来源：http://jgr.sxryk.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mwu.jiagoushi.top

[R19] 数组长度
来源：http://uet.shanyushiyangtech.top

echo "${#arr[@]}"
来源：http://yvr.zhixingplan.top

[R20] 关联数组（字典）
来源：http://haz.jiagoushi.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bfe.svipenyu.cn

[R21] 字符串长度
来源：http://udr.jqgufenzy.top

echo "${#s}"
来源：http://kjy.jlsjyb.cn

[R22] 截取子串
来源：http://dli.nanxinkj.top

echo "${s:0:5}"
来源：http://kod.jqgufenzy.top

[R23] 字符串替换
来源：http://rur.jqgufenzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://swr.zhengqikj.top

[R24] 大小写转换
来源：http://orv.yanxiufei.cn

echo "${s^^}"; echo "${s,,}"
来源：http://wup.zhiwuduotai.top

[R25] 去后缀 / 去前缀
来源：http://dqs.jianghu66.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://sco.nwbrower.top

[R26] 命令替换
来源：http://uyj.hesvh.cn

now=$(date +%F); echo "$now"
来源：http://dfi.yfazqb.com

[R27] 算术展开
来源：http://vsl.hammf.cn

echo $((1 + 2 * 3))
来源：http://tvw.quarkkingdee.top

[R28] 浮点运算
来源：http://sfl.ydjk.org.cn

echo "scale=2; 10/3" | bc
来源：http://cja.cqqwz.cn

[R29] 定义函数
来源：http://yze.cucudq.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zjp.jinghuilouyu.cn

[R30] 函数返回状态码
来源：http://tfj.yj20258888.top

f() { return 0; }; f || echo "失败了"
来源：http://jcg.yueranfly.top

[R31] 局部变量
来源：http://ccx.tarul.cn

f() { local x=1; echo "$x"; }
来源：http://qik.aibaodan.cn

[R32] 参数个数校验
来源：http://srw.daria6918.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bgw.jiagoushi.top

[R33] 捕获错误并提示行号
来源：http://ooa.jinyuanbaomall.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fea.chenzaomai.com

[R34] 退出时清理
来源：http://cnc.shangyingyoupin.top

trap 'rm -f "$tmp"' EXIT
来源：http://qkr.xingfuxueyuan.xyz

[R35] 后台执行并等待
来源：http://fci.uphjek.com

sleep 5 & pid=$!; wait "$pid"
来源：http://gro.zhongyouzk.top

[R36] 并发执行多个任务
来源：http://eya.pycfn.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hbo.xinyue.icu

[R37] 把输出赋给变量
来源：http://flo.shzxlz.cn

files=$(ls -1)
来源：http://dev.jinqigfzy.top

[R38] 管道串联
来源：http://wuu.yfazqb.com

cat a.txt | grep -i error | wc -l
来源：http://zso.cdnleiting.top

[R39] 重定向标准输出与错误
来源：http://hnq.cqqwz.cn

cmd > out.log 2>&1
来源：http://kuq.pycfn.com

[R40] 追加写日志
来源：http://kfl.guannengcc.top

echo "log" >> out.log
来源：http://zwy.xziqi.cn

[R41] 丢弃输出
来源：http://gnp.jinqigufen.top

cmd >/dev/null 2>&1
来源：http://ydy.hywenlv.cn

[R42] 输入重定向
来源：http://bvq.jqgufenzy.top

wc -l < a.txt
来源：http://fjl.cucudq.cn

[R43] 按名字查找文件
来源：http://svw.fzhhl.top

find . -name "*.log" -type f
来源：http://frd.jinyuanbaomall.cn

[R44] 按修改时间查找
来源：http://irg.cdnleiting.top

find . -mtime -7 -type f
来源：http://uwz.hesvh.cn

[R45] 批量删除
来源：http://tma.cashguo.top

find . -name "*.tmp" -delete
来源：http://gmc.havefunace.top

[R46] 递归替换文件内容
来源：http://cco.cashguo.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tmh.snrcjt.cn

[R47] sed 单行替换
来源：http://bzx.sufxvd.cn

sed -i 's/foo/bar/g' a.txt
来源：http://rig.zhongyouzk.top

[R48] awk 取指定列
来源：http://ika.jlsjyb.cn

awk '{print $1, $3}' a.txt
来源：http://poc.epnwcf.com

[R49] awk 带条件
来源：http://pyy.feifeiyinyue.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bau.hfpthk.cn

[R50] awk 求和
来源：http://jmv.zhongyouzk.top

awk '{s += $2} END {print s}' a.txt
来源：http://xlh.jinqigufen.top

[R51] 排序去重取前几
来源：http://zyf.guannengcc.top

sort a.txt | uniq -c | sort -rn | head
来源：http://msq.xuetiantiany.cn

[R52] 统计行数
来源：http://jkl.vqdsnc.cn

wc -l a.txt
来源：http://rym.cdnleiting.top

[R53] 查看文件头与实时尾
来源：http://ykb.hesvh.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ram.jlsjyb.cn

[R54] 比较两个文件
来源：http://ckp.xuanzx.com

diff a.txt b.txt
来源：http://ebc.tarul.cn

[R55] 压缩与解压
来源：http://kxs.zhoulong.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tpl.c1oappe.top

[R56] 远程拷贝
来源：http://wdn.cqqwz.cn

scp file user@host:/path/
来源：http://nau.snrcjt.cn

[R57] 远程执行命令
来源：http://jwm.daxiang520.top

ssh user@host 'uptime'
来源：http://hpx.zhiwuduotai.top

[R58] 下载文件
来源：http://cfq.yanxiufei.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://brx.zhongyouzk.top

[R59] 发 POST JSON
来源：http://ryy.yuanzhike.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qut.ydjk.org.cn

[R60] 只看 HTTP 状态码
来源：http://vhx.hfpthk.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ztj.shzxlz.cn

[R61] 磁盘占用
来源：http://phh.316326.xyz

df -h;  du -sh *
来源：http://nef.iojbl.cn

[R62] 找最占空间的文件
来源：http://mxs.yongpay.top

du -ah . | sort -rh | head -10
来源：http://qeo.haohaochexian.top

[R63] 内存与进程
来源：http://ahh.jqgfzy.top

free -h;  ps aux | grep nginx
来源：http://rui.daria6918.cn

[R64] 结束进程
来源：http://zen.xuetiantiany.cn

kill -9 $(pgrep -f app.py)
来源：http://rps.pycfn.com

[R65] 查看端口占用
来源：http://qqk.xingfuxueyuan.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ygb.hammf.cn

[R66] 定时任务
来源：http://ssp.jiagoushi.top

crontab -e;  crontab -l
来源：http://qev.havefunace.top

[R67] 生成随机十六进制串
来源：http://bmq.aizwys.cn

openssl rand -hex 16
来源：http://xwv.vqdsnc.cn

[R68] 计算文件校验值
来源：http://gyd.gaohongyu789.top

sha256sum a.txt;  md5sum a.txt
来源：http://ktb.daria6918.cn

[R69] 生成随机密码
来源：http://wnw.pengpengdd.cyou

head -c 16 /dev/urandom | base64
来源：http://igu.tianlin.xyz

[R70] 时间戳与互转
来源：http://vrw.vqdsnc.cn

date +%s;  date -d @1700000000
来源：http://lrh.9152youxi.cn

[R71] 日期格式化
来源：http://qnm.kuanghao11.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://tcx.fengsongda.top

[R72] 等待端口就绪
来源：http://icy.guowangkeji.top

until nc -z localhost 3306; do sleep 1; done
来源：http://suu.guannengcc.top

[R73] 分割大日志
来源：http://gie.havefunace.top

split -l 1000 big.log part_
来源：http://rls.hongshengwenyu.top

[R74] 批量重命名
来源：http://fhu.fanxiaobao.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gdw.sjlbkw.cn

[R75] 导出环境变量
来源：http://qhv.c1oappe.top

export PATH="$HOME/bin:$PATH"
来源：http://pkk.9152youxi.cn

[R76] 使用临时文件
来源：http://iqu.pycfn.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zlm.ehwqpu.com

[R77] 读取用户输入
来源：http://hql.tian-w.cn

read -rp "请输入: " ans
来源：http://qew.316326.xyz

[R78] 交互式菜单
来源：http://wlj.52xcode.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zbs.bjfxy.top

[R79] 解析命令行选项
来源：http://vim.gaohongyu789.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pwh.yj20258888.top

[R80] 查看脚本执行耗时
来源：http://ezy.bjfxy.top

time ./run.sh
来源：http://fzr.smart0.xyz

================================================================================
来源：http://uoq.hammf.cn

S. C / C++ 专题
来源：http://fkt.guowangkeji.top

================================================================================
来源：http://cnh.hongshengwenyu.top

[S01] C：Hello World
来源：http://gez.zhengqikj.top

#include <stdio.h>
来源：http://rre.zhoulong.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://gnv.shzxlz.cn

[S02] C：变量与格式化输出
来源：http://hxg.snrcjt.cn

int a = 10; printf("%d\n", a);
来源：http://eyk.52xcode.cn

[S03] C：读入整数
来源：http://fww.gotoacloud.top

int x; scanf("%d", &x);
来源：http://qea.aibaodan.cn

[S04] C：字符串复制
来源：http://lda.sufxvd.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gpd.nanxuanxn.top

[S05] C：字符串长度
来源：http://yma.ywan-chungtsiang.top

strlen(s)
来源：http://rwa.xingfuxueyuan.xyz

[S06] C：字符串比较
来源：http://umo.pengpengdd.cyou

strcmp(a, b) == 0
来源：http://fvl.birdmap.top

[S07] C：数组遍历求和
来源：http://jks.hfpthk.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kcc.fengsongda.top

[S08] C：动态内存分配与释放
来源：http://xyd.cheryme.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://euw.jinyuanbaomall.cn

[S09] C：结构体定义与初始化
来源：http://nwc.jqgfzy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://aeu.sweek.top

[S10] C：指针与解引用
来源：http://vrx.pycfn.com

int *p = &a;  *p = 5;
来源：http://hbz.dashuyun.cn

[S11] C：逐行读文件
来源：http://uwg.daria6918.cn

FILE *f = fopen("a.txt", "r");
来源：http://mag.haohaochexian.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://cji.shanyushiyangkeji.top

fclose(f);
来源：http://efk.meibo888.top

[S12] C：写文件
来源：http://krc.zhongyouzk.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sfv.nwbrower.top

[S13] C：宏定义
来源：http://frs.yonumen.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kzj.xuetiantiany.cn

[S14] C：枚举
来源：http://lrw.zhijiandao.cn

enum Color { RED, GREEN, BLUE };
来源：http://jow.cucudq.cn

[S15] C：类型转换
来源：http://cze.nanxuanxn.top

(double) a / b
来源：http://wwh.hfpthk.cn

[S16] C：位操作置位
来源：http://ohx.quarkkingdee.top

x |= (1 << 3);
来源：http://jdv.nanxinkj.top

[S17] C：安全拼接字符串
来源：http://jyb.bjfxy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://woz.hywenlv.cn

[S18] C：命令行参数
来源：http://amm.jqgufenzy.top

int main(int argc, char **argv)
来源：http://lvg.mhx1999.top

[S19] C：快速排序
来源：http://erz.uphjek.com

qsort(a, n, sizeof(int), cmp);
来源：http://fdj.yanxiufei.cn

[S20] C：二分查找
来源：http://xqj.zycfv.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bje.jinqigfzy.top

[S21] C：字符类别判断
来源：http://txu.pycfn.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xrd.zhengqikj.top

[S22] C：字符串转数字
来源：http://qif.tianlin.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://vmz.chenjidiqi.icu

[S23] C：随机数
来源：http://twr.iojbl.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kro.zhiwuduotai.top

[S24] C：获取本地时间
来源：http://hia.yonumen.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mfm.zdbjq.cn

[S25] C：内存拷贝
来源：http://kjo.hywenlv.cn

memcpy(dst, src, n);
来源：http://dqy.guowangkeji.top

[S26] C：内存清零
来源：http://rnp.hywenlv.cn

memset(a, 0, sizeof a);
来源：http://zjd.chenlongwang.top

[S27] C：定义常量
来源：http://pff.ctjpmb.com

const double PI = 3.14159;
来源：http://kjy.tarul.cn

[S28] C：静态变量
来源：http://ihc.sxryk.cn

static int counter = 0;
来源：http://ccj.yvedp.cn

[S29] C：变参函数
来源：http://dru.cdnleiting.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ine.nanxuanxn.top

[S30] C：头文件保护
来源：http://fvx.aizwys.cn

#ifndef X_H
来源：http://pow.ehwqpu.com

#define X_H
来源：http://tmy.uphjek.com

#endif
来源：http://jkm.bjfxy.top

[S31] C++：Hello World
来源：http://olt.zycfv.cn

#include <iostream>
来源：http://hco.andypj.xyz

int main() { std::cout << "Hello\n"; }
来源：http://yop.vqdsnc.cn

[S32] C++：字符串
来源：http://fzz.pengpengdd.cyou

std::string s = "hi";  s += "!";
来源：http://bhi.chenzaomai.com

[S33] C++：vector 增删
来源：http://emo.c1oappe.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://khv.gzhubu.top

[S34] C++：遍历 vector
来源：http://scj.shuidangran.top

for (auto &x : v) { std::cout << x; }
来源：http://osi.jinqigfzy.top

[S35] C++：map
来源：http://msf.chenlongwang.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://evu.nanxinkj.top

[S36] C++：unordered_map
来源：http://bwn.fanxiaobao.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wea.uphjek.com

[S37] C++：set
来源：http://mef.xingfuxueyuan.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vmn.hesvh.cn

[S38] C++：排序
来源：http://riu.fengsongda.top

std::sort(v.begin(), v.end());
来源：http://mze.52xcode.cn

[S39] C++：自定义比较器排序
来源：http://zpt.cucudq.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hgf.shanyushiyangtech.top

[S40] C++：查找元素
来源：http://div.ivvv.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ujn.zdqjudy.top

[S41] C++：类与构造函数
来源：http://msj.zhongyouzk.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://chp.zdqjudy.top

[S42] C++：继承与虚函数
来源：http://bnr.cheryme.top

class B : public Base { public: void f() override {} };
来源：http://tli.sweek.top

[S43] C++：智能指针
来源：http://jgn.uphjek.com

auto p = std::make_unique<int>(5);
来源：http://xgv.ivvv.top

[S44] C++：引用传参
来源：http://oto.meibo888.top

void inc(int &x) { ++x; }
来源：http://xcz.xuetiantiany.cn

[S45] C++：lambda
来源：http://sep.hywenlv.cn

auto add = [](int a, int b) { return a + b; };
来源：http://age.dashuyun.cn

[S46] C++：函数模板
来源：http://mtk.fengsongda.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uru.xuetiantiany.cn

[S47] C++：结构化绑定遍历
来源：http://klb.bbcook.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jxj.hesvh.cn

[S48] C++：逐行读文件
来源：http://hsv.birdmap.top

std::ifstream in("a.txt");  std::string line;
来源：http://ydb.quarkkingdee.top

while (std::getline(in, line)) { }
来源：http://mmb.ehwqpu.com

[S49] C++：写文件
来源：http://rdj.fzhhl.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ylo.nanxinkj.top

[S50] C++：格式化数字
来源：http://lej.zhengqikj.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vuy.shuidangran.top

[S51] C++：显式类型转换
来源：http://zwh.shanyushiyangtech.top

static_cast<double>(a) / b
来源：http://qfm.cheryme.top

[S52] C++：const 与 noexcept
来源：http://yrm.0kj1m.cn

int size() const noexcept { return n_; }
来源：http://qfq.ppjwa.cn

[S53] C++：移动语义
来源：http://lpr.birdmap.top

std::vector<int> w = std::move(v);
来源：http://lxg.nwbrower.top

[S54] C++：异常处理
来源：http://jko.yueranfly.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qbb.fanxiaobao.xyz

[S55] C++：结构化绑定
来源：http://tji.c1oappe.top

auto [a, b] = std::make_pair(1, 2);
来源：http://fxd.nwbrower.top

[S56] C++：optional
来源：http://hdq.yueranfly.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fcq.xinyue.icu

[S57] C++：编译期常量
来源：http://nbn.ydzc1.top

constexpr int N = 10;
来源：http://txl.dashuyun.cn

[S58] C++：命名空间
来源：http://qyl.cqqwz.cn

namespace ns { int f() { return 1; } }
来源：http://oex.9152youxi.cn

[S59] C++：静态断言
来源：http://mhk.fzhhl.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zcn.chenlongwang.top

[S60] C++：遍历并删除元素
来源：http://vay.sufxvd.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://frr.tarul.cn

================================================================================
来源：http://wqu.mhx1999.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mks.hnqzz.top

================================================================================
来源：http://omm.ehwqpu.com


<!-- 参考信息 -->