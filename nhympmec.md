代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://iot.nwbrower.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yls.haohaochexian.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qab.zhiwuduotai.top

[Q89] 判断表是否存在
来源：http://rai.cucudq.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qsz.yuanzhike.top

[Q90] 生成序号列
来源：http://mbn.nanxinkj.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nmv.zhixingplan.top

================================================================================
来源：http://mbn.yfazqb.com

R. Bash 专题
来源：http://ngb.jlsjyb.cn

================================================================================
来源：http://yyg.zhaomingkeji.xyz

[R01] shebang 与严格模式
来源：http://exs.tian-w.cn

#!/usr/bin/env bash
来源：http://elg.jinqigfzy.top

set -euo pipefail
来源：http://axg.andypj.xyz

[R02] 变量赋值与使用
来源：http://wge.xingfuxueyuan.xyz

name="Tom"; echo "$name"
来源：http://zxr.shangyingyoupin.top

[R03] 只读变量
来源：http://kpe.epnwcf.com

readonly PI=3.14
来源：http://cow.zdbjq.cn

[R04] 位置参数
来源：http://vvo.dashuyun.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mzl.iojbl.cn

[R05] 参数默认值
来源：http://jap.yongpay.top

name="${1:-default}"
来源：http://nye.zdqjudy.top

[R06] 判断命令是否存在
来源：http://bhp.iojbl.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qyt.yj20258.top

[R07] if 判断文件
来源：http://usf.hywenlv.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://beh.fengsongda.top

[R08] 数值比较
来源：http://pob.xziqi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://saf.nanxuanxn.top

[R09] 字符串比较
来源：http://vdh.ydjk.org.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pns.fengsongda.top

[R10] 正则匹配
来源：http://shq.havefunace.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dfn.pycfn.com

[R11] case 多分支
来源：http://bvm.shangyingyoupin.top

case "$1" in
来源：http://ykn.cheryme.top

start) echo "启动" ;;
来源：http://ebk.dianchejie.cn

stop)  echo "停止" ;;
来源：http://wau.yj20258888.top

*)     echo "未知命令" ;;
来源：http://sfq.jinqigfzy.top

esac
来源：http://bfn.bbcook.cn

[R12] for 遍历文件
来源：http://moz.gaohongyu789.top

for f in *.txt; do echo "$f"; done
来源：http://qxs.xziqi.cn

[R13] for 计数循环
来源：http://uzb.aizwys.cn

for i in {1..10}; do echo "$i"; done
来源：http://gtn.yj202588.top

[R14] C 风格 for
来源：http://kur.xylfe.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qzb.316326.xyz

[R15] while 逐行读文件
来源：http://hhc.kuanghao11.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jxn.zhaomingkeji.xyz

[R16] until 等待条件
来源：http://fvm.bjfxy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://euj.shzxlz.cn

[R17] 数组定义与取值
来源：http://mmp.yvedp.cn

arr=(a b c); echo "${arr[0]}"
来源：http://otg.ivvv.top

[R18] 遍历数组
来源：http://ohh.tianlin.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gda.birdmap.top

[R19] 数组长度
来源：http://uvf.0kj1m.cn

echo "${#arr[@]}"
来源：http://ihd.jiagoushi.top

[R20] 关联数组（字典）
来源：http://dqs.zhongyouzk.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yki.ywan-chungtsiang.top

[R21] 字符串长度
来源：http://gyb.quarkkingdee.top

echo "${#s}"
来源：http://wtd.zhiwuduotai.top

[R22] 截取子串
来源：http://drp.jinghuilouyu.cn

echo "${s:0:5}"
来源：http://enr.jyoumei.cn

[R23] 字符串替换
来源：http://ppu.dashuyun.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://udf.tanke756.top

[R24] 大小写转换
来源：http://bxd.epnwcf.com

echo "${s^^}"; echo "${s,,}"
来源：http://xml.mhx1999.top

[R25] 去后缀 / 去前缀
来源：http://vvo.chenlongwang.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://wwk.yonumen.top

[R26] 命令替换
来源：http://hbm.snrcjt.cn

now=$(date +%F); echo "$now"
来源：http://csp.sysykeji.top

[R27] 算术展开
来源：http://mmn.0kj1m.cn

echo $((1 + 2 * 3))
来源：http://sfy.gzhubu.top

[R28] 浮点运算
来源：http://lbq.jinqigufen.top

echo "scale=2; 10/3" | bc
来源：http://aan.yj202588.top

[R29] 定义函数
来源：http://uns.epnwcf.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rbr.52xcode.cn

[R30] 函数返回状态码
来源：http://guz.birdmap.top

f() { return 0; }; f || echo "失败了"
来源：http://hbf.0kj1m.cn

[R31] 局部变量
来源：http://afo.zhaomingkeji.xyz

f() { local x=1; echo "$x"; }
来源：http://ovi.pengpengdd.cyou

[R32] 参数个数校验
来源：http://hcs.gzhubu.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://arw.mhx1999.top

[R33] 捕获错误并提示行号
来源：http://xen.tian-w.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rvv.jinqigufen.top

[R34] 退出时清理
来源：http://tvu.yfazqb.com

trap 'rm -f "$tmp"' EXIT
来源：http://feg.hysaishi.cn

[R35] 后台执行并等待
来源：http://hzc.fehbvm.com

sleep 5 & pid=$!; wait "$pid"
来源：http://gqu.yj202588.top

[R36] 并发执行多个任务
来源：http://jod.hcnkem.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yhj.fktsv.cn

[R37] 把输出赋给变量
来源：http://vrc.nanxuanxn.top

files=$(ls -1)
来源：http://gyx.pycfn.com

[R38] 管道串联
来源：http://vdf.ppjwa.cn

cat a.txt | grep -i error | wc -l
来源：http://dtt.cheryme.top

[R39] 重定向标准输出与错误
来源：http://sjw.c1oappe.top

cmd > out.log 2>&1
来源：http://abs.sxryk.cn

[R40] 追加写日志
来源：http://zsy.gogol.net.cn

echo "log" >> out.log
来源：http://nae.xuanzx.com

[R41] 丢弃输出
来源：http://hdb.ydjk.org.cn

cmd >/dev/null 2>&1
来源：http://igc.zhongyouzk.top

[R42] 输入重定向
来源：http://uhx.jqgufenzy.top

wc -l < a.txt
来源：http://ltn.hfpthk.cn

[R43] 按名字查找文件
来源：http://qan.dashuyun.cn

find . -name "*.log" -type f
来源：http://kda.jqgufenzy.top

[R44] 按修改时间查找
来源：http://fqu.gzhubu.top

find . -mtime -7 -type f
来源：http://kfu.hnxiangtu.top

[R45] 批量删除
来源：http://cbg.pengpengdd.cyou

find . -name "*.tmp" -delete
来源：http://ofz.sweek.top

[R46] 递归替换文件内容
来源：http://aqp.bbcook.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dfn.mhx1999.top

[R47] sed 单行替换
来源：http://vmr.jianghu66.top

sed -i 's/foo/bar/g' a.txt
来源：http://ixx.shuidangran.top

[R48] awk 取指定列
来源：http://uau.wangshuangyany.cn

awk '{print $1, $3}' a.txt
来源：http://fsm.pengpengdd.cyou

[R49] awk 带条件
来源：http://kww.cqqwz.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hlv.shuidangran.top

[R50] awk 求和
来源：http://bwj.yj202588.top

awk '{s += $2} END {print s}' a.txt
来源：http://fts.hywenlv.cn

[R51] 排序去重取前几
来源：http://blk.quarkkingdee.top

sort a.txt | uniq -c | sort -rn | head
来源：http://fkn.gzhubu.top

[R52] 统计行数
来源：http://tco.c1oappe.top

wc -l a.txt
来源：http://mlf.9152youxi.cn

[R53] 查看文件头与实时尾
来源：http://zbx.fzhhl.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wdd.yvedp.cn

[R54] 比较两个文件
来源：http://nbq.kuanghao11.cn

diff a.txt b.txt
来源：http://egd.quarkkingdee.top

[R55] 压缩与解压
来源：http://dea.nanxuanxn.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bjt.cashguo.top

[R56] 远程拷贝
来源：http://rja.hywenlv.cn

scp file user@host:/path/
来源：http://brt.yangfankeji.com

[R57] 远程执行命令
来源：http://rny.zhiwuduotai.top

ssh user@host 'uptime'
来源：http://lzo.hywenlv.cn

[R58] 下载文件
来源：http://cwm.zhaomingkeji.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wvl.zdqjudy.top

[R59] 发 POST JSON
来源：http://kcw.yueranfly.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://flv.daria6918.cn

[R60] 只看 HTTP 状态码
来源：http://ruo.vehdjk.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ujc.shanyushiyangtech.top

[R61] 磁盘占用
来源：http://szj.zhengqikj.top

df -h;  du -sh *
来源：http://cuj.aizwys.cn

[R62] 找最占空间的文件
来源：http://tju.zhengqikj.top

du -ah . | sort -rh | head -10
来源：http://xpp.wangdashe.top

[R63] 内存与进程
来源：http://odh.gogol.net.cn

free -h;  ps aux | grep nginx
来源：http://evs.tian-w.cn

[R64] 结束进程
来源：http://zip.sufxvd.cn

kill -9 $(pgrep -f app.py)
来源：http://lfg.hfpthk.cn

[R65] 查看端口占用
来源：http://oyb.ivvv.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vlr.52xcode.cn

[R66] 定时任务
来源：http://ykk.wangdashe.top

crontab -e;  crontab -l
来源：http://oqp.sufxvd.cn

[R67] 生成随机十六进制串
来源：http://mrd.jqgufenzy.top

openssl rand -hex 16
来源：http://smd.tianlin.xyz

[R68] 计算文件校验值
来源：http://yrz.jqgufenzy.top

sha256sum a.txt;  md5sum a.txt
来源：http://qso.zhoulong.xyz

[R69] 生成随机密码
来源：http://omw.yueranfly.top

head -c 16 /dev/urandom | base64
来源：http://dhp.haohaochexian.top

[R70] 时间戳与互转
来源：http://ubc.xinyue.icu

date +%s;  date -d @1700000000
来源：http://bek.cashguo.top

[R71] 日期格式化
来源：http://hxc.316326.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://hti.fzhhl.top

[R72] 等待端口就绪
来源：http://nos.fzhhl.top

until nc -z localhost 3306; do sleep 1; done
来源：http://vha.gotoacloud.top

[R73] 分割大日志
来源：http://fzs.jianghu66.top

split -l 1000 big.log part_
来源：http://rqg.yj20258888.top

[R74] 批量重命名
来源：http://mce.ydzc1.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://syt.iojbl.cn

[R75] 导出环境变量
来源：http://epz.jqgfzy.top

export PATH="$HOME/bin:$PATH"
来源：http://elp.yangfankeji.com

[R76] 使用临时文件
来源：http://nqi.sufxvd.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pww.52xcode.cn

[R77] 读取用户输入
来源：http://eiz.pengpengdd.cyou

read -rp "请输入: " ans
来源：http://xuy.hammf.cn

[R78] 交互式菜单
来源：http://xdc.cheryme.top

select opt in a b c; do echo "$opt"; break; done
来源：http://qnk.wangshuangyany.cn

[R79] 解析命令行选项
来源：http://urb.pengpengdd.cyou

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uob.chenjidiqi.icu

[R80] 查看脚本执行耗时
来源：http://zlo.hongshengwenyu.top

time ./run.sh
来源：http://wxy.zhoulong.xyz

================================================================================
来源：http://jur.xziqi.cn

S. C / C++ 专题
来源：http://wmb.zhongyouzk.top

================================================================================
来源：http://bsk.yongpay.top

[S01] C：Hello World
来源：http://wqu.shangyingyoupin.top

#include <stdio.h>
来源：http://ymq.hcnkem.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://rkb.sufxvd.cn

[S02] C：变量与格式化输出
来源：http://xjt.yangfankeji.com

int a = 10; printf("%d\n", a);
来源：http://ykx.guowangkeji.top

[S03] C：读入整数
来源：http://gfs.wangshuangyany.cn

int x; scanf("%d", &x);
来源：http://euj.chenzaomai.com

[S04] C：字符串复制
来源：http://khw.kuanghao11.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ygo.fzhhl.top

[S05] C：字符串长度
来源：http://ocd.zdbjq.cn

strlen(s)
来源：http://oyt.zhoulong.xyz

[S06] C：字符串比较
来源：http://fmv.zhoulong.xyz

strcmp(a, b) == 0
来源：http://ucv.fengsongda.top

[S07] C：数组遍历求和
来源：http://cpw.aizwys.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qtp.chenzaomai.com

[S08] C：动态内存分配与释放
来源：http://ols.dianchejie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hjd.sxryk.cn

[S09] C：结构体定义与初始化
来源：http://utl.jinqigufen.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xru.meibo888.top

[S10] C：指针与解引用
来源：http://vgs.fehbvm.com

int *p = &a;  *p = 5;
来源：http://deb.jinghuilouyu.cn

[S11] C：逐行读文件
来源：http://qtq.kuanghao11.cn

FILE *f = fopen("a.txt", "r");
来源：http://ebm.yuanzhike.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://xfd.yangfankeji.com

fclose(f);
来源：http://itv.vehdjk.com

[S12] C：写文件
来源：http://xwq.meibo888.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://aot.aizwys.cn

[S13] C：宏定义
来源：http://smt.meibo888.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mpk.haohaochexian.top

[S14] C：枚举
来源：http://wha.shangyingyoupin.top

enum Color { RED, GREEN, BLUE };
来源：http://jjv.316326.xyz

[S15] C：类型转换
来源：http://fhr.ehwqpu.com

(double) a / b
来源：http://zzo.ppjwa.cn

[S16] C：位操作置位
来源：http://fiw.nwbrower.top

x |= (1 << 3);
来源：http://gow.xingfuxueyuan.xyz

[S17] C：安全拼接字符串
来源：http://giv.zhongyouzk.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hpv.chenjidiqi.icu

[S18] C：命令行参数
来源：http://enw.yangfankeji.com

int main(int argc, char **argv)
来源：http://djw.hfpthk.cn

[S19] C：快速排序
来源：http://nsl.tianlin.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://dub.aibaodan.cn

[S20] C：二分查找
来源：http://idd.aibaodan.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://eiv.zhaomingkeji.xyz

[S21] C：字符类别判断
来源：http://voa.jinghuilouyu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sup.yonumen.top

[S22] C：字符串转数字
来源：http://tfx.aizwys.cn

atoi("42");  strtod("3.14", NULL);
来源：http://pjr.xinyue.icu

[S23] C：随机数
来源：http://rfx.aizwys.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bae.shangyingyoupin.top

[S24] C：获取本地时间
来源：http://cgv.cashguo.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jso.hywenlv.cn

[S25] C：内存拷贝
来源：http://yam.sxryk.cn

memcpy(dst, src, n);
来源：http://moi.xinyue.icu

[S26] C：内存清零
来源：http://eam.tian-w.cn

memset(a, 0, sizeof a);
来源：http://hac.daria6918.cn

[S27] C：定义常量
来源：http://xuu.yj20258.top

const double PI = 3.14159;
来源：http://eth.kuanghao11.cn

[S28] C：静态变量
来源：http://ibp.xuanzx.com

static int counter = 0;
来源：http://tov.jqgfzy.top

[S29] C：变参函数
来源：http://qxi.yj202588.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gpo.uphjek.com

[S30] C：头文件保护
来源：http://pmo.bjfxy.top

#ifndef X_H
来源：http://ute.zhoulong.xyz

#define X_H
来源：http://ule.xuetiantiany.cn

#endif
来源：http://gof.dashuyun.cn

[S31] C++：Hello World
来源：http://sgq.zhiwuduotai.top

#include <iostream>
来源：http://xyc.xuetiantiany.cn

int main() { std::cout << "Hello\n"; }
来源：http://the.mhx1999.top

[S32] C++：字符串
来源：http://dre.aibaodan.cn

std::string s = "hi";  s += "!";
来源：http://ava.uphjek.com

[S33] C++：vector 增删
来源：http://rte.zycfv.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ohv.shanyushiyangtech.top

[S34] C++：遍历 vector
来源：http://cyk.zhongyouzk.top

for (auto &x : v) { std::cout << x; }
来源：http://obc.zdqjudy.top

[S35] C++：map
来源：http://rac.zycfv.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vjq.sweek.top

[S36] C++：unordered_map
来源：http://pio.kuanghao11.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://prg.gotoacloud.top

[S37] C++：set
来源：http://lrx.jqgufenzy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fej.vehdjk.com

[S38] C++：排序
来源：http://sna.shzxlz.cn

std::sort(v.begin(), v.end());
来源：http://ktd.guannengcc.top

[S39] C++：自定义比较器排序
来源：http://igv.jinqigufen.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://oko.aibaodan.cn

[S40] C++：查找元素
来源：http://ukv.haohaochexian.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jov.ppjwa.cn

[S41] C++：类与构造函数
来源：http://vvi.52xcode.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ztl.dianchejie.cn

[S42] C++：继承与虚函数
来源：http://yjo.hongshengwenyu.top

class B : public Base { public: void f() override {} };
来源：http://jfl.dashuyun.cn

[S43] C++：智能指针
来源：http://paw.yangfankeji.com

auto p = std::make_unique<int>(5);
来源：http://amk.jiagoushi.top

[S44] C++：引用传参
来源：http://pxz.cheryme.top

void inc(int &x) { ++x; }
来源：http://rwl.shzxlz.cn

[S45] C++：lambda
来源：http://kyf.tarul.cn

auto add = [](int a, int b) { return a + b; };
来源：http://kqr.zhaomingkeji.xyz

[S46] C++：函数模板
来源：http://qcg.yuanzhike.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rvj.uphjek.com

[S47] C++：结构化绑定遍历
来源：http://myp.shuidangran.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ins.hfpthk.cn

[S48] C++：逐行读文件
来源：http://ifo.shanyushiyangtech.top

std::ifstream in("a.txt");  std::string line;
来源：http://scb.jianghu66.top

while (std::getline(in, line)) { }
来源：http://xab.uphjek.com

[S49] C++：写文件
来源：http://yrm.shangyingyoupin.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pmc.daria6918.cn

[S50] C++：格式化数字
来源：http://huy.shanyushiyangtech.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bqp.yonumen.top

[S51] C++：显式类型转换
来源：http://cji.shangyingyoupin.top

static_cast<double>(a) / b
来源：http://qff.yj20258888.top

[S52] C++：const 与 noexcept
来源：http://kpo.gotoacloud.top

int size() const noexcept { return n_; }
来源：http://wrm.cqqwz.cn

[S53] C++：移动语义
来源：http://dtm.snrcjt.cn

std::vector<int> w = std::move(v);
来源：http://xkq.yvedp.cn

[S54] C++：异常处理
来源：http://lse.shangyingyoupin.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tyj.yuanzhike.top

[S55] C++：结构化绑定
来源：http://ruc.zhoulong.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://uew.redwolf501.top

[S56] C++：optional
来源：http://mdu.ehwqpu.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nxz.zhongyouzk.top

[S57] C++：编译期常量
来源：http://dkn.ybcxt.top

constexpr int N = 10;
来源：http://ysi.snrcjt.cn

[S58] C++：命名空间
来源：http://kbk.mhx1999.top


<!-- 参考信息 -->